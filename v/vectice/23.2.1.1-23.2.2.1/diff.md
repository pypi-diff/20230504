# Comparing `tmp/vectice-23.2.1.1.tar.gz` & `tmp/vectice-23.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-23.2.1.1.tar", last modified: Mon Apr 17 08:09:05 2023, max compression
+gzip compressed data, was "vectice-23.2.2.1.tar", last modified: Thu May  4 08:06:32 2023, max compression
```

## Comparing `vectice-23.2.1.1.tar` & `vectice-23.2.2.1.tar`

### file list

```diff
@@ -1,125 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.407174 vectice-23.2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 08:08:56.000000 vectice-23.2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-17 08:09:05.407174 vectice-23.2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 08:08:56.000000 vectice-23.2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-17 08:08:56.000000 vectice-23.2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 08:09:05.407174 vectice-23.2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-17 08:08:56.000000 vectice-23.2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.387174 vectice-23.2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.391174 vectice-23.2.1.1/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.395174 vectice-23.2.1.1/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.399174 vectice-23.2.1.1/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/file_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/s3_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/dataframe_column_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.395174 vectice-23.2.1.1/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 08:06:24.000000 vectice-23.2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-04 08:06:32.946823 vectice-23.2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 08:06:24.000000 vectice-23.2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 08:06:24.000000 vectice-23.2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 08:06:32.946823 vectice-23.2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-04 08:06:24.000000 vectice-23.2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.930823 vectice-23.2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.930823 vectice-23.2.2.1/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.934823 vectice-23.2.2.1/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.938823 vectice-23.2.2.1/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/dataframe_column_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22703 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.942823 vectice-23.2.2.1/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-04 08:06:24.000000 vectice-23.2.2.1/src/vectice/utils/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:06:32.930823 vectice-23.2.2.1/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 08:06:32.000000 vectice-23.2.2.1/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-23.2.1.1/LICENSE` & `vectice-23.2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/PKG-INFO` & `vectice-23.2.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.1.1
+Version: 23.2.2.1
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.1.1/setup.py` & `vectice-23.2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
             "pytest",
             "pytest-randomly",
             "coverage",
             "pytest-cov",
             "scikit-learn<=0.24.2",
             "testcontainers",
             "testbook",
+            "db-dtypes>=1.1.1",
         ],
         "gcs": ["google-cloud-storage>=1.17.0", "google-cloud-bigquery"],
         "s3": ["boto3"],
     },
     classifiers=[
         "Topic :: Internet",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `vectice-23.2.1.1/src/vectice/__init__.py` & `vectice-23.2.2.1/src/vectice/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,23 +20,26 @@
 
 import warnings
 
 from vectice import api, models
 from vectice.__version__ import __version__
 from vectice.connection import Connection
 from vectice.models.dataset import Dataset
-from vectice.models.datasource.datawrapper.file_data_wrapper import FileDataWrapper
-from vectice.models.datasource.datawrapper.gcs_data_wrapper import GcsDataWrapper
-from vectice.models.datasource.datawrapper.s3_data_wrapper import S3DataWrapper
 from vectice.models.git_version import CodeSource
-from vectice.models.model import Model
-from vectice.models.resource.file_resource import FileResource
-from vectice.models.resource.gcs_resource import GCSResource
-from vectice.models.resource.metadata.base import DatasetSourceUsage, DatasetType
-from vectice.models.resource.s3_resource import S3Resource
+from vectice.models.model import Metric, Model, Property
+from vectice.models.resource import BigQueryResource, FileResource, GCSResource, Resource, S3Resource
+from vectice.models.resource.metadata import (
+    DatasetSourceOrigin,
+    DatasetSourceUsage,
+    DatasetType,
+    DBMetadata,
+    File,
+    FilesMetadata,
+    MetadataDB,
+)
 from vectice.utils.logging_utils import _configure_vectice_loggers, disable_logging
 
 connect = Connection.connect
 
 code_capture = True
 """Global code capture flag, enabled by default.
 
@@ -66,20 +69,26 @@
 version = __version__
 
 __all__ = [
     "api",
     "models",
     "version",
     "connect",
+    "BigQueryResource",
+    "Resource",
     "FileResource",
     "GCSResource",
     "S3Resource",
     "DatasetSourceUsage",
+    "DatasetSourceOrigin",
+    "DBMetadata",
+    "FilesMetadata",
+    "File",
+    "MetadataDB",
     "DatasetType",
     "silent",
     "Model",
+    "Metric",
+    "Property",
     "CodeSource",
     "Dataset",
-    "FileDataWrapper",
-    "GcsDataWrapper",
-    "S3DataWrapper",
 ]
```

### Comparing `vectice-23.2.1.1/src/vectice/api/__init__.py` & `vectice-23.2.2.1/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/_auth.py` & `vectice-23.2.2.1/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/_utils.py` & `vectice-23.2.2.1/src/vectice/api/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     Raises:
         ValueError: When no arguments are given.
 
     Returns:
         A list of configuration items.
     """
     if len(args) == 0:
-        raise ValueError("At least one argument must be provided to read.")
+        raise ValueError(
+            "No configuration arguments found.  At least one argument must be provided to connect to Vectice."
+        )
     config: dict[str, str | None] = {
         **dotenv_values(find_dotenv(".vectice")),
         **dotenv_values(find_dotenv(".env")),
         **os.environ,
     }
     return [config.get(key) for key in args]
```

### Comparing `vectice-23.2.1.1/src/vectice/api/attachment.py` & `vectice-23.2.2.1/src/vectice/api/attachment.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,98 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, Any, BinaryIO, NoReturn
 
 from vectice.api.http_error_handlers import InvalidReferenceError
 from vectice.api.json import AttachmentOutput, ModelVersionOutput, PagedResponse
+from vectice.api.json.dataset_version import DatasetVersionOutput
 from vectice.api.rest_api import HttpError, RestApi
 
 if TYPE_CHECKING:
     from io import BytesIO
 
     from requests import Response
 
 
 MODEL_VERSION = "model version"
+DATASET_VERSION = "dataset version"
 
 
 _logger = logging.getLogger(__name__)
 
 
 class AttachmentApi(RestApi):
     def _generate_model_url_and_id(self, model_version: ModelVersionOutput) -> tuple[str, str | None]:
         try:
             model_name = model_version.model.name
             version_name = model_version.name
-            url = self._build_url(model_version.model.project_id, model_version.id)
+            url = self._build_url(model_version.model.project_id, model_version.id, "modelversion")
             model_repr = f"Model(name='{model_name}', version='{version_name}')"
             return url, model_repr
         except HttpError as e:
             self._handle_http_error(e, model_version)
 
+    def _generate_dataset_url_and_id(self, dataset_version: DatasetVersionOutput) -> tuple[str, str | None]:
+        try:
+            dataset_name = dataset_version.dataset.name
+            version_name = dataset_version.name
+            url = self._build_url(dataset_version.dataset.project_id, dataset_version.id, "datasetversion")
+            dataset_repr = f"Dataset(name='{dataset_name}', version='{version_name}')"
+            return url, dataset_repr
+        except HttpError as e:
+            self._handle_http_error(e, dataset_version)
+
+    def _generate_version_url_and_id(
+        self, version: ModelVersionOutput | DatasetVersionOutput
+    ) -> tuple[str, str | None]:
+        if isinstance(version, ModelVersionOutput):
+            return self._generate_model_url_and_id(version)
+
+        return self._generate_dataset_url_and_id(version)
+
     @staticmethod
-    def _build_url(project_id: int, model_version_id: int) -> str:
-        return f"/metadata/project/{project_id}/entityfiles/modelversion/{model_version_id}"
+    def _build_url(project_id: int, version: int, type: str) -> str:
+        return f"/metadata/project/{project_id}/entityfiles/{type}/{version}"
 
     def post_attachment(
-        self, files: list[tuple[str, tuple[str, BinaryIO]]], model_version: ModelVersionOutput
+        self, files: list[tuple[str, tuple[str, BinaryIO]]], version: ModelVersionOutput | DatasetVersionOutput
     ) -> list[dict]:
         entity_files = []
         try:
-            url, model_repr = self._generate_model_url_and_id(model_version)
+            url, repr = self._generate_version_url_and_id(version)
             if len(files) == 1:
                 response = self._post_attachments(url, files)
                 if response:
                     entity_files.append(response.json())
-                _logger.debug(f"Attachment with name: {files[0][1][0]} successfully attached to {model_repr}.")
+                _logger.debug(f"Attachment with name: {files[0][1][0]} successfully attached to {repr}.")
             elif len(files) > 1:
                 for file in files:
                     response = self._post_attachments(url, [file])
                     if response:
                         entity_files.append(response.json())
-                _logger.debug(
-                    f"Attachments with names: {[f[1][0] for f in files]} successfully attached to {model_repr}."
-                )
+                _logger.debug(f"Attachments with names: {[f[1][0] for f in files]} successfully attached to {repr}.")
             return entity_files
         except HttpError as e:
-            self._handle_http_error(e, model_version)
+            self._handle_http_error(e, version)
 
     def post_model_predictor(self, model_type: str, model_content: BytesIO, model_version: ModelVersionOutput) -> None:
         url, model_repr = self._generate_model_url_and_id(model_version)
         url += f"?modelFramework={model_type}"
         attachment = ("file", ("model_pickle", model_content))
         self._post_attachments(url, [attachment])
         _logger.info(f"Model {model_type} successfully attached to {model_repr}.")
 
     def _identify_object(self, code_version_id: int | None = None, phase_id: int | None = None) -> tuple:
         if phase_id:
             return "phase", phase_id
         elif code_version_id:
             return "codeversion", code_version_id
         else:
-            raise ValueError("No id provided for create attachment!")
+            raise ValueError("No ID was provided for create attachment.")
 
     def create_attachments(
         self,
         files: list[tuple[str, tuple[str, Any]]],
         project_id: int,
         code_version_id: int | None = None,
         phase_id: int | None = None,
@@ -99,22 +117,22 @@
         try:
             return self._get_attachment(
                 f"/metadata/project/{project_id}/entityfiles/codeversion/{code_version_id}/{file_id}"
             )
         except HttpError as e:
             self._handle_code_version_error(e, code_version_id)
 
-    def list_attachments(self, model_version: ModelVersionOutput) -> PagedResponse[AttachmentOutput]:
+    def list_attachments(self, version: ModelVersionOutput | DatasetVersionOutput) -> PagedResponse[AttachmentOutput]:
         try:
-            url, model_repr = self._generate_model_url_and_id(model_version)
+            url, repr = self._generate_version_url_and_id(version)
             if url is None:
-                raise InvalidReferenceError(MODEL_VERSION, model_version.id)
+                raise InvalidReferenceError(MODEL_VERSION, version.id)
             attachments = self._list_attachments(url)
         except HttpError as e:
-            self._handle_http_error(e, model_version)
+            self._handle_http_error(e, version)
         return PagedResponse(
             item_cls=AttachmentOutput,
             total=len(attachments),
             page={},
             items=attachments,
         )
 
@@ -143,12 +161,13 @@
         return PagedResponse(
             item_cls=AttachmentOutput,
             total=len(attachments),
             page={},
             items=attachments,
         )
 
-    def _handle_http_error(self, error: HttpError, model_version: ModelVersionOutput) -> NoReturn:
-        self._httpErrorHandler.handle_get_http_error(error, MODEL_VERSION, model_version.id)
+    def _handle_http_error(self, error: HttpError, version: ModelVersionOutput | DatasetVersionOutput) -> NoReturn:
+        ref_type = MODEL_VERSION if isinstance(version, ModelVersionOutput) else DATASET_VERSION
+        self._httpErrorHandler.handle_get_http_error(error, ref_type, version.id)
 
     def _handle_code_version_error(self, error: HttpError, code_version_id: int) -> NoReturn:
         self._httpErrorHandler.handle_get_http_error(error, "code version", code_version_id)
```

### Comparing `vectice-23.2.1.1/src/vectice/api/client.py` & `vectice-23.2.2.1/src/vectice/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     Page,
     PagedResponse,
     ProjectInput,
     PropertyInput,
     StepOutput,
 )
 from vectice.api.json.dataset_register import DatasetRegisterInput, DatasetRegisterOutput
+from vectice.api.json.dataset_version import DatasetVersionOutput
 from vectice.api.json.metric import MetricInput
 from vectice.api.json.step import StepUpdateInput
 from vectice.api.last_assets import LastAssetApi
 from vectice.api.phase import PhaseApi
 from vectice.api.project import ProjectApi
 from vectice.api.step import StepApi
 from vectice.api.version import VersionApi
@@ -279,27 +280,27 @@
             project_id: The project id associated to the code version id.
 
         Returns:
             The JSON structure.
         """
         return AttachmentApi(self.auth).create_attachments(files, project_id, code_version_id=code_version_id)
 
-    def create_model_attachments(
-        self, files: list[tuple[str, tuple[str, BinaryIO]]], model_version: ModelVersionOutput
+    def create_version_attachments(
+        self, files: list[tuple[str, tuple[str, BinaryIO]]], version: ModelVersionOutput | DatasetVersionOutput
     ):
         """Create an attachment.
 
         Parameters:
             files: The paths to the files to attach.
-            model_version: The model version to attach files to.
+            version: The version to attach files to.
 
         Returns:
             The JSON structure.
         """
-        return AttachmentApi(self.auth).post_attachment(files, model_version)
+        return AttachmentApi(self.auth).post_attachment(files, version)
 
     def create_phase_attachments(
         self, files: list[tuple[str, tuple[str, BytesIO | IOBase]]], phase_id: int, project_id: int
     ) -> list[dict]:
         """Create an attachment.
 
         Parameters:
@@ -321,24 +322,24 @@
             model_version: The model version to attach files to.
 
         Returns:
             The JSON structure.
         """
         return AttachmentApi(self.auth).post_model_predictor(model_type, model_content, model_version)
 
-    def list_attachments(self, model_version: ModelVersionOutput) -> PagedResponse[AttachmentOutput]:
+    def list_attachments(self, version: ModelVersionOutput | DatasetVersionOutput) -> PagedResponse[AttachmentOutput]:
         """List the attachments of an artifact.
 
         Parameters:
-            model_version: The model version to list attachments from.
+            version: The version to list attachments from.
 
         Returns:
             The attachments of an artifact.
         """
-        return AttachmentApi(self.auth).list_attachments(model_version)
+        return AttachmentApi(self.auth).list_attachments(version)
 
     def list_code_attachments(self, code_version_id: int, project_id: int) -> PagedResponse[AttachmentOutput]:
         """List the attachments of a code version.
 
         Parameters:
             code_version_id: The id of the code version to list attachments from.
             project_id: The id of the project the code version belongs to.
@@ -398,15 +399,15 @@
                     return step
             raise StepIdError(step_reference)
         elif isinstance(step_reference, str):
             for step in steps:
                 if step.name == step_reference:
                     return step
             raise StepNameError(step_reference)
-        raise ValueError(f"No such step reference '{step_reference}' exists in the phase '{phase_id}'")
+        raise ValueError(f"Step reference '{step_reference}' does not exists in the phase '{phase_id}'")
 
     def get_step_by_name(self, step_reference: str, iteration_id: int) -> StepOutput:
         return StepApi(self._gql_client, self.auth).get_step(step_reference, iteration_id)
 
     def list_steps(
         self,
         phase_id: int,
@@ -469,15 +470,15 @@
         if dataset._has_bigquery_resource and self.is_feature_flag_enabled("bigquery-dataset-source") is False:
             raise VecticeException(DISABLED_FEATURE_FLAG_MESSAGE.format("bigquery-dataset-source"))
 
         if dataset._has_dataframe is True and self.is_feature_flag_enabled("dataset-dataframe") is False:
             raise VecticeException(DISABLED_FEATURE_FLAG_MESSAGE.format("dataset-dataframe"))
 
         name = self.get_dataset_name(dataset)
-        derived_from = self.get_dataset_derived_from(dataset)
+        derived_from = self.get_derived_from(dataset)
         if isinstance(dataset.resource, tuple):
             # modeling dataset
             metadata_asdict = [data_source.metadata.asdict() for data_source in dataset.resource if data_source]
         else:
             metadata_asdict = [dataset.resource.metadata.asdict()]
 
         properties = (
@@ -497,28 +498,28 @@
         return dataset_register_output
 
     @staticmethod
     def get_dataset_name(dataset: Dataset) -> str:
         return f"dataset {datetime.time}" if dataset.name is None else dataset.name
 
     @staticmethod
-    def get_dataset_derived_from(dataset: Dataset) -> list[int]:
-        return [] if dataset.derived_from is None else dataset.derived_from
+    def get_derived_from(obj: Dataset | Model) -> list[int]:
+        return [] if obj.derived_from is None else obj.derived_from
 
     def register_dataset(
         self,
         dataset_register_input: DatasetRegisterInput,
         project_id: int | None = None,
         phase_id: int | None = None,
         iteration_id: int | None = None,
     ) -> DatasetRegisterOutput:
         data: DatasetRegisterOutput = GqlDatasetApi(self._gql_client, self.auth).register_dataset(
             dataset_register_input, project_id, phase_id, iteration_id
         )
-        _logger.info(
+        _logger.debug(
             f"Successfully registered Dataset("
             f"name='{dataset_register_input.name}', "
             f"id={data['datasetVersion']['id']}, "
             f"version='{data['datasetVersion']['name']}', "
             f"type={dataset_register_input.type})."
         )
         return data
@@ -565,38 +566,37 @@
     def register_model(
         self,
         model: Model,
         project_id: int,
         phase_id: int | None = None,
         iteration_id: int | None = None,
         code_version_id: int | None = None,
-        derived_from: list[int] | None = None,
     ) -> ModelRegisterOutput:
         """Register a model.
 
         Parameters:
             model: The model to register
             project_id: The project ID
             phase_id: The phase ID
             iteration_id: The iteration ID
             code_version_id: The code version ID
-            derived_from: The IDs of datasets the model is derived from
 
         Returns:
             The registered model.
         """
         metrics = [vars(MetricInput(metric.key, metric.value)) for metric in model.metrics] if model.metrics else None
         properties = (
             [vars(PropertyInput(prop.key, prop.value)) for prop in model.properties] if model.properties else None
         )
+        derived_from = self.get_derived_from(model)
         model_register_input = ModelRegisterInput(
             name=model.name,
             modelType=ModelType.OTHER.value,
             status=ModelVersionStatus.EXPERIMENTATION.value,
-            inputs=derived_from or [],
+            inputs=derived_from,
             metrics=metrics,
             properties=properties,
             algorithmName=model.technique,
             framework=model.library,
             codeVersionId=code_version_id,
         )
         return GqlModelApi(self._gql_client, self.auth).register_model(
```

### Comparing `vectice-23.2.1.1/src/vectice/api/gql_api.py` & `vectice-23.2.2.1/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/gql_code.py` & `vectice-23.2.2.1/src/vectice/api/gql_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             kw = "codeId:$codeId"
         elif isinstance(code, str) and project_id:
             gql_query = "getCodeByName"
             variable_types = "$name:String!,$projectId:VecticeId!"
             variables = {"name": code, "projectId": project_id}  # type: ignore[dict-item]
             kw = "name:$name,projectId:$projectId"
         else:
-            raise ValueError("string and parent id required.")
+            raise ValueError("Missing parameters: string and parent id required.")
         query = GqlApi.build_query(
             gql_query=gql_query, variable_types=variable_types, returns=_RETURNS, keyword_arguments=kw, query=True
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             phase_output: CodeOutput = Parser().parse_item(response[gql_query])
```

### Comparing `vectice-23.2.1.1/src/vectice/api/gql_code_version.py` & `vectice-23.2.2.1/src/vectice/api/gql_code_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             kw = "codeVersionId:$codeVersionId"
         elif isinstance(code_version, str) and code_id:
             gql_query = "getCodeVersionByName"
             variable_types = "$name:String!,$codeId:Float!"
             variables = {"name": code_version, "codeId": code_id}  # type: ignore[dict-item]
             kw = "name:$name,codeId:$codeId"
         else:
-            raise ValueError("string and parent id required.")
+            raise ValueError("Missing parameters: string and parent id required.")
         query = GqlApi.build_query(
             gql_query=gql_query, variable_types=variable_types, returns=_RETURNS, keyword_arguments=kw, query=True
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             phase_output: CodeVersionOutput = Parser().parse_item(response[gql_query])
```

### Comparing `vectice-23.2.1.1/src/vectice/api/gql_dataset.py` & `vectice-23.2.2.1/src/vectice/api/gql_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 _logger = logging.getLogger(__name__)
 
 # TODO JobRun for lineages
 _RETURNS = """
             datasetVersion {
                           id
                           name
+                          dataSet {
+                            name
+                            projectId
+                          }
             }
             useExistingDataset
             useExistingVersion
             __typename
             """
 
 
@@ -45,15 +49,15 @@
             kw = "projectId:$projectId,phaseId:$phaseId,iterationId:$iterationId,data:$data"
             variables = {"projectId": project_id, "phaseId": phase_id, "iterationId": iteration_id, "data": data}
         elif project_id:
             variable_types = "$projectId:VecticeId!,$data:DatasetRegisterInput!"
             kw = "projectId:$projectId,data:$data"
             variables = {"projectId": project_id, "data": data}
         else:
-            raise RuntimeError("The provided parent child ids do not match!")
+            raise RuntimeError("The provided parent child ids do not match.")
 
         query = GqlApi.build_query(
             gql_query="registerDataset",
             variable_types=variable_types,
             returns=_RETURNS,
             keyword_arguments=kw,
             query=False,
```

### Comparing `vectice-23.2.1.1/src/vectice/api/gql_feature_flag.py` & `vectice-23.2.2.1/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/gql_model.py` & `vectice-23.2.2.1/src/vectice/api/gql_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from gql import gql
+from gql.transport.exceptions import TransportQueryError
 
 from vectice.api.gql_api import GqlApi, Parser
 
 if TYPE_CHECKING:
     from vectice.api.json.model_register import ModelRegisterInput, ModelRegisterOutput
 
 _RETURNS = """
@@ -52,10 +53,13 @@
             gql_query=query_name,
             variable_types=variable_types,
             returns=_RETURNS,
             keyword_arguments=kw,
             query=False,
         )
         query_built = gql(query)
-        response = self.execute(query_built, variables)
-        model_output: ModelRegisterOutput = Parser().parse_item(response[query_name])
-        return model_output
+        try:
+            response = self.execute(query_built, variables)
+            model_output: ModelRegisterOutput = Parser().parse_item(response[query_name])
+            return model_output
+        except TransportQueryError as e:
+            self._error_handler.handle_post_gql_error(e, "model", "register model")
```

### Comparing `vectice-23.2.1.1/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.2.2.1/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/http_error.py` & `vectice-23.2.2.1/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/http_error_handlers.py` & `vectice-23.2.2.1/src/vectice/api/http_error_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 class InvalidReferenceError(ValueError):
     """When an incorrect value type is passed at the client level."""
 
     def __init__(self, reference_type: str, value: Any) -> None:
         super().__init__(
-            f"The {reference_type} reference is invalid. Please check the provided value. "
-            + "it should be a string or a number. "
+            f"The {reference_type} reference is invalid."
+            + "Please check the provided value as it should be a string or a number."
             + f"Provided value is {value} ({type(value)})"
         )
 
 
 class MissingReferenceError(ValueError):
     """When a value is missing at the client level."""
 
@@ -46,15 +46,15 @@
 
     def handle_code(self, e: HttpError, reference_type: str, reference: str | int) -> NoReturn:
         if e.code == 404:
             raise BadReferenceFactory.get_reference(reference_type, reference)
         elif e.code == 401:
             raise ConnectionRefusedError(BAD_OR_MISSING_CREDENTIALS_ERROR_MESSAGE)
         elif e.code == 403:
-            raise PermissionError(f"Missing rights to access this {reference_type}")
+            raise PermissionError(f"Missing permissions to access this {reference_type}")
         raise RuntimeError(f"Can not access {reference_type}: {e.reason}")
 
     def handle_get_http_error(self, e: HttpError, reference_type: str, reference: str | int) -> NoReturn:
         self.handle_code(e, reference_type, reference)
 
     def handle_put_http_error(self, e: HttpError, reference_type: str, reference: str | int) -> NoReturn:
         self.handle_code(e, reference_type, reference)
@@ -62,30 +62,30 @@
     def handle_delete_http_error(self, e: HttpError, reference_type: str, reference: str | int) -> NoReturn:
         self.handle_code(e, reference_type, reference)
 
     def handle_post_http_error(self, e: HttpError, reference_type: str, action: str = "create") -> NoReturn:
         if e.code == 401:
             raise ConnectionRefusedError(BAD_OR_MISSING_CREDENTIALS_ERROR_MESSAGE)
         elif e.code == 403:
-            raise PermissionError(f"Missing rights to access this {reference_type}")
+            raise PermissionError(f"Missing permissions to access this {reference_type}")
         elif e.code == 400:
             raise RuntimeError(f"Can not {action} {reference_type}: {e.reason}")
         raise RuntimeError(f"Unexpected error: {e.reason}")
 
     def handle_post_gql_error(self, error: TransportQueryError, reference_type: str, reference: str | int) -> NoReturn:
         try:
             status_code = error.errors[0]["extensions"]["exception"]["status"]  # type: ignore[index]
         except KeyError:
             status_code = -1
         if status_code == 404:
             raise BadReferenceFactory.get_reference(reference_type, reference)
         elif status_code == 401:
             raise ConnectionRefusedError(BAD_OR_MISSING_CREDENTIALS_ERROR_MESSAGE)
         elif status_code == 403:
-            raise PermissionError(f"Missing rights to access this {reference_type}")
+            raise PermissionError(f"Missing permissions to access this {reference_type}")
         elif status_code == 400 or status_code == 412:
             # backend always adds a "message" to the response
             message = error.errors[0]["message"]  # type: ignore
             raise VecticeException(f"{reference_type}: {message}")
         raise self._graphql_error_formatter(error) from error
 
 
@@ -182,20 +182,24 @@
 class PhaseIdError(VecticeBaseNameError):
     def __init__(self, value: int):
         super().__init__(f"The phase with id '{value}' is unknown.")
 
 
 class StepNameError(VecticeBaseNameError):
     def __init__(self, value: str):
-        super().__init__(f"The step with name '{value}' is unknown.")
+        super().__init__(
+            f"The step with name '{value}' is unknown. Use <your iteration>.list_steps() method to find step names."
+        )
 
 
 class StepIdError(VecticeBaseNameError):
     def __init__(self, value: int):
-        super().__init__(f"The step with id '{value}' is unknown.")
+        super().__init__(
+            f"The step with id '{value}' is unknown. Use <your iteration>.list_steps() method to find step ids."
+        )
 
 
 class IterationIdError(VecticeBaseNameError):
     def __init__(self, value: int):
         super().__init__(f"The iteration with id '{value}' is unknown.")
 
 
@@ -208,8 +212,8 @@
     def __init__(self, value: str):
         super().__init__(f"The iteration with name '{value}' is unknown.")
 
 
 class NoStepsInPhaseError(VecticeBaseNameError):
     def __init__(self, value: str | int):
         ref = f"with id '{value}'" if isinstance(value, int) else f"'{value}'"
-        super().__init__(f"There are no steps in the phase {ref}.")
+        super().__init__(f"There are no steps in the phase {ref}. Must create steps for this phase in the UI.")
```

### Comparing `vectice-23.2.1.1/src/vectice/api/iteration.py` & `vectice-23.2.2.1/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/__init__.py` & `vectice-23.2.2.1/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/artifact_version.py` & `vectice-23.2.2.1/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/code.py` & `vectice-23.2.2.1/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/code_version.py` & `vectice-23.2.2.1/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/files_metadata.py` & `vectice-23.2.2.1/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/iteration.py` & `vectice-23.2.2.1/src/vectice/api/json/iteration.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,16 +63,33 @@
         return int(self["id"])
 
     @property
     def type(self) -> str:
         return str(self["type"])
 
     @property
-    def entity_file_id(self) -> int:
-        return int(self["entityFileId"])
+    def dataset_version_id(self) -> int | None:
+        if self.get("datasetVersionId"):
+            return int(self["datasetVersionId"])
+        else:
+            return None
+
+    @property
+    def model_version_id(self) -> int | None:
+        if self.get("modelVersionId"):
+            return int(self["modelVersionId"])
+        else:
+            return None
+
+    @property
+    def entity_file_id(self) -> int | None:
+        if self.get("entityFileId"):
+            return int(self["entityFileId"])
+        else:
+            return None
 
 
 class IterationInput(dict):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     from vectice.api.json.step import StepInput
```

### Comparing `vectice-23.2.1.1/src/vectice/api/json/last_assets.py` & `vectice-23.2.2.1/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/metric.py` & `vectice-23.2.2.1/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/model.py` & `vectice-23.2.2.1/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/model_register.py` & `vectice-23.2.2.1/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/model_version.py` & `vectice-23.2.2.1/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/paged_response.py` & `vectice-23.2.2.1/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/phase.py` & `vectice-23.2.2.1/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/project.py` & `vectice-23.2.2.1/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/property.py` & `vectice-23.2.2.1/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/public_config.py` & `vectice-23.2.2.1/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/step.py` & `vectice-23.2.2.1/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/json/workspace.py` & `vectice-23.2.2.1/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/last_assets.py` & `vectice-23.2.2.1/src/vectice/api/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/phase.py` & `vectice-23.2.2.1/src/vectice/api/phase.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             kw = "id:$id"
         elif isinstance(phase, str) and parent_id:
             gql_query = "getPhaseByName"
             variable_types = "$name:String!,$parentId:VecticeId!"
             variables = {"name": phase, "parentId": parent_id}  # type: ignore[dict-item]
             kw = "name:$name,parentId:$parentId"
         else:
-            raise ValueError("string and parent id required.")
+            raise ValueError("Missing parameters: string and parent id required.")
         query = GqlApi.build_query(
             gql_query=gql_query, variable_types=variable_types, returns=_RETURNS, keyword_arguments=kw, query=True
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             phase_output: PhaseOutput = Parser().parse_item(response[gql_query])
```

### Comparing `vectice-23.2.1.1/src/vectice/api/project.py` & `vectice-23.2.2.1/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/rest_api.py` & `vectice-23.2.2.1/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/step.py` & `vectice-23.2.2.1/src/vectice/api/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     def get_step(self, step: str, iteration_id: int) -> StepOutput:
         if isinstance(step, str) and iteration_id:
             gql_query = "getStepByName"
             variable_types = "$name:String!,$parentId:VecticeId!"
             variables = {"name": step, "parentId": iteration_id}
             kw = "name:$name,parentId:$parentId"
         else:
-            raise ValueError("string and parent id required.")
+            raise ValueError("Missing parameters: string and parent id required.")
         query = GqlApi.build_query(
             gql_query=gql_query, variable_types=variable_types, returns=_RETURNS, keyword_arguments=kw, query=True
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             step_output: StepOutput = Parser().parse_item(response[gql_query])
```

### Comparing `vectice-23.2.1.1/src/vectice/api/version.py` & `vectice-23.2.2.1/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/api/workspace.py` & `vectice-23.2.2.1/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/connection.py` & `vectice-23.2.2.1/src/vectice/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,21 +132,29 @@
 
         Returns:
             The desired workspace.
         """
         output = self._client.get_workspace(workspace)
         result = Workspace(output.id, output.name, output.description)
         result.__post_init__(self._client, self)
+        logging_output = dedent(
+            f"""
+                        Workspace {result.name!r} successfully retrieved."
+
+                        For quick access to the workspace in the Vectice web app, visit:
+                        {self._client.auth._API_BASE_URL}/workspace/dashboard/project-progress?w={result.id}"""
+        ).lstrip()
+        _logger.info(logging_output)
         return result
 
     def list_workspaces(self) -> None:
-        """List the workspaces to which this connection has access and log the workspaces in a tabular format.
+        """Prints a list of workspaces in a tabular format, limited to the first 10 items. A link is provided to view the remaining workspaces.
 
         Returns:
-            The workspaces to which this connection has access.
+            None
         """
         workspace_outputs = self._client.list_workspaces().list
         user_name, _ = _get_last_user_and_default_workspace(self._client)
 
         rich_table = Table(expand=True, show_edge=False)
 
         rich_table.add_column("workspace id", justify="left", no_wrap=True, min_width=4, max_width=10)
@@ -154,19 +162,22 @@
         rich_table.add_column("description", justify="left", no_wrap=True, max_width=50)
 
         for count, workspace in enumerate(workspace_outputs, 1):
             if count > 10:
                 break
             rich_table.add_row(str(workspace.id), workspace.name, format_description(workspace.description))
 
-        description = f"""There are {len(workspace_outputs)} workspaces."""
+        description = dedent(
+            f"""
+        There are {len(workspace_outputs)} workspaces and a maximum of 10 workspaces are displayed in the table below:"""
+        ).lstrip()
         tips = dedent(
             """
-        >> To access your personal workspace, use connection.my_workspace or connect.workspaces[0]
-        >> To access a specific workspace, use connection.workspace(Workspace ID)"""
+        To access your personal workspace, use \033[1mconnection\033[0m.my_workspace
+        To access a specific workspace, use \033[1mconnection\033[0m.workspace(Workspace ID)"""
         ).lstrip()
         link = dedent(
             f"""
         For quick access to the list of workspaces in the Vectice web app, visit:
         {self._client.auth._API_BASE_URL}/workspaces"""
         ).lstrip()
         _temp_print(description)
```

### Comparing `vectice-23.2.1.1/src/vectice/models/__init__.py` & `vectice-23.2.2.1/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/attachment_container.py` & `vectice-23.2.2.1/src/vectice/models/attachment_container.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,69 @@
 from __future__ import annotations
 
 import io
 import logging
 import os
 from typing import TYPE_CHECKING, BinaryIO, List
 
+from vectice.api.json.dataset_version import DatasetVersionOutput
 from vectice.api.json.model_version import ModelVersionOutput
 
 if TYPE_CHECKING:
     from vectice.api import Client
 
 _logger = logging.getLogger(__name__)
 
 FILE_PATH_DOES_NOT_EXIST_ERROR_MESSAGE = "The file path '%s' is not valid. The file does not exist."
 
 
 class AttachmentContainer:
-    def __init__(self, model_version: ModelVersionOutput, client: Client):
+    def __init__(self, version: ModelVersionOutput | DatasetVersionOutput, client: Client):
         self._client = client
-        self._model_version = model_version
-        self._id = model_version.id
-        self._name = model_version.name
+        self._version = version
+        self._id = version.id
+        self._name = version.name
 
     @property
-    def model_version(self):
-        return self._model_version
+    def version(self):
+        return self._version
 
     @property
     def name(self):
         return self._name
 
     @property
     def id(self):
         return self._id
 
-    def list_attachments(self) -> list[str]:
-        """List the names of the entity's attachments.
-
-        Returns:
-            The names of the entity's attachments.
-        """
-        attachments = self._client.list_attachments(self.model_version).list
-        return [attachment.fileName for attachment in attachments]
-
     def add_attachments(self, file_paths: str | list[str]):
         """Add an attachment or set of attachments to the entity.
 
         Parameters:
             file_paths: The paths of the attachment(s).
 
         Returns:
             A list of dictionaries describing the attachments.
         """
-        attached_files = self.list_attachments()
         file_paths = [file_paths] if isinstance(file_paths, str) else file_paths
-        attachments = self._add_files_to_attachments(file_paths, attached_files)
+        attachments = self._add_files_to_attachments(file_paths)
         try:
-            return self._client.create_model_attachments(attachments, self.model_version)
+            return self._client.create_version_attachments(attachments, self._version)
         finally:
             self._close_attached_files(attachments)
 
-    def _add_files_to_attachments(
-        self, file_paths: list[str], attached_files: list[str]
-    ) -> list[tuple[str, tuple[str, BinaryIO]]]:
+    def _add_files_to_attachments(self, file_paths: list[str]) -> list[tuple[str, tuple[str, BinaryIO]]]:
         attachments: List[tuple[str, tuple[str, BinaryIO]]] = []
         for file_path in file_paths:
             if not os.path.exists(file_path):
                 raise ValueError(FILE_PATH_DOES_NOT_EXIST_ERROR_MESSAGE % file_path)
             curr_file = ("file", (file_path, open(file_path, "rb")))
             attachments.append(curr_file)
-            file_name = file_path.split("/")[-1]
-            if file_name in attached_files:
-                raise RuntimeError(f"'{file_paths}' is already attached to '{self.name}'")
         return attachments
 
     def _close_attached_files(self, attachments: list[tuple[str, tuple[str, BinaryIO]]]) -> None:
         for attachment in attachments:
             attachment[1][1].close()
 
     def add_serialized_model(self, model_type: str, model_content: bytes):
-        self._client.create_model_predictor(model_type, io.BytesIO(model_content), self.model_version)
+        if isinstance(self._version, ModelVersionOutput):
+            self._client.create_model_predictor(model_type, io.BytesIO(model_content), self._version)
```

### Comparing `vectice-23.2.1.1/src/vectice/models/dataset.py` & `vectice-23.2.2.1/src/vectice/models/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
 
-from pandas import DataFrame
-
 from vectice.models.property import Property
 from vectice.models.resource.base import Resource
 from vectice.models.resource.bigquery_resource import BigQueryResource
 from vectice.models.resource.metadata.base import DatasetSourceUsage, DatasetType
-from vectice.models.resource.metadata.db_metadata import DBMetadata
-from vectice.models.resource.metadata.files_metadata import FilesMetadata
-from vectice.models.resource.metadata.source import Source
 
 _logger = logging.getLogger(__name__)
 
 
 class Dataset:
     def __init__(
         self,
         type: DatasetType,
         name: str | None = None,
         resource: Resource | None = None,
         training_resource: Resource | None = None,
         testing_resource: Resource | None = None,
         validation_resource: Resource | None = None,
         derived_from: list[int | Dataset] | None = None,
-        dataframe: DataFrame | None = None,
-        training_dataframe: DataFrame | None = None,
-        testing_dataframe: DataFrame | None = None,
-        validation_dataframe: DataFrame | None = None,
-        # attachments: str | list[str] | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
+        attachments: str | list[str] | None = None,
     ):
         """Initialize a dataset.
 
         Users should not instantiate a dataset directly but rather use the provided static methods
         [`origin()`][vectice.models.dataset.Dataset.origin],
         [`clean()`][vectice.models.dataset.Dataset.clean], and
         [`modeling()`][vectice.models.dataset.Dataset.modeling].
@@ -44,19 +35,15 @@
             type: The type of dataset.
             name: The name of the dataset.
             resource: A single resource (for origin and clean datasets).
             training_resource: The resource for the training set (for modeling datasets).
             testing_resource: The resource for the testing set (for modeling datasets).
             validation_resource: The resource for the validation set (optional, for modeling datasets).
             derived_from: A list of datasets (or ids) from which this dataset is derived.
-            dataframe: A pandas dataframe for clean and origin datasets.
-            training_dataframe: A pandas dataframe for modeling dataset.
-            testing_dataframe: A pandas dataframe for modeling dataset.
-            validation_dataframe: A pandas dataframe for modeling dataset.
-            properties: A dict, for example `{"folds": 32}`.
+            attachments: Path of a file that will be attached to the step along with the dataset.
         """
         derived_from_ids = []
         for df in derived_from or []:
             if isinstance(df, Dataset):
                 if df.latest_version_id is None:
                     raise ValueError(
                         f"Dataset '{df.name}' does not have a version id. "
@@ -70,15 +57,15 @@
         self._resource = resource
         self._training_resource = training_resource
         self._testing_resource = testing_resource
         self._validation_resource = validation_resource
         self._derived_from = derived_from_ids
         self._latest_version_id: int | None = None
         self._properties = self._format_properties(properties) if properties else None
-        # self._attachments = self._format_attachments(attachments) if attachments else None
+        self._attachments = self._format_attachments(attachments) if attachments else None
 
         if self._type is DatasetType.MODELING:
             if self._training_resource is None or self._testing_resource is None:
                 raise ValueError("You cannot create a modeling dataset without both training and testing sets")
 
             self._training_resource.usage = DatasetSourceUsage.TRAINING
             self._testing_resource.usage = DatasetSourceUsage.TESTING
@@ -86,151 +73,130 @@
                 self._validation_resource.usage = DatasetSourceUsage.VALIDATION
 
         self._has_bigquery_resource = (
             isinstance(self._resource, BigQueryResource)
             or isinstance(self._training_resource, BigQueryResource)
             or isinstance(self._testing_resource, BigQueryResource)
             or isinstance(self._validation_resource, BigQueryResource)
-            or isinstance(self.resource, BigQueryResource)
         )
         self._has_dataframe = (
-            dataframe is not None
-            or training_dataframe is not None
-            or testing_dataframe is not None
-            or validation_dataframe is not None
-        )
-        self._fill_file_dataframe(
-            [
-                (resource, dataframe, "dataframe"),
-                (training_resource, training_dataframe, "training_dataframe"),
-                (testing_resource, testing_dataframe, "testing_dataframe"),
-                (validation_resource, validation_dataframe, "validation_dataframe"),
-            ]
+            (self._resource is not None and self._resource._dataframes is not None)
+            or (self._training_resource is not None and self._training_resource._dataframes is not None)
+            or (self._testing_resource is not None and self._testing_resource._dataframes is not None)
+            or (self._validation_resource is not None and self._validation_resource._dataframes is not None)
         )
 
     @staticmethod
     def origin(
         resource: Resource,
         name: str | None = None,
-        dataframe: DataFrame | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
-        # attachments: str | list[str] | None = None,
+        attachments: str | list[str] | None = None,
     ) -> Dataset:
         """Create an origin dataset.
 
         Examples:
             ```python
             from vectice import Dataset, FileResource
 
             dataset = Dataset.origin(
                 name="my origin dataset",
-                resource=FileResource(path="origin_dataset.csv"),
+                resource=FileResource(paths="origin_dataset.csv"),
             )
             ```
 
         Parameters:
             resource: The resource for the origin dataset.
             name: The name of the dataset.
-            dataframe: A pandas dataframe allowing vectice to compute more metadata about this dataset.
             properties: A dict, for example `{"folds": 32}`.
+            attachments: Path of a file that will be attached to the step along with the dataset.
         """
         return Dataset(
             type=DatasetType.ORIGIN,
             name=name,
             resource=resource,
-            dataframe=dataframe,
             properties=properties,
-            # attachments=attachments,
+            attachments=attachments,
         )
 
     @staticmethod
     def clean(
         resource: Resource,
         name: str | None = None,
         derived_from: list[int | Dataset] | None = None,
-        dataframe: DataFrame | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
-        # attachments: str | list[str] | None = None,
+        attachments: str | list[str] | None = None,
     ) -> Dataset:
         """Create a clean dataset.
 
         Examples:
             ```python
             from vectice import Dataset, FileResource
 
             dataset = Dataset.clean(
                 name="my clean dataset",
-                resource=FileResource(path="clean_dataset.csv"),
-                properties: A dict, for example `{"folds": 32}`.
+                resource=FileResource(paths="clean_dataset.csv"),
             )
             ```
 
         Parameters:
             resource: The resource for the clean dataset.
             name: The name of the dataset.
             derived_from: A list of datasets (or ids) from which this dataset is derived.
-            dataframe: A pandas dataframe allowing vectice to compute more metadata about this dataset.
+            properties: A dict, for example `{"folds": 32}`.
+            attachments: Path of a file that will be attached to the step along with the dataset.
         """
         return Dataset(
             type=DatasetType.CLEAN,
             name=name,
             resource=resource,
             derived_from=derived_from,
-            dataframe=dataframe,
             properties=properties,
-            # attachments=attachments,
+            attachments=attachments,
         )
 
     @staticmethod
     def modeling(
         training_resource: Resource,
         testing_resource: Resource,
         validation_resource: Resource | None = None,
         name: str | None = None,
-        training_dataframe: DataFrame | None = None,
-        testing_dataframe: DataFrame | None = None,
-        validation_dataframe: DataFrame | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
-        # attachments: str | list[str] | None = None,
+        attachments: str | list[str] | None = None,
     ) -> Dataset:
         """Create a modeling dataset.
 
         Examples:
             ```python
             from vectice import Dataset, FileResource
 
             dataset = Dataset.modeling(
                 name="my modeling dataset",
-                training_resource=FileResource(path="training_dataset.csv"),
-                testing_resource=FileResource(path="testing_dataset.csv"),
-                validation_resource=FileResource(path="validation_dataset.csv"),
+                training_resource=FileResource(paths="training_dataset.csv"),
+                testing_resource=FileResource(paths="testing_dataset.csv"),
+                validation_resource=FileResource(paths="validation_dataset.csv"),
             )
             ```
 
         Parameters:
             training_resource: The resource for the training set (for modeling datasets).
             testing_resource: The resource for the testing set (for modeling datasets).
             validation_resource: The resource for the validation set (optional, for modeling datasets).
             name: The name of the dataset.
-            training_dataframe: A pandas dataframe allowing vectice to compute more metadata about the training set.
-            testing_dataframe: A pandas dataframe allowing vectice to compute more metadata about the testing set.
-            validation_dataframe: A pandas dataframe allowing vectice to compute more metadata about the validation set.
             properties: A dict, for example `{"folds": 32}`.
+            attachments: Path of a file that will be attached to the step along with the dataset.
         """
         return Dataset(
             type=DatasetType.MODELING,
             name=name,
             training_resource=training_resource,
             testing_resource=testing_resource,
             validation_resource=validation_resource,
-            training_dataframe=training_dataframe,
-            testing_dataframe=testing_dataframe,
-            validation_dataframe=validation_dataframe,
             properties=properties,
-            # attachments=attachments,
+            attachments=attachments,
         )
 
     def __repr__(self):
         return f"Dataset(name={self.name!r}, type={self.type!r})"
 
     @property
     def type(self) -> DatasetType:
@@ -312,40 +278,40 @@
 
         Parameters:
             properties: The properties of the dataset.
         """
         _logger.warning("To save your updated dataset properties, you must reassign your dataset to a step.")
         self._properties = self._format_properties(properties)
 
-    # @property
-    # def attachments(self) -> list[str] | None:
-    #     """The attachments associated with the dataset.
-
-    #     Returns:
-    #         The attachments associated with the dataset.
-    #     """
-    #     return self._attachments
-
-    # @attachments.setter
-    # def attachments(self, attachments: list[str] | str):
-    #     """Attach a file or files to the dataset.
-
-    #     Parameters:
-    #         attachments: The filename or filenames of the file or set of files to attach to the dataset.
-    #     """
-    #     self._attachments = self._format_attachments(attachments)
+    @property
+    def attachments(self) -> list[str] | None:
+        """The attachments associated with the dataset.
+
+        Returns:
+            The attachments associated with the dataset.
+        """
+        return self._attachments
+
+    @attachments.setter
+    def attachments(self, attachments: list[str] | str):
+        """Attach a file or files to the dataset.
+
+        Parameters:
+            attachments: The filename or filenames of the file or set of files to attach to the dataset.
+        """
+        self._attachments = self._format_attachments(attachments)
 
     @staticmethod
     def _check_key_duplicates(key_list: list[str]):
         if len(key_list) != len(set(key_list)):
             raise ValueError("Duplicate keys are not allowed.")
 
-    # @staticmethod
-    # def _format_attachments(attachments: str | list[str]) -> list[str]:
-    #     return [attachment for attachment in set(attachments)] if isinstance(attachments, list) else [attachments]
+    @staticmethod
+    def _format_attachments(attachments: str | list[str]) -> list[str]:
+        return [attachment for attachment in set(attachments)] if isinstance(attachments, list) else [attachments]
 
     def _format_properties(self, properties: dict[str, str | int] | list[Property] | Property | None) -> list[Property]:
         if properties is None:
             return []
         if isinstance(properties, Property):
             return [properties]
         if isinstance(properties, list):
@@ -353,33 +319,14 @@
             key_list = [prop.key for prop in properties]
             self._check_key_duplicates(key_list)
             return properties
         if isinstance(properties, dict):
             return [Property(key, str(value)) for (key, value) in properties.items()]
         raise ValueError("Please check property type.")
 
-    def _fill_file_dataframe(self, resources: list[tuple[Resource | None, DataFrame | None, str]]):
-        for resource, dataframe, arg in resources:
-            if dataframe is not None and not isinstance(dataframe, DataFrame):
-                raise ValueError(
-                    f"Argument '{arg}' of type '{type(dataframe)}' is invalid, only pandas DataFrame is supported."
-                )
-            if resource is not None and dataframe is not None:
-                if isinstance(resource.metadata, FilesMetadata):
-                    source = self._get_latest_source(sources=list(resource.metadata.files))
-                elif isinstance(resource.metadata, DBMetadata):
-                    source = self._get_latest_source(sources=list(resource.metadata.dbs))
-                if source is not None:
-                    source._dataframe = dataframe
-
-    def _get_latest_source(self, sources: list[Source]) -> Source | None:
-        if len(sources) == 0:
-            return None
-        return sorted(sources, key=lambda source: source.name.lower())[0]
-
     @staticmethod
     def _remove_incorrect_properties(properties: list[Property]) -> list[Property]:
         for prop in properties:
             if not isinstance(prop, Property):
                 _logger.warning(f"Incorrect property '{prop}'. Please check property type.")
                 properties.remove(prop)
         return properties
```

### Comparing `vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/file_data_wrapper.py` & `vectice-23.2.2.1/src/vectice/models/resource/file_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,152 +2,149 @@
 
 import datetime
 import glob
 import hashlib
 import logging
 import os
 
-from vectice.models.datasource.datawrapper.data_wrapper import DataWrapper
-from vectice.models.resource.metadata import (
-    DatasetSourceOrigin,
-    DatasetSourceUsage,
-    DatasetType,
-    File,
-    FilesMetadata,
-)
+from pandas import DataFrame
 
-_logger = logging.getLogger(__name__)
+from vectice.models.resource.base import Resource
+from vectice.models.resource.metadata.base import DatasetSourceOrigin
+from vectice.models.resource.metadata.files_metadata import File, FilesMetadata
 
+_logger = logging.getLogger(__name__)
 
-class FileDataWrapper(DataWrapper):
-    """Deprecated. Wrap columnar data and its metadata in a local file.
 
-    WARNING: **Wrappers are deprecated.**
-    Instead, use [`Dataset`][vectice.models.dataset.Dataset]
-    and [`FileResource`][vectice.models.resource.file_resource.FileResource].
+class FileResource(Resource):
+    """Wrap columnar data and its metadata in a local file.
 
     Vectice stores metadata -- data about your dataset -- communicated
-    with a DataWrapper.  Your actual dataset is not stored by Vectice.
+    with a resource.  Your actual dataset is not stored by Vectice.
 
-    This DataWrapper wraps data that you have stored in a local file.
+    This resource wraps data that you have stored in a local file.
 
     ```python
-    from vectice import DatasetType, FileDataWrapper, connect
+    from vectice import FileResource, connect
 
     my_project = connect(...)  # (1)
     my_phase = my_project.phase(...)  # (2)
     my_iter = my_phase.iteration()  # (3)
 
-    my_iter.step_my_data = FileDataWrapper(
-        path="my/file/path",
-        name="My origin dataset name",
-        type=DatasetType.ORIGIN,
-    )
+    my_iter.step_my_data = FileResource(paths="my/file/path")
     ```
 
     1. See [connection][vectice.Connection.connect].
     1. See [phases][vectice.models.Phase].
     1. See [iterations][vectice.models.Iteration].
 
     Note that these three concepts are distinct, even if easily conflated:
 
     * Where the data is stored
     * The format at rest (in storage)
-    * The format when loaded in a running python program
+    * The format when loaded in a running Python program
 
     Notably, the statistics collectors provided by Vectice operate
-    only on this last and only in the even that the data is loaded as
+    only on this last and only in the event that the data is loaded as
     a pandas dataframe.
     """
 
+    _origin = DatasetSourceOrigin.LOCAL.value
+
     def __init__(
         self,
-        path: str,
-        name: str,
-        usage: DatasetSourceUsage | None = None,
-        derived_from: list[int] | None = None,
-        type: DatasetType | None = None,
+        paths: str | list[str],
+        dataframes: DataFrame | list[DataFrame] | None = None,
     ):
-        """Initialize a file data wrapper.
+        """Initialize a file resource.
 
         Parameters:
-            path: The path of the file to wrap.
-            name: The name of the DataWrapper (local to Vectice).
-            usage: The usage of the dataset.
-            derived_from: The list of dataset ids to derive this new dataset from.
-            type: The type of the dataset.
+            paths: The paths of the files to wrap.
+            dataframes: The pandas dataframes allowing vectice to compute more metadata about this resource.
 
         Examples:
             The following example shows how to wrap a CSV file
             called `iris.csv` in the current directory:
 
-            >>> from vectice import FileDataWrapper, DatasetSourceUsage, DatasetType
-            >>> iris_trainset = FileDataWrapper(
-            ...     path="iris.csv",
-            ...     name="training dataset",
-            ...     type=DatasetType.MODELING,
-            ...     usage=DatasetSourceUsage.TRAINING,
-            ...     derived_from=[64, 128],
-            ... )
-            2023/02/01 15:43:59 INFO vectice.models.datasource.datawrapper.file_data_wrapper: File: iris.csv wrapped successfully.
+            ```python
+            from vectice import FileResource
+            iris_trainset = FileResource(paths="iris.csv")
+            ```
         """
-        self.path = path
-        super().__init__(name=name, type=type, usage=usage, derived_from=derived_from)
-        _logger.info(f"File: {path} wrapped successfully.")
+        super().__init__(paths=paths, dataframes=dataframes)
+        paths_log = ", ".join(self._paths) if len(self._paths) > 1 else self._paths[0]
+        _logger.info(f"File: {paths_log} wrapped successfully.")
 
     def _fetch_data(self) -> dict[str, bytes]:
         datas = {}
-        for file in self.metadata.files:
+        metadata: FilesMetadata = self.metadata  # type:ignore[assignment]
+        for file in metadata.files:
             with open(file.name, "rb") as opened_file:
                 datas[file.name] = opened_file.read()
         return datas
 
-    def _build_metadata(self, path: str | None = None) -> FilesMetadata:
-        if self.path is None:
-            raise ValueError("Path can not be None.")
-        files, total_size = self._file_visitor_list_builder(self.path, [])
-        metadata = FilesMetadata(size=total_size, origin=DatasetSourceOrigin.LOCAL.value, files=files, usage=self.usage)
+    def _build_metadata(self) -> FilesMetadata:
+        if self._paths is None:
+            raise ValueError("Paths can not be None.")
+        size = None
+        files = []
+        df_index = 0
+        for path in self._paths:
+            new_files, total_size, new_df_index = self._file_visitor_list_builder(index=df_index, path=path)
+            df_index += new_df_index
+            if size is None:
+                size = 0
+            size += total_size
+            files.extend(new_files)
+
+        metadata = FilesMetadata(size=size, origin=self._origin, files=files)
         return metadata
 
-    def _file_visitor_list_builder(self, path: str, files: list[File]) -> tuple[list[File], int]:
+    def _file_visitor_list_builder(self, index: int, path: str) -> tuple[list[File], int, int]:
+        files: list[File] = []
         total_size = 0
+        df_index = 0
         if not os.path.exists(path):
             raise FileNotFoundError
         if os.path.isfile(path):
-            file: File = self._build_file_from_path(path)
+            dataframe = (
+                self._dataframes[index] if self._dataframes is not None and len(self._dataframes) > index else None
+            )
+            file: File = self._build_file_from_path(path=path, dataframe=dataframe)
             total_size += file.size or 0
             files.append(file)
+            df_index += 1
         else:
-            for entry_path in glob.glob(f"{path}/**", recursive=True):
-                if os.path.isfile(entry_path):
-                    glob_file: File = self._build_file_from_path(entry_path)
-                    total_size += glob_file.size or 0
-                    files.append(glob_file)
-        return files, total_size
+            dir_paths = glob.glob(f"{path}/**", recursive=True)
+            for entry_path in filter(lambda x: os.path.isfile(x), sorted(dir_paths, key=str.lower)):
+                new_index = index + df_index
+                dataframe = (
+                    self._dataframes[new_index]
+                    if self._dataframes is not None and len(self._dataframes) > new_index
+                    else None
+                )
+                glob_file: File = self._build_file_from_path(path=entry_path, dataframe=dataframe)
+                total_size += glob_file.size or 0
+                files.append(glob_file)
+                df_index += 1
+        return files, total_size, df_index
 
-    def _build_file_from_path(self, path: str) -> File:
+    def _build_file_from_path(self, path: str, dataframe: DataFrame | None = None) -> File:
         entry_stats: os.stat_result = os.stat(path)
         name = path.split("\\")[-1]
         return File(
             name=name,
             size=entry_stats.st_size,
             fingerprint=self._compute_digest_for_path(path),
             updated_date=self._convert_date_to_iso(entry_stats.st_mtime),
-            created_date=self._convert_date_to_iso(self._get_created_date(entry_stats)),
             uri=f"file://{os.path.abspath(path)}",
+            dataframe=dataframe,
         )
 
     @staticmethod
-    def _get_created_date(entry_stats: os.stat_result) -> float:
-        try:
-            return float(entry_stats.st_birthtime)  # type: ignore[attr-defined]
-        except AttributeError:
-            return entry_stats.st_ctime
-
-    @staticmethod
     def _compute_digest_for_path(path: str) -> str:
         sha = hashlib.sha256()
         bytes_array = bytearray(128 * 1024)
         mv = memoryview(bytes_array)
         with open(path, "rb", buffering=0) as file:
             n = file.readinto(mv)
             while n:
```

### Comparing `vectice-23.2.1.1/src/vectice/models/git_version.py` & `vectice-23.2.2.1/src/vectice/models/git_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,21 +114,21 @@
         _logger.info(f"Code captured the following changed files; {', '.join(file_names)}")
 
 
 def _look_for_git_repository(repo_path=".") -> Any | None:
     try:
         repo_path = os.path.abspath(repo_path)
     except OSError:
-        _logger.warning(f"Code capture failed: the directory '{repo_path}' cannot be accessed by the system")
+        _logger.debug(f"Code capture failed: the directory '{repo_path}' cannot be accessed by the system")
         return None
     try:
         return Repo(repo_path, search_parent_directories=True)
     except GitError as error:
         error_message = str(error) or repo_path
-        _logger.warning(
+        _logger.debug(
             f"Code capture failed: {error.__class__.__name__}: {error_message}. "
             "Make sure the current directory is a valid Git repository (non-bare, non worktree) "
             "and its permissions allow the current user to access it."
         )
         return None
```

### Comparing `vectice-23.2.1.1/src/vectice/models/iteration.py` & `vectice-23.2.2.1/src/vectice/models/iteration.py`

 * *Files 12% similar despite different names*

```diff
@@ -113,53 +113,49 @@
     def __eq__(self, other: object):
         if not isinstance(other, Iteration):
             return NotImplemented
         return self.id == other.id
 
     def _populate_steps(self):
         with suppress(NoStepsInPhaseError):
-            return {step.slug: step for step in self.steps}
+            check = {step.slug: step for step in self.steps}
+            return check
         return {}
 
     def __getattr__(self, item):
         if item in self.__dict__:
             return self.__dict__[item]
         if item in super().__getattribute__("_steps"):
-            if not self._temp_type_filter(item):
-                self._steps[item] = self.step(self._steps[item].name)
-            return self._steps[item]
+            step_item = self._steps[item]
+            step = self._client.get_step_by_name(step_item.name, self.id)
+            step_object = _get_step_type(
+                id=step.id,
+                iteration=self,
+                name=step.name,
+                index=step.index,
+                slug=step.slug,
+                description=step.description,
+                completed=step.completed,
+                artifacts=step.artifacts,
+                step_type=step.step_type,
+                text=step.text,
+            )
+            return step_object
         raise AttributeError(f"The attribute '{item}' does not exist.")
 
     def __setattr__(self, attr_name, attr_value):
-        if not (hasattr(self, attr_name) or attr_name in self.__slots__):
-            raise AttributeError(f"The attribute '{attr_name}' does not exist.")
-        elif hasattr(self, "_steps") and attr_name in super().__getattribute__("_steps"):
+        if hasattr(self, "_steps") and attr_name in super().__getattribute__("_steps"):
             if self._status in {IterationStatus.Abandoned, IterationStatus.Completed}:
                 raise VecticeException(f"The Iteration is {self._status.name} and is read-only!")
             self._steps[attr_name] = self._steps[attr_name]._step_factory_and_update(value=attr_value)
+        elif hasattr(self, "__dict__") and attr_name not in self.__slots__:
+            raise AttributeError(f"The attribute '{attr_name}' does not exist.")
         else:
             super().__setattr__(attr_name, attr_value)
 
-    # TODO: remove this once StepModel is implemented
-    def _temp_type_filter(self, slug: str) -> bool:
-        """Temporary step type filter.
-
-        Currently we rely on the model being set. Once StepModel is
-        implemented we can remove this as we won't rely on the attributes being set.
-
-        Parameters:
-            slug: The step slug.
-
-        Returns:
-            A boolean.
-        """
-        if self._steps[slug]._model:
-            return True
-        return False
-
     @property
     def id(self) -> int:
         """The iteration's identifier.
 
         Returns:
             The iteration's identifier.
         """
@@ -207,42 +203,14 @@
         """The names of the steps required in this iteration.
 
         Returns:
             The steps names.
         """
         return [step.name for step in self.steps]
 
-    def step(self, step: str) -> Step:
-        """Get a step by name.
-
-        Step names are configured for a phase by the Vectice administrator.
-
-        Parameters:
-            step: The name of the step
-
-        Returns:
-            A step.
-        """
-        steps_output = self._client.get_step_by_name(step, self.id)
-        _logger.debug(f"Step: {steps_output.name} successfully retrieved.")
-        step_object = _get_step_type(
-            id=steps_output.id,
-            iteration=self,
-            name=steps_output.name,
-            index=steps_output.index,
-            slug=steps_output.slug,
-            description=steps_output.description,
-            completed=steps_output.completed or None,
-            artifacts=steps_output.artifacts,
-            step_type=steps_output.step_type,
-            text=steps_output.text,
-        )
-        self._current_step = step_object
-        return step_object
-
     @property
     def steps(self) -> list[Step]:
         """The steps required in this iteration.
 
         Returns:
             The steps required in this iteration.
         """
@@ -259,72 +227,41 @@
                 artifacts=item.artifacts,
                 step_type=item.step_type,
             )
             for item in sorted(steps_output, key=lambda x: x.index)
         ]
 
     def list_steps(self) -> None:
-        """List the steps to which this iteration has access and print the steps in a tabular format.
+        """Prints a list of steps belonging to the iteration in a tabular format, limited to the first 10 items. A link is provided to view the remaining steps.
 
         Returns:
             None
         """
         steps_output = sorted(self._client.list_steps(self.phase.id, self.index), key=lambda x: x.index)
         user_name, _ = _get_last_user_and_default_workspace(self._client)
 
         rich_table = Table(expand=True, show_edge=False)
 
-        rich_table.add_column("step id", justify="left", no_wrap=True, min_width=5, max_width=5)
+        rich_table.add_column("index", justify="left", no_wrap=True, min_width=5, max_width=5)
         rich_table.add_column("shortcut", justify="left", no_wrap=True, min_width=5, max_width=20)
         rich_table.add_column("artifacts", justify="left", no_wrap=True, min_width=5, max_width=15)
         rich_table.add_column("comment", justify="left", no_wrap=True, min_width=5, max_width=20)
 
-        def _get_artifact_id(artifact) -> int | None:
-            if artifact.dataset_version_id:
-                return int(artifact.dataset_version_id)
-            if artifact.model_version_id:
-                return int(artifact.model_version_id)
-            if artifact.entity_file_id:
-                return int(artifact.entity_file_id)
-            return None
-
         for count, step in enumerate(steps_output, 1):
             if count > 10:
                 break
-            step_text = step.text if step.text != "None" else None
-            steps_started = False
-            # TODO no artifacts, remove nested
-            for number, artifact in enumerate(step.artifacts, 1):
-                artifact_id = _get_artifact_id(artifact)
-                if not steps_started:
-                    rich_table.add_row(
-                        str(step.id), step.slug, f"{number}. {artifact.type.value} {artifact_id}", step_text
-                    )
-                if steps_started:
-                    rich_table.add_row(None, None, f"{number}. {artifact.type.value} {artifact_id}", None)
-                steps_started = True
-            if not step.artifacts:
-                rich_table.add_row(
-                    str(step.id),
-                    step.slug,
-                    None,
-                    step_text,
-                )
-        if not steps_output:
-            rich_table.add_row(
-                None,
-                None,
-                None,
-                None,
-            )
-        description = f"""There are {len(steps_output)} steps in iteration {self.index!r}."""
+            step_text = 1 if step.text != "None" else 0
+            number_of_artifacts = len(step.artifacts) + step_text
+            rich_table.add_row(str(count), step.slug, str(number_of_artifacts), "True" if step_text == 1 else "False")
+
+        description = f"""There are {len(steps_output)} steps in Iteration '{self.index!r}' and a maximum of 10 steps are displayed in the table below:"""
         tips = dedent(
             """
-        >> To access a specific step, use iteration.step(Step ID)
-        >> To access an array of steps, use iteration.steps"""
+        To access a specific step, use the step shortcut \033[1iiteration\033[0m.step_my_step_name
+        The step reference is referred to as shortcut"""
         ).lstrip()
         link = dedent(
             f"""
         For quick access to the list of steps in the Vectice web app, visit:
         {self._client.auth._API_BASE_URL}/project/phase/iteration?w={self.workspace.id}&iterationId={self.id}"""
         ).lstrip()
 
@@ -343,15 +280,22 @@
     def complete(self) -> None:
         """Mark the iteration as completed."""
         if self._status is IterationStatus.Abandoned:
             raise VecticeException("The iteration is canceled and cannot be completed.")
         iteration_input = IterationInput(status=IterationStatus.Completed.name)
         self._client.update_iteration(self.id, iteration_input)
         self._status = IterationStatus.Completed
-        _logger.info(f"Iteration with index {self.index} completed.")
+        logging_output = dedent(
+            f"""
+                        Iteration with index {self.index} completed.
+
+                        For quick access to the Iteration in the Vectice web app, visit:
+                        {self._client.auth._API_BASE_URL}/project/phase/iteration?w={self.workspace.id}&iterationId={self.id}"""
+        ).lstrip()
+        _logger.info(logging_output)
 
     def delete(self) -> None:
         self._client.delete_iteration(self.id)
         _logger.info(f"Iteration with index {self.index} was deleted.")
 
     @property
     def connection(self) -> Connection:
```

### Comparing `vectice-23.2.1.1/src/vectice/models/metric.py` & `vectice-23.2.2.1/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/model.py` & `vectice-23.2.2.1/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/phase.py` & `vectice-23.2.2.1/src/vectice/models/phase.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     ```
 
     Iterations can then be created for this phase,
     to complete the phase steps:
 
     ```python
     my_origin_dataset = ...
-    my_iteration = my_phase.iteration()
+    my_iteration = my_phase.create_iteration()
     my_iteration.step_origin_dataset = my_origin_dataset
     ```
 
     NOTE: **Phases and Steps Definitions are created in the Vectice App,
     Iterations are created from the Vectice Python API.**
 
     See the documentation of [Iterations][vectice.models.Iteration]
@@ -174,16 +174,16 @@
             The phase's iterations.
         """
         iteration_outputs = self._client.list_iterations(self.id)
         return sorted(
             [Iteration(item.id, item.index, self, item.status) for item in iteration_outputs], key=lambda x: x.index
         )
 
-    def list_step_definitions(self) -> None:
-        """List the step definitions to which this phase has access and print the step definitions in a tabular format.
+    def list_steps(self) -> None:
+        """Prints a list of step definitionss belonging to the phase in a tabular format, limited to the first 10 items. A link is provided to view the remaining step definitionss.
 
         Returns:
             None
         """
         steps_output = sorted(self._client.list_step_definitions(self.id), key=lambda x: x.index)
         user_name, _ = _get_last_user_and_default_workspace(self._client)
 
@@ -193,42 +193,72 @@
         rich_table.add_column("name", justify="left", no_wrap=True, min_width=5, max_width=10)
         rich_table.add_column("description", justify="left", no_wrap=True, min_width=3, max_width=15)
 
         for count, step in enumerate(steps_output, 1):
             if count > 10:
                 break
             rich_table.add_row(step.slug, step.name, format_description(step.description))
-        description = f"""There are {len(steps_output)} steps required in the phase {self.name!r}."""
+        description = f"""There are {len(steps_output)} steps required in the phase {self.name!r} and a maximum of 10 steps are displayed in the table below:"""
         link = dedent(
             f"""
         For quick access to the list of step definitions in the Vectice web app, visit:
         {self._client.auth._API_BASE_URL}/project/phase/steps?w={self.workspace.id}&pageId={self.id}"""
         ).lstrip()
         _temp_print(description)
         _temp_print(table=rich_table)
         _temp_print(link)
 
-    def iteration(self, index: int | None = None) -> Iteration:
-        """Get a (possibly new) iteration.
+    def iteration(self, index: int) -> Iteration:
+        """Get an iteration.
 
-        Fetch and return an iteration by index. If no index is
-        provided, return a new iteration.
+        Fetch and return an iteration by index.
 
         Parameters:
             index: The id of an existing iteration.
 
         Returns:
             An iteration.
         """
-        if index:
-            iteration_output = self._client.get_iteration_by_index(self.id, index)
-        else:
-            iteration_output = self._client.create_iteration(self.id)
-            _logger.info(f"New Iteration number {iteration_output.index!r} created.")
-        _logger.info(f"Iteration number {iteration_output.index!r} successfully retrieved.")
+        iteration_output = self._client.get_iteration_by_index(self.id, index)
+
+        iteration_object = Iteration(
+            id=iteration_output.id,
+            index=iteration_output.index,
+            phase=self,
+            status=iteration_output.status,
+        )
+        logging_output = dedent(
+            f"""
+                Iteration number '{iteration_output.index!r}' successfully retrieved."
+
+                For quick access to the Iteration in the Vectice web app, visit:
+                {self._client.auth._API_BASE_URL}/project/phase/iteration?w={self.workspace.id}&iterationId={iteration_object.id}"""
+        ).lstrip()
+        _logger.info(logging_output)
+        self._current_iteration = iteration_object
+        return iteration_object
+
+    def create_iteration(self) -> Iteration:
+        """Create a new iteration.
+
+        Create and return an iteration.
+
+        Returns:
+            An iteration.
+        """
+        iteration_output = self._client.create_iteration(self.id)
+        logging_output = dedent(
+            f"""
+        New Iteration number '{iteration_output.index!r}' created.
+
+        For quick access to the Iteration in the Vectice web app, visit:
+        {self._client.auth._API_BASE_URL}/project/phase/iteration?w={self.workspace.id}&iterationId={iteration_output.id}"""
+        ).lstrip()
+        _logger.info(logging_output)
+
         iteration_object = Iteration(
             id=iteration_output.id,
             index=iteration_output.index,
             phase=self,
             status=iteration_output.status,
         )
         self._current_iteration = iteration_object
```

### Comparing `vectice-23.2.1.1/src/vectice/models/project.py` & `vectice-23.2.2.1/src/vectice/models/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,21 +146,29 @@
         Parameters:
             phase: The name or id of the phase to get.
 
         Returns:
             The specified phase.
         """
         item = self._client.get_phase(phase, project_id=self._id)
-        _logger.info(f"Phase {item.name!r} successfully retrieved.")
         phase_object = Phase(item.id, self, item.name, item.index, item.status)
+        logging_output = dedent(
+            f"""
+                        Phase {item.name!r} successfully retrieved."
+
+                        For quick access to the Phase in the Vectice web app, visit:
+                        {self._client.auth._API_BASE_URL}/project/phase?w={self.workspace.id}&pageId={phase_object.id}"""
+        ).lstrip()
+        _logger.info(logging_output)
+
         self._phase = phase_object
         return phase_object
 
     def list_phases(self) -> None:
-        """List the phases to which this project has access and print the phases in a tabular format.
+        """Prints a list of phases belonging to the project in a tabular format, limited to the first 10 items. A link is provided to view the remaining phases.
 
         Returns:
             None
         """
         phase_outputs = sorted(self._client.list_phases(project=self.id), key=lambda x: x.index)
         user_name, _ = _get_last_user_and_default_workspace(self._client)
 
@@ -193,19 +201,18 @@
                 str(phase.id),
                 phase.name,
                 phase_owner,
                 phase_status,
                 f"{active_iterations}/{iterations_total}",
                 str(total_phase_steps),
             )
-        description = f"""There are {len(phase_outputs)} phases in the project {self.name!r}."""
+        description = f"""There are {len(phase_outputs)} phases in the project {self.name!r} and a maximum of 10 phases are displayed in the table below:"""
         tips = dedent(
             """
-        >> To access a specific phase, use project.phase(PhaseID)
-        >> To access an array of phases, use project.phases"""
+        To access a specific phase, use \033[1mproject\033[0m.phase(Phase ID)"""
         ).lstrip()
         link = dedent(
             f"""
         For quick access to the list of phases for this project, visit:
         {self._client.auth._API_BASE_URL}/project?w={self.workspace.id}&resourceId={self.id}"""
         ).lstrip()
         legend = """**Legend**     [C]  Completed     [IP] In Progress
```

### Comparing `vectice-23.2.1.1/src/vectice/models/property.py` & `vectice-23.2.2.1/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/__init__.py` & `vectice-23.2.2.1/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/bigquery_resource.py` & `vectice-23.2.2.1/src/vectice/models/resource/bigquery_resource.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
+from pandas import DataFrame
+
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata import DatasetSourceOrigin
 from vectice.models.resource.metadata.column_metadata import DBColumn
 from vectice.models.resource.metadata.db_metadata import DBMetadata, MetadataDB
 
 if TYPE_CHECKING:
     from google.cloud.bigquery import Client as BQClient
@@ -26,16 +28,16 @@
     ```python
     from vectice import BigQueryResource
     from google.cloud.bigquery import Client
 
     my_service_account_file = "MY_SERVICE_ACCOUNT_JSON_PATH"  # (1)
     bq_client = Client.from_service_account_json(json_credentials_path=my_service_account_file)  # (2)
     bq_resource = BigQueryResource(
-        bq_client,
-        table="bigquery-public-data.stackoverflow.posts_questions",
+        bq_client=bq_client,
+        paths="bigquery-public-data.stackoverflow.posts_questions",
     )
     ```
 
     1. See [Service account credentials](https://developers.google.com/workspace/guides/create-credentials#service-account).
     1. See [GCS docs](https://cloud.google.com/python/docs/reference/storage/latest/modules).
 
     Note that these three concepts are distinct, even if easily conflated:
@@ -49,76 +51,130 @@
     a pandas dataframe.
     """
 
     _origin = DatasetSourceOrigin.BIGQUERY.value
 
     def __init__(
         self,
-        bq_client: BQClient,
-        path: str,
+        paths: str | list[str],
+        dataframes: DataFrame | list[DataFrame] | None = None,
+        bq_client: BQClient | None = None,
     ):
         """Initialize a BigQuery resource.
 
         Parameters:
+            paths: The paths to retrieve the datasets or the tables.
+            dataframes: The pandas dataframes allowing vectice to compute more metadata about this resource.
             bq_client: The `google.cloud.bigquery.Client` used
                 to interact with BigQuery.
-            path: The path to retrieve the dataset or the table.
         """
-        super().__init__()
-        self.path = path
+        super().__init__(paths=paths, dataframes=dataframes)
         self.bq_client = bq_client
 
-    def _fetch_data(self) -> dict[str, Table | None]:
-        from google.api_core.exceptions import Forbidden
+    def _fetch_data(self) -> dict[str, tuple[Table | None, DataFrame | None]]:
+        tables: dict[str, tuple[Table | None, DataFrame | None]] = {}
+        df_index = 0
+        for path in self._paths:
+            path_tables, new_df_index = self._fetch_path_data(index=df_index, path=path)
+            tables.update(path_tables)
+            df_index += new_df_index
 
-        count_dots_in_path = self.path.count(".")
+        return tables
+
+    def _fetch_path_data(self, index: int, path: str) -> tuple[dict[str, tuple[Table | None, DataFrame | None]], int]:
+        count_dots_in_path = path.count(".")
         is_dataset = count_dots_in_path == 1
         is_table = count_dots_in_path == 2
 
         if is_table is True:
-            table_name = self.path.rpartition(".")[-1]
-            tb = None
-            try:
-                tb = self.bq_client.get_table(table=self.path)
-            except Forbidden:
-                _logger.warning(f"Failed to fetch data information for table {table_name}")
-                pass
-
-            return {table_name: tb}
+            return self._fetch_table_data(index=index, path=path), 1
 
         if is_dataset is True:
-            tables_dict: dict[str, Table | None] = {}
-            try:
-                tables = self.bq_client.list_tables(dataset=self.path)
-                for table in tables:
-                    try:
-                        tables_dict[table.table_id] = self.bq_client.get_table(table=f"{self.path}.{table.table_id}")
-                    except Exception:
-                        _logger.warning(f"Failed to fetch data information for table {table.table_id}")
-                        tables_dict[table.table_id] = None
-                        continue
-                return tables_dict
-            except Forbidden:
-                _logger.warning(f"Failed to list tables for dataset {self.path}")
-                return {}
+            return self._fetch_dataset_data(index=index, path=path)
+
+        raise ValueError(f"Path '{path}' is invalid, please reference either a dataset or a table.")
+
+    def _fetch_table_data(self, index: int, path: str) -> dict[str, tuple[Table | None, DataFrame | None]]:
+        from google.api_core.exceptions import Forbidden
 
-        raise ValueError("path is invalid, please reference either a dataset or a table.")
+        table_name = path.partition(".")[-1]
+
+        dataframe = self._dataframes[index] if self._dataframes is not None and len(self._dataframes) > index else None
+        if self.bq_client is None:
+            return {table_name: (None, dataframe)}
+
+        tb = None
+        try:
+            tb = self.bq_client.get_table(table=path)
+        except Forbidden:
+            _logger.warning(f"Failed to fetch data information for table {table_name}")
+            pass
+
+        return {table_name: (tb, dataframe)}
+
+    def _fetch_dataset_data(
+        self, index: int, path: str
+    ) -> tuple[dict[str, tuple[Table | None, DataFrame | None]], int]:
+        from google.api_core.exceptions import Forbidden
+
+        df_index = 0
+        tables_dict: dict[str, tuple[Table | None, DataFrame | None]] = {}
+        dataset = path.partition(".")[-1]
+        if self.bq_client is None:
+            new_index = df_index + index
+            dataframe = (
+                self._dataframes[new_index]
+                if self._dataframes is not None and len(self._dataframes) > new_index
+                else None
+            )
+            return {dataset: (None, dataframe)}, 1
+        try:
+            tables_data: list[Table] = self.bq_client.list_tables(dataset=path)  # type: ignore[assignment]
+            tables = sorted(tables_data, key=lambda table: table.table_id.lower())
+            for table in tables:
+                new_index = df_index + index
+                dataframe = (
+                    self._dataframes[new_index]
+                    if self._dataframes is not None and len(self._dataframes) > new_index
+                    else None
+                )
+                dataset = path.partition(".")[-1]
+                table_name = f"{dataset}.{table.table_id}"
+                try:
+                    tables_dict[table_name] = (
+                        self.bq_client.get_table(table=f"{path}.{table.table_id}"),
+                        dataframe,
+                    )
+                except Exception:
+                    _logger.warning(f"Failed to fetch data information for table {table_name}")
+                    tables_dict[table_name] = None, dataframe
+                    pass
+
+                df_index += 1
+            return tables_dict, df_index
+        except Forbidden:
+            _logger.warning(f"Failed to list tables for dataset {path}")
+            return {}, 0
 
     def _build_metadata(self) -> DBMetadata:
-        tables_metadata: dict[str, Table | None] = self.data  # type:ignore[assignment]
+        tables_metadata: dict[str, tuple[Table | None, DataFrame | None]] = self.data  # type:ignore[assignment]
         dbs: list[MetadataDB] = []
-        for table_name, table_metadata in tables_metadata.items():
+        for table_name, [table_metadata, dataframe] in tables_metadata.items():
             columns: list[DBColumn] = []
             size = None
             rows_number = None
             updated_date = None
+            created_date = None
             if table_metadata is not None:
                 size = table_metadata.num_bytes
                 rows_number = table_metadata.num_rows
-                updated_date = table_metadata.modified.isoformat()
+                modified = table_metadata.modified
+                updated_date = modified.isoformat() if modified is not None else None
+                created = table_metadata.created
+                created_date = created.isoformat() if created is not None else None
                 for column in table_metadata.schema:
                     columns.append(
                         DBColumn(
                             name=column.name,
                             data_type=column.field_type,
                             is_unique=False,
                             nullable=column.is_nullable,
@@ -129,15 +185,17 @@
 
             dbs.append(
                 MetadataDB(
                     name=table_name,
                     rows_number=rows_number,
                     size=size,
                     columns=columns,
+                    created_date=created_date,
                     updated_date=updated_date,
+                    dataframe=dataframe,
                 )
             )
 
         metadata_size = None
         for db in dbs:
             if db.size is not None:
                 if metadata_size is None:
```

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/description.py` & `vectice-23.2.2.1/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.2.2.1/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/metadata/base.py` & `vectice-23.2.2.1/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-23.2.2.1/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/metadata/dataframe_column_parser.py` & `vectice-23.2.2.1/src/vectice/models/resource/metadata/dataframe_column_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import logging
 
+import pandas as pd
 from pandas import DataFrame, Series, api
 
 from vectice.models.resource.metadata.column_metadata import Column, StatValue
 
 # mypy: ignore-errors
 
 _logger = logging.getLogger(__name__)
@@ -34,14 +35,16 @@
 
 
 def capture_column_stats(series: Series) -> list[StatValue] | None:
     if api.types.is_bool_dtype(series):
         return compute_boolean_column_statistics(series)
     elif api.types.is_numeric_dtype(series):
         return compute_numeric_column_statistics(series)
+    elif api.types.is_datetime64_any_dtype(series) | (series.dtypes == "dbdate"):
+        return compute_date_column_statistics(series)
     elif api.types.is_string_dtype(series):
         return compute_string_column_statistics(series)
     return None
 
 
 def compute_boolean_column_statistics(series: Series) -> list[StatValue]:
     """Parse a dataframe series and return statistics about it.
@@ -84,16 +87,17 @@
     Parameters:
         series: The pandas series to get information from.
 
     Returns:
         A list of StatValue.
     """
     var = series.var()
+    med = series.median()
     stats = [
-        StatValue("median", series.median()),
+        StatValue("median", float(med) if isinstance(med, float) else int(med)),
         StatValue("variance", float(var) if isinstance(var, float) else int(var)),
     ]
     stats.extend(
         [
             StatValue(str(name), float(value) if isinstance(value, float) else int(value))
             for name, value in series.describe().items()
         ]
@@ -114,10 +118,40 @@
         series: The pandas series to get information from.
 
     Returns:
         A list of StatValue.
     """
     stats = [StatValue("null", int(series.isna().sum()))]
     for name, value in series.describe(include="all").items():
-        stats.extend([StatValue(str(name), int(value) if not isinstance(value, str) else str(value))])
+        stats.extend([StatValue(str(name), int(value) if isinstance(value, (int, float)) else str(value))])
 
     return stats
+
+
+def compute_date_column_statistics(series: Series) -> list[StatValue]:
+    """Parse a dataframe series and return statistics about it.
+
+    The computed statistics are:
+    - the min value
+    - the mean
+    - max value
+    - the null count
+    Parameters:
+        series: The pandas series to get information from.
+
+    Returns:
+        A list of StatValue.
+    """
+    # Convert to datetime since mean is not supported for non datetime pandas object such as dbdates
+    series = pd.to_datetime(series)
+    min = series.min().date()
+    mean = series.mean().date()
+    median = series.median().date()
+    max = series.max().date()
+
+    return [
+        StatValue("null", int(series.isna().sum())),
+        StatValue(key="min", value=str(min)),
+        StatValue(key="mean", value=str(mean)),
+        StatValue(key="median", value=str(median)),
+        StatValue(key="max", value=str(max)),
+    ]
```

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.2.2.1/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,27 +43,36 @@
     def __init__(
         self,
         name: str,
         columns: list[DBColumn],
         rows_number: int | None = None,
         size: int | None = None,
         updated_date: str | None = None,
+        created_date: str | None = None,
         dataframe: DataFrame | None = None,
     ):
         """Initialize a MetadataDB instance.
 
         Parameters:
             name: The name of the table.
             columns: The columns that compose the table.
             rows_number: The number of row of the table.
             size: The size of the table.
             updated_date: The date of last update of the table.
+            created_date: The creation date of the table.
             dataframe: A pandas dataframe which will capture the tables metadata.
         """
-        super().__init__(name=name, size=size, columns=list(columns), updated_date=updated_date, dataframe=dataframe)
+        super().__init__(
+            name=name,
+            size=size,
+            columns=list(columns),
+            updated_date=updated_date,
+            created_date=created_date,
+            dataframe=dataframe,
+        )
         self.rows_number = rows_number
         if dataframe is not None:
             self.rows_number = len(dataframe.index)
 
     def asdict(self) -> dict:
         return {
             **super().asdict(),
```

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-23.2.2.1/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
 class File(Source):
     """Describe a dataset file."""
 
     def __init__(
         self,
         name: str,
-        size: int,
-        fingerprint: str,
+        size: int | None = None,
+        fingerprint: str | None = None,
         created_date: str | None = None,
         updated_date: str | None = None,
         uri: str | None = None,
         columns: list[Column] | None = None,
         dataframe: DataFrame | None = None,
     ):
         """Initialize a file.
@@ -62,17 +62,23 @@
             fingerprint: The hash of the file.
             created_date: The date of creation of the file.
             updated_date: The date of last update of the file.
             uri: The uri of the file.
             columns: The columns coming from the dataframe with the statistics.
             dataframe: A pandas dataframe which will capture the files metadata.
         """
-        super().__init__(name=name, size=size, columns=columns, updated_date=updated_date, dataframe=dataframe)
+        super().__init__(
+            name=name,
+            size=size,
+            columns=columns,
+            created_date=created_date,
+            updated_date=updated_date,
+            dataframe=dataframe,
+        )
         self.fingerprint = fingerprint
-        self.created_date = created_date
         self.uri = uri
 
     def asdict(self) -> dict:
         return {
             **super().asdict(),
             "fingerprint": self.fingerprint,
             "createdDate": self.created_date,
```

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/metadata/source.py` & `vectice-23.2.2.1/src/vectice/models/resource/metadata/source.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,33 +9,38 @@
 class Source:
     def __init__(
         self,
         name: str,
         size: int | None = None,
         columns: list[Column] | None = None,
         updated_date: str | None = None,
+        created_date: str | None = None,
         dataframe: DataFrame | None = None,
     ):
         """Initialize a MetadataDB instance.
 
         Parameters:
             name: The name of the source.
             size: The size of the source.
             columns: The columns that compose the source.
             updated_date: The date of last update of the source.
+            created_date: The date of last update of the source.
             dataframe: A pandas dataframe which will capture the sources metadata.
         """
         self.name = name
         self.size = size
         self.columns = columns
+        self.created_date = created_date
         self.updated_date = updated_date
         self._dataframe = dataframe
         if dataframe is not None:
-            self.size = dataframe.size
+            size = dataframe.size
+            self.size = float(size) if isinstance(size, float) else int(size)  # type: ignore[arg-type]
 
     def asdict(self) -> dict:
         return {
             "name": self.name,
             "size": self.size,
             "updatedDate": self.updated_date,
+            "createdDate": self.created_date,
             "columns": capture_columns(init_columns=self.columns, dataframe=self._dataframe),
         }
```

### Comparing `vectice-23.2.1.1/src/vectice/models/resource/s3_resource.py` & `vectice-23.2.2.1/src/vectice/models/resource/s3_resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from __future__ import annotations
 
+import re
 from typing import TYPE_CHECKING
 
+from pandas import DataFrame
+
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata.base import DatasetSourceOrigin
 from vectice.models.resource.metadata.files_metadata import File, FilesMetadata
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import Client
     from mypy_boto3_s3.type_defs import ListObjectsV2OutputTypeDef, ObjectTypeDef
 
 
+S3_URI_REG = r"(s3:\/\/)([^\/]+)\/(.+)"
+
+
 class S3Resource(Resource):
     """Wrap columnar data and its metadata in AWS S3.
 
     Vectice stores metadata -- data about your dataset -- communicated
     with a resource. Your actual dataset is not stored by Vectice.
 
     This resource wraps data that you have stored in AWS S3.
@@ -28,17 +34,16 @@
         aws_access_key_id="...",
         aws_secret_access_key="...",
         region_name="us-east-1",
     )
     s3_client = s3_session.client(service_name="s3")  # (2)
 
     s3_resource = S3Resource(
-        s3_client,
-        bucket_name="my_bucket",
-        resource_path="my_resource_path",
+        s3_client=s3_client,
+        uris="s3://<bucket_name>/<file_path_inside_bucket>",
     )
     ```
 
     1. See [boto3 sessions][boto3.session.Session].
     1. See [boto3 session client][boto3.session.Session.client].
 
     Note that these three concepts are distinct, even if easily conflated:
@@ -52,77 +57,132 @@
     a pandas dataframe.
     """
 
     _origin = DatasetSourceOrigin.S3.value
 
     def __init__(
         self,
-        s3_client: Client,
-        bucket_name: str,
-        resource_path: str,
+        uris: str | list[str],
+        dataframes: DataFrame | list[DataFrame] | None = None,
+        s3_client: Client | None = None,
     ):
         """Initialize an S3 resource.
 
         Parameters:
+            uris: The uris of the resources to get. Should follow the pattern 'gs://<bucket_name>/<file_path_inside_bucket>'
+            dataframes: The pandas dataframes allowing vectice to compute more metadata about this resource.
             s3_client: The client used to interact with Amazon s3.
-            bucket_name: The name of the bucket to get data from.
-            resource_path: The paths of the resources to get.
         """
-        super().__init__()
+        super().__init__(paths=uris, dataframes=dataframes)
         self.s3_client = s3_client
-        self.bucket_name = bucket_name
-        self.resource_path = resource_path
 
-    def _fetch_data(self) -> dict[str, bytes]:
-        s3_objects_list = self._get_s3_objects_list()
+        for uri in self._paths:
+            if not re.search(S3_URI_REG, uri):
+                raise ValueError(
+                    f"Uri '{uri}' is not following the right pattern 's3://<bucket_name>/<file_path_inside_bucket>'"
+                )
+
+    def _fetch_data(self) -> dict[str, bytes | None]:
         datas = {}
-        for s3_object in s3_objects_list["Contents"]:
-            object_path = s3_object["Key"]
-            data = self._get_aws_data(object_path)
-            datas[f"{self.bucket_name}/{object_path}"] = data
+        if self.s3_client:
+            s3_objects_list = self._get_s3_objects_list(self.s3_client)
+            for bucket_name, s3_objects in s3_objects_list:
+                for s3_object in s3_objects["Contents"]:
+                    object_path = s3_object["Key"]
+                    data = self._get_aws_data(self.s3_client, bucket_name, object_path)
+                    datas[f"{bucket_name}/{object_path}"] = data
+        else:
+            for path in self._paths:
+                datas[path] = None
+
         return datas
 
-    def _get_aws_data(self, object_path: str):
-        data_response = self.s3_client.get_object(Bucket=self.bucket_name, Key=object_path)
+    def _get_aws_data(self, s3_client: Client, bucket_name: str, object_path: str):
+        data_response = s3_client.get_object(Bucket=bucket_name, Key=object_path)
         return data_response["Body"].read()
 
     def _build_metadata(self) -> FilesMetadata:
-        s3_objects_list = self._get_s3_objects_list()
-        metadata = self._build_metadata_from_objects(s3_objects_list)
-        return metadata
-
-    def _get_s3_objects_list(self) -> ListObjectsV2OutputTypeDef:
-        return self.s3_client.list_objects_v2(Bucket=self.bucket_name, Prefix=self.resource_path)
+        size = None
+        files = []
+        df_index = 0
+        if self.s3_client:
+            s3_objects_list = self._get_s3_objects_list(self.s3_client)
+            for bucket_name, s3_objects in s3_objects_list:
+                if s3_objects["KeyCount"] == 0:
+                    raise NoSuchS3ResourceError(bucket_name, s3_objects["Prefix"])
+                s3_object = s3_objects["Contents"]
+                new_files, total_size, new_df_index = self._build_files_list_with_size(
+                    index=df_index, bucket_name=bucket_name, s3_object=s3_object
+                )
+                if size is None:
+                    size = 0
+                size += total_size
+                files.extend(new_files)
+                df_index += new_df_index
+        else:
+            for index, uri in enumerate(self._paths):
+                dataframe = (
+                    self._dataframes[index] if self._dataframes is not None and len(self._dataframes) > index else None
+                )
+                _, path = self._get_bucket_and_path_from_uri(uri)
+                file = File(name=path, uri=uri, dataframe=dataframe)
+                files.append(file)
 
-    def _build_metadata_from_objects(self, s3_objects_list: ListObjectsV2OutputTypeDef) -> FilesMetadata:
-        if s3_objects_list["KeyCount"] == 0:
-            raise NoSuchS3ResourceError(self.bucket_name, self.resource_path)
-        s3_objects = s3_objects_list["Contents"]
-        files, total_size = self._build_files_list_with_size(s3_objects)
-        metadata = FilesMetadata(files=files, origin=self._origin, size=total_size)
+        metadata = FilesMetadata(files=files, origin=self._origin, size=size)
         return metadata
 
-    def _build_files_list_with_size(self, s3_objects: list[ObjectTypeDef]) -> tuple[list[File], int]:
+    def _build_files_list_with_size(
+        self, index: int, bucket_name: str, s3_object: list[ObjectTypeDef]
+    ) -> tuple[list[File], int, int]:
         files: list[File] = []
         total_size = 0
-        for object in s3_objects:
-            if not self._is_s3_object_a_folder(object):
-                name = object["Key"]
-                size = object["Size"]
-                file = File(
-                    name=name,
-                    size=size,
-                    fingerprint=self._get_formatted_etag_from_object(object),
-                    updated_date=object["LastModified"].isoformat(),
-                    created_date=None,
-                    uri=f"s3://{self.bucket_name}/{name}",
-                )
-                total_size += size
-                files.append(file)
-        return files, total_size
+        df_index = 0
+        filtered_s3_object = list(filter(lambda obj: self._is_s3_object_a_folder(obj) is False, s3_object))
+        sorted_s3_object = sorted(filtered_s3_object, key=lambda obj: obj["Key"].lower())
+        for object in sorted_s3_object:
+            new_index = df_index + index
+            name = object["Key"]
+            size = object["Size"]
+            uri = f"s3://{bucket_name}/{name}"
+            dataframe = (
+                self._dataframes[new_index]
+                if self._dataframes is not None and len(self._dataframes) > new_index
+                else None
+            )
+
+            file = File(
+                name=name,
+                size=size,
+                fingerprint=self._get_formatted_etag_from_object(object),
+                updated_date=object["LastModified"].isoformat(),
+                created_date=None,
+                uri=uri,
+                dataframe=dataframe,
+            )
+            total_size += size
+            files.append(file)
+            df_index += 1
+        return files, total_size, df_index
+
+    def _get_s3_objects_list(self, s3_client: Client) -> list[tuple[str, ListObjectsV2OutputTypeDef]]:
+        return list(map(lambda uri: self._get_s3_objects(s3_client, uri), self._paths))
+
+    def _get_s3_objects(self, s3_client: Client, uri: str) -> tuple[str, ListObjectsV2OutputTypeDef]:
+        bucket_name, path = self._get_bucket_and_path_from_uri(uri)
+        return bucket_name, s3_client.list_objects_v2(Bucket=bucket_name, Prefix=path)
+
+    def _get_bucket_and_path_from_uri(self, uri: str) -> tuple[str, str]:
+        match = re.search(S3_URI_REG, uri)
+        if match is not None:
+            _, bucket_name, path = match.groups()
+            return bucket_name, path
+
+        raise ValueError(
+            f"Uri '{uri}' is not following the right pattern 's3://<bucket_name>/<file_path_inside_bucket>'"
+        )
 
     @staticmethod
     def _get_formatted_etag_from_object(object: ObjectTypeDef) -> str:
         return str(object["ETag"].replace("'", "").replace('"', ""))
 
     @staticmethod
     def _is_s3_object_a_folder(object: ObjectTypeDef) -> bool:
```

### Comparing `vectice-23.2.1.1/src/vectice/models/step.py` & `vectice-23.2.2.1/src/vectice/models/step.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,41 +4,36 @@
 import pickle  # nosec
 from io import IOBase
 from typing import TYPE_CHECKING, Any
 
 from PIL.Image import Image
 
 import vectice
+from vectice.api.json.dataset_register import DatasetRegisterOutput
+from vectice.api.json.dataset_version import DatasetVersionOutput
 from vectice.api.json.iteration import (
     IterationStatus,
     IterationStepArtifact,
     IterationStepArtifactInput,
     IterationStepArtifactType,
 )
 from vectice.api.json.model_register import ModelRegisterOutput
 from vectice.api.json.model_version import ModelVersionOutput
 from vectice.api.json.step import StepType
 from vectice.models.attachment_container import AttachmentContainer
-from vectice.models.resource.base import Resource
-from vectice.models.resource.metadata import DatasetType
-from vectice.utils.automatic_link_utils import (
-    existing_dataset_logger,
-    existing_model_logger,
-    link_assets_to_step,
-    link_dataset_to_step,
-)
-from vectice.utils.common_utils import _check_image_path, _check_read_only, _get_image_variables
-from vectice.utils.last_assets import _register_dataset_logging, _register_model_logging
+from vectice.utils.common_utils import _check_image_path, _get_image_variables
+from vectice.utils.last_assets import _comment_or_image_logging, _register_dataset_logging, _register_model_logging
 
 if TYPE_CHECKING:
     from vectice import Connection
     from vectice.models import Iteration, Phase, Project, Workspace
     from vectice.models.dataset import Dataset
     from vectice.models.model import Model
     from vectice.models.step_dataset import StepDataset
+    from vectice.models.step_model import StepModel
     from vectice.models.step_number import StepNumber
     from vectice.models.step_string import StepString
 
 _logger = logging.getLogger(__name__)
 
 MISSING_DATASOURCE_ERROR_MESSAGE = "Cannot create modeling dataset. Missing %s data source."
 
@@ -142,153 +137,218 @@
             return NotImplemented
         return self.id == other.id
 
     def __iadd__(self, value):
         # TODO cyclic import
         from vectice.models.dataset import Dataset
         from vectice.models.model import Model
+        from vectice.models.step_dataset import StepDataset
+        from vectice.models.step_model import StepModel
 
         if isinstance(value, Model):
             if self._type not in {StepType.StepModel, StepType.Step}:
                 raise TypeError(f"A model can't be added to a step of type {self._type!r}.")
-            model_artifact = self._register_model(value)
-            self.artifacts.append(model_artifact)
+            code_version_id = self._get_code_version_id()
+            model_data = self._client.register_model(
+                model=value,
+                project_id=self.project.id,
+                phase_id=self.phase.id,
+                iteration_id=self.iteration.id,
+                code_version_id=code_version_id,
+            )
+            attachments_output = self._set_model_attachments(value, model_data.model_version)
+            model_artifact = IterationStepArtifact(modelVersionId=model_data["modelVersion"]["id"], type="ModelVersion")
+            copy_artifacts = self.artifacts.copy()
+            self.artifacts += [model_artifact]
+            attachments = (
+                [
+                    IterationStepArtifact(entityFileId=attach["fileId"], type="EntityFile")
+                    for attach in attachments_output
+                ]
+                if attachments_output
+                else []
+            )
+            self.artifacts += attachments
+
             self._keep_artifacts_and_update_step(StepType.StepModel, value)
+            step = StepModel(self, model_artifact, value)
+            _register_model_logging(self, model_data, value, self.name, attachments_output, _logger, copy_artifacts)
+            self._iteration._steps[self.name] = step
         elif isinstance(value, Dataset):
             if self._type not in {StepType.StepDataset, StepType.Step}:
                 raise TypeError(f"A dataset can't be added to a step of type {self._type!r}.")
-            dataset_artifact, _ = self._register_dataset(value)
+            code_version_id = self._get_code_version_id()
+            dataset_output = self._client.register_dataset_from_source(
+                dataset=value,
+                project_id=self.project.id,
+                phase_id=self.phase.id,
+                iteration_id=self.iteration.id,
+                code_version_id=code_version_id,
+            )
+            attachments_output = self._set_dataset_attachments(value, dataset_output.dataset_version)
+            dataset_artifact = IterationStepArtifact(
+                datasetVersionId=dataset_output["datasetVersion"]["id"],
+                type=IterationStepArtifactType.DataSetVersion.name,
+            )
+            copy_artifacts = self.artifacts.copy()
             self.artifacts.append(dataset_artifact)
+            attachments = (
+                [
+                    IterationStepArtifact(entityFileId=attach["fileId"], type="EntityFile")
+                    for attach in attachments_output
+                ]
+                if attachments_output
+                else []
+            )
+            self.artifacts += attachments
             self._keep_artifacts_and_update_step(StepType.StepDataset, value)
+            step = StepDataset(self, dataset_artifact)
+            _register_dataset_logging(self, dataset_output, value, attachments_output, _logger, copy_artifacts)
+            self._iteration._steps[self.name] = step
         else:
             raise TypeError(f"Expected Dataset or a Model, got {type(value)}")
 
     def _keep_artifacts_and_update_step(self, step_type: StepType, value) -> None:
-        if self._type is StepType.Step:
-            artifacts = self.iteration.step(self.name).artifacts
+        artifacts = self._client.get_step_by_name(self.name, self._iteration.id).artifacts
 
-            def _get_artifact_id(artifact: IterationStepArtifact) -> int:
-                if artifact.model_version_id:
-                    return artifact.model_version_id
-                if artifact.dataset_version_id:
-                    return artifact.dataset_version_id
-                if artifact.entity_file_id:
-                    return artifact.entity_file_id
-                raise ValueError("No artifact ID.")
-
-            maintain_artifacts = [
-                IterationStepArtifactInput(id=_get_artifact_id(artifact), type=artifact.type.value)
-                for artifact in artifacts
-            ]
-            self._client.update_iteration_step_artifact(self.id, step_type, artifacts=maintain_artifacts)
-            self._warn_step_change(value)
+        def _get_artifact_id(artifact: IterationStepArtifact) -> int:
+            if artifact.model_version_id:
+                return artifact.model_version_id
+            if artifact.dataset_version_id:
+                return artifact.dataset_version_id
+            if artifact.entity_file_id:
+                return artifact.entity_file_id
+            raise ValueError("No artifact ID.")
 
-    def _refresh_step(self) -> Step:
-        step = self._iteration.step(self.name)
-        setattr(self._iteration, step.slug, step)
-        return step
+        def _maintain_and_add_artifacts(session_artifacts, existing_artifacts):
+            # Ensure we don't keep adding an instances artifacts to the step
+            maintain_artifacts = existing_artifacts
+            for artifact in session_artifacts:
+                match = any(filter(lambda x: x.id == artifact.id, existing_artifacts))
+                if not match:
+                    maintain_artifacts += [artifact]
+            return maintain_artifacts
+
+        # These are artifacts that exist in the current instance
+        session_artifacts = [
+            IterationStepArtifactInput(id=_get_artifact_id(artifact), type=artifact.type.value)
+            for artifact in self.artifacts
+        ]
+        # These are artifacts in Vectice
+        existing_artifacts = [
+            IterationStepArtifactInput(id=_get_artifact_id(artifact), type=artifact.type.value)
+            for artifact in artifacts
+        ]
+        # Ensure no crossover or duplicates
+        maintain_artifacts = _maintain_and_add_artifacts(session_artifacts, existing_artifacts)
+        self._client.update_iteration_step_artifact(self.id, step_type, artifacts=maintain_artifacts)
+        self._warn_step_change(value)
 
     def _step_factory_and_update(
         self, value: Dataset | Model | int | float | str | None = None
-    ) -> Step | StepString | StepNumber | StepDataset:
+    ) -> Step | StepString | StepNumber | StepDataset | StepModel:
         # TODO cyclic imports
         from vectice.models.dataset import Dataset
         from vectice.models.model import Model
         from vectice.models.step_dataset import StepDataset
         from vectice.models.step_image import StepImage
         from vectice.models.step_model import StepModel
         from vectice.models.step_number import StepNumber
         from vectice.models.step_string import StepString
 
         if isinstance(value, (int, float)):
             self._update_iteration_step(StepType.StepNumber, value)
+            _comment_or_image_logging(self, _logger)
             return StepNumber(step=self, number=value)
 
         if (
             isinstance(value, Image)
             or isinstance(value, IOBase)
             or (isinstance(value, str) and _check_image_path(value))
         ):
             step_artifacts, filename = self._create_image_artifact(value)
             self._update_iteration_step(StepType.StepImage, value, step_artifacts)
-            _logger.info(f"File {filename!r} linked to Step {self.name!r}.")
+            _comment_or_image_logging(self, _logger, filename)
             return StepImage(self, value)
 
         if isinstance(value, str):
             self._update_iteration_step(StepType.StepString, value)
+            _comment_or_image_logging(self, _logger)
             return StepString(self, string=value)
 
         if isinstance(value, Model):
             code_version_id = self._get_code_version_id()
             data = self._client.register_model(
                 model=value,
                 project_id=self.project.id,
                 phase_id=self.phase.id,
                 iteration_id=self.iteration.id,
                 code_version_id=code_version_id,
             )
             attachments_output = self._set_model_attachments(value, data.model_version)
 
-            artifacts = self._get_model_artifacts(data, attachments_output)
-            step_output = self._client.update_iteration_step_artifact(
+            artifacts = self._get_version_artifacts(data, attachments_output)
+            self._client.update_iteration_step_artifact(
                 self.id,
                 StepType.StepModel,
                 None,
                 artifacts,
             )
             _register_model_logging(self, data, value, self.name, attachments_output, _logger)
-            self.artifacts = [IterationStepArtifact(modelVersionId=step_output.id, type="ModelVersion")]
+            self.artifacts = [IterationStepArtifact(modelVersionId=data["modelVersion"]["id"], type="ModelVersion")]
             self._warn_step_change(value)
             return StepModel(self, self.artifacts[0], value)
 
         if isinstance(value, Dataset):
             code_version_id = self._get_code_version_id()
             dataset = self._client.register_dataset_from_source(
                 dataset=value,
                 project_id=self.project.id,
                 phase_id=self.phase.id,
                 iteration_id=self.iteration.id,
                 code_version_id=code_version_id,
             )
-            artifacts = [
-                IterationStepArtifactInput(
-                    id=dataset["datasetVersion"]["id"],
-                    type=IterationStepArtifactType.DataSetVersion.name,
-                )
-            ]
-            step_output = self._client.update_iteration_step_artifact(
+            attachments_output = self._set_dataset_attachments(value, dataset.dataset_version)
+            artifacts = self._get_version_artifacts(dataset, attachments_output)
+            self._client.update_iteration_step_artifact(
                 self.id,
                 StepType.StepDataset,
                 None,
                 artifacts,
             )
-
-            _register_dataset_logging(self, dataset, value, step_output, _logger)
-            self.artifacts = [IterationStepArtifact(datasetVersionId=step_output.id, type="DataSetVersion")]
+            _register_dataset_logging(self, dataset, value, attachments_output, _logger)
+            self.artifacts = [
+                IterationStepArtifact(datasetVersionId=dataset["datasetVersion"]["id"], type="DataSetVersion")
+            ]
             self._warn_step_change(value)
-            return StepDataset(self, dataset_version=step_output.artifacts[0])
+            return StepDataset(self, dataset_version=self.artifacts[0])
 
         return self
 
-    def _get_model_artifacts(
-        self, data: ModelRegisterOutput, attachments_output: list[dict] | None = None
+    def _get_version_artifacts(
+        self, data: ModelRegisterOutput | DatasetRegisterOutput, attachments_output: list[dict] | None = None
     ) -> list[IterationStepArtifactInput]:
         attachments = None
         if attachments_output:
             attachments = (
                 [IterationStepArtifactInput(id=attach["fileId"], type="EntityFile") for attach in attachments_output]
                 if attachments_output
                 else None
             )
-        artifacts = [
-            IterationStepArtifactInput(
+        if isinstance(data, ModelRegisterOutput):
+            artifact = IterationStepArtifactInput(
                 id=data["modelVersion"]["id"],
                 type=IterationStepArtifactType.ModelVersion.name,
             )
-        ]
+        else:
+            artifact = IterationStepArtifactInput(
+                id=data["datasetVersion"]["id"],
+                type=IterationStepArtifactType.DataSetVersion.name,
+            )
+        artifacts = [artifact]
         artifacts += attachments if attachments else []
         return artifacts
 
     def _create_image_artifact(self, value: str | IOBase | Image) -> tuple[list[IterationStepArtifactInput], str]:
         image, filename = _get_image_variables(value)
         try:
             attachments_output = self._client.create_phase_attachments(
@@ -340,15 +400,15 @@
                 maintain_artifacts,
             )
 
             self._warn_step_change(value)
         elif isinstance(value, Model) or type is StepType.StepModel:
             self._client.update_iteration_step_artifact(self.id, StepType.StepModel, artifacts=step_artifacts)
             self._warn_step_change(value)
-            self.model = value
+            self._model = value
         elif type is StepType.StepDataset:
             self._client.update_iteration_step_artifact(self.id, StepType.StepDataset, artifacts=step_artifacts)
             self._warn_step_change(value)
 
     def _warn_step_change(self, value):
         # TODO: cyclic import
         from vectice.models.dataset import Dataset
@@ -481,36 +541,14 @@
         """The iteration to which this step belongs.
 
         Returns:
             The iteration to which this step belongs.
         """
         return self._iteration
 
-    @staticmethod
-    def _get_datasources_in_order(data_sources: tuple[Resource, ...]) -> tuple[Resource, Resource, Resource | None]:
-        from vectice import DatasetSourceUsage
-
-        if len(data_sources) != 3 and len(data_sources) != 2:
-            raise ValueError("Exactly two or three datasources are needed to create a modeling dataset.")
-
-        train_datasource, test_datasource, validation_datasource = None, None, None
-        for data_source in data_sources:
-            if data_source:
-                if data_source.metadata.usage == DatasetSourceUsage.TRAINING:
-                    train_datasource = data_source
-                elif data_source.metadata.usage == DatasetSourceUsage.TESTING:
-                    test_datasource = data_source
-                elif data_source.metadata.usage == DatasetSourceUsage.VALIDATION:
-                    validation_datasource = data_source
-        if not train_datasource:
-            raise ValueError(MISSING_DATASOURCE_ERROR_MESSAGE % "training")
-        if not test_datasource:
-            raise ValueError(MISSING_DATASOURCE_ERROR_MESSAGE % "testing")
-        return train_datasource, test_datasource, validation_datasource
-
     def _get_code_version_id(self):
         # TODO: cyclic imports
         from vectice.models.git_version import _check_code_source, _inform_if_git_repo
 
         if vectice.code_capture:
             return _check_code_source(self._client, self.project.id, _logger)
         else:
@@ -522,99 +560,31 @@
         """The step's model.
 
         Returns:
             The step's model.
         """
         return self._model
 
-    @model.setter
-    def model(self, model: Model):
-        """Set the model for the step.
-
-        The model can be created using the Model Wrapper, accessed via
-        vectice.Model or `from vectice import Model`.
-
-        Parameters:
-            model: The model.
-        """
-        model_artifact = self._register_model(model)
-        self._model = model
-        self.artifacts = [model_artifact]
-
     def _set_model_attachments(self, model: Model, model_version: ModelVersionOutput):
         logging.getLogger("vectice.models.attachment_container").propagate = True
         attachments = None
         if model.attachments:
             container = AttachmentContainer(model_version, self._client)
             attachments = container.add_attachments(model.attachments)
         if model.predictor:
             model_content = self._serialize_model(model.predictor)
             model_type_name = type(model.predictor).__name__
             container = AttachmentContainer(model_version, self._client)
             container.add_serialized_model(model_type_name, model_content)
         return attachments
 
+    def _set_dataset_attachments(self, dataset: Dataset, dataset_version: DatasetVersionOutput):
+        logging.getLogger("vectice.models.attachment_container").propagate = True
+        attachments = None
+        if dataset.attachments:
+            container = AttachmentContainer(dataset_version, self._client)
+            attachments = container.add_attachments(dataset.attachments)
+        return attachments
+
     @staticmethod
     def _serialize_model(model: Any) -> bytes:
         return pickle.dumps(model)
-
-    def _register_model(self, model: Model) -> IterationStepArtifact:
-        from vectice.models.git_version import _check_code_source, _inform_if_git_repo
-
-        _check_read_only(self._iteration)
-        if vectice.code_capture:
-            code_version_id = _check_code_source(self._client, self._iteration._phase._project._id, _logger)
-        else:
-            _inform_if_git_repo()
-            code_version_id = None
-        model_output = self._client.register_model(
-            model, self.iteration.project.id, self.phase.id, self.iteration.id, code_version_id, model.derived_from
-        )
-        model_version = model_output.model_version
-        attachments = self._set_model_attachments(model, model_version)
-        _logger.info(
-            f"Successfully registered Model(name='{model.name}', library='{model.library}', "
-            f"technique='{model.technique}', version='{model_version.name}')."
-        )
-        existing_model_logger(model_output, model.name, _logger)
-        step_artifact = IterationStepArtifactInput(id=model_output["modelVersion"]["id"], type="ModelVersion")
-        attachments = (
-            [
-                IterationStepArtifactInput(id=attach["fileId"], entityFileId=attach["entityId"], type="EntityFile")
-                for attach in attachments
-            ]
-            if attachments
-            else None
-        )
-        logging.getLogger("vectice.models.project").propagate = False
-        link_assets_to_step(self, step_artifact, model.name, model_output, _logger, attachments)
-        model_artifact = IterationStepArtifact(modelVersionId=step_artifact.id, type=step_artifact.type)
-        return model_artifact
-
-    def _register_dataset(self, dataset: Dataset) -> tuple[IterationStepArtifact, dict]:
-        _check_read_only(self.iteration)
-        code_version_id = self._get_code_version_id()
-
-        data = self._client.register_dataset_from_source(
-            dataset=dataset,
-            project_id=self.project.id,
-            phase_id=self.phase.id,
-            iteration_id=self.iteration.id,
-            code_version_id=code_version_id,
-        )
-        existing_dataset_logger(data, dataset.name, _logger)
-        step_artifact = IterationStepArtifactInput(id=data["datasetVersion"]["id"], type="DataSetVersion")
-        logging.getLogger("vectice.models.iteration").propagate = False
-        logging.getLogger("vectice.models.project").propagate = False
-
-        if dataset.type is DatasetType.MODELING:
-            link_assets_to_step(self, step_artifact, dataset.name, data, _logger)
-        else:
-            link_dataset_to_step(step_artifact, dataset, data, _logger, self)
-        dataset_artifact = IterationStepArtifact(datasetVersionId=step_artifact.id, type=step_artifact.type)
-        return dataset_artifact, data
-
-    def _manage_dataset_artifact_update(self, step_artifact: IterationStepArtifact):
-        self.artifacts.append(step_artifact)
-        refreshed_step = self._refresh_step()
-        if refreshed_step._type is not StepType.StepDataset:
-            _logger.warning(f"Step: {self.name!r} type changed from {self._type.name} to StepDataset")
```

### Comparing `vectice-23.2.1.1/src/vectice/models/step_dataset.py` & `vectice-23.2.2.1/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/step_image.py` & `vectice-23.2.2.1/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/step_model.py` & `vectice-23.2.2.1/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/step_number.py` & `vectice-23.2.2.1/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/step_string.py` & `vectice-23.2.2.1/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/models/workspace.py` & `vectice-23.2.2.1/src/vectice/models/workspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         """
         item = self._client.get_project(project, self.id)
         _logger.debug(f"Your current project: {item.id}")
         project_object = Project(item.id, self, item.name, item.description)
         return project_object
 
     def list_projects(self) -> None:
-        """List the projects to which this workspace has access and log the projects in a tabular format.
+        """Prints a list of projects belonging to the workspace in a tabular format, limited to the first 10 items. A link is provided to view the remaining projects.
 
         Returns:
             None
         """
         project_outputs = self.projects
         user_name, _ = _get_last_user_and_default_workspace(self._client)
 
@@ -151,19 +151,22 @@
         rich_table.add_column("description", justify="left", no_wrap=True, max_width=50)
 
         for count, project in enumerate(project_outputs, 1):
             if count > 10:
                 break
             rich_table.add_row(str(project.id), project.name, format_description(project.description))
 
-        description = f"""There are {len(project_outputs)} projects in the workspace {self.name!r}."""
+        description = dedent(
+            f"""
+        There are {len(project_outputs)} projects in the workspace {self.name!r} and a maximum of 10 projects are displayed in the table below:
+        """
+        ).lstrip()
         tips = dedent(
             """
-        >> To access a specific project, use workspace.project(Project ID)
-        >> To access an array of projects, use workspace.projects"""
+        To access a specific project, use \033[1mworkspace\033[0m.project(Project ID)"""
         ).lstrip()
         link = dedent(
             f"""
             For quick access to the list of projects in the Vectice web app, visit:
             {self._client.auth._API_BASE_URL}/workspace/projects?w={self.id}"""
         ).lstrip()
```

### Comparing `vectice-23.2.1.1/src/vectice/utils/common_utils.py` & `vectice-23.2.2.1/src/vectice/utils/common_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         iteration: The iteration to check.
 
     Raises:
         RuntimeError: When the iteration is read-only (completed or canceled).
     """
     refresh_iteration = iteration._phase.iteration(iteration.index)
     if refresh_iteration._status in {IterationStatus.Completed, IterationStatus.Abandoned}:
-        raise RuntimeError(f"The Iteration is {refresh_iteration._status.name} and is read-only!")
+        raise RuntimeError(f"The Iteration is {refresh_iteration._status.name} and is read-only.")
 
 
 def _get_step_type(
     id: int,
     iteration: Iteration,
     name: str,
     index: int,
@@ -58,38 +58,51 @@
     artifacts: list[IterationStepArtifact] | None = None,
     text: str | None = None,
 ) -> Step | Any:
     # TODO: cyclic imports
     from vectice.models.step import Step
     from vectice.models.step_dataset import StepDataset
     from vectice.models.step_image import StepImage
+    from vectice.models.step_model import StepModel
     from vectice.models.step_number import StepNumber
     from vectice.models.step_string import StepString
 
     step = Step(
         id=id,
         iteration=iteration,
         name=name,
         index=index,
         slug=slug,
         description=description,
         artifacts=artifacts,
         step_type=step_type,
         text=text,
     )
+
+    def _get_number(text):
+        try:
+            number = float(text)
+        except ValueError:
+            number = int(text)
+        return number
+
     if step_type is StepType.StepNumber:
-        return StepNumber(step, float(text) if text else None)
+        number = _get_number(text) if text else None
+        return StepNumber(step, number)
     if step_type is StepType.StepString:
         return StepString(step, text)
     if step_type is StepType.StepImage:
         image = _get_image_info(iteration, artifacts) if artifacts else None
         return StepImage(step, image=image)
     if step_type is StepType.StepDataset:
         dataset_version = artifacts[0]  # type: ignore[index]
         return StepDataset(step, dataset_version=dataset_version)
+    if step_type is StepType.StepModel:
+        model_version = artifacts[0]  # type: ignore[index]
+        return StepModel(step, model_version=model_version)
     return step
 
 
 def _get_image_info(iteration: Iteration, artifacts: list[IterationStepArtifact]):
     artifacts = [image for image in artifacts if image.type.value == "EntityFile"]
     artifact = artifacts[0] if artifacts else None
     attachments = iteration._client.list_phase_attachments(iteration.phase.id, iteration.project.id)
@@ -118,17 +131,15 @@
 def _validate_image(path: str) -> BytesIO:
     try:
         byte_io = BytesIO()
         image = Image.open(path)
         image.save(byte_io, image.format)
         byte_io.seek(0)
     except UnidentifiedImageError:
-        raise ValueError(
-            f"The provided image {path!r} cannot be opened with Pillow, check its format and permissions."
-        ) from None
+        raise ValueError(f"The provided image {path!r} cannot be opened. Check its format and permissions.") from None
     return byte_io
 
 
 def _get_image_variables(value: str | IOBase | Image.Image) -> tuple[BytesIO | IOBase, str]:
     if isinstance(value, IOBase):
         image = value
         filename = os.path.basename(value.name)  # type: ignore[attr-defined]
```

### Comparing `vectice-23.2.1.1/src/vectice/utils/configuration.py` & `vectice-23.2.2.1/src/vectice/utils/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 class Configuration:
     def __init__(self, config_file_path: str):
         with open(config_file_path, "r") as config_file:
             try:
                 self.config_object = json.load(config_file)
             except JSONDecodeError as error:
-                raise SyntaxError(
-                    "The JSON config file could not be read. Check that the file structure is valid."
-                ) from error
+                raise SyntaxError("Can not read JSON config file. Check that the file structure is valid.") from error
 
     def __getitem__(self, key) -> str | int:
         information: str | int = self.config_object.get(key)
         if not information:
-            raise KeyError(key)
+            raise KeyError(f"Error while reading the configuration, {key} is empty.")
         return information
```

### Comparing `vectice-23.2.1.1/src/vectice/utils/deprecation.py` & `vectice-23.2.2.1/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.1/src/vectice/utils/last_assets.py` & `vectice-23.2.2.1/src/vectice/utils/last_assets.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from vectice.utils.automatic_link_utils import existing_dataset_logger, existing_model_logger
 
 if TYPE_CHECKING:
     from logging import Logger
 
     from vectice.api import Client
     from vectice.api.json.last_assets import ActivityTargetType
-    from vectice.api.json.step import StepOutput
     from vectice.models.step import Step
 
 
 def _get_last_assets(target_types: list[ActivityTargetType], client: Client, _logger: Logger):
     target_types_array = [target.value for target in target_types]
     try:
         last_asset = client.get_last_assets(target_types_array, {"index": 1, "size": 1}).list[0]
@@ -37,76 +36,107 @@
         logging_output = f"For quick access to your default workspace in the Vectice web app, visit:\n{host}/workspace/dashboard?w={workspace_id}"
         _logger.info(CONNECTION_LOGGING.format(user=user_name, logging_output=logging_output))
         return
     logging_output = f"For quick access to the list of workspaces in the Vectice web app, visit:\n{host}/workspaces"
     _logger.info(CONNECTION_LOGGING.format(user=user_name, logging_output=logging_output))
 
 
-def _register_dataset_logging(step: Step, data: dict, value: Any, step_output: StepOutput, _logger: Logger):
+def _register_dataset_logging(
+    step: Step, data: dict, value: Any, attachments, _logger: Logger, step_artifacts: Any | None = None
+):
     iteration_id = step._iteration.id
     url = step._client.auth.api_base_url
     hyper_link = f"{url}/project/phase/iteration?w={step.workspace.id}&iterationId={iteration_id}"
 
     # check if exists
     existing_logging = existing_dataset_logger(data, value.name, _logger)
     # check if attached to step
-    match = next(filter(lambda x: x.dataset_version_id == data["datasetVersion"]["id"], step.artifacts), None)
+    check_artifacts = step_artifacts if step_artifacts else step.artifacts
+    match = next(filter(lambda x: x.dataset_version_id == data["datasetVersion"]["id"], check_artifacts), None)
+    attachments_output = None
+    if attachments:
+        attachments_output = ", ".join([attach["fileName"] for attach in attachments])
     logging_output = None
     if existing_logging and match:
         logging_output = dedent(
             f"""
-                                Existing Dataset: {value.name!r} Version: {data['datasetVersion']['name']!r} already linked to Step: {step_output.name}
+                                Existing Dataset: {value.name!r} and Version: {data['datasetVersion']['name']!r} already linked to Step: {step.name}
+                                Attachments: {attachments_output}
                                 Link to Step: {hyper_link}
                                 """
         ).lstrip()
     if existing_logging and not match:
         logging_output = dedent(
             f"""
-                    Existing Dataset: {value.name!r} Version: {data['datasetVersion']['name']!r} added to Step: {step_output.name}
+                    New Version: {data['datasetVersion']['name']!r} of Dataset: {value.name!r} added to Step: {step.name}
+                    Attachments: {attachments_output}
                     Link to Step: {hyper_link}
                     """
         ).lstrip()
     if not existing_logging and not match:
         logging_output = dedent(
             f"""
-                                    New Dataset: {value.name!r} Version: {data['datasetVersion']['name']!r} added to Step: {step_output.name}
+                                    New Dataset: {value.name!r} Version: {data['datasetVersion']['name']!r} added to Step: {step.name}
+                                    Attachments: {attachments_output}
                                     Link to Step: {hyper_link}
                                     """
         ).lstrip()
     if logging_output:
         _logger.info(logging_output)
     else:
         _logger.debug("Logging failed for register dataset at step, check _register_dataset_logging.")
 
 
-def _register_model_logging(step: Step, data: dict, value: Any, step_name: str, attachments, _logger: Logger):
+def _comment_or_image_logging(step: Step, _logger: Logger, filename: str | None = None):
+    iteration_id = step._iteration.id
+    url = step._client.auth.api_base_url
+    hyper_link = f"{url}/project/phase/iteration?w={step.workspace.id}&iterationId={iteration_id}"
+    if filename:
+        artifact_reference = f"Image: {filename!r}"
+    else:
+        artifact_reference = "Comment"
+    logging_output = dedent(
+        f"""
+        Added {artifact_reference} to Step: {step.name}
+
+        Link to Step: {hyper_link}
+        """
+    ).lstrip()
+
+    _logger.info(logging_output)
+
+
+def _register_model_logging(
+    step: Step, data: dict, value: Any, step_name: str, attachments, _logger: Logger, step_artifacts: Any | None = None
+):
     iteration_id = step._iteration.id
     url = step._client.auth.api_base_url
     hyper_link = f"{url}/project/phase/iteration?w={step.workspace.id}&iterationId={iteration_id}"
 
     # check if exists
     existing_logging = existing_model_logger(data, value.name, _logger)
     # check if attached to step already
-    match = next(filter(lambda x: x.model_version_id == data["modelVersion"]["id"], step.artifacts), None)
+    check_artifacts = step_artifacts if step_artifacts else step.artifacts
+    match = next(filter(lambda x: x.model_version_id == data["modelVersion"]["id"], check_artifacts), None)
     attachments_output = None
     if attachments:
         attachments_output = ", ".join([attach["fileName"] for attach in attachments])
     logging_output = None
-    if (existing_logging or not existing_logging) and match:
+    if existing_logging and match:
         logging_output = dedent(
             f"""
-                                Existing Model: {value.name!r} Version: {data['modelVersion']['name']!r} already linked to Step: {step_name}
+                                Existing Model: {value.name!r} and Version: {data['modelVersion']['name']!r} already linked to Step: {step_name}
                                 Attachments: {attachments_output}
                                 Link to Step: {hyper_link}
                                 """
         ).lstrip()
     if existing_logging and not match:
         logging_output = dedent(
             f"""
-                    Existing Model: {value.name!r} Version: {data['modelVersion']['name']!r} added to Step: {step_name}
+                    New Version: {data['modelVersion']['name']!r} of Model: {value.name!r} added to Step: {step_name}
                     Attachments: {attachments_output}
                     Link to Step: {hyper_link}
                     """
         ).lstrip()
     if not existing_logging and not match:
         logging_output = dedent(
             f"""
```

### Comparing `vectice-23.2.1.1/src/vectice/utils/logging_utils.py` & `vectice-23.2.2.1/src/vectice/utils/logging_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 
 if TYPE_CHECKING:
     from vectice.api.json.phase import PhaseStatus
 
 
 CONNECTION_LOGGING = """Welcome, {user}. You`re now successfully connected to Vectice.
 
-To access your personal workspace, use connection.my_workspace or connection.workspaces[0]
-To access a specific workspace, use connection.workspace(Workspace ID)
-To get a list of workspaces you can access and their IDs, use connection.list_workspaces()
+To access your personal workspace, use \033[1mconnection\033[0m.my_workspace
+To access a specific workspace, use \033[1mconnection\033[0m.workspace(Workspace ID)
+To get a list of workspaces you can access and their IDs, use \033[1mconnection\033[0m.list_workspaces()
 
 If you are using a notebook you can call the help by using a Vectice returned object with the builtin notebook "?":
 >> connection?
 
 If you are using an IDE you can call the help() method on any object returned by Vectice:
 >> help(connection)
 
 {logging_output}"""
 
 CONNECTION_WORKSPACE_LOGGING = """Welcome, {user!r}. You`re now successfully connected to the workspace {workspace_name!r} in Vectice.
 
-To access a specific project, use workspace.project(Project ID)
-To get a list of projects you can access and their IDs, use workspace.list_projects()
+To access a specific project, use \033[1mworkspace\033[0m.project(Project ID)
+To get a list of projects you can access and their IDs, use \033[1mworkspace\033[0m.list_projects()
 
 For quick access to the list of projects in the Vectice web app, visit:
 {url}/workspace/projects?w={workspace_id}"""
 
 CONNECTION_PROJECT_LOGGING = """Welcome, {user!r}. You`re now successfully connected to the project {project_name!r} in Vectice.
 
-To access a specific phase, use project.phase(Phase ID)
-To get a list of phases you can access and their IDs, use project.list_phases()
+To access a specific phase, use \033[1mproject\033[0m.phase(Phase ID)
+To get a list of phases you can access and their IDs, use \033[1mproject\033[0m.list_phases()
 
 For quick access to the list of phases in the Vectice web app, visit:
 {url}/project?w={workspace_id}&resourceId={project_id}"""
 
 
 class VecticeLoggingStream:
     """A Python stream for use with event logging APIs throughout vectice (`logger.info()`, etc.).
```

### Comparing `vectice-23.2.1.1/src/vectice.egg-info/PKG-INFO` & `vectice-23.2.2.1/src/vectice.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.1.1
+Version: 23.2.2.1
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.1.1/src/vectice.egg-info/SOURCES.txt` & `vectice-23.2.2.1/src/vectice.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 src/vectice/api/json/__init__.py
 src/vectice/api/json/artifact_version.py
 src/vectice/api/json/attachment.py
 src/vectice/api/json/code.py
 src/vectice/api/json/code_version.py
 src/vectice/api/json/compatibility.py
 src/vectice/api/json/dataset_register.py
+src/vectice/api/json/dataset_version.py
 src/vectice/api/json/files_metadata.py
 src/vectice/api/json/iteration.py
 src/vectice/api/json/last_assets.py
 src/vectice/api/json/metric.py
 src/vectice/api/json/model.py
 src/vectice/api/json/model_register.py
 src/vectice/api/json/model_version.py
@@ -74,24 +75,14 @@
 src/vectice/models/step.py
 src/vectice/models/step_dataset.py
 src/vectice/models/step_image.py
 src/vectice/models/step_model.py
 src/vectice/models/step_number.py
 src/vectice/models/step_string.py
 src/vectice/models/workspace.py
-src/vectice/models/datasource/__init__.py
-src/vectice/models/datasource/datawrapper/__init__.py
-src/vectice/models/datasource/datawrapper/data_wrapper.py
-src/vectice/models/datasource/datawrapper/file_data_wrapper.py
-src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py
-src/vectice/models/datasource/datawrapper/s3_data_wrapper.py
-src/vectice/models/datasource/datawrapper/metadata/__init__.py
-src/vectice/models/datasource/datawrapper/metadata/db_metadata.py
-src/vectice/models/datasource/datawrapper/metadata/files_metadata.py
-src/vectice/models/datasource/datawrapper/metadata/metadata.py
 src/vectice/models/resource/__init__.py
 src/vectice/models/resource/base.py
 src/vectice/models/resource/bigquery_resource.py
 src/vectice/models/resource/description.py
 src/vectice/models/resource/file_resource.py
 src/vectice/models/resource/gcs_resource.py
 src/vectice/models/resource/s3_resource.py
```

### Comparing `vectice-23.2.1.1/src/vectice.egg-info/requires.txt` & `vectice-23.2.2.1/src/vectice.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -43,7 +43,8 @@
 pytest
 pytest-randomly
 coverage
 pytest-cov
 scikit-learn<=0.24.2
 testcontainers
 testbook
+db-dtypes>=1.1.1
```

