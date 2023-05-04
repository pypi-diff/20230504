# Comparing `tmp/lixinger-0.1.1.tar.gz` & `tmp/lixinger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixinger-0.1.1.tar", last modified: Wed May  3 10:12:07 2023, max compression
+gzip compressed data, was "lixinger-0.1.2.tar", last modified: Thu May  4 10:40:26 2023, max compression
```

## Comparing `lixinger-0.1.1.tar` & `lixinger-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      705 2023-05-03 10:11:52.615764 lixinger-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.1/lixinger/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.1/lixinger/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.1/lixinger/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.1/lixinger/api/cn/company/__init__.py
--rw-r--r--   0        0        0     2096 2023-05-03 10:00:43.645184 lixinger-0.1.1/lixinger/api/cn/company/base.py
--rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.1/lixinger/api/cn/index/__init__.py
--rw-r--r--   0        0        0     1685 2023-05-03 09:59:49.921863 lixinger-0.1.1/lixinger/api/cn/index/fundamental.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.1/lixinger/api/hk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.1/lixinger/api/macro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.1/lixinger/api/us/__init__.py
--rw-r--r--   0        0        0     1540 2023-05-03 04:05:06.981904 lixinger-0.1.1/lixinger/config.py
--rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.1/lixinger/py.typed
--rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.1/lixinger/settings.toml
--rw-r--r--   0        0        0     1030 2023-05-03 09:26:05.615918 lixinger-0.1.1/lixinger/utils.py
--rw-r--r--   0        0        0      616 2023-05-03 10:12:07.486854 lixinger-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.1/tests/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.1/tests/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.1/tests/api/cn/company/__init__.py
--rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.1/tests/api/cn/company/test_base.py
--rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.1/tests/api/cn/index/__init__.py
--rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.1/tests/api/cn/index/test_fundamental.py
--rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 lixinger-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      705 2023-05-03 10:11:52.615764 lixinger-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.2/lixinger/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.2/lixinger/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.2/lixinger/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.2/lixinger/api/cn/company/__init__.py
+-rw-r--r--   0        0        0     2132 2023-05-04 10:40:12.138787 lixinger-0.1.2/lixinger/api/cn/company/base.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.2/lixinger/api/cn/index/__init__.py
+-rw-r--r--   0        0        0     1721 2023-05-04 10:40:12.140548 lixinger-0.1.2/lixinger/api/cn/index/fundamental.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.2/lixinger/api/hk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.2/lixinger/api/macro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.2/lixinger/api/us/__init__.py
+-rw-r--r--   0        0        0     1582 2023-05-04 10:40:12.141591 lixinger-0.1.2/lixinger/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.2/lixinger/py.typed
+-rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.2/lixinger/settings.toml
+-rw-r--r--   0        0        0      978 2023-05-04 10:40:12.142362 lixinger-0.1.2/lixinger/utils.py
+-rw-r--r--   0        0        0     1013 2023-05-04 10:40:26.894124 lixinger-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.2/tests/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.2/tests/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.2/tests/api/cn/company/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.2/tests/api/cn/company/test_base.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.2/tests/api/cn/index/__init__.py
+-rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.2/tests/api/cn/index/test_fundamental.py
+-rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 lixinger-0.1.2/PKG-INFO
```

### Comparing `lixinger-0.1.1/README.md` & `lixinger-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.1/lixinger/api/cn/company/base.py` & `lixinger-0.1.2/lixinger/api/cn/company/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Literal, Optional
 
 import pandas as pd
 import pandera as pa
 import requests
 from pydantic import validate_arguments
```

### Comparing `lixinger-0.1.1/lixinger/api/cn/index/fundamental.py` & `lixinger-0.1.2/lixinger/api/cn/index/fundamental.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pandas as pd
 import pandera as pa
 import requests
 from pydantic import validate_arguments
 
 from lixinger.config import settings
 from lixinger.utils import get_response_df
```

### Comparing `lixinger-0.1.1/lixinger/config.py` & `lixinger-0.1.2/lixinger/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import pathlib
 
 from dynaconf import Dynaconf, Validator
 
 DEFAULT_SETTINGS_PATH: pathlib.Path = (
     pathlib.Path(__file__).resolve().parent / "settings.toml"
@@ -36,15 +38,15 @@
 def get_validators() -> list[Validator]:
     """Get validators for settings.
 
     Cast settings to their types.
     """
     settings_types = vars(TypedDynaconf)["__annotations__"]
     return [
-        Validator(key, cast=settings_cast_map.get(key, type_))
+        Validator(key, cast=cast(settings_cast_map.get(key, type_)))
         for key, type_ in settings_types.items()
     ]
 
 
 def load_settings(
     path: pathlib.Path = DEFAULT_SETTINGS_PATH,
     user_settings_path: pathlib.Path = USER_SETTINGS_PATH,
```

### Comparing `lixinger-0.1.1/lixinger/utils.py` & `lixinger-0.1.2/lixinger/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 
 import numpy as np
 import pandas as pd
 from requests import Response
 
 
@@ -20,18 +22,14 @@
     try:
         return ",".join(map(str, column))
     except TypeError:
         return np.nan
 
 
 def get_response_data(response: Response) -> list[dict[str, any]]:
-    try:
-        response.raise_for_status()
-    except Exception as e:
-        raise e
     resp_json = response.json()
     if resp_json.get("code") != 1:
         raise ValueError(f"[{resp_json.get('code')}]{resp_json.get('error')}")
     return resp_json["data"]
 
 
 def get_response_df(response: Response) -> pd.DataFrame:
```

