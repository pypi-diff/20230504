# Comparing `tmp/msgraphy-0.3.5.tar.gz` & `tmp/msgraphy-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgraphy-0.3.5.tar", max compression
+gzip compressed data, was "msgraphy-0.3.6.tar", max compression
```

## Comparing `msgraphy-0.3.5.tar` & `msgraphy-0.3.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1068 2023-05-04 13:56:01.515912 msgraphy-0.3.5/LICENSE
--rw-r--r--   0        0        0       91 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/__init__.py
--rw-r--r--   0        0        0     1300 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/api.py
--rw-r--r--   0        0        0        0 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/auth/__init__.py
--rw-r--r--   0        0        0     2914 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/auth/config.py
--rw-r--r--   0        0        0     4642 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/auth/graph_auth.py
--rw-r--r--   0        0        0     3057 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/cli/__commands.py
--rw-r--r--   0        0        0       57 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/cli/__init__.py
--rw-r--r--   0        0        0      153 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/cli/__settings.py
--rw-r--r--   0        0        0        0 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/client/__init__.py
--rw-r--r--   0        0        0     3626 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/client/graph_batch.py
--rw-r--r--   0        0        0     3662 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/client/graph_client.py
--rw-r--r--   0        0        0     3601 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/__init__.py
--rw-r--r--   0        0        0     2469 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/file.py
--rw-r--r--   0        0        0     1355 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/group.py
--rw-r--r--   0        0        0      274 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/identity.py
--rw-r--r--   0        0        0      584 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/list.py
--rw-r--r--   0        0        0      533 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/monitor.py
--rw-r--r--   0        0        0     1051 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/sharepoint.py
--rw-r--r--   0        0        0      576 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/site_page.py
--rw-r--r--   0        0        0      727 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/team.py
--rw-r--r--   0        0        0      796 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/user.py
--rw-r--r--   0        0        0     1432 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/workbook.py
--rw-r--r--   0        0        0        0 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/__init__.py
--rw-r--r--   0        0        0     7187 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/files.py
--rw-r--r--   0        0        0     1192 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/group.py
--rw-r--r--   0        0        0     3009 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/list.py
--rw-r--r--   0        0        0      295 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/monitor.py
--rw-r--r--   0        0        0     1768 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/sharepoint.py
--rw-r--r--   0        0        0     2772 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/team.py
--rw-r--r--   0        0        0     1425 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/user.py
--rw-r--r--   0        0        0     6299 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/workbook.py
--rw-r--r--   0        0        0        0 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/fs/__init__.py
--rw-r--r--   0        0        0     8125 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/fs/onedrivefs.py
--rw-r--r--   0        0        0      606 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/fs/opener.py
--rw-r--r--   0        0        0     3258 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/sharepoint_classic/__init__.py
--rw-r--r--   0        0        0     1006 2023-05-04 13:56:01.523912 msgraphy-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 msgraphy-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-04 15:38:13.606407 msgraphy-0.3.6/LICENSE
+-rw-r--r--   0        0        0       91 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/__init__.py
+-rw-r--r--   0        0        0     1300 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/api.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/auth/__init__.py
+-rw-r--r--   0        0        0     3406 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/auth/config.py
+-rw-r--r--   0        0        0     5056 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/auth/graph_auth.py
+-rw-r--r--   0        0        0     3057 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/cli/__commands.py
+-rw-r--r--   0        0        0       57 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/cli/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/cli/__settings.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/client/__init__.py
+-rw-r--r--   0        0        0     3626 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/client/graph_batch.py
+-rw-r--r--   0        0        0     3662 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/client/graph_client.py
+-rw-r--r--   0        0        0     3601 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/__init__.py
+-rw-r--r--   0        0        0     2469 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/file.py
+-rw-r--r--   0        0        0     1355 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/group.py
+-rw-r--r--   0        0        0      274 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/identity.py
+-rw-r--r--   0        0        0      584 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/list.py
+-rw-r--r--   0        0        0      533 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/monitor.py
+-rw-r--r--   0        0        0     1051 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/sharepoint.py
+-rw-r--r--   0        0        0      576 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/site_page.py
+-rw-r--r--   0        0        0      727 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/team.py
+-rw-r--r--   0        0        0      796 2023-05-04 15:38:13.606407 msgraphy-0.3.6/msgraphy/data/user.py
+-rw-r--r--   0        0        0     1432 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/data/workbook.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/__init__.py
+-rw-r--r--   0        0        0     7187 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/files.py
+-rw-r--r--   0        0        0     1192 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/group.py
+-rw-r--r--   0        0        0     3009 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/list.py
+-rw-r--r--   0        0        0      295 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/monitor.py
+-rw-r--r--   0        0        0     1768 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/sharepoint.py
+-rw-r--r--   0        0        0     2772 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/team.py
+-rw-r--r--   0        0        0     1425 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/user.py
+-rw-r--r--   0        0        0     6299 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/domains/workbook.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/fs/__init__.py
+-rw-r--r--   0        0        0     8125 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/fs/onedrivefs.py
+-rw-r--r--   0        0        0      606 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/fs/opener.py
+-rw-r--r--   0        0        0     3258 2023-05-04 15:38:13.610407 msgraphy-0.3.6/msgraphy/sharepoint_classic/__init__.py
+-rw-r--r--   0        0        0     1006 2023-05-04 15:38:13.610407 msgraphy-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 msgraphy-0.3.6/PKG-INFO
```

### Comparing `msgraphy-0.3.5/LICENSE` & `msgraphy-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/api.py` & `msgraphy-0.3.6/msgraphy/api.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/auth/config.py` & `msgraphy-0.3.6/msgraphy/auth/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,26 @@
             tenant_id = os.getenv(f'{env_prefix}_TENANT_ID')
         self.tenant_id = tenant_id
 
         if not authority:
             authority = os.getenv(f'{env_prefix}_AUTHORITY')
 
         if device_flow is None:
-            device_flow = bool(os.getenv(f'{env_prefix}_DEVICE_FLOW', "False"))
+            device_flow = os.getenv(f'{env_prefix}_DEVICE_FLOW')
+
+        if isinstance(device_flow, str):
+            if device_flow.lower() in ['true', '1', 'yes', 'y', 't']:
+                from .graph_auth import default_device_flow_handler
+                device_flow = default_device_flow_handler
+            else:
+                try:
+                    from pkgutil import resolve_name
+                except ImportError:
+                    raise Exception("Using resolver plugins requires Python >= 3.9")
+                device_flow = resolve_name(device_flow)
         self.device_flow = device_flow
 
         if not authority:
             if tenant_id:
                 authority = f"https://login.microsoftonline.com/{tenant_id}"
             else:
                 raise Exception("Either 'authority' or 'tenant_id' must be set")
```

### Comparing `msgraphy-0.3.5/msgraphy/auth/graph_auth.py` & `msgraphy-0.3.6/msgraphy/auth/graph_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 import atexit
 from pathlib import Path
-from typing import List, Union
+from typing import Callable, List, Union
 import msal
 
 from msgraphy.auth.config import MSGraphyConfig
 
 
+def default_device_flow_handler(device_code):
+    myprint = print
+    try:
+        from rich import print as myprint
+    except ImportError:
+        pass
+    myprint(device_code['message'])
+
+
 class FileSystemTokenCache(msal.SerializableTokenCache):
     """
     A very basic implementation of the MSAL SerializableTokenCache that stores the cached credentials
     in a file.
 
     Think carefully before using whether this is safe enough for your purposes. Ideally use as a wrapper around
     your protected credential store.
@@ -43,27 +52,33 @@
 
 
     To use this, simply pass to the Graph Client:
     RequestsGraphClient(InteractiveTokenWrapper(PublicClientApplication(....), ['Scope1', 'Scope2']))
 
     """
 
-    def __init__(self, app: msal.PublicClientApplication, scopes: List[str], device_flow=False):
+    def __init__(self, app: msal.PublicClientApplication, scopes: List[str], device_flow: Callable = None):
         self.__app = app
         self.__scopes = scopes
+
+        # Support older versions of configuration
+        if isinstance(device_flow, bool) and device_flow:
+            device_flow = default_device_flow_handler
+
         self.__device_flow = device_flow
 
     def __call__(self):
         for account in self.__app.get_accounts():
             result = self.__app.acquire_token_silent(self.__scopes, account=account)
             if result and 'access_token' in result and result.get('expires_in', 0) > 30:
                 return result['access_token']
 
         if self.__device_flow:
             flow = self.__app.initiate_device_flow(self.__scopes)
+            self.__device_flow(flow)
             result = self.__app.acquire_token_by_device_flow(flow)
         else:
             result = self.__app.acquire_token_interactive(self.__scopes)
         return result['access_token']
 
 
 class ConfidentialTokenWrapper:
```

### Comparing `msgraphy-0.3.5/msgraphy/cli/__commands.py` & `msgraphy-0.3.6/msgraphy/cli/__commands.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/client/graph_batch.py` & `msgraphy-0.3.6/msgraphy/client/graph_batch.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/client/graph_client.py` & `msgraphy-0.3.6/msgraphy/client/graph_client.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/__init__.py` & `msgraphy-0.3.6/msgraphy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/file.py` & `msgraphy-0.3.6/msgraphy/data/file.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/group.py` & `msgraphy-0.3.6/msgraphy/data/group.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/list.py` & `msgraphy-0.3.6/msgraphy/data/list.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/monitor.py` & `msgraphy-0.3.6/msgraphy/data/monitor.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/sharepoint.py` & `msgraphy-0.3.6/msgraphy/data/sharepoint.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/site_page.py` & `msgraphy-0.3.6/msgraphy/data/site_page.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/team.py` & `msgraphy-0.3.6/msgraphy/data/team.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/user.py` & `msgraphy-0.3.6/msgraphy/data/user.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/data/workbook.py` & `msgraphy-0.3.6/msgraphy/data/workbook.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/domains/files.py` & `msgraphy-0.3.6/msgraphy/domains/files.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/domains/group.py` & `msgraphy-0.3.6/msgraphy/domains/group.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/domains/list.py` & `msgraphy-0.3.6/msgraphy/domains/list.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/domains/sharepoint.py` & `msgraphy-0.3.6/msgraphy/domains/sharepoint.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/domains/team.py` & `msgraphy-0.3.6/msgraphy/domains/team.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/domains/user.py` & `msgraphy-0.3.6/msgraphy/domains/user.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/domains/workbook.py` & `msgraphy-0.3.6/msgraphy/domains/workbook.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/fs/onedrivefs.py` & `msgraphy-0.3.6/msgraphy/fs/onedrivefs.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/fs/opener.py` & `msgraphy-0.3.6/msgraphy/fs/opener.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/msgraphy/sharepoint_classic/__init__.py` & `msgraphy-0.3.6/msgraphy/sharepoint_classic/__init__.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.5/pyproject.toml` & `msgraphy-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msgraphy"
-version = "0.3.5"
+version = "0.3.6"
 description = "An API generator for the MS Graph API"
 authors = ["Kaj Siebert <kaj@k-si.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.7, <4"
 msal = "^1.10.0"
```

### Comparing `msgraphy-0.3.5/PKG-INFO` & `msgraphy-0.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgraphy
-Version: 0.3.5
+Version: 0.3.6
 Summary: An API generator for the MS Graph API
 License: MIT
 Author: Kaj Siebert
 Author-email: kaj@k-si.com
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

