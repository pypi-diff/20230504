# Comparing `tmp/gwdc_python-0.5.0.tar.gz` & `tmp/gwdc_python-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdc_python-0.5.0.tar", max compression
+gzip compressed data, was "gwdc_python-0.5.1.tar", max compression
```

## Comparing `gwdc_python-0.5.0.tar` & `gwdc_python-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1076 2021-07-19 20:27:11.070554 gwdc_python-0.5.0/LICENSE
--rw-r--r--   0        0        0      195 2021-07-19 20:27:11.070554 gwdc_python-0.5.0/README.rst
--rw-r--r--   0        0        0       67 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/__init__.py
--rw-r--r--   0        0        0     1091 2022-08-09 17:58:23.302425 gwdc_python-0.5.0/gwdc_python/exceptions.py
--rw-r--r--   0        0        0       61 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/__init__.py
--rw-r--r--   0        0        0     3980 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/file_reference.py
--rw-r--r--   0        0        0     2598 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/filters.py
--rw-r--r--   0        0        0      659 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/identifiers.py
--rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/tests/__init__.py
--rw-r--r--   0        0        0     4897 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/tests/test_file_reference.py
--rw-r--r--   0        0        0     4444 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/tests/test_filters.py
--rw-r--r--   0        0        0     3296 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/files/tests/test_identifiers.py
--rw-r--r--   0        0        0     4485 2023-04-26 01:47:22.282014 gwdc_python-0.5.0/gwdc_python/gwdc.py
--rw-r--r--   0        0        0      541 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/helpers.py
--rw-r--r--   0        0        0       26 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/__init__.py
--rw-r--r--   0        0        0     1421 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/base.py
--rw-r--r--   0        0        0     3298 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/meta.py
--rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/tests/__init__.py
--rw-r--r--   0        0        0      789 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/tests/test_base.py
--rw-r--r--   0        0        0      830 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/jobs/tests/test_meta.py
--rw-r--r--   0        0        0      227 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/logger.py
--rw-r--r--   0        0        0        0 2021-06-30 01:51:45.372719 gwdc_python-0.5.0/gwdc_python/tests/__init__.py
--rw-r--r--   0        0        0     5269 2023-04-26 01:46:57.208773 gwdc_python-0.5.0/gwdc_python/tests/test_gwdc_python.py
--rw-r--r--   0        0        0      112 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/tests/__init__.py
--rw-r--r--   0        0        0     2244 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/tests/test_utils.py
--rw-r--r--   0        0        0     1337 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/typed_list.py
--rw-r--r--   0        0        0     2709 2022-06-17 01:28:34.516404 gwdc_python-0.5.0/gwdc_python/utils/utils.py
--rw-r--r--   0        0        0      879 2023-04-26 02:44:46.210050 gwdc_python-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 gwdc_python-0.5.0/setup.py
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 gwdc_python-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2021-07-19 20:27:11.070554 gwdc_python-0.5.1/LICENSE
+-rw-r--r--   0        0        0      195 2021-07-19 20:27:11.070554 gwdc_python-0.5.1/README.rst
+-rw-r--r--   0        0        0       67 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-04 01:13:40.935287 gwdc_python-0.5.1/gwdc_python/constants.py
+-rw-r--r--   0        0        0     1091 2022-08-09 17:58:23.302425 gwdc_python-0.5.1/gwdc_python/exceptions.py
+-rw-r--r--   0        0        0       61 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/__init__.py
+-rw-r--r--   0        0        0     3980 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/file_reference.py
+-rw-r--r--   0        0        0     2598 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/filters.py
+-rw-r--r--   0        0        0      659 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/identifiers.py
+-rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/tests/__init__.py
+-rw-r--r--   0        0        0     4897 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/tests/test_file_reference.py
+-rw-r--r--   0        0        0     4444 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/tests/test_filters.py
+-rw-r--r--   0        0        0     3296 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/files/tests/test_identifiers.py
+-rw-r--r--   0        0        0     5626 2023-05-04 01:13:40.935287 gwdc_python-0.5.1/gwdc_python/gwdc.py
+-rw-r--r--   0        0        0      541 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/helpers.py
+-rw-r--r--   0        0        0       26 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/__init__.py
+-rw-r--r--   0        0        0     1421 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/base.py
+-rw-r--r--   0        0        0     3298 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/meta.py
+-rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/tests/__init__.py
+-rw-r--r--   0        0        0      789 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/tests/test_base.py
+-rw-r--r--   0        0        0      830 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/jobs/tests/test_meta.py
+-rw-r--r--   0        0        0      227 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/logger.py
+-rw-r--r--   0        0        0        0 2021-06-30 01:51:45.372719 gwdc_python-0.5.1/gwdc_python/tests/__init__.py
+-rw-r--r--   0        0        0     5422 2023-05-04 01:13:40.935287 gwdc_python-0.5.1/gwdc_python/tests/test_gwdc_python.py
+-rw-r--r--   0        0        0      112 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/tests/__init__.py
+-rw-r--r--   0        0        0     2244 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/tests/test_utils.py
+-rw-r--r--   0        0        0     1337 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/typed_list.py
+-rw-r--r--   0        0        0     2709 2022-06-17 01:28:34.516404 gwdc_python-0.5.1/gwdc_python/utils/utils.py
+-rw-r--r--   0        0        0      898 2023-05-04 01:13:40.935287 gwdc_python-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 gwdc_python-0.5.1/setup.py
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 gwdc_python-0.5.1/PKG-INFO
```

### Comparing `gwdc_python-0.5.0/LICENSE` & `gwdc_python-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/exceptions.py` & `gwdc_python-0.5.1/gwdc_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/files/file_reference.py` & `gwdc_python-0.5.1/gwdc_python/files/file_reference.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/files/filters.py` & `gwdc_python-0.5.1/gwdc_python/files/filters.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/files/identifiers.py` & `gwdc_python-0.5.1/gwdc_python/files/identifiers.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/files/tests/test_file_reference.py` & `gwdc_python-0.5.1/gwdc_python/files/tests/test_file_reference.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/files/tests/test_filters.py` & `gwdc_python-0.5.1/gwdc_python/files/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/files/tests/test_identifiers.py` & `gwdc_python-0.5.1/gwdc_python/files/tests/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/gwdc.py` & `gwdc_python-0.5.1/gwdc_python/gwdc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,63 @@
 import json
+from pathlib import Path
+from uuid import uuid4
+
 import requests
+from appdirs import user_config_dir
+from humps import camelize, decamelize
 from requests_toolbelt.multipart.encoder import MultipartEncoder, MultipartEncoderMonitor
 from tqdm import tqdm
-from humps import camelize, decamelize
 
+from .constants import APP_NAME, ORGANISATION
 from .exceptions import GWDCRequestException, handle_request_errors
-from .utils import split_variables_dict
 from .logger import create_logger
+from .utils import split_variables_dict
 
 logger = create_logger(__name__)
 
 
 class GWDC:
     def __init__(self, token, auth_endpoint, endpoint, custom_error_handler=None):
         self.api_token = token
         self.auth_endpoint = auth_endpoint
         self.endpoint = endpoint
         if custom_error_handler:
             self._apply_custom_error_handler(custom_error_handler)
 
         if self.api_token:
             self._obtain_access_token()
+        else:
+            self.public_id = self._obtain_public_id()
+            self.session_id = self._obtain_session_id()
+
+    def _obtain_session_id(self):
+        return str(uuid4())
+
+    def _obtain_public_id(self):
+        config_file = Path(user_config_dir(APP_NAME, ORGANISATION)) / 'config.json'
+
+        def write_new_config():
+            uuid = str(uuid4())
+
+            config = {
+                'public_id': uuid
+            }
+
+            config_file.parent.mkdir(parents=True, exist_ok=True)
+            config_file.write_text(json.dumps(config))
+
+        if not config_file.exists():
+            write_new_config()
+
+        try:
+            return json.loads(config_file.read_text())['public_id']
+        except Exception:
+            write_new_config()
+            return json.loads(config_file.read_text())['public_id']
 
     def _apply_custom_error_handler(self, custom_error_handler):
         self._obtain_access_token = custom_error_handler(self._obtain_access_token)
         self._refresh_access_token = custom_error_handler(self._refresh_access_token)
         self.request = custom_error_handler(self.request)
 
     def _request(self, endpoint, query, variables=None, headers=None, method="POST"):
@@ -120,12 +153,18 @@
         )
         self.jwt_token = data["refresh_token"]["token"]
         self.refresh_token = data["refresh_token"]["refresh_token"]
 
     @handle_request_errors
     def request(self, query, variables=None, headers=None, authorize=True):
 
-        all_headers = {'Authorization': 'JWT ' + self.jwt_token} if authorize and self.api_token else {}
+        all_headers = {}
+        if authorize:
+            if self.api_token:
+                all_headers = {'Authorization': 'JWT ' + self.jwt_token}
+            elif self.public_id:
+                all_headers = {'X-Correlation-ID': f"{self.public_id} {self.session_id}"}
+
         if headers is not None:
             all_headers = {**all_headers, **headers}
 
         return self._request(endpoint=self.endpoint, query=query, variables=variables, headers=all_headers)
```

### Comparing `gwdc_python-0.5.0/gwdc_python/helpers.py` & `gwdc_python-0.5.1/gwdc_python/helpers.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/jobs/base.py` & `gwdc_python-0.5.1/gwdc_python/jobs/base.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/jobs/meta.py` & `gwdc_python-0.5.1/gwdc_python/jobs/meta.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/jobs/tests/test_base.py` & `gwdc_python-0.5.1/gwdc_python/jobs/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/jobs/tests/test_meta.py` & `gwdc_python-0.5.1/gwdc_python/jobs/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/tests/test_gwdc_python.py` & `gwdc_python-0.5.1/gwdc_python/tests/test_gwdc_python.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,14 +112,15 @@
     )
     assert gwdc.jwt_token == "mock_jwt_token_new"
     assert gwdc.refresh_token == "mock_refresh_token_new"
     assert response["test_response"] == "mock_response"
 
     # Authorization should have been provided in the headers
     assert "Authorization" in requests_mock.request_history[-1].headers
+    assert "X-Correlation-ID" not in requests_mock.request_history[-1].headers
 
 
 # Test that GWDC will allow the custom error handler to intercept raised errors
 def test_gwdc_custom_error_handling_token(setup_gwdc):
     class TestException(Exception):
         pass
 
@@ -168,7 +169,8 @@
         """
     )
 
     assert response["test_response"] == "mock_response"
 
     # Authorization should not have been provided in the headers
     assert "Authorization" not in requests_mock.request_history[0].headers
+    assert "X-Correlation-ID" in requests_mock.request_history[0].headers
```

### Comparing `gwdc_python-0.5.0/gwdc_python/utils/tests/test_utils.py` & `gwdc_python-0.5.1/gwdc_python/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/utils/typed_list.py` & `gwdc_python-0.5.1/gwdc_python/utils/typed_list.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/gwdc_python/utils/utils.py` & `gwdc_python-0.5.1/gwdc_python/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gwdc_python-0.5.0/pyproject.toml` & `gwdc_python-0.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwdc-python"
-version = "0.5.0"
+version = "0.5.1"
 description = "API for GWDC modules"
 authors = ["Thomas Reichardt <treichardt@swin.edu.au>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/gravitationalwavedc/gwdc_python"
 include = ["LICENSE",]
 
@@ -14,14 +14,15 @@
 jwt = "^1.2.0"
 requests-toolbelt = "^0.9.1"
 tqdm = "^4.61.2"
 importlib-metadata = "^4.5.0"
 Sphinx = {version = "^4.0.2", optional = true}
 sphinx-rtd-theme = {version = "^0.5.2", optional = true}
 pyhumps = "^3.7.1"
+appdirs = "^1.4.4"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-rtd-theme"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3"
 requests-mock = "^1.8.0"
```

### Comparing `gwdc_python-0.5.0/setup.py` & `gwdc_python-0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,28 @@
  'gwdc_python.utils',
  'gwdc_python.utils.tests']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['importlib-metadata>=4.5.0,<5.0.0',
+['appdirs>=1.4.4,<2.0.0',
+ 'importlib-metadata>=4.5.0,<5.0.0',
  'jwt>=1.2.0,<2.0.0',
  'pyhumps>=3.7.1,<4.0.0',
  'requests-toolbelt>=0.9.1,<0.10.0',
  'requests>=2.25.1,<3.0.0',
  'tqdm>=4.61.2,<5.0.0']
 
 extras_require = \
 {'docs': ['Sphinx>=4.0.2,<5.0.0', 'sphinx-rtd-theme>=0.5.2,<0.6.0']}
 
 setup_kwargs = {
     'name': 'gwdc-python',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'API for GWDC modules',
     'long_description': 'GWDC Python API\n===============\n\nThis package handles requests for the GWDC modules. Presently, it primarily handles the requests for `gwcloud-python <https://pypi.org/project/gwcloud-python/>`_.',
     'author': 'Thomas Reichardt',
     'author_email': 'treichardt@swin.edu.au',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/gravitationalwavedc/gwdc_python',
```

### Comparing `gwdc_python-0.5.0/PKG-INFO` & `gwdc_python-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdc-python
-Version: 0.5.0
+Version: 0.5.1
 Summary: API for GWDC modules
 Home-page: https://github.com/gravitationalwavedc/gwdc_python
 License: MIT
 Author: Thomas Reichardt
 Author-email: treichardt@swin.edu.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=4.0.2,<5.0.0) ; extra == "docs"
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.5.0,<5.0.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: pyhumps (>=3.7.1,<4.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
 Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
 Requires-Dist: tqdm (>=4.61.2,<5.0.0)
```

