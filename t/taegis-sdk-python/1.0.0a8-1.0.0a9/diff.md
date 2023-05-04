# Comparing `tmp/taegis-sdk-python-1.0.0a8.tar.gz` & `tmp/taegis-sdk-python-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taegis-sdk-python-1.0.0a8.tar", last modified: Tue Apr 25 17:56:51 2023, max compression
+gzip compressed data, was "taegis-sdk-python-1.0.0a9.tar", last modified: Thu May  4 18:48:20 2023, max compression
```

## Comparing `taegis-sdk-python-1.0.0a8.tar` & `taegis-sdk-python-1.0.0a9.tar`

### file list

```diff
@@ -1,184 +1,196 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.483963 taegis-sdk-python-1.0.0a8/
--rw-rw-rw-   0 root         (0) root         (0)    10173 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-25 17:56:29.000000 taegis-sdk-python-1.0.0a8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5757 2023-04-25 17:56:51.482963 taegis-sdk-python-1.0.0a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5320 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 17:56:51.483963 taegis-sdk-python-1.0.0a8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-04-25 17:56:29.000000 taegis-sdk-python-1.0.0a8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.458963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/_consts.py
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8552 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    10879 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/service_core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.459963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/
--rw-rw-rw-   0 root         (0) root         (0)    11799 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.460963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2370 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.461963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2560 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.461963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3851 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6644 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    78106 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.463963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6326 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    14905 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    23548 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.463963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9259 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    12852 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24754 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.464963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3040 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.465963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3843 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.466963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15774 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    22563 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    30929 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.467963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4105 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6219 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5118 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.468963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8546 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.469963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.470963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      851 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.470963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4228 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.471963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8988 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.472963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12950 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    10408 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    24248 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.473963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22054 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    27703 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    39186 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.474963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10512 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6558 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    36501 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.475963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     9242 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.476963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.477963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6809 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8811 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.478963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    16048 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22172 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.478963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/
--rw-rw-rw-   0 root         (0) root         (0)      941 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.479963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11568 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     5864 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    31540 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.480963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3394 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)    13732 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    53278 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.481963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     3856 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7946 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.482963 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11509 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     6309 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/queries.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/subscriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    25501 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/types.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     5811 2023-04-25 16:03:33.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 17:56:51.459963 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5757 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7173 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-25 17:56:51.000000 taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.536567 taegis-sdk-python-1.0.0a9/
+-rw-rw-rw-   0 root         (0) root         (0)    10173 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-05-04 18:48:20.536567 taegis-sdk-python-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 18:48:20.536567 taegis-sdk-python-1.0.0a9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.512569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8552 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    10956 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/service_core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.513569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/
+-rw-rw-rw-   0 root         (0) root         (0)    12477 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.514569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2370 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.515569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.516569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6644 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    78106 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.516569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    14905 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    23548 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.517569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9259 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    12852 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25353 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.518569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3040 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.519569 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.520568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15774 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    22563 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    30929 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.520568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6219 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.521568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3145 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/detector_registry/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.522568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8546 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.523568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.524568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      851 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.524568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4228 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.525568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8988 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.526568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12950 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10408 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    24248 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.527568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22054 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    27703 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    39186 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.528568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11536 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     7165 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    38776 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.528568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     9242 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.529568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.530568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6809 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.531568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5229 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12489 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/preferences/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.531568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    16048 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    22172 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.532568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/
+-rw-rw-rw-   0 root         (0) root         (0)      941 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.533568 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11568 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5864 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    31540 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.534567 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3394 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)    13732 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    53278 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.535567 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3856 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7946 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.535567 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11509 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6309 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/subscriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    25501 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     5811 2023-05-04 18:40:28.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:48:20.513569 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7717 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-04 18:48:20.000000 taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/top_level.txt
```

### Comparing `taegis-sdk-python-1.0.0a8/LICENSE` & `taegis-sdk-python-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/PKG-INFO` & `taegis-sdk-python-1.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.0a8/README.md` & `taegis-sdk-python-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/setup.py` & `taegis-sdk-python-1.0.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/_consts.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/_consts.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/authentication.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/config.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/config.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/errors.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/errors.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/service_core.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/service_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,24 +74,28 @@
         )
         client = Client(transport=transport, fetch_schema_from_transport=True)
         return client
 
     @property
     def ws_client(self) -> Client:
         """GraphQL WebSockets Transport with Client."""
+        subprotocols = [
+            "graphql-ws",
+            f"access-token-{self.service.access_token}",
+        ]
+
+        if self.service.tenant_id:
+            subprotocols.append(f"x-tenant-context-{self.service.tenant_id}")
+
         transport = WebsocketsTransport(
             f"{self.wss_url}{self.gateway}",
             headers={
                 "User-Agent": f"taegis_sdk_python/{__version__}",
             },
-            subprotocols=[
-                "graphql-ws",
-                f"x-tenant-context-{self.service.tenant_id}",
-                f"access-token-{self.service.access_token}",
-            ],
+            subprotocols=subprotocols,
             connect_args={"max_size": None},
         )
         client = Client(transport=transport, fetch_schema_from_transport=True)
         return client
 
     def get_sync_schema(self) -> GraphQLSchema:
         """Retrieves introspection schema from Synchronous endpoint.
```

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from taegis_sdk_python.services.alerts import AlertsService
 from taegis_sdk_python.services.assets import AssetsService
 from taegis_sdk_python.services.assets2 import Assets2Service
 from taegis_sdk_python.services.audits import AuditsService
 from taegis_sdk_python.services.clients import ClientsService
 from taegis_sdk_python.services.collector import CollectorService
 from taegis_sdk_python.services.comments import CommentsService
+from taegis_sdk_python.services.detector_registry import DetectorRegistryService
 from taegis_sdk_python.services.endpoint_command_manager import (
     EndpointCommandManagerService,
 )
 from taegis_sdk_python.services.endpoint_management_service import (
     EndpointManagementServiceService,
 )
 from taegis_sdk_python.services.entity_profile import EntityProfileService
@@ -28,14 +29,15 @@
 from taegis_sdk_python.services.events import EventsService
 from taegis_sdk_python.services.exports import ExportsService
 from taegis_sdk_python.services.investigations import InvestigationsService
 from taegis_sdk_python.services.investigations2 import Investigations2Service
 from taegis_sdk_python.services.mitre_attack_info import MitreAttackInfoService
 from taegis_sdk_python.services.notebooks import NotebooksService
 from taegis_sdk_python.services.notifications import NotificationsService
+from taegis_sdk_python.services.preferences import PreferencesService
 from taegis_sdk_python.services.rules import RulesService
 from taegis_sdk_python.services.sharelinks import SharelinksService
 from taegis_sdk_python.services.tenants import TenantsService
 from taegis_sdk_python.services.threat import ThreatService
 from taegis_sdk_python.services.trip import TripService
 from taegis_sdk_python.services.users import UsersService
 
@@ -87,25 +89,27 @@
         self._alerts = None
         self._assets = None
         self._assets2 = None
         self._audits = None
         self._clients = None
         self._collector = None
         self._comments = None
+        self._detector_registry = None
         self._endpoint_command_manager = None
         self._endpoint_management_service = None
         self._entity_profile = None
         self._event_search = None
         self._events = None
         self._exports = None
         self._investigations = None
         self._investigations2 = None
         self._mitre_attack_info = None
         self._notebooks = None
         self._notifications = None
+        self._preferences = None
         self._rules = None
         self._core = None
         self._sharelinks = None
         self._tenants = None
         self._threat = None
         self._trip = None
         self._users = None
@@ -239,14 +243,21 @@
     def comments(self):
         """Comments Service Endpoint."""
         if not self._comments:
             self._comments = CommentsService(self)
         return self._comments
 
     @property
+    def detector_registry(self):
+        """Detector Registry Service Endpoint."""
+        if not self._detector_registry:
+            self._detector_registry = DetectorRegistryService(self)
+        return self._detector_registry
+
+    @property
     def endpoint_command_manager(self):
         """Endpoint Command Manager Service Endpoint."""
         if not self._endpoint_command_manager:
             self._endpoint_command_manager = EndpointCommandManagerService(self)
         return self._endpoint_command_manager
 
     @property
@@ -316,14 +327,21 @@
     def notifications(self):
         """Notifications Service Endpoint."""
         if not self._notifications:
             self._notifications = NotificationsService(self)
         return self._notifications
 
     @property
+    def preferences(self):
+        """Preferences Service Endpoint."""
+        if not self._preferences:
+            self._preferences = PreferencesService(self)
+        return self._preferences
+
+    @property
     def rules(self):
         """Rules Service Endpoint."""
         if not self._rules:
             self._rules = RulesService(self)
         return self._rules
 
     @property
```

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/access_points/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/access_points/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/agent/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/agent/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/alerts/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/alerts/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/assets2/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/assets2/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,21 @@
     TAG_KEY_DESC = "tag_key_desc"
     TAG_VALUE_ASC = "tag_value_asc"
     TAG_VALUE_DESC = "tag_value_desc"
     TAG_ASC = "tag_asc"
     TAG_DESC = "tag_desc"
 
 
+class InvestigationsOrderByInput(str, Enum):
+    """InvestigationsOrderByInput."""
+
+    CREATED_AT_ASC = "created_at_asc"
+    CREATED_AT_DESC = "created_at_desc"
+
+
 class CanIsolateResponse(str, Enum):
     """CanIsolateResponse."""
 
     UNAUTHORIZED = "unauthorized"
     AUTHORIZED = "authorized"
     ALWAYS = "always"
 
@@ -195,18 +202,28 @@
     tag: Optional[str] = field(default=None, metadata=config(field_name="tag"))
     key: Optional[str] = field(default=None, metadata=config(field_name="key"))
     value: Optional[str] = field(default=None, metadata=config(field_name="value"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
-class Investigation:
-    """Investigation."""
+class AssetInvestigation:
+    """AssetInvestigation."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
+    investigation_id: Optional[str] = field(
+        default=None, metadata=config(field_name="investigationId")
+    )
+    created_at: Optional[str] = field(
+        default=None, metadata=config(field_name="createdAt")
+    )
+    updated_at: Optional[str] = field(
+        default=None, metadata=config(field_name="updatedAt")
+    )
+    host_id: Optional[str] = field(default=None, metadata=config(field_name="hostId"))
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class FacetV2:
     """FacetV2."""
 
@@ -607,15 +624,15 @@
     )
     tags: Optional[List[TagV2]] = field(
         default=None, metadata=config(field_name="tags")
     )
     endpoint_group: Optional[EndpointGroupV2] = field(
         default=None, metadata=config(field_name="endpointGroup")
     )
-    investigations: Optional[List[Investigation]] = field(
+    investigations: Optional[List[AssetInvestigation]] = field(
         default=None, metadata=config(field_name="investigations")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
 class BulkReconnectNativeAssetsInput:
```

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/audits/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/audits/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/clients/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/clients/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/collector/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/collector/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/comments/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/comments/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_command_manager/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_command_manager/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/endpoint_management_service/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/endpoint_management_service/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/entity_profile/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/entity_profile/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/event_search/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/event_search/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/events/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/events/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/exports/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/exports/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,37 @@
             },
             output=build_output_string(AddEvidenceToInvestigationResult),
         )
         if result.get(endpoint) is not None:
             return AddEvidenceToInvestigationResult.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for mutation addEvidenceToInvestigation")
 
+    def remove_evidence_from_investigation(
+        self, input_: RemoveEvidenceFromInvestigationInput
+    ) -> RemoveEvidenceFromInvestigationResult:
+        """Remove evidence from an existing investigation
+
+        This is a background job, it will be pretty quick, but removed alerts/events will likely still be present in the returned investigation
+        The processing status will reflect where the the investigation is at in the processing job.
+        """
+        endpoint = "removeEvidenceFromInvestigation"
+
+        result = self.service.execute_mutation(
+            endpoint=endpoint,
+            variables={
+                "input": prepare_input(input_),
+            },
+            output=build_output_string(RemoveEvidenceFromInvestigationResult),
+        )
+        if result.get(endpoint) is not None:
+            return RemoveEvidenceFromInvestigationResult.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError(
+            "for mutation removeEvidenceFromInvestigation"
+        )
+
     def create_investigation_rule(
         self, input_: CreateInvestigationRuleInput
     ) -> InvestigationRule:
         """Create a new investigation rule."""
         endpoint = "createInvestigationRule"
 
         result = self.service.execute_mutation(
```

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,31 @@
             },
             output=build_output_string(InvestigationV2),
         )
         if result.get(endpoint) is not None:
             return InvestigationV2.from_dict(result.get(endpoint))
         raise GraphQLNoRowsInResultSetError("for query investigationV2")
 
+    def investigations_v2(
+        self, arguments: InvestigationsV2Arguments
+    ) -> InvestigationsV2:
+        """Search investigations."""
+        endpoint = "investigationsV2"
+
+        result = self.service.execute_query(
+            endpoint=endpoint,
+            variables={
+                "arguments": prepare_input(arguments),
+            },
+            output=build_output_string(InvestigationsV2),
+        )
+        if result.get(endpoint) is not None:
+            return InvestigationsV2.from_dict(result.get(endpoint))
+        raise GraphQLNoRowsInResultSetError("for query investigationsV2")
+
     def investigation_rule(
         self, arguments: InvestigationRuleArguments
     ) -> InvestigationRule:
         """Get an auto-investigation rule."""
         endpoint = "investigationRule"
 
         result = self.service.execute_query(
```

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/investigations2/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/investigations2/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,33 @@
     events: Optional[List[str]] = field(
         default=None, metadata=config(field_name="events")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class RemoveEvidenceFromInvestigationInput:
+    """RemoveEvidenceFromInvestigationInput."""
+
+    investigation_id: Optional[str] = field(
+        default=None, metadata=config(field_name="investigationId")
+    )
+    alerts: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="alerts")
+    )
+    events: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="events")
+    )
+    assets: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="assets")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class DeleteInvestigationRuleInput:
     """DeleteInvestigationRuleInput."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
 
 
 @dataclass_json
@@ -150,14 +169,33 @@
     events: Optional[List[str]] = field(
         default=None, metadata=config(field_name="events")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class RemoveEvidenceFromInvestigationResult:
+    """RemoveEvidenceFromInvestigationResult."""
+
+    investigation_id: Optional[str] = field(
+        default=None, metadata=config(field_name="investigationId")
+    )
+    alerts: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="alerts")
+    )
+    events: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="events")
+    )
+    assets: Optional[List[str]] = field(
+        default=None, metadata=config(field_name="assets")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class CreateInvestigationTemplateInput:
     """CreateInvestigationTemplateInput."""
 
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     title: Optional[str] = field(default=None, metadata=config(field_name="title"))
     description: Optional[str] = field(
         default=None, metadata=config(field_name="description")
@@ -462,14 +500,17 @@
     )
     tenant_filter: Optional[str] = field(
         default=None, metadata=config(field_name="tenantFilter")
     )
     template_id: Optional[str] = field(
         default=None, metadata=config(field_name="templateId")
     )
+    response_data: Optional[dict] = field(
+        default=None, metadata=config(field_name="responseData")
+    )
     state: Optional[InvestigationRuleState] = field(
         default=None, metadata=config(field_name="state")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
@@ -510,21 +551,37 @@
     )
     tenant_filter: Optional[str] = field(
         default=None, metadata=config(field_name="tenantFilter")
     )
     template_id: Optional[str] = field(
         default=None, metadata=config(field_name="templateId")
     )
+    response_data: Optional[dict] = field(
+        default=None, metadata=config(field_name="responseData")
+    )
     state: Optional[InvestigationRuleState] = field(
         default=None, metadata=config(field_name="state")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class InvestigationsV2Arguments:
+    """InvestigationsV2Arguments."""
+
+    page: Optional[int] = field(default=None, metadata=config(field_name="page"))
+    per_page: Optional[int] = field(default=None, metadata=config(field_name="perPage"))
+    cql: Optional[str] = field(default=None, metadata=config(field_name="cql"))
+    order_by: Optional[PaginationOrder] = field(
+        default=None, metadata=config(field_name="orderBy")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class ExportInvestigationResourcesArgument:
     """ExportInvestigationResourcesArgument."""
 
     id: Optional[str] = field(default=None, metadata=config(field_name="id"))
     name: Optional[str] = field(default=None, metadata=config(field_name="name"))
     type: Optional[InvestigationResourceType] = field(
         default=None, metadata=config(field_name="type")
@@ -969,14 +1026,27 @@
     comments_count: Optional[InvestigationCommentsCount] = field(
         default=None, metadata=config(field_name="commentsCount")
     )
 
 
 @dataclass_json
 @dataclass(order=True, eq=True, frozen=True)
+class InvestigationsV2:
+    """InvestigationsV2."""
+
+    total_count: Optional[int] = field(
+        default=None, metadata=config(field_name="totalCount")
+    )
+    investigations: Optional[List[InvestigationV2]] = field(
+        default=None, metadata=config(field_name="investigations")
+    )
+
+
+@dataclass_json
+@dataclass(order=True, eq=True, frozen=True)
 class InvestigationTemplates:
     """InvestigationTemplates."""
 
     total_count: Optional[int] = field(
         default=None, metadata=config(field_name="totalCount")
     )
     templates: Optional[List[InvestigationTemplate]] = field(
```

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/mitre_attack_info/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/mitre_attack_info/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notebooks/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notebooks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/notifications/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/notifications/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/rules/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/rules/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/sharelinks/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/sharelinks/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/tenants/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/tenants/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/threat/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/threat/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/trip/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/trip/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/__init__.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/__init__.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/mutations.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/mutations.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/queries.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/queries.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/subscriptions.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/subscriptions.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/services/users/types.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/services/users/types.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/tokens.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/tokens.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python/utils.py` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python/utils.py`

 * *Files identical despite different names*

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/PKG-INFO` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taegis-sdk-python
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Taegis Python SDK
 Home-page: https://github.com/secureworks/taegis-sdk-python
 Author: Secureworks
 Author-email: sdks@secureworks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `taegis-sdk-python-1.0.0a8/taegis_sdk_python.egg-info/SOURCES.txt` & `taegis-sdk-python-1.0.0a9/taegis_sdk_python.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,19 @@
 taegis_sdk_python/services/collector/subscriptions.py
 taegis_sdk_python/services/collector/types.py
 taegis_sdk_python/services/comments/__init__.py
 taegis_sdk_python/services/comments/mutations.py
 taegis_sdk_python/services/comments/queries.py
 taegis_sdk_python/services/comments/subscriptions.py
 taegis_sdk_python/services/comments/types.py
+taegis_sdk_python/services/detector_registry/__init__.py
+taegis_sdk_python/services/detector_registry/mutations.py
+taegis_sdk_python/services/detector_registry/queries.py
+taegis_sdk_python/services/detector_registry/subscriptions.py
+taegis_sdk_python/services/detector_registry/types.py
 taegis_sdk_python/services/endpoint_command_manager/__init__.py
 taegis_sdk_python/services/endpoint_command_manager/mutations.py
 taegis_sdk_python/services/endpoint_command_manager/queries.py
 taegis_sdk_python/services/endpoint_command_manager/subscriptions.py
 taegis_sdk_python/services/endpoint_command_manager/types.py
 taegis_sdk_python/services/endpoint_management_service/__init__.py
 taegis_sdk_python/services/endpoint_management_service/mutations.py
@@ -116,14 +121,19 @@
 taegis_sdk_python/services/notebooks/subscriptions.py
 taegis_sdk_python/services/notebooks/types.py
 taegis_sdk_python/services/notifications/__init__.py
 taegis_sdk_python/services/notifications/mutations.py
 taegis_sdk_python/services/notifications/queries.py
 taegis_sdk_python/services/notifications/subscriptions.py
 taegis_sdk_python/services/notifications/types.py
+taegis_sdk_python/services/preferences/__init__.py
+taegis_sdk_python/services/preferences/mutations.py
+taegis_sdk_python/services/preferences/queries.py
+taegis_sdk_python/services/preferences/subscriptions.py
+taegis_sdk_python/services/preferences/types.py
 taegis_sdk_python/services/rules/__init__.py
 taegis_sdk_python/services/rules/mutations.py
 taegis_sdk_python/services/rules/queries.py
 taegis_sdk_python/services/rules/subscriptions.py
 taegis_sdk_python/services/rules/types.py
 taegis_sdk_python/services/sharelinks/__init__.py
 taegis_sdk_python/services/sharelinks/mutations.py
```

