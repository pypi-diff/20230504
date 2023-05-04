# Comparing `tmp/dagster_cloud-1.3.2.tar.gz` & `tmp/dagster_cloud-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.3.2.tar", last modified: Thu Apr 27 19:41:46 2023, max compression
+gzip compressed data, was "dagster_cloud-1.3.3.tar", last modified: Thu May  4 17:55:39 2023, max compression
```

## Comparing `dagster_cloud-1.3.2.tar` & `dagster_cloud-1.3.3.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.725780 dagster_cloud-1.3.2/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-04-27 19:41:46.725780 dagster_cloud-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.333778 dagster_cloud-1.3.2/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      140 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.397779 dagster_cloud-1.3.2/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.401779 dagster_cloud-1.3.2/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43090 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.405779 dagster_cloud-1.3.2/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16985 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.409779 dagster_cloud-1.3.2/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.409779 dagster_cloud-1.3.2/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.413779 dagster_cloud-1.3.2/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.413779 dagster_cloud-1.3.2/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14189 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.469779 dagster_cloud-1.3.2/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.469779 dagster_cloud-1.3.2/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18148 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.473779 dagster_cloud-1.3.2/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.477779 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.481779 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-27 18:31:35.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4541 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.489779 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.489779 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10312 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9912 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    11492 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.489779 dagster_cloud-1.3.2/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.493779 dagster_cloud-1.3.2/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.497779 dagster_cloud-1.3.2/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.549779 dagster_cloud-1.3.2/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4582 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.569779 dagster_cloud-1.3.2/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9532 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    26776 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.629779 dagster_cloud-1.3.2/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19107 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.629779 dagster_cloud-1.3.2/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     6552 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.629779 dagster_cloud-1.3.2/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.633780 dagster_cloud-1.3.2/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.637780 dagster_cloud-1.3.2/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6948 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.641780 dagster_cloud-1.3.2/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     4972 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.641780 dagster_cloud-1.3.2/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12011 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.709780 dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22459 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    20446 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.713780 dagster_cloud-1.3.2/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17127 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.725780 dagster_cloud-1.3.2/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    74040 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:41:46.389779 dagster_cloud-1.3.2/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-04-27 19:41:46.000000 dagster_cloud-1.3.2/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-04-27 19:41:46.000000 dagster_cloud-1.3.2/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:41:46.000000 dagster_cloud-1.3.2/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-27 19:41:46.000000 dagster_cloud-1.3.2/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-27 19:41:46.000000 dagster_cloud-1.3.2/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 19:41:46.725780 dagster_cloud-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2890 2023-04-27 18:31:36.000000 dagster_cloud-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.285870 dagster_cloud-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-05-04 17:55:39.285870 dagster_cloud-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.233870 dagster_cloud-1.3.3/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.237870 dagster_cloud-1.3.3/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.237870 dagster_cloud-1.3.3/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43075 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.241870 dagster_cloud-1.3.3/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16984 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.241870 dagster_cloud-1.3.3/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.241870 dagster_cloud-1.3.3/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.245870 dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.245870 dagster_cloud-1.3.3/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14188 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.245870 dagster_cloud-1.3.3/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.245870 dagster_cloud-1.3.3/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    18147 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.249870 dagster_cloud-1.3.3/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.249870 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.253870 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4541 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.253870 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.257870 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9912 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    11492 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.257870 dagster_cloud-1.3.3/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.257870 dagster_cloud-1.3.3/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.257870 dagster_cloud-1.3.3/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.261870 dagster_cloud-1.3.3/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.261870 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9532 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    26757 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.265870 dagster_cloud-1.3.3/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19041 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.269870 dagster_cloud-1.3.3/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.269870 dagster_cloud-1.3.3/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.269870 dagster_cloud-1.3.3/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.269870 dagster_cloud-1.3.3/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.273870 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.273870 dagster_cloud-1.3.3/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12011 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.277870 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22459 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.281870 dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17127 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.285870 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    74040 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:39.237870 dagster_cloud-1.3.3/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-04 17:55:39.000000 dagster_cloud-1.3.3/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 17:55:39.285870 dagster_cloud-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-05-04 17:42:29.000000 dagster_cloud-1.3.3/setup.py
```

### Comparing `dagster_cloud-1.3.2/PKG-INFO` & `dagster_cloud-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.3.2
+Version: 1.3.3
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.2/README.md` & `dagster_cloud-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.3.3/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.3.3/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,15 +541,15 @@
     ) -> Optional[CodeLocationOrigin]:
         """Derive the location from the specific argument passed in to a dagster_cloud_api call."""
         api_name = request.request_api
         if api_name in {
             DagsterCloudApi.GET_EXTERNAL_EXECUTION_PLAN,
             DagsterCloudApi.GET_SUBSET_EXTERNAL_PIPELINE_RESULT,
         }:
-            external_pipeline_origin = request.request_args.pipeline_origin
+            external_pipeline_origin = request.request_args.job_origin
             return external_pipeline_origin.external_repository_origin.code_location_origin
         elif api_name in {
             DagsterCloudApi.GET_EXTERNAL_PARTITION_CONFIG,
             DagsterCloudApi.GET_EXTERNAL_PARTITION_TAGS,
             DagsterCloudApi.GET_EXTERNAL_PARTITION_NAMES,
             DagsterCloudApi.GET_EXTERNAL_PARTITION_SET_EXECUTION_PARAM_DATA,
             DagsterCloudApi.GET_EXTERNAL_SCHEDULE_EXECUTION_DATA,
@@ -707,15 +707,15 @@
                         f"Launching {run.run_id} without an isolated run environment.",
                         run,
                         cls=self.__class__,
                     )
 
                     run_location_name = cast(
                         str,
-                        run.external_pipeline_origin.external_repository_origin.code_location_origin.location_name,
+                        run.external_job_origin.external_repository_origin.code_location_origin.location_name,
                     )
 
                     server = user_code_launcher.get_grpc_server(deployment_name, run_location_name)
 
                     # Record the server handle that we launched it on to for run monitoring
                     scoped_instance.add_run_tags(
                         run.run_id, new_tags={SERVER_HANDLE_TAG: str(server.server_handle)}
@@ -751,15 +751,15 @@
                     )
                     if is_isolated_run(run):
                         launcher = scoped_instance.get_run_launcher_for_run(run)  # type: ignore  # (instance subclass)
                         launcher.terminate(run.run_id)
                     else:
                         run_location_name = cast(
                             str,
-                            run.external_pipeline_origin.external_repository_origin.code_location_origin.location_name,
+                            run.external_job_origin.external_repository_origin.code_location_origin.location_name,
                         )
 
                         server = user_code_launcher.get_grpc_server(
                             deployment_name, run_location_name
                         )
                         client = server.server_endpoint.create_client()
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud/agent/queries.py` & `dagster_cloud-1.3.3/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.3.3/dagster_cloud/api/dagster_cloud_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pendulum
 from dagster._core.code_pointer import CodePointer
 from dagster._core.definitions.selector import JobSelector
 from dagster._core.host_representation import (
     CodeLocationOrigin,
     ExternalRepositoryData,
 )
-from dagster._core.storage.pipeline_run import DagsterRun
+from dagster._core.storage.dagster_run import DagsterRun
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo
 from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
 
 from dagster_cloud.execution.monitoring import CloudCodeServerHeartbeat, CloudRunWorkerStatuses
 
 DEFAULT_EXPIRATION_MILLISECONDS = 10 * 60 * 1000
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud/auth/constants.py` & `dagster_cloud-1.3.3/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster_cloud-1.3.3/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,31 +17,31 @@
 class CloudProcessRunLauncher(RunLauncher):
     def __init__(self):
         self._run_ids = set()
         super().__init__()
 
     def launch_run(self, context: LaunchRunContext) -> None:
         run = context.dagster_run
-        pipeline_code_origin = check.not_none(context.pipeline_code_origin)
+        pipeline_code_origin = check.not_none(context.job_code_origin)
 
         run_args = ExecuteRunArgs(
-            pipeline_origin=pipeline_code_origin,
-            pipeline_run_id=run.run_id,
+            job_origin=pipeline_code_origin,
+            run_id=run.run_id,
             instance_ref=self._instance.get_ref(),
         )
         args = run_args.get_command_args()
 
         kwargs = {}
         if (
-            run.pipeline_code_origin
-            and run.pipeline_code_origin.repository_origin.container_context
-            and run.pipeline_code_origin.repository_origin.container_context.get("env_vars")
+            run.job_code_origin
+            and run.job_code_origin.repository_origin.container_context
+            and run.job_code_origin.repository_origin.container_context.get("env_vars")
         ):
             kwargs["env"] = {**os.environ}
-            for kev in run.pipeline_code_origin.repository_origin.container_context["env_vars"]:
+            for kev in run.job_code_origin.repository_origin.container_context["env_vars"]:
                 key, value = parse_env_var(kev)
                 kwargs["env"][key] = value
 
         p = open_ipc_subprocess(args, **kwargs)
         pid = p.pid
 
         self._run_ids.add(run.run_id)
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.3.3/dagster_cloud/execution/monitoring/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from enum import Enum
 from typing import Dict, Iterable, List, Mapping, NamedTuple, Optional, Sequence, Set, Tuple, Union
 
 import dagster._check as check
 import grpc
 from dagster import DagsterInstance, DagsterRunStatus
 from dagster._core.launcher import CheckRunHealthResult, WorkerStatus
-from dagster._core.storage.pipeline_run import IN_PROGRESS_RUN_STATUSES, RunsFilter
+from dagster._core.storage.dagster_run import IN_PROGRESS_RUN_STATUSES, RunsFilter
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
 from dagster_cloud.instance import DagsterCloudAgentInstance
 from dagster_cloud.util import SERVER_HANDLE_TAG, is_isolated_run
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.3.3/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.3.3/dagster_cloud/instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 from dagster._config import process_config
 from dagster._core.errors import DagsterInvalidConfigError, DagsterInvariantViolationError
 from dagster._core.instance import DagsterInstance
 from dagster._core.instance.config import config_field_for_configurable_class
 from dagster._core.instance.ref import InstanceRef, configurable_class_data
 from dagster._core.launcher import DefaultRunLauncher, RunLauncher
-from dagster._core.storage.pipeline_run import DagsterRun
+from dagster._core.storage.dagster_run import DagsterRun
 from dagster._serdes import ConfigurableClassData
 from dagster_cloud_cli.core.graphql_client import (
     create_graphql_requests_session,
     create_proxy_client,
     get_agent_headers,
 )
 from dagster_cloud_cli.core.headers.auth import DagsterCloudInstanceScope
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.3.3/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.3.3/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.3.3/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/storage/client.py` & `dagster_cloud-1.3.3/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.3.3/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 import dagster._check as check
 from dagster._core.assets import AssetDetails
 from dagster._core.definitions.events import AssetKey, ExpectationResult
 from dagster._core.event_api import EventLogRecord, EventRecordsFilter, RunShardedEventsCursor
 from dagster._core.events import DagsterEvent, DagsterEventType
 from dagster._core.events.log import EventLogEntry
 from dagster._core.execution.stats import RunStepKeyStatsSnapshot, RunStepMarker, StepEventStatus
+from dagster._core.storage.dagster_run import DagsterRunStatsSnapshot
 from dagster._core.storage.event_log.base import (
     AssetEntry,
     AssetRecord,
     EventLogConnection,
     EventLogStorage,
 )
 from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
-from dagster._core.storage.pipeline_run import PipelineRunStatsSnapshot
 from dagster._serdes import (
     ConfigurableClass,
     ConfigurableClassData,
     serialize_value,
 )
 from dagster._serdes.serdes import deserialize_value
 from dagster._utils import datetime_as_float
@@ -92,15 +92,15 @@
 
 def _input_for_dagster_event(dagster_event: Optional[DagsterEvent]):
     if dagster_event is None:
         return None
 
     return {
         "eventTypeValue": dagster_event.event_type_value,
-        "pipelineName": dagster_event.pipeline_name,
+        "pipelineName": dagster_event.job_name,
         "stepHandleKey": dagster_event.step_handle.to_key() if dagster_event.step_handle else None,
         "solidHandleId": (
             dagster_event.node_handle.to_string() if dagster_event.node_handle else None
         ),
         "stepKindValue": dagster_event.step_kind_value,
         "loggingTags": (
             json.dumps(dagster_event.logging_tags) if dagster_event.logging_tags else None
@@ -128,15 +128,15 @@
             else None
         ),
         level=check.int_elem(graphene_event_log_entry, "level"),
         user_message=check.str_elem(graphene_event_log_entry, "userMessage"),
         run_id=check.str_elem(graphene_event_log_entry, "runId"),
         timestamp=check.float_elem(graphene_event_log_entry, "timestamp"),
         step_key=check.opt_str_elem(graphene_event_log_entry, "stepKey"),
-        pipeline_name=check.opt_str_elem(graphene_event_log_entry, "pipelineName"),
+        job_name=check.opt_str_elem(graphene_event_log_entry, "pipelineName"),
         dagster_event=(
             deserialize_value(
                 check.str_elem(graphene_event_log_entry, "dagsterEvent"),
                 DagsterEvent,
             )
             if graphene_event_log_entry.get("dagsterEvent") is not None
             else None
@@ -313,20 +313,20 @@
         connection_data = res["data"]["eventLogs"]["getRecordsForRun"]
         return EventLogConnection(
             records=[_event_record_from_graphql(record) for record in connection_data["records"]],
             cursor=connection_data["cursor"],
             has_more=connection_data["hasMore"],
         )
 
-    def get_stats_for_run(self, run_id: str) -> PipelineRunStatsSnapshot:
+    def get_stats_for_run(self, run_id: str) -> DagsterRunStatsSnapshot:
         res = self._execute_query(
             GET_STATS_FOR_RUN_QUERY, variables={"runId": check.str_param(run_id, "run_id")}
         )
         stats = res["data"]["eventLogs"]["getStatsForRun"]
-        return PipelineRunStatsSnapshot(
+        return DagsterRunStatsSnapshot(
             run_id=check.str_elem(stats, "runId"),
             steps_succeeded=check.int_elem(stats, "stepsSucceeded"),
             steps_failed=check.int_elem(stats, "stepsFailed"),
             materializations=check.int_elem(stats, "materializations"),
             expectations=check.int_elem(stats, "expectations"),
             enqueued_time=check.opt_float_elem(stats, "enqueuedTime"),
             launch_time=check.opt_float_elem(stats, "launchTime"),
@@ -397,15 +397,15 @@
                 "eventRecord": {
                     "errorInfo": _input_for_serializable_error_info(event.error_info),
                     "level": event.level,
                     "userMessage": event.user_message,
                     "runId": event.run_id,
                     "timestamp": event.timestamp,
                     "stepKey": event.step_key,
-                    "pipelineName": event.pipeline_name,
+                    "pipelineName": event.job_name,
                     "dagsterEvent": _input_for_dagster_event(event.dagster_event),
                 }
             },
             headers=headers,
         )
 
     def delete_events(self, run_id: str):
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.3.3/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.3.3/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.3.3/dagster_cloud/storage/runs/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,22 @@
     DagsterInvariantViolationError,
     DagsterRunAlreadyExists,
     DagsterRunNotFoundError,
     DagsterSnapshotDoesNotExist,
 )
 from dagster._core.events import DagsterEvent
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
-from dagster._core.host_representation.origin import ExternalPipelineOrigin
+from dagster._core.host_representation.origin import ExternalJobOrigin
 from dagster._core.snap import (
     ExecutionPlanSnapshot,
-    PipelineSnapshot,
+    JobSnapshot,
     create_execution_plan_snapshot_id,
-    create_pipeline_snapshot_id,
+    create_job_snapshot_id,
 )
-from dagster._core.storage.pipeline_run import (
+from dagster._core.storage.dagster_run import (
     DagsterRun,
     JobBucket,
     RunPartitionData,
     RunRecord,
     RunsFilter,
     TagBucket,
 )
@@ -82,15 +82,15 @@
 def _get_filters_input(filters: Optional[RunsFilter]) -> Optional[Dict[str, Any]]:
     filters = check.opt_inst_param(filters, "filters", RunsFilter)
 
     if filters is None:
         return None
     return {
         "runIds": filters.run_ids,
-        "pipelineName": filters.pipeline_name,
+        "pipelineName": filters.job_name,
         "statuses": [status.value for status in filters.statuses],
         "tags": [
             merge_dicts(
                 {"key": tag_key},
                 ({"value": tag_value} if isinstance(tag_value, str) else {"values": tag_value}),
             )
             for tag_key, tag_value in filters.tags.items()
@@ -341,45 +341,45 @@
 
     def has_run(self, run_id: str) -> bool:
         res = self._execute_query(
             HAS_RUN_QUERY, variables={"runId": check.str_param(run_id, "run_id")}
         )
         return res["data"]["runs"]["hasRun"]
 
-    def has_pipeline_snapshot(self, pipeline_snapshot_id: str) -> bool:
+    def has_job_snapshot(self, pipeline_snapshot_id: str) -> bool:
         res = self._execute_query(
             HAS_PIPELINE_SNAPSHOT_QUERY,
             variables={
                 "pipelineSnapshotId": check.str_param(pipeline_snapshot_id, "pipeline_snapshot_id")
             },
         )
         return res["data"]["runs"]["hasPipelineSnapshot"]
 
-    def add_pipeline_snapshot(
-        self, pipeline_snapshot: PipelineSnapshot, snapshot_id: Optional[str] = None
+    def add_job_snapshot(
+        self, pipeline_snapshot: JobSnapshot, snapshot_id: Optional[str] = None
     ) -> str:
         self._execute_query(
             ADD_PIPELINE_SNAPSHOT_MUTATION,
             variables={
                 "serializedPipelineSnapshot": serialize_value(
-                    check.inst_param(pipeline_snapshot, "pipeline_snapshot", PipelineSnapshot)
+                    check.inst_param(pipeline_snapshot, "pipeline_snapshot", JobSnapshot)
                 ),
                 "snapshotId": snapshot_id,
             },
         )
-        return snapshot_id if snapshot_id else create_pipeline_snapshot_id(pipeline_snapshot)
+        return snapshot_id if snapshot_id else create_job_snapshot_id(pipeline_snapshot)
 
-    def get_pipeline_snapshot(self, pipeline_snapshot_id: str) -> PipelineSnapshot:
+    def get_job_snapshot(self, pipeline_snapshot_id: str) -> JobSnapshot:
         res = self._execute_query(
             GET_PIPELINE_SNAPSHOT_QUERY,
             variables={
                 "pipelineSnapshotId": check.str_param(pipeline_snapshot_id, "pipeline_snapshot_id")
             },
         )
-        return deserialize_value(res["data"]["runs"]["getPipelineSnapshot"], PipelineSnapshot)
+        return deserialize_value(res["data"]["runs"]["getPipelineSnapshot"], JobSnapshot)
 
     def has_execution_plan_snapshot(self, execution_plan_snapshot_id: str) -> bool:
         res = self._execute_query(
             HAS_EXECUTION_PLAN_SNAPSHOT_QUERY,
             variables={
                 "executionPlanSnapshotId": check.str_param(
                     execution_plan_snapshot_id, "execution_plan_snapshot_id"
@@ -510,15 +510,15 @@
     def get_cursor_values(self, keys: Set[str]):
         return NotImplementedError("KVS is not supported from the user cloud")
 
     def set_cursor_values(self, pairs: Mapping[str, str]):
         return NotImplementedError("KVS is not supported from the user cloud")
 
     # Migrating run history
-    def replace_job_origin(self, run: DagsterRun, job_origin: ExternalPipelineOrigin):
+    def replace_job_origin(self, run: DagsterRun, job_origin: ExternalJobOrigin):
         self._execute_query(
             MUTATE_JOB_ORIGIN,
             variables={
                 "runId": run.run_id,
                 "serializedJobOrigin": serialize_value(job_origin),
             },
         )
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.3.3/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.3.3/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/util/__init__.py` & `dagster_cloud-1.3.3/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 
     @property
     def inst_data(self) -> Optional[ConfigurableClassData]:
         return self._inst_data
 
     def _write_liveness_sentinel(self) -> None:
         # Write to a sentinel file to indicate that we've finished our initial
-        # reconciliation - this is used in serverless to indicate that we're ready to
+        # reconciliation - this is used to indicate that we're ready to
         # serve requests
         Path("/opt/finished_initial_reconciliation_sentinel.txt").touch(exist_ok=True)
         self._logger.info(
             "Wrote liveness sentinel: indicating that agent is ready to serve requests"
         )
 
     def _get_grpc_server_sidecars(self) -> Optional[List[Dict[str, Any]]]:
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dagster_cloud.instance import DagsterCloudAgentInstance
 
 from .utils import get_task_definition_family
 
 
 class CloudEcsRunLauncher(EcsRunLauncher[DagsterCloudAgentInstance]):
     def _get_run_task_definition_family(self, run) -> str:
-        pipeline_origin = check.not_none(run.external_pipeline_origin)
+        pipeline_origin = check.not_none(run.external_job_origin)
         location_name = (
             pipeline_origin.external_repository_origin.code_location_origin.location_name
         )
 
         return get_task_definition_family(
             "run", self._instance.organization_name, self._instance.deployment_name, location_name  # type: ignore  # (possible none)
         )
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.3.3/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.3.3/dagster_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.3.2
+Version: 1.3.3
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.2/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.3.3/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.2/setup.py` & `dagster_cloud-1.3.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.2",
-        "dagster-cloud-cli==1.3.2",
+        "dagster==1.3.3",
+        "dagster-cloud-cli==1.3.3",
         "pex",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -58,19 +58,19 @@
             "mypy",
             "paramiko",
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
-            "dagster_k8s==0.19.2",
+            "dagster_k8s==0.19.3",
         ],
-        "docker": ["docker", "dagster_docker==0.19.2"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.19.2"],
-        "ecs": ["dagster_aws==0.19.2", "boto3"],
+        "docker": ["docker", "dagster_docker==0.19.3"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.19.3"],
+        "ecs": ["dagster_aws==0.19.3", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

