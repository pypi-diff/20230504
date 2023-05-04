# Comparing `tmp/hsmm_mvpy-0.1.0a0.tar.gz` & `tmp/hsmm_mvpy-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0a0.tar", last modified: Thu May  4 09:29:16 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0a1.tar", last modified: Thu May  4 10:13:30 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0a0.tar` & `hsmm_mvpy-0.1.0a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0a0/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22533 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20167 2023-05-04 09:20:47.000000 hsmm_mvpy-0.1.0a0/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      825 2023-05-04 09:24:53.000000 hsmm_mvpy-0.1.0a0/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      171 2022-09-28 08:31:43.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57128 2023-05-04 06:34:27.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     8910 2023-05-02 16:12:55.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    36660 2023-05-04 07:49:35.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20999 2023-05-03 22:23:27.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 09:29:16.790388 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22533 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      343 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       66 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-05-04 09:29:16.000000 hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 10:13:30.535035 hsmm_mvpy-0.1.0a1/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0a1/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22533 2023-05-04 10:13:30.535035 hsmm_mvpy-0.1.0a1/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20167 2023-05-04 09:20:47.000000 hsmm_mvpy-0.1.0a1/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      831 2023-05-04 10:13:21.000000 hsmm_mvpy-0.1.0a1/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-05-04 10:13:30.535035 hsmm_mvpy-0.1.0a1/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 10:13:30.535035 hsmm_mvpy-0.1.0a1/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 10:13:30.535035 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      171 2022-09-28 08:31:43.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57128 2023-05-04 06:34:27.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     8910 2023-05-02 16:12:55.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    36660 2023-05-04 07:49:35.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    20999 2023-05-03 22:23:27.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-05-04 10:13:30.535035 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22533 2023-05-04 10:13:30.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      343 2023-05-04 10:13:30.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-05-04 10:13:30.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-05-04 10:13:30.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-05-04 10:13:30.000000 hsmm_mvpy-0.1.0a1/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0a0/LICENSE.md` & `hsmm_mvpy-0.1.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0a0/PKG-INFO` & `hsmm_mvpy-0.1.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

### Comparing `hsmm_mvpy-0.1.0a0/README.md` & `hsmm_mvpy-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0a0/pyproject.toml` & `hsmm_mvpy-0.1.0a1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-alpha"
+version = "0.1.0-alpha1"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
@@ -18,15 +18,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies=["mne >=1.0.0",
 "numpy",
 "xarray",
-"sklearn",
+"scikit-learn",
 "seaborn",
 "scipy",
 "netcdf4",
 "xskillscore"]
 
 [project.urls]
 "Homepage" = "https://github.com/GWeindel/hmp"
```

### Comparing `hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/models.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/simulations.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/utils.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0a0/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0a1/src/hsmm_mvpy/visu.py`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0a0/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0a1/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
```

