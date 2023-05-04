# Comparing `tmp/conduit-sdk-0.2.4.tar.gz` & `tmp/conduit_sdk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conduit-sdk-0.2.4.tar", max compression
+gzip compressed data, was "conduit_sdk-0.2.5.tar", max compression
```

## Comparing `conduit-sdk-0.2.4.tar` & `conduit_sdk-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/__init__.py
--rw-r--r--   0        0        0        0 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/block/__init__.py
--rw-r--r--   0        0        0      581 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/block/callback_script.py
--rw-r--r--   0        0        0     3681 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/block/csv.py
--rw-r--r--   0        0        0     4452 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/block/parse.py
--rw-r--r--   0        0        0      867 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/block/schema.py
--rw-r--r--   0        0        0        0 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/common/__init__.py
--rw-r--r--   0        0        0      648 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/common/schema.py
--rw-r--r--   0        0        0      140 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/errors.py
--rw-r--r--   0        0        0      821 2022-09-23 11:18:23.543777 conduit-sdk-0.2.4/conduit_sdk/vault.py
--rw-r--r--   0        0        0     1385 2022-09-23 11:18:23.547777 conduit-sdk-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 conduit-sdk-0.2.4/setup.py
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 conduit-sdk-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-04 10:47:30.079241 conduit_sdk-0.2.5/conduit_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:47:30.079241 conduit_sdk-0.2.5/conduit_sdk/block/__init__.py
+-rw-r--r--   0        0        0      581 2023-05-04 10:47:30.083241 conduit_sdk-0.2.5/conduit_sdk/block/callback_script.py
+-rw-r--r--   0        0        0     3681 2023-05-04 10:47:30.083241 conduit_sdk-0.2.5/conduit_sdk/block/csv.py
+-rw-r--r--   0        0        0     4804 2023-05-04 10:47:30.083241 conduit_sdk-0.2.5/conduit_sdk/block/parse.py
+-rw-r--r--   0        0        0      867 2023-05-04 10:47:30.083241 conduit_sdk-0.2.5/conduit_sdk/block/schema.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:47:30.083241 conduit_sdk-0.2.5/conduit_sdk/common/__init__.py
+-rw-r--r--   0        0        0      648 2023-05-04 10:47:30.083241 conduit_sdk-0.2.5/conduit_sdk/common/schema.py
+-rw-r--r--   0        0        0      140 2023-05-04 10:47:30.083241 conduit_sdk-0.2.5/conduit_sdk/errors.py
+-rw-r--r--   0        0        0      821 2023-05-04 10:47:30.083241 conduit_sdk-0.2.5/conduit_sdk/vault.py
+-rw-r--r--   0        0        0     1385 2023-05-04 10:47:30.083241 conduit_sdk-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 conduit_sdk-0.2.5/setup.py
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 conduit_sdk-0.2.5/PKG-INFO
```

### Comparing `conduit-sdk-0.2.4/conduit_sdk/block/callback_script.py` & `conduit_sdk-0.2.5/conduit_sdk/block/callback_script.py`

 * *Files identical despite different names*

### Comparing `conduit-sdk-0.2.4/conduit_sdk/block/csv.py` & `conduit_sdk-0.2.5/conduit_sdk/block/csv.py`

 * *Files identical despite different names*

### Comparing `conduit-sdk-0.2.4/conduit_sdk/block/parse.py` & `conduit_sdk-0.2.5/conduit_sdk/block/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,15 +91,22 @@
         return
 
     raise ValidationError(f'Bad origin: {origin}')
 
 
 def _parse_columns(columns: list[dict[str, Any]]) -> list[DataColumnSchema]:
     parsed_columns = []
+
+    if not isinstance(columns, list):
+        raise ValidationError('Columns field must be a list instance')
+
     for col_number, col in enumerate(columns, 1):
+        if not isinstance(col, dict):
+            raise ValidationError(f'Column {col_number} must be a dict instance')
+
         name = _get_column_field(col, 'name', col_number)
         type_key = _get_column_field(col, 'type', col_number)
         kind_key = _get_column_field(col, 'kind', col_number)
         agg_key = _get_column_field(col, 'agg', col_number)
 
         parsed_columns.append(
             DataColumnSchema(
@@ -109,14 +116,17 @@
                 agg=AggregationType[agg_key],
             ),
         )
     return parsed_columns
 
 
 def _parse_localization(localization: dict[str, Any]) -> LocalizationSchema:
+    if not isinstance(localization, dict):
+        raise ValidationError('Localization field must be a dict instance')
+
     week_start = _get_body_field(localization, 'week_start')
     locale = _get_body_field(localization, 'locale')
     currency = _get_body_field(localization, 'currency')
     decimal_digits = _get_body_field(localization, 'decimal_digits')
     money_digits = _get_body_field(localization, 'money_digits')
     percent_digits = _get_body_field(localization, 'percent_digits')
```

### Comparing `conduit-sdk-0.2.4/conduit_sdk/block/schema.py` & `conduit_sdk-0.2.5/conduit_sdk/block/schema.py`

 * *Files identical despite different names*

### Comparing `conduit-sdk-0.2.4/conduit_sdk/common/schema.py` & `conduit_sdk-0.2.5/conduit_sdk/common/schema.py`

 * *Files identical despite different names*

### Comparing `conduit-sdk-0.2.4/conduit_sdk/vault.py` & `conduit_sdk-0.2.5/conduit_sdk/vault.py`

 * *Files identical despite different names*

### Comparing `conduit-sdk-0.2.4/pyproject.toml` & `conduit_sdk-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "conduit-sdk"
-version = "0.2.4"
+version = "0.2.5"
 description = "Conduit sdk is a collection of utils for development of conduit external block."
 authors = ["Conduit.app <support@getconduit.app>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.1"
```

### Comparing `conduit-sdk-0.2.4/setup.py` & `conduit_sdk-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'conduit-sdk',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Conduit sdk is a collection of utils for development of conduit external block.',
     'long_description': 'None',
     'author': 'Conduit.app',
     'author_email': 'support@getconduit.app',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

