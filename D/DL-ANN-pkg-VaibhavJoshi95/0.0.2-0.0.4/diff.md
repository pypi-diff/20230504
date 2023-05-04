# Comparing `tmp/DL-ANN_pkg-VaibhavJoshi95-0.0.2.tar.gz` & `tmp/DL-ANN-pkg-VaibhavJoshi95-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DL-ANN_pkg-VaibhavJoshi95-0.0.2.tar", last modified: Thu May  4 11:59:20 2023, max compression
+gzip compressed data, was "DL-ANN-pkg-VaibhavJoshi95-0.0.4.tar", last modified: Thu May  4 12:30:43 2023, max compression
```

## Comparing `DL-ANN_pkg-VaibhavJoshi95-0.0.2.tar` & `DL-ANN-pkg-VaibhavJoshi95-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:59:20.869832 DL-ANN_pkg-VaibhavJoshi95-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 11:59:09.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-04 11:59:20.869832 DL-ANN_pkg-VaibhavJoshi95-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-04 11:59:09.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 11:59:09.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:59:20.869832 DL-ANN_pkg-VaibhavJoshi95-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-04 11:59:09.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:59:20.869832 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:59:20.869832 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:59:09.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-04 11:59:09.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN/perceptron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:59:20.869832 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-04 11:59:20.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-04 11:59:20.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:59:20.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 11:59:20.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 11:59:20.000000 DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:30:43.523314 DL-ANN-pkg-VaibhavJoshi95-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 12:30:30.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-04 12:30:43.523314 DL-ANN-pkg-VaibhavJoshi95-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-04 12:30:30.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 12:30:30.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:30:43.523314 DL-ANN-pkg-VaibhavJoshi95-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-04 12:30:30.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:30:43.519314 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:30:43.523314 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:30:30.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-04 12:30:30.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN/perceptron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:30:43.523314 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-04 12:30:43.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-04 12:30:43.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:30:43.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 12:30:43.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 12:30:43.000000 DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/top_level.txt
```

### Comparing `DL-ANN_pkg-VaibhavJoshi95-0.0.2/LICENSE` & `DL-ANN-pkg-VaibhavJoshi95-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DL-ANN_pkg-VaibhavJoshi95-0.0.2/PKG-INFO` & `DL-ANN-pkg-VaibhavJoshi95-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: DL-ANN_pkg-VaibhavJoshi95
-Version: 0.0.2
+Name: DL-ANN-pkg-VaibhavJoshi95
+Version: 0.0.4
 Summary: A small package for perceptron
-Home-page: https://github.com/VaibhavJoshi95/DLANN-pkg
+Home-page: https://github.com/VaibhavJoshi95/DL-ANN-pkg
 Author: VaibhavJoshi95
 Author-email: vaibhavgjoshi95@gmail.com
-Project-URL: Bug Tracker, https://github.com/VaibhavJoshi95/DLANN-pkg/issues
+Project-URL: Bug Tracker, https://github.com/VaibhavJoshi95/DL-ANN-pkg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `DL-ANN_pkg-VaibhavJoshi95-0.0.2/setup.py` & `DL-ANN-pkg-VaibhavJoshi95-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-PKG_NAME = "DL-ANN_pkg"
+PKG_NAME = "DL-ANN-pkg"
 USER_NAME = "VaibhavJoshi95"
-PROJECT_NAME = "DLANN-pkg"
+PROJECT_NAME = "DL-ANN-pkg"
 
 setuptools.setup(
     name=f"{PKG_NAME}-{USER_NAME}",
-    version="0.0.2",
+    version="0.0.4",
     author=USER_NAME,
     author_email="vaibhavgjoshi95@gmail.com",
     description="A small package for perceptron",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/{USER_NAME}/{PROJECT_NAME}",
     project_urls={
```

### Comparing `DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN/perceptron.py` & `DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN/perceptron.py`

 * *Files identical despite different names*

### Comparing `DL-ANN_pkg-VaibhavJoshi95-0.0.2/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/PKG-INFO` & `DL-ANN-pkg-VaibhavJoshi95-0.0.4/src/DL_ANN_pkg_VaibhavJoshi95.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: DL-ANN-pkg-VaibhavJoshi95
-Version: 0.0.2
+Version: 0.0.4
 Summary: A small package for perceptron
-Home-page: https://github.com/VaibhavJoshi95/DLANN-pkg
+Home-page: https://github.com/VaibhavJoshi95/DL-ANN-pkg
 Author: VaibhavJoshi95
 Author-email: vaibhavgjoshi95@gmail.com
-Project-URL: Bug Tracker, https://github.com/VaibhavJoshi95/DLANN-pkg/issues
+Project-URL: Bug Tracker, https://github.com/VaibhavJoshi95/DL-ANN-pkg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

