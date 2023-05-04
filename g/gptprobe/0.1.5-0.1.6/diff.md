# Comparing `tmp/gptprobe-0.1.5.tar.gz` & `tmp/gptprobe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptprobe-0.1.5.tar", last modified: Thu May  4 21:43:00 2023, max compression
+gzip compressed data, was "gptprobe-0.1.6.tar", last modified: Thu May  4 21:47:43 2023, max compression
```

## Comparing `gptprobe-0.1.5.tar` & `gptprobe-0.1.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:00.121756 gptprobe-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 21:42:29.000000 gptprobe-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-04 21:43:00.121756 gptprobe-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-04 21:42:29.000000 gptprobe-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:00.117756 gptprobe-0.1.5/gptprobe/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:00.121756 gptprobe-0.1.5/gptprobe/askfor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/clarification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/clarificationfromquestionandanswer.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/dictfrompoorlyformattedtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/dictfromquestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/dictfromquestionanswerandclarification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/dictfromquestionwithratification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/dictfromquestionwithretries.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/dictfromtext.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/dicttext.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/flaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/flawfromquestionandanswer.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/ratification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/ratificationfromquestionandanswer.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/rephrasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/rephrasingfromquestionandanswer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/rephrasingfromquestionanswerandflaw.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/textfrompoorlyformatteddicttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/askfor/textfromquestion.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/keysinenviron.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/public_setenv.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/public_setenv_triple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:00.121756 gptprobe-0.1.5/gptprobe/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/utils/customtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/utils/enginedefaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/utils/equivalence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-04 21:42:29.000000 gptprobe-0.1.5/gptprobe/utils/parsedictrobustly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:43:00.117756 gptprobe-0.1.5/gptprobe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-04 21:43:00.000000 gptprobe-0.1.5/gptprobe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-04 21:43:00.000000 gptprobe-0.1.5/gptprobe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:43:00.000000 gptprobe-0.1.5/gptprobe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 21:43:00.000000 gptprobe-0.1.5/gptprobe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 21:43:00.000000 gptprobe-0.1.5/gptprobe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 21:43:00.000000 gptprobe-0.1.5/gptprobe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:43:00.121756 gptprobe-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 21:42:29.000000 gptprobe-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:47:43.339726 gptprobe-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 21:47:12.000000 gptprobe-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-04 21:47:43.339726 gptprobe-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-04 21:47:12.000000 gptprobe-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:47:43.335726 gptprobe-0.1.6/gptprobe/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:47:43.339726 gptprobe-0.1.6/gptprobe/askfor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/clarification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/clarificationfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/dictfrompoorlyformattedtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/dictfromquestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/dictfromquestionanswerandclarification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/dictfromquestionwithratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/dictfromquestionwithretries.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/dictfromtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/dicttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/flaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/flawfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/ratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/ratificationfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/rephrasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/rephrasingfromquestionandanswer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/rephrasingfromquestionanswerandflaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/textfrompoorlyformatteddicttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/askfor/textfromquestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/keysinenviron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/public_setenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/public_setenv_triple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:47:43.339726 gptprobe-0.1.6/gptprobe/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/utils/customtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/utils/enginedefaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/utils/equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-04 21:47:12.000000 gptprobe-0.1.6/gptprobe/utils/parsedictrobustly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:47:43.335726 gptprobe-0.1.6/gptprobe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-04 21:47:43.000000 gptprobe-0.1.6/gptprobe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-04 21:47:43.000000 gptprobe-0.1.6/gptprobe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:47:43.000000 gptprobe-0.1.6/gptprobe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 21:47:43.000000 gptprobe-0.1.6/gptprobe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 21:47:43.000000 gptprobe-0.1.6/gptprobe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 21:47:43.000000 gptprobe-0.1.6/gptprobe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:47:43.339726 gptprobe-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-04 21:47:12.000000 gptprobe-0.1.6/setup.py
```

### Comparing `gptprobe-0.1.5/LICENSE` & `gptprobe-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/PKG-INFO` & `gptprobe-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptprobe
-Version: 0.1.5
+Version: 0.1.6
 Summary: Probing chatgpt
 Home-page: https://github.com/gptprobe/gptprobe
 Author: gptprobe
 Author-email: pcotton@intechinvestments.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gptprobe-0.1.5/README.md` & `gptprobe-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/clarificationfromquestionandanswer.py` & `gptprobe-0.1.6/gptprobe/askfor/clarificationfromquestionandanswer.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/dictfrompoorlyformattedtext.py` & `gptprobe-0.1.6/gptprobe/askfor/dictfrompoorlyformattedtext.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/dictfromquestion.py` & `gptprobe-0.1.6/gptprobe/askfor/dictfromquestion.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/dictfromquestionanswerandclarification.py` & `gptprobe-0.1.6/gptprobe/askfor/dictfromquestionanswerandclarification.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/dictfromquestionwithratification.py` & `gptprobe-0.1.6/gptprobe/askfor/dictfromquestionwithratification.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/dictfromquestionwithretries.py` & `gptprobe-0.1.6/gptprobe/askfor/dictfromquestionwithretries.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,9 +47,9 @@
 if __name__=='__main__':
     from gptprobe.private_setenv import NOTHING
     question = """Return a dictionary with double-quoted keys given by trees and numeric values
                   indicating the month of the year when they are most likely to bloom.
                """
     import os
     os.environ['GPTPROBE_VERBOSITY']="1"
-    d = ask_for_dict_from_question_with_ratification(question=question)
+    d = ask_for_dict_from_question_with_retries(question=question)
     print(d)
```

### Comparing `gptprobe-0.1.5/gptprobe/askfor/flawfromquestionandanswer.py` & `gptprobe-0.1.6/gptprobe/askfor/flawfromquestionandanswer.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/ratificationfromquestionandanswer.py` & `gptprobe-0.1.6/gptprobe/askfor/ratificationfromquestionandanswer.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/rephrasingfromquestionandanswer.py` & `gptprobe-0.1.6/gptprobe/askfor/rephrasingfromquestionandanswer.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/rephrasingfromquestionanswerandflaw.py` & `gptprobe-0.1.6/gptprobe/askfor/rephrasingfromquestionanswerandflaw.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/textfrompoorlyformatteddicttext.py` & `gptprobe-0.1.6/gptprobe/askfor/textfrompoorlyformatteddicttext.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/askfor/textfromquestion.py` & `gptprobe-0.1.6/gptprobe/askfor/textfromquestion.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/keysinenviron.py` & `gptprobe-0.1.6/gptprobe/keysinenviron.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/utils/equivalence.py` & `gptprobe-0.1.6/gptprobe/utils/equivalence.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe/utils/parsedictrobustly.py` & `gptprobe-0.1.6/gptprobe/utils/parsedictrobustly.py`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/gptprobe.egg-info/PKG-INFO` & `gptprobe-0.1.6/gptprobe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptprobe
-Version: 0.1.5
+Version: 0.1.6
 Summary: Probing chatgpt
 Home-page: https://github.com/gptprobe/gptprobe
 Author: gptprobe
 Author-email: pcotton@intechinvestments.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gptprobe-0.1.5/gptprobe.egg-info/SOURCES.txt` & `gptprobe-0.1.6/gptprobe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gptprobe-0.1.5/setup.py` & `gptprobe-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="gptprobe",
-    version="0.1.5",
+    version="0.1.6",
     description="Probing chatgpt",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/gptprobe/gptprobe",
     author="gptprobe",
     author_email="pcotton@intechinvestments.com",
     license="MIT",
```

