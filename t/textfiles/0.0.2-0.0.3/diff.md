# Comparing `tmp/textfiles-0.0.2.tar.gz` & `tmp/textfiles-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textfiles-0.0.2.tar", last modified: Wed Apr 19 21:59:26 2023, max compression
+gzip compressed data, was "textfiles-0.0.3.tar", last modified: Thu May  4 12:54:43 2023, max compression
```

## Comparing `textfiles-0.0.2.tar` & `textfiles-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-04-19 21:59:26.195616 textfiles-0.0.2/
--rwxrwxrwx   0 hemed     (1000) hemed     (1000)     1087 2023-01-12 08:44:14.000000 textfiles-0.0.2/LICENSE
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2928 2023-04-19 21:59:26.195616 textfiles-0.0.2/PKG-INFO
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2349 2023-04-02 12:49:17.000000 textfiles-0.0.2/README.md
--rw-rw-r--   0 hemed     (1000) hemed     (1000)       38 2023-04-19 21:59:26.195616 textfiles-0.0.2/setup.cfg
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     1054 2023-04-19 21:57:55.000000 textfiles-0.0.2/setup.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-04-19 21:59:26.191615 textfiles-0.0.2/tests/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      832 2023-03-09 05:46:03.000000 textfiles-0.0.2/tests/test_for_csv.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      823 2023-04-02 11:21:54.000000 textfiles-0.0.2/tests/tests_for_txt.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-04-19 21:59:26.191615 textfiles-0.0.2/textfiles/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      185 2023-04-02 11:25:23.000000 textfiles-0.0.2/textfiles/__init__.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     9421 2023-04-19 18:50:04.000000 textfiles-0.0.2/textfiles/csv_file.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     1387 2023-04-19 18:50:04.000000 textfiles-0.0.2/textfiles/exceptions.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2576 2023-04-19 18:50:04.000000 textfiles-0.0.2/textfiles/file_factory.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     8494 2023-04-19 18:51:27.000000 textfiles-0.0.2/textfiles/json_file.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2426 2023-04-19 18:50:04.000000 textfiles-0.0.2/textfiles/text_file_parent.py
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     3733 2023-04-19 18:50:04.000000 textfiles-0.0.2/textfiles/txt_file.py
-drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-04-19 21:59:26.195616 textfiles-0.0.2/textfiles.egg-info/
--rw-rw-r--   0 hemed     (1000) hemed     (1000)     2928 2023-04-19 21:59:26.000000 textfiles-0.0.2/textfiles.egg-info/PKG-INFO
--rw-rw-r--   0 hemed     (1000) hemed     (1000)      404 2023-04-19 21:59:26.000000 textfiles-0.0.2/textfiles.egg-info/SOURCES.txt
--rw-rw-r--   0 hemed     (1000) hemed     (1000)        1 2023-04-19 21:59:26.000000 textfiles-0.0.2/textfiles.egg-info/dependency_links.txt
--rw-rw-r--   0 hemed     (1000) hemed     (1000)        9 2023-04-19 21:59:26.000000 textfiles-0.0.2/textfiles.egg-info/requires.txt
--rw-rw-r--   0 hemed     (1000) hemed     (1000)       10 2023-04-19 21:59:26.000000 textfiles-0.0.2/textfiles.egg-info/top_level.txt
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 12:54:43.956968 textfiles-0.0.3/
+-rwxrwxrwx   0 hemed     (1000) hemed     (1000)     1087 2023-01-12 08:44:14.000000 textfiles-0.0.3/LICENSE
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 12:54:43.956968 textfiles-0.0.3/PKG-INFO
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2272 2023-05-04 12:50:33.000000 textfiles-0.0.3/README.md
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)       38 2023-05-04 12:54:43.956968 textfiles-0.0.3/setup.cfg
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     1044 2023-05-04 12:50:33.000000 textfiles-0.0.3/setup.py
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 12:54:43.952968 textfiles-0.0.3/tests/
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      832 2023-03-09 05:46:03.000000 textfiles-0.0.3/tests/test_for_csv.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      823 2023-04-02 11:21:54.000000 textfiles-0.0.3/tests/tests_for_txt.py
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 12:54:43.956968 textfiles-0.0.3/textfiles/
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      185 2023-04-02 11:25:23.000000 textfiles-0.0.3/textfiles/__init__.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     9421 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/csv_file.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     1387 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/exceptions.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2576 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/file_factory.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     8494 2023-04-19 18:51:27.000000 textfiles-0.0.3/textfiles/json_file.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2426 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/text_file_parent.py
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     3733 2023-04-19 18:50:04.000000 textfiles-0.0.3/textfiles/txt_file.py
+drwxrwxr-x   0 hemed     (1000) hemed     (1000)        0 2023-05-04 12:54:43.956968 textfiles-0.0.3/textfiles.egg-info/
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)     2851 2023-05-04 12:54:43.000000 textfiles-0.0.3/textfiles.egg-info/PKG-INFO
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)      372 2023-05-04 12:54:43.000000 textfiles-0.0.3/textfiles.egg-info/SOURCES.txt
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)        1 2023-05-04 12:54:43.000000 textfiles-0.0.3/textfiles.egg-info/dependency_links.txt
+-rw-rw-r--   0 hemed     (1000) hemed     (1000)       10 2023-05-04 12:54:43.000000 textfiles-0.0.3/textfiles.egg-info/top_level.txt
```

### Comparing `textfiles-0.0.2/LICENSE` & `textfiles-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.2/PKG-INFO` & `textfiles-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: textfiles
-Version: 0.0.2
+Version: 0.0.3
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
 
 
-# TextFiles v0.0.1
+# TextFiles v0.0.3
 A convenient Python API for working with the text files CSV, JSON, TXT
-This is a shared project with Yael Ben Yair `https://github.com/YaelBenYair`
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
 ```
```

### Comparing `textfiles-0.0.2/README.md` & `textfiles-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# TextFiles v0.0.1
+# TextFiles v0.0.3
 A convenient Python API for working with the text files CSV, JSON, TXT
-This is a shared project with Yael Ben Yair `https://github.com/YaelBenYair`
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
 ```
```

### Comparing `textfiles-0.0.2/setup.py` & `textfiles-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as fh:
     readme = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Managing the text files txt, csv and json'
 LONG_DESCRIPTION = 'A package that includes friendly API for using the text files in the formats csv, ' \
                    'txt and json.'
 
 # Setting up
 setup(
     name="textfiles",
     version=VERSION,
     author="Yael Ben Yair, Hemed Tov",
     author_email=" <yaelmadmon1011@gmail.com>, <hemedbz@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(),
-    install_requires=['psycopg2'],
+    install_requires=[],
     keywords=['python', 'text', 'file', 'csv', 'json', 'txt'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `textfiles-0.0.2/tests/test_for_csv.py` & `textfiles-0.0.3/tests/test_for_csv.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.2/tests/tests_for_txt.py` & `textfiles-0.0.3/tests/tests_for_txt.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.2/textfiles/csv_file.py` & `textfiles-0.0.3/textfiles/csv_file.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.2/textfiles/exceptions.py` & `textfiles-0.0.3/textfiles/exceptions.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.2/textfiles/file_factory.py` & `textfiles-0.0.3/textfiles/file_factory.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.2/textfiles/json_file.py` & `textfiles-0.0.3/textfiles/json_file.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.2/textfiles/text_file_parent.py` & `textfiles-0.0.3/textfiles/text_file_parent.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.2/textfiles/txt_file.py` & `textfiles-0.0.3/textfiles/txt_file.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.2/textfiles.egg-info/PKG-INFO` & `textfiles-0.0.3/textfiles.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: textfiles
-Version: 0.0.2
+Version: 0.0.3
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
 
 
-# TextFiles v0.0.1
+# TextFiles v0.0.3
 A convenient Python API for working with the text files CSV, JSON, TXT
-This is a shared project with Yael Ben Yair `https://github.com/YaelBenYair`
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
 ```
```

