# Comparing `tmp/brim_cloud_client-1.0.0.tar.gz` & `tmp/brim_cloud_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brim_cloud_client-1.0.0.tar", last modified: Wed May  3 23:58:38 2023, max compression
+gzip compressed data, was "brim_cloud_client-1.0.1.tar", last modified: Thu May  4 00:03:32 2023, max compression
```

## Comparing `brim_cloud_client-1.0.0.tar` & `brim_cloud_client-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-03 23:58:38.144503 brim_cloud_client-1.0.0/
--rw-rw-r--   0 lance     (1001) lance     (1001)    35149 2023-05-03 22:18:27.000000 brim_cloud_client-1.0.0/LICENSE
--rw-rw-r--   0 lance     (1001) lance     (1001)     1108 2023-05-03 23:58:38.144503 brim_cloud_client-1.0.0/PKG-INFO
--rw-rw-r--   0 lance     (1001) lance     (1001)      546 2023-05-03 23:35:48.000000 brim_cloud_client-1.0.0/README.md
--rw-rw-r--   0 lance     (1001) lance     (1001)      635 2023-05-03 23:55:15.000000 brim_cloud_client-1.0.0/pyproject.toml
--rw-rw-r--   0 lance     (1001) lance     (1001)       38 2023-05-03 23:58:38.144503 brim_cloud_client-1.0.0/setup.cfg
-drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-03 23:58:38.132503 brim_cloud_client-1.0.0/src/
-drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-03 23:58:38.140503 brim_cloud_client-1.0.0/src/brim_cloud_client/
--rw-rw-r--   0 lance     (1001) lance     (1001)     2076 2023-05-03 23:26:55.000000 brim_cloud_client-1.0.0/src/brim_cloud_client/BRIM.py
--rw-rw-r--   0 lance     (1001) lance     (1001)        0 2023-05-03 23:32:45.000000 brim_cloud_client-1.0.0/src/brim_cloud_client/__init__.py
--rw-rw-r--   0 lance     (1001) lance     (1001)     1665 2023-05-03 23:25:17.000000 brim_cloud_client-1.0.0/src/brim_cloud_client/loader.py
--rw-rw-r--   0 lance     (1001) lance     (1001)      254 2023-05-03 23:27:16.000000 brim_cloud_client-1.0.0/src/brim_cloud_client/test.py
-drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-03 23:58:38.144503 brim_cloud_client-1.0.0/src/brim_cloud_client.egg-info/
--rw-rw-r--   0 lance     (1001) lance     (1001)     1108 2023-05-03 23:58:38.000000 brim_cloud_client-1.0.0/src/brim_cloud_client.egg-info/PKG-INFO
--rw-rw-r--   0 lance     (1001) lance     (1001)      338 2023-05-03 23:58:38.000000 brim_cloud_client-1.0.0/src/brim_cloud_client.egg-info/SOURCES.txt
--rw-rw-r--   0 lance     (1001) lance     (1001)        1 2023-05-03 23:58:38.000000 brim_cloud_client-1.0.0/src/brim_cloud_client.egg-info/dependency_links.txt
--rw-rw-r--   0 lance     (1001) lance     (1001)       18 2023-05-03 23:58:38.000000 brim_cloud_client-1.0.0/src/brim_cloud_client.egg-info/top_level.txt
+drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-04 00:03:32.022728 brim_cloud_client-1.0.1/
+-rw-rw-r--   0 lance     (1001) lance     (1001)    35149 2023-05-03 22:18:27.000000 brim_cloud_client-1.0.1/LICENSE
+-rw-rw-r--   0 lance     (1001) lance     (1001)     1108 2023-05-04 00:03:32.018728 brim_cloud_client-1.0.1/PKG-INFO
+-rw-rw-r--   0 lance     (1001) lance     (1001)      546 2023-05-03 23:35:48.000000 brim_cloud_client-1.0.1/README.md
+-rw-rw-r--   0 lance     (1001) lance     (1001)      635 2023-05-04 00:03:24.000000 brim_cloud_client-1.0.1/pyproject.toml
+-rw-rw-r--   0 lance     (1001) lance     (1001)       38 2023-05-04 00:03:32.022728 brim_cloud_client-1.0.1/setup.cfg
+drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-04 00:03:32.006728 brim_cloud_client-1.0.1/src/
+drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-04 00:03:32.014727 brim_cloud_client-1.0.1/src/brim_cloud_client/
+-rw-rw-r--   0 lance     (1001) lance     (1001)     2094 2023-05-04 00:03:06.000000 brim_cloud_client-1.0.1/src/brim_cloud_client/BRIM.py
+-rw-rw-r--   0 lance     (1001) lance     (1001)        0 2023-05-03 23:32:45.000000 brim_cloud_client-1.0.1/src/brim_cloud_client/__init__.py
+-rw-rw-r--   0 lance     (1001) lance     (1001)     1665 2023-05-03 23:25:17.000000 brim_cloud_client-1.0.1/src/brim_cloud_client/loader.py
+-rw-rw-r--   0 lance     (1001) lance     (1001)      254 2023-05-03 23:27:16.000000 brim_cloud_client-1.0.1/src/brim_cloud_client/test.py
+drwxrwxr-x   0 lance     (1001) lance     (1001)        0 2023-05-04 00:03:32.018728 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/
+-rw-rw-r--   0 lance     (1001) lance     (1001)     1108 2023-05-04 00:03:31.000000 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/PKG-INFO
+-rw-rw-r--   0 lance     (1001) lance     (1001)      338 2023-05-04 00:03:31.000000 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 lance     (1001) lance     (1001)        1 2023-05-04 00:03:31.000000 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 lance     (1001) lance     (1001)       18 2023-05-04 00:03:31.000000 brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/top_level.txt
```

### Comparing `brim_cloud_client-1.0.0/LICENSE` & `brim_cloud_client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brim_cloud_client-1.0.0/PKG-INFO` & `brim_cloud_client-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brim_cloud_client
-Version: 1.0.0
+Version: 1.0.1
 Summary: BRIM cloud client
 Author-email: Lance1o7 <10292888+Lance1o7@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Lance1o7/brim-cloud-client
 Project-URL: Bug Tracker, https://github.com/Lance1o7/brim-cloud-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `brim_cloud_client-1.0.0/README.md` & `brim_cloud_client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `brim_cloud_client-1.0.0/pyproject.toml` & `brim_cloud_client-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brim_cloud_client"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Lance1o7", email="10292888+Lance1o7@users.noreply.github.com" },
 ]
 description = "BRIM cloud client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `brim_cloud_client-1.0.0/src/brim_cloud_client/BRIM.py` & `brim_cloud_client-1.0.1/src/brim_cloud_client/BRIM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from loader import Loader
+from brim_cloud_client.loader import Loader
 
 class TMB:
     """Client for BRIM cloud server"""
 
     def __init__(self, cm, cb, p, Rc, C, anneal=0.00011, seed=0):
         self.server_url = 'https://ord1.isingmodel.org/'
         self.api_key = ''
```

### Comparing `brim_cloud_client-1.0.0/src/brim_cloud_client/loader.py` & `brim_cloud_client-1.0.1/src/brim_cloud_client/loader.py`

 * *Files identical despite different names*

### Comparing `brim_cloud_client-1.0.0/src/brim_cloud_client.egg-info/PKG-INFO` & `brim_cloud_client-1.0.1/src/brim_cloud_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brim-cloud-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: BRIM cloud client
 Author-email: Lance1o7 <10292888+Lance1o7@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Lance1o7/brim-cloud-client
 Project-URL: Bug Tracker, https://github.com/Lance1o7/brim-cloud-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

