# Comparing `tmp/sbioapputils-1.0.3.tar.gz` & `tmp/sbioapputils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbioapputils-1.0.3.tar", last modified: Thu May  4 16:29:59 2023, max compression
+gzip compressed data, was "sbioapputils-1.0.4.tar", last modified: Thu May  4 16:50:59 2023, max compression
```

## Comparing `sbioapputils-1.0.3.tar` & `sbioapputils-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:29:59.824488 sbioapputils-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-05-03 10:08:17.000000 sbioapputils-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      783 2023-05-04 16:29:59.823490 sbioapputils-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-03 10:08:17.000000 sbioapputils-1.0.3/README.md
--rw-rw-rw-   0        0        0      837 2023-05-04 16:21:06.000000 sbioapputils-1.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-04 16:29:59.815980 sbioapputils-1.0.3/sbioapputils/
--rw-rw-rw-   0        0        0      188 2023-05-04 16:15:20.000000 sbioapputils-1.0.3/sbioapputils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:29:59.822489 sbioapputils-1.0.3/sbioapputils.egg-info/
--rw-rw-rw-   0        0        0      783 2023-05-04 16:29:59.000000 sbioapputils-1.0.3/sbioapputils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-04 16:29:59.000000 sbioapputils-1.0.3/sbioapputils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:29:59.000000 sbioapputils-1.0.3/sbioapputils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-04 16:29:59.000000 sbioapputils-1.0.3/sbioapputils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 16:29:59.000000 sbioapputils-1.0.3/sbioapputils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 16:29:59.824488 sbioapputils-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      446 2023-05-04 16:29:51.000000 sbioapputils-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:50:59.548531 sbioapputils-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-05-03 10:08:17.000000 sbioapputils-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      783 2023-05-04 16:50:59.548531 sbioapputils-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-03 10:08:17.000000 sbioapputils-1.0.4/README.md
+-rw-rw-rw-   0        0        0      837 2023-05-04 16:43:10.000000 sbioapputils-1.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-04 16:50:59.520406 sbioapputils-1.0.4/sbioapputils/
+-rw-rw-rw-   0        0        0      495 2023-05-04 16:49:40.000000 sbioapputils-1.0.4/sbioapputils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:50:59.546538 sbioapputils-1.0.4/sbioapputils.egg-info/
+-rw-rw-rw-   0        0        0      783 2023-05-04 16:50:59.000000 sbioapputils-1.0.4/sbioapputils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-04 16:50:59.000000 sbioapputils-1.0.4/sbioapputils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:50:59.000000 sbioapputils-1.0.4/sbioapputils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-04 16:50:59.000000 sbioapputils-1.0.4/sbioapputils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 16:50:59.000000 sbioapputils-1.0.4/sbioapputils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:50:59.548531 sbioapputils-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      405 2023-05-04 16:31:23.000000 sbioapputils-1.0.4/setup.py
```

### Comparing `sbioapputils-1.0.3/LICENSE` & `sbioapputils-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sbioapputils-1.0.3/PKG-INFO` & `sbioapputils-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbioapputils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Utilities for developing apps with Superbio
 Home-page: https://github.com/Superbio-ai/app-sbioutils
 Author: Superbio AI
 Author-email: Superbio AI <smorgan@superbio.ai>
 Project-URL: Homepage, https://github.com/Superbio-ai/app-sbioutils
 Project-URL: Bug Tracker, https://github.com/Superbio-ai/app-sbioutils/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sbioapputils-1.0.3/pyproject.toml` & `sbioapputils-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=65"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "sbioapputils"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Superbio AI", email="smorgan@superbio.ai" },
 ]
 description = "Utilities for developing apps with Superbio"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `sbioapputils-1.0.3/sbioapputils.egg-info/PKG-INFO` & `sbioapputils-1.0.4/sbioapputils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbioapputils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Utilities for developing apps with Superbio
 Home-page: https://github.com/Superbio-ai/app-sbioutils
 Author: Superbio AI
 Author-email: Superbio AI <smorgan@superbio.ai>
 Project-URL: Homepage, https://github.com/Superbio-ai/app-sbioutils
 Project-URL: Bug Tracker, https://github.com/Superbio-ai/app-sbioutils/issues
 Classifier: Programming Language :: Python :: 3
```

