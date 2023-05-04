# Comparing `tmp/sklean123-0.1.0.tar.gz` & `tmp/sklean123-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklean123-0.1.0.tar", last modified: Thu May  4 16:34:30 2023, max compression
+gzip compressed data, was "sklean123-0.2.0.tar", last modified: Thu May  4 17:43:57 2023, max compression
```

## Comparing `sklean123-0.1.0.tar` & `sklean123-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:34:30.100207 sklean123-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-04 16:34:19.000000 sklean123-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 16:34:19.000000 sklean123-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-05-04 16:34:30.100207 sklean123-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-05-04 16:34:19.000000 sklean123-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 16:34:19.000000 sklean123-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 16:34:30.100207 sklean123-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-04 16:34:19.000000 sklean123-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:34:30.096207 sklean123-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:34:30.096207 sklean123-0.1.0/src/sklean123/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 16:34:19.000000 sklean123-0.1.0/src/sklean123/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16310 2023-05-04 16:34:19.000000 sklean123-0.1.0/src/sklean123/module1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:34:30.096207 sklean123-0.1.0/src/sklean123.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-05-04 16:34:30.000000 sklean123-0.1.0/src/sklean123.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-04 16:34:30.000000 sklean123-0.1.0/src/sklean123.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:34:30.000000 sklean123-0.1.0/src/sklean123.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 16:34:30.000000 sklean123-0.1.0/src/sklean123.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 16:34:30.000000 sklean123-0.1.0/src/sklean123.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:34:30.096207 sklean123-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 16:34:19.000000 sklean123-0.1.0/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:57.138497 sklean123-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-04 17:43:42.000000 sklean123-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 17:43:42.000000 sklean123-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-05-04 17:43:57.138497 sklean123-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-05-04 17:43:42.000000 sklean123-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 17:43:42.000000 sklean123-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 17:43:57.142497 sklean123-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-04 17:43:42.000000 sklean123-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:57.138497 sklean123-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:57.138497 sklean123-0.2.0/src/sklean123/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 17:43:42.000000 sklean123-0.2.0/src/sklean123/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52527 2023-05-04 17:43:42.000000 sklean123-0.2.0/src/sklean123/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:57.138497 sklean123-0.2.0/src/sklean123.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-05-04 17:43:57.000000 sklean123-0.2.0/src/sklean123.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-04 17:43:57.000000 sklean123-0.2.0/src/sklean123.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:43:57.000000 sklean123-0.2.0/src/sklean123.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 17:43:57.000000 sklean123-0.2.0/src/sklean123.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 17:43:57.000000 sklean123-0.2.0/src/sklean123.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:43:57.138497 sklean123-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 17:43:42.000000 sklean123-0.2.0/tests/test_module1.py
```

### Comparing `sklean123-0.1.0/LICENSE` & `sklean123-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sklean123-0.1.0/PKG-INFO` & `sklean123-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklean123
-Version: 0.1.0
+Version: 0.2.0
 Summary: Example PyPI (Python Package Index) Package
 Home-page: https://github.com/bloobdev/sklean123
 Author: Tom Chen
 Author-email: tomchen.org@gmail.com
 Project-URL: Documentation, https://github.com/bloobdev/sklean123
 Project-URL: Bug Reports, https://github.com/bloobdev/sklean123/issues
 Project-URL: Source Code, https://github.com/bloobdev/sklean123
```

### Comparing `sklean123-0.1.0/README.md` & `sklean123-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sklean123-0.1.0/setup.py` & `sklean123-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `sklean123-0.1.0/src/sklean123.egg-info/PKG-INFO` & `sklean123-0.2.0/src/sklean123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklean123
-Version: 0.1.0
+Version: 0.2.0
 Summary: Example PyPI (Python Package Index) Package
 Home-page: https://github.com/bloobdev/sklean123
 Author: Tom Chen
 Author-email: tomchen.org@gmail.com
 Project-URL: Documentation, https://github.com/bloobdev/sklean123
 Project-URL: Bug Reports, https://github.com/bloobdev/sklean123/issues
 Project-URL: Source Code, https://github.com/bloobdev/sklean123
```

