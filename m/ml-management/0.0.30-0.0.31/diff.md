# Comparing `tmp/ml-management-0.0.30.tar.gz` & `tmp/ml-management-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.30.tar", last modified: Tue May  2 17:28:10 2023, max compression
+gzip compressed data, was "ml-management-0.0.31.tar", last modified: Thu May  4 11:23:59 2023, max compression
```

## Comparing `ml-management-0.0.30.tar` & `ml-management-0.0.31.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/
--rw-rw-r--   0 denis     (1000) denis     (1000)       18 2023-04-17 13:42:26.000000 ml-management-0.0.30/MANIFEST.in
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.30/ML_management/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/dataset/
--rw-rw-r--   0 denis     (1000) denis     (1000)      191 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/dataset/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      330 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/dataset/datamodel.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1298 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/dataset/dataset.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/dataset/dummy_dataset/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/dataset/dummy_dataset/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      560 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/dataset/dummy_dataset/dummy_dataset.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/dataset/s3_dataset/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/dataset/s3_dataset/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    10399 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/dataset/s3_dataset/s3dataset.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/executor_template/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.284478 ml-management-0.0.30/ML_management/executor_template/default_executors/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      895 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      843 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      869 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4592 2023-04-28 13:10:54.000000 ml-management-0.0.30/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      401 2023-04-28 11:28:11.000000 ml-management-0.0.30/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      334 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/mlmanagement/
--rw-rw-r--   0 denis     (1000) denis     (1000)      581 2023-04-26 06:58:05.000000 ml-management-0.0.30/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3392 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5054 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    11676 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     9478 2023-05-02 08:26:15.000000 ml-management-0.0.30/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      163 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5001 2023-05-02 11:36:10.000000 ml-management-0.0.30/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      261 2023-04-28 08:12:41.000000 ml-management-0.0.30/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/models/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.30/ML_management/models/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      949 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/models/patterns/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4365 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      561 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      445 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/registry/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.30/ML_management/registry/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2566 2023-04-28 08:49:51.000000 ml-management-0.0.30/ML_management/registry/exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     7556 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ML_management/tests/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/tests/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3361 2023-04-17 13:42:26.000000 ml-management-0.0.30/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     9508 2023-04-28 06:57:33.000000 ml-management-0.0.30/ML_management/tests/test_s3_dataset.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-02 17:28:10.288478 ml-management-0.0.30/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)       56 2022-11-02 13:55:55.000000 ml-management-0.0.30/README.md
--rw-rw-r--   0 denis     (1000) denis     (1000)        7 2023-05-02 17:22:45.000000 ml-management-0.0.30/VERSION
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-02 17:28:10.288478 ml-management-0.0.30/ml_management.egg-info/
--rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)     1938 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)      142 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/requires.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       14 2023-05-02 17:28:10.000000 ml-management-0.0.30/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-05-02 17:28:10.288478 ml-management-0.0.30/setup.cfg
--rw-rw-r--   0 denis     (1000) denis     (1000)     1030 2023-04-28 06:57:33.000000 ml-management-0.0.30/setup.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       18 2023-05-02 14:30:21.000000 ml-management-0.0.31/MANIFEST.in
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/dataset/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      191 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/dataset/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      330 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/dataset/datamodel.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1298 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/dataset/dataset.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/dataset/dummy_dataset/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/dataset/dummy_dataset/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      560 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/dataset/dummy_dataset/dummy_dataset.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/dataset/s3_dataset/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/dataset/s3_dataset/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10399 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/dataset/s3_dataset/s3dataset.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.533529 ml-management-0.0.31/ML_management/executor_template/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      895 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      843 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      869 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4592 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      401 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      334 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/mlmanagement/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      581 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3392 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5054 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    11676 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9511 2023-05-04 09:36:23.000000 ml-management-0.0.31/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      163 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5001 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      261 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/models/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/models/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      949 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/models/patterns/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4365 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      561 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      445 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/registry/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/registry/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2566 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/registry/exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     7556 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ML_management/tests/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/tests/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3361 2023-05-02 14:30:21.000000 ml-management-0.0.31/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9508 2023-05-04 08:40:01.000000 ml-management-0.0.31/ML_management/tests/test_s3_dataset.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-05-04 11:23:59.537529 ml-management-0.0.31/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       56 2023-05-02 14:30:21.000000 ml-management-0.0.31/README.md
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        7 2023-05-04 11:23:57.000000 ml-management-0.0.31/VERSION
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-05-04 11:23:59.537529 ml-management-0.0.31/ml_management.egg-info/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1938 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        1 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      142 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       14 2023-05-04 11:23:59.000000 ml-management-0.0.31/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       38 2023-05-04 11:23:59.537529 ml-management-0.0.31/setup.cfg
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1030 2023-05-04 08:40:01.000000 ml-management-0.0.31/setup.py
```

### Comparing `ml-management-0.0.30/ML_management/dataset/dataset.py` & `ml-management-0.0.31/ML_management/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/dataset/dummy_dataset/dummy_dataset.py` & `ml-management-0.0.31/ML_management/dataset/dummy_dataset/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/dataset/s3_dataset/s3dataset.py` & `ml-management-0.0.31/ML_management/dataset/s3_dataset/s3dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.31/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.31/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.31/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.31/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.31/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.31/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.31/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.31/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.31/ML_management/mlmanagement/mlmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,18 @@
     files = {
         "mlflow_request": json.dumps(mlflow_request),
         "model_zip": ("filename", model_file, "multipart/form-data"),
     }
 
     multipart = MultipartEncoder(fields=files)
     return requests.post(
-        server_ml_api, data=multipart, headers={"Content-Type": multipart.content_type}, auth=(os.getenv("login"), os.getenv("password"))
+        server_ml_api,
+        data=multipart,
+        headers={"Content-Type": multipart.content_type},
+        auth=(os.getenv("login", ""), os.getenv("password", "")),
     )
 
 
 def send_request_to_server(function_name, kwargs, extra_attrs, for_class):
     """
     Send request to server.
```

### Comparing `ml-management-0.0.30/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.31/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.31/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.31/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.31/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/registry/exceptions.py` & `ml-management-0.0.31/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/registry/registry_manager.py` & `ml-management-0.0.31/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.31/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.31/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.31/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.30/setup.py` & `ml-management-0.0.31/setup.py`

 * *Files identical despite different names*

