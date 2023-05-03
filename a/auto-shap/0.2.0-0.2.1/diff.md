# Comparing `tmp/auto_shap-0.2.0.tar.gz` & `tmp/auto_shap-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto_shap-0.2.0.tar", last modified: Wed May  3 23:47:03 2023, max compression
+gzip compressed data, was "dist/auto_shap-0.2.1.tar", last modified: Wed May  3 23:55:41 2023, max compression
```

## Comparing `auto_shap-0.2.0.tar` & `auto_shap-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2023-05-03 23:47:03.000000 auto_shap-0.2.0/
--rw-r--r--   0 micahmelling   (501) staff       (20)    13528 2023-05-03 23:47:03.000000 auto_shap-0.2.0/PKG-INFO
--rw-r--r--   0 micahmelling   (501) staff       (20)    11091 2023-05-03 23:44:57.000000 auto_shap-0.2.0/README.md
-drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap/
--rw-r--r--   0 micahmelling   (501) staff       (20)       48 2023-05-03 04:47:03.000000 auto_shap-0.2.0/auto_shap/__init__.py
--rw-r--r--   0 micahmelling   (501) staff       (20)    20598 2023-05-03 04:18:28.000000 auto_shap-0.2.0/auto_shap/auto_shap.py
--rw-r--r--   0 micahmelling   (501) staff       (20)      334 2022-09-03 19:43:26.000000 auto_shap-0.2.0/auto_shap/config.py
--rw-r--r--   0 micahmelling   (501) staff       (20)     1551 2022-09-03 20:18:38.000000 auto_shap-0.2.0/auto_shap/scratch.py
--rw-r--r--   0 micahmelling   (501) staff       (20)     8987 2023-04-27 03:57:35.000000 auto_shap-0.2.0/auto_shap/utilities.py
-drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/
--rw-r--r--   0 micahmelling   (501) staff       (20)    13528 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/PKG-INFO
--rw-r--r--   0 micahmelling   (501) staff       (20)      301 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/SOURCES.txt
--rw-r--r--   0 micahmelling   (501) staff       (20)        1 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/dependency_links.txt
--rw-r--r--   0 micahmelling   (501) staff       (20)       59 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/requires.txt
--rw-r--r--   0 micahmelling   (501) staff       (20)       10 2023-05-03 23:47:03.000000 auto_shap-0.2.0/auto_shap.egg-info/top_level.txt
--rw-r--r--   0 micahmelling   (501) staff       (20)       79 2023-05-03 23:47:03.000000 auto_shap-0.2.0/setup.cfg
--rw-r--r--   0 micahmelling   (501) staff       (20)      801 2023-05-03 04:47:03.000000 auto_shap-0.2.0/setup.py
+drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2023-05-03 23:55:41.000000 auto_shap-0.2.1/
+-rw-r--r--   0 micahmelling   (501) staff       (20)    13528 2023-05-03 23:55:41.000000 auto_shap-0.2.1/PKG-INFO
+-rw-r--r--   0 micahmelling   (501) staff       (20)    11091 2023-05-03 23:44:57.000000 auto_shap-0.2.1/README.md
+drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2023-05-03 23:55:41.000000 auto_shap-0.2.1/auto_shap/
+-rw-r--r--   0 micahmelling   (501) staff       (20)       48 2023-05-03 23:55:27.000000 auto_shap-0.2.1/auto_shap/__init__.py
+-rw-r--r--   0 micahmelling   (501) staff       (20)    20598 2023-05-03 04:18:28.000000 auto_shap-0.2.1/auto_shap/auto_shap.py
+-rw-r--r--   0 micahmelling   (501) staff       (20)      334 2022-09-03 19:43:26.000000 auto_shap-0.2.1/auto_shap/config.py
+-rw-r--r--   0 micahmelling   (501) staff       (20)     1551 2022-09-03 20:18:38.000000 auto_shap-0.2.1/auto_shap/scratch.py
+-rw-r--r--   0 micahmelling   (501) staff       (20)     8987 2023-04-27 03:57:35.000000 auto_shap-0.2.1/auto_shap/utilities.py
+drwxr-xr-x   0 micahmelling   (501) staff       (20)        0 2023-05-03 23:55:41.000000 auto_shap-0.2.1/auto_shap.egg-info/
+-rw-r--r--   0 micahmelling   (501) staff       (20)    13528 2023-05-03 23:55:41.000000 auto_shap-0.2.1/auto_shap.egg-info/PKG-INFO
+-rw-r--r--   0 micahmelling   (501) staff       (20)      301 2023-05-03 23:55:41.000000 auto_shap-0.2.1/auto_shap.egg-info/SOURCES.txt
+-rw-r--r--   0 micahmelling   (501) staff       (20)        1 2023-05-03 23:55:41.000000 auto_shap-0.2.1/auto_shap.egg-info/dependency_links.txt
+-rw-r--r--   0 micahmelling   (501) staff       (20)       73 2023-05-03 23:55:41.000000 auto_shap-0.2.1/auto_shap.egg-info/requires.txt
+-rw-r--r--   0 micahmelling   (501) staff       (20)       10 2023-05-03 23:55:41.000000 auto_shap-0.2.1/auto_shap.egg-info/top_level.txt
+-rw-r--r--   0 micahmelling   (501) staff       (20)       79 2023-05-03 23:55:41.000000 auto_shap-0.2.1/setup.cfg
+-rw-r--r--   0 micahmelling   (501) staff       (20)      818 2023-05-03 23:55:27.000000 auto_shap-0.2.1/setup.py
```

### Comparing `auto_shap-0.2.0/PKG-INFO` & `auto_shap-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_shap
-Version: 0.2.0
+Version: 0.2.1
 Summary: Calculate SHAP values in parallel and automatically detect what explainer to use
 Home-page: https://github.com/micahmelling/auto-shap
 Author: Micah Melling
 Author-email: micahmelling@gmail.com
 License: MIT
 Description: # auto-shap
         The auto-shap library is your best friend when calculating SHAP values!
```

### Comparing `auto_shap-0.2.0/README.md` & `auto_shap-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `auto_shap-0.2.0/auto_shap/auto_shap.py` & `auto_shap-0.2.1/auto_shap/auto_shap.py`

 * *Files identical despite different names*

### Comparing `auto_shap-0.2.0/auto_shap/scratch.py` & `auto_shap-0.2.1/auto_shap/scratch.py`

 * *Files identical despite different names*

### Comparing `auto_shap-0.2.0/auto_shap/utilities.py` & `auto_shap-0.2.1/auto_shap/utilities.py`

 * *Files identical despite different names*

### Comparing `auto_shap-0.2.0/auto_shap.egg-info/PKG-INFO` & `auto_shap-0.2.1/auto_shap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-shap
-Version: 0.2.0
+Version: 0.2.1
 Summary: Calculate SHAP values in parallel and automatically detect what explainer to use
 Home-page: https://github.com/micahmelling/auto-shap
 Author: Micah Melling
 Author-email: micahmelling@gmail.com
 License: MIT
 Description: # auto-shap
         The auto-shap library is your best friend when calculating SHAP values!
```

### Comparing `auto_shap-0.2.0/setup.py` & `auto_shap-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="auto_shap",
-    version="0.2.0",
+    version="0.2.1",
     author="Micah Melling",
     author_email="micahmelling@gmail.com",
     description="Calculate SHAP values in parallel and automatically detect what explainer to use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/micahmelling/auto-shap',
     license="MIT",
     packages=['auto_shap'],
-    install_requires=['shap>=0.35.0', 'pandas>=1.1.5', 'numpy>=1.19.4', 'matplotlib>=3.2.0'],
+    install_requires=['shap>=0.35.0', 'pandas>=1.1.5', 'numpy>=1.21.6', 'matplotlib>=3.2.0', "numba>=0.56.4"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

