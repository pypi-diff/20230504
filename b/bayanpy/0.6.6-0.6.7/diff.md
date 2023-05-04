# Comparing `tmp/bayanpy-0.6.6.tar.gz` & `tmp/bayanpy-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.6.6.tar", last modified: Thu May  4 01:03:22 2023, max compression
+gzip compressed data, was "bayanpy-0.6.7.tar", last modified: Thu May  4 01:05:12 2023, max compression
```

## Comparing `bayanpy-0.6.6.tar` & `bayanpy-0.6.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-04 01:03:22.145680 bayanpy-0.6.6/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.6/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-04 01:03:22.145680 bayanpy-0.6.6/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.6/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-04 01:03:22.145680 bayanpy-0.6.6/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57350 2023-05-04 00:58:33.000000 bayanpy-0.6.6/bayanpy/BayanImplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.6/bayanpy/__init__.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-04 01:03:22.145680 bayanpy-0.6.6/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-04 01:03:22.000000 bayanpy-0.6.6/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-04 01:03:22.000000 bayanpy-0.6.6/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-04 01:03:22.000000 bayanpy-0.6.6/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       61 2023-05-04 01:03:22.000000 bayanpy-0.6.6/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-04 01:03:22.000000 bayanpy-0.6.6/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-04 01:03:22.145680 bayanpy-0.6.6/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      583 2023-05-04 01:03:18.000000 bayanpy-0.6.6/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-04 01:05:12.529183 bayanpy-0.6.7/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6.7/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-04 01:05:12.529183 bayanpy-0.6.7/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5056 2023-04-11 16:11:47.000000 bayanpy-0.6.7/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-04 01:05:12.529183 bayanpy-0.6.7/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    57350 2023-05-04 00:58:33.000000 bayanpy-0.6.7/bayanpy/BayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-13 14:38:52.000000 bayanpy-0.6.7/bayanpy/__init__.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-05-04 01:05:12.529183 bayanpy-0.6.7/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      359 2023-05-04 01:05:12.000000 bayanpy-0.6.7/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      224 2023-05-04 01:05:12.000000 bayanpy-0.6.7/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-05-04 01:05:12.000000 bayanpy-0.6.7/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       55 2023-05-04 01:05:12.000000 bayanpy-0.6.7/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-05-04 01:05:12.000000 bayanpy-0.6.7/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-05-04 01:05:12.529183 bayanpy-0.6.7/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      563 2023-05-04 01:05:08.000000 bayanpy-0.6.7/setup.py
```

### Comparing `bayanpy-0.6.6/LICENSE` & `bayanpy-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.6/README.md` & `bayanpy-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.6/bayanpy/BayanImplied.py` & `bayanpy-0.6.7/bayanpy/BayanImplied.py`

 * *Files identical despite different names*

### Comparing `bayanpy-0.6.6/setup.py` & `bayanpy-0.6.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.6.6",
+    version="0.6.7",
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
-        "cdlib",
-	    "joblib",
+	 "joblib",
         "pycombo"
     ],
 )
```

