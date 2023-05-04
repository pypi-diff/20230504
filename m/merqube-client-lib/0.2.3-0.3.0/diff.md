# Comparing `tmp/merqube_client_lib-0.2.3.tar.gz` & `tmp/merqube_client_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.2.3.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.3.0.tar", max compression
```

## Comparing `merqube_client_lib-0.2.3.tar` & `merqube_client_lib-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/LICENSE
--rw-r--r--   0        0        0      377 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0      207 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/py.typed
--rw-r--r--   0        0        0    10941 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/session.py
--rw-r--r--   0        0        0      351 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/merqube_client_lib/types.py
--rw-r--r--   0        0        0     1677 2023-05-02 22:49:58.330060 merqube_client_lib-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/LICENSE
+-rw-r--r--   0        0        0      377 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0    10952 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      351 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/merqube_client_lib/types.py
+-rw-r--r--   0        0        0     1677 2023-05-03 13:45:54.098345 merqube_client_lib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.3.0/PKG-INFO
```

### Comparing `merqube_client_lib-0.2.3/LICENSE` & `merqube_client_lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.2.3/merqube_client_lib/session.py` & `merqube_client_lib-0.3.0/merqube_client_lib/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Merqube API Session - subcomponent of the client library wrapper
 """
 
 
 import json
-import logging
 import os
 import uuid
 from typing import Any, Optional, Union, cast
 from urllib.parse import urljoin
 
 from cachetools import LRUCache, cached
 from requests import PreparedRequest, Response, Session
@@ -18,19 +17,19 @@
 
 from merqube_client_lib.constants import (
     API_URL,
     MERQ_REQUEST_ID_ENV_VAR,
     REQUEST_ID_HEADER,
 )
 from merqube_client_lib.exceptions import APIError
+from merqube_client_lib.logging import get_module_logger
 from merqube_client_lib.types import HTTP_METHODS
 from merqube_client_lib.types import HTTPMethod as httpm
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+logger = get_module_logger(__name__)
 
 
 class TimeoutHTTPAdapter(HTTPAdapter):
     def __init__(self, timeout: int | None = None, **kwargs: Any):
         """
         Adapter to allow for setting timeouts on API calls.
         Timeout should be in seconds
```

### Comparing `merqube_client_lib-0.2.3/pyproject.toml` & `merqube_client_lib-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.2.3"
+version = "0.3.0"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
```

### Comparing `merqube_client_lib-0.2.3/PKG-INFO` & `merqube_client_lib-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merqube-client-lib
-Version: 0.2.3
+Version: 0.3.0
 Summary: MerQube IndexAPI + SecAPI client library
 Home-page: https://github.com/merqube/merqube-client-lib
 License: Apache-2.0
 Author: Merqube
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

