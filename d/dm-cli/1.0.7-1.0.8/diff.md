# Comparing `tmp/dm-cli-1.0.7.tar.gz` & `tmp/dm-cli-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-cli-1.0.7.tar", last modified: Thu Apr 27 06:54:53 2023, max compression
+gzip compressed data, was "dm-cli-1.0.8.tar", last modified: Thu May  4 11:36:37 2023, max compression
```

## Comparing `dm-cli-1.0.7.tar` & `dm-cli-1.0.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.470937 dm-cli-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 06:54:45.000000 dm-cli-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-27 06:54:53.470937 dm-cli-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-27 06:54:45.000000 dm-cli-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.462937 dm-cli-1.0.7/dm_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.462937 dm-cli-1.0.7/dm_cli/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/bin/dm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.462937 dm-cli-1.0.7/dm_cli/command_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/command_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/command_group/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/command_group/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.462937 dm-cli-1.0.7/dm_cli/dmss_api/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.466937 dm-cli-1.0.7/dm_cli/dmss_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/access_control_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/blob_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/blueprint_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/datasource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   150478 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/document_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/export_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/health_check_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/lookup_table_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/personal_access_token_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/reference_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api/whoami_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36779 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.466937 dm-cli-1.0.7/dm_cli/dmss_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/access_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/basic_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/data_source_information.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/data_source_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/get_blueprint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/pat_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/recipe_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/repository_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/storage_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/storage_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model/storage_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.466937 dm-cli-1.0.7/dm_cli/dmss_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/dmss_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/import_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/import_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/package_tree_from_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.466937 dm-cli-1.0.7/dm_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/utils/file_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/utils/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-27 06:54:45.000000 dm-cli-1.0.7/dm_cli/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:54:53.462937 dm-cli-1.0.7/dm_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-27 06:54:53.000000 dm-cli-1.0.7/dm_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-27 06:54:53.000000 dm-cli-1.0.7/dm_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:54:53.000000 dm-cli-1.0.7/dm_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 06:54:53.000000 dm-cli-1.0.7/dm_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 06:54:53.000000 dm-cli-1.0.7/dm_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 06:54:45.000000 dm-cli-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:54:53.470937 dm-cli-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 06:54:45.000000 dm-cli-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.755676 dm-cli-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 11:36:27.000000 dm-cli-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-04 11:36:37.755676 dm-cli-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-04 11:36:27.000000 dm-cli-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.747676 dm-cli-1.0.8/dm_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.747676 dm-cli-1.0.8/dm_cli/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/bin/dm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.747676 dm-cli-1.0.8/dm_cli/command_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/command_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/command_group/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/command_group/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.751676 dm-cli-1.0.8/dm_cli/dmss_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.751676 dm-cli-1.0.8/dm_cli/dmss_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/access_control_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/blob_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/blueprint_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/datasource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150478 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/document_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/export_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/health_check_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/lookup_table_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/personal_access_token_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/reference_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api/whoami_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36779 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.755676 dm-cli-1.0.8/dm_cli/dmss_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/access_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/basic_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/data_source_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/data_source_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/get_blueprint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/pat_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/recipe_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/repository_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/storage_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/storage_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model/storage_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.755676 dm-cli-1.0.8/dm_cli/dmss_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/dmss_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/import_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/import_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/package_tree_from_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.755676 dm-cli-1.0.8/dm_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/file_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-04 11:36:27.000000 dm-cli-1.0.8/dm_cli/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:36:37.747676 dm-cli-1.0.8/dm_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 11:36:37.000000 dm-cli-1.0.8/dm_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-04 11:36:27.000000 dm-cli-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:36:37.755676 dm-cli-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-04 11:36:27.000000 dm-cli-1.0.8/setup.py
```

### Comparing `dm-cli-1.0.7/PKG-INFO` & `dm-cli-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-cli
-Version: 1.0.7
+Version: 1.0.8
 Summary: UNKNOWN
 Home-page: https://github.com/equinor/dm-cli
 Author: 
 Author-email: 
 License: MIT
 Description: [![PyPi version](https://img.shields.io/pypi/v/dm-cli)](https://pypi.org/project/dm-cli)
         [![PyPi downloads](https://img.shields.io/pypi/dm/dm-cli)](https://pypi.org/project/dm-cli)
```

### Comparing `dm-cli-1.0.7/README.md` & `dm-cli-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/bin/dm` & `dm-cli-1.0.8/dm_cli/bin/dm`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/command_group/data_source.py` & `dm-cli-1.0.8/dm_cli/command_group/data_source.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/command_group/entities.py` & `dm-cli-1.0.8/dm_cli/command_group/entities.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss.py` & `dm-cli-1.0.8/dm_cli/dmss.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import json
-import traceback
 from typing import Any, Callable
 
 import requests
 import typer
-from rich import print
+from rich.console import Console
+from rich.text import Text
 
 from dm_cli.dmss_api import ApiException
 from dm_cli.dmss_api.api.default_api import DefaultApi
 from dm_cli.dmss_api.exceptions import NotFoundException
 from dm_cli.state import state
 
+console = Console()
+
 dmss_api = DefaultApi()
 
 
 class ApplicationException(Exception):
     status: int = 500
     type: str = "ApplicationException"
     message: str = "The requested operation failed"
@@ -64,17 +66,25 @@
 def dmss_exception_wrapper(
     function: Callable,
     *args,
     **kwargs,
 ) -> Any:
     try:
         return function(*args, **kwargs)
-    except (ApplicationException, NotFoundException, ApiException) as e:
+    except ApplicationException as e:
+        if state.debug:
+            console.print_exception()
+        exception = e.dict()
+        console.print(exception, style="red1")
+        raise typer.Exit(code=1)
+    except (NotFoundException, ApiException) as e:
         if state.debug:
-            traceback.print_exc()
+            console.print_exception()
         exception = json.loads(e.body)
-        print(exception)
+        console.print(exception, style="red1")
         raise typer.Exit(code=1)
     except Exception as error:
-        traceback.print_exc()
-        print(error)
+        if state.debug:
+            console.print_exception()
+        text = Text(str(error))
+        console.print(text, style="red1")
         raise typer.Exit(code=1)
```

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/__init__.py` & `dm-cli-1.0.8/dm_cli/dmss_api/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/access_control_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/access_control_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/blob_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/blob_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/blueprint_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/blueprint_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/datasource_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/datasource_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/default_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/default_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/document_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/document_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/entity_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/entity_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/export_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/health_check_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/health_check_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/lookup_table_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/lookup_table_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/personal_access_token_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/personal_access_token_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/reference_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/reference_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/search_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/search_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api/whoami_api.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api/whoami_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/api_client.py` & `dm-cli-1.0.8/dm_cli/dmss_api/api_client.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/configuration.py` & `dm-cli-1.0.8/dm_cli/dmss_api/configuration.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/exceptions.py` & `dm-cli-1.0.8/dm_cli/dmss_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/access_level.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/access_level.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/acl.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/acl.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/basic_entity.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/basic_entity.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/data_source_information.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/data_source_information.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/data_source_request.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/data_source_request.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/entity.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/entity.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/error_response.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/error_response.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/get_blueprint_response.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/get_blueprint_response.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/lookup.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/lookup.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/pat_data.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/pat_data.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/recipe.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/recipe.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/recipe_attribute.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/recipe_attribute.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/reference.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/reference.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/repository.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/repository.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/repository_type.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/repository_type.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/storage_attribute.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/storage_attribute.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/storage_data_types.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/storage_data_types.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model/storage_recipe.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model/storage_recipe.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/model_utils.py` & `dm-cli-1.0.8/dm_cli/dmss_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/models/__init__.py` & `dm-cli-1.0.8/dm_cli/dmss_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/dmss_api/rest.py` & `dm-cli-1.0.8/dm_cli/dmss_api/rest.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/domain.py` & `dm-cli-1.0.8/dm_cli/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,33 +88,33 @@
 
     def _content_to_ref_dict(self):
         result = []
         for child in self.content:
             if isinstance(child, Package):
                 result.append(
                     {
-                        "address": str(child.uid),
+                        "address": f"${str(child.uid)}",
                         "type": "dmss://system/SIMOS/Reference",
                         "referenceType": "link",
                     }
                 )
             else:  # Assume the child is a dict
                 if "name" in child:
                     result.append(
                         {
-                            "address": child["_id"],
+                            "address": f"${child['_id']}",
                             "type": "dmss://system/SIMOS/Reference",
                             "referenceType": "link",
                         }
                     )
 
                 else:
                     result.append(
                         {
-                            "address": child["_id"],
+                            "address": f"${child['_id']}",
                             "type": "dmss://system/SIMOS/Reference",
                             "referenceType": "link",
                         }
                     )
         return result
```

### Comparing `dm-cli-1.0.7/dm_cli/enums.py` & `dm-cli-1.0.8/dm_cli/enums.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/import_entity.py` & `dm-cli-1.0.8/dm_cli/import_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     )
 
 
 def import_folder_entity(source_path: Path, destination: str) -> None:
     print(f"Importing PACKAGE '{source_path.name}' --> '{destination}/'")
     destination_path = Path(destination)
     data_source = destination_path.parts[0]
+
     try:  # Check if target already exists on remote. Then delete or raise exception
         dmss_api.document_get_by_path(f"dmss://{destination}/{source_path.name}")
         if not state.force:
             raise ValueError(f"Failed to upload to 'dmss://{destination}/{source_path.name}' - It already exists.")
         console.print(
             f"WARNING: '{destination}/{source_path.name}' already exists. Replacing it...", style="dark_orange"
         )
```

### Comparing `dm-cli-1.0.7/dm_cli/import_package.py` & `dm-cli-1.0.8/dm_cli/import_package.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/package_tree_from_zip.py` & `dm-cli-1.0.8/dm_cli/package_tree_from_zip.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/utils/file_structure.py` & `dm-cli-1.0.8/dm_cli/utils/file_structure.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli/utils/reference.py` & `dm-cli-1.0.8/dm_cli/utils/reference.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,26 +93,32 @@
             dependencies,
             data_source,
             file_path,
         )
 
     # If the value is a complex type, dig down recursively.
     if isinstance(value, dict) and value != {}:
+        if not value.get("type"):
+            raise KeyError(f"Object with key '{key}' is missing the required 'type' attribute. File: '{file_path}'")
         # First check if the type is a blob type
         if (
             replace_relative_references(
                 "type",
                 value["type"],
                 dependencies,
                 data_source,
                 file_path=file_path,
                 zip_file=zip_file,
             )
             == SIMOS.BLOB.value
         ):
+            if not value.get("name"):
+                raise KeyError(
+                    f"Blob object with key '{key}' is missing the required 'name' attribute. File: '{file_path}'"
+                )
             # Add blob data to the blob-entity
             if parent_directory:  # entity
                 _blob_data = None
                 # value['name'] must be relative to the parent directory of the document accessing it
                 _blob_path = parent_directory.joinpath(value["name"])
                 if not _blob_path.is_file():
                     raise FileNotFoundError(
```

### Comparing `dm-cli-1.0.7/dm_cli/utils/utils.py` & `dm-cli-1.0.8/dm_cli/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     return document
 
 
 def add_package_to_path(name: str, path: Path):
     package = Package(name, is_root=len(path.parts) == 2)
     dmss_api.document_add_to_path(
-        str(path.parent),
+        f"/{str(path.parent)}/",
         json.dumps(package.to_dict()),
         update_uncontained=False,
         files=[],
     )
 
 
 def destination_is_root(destination: Path) -> bool:
@@ -116,18 +116,18 @@
         return False
     return True
 
 
 def ensure_package_structure(path: Path):
     """Create any missing packages in the provided path (mkdir -R)"""
     try:
-        dmss_api.document_get_by_path(f"dmss://{path}")
+        dmss_api.document_get_by_path(f"dmss://{path}/")
     except NotFoundException as e:
         error = json.loads(e.body)
-        if str(f"{path}") not in error["message"]:
+        if error["status"] != 404:
             print(f"Target package '{path}' is likely corrupt!")
             pprint.pformat(error)
             raise typer.Exit(code=1)
 
         if len(path.parts) > 2:  # We're at root package level. Do not check for datasource.
             ensure_package_structure(path.parent)
```

### Comparing `dm-cli-1.0.7/dm_cli/utils/zip.py` & `dm-cli-1.0.8/dm_cli/utils/zip.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/dm_cli.egg-info/PKG-INFO` & `dm-cli-1.0.8/dm_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-cli
-Version: 1.0.7
+Version: 1.0.8
 Summary: UNKNOWN
 Home-page: https://github.com/equinor/dm-cli
 Author: 
 Author-email: 
 License: MIT
 Description: [![PyPi version](https://img.shields.io/pypi/v/dm-cli)](https://pypi.org/project/dm-cli)
         [![PyPi downloads](https://img.shields.io/pypi/dm/dm-cli)](https://pypi.org/project/dm-cli)
```

### Comparing `dm-cli-1.0.7/dm_cli.egg-info/SOURCES.txt` & `dm-cli-1.0.8/dm_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.7/setup.py` & `dm-cli-1.0.8/setup.py`

 * *Files identical despite different names*

