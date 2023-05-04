# Comparing `tmp/textfiles-0.0.6.tar.gz` & `tmp/textfiles-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textfiles-0.0.6.tar", last modified: Thu May  4 16:42:09 2023, max compression
+gzip compressed data, was "textfiles-0.0.7.tar", last modified: Thu May  4 17:56:45 2023, max compression
```

## Comparing `textfiles-0.0.6.tar` & `textfiles-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:42:09.241960 textfiles-0.0.6/
--rw-rw-rw-   0        0        0     1087 2023-01-12 08:45:31.000000 textfiles-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3004 2023-05-04 16:42:09.240960 textfiles-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2347 2023-05-04 16:32:01.000000 textfiles-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 16:42:09.242960 textfiles-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-05-04 16:32:01.000000 textfiles-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:42:09.224950 textfiles-0.0.6/textfiles/
--rw-rw-rw-   0        0        0        0 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/__init__.py
--rw-rw-rw-   0        0        0     9737 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/csv_file.py
--rw-rw-rw-   0        0        0     1455 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/exceptions.py
--rw-rw-rw-   0        0        0     2673 2023-05-04 16:27:12.000000 textfiles-0.0.6/textfiles/file_factory.py
--rw-rw-rw-   0        0        0     8710 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/json_file.py
--rw-rw-rw-   0        0        0     2529 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/text_file_parent.py
--rw-rw-rw-   0        0        0     3867 2023-05-04 16:24:25.000000 textfiles-0.0.6/textfiles/txt_file.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:42:09.239961 textfiles-0.0.6/textfiles.egg-info/
--rw-rw-rw-   0        0        0     3004 2023-05-04 16:42:09.000000 textfiles-0.0.6/textfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-05-04 16:42:09.000000 textfiles-0.0.6/textfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:42:09.000000 textfiles-0.0.6/textfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 16:42:09.000000 textfiles-0.0.6/textfiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 17:56:45.444088 textfiles-0.0.7/
+-rw-rw-rw-   0        0        0     1087 2023-01-12 08:45:31.000000 textfiles-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3004 2023-05-04 17:56:45.443115 textfiles-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2347 2023-05-04 17:53:09.000000 textfiles-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:56:45.444088 textfiles-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-05-04 17:53:09.000000 textfiles-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:56:45.435122 textfiles-0.0.7/textfiles/
+-rw-rw-rw-   0        0        0        0 2023-05-04 16:24:25.000000 textfiles-0.0.7/textfiles/__init__.py
+-rw-rw-rw-   0        0        0     9737 2023-05-04 16:24:25.000000 textfiles-0.0.7/textfiles/csv_file.py
+-rw-rw-rw-   0        0        0     1455 2023-05-04 16:24:25.000000 textfiles-0.0.7/textfiles/exceptions.py
+-rw-rw-rw-   0        0        0     2673 2023-05-04 17:51:28.000000 textfiles-0.0.7/textfiles/file_factory.py
+-rw-rw-rw-   0        0        0     8943 2023-05-04 17:50:36.000000 textfiles-0.0.7/textfiles/json_file.py
+-rw-rw-rw-   0        0        0     2529 2023-05-04 16:24:25.000000 textfiles-0.0.7/textfiles/text_file_parent.py
+-rw-rw-rw-   0        0        0     3867 2023-05-04 16:24:25.000000 textfiles-0.0.7/textfiles/txt_file.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:56:45.442085 textfiles-0.0.7/textfiles.egg-info/
+-rw-rw-rw-   0        0        0     3004 2023-05-04 17:56:45.000000 textfiles-0.0.7/textfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-05-04 17:56:45.000000 textfiles-0.0.7/textfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:56:45.000000 textfiles-0.0.7/textfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 17:56:45.000000 textfiles-0.0.7/textfiles.egg-info/top_level.txt
```

### Comparing `textfiles-0.0.6/LICENSE` & `textfiles-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.6/PKG-INFO` & `textfiles-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textfiles
-Version: 0.0.6
+Version: 0.0.7
 Summary: Managing the text files txt, csv and json
 Home-page: UNKNOWN
 Author: Yael Ben Yair, Hemed Tov
 Author-email:  <yaelmadmon1011@gmail.com>, <hemedbz@gmail.com>
 License: UNKNOWN
 Keywords: python,text,file,csv,json,txt
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# TextFiles v0.0.6
+# TextFiles v0.0.7
 A convenient Python API for working with the text files CSV, JSON, TXT
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
@@ -45,17 +45,17 @@
 To create an instance of a CsvFile, TxtFile, or JsonFile class, simply call the appropriate static method and pass in the necessary parameters. The factory will then return an instance of the appropriate class.
 
 Examples: Here are some examples of how to use TextFile:
 
 To create an instance of an existing file:
 
 ```python
-file = TextFile.make_file_instance('path/to/file.csv', 'csv', has_header=True, delimiter=',')
-file = TextFile.make_file_instance('path/to/file.txt', 'txt')
-file = TextFile.make_file_instance('path/to/file.json', 'json')
+file = TextFile.make_file_instance('csv', 'path/to/file.csv', has_header=True, delimiter=',')
+file = TextFile.make_file_instance('txt', 'path/to/file.txt')
+file = TextFile.make_file_instance('json', 'path/to/file.json')
 ```
 
 To create a new file:
 
 ```python
 file = TextFile.make_file('csv', 'path/to/file.csv', ['Header1', 'Header2'])
 file = TextFile.make_file('txt', 'path/to/file.txt')
```

### Comparing `textfiles-0.0.6/README.md` & `textfiles-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TextFiles v0.0.6
+# TextFiles v0.0.7
 A convenient Python API for working with the text files CSV, JSON, TXT
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
@@ -25,17 +25,17 @@
 To create an instance of a CsvFile, TxtFile, or JsonFile class, simply call the appropriate static method and pass in the necessary parameters. The factory will then return an instance of the appropriate class.
 
 Examples: Here are some examples of how to use TextFile:
 
 To create an instance of an existing file:
 
 ```python
-file = TextFile.make_file_instance('path/to/file.csv', 'csv', has_header=True, delimiter=',')
-file = TextFile.make_file_instance('path/to/file.txt', 'txt')
-file = TextFile.make_file_instance('path/to/file.json', 'json')
+file = TextFile.make_file_instance('csv', 'path/to/file.csv', has_header=True, delimiter=',')
+file = TextFile.make_file_instance('txt', 'path/to/file.txt')
+file = TextFile.make_file_instance('json', 'path/to/file.json')
 ```
 
 To create a new file:
 
 ```python
 file = TextFile.make_file('csv', 'path/to/file.csv', ['Header1', 'Header2'])
 file = TextFile.make_file('txt', 'path/to/file.txt')
```

### Comparing `textfiles-0.0.6/setup.py` & `textfiles-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as fh:
     readme = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Managing the text files txt, csv and json'
 LONG_DESCRIPTION = 'A package that includes friendly API for using the text files in the formats csv, ' \
                    'txt and json.'
 
 # Setting up
 setup(
     name="textfiles",
```

### Comparing `textfiles-0.0.6/textfiles/csv_file.py` & `textfiles-0.0.7/textfiles/csv_file.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.6/textfiles/exceptions.py` & `textfiles-0.0.7/textfiles/exceptions.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.6/textfiles/file_factory.py` & `textfiles-0.0.7/textfiles/file_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .txt_file import TxtFile
 from .exceptions import *
 
 
 class TextFile:
 
     @staticmethod
-    def make_file_instance(path: str, filetype: str, has_header: bool = True, delimiter: str = ',', max_size: int = 50)\
+    def make_file_instance(filetype: str, path: str, has_header: bool = True, delimiter: str = ',', max_size: int = 50)\
             ->\
             CsvFile | TxtFile | JsonFile:
         """
         This functions creates a file class instance for an existing text file.
         If the file type is not one of the three specified -> txt, csv, json,
         it will not be possible to use the library.
         :param filetype: str (csv/json/txt).
```

### Comparing `textfiles-0.0.6/textfiles/json_file.py` & `textfiles-0.0.7/textfiles/json_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,41 +114,48 @@
                 If the item is a dictionary, it must include a key
         :param new_value: The value that you want to add.
         :param to_list: True, if you want to add the value to a list, otherwise False -
                 False is the default. -> only if type - only if the type is str, int, or float.
         """
 
         file_content = self.content
+        file_type = ''
         self.lock.acquire()
 
         # check if content_locator is None - if True insert to content the whole content
         if content_locator is None:
             content = self.content
         else:
             content = self._locator(content_locator)
 
         # content = file_content[content_locator]
         tyc = type(content)
         if tyc == dict:
             if new_key is None:
                 raise KeyError("For dictionary type must insert a key")
             content = self._add_data_dict(content, new_key, new_value)
+            file_type = {}
         elif tyc == list:
             content = self._add_data_list(content, new_index, new_value)
+            file_type = []
         elif tyc == str:
             content = self._add_data_str(content, new_value, to_list)
         elif tyc == float or tyc == int:
             content = self._add_data_num(content, new_value, to_list)
         elif tyc == bool:
             content = self._add_data_bool(content, new_value)
         elif content is None:
             content = new_value
             # self._add_data_none(content, new_value)
 
-        exec(f"file_content{content_locator} = content\nself._content = file_content")
+        if self.content is None:
+            self._content = content
+        else:
+            exec(f"file_content{content_locator} = content\nself._content = file_content")
+        # exec(f"self._content[{content_locator}] = content")
 
         self._dump_content()
         self.lock.release()
 
     def remove_data(self, content_locator: str, key: str | int = None, index: int = None):
         """
         removes specific data from json for type -> list, dict only
```

### Comparing `textfiles-0.0.6/textfiles/text_file_parent.py` & `textfiles-0.0.7/textfiles/text_file_parent.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.6/textfiles/txt_file.py` & `textfiles-0.0.7/textfiles/txt_file.py`

 * *Files identical despite different names*

### Comparing `textfiles-0.0.6/textfiles.egg-info/PKG-INFO` & `textfiles-0.0.7/textfiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textfiles
-Version: 0.0.6
+Version: 0.0.7
 Summary: Managing the text files txt, csv and json
 Home-page: UNKNOWN
 Author: Yael Ben Yair, Hemed Tov
 Author-email:  <yaelmadmon1011@gmail.com>, <hemedbz@gmail.com>
 License: UNKNOWN
 Keywords: python,text,file,csv,json,txt
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# TextFiles v0.0.6
+# TextFiles v0.0.7
 A convenient Python API for working with the text files CSV, JSON, TXT
 
 The library allows handling csv, txt and json files easily from within Python.
 
 ## Installation
 ```terminal
 pip install textfiles
@@ -45,17 +45,17 @@
 To create an instance of a CsvFile, TxtFile, or JsonFile class, simply call the appropriate static method and pass in the necessary parameters. The factory will then return an instance of the appropriate class.
 
 Examples: Here are some examples of how to use TextFile:
 
 To create an instance of an existing file:
 
 ```python
-file = TextFile.make_file_instance('path/to/file.csv', 'csv', has_header=True, delimiter=',')
-file = TextFile.make_file_instance('path/to/file.txt', 'txt')
-file = TextFile.make_file_instance('path/to/file.json', 'json')
+file = TextFile.make_file_instance('csv', 'path/to/file.csv', has_header=True, delimiter=',')
+file = TextFile.make_file_instance('txt', 'path/to/file.txt')
+file = TextFile.make_file_instance('json', 'path/to/file.json')
 ```
 
 To create a new file:
 
 ```python
 file = TextFile.make_file('csv', 'path/to/file.csv', ['Header1', 'Header2'])
 file = TextFile.make_file('txt', 'path/to/file.txt')
```

