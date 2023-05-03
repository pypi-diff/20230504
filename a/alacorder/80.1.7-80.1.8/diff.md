# Comparing `tmp/alacorder-80.1.7.tar.gz` & `tmp/alacorder-80.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.1.7.tar", max compression
+gzip compressed data, was "alacorder-80.1.8.tar", max compression
```

## Comparing `alacorder-80.1.7.tar` & `alacorder-80.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.7/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.7/README.md
--rw-r--r--   0        0        0      697 2023-05-03 18:10:15.008640 alacorder-80.1.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-03 14:11:51.129473 alacorder-80.1.7/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.7/src/alacorder/__init__.py
--rw-r--r--   0        0        0   214689 2023-05-03 18:09:57.733582 alacorder-80.1.7/src/alacorder/__main__.py
--rw-r--r--   0        0        0   214689 2023-05-03 18:09:49.350335 alacorder-80.1.7/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.8/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.8/README.md
+-rw-r--r--   0        0        0      697 2023-05-03 22:58:53.514157 alacorder-80.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-03 22:59:11.024671 alacorder-80.1.8/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.8/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   214510 2023-05-03 22:58:25.321932 alacorder-80.1.8/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   214510 2023-05-03 22:58:17.882270 alacorder-80.1.8/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.8/PKG-INFO
```

### Comparing `alacorder-80.1.7/LICENSE` & `alacorder-80.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.7/README.md` & `alacorder-80.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.7/pyproject.toml` & `alacorder-80.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.1.7"
+version = "80.1.8"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.1.7/src/alacorder/.DS_Store` & `alacorder-80.1.8/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.7/src/alacorder/__main__.py` & `alacorder-80.1.8/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.7"
+version = "80.1.8"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1095,15 +1095,17 @@
     """
     From path, return text of first page of PDF as string (PyMuPdf engine required!)
     """
     try:
         doc = fitz.open(path)
     except:
         return ""
-    text = doc[0].get_text(option="blocks")
+    text = " \n ".join(
+                x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
+            )
     return text
 
 def append_archive(inpath="", outpath="", cf=None):
     """
     Append the contents of one archive to another.
 
     Args:
@@ -1145,24 +1147,14 @@
 
     if window:
         window.write_event_value("COMPLETE-AA", True)
     write(out, path=outpath, overwrite=True)
     return out
 
 
-def getCaseNumber(text):
-    try:
-        return (
-            re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2]
-            + "-"
-            + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
-        )
-    except:
-        return ""
-
 
 def rename_pdfs(cf):
     if isinstance(cf, dict):
         q = cf["QUEUE"]
     elif isinstance(cf, pl.dataframe.frame.DataFrame):
         if "Path" in cf.columns:
             q = cf.select("Path").to_series().to_list()
@@ -1171,32 +1163,33 @@
         q = cf
         cf = {"LOG": False}
     if cf["LOG"]:
         for path in tqdm(q):
             text = extract_text_pg_one(path)
             try:
                 cnum = (
-                    re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[
-                        0:2
-                    ]
+                    re.search(r"County: (\d\d)", str(text)).group(1)
                     + "-"
                     + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
                 )
             except:
                 cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
     else:
         for path in q:
             text = extract_text_pg_one(path)
-            cnum = (
-                re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2]
-                + "-"
-                + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
-            )
+            try:
+                cnum = (
+                    re.search(r"County: (\d\d)", str(text)).group(1)
+                    + "-"
+                    + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+                )
+            except:
+                cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
 
 
 def make_pairs_template(df, debug=False):
     if isinstance(df, str):
         df = read(df)
```

### Comparing `alacorder-80.1.7/src/alacorder/alac.py` & `alacorder-80.1.8/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.7"
+version = "80.1.8"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1095,15 +1095,17 @@
     """
     From path, return text of first page of PDF as string (PyMuPdf engine required!)
     """
     try:
         doc = fitz.open(path)
     except:
         return ""
-    text = doc[0].get_text(option="blocks")
+    text = " \n ".join(
+                x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
+            )
     return text
 
 def append_archive(inpath="", outpath="", cf=None):
     """
     Append the contents of one archive to another.
 
     Args:
@@ -1145,24 +1147,14 @@
 
     if window:
         window.write_event_value("COMPLETE-AA", True)
     write(out, path=outpath, overwrite=True)
     return out
 
 
-def getCaseNumber(text):
-    try:
-        return (
-            re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2]
-            + "-"
-            + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
-        )
-    except:
-        return ""
-
 
 def rename_pdfs(cf):
     if isinstance(cf, dict):
         q = cf["QUEUE"]
     elif isinstance(cf, pl.dataframe.frame.DataFrame):
         if "Path" in cf.columns:
             q = cf.select("Path").to_series().to_list()
@@ -1171,32 +1163,33 @@
         q = cf
         cf = {"LOG": False}
     if cf["LOG"]:
         for path in tqdm(q):
             text = extract_text_pg_one(path)
             try:
                 cnum = (
-                    re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[
-                        0:2
-                    ]
+                    re.search(r"County: (\d\d)", str(text)).group(1)
                     + "-"
                     + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
                 )
             except:
                 cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
     else:
         for path in q:
             text = extract_text_pg_one(path)
-            cnum = (
-                re.search(r"Case Number: (\d\d-\w+) County:", str(text)).group(1)[0:2]
-                + "-"
-                + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
-            )
+            try:
+                cnum = (
+                    re.search(r"County: (\d\d)", str(text)).group(1)
+                    + "-"
+                    + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+                )
+            except:
+                cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
 
 
 def make_pairs_template(df, debug=False):
     if isinstance(df, str):
         df = read(df)
```

### Comparing `alacorder-80.1.7/PKG-INFO` & `alacorder-80.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.1.7
+Version: 80.1.8
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

