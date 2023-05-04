# Comparing `tmp/fiddler-client-1.8.0.dev1.tar.gz` & `tmp/fiddler-client-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-1.8.0.dev1.tar", last modified: Thu May  4 20:45:34 2023, max compression
+gzip compressed data, was "fiddler-client-2.0.0.dev1.tar", last modified: Fri Apr 21 22:06:20 2023, max compression
```

## Comparing `fiddler-client-1.8.0.dev1.tar` & `fiddler-client-2.0.0.dev1.tar`

### file list

```diff
@@ -1,117 +1,99 @@
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.991813 fiddler-client-1.8.0.dev1/
--rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1000) docker    (1001)    18969 2023-05-04 20:45:34.991813 fiddler-client-1.8.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)    15485 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/PUBLIC.md
--rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/README.md
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)    32572 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/_version.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    11453 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/api/monitoring.py
--rw-r--r--   0 runner    (1000) docker    (1001)    12356 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/api/publish_event.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/assets/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/assets/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/assets/pg_reserved_words.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6393 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/aws_utils.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5098 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/client.py
--rw-r--r--   0 runner    (1000) docker    (1001)    21425 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/connection.py
--rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)   135418 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/core_objects.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16945 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/experimental.py
--rw-r--r--   0 runner    (1000) docker    (1001)    81387 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/fiddler_api.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/file_processor/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/file_processor/src/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/src/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2024 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/src/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2193 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/src/extractor.py
--rw-r--r--   0 runner    (1000) docker    (1001)      537 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/src/facade.py
--rw-r--r--   0 runner    (1000) docker    (1001)      557 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/src/file_workflow_executor.py
--rw-r--r--   0 runner    (1000) docker    (1001)    11629 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/src/processor.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1754 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/src/utils.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/file_processor/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/tests/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/file_processor/tests/resources/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/tests/resources/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/file_processor/tests/resources/csvs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/tests/resources/csvs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2495 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/tests/test_extractor.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2098 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/tests/test_facade.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5389 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/file_processor/tests/test_file_processor.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/libs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4188 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15196 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6387 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/model_info_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    17870 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/monitoring_validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/packtools/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/packtools/template_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4515 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/project.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)     4352 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3208 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/utils/formatting.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/utils/general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)      775 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/utils/helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/utils/logging.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5806 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/utils/pandas.py
--rw-r--r--   0 runner    (1000) docker    (1001)    18586 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v1_v2_compat.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.987813 fiddler-client-1.8.0.dev1/fiddler/v2/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.991813 fiddler-client-1.8.0.dev1/fiddler/v2/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14039 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/alert_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1892 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5923 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/baseline_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    11539 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/dataset_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14751 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/events_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13480 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/explainability_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4371 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4472 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/job_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/model_artifact_deploy.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3105 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/model_deployment_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14391 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/model_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2664 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/api/project_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1125 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/constants.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.991813 fiddler-client-1.8.0.dev1/fiddler/v2/schema/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4530 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)      462 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2533 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/common.py
--rw-r--r--   0 runner    (1000) docker    (1001)      640 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/events.py
--rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/job.py
--rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1085 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/model_deployment.py
--rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/project.py
--rw-r--r--   0 runner    (1000) docker    (1001)      359 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/server_info.py
--rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/schema/user.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.991813 fiddler-client-1.8.0.dev1/fiddler/v2/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1237 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/utils/decorators.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4127 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1600 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/utils/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2004 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/utils/response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/utils/validations.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.991813 fiddler-client-1.8.0.dev1/fiddler/v2/validators/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/validators/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1527 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/v2/validators/dataset_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13965 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/fiddler/validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.991813 fiddler-client-1.8.0.dev1/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1000) docker    (1001)    18969 2023-05-04 20:45:34.000000 fiddler-client-1.8.0.dev1/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)     2901 2023-05-04 20:45:34.000000 fiddler-client-1.8.0.dev1/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-05-04 20:45:34.000000 fiddler-client-1.8.0.dev1/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker    (1001)      226 2023-05-04 20:45:34.000000 fiddler-client-1.8.0.dev1/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-05-04 20:45:34.000000 fiddler-client-1.8.0.dev1/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-05-04 20:45:34.991813 fiddler-client-1.8.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1000) docker    (1001)     1420 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/setup.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:34.991813 fiddler-client-1.8.0.dev1/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2132 2023-05-04 20:45:29.000000 fiddler-client-1.8.0.dev1/tests/test_fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.535634 fiddler-client-2.0.0.dev1/
+-rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1000) docker    (1001)    19014 2023-04-21 22:06:20.535634 fiddler-client-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)    15514 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/PUBLIC.md
+-rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/README.md
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)    31118 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-04-21 22:06:14.000000 fiddler-client-2.0.0.dev1/fiddler/_version.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    11453 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/api/monitoring.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    12340 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/api/publish_event.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/assets/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/assets/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/assets/pg_reserved_words.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6393 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/aws_utils.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5098 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    21386 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/connection.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/constants.py
+-rw-r--r--   0 runner    (1000) docker    (1001)   134153 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/core_objects.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16945 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/experimental.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    42915 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/libs/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5149 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5056 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7444 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/model_info_validator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    17870 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/monitoring_validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/packtools/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/packtools/template_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1808 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/project.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)     4352 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3208 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/formatting.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      775 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/logging.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5734 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/utils/pandas.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    19454 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v1_v2_compat.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.527634 fiddler-client-2.0.0.dev1/fiddler/v2/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler/v2/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14039 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/alert_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2063 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5923 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/baseline_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16074 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/dataset_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14721 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/events_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15444 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/explainability_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4725 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4472 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/job_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/model_artifact_deploy.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3105 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/model_deployment_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14627 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/model_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2664 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/api/project_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1324 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/constants.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler/v2/schema/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4600 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      462 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5948 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/common.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      640 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/events.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1085 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/model_deployment.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      364 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/server_info.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/schema/user.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler/v2/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1237 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/decorators.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4127 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2283 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2004 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/utils/validations.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler/v2/validators/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/validators/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1527 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/v2/validators/dataset_validator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13965 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/fiddler/validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.531634 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1000) docker    (1001)    19014 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)     2317 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)      217 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-04-21 22:06:20.000000 fiddler-client-2.0.0.dev1/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-04-21 22:06:20.535634 fiddler-client-2.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1000) docker    (1001)     1400 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/setup.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:20.535634 fiddler-client-2.0.0.dev1/tests/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1757 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/tests/test_fiddler_api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3721 2023-04-21 22:06:13.000000 fiddler-client-2.0.0.dev1/tests/test_v1_v2_compat.py
```

### Comparing `fiddler-client-1.8.0.dev1/PKG-INFO` & `fiddler-client-2.0.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 1.8.0.dev1
+Version: 2.0.0.dev1
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -22,33 +22,35 @@
         
         API Example Usage
         -------------
         Documentation for the API can be found [here](https://api.fiddler.ai/#introduction). For examples of interacting with our APIs, please check out our [Quick Start Guide](https://docs.fiddler.ai/quick-start/) as well as the work notebooks found on our [Samples Github](https://github.com/fiddler-labs/fiddler-samples).
         
         Version History
         -------------
-        ### 1.8.0
+        
+        ### 2.0.0
+          - #### **Removed**
+            - Following methods are removed
+              - register_model
+              - upload_model_package
+              - update_model
+              - trigger_pre_computation
+              - _trigger_model_predictions
+              - generate_sample_events
+              - list_teams
+              - list_project_roles
+              - list_org_roles
+              - unshare_project
+              - share_project
+              - process_avro
+              - process_csv
           - #### **Modifications**
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
-            - CURRENT_DATA_TYPE_VERSION increased to v1
-            - removed type conversion of possible_values
-        
-        
-        ### 1.7.3
-          - #### **Modification**
-            - Send row and column count information to dataset upload api
-        
-        ### 1.7.2
-          - #### **Modification**
-            - Bring back `WeightingParams` object
         
-        ### 1.7.1
-          - #### **Modification**
-            - Relaxed boto3 version constraint
         
         ### 1.7.0
           - #### **Removed**
             - Remove support for initializing fiddler client with version=1
             - Following methods are removed
               - get_segment_info
               - delete_segment
@@ -58,27 +60,27 @@
               - upload_segment
               - add_monitoring_config
               - publish_parquet_s3
               - publish_events_log
         
         ### 1.6.2
           - #### **Modifications**
-            - Make dataset_id a required field in add_model()
+            - Made dataset_id a required field in add_model()
             - Update max_inferred_cardinality to 100
           - #### **New Features**
             - New method for updating a model artifact `update_model_artifact`
         
         ### 1.5.3
           - #### **Modifications**
             - Fix add_model_artifact error for NLP models
             - Add model_info validation during add_model
         
         ### 1.5.2
           - #### **Modifications**
-            - Adds fix for self signed certificate not working by adding verify param to FiddlerApi
+            - Add fix for self signed certificate not working by adding verify param to FiddlerApi
         
         ### 1.5.1
           - #### **Modifications**
             - Fix in `violation_of_type` to include numpy dtypes such as `int64`
         
         ### 1.5.0
           - #### **New Features**
```

### Comparing `fiddler-client-1.8.0.dev1/PUBLIC.md` & `fiddler-client-2.0.0.dev1/PUBLIC.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,33 +15,35 @@
 
 API Example Usage
 -------------
 Documentation for the API can be found [here](https://api.fiddler.ai/#introduction). For examples of interacting with our APIs, please check out our [Quick Start Guide](https://docs.fiddler.ai/quick-start/) as well as the work notebooks found on our [Samples Github](https://github.com/fiddler-labs/fiddler-samples).
 
 Version History
 -------------
-### 1.8.0
+
+### 2.0.0
+  - #### **Removed**
+    - Following methods are removed
+      - register_model
+      - upload_model_package
+      - update_model
+      - trigger_pre_computation
+      - _trigger_model_predictions
+      - generate_sample_events
+      - list_teams
+      - list_project_roles
+      - list_org_roles
+      - unshare_project
+      - share_project
+      - process_avro
+      - process_csv
   - #### **Modifications**
     - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
       `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
-    - CURRENT_DATA_TYPE_VERSION increased to v1
-    - removed type conversion of possible_values
-
-
-### 1.7.3
-  - #### **Modification**
-    - Send row and column count information to dataset upload api
-
-### 1.7.2
-  - #### **Modification**
-    - Bring back `WeightingParams` object
 
-### 1.7.1
-  - #### **Modification**
-    - Relaxed boto3 version constraint
 
 ### 1.7.0
   - #### **Removed**
     - Remove support for initializing fiddler client with version=1
     - Following methods are removed
       - get_segment_info
       - delete_segment
@@ -51,27 +53,27 @@
       - upload_segment
       - add_monitoring_config
       - publish_parquet_s3
       - publish_events_log
 
 ### 1.6.2
   - #### **Modifications**
-    - Make dataset_id a required field in add_model()
+    - Made dataset_id a required field in add_model()
     - Update max_inferred_cardinality to 100
   - #### **New Features**
     - New method for updating a model artifact `update_model_artifact`
 
 ### 1.5.3
   - #### **Modifications**
     - Fix add_model_artifact error for NLP models
     - Add model_info validation during add_model
 
 ### 1.5.2
   - #### **Modifications**
-    - Adds fix for self signed certificate not working by adding verify param to FiddlerApi
+    - Add fix for self signed certificate not working by adding verify param to FiddlerApi
 
 ### 1.5.1
   - #### **Modifications**
     - Fix in `violation_of_type` to include numpy dtypes such as `int64`
 
 ### 1.5.0
   - #### **New Features**
```

### Comparing `fiddler-client-1.8.0.dev1/README.md` & `fiddler-client-2.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/__init__.py` & `fiddler-client-2.0.0.dev1/fiddler/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 
 A Python client for Fiddler service.
 
 TODO: Add Licence.
 """
 import configparser
 import functools
+import warnings
 from collections import namedtuple
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, NamedTuple, Optional, Tuple, Union
 
 import pandas as pd
+from requests.exceptions import HTTPError
 
 from fiddler.api.monitoring import Monitoring
-from fiddler.project import Project
 from fiddler.v2.schema.alert import (
     AlertCondition,
     AlertType,
     BinSize,
     ComparePeriod,
     CompareTo,
     Metric,
@@ -43,39 +44,38 @@
     FiddlerPublishSchema,
     FiddlerTimestamp,
     MLFlowParams,
     ModelDeploymentParams,
     ModelInfo,
     ModelInputType,
     ModelTask,
-    WeightingParams,
     WindowSize,
 )
 from .fiddler_api import FiddlerApi as FiddlerApiV1
-from .file_processor.src.constants import (
-    CSV_EXTENSION,
-    PARQUET_COMPRESSION,
-    PARQUET_ENGINE,
-    PARQUET_EXTENSION,
-    PARQUET_ROW_GROUP_SIZE,
-)
 from .packtools import gem
 from .utils import ColorLogger
 from .v1_v2_compat import V1V2Compat
 from .v2.api.api import Client as FiddlerApiV2
 from .v2.api.explainability_mixin import (
     DatasetDataSource,
     RowDataSource,
     SqlSliceQueryDataSource,
 )
-from .v2.constants import ServerDeploymentMode
+from .v2.constants import (
+    CSV_EXTENSION,
+    PARQUET_COMPRESSION,
+    PARQUET_ENGINE,
+    PARQUET_EXTENSION,
+    PARQUET_ROW_GROUP_SIZE,
+    FileType,
+)
 from .v2.schema.job import JobStatus
 from .v2.schema.model_deployment import DeploymentParams, ModelDeployment
-from .v2.schema.server_info import ServerInfo
-from .v2.utils.helpers import match_semvar
+from .v2.utils.exceptions import NotSupported
+from .v2.utils.helpers import match_semvar, raise_not_support
 from .validator import PackageValidator, ValidationChainSettings, ValidationModule
 
 logger = utils.logging.getLogger(__name__)
 
 VERSIONS = [2]
 
 
@@ -106,15 +106,15 @@
         proxies: Optional[dict] = None,
         verbose: Optional[bool] = False,
         timeout: int = 1200,  # sec
         version: int = 2,
         verify: bool = True,
     ):
         url, org_id, auth_token = cls._get_connection_parameters(
-            cls, url, org_id, auth_token, version
+            url, org_id, auth_token, version
         )
 
         # Validation of version, org_id is handled by FiddlerApiV1.
         client_v1 = FiddlerApiV1(
             url=url,
             org_id=org_id,
             auth_token=auth_token,
@@ -127,25 +127,24 @@
         client_v2 = FiddlerApiV2(
             url=url,
             organization_name=org_id,
             auth_token=auth_token,
             timeout=timeout,
             verify=verify,
         )
-        supported_features = cls._get_supported_features(cls, client_v1, org_id)
-
-        # Setting server_info explicitly since /get_supported_features is not available
-        # in F2 construct
-        client_v2.server_info = cls._get_server_info(cls, supported_features)
-
-        server_deployment_mode = cls._get_server_deployment_mode(
-            cls, supported_features
-        )
 
-        logger.info(f'Version deployed on the server side {server_deployment_mode}')
+        if match_semvar(
+            client_v2.server_info.server_version,
+            '<22.12.0',
+        ):
+            raise_not_support(
+                compatible_client_version='1.7',
+                client_version=__version__,
+                server_version=client_v2.server_info.server_version,
+            )
 
         compat_client = V1V2Compat(client_v2)
 
         obj = lambda: None  # instantiate an empty object # noqa
 
         obj.list_datasets = compat_client.get_datasets
         obj.get_dataset_info = compat_client.get_dataset_info
@@ -158,61 +157,38 @@
 
         obj.list_models = compat_client.get_models
         obj.get_model_info = compat_client.get_model_info
 
         obj.upload_dataset = (
             compat_client.upload_dataset_dataframe
         )  # this is uploading dataframe in v1 and csv in v2
-        obj.upload_dataset_from_file = (
-            compat_client.upload_dataset
+        obj.upload_dataset_from_file = functools.partial(
+            _upload_dataset_from_file, client_v2
         )  # currently only supports csv
         obj.upload_dataset_from_dir = compat_client.upload_dataset_from_dir
-        # obj.process_csv = client_v1.process_csv
-        # obj.process_avro = client_v1.process_avro
 
         obj.publish_event = compat_client.publish_event
         obj.publish_events_batch = compat_client.publish_events_batch
         obj.publish_events_batch_schema = compat_client.publish_events_batch_schema
-        obj.generate_sample_events = client_v1.generate_sample_events
-
-        obj.upload_model_package = functools.partial(
-            functools.partial(v1_upload_model_package, v1_client=client_v1),
-            v2_client=client_v2,
-        )
-        obj.upload_model_package.__doc__ = client_v1.upload_model_package.__doc__
-
-        obj.trigger_pre_computation = client_v1.trigger_pre_computation
-
-        obj.register_model = functools.partial(
-            functools.partial(v1_register_model, v1_client=client_v1),
-            v2_client=client_v2,
-        )
-        obj.register_model.__doc__ = client_v1.register_model.__doc__
-
-        obj.update_model = client_v1.update_model
 
         obj.add_model = functools.partial(
             functools.partial(add_model, v1_client=client_v1),
             v2_client=client_v2,
         )
         obj.add_model.__doc__ = add_model.__doc__
 
-        obj.add_model_surrogate = functools.partial(
-            _add_model_surrogate, client_v1, client_v2
-        )
+        obj.add_model_surrogate = functools.partial(_add_model_surrogate, client_v2)
         obj.add_model_surrogate.__doc__ = _add_model_surrogate.__doc__
 
         obj.update_model_surrogate = functools.partial(
             _update_model_surrogate, client_v2
         )
         obj.update_model_surrogate.__doc__ = _update_model_surrogate.__doc__
 
-        obj.add_model_artifact = functools.partial(
-            _add_model_artifact, client_v1, client_v2
-        )
+        obj.add_model_artifact = functools.partial(_add_model_artifact, client_v2)
         obj.add_model_artifact.__doc__ = _add_model_artifact.__doc__
 
         obj.delete_model = functools.partial(_delete_model, client_v1, client_v2)
         obj.delete_model.__doc__ = client_v1.delete_model.__doc__
 
         obj.update_model_artifact = functools.partial(_update_model_artifact, client_v2)
         obj.update_model_artifact.__doc__ = _update_model_artifact.__doc__
@@ -221,84 +197,78 @@
         obj.get_model_deployment.__doc__ = _get_model_deployment.__doc__
 
         obj.update_model_deployment = functools.partial(
             _update_model_deployment, client_v2
         )
         obj.update_model_deployment.__doc__ = _update_model_deployment.__doc__
 
-        obj._trigger_model_predictions = client_v1._trigger_model_predictions
+        # Explainability apis
+
+        # Feature impact / importance
+        obj.run_feature_importance = functools.partial(
+            _get_feature_importance, client_v2
+        )
+        obj.run_feature_importance.__doc__ = client_v1.run_feature_importance.__doc__
+
+        # Explain
+        obj.run_explanation = functools.partial(_get_explanation, client_v2)
+        obj.run_explanation.__doc__ = client_v1.run_explanation.__doc__
+
+        # Fairness
+        obj.run_fairness = functools.partial(_get_fairness, client_v2)
+        obj.run_fairness.__doc__ = client_v1.run_fairness.__doc__
+
+        # Slice query
+        obj.get_slice = functools.partial(_run_slice_query, client_v2)
+        obj.get_slice.__doc__ = client_v1.get_slice.__doc__
+
+        # Predictions
+        obj.run_model = functools.partial(_get_predictions, client_v2)
+        obj.run_model.__doc__ = client_v1.run_model.__doc__
 
         if match_semvar(
             client_v2.server_info.server_version,
-            client_v2.EXPLAINABILITY_SERVER_VERSION,
+            '>=23.2.0',
         ):
-            # Explainability apis are available only after 22.12.0
-
-            # Feature impact / importance
-            obj.run_feature_importance = functools.partial(
-                _get_feature_importance, client_v2
+            obj.get_mutual_information = functools.partial(
+                _get_mutual_information, client_v2
             )
-            obj.run_feature_importance.__doc__ = (
-                client_v1.run_feature_importance.__doc__
+            obj.get_mutual_information.__doc__ = (
+                client_v1.get_mutual_information.__doc__
             )
-
-            # Explain
-            obj.run_explanation = functools.partial(_get_explanation, client_v2)
-            obj.run_explanation.__doc__ = client_v1.run_explanation.__doc__
-
-            # Fairness
-            obj.run_fairness = functools.partial(_get_fairness, client_v2)
-            obj.run_fairness.__doc__ = client_v1.run_fairness.__doc__
-
-            # Slice query
-            obj.get_slice = functools.partial(_run_slice_query, client_v2)
-            obj.get_slice.__doc__ = client_v1.get_slice.__doc__
-
-            # Predictions
-            obj.run_model = functools.partial(_get_predictions, client_v2)
-            obj.run_model.__doc__ = client_v1.run_model.__doc__
         else:
-            obj.run_feature_importance = client_v1.run_feature_importance
-            obj.run_explanation = client_v1.run_explanation
-            obj.run_fairness = client_v1.run_fairness
-            obj.get_slice = client_v1.get_slice
-            obj.run_model = client_v1.run_model
+            obj.get_mutual_information = client_v1.get_mutual_information
 
         # explicitly binding non-conflicting v1 methods to the v2 obj
         # conflicting methods will use v2 method by default for this condition
         # obj.project = client_v1.project
 
-        obj.get_mutual_information = client_v1.get_mutual_information
-
         # Alerts
         obj.get_alert_rules = client_v2.get_alert_rules
         obj.get_triggered_alerts = client_v2.get_triggered_alerts
         obj.add_alert_rule = client_v2.add_alert_rule
         obj.delete_alert_rule = client_v2.delete_alert_rule
         obj.build_notifications_config = client_v2.build_notifications_config
 
         # Baseline handling
         obj.add_baseline = client_v2.add_baseline
         obj.get_baseline = client_v2.get_baseline
         obj.list_baselines = client_v2.list_baselines
         obj.delete_baseline = client_v2.delete_baseline
 
-        # The below methods are not used so not mapping them.
-        # obj.share_project = client_v1.share_project
-        # obj.unshare_project = client_v1.unshare_project
-        # obj.list_org_roles = client_v1.list_org_roles
-        # obj.list_project_roles = client_v1.list_project_roles
-        # obj.list_teams = client_v1.list_teams
+        # Infer DatasetInfo using infer-data-type API
+        obj.infer_dataset_info = client_v2.infer_dataset_info
 
         obj.v1 = client_v1
         obj.v2 = client_v2
         return obj
 
+    @staticmethod
     def _get_connection_parameters(
-        self, url: str, org_id: str, auth_token: str, version: int
+        url: str, org_id: str, auth_token: str, version: int
     ) -> Tuple:
         if Path('fiddler.ini').is_file():
             config = configparser.ConfigParser()
             config.read('fiddler.ini')
             info = config['FIDDLER']
             if not url:
                 url = info.get('url', None)
@@ -319,98 +289,39 @@
             raise ValueError(
                 f'version={version} not supported. Please enter a valid version. '
                 f'Supported versions={VERSIONS}'
             )
 
         return url, org_id, auth_token
 
-    def _get_supported_features(self, client_v1: FiddlerApiV1, org_id: str) -> Dict:
-        path: List['str'] = ['get_supported_features', org_id]
-        return client_v1.connection.call(path, is_get_request=True)
-
-    def _get_server_info(self, supported_features: Dict) -> ServerInfo:
-        # @TODO refactor this once /get_supported_features is available as F2 endpoint
-
-        server_info_dict = {
-            'features': supported_features.get('features'),
-            'server_version': supported_features.get('server_version'),
-        }
-
-        return ServerInfo(**server_info_dict)
-
-    def _get_server_deployment_mode(
-        self, supported_features: Dict
-    ) -> ServerDeploymentMode:
-
-        if supported_features.get('enable_fiddler_v2', False):
-            return ServerDeploymentMode.F2
-
-        return ServerDeploymentMode.F1
-
 
-def v1_upload_model_package(
-    artifact_path: Path,
-    project_id: str,
-    model_id: str,
-    deployment_type: Optional[str] = DeploymentType.PREDICTOR,
-    # model deployment type. One of {'predictor', 'executor'}
-    image_uri: Optional[str] = None,  # image to be used for newly uploaded model
-    namespace: Optional[str] = None,  # kubernetes namespace
-    port: Optional[int] = 5100,  # port on which model is served
-    replicas: Optional[int] = 1,  # number of replicas
-    cpus: Optional[float] = 0.25,  # number of CPU cores
-    memory: Optional[str] = '128m',  # amount of memory required.
-    gpus: Optional[int] = 0,  # number of GPU cores
-    await_deployment: Optional[bool] = True,  # wait for deployment
-    is_sync=True,
-    v2_client: FiddlerApiV2 = None,
-    v1_client: FiddlerApiV1 = None,
-):
-    v1_client.upload_model_package(
-        artifact_path,
-        project_id,
-        model_id,
-        deployment_type,
-        image_uri,
-        namespace,
-        port,
-        replicas,
-        cpus,
-        memory,
-        gpus,
-        await_deployment,
-    )
-
-    call_init_monitoring(v1_client, v2_client, project_id, model_id, is_sync)
-
-
-def v1_register_model(
+def _upload_dataset_from_file(
+    client_v2: FiddlerApiV2,
     project_id: str,
-    model_id: str,
     dataset_id: str,
-    model_info: ModelInfo,
-    deployment: Optional[DeploymentOptions] = None,
-    cache_global_impact_importance: bool = True,
-    cache_global_pdps: bool = False,
-    cache_dataset: bool = True,
-    is_sync=True,
-    v2_client: FiddlerApiV2 = None,
-    v1_client: FiddlerApiV1 = None,
-):
-    v1_client.register_model(
-        project_id,
-        model_id,
-        dataset_id,
-        model_info,
-        deployment,
-        cache_global_impact_importance,
-        cache_global_pdps,
-        cache_dataset,
+    file_path: str,
+    file_type: str = 'csv',
+    file_schema=Dict[str, Any],
+    info: Optional[DatasetInfo] = None,
+    size_check_enabled: bool = False,
+) -> Dict[str, str]:
+    if file_type.endswith('csv'):
+        return client_v2.upload_dataset(
+            project_name=project_id,
+            dataset_name=dataset_id,
+            files={Path(file_path).name: Path(file_path)},
+            info=info,
+            file_type=FileType.CSV,
+            file_schema=None,
+            is_sync=True,
+        )
+
+    raise ValueError(
+        f'Invalid file_type :{file_type}. CSV is the only valid file type.'
     )
-    call_init_monitoring(v1_client, v2_client, project_id, model_id, is_sync)
 
 
 def add_model(
     project_id: str,
     model_id: str,
     dataset_id: str,
     model_info: ModelInfo,
@@ -428,14 +339,21 @@
     :param dataset_id: name of the dataset
     :type dataset_id: string
     :param model_info: model related information from user
     :type model_info: ModelInfo
     :param is_sync: perform add model synchronously
     :type is_sync: boolean
     """
+
+    if not isinstance(model_info, ModelInfo):
+        raise ValueError(
+            f'The value passed to the model_info parameter must be a ModelInfo object.'
+            f'Instead, found value of type {type(model_info)}'
+        )
+
     outputs = model_info.get_output_names()
     dataset = v2_client.get_dataset(project_name=project_id, dataset_name=dataset_id)
     dataset_cols = set([col.name for col in dataset.info.columns])
 
     # @TODO: FDL-9002: Move output column validation to BE's ModelInfoValidator
     if not all(elem in dataset_cols for elem in outputs):
         raise ValueError(f'Dataset {dataset_id} does not have output columns')
@@ -448,15 +366,14 @@
         model_name=model_id, project_name=project_id, info=model_info
     )
     call_init_monitoring(v1_client, v2_client, project_id, model_id, is_sync)
     logger.info(f'Successfully added model {model.name} to project {project_id}')
 
 
 def _add_model_surrogate(
-    client_v1: FiddlerApiV1,
     client_v2: FiddlerApiV2,
     project_id: str,
     model_id: str,
     deployment_params: Optional[DeploymentParams] = None,
 ) -> None:
     """
     Trigger generation of surrogate model
@@ -464,42 +381,22 @@
     :param project_id: project name where the model will be added
     :type project_id: string
     :param model_id: name of the model
     :type model_id: string
     :param deployment_params: Model deployment parameters
     :type deployment_params: DeploymentParams
     """
-    if match_semvar(
-        client_v2.server_info.server_version, client_v2.ADD_SURROGATE_MODEL_API_VERSION
-    ):
-        client_v2.add_model_surrogate(
-            model_name=model_id,
-            project_name=project_id,
-            deployment_params=deployment_params,
-        )
-        return
-
-    model_info = Project(client_v1.connection, project_id).model(model_id).get_info()
-
-    if (
-        model_info.artifact_status
-        and model_info.artifact_status.value != ArtifactStatus.NO_MODEL.value
-    ):
-        raise ValueError(
-            f'Model {model_id} in project {project_id} already has artifact associated '
-            f'with it'
-        )
-
-    dataset_name = model_info.datasets[0]
-    model_info.artifact_status = ArtifactStatus.SURROGATE
-    client_v1.register_model(project_id, model_id, dataset_name, model_info)
+    client_v2.add_model_surrogate(
+        model_name=model_id,
+        project_name=project_id,
+        deployment_params=deployment_params,
+    )
 
 
 def _add_model_artifact(
-    client_v1: FiddlerApiV1,
     client_v2: FiddlerApiV2,
     project_id: str,
     model_id: str,
     model_dir: str,
     deployment_params: Optional[DeploymentParams] = None,
 ) -> None:
     """
@@ -513,53 +410,37 @@
     :param model_id: model id
     :type model_id: string
     :param model_dir: model directory
     :type model_dir: string
     :param deployment_params: Model deployment parameters
     :type deployment_params: DeploymentParams
     """
-    if match_semvar(
-        client_v2.server_info.server_version, client_v2.ADD_MODEL_ARTIFACT_API_VERSION
-    ):
-        client_v2.add_model_artifact(
-            model_name=model_id,
-            project_name=project_id,
-            artifact_dir=model_dir,
-            deployment_params=deployment_params,
-        )
-        return
-
-    client_v1.update_model(
-        project_id=project_id,
-        model_id=model_id,
-        model_dir=model_dir,
-        force_pre_compute=True,
+    client_v2.add_model_artifact(
+        model_name=model_id,
+        project_name=project_id,
+        artifact_dir=model_dir,
+        deployment_params=deployment_params,
     )
 
 
 def _delete_model(
-    client_v1: FiddlerApiV1,
     client_v2: FiddlerApiV2,
     project_id: str,
     model_id: str,
     delete_prod=True,
     delete_pred=True,
 ) -> None:
-    if match_semvar(
-        client_v2.server_info.server_version, client_v2.DELETE_MODEL_API_VERSION
-    ):
+    try:
         client_v2.delete_model(model_name=model_id, project_name=project_id)
-        return
-
-    client_v1.delete_model(
-        project_id=project_id,
-        model_id=model_id,
-        delete_prod=delete_prod,
-        delete_pred=delete_pred,
-    )
+    except HTTPError as err:
+        if err.response.status_code == 404:
+            logger.warning(f'Model {model_id} in project {project_id} does not exist')
+        else:
+            raise err
+    return
 
 
 def call_init_monitoring(
     v1_client: FiddlerApiV1,
     v2_client: FiddlerApiV2,
     project_id: str,
     model_id: str,
@@ -712,24 +593,43 @@
     dataset_id: Optional[str] = None,
     n_permutation: Optional[int] = None,
     n_background: Optional[int] = None,
     casting_type: Optional[bool] = False,
     return_raw_response=False,
     **kwargs,
 ) -> Any:
+
     if not isinstance(explanations, (str, list)):
         raise ValueError(
             'explanation can only be a string or a list of a single element'
         )
 
     if isinstance(explanations, list):
         if len(explanations) != 1:
             raise NotImplementedError('Only one explanation method can be used.')
         explanations = explanations[0]
 
+    if explanations == 'ig':
+        message = (
+            "Method named 'ig' is deprecated. " "Running instead with method named 'IG'"
+        )
+        warnings.warn(message, DeprecationWarning)
+
+    if not isinstance(df, pd.DataFrame):
+        raise ValueError(
+            f'Argument df should be a pandas DataFrame, not of type {type(df)}'
+        )
+    if df.shape[0] > 1:
+        raise NotSupported(
+            f"Currently, only single point explanation is implemented. You can't call "
+            f'this method with {df.shape[0]} rows in the dataframe.'
+        )
+    if df.shape[0] == 0:
+        raise ValueError('df is empty. Please provide a valid dataframe.')
+
     # Transform old explanation names to new ones:
     new_explanation_names = {
         'shap': 'SHAP',
         'fiddler_shapley_values': 'FIDDLER_SHAP',
         'ig_flex': 'IG',
         'permute': 'PERMUTE',
         'mean_reset': 'MEAN_RESET',
@@ -749,14 +649,17 @@
         'ci_level': kwargs.get('ci_level'),
         'top_n_class': kwargs.get('top_n_class', None),
         'input_data_source': RowDataSource(row=df.to_dict(orient='records')[0]),
     }
 
     model_info = client_v2.get_model(project_name=project_id, model_name=model_id).info
 
+    if dataset_id is None:
+        dataset_id = model_info['datasets'][0]
+
     if (explanations in ['SHAP', 'FIDDLER_SHAP', 'PERMUTE', 'MEAN_RESET']) and (
         model_info['input-type'] != ModelInputType.TEXT.value
     ):
         # Only for non text inputs and some explanation methods
         # we need the reference dataset
         fn_kwargs['ref_data_source'] = DatasetDataSource(
             dataset_name=dataset_id, source=None, num_samples=n_background
@@ -764,15 +667,15 @@
 
     explanation = client_v2.get_explanation(**fn_kwargs)
     response = explanation._asdict()  # noqa
 
     if return_raw_response:
         return response
 
-    if len(response.keys()) == 1:
+    if len(response['explanations'].keys()) == 1:
         return namedtuple('AttributionExplanation', response)(**response)
 
     return namedtuple('MulticlassAttributionExplanation', response)(**response)
 
 
 def _get_fairness(
     client_v2: FiddlerApiV2,
@@ -949,14 +852,76 @@
         model_name=model_id,
         project_name=project_id,
         deployment_params=deployment_params,
         wait=wait,
     )
 
 
+def _get_mutual_information(
+    client_v2: FiddlerApiV2,
+    project_id: str,
+    dataset_id: str,
+    features: List[str],
+    normalized: Optional[bool] = False,
+    slice_query: Optional[str] = None,
+    sample_size: Optional[int] = None,
+    seed: Optional[float] = None,
+) -> Dict[str, Dict[str, float]]:
+    """
+    The Mutual information measures the dependency between two random variables.
+    It's a non-negative value. If two random variables are independent MI is
+    equal to zero. Higher MI values means higher dependency.
+
+    :param project_id: The unique identifier of the model's project on the
+        Fiddler engine.
+    :param dataset_id: The unique identifier of the dataset in the
+        Fiddler engine.
+    :param features: list of features to compute mutual information with respect to
+           all the variables in the dataset.
+    :param normalized: If set to True, it will compute Normalized Mutual Information
+    :param slice_query: Optional slice query
+    :param sample_size: Optional sample size for the selected dataset
+    :param seed: Optional seed for sampling
+    :return: a dictionary of mutual information w.r.t the given features.
+    """
+    if seed:
+        message = 'Argument seed is now deprecated, ignoring it.'
+        warnings.warn(message, DeprecationWarning)
+
+    if not slice_query:
+        slice_query = f'SELECT * FROM {dataset_id}'
+
+    if isinstance(features, list):
+        message = (
+            'Argument features will soon support a single column to compute '
+            'mutual information on.'
+        )
+        warnings.warn(message, DeprecationWarning)
+
+    if isinstance(features, str):
+        features = [features]
+
+    if not isinstance(features, list):
+        raise ValueError(f'Invalid type: {type(features)} for the argument features.')
+
+    # Compatibility layer
+    response = {}
+    for column_name in features:
+        response[column_name] = client_v2.get_mutual_information(
+            project_name=project_id,
+            dataset_name=dataset_id,
+            query=slice_query,
+            column_names=features,
+            normalized=normalized,
+            num_samples=sample_size,
+        )
+
+    return response
+
+
 __all__ = [
     '__version__',
     'BatchPublishType',
     'Column',
     'CustomFeature',
     'ColorLogger',
     'DatasetInfo',
@@ -967,15 +932,14 @@
     'FiddlerPublishSchema',
     'gem',
     'MLFlowParams',
     'ModelDeploymentParams',
     'ModelInfo',
     'ModelInputType',
     'ModelTask',
-    'WeightingParams',
     'ExplanationMethod',
     'PredictionEventBundle',
     'PackageValidator',
     'ValidationChainSettings',
     'ValidationModule',
     'utils',
     # Exposing constants
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/api/monitoring.py` & `fiddler-client-2.0.0.dev1/fiddler/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/api/publish_event.py` & `fiddler-client-2.0.0.dev1/fiddler/api/publish_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
 
 from fiddler.connection import Connection
-from fiddler.file_processor.src.constants import PARQUET_EXTENSION
+from fiddler.v2.constants import PARQUET_EXTENSION
 
 from ..aws_utils import validate_gcp_uri_access, validate_s3_uri_access
 from ..core_objects import BatchPublishType, FiddlerTimestamp
 from ..utils.formatting import formatted_utcnow, print_streamed_result
 from ..utils.helper import infer_data_source
 from ..utils.pandas import clean_df_types, write_dataframe_to_parquet_file
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/assets/pg_reserved_words.py` & `fiddler-client-2.0.0.dev1/fiddler/assets/pg_reserved_words.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/aws_utils.py` & `fiddler-client-2.0.0.dev1/fiddler/aws_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/client.py` & `fiddler-client-2.0.0.dev1/fiddler/client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/connection.py` & `fiddler-client-2.0.0.dev1/fiddler/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,14 @@
             'executor',
             'explain',
             'explain_by_row_id',
             'fairness',
             'feature_importance',
             'generate',
             'new_project',
-            'trigger_pre_computation',
             'precache_globals',
         )
         if path_base in executor_service_bases:
             return {Connection.ROUTING_HEADER_KEY: 'executor_service'}
         else:
             return {Connection.ROUTING_HEADER_KEY: 'data_service'}
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/core_objects.py` & `fiddler-client-2.0.0.dev1/fiddler/core_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,15 @@
 # default for DatasetInfo.data_type_version and ModelInfo.data_type_version
 # Introduced to bypass certain data type conversion functions
 # from both client and server.
 # More details https://fiddlerlabs.atlassian.net/wiki/spaces/FL/pages/1973617158/Introducing+Version+in+DatasetInfo+and+ModelInfo
 
 # v0 means variable is just defined, no change in any logic.
 # v0 is launched in python-client release 1.7.0
-
-# v1 ignores typecasting of possible_values of categorical data type
-# v1 is launched in python-client release 1.8.0
-CURRENT_DATA_TYPE_VERSION: str = 'v1'
+CURRENT_DATA_TYPE_VERSION: str = 'v0'
 
 LOG = logging.getLogger(__name__)
 
 
 class IntegrityViolationStatus(NamedTuple):
     is_nullable_violation: bool
     is_type_violation: bool
@@ -433,24 +430,27 @@
     """A class used to define custom features such as complex/vector features
 
     :param name: The name of the custom feature as it will appear in the monitoring tab.
     :param columns: The name of the data column(s) that constitute the custom feature.
     :param transformation: The transformation method applied on the original data.
     :param n_clusters: The number of clusters used for creating clustering-based histograms.
                        If not specified a preprocessing step will run to choose the number of clusters automatically.
-    :param monitor: A boolean variable that specifies whether this custom feature will be monitored using the
-                            clustering-based histogram binning.
+    :param monitor: A boolean variable that specifies whether this custom feature will
+        be monitored using the clustering-based histogram binning.
+    :param monitor_components: A boolean variable that specifies whether each individual
+        component of this custom feature will be monitored. Default to False
     """
 
     name: str
     columns: Union[str, List[str]]
     type: CustomFeatureType
     transformation: Optional[str] = None
     n_clusters: Optional[int] = None
     monitor: bool = True
+    monitor_components: bool = False
 
     def __post_init__(self):
         if self.n_clusters is not None and not isinstance(self.n_clusters, int):
             raise TypeError(
                 f'n_clusters argument must be of type int but received {type(self.n_clusters)}.'
             )
 
@@ -459,46 +459,50 @@
         res = {
             'name': self.name,
             'columns': self.columns,
             'type': self.type.value,
             'transformation': self.transformation,
             'n_clusters': self.n_clusters,
             'monitor': self.monitor,
+            'monitor_components': getattr(self, 'monitor_components', False),
         }
         return res
 
     @classmethod
     def from_dict(cls, desrialized_json: dict):
         """Creates a CustomFeature object from deserialized JSON"""
-
         return cls(
             name=desrialized_json['name'],
             columns=desrialized_json['columns'],
             type=CustomFeatureType(desrialized_json['type']),
             transformation=desrialized_json['transformation'],
             n_clusters=desrialized_json['n_clusters'],
             monitor=desrialized_json['monitor'],
+            monitor_components=bool(desrialized_json.get('monitor_components', False)),
         )
 
     @classmethod
     def from_columns(
         cls,
         cols: List[str],
         custom_name: str,
         transformation: Optional[str] = None,
         n_clusters: Optional[int] = None,
         monitor: bool = True,
+        monitor_components: bool = False,
     ):
         """Creates a custom feature from multiple numerical columns.
         :param cols: A list of column names that define this custom feature.
         :param custom_name: The name of this custom feature as it will appear in the monitoring tab.
         :param transformation: [Optional] An optional transformation step (eg, dimensionality reduction via SVD).
         :param n_clusters: [Optional] Number of clusters for clustering-based monitoring.
         :param monitor:A boolean variable that specifies whether this custom feature will be monitored using the
                             clustering-based histogram binning.
+        :param monitor_components: A boolean variable that specifies whether each
+        individual component of this custom feature will be monitored. Default to False
         """
         if not isinstance(custom_name, str):
             raise TypeError(
                 f'custom_name argument must be of type str but received {type(custom_name)}'
             )
 
         if not (isinstance(cols, list) and all(isinstance(col, str) for col in cols)):
@@ -519,24 +523,26 @@
         return cls(
             name=custom_name,
             columns=cols,
             type=CustomFeatureType.FROM_COLUMNS,
             transformation=transformation,
             n_clusters=n_clusters,
             monitor=monitor,
+            monitor_components=monitor_components,
         )
 
     # ToDo: This class method will be added later. For the first version we only use from_columns constructor
     # @classmethod
     # def from_text(cls,
     #               text_col: str,
     #               transformation: str,
     #               custom_name: Optional[str] = None,
     #               n_clusters: Optional[int] = None,
     #               monitor: bool = True,
+    #               monitor_components = False,
     #               ):
     #     """Creates a custom feature from a single text column.
     #     :param text_col: The name of the dataset column that contains text data.
     #     :param transformation: The transformation used to convert text data to numerical vectors.
     #     :param custom_name: [Optional] A new name assigned to this custom feature. If not specified, the name of the text column will be used.
     #     :param n_clusters: [Optional] Number of clusters for clustering-based monitoring.
     #     :param monitor:A boolean variable that specifies whether this custom feature will be monitored using the
@@ -550,15 +556,16 @@
     #
     #     custom_feature_name = custom_name if custom_name else text_col
     #     return cls(name=custom_feature_name,
     #                columns=text_col,
     #                type=CustomFeatureType.FROM_TEXT,
     #                transformation=transformation,
     #                n_clusters=n_clusters,
-    #                monitor=monitor)
+    #                monitor=monitor,
+    #                monitor_components=monitor_components)
 
 
 class Column:
     """Represents a single column of a dataset or model input/output.
 
     :param name: The name of the column (corresponds to the header row of a
         CSV file)
@@ -839,24 +846,14 @@
         self.display_name = display_name
         self.dataset_id = dataset_id
         self.columns = DatasetInfo._datatype_check(columns)
         self.files = files if files is not None else list()
         self.data_type_version = data_type_version
         self.misc = kwargs
 
-    def to_dict(self) -> Dict[str, Any]:
-        """Converts this object to a more JSON-friendly form."""
-        res = {
-            'name': self.display_name,
-            'data_type_version': self.data_type_version,
-            'columns': [c.to_dict() for c in self.columns],
-            'files': self.files,
-        }
-        return {**res, **self.misc}
-
     def get_pandas_dtypes(self) -> Dict:
         """
         Convert dataset info columns data types to pandas compatible data types
         :return: Dictionary of pandas data types for dataset columns
         """
 
         dtypes = {}
@@ -1041,101 +1038,86 @@
         columns = []
         if df.index.name is not None:
             # add index column if it is not just an unnamed RangeIndex
             df = df.reset_index(inplace=False)
         name_series_iter = df.items()
         for column_name, column_series in name_series_iter:
             column_info = cls._calculate_stats_for_col(
-                column_name, 
-                column_series, 
-                max_inferred_cardinality,
-                data_type_version=CURRENT_DATA_TYPE_VERSION
+                column_name, column_series, max_inferred_cardinality
             )
             columns.append(column_info)
         return cls(
             display_name,
             columns,
             dataset_id=dataset_id,
             data_type_version=CURRENT_DATA_TYPE_VERSION,
         )
 
     @staticmethod
-    def _calculate_stats_for_col(
-        column_name, 
-        column_series, 
-        max_inferred_cardinality,
-        data_type_version:Optional[str]='v0'):
+    def _calculate_stats_for_col(column_name, column_series, max_inferred_cardinality):
         # @TODO Automatically drop the empty column with warning and proceed instead of aborting the upload
         if column_series.isna().all():
             raise ValueError(
                 f'Column {column_name} is empty. '
                 f'Please remove it and re-upload the dataset.'
             )
 
         # if we infer string or categorical, ensure that the underlying data
         # is also string by casting it.
-
-        # FDL-10905: dropna is needed to take care of cases where having None changes
-        # data type of int, float, bool to category. dropna() won't change 
-        # is_nullable detection as column_series.dropna() returns a new instance.
-        column_series_dropped_na = column_series.dropna()
         column_dtype = DatasetInfo.datatype_from_pandas_dtype(
-            column_series_dropped_na.infer_objects().dtype
+            column_series.infer_objects().dtype
         )
-        # get nullability before any datatype modifications like 'astype'
-        # which distorts None values.
-        is_nullable = bool(column_series.isna().any())
-
         if column_dtype in [DataType.CATEGORY, DataType.STRING]:
             if 'mixed' in pd.api.types.infer_dtype(column_series):
                 LOG.warning(
                     '***********************************\n'
                     'WARNING: The column passed has mixed datatypes.\n'
                     ' We have casted the column to string to ensure smooth functionality.\n'
                     '***********************************'
                 )
+            column_series = column_series.astype(str)
 
         # infer categorical if configured to do so
         if (
             max_inferred_cardinality
             and column_dtype.value == DataType.STRING.value
             and not is_datetime(column_series)
-            and column_series_dropped_na.nunique() <= max_inferred_cardinality
+            and column_series.nunique() <= max_inferred_cardinality
         ):
             column_dtype = DataType.CATEGORY
 
         # get possible values for categorical type
         if column_dtype.value in [DataType.CATEGORY.value, DataType.BOOLEAN.value]:
-            possible_values = np.sort(column_series_dropped_na.astype(str).unique()).tolist()
-            # Only when data_type_version is 'v0', 
-            # categorical column values undergo int/bool -> float -> string conversion.        
-            if data_type_version == 'v0':
-                possible_values_floats = None
-                if column_dtype.value == DataType.CATEGORY.value:
-                    try:
-                        possible_values_floats = [
-                            str(float(raw_val)) for raw_val in possible_values
-                        ]
-                    except ValueError:
-                        pass
-                if possible_values_floats is not None:
-                    possible_values = possible_values_floats
+            possible_values = np.sort(column_series.dropna().unique()).tolist()
+            possible_values_floats = None
+            if column_dtype.value == DataType.CATEGORY.value:
+                try:
+                    possible_values_floats = [
+                        str(float(raw_val)) for raw_val in possible_values
+                    ]
+                except ValueError:
+                    pass
+            if possible_values_floats is not None:
+                possible_values = possible_values_floats
         else:
             possible_values = None
 
         # get value range for numerical dtype
         if column_dtype.is_numeric():
-            value_min, value_max = column_series.agg(['min', 'max'])
+            # these are saved as series members.
+            value_min, value_max = column_series.min(), column_series.max()
             if np.isnan(value_min):
                 value_min = None
             if np.isnan(value_max):
                 value_max = None
         else:
             value_min, value_max = None, None
 
+        # get nullability
+        is_nullable = bool(column_series.isna().any())
         return Column(
             name=column_name,
             data_type=column_dtype,
             possible_values=possible_values,
             is_nullable=is_nullable,
             value_range_min=value_min,
             value_range_max=value_max,
@@ -1376,18 +1358,18 @@
     def __init__(
         self,
         display_name: str,
         input_type: ModelInputType,
         model_task: ModelTask,
         inputs: List[Column],
         outputs: List[Column],
-        targets: [List[Column]],
         target_class_order: Optional[List] = None,
         metadata: Optional[List[Column]] = None,
         decisions: Optional[List[Column]] = None,
+        targets: Optional[List[Column]] = None,
         algorithm: Optional[str] = None,
         framework: Optional[str] = None,
         description: Optional[str] = None,
         datasets: Optional[List[str]] = None,
         weighting_params: Optional[WeightingParams] = None,
         mlflow_params: Optional[MLFlowParams] = None,
         model_deployment_params: Optional[ModelDeploymentParams] = None,
@@ -1452,26 +1434,23 @@
                 param_name='artifact_status', from_version='1.7'
             )
 
         if custom_explanation_names is None:
             custom_explanation_names = []
 
         self.is_binary_ranking_model = is_binary_ranking_model
-        self._validate_columns()
-        
-        self.target_class_order = self.get_target_class_order(
-            self.target_class_order, self.model_task, self.targets[0])
+
+        self.target_class_order = self.get_target_class_order(self.target_class_order, self.model_task, self.targets[0])
 
         if model_task == ModelTask.RANKING:
             if group_by is None:
                 raise ValueError(
                     'The argument group_by cannot be empty for Ranking models'
                 )
-            if target_class_order is not None:
-                self.is_binary_ranking_model = len(target_class_order) == 2
+            self.is_binary_ranking_model = len(self.target_class_order) == 2
 
         self.group_by = group_by
 
         if tree_shap_enabled:
             custom_explanation_names.append('Tree Shap')
             if preferred_explanation_method is None:
                 preferred_explanation_method = 'Tree Shap'
@@ -1482,23 +1461,24 @@
 
         # Prevent the user from overloading a built-in.
         if custom_explanation_names is not None:
             duplicated_names = []
             for name in custom_explanation_names:
                 if type(name) != str:
                     raise ValueError(
-                        f"custom_explanation_names for ModelInfo must all be of type 'str', "
-                        f"but '{name}' is of type '{type(name)}'"
+                        f'custom_explanation_names for ModelInfo must all be of '
+                        f"type 'str', but '{name}' is of type '{type(name)}'"
                     )
                 if name in BUILT_IN_EXPLANATION_NAMES:
                     duplicated_names.append(name)
             if len(duplicated_names) > 0:
                 raise ValueError(
-                    f'Please select different names for your custom explanations. The following are reserved'
-                    f' built-ins duplicated in your custom explanation names: {duplicated_names}.'
+                    f'Please select different names for your custom explanations. '
+                    f'The following are reserved built-ins duplicated in your custom '
+                    f'explanation names: {duplicated_names}.'
                 )
 
         # Prevent the user from defaulting to an explanation that doesn't exist
         assert (
             custom_explanation_names is not None
         ), 'custom_explanation_names is unexpectedly None'
         if (
@@ -1520,43 +1500,53 @@
 
         self.preferred_explanation_method = preferred_explanation_method
         self.custom_explanation_names = custom_explanation_names
         self.misc = kwargs
 
         if fall_back is not None:
             LOG.warning(
-                'WARNING: fall_back will be deprecated in a future version. Use missing_value_encodings instead. '
+                'WARNING: fall_back will be deprecated in a future version. '
+                'Use missing_value_encodings instead. '
             )
         if missing_value_encodings is None:
             self.missing_value_encodings = fall_back
         else:
             self.missing_value_encodings = missing_value_encodings
             if fall_back is not None and fall_back != missing_value_encodings:
                 LOG.warning(
-                    'WARNING: Both missing_value_encodings and fall_back are specified, accept '
-                    'missing_value_encodings and ignore fall_back. '
+                    'WARNING: Both missing_value_encodings and fall_back are specified,'
+                    ' accept missing_value_encodings and ignore fall_back. '
                 )
         if self.missing_value_encodings is not None:
             ModelInfo.validate_missing_value_encodings(
                 self.missing_value_encodings, self.get_all_cols()
             )
         self.fall_back = self.missing_value_encodings  # backward compatability
 
-        available_cols = (
-            self.get_input_names() + self.get_target_names() + self.get_metadata_names()
-        )
         if self.custom_features is not None:
             if not isinstance(self.custom_features, List):
                 raise ValueError(
                     'The custom_features argument only accepts a list of CustomFeature objects.'
                 )
             if len(self.custom_features) > MAX_NUMBER_OF_CUSTOM_FEATURES:
                 raise ValueError(
                     f'The maximum number of custom features in a project cannot exceed {MAX_NUMBER_OF_CUSTOM_FEATURES}. {len(self.custom_features)} custom features are defined.'
                 )
+
+            available_cols = (
+                self.get_input_names() + self.get_target_names() + self.get_metadata_names()
+            )
+            numeric_cols = self.get_input_pandas_dtypes()
+            if self.metadata:
+                numeric_cols.update(self.get_metadata_pandas_dtypes())
+            if self.targets:
+                numeric_cols.update(self.get_target_pandas_dtypes())
+            valid_col_names = [k for k, v in numeric_cols.items() if
+                               v in (DataType.INTEGER.value, DataType.FLOAT.value)]
+
             unique_cf_names = []
             for feature in self.custom_features:
 
                 if not isinstance(feature, CustomFeature):
                     raise ValueError(
                         'The custom_features argument only accepts a list of CustomFeature objects.'
                     )
@@ -1571,22 +1561,22 @@
                         f'Multiple custom features are defined with the same name {feature.name}.'
                     )
                 else:
                     unique_cf_names.append(feature.name)
 
                 if isinstance(feature.columns, list):
                     for col in feature.columns:
-                        if col not in available_cols:
+                        if col not in valid_col_names:
                             raise ValueError(
-                                f"Custom features '{feature.name}' is defined based on column '{col}' which was not found."
+                                f"Custom features '{feature.name}' defined on column '{col}' is not found or not of type int/float."
                             )
                 else:
-                    if feature.columns not in available_cols:
+                    if feature.columns not in valid_col_names:
                         raise ValueError(
-                            f"Custom features '{feature.name}' is defined based on column '{feature.columns}' which was not found."
+                            f"Custom features '{feature.name}' defined on column '{feature.columns}' is not found or not of type int/float."
                         )
 
     def warn_deprecated_parameter(self, param_name: str, from_version: str) -> None:
         warnings.warn(
             f'WARNING: {param_name} is deprecated in {from_version}. It will be removed from 2.0.0 version.',
             DeprecationWarning,
         )
@@ -1596,24 +1586,25 @@
         res = {
             'name': self.display_name,
             'input-type': self.input_type.value,
             'model-task': self.model_task.value,
             'inputs': [c.to_dict() for c in self.inputs],
             'outputs': [c.to_dict() for c in self.outputs],
             'datasets': self.datasets or [],
-            'targets': [target_col.to_dict() for target_col in self.targets],
         }
         if self.target_class_order is not None:
             res['target-class-order'] = self.target_class_order
         if self.metadata:
             res['metadata'] = [metadata_col.to_dict() for metadata_col in self.metadata]
         if self.decisions:
             res['decisions'] = [
                 decision_col.to_dict() for decision_col in self.decisions
             ]
+        if self.targets:
+            res['targets'] = [target_col.to_dict() for target_col in self.targets]
         if self.description is not None:
             res['description'] = self.description
         if self.algorithm is not None:
             res['algorithm'] = self.algorithm
         if self.framework is not None:
             res['framework'] = self.framework
         if self.mlflow_params is not None:
@@ -1813,31 +1804,14 @@
             data_type_version=data_type_version,
             **deserialized_json,
         )
         # Explicitly set the version number
         model_info.schema_version = schema_version
         return model_info
 
-    def _validate_columns(self) -> None:
-        """
-        validate if required columns are provided in constructor and populate target_class_order
-        """
-        if not self.inputs:
-            raise ValueError('Model inputs not specified')
-
-        if not self.outputs:
-            raise ValueError('Model outputs not specified')
-
-        if not self.targets:
-            raise ValueError('Model targets not specified')
-
-        if not isinstance(self.targets, list) or len(self.targets) != 1:
-            raise ValueError('Model target must be a list of Column with length 1')
-
-
     @staticmethod
     def validate_missing_value_encodings(
         missing_value_encodings: dict, all_columns: List[Column]
     ) -> None:
         unmatched_col = []
         if not isinstance(missing_value_encodings, dict):
             raise ValueError(
@@ -1882,14 +1856,15 @@
         for k in unmatched_col:
             del missing_value_encodings[k]
         if len(missing_value_encodings) == 0:
             raise ValueError(
                 'None of the missing_value_encodings(fall_back) matches the column names entered, please provide '
                 'dictionary with valid keys.'
             )
+
     @staticmethod
     def _infer_target_class_order(target_column: Column, model_task: ModelTask):
         '''
         function is called when users don't provide target-class-order when creating
         model-info object, from __init__ and from_dataset_info.
         -regression: None
         -binary_classification:
@@ -1945,14 +1920,16 @@
         """Returns a list of names for model decisions."""
         if self.decisions is None:
             return []
         return [column.name for column in self.decisions]
 
     def get_target_names(self):
         """Returns a list of names for model targets."""
+        if self.targets is None:
+            return []
         return [column.name for column in self.targets]
 
     def get_input_pandas_dtypes(
         self,
     ) -> Dict[str, Union[str, pandas.api.types.CategoricalDtype]]:
         """Get a dictionary describing the pandas datatype of every input."""
         return _get_field_pandas_dtypes(self.inputs)
@@ -1982,14 +1959,23 @@
     def get_target_pandas_dtypes(
         self,
     ) -> Dict[str, Union[str, pandas.api.types.CategoricalDtype]]:
         """Get a dictionary describing the pandas datatype of every target."""
         assert self.targets is not None
         return _get_field_pandas_dtypes(self.targets)
 
+    def get_non_monitor_components(self):
+        ret = []
+        if self.custom_features is None:
+            return ret
+        for cf in self.custom_features:
+            if not getattr(cf, 'monitor_components', False):
+                ret.extend(cf.columns)
+        return ret
+
     @classmethod  # noqa: C901
     def from_dataset_info(
         cls,
         dataset_info: DatasetInfo,
         target: str,
         dataset_id: Optional[str] = None,
         features: Optional[Sequence[str]] = None,
@@ -2002,23 +1988,25 @@
         algorithm: Optional[str] = None,
         framework: Optional[str] = None,
         input_type: ModelInputType = ModelInputType.TABULAR,
         model_task: Optional[ModelTask] = None,
         outputs: Optional[Any] = None,
         categorical_target_class_details: Optional[Any] = None,
         weighting_params: Optional[WeightingParams] = None,
+        model_deployment_params: Optional[ModelDeploymentParams] = None,
         preferred_explanation_method: Optional[str] = None,
         custom_explanation_names: Optional[List[str]] = None,
         binary_classification_threshold: Optional[float] = None,
         ranking_top_k: Optional[int] = None,
         group_by: Optional[str] = None,
         tree_shap_enabled: Optional[bool] = False,
         custom_features: Optional[List[CustomFeature]] = None,
     ):
         """Produces a ModelInfo for a model trained on a dataset.
+
         :param dataset_info: A DatasetInfo object describing the training
             dataset.
         :param target: The column name of the target the model predicts.
         :param dataset_id: Specify the dataset_id for the model. Must be provided if the dataset_id cannot be inferred from the dataset_info.
         :param features: A list of column names for columns used as features.
         :param missing_value_encodings(fall_back): A dictionary of list representing the values that should be
            replaced with null for each columns. Key is the column name.
@@ -2033,41 +2021,47 @@
         :param framework: A string providing information about the software library
             and version used to train and run this model.
         :param input_type: Specifies the paradigm (tabular or text) of the
             model.
         :param model_task: Specifies the prediction task addressed by the
             model. If not explicitly provided, this will be inferred from the
             data type of the target variable.
+        :param mlflow_params: MLFlow parameters.
         :param outputs: model output names, if multiclass classification, must be a sequence in the same order as categorical_target_class_details.
             If binary classification, must be a single name signifying the probability of the positive class. # TODO: bulletproofing
             If regression/ranking, must be a dictionary of the form {column_name: (min_value, max_value)}, or a
             dictionary with empty range {column_name:[]} if column_name can be found in the dataset
         :param categorical_target_class_details: specify the output categories of your model (only applicable for classification and ranking models)
             This parameter *must* be provided for multiclass, binary-classification and ranking models where
             the target is of type CATEGORY. It is optional for binary classification with BOOLEAN targets, and ignored for regression.
+
             For multiclass classification models, provide a list of all the possible
             output categories of your model. The same order will be implicitly assumed
             by register model surrogate, and must match the outputs from custom package.py
             uploads. # TODO: ensure surrogate order matches this order.
+
             For binary classification models, if you provide a single element (or a list with
             a single element) then that element will be considered to be the positive class.
             Alternatively you can provide a list with 2 elements. The 0th element,
             by convention will be considered to be the negative class, and the 1th element will
             define the positive class. These params can be used to override the default convention
             specified below.
+
             For binary classification with target of type BOOLEAN:
                 - by default `True` is the positive class for `True`/`False` targets.
                 - by default `1` or `1.0` for `1`/`0` integer targets or `1.`/`0.` float targets,
             For other binary classification tasks on numeric types:
                 - by default the higher of the two possible values will be considered the positive class.
             In all other cases, one of the two classes will arbitrarily be FIXED as the positive class.
+
             For ranking models, provide a list of all the possible target values in order of relevance. The first element will be considered
             as not relevant, the last element from the list will be considered the most relevant grade.
         :param weighting_params: [Optional] Weighting parameters to account for class-imbalance. These parameters
             will be used to generate reference and production histograms.
+        :param model_deployment_params: Model Deployment parameters.
         :param preferred_explanation_method: [Optional] Specifies a preference
             for the default explanation algorithm.  Front-end will choose
             explanaton method if unspecified (typically Fiddler Shapley).
             Providing ExplanationMethod.CUSTOM will cause the first of the
             custom_explanation_names to be the default (which must be defined
             in that case).
         :param custom_explanation_names: [Optional] List of names that
@@ -2080,14 +2074,15 @@
         :param group_by: [Optional] A string representing the column name performance metrics have
          to be group by with for performance metrics computation. This have to be given for Ranking for MAP
           and NDCG computations. For ranking models, it represents the query/session id column.
         :param tree_shap_enabled: [Optional] Boolean value indicating if Tree SHAP should be enabled for this model.
            If set to True, Tree SHAP will become the default explanation method unless you specify another
            preferred explanation method.
         :param custom_features: [Optional] A list of custom features that are instances of CustomFeature class.
+
         :returns A ModelInfo object.
         """
         if categorical_target_class_details is not None:
             warnings.warn(
                 'WARNING: categorical_target_class_details is deprecated in 1.7 and '
                 'will be removed from 2.0.0 version. As a replacement, use target_class'
                 '_order while constructing ModelInfo.',
@@ -2220,14 +2215,16 @@
             inputs=inputs,
             outputs=output_columns,
             target_class_order=target_class_order,
             metadata=metadata,
             decisions=decisions,
             targets=[target_column],
             weighting_params=weighting_params,
+            mlflow_params=None,
+            model_deployment_params=model_deployment_params,
             preferred_explanation_method=preferred_explanation_method,
             custom_explanation_names=custom_explanation_names,
             binary_classification_threshold=binary_classification_threshold,
             ranking_top_k=ranking_top_k,
             group_by=group_by,
             fall_back=fall_back,
             missing_value_encodings=missing_value_encodings,
@@ -2404,20 +2401,20 @@
     @classmethod
     def check_binary_target(cls, target_column: Column) -> bool:
         if target_column.data_type.value in [
             DataType.INTEGER.value,
             DataType.FLOAT.value,
         ]:
             return (
-                       int(target_column.value_range_max) == 1
-                       and int(target_column.value_range_min) in [0, -1]
-                   ) or (
-                       target_column.data_type.value == DataType.INTEGER.value
-                       and target_column.value_range_max - target_column.value_range_min == 1
-                   )
+                int(target_column.value_range_max) == 1
+                and int(target_column.value_range_min) in [0, -1]
+            ) or (
+                target_column.data_type.value == DataType.INTEGER.value
+                and target_column.value_range_max - target_column.value_range_min == 1
+            )
         else:
             return len(target_column.possible_values) == 2
 
     @classmethod
     def get_inputs_metadata_decisions(
         cls,
         dataset_info: DatasetInfo,
@@ -2464,67 +2461,48 @@
         dataset_info: DatasetInfo,
         model_task: ModelTask,
     ) -> Optional[List[Column]]:
         if not output_names:
             return None
 
         output_columns = []
-        ds_info_names_columns = {}
-        for ds_column in dataset_info.columns:
-            ds_info_names_columns[ds_column.name] = ds_column
 
         if model_task.is_classification():
             if isinstance(output_names, dict):
                 output_names = list(output_names.keys())
             for name in output_names:
-                if name in ds_info_names_columns:
-                    output_columns.append(ds_info_names_columns[name])
-                else:
-                    output_columns.append(
-                        Column(
-                            name=name,
-                            data_type=DataType.FLOAT,
-                            is_nullable=False,
-                            value_range_min=0.0,
-                            value_range_max=1.0,
-                        )
+                output_columns.append(
+                    Column(
+                        name=name,
+                        data_type=DataType.FLOAT,
+                        is_nullable=False,
+                        value_range_min=0.0,
+                        value_range_max=1.0,
                     )
+                )
             return output_columns
 
         if isinstance(output_names, dict):
             for name in output_names.keys():
                 values = output_names[name]
                 if not isinstance(values, (list, tuple)) or len(values) != 2:
                     raise ValueError(
                         f'If outputs is a dictionary, the values should '
                         f'be a tuple of 2 values. Currently passing: '
                         f'{values} for output {name}. Please correct.'
                     )
-                if name in ds_info_names_columns:
-                    column = ds_info_names_columns[name]
-                    if not (
-                        column.data_type == DataType.FLOAT or column.data_type == DataType.INTEGER):
-                        raise ValueError(
-                            f'Column {name} with type {column.data_type} can not be specified as output.'
-                            f'Output column type has to be either INTEGER or FLOAT.'
-                            f'Please correct.'
-                        )
-                    column.value_range_min = min(values)
-                    column.value_range_max = max(values)
-                    output_columns.append(column)
-                else:
-                    output_columns.append(
-                        Column(
-                            name=name,
-                            data_type=DataType.FLOAT,
-                            is_nullable=False,
-                            value_range_min=float(min(values)),
-                            value_range_max=float(max(values)),
-                        )
+                output_columns.append(
+                    Column(
+                        name=name,
+                        data_type=DataType.FLOAT,
+                        is_nullable=False,
+                        value_range_min=float(min(values)),
+                        value_range_max=float(max(values)),
                     )
+                )
             return output_columns
 
         if isinstance(output_names, list):
             for name in output_names:
                 col = name
                 if name not in dataset_info.get_column_names():
                     if model_task.value == ModelTask.REGRESSION.value and target_column:
@@ -2532,20 +2510,14 @@
                         col = target_column.name
                     else:
                         raise ValueError(
                             f'Output {name} is not present in the dataset. '
                             f'Please provide a dictionary with the range: '
                             f'{name}: (min_value, max_value).'
                         )
-                if dataset_info[col].value_range_min is None or dataset_info[
-                    col].value_range_max is None:
-                    raise ValueError(
-                        f'Column {name} with value_range_min or value_range_max as None can not be specified as output.'
-                        f'Please correct.'
-                    )
                 output_columns.append(
                     Column(
                         name=name,
                         data_type=DataType.FLOAT,
                         is_nullable=False,
                         value_range_min=float(dataset_info[col].value_range_min),
                         value_range_max=float(dataset_info[col].value_range_max),
@@ -3276,46 +3248,49 @@
 
 
 def _summary_dataframe_for_custom_features(
     custom_features: Sequence[CustomFeature], placeholder=''
 ) -> pd.DataFrame:
     """
         Example:
-        name    column                      type                transformation  n_clusters  monitor
-    0   F1      'col_name1'                 FROM_TEXT           'Word2vec'      3           True
-    1   F2      ['col_name2','col_name3']   FROM_COLUMNS        None            4           True
-    2   F3      'col_name4'                 FROM_VECTOR         None            auto        True
-    3   F4      'col_name5'                 FROM_DICTIONARY     None            auto        True
+        name    column                      type                transformation  n_clusters  monitor  monitor_components
+    0   F1      'col_name1'                 FROM_TEXT           'Word2vec'      3           True        False
+    1   F2      ['col_name2','col_name3']   FROM_COLUMNS        None            4           True        False
+    2   F3      'col_name4'                 FROM_VECTOR         None            auto        True        False
+    3   F4      'col_name5'                 FROM_DICTIONARY     None            auto        True        False
     """  # noqa E501
     names = []
     columns = []
     types = []
     transformations = []
     clusters = []
     monitors = []
+    monitor_components = []
 
     for feature in custom_features:
         names.append(feature.name)
         columns.append(feature.columns)
         types.append(feature.type.name)
         transformations.append(feature.transformation)
         if feature.n_clusters is not None:
             clusters.append(feature.n_clusters)
         else:
             clusters.append('auto')
         monitors.append(feature.monitor)
+        monitor_components.append(feature.monitor_components)
 
     return pd.DataFrame(
         {
             'name': names,
             'column': columns,
             'type': types,
             'transformation': transformations,
             'n_clusters': clusters,
             'monitor': monitors,
+            'monitor_components': monitor_components,
         }
     )
 
 
 @enum.unique
 class BaselineType(str, enum.Enum):
     PRE_PRODUCTION = 'PRE_PRODUCTION'
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/dataset.py` & `fiddler-client-2.0.0.dev1/fiddler/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/experimental.py` & `fiddler-client-2.0.0.dev1/fiddler/experimental.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/libs/http_client.py` & `fiddler-client-2.0.0.dev1/fiddler/libs/http_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from copy import deepcopy
 from typing import Dict, Optional
 from urllib.parse import urljoin
 
 import requests
 from requests.adapters import HTTPAdapter
+from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 APP_JSON_CONTENT_TYPE = 'application/json'
 
 
 class RequestClient:
     def __init__(
         self, base_url: str, headers: Dict[str, str], verify: bool = True
@@ -29,19 +30,25 @@
         *,
         method: str,
         url: str,
         params: Optional[dict] = None,
         headers: Optional[dict] = None,
         data: Optional[dict] = None,
         timeout: Optional[int] = None,
+        files_encoders: Optional[Dict[str, MultipartEncoder]] = None,
         **kwargs,
     ) -> requests.Response:
         """
         Make request to server
+
+        :param files_encoders  (optional) Dictionary of 'filename': file-like-objects
+            for multipart encoding upload. Make sure all MultipartEncoder values have
+            same content_type.
         """
+
         full_url = urljoin(self.base_url + '/', url)
 
         request_headers = self.headers
         # override/update headers coming from the calling method
         if headers:
             request_headers = deepcopy(self.headers)
             request_headers.update(headers)
@@ -51,23 +58,37 @@
             data = json.dumps(data)
 
         kwargs.setdefault('allow_redirects', True)
         # requests is not able to pass the value of self.session.verify to the
         # verify param in kwargs when REQUESTS_CA_BUNDLE is set.
         # So setting that as default here
         kwargs.setdefault('verify', self.session.verify)
-        response = self.session.request(
-            method,
-            full_url,
-            params=params,
-            data=data,
-            headers=request_headers,
-            timeout=timeout,
-            **kwargs,
-        )
+        if files_encoders:
+            encoders = list(files_encoders.values())
+            if encoders:
+                request_headers['Content-Type'] = encoders[0].content_type
+            response = self.session.request(
+                method,
+                full_url,
+                params=params,
+                files=files_encoders,
+                headers=request_headers,
+                timeout=timeout,
+                **kwargs,
+            )
+        else:
+            response = self.session.request(
+                method,
+                full_url,
+                params=params,
+                data=data,
+                headers=request_headers,
+                timeout=timeout,
+                **kwargs,
+            )
         response.raise_for_status()
         return response
 
     def get(
         self,
         *,
         url: str,
@@ -107,23 +128,25 @@
         self,
         *,
         url: str,
         params: Optional[dict] = None,
         headers: Optional[dict] = None,
         timeout: Optional[int] = None,
         data: Optional[dict] = None,
+        files_encoders: Optional[Dict[str, MultipartEncoder]] = None,
         **kwargs,
     ):
         return self.call(
             method='POST',
             url=url,
             params=params,
             headers=headers,
             timeout=timeout,
             data=data,
+            files_encoders=files_encoders,
             **kwargs,
         )
 
     def put(
         self,
         *,
         url: str,
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/model_info_validator.py` & `fiddler-client-2.0.0.dev1/fiddler/model_info_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-from fiddler.core_objects import (
-    DatasetInfo,
-    DataType,
-    ModelInfo,
-    ModelInputType,
-    ModelTask,
-)
+from .core_objects import DatasetInfo, DataType, ModelInfo, ModelInputType, ModelTask
 
 
 class ModelInfoValidator:
     def __init__(self, model_info: ModelInfo, dataset_info: DatasetInfo):
         self.model_info = model_info
         self.dataset_info = dataset_info
 
@@ -42,20 +36,36 @@
     def validate_add_model(self):
         if not self.model_info.targets:
             raise ValueError('Target not specified')
 
         if len(self.model_info.targets) != 1:
             raise ValueError('More than one target specified')
 
-        if len(self.model_info.inputs) < 1:
+        if not self.model_info.inputs:
             raise ValueError('Input features not specified')
 
-        if len(self.model_info.outputs) < 1:
+        if not self.model_info.outputs:
             raise ValueError('Model outputs not defined')
 
+        if self.model_info.input_type.value == ModelInputType.TEXT.value:
+            if len(self.model_info.inputs) != 1:
+                raise ValueError(
+                    f'Text models may only contain a single feature column containing '
+                    f'text data. Please remove any other non-text features from the '
+                    f'features argument if you wish to add a text model. You can add '
+                    f'other columns as metadata columns. If your model has multiple '
+                    f'inputs please specify the input_type to {ModelInputType.TABULAR}.'
+                )
+            if self.model_info.inputs[0].data_type.value != DataType.STRING:
+                raise ValueError(
+                    'Text features must be of type STRING. Please double check the '
+                    'data type of the feature column passed into the '
+                    'features argument.'
+                )
+
         if self.model_info.model_task == ModelTask.REGRESSION:
             self.validate_regression_model()
         elif self.model_info.model_task == ModelTask.BINARY_CLASSIFICATION:
             self.validate_binary_classification_model()
         elif self.model_info.model_task == ModelTask.MULTICLASS_CLASSIFICATION:
             self.validate_multiclass_classification()
         elif self.model_info.model_task == ModelTask.RANKING:
@@ -144,11 +154,15 @@
         if self.model_info.outputs[0].data_type != DataType.FLOAT:
             raise ValueError('model output must be of type FLOAT')
         if self.model_info.targets[0].data_type == DataType.STRING:
             raise ValueError(
                 """Target cannot be of type string.
                  Please review dataset schema."""
             )
+        if not self.model_info.group_by:
+            raise ValueError(
+                'Argument group_by has to be specified for ranking models.'
+            )
 
     def validate_weighting(self):
         # TODO: validate weighting params
         pass
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/monitoring_validator.py` & `fiddler-client-2.0.0.dev1/fiddler/monitoring_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/packtools/gem.py` & `fiddler-client-2.0.0.dev1/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-2.0.0.dev1/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-2.0.0.dev1/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/packtools/template_model.py` & `fiddler-client-2.0.0.dev1/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/project.py` & `fiddler-client-2.0.0.dev1/fiddler/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,143 @@
-from typing import List, Optional
+import os
+import tarfile
+import tempfile
+from pathlib import Path
+
+import requests
 
 from fiddler.connection import Connection
-from fiddler.dataset import Dataset
-from fiddler.model import Model
+from fiddler.core_objects import ModelInfo
 from fiddler.utils.general_checks import type_enforce
 
 
-class Project:
-    def __init__(self, connection: Connection, project_id: str):
+class Model:
+    def __init__(self, connection: Connection, project_id: str, model_id):
         self.connection = connection
         self.project_id = project_id
+        self.model_id = model_id
 
-    def list_models(self) -> List[str]:
-        """List the names of all models in a project.
+    def get_info(self) -> ModelInfo:
+        """Get ModelInfo for a model in a certain project.
 
-        :returns: List of strings containing the ids of each model in the
-            specified project.
+        :returns: A fiddler.ModelInfo object describing the model.
         """
+        # Type enforcement
         project_id = type_enforce('project_id', self.project_id, str)
-        path = ['list_models', self.connection.org_id, project_id]
+        model_id = type_enforce('model_id', self.model_id, str)
+
+        path = ['model_info', self.connection.org_id, project_id, model_id]
         res = self.connection.call(path, is_get_request=True)
-        return res
+        return ModelInfo.from_dict(res)
+
+    def delete(self, delete_prod=False, delete_pred=True):
+        """Permanently delete a model.
+
+        :param delete_prod: Boolean value to delete the production table.
+            By default this table is not dropped.
+        :param delete_pred: Boolean value to delete the prediction table.
+            By default this table is dropped.
 
-    def delete(self):
-        """Permanently delete a project.
         :returns: Server response for deletion action.
         """
         # Type enforcement
         project_id = type_enforce('project_id', self.project_id, str)
-        path = ['delete_project', self.connection.org_id, project_id]
-        result = self.connection.call(path)
-        return result
-
-    def share(
-        self,
-        role: str,
-        user_name: Optional[str] = None,
-        team_name: Optional[str] = None,
-    ):
-        """Share a project with other users and/or teams.
-
-        :param role: one of ["READ", "WRITE", "OWNER"].
-        :param user_name: (optional) username, typically an email address.
-        :param team_name: (optional) name of the team.
-
-        :returns: Server response for creation action.
-        """
-        if user_name is None and team_name is None:
-            err = 'one of user_name, team_name must be provided'
-            raise ValueError(err)
-
-        if user_name is not None and team_name is not None:
-            err = 'Only one of user_name or team_name must be provided'
-            raise ValueError(err)
-
-        if role not in ['READ', 'WRITE', 'OWNER']:
-            err = 'role must be one of READ, WRITE, or OWNER'
-            raise ValueError(err)
+        model_id = type_enforce('model_id', self.model_id, str)
 
         payload = {
-            'role': role,
-            'user_name': user_name,
-            'team_name': team_name,
+            'project_id': project_id,
+            'model_id': model_id,
+            'delete_prod': delete_prod,
+            'delete_pred': delete_pred,
         }
 
-        path = ['apply_project_role', self.connection.org_id, self.project_id]
-        return self.connection.call(path, json_payload=payload)
+        path = ['delete_model', self.connection.org_id, project_id, model_id]
+        try:
+            result = self.connection.call(path, json_payload=payload)
+        except Exception:
+            # retry on error
+            result = self.connection.call(path, json_payload=payload)
+
+        self._delete_artifacts()
+
+        # wait for ES to come back healthy
+        for i in range(3):
+            try:
+                self.connection.call_executor_service(
+                    ['deploy', self.connection.org_id], is_get_request=True
+                )
+                break
+            except Exception:
+                pass
 
-    def unshare(
-        self,
-        role: str,
-        user_name: Optional[str] = None,
-        team_name: Optional[str] = None,
-    ):
-        """un-Share a project with other users and/or teams.
-
-        :param role: one of ["READ", "WRITE", "OWNER"].
-        :param user_name: (optional) username, typically an email address.
-        :param team_name: (optional) name of the team.
+        return result
 
-        :returns: Server response for creation action.
-        """
-        if user_name is None and team_name is None:
-            err = 'one of user_name, team_name must be provided'
-            raise ValueError(err)
-
-        if user_name is not None and team_name is not None:
-            err = 'Only one of user_name or team_name must be provided'
-            raise ValueError(err)
-
-        if role not in ['READ', 'WRITE', 'OWNER']:
-            err = 'role must be one of READ, WRITE, or OWNER'
-            raise ValueError(err)
+    def _delete_artifacts(self):
+        """Permanently delete a model artifacts.
 
-        payload = {
-            'role': role,
-            'user_name': user_name,
-            'team_name': team_name,
-        }
+        :param project_id: The unique identifier of the model's project on the
+            Fiddler engine.
+        :param model_id: The unique identifier of the model in the specified
+            project on the Fiddler engine.
 
-        path = ['delete_project_role', self.connection.org_id, self.project_id]
-        return self.connection.call(path, json_payload=payload)
+        :returns: Server response for deletion action.
+        """
+        # delete from executor service cache
+        # Type enforcement
+        project_id = type_enforce('project_id', self.project_id, str)
+        model_id = type_enforce('model_id', self.model_id, str)
 
-    def list_roles(self):
-        """List the users and teams with access to a given project.
+        path = ['delete_model_artifacts', self.connection.org_id, project_id, model_id]
+        result = self.connection.call_executor_service(path)
 
-        :returns: list of users and teams with access to a given project.
-        """
-        path = ['roles', self.connection.org_id, self.project_id]
-        return self.connection.call(path, is_get_request=True)
+        return result
 
-    def list_datasets(self) -> List[str]:
-        """List the ids of all datasets in the organization.
+    def download(self, output_dir: Path):
+        """
+        download the model binary, package.py and model.yaml to the given
+        output dir.
 
-        :returns: List of strings containing the ids of each dataset.
+        :param output_dir: output directory
+        :return: model artifacts
         """
         # Type enforcement
         project_id = type_enforce('project_id', self.project_id, str)
+        model_id = type_enforce('model_id', self.model_id, str)
+        output_dir = type_enforce('output_dir', output_dir, Path)
 
-        path = ['list_datasets', self.connection.org_id, project_id]
-        res = self.connection.call(path, is_get_request=True)
+        if output_dir.exists():
+            raise ValueError(f'output dir already exists {output_dir}')
 
-        return res
+        headers = dict()
+        headers.update(self.connection.auth_header)
 
-    def model(self, model_id: str) -> Model:
-        return Model(self.connection, self.project_id, model_id)
+        _, tfile = tempfile.mkstemp('.tar.gz')
+        url = f'{self.connection.url}/get_model/{self.connection.org_id}/{project_id}/{model_id}'
+
+        with requests.get(url, headers=headers, stream=True) as r:
+            r.raise_for_status()
+            with open(tfile, 'wb') as f:
+                for chunk in r.iter_content(chunk_size=8192):
+                    # If you have chunk encoded response uncomment if
+                    # and set chunk_size parameter to None.
+                    # if chunk:
+                    f.write(chunk)
+
+        tar = tarfile.open(tfile)
+        output_dir.mkdir(parents=True)
+        tar.extractall(path=output_dir)
+        tar.close()
+        os.remove(tfile)
+        return True
+
+    def _trigger_model_predictions(self, dataset_id: str):
+        """Makes the Fiddler service compute and cache model predictions on a
+        dataset."""
+        # Type enforcement
+        project_id = type_enforce('project_id', self.project_id, str)
+        model_id = type_enforce('model_id', self.model_id, str)
+        dataset_id = type_enforce('dataset_id', dataset_id, str)
 
-    def dataset(self, dataset_id: str) -> Dataset:
-        return Dataset(self.connection, self.project_id, dataset_id)
+        return self.connection.call_executor_service(
+            ['dataset_predictions', self.connection.org_id, project_id],
+            dict(model=model_id, dataset=dataset_id),
+        )
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/utils/__init__.py` & `fiddler-client-2.0.0.dev1/fiddler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/utils/exceptions.py` & `fiddler-client-2.0.0.dev1/fiddler/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/utils/formatting.py` & `fiddler-client-2.0.0.dev1/fiddler/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/utils/general_checks.py` & `fiddler-client-2.0.0.dev1/fiddler/utils/general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/utils/helper.py` & `fiddler-client-2.0.0.dev1/fiddler/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/utils/pandas.py` & `fiddler-client-2.0.0.dev1/fiddler/utils/pandas.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
-from fiddler.file_processor.src.constants import (
-    PARQUET_COMPRESSION,
-    PARQUET_ROW_GROUP_SIZE,
-)
+
+from fiddler.v2.constants import PARQUET_COMPRESSION, PARQUET_ROW_GROUP_SIZE
 
 from .. import constants
 
 LOG = logging.getLogger(__name__)
 TIMESTAMP = 'TIMESTAMP'
 
 
@@ -37,21 +35,18 @@
     works to:
     - Convert datetime to string
 
     TODO: Expand to all other datatypes
     """
     for ind, col_type in enumerate(df.dtypes):
         col = df.columns[ind]
-        if (
-            col_type is not None
-            and 'datetime64' in str(col_type)
-        ):
-            df[col] = pd.to_datetime(
-                df[col], utc=True
-            ).dt.tz_localize(None)  # Skipping timezone information from the column. REF: https://fiddlerlabs.atlassian.net/browse/FDL-2592
+        if col_type is not None and 'datetime64' in str(col_type):
+            df[col] = pd.to_datetime(df[col], utc=True).dt.tz_localize(
+                None
+            )  # Skipping timezone information from the column. REF: https://fiddlerlabs.atlassian.net/browse/FDL-2592
             df[col] = df[col].dt.strftime(constants.TIMESTAMP_FORMAT)
             df[col] = df[col].astype('string')
 
         # pandas considers the datatype as an object, if it finds multiple datatypes in a column
         # If such columns are consists of timestamp values, and those values are less than
         # specified 'max_inferred_cardinality' value. System infers the timestamp variable as a categorical
         # variable. To avoid that, we added a check where we check the object is a datetime object
@@ -138,15 +133,15 @@
 
     schema = schema or table.schema
 
     with pq.ParquetWriter(
         file_path, schema=schema, compression=PARQUET_COMPRESSION
     ) as pq_writer:
         pq_writer.write_table(table, row_group_size=PARQUET_ROW_GROUP_SIZE)
-        
+
 
 def convert_flat_csv_data_to_grouped(
     input_data: pd.DataFrame, group_by_col: str, output_path: Optional[str] = None
 ) -> pd.DataFrame:
     """
     :param input_data: The dataframe with flat data.
     :param group_by_col: The column to group the data by.
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v1_v2_compat.py` & `fiddler-client-2.0.0.dev1/fiddler/v1_v2_compat.py`

 * *Files 7% similar despite different names*

```diff
@@ -387,17 +387,15 @@
                          the following order: query_id 31,31,31,31,31,31,2,2.
         """
         v2_timestamp_format = V2FiddlerTimestamp(timestamp_format.value)
         if type(batch_source) == pd.DataFrame and (
             data_source is None or BatchPublishType.DATAFRAME == data_source
         ):
             if batch_source.empty:
-                raise ValueError(
-                    'The batch provided is empty. Please retry with at least one row of data.'
-                )
+                raise ValueError("The batch provided is empty. Please retry with at least one row of data.")
 
             return self.client_v2.publish_events_batch_dataframe(
                 project_name=project_id,
                 model_name=model_id,
                 events_df=batch_source,
                 id_field=id_field,
                 is_update=update_event,
@@ -418,17 +416,26 @@
                 timestamp_field=timestamp_field,
                 timestamp_format=v2_timestamp_format,
                 group_by=group_by,
                 file_type=FileType.CSV,
                 is_sync=False,
             )
         else:
-            raise NotImplementedError(
-                'Batch source other than dataframe and csv is not implemented now'
-            )
+            if data_source is not None:
+                if (data_source not in [BatchPublishType.LOCAL_DISK, BatchPublishType.DATAFRAME]):
+                    raise NotImplementedError(
+                        f'support for data_source type of {data_source} is not yet implemented'
+                    )
+                elif BatchPublishType.DATAFRAME == data_source and not isinstance(batch_source, pd.DataFrame):
+                    raise ValueError(f'based on the provided data_source type ({data_source}), expecting batch_source to be a pandas DataFrame, but instead found a {type(batch_source)}')
+                elif BatchPublishType.LOCAL_DISK == data_source and not isinstance(batch_source, str):
+                    raise ValueError(f'based on the provided data_source type ({data_source}), expecting batch_source to be a filepath string, but instead found a {type(batch_source)}')
+            else:
+                raise ValueError('batch_source must be either a filepath string or a pandas DataFrame')
+                            
 
     def publish_event(
         self,
         project_id: str,
         model_id: str,
         event: dict,
         event_id: Optional[str] = None,
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/alert_mixin.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/alert_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/api.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,9 +47,17 @@
         self.request_headers = {'Authorization': f'Bearer {auth_token}'}
         self.request_headers.update({FIDDLER_CLIENT_VERSION_HEADER: f'{__version__}'})
         self.timeout = timeout
         self.client = RequestClient(
             base_url=self.url, headers=self.request_headers, verify=verify
         )
 
-        # @TODO Move this from optional to required once /get_supported_features api moved to v2
-        self.server_info: Optional[ServerInfo] = None
+        self.server_info: Optional[ServerInfo] = self._get_server_info()
+
+    def _get_server_info(self) -> ServerInfo:
+
+        response = self.client.get(
+            url='server-info',
+            params={'organization_name': self.organization_name},
+        )
+
+        return ServerInfo(**response.json().get('data'))
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/baseline_mixin.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/baseline_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/events_mixin.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/events_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,17 +211,15 @@
                         in the file. For example, having a file with rows belonging to query_id 31,31,31,2,2,31,31,31
                         would not work. Please sort the file by group_by group first to have rows with
                         the following order: query_id 31,31,31,31,31,31,2,2.
         :param is_sync: A boolean value which determines if the upload method works in synchronous mode or async mode
         :returns: Dictionary containing details of the job used to publish events incase of 202 response from the server.
         """
         if events_df is None or events_df.empty:
-            raise ValueError(
-                'The batch provided is empty. Please retry with at least one row of data.'
-            )
+            raise ValueError("The batch provided is empty. Please retry with at least one row of data.")
 
         file_type = FileType.CSV
         with tempfile.NamedTemporaryFile(suffix=file_type) as temp:
             events_df.to_csv(temp, index=False)
             events_path = Path(temp.name)
             return self.publish_events_batch(
                 project_name=project_name,
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/explainability_mixin.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/explainability_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import namedtuple
-from typing import List, NamedTuple, Optional, Union
+from typing import Dict, List, NamedTuple, Optional, Union
 
 import pandas as pd
 from pydantic import BaseModel
 
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.utils.pandas import try_series_retype
@@ -368,7 +368,59 @@
             url='predict',
             data=request_body,
         )
 
         response_dict = APIResponseHandler(response).get_data()
 
         return pd.DataFrame(response_dict['predictions'])
+
+    @handle_api_error_response
+    def get_mutual_information(
+        self,
+        project_name: str,
+        dataset_name: str,
+        query: str,
+        column_name: str,
+        normalized: Optional[bool] = False,
+        num_samples: Optional[int] = None,
+    ) -> Dict[str, float]:
+        """
+        The Mutual information measures the dependency between two random variables.
+        It's a non-negative value. If two random variables are independent MI is
+        equal to zero. Higher MI values means higher dependency.
+
+        :param project_name: The unique identifier of the model's project on the
+            Fiddler engine.
+        :param dataset_name: The unique identifier of the dataset in the
+            Fiddler engine.
+        :param column_name: column name to compute mutual information with respect to
+               all the variables in the dataset.
+        :param normalized: If set to True, it will compute Normalized Mutual Information
+        :param query: slice query to compute Mutual information on
+        :param num_samples: Number of samples to select for computation
+        :return: a dictionary of mutual information w.r.t the given feature
+                 for each column given
+        """
+
+        if not isinstance(column_name, str):
+            raise ValueError(
+                f'Invalid type: {type(column_name)}. Argument column_name has '
+                f'to be a string.'
+            )
+
+        request_body = dict(
+            project_name=project_name,
+            organization_name=self.organization_name,
+            dataset_name=dataset_name,
+            column_name=column_name,
+            normalized=normalized,
+            query=query,
+            num_samples=num_samples,
+        )
+
+        response = self.client.post(
+            url='mutual-information',
+            data=request_body,
+        )
+        response_dict = APIResponseHandler(response).get_data()
+
+        return response_dict
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/helpers.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 import math
 import os
 from typing import Dict, Optional
 from urllib.parse import urljoin
+
 from tqdm import trange
 
 from fiddler.libs.http_client import RequestClient
 from fiddler.utils import logging
 from fiddler.v2.constants import (
     CONTENT_TYPE_OCTET_STREAM_HEADER,
+    MULTI_PART_CHUNK_SIZE,
     MULTI_PART_UPLOAD_SIZE_THRESHOLD,
     UploadType,
 )
 from fiddler.v2.utils.response_handler import APIResponseHandler
 
 logger = logging.getLogger(__name__)
 
 UPLOAD_ID_KEY = 'upload_id'
 UPLOAD_TYPE_KEY = 'upload_type'
 RESOURCE_IDENT_KEY = 'resource_identifier'
 FILE_NAME_KEY = 'file_name'
 MULTIPART_UPLOAD_KEY = 'multipart_upload'
+NUM_ROWS_KEY = 'num_rows'
+NUM_COLS_KEY = 'num_cols'
 IS_UPDATE = 'is_update'
 
 
 def multipart_upload(
     client: RequestClient,
     organization_name: str,
     project_name: str,
     identifier: str,
     upload_type: UploadType,
     file_path: str,
     file_name: str,
-    chunk_size: Optional[int] = 100 * 1024 * 1024,  # bytes
+    chunk_size: Optional[int] = MULTI_PART_CHUNK_SIZE,  # bytes
 ) -> Dict[str, str]:
     """
     Perform multipart upload for datasets/events ingestion
     """
     base_url = f'datasets/{organization_name}:{project_name}/'
     UPLOAD_INITIALIZE_URL = urljoin(base_url, 'initialize')
     UPLOAD_URL = urljoin(base_url, 'upload')
     UPLOAD_COMPLETE_URL = urljoin(base_url, 'complete')
 
     if not os.path.exists(file_path):
         raise ValueError(
             f'File {file_path} not found. Please check if the entered path is correct.'
         )
     file_size = os.path.getsize(file_path)
+
     if file_size < MULTI_PART_UPLOAD_SIZE_THRESHOLD:
         with open(file_path, 'rb') as f:
             file_data = f.read()
             response = client.put(
                 url=UPLOAD_URL,
                 params={
                     UPLOAD_TYPE_KEY: upload_type,
@@ -57,39 +62,47 @@
                     RESOURCE_IDENT_KEY: identifier,
                     FILE_NAME_KEY: file_name,
                 },
                 data=file_data,
                 headers=CONTENT_TYPE_OCTET_STREAM_HEADER,
             )
     else:
-        # Step 1: Initialize multipart upload
+        with open(file_path, 'rb') as f:
+            # from header
+            num_cols = len(f.readline().split(b','))
+            # from rest of the file
+            num_rows = sum(1 for _ in f)
+
+        # Step 1: Initialize upload
         response = client.post(
             url=UPLOAD_INITIALIZE_URL,
             data={
                 RESOURCE_IDENT_KEY: identifier,
                 FILE_NAME_KEY: file_name,
                 UPLOAD_TYPE_KEY: upload_type,
+                NUM_COLS_KEY: num_cols,
+                NUM_ROWS_KEY: num_rows,
             },
         )
         response_data = APIResponseHandler(response).get_data()
         upload_id = response_data.get(UPLOAD_ID_KEY)
         file_name = response_data.get(FILE_NAME_KEY)
 
         parts = []
         total_chunks = math.ceil(file_size / chunk_size)
+
         # Step 2: Chunk and upload
         logger.info('Beginning chunk upload')
         with open(file_path, 'rb') as f:
             for part_no in trange(1, total_chunks + 1, desc=file_name):
                 file_data = f.read(chunk_size)
                 if not file_data:
                     # continue, rather than break so that the progress bar completes.
                     # This will incur at max only one extra iteration.
                     continue
-
                 response = client.put(
                     url=UPLOAD_URL,
                     params={
                         UPLOAD_TYPE_KEY: upload_type,
                         MULTIPART_UPLOAD_KEY: True,
                         RESOURCE_IDENT_KEY: identifier,
                         FILE_NAME_KEY: file_name,
@@ -103,14 +116,15 @@
                 parts.append(
                     {
                         'ETag': resp_data.get('info').get('ETag'),
                         'PartNumber': resp_data.get('info').get('PartNumber'),
                     }
                 )
                 logger.info(f'Chunk uploaded: {part_no}/{total_chunks}')
+
         # Step 3: Complete the upload
         response = client.post(
             url=UPLOAD_COMPLETE_URL,
             params={
                 UPLOAD_TYPE_KEY: upload_type,
                 RESOURCE_IDENT_KEY: identifier,
                 FILE_NAME_KEY: file_name,
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/job_mixin.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/job_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/model_artifact_deploy.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/model_artifact_deploy.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/model_deployment_mixin.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/model_deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/model_mixin.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/model_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,20 @@
         :param model_name: name of the model
         :type model_name: string
         :param info: model related information
         :type info: ModelInfo
 
         :return: Model object which contains the model details
         """
+        if not isinstance(info, ModelInfo):
+            raise ValueError(
+                f'The value passed to the info parameter must be a ModelInfo object.'
+                f'Instead, found value of type {type(info)}'
+            )
+
         request_body = {
             'name': model_name,
             'project_name': project_name,
             'organization_name': self.organization_name,
             'info': info.to_dict(),
             'model_type': None,
             'file_list': None,
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/api/project_mixin.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/api/project_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/constants.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 CONTENT_TYPE_OCTET_STREAM = 'application/octet-stream'
 CONTENT_TYPE_OCTET_STREAM_HEADER = {CONTENT_TYPE_HEADER_KEY: CONTENT_TYPE_OCTET_STREAM}
 
 # Multi-part upload
 MULTI_PART_UPLOAD_SIZE_THRESHOLD = 5 * 1024 * 1024  # 5MB in bytes
 MULTI_PART_CHUNK_SIZE = 100 * 1024 * 1024  # 100MB in bytes
 
+# File processor
+SUPPORTABLE_FILE_EXTENSIONS = ['.csv']
+CSV_EXTENSION = 'csv'
+PARQUET_EXTENSION = 'parquet'
+PARQUET_COMPRESSION = 'snappy'
+PARQUET_ENGINE = 'pyarrow'
+PARQUET_ROW_GROUP_SIZE = 10_000
+
 
 @enum.unique
 class FiddlerTimestamp(str, enum.Enum):
     """Supported timestamp formats for events published to Fiddler"""
 
     EPOCH_MILLISECONDS = 'epoch milliseconds'
     EPOCH_SECONDS = 'epoch seconds'
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/schema/alert.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/schema/alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 class AlertType(str, enum.Enum):
     """Supported Alert types"""
 
     PERFORMANCE = 'performance'
     DATA_INTEGRITY = 'data_integrity'
     DATA_DRIFT = 'drift'
     SERVICE_METRICS = 'service_metrics'
+    STATISTIC = 'statistic'
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}.{self.name}'
 
 
 @enum.unique
 class Metric(str, enum.Enum):
@@ -56,14 +57,17 @@
     # Ranking
     MAP = 'map'
     MEAN_NDCG = 'mean_ndcg'
 
     ## Service Metrics
     TRAFFIC = 'Traffic'
 
+    ## Statistic
+    AVERAGE = 'average'
+
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}.{self.name}'
 
 
 @enum.unique
 class BinSize(enum.IntEnum):
     """Bin Size values in millisecs Alerts can be set on"""
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/schema/dataset.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/schema/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/schema/events.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/schema/events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/schema/model_deployment.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/schema/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/utils/decorators.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/utils/exceptions.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/utils/response_handler.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/utils/response_handler.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/v2/validators/dataset_validator.py` & `fiddler-client-2.0.0.dev1/fiddler/v2/validators/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler/validator.py` & `fiddler-client-2.0.0.dev1/fiddler/validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.8.0.dev1/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-2.0.0.dev1/fiddler_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 1.8.0.dev1
+Version: 2.0.0.dev1
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
         
@@ -22,33 +22,35 @@
         
         API Example Usage
         -------------
         Documentation for the API can be found [here](https://api.fiddler.ai/#introduction). For examples of interacting with our APIs, please check out our [Quick Start Guide](https://docs.fiddler.ai/quick-start/) as well as the work notebooks found on our [Samples Github](https://github.com/fiddler-labs/fiddler-samples).
         
         Version History
         -------------
-        ### 1.8.0
+        
+        ### 2.0.0
+          - #### **Removed**
+            - Following methods are removed
+              - register_model
+              - upload_model_package
+              - update_model
+              - trigger_pre_computation
+              - _trigger_model_predictions
+              - generate_sample_events
+              - list_teams
+              - list_project_roles
+              - list_org_roles
+              - unshare_project
+              - share_project
+              - process_avro
+              - process_csv
           - #### **Modifications**
             - Add `target_class_order` as a required field of `ModelInfo` object when `model_task` is `MULTICLASS_CLASSIFICATION`,
               `RANKING` or `BINARY_CLASSIFICATION`. Only applies for `BINARY_CLASSIFICATION` when target column is of type `CATEGORY`
-            - CURRENT_DATA_TYPE_VERSION increased to v1
-            - removed type conversion of possible_values
-        
-        
-        ### 1.7.3
-          - #### **Modification**
-            - Send row and column count information to dataset upload api
-        
-        ### 1.7.2
-          - #### **Modification**
-            - Bring back `WeightingParams` object
         
-        ### 1.7.1
-          - #### **Modification**
-            - Relaxed boto3 version constraint
         
         ### 1.7.0
           - #### **Removed**
             - Remove support for initializing fiddler client with version=1
             - Following methods are removed
               - get_segment_info
               - delete_segment
@@ -58,27 +60,27 @@
               - upload_segment
               - add_monitoring_config
               - publish_parquet_s3
               - publish_events_log
         
         ### 1.6.2
           - #### **Modifications**
-            - Make dataset_id a required field in add_model()
+            - Made dataset_id a required field in add_model()
             - Update max_inferred_cardinality to 100
           - #### **New Features**
             - New method for updating a model artifact `update_model_artifact`
         
         ### 1.5.3
           - #### **Modifications**
             - Fix add_model_artifact error for NLP models
             - Add model_info validation during add_model
         
         ### 1.5.2
           - #### **Modifications**
-            - Adds fix for self signed certificate not working by adding verify param to FiddlerApi
+            - Add fix for self signed certificate not working by adding verify param to FiddlerApi
         
         ### 1.5.1
           - #### **Modifications**
             - Fix in `violation_of_type` to include numpy dtypes such as `int64`
         
         ### 1.5.0
           - #### **New Features**
```

### Comparing `fiddler-client-1.8.0.dev1/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-2.0.0.dev1/fiddler_client.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,28 +19,14 @@
 fiddler/v1_v2_compat.py
 fiddler/validator.py
 fiddler/api/__init__.py
 fiddler/api/monitoring.py
 fiddler/api/publish_event.py
 fiddler/assets/__init__.py
 fiddler/assets/pg_reserved_words.py
-fiddler/file_processor/__init__.py
-fiddler/file_processor/src/__init__.py
-fiddler/file_processor/src/constants.py
-fiddler/file_processor/src/extractor.py
-fiddler/file_processor/src/facade.py
-fiddler/file_processor/src/file_workflow_executor.py
-fiddler/file_processor/src/processor.py
-fiddler/file_processor/src/utils.py
-fiddler/file_processor/tests/__init__.py
-fiddler/file_processor/tests/test_extractor.py
-fiddler/file_processor/tests/test_facade.py
-fiddler/file_processor/tests/test_file_processor.py
-fiddler/file_processor/tests/resources/__init__.py
-fiddler/file_processor/tests/resources/csvs/__init__.py
 fiddler/libs/__init__.py
 fiddler/libs/http_client.py
 fiddler/packtools/__init__.py
 fiddler/packtools/gem.py
 fiddler/packtools/keras_ig_helpers.py
 fiddler/packtools/project_attributions_helpers.py
 fiddler/packtools/template_model.py
@@ -89,8 +75,9 @@
 fiddler/v2/validators/dataset_validator.py
 fiddler_client.egg-info/PKG-INFO
 fiddler_client.egg-info/SOURCES.txt
 fiddler_client.egg-info/dependency_links.txt
 fiddler_client.egg-info/requires.txt
 fiddler_client.egg-info/top_level.txt
 tests/__init__.py
-tests/test_fiddler_api.py
+tests/test_fiddler_api.py
+tests/test_v1_v2_compat.py
```

### Comparing `fiddler-client-1.8.0.dev1/setup.py` & `fiddler-client-2.0.0.dev1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         'requests<3',
         'requests-toolbelt',
         'pandas>=1.2.5,<=1.5.3',
         'pyyaml',
         'packaging',
         'deepdiff',
         'boto3',
-        'fastavro',
         'importlib-resources',
         'Werkzeug',
         'pyarrow>=3.0.0',
         'deprecation==2.1.0',
         'pydantic>=1.9.0',
         'deprecated==1.2.13',
         'semver>=2,<3',
```

