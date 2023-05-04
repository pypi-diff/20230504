# Comparing `tmp/textfiles-0.0.4.tar.gz` & `tmp/textfiles-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textfiles-0.0.4.tar", last modified: Thu May  4 15:18:54 2023, max compression
+gzip compressed data, was "textfiles-0.0.5.tar", last modified: Thu May  4 15:29:38 2023, max compression
```

## Comparing `textfiles-0.0.4.tar` & `textfiles-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:18:54.563207 textfiles-0.0.4/
--rwxrwxrwx   0 hemed     (1000) hemed     (1000)     1087 2023-01-12 08:44:14.000000 textfiles-0.0.4/LICENSE
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 15:18:54.563207 textfiles-0.0.4/PKG-INFO
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2272 2023-05-04 15:17:13.000000 textfiles-0.0.4/README.md
--rw-rw-r--   0 hemed     (1000) hemed     (1000)       38 2023-05-04 15:18:54.563207 textfiles-0.0.4/setup.cfg
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     1044 2023-05-04 15:17:13.000000 textfiles-0.0.4/setup.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:18:54.559208 textfiles-0.0.4/tests/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      832 2023-03-09 05:46:03.000000 textfiles-0.0.4/tests/test_for_csv.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      823 2023-04-02 11:21:54.000000 textfiles-0.0.4/tests/tests_for_txt.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:18:54.559208 textfiles-0.0.4/textfiles/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:17:13.000000 textfiles-0.0.4/textfiles/__init__.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     9422 2023-05-04 15:18:38.000000 textfiles-0.0.4/textfiles/csv_file.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     1387 2023-04-19 18:50:04.000000 textfiles-0.0.4/textfiles/exceptions.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2580 2023-05-04 15:18:39.000000 textfiles-0.0.4/textfiles/file_factory.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     8496 2023-05-04 15:18:39.000000 textfiles-0.0.4/textfiles/json_file.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2427 2023-05-04 15:18:39.000000 textfiles-0.0.4/textfiles/text_file_parent.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     3735 2023-05-04 15:18:39.000000 textfiles-0.0.4/textfiles/txt_file.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:18:54.559208 textfiles-0.0.4/textfiles.egg-info/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 15:18:54.000000 textfiles-0.0.4/textfiles.egg-info/PKG-INFO
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      372 2023-05-04 15:18:54.000000 textfiles-0.0.4/textfiles.egg-info/SOURCES.txt
--rw-rw-r--   0 hemed     (1000) hemed     (1000)        1 2023-05-04 15:18:54.000000 textfiles-0.0.4/textfiles.egg-info/dependency_links.txt
--rw-rw-r--   0 hemed     (1000) hemed     (1000)       10 2023-05-04 15:18:54.000000 textfiles-0.0.4/textfiles.egg-info/top_level.txt
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:29:38.737907 textfiles-0.0.5/
+-rwxrwxrwx   0 hemed     (1000) hemed     (1000)     1087 2023-01-12 08:44:14.000000 textfiles-0.0.5/LICENSE
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 15:29:38.737907 textfiles-0.0.5/PKG-INFO
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2272 2023-05-04 15:29:30.000000 textfiles-0.0.5/README.md
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)       38 2023-05-04 15:29:38.737907 textfiles-0.0.5/setup.cfg
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     1044 2023-05-04 15:29:30.000000 textfiles-0.0.5/setup.py
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:29:38.737907 textfiles-0.0.5/tests/
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      832 2023-03-09 05:46:03.000000 textfiles-0.0.5/tests/test_for_csv.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      823 2023-04-02 11:21:54.000000 textfiles-0.0.5/tests/tests_for_txt.py
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:29:38.737907 textfiles-0.0.5/textfiles/
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:17:13.000000 textfiles-0.0.5/textfiles/__init__.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     9423 2023-05-04 15:28:40.000000 textfiles-0.0.5/textfiles/csv_file.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     1395 2023-05-04 15:27:17.000000 textfiles-0.0.5/textfiles/exceptions.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2580 2023-05-04 15:18:39.000000 textfiles-0.0.5/textfiles/file_factory.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     8496 2023-05-04 15:18:39.000000 textfiles-0.0.5/textfiles/json_file.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2427 2023-05-04 15:18:39.000000 textfiles-0.0.5/textfiles/text_file_parent.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     3735 2023-05-04 15:18:39.000000 textfiles-0.0.5/textfiles/txt_file.py
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:29:38.737907 textfiles-0.0.5/textfiles.egg-info/
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 15:29:38.000000 textfiles-0.0.5/textfiles.egg-info/PKG-INFO
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      372 2023-05-04 15:29:38.000000 textfiles-0.0.5/textfiles.egg-info/SOURCES.txt
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)        1 2023-05-04 15:29:38.000000 textfiles-0.0.5/textfiles.egg-info/dependency_links.txt
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)       10 2023-05-04 15:29:38.000000 textfiles-0.0.5/textfiles.egg-info/top_level.txt
```

### Comparing `textfiles-0.0.4/LICENSE` & `textfiles-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.4/PKG-INFO` & `textfiles-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: textfiles
-Version: 0.0.4
+Version: 0.0.5
 Summary: Managing the text files txt, csv and json
 Author: Yael Ben Yair, Hemed Tov
 Author-email:  <yaelmadmon1011@gmail.com>, <hemedbz@gmail.com>
 Keywords: python,text,file,csv,json,txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# TextFiles v0.0.4
+# TextFiles v0.0.5
 A convenient Python API for working with the text files CSV, JSON, TXT
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
```

### Comparing `textfiles-0.0.4/README.md` & `textfiles-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TextFiles v0.0.4
+# TextFiles v0.0.5
 A convenient Python API for working with the text files CSV, JSON, TXT
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
```

### Comparing `textfiles-0.0.4/setup.py` & `textfiles-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as fh:
     readme = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Managing the text files txt, csv and json'
 LONG_DESCRIPTION = 'A package that includes friendly API for using the text files in the formats csv, ' \
                    'txt and json.'
 
 # Setting up
 setup(
     name="textfiles",
```

### Comparing `textfiles-0.0.4/tests/test_for_csv.py` & `textfiles-0.0.5/tests/test_for_csv.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.4/tests/tests_for_txt.py` & `textfiles-0.0.5/tests/tests_for_txt.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.4/textfiles/csv_file.py` & `textfiles-0.0.5/textfiles/csv_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from text_file_parent import TextFile
+from .text_file_parent import TextFile
 import csv, os
 from .exceptions import *
 
 # Menu for this file:
     # built-in functions
     # public functions - read
     # math functions - write
```

### Comparing `textfiles-0.0.4/textfiles/exceptions.py` & `textfiles-0.0.5/textfiles/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,14 @@
 class IndexValueError(TextFileExceptions):
     def __init__(self, msg):
         super().__init__(msg)
 
 
 class InvalidTypeError(TextFileExceptions):
         def __init__(self, param):
-        super().__init__(f'{param} file not supported')
+            super().__init__(f'{param} file not supported')
 
 
 class SizeError(TextFileExceptions):
         def __init__(self, param):
-        super().__init__(f'{param} is too large')
+            super().__init__(f'{param} is too large')
```

### Comparing `textfiles-0.0.4/textfiles/file_factory.py` & `textfiles-0.0.5/textfiles/file_factory.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.4/textfiles/json_file.py` & `textfiles-0.0.5/textfiles/json_file.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.4/textfiles/text_file_parent.py` & `textfiles-0.0.5/textfiles/text_file_parent.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.4/textfiles/txt_file.py` & `textfiles-0.0.5/textfiles/txt_file.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.4/textfiles.egg-info/PKG-INFO` & `textfiles-0.0.5/textfiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: textfiles
-Version: 0.0.4
+Version: 0.0.5
 Summary: Managing the text files txt, csv and json
 Author: Yael Ben Yair, Hemed Tov
 Author-email:  <yaelmadmon1011@gmail.com>, <hemedbz@gmail.com>
 Keywords: python,text,file,csv,json,txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# TextFiles v0.0.4
+# TextFiles v0.0.5
 A convenient Python API for working with the text files CSV, JSON, TXT
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
```

