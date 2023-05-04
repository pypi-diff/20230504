# Comparing `tmp/gotji-1.0.5.tar.gz` & `tmp/gotji-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotji-1.0.5.tar", last modified: Thu May  4 07:52:02 2023, max compression
+gzip compressed data, was "gotji-1.0.6.tar", last modified: Thu May  4 08:01:32 2023, max compression
```

## Comparing `gotji-1.0.5.tar` & `gotji-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:52:02.142089 gotji-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 07:51:48.000000 gotji-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:52:02.142089 gotji-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 07:51:48.000000 gotji-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:52:02.142089 gotji-1.0.5/gotji/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 07:51:48.000000 gotji-1.0.5/gotji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-04 07:51:48.000000 gotji-1.0.5/gotji/gotji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:52:02.142089 gotji-1.0.5/gotji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 07:51:48.000000 gotji-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:52:02.142089 gotji-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-04 07:51:48.000000 gotji-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:32.916507 gotji-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 08:01:19.000000 gotji-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 08:01:32.916507 gotji-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 08:01:19.000000 gotji-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:32.916507 gotji-1.0.6/gotji/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 08:01:19.000000 gotji-1.0.6/gotji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-04 08:01:19.000000 gotji-1.0.6/gotji/gotji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:01:32.916507 gotji-1.0.6/gotji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 08:01:32.000000 gotji-1.0.6/gotji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 08:01:32.000000 gotji-1.0.6/gotji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:01:32.000000 gotji-1.0.6/gotji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 08:01:32.000000 gotji-1.0.6/gotji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 08:01:32.000000 gotji-1.0.6/gotji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 08:01:19.000000 gotji-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:01:32.916507 gotji-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-04 08:01:19.000000 gotji-1.0.6/setup.py
```

### Comparing `gotji-1.0.5/LICENSE` & `gotji-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gotji-1.0.5/PKG-INFO` & `gotji-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotji
-Version: 1.0.5
+Version: 1.0.6
 Summary: Dev by Meoaw
 Home-page: https://github.com/exaDev99/gotji
 Author: exaDev99
 Author-email: meoawdev.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gotji-1.0.5/gotji/gotji.py` & `gotji-1.0.6/gotji/gotji.py`

 * *Files identical despite different names*

### Comparing `gotji-1.0.5/gotji.egg-info/PKG-INFO` & `gotji-1.0.6/gotji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotji
-Version: 1.0.5
+Version: 1.0.6
 Summary: Dev by Meoaw
 Home-page: https://github.com/exaDev99/gotji
 Author: exaDev99
 Author-email: meoawdev.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gotji-1.0.5/setup.py` & `gotji-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gotji",
-    version="1.0.5",
+    version="1.0.6",
     description="Dev by Meoaw",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/exaDev99/gotji",
     author="exaDev99",
     author_email="meoawdev.me@gmail.com",
     license="MIT",
```

