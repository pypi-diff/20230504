# Comparing `tmp/unify-sdk-4.0.2.tar.gz` & `tmp/unify-sdk-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-sdk-4.0.2.tar", last modified: Mon Mar  6 17:44:57 2023, max compression
+gzip compressed data, was "dist/unify-sdk-4.1.0.tar", last modified: Thu May  4 21:28:41 2023, max compression
```

## Comparing `unify-sdk-4.0.2.tar` & `unify-sdk-4.1.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2331 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1774 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2581 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3881 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/disable_test_connectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3811 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/disable_test_connectors_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7017 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_aa_permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4821 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_api_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4416 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_api_manager_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_asset_access.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2600 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_graph_v2.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_graph_v2_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1852 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_hierarchies.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1747 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_hierarchies_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_org_admin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2958 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_org_admin_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8643 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_pipelines.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8064 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_pipelines_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2388 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_properties.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10038 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_sources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6669 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_sources_default_org.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3616 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3390 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/tests/test_templates_default_org.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/Unify.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4376 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/WaitingLibrary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    44899 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/apimanager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8167 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/apirequestsmng.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/apiutils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3609 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/assetaccess.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/clusters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11459 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/connectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3057 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/generalutils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5142 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/graph.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify/helpers/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify/helpers/Permissions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      864 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/Permissions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/SingleOrg.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify/helpers/datasets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/datasets/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2084 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/datasets/column.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify/helpers/graph_ql/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/graph_ql/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/graph_ql/dataset_gql.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10009 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/graph_ql/graphql.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/graph_ql/permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5401 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/graph_ql/pipeline_gql.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify/helpers/pipeline/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/pipeline/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      449 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/pipeline/flow_column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/pipeline/schema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/staticsql.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify/helpers/unify_objects/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1001 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/unify_objects/Template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/helpers/unify_objects/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5399 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/hierarchies.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16874 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/orgadmin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8738 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/permissions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30555 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/pipelines.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14043 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/properties.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    52294 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/sources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21586 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3803 2023-03-06 17:44:51.000000 unify-sdk-4.0.2/unify/users.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify_sdk.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2023-03-06 17:44:57.000000 unify-sdk-4.0.2/unify_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2331 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1774 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2581 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3881 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/disable_test_connectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3811 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/disable_test_connectors_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7017 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_aa_permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4821 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_api_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4416 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_api_manager_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1481 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_asset_access.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2600 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_graph_v2.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_graph_v2_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1852 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_hierarchies.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1747 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_hierarchies_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_org_admin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2958 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_org_admin_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8643 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_pipelines.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8064 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_pipelines_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2388 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_properties.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10038 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_sources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6669 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_sources_default_org.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3616 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3390 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/tests/test_templates_default_org.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/Unify.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4376 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/WaitingLibrary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    44927 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/apimanager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8167 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/apirequestsmng.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2950 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/apiutils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3609 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/assetaccess.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1480 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/clusters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11459 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/connectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3057 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/generalutils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5142 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/graph.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/Permissions/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      864 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/Permissions/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      450 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/SingleOrg.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/datasets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/datasets/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2084 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/datasets/column.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/dataset_gql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10009 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/graphql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7479 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5401 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/graph_ql/pipeline_gql.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/pipeline/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/pipeline/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      449 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/pipeline/flow_column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/pipeline/schema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      894 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/staticsql.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify/helpers/unify_objects/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1001 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/unify_objects/Template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/helpers/unify_objects/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5399 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/hierarchies.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16874 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/orgadmin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8738 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/permissions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30555 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/pipelines.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14043 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/properties.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    52295 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/sources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21586 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3803 2023-05-04 21:28:33.000000 unify-sdk-4.1.0/unify/users.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-04 21:28:41.000000 unify-sdk-4.1.0/unify_sdk.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2747 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1728 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       75 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2023-05-04 21:28:40.000000 unify-sdk-4.1.0/unify_sdk.egg-info/top_level.txt
```

### Comparing `unify-sdk-4.0.2/LICENSE` & `unify-sdk-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/PKG-INFO` & `unify-sdk-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-sdk
-Version: 4.0.2
+Version: 4.1.0
 Summary: Unify Python SDK
 Home-page: https://github.com/ElementAnalytics/unify-python-sdk
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-sdk-4.0.2/README.md` & `unify-sdk-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/setup.py` & `unify-sdk-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/__init__.py` & `unify-sdk-4.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/disable_test_connectors.py` & `unify-sdk-4.1.0/tests/disable_test_connectors.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/disable_test_connectors_default_org.py` & `unify-sdk-4.1.0/tests/disable_test_connectors_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_aa_permissions.py` & `unify-sdk-4.1.0/tests/test_aa_permissions.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_api_manager.py` & `unify-sdk-4.1.0/tests/test_api_manager.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_api_manager_default_org.py` & `unify-sdk-4.1.0/tests/test_api_manager_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_asset_access.py` & `unify-sdk-4.1.0/tests/test_asset_access.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_graph_v2.py` & `unify-sdk-4.1.0/tests/test_graph_v2.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_graph_v2_default_org.py` & `unify-sdk-4.1.0/tests/test_graph_v2_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_hierarchies.py` & `unify-sdk-4.1.0/tests/test_hierarchies.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_hierarchies_default_org.py` & `unify-sdk-4.1.0/tests/test_hierarchies_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_org_admin.py` & `unify-sdk-4.1.0/tests/test_org_admin.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_org_admin_default_org.py` & `unify-sdk-4.1.0/tests/test_org_admin_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_pipelines.py` & `unify-sdk-4.1.0/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_pipelines_default_org.py` & `unify-sdk-4.1.0/tests/test_pipelines_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_properties.py` & `unify-sdk-4.1.0/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_sources.py` & `unify-sdk-4.1.0/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_sources_default_org.py` & `unify-sdk-4.1.0/tests/test_sources_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_templates.py` & `unify-sdk-4.1.0/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/tests/test_templates_default_org.py` & `unify-sdk-4.1.0/tests/test_templates_default_org.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/WaitingLibrary.py` & `unify-sdk-4.1.0/unify/WaitingLibrary.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/apimanager.py` & `unify-sdk-4.1.0/unify/apimanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,15 +540,15 @@
         :param pipeline_id: Pipeline id
         :type pipeline_id: int or str
         :param skip: skip
         :type skip: list
         :return:
         """
 
-        sources = self.sources.get_sources(org_id=org_id)
+        sources = self.sources.get_sources(org_id=org_id, page_num=1, page_size=2000)
 
         source_id_to_data = {}
 
         result_data = []
 
         for source in sources:
             source_id_to_data[source["id"]["id"]] = source
```

### Comparing `unify-sdk-4.0.2/unify/apirequestsmng.py` & `unify-sdk-4.1.0/unify/apirequestsmng.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/apiutils.py` & `unify-sdk-4.1.0/unify/apiutils.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/assetaccess.py` & `unify-sdk-4.1.0/unify/assetaccess.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/clusters.py` & `unify-sdk-4.1.0/unify/clusters.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/connectors.py` & `unify-sdk-4.1.0/unify/connectors.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/generalutils.py` & `unify-sdk-4.1.0/unify/generalutils.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/graph.py` & `unify-sdk-4.1.0/unify/graph.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/helpers/Permissions/__init__.py` & `unify-sdk-4.1.0/unify/helpers/Permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/helpers/datasets/column.py` & `unify-sdk-4.1.0/unify/helpers/datasets/column.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/helpers/graph_ql/dataset_gql.py` & `unify-sdk-4.1.0/unify/helpers/graph_ql/dataset_gql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/helpers/graph_ql/graphql.py` & `unify-sdk-4.1.0/unify/helpers/graph_ql/graphql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/helpers/graph_ql/permissions.py` & `unify-sdk-4.1.0/unify/helpers/graph_ql/permissions.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/helpers/graph_ql/pipeline_gql.py` & `unify-sdk-4.1.0/unify/helpers/graph_ql/pipeline_gql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/helpers/pipeline/schema.py` & `unify-sdk-4.1.0/unify/helpers/pipeline/schema.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/helpers/staticsql.py` & `unify-sdk-4.1.0/unify/helpers/staticsql.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/helpers/unify_objects/Template.py` & `unify-sdk-4.1.0/unify/helpers/unify_objects/Template.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/hierarchies.py` & `unify-sdk-4.1.0/unify/hierarchies.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/orgadmin.py` & `unify-sdk-4.1.0/unify/orgadmin.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/permissions.py` & `unify-sdk-4.1.0/unify/permissions.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/pipelines.py` & `unify-sdk-4.1.0/unify/pipelines.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/properties.py` & `unify-sdk-4.1.0/unify/properties.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/sources.py` & `unify-sdk-4.1.0/unify/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1200,15 +1200,15 @@
 
         if post_upload_file.status_code == 200:
             return json.loads(post_upload_file.content)
 
         raise Exception(repr(post_upload_file.content))
 
     @single_org
-    def get_sources(self, org_id=None, page_num=1, page_size=200):
+    def get_sources(self, org_id=None, page_num=1, page_size=1000):
 
         """
         Retrieves all the metadata of datasets on an org.
 
         :param org_id: Org to be queried
         :type org_id: int or str
         :param page_num: pagination page number
```

### Comparing `unify-sdk-4.0.2/unify/templates.py` & `unify-sdk-4.1.0/unify/templates.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify/users.py` & `unify-sdk-4.1.0/unify/users.py`

 * *Files identical despite different names*

### Comparing `unify-sdk-4.0.2/unify_sdk.egg-info/PKG-INFO` & `unify-sdk-4.1.0/unify_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-sdk
-Version: 4.0.2
+Version: 4.1.0
 Summary: Unify Python SDK
 Home-page: https://github.com/ElementAnalytics/unify-python-sdk
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-sdk-4.0.2/unify_sdk.egg-info/SOURCES.txt` & `unify-sdk-4.1.0/unify_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

