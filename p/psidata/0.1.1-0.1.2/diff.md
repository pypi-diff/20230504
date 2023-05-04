# Comparing `tmp/psidata-0.1.1.tar.gz` & `tmp/psidata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psidata-0.1.1.tar", last modified: Thu Feb 23 14:52:15 2023, max compression
+gzip compressed data, was "psidata-0.1.2.tar", last modified: Thu May  4 14:53:55 2023, max compression
```

## Comparing `psidata-0.1.1.tar` & `psidata-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:52:15.357558 psidata-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:52:15.353558 psidata-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:52:15.353558 psidata-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-02-23 14:52:00.000000 psidata-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-23 14:52:00.000000 psidata-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-23 14:52:00.000000 psidata-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-02-23 14:52:15.357558 psidata-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-23 14:52:00.000000 psidata-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:52:15.357558 psidata-0.1.1/psidata/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-23 14:52:00.000000 psidata-0.1.1/psidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-23 14:52:00.000000 psidata-0.1.1/psidata/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-02-23 14:52:00.000000 psidata-0.1.1/psidata/bcolz_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-02-23 14:52:00.000000 psidata-0.1.1/psidata/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-02-23 14:52:00.000000 psidata-0.1.1/psidata/legacy_bcolz_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-02-23 14:52:00.000000 psidata-0.1.1/psidata/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-02-23 14:52:00.000000 psidata-0.1.1/psidata/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-23 14:52:15.000000 psidata-0.1.1/psidata/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-23 14:52:00.000000 psidata-0.1.1/psidata/zarr_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:52:15.357558 psidata-0.1.1/psidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-02-23 14:52:15.000000 psidata-0.1.1/psidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-23 14:52:15.000000 psidata-0.1.1/psidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 14:52:15.000000 psidata-0.1.1/psidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-23 14:52:15.000000 psidata-0.1.1/psidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-23 14:52:15.000000 psidata-0.1.1/psidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-23 14:52:00.000000 psidata-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 14:52:15.357558 psidata-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.402316 psidata-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.398316 psidata-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.398316 psidata-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 14:53:44.000000 psidata-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-04 14:53:44.000000 psidata-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-04 14:53:44.000000 psidata-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-04 14:53:55.402316 psidata-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-04 14:53:44.000000 psidata-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.402316 psidata-0.1.2/psidata/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/bcolz_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/legacy_bcolz_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-04 14:53:44.000000 psidata-0.1.2/psidata/zarr_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:55.402316 psidata-0.1.2/psidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 14:53:55.000000 psidata-0.1.2/psidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-04 14:53:44.000000 psidata-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:53:55.402316 psidata-0.1.2/setup.cfg
```

### Comparing `psidata-0.1.1/.github/workflows/publish-to-pypi.yml` & `psidata-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `psidata-0.1.1/.gitignore` & `psidata-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `psidata-0.1.1/LICENSE.txt` & `psidata-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psidata-0.1.1/PKG-INFO` & `psidata-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psidata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lightweight wrapper for managing psiexperiment data
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2017-2022 psiepxeriment development team
```

### Comparing `psidata-0.1.1/psidata/bcolz_tools.py` & `psidata-0.1.2/psidata/bcolz_tools.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.1/psidata/calibration.py` & `psidata-0.1.2/psidata/calibration.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.1/psidata/legacy_bcolz_tools.py` & `psidata-0.1.2/psidata/legacy_bcolz_tools.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.1/psidata/recording.py` & `psidata-0.1.2/psidata/recording.py`

 * *Files identical despite different names*

### Comparing `psidata-0.1.1/psidata/zarr_tools.py` & `psidata-0.1.2/psidata/zarr_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     @classmethod
     def from_path(cls, path):
         path = path.with_suffix('.zarr')
         array = zarr.open(store=str(path), mode='r')
         return cls(array)
 
     def __init__(self, array):
+        super().__init__()
         self.array = array
 
     @property
     def fs(self):
         return self.array.attrs['fs']
 
     @property
```

### Comparing `psidata-0.1.1/psidata.egg-info/PKG-INFO` & `psidata-0.1.2/psidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psidata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lightweight wrapper for managing psiexperiment data
 Author-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, Brad Buran <buran@ohsu.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2017-2022 psiepxeriment development team
```

### Comparing `psidata-0.1.1/pyproject.toml` & `psidata-0.1.2/pyproject.toml`

 * *Files identical despite different names*

