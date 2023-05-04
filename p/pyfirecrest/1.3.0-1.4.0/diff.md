# Comparing `tmp/pyfirecrest-1.3.0.tar.gz` & `tmp/pyfirecrest-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirecrest-1.3.0.tar", max compression
+gzip compressed data, was "pyfirecrest-1.4.0.tar", last modified: Thu May  4 12:18:39 2023, max compression
```

## Comparing `pyfirecrest-1.3.0.tar` & `pyfirecrest-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,32 @@
--rw-r--r--   0        0        0     1515 2023-01-24 15:42:22.197508 pyfirecrest-1.3.0/LICENSE
--rw-r--r--   0        0        0     1723 2023-01-24 15:42:22.197508 pyfirecrest-1.3.0/README.md
--rw-r--r--   0        0        0     3153 2023-01-24 15:42:22.201508 pyfirecrest-1.3.0/firecrest/Authorization.py
--rw-r--r--   0        0        0    53340 2023-01-24 15:42:22.201508 pyfirecrest-1.3.0/firecrest/BasicClient.py
--rw-r--r--   0        0        0     2516 2023-01-24 15:42:22.201508 pyfirecrest-1.3.0/firecrest/FirecrestException.py
--rw-r--r--   0        0        0      930 2023-01-24 15:42:22.201508 pyfirecrest-1.3.0/firecrest/__init__.py
--rw-r--r--   0        0        0    35201 2023-01-24 15:42:22.201508 pyfirecrest-1.3.0/firecrest/cli/__init__.py
--rw-r--r--   0        0        0      321 2023-01-24 15:42:22.201508 pyfirecrest-1.3.0/firecrest/cli_script.py
--rw-r--r--   0        0        0      186 2023-01-24 15:42:22.201508 pyfirecrest-1.3.0/firecrest/version.py
--rw-r--r--   0        0        0     1097 2023-01-24 15:42:22.201508 pyfirecrest-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 pyfirecrest-1.3.0/setup.py
--rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 pyfirecrest-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      549 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1675 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0     2773 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/.gitignore
+-rw-r--r--   0        0        0      309 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1515 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3178 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/README.md
+-rw-r--r--   0        0        0      638 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/docs/Makefile
+-rw-r--r--   0        0        0     1639 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/docs/source/authorization.rst
+-rw-r--r--   0        0        0     1995 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0      774 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1034 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/docs/source/reference.rst
+-rw-r--r--   0        0        0    12030 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/docs/source/tutorial.rst
+-rw-r--r--   0        0        0     3794 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/firecrest/Authorization.py
+-rw-r--r--   0        0        0    56215 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/firecrest/BasicClient.py
+-rw-r--r--   0        0        0     2735 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/firecrest/FirecrestException.py
+-rw-r--r--   0        0        0      892 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/firecrest/__init__.py
+-rw-r--r--   0        0        0    37849 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/firecrest/cli/__init__.py
+-rw-r--r--   0        0        0      329 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/firecrest/cli_script.py
+-rw-r--r--   0        0        0       26 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/firecrest/py.typed
+-rw-r--r--   0        0        0     2616 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/firecrest/types.py
+-rw-r--r--   0        0        0     1559 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/tests/common.py
+-rw-r--r--   0        0        0      123 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/tests/context.py
+-rw-r--r--   0        0        0     3461 2023-05-04 12:18:34.277071 pyfirecrest-1.4.0/tests/test_authoriation.py
+-rw-r--r--   0        0        0    41385 2023-05-04 12:18:34.281071 pyfirecrest-1.4.0/tests/test_compute.py
+-rw-r--r--   0        0        0    11378 2023-05-04 12:18:34.281071 pyfirecrest-1.4.0/tests/test_extras.py
+-rw-r--r--   0        0        0     6017 2023-05-04 12:18:34.281071 pyfirecrest-1.4.0/tests/test_reservation.py
+-rw-r--r--   0        0        0    10326 2023-05-04 12:18:34.281071 pyfirecrest-1.4.0/tests/test_status.py
+-rw-r--r--   0        0        0    21405 2023-05-04 12:18:34.281071 pyfirecrest-1.4.0/tests/test_storage.py
+-rw-r--r--   0        0        0    44163 2023-05-04 12:18:34.281071 pyfirecrest-1.4.0/tests/test_utilities.py
+-rw-r--r--   0        0        0      255 2023-05-04 12:18:34.281071 pyfirecrest-1.4.0/tox.ini
+-rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 pyfirecrest-1.4.0/PKG-INFO
```

### Comparing `pyfirecrest-1.3.0/LICENSE` & `pyfirecrest-1.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018-2022 ETH Zurich. All rights reserved.
+Copyright (c) 2018-2023 ETH Zurich. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
     1. Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.
     2. Redistributions in binary form must reproduce the above copyright notice,
```

### Comparing `pyfirecrest-1.3.0/firecrest/Authorization.py` & `pyfirecrest-1.4.0/firecrest/Authorization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #
-#  Copyright (c) 2019-2022, ETH Zurich. All rights reserved.
+#  Copyright (c) 2019-2023, ETH Zurich. All rights reserved.
 #
 #  Please, refer to the LICENSE file in the root directory.
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 import logging
 import requests
 import time
-import datetime
 
 import firecrest.FirecrestException as fe
 
 from datetime import datetime
-from requests.compat import json
+from requests.compat import json  # type: ignore
+from typing import Optional, Tuple, Union
 
 logger = logging.getLogger(__name__)
 
 
 class ClientCredentialsAuth:
     """
     Client Credentials Authorization class.
@@ -27,27 +27,39 @@
     :type client_secret: string
     :param token_uri: URI of the token request in the authorization server (e.g. https://auth.your-server.com/auth/realms/cscs/protocol/openid-connect/token)
     :type token_uri: string
     :param min_token_validity: reuse OIDC token until {min_token_validity} sec before the expiration time (by default 10). Since the token will be checked by different microservices, setting more time in min_token_validity will ensure that the token doesn't expire in the middle of the request.
     :type min_token_validity: float
     """
 
-    def __init__(self, client_id, client_secret, token_uri, min_token_validity=10):
+    def __init__(
+        self,
+        client_id: str,
+        client_secret: str,
+        token_uri: str,
+        min_token_validity: int = 10,
+    ):
         self._client_id = client_id
         self._client_secret = client_secret
         self._token_uri = token_uri
         self._access_token = None
         self._token_expiration_ts = None
         self._min_token_validity = min_token_validity
+        #: It will be passed to all the requests that will be made.
+        #: How many seconds to wait for the server to send data before giving up.
+        #: After that time a `requests.exceptions.Timeout` error will be raised.
+        #:
+        #: It can be a float or a tuple. More details here: https://requests.readthedocs.io.
+        self.timeout: Optional[
+            Union[float, Tuple[float, float], Tuple[float, None]]
+        ] = None
 
-    def get_access_token(self):
+    def get_access_token(self) -> str:
         """Returns an access token to be used for accessing resources.
         If the request fails the token will be None
-
-        :rtype: string
         """
 
         # Make sure that the access token has at least {min_token_validity} sec left before
         # it expires, otherwise make a new request
         if (
             self._access_token
             and self._token_expiration_ts
@@ -60,25 +72,28 @@
 
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
         data = {
             "grant_type": "client_credentials",
             "client_id": self._client_id,
             "client_secret": self._client_secret,
         }
-        resp = requests.post(self._token_uri, headers=headers, data=data)
+        resp = requests.post(
+            self._token_uri, headers=headers, data=data, timeout=self.timeout
+        )
         try:
             resp_json = resp.json()
         except json.JSONDecodeError:
             resp_json = ""
 
         if not resp.ok:
             logger.critical(
                 f"Could not obtain token: {fe.ClientsCredentialsException([resp])}"
             )
             raise fe.ClientsCredentialsException([resp])
 
         self._access_token = resp_json["access_token"]
         self._token_expiration_ts = time.time() + resp_json["expires_in"]
+        assert self._token_expiration_ts is not None
         logger.info(
             f"Token expires at {datetime.fromtimestamp(self._token_expiration_ts)}"
         )
         return self._access_token
```

### Comparing `pyfirecrest-1.3.0/firecrest/BasicClient.py` & `pyfirecrest-1.4.0/firecrest/BasicClient.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 #
-#  Copyright (c) 2019-2022, ETH Zurich. All rights reserved.
+#  Copyright (c) 2019-2023, ETH Zurich. All rights reserved.
 #
 #  Please, refer to the LICENSE file in the root directory.
 #  SPDX-License-Identifier: BSD-3-Clause
 #
+from __future__ import annotations
+
+from io import BufferedWriter, BytesIO
 import itertools
 import jwt
 import logging
 import pathlib
 import requests
 import shlex
 import shutil
 import subprocess
+import sys
 import time
+from typing import Any, ContextManager, Optional, overload, Sequence, Tuple, List
 import urllib.request
 
 import firecrest.FirecrestException as fe
+import firecrest.types as t
 
 from contextlib import nullcontext
-from requests.compat import json
+from requests.compat import json  # type: ignore
 
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
 
 logger = logging.getLogger(__name__)
 
 # This function is temporarily here
 def handle_response(response):
     print("\nResponse status code:")
     print(response.status_code)
@@ -36,79 +46,79 @@
         print("-")
 
 
 class ExternalStorage:
     """External storage object.
     """
 
-    def __init__(self, client, task_id, previous_responses=None):
+    _final_states: set[str]
+
+    def __init__(
+        self,
+        client: Firecrest,
+        task_id: str,
+        previous_responses: Optional[List[requests.Response]] = None,
+    ) -> None:
         previous_responses = [] if previous_responses is None else previous_responses
         self._client = client
         self._task_id = task_id
         self._in_progress = True
-        self._status = None
+        self._status: Optional[str] = None
         self._data = None
         self._object_storage_data = None
         self._sleep_time = itertools.cycle([1, 5, 10])
         self._responses = previous_responses
 
     @property
-    def client(self):
+    def client(self) -> Firecrest:
         """Returns the client that will be used to get information for the task.
-
-        :rtype: Firecrest Object
         """
         return self._client
 
     @property
-    def task_id(self):
+    def task_id(self) -> str:
         """Returns the FirecREST task ID that is associated with this transfer.
-
-        :rtype: string
         """
         return self._task_id
 
-    def _update(self):
+    def _update(self) -> None:
         if self._status not in self._final_states:
             task = self._client._task_safe(self._task_id, self._responses)
             self._status = task["status"]
             self._data = task["data"]
             logger.info(f"Task {self._task_id} has status {self._status}")
             if not self._object_storage_data:
                 if self._status == "111":
                     self._object_storage_data = task["data"]["msg"]
                 elif self._status == "117":
                     self._object_storage_data = task["data"]
 
     @property
-    def status(self):
+    def status(self) -> str:
         """Returns status of the task that is associated with this transfer.
 
         :calls: GET `/tasks/{taskid}`
-        :rtype: string
         """
         self._update()
-        return self._status
+        return self._status  # type: ignore
 
     @property
-    def in_progress(self):
+    def in_progress(self) -> bool:
         """Returns `False` when the transfer has been completed (succesfully or with errors), otherwise `True`.
 
         :calls: GET `/tasks/{taskid}`
-        :rtype: boolean
         """
         self._update()
         return self._status not in self._final_states
 
     @property
-    def data(self):
+    def data(self) -> Optional[dict]:
         """Returns the task information from the latest response.
 
         :calls: GET `/tasks/{taskid}`
-        :rtype: dictionary
         """
         self._update()
         return self._data
 
     @property
     def object_storage_data(self):
         """Returns the necessary information for the external transfer.
@@ -149,34 +159,35 @@
     +--------+--------------------------------------------------------------------+
     | 114    | Download from Object Storage to server has finished                |
     +--------+--------------------------------------------------------------------+
     | 115    | Download from Object Storage error                                 |
     +--------+--------------------------------------------------------------------+
 
     :param client: FirecREST client associated with the transfer
-    :type client: Firecrest
     :param task_id: FirecrREST task associated with the transfer
-    :type task_id: string
     """
 
-    def __init__(self, client, task_id, previous_responses=None):
+    def __init__(
+        self,
+        client: Firecrest,
+        task_id: str,
+        previous_responses: Optional[List[requests.Response]] = None,
+    ) -> None:
         previous_responses = [] if previous_responses is None else previous_responses
         super().__init__(client, task_id, previous_responses)
         self._final_states = {"114", "115"}
         logger.info(f"Creating ExternalUpload object for task {task_id}")
 
-    def finish_upload(self):
+    def finish_upload(self) -> None:
         """Finish the upload process.
         This call will upload the file to the staging area.
         Check with the method `status` or `in_progress` to see the status of the transfer.
         The transfer from the staging area to the systems's filesystem can take several seconds to start to start.
-
-        :rtype: None
         """
-        c = self.object_storage_data["command"]
+        c = self.object_storage_data["command"]  # typer: ignore
         # LOCAL FIX FOR MAC
         # c = c.replace("192.168.220.19", "localhost")
         logger.info(f"Uploading the file to the staging area with the command: {c}")
         command = subprocess.run(
             shlex.split(c), stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
         if command.returncode != 0:
@@ -201,90 +212,129 @@
     +--------+--------------------------------------------------------------------+
     | 117    | Upload from filesystem to Object Storage has finished successfully |
     +--------+--------------------------------------------------------------------+
     | 118    | Upload from filesystem to Object Storage has finished with errors  |
     +--------+--------------------------------------------------------------------+
 
     :param client: FirecREST client associated with the transfer
-    :type client: Firecrest
     :param task_id: FirecrREST task associated with the transfer
-    :type task_id: string
     """
 
-    def __init__(self, client, task_id, previous_responses=None):
+    def __init__(
+        self,
+        client: Firecrest,
+        task_id: str,
+        previous_responses: Optional[List[requests.Response]] = None,
+    ) -> None:
         previous_responses = [] if previous_responses is None else previous_responses
         super().__init__(client, task_id, previous_responses)
         self._final_states = {"117", "118"}
         logger.info(f"Creating ExternalDownload object for task {task_id}")
 
-    def invalidate_object_storage_link(self):
+    def invalidate_object_storage_link(self) -> None:
         """Invalidate the temporary URL for downloading.
 
         :calls: POST `/storage/xfer-external/invalidate`
-        :rtype: None
         """
         self._client._invalidate(self._task_id)
 
-    def finish_download(self, target_path):
+    def finish_download(self, target_path: str | pathlib.Path | BufferedWriter) -> None:
         """Finish the download process.
 
         :param target_path: the local path to save the file
-        :type target_path: string or binary stream
-        :rtype: None
         """
         url = self.object_storage_data
         logger.info(f"Downloading the file from {url} and saving to {target_path}")
         # LOCAL FIX FOR MAC
         # url = url.replace("192.168.220.19", "localhost")
-        context = (
-            open(target_path, "wb")
-            if isinstance(target_path, str)
-            or isinstance(target_path, pathlib.PosixPath)
+        context: ContextManager[BufferedWriter] = (
+            open(target_path, "wb")  # type: ignore
+            if isinstance(target_path, str) or isinstance(target_path, pathlib.Path)
             else nullcontext(target_path)
         )
         with urllib.request.urlopen(url) as response, context as out_file:
             shutil.copyfileobj(response, out_file)
 
 
 class Firecrest:
     """
     This is the basic class you instantiate to access the FirecREST API v1.
     Necessary parameters are the firecrest URL and an authorization object.
-    This object is responsible of handling the credentials and the only
-    requirement for it is that it has a method get_access_token() that returns
-    a valid access token.
 
     :param firecrest_url: FirecREST's URL
-    :type firecrest_url: string
-    :param authorization: the authorization object
-    :type authorization: object
-    :param verify: either a boolean, in which case it controls whether requests will verify the server’s TLS certificate, or a string, in which case it must be a path to a CA bundle to use (default True)
-    :type verify: boolean or string, optional
+    :param authorization: the authorization object. This object is responsible of handling the credentials and the only requirement for it is that it has a method get_access_token() that returns a valid access token.
+    :param verify: either a boolean, in which case it controls whether requests will verify the server’s TLS certificate, or a string, in which case it must be a path to a CA bundle to use
     :param sa_role: this corresponds to the `F7T_AUTH_ROLE` configuration parameter of the site. If you don't know how FirecREST is setup it's better to leave the default.
-    :type sa_role: string, optional
     """
 
+    TOO_MANY_REQUESTS_CODE = 429
+
+    def _retry_requests(func):
+        def wrapper(*args, **kwargs):
+            client = args[0]
+            num_retries = 0
+            resp = func(*args, **kwargs)
+            while True:
+                if resp.status_code != client.TOO_MANY_REQUESTS_CODE:
+                    break
+                elif (
+                    client.num_retries_rate_limit is not None
+                    and num_retries >= client.num_retries_rate_limit
+                ):
+                    logger.debug(
+                        f"Rate limit is reached and the request has "
+                        f"been retried already {num_retries} times"
+                    )
+                    break
+                else:
+                    reset = resp.headers.get(
+                        "Retry-After",
+                        default=resp.headers.get("RateLimit-Reset", default=10),
+                    )
+                    logger.info(
+                        f"Rate limit is reached, will sleep for "
+                        f"{reset} seconds and try again"
+                    )
+                    reset = int(reset)
+                    time.sleep(reset)
+                    resp = func(*args, **kwargs)
+                    num_retries += 1
+
+            return resp
+
+        return wrapper
+
     def __init__(
-        self, firecrest_url, authorization, verify=None, sa_role="firecrest-sa"
-    ):
+        self,
+        firecrest_url: str,
+        authorization: Any,
+        verify: Optional[str | bool] = None,
+        sa_role: str = "firecrest-sa",
+    ) -> None:
         self._firecrest_url = firecrest_url
         self._authorization = authorization
         # This should be used only for blocking operations that require multiple requests,
         # not for external upload/download
-        self._current_method_requests = []
+        self._current_method_requests: List[requests.Response] = []
         self._verify = verify
         self._sa_role = sa_role
-        #: It will be passed to all the requests that will be made.
+        #: This attribute will be passed to all the requests that will be made.
         #: How many seconds to wait for the server to send data before giving up.
         #: After that time a `requests.exceptions.Timeout` error will be raised.
         #:
         #: It can be a float or a tuple. More details here: https://requests.readthedocs.io.
-        self.timeout = None
-
-    def _get_request(self, endpoint, additional_headers=None, params=None):
+        self.timeout: Optional[float | Tuple[float, float] | Tuple[float, None]] = None
+        #: Number of retries in case the rate limit is reached. When it is set to `None`, the
+        #: client will keep trying until it gets a different status code than 429.
+        self.num_retries_rate_limit: Optional[int] = None
+
+    @_retry_requests  # type: ignore
+    def _get_request(
+        self, endpoint, additional_headers=None, params=None
+    ) -> requests.Response:
         url = f"{self._firecrest_url}{endpoint}"
         headers = {"Authorization": f"Bearer {self._authorization.get_access_token()}"}
         if additional_headers:
             headers.update(additional_headers)
 
         logger.info(f"Making GET request to {endpoint}")
         resp = requests.get(
@@ -292,15 +342,18 @@
             headers=headers,
             params=params,
             verify=self._verify,
             timeout=self.timeout,
         )
         return resp
 
-    def _post_request(self, endpoint, additional_headers=None, data=None, files=None):
+    @_retry_requests  # type: ignore
+    def _post_request(
+        self, endpoint, additional_headers=None, data=None, files=None
+    ) -> requests.Response:
         url = f"{self._firecrest_url}{endpoint}"
         headers = {"Authorization": f"Bearer {self._authorization.get_access_token()}"}
         if additional_headers:
             headers.update(additional_headers)
 
         logger.info(f"Making POST request to {endpoint}")
         resp = requests.post(
@@ -309,15 +362,18 @@
             data=data,
             files=files,
             verify=self._verify,
             timeout=self.timeout,
         )
         return resp
 
-    def _put_request(self, endpoint, additional_headers=None, data=None):
+    @_retry_requests  # type: ignore
+    def _put_request(
+        self, endpoint, additional_headers=None, data=None
+    ) -> requests.Response:
         url = f"{self._firecrest_url}{endpoint}"
         headers = {"Authorization": f"Bearer {self._authorization.get_access_token()}"}
         if additional_headers:
             headers.update(additional_headers)
 
         logger.info(f"Making PUT request to {endpoint}")
         resp = requests.put(
@@ -325,15 +381,18 @@
             headers=headers,
             data=data,
             verify=self._verify,
             timeout=self.timeout,
         )
         return resp
 
-    def _delete_request(self, endpoint, additional_headers=None, data=None):
+    @_retry_requests  # type: ignore
+    def _delete_request(
+        self, endpoint, additional_headers=None, data=None
+    ) -> requests.Response:
         url = f"{self._firecrest_url}{endpoint}"
         headers = {"Authorization": f"Bearer {self._authorization.get_access_token()}"}
         if additional_headers:
             headers.update(additional_headers)
 
         logger.info(f"Making DELETE request to {endpoint}")
         resp = requests.delete(
@@ -341,19 +400,43 @@
             headers=headers,
             data=data,
             verify=self._verify,
             timeout=self.timeout,
         )
         return resp
 
-    def _json_response(self, responses, expected_status_code):
+    @overload
+    def _json_response(
+        self,
+        responses: List[requests.Response],
+        expected_status_code: int,
+        allow_none_result: Literal[False] = ...,
+    ) -> dict:
+        ...
+
+    @overload
+    def _json_response(
+        self,
+        responses: List[requests.Response],
+        expected_status_code: int,
+        allow_none_result: Literal[True],
+    ) -> Optional[dict]:
+        ...
+
+    def _json_response(
+        self,
+        responses: List[requests.Response],
+        expected_status_code: int,
+        allow_none_result: bool = False,
+    ):
         # Will examine only the last response
         response = responses[-1]
         status_code = response.status_code
         # handle_response(response)
+        exc: fe.FirecrestException
         for h in fe.ERROR_HEADERS:
             if h in response.headers:
                 logger.critical(f"Header '{h}' is included in the response")
                 exc = fe.HeaderException(responses)
                 logger.critical(exc)
                 raise exc
 
@@ -379,31 +462,37 @@
             exc = fe.UnexpectedStatusException(responses, expected_status_code)
             logger.critical(exc)
             raise exc
 
         try:
             ret = response.json()
         except json.decoder.JSONDecodeError:
-            ret = None
+            if allow_none_result:
+                ret = None
+            else:
+                exc = fe.NoJSONException(responses)
+                logger.critical(exc)
+                raise exc
 
         return ret
 
-    def _tasks(self, task_ids=None, responses=None):
+    def _tasks(
+        self,
+        task_ids: Optional[List[str]] = None,
+        responses: Optional[List[requests.Response]] = None,
+    ) -> dict[str, t.Task]:
         """Return a dictionary of FirecREST tasks and their last update.
         When `task_ids` is an empty list or contains more than one element the
         `/tasks` endpoint will be called. Otherwise `/tasks/{taskid}`.
         When the `/tasks` is called the method will not give an error for invalid IDs,
         but `/tasks/{taskid}` will raise an exception.
 
         :param task_ids: list of task IDs. When empty all tasks are returned.
-        :type task_ids: list
         :param responses: list of responses that are associated with these tasks (only relevant for error)
-        :type responses: list
         :calls: GET `/tasks` or `/tasks/{taskid}`
-        :rtype: dictionary
         """
         task_ids = [] if task_ids is None else task_ids
         responses = [] if responses is None else responses
         endpoint = "/tasks/"
         if len(task_ids) == 1:
             endpoint += task_ids[0]
 
@@ -413,20 +502,23 @@
         if len(task_ids) == 0:
             return taskinfo["tasks"]
         elif len(task_ids) == 1:
             return {task_ids[0]: taskinfo["task"]}
         else:
             return {k: v for k, v in taskinfo["tasks"].items() if k in task_ids}
 
-    def _task_safe(self, task_id, responses=None):
+    def _task_safe(
+        self, task_id: str, responses: Optional[List[requests.Response]] = None
+    ) -> t.Task:
         if responses is None:
             responses = self._current_method_requests
 
         task = self._tasks([task_id], responses)[task_id]
         status = int(task["status"])
+        exc: fe.FirecrestException
         if status == 115:
             logger.critical("Task has error status code 115")
             exc = fe.StorageUploadException(responses)
             logger.critical(exc)
             raise exc
 
         if status == 118:
@@ -439,188 +531,170 @@
             logger.critical(f"Task has error status code {status}")
             exc = fe.FirecrestException(responses)
             logger.critical(exc)
             raise exc
 
         return task
 
-    def _invalidate(self, task_id, responses=None):
+    def _invalidate(
+        self, task_id: str, responses: Optional[List[requests.Response]] = None
+    ):
         responses = [] if responses is None else responses
         resp = self._post_request(
             endpoint="/storage/xfer-external/invalidate",
             additional_headers={"X-Task-Id": task_id},
         )
         responses.append(resp)
-        return self._json_response(responses, 201)
+        return self._json_response(responses, 201, allow_none_result=True)
 
-    def _poll_tasks(self, task_id, final_status, sleep_time):
+    def _poll_tasks(self, task_id: str, final_status, sleep_time):
         logger.info(f"Polling task {task_id} until status is {final_status}")
         resp = self._task_safe(task_id)
         while resp["status"] < final_status:
             t = next(sleep_time)
             logger.info(
                 f'Status of {task_id} is {resp["status"]}, sleeping for {t} sec'
             )
             time.sleep(t)
             resp = self._task_safe(task_id)
 
         logger.info(f'Status of {task_id} is {resp["status"]}')
         return resp["data"]
 
     # Status
-    def all_services(self):
+    def all_services(self) -> List[t.Service]:
         """Returns a list containing all available micro services with a name, description, and status.
 
         :calls: GET `/status/services`
-        :rtype: list of dictionaries (one for each service)
         """
         resp = self._get_request(endpoint="/status/services")
         return self._json_response([resp], 200)["out"]
 
-    def service(self, service_name):
+    def service(self, service_name: str) -> t.Service:
         """Returns information about a micro service.
         Returns the name, description, and status.
 
         :param service_name: the service name
-        :type service_name: string
         :calls: GET `/status/services/{service_name}`
-        :rtype: list of dictionaries (one for each service)
         """
         resp = self._get_request(endpoint=f"/status/services/{service_name}")
-        return self._json_response([resp], 200)
+        return self._json_response([resp], 200)  # type: ignore
 
-    def all_systems(self):
+    def all_systems(self) -> List[t.System]:
         """Returns a list containing all available systems and response status.
 
         :calls: GET `/status/systems`
-        :rtype: list of dictionaries (one for each system)
         """
         resp = self._get_request(endpoint="/status/systems")
         return self._json_response([resp], 200)["out"]
 
-    def system(self, system_name):
+    def system(self, system_name: str) -> t.System:
         """Returns information about a system.
         Returns the name, description, and status.
 
         :param system_name: the system name
-        :type system_name: string
         :calls: GET `/status/systems/{system_name}`
-        :rtype: list of dictionaries (one for each system)
         """
         resp = self._get_request(endpoint=f"/status/systems/{system_name}")
         return self._json_response([resp], 200)["out"]
 
-    def parameters(self):
-        """Returns list of parameters that can be configured in environment files.
+    def parameters(self) -> t.Parameters:
+        """Returns configuration parameters of the FirecREST deployment that is associated with the client.
 
         :calls: GET `/status/parameters`
-        :rtype: list of parameters
         """
         resp = self._get_request(endpoint="/status/parameters")
         return self._json_response([resp], 200)["out"]
 
     # Utilities
-    def list_files(self, machine, target_path, show_hidden=None):
+    def list_files(
+        self, machine: str, target_path: str, show_hidden: bool = False
+    ) -> List[t.LsFile]:
         """Returns a list of files in a directory.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string
         :param show_hidden: show hidden files
-        :type show_hidden: boolean, optional
         :calls: GET `/utilities/ls`
-        :rtype: list of files
         """
-        params = {"targetPath": f"{target_path}"}
-        if show_hidden == True:
+        params: dict[str, Any] = {"targetPath": f"{target_path}"}
+        if show_hidden is True:
             params["showhidden"] = show_hidden
 
         resp = self._get_request(
             endpoint="/utilities/ls",
             additional_headers={"X-Machine-Name": machine},
             params=params,
         )
         return self._json_response([resp], 200)["output"]
 
-    def mkdir(self, machine, target_path, p=None):
+    def mkdir(self, machine: str, target_path: str, p: Optional[bool] = None) -> None:
         """Creates a new directory.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string
         :param p: no error if existing, make parent directories as needed
-        :type p: boolean, optional
         :calls: POST `/utilities/mkdir`
-        :rtype: None
         """
-        data = {"targetPath": target_path}
+        data: dict[str, Any] = {"targetPath": target_path}
         if p:
             data["p"] = p
 
         resp = self._post_request(
             endpoint="/utilities/mkdir",
             additional_headers={"X-Machine-Name": machine},
             data=data,
         )
         self._json_response([resp], 201)
 
-    def mv(self, machine, source_path, target_path):
+    def mv(self, machine: str, source_path: str, target_path: str) -> None:
         """Rename/move a file, directory, or symlink at the `source_path` to the `target_path` on `machine`'s filesystem.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param source_path: the absolute source path
-        :type source_path: string
         :param target_path: the absolute target path
-        :type target_path: string
         :calls: PUT `/utilities/rename`
-        :rtype: None
         """
         resp = self._put_request(
             endpoint="/utilities/rename",
             additional_headers={"X-Machine-Name": machine},
             data={"targetPath": target_path, "sourcePath": source_path},
         )
         self._json_response([resp], 200)
 
-    def chmod(self, machine, target_path, mode):
+    def chmod(self, machine: str, target_path: str, mode: str) -> None:
         """Changes the file mod bits of a given file according to the specified mode.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string
         :param mode: same as numeric mode of linux chmod tool
-        :type mode: string
         :calls: PUT `/utilities/chmod`
-        :rtype: None
         """
         resp = self._put_request(
             endpoint="/utilities/chmod",
             additional_headers={"X-Machine-Name": machine},
             data={"targetPath": target_path, "mode": mode},
         )
         self._json_response([resp], 200)
 
-    def chown(self, machine, target_path, owner=None, group=None):
+    def chown(
+        self,
+        machine: str,
+        target_path: str,
+        owner: Optional[str] = None,
+        group: Optional[str] = None,
+    ) -> None:
         """Changes the user and/or group ownership of a given file.
         If only owner or group information is passed, only that information will be updated.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string
         :param owner: owner ID for target
-        :type owner: string, optional
         :param group: group ID for target
-        :type group: string, optional
         :calls: PUT `/utilities/chown`
-        :rtype: None
         """
         if owner is None and group is None:
             return
 
         data = {"targetPath": target_path}
         if owner:
             data["owner"] = owner
@@ -631,213 +705,240 @@
         resp = self._put_request(
             endpoint="/utilities/chown",
             additional_headers={"X-Machine-Name": machine},
             data=data,
         )
         self._json_response([resp], 200)
 
-    def copy(self, machine, source_path, target_path):
+    def copy(self, machine: str, source_path: str, target_path: str) -> None:
         """Copies file from `source_path` to `target_path`.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param source_path: the absolute source path
-        :type source_path: string
         :param target_path: the absolute target path
-        :type target_path: string
         :calls: POST `/utilities/copy`
-        :rtype: None
         """
         resp = self._post_request(
             endpoint="/utilities/copy",
             additional_headers={"X-Machine-Name": machine},
             data={"targetPath": target_path, "sourcePath": source_path},
         )
         self._json_response([resp], 201)
 
-    def file_type(self, machine, target_path):
+    def file_type(self, machine: str, target_path: str) -> str:
         """Uses the `file` linux application to determine the type of a file.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string
         :calls: GET `/utilities/file`
-        :rtype: string
         """
         resp = self._get_request(
             endpoint="/utilities/file",
             additional_headers={"X-Machine-Name": machine},
             params={"targetPath": target_path},
         )
         return self._json_response([resp], 200)["output"]
 
-    def stat(self, machine, target_path, dereference=False):
+    def stat(
+        self, machine: str, target_path: str, dereference: bool = False
+    ) -> t.StatFile:
         """Uses the stat linux application to determine the status of a file on the machine's filesystem.
         The result follows: https://docs.python.org/3/library/os.html#os.stat_result.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string
         :param dereference: follow link (default False)
-        :type dereference: boolean, optional
         :calls: GET `/utilities/stat`
-        :rtype: string
         """
-        params = {"targetPath": target_path}
+        params: dict[str, Any] = {"targetPath": target_path}
         if dereference:
             params["dereference"] = dereference
 
         resp = self._get_request(
             endpoint="/utilities/stat",
             additional_headers={"X-Machine-Name": machine},
             params=params,
         )
         return self._json_response([resp], 200)["output"]
 
-    def symlink(self, machine, target_path, link_path):
+    def symlink(self, machine: str, target_path: str, link_path: str) -> None:
         """Creates a symbolic link.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute path that the symlink will point to
-        :type target_path: string
         :param link_path: the absolute path to the new symlink
-        :type link_path: string
         :calls: POST `/utilities/symlink`
-        :rtype: None
         """
         resp = self._post_request(
             endpoint="/utilities/symlink",
             additional_headers={"X-Machine-Name": machine},
             data={"targetPath": target_path, "linkPath": link_path},
         )
         self._json_response([resp], 201)
 
-    def simple_download(self, machine, source_path, target_path):
+    def simple_download(
+        self, machine: str, source_path: str, target_path: str | pathlib.Path | BytesIO
+    ) -> None:
         """Blocking call to download a small file.
         The maximun size of file that is allowed can be found from the parameters() call.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param source_path: the absolute source path
-        :type source_path: string
         :param target_path: the target path in the local filesystem or binary stream
-        :type target_path: string or binary stream
         :calls: GET `/utilities/download`
-        :rtype: None
         """
         resp = self._get_request(
             endpoint="/utilities/download",
             additional_headers={"X-Machine-Name": machine},
             params={"sourcePath": source_path},
         )
-        self._json_response([resp], 200)
-        context = (
-            open(target_path, "wb")
-            if isinstance(target_path, str)
-            or isinstance(target_path, pathlib.PosixPath)
+        self._json_response([resp], 200, allow_none_result=True)
+        context: ContextManager[BytesIO] = (
+            open(target_path, "wb")  # type: ignore
+            if isinstance(target_path, str) or isinstance(target_path, pathlib.Path)
             else nullcontext(target_path)
         )
         with context as f:
             f.write(resp.content)
 
-    def simple_upload(self, machine, source_path, target_path, filename=None):
+    def simple_upload(
+        self,
+        machine: str,
+        source_path: str | pathlib.Path | BytesIO,
+        target_path: str,
+        filename: Optional[str] = None,
+    ) -> None:
         """Blocking call to upload a small file.
         The file that will be uploaded will have the same name as the source_path.
         The maximum size of file that is allowed can be found from the parameters() call.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param source_path: the source path of the file or binary stream
-        :type source_path: string or binary stream
         :param target_path: the absolute target path of the directory where the file will be uploaded
-        :type target_path: string
         :param filename: naming target file to filename (default is same as the local one)
-        :type filename: string
         :calls: POST `/utilities/upload`
-        :rtype: None
         """
-        context = (
-            open(source_path, "rb")
-            if isinstance(source_path, str)
-            or isinstance(source_path, pathlib.PosixPath)
+        context: ContextManager[BytesIO] = (
+            open(source_path, "rb")  # type: ignore
+            if isinstance(source_path, str) or isinstance(source_path, pathlib.Path)
             else nullcontext(source_path)
         )
         with context as f:
             # Set filename
             if filename is not None:
-                f = (filename, f)
+                f = (filename, f)  # type: ignore
 
             resp = self._post_request(
                 endpoint="/utilities/upload",
                 additional_headers={"X-Machine-Name": machine},
                 data={"targetPath": target_path},
                 files={"file": f},
             )
 
         self._json_response([resp], 201)
 
-    def simple_delete(self, machine, target_path):
+    def simple_delete(self, machine: str, target_path: str) -> None:
         """Blocking call to delete a small file.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string
         :calls: DELETE `/utilities/rm`
-        :rtype: None
         """
         resp = self._delete_request(
             endpoint="/utilities/rm",
             additional_headers={"X-Machine-Name": machine},
             data={"targetPath": target_path},
         )
-        self._json_response([resp], 204)
+        self._json_response([resp], 204, allow_none_result=True)
 
-    def checksum(self, machine, target_path):
+    def checksum(self, machine: str, target_path: str) -> str:
         """Calculate the SHA256 (256-bit) checksum of a specified file.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string
         :calls: GET `/utilities/checksum`
-        :rtype: string
         """
         resp = self._get_request(
             endpoint="/utilities/checksum",
             additional_headers={"X-Machine-Name": machine},
             params={"targetPath": target_path},
         )
         return self._json_response([resp], 200)["output"]
 
-    def view(self, machine, target_path):
+    def head(
+        self,
+        machine: str,
+        target_path: str,
+        bytes: Optional[int] = None,
+        lines: Optional[int] = None,
+    ) -> str:
+        """Display the beginning of a specified file.
+        By default 10 lines will be returned.
+        Bytes and lines cannot be specified simultaneously.
+        The final result will be smaller than `UTILITIES_MAX_FILE_SIZE` bytes.
+        This variable is available in the parameters command.
+
+        :param machine: the machine name where the filesystem belongs to
+        :param target_path: the absolute target path
+        :param lines: the number of lines to be displayed
+        :param bytes: the number of bytes to be displayed
+        :calls: GET `/utilities/head`
+        """
+        resp = self._get_request(
+            endpoint="/utilities/head",
+            additional_headers={"X-Machine-Name": machine},
+            params={"targetPath": target_path, "lines": lines, "bytes": bytes},
+        )
+        return self._json_response([resp], 200)["output"]
+
+    def tail(
+        self,
+        machine: str,
+        target_path: str,
+        bytes: Optional[int] = None,
+        lines: Optional[int] = None,
+    ) -> str:
+        """Display the last part of a specified file.
+        By default 10 lines will be returned.
+        Bytes and lines cannot be specified simultaneously.
+        The final result will be smaller than `UTILITIES_MAX_FILE_SIZE` bytes.
+        This variable is available in the parameters command.
+
+        :param machine: the machine name where the filesystem belongs to
+        :param target_path: the absolute target path
+        :param lines: the number of lines to be displayed
+        :param bytes: the number of bytes to be displayed
+        :calls: GET `/utilities/head`
+        """
+        resp = self._get_request(
+            endpoint="/utilities/tail",
+            additional_headers={"X-Machine-Name": machine},
+            params={"targetPath": target_path, "lines": lines, "bytes": bytes},
+        )
+        return self._json_response([resp], 200)["output"]
+
+    def view(self, machine: str, target_path: str) -> str:
         """View the content of a specified file.
+        The final result will be smaller than `UTILITIES_MAX_FILE_SIZE` bytes.
+        This variable is available in the parameters command.
 
         :param machine: the machine name where the filesystem belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string
         :calls: GET `/utilities/checksum`
-        :rtype: string
         """
         resp = self._get_request(
             endpoint="/utilities/view",
             additional_headers={"X-Machine-Name": machine},
             params={"targetPath": target_path},
         )
         return self._json_response([resp], 200)["output"]
 
-    def whoami(self):
+    def whoami(self) -> Optional[str]:
         """Returns the username that FirecREST will be using to perform the other calls.
         Will return `None` if the token is not valid.
-
-        :rtype: string or None
         """
 
         # FIXME This needs to be added as an endpoint in FirecREST,
         # now it's making a guess and it could be wrong.
         try:
             decoded = jwt.decode(
                 self._authorization.get_access_token(),
@@ -854,47 +955,57 @@
                 return decoded["preferred_username"]
 
         except Exception:
             # Invalid token, cannot retrieve username
             return None
 
     # Compute
-    def _submit_request(self, machine, job_script, local_file):
+    def _submit_request(self, machine: str, job_script, local_file, account=None):
         if local_file:
             with open(job_script, "rb") as f:
+                if account:
+                    data = {"account": account}
+                else:
+                    data = None
+
                 resp = self._post_request(
                     endpoint="/compute/jobs/upload",
                     additional_headers={"X-Machine-Name": machine},
                     files={"file": f},
+                    data=data,
                 )
         else:
+            data = {"targetPath": job_script}
+            if account:
+                data["account"] = account
+
             resp = self._post_request(
                 endpoint="/compute/jobs/path",
                 additional_headers={"X-Machine-Name": machine},
-                data={"targetPath": job_script},
+                data=data,
             )
 
         self._current_method_requests.append(resp)
         return self._json_response(self._current_method_requests, 201)
 
-    def _squeue_request(self, machine, jobs=None):
+    def _squeue_request(self, machine: str, jobs=None):
         jobs = [] if jobs is None else jobs
         params = {}
         if jobs:
             params = {"jobs": ",".join([str(j) for j in jobs])}
 
         resp = self._get_request(
             endpoint="/compute/jobs",
             additional_headers={"X-Machine-Name": machine},
             params=params,
         )
         self._current_method_requests.append(resp)
         return self._json_response(self._current_method_requests, 200)
 
-    def _acct_request(self, machine, jobs=None, start_time=None, end_time=None):
+    def _acct_request(self, machine: str, jobs=None, start_time=None, end_time=None):
         jobs = [] if jobs is None else jobs
         params = {}
         if jobs:
             params["jobs"] = ",".join(jobs)
 
         if start_time:
             params["starttime"] = start_time
@@ -906,101 +1017,100 @@
             endpoint="/compute/acct",
             additional_headers={"X-Machine-Name": machine},
             params=params,
         )
         self._current_method_requests.append(resp)
         return self._json_response(self._current_method_requests, 200)
 
-    def submit(self, machine, job_script, local_file=True):
+    def submit(
+        self,
+        machine: str,
+        job_script: str,
+        local_file: Optional[bool] = True,
+        account: Optional[str] = None,
+    ) -> t.JobSubmit:
         """Submits a batch script to SLURM on the target system
 
         :param machine: the machine name where the scheduler belongs to
-        :type machine: string
         :param job_script: the path of the script (if it's local it can be relative path, if it is on the machine it has to be the absolute path)
-        :type job_script: string
         :param local_file: batch file can be local (default) or on the machine's filesystem
-        :type local_file: boolean, optional
+        :param account: submit the job with this project account
         :calls: POST `/compute/jobs/upload` or POST `/compute/jobs/path`
 
                 GET `/tasks/{taskid}`
-        :rtype: dictionary
         """
         self._current_method_requests = []
-        json_response = self._submit_request(machine, job_script, local_file)
+        json_response = self._submit_request(machine, job_script, local_file, account)
         logger.info(f"Job submission task: {json_response['task_id']}")
         return self._poll_tasks(
             json_response["task_id"], "200", itertools.cycle([1, 5, 10])
         )
 
-    def poll(self, machine, jobs=None, start_time=None, end_time=None):
+    def poll(
+        self,
+        machine: str,
+        jobs: Optional[Sequence[str | int]] = None,
+        start_time: Optional[str] = None,
+        end_time: Optional[str] = None,
+    ) -> List[t.JobAcct]:
         """Retrieves information about submitted jobs.
         This call uses the `sacct` command.
 
         :param machine: the machine name where the scheduler belongs to
-        :type machine: string
         :param jobs: list of the IDs of the jobs
-        :type jobs: list of strings/integers, optional
         :param start_time: Start time (and/or date) of job's query. Allowed formats are HH:MM[:SS] [AM|PM] MMDD[YY] or MM/DD[/YY] or MM.DD[.YY] MM/DD[/YY]-HH:MM[:SS] YYYY-MM-DD[THH:MM[:SS]]
-        :type start_time: string, optional
         :param end_time: End time (and/or date) of job's query. Allowed formats are HH:MM[:SS] [AM|PM] MMDD[YY] or MM/DD[/YY] or MM.DD[.YY] MM/DD[/YY]-HH:MM[:SS] YYYY-MM-DD[THH:MM[:SS]]
-        :type end_time: string, optional
         :calls: GET `/compute/acct`
 
                 GET `/tasks/{taskid}`
-        :rtype: dictionary
         """
         self._current_method_requests = []
-        jobs = jobs if jobs else []
-        jobids = [str(j) for j in jobs]
+        jobids = [str(j) for j in jobs] if jobs else []
         json_response = self._acct_request(machine, jobids, start_time, end_time)
         logger.info(f"Job polling task: {json_response['task_id']}")
         res = self._poll_tasks(
             json_response["task_id"], "200", itertools.cycle([1, 5, 10])
         )
         # When there is no job in the sacct output firecrest will return an empty dictionary instead of list
         if isinstance(res, dict):
             return list(res.values())
         else:
             return res
 
-    def poll_active(self, machine, jobs=None):
+    def poll_active(
+        self, machine: str, jobs: Optional[Sequence[str | int]] = None
+    ) -> List[t.JobQueue]:
         """Retrieves information about active jobs.
         This call uses the `squeue -u <username>` command.
 
         :param machine: the machine name where the scheduler belongs to
-        :type machine: string
         :param jobs: list of the IDs of the jobs
-        :type jobs: list of strings/integers, optional
         :calls: GET `/compute/jobs`
 
                 GET `/tasks/{taskid}`
-        :rtype: dictionary
         """
         self._current_method_requests = []
         jobs = jobs if jobs else []
         jobids = [str(j) for j in jobs]
         json_response = self._squeue_request(machine, jobids)
         logger.info(f"Job active polling task: {json_response['task_id']}")
         dict_result = self._poll_tasks(
             json_response["task_id"], "200", itertools.cycle([1, 5, 10])
         )
         return list(dict_result.values())
 
-    def cancel(self, machine, job_id):
+    def cancel(self, machine: str, job_id: str | int) -> str:
         """Cancels running job.
         This call uses the `scancel` command.
 
         :param machine: the machine name where the scheduler belongs to
-        :type machine: string
-        :param job_id: the absolute target path (default [])
-        :type job_id: list of strings/integers, optional
+        :param job_id: the ID of the job
         :calls: DELETE `/compute/jobs/{job_id}`
 
                 GET `/tasks/{taskid}`
-        :rtype: dictionary
         """
         self._current_method_requests = []
         resp = self._delete_request(
             endpoint=f"/compute/jobs/{job_id}",
             additional_headers={"X-Machine-Name": machine},
         )
         self._current_method_requests.append(resp)
@@ -1042,45 +1152,37 @@
             endpoint=endpoint, additional_headers={"X-Machine-Name": machine}, data=data
         )
         self._current_method_requests.append(resp)
         return self._json_response(self._current_method_requests, 201)
 
     def submit_move_job(
         self,
-        machine,
-        source_path,
-        target_path,
-        job_name=None,
-        time=None,
-        stage_out_job_id=None,
-        account=None,
-    ):
+        machine: str,
+        source_path: str,
+        target_path: str,
+        job_name: Optional[str] = None,
+        time: Optional[str] = None,
+        stage_out_job_id: Optional[str] = None,
+        account: Optional[str] = None,
+    ) -> t.JobSubmit:
         """Move files between internal CSCS file systems.
         Rename/Move source_path to target_path.
         Possible to stage-out jobs providing the SLURM ID of a production job.
         More info about internal transfer: https://user.cscs.ch/storage/data_transfer/internal_transfer/
 
         :param machine: the machine name where the scheduler belongs to
-        :type machine: string
         :param source_path: the absolute source path
-        :type source_path: string
         :param target_path: the absolute target path
-        :type target_path: string,
         :param job_name: job name
-        :type job_name: string, optional
         :param time: limit on the total run time of the job. Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
-        :type time: string, optional
         :param stage_out_job_id: transfer data after job with ID {stage_out_job_id} is completed
-        :type stage_out_job_id: string, optional
         :param account: name of the bank account to be used in SLURM. If not set, system default is taken.
-        :type account: string, optional
         :calls: POST `/storage/xfer-internal/mv`
 
                 GET `/tasks/{taskid}`
-        :rtype: dictionary with the jobid of the submitted job
         """
         self._current_method_requests = []
         endpoint = "/storage/xfer-internal/mv"
         json_response = self._internal_transfer(
             endpoint,
             machine,
             source_path,
@@ -1093,45 +1195,37 @@
         logger.info(f"Job submission task: {json_response['task_id']}")
         return self._poll_tasks(
             json_response["task_id"], "200", itertools.cycle([1, 5, 10])
         )
 
     def submit_copy_job(
         self,
-        machine,
-        source_path,
-        target_path,
-        job_name=None,
-        time=None,
-        stage_out_job_id=None,
-        account=None,
-    ):
+        machine: str,
+        source_path: str,
+        target_path: str,
+        job_name: Optional[str] = None,
+        time: Optional[str] = None,
+        stage_out_job_id: Optional[str] = None,
+        account: Optional[str] = None,
+    ) -> t.JobSubmit:
         """Copy files between internal CSCS file systems.
         Copy source_path to target_path.
         Possible to stage-out jobs providing the SLURM Id of a production job.
         More info about internal transfer: https://user.cscs.ch/storage/data_transfer/internal_transfer/
 
         :param machine: the machine name where the scheduler belongs to
-        :type machine: string
         :param source_path: the absolute source path
-        :type source_path: string
         :param target_path: the absolute target path
-        :type target_path: string,
         :param job_name: job name
-        :type job_name: string, optional
         :param time: limit on the total run time of the job. Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
-        :type time: string, optional
         :param stage_out_job_id: transfer data after job with ID {stage_out_job_id} is completed
-        :type stage_out_job_id: string, optional
         :param account: name of the bank account to be used in SLURM. If not set, system default is taken.
-        :type account: string, optional
         :calls: POST `/storage/xfer-internal/cp`
 
                 GET `/tasks/{taskid}`
-        :rtype: dictionary with the jobid of the submitted job
         """
         self._current_method_requests = []
         endpoint = "/storage/xfer-internal/cp"
         json_response = self._internal_transfer(
             endpoint,
             machine,
             source_path,
@@ -1144,45 +1238,37 @@
         logger.info(f"Job submission task: {json_response['task_id']}")
         return self._poll_tasks(
             json_response["task_id"], "200", itertools.cycle([1, 5, 10])
         )
 
     def submit_rsync_job(
         self,
-        machine,
-        source_path,
-        target_path,
-        job_name=None,
-        time=None,
-        stage_out_job_id=None,
-        account=None,
-    ):
+        machine: str,
+        source_path: str,
+        target_path: str,
+        job_name: Optional[str] = None,
+        time: Optional[str] = None,
+        stage_out_job_id: Optional[str] = None,
+        account: Optional[str] = None,
+    ) -> t.JobSubmit:
         """Transfer files between internal CSCS file systems.
         Transfer source_path to target_path.
         Possible to stage-out jobs providing the SLURM Id of a production job.
         More info about internal transfer: https://user.cscs.ch/storage/data_transfer/internal_transfer/
 
         :param machine: the machine name where the scheduler belongs to
-        :type machine: string
         :param source_path: the absolute source path
-        :type source_path: string
         :param target_path: the absolute target path
-        :type target_path: string,
         :param job_name: job name
-        :type job_name: string, optional
         :param time: limit on the total run time of the job. Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
-        :type time: string, optional
         :param stage_out_job_id: transfer data after job with ID {stage_out_job_id} is completed
-        :type stage_out_job_id: string, optional
         :param account: name of the bank account to be used in SLURM. If not set, system default is taken.
-        :type account: string, optional
         :calls: POST `/storage/xfer-internal/rsync`
 
                 GET `/tasks/{taskid}`
-        :rtype: dictionary with the jobid of the submitted job
         """
         self._current_method_requests = []
         endpoint = "/storage/xfer-internal/rsync"
         json_response = self._internal_transfer(
             endpoint,
             machine,
             source_path,
@@ -1195,42 +1281,35 @@
         logger.info(f"Job submission task: {json_response['task_id']}")
         return self._poll_tasks(
             json_response["task_id"], "200", itertools.cycle([1, 5, 10])
         )
 
     def submit_delete_job(
         self,
-        machine,
-        target_path,
-        job_name=None,
-        time=None,
-        stage_out_job_id=None,
-        account=None,
-    ):
+        machine: str,
+        target_path: str,
+        job_name: Optional[str] = None,
+        time: Optional[str] = None,
+        stage_out_job_id: Optional[str] = None,
+        account: Optional[str] = None,
+    ) -> t.JobSubmit:
         """Remove files in internal CSCS file systems.
         Remove file in target_path.
         Possible to stage-out jobs providing the SLURM Id of a production job.
         More info about internal transfer: https://user.cscs.ch/storage/data_transfer/internal_transfer/
 
         :param machine: the machine name where the scheduler belongs to
-        :type machine: string
         :param target_path: the absolute target path
-        :type target_path: string,
         :param job_name: job name
-        :type job_name: string, optional
         :param time: limit on the total run time of the job. Acceptable time formats 'minutes', 'minutes:seconds', 'hours:minutes:seconds', 'days-hours', 'days-hours:minutes' and 'days-hours:minutes:seconds'.
-        :type time: string, optional
         :param stage_out_job_id: transfer data after job with ID {stage_out_job_id} is completed
-        :type stage_out_job_id: string, optional
         :param account: name of the bank account to be used in SLURM. If not set, system default is taken.
-        :type account: string, optional
         :calls: POST `/storage/xfer-internal/rm`
 
                 GET `/tasks/{taskid}`
-        :rtype: dictionary with the jobid of the submitted job
         """
         self._current_method_requests = []
         endpoint = "/storage/xfer-internal/rm"
         json_response = self._internal_transfer(
             endpoint,
             machine,
             None,
@@ -1241,95 +1320,80 @@
             account,
         )
         logger.info(f"Job submission task: {json_response['task_id']}")
         return self._poll_tasks(
             json_response["task_id"], "200", itertools.cycle([1, 5, 10])
         )
 
-    def external_upload(self, machine, source_path, target_path):
+    def external_upload(
+        self, machine: str, source_path: str, target_path: str
+    ) -> ExternalUpload:
         """Non blocking call for the upload of larger files.
 
         :param machine: the machine where the filesystem belongs to
-        :type machine: string
         :param source_path: the source path in the local filesystem
-        :type source_path: string
         :param target_path: the target path in the machine's filesystem
-        :type target_path: string
         :returns: an ExternalUpload object
-        :rtype: ExternalUpload
         """
         resp = self._post_request(
             endpoint="/storage/xfer-external/upload",
             additional_headers={"X-Machine-Name": machine},
             data={"targetPath": target_path, "sourcePath": source_path},
         )
         json_response = self._json_response([resp], 201)["task_id"]
         return ExternalUpload(self, json_response, [resp])
 
-    def external_download(self, machine, source_path):
+    def external_download(self, machine: str, source_path: str) -> ExternalDownload:
         """Non blocking call for the download of larger files.
 
         :param machine: the machine where the filesystem belongs to
-        :type machine: string
         :param source_path: the source path in the local filesystem
-        :type source_path: string
         :returns: an ExternalDownload object
-        :rtype: ExternalDownload
         """
         resp = self._post_request(
             endpoint="/storage/xfer-external/download",
             additional_headers={"X-Machine-Name": machine},
             data={"sourcePath": source_path},
         )
         return ExternalDownload(
             self, self._json_response([resp], 201)["task_id"], [resp]
         )
 
     # Reservation
-    def all_reservations(self, machine):
+    def all_reservations(self, machine: str) -> List[dict]:
         """List all active reservations and their status
 
         :param machine: the machine name
-        :type machine: string
         :calls: GET `/reservations`
-        :rtype: list of dictionaries (one for each reservation)
         """
         resp = self._get_request(
             endpoint="/reservations", additional_headers={"X-Machine-Name": machine}
         )
         return self._json_response([resp], 200)["success"]
 
     def create_reservation(
         self,
-        machine,
-        reservation,
-        account,
-        number_of_nodes,
-        node_type,
-        start_time,
-        end_time,
-    ):
+        machine: str,
+        reservation: str,
+        account: str,
+        number_of_nodes: str,
+        node_type: str,
+        start_time: str,
+        end_time: str,
+    ) -> None:
         """Creates a new reservation with {reservation} name for a given SLURM groupname
 
         :param machine: the machine name
-        :type machine: string
         :param reservation: the reservation name
-        :type reservation: string
         :param account: the account in SLURM to which the reservation is made for
-        :type account: string
         :param number_of_nodes: number of nodes needed for the reservation
-        :type number_of_nodes: string
         :param node_type: type of node
-        :type node_type: string
         :param start_time: start time for reservation (YYYY-MM-DDTHH:MM:SS)
-        :type start_time: string
         :param end_time: end time for reservation (YYYY-MM-DDTHH:MM:SS)
-        :type end_time: string
         :calls: POST `/reservations`
-        :rtype: None
         """
         data = {
             "reservation": reservation,
             "account": account,
             "numberOfNodes": number_of_nodes,
             "nodeType": node_type,
             "starttime": start_time,
@@ -1340,40 +1404,32 @@
             additional_headers={"X-Machine-Name": machine},
             data=data,
         )
         self._json_response([resp], 201)
 
     def update_reservation(
         self,
-        machine,
-        reservation,
-        account,
-        number_of_nodes,
-        node_type,
-        start_time,
-        end_time,
-    ):
+        machine: str,
+        reservation: str,
+        account: str,
+        number_of_nodes: str,
+        node_type: str,
+        start_time: str,
+        end_time: str,
+    ) -> None:
         """Updates an already created reservation named {reservation}
 
         :param machine: the machine name
-        :type machine: string
         :param reservation: the reservation name
-        :type reservation: string
         :param account: the account in SLURM to which the reservation is made for
-        :type account: string
         :param number_of_nodes: number of nodes needed for the reservation
-        :type number_of_nodes: string
         :param node_type: type of node
-        :type node_type: string
         :param start_time: start time for reservation (YYYY-MM-DDTHH:MM:SS)
-        :type start_time: string
         :param end_time: end time for reservation (YYYY-MM-DDTHH:MM:SS)
-        :type end_time: string
         :calls: PUT `/reservations/{reservation}`
-        :rtype: None
         """
         data = {
             "account": account,
             "numberOfNodes": number_of_nodes,
             "nodeType": node_type,
             "starttime": start_time,
             "endtime": end_time,
@@ -1381,22 +1437,19 @@
         resp = self._put_request(
             endpoint=f"/reservations/{reservation}",
             additional_headers={"X-Machine-Name": machine},
             data=data,
         )
         self._json_response([resp], 200)
 
-    def delete_reservation(self, machine, reservation):
+    def delete_reservation(self, machine: str, reservation: str) -> None:
         """Deletes an already created reservation named {reservation}
 
         :param machine: the machine name
-        :type machine: string
         :param reservation: the reservation name
-        :type reservation: string
         :calls: DELETE `/reservations/{reservation}`
-        :rtype: None
         """
         resp = self._delete_request(
             endpoint=f"/reservations/{reservation}",
             additional_headers={"X-Machine-Name": machine},
         )
-        self._json_response([resp], 204)
+        self._json_response([resp], 204, allow_none_result=True)
```

### Comparing `pyfirecrest-1.3.0/firecrest/FirecrestException.py` & `pyfirecrest-1.4.0/firecrest/FirecrestException.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright (c) 2019-2022, ETH Zurich. All rights reserved.
+#  Copyright (c) 2019-2023, ETH Zurich. All rights reserved.
 #
 #  Please, refer to the LICENSE file in the root directory.
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 import json
 
 
@@ -87,14 +87,22 @@
         super().__init__(responses)
         self._expected_status_code = expected_status_code
 
     def __str__(self):
         return f"{super().__str__()}: expected status {self._expected_status_code}"
 
 
+class NoJSONException(FirecrestException):
+    """Exception raised when JSON in not included in the response
+    """
+
+    def __str__(self):
+        return f"{super().__str__()}: JSON is not included in the response"
+
+
 class StorageDownloadException(FirecrestException):
     """Exception raised by a failed external download
     """
 
 
 class StorageUploadException(FirecrestException):
     """Exception raised by a failed external upload
```

### Comparing `pyfirecrest-1.3.0/firecrest/__init__.py` & `pyfirecrest-1.4.0/firecrest/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #
-#  Copyright (c) 2019-2022, ETH Zurich. All rights reserved.
+#  Copyright (c) 2019-2023, ETH Zurich. All rights reserved.
 #
 #  Please, refer to the LICENSE file in the root directory.
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 import sys
-from firecrest.version import VERSION
 
 
-__version__ = VERSION
+__version__ = "1.4.0"
 __app_name__ = "firecrest"
 MIN_PYTHON_VERSION = (3, 7, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
     sys.stderr.write(
         "Unsupported Python version: "
```

### Comparing `pyfirecrest-1.3.0/firecrest/cli/__init__.py` & `pyfirecrest-1.4.0/firecrest/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright (c) 2019-2022, ETH Zurich. All rights reserved.
+#  Copyright (c) 2019-2023, ETH Zurich. All rights reserved.
 #
 #  Please, refer to the LICENSE file in the root directory.
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 import logging
 import typer
 
@@ -58,23 +58,30 @@
 
 custom_theme = {
     "repr.attrib_name": "none",
     "repr.attrib_value": "none",
     "repr.number": "none",
 }
 console = Console(theme=Theme(custom_theme))
-client = None
+client: fc.Firecrest = None  # type: ignore
+logger = logging.getLogger(__name__)
 
 
-def examine_exeption(e):
-    msg = "{__app_name__}: Operation failed"
+def examine_exeption(e: Exception) -> None:
+    msg = f"{__app_name__}: Operation failed"
     if isinstance(e, fc.ClientsCredentialsException):
         msg += ": could not fetch token"
+    elif isinstance(e, fc.FirecrestException):
+        msg += ": a Firecrest client error has occurred"
+    else:
+        # in case of FirecrestException and ClientsCredentialsException
+        # we don't need to log again the exception
+        logger.critical(e)
 
-    console.print(f"[red]{__app_name__}: Operation failed[/red]")
+    console.print(f"[red]{msg}[/red]")
 
 
 def create_table(table_title, data, *mappings):
     table = Table(title=table_title, box=box.ASCII)
     for (title, _) in mappings:
         table.add_column(title, overflow="fold")
 
@@ -110,15 +117,15 @@
             title,
             result,
             ("Service", "service"),
             ("Status", "status"),
             ("Description", "description"),
         )
         console.print(table, overflow="fold")
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Status commands")
 def systems(
     name: Optional[str] = typer.Option(
@@ -139,15 +146,15 @@
             title,
             result,
             ("System", "system"),
             ("Status", "status"),
             ("Description", "description"),
         )
         console.print(table, overflow="fold")
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Status commands")
 def parameters():
     """Configurable parameters of FirecREST
@@ -167,15 +174,15 @@
             result["utilities"],
             ("Name", "name"),
             ("Value", "value"),
             ("Unit", "unit"),
         )
 
         console.print(storage_table, utilities_table, overflow="fold")
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Status commands")
 def tasks(
     taskids: Optional[List[str]] = typer.Argument(
@@ -204,15 +211,15 @@
         )
         if pager:
             with console.pager():
                 console.print(table)
         else:
             console.print(table)
 
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def ls(
     machine: str = typer.Argument(
@@ -244,15 +251,15 @@
                 ("Size", "size"),
                 ("User", "user"),
                 ("Last modified", "last_modified"),
                 ("Link target", "link_target"),
             )
 
             console.print(table)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def mkdir(
     machine: str = typer.Argument(
@@ -265,15 +272,15 @@
         help="Create intermediate directories as required, equivalent to `-p` of the unix command.",
     ),
 ):
     """Create new directories
     """
     try:
         client.mkdir(machine, path, p)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def mv(
     machine: str = typer.Argument(
@@ -282,15 +289,15 @@
     source: str = typer.Argument(..., help="The absolute source path."),
     destination: str = typer.Argument(..., help="The absolute destination path."),
 ):
     """Rename/move files, directory, or symlink at the `source_path` to the `target_path` on `machine`'s filesystem
     """
     try:
         client.mv(machine, source, destination)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def chmod(
     machine: str = typer.Argument(
@@ -299,15 +306,15 @@
     path: str = typer.Argument(..., help="The absolute target path."),
     mode: str = typer.Argument(..., help="Same as numeric mode of linux chmod tool."),
 ):
     """Change the file mod bits of a given file according to the specified mode
     """
     try:
         client.chmod(machine, path, mode)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def chown(
     machine: str = typer.Argument(
@@ -319,15 +326,15 @@
 ):
     """Change the user and/or group ownership of a given file.
 
     If only owner or group information is passed, only that information will be updated.
     """
     try:
         client.chown(machine, path, owner, group)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def cp(
     machine: str = typer.Argument(
@@ -336,15 +343,15 @@
     source: str = typer.Argument(..., help="The absolute source path."),
     destination: str = typer.Argument(..., help="The absolute destination path."),
 ):
     """Copy files
     """
     try:
         client.copy(machine, source, destination)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def file(
     machine: str = typer.Argument(
@@ -352,15 +359,15 @@
     ),
     path: str = typer.Argument(..., help="The absolute target path."),
 ):
     """Determine file type
     """
     try:
         console.print(client.file_type(machine, path))
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def stat(
     machine: str = typer.Argument(
@@ -438,15 +445,15 @@
                 data,
                 ("Attribute", "Attribute"),
                 ("Value", "Value"),
                 ("Description", "Description"),
             )
 
             console.print(table)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def symlink(
     machine: str = typer.Argument(
@@ -455,15 +462,15 @@
     target: str = typer.Argument(..., help="The path of the original file."),
     link_name: str = typer.Argument(..., help="The name of the link to the TARGET."),
 ):
     """Create a symbolic link
     """
     try:
         client.symlink(machine, target, link_name)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def rm(
     machine: str,
@@ -478,15 +485,15 @@
     """Remove directory entries
     """
     try:
         if force:
             client.simple_delete(machine, path)
         else:
             console.print("Operation cancelled")
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def checksum(
     machine: str = typer.Argument(
@@ -494,45 +501,92 @@
     ),
     path: str = typer.Argument(..., help="The absolute target path."),
 ):
     """Calculate the SHA256 (256-bit) checksum
     """
     try:
         console.print(client.checksum(machine, path))
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def head(
     machine: str = typer.Argument(
         ..., help="The machine name where the filesystem belongs to."
     ),
     path: str = typer.Argument(..., help="The absolute target path."),
+    lines: int = typer.Option(
+        None, "-n", "--lines", help="Print count lines of each of the specified files."
+    ),
+    bytes: int = typer.Option(
+        None, "-c", "--bytes", help="Print bytes of each of the specified files."
+    ),
+):
+    """Display the beginning of a specified file.
+    By default the first 10 lines will be returned.
+    Bytes and lines cannot be specified simultaneously.
+
+    You view only files smaller than UTILITIES_MAX_FILE_SIZE bytes.
+    This variable is available in the parameters command.
+    """
+    if lines and bytes:
+        console.print(
+            f"[red]{__app_name__} head: cannot specify both 'bytes' and 'lines'[/red]"
+        )
+        raise typer.Exit(code=1)
+
+    try:
+        console.print(client.head(machine, path, bytes, lines))
+    except Exception as e:
+        examine_exeption(e)
+        raise typer.Exit(code=1)
+
+
+@app.command(rich_help_panel="Utilities commands")
+def tail(
+    machine: str = typer.Argument(
+        ..., help="The machine name where the filesystem belongs to."
+    ),
+    path: str = typer.Argument(..., help="The absolute target path."),
+    lines: int = typer.Option(
+        None, "-n", "--lines", help="Print count lines of each of the specified files."
+    ),
+    bytes: int = typer.Option(
+        None, "-c", "--bytes", help="Print bytes of each of the specified files."
+    ),
 ):
-    """View the content of a specified file
+    """Display the end of a specified file.
+    By default the last 10 lines will be returned.
+    Bytes and lines cannot be specified simultaneously.
 
     You view only files smaller than UTILITIES_MAX_FILE_SIZE bytes.
     This variable is available in the parameters command.
     """
+    if lines and bytes:
+        console.print(
+            f"[red]{__app_name__} tail: cannot specify both 'bytes' and 'lines'[/red]"
+        )
+        raise typer.Exit(code=1)
+
     try:
-        console.print(client.view(machine, path))
-    except fc.FirecrestException as e:
+        console.print(client.tail(machine, path, bytes, lines))
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Utilities commands")
 def whoami():
     """Return the username that FirecREST will be using to perform the other calls
     """
     try:
         console.print(client.whoami())
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 class TransferType(str, Enum):
     direct = "direct"
     external = "external"
@@ -548,22 +602,24 @@
         None,
         help="The destination path (can be relative). It is required only when the download is `direct`.",
     ),
     transfer_type: TransferType = typer.Option(
         TransferType.direct,
         "--type",
         case_sensitive=False,
-        help=f"Select type of transfer (run `{__app_name__} download --help` for details).",
+        help=f"Select type of transfer.",
     ),
 ):
     """Download a file
 
-    Direct download will download the file to the DESTINATION but it will work only for small files. You can find the maximum size by running the `parameters` command.
+    Direct download will download the file to the DESTINATION but it will work only for small files.
+    You can find the maximum size in UTILITIES_MAX_FILE_SIZE by running the `parameters` command.
 
-    External download will return with a link in case of success. The file can be downloaded locally from there without any authentication.
+    External download will return with a link in case of success.
+    The file can be downloaded locally from there without any authentication.
     """
     try:
         if transfer_type == TransferType.direct:
             if destination:
                 client.simple_download(machine, source, destination)
             else:
                 console.print("`destination` is required when the ")
@@ -574,15 +630,15 @@
                 f"Follow the status of the transfer asynchronously with that task ID: [green]{down_obj.task_id}[/green]"
             )
             with console.status(
                 "Moving file to the staging area... It is safe to "
                 "cancel the command and follow up through the task."
             ):
                 console.out(f"Download the file from:\n{down_obj.object_storage_data}")
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Storage commands")
 def upload(
     machine: str = typer.Argument(
@@ -590,24 +646,30 @@
     ),
     source: str = typer.Argument(..., help="The source path (can be relative)."),
     destination_directory: str = typer.Argument(
         ..., help="The absolute destination path."
     ),
     filename: Optional[str] = typer.Argument(
         None,
-        help="The name of the file in the machine (by default it will be same as the local file).",
+        help="The name of the file in the machine (by default it will be same as the local file). It works only for a direct upload.",
     ),
     transfer_type: TransferType = typer.Option(
         TransferType.direct,
         "--type",
         case_sensitive=False,
-        help=f"Select type of transfer (run `{__app_name__} upload --help` for details).",
+        help=f"Select type of transfer.",
     ),
 ):
     """Upload a file
+
+    Direct upload will upload the file to the DESTINATION directory but it will work only for small files.
+    You can find the maximum size in UTILITIES_MAX_FILE_SIZE by running the `parameters` command.
+
+    External download will return with a command that will need to be run in case of success.
+    The file can be uploaded to a stage area without any authentication and FirecREST will move the file to the cluster's filesystem as soon as it finished.
     """
     try:
         if transfer_type == TransferType.direct:
             client.simple_upload(machine, source, destination_directory, filename)
         elif transfer_type == TransferType.external:
             up_obj = client.external_upload(machine, source, destination_directory)
             console.print(
@@ -617,47 +679,52 @@
                 "Waiting for Presigned URL to upload file to staging "
                 "area... It is safe to cancel the command and follow "
                 "up through the task."
             ):
                 data = up_obj.object_storage_data
                 if "command" in data:
                     console.print(
-                        "\nRun the following the following command to finish the upload:"
+                        "\nNecessary information to upload the file in the staging area:"
                     )
-                    console.out(data["command"])
+                    console.print(f"[yellow]{data['parameters']}[/yellow]")
                     console.print(
-                        "\nYou can also use a different software to upload the file:"
+                        "\nOr simply run the following command to finish the upload:"
                     )
-                    console.print(f"[yellow]{data['parameters']}[/yellow]")
+                    console.print(f"[green]{data['command']}[/green]")
                 else:
                     console.print(data)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Compute commands")
 def submit(
     machine: str = typer.Argument(
         ..., help="The machine name where the source filesystem belongs to."
     ),
     job_script: str = typer.Argument(
         ...,
         help="The path of the script (if it's local it can be relative path, if it is on the machine it has to be the absolute path)",
     ),
+    account: Optional[str] = typer.Option(
+        None,
+        "--account",
+        help="Charge resources used by this job to specified account.",
+    ),
     local: Optional[bool] = typer.Option(
         True,
         help="The batch file can be local (default) or on the machine's filesystem.",
     ),
 ):
     """Submit a batch script to the workload manger of the target system
     """
     try:
-        console.print(client.submit(machine, job_script, local))
-    except fc.FirecrestException as e:
+        console.print(client.submit(machine, job_script, local, account=account))
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @submit_template_app.command("mv")
 def submit_mv(
     machine: str = typer.Argument(
@@ -689,15 +756,15 @@
     """
     try:
         console.print(
             client.submit_move_job(
                 machine, source, destination, job_name, time, jobid, account
             )
         )
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @submit_template_app.command("cp")
 def submit_cp(
     machine: str = typer.Argument(
@@ -729,15 +796,15 @@
     """
     try:
         console.print(
             client.submit_copy_job(
                 machine, source, destination, job_name, time, jobid, account
             )
         )
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @submit_template_app.command("rsync")
 def submit_rsync(
     machine: str = typer.Argument(
@@ -769,15 +836,15 @@
     """
     try:
         console.print(
             client.submit_rsync_job(
                 machine, source, destination, job_name, time, jobid, account
             )
         )
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @submit_template_app.command("rm")
 def submit_rm(
     machine: str = typer.Argument(
@@ -806,15 +873,15 @@
 ):
     """Remove files
     """
     try:
         console.print(
             client.submit_delete_job(machine, path, job_name, time, jobid, account)
         )
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Compute commands")
 def poll(
     machine: str = typer.Argument(
@@ -852,15 +919,15 @@
                 ("Start time", "start_time"),
                 ("State", "state"),
                 ("Time", "time"),
                 ("Time left", "time_left"),
                 ("User", "user"),
             )
             console.print(table)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Compute commands")
 def poll_active(
     machine: str = typer.Argument(
@@ -890,15 +957,15 @@
                 ("Start time", "start_time"),
                 ("State", "state"),
                 ("Time", "time"),
                 ("Time left", "time_left"),
                 ("User", "user"),
             )
             console.print(table)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.command(rich_help_panel="Compute commands")
 def cancel(
     machine: str = typer.Argument(
@@ -906,15 +973,15 @@
     ),
     job: str = typer.Argument(..., help="The ID of the job that will be cancelled."),
 ):
     """Cancel job
     """
     try:
         client.cancel(machine, job)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @reservation_app.command(rich_help_panel="Reservation commands")
 def list(
     machine: str = typer.Argument(
@@ -922,15 +989,15 @@
     )
 ):
     """List all active reservations and their status
     """
     try:
         res = client.all_reservations(machine)
         console.print(res)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @reservation_app.command(rich_help_panel="Reservation commands")
 def create(
     machine: str = typer.Argument(
@@ -953,15 +1020,15 @@
 ):
     """Create a reservation
     """
     try:
         client.create_reservation(
             machine, name, account, num_nodes, node_type, start_time, end_time
         )
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @reservation_app.command(rich_help_panel="Reservation commands")
 def update(
     machine: str = typer.Argument(
@@ -984,15 +1051,15 @@
 ):
     """Update a reservation
     """
     try:
         client.update_reservation(
             machine, name, account, num_nodes, node_type, start_time, end_time
         )
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @reservation_app.command(rich_help_panel="Reservation commands")
 def delete(
     machine: str = typer.Argument(
@@ -1000,15 +1067,15 @@
     ),
     name: str = typer.Argument(..., help="The reservation name."),
 ):
     """Delete a reservation
     """
     try:
         client.delete_reservation(machine, name)
-    except fc.FirecrestException as e:
+    except Exception as e:
         examine_exeption(e)
         raise typer.Exit(code=1)
 
 
 @app.callback()
 def main(
     version: Optional[bool] = typer.Option(
@@ -1031,28 +1098,38 @@
         ...,
         help="URL of the token request in the authorization server (e.g. https://auth.com/auth/.../openid-connect/token).",
         envvar="AUTH_TOKEN_URL",
     ),
     verbose: Optional[bool] = typer.Option(
         None, "-v", "--verbose", help="Enable verbose mode."
     ),
+    timeout: Optional[float] = typer.Option(
+        None,
+        help="How many seconds to wait for the FirecREST server to send data before giving up.",
+    ),
+    auth_timeout: Optional[float] = typer.Option(
+        None,
+        help="How many seconds to wait for the authorization server to send data before giving up.",
+    ),
     debug: Optional[bool] = typer.Option(None, help="Enable debug mode."),
 ):
     """
     CLI for FirecREST
 
     Before running you need to setup the following variables or pass them as required options:
     - FIRECREST_URL: FirecREST URL
     - FIRECREST_CLIENT_ID: registered client ID
     - FIRECREST_CLIENT_SECRET: secret for the client
     - AUTH_TOKEN_URL: URL for the token request in the authorization server (e.g. https://auth.your-server.com/auth/.../openid-connect/token)
     """
     global client
     auth_obj = fc.ClientCredentialsAuth(client_id, client_secret, token_url)
+    auth_obj.timeout = auth_timeout
     client = fc.Firecrest(firecrest_url=firecrest_url, authorization=auth_obj)
+    client.timeout = timeout
     if debug:
         logging.basicConfig(
             level=logging.DEBUG,
             format="%(message)s",
             handlers=[RichHandler(console=console)],
         )
     elif verbose:
```

### Comparing `pyfirecrest-1.3.0/setup.py` & `pyfirecrest-1.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,92 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# PyFirecREST
 
-packages = \
-['firecrest', 'firecrest.cli']
+This is a simple python wrapper for the [FirecREST API](https://github.com/eth-cscs/firecrest).
 
-package_data = \
-{'': ['*']}
+### How to install
+- Through [PyPI](https://pypi.org/project/pyfirecrest/):
 
-install_requires = \
-['PyJWT>=2.4.0', 'requests>=2.14.0', 'typer[all]>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['firecrest = firecrest.cli_script:main']}
-
-setup_kwargs = {
-    'name': 'pyfirecrest',
-    'version': '1.3.0',
-    'description': 'pyFirecrest is a python wrapper for FirecREST',
-    'long_description': '# PyFirecREST\n\nThis is a simple python wrapper for the [FirecREST API](https://github.com/eth-cscs/firecrest).\n\n### How to install\n- Through [PyPI](https://pypi.org/project/pyfirecrest/):\n\n  ```\n  python3 -m pip install pyfirecrest\n  ```\n\n### How to use\nThe full documentation of pyFirecREST is in [this page](https://pyfirecrest.readthedocs.io) but you can get an idea from the following example.\nThis is how you can use the testbuild from the demo environment [here](https://github.com/eth-cscs/firecrest/tree/master/deploy/demo).\nThe configuration corresponds to the account `firecrest-sample`.\n\n```python\nimport firecrest as f7t\n\n# Configuration parameters for the Authorization Object\nclient_id = "firecrest-sample"\nclient_secret = "b391e177-fa50-4987-beaf-e6d33ca93571"\ntoken_uri = "http://localhost:8080/auth/realms/kcrealm/protocol/openid-connect/token"\n\n# Create an authorization object with Client Credentials authorization grant\nkeycloak = f7t.ClientCredentialsAuth(\n    client_id, client_secret, token_uri\n)\n\n# Setup the client for the specific account\nclient = f7t.Firecrest(\n    firecrest_url="http://localhost:8000", authorization=keycloak\n)\n\ntry:\n    parameters = client.parameters()\n    print(f"Firecrest parameters: {parameters}")\nexcept f7t.FirecrestException as e:\n    # When the error comes from the responses to a firecrest request you will get a\n    # `FirecrestException` and from this you can examine the http responses yourself\n    # through the `responses` property\n    print(e)\n    print(e.responses)\nexcept Exception as e:\n    # You might also get regular exceptions in some cases. For example when you are\n    # trying to upload a file that doesn\'t exist in your local filesystem.\n    pass\n```',
-    'author': 'CSCS',
-    'author_email': 'None',
-    'maintainer': 'Eirini Koutsaniti',
-    'maintainer_email': 'eirini.koutsaniti@cscs.ch',
-    'url': 'https://pyfirecrest.readthedocs.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+  ```
+  python3 -m pip install pyfirecrest
+  ```
+
+### How to use it as a python package
+The full documentation of pyFirecREST is in [this page](https://pyfirecrest.readthedocs.io) but you can get an idea from the following example.
+This is how you can use the testbuild from the demo environment [here](https://github.com/eth-cscs/firecrest/tree/master/deploy/demo).
+The configuration corresponds to the account `firecrest-sample`.
+
+```python
+import firecrest as f7t
+
+# Configuration parameters for the Authorization Object
+client_id = "firecrest-sample"
+client_secret = "b391e177-fa50-4987-beaf-e6d33ca93571"
+token_uri = "http://localhost:8080/auth/realms/kcrealm/protocol/openid-connect/token"
+
+# Create an authorization object with Client Credentials authorization grant
+keycloak = f7t.ClientCredentialsAuth(
+    client_id, client_secret, token_uri
+)
+
+# Setup the client for the specific account
+client = f7t.Firecrest(
+    firecrest_url="http://localhost:8000", authorization=keycloak
+)
+
+try:
+    parameters = client.parameters()
+    print(f"Firecrest parameters: {parameters}")
+except f7t.FirecrestException as e:
+    # When the error comes from the responses to a firecrest request you will get a
+    # `FirecrestException` and from this you can examine the http responses yourself
+    # through the `responses` property
+    print(e)
+    print(e.responses)
+except Exception as e:
+    # You might also get regular exceptions in some cases. For example when you are
+    # trying to upload a file that doesn't exist in your local filesystem.
+    pass
+```
+
+### How to use it from the terminal
+
+After version 1.3.0 pyFirecREST comes together with a CLI but for now it can only be used with the `f7t.ClientCredentialsAuth` authentication class.
+
+Assuming you are using the same client, you can start by setting as environment variables:
+```bash
+export FIRECREST_CLIENT_ID=firecrest-sample
+export FIRECREST_CLIENT_SECRET=b391e177-fa50-4987-beaf-e6d33ca93571
+export FIRECREST_URL=http://localhost:8000
+export AUTH_TOKEN_URL=http://localhost:8080/auth/realms/kcrealm/protocol/openid-connect/token
+```
+
+After that you can explore the capabilities of the CLI with the `--help` option:
+```bash
+firecrest --help
+firecrest ls --help
+firecrest submit --help
+firecrest upload --help
+firecrest download --help
+firecrest submit-template --help
+```
+
+Some basic examples:
+```bash
+# Get the available systems
+firecrest systems
+
+# Get the parameters of different microservices of FirecREST
+firecrest parameters
+
+# List files of directory
+firecrest ls cluster1 /home
+
+# Submit a job
+firecrest submit cluster script.sh
+
+# Upload a "small" file (you can check the maximum size in `UTILITIES_MAX_FILE_SIZE` from the `parameters` command)
+firecrest upload --type=direct cluster local_file.txt /path/to/cluster/fs
+
+# Upload a "large" file
+firecrest upload --type=external cluster local_file.txt /path/to/cluster/fs
+# You will have to finish the upload with a second command that will be given in the output
+```
```

