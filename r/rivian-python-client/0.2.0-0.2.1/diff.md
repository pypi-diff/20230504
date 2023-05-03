# Comparing `tmp/rivian-python-client-0.2.0.tar.gz` & `tmp/rivian-python-client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivian-python-client-0.2.0.tar", max compression
+gzip compressed data, was "rivian-python-client-0.2.1.tar", max compression
```

## Comparing `rivian-python-client-0.2.0.tar` & `rivian-python-client-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      325 2023-04-26 14:26:04.905314 rivian-python-client-0.2.0/README.md
--rw-r--r--   0        0        0      555 2023-04-26 14:26:04.905314 rivian-python-client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      102 2023-04-26 14:26:04.905314 rivian-python-client-0.2.0/src/rivian/__init__.py
--rw-r--r--   0        0        0     2888 2023-04-26 14:26:04.909314 rivian-python-client-0.2.0/src/rivian/const.py
--rw-r--r--   0        0        0      779 2023-04-26 14:26:04.909314 rivian-python-client-0.2.0/src/rivian/exceptions.py
--rw-r--r--   0        0        0    24357 2023-04-26 14:26:04.909314 rivian-python-client-0.2.0/src/rivian/rivian.py
--rw-r--r--   0        0        0     6962 2023-04-26 14:26:04.909314 rivian-python-client-0.2.0/src/rivian/ws_monitor.py
--rw-r--r--   0        0        0     1045 2023-04-26 14:26:36.278962 rivian-python-client-0.2.0/setup.py
--rw-r--r--   0        0        0      832 2023-04-26 14:26:36.279379 rivian-python-client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      325 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/README.md
+-rw-r--r--   0        0        0      555 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/__init__.py
+-rw-r--r--   0        0        0     2888 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/const.py
+-rw-r--r--   0        0        0      779 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/exceptions.py
+-rw-r--r--   0        0        0    23660 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/rivian.py
+-rw-r--r--   0        0        0     6962 2023-05-03 23:40:03.784370 rivian-python-client-0.2.1/src/rivian/ws_monitor.py
+-rw-r--r--   0        0        0     1045 2023-05-03 23:40:26.163903 rivian-python-client-0.2.1/setup.py
+-rw-r--r--   0        0        0      832 2023-05-03 23:40:26.164202 rivian-python-client-0.2.1/PKG-INFO
```

### Comparing `rivian-python-client-0.2.0/pyproject.toml` & `rivian-python-client-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rivian-python-client"
-version = "0.2.0"
+version = "0.2.1"
 description = "Rivian API Client (Unofficial)"
 readme = "README.md"
 authors = ["Brian Retterer <bretterer@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "rivian", from = "src" },
 ]
```

### Comparing `rivian-python-client-0.2.0/src/rivian/const.py` & `rivian-python-client-0.2.1/src/rivian/const.py`

 * *Files identical despite different names*

### Comparing `rivian-python-client-0.2.0/src/rivian/exceptions.py` & `rivian-python-client-0.2.1/src/rivian/exceptions.py`

 * *Files identical despite different names*

### Comparing `rivian-python-client-0.2.0/src/rivian/rivian.py` & `rivian-python-client-0.2.1/src/rivian/rivian.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,18 +80,17 @@
 
     async def authenticate(
         self,
         username: str,
         password: str,
     ) -> ClientResponse | dict[str, str]:
         """Authenticate against the Rivian API with Username and Password"""
-        url = url = AUTH_BASEPATH + "/token/auth"
+        url = AUTH_BASEPATH + "/token/auth"
 
-        headers = {}
-        headers.update(BASE_HEADERS)
+        headers = {**BASE_HEADERS}
 
         json_data = {
             "grant_type": "password",
             "username": username,
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "pwd": password,
@@ -145,23 +144,17 @@
 
     async def validate_otp(
         self,
         username: str,
         otp: str,
     ) -> dict[str, Any]:
         """Validate the OTP"""
-        url = url = AUTH_BASEPATH + "/token/auth"
+        url = AUTH_BASEPATH + "/token/auth"
 
-        headers = dict()
-        headers.update(BASE_HEADERS)
-        headers.update(
-            {
-                "Authorization": "Bearer " + self._session_token,
-            }
-        )
+        headers = BASE_HEADERS | {"Authorization": "Bearer " + self._session_token}
 
         json_data = {
             "grant_type": "password",
             "username": username,
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "otp_token": otp,
@@ -210,18 +203,17 @@
     async def refresh_access_token(
         self,
         refresh_token: str,
         client_id: str,
         client_secret: str,
     ) -> ClientRequest:
         """Validate the OTP"""
-        url = url = AUTH_BASEPATH + "/token/refresh"
+        url = AUTH_BASEPATH + "/token/refresh"
 
-        headers = dict()
-        headers.update(BASE_HEADERS)
+        headers = {**BASE_HEADERS}
 
         json_data = {
             "token": refresh_token,
             "client_id": client_id,
             "client_secret": client_secret,
         }
 
@@ -267,21 +259,15 @@
 
     async def get_vehicle_info(
         self, vin: str, access_token: str, properties: dict[str]
     ) -> dict[str, Any]:
         """get the vehicle info"""
         url = CESIUM_BASEPATH + "/vehicle/latest"
 
-        headers = dict()
-        headers.update(BASE_HEADERS)
-        headers.update(
-            {
-                "Authorization": "Bearer " + access_token,
-            }
-        )
+        headers = BASE_HEADERS | {"Authorization": "Bearer " + access_token}
 
         json_data = {
             "car": vin,
             "properties": properties,
         }
 
         if self._session is None:
@@ -324,20 +310,18 @@
                 headers,
                 json_data,
             )
 
         return response
 
     async def create_csrf_token(self) -> dict[str, Any]:
-        """create cross-site-request-forgery (csrf) token"""
-
+        """Create cross-site-request-forgery (csrf) token."""
         url = GRAPHQL_GATEWAY
 
-        headers = dict()
-        headers.update(BASE_HEADERS)
+        headers = {**BASE_HEADERS}
 
         graphql_json = {
             "operationName": "CreateCSRFToken",
             "query": "mutation CreateCSRFToken {\n  createCsrfToken {\n    __typename\n    csrfToken\n    appSessionToken\n  }\n}",
             "variables": None,
         }
 
@@ -353,27 +337,22 @@
 
     async def authenticate_graphql(
         self,
         username: str,
         password: str,
     ) -> dict[str, Any]:
         """Authenticate against the Rivian GraphQL API with Username and Password"""
-
         url = GRAPHQL_GATEWAY
 
-        headers = {}
-        headers.update(BASE_HEADERS)
-        headers.update(
-            {
-                "Csrf-Token": self._csrf_token,
-                "A-Sess": self._app_session_token,
-                "Apollographql-Client-Name": APOLLO_CLIENT_NAME,
-                "Dc-Cid": f"m-ios-{uuid.uuid4()}",
-            }
-        )
+        headers = BASE_HEADERS | {
+            "Csrf-Token": self._csrf_token,
+            "A-Sess": self._app_session_token,
+            "Apollographql-Client-Name": APOLLO_CLIENT_NAME,
+            "Dc-Cid": f"m-ios-{uuid.uuid4()}",
+        }
 
         graphql_json = {
             "operationName": "Login",
             "query": "mutation Login($email: String!, $password: String!) {\n  login(email: $email, password: $password) {\n    __typename\n    ... on MobileLoginResponse {\n      __typename\n      accessToken\n      refreshToken\n      userSessionToken\n    }\n    ... on MobileMFALoginResponse {\n      __typename\n      otpToken\n    }\n  }\n}",
             "variables": {"email": username, "password": password},
         }
 
@@ -391,26 +370,21 @@
             self._refresh_token = login_data["refreshToken"]
             self._user_session_token = login_data["userSessionToken"]
 
         return response
 
     async def validate_otp_graphql(self, username: str, otpCode: str) -> dict[str, Any]:
         """Validates OTP against the Rivian GraphQL API with Username, OTP Code, and OTP Token"""
-
         url = GRAPHQL_GATEWAY
 
-        headers = dict()
-        headers.update(BASE_HEADERS)
-        headers.update(
-            {
-                "Csrf-Token": self._csrf_token,
-                "A-Sess": self._app_session_token,
-                "Apollographql-Client-Name": APOLLO_CLIENT_NAME,
-            }
-        )
+        headers = BASE_HEADERS | {
+            "Csrf-Token": self._csrf_token,
+            "A-Sess": self._app_session_token,
+            "Apollographql-Client-Name": APOLLO_CLIENT_NAME,
+        }
 
         graphql_json = {
             "operationName": "LoginWithOTP",
             "query": "mutation LoginWithOTP($email: String!, $otpCode: String!, $otpToken: String!) {\n  loginWithOTP(email: $email, otpCode: $otpCode, otpToken: $otpToken) {\n    __typename\n    ... on MobileLoginResponse {\n      __typename\n      accessToken\n      refreshToken\n      userSessionToken\n    }\n  }\n}",
             "variables": {
                 "email": username,
                 "otpCode": otpCode,
@@ -430,59 +404,53 @@
 
         return response
 
     async def get_user_information(self) -> ClientResponse:
         """get user information (user.id, vehicle vins)"""
         url = GRAPHQL_GATEWAY
 
-        headers = dict()
-        headers.update(BASE_HEADERS)
-        headers.update(
-            {"A-Sess": self._app_session_token, "U-Sess": self._user_session_token}
-        )
+        headers = BASE_HEADERS | {
+            "A-Sess": self._app_session_token,
+            "U-Sess": self._user_session_token,
+        }
 
         graphql_json = {
             "operationName": "getUserInfo",
-            "query": "query getUserInfo {\n    currentUser {\n        __typename\n        id\n        vehicles {\n        id\n        vin\n        vas {\n            __typename\n            vasVehicleId\n            vehiclePublicKey\n        }\n        roles\n        state\n        createdAt\n        updatedAt\n        vehicle {\n            __typename\n            id\n            vin\n            modelYear\n            make\n            model\n            expectedBuildDate\n            plannedBuildDate\n            expectedGeneralAssemblyStartDate\n            actualGeneralAssemblyDate\n        }\n        }\n    }\n}",
+            "query": "query getUserInfo {\n    currentUser {\n        __typename\n        id\n        vehicles {\n        id\n        vin\n        name\n        vas {\n            __typename\n            vasVehicleId\n            vehiclePublicKey\n        }\n        roles\n        state\n        createdAt\n        updatedAt\n        vehicle {\n            __typename\n            id\n            vin\n            modelYear\n            make\n            model\n            expectedBuildDate\n            plannedBuildDate\n            expectedGeneralAssemblyStartDate\n            actualGeneralAssemblyDate\n        }\n        }\n    }\n}",
             "variables": None,
         }
 
         return await self.__graphql_query(headers, url, graphql_json)
 
     async def get_registered_wallboxes(self) -> ClientResponse:
         """get wallboxes (graphql)"""
         url = GRAPHQL_CHARGING
 
-        headers = dict()
-        headers.update(BASE_HEADERS)
-        headers.update(
-            {
-                "Csrf-Token": self._csrf_token,
-                "A-Sess": self._app_session_token,
-                "U-Sess": self._user_session_token,
-            }
-        )
+        headers = BASE_HEADERS | {
+            "Csrf-Token": self._csrf_token,
+            "A-Sess": self._app_session_token,
+            "U-Sess": self._user_session_token,
+        }
 
         graphql_json = {
             "operationName": "getRegisteredWallboxes",
             "query": "query getRegisteredWallboxes {\n  getRegisteredWallboxes {\n    __typename\n    wallboxId\n    userId\n    wifiId\n    name\n    linked\n    latitude\n    longitude\n    chargingStatus\n    power\n    currentVoltage\n    currentAmps\n    softwareVersion\n    model\n    serialNumber\n    maxAmps\n    maxVoltage\n    maxPower\n  }\n}",
             "variables": None,
         }
 
         return await self.__graphql_query(headers, url, graphql_json)
 
     async def get_vehicle_state(self, vin: str, properties: set[str]) -> ClientResponse:
         """get vehicle state (graphql)"""
         url = GRAPHQL_GATEWAY
 
-        headers = {}
-        headers.update(BASE_HEADERS)
-        headers.update(
-            {"A-Sess": self._app_session_token, "U-Sess": self._user_session_token}
-        )
+        headers = BASE_HEADERS | {
+            "A-Sess": self._app_session_token,
+            "U-Sess": self._user_session_token,
+        }
 
         graphql_query = "query GetVehicleState($vehicleID: String!) {\n  vehicleState(id: $vehicleID) "
         graphql_query += self._build_vehicle_state_fragment(properties)
         graphql_query += "}"
 
         graphql_json = {
             "operationName": "GetVehicleState",
@@ -494,17 +462,15 @@
 
     async def get_live_charging_session(
         self, user_id: str, vin: str, properties: dict[str]
     ) -> ClientResponse:
         """get live charging session data (graphql)"""
         url = GRAPHQL_CHARGING
 
-        headers = dict()
-        headers.update(BASE_HEADERS)
-        headers.update({"U-Sess": self._user_session_token})
+        headers = BASE_HEADERS | {"U-Sess": self._user_session_token}
 
         graphql_query = "query getLiveSessionData($vehicleId: ID!) {\n  getLiveSessionData(vehicleId: $vehicleId) {\n    __typename\n   "
         detail_sensors = [
             "vehicleChargerState",
             "timeRemaining",
             "kilometersChargedPerHour",
             "power",
```

### Comparing `rivian-python-client-0.2.0/src/rivian/ws_monitor.py` & `rivian-python-client-0.2.1/src/rivian/ws_monitor.py`

 * *Files identical despite different names*

### Comparing `rivian-python-client-0.2.0/setup.py` & `rivian-python-client-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0.0', 'yarl>=1.6.0']
 
 setup_kwargs = {
     'name': 'rivian-python-client',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Rivian API Client (Unofficial)',
     'long_description': '# Python: Rivian API Client\n\nCurrently a Work In Progress\n\n## Dependencies\n\n[Poetry](https://python-poetry.org/docs/)\n\n```\ncurl -sSL https://install.python-poetry.org | python3 -\n```\n\n## Setup\n\nInstall project dependencies into the poetry virtual environment.\n\n```\npoetry install\n```\n\n## Run Tests\n\n```\npoetry run pytest\n```\n',
     'author': 'Brian Retterer',
     'author_email': 'bretterer@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `rivian-python-client-0.2.0/PKG-INFO` & `rivian-python-client-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivian-python-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Rivian API Client (Unofficial)
 License: MIT
 Author: Brian Retterer
 Author-email: bretterer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

