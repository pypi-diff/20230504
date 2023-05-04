# Comparing `tmp/armonik-3.8.2.dev302.tar.gz` & `tmp/armonik-3.8.2.dev306.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armonik-3.8.2.dev302.tar", last modified: Thu May  4 07:41:59 2023, max compression
+gzip compressed data, was "armonik-3.8.2.dev306.tar", last modified: Thu May  4 15:32:45 2023, max compression
```

## Comparing `armonik-3.8.2.dev302.tar` & `armonik-3.8.2.dev306.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.542309 armonik-3.8.2.dev302/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-04 07:41:59.542309 armonik-3.8.2.dev302/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:41:59.542309 armonik-3.8.2.dev302/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.530309 armonik-3.8.2.dev302/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.530309 armonik-3.8.2.dev302/src/armonik/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.530309 armonik-3.8.2.dev302/src/armonik/client/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/client/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/client/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.530309 armonik-3.8.2.dev302/src/armonik/common/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/common/enumwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.530309 armonik-3.8.2.dev302/src/armonik/protogen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.534309 armonik-3.8.2.dev302/src/armonik/protogen/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/applications_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/applications_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/applications_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/auth_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/auth_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/auth_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/events_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/events_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/events_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/partitions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/partitions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/partitions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/results_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/results_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/results_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/sessions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/sessions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/sessions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/submitter_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/submitter_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/submitter_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/tasks_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/tasks_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/client/tasks_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.538309 armonik-3.8.2.dev302/src/armonik/protogen/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/agent_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/agent_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/agent_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/applications_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/applications_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/applications_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/auth_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/auth_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/auth_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/events_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/events_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/events_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/objects_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/objects_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/objects_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/partitions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/partitions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/partitions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/result_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/result_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/result_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/results_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/results_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/results_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/session_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/session_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/session_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/sessions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/sessions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/sessions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/submitter_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/submitter_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/submitter_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/task_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/task_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/task_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/tasks_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/tasks_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/tasks_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/worker_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/worker_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/common/worker_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.542309 armonik-3.8.2.dev302/src/armonik/protogen/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/worker/agent_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/worker/agent_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/worker/agent_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/worker/worker_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/worker/worker_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-04 07:41:53.000000 armonik-3.8.2.dev302/src/armonik/protogen/worker/worker_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.542309 armonik-3.8.2.dev302/src/armonik/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/worker/seqlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/worker/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 07:41:43.000000 armonik-3.8.2.dev302/src/armonik/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:41:59.530309 armonik-3.8.2.dev302/src/armonik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-04 07:41:59.000000 armonik-3.8.2.dev302/src/armonik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-04 07:41:59.000000 armonik-3.8.2.dev302/src/armonik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:41:59.000000 armonik-3.8.2.dev302/src/armonik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 07:41:59.000000 armonik-3.8.2.dev302/src/armonik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 07:41:59.000000 armonik-3.8.2.dev302/src/armonik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.659674 armonik-3.8.2.dev306/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.663674 armonik-3.8.2.dev306/src/armonik/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.663674 armonik-3.8.2.dev306/src/armonik/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/client/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/client/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.667674 armonik-3.8.2.dev306/src/armonik/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/common/enumwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.663674 armonik-3.8.2.dev306/src/armonik/protogen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.671674 armonik-3.8.2.dev306/src/armonik/protogen/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/results_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/results_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/results_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.679674 armonik-3.8.2.dev306/src/armonik/protogen/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/agent_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/agent_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/agent_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/result_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/result_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/result_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/results_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/results_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/results_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/session_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/session_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/session_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/src/armonik/protogen/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/src/armonik/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/worker/seqlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/worker/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.663674 armonik-3.8.2.dev306/src/armonik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/top_level.txt
```

### Comparing `armonik-3.8.2.dev302/PKG-INFO` & `armonik-3.8.2.dev306/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev302
+Version: 3.8.2.dev306
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev302/README.md` & `armonik-3.8.2.dev306/README.md`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/pyproject.toml` & `armonik-3.8.2.dev306/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/client/submitter.py` & `armonik-3.8.2.dev306/src/armonik/client/submitter.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/client/tasks.py` & `armonik-3.8.2.dev306/src/armonik/client/tasks.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/common/enumwrapper.py` & `armonik-3.8.2.dev306/src/armonik/common/enumwrapper.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/common/helpers.py` & `armonik-3.8.2.dev306/src/armonik/common/helpers.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/common/objects.py` & `armonik-3.8.2.dev306/src/armonik/common/objects.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/applications_service_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/applications_service_pb2_grpc.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/auth_service_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/auth_service_pb2_grpc.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/events_service_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/events_service_pb2_grpc.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/partitions_service_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/partitions_service_pb2_grpc.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/results_service_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: results_service.proto
+# source: worker_service.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from ..common import results_common_pb2 as results__common__pb2
+from ..common import objects_pb2 as objects__pb2
+from ..common import worker_common_pb2 as worker__common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15results_service.proto\x12\x1b\x61rmonik.api.grpc.v1.results\x1a\x14results_common.proto2\xf8\x01\n\x07Results\x12r\n\x0bListResults\x12/.armonik.api.grpc.v1.results.ListResultsRequest\x1a\x30.armonik.api.grpc.v1.results.ListResultsResponse\"\x00\x12y\n\x0eGetOwnerTaskId\x12\x32.armonik.api.grpc.v1.results.GetOwnerTaskIdRequest\x1a\x33.armonik.api.grpc.v1.results.GetOwnerTaskIdResponseB\x1e\xaa\x02\x1b\x41rmoniK.Api.gRPC.V1.Resultsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14worker_service.proto\x12\x1a\x61rmonik.api.grpc.v1.worker\x1a\robjects.proto\x1a\x13worker_common.proto2\xc4\x01\n\x06Worker\x12\x61\n\x07Process\x12*.armonik.api.grpc.v1.worker.ProcessRequest\x1a(.armonik.api.grpc.v1.worker.ProcessReply(\x01\x12W\n\x0bHealthCheck\x12\x1a.armonik.api.grpc.v1.Empty\x1a,.armonik.api.grpc.v1.worker.HealthCheckReplyB\x1d\xaa\x02\x1a\x41rmoniK.Api.gRPC.V1.Workerb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'results_service_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'worker_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\252\002\033ArmoniK.Api.gRPC.V1.Results'
-  _RESULTS._serialized_start=77
-  _RESULTS._serialized_end=325
+  DESCRIPTOR._serialized_options = b'\252\002\032ArmoniK.Api.gRPC.V1.Worker'
+  _WORKER._serialized_start=89
+  _WORKER._serialized_end=285
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/results_service_pb2_grpc.py` & `armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2_grpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,100 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from ..common import results_common_pb2 as results__common__pb2
+from ..common import objects_pb2 as objects__pb2
+from ..common import worker_common_pb2 as worker__common__pb2
 
 
-class ResultsStub(object):
-    """*
-    The ResultsService provides methods for interacting with results
-    """
+class WorkerStub(object):
+    """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.ListResults = channel.unary_unary(
-                '/armonik.api.grpc.v1.results.Results/ListResults',
-                request_serializer=results__common__pb2.ListResultsRequest.SerializeToString,
-                response_deserializer=results__common__pb2.ListResultsResponse.FromString,
+        self.Process = channel.stream_unary(
+                '/armonik.api.grpc.v1.worker.Worker/Process',
+                request_serializer=worker__common__pb2.ProcessRequest.SerializeToString,
+                response_deserializer=worker__common__pb2.ProcessReply.FromString,
                 )
-        self.GetOwnerTaskId = channel.unary_unary(
-                '/armonik.api.grpc.v1.results.Results/GetOwnerTaskId',
-                request_serializer=results__common__pb2.GetOwnerTaskIdRequest.SerializeToString,
-                response_deserializer=results__common__pb2.GetOwnerTaskIdResponse.FromString,
+        self.HealthCheck = channel.unary_unary(
+                '/armonik.api.grpc.v1.worker.Worker/HealthCheck',
+                request_serializer=objects__pb2.Empty.SerializeToString,
+                response_deserializer=worker__common__pb2.HealthCheckReply.FromString,
                 )
 
 
-class ResultsServicer(object):
-    """*
-    The ResultsService provides methods for interacting with results
-    """
-
-    def ListResults(self, request, context):
-        """*
-        Get a results list using pagination, filters and sorting
-        """
+class WorkerServicer(object):
+    """Missing associated documentation comment in .proto file."""
+
+    def Process(self, request_iterator, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetOwnerTaskId(self, request, context):
-        """*
-        Get the id of the task that should produce the result
-        """
+    def HealthCheck(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_ResultsServicer_to_server(servicer, server):
+def add_WorkerServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'ListResults': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListResults,
-                    request_deserializer=results__common__pb2.ListResultsRequest.FromString,
-                    response_serializer=results__common__pb2.ListResultsResponse.SerializeToString,
+            'Process': grpc.stream_unary_rpc_method_handler(
+                    servicer.Process,
+                    request_deserializer=worker__common__pb2.ProcessRequest.FromString,
+                    response_serializer=worker__common__pb2.ProcessReply.SerializeToString,
             ),
-            'GetOwnerTaskId': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetOwnerTaskId,
-                    request_deserializer=results__common__pb2.GetOwnerTaskIdRequest.FromString,
-                    response_serializer=results__common__pb2.GetOwnerTaskIdResponse.SerializeToString,
+            'HealthCheck': grpc.unary_unary_rpc_method_handler(
+                    servicer.HealthCheck,
+                    request_deserializer=objects__pb2.Empty.FromString,
+                    response_serializer=worker__common__pb2.HealthCheckReply.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'armonik.api.grpc.v1.results.Results', rpc_method_handlers)
+            'armonik.api.grpc.v1.worker.Worker', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class Results(object):
-    """*
-    The ResultsService provides methods for interacting with results
-    """
+class Worker(object):
+    """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def ListResults(request,
+    def Process(request_iterator,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.results.Results/ListResults',
-            results__common__pb2.ListResultsRequest.SerializeToString,
-            results__common__pb2.ListResultsResponse.FromString,
+        return grpc.experimental.stream_unary(request_iterator, target, '/armonik.api.grpc.v1.worker.Worker/Process',
+            worker__common__pb2.ProcessRequest.SerializeToString,
+            worker__common__pb2.ProcessReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetOwnerTaskId(request,
+    def HealthCheck(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.results.Results/GetOwnerTaskId',
-            results__common__pb2.GetOwnerTaskIdRequest.SerializeToString,
-            results__common__pb2.GetOwnerTaskIdResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.worker.Worker/HealthCheck',
+            objects__pb2.Empty.SerializeToString,
+            worker__common__pb2.HealthCheckReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/sessions_service_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/sessions_service_pb2_grpc.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/submitter_service_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/submitter_service_pb2_grpc.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/tasks_service_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import tasks_common_pb2 as tasks__common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13tasks_service.proto\x12\x19\x61rmonik.api.grpc.v1.tasks\x1a\x12tasks_common.proto2\xbc\x04\n\x05Tasks\x12h\n\tListTasks\x12+.armonik.api.grpc.v1.tasks.ListTasksRequest\x1a,.armonik.api.grpc.v1.tasks.ListTasksResponse\"\x00\x12\x62\n\x07GetTask\x12).armonik.api.grpc.v1.tasks.GetTaskRequest\x1a*.armonik.api.grpc.v1.tasks.GetTaskResponse\"\x00\x12n\n\x0b\x43\x61ncelTasks\x12-.armonik.api.grpc.v1.tasks.CancelTasksRequest\x1a..armonik.api.grpc.v1.tasks.CancelTasksResponse\"\x00\x12o\n\x0cGetResultIds\x12..armonik.api.grpc.v1.tasks.GetResultIdsRequest\x1a/.armonik.api.grpc.v1.tasks.GetResultIdsResponse\x12\x83\x01\n\x12\x43ountTasksByStatus\x12\x34.armonik.api.grpc.v1.tasks.CountTasksByStatusRequest\x1a\x35.armonik.api.grpc.v1.tasks.CountTasksByStatusResponse\"\x00\x42\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Tasksb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13tasks_service.proto\x12\x19\x61rmonik.api.grpc.v1.tasks\x1a\x12tasks_common.proto2\x9c\x06\n\x05Tasks\x12h\n\tListTasks\x12+.armonik.api.grpc.v1.tasks.ListTasksRequest\x1a,.armonik.api.grpc.v1.tasks.ListTasksResponse\"\x00\x12n\n\x0cListTasksRaw\x12+.armonik.api.grpc.v1.tasks.ListTasksRequest\x1a/.armonik.api.grpc.v1.tasks.ListTasksRawResponse\"\x00\x12\x62\n\x07GetTask\x12).armonik.api.grpc.v1.tasks.GetTaskRequest\x1a*.armonik.api.grpc.v1.tasks.GetTaskResponse\"\x00\x12n\n\x0b\x43\x61ncelTasks\x12-.armonik.api.grpc.v1.tasks.CancelTasksRequest\x1a..armonik.api.grpc.v1.tasks.CancelTasksResponse\"\x00\x12o\n\x0cGetResultIds\x12..armonik.api.grpc.v1.tasks.GetResultIdsRequest\x1a/.armonik.api.grpc.v1.tasks.GetResultIdsResponse\x12\x83\x01\n\x12\x43ountTasksByStatus\x12\x34.armonik.api.grpc.v1.tasks.CountTasksByStatusRequest\x1a\x35.armonik.api.grpc.v1.tasks.CountTasksByStatusResponse\"\x00\x12n\n\x0bSubmitTasks\x12-.armonik.api.grpc.v1.tasks.SubmitTasksRequest\x1a..armonik.api.grpc.v1.tasks.SubmitTasksResponse\"\x00\x42\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Tasksb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tasks_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\031ArmoniK.Api.gRPC.V1.Tasks'
   _TASKS._serialized_start=71
-  _TASKS._serialized_end=643
+  _TASKS._serialized_end=867
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/client/tasks_service_pb2_grpc.py` & `armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2_grpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,19 @@
             channel: A grpc.Channel.
         """
         self.ListTasks = channel.unary_unary(
                 '/armonik.api.grpc.v1.tasks.Tasks/ListTasks',
                 request_serializer=tasks__common__pb2.ListTasksRequest.SerializeToString,
                 response_deserializer=tasks__common__pb2.ListTasksResponse.FromString,
                 )
+        self.ListTasksRaw = channel.unary_unary(
+                '/armonik.api.grpc.v1.tasks.Tasks/ListTasksRaw',
+                request_serializer=tasks__common__pb2.ListTasksRequest.SerializeToString,
+                response_deserializer=tasks__common__pb2.ListTasksRawResponse.FromString,
+                )
         self.GetTask = channel.unary_unary(
                 '/armonik.api.grpc.v1.tasks.Tasks/GetTask',
                 request_serializer=tasks__common__pb2.GetTaskRequest.SerializeToString,
                 response_deserializer=tasks__common__pb2.GetTaskResponse.FromString,
                 )
         self.CancelTasks = channel.unary_unary(
                 '/armonik.api.grpc.v1.tasks.Tasks/CancelTasks',
@@ -37,14 +42,19 @@
                 response_deserializer=tasks__common__pb2.GetResultIdsResponse.FromString,
                 )
         self.CountTasksByStatus = channel.unary_unary(
                 '/armonik.api.grpc.v1.tasks.Tasks/CountTasksByStatus',
                 request_serializer=tasks__common__pb2.CountTasksByStatusRequest.SerializeToString,
                 response_deserializer=tasks__common__pb2.CountTasksByStatusResponse.FromString,
                 )
+        self.SubmitTasks = channel.unary_unary(
+                '/armonik.api.grpc.v1.tasks.Tasks/SubmitTasks',
+                request_serializer=tasks__common__pb2.SubmitTasksRequest.SerializeToString,
+                response_deserializer=tasks__common__pb2.SubmitTasksResponse.FromString,
+                )
 
 
 class TasksServicer(object):
     """*
     Service for handling tasks.
     """
 
@@ -52,14 +62,22 @@
         """*
         Get a tasks list using pagination, filters and sorting.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListTasksRaw(self, request, context):
+        """*
+        Get a tasks list using pagination, filters and sorting with complete metada.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetTask(self, request, context):
         """*
         Get a task by its id.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
@@ -84,22 +102,35 @@
         """*
         Get count from tasks status.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SubmitTasks(self, request, context):
+        """*
+        Create tasks metadata and submit task for processing.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_TasksServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ListTasks': grpc.unary_unary_rpc_method_handler(
                     servicer.ListTasks,
                     request_deserializer=tasks__common__pb2.ListTasksRequest.FromString,
                     response_serializer=tasks__common__pb2.ListTasksResponse.SerializeToString,
             ),
+            'ListTasksRaw': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListTasksRaw,
+                    request_deserializer=tasks__common__pb2.ListTasksRequest.FromString,
+                    response_serializer=tasks__common__pb2.ListTasksRawResponse.SerializeToString,
+            ),
             'GetTask': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTask,
                     request_deserializer=tasks__common__pb2.GetTaskRequest.FromString,
                     response_serializer=tasks__common__pb2.GetTaskResponse.SerializeToString,
             ),
             'CancelTasks': grpc.unary_unary_rpc_method_handler(
                     servicer.CancelTasks,
@@ -112,14 +143,19 @@
                     response_serializer=tasks__common__pb2.GetResultIdsResponse.SerializeToString,
             ),
             'CountTasksByStatus': grpc.unary_unary_rpc_method_handler(
                     servicer.CountTasksByStatus,
                     request_deserializer=tasks__common__pb2.CountTasksByStatusRequest.FromString,
                     response_serializer=tasks__common__pb2.CountTasksByStatusResponse.SerializeToString,
             ),
+            'SubmitTasks': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubmitTasks,
+                    request_deserializer=tasks__common__pb2.SubmitTasksRequest.FromString,
+                    response_serializer=tasks__common__pb2.SubmitTasksResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'armonik.api.grpc.v1.tasks.Tasks', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -142,14 +178,31 @@
         return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.tasks.Tasks/ListTasks',
             tasks__common__pb2.ListTasksRequest.SerializeToString,
             tasks__common__pb2.ListTasksResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ListTasksRaw(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.tasks.Tasks/ListTasksRaw',
+            tasks__common__pb2.ListTasksRequest.SerializeToString,
+            tasks__common__pb2.ListTasksRawResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetTask(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -208,7 +261,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.tasks.Tasks/CountTasksByStatus',
             tasks__common__pb2.CountTasksByStatusRequest.SerializeToString,
             tasks__common__pb2.CountTasksByStatusResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubmitTasks(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.tasks.Tasks/SubmitTasks',
+            tasks__common__pb2.SubmitTasksRequest.SerializeToString,
+            tasks__common__pb2.SubmitTasksResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/agent_common_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,68 @@
 from . import objects_pb2 as _objects_pb2
 from google.protobuf.internal import containers as _containers
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CreateTaskReply(_message.Message):
-    __slots__ = ["communication_token", "creation_status_list", "error"]
-    class CreationStatus(_message.Message):
-        __slots__ = ["error", "task_info"]
-        ERROR_FIELD_NUMBER: _ClassVar[int]
-        TASK_INFO_FIELD_NUMBER: _ClassVar[int]
-        error: str
-        task_info: CreateTaskReply.TaskInfo
-        def __init__(self, task_info: _Optional[_Union[CreateTaskReply.TaskInfo, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
-    class CreationStatusList(_message.Message):
-        __slots__ = ["creation_statuses"]
-        CREATION_STATUSES_FIELD_NUMBER: _ClassVar[int]
-        creation_statuses: _containers.RepeatedCompositeFieldContainer[CreateTaskReply.CreationStatus]
-        def __init__(self, creation_statuses: _Optional[_Iterable[_Union[CreateTaskReply.CreationStatus, _Mapping]]] = ...) -> None: ...
-    class TaskInfo(_message.Message):
-        __slots__ = ["data_dependencies", "expected_output_keys", "task_id"]
-        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
-        EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
-        expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
-        task_id: str
-        def __init__(self, task_id: _Optional[str] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ...) -> None: ...
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    CREATION_STATUS_LIST_FIELD_NUMBER: _ClassVar[int]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    creation_status_list: CreateTaskReply.CreationStatusList
-    error: str
-    def __init__(self, creation_status_list: _Optional[_Union[CreateTaskReply.CreationStatusList, _Mapping]] = ..., error: _Optional[str] = ..., communication_token: _Optional[str] = ...) -> None: ...
-
-class CreateTaskRequest(_message.Message):
-    __slots__ = ["communication_token", "init_request", "init_task", "task_payload"]
-    class InitRequest(_message.Message):
-        __slots__ = ["task_options"]
-        TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
-        task_options: _objects_pb2.TaskOptions
-        def __init__(self, task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    INIT_REQUEST_FIELD_NUMBER: _ClassVar[int]
-    INIT_TASK_FIELD_NUMBER: _ClassVar[int]
-    TASK_PAYLOAD_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    init_request: CreateTaskRequest.InitRequest
-    init_task: _objects_pb2.InitTaskRequest
-    task_payload: _objects_pb2.DataChunk
-    def __init__(self, init_request: _Optional[_Union[CreateTaskRequest.InitRequest, _Mapping]] = ..., init_task: _Optional[_Union[_objects_pb2.InitTaskRequest, _Mapping]] = ..., task_payload: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., communication_token: _Optional[str] = ...) -> None: ...
-
-class DataReply(_message.Message):
-    __slots__ = ["communication_token", "data", "error", "init"]
-    class Init(_message.Message):
-        __slots__ = ["data", "error", "key"]
+class HealthCheckReply(_message.Message):
+    __slots__ = ["status"]
+    class ServingStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+    NOT_SERVING: HealthCheckReply.ServingStatus
+    SERVING: HealthCheckReply.ServingStatus
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    UNKNOWN: HealthCheckReply.ServingStatus
+    status: HealthCheckReply.ServingStatus
+    def __init__(self, status: _Optional[_Union[HealthCheckReply.ServingStatus, str]] = ...) -> None: ...
+
+class ProcessReply(_message.Message):
+    __slots__ = ["communication_token", "output"]
+    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_FIELD_NUMBER: _ClassVar[int]
+    communication_token: str
+    output: _objects_pb2.Output
+    def __init__(self, communication_token: _Optional[str] = ..., output: _Optional[_Union[_objects_pb2.Output, _Mapping]] = ...) -> None: ...
+
+class ProcessRequest(_message.Message):
+    __slots__ = ["communication_token", "compute"]
+    class ComputeRequest(_message.Message):
+        __slots__ = ["data", "init_data", "init_request", "payload"]
+        class InitData(_message.Message):
+            __slots__ = ["key", "last_data"]
+            KEY_FIELD_NUMBER: _ClassVar[int]
+            LAST_DATA_FIELD_NUMBER: _ClassVar[int]
+            key: str
+            last_data: bool
+            def __init__(self, key: _Optional[str] = ..., last_data: bool = ...) -> None: ...
+        class InitRequest(_message.Message):
+            __slots__ = ["configuration", "expected_output_keys", "payload", "session_id", "task_id", "task_options"]
+            CONFIGURATION_FIELD_NUMBER: _ClassVar[int]
+            EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+            PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+            SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+            TASK_ID_FIELD_NUMBER: _ClassVar[int]
+            TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+            configuration: _objects_pb2.Configuration
+            expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+            payload: _objects_pb2.DataChunk
+            session_id: str
+            task_id: str
+            task_options: _objects_pb2.TaskOptions
+            def __init__(self, configuration: _Optional[_Union[_objects_pb2.Configuration, _Mapping]] = ..., session_id: _Optional[str] = ..., task_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., payload: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ...) -> None: ...
         DATA_FIELD_NUMBER: _ClassVar[int]
-        ERROR_FIELD_NUMBER: _ClassVar[int]
-        KEY_FIELD_NUMBER: _ClassVar[int]
+        INIT_DATA_FIELD_NUMBER: _ClassVar[int]
+        INIT_REQUEST_FIELD_NUMBER: _ClassVar[int]
+        PAYLOAD_FIELD_NUMBER: _ClassVar[int]
         data: _objects_pb2.DataChunk
-        error: str
-        key: str
-        def __init__(self, key: _Optional[str] = ..., data: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    INIT_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    data: _objects_pb2.DataChunk
-    error: str
-    init: DataReply.Init
-    def __init__(self, communication_token: _Optional[str] = ..., init: _Optional[_Union[DataReply.Init, _Mapping]] = ..., data: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
-
-class DataRequest(_message.Message):
-    __slots__ = ["communication_token", "key"]
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    KEY_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    key: str
-    def __init__(self, communication_token: _Optional[str] = ..., key: _Optional[str] = ...) -> None: ...
-
-class Result(_message.Message):
-    __slots__ = ["communication_token", "data", "init"]
-    COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    INIT_FIELD_NUMBER: _ClassVar[int]
-    communication_token: str
-    data: _objects_pb2.DataChunk
-    init: _objects_pb2.InitKeyedDataStream
-    def __init__(self, init: _Optional[_Union[_objects_pb2.InitKeyedDataStream, _Mapping]] = ..., data: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., communication_token: _Optional[str] = ...) -> None: ...
-
-class ResultReply(_message.Message):
-    __slots__ = ["Error", "Ok", "communication_token"]
+        init_data: ProcessRequest.ComputeRequest.InitData
+        init_request: ProcessRequest.ComputeRequest.InitRequest
+        payload: _objects_pb2.DataChunk
+        def __init__(self, init_request: _Optional[_Union[ProcessRequest.ComputeRequest.InitRequest, _Mapping]] = ..., payload: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ..., init_data: _Optional[_Union[ProcessRequest.ComputeRequest.InitData, _Mapping]] = ..., data: _Optional[_Union[_objects_pb2.DataChunk, _Mapping]] = ...) -> None: ...
     COMMUNICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
-    ERROR_FIELD_NUMBER: _ClassVar[int]
-    Error: str
-    OK_FIELD_NUMBER: _ClassVar[int]
-    Ok: _objects_pb2.Empty
+    COMPUTE_FIELD_NUMBER: _ClassVar[int]
     communication_token: str
-    def __init__(self, communication_token: _Optional[str] = ..., Ok: _Optional[_Union[_objects_pb2.Empty, _Mapping]] = ..., Error: _Optional[str] = ...) -> None: ...
+    compute: ProcessRequest.ComputeRequest
+    def __init__(self, communication_token: _Optional[str] = ..., compute: _Optional[_Union[ProcessRequest.ComputeRequest, _Mapping]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/applications_common_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/applications_common_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/auth_common_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/auth_common_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/events_common_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/events_common_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/objects_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from . import task_status_pb2 as task__status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\robjects.proto\x12\x13\x61rmonik.api.grpc.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x11task_status.proto\"\x07\n\x05\x45mpty\"\xf3\x02\n\x0bTaskOptions\x12>\n\x07options\x18\x01 \x03(\x0b\x32-.armonik.api.grpc.v1.TaskOptions.OptionsEntry\x12/\n\x0cmax_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x0bmax_retries\x18\x03 \x01(\x05\x12\x10\n\x08priority\x18\x04 \x01(\x05\x12\x14\n\x0cpartition_id\x18\x05 \x01(\t\x12\x18\n\x10\x61pplication_name\x18\x06 \x01(\t\x12\x1b\n\x13\x61pplication_version\x18\x07 \x01(\t\x12\x1d\n\x15\x61pplication_namespace\x18\x08 \x01(\t\x12\x1b\n\x13\x61pplication_service\x18\t \x01(\t\x12\x13\n\x0b\x65ngine_type\x18\n \x01(\t\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x15\n\x07Session\x12\n\n\x02id\x18\x01 \x01(\t\",\n\rConfiguration\x12\x1b\n\x13\x64\x61ta_chunk_max_size\x18\x01 \x01(\x05\"\x88\x01\n\x06Output\x12(\n\x02ok\x18\x02 \x01(\x0b\x32\x1a.armonik.api.grpc.v1.EmptyH\x00\x12\x32\n\x05\x65rror\x18\x03 \x01(\x0b\x32!.armonik.api.grpc.v1.Output.ErrorH\x00\x1a\x18\n\x05\x45rror\x12\x0f\n\x07\x64\x65tails\x18\x01 \x01(\tB\x06\n\x04type\"W\n\x0bTaskRequest\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\x12\x0f\n\x07payload\x18\x03 \x01(\x0c\"C\n\x13InitKeyedDataStream\x12\r\n\x03key\x18\x01 \x01(\tH\x00\x12\x15\n\x0blast_result\x18\x02 \x01(\x08H\x00\x42\x06\n\x04type\"<\n\tDataChunk\x12\x0e\n\x04\x64\x61ta\x18\x01 \x01(\x0cH\x00\x12\x17\n\rdata_complete\x18\x02 \x01(\x08H\x00\x42\x06\n\x04type\"L\n\x11TaskRequestHeader\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\"h\n\x0fInitTaskRequest\x12\x38\n\x06header\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.TaskRequestHeaderH\x00\x12\x13\n\tlast_task\x18\x02 \x01(\x08H\x00\x42\x06\n\x04type\"\'\n\x06TaskId\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x0c\n\x04task\x18\x02 \x01(\t\"\x1e\n\nTaskIdList\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"Y\n\x0bStatusCount\x12;\n\x06status\x18\x01 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\"9\n\x05\x43ount\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCount\"3\n\rResultRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\t\"5\n\x11TaskOutputRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"Y\n\x05\x45rror\x12@\n\x0btask_status\x18\x01 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x0e\n\x06\x64\x65tail\x18\x02 \x01(\t\"H\n\tTaskError\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12*\n\x06\x65rrors\x18\x02 \x03(\x0b\x32\x1a.armonik.api.grpc.v1.Error\"9\n\x08TaskList\x12-\n\x08task_ids\x18\x01 \x03(\x0b\x32\x1b.armonik.api.grpc.v1.TaskId\"}\n\x10TaskIdWithStatus\x12,\n\x07task_id\x18\x01 \x01(\x0b\x32\x1b.armonik.api.grpc.v1.TaskId\x12;\n\x06status\x18\x02 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatusB\x16\xaa\x02\x13\x41rmoniK.Api.gRPC.V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\robjects.proto\x12\x13\x61rmonik.api.grpc.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x11task_status.proto\"\x07\n\x05\x45mpty\"\xf3\x02\n\x0bTaskOptions\x12>\n\x07options\x18\x01 \x03(\x0b\x32-.armonik.api.grpc.v1.TaskOptions.OptionsEntry\x12/\n\x0cmax_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x0bmax_retries\x18\x03 \x01(\x05\x12\x10\n\x08priority\x18\x04 \x01(\x05\x12\x14\n\x0cpartition_id\x18\x05 \x01(\t\x12\x18\n\x10\x61pplication_name\x18\x06 \x01(\t\x12\x1b\n\x13\x61pplication_version\x18\x07 \x01(\t\x12\x1d\n\x15\x61pplication_namespace\x18\x08 \x01(\t\x12\x1b\n\x13\x61pplication_service\x18\t \x01(\t\x12\x13\n\x0b\x65ngine_type\x18\n \x01(\t\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x15\n\x07Session\x12\n\n\x02id\x18\x01 \x01(\t\",\n\rConfiguration\x12\x1b\n\x13\x64\x61ta_chunk_max_size\x18\x01 \x01(\x05\"\x88\x01\n\x06Output\x12(\n\x02ok\x18\x02 \x01(\x0b\x32\x1a.armonik.api.grpc.v1.EmptyH\x00\x12\x32\n\x05\x65rror\x18\x03 \x01(\x0b\x32!.armonik.api.grpc.v1.Output.ErrorH\x00\x1a\x18\n\x05\x45rror\x12\x0f\n\x07\x64\x65tails\x18\x01 \x01(\tB\x06\n\x04type\"m\n\x0bTaskRequest\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\x12\x0f\n\x07payload\x18\x03 \x01(\x0c\x12\x14\n\x0cpayload_name\x18\x04 \x01(\t\"C\n\x13InitKeyedDataStream\x12\r\n\x03key\x18\x01 \x01(\tH\x00\x12\x15\n\x0blast_result\x18\x02 \x01(\x08H\x00\x42\x06\n\x04type\"<\n\tDataChunk\x12\x0e\n\x04\x64\x61ta\x18\x01 \x01(\x0cH\x00\x12\x17\n\rdata_complete\x18\x02 \x01(\x08H\x00\x42\x06\n\x04type\"L\n\x11TaskRequestHeader\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\"h\n\x0fInitTaskRequest\x12\x38\n\x06header\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.TaskRequestHeaderH\x00\x12\x13\n\tlast_task\x18\x02 \x01(\x08H\x00\x42\x06\n\x04type\"\'\n\x06TaskId\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x0c\n\x04task\x18\x02 \x01(\t\"\x1e\n\nTaskIdList\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"Y\n\x0bStatusCount\x12;\n\x06status\x18\x01 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\"9\n\x05\x43ount\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCount\"3\n\rResultRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\t\"5\n\x11TaskOutputRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"Y\n\x05\x45rror\x12@\n\x0btask_status\x18\x01 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x0e\n\x06\x64\x65tail\x18\x02 \x01(\t\"H\n\tTaskError\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12*\n\x06\x65rrors\x18\x02 \x03(\x0b\x32\x1a.armonik.api.grpc.v1.Error\"9\n\x08TaskList\x12-\n\x08task_ids\x18\x01 \x03(\x0b\x32\x1b.armonik.api.grpc.v1.TaskId\"}\n\x10TaskIdWithStatus\x12,\n\x07task_id\x18\x01 \x01(\x0b\x32\x1b.armonik.api.grpc.v1.TaskId\x12;\n\x06status\x18\x02 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatusB\x16\xaa\x02\x13\x41rmoniK.Api.gRPC.V1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'objects_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\023ArmoniK.Api.gRPC.V1'
@@ -36,37 +36,37 @@
   _CONFIGURATION._serialized_start=495
   _CONFIGURATION._serialized_end=539
   _OUTPUT._serialized_start=542
   _OUTPUT._serialized_end=678
   _OUTPUT_ERROR._serialized_start=646
   _OUTPUT_ERROR._serialized_end=670
   _TASKREQUEST._serialized_start=680
-  _TASKREQUEST._serialized_end=767
-  _INITKEYEDDATASTREAM._serialized_start=769
-  _INITKEYEDDATASTREAM._serialized_end=836
-  _DATACHUNK._serialized_start=838
-  _DATACHUNK._serialized_end=898
-  _TASKREQUESTHEADER._serialized_start=900
-  _TASKREQUESTHEADER._serialized_end=976
-  _INITTASKREQUEST._serialized_start=978
-  _INITTASKREQUEST._serialized_end=1082
-  _TASKID._serialized_start=1084
-  _TASKID._serialized_end=1123
-  _TASKIDLIST._serialized_start=1125
-  _TASKIDLIST._serialized_end=1155
-  _STATUSCOUNT._serialized_start=1157
-  _STATUSCOUNT._serialized_end=1246
-  _COUNT._serialized_start=1248
-  _COUNT._serialized_end=1305
-  _RESULTREQUEST._serialized_start=1307
-  _RESULTREQUEST._serialized_end=1358
-  _TASKOUTPUTREQUEST._serialized_start=1360
-  _TASKOUTPUTREQUEST._serialized_end=1413
-  _ERROR._serialized_start=1415
-  _ERROR._serialized_end=1504
-  _TASKERROR._serialized_start=1506
-  _TASKERROR._serialized_end=1578
-  _TASKLIST._serialized_start=1580
-  _TASKLIST._serialized_end=1637
-  _TASKIDWITHSTATUS._serialized_start=1639
-  _TASKIDWITHSTATUS._serialized_end=1764
+  _TASKREQUEST._serialized_end=789
+  _INITKEYEDDATASTREAM._serialized_start=791
+  _INITKEYEDDATASTREAM._serialized_end=858
+  _DATACHUNK._serialized_start=860
+  _DATACHUNK._serialized_end=920
+  _TASKREQUESTHEADER._serialized_start=922
+  _TASKREQUESTHEADER._serialized_end=998
+  _INITTASKREQUEST._serialized_start=1000
+  _INITTASKREQUEST._serialized_end=1104
+  _TASKID._serialized_start=1106
+  _TASKID._serialized_end=1145
+  _TASKIDLIST._serialized_start=1147
+  _TASKIDLIST._serialized_end=1177
+  _STATUSCOUNT._serialized_start=1179
+  _STATUSCOUNT._serialized_end=1268
+  _COUNT._serialized_start=1270
+  _COUNT._serialized_end=1327
+  _RESULTREQUEST._serialized_start=1329
+  _RESULTREQUEST._serialized_end=1380
+  _TASKOUTPUTREQUEST._serialized_start=1382
+  _TASKOUTPUTREQUEST._serialized_end=1435
+  _ERROR._serialized_start=1437
+  _ERROR._serialized_end=1526
+  _TASKERROR._serialized_start=1528
+  _TASKERROR._serialized_end=1600
+  _TASKLIST._serialized_start=1602
+  _TASKLIST._serialized_end=1659
+  _TASKIDWITHSTATUS._serialized_start=1661
+  _TASKIDWITHSTATUS._serialized_end=1786
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/objects_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -162,22 +162,24 @@
     SESSION_FIELD_NUMBER: _ClassVar[int]
     TASK_ID_FIELD_NUMBER: _ClassVar[int]
     session: str
     task_id: str
     def __init__(self, session: _Optional[str] = ..., task_id: _Optional[str] = ...) -> None: ...
 
 class TaskRequest(_message.Message):
-    __slots__ = ["data_dependencies", "expected_output_keys", "payload"]
+    __slots__ = ["data_dependencies", "expected_output_keys", "payload", "payload_name"]
     DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
     EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
     PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    PAYLOAD_NAME_FIELD_NUMBER: _ClassVar[int]
     data_dependencies: _containers.RepeatedScalarFieldContainer[str]
     expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
     payload: bytes
-    def __init__(self, expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload: _Optional[bytes] = ...) -> None: ...
+    payload_name: str
+    def __init__(self, expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload: _Optional[bytes] = ..., payload_name: _Optional[str] = ...) -> None: ...
 
 class TaskRequestHeader(_message.Message):
     __slots__ = ["data_dependencies", "expected_output_keys"]
     DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
     EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
     data_dependencies: _containers.RepeatedScalarFieldContainer[str]
     expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/partitions_common_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/partitions_common_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/result_status_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/result_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/results_common_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,140 @@
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
-from . import result_status_pb2 as _result_status_pb2
+from . import objects_pb2 as _objects_pb2
+from . import session_status_pb2 as _session_status_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class GetOwnerTaskIdRequest(_message.Message):
-    __slots__ = ["result_id", "session_id"]
-    RESULT_ID_FIELD_NUMBER: _ClassVar[int]
+class CancelSessionRequest(_message.Message):
+    __slots__ = ["session_id"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    result_id: _containers.RepeatedScalarFieldContainer[str]
     session_id: str
-    def __init__(self, session_id: _Optional[str] = ..., result_id: _Optional[_Iterable[str]] = ...) -> None: ...
+    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
 
-class GetOwnerTaskIdResponse(_message.Message):
-    __slots__ = ["result_task", "session_id"]
-    class MapResultTask(_message.Message):
-        __slots__ = ["result_id", "task_id"]
-        RESULT_ID_FIELD_NUMBER: _ClassVar[int]
-        TASK_ID_FIELD_NUMBER: _ClassVar[int]
-        result_id: str
-        task_id: str
-        def __init__(self, result_id: _Optional[str] = ..., task_id: _Optional[str] = ...) -> None: ...
-    RESULT_TASK_FIELD_NUMBER: _ClassVar[int]
+class CancelSessionResponse(_message.Message):
+    __slots__ = ["session"]
+    SESSION_FIELD_NUMBER: _ClassVar[int]
+    session: SessionRaw
+    def __init__(self, session: _Optional[_Union[SessionRaw, _Mapping]] = ...) -> None: ...
+
+class CountTasksByStatusRequest(_message.Message):
+    __slots__ = ["session_id"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
-    result_task: _containers.RepeatedCompositeFieldContainer[GetOwnerTaskIdResponse.MapResultTask]
     session_id: str
-    def __init__(self, result_task: _Optional[_Iterable[_Union[GetOwnerTaskIdResponse.MapResultTask, _Mapping]]] = ..., session_id: _Optional[str] = ...) -> None: ...
+    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
+
+class CountTasksByStatusResponse(_message.Message):
+    __slots__ = ["status"]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    status: _containers.RepeatedCompositeFieldContainer[_objects_pb2.StatusCount]
+    def __init__(self, status: _Optional[_Iterable[_Union[_objects_pb2.StatusCount, _Mapping]]] = ...) -> None: ...
+
+class GetSessionRequest(_message.Message):
+    __slots__ = ["session_id"]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    session_id: str
+    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
+
+class GetSessionResponse(_message.Message):
+    __slots__ = ["session"]
+    SESSION_FIELD_NUMBER: _ClassVar[int]
+    session: SessionRaw
+    def __init__(self, session: _Optional[_Union[SessionRaw, _Mapping]] = ...) -> None: ...
 
-class ListResultsRequest(_message.Message):
-    __slots__ = ["filter", "page", "page_size", "sort"]
+class ListSessionsRequest(_message.Message):
+    __slots__ = ["filter", "page", "page_size", "sort", "with_task_options"]
     class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class Filter(_message.Message):
-        __slots__ = ["created_after", "created_before", "name", "owner_task_id", "session_id", "status"]
+        __slots__ = ["application_name", "application_version", "cancelled_after", "cancelled_before", "created_after", "created_before", "session_id", "status"]
+        APPLICATION_NAME_FIELD_NUMBER: _ClassVar[int]
+        APPLICATION_VERSION_FIELD_NUMBER: _ClassVar[int]
+        CANCELLED_AFTER_FIELD_NUMBER: _ClassVar[int]
+        CANCELLED_BEFORE_FIELD_NUMBER: _ClassVar[int]
         CREATED_AFTER_FIELD_NUMBER: _ClassVar[int]
         CREATED_BEFORE_FIELD_NUMBER: _ClassVar[int]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        OWNER_TASK_ID_FIELD_NUMBER: _ClassVar[int]
         SESSION_ID_FIELD_NUMBER: _ClassVar[int]
         STATUS_FIELD_NUMBER: _ClassVar[int]
+        application_name: str
+        application_version: str
+        cancelled_after: _timestamp_pb2.Timestamp
+        cancelled_before: _timestamp_pb2.Timestamp
         created_after: _timestamp_pb2.Timestamp
         created_before: _timestamp_pb2.Timestamp
-        name: str
-        owner_task_id: str
         session_id: str
-        status: _result_status_pb2.ResultStatus
-        def __init__(self, session_id: _Optional[str] = ..., name: _Optional[str] = ..., owner_task_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., created_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., created_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+        status: _session_status_pb2.SessionStatus
+        def __init__(self, application_name: _Optional[str] = ..., application_version: _Optional[str] = ..., session_id: _Optional[str] = ..., created_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., created_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ...) -> None: ...
     class Sort(_message.Message):
         __slots__ = ["direction", "field"]
         DIRECTION_FIELD_NUMBER: _ClassVar[int]
         FIELD_FIELD_NUMBER: _ClassVar[int]
-        direction: ListResultsRequest.OrderDirection
-        field: ListResultsRequest.OrderByField
-        def __init__(self, field: _Optional[_Union[ListResultsRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListResultsRequest.OrderDirection, str]] = ...) -> None: ...
+        direction: ListSessionsRequest.OrderDirection
+        field: ListSessionsRequest.OrderByField
+        def __init__(self, field: _Optional[_Union[ListSessionsRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListSessionsRequest.OrderDirection, str]] = ...) -> None: ...
     FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_CREATED_AT: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_NAME: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_OWNER_TASK_ID: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_SESSION_ID: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_STATUS: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListResultsRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListResultsRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListResultsRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListResultsRequest.OrderDirection
+    ORDER_BY_FIELD_CANCELLED_AT: ListSessionsRequest.OrderByField
+    ORDER_BY_FIELD_CREATED_AT: ListSessionsRequest.OrderByField
+    ORDER_BY_FIELD_SESSION_ID: ListSessionsRequest.OrderByField
+    ORDER_BY_FIELD_STATUS: ListSessionsRequest.OrderByField
+    ORDER_BY_FIELD_UNSPECIFIED: ListSessionsRequest.OrderByField
+    ORDER_DIRECTION_ASC: ListSessionsRequest.OrderDirection
+    ORDER_DIRECTION_DESC: ListSessionsRequest.OrderDirection
+    ORDER_DIRECTION_UNSPECIFIED: ListSessionsRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
-    filter: ListResultsRequest.Filter
+    WITH_TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    filter: ListSessionsRequest.Filter
     page: int
     page_size: int
-    sort: ListResultsRequest.Sort
-    def __init__(self, page: _Optional[int] = ..., page_size: _Optional[int] = ..., filter: _Optional[_Union[ListResultsRequest.Filter, _Mapping]] = ..., sort: _Optional[_Union[ListResultsRequest.Sort, _Mapping]] = ...) -> None: ...
+    sort: ListSessionsRequest.Sort
+    with_task_options: bool
+    def __init__(self, page: _Optional[int] = ..., page_size: _Optional[int] = ..., filter: _Optional[_Union[ListSessionsRequest.Filter, _Mapping]] = ..., sort: _Optional[_Union[ListSessionsRequest.Sort, _Mapping]] = ..., with_task_options: bool = ...) -> None: ...
 
-class ListResultsResponse(_message.Message):
-    __slots__ = ["page", "page_size", "results", "total"]
+class ListSessionsResponse(_message.Message):
+    __slots__ = ["page", "page_size", "sessions", "total"]
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
-    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    SESSIONS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     page: int
     page_size: int
-    results: _containers.RepeatedCompositeFieldContainer[ResultRaw]
+    sessions: _containers.RepeatedCompositeFieldContainer[SessionSummary]
     total: int
-    def __init__(self, results: _Optional[_Iterable[_Union[ResultRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
+    def __init__(self, sessions: _Optional[_Iterable[_Union[SessionSummary, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
+
+class SessionRaw(_message.Message):
+    __slots__ = ["cancelled_at", "created_at", "options", "partition_ids", "session_id", "status"]
+    CANCELLED_AT_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    PARTITION_IDS_FIELD_NUMBER: _ClassVar[int]
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    cancelled_at: _timestamp_pb2.Timestamp
+    created_at: _timestamp_pb2.Timestamp
+    options: _objects_pb2.TaskOptions
+    partition_ids: _containers.RepeatedScalarFieldContainer[str]
+    session_id: str
+    status: _session_status_pb2.SessionStatus
+    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., partition_ids: _Optional[_Iterable[str]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
-class ResultRaw(_message.Message):
-    __slots__ = ["created_at", "name", "owner_task_id", "session_id", "status"]
+class SessionSummary(_message.Message):
+    __slots__ = ["cancelled_at", "created_at", "options", "session_id", "status"]
+    CANCELLED_AT_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    OWNER_TASK_ID_FIELD_NUMBER: _ClassVar[int]
+    OPTIONS_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    cancelled_at: _timestamp_pb2.Timestamp
     created_at: _timestamp_pb2.Timestamp
-    name: str
-    owner_task_id: str
+    options: _objects_pb2.TaskOptions
     session_id: str
-    status: _result_status_pb2.ResultStatus
-    def __init__(self, session_id: _Optional[str] = ..., name: _Optional[str] = ..., owner_task_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+    status: _session_status_pb2.SessionStatus
+    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/session_status_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/session_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/sessions_common_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/submitter_common_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from . import objects_pb2 as objects__pb2
 from . import result_status_pb2 as result__status__pb2
 from . import session_status_pb2 as session__status__pb2
 from . import task_status_pb2 as task__status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16submitter_common.proto\x12\x1d\x61rmonik.api.grpc.v1.submitter\x1a\robjects.proto\x1a\x13result_status.proto\x1a\x14session_status.proto\x1a\x11task_status.proto\"=\n\x0bSessionList\x12.\n\x08sessions\x18\x01 \x03(\x0b\x32\x1c.armonik.api.grpc.v1.Session\"$\n\rSessionIdList\x12\x13\n\x0bsession_ids\x18\x01 \x03(\t\"l\n\x14\x43reateSessionRequest\x12=\n\x13\x64\x65\x66\x61ult_task_option\x18\x01 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12\x15\n\rpartition_ids\x18\x02 \x03(\t\"(\n\x12\x43reateSessionReply\x12\x12\n\nsession_id\x18\x01 \x01(\t\"\x9d\x01\n\x16\x43reateSmallTaskRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12\x37\n\rtask_requests\x18\x03 \x03(\x0b\x32 .armonik.api.grpc.v1.TaskRequest\"\xc9\x02\n\x16\x43reateLargeTaskRequest\x12Y\n\x0cinit_request\x18\x01 \x01(\x0b\x32\x41.armonik.api.grpc.v1.submitter.CreateLargeTaskRequest.InitRequestH\x00\x12\x39\n\tinit_task\x18\x02 \x01(\x0b\x32$.armonik.api.grpc.v1.InitTaskRequestH\x00\x12\x36\n\x0ctask_payload\x18\x03 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x1aY\n\x0bInitRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptionsB\x06\n\x04type\"\xd2\x03\n\x0f\x43reateTaskReply\x12\x61\n\x14\x63reation_status_list\x18\x01 \x01(\x0b\x32\x41.armonik.api.grpc.v1.submitter.CreateTaskReply.CreationStatusListH\x00\x12\x0f\n\x05\x65rror\x18\x02 \x01(\tH\x00\x1aT\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x1c\n\x14\x65xpected_output_keys\x18\x02 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x03 \x03(\t\x1ay\n\x0e\x43reationStatus\x12L\n\ttask_info\x18\x01 \x01(\x0b\x32\x37.armonik.api.grpc.v1.submitter.CreateTaskReply.TaskInfoH\x00\x12\x0f\n\x05\x65rror\x18\x02 \x01(\tH\x00\x42\x08\n\x06Status\x1an\n\x12\x43reationStatusList\x12X\n\x11\x63reation_statuses\x18\x01 \x03(\x0b\x32=.armonik.api.grpc.v1.submitter.CreateTaskReply.CreationStatusB\n\n\x08Response\"\xb9\x03\n\nTaskFilter\x12G\n\x07session\x18\x01 \x01(\x0b\x32\x34.armonik.api.grpc.v1.submitter.TaskFilter.IdsRequestH\x00\x12\x44\n\x04task\x18\x03 \x01(\x0b\x32\x34.armonik.api.grpc.v1.submitter.TaskFilter.IdsRequestH\x00\x12M\n\x08included\x18\x04 \x01(\x0b\x32\x39.armonik.api.grpc.v1.submitter.TaskFilter.StatusesRequestH\x01\x12M\n\x08\x65xcluded\x18\x05 \x01(\x0b\x32\x39.armonik.api.grpc.v1.submitter.TaskFilter.StatusesRequestH\x01\x1a\x19\n\nIdsRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x1aP\n\x0fStatusesRequest\x12=\n\x08statuses\x18\x01 \x03(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatusB\x05\n\x03idsB\n\n\x08statuses\"\xa9\x02\n\rSessionFilter\x12\x10\n\x08sessions\x18\x01 \x03(\t\x12P\n\x08included\x18\x04 \x01(\x0b\x32<.armonik.api.grpc.v1.submitter.SessionFilter.StatusesRequestH\x00\x12P\n\x08\x65xcluded\x18\x05 \x01(\x0b\x32<.armonik.api.grpc.v1.submitter.SessionFilter.StatusesRequestH\x00\x1aV\n\x0fStatusesRequest\x12\x43\n\x08statuses\x18\x01 \x03(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatusB\n\n\x08statuses\"(\n\x14GetTaskStatusRequest\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"\xbf\x01\n\x12GetTaskStatusReply\x12O\n\x0bid_statuses\x18\x01 \x03(\x0b\x32:.armonik.api.grpc.v1.submitter.GetTaskStatusReply.IdStatus\x1aX\n\x08IdStatus\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12;\n\x06status\x18\x02 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\"@\n\x16GetResultStatusRequest\x12\x12\n\nresult_ids\x18\x01 \x03(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\"\xc9\x01\n\x14GetResultStatusReply\x12Q\n\x0bid_statuses\x18\x01 \x03(\x0b\x32<.armonik.api.grpc.v1.submitter.GetResultStatusReply.IdStatus\x1a^\n\x08IdStatus\x12\x11\n\tresult_id\x18\x01 \x01(\t\x12?\n\x06status\x18\x02 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\"\x96\x01\n\x0bResultReply\x12\x30\n\x06result\x18\x01 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x12/\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.TaskErrorH\x00\x12\x1c\n\x12not_completed_task\x18\x03 \x01(\tH\x00\x42\x06\n\x04type\"\x94\x01\n\x11\x41vailabilityReply\x12(\n\x02ok\x18\x01 \x01(\x0b\x32\x1a.armonik.api.grpc.v1.EmptyH\x00\x12/\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.TaskErrorH\x00\x12\x1c\n\x12not_completed_task\x18\x03 \x01(\tH\x00\x42\x06\n\x04type\"\x93\x01\n\x0bWaitRequest\x12\x39\n\x06\x66ilter\x18\x01 \x01(\x0b\x32).armonik.api.grpc.v1.submitter.TaskFilter\x12 \n\x18stop_on_first_task_error\x18\x02 \x01(\x08\x12\'\n\x1fstop_on_first_task_cancellation\x18\x03 \x01(\x08\"\xba\x01\n\x12WatchResultRequest\x12G\n\x0e\x66\x65tch_statuses\x18\x01 \x03(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12G\n\x0ewatch_statuses\x18\x02 \x03(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x12\n\nresult_ids\x18\x03 \x03(\t\"h\n\x11WatchResultStream\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x12\n\nresult_ids\x18\x02 \x03(\tB \xaa\x02\x1d\x41rmoniK.Api.gRPC.V1.Submitterb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16submitter_common.proto\x12\x1d\x61rmonik.api.grpc.v1.submitter\x1a\robjects.proto\x1a\x13result_status.proto\x1a\x14session_status.proto\x1a\x11task_status.proto\"=\n\x0bSessionList\x12.\n\x08sessions\x18\x01 \x03(\x0b\x32\x1c.armonik.api.grpc.v1.Session\"$\n\rSessionIdList\x12\x13\n\x0bsession_ids\x18\x01 \x03(\t\"l\n\x14\x43reateSessionRequest\x12=\n\x13\x64\x65\x66\x61ult_task_option\x18\x01 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12\x15\n\rpartition_ids\x18\x02 \x03(\t\"(\n\x12\x43reateSessionReply\x12\x12\n\nsession_id\x18\x01 \x01(\t\"\x9d\x01\n\x16\x43reateSmallTaskRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12\x37\n\rtask_requests\x18\x03 \x03(\x0b\x32 .armonik.api.grpc.v1.TaskRequest\"\xc9\x02\n\x16\x43reateLargeTaskRequest\x12Y\n\x0cinit_request\x18\x01 \x01(\x0b\x32\x41.armonik.api.grpc.v1.submitter.CreateLargeTaskRequest.InitRequestH\x00\x12\x39\n\tinit_task\x18\x02 \x01(\x0b\x32$.armonik.api.grpc.v1.InitTaskRequestH\x00\x12\x36\n\x0ctask_payload\x18\x03 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x1aY\n\x0bInitRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptionsB\x06\n\x04type\"\xe6\x03\n\x0f\x43reateTaskReply\x12\x61\n\x14\x63reation_status_list\x18\x01 \x01(\x0b\x32\x41.armonik.api.grpc.v1.submitter.CreateTaskReply.CreationStatusListH\x00\x12\x0f\n\x05\x65rror\x18\x02 \x01(\tH\x00\x1ah\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x1c\n\x14\x65xpected_output_keys\x18\x02 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x03 \x03(\t\x12\x12\n\npayload_id\x18\x04 \x01(\t\x1ay\n\x0e\x43reationStatus\x12L\n\ttask_info\x18\x01 \x01(\x0b\x32\x37.armonik.api.grpc.v1.submitter.CreateTaskReply.TaskInfoH\x00\x12\x0f\n\x05\x65rror\x18\x02 \x01(\tH\x00\x42\x08\n\x06Status\x1an\n\x12\x43reationStatusList\x12X\n\x11\x63reation_statuses\x18\x01 \x03(\x0b\x32=.armonik.api.grpc.v1.submitter.CreateTaskReply.CreationStatusB\n\n\x08Response\"\xb9\x03\n\nTaskFilter\x12G\n\x07session\x18\x01 \x01(\x0b\x32\x34.armonik.api.grpc.v1.submitter.TaskFilter.IdsRequestH\x00\x12\x44\n\x04task\x18\x03 \x01(\x0b\x32\x34.armonik.api.grpc.v1.submitter.TaskFilter.IdsRequestH\x00\x12M\n\x08included\x18\x04 \x01(\x0b\x32\x39.armonik.api.grpc.v1.submitter.TaskFilter.StatusesRequestH\x01\x12M\n\x08\x65xcluded\x18\x05 \x01(\x0b\x32\x39.armonik.api.grpc.v1.submitter.TaskFilter.StatusesRequestH\x01\x1a\x19\n\nIdsRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\x1aP\n\x0fStatusesRequest\x12=\n\x08statuses\x18\x01 \x03(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatusB\x05\n\x03idsB\n\n\x08statuses\"\xa9\x02\n\rSessionFilter\x12\x10\n\x08sessions\x18\x01 \x03(\t\x12P\n\x08included\x18\x04 \x01(\x0b\x32<.armonik.api.grpc.v1.submitter.SessionFilter.StatusesRequestH\x00\x12P\n\x08\x65xcluded\x18\x05 \x01(\x0b\x32<.armonik.api.grpc.v1.submitter.SessionFilter.StatusesRequestH\x00\x1aV\n\x0fStatusesRequest\x12\x43\n\x08statuses\x18\x01 \x03(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatusB\n\n\x08statuses\"(\n\x14GetTaskStatusRequest\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"\xbf\x01\n\x12GetTaskStatusReply\x12O\n\x0bid_statuses\x18\x01 \x03(\x0b\x32:.armonik.api.grpc.v1.submitter.GetTaskStatusReply.IdStatus\x1aX\n\x08IdStatus\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12;\n\x06status\x18\x02 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\"@\n\x16GetResultStatusRequest\x12\x12\n\nresult_ids\x18\x01 \x03(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\"\xc9\x01\n\x14GetResultStatusReply\x12Q\n\x0bid_statuses\x18\x01 \x03(\x0b\x32<.armonik.api.grpc.v1.submitter.GetResultStatusReply.IdStatus\x1a^\n\x08IdStatus\x12\x11\n\tresult_id\x18\x01 \x01(\t\x12?\n\x06status\x18\x02 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\"\x96\x01\n\x0bResultReply\x12\x30\n\x06result\x18\x01 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.DataChunkH\x00\x12/\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.TaskErrorH\x00\x12\x1c\n\x12not_completed_task\x18\x03 \x01(\tH\x00\x42\x06\n\x04type\"\x94\x01\n\x11\x41vailabilityReply\x12(\n\x02ok\x18\x01 \x01(\x0b\x32\x1a.armonik.api.grpc.v1.EmptyH\x00\x12/\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1e.armonik.api.grpc.v1.TaskErrorH\x00\x12\x1c\n\x12not_completed_task\x18\x03 \x01(\tH\x00\x42\x06\n\x04type\"\x93\x01\n\x0bWaitRequest\x12\x39\n\x06\x66ilter\x18\x01 \x01(\x0b\x32).armonik.api.grpc.v1.submitter.TaskFilter\x12 \n\x18stop_on_first_task_error\x18\x02 \x01(\x08\x12\'\n\x1fstop_on_first_task_cancellation\x18\x03 \x01(\x08\"\xba\x01\n\x12WatchResultRequest\x12G\n\x0e\x66\x65tch_statuses\x18\x01 \x03(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12G\n\x0ewatch_statuses\x18\x02 \x03(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x12\n\nresult_ids\x18\x03 \x03(\t\"h\n\x11WatchResultStream\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x12\n\nresult_ids\x18\x02 \x03(\tB \xaa\x02\x1d\x41rmoniK.Api.gRPC.V1.Submitterb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'submitter_common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\035ArmoniK.Api.gRPC.V1.Submitter'
@@ -36,47 +36,47 @@
   _CREATESMALLTASKREQUEST._serialized_start=388
   _CREATESMALLTASKREQUEST._serialized_end=545
   _CREATELARGETASKREQUEST._serialized_start=548
   _CREATELARGETASKREQUEST._serialized_end=877
   _CREATELARGETASKREQUEST_INITREQUEST._serialized_start=780
   _CREATELARGETASKREQUEST_INITREQUEST._serialized_end=869
   _CREATETASKREPLY._serialized_start=880
-  _CREATETASKREPLY._serialized_end=1346
+  _CREATETASKREPLY._serialized_end=1366
   _CREATETASKREPLY_TASKINFO._serialized_start=1015
-  _CREATETASKREPLY_TASKINFO._serialized_end=1099
-  _CREATETASKREPLY_CREATIONSTATUS._serialized_start=1101
-  _CREATETASKREPLY_CREATIONSTATUS._serialized_end=1222
-  _CREATETASKREPLY_CREATIONSTATUSLIST._serialized_start=1224
-  _CREATETASKREPLY_CREATIONSTATUSLIST._serialized_end=1334
-  _TASKFILTER._serialized_start=1349
-  _TASKFILTER._serialized_end=1790
-  _TASKFILTER_IDSREQUEST._serialized_start=1664
-  _TASKFILTER_IDSREQUEST._serialized_end=1689
-  _TASKFILTER_STATUSESREQUEST._serialized_start=1691
-  _TASKFILTER_STATUSESREQUEST._serialized_end=1771
-  _SESSIONFILTER._serialized_start=1793
-  _SESSIONFILTER._serialized_end=2090
-  _SESSIONFILTER_STATUSESREQUEST._serialized_start=1992
-  _SESSIONFILTER_STATUSESREQUEST._serialized_end=2078
-  _GETTASKSTATUSREQUEST._serialized_start=2092
-  _GETTASKSTATUSREQUEST._serialized_end=2132
-  _GETTASKSTATUSREPLY._serialized_start=2135
-  _GETTASKSTATUSREPLY._serialized_end=2326
-  _GETTASKSTATUSREPLY_IDSTATUS._serialized_start=2238
-  _GETTASKSTATUSREPLY_IDSTATUS._serialized_end=2326
-  _GETRESULTSTATUSREQUEST._serialized_start=2328
-  _GETRESULTSTATUSREQUEST._serialized_end=2392
-  _GETRESULTSTATUSREPLY._serialized_start=2395
-  _GETRESULTSTATUSREPLY._serialized_end=2596
-  _GETRESULTSTATUSREPLY_IDSTATUS._serialized_start=2502
-  _GETRESULTSTATUSREPLY_IDSTATUS._serialized_end=2596
-  _RESULTREPLY._serialized_start=2599
-  _RESULTREPLY._serialized_end=2749
-  _AVAILABILITYREPLY._serialized_start=2752
-  _AVAILABILITYREPLY._serialized_end=2900
-  _WAITREQUEST._serialized_start=2903
-  _WAITREQUEST._serialized_end=3050
-  _WATCHRESULTREQUEST._serialized_start=3053
-  _WATCHRESULTREQUEST._serialized_end=3239
-  _WATCHRESULTSTREAM._serialized_start=3241
-  _WATCHRESULTSTREAM._serialized_end=3345
+  _CREATETASKREPLY_TASKINFO._serialized_end=1119
+  _CREATETASKREPLY_CREATIONSTATUS._serialized_start=1121
+  _CREATETASKREPLY_CREATIONSTATUS._serialized_end=1242
+  _CREATETASKREPLY_CREATIONSTATUSLIST._serialized_start=1244
+  _CREATETASKREPLY_CREATIONSTATUSLIST._serialized_end=1354
+  _TASKFILTER._serialized_start=1369
+  _TASKFILTER._serialized_end=1810
+  _TASKFILTER_IDSREQUEST._serialized_start=1684
+  _TASKFILTER_IDSREQUEST._serialized_end=1709
+  _TASKFILTER_STATUSESREQUEST._serialized_start=1711
+  _TASKFILTER_STATUSESREQUEST._serialized_end=1791
+  _SESSIONFILTER._serialized_start=1813
+  _SESSIONFILTER._serialized_end=2110
+  _SESSIONFILTER_STATUSESREQUEST._serialized_start=2012
+  _SESSIONFILTER_STATUSESREQUEST._serialized_end=2098
+  _GETTASKSTATUSREQUEST._serialized_start=2112
+  _GETTASKSTATUSREQUEST._serialized_end=2152
+  _GETTASKSTATUSREPLY._serialized_start=2155
+  _GETTASKSTATUSREPLY._serialized_end=2346
+  _GETTASKSTATUSREPLY_IDSTATUS._serialized_start=2258
+  _GETTASKSTATUSREPLY_IDSTATUS._serialized_end=2346
+  _GETRESULTSTATUSREQUEST._serialized_start=2348
+  _GETRESULTSTATUSREQUEST._serialized_end=2412
+  _GETRESULTSTATUSREPLY._serialized_start=2415
+  _GETRESULTSTATUSREPLY._serialized_end=2616
+  _GETRESULTSTATUSREPLY_IDSTATUS._serialized_start=2522
+  _GETRESULTSTATUSREPLY_IDSTATUS._serialized_end=2616
+  _RESULTREPLY._serialized_start=2619
+  _RESULTREPLY._serialized_end=2769
+  _AVAILABILITYREPLY._serialized_start=2772
+  _AVAILABILITYREPLY._serialized_end=2920
+  _WAITREQUEST._serialized_start=2923
+  _WAITREQUEST._serialized_end=3070
+  _WATCHRESULTREQUEST._serialized_start=3073
+  _WATCHRESULTREQUEST._serialized_end=3259
+  _WATCHRESULTSTREAM._serialized_start=3261
+  _WATCHRESULTSTREAM._serialized_end=3365
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/submitter_common_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -71,22 +71,24 @@
         def __init__(self, task_info: _Optional[_Union[CreateTaskReply.TaskInfo, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
     class CreationStatusList(_message.Message):
         __slots__ = ["creation_statuses"]
         CREATION_STATUSES_FIELD_NUMBER: _ClassVar[int]
         creation_statuses: _containers.RepeatedCompositeFieldContainer[CreateTaskReply.CreationStatus]
         def __init__(self, creation_statuses: _Optional[_Iterable[_Union[CreateTaskReply.CreationStatus, _Mapping]]] = ...) -> None: ...
     class TaskInfo(_message.Message):
-        __slots__ = ["data_dependencies", "expected_output_keys", "task_id"]
+        __slots__ = ["data_dependencies", "expected_output_keys", "payload_id", "task_id"]
         DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
         EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+        PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
         TASK_ID_FIELD_NUMBER: _ClassVar[int]
         data_dependencies: _containers.RepeatedScalarFieldContainer[str]
         expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+        payload_id: str
         task_id: str
-        def __init__(self, task_id: _Optional[str] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ...) -> None: ...
+        def __init__(self, task_id: _Optional[str] = ..., expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
     CREATION_STATUS_LIST_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     creation_status_list: CreateTaskReply.CreationStatusList
     error: str
     def __init__(self, creation_status_list: _Optional[_Union[CreateTaskReply.CreationStatusList, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
 
 class GetResultStatusReply(_message.Message):
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/task_status_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/task_status_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/tasks_common_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import objects_pb2 as objects__pb2
 from . import task_status_pb2 as task__status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12tasks_common.proto\x12\x19\x61rmonik.api.grpc.v1.tasks\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x11task_status.proto\"\xf8\x05\n\x07TaskRaw\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x14\n\x0cowner_pod_id\x18\x03 \x01(\t\x12\x17\n\x0fparent_task_ids\x18\x04 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x05 \x03(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x06 \x03(\t\x12\x14\n\x0cretry_of_ids\x18\x07 \x03(\t\x12;\n\x06status\x18\x08 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x16\n\x0estatus_message\x18\t \x01(\t\x12\x31\n\x07options\x18\n \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0csubmitted_at\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07pod_ttl\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x06output\x18\x10 \x01(\x0b\x32).armonik.api.grpc.v1.tasks.TaskRaw.Output\x12\x14\n\x0cpod_hostname\x18\x11 \x01(\t\x12/\n\x0breceived_at\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x61\x63quired_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a(\n\x06Output\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\xba\x02\n\x0bTaskSummary\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x31\n\x07options\x18\x03 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12;\n\x06status\x18\x04 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05\x65rror\x18\x08 \x01(\t\"\xc2\x08\n\x10ListTasksRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x42\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x32.armonik.api.grpc.v1.tasks.ListTasksRequest.Filter\x12>\n\x04sort\x18\x04 \x01(\x0b\x32\x30.armonik.api.grpc.v1.tasks.ListTasksRequest.Sort\x12\x13\n\x0bwith_errors\x18\x05 \x01(\x08\x1a\x8a\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x06status\x18\x02 \x03(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x31\n\rcreated_after\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rstarted_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0estarted_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x65nded_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x65nded_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\x9e\x01\n\x04Sort\x12G\n\x05\x66ield\x18\x01 \x01(\x0e\x32\x38.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderByField\x12M\n\tdirection\x18\x02 \x01(\x0e\x32:.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderDirection\"\xdf\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1a\n\x16ORDER_BY_FIELD_TASK_ID\x10\x01\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x02\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x03\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x04\x12\x1d\n\x19ORDER_BY_FIELD_STARTED_AT\x10\x05\x12\x1b\n\x17ORDER_BY_FIELD_ENDED_AT\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"z\n\x11ListTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"!\n\x0eGetTaskRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\t\"C\n\x0fGetTaskResponse\x12\x30\n\x04task\x18\x01 \x01(\x0b\x32\".armonik.api.grpc.v1.tasks.TaskRaw\"&\n\x12\x43\x61ncelTasksRequest\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"L\n\x13\x43\x61ncelTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\"&\n\x13GetResultIdsRequest\x12\x0f\n\x07task_id\x18\x01 \x03(\t\"\xa1\x01\n\x14GetResultIdsResponse\x12S\n\x0ctask_results\x18\x01 \x03(\x0b\x32=.armonik.api.grpc.v1.tasks.GetResultIdsResponse.MapTaskResult\x1a\x34\n\rMapTaskResult\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x12\n\nresult_ids\x18\x02 \x03(\t\"\x1b\n\x19\x43ountTasksByStatusRequest\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCountB\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Tasksb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12tasks_common.proto\x12\x19\x61rmonik.api.grpc.v1.tasks\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x11task_status.proto\"\xf8\x05\n\x07TaskRaw\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x14\n\x0cowner_pod_id\x18\x03 \x01(\t\x12\x17\n\x0fparent_task_ids\x18\x04 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x05 \x03(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x06 \x03(\t\x12\x14\n\x0cretry_of_ids\x18\x07 \x03(\t\x12;\n\x06status\x18\x08 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x16\n\x0estatus_message\x18\t \x01(\t\x12\x31\n\x07options\x18\n \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0csubmitted_at\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07pod_ttl\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x06output\x18\x10 \x01(\x0b\x32).armonik.api.grpc.v1.tasks.TaskRaw.Output\x12\x14\n\x0cpod_hostname\x18\x11 \x01(\t\x12/\n\x0breceived_at\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x61\x63quired_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a(\n\x06Output\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\xba\x02\n\x0bTaskSummary\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x31\n\x07options\x18\x03 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12;\n\x06status\x18\x04 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05\x65rror\x18\x08 \x01(\t\"\xc2\x08\n\x10ListTasksRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x42\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x32.armonik.api.grpc.v1.tasks.ListTasksRequest.Filter\x12>\n\x04sort\x18\x04 \x01(\x0b\x32\x30.armonik.api.grpc.v1.tasks.ListTasksRequest.Sort\x12\x13\n\x0bwith_errors\x18\x05 \x01(\x08\x1a\x8a\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x06status\x18\x02 \x03(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x31\n\rcreated_after\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rstarted_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0estarted_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x65nded_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x65nded_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\x9e\x01\n\x04Sort\x12G\n\x05\x66ield\x18\x01 \x01(\x0e\x32\x38.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderByField\x12M\n\tdirection\x18\x02 \x01(\x0e\x32:.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderDirection\"\xdf\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1a\n\x16ORDER_BY_FIELD_TASK_ID\x10\x01\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x02\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x03\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x04\x12\x1d\n\x19ORDER_BY_FIELD_STARTED_AT\x10\x05\x12\x1b\n\x17ORDER_BY_FIELD_ENDED_AT\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"z\n\x11ListTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"y\n\x14ListTasksRawResponse\x12\x31\n\x05tasks\x18\x01 \x03(\x0b\x32\".armonik.api.grpc.v1.tasks.TaskRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"!\n\x0eGetTaskRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\t\"C\n\x0fGetTaskResponse\x12\x30\n\x04task\x18\x01 \x01(\x0b\x32\".armonik.api.grpc.v1.tasks.TaskRaw\"&\n\x12\x43\x61ncelTasksRequest\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"L\n\x13\x43\x61ncelTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\"&\n\x13GetResultIdsRequest\x12\x0f\n\x07task_id\x18\x01 \x03(\t\"\xa1\x01\n\x14GetResultIdsResponse\x12S\n\x0ctask_results\x18\x01 \x03(\x0b\x32=.armonik.api.grpc.v1.tasks.GetResultIdsResponse.MapTaskResult\x1a\x34\n\rMapTaskResult\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x12\n\nresult_ids\x18\x02 \x03(\t\"\x1b\n\x19\x43ountTasksByStatusRequest\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCount\"\xca\x02\n\x12SubmitTasksRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12R\n\x0etask_creations\x18\x03 \x03(\x0b\x32:.armonik.api.grpc.v1.tasks.SubmitTasksRequest.TaskCreation\x1a\x93\x01\n\x0cTaskCreation\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\x12\x12\n\npayload_id\x18\x03 \x01(\t\x12\x36\n\x0ctask_options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\"\xcb\x01\n\x13SubmitTasksResponse\x12K\n\ntask_infos\x18\x01 \x03(\x0b\x32\x37.armonik.api.grpc.v1.tasks.SubmitTasksResponse.TaskInfo\x1ag\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x02 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x03 \x03(\t\x12\x12\n\npayload_id\x18\x04 \x01(\tB\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Tasksb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tasks_common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\031ArmoniK.Api.gRPC.V1.Tasks'
@@ -38,26 +38,36 @@
   _LISTTASKSREQUEST_SORT._serialized_end=1959
   _LISTTASKSREQUEST_ORDERBYFIELD._serialized_start=1962
   _LISTTASKSREQUEST_ORDERBYFIELD._serialized_end=2185
   _LISTTASKSREQUEST_ORDERDIRECTION._serialized_start=2187
   _LISTTASKSREQUEST_ORDERDIRECTION._serialized_end=2287
   _LISTTASKSRESPONSE._serialized_start=2289
   _LISTTASKSRESPONSE._serialized_end=2411
-  _GETTASKREQUEST._serialized_start=2413
-  _GETTASKREQUEST._serialized_end=2446
-  _GETTASKRESPONSE._serialized_start=2448
-  _GETTASKRESPONSE._serialized_end=2515
-  _CANCELTASKSREQUEST._serialized_start=2517
-  _CANCELTASKSREQUEST._serialized_end=2555
-  _CANCELTASKSRESPONSE._serialized_start=2557
-  _CANCELTASKSRESPONSE._serialized_end=2633
-  _GETRESULTIDSREQUEST._serialized_start=2635
-  _GETRESULTIDSREQUEST._serialized_end=2673
-  _GETRESULTIDSRESPONSE._serialized_start=2676
-  _GETRESULTIDSRESPONSE._serialized_end=2837
-  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_start=2785
-  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_end=2837
-  _COUNTTASKSBYSTATUSREQUEST._serialized_start=2839
-  _COUNTTASKSBYSTATUSREQUEST._serialized_end=2866
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=2868
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=2946
+  _LISTTASKSRAWRESPONSE._serialized_start=2413
+  _LISTTASKSRAWRESPONSE._serialized_end=2534
+  _GETTASKREQUEST._serialized_start=2536
+  _GETTASKREQUEST._serialized_end=2569
+  _GETTASKRESPONSE._serialized_start=2571
+  _GETTASKRESPONSE._serialized_end=2638
+  _CANCELTASKSREQUEST._serialized_start=2640
+  _CANCELTASKSREQUEST._serialized_end=2678
+  _CANCELTASKSRESPONSE._serialized_start=2680
+  _CANCELTASKSRESPONSE._serialized_end=2756
+  _GETRESULTIDSREQUEST._serialized_start=2758
+  _GETRESULTIDSREQUEST._serialized_end=2796
+  _GETRESULTIDSRESPONSE._serialized_start=2799
+  _GETRESULTIDSRESPONSE._serialized_end=2960
+  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_start=2908
+  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_end=2960
+  _COUNTTASKSBYSTATUSREQUEST._serialized_start=2962
+  _COUNTTASKSBYSTATUSREQUEST._serialized_end=2989
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=2991
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=3069
+  _SUBMITTASKSREQUEST._serialized_start=3072
+  _SUBMITTASKSREQUEST._serialized_end=3402
+  _SUBMITTASKSREQUEST_TASKCREATION._serialized_start=3255
+  _SUBMITTASKSREQUEST_TASKCREATION._serialized_end=3402
+  _SUBMITTASKSRESPONSE._serialized_start=3405
+  _SUBMITTASKSRESPONSE._serialized_end=3608
+  _SUBMITTASKSRESPONSE_TASKINFO._serialized_start=3505
+  _SUBMITTASKSRESPONSE_TASKINFO._serialized_end=3608
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/tasks_common_pb2.pyi` & `armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -58,14 +58,26 @@
 
 class GetTaskResponse(_message.Message):
     __slots__ = ["task"]
     TASK_FIELD_NUMBER: _ClassVar[int]
     task: TaskRaw
     def __init__(self, task: _Optional[_Union[TaskRaw, _Mapping]] = ...) -> None: ...
 
+class ListTasksRawResponse(_message.Message):
+    __slots__ = ["page", "page_size", "tasks", "total"]
+    PAGE_FIELD_NUMBER: _ClassVar[int]
+    PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
+    TASKS_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    page: int
+    page_size: int
+    tasks: _containers.RepeatedCompositeFieldContainer[TaskRaw]
+    total: int
+    def __init__(self, tasks: _Optional[_Iterable[_Union[TaskRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
+
 class ListTasksRequest(_message.Message):
     __slots__ = ["filter", "page", "page_size", "sort", "with_errors"]
     class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class Filter(_message.Message):
@@ -124,14 +136,52 @@
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     page: int
     page_size: int
     tasks: _containers.RepeatedCompositeFieldContainer[TaskSummary]
     total: int
     def __init__(self, tasks: _Optional[_Iterable[_Union[TaskSummary, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
+class SubmitTasksRequest(_message.Message):
+    __slots__ = ["session_id", "task_creations", "task_options"]
+    class TaskCreation(_message.Message):
+        __slots__ = ["data_dependencies", "expected_output_keys", "payload_id", "task_options"]
+        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+        EXPECTED_OUTPUT_KEYS_FIELD_NUMBER: _ClassVar[int]
+        PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
+        TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+        expected_output_keys: _containers.RepeatedScalarFieldContainer[str]
+        payload_id: str
+        task_options: _objects_pb2.TaskOptions
+        def __init__(self, expected_output_keys: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    TASK_CREATIONS_FIELD_NUMBER: _ClassVar[int]
+    TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    session_id: str
+    task_creations: _containers.RepeatedCompositeFieldContainer[SubmitTasksRequest.TaskCreation]
+    task_options: _objects_pb2.TaskOptions
+    def __init__(self, session_id: _Optional[str] = ..., task_options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., task_creations: _Optional[_Iterable[_Union[SubmitTasksRequest.TaskCreation, _Mapping]]] = ...) -> None: ...
+
+class SubmitTasksResponse(_message.Message):
+    __slots__ = ["task_infos"]
+    class TaskInfo(_message.Message):
+        __slots__ = ["data_dependencies", "expected_output_ids", "payload_id", "task_id"]
+        DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
+        EXPECTED_OUTPUT_IDS_FIELD_NUMBER: _ClassVar[int]
+        PAYLOAD_ID_FIELD_NUMBER: _ClassVar[int]
+        TASK_ID_FIELD_NUMBER: _ClassVar[int]
+        data_dependencies: _containers.RepeatedScalarFieldContainer[str]
+        expected_output_ids: _containers.RepeatedScalarFieldContainer[str]
+        payload_id: str
+        task_id: str
+        def __init__(self, task_id: _Optional[str] = ..., expected_output_ids: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
+    TASK_INFOS_FIELD_NUMBER: _ClassVar[int]
+    task_infos: _containers.RepeatedCompositeFieldContainer[SubmitTasksResponse.TaskInfo]
+    def __init__(self, task_infos: _Optional[_Iterable[_Union[SubmitTasksResponse.TaskInfo, _Mapping]]] = ...) -> None: ...
+
 class TaskRaw(_message.Message):
     __slots__ = ["acquired_at", "created_at", "data_dependencies", "ended_at", "expected_output_ids", "id", "options", "output", "owner_pod_id", "parent_task_ids", "pod_hostname", "pod_ttl", "received_at", "retry_of_ids", "session_id", "started_at", "status", "status_message", "submitted_at"]
     class Output(_message.Message):
         __slots__ = ["error", "success"]
         ERROR_FIELD_NUMBER: _ClassVar[int]
         SUCCESS_FIELD_NUMBER: _ClassVar[int]
         error: str
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/common/worker_common_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/worker/agent_service_pb2.py` & `armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from ..common import agent_common_pb2 as agent__common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61gent_service.proto\x12\x19\x61rmonik.api.grpc.v1.agent\x1a\x12\x61gent_common.proto2\xf1\x03\n\x05\x41gent\x12h\n\nCreateTask\x12,.armonik.api.grpc.v1.agent.CreateTaskRequest\x1a*.armonik.api.grpc.v1.agent.CreateTaskReply(\x01\x12\x61\n\x0fGetResourceData\x12&.armonik.api.grpc.v1.agent.DataRequest\x1a$.armonik.api.grpc.v1.agent.DataReply0\x01\x12_\n\rGetCommonData\x12&.armonik.api.grpc.v1.agent.DataRequest\x1a$.armonik.api.grpc.v1.agent.DataReply0\x01\x12_\n\rGetDirectData\x12&.armonik.api.grpc.v1.agent.DataRequest\x1a$.armonik.api.grpc.v1.agent.DataReply0\x01\x12Y\n\nSendResult\x12!.armonik.api.grpc.v1.agent.Result\x1a&.armonik.api.grpc.v1.agent.ResultReply(\x01\x42\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Agentb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61gent_service.proto\x12\x19\x61rmonik.api.grpc.v1.agent\x1a\x12\x61gent_common.proto2\xe7\x07\n\x05\x41gent\x12\x8c\x01\n\x15\x43reateResultsMetaData\x12\x37.armonik.api.grpc.v1.agent.CreateResultsMetaDataRequest\x1a\x38.armonik.api.grpc.v1.agent.CreateResultsMetaDataResponse\"\x00\x12t\n\rCreateResults\x12/.armonik.api.grpc.v1.agent.CreateResultsRequest\x1a\x30.armonik.api.grpc.v1.agent.CreateResultsResponse\"\x00\x12\x7f\n\x10UploadResultData\x12\x32.armonik.api.grpc.v1.agent.UploadResultDataRequest\x1a\x33.armonik.api.grpc.v1.agent.UploadResultDataResponse\"\x00(\x01\x12n\n\x0bSubmitTasks\x12-.armonik.api.grpc.v1.agent.SubmitTasksRequest\x1a..armonik.api.grpc.v1.agent.SubmitTasksResponse\"\x00\x12h\n\nCreateTask\x12,.armonik.api.grpc.v1.agent.CreateTaskRequest\x1a*.armonik.api.grpc.v1.agent.CreateTaskReply(\x01\x12\x61\n\x0fGetResourceData\x12&.armonik.api.grpc.v1.agent.DataRequest\x1a$.armonik.api.grpc.v1.agent.DataReply0\x01\x12_\n\rGetCommonData\x12&.armonik.api.grpc.v1.agent.DataRequest\x1a$.armonik.api.grpc.v1.agent.DataReply0\x01\x12_\n\rGetDirectData\x12&.armonik.api.grpc.v1.agent.DataRequest\x1a$.armonik.api.grpc.v1.agent.DataReply0\x01\x12Y\n\nSendResult\x12!.armonik.api.grpc.v1.agent.Result\x1a&.armonik.api.grpc.v1.agent.ResultReply(\x01\x42\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Agentb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'agent_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\031ArmoniK.Api.gRPC.V1.Agent'
   _AGENT._serialized_start=71
-  _AGENT._serialized_end=568
+  _AGENT._serialized_end=1070
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev302/src/armonik/protogen/worker/agent_service_pb2_grpc.py` & `armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2_grpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,34 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
+        self.CreateResultsMetaData = channel.unary_unary(
+                '/armonik.api.grpc.v1.agent.Agent/CreateResultsMetaData',
+                request_serializer=agent__common__pb2.CreateResultsMetaDataRequest.SerializeToString,
+                response_deserializer=agent__common__pb2.CreateResultsMetaDataResponse.FromString,
+                )
+        self.CreateResults = channel.unary_unary(
+                '/armonik.api.grpc.v1.agent.Agent/CreateResults',
+                request_serializer=agent__common__pb2.CreateResultsRequest.SerializeToString,
+                response_deserializer=agent__common__pb2.CreateResultsResponse.FromString,
+                )
+        self.UploadResultData = channel.stream_unary(
+                '/armonik.api.grpc.v1.agent.Agent/UploadResultData',
+                request_serializer=agent__common__pb2.UploadResultDataRequest.SerializeToString,
+                response_deserializer=agent__common__pb2.UploadResultDataResponse.FromString,
+                )
+        self.SubmitTasks = channel.unary_unary(
+                '/armonik.api.grpc.v1.agent.Agent/SubmitTasks',
+                request_serializer=agent__common__pb2.SubmitTasksRequest.SerializeToString,
+                response_deserializer=agent__common__pb2.SubmitTasksResponse.FromString,
+                )
         self.CreateTask = channel.stream_unary(
                 '/armonik.api.grpc.v1.agent.Agent/CreateTask',
                 request_serializer=agent__common__pb2.CreateTaskRequest.SerializeToString,
                 response_deserializer=agent__common__pb2.CreateTaskReply.FromString,
                 )
         self.GetResourceData = channel.unary_stream(
                 '/armonik.api.grpc.v1.agent.Agent/GetResourceData',
@@ -40,14 +60,47 @@
                 response_deserializer=agent__common__pb2.ResultReply.FromString,
                 )
 
 
 class AgentServicer(object):
     """Missing associated documentation comment in .proto file."""
 
+    def CreateResultsMetaData(self, request, context):
+        """*
+        Create the metadata of multiple results at once
+        Data have to be uploaded separately
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def CreateResults(self, request, context):
+        """*
+        Create one result with data included in the request
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UploadResultData(self, request_iterator, context):
+        """*
+        Upload data for result with stream
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SubmitTasks(self, request, context):
+        """*
+        Create tasks metadata and submit task for processing.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def CreateTask(self, request_iterator, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetResourceData(self, request, context):
@@ -73,14 +126,34 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_AgentServicer_to_server(servicer, server):
     rpc_method_handlers = {
+            'CreateResultsMetaData': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateResultsMetaData,
+                    request_deserializer=agent__common__pb2.CreateResultsMetaDataRequest.FromString,
+                    response_serializer=agent__common__pb2.CreateResultsMetaDataResponse.SerializeToString,
+            ),
+            'CreateResults': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateResults,
+                    request_deserializer=agent__common__pb2.CreateResultsRequest.FromString,
+                    response_serializer=agent__common__pb2.CreateResultsResponse.SerializeToString,
+            ),
+            'UploadResultData': grpc.stream_unary_rpc_method_handler(
+                    servicer.UploadResultData,
+                    request_deserializer=agent__common__pb2.UploadResultDataRequest.FromString,
+                    response_serializer=agent__common__pb2.UploadResultDataResponse.SerializeToString,
+            ),
+            'SubmitTasks': grpc.unary_unary_rpc_method_handler(
+                    servicer.SubmitTasks,
+                    request_deserializer=agent__common__pb2.SubmitTasksRequest.FromString,
+                    response_serializer=agent__common__pb2.SubmitTasksResponse.SerializeToString,
+            ),
             'CreateTask': grpc.stream_unary_rpc_method_handler(
                     servicer.CreateTask,
                     request_deserializer=agent__common__pb2.CreateTaskRequest.FromString,
                     response_serializer=agent__common__pb2.CreateTaskReply.SerializeToString,
             ),
             'GetResourceData': grpc.unary_stream_rpc_method_handler(
                     servicer.GetResourceData,
@@ -109,14 +182,82 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class Agent(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
+    def CreateResultsMetaData(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.agent.Agent/CreateResultsMetaData',
+            agent__common__pb2.CreateResultsMetaDataRequest.SerializeToString,
+            agent__common__pb2.CreateResultsMetaDataResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateResults(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.agent.Agent/CreateResults',
+            agent__common__pb2.CreateResultsRequest.SerializeToString,
+            agent__common__pb2.CreateResultsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UploadResultData(request_iterator,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.stream_unary(request_iterator, target, '/armonik.api.grpc.v1.agent.Agent/UploadResultData',
+            agent__common__pb2.UploadResultDataRequest.SerializeToString,
+            agent__common__pb2.UploadResultDataResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SubmitTasks(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/armonik.api.grpc.v1.agent.Agent/SubmitTasks',
+            agent__common__pb2.SubmitTasksRequest.SerializeToString,
+            agent__common__pb2.SubmitTasksResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def CreateTask(request_iterator,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `armonik-3.8.2.dev302/src/armonik/worker/seqlogger.py` & `armonik-3.8.2.dev306/src/armonik/worker/seqlogger.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/worker/taskhandler.py` & `armonik-3.8.2.dev306/src/armonik/worker/taskhandler.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik/worker/worker.py` & `armonik-3.8.2.dev306/src/armonik/worker/worker.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev302/src/armonik.egg-info/PKG-INFO` & `armonik-3.8.2.dev306/src/armonik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev302
+Version: 3.8.2.dev306
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev302/src/armonik.egg-info/SOURCES.txt` & `armonik-3.8.2.dev306/src/armonik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

