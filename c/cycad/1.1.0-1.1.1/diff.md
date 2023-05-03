# Comparing `tmp/cycad-1.1.0.tar.gz` & `tmp/cycad-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycad-1.1.0.tar", last modified: Wed May  3 16:39:28 2023, max compression
+gzip compressed data, was "cycad-1.1.1.tar", last modified: Wed May  3 22:13:09 2023, max compression
```

## Comparing `cycad-1.1.0.tar` & `cycad-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yuewu    (1662288217) 1704612529        0 2023-05-03 16:39:28.790320 cycad-1.1.0/
--rw-r--r--   0 yuewu    (1662288217) 1704612529     1062 2023-05-03 16:32:47.000000 cycad-1.1.0/LICENSE
--rw-r--r--   0 yuewu    (1662288217) 1704612529      399 2023-05-03 16:39:28.790132 cycad-1.1.0/PKG-INFO
-drwxr-xr-x   0 yuewu    (1662288217) 1704612529        0 2023-05-03 16:39:28.787726 cycad-1.1.0/cycad/
-drwxr-xr-x   0 yuewu    (1662288217) 1704612529        0 2023-05-03 16:39:28.788621 cycad-1.1.0/cycad/src/
-drwxr-xr-x   0 yuewu    (1662288217) 1704612529        0 2023-05-03 16:39:28.789895 cycad-1.1.0/cycad/src/cycad.egg-info/
--rw-r--r--   0 yuewu    (1662288217) 1704612529      399 2023-05-03 16:39:28.000000 cycad-1.1.0/cycad/src/cycad.egg-info/PKG-INFO
--rw-r--r--   0 yuewu    (1662288217) 1704612529      229 2023-05-03 16:39:28.000000 cycad-1.1.0/cycad/src/cycad.egg-info/SOURCES.txt
--rw-r--r--   0 yuewu    (1662288217) 1704612529        1 2023-05-03 16:39:28.000000 cycad-1.1.0/cycad/src/cycad.egg-info/dependency_links.txt
--rw-r--r--   0 yuewu    (1662288217) 1704612529       59 2023-05-03 16:39:28.000000 cycad-1.1.0/cycad/src/cycad.egg-info/requires.txt
--rw-r--r--   0 yuewu    (1662288217) 1704612529        6 2023-05-03 16:39:28.000000 cycad-1.1.0/cycad/src/cycad.egg-info/top_level.txt
--rw-r--r--   0 yuewu    (1662288217) 1704612529    21101 2023-05-03 16:36:04.000000 cycad-1.1.0/cycad/src/cycad.py
--rw-r--r--   0 yuewu    (1662288217) 1704612529       38 2023-05-03 16:39:28.790379 cycad-1.1.0/setup.cfg
--rw-r--r--   0 yuewu    (1662288217) 1704612529     1309 2023-05-03 16:36:20.000000 cycad-1.1.0/setup.py
+drwxr-xr-x   0 yuewu    (1662288217) 1704612529        0 2023-05-03 22:13:09.944634 cycad-1.1.1/
+-rw-r--r--   0 yuewu    (1662288217) 1704612529     1062 2023-05-03 16:32:47.000000 cycad-1.1.1/LICENSE
+-rw-r--r--   0 yuewu    (1662288217) 1704612529      399 2023-05-03 22:13:09.944429 cycad-1.1.1/PKG-INFO
+drwxr-xr-x   0 yuewu    (1662288217) 1704612529        0 2023-05-03 22:13:09.942148 cycad-1.1.1/cycad/
+drwxr-xr-x   0 yuewu    (1662288217) 1704612529        0 2023-05-03 22:13:09.943190 cycad-1.1.1/cycad/src/
+drwxr-xr-x   0 yuewu    (1662288217) 1704612529        0 2023-05-03 22:13:09.944160 cycad-1.1.1/cycad/src/cycad.egg-info/
+-rw-r--r--   0 yuewu    (1662288217) 1704612529      399 2023-05-03 22:13:09.000000 cycad-1.1.1/cycad/src/cycad.egg-info/PKG-INFO
+-rw-r--r--   0 yuewu    (1662288217) 1704612529      229 2023-05-03 22:13:09.000000 cycad-1.1.1/cycad/src/cycad.egg-info/SOURCES.txt
+-rw-r--r--   0 yuewu    (1662288217) 1704612529        1 2023-05-03 22:13:09.000000 cycad-1.1.1/cycad/src/cycad.egg-info/dependency_links.txt
+-rw-r--r--   0 yuewu    (1662288217) 1704612529       59 2023-05-03 22:13:09.000000 cycad-1.1.1/cycad/src/cycad.egg-info/requires.txt
+-rw-r--r--   0 yuewu    (1662288217) 1704612529        6 2023-05-03 22:13:09.000000 cycad-1.1.1/cycad/src/cycad.egg-info/top_level.txt
+-rw-r--r--   0 yuewu    (1662288217) 1704612529    20925 2023-05-03 22:12:36.000000 cycad-1.1.1/cycad/src/cycad.py
+-rw-r--r--   0 yuewu    (1662288217) 1704612529       38 2023-05-03 22:13:09.944691 cycad-1.1.1/setup.cfg
+-rw-r--r--   0 yuewu    (1662288217) 1704612529     1164 2023-05-03 22:12:33.000000 cycad-1.1.1/setup.py
```

### Comparing `cycad-1.1.0/LICENSE` & `cycad-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cycad-1.1.0/cycad/src/cycad.py` & `cycad-1.1.1/cycad/src/cycad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # CYCAD - CYCling Autocorrelation Dataviz
-# 1.1.0
+# 1.1.1
 import csv
 import glob
 import os
 import re
 import warnings
 
 import h5py
@@ -71,21 +71,15 @@
         :type root: str
         :param filetype: Filetype of the files.
         :type filetype: str
         """
         self.root = root
         self.runname = os.path.normpath(self.root).split(os.path.sep)[-1]
         self.filetype = filetype
-        if range:
-            self.files = self.natural_sort(glob.glob(self.root + "/*" + self.filetype))[
-                range[0] : range[1]
-            ]
-        else:
-            self.files = self.natural_sort(glob.glob(self.root + "/*" + self.filetype))
-
+        self.files = self.natural_sort(glob.glob(self.root + "/*" + self.filetype))
         self.read_data()
 
     def read_data(self, parse_names=False):
         """
         Read data from a list of files found by read_folder.
         Takes the first column of the first file as the x-values.
         Filetype is specified by :func:`self.read_folder()`.
```

### Comparing `cycad-1.1.0/setup.py` & `cycad-1.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="cycad",                     # This is the name of the package
-    version="1.1.0",                        # release version
-    author="Yue Wu",                     # Full name of the author
+    name="cycad",  # This is the name of the package
+    version="1.1.1",  # release version
+    author="Yue Wu",  # Full name of the author
     description="CYCling Autocorrelation Dataviz",
-    long_description=long_description,      # Long description read from the the readme file
+    long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),    # List of all python modules to be installed
+    packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-    ],                                      # Information to filter the project on PyPi website
-    python_requires='>=3.6',                # Minimum version requirement of the package
-    py_modules=["cycad"],             # Name of the python package
-    package_dir={'':'cycad/src'},     # Directory of the source code of the package
+    ],  # Information to filter the project on PyPi website
+    python_requires=">=3.6",  # Minimum version requirement of the package
+    py_modules=["cycad"],  # Name of the python package
+    package_dir={"": "cycad/src"},  # Directory of the source code of the package
     install_requires=[
-        'numpy',
-        'pandas',
-        'matplotlib',
-        'charset-normalizer',
-        'scipy',
-        'tqdm',
-        'h5py'
-    ]                     # Install other dependencies if any
-)
+        "numpy",
+        "pandas",
+        "matplotlib",
+        "charset-normalizer",
+        "scipy",
+        "tqdm",
+        "h5py",
+    ],  # Install other dependencies if any
+)
```

