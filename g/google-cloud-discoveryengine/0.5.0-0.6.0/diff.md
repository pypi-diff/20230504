# Comparing `tmp/google-cloud-discoveryengine-0.5.0.tar.gz` & `tmp/google-cloud-discoveryengine-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-discoveryengine-0.5.0.tar", last modified: Tue Apr 25 18:08:22 2023, max compression
+gzip compressed data, was "google-cloud-discoveryengine-0.6.0.tar", last modified: Thu May  4 17:24:58 2023, max compression
```

## Comparing `google-cloud-discoveryengine-0.5.0.tar` & `google-cloud-discoveryengine-0.6.0.tar`

### file list

```diff
@@ -1,118 +1,119 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.917395 google-cloud-discoveryengine-0.5.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4587 2023-04-25 18:08:22.917395 google-cloud-discoveryengine-0.5.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3663 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.897393 google-cloud-discoveryengine-0.5.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.897393 google-cloud-discoveryengine-0.5.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/
--rw-rw-r--   0 root         (0)     1003     5454 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003     4164 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     8894 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17110 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    26203 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6711 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13616 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13824 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22544 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.901394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    42805 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    53274 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py
--rw-rw-r--   0 root         (0)     1003     5921 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.905394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9576 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20553 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20965 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    54046 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.905394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17422 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27322 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.905394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6712 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13617 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13829 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22701 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.905394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    38222 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48529 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
--rw-rw-r--   0 root         (0)     1003     5829 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8553 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18711 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19114 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    48576 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17633 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28264 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py
--rw-rw-r--   0 root         (0)     1003     5757 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6603 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13401 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13619 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22431 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27473 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37338 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.909394 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8165 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17230 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17568 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    40240 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     2995 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5269 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/common.py
--rw-rw-r--   0 root         (0)     1003     4646 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/completion_service.py
--rw-rw-r--   0 root         (0)     1003     6373 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/document.py
--rw-rw-r--   0 root         (0)     1003     9481 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/document_service.py
--rw-rw-r--   0 root         (0)     1003    18586 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/import_config.py
--rw-rw-r--   0 root         (0)     1003    10788 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
--rw-rw-r--   0 root         (0)     1003     2396 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/schema.py
--rw-rw-r--   0 root         (0)     1003     9031 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/schema_service.py
--rw-rw-r--   0 root         (0)     1003    35635 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/search_service.py
--rw-rw-r--   0 root         (0)     1003    27269 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/user_event.py
--rw-rw-r--   0 root         (0)     1003     3436 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/
--rw-r--r--   0 root         (0)     1003     4587 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     6123 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-25 18:08:22.000000 google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-04-25 18:08:22.917395 google-cloud-discoveryengine-0.5.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2956 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.913395 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-25 18:08:22.917395 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    83584 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
--rw-rw-r--   0 root         (0)     1003   188394 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
--rw-rw-r--   0 root         (0)     1003    86195 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
--rw-rw-r--   0 root         (0)     1003   168594 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
--rw-rw-r--   0 root         (0)     1003    93887 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
--rw-rw-r--   0 root         (0)     1003   119713 2023-04-25 18:05:53.000000 google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.482420 google-cloud-discoveryengine-0.6.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4587 2023-05-04 17:24:58.482420 google-cloud-discoveryengine-0.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3663 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.462418 google-cloud-discoveryengine-0.6.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.462418 google-cloud-discoveryengine-0.6.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.462418 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/
+-rw-rw-r--   0 root         (0)     1003     5697 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003     4372 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9266 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17110 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26203 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6711 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13616 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13824 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22544 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.466419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47829 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58424 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5921 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10042 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23048 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    59724 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17422 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27322 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6712 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13617 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13829 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22701 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38222 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48529 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5829 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.470419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8553 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18711 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19114 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    48576 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.474419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17633 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28264 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5757 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.474419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6603 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13401 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13619 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22431 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.474419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27473 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37338 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.474419 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8165 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17230 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17568 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    40240 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     3197 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5368 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4646 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/completion_service.py
+-rw-rw-r--   0 root         (0)     1003     6373 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/document.py
+-rw-rw-r--   0 root         (0)     1003     9481 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/document_service.py
+-rw-rw-r--   0 root         (0)     1003    18586 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/import_config.py
+-rw-rw-r--   0 root         (0)     1003     4085 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/purge_config.py
+-rw-rw-r--   0 root         (0)     1003    10788 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003     2396 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     9031 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/schema_service.py
+-rw-rw-r--   0 root         (0)     1003    35635 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/search_service.py
+-rw-rw-r--   0 root         (0)     1003    27718 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/user_event.py
+-rw-rw-r--   0 root         (0)     1003     3436 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/
+-rw-r--r--   0 root         (0)     1003     4587 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     6181 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-04 17:24:58.000000 google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-05-04 17:24:58.482420 google-cloud-discoveryengine-0.6.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.478420 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:24:58.482420 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83584 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py
+-rw-rw-r--   0 root         (0)     1003   201685 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py
+-rw-rw-r--   0 root         (0)     1003    86195 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py
+-rw-rw-r--   0 root         (0)     1003   168594 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py
+-rw-rw-r--   0 root         (0)     1003    93887 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py
+-rw-rw-r--   0 root         (0)     1003   119713 2023-05-04 17:22:05.000000 google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py
```

### Comparing `google-cloud-discoveryengine-0.5.0/LICENSE` & `google-cloud-discoveryengine-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/MANIFEST.in` & `google-cloud-discoveryengine-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/PKG-INFO` & `google-cloud-discoveryengine-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.5.0
+Version: 0.6.0
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.5.0/README.rst` & `google-cloud-discoveryengine-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,14 +79,19 @@
     ImportDocumentsRequest,
     ImportDocumentsResponse,
     ImportErrorConfig,
     ImportUserEventsMetadata,
     ImportUserEventsRequest,
     ImportUserEventsResponse,
 )
+from google.cloud.discoveryengine_v1beta.types.purge_config import (
+    PurgeDocumentsMetadata,
+    PurgeDocumentsRequest,
+    PurgeDocumentsResponse,
+)
 from google.cloud.discoveryengine_v1beta.types.recommendation_service import (
     RecommendRequest,
     RecommendResponse,
 )
 from google.cloud.discoveryengine_v1beta.types.schema import Schema
 from google.cloud.discoveryengine_v1beta.types.schema_service import (
     CreateSchemaMetadata,
@@ -148,14 +153,17 @@
     "ImportDocumentsMetadata",
     "ImportDocumentsRequest",
     "ImportDocumentsResponse",
     "ImportErrorConfig",
     "ImportUserEventsMetadata",
     "ImportUserEventsRequest",
     "ImportUserEventsResponse",
+    "PurgeDocumentsMetadata",
+    "PurgeDocumentsRequest",
+    "PurgeDocumentsResponse",
     "RecommendRequest",
     "RecommendResponse",
     "Schema",
     "CreateSchemaMetadata",
     "CreateSchemaRequest",
     "DeleteSchemaMetadata",
     "DeleteSchemaRequest",
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine/gapic_version.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.5.0"  # {x-release-please-version}
+__version__ = "0.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,19 @@
     ImportDocumentsRequest,
     ImportDocumentsResponse,
     ImportErrorConfig,
     ImportUserEventsMetadata,
     ImportUserEventsRequest,
     ImportUserEventsResponse,
 )
+from .types.purge_config import (
+    PurgeDocumentsMetadata,
+    PurgeDocumentsRequest,
+    PurgeDocumentsResponse,
+)
 from .types.recommendation_service import RecommendRequest, RecommendResponse
 from .types.schema import Schema
 from .types.schema_service import (
     CreateSchemaMetadata,
     CreateSchemaRequest,
     DeleteSchemaMetadata,
     DeleteSchemaRequest,
@@ -118,14 +123,17 @@
     "ListDocumentsRequest",
     "ListDocumentsResponse",
     "ListSchemasRequest",
     "ListSchemasResponse",
     "MediaInfo",
     "PageInfo",
     "PanelInfo",
+    "PurgeDocumentsMetadata",
+    "PurgeDocumentsRequest",
+    "PurgeDocumentsResponse",
     "RecommendRequest",
     "RecommendResponse",
     "RecommendationServiceClient",
     "Schema",
     "SchemaServiceClient",
     "SearchInfo",
     "SearchRequest",
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/gapic_metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999937996031746%*

 * *Differences: {"'services'": "{'DocumentService': {'clients': {'grpc': {'rpcs': {'PurgeDocuments': "*

 * *               "OrderedDict([('methods', ['purge_documents'])])}}, 'grpc-async': {'rpcs': "*

 * *               "{'PurgeDocuments': OrderedDict([('methods', ['purge_documents'])])}}, 'rest': "*

 * *               "{'rpcs': {'PurgeDocuments': OrderedDict([('methods', ['purge_documents'])])}}}}}"}*

```diff
@@ -65,14 +65,19 @@
                             ]
                         },
                         "ListDocuments": {
                             "methods": [
                                 "list_documents"
                             ]
                         },
+                        "PurgeDocuments": {
+                            "methods": [
+                                "purge_documents"
+                            ]
+                        },
                         "UpdateDocument": {
                             "methods": [
                                 "update_document"
                             ]
                         }
                     }
                 },
@@ -100,14 +105,19 @@
                             ]
                         },
                         "ListDocuments": {
                             "methods": [
                                 "list_documents"
                             ]
                         },
+                        "PurgeDocuments": {
+                            "methods": [
+                                "purge_documents"
+                            ]
+                        },
                         "UpdateDocument": {
                             "methods": [
                                 "update_document"
                             ]
                         }
                     }
                 },
@@ -135,14 +145,19 @@
                             ]
                         },
                         "ListDocuments": {
                             "methods": [
                                 "list_documents"
                             ]
                         },
+                        "PurgeDocuments": {
+                            "methods": [
+                                "purge_documents"
+                            ]
+                        },
                         "UpdateDocument": {
                             "methods": [
                                 "update_document"
                             ]
                         }
                     }
                 }
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/gapic_version.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.5.0"  # {x-release-please-version}
+__version__ = "0.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/completion_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,19 @@
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.longrunning import operations_pb2
 from google.protobuf import struct_pb2  # type: ignore
 
 from google.cloud.discoveryengine_v1beta.services.document_service import pagers
-from google.cloud.discoveryengine_v1beta.types import document_service, import_config
+from google.cloud.discoveryengine_v1beta.types import (
+    document_service,
+    import_config,
+    purge_config,
+)
 from google.cloud.discoveryengine_v1beta.types import document
 from google.cloud.discoveryengine_v1beta.types import document as gcd_document
 
 from .client import DocumentServiceClient
 from .transports.base import DEFAULT_CLIENT_INFO, DocumentServiceTransport
 from .transports.grpc_asyncio import DocumentServiceGrpcAsyncIOTransport
 
@@ -908,14 +912,131 @@
             import_config.ImportDocumentsResponse,
             metadata_type=import_config.ImportDocumentsMetadata,
         )
 
         # Done; return the response.
         return response
 
+    async def purge_documents(
+        self,
+        request: Optional[Union[purge_config.PurgeDocumentsRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation_async.AsyncOperation:
+        r"""Permanently deletes all selected
+        [Document][google.cloud.discoveryengine.v1beta.Document]s in a
+        branch.
+
+        This process is asynchronous. Depending on the number of
+        [Document][google.cloud.discoveryengine.v1beta.Document]s to be
+        deleted, this operation can take hours to complete. Before the
+        delete operation completes, some
+        [Document][google.cloud.discoveryengine.v1beta.Document]s might
+        still be returned by
+        [DocumentService.GetDocument][google.cloud.discoveryengine.v1beta.DocumentService.GetDocument]
+        or
+        [DocumentService.ListDocuments][google.cloud.discoveryengine.v1beta.DocumentService.ListDocuments].
+
+        To get a list of the
+        [Document][google.cloud.discoveryengine.v1beta.Document]s to be
+        deleted, set
+        [PurgeDocumentsRequest.force][google.cloud.discoveryengine.v1beta.PurgeDocumentsRequest.force]
+        to false.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import discoveryengine_v1beta
+
+            async def sample_purge_documents():
+                # Create a client
+                client = discoveryengine_v1beta.DocumentServiceAsyncClient()
+
+                # Initialize request argument(s)
+                request = discoveryengine_v1beta.PurgeDocumentsRequest(
+                    parent="parent_value",
+                    filter="filter_value",
+                )
+
+                # Make the request
+                operation = client.purge_documents(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = (await operation).result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.discoveryengine_v1beta.types.PurgeDocumentsRequest, dict]]):
+                The request object. Request message for
+                [DocumentService.PurgeDocuments][google.cloud.discoveryengine.v1beta.DocumentService.PurgeDocuments]
+                method.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation_async.AsyncOperation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.cloud.discoveryengine_v1beta.types.PurgeDocumentsResponse` Response message for
+                   [DocumentService.PurgeDocuments][google.cloud.discoveryengine.v1beta.DocumentService.PurgeDocuments]
+                   method. If the long running operation is successfully
+                   done, then this message is returned by the
+                   google.longrunning.Operations.response field.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = purge_config.PurgeDocumentsRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.purge_documents,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation_async.from_gapic(
+            response,
+            self._client._transport.operations_client,
+            purge_config.PurgeDocumentsResponse,
+            metadata_type=purge_config.PurgeDocumentsMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def list_operations(
         self,
         request: Optional[operations_pb2.ListOperationsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,19 @@
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.longrunning import operations_pb2
 from google.protobuf import struct_pb2  # type: ignore
 
 from google.cloud.discoveryengine_v1beta.services.document_service import pagers
-from google.cloud.discoveryengine_v1beta.types import document_service, import_config
+from google.cloud.discoveryengine_v1beta.types import (
+    document_service,
+    import_config,
+    purge_config,
+)
 from google.cloud.discoveryengine_v1beta.types import document
 from google.cloud.discoveryengine_v1beta.types import document as gcd_document
 
 from .transports.base import DEFAULT_CLIENT_INFO, DocumentServiceTransport
 from .transports.grpc import DocumentServiceGrpcTransport
 from .transports.grpc_asyncio import DocumentServiceGrpcAsyncIOTransport
 from .transports.rest import DocumentServiceRestTransport
@@ -1156,14 +1160,132 @@
             import_config.ImportDocumentsResponse,
             metadata_type=import_config.ImportDocumentsMetadata,
         )
 
         # Done; return the response.
         return response
 
+    def purge_documents(
+        self,
+        request: Optional[Union[purge_config.PurgeDocumentsRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""Permanently deletes all selected
+        [Document][google.cloud.discoveryengine.v1beta.Document]s in a
+        branch.
+
+        This process is asynchronous. Depending on the number of
+        [Document][google.cloud.discoveryengine.v1beta.Document]s to be
+        deleted, this operation can take hours to complete. Before the
+        delete operation completes, some
+        [Document][google.cloud.discoveryengine.v1beta.Document]s might
+        still be returned by
+        [DocumentService.GetDocument][google.cloud.discoveryengine.v1beta.DocumentService.GetDocument]
+        or
+        [DocumentService.ListDocuments][google.cloud.discoveryengine.v1beta.DocumentService.ListDocuments].
+
+        To get a list of the
+        [Document][google.cloud.discoveryengine.v1beta.Document]s to be
+        deleted, set
+        [PurgeDocumentsRequest.force][google.cloud.discoveryengine.v1beta.PurgeDocumentsRequest.force]
+        to false.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import discoveryengine_v1beta
+
+            def sample_purge_documents():
+                # Create a client
+                client = discoveryengine_v1beta.DocumentServiceClient()
+
+                # Initialize request argument(s)
+                request = discoveryengine_v1beta.PurgeDocumentsRequest(
+                    parent="parent_value",
+                    filter="filter_value",
+                )
+
+                # Make the request
+                operation = client.purge_documents(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.discoveryengine_v1beta.types.PurgeDocumentsRequest, dict]):
+                The request object. Request message for
+                [DocumentService.PurgeDocuments][google.cloud.discoveryengine.v1beta.DocumentService.PurgeDocuments]
+                method.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.cloud.discoveryengine_v1beta.types.PurgeDocumentsResponse` Response message for
+                   [DocumentService.PurgeDocuments][google.cloud.discoveryengine.v1beta.DocumentService.PurgeDocuments]
+                   method. If the long running operation is successfully
+                   done, then this message is returned by the
+                   google.longrunning.Operations.response field.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a purge_config.PurgeDocumentsRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, purge_config.PurgeDocumentsRequest):
+            request = purge_config.PurgeDocumentsRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.purge_documents]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            purge_config.PurgeDocumentsResponse,
+            metadata_type=purge_config.PurgeDocumentsMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def __enter__(self) -> "DocumentServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,19 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
 from google.cloud.discoveryengine_v1beta import gapic_version as package_version
-from google.cloud.discoveryengine_v1beta.types import document_service, import_config
+from google.cloud.discoveryengine_v1beta.types import (
+    document_service,
+    import_config,
+    purge_config,
+)
 from google.cloud.discoveryengine_v1beta.types import document
 from google.cloud.discoveryengine_v1beta.types import document as gcd_document
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
@@ -161,14 +165,19 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=300.0,
                 ),
                 default_timeout=300.0,
                 client_info=client_info,
             ),
+            self.purge_documents: gapic_v1.method.wrap_method(
+                self.purge_documents,
+                default_timeout=None,
+                client_info=client_info,
+            ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
         .. warning::
              Only call this method if the transport is NOT shared
@@ -235,14 +244,23 @@
     ) -> Callable[
         [import_config.ImportDocumentsRequest],
         Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
     ]:
         raise NotImplementedError()
 
     @property
+    def purge_documents(
+        self,
+    ) -> Callable[
+        [purge_config.PurgeDocumentsRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def list_operations(
         self,
     ) -> Callable[
         [operations_pb2.ListOperationsRequest],
         Union[
             operations_pb2.ListOperationsResponse,
             Awaitable[operations_pb2.ListOperationsResponse],
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,57 +9,106 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers, operations_v1
-import google.auth  # type: ignore
+from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
+from grpc.experimental import aio  # type: ignore
 
-from google.cloud.discoveryengine_v1beta.types import document_service, import_config
+from google.cloud.discoveryengine_v1beta.types import (
+    document_service,
+    import_config,
+    purge_config,
+)
 from google.cloud.discoveryengine_v1beta.types import document
 from google.cloud.discoveryengine_v1beta.types import document as gcd_document
 
 from .base import DEFAULT_CLIENT_INFO, DocumentServiceTransport
+from .grpc import DocumentServiceGrpcTransport
 
 
-class DocumentServiceGrpcTransport(DocumentServiceTransport):
-    """gRPC backend transport for DocumentService.
+class DocumentServiceGrpcAsyncIOTransport(DocumentServiceTransport):
+    """gRPC AsyncIO backend transport for DocumentService.
 
     Service for ingesting
     [Document][google.cloud.discoveryengine.v1beta.Document] information
     of the customer's website.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _stubs: Dict[str, Callable]
+    _grpc_channel: aio.Channel
+    _stubs: Dict[str, Callable] = {}
+
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "discoveryengine.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> aio.Channel:
+        """Create and return a gRPC AsyncIO channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            aio.Channel: A gRPC AsyncIO channel object.
+        """
+
+        return grpc_helpers_async.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
 
     def __init__(
         self,
         *,
         host: str = "discoveryengine.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[aio.Channel] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -75,17 +124,18 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            channel (Optional[aio.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -104,36 +154,35 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
+            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
-        self._operations_client: Optional[operations_v1.OperationsClient] = None
+        self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
-
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -179,91 +228,51 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "discoveryengine.googleapis.com",
-        credentials: Optional[ga_credentials.Credentials] = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> grpc.Channel:
-        """Create and return a gRPC channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is mutually exclusive with credentials.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            grpc.Channel: A gRPC channel object.
+    @property
+    def grpc_channel(self) -> aio.Channel:
+        """Create the channel designed to connect to this service.
 
-        Raises:
-            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
-              and ``credentials_file`` are passed.
+        This property caches on the instance; repeated calls return
+        the same channel.
         """
-
-        return grpc_helpers.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
-
-    @property
-    def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service."""
+        # Return the channel from cache.
         return self._grpc_channel
 
     @property
-    def operations_client(self) -> operations_v1.OperationsClient:
+    def operations_client(self) -> operations_v1.OperationsAsyncClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
         # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
-            self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
+            self._operations_client = operations_v1.OperationsAsyncClient(
+                self.grpc_channel
+            )
 
         # Return the client from cache.
         return self._operations_client
 
     @property
     def get_document(
         self,
-    ) -> Callable[[document_service.GetDocumentRequest], document.Document]:
+    ) -> Callable[[document_service.GetDocumentRequest], Awaitable[document.Document]]:
         r"""Return a callable for the get document method over gRPC.
 
         Gets a [Document][google.cloud.discoveryengine.v1beta.Document].
 
         Returns:
             Callable[[~.GetDocumentRequest],
-                    ~.Document]:
+                    Awaitable[~.Document]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -275,24 +284,25 @@
             )
         return self._stubs["get_document"]
 
     @property
     def list_documents(
         self,
     ) -> Callable[
-        [document_service.ListDocumentsRequest], document_service.ListDocumentsResponse
+        [document_service.ListDocumentsRequest],
+        Awaitable[document_service.ListDocumentsResponse],
     ]:
         r"""Return a callable for the list documents method over gRPC.
 
         Gets a list of
         [Document][google.cloud.discoveryengine.v1beta.Document]s.
 
         Returns:
             Callable[[~.ListDocumentsRequest],
-                    ~.ListDocumentsResponse]:
+                    Awaitable[~.ListDocumentsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -303,23 +313,25 @@
                 response_deserializer=document_service.ListDocumentsResponse.deserialize,
             )
         return self._stubs["list_documents"]
 
     @property
     def create_document(
         self,
-    ) -> Callable[[document_service.CreateDocumentRequest], gcd_document.Document]:
+    ) -> Callable[
+        [document_service.CreateDocumentRequest], Awaitable[gcd_document.Document]
+    ]:
         r"""Return a callable for the create document method over gRPC.
 
         Creates a
         [Document][google.cloud.discoveryengine.v1beta.Document].
 
         Returns:
             Callable[[~.CreateDocumentRequest],
-                    ~.Document]:
+                    Awaitable[~.Document]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -330,23 +342,25 @@
                 response_deserializer=gcd_document.Document.deserialize,
             )
         return self._stubs["create_document"]
 
     @property
     def update_document(
         self,
-    ) -> Callable[[document_service.UpdateDocumentRequest], document.Document]:
+    ) -> Callable[
+        [document_service.UpdateDocumentRequest], Awaitable[document.Document]
+    ]:
         r"""Return a callable for the update document method over gRPC.
 
         Updates a
         [Document][google.cloud.discoveryengine.v1beta.Document].
 
         Returns:
             Callable[[~.UpdateDocumentRequest],
-                    ~.Document]:
+                    Awaitable[~.Document]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -357,23 +371,23 @@
                 response_deserializer=document.Document.deserialize,
             )
         return self._stubs["update_document"]
 
     @property
     def delete_document(
         self,
-    ) -> Callable[[document_service.DeleteDocumentRequest], empty_pb2.Empty]:
+    ) -> Callable[[document_service.DeleteDocumentRequest], Awaitable[empty_pb2.Empty]]:
         r"""Return a callable for the delete document method over gRPC.
 
         Deletes a
         [Document][google.cloud.discoveryengine.v1beta.Document].
 
         Returns:
             Callable[[~.DeleteDocumentRequest],
-                    ~.Empty]:
+                    Awaitable[~.Empty]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -384,29 +398,31 @@
                 response_deserializer=empty_pb2.Empty.FromString,
             )
         return self._stubs["delete_document"]
 
     @property
     def import_documents(
         self,
-    ) -> Callable[[import_config.ImportDocumentsRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [import_config.ImportDocumentsRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the import documents method over gRPC.
 
         Bulk import of multiple
         [Document][google.cloud.discoveryengine.v1beta.Document]s.
         Request processing may be synchronous. Non-existing items will
         be created.
 
         Note: It is possible for a subset of the
         [Document][google.cloud.discoveryengine.v1beta.Document]s to be
         successfully updated.
 
         Returns:
             Callable[[~.ImportDocumentsRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -414,16 +430,62 @@
             self._stubs["import_documents"] = self.grpc_channel.unary_unary(
                 "/google.cloud.discoveryengine.v1beta.DocumentService/ImportDocuments",
                 request_serializer=import_config.ImportDocumentsRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["import_documents"]
 
+    @property
+    def purge_documents(
+        self,
+    ) -> Callable[
+        [purge_config.PurgeDocumentsRequest], Awaitable[operations_pb2.Operation]
+    ]:
+        r"""Return a callable for the purge documents method over gRPC.
+
+        Permanently deletes all selected
+        [Document][google.cloud.discoveryengine.v1beta.Document]s in a
+        branch.
+
+        This process is asynchronous. Depending on the number of
+        [Document][google.cloud.discoveryengine.v1beta.Document]s to be
+        deleted, this operation can take hours to complete. Before the
+        delete operation completes, some
+        [Document][google.cloud.discoveryengine.v1beta.Document]s might
+        still be returned by
+        [DocumentService.GetDocument][google.cloud.discoveryengine.v1beta.DocumentService.GetDocument]
+        or
+        [DocumentService.ListDocuments][google.cloud.discoveryengine.v1beta.DocumentService.ListDocuments].
+
+        To get a list of the
+        [Document][google.cloud.discoveryengine.v1beta.Document]s to be
+        deleted, set
+        [PurgeDocumentsRequest.force][google.cloud.discoveryengine.v1beta.PurgeDocumentsRequest.force]
+        to false.
+
+        Returns:
+            Callable[[~.PurgeDocumentsRequest],
+                    Awaitable[~.Operation]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "purge_documents" not in self._stubs:
+            self._stubs["purge_documents"] = self.grpc_channel.unary_unary(
+                "/google.cloud.discoveryengine.v1beta.DocumentService/PurgeDocuments",
+                request_serializer=purge_config.PurgeDocumentsRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["purge_documents"]
+
     def close(self):
-        self.grpc_channel.close()
+        return self.grpc_channel.close()
 
     @property
     def get_operation(
         self,
     ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
         r"""Return a callable for the get_operation method over gRPC."""
         # Generate a "stub function" on-the-fly which will actually make
@@ -453,13 +515,9 @@
             self._stubs["list_operations"] = self.grpc_channel.unary_unary(
                 "/google.longrunning.Operations/ListOperations",
                 request_serializer=operations_pb2.ListOperationsRequest.SerializeToString,
                 response_deserializer=operations_pb2.ListOperationsResponse.FromString,
             )
         return self._stubs["list_operations"]
 
-    @property
-    def kind(self) -> str:
-        return "grpc"
-
 
-__all__ = ("DocumentServiceGrpcTransport",)
+__all__ = ("DocumentServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,102 +9,61 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
+from google.api_core import gapic_v1, grpc_helpers, operations_v1
+import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
-from grpc.experimental import aio  # type: ignore
 
-from google.cloud.discoveryengine_v1beta.types import document_service, import_config
+from google.cloud.discoveryengine_v1beta.types import (
+    document_service,
+    import_config,
+    purge_config,
+)
 from google.cloud.discoveryengine_v1beta.types import document
 from google.cloud.discoveryengine_v1beta.types import document as gcd_document
 
 from .base import DEFAULT_CLIENT_INFO, DocumentServiceTransport
-from .grpc import DocumentServiceGrpcTransport
 
 
-class DocumentServiceGrpcAsyncIOTransport(DocumentServiceTransport):
-    """gRPC AsyncIO backend transport for DocumentService.
+class DocumentServiceGrpcTransport(DocumentServiceTransport):
+    """gRPC backend transport for DocumentService.
 
     Service for ingesting
     [Document][google.cloud.discoveryengine.v1beta.Document] information
     of the customer's website.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _grpc_channel: aio.Channel
-    _stubs: Dict[str, Callable] = {}
-
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "discoveryengine.googleapis.com",
-        credentials: Optional[ga_credentials.Credentials] = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> aio.Channel:
-        """Create and return a gRPC AsyncIO channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            aio.Channel: A gRPC AsyncIO channel object.
-        """
-
-        return grpc_helpers_async.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
+    _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "discoveryengine.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[grpc.Channel] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -120,18 +79,17 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            channel (Optional[grpc.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -150,35 +108,36 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
+          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
-        self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
+        self._operations_client: Optional[operations_v1.OperationsClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
+
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -224,51 +183,91 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @property
-    def grpc_channel(self) -> aio.Channel:
-        """Create the channel designed to connect to this service.
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "discoveryengine.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> grpc.Channel:
+        """Create and return a gRPC channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is mutually exclusive with credentials.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            grpc.Channel: A gRPC channel object.
 
-        This property caches on the instance; repeated calls return
-        the same channel.
+        Raises:
+            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
+              and ``credentials_file`` are passed.
         """
-        # Return the channel from cache.
+
+        return grpc_helpers.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
+
+    @property
+    def grpc_channel(self) -> grpc.Channel:
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
-    def operations_client(self) -> operations_v1.OperationsAsyncClient:
+    def operations_client(self) -> operations_v1.OperationsClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
         # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
-            self._operations_client = operations_v1.OperationsAsyncClient(
-                self.grpc_channel
-            )
+            self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
 
         # Return the client from cache.
         return self._operations_client
 
     @property
     def get_document(
         self,
-    ) -> Callable[[document_service.GetDocumentRequest], Awaitable[document.Document]]:
+    ) -> Callable[[document_service.GetDocumentRequest], document.Document]:
         r"""Return a callable for the get document method over gRPC.
 
         Gets a [Document][google.cloud.discoveryengine.v1beta.Document].
 
         Returns:
             Callable[[~.GetDocumentRequest],
-                    Awaitable[~.Document]]:
+                    ~.Document]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -280,25 +279,24 @@
             )
         return self._stubs["get_document"]
 
     @property
     def list_documents(
         self,
     ) -> Callable[
-        [document_service.ListDocumentsRequest],
-        Awaitable[document_service.ListDocumentsResponse],
+        [document_service.ListDocumentsRequest], document_service.ListDocumentsResponse
     ]:
         r"""Return a callable for the list documents method over gRPC.
 
         Gets a list of
         [Document][google.cloud.discoveryengine.v1beta.Document]s.
 
         Returns:
             Callable[[~.ListDocumentsRequest],
-                    Awaitable[~.ListDocumentsResponse]]:
+                    ~.ListDocumentsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -309,25 +307,23 @@
                 response_deserializer=document_service.ListDocumentsResponse.deserialize,
             )
         return self._stubs["list_documents"]
 
     @property
     def create_document(
         self,
-    ) -> Callable[
-        [document_service.CreateDocumentRequest], Awaitable[gcd_document.Document]
-    ]:
+    ) -> Callable[[document_service.CreateDocumentRequest], gcd_document.Document]:
         r"""Return a callable for the create document method over gRPC.
 
         Creates a
         [Document][google.cloud.discoveryengine.v1beta.Document].
 
         Returns:
             Callable[[~.CreateDocumentRequest],
-                    Awaitable[~.Document]]:
+                    ~.Document]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -338,25 +334,23 @@
                 response_deserializer=gcd_document.Document.deserialize,
             )
         return self._stubs["create_document"]
 
     @property
     def update_document(
         self,
-    ) -> Callable[
-        [document_service.UpdateDocumentRequest], Awaitable[document.Document]
-    ]:
+    ) -> Callable[[document_service.UpdateDocumentRequest], document.Document]:
         r"""Return a callable for the update document method over gRPC.
 
         Updates a
         [Document][google.cloud.discoveryengine.v1beta.Document].
 
         Returns:
             Callable[[~.UpdateDocumentRequest],
-                    Awaitable[~.Document]]:
+                    ~.Document]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -367,23 +361,23 @@
                 response_deserializer=document.Document.deserialize,
             )
         return self._stubs["update_document"]
 
     @property
     def delete_document(
         self,
-    ) -> Callable[[document_service.DeleteDocumentRequest], Awaitable[empty_pb2.Empty]]:
+    ) -> Callable[[document_service.DeleteDocumentRequest], empty_pb2.Empty]:
         r"""Return a callable for the delete document method over gRPC.
 
         Deletes a
         [Document][google.cloud.discoveryengine.v1beta.Document].
 
         Returns:
             Callable[[~.DeleteDocumentRequest],
-                    Awaitable[~.Empty]]:
+                    ~.Empty]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -394,31 +388,29 @@
                 response_deserializer=empty_pb2.Empty.FromString,
             )
         return self._stubs["delete_document"]
 
     @property
     def import_documents(
         self,
-    ) -> Callable[
-        [import_config.ImportDocumentsRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[import_config.ImportDocumentsRequest], operations_pb2.Operation]:
         r"""Return a callable for the import documents method over gRPC.
 
         Bulk import of multiple
         [Document][google.cloud.discoveryengine.v1beta.Document]s.
         Request processing may be synchronous. Non-existing items will
         be created.
 
         Note: It is possible for a subset of the
         [Document][google.cloud.discoveryengine.v1beta.Document]s to be
         successfully updated.
 
         Returns:
             Callable[[~.ImportDocumentsRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -426,16 +418,60 @@
             self._stubs["import_documents"] = self.grpc_channel.unary_unary(
                 "/google.cloud.discoveryengine.v1beta.DocumentService/ImportDocuments",
                 request_serializer=import_config.ImportDocumentsRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["import_documents"]
 
+    @property
+    def purge_documents(
+        self,
+    ) -> Callable[[purge_config.PurgeDocumentsRequest], operations_pb2.Operation]:
+        r"""Return a callable for the purge documents method over gRPC.
+
+        Permanently deletes all selected
+        [Document][google.cloud.discoveryengine.v1beta.Document]s in a
+        branch.
+
+        This process is asynchronous. Depending on the number of
+        [Document][google.cloud.discoveryengine.v1beta.Document]s to be
+        deleted, this operation can take hours to complete. Before the
+        delete operation completes, some
+        [Document][google.cloud.discoveryengine.v1beta.Document]s might
+        still be returned by
+        [DocumentService.GetDocument][google.cloud.discoveryengine.v1beta.DocumentService.GetDocument]
+        or
+        [DocumentService.ListDocuments][google.cloud.discoveryengine.v1beta.DocumentService.ListDocuments].
+
+        To get a list of the
+        [Document][google.cloud.discoveryengine.v1beta.Document]s to be
+        deleted, set
+        [PurgeDocumentsRequest.force][google.cloud.discoveryengine.v1beta.PurgeDocumentsRequest.force]
+        to false.
+
+        Returns:
+            Callable[[~.PurgeDocumentsRequest],
+                    ~.Operation]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "purge_documents" not in self._stubs:
+            self._stubs["purge_documents"] = self.grpc_channel.unary_unary(
+                "/google.cloud.discoveryengine.v1beta.DocumentService/PurgeDocuments",
+                request_serializer=purge_config.PurgeDocumentsRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["purge_documents"]
+
     def close(self):
-        return self.grpc_channel.close()
+        self.grpc_channel.close()
 
     @property
     def get_operation(
         self,
     ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
         r"""Return a callable for the get_operation method over gRPC."""
         # Generate a "stub function" on-the-fly which will actually make
@@ -465,9 +501,13 @@
             self._stubs["list_operations"] = self.grpc_channel.unary_unary(
                 "/google.longrunning.Operations/ListOperations",
                 request_serializer=operations_pb2.ListOperationsRequest.SerializeToString,
                 response_deserializer=operations_pb2.ListOperationsResponse.FromString,
             )
         return self._stubs["list_operations"]
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
-__all__ = ("DocumentServiceGrpcAsyncIOTransport",)
+__all__ = ("DocumentServiceGrpcTransport",)
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/document_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,19 @@
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 
 from google.longrunning import operations_pb2  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 
-from google.cloud.discoveryengine_v1beta.types import document_service, import_config
+from google.cloud.discoveryengine_v1beta.types import (
+    document_service,
+    import_config,
+    purge_config,
+)
 from google.cloud.discoveryengine_v1beta.types import document
 from google.cloud.discoveryengine_v1beta.types import document as gcd_document
 
 from .base import DEFAULT_CLIENT_INFO as BASE_DEFAULT_CLIENT_INFO
 from .base import DocumentServiceTransport
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
@@ -107,14 +111,22 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_list_documents(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_purge_documents(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_purge_documents(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_update_document(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_update_document(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -223,14 +235,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the DocumentService server but before
         it is returned to user code.
         """
         return response
 
+    def pre_purge_documents(
+        self,
+        request: purge_config.PurgeDocumentsRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[purge_config.PurgeDocumentsRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for purge_documents
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the DocumentService server.
+        """
+        return request, metadata
+
+    def post_purge_documents(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for purge_documents
+
+        Override in a subclass to manipulate the response
+        after it is returned by the DocumentService server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_update_document(
         self,
         request: document_service.UpdateDocumentRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[document_service.UpdateDocumentRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for update_document
 
@@ -974,14 +1009,117 @@
             resp = document_service.ListDocumentsResponse()
             pb_resp = document_service.ListDocumentsResponse.pb(resp)
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_list_documents(resp)
             return resp
 
+    class _PurgeDocuments(DocumentServiceRestStub):
+        def __hash__(self):
+            return hash("PurgeDocuments")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: purge_config.PurgeDocumentsRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+            r"""Call the purge documents method over HTTP.
+
+            Args:
+                request (~.purge_config.PurgeDocumentsRequest):
+                    The request object. Request message for
+                [DocumentService.PurgeDocuments][google.cloud.discoveryengine.v1beta.DocumentService.PurgeDocuments]
+                method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.operations_pb2.Operation:
+                    This resource represents a
+                long-running operation that is the
+                result of a network API call.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1beta/{parent=projects/*/locations/*/dataStores/*/branches/*}/documents:purge",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1beta/{parent=projects/*/locations/*/collections/*/dataStores/*/branches/*}/documents:purge",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_purge_documents(request, metadata)
+            pb_request = purge_config.PurgeDocumentsRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = operations_pb2.Operation()
+            json_format.Parse(response.content, resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_purge_documents(resp)
+            return resp
+
     class _UpdateDocument(DocumentServiceRestStub):
         def __hash__(self):
             return hash("UpdateDocument")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -1122,14 +1260,22 @@
         [document_service.ListDocumentsRequest], document_service.ListDocumentsResponse
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._ListDocuments(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def purge_documents(
+        self,
+    ) -> Callable[[purge_config.PurgeDocumentsRequest], operations_pb2.Operation]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._PurgeDocuments(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def update_document(
         self,
     ) -> Callable[[document_service.UpdateDocumentRequest], document.Document]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._UpdateDocument(self._session, self._host, self._interceptor)  # type: ignore
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/recommendation_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/schema_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/search_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/__init__.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,19 @@
     ImportDocumentsRequest,
     ImportDocumentsResponse,
     ImportErrorConfig,
     ImportUserEventsMetadata,
     ImportUserEventsRequest,
     ImportUserEventsResponse,
 )
+from .purge_config import (
+    PurgeDocumentsMetadata,
+    PurgeDocumentsRequest,
+    PurgeDocumentsResponse,
+)
 from .recommendation_service import RecommendRequest, RecommendResponse
 from .schema import Schema
 from .schema_service import (
     CreateSchemaMetadata,
     CreateSchemaRequest,
     DeleteSchemaMetadata,
     DeleteSchemaRequest,
@@ -79,14 +84,17 @@
     "ImportDocumentsMetadata",
     "ImportDocumentsRequest",
     "ImportDocumentsResponse",
     "ImportErrorConfig",
     "ImportUserEventsMetadata",
     "ImportUserEventsRequest",
     "ImportUserEventsResponse",
+    "PurgeDocumentsMetadata",
+    "PurgeDocumentsRequest",
+    "PurgeDocumentsResponse",
     "RecommendRequest",
     "RecommendResponse",
     "Schema",
     "CreateSchemaMetadata",
     "CreateSchemaRequest",
     "DeleteSchemaMetadata",
     "DeleteSchemaRequest",
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/common.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,17 @@
             The field must be a UTF-8 encoded string with a length limit
             of 1,000 characters. Otherwise, an ``INVALID_ARGUMENT``
             error is returned.
 
             This should not be set when using the client side event
             reporting with GTM or JavaScript tag in
             [UserEventService.CollectUserEvent][google.cloud.discoveryengine.v1beta.UserEventService.CollectUserEvent]
-            or if [direct_user_request][] is set.
+            or if
+            [UserEvent.direct_user_request][google.cloud.discoveryengine.v1beta.UserEvent.direct_user_request]
+            is set.
     """
 
     user_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
     user_agent: str = proto.Field(
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/completion_service.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/document.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/document_service.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/document_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/import_config.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/import_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/schema.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/schema_service.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/search_service.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/user_event.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/user_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,26 +126,29 @@
             information for certain event types such as
             ``view-category-page``.
         attribution_token (str):
             Token to attribute an API response to user action(s) to
             trigger the event.
 
             Highly recommended for user events that are the result of
-            [PredictionService.Predict][]. This field enables accurate
-            attribution of recommendation model performance.
+            [RecommendationService.Recommend][google.cloud.discoveryengine.v1beta.RecommendationService.Recommend].
+            This field enables accurate attribution of recommendation
+            model performance.
 
             The value must be one of:
 
             -  [PredictResponse.attribution_token][] for events that are
-               the result of [PredictionService.Predict][].
+               the result of
+               [RecommendationService.Recommend][google.cloud.discoveryengine.v1beta.RecommendationService.Recommend].
             -  [SearchResponse.attribution_token][google.cloud.discoveryengine.v1beta.SearchResponse.attribution_token]
                for events that are the result of
                [SearchService.Search][google.cloud.discoveryengine.v1beta.SearchService.Search].
             -  [CompleteQueryResponse.attribution_token][] for events
-               that are the result of [SearchService.CompleteQuery][].
+               that are the result of
+               [CompletionService.CompleteQuery][google.cloud.discoveryengine.v1beta.CompletionService.CompleteQuery].
 
             This token enables us to accurately attribute page view or
             conversion completion back to the event and the particular
             predict response containing this clicked/purchased product.
             If user clicks on product K in the recommendation results,
             pass [PredictResponse.attribution_token][] as a URL
             parameter to product K's page. When recording events on
@@ -153,23 +156,24 @@
             [PredictResponse.attribution_token][] to this field.
         filter (str):
             The filter syntax consists of an expression language for
             constructing a predicate from one or more fields of the
             documents being filtered.
 
             One example is for ``search`` events, the associated
-            [SearchService.SearchRequest][] may contain a filter
-            expression in [SearchService.SearchRequest.filter][]
+            [SearchRequest][google.cloud.discoveryengine.v1beta.SearchRequest]
+            may contain a filter expression in
+            [SearchRequest.filter][google.cloud.discoveryengine.v1beta.SearchRequest.filter]
             conforming to https://google.aip.dev/160#filtering.
 
             Similarly, for ``view-item-list`` events that are generated
-            from a [PredictionService.PredictRequest][], this field may
-            be populated directly from
-            [PredictionService.PredictRequest.filter][] conforming to
-            https://google.aip.dev/160#filtering.
+            from a [RecommendationService.RecommendRequest][], this
+            field may be populated directly from
+            [RecommendationService.RecommendRequest.filter][] conforming
+            to https://google.aip.dev/160#filtering.
 
             The value must be a UTF-8 encoded string with a length limit
             of 1,000 characters. Otherwise, an INVALID_ARGUMENT error is
             returned.
         documents (MutableSequence[google.cloud.discoveryengine_v1beta.types.DocumentInfo]):
             List of Documents associated with this user event.
 
@@ -414,17 +418,19 @@
 
             The value must be a UTF-8 encoded string with a length limit
             of 5,000 characters. Otherwise, an INVALID_ARGUMENT error is
             returned.
 
             At least one of
             [search_query][google.cloud.discoveryengine.v1beta.SearchInfo.search_query]
-            or [page_categories][] is required for ``search`` events.
-            Other event types should not set this field. Otherwise, an
-            INVALID_ARGUMENT error is returned.
+            or
+            [PageInfo.page_category][google.cloud.discoveryengine.v1beta.PageInfo.page_category]
+            is required for ``search`` events. Other event types should
+            not set this field. Otherwise, an INVALID_ARGUMENT error is
+            returned.
         order_by (str):
             The order in which products are returned, if applicable.
 
             See
             [SearchRequest.order_by][google.cloud.discoveryengine.v1beta.SearchRequest.order_by]
             for definition and syntax.
```

### Comparing `google-cloud-discoveryengine-0.5.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py` & `google-cloud-discoveryengine-0.6.0/google/cloud/discoveryengine_v1beta/types/user_event_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/PKG-INFO` & `google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-discoveryengine
-Version: 0.5.0
+Version: 0.6.0
 Summary: Google Cloud Discoveryengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-discoveryengine-0.5.0/google_cloud_discoveryengine.egg-info/SOURCES.txt` & `google-cloud-discoveryengine-0.6.0/google_cloud_discoveryengine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 google/cloud/discoveryengine_v1beta/services/user_event_service/transports/rest.py
 google/cloud/discoveryengine_v1beta/types/__init__.py
 google/cloud/discoveryengine_v1beta/types/common.py
 google/cloud/discoveryengine_v1beta/types/completion_service.py
 google/cloud/discoveryengine_v1beta/types/document.py
 google/cloud/discoveryengine_v1beta/types/document_service.py
 google/cloud/discoveryengine_v1beta/types/import_config.py
+google/cloud/discoveryengine_v1beta/types/purge_config.py
 google/cloud/discoveryengine_v1beta/types/recommendation_service.py
 google/cloud/discoveryengine_v1beta/types/schema.py
 google/cloud/discoveryengine_v1beta/types/schema_service.py
 google/cloud/discoveryengine_v1beta/types/search_service.py
 google/cloud/discoveryengine_v1beta/types/user_event.py
 google/cloud/discoveryengine_v1beta/types/user_event_service.py
 google_cloud_discoveryengine.egg-info/PKG-INFO
```

### Comparing `google-cloud-discoveryengine-0.5.0/setup.py` & `google-cloud-discoveryengine-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/tests/__init__.py` & `google-cloud-discoveryengine-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/tests/unit/__init__.py` & `google-cloud-discoveryengine-0.6.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/__init__.py` & `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py` & `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py` & `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_completion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py` & `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_document_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,19 @@
 
 from google.cloud.discoveryengine_v1beta.services.document_service import (
     DocumentServiceAsyncClient,
     DocumentServiceClient,
     pagers,
     transports,
 )
-from google.cloud.discoveryengine_v1beta.types import document_service, import_config
+from google.cloud.discoveryengine_v1beta.types import (
+    document_service,
+    import_config,
+    purge_config,
+)
 from google.cloud.discoveryengine_v1beta.types import document
 from google.cloud.discoveryengine_v1beta.types import document as gcd_document
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
@@ -2256,14 +2260,158 @@
         "parent=parent_value",
     ) in kw["metadata"]
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        purge_config.PurgeDocumentsRequest,
+        dict,
+    ],
+)
+def test_purge_documents(request_type, transport: str = "grpc"):
+    client = DocumentServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.purge_documents), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/spam")
+        response = client.purge_documents(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == purge_config.PurgeDocumentsRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+def test_purge_documents_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = DocumentServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.purge_documents), "__call__") as call:
+        client.purge_documents()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == purge_config.PurgeDocumentsRequest()
+
+
+@pytest.mark.asyncio
+async def test_purge_documents_async(
+    transport: str = "grpc_asyncio", request_type=purge_config.PurgeDocumentsRequest
+):
+    client = DocumentServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.purge_documents), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.purge_documents(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == purge_config.PurgeDocumentsRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+@pytest.mark.asyncio
+async def test_purge_documents_async_from_dict():
+    await test_purge_documents_async(request_type=dict)
+
+
+def test_purge_documents_field_headers():
+    client = DocumentServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = purge_config.PurgeDocumentsRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.purge_documents), "__call__") as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.purge_documents(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_purge_documents_field_headers_async():
+    client = DocumentServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = purge_config.PurgeDocumentsRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.purge_documents), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.purge_documents(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         document_service.GetDocumentRequest,
         dict,
     ],
 )
 def test_get_document_rest(request_type):
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3975,14 +4123,239 @@
 
 def test_import_documents_rest_error():
     client = DocumentServiceClient(
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        purge_config.PurgeDocumentsRequest,
+        dict,
+    ],
+)
+def test_purge_documents_rest(request_type):
+    client = DocumentServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "parent": "projects/sample1/locations/sample2/dataStores/sample3/branches/sample4"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.purge_documents(request)
+
+    # Establish that the response is the type that we expect.
+    assert response.operation.name == "operations/spam"
+
+
+def test_purge_documents_rest_required_fields(
+    request_type=purge_config.PurgeDocumentsRequest,
+):
+    transport_class = transports.DocumentServiceRestTransport
+
+    request_init = {}
+    request_init["parent"] = ""
+    request_init["filter"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).purge_documents._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["parent"] = "parent_value"
+    jsonified_request["filter"] = "filter_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).purge_documents._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "parent" in jsonified_request
+    assert jsonified_request["parent"] == "parent_value"
+    assert "filter" in jsonified_request
+    assert jsonified_request["filter"] == "filter_value"
+
+    client = DocumentServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = operations_pb2.Operation(name="operations/spam")
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "post",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.purge_documents(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_purge_documents_rest_unset_required_fields():
+    transport = transports.DocumentServiceRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.purge_documents._get_unset_required_fields({})
+    assert set(unset_fields) == (
+        set(())
+        & set(
+            (
+                "parent",
+                "filter",
+            )
+        )
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_purge_documents_rest_interceptors(null_interceptor):
+    transport = transports.DocumentServiceRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.DocumentServiceRestInterceptor(),
+    )
+    client = DocumentServiceClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        operation.Operation, "_set_result_from_operation"
+    ), mock.patch.object(
+        transports.DocumentServiceRestInterceptor, "post_purge_documents"
+    ) as post, mock.patch.object(
+        transports.DocumentServiceRestInterceptor, "pre_purge_documents"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = purge_config.PurgeDocumentsRequest.pb(
+            purge_config.PurgeDocumentsRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = json_format.MessageToJson(
+            operations_pb2.Operation()
+        )
+
+        request = purge_config.PurgeDocumentsRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = operations_pb2.Operation()
+
+        client.purge_documents(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_purge_documents_rest_bad_request(
+    transport: str = "rest", request_type=purge_config.PurgeDocumentsRequest
+):
+    client = DocumentServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "parent": "projects/sample1/locations/sample2/dataStores/sample3/branches/sample4"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.purge_documents(request)
+
+
+def test_purge_documents_rest_error():
+    client = DocumentServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.DocumentServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = DocumentServiceClient(
@@ -4120,14 +4493,15 @@
     methods = (
         "get_document",
         "list_documents",
         "create_document",
         "update_document",
         "delete_document",
         "import_documents",
+        "purge_documents",
         "get_operation",
         "list_operations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
@@ -4420,14 +4794,17 @@
     assert session1 != session2
     session1 = client1.transport.delete_document._session
     session2 = client2.transport.delete_document._session
     assert session1 != session2
     session1 = client1.transport.import_documents._session
     session2 = client2.transport.import_documents._session
     assert session1 != session2
+    session1 = client1.transport.purge_documents._session
+    session2 = client2.transport.purge_documents._session
+    assert session1 != session2
 
 
 def test_document_service_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.DocumentServiceGrpcTransport(
```

### Comparing `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py` & `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_recommendation_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py` & `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_schema_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py` & `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-discoveryengine-0.5.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py` & `google-cloud-discoveryengine-0.6.0/tests/unit/gapic/discoveryengine_v1beta/test_user_event_service.py`

 * *Files identical despite different names*

