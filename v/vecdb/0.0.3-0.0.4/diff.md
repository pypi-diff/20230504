# Comparing `tmp/vecdb-0.0.3.tar.gz` & `tmp/vecdb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecdb-0.0.3.tar", last modified: Mon May  1 23:40:11 2023, max compression
+gzip compressed data, was "vecdb-0.0.4.tar", last modified: Thu May  4 00:02:49 2023, max compression
```

## Comparing `vecdb-0.0.3.tar` & `vecdb-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-01 23:39:43.000000 vecdb-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-01 23:40:11.199694 vecdb-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 23:39:43.000000 vecdb-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-01 23:39:43.000000 vecdb-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 23:40:11.203694 vecdb-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-01 23:39:43.000000 vecdb-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.195694 vecdb-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.195694 vecdb-0.0.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.195694 vecdb-0.0.3/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_api/test_endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.195694 vecdb-0.0.3/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-01 23:39:43.000000 vecdb-0.0.3/tests/test_connection_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/api/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/collections/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/collections/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-01 23:39:43.000000 vecdb-0.0.3/vecdb/utils/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:40:11.199694 vecdb-0.0.3/vecdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 23:40:11.000000 vecdb-0.0.3/vecdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-04 00:02:28.000000 vecdb-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 00:02:49.968280 vecdb-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 00:02:28.000000 vecdb-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 00:02:28.000000 vecdb-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 00:02:49.968280 vecdb-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-04 00:02:28.000000 vecdb-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_api/test_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/api/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/collections/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/collections/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/utils/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/top_level.txt
```

### Comparing `vecdb-0.0.3/LICENSE` & `vecdb-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/setup.py` & `vecdb-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/tests/conftest.py` & `vecdb-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/tests/core/test_api/test_client.py` & `vecdb-0.0.4/tests/core/test_api/test_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+import os
 import time
+import vecdb
 import random
 
 from vecdb.api.local import Client
 from vecdb.utils.example_documents import mock_documents
 
 
 class TestClient:
+    def test_init(self):
+        vecdb.init(os.getenv("DEVELOPMENT_TOKEN"))
+        client = Client()
+        assert True
+
     def test_init_dataset(self, test_client: Client, test_dataset_id: str):
         test_client.create_dataset(test_dataset_id)
         test_client.delete_dataset(test_dataset_id)
         assert True
 
     def test_create_dataset(self, test_client: Client, test_dataset_id: str):
         dataset = test_client.create_dataset(test_dataset_id)
```

### Comparing `vecdb-0.0.3/tests/core/test_dataset/test_dataset.py` & `vecdb-0.0.4/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/tests/core/test_dataset/test_field.py` & `vecdb-0.0.4/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/vecdb/api/api.py` & `vecdb-0.0.4/vecdb/api/api.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/vecdb/api/local.py` & `vecdb-0.0.4/vecdb/api/local.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)
 
 
 class Client:
-    def __init__(self, token: str, authenticate: bool = True) -> None:
+    def __init__(self, token: str = None, authenticate: bool = True) -> None:
+        if token is None:
+            token = os.getenv("VECDB_API_KEY")
+
         self._credentials = helpers.process_token(token)
         self._token = token
         self._api = api.API(credentials=self.credentials)
 
         if authenticate:
             try:
                 self.list_datasets()["datasets"]
```

### Comparing `vecdb-0.0.3/vecdb/collections/dataset.py` & `vecdb-0.0.4/vecdb/collections/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,16 +91,20 @@
     ) -> Dict[str, Any]:
 
         encoders = [] if encoders is None else encoders
         if not encoders:
             encoders += [{"model_name": "all-mpnet-base-v2", "field": "text", "body": "text"}]
 
         if not documents:
-            assert len(data) == len(metadata)
-            documents = [{"text": d, **md} for d, md in zip(data, metadata)]
+            if metadata:
+                assert len(data) == len(metadata)
+                documents = [{"text": d, **md} for d, md in zip(data, metadata)]
+
+            else:
+                documents = [{"text": d} for d in data]
 
             if vector:
                 assert len(vector) == len(data)
                 for index, document in enumerate(documents):
                     document["text_vector_"] = vector[index]
 
             if ids:
```

### Comparing `vecdb-0.0.3/vecdb/collections/field.py` & `vecdb-0.0.4/vecdb/collections/field.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/vecdb/types.py` & `vecdb-0.0.4/vecdb/types.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/vecdb/utils/document.py` & `vecdb-0.0.4/vecdb/utils/document.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/vecdb/utils/example_documents.py` & `vecdb-0.0.4/vecdb/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/vecdb/utils/json_encoder.py` & `vecdb-0.0.4/vecdb/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.3/vecdb.egg-info/SOURCES.txt` & `vecdb-0.0.4/vecdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

