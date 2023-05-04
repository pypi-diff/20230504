# Comparing `tmp/version-query-1.4.0.tar.gz` & `tmp/version-query-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "version-query-1.4.0.tar", last modified: Thu May  4 13:33:42 2023, max compression
+gzip compressed data, was "version-query-1.4.0rc1.tar", last modified: Thu May  4 13:13:35 2023, max compression
```

## Comparing `version-query-1.4.0.tar` & `version-query-1.4.0rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:33:42.921837 version-query-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 13:33:36.000000 version-query-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-04 13:33:36.000000 version-query-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-04 13:33:36.000000 version-query-1.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-04 13:33:42.921837 version-query-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-05-04 13:33:36.000000 version-query-1.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-04 13:33:36.000000 version-query-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 13:33:36.000000 version-query-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 13:33:36.000000 version-query-1.4.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:33:42.921837 version-query-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-04 13:33:36.000000 version-query-1.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-05-04 13:33:36.000000 version-query-1.4.0/setup_boilerplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:33:42.921837 version-query-1.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-04 13:33:36.000000 version-query-1.4.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-04 13:33:36.000000 version-query-1.4.0/test/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-04 13:33:36.000000 version-query-1.4.0/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-05-04 13:33:36.000000 version-query-1.4.0/test/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-05-04 13:33:36.000000 version-query-1.4.0/test/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-05-04 13:33:36.000000 version-query-1.4.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-04 13:33:36.000000 version-query-1.4.0/test/test_with_git_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:33:42.921837 version-query-1.4.0/version_query/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 13:33:36.000000 version-query-1.4.0/version_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-04 13:33:36.000000 version-query-1.4.0/version_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 13:33:36.000000 version-query-1.4.0/version_query/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-04 13:33:36.000000 version-query-1.4.0/version_query/git_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-04 13:33:36.000000 version-query-1.4.0/version_query/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:33:36.000000 version-query-1.4.0/version_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-04 13:33:36.000000 version-query-1.4.0/version_query/py_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-04 13:33:36.000000 version-query-1.4.0/version_query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-05-04 13:33:36.000000 version-query-1.4.0/version_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:33:42.921837 version-query-1.4.0/version_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-04 13:33:42.000000 version-query-1.4.0/version_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 13:33:42.000000 version-query-1.4.0/version_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:33:42.000000 version-query-1.4.0/version_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 13:33:42.000000 version-query-1.4.0/version_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 13:33:42.000000 version-query-1.4.0/version_query.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/setup_boilerplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/test/test_with_git_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/version_query/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/git_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/py_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26593 2023-05-04 13:13:28.000000 version-query-1.4.0rc1/version_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:13:35.891271 version-query-1.4.0rc1/version_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 13:13:35.000000 version-query-1.4.0rc1/version_query.egg-info/top_level.txt
```

### Comparing `version-query-1.4.0/LICENSE` & `version-query-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/NOTICE` & `version-query-1.4.0rc1/NOTICE`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/PKG-INFO` & `version-query-1.4.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: version-query
-Version: 1.4.0
+Version: 1.4.0rc1
 Summary: Zero-overhead package versioning for Python.
 Home-page: https://github.com/mbdevpl/version-query
 Download-URL: 
 Author: Mateusz Bysiek, John Vandenberg
 Author-email: mateusz.bysiek@gmail.com
 Maintainer: Mateusz Bysiek
 Maintainer-email: mateusz.bysiek@gmail.com
@@ -58,15 +58,15 @@
     :alt: test coverage from Codecov
 
 .. image:: https://api.codacy.com/project/badge/Grade/437ab82bd6324530847fe8ed833f8d78
     :target: https://app.codacy.com/gh/mbdevpl/version-query
     :alt: grade from Codacy
 
 .. image:: https://img.shields.io/github/license/mbdevpl/version-query.svg
-    :target: https://github.com/mbdevpl/version-query/blob/v1.4.0/NOTICE
+    :target: https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/NOTICE
     :alt: license
 
 Package versioning toolkit for Python which relies on git tags, git history traversal
 and status of git repository to generate a very fine-grained version number.
 
 Aren't you tired hardcoding the version numbers when maintaining a Python package?!
 
@@ -468,12 +468,12 @@
 
 
 Requirements
 ============
 
 Python version 3.9 or later.
 
-Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0/requirements.txt>`_.
+Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/requirements.txt>`_.
 
-Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0/requirements_test.txt>`_.
+Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/requirements_test.txt>`_.
 
 Tested on Linux, OS X and Windows.
```

### Comparing `version-query-1.4.0/README.rst` & `version-query-1.4.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/pyproject.toml` & `version-query-1.4.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/setup.py` & `version-query-1.4.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/setup_boilerplate.py` & `version-query-1.4.0rc1/setup_boilerplate.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/test/__init__.py` & `version-query-1.4.0rc1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/test/examples.py` & `version-query-1.4.0rc1/test/examples.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/test/test_git.py` & `version-query-1.4.0rc1/test/test_git.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/test/test_query.py` & `version-query-1.4.0rc1/test/test_query.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/test/test_setup.py` & `version-query-1.4.0rc1/test/test_setup.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/test/test_version.py` & `version-query-1.4.0rc1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/test/test_with_git_repo.py` & `version-query-1.4.0rc1/test/test_with_git_repo.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/version_query/git_query.py` & `version-query-1.4.0rc1/version_query/git_query.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/version_query/main.py` & `version-query-1.4.0rc1/version_query/main.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/version_query/py_query.py` & `version-query-1.4.0rc1/version_query/py_query.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/version_query/query.py` & `version-query-1.4.0rc1/version_query/query.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/version_query/version.py` & `version-query-1.4.0rc1/version_query/version.py`

 * *Files identical despite different names*

### Comparing `version-query-1.4.0/version_query.egg-info/PKG-INFO` & `version-query-1.4.0rc1/version_query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: version-query
-Version: 1.4.0
+Version: 1.4.0rc1
 Summary: Zero-overhead package versioning for Python.
 Home-page: https://github.com/mbdevpl/version-query
 Download-URL: 
 Author: Mateusz Bysiek, John Vandenberg
 Author-email: mateusz.bysiek@gmail.com
 Maintainer: Mateusz Bysiek
 Maintainer-email: mateusz.bysiek@gmail.com
@@ -58,15 +58,15 @@
     :alt: test coverage from Codecov
 
 .. image:: https://api.codacy.com/project/badge/Grade/437ab82bd6324530847fe8ed833f8d78
     :target: https://app.codacy.com/gh/mbdevpl/version-query
     :alt: grade from Codacy
 
 .. image:: https://img.shields.io/github/license/mbdevpl/version-query.svg
-    :target: https://github.com/mbdevpl/version-query/blob/v1.4.0/NOTICE
+    :target: https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/NOTICE
     :alt: license
 
 Package versioning toolkit for Python which relies on git tags, git history traversal
 and status of git repository to generate a very fine-grained version number.
 
 Aren't you tired hardcoding the version numbers when maintaining a Python package?!
 
@@ -468,12 +468,12 @@
 
 
 Requirements
 ============
 
 Python version 3.9 or later.
 
-Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0/requirements.txt>`_.
+Python libraries as specified in `requirements.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/requirements.txt>`_.
 
-Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0/requirements_test.txt>`_.
+Building and running tests additionally requires packages listed in `requirements_test.txt <https://github.com/mbdevpl/version-query/blob/v1.4.0rc1/requirements_test.txt>`_.
 
 Tested on Linux, OS X and Windows.
```

### Comparing `version-query-1.4.0/version_query.egg-info/SOURCES.txt` & `version-query-1.4.0rc1/version_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

