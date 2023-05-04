# Comparing `tmp/textfiles-0.0.3.tar.gz` & `tmp/textfiles-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textfiles-0.0.3.tar", last modified: Thu May  4 12:54:43 2023, max compression
+gzip compressed data, was "textfiles-0.0.4.tar", last modified: Thu May  4 15:18:54 2023, max compression
```

## Comparing `textfiles-0.0.3.tar` & `textfiles-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 12:54:43.956968 textfiles-0.0.3/
--rwxrwxrwx   0 hemed     (1000) hemed     (1000)     1087 2023-01-12 08:44:14.000000 textfiles-0.0.3/LICENSE
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 12:54:43.956968 textfiles-0.0.3/PKG-INFO
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2272 2023-05-04 12:50:33.000000 textfiles-0.0.3/README.md
--rw-rw-r--   0 hemed     (1000) hemed     (1000)       38 2023-05-04 12:54:43.956968 textfiles-0.0.3/setup.cfg
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     1044 2023-05-04 12:50:33.000000 textfiles-0.0.3/setup.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 12:54:43.952968 textfiles-0.0.3/tests/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      832 2023-03-09 05:46:03.000000 textfiles-0.0.3/tests/test_for_csv.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      823 2023-04-02 11:21:54.000000 textfiles-0.0.3/tests/tests_for_txt.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 12:54:43.956968 textfiles-0.0.3/textfiles/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      185 2023-04-02 11:25:23.000000 textfiles-0.0.3/textfiles/__init__.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     9421 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/csv_file.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     1387 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/exceptions.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2576 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/file_factory.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     8494 2023-04-19 18:51:27.000000 textfiles-0.0.3/textfiles/json_file.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2426 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/text_file_parent.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     3733 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/txt_file.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 12:54:43.956968 textfiles-0.0.3/textfiles.egg-info/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 12:54:43.000000 textfiles-0.0.3/textfiles.egg-info/PKG-INFO
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      372 2023-05-04 12:54:43.000000 textfiles-0.0.3/textfiles.egg-info/SOURCES.txt
--rw-rw-r--   0 hemed     (1000) hemed     (1000)        1 2023-05-04 12:54:43.000000 textfiles-0.0.3/textfiles.egg-info/dependency_links.txt
--rw-rw-r--   0 hemed     (1000) hemed     (1000)       10 2023-05-04 12:54:43.000000 textfiles-0.0.3/textfiles.egg-info/top_level.txt
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:18:54.563207 textfiles-0.0.4/
+-rwxrwxrwx   0 hemed     (1000) hemed     (1000)     1087 2023-01-12 08:44:14.000000 textfiles-0.0.4/LICENSE
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 15:18:54.563207 textfiles-0.0.4/PKG-INFO
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2272 2023-05-04 15:17:13.000000 textfiles-0.0.4/README.md
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)       38 2023-05-04 15:18:54.563207 textfiles-0.0.4/setup.cfg
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     1044 2023-05-04 15:17:13.000000 textfiles-0.0.4/setup.py
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:18:54.559208 textfiles-0.0.4/tests/
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      832 2023-03-09 05:46:03.000000 textfiles-0.0.4/tests/test_for_csv.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      823 2023-04-02 11:21:54.000000 textfiles-0.0.4/tests/tests_for_txt.py
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:18:54.559208 textfiles-0.0.4/textfiles/
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:17:13.000000 textfiles-0.0.4/textfiles/__init__.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     9422 2023-05-04 15:18:38.000000 textfiles-0.0.4/textfiles/csv_file.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     1387 2023-04-19 18:50:04.000000 textfiles-0.0.4/textfiles/exceptions.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2580 2023-05-04 15:18:39.000000 textfiles-0.0.4/textfiles/file_factory.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     8496 2023-05-04 15:18:39.000000 textfiles-0.0.4/textfiles/json_file.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2427 2023-05-04 15:18:39.000000 textfiles-0.0.4/textfiles/text_file_parent.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     3735 2023-05-04 15:18:39.000000 textfiles-0.0.4/textfiles/txt_file.py
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 15:18:54.559208 textfiles-0.0.4/textfiles.egg-info/
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 15:18:54.000000 textfiles-0.0.4/textfiles.egg-info/PKG-INFO
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      372 2023-05-04 15:18:54.000000 textfiles-0.0.4/textfiles.egg-info/SOURCES.txt
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)        1 2023-05-04 15:18:54.000000 textfiles-0.0.4/textfiles.egg-info/dependency_links.txt
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)       10 2023-05-04 15:18:54.000000 textfiles-0.0.4/textfiles.egg-info/top_level.txt
```

### Comparing `textfiles-0.0.3/LICENSE` & `textfiles-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.3/PKG-INFO` & `textfiles-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: textfiles
-Version: 0.0.3
+Version: 0.0.4
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
 
 
-# TextFiles v0.0.3
+# TextFiles v0.0.4
 A convenient Python API for working with the text files CSV, JSON, TXT
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
```

### Comparing `textfiles-0.0.3/README.md` & `textfiles-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TextFiles v0.0.3
+# TextFiles v0.0.4
 A convenient Python API for working with the text files CSV, JSON, TXT
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
```

### Comparing `textfiles-0.0.3/setup.py` & `textfiles-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as fh:
     readme = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Managing the text files txt, csv and json'
 LONG_DESCRIPTION = 'A package that includes friendly API for using the text files in the formats csv, ' \
                    'txt and json.'
 
 # Setting up
 setup(
     name="textfiles",
```

### Comparing `textfiles-0.0.3/tests/test_for_csv.py` & `textfiles-0.0.4/tests/test_for_csv.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.3/tests/tests_for_txt.py` & `textfiles-0.0.4/tests/tests_for_txt.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.3/textfiles/csv_file.py` & `textfiles-0.0.4/textfiles/csv_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from text_file_parent import TextFile
 import csv, os
-from exceptions import *
+from .exceptions import *
 
 # Menu for this file:
     # built-in functions
     # public functions - read
     # math functions - write
     # private functions
```

### Comparing `textfiles-0.0.3/textfiles/exceptions.py` & `textfiles-0.0.4/textfiles/exceptions.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.3/textfiles/file_factory.py` & `textfiles-0.0.4/textfiles/file_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json, csv
 import os.path
-from csv_file import CsvFile
-from json_file import JsonFile
-from txt_file import TxtFile
-from exceptions import *
+from .csv_file import CsvFile
+from .json_file import JsonFile
+from .txt_file import TxtFile
+from .exceptions import *
 
 
 class TextFile:
 
     @staticmethod
     def make_file_instance(path: str, filetype: str, has_header: bool = True, delimiter: str = ',', max_size: int = 50)\
             ->\
```

### Comparing `textfiles-0.0.3/textfiles/json_file.py` & `textfiles-0.0.4/textfiles/json_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from text_file_parent import TextFile
+from .text_file_parent import TextFile
 import json
 import re
-from exceptions import *
+from .exceptions import *
 
 
 class JsonFile(TextFile):
 
     def __init__(self, file_path: str):
         """
         :param file_path: str
```

### Comparing `textfiles-0.0.3/textfiles/text_file_parent.py` & `textfiles-0.0.4/textfiles/text_file_parent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 import os
-from exceptions import *
+from .exceptions import *
 import time
 from threading import Lock
 
 
 class TextFile(ABC):
 
     def __init__(self, file_path: str):
```

### Comparing `textfiles-0.0.3/textfiles/txt_file.py` & `textfiles-0.0.4/textfiles/txt_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from text_file_parent import TextFile
-from exceptions import *
+from .text_file_parent import TextFile
+from .exceptions import *
 import os
 
 
 class TxtFile (TextFile):
     """
     The class corresponds to a txt file, allowing an easy API for handling it.
     To initiate, simply provide the file path as a string.
```

### Comparing `textfiles-0.0.3/textfiles.egg-info/PKG-INFO` & `textfiles-0.0.4/textfiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: textfiles
-Version: 0.0.3
+Version: 0.0.4
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
 
 
-# TextFiles v0.0.3
+# TextFiles v0.0.4
 A convenient Python API for working with the text files CSV, JSON, TXT
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
```

