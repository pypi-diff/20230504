# Comparing `tmp/gstatsim-1.0.2.tar.gz` & `tmp/gstatsim-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gstatsim-1.0.2.tar", last modified: Thu Apr 27 17:10:39 2023, max compression
+gzip compressed data, was "gstatsim-1.0.3.tar", last modified: Thu May  4 18:16:24 2023, max compression
```

## Comparing `gstatsim-1.0.2.tar` & `gstatsim-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-04-27 17:10:39.252550 gstatsim-1.0.2/
--rw-r--r--   0 michaelfield   (502) staff       (20)     1068 2023-04-27 17:08:18.000000 gstatsim-1.0.2/LICENSE
--rw-r--r--   0 michaelfield   (502) staff       (20)     5160 2023-04-27 17:10:39.252421 gstatsim-1.0.2/PKG-INFO
--rw-r--r--   0 michaelfield   (502) staff       (20)     4620 2023-04-27 17:10:19.000000 gstatsim-1.0.2/README.md
-drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-04-27 17:10:39.252265 gstatsim-1.0.2/gstatsim.egg-info/
--rw-r--r--   0 michaelfield   (502) staff       (20)     5160 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/PKG-INFO
--rw-r--r--   0 michaelfield   (502) staff       (20)      197 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/SOURCES.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)        1 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/dependency_links.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)       69 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/requires.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)        9 2023-04-27 17:10:39.000000 gstatsim-1.0.2/gstatsim.egg-info/top_level.txt
--rw-r--r--   0 michaelfield   (502) staff       (20)    56584 2023-04-27 16:20:42.000000 gstatsim-1.0.2/gstatsim.py
--rw-r--r--   0 michaelfield   (502) staff       (20)       38 2023-04-27 17:10:39.252585 gstatsim-1.0.2/setup.cfg
--rw-r--r--   0 michaelfield   (502) staff       (20)      938 2023-04-27 17:10:12.000000 gstatsim-1.0.2/setup.py
+drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-05-04 18:16:24.713975 gstatsim-1.0.3/
+-rw-r--r--   0 michaelfield   (502) staff       (20)     1068 2023-04-27 17:08:18.000000 gstatsim-1.0.3/LICENSE
+-rw-r--r--   0 michaelfield   (502) staff       (20)     5160 2023-05-04 18:16:24.713855 gstatsim-1.0.3/PKG-INFO
+-rw-r--r--   0 michaelfield   (502) staff       (20)     4620 2023-05-04 18:15:23.000000 gstatsim-1.0.3/README.md
+drwxr-xr-x   0 michaelfield   (502) staff       (20)        0 2023-05-04 18:16:24.713672 gstatsim-1.0.3/gstatsim.egg-info/
+-rw-r--r--   0 michaelfield   (502) staff       (20)     5160 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/PKG-INFO
+-rw-r--r--   0 michaelfield   (502) staff       (20)      197 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)        1 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)       69 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/requires.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)        9 2023-05-04 18:16:24.000000 gstatsim-1.0.3/gstatsim.egg-info/top_level.txt
+-rw-r--r--   0 michaelfield   (502) staff       (20)    56584 2023-04-27 16:20:42.000000 gstatsim-1.0.3/gstatsim.py
+-rw-r--r--   0 michaelfield   (502) staff       (20)       38 2023-05-04 18:16:24.714012 gstatsim-1.0.3/setup.cfg
+-rw-r--r--   0 michaelfield   (502) staff       (20)      938 2023-05-04 18:15:36.000000 gstatsim-1.0.3/setup.py
```

### Comparing `gstatsim-1.0.2/LICENSE` & `gstatsim-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gstatsim-1.0.2/PKG-INFO` & `gstatsim-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gstatsim
-Version: 1.0.2
+Version: 1.0.3
 Summary: Geostatistics tools for interpolation and simulation.
 Home-page: https://github.com/GatorGlaciology/GStatSim
 Author: (Emma) Mickey MacKie
 Author-email: emackie@ufl.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gstatsim-1.0.2/README.md` & `gstatsim-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gstatsim-1.0.2/gstatsim.egg-info/PKG-INFO` & `gstatsim-1.0.3/gstatsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gstatsim
-Version: 1.0.2
+Version: 1.0.3
 Summary: Geostatistics tools for interpolation and simulation.
 Home-page: https://github.com/GatorGlaciology/GStatSim
 Author: (Emma) Mickey MacKie
 Author-email: emackie@ufl.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gstatsim-1.0.2/gstatsim.py` & `gstatsim-1.0.3/gstatsim.py`

 * *Files identical despite different names*

### Comparing `gstatsim-1.0.2/setup.py` & `gstatsim-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '1.0.2'
+version = '1.0.3'
 
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Topic :: Scientific/Engineering :: Information Analysis',
 ]
```

