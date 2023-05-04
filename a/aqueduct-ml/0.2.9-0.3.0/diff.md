# Comparing `tmp/aqueduct-ml-0.2.9.tar.gz` & `tmp/aqueduct-ml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-ml-0.2.9.tar", last modified: Wed Apr  5 19:18:44 2023, max compression
+gzip compressed data, was "aqueduct-ml-0.3.0.tar", last modified: Thu May  4 05:05:25 2023, max compression
```

## Comparing `aqueduct-ml-0.2.9.tar` & `aqueduct-ml-0.3.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6924 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/migrators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/operators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3010 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/athena.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3297 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      694 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2795 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/connector.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12959 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6060 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/relational.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8183 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6878 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5473 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15071 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/extract_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1471 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      419 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8793 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/execute_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9678 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/execute_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      435 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7496 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      787 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/parse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3082 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/timer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6924 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5729 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/bin/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29101 2023-04-04 22:01:25.000000 aqueduct-ml-0.2.9/bin/aqueduct
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-04-04 22:01:25.000000 aqueduct-ml-0.2.9/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      807 2023-04-04 22:01:25.000000 aqueduct-ml-0.2.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.580891 aqueduct-ml-0.3.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2023-05-04 05:05:25.580891 aqueduct-ml-0.3.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.544890 aqueduct-ml-0.3.0/aqueduct_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.544890 aqueduct-ml-0.3.0/aqueduct_executor/migrators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.544890 aqueduct-ml-0.3.0/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.548890 aqueduct-ml-0.3.0/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.548890 aqueduct-ml-0.3.0/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.552890 aqueduct-ml-0.3.0/aqueduct_executor/operators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.552890 aqueduct-ml-0.3.0/aqueduct_executor/operators/airflow/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/airflow/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3010 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/airflow/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/airflow/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/airflow/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.552890 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.560891 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/athena.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3297 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      694 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2892 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/connector.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15392 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6057 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/relational.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8690 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6878 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.560891 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5473 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.568890 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.568890 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.572890 aqueduct-ml-0.3.0/aqueduct_executor/operators/param_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/param_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/param_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      419 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/param_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/param_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.572890 aqueduct-ml-0.3.0/aqueduct_executor/operators/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/spark/execute_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/spark/execute_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/spark/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.572890 aqueduct-ml-0.3.0/aqueduct_executor/operators/system_metric_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      435 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.576890 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7531 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/execution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.580891 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/parse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/storage.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/timer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-03-07 22:19:47.000000 aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.580891 aqueduct-ml-0.3.0/aqueduct_ml.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2023-05-04 05:05:25.000000 aqueduct-ml-0.3.0/aqueduct_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5703 2023-05-04 05:05:25.000000 aqueduct-ml-0.3.0/aqueduct_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-04 05:05:25.000000 aqueduct-ml-0.3.0/aqueduct_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-04 05:05:25.000000 aqueduct-ml-0.3.0/aqueduct_ml.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 05:05:25.580891 aqueduct-ml-0.3.0/bin/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29290 2023-05-04 03:12:43.000000 aqueduct-ml-0.3.0/bin/aqueduct
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-04 03:12:43.000000 aqueduct-ml-0.3.0/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-04 05:05:25.580891 aqueduct-ml-0.3.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1082 2023-05-04 03:10:27.000000 aqueduct-ml-0.3.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-04 03:12:43.000000 aqueduct-ml-0.3.0/version
```

### Comparing `aqueduct-ml-0.2.9/PKG-INFO` & `aqueduct-ml-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.2.9
-Summary: Prediction Infrastructure for Data Scientists
+Version: 0.3.0
+Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
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

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `aqueduct-ml-0.3.0/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `aqueduct-ml-0.3.0/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `aqueduct-ml-0.3.0/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `aqueduct-ml-0.3.0/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `aqueduct-ml-0.3.0/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `aqueduct-ml-0.3.0/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/execute.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/spec.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/athena.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/bigquery.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/common.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/config.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,19 @@
 
     # Config credentials
     config_file_path: str = ""
     config_file_content: str = ""
     config_file_profile: str = ""
 
     bucket: str = ""
-
     region: str = ""
+
+    # This is unused for data integrations. It is only used for storage.
+    root_dir: str = ""
+
     use_as_storage: str = ""
 
 
 class AthenaConfig(models.BaseConfig):
     # default type to ACCESS_KEY mainly for backward compatibility
     type: AWSCredentialType = AWSCredentialType.ACCESS_KEY
```

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/connector.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/execute.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import platform
 import sys
 from typing import Any
 
 from aqueduct_executor.operators.connectors.data import common, config, connector, extract
 from aqueduct_executor.operators.connectors.data.spec import (
     AQUEDUCT_DEMO_NAME,
     AuthenticateSpec,
@@ -43,19 +44,57 @@
     - load-table
     - delete-saved-objects
     - discover
 
     Arguments:
     - spec: The spec provided for this operator.
     """
+    return execute_data_spec(
+        spec=spec,
+        read_artifacts_func=utils.read_artifacts,
+        write_artifact_func=utils.write_artifact,
+        setup_connector_func=setup_connector,
+        is_spark=False,
+    )
+
+
+def execute_data_spec(
+    spec: Spec,
+    read_artifacts_func: Any,
+    write_artifact_func: Any,
+    setup_connector_func: Any,
+    is_spark: bool,
+    **kwargs: Any,
+) -> None:
+    """
+    This function executes the spec provided. If run in a Spark environment, it uses
+    the Spark specific utils functions to read/write to storage layer and to setup connectors.
+    The only kwarg we expect is spark_session_obj
+
+    Args:
+        spec: The spec provided for this operator.
+        read_artifacts_func: function used to read artifacts from storage layer
+        write_artifact_func: function used to write artifacts to storage layer
+        setup_connector_func: function to use to setup the connectors
+        is_spark Whether or not we are running in a Spark env.
+    """
     storage = parse_storage(spec.storage_config)
     exec_state = ExecutionState(user_logs=Logs())
 
     try:
-        _execute(spec, storage, exec_state)
+        _execute(
+            spec,
+            storage,
+            exec_state,
+            read_artifacts_func,
+            write_artifact_func,
+            setup_connector_func,
+            is_spark,
+            **kwargs,
+        )
         # Write operator execution metadata
         # Each decorator may set exec_state.status to FAILED, but if none of them did, then we are
         # certain that the operator succeeded.
         if exec_state.status == ExecutionStatus.FAILED:
             print(f"Failed with error. Full Logs:\n{exec_state.json()}")
             utils.write_exec_state(storage, spec.metadata_path, exec_state)
             sys.exit(1)
@@ -81,129 +120,183 @@
         )
         print(f"Failed with system error. Full Logs:\n{exec_state.json()}")
 
         utils.write_exec_state(storage, spec.metadata_path, exec_state)
         sys.exit(1)
 
 
-def _execute(spec: Spec, storage: Storage, exec_state: ExecutionState) -> None:
+def _execute(
+    spec: Spec,
+    storage: Storage,
+    exec_state: ExecutionState,
+    read_artifacts_func: Any,
+    write_artifact_func: Any,
+    setup_connector_func: Any,
+    is_spark: bool,
+    **kwargs: Any,
+) -> None:
     if spec.type == JobType.DELETESAVEDOBJECTS:
         run_delete_saved_objects(spec, storage, exec_state)
 
     # Because constructing certain connectors (eg. Postgres) can also involve authentication,
     # we do both in `run_authenticate()`, and give a more helpful error message on failure.
     elif spec.type == JobType.AUTHENTICATE:
-        run_authenticate(spec, exec_state, is_demo=(spec.name == AQUEDUCT_DEMO_NAME))
+        run_authenticate(
+            spec,
+            exec_state,
+            is_demo=(spec.name == AQUEDUCT_DEMO_NAME),
+            setup_connector_func=setup_connector_func,
+        )
 
     else:
-        op = setup_connector(spec.connector_name, spec.connector_config)
+        op = setup_connector_func(spec.connector_name, spec.connector_config)
         if spec.type == JobType.EXTRACT:
-            run_extract(spec, op, storage, exec_state)
+            run_extract(
+                spec,
+                op,
+                storage,
+                exec_state,
+                read_artifacts_func,
+                write_artifact_func,
+                is_spark,
+                **kwargs,
+            )
         elif spec.type == JobType.LOADTABLE:
-            run_load_table(spec, op, storage)
+            run_load_table(spec, op, storage, is_spark)
         elif spec.type == JobType.LOAD:
-            run_load(spec, op, storage, exec_state)
+            run_load(spec, op, storage, exec_state, read_artifacts_func, is_spark, **kwargs)
         elif spec.type == JobType.DISCOVER:
             run_discover(spec, op, storage)
         else:
             raise Exception("Unknown job: %s" % spec.type)
 
 
 def run_authenticate(
     spec: AuthenticateSpec,
     exec_state: ExecutionState,
     is_demo: bool,
+    setup_connector_func: Any,
 ) -> None:
     @exec_state.user_fn_redirected(
         failure_tip=TIP_DEMO_CONNECTION if is_demo else TIP_INTEGRATION_CONNECTION
     )
     def _authenticate() -> None:
-        op = setup_connector(spec.connector_name, spec.connector_config)
+        op = setup_connector_func(spec.connector_name, spec.connector_config)
         op.authenticate()
 
     _authenticate()
 
 
 def run_extract(
-    spec: ExtractSpec, op: connector.DataConnector, storage: Storage, exec_state: ExecutionState
+    spec: ExtractSpec,
+    op: connector.DataConnector,
+    storage: Storage,
+    exec_state: ExecutionState,
+    read_artifacts_func: Any,
+    write_artifact_func: Any,
+    is_spark: bool,
+    **kwargs: Any,
 ) -> None:
     extract_params = spec.parameters
 
     # Search for user-defined placeholders if this is a relational query, and replace them with
     # the appropriate values.
     if isinstance(extract_params, extract.RelationalParams) or isinstance(
         extract_params, extract.MongoDBParams
     ):
-        input_vals, _, _ = utils.read_artifacts(
-            storage,
-            spec.input_content_paths,
-            spec.input_metadata_paths,
+        input_vals, _, _ = read_artifacts_func(
+            storage=storage,
+            input_paths=spec.input_content_paths,
+            input_metadata_paths=spec.input_metadata_paths,
+            **kwargs,
         )
         assert all(
             isinstance(param_val, str) for param_val in input_vals
         ), "Parameter value must be a string."
         extract_params.compile(input_vals)
 
     @exec_state.user_fn_redirected(failure_tip=TIP_EXTRACT)
     def _extract() -> Any:
-        return op.extract(spec.parameters)
+        if is_spark:
+            return op.extract_spark(spec.parameters, **kwargs)  # type: ignore
+        else:
+            return op.extract(spec.parameters)
 
     output = _extract()
 
     output_artifact_type = ArtifactType.TABLE
     derived_from_bson = isinstance(extract_params, extract.MongoDBParams)
     if isinstance(extract_params, extract.S3Params):
         output_artifact_type = extract_params.artifact_type
         # If the type of the output is tuple, then it could be a multi-file S3 request so we
         # overwrite the output type to tuple.
         if isinstance(output, tuple):
             output_artifact_type = ArtifactType.TUPLE
 
     if exec_state.status != ExecutionStatus.FAILED:
-        utils.write_artifact(
+        write_artifact_func(
             storage,
             output_artifact_type,
             derived_from_bson,
             spec.output_content_path,
             spec.output_metadata_path,
             output,
             system_metadata={},
+            **kwargs,
         )
 
 
 def run_delete_saved_objects(spec: Spec, storage: Storage, exec_state: ExecutionState) -> None:
     results = {}
     assert isinstance(spec.connector_name, dict)
     for integration in spec.connector_name:
         op = setup_connector(spec.connector_name[integration], spec.connector_config[integration])
         results[integration] = op.delete(spec.integration_to_object[integration])
     utils.write_delete_saved_objects_results(storage, spec.output_content_path, results)
 
 
 def run_load(
-    spec: LoadSpec, op: connector.DataConnector, storage: Storage, exec_state: ExecutionState
+    spec: LoadSpec,
+    op: connector.DataConnector,
+    storage: Storage,
+    exec_state: ExecutionState,
+    read_artifacts_func: Any,
+    is_spark: bool,
+    **kwargs: Any,
 ) -> None:
-    inputs, input_types, _ = utils.read_artifacts(
-        storage,
-        [spec.input_content_path],
-        [spec.input_metadata_path],
+    inputs, input_types, _ = read_artifacts_func(
+        storage=storage,
+        input_paths=[spec.input_content_path],
+        input_metadata_paths=[spec.input_metadata_path],
+        **kwargs,
     )
     if len(inputs) != 1:
         raise Exception("Expected 1 input artifact, but got %d" % len(inputs))
 
     @exec_state.user_fn_redirected(failure_tip=TIP_LOAD)
     def _load() -> None:
-        op.load(spec.parameters, inputs[0], input_types[0])
+        if is_spark:
+            op.load_spark(spec.parameters, inputs[0], input_types[0])  # type: ignore
+        else:
+            op.load(spec.parameters, inputs[0], input_types[0])
 
     _load()
 
 
-def run_load_table(spec: LoadTableSpec, op: connector.DataConnector, storage: Storage) -> None:
+def run_load_table(
+    spec: LoadTableSpec,
+    op: connector.DataConnector,
+    storage: Storage,
+    is_spark: bool,
+) -> None:
     df = utils._read_csv(storage.get(spec.csv))
-    op.load(spec.load_parameters.parameters, df, ArtifactType.TABLE)
+    if is_spark:
+        op.load_spark(spec.load_parameters.parameters, df, ArtifactType.TABLE)  # type: ignore
+    else:
+        op.load(spec.load_parameters.parameters, df, ArtifactType.TABLE)
 
 
 def run_discover(spec: DiscoverSpec, op: connector.DataConnector, storage: Storage) -> None:
     tables = op.discover()
     utils.write_discover_results(storage, spec.output_content_path, tables)
 
 
@@ -263,36 +356,31 @@
             raise MissingConnectorDependencyException(
                 "Unable to initialize the SQL Server connector. Have you run `aqueduct install sqlserver`?"
             )
 
         from aqueduct_executor.operators.connectors.data.sql_server import (  # type: ignore
             SqlServerConnector as OpConnector,
         )
-    elif connector_name == common.Name.MYSQL:
+    elif connector_name == common.Name.MYSQL or connector_name == common.Name.MARIA_DB:
         try:
+            # Use pythonic mysql library to fix crossplatform compatibility issues.
+            # MySQLdb is a C-based library
+            import pymysql
+
+            # Implementation can be found here: https://github.com/PyMySQL/PyMySQL/blob/main/pymysql/__init__.py
+            pymysql.install_as_MySQLdb()
             import MySQLdb
         except:
             raise MissingConnectorDependencyException(
-                "Unable to initialize the MySQL connector. Have you run `aqueduct install mysql`?"
+                "Unable to initialize the MySQL\/MariaDB connector. Have you run `aqueduct install mysql`?"
             )
 
         from aqueduct_executor.operators.connectors.data.mysql import (  # type: ignore
             MySqlConnector as OpConnector,
         )
-    elif connector_name == common.Name.MARIA_DB:
-        try:
-            import MySQLdb
-        except:
-            raise MissingConnectorDependencyException(
-                "Unable to initialize the MariaDB connector. Have you run `aqueduct install mariadb`?"
-            )
-
-        from aqueduct_executor.operators.connectors.data.maria_db import (  # type: ignore
-            MariaDbConnector as OpConnector,
-        )
     elif connector_name == common.Name.AZURE_SQL:
         try:
             import pyodbc
         except:
             raise MissingConnectorDependencyException(
                 "Unable to initialize the Azure SQL connector. Have you run `aqueduct install azuresql`?"
             )
```

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/extract.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import re
 import uuid
 from typing import Any, Dict, List, Optional, Union
 
-from aqueduct.integrations.parameters import BUILT_IN_EXPANSIONS, TAG_PATTERN
+from aqueduct.resources.parameters import BUILT_IN_EXPANSIONS, TAG_PATTERN
 from aqueduct_executor.operators.connectors.data import common, models
 from aqueduct_executor.operators.utils.enums import ArtifactType
 from pydantic import parse_obj_as
 
 # The TAG for 'previous table' when the user specifies a chained query.
 PREV_TABLE_TAG = "$"
```

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/gcs.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/load.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/main.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/models.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/mongodb.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/mysql.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/postgres.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/relational.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/s3.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,26 +21,36 @@
 
 
 class S3Connector(connector.DataConnector):
     def __init__(self, config: S3Config):
         session = construct_boto_session(config)
         self.s3 = session.resource("s3")
         self.bucket = config.bucket
+        self.root_dir = config.root_dir
 
     def authenticate(self) -> None:
         try:
             # Below is a low-overhead way of checking if the user has access to the bucket.
             # Source: https://stackoverflow.com/a/49817544
             self.s3.meta.client.head_bucket(Bucket=self.bucket)
         except ClientError as e:
             raise Exception(
                 "Bucket does not exist or you do not have permission to access the bucket: %s."
                 % str(e)
             )
 
+        # Check that any user-supplied root directory exists.
+        if self.root_dir != "":
+            # If nothing is returned by this filter call, then the directory does not exist.
+            if len(list(self.s3.Bucket(self.bucket).objects.filter(Prefix=self.root_dir))) == 0:
+                raise Exception(
+                    "Supplied root directory `%s` does not exist in bucket %s."
+                    % (self.root_dir, self.bucket)
+                )
+
     def discover(self) -> List[str]:
         raise Exception("Discover is not supported for S3.")
 
     def fetch_object(self, key: str, params: extract.S3Params) -> Any:
         response = self.s3.Object(self.bucket, key).get()
         data = response["Body"].read()
```

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/snowflake.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/s3.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spec.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/sql_server.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/sqlite.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/utils.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/conf.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/utils.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/execute.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/execute.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
 import json
 import os
 import shutil
+import subprocess
 import sys
 import tracemalloc
 import uuid
 from typing import Any, Callable, Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
@@ -138,14 +139,15 @@
     sys.path.pop(0)
     return results, system_metadata
 
 
 def _validate_result_count_and_infer_type(
     spec: FunctionSpec,
     results: List[Any],
+    infer_type_func: Any,
 ) -> List[ArtifactType]:
     """
     Validates that the expected number of results were returned by the Function
     and infers the ArtifactType of each result.
 
     Args:
         spec: The FunctionSpec for the Function
@@ -160,35 +162,38 @@
     if len(spec.output_content_paths) > 1 and len(spec.output_content_paths) != len(results):
         raise ExecFailureException(
             failure_type=FailureType.USER_FATAL,
             tip="Expected function to have %s outputs, but instead it had %s."
             % (len(spec.output_content_paths), len(results)),
         )
 
-    return [infer_artifact_type(res) for res in results]
+    return [infer_type_func(res) for res in results]
 
 
 def _write_artifacts(
+    write_artifact_func: Any,
     results: Any,
     result_types: List[ArtifactType],
     derived_from_bson: bool,
     output_content_paths: List[str],
     output_metadata_paths: List[str],
     system_metadata: Any,
     storage: Storage,
+    **kwargs: Any,
 ) -> None:
     for i, result in enumerate(results):
-        utils.write_artifact(
+        write_artifact_func(
             storage,
             result_types[i],
             derived_from_bson,
             output_content_paths[i],
             output_metadata_paths[i],
             result,
             system_metadata=system_metadata,
+            **kwargs,
         )
 
 
 def validate_spec(spec: FunctionSpec) -> None:
     if len(spec.input_content_paths) != len(spec.input_metadata_paths):
         raise Exception(
             "Found inconsistent number of input paths (%d) and input metadata paths (%d)"
@@ -235,23 +240,56 @@
         shutil.rmtree(spec.function_extract_path)
 
 
 def run(spec: FunctionSpec) -> None:
     """
     Executes a function operator.
     """
+    execute_function_spec(
+        spec=spec,
+        read_artifacts_func=utils.read_artifacts,
+        write_artifact_func=utils.write_artifact,
+        infer_type_func=infer_artifact_type,
+    )
+
+
+def execute_function_spec(
+    spec: FunctionSpec,
+    read_artifacts_func: Any,
+    write_artifact_func: Any,
+    infer_type_func: Any,
+    **kwargs: Any,
+) -> None:
+    """
+    Executes a function operator. If run in a Spark environment, it uses the Spark specific utils
+    functions to read/write to storage layer and to infer the type of artifact.
+    The only kwarg we expect is spark_session_obj.
+
+    Args:
+        spec: The spec provided for this operator.
+        read_artifacts_func: function used to read artifacts from storage layer
+        write_artifact_func: function used to write artifacts to storage layer
+        infer_type_func: function used to infer type of artifacts returned by operators.
+    """
     exec_state = ExecutionState(user_logs=Logs())
     storage = parse_storage(spec.storage_config)
     try:
+        check_package_version_mismatch()
+
         validate_spec(spec)
 
         # Read the input data from intermediate storage.
         inputs, _, serialization_types = time_it(
             job_name=spec.name, job_type=spec.type.value, step="Reading Inputs"
-        )(utils.read_artifacts)(storage, spec.input_content_paths, spec.input_metadata_paths)
+        )(read_artifacts_func)(
+            storage=storage,
+            input_paths=spec.input_content_paths,
+            input_metadata_paths=spec.input_metadata_paths,
+            **kwargs,
+        )
 
         # We need to check for BSON_TABLE serialization type at both the top level
         # and within any serialized pickled collection (if it exists).
         derived_from_bson = SerializationType.BSON_TABLE in serialization_types
         if not derived_from_bson:
             for i, serialization_type in enumerate(serialization_types):
                 collection_data = check_and_fetch_pickled_collection_format(
@@ -271,15 +309,17 @@
         if exec_state.status == ExecutionStatus.FAILED:
             # user failure
             utils.write_exec_state(storage, spec.metadata_path, exec_state)
             sys.exit(1)
 
         print("Function invoked successfully!")
 
-        result_types = _validate_result_count_and_infer_type(spec, results)
+        result_types = _validate_result_count_and_infer_type(
+            spec=spec, results=results, infer_type_func=infer_type_func
+        )
 
         # Perform type checking on the function output.
         if spec.operator_type == OperatorType.METRIC:
             assert len(results) == 1, "Metric operator can only have a single output."
             result = results[0]
 
             if not (
@@ -312,23 +352,23 @@
                     tip=TIP_NOT_BOOL,
                 )
 
             # If the check returned a value we interpret to mean 'false', we exit here, but
             # not before recording the output artifact value (which will be False).
             if not check_passed:
                 print(f"Check Operator did not pass.")
-
-                utils.write_artifact(
-                    storage,
-                    ArtifactType.BOOL,
-                    derived_from_bson,  # derived_from_bson doesn't apply to bool artifact
-                    spec.output_content_paths[0],
-                    spec.output_metadata_paths[0],
-                    check_passed,
+                write_artifact_func(
+                    storage=storage,
+                    artifact_type=ArtifactType.BOOL,
+                    derived_from_bson=derived_from_bson,  # derived_from_bson doesn't apply to bool artifact
+                    output_path=spec.output_content_paths[0],
+                    output_metadata_path=spec.output_metadata_paths[0],
+                    content=check_passed,
                     system_metadata=system_metadata,
+                    **kwargs,
                 )
 
                 check_severity = spec.check_severity
                 if spec.check_severity is None:
                     print(
                         "Check operator has an unspecified severity on spec. Defaulting to ERROR."
                     )
@@ -355,21 +395,23 @@
                         tip="Expected type %s for the %d-th output of function, but it is of type %s."
                         % (expected_output_type, i, result_types[i]),
                     )
 
         time_it(job_name=spec.name, job_type=spec.type.value, step="Writing Outputs")(
             _write_artifacts
         )(
-            results,
-            result_types,
-            derived_from_bson,
-            spec.output_content_paths,
-            spec.output_metadata_paths,
-            system_metadata,
-            storage,
+            write_artifact_func=write_artifact_func,
+            results=results,
+            result_types=result_types,
+            derived_from_bson=derived_from_bson,
+            output_content_paths=spec.output_content_paths,
+            output_metadata_paths=spec.output_metadata_paths,
+            system_metadata=system_metadata,
+            storage=storage,
+            **kwargs,
         )
 
         # If we made it here, then the operator has succeeded.
         exec_state.status = ExecutionStatus.SUCCEEDED
         print(f"Succeeded! Full logs: {exec_state.json()}")
         utils.write_exec_state(storage, spec.metadata_path, exec_state)
 
@@ -406,7 +448,22 @@
     extract_function.run(spec)
 
     requirements_path = os.path.join(op_path, "requirements.txt")
     if os.path.exists(requirements_path):
         os.system("{} -m pip install -r {}".format(sys.executable, requirements_path))
 
     run(spec)
+
+
+def check_package_version_mismatch() -> None:
+    expected_version = os.environ.get("AQUEDUCT_EXPECTED_VERSION")
+    if expected_version:
+        aqueduct_version = subprocess.check_output(["aqueduct", "version"]).decode("utf-8").strip()
+
+        print(
+            f"Comparing Aqueduct version ({aqueduct_version}) to expected version ({expected_version})"
+        )
+        if aqueduct_version != expected_version:
+            raise ExecFailureException(
+                failure_type=FailureType.USER_FATAL,
+                tip=f"Aqueduct version ({aqueduct_version}) does not match expected version ({expected_version})",
+            )
```

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/extract_function.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/get_extract_path.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/install_requirements.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/main.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/set_conda_version.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/spec.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/function_executor/spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,16 +34,17 @@
     output_metadata_paths: List[str]
     expected_output_artifact_types: List[ArtifactType]
     operator_type: OperatorType
 
     # This is specific to the check operator. This is left unset by any other function type.
     check_severity: Optional[CheckSeverity]
 
-    # This is always unset - it is only here because we forbid extra fields.
+    # These are always unset - they are only here because we forbid extra fields.
     resources: Optional[Any]
+    image: Optional[Any]
 
     class Config:
         extra = Extra.forbid
 
 
 def parse_spec(spec_json: bytes) -> FunctionSpec:
     """
```

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/execute.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/spec.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/utils.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/execute.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/spec.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/enums.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/execution.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 _TIP_CREATE_BUG_REPORT = (
     f"Please create bug report in github: {_GITHUB_ISSUE_LINK} . "
     "We will get back to you as soon as we can."
 )
 TIP_UNKNOWN_ERROR = f"Sorry, we've run into an unexpected error! {_TIP_CREATE_BUG_REPORT}"
 TIP_INTEGRATION_CONNECTION = (
     "We were unable to connect to this integration. "
-    "Please check your credentials or contact your integration's provider."
+    "If the stack trace is not helpful, please check your credentials or contact your integration's provider."
 )
 TIP_DEMO_CONNECTION = f"We have trouble connecting to demo DB. {_TIP_CREATE_BUG_REPORT}"
 
 TIP_EXTRACT = "We couldn't execute the provided query. Please double check your query is correct."
 TIP_LOAD = "We couldn't load to the integration. Please make sure the target exists, or you have the right permission."
 TIP_DISCOVER = "We couldn't list items in the integration. Please make sure your credentials have the right permission."
```

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/config.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 class FileStorageConfig(BaseModel):
     directory: str
 
 
 class S3StorageConfig(BaseModel):
     region: str
     bucket: str
+
+    # Expected to be in the format "path/to/dir/" (without a leading slash, but with a trailing one).
+    root_dir: str = ""
+
     credentials_path: str
     credentials_profile: str
     aws_access_key_id: str = ""
     aws_secret_access_key: str = ""
 
 
 class GCSStorageConfig(BaseModel):
```

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/file.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/gcs.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/parse.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/s3.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,49 +28,70 @@
                 aws_secret_access_key=os.environ["AWS_SECRET_ACCESS_KEY"],
             )
         else:
             # Boto3 uses an environment variable to determine the credentials filepath and profile
             os.environ["AWS_SHARED_CREDENTIALS_FILE"] = config.credentials_path
             os.environ["AWS_PROFILE"] = config.credentials_profile
             self._client = boto3.client("s3", config=BotoConfig(region_name=config.region))
+
         self._config = config
 
-        bucket, key_prefix = parse_s3_path(self._config.bucket)
+        bucket, key_prefix = parse_s3_bucket_and_key_prefix(
+            self._config.bucket, self._config.root_dir
+        )
         self._bucket = bucket
         self._key_prefix = key_prefix
 
     def put(self, key: str, value: bytes) -> None:
-        key = self._prefix_key(key)
+        key = self._resolve_full_key(key)
         print(f"writing to s3: {key}")
         self._client.put_object(Bucket=self._bucket, Key=key, Body=value)
 
     def get(self, key: str) -> bytes:
-        key = self._prefix_key(key)
+        key = self._resolve_full_key(key)
         print(f"reading from s3: {key}")
         return self._client.get_object(Bucket=self._bucket, Key=key)["Body"].read()  # type: ignore
 
     def exists(self, key: str) -> bool:
-        key = self._prefix_key(key)
+        key = self._resolve_full_key(key)
         print(f"checking if exists in s3: {key}")
         try:
             self._client.head_object(Bucket=self._bucket, Key=key)
         except ClientError as e:
             # checking for NoSuchKey error
             if e.response["Error"]["Code"] == "404":
                 return False
             else:
                 # TODO: ENG-2428 we should explicitly surface other error types to the caller
                 # instead of just returning `false` for non s3.ErrCodeNoSuchKey errors.
                 return False
         return True
 
-    def _prefix_key(self, key: str) -> str:
+    def _resolve_full_key(self, key: str) -> str:
+        """The `key_prefix` is expected to be in the format `path/to/dir/`."""
         if not self._key_prefix:
             return key
-        return self._key_prefix + "/" + key
 
+        assert self._key_prefix[0] != "/" and self._key_prefix[-1] == "/"
+        return self._key_prefix + key
+
+
+def _sanitize_path(path: str) -> str:
+    """Sanitize the given path to be in the format `path/to/dir/` (no leading slash but one trailing slash)."""
+    if path == "":
+        return path
+    if path[0] == "/":
+        path = path[1:]
+    if path[-1] != "/":
+        path += "/"
+    return path
 
-def parse_s3_path(s3_path: str) -> Tuple[str, str]:
-    path_parts = s3_path.replace("s3://", "").split("/")
+
+def parse_s3_bucket_and_key_prefix(s3_bucket_path: str, root_dir_path: str) -> Tuple[str, str]:
+    path_parts = s3_bucket_path.replace("s3://", "").split("/")
     bucket = path_parts.pop(0)
-    key = "/".join(path_parts)
-    return bucket, key
+
+    if root_dir_path != "":
+        path_parts += [_sanitize_path(root_dir_path)]
+
+    key_prefix = "/".join(path_parts)
+    return bucket, _sanitize_path(key_prefix)
```

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/timer.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/utils.py` & `aqueduct-ml-0.3.0/aqueduct_executor/operators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.9/aqueduct_ml.egg-info/PKG-INFO` & `aqueduct-ml-0.3.0/aqueduct_ml.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.2.9
-Summary: Prediction Infrastructure for Data Scientists
+Version: 0.3.0
+Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
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

### Comparing `aqueduct-ml-0.2.9/aqueduct_ml.egg-info/SOURCES.txt` & `aqueduct-ml-0.3.0/aqueduct_ml.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MANIFEST.in
 requirements.txt
 setup.py
+version
 aqueduct_executor/__init__.py
 aqueduct_executor/migrators/__init__.py
 aqueduct_executor/migrators/artifact_migration_000016/__init__.py
 aqueduct_executor/migrators/artifact_migration_000016/execute.py
 aqueduct_executor/migrators/artifact_migration_000016/main.py
 aqueduct_executor/migrators/artifact_migration_000016/spec.py
 aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
@@ -98,10 +99,9 @@
 aqueduct_executor/operators/utils/storage/gcs.py
 aqueduct_executor/operators/utils/storage/parse.py
 aqueduct_executor/operators/utils/storage/s3.py
 aqueduct_executor/operators/utils/storage/storage.py
 aqueduct_ml.egg-info/PKG-INFO
 aqueduct_ml.egg-info/SOURCES.txt
 aqueduct_ml.egg-info/dependency_links.txt
-aqueduct_ml.egg-info/requires.txt
 aqueduct_ml.egg-info/top_level.txt
 bin/aqueduct
```

### Comparing `aqueduct-ml-0.2.9/bin/aqueduct` & `aqueduct-ml-0.3.0/bin/aqueduct`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import distro
 import requests
 import yaml
 from packaging.version import parse as parse_version
 from tqdm import tqdm
 
-SCHEMA_VERSION = "25"
+SCHEMA_VERSION = "26"
 CHUNK_SIZE = 4096
 
 # Connector Package Version Bounds
 PYMONGO_VERSION_BOUND = "<=4.3.3"
 PSYCOPG2_VERSION_BOUND = "<=2.9.5"
 BIGQUERY_VERSION_BOUND = "<=3.5.0"
 SNOWFLAKE_VERSION_BOUND = "<=1.4.4"
@@ -33,15 +33,15 @@
 MYSQL_CLIENT_VERSION_BOUND = "<=2.1.1"
 PYODBC_VERSION_BOUND = "<=4.0.35"
 
 base_directory = os.path.join(os.environ["HOME"], ".aqueduct")
 server_directory = os.path.join(os.environ["HOME"], ".aqueduct", "server")
 ui_directory = os.path.join(os.environ["HOME"], ".aqueduct", "ui")
 
-package_version = "0.2.9"
+package_version = "0.3.0"
 aws_credentials_path = os.path.join(os.environ["HOME"], ".aws", "credentials")
 
 default_server_port = 8080
 
 s3_server_prefix = (
     "https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/%s/server" % package_version
 )
@@ -183,21 +183,17 @@
 
 
 def download_server_binaries(architecture):
     print("Downloading server binaries...")
     with open(os.path.join(server_directory, "bin/server"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/{architecture}/server"), f, "Server")
     with open(os.path.join(server_directory, "bin/executor"), "wb") as f:
-        _download_file(
-            os.path.join(s3_server_prefix, f"bin/{architecture}/executor"), f, "Executor"
-        )
+        _download_file(os.path.join(s3_server_prefix, f"bin/{architecture}/executor"), f, "Executor")
     with open(os.path.join(server_directory, "bin/migrator"), "wb") as f:
-        _download_file(
-            os.path.join(s3_server_prefix, f"bin/{architecture}/migrator"), f, "Migrator"
-        )
+        _download_file(os.path.join(s3_server_prefix, f"bin/{architecture}/migrator"), f, "Migrator")
 
     print("Downloading integration set up scripts...")
     with open(os.path.join(server_directory, "bin/start-function-executor.sh"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/start-function-executor.sh"), f)
     with open(os.path.join(server_directory, "bin/dag.template"), "wb") as f:
         _download_file(os.path.join(s3_server_prefix, f"bin/dag.template"), f)
     with open(os.path.join(server_directory, "bin/install_sqlserver_ubuntu.sh"), "wb") as f:
@@ -283,14 +279,15 @@
         ]
     )
 
     if parse_version(current_version) < parse_version("0.1.0") and parse_version(package_version) >= parse_version("0.1.0"):
         # We add a couple new tables to the demo db for the v0.1.0 release.
         # If we want to add tables in other releases in the future, we should refactor each of them
         # into a helper function.
+        print("Adding new tables to the demo db...")
         data_script_path = os.path.join(server_directory, "db", "0.1.0", "create_tables.py")
         data_script_dir = os.path.dirname(data_script_path)
         if not os.path.isdir(data_script_dir):
             os.mkdir(data_script_dir)
         s3_path = ("https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/demo/0.1.0/create_tables.py")
         with open(data_script_path, "wb") as f:
             f.write(requests.get(s3_path).content)
@@ -383,33 +380,34 @@
     else:
         try:
             ec2_ip = requests.get(
                 "http://169.254.169.254/latest/meta-data/public-ipv4", timeout=0.25
             )
             if ec2_ip.status_code != 404: # User is in EC2 instance.
                 expose_ip = ec2_ip.content.decode("utf-8")
-            else:  
+            else:
                 # Assume is Google Cloud
                 metadata_flavor = {'Metadata-Flavor': 'Google'}
-                gcp_ip = requests.get('http://169.254.169.254/computeMetadata/v1/instance/network-interfaces/0/access-configs/0/external-ip', headers = metadata_flavor, timeout=0.25)
+                gcp_ip = requests.get('http://169.254.169.254/computeMetadata/v1/instance/network-interfaces/0/access-configs/0/external-ip', headers=metadata_flavor, timeout=0.25)
                 if gcp_ip.status_code != 404:
                     expose_ip = gcp_ip.text
                 else:
                     # Assume is Azure
-                    azure_ip = requests.get('http://169.254.169.254/metadata/instance/network/interface/0/ipv4/ipAddress/0/publicIpAddress?api-version=2017-08-01&format=text', headers = {'Metadata': 'true'}, timeout=0.25)
+                    azure_ip = requests.get('http://169.254.169.254/metadata/instance/network/interface/0/ipv4/ipAddress/0/publicIpAddress?api-version=2017-08-01&format=text', headers={'Metadata': 'true'}, timeout=0.25)
                     if azure_ip.status_code != 404:
                         expose_ip = azure_ip.text
                     else:
                         # Default
                         expose_ip = "<IP_ADDRESS>"
         except:  # If you're not running on EC2, this will return an error.
             expose_ip = "<IP_ADDRESS>"
-    
+
     return expose_ip
 
+
 def generate_welcome_message(addr, port):
     apikey = get_apikey()
 
     return (
         welcome_message % (apikey, package_version, addr, port, apikey),
         login_url % (addr, port, apikey),
     )
@@ -452,42 +450,49 @@
         str(server_port),
         "--external-ip",
         addr,
     ]
 
     if expose:
         command.append("--expose")
-    
+
     if verbose:
         command.append("--verbose")
 
     if disable_usage_stats:
         command.append("--disable-usage-stats")
 
     popen_handle = execute_command_nonblocking(command)
     return popen_handle, server_port
 
+
 def install_mongodb():
     execute_command([sys.executable, "-m", "pip", "install", "pymongo%s" % PYMONGO_VERSION_BOUND])
 
+
 def install_postgres():
     execute_command([sys.executable, "-m", "pip", "install", "psycopg2-binary%s" % PSYCOPG2_VERSION_BOUND])
 
+
 def install_bigquery():
     execute_command([sys.executable, "-m", "pip", "install", "google-cloud-bigquery%s" % BIGQUERY_VERSION_BOUND])
 
+
 def install_snowflake():
     execute_command([sys.executable, "-m", "pip", "install", "snowflake-sqlalchemy%s" % SNOWFLAKE_VERSION_BOUND])
 
+
 def install_s3():
     execute_command([sys.executable, "-m", "pip", "install", "pyarrow%s" % PYARROW_VERSION_BOUND])
 
+
 def install_athena():
     execute_command([sys.executable, "-m", "pip", "install", "awswrangler%s" % AWS_WRANGLER_VERSION_BOUND])
 
+
 def install_mysql():
     system = platform.system()
     if system == "Linux":
         if distro.id() == "ubuntu" or distro.id() == "debian":
             execute_command(
                 [
                     "sudo",
@@ -501,30 +506,34 @@
             )
         elif distro.id() == "centos" or distro.id() == "rhel":
             execute_command(["sudo", "yum", "install", "-y", "python3-devel", "mysql-devel"])
         else:
             print("Unsupported distribution:", distro.id())
     elif system == "Darwin":
         cmd = ["brew", "install", "mysql"]
-        architecture = subprocess.Popen(["which", "-a", "brew"], stdout=subprocess.PIPE ).communicate()[0]
-        if architecture.startswith(b"/opt/homebrew"): # Using arm verison of brew
+        architecture = subprocess.Popen(
+            ["which", "-a", "brew"], stdout=subprocess.PIPE).communicate()[0]
+        # Using arm verison of brew
+        if architecture.startswith(b"/opt/homebrew"):
             cmd = ["arch", "-arm64", *cmd]
         execute_command(cmd)
     else:
         print("Unsupported operating system:", system)
 
-    execute_command([sys.executable, "-m", "pip", "install", "mysqlclient%s" % MYSQL_CLIENT_VERSION_BOUND])
-
+    execute_command(["pip", "install", "PyMySQL"])
+    execute_command([sys.executable, "-m", "pip", "install",
+                    "mysqlclient%s" % MYSQL_CLIENT_VERSION_BOUND])
 
 def install_sqlserver():
     system = platform.system()
     if system == "Linux":
         if distro.id() == "ubuntu":
             execute_command(
-                ["bash", os.path.join(server_directory, "bin", "install_sqlserver_ubuntu.sh")]
+                ["bash", os.path.join(
+                    server_directory, "bin", "install_sqlserver_ubuntu.sh")]
             )
         else:
             print("Unsupported distribution:", distro.id())
     elif system == "Darwin":
         execute_command(
             [
                 "brew",
@@ -543,15 +552,16 @@
                 "msodbcsql17",
                 "mssql-tools",
             ]
         )
     else:
         print("Unsupported operating system:", system)
 
-    execute_command([sys.executable, "-m", "pip", "install", "pyodbc%s" % PYODBC_VERSION_BOUND])
+    execute_command([sys.executable, "-m", "pip", "install",
+                    "pyodbc%s" % PYODBC_VERSION_BOUND])
 
 
 def install(system):
     if system == "postgres" or system == "redshift":
         install_postgres()
     elif system == "bigquery":
         install_bigquery()
@@ -690,17 +700,20 @@
     )
     install_args.add_argument(
         "system",
         nargs=1,
         help="Supported integrations: postgres, redshift, mysql, mariadb, sqlserver, azuresql, s3, athena, snowflake, bigquery.",
     )
 
-    apikey_args = subparsers.add_parser("apikey", help="Display your Aqueduct API key.")
-    clear_args = subparsers.add_parser("clear", help="Erase your Aqueduct installation.")
-    version_args = subparsers.add_parser("version", help="Retrieve the package version number.")
+    apikey_args = subparsers.add_parser(
+        "apikey", help="Display your Aqueduct API key.")
+    clear_args = subparsers.add_parser(
+        "clear", help="Erase your Aqueduct installation.")
+    version_args = subparsers.add_parser(
+        "version", help="Retrieve the package version number.")
 
     storage_args = subparsers.add_parser(
         "storage",
         help="""This changes the storage location for any new workflows created.
                                The change will take affect once you restart the Aqueduct server.
                                We are currently working on adding support for modifying the storage
                                location of existing workflows.
@@ -756,15 +769,16 @@
                 args.disable_usage_stats,
             )
             time.sleep(1)
             terminated = popen_handle.poll()
             if terminated:
                 print("Server terminated due to an error.")
             else:
-                welcome_message, url = generate_welcome_message(addr, server_port)
+                welcome_message, url = generate_welcome_message(
+                    addr, server_port)
                 print(welcome_message)
 
                 if not args.expose:
                     webbrowser.open(url)
                 popen_handle.wait()
         except (Exception, KeyboardInterrupt) as e:
             print(e)
@@ -772,15 +786,16 @@
             popen_handle.kill()
             print("Aqueduct service successfully terminated.")
     elif args.command == "server":
         print(
             "aqueduct ui and aqueduct server have been deprecated; please use aqueduct start to run both the UI and backend servers"
         )
     elif args.command == "install":
-        install(args.system[0])  # argparse makes this an array so only pass in value [0].
+        # argparse makes this an array so only pass in value [0].
+        install(args.system[0])
     elif args.command == "ui":
         print(
             "aqueduct ui and aqueduct server have been deprecated; please use aqueduct start to run both the UI and backend servers"
         )
     elif args.command == "apikey":
         apikey()
     elif args.command == "clear":
```

### Comparing `aqueduct-ml-0.2.9/setup.py` & `aqueduct-ml-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 import os
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
-install_requires = open("requirements.txt").read().strip().split("\n")
+version = open("version").read()
+if not version:
+    raise Exception("Version file must contain a valid version string.")
+
+install_requires = (
+    open("requirements.txt")
+    .read()
+    .strip()
+    .split("\n")
+    .append(
+        # We expect the SDK version always being consistent with executor version
+        f"aqueduct-sdk=={version}"
+    )
+)
 
 readme_path = Path(os.environ["PWD"], "../../README.md")
 long_description = open(readme_path).read()
 
 setup(
     name="aqueduct-ml",
-    version="0.2.9",
+    version=version,
     install_requires=install_requires,
     scripts=["bin/aqueduct"],
     packages=find_packages(),
-    description="Prediction Infrastructure for Data Scientists",
+    description="The control center for ML in the cloud",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.aqueducthq.com/",
     license="Apache License 2.0",
     author="Aqueduct, Inc.",
     author_email="hello@aqueducthq.com",
     classifiers=[
```

