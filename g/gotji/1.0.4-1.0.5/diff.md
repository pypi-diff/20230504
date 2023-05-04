# Comparing `tmp/gotji-1.0.4.tar.gz` & `tmp/gotji-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotji-1.0.4.tar", last modified: Thu May  4 07:38:06 2023, max compression
+gzip compressed data, was "gotji-1.0.5.tar", last modified: Thu May  4 07:52:02 2023, max compression
```

## Comparing `gotji-1.0.4.tar` & `gotji-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:38:06.591547 gotji-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 07:37:52.000000 gotji-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:38:06.591547 gotji-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 07:37:52.000000 gotji-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:38:06.591547 gotji-1.0.4/gotji/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 07:37:52.000000 gotji-1.0.4/gotji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-04 07:37:52.000000 gotji-1.0.4/gotji/gotji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:38:06.591547 gotji-1.0.4/gotji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:38:06.000000 gotji-1.0.4/gotji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 07:38:06.000000 gotji-1.0.4/gotji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:38:06.000000 gotji-1.0.4/gotji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 07:38:06.000000 gotji-1.0.4/gotji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 07:38:06.000000 gotji-1.0.4/gotji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 07:37:52.000000 gotji-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:38:06.591547 gotji-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 07:37:52.000000 gotji-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:52:02.142089 gotji-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 07:51:48.000000 gotji-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:52:02.142089 gotji-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 07:51:48.000000 gotji-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:52:02.142089 gotji-1.0.5/gotji/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 07:51:48.000000 gotji-1.0.5/gotji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-04 07:51:48.000000 gotji-1.0.5/gotji/gotji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:52:02.142089 gotji-1.0.5/gotji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 07:52:02.000000 gotji-1.0.5/gotji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 07:51:48.000000 gotji-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:52:02.142089 gotji-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-04 07:51:48.000000 gotji-1.0.5/setup.py
```

### Comparing `gotji-1.0.4/LICENSE` & `gotji-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gotji-1.0.4/PKG-INFO` & `gotji-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotji
-Version: 1.0.4
+Version: 1.0.5
 Summary: Dev by Meoaw
 Home-page: https://github.com/exaDev99/gotji
 Author: exaDev99
 Author-email: meoawdev.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gotji-1.0.4/gotji.egg-info/PKG-INFO` & `gotji-1.0.5/gotji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotji
-Version: 1.0.4
+Version: 1.0.5
 Summary: Dev by Meoaw
 Home-page: https://github.com/exaDev99/gotji
 Author: exaDev99
 Author-email: meoawdev.me@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gotji-1.0.4/setup.py` & `gotji-1.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gotji",
-    version="1.0.4",
+    version="1.0.5",
     description="Dev by Meoaw",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/exaDev99/gotji",
     author="exaDev99",
     author_email="meoawdev.me@gmail.com",
     license="MIT",
@@ -18,10 +18,15 @@
         "Programming Language :: Python :: 3",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "requests",
-        "pystyle"
+        "pystyle",
+        "platform",
+        "os",
+        "replit",
+        "flask",
+        "flask_restful"
     ],
 )
```

