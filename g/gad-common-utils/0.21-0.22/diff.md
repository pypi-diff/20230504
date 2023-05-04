# Comparing `tmp/gad_common_utils-0.21.tar.gz` & `tmp/gad_common_utils-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gad_common_utils-0.21.tar", last modified: Thu May  4 11:19:40 2023, max compression
+gzip compressed data, was "gad_common_utils-0.22.tar", last modified: Thu May  4 13:02:20 2023, max compression
```

## Comparing `gad_common_utils-0.21.tar` & `gad_common_utils-0.22.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.974609 gad_common_utils-0.21/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.966609 gad_common_utils-0.21/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.970609 gad_common_utils-0.21/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.github/workflows/black-format-checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 11:19:40.974609 gad_common_utils-0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-04 11:19:29.000000 gad_common_utils-0.21/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.974609 gad_common_utils-0.21/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-04 11:19:40.000000 gad_common_utils-0.21/common_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/data_loading_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/data_type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/date_time_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/dynamodb_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/dynamodb_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/files_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/gad_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/gad_utils_additionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/json_schema_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/run_athena_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/s3_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/sql_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/string_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.974609 gad_common_utils-0.21/gad_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 11:19:29.000000 gad_common_utils-0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:19:40.974609 gad_common_utils-0.21/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.974609 gad_common_utils-0.21/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:29.000000 gad_common_utils-0.21/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 11:19:29.000000 gad_common_utils-0.21/tests/test_json_schema_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.449598 gad_common_utils-0.22/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.445598 gad_common_utils-0.22/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.445598 gad_common_utils-0.22/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.github/workflows/black-format-checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 13:02:10.000000 gad_common_utils-0.22/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 13:02:20.449598 gad_common_utils-0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-04 13:02:10.000000 gad_common_utils-0.22/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.449598 gad_common_utils-0.22/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-04 13:02:20.000000 gad_common_utils-0.22/common_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/data_loading_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/data_type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/date_time_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/dynamodb_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/dynamodb_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/files_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/gad_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/gad_utils_additionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/json_schema_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/run_athena_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/s3_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/sql_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 13:02:10.000000 gad_common_utils-0.22/common_utils/string_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.449598 gad_common_utils-0.22/gad_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 13:02:20.000000 gad_common_utils-0.22/gad_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 13:02:10.000000 gad_common_utils-0.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:02:20.449598 gad_common_utils-0.22/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:20.449598 gad_common_utils-0.22/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:02:10.000000 gad_common_utils-0.22/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 13:02:10.000000 gad_common_utils-0.22/tests/test_json_schema_methods.py
```

### Comparing `gad_common_utils-0.21/.github/workflows/black-format-checker.yml` & `gad_common_utils-0.22/.github/workflows/black-format-checker.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/.github/workflows/publish-to-pypi.yml` & `gad_common_utils-0.22/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/.github/workflows/pytest.yml` & `gad_common_utils-0.22/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/PKG-INFO` & `gad_common_utils-0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad_common_utils
-Version: 0.21
+Version: 0.22
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.21/common_utils/data_loading_management.py` & `gad_common_utils-0.22/common_utils/data_loading_management.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/data_type_conversion.py` & `gad_common_utils-0.22/common_utils/data_type_conversion.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/date_time_methods.py` & `gad_common_utils-0.22/common_utils/date_time_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/dynamodb_methods.py` & `gad_common_utils-0.22/common_utils/dynamodb_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/files_methods.py` & `gad_common_utils-0.22/common_utils/files_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/gad_utils.py` & `gad_common_utils-0.22/common_utils/gad_utils.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/gad_utils_additionals.py` & `gad_common_utils-0.22/common_utils/gad_utils_additionals.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/json_schema_methods.py` & `gad_common_utils-0.22/common_utils/json_schema_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/run_athena_query.py` & `gad_common_utils-0.22/common_utils/run_athena_query.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/s3_methods.py` & `gad_common_utils-0.22/common_utils/s3_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/common_utils/string_transformations.py` & `gad_common_utils-0.22/common_utils/string_transformations.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/gad_common_utils.egg-info/PKG-INFO` & `gad_common_utils-0.22/gad_common_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad-common-utils
-Version: 0.21
+Version: 0.22
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.21/gad_common_utils.egg-info/SOURCES.txt` & `gad_common_utils-0.22/gad_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/pyproject.toml` & `gad_common_utils-0.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.21/tests/test_json_schema_methods.py` & `gad_common_utils-0.22/tests/test_json_schema_methods.py`

 * *Files identical despite different names*

