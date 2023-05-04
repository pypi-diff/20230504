# Comparing `tmp/polysplit-0.1.1.tar.gz` & `tmp/polysplit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polysplit-0.1.1.tar", last modified: Sun Apr 23 23:15:27 2023, max compression
+gzip compressed data, was "polysplit-0.1.2.tar", last modified: Thu May  4 19:43:03 2023, max compression
```

## Comparing `polysplit-0.1.1.tar` & `polysplit-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 23:15:27.742909 polysplit-0.1.1/
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 23:15:27.738621 polysplit-0.1.1/.github/
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 23:15:27.739444 polysplit-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      834 2023-02-20 05:22:23.000000 polysplit-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      595 2023-02-20 05:22:23.000000 polysplit-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      118 2023-04-23 22:51:26.000000 polysplit-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 23:15:27.739957 polysplit-0.1.1/.github/workflows/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1154 2023-04-23 22:51:26.000000 polysplit-0.1.1/.github/workflows/build.yml
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       55 2023-04-23 22:51:26.000000 polysplit-0.1.1/.gitignore
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1986 2023-04-23 22:51:26.000000 polysplit-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1073 2023-02-20 05:22:23.000000 polysplit-0.1.1/LICENSE
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       44 2023-04-23 22:51:26.000000 polysplit-0.1.1/MANIFEST.in
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2225 2023-04-23 22:51:26.000000 polysplit-0.1.1/Makefile
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     4214 2023-04-23 23:15:27.742660 polysplit-0.1.1/PKG-INFO
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2107 2023-04-23 22:51:26.000000 polysplit-0.1.1/README.md
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 23:15:27.740487 polysplit-0.1.1/polysplit/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      362 2023-04-23 22:51:26.000000 polysplit-0.1.1/polysplit/__init__.py
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     8601 2023-04-23 22:51:26.000000 polysplit-0.1.1/polysplit/polysplit.py
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 23:15:27.742262 polysplit-0.1.1/polysplit/tests/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 22:51:26.000000 polysplit-0.1.1/polysplit/tests/__init__.py
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2497 2023-04-23 22:51:26.000000 polysplit-0.1.1/polysplit/tests/test_polysplit.py
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 23:15:27.741795 polysplit-0.1.1/polysplit.egg-info/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     4214 2023-04-23 23:15:27.000000 polysplit-0.1.1/polysplit.egg-info/PKG-INFO
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      507 2023-04-23 23:15:27.000000 polysplit-0.1.1/polysplit.egg-info/SOURCES.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)        1 2023-04-23 23:15:27.000000 polysplit-0.1.1/polysplit.egg-info/dependency_links.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      236 2023-04-23 23:15:27.000000 polysplit-0.1.1/polysplit.egg-info/requires.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       10 2023-04-23 23:15:27.000000 polysplit-0.1.1/polysplit.egg-info/top_level.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2402 2023-04-23 22:59:23.000000 polysplit-0.1.1/pyproject.toml
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      224 2023-04-23 22:51:26.000000 polysplit-0.1.1/requirements.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       38 2023-04-23 23:15:27.742983 polysplit-0.1.1/setup.cfg
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       39 2023-04-23 22:51:26.000000 polysplit-0.1.1/setup.py
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.408188 polysplit-0.1.2/
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.402845 polysplit-0.1.2/.github/
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.403772 polysplit-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      834 2023-02-20 05:22:23.000000 polysplit-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      595 2023-02-20 05:22:23.000000 polysplit-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      118 2023-04-23 22:51:26.000000 polysplit-0.1.2/.github/dependabot.yml
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.404189 polysplit-0.1.2/.github/workflows/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1154 2023-04-23 22:51:26.000000 polysplit-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       55 2023-04-23 22:51:26.000000 polysplit-0.1.2/.gitignore
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1986 2023-04-23 22:51:26.000000 polysplit-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1073 2023-02-20 05:22:23.000000 polysplit-0.1.2/LICENSE
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       44 2023-04-23 22:51:26.000000 polysplit-0.1.2/MANIFEST.in
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2225 2023-04-23 22:51:26.000000 polysplit-0.1.2/Makefile
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     4236 2023-05-04 19:43:03.407934 polysplit-0.1.2/PKG-INFO
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2107 2023-04-23 22:51:26.000000 polysplit-0.1.2/README.md
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.405043 polysplit-0.1.2/polysplit/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      362 2023-04-23 22:51:26.000000 polysplit-0.1.2/polysplit/__init__.py
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     8601 2023-04-23 22:51:26.000000 polysplit-0.1.2/polysplit/polysplit.py
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.407286 polysplit-0.1.2/polysplit/tests/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 22:51:26.000000 polysplit-0.1.2/polysplit/tests/__init__.py
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2497 2023-04-23 22:51:26.000000 polysplit-0.1.2/polysplit/tests/test_polysplit.py
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.406586 polysplit-0.1.2/polysplit.egg-info/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     4236 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/PKG-INFO
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      507 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/SOURCES.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)        1 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/dependency_links.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      254 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/requires.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       10 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/top_level.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2699 2023-05-04 19:31:08.000000 polysplit-0.1.2/pyproject.toml
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      224 2023-04-23 22:51:26.000000 polysplit-0.1.2/requirements.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       38 2023-05-04 19:43:03.408277 polysplit-0.1.2/setup.cfg
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      347 2023-05-04 18:17:46.000000 polysplit-0.1.2/setup.py
```

### Comparing `polysplit-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `polysplit-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `polysplit-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.1/.github/workflows/build.yml` & `polysplit-0.1.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.1/CONTRIBUTING.md` & `polysplit-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.1/LICENSE` & `polysplit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.1/Makefile` & `polysplit-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.1/PKG-INFO` & `polysplit-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polysplit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library implementing a method for splitting a polygon into regions
 Author-email: Dmitrii Zakharov <d.zakharov@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Dmitrii Zakharov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,14 +33,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 Provides-Extra: develop
 License-File: LICENSE
 
 # polysplit
 
 A lightweight library for splitting polygons into regions based on proximity of points.\
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `polysplit-0.1.1/README.md` & `polysplit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.1/polysplit/polysplit.py` & `polysplit-0.1.2/polysplit/polysplit.py`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.1/polysplit/tests/test_polysplit.py` & `polysplit-0.1.2/polysplit/tests/test_polysplit.py`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.1/polysplit.egg-info/PKG-INFO` & `polysplit-0.1.2/polysplit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polysplit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library implementing a method for splitting a polygon into regions
 Author-email: Dmitrii Zakharov <d.zakharov@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Dmitrii Zakharov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,14 +33,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 Provides-Extra: develop
 License-File: LICENSE
 
 # polysplit
 
 A lightweight library for splitting polygons into regions based on proximity of points.\
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `polysplit-0.1.1/pyproject.toml` & `polysplit-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 [build-system]
 requires = [
     "setuptools",
     "setuptools-scm",
     "wheel",
+    "black>=22",
+    "bump2version>=1.0.0",
+    "check-manifest",
+    "flake8>=3.7.8",
+    "flake8-black>=0.2.1",
+    "flake8-pyproject",
+    "mypy",
+    "pytest>=4.3.0",
+    "pytest-cov>=2.6.1",
+    "twine",
+    "matplotlib",
+    "shapely",
+    "numpy",
+    "scikit-learn>=1.2.1",
+    "scikit-learn-extra>=0.2.0",
+    "networkx"
 ]
 build-backend="setuptools.build_meta"
-package_dir = {'' = 'polysplit'}
 
 [project]
 name = "polysplit"
 authors = [{name = "Dmitrii Zakharov", email = "d.zakharov@columbia.edu"}]
 description="A Python library implementing a method for splitting a polygon into regions"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

