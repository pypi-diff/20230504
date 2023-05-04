# Comparing `tmp/gad_common_utils-0.20.tar.gz` & `tmp/gad_common_utils-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gad_common_utils-0.20.tar", last modified: Tue May  2 14:17:55 2023, max compression
+gzip compressed data, was "gad_common_utils-0.21.tar", last modified: Thu May  4 11:19:40 2023, max compression
```

## Comparing `gad_common_utils-0.20.tar` & `gad_common_utils-0.21.tar`

### file list

```diff
@@ -1,42 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:55.578384 gad_common_utils-0.20/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:55.574385 gad_common_utils-0.20/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:55.578384 gad_common_utils-0.20/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-02 14:17:44.000000 gad_common_utils-0.20/.github/workflows/black-format-checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-02 14:17:44.000000 gad_common_utils-0.20/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-02 14:17:44.000000 gad_common_utils-0.20/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-02 14:17:44.000000 gad_common_utils-0.20/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-02 14:17:55.578384 gad_common_utils-0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-02 14:17:44.000000 gad_common_utils-0.20/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:55.578384 gad_common_utils-0.20/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:55.578384 gad_common_utils-0.20/common_utils/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/__pycache__/json_schema_methods.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-02 14:17:55.000000 gad_common_utils-0.20/common_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/data_loading_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/data_type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/date_time_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/dynamodb_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/dynamodb_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/files_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/gad_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/gad_utils_additionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/json_schema_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/run_athena_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/s3_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-02 14:17:44.000000 gad_common_utils-0.20/common_utils/string_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:55.578384 gad_common_utils-0.20/gad_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-02 14:17:55.000000 gad_common_utils-0.20/gad_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-02 14:17:55.000000 gad_common_utils-0.20/gad_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:17:55.000000 gad_common_utils-0.20/gad_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 14:17:55.000000 gad_common_utils-0.20/gad_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 14:17:55.000000 gad_common_utils-0.20/gad_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-02 14:17:44.000000 gad_common_utils-0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:17:55.578384 gad_common_utils-0.20/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:55.578384 gad_common_utils-0.20/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:44.000000 gad_common_utils-0.20/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:55.578384 gad_common_utils-0.20/tests/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-02 14:17:44.000000 gad_common_utils-0.20/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-02 14:17:44.000000 gad_common_utils-0.20/tests/__pycache__/test_json_schema_methods.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-02 14:17:44.000000 gad_common_utils-0.20/tests/test_json_schema_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.974609 gad_common_utils-0.21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.966609 gad_common_utils-0.21/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.970609 gad_common_utils-0.21/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.github/workflows/black-format-checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 11:19:29.000000 gad_common_utils-0.21/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 11:19:40.974609 gad_common_utils-0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-04 11:19:29.000000 gad_common_utils-0.21/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.974609 gad_common_utils-0.21/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-04 11:19:40.000000 gad_common_utils-0.21/common_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/data_loading_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/data_type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/date_time_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/dynamodb_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/dynamodb_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/files_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/gad_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/gad_utils_additionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/json_schema_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/run_athena_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/s3_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/sql_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 11:19:29.000000 gad_common_utils-0.21/common_utils/string_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.974609 gad_common_utils-0.21/gad_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 11:19:40.000000 gad_common_utils-0.21/gad_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 11:19:29.000000 gad_common_utils-0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:19:40.974609 gad_common_utils-0.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:40.974609 gad_common_utils-0.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:19:29.000000 gad_common_utils-0.21/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 11:19:29.000000 gad_common_utils-0.21/tests/test_json_schema_methods.py
```

### Comparing `gad_common_utils-0.20/.github/workflows/black-format-checker.yml` & `gad_common_utils-0.21/.github/workflows/black-format-checker.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/.github/workflows/publish-to-pypi.yml` & `gad_common_utils-0.21/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/.github/workflows/pytest.yml` & `gad_common_utils-0.21/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/PKG-INFO` & `gad_common_utils-0.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad_common_utils
-Version: 0.20
+Version: 0.21
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.20/common_utils/data_loading_management.py` & `gad_common_utils-0.21/common_utils/data_loading_management.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/data_type_conversion.py` & `gad_common_utils-0.21/common_utils/data_type_conversion.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/date_time_methods.py` & `gad_common_utils-0.21/common_utils/date_time_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/dynamodb_methods.py` & `gad_common_utils-0.21/common_utils/dynamodb_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/files_methods.py` & `gad_common_utils-0.21/common_utils/files_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/gad_utils.py` & `gad_common_utils-0.21/common_utils/gad_utils.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/gad_utils_additionals.py` & `gad_common_utils-0.21/common_utils/gad_utils_additionals.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/json_schema_methods.py` & `gad_common_utils-0.21/common_utils/json_schema_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/run_athena_query.py` & `gad_common_utils-0.21/common_utils/run_athena_query.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/s3_methods.py` & `gad_common_utils-0.21/common_utils/s3_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/common_utils/string_transformations.py` & `gad_common_utils-0.21/common_utils/string_transformations.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/gad_common_utils.egg-info/PKG-INFO` & `gad_common_utils-0.21/gad_common_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gad-common-utils
-Version: 0.20
+Version: 0.21
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.20/gad_common_utils.egg-info/SOURCES.txt` & `gad_common_utils-0.21/gad_common_utils.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.gitignore
 .pre-commit-config.yaml
 Readme.md
 pyproject.toml
 .github/workflows/black-format-checker.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/pytest.yml
 common_utils/Readme.md
@@ -14,19 +15,16 @@
 common_utils/dynamodb_ray.py
 common_utils/files_methods.py
 common_utils/gad_utils.py
 common_utils/gad_utils_additionals.py
 common_utils/json_schema_methods.py
 common_utils/run_athena_query.py
 common_utils/s3_methods.py
+common_utils/sql_methods.py
 common_utils/string_transformations.py
-common_utils/__pycache__/__init__.cpython-310.pyc
-common_utils/__pycache__/json_schema_methods.cpython-310.pyc
 gad_common_utils.egg-info/PKG-INFO
 gad_common_utils.egg-info/SOURCES.txt
 gad_common_utils.egg-info/dependency_links.txt
 gad_common_utils.egg-info/requires.txt
 gad_common_utils.egg-info/top_level.txt
 tests/__init__.py
-tests/test_json_schema_methods.py
-tests/__pycache__/__init__.cpython-310.pyc
-tests/__pycache__/test_json_schema_methods.cpython-310-pytest-7.2.2.pyc
+tests/test_json_schema_methods.py
```

### Comparing `gad_common_utils-0.20/pyproject.toml` & `gad_common_utils-0.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.20/tests/test_json_schema_methods.py` & `gad_common_utils-0.21/tests/test_json_schema_methods.py`

 * *Files identical despite different names*

