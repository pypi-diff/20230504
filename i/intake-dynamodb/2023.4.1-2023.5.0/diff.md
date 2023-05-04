# Comparing `tmp/intake-dynamodb-2023.4.1.tar.gz` & `tmp/intake-dynamodb-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-dynamodb-2023.4.1.tar", last modified: Wed Apr 12 18:06:50 2023, max compression
+gzip compressed data, was "intake-dynamodb-2023.5.0.tar", last modified: Thu May  4 20:49:04 2023, max compression
```

## Comparing `intake-dynamodb-2023.4.1.tar` & `intake-dynamodb-2023.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.ciocheck
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.956089 intake-dynamodb-2023.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.956089 intake-dynamodb-2023.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.956089 intake-dynamodb-2023.4.1/intake_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/intake_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/intake_dynamodb/dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 18:06:50.000000 intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.956089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/data/abcdefghijklmnopqrstuvwxyz.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/data/abcdefghijklmnopqrstuvwxyz.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-files.json
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-summary.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:06:50.960089 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz.json
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz2.json
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz2.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-files.json
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-summary.json
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-04-12 18:06:38.000000 intake-dynamodb-2023.4.1/tests/test_dynamodb_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.036629 intake-dynamodb-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/.ciocheck
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.028629 intake-dynamodb-2023.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.032629 intake-dynamodb-2023.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-04 20:49:04.036629 intake-dynamodb-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.032629 intake-dynamodb-2023.5.0/intake_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/intake_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/intake_dynamodb/dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.032629 intake-dynamodb-2023.5.0/intake_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-04 20:49:04.000000 intake-dynamodb-2023.5.0/intake_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-04 20:49:04.000000 intake-dynamodb-2023.5.0/intake_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:49:04.000000 intake-dynamodb-2023.5.0/intake_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 20:49:04.000000 intake-dynamodb-2023.5.0/intake_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 20:49:04.000000 intake-dynamodb-2023.5.0/intake_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 20:49:04.000000 intake-dynamodb-2023.5.0/intake_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 20:49:04.036629 intake-dynamodb-2023.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.032629 intake-dynamodb-2023.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.028629 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.032629 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.032629 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh/data/abcdefghijklmnopqrstuvwxyz.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh/data/abcdefghijklmnopqrstuvwxyz.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-summary.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.032629 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:49:04.036629 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz.json
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh2/data/abcdefghijklmnopqrstuvwxyz2.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-summary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-05-04 20:48:50.000000 intake-dynamodb-2023.5.0/tests/test_dynamodb_catalog.py
```

### Comparing `intake-dynamodb-2023.4.1/.ciocheck` & `intake-dynamodb-2023.5.0/.ciocheck`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/.github/workflows/python-package.yml` & `intake-dynamodb-2023.5.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/.github/workflows/python-publish.yml` & `intake-dynamodb-2023.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/.gitignore` & `intake-dynamodb-2023.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/.pre-commit-config.yaml` & `intake-dynamodb-2023.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/LICENSE` & `intake-dynamodb-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/PKG-INFO` & `intake-dynamodb-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-dynamodb
-Version: 2023.4.1
+Version: 2023.5.0
 Summary: Intake plugin for reading data from dynamodb
 Author-email: Ray Bell <rayjohnbell0@gmail.com>
 Project-URL: repository, https://github.com/intake-dynamodb/intake-dynamodb
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/PKG-INFO` & `intake-dynamodb-2023.5.0/intake_dynamodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-dynamodb
-Version: 2023.4.1
+Version: 2023.5.0
 Summary: Intake plugin for reading data from dynamodb
 Author-email: Ray Bell <rayjohnbell0@gmail.com>
 Project-URL: repository, https://github.com/intake-dynamodb/intake-dynamodb
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `intake-dynamodb-2023.4.1/intake_dynamodb.egg-info/SOURCES.txt` & `intake-dynamodb-2023.5.0/intake_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/pyproject.toml` & `intake-dynamodb-2023.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 follow_imports = "silent"
 ignore_missing_imports = true
 scripts_are_modules = true
 
 [tool.pytest.ini_options]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
+    "s3test: marks tests that use s3 (deselect with '-m \"not s3\"')",
 ]
 
 [tool.ruff]
 select = [
     # Pyflakes
     "E",
     # pycodestyle
```

### Comparing `intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-summary.json` & `intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh/manifest-summary.json`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-summary.json` & `intake-dynamodb-2023.5.0/tests/AWSDynamoDB/0123456789-abcdefgh2/manifest-summary.json`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/tests/conftest.py` & `intake-dynamodb-2023.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `intake-dynamodb-2023.4.1/tests/test.yaml` & `intake-dynamodb-2023.5.0/tests/test.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 sources:
   example_small_table:
     description: example small dynamodb table
     driver: dynamodb
     args:
       table_name: 'example-small-table'
       region_name: 'us-east-1'
+  example_small_table_limit:
+    description: example small dynamodb table with limit
+    driver: dynamodb
+    args:
+      table_name: 'example-small-table'
+      region_name: 'us-east-1'
+      limit: 1
   example_small_table_filtered_num:
     description: example small dynamodb table with a numeric filter
     driver: dynamodb
     args:
       table_name: 'example-small-table'
       region_name: 'us-east-1'
       filter_expression: 'ag = :ag_value'
@@ -39,12 +46,21 @@
       sts_role_arn: 'arn:aws:iam::ACCOUNT_ID:role/ROLE_NAME'
       region_name: 'us-west-2'
   example_small_s3_export:
     description: example small dynamodb table exported to s3
     driver: dynamodbjson
     args:
       s3_path: 's3://example-bucket/AWSDynamoDB/0123456789-abcdefgh'
+  example_small_s3_export_with_kwargs:
+    description: example small dynamodb table exported to s3
+    driver: dynamodbjson
+    args:
+      s3_path: 's3://example-bucket/AWSDynamoDB/0123456789-abcdefgh'
+      storage_options:
+        profile: 'dev'
+      config_kwargs:
+        read_timeout: 3600  # Default is 15
   example_partitioned_s3_export:
     description: example big dynamodb table exported to s3
     driver: dynamodbjson
     args:
       s3_path: 's3://example-bucket/AWSDynamoDB/0123456789-abcdefgh2'
```

### Comparing `intake-dynamodb-2023.4.1/tests/test_dynamodb_catalog.py` & `intake-dynamodb-2023.5.0/tests/test_dynamodb_catalog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import botocore
+import dask
 import dask.dataframe as dd
 import intake
 import pandas as pd
 import pandas._testing as pd_testing
 import pytest
 from dask.dataframe.utils import assert_eq as dask_dataframe_assert_eq
 from intake.source.base import DataSource
@@ -193,28 +194,46 @@
 
 
 @pytest.fixture
 def yaml_catalog() -> DataSource:
     return intake.open_catalog("tests/test.yaml")
 
 
+#######################################
+########### END OF FIXTURES ###########
+#######################################
+
+
 def test_dynamodb_source(example_small_table):
     source = DynamoDBSource(table_name=example_small_table)
     assert isinstance(source, DynamoDBSource)
 
 
 def test_dynamodb_scan(example_small_table, example_small_table_items):
     source = DynamoDBSource(
         table_name=example_small_table,
         region_name="us-east-1",
     )
     items = source._scan_table()
     assert items == example_small_table_items
 
 
+def test_dynamodb_scan_limit(
+    example_small_table,
+    example_small_table_items,
+):
+    source = DynamoDBSource(
+        table_name=example_small_table,
+        region_name="us-east-1",
+        limit=1,
+    )
+    items = source._scan_table()
+    assert items == [example_small_table_items[0]]
+
+
 def test_dynamodb_scan_filtered_num(
     example_small_table, example_small_table_items_filtered
 ):
     source = DynamoDBSource(
         table_name=example_small_table,
         region_name="us-east-1",
         filter_expression="ag = :ag_value",
@@ -233,24 +252,37 @@
         filter_expression="nm = :nm_value",
         filter_expression_value="John Doe",
     )
     items = source._scan_table()
     assert items == example_small_table_items_filtered
 
 
-def test_dynamodb_to_dask(
+def test_dynamodb_to_dask(example_small_table):
+    source = DynamoDBSource(
+        table_name=example_small_table,
+        region_name="us-east-1",
+    )
+    actual_dask = source.to_dask()
+    expected_dask = dask.delayed(source.read())
+    pd_testing.assert_equal(
+        actual_dask.compute(),
+        expected_dask.compute(),
+    )
+
+
+def test_dynamodb_to_dask_df(
     example_small_table,
     example_small_table_expected_ddf,
 ):
     source = DynamoDBSource(
         table_name=example_small_table,
         region_name="us-east-1",
     )
-    actual_dask = source.to_dask()
-    dask_dataframe_assert_eq(actual_dask, example_small_table_expected_ddf)
+    actual_dask_df = source.to_dask_df()
+    dask_dataframe_assert_eq(actual_dask_df, example_small_table_expected_ddf)
 
 
 def test_dynamodb_read(
     example_small_table,
     example_small_table_expected_ddf,
 ):
     source = DynamoDBSource(
@@ -260,14 +292,41 @@
     actual_df = source.read()
     pd_testing.assert_equal(
         actual_df,
         example_small_table_expected_ddf.compute(),
     )
 
 
+def test_yaml_small_table(
+    yaml_catalog,
+    example_small_table,
+    example_small_table_expected_ddf,
+):
+    source = yaml_catalog.example_small_table
+    actual_df = source.read()
+    pd_testing.assert_equal(
+        actual_df,
+        example_small_table_expected_ddf.compute(),
+    )
+
+
+def test_yaml_small_table_limit(
+    yaml_catalog,
+    example_small_table,
+    example_small_table_expected_ddf,
+):
+    source = yaml_catalog.example_small_table_limit
+    actual_df = source.read()
+    expected_df = example_small_table_expected_ddf.compute().loc[[0]]
+    pd_testing.assert_equal(
+        actual_df,
+        expected_df,
+    )
+
+
 def test_yaml_small_table_filtered_num(
     yaml_catalog,
     example_small_table,
     example_small_table_expected_ddf_filtered,
 ):
     source = yaml_catalog.example_small_table_filtered_num
     actual_df = source.read()
@@ -313,60 +372,48 @@
     actual_df = source.read()
     pd_testing.assert_equal(
         actual_df,
         example_small_table_different_account_expected_ddf.compute(),
     )
 
 
-def test_yaml_small_table(
-    yaml_catalog,
-    example_small_table,
-    example_small_table_expected_ddf,
-):
-    source = yaml_catalog.example_small_table
-    actual_df = source.read()
-    pd_testing.assert_equal(
-        actual_df,
-        example_small_table_expected_ddf.compute(),
-    )
-
-
 @pytest.mark.slow
 def test_yaml_big_table(
     yaml_catalog,
     example_big_table,
     example_big_table_expected_ddf,
 ):
     source = yaml_catalog.example_big_table
-    actual_ddf = source.to_dask()
+    actual_ddf = source.to_dask_df()
     dask_dataframe_assert_eq(
         actual_ddf,
         example_big_table_expected_ddf,
     )
 
 
 def test_yaml_different_account(
     yaml_catalog,
     example_small_table_different_account,
     example_small_table_different_account_expected_ddf,
 ):
     source = yaml_catalog.example_small_table_different_account
-    actual_ddf = source.to_dask()
+    actual_ddf = source.to_dask_df()
     dask_dataframe_assert_eq(
         actual_ddf, example_small_table_different_account_expected_ddf
     )
 
 
 def test_dynamodbjson_source(example_bucket):
     source = DynamoDBJSONSource(
         s3_path=f"s3://{example_bucket}/AWSDynamoDB/0123456789-abcdefgh",
     )
     assert isinstance(source, DynamoDBJSONSource)
 
 
+@pytest.mark.s3test
 def test_dynamodbjson_small_s3_export(
     example_bucket,
     s3,
     example_small_table_expected_ddf,
 ):
     source = DynamoDBJSONSource(
         s3_path=f"s3://{example_bucket}/AWSDynamoDB/0123456789-abcdefgh",
@@ -374,27 +421,43 @@
     actual_df = source.read()
     pd_testing.assert_equal(
         actual_df,
         example_small_table_expected_ddf.compute(),
     )
 
 
+@pytest.mark.s3test
 def test_dynamodbjson_small_s3_export_yaml(
     yaml_catalog,
     example_bucket,
     s3,
     example_small_table,
 ):
     source_s3_export = yaml_catalog.example_small_s3_export
     s3_export_df = source_s3_export.read()
     source_dynamodb = yaml_catalog.example_small_table
     dynamodb_df = source_dynamodb.read()
     pd_testing.assert_equal(s3_export_df, dynamodb_df)
 
 
+@pytest.mark.s3test
+def test_dynamodbjson_small_s3_export_yaml_with_kwargs(
+    yaml_catalog,
+    example_bucket,
+    s3,
+    example_small_table,
+):
+    source_s3_export = yaml_catalog.example_small_s3_export_with_kwargs
+    s3_export_df = source_s3_export.read()
+    source_dynamodb = yaml_catalog.example_small_table
+    dynamodb_df = source_dynamodb.read()
+    pd_testing.assert_equal(s3_export_df, dynamodb_df)
+
+
+@pytest.mark.s3test
 def test_dynamodbjson_partitioned_s3_export(
     example_bucket,
     s3,
     example_small_table_expected_ddf,
 ):
     source = DynamoDBJSONSource(
         s3_path=f"s3://{example_bucket}/AWSDynamoDB/0123456789-abcdefgh2",
@@ -402,14 +465,15 @@
     actual_df = source.read()
     pd_testing.assert_equal(
         actual_df,
         example_small_table_expected_ddf.compute(),
     )
 
 
+@pytest.mark.s3test
 def test_dynamodbjson_partitioned_s3_export_yaml(
     yaml_catalog,
     example_bucket,
     s3,
     example_small_table,
 ):
     source_paritioned_s3_export = yaml_catalog.example_partitioned_s3_export
```

