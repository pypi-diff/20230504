# Comparing `tmp/alacorder-80.2.1.tar.gz` & `tmp/alacorder-80.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.2.1.tar", max compression
+gzip compressed data, was "alacorder-80.2.2.tar", max compression
```

## Comparing `alacorder-80.2.1.tar` & `alacorder-80.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.1/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.1/README.md
--rw-r--r--   0        0        0      697 2023-05-04 17:24:01.914633 alacorder-80.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   215919 2023-05-04 17:23:45.877548 alacorder-80.2.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   215919 2023-05-04 17:23:41.277004 alacorder-80.2.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.2/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.2/README.md
+-rw-r--r--   0        0        0      697 2023-05-04 17:45:17.811797 alacorder-80.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.2/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   213003 2023-05-04 17:44:09.990203 alacorder-80.2.2/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   213003 2023-05-04 17:44:03.464820 alacorder-80.2.2/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.2/PKG-INFO
```

### Comparing `alacorder-80.2.1/LICENSE` & `alacorder-80.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.1/README.md` & `alacorder-80.2.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.1/pyproject.toml` & `alacorder-80.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.2.1"
+version = "80.2.2"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.2.1/src/alacorder/__main__.py` & `alacorder-80.2.2/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.1"
+version = "80.2.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -139,18 +139,20 @@
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
-    ca, ac, af = _split_cases(df, debug=cf["DEBUG"])
+    ca = _split_cases(df, debug=cf["DEBUG"])
     print("Parsing charges...", cf=cf)
+    ac = _explode_charges(df, debug=cf["DEBUG"])
     ch = _split_charges(ac, debug=cf["DEBUG"])
     print("Parsing fees...", cf=cf)
+    af = _explode_fees(df, debug=cf["DEBUG"])
     fs = _split_fees(af, debug=cf["DEBUG"])
     print("Parsing financial history...", cf=cf)
     fh = _explode_split_financial_history(df, debug=cf["DEBUG"])
     print("Parsing sentences...", cf=cf)
     sent = _explode_split_sentences(df, debug=cf["DEBUG"])
     print("Parsing settings...", cf=cf)
     settings = _explode_settings(df)
@@ -210,15 +212,15 @@
 def cases(cf):
     """
     Start cases table collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
-    ca, ac, af = _split_cases(df)
+    ca = _split_cases(df)
     if not cf["NO_WRITE"]:
         print("Writing to output path...")
         write(ca, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -1659,24 +1661,14 @@
             .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=2)
             .str.strip()
             .alias("State"),
             pl.col("AllPagesText")
-            .str.extract_all(
-                r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
-            )
-            .alias("RE_Charges"),
-            pl.col("AllPagesText")
-            .str.extract_all(
-                r"(ACTIVE [^\(\n]+\$[^\(\n]+ACTIVE[^\(\n]+[^\n]|Total:.+\$[^\n]*)"
-            )
-            .alias("RE_Fees"),
-            pl.col("AllPagesText")
             .str.extract(r"(Total:.+\$[^\n]*)")
             .str.replace_all(r"[^0-9|\.|\s|\$]", "")
             .str.extract_all(r"\s\$\d+\.\d{2}")
             .alias("TOTALS"),
             pl.col("AllPagesText")
             .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
             .str.extract_all(r"\$\d+\.\d{2}")
@@ -2089,90 +2081,14 @@
     cases = cases.with_columns(
         pl.when(pl.col("CLEAN_Phone").str.n_chars() < 7)
         .then(None)
         .otherwise(pl.col("CLEAN_Phone"))
         .alias("Phone"),
     )
 
-    # clean Charges strings
-    # explode Charges for table parsing
-    all_charges = cases.with_columns(
-        [
-            pl.concat_str(
-                [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
-                ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText")
-            .str.extract(
-                r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
-                group_index=1,
-            )
-            .str.replace_all("Case Number:", "", literal=True)
-            .str.replace(r"C$", "")
-            .str.strip()
-            .alias("Name"),
-            pl.col("AllPagesText")
-            .str.extract_all(
-                r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
-            )
-            .alias("RE_Charges"),
-            pl.col("AllPagesText")
-            .str.extract(r"(Total:.+\$[^\n]*)")
-            .str.replace_all(r"[^0-9|\.|\s|\$]", "")
-            .str.extract_all(r"\s\$\d+\.\d{2}")
-            .arr.get(2)
-            .str.replace_all(r"[^0-9\.]", "")
-            .cast(pl.Float64, strict=False)
-            .alias("RAWTotalBalance"),
-            pl.col("AllPagesText")
-            .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
-            .str.extract_all(r"\$\d+\.\d{2}")
-            .arr.get(-1)
-            .str.replace(r"[\$\s]", "")
-            .cast(pl.Float64, strict=False)
-            .alias("RAWD999"),
-        ]
-    )
-
-    all_charges = all_charges.explode("RE_Charges").select(
-        [
-            pl.col("Name"),
-            pl.col("CaseNumber"),
-            pl.col("RE_Charges")
-            .str.replace_all(r"[A-Z][a-z][A-Za-z\s\$]+.+", "")
-            .str.strip()
-            .alias("Charges"),
-            pl.when(pl.col("RAWTotalBalance").is_null())
-            .then(pl.lit(0.0))
-            .otherwise(pl.col("RAWTotalBalance"))
-            .alias("TotalBalance"),
-            pl.when(pl.col("RAWD999").is_null())
-            .then(pl.lit(0.0))
-            .otherwise(pl.col("RAWD999"))
-            .alias("TotalD999"),
-        ]
-    )
-
-    # clean Fees strings
-    # explode Fees for table parsing
-    all_fees = cases.explode("RE_Fees").select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("RE_Fees")
-            .str.replace_all(r"[^A-Z0-9|\.|\s|\$|\n]", " ")
-            .str.strip()
-            .alias("Fees"),
-        ]
-    )
-
     dlog(cases.columns, cases.shape, cf=debug)
 
     cases = cases.fill_null("")
 
     cases = cases.select(
         "Retrieved",
         "CaseNumber",
@@ -2262,15 +2178,15 @@
         "DAMailer",
         "DAMailerDate",
         "WarrantMailer",
         "WarrantMailerDate",
         "EnforcementLastUpdate",
         "EnforcementUpdatedBy",
     )
-    return cases, all_charges, all_fees
+    return cases
 
 
 def _explode_split_financial_history(df, debug=False):
     fh = df.with_columns(
         [
             pl.concat_str(
                 [
```

### Comparing `alacorder-80.2.1/src/alacorder/alac.py` & `alacorder-80.2.2/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.1"
+version = "80.2.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -139,18 +139,20 @@
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
-    ca, ac, af = _split_cases(df, debug=cf["DEBUG"])
+    ca = _split_cases(df, debug=cf["DEBUG"])
     print("Parsing charges...", cf=cf)
+    ac = _explode_charges(df, debug=cf["DEBUG"])
     ch = _split_charges(ac, debug=cf["DEBUG"])
     print("Parsing fees...", cf=cf)
+    af = _explode_fees(df, debug=cf["DEBUG"])
     fs = _split_fees(af, debug=cf["DEBUG"])
     print("Parsing financial history...", cf=cf)
     fh = _explode_split_financial_history(df, debug=cf["DEBUG"])
     print("Parsing sentences...", cf=cf)
     sent = _explode_split_sentences(df, debug=cf["DEBUG"])
     print("Parsing settings...", cf=cf)
     settings = _explode_settings(df)
@@ -210,15 +212,15 @@
 def cases(cf):
     """
     Start cases table collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
-    ca, ac, af = _split_cases(df)
+    ca = _split_cases(df)
     if not cf["NO_WRITE"]:
         print("Writing to output path...")
         write(ca, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -1659,24 +1661,14 @@
             .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=2)
             .str.strip()
             .alias("State"),
             pl.col("AllPagesText")
-            .str.extract_all(
-                r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
-            )
-            .alias("RE_Charges"),
-            pl.col("AllPagesText")
-            .str.extract_all(
-                r"(ACTIVE [^\(\n]+\$[^\(\n]+ACTIVE[^\(\n]+[^\n]|Total:.+\$[^\n]*)"
-            )
-            .alias("RE_Fees"),
-            pl.col("AllPagesText")
             .str.extract(r"(Total:.+\$[^\n]*)")
             .str.replace_all(r"[^0-9|\.|\s|\$]", "")
             .str.extract_all(r"\s\$\d+\.\d{2}")
             .alias("TOTALS"),
             pl.col("AllPagesText")
             .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
             .str.extract_all(r"\$\d+\.\d{2}")
@@ -2089,90 +2081,14 @@
     cases = cases.with_columns(
         pl.when(pl.col("CLEAN_Phone").str.n_chars() < 7)
         .then(None)
         .otherwise(pl.col("CLEAN_Phone"))
         .alias("Phone"),
     )
 
-    # clean Charges strings
-    # explode Charges for table parsing
-    all_charges = cases.with_columns(
-        [
-            pl.concat_str(
-                [
-                    pl.col("AllPagesText").str.extract(
-                        r"(County: )(\d{2})", group_index=2
-                    ),
-                    pl.lit("-"),
-                    pl.col("AllPagesText").str.extract(r"(\w{2}\-\d{4}\-\d{6}\.\d{2})"),
-                ]
-            ).alias("CaseNumber"),
-            pl.col("AllPagesText")
-            .str.extract(
-                r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
-                group_index=1,
-            )
-            .str.replace_all("Case Number:", "", literal=True)
-            .str.replace(r"C$", "")
-            .str.strip()
-            .alias("Name"),
-            pl.col("AllPagesText")
-            .str.extract_all(
-                r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{0,75})"
-            )
-            .alias("RE_Charges"),
-            pl.col("AllPagesText")
-            .str.extract(r"(Total:.+\$[^\n]*)")
-            .str.replace_all(r"[^0-9|\.|\s|\$]", "")
-            .str.extract_all(r"\s\$\d+\.\d{2}")
-            .arr.get(2)
-            .str.replace_all(r"[^0-9\.]", "")
-            .cast(pl.Float64, strict=False)
-            .alias("RAWTotalBalance"),
-            pl.col("AllPagesText")
-            .str.extract(r"(ACTIVE[^\n]+D999[^\n]+)")
-            .str.extract_all(r"\$\d+\.\d{2}")
-            .arr.get(-1)
-            .str.replace(r"[\$\s]", "")
-            .cast(pl.Float64, strict=False)
-            .alias("RAWD999"),
-        ]
-    )
-
-    all_charges = all_charges.explode("RE_Charges").select(
-        [
-            pl.col("Name"),
-            pl.col("CaseNumber"),
-            pl.col("RE_Charges")
-            .str.replace_all(r"[A-Z][a-z][A-Za-z\s\$]+.+", "")
-            .str.strip()
-            .alias("Charges"),
-            pl.when(pl.col("RAWTotalBalance").is_null())
-            .then(pl.lit(0.0))
-            .otherwise(pl.col("RAWTotalBalance"))
-            .alias("TotalBalance"),
-            pl.when(pl.col("RAWD999").is_null())
-            .then(pl.lit(0.0))
-            .otherwise(pl.col("RAWD999"))
-            .alias("TotalD999"),
-        ]
-    )
-
-    # clean Fees strings
-    # explode Fees for table parsing
-    all_fees = cases.explode("RE_Fees").select(
-        [
-            pl.col("CaseNumber"),
-            pl.col("RE_Fees")
-            .str.replace_all(r"[^A-Z0-9|\.|\s|\$|\n]", " ")
-            .str.strip()
-            .alias("Fees"),
-        ]
-    )
-
     dlog(cases.columns, cases.shape, cf=debug)
 
     cases = cases.fill_null("")
 
     cases = cases.select(
         "Retrieved",
         "CaseNumber",
@@ -2262,15 +2178,15 @@
         "DAMailer",
         "DAMailerDate",
         "WarrantMailer",
         "WarrantMailerDate",
         "EnforcementLastUpdate",
         "EnforcementUpdatedBy",
     )
-    return cases, all_charges, all_fees
+    return cases
 
 
 def _explode_split_financial_history(df, debug=False):
     fh = df.with_columns(
         [
             pl.concat_str(
                 [
```

### Comparing `alacorder-80.2.1/PKG-INFO` & `alacorder-80.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.2.1
+Version: 80.2.2
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

