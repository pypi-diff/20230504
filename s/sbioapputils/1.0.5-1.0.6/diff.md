# Comparing `tmp/sbioapputils-1.0.5.tar.gz` & `tmp/sbioapputils-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbioapputils-1.0.5.tar", last modified: Thu May  4 16:56:24 2023, max compression
+gzip compressed data, was "sbioapputils-1.0.6.tar", last modified: Thu May  4 17:06:56 2023, max compression
```

## Comparing `sbioapputils-1.0.5.tar` & `sbioapputils-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:56:24.558387 sbioapputils-1.0.5/
--rw-rw-rw-   0        0        0    35823 2023-05-03 10:08:17.000000 sbioapputils-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      783 2023-05-04 16:56:24.557882 sbioapputils-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-03 10:08:17.000000 sbioapputils-1.0.5/README.md
--rw-rw-rw-   0        0        0      837 2023-05-04 16:56:00.000000 sbioapputils-1.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-04 16:56:24.546023 sbioapputils-1.0.5/sbioapputils/
--rw-rw-rw-   0        0        0        0 2023-05-04 16:55:55.000000 sbioapputils-1.0.5/sbioapputils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:56:24.556091 sbioapputils-1.0.5/sbioapputils.egg-info/
--rw-rw-rw-   0        0        0      783 2023-05-04 16:56:24.000000 sbioapputils-1.0.5/sbioapputils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-04 16:56:24.000000 sbioapputils-1.0.5/sbioapputils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:56:24.000000 sbioapputils-1.0.5/sbioapputils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-04 16:56:24.000000 sbioapputils-1.0.5/sbioapputils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 16:56:24.000000 sbioapputils-1.0.5/sbioapputils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 16:56:24.558387 sbioapputils-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      405 2023-05-04 16:31:23.000000 sbioapputils-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:06:56.412286 sbioapputils-1.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-05-03 10:08:17.000000 sbioapputils-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      783 2023-05-04 17:06:56.411286 sbioapputils-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-03 10:08:17.000000 sbioapputils-1.0.6/README.md
+-rw-rw-rw-   0        0        0      837 2023-05-04 17:06:52.000000 sbioapputils-1.0.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-04 17:06:56.404285 sbioapputils-1.0.6/sbioapputils/
+-rw-rw-rw-   0        0        0      222 2023-05-04 17:06:31.000000 sbioapputils-1.0.6/sbioapputils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:06:56.410285 sbioapputils-1.0.6/sbioapputils.egg-info/
+-rw-rw-rw-   0        0        0      783 2023-05-04 17:06:56.000000 sbioapputils-1.0.6/sbioapputils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-04 17:06:56.000000 sbioapputils-1.0.6/sbioapputils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:06:56.000000 sbioapputils-1.0.6/sbioapputils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-04 17:06:56.000000 sbioapputils-1.0.6/sbioapputils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 17:06:56.000000 sbioapputils-1.0.6/sbioapputils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:06:56.412286 sbioapputils-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      405 2023-05-04 16:31:23.000000 sbioapputils-1.0.6/setup.py
```

### Comparing `sbioapputils-1.0.5/LICENSE` & `sbioapputils-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sbioapputils-1.0.5/PKG-INFO` & `sbioapputils-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbioapputils
-Version: 1.0.5
+Version: 1.0.6
 Summary: Utilities for developing apps with Superbio
 Home-page: https://github.com/Superbio-ai/app-sbioutils
 Author: Superbio AI
 Author-email: Superbio AI <smorgan@superbio.ai>
 Project-URL: Homepage, https://github.com/Superbio-ai/app-sbioutils
 Project-URL: Bug Tracker, https://github.com/Superbio-ai/app-sbioutils/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sbioapputils-1.0.5/pyproject.toml` & `sbioapputils-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=65"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "sbioapputils"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Superbio AI", email="smorgan@superbio.ai" },
 ]
 description = "Utilities for developing apps with Superbio"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `sbioapputils-1.0.5/sbioapputils.egg-info/PKG-INFO` & `sbioapputils-1.0.6/sbioapputils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbioapputils
-Version: 1.0.5
+Version: 1.0.6
 Summary: Utilities for developing apps with Superbio
 Home-page: https://github.com/Superbio-ai/app-sbioutils
 Author: Superbio AI
 Author-email: Superbio AI <smorgan@superbio.ai>
 Project-URL: Homepage, https://github.com/Superbio-ai/app-sbioutils
 Project-URL: Bug Tracker, https://github.com/Superbio-ai/app-sbioutils/issues
 Classifier: Programming Language :: Python :: 3
```

