# Comparing `tmp/alacorder-80.1.9.tar.gz` & `tmp/alacorder-80.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.1.9.tar", max compression
+gzip compressed data, was "alacorder-80.2.0.tar", max compression
```

## Comparing `alacorder-80.1.9.tar` & `alacorder-80.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.9/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.9/README.md
--rw-r--r--   0        0        0      697 2023-05-04 02:05:41.091872 alacorder-80.1.9/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-03 22:59:11.024671 alacorder-80.1.9/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   215515 2023-05-04 02:05:20.083537 alacorder-80.1.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   215515 2023-05-04 02:04:41.811135 alacorder-80.1.9/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.0/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.0/README.md
+-rw-r--r--   0        0        0      697 2023-05-04 16:42:21.565233 alacorder-80.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-04 16:42:22.855831 alacorder-80.2.0/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   215964 2023-05-04 16:41:49.636066 alacorder-80.2.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   215964 2023-05-04 16:41:45.053162 alacorder-80.2.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.0/PKG-INFO
```

### Comparing `alacorder-80.1.9/LICENSE` & `alacorder-80.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.9/README.md` & `alacorder-80.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.9/pyproject.toml` & `alacorder-80.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.1.9"
+version = "80.2.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.1.9/src/alacorder/.DS_Store` & `alacorder-80.2.0/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.9/src/alacorder/__main__.py` & `alacorder-80.2.0/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.9"
+version = "80.2.0"
 
-autoload_graphical_user_interface = False
+_autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from selenium import webdriver
 from selenium.webdriver.common.by import By
@@ -31,21 +31,19 @@
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
 pl.Config.set_tbl_width_chars(90)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_dataframe_shape_below(True)
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
-
-fname = f"{name} {version}"
-fshort_name = f"{name} {'.'.join(version.split('.')[0:-1])}"
+FNAME = f"{name} {version}"
+FSHORT_NAME = f"{name} {'.'.join(version.split('.')[0:-1])}"
 
 prt = print
 
-
 def plog(*msg, cf=None):
     global prt
     if len(msg) == 1:
         msg = msg[0]
         if isinstance(cf, dict):
             try:
                 if cf["LOG"] == True:
@@ -65,15 +63,14 @@
                 except:
                     prt(m)
             elif cf == None:
                 prt(m)
             elif type(cf) == bool and cf:
                 prt(m)
 
-
 print = plog
 
 
 def dlog(*msg, cf=None):
     if type(cf) == bool:
         if cf:
             for m in msg:
@@ -122,40 +119,53 @@
     else:
         print(message)
 
 
 #   #   #   #            TABLE PARSERS           #   #   #   #
 
 
+def archive(cf):
+    """
+    Write a full text archive from inputs using configuration `cf`.
+    """
+    start = time.time()
+    a = read(cf)
+    write(a, cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
+    if cf["WINDOW"]:
+        cf["WINDOW"].write_event_value("COMPLETE-MA", True)
+    return a
+
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
-    ca, ac, af = split_cases(df, debug=cf["DEBUG"])
+    ca, ac, af = _split_cases(df, debug=cf["DEBUG"])
     print("Parsing charges...", cf=cf)
-    ch = split_charges(ac, debug=cf["DEBUG"])
+    ch = _split_charges(ac, debug=cf["DEBUG"])
     print("Parsing fees...", cf=cf)
-    fs = split_fees(af, debug=cf["DEBUG"])
+    fs = _split_fees(af, debug=cf["DEBUG"])
     print("Parsing financial history...", cf=cf)
-    fh = explode_split_financial_history(df, debug=cf["DEBUG"])
+    fh = _explode_split_financial_history(df, debug=cf["DEBUG"])
     print("Parsing sentences...", cf=cf)
-    sent = explode_split_sentences(df, debug=cf["DEBUG"])
+    sent = _explode_split_sentences(df, debug=cf["DEBUG"])
     print("Parsing settings...", cf=cf)
-    settings = explode_settings(df)
+    settings = _explode_settings(df)
     print("Parsing case action summaries...", cf=cf)
-    cas = explode_case_action_summary(df)
+    cas = _explode_case_action_summary(df)
     print("Parsing witnesses...", cf=cf)
-    wit = explode_witnesses(df)
+    wit = _explode_witnesses(df)
     print("Parsing attorneys...", cf=cf)
-    att = explode_attorneys(df)
+    att = _explode_attorneys(df)
     print("Parsing images...", cf=cf)
-    img = explode_images(df)
+    img = _explode_images(df)
     dlog(ca, ch, fs, settings, cas, wit, att, img, cf=cf)
     ch_filing = ch.filter(pl.col("Filing") == True).select(
         pl.exclude("CourtAction", "CourtActionDate")
     )
     ch_disposition = ch.filter(pl.col("Filing") == False)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
@@ -200,15 +210,15 @@
 def cases(cf):
     """
     Start cases table collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
-    ca, ac, af = split_cases(df)
+    ca, ac, af = _split_cases(df)
     if not cf["NO_WRITE"]:
         print("Writing to output path...")
         write(ca, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -218,16 +228,16 @@
 def charges(cf):
     """
     Start charges table collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing charges...", cf=cf)
-    ac = explode_charges(df)
-    ch = split_charges(ac)
+    ac = _explode_charges(df)
+    ch = _split_charges(ac)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(ch, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -237,16 +247,16 @@
 def fees(cf):
     """
     Start fee sheet collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing fee sheets...", cf=cf)
-    af = explode_fees(df)
-    fs = split_fees(af)
+    af = _explode_fees(df)
+    fs = _split_fees(af)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(fs, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -256,15 +266,15 @@
 def witnesses(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing witnesses...", cf=cf)
-    out = explode_witnesses(q)
+    out = _explode_witnesses(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["witnesses"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -274,15 +284,15 @@
 def financial_history(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing financial history...", cf=cf)
-    out = explode_split_financial_history(q)
+    out = _explode_split_financial_history(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["financial-history"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -292,15 +302,15 @@
 def sentences(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing sentences...", cf=cf)
-    out = explode_split_sentences(q)
+    out = _explode_split_sentences(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["sentences"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -310,15 +320,15 @@
 def cas(cf):
     """
     Collect case action summaries using configuration object `cf`.
     """
     start = time.time()
     print("Parsing case action summaries...", cf=cf)
     q = read(cf["QUEUE"])
-    out = explode_case_action_summary(q)
+    out = _explode_case_action_summary(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["case-action-summary"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -328,15 +338,15 @@
 def attorneys(cf):
     """
     Collect attorneys tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing attorneys...", cf=cf)
-    out = explode_attorneys(q)
+    out = _explode_attorneys(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["attorneys"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -345,15 +355,15 @@
 
 def settings(cf):
     """
     Collect settings tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
-    out = explode_settings(q)
+    out = _explode_settings(q)
     print("Parsing settings...", cf=cf)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["settings"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
@@ -364,15 +374,15 @@
 def images(cf):
     """
     Collect images tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing images...", cf=cf)
-    out = explode_images(q)
+    out = _explode_images(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["images"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -442,27 +452,14 @@
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
 
-def archive(cf):
-    """
-    Write a full text archive from inputs using configuration `cf`.
-    """
-    start = time.time()
-    a = read(cf)
-    write(a, cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-MA", True)
-    return a
-
 
 #   #   #   #         CONFIGURATION & I/O        #   #   #   #
 
 
 def set(
     inputs,
     outputs=None,
@@ -1499,15 +1496,15 @@
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
 
-def explode_charges(df, debug=False):
+def _explode_charges(df, debug=False):
     all_charges = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -1566,15 +1563,15 @@
         ]
     )
 
     dlog(all_charges, all_charges.columns, cf=debug)
     return all_charges
 
 
-def explode_fees(df, debug=False):
+def _explode_fees(df, debug=False):
     cases = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -1598,15 +1595,15 @@
             .alias("Fees"),
         ]
     )
     dlog(all_fees.columns, cf=debug)
     return all_fees
 
 
-def split_cases(df, debug=False):
+def _split_cases(df, debug=False):
     cases = df.with_columns(
         [
             pl.col("AllPagesText")
             .str.extract(
                 r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
                 group_index=1,
             )
@@ -1993,21 +1990,14 @@
             .str.strip()
             .alias("Frequency"),
             pl.col("AllPagesText")
             .str.extract(r"Placement Status\: (.+)")
             .str.strip()
             .alias("PlacementStatus"),
             pl.col("AllPagesText")
-            .str.extract(r"Comments\: (.+)")
-            .str.strip()
-            .alias("Comments"),
-            pl.col("AllPagesText")
-            .str.extract(r"Over/Under Paid\: \$(\d+\.\d\d)")
-            .alias("OverUnderPaid"),
-            pl.col("AllPagesText")
             .str.extract(r"PreTrial\: (YES|NO)")
             .alias("PreTrial"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrail Date\: (.+)PreTrial")
             .str.strip()
             .alias("PreTrialDate"),
             pl.col("AllPagesText")
@@ -2277,15 +2267,15 @@
         "WarrantMailerDate",
         "EnforcementLastUpdate",
         "EnforcementUpdatedBy",
     )
     return cases, all_charges, all_fees
 
 
-def explode_split_financial_history(df, debug=False):
+def _explode_split_financial_history(df, debug=False):
     fh = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2346,15 +2336,15 @@
         "Operator",
     )
     fh = fh.drop_nulls()
     fh = fh.fill_null("")
     return fh
 
 
-def split_charges(df, debug=False):
+def _split_charges(df, debug=False):
     dlog(df.columns, df.shape, "^ split_charges input param", cf=debug)
     charges = df.with_columns(
         [
             pl.col("Name"),
             pl.col("CaseNumber"),
             pl.col("Charges").str.slice(0, 3).alias("Num"),
             pl.col("Charges").str.slice(4, 4).alias("Code"),
@@ -2583,15 +2573,15 @@
         "PaymentToRestore",
         "ChargesSummary",
     )
     dlog(charges.columns, charges.shape, cf=debug)
     return charges
 
 
-def split_fees(df, debug=False):
+def _split_fees(df, debug=False):
     df = df.with_columns(
         [
             pl.col("CaseNumber"),
             pl.col("Fees")
             .str.replace(r"(?:\$\d{1,2})( )", "\2")
             .str.split(" ")
             .alias("SPACE_SEP"),
@@ -2678,15 +2668,15 @@
     )
     dlog(out.columns, out.shape, cf=debug)
     out = out.fill_null("")
     out = out.drop_nulls("AmtDue")
     return out
 
 
-def explode_images(df, debug=False):
+def _explode_images(df, debug=False):
     images = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2721,15 +2711,15 @@
             .str.replace_all(r"[\s\:]+", " ")
             .str.strip(),
         ]
     )
     return images
 
 
-def explode_case_action_summary(df, debug=False):
+def _explode_case_action_summary(df, debug=False):
     cas = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2758,15 +2748,15 @@
         ]
     )
     cas = cas.explode("CaseActionSummary")
     cas = cas.filter(pl.col("CaseActionSummary").str.contains(r"[A-Za-z0-9]"))
     return cas
 
 
-def explode_attorneys(df, debug=False):
+def _explode_attorneys(df, debug=False):
     att = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2785,15 +2775,15 @@
             .str.strip()
             .alias("Attorneys"),
         ]
     )
     return att.drop_nulls()
 
 
-def explode_witnesses(df, debug=False):
+def _explode_witnesses(df, debug=False):
     wit = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2820,15 +2810,15 @@
             .str.strip()
             .alias("Witnesses"),
         ]
     )
     return wit.drop_nulls()
 
 
-def explode_settings(df, debug=False):
+def _explode_settings(df, debug=False):
     settings = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2862,15 +2852,15 @@
             .str.strip()
             .alias("Settings"),
         ]
     )
     return settings.drop_nulls()
 
 
-def explode_split_sentences(df, debug=False):
+def _explode_split_sentences(df, debug=False):
     sent = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2895,22 +2885,24 @@
             .str.extract(r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
             .alias("LastUpdate"),
             pl.col("Sentence")
             .str.extract(r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
             .alias("UpdatedBy"),
             pl.col("Sentence")
             .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
+            .str.replace(r'Sentence.*','')
+            .str.replace(r'License.+','')
             .str.strip()
             .alias("ProbationRevoke"),
             pl.col("Sentence")
             .str.extract(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("LicenseSuspPeriod"),
             pl.col("Sentence")
-            .str.extract(r"Days\.\s+(\d+ Years, \d+ Months, \d+ Days\.)\s+")
-            .alias("JailCreditPeriod"),  ## CHECK !!
+            .str.extract(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+")
+            .alias("JailCreditPeriod"), 
             pl.col("Sentence")
             .str.extract(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("ProbationPeriod"),
             pl.col("Sentence")
             .str.extract(r"Sentence Provisions\: ([YN])")
             .alias("Provisions"),
             pl.col("Sentence")
@@ -2922,110 +2914,115 @@
             pl.col("Sentence")
             .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
             .alias("StartDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
             .alias("EndDate"),
             pl.col("Sentence")
-            .str.extract(r"Jail Fee\: (.+?) Costs")
+            .str.extract(r"Jail Fee\:(.+?)Costs")
             .str.replace(r"[A-Z]-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("JailFee"),
             pl.col("Sentence")
-            .str.extract(r"Costs\: (.+?)Fine\: .+? Crime Victims")
+            .str.extract(r"Costs\: (.+?)Fine\:")
+            .str.replace(r'Fine.+','')
             .str.strip()
             .alias("Costs"),
             pl.col("Sentence")
-            .str.extract(r"Costs\: .+?Fine\: (.+?) Crime Victims")
+            .str.extract(r"Fine\:(.+?)Crime Victims") 
             .str.strip()
             .alias("Fine"),
             pl.col("Sentence")
-            .str.extract(r"Crime Victims Fee\: (.+?) Monetary")
+            .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
             .str.strip()
             .alias("CrimeVictimsFee"),
             pl.col("Sentence")
-            .str.extract(r"Municipal Court\: (.+?) Fine Suspended")
+            .str.extract(r"Municipal Court\:(.+?)Fine Suspended") ## NONE
             .str.replace(r"X-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("MunicipalCourt"),
             pl.col("Sentence")
-            .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
+            .str.extract(r"Fine Suspended\: (.+?)Immigration Fine") 
             .str.strip()
-            .alias("FineSuspended"),  ## NONE !!
+            .alias("FineSuspended"), 
             pl.col("Sentence")
             .str.extract(r"Immigration Fine\: (.+?)Fine")
             .str.strip()
-            .alias("ImmigrationFine"),  ## NONE !!
+            .alias("ImmigrationFine"),
             pl.col("Sentence")
             .str.extract(r"Fine Imposed\: (.+?) Alias Warrant")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("FineImposed"),
             pl.col("Sentence")
-            .str.extract(r"Drug Docket Fees\: (.+?) Prelim Hearing")
+            .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing") 
+            .str.replace(r'Prelim Hearing.+','')
             .str.strip()
             .alias("DrugDocketFees"),
             pl.col("Sentence")
-            .str.extract(r"Prelim Hearing\: (.+?) Amt Over Minimum CVF")
+            .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
+            .str.replace(r'Amt.+','') 
             .str.strip()
             .alias("PrelimHearing"),
             pl.col("Sentence")
             .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
             .str.replace_all(r"[A-Z\s]|\-|\$", "")
             .cast(pl.Float64, strict=False)
             .alias("AmtOverMinimumCVF"),
             pl.col("Sentence")
-            .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
+            .str.extract(r"WC Fee DA\: (.+?)Removal Bill") 
             .str.strip()
             .alias("WCFeeDA"),  ## NONE !!
             pl.col("Sentence")
-            .str.extract(r"Removal Bill\: (.+?) Crime History Fee")
+            .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
             .str.strip()
             .alias("RemovalBill"),
             pl.col("Sentence")
-            .str.extract(r"Crime History Fee\: (.+?) SX10")
+            .str.extract(r"Crime History Fee\: (.+?) SX10") 
             .str.strip()
             .alias("CrimeHistoryFee"),
             pl.col("Sentence")
-            .str.extract(r"SX10\: (.+?) License Suspension Fee")
+            .str.extract(r"SX10\: (.+?)License Suspension Fee")
             .str.strip()
             .alias("SX10"),
             pl.col("Sentence")
             .str.extract(r"License Suspension Fee\: (.+?) WC Fee 85%")
             .str.replace_all(r"[A-Z\s]+", "")
             .cast(pl.Float64, strict=False)
             .alias("LicenseSuspensionFee"),
             pl.col("Sentence")
-            .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing")
+            .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:") 
+            .str.replace(r'Demand Reduction Hearing.+','')
             .str.strip()
             .alias("WCFee85"),
             pl.col("Sentence")
-            .str.extract(r"Demand Reduction Hearing\: (.+?) Drug User Fee")
+            .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee") 
             .str.replace_all(r"[A-Z]\-|\s|\$", "")
             .str.strip()
-            .cast(pl.Float64, strict=False)
+             .cast(pl.Float64, strict=False)
             .alias("DemandReductionHearing"),
             pl.col("Sentence")
             .str.extract(r"Drug User Fee\: (.+?) Subpoena")
             .str.strip()
             .alias("DrugUserFee"),
             pl.col("Sentence")
             .str.extract(r"Subpoena\: (.+?) Attorney Fees")
             .str.replace_all(r"[X\-\s\$]", "")
             .cast(pl.Float64, strict=False)
             .alias("Subpoena"),
             pl.col("Sentence")
             .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
             .str.replace("© Alacourt.com", "", literal=True)
+            .str.replace(r'Split.+','')
+            .str.replace(r'Confinement.+','')
             .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
             .str.replace(r"\$|Recipient", "")
             .str.replace_all(r"\s+", "")
-            .cast(pl.Float64, strict=False)
             .alias("AttorneyFees"),
             pl.col("Sentence")
             .str.extract(
                 r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("ImposedConfinementPeriod"),
             pl.col("Sentence")
@@ -3033,122 +3030,130 @@
                 r"Total Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("TotalConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(
                 r"Suspended Confinement Period (\d+ Years, \d+ Months, \d+ Days\.)"
             )
-            .alias("SuspendedConfinementPeriod"),  ## CHECK
+            .alias("SuspendedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(r"Boot Camp\: (.+?) (Penitentiary|Life Without Parole)")
+            .str.replace(r'Penitentiary.+','')
             .str.strip()
             .alias("BootCamp"),
             pl.col("Sentence")
-            .str.extract(r"Life Without Parole\: (.+?) (Restitution|Death)")
+            .str.extract(r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1) 
+            .str.replace(r'Death.+','')
+            .str.replace(r'Restitution.+','')
             .str.strip()
             .alias("LifeWithoutParole"),
             pl.col("Sentence")
-            .str.extract(r"Attorney Fees\: .+? Split\: (.+?) (Concurrent|Confinement)")
+            .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1) 
             .str.strip()
             .alias("Split"),
             pl.col("Sentence")
             .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
             .str.strip()
             .alias("ConcurrentSentence"),
             pl.col("Sentence")
-            .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
+            .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s") 
             .str.strip()
             .alias("ConsecutiveSentence"),
             pl.col("Sentence")
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
-            .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
+            .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)") 
             .str.replace_all(r"Death\: Life\:", "")
             .str.strip()
             .alias("ReverseSplit"),
             pl.col("Sentence")
             .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
             .alias("CoterminousSentence"),
             pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
             pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
             pl.col("Sentence")
             .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
             .alias("ChainGang"),
             pl.col("Sentence").str.extract(r"Jail\:\s+([0-9]|X?)").alias("Jail"),
             pl.col("Sentence")
-            .str.extract(r"Community Service Hrs\:\s+(0|X?)")
+            .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)") 
             .alias("CommunityServiceHrs"),
             pl.col("Sentence")
             .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
             .alias("JailDiversion"),
             pl.col("Sentence")
-            .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
+            .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s") 
             .alias("Alcoholics Anonymous"),
             pl.col("Sentence")
-            .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
+            .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s") 
             .alias("BadCheckSchool"),
             pl.col("Sentence")
             .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
             .alias("InformalProbation"),
             pl.col("Sentence")
-            .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s")
+            .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s") 
             .alias("CourtReferralProgram"),
             pl.col("Sentence")
-            .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
+            .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s") 
             .alias("CommunityService"),
             pl.col("Sentence")
-            .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
+            .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s") 
             .alias("AlternativeSentencing"),
             pl.col("Sentence")
-            .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
+            .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s") 
             .alias("PreTrialDiversion"),
             pl.col("Sentence")
             .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
             .alias("DUISchool"),
             pl.col("Sentence")
-            .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
+            .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s") 
             .alias("DefensiveDrivingSchool"),
             pl.col("Sentence")
-            .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
+            .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)") 
             .alias("DocCommunityCorrections"),
             pl.col("Sentence")
             .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
             .alias("JailCommunityCorrections"),
             pl.col("Sentence")
             .str.extract(r"Mental Health\:\s+([0-9]|X?)")
             .alias("MentalHealth"),
             pl.col("Sentence")
-            .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
+            .str.extract(r"Anger Management Program\:\s+([0-9]|X?)") 
             .alias("AngerManagementProgram"),
             pl.col("Sentence")
             .str.extract(r"Drug Court\:\s+([0-9]|X?)")
             .alias("DrugCourt"),
             pl.col("Sentence")
             .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
             .alias("DocDrugProgram"),
             pl.col("Sentence")
-            .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
+            .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project") 
             .str.strip()
             .alias("DrugMeasureUnit"),
             pl.col("Sentence")
             .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
             .str.strip()
             .alias("DrugNearProject"),
             pl.col("Sentence")
-            .str.extract(r"Drugs Near School\: (.+?)Habitual Offender")
+            .str.extract(r"Drugs Near School\: (.+?)Habitual Offender") 
+            .str.replace(r'Habitual Offender\:','')
+            .str.replace(r'Sex Offender Community Notification\:','')
+            .str.replace(r'Drug Volume\:','')
+            .str.replace(r'Drug\:','')
+            .str.replace(r'Drug Code\:\s?\d*','')
             .str.strip()
             .alias("DrugsNearSchool"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
             .alias("HabitualOffender"),
             pl.col("Sentence")
-            .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
+            .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume") 
             .str.replace_all(r"[X\s0-9]", "")
             .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
             .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
             .cast(pl.Float64, strict=False)
             .alias("DrugVolume"),
             pl.col("Sentence")
@@ -4127,15 +4132,15 @@
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
             [sg.Tab("append", layout=append_layout, pad=(2, 2))],
             [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
-        [sg.Text(fshort_name, font=LOGO_FONT, pad=(5, 5))],
+        [sg.Text(FSHORT_NAME, font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
             sg.ProgressBar(
                 100,
                 size=[5, 10],
                 expand_y=False,
                 orientation="h",
@@ -4375,29 +4380,29 @@
             pass
 
 
 #   #   #   #       COMMAND LINE INTERFACE     #   #   #   #
 
 
 @click.group(
-    invoke_without_command=autoload_graphical_user_interface,
+    invoke_without_command=_autoload_graphical_user_interface,
     context_settings=CONTEXT_SETTINGS,
 )
 @click.version_option(f"{version}", package_name=f"{name} {long_version}")
 @click.pass_context
 def main(ctx):
     """
     ALACORDER collects and processes case detail PDFs into data tables suitable for research purposes.
     """
-    if autoload_graphical_user_interface and ctx.invoked_subcommand == None:
+    if _autoload_graphical_user_interface and ctx.invoked_subcommand == None:
         loadgui()
 
 
 @main.command(name="start", help="Launch graphical user interface")
-def cli_start():
+def _cli_start():
     loadgui()
 
 
 @main.command(name="append", help="Append one case text archive to another")
 @click.option(
     "--input-path",
     "-in",
@@ -4420,15 +4425,15 @@
     "--no-write",
     "-n",
     default=False,
     is_flag=True,
     help="Do not export to output path",
     hidden=True,
 )
-def cli_append(in_path, out_path, no_write=False):
+def _cli_append(in_path, out_path, no_write=False):
     """Append one case text archive to another
 
     Args:
         in_path (Path|DataFrame): Path to input archive / PDF directory
         out_path (Path): Path to output archive
         no_write (bool, optional): Do not export to output path
 
@@ -4514,15 +4519,15 @@
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def cli_fetch(querypath, path, criminal, cID, uID, pwd, qmax, qskip, no_update, debug):
+def _cli_fetch(querypath, path, criminal, cID, uID, pwd, qmax, qskip, no_update, debug):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
         criminal (bool, optional): only search criminal cases
         cID (str): Customer ID on Alacourt.com
@@ -4592,15 +4597,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_multi(
+def _cli_multi(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write data tables to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -4677,15 +4682,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_cases(
+def _cli_cases(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -4776,15 +4781,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_charges(
+def _cli_charges(
     input_path,
     output_path,
     filing,
     disposition,
     count,
     overwrite,
     no_write,
@@ -4883,15 +4888,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_fees(
+def _cli_fees(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -4976,15 +4981,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_settings(
+def _cli_settings(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5071,15 +5076,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_finhist(
+def _cli_finhist(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5164,15 +5169,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_sentences(
+def _cli_sentences(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5257,15 +5262,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_witnesses(
+def _cli_witnesses(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5352,15 +5357,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_case_action_summary(
+def _cli_case_action_summary(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5445,15 +5450,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_images(
+def _cli_images(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5538,15 +5543,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_attorneys(
+def _cli_attorneys(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5637,15 +5642,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
-def cli_archive(
+def _cli_archive(
     input_path, output_path, count, overwrite, append, no_log, no_prompt, debug
 ):
     """
     Write a full text archive from a directory of case detail PDFs.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5716,15 +5721,15 @@
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
-def cli_pair(input_path, output_path, overwrite, debug):
+def _cli_pair(input_path, output_path, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
@@ -5766,15 +5771,15 @@
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
-def cli_vrr(input_path, output_path, pairs, overwrite, debug):
+def _cli_vrr(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         vrr_summary=True,
         debug=debug,
         overwrite=overwrite,
@@ -5816,15 +5821,15 @@
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
-def cli_charge_pairs(input_path, output_path, pairs, overwrite, debug):
+def _cli_charge_pairs(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         charges_summary=True,
         debug=debug,
         overwrite=overwrite,
@@ -5866,15 +5871,15 @@
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
-def cli_conv_pairs(input_path, output_path, pairs, overwrite, debug):
+def _cli_conv_pairs(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         convictions_summary=True,
         debug=debug,
         overwrite=overwrite,
```

### Comparing `alacorder-80.1.9/src/alacorder/alac.py` & `alacorder-80.2.0/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.9"
+version = "80.2.0"
 
-autoload_graphical_user_interface = False
+_autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from selenium import webdriver
 from selenium.webdriver.common.by import By
@@ -31,21 +31,19 @@
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
 pl.Config.set_tbl_width_chars(90)
 pl.Config.set_tbl_formatting("NOTHING")
 pl.Config.set_tbl_dataframe_shape_below(True)
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
-
-fname = f"{name} {version}"
-fshort_name = f"{name} {'.'.join(version.split('.')[0:-1])}"
+FNAME = f"{name} {version}"
+FSHORT_NAME = f"{name} {'.'.join(version.split('.')[0:-1])}"
 
 prt = print
 
-
 def plog(*msg, cf=None):
     global prt
     if len(msg) == 1:
         msg = msg[0]
         if isinstance(cf, dict):
             try:
                 if cf["LOG"] == True:
@@ -65,15 +63,14 @@
                 except:
                     prt(m)
             elif cf == None:
                 prt(m)
             elif type(cf) == bool and cf:
                 prt(m)
 
-
 print = plog
 
 
 def dlog(*msg, cf=None):
     if type(cf) == bool:
         if cf:
             for m in msg:
@@ -122,40 +119,53 @@
     else:
         print(message)
 
 
 #   #   #   #            TABLE PARSERS           #   #   #   #
 
 
+def archive(cf):
+    """
+    Write a full text archive from inputs using configuration `cf`.
+    """
+    start = time.time()
+    a = read(cf)
+    write(a, cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
+    if cf["WINDOW"]:
+        cf["WINDOW"].write_event_value("COMPLETE-MA", True)
+    return a
+
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
-    ca, ac, af = split_cases(df, debug=cf["DEBUG"])
+    ca, ac, af = _split_cases(df, debug=cf["DEBUG"])
     print("Parsing charges...", cf=cf)
-    ch = split_charges(ac, debug=cf["DEBUG"])
+    ch = _split_charges(ac, debug=cf["DEBUG"])
     print("Parsing fees...", cf=cf)
-    fs = split_fees(af, debug=cf["DEBUG"])
+    fs = _split_fees(af, debug=cf["DEBUG"])
     print("Parsing financial history...", cf=cf)
-    fh = explode_split_financial_history(df, debug=cf["DEBUG"])
+    fh = _explode_split_financial_history(df, debug=cf["DEBUG"])
     print("Parsing sentences...", cf=cf)
-    sent = explode_split_sentences(df, debug=cf["DEBUG"])
+    sent = _explode_split_sentences(df, debug=cf["DEBUG"])
     print("Parsing settings...", cf=cf)
-    settings = explode_settings(df)
+    settings = _explode_settings(df)
     print("Parsing case action summaries...", cf=cf)
-    cas = explode_case_action_summary(df)
+    cas = _explode_case_action_summary(df)
     print("Parsing witnesses...", cf=cf)
-    wit = explode_witnesses(df)
+    wit = _explode_witnesses(df)
     print("Parsing attorneys...", cf=cf)
-    att = explode_attorneys(df)
+    att = _explode_attorneys(df)
     print("Parsing images...", cf=cf)
-    img = explode_images(df)
+    img = _explode_images(df)
     dlog(ca, ch, fs, settings, cas, wit, att, img, cf=cf)
     ch_filing = ch.filter(pl.col("Filing") == True).select(
         pl.exclude("CourtAction", "CourtActionDate")
     )
     ch_disposition = ch.filter(pl.col("Filing") == False)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
@@ -200,15 +210,15 @@
 def cases(cf):
     """
     Start cases table collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
-    ca, ac, af = split_cases(df)
+    ca, ac, af = _split_cases(df)
     if not cf["NO_WRITE"]:
         print("Writing to output path...")
         write(ca, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -218,16 +228,16 @@
 def charges(cf):
     """
     Start charges table collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing charges...", cf=cf)
-    ac = explode_charges(df)
-    ch = split_charges(ac)
+    ac = _explode_charges(df)
+    ch = _split_charges(ac)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(ch, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -237,16 +247,16 @@
 def fees(cf):
     """
     Start fee sheet collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing fee sheets...", cf=cf)
-    af = explode_fees(df)
-    fs = split_fees(af)
+    af = _explode_fees(df)
+    fs = _split_fees(af)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(fs, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -256,15 +266,15 @@
 def witnesses(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing witnesses...", cf=cf)
-    out = explode_witnesses(q)
+    out = _explode_witnesses(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["witnesses"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -274,15 +284,15 @@
 def financial_history(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing financial history...", cf=cf)
-    out = explode_split_financial_history(q)
+    out = _explode_split_financial_history(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["financial-history"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -292,15 +302,15 @@
 def sentences(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing sentences...", cf=cf)
-    out = explode_split_sentences(q)
+    out = _explode_split_sentences(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["sentences"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -310,15 +320,15 @@
 def cas(cf):
     """
     Collect case action summaries using configuration object `cf`.
     """
     start = time.time()
     print("Parsing case action summaries...", cf=cf)
     q = read(cf["QUEUE"])
-    out = explode_case_action_summary(q)
+    out = _explode_case_action_summary(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["case-action-summary"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -328,15 +338,15 @@
 def attorneys(cf):
     """
     Collect attorneys tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing attorneys...", cf=cf)
-    out = explode_attorneys(q)
+    out = _explode_attorneys(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["attorneys"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -345,15 +355,15 @@
 
 def settings(cf):
     """
     Collect settings tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
-    out = explode_settings(q)
+    out = _explode_settings(q)
     print("Parsing settings...", cf=cf)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["settings"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
@@ -364,15 +374,15 @@
 def images(cf):
     """
     Collect images tables using configuration object `cf`.
     """
     start = time.time()
     q = read(cf)
     print("Parsing images...", cf=cf)
-    out = explode_images(q)
+    out = _explode_images(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["images"], cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
@@ -442,27 +452,14 @@
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
 
-def archive(cf):
-    """
-    Write a full text archive from inputs using configuration `cf`.
-    """
-    start = time.time()
-    a = read(cf)
-    write(a, cf=cf)
-    elapsed = math.floor(time.time() - start)
-    print(f"Completed in {elapsed} seconds.", cf=cf)
-    if cf["WINDOW"]:
-        cf["WINDOW"].write_event_value("COMPLETE-MA", True)
-    return a
-
 
 #   #   #   #         CONFIGURATION & I/O        #   #   #   #
 
 
 def set(
     inputs,
     outputs=None,
@@ -1499,15 +1496,15 @@
         ]
     )
     summary = summary.filter(pl.col("Name") != "")
     summary = summary.fill_null("")
     return summary
 
 
-def explode_charges(df, debug=False):
+def _explode_charges(df, debug=False):
     all_charges = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -1566,15 +1563,15 @@
         ]
     )
 
     dlog(all_charges, all_charges.columns, cf=debug)
     return all_charges
 
 
-def explode_fees(df, debug=False):
+def _explode_fees(df, debug=False):
     cases = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -1598,15 +1595,15 @@
             .alias("Fees"),
         ]
     )
     dlog(all_fees.columns, cf=debug)
     return all_fees
 
 
-def split_cases(df, debug=False):
+def _split_cases(df, debug=False):
     cases = df.with_columns(
         [
             pl.col("AllPagesText")
             .str.extract(
                 r"(?:VS\.|V\.| VS | V | VS: |-VS-{1})([A-Z\s]{10,100})(Case Number)*",
                 group_index=1,
             )
@@ -1993,21 +1990,14 @@
             .str.strip()
             .alias("Frequency"),
             pl.col("AllPagesText")
             .str.extract(r"Placement Status\: (.+)")
             .str.strip()
             .alias("PlacementStatus"),
             pl.col("AllPagesText")
-            .str.extract(r"Comments\: (.+)")
-            .str.strip()
-            .alias("Comments"),
-            pl.col("AllPagesText")
-            .str.extract(r"Over/Under Paid\: \$(\d+\.\d\d)")
-            .alias("OverUnderPaid"),
-            pl.col("AllPagesText")
             .str.extract(r"PreTrial\: (YES|NO)")
             .alias("PreTrial"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrail Date\: (.+)PreTrial")
             .str.strip()
             .alias("PreTrialDate"),
             pl.col("AllPagesText")
@@ -2277,15 +2267,15 @@
         "WarrantMailerDate",
         "EnforcementLastUpdate",
         "EnforcementUpdatedBy",
     )
     return cases, all_charges, all_fees
 
 
-def explode_split_financial_history(df, debug=False):
+def _explode_split_financial_history(df, debug=False):
     fh = df.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2346,15 +2336,15 @@
         "Operator",
     )
     fh = fh.drop_nulls()
     fh = fh.fill_null("")
     return fh
 
 
-def split_charges(df, debug=False):
+def _split_charges(df, debug=False):
     dlog(df.columns, df.shape, "^ split_charges input param", cf=debug)
     charges = df.with_columns(
         [
             pl.col("Name"),
             pl.col("CaseNumber"),
             pl.col("Charges").str.slice(0, 3).alias("Num"),
             pl.col("Charges").str.slice(4, 4).alias("Code"),
@@ -2583,15 +2573,15 @@
         "PaymentToRestore",
         "ChargesSummary",
     )
     dlog(charges.columns, charges.shape, cf=debug)
     return charges
 
 
-def split_fees(df, debug=False):
+def _split_fees(df, debug=False):
     df = df.with_columns(
         [
             pl.col("CaseNumber"),
             pl.col("Fees")
             .str.replace(r"(?:\$\d{1,2})( )", "\2")
             .str.split(" ")
             .alias("SPACE_SEP"),
@@ -2678,15 +2668,15 @@
     )
     dlog(out.columns, out.shape, cf=debug)
     out = out.fill_null("")
     out = out.drop_nulls("AmtDue")
     return out
 
 
-def explode_images(df, debug=False):
+def _explode_images(df, debug=False):
     images = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2721,15 +2711,15 @@
             .str.replace_all(r"[\s\:]+", " ")
             .str.strip(),
         ]
     )
     return images
 
 
-def explode_case_action_summary(df, debug=False):
+def _explode_case_action_summary(df, debug=False):
     cas = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2758,15 +2748,15 @@
         ]
     )
     cas = cas.explode("CaseActionSummary")
     cas = cas.filter(pl.col("CaseActionSummary").str.contains(r"[A-Za-z0-9]"))
     return cas
 
 
-def explode_attorneys(df, debug=False):
+def _explode_attorneys(df, debug=False):
     att = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2785,15 +2775,15 @@
             .str.strip()
             .alias("Attorneys"),
         ]
     )
     return att.drop_nulls()
 
 
-def explode_witnesses(df, debug=False):
+def _explode_witnesses(df, debug=False):
     wit = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2820,15 +2810,15 @@
             .str.strip()
             .alias("Witnesses"),
         ]
     )
     return wit.drop_nulls()
 
 
-def explode_settings(df, debug=False):
+def _explode_settings(df, debug=False):
     settings = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2862,15 +2852,15 @@
             .str.strip()
             .alias("Settings"),
         ]
     )
     return settings.drop_nulls()
 
 
-def explode_split_sentences(df, debug=False):
+def _explode_split_sentences(df, debug=False):
     sent = df.select(
         [
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
@@ -2895,22 +2885,24 @@
             .str.extract(r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
             .alias("LastUpdate"),
             pl.col("Sentence")
             .str.extract(r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
             .alias("UpdatedBy"),
             pl.col("Sentence")
             .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
+            .str.replace(r'Sentence.*','')
+            .str.replace(r'License.+','')
             .str.strip()
             .alias("ProbationRevoke"),
             pl.col("Sentence")
             .str.extract(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("LicenseSuspPeriod"),
             pl.col("Sentence")
-            .str.extract(r"Days\.\s+(\d+ Years, \d+ Months, \d+ Days\.)\s+")
-            .alias("JailCreditPeriod"),  ## CHECK !!
+            .str.extract(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+")
+            .alias("JailCreditPeriod"), 
             pl.col("Sentence")
             .str.extract(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("ProbationPeriod"),
             pl.col("Sentence")
             .str.extract(r"Sentence Provisions\: ([YN])")
             .alias("Provisions"),
             pl.col("Sentence")
@@ -2922,110 +2914,115 @@
             pl.col("Sentence")
             .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
             .alias("StartDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
             .alias("EndDate"),
             pl.col("Sentence")
-            .str.extract(r"Jail Fee\: (.+?) Costs")
+            .str.extract(r"Jail Fee\:(.+?)Costs")
             .str.replace(r"[A-Z]-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("JailFee"),
             pl.col("Sentence")
-            .str.extract(r"Costs\: (.+?)Fine\: .+? Crime Victims")
+            .str.extract(r"Costs\: (.+?)Fine\:")
+            .str.replace(r'Fine.+','')
             .str.strip()
             .alias("Costs"),
             pl.col("Sentence")
-            .str.extract(r"Costs\: .+?Fine\: (.+?) Crime Victims")
+            .str.extract(r"Fine\:(.+?)Crime Victims") 
             .str.strip()
             .alias("Fine"),
             pl.col("Sentence")
-            .str.extract(r"Crime Victims Fee\: (.+?) Monetary")
+            .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
             .str.strip()
             .alias("CrimeVictimsFee"),
             pl.col("Sentence")
-            .str.extract(r"Municipal Court\: (.+?) Fine Suspended")
+            .str.extract(r"Municipal Court\:(.+?)Fine Suspended") ## NONE
             .str.replace(r"X-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("MunicipalCourt"),
             pl.col("Sentence")
-            .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
+            .str.extract(r"Fine Suspended\: (.+?)Immigration Fine") 
             .str.strip()
-            .alias("FineSuspended"),  ## NONE !!
+            .alias("FineSuspended"), 
             pl.col("Sentence")
             .str.extract(r"Immigration Fine\: (.+?)Fine")
             .str.strip()
-            .alias("ImmigrationFine"),  ## NONE !!
+            .alias("ImmigrationFine"),
             pl.col("Sentence")
             .str.extract(r"Fine Imposed\: (.+?) Alias Warrant")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("FineImposed"),
             pl.col("Sentence")
-            .str.extract(r"Drug Docket Fees\: (.+?) Prelim Hearing")
+            .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing") 
+            .str.replace(r'Prelim Hearing.+','')
             .str.strip()
             .alias("DrugDocketFees"),
             pl.col("Sentence")
-            .str.extract(r"Prelim Hearing\: (.+?) Amt Over Minimum CVF")
+            .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
+            .str.replace(r'Amt.+','') 
             .str.strip()
             .alias("PrelimHearing"),
             pl.col("Sentence")
             .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
             .str.replace_all(r"[A-Z\s]|\-|\$", "")
             .cast(pl.Float64, strict=False)
             .alias("AmtOverMinimumCVF"),
             pl.col("Sentence")
-            .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
+            .str.extract(r"WC Fee DA\: (.+?)Removal Bill") 
             .str.strip()
             .alias("WCFeeDA"),  ## NONE !!
             pl.col("Sentence")
-            .str.extract(r"Removal Bill\: (.+?) Crime History Fee")
+            .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
             .str.strip()
             .alias("RemovalBill"),
             pl.col("Sentence")
-            .str.extract(r"Crime History Fee\: (.+?) SX10")
+            .str.extract(r"Crime History Fee\: (.+?) SX10") 
             .str.strip()
             .alias("CrimeHistoryFee"),
             pl.col("Sentence")
-            .str.extract(r"SX10\: (.+?) License Suspension Fee")
+            .str.extract(r"SX10\: (.+?)License Suspension Fee")
             .str.strip()
             .alias("SX10"),
             pl.col("Sentence")
             .str.extract(r"License Suspension Fee\: (.+?) WC Fee 85%")
             .str.replace_all(r"[A-Z\s]+", "")
             .cast(pl.Float64, strict=False)
             .alias("LicenseSuspensionFee"),
             pl.col("Sentence")
-            .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing")
+            .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:") 
+            .str.replace(r'Demand Reduction Hearing.+','')
             .str.strip()
             .alias("WCFee85"),
             pl.col("Sentence")
-            .str.extract(r"Demand Reduction Hearing\: (.+?) Drug User Fee")
+            .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee") 
             .str.replace_all(r"[A-Z]\-|\s|\$", "")
             .str.strip()
-            .cast(pl.Float64, strict=False)
+             .cast(pl.Float64, strict=False)
             .alias("DemandReductionHearing"),
             pl.col("Sentence")
             .str.extract(r"Drug User Fee\: (.+?) Subpoena")
             .str.strip()
             .alias("DrugUserFee"),
             pl.col("Sentence")
             .str.extract(r"Subpoena\: (.+?) Attorney Fees")
             .str.replace_all(r"[X\-\s\$]", "")
             .cast(pl.Float64, strict=False)
             .alias("Subpoena"),
             pl.col("Sentence")
             .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
             .str.replace("© Alacourt.com", "", literal=True)
+            .str.replace(r'Split.+','')
+            .str.replace(r'Confinement.+','')
             .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
             .str.replace(r"\$|Recipient", "")
             .str.replace_all(r"\s+", "")
-            .cast(pl.Float64, strict=False)
             .alias("AttorneyFees"),
             pl.col("Sentence")
             .str.extract(
                 r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("ImposedConfinementPeriod"),
             pl.col("Sentence")
@@ -3033,122 +3030,130 @@
                 r"Total Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("TotalConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(
                 r"Suspended Confinement Period (\d+ Years, \d+ Months, \d+ Days\.)"
             )
-            .alias("SuspendedConfinementPeriod"),  ## CHECK
+            .alias("SuspendedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(r"Boot Camp\: (.+?) (Penitentiary|Life Without Parole)")
+            .str.replace(r'Penitentiary.+','')
             .str.strip()
             .alias("BootCamp"),
             pl.col("Sentence")
-            .str.extract(r"Life Without Parole\: (.+?) (Restitution|Death)")
+            .str.extract(r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1) 
+            .str.replace(r'Death.+','')
+            .str.replace(r'Restitution.+','')
             .str.strip()
             .alias("LifeWithoutParole"),
             pl.col("Sentence")
-            .str.extract(r"Attorney Fees\: .+? Split\: (.+?) (Concurrent|Confinement)")
+            .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1) 
             .str.strip()
             .alias("Split"),
             pl.col("Sentence")
             .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
             .str.strip()
             .alias("ConcurrentSentence"),
             pl.col("Sentence")
-            .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
+            .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s") 
             .str.strip()
             .alias("ConsecutiveSentence"),
             pl.col("Sentence")
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
-            .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
+            .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)") 
             .str.replace_all(r"Death\: Life\:", "")
             .str.strip()
             .alias("ReverseSplit"),
             pl.col("Sentence")
             .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
             .alias("CoterminousSentence"),
             pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
             pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
             pl.col("Sentence")
             .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
             .alias("ChainGang"),
             pl.col("Sentence").str.extract(r"Jail\:\s+([0-9]|X?)").alias("Jail"),
             pl.col("Sentence")
-            .str.extract(r"Community Service Hrs\:\s+(0|X?)")
+            .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)") 
             .alias("CommunityServiceHrs"),
             pl.col("Sentence")
             .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
             .alias("JailDiversion"),
             pl.col("Sentence")
-            .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
+            .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s") 
             .alias("Alcoholics Anonymous"),
             pl.col("Sentence")
-            .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
+            .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s") 
             .alias("BadCheckSchool"),
             pl.col("Sentence")
             .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
             .alias("InformalProbation"),
             pl.col("Sentence")
-            .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s")
+            .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s") 
             .alias("CourtReferralProgram"),
             pl.col("Sentence")
-            .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
+            .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s") 
             .alias("CommunityService"),
             pl.col("Sentence")
-            .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
+            .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s") 
             .alias("AlternativeSentencing"),
             pl.col("Sentence")
-            .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
+            .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s") 
             .alias("PreTrialDiversion"),
             pl.col("Sentence")
             .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
             .alias("DUISchool"),
             pl.col("Sentence")
-            .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
+            .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s") 
             .alias("DefensiveDrivingSchool"),
             pl.col("Sentence")
-            .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
+            .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)") 
             .alias("DocCommunityCorrections"),
             pl.col("Sentence")
             .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
             .alias("JailCommunityCorrections"),
             pl.col("Sentence")
             .str.extract(r"Mental Health\:\s+([0-9]|X?)")
             .alias("MentalHealth"),
             pl.col("Sentence")
-            .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
+            .str.extract(r"Anger Management Program\:\s+([0-9]|X?)") 
             .alias("AngerManagementProgram"),
             pl.col("Sentence")
             .str.extract(r"Drug Court\:\s+([0-9]|X?)")
             .alias("DrugCourt"),
             pl.col("Sentence")
             .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
             .alias("DocDrugProgram"),
             pl.col("Sentence")
-            .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
+            .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project") 
             .str.strip()
             .alias("DrugMeasureUnit"),
             pl.col("Sentence")
             .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
             .str.strip()
             .alias("DrugNearProject"),
             pl.col("Sentence")
-            .str.extract(r"Drugs Near School\: (.+?)Habitual Offender")
+            .str.extract(r"Drugs Near School\: (.+?)Habitual Offender") 
+            .str.replace(r'Habitual Offender\:','')
+            .str.replace(r'Sex Offender Community Notification\:','')
+            .str.replace(r'Drug Volume\:','')
+            .str.replace(r'Drug\:','')
+            .str.replace(r'Drug Code\:\s?\d*','')
             .str.strip()
             .alias("DrugsNearSchool"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
             .alias("HabitualOffender"),
             pl.col("Sentence")
-            .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
+            .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume") 
             .str.replace_all(r"[X\s0-9]", "")
             .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
             .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
             .cast(pl.Float64, strict=False)
             .alias("DrugVolume"),
             pl.col("Sentence")
@@ -4127,15 +4132,15 @@
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
             [sg.Tab("append", layout=append_layout, pad=(2, 2))],
             [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
-        [sg.Text(fshort_name, font=LOGO_FONT, pad=(5, 5))],
+        [sg.Text(FSHORT_NAME, font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
             sg.ProgressBar(
                 100,
                 size=[5, 10],
                 expand_y=False,
                 orientation="h",
@@ -4375,29 +4380,29 @@
             pass
 
 
 #   #   #   #       COMMAND LINE INTERFACE     #   #   #   #
 
 
 @click.group(
-    invoke_without_command=autoload_graphical_user_interface,
+    invoke_without_command=_autoload_graphical_user_interface,
     context_settings=CONTEXT_SETTINGS,
 )
 @click.version_option(f"{version}", package_name=f"{name} {long_version}")
 @click.pass_context
 def main(ctx):
     """
     ALACORDER collects and processes case detail PDFs into data tables suitable for research purposes.
     """
-    if autoload_graphical_user_interface and ctx.invoked_subcommand == None:
+    if _autoload_graphical_user_interface and ctx.invoked_subcommand == None:
         loadgui()
 
 
 @main.command(name="start", help="Launch graphical user interface")
-def cli_start():
+def _cli_start():
     loadgui()
 
 
 @main.command(name="append", help="Append one case text archive to another")
 @click.option(
     "--input-path",
     "-in",
@@ -4420,15 +4425,15 @@
     "--no-write",
     "-n",
     default=False,
     is_flag=True,
     help="Do not export to output path",
     hidden=True,
 )
-def cli_append(in_path, out_path, no_write=False):
+def _cli_append(in_path, out_path, no_write=False):
     """Append one case text archive to another
 
     Args:
         in_path (Path|DataFrame): Path to input archive / PDF directory
         out_path (Path): Path to output archive
         no_write (bool, optional): Do not export to output path
 
@@ -4514,15 +4519,15 @@
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def cli_fetch(querypath, path, criminal, cID, uID, pwd, qmax, qskip, no_update, debug):
+def _cli_fetch(querypath, path, criminal, cID, uID, pwd, qmax, qskip, no_update, debug):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
         criminal (bool, optional): only search criminal cases
         cID (str): Customer ID on Alacourt.com
@@ -4592,15 +4597,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_multi(
+def _cli_multi(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write data tables to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -4677,15 +4682,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_cases(
+def _cli_cases(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -4776,15 +4781,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_charges(
+def _cli_charges(
     input_path,
     output_path,
     filing,
     disposition,
     count,
     overwrite,
     no_write,
@@ -4883,15 +4888,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_fees(
+def _cli_fees(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -4976,15 +4981,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_settings(
+def _cli_settings(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5071,15 +5076,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_finhist(
+def _cli_finhist(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5164,15 +5169,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_sentences(
+def _cli_sentences(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5257,15 +5262,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_witnesses(
+def _cli_witnesses(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5352,15 +5357,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_case_action_summary(
+def _cli_case_action_summary(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5445,15 +5450,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_images(
+def _cli_images(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5538,15 +5543,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print debug logs to console"
 )
 @click.version_option(
     package_name="alacorder", prog_name=name, message="%(prog)s beta %(version)s"
 )
-def cli_attorneys(
+def _cli_attorneys(
     input_path, output_path, count, overwrite, no_write, no_log, no_prompt, debug
 ):
     """
     Write `cases` table to output path from archive or directory input.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5637,15 +5642,15 @@
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
-def cli_archive(
+def _cli_archive(
     input_path, output_path, count, overwrite, append, no_log, no_prompt, debug
 ):
     """
     Write a full text archive from a directory of case detail PDFs.
 
     Args:
         input_path (str): PDF directory or archive input
@@ -5716,15 +5721,15 @@
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
-def cli_pair(input_path, output_path, overwrite, debug):
+def _cli_pair(input_path, output_path, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         debug=debug,
         overwrite=overwrite,
         log=True,
     )
@@ -5766,15 +5771,15 @@
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
-def cli_vrr(input_path, output_path, pairs, overwrite, debug):
+def _cli_vrr(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         vrr_summary=True,
         debug=debug,
         overwrite=overwrite,
@@ -5816,15 +5821,15 @@
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
-def cli_charge_pairs(input_path, output_path, pairs, overwrite, debug):
+def _cli_charge_pairs(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         charges_summary=True,
         debug=debug,
         overwrite=overwrite,
@@ -5866,15 +5871,15 @@
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
-def cli_conv_pairs(input_path, output_path, pairs, overwrite, debug):
+def _cli_conv_pairs(input_path, output_path, pairs, overwrite, debug):
     conf = cf(
         inputs=input_path,
         outputs=output_path,
         pairs=pairs,
         convictions_summary=True,
         debug=debug,
         overwrite=overwrite,
```

### Comparing `alacorder-80.1.9/PKG-INFO` & `alacorder-80.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.1.9
+Version: 80.2.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

