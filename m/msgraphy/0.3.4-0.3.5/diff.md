# Comparing `tmp/msgraphy-0.3.4.tar.gz` & `tmp/msgraphy-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgraphy-0.3.4.tar", max compression
+gzip compressed data, was "msgraphy-0.3.5.tar", max compression
```

## Comparing `msgraphy-0.3.4.tar` & `msgraphy-0.3.5.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     1068 2022-01-20 22:05:26.055098 msgraphy-0.3.4/LICENSE
--rw-r--r--   0        0        0       91 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/__init__.py
--rw-r--r--   0        0        0     1300 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/api.py
--rw-r--r--   0        0        0        0 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/auth/__init__.py
--rw-r--r--   0        0        0     1072 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/auth/config.py
--rw-r--r--   0        0        0     4638 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/auth/graph_auth.py
--rw-r--r--   0        0        0        0 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/client/__init__.py
--rw-r--r--   0        0        0     3626 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/client/graph_batch.py
--rw-r--r--   0        0        0     3757 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/client/graph_client.py
--rw-r--r--   0        0        0     3601 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/__init__.py
--rw-r--r--   0        0        0     2469 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/file.py
--rw-r--r--   0        0        0     1355 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/group.py
--rw-r--r--   0        0        0      274 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/identity.py
--rw-r--r--   0        0        0      584 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/list.py
--rw-r--r--   0        0        0      533 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/monitor.py
--rw-r--r--   0        0        0     1051 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/sharepoint.py
--rw-r--r--   0        0        0      576 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/site_page.py
--rw-r--r--   0        0        0      727 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/team.py
--rw-r--r--   0        0        0      796 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/user.py
--rw-r--r--   0        0        0     1432 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/data/workbook.py
--rw-r--r--   0        0        0        0 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/domains/__init__.py
--rw-r--r--   0        0        0     6392 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/domains/files.py
--rw-r--r--   0        0        0     1192 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/domains/group.py
--rw-r--r--   0        0        0     3009 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/domains/list.py
--rw-r--r--   0        0        0      295 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/domains/monitor.py
--rw-r--r--   0        0        0     1768 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/domains/sharepoint.py
--rw-r--r--   0        0        0     2772 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/domains/team.py
--rw-r--r--   0        0        0     1425 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/domains/user.py
--rw-r--r--   0        0        0     6299 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/domains/workbook.py
--rw-r--r--   0        0        0        0 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/fs/__init__.py
--rw-r--r--   0        0        0     8125 2022-01-20 22:05:26.055098 msgraphy-0.3.4/msgraphy/fs/onedrivefs.py
--rw-r--r--   0        0        0      606 2022-01-20 22:05:26.059098 msgraphy-0.3.4/msgraphy/fs/opener.py
--rw-r--r--   0        0        0     3258 2022-01-20 22:05:26.059098 msgraphy-0.3.4/msgraphy/sharepoint_classic/__init__.py
--rw-r--r--   0        0        0      668 2022-01-20 22:05:26.059098 msgraphy-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1008 2022-01-20 22:05:40.741909 msgraphy-0.3.4/setup.py
--rw-r--r--   0        0        0      685 2022-01-20 22:05:40.742236 msgraphy-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-04 13:56:01.515912 msgraphy-0.3.5/LICENSE
+-rw-r--r--   0        0        0       91 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/__init__.py
+-rw-r--r--   0        0        0     1300 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/api.py
+-rw-r--r--   0        0        0        0 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/auth/__init__.py
+-rw-r--r--   0        0        0     2914 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/auth/config.py
+-rw-r--r--   0        0        0     4642 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/auth/graph_auth.py
+-rw-r--r--   0        0        0     3057 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/cli/__commands.py
+-rw-r--r--   0        0        0       57 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/cli/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/cli/__settings.py
+-rw-r--r--   0        0        0        0 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/client/__init__.py
+-rw-r--r--   0        0        0     3626 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/client/graph_batch.py
+-rw-r--r--   0        0        0     3662 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/client/graph_client.py
+-rw-r--r--   0        0        0     3601 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/__init__.py
+-rw-r--r--   0        0        0     2469 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/file.py
+-rw-r--r--   0        0        0     1355 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/group.py
+-rw-r--r--   0        0        0      274 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/identity.py
+-rw-r--r--   0        0        0      584 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/list.py
+-rw-r--r--   0        0        0      533 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/monitor.py
+-rw-r--r--   0        0        0     1051 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/sharepoint.py
+-rw-r--r--   0        0        0      576 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/site_page.py
+-rw-r--r--   0        0        0      727 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/team.py
+-rw-r--r--   0        0        0      796 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/user.py
+-rw-r--r--   0        0        0     1432 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/data/workbook.py
+-rw-r--r--   0        0        0        0 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/__init__.py
+-rw-r--r--   0        0        0     7187 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/files.py
+-rw-r--r--   0        0        0     1192 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/group.py
+-rw-r--r--   0        0        0     3009 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/list.py
+-rw-r--r--   0        0        0      295 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/monitor.py
+-rw-r--r--   0        0        0     1768 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/sharepoint.py
+-rw-r--r--   0        0        0     2772 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/team.py
+-rw-r--r--   0        0        0     1425 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/user.py
+-rw-r--r--   0        0        0     6299 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/domains/workbook.py
+-rw-r--r--   0        0        0        0 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/fs/__init__.py
+-rw-r--r--   0        0        0     8125 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/fs/onedrivefs.py
+-rw-r--r--   0        0        0      606 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/fs/opener.py
+-rw-r--r--   0        0        0     3258 2023-05-04 13:56:01.519912 msgraphy-0.3.5/msgraphy/sharepoint_classic/__init__.py
+-rw-r--r--   0        0        0     1006 2023-05-04 13:56:01.523912 msgraphy-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 msgraphy-0.3.5/PKG-INFO
```

### Comparing `msgraphy-0.3.4/LICENSE` & `msgraphy-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/api.py` & `msgraphy-0.3.5/msgraphy/api.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/auth/graph_auth.py` & `msgraphy-0.3.5/msgraphy/auth/graph_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import atexit
-import os
 from pathlib import Path
 from typing import List, Union
 import msal
 
 from msgraphy.auth.config import MSGraphyConfig
 
 
@@ -57,15 +56,14 @@
         for account in self.__app.get_accounts():
             result = self.__app.acquire_token_silent(self.__scopes, account=account)
             if result and 'access_token' in result and result.get('expires_in', 0) > 30:
                 return result['access_token']
 
         if self.__device_flow:
             flow = self.__app.initiate_device_flow(self.__scopes)
-            print(flow['message'])
             result = self.__app.acquire_token_by_device_flow(flow)
         else:
             result = self.__app.acquire_token_interactive(self.__scopes)
         return result['access_token']
 
 
 class ConfidentialTokenWrapper:
@@ -126,12 +124,13 @@
         else:
             self.__token_fetcher = InteractiveTokenWrapper(
                 msal.PublicClientApplication(
                     config.client_id,
                     authority=config.authority,
                     token_cache=token_cache,
                 ),
-                scopes=scopes
+                scopes=scopes,
+                device_flow=config.device_flow,
             )
 
     def __call__(self):
         return self.__token_fetcher()
```

### Comparing `msgraphy-0.3.4/msgraphy/client/graph_batch.py` & `msgraphy-0.3.5/msgraphy/client/graph_batch.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/client/graph_client.py` & `msgraphy-0.3.5/msgraphy/client/graph_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,14 @@
     def single_client(self) -> "GraphClient":
         return NotImplemented
 
 
 class RequestsGraphClient(GraphClient):
     DEFAULTS = dict(
         root_url=URL_V1,
-        scope='https://graph.microsoft.com/.default',
-        grant_type='client_credentials',
         timeout=5,
     )
 
     def __init__(self, token_fetcher: Callable, **kwargs):
         self._config = {**RequestsGraphClient.DEFAULTS, **kwargs}
         self.__token_fetcher = token_fetcher
```

### Comparing `msgraphy-0.3.4/msgraphy/data/__init__.py` & `msgraphy-0.3.5/msgraphy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/data/file.py` & `msgraphy-0.3.5/msgraphy/data/file.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/data/group.py` & `msgraphy-0.3.5/msgraphy/data/group.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/data/list.py` & `msgraphy-0.3.5/msgraphy/data/list.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/data/monitor.py` & `msgraphy-0.3.5/msgraphy/data/monitor.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/data/sharepoint.py` & `msgraphy-0.3.5/msgraphy/data/sharepoint.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/data/site_page.py` & `msgraphy-0.3.5/msgraphy/data/site_page.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/data/team.py` & `msgraphy-0.3.5/msgraphy/data/team.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/data/user.py` & `msgraphy-0.3.5/msgraphy/data/user.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/data/workbook.py` & `msgraphy-0.3.5/msgraphy/data/workbook.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/domains/files.py` & `msgraphy-0.3.5/msgraphy/domains/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,34 @@
 
         resource = f"/drives/{urllib.parse.quote(drive.id)}/root"
         if filename and filename != "/":
             resource += f":{filename}"
 
         return self._api.client.make_request(url=resource, method="get", response_type=DriveItem)
 
+    def list_permissions(self, item: DriveItem, role=None, granted_to=None) -> GraphResponse:
+        filter_list = []
+        if granted_to:
+            filter_list.append(f"grantedTo/user/displayName eq '{granted_to}'")
+        if role:
+            filter_list.append(f"roles/any(x:x eq '{role}')")
+
+        params = {}
+        if filter_list:
+            params['$filter'] = " and ".join(filter_list)
+
+        return self._api.client.make_request(f"{item.get_api_reference()}/permissions", params=params)
+
+    def update_permission(self, item: DriveItem, permission_id: str, role) -> GraphResponse:
+        return self._api.client.make_request(
+            f"{item.get_api_reference()}/permissions/{permission_id}",
+            method="patch",
+            json=dict(roles=[role]),
+        )
+
     def copy(self, item: BaseItem, new_parent_ref: BaseItem = None,
              new_name: str = None, conflict_behaviour=None) -> GraphResponse[Monitor]:
         """
         Copies a file to a new location.
         :param item: This is the item you want to copy
         :param new_parent_ref: The new parent of the item [optional]
         :param new_name: The new name of the item [optional]
```

### Comparing `msgraphy-0.3.4/msgraphy/domains/group.py` & `msgraphy-0.3.5/msgraphy/domains/group.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/domains/list.py` & `msgraphy-0.3.5/msgraphy/domains/list.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/domains/sharepoint.py` & `msgraphy-0.3.5/msgraphy/domains/sharepoint.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/domains/team.py` & `msgraphy-0.3.5/msgraphy/domains/team.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/domains/user.py` & `msgraphy-0.3.5/msgraphy/domains/user.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/domains/workbook.py` & `msgraphy-0.3.5/msgraphy/domains/workbook.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/fs/onedrivefs.py` & `msgraphy-0.3.5/msgraphy/fs/onedrivefs.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/fs/opener.py` & `msgraphy-0.3.5/msgraphy/fs/opener.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/msgraphy/sharepoint_classic/__init__.py` & `msgraphy-0.3.5/msgraphy/sharepoint_classic/__init__.py`

 * *Files identical despite different names*

### Comparing `msgraphy-0.3.4/pyproject.toml` & `msgraphy-0.3.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 [tool.poetry]
 name = "msgraphy"
-version = "0.3.4"
+version = "0.3.5"
 description = "An API generator for the MS Graph API"
 authors = ["Kaj Siebert <kaj@k-si.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.7, <4"
 msal = "^1.10.0"
 requests = "^2.25.1"
 pyhumps = "^3.0.2"
 "fs.onedrivefs" = {version = "^1.1.1", optional = true}
-
+click = {version = "^8.1.3", optional = true}
+click-log = {version = "^0.4.0", optional = true}
+usersettings = {version = "^1.1.5", optional = true}
+rich = {version = "^12.6.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 python-dotenv = "^0.17.0"
 pytest = "^6.2.5"
 bump2version = "^1.0.1"
 coverage = "^6.2"
 
 [tool.poetry.extras]
 fs = ["fs.onedrivefs"]
+cli = ["click", "click-log", "usersettings", "rich"]
+
+[tool.poetry.scripts]
+msgraphy = { callable = "msgraphy:cli.msgraphy", extras = ["cli"] }
 
 [tool.poetry.plugins."fs.opener"]
 "o365" = "msgraphy.fs.opener:MSGraphyOneDriveFSOpener"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

