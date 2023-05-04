# Comparing `tmp/apify_client-1.1.0a2.tar.gz` & `tmp/apify_client-1.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.1.0a2.tar", last modified: Thu May  4 17:52:48 2023, max compression
+gzip compressed data, was "apify_client-1.1.0a3.tar", last modified: Thu May  4 18:29:44 2023, max compression
```

## Comparing `apify_client-1.1.0a2.tar` & `apify_client-1.1.0a3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-04 17:52:44.000000 apify_client-1.1.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-04 18:29:41.000000 apify_client-1.1.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:44.642367 apify_client-1.1.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/src/apify_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/src/apify_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/top_level.txt
```

### Comparing `apify_client-1.1.0a2/LICENSE` & `apify_client-1.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a2/PKG-INFO` & `apify_client-1.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.1.0a2
+Version: 1.1.0a3
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.1.0a2/README.md` & `apify_client-1.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a2/pyproject.toml` & `apify_client-1.1.0a3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "apify_client"
 
-version = "1.1.0a2"
+version = "1.1.0a3"
 description = "Apify API client for Python"
 
 readme = "README.md"
 
 license = {text = "Apache Software License"}
 
 authors = [
@@ -43,67 +43,69 @@
 
 
 
 requires-python = ">=3.8"
 
 dependencies = [
 
-    "httpx ~= 0.23.0"
+    "httpx ~= 0.24.0"
 
 ]
 
 
 
 [project.optional-dependencies]
 
 dev = [
 
-    "autopep8 ~= 2.0.1",
+    "autopep8 ~= 2.0.2",
+
+    "build ~= 0.10.0",
 
     "flake8 ~= 6.0.0",
 
-    "flake8-bugbear ~= 23.1.20",
+    "flake8-bugbear ~= 23.3.23",
 
     "flake8-commas ~= 2.1.0",
 
-    "flake8-comprehensions ~= 3.10.1",
+    "flake8-comprehensions ~= 3.12.0",
 
     "flake8-datetimez ~= 20.10.0",
 
     "flake8-docstrings ~= 1.7.0",
 
     "flake8-isort ~= 6.0.0",
 
-    "flake8-noqa ~= 1.3.0",
+    "flake8-noqa ~= 1.3.1",
 
     "flake8-pytest-style ~= 1.7.2",
 
-    "flake8-quotes ~= 3.3.1",
+    "flake8-quotes ~= 3.3.2",
 
     "flake8-unused-arguments ~= 0.0.13",
 
     "isort ~= 5.12.0",
 
-    "mypy ~= 1.0.0",
+    "mypy ~= 1.2.0",
 
-    "pep8-naming ~= 0.13.2",
+    "pep8-naming ~= 0.13.3",
 
-    "pre-commit ~= 3.0.1",
+    "pre-commit ~= 3.3.1",
 
-    "pytest ~= 7.2.0",
+    "pytest ~= 7.3.1",
 
-    "pytest-asyncio ~= 0.20.3",
+    "pytest-asyncio ~= 0.21.0",
 
     "pytest-only ~= 2.0.0",
 
     "pytest-randomly ~= 3.12.0",
 
     "pytest-timeout ~= 2.1.0",
 
-    "pytest-xdist ~= 3.2.0",
+    "pytest-xdist ~= 3.2.1",
 
     "redbaron ~= 0.9.2",
 
     "sphinx ~= 6.1.3",
 
     "sphinx-autodoc-typehints ~= 1.22",
```

### Comparing `apify_client-1.1.0a2/src/apify_client/_errors.py` & `apify_client-1.1.0a3/src/apify_client/_errors.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a2/src/apify_client/_http_client.py` & `apify_client-1.1.0a3/src/apify_client/_http_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a2/src/apify_client/_logging.py` & `apify_client-1.1.0a3/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a2/src/apify_client/_utils.py` & `apify_client-1.1.0a3/src/apify_client/_utils.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a2/src/apify_client/client.py` & `apify_client-1.1.0a3/src/apify_client/client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a2/src/apify_client/consts.py` & `apify_client-1.1.0a3/src/apify_client/consts.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a2/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.1.0a3/src/apify_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-client
-Version: 1.1.0a2
+Version: 1.1.0a3
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.1.0a2/src/apify_client.egg-info/requires.txt` & `apify_client-1.1.0a3/src/apify_client.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-httpx~=0.23.0
+httpx~=0.24.0
 
 [dev]
-autopep8~=2.0.1
+autopep8~=2.0.2
+build~=0.10.0
 flake8~=6.0.0
-flake8-bugbear~=23.1.20
+flake8-bugbear~=23.3.23
 flake8-commas~=2.1.0
-flake8-comprehensions~=3.10.1
+flake8-comprehensions~=3.12.0
 flake8-datetimez~=20.10.0
 flake8-docstrings~=1.7.0
 flake8-isort~=6.0.0
-flake8-noqa~=1.3.0
+flake8-noqa~=1.3.1
 flake8-pytest-style~=1.7.2
-flake8-quotes~=3.3.1
+flake8-quotes~=3.3.2
 flake8-unused-arguments~=0.0.13
 isort~=5.12.0
-mypy~=1.0.0
-pep8-naming~=0.13.2
-pre-commit~=3.0.1
-pytest~=7.2.0
-pytest-asyncio~=0.20.3
+mypy~=1.2.0
+pep8-naming~=0.13.3
+pre-commit~=3.3.1
+pytest~=7.3.1
+pytest-asyncio~=0.21.0
 pytest-only~=2.0.0
 pytest-randomly~=3.12.0
 pytest-timeout~=2.1.0
-pytest-xdist~=3.2.0
+pytest-xdist~=3.2.1
 redbaron~=0.9.2
 sphinx~=6.1.3
 sphinx-autodoc-typehints~=1.22
 sphinx-markdown-builder==0.5.4
 twine~=4.0.2
```

