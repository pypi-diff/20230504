# Comparing `tmp/apify_client-1.1.0a1.tar.gz` & `tmp/apify_client-1.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.1.0a1.tar", last modified: Thu May  4 15:48:30 2023, max compression
+gzip compressed data, was "apify_client-1.1.0a2.tar", last modified: Thu May  4 17:52:48 2023, max compression
```

## Comparing `apify_client-1.1.0a1.tar` & `apify_client-1.1.0a2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-04 15:48:27.000000 apify_client-1.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:30.483518 apify_client-1.1.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:47:53.000000 apify_client-1.1.0a1/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:48:30.487518 apify_client-1.1.0a1/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 15:48:30.000000 apify_client-1.1.0a1/src/apify_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-04 17:52:44.000000 apify_client-1.1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/src/apify_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:06.000000 apify_client-1.1.0a2/src/apify_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:52:48.335179 apify_client-1.1.0a2/src/apify_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 17:52:48.000000 apify_client-1.1.0a2/src/apify_client.egg-info/top_level.txt
```

### Comparing `apify_client-1.1.0a1/LICENSE` & `apify_client-1.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a1/PKG-INFO` & `apify_client-1.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.1.0a1/README.md` & `apify_client-1.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a1/pyproject.toml` & `apify_client-1.1.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "apify_client"
 
-version = "1.1.0a1"
+version = "1.1.0a2"
 description = "Apify API client for Python"
 
 readme = "README.md"
 
 license = {text = "Apache Software License"}
 
 authors = [
```

### Comparing `apify_client-1.1.0a1/src/apify_client/_errors.py` & `apify_client-1.1.0a2/src/apify_client/_errors.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a1/src/apify_client/_http_client.py` & `apify_client-1.1.0a2/src/apify_client/_http_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a1/src/apify_client/_logging.py` & `apify_client-1.1.0a2/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a1/src/apify_client/_utils.py` & `apify_client-1.1.0a2/src/apify_client/_utils.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a1/src/apify_client/client.py` & `apify_client-1.1.0a2/src/apify_client/client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a1/src/apify_client/consts.py` & `apify_client-1.1.0a2/src/apify_client/consts.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a1/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.1.0a2/src/apify_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-client
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.1.0a1/src/apify_client.egg-info/requires.txt` & `apify_client-1.1.0a2/src/apify_client.egg-info/requires.txt`

 * *Files identical despite different names*

