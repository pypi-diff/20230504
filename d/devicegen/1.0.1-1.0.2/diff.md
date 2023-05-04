# Comparing `tmp/devicegen-1.0.1.tar.gz` & `tmp/devicegen-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicegen-1.0.1.tar", last modified: Thu May  4 15:12:44 2023, max compression
+gzip compressed data, was "devicegen-1.0.2.tar", last modified: Thu May  4 15:23:07 2023, max compression
```

## Comparing `devicegen-1.0.1.tar` & `devicegen-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 matador   (1000) matador   (1000)        0 2023-05-04 15:12:44.844195 devicegen-1.0.1/
--rw-rw-r--   0 matador   (1000) matador   (1000)    35149 2023-05-01 15:05:39.000000 devicegen-1.0.1/LICENSE.txt
--rw-rw-r--   0 matador   (1000) matador   (1000)      514 2023-05-04 15:12:44.844195 devicegen-1.0.1/PKG-INFO
--rw-rw-r--   0 matador   (1000) matador   (1000)     1899 2023-05-01 15:05:39.000000 devicegen-1.0.1/README.md
-drwxrwxr-x   0 matador   (1000) matador   (1000)        0 2023-05-04 15:12:44.840195 devicegen-1.0.1/devicegen/
--rw-rw-r--   0 matador   (1000) matador   (1000)       48 2023-05-04 13:25:12.000000 devicegen-1.0.1/devicegen/__init__.py
--rw-rw-r--   0 matador   (1000) matador   (1000)    42406 2023-05-04 13:25:12.000000 devicegen-1.0.1/devicegen/device_gen.py
--rw-rw-r--   0 matador   (1000) matador   (1000)     6992 2023-05-04 13:25:12.000000 devicegen-1.0.1/devicegen/gds_parser.py
-drwxrwxr-x   0 matador   (1000) matador   (1000)        0 2023-05-04 15:12:44.840195 devicegen-1.0.1/devicegen.egg-info/
--rw-rw-r--   0 matador   (1000) matador   (1000)      514 2023-05-04 15:12:44.000000 devicegen-1.0.1/devicegen.egg-info/PKG-INFO
--rw-rw-r--   0 matador   (1000) matador   (1000)      232 2023-05-04 15:12:44.000000 devicegen-1.0.1/devicegen.egg-info/SOURCES.txt
--rw-rw-r--   0 matador   (1000) matador   (1000)        1 2023-05-04 15:12:44.000000 devicegen-1.0.1/devicegen.egg-info/dependency_links.txt
--rw-rw-r--   0 matador   (1000) matador   (1000)       10 2023-05-04 15:12:44.000000 devicegen-1.0.1/devicegen.egg-info/top_level.txt
--rw-rw-r--   0 matador   (1000) matador   (1000)       38 2023-05-04 15:12:44.844195 devicegen-1.0.1/setup.cfg
--rw-rw-r--   0 matador   (1000) matador   (1000)      611 2023-05-04 15:11:18.000000 devicegen-1.0.1/setup.py
+drwxrwxr-x   0 matador   (1000) matador   (1000)        0 2023-05-04 15:23:07.678168 devicegen-1.0.2/
+-rw-rw-r--   0 matador   (1000) matador   (1000)    35149 2023-05-01 15:05:39.000000 devicegen-1.0.2/LICENSE.txt
+-rw-rw-r--   0 matador   (1000) matador   (1000)      685 2023-05-04 15:23:07.678168 devicegen-1.0.2/PKG-INFO
+-rw-rw-r--   0 matador   (1000) matador   (1000)     1899 2023-05-01 15:05:39.000000 devicegen-1.0.2/README.md
+drwxrwxr-x   0 matador   (1000) matador   (1000)        0 2023-05-04 15:23:07.678168 devicegen-1.0.2/devicegen/
+-rw-rw-r--   0 matador   (1000) matador   (1000)       48 2023-05-04 13:25:12.000000 devicegen-1.0.2/devicegen/__init__.py
+-rw-rw-r--   0 matador   (1000) matador   (1000)    42406 2023-05-04 13:25:12.000000 devicegen-1.0.2/devicegen/device_gen.py
+-rw-rw-r--   0 matador   (1000) matador   (1000)     6992 2023-05-04 13:25:12.000000 devicegen-1.0.2/devicegen/gds_parser.py
+drwxrwxr-x   0 matador   (1000) matador   (1000)        0 2023-05-04 15:23:07.678168 devicegen-1.0.2/devicegen.egg-info/
+-rw-rw-r--   0 matador   (1000) matador   (1000)      685 2023-05-04 15:23:07.000000 devicegen-1.0.2/devicegen.egg-info/PKG-INFO
+-rw-rw-r--   0 matador   (1000) matador   (1000)      232 2023-05-04 15:23:07.000000 devicegen-1.0.2/devicegen.egg-info/SOURCES.txt
+-rw-rw-r--   0 matador   (1000) matador   (1000)        1 2023-05-04 15:23:07.000000 devicegen-1.0.2/devicegen.egg-info/dependency_links.txt
+-rw-rw-r--   0 matador   (1000) matador   (1000)       10 2023-05-04 15:23:07.000000 devicegen-1.0.2/devicegen.egg-info/top_level.txt
+-rw-rw-r--   0 matador   (1000) matador   (1000)       38 2023-05-04 15:23:07.678168 devicegen-1.0.2/setup.cfg
+-rw-rw-r--   0 matador   (1000) matador   (1000)      805 2023-05-04 15:22:38.000000 devicegen-1.0.2/setup.py
```

### Comparing `devicegen-1.0.1/LICENSE.txt` & `devicegen-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devicegen-1.0.1/README.md` & `devicegen-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `devicegen-1.0.1/devicegen/device_gen.py` & `devicegen-1.0.2/devicegen/device_gen.py`

 * *Files identical despite different names*

### Comparing `devicegen-1.0.1/devicegen/gds_parser.py` & `devicegen-1.0.2/devicegen/gds_parser.py`

 * *Files identical despite different names*

