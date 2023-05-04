# Comparing `tmp/gotji-1.0.1.tar.gz` & `tmp/gotji-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotji-1.0.1.tar", last modified: Thu May  4 07:09:29 2023, max compression
+gzip compressed data, was "gotji-1.0.2.tar", last modified: Thu May  4 07:15:50 2023, max compression
```

## Comparing `gotji-1.0.1.tar` & `gotji-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:09:29.507990 gotji-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 07:09:12.000000 gotji-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:09:29.507990 gotji-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 07:09:12.000000 gotji-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:09:29.503990 gotji-1.0.1/gotji/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 07:09:12.000000 gotji-1.0.1/gotji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 07:09:12.000000 gotji-1.0.1/gotji/gotji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:09:29.507990 gotji-1.0.1/gotji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:09:29.000000 gotji-1.0.1/gotji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 07:09:29.000000 gotji-1.0.1/gotji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:09:29.000000 gotji-1.0.1/gotji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 07:09:29.000000 gotji-1.0.1/gotji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 07:09:29.000000 gotji-1.0.1/gotji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 07:09:12.000000 gotji-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:09:29.507990 gotji-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-04 07:09:12.000000 gotji-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:15:50.756934 gotji-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 07:15:39.000000 gotji-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:15:50.756934 gotji-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 07:15:39.000000 gotji-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:15:50.756934 gotji-1.0.2/gotji/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:15:39.000000 gotji-1.0.2/gotji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 07:15:39.000000 gotji-1.0.2/gotji/gotji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:15:50.756934 gotji-1.0.2/gotji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:15:50.000000 gotji-1.0.2/gotji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 07:15:50.000000 gotji-1.0.2/gotji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:15:50.000000 gotji-1.0.2/gotji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 07:15:50.000000 gotji-1.0.2/gotji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 07:15:50.000000 gotji-1.0.2/gotji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 07:15:39.000000 gotji-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:15:50.756934 gotji-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 07:15:39.000000 gotji-1.0.2/setup.py
```

### Comparing `gotji-1.0.1/LICENSE` & `gotji-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gotji-1.0.1/PKG-INFO` & `gotji-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotji
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dev by Meoaw
 Home-page: https://github.com/exaDev99/gotji
 Author: exaDev99
 Author-email: meoawdev.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gotji-1.0.1/gotji.egg-info/PKG-INFO` & `gotji-1.0.2/gotji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotji
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dev by Meoaw
 Home-page: https://github.com/exaDev99/gotji
 Author: exaDev99
 Author-email: meoawdev.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gotji-1.0.1/setup.py` & `gotji-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gotji",
-    version="1.0.1",
+    version="1.0.2",
     description="Dev by Meoaw",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/exaDev99/gotji",
     author="exaDev99",
     author_email="meoawdev.me@gmail.com",
     license="MIT",
@@ -20,8 +20,8 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "requests",
         "pystyle"
     ],
-)
+)
```

