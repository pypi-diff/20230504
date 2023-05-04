# Comparing `tmp/gotji-1.0.7.tar.gz` & `tmp/gotji-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotji-1.0.7.tar", last modified: Thu May  4 09:15:17 2023, max compression
+gzip compressed data, was "gotji-1.0.8.tar", last modified: Thu May  4 09:36:32 2023, max compression
```

## Comparing `gotji-1.0.7.tar` & `gotji-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:15:17.470684 gotji-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 09:15:06.000000 gotji-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 09:15:17.470684 gotji-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 09:15:06.000000 gotji-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:15:17.470684 gotji-1.0.7/gotji/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 09:15:06.000000 gotji-1.0.7/gotji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-04 09:15:06.000000 gotji-1.0.7/gotji/gotji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:15:17.470684 gotji-1.0.7/gotji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 09:15:17.000000 gotji-1.0.7/gotji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 09:15:17.000000 gotji-1.0.7/gotji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:15:17.000000 gotji-1.0.7/gotji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 09:15:17.000000 gotji-1.0.7/gotji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 09:15:17.000000 gotji-1.0.7/gotji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 09:15:06.000000 gotji-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:15:17.470684 gotji-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-04 09:15:06.000000 gotji-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:36:32.726493 gotji-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 09:36:20.000000 gotji-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 09:36:32.726493 gotji-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 09:36:20.000000 gotji-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:36:32.722493 gotji-1.0.8/gotji/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 09:36:20.000000 gotji-1.0.8/gotji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-04 09:36:20.000000 gotji-1.0.8/gotji/gotji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:36:32.726493 gotji-1.0.8/gotji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 09:36:32.000000 gotji-1.0.8/gotji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 09:36:32.000000 gotji-1.0.8/gotji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:36:32.000000 gotji-1.0.8/gotji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 09:36:32.000000 gotji-1.0.8/gotji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 09:36:32.000000 gotji-1.0.8/gotji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 09:36:20.000000 gotji-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:36:32.726493 gotji-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 09:36:20.000000 gotji-1.0.8/setup.py
```

### Comparing `gotji-1.0.7/LICENSE` & `gotji-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gotji-1.0.7/PKG-INFO` & `gotji-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotji
-Version: 1.0.7
+Version: 1.0.8
 Summary: Dev by Meoaw
 Home-page: https://github.com/exaDev99/gotji
 Author: exaDev99
 Author-email: meoawdev.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gotji-1.0.7/gotji/gotji.py` & `gotji-1.0.8/gotji/gotji.py`

 * *Files identical despite different names*

### Comparing `gotji-1.0.7/gotji.egg-info/PKG-INFO` & `gotji-1.0.8/gotji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotji
-Version: 1.0.7
+Version: 1.0.8
 Summary: Dev by Meoaw
 Home-page: https://github.com/exaDev99/gotji
 Author: exaDev99
 Author-email: meoawdev.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gotji-1.0.7/setup.py` & `gotji-1.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gotji",
-    version="1.0.7",
+    version="1.0.8",
     description="Dev by Meoaw",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/exaDev99/gotji",
     author="exaDev99",
     author_email="meoawdev.me@gmail.com",
     license="MIT",
@@ -23,8 +23,8 @@
     install_requires=[
         "requests",
         "pystyle",
         "replit",
         "flask",
         "flask_restful"
     ],
-)
+)
```

