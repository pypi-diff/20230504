# Comparing `tmp/apache-airflow-client-2.6.0rc1.tar.gz` & `tmp/apache-airflow-client-2.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-client-2.6.0rc1.tar", last modified: Tue May  2 08:06:46 2023, max compression
+gzip compressed data, was "apache-airflow-client-2.6.0rc2.tar", last modified: Thu May  4 19:16:10 2023, max compression
```

## Comparing `apache-airflow-client-2.6.0rc1.tar` & `apache-airflow-client-2.6.0rc2.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-02 08:06:46.208565 apache-airflow-client-2.6.0rc1/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10850 2023-05-01 07:39:05.000000 apache-airflow-client-2.6.0rc1/LICENSE
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)      240 2023-05-01 07:39:05.000000 apache-airflow-client-2.6.0rc1/NOTICE
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     3517 2023-05-02 08:06:46.208662 apache-airflow-client-2.6.0rc1/PKG-INFO
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     2745 2023-05-01 07:39:05.000000 apache-airflow-client-2.6.0rc1/README.md
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-02 08:06:46.111309 apache-airflow-client-2.6.0rc1/airflow_client/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)      786 2023-05-01 07:45:39.000000 apache-airflow-client-2.6.0rc1/airflow_client/__init__.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-02 08:06:46.114620 apache-airflow-client-2.6.0rc1/airflow_client/client/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9469 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/__init__.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-02 08:06:46.123212 apache-airflow-client-2.6.0rc1/airflow_client/client/api/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1010 2023-05-01 07:45:52.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    13912 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/config_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    39453 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/connection_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    68995 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/dag_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    61136 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/dag_run_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    15578 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/dag_warning_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    32065 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/dataset_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19786 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/event_log_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19839 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/import_error_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    18299 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/monitoring_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14726 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/permission_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14713 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/plugin_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34071 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/pool_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14163 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/provider_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34385 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/role_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    86070 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/task_instance_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34688 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/user_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34669 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/variable_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22471 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api/x_com_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    46315 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/api_client.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-02 08:06:46.123592 apache-airflow-client-2.6.0rc1/airflow_client/client/apis/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     2311 2023-05-01 07:45:52.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/apis/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25521 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/configuration.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    13735 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/exceptions.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-02 08:06:46.165528 apache-airflow-client-2.6.0rc1/airflow_client/client/model/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1134 2023-05-01 07:45:52.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19754 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/action.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22638 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/action_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19906 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/action_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20186 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/action_resource.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22780 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/basic_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20016 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/class_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20119 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/clear_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25069 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/clear_task_instances.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19963 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/collection_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20183 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/color.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19916 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/config.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19932 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/config_option.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20133 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/config_section.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24401 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20133 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22818 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20066 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21445 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20058 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_test.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19944 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/cron_expression.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    31162 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22578 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19861 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    37978 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_detail.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24600 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_detail_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26979 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22645 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_run_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19912 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_run_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20424 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_schedule_dataset_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20696 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20702 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_warning.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22730 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_warning_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19977 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_warning_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21910 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22658 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19921 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22564 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_event.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22765 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_event_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20002 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_event_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21570 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/error.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22192 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/event_log.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22685 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/event_log_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19942 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/event_log_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20347 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/extra_link.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19942 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/extra_link_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20344 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/health_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20296 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/health_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20705 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/import_error.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22745 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/import_error_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19987 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/import_error_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19972 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/inline_response200.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19727 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/inline_response2001.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21791 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/job.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24932 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/list_dag_runs_form.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25493 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/list_task_instance_form.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19929 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/metadatabase_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22738 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/plugin_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20006 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/plugin_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23769 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/plugin_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21899 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/pool.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22598 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/pool_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19876 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/pool_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20326 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/provider.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19921 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/provider_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22954 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/relative_delta.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19734 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/resource.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20389 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/role.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22598 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/role_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19876 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/role_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25358 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/schedule_interval.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20383 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/scheduler_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19789 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/set_dag_run_note.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19851 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/set_task_instance_note.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21102 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/sla_miss.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19667 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/tag.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26335 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19861 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19946 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_extra_links.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26317 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22765 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20002 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20589 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20078 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance_reference_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20679 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_outlet_dataset_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22425 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20420 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/time_delta.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20529 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/trigger.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21623 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/trigger_rule.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19905 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/update_dag_run_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20488 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/update_task_instance.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22917 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/update_task_instances_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26417 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/user.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19705 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22698 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19976 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23995 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19726 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_collection_item_roles.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22594 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19702 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22778 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20036 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20083 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20090 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/version_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20382 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/weight_rule.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23014 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19712 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22735 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20012 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20519 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    90756 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/model_utils.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-02 08:06:46.165938 apache-airflow-client-2.6.0rc1/airflow_client/client/models/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9137 2023-05-01 07:45:52.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/models/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22866 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/client/rest.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-02 08:06:46.206725 apache-airflow-client-2.6.0rc1/airflow_client/test/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)      786 2023-05-01 07:45:52.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/__init__.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9459 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_action.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9875 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_action_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9650 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_action_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9690 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_action_resource.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9588 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_basic_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9516 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_class_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9496 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_clear_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9545 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_clear_task_instances.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9516 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_collection_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9452 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_color.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9571 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_config.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9460 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_config_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9502 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_config_option.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9617 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_config_section.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9765 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9524 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10210 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9993 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9752 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9587 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9516 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_test.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9516 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_cron_expression.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9633 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10904 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9830 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9617 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9961 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_detail.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9614 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_detail_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9552 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_run.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10648 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_run_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9878 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_run_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9652 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_run_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9609 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_schedule_dataset_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9474 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9488 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_warning.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9485 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_warning_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9938 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_warning_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9696 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_warning_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9802 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9923 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9890 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9661 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9607 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_event.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9968 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_event_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9718 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_event_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9452 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_error.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9474 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_event_log.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9608 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_event_log_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9908 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_event_log_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9674 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_event_log_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9597 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_extra_link.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9648 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_extra_link_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9740 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_health_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9502 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_health_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9495 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_import_error.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9641 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_import_error_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9953 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_import_error_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9707 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_import_error_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9537 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_inline_response200.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9544 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_inline_response2001.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9438 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_job.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9525 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_list_dag_runs_form.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9656 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_list_task_instance_form.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9652 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_metadatabase_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9616 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_monitoring_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9481 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_permission_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9465 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_plugin_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9933 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_plugin_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9708 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_plugin_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9559 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_plugin_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9445 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_pool.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9946 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_pool_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9845 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_pool_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9628 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_pool_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9473 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_provider.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9465 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_provider_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9635 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_provider_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9509 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_relative_delta.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9473 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_resource.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9561 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_role.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9946 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_role_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9845 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_role_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9628 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_role_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9854 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_schedule_interval.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9631 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_scheduler_status.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9511 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_set_dag_run_note.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9553 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_set_task_instance_note.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9467 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_sla_miss.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9438 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_tag.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10128 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9591 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9633 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_extra_links.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9844 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    11146 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9968 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9718 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9566 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9782 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_reference_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9602 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_outlet_dataset_reference.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9481 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9481 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_time_delta.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9466 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_trigger.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9495 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_trigger_rule.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9539 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_update_dag_run_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9545 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_update_task_instance.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9588 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_update_task_instances_state.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9829 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_user.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9482 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9946 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9903 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9686 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9699 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9581 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_collection_item_roles.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9735 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9510 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10028 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9963 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9730 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9573 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_collection_item.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9495 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_version_info.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9488 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_weight_rule.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9678 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9483 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9597 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_api.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9906 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_collection.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9688 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_collection_all_of.py
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9546 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_collection_item.py
-drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-02 08:06:46.208350 apache-airflow-client-2.6.0rc1/apache_airflow_client.egg-info/
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     3517 2023-05-02 08:06:46.000000 apache-airflow-client-2.6.0rc1/apache_airflow_client.egg-info/PKG-INFO
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)    12437 2023-05-02 08:06:46.000000 apache-airflow-client-2.6.0rc1/apache_airflow_client.egg-info/SOURCES.txt
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)        1 2023-05-02 08:06:46.000000 apache-airflow-client-2.6.0rc1/apache_airflow_client.egg-info/dependency_links.txt
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)        1 2023-05-02 07:55:57.000000 apache-airflow-client-2.6.0rc1/apache_airflow_client.egg-info/not-zip-safe
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)       32 2023-05-02 08:06:46.000000 apache-airflow-client-2.6.0rc1/apache_airflow_client.egg-info/requires.txt
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)       15 2023-05-02 08:06:46.000000 apache-airflow-client-2.6.0rc1/apache_airflow_client.egg-info/top_level.txt
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)      726 2023-05-02 08:06:46.209036 apache-airflow-client-2.6.0rc1/setup.cfg
--rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1519 2023-05-02 07:36:33.000000 apache-airflow-client-2.6.0rc1/setup.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-04 19:16:10.515949 apache-airflow-client-2.6.0rc2/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10850 2023-05-04 18:47:01.000000 apache-airflow-client-2.6.0rc2/LICENSE
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)      240 2023-05-04 18:47:01.000000 apache-airflow-client-2.6.0rc2/NOTICE
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     3517 2023-05-04 19:16:10.516115 apache-airflow-client-2.6.0rc2/PKG-INFO
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     2745 2023-05-04 18:47:01.000000 apache-airflow-client-2.6.0rc2/README.md
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-04 19:16:10.423638 apache-airflow-client-2.6.0rc2/airflow_client/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)      786 2023-05-04 18:58:57.000000 apache-airflow-client-2.6.0rc2/airflow_client/__init__.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-04 19:16:10.426542 apache-airflow-client-2.6.0rc2/airflow_client/client/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9469 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/__init__.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-04 19:16:10.433738 apache-airflow-client-2.6.0rc2/airflow_client/client/api/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1010 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    13912 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/config_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    39453 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/connection_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    68995 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/dag_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    61136 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/dag_run_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    15578 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/dag_warning_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    32065 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/dataset_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19786 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/event_log_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19839 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/import_error_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    18299 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/monitoring_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14726 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/permission_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14713 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/plugin_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34071 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/pool_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    14163 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/provider_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34385 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/role_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    86070 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/task_instance_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34688 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/user_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    34669 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/variable_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22471 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api/x_com_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    46315 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/api_client.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-04 19:16:10.434092 apache-airflow-client-2.6.0rc2/airflow_client/client/apis/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     2311 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/apis/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25521 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/configuration.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    13735 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/exceptions.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-04 19:16:10.475553 apache-airflow-client-2.6.0rc2/airflow_client/client/model/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1134 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19754 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/action.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22638 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/action_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19906 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/action_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20186 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/action_resource.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22780 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/basic_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20016 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/class_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20119 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/clear_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25069 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/clear_task_instances.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19963 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/collection_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20183 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/color.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19916 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/config.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19932 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/config_option.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20133 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/config_section.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24401 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20133 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22818 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20066 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21445 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20058 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_test.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19944 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/cron_expression.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    31162 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22578 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19861 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    37978 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_detail.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24633 2023-05-04 19:00:53.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_detail_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26979 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22645 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_run_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19912 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_run_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20424 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_schedule_dataset_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20696 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20702 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_warning.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22730 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_warning_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19977 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_warning_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21910 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22658 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19921 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22564 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_event.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22765 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_event_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20002 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_event_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21570 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/error.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22192 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/event_log.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22685 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/event_log_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19942 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/event_log_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20347 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/extra_link.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19942 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/extra_link_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20344 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/health_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20296 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/health_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20705 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/import_error.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22745 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/import_error_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19987 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/import_error_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19972 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/inline_response200.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19727 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/inline_response2001.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21791 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/job.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    24932 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/list_dag_runs_form.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25493 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/list_task_instance_form.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19929 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/metadatabase_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22738 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/plugin_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20006 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/plugin_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23769 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/plugin_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21899 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/pool.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22598 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/pool_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19876 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/pool_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20326 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/provider.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19921 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/provider_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22954 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/relative_delta.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19734 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/resource.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20389 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/role.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22598 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/role_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19876 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/role_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    25358 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/schedule_interval.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20383 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/scheduler_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19789 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/set_dag_run_note.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19851 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/set_task_instance_note.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21102 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/sla_miss.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19667 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/tag.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26368 2023-05-04 19:00:53.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19861 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19946 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_extra_links.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26317 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22765 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20002 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20589 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20078 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance_reference_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20679 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_outlet_dataset_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22425 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20420 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/time_delta.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20529 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/trigger.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    21623 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/trigger_rule.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19905 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/update_dag_run_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20488 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/update_task_instance.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22917 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/update_task_instances_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    26417 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/user.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19705 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22698 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19976 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23995 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19726 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_collection_item_roles.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22594 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19702 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22778 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20036 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20083 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20090 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/version_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20382 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/weight_rule.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    23014 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    19712 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22735 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20012 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    20519 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    90756 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/model_utils.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-04 19:16:10.475783 apache-airflow-client-2.6.0rc2/airflow_client/client/models/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9137 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/models/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    22866 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/client/rest.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-04 19:16:10.514544 apache-airflow-client-2.6.0rc2/airflow_client/test/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)      786 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/__init__.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9459 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_action.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9875 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_action_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9650 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_action_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9690 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_action_resource.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9588 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_basic_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9516 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_class_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9496 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_clear_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9545 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_clear_task_instances.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9516 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_collection_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9452 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_color.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9571 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_config.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9460 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_config_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9502 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_config_option.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9617 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_config_section.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9765 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9524 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10210 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9993 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9752 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9587 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9516 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_test.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9516 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_cron_expression.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9633 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10904 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9830 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9617 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9961 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_detail.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9614 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_detail_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9552 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_run.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10648 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_run_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9878 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_run_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9652 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_run_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9609 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_schedule_dataset_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9474 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9488 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_warning.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9485 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_warning_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9938 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_warning_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9696 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_warning_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9802 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9923 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9890 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9661 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9607 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_event.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9968 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_event_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9718 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_event_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9452 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_error.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9474 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_event_log.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9608 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_event_log_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9908 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_event_log_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9674 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_event_log_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9597 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_extra_link.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9648 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_extra_link_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9740 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_health_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9502 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_health_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9495 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_import_error.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9641 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_import_error_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9953 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_import_error_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9707 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_import_error_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9537 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_inline_response200.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9544 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_inline_response2001.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9438 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_job.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9525 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_list_dag_runs_form.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9656 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_list_task_instance_form.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9652 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_metadatabase_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9616 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_monitoring_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9481 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_permission_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9465 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_plugin_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9933 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_plugin_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9708 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_plugin_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9559 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_plugin_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9445 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_pool.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9946 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_pool_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9845 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_pool_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9628 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_pool_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9473 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_provider.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9465 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_provider_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9635 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_provider_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9509 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_relative_delta.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9473 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_resource.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9561 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_role.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9946 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_role_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9845 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_role_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9628 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_role_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9854 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_schedule_interval.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9631 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_scheduler_status.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9511 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_set_dag_run_note.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9553 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_set_task_instance_note.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9467 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_sla_miss.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9438 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_tag.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10128 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9591 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9633 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_extra_links.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9844 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    11146 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9968 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9718 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9566 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9782 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_reference_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9602 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_outlet_dataset_reference.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9481 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9481 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_time_delta.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9466 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_trigger.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9495 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_trigger_rule.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9539 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_update_dag_run_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9545 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_update_task_instance.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9588 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_update_task_instances_state.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9829 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_user.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9482 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9946 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9903 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9686 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9699 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9581 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_collection_item_roles.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9735 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9510 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    10028 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9963 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9730 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9573 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_collection_item.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9495 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_version_info.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9488 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_weight_rule.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9678 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9483 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9597 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_api.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9906 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_collection.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9688 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_collection_all_of.py
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     9546 2023-05-04 18:58:58.000000 apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_collection_item.py
+drwxr-xr-x   0 ephraimbuddy   (502) staff       (20)        0 2023-05-04 19:16:10.515780 apache-airflow-client-2.6.0rc2/apache_airflow_client.egg-info/
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     3517 2023-05-04 19:16:10.000000 apache-airflow-client-2.6.0rc2/apache_airflow_client.egg-info/PKG-INFO
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)    12437 2023-05-04 19:16:10.000000 apache-airflow-client-2.6.0rc2/apache_airflow_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)        1 2023-05-04 19:16:10.000000 apache-airflow-client-2.6.0rc2/apache_airflow_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)        1 2023-05-04 19:08:26.000000 apache-airflow-client-2.6.0rc2/apache_airflow_client.egg-info/not-zip-safe
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)       32 2023-05-04 19:16:10.000000 apache-airflow-client-2.6.0rc2/apache_airflow_client.egg-info/requires.txt
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)       15 2023-05-04 19:16:10.000000 apache-airflow-client-2.6.0rc2/apache_airflow_client.egg-info/top_level.txt
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)      726 2023-05-04 19:16:10.516636 apache-airflow-client-2.6.0rc2/setup.cfg
+-rw-r--r--   0 ephraimbuddy   (502) staff       (20)     1519 2023-05-04 18:47:01.000000 apache-airflow-client-2.6.0rc2/setup.py
```

### Comparing `apache-airflow-client-2.6.0rc1/LICENSE` & `apache-airflow-client-2.6.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/PKG-INFO` & `apache-airflow-client-2.6.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-client
-Version: 2.6.0rc1
+Version: 2.6.0rc2
 Summary: Apache Airflow API (Stable)
 Home-page: https://airflow.apache.org/
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Download-URL: https://archive.apache.org/dist/airflow/clients/python/2.6.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow/stable/stable-rest-api-ref.html
```

### Comparing `apache-airflow-client-2.6.0rc1/README.md` & `apache-airflow-client-2.6.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/__init__.py` & `apache-airflow-client-2.6.0rc2/airflow_client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/__init__.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/__init__.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/config_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/config_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/connection_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/connection_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/dag_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/dag_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/dag_run_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/dag_run_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/dag_warning_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/dag_warning_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/dataset_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/event_log_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/event_log_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/import_error_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/import_error_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/monitoring_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/monitoring_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/permission_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/permission_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/plugin_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/plugin_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/pool_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/pool_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/provider_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/provider_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/role_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/role_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/task_instance_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/task_instance_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/user_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/variable_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/variable_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api/x_com_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api/x_com_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/api_client.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/api_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/apis/__init__.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/configuration.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/configuration.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/exceptions.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/__init__.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/action.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/action.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/action_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/action_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/action_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/action_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/action_resource.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/action_resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/basic_dag_run.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/basic_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/class_reference.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/class_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/clear_dag_run.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/clear_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/clear_task_instances.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/clear_task_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/collection_info.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/collection_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/color.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/color.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/config.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/config.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/config_option.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/config_option.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/config_section.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/config_section.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/connection_test.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/cron_expression.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/cron_expression.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_detail.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_detail.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_detail_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_detail_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         lazy_import()
         return {
             'timezone': (str,),  # noqa: E501
             'catchup': (bool,),  # noqa: E501
             'orientation': (str,),  # noqa: E501
             'concurrency': (float,),  # noqa: E501
             'start_date': (datetime, none_type,),  # noqa: E501
-            'dag_run_timeout': (TimeDelta,),  # noqa: E501
+            'dag_run_timeout': (TimeDelta, none_type,),  # noqa: E501
             'doc_md': (str, none_type,),  # noqa: E501
             'default_view': (str,),  # noqa: E501
             'params': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'end_date': (datetime, none_type,),  # noqa: E501
             'is_paused_upon_creation': (bool, none_type,),  # noqa: E501
             'last_parsed': (datetime, none_type,),  # noqa: E501
             'template_search_path': ([str], none_type,),  # noqa: E501
@@ -196,15 +196,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             timezone (str): [optional]  # noqa: E501
             catchup (bool): [optional]  # noqa: E501
             orientation (str): [optional]  # noqa: E501
             concurrency (float): [optional]  # noqa: E501
             start_date (datetime, none_type): The DAG's start date.  *Changed in version 2.0.1*&#58; Field becomes nullable. . [optional]  # noqa: E501
-            dag_run_timeout (TimeDelta): [optional]  # noqa: E501
+            dag_run_timeout (TimeDelta, none_type): [optional]  # noqa: E501
             doc_md (str, none_type): [optional]  # noqa: E501
             default_view (str): [optional]  # noqa: E501
             params ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): User-specified DAG params.  *New in version 2.0.1* . [optional]  # noqa: E501
             end_date (datetime, none_type): The DAG's end date.  *New in version 2.3.0*. . [optional]  # noqa: E501
             is_paused_upon_creation (bool, none_type): Whether the DAG is paused upon creation.  *New in version 2.3.0* . [optional]  # noqa: E501
             last_parsed (datetime, none_type): The last time the DAG was parsed.  *New in version 2.3.0* . [optional]  # noqa: E501
             template_search_path ([str], none_type): The template search path.  *New in version 2.3.0* . [optional]  # noqa: E501
@@ -291,15 +291,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             timezone (str): [optional]  # noqa: E501
             catchup (bool): [optional]  # noqa: E501
             orientation (str): [optional]  # noqa: E501
             concurrency (float): [optional]  # noqa: E501
             start_date (datetime, none_type): The DAG's start date.  *Changed in version 2.0.1*&#58; Field becomes nullable. . [optional]  # noqa: E501
-            dag_run_timeout (TimeDelta): [optional]  # noqa: E501
+            dag_run_timeout (TimeDelta, none_type): [optional]  # noqa: E501
             doc_md (str, none_type): [optional]  # noqa: E501
             default_view (str): [optional]  # noqa: E501
             params ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): User-specified DAG params.  *New in version 2.0.1* . [optional]  # noqa: E501
             end_date (datetime, none_type): The DAG's end date.  *New in version 2.3.0*. . [optional]  # noqa: E501
             is_paused_upon_creation (bool, none_type): Whether the DAG is paused upon creation.  *New in version 2.3.0* . [optional]  # noqa: E501
             last_parsed (datetime, none_type): The last time the DAG was parsed.  *New in version 2.3.0* . [optional]  # noqa: E501
             template_search_path ([str], none_type): The template search path.  *New in version 2.3.0* . [optional]  # noqa: E501
```

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_run.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_run_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_run_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_run_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_run_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_schedule_dataset_reference.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_schedule_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_state.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_warning.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_warning.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_warning_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_warning_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dag_warning_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dag_warning_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_event.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_event_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/dataset_event_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/dataset_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/error.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/event_log.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/event_log.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/event_log_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/event_log_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/event_log_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/event_log_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/extra_link.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/extra_link.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/extra_link_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/extra_link_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/health_info.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/health_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/health_status.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/health_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/import_error.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/import_error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/import_error_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/import_error_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/import_error_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/import_error_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/inline_response200.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/inline_response2001.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/job.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/job.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/list_dag_runs_form.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/list_dag_runs_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/list_task_instance_form.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/list_task_instance_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/metadatabase_status.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/metadatabase_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/plugin_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/plugin_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/plugin_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/plugin_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/plugin_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/plugin_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/pool.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/pool.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/pool_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/pool_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/pool_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/pool_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/provider.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/provider.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/provider_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/provider_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/relative_delta.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/relative_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/resource.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/role.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/role.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/role_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/role_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/role_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/role_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/schedule_interval.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/schedule_interval.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/scheduler_status.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/scheduler_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/set_dag_run_note.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/set_dag_run_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/set_task_instance_note.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/set_task_instance_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/sla_miss.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/sla_miss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/tag.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/tag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             'depends_on_past': (bool,),  # noqa: E501
             'is_mapped': (bool,),  # noqa: E501
             'wait_for_downstream': (bool,),  # noqa: E501
             'retries': (float,),  # noqa: E501
             'queue': (str, none_type,),  # noqa: E501
             'pool': (str,),  # noqa: E501
             'pool_slots': (float,),  # noqa: E501
-            'execution_timeout': (TimeDelta,),  # noqa: E501
+            'execution_timeout': (TimeDelta, none_type,),  # noqa: E501
             'retry_delay': (TimeDelta,),  # noqa: E501
             'retry_exponential_backoff': (bool,),  # noqa: E501
             'priority_weight': (float,),  # noqa: E501
             'weight_rule': (WeightRule,),  # noqa: E501
             'ui_color': (Color,),  # noqa: E501
             'ui_fgcolor': (Color,),  # noqa: E501
             'template_fields': ([str],),  # noqa: E501
@@ -242,15 +242,15 @@
             depends_on_past (bool): [optional]  # noqa: E501
             is_mapped (bool): [optional]  # noqa: E501
             wait_for_downstream (bool): [optional]  # noqa: E501
             retries (float): [optional]  # noqa: E501
             queue (str, none_type): [optional]  # noqa: E501
             pool (str): [optional]  # noqa: E501
             pool_slots (float): [optional]  # noqa: E501
-            execution_timeout (TimeDelta): [optional]  # noqa: E501
+            execution_timeout (TimeDelta, none_type): [optional]  # noqa: E501
             retry_delay (TimeDelta): [optional]  # noqa: E501
             retry_exponential_backoff (bool): [optional]  # noqa: E501
             priority_weight (float): [optional]  # noqa: E501
             weight_rule (WeightRule): [optional]  # noqa: E501
             ui_color (Color): [optional]  # noqa: E501
             ui_fgcolor (Color): [optional]  # noqa: E501
             template_fields ([str]): [optional]  # noqa: E501
@@ -347,15 +347,15 @@
             depends_on_past (bool): [optional]  # noqa: E501
             is_mapped (bool): [optional]  # noqa: E501
             wait_for_downstream (bool): [optional]  # noqa: E501
             retries (float): [optional]  # noqa: E501
             queue (str, none_type): [optional]  # noqa: E501
             pool (str): [optional]  # noqa: E501
             pool_slots (float): [optional]  # noqa: E501
-            execution_timeout (TimeDelta): [optional]  # noqa: E501
+            execution_timeout (TimeDelta, none_type): [optional]  # noqa: E501
             retry_delay (TimeDelta): [optional]  # noqa: E501
             retry_exponential_backoff (bool): [optional]  # noqa: E501
             priority_weight (float): [optional]  # noqa: E501
             weight_rule (WeightRule): [optional]  # noqa: E501
             ui_color (Color): [optional]  # noqa: E501
             ui_fgcolor (Color): [optional]  # noqa: E501
             template_fields ([str]): [optional]  # noqa: E501
```

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_extra_links.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_extra_links.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance_reference.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_instance_reference_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_instance_reference_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_outlet_dataset_reference.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_outlet_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/task_state.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/task_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/time_delta.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/time_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/trigger.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/trigger_rule.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/update_dag_run_state.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/update_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/update_task_instance.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/update_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/update_task_instances_state.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/update_task_instances_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/user.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/user.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/user_collection_item_roles.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/user_collection_item_roles.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/variable_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/variable_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/version_info.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/version_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/weight_rule.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/weight_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model/x_com_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model/x_com_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/model_utils.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/models/__init__.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/client/rest.py` & `apache-airflow-client-2.6.0rc2/airflow_client/client/rest.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/__init__.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_action.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_action.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_action_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_action_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_action_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_action_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_action_resource.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_action_resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_basic_dag_run.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_basic_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_class_reference.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_class_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_clear_dag_run.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_clear_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_clear_task_instances.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_clear_task_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_collection_info.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_collection_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_color.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_color.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_config.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_config.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_config_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_config_option.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_config_option.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_config_section.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_config_section.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_connection_test.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_connection_test.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_cron_expression.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_cron_expression.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_detail.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_detail.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_detail_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_run.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_run_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_run_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_run_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_run_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_run_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_run_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_schedule_dataset_reference.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_schedule_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_state.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_warning.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_warning.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_warning_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_warning_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_warning_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_warning_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dag_warning_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dag_warning_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_event.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_event_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_dataset_event_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_dataset_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_error.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_event_log.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_event_log.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_event_log_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_event_log_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_event_log_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_event_log_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_event_log_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_event_log_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_extra_link.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_extra_link.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_extra_link_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_extra_link_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_health_info.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_health_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_health_status.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_health_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_import_error.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_import_error.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_import_error_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_import_error_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_import_error_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_import_error_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_import_error_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_import_error_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_inline_response200.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_inline_response2001.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_job.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_job.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_list_dag_runs_form.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_list_dag_runs_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_list_task_instance_form.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_list_task_instance_form.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_metadatabase_status.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_metadatabase_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_monitoring_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_monitoring_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_permission_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_permission_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_plugin_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_plugin_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_plugin_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_plugin_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_plugin_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_plugin_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_plugin_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_plugin_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_pool.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_pool.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_pool_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_pool_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_pool_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_pool_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_pool_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_pool_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_provider.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_provider_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_provider_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_provider_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_provider_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_relative_delta.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_relative_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_resource.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_role.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_role.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_role_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_role_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_role_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_role_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_role_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_role_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_schedule_interval.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_schedule_interval.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_scheduler_status.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_scheduler_status.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_set_dag_run_note.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_set_dag_run_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_set_task_instance_note.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_set_task_instance_note.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_sla_miss.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_sla_miss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_tag.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_extra_links.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_extra_links.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_reference.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_instance_reference_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_instance_reference_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_outlet_dataset_reference.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_outlet_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_task_state.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_task_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_time_delta.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_time_delta.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_trigger.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_trigger_rule.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_trigger_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_update_dag_run_state.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_update_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_update_task_instance.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_update_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_update_task_instances_state.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_update_task_instances_state.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_user.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_user.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_user_collection_item_roles.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_user_collection_item_roles.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_variable_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_variable_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_version_info.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_version_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_weight_rule.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_weight_rule.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_api.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_collection.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_collection.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_collection_all_of.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/airflow_client/test/test_x_com_collection_item.py` & `apache-airflow-client-2.6.0rc2/airflow_client/test/test_x_com_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/apache_airflow_client.egg-info/PKG-INFO` & `apache-airflow-client-2.6.0rc2/apache_airflow_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-client
-Version: 2.6.0rc1
+Version: 2.6.0rc2
 Summary: Apache Airflow API (Stable)
 Home-page: https://airflow.apache.org/
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Download-URL: https://archive.apache.org/dist/airflow/clients/python/2.6.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow/stable/stable-rest-api-ref.html
```

### Comparing `apache-airflow-client-2.6.0rc1/apache_airflow_client.egg-info/SOURCES.txt` & `apache-airflow-client-2.6.0rc2/apache_airflow_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-client-2.6.0rc1/setup.cfg` & `apache-airflow-client-2.6.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -20,10 +20,10 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 python_requires = ~=3.6
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-client-2.6.0rc1/setup.py` & `apache-airflow-client-2.6.0rc2/setup.py`

 * *Files identical despite different names*

