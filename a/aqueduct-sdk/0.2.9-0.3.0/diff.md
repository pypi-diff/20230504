# Comparing `tmp/aqueduct-sdk-0.2.9.tar.gz` & `tmp/aqueduct-sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-sdk-0.2.9.tar", last modified: Wed Apr  5 19:17:31 2023, max compression
+gzip compressed data, was "aqueduct-sdk-0.3.0.tar", last modified: Thu May  4 05:04:36 2023, max compression
```

## Comparing `aqueduct-sdk-0.2.9.tar` & `aqueduct-sdk-0.3.0.tar`

### file list

```diff
@@ -1,111 +1,118 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6944 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1474 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/artifacts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/base_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/bool_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/generic_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11574 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/numeric_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6632 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/preview.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/system_metric.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24898 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/table_artifact.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/backend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/backend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22951 2023-04-04 21:44:50.000000 aqueduct-sdk-0.2.9/aqueduct/backend/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6404 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/backend/response_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7033 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/backend/response_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32293 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/constants/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/constants/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6511 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/constants/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/constants/exports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/constants/metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45150 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/decorator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3637 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6366 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4450 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/flow_run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8272 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/github.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/globals/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/globals/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/globals/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/globals/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/globals/dag.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/integrations/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/airflow_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      659 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/aws_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11711 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/connect_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/databricks_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7231 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/dynamic_k8s_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4767 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/google_sheets_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      469 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/k8s_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      472 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/lambda_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8850 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/mongodb_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/parameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8924 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/s3_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/salesforce_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3208 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/save.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/spark_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11770 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/sql_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/logger.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      507 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/models/artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1733 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/models/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19371 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/models/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2814 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/models/dag_rules.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2279 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/models/integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7459 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/models/operators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2759 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/schedule.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/connect_config_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/dag_delta_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/dag_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/decorator_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/decorators_with_without_parentheses_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/enum_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/flow_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/helpers_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/metric_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/naming_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15599 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/serialization_test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/python_function.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/test_dependency_folder/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6072 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/type_annotations.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/aqueduct/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10504 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/dag_deltas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/utils/describe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/format.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/function_packaging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1946 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/local_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/naming.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14431 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/type_inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7700 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6944 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3121 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/requirements/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/requirements/python-3-10.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/requirements/python-3-7.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/requirements/python-3-8.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/requirements/python-3-9.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1104 2023-04-04 22:01:25.000000 aqueduct-sdk-0.2.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.160962 aqueduct-sdk-0.3.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7511 2023-05-04 05:04:36.160962 aqueduct-sdk-0.3.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.140962 aqueduct-sdk-0.3.0/aqueduct/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.144963 aqueduct-sdk-0.3.0/aqueduct/artifacts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/base_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/bool_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/generic_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/numeric_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6599 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/preview.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/system_metric.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24895 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/artifacts/table_artifact.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.144963 aqueduct-sdk-0.3.0/aqueduct/backend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/backend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24487 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/backend/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/backend/response_helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34643 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.144963 aqueduct-sdk-0.3.0/aqueduct/constants/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/constants/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6666 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/constants/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/constants/exports.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/constants/metrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52868 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/decorator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3930 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/error.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5525 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/flow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/flow_run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8269 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/github.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.144963 aqueduct-sdk-0.3.0/aqueduct/globals/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/globals/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/globals/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/globals/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/globals/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8354 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/llm_wrapper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/logger.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.148963 aqueduct-sdk-0.3.0/aqueduct/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/models/artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/models/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19371 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/models/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/models/dag_rules.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/models/execution_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3099 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/models/integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7640 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/models/operators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9747 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/models/response_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/models/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.148963 aqueduct-sdk-0.3.0/aqueduct/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/airflow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/aws.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      464 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/aws_lambda.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13077 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/connect_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/databricks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/dynamic_k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1787 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/ecr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4878 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/google_sheets.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8993 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/parameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9035 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5519 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/salesforce.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3199 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/save.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/spark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12065 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      687 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/resources/validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/schedule.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.152963 aqueduct-sdk-0.3.0/aqueduct/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/tests/connect_config_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/tests/dag_delta_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/dag_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/tests/decorator_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/decorators_with_without_parentheses_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/enum_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/flow_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/tests/helpers_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/metric_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/tests/naming_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15641 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/tests/serialization_test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.152963 aqueduct-sdk-0.3.0/aqueduct/tests/test_files/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/test_files/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.152963 aqueduct-sdk-0.3.0/aqueduct/tests/test_files/python_function/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/test_files/python_function/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/test_files/python_function/python_function.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.156962 aqueduct-sdk-0.3.0/aqueduct/tests/test_files/python_function/test_dependency_folder/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/tests/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/type_annotations.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.156962 aqueduct-sdk-0.3.0/aqueduct/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10504 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/utils/dag_deltas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/utils/describe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/utils/format.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/utils/function_packaging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/utils/integration_validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/utils/local_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/utils/naming.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16432 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/utils/serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-03-07 22:19:47.000000 aqueduct-sdk-0.3.0/aqueduct/utils/type_inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8505 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/aqueduct/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.156962 aqueduct-sdk-0.3.0/aqueduct_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7511 2023-05-04 05:04:36.000000 aqueduct-sdk-0.3.0/aqueduct_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-05-04 05:04:36.000000 aqueduct-sdk-0.3.0/aqueduct_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-04 05:04:36.000000 aqueduct-sdk-0.3.0/aqueduct_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-04 05:04:36.000000 aqueduct-sdk-0.3.0/aqueduct_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-04 05:04:36.000000 aqueduct-sdk-0.3.0/aqueduct_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:04:36.160962 aqueduct-sdk-0.3.0/requirements/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/requirements/python-3-10.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/requirements/python-3-7.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/requirements/python-3-8.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/requirements/python-3-9.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-04 05:04:36.160962 aqueduct-sdk-0.3.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-04 03:10:27.000000 aqueduct-sdk-0.3.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-04 03:12:43.000000 aqueduct-sdk-0.3.0/version
```

### Comparing `aqueduct-sdk-0.2.9/PKG-INFO` & `aqueduct-sdk-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.2.9
-Summary: Python SDK for the Aqueduct prediction infrastructure
+Version: 0.3.0
+Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-[<img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width= "35%" />](https://www.aqueducthq.com)
 
-## Aqueduct: The easiest way to run ML on any cloud
 
+<div align="center">
+  <a href="https://aqueducthq.com">
+    <img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width="40%" />
+  </a>
+  
+  <h2 style="border: 0px white;">The Python API to run machine learning in your cloud</h2>
+
+### 📢 [Slack](https://slack.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🗺️ [Roadmap](https://roadmap.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🐞 [Report a bug](https://github.com/aqueducthq/aqueduct/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5BBUG%5D)&nbsp;&nbsp;|&nbsp;&nbsp;✍️ [Blog](https://blog.aqueducthq.com)
+
+  
 [![Start Sandbox](https://img.shields.io/static/v1?label=%20&logo=github&message=Start%20Sandbox&color=black)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=496844646)
 [![Downloads](https://pepy.tech/badge/aqueduct-ml/month)](https://pypi.org/project/aqueduct-ml/)
 [![Slack](https://img.shields.io/static/v1.svg?label=chat&message=on%20slack&color=27b1ff&style=flat)](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A)
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/aqueducthq/aqueduct/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/aqueduct-ml.svg)](https://pypi.org/project/aqueduct-ml/)
 [![Tests](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml)
+</div>
+
+**Aqueduct enables you to easily define, run, and manage AI & ML tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
-**Aqueduct enables you to easily run machine learning tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/867892/230214641-b0aec53b-4988-4581-84ed-134f97ed9276.png" width="80%" />
+</p>
 
-Aqueduct is an open-source MLOps framework that allows you to define ML tasks in vanilla Python, run those tasks on any infrastructure you'd like to use, and gain visibility into the execution and performance of your ML. **[See what tools Aqueduct works with. →](https://aqueducthq.com/integrations/)**
+Aqueduct is an open-source MLOps framework that allows you to write code in vanilla Python, run that code on any cloud infrastructure you'd like to use, and gain visibility into the execution and performance of your models and predictions. **[See what infrastructure Aqueduct works with. →](https://aqueducthq.com/integrations/)**
 
 Here's how you can get started: 
 
 ```bash
 pip3 install aqueduct-ml
 aqueduct start
 ```
@@ -92,8 +105,8 @@
 * and more details on [creating workflows](https://docs.aqueducthq.com/workflows)
 
 If you have questions or comments or would like to learn more about what we're
 building, please [reach out](mailto:hello@aqueducthq.com), [join our Slack
 channel](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A), or [start a conversation on GitHub](https://github.com/aqueducthq/aqueduct/issues/new).
 We'd love to hear from you!
 
-If you're interested in contributing, please check out our [roadmap](https://github.com/aqueducthq/aqueduct/wiki/Aqueduct-Roadmap) and join the development channel in [our community Slack](https://slack.aqueducthq.com).
+If you're interested in contributing, please check out our [roadmap](https://roadmap.aqueducthq.com) and join the development channel in [our community Slack](https://slack.aqueducthq.com).
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/__init__.py` & `aqueduct-sdk-0.3.0/aqueduct/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, List
 
 from aqueduct.client import Client, get_apikey, global_config
 from aqueduct.constants import exports
 from aqueduct.constants.enums import CheckSeverity, LoadUpdateMode
 from aqueduct.decorator import check, metric, op, to_operator
 from aqueduct.flow import Flow
+from aqueduct.llm_wrapper import llm_op, supported_llms
 from aqueduct.schedule import DayOfMonth, DayOfWeek, Hour, Minute, daily, hourly, monthly, weekly
 
 
 # Retrieves all valid import paths for all variables in a given module, using the import path prefix
 # When you add a constant module, call this function to generate a
 # `aqueduct.SUPPORTED_<MODULE_NAME>` field to let user know valid import paths
 # for your module.
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/artifacts/_create.py` & `aqueduct-sdk-0.3.0/aqueduct/artifacts/_create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/artifacts/base_artifact.py` & `aqueduct-sdk-0.3.0/aqueduct/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/artifacts/bool_artifact.py` & `aqueduct-sdk-0.3.0/aqueduct/artifacts/bool_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/artifacts/create.py` & `aqueduct-sdk-0.3.0/aqueduct/artifacts/create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/artifacts/generic_artifact.py` & `aqueduct-sdk-0.3.0/aqueduct/artifacts/generic_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/artifacts/numeric_artifact.py` & `aqueduct-sdk-0.3.0/aqueduct/artifacts/numeric_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,16 +178,16 @@
             bound_value = value
 
         if not param_found:
             raise AqueductError(
                 "Could not find a parameter for bounding the metric please specify one of either: %s"
                 % (",".join(input_mapping.keys()))
             )
-
-        assert bound_name and bound_value
+        # Specify is not None because otherwise will incorrectly capture Falsey values e.g. 0, "" is a Falsey value
+        assert bound_name is not None and bound_value is not None
 
         accepted_types = [float, int]
         if type(bound_value) not in accepted_types:
             raise AqueductError(
                 "Value for bound '%s' must be one of %s type, found %s"
                 % (
                     bound_name,
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/artifacts/preview.py` & `aqueduct-sdk-0.3.0/aqueduct/artifacts/preview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import uuid
 from typing import Any, Dict, List, Optional
 
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.create import to_artifact_class
-from aqueduct.backend.response_models import ArtifactResult
 from aqueduct.constants.enums import ArtifactType, K8sClusterStatusType
-from aqueduct.error import InvalidArtifactTypeException, InvalidIntegrationException
+from aqueduct.error import InvalidArtifactTypeException
 from aqueduct.models.config import EngineConfig
 from aqueduct.models.dag import DAG
+from aqueduct.models.response_models import ArtifactResult
 from aqueduct.utils.dag_deltas import SubgraphDAGDelta, UpdateParametersDelta, apply_deltas_to_dag
 from aqueduct.utils.serialization import deserialize
 from aqueduct.utils.type_inference import infer_artifact_type
 from aqueduct.utils.utils import generate_engine_config
 
 from aqueduct import globals
 
@@ -33,34 +33,34 @@
     dag: DAG, target_artifact_ids: List[uuid.UUID], parameters: Optional[Dict[str, Any]] = None
 ) -> List[BaseArtifact]:
     """Batch version of `preview_artifact()`
 
     Returns a list of artifacts, each corresponding to one of the provided `target_artifact_ids`, in
     the same order.
     """
+    global_engine_config: Optional[EngineConfig] = None
+    if globals.__GLOBAL_CONFIG__.engine is not None:
+        global_engine_config = generate_engine_config(
+            globals.__GLOBAL_API_CLIENT__.list_resources(),
+            globals.__GLOBAL_CONFIG__.engine,
+        )
+
     subgraph = apply_deltas_to_dag(
         dag,
         deltas=[
             SubgraphDAGDelta(
                 artifact_ids=target_artifact_ids,
                 include_saves=False,
             ),
             UpdateParametersDelta(
                 parameters=parameters,
             ),
         ],
         make_copy=True,
     )
-
-    global_engine_config: Optional[EngineConfig] = None
-    if globals.__GLOBAL_CONFIG__.engine is not None:
-        global_engine_config = generate_engine_config(
-            globals.__GLOBAL_API_CLIENT__.list_integrations(),
-            globals.__GLOBAL_CONFIG__.engine,
-        )
     subgraph.set_engine_config(global_engine_config=global_engine_config)
 
     engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status_by_dag(dag=subgraph)
     for name in engine_statuses:
         engine_status = engine_statuses[name]
         if engine_status.status != K8sClusterStatusType.ACTIVE:
             print(
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/artifacts/system_metric.py` & `aqueduct-sdk-0.3.0/aqueduct/artifacts/system_metric.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/artifacts/table_artifact.py` & `aqueduct-sdk-0.3.0/aqueduct/artifacts/table_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         assert isinstance(content, pd.DataFrame)
         return content
 
     def head(self, n: int = 5, parameters: Optional[Dict[str, Any]] = None) -> pd.DataFrame:
         """Returns a preview of the table artifact.
 
-        >>> db = client.integration(name="demo/")
+        >>> db = client.resource(name="demo/")
         >>> customer_data = db.sql("SELECT * from customers")
         >>> churn_predictions = predict_churn(customer_data)
         >>> churn_predictions.head()
 
         Args:
             n:
                 the number of row previewed. Default to 5.
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/backend/api_client.py` & `aqueduct-sdk-0.3.0/aqueduct/backend/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,37 +13,39 @@
     InvalidUserActionException,
     NoConnectedIntegrationsException,
     ResourceNotFoundError,
     UnprocessableEntityError,
 )
 from aqueduct.logger import logger
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import Integration, IntegrationInfo
+from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import ParamSpec
-from aqueduct.utils.serialization import deserialize
-from pkg_resources import get_distribution, parse_version
-
-from ..integrations.connect_config import DynamicK8sConfig, IntegrationConfig
-from .response_helpers import (
-    _construct_preview_response,
-    _handle_preview_resp,
-    _parse_artifact_result_response,
-)
-from .response_models import (
+from aqueduct.models.response_models import (
     DeleteWorkflowResponse,
     DynamicEngineStatusResponse,
+    GetImageURLResponse,
     GetVersionResponse,
+    GetWorkflowDagResultResponse,
     GetWorkflowResponse,
     ListWorkflowResponseEntry,
     ListWorkflowSavedObjectsResponse,
     PreviewResponse,
     RegisterAirflowWorkflowResponse,
     RegisterWorkflowResponse,
     SavedObjectUpdate,
 )
+from aqueduct.utils.serialization import deserialize
+from pkg_resources import get_distribution, parse_version
+
+from ..resources.connect_config import DynamicK8sConfig, ResourceConfig
+from .response_helpers import (
+    _construct_preview_response,
+    _handle_preview_resp,
+    _parse_artifact_result_response,
+)
 
 # The maximum http request size is capped at 32 MB. DAG containing
 # local data parameter(s) should not go beyond this value.
 MAX_REQUEST_BODY_SIZE = 32 << 20
 
 
 class APIClient:
@@ -59,28 +61,31 @@
     DELETE_INTEGRATION_ROUTE_TEMPLATE = "/api/integration/%s/delete"
     PREVIEW_ROUTE = "/api/preview"
     REGISTER_WORKFLOW_ROUTE = "/api/workflow/register"
     REGISTER_AIRFLOW_WORKFLOW_ROUTE = "/api/workflow/register/airflow"
     LIST_INTEGRATIONS_ROUTE = "/api/integrations"
     LIST_INTEGRATION_OBJECTS_ROUTE_TEMPLATE = "/api/integration/%s/objects"
     GET_WORKFLOW_ROUTE_TEMPLATE = "/api/workflow/%s"
+    GET_WORKFLOW_DAG_RESULT_TEMPLATE = "/api/workflow/%s/result/%s"
     LIST_WORKFLOW_SAVED_OBJECTS_ROUTE = "/api/workflow/%s/objects"
     GET_ARTIFACT_RESULT_TEMPLATE = "/api/artifact/%s/%s/result"
 
     LIST_WORKFLOWS_ROUTE = "/api/workflows"
     REFRESH_WORKFLOW_ROUTE_TEMPLATE = "/api/workflow/%s/refresh"
     DELETE_WORKFLOW_ROUTE_TEMPLATE = "/api/workflow/%s/delete"
     LIST_GITHUB_REPO_ROUTE = "/api/integrations/github/repos"
     LIST_GITHUB_BRANCH_ROUTE = "/api/integrations/github/branches"
     NODE_POSITION_ROUTE = "/api/positioning"
     EXPORT_FUNCTION_ROUTE = "/api/function/%s/export"
 
     GET_DYNAMIC_ENGINE_STATUS_ROUTE = "/api/integration/dynamic-engine/status"
     EDIT_DYNAMIC_ENGINE_ROUTE_TEMPLATE = "/api/integration/dynamic-engine/%s/edit"
 
+    GET_IMAGE_URL_ROUTE = "/api/integration/container-registry/url"
+
     # Auth header
     API_KEY_HEADER = "api-key"
 
     configured = False
 
     def raise_errors(self, response: requests.Response) -> None:
         def _extract_err_msg() -> str:
@@ -213,26 +218,26 @@
         self.raise_errors(resp)
         return GetVersionResponse(**resp.json()).version
 
     def url_prefix(self) -> str:
         self._check_config()
         return self.HTTPS_PREFIX if self.use_https else self.HTTP_PREFIX
 
-    def list_integrations(self) -> Dict[str, IntegrationInfo]:
+    def list_resources(self) -> Dict[str, ResourceInfo]:
         url = self.construct_full_url(self.LIST_INTEGRATIONS_ROUTE)
         headers = self._generate_auth_headers()
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
         if len(resp.json()) == 0:
             raise NoConnectedIntegrationsException(
                 "Unable to create flow. Must be connected to at least one integration!"
             )
 
         return {
-            integration_info["name"]: IntegrationInfo(**integration_info)
+            integration_info["name"]: ResourceInfo(**integration_info)
             for integration_info in resp.json()
         }
 
     def list_github_repos(self) -> List[str]:
         url = self.construct_full_url(self.LIST_GITHUB_REPO_ROUTE)
         headers = self._generate_auth_headers()
 
@@ -255,15 +260,15 @@
         headers = self._generate_auth_headers()
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
 
         return [x for x in resp.json()["object_names"]]
 
     def connect_integration(
-        self, name: str, service: Union[str, ServiceType], config: IntegrationConfig
+        self, name: str, service: Union[str, ServiceType], config: ResourceConfig
     ) -> None:
         integration_service = service
         if isinstance(integration_service, ServiceType):
             # The enum value needs to be used
             integration_service = integration_service.value
 
         headers = self._generate_auth_headers()
@@ -500,15 +505,15 @@
 
         response = requests.post(url, headers=headers, data=body)
         self.raise_errors(response)
 
     def delete_workflow(
         self,
         flow_id: str,
-        saved_objects_to_delete: DefaultDict[Union[str, Integration], List[SavedObjectUpdate]],
+        saved_objects_to_delete: DefaultDict[Union[str, BaseResource], List[SavedObjectUpdate]],
         force: bool,
     ) -> DeleteWorkflowResponse:
         headers = self._generate_auth_headers()
         url = self.construct_full_url(self.DELETE_WORKFLOW_ROUTE_TEMPLATE % flow_id)
         body = {
             "external_delete": {
                 str(integration): [obj.spec.json() for obj in saved_objects_to_delete[integration]]
@@ -521,16 +526,22 @@
         return DeleteWorkflowResponse(**response.json())
 
     def get_workflow(self, flow_id: str) -> GetWorkflowResponse:
         headers = self._generate_auth_headers()
         url = self.construct_full_url(self.GET_WORKFLOW_ROUTE_TEMPLATE % flow_id)
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
-        workflow_response = GetWorkflowResponse(**resp.json())
-        return workflow_response
+        return GetWorkflowResponse(**resp.json())
+
+    def get_workflow_dag_result(self, flow_id: str, result_id: str) -> GetWorkflowDagResultResponse:
+        headers = self._generate_auth_headers()
+        url = self.construct_full_url(self.GET_WORKFLOW_DAG_RESULT_TEMPLATE % (flow_id, result_id))
+        resp = requests.get(url, headers=headers)
+        self.raise_errors(resp)
+        return GetWorkflowDagResultResponse(**resp.json())
 
     def list_saved_objects(self, flow_id: str) -> ListWorkflowSavedObjectsResponse:
         headers = self._generate_auth_headers()
         url = self.construct_full_url(self.LIST_WORKFLOW_SAVED_OBJECTS_ROUTE % flow_id)
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
         workflow_writes_response = ListWorkflowSavedObjectsResponse(**resp.json())
@@ -554,17 +565,48 @@
         )
         resp = requests.get(url, headers=headers)
         self.raise_errors(resp)
 
         parsed_response = _parse_artifact_result_response(resp)
         execution_status = parsed_response["metadata"]["exec_state"]["status"]
 
-        if execution_status != ExecutionStatus.SUCCEEDED:
-            print("Artifact result unavailable due to unsuccessful execution.")
-            return None, execution_status
-
         serialization_type = parsed_response["metadata"]["serialization_type"]
         artifact_type = parsed_response["metadata"]["artifact_type"]
-        return (
-            deserialize(serialization_type, artifact_type, parsed_response["data"]),
-            execution_status,
-        )
+
+        return_value = None
+        if "data" in parsed_response:
+            return_value = deserialize(serialization_type, artifact_type, parsed_response["data"])
+
+        if execution_status != ExecutionStatus.SUCCEEDED:
+            logger().warning("Artifact result unavailable due to unsuccessful execution.")
+
+        return (return_value, execution_status)
+
+    def get_image_url(
+        self,
+        integration_id: str,
+        service: ServiceType,
+        image_name: str,
+    ) -> GetImageURLResponse:
+        """Makes a request against the /api/integration/container-registry/url endpoint.
+
+        Args:
+            integration_id:
+                Container registry integration ID.
+            service:
+                Container registry service type.
+            image_name:
+                Image name to get the URL for.
+
+        Returns:
+            GetImageURLResponse that contains the URL to the image.
+        """
+        headers = self._generate_auth_headers()
+        headers["integration-id"] = integration_id
+        headers["service"] = service.value
+        headers["image-name"] = image_name
+
+        url = self.construct_full_url(self.GET_IMAGE_URL_ROUTE)
+        resp = requests.get(url, headers=headers)
+        self.raise_errors(resp)
+
+        return GetImageURLResponse(**resp.json())
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/backend/response_helpers.py` & `aqueduct-sdk-0.3.0/aqueduct/backend/response_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from typing import Any, Dict, List
 
 import multipart
 import requests
 from aqueduct.constants.enums import ExecutionStatus
 from aqueduct.error import AqueductError, InternalAqueductError
 from aqueduct.models.dag import DAG
+from aqueduct.models.execution_state import ExecutionState, Logs
 from aqueduct.models.operators import Operator
-from aqueduct.utils.utils import indent_multiline_string, is_string_valid_uuid
+from aqueduct.models.response_models import ArtifactResult, PreviewResponse
+from aqueduct.utils.utils import is_string_valid_uuid, print_logs
 from requests_toolbelt.multipart import decoder
 
-from .response_models import ArtifactResult, ExecutionState, Logs, PreviewResponse
-
 
 def _parse_artifact_result_response(response: requests.Response) -> Dict[str, Any]:
     multipart_data = decoder.MultipartDecoder.from_response(response)
     parse = multipart.parse_options_header
 
     result = {}
 
@@ -33,15 +33,14 @@
             )
 
     return result
 
 
 def _construct_preview_response(response: requests.Response) -> PreviewResponse:
     artifact_results = {}
-    artifact_result_constructor = {}
     preview_response = {}
     is_metadata_received = False
     multipart_data = decoder.MultipartDecoder.from_response(response)
     parse = multipart.parse_options_header
 
     for part in multipart_data.parts:
         field_name = part.headers[b"Content-Disposition"].decode(multipart_data.encoding)
@@ -94,14 +93,15 @@
             f"{op_result.error.tip}\n"
             f"\n"
         )
 
     def _print_op_user_logs(op_name: str, logs: Logs) -> None:
         """Prints out the logs for a single operator. The format is:
 
+        Operator {op_name} Logs:
         stdout:
             {logs}
             {logs}
         ----------------------------------
         stderr:
             {logs}
             {logs}
@@ -109,24 +109,15 @@
         If either stdout or stderr is empty, we do not print anything for
         the empty section, and do not draw the "--" delimiter line.
         """
         if logs.is_empty():
             return
 
         print(f"Operator {op_name} Logs:")
-        if len(logs.stdout) > 0:
-            print("stdout:")
-            print(indent_multiline_string(logs.stdout).rstrip("\n"))
-
-        if len(logs.stdout) > 0 and len(logs.stderr) > 0:
-            print("----------------------------------")
-
-        if len(logs.stderr) > 0:
-            print("stderr:")
-            print(indent_multiline_string(logs.stderr).rstrip("\n"))
+        print_logs(logs)
         print("")
 
     q: List[Operator] = dag.list_root_operators()
     seen_op_ids = set(op.id for op in q)
     while len(q) > 0:
         curr_op = q.pop(0)
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/backend/response_models.py` & `aqueduct-sdk-0.3.0/aqueduct/models/response_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,25 @@
 import uuid
+from datetime import datetime
 from typing import Dict, List, Optional
 
 from aqueduct.constants.enums import (
     ArtifactType,
     ExecutionStatus,
-    FailureType,
     K8sClusterStatusType,
     SerializationType,
 )
 from aqueduct.models.artifact import ArtifactMetadata
-from aqueduct.models.dag import Metadata
-from aqueduct.models.operators import LoadSpec, Operator
-from aqueduct.utils.utils import human_readable_timestamp
+from aqueduct.models.dag import Metadata, RetentionPolicy, Schedule
+from aqueduct.models.execution_state import ExecutionState
+from aqueduct.models.operators import LoadSpec, Operator, OperatorSpec
+from aqueduct.models.utils import human_readable_timestamp
 from pydantic import BaseModel
 
 
-class Logs(BaseModel):
-    stdout: str = ""
-    stderr: str = ""
-
-    def is_empty(self) -> bool:
-        return self.stdout == "" and self.stderr == ""
-
-
-class Error(BaseModel):
-    context: str = ""
-    tip: str = ""
-
-
-class ExecutionState(BaseModel):
-    user_logs: Optional[Logs] = None
-    error: Optional[Error] = None
-    status: ExecutionStatus = ExecutionStatus.UNKNOWN
-    failure_type: Optional[FailureType] = None
-
-
 class ArtifactResult(BaseModel):
     serialization_type: SerializationType
     artifact_type: ArtifactType
     content: bytes
 
 
 class PreviewResponse(BaseModel):
@@ -64,17 +45,20 @@
 
 class RegisterWorkflowResponse(BaseModel):
     """This is the response object returned by api_client.register_workflow().
 
     Attributes:
         id:
             The uuid if of the newly registered workflow.
+        python_version:
+            The Python version in the engine in string format "Python {major_version}.{minor_version}.{patch_level}" e.g. "Python 3.9.11".
     """
 
     id: uuid.UUID
+    python_version: str
 
 
 class RegisterAirflowWorkflowResponse(BaseModel):
     """This is the response object returned by api_client.register_airflow_workflow().
 
     Attributes:
         id:
@@ -145,26 +129,30 @@
     workflow_id: uuid.UUID
     metadata: Metadata
     operators: Dict[str, Operator]
     artifacts: Dict[str, ArtifactMetadata]
 
 
 class WorkflowDagResultResponse(BaseModel):
-    """Represents the result of a single workflwo run.
+    """Represents the result of a single workflow run.
+
+    NOTE: Very confusingly, this is not the response from `get_workflow_dag_result.go`, but instead is
+    derived from the `get_workflow.go` response.
 
     Attributes:
         id:
             The id of the workflow run. This is the same id users can use to fetch
             FlowRuns.
         created_at:
             The unix timestamp in seconds that this workflow run was started at.
         status:
             The execution status of this workflow run.
         workflow_dag_id:
             This id can be used to find the corresponding workflow dag version.
+
     """
 
     id: uuid.UUID
     created_at: int
 
     # TODO(ENG-2665): remove the status field.
     status: ExecutionStatus
@@ -195,28 +183,111 @@
         watcher_auth_ids
     """
 
     workflow_dags: Dict[uuid.UUID, WorkflowDagResponse]
     workflow_dag_results: List[WorkflowDagResultResponse]
 
 
+class WorkflowDagResultResultResponse(BaseModel):
+    """A workflow dag result's execution state, derived from api_client.get_workflow_dag_result()."""
+
+    id: uuid.UUID
+    exec_state: ExecutionState
+
+
+class OperatorRawResultResponse(BaseModel):
+    """An operator result's execution state, derived from api_client.get_workflow_dag_result()."""
+
+    id: uuid.UUID
+    exec_state: ExecutionState
+
+
+class ArtifactRawResultResponse(BaseModel):
+    """An artifact result's execution state, derived from api_client.get_workflow_dag_result()."""
+
+    id: uuid.UUID
+    exec_state: ExecutionState
+
+
+class OperatorResultResponse(BaseModel):
+    """An operator result, derived from the returned response from api_client.get_workflow_dag_result()."""
+
+    # Copied from the Operator class, because the golang response nests that class
+    # in a way that is hard to represent in pydantic.
+    id: uuid.UUID
+    name: str
+    description: str
+    spec: OperatorSpec
+    inputs: List[uuid.UUID] = []
+    outputs: List[uuid.UUID] = []
+
+    # The operator execution result.
+    result: Optional[OperatorRawResultResponse]
+
+    def to_operator(self) -> Operator:
+        """Convert to an operator class."""
+        return Operator(**self.dict())
+
+
+class ArtifactResultResponse(BaseModel):
+    """An artifact result, derived from the returned response from api_client.get_workflow_dag_result().
+
+    Excluded attributes:
+    - from: the upstream operator ID. Also, "from" is a reserved keyword in pydantic.
+    - to: the downstream operator IDs.
+    """
+
+    # Copied from the ArtifactMetadata class, because the golang response nests that class
+    # in a way that is hard to represent in pydantic.
+    id: uuid.UUID
+    name: str
+    type: ArtifactType
+
+    def to_artifact(self) -> ArtifactMetadata:
+        """Convert to an artifact class."""
+        return ArtifactMetadata(**self.dict())
+
+
+class GetWorkflowDagResultResponse(BaseModel):
+    """This is the response object returned by api_client.get_workflow_dag_result().
+
+    Excluded attributes:
+        Only the necessary metadata fields are included.
+    """
+
+    # This is a subset of what metadata is available on the backend.
+    # Allows for this object to be cast into a Metadata object.
+    name: Optional[str]
+    description: Optional[str]
+    schedule: Optional[Schedule]
+    retention_policy: Optional[RetentionPolicy]
+    dag_created_at: datetime
+
+    result: WorkflowDagResultResultResponse
+    operators: Dict[uuid.UUID, OperatorResultResponse]
+    artifacts: Dict[uuid.UUID, ArtifactResultResponse]
+
+    def metadata(self) -> Metadata:
+        return Metadata(**self.dict())
+
+
 class SavedObjectDelete(BaseModel):
     """This is an item in the list returned by DeleteWorkflowResponse."""
 
     name: str
     exec_state: ExecutionState
 
 
 class DeleteWorkflowResponse(BaseModel):
     """This is the response object returned by api_client.delete_workflow().
 
     Attributes:
         saved_object_deletion_results:
             Results of deleting saved objects.
-            Key: Integration name
+            Key: Resource name
             Value: List of SavedObjectDelete belonging to that integration
     """
 
     saved_object_deletion_results: Dict[str, List[SavedObjectDelete]]
 
 
 class SavedObjectUpdate(BaseModel):
@@ -245,7 +316,11 @@
     version: str
 
 
 class DynamicEngineStatusResponse(BaseModel):
     id: uuid.UUID
     name: str
     status: K8sClusterStatusType
+
+
+class GetImageURLResponse(BaseModel):
+    url: str
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/client.py` & `aqueduct-sdk-0.3.0/aqueduct/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 import logging
 import os
+import platform
 import uuid
 import warnings
 from collections import defaultdict
 from typing import Any, DefaultDict, Dict, List, Optional, Union
 
 import __main__ as main
 import yaml
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.bool_artifact import BoolArtifact
 from aqueduct.artifacts.create import create_param_artifact
 from aqueduct.artifacts.numeric_artifact import NumericArtifact
-from aqueduct.backend.response_models import SavedObjectUpdate
 from aqueduct.constants.enums import (
     ArtifactType,
     ExecutionStatus,
-    OperatorType,
     RelationalDBServices,
     RuntimeType,
     ServiceType,
 )
 from aqueduct.error import (
     InvalidIntegrationException,
     InvalidUserActionException,
     InvalidUserArgumentException,
 )
 from aqueduct.flow import Flow
 from aqueduct.github import Github
-from aqueduct.integrations.airflow_integration import AirflowIntegration
-from aqueduct.integrations.aws_integration import AWSIntegration
-from aqueduct.integrations.connect_config import (
+from aqueduct.logger import logger
+from aqueduct.models.dag import Metadata, RetentionPolicy
+from aqueduct.models.integration import BaseResource, ResourceInfo
+from aqueduct.models.operators import ParamSpec
+from aqueduct.models.response_models import SavedObjectUpdate
+from aqueduct.resources.airflow import AirflowResource
+from aqueduct.resources.aws import AWSResource
+from aqueduct.resources.aws_lambda import LambdaResource
+from aqueduct.resources.connect_config import (
     BaseConnectionConfig,
-    IntegrationConfig,
+    ResourceConfig,
     convert_dict_to_integration_connect_config,
     prepare_integration_config,
 )
-from aqueduct.integrations.databricks_integration import DatabricksIntegration
-from aqueduct.integrations.google_sheets_integration import GoogleSheetsIntegration
-from aqueduct.integrations.k8s_integration import K8sIntegration
-from aqueduct.integrations.lambda_integration import LambdaIntegration
-from aqueduct.integrations.mongodb_integration import MongoDBIntegration
-from aqueduct.integrations.s3_integration import S3Integration
-from aqueduct.integrations.salesforce_integration import SalesforceIntegration
-from aqueduct.integrations.spark_integration import SparkIntegration
-from aqueduct.integrations.sql_integration import RelationalDBIntegration
-from aqueduct.logger import logger
-from aqueduct.models.dag import Metadata, RetentionPolicy
-from aqueduct.models.integration import Integration, IntegrationInfo
-from aqueduct.models.operators import ParamSpec
+from aqueduct.resources.databricks import DatabricksResource
+from aqueduct.resources.dynamic_k8s import DynamicK8sResource
+from aqueduct.resources.ecr import ECRResource
+from aqueduct.resources.google_sheets import GoogleSheetsResource
+from aqueduct.resources.k8s import K8sResource
+from aqueduct.resources.mongodb import MongoDBResource
+from aqueduct.resources.s3 import S3Resource
+from aqueduct.resources.salesforce import SalesforceResource
+from aqueduct.resources.spark import SparkResource
+from aqueduct.resources.sql import RelationalDBResource
 from aqueduct.utils.dag_deltas import (
     SubgraphDAGDelta,
     apply_deltas_to_dag,
     validate_overwriting_parameters,
 )
 from aqueduct.utils.local_data import validate_local_data
-from aqueduct.utils.serialization import deserialize, extract_val_from_local_data
-from aqueduct.utils.type_inference import _base64_string_to_bytes, infer_artifact_type
+from aqueduct.utils.serialization import extract_val_from_local_data
+from aqueduct.utils.type_inference import infer_artifact_type
 from aqueduct.utils.utils import (
     construct_param_spec,
     find_flow_with_user_supplied_id_and_name,
     generate_engine_config,
     generate_flow_schedule,
     generate_ui_url,
 )
@@ -148,16 +150,16 @@
         logging.basicConfig(format="%(levelname)s:%(message)s", level=logging_level)
 
         if api_key == "":
             api_key = get_apikey()
 
         globals.__GLOBAL_API_CLIENT__.configure(api_key, aqueduct_address)
         self._connected_integrations: Dict[
-            str, IntegrationInfo
-        ] = globals.__GLOBAL_API_CLIENT__.list_integrations()
+            str, ResourceInfo
+        ] = globals.__GLOBAL_API_CLIENT__.list_resources()
         self._dag = globals.__GLOBAL_DAG__
 
         # Will show graph if in an ipynb or Python console, but not if running a Python script.
         self._in_notebook_or_console_context = (not hasattr(main, "__file__")) and (
             not "PYTEST_CURRENT_TEST" in os.environ
         )
 
@@ -227,15 +229,27 @@
             is_local_data=use_local,
         )
 
     def connect_integration(
         self,
         name: str,
         service: Union[str, ServiceType],
-        config: Union[Dict[str, str], IntegrationConfig],
+        config: Union[Dict[str, str], ResourceConfig],
+    ) -> None:
+        """Deprecated. Use `client.connect_resource()` instead."""
+        logger().warning(
+            "client.connect_integration() will be deprecated soon. Use `client.connect_resource() instead."
+        )
+        return self.connect_resource(name, service, config)
+
+    def connect_resource(
+        self,
+        name: str,
+        service: Union[str, ServiceType],
+        config: Union[Dict[str, str], ResourceConfig],
     ) -> None:
         """Connects the Aqueduct server to an integration.
 
         Args:
             name:
                 The name to assign this integration. Will error if an integration with that name
                 already exists.
@@ -246,15 +260,15 @@
                 configuration credentials needed to connect.
         """
         if service not in ServiceType:
             raise InvalidUserArgumentException(
                 "Service argument must match exactly one of the enum values in ServiceType (case-sensitive)."
             )
 
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_integrations()
+        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
         if name in self._connected_integrations.keys():
             raise InvalidUserActionException(
                 "Cannot connect a new integration with name `%s`. An integration with this name already exists."
                 % name
             )
 
         if not isinstance(config, dict) and not isinstance(config, BaseConnectionConfig):
@@ -271,52 +285,93 @@
         globals.__GLOBAL_API_CLIENT__.connect_integration(name, service, config)
         logger().info("Successfully connected to new %s integration `%s`." % (service, name))
 
     def delete_integration(
         self,
         name: str,
     ) -> None:
+        """Deprecated. Use `client.delete_resource()` instead."""
+        logger().warning(
+            "client.delete_integration() will be deprecated soon. Use `client.delete_resource() instead."
+        )
+        return self.delete_resource(name)
+
+    def delete_resource(
+        self,
+        name: str,
+    ) -> None:
         """Deletes the integration from Aqueduct.
 
         Args:
             name:
                 The name of the integration to delete.
         """
-        existing_integrations = globals.__GLOBAL_API_CLIENT__.list_integrations()
+        existing_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
         if name not in existing_integrations.keys():
             raise InvalidIntegrationException("Not connected to integration %s!" % name)
 
         globals.__GLOBAL_API_CLIENT__.delete_integration(existing_integrations[name].id)
 
         # Update the connected integrations cached on this object.
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_integrations()
+        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
+
+    def list_integrations(self) -> Dict[str, ResourceInfo]:
+        """Deprecated. Use `client.list_resources()` instead."""
+        logger().warning(
+            "client.list_integrations() will be deprecated soon. Use `client.list_resources() instead."
+        )
+        return self.list_resources()
 
-    def list_integrations(self) -> Dict[str, IntegrationInfo]:
+    def list_resources(self) -> Dict[str, ResourceInfo]:
         """Retrieves a dictionary of integrations the client can use.
 
         Returns:
             A dictionary mapping from integration name to additional info.
         """
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_integrations()
+        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
         return self._connected_integrations
 
     def integration(
+        self,
+        name: str,
+    ) -> Union[
+        SalesforceResource,
+        S3Resource,
+        GoogleSheetsResource,
+        RelationalDBResource,
+        AirflowResource,
+        K8sResource,
+        LambdaResource,
+        MongoDBResource,
+        DatabricksResource,
+        SparkResource,
+        AWSResource,
+        ECRResource,
+    ]:
+        """Deprecated. Use `client.resource()` instead."""
+        logger().warning(
+            "client.integration() will be deprecated soon. Use `client.resource() instead."
+        )
+        return self.resource(name)
+
+    def resource(
         self, name: str
     ) -> Union[
-        SalesforceIntegration,
-        S3Integration,
-        GoogleSheetsIntegration,
-        RelationalDBIntegration,
-        AirflowIntegration,
-        K8sIntegration,
-        LambdaIntegration,
-        MongoDBIntegration,
-        DatabricksIntegration,
-        SparkIntegration,
-        AWSIntegration,
+        SalesforceResource,
+        S3Resource,
+        GoogleSheetsResource,
+        RelationalDBResource,
+        AirflowResource,
+        K8sResource,
+        LambdaResource,
+        MongoDBResource,
+        DatabricksResource,
+        SparkResource,
+        AWSResource,
+        ECRResource,
     ]:
         """Retrieves a connected integration object.
 
         Args:
             name:
                 The name of the integration
 
@@ -325,74 +380,78 @@
 
         Raises:
             InvalidIntegrationException:
                 An error occurred because the cluster is not connected to the
                 provided integration or the provided integration is of an
                 incompatible type.
         """
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_integrations()
+        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
 
         if name not in self._connected_integrations.keys():
             raise InvalidIntegrationException("Not connected to integration %s!" % name)
 
         integration_info = self._connected_integrations[name]
         if integration_info.service in RelationalDBServices:
-            return RelationalDBIntegration(
+            return RelationalDBResource(
                 dag=self._dag,
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.SALESFORCE:
-            return SalesforceIntegration(
+            return SalesforceResource(
                 dag=self._dag,
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.GOOGLE_SHEETS:
-            return GoogleSheetsIntegration(
+            return GoogleSheetsResource(
                 dag=self._dag,
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.S3:
-            return S3Integration(
+            return S3Resource(
                 dag=self._dag,
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.AIRFLOW:
-            return AirflowIntegration(
+            return AirflowResource(
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.K8S:
-            return K8sIntegration(
+            return K8sResource(
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.LAMBDA:
-            return LambdaIntegration(
+            return LambdaResource(
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.MONGO_DB:
-            return MongoDBIntegration(
+            return MongoDBResource(
                 dag=self._dag,
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.DATABRICKS:
-            return DatabricksIntegration(
+            return DatabricksResource(
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.SPARK:
-            return SparkIntegration(
+            return SparkResource(
                 metadata=integration_info,
             )
         elif integration_info.service == ServiceType.AWS:
             dynamic_k8s_integration_name = "%s:aqueduct_ondemand_k8s" % name
             dynamic_k8s_integration_info = self._connected_integrations[
                 dynamic_k8s_integration_name
             ]
-            return AWSIntegration(
+            return AWSResource(
                 metadata=integration_info,
                 k8s_integration_metadata=dynamic_k8s_integration_info,
             )
+        elif integration_info.service == ServiceType.ECR:
+            return ECRResource(
+                metadata=integration_info,
+            )
         else:
             raise InvalidIntegrationException(
                 "This method does not support loading integration of type %s"
                 % integration_info.service
             )
 
     def list_flows(self) -> List[Dict[str, str]]:
@@ -440,15 +499,15 @@
         )
 
     def publish_flow(
         self,
         name: str,
         description: str = "",
         schedule: str = "",
-        engine: Optional[str] = None,
+        engine: Optional[Union[str, DynamicK8sResource]] = None,
         artifacts: Optional[Union[BaseArtifact, List[BaseArtifact]]] = None,
         metrics: Optional[List[NumericArtifact]] = None,
         checks: Optional[List[BoolArtifact]] = None,
         k_latest_runs: Optional[int] = None,
         source_flow: Optional[Union[Flow, str, uuid.UUID]] = None,
         run_now: Optional[bool] = None,
         use_local: Optional[bool] = False,
@@ -514,15 +573,17 @@
             A flow object handle to be used to fetch information about this productionized flow.
         """
         if not isinstance(name, str) or name == "":
             raise InvalidUserArgumentException(
                 "A non-empty string must be supplied for the flow's name."
             )
 
-        if engine is not None and not isinstance(engine, str):
+        if engine is not None and not (
+            isinstance(engine, str) or isinstance(engine, DynamicK8sResource)
+        ):
             raise InvalidUserArgumentException(
                 "`engine` parameter must be a string, got %s." % type(engine)
             )
 
         if artifacts is None or artifacts == []:
             raise InvalidUserArgumentException(
                 "Must supply at least one artifact to compute when creating a flow."
@@ -624,14 +685,15 @@
         dag.set_engine_config(
             global_engine_config=generate_engine_config(
                 self._connected_integrations,
                 globals.__GLOBAL_CONFIG__.engine,
             ),
             publish_flow_engine_config=generate_engine_config(self._connected_integrations, engine),
         )
+
         dag.validate_and_resolve_artifact_names()
 
         if dag.engine_config.type == RuntimeType.AIRFLOW:
             if run_now is not None:
                 raise InvalidUserArgumentException(
                     "run_now parameter is not supported for Airflow engine."
                 )
@@ -658,15 +720,28 @@
                     Please copy it to your Airflow server to begin execution.""".format(
                         file
                     )
                 )
         else:
             if run_now is None:
                 run_now = True
-            flow_id = globals.__GLOBAL_API_CLIENT__.register_workflow(dag, run_now).id
+            registered_metadata = globals.__GLOBAL_API_CLIENT__.register_workflow(dag, run_now)
+            flow_id = registered_metadata.id
+            server_python_version = (
+                registered_metadata.python_version.strip()
+            )  # Remove newline at the end
+            client_python_version = f"Python {platform.python_version()}"
+            if (
+                dag.engine_config.type == RuntimeType.AQUEDUCT
+                and client_python_version != server_python_version
+            ):
+                warnings.warn(
+                    "There is a mismatch between the Python version on the engine (%s) and the client (%s)."
+                    % (server_python_version, client_python_version)
+                )
 
         url = generate_ui_url(
             globals.__GLOBAL_API_CLIENT__.construct_base_url(),
             str(flow_id),
         )
         print("Url: ", url)
 
@@ -729,15 +804,15 @@
         globals.__GLOBAL_API_CLIENT__.refresh_workflow(flow_id, param_specs)
 
     def delete_flow(
         self,
         flow_id: Optional[Union[str, uuid.UUID]] = None,
         flow_name: Optional[str] = None,
         saved_objects_to_delete: Optional[
-            DefaultDict[Union[str, Integration], List[SavedObjectUpdate]]
+            DefaultDict[Union[str, BaseResource], List[SavedObjectUpdate]]
         ] = None,
         force: bool = False,
     ) -> None:
         """Deletes a flow object.
 
         Args:
             flow_id:
@@ -791,11 +866,11 @@
             )
 
     def describe(self) -> None:
         """Prints out info about this client in a human-readable format."""
         print("============================= Aqueduct Client =============================")
         print("Connected endpoint: %s" % globals.__GLOBAL_API_CLIENT__.aqueduct_address)
         print("Log Level: %s" % logging.getLevelName(logging.root.level))
-        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_integrations()
+        self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
         print("Current Integrations:")
         for integrations in self._connected_integrations:
             print("\t -" + integrations)
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/constants/enums.py` & `aqueduct-sdk-0.3.0/aqueduct/constants/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,21 @@
     SQLITE = "SQLite"
     AIRFLOW = "Airflow"
     K8S = "Kubernetes"
     GCS = "GCS"
     LAMBDA = "Lambda"
     MONGO_DB = "MongoDB"
     CONDA = "Conda"
-    AQUEDUCT_ENGINE = "Aqueduct Engine"
+    AQUEDUCT_ENGINE = "Aqueduct"
     DATABRICKS = "Databricks"
     EMAIL = "Email"
     SLACK = "Slack"
     SPARK = "Spark"
     AWS = "AWS"
+    ECR = "ECR"
 
 
 class RelationalDBServices(str, Enum, metaclass=MetaEnum):
     """Must match the corresponding entries in `ServiceType` exactly."""
 
     POSTGRES = "Postgres"
     SNOWFLAKE = "Snowflake"
@@ -237,14 +238,19 @@
 
 
 class LocalDataSerializationType(str, Enum, metaclass=MetaEnum):
     CSV_TABLE = "csv_table"
     JSON_TABLE = "json_table"
     PARQUET_TABLE = "parquet_table"
     IMAGE = "image"
+    JSON = "json"
+    PICKLE = "pickle"
+    STRING = "string"
+    BYTES = "bytes"
+    TF_KERAS = "tensorflow-keras-model"
 
 
 class K8sClusterActionType(str, Enum, metaclass=MetaEnum):
     CREATE = "create"
     UPDATE = "update"
     DELETE = "delete"
     FORCE_DELETE = "force-delete"
@@ -253,7 +259,8 @@
 # These are keys for resources that users can customize for operators.
 # They are used as dict keys, eg @op(resources={'num_cpus': 1, ...})
 class CustomizableResourceType(str, Enum, metaclass=MetaEnum):
     NUM_CPUS = "num_cpus"
     MEMORY = "memory"
     GPU_RESOURCE_NAME = "gpu_resource_name"
     CUDA_VERSION = "cuda_version"
+    USE_LLM = "use_llm"
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/decorator.py` & `aqueduct-sdk-0.3.0/aqueduct/decorator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
-import uuid
-import warnings
+import io
+import os
+import zipfile
 from functools import wraps
 from typing import Any, Callable, Dict, List, Mapping, Optional, Union, cast
 
 import numpy as np
 from aqueduct.artifacts._create import create_metric_or_check_artifact
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.bool_artifact import BoolArtifact
@@ -15,35 +16,33 @@
     ArtifactType,
     CheckSeverity,
     CustomizableResourceType,
     ExecutionMode,
     FunctionGranularity,
     FunctionType,
     OperatorType,
+    RuntimeType,
 )
 from aqueduct.error import InvalidUserActionException, InvalidUserArgumentException
 from aqueduct.logger import logger
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.operators import (
     CheckSpec,
     FunctionSpec,
+    ImageConfig,
     MetricSpec,
     Operator,
     OperatorSpec,
     ResourceConfig,
     get_operator_type,
 )
+from aqueduct.resources.dynamic_k8s import DynamicK8sResource
 from aqueduct.type_annotations import CheckFunction, MetricFunction, Number, UserFunction
-from aqueduct.utils.dag_deltas import (
-    AddOperatorDelta,
-    DAGDelta,
-    RemoveOperatorDelta,
-    apply_deltas_to_dag,
-)
-from aqueduct.utils.function_packaging import serialize_function
+from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
+from aqueduct.utils.function_packaging import REQUIREMENTS_FILE, serialize_function
 from aqueduct.utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
 from aqueduct.utils.utils import generate_engine_config, generate_uuid
 
 from aqueduct import globals
 
 OutputArtifactFunction = Callable[..., BaseArtifact]
 
@@ -177,22 +176,26 @@
     return output_artifacts if len(output_artifacts) > 1 else output_artifacts[0]
 
 
 def _typecheck_op_decorator_arguments(
     description: Optional[str],
     file_dependencies: Optional[List[str]],
     requirements: Optional[Union[str, List[str]]],
-    engine: Optional[str],
+    engine: Optional[Union[str, DynamicK8sResource]],
     num_outputs: int,
     outputs: Optional[List[str]],
 ) -> None:
     _typecheck_common_decorator_arguments(description, file_dependencies, requirements)
 
-    if engine is not None and not isinstance(engine, str):
-        raise InvalidUserArgumentException("`engine` must be a string.")
+    if engine is not None and not (
+        isinstance(engine, str) or isinstance(engine, DynamicK8sResource)
+    ):
+        raise InvalidUserArgumentException(
+            "`engine` must be a string or a DynamicK8sResource object."
+        )
 
     if num_outputs is not None:
         if not isinstance(num_outputs, int) or num_outputs < 1:
             raise InvalidUserArgumentException("`num_outputs` must be set to a positive integer.")
 
     if outputs is not None:
         if not (isinstance(outputs, str) or isinstance(outputs, List)):
@@ -358,15 +361,15 @@
             "Memory value `%s` not long enough, it must be a number and a two character suffix (eg. 100MB)."
             % memory_str
         )
 
     if memory_str[-2:].upper() == "MB":
         multiplier = 1
     elif memory_str[-2:].upper() == "GB":
-        multiplier = 1000
+        multiplier = 1024
     else:
         raise InvalidUserArgumentException(
             "Memory value `%s` is invalid. It must have a suffix that is one of mb/MB/gb/GB."
             % memory_str,
         )
 
     memory_scalar_str = memory_str[:-2].strip()
@@ -377,40 +380,48 @@
         )
 
     return multiplier * int(memory_scalar_str)
 
 
 def _update_operator_spec_with_engine(
     spec: OperatorSpec,
-    engine: Optional[str] = None,
+    engine: Optional[Union[str, DynamicK8sResource]] = None,
 ) -> None:
     if engine is not None:
         if globals.__GLOBAL_API_CLIENT__ is None:
             raise InvalidUserActionException(
                 "Aqueduct Client was not instantiated! Please create a client and retry."
             )
 
         spec.engine_config = generate_engine_config(
-            globals.__GLOBAL_API_CLIENT__.list_integrations(),
+            globals.__GLOBAL_API_CLIENT__.list_resources(),
             engine,
         )
 
 
 def _update_operator_spec_with_resources(
     spec: OperatorSpec,
+    llm: bool,
     resources: Optional[Dict[str, Any]] = None,
 ) -> None:
+    if llm:
+        if resources is None:
+            resources = {}
+
+        resources[CustomizableResourceType.USE_LLM] = True
+
     if resources is not None:
         if not isinstance(resources, Dict) or any(not isinstance(k, str) for k in resources):
             raise InvalidUserArgumentException("`resources` must be a dictionary with string keys.")
 
         num_cpus = resources.get(CustomizableResourceType.NUM_CPUS)
         memory = resources.get(CustomizableResourceType.MEMORY)
         gpu_resource_name = resources.get(CustomizableResourceType.GPU_RESOURCE_NAME)
         cuda_version = resources.get(CustomizableResourceType.CUDA_VERSION)
+        use_llm = resources.get(CustomizableResourceType.USE_LLM)
 
         if num_cpus is not None and (not isinstance(num_cpus, int) or num_cpus < 0):
             raise InvalidUserArgumentException(
                 "`num_cpus` value must be set to a positive integer."
             )
 
         # `memory` value can be either an int (in MBs) or a string. We will convert it into an integer
@@ -440,27 +451,131 @@
 
         if cuda_version is not None and gpu_resource_name is None:
             raise InvalidUserArgumentException(
                 "`cuda_version` can only be set if a `gpu_resource_name` is specified."
             )
 
         spec.resources = ResourceConfig(
-            num_cpus=num_cpus, memory_mb=memory, gpu_resource_name=gpu_resource_name
+            num_cpus=num_cpus,
+            memory_mb=memory,
+            gpu_resource_name=gpu_resource_name,
+            cuda_version=cuda_version,
+            use_llm=use_llm,
+        )
+
+
+def _check_llm_requirements(spec: OperatorSpec) -> None:
+    assert spec.resources is not None
+
+    min_required_memory = 8192  # 8GB
+
+    if spec.engine_config is not None and spec.engine_config.type is RuntimeType.K8S:
+        # Check to see if the resources meet the constraints of the LLM.
+        requested_gpu = False  # this is what we default to if gpu_resource_name is not specified.
+        requested_memory = 4096  # 4GB, this is what we defaults to if memory is not specified.
+
+        if spec.resources.gpu_resource_name is not None:
+            requested_gpu = True
+        if spec.resources.memory_mb is not None:
+            requested_memory = spec.resources.memory_mb
+
+        if not requested_gpu:
+            raise InvalidUserArgumentException("LLM requires GPU resource but it is not requested.")
+
+        if min_required_memory > requested_memory:
+            raise InvalidUserArgumentException(
+                "LLMs require at least %dMB of memory but only %dMB is requested."
+                % (min_required_memory, requested_memory)
+            )
+
+
+def _check_if_requirements_contain_llm(zip_file: bytes) -> bool:
+    # create a ZipFile instance from the file-like object
+    with zipfile.ZipFile(io.BytesIO(zip_file), "r") as f:
+        # check if requirements.txt is in the archive
+        for filename in f.namelist():
+            # check if the file name is requirements.txt
+            if os.path.basename(filename) == REQUIREMENTS_FILE:
+                with f.open(filename) as requirements_file:
+                    for line in requirements_file:
+                        package_name = line.decode(
+                            "utf-8"
+                        ).strip()  # decode bytes to str and remove whitespace
+
+                        # skip lines that are commented out
+                        if package_name.startswith("#"):
+                            continue
+
+                        # check if aqueduct-llm is one of the requirements
+                        if "aqueduct-llm" in package_name:
+                            return True
+
+    return False
+
+
+def _update_operator_spec_with_image(
+    spec: OperatorSpec,
+    image: Optional[Dict[str, str]] = None,
+) -> None:
+    if image is not None:
+        if spec.engine_config is None or spec.engine_config.type is not RuntimeType.K8S:
+            engine_type = (
+                RuntimeType.AQUEDUCT if spec.engine_config is None else spec.engine_config.type
+            )
+            raise InvalidUserArgumentException(
+                "`image` is only compatible with Kubernetes engine. "
+                "Got engine type: %s. " % engine_type.value
+            )
+
+        if not isinstance(image, Dict) or any(not isinstance(k, str) for k in image):
+            raise InvalidUserArgumentException("`image` must be a dictionary with string keys.")
+
+        registry_name = image.get("registry_name")
+        url = image.get("url")
+
+        if registry_name is None:
+            raise InvalidUserArgumentException(
+                "`registry_name` must be specified when `image` is set."
+            )
+
+        connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
+        if registry_name not in connected_integrations.keys():
+            raise InvalidUserArgumentException(
+                "Registry name `%s` is not one of the connected resources." % registry_name,
+            )
+
+        if url is None:
+            raise InvalidUserArgumentException("`url` must be specified when `image` is set.")
+
+        if len(url.split(":")) != 2:
+            if len(url.split(":")) == 1:
+                url = url + ":latest"
+            else:
+                raise InvalidUserArgumentException(
+                    "Image URL must be in the form of `endpoint/repo:tag`. "
+                    "Such as 123456789012.dkr.ecr.us-east-1.amazonaws.com/my-image:latest."
+                )
+
+        spec.image = ImageConfig(
+            registry_id=str(connected_integrations[registry_name].id),
+            service=connected_integrations[registry_name].service,
+            url=url,
         )
 
 
 def op(
     name: Optional[Union[str, UserFunction]] = None,
     description: Optional[str] = None,
-    engine: Optional[str] = None,
+    engine: Optional[Union[str, DynamicK8sResource]] = None,
     file_dependencies: Optional[List[str]] = None,
     requirements: Optional[Union[str, List[str]]] = None,
     num_outputs: Optional[int] = None,
     outputs: Optional[List[str]] = None,
     resources: Optional[Dict[str, Any]] = None,
+    image: Optional[Dict[str, str]] = None,
 ) -> Union[DecoratedFunction, OutputArtifactsFunction]:
     """Decorator that converts regular python functions into an operator.
 
     Calling the decorated function returns an Artifact. The decorated function
     can take any number of artifact inputs.
 
     To run the wrapped code locally, without Aqueduct, use the `local` attribute. Eg:
@@ -511,14 +626,20 @@
             "gpu_resource_name" (str):
                 Name of the gpu resource to use (only applicable for Kubernetes engine).
 
                 For example, the following value is valid: "nvidia.com/gpu".
             "cuda_version" (str):
                 Version of CUDA to use with GPU (only applicable for Kubernetes engine). The currently supported
                 values are "11.4.1" and "11.8.0".
+        image:
+            A dictionary containing the custom image configurations that this operator will run with.
+            The dictionary needs to contain the following keys:
+            "registry_name" (str): The name of the registry integration to use.
+            "url" (str): The full URL of the image to use. Example: "123456789012.dkr.ecr.us-east-1.amazonaws.com/my-image:latest"
+            It is recommended to get the dictionary via `client.resource("my_registry_name").image("my-image:latest")`
 
     Examples:
         The op name is inferred from the function name. The description is pulled from the function
         docstring or can be explicitly set in the decorator.
 
         >>> @op
         ... def compute_recommendations(customer_profiles, recent_clicks):
@@ -594,15 +715,22 @@
             )
 
             op_spec = OperatorSpec(
                 function=function_spec,
             )
 
             _update_operator_spec_with_engine(op_spec, engine)
-            _update_operator_spec_with_resources(op_spec, resources)
+            _update_operator_spec_with_resources(
+                op_spec, _check_if_requirements_contain_llm(zip_file), resources
+            )
+
+            if op_spec.resources is not None and op_spec.resources.use_llm:
+                _check_llm_requirements(op_spec)
+
+            _update_operator_spec_with_image(op_spec, image)
 
             assert isinstance(num_outputs, int)
             return wrap_spec(
                 op_spec,
                 *artifacts,
                 op_name=name,
                 output_artifact_names=outputs,
@@ -637,16 +765,17 @@
 
 def metric(
     name: Optional[Union[str, MetricFunction]] = None,
     description: Optional[str] = None,
     file_dependencies: Optional[List[str]] = None,
     requirements: Optional[Union[str, List[str]]] = None,
     output: Optional[str] = None,
-    engine: Optional[str] = None,
+    engine: Optional[Union[str, DynamicK8sResource]] = None,
     resources: Optional[Dict[str, Any]] = None,
+    image: Optional[Dict[str, str]] = None,
 ) -> Union[DecoratedMetricFunction, OutputArtifactFunction]:
     """Decorator that converts regular python functions into a metric.
 
     Calling the decorated function returns a NumericArtifact. The decorated function
     can take any number of artifact inputs.
 
     The requirements.txt file in the current directory is used, if it exists.
@@ -691,14 +820,25 @@
                 a suffix indicating the memory unit must be supplied. Supported memory units are "MB" and "GB",
                 case-insensitive.
 
                 For example, the following values are valid: 100, "100MB", "1GB", "100mb", "1gb".
             "gpu_resource_name" (str):
                 Name of the gpu resource to use (only applicable for Kubernetes engine).
 
+                For example, the following value is valid: "nvidia.com/gpu".
+            "cuda_version" (str):
+                Version of CUDA to use with GPU (only applicable for Kubernetes engine). The currently supported
+                values are "11.4.1" and "11.8.0".
+        image:
+            A dictionary containing the custom image configurations that this operator will run with.
+            The dictionary needs to contain the following keys:
+            "registry_name" (str): The name of the registry integration to use.
+            "url" (str): The full URL of the image to use. Example: "123456789012.dkr.ecr.us-east-1.amazonaws.com/my-image:latest"
+            It is recommended to get the dictionary via `client.resource("my_registry_name").image("my-image:latest")`
+
     Examples:
         The metric name is inferred from the function name. The description is pulled from the function
         docstring or can be explicitly set in the decorator.
 
         >>> @metric()
         ... def avg_churn(churn_table):
         ...     return churn_table['pred_churn'].mean()
@@ -762,15 +902,22 @@
                 granularity=FunctionGranularity.TABLE,
                 file=zip_file,
             )
 
             metric_spec = MetricSpec(function=function_spec)
             op_spec = OperatorSpec(metric=metric_spec)
             _update_operator_spec_with_engine(op_spec, engine)
-            _update_operator_spec_with_resources(op_spec, resources)
+            _update_operator_spec_with_resources(
+                op_spec, _check_if_requirements_contain_llm(zip_file), resources
+            )
+
+            if op_spec.resources is not None and op_spec.resources.use_llm:
+                _check_llm_requirements(op_spec)
+
+            _update_operator_spec_with_image(op_spec, image)
 
             output_names = [output] if output is not None else None
             numeric_artifact = wrap_spec(
                 op_spec,
                 *artifacts,
                 op_name=name,
                 output_artifact_names=output_names,
@@ -818,16 +965,17 @@
 def check(
     name: Optional[Union[str, CheckFunction]] = None,
     description: Optional[str] = None,
     severity: CheckSeverity = CheckSeverity.WARNING,
     file_dependencies: Optional[List[str]] = None,
     requirements: Optional[Union[str, List[str]]] = None,
     output: Optional[str] = None,
-    engine: Optional[str] = None,
+    engine: Optional[Union[str, DynamicK8sResource]] = None,
     resources: Optional[Dict[str, Any]] = None,
+    image: Optional[Dict[str, str]] = None,
 ) -> Union[DecoratedCheckFunction, OutputArtifactFunction]:
     """Decorator that converts a regular python function into a check.
 
     Calling the decorated function returns a BoolArtifact. The decorated python function
     can have any number of artifact inputs.
 
     A check can be set with either WARNING or ERROR severity. A failing check with ERROR severity
@@ -875,14 +1023,25 @@
                 a suffix indicating the memory unit must be supplied. Supported memory units are "MB" and "GB",
                 case-insensitive.
 
                 For example, the following values are valid: 100, "100MB", "1GB", "100mb", "1gb".
             "gpu_resource_name" (str):
                 Name of the gpu resource to use (only applicable for Kubernetes engine).
 
+                For example, the following value is valid: "nvidia.com/gpu".
+            "cuda_version" (str):
+                Version of CUDA to use with GPU (only applicable for Kubernetes engine). The currently supported
+                values are "11.4.1" and "11.8.0".
+        image:
+            A dictionary containing the custom image configurations that this operator will run with.
+            The dictionary needs to contain the following keys:
+            "registry_name" (str): The name of the registry integration to use.
+            "url" (str): The full URL of the image to use. Example: "123456789012.dkr.ecr.us-east-1.amazonaws.com/my-image:latest"
+            It is recommended to get the dictionary via `client.resource("my_registry_name").image("my-image:latest")`
+
     Examples:
         The check name is inferred from the function name. The description is pulled from the function
         docstring or can be explicitly set in the decorator.
 
         >>> @check(
         ... description="The average predicted churn is below 0.1",
         ... severity=CheckSeverity.ERROR,
@@ -945,15 +1104,22 @@
                 type=FunctionType.FILE,
                 granularity=FunctionGranularity.TABLE,
                 file=zip_file,
             )
             check_spec = CheckSpec(level=severity, function=function_spec)
             op_spec = OperatorSpec(check=check_spec)
             _update_operator_spec_with_engine(op_spec, engine)
-            _update_operator_spec_with_resources(op_spec, resources)
+            _update_operator_spec_with_resources(
+                op_spec, _check_if_requirements_contain_llm(zip_file), resources
+            )
+
+            if op_spec.resources is not None and op_spec.resources.use_llm:
+                _check_llm_requirements(op_spec)
+
+            _update_operator_spec_with_image(op_spec, image)
 
             output_names = [output] if output is not None else None
             bool_artifact = wrap_spec(
                 op_spec,
                 *artifacts,
                 op_name=name,
                 output_artifact_names=output_names,
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/error.py` & `aqueduct-sdk-0.3.0/aqueduct/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,7 +131,17 @@
 class ClientValidationError(Error):
     pass
 
 
 # Exception raised when requirements.txt file is missing
 class RequirementsMissingError(Error):
     pass
+
+
+# Exception raised when the user attempts to use an integration that has failed to connected.
+class IntegrationFailedToConnect(Error):
+    pass
+
+
+# Exception raised when the user attempts to use an integration that is still connecting.
+class IntegrationConnectionInProgress(Error):
+    pass
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/flow.py` & `aqueduct-sdk-0.3.0/aqueduct/flow.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import json
 import textwrap
 import uuid
 from collections import defaultdict
 from typing import DefaultDict, Dict, List, Optional, Union
 
-from aqueduct.backend.response_models import (
+from aqueduct.error import InvalidUserArgumentException
+from aqueduct.flow_run import FlowRun
+from aqueduct.models.response_models import (
     GetWorkflowResponse,
     SavedObjectUpdate,
     WorkflowDagResponse,
-    WorkflowDagResultResponse,
 )
-from aqueduct.error import InvalidUserActionException, InvalidUserArgumentException
-from aqueduct.flow_run import FlowRun
-from aqueduct.models.dag import DAG
 from aqueduct.utils.utils import format_header_for_print, generate_ui_url, parse_user_supplied_id
 
 from aqueduct import globals
 
 
 class Flow:
     """This class is a read-only handle to flow already in the system.
@@ -63,35 +61,14 @@
 
         resp = globals.__GLOBAL_API_CLIENT__.get_workflow(self._id)
         return [
             dag_result.to_readable_dict()
             for dag_result in list(reversed(resp.workflow_dag_results))[:limit]
         ]
 
-    def _construct_flow_run(
-        self, dag_result: WorkflowDagResultResponse, dag_resp: WorkflowDagResponse
-    ) -> FlowRun:
-        """Constructs a flow run from a GetWorkflowResponse."""
-        dag = DAG(
-            operators=dag_resp.operators,
-            artifacts=dag_resp.artifacts,
-            operator_by_name={op.name: op for op in dag_resp.operators.values()},
-            metadata=dag_resp.metadata,
-        )
-
-        # The dags for fetched flow runs are missing their serialized functions.
-        return FlowRun(
-            flow_id=self._id,
-            run_id=str(dag_result.id),
-            in_notebook_or_console_context=self._in_notebook_or_console_context,
-            dag=dag,
-            created_at=dag_result.created_at,
-            status=dag_result.status,
-        )
-
     def _get_latest_dag_resp(self) -> WorkflowDagResponse:
         resp = self._get_workflow_resp()
         if not resp.workflow_dag_results:
             assert bool(resp.workflow_dags)
             return list(resp.workflow_dags.values())[0]
 
         latest_result = resp.workflow_dag_results[-1]
@@ -99,35 +76,40 @@
 
     def latest(self) -> Optional[FlowRun]:
         resp = self._get_workflow_resp()
         if not resp.workflow_dag_results:
             return None
 
         latest_result = resp.workflow_dag_results[-1]
-        latest_workflow_dag = resp.workflow_dags[latest_result.workflow_dag_id]
-        return self._construct_flow_run(latest_result, latest_workflow_dag)
+        return FlowRun(
+            flow_id=self._id,
+            run_id=str(latest_result.id),
+            in_notebook_or_console_context=self._in_notebook_or_console_context,
+        )
 
     def fetch(self, run_id: Union[str, uuid.UUID]) -> FlowRun:
         run_id = parse_user_supplied_id(run_id)
 
         resp = self._get_workflow_resp()
-
-        result = None
+        found = False
         for candidate_result in resp.workflow_dag_results:
             if str(candidate_result.id) == run_id:
-                assert result is None, "Cannot have two runs with the same id."
-                result = candidate_result
+                assert not found, "Cannot have two runs with the same id."
+                found = True
 
-        if result is None:
+        if not found:
             raise InvalidUserArgumentException(
                 "Cannot find any run with id %s on this flow." % run_id
             )
 
-        workflow_dag = resp.workflow_dags[result.workflow_dag_id]
-        return self._construct_flow_run(result, workflow_dag)
+        return FlowRun(
+            flow_id=self._id,
+            run_id=str(run_id),
+            in_notebook_or_console_context=self._in_notebook_or_console_context,
+        )
 
     def list_saved_objects(self) -> DefaultDict[str, List[SavedObjectUpdate]]:
         """Get everything saved by the flow.
 
         Returns:
             A dictionary mapping the integration id to the list of table names/storage path.
         """
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/github.py` & `aqueduct-sdk-0.3.0/aqueduct/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             Assuming a github repo structure:
             ```
             /queries
                 hotels.sql
             ```
             Then to use it:
             ```
-            warehouse = aqueduct_client.integration(name="aqueduct_demo")
+            warehouse = aqueduct_client.resource(name="aqueduct_demo")
             gh = aqueduct_client.github(repo=<repo_name>, branch=<branch_name>)
             reviews = warehouse.sql(
                 query=gh.query(path="queries/hotel.sql")
             )
             ```
         """
         repo_config_content_type = GithubRepoConfigContentType.QUERY if query_name else None
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/aws_integration.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/aws.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from aqueduct.integrations.dynamic_k8s_integration import DynamicK8sIntegration
-from aqueduct.models.integration import Integration, IntegrationInfo
+from aqueduct.models.integration import BaseResource, ResourceInfo
+from aqueduct.resources.dynamic_k8s import DynamicK8sResource
 
 
-class AWSIntegration(Integration):
+class AWSResource(BaseResource):
     """
     Class for AWS integration.
     """
 
-    def __init__(self, metadata: IntegrationInfo, k8s_integration_metadata: IntegrationInfo):
+    def __init__(self, metadata: ResourceInfo, k8s_integration_metadata: ResourceInfo):
         self._metadata = metadata
-        self.k8s = DynamicK8sIntegration(k8s_integration_metadata)
+        self.k8s = DynamicK8sResource(k8s_integration_metadata)
 
     def describe(self) -> None:
         """Prints out a human-readable description of the K8s integration."""
-        print("==================== AWS Integration  =============================")
+        print("==================== AWS Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/connect_config.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/connect_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,18 @@
     # Config credentials
     config_file_path: str = ""
     config_file_profile: str = ""
 
     bucket: str
     region: str
 
+    # When connecting a new integration, we allow both leading or trailing slashes here.
+    # The path will be sanitized before being stored in the database.
+    root_dir: str = ""
+
     use_as_storage: str = "false"
 
 
 class GCSConfig(BaseConnectionConfig):
     bucket: str
     service_account_credentials: str
     use_as_storage: str = "false"
@@ -191,14 +195,25 @@
     secret_access_key: str = ""
     region: str = ""
     config_file_path: str = ""
     config_file_profile: str = ""
     k8s: Optional[DynamicK8sConfig]
 
 
+class ECRConfig(BaseConnectionConfig):
+    # Either 1) all of access_key_id, secret_access_key, region, or 2) both config_file_path and
+    # config_file_profile need to be specified. Any other cases will be rejected by the server's
+    # config validation process.
+    access_key_id: str = ""
+    secret_access_key: str = ""
+    region: str = ""
+    config_file_path: str = ""
+    config_file_profile: str = ""
+
+
 class _AWSConfigWithSerializedConfig(BaseConnectionConfig):
     access_key_id: str = ""
     secret_access_key: str = ""
     region: str = ""
     config_file_path: str = ""
     config_file_profile: str = ""
     k8s_serialized: Optional[
@@ -212,60 +227,83 @@
     host: str
     port: int
     targets: List[str]
     level: Optional[NotificationLevel] = None
     enabled: bool
 
 
+class CondaConfig(BaseConnectionConfig):
+    pass
+
+
 class _EmailConfigWithStringField(BaseConnectionConfig):
     user: str
     password: str
     host: str
     port: str
     targets_serialized: str
     level: str
     enabled: str
 
 
+class AirflowConfig(BaseConnectionConfig):
+    host: str
+    username: str
+    password: str
+    s3_credentials_path: str
+    s3_credentials_profile: str
+
+
 class SparkConfig(BaseConnectionConfig):
     livy_server_url: str
 
 
+class DatabricksConfig(BaseConnectionConfig):
+    workspace_url: str
+    access_token: str
+    s3_instance_profile_arn: str
+    instance_pool_id: Optional[str] = None
+
+
 class K8sConfig(BaseConnectionConfig):
     kubeconfig_path: str
     cluster_name: str
     use_same_cluster: str = "false"
     dynamic: str = "false"
     cloud_integration_id: str = ""
 
 
-IntegrationConfig = Union[
+ResourceConfig = Union[
     BigQueryConfig,
     EmailConfig,
     _EmailConfigWithStringField,
     MySQLConfig,
     MongoDBConfig,
     PostgresConfig,
     S3Config,
     AthenaConfig,
     SnowflakeConfig,
     SqlServerConfig,
     SQLiteConfig,
     SlackConfig,
     AWSConfig,
+    ECRConfig,
     _AWSConfigWithSerializedConfig,
     _SlackConfigWithStringField,
+    AirflowConfig,
     SparkConfig,
+    DatabricksConfig,
     K8sConfig,
+    CondaConfig,
 ]
 
 
 def convert_dict_to_integration_connect_config(
     service: Union[str, ServiceType], config_dict: Dict[str, str]
-) -> IntegrationConfig:
+) -> ResourceConfig:
     if service == ServiceType.BIGQUERY:
         return BigQueryConfig(**config_dict)
     elif service in [ServiceType.MARIADB, ServiceType.MYSQL]:
         return MySQLConfig(**config_dict)
     elif service == ServiceType.MONGO_DB:
         return MongoDBConfig(**config_dict)
     elif service == ServiceType.POSTGRES:
@@ -282,27 +320,35 @@
         return SQLiteConfig(**config_dict)
     elif service == ServiceType.REDSHIFT:
         return RedshiftConfig(**config_dict)
     elif service == ServiceType.SLACK:
         return SlackConfig(**config_dict)
     elif service == ServiceType.EMAIL:
         return EmailConfig(**config_dict)
+    elif service == ServiceType.CONDA:
+        return CondaConfig(**config_dict)
+    elif service == ServiceType.AIRFLOW:
+        return AirflowConfig(**config_dict)
     elif service == ServiceType.SPARK:
         return SparkConfig(**config_dict)
+    elif service == ServiceType.DATABRICKS:
+        return DatabricksConfig(**config_dict)
     elif service == ServiceType.AWS:
         return AWSConfig(**config_dict)
     elif service == ServiceType.K8S:
         return K8sConfig(**config_dict)
+    elif service == ServiceType.ECR:
+        return ECRConfig(**config_dict)
     raise InternalAqueductError("Unexpected Service Type: %s" % service)
 
 
 def prepare_integration_config(
-    service: Union[str, ServiceType], config: IntegrationConfig
-) -> IntegrationConfig:
-    """Prepares the IntegrationConfig object to be sent to the backend
+    service: Union[str, ServiceType], config: ResourceConfig
+) -> ResourceConfig:
+    """Prepares the ResourceConfig object to be sent to the backend
     as part of a request to connect a new integration.
     """
     if service == ServiceType.BIGQUERY:
         return _prepare_big_query_config(cast(BigQueryConfig, config))
 
     if service == ServiceType.SLACK:
         return _prepare_slack_config(cast(SlackConfig, config))
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/dynamic_k8s_integration.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/dynamic_k8s.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Dict, Union
 
-from aqueduct.backend.response_models import DynamicEngineStatusResponse
 from aqueduct.constants.enums import K8sClusterActionType, K8sClusterStatusType
 from aqueduct.error import InvalidIntegrationException, InvalidUserArgumentException
-from aqueduct.integrations.connect_config import DynamicK8sConfig
-from aqueduct.models.integration import Integration, IntegrationInfo
-
-from aqueduct import globals
+from aqueduct.models.integration import BaseResource, ResourceInfo
+from aqueduct.models.response_models import DynamicEngineStatusResponse
+from aqueduct.resources.connect_config import DynamicK8sConfig
+from aqueduct.resources.validation import validate_is_connected
 
 
 def parse_dynamic_k8s_config(
     config_delta: Union[Dict[str, Union[int, str]], DynamicK8sConfig]
 ) -> DynamicK8sConfig:
     if not isinstance(config_delta, dict) and not isinstance(config_delta, DynamicK8sConfig):
         raise InvalidUserArgumentException(
@@ -29,32 +28,36 @@
     if len(engine_statuses) == 0:
         raise InvalidIntegrationException("Dynamic engine %s does not exist!" % name)
 
     if len(engine_statuses) > 1:
         raise InvalidIntegrationException("Duplicate dynamic engine with name %s!" % name)
 
 
-class DynamicK8sIntegration(Integration):
+class DynamicK8sResource(BaseResource):
     """
     Class for Dynamic K8s integration.
     """
 
-    def __init__(self, metadata: IntegrationInfo):
+    def __init__(self, metadata: ResourceInfo):
         self._metadata = metadata
 
+    @validate_is_connected()
     def status(self) -> str:
         """Get the current status of the dynamic Kubernetes cluster."""
+        from aqueduct import globals
+
         engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status(
             engine_integration_ids=[str(self._metadata.id)]
         )
 
         validate_engine_record(self._metadata.name, engine_statuses)
 
         return engine_statuses[self._metadata.name].status.value
 
+    @validate_is_connected()
     def create(
         self, config_delta: Union[Dict[str, Union[int, str]], DynamicK8sConfig] = {}
     ) -> None:
         """Creates the dynamic Kubernetes cluster, if it is not currently running.
 
         Args:
             config_delta (optional):
@@ -66,14 +69,16 @@
             InvalidIntegrationException:
                 An error occurred when the dynamic engine doesn't exist.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
         config_delta = parse_dynamic_k8s_config(config_delta)
 
+        from aqueduct import globals
+
         engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status(
             engine_integration_ids=[str(self._metadata.id)]
         )
 
         validate_engine_record(self._metadata.name, engine_statuses)
 
         status = engine_statuses[self._metadata.name].status
@@ -89,14 +94,15 @@
         )
         globals.__GLOBAL_API_CLIENT__.edit_dynamic_engine(
             action=K8sClusterActionType.CREATE,
             integration_id=str(self._metadata.id),
             config_delta=config_delta,
         )
 
+    @validate_is_connected()
     def update(self, config_delta: Union[Dict[str, Union[int, str]], DynamicK8sConfig]) -> None:
         """Update the dynamic Kubernetes cluster. This can only be done when the cluster is in
             Active status.
 
         Args:
             config_delta:
                 This field contains new config values to be used in creating the cluster.
@@ -107,14 +113,16 @@
             InvalidIntegrationException:
                 An error occurred when the dynamic engine doesn't exist.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
         config_delta = parse_dynamic_k8s_config(config_delta)
 
+        from aqueduct import globals
+
         engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status(
             engine_integration_ids=[str(self._metadata.id)]
         )
 
         validate_engine_record(self._metadata.name, engine_statuses)
 
         status = engine_statuses[self._metadata.name].status
@@ -131,14 +139,15 @@
         )
         globals.__GLOBAL_API_CLIENT__.edit_dynamic_engine(
             action=K8sClusterActionType.UPDATE,
             integration_id=str(self._metadata.id),
             config_delta=config_delta,
         )
 
+    @validate_is_connected()
     def delete(self, force: bool = False) -> None:
         """Deletes the dynamic Kubernetes cluster if it is running, ignoring the keepalive period.
 
         Args:
             force:
                 By default, if there are any pods in the "Running" or "ContainerCreating" status,
                 the deletion process will fail. However, if the flag is set to "True", this check
@@ -146,14 +155,16 @@
 
         Raises:
             InvalidIntegrationException:
                 An error occurred when the dynamic engine doesn't exist.
             InternalServerError:
                 An unexpected error occurred within the Aqueduct cluster.
         """
+        from aqueduct import globals
+
         engine_statuses = globals.__GLOBAL_API_CLIENT__.get_dynamic_engine_status(
             engine_integration_ids=[str(self._metadata.id)]
         )
 
         validate_engine_record(self._metadata.name, engine_statuses)
 
         status = engine_statuses[self._metadata.name].status
@@ -172,9 +183,9 @@
 
         globals.__GLOBAL_API_CLIENT__.edit_dynamic_engine(
             action=action, integration_id=str(self._metadata.id)
         )
 
     def describe(self) -> None:
         """Prints out a human-readable description of the K8s integration."""
-        print("==================== Dynamic K8s Integration  =============================")
+        print("==================== Dynamic K8s Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/google_sheets_integration.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/google_sheets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from typing import Optional
 
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.table_artifact import TableArtifact
 from aqueduct.constants.enums import ArtifactType, GoogleSheetsSaveMode
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import Integration, IntegrationInfo
+from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     GoogleSheetsExtractParams,
     GoogleSheetsLoadParams,
     Operator,
     OperatorSpec,
 )
+from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.utils import generate_uuid
 
 from ..utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
 from .save import _save_artifact
 
 
-class GoogleSheetsIntegration(Integration):
+class GoogleSheetsResource(BaseResource):
     """
     Class for Google Sheets integration.
     """
 
-    def __init__(self, dag: DAG, metadata: IntegrationInfo):
+    def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
+    @validate_is_connected()
     def spreadsheet(
         self,
         spreadsheet_id: str,
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
     ) -> TableArtifact:
@@ -92,14 +94,15 @@
         )
 
         return TableArtifact(
             dag=self._dag,
             artifact_id=output_artifact_id,
         )
 
+    @validate_is_connected()
     def save(
         self,
         artifact: BaseArtifact,
         filepath: str,
         save_mode: GoogleSheetsSaveMode = GoogleSheetsSaveMode.OVERWRITE,
     ) -> None:
         """Registers a save operator of the given artifact, to be executed when it's computed in a published flow.
@@ -122,9 +125,9 @@
             self._dag,
             self._metadata,
             save_params=GoogleSheetsLoadParams(filepath=filepath, save_mode=save_mode),
         )
 
     def describe(self) -> None:
         """Prints out a human-readable description of the google sheets integration."""
-        print("==================== Google Sheets Integration  =============================")
+        print("==================== Google Sheets Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/mongodb_integration.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/mongodb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import json
 from typing import Any, Dict, List, Optional
 
 from aqueduct.artifacts import preview as artifact_utils
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.table_artifact import TableArtifact
 from aqueduct.constants.enums import ArtifactType, ExecutionMode, LoadUpdateMode
-from aqueduct.integrations.parameters import _validate_parameters
-from aqueduct.integrations.save import _save_artifact
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import Integration, IntegrationInfo
+from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     MongoExtractParams,
     Operator,
     OperatorSpec,
     RelationalDBLoadParams,
 )
+from aqueduct.resources.parameters import _validate_parameters
+from aqueduct.resources.save import _save_artifact
+from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
 from aqueduct.utils.utils import generate_uuid
 
 from aqueduct import globals
 
 
-class MongoDBCollectionIntegration(Integration):
+class MongoDBCollectionIntegration(BaseResource):
     _collection_name: str
     _dag: DAG
 
-    def __init__(self, dag: DAG, metadata: IntegrationInfo, collection_name: str) -> None:
+    def __init__(self, dag: DAG, metadata: ResourceInfo, collection_name: str) -> None:
         self._metadata = metadata
         self._dag = dag
         self._collection_name = collection_name
 
+    @validate_is_connected()
     def find(
         self,
         *args: List[Any],
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
         parameters: Optional[List[BaseArtifact]] = None,
@@ -152,14 +154,15 @@
             artifact = artifact_utils.preview_artifact(self._dag, output_artf_id)
             assert isinstance(artifact, TableArtifact)
             return artifact
         else:
             # We are in lazy mode.
             return TableArtifact(self._dag, output_artf_id)
 
+    @validate_is_connected()
     def save(self, artifact: BaseArtifact, update_mode: LoadUpdateMode) -> None:
         """Registers a save operator of the given artifact, to be executed when it's computed in a published flow.
 
         Args:
             artifact:
                 The artifact to save into this collection.
             update_mode:
@@ -172,41 +175,43 @@
             self._metadata,
             save_params=RelationalDBLoadParams(
                 table=self._collection_name, update_mode=update_mode
             ),
         )
 
 
-class MongoDBIntegration(Integration):
+class MongoDBResource(BaseResource):
     """
     Class for MongoDB integration. This works similar to mongo's `Database` object:
 
-    mongo_integration = client.integration("my_integration_name")
+    mongo_integration = client.resource("my_resource_name")
     my_table_artifact = mongo_integration.collection("my_collection").find({})
     """
 
-    def __init__(self, dag: DAG, metadata: IntegrationInfo):
+    def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
+    @validate_is_connected()
     def collection(self, name: str) -> MongoDBCollectionIntegration:
         """Returns a specific collection object to call `.find()` method.
 
         Example:
 
-        mongo_integration = client.integration("my_integration_name")
-        my_table_artifact = mongo_integration.collection("my_collection").find({})
+        mongo_resource = client.resource("my_resource_name")
+        my_table_artifact = mongo_resource.collection("my_collection").find({})
         """
         return MongoDBCollectionIntegration(self._dag, self._metadata, name)
 
     def describe(self) -> None:
         """Prints out a human-readable description of the MongoDB integration."""
-        print("==================== MongoDB Integration  =============================")
+        print("==================== MongoDB Resource =============================")
         self._metadata.describe()
 
+    @validate_is_connected()
     def save(self, artifact: BaseArtifact, collection: str, update_mode: LoadUpdateMode) -> None:
         """Registers a save operator of the given artifact, to be executed when it's computed in a published flow.
 
         Args:
             artifact:
                 The artifact to save into the given collection.
             collection:
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/parameters.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/parameters.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/s3_integration.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from typing import List, Optional, Union
 
 from aqueduct.artifacts import preview as artifact_utils
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.constants.enums import ArtifactType, ExecutionMode, S3TableFormat
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import Integration, IntegrationInfo
+from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     Operator,
     OperatorSpec,
     S3ExtractParams,
     S3LoadParams,
 )
+from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.utils import generate_uuid
 
 from aqueduct import globals
 
 from ..artifacts.create import to_artifact_class
 from ..error import InvalidUserArgumentException
@@ -38,23 +39,24 @@
     elif lowercased_format == S3TableFormat.PARQUET.value.lower():
         format_enum = S3TableFormat.PARQUET
     else:
         raise InvalidUserArgumentException("Unsupported S3 file format `%s`." % format)
     return format_enum
 
 
-class S3Integration(Integration):
+class S3Resource(BaseResource):
     """
     Class for S3 integration.
     """
 
-    def __init__(self, dag: DAG, metadata: IntegrationInfo):
+    def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
+    @validate_is_connected()
     def file(
         self,
         filepaths: Union[List[str], str],
         artifact_type: ArtifactType,
         format: Optional[str] = None,
         merge: Optional[bool] = None,
         name: Optional[str] = None,
@@ -167,14 +169,15 @@
         if execution_mode == ExecutionMode.EAGER:
             # Issue preview request since this is an eager execution.
             return artifact_utils.preview_artifact(self._dag, output_artifact_id)
         else:
             # We are in lazy mode.
             return to_artifact_class(self._dag, output_artifact_id, artifact_type)
 
+    @validate_is_connected()
     def save(self, artifact: BaseArtifact, filepath: str, format: Optional[str] = None) -> None:
         """Registers a save operator of the given artifact, to be executed when it's computed in a published flow.
 
         Args:
             artifact:
                 The artifact to save into S3.
             filepath:
@@ -202,9 +205,9 @@
             self._dag,
             self._metadata,
             save_params=S3LoadParams(filepath=filepath, format=_convert_to_s3_table_format(format)),
         )
 
     def describe(self) -> None:
         """Prints out a human-readable description of the S3 integration."""
-        print("==================== S3 Integration  =============================")
+        print("==================== S3 Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/salesforce_integration.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/salesforce.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 from typing import Optional
 
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.table_artifact import TableArtifact
 from aqueduct.constants.enums import ArtifactType, SalesforceExtractType
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import Integration, IntegrationInfo
+from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     Operator,
     OperatorSpec,
     SalesforceExtractParams,
     SalesforceLoadParams,
 )
+from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.utils import generate_uuid
 
 from ..utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
 from .save import _save_artifact
 
 
-class SalesforceIntegration(Integration):
+class SalesforceResource(BaseResource):
     """
     Class for Salesforce integration.
     """
 
-    def __init__(self, dag: DAG, metadata: IntegrationInfo):
+    def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
+    @validate_is_connected()
     def search(
         self,
         search_query: str,
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
     ) -> TableArtifact:
@@ -65,14 +67,15 @@
         )
 
         return TableArtifact(
             dag=self._dag,
             artifact_id=output_artifact_id,
         )
 
+    @validate_is_connected()
     def query(
         self,
         query: str,
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
     ) -> TableArtifact:
@@ -98,14 +101,15 @@
         )
 
         return TableArtifact(
             dag=self._dag,
             artifact_id=output_artifact_id,
         )
 
+    @validate_is_connected()
     def save(self, artifact: BaseArtifact, object: str) -> None:
         """Registers a save operator of the given artifact, to be executed when it's computed in a published flow.
 
         Args:
             artifact:
                 The artifact to save into Salesforce.
             object:
@@ -160,9 +164,9 @@
             ],
         )
 
         return output_artifact_id
 
     def describe(self) -> None:
         """Prints out a human-readable description of the Salesforce integration."""
-        print("==================== Salesforce Integration  =============================")
+        print("==================== Salesforce Resource =============================")
         self._metadata.describe()
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/save.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/save.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import uuid
 from typing import List
 
 from aqueduct.constants.enums import OperatorType
 from aqueduct.error import InvalidIntegrationException
 from aqueduct.globals import __GLOBAL_API_CLIENT__ as global_api_client
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import IntegrationInfo
+from aqueduct.models.integration import ResourceInfo
 from aqueduct.models.operators import LoadSpec, Operator, OperatorSpec, UnionLoadParams
 from aqueduct.utils.dag_deltas import (
     AddOperatorDelta,
     DAGDelta,
     RemoveOperatorDelta,
     apply_deltas_to_dag,
 )
 from aqueduct.utils.utils import generate_uuid
 
 
 def _save_artifact(
     artifact_id: uuid.UUID,
     dag: DAG,
-    integration_info: IntegrationInfo,
+    integration_info: ResourceInfo,
     save_params: UnionLoadParams,
 ) -> None:
     """Configures the given artifact to be written to a specific integration after it's computed in a published flow.
 
     Args:
         artifact_id:
             The artifact who's contents will be saved.
@@ -40,15 +40,15 @@
             found.
         InvalidUserActionException:
             An error occurred because you are trying to load non-relational data into a relational integration.
         InvalidUserArgumentException:
             An error occurred because some necessary fields are missing in the SaveParams.
     """
 
-    integrations_map = global_api_client.list_integrations()
+    integrations_map = global_api_client.list_resources()
     if integration_info.name not in integrations_map:
         raise InvalidIntegrationException(
             "Not connected to integration %s!" % integration_info.name
         )
 
     # We currently do not allow multiple save operators on the same artifact to the same integration.
     # We do allow multiple artifacts to write to the same integration, as well as a single artifact
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/integrations/sql_integration.py` & `aqueduct-sdk-0.3.0/aqueduct/resources/sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,61 +2,64 @@
 
 import pandas as pd
 from aqueduct.artifacts.base_artifact import BaseArtifact
 from aqueduct.artifacts.preview import preview_artifact
 from aqueduct.artifacts.table_artifact import TableArtifact
 from aqueduct.constants.enums import ArtifactType, ExecutionMode, LoadUpdateMode, ServiceType
 from aqueduct.error import InvalidUserActionException, InvalidUserArgumentException
-from aqueduct.integrations.parameters import _validate_builtin_expansions, _validate_parameters
-from aqueduct.integrations.save import _save_artifact
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG
-from aqueduct.models.integration import Integration, IntegrationInfo
+from aqueduct.models.integration import BaseResource, ResourceInfo
 from aqueduct.models.operators import (
     ExtractSpec,
     Operator,
     OperatorSpec,
     RelationalDBExtractParams,
     RelationalDBLoadParams,
 )
+from aqueduct.resources.parameters import _validate_builtin_expansions, _validate_parameters
+from aqueduct.resources.save import _save_artifact
+from aqueduct.resources.validation import validate_is_connected
 from aqueduct.utils.dag_deltas import AddOperatorDelta, apply_deltas_to_dag
 from aqueduct.utils.naming import default_artifact_name_from_op_name, sanitize_artifact_name
 from aqueduct.utils.utils import generate_uuid
 
 from aqueduct import globals
 
 LIST_TABLES_QUERY_PG = "SELECT tablename, tableowner FROM pg_catalog.pg_tables WHERE schemaname != 'pg_catalog' AND schemaname != 'information_schema';"
 LIST_TABLES_QUERY_SNOWFLAKE = "SELECT table_name AS \"tablename\", table_owner AS \"tableowner\" FROM information_schema.tables WHERE table_schema != 'INFORMATION_SCHEMA' AND table_type = 'BASE TABLE';"
-LIST_TABLES_QUERY_MYSQL = "SELECT table_name FROM INFORMATION_SCHEMA.TABLES WHERE table_type = 'BASE TABLE' AND table_schema NOT IN ('mysql', 'sys', 'performance_schema');"
+LIST_TABLES_QUERY_MYSQL = "SELECT table_name AS tablename FROM INFORMATION_SCHEMA.TABLES WHERE table_type = 'BASE TABLE' AND table_schema NOT IN ('mysql', 'sys', 'performance_schema');"
 LIST_TABLES_QUERY_MARIADB = "SELECT table_name AS \"tablename\" FROM INFORMATION_SCHEMA.TABLES WHERE table_type = 'BASE TABLE' AND table_schema NOT IN ('mysql', 'sys', 'performance_schema');"
 
 LIST_TABLES_QUERY_SQLSERVER = (
     "SELECT table_name FROM INFORMATION_SCHEMA.TABLES WHERE table_type = 'BASE TABLE';"
 )
 GET_TABLE_QUERY = "select * from %s"
 LIST_TABLES_QUERY_SQLITE = "SELECT name AS tablename FROM sqlite_master WHERE type='table';"
 LIST_TABLES_QUERY_ATHENA = "AQUEDUCT_ATHENA_LIST_TABLE"
 
 
-class RelationalDBIntegration(Integration):
+class RelationalDBResource(BaseResource):
     """
     Class for Relational integrations.
     """
 
-    def __init__(self, dag: DAG, metadata: IntegrationInfo):
+    def __init__(self, dag: DAG, metadata: ResourceInfo):
         self._dag = dag
         self._metadata = metadata
 
+    @validate_is_connected()
     def list_tables(self) -> pd.DataFrame:
         """
         Lists the tables available in the RelationalDB integration.
 
         Returns:
             pd.DataFrame of available tables.
         """
+
         if self.type() in [ServiceType.BIGQUERY, ServiceType.SNOWFLAKE]:
             # Use the list integration objects endpoint instead of
             # providing a hardcoded SQL query to execute
             tables = globals.__GLOBAL_API_CLIENT__.list_tables(str(self.id()))
             return pd.DataFrame(tables, columns=["tablename"])
 
         if self.type() in [
@@ -75,28 +78,30 @@
             list_tables_query = LIST_TABLES_QUERY_SQLITE
         elif self.type() == ServiceType.ATHENA:
             list_tables_query = LIST_TABLES_QUERY_ATHENA
 
         sql_artifact = self.sql(query=list_tables_query)
         return sql_artifact.get()
 
+    @validate_is_connected()
     def table(self, name: str) -> pd.DataFrame:
         """
-        Retrieves a table from a RealtionalDB integration.
+        Retrieves a table from a RelationalDB integration.
 
         Args:
             name:
                 The name of the table to retrieve.
 
         Returns:
             pd.DataFrame of the table to retrieve.
         """
         sql_artifact = self.sql(query=GET_TABLE_QUERY % name)
         return sql_artifact.get()
 
+    @validate_is_connected()
     def sql(
         self,
         query: Union[str, List[str], RelationalDBExtractParams],
         name: Optional[str] = None,
         output: Optional[str] = None,
         description: str = "",
         parameters: Optional[List[BaseArtifact]] = None,
@@ -228,14 +233,15 @@
             artifact = preview_artifact(self._dag, sql_output_artifact_id)
             assert isinstance(artifact, TableArtifact)
             return artifact
         else:
             # We are in lazy mode.
             return TableArtifact(self._dag, sql_output_artifact_id)
 
+    @validate_is_connected()
     def save(self, artifact: BaseArtifact, table_name: str, update_mode: LoadUpdateMode) -> None:
         """Registers a save operator of the given artifact, to be executed when it's computed in a published flow.
 
         Args:
             artifact:
                 The artifact to save into this sql integration.
             table_name:
@@ -261,13 +267,18 @@
             save_params=RelationalDBLoadParams(table=table_name, update_mode=update_mode),
         )
 
     def describe(self) -> None:
         """
         Prints out a human-readable description of the SQL integration.
         """
-        print("==================== SQL Integration =============================")
-        print("Integration Information:")
+        print("==================== SQL Resource =============================")
+        print("Resource Information:")
         self._metadata.describe()
-        print("Integration Table List Preview:")
-        print(self.list_tables()["name"].head().to_string())
-        print("(only first 5 tables are shown)")
+
+        # Only list the tables if the integration is connected.
+        try:
+            print("Resource Table List Preview:")
+            print(self.list_tables()["name"].head().to_string())
+            print("(only first 5 tables are shown)")
+        except:
+            pass
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/models/dag.py` & `aqueduct-sdk-0.3.0/aqueduct/models/dag.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/models/dag_rules.py` & `aqueduct-sdk-0.3.0/aqueduct/models/dag_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,22 @@
     engine_config: EngineConfig,
     op_name: str,
 ) -> None:
     allowed_customizable_resources: Dict[str, bool] = {
         CustomizableResourceType.NUM_CPUS: False,
         CustomizableResourceType.MEMORY: False,
         CustomizableResourceType.GPU_RESOURCE_NAME: False,
+        CustomizableResourceType.CUDA_VERSION: False,
     }
     if engine_config.type == RuntimeType.K8S:
         allowed_customizable_resources = {
             CustomizableResourceType.NUM_CPUS: True,
             CustomizableResourceType.MEMORY: True,
             CustomizableResourceType.GPU_RESOURCE_NAME: True,
+            CustomizableResourceType.CUDA_VERSION: True,
         }
     elif engine_config.type == RuntimeType.LAMBDA:
         allowed_customizable_resources[CustomizableResourceType.MEMORY] = True
 
     if not allowed_customizable_resources[CustomizableResourceType.NUM_CPUS] and resources.num_cpus:
         raise InvalidUserArgumentException(
             "Operator `%s` cannot configure the number of cpus, since it is not supported when running on %s."
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/models/operators.py` & `aqueduct-sdk-0.3.0/aqueduct/models/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     S3TableFormat,
     SalesforceExtractType,
     SerializationType,
     ServiceType,
 )
 from aqueduct.error import AqueductError, UnsupportedFeatureException
 from aqueduct.models.config import EngineConfig
-from aqueduct.models.integration import IntegrationInfo
+from aqueduct.models.integration import ResourceInfo
 from pydantic import BaseModel, Extra
 
 
 class GithubMetadata(BaseModel):
     """
     Specifies a destination in github integration.
     There are two ways to specify the content:
@@ -197,25 +197,34 @@
 class ResourceConfig(BaseModel):
     # These resources are configured exactly. The user is not given any more
     # or any less. If the requested resources exceeds capacity, an error
     # will be thrown at execution time.
     num_cpus: Optional[int]
     memory_mb: Optional[int]
     gpu_resource_name: Optional[str]
+    cuda_version: Optional[str]
+    use_llm: Optional[bool]
+
+
+class ImageConfig(BaseModel):
+    registry_id: str
+    service: ServiceType
+    url: str
 
 
 class OperatorSpec(BaseModel):
     extract: Optional[ExtractSpec]
     load: Optional[LoadSpec]
     function: Optional[FunctionSpec]
     metric: Optional[MetricSpec]
     check: Optional[CheckSpec]
     param: Optional[ParamSpec]
     system_metric: Optional[SystemMetricSpec]
     resources: Optional[ResourceConfig]
+    image: Optional[ImageConfig]
 
     # If set, overwrites any default engine on the DAG.
     engine_config: Optional[EngineConfig]
 
 
 class Operator(BaseModel):
     id: uuid.UUID
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/tests/dag_delta_test.py` & `aqueduct-sdk-0.3.0/aqueduct/tests/dag_delta_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/tests/dag_test.py` & `aqueduct-sdk-0.3.0/aqueduct/tests/dag_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/tests/decorator_test.py` & `aqueduct-sdk-0.3.0/aqueduct/tests/decorator_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/tests/decorators_with_without_parentheses_test.py` & `aqueduct-sdk-0.3.0/aqueduct/tests/decorators_with_without_parentheses_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/tests/flow_test.py` & `aqueduct-sdk-0.3.0/aqueduct/tests/flow_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/tests/helpers_test.py` & `aqueduct-sdk-0.3.0/aqueduct/tests/helpers_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,20 @@
             assert err_msg in str(e)
         except Exception:
             assert False, "Wrong exception type was raised."
 
     _run_test("150MB", 150)
     _run_test("150Mb", 150)
     _run_test("150mb", 150)
-    _run_test("150GB", 150 * 1000)
-    _run_test("150Gb", 150 * 1000)
-    _run_test("150gb", 150 * 1000)
-    _run_test("150GB       ", 150 * 1000)
-    _run_test("150   GB       ", 150 * 1000)
-    _run_test("   150 GB  ", 150 * 1000)
+    _run_test("150GB", 150 * 1024)
+    _run_test("150Gb", 150 * 1024)
+    _run_test("150gb", 150 * 1024)
+    _run_test("150GB       ", 150 * 1024)
+    _run_test("150   GB       ", 150 * 1024)
+    _run_test("   150 GB  ", 150 * 1024)
 
     _run_test("1", -1, "not long enough")
     _run_test("150", -1, "must have a suffix that is one of")
     _run_test("150de", -1, "must have a suffix that is one of")
     _run_test("-150 MB", -1, "must be a positive integer")
     _run_test("abcMB", -1, "must be a positive integer")
     _run_test("abc150MB", -1, "must be a positive integer")
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/tests/metric_test.py` & `aqueduct-sdk-0.3.0/aqueduct/tests/metric_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/tests/serialization_test.py` & `aqueduct-sdk-0.3.0/aqueduct/tests/serialization_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import uuid
 
 import cloudpickle as pickle
-from aqueduct.backend.response_models import ArtifactResult, ExecutionState, Logs, PreviewResponse
 from aqueduct.constants.enums import (
     ArtifactType,
     ExecutionStatus,
     FunctionGranularity,
     FunctionType,
     GoogleSheetsSaveMode,
     LoadUpdateMode,
@@ -14,14 +13,15 @@
     S3TableFormat,
     SalesforceExtractType,
     SerializationType,
     ServiceType,
 )
 from aqueduct.models.artifact import ArtifactMetadata
 from aqueduct.models.dag import DAG, Metadata
+from aqueduct.models.execution_state import ExecutionState, Logs
 from aqueduct.models.operators import (
     ExtractSpec,
     FunctionSpec,
     GoogleSheetsExtractParams,
     GoogleSheetsLoadParams,
     LoadSpec,
     Operator,
@@ -29,14 +29,15 @@
     RelationalDBExtractParams,
     RelationalDBLoadParams,
     S3ExtractParams,
     S3LoadParams,
     SalesforceExtractParams,
     SalesforceLoadParams,
 )
+from aqueduct.models.response_models import ArtifactResult, PreviewResponse
 from aqueduct.tests.utils import _construct_dag, _construct_operator
 from aqueduct.utils.serialization import (
     PickleableCollectionSerializationFormat,
     _read_image_content,
     _read_pickle_content,
     _read_string_content,
     artifact_type_to_serialization_type,
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/tests/utils.py` & `aqueduct-sdk-0.3.0/aqueduct/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import uuid
 from typing import List, Optional
 
 import pandas as pd
 from aqueduct.artifacts.table_artifact import TableArtifact
-from aqueduct.backend.response_models import ArtifactResult, PreviewResponse
 from aqueduct.constants.enums import (
     ArtifactType,
     CheckSeverity,
     ExecutionStatus,
     FunctionGranularity,
     FunctionType,
     LoadUpdateMode,
@@ -25,14 +24,15 @@
     LoadSpec,
     MetricSpec,
     Operator,
     OperatorSpec,
     RelationalDBExtractParams,
     RelationalDBLoadParams,
 )
+from aqueduct.models.response_models import ArtifactResult, PreviewResponse
 from aqueduct.utils.utils import generate_uuid
 
 from aqueduct import globals
 
 
 def generate_uuids(num: int) -> List[uuid.UUID]:
     return [generate_uuid() for _ in range(num)]
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/utils/dag_deltas.py` & `aqueduct-sdk-0.3.0/aqueduct/utils/dag_deltas.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/utils/describe.py` & `aqueduct-sdk-0.3.0/aqueduct/utils/describe.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/utils/function_packaging.py` & `aqueduct-sdk-0.3.0/aqueduct/utils/function_packaging.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/utils/local_data.py` & `aqueduct-sdk-0.3.0/aqueduct/utils/local_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,20 +32,15 @@
     file_format = format
 
     if artifact_type is None:
         raise InvalidUserArgumentException(
             "Specify artifact type in `as_type` field in `create_param` to use local data. "
         )
 
-    if (artifact_type is not ArtifactType.TABLE) and (artifact_type is not ArtifactType.IMAGE):
-        raise InvalidUserArgumentException(
-            "We currently only support using Image and Table Artifacts from local data."
-        )
-
-    if not os.path.isfile(file_path):
+    if not os.path.exists(file_path):
         raise InvalidUserArgumentException(
             "Given path file '%s' to local data does not exist." % file_path
         )
 
     if artifact_type == ArtifactType.TABLE and file_format is None:
         raise InvalidUserArgumentException(
             "Specify format in order to use local data as TableArtifact."
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/utils/naming.py` & `aqueduct-sdk-0.3.0/aqueduct/utils/naming.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/utils/serialization.py` & `aqueduct-sdk-0.3.0/aqueduct/utils/serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,30 +71,56 @@
     return content.decode(DEFAULT_ENCODING)
 
 
 def _read_bytes_content(content: bytes) -> bytes:
     return content
 
 
-def _read_local_csv_table_content(path: str) -> Any:
+def _read_local_csv_table_content(path: str) -> pd.DataFrame:
     return pd.read_csv(path)
 
 
-def _read_local_json_table_content(path: str) -> Any:
+def _read_local_json_table_content(path: str) -> pd.DataFrame:
     return pd.read_json(path, orient="table")
 
 
-def _read_local_parquet_table_content(path: str) -> Any:
+def _read_local_parquet_table_content(path: str) -> pd.DataFrame:
     return pd.read_parquet(path)
 
 
-def _read_local_image_content(path: str) -> Any:
+def _read_local_image_content(path: str) -> Image.Image:
     return Image.open(path)
 
 
+def _read_local_json_content(path: str) -> Any:
+    with open(path, mode="rb", encoding=DEFAULT_ENCODING) as file:
+        return json.load(file)
+
+
+def _read_local_pickle_content(path: str) -> Any:
+    with open(path, mode="rb") as file:
+        return pickle.load(file)
+
+
+def _read_local_string_content(path: str) -> str:
+    with open(path, mode="r", encoding=DEFAULT_ENCODING) as file:
+        return file.read()
+
+
+def _read_local_bytes_content(path: str) -> bytes:
+    with open(path, mode="rb") as file:
+        return file.read()
+
+
+def _read_local_tf_keras_model(path: str) -> Any:
+    from tensorflow import keras
+
+    return keras.models.load_model(path)
+
+
 # Returns a tf.keras.Model type. We don't assume that every user has it installed,
 # so we return "Any" type.
 def _read_tf_keras_model(content: bytes) -> Any:
     temp_model_dir = None
     try:
         temp_model_dir = _make_temp_dir()
         model_file_path = os.path.join(temp_model_dir, _TEMP_KERAS_MODEL_NAME)
@@ -123,14 +149,19 @@
 
 # Not intended for use outside of `deserialize()`.
 __local_data_deserialization_function_mapping: Dict[str, Callable[[str], Any]] = {
     LocalDataSerializationType.CSV_TABLE: _read_local_csv_table_content,
     LocalDataSerializationType.JSON_TABLE: _read_local_json_table_content,
     LocalDataSerializationType.PARQUET_TABLE: _read_local_parquet_table_content,
     LocalDataSerializationType.IMAGE: _read_local_image_content,
+    LocalDataSerializationType.JSON: _read_local_json_content,
+    LocalDataSerializationType.BYTES: _read_local_bytes_content,
+    LocalDataSerializationType.PICKLE: _read_local_pickle_content,
+    LocalDataSerializationType.STRING: _read_local_string_content,
+    LocalDataSerializationType.TF_KERAS: _read_local_tf_keras_model,
 }
 
 
 def check_and_fetch_pickled_collection_format(
     serialization_type: Union[SerializationType, S3SerializationType],
     deserialized_val: Any,
 ) -> Optional[PickleableCollectionSerializationFormat]:
@@ -358,27 +389,44 @@
 ) -> Any:
     """Extract value of specified type in Local Data."""
     artifact_type = as_type
     local_data_path = path
     local_data_format = _convert_to_local_data_table_format(format)
     if artifact_type == ArtifactType.TABLE:
         if local_data_format == LocalDataTableFormat.CSV:
-            deserialized_val = deserialize_from_local_data(
-                LocalDataSerializationType.CSV_TABLE, artifact_type, local_data_path
-            )
+            local_data_serialization_format = LocalDataSerializationType.CSV_TABLE
         elif local_data_format == LocalDataTableFormat.JSON:
-            deserialized_val = deserialize_from_local_data(
-                LocalDataSerializationType.JSON_TABLE, artifact_type, local_data_path
-            )
+            local_data_serialization_format = LocalDataSerializationType.JSON_TABLE
         elif local_data_format == LocalDataTableFormat.PARQUET:
-            deserialized_val = deserialize_from_local_data(
-                LocalDataSerializationType.PARQUET_TABLE, artifact_type, local_data_path
-            )
+            local_data_serialization_format = LocalDataSerializationType.PARQUET_TABLE
         else:
             raise Exception("Unsupported file format %s" % format)
     elif artifact_type == ArtifactType.IMAGE:
-        deserialized_val = deserialize_from_local_data(
-            LocalDataSerializationType.IMAGE, artifact_type, local_data_path
-        )
+        local_data_serialization_format = LocalDataSerializationType.IMAGE
+    elif artifact_type == ArtifactType.JSON or artifact_type == ArtifactType.STRING:
+        local_data_serialization_format = LocalDataSerializationType.STRING
+    elif artifact_type == ArtifactType.BYTES:
+        local_data_serialization_format = LocalDataSerializationType.BYTES
+    elif artifact_type == ArtifactType.BOOL or artifact_type == ArtifactType.NUMERIC:
+        local_data_serialization_format = LocalDataSerializationType.JSON
+    elif artifact_type == ArtifactType.PICKLABLE:
+        local_data_serialization_format = LocalDataSerializationType.PICKLE
+    elif (
+        artifact_type == ArtifactType.DICT
+        or artifact_type == ArtifactType.TUPLE
+        or artifact_type == ArtifactType.LIST
+    ):
+        try:
+            with open(local_data_path, mode="rb") as file:
+                json.dumps(file.read())
+            local_data_serialization_format = LocalDataSerializationType.JSON
+        except:
+            local_data_serialization_format = LocalDataSerializationType.PICKLE
+    elif artifact_type == ArtifactType.TF_KERAS:
+        local_data_serialization_format = LocalDataSerializationType.TF_KERAS
     else:
         raise Exception("Unsupported artifact type %s" % artifact_type)
+
+    deserialized_val = deserialize_from_local_data(
+        local_data_serialization_format, artifact_type, local_data_path
+    )
     return deserialized_val
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct/utils/type_inference.py` & `aqueduct-sdk-0.3.0/aqueduct/utils/type_inference.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.9/aqueduct/utils/utils.py` & `aqueduct-sdk-0.3.0/aqueduct/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import uuid
-from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from aqueduct.constants.enums import ArtifactType, RuntimeType, ServiceType, TriggerType
 from aqueduct.error import *
 from aqueduct.models.config import (
     AirflowEngineConfig,
     DatabricksEngineConfig,
     EngineConfig,
     K8sEngineConfig,
     LambdaEngineConfig,
     SparkEngineConfig,
 )
 from aqueduct.models.dag import Schedule
-from aqueduct.models.integration import IntegrationInfo
+from aqueduct.models.integration import ResourceInfo
 from aqueduct.models.operators import ParamSpec
+from aqueduct.resources.dynamic_k8s import DynamicK8sResource
+from aqueduct.utils.integration_validation import validate_integration_is_connected
 from croniter import croniter
 
+from ..models.execution_state import Logs
 from .serialization import artifact_type_to_serialization_type, serialize_val
 from .type_inference import _bytes_to_base64_string
 
 
 def format_header_for_print(header: str) -> str:
     """Used to print the header of a section in "describe()" with a consistent length.
 
@@ -80,24 +82,42 @@
 
     if not croniter.is_valid(schedule_str):
         raise InvalidCronStringException("%s is not a valid cron string!" % schedule_str)
 
     return Schedule(trigger=TriggerType.PERIODIC, cron_schedule=schedule_str)
 
 
-def human_readable_timestamp(ts: int) -> str:
-    format = "%Y-%m-%d %H:%M:%S"
-    return datetime.utcfromtimestamp(ts).strftime(format)
-
-
 def indent_multiline_string(content: str) -> str:
     """Indents every line of a multiline string block."""
     return "\t" + "\t".join(content.splitlines(True))
 
 
+def print_logs(logs: Logs) -> None:
+    """Prints out the logs with the following format:
+
+    stdout:
+        {logs}
+        {logs}
+    ----------------------------------
+    stderr:
+        {logs}
+        {logs}
+    """
+    if len(logs.stdout) > 0:
+        print("stdout:")
+        print(indent_multiline_string(logs.stdout).rstrip("\n"))
+
+    if len(logs.stdout) > 0 and len(logs.stderr) > 0:
+        print("----------------------------------")
+
+    if len(logs.stderr) > 0:
+        print("stderr:")
+        print(indent_multiline_string(logs.stderr).rstrip("\n"))
+
+
 def parse_user_supplied_id(id: Union[str, uuid.UUID]) -> str:
     """Verifies that a user-defined id is of the expected types, returning the string version of the id."""
     if not isinstance(id, str) and not isinstance(id, uuid.UUID):
         raise InvalidUserArgumentException("Provided id must be either str or uuid.")
 
     if isinstance(id, uuid.UUID):
         return str(id)
@@ -123,29 +143,35 @@
     return ParamSpec(
         val=_bytes_to_base64_string(serialize_val(val, serialization_type, derived_from_bson)),
         serialization_type=serialization_type,
     )
 
 
 def generate_engine_config(
-    integrations: Dict[str, IntegrationInfo], integration_name: Optional[str]
+    integrations: Dict[str, ResourceInfo],
+    integration_name: Optional[Union[str, DynamicK8sResource]],
 ) -> Optional[EngineConfig]:
     """Generates an EngineConfig from an integration info object.
 
     Both None and "Aqueduct" (case-insensitive) map to the Aqueduct Engine.
     """
+    if isinstance(integration_name, DynamicK8sResource):
+        integration_name = integration_name.name()
+
     if integration_name is None or integration_name.lower() == "aqueduct":
         return None
 
     if integration_name not in integrations.keys():
         raise InvalidIntegrationException(
             "Not connected to compute integration `%s`!" % integration_name
         )
 
     integration = integrations[integration_name]
+    validate_integration_is_connected(integration_name, integration.exec_state)
+
     if integration.service == ServiceType.AIRFLOW:
         return EngineConfig(
             type=RuntimeType.AIRFLOW,
             name=integration_name,
             airflow_config=AirflowEngineConfig(
                 integration_id=integration.id,
             ),
```

### Comparing `aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/PKG-INFO` & `aqueduct-sdk-0.3.0/aqueduct_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.2.9
-Summary: Python SDK for the Aqueduct prediction infrastructure
+Version: 0.3.0
+Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-[<img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width= "35%" />](https://www.aqueducthq.com)
 
-## Aqueduct: The easiest way to run ML on any cloud
 
+<div align="center">
+  <a href="https://aqueducthq.com">
+    <img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width="40%" />
+  </a>
+  
+  <h2 style="border: 0px white;">The Python API to run machine learning in your cloud</h2>
+
+### 📢 [Slack](https://slack.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🗺️ [Roadmap](https://roadmap.aqueducthq.com)&nbsp;&nbsp;|&nbsp;&nbsp;🐞 [Report a bug](https://github.com/aqueducthq/aqueduct/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5BBUG%5D)&nbsp;&nbsp;|&nbsp;&nbsp;✍️ [Blog](https://blog.aqueducthq.com)
+
+  
 [![Start Sandbox](https://img.shields.io/static/v1?label=%20&logo=github&message=Start%20Sandbox&color=black)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=496844646)
 [![Downloads](https://pepy.tech/badge/aqueduct-ml/month)](https://pypi.org/project/aqueduct-ml/)
 [![Slack](https://img.shields.io/static/v1.svg?label=chat&message=on%20slack&color=27b1ff&style=flat)](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A)
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/aqueducthq/aqueduct/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/aqueduct-ml.svg)](https://pypi.org/project/aqueduct-ml/)
 [![Tests](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml)
+</div>
+
+**Aqueduct enables you to easily define, run, and manage AI & ML tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
-**Aqueduct enables you to easily run machine learning tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/867892/230214641-b0aec53b-4988-4581-84ed-134f97ed9276.png" width="80%" />
+</p>
 
-Aqueduct is an open-source MLOps framework that allows you to define ML tasks in vanilla Python, run those tasks on any infrastructure you'd like to use, and gain visibility into the execution and performance of your ML. **[See what tools Aqueduct works with. →](https://aqueducthq.com/integrations/)**
+Aqueduct is an open-source MLOps framework that allows you to write code in vanilla Python, run that code on any cloud infrastructure you'd like to use, and gain visibility into the execution and performance of your models and predictions. **[See what infrastructure Aqueduct works with. →](https://aqueducthq.com/integrations/)**
 
 Here's how you can get started: 
 
 ```bash
 pip3 install aqueduct-ml
 aqueduct start
 ```
@@ -92,8 +105,8 @@
 * and more details on [creating workflows](https://docs.aqueducthq.com/workflows)
 
 If you have questions or comments or would like to learn more about what we're
 building, please [reach out](mailto:hello@aqueducthq.com), [join our Slack
 channel](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A), or [start a conversation on GitHub](https://github.com/aqueducthq/aqueduct/issues/new).
 We'd love to hear from you!
 
-If you're interested in contributing, please check out our [roadmap](https://github.com/aqueducthq/aqueduct/wiki/Aqueduct-Roadmap) and join the development channel in [our community Slack](https://slack.aqueducthq.com).
+If you're interested in contributing, please check out our [roadmap](https://roadmap.aqueducthq.com) and join the development channel in [our community Slack](https://slack.aqueducthq.com).
```

### Comparing `aqueduct-sdk-0.2.9/setup.py` & `aqueduct-sdk-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import os
 import sys
 from pathlib import Path
 
 import setuptools
 
+version = open("version").read()
+if not version:
+    raise Exception("Version file must contain a valid version string.")
+
 readme_path = Path(os.environ["PWD"], "../README.md")
 long_description = open(readme_path).read()
 
 req_file_name = "requirements/python-%s-%s.txt" % (sys.version_info[0], sys.version_info[1])
 
 if os.path.exists(req_file_name):
     install_requires = open(req_file_name).read().strip().split("\n")
 else:
     raise Exception(
         "Python Version %s.%s not supported" % (sys.version_info[0], sys.version_info[1])
     )
 
 setuptools.setup(
     name="aqueduct-sdk",
-    version="0.2.9",
+    version=version,
     author="Aqueduct, Inc.",
     author_email="hello@aqueducthq.com",
-    description="Python SDK for the Aqueduct prediction infrastructure",
+    description="Python SDK for Aqueduct",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aqueducthq/aqueduct",
     license="Apache License 2.0",
     packages=setuptools.find_packages(),
     install_requires=install_requires,
     setup_requires=["numpy", "cython", "packaging"],
```

