# Comparing `tmp/ABCParse-0.0.3rc0.tar.gz` & `tmp/ABCParse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABCParse-0.0.3rc0.tar", last modified: Sun Apr  9 04:45:15 2023, max compression
+gzip compressed data, was "ABCParse-0.0.4.tar", last modified: Thu May  4 14:52:52 2023, max compression
```

## Comparing `ABCParse-0.0.3rc0.tar` & `ABCParse-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/ABCParse/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/ABCParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/ABCParse/_abc_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/ABCParse/_function_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/ABCParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-09 04:45:14.000000 ABCParse-0.0.3rc0/ABCParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-09 04:45:14.000000 ABCParse-0.0.3rc0/ABCParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 04:45:14.000000 ABCParse-0.0.3rc0/ABCParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 04:45:14.000000 ABCParse-0.0.3rc0/ABCParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:52.793101 ABCParse-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:52.789101 ABCParse-0.0.4/ABCParse/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-04 14:52:37.000000 ABCParse-0.0.4/ABCParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-04 14:52:37.000000 ABCParse-0.0.4/ABCParse/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-04 14:52:37.000000 ABCParse-0.0.4/ABCParse/_function_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:52.789101 ABCParse-0.0.4/ABCParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-04 14:52:52.000000 ABCParse-0.0.4/ABCParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 14:52:52.000000 ABCParse-0.0.4/ABCParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:52:52.000000 ABCParse-0.0.4/ABCParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 14:52:52.000000 ABCParse-0.0.4/ABCParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-04 14:52:37.000000 ABCParse-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-04 14:52:52.789101 ABCParse-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-04 14:52:37.000000 ABCParse-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:52:52.793101 ABCParse-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 14:52:37.000000 ABCParse-0.0.4/setup.py
```

### Comparing `ABCParse-0.0.3rc0/ABCParse/_abc_parse.py` & `ABCParse-0.0.4/ABCParse/_abc_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,19 @@
         
         for key, val in kwargs_val.items():
             self.__collect__(key, val)
     
     def __hide__(self, key):
         return "_{}".format(key)
 
-    def __collect__(self, key, val):
+    def __collect__(self, key, hidden_key, val):
         if not hasattr(self, "_PARAMS"):
             self.__init_kwargs__()
             
-        self._PARAMS[key] = val
+        self._PARAMS[hidden_key] = val
         setattr(self, key, val)
 
     def __parse__(
         self,
         kwargs:  dict,
         ignore:  list = ["self"],
         private: list = ["ignore", "private", "public"],
@@ -102,9 +102,9 @@
 
         for key, val in kwargs.items():
             if not key in ignore:
                 if key == kwargs_key:
                     self._collect_literal_kwargs(val)
                 else:
                     if (key in private) and (not key in public):
-                        key = self.__hide__(key)
-                    self.__collect__(key, val)
+                        hidden_key = self.__hide__(key)
+                    self.__collect__(key, hidden_key, val)
```

### Comparing `ABCParse-0.0.3rc0/ABCParse/_function_kwargs.py` & `ABCParse-0.0.4/ABCParse/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.3rc0/ABCParse.egg-info/PKG-INFO` & `ABCParse-0.0.4/ABCParse.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ABCParse
-Version: 0.0.3rc0
+Version: 0.0.4
 Summary: A better base class to automatically parse local args.
 Author: Michael E. Vinyard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >3.7.0
+Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ABCParse
 
 ![Python Tests](https://github.com/mvinyard/ABCParse/actions/workflows/python-tests.yml/badge.svg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ABCParse.svg)](https://pypi.python.org/pypi/ABCParse/)
```

### Comparing `ABCParse-0.0.3rc0/LICENSE` & `ABCParse-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.3rc0/PKG-INFO` & `ABCParse-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ABCParse
-Version: 0.0.3rc0
+Version: 0.0.4
 Summary: A better base class to automatically parse local args.
 Author: Michael E. Vinyard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >3.7.0
+Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ABCParse
 
 ![Python Tests](https://github.com/mvinyard/ABCParse/actions/workflows/python-tests.yml/badge.svg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ABCParse.svg)](https://pypi.python.org/pypi/ABCParse/)
```

### Comparing `ABCParse-0.0.3rc0/README.md` & `ABCParse-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.3rc0/setup.py` & `ABCParse-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="ABCParse",
-    version="0.0.3rc0",
-    python_requires=">3.7.0",
+    version="0.0.4",
+    python_requires=">3.9.0",
     author="Michael E. Vinyard",
     author_email="mvinyard@broadinstitute.org",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="A better base class to automatically parse local args.",
     packages=setuptools.find_packages(),
     install_requires=[],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     license="MIT",
 )
```

