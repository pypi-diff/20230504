# Comparing `tmp/n64img-0.3.0.tar.gz` & `tmp/n64img-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n64img-0.3.0.tar", last modified: Wed May  3 15:13:17 2023, max compression
+gzip compressed data, was "n64img-0.3.1.tar", last modified: Thu May  4 15:48:19 2023, max compression
```

## Comparing `n64img-0.3.0.tar` & `n64img-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:17.391980 n64img-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-03 15:13:10.000000 n64img-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 15:13:17.391980 n64img-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-03 15:13:10.000000 n64img-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:17.391980 n64img-0.3.0/n64img/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:10.000000 n64img-0.3.0/n64img/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-03 15:13:10.000000 n64img-0.3.0/n64img/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 15:13:10.000000 n64img-0.3.0/n64img/iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:17.391980 n64img-0.3.0/n64img.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 15:13:10.000000 n64img-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-03 15:13:17.391980 n64img-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:17.391980 n64img-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:10.000000 n64img-0.3.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-03 15:13:10.000000 n64img-0.3.0/test/test_endian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-03 15:13:10.000000 n64img-0.3.0/test/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:19.910780 n64img-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 15:48:08.000000 n64img-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-04 15:48:19.910780 n64img-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 15:48:08.000000 n64img-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:19.906780 n64img-0.3.1/n64img/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:08.000000 n64img-0.3.1/n64img/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-04 15:48:08.000000 n64img-0.3.1/n64img/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-04 15:48:08.000000 n64img-0.3.1/n64img/iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:19.910780 n64img-0.3.1/n64img.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 15:48:19.000000 n64img-0.3.1/n64img.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 15:48:08.000000 n64img-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-04 15:48:19.910780 n64img-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:19.910780 n64img-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:08.000000 n64img-0.3.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-04 15:48:08.000000 n64img-0.3.1/test/test_endian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-04 15:48:08.000000 n64img-0.3.1/test/test_image.py
```

### Comparing `n64img-0.3.0/LICENSE` & `n64img-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `n64img-0.3.0/n64img/image.py` & `n64img-0.3.1/n64img/image.py`

 * *Files identical despite different names*

### Comparing `n64img-0.3.0/n64img/iter.py` & `n64img-0.3.1/n64img/iter.py`

 * *Files identical despite different names*

### Comparing `n64img-0.3.0/test/test_endian.py` & `n64img-0.3.1/test/test_endian.py`

 * *Files identical despite different names*

### Comparing `n64img-0.3.0/test/test_image.py` & `n64img-0.3.1/test/test_image.py`

 * *Files identical despite different names*

