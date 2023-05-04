# Comparing `tmp/ikea_api-2.0.7.tar.gz` & `tmp/ikea_api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikea_api-2.0.7.tar", max compression
+gzip compressed data, was "ikea_api-2.1.0.tar", max compression
```

## Comparing `ikea_api-2.0.7.tar` & `ikea_api-2.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0     1081 2022-10-29 06:54:37.346727 ikea_api-2.0.7/LICENSE
--rw-r--r--   0        0        0     8486 2022-10-29 06:54:37.346727 ikea_api-2.0.7/README.md
--rw-r--r--   0        0        0     1808 2022-10-29 06:54:37.346727 ikea_api-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     2006 2022-10-29 06:54:37.346727 ikea_api-2.0.7/src/ikea_api/__init__.py
--rw-r--r--   0        0        0     3950 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/abc.py
--rw-r--r--   0        0        0      912 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/base_ikea_api.py
--rw-r--r--   0        0        0      853 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/constants.py
--rw-r--r--   0        0        0        0 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/__init__.py
--rw-r--r--   0        0        0     1017 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/auth.py
--rw-r--r--   0        0        0     8731 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/cart.py
--rw-r--r--   0        0        0     1357 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/ingka_items.py
--rw-r--r--   0        0        0     3116 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/iows_items.py
--rw-r--r--   0        0        0     3628 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/order_capture.py
--rw-r--r--   0        0        0     1213 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/pip_item.py
--rw-r--r--   0        0        0     8442 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/purchases.py
--rw-r--r--   0        0        0     1236 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/search.py
--rw-r--r--   0        0        0     1096 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/endpoints/stock.py
--rw-r--r--   0        0        0      940 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/error_handlers.py
--rw-r--r--   0        0        0     1250 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/executors/__init__.py
--rw-r--r--   0        0        0     2064 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/executors/httpx.py
--rw-r--r--   0        0        0     2003 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/executors/requests.py
--rw-r--r--   0        0        0        0 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/py.typed
--rw-r--r--   0        0        0     1960 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/utils.py
--rw-r--r--   0        0        0        0 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/__init__.py
--rw-r--r--   0        0        0        0 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/parsers/__init__.py
--rw-r--r--   0        0        0     4884 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/parsers/ingka_items.py
--rw-r--r--   0        0        0     6560 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/parsers/iows_items.py
--rw-r--r--   0        0        0      759 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/parsers/item_base.py
--rw-r--r--   0        0        0     7707 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/parsers/order_capture.py
--rw-r--r--   0        0        0     1177 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/parsers/pip_item.py
--rw-r--r--   0        0        0     2757 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/parsers/purchases.py
--rw-r--r--   0        0        0     1625 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/types.py
--rw-r--r--   0        0        0     7467 2022-10-29 06:54:37.350727 ikea_api-2.0.7/src/ikea_api/wrappers/wrappers.py
--rw-r--r--   0        0        0     9866 1970-01-01 00:00:00.000000 ikea_api-2.0.7/setup.py
--rw-r--r--   0        0        0     9758 1970-01-01 00:00:00.000000 ikea_api-2.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1081 2023-05-04 15:43:16.205672 ikea_api-2.1.0/LICENSE
+-rw-r--r--   0        0        0     8646 2023-05-04 15:43:16.205672 ikea_api-2.1.0/README.md
+-rw-r--r--   0        0        0     1855 2023-05-04 15:43:43.122951 ikea_api-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2074 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/__init__.py
+-rw-r--r--   0        0        0     3950 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/abc.py
+-rw-r--r--   0        0        0      912 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/base_ikea_api.py
+-rw-r--r--   0        0        0      853 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/constants.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/__init__.py
+-rw-r--r--   0        0        0     1017 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/auth.py
+-rw-r--r--   0        0        0     8731 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/cart.py
+-rw-r--r--   0        0        0     1357 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/ingka_items.py
+-rw-r--r--   0        0        0     3116 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/iows_items.py
+-rw-r--r--   0        0        0     3628 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/order_capture.py
+-rw-r--r--   0        0        0     1213 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/pip_item.py
+-rw-r--r--   0        0        0     8442 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/purchases.py
+-rw-r--r--   0        0        0      934 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/rotera_item.py
+-rw-r--r--   0        0        0     1236 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/search.py
+-rw-r--r--   0        0        0     1096 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/endpoints/stock.py
+-rw-r--r--   0        0        0      940 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/error_handlers.py
+-rw-r--r--   0        0        0     1250 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/executors/__init__.py
+-rw-r--r--   0        0        0     2064 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/executors/httpx.py
+-rw-r--r--   0        0        0     2003 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/executors/requests.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/py.typed
+-rw-r--r--   0        0        0     1960 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/utils.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/parsers/__init__.py
+-rw-r--r--   0        0        0     4884 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/parsers/ingka_items.py
+-rw-r--r--   0        0        0     6560 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/parsers/iows_items.py
+-rw-r--r--   0        0        0      759 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/parsers/item_base.py
+-rw-r--r--   0        0        0     7753 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/parsers/order_capture.py
+-rw-r--r--   0        0        0     1177 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/parsers/pip_item.py
+-rw-r--r--   0        0        0     2757 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/parsers/purchases.py
+-rw-r--r--   0        0        0     1625 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/types.py
+-rw-r--r--   0        0        0     7467 2023-05-04 15:43:16.205672 ikea_api-2.1.0/src/ikea_api/wrappers/wrappers.py
+-rw-r--r--   0        0        0     9918 1970-01-01 00:00:00.000000 ikea_api-2.1.0/PKG-INFO
```

### Comparing `ikea_api-2.0.7/LICENSE` & `ikea_api-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/README.md` & `ikea_api-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Features
 
 With this library you can access following IKEA's APIs:
 
 - Cart,
 - Home Delivery and Collect Services (actually, Order Capture),
 - Items info (3 different services),
+- 3D models,
 - Purchases (history and order info),
 - Search,
 - Stock.
 
 Also the package:
 
 - Is **backend agnostic**: choose HTTP library you want (async, too!),
@@ -268,14 +269,23 @@
 
 > 💡 You probably won't want to use raw APIs when there's convenient "smart" wrapper that combines them all and parses basic info:
 >
 > ```python
 > ikea_api.get_items(["30457903"])
 > ```
 
+### 📦 Item 3D models
+
+Get 3D models by item code.
+
+```python
+rotera_item = ikea_api.RoteraItem(constants)
+rotera_item.get_item("30221043")
+```
+
 ### 🟢 Item availability
 
 Get availability by item code (product number or whatever).
 
 ```python
 stock = ikea_api.Stock(constants)
 stock.get_stock("30457903")
```

### Comparing `ikea_api-2.0.7/pyproject.toml` & `ikea_api-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ikea_api"
-version = "0"
+version = "2.1.0"
 description = "Client for several IKEA's APIs"
 authors = ["Lev Vereshchagin <mail@vrslev.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/vrslev/ikea-api-client"
 keywords = ["ikea", "ikea api", "api", "api client"]
 classifiers = [
@@ -16,35 +16,35 @@
 include = ["src/ikea_api/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typing-extensions = {version = "^4.0.0", python = "<3.10"}
 requests = {version = "*", optional = true}
 pydantic = {version = "^1.8.0", optional = true}
-httpx = {version = "^0.22.0", optional = true}
+httpx = {version = ">=0.22,<0.25", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = "7.1.3"
-pytest-asyncio = "0.19.0"
-pytest-cov = "3.0.0"
-black = {version = "22.8.0"}
-pre-commit = "2.20.0"
+pytest = "7.3.1"
+pytest-asyncio = "0.21.0"
+pytest-cov = "4.0.0"
+black = {version = "23.3.0"}
+pre-commit = "3.2.2"
 
 [tool.poetry.extras]
 wrappers = ["pydantic"]
 requests = ["requests"]
 httpx = ["httpx"]
 all = ["pydantic", "requests", "httpx"]
 
-[tool.poetry-version-plugin]
-source = "git-tag"
+[tool.poetry-dynamic-versioning]
+enable = false
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 target-version = ["py38", "py39", "py310"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `ikea_api-2.0.7/src/ikea_api/__init__.py` & `ikea_api-2.1.0/src/ikea_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from ikea_api.endpoints.iows_items import IowsItems as IowsItems
 from ikea_api.endpoints.order_capture import OrderCapture as OrderCapture
 from ikea_api.endpoints.order_capture import (
     convert_cart_to_checkout_items as convert_cart_to_checkout_items,
 )
 from ikea_api.endpoints.pip_item import PipItem as PipItem
 from ikea_api.endpoints.purchases import Purchases as Purchases
+from ikea_api.endpoints.rotera_item import RoteraItem as RoteraItem
 from ikea_api.endpoints.search import Search as Search
 from ikea_api.endpoints.stock import Stock as Stock
 from ikea_api.exceptions import APIError as APIError
 from ikea_api.exceptions import AuthError as AuthError
 from ikea_api.exceptions import GraphQLError as GraphQLError
 from ikea_api.exceptions import ItemFetchError as ItemFetchError
 from ikea_api.exceptions import JSONError as JSONError
```

### Comparing `ikea_api-2.0.7/src/ikea_api/abc.py` & `ikea_api-2.1.0/src/ikea_api/abc.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/base_ikea_api.py` & `ikea_api-2.1.0/src/ikea_api/base_ikea_api.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/constants.py` & `ikea_api-2.1.0/src/ikea_api/constants.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/endpoints/auth.py` & `ikea_api-2.1.0/src/ikea_api/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/endpoints/cart.py` & `ikea_api-2.1.0/src/ikea_api/endpoints/cart.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/endpoints/ingka_items.py` & `ikea_api-2.1.0/src/ikea_api/endpoints/ingka_items.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/endpoints/iows_items.py` & `ikea_api-2.1.0/src/ikea_api/endpoints/iows_items.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/endpoints/order_capture.py` & `ikea_api-2.1.0/src/ikea_api/endpoints/order_capture.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/endpoints/pip_item.py` & `ikea_api-2.1.0/src/ikea_api/endpoints/pip_item.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/endpoints/purchases.py` & `ikea_api-2.1.0/src/ikea_api/endpoints/purchases.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/endpoints/search.py` & `ikea_api-2.1.0/src/ikea_api/endpoints/search.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/endpoints/stock.py` & `ikea_api-2.1.0/src/ikea_api/endpoints/stock.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/error_handlers.py` & `ikea_api-2.1.0/src/ikea_api/error_handlers.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/exceptions.py` & `ikea_api-2.1.0/src/ikea_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/executors/httpx.py` & `ikea_api-2.1.0/src/ikea_api/executors/httpx.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/executors/requests.py` & `ikea_api-2.1.0/src/ikea_api/executors/requests.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/utils.py` & `ikea_api-2.1.0/src/ikea_api/utils.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/wrappers/parsers/ingka_items.py` & `ikea_api-2.1.0/src/ikea_api/wrappers/parsers/ingka_items.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/wrappers/parsers/iows_items.py` & `ikea_api-2.1.0/src/ikea_api/wrappers/parsers/iows_items.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/wrappers/parsers/item_base.py` & `ikea_api-2.1.0/src/ikea_api/wrappers/parsers/item_base.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/wrappers/parsers/order_capture.py` & `ikea_api-2.1.0/src/ikea_api/wrappers/parsers/order_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any, List, Optional
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, validator  # pyright: ignore[reportUnknownVariableType]
 
 from ikea_api.constants import Constants
 from ikea_api.utils import translate_from_dict
 from ikea_api.wrappers import types
 from ikea_api.wrappers.parsers.item_base import ItemCode
 
 DELIVERY_TYPES = {
```

### Comparing `ikea_api-2.0.7/src/ikea_api/wrappers/parsers/pip_item.py` & `ikea_api-2.1.0/src/ikea_api/wrappers/parsers/pip_item.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/wrappers/parsers/purchases.py` & `ikea_api-2.1.0/src/ikea_api/wrappers/parsers/purchases.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/wrappers/types.py` & `ikea_api-2.1.0/src/ikea_api/wrappers/types.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/src/ikea_api/wrappers/wrappers.py` & `ikea_api-2.1.0/src/ikea_api/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `ikea_api-2.0.7/setup.py` & `ikea_api-2.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,364 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ikea-api
+Version: 2.1.0
+Summary: Client for several IKEA's APIs
+Home-page: https://github.com/vrslev/ikea-api-client
+License: MIT
+Keywords: ikea,ikea api,api,api client
+Author: Lev Vereshchagin
+Author-email: mail@vrslev.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Provides-Extra: all
+Provides-Extra: httpx
+Provides-Extra: requests
+Provides-Extra: wrappers
+Requires-Dist: httpx (>=0.22,<0.25) ; extra == "httpx" or extra == "all"
+Requires-Dist: pydantic (>=1.8.0,<2.0.0) ; extra == "wrappers" or extra == "all"
+Requires-Dist: requests ; extra == "requests" or extra == "all"
+Requires-Dist: typing-extensions (>=4.0.0,<5.0.0) ; python_version < "3.10"
+Project-URL: Repository, https://github.com/vrslev/ikea-api-client
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+Client for several IKEA APIs.
 
-packages = \
-['ikea_api',
- 'ikea_api.endpoints',
- 'ikea_api.executors',
- 'ikea_api.wrappers',
- 'ikea_api.wrappers.parsers']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{':python_version < "3.10"': ['typing-extensions>=4.0.0,<5.0.0'],
- 'all': ['requests', 'pydantic>=1.8.0,<2.0.0', 'httpx>=0.22.0,<0.23.0'],
- 'httpx': ['httpx>=0.22.0,<0.23.0'],
- 'requests': ['requests'],
- 'wrappers': ['pydantic>=1.8.0,<2.0.0']}
-
-setup_kwargs = {
-    'name': 'ikea-api',
-    'version': '2.0.7',
-    'description': "Client for several IKEA's APIs",
-    'long_description': 'Client for several IKEA APIs.\n\n[![Test](https://github.com/vrslev/ikea-api-client/actions/workflows/test.yml/badge.svg)](https://github.com/vrslev/ikea-api-client/actions/workflows/test.yml)\n[![Python](https://img.shields.io/pypi/pyversions/ikea_api?label=Python)](https://pypi.org/project/ikea_api)\n[![Downloads](https://img.shields.io/pypi/dm/ikea_api?label=Downloads&color=blueviolet)](https://pypi.org/project/ikea_api)\n\n# Features\n\nWith this library you can access following IKEA\'s APIs:\n\n- Cart,\n- Home Delivery and Collect Services (actually, Order Capture),\n- Items info (3 different services),\n- Purchases (history and order info),\n- Search,\n- Stock.\n\nAlso the package:\n\n- Is **backend agnostic**: choose HTTP library you want (async, too!),\n- Is **fully typed and tested**,\n- Has optional wrappers around some APIs based on Pydantic.\n\n# Installation\n\n```bash\npip install ikea_api\n```\n\n- Use [httpx](https://www.python-httpx.org) — awesome async HTTP library —\xa0as backend:\n\n```bash\npip install "ikea_api[httpx]"\n```\n\n- Use [requests](https://docs.python-requests.org)\xa0as backend:\n\n```bash\npip install "ikea_api[requests]"\n```\n\n- Use wrappers:\n\n```bash\npip install "ikea_api[wrappers]"\n```\n\n- Install everything:\n\n```bash\npip install "ikea_api[all]"\n```\n\n# Usage\n\n_ikea_api_ is unusual API client. It decouples I/O from logic for easier testing and maintenance. As a bonus, you can use literally _any_ HTTP library.\nLet\'s have a look at how to work with ikea_api.\n\n```python\nimport ikea_api\n\n# Constants like country, language, base url\nconstants = ikea_api.Constants(country="us", language="en")\n# Search API\nsearch = ikea_api.Search(constants)\n# Search endpoint with prepared data\nendpoint = search.search("Billy")\n```\n\nAs you can see, nothing happened up to this point. Code suggests that we already should get the result of the search but we don\'t. What happened is `search()` returned a data class that contains information about endpoint that can be interpreted by an endpoint runner. There are two built-in: for [requests](https://docs.python-requests.org) (sync) and [httpx](https://www.python-httpx.org) (async), but you can easily write one yourself.\n\nHere\'s how you would use _requests_ one:\n\n```python\nikea_api.run(endpoint)\n```\n\nAnd _httpx_ one:\n\n```python\nawait ikea_api.run_async(endpoint)\n```\n\n`ikea_api.run_async()` is async function, so you have to "await" it or run using `asyncio.run()`.\n\n## Endpoints reference\n\n### 🔑 Authorization\n\nFirst time you open ikea.com, guest token is being generated and stored in cookies. Same thing must be done in here before using any endpoint.\n\nThis token expires in 30 days.\n\n```python\nikea_api.Auth(constants).get_guest_token()\n```\n\nPreviously you could login as user (with login and password), but now there\'s very advanced telemetry that I wouldn\'t be able to solve in hundred years 🤪\n\n### 🛒 Cart\n\nWith this endpoint you can do everything you can using IKEA\'s frontend:\n\n```python\ncart = ikea_api.Cart(constants, token=...)\n```\n\n- Show the cart\n\n```python\ncart.show()\n```\n\n- Clear it\n\n```python\ncart.clear()\n```\n\n- Add, update and delete items\n\n```python\ncart.add_items({"30457903": 1})  # { item_code: quantity }\n\ncart.update_items({"30457903": 5})\n\ncart.remove_items(["30457903"])\n```\n\n- Set and clear coupon\n\n```python\ncart.set_coupon(...)\n\ncart.clear_coupon()\n```\n\n- and even copy another user\'s cart.\n\n```python\ncart.copy_items(source_user_id=...)\n```\n\nYou can edit your user\'s actual cart if you use authorized token (copy-paste from cookies).\n\n> 💡\xa0There\'s wrapper that clears current cart and adds items with error handling: if requested item doesn\'t exist, the function just skips it and tries again.\n>\n> ```python\n> ikea_api.add_items_to_cart(  # Function returns items that can\'t be added. In this case: [\'11111111\']\n>     cart=cart,\n>     items={\n>         "30457903": 1,\n>         "11111111": 2,  # invalid item that will be skipped\n>     },\n> )\n> ```\n\n### 🚛 Order Capture\n\nCheck pickup or delivery availability. If you need to know whether items are available _in stores_, use [Item availability endpoint](#%F0%9F%9F%A2-item-availability) or [ikea-availability-checker](https://github.com/Ephigenia/ikea-availability-checker).\n\n```python\norder = ikea_api.OrderCapture(constants, token=token)\n\ncart_show = run(cart.show())\nitems = ikea_api.convert_cart_to_checkout_items(cart_show)\n\ncheckout_id = run(order.get_checkout(items))\nservice_area_id = run(\n    order.get_service_area(\n        checkout_id,\n        zip_code="02215",\n        state_code="MA",  # pass State Code only if your country has them\n    )\n)\nhome_services = run(order.get_home_delivery_services(checkout_id, service_area_id))\ncollect_services = run(\n    order.get_collect_delivery_services(checkout_id, service_area_id)\n)\n```\n\n> 💡\xa0You can use wrapper to add items to cart (clearing cart before and handling unknown item errors if they appear) and parse response in nice Pydantic models:\n>\n> ```python\n> services = await ikea_api.get_delivery_services(\n>     constants=constants,\n>     token=...,\n>     items={\n>         "30457903": 1,\n>         "11111111": 2,  # invalid item that will be skipped\n>     },\n>     zip_code="101000",\n> )\n> services.delivery_options  # List of parsed delivery services\n> services.cannot_add  # [\'11111111\']\n> ```\n\n### 📦 Purchases\n\n```python\npurchases = ikea_api.Purchases(constants, token=token)\n```\n\n#### History\n\nThis method requires authentication, so if you don\'t have authorized token, it won\'t work.\n\n```python\npurchases.history()\n\n# Get all purchases:\npurchases.history(take=10000)\n\n# Pagination:\npurchases.history(take=10, skip=1)\n```\n\n> 💡 Get parsed response with the wrapper:\n>\n> ```python\n> ikea_api.get_purchase_history(purchases)  # Returns a list of parsed purchases\n> ```\n\n#### Order info\n\n```python\npurchases.order_info(order_number=..., email=...)\n\n# If you have authorized token, you can drop email:\npurchases.order_info(order_number="111111111")\n\n# The method also has other params but they\'re mostly internal:\npurchases.order_info(\n    order_number=...,\n    email=...,\n    queries=...,  # Queries that will be included in request, combine any of: ["StatusBannerOrder", "CostsOrder", "ProductListOrder"]. By default, all of them are included.\n    # Params below are relevant to ProductListOrder\n    skip_products=...,\n    skip_product_prices=...,\n    take_products=...,\n)\n```\n\n> 💡 Get parsed response with the wrapper:\n>\n> ```python\n> ikea_api.get_purchase_info(  # Returns parsed purchase object. Items are not listed.\n>    purchases=purchases,\n>    order_number=...,\n>    email=...,\n> )\n> ```\n\n### 🪑 Item info\n\nGet item specification by item code (product number or whatever). There are 3 endpoints to do this because you can\'t get all the data about all the items using only one endpoint.\n\n```python\niows_items = ikea_api.IowsItems(constants)\niows_items.get_items(["30457903"])\n\ningka_items = ikea_api.IngkaItems(constants)\ningka_items.get_items(["30457903"])\n\npip_item = ikea_api.PipItem(constants)\npip_item.get_item("30457903")\n```\n\n> 💡 You probably won\'t want to use raw APIs when there\'s convenient "smart" wrapper that combines them all and parses basic info:\n>\n> ```python\n> ikea_api.get_items(["30457903"])\n> ```\n\n### 🟢 Item availability\n\nGet availability by item code (product number or whatever).\n\n```python\nstock = ikea_api.Stock(constants)\nstock.get_stock("30457903")\n```\n\n### 🔎 Search\n\nSearch for products in the product catalog by product name. Optionally also specify a maximum amount of returned search results (defaults to 24) and types of required search results.\n\n```python\nsearch = ikea_api.Search(constants)\nsearch.search("Billy")\n\n# Retrieve 10 search results (default is 24)\nsearch.search("Billy", limit=10)\n\n# Configure search results types\nsearch.search(\n    "Billy",\n    types=...,  # Combine any of: ["PRODUCT", "CONTENT", "PLANNER", "REFINED_SEARCHES", "ANSWER"]\n)\n```\n\n### 🛠 Utilities\n\n#### Parse item codes\n\nParse item codes from string or list.\n\n```python\nassert ikea_api.parse_item_codes("111.111.11") == ["11111111"]\nassert ikea_api.parse_item_codes("11111111, 222.222.22") == ["11111111", "22222222"]\nassert ikea_api.parse_item_codes("111") == []\n```\n\n#### Format item code\n\nParse item code and format it.\n\n```python\nassert ikea_api.format_item_code("11111111") == "111.111.11"\nassert ikea_api.format_item_code("111-111-11") == "111.111.11"\nassert ikea_api.format_item_code("111.111.11") == "111.111.11"\n```\n',
-    'author': 'Lev Vereshchagin',
-    'author_email': 'mail@vrslev.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/vrslev/ikea-api-client',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
+[![Test](https://github.com/vrslev/ikea-api-client/actions/workflows/test.yml/badge.svg)](https://github.com/vrslev/ikea-api-client/actions/workflows/test.yml)
+[![Python](https://img.shields.io/pypi/pyversions/ikea_api?label=Python)](https://pypi.org/project/ikea_api)
+[![Downloads](https://img.shields.io/pypi/dm/ikea_api?label=Downloads&color=blueviolet)](https://pypi.org/project/ikea_api)
 
+# Features
+
+With this library you can access following IKEA's APIs:
+
+- Cart,
+- Home Delivery and Collect Services (actually, Order Capture),
+- Items info (3 different services),
+- 3D models,
+- Purchases (history and order info),
+- Search,
+- Stock.
+
+Also the package:
+
+- Is **backend agnostic**: choose HTTP library you want (async, too!),
+- Is **fully typed and tested**,
+- Has optional wrappers around some APIs based on Pydantic.
+
+# Installation
+
+```bash
+pip install ikea_api
+```
+
+- Use [httpx](https://www.python-httpx.org) — awesome async HTTP library — as backend:
+
+```bash
+pip install "ikea_api[httpx]"
+```
+
+- Use [requests](https://docs.python-requests.org) as backend:
+
+```bash
+pip install "ikea_api[requests]"
+```
+
+- Use wrappers:
+
+```bash
+pip install "ikea_api[wrappers]"
+```
+
+- Install everything:
+
+```bash
+pip install "ikea_api[all]"
+```
+
+# Usage
+
+_ikea_api_ is unusual API client. It decouples I/O from logic for easier testing and maintenance. As a bonus, you can use literally _any_ HTTP library.
+Let's have a look at how to work with ikea_api.
+
+```python
+import ikea_api
+
+# Constants like country, language, base url
+constants = ikea_api.Constants(country="us", language="en")
+# Search API
+search = ikea_api.Search(constants)
+# Search endpoint with prepared data
+endpoint = search.search("Billy")
+```
+
+As you can see, nothing happened up to this point. Code suggests that we already should get the result of the search but we don't. What happened is `search()` returned a data class that contains information about endpoint that can be interpreted by an endpoint runner. There are two built-in: for [requests](https://docs.python-requests.org) (sync) and [httpx](https://www.python-httpx.org) (async), but you can easily write one yourself.
+
+Here's how you would use _requests_ one:
+
+```python
+ikea_api.run(endpoint)
+```
+
+And _httpx_ one:
+
+```python
+await ikea_api.run_async(endpoint)
+```
+
+`ikea_api.run_async()` is async function, so you have to "await" it or run using `asyncio.run()`.
+
+## Endpoints reference
+
+### 🔑 Authorization
+
+First time you open ikea.com, guest token is being generated and stored in cookies. Same thing must be done in here before using any endpoint.
+
+This token expires in 30 days.
+
+```python
+ikea_api.Auth(constants).get_guest_token()
+```
+
+Previously you could login as user (with login and password), but now there's very advanced telemetry that I wouldn't be able to solve in hundred years 🤪
+
+### 🛒 Cart
+
+With this endpoint you can do everything you can using IKEA's frontend:
+
+```python
+cart = ikea_api.Cart(constants, token=...)
+```
+
+- Show the cart
+
+```python
+cart.show()
+```
+
+- Clear it
+
+```python
+cart.clear()
+```
+
+- Add, update and delete items
+
+```python
+cart.add_items({"30457903": 1})  # { item_code: quantity }
+
+cart.update_items({"30457903": 5})
+
+cart.remove_items(["30457903"])
+```
+
+- Set and clear coupon
+
+```python
+cart.set_coupon(...)
+
+cart.clear_coupon()
+```
+
+- and even copy another user's cart.
+
+```python
+cart.copy_items(source_user_id=...)
+```
+
+You can edit your user's actual cart if you use authorized token (copy-paste from cookies).
+
+> 💡 There's wrapper that clears current cart and adds items with error handling: if requested item doesn't exist, the function just skips it and tries again.
+>
+> ```python
+> ikea_api.add_items_to_cart(  # Function returns items that can't be added. In this case: ['11111111']
+>     cart=cart,
+>     items={
+>         "30457903": 1,
+>         "11111111": 2,  # invalid item that will be skipped
+>     },
+> )
+> ```
+
+### 🚛 Order Capture
+
+Check pickup or delivery availability. If you need to know whether items are available _in stores_, use [Item availability endpoint](#%F0%9F%9F%A2-item-availability) or [ikea-availability-checker](https://github.com/Ephigenia/ikea-availability-checker).
+
+```python
+order = ikea_api.OrderCapture(constants, token=token)
+
+cart_show = run(cart.show())
+items = ikea_api.convert_cart_to_checkout_items(cart_show)
+
+checkout_id = run(order.get_checkout(items))
+service_area_id = run(
+    order.get_service_area(
+        checkout_id,
+        zip_code="02215",
+        state_code="MA",  # pass State Code only if your country has them
+    )
+)
+home_services = run(order.get_home_delivery_services(checkout_id, service_area_id))
+collect_services = run(
+    order.get_collect_delivery_services(checkout_id, service_area_id)
+)
+```
+
+> 💡 You can use wrapper to add items to cart (clearing cart before and handling unknown item errors if they appear) and parse response in nice Pydantic models:
+>
+> ```python
+> services = await ikea_api.get_delivery_services(
+>     constants=constants,
+>     token=...,
+>     items={
+>         "30457903": 1,
+>         "11111111": 2,  # invalid item that will be skipped
+>     },
+>     zip_code="101000",
+> )
+> services.delivery_options  # List of parsed delivery services
+> services.cannot_add  # ['11111111']
+> ```
+
+### 📦 Purchases
+
+```python
+purchases = ikea_api.Purchases(constants, token=token)
+```
+
+#### History
+
+This method requires authentication, so if you don't have authorized token, it won't work.
+
+```python
+purchases.history()
+
+# Get all purchases:
+purchases.history(take=10000)
+
+# Pagination:
+purchases.history(take=10, skip=1)
+```
+
+> 💡 Get parsed response with the wrapper:
+>
+> ```python
+> ikea_api.get_purchase_history(purchases)  # Returns a list of parsed purchases
+> ```
+
+#### Order info
+
+```python
+purchases.order_info(order_number=..., email=...)
+
+# If you have authorized token, you can drop email:
+purchases.order_info(order_number="111111111")
+
+# The method also has other params but they're mostly internal:
+purchases.order_info(
+    order_number=...,
+    email=...,
+    queries=...,  # Queries that will be included in request, combine any of: ["StatusBannerOrder", "CostsOrder", "ProductListOrder"]. By default, all of them are included.
+    # Params below are relevant to ProductListOrder
+    skip_products=...,
+    skip_product_prices=...,
+    take_products=...,
+)
+```
+
+> 💡 Get parsed response with the wrapper:
+>
+> ```python
+> ikea_api.get_purchase_info(  # Returns parsed purchase object. Items are not listed.
+>    purchases=purchases,
+>    order_number=...,
+>    email=...,
+> )
+> ```
+
+### 🪑 Item info
+
+Get item specification by item code (product number or whatever). There are 3 endpoints to do this because you can't get all the data about all the items using only one endpoint.
+
+```python
+iows_items = ikea_api.IowsItems(constants)
+iows_items.get_items(["30457903"])
+
+ingka_items = ikea_api.IngkaItems(constants)
+ingka_items.get_items(["30457903"])
+
+pip_item = ikea_api.PipItem(constants)
+pip_item.get_item("30457903")
+```
+
+> 💡 You probably won't want to use raw APIs when there's convenient "smart" wrapper that combines them all and parses basic info:
+>
+> ```python
+> ikea_api.get_items(["30457903"])
+> ```
+
+### 📦 Item 3D models
+
+Get 3D models by item code.
+
+```python
+rotera_item = ikea_api.RoteraItem(constants)
+rotera_item.get_item("30221043")
+```
+
+### 🟢 Item availability
+
+Get availability by item code (product number or whatever).
+
+```python
+stock = ikea_api.Stock(constants)
+stock.get_stock("30457903")
+```
+
+### 🔎 Search
+
+Search for products in the product catalog by product name. Optionally also specify a maximum amount of returned search results (defaults to 24) and types of required search results.
+
+```python
+search = ikea_api.Search(constants)
+search.search("Billy")
+
+# Retrieve 10 search results (default is 24)
+search.search("Billy", limit=10)
+
+# Configure search results types
+search.search(
+    "Billy",
+    types=...,  # Combine any of: ["PRODUCT", "CONTENT", "PLANNER", "REFINED_SEARCHES", "ANSWER"]
+)
+```
+
+### 🛠 Utilities
+
+#### Parse item codes
+
+Parse item codes from string or list.
+
+```python
+assert ikea_api.parse_item_codes("111.111.11") == ["11111111"]
+assert ikea_api.parse_item_codes("11111111, 222.222.22") == ["11111111", "22222222"]
+assert ikea_api.parse_item_codes("111") == []
+```
+
+#### Format item code
+
+Parse item code and format it.
+
+```python
+assert ikea_api.format_item_code("11111111") == "111.111.11"
+assert ikea_api.format_item_code("111-111-11") == "111.111.11"
+assert ikea_api.format_item_code("111.111.11") == "111.111.11"
+```
 
-setup(**setup_kwargs)
```

