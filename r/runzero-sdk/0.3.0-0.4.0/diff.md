# Comparing `tmp/runzero_sdk-0.3.0.tar.gz` & `tmp/runzero_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runzero_sdk-0.3.0.tar", max compression
+gzip compressed data, was "runzero_sdk-0.4.0.tar", max compression
```

## Comparing `runzero_sdk-0.3.0.tar` & `runzero_sdk-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      193 2023-04-26 01:02:34.446004 runzero_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0     6504 2023-04-26 01:02:34.446004 runzero_sdk-0.3.0/README.md
--rw-r--r--   0        0        0     4748 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      541 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/__init__.py
--rw-r--r--   0        0        0      636 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/__init__.py
--rw-r--r--   0        0        0      432 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/__init__.py
--rw-r--r--   0        0        0    11425 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/_sdk_source_icon.py
--rw-r--r--   0        0        0     5730 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/custom_integrations.py
--rw-r--r--   0        0        0     3423 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/orgs.py
--rw-r--r--   0        0        0     5651 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/admin/tasks.py
--rw-r--r--   0        0        0     2769 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/custom_integrations.py
--rw-r--r--   0        0        0     5059 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/explorers.py
--rw-r--r--   0        0        0     2924 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/hosted_zones.py
--rw-r--r--   0        0        0      274 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/imports/__init__.py
--rw-r--r--   0        0        0     4950 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/imports/assets.py
--rw-r--r--   0        0        0     1393 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/scans.py
--rw-r--r--   0        0        0     4500 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/sites.py
--rw-r--r--   0        0        0     4059 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/api/tasks.py
--rw-r--r--   0        0        0      441 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/__init__.py
--rw-r--r--   0        0        0      318 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/_http/__init__.py
--rw-r--r--   0        0        0     2496 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/_http/auth.py
--rw-r--r--   0        0        0     8120 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/_http/io.py
--rw-r--r--   0        0        0    11384 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/client.py
--rw-r--r--   0        0        0     7081 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/client/errors.py
--rw-r--r--   0        0        0     1077 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/errors.py
--rw-r--r--   0        0        0        0 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/py.typed
--rw-r--r--   0        0        0     1687 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/__init__.py
--rw-r--r--   0        0        0    36416 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/_data_models_gen.py
--rw-r--r--   0        0        0     2319 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/_rate_limit_information.py
--rw-r--r--   0        0        0     3410 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/_wrapped.py
--rw-r--r--   0        0        0      762 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/types/errors.py
--rw-r--r--   0        0        0      256 2023-04-26 01:02:34.450004 runzero_sdk-0.3.0/runzero/version.py
--rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 runzero_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6504 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0     4817 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      593 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/__init__.py
+-rw-r--r--   0        0        0      636 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/__init__.py
+-rw-r--r--   0        0        0      432 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/admin/__init__.py
+-rw-r--r--   0        0        0    11425 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/admin/_sdk_source_icon.py
+-rw-r--r--   0        0        0     5751 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/admin/custom_integrations.py
+-rw-r--r--   0        0        0     3427 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/admin/orgs.py
+-rw-r--r--   0        0        0     5702 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/admin/tasks.py
+-rw-r--r--   0        0        0     2760 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/custom_integrations.py
+-rw-r--r--   0        0        0     5037 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/explorers.py
+-rw-r--r--   0        0        0     2913 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/hosted_zones.py
+-rw-r--r--   0        0        0      274 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/imports/__init__.py
+-rw-r--r--   0        0        0     4953 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/imports/assets.py
+-rw-r--r--   0        0        0     1385 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/scans.py
+-rw-r--r--   0        0        0     4478 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/sites.py
+-rw-r--r--   0        0        0     5296 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/api/tasks.py
+-rw-r--r--   0        0        0      441 2023-05-04 15:20:50.097166 runzero_sdk-0.4.0/runzero/client/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/client/_http/__init__.py
+-rw-r--r--   0        0        0     2384 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/client/_http/auth.py
+-rw-r--r--   0        0        0     8120 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/client/_http/io.py
+-rw-r--r--   0        0        0    11320 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/client/client.py
+-rw-r--r--   0        0        0     7081 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/client/errors.py
+-rw-r--r--   0        0        0     1077 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/errors.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/py.typed
+-rw-r--r--   0        0        0     1687 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/types/__init__.py
+-rw-r--r--   0        0        0    36113 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/types/_data_models_gen.py
+-rw-r--r--   0        0        0     2319 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/types/_rate_limit_information.py
+-rw-r--r--   0        0        0     3410 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/types/_wrapped.py
+-rw-r--r--   0        0        0      762 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/types/errors.py
+-rw-r--r--   0        0        0      256 2023-05-04 15:20:50.101166 runzero_sdk-0.4.0/runzero/version.py
+-rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 runzero_sdk-0.4.0/PKG-INFO
```

### Comparing `runzero_sdk-0.3.0/README.md` & `runzero_sdk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/pyproject.toml` & `runzero_sdk-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runzero-sdk"
-version = "0.3.0"
+version = "0.4.0"
 description = "The runZero platform sdk"
 license = "BSD-2-Clause"
 authors = ["runZero <support@runzero.com>"]
 readme = "README.md"
 homepage = "https://runzero.com/"
 documentation = "https://runzeroinc.github.io/runzero-sdk-py"
 repository = "https://github.com/runZeroInc/runzero-sdk-py"
@@ -92,16 +92,14 @@
     commands =
       poetry run pytest --import-mode importlib --cov --with-integration --integration-cover
 
 """
 
 
 
-
-
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6.1.3"
 myst_parser = "^1.0.0"
 pandoc = "^2.3"
 sphinx-last-updated-by-git = "^0.3.4"
 sphinx-codeautolink = ">=0.14.1,<0.16.0"
 sphinx-autoapi = "^2.1.0"
@@ -190,7 +188,10 @@
   "fixme",
   "too-few-public-methods",
   "too-many-arguments", # TODO: consider re-enabling and refactoring error locations
   "too-many-branches", # TODO: consider re-enabling and refactoring error locations
   "too-many-instance-attributes", # TODO: consider re-enabling and refactoring error locations
   "unnecessary-pass",
 ]
+
+[tool.pytest.ini_options]
+addopts = "tests runzero --doctest-modules"
```

### Comparing `runzero_sdk-0.3.0/runzero/__init__.py` & `runzero_sdk-0.4.0/runzero/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,11 +11,14 @@
 from runzero.errors import APIError, Error
 from runzero.types import ValidationError
 
 __version__ = runzero.version.__version__
 
 __all__ = [
     "__version__",
+    "Client",
+    "ClientError",
+    "ServerError",
     "APIError",
     "Error",
     "ValidationError",
 ]
```

### Comparing `runzero_sdk-0.3.0/runzero/api/__init__.py` & `runzero_sdk-0.4.0/runzero/api/__init__.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/runzero/api/admin/_sdk_source_icon.py` & `runzero_sdk-0.4.0/runzero/api/admin/_sdk_source_icon.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/runzero/api/admin/custom_integrations.py` & `runzero_sdk-0.4.0/runzero/api/admin/custom_integrations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-enables administrative management of runZero custom integrations, including write operations.
+Administrative management of runZero custom integrations, including write operations.
 
 These operations are privileged and require an account token directly or an OAuth key that can generate one.
 """
 import base64
 import pathlib
 import uuid
 from pathlib import Path
@@ -15,16 +15,16 @@
 
 from ._sdk_source_icon import _PY_ICON_BYTES
 
 
 class CustomIntegrationsAdmin:
     """Full Management of custom integrations.
 
-    Full management of custom integrations are descriptive registered associations
-    between integrations of data and assets imported which are associated with those integrations.
+    Custom integrations are descriptive registered associations between integrations of data and
+    assets imported which are associated with those integrations.
 
     This is a superset of operations available in runzero.custom_integrations.CustomIntegrations
     which allows only read operations.
 
     :param client: A handle to the :class:`runzero.Client` which manages interactions
         with the runZero server.
     """
@@ -38,16 +38,16 @@
         """Constructor method"""
         self._client = client
 
     def get_all(self) -> List[CustomIntegration]:
         """
         Lists all custom integrations available to your account.
 
-        :return: List of custom integrations
-        :raises AuthError, ClientError, ServerError
+        :returns: List of custom integrations
+        :raises: AuthError, ClientError, ServerError
         """
         res = self._client.execute("GET", self._ENDPOINT)
         result: List[CustomIntegration] = []
         for src in res.json_obj:
             result.append(_resp_to_source(src))
         return result
 
@@ -55,22 +55,23 @@
         self, name: Optional[str] = None, custom_integration_id: Optional[uuid.UUID] = None
     ) -> Optional[CustomIntegration]:
         """
         Retrieves runZero custom integrations with either the matching ID or Name.
 
         :param name: Optional, name of the custom integration to retrieve
         :param custom_integration_id: Optional, the id of the custom integration to retrieve
-        :raises AuthError, ClientError, ServerError
+
+        :raises: AuthError, ClientError, ServerError
             ValueError if neither custom_integration_id nor name are provided.
-        :return: The matching CustomIntegration or None
+        :returns: The matching CustomIntegration or None
         """
         if name is None and custom_integration_id is None:
             raise ValueError("must provide custom_integration_id or source name")
         if custom_integration_id is not None:
-            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(custom_integration_id)}")
+            res = self._client.execute("GET", f"{self._ENDPOINT}/{custom_integration_id}")
             return _resp_to_source(res.json_obj)
         # name
         for src in self.get_all():
             if src.name == name:
                 return src
         return None
 
@@ -89,16 +90,16 @@
         :param icon: Optional file path to, or bytes of icon data. The icon must be
             a png formatted image with a maximum size of 32x32. Icon format
             is validated by the server. The default value assigns your custom
             data source the Python logo to indicate it was created by this SDK.
             Use None to have the server choose the default custom integration logo,
             a grey runZero logo
 
-        :return CustomIntegration created
-        :raises AuthError, ClientError, ServerError
+        :returns: CustomIntegration created
+        :raises: AuthError, ClientError, ServerError
         """
 
         if isinstance(icon, (Path, str)):
             try:
                 icon = pathlib.Path(icon).resolve()
                 with icon.open("rb") as iconf:
                     icon = iconf.read()
@@ -112,26 +113,29 @@
 
     def update(self, custom_integration_id: uuid.UUID, source_options: BaseCustomIntegration) -> CustomIntegration:
         """
         Updates a custom integration associated with your account.
 
         :param custom_integration_id: custom integration with updated values
         :param source_options: custom integration request values to update
-        :return CustomIntegration updated
-        :raises AuthError, ClientError, ServerError
+
+        :returns: CustomIntegration updated
+        :raises: AuthError, ClientError, ServerError
         """
-        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{str(custom_integration_id)}", data=source_options)
+        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{custom_integration_id}", data=source_options)
         return _resp_to_source(res.json_obj)
 
     def delete(self, custom_integration_id: uuid.UUID) -> CustomIntegration:
         """
         Deletes a custom integration from your account.
 
         :param custom_integration_id: custom integration id to delete
-        :raises AuthError, ClientError, ServerError
+
+        :returns: CustomIntegration deleted
+        :raises: AuthError, ClientError, ServerError
         """
         res = self._client.execute("DELETE", f"{self._ENDPOINT}/{custom_integration_id}")
         return _resp_to_source(res.json_obj)
 
 
 def _resp_to_source(json_obj: Any) -> CustomIntegration:
     source = CustomIntegration.parse_obj(json_obj)
```

### Comparing `runzero_sdk-0.3.0/runzero/api/admin/orgs.py` & `runzero_sdk-0.4.0/runzero/api/admin/orgs.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,50 +24,51 @@
         """Constructor method"""
         self._client = client
 
     def get_all(self) -> List[Organization]:
         """
         Retrieves all runZero Organizations available to your account
 
-        :return: A list of all Organizations available to your account
-        :raises AuthError, ClientError, ServerError
+        :returns: A list of all Organizations available to your account
+        :raises: AuthError, ClientError, ServerError
         """
         res = self._client.execute("GET", self._ENDPOINT)
         result: List[Organization] = []
         for org in res.json_obj:
             result.append(Organization.parse_obj(org))
         return result
 
     def get(self, org_id: Optional[uuid.UUID] = None, name: Optional[str] = None) -> Optional[Organization]:
         """
         Retrieves the runZero Organization with the provided name or id, if it exists in your account.
 
         :param org_id: Optional id of the organization to retrieve
         :param name: Optional name of the organization to retrieve
-        :return: Organization if found, or None
-        :raises AuthError, ClientError, ServerError
+
+        :returns: Organization if found, or None
+        :raises: AuthError, ClientError, ServerError
         """
         if name is None and org_id is None:
             raise ValueError("must provide org_id or organization name")
         if org_id is not None:
-            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(org_id)}")
+            res = self._client.execute("GET", f"{self._ENDPOINT}/{org_id}")
             return Organization.parse_obj(res.json_obj)
         # name
         for org in self.get_all():
             if org.name == name:
                 return org
         return None
 
     def create(self, org_options: OrgOptions) -> Optional[Organization]:
         """
         Creates a new organization in your account.
 
         :param org_options: Description of organization to create
-        :return Organization created or None
-        :raises AuthError, ClientError, ServerError
+        :returns: Organization created or None
+        :raises: AuthError, ClientError, ServerError
         """
         res = self._client.execute("PUT", self._ENDPOINT, data=org_options)
         obj = res.json_obj
         data_obj = obj.get("data", "")
         if data_obj:
             obj = data_obj
 
@@ -75,22 +76,22 @@
 
     def update(self, org_id: uuid.UUID, org_options: OrgOptions) -> Optional[Organization]:
         """
         Updates an organization associated with your account.
 
         :param org_id: The ID of the organization to patch
         :param org_options: Organization's updated values
-        :return Organization updated or None
-        :raises AuthError, ClientError, ServerError
+        :returns: Organization updated or None
+        :raises: AuthError, ClientError, ServerError
         """
-        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{str(org_id)}", data=org_options)
+        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{org_id}", data=org_options)
         return Organization.parse_obj(res.json_obj)
 
     def delete(self, org_id: uuid.UUID) -> None:
         """
         Deletes an organization with provided ID from your account.
 
         :param org_id: The ID of the organization to operate against
-        :return None
-        :raises AuthError, ClientError, ServerError
+        :returns: None
+        :raises: AuthError, ClientError, ServerError
         """
         self._client.execute("DELETE", f"{self._ENDPOINT}/{org_id}")
```

### Comparing `runzero_sdk-0.3.0/runzero/api/admin/tasks.py` & `runzero_sdk-0.4.0/runzero/api/admin/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         """
         Retrieves up to 1000 runZero Tasks available within all organizations in the account.
 
         :param query: An optional query to filter returned tasks.
             Query string format is the same as in-UI search. See https://www.runzero.com/docs/search-query-tasks/
         :param status: An optional status value to filter tasks by. This is a
             case-insensitive string match, stripped of surrounding whitespace.
-        :return: A list of all tasks, or tasks which match the provided query string
+
+        :returns: A list of all tasks, or tasks which match the provided query string
         """
         params = {}
         if query is not None:
             params["search"] = query.strip()
         if status is not None:
             params["status"] = status.strip()
         res = self._client.execute("GET", self._ENDPOINT, params=params)
@@ -60,18 +61,19 @@
         """Constructor method"""
         self._client = client
 
     def get_all(self, query: Optional[str] = None) -> List[ScanTemplate]:
         """
         Retrieves up to 1000 runZero task scan templates available to all organizations in the account.
 
-        :param query: An optional query to filter returned tasks.
+        :param query: An optional query to filter returned templates.
             Query string format is the same as in-UI search. See https://www.runzero.com/docs/search-query-tasks/
-        :return: A list of all task scan templates
-        :raises AuthError, ClientError, ServerError
+
+        :returns: A list of all task scan templates
+        :raises: AuthError, ClientError, ServerError
         """
         params = {}
         if query is not None:
             params["search"] = query.strip()
         res = self._client.execute("GET", f"{self._ENDPOINT}", params=params)
         result: List[ScanTemplate] = []
         for obj in res.json_obj:
@@ -81,35 +83,38 @@
 
     def get(self, name: Optional[str] = None, scan_template_id: Optional[uuid.UUID] = None) -> Optional[ScanTemplate]:
         """
         Retrieves the scan template with the provided name or id, if it exists in your account.
 
         :param name: Optional, name of the scan template to retrieve
         :param scan_template_id: Optional, the id of the scan template to retrieve
-        :raises AuthError, ClientError, ServerError
+
+        :returns: ScanTemplate created or None
+        :raises: AuthError, ClientError, ServerError
             ValueError if neither scan_template_id nor name are provided.
         """
         if name is None and scan_template_id is None:
             raise ValueError("must provide scan_template_id or scan template name")
         if scan_template_id is not None:
-            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(scan_template_id)}")
+            res = self._client.execute("GET", f"{self._ENDPOINT}/{scan_template_id}")
             return ScanTemplate.parse_obj(res.json_obj)
 
         for scan_template in self.get_all():
             if scan_template.name == name:
                 return scan_template
         return None
 
     def create(self, scan_template_options: ScanTemplateOptions) -> Optional[ScanTemplate]:
         """
         Creates a new scan template in your account.
 
         :param scan_template_options: Description of scan template to create
-        :return ScanTemplate created or None
-        :raises AuthError, ClientError, ServerError
+
+        :returns: ScanTemplate created or None
+        :raises: AuthError, ClientError, ServerError
         """
         res = self._client.execute("POST", f"{self._ENDPOINT}", data=scan_template_options)
         return ScanTemplate.parse_obj(res.json_obj)
 
     def update(
         self,
         new_scan_template_values: ScanTemplate,
@@ -118,22 +123,24 @@
         Updates an existing scan template in your account by replacing all values.
 
         The 'id' field of the ScanTemplate must match an existing scan template, which
         will be changed to the new ScanTemplate.
 
         :param scan_template_id: The id of the scan template to update
         :param new_scan_template_values: Values to update the target scan template with
-        :return ScanTemplate updated with new values or None
-        :raises AuthError, ClientError, ServerError
+
+        :returns: ScanTemplate updated with new values or None
+        :raises: AuthError, ClientError, ServerError
         """
         res = self._client.execute("PUT", f"{self._ENDPOINT}", data=new_scan_template_values)
         return ScanTemplate.parse_obj(res.json_obj)
 
     def delete(self, scan_template_id: uuid.UUID) -> None:
         """
         Deletes a scan template with provided ID from your account.
 
-        :param scan_template_id: The ID of the scan template to operate against
-        :return None
-        :raises AuthError, ClientError, ServerError
+        :param scan_template_id: The ID of the scan template to delete
+
+        :returns: None
+        :raises: AuthError, ClientError, ServerError
         """
-        self._client.execute("DELETE", f"{self._ENDPOINT}/{str(scan_template_id)}")
+        self._client.execute("DELETE", f"{self._ENDPOINT}/{scan_template_id}")
```

### Comparing `runzero_sdk-0.3.0/runzero/api/custom_integrations.py` & `runzero_sdk-0.4.0/runzero/api/custom_integrations.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,20 @@
         self._client = client
 
     def get_all(self, org_id: uuid.UUID) -> List[CustomIntegration]:
         """
         Lists all custom integrations available to your account.
 
         :param org_id: The ID of the organization to operate against
-        :return: List of custom integrations
-        :raises AuthError, ClientError, ServerError
+
+        :returns: List of custom integrations
+        :raises: AuthError, ClientError, ServerError
         """
 
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         res = self._client.execute("GET", self._ENDPOINT, params=params)
         result: List[CustomIntegration] = []
         for src in res.json_obj:
             result.append(_resp_to_source(src))
         return result
 
     def get(
@@ -46,23 +47,24 @@
     ) -> Optional[CustomIntegration]:
         """
         Retrieves runZero custom integrations with either the matching ID or Name.
 
         :param org_id: The ID of the organization to operate against
         :param name: Optional, name of the organization you want the UUID for
         :param custom_integration_id: Optional, the id of the source to retrieve
-        :raises AuthError, ClientError, ServerError
+
+        :raises: AuthError, ClientError, ServerError
             ValueError if neither custom_integration_id nor name are provided.
-        :return: The matching CustomIntegration or None
+        :returns: The matching CustomIntegration or None
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         if name is None and custom_integration_id is None:
             raise ValueError("must provide custom_integration_id or source name")
         if custom_integration_id is not None:
-            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(custom_integration_id)}", params=params)
+            res = self._client.execute("GET", f"{self._ENDPOINT}/{custom_integration_id}", params=params)
             return _resp_to_source(res.json_obj)
         # name
         for src in self.get_all(org_id):
             if src.name == name:
                 return src
         return None
```

### Comparing `runzero_sdk-0.3.0/runzero/api/explorers.py` & `runzero_sdk-0.4.0/runzero/api/explorers.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 
     def get_all(self, org_id: uuid.UUID) -> List[Explorer]:
         """
         Retrieves all active runZero Explorers available within the given Organization.
 
         :param org_id: The ID of the organization to operate against
 
-        :return: a list of all Explorers available within the given Organization
-        :raises AuthError, ClientError, ServerError
+        :returns: a list of all Explorers available within the given Organization
+        :raises: AuthError, ClientError, ServerError
 
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         res = self._client.execute("GET", self._ENDPOINT, params=params)
         result: List[Explorer] = []
         for explorer in res.json_obj:
             result.append(Explorer.parse_obj(explorer))
         return result
 
     def get(
@@ -57,23 +57,23 @@
         Retrieves the runZero Explorer with the provided name or id, if it is active and exists in the Organization.
 
         :param org_id: The ID of the organization to operate against
         :param name: Optional name of the explorer to retrieve. This is a case-insensitive hostname match.
             If not provided, must provide explorer_id.
         :param explorer_id: Optional id of the explorer to retrieve. If not provided, must provide name.
 
-        :return: explorer requested or None
-        :raises AuthError, ClientError, ServerError,
+        :returns: explorer requested or None
+        :raises: AuthError, ClientError, ServerError,
             ValueError if neither explorer_id nor name are provided.
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         if name is None and explorer_id is None:
             raise ValueError("must provide explorer_id or explorer name")
         if explorer_id is not None:
-            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(explorer_id)}", params=params)
+            res = self._client.execute("GET", f"{self._ENDPOINT}/{explorer_id}", params=params)
             if not res:
                 return None
             return Explorer.parse_obj(res.json_obj)
         for explorer in self.get_all(org_id):
             if explorer.name == name:
                 return explorer
         return None
@@ -83,48 +83,48 @@
         Updates an explorer with given explorer id to the latest explorer software version available.
 
         This will force the explorer to upgrade and restart.
 
         :param org_id: The ID of the organization to operate against
         :param explorer_id: The ID of the explorer to update
 
-        :return None
-        :raises AuthError, ClientError, ServerError
+        :returns: None
+        :raises: AuthError, ClientError, ServerError
         """
-        params = {"_oid": str(org_id)}
-        self._client.execute("POST", f"{self._ENDPOINT}/{str(explorer_id)}/update", params=params)
+        params = {"_oid": org_id}
+        self._client.execute("POST", f"{self._ENDPOINT}/{explorer_id}/update", params=params)
 
     def delete(self, org_id: uuid.UUID, explorer_id: uuid.UUID) -> None:
         """
         Removes and uninstalls an explorer from your Organization.
 
         :param org_id: The ID of the organization to operate against
         :param explorer_id: ID of explorer to delete
 
-        :return None
-        :raises AuthError, ClientError, ServerError
+        :returns: None
+        :raises: AuthError, ClientError, ServerError
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         self._client.execute("DELETE", f"{self._ENDPOINT}/{explorer_id}", params=params)
 
     def move_to_site(self, org_id: uuid.UUID, explorer_id: uuid.UUID, site_id: uuid.UUID) -> Explorer:
         """
         Moves an explorer to a different site.
 
         Explorers moved to a new site will no longer execute tasks defined in the old site,
         and will be available to execute tasks defined in the new site.
 
         :param org_id: The ID of the organization to operate against
         :param explorer_id: ID of explorer to assign to a new site
         :param site_id: ID of the site the explorer will be assigned to
 
-        :return The Explorer with the provided ID, assigned to new site site_id
-        :raises AuthError, ClientError, ServerError
+        :returns: The Explorer with the provided ID, assigned to new site site_id
+        :raises: AuthError, ClientError, ServerError
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         res = self._client.execute(
             "PATCH",
             f"{self._ENDPOINT}/{explorer_id}",
             params=params,
             data=ExplorerSiteID(site_id=site_id),
         )
         return Explorer.parse_obj(res.json_obj)
```

### Comparing `runzero_sdk-0.3.0/runzero/api/hosted_zones.py` & `runzero_sdk-0.4.0/runzero/api/hosted_zones.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,45 +35,45 @@
 
     def get_all(self, org_id: uuid.UUID) -> List[HostedZone]:
         """
         Retrieves all active runZero hosted zones available within the given organization.
 
         :param org_id: The ID of the organization to operate against
 
-        :return: list of HostedZones
-        :raises AuthError, ClientError, ServerError
+        :returns: list of HostedZones
+        :raises: AuthError, ClientError, ServerError
 
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         res = self._client.execute("GET", self._ENDPOINT, params=params)
         result: List[HostedZone] = []
         for hosted_zone in res.json_obj:
             result.append(HostedZone.parse_obj(hosted_zone))
         return result
 
     def get(
         self, org_id: uuid.UUID, name: Optional[str] = None, hosted_zone_id: Optional[uuid.UUID] = None
     ) -> Optional[HostedZone]:
         """
         Retrieves the runZero hosted zone with the provided name or id, if it is active and exists in the Organization.
 
         :param org_id: The ID of the organization to operate against
-
         :param name: Optional name of the hosted zone to retrieve. This is a case-insensitive match.
             If not provided, must provide hosted_zone_id.
         :param hosted_zone_id: Optional id of the hosted zone to retrieve. If not provided, must provide name.
-        :return: HostedZone requested or None
-        :raises AuthError, ClientError, ServerError,
+
+        :returns: HostedZone requested or None
+        :raises: AuthError, ClientError, ServerError,
             ValueError if neither hosted_zone_id nor name are provided.
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         if name is None and hosted_zone_id is None:
             raise ValueError("must provide hosted_zone_id or hosted zone name")
         if hosted_zone_id is not None:
-            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(hosted_zone_id)}", params=params)
+            res = self._client.execute("GET", f"{self._ENDPOINT}/{hosted_zone_id}", params=params)
             if not res:
                 return None
             return HostedZone.parse_obj(res.json_obj)
         # name
         for hosted_zone in self.get_all(org_id):
             if hosted_zone.name == name:
                 return hosted_zone
```

### Comparing `runzero_sdk-0.3.0/runzero/api/imports/assets.py` & `runzero_sdk-0.4.0/runzero/api/imports/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
         :param org_id: Organization ID to import these assets into
         :param site_id: ID of the Site to import these asstes into
         :param custom_integration_id: custom integration id for the provided Import Assets
         :param assets: A collection of ImportAssets to upload
         :param task_info: Descriptive information associated with the import
             task to be created. If omitted, a task name is generated for you
 
-        :return Task: The runZero task associated with processing the asset upload
-        :raises ServerError, ClientError, AuthError
+        :returns: Task: The runZero task associated with processing the asset upload
+        :raises: ServerError, ClientError, AuthError
         """
         # create default task_info not supplied
         if task_info is None:
             task_info = ImportTask(name=f"Custom Asset Import {time.time_ns():.0f}", description="py-sdk import")
         else:
             # set defaults if user sets these to empty
             if task_info.name == "":
```

### Comparing `runzero_sdk-0.3.0/runzero/api/scans.py` & `runzero_sdk-0.4.0/runzero/api/scans.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,14 @@
         """
         Starts a scan to bring data into the site using provided options.
 
         :param org_id: The ID of the organization to operate against
         :param scan_options: ScanOptions describing the scan to perform on the given site.
         :param site_id: The ID of the site which will have inventory modified by results of the scan.
 
-        :return: Task
-        :raises AuthError, ClientError, ServerError
+        :returns: Task
+        :raises: AuthError, ClientError, ServerError
         """
         res = self._client.execute(
-            "PUT", f"{self._ENDPOINT}/{str(site_id)}/scan", params={"_oid": str(org_id)}, data=scan_options
+            "PUT", f"{self._ENDPOINT}/{site_id}/scan", params={"_oid": org_id}, data=scan_options
         )
         return Task.parse_obj(res.json_obj)
```

### Comparing `runzero_sdk-0.3.0/runzero/api/sites.py` & `runzero_sdk-0.4.0/runzero/api/sites.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,42 +31,42 @@
 
     def get_all(self, org_id: uuid.UUID) -> List[Site]:
         """
         Retrieves all runZero Sites available within the given organization
 
         :param org_id: The ID of the organization to operate against
 
-        :return: a list of all Sites available within the given organization
-        :raises AuthError, ClientError, ServerError
+        :returns: a list of all Sites available within the given organization
+        :raises: AuthError, ClientError, ServerError
 
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         res = self._client.execute("GET", self._ENDPOINT, params=params)
         result: List[Site] = []
         for site in res.json_obj:
             result.append(Site.parse_obj(site))
         return result
 
     def get(self, org_id: uuid.UUID, name: Optional[str] = None, site_id: Optional[uuid.UUID] = None) -> Optional[Site]:
         """
         Retrieves the runZero Site with the provided name or id, if it exists in your account
 
         :param org_id: The ID of the organization to operate against
         :param name: Optional name of the site to retrieve. If not provided, must provide site_id.
         :param site_id: Optional id of the site to retrieve. If not provided, must provide name.
 
-        :return: site requested or None
-        :raises AuthError, ClientError, ServerError,
+        :returns: site requested or None
+        :raises: AuthError, ClientError, ServerError,
             ValueError if neither site_id nor name are provided.
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         if name is None and site_id is None:
             raise ValueError("must provide site_id or site name")
         if site_id is not None:
-            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(site_id)}", params=params)
+            res = self._client.execute("GET", f"{self._ENDPOINT}/{site_id}", params=params)
             if not res:
                 return None
             site_obj = res.json_obj
             data_obj = site_obj.get("data", "")
             if data_obj:
                 site_obj = data_obj
 
@@ -80,47 +80,47 @@
     def create(self, org_id: uuid.UUID, site_options: SiteOptions) -> Optional[Site]:
         """
         Creates a new site in the given org.
 
         :param org_id: The ID of the organization to operate against
         :param site_options: Description of site to create
 
-        :return Site created or None
-        :raises AuthError, ClientError, ServerError
+        :returns: Site created or None
+        :raises: AuthError, ClientError, ServerError
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         res = self._client.execute("PUT", self._ENDPOINT, params=params, data=site_options)
         site_data = res.json_obj.get("data", "")
         if site_data:
             return self.get(org_id=org_id, name=site_options.name)
         return Site.parse_obj(res.json_obj)
 
     def update(self, org_id: uuid.UUID, site_id: uuid.UUID, site_options: SiteOptions) -> Optional[Site]:
         """
         Updates a site associated with your organization.
 
         :param org_id: The ID of the organization to operate against
         :param site_id: The ID of the site to update.
         :param site_options: Site's updated values
 
-        :return Site updated or None
-        :raises AuthError, ClientError, ServerError
+        :returns: Site updated or None
+        :raises: AuthError, ClientError, ServerError
         """
-        params = {"_oid": str(org_id)}
-        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{str(site_id)}", params=params, data=site_options)
+        params = {"_oid": org_id}
+        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{site_id}", params=params, data=site_options)
         site_data = res.json_obj.get("data", "")
         if site_data:
             return self.get(org_id=org_id, name=site_options.name)
         return Site.parse_obj(res.json_obj)
 
     def delete(self, org_id: uuid.UUID, site_id: uuid.UUID) -> None:
         """
         Deletes a site from your account.
 
         :param org_id: The ID of the organization to operate against
         :param site_id: Custom asset site id to delete
 
-        :return None
-        :raises AuthError, ClientError, ServerError
+        :returns: None
+        :raises: AuthError, ClientError, ServerError
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         self._client.execute("DELETE", f"{self._ENDPOINT}/{site_id}", params=params)
```

### Comparing `runzero_sdk-0.3.0/runzero/api/tasks.py` & `runzero_sdk-0.4.0/runzero/api/tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Management of runZero tasks.
 """
 import uuid
-from typing import List, Optional
+from typing import Dict, List, Optional, Union
 
 from runzero.client import Client
 from runzero.types import Task, TaskOptions
 
 
 class Tasks:
     """Management of runZero tasks.
@@ -26,17 +26,17 @@
         Retrieves all runZero Tasks available within the given Organization
 
         :param org_id: The unique ID of the organization to retrieve the tasks from.
         :param status: An optional status value to filter tasks by. This is a
             case-insensitive string match, stripped of surrounding whitespace.
         :param query: An optional query to filter returned tasks.
             Query string format is the same as in-UI search. See https://www.runzero.com/docs/search-query-tasks/
-        :return: A list of all tasks
+        :returns: A list of all tasks
         """
-        params = {"_oid": str(org_id)}
+        params: Dict[str, Union[str, uuid.UUID]] = {"_oid": org_id}
         if query is not None:
             params["search"] = query.strip()
         if status is not None:
             params["status"] = status.strip()
         res = self._client.execute("GET", self._ENDPOINT, params=params)
         result: List[Task] = []
         for obj in res.json_obj:
@@ -44,56 +44,86 @@
             result.append(task)
         return result
 
     def get(self, org_id: uuid.UUID, name: Optional[str] = None, task_id: Optional[uuid.UUID] = None) -> Optional[Task]:
         """
         Retrieves the runZero Task with the provided name or id, if it exists in your organization.
 
-        :param org_id: ID of the organization the requested Task is in
+        :param org_id: ID of the organization the requested task is in
         :param name: Optional name of the task to retrieve. If not provided, must provide task_id.
         :param task_id: Optional id of the task to retrieve. If not provided, must provide name.
 
-        :raises AuthError, ClientError, ServerError
+        :raises: AuthError, ClientError, ServerError
             ValueError if neither task_id nor name are provided.
         """
-        params = {"_oid": str(org_id)}
+        params = {"_oid": org_id}
         if name is None and task_id is None:
             raise ValueError("must provide either task_id or task name")
         if task_id is not None:
-            res = self._client.execute("GET", f"{self._ENDPOINT}/{str(task_id)}", params=params)
+            res = self._client.execute("GET", f"{self._ENDPOINT}/{task_id}", params=params)
             return Task.parse_obj(res.json_obj)
         # name
         for task in self.get_all(org_id):
             if task.name == name:
                 return task
         return None
 
     def get_status(self, org_id: uuid.UUID, task_id: uuid.UUID) -> Optional[str]:
         """
         Retrieves the status of a runZero Task with the provided id, if it exists in your organization.
 
         The org_id should be provided if using an Account level api key.
 
+        :param org_id: ID of the organization the requested task is in
         :param task_id: ID of the task you want the status for
-        :param org_id: ID of the organization the requested Task is in. This is
-            necessary if you use an Auth token.
-        :return: a string result indicating task status, or None
+        :returns: a string result indicating task status, or None
         """
-        params = {"_oid": str(org_id)}
-        res = self._client.execute("GET", f"{self._ENDPOINT}/{str(task_id)}", params=params)
+        params = {"_oid": org_id}
+        res = self._client.execute("GET", f"{self._ENDPOINT}/{task_id}", params=params)
         task = Task.parse_obj(res.json_obj)
         if task is None:
             return None
         return task.status
 
     def update(self, org_id: uuid.UUID, task_id: uuid.UUID, task_options: TaskOptions) -> Task:
         """
         Updates task parameters with provided task options values.
 
-        :param task_id: task to modify
+        :param org_id: ID of the organization the requested task is in
+        :param task_id: ID of task to modify
         :param task_options: task values to update
-        :return Task which has been updated
-        :raises AuthError, ClientError, ServerError
+
+        :returns: Task which has been updated
+        :raises: AuthError, ClientError, ServerError
+        """
+        params = {"_oid": org_id}
+        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{task_id}", data=task_options, params=params)
+        return Task.parse_obj(res.json_obj)
+
+    def stop(self, org_id: uuid.UUID, task_id: uuid.UUID) -> Task:
+        """
+        Signals an explorer to stop a currently running task, or signals server to remove
+        a future or recurring task.
+
+        :param org_id: ID of the organization the requested task is in
+        :param task_id: ID of task to stop, or scheduled task to remove from schedule.
+
+        :returns: Task which has been signalled to stop
+        :raises: AuthError, ClientError, ServerError
+        """
+        params = {"_oid": org_id}
+        res = self._client.execute("POST", f"{self._ENDPOINT}/{task_id}/stop", params=params)
+        return Task.parse_obj(res.json_obj)
+
+    def hide(self, org_id: uuid.UUID, task_id: uuid.UUID) -> Task:
+        """
+        Signal that a completed task should be hidden.
+
+        :param org_id: ID of the organization the requested task is in
+        :param task_id: task to modify
+
+        :returns: Completed task which has been hidden
+        :raises: AuthError, ClientError, ServerError
         """
-        params = {"_oid": str(org_id)}
-        res = self._client.execute("PATCH", f"{self._ENDPOINT}/{str(task_id)}", data=task_options, params=params)
+        params = {"_oid": org_id}
+        res = self._client.execute("POST", f"{self._ENDPOINT}/{task_id}/hide", params=params)
         return Task.parse_obj(res.json_obj)
```

### Comparing `runzero_sdk-0.3.0/runzero/client/_http/auth.py` & `runzero_sdk-0.4.0/runzero/client/_http/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 
     created_at: datetime = datetime.now()
 
     def is_expired(self) -> bool:
         """
         Determines if the oauth token is expired or will expire within a minute
 
-        :return: Returns a bool of whether the token is expired or about to
-        :rtype bool
+        :returns: Returns a bool of whether the token is expired or about to
         """
         delta = self.created_at - datetime.now()
         return not delta.total_seconds() <= (self.expires_in + 60)
 
 
 class BearerToken(AuthBase):
     """Implements bearer token authentication scheme"""
@@ -39,16 +38,16 @@
         self._token: str = token
 
     def __call__(self, r: requests.PreparedRequest) -> requests.PreparedRequest:
         """
         Attaches the bearer token to the request headers
 
         :param r: the calling requests object - which is a requests.PreparedRequest
-        :return the calling object
-        :rtype requests.PreparedRequest
+
+        :returns: the calling object
         """
         r.headers["Authorization"] = f"Bearer {self._token}"
         return r
 
 
 class RegisteredAPIClient(AuthBase):
     """Handles the runZero API client registration to retrieve a bearer token"""
@@ -58,22 +57,20 @@
         self._client_secret: str = client_secret
 
     def __call__(self, r: requests.PreparedRequest) -> requests.PreparedRequest:
         """
         Attach appropriate headers to the request for api client registration
 
         :param r: the calling requests object - which is a requests.PreparedRequest
-        :return the calling object
-        :rtype requests.PreparedRequest
+        :returns: the calling object
         """
         r.headers["Content-Type"] = "application/x-www-form-urlencoded"
         return r
 
     def register(self) -> Dict[str, str]:
         """
         Uses the provided OAuth credentials to construct the url for requesting the OAuth bearer token.
 
-        :return dict containing the required components to be urlencoded for OAuth authentication
-        :rtype dict
+        :returns: dict containing the required components to be urlencoded for OAuth authentication
         """
 
         return {"grant_type": "client_credentials", "client_id": self._client_id, "client_secret": self._client_secret}
```

### Comparing `runzero_sdk-0.3.0/runzero/client/_http/io.py` & `runzero_sdk-0.4.0/runzero/client/_http/io.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/runzero/client/client.py` & `runzero_sdk-0.4.0/runzero/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,28 +109,28 @@
     def oauth_token_is_expired(self) -> bool:
         """Returns true if the oauth token is no longer valid.
 
         Note that the token is automatically refreshed for you when
         possible. This value doesn't need to be checked and manually
         refreshed in most cases.
 
-        :return bool: indicating whether the oauth token is expired.
+        :returns: bool: indicating whether the oauth token is expired.
              If OAuth is not in-use with the client, value is always false.
         """
         if self.__token:
             return self.__token.is_expired()
         return False
 
     @property
     def oauth_active(self) -> bool:
         """
          Returns true if the OAuth is in use.
              This happens when register_api_client was called successfully
 
-        :return bool: indicating whether the oauth token is expired.
+        :returns: bool: indicating whether the oauth token is expired.
              If there is no oauth used with the client, value is always false.
         """
         return self._use_token
 
     def oauth_login(self, client_id: str, client_secret: str) -> None:
         """
         Registers the runZero SDK client using OAuth credentials, and
@@ -138,35 +138,36 @@
 
         To obtain a client ID and client secret, see the API Clients area
         of the product. Generation of these values is restricted to account
         administrators.
 
         :param client_id: The client ID for the runZero registered API client
         :param client_secret: The client secret for the runZero registered API client
-        :raise AuthError: Exception for invalid OAuth configurations
+
+        :raises: AuthError: Exception for invalid OAuth configurations
         """
         self.__client_id = client_id
         self.__client_secret = client_secret
         self._use_token = True
         return self._login()
 
     @property
     def url(self) -> str:
         """The url of the server
 
-        :return: str: The URL of the runZero server
+        :returns: str: The URL of the runZero server
         """
         return self.server_url
 
     # This is only used if the auth type is a registered api client
     def _login(self) -> None:
         """
         Attempts to use the client secret and client id to generate an OAuth token.
 
-        :raise AuthError
+        :raises: AuthError
         """
         if not self._use_token or (self.__client_id is None or self.__client_secret is None):
             raise AuthError("invalid auth configuration")
         try:
             resp = requests.post(
                 f"{self.server_url}/{self._Paths.TOKEN.value}",
                 data=RegisteredAPIClient(self.__client_id, self.__client_secret).register(),
@@ -187,17 +188,18 @@
     def _get_auth_token(self, scope: _AuthScope) -> str:
         """
         Validates and resolves the bearer token to use depending on the provided API scope.
 
         Will also refresh the OAuth token if it's about to expire.
 
         :param scope: Authentication scope for the requested credential to resolve
-        :return: Bearer token for the required API scope
+        :returns: Bearer token for the required API scope
         :rtype string
-        :raise AuthError
+
+        :raises: AuthError
         """
         self._validate_scope_permissions(scope)
 
         if self._use_token:
             if self.__token is not None:
                 # this handles refreshing the token if necessary
                 if self.__token.is_expired():
@@ -228,31 +230,34 @@
                     raise AuthError("missing organization or account key")
             return
 
     @property
     def last_rate_limit_information(self) -> Optional[RateLimitInformation]:
         """
         The last rate limit information retrieved from the server.
-        :return: Optional[RateLimitInformation]
+
+        :returns: Rate limit information when provided.
         """
         return self._rate_limit_information
 
     @property
     def timeout(self) -> int:
         """
         The set request timeout value in seconds
-        :return: int
+
+        :returns: timeout in seconds
         """
         return self._timeout
 
     @property
     def validate_cert(self) -> bool:
         """
         Boolean indicating whether the https cert must valid before proceeding.
-        :return: bool
+
+        :returns: true if certficate information is validated, false if not
         """
         return self._validate_cert
 
     def execute(
         self,
         method: str,
         endpoint: str,
@@ -265,16 +270,17 @@
 
         :param method: The REST verb to use
         :param endpoint: The path to execute against
         :param params: URL query parameters
         :param data: The data to send in form body (POST, PATCH, PUT)
         :param files: For multipart form data or file uploads. Format varies.
         :param multipart: True if using a multipart form data (combination file[s] and form data)
-        :return: The result of the execution as class:.`Response`
-        :raises ValidationError, ConnTimeoutError, ConnError, CommunicationError
+
+        :returns: The result of the execution as class:.`Response`
+        :raises: ValidationError, ConnTimeoutError, ConnError, CommunicationError
         """
         token: str = ""
         try:
             token = self._get_auth_token(self._AuthScope.ACCOUNT)
         except AuthError:
             pass
 
@@ -292,10 +298,8 @@
             timeout=self.timeout,
             validate_certificate=self.validate_cert,
             data=form_data,
             files=files,
             multipart=multipart,
         ).execute()
         self._rate_limit_information = resp.rate_limit_information
-        # If the result doesn't have JSON decoded, it's not a valid result.
-        # TODO: Decide if absolutely anything else else should be a raised error here
         return resp
```

### Comparing `runzero_sdk-0.3.0/runzero/client/errors.py` & `runzero_sdk-0.4.0/runzero/client/errors.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/runzero/errors.py` & `runzero_sdk-0.4.0/runzero/errors.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/runzero/types/__init__.py` & `runzero_sdk-0.4.0/runzero/types/__init__.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/runzero/types/_data_models_gen.py` & `runzero_sdk-0.4.0/runzero/types/_data_models_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  proposed-runzero-api.yml
-#   timestamp: 2023-04-24T21:50:18+00:00
+#   timestamp: 2023-04-28T22:36:38+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from ipaddress import IPv4Address, IPv6Address
 from typing import Any, Dict, List, Optional
@@ -135,18 +135,14 @@
     """
     custom_integration_id: UUID = Field(
         ..., alias="customIntegrationId", example="e77602e0-3fb8-4734-aef9-fbc6fdcb0fa8"
     )
     """
     The unique ID of the registered custom integration which produced the asset data. Uniqueness is not checked/enforced. See /account/custom-integrations api.
     """
-    run_zero_id: Optional[UUID] = Field(None, alias="runZeroId", example="e77602e0-3fb8-4734-aef9-fbc6fdcb0fa8")
-    """
-    The unique ID of the runZero asset to force a merge onto. It is not necessary to provide this data, merging will work according to typical runZero merge rules otherwise.
-    """
     import_task: ImportTask = Field(..., alias="importTask", title="ImportTask")
     """
     Information which describes the task created when asset data is imported.
     """
     asset_data: bytes = Field(..., alias="assetData")
     """
     A gzip (not .tar.gz) compressed file containing ImportAsset objects. The file data may be a JSON array of
```

### Comparing `runzero_sdk-0.3.0/runzero/types/_rate_limit_information.py` & `runzero_sdk-0.4.0/runzero/types/_rate_limit_information.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/runzero/types/_wrapped.py` & `runzero_sdk-0.4.0/runzero/types/_wrapped.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/runzero/types/errors.py` & `runzero_sdk-0.4.0/runzero/types/errors.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.3.0/PKG-INFO` & `runzero_sdk-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runzero-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: The runZero platform sdk
 Home-page: https://runzero.com/
 License: BSD-2-Clause
 Keywords: runzero,api,sdk
 Author: runZero
 Author-email: support@runzero.com
 Requires-Python: >=3.8,<4.0
```

