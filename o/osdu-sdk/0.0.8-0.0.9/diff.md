# Comparing `tmp/osdu-sdk-0.0.8.tar.gz` & `tmp/osdu-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osdu-sdk-0.0.8.tar", last modified: Mon Nov  1 14:05:01 2021, max compression
+gzip compressed data, was "osdu-sdk-0.0.9.tar", last modified: Wed Dec  8 11:26:57 2021, max compression
```

## Comparing `osdu-sdk-0.0.8.tar` & `osdu-sdk-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 14:05:01.194266 osdu-sdk-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-11-01 14:05:01.194266 osdu-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      668 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-01 14:05:01.194266 osdu-sdk-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 14:05:01.190266 osdu-sdk-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 14:05:01.190266 osdu-sdk-0.0.8/src/osdu/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7642 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 14:05:01.190266 osdu-sdk-0.0.8/src/osdu/entitlements/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/entitlements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3620 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/entitlements/_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 14:05:01.190266 osdu-sdk-0.0.8/src/osdu/identity/
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/identity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 14:05:01.194266 osdu-sdk-0.0.8/src/osdu/identity/_credential/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/identity/_credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/identity/_credential/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4518 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/identity/_credential/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     6036 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/identity/_credential/msal_interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     4605 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/identity/_credential/token.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/identity/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/identity/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 14:05:01.194266 osdu-sdk-0.0.8/src/osdu/search/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/search/_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3145 2021-11-01 14:04:37.000000 osdu-sdk-0.0.8/src/osdu/serviceclientbase.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-01 14:05:01.194266 osdu-sdk-0.0.8/src/osdu_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-11-01 14:05:01.000000 osdu-sdk-0.0.8/src/osdu_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      705 2021-11-01 14:05:01.000000 osdu-sdk-0.0.8/src/osdu_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-01 14:05:01.000000 osdu-sdk-0.0.8/src/osdu_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-11-01 14:05:01.000000 osdu-sdk-0.0.8/src/osdu_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-01 14:05:01.000000 osdu-sdk-0.0.8/src/osdu_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 11:26:57.657533 osdu-sdk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1566 2021-12-08 11:26:57.657533 osdu-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      811 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-08 11:26:57.657533 osdu-sdk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 11:26:57.653533 osdu-sdk-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 11:26:57.653533 osdu-sdk-0.0.9/src/osdu/
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7642 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 11:26:57.657533 osdu-sdk-0.0.9/src/osdu/entitlements/
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/entitlements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3620 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/entitlements/_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 11:26:57.657533 osdu-sdk-0.0.9/src/osdu/identity/
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/identity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 11:26:57.657533 osdu-sdk-0.0.9/src/osdu/identity/_credential/
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/identity/_credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/identity/_credential/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4518 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/identity/_credential/environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6036 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/identity/_credential/msal_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4605 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/identity/_credential/token.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/identity/consts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/identity/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 11:26:57.657533 osdu-sdk-0.0.9/src/osdu/search/
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4530 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/search/_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3145 2021-12-08 11:26:36.000000 osdu-sdk-0.0.9/src/osdu/serviceclientbase.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 11:26:57.657533 osdu-sdk-0.0.9/src/osdu_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1566 2021-12-08 11:26:57.000000 osdu-sdk-0.0.9/src/osdu_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2021-12-08 11:26:57.000000 osdu-sdk-0.0.9/src/osdu_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-08 11:26:57.000000 osdu-sdk-0.0.9/src/osdu_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-12-08 11:26:57.000000 osdu-sdk-0.0.9/src/osdu_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-08 11:26:57.000000 osdu-sdk-0.0.9/src/osdu_sdk.egg-info/top_level.txt
```

### Comparing `osdu-sdk-0.0.8/LICENSE.md` & `osdu-sdk-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/PKG-INFO` & `osdu-sdk-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osdu-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: OSDU SDK for Python
 Home-page: https://github.com/equinor/osdu-sdk-python
 Author: Equinor ASA
 Author-email: mhew@equinor.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/equinor/osdu-sdk-python/issues
 Keywords: osdu sdk python
@@ -28,15 +28,22 @@
 Usage
 =====
 
 Note: This is currently a WIP so will be subject to breaking changes.
 
 Change Log
 ==========
-                  
+                   
+0.0.9
+-----
+
+- Search query_by_kind function
+- Search query_by_id supports limit
+- Search query supports a specific query
+                   
 0.0.8
 -----
 
 - search query supports limit
 
 0.0.7
 -----
```

### Comparing `osdu-sdk-0.0.8/README.rst` & `osdu-sdk-0.0.9/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,22 @@
 Usage
 =====
 
 Note: This is currently a WIP so will be subject to breaking changes.
 
 Change Log
 ==========
-                  
+                   
+0.0.9
+-----
+
+- Search query_by_kind function
+- Search query_by_id supports limit
+- Search query supports a specific query
+                   
 0.0.8
 -----
 
 - search query supports limit
 
 0.0.7
 -----
```

### Comparing `osdu-sdk-0.0.8/setup.py` & `osdu-sdk-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/client.py` & `osdu-sdk-0.0.9/src/osdu/client.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/entitlements/_client.py` & `osdu-sdk-0.0.9/src/osdu/entitlements/_client.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/identity/__init__.py` & `osdu-sdk-0.0.9/src/osdu/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/identity/_credential/__init__.py` & `osdu-sdk-0.0.9/src/osdu/identity/_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/identity/_credential/base.py` & `osdu-sdk-0.0.9/src/osdu/identity/_credential/base.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/identity/_credential/environment.py` & `osdu-sdk-0.0.9/src/osdu/identity/_credential/environment.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/identity/_credential/msal_interactive.py` & `osdu-sdk-0.0.9/src/osdu/identity/_credential/msal_interactive.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/identity/_credential/token.py` & `osdu-sdk-0.0.9/src/osdu/identity/_credential/token.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/identity/consts.py` & `osdu-sdk-0.0.9/src/osdu/identity/consts.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/identity/exceptions.py` & `osdu-sdk-0.0.9/src/osdu/identity/exceptions.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu/search/_client.py` & `osdu-sdk-0.0.9/src/osdu/search/_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,48 +57,79 @@
         Returns:
             dict: containing the result
         """
         request_data = {"kind": "*:*:*:*", "limit": 1, "query": "*", "aggregateBy": "kind"}
         response_json = self._client.post_returning_json(self.api_url("query"), request_data)
         return response_json
 
-    def query(self, kind: str = None, identifier: str = None, limit: int = None) -> dict:
+    def query(
+        self, kind: str = None, identifier: str = None, query: str = None, limit: int = None
+    ) -> dict:
         """Query records
 
         Args:
             kind (str): kind to query for
             identifier (str): id to query for
+            query (str): a specific query
+            limit (str): limit on number of records to return
 
         Returns:
             dict: containing the result
         """
+
+        if identifier is not None and query is not None:
+            raise ValueError("You can't specify both identifier and query")
+
         request_data = {}
         if kind is None:
             request_data["kind"] = "*:*:*:*"
         else:
             request_data["kind"] = kind
 
         if identifier is not None:
             request_data["query"] = f'id:("{identifier}")'
 
+        if query is not None:
+            request_data["query"] = query
+
         if limit is not None:
             request_data["limit"] = limit
 
         response_json = self._client.post_returning_json(self.api_url("query"), request_data)
         return response_json
 
-    def query_by_id(self, identifier: str) -> dict:
+    def query_by_id(self, identifier: str, limit: int = None) -> dict:
         """Returns a list of all kinds including number of records
 
         Args:
             identifier (str): id to query for
 
         Returns:
             dict: containing the result
         """
         request_data = {
             "kind": "*:*:*:*",
             "query": f'id:("{identifier}")',
         }
 
+        if limit is not None:
+            request_data["limit"] = limit
+
+        response_json = self._client.post_returning_json(self.api_url("query"), request_data)
+        return response_json
+
+    def query_by_kind(self, kind: str, limit: int = None) -> dict:
+        """Returns a list of all records for the given kind
+
+        Args:
+            kind (str): kind to query for
+
+        Returns:
+            dict: containing the result
+        """
+        request_data = {"kind": kind}
+
+        if limit is not None:
+            request_data["limit"] = limit
+
         response_json = self._client.post_returning_json(self.api_url("query"), request_data)
         return response_json
```

### Comparing `osdu-sdk-0.0.8/src/osdu/serviceclientbase.py` & `osdu-sdk-0.0.9/src/osdu/serviceclientbase.py`

 * *Files identical despite different names*

### Comparing `osdu-sdk-0.0.8/src/osdu_sdk.egg-info/PKG-INFO` & `osdu-sdk-0.0.9/src/osdu_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osdu-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: OSDU SDK for Python
 Home-page: https://github.com/equinor/osdu-sdk-python
 Author: Equinor ASA
 Author-email: mhew@equinor.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/equinor/osdu-sdk-python/issues
 Keywords: osdu sdk python
@@ -28,15 +28,22 @@
 Usage
 =====
 
 Note: This is currently a WIP so will be subject to breaking changes.
 
 Change Log
 ==========
-                  
+                   
+0.0.9
+-----
+
+- Search query_by_kind function
+- Search query_by_id supports limit
+- Search query supports a specific query
+                   
 0.0.8
 -----
 
 - search query supports limit
 
 0.0.7
 -----
```

### Comparing `osdu-sdk-0.0.8/src/osdu_sdk.egg-info/SOURCES.txt` & `osdu-sdk-0.0.9/src/osdu_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

