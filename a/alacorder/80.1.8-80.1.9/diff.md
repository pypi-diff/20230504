# Comparing `tmp/alacorder-80.1.8.tar.gz` & `tmp/alacorder-80.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.1.8.tar", max compression
+gzip compressed data, was "alacorder-80.1.9.tar", max compression
```

## Comparing `alacorder-80.1.8.tar` & `alacorder-80.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.8/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.8/README.md
--rw-r--r--   0        0        0      697 2023-05-03 22:58:53.514157 alacorder-80.1.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-03 22:59:11.024671 alacorder-80.1.8/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.8/src/alacorder/__init__.py
--rw-r--r--   0        0        0   214510 2023-05-03 22:58:25.321932 alacorder-80.1.8/src/alacorder/__main__.py
--rw-r--r--   0        0        0   214510 2023-05-03 22:58:17.882270 alacorder-80.1.8/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.9/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.9/README.md
+-rw-r--r--   0        0        0      697 2023-05-04 02:05:41.091872 alacorder-80.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-03 22:59:11.024671 alacorder-80.1.9/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.1.9/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   215515 2023-05-04 02:05:20.083537 alacorder-80.1.9/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   215515 2023-05-04 02:04:41.811135 alacorder-80.1.9/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.9/PKG-INFO
```

### Comparing `alacorder-80.1.8/LICENSE` & `alacorder-80.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.8/README.md` & `alacorder-80.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.8/pyproject.toml` & `alacorder-80.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.1.8"
+version = "80.1.9"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.1.8/src/alacorder/.DS_Store` & `alacorder-80.1.9/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.8/src/alacorder/__main__.py` & `alacorder-80.1.9/src/alacorder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.8"
+version = "80.1.9"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
-import os, sys, time, glob, re
+import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
@@ -126,14 +126,15 @@
 #   #   #   #            TABLE PARSERS           #   #   #   #
 
 
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
+    start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
     ca, ac, af = split_cases(df, debug=cf["DEBUG"])
     print("Parsing charges...", cf=cf)
     ch = split_charges(ac, debug=cf["DEBUG"])
     print("Parsing fees...", cf=cf)
     fs = split_fees(af, debug=cf["DEBUG"])
@@ -187,253 +188,277 @@
         "sentences": sent,
         "settings": settings,
         "case-action-summary": cas,
         "witnesses": wit,
         "attorneys": att,
         "images": img,
     }
-    print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     return out
 
 
 def cases(cf):
     """
     Start cases table collection using configuration object `cf`.
     """
+    start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
     ca, ac, af = split_cases(df)
     if not cf["NO_WRITE"]:
         print("Writing to output path...")
         write(ca, cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ca
 
 
 def charges(cf):
     """
     Start charges table collection using configuration object `cf`.
     """
+    start = time.time()
     df = read(cf)
     print("Parsing charges...", cf=cf)
     ac = explode_charges(df)
     ch = split_charges(ac)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(ch, cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ch
 
 
 def fees(cf):
     """
     Start fee sheet collection using configuration object `cf`.
     """
+    start = time.time()
     df = read(cf)
     print("Parsing fee sheets...", cf=cf)
     af = explode_fees(df)
     fs = split_fees(af)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(fs, cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return fs
 
 
 def witnesses(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing witnesses...", cf=cf)
     out = explode_witnesses(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["witnesses"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def financial_history(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing financial history...", cf=cf)
     out = explode_split_financial_history(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["financial-history"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def sentences(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing sentences...", cf=cf)
     out = explode_split_sentences(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["sentences"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def cas(cf):
     """
     Collect case action summaries using configuration object `cf`.
     """
+    start = time.time()
     print("Parsing case action summaries...", cf=cf)
     q = read(cf["QUEUE"])
     out = explode_case_action_summary(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["case-action-summary"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def attorneys(cf):
     """
     Collect attorneys tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing attorneys...", cf=cf)
     out = explode_attorneys(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["attorneys"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def settings(cf):
     """
     Collect settings tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     out = explode_settings(q)
     print("Parsing settings...", cf=cf)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["settings"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def images(cf):
     """
     Collect images tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing images...", cf=cf)
     out = explode_images(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["images"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def vrr_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    start = time.time()
     print(
         "Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf
     )
     vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
-        print("Completed table export.", cf=cf)
-    if cf["LOG"]:
-        print("Created table successfully.")
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
     return vr
 
 
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    start = time.time()
     print("Combining cases by AIS / Unique ID to create charges summary...", cf=cf)
     ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             ch,
             sheet_names=["ChargesSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
         )
         print("Completed table export.", cf=cf)
-    if cf["LOG"]:
-        print("Created table successfully.")
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CHSUM-COMPLETE", True)
     return ch
 
 
 def convictions_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    start = time.time()
     print("Combining cases by AIS / Unique ID to create convictions summary...", cf=cf)
     conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             conv,
             sheet_names=["ConvictionsSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
         )
         print("Completed table export.", cf=cf)
-    if cf["LOG"]:
-        print("Created table successfully.")
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
 
 def archive(cf):
     """
     Write a full text archive from inputs using configuration `cf`.
     """
-    print("Extracting text...", cf=cf)
+    start = time.time()
     a = read(cf)
     write(a, cf=cf)
-    print("Completed archive export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-MA", True)
     return a
 
 
 #   #   #   #         CONFIGURATION & I/O        #   #   #   #
```

### Comparing `alacorder-80.1.8/src/alacorder/alac.py` & `alacorder-80.1.9/src/alacorder/alac.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.8"
+version = "80.1.9"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
-import os, sys, time, glob, re
+import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
@@ -126,14 +126,15 @@
 #   #   #   #            TABLE PARSERS           #   #   #   #
 
 
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
+    start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
     ca, ac, af = split_cases(df, debug=cf["DEBUG"])
     print("Parsing charges...", cf=cf)
     ch = split_charges(ac, debug=cf["DEBUG"])
     print("Parsing fees...", cf=cf)
     fs = split_fees(af, debug=cf["DEBUG"])
@@ -187,253 +188,277 @@
         "sentences": sent,
         "settings": settings,
         "case-action-summary": cas,
         "witnesses": wit,
         "attorneys": att,
         "images": img,
     }
-    print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     return out
 
 
 def cases(cf):
     """
     Start cases table collection using configuration object `cf`.
     """
+    start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
     ca, ac, af = split_cases(df)
     if not cf["NO_WRITE"]:
         print("Writing to output path...")
         write(ca, cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ca
 
 
 def charges(cf):
     """
     Start charges table collection using configuration object `cf`.
     """
+    start = time.time()
     df = read(cf)
     print("Parsing charges...", cf=cf)
     ac = explode_charges(df)
     ch = split_charges(ac)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(ch, cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return ch
 
 
 def fees(cf):
     """
     Start fee sheet collection using configuration object `cf`.
     """
+    start = time.time()
     df = read(cf)
     print("Parsing fee sheets...", cf=cf)
     af = explode_fees(df)
     fs = split_fees(af)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(fs, cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return fs
 
 
 def witnesses(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing witnesses...", cf=cf)
     out = explode_witnesses(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["witnesses"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def financial_history(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing financial history...", cf=cf)
     out = explode_split_financial_history(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["financial-history"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def sentences(cf):
     """
     Collect witnesses tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing sentences...", cf=cf)
     out = explode_split_sentences(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["sentences"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def cas(cf):
     """
     Collect case action summaries using configuration object `cf`.
     """
+    start = time.time()
     print("Parsing case action summaries...", cf=cf)
     q = read(cf["QUEUE"])
     out = explode_case_action_summary(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["case-action-summary"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def attorneys(cf):
     """
     Collect attorneys tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing attorneys...", cf=cf)
     out = explode_attorneys(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["attorneys"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def settings(cf):
     """
     Collect settings tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     out = explode_settings(q)
     print("Parsing settings...", cf=cf)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["settings"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def images(cf):
     """
     Collect images tables using configuration object `cf`.
     """
+    start = time.time()
     q = read(cf)
     print("Parsing images...", cf=cf)
     out = explode_images(q)
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(out, sheet_names=["images"], cf=cf)
-        print("Completed table export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-TB", True)
     return out
 
 
 def vrr_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    start = time.time()
     print(
         "Combining cases by AIS / Unique ID to create voting rights summary...", cf=cf
     )
     vr = vrr_summary_from_pairs(cf["INPUTS"], cf["PAIRS"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             vr, sheet_names=["VRR"], path=cf["OUTPUT_PATH"], overwrite=cf["OVERWRITE"]
         )
-        print("Completed table export.", cf=cf)
-    if cf["LOG"]:
-        print("Created table successfully.")
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("VRR-COMPLETE", True)
     return vr
 
 
 def charges_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    start = time.time()
     print("Combining cases by AIS / Unique ID to create charges summary...", cf=cf)
     ch = charges_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             ch,
             sheet_names=["ChargesSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
         )
         print("Completed table export.", cf=cf)
-    if cf["LOG"]:
-        print("Created table successfully.")
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CHSUM-COMPLETE", True)
     return ch
 
 
 def convictions_summary(cf):
     """
     Summarize voting rights status from pairs using configuration object `cf`.
     """
+    start = time.time()
     print("Combining cases by AIS / Unique ID to create convictions summary...", cf=cf)
     conv = convictions_summary_from_pairs(cf["INPUTS"], cf["PAIRS"], debug=cf["DEBUG"])
     if not cf["NO_WRITE"]:
         print("Writing to output path...", cf=cf)
         write(
             conv,
             sheet_names=["ConvictionsSummary"],
             path=cf["OUTPUT_PATH"],
             overwrite=cf["OVERWRITE"],
         )
         print("Completed table export.", cf=cf)
-    if cf["LOG"]:
-        print("Created table successfully.")
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
 
 def archive(cf):
     """
     Write a full text archive from inputs using configuration `cf`.
     """
-    print("Extracting text...", cf=cf)
+    start = time.time()
     a = read(cf)
     write(a, cf=cf)
-    print("Completed archive export.", cf=cf)
+    elapsed = math.floor(time.time() - start)
+    print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-MA", True)
     return a
 
 
 #   #   #   #         CONFIGURATION & I/O        #   #   #   #
```

### Comparing `alacorder-80.1.8/PKG-INFO` & `alacorder-80.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.1.8
+Version: 80.1.9
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

