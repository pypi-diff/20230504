# Comparing `tmp/dh-facebook-client-0.2.0.tar.gz` & `tmp/dh_facebook_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh-facebook-client-0.2.0.tar", max compression
+gzip compressed data, was "dh_facebook_client-0.2.1.tar", max compression
```

## Comparing `dh-facebook-client-0.2.0.tar` & `dh_facebook_client-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1086 2022-11-22 13:28:44.818483 dh-facebook-client-0.2.0/dh_facebook_client/__init__.py
--rw-r--r--   0        0        0    11071 2022-11-22 13:28:44.819436 dh-facebook-client-0.2.0/dh_facebook_client/client.py
--rw-r--r--   0        0        0      248 2022-11-22 13:29:01.312834 dh-facebook-client-0.2.0/dh_facebook_client/constants.py
--rw-r--r--   0        0        0     5353 2022-11-22 13:28:44.821441 dh-facebook-client-0.2.0/dh_facebook_client/dataclasses.py
--rw-r--r--   0        0        0      521 2022-01-07 20:33:55.410330 dh-facebook-client-0.2.0/dh_facebook_client/error_code.py
--rw-r--r--   0        0        0     4502 2022-06-14 20:10:02.880771 dh-facebook-client-0.2.0/dh_facebook_client/exceptions.py
--rw-r--r--   0        0        0     2828 2022-11-22 13:28:44.822379 dh-facebook-client-0.2.0/dh_facebook_client/helpers.py
--rw-r--r--   0        0        0     1049 2022-11-22 13:28:44.823050 dh-facebook-client-0.2.0/dh_facebook_client/page_client.py
--rw-r--r--   0        0        0      435 2022-11-22 13:28:44.823651 dh-facebook-client-0.2.0/dh_facebook_client/typings.py
--rw-r--r--   0        0        0     1894 2022-11-22 13:28:44.824400 dh-facebook-client-0.2.0/dh_facebook_client/user_client.py
--rw-r--r--   0        0        0      651 2022-11-22 13:29:07.483041 dh-facebook-client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      689 2022-11-22 14:17:47.890095 dh-facebook-client-0.2.0/setup.py
--rw-r--r--   0        0        0      391 2022-11-22 14:17:47.890352 dh-facebook-client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-03 19:25:20.013300 dh_facebook_client-0.2.1/dh_facebook_client/__init__.py
+-rw-r--r--   0        0        0    11071 2023-05-03 19:25:20.013488 dh_facebook_client-0.2.1/dh_facebook_client/client.py
+-rw-r--r--   0        0        0      260 2023-05-04 15:33:07.172663 dh_facebook_client-0.2.1/dh_facebook_client/constants.py
+-rw-r--r--   0        0        0     5353 2023-05-03 19:25:20.013782 dh_facebook_client-0.2.1/dh_facebook_client/dataclasses.py
+-rw-r--r--   0        0        0      521 2023-05-03 19:25:20.013909 dh_facebook_client-0.2.1/dh_facebook_client/error_code.py
+-rw-r--r--   0        0        0     4502 2023-05-03 19:25:20.014061 dh_facebook_client-0.2.1/dh_facebook_client/exceptions.py
+-rw-r--r--   0        0        0     2902 2023-05-04 15:33:14.240260 dh_facebook_client-0.2.1/dh_facebook_client/helpers.py
+-rw-r--r--   0        0        0     1049 2023-05-03 19:25:20.014307 dh_facebook_client-0.2.1/dh_facebook_client/page_client.py
+-rw-r--r--   0        0        0      435 2023-05-03 19:25:20.014436 dh_facebook_client-0.2.1/dh_facebook_client/typings.py
+-rw-r--r--   0        0        0     1894 2023-05-03 19:25:20.014566 dh_facebook_client-0.2.1/dh_facebook_client/user_client.py
+-rw-r--r--   0        0        0      651 2023-05-04 15:33:18.662056 dh_facebook_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 dh_facebook_client-0.2.1/PKG-INFO
```

### Comparing `dh-facebook-client-0.2.0/dh_facebook_client/__init__.py` & `dh_facebook_client-0.2.1/dh_facebook_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.2.0/dh_facebook_client/client.py` & `dh_facebook_client-0.2.1/dh_facebook_client/client.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.2.0/dh_facebook_client/dataclasses.py` & `dh_facebook_client-0.2.1/dh_facebook_client/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.2.0/dh_facebook_client/error_code.py` & `dh_facebook_client-0.2.1/dh_facebook_client/error_code.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.2.0/dh_facebook_client/exceptions.py` & `dh_facebook_client-0.2.1/dh_facebook_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.2.0/dh_facebook_client/helpers.py` & `dh_facebook_client-0.2.1/dh_facebook_client/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 from datetime import datetime
-from typing import Any, Callable, Iterable, Optional
+from typing import Any, Callable, Iterable, Optional, Final
 
 from typing_extensions import NotRequired, TypedDict
 
 # TODO: Recursive type hints not yet available in mypy,
 #  should change sub_fields hint to Optional[List[FieldConfig]] when possible:
 #  https://github.com/python/mypy/issues/731
 FieldConfig = TypedDict(
     'FieldConfig',
     {
         'field_name': str,
         'limit': NotRequired[int],
         'after': NotRequired[str],
+        'date_preset': NotRequired[str],
         'sub_fields': NotRequired[list[Any]],
     },
 )
 
 
+ACCEPTED_SUB_PARAM_NAMES: Final = (
+    'limit',
+    'after',
+    'date_preset',
+)
+
+
 def format_fields_str(fields_config: list[FieldConfig]) -> str:
     """
     Helper function to support field expansion / limiting functionality:
     https://developers.facebook.com/docs/graph-api/field-expansion
     :param fields_config: The field configurations you want contained in string format
     :return: A formatted fields string
     """
     fields_str = ''
     for config in fields_config:
-        # Prep the base sub string for a field (i.e. foo.limit(5).after(BAR))
-        limit_sub_str = _format_field_config_paging_sub_str(config, 'limit')
-        after_sub_str = _format_field_config_paging_sub_str(config, 'after')
-        fields_str += f'{config["field_name"]}{limit_sub_str}{after_sub_str}'
-
-        # If sub-fields exist, prep the nested sub field(s) strings
+        # Prep the base sub string for a field w/ params (i.e. foo.limit(5).after(BAR))
+        fields_str = f'{config["field_name"]}'
+        for param_name in ACCEPTED_SUB_PARAM_NAMES:
+            fields_str += _format_sub_parameter_str(config, param_name)
+        # If sub-fields exist, prep the nested sub-field(s) strings
         sub_fields = config.get('sub_fields')
         if sub_fields:
             fields_str += f'{{{format_fields_str(sub_fields)}}}'
 
         # If not the last item in a config list, add a comma separator
         if config != fields_config[-1]:
             fields_str += ','
     return fields_str
 
 
-def _format_field_config_paging_sub_str(config: FieldConfig, param_name: str) -> str:
+def _format_sub_parameter_str(config: FieldConfig, param_name: str) -> str:
     """
-    Used to help format paging sub strings for a specific field:
-    https://developers.facebook.com/docs/graph-api/field-expansion#limiting-results
+    Used to help format sub-param strings for a specific field:
+    Ex: https://developers.facebook.com/docs/graph-api/field-expansion#limiting-results
     :param config: An instance of FieldConfig
     :param param_name: The parameter name to pluck from config (i.e. limit or after)
     :return: A formatted paging sub string (i.e. .limit(5))
     """
     param = config.get(param_name)
     return f'.{param_name}({param})' if param else ''
```

### Comparing `dh-facebook-client-0.2.0/dh_facebook_client/page_client.py` & `dh_facebook_client-0.2.1/dh_facebook_client/page_client.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.2.0/dh_facebook_client/user_client.py` & `dh_facebook_client-0.2.1/dh_facebook_client/user_client.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.2.0/pyproject.toml` & `dh_facebook_client-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dh-facebook-client"
-version = "0.2.0"
+version = "0.2.1"
 description = "Simple client for interacting with the Facebook Graph API"
 authors = ["pchisholm <chisholm.p@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.26.0"
 backoff = "^1.11.1"
```

