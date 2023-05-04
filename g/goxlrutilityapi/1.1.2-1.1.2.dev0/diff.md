# Comparing `tmp/goxlrutilityapi-1.1.2.tar.gz` & `tmp/goxlrutilityapi-1.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.1.2.tar", last modified: Sun Apr 30 20:07:42 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.1.2.dev0.tar", last modified: Thu May  4 20:38:39 2023, max compression
```

## Comparing `goxlrutilityapi-1.1.2.tar` & `goxlrutilityapi-1.1.2.dev0.tar`

### file list

```diff
@@ -1,28 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/map_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 20:07:42.000000 goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 20:07:42.758635 goxlrutilityapi-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 20:07:24.000000 goxlrutilityapi-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:38:39.971116 goxlrutilityapi-1.1.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 20:38:39.971116 goxlrutilityapi-1.1.2.dev0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:38:39.967115 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 20:38:38.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:38:39.967115 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:38:39.967115 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:38:39.967115 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/tests/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/tests/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/tests/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/tests/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/tests/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:38:39.971116 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/models/map_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:38:39.967115 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 20:38:39.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-04 20:38:39.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:38:39.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 20:38:39.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 20:38:39.000000 goxlrutilityapi-1.1.2.dev0/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 20:38:39.971116 goxlrutilityapi-1.1.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 20:38:04.000000 goxlrutilityapi-1.1.2.dev0/setup.py
```

### Comparing `goxlrutilityapi-1.1.2/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.2/goxlrutilityapi/const.py` & `goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/const.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.2/goxlrutilityapi/helper.py` & `goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/helpers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""GoXLR Utility API: Helper"""
+"""GoXLR Utility API: Helpers"""
 from __future__ import annotations
 
 import logging
 from typing import Optional
 
-from .const import VOLUME_MAX
-from .models.patch import Patch
-from .models.status import Mixer, Status
+from ..const import VOLUME_MAX
+from ..models.patch import Patch
+from ..models.status import Mixer, Status
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def get_mixer_from_status(status: Status) -> Optional[Mixer]:
     """Get first mixer from status"""
     return next(iter(status.mixers.values()), None)
```

### Comparing `goxlrutilityapi-1.1.2/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/models/status.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.2/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.1.2.dev0/goxlrutilityapi/websocket_client.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.2/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.1.2.dev0/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 setup.py
 goxlrutilityapi/__init__.py
 goxlrutilityapi/__main__.py
 goxlrutilityapi/_version.py
 goxlrutilityapi/base.py
 goxlrutilityapi/const.py
 goxlrutilityapi/exceptions.py
-goxlrutilityapi/helper.py
 goxlrutilityapi/logger.py
 goxlrutilityapi/websocket_client.py
 goxlrutilityapi.egg-info/PKG-INFO
 goxlrutilityapi.egg-info/SOURCES.txt
 goxlrutilityapi.egg-info/dependency_links.txt
 goxlrutilityapi.egg-info/requires.txt
 goxlrutilityapi.egg-info/top_level.txt
+goxlrutilityapi/helpers/__init__.py
+goxlrutilityapi/helpers/tests/__init__.py
+goxlrutilityapi/helpers/tests/models/__init__.py
+goxlrutilityapi/helpers/tests/models/map_item.py
+goxlrutilityapi/helpers/tests/models/patch.py
+goxlrutilityapi/helpers/tests/models/request.py
+goxlrutilityapi/helpers/tests/models/response.py
+goxlrutilityapi/helpers/tests/models/status.py
 goxlrutilityapi/models/__init__.py
 goxlrutilityapi/models/map_item.py
 goxlrutilityapi/models/patch.py
 goxlrutilityapi/models/request.py
 goxlrutilityapi/models/response.py
 goxlrutilityapi/models/status.py
```

### Comparing `goxlrutilityapi-1.1.2/pyproject.toml` & `goxlrutilityapi-1.1.2.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.1.2/setup.py` & `goxlrutilityapi-1.1.2.dev0/setup.py`

 * *Files identical despite different names*

