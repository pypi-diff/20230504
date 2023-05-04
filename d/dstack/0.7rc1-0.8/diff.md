# Comparing `tmp/dstack-0.7rc1.tar.gz` & `tmp/dstack-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstack-0.7rc1.tar", last modified: Tue Apr 11 14:42:51 2023, max compression
+gzip compressed data, was "dstack-0.8.tar", last modified: Thu May  4 07:20:45 2023, max compression
```

## Comparing `dstack-0.7rc1.tar` & `dstack-0.8.tar`

### file list

```diff
@@ -1,228 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-04-11 14:42:02.000000 dstack-0.7rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-11 14:42:51.143200 dstack-0.7rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-11 14:42:02.000000 dstack-0.7rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/backend/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    18797 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27843 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    23592 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/local/
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/cp/
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/cp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/init/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/logs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/ls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/prune/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/prune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/ps/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/ps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/pull/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/pull/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/push/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/push/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/rm/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/rm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/run/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/stop/
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/stop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/tags/
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/dependents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/userconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/hub/background/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/background/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/background/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/background/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/background/tasks/resubmit_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/db/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/migration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/migration/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/versions/3b900659c822_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/repository/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/repository/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/security/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/security/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/_torchrun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/_torchrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/_torchrun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/bash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/bash/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/code/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/docker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/providers/lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/lab/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/providers/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/notebook/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/random_names.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 14:42:50.000000 dstack-0.7rc1/cli/dstack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/backend/base/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/docker/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/test_local_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/utils/test_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:42:51.143200 dstack-0.7rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-11 14:42:02.000000 dstack-0.7rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.419316 dstack-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-05-04 07:19:59.000000 dstack-0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-04 07:20:45.419316 dstack-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-04 07:19:59.000000 dstack-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.395315 dstack-0.8/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.395315 dstack-0.8/cli/dstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/api/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19382 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/hub/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/api/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/internal/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/api/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/backend/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.399315 dstack-0.8/cli/dstack/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/base/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/backend/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/backend/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/backend/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/cp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/cp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/logs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/ls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/prune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/prune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/ps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/ps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/rm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/rm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/run/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/start/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/start/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/stop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.403315 dstack-0.8/cli/dstack/cli/commands/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/commands/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/cli/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/dependents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/log_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/core/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/repo/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/core/userconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/background/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/background/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/background/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/background/tasks/resubmit_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/db/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/migration/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/migration/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/migration/versions/3b900659c822_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/migration/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.407316 dstack-0.8/cli/dstack/hub/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/repository/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/repository/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/routers/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/security/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/security/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/services/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/services/backends/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/hub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/hub/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    18554 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/_torchrun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/_torchrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/_torchrun/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/bash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/bash/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/code/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/docker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.411316 dstack-0.8/cli/dstack/providers/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/lab/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/dstack/providers/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/providers/notebook/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/dstack/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/dstack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/random_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-04 07:19:59.000000 dstack-0.8/cli/dstack/utils/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 07:20:44.000000 dstack-0.8/cli/dstack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.395315 dstack-0.8/cli/dstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 07:20:45.000000 dstack-0.8/cli/dstack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/backend/base/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/routers/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/routers/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/hub/routers/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/integration/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/integration/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.415316 dstack-0.8/cli/tests/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/providers/docker/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/providers/test_local_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:20:45.419316 dstack-0.8/cli/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/test_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/test_merge_workflow_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 07:19:59.000000 dstack-0.8/cli/tests/utils/test_tarignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:20:45.419316 dstack-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-04 07:19:59.000000 dstack-0.8/setup.py
```

### Comparing `dstack-0.7rc1/LICENSE.md` & `dstack-0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/api/run.py` & `dstack-0.8/cli/dstack/api/runs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,80 +1,49 @@
-from collections import defaultdict
 from typing import List, Optional, Tuple
 
-from dstack.api.repo import load_repo_data
+from dstack.api.hub import HubClient
 from dstack.backend.base import Backend
-from dstack.core.repo import RepoData
 from dstack.core.run import RunHead
 from dstack.core.tag import TagHead
 
 
 class RunNotFoundError(Exception):
     pass
 
 
 class TagNotFoundError(Exception):
     pass
 
 
-def list_runs_with_merged_backends(
-    backends: List[Backend], run_name: str = "", all: bool = False
-) -> List[Tuple[RunHead, List[Backend]]]:
-    runs = list_runs(backends, run_name, all)
-    run_name_to_run_map = {r.run_name: r for r, _ in runs}
-
-    run_name_to_backends_map = defaultdict(list)
-    for run, backend in runs:
-        run_name_to_backends_map[run.run_name].append(backend)
-
-    runs_with_merged_backends = []
-    for run_name in run_name_to_run_map:
-        runs_with_merged_backends.append(
-            (
-                run_name_to_run_map[run_name],
-                list(sorted(run_name_to_backends_map[run_name], key=lambda b: b.name)),
-            )
-        )
-    return runs_with_merged_backends
-
-
-def list_runs(
-    backends: List[Backend], run_name: str = "", all: bool = False
-) -> List[Tuple[RunHead, Backend]]:
-    repo_data = load_repo_data()
-    runs = []
-    for backend in backends:
-        runs += [(run, backend) for run in _get_runs(repo_data, backend, run_name, all)]
-    return list(sorted(runs, key=lambda r: -r[0].submitted_at))
-
-
-def _get_runs(
-    repo_data: RepoData, backend: Backend, run_name: str = "", all: bool = False
-) -> List[RunHead]:
-    runs = []
-    runs_backend = backend.list_run_heads(repo_data, run_name)
-    for run in runs_backend:
-        runs.append(run)
+def list_runs(hub_client: HubClient, run_name: str = "", all: bool = False) -> List[RunHead]:
+    runs = [run for run in _get_runs(hub_client, run_name, all)]
+    return list(sorted(runs, key=lambda r: -r.submitted_at))
+
+
+def _get_runs(hub_client: HubClient, run_name: str = "", all: bool = False) -> List[RunHead]:
+    runs = hub_client.list_run_heads(run_name)
     if not all:
         unfinished = any(run.status.is_unfinished() for run in runs)
         if unfinished:
             runs = list(filter(lambda r: r.status.is_unfinished(), runs))
         else:
             runs = runs[:1]
     return runs
 
 
-def get_tagged_run_name(repo_data, backend, run_name_or_tag_name) -> Tuple[str, Optional[TagHead]]:
+def get_tagged_run_name(
+    hub_client: HubClient, run_name_or_tag_name: str
+) -> Tuple[str, Optional[TagHead]]:
     if run_name_or_tag_name.startswith(":"):
         tag_name = run_name_or_tag_name[1:]
-        tag_head = backend.get_tag_head(repo_data, tag_name)
+        tag_head = hub_client.get_tag_head(tag_name)
         if tag_head is not None:
             return tag_head.run_name, tag_head
         else:
             raise TagNotFoundError()
     else:
         run_name = run_name_or_tag_name
-        job_heads = backend.list_job_heads(repo_data, run_name)
+        job_heads = hub_client.list_job_heads(run_name)
         if job_heads:
             return run_name, None
         else:
             raise RunNotFoundError()
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/aws/__init__.py` & `dstack-0.8/cli/dstack/backend/aws/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,53 @@
-from pathlib import Path
+from datetime import datetime
 from typing import Generator, List, Optional
 
 import boto3
 from botocore.client import BaseClient
 
-from dstack.backend.aws import config, logs
+from dstack.backend.aws import logs
 from dstack.backend.aws.compute import AWSCompute
-from dstack.backend.aws.config import AWSConfig, AWSConfigurator
+from dstack.backend.aws.config import AWSConfig
 from dstack.backend.aws.secrets import AWSSecretsManager
 from dstack.backend.aws.storage import AWSStorage
-from dstack.backend.base import CloudBackend
+from dstack.backend.base import Backend
 from dstack.backend.base import artifacts as base_artifacts
 from dstack.backend.base import cache as base_cache
 from dstack.backend.base import jobs as base_jobs
 from dstack.backend.base import repos as base_repos
 from dstack.backend.base import runs as base_runs
 from dstack.backend.base import secrets as base_secrets
 from dstack.backend.base import tags as base_tags
 from dstack.core.artifact import Artifact
-from dstack.core.error import ConfigError
 from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.log_event import LogEvent
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials, RepoHead
+from dstack.core.repo import RemoteRepoCredentials, RepoHead, RepoSpec
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
+from dstack.utils.common import PathLike
 
 
-class AwsBackend(CloudBackend):
-    _session: Optional[boto3.Session] = None
+class AwsBackend(Backend):
+    NAME = "aws"
     backend_config: AWSConfig
+    _storage: AWSStorage
+    _compute: AWSCompute
+    _secrets_manager: AWSSecretsManager
 
-    @property
-    def name(self):
-        return "aws"
-
-    def __init__(self, backend_config: Optional[AWSConfig] = None):
-        if backend_config is None:
-            self.backend_config = AWSConfig()
-            try:
-                self.backend_config.load()
-                self._loaded = True
-            except ConfigError:
-                self._loaded = False
-                return
-        else:
-            self.backend_config = backend_config
-            self._loaded = True
-
-        if self.backend_config.credentials is not None:
-            self._session = boto3.session.Session(
-                region_name=self.backend_config.region_name,
-                aws_access_key_id=self.backend_config.credentials.get("access_key"),
-                aws_secret_access_key=self.backend_config.credentials.get("secret_key"),
-            )
-
+    def __init__(
+        self,
+        backend_config: AWSConfig,
+    ):
+        super().__init__(backend_config=backend_config)
+        self._session = boto3.session.Session(
+            region_name=self.backend_config.region_name,
+            aws_access_key_id=self.backend_config.credentials.get("access_key"),
+            aws_secret_access_key=self.backend_config.credentials.get("secret_key"),
+        )
         self._storage = AWSStorage(
             s3_client=self._s3_client(), bucket_name=self.backend_config.bucket_name
         )
         self._compute = AWSCompute(
             ec2_client=self._ec2_client(),
             iam_client=self._iam_client(),
             bucket_name=self.backend_config.bucket_name,
@@ -87,217 +76,170 @@
     def _secretsmanager_client(self) -> BaseClient:
         return self._get_client("secretsmanager")
 
     def _sts_client(self) -> BaseClient:
         return self._get_client("sts")
 
     def _get_client(self, client_name: str) -> BaseClient:
-        if self._session is None:
-            self._session = boto3.Session(
-                profile_name=self.backend_config.profile_name,
-                region_name=self.backend_config.region_name,
-            )
         return self._session.client(client_name)
 
-    def configure(self):
-        config.configure(
-            self._ec2_client(),
-            self._iam_client(),
-            self.backend_config.bucket_name,
-            self.backend_config.subnet_id,
+    def create_run(self, repo_id: str) -> str:
+        logs.create_log_groups_if_not_exist(
+            self._logs_client(), self.backend_config.bucket_name, repo_id
         )
-
-    def create_run(self, repo_address: RepoAddress) -> str:
-        logs.create_log_group_if_not_exists(
-            self._logs_client(), self.backend_config.bucket_name, repo_address
-        )
-        return base_runs.create_run(self._storage, repo_address, self.type)
+        return base_runs.create_run(self._storage)
 
     def create_job(self, job: Job):
         base_jobs.create_job(self._storage, job)
 
-    def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
-        return base_jobs.get_job(self._storage, repo_address, job_id)
+    def get_job(self, repo_id: str, job_id: str) -> Optional[Job]:
+        return base_jobs.get_job(self._storage, repo_id, job_id)
 
-    def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
-        return base_jobs.list_jobs(self._storage, repo_address, run_name)
+    def list_jobs(self, repo_id: str, run_name: str) -> List[Job]:
+        return base_jobs.list_jobs(self._storage, repo_id, run_name)
 
     def run_job(self, job: Job, failed_to_start_job_new_status: JobStatus):
         base_jobs.run_job(self._storage, self._compute, job, failed_to_start_job_new_status)
 
-    def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
-        base_jobs.stop_job(self._storage, self._compute, repo_address, job_id, abort)
+    def stop_job(self, repo_id: str, abort: bool, job_id: str):
+        base_jobs.stop_job(self._storage, self._compute, repo_id, job_id, abort)
 
-    def list_job_heads(
-        self, repo_address: RepoAddress, run_name: Optional[str] = None
-    ) -> List[JobHead]:
-        return base_jobs.list_job_heads(self._storage, repo_address, run_name)
+    def list_job_heads(self, repo_id: str, run_name: Optional[str] = None) -> List[JobHead]:
+        return base_jobs.list_job_heads(self._storage, repo_id, run_name)
 
-    def delete_job_head(self, repo_address: RepoAddress, job_id: str):
-        base_jobs.delete_job_head(self._storage, repo_address, job_id)
+    def delete_job_head(self, repo_id: str, job_id: str):
+        base_jobs.delete_job_head(self._storage, repo_id, job_id)
 
     def list_run_heads(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
         interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
-        job_heads = self.list_job_heads(repo_address, run_name)
+        job_heads = self.list_job_heads(repo_id=repo_id, run_name=run_name)
         return base_runs.get_run_heads(
             self._storage,
             self._compute,
             job_heads,
             include_request_heads,
             interrupted_job_new_status,
         )
 
     def poll_logs(
         self,
-        repo_address: RepoAddress,
-        job_heads: List[JobHead],
-        start_time: int,
-        attached: bool,
+        repo_id: str,
+        run_name: str,
+        start_time: datetime,
+        end_time: Optional[datetime] = None,
+        descending: bool = False,
     ) -> Generator[LogEvent, None, None]:
         return logs.poll_logs(
             self._storage,
-            self._compute,
             self._logs_client(),
             self.backend_config.bucket_name,
-            repo_address,
-            job_heads,
+            repo_id,
+            run_name,
             start_time,
-            attached,
+            end_time,
+            descending,
         )
 
-    def list_run_artifact_files(self, repo_address: RepoAddress, run_name: str) -> List[Artifact]:
-        return base_artifacts.list_run_artifact_files(self._storage, repo_address, run_name)
+    def list_run_artifact_files(self, repo_id: str, run_name: str) -> List[Artifact]:
+        return base_artifacts.list_run_artifact_files(self._storage, repo_id, run_name)
 
     def download_run_artifact_files(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         run_name: str,
-        output_dir: Optional[str],
-        files_path: Optional[str] = None,
+        output_dir: Optional[PathLike],
+        files_path: Optional[PathLike] = None,
     ):
-        artifacts = self.list_run_artifact_files(repo_address=repo_address, run_name=run_name)
+        artifacts = self.list_run_artifact_files(repo_id, run_name=run_name)
         base_artifacts.download_run_artifact_files(
             storage=self._storage,
-            repo_address=repo_address,
+            repo_id=repo_id,
             artifacts=artifacts,
             output_dir=output_dir,
             files_path=files_path,
         )
 
     def upload_job_artifact_files(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         job_id: str,
         artifact_name: str,
-        artifact_path: str,
-        local_path: Path,
+        artifact_path: PathLike,
+        local_path: PathLike,
     ):
         base_artifacts.upload_job_artifact_files(
             storage=self._storage,
-            repo_address=repo_address,
+            repo_id=repo_id,
             job_id=job_id,
             artifact_name=artifact_name,
             artifact_path=artifact_path,
             local_path=local_path,
         )
 
-    def list_tag_heads(self, repo_address: RepoAddress) -> List[TagHead]:
-        return base_tags.list_tag_heads(self._storage, repo_address)
+    def list_tag_heads(self, repo_id: str) -> List[TagHead]:
+        return base_tags.list_tag_heads(self._storage, repo_id)
 
-    def get_tag_head(self, repo_address: RepoAddress, tag_name: str) -> Optional[TagHead]:
-        return base_tags.get_tag_head(self._storage, repo_address, tag_name)
+    def get_tag_head(self, repo_id: str, tag_name: str) -> Optional[TagHead]:
+        return base_tags.get_tag_head(self._storage, repo_id, tag_name)
 
     def add_tag_from_run(
-        self,
-        repo_address: RepoAddress,
-        tag_name: str,
-        run_name: str,
-        run_jobs: Optional[List[Job]],
+        self, repo_id: str, tag_name: str, run_name: str, run_jobs: Optional[List[Job]]
     ):
         base_tags.create_tag_from_run(
             self._storage,
-            repo_address,
+            repo_id,
             tag_name,
             run_name,
             run_jobs,
         )
 
-    def add_tag_from_local_dirs(
-        self, repo_data: LocalRepoData, tag_name: str, local_dirs: List[str]
-    ):
-        base_tags.create_tag_from_local_dirs(
-            self._storage,
-            repo_data,
-            tag_name,
-            local_dirs,
-            self.type,
-        )
+    def add_tag_from_local_dirs(self, tag_name: str, local_dirs: List[str]):
+        # base_tags.create_tag_from_local_dirs(self._storage, self.repo, tag_name, local_dirs)
+        raise NotImplementedError()
 
-    def delete_tag_head(self, repo_address: RepoAddress, tag_head: TagHead):
-        base_tags.delete_tag(self._storage, repo_address, tag_head)
+    def delete_tag_head(self, repo_id: str, tag_head: TagHead):
+        base_tags.delete_tag(self._storage, repo_id, tag_head)
 
     def list_repo_heads(self) -> List[RepoHead]:
         return base_repos.list_repo_heads(self._storage)
 
-    def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
+    def update_repo_last_run_at(self, repo_spec: RepoSpec, last_run_at: int):
         base_repos.update_repo_last_run_at(
             self._storage,
-            repo_address,
+            repo_spec,
             last_run_at,
         )
 
-    def get_repo_credentials(self, repo_address: RepoAddress) -> Optional[RepoCredentials]:
-        return base_repos.get_repo_credentials(self._secrets_manager, repo_address)
+    def get_repo_credentials(self, repo_id: str) -> Optional[RemoteRepoCredentials]:
+        return base_repos.get_repo_credentials(self._secrets_manager, repo_id)
 
-    def save_repo_credentials(self, repo_address: RepoAddress, repo_credentials: RepoCredentials):
-        base_repos.save_repo_credentials(
-            self._secrets_manager,
-            repo_address,
-            repo_credentials,
-        )
+    def save_repo_credentials(self, repo_id: str, repo_credentials: RemoteRepoCredentials):
+        base_repos.save_repo_credentials(self._secrets_manager, repo_id, repo_credentials)
 
-    def list_secret_names(self, repo_address: RepoAddress) -> List[str]:
-        return base_secrets.list_secret_names(self._storage, repo_address)
+    def list_secret_names(self, repo_id: str) -> List[str]:
+        return base_secrets.list_secret_names(self._storage, repo_id)
 
-    def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
-        return base_secrets.get_secret(self._secrets_manager, repo_address, secret_name)
+    def get_secret(self, repo_id: str, secret_name: str) -> Optional[Secret]:
+        return base_secrets.get_secret(self._secrets_manager, repo_id, repo_id)
 
-    def add_secret(self, repo_address: RepoAddress, secret: Secret):
-        base_secrets.add_secret(
-            self._storage,
-            self._secrets_manager,
-            repo_address,
-            secret,
-        )
+    def add_secret(self, repo_id: str, secret: Secret):
+        base_secrets.add_secret(self._storage, self._secrets_manager, repo_id, secret)
 
-    def update_secret(self, repo_address: RepoAddress, secret: Secret):
-        base_secrets.update_secret(
-            self._storage,
-            self._secrets_manager,
-            repo_address,
-            secret,
-        )
+    def update_secret(self, repo_id: str, secret: Secret):
+        base_secrets.update_secret(self._storage, self._secrets_manager, repo_id, secret)
 
-    def delete_secret(self, repo_address: RepoAddress, secret_name: str):
-        base_secrets.delete_secret(
-            self._storage,
-            self._secrets_manager,
-            repo_address,
-            secret_name,
-        )
+    def delete_secret(self, repo_id: str, secret_name: str):
+        base_secrets.delete_secret(self._storage, self._secrets_manager, repo_id, repo_id)
 
     def get_signed_download_url(self, object_key: str) -> str:
         return self._storage.get_signed_download_url(object_key)
 
     def get_signed_upload_url(self, object_key: str) -> str:
         return self._storage.get_signed_upload_url(object_key)
 
-    def get_configurator(self):
-        return AWSConfigurator()
-
-    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
-        base_cache.delete_workflow_cache(self._storage, repo_address, username, workflow_name)
+    def delete_workflow_cache(self, repo_id: str, hub_user_name: str, workflow_name: str):
+        base_cache.delete_workflow_cache(self._storage, repo_id, hub_user_name, workflow_name)
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/aws/compute.py` & `dstack-0.8/cli/dstack/backend/aws/compute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Optional, Tuple
+from typing import Optional
 
 from botocore.client import BaseClient
 
 from dstack.backend.aws import runners
 from dstack.backend.base.compute import Compute
 from dstack.core.instance import InstanceType
-from dstack.core.job import Job, Requirements
+from dstack.core.job import Job
 from dstack.core.request import RequestHead
 
 
 class AWSCompute(Compute):
     def __init__(
         self,
         ec2_client: BaseClient,
@@ -42,17 +42,16 @@
             ec2_client=self.ec2_client,
             iam_client=self.iam_client,
             bucket_name=self.bucket_name,
             region_name=self.region_name,
             subnet_id=self.subnet_id,
             runner_id=job.runner_id,
             instance_type=instance_type,
-            local_repo_user_name=job.local_repo_user_name,
-            local_repo_user_email=job.local_repo_user_email,
-            repo_address=job.repo_address,
+            repo_id=job.repo_ref.repo_id,
+            hub_user_name=job.hub_user_name,
             ssh_key_pub=job.ssh_key_pub,
         )
 
     def terminate_instance(self, request_id: str):
         runners.terminate_instance(
             ec2_client=self.ec2_client,
             request_id=request_id,
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/aws/runners.py` & `dstack-0.8/cli/dstack/backend/aws/runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import botocore.exceptions
 from botocore.client import BaseClient
 
 from dstack import version
 from dstack.backend.base.compute import NoCapacityError, choose_instance_type
 from dstack.core.instance import InstanceType
 from dstack.core.job import Job, Requirements
-from dstack.core.repo import RepoAddress
+from dstack.core.repo import RepoRef
 from dstack.core.request import RequestHead, RequestStatus
 from dstack.core.runners import Gpu, Resources
 
 CREATE_INSTANCE_RETRY_RATE_SECS = 3
 
 
 def get_instance_type(
@@ -338,17 +338,16 @@
     ec2_client: BaseClient,
     iam_client: BaseClient,
     bucket_name: str,
     region_name: str,
     subnet_id: Optional[str],
     runner_id: str,
     instance_type: InstanceType,
-    local_repo_user_name: Optional[str],
-    local_repo_user_email: Optional[str],
-    repo_address: RepoAddress,
+    repo_id: str,
+    hub_user_name: str,
     ssh_key_pub: str,
 ) -> str:
     launch_specification = {}
     if not version.__is_release__:
         launch_specification["KeyName"] = "dstack_victor"
     if instance_type.resources.interruptible:
         launch_specification["InstanceMarketOptions"] = {
@@ -370,20 +369,17 @@
     else:
         launch_specification["SecurityGroupIds"] = [
             _get_security_group_id(ec2_client, bucket_name, subnet_id)
         ]
     tags = [
         {"Key": "owner", "Value": "dstack"},
         {"Key": "dstack_bucket", "Value": bucket_name},
-        {"Key": "dstack_repo", "Value": repo_address.path()},
+        {"Key": "dstack_repo", "Value": repo_id},
+        {"Key": "dstack_repo_user", "Value": hub_user_name},
     ]
-    if local_repo_user_name:
-        tags.append({"Key": "dstack_user_name", "Value": local_repo_user_name})
-    if local_repo_user_email:
-        tags.append({"Key": "dstack_user_email", "Value": local_repo_user_email})
     response = ec2_client.run_instances(
         BlockDeviceMappings=[
             {
                 "DeviceName": "/dev/sda1",
                 "Ebs": {
                     "VolumeSize": 100,
                     "VolumeType": "gp2",
@@ -420,32 +416,30 @@
     ec2_client: BaseClient,
     iam_client: BaseClient,
     bucket_name: str,
     region_name: str,
     subnet_id: Optional[str],
     runner_id: str,
     instance_type: InstanceType,
-    local_repo_user_name: Optional[str],
-    local_repo_user_email: Optional[str],
-    repo_address: RepoAddress,
+    repo_id: str,
+    hub_user_name: str,
     ssh_key_pub: str,
     attempts: int = 3,
 ) -> str:
     try:
         return _run_instance(
             ec2_client,
             iam_client,
             bucket_name,
             region_name,
             subnet_id,
             runner_id,
             instance_type,
-            local_repo_user_name,
-            local_repo_user_email,
-            repo_address,
+            repo_id,
+            hub_user_name,
             ssh_key_pub,
         )
     except botocore.exceptions.ClientError as e:
         # FIXME: why retry on "InvalidParameterValue"
         if e.response["Error"]["Code"] == "InvalidParameterValue":
             if attempts > 0:
                 time.sleep(CREATE_INSTANCE_RETRY_RATE_SECS)
@@ -453,29 +447,34 @@
                     ec2_client,
                     iam_client,
                     bucket_name,
                     region_name,
                     subnet_id,
                     runner_id,
                     instance_type,
-                    local_repo_user_name,
-                    local_repo_user_email,
-                    repo_address,
+                    repo_id,
+                    hub_user_name,
                     ssh_key_pub,
                     attempts - 1,
                 )
             else:
                 raise Exception("Failed to retry", e)
         elif e.response["Error"]["Code"] == "InsufficientInstanceCapacity":
             raise NoCapacityError()
         raise e
 
 
 def cancel_spot_request(ec2_client: BaseClient, request_id: str):
-    ec2_client.cancel_spot_instance_requests(SpotInstanceRequestIds=[request_id])
+    try:
+        ec2_client.cancel_spot_instance_requests(SpotInstanceRequestIds=[request_id])
+    except botocore.exceptions.ClientError as e:
+        if e.response["Error"]["Code"] == "InvalidSpotInstanceRequestID.NotFound":
+            return
+        else:
+            raise e
     response = ec2_client.describe_instances(
         Filters=[
             {"Name": "spot-instance-request-id", "Values": [request_id]},
         ],
     )
     if response.get("Reservations") and response["Reservations"][0].get("Instances"):
         ec2_client.terminate_instances(
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/aws/secrets.py` & `dstack-0.8/cli/dstack/backend/aws/secrets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
-from typing import List, Optional
+from typing import Optional
 
 from botocore.client import BaseClient
 
 from dstack.backend.aws import runners
 from dstack.backend.aws.utils import retry_operation_on_service_errors
 from dstack.backend.base.secrets import SecretsManager
-from dstack.core.repo import RepoAddress
 from dstack.core.secret import Secret
 
 
 class AWSSecretsManager(SecretsManager):
     def __init__(
         self,
         secretsmanager_client: BaseClient,
@@ -19,66 +18,66 @@
         bucket_name: str,
     ):
         self.secretsmanager_client = secretsmanager_client
         self.iam_client = iam_client
         self.sts_client = sts_client
         self.bucket_name = bucket_name
 
-    def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
+    def get_secret(self, repo_id: str, secret_name: str) -> Optional[Secret]:
         value = _get_secret_value(
             secretsmanager_client=self.secretsmanager_client,
-            secret_key=_get_secret_key(self.bucket_name, repo_address, secret_name),
+            secret_key=_get_secret_key(self.bucket_name, repo_id, secret_name),
         )
         if value is None:
             return None
         return Secret(secret_name=secret_name, secret_value=value)
 
-    def add_secret(self, repo_address: RepoAddress, secret: Secret):
+    def add_secret(self, repo_id: str, secret: Secret):
         _add_secret(
             secretsmanager_client=self.secretsmanager_client,
             sts_client=self.sts_client,
             iam_client=self.iam_client,
             bucket_name=self.bucket_name,
-            secret_key=_get_secret_key(self.bucket_name, repo_address, secret.secret_name),
+            secret_key=_get_secret_key(self.bucket_name, repo_id, secret.secret_name),
             secret_value=secret.secret_value,
         )
 
-    def update_secret(self, repo_address: RepoAddress, secret: Secret):
+    def update_secret(self, repo_id: str, secret: Secret):
         _update_secret(
             secretsmanager_client=self.secretsmanager_client,
-            secret_key=_get_secret_key(self.bucket_name, repo_address, secret.secret_name),
+            secret_key=_get_secret_key(self.bucket_name, repo_id, secret.secret_name),
             secret_value=secret.secret_value,
         )
 
-    def delete_secret(self, repo_address: RepoAddress, secret_name: str):
+    def delete_secret(self, repo_id: str, secret_name: str):
         _delete_secret(
             secretsmanager_client=self.secretsmanager_client,
-            secret_key=_get_secret_key(self.bucket_name, repo_address, secret_name),
+            secret_key=_get_secret_key(self.bucket_name, repo_id, secret_name),
         )
 
-    def get_credentials(self, repo_address: RepoAddress) -> Optional[str]:
+    def get_credentials(self, repo_id: str) -> Optional[str]:
         return _get_secret_value(
             secretsmanager_client=self.secretsmanager_client,
-            secret_key=_get_credentials_key(self.bucket_name, repo_address),
+            secret_key=_get_credentials_key(self.bucket_name, repo_id),
         )
 
-    def add_credentials(self, repo_address: RepoAddress, data: str):
+    def add_credentials(self, repo_id: str, data: str):
         _add_secret(
             secretsmanager_client=self.secretsmanager_client,
             sts_client=self.sts_client,
             iam_client=self.iam_client,
             bucket_name=self.bucket_name,
-            secret_key=_get_credentials_key(self.bucket_name, repo_address),
+            secret_key=_get_credentials_key(self.bucket_name, repo_id),
             secret_value=data,
         )
 
-    def update_credentials(self, repo_address: RepoAddress, data: str):
+    def update_credentials(self, repo_id: str, data: str):
         _update_secret(
             secretsmanager_client=self.secretsmanager_client,
-            secret_key=_get_credentials_key(self.bucket_name, repo_address),
+            secret_key=_get_credentials_key(self.bucket_name, repo_id),
             secret_value=data,
         )
 
 
 def _get_secret_value(
     secretsmanager_client: BaseClient,
     secret_key: str,
@@ -159,13 +158,13 @@
 ):
     secretsmanager_client.delete_secret(
         SecretId=secret_key,
         ForceDeleteWithoutRecovery=True,
     )
 
 
-def _get_secret_key(bucket_name: str, repo_address: RepoAddress, secret_name: str) -> str:
-    return f"/dstack/{bucket_name}/secrets/{repo_address.path()}/{secret_name}"
+def _get_secret_key(bucket_name: str, repo_id: str, secret_name: str) -> str:
+    return f"/dstack/{bucket_name}/secrets/{repo_id}/{secret_name}"
 
 
-def _get_credentials_key(bucket_name: str, repo_address: RepoAddress) -> str:
-    return f"/dstack/{bucket_name}/credentials/{repo_address.path()}"
+def _get_credentials_key(bucket_name: str, repo_id: str) -> str:
+    return f"/dstack/{bucket_name}/credentials/{repo_id}"
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/aws/storage.py` & `dstack-0.8/cli/dstack/backend/aws/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/backend/aws/utils.py` & `dstack-0.8/cli/dstack/backend/aws/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/__init__.py` & `dstack-0.8/cli/dstack/backend/base/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,240 +1,191 @@
-import sys
 from abc import ABC, abstractmethod
-from enum import Enum
-from pathlib import Path
-from typing import Any, Generator, List, Optional
+from datetime import datetime
+from typing import Generator, List, Optional
 
-from dstack.backend.base import jobs
+from dstack.backend.base import jobs as base_jobs
+from dstack.backend.base.compute import Compute
+from dstack.backend.base.config import BackendConfig
+from dstack.backend.base.secrets import SecretsManager
+from dstack.backend.base.storage import Storage
 from dstack.core.artifact import Artifact
-from dstack.core.config import BackendConfig, Configurator
 from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.log_event import LogEvent
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials, RepoHead
+from dstack.core.repo import RemoteRepoCredentials, RepoHead, RepoSpec
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
-
-
-class BackendType(Enum):
-    REMOTE = "remote"
-    LOCAL = "local"
-
-    def __str__(self):
-        return str(self.value)
+from dstack.utils.common import PathLike
 
 
 class Backend(ABC):
-    _loaded = False
+    NAME = None
+    backend_config: BackendConfig
+    _storage: Storage
+    _compute: Compute
+    _secrets_manager: SecretsManager
 
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        pass
-
-    @property
-    @abstractmethod
-    def type(self) -> BackendType:
-        pass
+    def __init__(
+        self,
+        backend_config: BackendConfig,
+    ):
+        self.backend_config = backend_config
 
     @property
-    def loaded(self):
-        return self._loaded
-
-    @abstractmethod
-    def configure(self):
-        pass
+    def name(self) -> str:
+        return self.NAME
 
     @abstractmethod
-    def create_run(self, repo_address: RepoAddress) -> str:
+    def create_run(self, repo_id: str) -> str:
         pass
 
     @abstractmethod
     def create_job(self, job: Job):
         pass
 
     def submit_job(self, job: Job, failed_to_start_job_new_status: JobStatus = JobStatus.FAILED):
         self.create_job(job)
         self.run_job(job, failed_to_start_job_new_status)
 
     def resubmit_job(self, job: Job, failed_to_start_job_new_status: JobStatus = JobStatus.FAILED):
-        jobs.update_job_submission(job)
+        base_jobs.update_job_submission(job)
         self.run_job(job, failed_to_start_job_new_status)
 
     @abstractmethod
-    def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
+    def get_job(self, repo_id: str, job_id: str) -> Optional[Job]:
         pass
 
     @abstractmethod
-    def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
+    def list_jobs(self, repo_id: str, run_name: str) -> List[Job]:
         pass
 
     @abstractmethod
     def run_job(self, job: Job, failed_to_start_job_new_status: JobStatus):
         pass
 
     @abstractmethod
-    def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
+    def stop_job(self, repo_id: str, abort: bool, job_id: str):
         pass
 
-    def stop_jobs(self, repo_address: RepoAddress, run_name: Optional[str], abort: bool):
-        job_heads = self.list_job_heads(repo_address, run_name)
-        for job_head in job_heads:
-            if job_head.status.is_unfinished():
-                self.stop_job(repo_address, job_head.job_id, abort)
-
     @abstractmethod
-    def list_job_heads(
-        self, repo_address: RepoAddress, run_name: Optional[str] = None
-    ) -> List[JobHead]:
+    def list_job_heads(self, repo_id: str, run_name: Optional[str] = None) -> List[JobHead]:
         pass
 
     @abstractmethod
-    def delete_job_head(self, repo_address: RepoAddress, job_id: str):
+    def delete_job_head(self, repo_id: str, job_id: str):
         pass
 
-    def delete_job_heads(self, repo_address: RepoAddress, run_name: Optional[str]):
-        job_heads = []
-        for job_head in self.list_job_heads(repo_address, run_name):
-            if job_head.status.is_finished():
-                job_heads.append(job_head)
-            else:
-                if run_name:
-                    sys.exit("The run is not finished yet. Stop the run first.")
-        for job_head in job_heads:
-            self.delete_job_head(repo_address, job_head.job_id)
-
     @abstractmethod
     def list_run_heads(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
         interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
         pass
 
     @abstractmethod
     def poll_logs(
         self,
-        repo_address: RepoAddress,
-        job_heads: List[JobHead],
-        start_time: int,
-        attached: bool,
+        repo_id: str,
+        run_name: str,
+        start_time: datetime,
+        end_time: Optional[datetime] = None,
+        descending: bool = False,
     ) -> Generator[LogEvent, None, None]:
         pass
 
     @abstractmethod
-    def list_run_artifact_files(self, repo_address: RepoAddress, run_name: str) -> List[Artifact]:
+    def list_run_artifact_files(self, repo_id: str, run_name: str) -> List[Artifact]:
         # TODO: add a flag for non-recursive listing.
         # Backends may implement this via list_run_artifact_files_and_folders()
         pass
 
     @abstractmethod
     def download_run_artifact_files(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         run_name: str,
-        output_dir: Optional[str],
-        files_path: Optional[str] = None,
+        output_dir: Optional[PathLike],
+        files_path: Optional[PathLike] = None,
     ):
         pass
 
     @abstractmethod
     def upload_job_artifact_files(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         job_id: str,
         artifact_name: str,
-        artifact_path: str,
-        local_path: Path,
+        artifact_path: PathLike,
+        local_path: PathLike,
     ):
         pass
 
     @abstractmethod
-    def list_tag_heads(self, repo_address: RepoAddress) -> List[TagHead]:
+    def list_tag_heads(self, repo_id: str) -> List[TagHead]:
         pass
 
     @abstractmethod
-    def get_tag_head(self, repo_address: RepoAddress, tag_name: str) -> Optional[TagHead]:
+    def get_tag_head(self, repo_id: str, tag_name: str) -> Optional[TagHead]:
         pass
 
     @abstractmethod
     def add_tag_from_run(
-        self,
-        repo_address: RepoAddress,
-        tag_name: str,
-        run_name: str,
-        run_jobs: Optional[List[Job]],
-    ):
-        pass
-
-    @abstractmethod
-    def add_tag_from_local_dirs(
-        self, repo_data: LocalRepoData, tag_name: str, local_dirs: List[str]
+        self, repo_id: str, tag_name: str, run_name: str, run_jobs: Optional[List[Job]]
     ):
         pass
 
     @abstractmethod
-    def delete_tag_head(self, repo_address: RepoAddress, tag_head: TagHead):
+    def add_tag_from_local_dirs(self, tag_name: str, local_dirs: List[str]):
         pass
 
     @abstractmethod
-    def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
+    def delete_tag_head(self, repo_id: str, tag_head: TagHead):
         pass
 
     @abstractmethod
-    def get_repo_credentials(self, repo_address: RepoAddress) -> Optional[RepoCredentials]:
+    def list_repo_heads(self) -> List[RepoHead]:
         pass
 
     @abstractmethod
-    def save_repo_credentials(self, repo_address: RepoAddress, repo_credentials: RepoCredentials):
+    def update_repo_last_run_at(self, repo_spec: RepoSpec, last_run_at: int):
         pass
 
     @abstractmethod
-    def list_secret_names(self, repo_address: RepoAddress) -> List[str]:
+    def get_repo_credentials(self, repo_id: str) -> Optional[RemoteRepoCredentials]:
         pass
 
     @abstractmethod
-    def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
+    def save_repo_credentials(self, repo_id: str, repo_credentials: RemoteRepoCredentials):
         pass
 
     @abstractmethod
-    def add_secret(self, repo_address: RepoAddress, secret: Secret):
+    def list_secret_names(self, repo_id: str) -> List[str]:
         pass
 
     @abstractmethod
-    def update_secret(self, repo_address: RepoAddress, secret: Secret):
+    def get_secret(self, repo_id: str, secret_name: str) -> Optional[Secret]:
         pass
 
     @abstractmethod
-    def delete_secret(self, repo_address: RepoAddress, secret_name: str):
+    def add_secret(self, repo_id: str, secret: Secret):
         pass
 
     @abstractmethod
-    def get_configurator(self) -> Configurator:
+    def update_secret(self, repo_id: str, secret: Secret):
         pass
 
     @abstractmethod
-    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
-        pass
-
-
-class RemoteBackend(Backend):
-    def __init__(self, backend_config: Optional[BackendConfig] = None, custom_client: Any = None):
+    def delete_secret(self, repo_id: str, secret_name: str):
         pass
 
-    @property
-    def type(self) -> BackendType:
-        return BackendType.REMOTE
-
-
-class CloudBackend(RemoteBackend):
     @abstractmethod
-    def list_repo_heads(self) -> List[RepoHead]:
+    def delete_workflow_cache(self, repo_id: str, hub_user_name: str, workflow_name: str):
         pass
 
     @abstractmethod
     def get_signed_download_url(self, object_key: str) -> str:
         pass
 
     @abstractmethod
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/artifacts.py` & `dstack-0.8/cli/dstack/backend/base/artifacts.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 from typing import List, Optional
 
 from tqdm import tqdm
 
 from dstack.backend.base import jobs
 from dstack.backend.base.storage import Storage
 from dstack.core.artifact import Artifact
-from dstack.core.repo import RepoAddress
+from dstack.utils.common import PathLike
 
 
-def list_run_artifact_files(
-    storage: Storage, repo_address: RepoAddress, run_name: str
-) -> List[Artifact]:
-    jobs_list = jobs.list_jobs(storage, repo_address, run_name)
+def list_run_artifact_files(storage: Storage, repo_id: str, run_name: str) -> List[Artifact]:
+    jobs_list = jobs.list_jobs(storage, repo_id, run_name)
     artifacts = []
     for job in jobs_list:
-        job_artifacts_dir = _get_job_artifacts_dir(repo_address, job.job_id)
+        job_artifacts_dir = _get_job_artifacts_dir(repo_id, job.job_id)
         if job.artifact_paths is None:
             continue
         for artifact_path in job.artifact_paths:
             artifact_name = os.path.join(artifact_path, "")
             artifact_path = artifact_name.lstrip(os.sep)
             job_artifact_files_path = os.path.join(job_artifacts_dir, artifact_path)
             artifact_files = storage.list_files(job_artifact_files_path)
@@ -32,15 +30,15 @@
             )
             artifacts.append(artifact)
     return artifacts
 
 
 def download_run_artifact_files(
     storage: Storage,
-    repo_address: RepoAddress,
+    repo_id: str,
     artifacts: List[Artifact],
     output_dir: Optional[str],
     files_path: Optional[str],
 ):
     if output_dir is None:
         output_dir = os.getcwd()
     for artifact in artifacts:
@@ -64,30 +62,30 @@
             desc=f"Downloading artifact '{artifact.name}'",
         ) as pbar:
 
             def callback(size):
                 pbar.update(size)
 
             for file in files:
-                artifacts_dir = _get_job_artifacts_dir(repo_address, artifact.job_id)
+                artifacts_dir = _get_job_artifacts_dir(repo_id, artifact.job_id)
                 source_path = os.path.join(artifacts_dir, artifact.path, file.filepath)
                 dest_path = os.path.join(output_dir, artifact.job_id, artifact.path, file.filepath)
                 Path(dest_path).parent.mkdir(parents=True, exist_ok=True)
                 storage.download_file(source_path, dest_path, callback)
 
 
 def upload_job_artifact_files(
     storage: Storage,
-    repo_address: RepoAddress,
+    repo_id: str,
     job_id: str,
     artifact_name: str,
-    artifact_path: str,
-    local_path: Path,
+    artifact_path: PathLike,
+    local_path: PathLike,
 ):
-    artifacts_dir = _get_job_artifacts_dir(repo_address, job_id)
+    artifacts_dir = _get_job_artifacts_dir(repo_id, job_id)
     total_size = 0
     for root, sub_dirs, files in os.walk(local_path):
         for filename in files:
             file_path = os.path.join(root, filename)
             file_size = os.path.getsize(file_path)
             total_size += file_size
     with tqdm(
@@ -107,13 +105,13 @@
                 source_path = filepath
                 dest_path = os.path.join(
                     artifacts_dir, artifact_path, Path(filepath).relative_to(local_path)
                 )
                 storage.upload_file(source_path, dest_path, callback)
 
 
-def _get_artifacts_dir(repo_address: RepoAddress) -> str:
-    return f"artifacts/{repo_address.path()}/"
+def _get_artifacts_dir(repo_id: str) -> str:
+    return f"artifacts/{repo_id}/"
 
 
-def _get_job_artifacts_dir(repo_address: RepoAddress, job_id: str) -> str:
-    return f"{_get_artifacts_dir(repo_address)}{job_id}/"
+def _get_job_artifacts_dir(repo_id: str, job_id: str) -> str:
+    return f"{_get_artifacts_dir(repo_id)}{job_id}/"
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/compute.py` & `dstack-0.8/cli/dstack/backend/base/compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from functools import cmp_to_key
-from typing import List, Optional, Tuple
+from typing import List, Optional
 
 from dstack.core.instance import InstanceType
 from dstack.core.job import Job, Requirements
 from dstack.core.request import RequestHead
 from dstack.core.runners import Resources
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/jobs.py` & `dstack-0.8/cli/dstack/backend/base/jobs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,145 +1,145 @@
 import uuid
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import yaml
 
 from dstack.backend.base import runners
 from dstack.backend.base.compute import Compute, NoCapacityError
 from dstack.backend.base.storage import Storage
-from dstack.core.job import Job, JobHead, JobStatus
-from dstack.core.repo import RepoAddress
+from dstack.core.error import NoMatchingInstanceError
+from dstack.core.job import Job, JobErrorCode, JobHead, JobStatus
+from dstack.core.repo import RepoRef
 from dstack.core.request import RequestStatus
 from dstack.core.runners import Runner
 from dstack.utils.common import get_milliseconds_since_epoch
 
 
 def create_job(
     storage: Storage,
     job: Job,
     create_head: bool = True,
 ):
     if create_head:
         storage.put_object(key=_get_job_head_filename(job), content="")
+
     storage.put_object(
-        key=_get_job_filename(job.repo_address, job.job_id), content=yaml.dump(job.serialize())
+        key=_get_job_filename(job.repo_ref.repo_id, job.job_id), content=yaml.dump(job.serialize())
     )
 
 
-def get_job(storage: Storage, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
-    obj = storage.get_object(_get_job_filename(repo_address, job_id))
+def get_job(storage: Storage, repo_id: str, job_id: str) -> Optional[Job]:
+    obj = storage.get_object(_get_job_filename(repo_id, job_id))
     if obj is None:
         return None
     job = Job.unserialize(yaml.load(obj, yaml.FullLoader))
     return job
 
 
 def update_job(storage: Storage, job: Job):
-    job_head_key_prefix = _get_job_head_filename_prefix(job.repo_address, job.job_id)
+    job_head_key_prefix = _get_job_head_filename_prefix(job.repo_ref.repo_id, job.job_id)
     job_keys = storage.list_objects(job_head_key_prefix)
     for key in job_keys:
         storage.delete_object(key)
     storage.put_object(key=_get_job_head_filename(job), content="")
     storage.put_object(
-        key=_get_job_filename(job.repo_address, job.job_id), content=yaml.dump(job.serialize())
+        key=_get_job_filename(job.repo_ref.repo_id, job.job_id), content=yaml.dump(job.serialize())
     )
 
 
-def list_jobs(
-    storage: Storage,
-    repo_address: RepoAddress,
-    run_name: str,
-) -> List[Job]:
-    job_key_run_prefix = _get_jobs_filenames_prefix(repo_address, run_name)
+def list_jobs(storage: Storage, repo_id: str, run_name: str) -> List[Job]:
+    job_key_run_prefix = _get_jobs_filenames_prefix(repo_id, run_name)
     jobs_keys = storage.list_objects(job_key_run_prefix)
     jobs = []
     for job_key in jobs_keys:
         job_obj = storage.get_object(job_key)
         job = Job.unserialize(yaml.load(job_obj, yaml.FullLoader))
         jobs.append(job)
     return jobs
 
 
-def list_job_head(storage: Storage, repo_address: RepoAddress, job_id: str) -> Optional[JobHead]:
-    job_head_key_prefix = _get_job_head_filename_prefix(repo_address, job_id)
+def list_job_head(storage: Storage, repo_id: str, job_id: str) -> Optional[JobHead]:
+    job_head_key_prefix = _get_job_head_filename_prefix(repo_id, job_id)
     job_head_keys = storage.list_objects(job_head_key_prefix)
     for job_head_key in job_head_keys:
         t = job_head_key[len(job_head_key_prefix) :].split(";")
-        # Skip legacy format
-        if len(t) == 7:
-            (
-                provider_name,
-                local_repo_user_name,
-                submitted_at,
-                status,
-                artifacts,
-                app_names,
-                tag_name,
-            ) = tuple(t)
-            run_name, workflow_name, job_index = tuple(job_id.split(","))
-            return JobHead(
-                job_id=job_id,
-                repo_address=repo_address,
-                run_name=run_name,
-                workflow_name=workflow_name or None,
-                provider_name=provider_name,
-                local_repo_user_name=local_repo_user_name or None,
-                status=JobStatus(status),
-                submitted_at=int(submitted_at),
-                artifact_paths=artifacts.split(",") if artifacts else None,
-                tag_name=tag_name or None,
-                app_names=app_names.split(",") or None,
-            )
+        (
+            provider_name,
+            hub_user_name,
+            submitted_at,
+            status_info,
+            artifacts,
+            app_names,
+            tag_name,
+        ) = tuple(t)
+        run_name, workflow_name, job_index = tuple(job_id.split(","))
+        status, error_code, container_exit_code = _parse_job_status_info(status_info)
+        return JobHead(
+            job_id=job_id,
+            repo_ref=RepoRef(repo_id=repo_id),
+            hub_user_name=hub_user_name,
+            run_name=run_name,
+            workflow_name=workflow_name or None,
+            provider_name=provider_name,
+            status=JobStatus(status),
+            error_code=JobErrorCode(error_code) if error_code else None,
+            container_exit_code=int(container_exit_code) if container_exit_code else None,
+            submitted_at=int(submitted_at),
+            artifact_paths=artifacts.split(",") if artifacts else None,
+            tag_name=tag_name or None,
+            app_names=app_names.split(",") or None,
+        )
     return None
 
 
 def list_job_heads(
     storage: Storage,
-    repo_address: RepoAddress,
+    repo_id: str,
     run_name: Optional[str] = None,
 ) -> List[JobHead]:
-    job_heads_keys_prefix = _get_job_heads_filenames_prefix(repo_address, run_name)
+    job_heads_keys_prefix = _get_job_heads_filenames_prefix(repo_id, run_name)
     job_heads_keys = storage.list_objects(job_heads_keys_prefix)
     job_heads = []
     for job_head_key in job_heads_keys:
-        t = job_head_key[len(_get_jobs_dir(repo_address)) :].split(";")
-        # Skip legacy format
-        if len(t) == 9:
-            (
-                _,
-                job_id,
-                provider_name,
-                local_repo_user_name,
-                submitted_at,
-                status,
-                artifacts,
-                app_names,
-                tag_name,
-            ) = tuple(t)
-            run_name, workflow_name, job_index = tuple(job_id.split(","))
-            job_heads.append(
-                JobHead(
-                    job_id=job_id,
-                    repo_address=repo_address,
-                    run_name=run_name,
-                    workflow_name=workflow_name or None,
-                    provider_name=provider_name,
-                    local_repo_user_name=local_repo_user_name,
-                    status=JobStatus(status),
-                    submitted_at=int(submitted_at),
-                    artifact_paths=artifacts.split(",") if artifacts else None,
-                    tag_name=tag_name or None,
-                    app_names=app_names.split(",") or None,
-                )
+        t = job_head_key[len(_get_jobs_dir(repo_id)) :].split(";")
+        (
+            _,
+            job_id,
+            provider_name,
+            hub_user_name,
+            submitted_at,
+            status_info,
+            artifacts,
+            app_names,
+            tag_name,
+        ) = tuple(t)
+        run_name, workflow_name, job_index = tuple(job_id.split(","))
+        status, error_code, container_exit_code = _parse_job_status_info(status_info)
+        job_heads.append(
+            JobHead(
+                job_id=job_id,
+                repo_ref=RepoRef(repo_id=repo_id),
+                hub_user_name=hub_user_name,
+                run_name=run_name,
+                workflow_name=workflow_name or None,
+                provider_name=provider_name,
+                status=JobStatus(status),
+                error_code=JobErrorCode(error_code) if error_code else None,
+                container_exit_code=int(container_exit_code) if container_exit_code else None,
+                submitted_at=int(submitted_at),
+                artifact_paths=artifacts.split(",") if artifacts else None,
+                tag_name=tag_name or None,
+                app_names=app_names.split(",") or None,
             )
+        )
     return job_heads
 
 
-def delete_job_head(storage: Storage, repo_address: RepoAddress, job_id: str):
-    job_head_key_prefix = _get_job_head_filename_prefix(repo_address, job_id)
+def delete_job_head(storage: Storage, repo_id: str, job_id: str):
+    job_head_key_prefix = _get_job_head_filename_prefix(repo_id, job_id)
     job_head_keys = storage.list_objects(job_head_key_prefix)
     for job_head_key in job_head_keys:
         storage.delete_object(job_head_key)
 
 
 def run_job(
     storage: Storage,
@@ -153,44 +153,45 @@
     runner = None
     try:
         job.runner_id = uuid.uuid4().hex
         update_job(storage, job)
         instance_type = compute.get_instance_type(job)
         if instance_type is None:
             job.status = JobStatus.FAILED
+            job.error_code = JobErrorCode.NO_INSTANCE_MATCHING_REQUIREMENTS
             update_job(storage, job)
-            exit(f"No instance type matching requirements.")
-
+            raise NoMatchingInstanceError("No instance type matching requirements")
         runner = Runner(
             runner_id=job.runner_id, request_id=None, resources=instance_type.resources, job=job
         )
         runners.create_runner(storage, runner)
         runner.request_id = compute.run_instance(job, instance_type)
         runners.update_runner(storage, runner)
     except NoCapacityError:
         job.status = failed_to_start_job_new_status
+        job.error_code = JobErrorCode.FAILED_TO_START_DUE_TO_NO_CAPACITY
         job.request_id = runner.request_id if runner else None
         update_job(storage, job)
     except Exception as e:
         job.status = JobStatus.FAILED
         job.request_id = runner.request_id if runner else None
         update_job(storage, job)
         raise e
 
 
 def stop_job(
     storage: Storage,
     compute: Compute,
-    repo_address: RepoAddress,
+    repo_id: str,
     job_id: str,
     abort: bool,
 ):
     # TODO: why checking statuses of job_head, job, runner at the same time
-    job_head = list_job_head(storage, repo_address, job_id)
-    job = get_job(storage, repo_address, job_id)
+    job_head = list_job_head(storage, repo_id, job_id)
+    job = get_job(storage, repo_id, job_id)
     runner = runners.get_runner(storage, job.runner_id) if job else None
     request_status = (
         compute.get_request_head(
             job, (runner.request_id if runner else None) or job.request_id
         ).status
         if job
         else RequestStatus.TERMINATED
@@ -245,43 +246,49 @@
 
 def update_job_submission(job: Job):
     job.status = JobStatus.SUBMITTED
     job.submission_num += 1
     job.submitted_at = get_milliseconds_since_epoch()
 
 
-def _get_jobs_dir(repo_address: RepoAddress) -> str:
-    return f"jobs/{repo_address.path()}/"
+def _get_jobs_dir(repo_id: str) -> str:
+    return f"jobs/{repo_id}/"
 
 
-def _get_job_filename(repo_address: RepoAddress, job_id: str) -> str:
-    return f"{_get_jobs_dir(repo_address)}{job_id}.yaml"
+def _get_job_filename(repo_id: str, job_id: str) -> str:
+    return f"{_get_jobs_dir(repo_id)}{job_id}.yaml"
 
 
-def _get_jobs_filenames_prefix(repo_address: RepoAddress, run_name: str) -> str:
-    return f"{_get_jobs_dir(repo_address)}{run_name},"
+def _get_jobs_filenames_prefix(repo_id: str, run_name: str) -> str:
+    return f"{_get_jobs_dir(repo_id)}{run_name},"
 
 
-def _get_job_heads_filenames_prefix(repo_address: RepoAddress, run_name: Optional[str]) -> str:
-    return f"{_get_jobs_dir(repo_address)}l;{run_name or ''}"
+def _get_job_heads_filenames_prefix(repo_id: str, run_name: Optional[str]) -> str:
+    return f"{_get_jobs_dir(repo_id)}l;{run_name or ''}"
 
 
-def _get_job_head_filename_prefix(repo_address: RepoAddress, job_id: str) -> str:
-    prefix = _get_jobs_dir(repo_address)
+def _get_job_head_filename_prefix(repo_id: str, job_id: str) -> str:
+    prefix = _get_jobs_dir(repo_id)
     key = f"{prefix}l;{job_id};"
     return key
 
 
 def _get_job_head_filename(job: Job) -> str:
-    prefix = _get_jobs_dir(job.repo_address)
+    prefix = _get_jobs_dir(job.repo_ref.repo_id)
     key = (
         f"{prefix}l;"
         f"{job.job_id};"
         f"{job.provider_name};"
-        f"{job.local_repo_user_name or ''};"
+        f"{job.hub_user_name};"
         f"{job.submitted_at};"
-        f"{job.status.value};"
+        f"{job.status.value},{job.error_code.value if job.error_code else ''},{job.container_exit_code or ''};"
         f"{','.join([a.artifact_path.replace('/', '_') for a in (job.artifact_specs or [])])};"
         f"{','.join([a.app_name for a in (job.app_specs or [])])};"
         f"{job.tag_name or ''}"
     )
     return key
+
+
+def _parse_job_status_info(status_info: str) -> Tuple[str, str, str]:
+    if len(status_info.split(",")) == 3:
+        return status_info.split(",")
+    return status_info, "", ""
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/logs.py` & `dstack-0.8/cli/dstack/backend/base/logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 import urllib.parse
 from typing import Any, Dict, Optional
 
 from dstack.backend.base import jobs
 from dstack.backend.base.storage import Storage
 from dstack.core.job import Job
 from dstack.core.log_event import LogEvent, LogEventSource
-from dstack.core.repo import RepoAddress
 
 WAIT_N_ONCE_FINISHED = 1
 
 CHECK_STATUS_EVERY_N = 3
 
 POLL_LOGS_RATE_SECS = 1
 
 
 def render_log_message(
     storage: Storage,
     event: Dict[str, Any],
-    repo_address: RepoAddress,
+    repo_id: str,
     jobs_cache: Dict[str, Job],
 ) -> LogEvent:
     if isinstance(event, str):
         event = json.loads(event)
     message = event["message"]
     if isinstance(message, str):
         message = json.loads(message)
     job_id = message["job_id"]
     log = message["log"]
     job = jobs_cache.get(job_id)
     if job is None:
-        job = jobs.get_job(storage, repo_address, job_id)
+        job = jobs.get_job(storage, repo_id, job_id)
         jobs_cache[job_id] = job
     log = fix_urls(log.encode(), job, {}).decode()
     return LogEvent(
         event_id=event["eventId"],
         timestamp=event["timestamp"],
         job_id=job_id,
         log_message=log,
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/repos.py` & `dstack-0.8/cli/dstack/backend/base/repos.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,146 @@
 import json
+import re
 from typing import List, Optional
 
 from dstack.backend.base.secrets import SecretsManager
 from dstack.backend.base.storage import Storage
-from dstack.core.repo import RepoAddress, RepoCredentials, RepoHead, RepoProtocol
+from dstack.core.repo import (
+    LocalRepoInfo,
+    RemoteRepoCredentials,
+    RemoteRepoInfo,
+    RepoHead,
+    RepoProtocol,
+    RepoSpec,
+)
+from dstack.utils.escape import Escaper
 
-
-def get_repo_head(storage: Storage, repo_address: RepoAddress) -> Optional[RepoHead]:
-    repo_head_prefix = _get_repo_head_filename_prefix(repo_address)
-    repo_heads_keys = storage.list_objects(repo_head_prefix)
-    if len(repo_heads_keys) == 0:
-        return None
-    repo_head_key = repo_heads_keys[0]
-    last_run_at, tags_count = repo_head_key[len(repo_head_prefix) :].split(";")
-    return RepoHead(
-        repo_host_name=repo_address.repo_host_name,
-        repo_port=repo_address.repo_port,
-        repo_user_name=repo_address.repo_user_name,
-        repo_name=repo_address.repo_name,
-        last_run_at=int(last_run_at) if last_run_at else None,
-        tags_count=int(tags_count),
-    )
+# repo_id, last_run_at, tags_count, repo_type, repo_info
+repo_head_re = re.compile(r"([^;]+);(\d+);(\d+);(remote|local);(.*)")
 
 
 def list_repo_heads(storage: Storage) -> List[RepoHead]:
     repo_heads_prefix = _get_repo_heads_prefix()
     repo_heads_keys = storage.list_objects(repo_heads_prefix)
     repo_heads = []
     for repo_head_key in repo_heads_keys:
-        tokens = repo_head_key[len(repo_heads_prefix) :].split(";")
-        # Skipt legacy repo heads
-        if len(tokens) != 3:
-            continue
-        repo_str, last_run_at, tags_count = tokens
-        repo_host_port, repo_user_name, repo_name = repo_str.split(",")
-        t = repo_host_port.split(":")
-        repo_host_name = t[0]
-        repo_port = t[1] if len(t) > 1 else None
-        repo_heads.append(
-            RepoHead(
-                repo_host_name=repo_host_name,
-                repo_port=repo_port,
-                repo_user_name=repo_user_name,
-                repo_name=repo_name,
-                last_run_at=int(last_run_at) if last_run_at else None,
-                tags_count=int(tags_count),
-            )
-        )
+        repo_head = _parse_repo_head_filename(repo_head_key)
+        if repo_head is not None:
+            repo_heads.append(repo_head)
     return repo_heads
 
 
-def update_repo_last_run_at(storage: Storage, repo_address: RepoAddress, last_run_at: int):
-    repo_head = get_repo_head(storage, repo_address)
+def update_repo_last_run_at(storage: Storage, repo_spec: RepoSpec, last_run_at: int):
+    repo_head = _get_repo_head(storage, repo_spec.repo_ref.repo_id)
     if repo_head is None:
+        repo_info = None
+        if repo_spec.repo_data.repo_type == "remote":
+            repo_info = RemoteRepoInfo(
+                repo_host_name=repo_spec.repo_data.repo_host_name,
+                repo_port=repo_spec.repo_data.repo_port,
+                repo_user_name=repo_spec.repo_data.repo_user_name,
+                repo_name=repo_spec.repo_data.repo_name,
+            )
+        elif repo_spec.repo_data.repo_type == "local":
+            repo_info = LocalRepoInfo(
+                repo_dir=Escaper({"/": "."}, escape_char="~").unescape(
+                    repo_spec.repo_data.repo_dir
+                ),
+            )
         repo_head = RepoHead(
-            repo_host_name=repo_address.repo_host_name,
-            repo_port=repo_address.repo_port,
-            repo_user_name=repo_address.repo_user_name,
-            repo_name=repo_address.repo_name,
-            last_run_at=None,
-            tags_count=0,
+            repo_id=repo_spec.repo_ref.repo_id,
+            repo_info=repo_info,
         )
     repo_head.last_run_at = last_run_at
     _create_or_update_repo_head(storage, repo_head)
 
 
-def delete_repo(storage: Storage, repo_address: RepoAddress):
-    _delete_repo_head(storage, repo_address)
+def delete_repo(storage: Storage, repo_id: str):
+    _delete_repo_head(storage, repo_id)
 
 
 def get_repo_credentials(
-    secrets_manager: SecretsManager, repo_address: RepoAddress
-) -> Optional[RepoCredentials]:
-    credentials_value = secrets_manager.get_credentials(repo_address)
+    secrets_manager: SecretsManager, repo_id: str
+) -> Optional[RemoteRepoCredentials]:
+    credentials_value = secrets_manager.get_credentials(repo_id)
     if credentials_value is None:
         return None
     credentials_data = json.loads(credentials_value)
-    return RepoCredentials(**credentials_data)
+    return RemoteRepoCredentials(**credentials_data)
 
 
 def save_repo_credentials(
-    secrets_manager: SecretsManager,
-    repo_address: RepoAddress,
-    repo_credentials: RepoCredentials,
+    secrets_manager: SecretsManager, repo_id, repo_credentials: RemoteRepoCredentials
 ):
     credentials_data = {"protocol": repo_credentials.protocol.value}
     if repo_credentials.protocol == RepoProtocol.HTTPS and repo_credentials.oauth_token:
         credentials_data["oauth_token"] = repo_credentials.oauth_token
     elif repo_credentials.protocol == RepoProtocol.SSH:
         if repo_credentials.private_key:
             credentials_data["private_key"] = repo_credentials.private_key
         else:
             raise Exception("No private key is specified")
 
-    credentials_value = secrets_manager.get_credentials(repo_address)
+    credentials_value = secrets_manager.get_credentials(repo_id)
     if credentials_value is not None:
-        secrets_manager.update_credentials(repo_address, json.dumps(credentials_data))
+        secrets_manager.update_credentials(repo_id, json.dumps(credentials_data))
     else:
-        secrets_manager.add_credentials(repo_address, json.dumps(credentials_data))
+        secrets_manager.add_credentials(repo_id, json.dumps(credentials_data))
+
+
+def _get_repo_head(storage: Storage, repo_id: str) -> Optional[RepoHead]:
+    repo_head_prefix = _get_repo_head_filename_prefix(repo_id)
+    repo_heads_keys = storage.list_objects(repo_head_prefix)
+    if len(repo_heads_keys) == 0:
+        return None
+    return _parse_repo_head_filename(repo_heads_keys[0])
 
 
 def _create_or_update_repo_head(storage: Storage, repo_head: RepoHead):
-    _delete_repo_head(storage=storage, repo_address=RepoAddress.parse_obj(repo_head))
-    repo_head_prefix = _get_repo_head_filename_prefix(
-        repo_address=RepoAddress.parse_obj(repo_head)
-    )
-    repo_head_key = (
-        f"{repo_head_prefix}" f"{repo_head.last_run_at or ''};" f"{repo_head.tags_count}"
-    )
+    _delete_repo_head(storage=storage, repo_id=repo_head.repo_id)
+    repo_head_prefix = _get_repo_head_filename_prefix(repo_head.repo_id)
+    repo_head_key = f"{repo_head_prefix}{repo_head.last_run_at or ''};{repo_head.tags_count};"
+    repo_head_key += repo_head.repo_info.head_key
     storage.put_object(key=repo_head_key, content="")
 
 
-def _delete_repo_head(storage: Storage, repo_address: RepoAddress):
-    repo_head_prefix = _get_repo_head_filename_prefix(repo_address)
+def _delete_repo_head(storage: Storage, repo_id: str):
+    repo_head_prefix = _get_repo_head_filename_prefix(repo_id)
     repo_heads_keys = storage.list_objects(repo_head_prefix)
     for repo_head_key in repo_heads_keys:
         storage.delete_object(repo_head_key)
 
 
 def _get_repo_heads_prefix() -> str:
     return "repos/l;"
 
 
-def _get_repo_head_filename_prefix(repo_address: RepoAddress) -> str:
-    return f"repos/l;{repo_address.path(delimiter=',')};"
+def _get_repo_head_filename_prefix(repo_id: str) -> str:
+    return f"{_get_repo_heads_prefix()}{repo_id};"
+
+
+def _parse_repo_head_filename(repo_head_filepath: str) -> Optional[RepoHead]:
+    repo_heads_prefix = _get_repo_heads_prefix()
+    r = repo_head_re.search(repo_head_filepath[len(repo_heads_prefix) :])
+    if r is None:
+        return r
+    repo_id, last_run_at, tags_count, repo_type, repo_info = r.groups()
+
+    if repo_type == "remote":
+        repo_host_name, repo_port, repo_user_name, repo_name = repo_info.split(",")
+        repo_info = RemoteRepoInfo(
+            repo_host_name=repo_host_name,
+            repo_port=repo_port or None,
+            repo_user_name=repo_user_name,
+            repo_name=repo_name,
+        )
+    elif repo_type == "local":
+        repo_dir = repo_info
+        repo_info = LocalRepoInfo(
+            repo_dir=Escaper({"/": "."}, escape_char="~").unescape(repo_dir),
+        )
+    return RepoHead(
+        repo_id=repo_id,
+        repo_info=repo_info,
+        last_run_at=int(last_run_at) if last_run_at else None,
+        tags_count=int(tags_count),
+    )
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/runners.py` & `dstack-0.8/cli/dstack/backend/base/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     obj = storage.get_object(_get_runner_filename(runner_id))
     if obj is None:
         return None
     return Runner.unserialize(yaml.load(obj, yaml.FullLoader))
 
 
 def create_runner(storage: Storage, runner: Runner):
-    metadata = {}
+    metadata = None
     if runner.job.status == JobStatus.STOPPING:
-        metadata["status"] = "stopping"
+        metadata = {"status": "stopping"}
     storage.put_object(
         key=_get_runner_filename(runner.runner_id),
         content=yaml.dump(runner.serialize()),
         metadata=metadata,
     )
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/runs.py` & `dstack-0.8/cli/dstack/backend/base/runs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,32 @@
 from typing import List
 
 import yaml
 
-from dstack.backend.base import BackendType, jobs, runners
+from dstack.backend.base import jobs, runners
 from dstack.backend.base.compute import Compute
 from dstack.backend.base.storage import Storage
 from dstack.core.app import AppHead
 from dstack.core.artifact import ArtifactHead
-from dstack.core.job import JobHead, JobStatus
-from dstack.core.repo import RepoAddress
-from dstack.core.run import (
-    RequestStatus,
-    RunHead,
-    generate_local_run_name_prefix,
-    generate_remote_run_name_prefix,
-)
+from dstack.core.job import JobErrorCode, JobHead, JobStatus
+from dstack.core.run import RequestStatus, RunHead, generate_remote_run_name_prefix
 
 
 def create_run(
     storage: Storage,
-    repo_address: RepoAddress,
-    backend_type: BackendType,
 ) -> str:
-    if backend_type is BackendType.LOCAL:
-        name = generate_local_run_name_prefix()
-    else:
-        name = generate_remote_run_name_prefix()
+    name = generate_remote_run_name_prefix()
     run_name_index = _next_run_name_index(storage, name)
     run_name = f"{name}-{run_name_index}"
     return run_name
 
 
 def _next_run_name_index(storage: Storage, run_name: str) -> int:
     count = 0
-    key = f"run-names/{run_name}.yaml"
+    key = f"run_names/{run_name}.yaml"
     obj = storage.get_object(key)
     if obj is None:
         storage.put_object(key=key, content=yaml.dump({"count": 1}))
         return 1
     count = yaml.load(obj, yaml.FullLoader)["count"]
     storage.put_object(key=key, content=yaml.dump({"count": count + 1}))
     return count + 1
@@ -95,37 +84,39 @@
         if job_head.artifact_paths
         else None
     )
     request_heads = None
     if include_request_heads and job_head.status.is_unfinished():
         if request_heads is None:
             request_heads = []
-        job = jobs.get_job(storage, job_head.repo_address, job_head.job_id)
+        job = jobs.get_job(storage, job_head.repo_ref.repo_id, job_head.job_id)
         request_id = job.request_id
         if request_id is None and job.runner_id is not None:
             runner = runners.get_runner(storage, job.runner_id)
             if not (runner is None):
                 request_id = runner.request_id
         request_head = compute.get_request_head(job, request_id)
         request_heads.append(request_head)
         if request_head.status == RequestStatus.NO_CAPACITY:
             job.status = job_head.status = interrupted_job_new_status
+            if interrupted_job_new_status == JobStatus.FAILED:
+                job.error_code = JobErrorCode.INTERRUPTED_BY_NO_CAPACITY
             jobs.update_job(storage, job)
     run_head = RunHead(
-        repo_address=job_head.repo_address,
         run_name=job_head.run_name,
         workflow_name=job_head.workflow_name,
         provider_name=job_head.provider_name,
-        local_repo_user_name=job_head.local_repo_user_name,
+        hub_user_name=job_head.hub_user_name,
         artifact_heads=artifact_heads or None,
         status=job_head.status,
         submitted_at=job_head.submitted_at,
         tag_name=job_head.tag_name,
         app_heads=app_heads,
         request_heads=request_heads,
+        job_heads=[job_head],
     )
     return run_head
 
 
 def _update_run(
     storage: Storage,
     compute: Compute,
@@ -159,18 +150,21 @@
                 )
             )
         )
     if job_head.status.is_unfinished():
         if include_request_heads:
             if run.request_heads is None:
                 run.request_heads = []
-            job = jobs.get_job(storage, job_head.repo_address, job_head.job_id)
+            job = jobs.get_job(storage, job_head.repo_ref.repo_id, job_head.job_id)
             request_id = job.request_id
             if request_id is None and job.runner_id is not None:
                 runner = runners.get_runner(storage, job.runner_id)
                 request_id = runner.request_id
             request_head = compute.get_request_head(job, request_id)
             run.request_heads.append(request_head)
             if request_head.status == RequestStatus.NO_CAPACITY:
                 job.status = job_head.status = interrupted_job_new_status
+                if interrupted_job_new_status == JobStatus.FAILED:
+                    job.error_code = JobErrorCode.INTERRUPTED_BY_NO_CAPACITY
                 jobs.update_job(storage, job)
         run.status = job_head.status
+    run.job_heads.append(job_head)
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/storage.py` & `dstack-0.8/cli/dstack/backend/base/storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         """
         pass
 
     def delete_prefix(self, keys_prefix: str):
         for key in self.list_objects(keys_prefix):
             self.delete_object(key)
 
+    def key_exists(self, key: str) -> bool:
+        return any(key == obj for obj in self.list_objects(key))
+
 
 class CloudStorage(Storage):
     @abstractmethod
     def get_signed_download_url(self, key: str) -> str:
         pass
 
     @abstractmethod
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/base/tags.py` & `dstack-0.8/cli/dstack/backend/base/tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,179 +1,180 @@
 import time
 from pathlib import Path
 from typing import List, Optional
 
-from dstack.backend.base import BackendType, artifacts, jobs, runs
+from dstack.backend.base import artifacts, jobs, runs
 from dstack.backend.base.storage import Storage
 from dstack.core.artifact import ArtifactHead, ArtifactSpec
 from dstack.core.error import BackendError
 from dstack.core.job import Job, JobStatus
-from dstack.core.repo import LocalRepoData, RepoAddress
+from dstack.core.repo import Repo
 from dstack.core.tag import TagHead
 from dstack.utils.common import get_milliseconds_since_epoch
 
 
-def get_tag_head(storage: Storage, repo_address: RepoAddress, tag_name: str) -> Optional[TagHead]:
-    tag_head_key_prefix = _get_tag_head_filename_prefix(repo_address, tag_name)
+def get_tag_head(storage: Storage, repo_id: str, tag_name: str) -> Optional[TagHead]:
+    tag_head_key_prefix = _get_tag_head_filename_prefix(repo_id, tag_name)
     tag_head_keys = storage.list_objects(keys_prefix=tag_head_key_prefix)
     if len(tag_head_keys) == 0:
         return None
     t = tag_head_keys[0][len(tag_head_key_prefix) :].split(";")
     if len(t) == 6:
         (
             run_name,
             workflow_name,
             provider_name,
-            local_repo_user_name,
+            hub_user_name,
             created_at,
             artifact_heads,
         ) = tuple(t)
         return TagHead(
-            repo_address=repo_address,
+            repo_id=repo_id,
             tag_name=tag_name,
             run_name=run_name,
             workflow_name=workflow_name or None,
             provider_name=provider_name or None,
-            local_repo_user_name=local_repo_user_name or None,
+            hub_user_name=hub_user_name or None,
             created_at=int(created_at),
             artifact_heads=_unserialize_artifact_heads(artifact_heads),
         )
 
 
-def list_tag_heads(storage: Storage, repo_address: RepoAddress):
-    tag_heads_keys_prefix = _get_tag_heads_filenames_prefix(repo_address)
+def list_tag_heads(storage: Storage, repo_id: str):
+    tag_heads_keys_prefix = _get_tag_heads_filenames_prefix(repo_id)
     tag_heads_keys = storage.list_objects(tag_heads_keys_prefix)
     tag_heads = []
     for tag_head_key in tag_heads_keys:
         t = tag_head_key[len(tag_heads_keys_prefix) :].split(";")
         if len(t) == 7:
             (
                 tag_name,
                 run_name,
                 workflow_name,
                 provider_name,
-                local_repo_user_name,
+                hub_user_name,
                 created_at,
                 artifact_heads,
             ) = tuple(t)
             tag_heads.append(
                 TagHead(
-                    repo_address=repo_address,
+                    repo_id=repo_id,
                     tag_name=tag_name,
                     run_name=run_name,
                     workflow_name=workflow_name or None,
                     provider_name=provider_name or None,
-                    local_repo_user_name=local_repo_user_name or None,
+                    hub_user_name=hub_user_name or None,
                     created_at=int(created_at),
                     artifact_heads=_unserialize_artifact_heads(artifact_heads),
                 )
             )
     return tag_heads
 
 
 def delete_tag(
     storage: Storage,
-    repo_address: RepoAddress,
+    repo_id: str,
     tag_head: TagHead,
 ):
     tag_jobs = []
-    job_heads = jobs.list_job_heads(storage, repo_address, tag_head.run_name)
+    job_heads = jobs.list_job_heads(storage, repo_id, tag_head.run_name)
     for job_head in job_heads:
-        job = jobs.get_job(storage, repo_address, job_head.job_id)
+        job = jobs.get_job(storage, repo_id, job_head.job_id)
         if job is not None:
             tag_jobs.append(job)
-    storage.delete_object(_get_tag_head_key(tag_head))
+    storage.delete_object(tag_head.key())
     for job in tag_jobs:
         job.tag_name = None
         jobs.update_job(storage, job)
 
 
 def create_tag_from_run(
     storage: Storage,
-    repo_address: RepoAddress,
+    repo_id: str,
     tag_name: str,
     run_name: str,
     run_jobs: Optional[List[Job]],
 ):
     if run_jobs:
         tag_jobs = run_jobs
     else:
         tag_jobs = []
         job_with_anther_tag = None
-        job_heads = jobs.list_job_heads(storage, repo_address, run_name)
+        job_heads = jobs.list_job_heads(storage, repo_id, run_name)
         for job_head in job_heads:
-            job = jobs.get_job(storage, repo_address, job_head.job_id)
+            job = jobs.get_job(storage, repo_id, job_head.job_id)
             if job:
                 tag_jobs.append(job)
                 if job.tag_name and job.tag_name != tag_name:
                     job_with_anther_tag = job
         if job_with_anther_tag:
             raise BackendError(
                 f"The run '{job_with_anther_tag.run_name}' refers to another tag: "
                 f"'{job_with_anther_tag.tag_name}'"
             )
         if not tag_jobs:
             exit(f"Cannot find the run '{run_name}'")
 
     tag_head = TagHead(
-        repo_address=repo_address,
+        repo_id=repo_id,
         tag_name=tag_name,
         run_name=run_name,
         workflow_name=tag_jobs[0].workflow_name,
         provider_name=tag_jobs[0].provider_name,
-        local_repo_user_name=tag_jobs[0].local_repo_user_name,
+        hub_user_name=tag_jobs[0].hub_user_name,
         created_at=int(round(time.time() * 1000)),
         artifact_heads=[
             ArtifactHead(job_id=run_job.job_id, artifact_path=artifact_spec.artifact_path)
             for run_job in tag_jobs
             for artifact_spec in run_job.artifact_specs or []
         ]
         or None,
     )
-    storage.put_object(key=_get_tag_head_key(tag_head), content="")
+    storage.put_object(key=tag_head.key(), content="")
 
     if not run_jobs:
         for job in tag_jobs:
             job.tag_name = tag_name
             jobs.update_job(storage, job)
 
 
 def create_tag_from_local_dirs(
     storage: Storage,
-    repo_data: LocalRepoData,
+    repo: Repo,
+    hub_user_name: str,
     tag_name: str,
     local_dirs: List[str],
-    backend_type: BackendType,
 ):
     local_paths = []
     tag_artifacts = []
     for local_dir in local_dirs:
         path = Path(local_dir)
         if path.is_dir():
             local_paths.append(path)
             tag_artifacts.append(str(path))
         else:
             exit(f"The '{local_dir}' path doesn't refer to an existing directory")
 
-    run_name = runs.create_run(storage, repo_data, backend_type)
+    run_name = runs.create_run(storage)
     job = Job(
         job_id=f"{run_name},,0",
-        repo_data=repo_data,
+        repo_ref=repo.repo_ref,
+        hub_user_name=hub_user_name,
+        repo_data=repo.repo_data,
         run_name=run_name,
         workflow_name=None,
         provider_name="bash",
-        local_repo_user_name=repo_data.local_repo_user_name,
-        local_repo_user_email=repo_data.local_repo_user_email,
         status=JobStatus.DONE,
         submitted_at=get_milliseconds_since_epoch(),
         image_name="scratch",
         commands=None,
         env=None,
         working_dir=None,
         artifact_specs=[ArtifactSpec(artifact_path=a, mount=False) for a in tag_artifacts],
+        cache_specs=[],
         port_count=None,
         ports=None,
         host_name=None,
         requirements=None,
         dep_specs=None,
         master_job=None,
         app_specs=None,
@@ -181,69 +182,54 @@
         request_id=None,
         tag_name=tag_name,
     )
     jobs.create_job(storage, job, create_head=False)
     for index, local_path in enumerate(local_paths):
         artifacts.upload_job_artifact_files(
             storage,
-            repo_data,
+            repo.repo_id,
             job.job_id,
             tag_artifacts[index],
             tag_artifacts[index],
             local_path,
         )
     tag_head = TagHead(
-        repo_address=repo_data,
+        repo_id=repo.repo_id,
         tag_name=tag_name,
         run_name=run_name,
         workflow_name=job.workflow_name,
         provider_name=job.provider_name,
-        local_repo_user_name=job.local_repo_user_name,
+        hub_user_name=hub_user_name,
         created_at=job.submitted_at,
         artifact_heads=[
             ArtifactHead(job_id=job.job_id, artifact_path=a.artifact_path)
             for a in job.artifact_specs
         ]
         if job.artifact_specs
         else None,
     )
-    tag_head_key = _get_tag_head_key(tag_head)
-    storage.put_object(key=tag_head_key, content="")
+    storage.put_object(key=tag_head.key(), content="")
 
 
-def _get_tags_dir(repo_address: RepoAddress) -> str:
-    return f"tags/{repo_address.path()}/"
+def _get_tags_dir(repo_id: str) -> str:
+    return f"tags/{repo_id}/"
 
 
-def _get_tag_head_filename_prefix(repo_address: RepoAddress, tag_name: str) -> str:
-    prefix = _get_tags_dir(repo_address)
+def _get_tag_head_filename_prefix(repo_id: str, tag_name: str) -> str:
+    prefix = _get_tags_dir(repo_id)
     key = f"{prefix}l;{tag_name};"
     return key
 
 
-def _get_tag_heads_filenames_prefix(repo_address: RepoAddress) -> str:
-    prefix = _get_tags_dir(repo_address)
+def _get_tag_heads_filenames_prefix(repo_id: str) -> str:
+    prefix = _get_tags_dir(repo_id)
     key = f"{prefix}l;"
     return key
 
 
-def _get_tag_head_key(tag_head: TagHead) -> str:
-    prefix = f"tags/{tag_head.repo_address.path()}"
-    key = (
-        f"{prefix}/l;{tag_head.tag_name};"
-        f"{tag_head.run_name};"
-        f"{tag_head.workflow_name or ''};"
-        f"{tag_head.provider_name or ''};"
-        f"{tag_head.local_repo_user_name or ''};"
-        f"{tag_head.created_at};"
-        f"{_serialize_artifact_heads(tag_head)}"
-    )
-    return key
-
-
 def _unserialize_artifact_heads(artifact_heads):
     return (
         [
             ArtifactHead(job_id=a.split("=")[0], artifact_path=a.split("=")[1])
             for a in artifact_heads.split(":")
         ]
         if artifact_heads
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/gcp/__init__.py` & `dstack-0.8/cli/dstack/backend/gcp/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,277 +1,229 @@
-import os
 import warnings
-from pathlib import Path
+from datetime import datetime
 from typing import Generator, List, Optional
 
 from google.auth._default import _CLOUD_SDK_CREDENTIALS_WARNING
 from google.oauth2 import service_account
 
-from dstack.backend.base import CloudBackend
+from dstack.backend.base import Backend
 from dstack.backend.base import artifacts as base_artifacts
 from dstack.backend.base import cache as base_cache
 from dstack.backend.base import jobs as base_jobs
 from dstack.backend.base import repos as base_repos
 from dstack.backend.base import runs as base_runs
 from dstack.backend.base import secrets as base_secrets
 from dstack.backend.base import tags as base_tags
 from dstack.backend.gcp.compute import GCPCompute
-from dstack.backend.gcp.config import GCPConfig, GCPConfigurator
+from dstack.backend.gcp.config import GCPConfig
 from dstack.backend.gcp.logs import GCPLogging
 from dstack.backend.gcp.secrets import GCPSecretsManager
-from dstack.backend.gcp.storage import BucketNotFoundError, GCPStorage
+from dstack.backend.gcp.storage import GCPStorage
 from dstack.cli.common import console
 from dstack.core.artifact import Artifact
-from dstack.core.error import ConfigError
 from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.log_event import LogEvent
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials, RepoHead
+from dstack.core.repo import RemoteRepoCredentials, RepoHead, RepoSpec
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
+from dstack.utils.common import PathLike
 
 warnings.filterwarnings("ignore", message=_CLOUD_SDK_CREDENTIALS_WARNING)
 
 
-class GCPBackend(CloudBackend):
-    def __init__(self, backend_config: Optional[GCPConfig] = None):
-        if backend_config is None:
-            try:
-                backend_config = GCPConfig.load()
-            except ConfigError:
-                return
-
-        self.config = backend_config
-
-        if self.config.credentials is not None:
-            credentials = service_account.Credentials.from_service_account_info(
-                self.config.credentials
-            )
-        elif self.config.credentials_file is not None:
-            credentials = service_account.Credentials.from_service_account_file(
-                self.config.credentials_file
-            )
-        else:
-            credentials_file = os.getenv("GOOGLE_APPLICATION_CREDENTIALS")
-            if credentials_file is None:
-                return
-            credentials = service_account.Credentials.from_service_account_file(credentials_file)
-
-        try:
-            self._storage = GCPStorage(
-                project_id=self.config.project_id,
-                bucket_name=self.config.bucket_name,
-                credentials=credentials,
-            )
-        except BucketNotFoundError:
-            return
-        self._compute = GCPCompute(gcp_config=self.config, credentials=credentials)
+class GCPBackend(Backend):
+    NAME = "gcp"
+    backend_config: GCPConfig
+    _storage: GCPStorage
+    _compute: GCPCompute
+    _secrets_manager: GCPSecretsManager
+
+    def __init__(
+        self,
+        backend_config: GCPConfig,
+    ):
+        super().__init__(backend_config=backend_config)
+        credentials = service_account.Credentials.from_service_account_info(
+            self.backend_config.credentials
+        )
+        self._storage = GCPStorage(
+            project_id=self.backend_config.project_id,
+            bucket_name=self.backend_config.bucket_name,
+            credentials=credentials,
+        )
+        self._compute = GCPCompute(gcp_config=self.backend_config, credentials=credentials)
         self._secrets_manager = GCPSecretsManager(
-            project_id=self.config.project_id,
-            bucket_name=self.config.bucket_name,
+            project_id=self.backend_config.project_id,
+            bucket_name=self.backend_config.bucket_name,
             credentials=credentials,
         )
         self._logging = GCPLogging(
-            project_id=self.config.project_id,
-            bucket_name=self.config.bucket_name,
+            project_id=self.backend_config.project_id,
+            bucket_name=self.backend_config.bucket_name,
             credentials=credentials,
         )
-        self._loaded = True
-
-    @property
-    def name(self) -> str:
-        return "gcp"
 
-    def configure(self):
-        pass
-
-    def create_run(self, repo_address: RepoAddress) -> str:
-        return base_runs.create_run(self._storage, repo_address, self.type)
+    def create_run(self, repo_id: str) -> str:
+        return base_runs.create_run(self._storage)
 
     def create_job(self, job: Job):
         if job.artifact_specs and any(art_spec.mount for art_spec in job.artifact_specs):
             console.print("Mount artifacts are not currently supported for 'gcp' backend")
             exit(1)
         base_jobs.create_job(self._storage, job)
 
-    def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
-        return base_jobs.get_job(self._storage, repo_address, job_id)
+    def get_job(self, repo_id: str, job_id: str) -> Optional[Job]:
+        return base_jobs.get_job(self._storage, repo_id, job_id)
 
-    def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
-        return base_jobs.list_jobs(self._storage, repo_address, run_name)
+    def list_jobs(self, repo_id: str, run_name: str) -> List[Job]:
+        return base_jobs.list_jobs(self._storage, repo_id, run_name)
 
     def run_job(self, job: Job, failed_to_start_job_new_status: JobStatus):
         base_jobs.run_job(self._storage, self._compute, job, failed_to_start_job_new_status)
 
-    def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
-        base_jobs.stop_job(self._storage, self._compute, repo_address, job_id, abort)
+    def stop_job(self, repo_id: str, abort: bool, job_id: str):
+        base_jobs.stop_job(self._storage, self._compute, repo_id, job_id, abort)
 
-    def list_job_heads(
-        self, repo_address: RepoAddress, run_name: Optional[str] = None
-    ) -> List[JobHead]:
-        return base_jobs.list_job_heads(self._storage, repo_address, run_name)
+    def list_job_heads(self, repo_id: str, run_name: Optional[str] = None) -> List[JobHead]:
+        return base_jobs.list_job_heads(self._storage, repo_id, run_name)
 
-    def delete_job_head(self, repo_address: RepoAddress, job_id: str):
-        base_jobs.delete_job_head(self._storage, repo_address, job_id)
+    def delete_job_head(self, repo_id: str, job_id: str):
+        base_jobs.delete_job_head(self._storage, repo_id, job_id)
 
     def list_run_heads(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
         interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
-        job_heads = self.list_job_heads(repo_address, run_name)
+        job_heads = self.list_job_heads(repo_id=repo_id, run_name=run_name)
         return base_runs.get_run_heads(
             self._storage,
             self._compute,
             job_heads,
             include_request_heads,
             interrupted_job_new_status,
         )
 
     def poll_logs(
         self,
-        repo_address: RepoAddress,
-        job_heads: List[JobHead],
-        start_time: int,
-        attached: bool,
+        repo_id: str,
+        run_name: str,
+        start_time: datetime,
+        end_time: Optional[datetime] = None,
+        descending: bool = False,
     ) -> Generator[LogEvent, None, None]:
         yield from self._logging.poll_logs(
             storage=self._storage,
-            repo_address=repo_address,
-            run_name=job_heads[0].run_name,
+            repo_id=repo_id,
+            run_name=run_name,
             start_time=start_time,
+            end_time=end_time,
+            descending=descending,
         )
 
-    def list_run_artifact_files(self, repo_address: RepoAddress, run_name: str) -> List[Artifact]:
-        return base_artifacts.list_run_artifact_files(self._storage, repo_address, run_name)
+    def list_run_artifact_files(self, repo_id: str, run_name: str) -> List[Artifact]:
+        return base_artifacts.list_run_artifact_files(self._storage, repo_id, run_name)
 
     def download_run_artifact_files(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         run_name: str,
-        output_dir: Optional[str],
-        files_path: Optional[str] = None,
+        output_dir: Optional[PathLike],
+        files_path: Optional[PathLike] = None,
     ):
-        artifacts = self.list_run_artifact_files(repo_address=repo_address, run_name=run_name)
+        artifacts = self.list_run_artifact_files(repo_id, run_name=run_name)
         base_artifacts.download_run_artifact_files(
             storage=self._storage,
-            repo_address=repo_address,
+            repo_id=repo_id,
             artifacts=artifacts,
             output_dir=output_dir,
             files_path=files_path,
         )
 
     def upload_job_artifact_files(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         job_id: str,
         artifact_name: str,
-        artifact_path: str,
-        local_path: Path,
+        artifact_path: PathLike,
+        local_path: PathLike,
     ):
         base_artifacts.upload_job_artifact_files(
             storage=self._storage,
-            repo_address=repo_address,
+            repo_id=repo_id,
             job_id=job_id,
             artifact_name=artifact_name,
             artifact_path=artifact_path,
             local_path=local_path,
         )
 
-    def list_tag_heads(self, repo_address: RepoAddress) -> List[TagHead]:
-        return base_tags.list_tag_heads(self._storage, repo_address)
+    def list_tag_heads(self, repo_id: str) -> List[TagHead]:
+        return base_tags.list_tag_heads(self._storage, repo_id)
 
-    def get_tag_head(self, repo_address: RepoAddress, tag_name: str) -> Optional[TagHead]:
-        return base_tags.get_tag_head(self._storage, repo_address, tag_name)
+    def get_tag_head(self, repo_id: str, tag_name: str) -> Optional[TagHead]:
+        return base_tags.get_tag_head(self._storage, repo_id, tag_name)
 
     def add_tag_from_run(
-        self,
-        repo_address: RepoAddress,
-        tag_name: str,
-        run_name: str,
-        run_jobs: Optional[List[Job]],
+        self, repo_id: str, tag_name: str, run_name: str, run_jobs: Optional[List[Job]]
     ):
         base_tags.create_tag_from_run(
             self._storage,
-            repo_address,
+            repo_id,
             tag_name,
             run_name,
             run_jobs,
         )
 
-    def add_tag_from_local_dirs(
-        self, repo_data: LocalRepoData, tag_name: str, local_dirs: List[str]
-    ):
-        base_tags.create_tag_from_local_dirs(
-            self._storage,
-            repo_data,
-            tag_name,
-            local_dirs,
-            self.type,
-        )
+    def add_tag_from_local_dirs(self, tag_name: str, local_dirs: List[str]):
+        # base_tags.create_tag_from_local_dirs(
+        #     self._storage,
+        #     self.repo,
+        #     tag_name,
+        #     local_dirs,
+        # )
+        raise NotImplementedError()
 
-    def delete_tag_head(self, repo_address: RepoAddress, tag_head: TagHead):
-        base_tags.delete_tag(self._storage, repo_address, tag_head)
+    def delete_tag_head(self, repo_id: str, tag_head: TagHead):
+        base_tags.delete_tag(self._storage, repo_id, tag_head)
 
     def list_repo_heads(self) -> List[RepoHead]:
         return base_repos.list_repo_heads(self._storage)
 
-    def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
+    def update_repo_last_run_at(self, repo_spec: RepoSpec, last_run_at: int):
         base_repos.update_repo_last_run_at(
             self._storage,
-            repo_address,
+            repo_spec,
             last_run_at,
         )
 
-    def get_repo_credentials(self, repo_address: RepoAddress) -> Optional[RepoCredentials]:
-        return base_repos.get_repo_credentials(self._secrets_manager, repo_address)
+    def get_repo_credentials(self, repo_id: str) -> Optional[RemoteRepoCredentials]:
+        return base_repos.get_repo_credentials(self._secrets_manager, repo_id)
 
-    def save_repo_credentials(self, repo_address: RepoAddress, repo_credentials: RepoCredentials):
-        base_repos.save_repo_credentials(
-            self._secrets_manager,
-            repo_address,
-            repo_credentials,
-        )
+    def save_repo_credentials(self, repo_id: str, repo_credentials: RemoteRepoCredentials):
+        base_repos.save_repo_credentials(self._secrets_manager, repo_id, repo_credentials)
 
-    def list_secret_names(self, repo_address: RepoAddress) -> List[str]:
-        return base_secrets.list_secret_names(self._storage, repo_address)
+    def list_secret_names(self, repo_id: str) -> List[str]:
+        return base_secrets.list_secret_names(self._storage, repo_id)
 
-    def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
-        return base_secrets.get_secret(self._secrets_manager, repo_address, secret_name)
+    def get_secret(self, repo_id: str, secret_name: str) -> Optional[Secret]:
+        return base_secrets.get_secret(self._secrets_manager, repo_id, secret_name)
 
-    def add_secret(self, repo_address: RepoAddress, secret: Secret):
-        base_secrets.add_secret(
-            self._storage,
-            self._secrets_manager,
-            repo_address,
-            secret,
-        )
+    def add_secret(self, repo_id: str, secret: Secret):
+        base_secrets.add_secret(self._storage, self._secrets_manager, repo_id, secret)
 
-    def update_secret(self, repo_address: RepoAddress, secret: Secret):
-        base_secrets.update_secret(
-            self._storage,
-            self._secrets_manager,
-            repo_address,
-            secret,
-        )
+    def update_secret(self, repo_id: str, secret: Secret):
+        base_secrets.update_secret(self._storage, self._secrets_manager, repo_id, secret)
 
-    def delete_secret(self, repo_address: RepoAddress, secret_name: str):
-        base_secrets.delete_secret(
-            self._storage,
-            self._secrets_manager,
-            repo_address,
-            secret_name,
-        )
+    def delete_secret(self, repo_id: str, secret_name: str):
+        base_secrets.delete_secret(self._storage, self._secrets_manager, repo_id, secret_name)
 
     def get_signed_download_url(self, object_key: str) -> str:
         return self._storage.get_signed_download_url(object_key)
 
     def get_signed_upload_url(self, object_key: str) -> str:
         return self._storage.get_signed_upload_url(object_key)
 
-    def get_configurator(self):
-        return GCPConfigurator()
-
-    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
-        base_cache.delete_workflow_cache(self._storage, repo_address, username, workflow_name)
+    def delete_workflow_cache(self, repo_id: str, hub_user_name: str, workflow_name: str):
+        base_cache.delete_workflow_cache(self._storage, repo_id, hub_user_name, workflow_name)
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/gcp/compute.py` & `dstack-0.8/cli/dstack/backend/gcp/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,35 @@
 
 DSTACK_INSTANCE_TAG = "dstack-runner-instance"
 
 
 _supported_accelerators = [
     {"accelerator_name": "nvidia-a100-80gb", "gpu_name": "A100", "memory_mb": 1024 * 80},
     {"accelerator_name": "nvidia-tesla-a100", "gpu_name": "A100", "memory_mb": 1024 * 40},
-    {"accelerator_name": "nvidia-tesla-v100", "gpu_name": "V100", "memory_mb": 1024 * 16},
-    {"accelerator_name": "nvidia-tesla-p100", "gpu_name": "P100", "memory_mb": 1024 * 16},
-    {"accelerator_name": "nvidia-tesla-k80", "gpu_name": "K80", "memory_mb": 1024 * 12},
+    {
+        "accelerator_name": "nvidia-tesla-v100",
+        "gpu_name": "V100",
+        "memory_mb": 1024 * 16,
+        "max_vcpu": 12,
+        "max_ram_mb": 1024 * 78,
+    },
+    {
+        "accelerator_name": "nvidia-tesla-p100",
+        "gpu_name": "P100",
+        "memory_mb": 1024 * 16,
+        "max_vcpu": 16,
+        "max_ram_mb": 1024 * 104,
+    },
+    {
+        "accelerator_name": "nvidia-tesla-k80",
+        "gpu_name": "K80",
+        "memory_mb": 1024 * 12,
+        "max_vcpu": 8,
+        "max_ram_mb": 1024 * 52,
+    },
 ]
 
 
 class GCPCompute(Compute):
     def __init__(
         self,
         gcp_config: GCPConfig,
@@ -313,14 +331,21 @@
         accelerator_types_client=accelerator_types_client,
         project_id=project_id,
         zone=zone,
         accelerator_families=["nvidia-tesla-v100", "nvidia-tesla-k80", "nvidia-tesla-p100"],
     )
     for at in accelerator_types:
         for gpu_count in range(1, at.maximum_cards_per_instance):
+            max_vcpu = _get_max_vcpu_per_accelerator(at.name) * gpu_count
+            max_ram_mb = _get_max_ram_per_accelerator(at.name) * gpu_count
+            if (
+                max_vcpu < instance_type.resources.cpus
+                or max_ram_mb < instance_type.resources.memory_mib
+            ):
+                continue
             instance_types.append(
                 InstanceType(
                     instance_name=instance_type.instance_name,
                     resources=Resources(
                         cpus=instance_type.resources.cpus,
                         memory_mib=instance_type.resources.memory_mib,
                         interruptible=instance_type.resources.interruptible,
@@ -362,14 +387,26 @@
 
 def _gpu_to_accelerator_name(gpu: Gpu) -> str:
     for acc in _supported_accelerators:
         if acc["gpu_name"] == gpu.name and acc["memory_mb"] == gpu.memory_mib:
             return acc["accelerator_name"]
 
 
+def _get_max_vcpu_per_accelerator(accelerator_name: str) -> int:
+    for acc in _supported_accelerators:
+        if acc["accelerator_name"] == accelerator_name:
+            return acc["max_vcpu"]
+
+
+def _get_max_ram_per_accelerator(accelerator_name: str) -> int:
+    for acc in _supported_accelerators:
+        if acc["accelerator_name"] == accelerator_name:
+            return acc["max_ram_mb"]
+
+
 def _get_image_name(
     images_client: compute_v1.ImagesClient, instance_type: InstanceType
 ) -> Optional[str]:
     if version.__is_release__:
         image_prefix = "dstack-"
     else:
         image_prefix = "stgn-dstack-"
@@ -431,21 +468,20 @@
 
 def _get_labels(bucket: str, job: Job) -> Dict[str, str]:
     labels = {
         "owner": "dstack",
     }
     if gcp_utils.is_valid_label_value(bucket):
         labels["dstack_bucket"] = bucket
-    dstack_repo = job.repo_address.path("-").lower().replace(".", "-")
+    dstack_repo = job.repo.repo_id.lower().replace(".", "-")
     if gcp_utils.is_valid_label_value(dstack_repo):
         labels["dstack_repo"] = dstack_repo
-    if job.local_repo_user_name is not None:
-        dstack_user_name = job.local_repo_user_name.lower().replace(" ", "_")
-        if gcp_utils.is_valid_label_value(dstack_user_name):
-            labels["dstack_user_name"] = dstack_user_name
+    dstack_user_name = job.hub_user_name.lower().replace(" ", "_")
+    if gcp_utils.is_valid_label_value(dstack_user_name):
+        labels["dstack_user_name"] = dstack_user_name
     return labels
 
 
 def _launch_instance(
     instances_client: compute_v1.InstancesClient,
     firewalls_client: compute_v1.FirewallsClient,
     project_id: str,
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/gcp/logs.py` & `dstack-0.8/cli/dstack/backend/gcp/logs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,77 @@
-import time
 from datetime import datetime
 from typing import Dict, Generator, Optional
 
 from google.cloud import logging
 from google.oauth2 import service_account
 
 from dstack.backend.base import jobs
 from dstack.backend.base.logs import fix_urls
 from dstack.backend.base.storage import Storage
 from dstack.core.job import Job
 from dstack.core.log_event import LogEvent, LogEventSource
-from dstack.core.repo import RepoAddress
 
-POLL_LOGS_ATTEMPTS = 5
-POLL_LOGS_WAIT_TIME = 2
+LOGS_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%f%z"
 
 
 class GCPLogging:
     def __init__(
         self, project_id: str, bucket_name: str, credentials: Optional[service_account.Credentials]
     ):
         self.project_id = project_id
         self.bucket_name = bucket_name
         self.logging_client = logging.Client(project=project_id, credentials=credentials)
 
     def poll_logs(
         self,
         storage: Storage,
-        repo_address: RepoAddress,
+        repo_id: str,
         run_name: str,
-        start_time: int,
+        start_time: datetime,
+        end_time: Optional[datetime],
+        descending: bool,
     ) -> Generator[LogEvent, None, None]:
-        log_name = _get_log_name(self.bucket_name, repo_address, run_name)
-        timestamp = datetime.fromtimestamp(start_time / 1000).strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+        log_name = _get_log_name(self.bucket_name, repo_id, run_name)
+
+        timestamp_from = start_time.strftime(LOGS_TIME_FORMAT)
+        filter = f'timestamp>="{timestamp_from}"'
+        if end_time is not None:
+            end_time_limit = end_time.replace(microsecond=end_time.microsecond + 1)
+            timestamp_to = end_time_limit.strftime(LOGS_TIME_FORMAT)
+            filter += f' AND timestamp<="{timestamp_to}"'
+
+        order_by = logging.ASCENDING
+        if descending:
+            order_by = logging.DESCENDING
+
         logger = self.logging_client.logger(log_name)
         jobs_cache = {}
-        # Hack: It takes some time for logs to become available after runner writes them.
-        # So we try reading logs multiple times.
-        # The proper solution would be for the runner to ensure logs availability before marking job as Done.
-        found_log = False
-        for _ in range(POLL_LOGS_ATTEMPTS):
-            log_entries = logger.list_entries(filter_=f'timestamp>="{timestamp}"')
-            for log_entry in log_entries:
-                found_log = True
-                yield _log_entry_to_log_event(storage, repo_address, log_entry, jobs_cache)
-            if found_log:
-                break
-            time.sleep(POLL_LOGS_WAIT_TIME)
+        log_entries = logger.list_entries(filter_=filter, order_by=order_by)
+        for log_entry in log_entries:
+            yield _log_entry_to_log_event(storage, repo_id, log_entry, jobs_cache)
 
 
-def _get_log_name(bucket_name: str, repo_address: RepoAddress, run_name) -> str:
-    return f"dstack-jobs-{bucket_name}-{repo_address.path('-')}-{run_name}"
+def _get_log_name(bucket_name: str, repo_id: str, run_name) -> str:
+    return f"dstack-jobs-{bucket_name}-{repo_id}-{run_name}"
 
 
 def _log_entry_to_log_event(
     storage: Storage,
-    repo_address: RepoAddress,
+    repo_id: str,
     log_entry: logging.LogEntry,
     jobs_cache: Dict[str, Job],
 ) -> LogEvent:
     job_id = log_entry.payload["job_id"]
     log = log_entry.payload["log"]
     job = jobs_cache.get(job_id)
     if job is None:
-        job = jobs.get_job(storage, repo_address, job_id)
+        job = jobs.get_job(storage, repo_id, job_id)
         jobs_cache[job_id] = job
     log = fix_urls(log.encode(), job, {}).decode()
-    timestamp = int(log_entry.timestamp.timestamp())
+    timestamp = log_entry.timestamp
     return LogEvent(
         event_id=log_entry.insert_id,
         timestamp=timestamp,
         job_id=job_id,
         log_message=log,
         log_source=LogEventSource.STDOUT
         if log_entry.payload["source"] == "stdout"
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/gcp/secrets.py` & `dstack-0.8/cli/dstack/backend/gcp/secrets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,80 @@
-from typing import List, Optional
+from typing import Optional
 
 from google.api_core import exceptions
 from google.cloud import secretmanager
 from google.oauth2 import service_account
 
 from dstack.backend.base.secrets import SecretsManager
-from dstack.core.repo import RepoAddress
 from dstack.core.secret import Secret
 
 
 class GCPSecretsManager(SecretsManager):
     def __init__(
-        self, project_id: str, bucket_name: str, credentials: Optional[service_account.Credentials]
+        self,
+        project_id: str,
+        bucket_name: str,
+        credentials: Optional[service_account.Credentials],
     ):
         self.project_id = project_id
         self.bucket_name = bucket_name
         self.secrets_client = secretmanager.SecretManagerServiceClient(credentials=credentials)
 
-    def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
+    def get_secret(self, repo_id: str, secret_name: str) -> Optional[Secret]:
         secret_value = self._get_secret_value(
-            _get_secret_key(self.bucket_name, repo_address, secret_name)
+            _get_secret_key(self.bucket_name, repo_id, secret_name)
         )
         if secret_value is None:
             return None
         return Secret(secret_name=secret_name, secret_value=secret_value)
 
-    def add_secret(self, repo_address: RepoAddress, secret: Secret):
-        secret_key = _get_secret_key(self.bucket_name, repo_address, secret.secret_name)
+    def add_secret(self, repo_id: str, secret: Secret):
+        secret_key = _get_secret_key(self.bucket_name, repo_id, secret.secret_name)
         self._create_secret(secret_key)
         self._add_secret_version(
             secret_key=secret_key,
             secret_value=secret.secret_value,
         )
 
-    def update_secret(self, repo_address: RepoAddress, secret: Secret):
+    def update_secret(self, repo_id: str, secret: Secret):
         self._add_secret_version(
-            secret_key=_get_secret_key(self.bucket_name, repo_address, secret.secret_name),
+            secret_key=_get_secret_key(self.bucket_name, repo_id, secret.secret_name),
             secret_value=secret.secret_value,
         )
 
-    def delete_secret(self, repo_address: RepoAddress, secret_name: str):
+    def delete_secret(self, repo_id: str, secret_name: str):
         secret_resource = _get_secret_resource(
-            self.project_id, _get_secret_key(self.bucket_name, repo_address, secret_name)
+            self.project_id, _get_secret_key(self.bucket_name, repo_id, secret_name)
         )
         self.secrets_client.delete_secret(request={"name": secret_resource})
 
-    def get_credentials(self, repo_address: RepoAddress) -> Optional[str]:
-        return self._get_secret_value(_get_credentials_key(self.bucket_name, repo_address))
+    def get_credentials(self, repo_id: str) -> Optional[str]:
+        return self._get_secret_value(_get_credentials_key(self.bucket_name, repo_id))
 
-    def add_credentials(self, repo_address: RepoAddress, data: str):
-        credentails_key = _get_credentials_key(self.bucket_name, repo_address)
+    def add_credentials(self, repo_id: str, data: str):
+        credentails_key = _get_credentials_key(self.bucket_name, repo_id)
         self._create_secret(credentails_key)
         self._add_secret_version(
             secret_key=credentails_key,
             secret_value=data,
         )
 
-    def update_credentials(self, repo_address: RepoAddress, data: str):
+    def update_credentials(self, repo_id: str, data: str):
         self._add_secret_version(
-            secret_key=_get_credentials_key(self.bucket_name, repo_address),
+            secret_key=_get_credentials_key(self.bucket_name, repo_id),
             secret_value=data,
         )
 
     def _get_secret_value(self, secret_key: str) -> Optional[str]:
         secret_version_resource = _get_secret_version_resource(self.project_id, secret_key)
         try:
             response = self.secrets_client.access_secret_version(name=secret_version_resource)
         except exceptions.NotFound:
             return None
-        return response.payload.data
+        return response.payload.data.decode()
 
     def _create_secret(self, secret_key: str):
         try:
             self.secrets_client.create_secret(
                 parent=_get_project_resource(self.project_id),
                 secret_id=secret_key,
                 secret={"replication": {"automatic": {}}},
@@ -96,17 +98,17 @@
 
 
 def _get_secret_version_resource(project_id: str, secret_key: str) -> str:
     secret_resource = _get_secret_resource(project_id, secret_key)
     return f"{secret_resource}/versions/latest"
 
 
-def _get_secret_key(bucket_name: str, repo_address: RepoAddress, secret_name: str) -> str:
-    key = f"dstack-secrets-{bucket_name}-{repo_address.path(delimiter='-')}-{secret_name}"
+def _get_secret_key(bucket_name: str, repo_id: str, secret_name: str) -> str:
+    key = f"dstack-secrets-{bucket_name}-{repo_id}-{secret_name}"
     key = key.replace(".", "-")
     return key
 
 
-def _get_credentials_key(bucket_name: str, repo_address: RepoAddress) -> str:
-    key = f"dstack-credentials-{bucket_name}-{repo_address.path(delimiter='-')}"
+def _get_credentials_key(bucket_name: str, repo_id: str) -> str:
+    key = f"dstack-credentials-{bucket_name}-{repo_id}"
     key = key.replace(".", "-")
     return key
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/gcp/storage.py` & `dstack-0.8/cli/dstack/backend/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/backend/gcp/utils.py` & `dstack-0.8/cli/dstack/backend/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/backend/hub/__init__.py` & `dstack-0.8/cli/dstack/backend/local/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,216 +1,198 @@
-import sys
-from abc import ABC
-from pathlib import Path
-from typing import Dict, Generator, List, Optional, Tuple
+from datetime import datetime
+from typing import Generator, List, Optional
 
-from dstack.backend.base import BackendType, RemoteBackend
+from dstack.backend.base import Backend
 from dstack.backend.base import artifacts as base_artifacts
-from dstack.backend.hub.client import HubClient
-from dstack.backend.hub.config import HUBConfig, HubConfigurator
-from dstack.backend.hub.storage import HUBStorage
+from dstack.backend.base import cache as base_cache
+from dstack.backend.base import jobs as base_jobs
+from dstack.backend.base import repos as base_repos
+from dstack.backend.base import runs as base_runs
+from dstack.backend.base import secrets as base_secrets
+from dstack.backend.base import tags as base_tags
+from dstack.backend.local import artifacts, logs
+from dstack.backend.local.compute import LocalCompute
+from dstack.backend.local.config import LocalConfig
+from dstack.backend.local.secrets import LocalSecretsManager
+from dstack.backend.local.storage import LocalStorage
 from dstack.core.artifact import Artifact
-from dstack.core.config import BackendConfig
-from dstack.core.error import ConfigError
 from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.log_event import LogEvent
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials, RepoHead
+from dstack.core.repo import RemoteRepoCredentials, RepoHead, RepoSpec
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
+from dstack.utils.common import PathLike
 
 
-class HubBackend(RemoteBackend):
-    _client = None
-    _storage = None
-
-    def __init__(self, config: Optional[BackendConfig] = None):
-        super().__init__(config)
-        self.backend_config = HUBConfig()
-        try:
-            self.backend_config.load()
-            self._loaded = True
-            self._storage = HUBStorage(self._hub_client())
-        except ConfigError:
-            self._loaded = False
-
-    def _hub_client(self) -> HubClient:
-        if self._client is None:
-            self._client = HubClient(
-                url=self.backend_config.url,
-                project=self.backend_config.project,
-                token=self.backend_config.token,
-            )
-        return self._client
-
-    @property
-    def name(self):
-        return "hub"
-
-    @property
-    def type(self) -> BackendType:
-        return BackendType.REMOTE
+class LocalBackend(Backend):
+    NAME = "local"
+    backend_config: LocalConfig
+    _storage: LocalStorage
+    _compute: LocalCompute
+    _secrets_manager: LocalSecretsManager
 
-    def configure(self):
-        pass
+    def __init__(
+        self,
+        backend_config: LocalConfig,
+    ):
+        super().__init__(backend_config=backend_config)
+        if self.backend_config is None:
+            return
+        self._storage = LocalStorage(self.backend_config.backend_dir)
+        self._compute = LocalCompute(self.backend_config)
+        self._secrets_manager = LocalSecretsManager(self.backend_config.backend_dir)
 
-    def create_run(self, repo_address: RepoAddress) -> str:
-        return self._hub_client().create_run(repo_address=repo_address)
+    def create_run(self, repo_id: str) -> str:
+        return base_runs.create_run(self._storage)
 
     def create_job(self, job: Job):
-        self._hub_client().create_job(job=job)
+        base_jobs.create_job(self._storage, job)
 
-    def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
-        return self._hub_client().get_job(repo_address=repo_address, job_id=job_id)
+    def get_job(self, repo_id: str, job_id: str) -> Optional[Job]:
+        return base_jobs.get_job(self._storage, repo_id, job_id)
 
-    def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
-        return self._hub_client().list_jobs(repo_address=repo_address, run_name=run_name)
+    def list_jobs(self, repo_id: str, run_name: str) -> List[Job]:
+        return base_jobs.list_jobs(self._storage, repo_id, run_name)
 
     def run_job(self, job: Job, failed_to_start_job_new_status: JobStatus):
-        self._hub_client().run_job(job=job)
+        base_jobs.run_job(self._storage, self._compute, job, failed_to_start_job_new_status)
 
-    def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
-        self._hub_client().stop_job(repo_address=repo_address, job_id=job_id, abort=abort)
+    def stop_job(self, repo_id: str, abort: bool, job_id: str):
+        base_jobs.stop_job(self._storage, self._compute, repo_id, job_id, abort)
 
-    def list_job_heads(
-        self, repo_address: RepoAddress, run_name: Optional[str] = None
-    ) -> List[JobHead]:
-        return self._hub_client().list_job_heads(repo_address=repo_address, run_name=run_name)
+    def list_job_heads(self, repo_id: str, run_name: Optional[str] = None) -> List[JobHead]:
+        return base_jobs.list_job_heads(self._storage, repo_id, run_name)
 
-    def delete_job_head(self, repo_address: RepoAddress, job_id: str):
-        self._hub_client().delete_job_head(repo_address=repo_address, job_id=job_id)
+    def delete_job_head(self, repo_id: str, job_id: str):
+        base_jobs.delete_job_head(self._storage, repo_id, job_id)
 
     def list_run_heads(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
         interrupted_job_new_status: JobStatus = JobStatus.FAILED,
     ) -> List[RunHead]:
-        return self._hub_client().list_run_heads(
-            repo_address=repo_address,
-            run_name=run_name,
-            include_request_heads=include_request_heads,
+        job_heads = self.list_job_heads(repo_id=repo_id, run_name=run_name)
+        return base_runs.get_run_heads(
+            self._storage,
+            self._compute,
+            job_heads,
+            include_request_heads,
+            interrupted_job_new_status,
         )
 
     def poll_logs(
         self,
-        repo_address: RepoAddress,
-        job_heads: List[JobHead],
-        start_time: int,
-        attached: bool,
+        repo_id: str,
+        run_name: str,
+        start_time: datetime,
+        end_time: Optional[datetime] = None,
+        descending: bool = False,
     ) -> Generator[LogEvent, None, None]:
-        # /{hub_name}/logs/poll
-        return self._hub_client().poll_logs(
-            repo_address=repo_address,
-            job_heads=job_heads,
-            start_time=start_time,
-            attached=attached,
+        return logs.poll_logs(
+            self.backend_config, self._storage, repo_id, run_name, start_time, end_time, descending
         )
 
-    def list_run_artifact_files(self, repo_address: RepoAddress, run_name: str) -> List[Artifact]:
-        # /{hub_name}/artifacts/list
-        return self._hub_client().list_run_artifact_files(
-            repo_address=repo_address, run_name=run_name
-        )
+    def list_run_artifact_files(self, repo_id: str, run_name: str) -> List[Artifact]:
+        return base_artifacts.list_run_artifact_files(self._storage, repo_id, run_name)
 
     def download_run_artifact_files(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         run_name: str,
-        output_dir: Optional[str],
-        files_path: Optional[str] = None,
+        output_dir: Optional[PathLike],
+        files_path: Optional[PathLike] = None,
     ):
-        # /{hub_name}/artifacts/download
-        artifacts = self.list_run_artifact_files(repo_address=repo_address, run_name=run_name)
+        list_artifacts = self.list_run_artifact_files(repo_id, run_name)
         base_artifacts.download_run_artifact_files(
             storage=self._storage,
-            repo_address=repo_address,
-            artifacts=artifacts,
+            repo_id=repo_id,
+            artifacts=list_artifacts,
             output_dir=output_dir,
             files_path=files_path,
         )
 
     def upload_job_artifact_files(
         self,
-        repo_address: RepoAddress,
+        repo_id: str,
         job_id: str,
         artifact_name: str,
-        artifact_path: str,
-        local_path: Path,
+        artifact_path: PathLike,
+        local_path: PathLike,
     ):
-        # /{hub_name}/artifacts/upload
         base_artifacts.upload_job_artifact_files(
             storage=self._storage,
-            repo_address=repo_address,
+            repo_id=repo_id,
             job_id=job_id,
             artifact_name=artifact_name,
             artifact_path=artifact_path,
             local_path=local_path,
         )
 
-    def list_tag_heads(self, repo_address: RepoAddress) -> List[TagHead]:
-        return self._hub_client().list_tag_heads(repo_address=repo_address)
+    def list_tag_heads(self, repo_id: str) -> List[TagHead]:
+        return base_tags.list_tag_heads(self._storage, repo_id)
 
-    def get_tag_head(self, repo_address: RepoAddress, tag_name: str) -> Optional[TagHead]:
-        return self._hub_client().get_tag_head(repo_address=repo_address, tag_name=tag_name)
+    def get_tag_head(self, repo_id: str, tag_name: str) -> Optional[TagHead]:
+        return base_tags.get_tag_head(self._storage, repo_id, tag_name)
 
     def add_tag_from_run(
-        self,
-        repo_address: RepoAddress,
-        tag_name: str,
-        run_name: str,
-        run_jobs: Optional[List[Job]],
+        self, repo_id: str, tag_name: str, run_name: str, run_jobs: Optional[List[Job]]
     ):
-        return self._hub_client().add_tag_from_run(
-            repo_address=repo_address, tag_name=tag_name, run_name=run_name, run_jobs=run_jobs
+        base_tags.create_tag_from_run(
+            self._storage,
+            repo_id,
+            tag_name,
+            run_name,
+            run_jobs,
         )
 
-    def add_tag_from_local_dirs(
-        self, repo_data: LocalRepoData, tag_name: str, local_dirs: List[str]
-    ):
-        # /{hub_name}/tags/add
-        return self._hub_client().add_tag_from_local_dirs(
-            repo_data=repo_data, tag_name=tag_name, local_dirs=local_dirs
-        )
+    def add_tag_from_local_dirs(self, tag_name: str, local_dirs: List[str]):
+        # base_tags.create_tag_from_local_dirs(
+        #     self._storage,
+        #     self.repo,
+        #     tag_name,
+        #     local_dirs,
+        # )
+        raise NotImplementedError()
 
-    def delete_tag_head(self, repo_address: RepoAddress, tag_head: TagHead):
-        # /{hub_name}/tags/delete
-        return self._hub_client().delete_tag_head(repo_address=repo_address, tag_head=tag_head)
-
-    def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
-        # /{hub_name}/repos/update
-        return self._hub_client().update_repo_last_run_at(
-            repo_address=repo_address, last_run_at=last_run_at
-        )
+    def delete_tag_head(self, repo_id: str, tag_head: TagHead):
+        base_tags.delete_tag(self._storage, repo_id, tag_head)
 
-    def get_repo_credentials(self, repo_address: RepoAddress) -> Optional[RepoCredentials]:
-        return self._hub_client().get_repos_credentials(repo_address=repo_address)
+    def list_repo_heads(self) -> List[RepoHead]:
+        return base_repos.list_repo_heads(self._storage)
 
-    def save_repo_credentials(self, repo_address: RepoAddress, repo_credentials: RepoCredentials):
-        self._hub_client().save_repos_credentials(
-            repo_address=repo_address, repo_credentials=repo_credentials
-        )
+    def update_repo_last_run_at(self, repo_spec: RepoSpec, last_run_at: int):
+        base_repos.update_repo_last_run_at(self._storage, repo_spec, last_run_at)
 
-    def list_secret_names(self, repo_address: RepoAddress) -> List[str]:
-        return self._hub_client().list_secret_names(repo_address=repo_address)
+    def get_repo_credentials(self, repo_id: str) -> Optional[RemoteRepoCredentials]:
+        return base_repos.get_repo_credentials(self._secrets_manager, repo_id)
 
-    def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
-        return self._hub_client().get_secret(repo_address=repo_address, secret_name=secret_name)
+    def save_repo_credentials(self, repo_id: str, repo_credentials: RemoteRepoCredentials):
+        base_repos.save_repo_credentials(self._secrets_manager, repo_id, repo_credentials)
 
-    def add_secret(self, repo_address: RepoAddress, secret: Secret):
-        self._hub_client().add_secret(repo_address=repo_address, secret=secret)
+    def list_secret_names(self, repo_id: str) -> List[str]:
+        return base_secrets.list_secret_names(self._storage, repo_id)
 
-    def update_secret(self, repo_address: RepoAddress, secret: Secret):
-        self._hub_client().update_secret(repo_address=repo_address, secret=secret)
+    def get_secret(self, repo_id: str, secret_name: str) -> Optional[Secret]:
+        return base_secrets.get_secret(self._secrets_manager, repo_id, secret_name)
 
-    def delete_secret(self, repo_address: RepoAddress, secret_name: str):
-        # /{hub_name}/secrets/delete
-        self._hub_client().delete_secret(repo_address=repo_address, secret_name=secret_name)
+    def add_secret(self, repo_id: str, secret: Secret):
+        base_secrets.add_secret(self._storage, self._secrets_manager, repo_id, secret)
 
-    def get_configurator(self):
-        return HubConfigurator()
+    def update_secret(self, repo_id: str, secret: Secret):
+        base_secrets.update_secret(self._storage, self._secrets_manager, repo_id, secret)
 
-    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
-        self._hub_client().delete_workflow_cache(
-            repo_address=repo_address, username=username, workflow_name=workflow_name
-        )
+    def delete_secret(self, repo_id: str, secret_name: str):
+        base_secrets.delete_secret(self._storage, self._secrets_manager, repo_id, secret_name)
+
+    def delete_workflow_cache(self, repo_id: str, hub_user_name: str, workflow_name: str):
+        base_cache.delete_workflow_cache(self._storage, repo_id, hub_user_name, workflow_name)
+
+    def get_signed_download_url(self, object_key: str) -> str:
+        # Implemented by Hub
+        raise NotImplementedError()
+
+    def get_signed_upload_url(self, object_key: str) -> str:
+        # Implemented by Hub
+        raise NotImplementedError()
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/hub/client.py` & `dstack-0.8/cli/dstack/api/hub/_api_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,758 +1,644 @@
-import json
+from datetime import datetime
 from typing import Dict, Generator, List, Optional
 from urllib.parse import urlencode, urlparse, urlunparse
 
 import requests
 
+from dstack.api.hub.errors import HubClientError
 from dstack.core.artifact import Artifact
+from dstack.core.error import NoMatchingInstanceError
 from dstack.core.job import Job, JobHead
 from dstack.core.log_event import LogEvent
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials
+from dstack.core.repo import RemoteRepoCredentials, Repo, RepoHead, RepoSpec
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
 from dstack.hub.models import (
     AddTagPath,
     AddTagRun,
+    JobHeadList,
     JobsGet,
     JobsList,
-    LinkUpload,
     PollLogs,
+    ProjectInfo,
     ReposUpdate,
     RunsList,
     SaveRepoCredentials,
     SecretAddUpdate,
     StopRunners,
-    UserRepoAddress,
+    StorageLink,
 )
 
 
-def _url(url: str, project: str, additional_path: str, query: dict = {}):
-    unparse_url = urlparse(url=url)
-    if additional_path.startswith("/"):
-        additional_path = additional_path[1:]
-
-    new_url = urlunparse(
-        (
-            unparse_url.scheme,
-            unparse_url.netloc,
-            f"/api/project/{project}/{additional_path}",
-            None,
-            urlencode(query=query),
-            unparse_url.fragment,
-        )
-    )
-    return new_url
-
-
-class HubClient:
-    def __init__(self, url: str, project: str, token: str):
+class HubAPIClient:
+    def __init__(self, url: str, project: str, token: str, repo: Optional[Repo]):
         self.url = url
         self.token = token
         self.project = project
-
-    @staticmethod
-    def validate(url: str, project: str, token: str) -> bool:
-        url = _url(url=url, project=project, additional_path="/info")
-        try:
-            resp = requests.get(url=url, headers=HubClient._auth(token=token))
-            if resp.ok:
-                print(resp.json())
-                return True
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return False
-        except requests.ConnectionError:
-            print(f"{url} connection refused")
-        return False
+        self.repo = repo
 
     @staticmethod
     def _auth(token: str) -> Dict[str, str]:
         if token == "":
             return {}
         headers = {"Authorization": f"Bearer {token}"}
         return headers
 
     def _headers(self):
-        headers = HubClient._auth(token=self.token)
+        headers = HubAPIClient._auth(token=self.token)
         headers["Content-type"] = "application/json"
         return headers
 
-    def get_repos_credentials(self, repo_address: RepoAddress) -> Optional[RepoCredentials]:
-        url = _url(
+    def get_project_info(self) -> ProjectInfo:
+        resp = _make_hub_request(
+            requests.get,
+            host=self.url,
+            url=f"{self.url}/api/projects/{self.project}",
+            headers=self._headers(),
+        )
+        if resp.ok:
+            return ProjectInfo.parse_obj(resp.json())
+        resp.raise_for_status()
+
+    def create_run(self) -> str:
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/repos/credentials/get",
+            additional_path=f"/runs/create",
         )
-        try:
-            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
-            if resp.ok:
-                json_data = resp.json()
-                return RepoCredentials(**json_data)
-            elif resp.status_code == 404:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=self.repo.repo_ref.json(),
+        )
+        if resp.ok:
+            return resp.text
+        resp.raise_for_status()
 
-    def save_repos_credentials(self, repo_address: RepoAddress, repo_credentials: RepoCredentials):
-        url = _url(
+    def create_job(self, job: Job):
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/repos/credentials/save",
+            additional_path=f"/jobs/create",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=SaveRepoCredentials(
-                    repo_address=repo_address,
-                    repo_credentials=repo_credentials,
-                ).json(),
-            )
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post, host=self.url, url=url, headers=self._headers(), data=job.json()
+        )
+        resp.raise_for_status()
+        job.hub_user_name = resp.json()["hub_user_name"]
 
-    def create_run(self, repo_address: RepoAddress) -> str:
-        url = _url(
+    def get_job(self, job_id: str) -> Optional[Job]:
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/runs/create",
+            additional_path=f"/jobs/get",
         )
-        try:
-            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
-            if resp.ok:
-                return resp.text
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return ""
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return ""
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=JobsGet(
+                repo_id=self.repo.repo_id,
+                job_id=job_id,
+            ).json(),
+        )
+        if resp.ok:
+            json_data = resp.json()
+            return Job.parse_obj(json_data)
+        resp.raise_for_status()
 
-    def create_job(self, job: Job):
-        url = _url(
+    def list_jobs(self, run_name: str) -> List[Job]:
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/jobs/create",
+            additional_path=f"/jobs/list",
         )
-        try:
-            resp = requests.post(url=url, headers=self._headers(), data=job.json())
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=JobsList(repo_id=self.repo.repo_id, run_name=run_name).json(),
+        )
+        if resp.ok:
+            body = resp.json()
+            return [Job.parse_obj(job) for job in body]
+        resp.raise_for_status()
 
     def run_job(self, job: Job):
-        url = _url(
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/runners/run",
         )
-        try:
-            resp = requests.post(url=url, headers=self._headers(), data=job.json())
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post, host=self.url, url=url, headers=self._headers(), data=job.json()
+        )
+        if resp.ok:
+            return
+        elif resp.status_code == 400:
+            body = resp.json()
+            if body["detail"]["code"] == NoMatchingInstanceError.code:
+                raise HubClientError(body["detail"]["msg"])
+        resp.raise_for_status()
 
-    def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
-        url = _url(
+    def stop_job(self, job_id: str, abort: bool):
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/runners/stop",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=StopRunners(
-                    repo_address=repo_address,
-                    job_id=job_id,
-                    abort=abort,
-                ).json(),
-            )
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=StopRunners(
+                repo_id=self.repo.repo_id,
+                job_id=job_id,
+                abort=abort,
+            ).json(),
+        )
+        if resp.ok:
+            return
+        resp.raise_for_status()
+
+    def list_job_heads(self, run_name: Optional[str] = None) -> Optional[List[JobHead]]:
+        url = _project_url(url=self.url, project=self.project, additional_path=f"/jobs/list/heads")
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=JobHeadList(repo_id=self.repo.repo_id, run_name=run_name).json(),
+        )
+        if resp.ok:
+            body = resp.json()
+            return [JobHead.parse_obj(job) for job in body]
+        resp.raise_for_status()
 
-    def get_tag_head(self, repo_address: RepoAddress, tag_name: str) -> Optional[TagHead]:
-        url = _url(
+    def delete_job_head(self, job_id: str):
+        url = _project_url(
+            url=self.url,
+            project=self.project,
+            additional_path=f"/jobs/delete",
+        )
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=JobsGet(repo_id=self.repo.repo_id, job_id=job_id).json(),
+        )
+        if resp.ok:
+            return
+        resp.raise_for_status()
+
+    def get_tag_head(self, tag_name: str) -> Optional[TagHead]:
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/tags/{tag_name}",
         )
-        try:
-            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
-            if resp.ok:
-                return TagHead.parse_obj(resp.json())
-            elif resp.status_code == 404:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=self.repo.repo_ref.json(),
+        )
+        if resp.ok:
+            return TagHead.parse_obj(resp.json())
+        elif resp.status_code == 404:
+            return None
+        resp.raise_for_status()
 
-    def list_tag_heads(self, repo_address: RepoAddress) -> Optional[List[TagHead]]:
-        url = _url(
+    def list_tag_heads(self) -> Optional[List[TagHead]]:
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/tags/list/heads",
         )
-        try:
-            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
-            if resp.ok:
-                body = resp.json()
-                return [TagHead.parse_obj(tag) for tag in body]
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=self.repo.repo_ref.json(),
+        )
+        if resp.ok:
+            body = resp.json()
+            return [TagHead.parse_obj(tag) for tag in body]
+        resp.raise_for_status()
 
     def add_tag_from_run(
         self,
-        repo_address: RepoAddress,
         tag_name: str,
         run_name: str,
         run_jobs: Optional[List[Job]],
     ):
-        url = _url(
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/tags/add/run",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=AddTagRun(
-                    repo_address=repo_address,
-                    tag_name=tag_name,
-                    run_name=run_name,
-                    run_jobs=run_jobs,
-                ).json(),
-            )
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=AddTagRun(
+                repo_id=self.repo.repo_id,
+                tag_name=tag_name,
+                run_name=run_name,
+                run_jobs=run_jobs,
+            ).json(),
+        )
+        if resp.ok:
+            return
+        resp.raise_for_status()
 
     def add_tag_from_local_dirs(
         self,
-        repo_data: LocalRepoData,
         tag_name: str,
         local_dirs: List[str],
     ):
-        url = _url(
-            url=self.url,
-            project=self.project,
-            additional_path=f"/tags/add/path",
-        )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=AddTagPath(
-                    repo_data=repo_data,
-                    tag_name=tag_name,
-                    local_dirs=local_dirs,
-                ).json(),
-            )
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        # url = _project_url(
+        #     url=self.url,
+        #     project=self.project,
+        #     additional_path=f"/tags/add/path",
+        # )
+        # resp = _make_hub_request(
+        #     requests.post,
+        #     host=self.url,
+        #     url=url,
+        #     headers=self._headers(),
+        #     data=AddTagPath(
+        #         repo_spec=RepoSpec.from_repo(self.repo),
+        #         tag_name=tag_name,
+        #         local_dirs=local_dirs,
+        #     ).json(),
+        # )
+        # if resp.ok:
+        #     return
+        # resp.raise_for_status()
+        raise NotImplementedError()
 
-    def delete_tag_head(self, repo_address: RepoAddress, tag_head: TagHead):
-        url = _url(
+    def delete_tag_head(self, tag_head: TagHead):
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/tags/{tag_head.tag_name}/delete",
         )
-        try:
-            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
-
-    def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
-        url = _url(
-            url=self.url,
-            project=self.project,
-            additional_path=f"/repos/update",
-        )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=ReposUpdate(
-                    repo_address=repo_address,
-                    last_run_at=last_run_at,
-                ).json(),
-            )
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
-
-    def list_job_heads(
-        self, repo_address: RepoAddress, run_name: Optional[str] = None
-    ) -> Optional[List[JobHead]]:
-        query = {}
-        if not (run_name is None):
-            query["run_name"] = run_name
-        url = _url(
-            url=self.url, project=self.project, additional_path=f"/jobs/list/heads", query=query
-        )
-        try:
-            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
-            if resp.ok:
-                body = resp.json()
-                return [JobHead.parse_obj(job) for job in body]
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=self.repo.repo_ref.json(),
+        )
+        if resp.ok:
+            return
+        resp.raise_for_status()
 
     def list_run_heads(
         self,
-        repo_address: RepoAddress,
         run_name: Optional[str] = None,
         include_request_heads: bool = True,
     ) -> List[RunHead]:
-        url = _url(
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/runs/list",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=RunsList(
-                    repo_address=repo_address,
-                    run_name=run_name,
-                    include_request_heads=include_request_heads,
-                ).json(),
-            )
-            if resp.ok:
-                body = resp.json()
-                return [RunHead.parse_obj(run) for run in body]
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return []
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return []
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=RunsList(
+                repo_id=self.repo.repo_id,
+                run_name=run_name,
+                include_request_heads=include_request_heads,
+            ).json(),
+        )
+        if resp.ok:
+            body = resp.json()
+            return [RunHead.parse_obj(run) for run in body]
+        resp.raise_for_status()
 
-    def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
-        url = _url(
+    def update_repo_last_run_at(self, last_run_at: int):
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/jobs/get",
+            additional_path=f"/repos/update",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=JobsGet(
-                    repo_address=repo_address,
-                    job_id=job_id,
-                ).json(),
-            )
-            if resp.ok:
-                json_data = resp.json()
-                return Job.parse_obj(json_data)
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=ReposUpdate(
+                repo_spec=RepoSpec.from_repo(self.repo),
+                last_run_at=last_run_at,
+            ).json(),
+        )
+        if resp.ok:
+            return
+        resp.raise_for_status()
+
+    def list_repo_heads(self) -> List[RepoHead]:
+        url = _project_url(
+            url=self.url,
+            project=self.project,
+            additional_path=f"/repos/heads/list",
+        )
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+        )
+        if resp.ok:
+            return [RepoHead.parse_obj(e) for e in resp.json()]
+        resp.raise_for_status()
 
-    def list_secret_names(self, repo_address: RepoAddress) -> List[str]:
-        url = _url(
+    def get_repos_credentials(self) -> Optional[RemoteRepoCredentials]:
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/secrets/list",
+            additional_path=f"/repos/credentials/get",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=repo_address.json(),
-            )
-            if resp.ok:
-                json_data = resp.json()
-                return json_data
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return []
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return []
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=self.repo.repo_ref.json(),
+        )
+        if resp.ok:
+            json_data = resp.json()
+            return RemoteRepoCredentials(**json_data)
+        elif resp.status_code == 404:
+            return None
+        resp.raise_for_status()
 
-    def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
-        url = _url(
+    def save_repos_credentials(self, repo_credentials: RemoteRepoCredentials):
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/secrets/{secret_name}/get",
+            additional_path=f"/repos/credentials/save",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=repo_address.json(),
-            )
-            if resp.ok:
-                json_data = resp.json()
-                return Secret.parse_obj(json_data)
-            elif resp.status_code == 404:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=SaveRepoCredentials(
+                repo_id=self.repo.repo_id,
+                repo_credentials=repo_credentials,
+            ).json(),
+        )
+        if resp.ok:
+            return resp.text
+        resp.raise_for_status()
 
-    def add_secret(self, repo_address: RepoAddress, secret: Secret):
-        url = _url(
+    def list_secret_names(self) -> List[str]:
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/secrets/add",
+            additional_path=f"/secrets/list",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=SecretAddUpdate(
-                    repo_address=repo_address,
-                    secret=secret,
-                ).json(),
-            )
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=self.repo.repo_ref.json(),
+        )
+        if resp.ok:
+            return resp.json()
+        resp.raise_for_status()
 
-    def update_secret(self, repo_address: RepoAddress, secret: Secret):
-        url = _url(
+    def get_secret(self, secret_name: str) -> Optional[Secret]:
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/secrets/update",
+            additional_path=f"/secrets/{secret_name}/get",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=SecretAddUpdate(
-                    repo_address=repo_address,
-                    secret=secret,
-                ).json(),
-            )
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=self.repo.repo_ref.json(),
+        )
+        if resp.ok:
+            json_data = resp.json()
+            return Secret.parse_obj(json_data)
+        elif resp.status_code == 404:
+            return None
+        resp.raise_for_status()
 
-    def delete_secret(self, repo_address: RepoAddress, secret_name: str):
-        url = _url(
+    def add_secret(self, secret: Secret):
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/secrets/{secret_name}/delete",
+            additional_path=f"/secrets/add",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=repo_address.json(),
-            )
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=SecretAddUpdate(
+                repo_id=self.repo.repo_id,
+                secret=secret,
+            ).json(),
+        )
+        if resp.ok:
+            return
+        resp.raise_for_status()
 
-    def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
-        url = _url(
+    def update_secret(self, secret: Secret):
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/jobs/list",
+            additional_path=f"/secrets/update",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=JobsList(repo_address=repo_address, run_name=run_name).json(),
-            )
-            if resp.ok:
-                job_data = resp.json()
-                return [Job.parse_obj(job) for job in job_data]
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return []
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return []
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=SecretAddUpdate(
+                repo_id=self.repo.repo_id,
+                secret=secret,
+            ).json(),
+        )
+        if resp.ok:
+            return
+        resp.raise_for_status()
 
-    def list_run_artifact_files(self, repo_address: RepoAddress, run_name: str) -> List[Artifact]:
-        url = _url(
+    def delete_secret(self, secret_name: str):
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/artifacts/list",
+            additional_path=f"/secrets/{secret_name}/delete",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=JobsList(repo_address=repo_address, run_name=run_name).json(),
-            )
-            if resp.ok:
-                artifact_data = resp.json()
-                return [Artifact.parse_obj(artifact) for artifact in artifact_data]
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return []
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return []
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=self.repo.repo_ref.json(),
+        )
+        if resp.ok:
+            return
+        resp.raise_for_status()
 
-    def delete_job_head(self, repo_address: RepoAddress, job_id: str):
-        url = _url(
+    def list_run_artifact_files(self, run_name: str) -> List[Artifact]:
+        url = _project_url(
             url=self.url,
             project=self.project,
-            additional_path=f"/jobs/delete",
+            additional_path=f"/artifacts/list",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=JobsGet(repo_address=repo_address, job_id=job_id).json(),
-            )
-            if resp.ok:
-                return None
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=JobsList(repo_id=self.repo.repo_id, run_name=run_name).json(),
+        )
+        if resp.ok:
+            artifact_data = resp.json()
+            return [Artifact.parse_obj(artifact) for artifact in artifact_data]
+        resp.raise_for_status()
 
     def poll_logs(
         self,
-        repo_address: RepoAddress,
-        job_heads: List[JobHead],
-        start_time: int,
-        attached: bool,
+        run_name: str,
+        start_time: datetime,
+        end_time: Optional[datetime],
+        descending: bool,
     ) -> Generator[LogEvent, None, None]:
-        url = _url(
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/logs/poll",
         )
-        try:
-            resp = requests.post(
+        prev_event_id = None
+        while True:
+            resp = _make_hub_request(
+                requests.post,
+                host=self.url,
                 url=url,
                 headers=self._headers(),
                 data=PollLogs(
-                    repo_address=repo_address,
-                    job_heads=job_heads,
-                    start_time=start_time,
-                    attached=attached,
+                    repo_id=self.repo.repo_id,
+                    run_name=run_name,
+                    start_time=start_time.isoformat(),
+                    end_time=end_time.isoformat() if end_time else None,
+                    descending=descending,
+                    prev_event_id=prev_event_id,
                 ).json(),
-                stream=True,
             )
-            if resp.ok:
-                _braces = 0
-                _body = bytearray()
-                for chunk in resp.iter_content(chunk_size=128):
-                    for b in chunk:
-                        if b == 123:
-                            _braces += 1
-                        elif b == 125:
-                            _braces -= 1
-                        _body.append(b)
-
-                        if _braces == 0:
-                            json_data = json.loads(_body)
-                            _body = bytearray()
-                            yield LogEvent.parse_obj(json_data)
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
+            if not resp.ok:
                 resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+            body = resp.json()
+            logs = [LogEvent.parse_obj(e) for e in body]
+            if len(logs) == 0:
+                return
+            yield from logs
+            if descending:
+                end_time = logs[-1].timestamp
+            else:
+                start_time = logs[-1].timestamp
+            prev_event_id = logs[-1].event_id
 
     def upload_file(self, dest_path: str) -> Optional[str]:
-        url = _url(
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/link/upload",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=LinkUpload(object_key=dest_path).json(),
-            )
-            if resp.ok:
-                return resp.text
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=StorageLink(object_key=dest_path).json(),
+        )
+        if resp.ok:
+            return resp.text
+        resp.raise_for_status()
 
     def download_file(self, dest_path: str) -> Optional[str]:
-        url = _url(
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/link/download",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=LinkUpload(object_key=dest_path).json(),
-            )
-            if resp.ok:
-                return resp.text
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return None
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
-        return None
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=StorageLink(object_key=dest_path).json(),
+        )
+        if resp.ok:
+            return resp.text
+        resp.raise_for_status()
 
-    def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
-        url = _url(
+    def delete_workflow_cache(self, workflow_name: str):
+        url = _project_url(
             url=self.url,
             project=self.project,
             additional_path=f"/workflows/{workflow_name}/cache/delete",
         )
-        try:
-            resp = requests.post(
-                url=url,
-                headers=self._headers(),
-                data=UserRepoAddress(username=username, repo_address=repo_address).json(),
-            )
-            if resp.ok:
-                return
-            elif resp.status_code == 401:
-                print("Unauthorized. Please set correct token")
-                return
-            else:
-                resp.raise_for_status()
-        except requests.ConnectionError:
-            print(f"{self.url} connection refused")
+        resp = _make_hub_request(
+            requests.post,
+            host=self.url,
+            url=url,
+            headers=self._headers(),
+            data=RepoSpec.from_repo(self.repo).json(),
+        )
+        if resp.ok:
+            return
+        resp.raise_for_status()
+
+
+def _project_url(url: str, project: str, additional_path: str, query: Optional[dict] = None):
+    query = {} if query is None else query
+    unparse_url = urlparse(url=url)
+    if additional_path.startswith("/"):
+        additional_path = additional_path[1:]
+    new_url = urlunparse(
+        (
+            unparse_url.scheme,
+            unparse_url.netloc,
+            f"/api/project/{project}/{additional_path}",
+            None,
+            urlencode(query=query),
+            unparse_url.fragment,
+        )
+    )
+    return new_url
+
+
+def _make_hub_request(request_func, host, *args, **kwargs) -> requests.Response:
+    try:
+        resp: requests.Response = request_func(*args, **kwargs)
+        if resp.status_code == 401:
+            raise HubClientError(f"Invalid hub token")
+        elif resp.status_code == 500:
+            url = kwargs.get("url")
+            raise HubClientError(
+                f"Got 500 Server Error from hub: {url}. Check hub logs for details."
+            )
+        return resp
+    except requests.ConnectionError:
+        raise HubClientError(f"Cannot connect to hub at {host}")
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/hub/storage.py` & `dstack-0.8/cli/dstack/api/hub/_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
 from abc import ABC
 from typing import Callable, Dict, List, Optional
 
 import requests
 
+from dstack.api.hub._api_client import HubAPIClient
 from dstack.backend.base.storage import SIGNED_URL_EXPIRATION, CloudStorage
-from dstack.backend.hub.client import HubClient
 from dstack.core.storage import StorageFile
 
 
 class HUBStorage(CloudStorage, ABC):
-    def __init__(self, _client: HubClient):
+    def __init__(self, _client: HubAPIClient):
         self._client = _client
 
     def upload_file(self, source_path: str, dest_path: str, callback: Callable[[int], None]):
         url = self._client.upload_file(dest_path=dest_path)
         if not (url is None):
             with open(source_path, "rb") as f:
-                resp = requests.put(url, data=f)
+                # AWS: requests.put() produces bad headers from empty file descriptor
+                resp = requests.put(url, data=f if os.stat(source_path).st_size > 0 else None)
                 if resp.ok:
                     file_stat = os.stat(source_path)
                     callback(file_stat.st_size)
 
     def download_file(self, source_path: str, dest_path: str, callback: Callable[[int], None]):
         url = self._client.download_file(dest_path=source_path)
         if not (url is None):
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/local/compute.py` & `dstack-0.8/cli/dstack/backend/local/compute.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-from typing import Optional, Tuple
+from typing import Optional
 
 from dstack.backend.base.compute import Compute
 from dstack.backend.local import runners
+from dstack.backend.local.config import LocalConfig
 from dstack.core.instance import InstanceType
-from dstack.core.job import Job, Requirements
+from dstack.core.job import Job
 from dstack.core.request import RequestHead
 
 
 class LocalCompute(Compute):
+    def __init__(self, backend_config: LocalConfig):
+        self.backend_config = backend_config
+
     def get_request_head(self, job: Job, request_id: Optional[str]) -> RequestHead:
         return runners.get_request_head(job, request_id)
 
     def get_instance_type(self, job: Job) -> Optional[InstanceType]:
-        resources = runners.check_runner_resources(job.runner_id)
+        resources = runners.check_runner_resources(self.backend_config, job.runner_id)
         return InstanceType(instance_name="local_runner", resources=resources)
 
     def run_instance(self, job: Job, instance_type: InstanceType) -> str:
-        return runners.start_runner_process(job.runner_id)
+        return runners.start_runner_process(self.backend_config, job.runner_id)
 
     def terminate_instance(self, request_id: str):
         runners.stop_process(request_id)
 
     def cancel_spot_request(self, request_id: str):
         runners.stop_process(request_id)
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/local/runners.py` & `dstack-0.8/cli/dstack/backend/local/runners.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import os
 import platform
 import shutil
 import signal
 import subprocess
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import Optional
 
 import cpuinfo
 import psutil
 import requests
 import yaml
 from psutil import NoSuchProcess
 from tqdm import tqdm
 
 from dstack import version
+from dstack.backend.local.config import LocalConfig
 from dstack.core.job import Job
 from dstack.core.request import RequestHead, RequestStatus
-from dstack.core.runners import Gpu, Resources, Runner
+from dstack.core.runners import Gpu, Resources
 
 
-def start_runner_process(runner_id: str) -> str:
+def start_runner_process(backend_config: LocalConfig, runner_id: str) -> str:
     _install_runner_if_necessary()
-    runner_config_dir = _get_runner_config_dir(runner_id)
+    runner_config_dir = _get_runner_config_dir(backend_config, runner_id)
     proc = subprocess.Popen(
         [
             _runner_path(),
             "--config-dir",
             runner_config_dir,
             "--log-level",
             "6",
@@ -34,26 +35,28 @@
         stdout=subprocess.DEVNULL,
         stderr=subprocess.STDOUT,
         start_new_session=True,
     )
     return f"l-{proc.pid}"
 
 
-def check_runner_resources(runner_id: str) -> Resources:
+def check_runner_resources(backend_config: LocalConfig, runner_id: str) -> Resources:
     _install_runner_if_necessary()
-    runner_config_dir = _get_runner_config_dir(runner_id, create=True)
+    runner_config_dir = _get_runner_config_dir(backend_config, runner_id, create=True)
+    backend_config_path = runner_config_dir / "config.yaml"
+    with open(backend_config_path, "w+") as f:
+        f.write(backend_config.serialize_yaml())
     runner_config_path = runner_config_dir / "runner.yaml"
     result = subprocess.run(
         [f"{_runner_path()} --config-dir {runner_config_dir} check"],
         shell=True,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.PIPE,
         text=True,
     )
-
     if result.returncode > 0:
         raise Exception(result.stderr)
     _runner_yaml = yaml.load(runner_config_path.open(), yaml.FullLoader)
     return _unserialize_runner_resources(_runner_yaml["resources"])
 
 
 def _unserialize_runner_resources(data: dict) -> Resources:
@@ -104,18 +107,18 @@
 def _runner_bucket() -> str:
     if version.__is_release__:
         return "dstack-runner-downloads"
     else:
         return "dstack-runner-downloads-stgn"
 
 
-def _get_runner_config_dir(runner_id: str, create: Optional[bool] = None) -> str:
-    runner_config_dir_path = Path(
-        os.path.join(_config_directory_path(), "tmp", "runner", "configs", runner_id)
-    )
+def _get_runner_config_dir(
+    backend_config: LocalConfig, runner_id: str, create: Optional[bool] = None
+) -> Path:
+    runner_config_dir_path = backend_config.backend_dir / "tmp" / "runner" / "configs" / runner_id
     if create:
         runner_config_dir_path.mkdir(parents=True, exist_ok=True)
         runner_config_path = runner_config_dir_path / "runner.yaml"
         runner_config_path.write_text(
             yaml.dump(
                 {
                     "id": runner_id,
@@ -154,26 +157,26 @@
     uname = platform.uname()
     arch = _arch()
     darwin = uname.system == "Darwin"
     windows = uname.system == "Windows"
     linux = uname.system == "Linux"
     arm64 = arch == "arm64" or arch == "aarch64"
     i386 = arch == "i386"
-    amd64 = arch == "x86_64"
+    amd64 = arch in ["x86_64", "AMD64"]
     if darwin and arm64:
         filename = "dstack-runner-darwin-arm64"
     elif darwin and amd64:
         filename = "dstack-runner-darwin-amd64"
     elif linux and i386:
         filename = "dstack-runner-linux-x86"
     elif linux and amd64:
         filename = "dstack-runner-linux-amd64"
     elif windows and i386:
         filename = "dstack-runner-windows-x86.exe"
-    elif linux and amd64:
+    elif windows and amd64:
         filename = "dstack-runner-windows-amd64.exe"
     else:
         raise Exception(f"Unsupported platform: {uname}")
     return filename
 
 
 def _config_directory_path() -> Path:
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/local/secrets.py` & `dstack-0.8/cli/dstack/backend/local/secrets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 import os
 import sqlite3
 from pathlib import Path
-from typing import List, Optional
+from typing import Optional
 
 from dstack.backend.base.secrets import SecretsManager
-from dstack.core.repo import RepoAddress
 from dstack.core.secret import Secret
 
 
 class LocalSecretsManager(SecretsManager):
     def __init__(self, root_path: str):
         self.root_path = root_path
 
-    def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
+    def get_secret(self, repo_id: str, secret_name: str) -> Optional[Secret]:
         value = _get_secret_value(
-            db_filepath=_get_secrets_db_filepath(self.root_path, repo_address),
-            key=_get_secret_key(repo_address, secret_name),
+            db_filepath=_get_secrets_db_filepath(self.root_path, repo_id),
+            key=_get_secret_key(repo_id, secret_name),
         )
         if value is None:
             return None
         return Secret(secret_name=secret_name, secret_value=value)
 
-    def add_secret(self, repo_address: RepoAddress, secret: Secret):
+    def add_secret(self, repo_id: str, secret: Secret):
         _create_secret(
-            db_filepath=_get_secrets_db_filepath(self.root_path, repo_address),
-            key=_get_secret_key(repo_address, secret.secret_name),
+            db_filepath=_get_secrets_db_filepath(self.root_path, repo_id),
+            key=_get_secret_key(repo_id, secret.secret_name),
             value=secret.secret_value,
         )
 
-    def update_secret(self, repo_address: RepoAddress, secret: Secret):
+    def update_secret(self, repo_id: str, secret: Secret):
         _update_secret(
-            db_filepath=_get_secrets_db_filepath(self.root_path, repo_address),
-            key=_get_secret_key(repo_address, secret.secret_name),
+            db_filepath=_get_secrets_db_filepath(self.root_path, repo_id),
+            key=_get_secret_key(repo_id, secret.secret_name),
             value=secret.secret_value,
         )
 
-    def delete_secret(self, repo_address: RepoAddress, secret_name: str):
+    def delete_secret(self, repo_id: str, secret_name: str):
         _delete_secret(
-            db_filepath=_get_secrets_db_filepath(self.root_path, repo_address),
-            key=_get_secret_key(repo_address, secret_name),
+            db_filepath=_get_secrets_db_filepath(self.root_path, repo_id),
+            key=_get_secret_key(repo_id, secret_name),
         )
 
-    def get_credentials(self, repo_address: RepoAddress) -> Optional[str]:
+    def get_credentials(self, repo_id: str) -> Optional[str]:
         return _get_secret_value(
-            db_filepath=_get_credentials_db_filepath(self.root_path, repo_address),
-            key=_get_credentials_key(repo_address),
+            db_filepath=_get_credentials_db_filepath(self.root_path),
+            key=_get_credentials_key(repo_id),
         )
 
-    def add_credentials(self, repo_address: RepoAddress, data: str):
+    def add_credentials(self, repo_id: str, data: str):
         _create_secret(
-            db_filepath=_get_credentials_db_filepath(self.root_path, repo_address),
-            key=_get_credentials_key(repo_address),
+            db_filepath=_get_credentials_db_filepath(self.root_path),
+            key=_get_credentials_key(repo_id),
             value=data,
         )
 
-    def update_credentials(self, repo_address: RepoAddress, data: str):
+    def update_credentials(self, repo_id: str, data: str):
         _update_secret(
-            db_filepath=_get_credentials_db_filepath(self.root_path, repo_address),
-            key=_get_credentials_key(repo_address),
+            db_filepath=_get_credentials_db_filepath(self.root_path),
+            key=_get_credentials_key(repo_id),
             value=data,
         )
 
 
 def _get_secret_value(db_filepath: str, key: str) -> Optional[str]:
     _check_db(db_filepath)
     con = sqlite3.connect(db_filepath)
@@ -107,25 +106,25 @@
         con = sqlite3.connect(db_filepath)
         cur = con.cursor()
         cur.execute("""CREATE TABLE IF NOT EXISTS KV (secret_name TEXT, secret_string TEXT);""")
         con.commit()
         con.close()
 
 
-def _get_secrets_db_filepath(root: str, repo_address: RepoAddress) -> str:
-    return os.path.join(_get_secrets_dir(root, repo_address), "_secrets_")
+def _get_secrets_db_filepath(root: str, repo_id: str) -> str:
+    return os.path.join(_get_secrets_dir(root, repo_id), "_secrets_")
 
 
-def _get_secrets_dir(root: str, repo_address: RepoAddress) -> str:
-    return os.path.join(root, "secrets", repo_address.path())
+def _get_secrets_dir(root: str, repo_id: str) -> str:
+    return os.path.join(root, "secrets", repo_id)
 
 
-def _get_secret_key(repo_address: RepoAddress, secret_name: str) -> str:
-    return f"/dstack/secrets/{repo_address.path()}/{secret_name}"
+def _get_secret_key(repo_id: str, secret_name: str) -> str:
+    return f"/dstack/secrets/{repo_id}/{secret_name}"
 
 
-def _get_credentials_db_filepath(root: str, repo_address: RepoAddress) -> str:
+def _get_credentials_db_filepath(root: str) -> str:
     return os.path.join(root, "repos", "_secrets_")
 
 
-def _get_credentials_key(repo_address: RepoAddress) -> str:
-    return f"/dstack/credentials/{repo_address.path()}"
+def _get_credentials_key(repo_id: str) -> str:
+    return f"/dstack/credentials/{repo_id}"
```

### Comparing `dstack-0.7rc1/cli/dstack/backend/local/storage.py` & `dstack-0.8/cli/dstack/backend/local/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import shutil
 from pathlib import Path
 from typing import Callable, Dict, List, Optional
 
+import yaml
+
 from dstack.backend.base.storage import Storage
 from dstack.core.storage import StorageFile
 from dstack.utils.common import removeprefix
 
 
 class LocalStorage(Storage):
     def __init__(self, root_path: str):
@@ -14,14 +16,20 @@
 
     def put_object(self, key: str, content: str, metadata: Optional[Dict] = None):
         _put_object(
             Root=self.root_path,
             Key=key,
             Body=content,
         )
+        if metadata is not None:
+            _put_object(
+                Root=self.root_path,
+                Key=_metadata_key(key),
+                Body=yaml.dump(metadata),
+            )
 
     def get_object(self, key: str) -> Optional[str]:
         try:
             return _get_object(
                 Root=self.root_path,
                 Key=key,
             )
@@ -115,8 +123,16 @@
 
 
 def _delete_object(Root: str, Key: str):
     if not os.path.exists(Root):
         return
     path = os.path.join(Root, Key)
     if os.path.exists(path):
-        os.remove(path)
+        if os.path.isdir(path):
+            shutil.rmtree(path, ignore_errors=True)
+        else:
+            os.remove(path)
+
+
+def _metadata_key(key: str) -> str:
+    parts = key.split("/")
+    return "/".join(parts[:-1] + [f"m;{parts[-1]}"])
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/__init__.py` & `dstack-0.8/cli/dstack/cli/commands/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 from argparse import Namespace, _SubParsersAction
 
 from rich_argparse import RichHelpFormatter
 
+from dstack.cli.common import check_cli_errors
 from dstack.cli.updates import check_for_updates
 
 
 class BasicCommand(object):
     NAME = "name the command"
     DESCRIPTION = "describe the command"
     SUBCOMMANDS = []
@@ -34,13 +35,14 @@
     @property
     def description(self):
         return self.DESCRIPTION
 
     def register(self):
         ...
 
+    @check_cli_errors
     def __command(self, args: Namespace):
         check_for_updates()
         self._command(args)
 
     def _command(self, args: Namespace):
         ...
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/cp/__init__.py` & `dstack-0.8/cli/dstack/cli/commands/cp/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,71 @@
 import os
 import shutil
+import sys
 from argparse import Namespace
 from pathlib import Path
 
-from dstack.api.backend import list_backends
-from dstack.api.repo import load_repo_data
-from dstack.api.run import RunNotFoundError, TagNotFoundError, get_tagged_run_name
-from dstack.backend.base import Backend
+from dstack.api.hub import HubClient
+from dstack.api.runs import RunNotFoundError, TagNotFoundError, get_tagged_run_name
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import console
-from dstack.core.config import get_dstack_dir
-from dstack.core.error import BackendError, check_config, check_git
-from dstack.core.repo import RepoAddress
+from dstack.cli.common import add_project_argument, check_init, console
+from dstack.cli.config import get_hub_client
+from dstack.utils.common import get_dstack_dir
 
 
 class CpCommand(BasicCommand):
     NAME = "cp"
     DESCRIPTION = "Copy artifact files to a local target path"
 
     def __init__(self, parser):
         super().__init__(parser)
 
     def register(self):
+        add_project_argument(self._parser)
         self._parser.add_argument(
             "run_name_or_tag_name",
             metavar="(RUN | :TAG)",
             type=str,
-            help="A name of a run or a tag",
+            help="The name of the run or the tag",
         )
         self._parser.add_argument(
             "source",
             metavar="SOURCE",
             type=str,
             help="A path of an artifact file or directory",
         )
         self._parser.add_argument(
             "target",
             metavar="TARGET",
             type=str,
             help="A local path to download artifact file or directory into",
         )
 
-    @check_config
-    @check_git
+    @check_init
     def _command(self, args: Namespace):
-        repo_data = load_repo_data()
-        backends = list_backends()
-        run_name = None
-        backend = None
-        for backend in backends:
-            try:
-                run_name, _ = get_tagged_run_name(repo_data, backend, args.run_name_or_tag_name)
-                break
-            except (TagNotFoundError, RunNotFoundError):
-                pass
-
-        if run_name is None:
+        hub_client = get_hub_client(project_name=args.project)
+        try:
+            run_name, _ = get_tagged_run_name(hub_client, args.run_name_or_tag_name)
+        except (TagNotFoundError, RunNotFoundError):
             console.print(f"Cannot find the run or tag '{args.run_name_or_tag_name}'")
             exit(1)
-
         _copy_artifact_files(
-            backend=backend,
-            repo_address=repo_data,
+            hub_client=hub_client,
             run_name=run_name,
             source=args.source,
             target=args.target,
         )
         console.print("Artifact files copied")
 
 
-def _copy_artifact_files(
-    backend: Backend, repo_address: RepoAddress, run_name: str, source: str, target: str
-):
-    tmp_output_dir = get_dstack_dir() / "tmp" / "copied_artifacts" / repo_address.path()
+def _copy_artifact_files(hub_client: HubClient, run_name: str, source: str, target: str):
+    tmp_output_dir = get_dstack_dir() / "tmp" / "copied_artifacts" / hub_client.repo.repo_id
     tmp_output_dir.mkdir(parents=True, exist_ok=True)
     source = _normalize_source(source)
-    backend.download_run_artifact_files(
-        repo_address=repo_address,
+    hub_client.download_run_artifact_files(
         run_name=run_name,
         output_dir=tmp_output_dir,
         files_path=source,
     )
     tmp_job_output_dir = None
     # TODO: We support copy for a single job.
     # Decide later how to work with multi-job artifacts.
@@ -94,15 +79,20 @@
     source_full_path = tmp_job_output_dir / source
     target_path = Path(target)
     if source_full_path.is_dir():
         if target_path.exists() and not target_path.is_dir():
             console.print(f"Local target path '{target}' exists and is not a directory")
             shutil.rmtree(tmp_job_output_dir)
             exit(1)
-        shutil.copytree(source_full_path, target, dirs_exist_ok=True)
+        if sys.version_info[1] >= 8:
+            shutil.copytree(source_full_path, target, dirs_exist_ok=True)
+        else:  # todo: drop along with 3.7
+            import distutils.dir_util
+
+            distutils.dir_util.copy_tree(source_full_path, target)
     else:
         if not target_path.exists():
             if target.endswith("/"):
                 target_path.mkdir(parents=True, exist_ok=True)
             else:
                 target_path.parent.mkdir(parents=True, exist_ok=True)
         shutil.copy2(source_full_path, target_path)
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/hub/__init__.py` & `dstack-0.8/cli/dstack/cli/commands/start/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,52 @@
 import os
 from argparse import Namespace
 
 import uvicorn
-from rich_argparse import RichHelpFormatter
 
 from dstack import version
 from dstack.cli.commands import BasicCommand
 
 
-class HubCommand(BasicCommand):
-    NAME = "hub"
-    DESCRIPTION = None  # Hidden by default
+class StartCommand(BasicCommand):
+    NAME = "start"
+    DESCRIPTION = "Start a hub server"
 
     def __init__(self, parser):
-        super(HubCommand, self).__init__(parser)
+        super(StartCommand, self).__init__(parser)
 
-    def _hub_start(self, args: Namespace):
+    def _command(self, args: Namespace):
         os.environ["DSTACK_HUB_HOST"] = args.host
         os.environ["DSTACK_HUB_PORT"] = str(args.port)
         os.environ["DSTACK_HUB_LOG_LEVEL"] = args.log_level
         if args.token:
             os.environ["DSTACK_HUB_ADMIN_TOKEN"] = args.token
         uvicorn.run(
             "dstack.hub.main:app",
             host=args.host,
             port=args.port,
             reload=version.__version__ is None,
             log_level="error",
         )
 
     def register(self):
-        subparsers = self._parser.add_subparsers()
-        hub_parser = subparsers.add_parser(
-            "start",
-            help="Start a hub server",
-            formatter_class=RichHelpFormatter,
-            add_help=False,
-        )
-        hub_parser.add_argument(
-            "-h",
-            "--help",
-            action="help",
-            help="Show this help message and exit",
-        )
-        hub_parser.add_argument(
+        self._parser.add_argument(
             "--host",
-            metavar="HOST",
             type=str,
             help="Bind socket to this host. Defaults to 127.0.0.1",
-            default="127.0.0.1",
+            default=os.getenv("DSTACK_HUB_HOST", "127.0.0.1"),
         )
-        hub_parser.add_argument(
+        self._parser.add_argument(
             "-p",
             "--port",
-            metavar="PORT",
             type=int,
             help="Bind socket to this port. Defaults to 3000.",
-            default=3000,
+            default=os.getenv("DSTACK_HUB_PORT", 3000),
         )
-        hub_parser.add_argument(
+        self._parser.add_argument(
             "-l",
             "--log-level",
-            metavar="LOG-LEVEL",
             type=str,
-            help="",
-            default="ERROR",
+            help="Logging level for hub. Defaults to ERROR.",
+            default=os.getenv("DSTACK_HUB_LOG_LEVEL", "ERROR"),
         )
-        hub_parser.add_argument("--token", metavar="TOKEN", type=str, help="The admin user token")
-        hub_parser.set_defaults(func=self._hub_start)
-
-    def _command(self, args: Namespace):
-        self._parser.print_help()
+        self._parser.add_argument("--token", type=str, help="The admin user token")
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/init/__init__.py` & `dstack-0.8/cli/dstack/cli/commands/init/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 from argparse import Namespace
 from pathlib import Path
 from typing import Optional
 
-from dstack.api.backend import list_backends
-from dstack.api.repo import load_repo_data
+import giturlparse
+from git.exc import InvalidGitRepositoryError
+
+from dstack.api.repos import get_local_repo_credentials
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import console
-from dstack.cli.config import BaseConfig
-from dstack.core.error import check_config, check_git
+from dstack.cli.common import add_project_argument, console
+from dstack.cli.config import config, get_hub_client
+from dstack.core.repo import LocalRepo, RemoteRepo
 from dstack.core.userconfig import RepoUserConfig
 
 
-def get_ssh_keypair(key_path: Optional[str], default: str = "~/.ssh/id_rsa") -> Optional[str]:
-    """Returns path to the private key if keypair exists"""
-    key_path = Path(key_path or default).expanduser().resolve()
-    pub_key = (
-        key_path if key_path.suffix == ".pub" else key_path.with_suffix(key_path.suffix + ".pub")
-    )
-    private_key = pub_key.with_suffix("")
-    if pub_key.exists() and private_key.exists():
-        return str(private_key)
-
-
 class InitCommand(BasicCommand):
     NAME = "init"
     DESCRIPTION = "Authorize dstack to access the current Git repo"
 
     def __init__(self, parser):
         super(InitCommand, self).__init__(parser)
 
     def register(self):
+        add_project_argument(self._parser)
         self._parser.add_argument(
             "-t",
             "--token",
             metavar="OAUTH_TOKEN",
             help="An authentication token for Git",
             type=str,
             dest="gh_token",
@@ -48,33 +40,58 @@
         self._parser.add_argument(
             "--ssh-identity",
             metavar="SSH_PRIVATE_KEY",
             help="A path to the private SSH key file for SSH tunneling",
             type=str,
             dest="ssh_identity_file",
         )
+        self._parser.add_argument("--local", action="store_true", help="Do not use git")
 
-    @check_config
-    @check_git
     def _command(self, args: Namespace):
-        local_repo_data = load_repo_data(args.gh_token, args.git_identity_file)
-        local_repo_data.ls_remote()
-        repo_credentials = local_repo_data.repo_credentials()
-
-        config = BaseConfig()
-        repo_user_config = RepoUserConfig(ssh_key_path=get_ssh_keypair(args.ssh_identity_file))
-        config.write(
-            config.repos / f"{local_repo_data.path(delimiter='.')}.yaml",
-            repo_user_config,
-            mkdir=True,
-        )
+        try:
+            if args.local:  # force fallback to LocalRepo
+                raise InvalidGitRepositoryError()
+            repo = RemoteRepo(local_repo_dir=Path.cwd())
+            repo_credentials = get_local_repo_credentials(
+                repo_data=repo.repo_data,
+                identity_file=args.git_identity_file,
+                oauth_token=args.gh_token,
+                original_hostname=giturlparse.parse(repo.repo_url).resource,
+            )
+        except InvalidGitRepositoryError:
+            console.print(
+                f"[gray58]No git remote is used, it could affect efficiency of source code transfer[/]"
+            )
+            repo = LocalRepo(repo_dir=Path.cwd())
+            repo_credentials = None
 
-        for backend in list_backends():
-            backend.save_repo_credentials(local_repo_data, repo_credentials)
-            status = (
-                "[yellow]WARNING[/]" if repo_user_config.ssh_key_path is None else "[green]OK[/]"
+        config.save_repo_user_config(
+            RepoUserConfig(
+                repo_id=repo.repo_ref.repo_id,
+                repo_type=repo.repo_data.repo_type,
+                ssh_key_path=get_ssh_keypair(args.ssh_identity_file),
             )
-            console.print(f"{status} [gray58](backend: {backend.name})[/]")
-        if repo_user_config.ssh_key_path is None:
+        )
+        hub_client = get_hub_client(project_name=args.project)
+        if repo_credentials is not None:
+            hub_client.save_repo_credentials(repo_credentials)
+        status = (
+            "[yellow]WARNING[/]"
+            if config.repo_user_config.ssh_key_path is None
+            else "[green]OK[/]"
+        )
+        console.print(f"{status}")
+        if config.repo_user_config.ssh_key_path is None:
             console.print(
                 f"[red]SSH is not enabled. To enable it, make sure `{args.ssh_identity_file or '~/.ssh/id_rsa'}` exists or call `dstack init --ssh-identity PATH`[/]"
             )
+
+
+def get_ssh_keypair(key_path: Optional[str], default: str = "~/.ssh/id_rsa") -> Optional[str]:
+    """Returns path to the private key if keypair exists"""
+    key_path = Path(key_path or default).expanduser().resolve()
+    pub_key = (
+        key_path if key_path.suffix == ".pub" else key_path.with_suffix(key_path.suffix + ".pub")
+    )
+    private_key = pub_key.with_suffix("")
+    if pub_key.exists() and private_key.exists():
+        return str(private_key)
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/ls/__init__.py` & `dstack-0.8/cli/dstack/cli/commands/ls/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 from argparse import Namespace
-from collections import defaultdict
 from pathlib import Path
-from typing import Optional
 
 from rich.table import Table
 
-from dstack.api.artifacts import list_artifacts_with_merged_backends
-from dstack.api.backend import list_backends
-from dstack.api.repo import load_repo_data
-from dstack.api.run import RunNotFoundError, TagNotFoundError, get_tagged_run_name
+from dstack.api.runs import RunNotFoundError, TagNotFoundError, get_tagged_run_name
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import console
-from dstack.core.error import check_config, check_git
+from dstack.cli.common import add_project_argument, check_init, console
+from dstack.cli.config import get_hub_client
 from dstack.utils.common import sizeof_fmt
 
 
 class LsCommand(BasicCommand):
     NAME = "ls"
     DESCRIPTION = "List artifacts"
 
     def __init__(self, parser):
         super(LsCommand, self).__init__(parser)
 
     def register(self):
+        add_project_argument(self._parser)
         self._parser.add_argument(
             "run_name_or_tag_name",
             metavar="RUN | :TAG",
             type=str,
-            help="A name of a run or a tag",
+            help="The name of the run or the tag",
         )
         self._parser.add_argument(
             "prefix",
             metavar="SEARCH_PREFIX",
             type=str,
             help="Show files starting with prefix",
             nargs="?",
@@ -41,87 +37,69 @@
         self._parser.add_argument(
             "-r", "--recursive", help="Show all files recursively", action="store_true"
         )
         self._parser.add_argument(
             "-t", "--total", help="Show total folder size", action="store_true"
         )
 
-    @check_config
-    @check_git
+    @check_init
     def _command(self, args: Namespace):
         table = Table(box=None)
         table.add_column("ARTIFACT", style="bold", no_wrap=True)
         table.add_column("FILE")
         table.add_column("SIZE", style="dark_sea_green4")
-        table.add_column("BACKENDS", style="bold")
 
-        repo_data = load_repo_data()
-        backends = list_backends()
-        run_names = []
-        backends_run_name = []
-        for backend in backends:
-            try:
-                run_name, _ = get_tagged_run_name(repo_data, backend, args.run_name_or_tag_name)
-                run_names.append(run_name)
-                backends_run_name.append(backend)
-            except (TagNotFoundError, RunNotFoundError):
-                pass
-
-        if len(run_names) == 0:
+        hub_client = get_hub_client(project_name=args.project)
+        try:
+            run_name, _ = get_tagged_run_name(hub_client, args.run_name_or_tag_name)
+        except (TagNotFoundError, RunNotFoundError):
             console.print(f"Cannot find the run or tag '{args.run_name_or_tag_name}'")
             exit(1)
 
-        artifacts = list_artifacts_with_merged_backends(
-            backends_run_name, load_repo_data(), run_names[0]
-        )
-
-        for artifact, _ in artifacts:
+        artifacts = hub_client.list_run_artifact_files(run_name)
+        for artifact in artifacts:
             artifact.files = sorted(
                 [
                     f
                     for f in artifact.files
                     if str(Path(artifact.name, f.filepath)).startswith(args.prefix)
                 ],
                 key=lambda f: f.filepath,
             )
 
         if args.recursive:
-            for artifact, backends in artifacts:
+            for artifact in artifacts:
                 for i, file in enumerate(artifact.files):
                     table.add_row(
                         artifact.name if i == 0 else "",
                         file.filepath,
                         sizeof_fmt(file.filesize_in_bytes),
-                        ", ".join(b.name for b in backends),
                     )
         else:
             entries = {}
-            for artifact, backends in artifacts:
+            for artifact in artifacts:
                 if entries.get(artifact.name) is None:
                     entries[artifact.name] = {}
                 for i, file in enumerate(artifact.files):
                     entry_name = _get_entry_name(file.filepath, args.prefix)
                     if entries[artifact.name].get(entry_name) is None:
                         entries[artifact.name][entry_name] = {"size": 0, "backends": set()}
                     entries[artifact.name][entry_name]["size"] += file.filesize_in_bytes
-                    entries[artifact.name][entry_name]["backends"].update(backends)
 
             for artifact_name, entry_map in entries.items():
                 first_entry = True
                 for entry_name, entry_dict in entry_map.items():
                     table.add_row(
                         artifact_name if first_entry else "",
                         entry_name,
                         sizeof_fmt(entry_dict["size"])
                         if not entry_name.endswith("/") or args.total
                         else "",
-                        ", ".join(b.name for b in entry_dict["backends"]),
                     )
                     first_entry = False
-
         console.print(table)
 
 
 def _get_entry_name(filepath: str, prefix: str) -> str:
     if prefix == "":
         prefix_parts_num = 1
     else:
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/ps/__init__.py` & `dstack-0.8/cli/dstack/cli/commands/ps/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import time
 from argparse import Namespace
 
 from rich.live import Live
 
-from dstack.api.backend import list_backends
-from dstack.api.run import list_runs_with_merged_backends
+from dstack.api.runs import list_runs
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import generate_runs_table, print_runs
-from dstack.core.error import check_config, check_git
+from dstack.cli.common import add_project_argument, check_init, generate_runs_table, print_runs
+from dstack.cli.config import get_hub_client
 
 LIVE_PROVISION_INTERVAL_SECS = 2
 
 REFRESH_RATE_PER_SEC = 3
 
 
 class PSCommand(BasicCommand):
@@ -19,42 +18,48 @@
     DESCRIPTION = "List runs"
 
     def __init__(self, parser):
         super(PSCommand, self).__init__(parser)
 
     def register(self):
         self._parser.add_argument(
-            "run_name", metavar="RUN", type=str, nargs="?", help="A name of a run"
+            "run_name", metavar="RUN", type=str, nargs="?", help="The name of the run"
         )
+        add_project_argument(self._parser)
         self._parser.add_argument(
             "-a",
             "--all",
             help="Show all runs. "
             "By default, it only shows unfinished runs or the last finished.",
             action="store_true",
         )
         self._parser.add_argument(
+            "-v",
+            "--verbose",
+            help="Show more information about runs",
+            action="store_true",
+        )
+        self._parser.add_argument(
             "-w",
             "--watch",
             help="Watch statuses of runs in realtime",
             action="store_true",
         )
 
-    @check_config
-    @check_git
+    @check_init
     def _command(self, args: Namespace):
-        list_runs = list_runs_with_merged_backends(list_backends(), args.run_name, args.all)
+        hub_client = get_hub_client(project_name=args.project)
+        runs = list_runs(hub_client, run_name=args.run_name, all=args.all)
         if args.watch:
             try:
                 with Live(
-                    generate_runs_table(list_runs), refresh_per_second=REFRESH_RATE_PER_SEC
+                    generate_runs_table(runs, verbose=args.verbose),
+                    refresh_per_second=REFRESH_RATE_PER_SEC,
                 ) as live:
                     while True:
                         time.sleep(LIVE_PROVISION_INTERVAL_SECS)
-                        list_runs = list_runs_with_merged_backends(
-                            list_backends(), args.run_name, args.all
-                        )
-                        live.update(generate_runs_table(list_runs))
+                        runs = list_runs(hub_client, run_name=args.run_name, all=args.all)
+                        live.update(generate_runs_table(runs, verbose=args.verbose))
             except KeyboardInterrupt:
                 pass
         else:
-            print_runs(list_runs)
+            print_runs(runs, verbose=args.verbose)
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/rm/__init__.py` & `dstack-0.8/cli/dstack/cli/commands/rm/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-import sys
 from argparse import Namespace
 
-from rich import print
 from rich.prompt import Confirm
 
-from dstack.api.backend import list_backends
-from dstack.api.repo import load_repo_data
 from dstack.cli.commands import BasicCommand
-from dstack.core.error import check_config, check_git
+from dstack.cli.common import add_project_argument, check_init, console
+from dstack.cli.config import get_hub_client
 
 
 class RMCommand(BasicCommand):
     NAME = "rm"
     DESCRIPTION = "Remove run(s)"
 
     def __init__(self, parser):
         super(RMCommand, self).__init__(parser)
 
     def register(self):
+        add_project_argument(self._parser)
         self._parser.add_argument(
-            "run_name", metavar="RUN", type=str, nargs="?", help="A name of a run"
+            "run_name", metavar="RUN", type=str, nargs="?", help="The name of the run"
         )
         self._parser.add_argument(
             "-a",
             "--all",
             help="Remove all finished runs",
             dest="all",
             action="store_true",
         )
         self._parser.add_argument(
             "-y", "--yes", help="Don't ask for confirmation", action="store_true"
         )
 
-    @check_config
-    @check_git
+    @check_init
     def _command(self, args: Namespace):
         if (
             args.run_name
             and (args.yes or Confirm.ask(f"[red]Delete the run '{args.run_name}'?[/]"))
         ) or (args.all and (args.yes or Confirm.ask("[red]Delete all runs?[/]"))):
-            repo_data = load_repo_data()
+            hub_client = get_hub_client(project_name=args.project)
             deleted_run = False
-            for backend in list_backends():
-                job_heads = backend.list_job_heads(repo_data, args.run_name)
-                if job_heads:
-                    finished_job_heads = []
-                    for job_head in job_heads:
-                        if job_head.status.is_finished():
-                            finished_job_heads.append(job_head)
-                        elif args.run_name:
-                            sys.exit("The run is not finished yet. Stop the run first.")
-                    for job_head in finished_job_heads:
-                        backend.delete_job_head(repo_data, job_head.job_id)
-                        deleted_run = True
+            job_heads = hub_client.list_job_heads(args.run_name)
+            if job_heads:
+                finished_job_heads = []
+                for job_head in job_heads:
+                    if job_head.status.is_finished():
+                        finished_job_heads.append(job_head)
+                    elif args.run_name:
+                        console.print("The run is not finished yet. Stop the run first.")
+                        exit(1)
+                for job_head in finished_job_heads:
+                    hub_client.delete_job_head(job_head.job_id)
+                    deleted_run = True
             if args.run_name and not deleted_run:
-                sys.exit(f"Cannot find the run '{args.run_name}'")
-            print(f"[grey58]OK[/]")
+                console.print(f"Cannot find the run '{args.run_name}'")
+                exit(1)
+            console.print(f"[grey58]OK[/]")
         else:
             if not args.run_name and not args.all:
-                sys.exit("Specify a run name or use --all to delete all runs")
+                console.print("Specify a run name or use --all to delete all runs")
+                exit(1)
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/run/ssh_tunnel.py` & `dstack-0.8/cli/dstack/cli/commands/run/ssh_tunnel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import socket
 import subprocess
 from contextlib import closing
-from os import PathLike
 from typing import Dict, List
 
 from dstack.core.job import Job
+from dstack.utils.common import PathLike
 
 
 def get_free_port() -> int:
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
         s.bind(("", 0))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         return s.getsockname()[1]
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/stop/__init__.py` & `dstack-0.8/cli/dstack/cli/commands/stop/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from argparse import Namespace
 
 from rich.prompt import Confirm
 
-from dstack.api.backend import list_backends
-from dstack.api.repo import load_repo_data
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import console
-from dstack.core.error import check_config, check_git
+from dstack.cli.common import add_project_argument, check_init, console
+from dstack.cli.config import get_hub_client
 
 
 def _verb(abort: bool):
     if abort:
         return "Abort"
     else:
         return "Stop"
@@ -20,16 +18,17 @@
     NAME = "stop"
     DESCRIPTION = "Stop run(s)"
 
     def __init__(self, parser):
         super(StopCommand, self).__init__(parser)
 
     def register(self):
+        add_project_argument(self._parser)
         self._parser.add_argument(
-            "run_name", metavar="RUN", type=str, nargs="?", help="A name of a run"
+            "run_name", metavar="RUN", type=str, nargs="?", help="The name of the run"
         )
         self._parser.add_argument(
             "-a",
             "--all",
             help="Stop all unfinished runs",
             dest="all",
             action="store_true",
@@ -41,31 +40,27 @@
             dest="abort",
             action="store_true",
         )
         self._parser.add_argument(
             "-y", "--yes", help="Don't ask for confirmation", action="store_true"
         )
 
-    @check_config
-    @check_git
+    @check_init
     def _command(self, args: Namespace):
         if not args.run_name and not args.all:
             console.print("Specify a run name or use --all to stop all workflows")
             exit(1)
         if (
             args.run_name
             and (
                 args.yes or Confirm.ask(f"[red]{_verb(args.abort)} the run '{args.run_name}'?[/]")
             )
         ) or (args.all and (args.yes or Confirm.ask(f"[red]{_verb(args.abort)} all runs?[/]"))):
-            repo_data = load_repo_data()
-            found_run = False
-            for backend in list_backends():
-                job_heads = backend.list_job_heads(repo_data, args.run_name)
-                found_run = len(job_heads) > 0
-                for job_head in job_heads:
-                    if job_head.status.is_unfinished():
-                        backend.stop_job(repo_data, job_head.job_id, args.abort)
-            if args.run_name and not found_run:
+            hub_client = get_hub_client(project_name=args.project)
+            job_heads = hub_client.list_job_heads(args.run_name)
+            if len(job_heads) == 0:
                 console.print(f"Cannot find the run '{args.run_name}'")
                 exit(1)
+            for job_head in job_heads:
+                if job_head.status.is_unfinished():
+                    hub_client.stop_job(job_head.job_id, args.abort)
             console.print(f"[grey58]OK[/]")
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/commands/tags/__init__.py` & `dstack-0.8/cli/dstack/cli/commands/tags/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-import sys
 from argparse import Namespace
 
 from rich import print
-from rich.console import Console
 from rich.prompt import Confirm
 from rich.table import Table
 from rich_argparse import RichHelpFormatter
 
-from dstack.api.backend import list_backends
-from dstack.api.repo import load_repo_data
-from dstack.api.tags import list_tag_heads_with_merged_backends
-from dstack.backend.base import BackendType
 from dstack.cli.commands import BasicCommand
-from dstack.core.error import BackendError, check_config, check_git
+from dstack.cli.common import add_project_argument, check_init, console
+from dstack.cli.config import get_hub_client
+from dstack.core.error import BackendError
 from dstack.utils.common import pretty_date
 
 
 class TAGCommand(BasicCommand):
     NAME = "tags"
     DESCRIPTION = "Manage tags"
 
@@ -25,130 +21,104 @@
 
     def register(self):
         subparsers = self._parser.add_subparsers()
 
         add_tags_parser = subparsers.add_parser(
             "add", help="Add a tag", formatter_class=RichHelpFormatter
         )
+        add_project_argument(add_tags_parser)
         add_tags_parser.add_argument(
             "tag_name", metavar="TAG", type=str, help="The name of the tag"
         )
         add_tags_parser.add_argument(
-            "run_name", metavar="RUN", type=str, help="A name of a run", nargs="?"
+            "run_name", metavar="RUN", type=str, help="The name of the run", nargs="?"
         )
         add_tags_parser.add_argument(
             "-a",
             "--artifact",
             metavar="PATH",
             type=str,
             help="A path to local directory to upload as an artifact",
             action="append",
             dest="artifact_paths",
         )
         add_tags_parser.add_argument(
-            "-r", "--remote", help="Upload artifact to remote", action="store_true"
-        )
-        add_tags_parser.add_argument(
             "-y", "--yes", help="Don't ask for confirmation", action="store_true"
         )
         add_tags_parser.set_defaults(func=self.add_tag)
 
         delete_tags_parser = subparsers.add_parser(
             "delete", help="Delete a tag", formatter_class=RichHelpFormatter
         )
+        add_project_argument(delete_tags_parser)
         delete_tags_parser.add_argument(
             "tag_name", metavar="TAG_NAME", type=str, help="The name of the tag"
         )
         delete_tags_parser.add_argument(
             "-y", "--yes", help="Don't ask for confirmation", action="store_true"
         )
         delete_tags_parser.set_defaults(func=self.delete_tag)
 
-    @check_config
-    @check_git
+    @check_init
     def _command(self, args: Namespace):
-        repo_data = load_repo_data()
-        console = Console()
         table = Table(box=None)
         table.add_column("TAG", style="bold", no_wrap=True)
         table.add_column("CREATED", style="grey58", no_wrap=True)
         table.add_column("RUN", style="grey58", no_wrap=True)
         table.add_column("OWNER", style="grey58", no_wrap=True, max_width=16)
         table.add_column("BACKENDS", style="bold green", no_wrap=True)
 
-        tag_heads = list_tag_heads_with_merged_backends(list_backends(), repo_data)
-
-        for tag_head, backends in tag_heads:
+        hub_client = get_hub_client(project_name=args.project)
+        tag_heads = hub_client.list_tag_heads()
+        for tag_head in tag_heads:
             created_at = pretty_date(round(tag_head.created_at / 1000))
             table.add_row(
                 tag_head.tag_name,
                 created_at,
                 tag_head.run_name,
-                tag_head.local_repo_user_name or "",
-                ", ".join(b.name for b in backends),
+                tag_head.hub_user_name,
             )
         console.print(table)
 
-    @check_config
+    @check_init
     def add_tag(self, args: Namespace):
-        if args.run_name or args.artifact_paths:
-            repo_data = load_repo_data()
-            added_tag = False
-            confirmed_override = False
-            for backend in list_backends():
-                tag_head = backend.get_tag_head(repo_data, args.tag_name)
-                if tag_head:
-                    if not args.yes and not confirmed_override:
-                        confirmed_override = Confirm.ask(
-                            f"[red]The tag '{args.tag_name}' already exists. "
-                            f"Do you want to override it?[/]"
-                        )
-                        if not confirmed_override:
-                            return
-                    backend.delete_tag_head(repo_data, tag_head)
-                if args.run_name is not None:
-                    jobs_heads = backend.list_job_heads(repo_data, args.run_name)
-                    if len(jobs_heads) == 0:
-                        continue
-                    try:
-                        backend.add_tag_from_run(
-                            repo_data, args.tag_name, args.run_name, run_jobs=None
-                        )
-                        added_tag = True
-                    except BackendError as e:
-                        print(e)
-                        exit(1)
-                else:
-                    if not args.remote and backend.type is BackendType.REMOTE:
-                        continue
-                    if args.remote and backend.type is BackendType.LOCAL:
-                        continue
-                    try:
-                        backend.add_tag_from_local_dirs(
-                            repo_data, args.tag_name, args.artifact_paths
-                        )
-                    except BackendError as e:
-                        print(e)
-                        exit(1)
-            if args.run_name is not None and not added_tag:
-                print(f"The run '{args.run_name}' doesn't exist")
+        if not args.run_name and not args.artifact_paths:
+            console.print("Specify -r RUN or -a PATH to create a tag")
+            exit(1)
+        hub_client = get_hub_client(project_name=args.project)
+        tag_head = hub_client.get_tag_head(args.tag_name)
+        if tag_head is not None:
+            if not args.yes and not Confirm.ask(
+                f"[red]The tag '{args.tag_name}' already exists. "
+                f"Do you want to override it?[/]"
+            ):
+                return
+            hub_client.delete_tag_head(tag_head)
+        if args.run_name is not None:
+            jobs_heads = hub_client.list_job_heads(args.run_name)
+            if len(jobs_heads) == 0:
+                console.print(f"The run '{args.run_name}' doesn't exist")
+                exit(1)
+            try:
+                hub_client.add_tag_from_run(args.tag_name, args.run_name, run_jobs=None)
+            except BackendError as e:
+                print(e)
                 exit(1)
-            print(f"[grey58]OK[/]")
         else:
-            sys.exit("Specify -r RUN or -a PATH to create a tag")
+            try:
+                hub_client.add_tag_from_local_dirs(args.tag_name, args.artifact_paths)
+            except BackendError as e:
+                print(e)
+                exit(1)
+        print(f"[grey58]OK[/]")
 
-    @check_config
+    @check_init
     def delete_tag(self, args: Namespace):
-        repo_data = load_repo_data()
-        tag_heads = []
-        for backend in list_backends():
-            tag_head = backend.get_tag_head(repo_data, args.tag_name)
-            if tag_head is not None:
-                tag_heads.append((backend, tag_head))
-
-        if len(tag_heads) == 0:
-            sys.exit(f"The tag '{args.tag_name}' doesn't exist")
+        hub_client = get_hub_client(project_name=args.project)
+        tag_head = hub_client.get_tag_head(args.tag_name)
+        if tag_head is None:
+            console.print(f"The tag '{args.tag_name}' doesn't exist")
+            exit(1)
 
         if args.yes or Confirm.ask(f" [red]Delete the tag '{args.tag_name}'?[/]"):
-            for backend, tag_head in tag_heads:
-                backend.delete_tag_head(repo_data, tag_head)
+            hub_client.delete_tag_head(tag_head)
             print(f"[grey58]OK[/]")
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/handlers.py` & `dstack-0.8/cli/dstack/cli/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-from dstack import version
 from dstack.cli.commands.config import ConfigCommand
 from dstack.cli.commands.cp import CpCommand
-from dstack.cli.commands.hub import HubCommand
 from dstack.cli.commands.init import InitCommand
 from dstack.cli.commands.logs import LogCommand
 from dstack.cli.commands.ls import LsCommand
 from dstack.cli.commands.prune import PruneCommand
 from dstack.cli.commands.ps import PSCommand
-from dstack.cli.commands.pull import PullCommand
-from dstack.cli.commands.push import PushCommand
 from dstack.cli.commands.rm import RMCommand
 from dstack.cli.commands.run import RunCommand
 from dstack.cli.commands.secrets import SecretCommand
+from dstack.cli.commands.start import StartCommand
 from dstack.cli.commands.stop import StopCommand
 from dstack.cli.commands.tags import TAGCommand
 
 commands_classes = [
     ConfigCommand,
     CpCommand,
     InitCommand,
     LogCommand,
     LsCommand,
     PruneCommand,
     PSCommand,
-    PullCommand,
-    PushCommand,
     RMCommand,
     RunCommand,
     SecretCommand,
     StopCommand,
     TAGCommand,
+    StartCommand,
 ]
 
-if not version.__is_release__:
-    commands_classes.append(HubCommand)
-
 
 def cli_initialize(parser):
     commands = [cls(parser=parser) for cls in commands_classes]
     for command in commands:
         command.register()
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/main.py` & `dstack-0.8/cli/dstack/cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import sys
 
 from rich_argparse import RichHelpFormatter
 
+from dstack.cli.common import check_cli_errors
 from dstack.cli.handlers import cli_initialize
 from dstack.version import __version__ as version
 
 
 def main():
     RichHelpFormatter.usage_markup = True
     RichHelpFormatter.styles["argparse.args"] = "bold sea_green3"
@@ -40,15 +41,15 @@
     parser.set_defaults(func=lambda _: parser.print_help())
     subparsers = parser.add_subparsers(metavar="COMMAND")
 
     cli_initialize(parser=subparsers)
 
     if len(sys.argv) < 2:
         parser.print_help()
-        exit(1)
+        exit(0)
     args, unknown = parser.parse_known_args()
     args.unknown = unknown
-    args.func(args)
+    check_cli_errors(args.func)(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dstack-0.7rc1/cli/dstack/cli/updates.py` & `dstack-0.8/cli/dstack/cli/updates.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/core/app.py` & `dstack-0.8/cli/dstack/core/app.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/core/job.py` & `dstack-0.8/cli/dstack/core/job.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from abc import abstractmethod
 from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field, root_validator
 
 from dstack.core.app import AppSpec
 from dstack.core.artifact import ArtifactSpec
 from dstack.core.cache import CacheSpec
 from dstack.core.dependents import DepSpec
-from dstack.core.repo import RepoAddress, RepoData
+from dstack.core.repo import (
+    LocalRepo,
+    LocalRepoData,
+    RemoteRepo,
+    RemoteRepoData,
+    Repo,
+    RepoData,
+    RepoRef,
+)
 from dstack.utils.common import _quoted, format_list
 
 
 class GpusRequirements(BaseModel):
     count: Optional[int] = None
     memory_mib: Optional[int] = None
     name: Optional[str] = None
@@ -81,15 +89,15 @@
     def set_id(self, job_id: Optional[str]):
         self.job_id = job_id
 
     def __str__(self) -> str:
         return f'JobRefId(job_id="{self.job_id}")'
 
 
-class JobStatus(Enum):
+class JobStatus(str, Enum):
     PENDING = "pending"
     SUBMITTED = "submitted"
     DOWNLOADING = "downloading"
     RUNNING = "running"
     UPLOADING = "uploading"
     STOPPING = "stopping"
     STOPPED = "stopped"
@@ -101,56 +109,47 @@
     def is_finished(self):
         return self in [self.STOPPED, self.ABORTED, self.FAILED, self.DONE]
 
     def is_unfinished(self):
         return not self.is_finished()
 
 
+class JobErrorCode(str, Enum):
+    # Set by CLI
+    NO_INSTANCE_MATCHING_REQUIREMENTS = "no_instance_matching_requirements"
+    FAILED_TO_START_DUE_TO_NO_CAPACITY = "failed_to_start_due_to_no_capacity"
+    INTERRUPTED_BY_NO_CAPACITY = "interrupted_by_no_capacity"
+    # Set by runner
+    CONTAINER_EXITED_WITH_ERROR = "container_exited_with_error"
+
+    def pretty_repr(self) -> str:
+        return " ".join(self.value.split("_")).capitalize()
+
+
 class JobHead(JobRef):
     job_id: str
-    repo_address: RepoAddress
+    repo_ref: RepoRef
+    hub_user_name: str
     run_name: str
     workflow_name: Optional[str]
     provider_name: str
-    local_repo_user_name: Optional[str]
     status: JobStatus
+    error_code: Optional[JobErrorCode]
+    container_exit_code: Optional[int]
     submitted_at: int
     artifact_paths: Optional[List[str]]
     tag_name: Optional[str]
     app_names: Optional[List[str]]
 
     def get_id(self) -> Optional[str]:
         return self.job_id
 
     def set_id(self, job_id: Optional[str]):
         self.job_id = job_id
 
-    def __str__(self) -> str:
-        artifact_paths = (
-            ("[" + ", ".join(map(lambda a: _quoted(str(a)), self.artifact_paths)) + "]")
-            if self.artifact_paths
-            else None
-        )
-        app_names = (
-            ("[" + ", ".join(map(lambda a: _quoted(a), self.app_names)) + "]")
-            if self.app_names
-            else None
-        )
-        return (
-            f'JobHead(job_id="{self.job_id}", repo_address={self.repo_address}, '
-            f'run_name="{self.run_name}", workflow_name={_quoted(self.workflow_name)}, '
-            f'provider_name="{self.provider_name}", '
-            f"local_repo_user_name={_quoted(self.local_repo_user_name)}, "
-            f"status=JobStatus.{self.status.name}, "
-            f"submitted_at={self.submitted_at}, "
-            f"artifact_paths={artifact_paths}, "
-            f"tag_name={_quoted(self.tag_name)}, "
-            f"app_names={app_names})"
-        )
-
 
 class RegistryAuth(BaseModel):
     username: Optional[str] = None
     password: Optional[str] = None
 
     def __str__(self) -> str:
         return f"RegistryCredentials(username={self.username}, password={self.password})"
@@ -165,21 +164,24 @@
     if hasattr(element, field):
         return getattr(element, field)
     return None
 
 
 class Job(JobHead):
     job_id: Optional[str]
-    repo_data: RepoData
+    repo_data: Union[RepoData, RemoteRepoData, LocalRepoData] = Field(
+        ..., discriminator="repo_type"
+    )
+    repo_code_filename: Optional[str] = None
     run_name: str
     workflow_name: Optional[str]
     provider_name: str
-    local_repo_user_name: Optional[str]
-    local_repo_user_email: Optional[str]
     status: JobStatus
+    error_code: Optional[JobErrorCode]
+    container_exit_code: Optional[int]
     submitted_at: int
     submission_num: int = 1
     image_name: str
     registry_auth: Optional[RegistryAuth]
     commands: Optional[List[str]]
     entrypoint: Optional[List[str]]
     env: Optional[Dict[str, str]]
@@ -194,112 +196,58 @@
     master_job: Optional[JobRef]
     app_specs: Optional[List[AppSpec]]
     runner_id: Optional[str]
     request_id: Optional[str]
     tag_name: Optional[str]
     ssh_key_pub: Optional[str]
 
-    def __init__(self, **data: Any):
+    @root_validator(pre=True)
+    def preprocess_data(cls, data):
         # TODO Ugly style
-        if type(data) == dict:
-            if "repo_address" in data:
-                del data["repo_address"]
-            if "artifact_paths" in data:
-                del data["artifact_paths"]
-            if "app_names" in data:
-                del data["app_names"]
-        super().__init__(
-            repo_address=data.get("repo_data"),
-            artifact_paths=[check_dict(a, "artifact_path") for a in data.get("artifact_specs")]
+        data["artifact_paths"] = (
+            [check_dict(a, "artifact_path") for a in data.get("artifact_specs")]
             if data.get("artifact_specs")
-            else None,
-            app_names=[check_dict(a, "app_name") for a in data.get("app_specs")]
-            if data.get("app_specs")
-            else None,
-            **data,
+            else None
         )
-
-    def get_id(self) -> Optional[str]:
-        return self.job_id
-
-    def set_id(self, job_id: Optional[str]):
-        self.job_id = job_id
-
-    def __str__(self) -> str:
-        commands = format_list(self.commands, formatter=lambda a: _quoted(str(a)))
-        entrypoint = format_list(self.entrypoint, formatter=lambda a: _quoted(str(a)))
-        artifact_specs = format_list(self.artifact_specs)
-        cache_specs = format_list(self.cache_specs or None)
-        app_specs = format_list(self.app_specs)
-        dep_specs = format_list(self.dep_specs)
-        ssk_key_pub = f"...{self.ssh_key_pub[-16:]}" if self.ssh_key_pub else None
-        return (
-            f'Job(job_id="{self.job_id}", repo_data={self.repo_data}, '
-            f'run_name="{self.run_name}", workflow_name={_quoted(self.workflow_name)}, '
-            f'provider_name="{self.provider_name}", '
-            f"local_repo_user_name={_quoted(self.local_repo_user_name)}, "
-            f"local_repo_user_email={_quoted(self.local_repo_user_email)}, "
-            f"status=JobStatus.{self.status.name}, "
-            f"submitted_at={self.submitted_at}, "
-            f'image_name="{self.image_name}", '
-            f'registry_auth="{self.registry_auth}", '
-            f"commands={commands}, "
-            f"entrypoint={entrypoint}, "
-            f"env={self.env}, "
-            f"working_dir={_quoted(self.working_dir)}, "
-            f"port_count={self.port_count}, "
-            f"ports={self.ports}, "
-            f"host_name={_quoted(self.host_name)}, "
-            f"artifact_specs={artifact_specs}, "
-            f"cache_specs={cache_specs}, "
-            f"requirements={self.requirements}, "
-            f"dep_specs={dep_specs}, "
-            f"master_job={self.master_job}, "
-            f"app_specs={app_specs}, "
-            f"runner_id={_quoted(self.runner_id)}, "
-            f"request_id={_quoted(self.request_id)}, "
-            f"tag_name={_quoted(self.tag_name)}"
-            f"ssh_key_pub={_quoted(ssk_key_pub)})"
+        data["app_names"] = (
+            [check_dict(a, "app_name") for a in data.get("app_specs")]
+            if data.get("app_specs")
+            else None
         )
+        return data
 
     def serialize(self) -> dict:
         deps = []
         if self.dep_specs:
             for dep in self.dep_specs:
                 deps.append(
                     {
-                        "repo_host_name": dep.repo_address.repo_host_name,
-                        "repo_port": dep.repo_address.repo_port or 0,
-                        "repo_user_name": dep.repo_address.repo_user_name,
-                        "repo_name": dep.repo_address.repo_name,
+                        "repo_id": dep.repo_ref.repo_id,
+                        "hub_user_name": self.hub_user_name,
                         "run_name": dep.run_name,
                         "mount": dep.mount,
                     }
                 )
         artifacts = []
         if self.artifact_specs:
             for artifact_spec in self.artifact_specs:
                 artifacts.append(
                     {"path": artifact_spec.artifact_path, "mount": artifact_spec.mount}
                 )
         job_data = {
             "job_id": self.job_id,
-            "repo_host_name": self.repo_address.repo_host_name,
-            "repo_port": self.repo_address.repo_port or 0,
-            "repo_user_name": self.repo_data.repo_user_name,
-            "repo_name": self.repo_data.repo_name,
-            "repo_branch": self.repo_data.repo_branch or "",
-            "repo_hash": self.repo_data.repo_hash or "",
-            "repo_diff": self.repo_data.repo_diff or "",
+            "repo_id": self.repo.repo_id,
+            "hub_user_name": self.hub_user_name,
+            "repo_type": self.repo.repo_data.repo_type,
             "run_name": self.run_name,
             "workflow_name": self.workflow_name or "",
             "provider_name": self.provider_name,
-            "local_repo_user_name": self.local_repo_user_name or "",
-            "local_repo_user_email": self.local_repo_user_email or "",
             "status": self.status.value,
+            "error_code": self.error_code.value if self.error_code is not None else "",
+            "container_exit_code": self.container_exit_code or "",
             "submitted_at": self.submitted_at,
             "submission_num": self.submission_num,
             "image_name": self.image_name,
             "registry_auth": self.registry_auth.serialize() if self.registry_auth else {},
             "commands": self.commands or [],
             "entrypoint": self.entrypoint,
             "env": self.env or {},
@@ -323,27 +271,35 @@
             ]
             if self.app_specs
             else [],
             "runner_id": self.runner_id or "",
             "request_id": self.request_id or "",
             "tag_name": self.tag_name or "",
             "ssh_key_pub": self.ssh_key_pub or "",
+            "repo_code_filename": self.repo_code_filename,
         }
+        if isinstance(self.repo_data, RemoteRepoData):
+            job_data["repo_host_name"] = self.repo_data.repo_host_name
+            job_data["repo_port"] = self.repo_data.repo_port or 0
+            job_data["repo_user_name"] = self.repo_data.repo_user_name
+            job_data["repo_name"] = self.repo_data.repo_name
+            job_data["repo_branch"] = self.repo_data.repo_branch or ""
+            job_data["repo_hash"] = self.repo_data.repo_hash or ""
         return job_data
 
     @staticmethod
     def unserialize(job_data: dict):
         _requirements = job_data.get("requirements")
         requirements = (
             Requirements(
                 cpus=_requirements.get("cpus") or None,
                 memory_mib=_requirements.get("memory_mib") or None,
                 gpus=GpusRequirements(
                     count=_requirements["gpus"].get("count") or None,
-                    memory=_requirements["gpus"].get("memory") or None,
+                    memory_mib=_requirements["gpus"].get("memory") or None,
                     name=_requirements["gpus"].get("name") or None,
                 )
                 if _requirements.get("gpus")
                 else None,
                 shm_size_mib=_requirements.get("shm_size_mib") or None,
                 interruptible=_requirements.get("interruptible") or None,
                 local=_requirements.get("local") or None,
@@ -367,20 +323,15 @@
                 and not not requirements.shm_size_mib
             ):
                 requirements = None
         dep_specs = []
         if job_data.get("deps"):
             for dep in job_data["deps"]:
                 dep_spec = DepSpec(
-                    repo_address=RepoAddress(
-                        repo_host_name=dep["repo_host_name"],
-                        repo_port=dep.get("repo_port") or None,
-                        repo_user_name=dep["repo_user_name"],
-                        repo_name=dep["repo_name"],
-                    ),
+                    repo_ref=RepoRef(repo_id=dep["repo_id"]),
                     run_name=dep["run_name"],
                     mount=dep.get("mount") is True,
                 )
                 dep_specs.append(dep_spec)
         artifact_specs = []
         if job_data.get("artifacts"):
             for artifact in job_data["artifacts"]:
@@ -401,31 +352,43 @@
                     app_name=a["app_name"],
                     url_path=a.get("url_path") or None,
                     url_query_params=a.get("url_query_params") or None,
                 )
                 for a in (job_data.get("apps") or [])
             ]
         ) or None
-        job = Job(
-            job_id=job_data["job_id"],
-            repo_data=RepoData(
+        error_code = job_data.get("error_code")
+        container_exit_code = job_data.get("container_exit_code")
+
+        if job_data["repo_type"] == "remote":
+            repo_data = RemoteRepoData(
                 repo_host_name=job_data["repo_host_name"],
                 repo_port=job_data.get("repo_port") or None,
                 repo_user_name=job_data["repo_user_name"],
                 repo_name=job_data["repo_name"],
                 repo_branch=job_data["repo_branch"] or None,
                 repo_hash=job_data["repo_hash"] or None,
-                repo_diff=job_data["repo_diff"] or None,
-            ),
+            )
+        elif job_data["repo_type"] == "local":
+            repo_data = LocalRepoData(repo_dir=job_data.get("repo_dir", ""))
+        else:
+            raise TypeError(f"Unknown repo_type: {job_data['repo_type']}")
+
+        job = Job(
+            job_id=job_data["job_id"],
+            repo_ref=RepoRef(repo_id=job_data["repo_id"]),
+            hub_user_name=job_data["hub_user_name"],
+            repo_data=repo_data,
+            repo_code_filename=job_data.get("repo_code_filename"),
             run_name=job_data["run_name"],
             workflow_name=job_data.get("workflow_name") or None,
             provider_name=job_data["provider_name"],
-            local_repo_user_name=job_data.get("local_repo_user_name"),
-            local_repo_user_email=job_data.get("local_repo_user_email") or None,
             status=JobStatus(job_data["status"]),
+            error_code=JobErrorCode(error_code) if error_code else None,
+            container_exit_code=int(container_exit_code) if container_exit_code else None,
             submitted_at=job_data["submitted_at"],
             submission_num=job_data.get("submission_num") or 1,
             image_name=job_data["image_name"],
             registry_auth=RegistryAuth(**job_data.get("registry_auth", {})),
             commands=job_data.get("commands") or None,
             entrypoint=job_data.get("entrypoint") or None,
             env=job_data["env"] or None,
@@ -442,17 +405,25 @@
             runner_id=job_data.get("runner_id") or None,
             request_id=job_data.get("request_id") or None,
             tag_name=job_data.get("tag_name") or None,
             ssh_key_pub=job_data.get("ssh_key_pub") or None,
         )
         return job
 
+    @property
+    def repo(self) -> Repo:
+        if isinstance(self.repo_data, RemoteRepoData):
+            return RemoteRepo(repo_ref=self.repo_ref, repo_data=self.repo_data)
+        elif isinstance(self.repo_data, LocalRepoData):
+            return LocalRepo(repo_ref=self.repo_ref, repo_data=self.repo_data)
+
 
 class JobSpec(JobRef):
     image_name: str
+    job_id: Optional[str] = None
     registry_auth: Optional[RegistryAuth] = None
     commands: Optional[List[str]] = None
     entrypoint: Optional[List[str]] = None
     env: Optional[Dict[str, str]] = None
     working_dir: Optional[str] = None
     artifact_specs: Optional[List[ArtifactSpec]] = None
     port_count: Optional[int] = None
```

### Comparing `dstack-0.7rc1/cli/dstack/core/repo.py` & `dstack-0.8/cli/dstack/core/repo/remote.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,148 +1,159 @@
-from enum import Enum
-from typing import Any, Optional, Union
+import os
+import tempfile
+from pathlib import Path
+from typing import Any, BinaryIO, Dict, Optional
 
 import git
+import giturlparse
 from pydantic import BaseModel
+from typing_extensions import Literal
 
-from dstack.utils.common import _quoted, _quoted_masked
+from dstack.core.repo import RepoProtocol
+from dstack.core.repo.base import Repo, RepoData, RepoInfo, RepoRef
+from dstack.utils.common import PathLike
+from dstack.utils.hash import get_sha256, slugify
+from dstack.utils.ssh import get_host_config, make_ssh_command_for_git
+from dstack.utils.workflows import load_workflows
 
 
-class RepoAddress(BaseModel):
-    repo_host_name: str
-    repo_port: Union[int, None]
-    repo_user_name: str
-    repo_name: str
-
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    def __str__(self) -> str:
-        return (
-            f'RepoAddress(repo_host_name="{self.repo_host_name}", '
-            f'repo_port={_quoted(self.repo_port)}", '
-            f'repo_user_name="{self.repo_user_name}", '
-            f'repo_name="{self.repo_name}")'
-        )
-
-    def path(self, delimiter: str = "/"):
-        return (
-            f"{self.repo_host_name}"
-            f"{(':' + str(self.repo_port)) if self.repo_port else ''}{delimiter}"
-            f"{self.repo_user_name}{delimiter}{self.repo_name}"
-        )
-
-
-class RepoHead(RepoAddress):
-    last_run_at: Union[int, None]
-    tags_count: int
-
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    def __str__(self) -> str:
-        return (
-            f'RepoHead(repo_host_name="{self.repo_host_name}", '
-            f'repo_port={_quoted(self.repo_port)}", '
-            f'repo_user_name="{self.repo_user_name}", '
-            f'repo_name="{self.repo_name}", '
-            f'last_run_at="{self.last_run_at}", '
-            f'tags_count="{self.tags_count}")'
-        )
-
-
-class RepoProtocol(Enum):
-    SSH = "ssh"
-    HTTPS = "https"
-
-
-class RepoCredentials(BaseModel):
+class RemoteRepoCredentials(BaseModel):
     protocol: RepoProtocol
-    private_key: Union[str, None]
-    oauth_token: Union[str, None]
-
-    def __str__(self) -> str:
-        return (
-            f"RepoCredentials(protocol=RepoProtocol.{self.protocol.name}, "
-            f"private_key_length={len(self.private_key) if self.private_key else None}, "
-            f"oauth_token={_quoted_masked(self.oauth_token)})"
-        )
-
-
-class RepoData(RepoAddress):
-    repo_branch: Optional[str]
-    repo_hash: Optional[str]
-    repo_diff: Union[str, None]
-
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    def __str__(self) -> str:
-        return (
-            f'RepoData(repo_host_name="{self.repo_host_name}", '
-            f'repo_port={_quoted(self.repo_port)}", '
-            f'repo_user_name="{self.repo_user_name}", '
-            f'repo_name="{self.repo_name}", '
-            f'repo_branch="{_quoted(self.repo_branch)}", '
-            f'repo_hash="{_quoted(self.repo_hash)}", '
-            f"repo_diff_length={len(self.repo_diff) if self.repo_diff else None})"
-        )
+    private_key: Optional[str]
+    oauth_token: Optional[str]
 
 
-class LocalRepoData(RepoData):
-    protocol: RepoProtocol
-    identity_file: Union[str, None]
-    oauth_token: Union[str, None]
-    local_repo_user_name: Union[str, None]
-    local_repo_user_email: Union[str, None]
-
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
-
-    def __str__(self) -> str:
-        return (
-            f'LocalRepoData(repo_host_name="{self.repo_host_name}", '
-            f'repo_port={_quoted(self.repo_port)}", '
-            f'repo_user_name="{self.repo_user_name}", '
-            f'repo_name="{self.repo_name}", '
-            f'repo_branch="{_quoted(self.repo_branch)}", '
-            f'repo_hash="{_quoted(self.repo_hash)}", '
-            f"repo_diff_length={len(self.repo_diff) if self.repo_diff else None}, "
-            f"protocol=RepoProtocol.{self.protocol.name}, "
-            f"identity_file={_quoted(self.identity_file)}, "
-            f"oauth_token={_quoted_masked(self.oauth_token)},"
-            f'local_repo_user_name="{_quoted(self.local_repo_user_name)}, '
-            f"local_repo_user_email={_quoted(self.local_repo_user_email)})"
-        )
+class RemoteRepoInfo(RepoInfo):
+    repo_type: Literal["remote"] = "remote"
+    repo_host_name: str
+    repo_port: Optional[int]
+    repo_user_name: str
+    repo_name: str
 
-    def ls_remote(self) -> str:
-        if self.protocol == RepoProtocol.HTTPS:
-            return git.cmd.Git().ls_remote(
-                f"https://"
-                f"{(self.oauth_token + '@') if self.oauth_token else ''}"
-                f"{self.path()}.git"
-            )
-        else:
-            if self.identity_file:
-                git_ssh_command = (
-                    f"ssh -o IdentitiesOnly=yes -F /dev/null -o IdentityFile={self.identity_file}"
-                )
-                if self.repo_port:
-                    url = f"ssh@{self.path()}.git"
-                else:
-                    url = f"git@{self.repo_host_name}:{self.repo_user_name}/{self.repo_name}.git"
-                return git.cmd.Git().ls_remote(url, env=dict(GIT_SSH_COMMAND=git_ssh_command))
+    @property
+    def head_key(self) -> str:
+        return f"{self.repo_type};{self.repo_host_name},{self.repo_port or ''},{self.repo_user_name},{self.repo_name}"
+
+
+class RemoteRepoData(RepoData, RemoteRepoInfo):
+    repo_type: Literal["remote"] = "remote"
+    repo_branch: Optional[str] = None
+    repo_hash: Optional[str] = None
+    repo_diff: Optional[str] = None
+
+    @staticmethod
+    def from_url(url: str, parse_ssh_config: bool = True):
+        url = giturlparse.parse(url)
+        data = RemoteRepoData(
+            repo_host_name=url.resource,
+            repo_port=url.port,
+            repo_user_name=url.owner,
+            repo_name=url.name,
+        )
+        if parse_ssh_config and url.protocol == "ssh":
+            host_config = get_host_config(data.repo_host_name)
+            data.repo_host_name = host_config.get("hostname", data.repo_host_name)
+            data.repo_port = host_config.get("port", data.repo_port)
+        return data
+
+    def path(self, sep: str = ".") -> str:
+        return sep.join(
+            [
+                self.repo_host_name
+                if self.repo_port is None
+                else f"{self.repo_host_name}:{self.repo_port}",
+                self.repo_user_name,
+                self.repo_name,
+            ]
+        )
+
+    def make_url(self, protocol: RepoProtocol, oauth_token: Optional[str] = None) -> str:
+        if protocol == RepoProtocol.HTTPS:
+            return f"https://{(oauth_token + '@') if oauth_token else ''}{self.path(sep='/')}.git"
+        elif protocol == RepoProtocol.SSH:
+            if self.repo_port:
+                return f"ssh@{self.path(sep='/')}.git"
             else:
-                raise Exception("No identity file is specified")
+                return f"git@{self.repo_host_name}:{self.repo_user_name}/{self.repo_name}.git"
 
-    def repo_credentials(self) -> RepoCredentials:
-        if self.protocol == RepoProtocol.HTTPS:
-            return RepoCredentials(
-                protocol=self.protocol, private_key=None, oauth_token=self.oauth_token
-            )
-        elif self.identity_file:
-            with open(self.identity_file, "r") as f:
-                return RepoCredentials(
-                    protocol=self.protocol, private_key=f.read(), oauth_token=None
-                )
+    def write_code_file(self, fp: BinaryIO) -> str:
+        if self.repo_diff is not None:
+            fp.write(self.repo_diff.encode())
+        return f"code/remote/{get_sha256(fp)}.patch"
+
+
+class RemoteRepo(Repo):
+    """Represents both local git repository with configured remote and just remote repository"""
+
+    repo_data: RemoteRepoData
+
+    def __init__(
+        self,
+        *,
+        repo_ref: Optional[RepoRef] = None,
+        local_repo_dir: Optional[PathLike] = None,
+        repo_url: Optional[str] = None,
+        repo_data: Optional[RemoteRepoData] = None,
+    ):
+        """
+        >>> RemoteRepo(local_repo_dir=os.getcwd())
+        >>> RemoteRepo(repo_ref=RepoRef(repo_id="playground"), repo_url="https://github.com/dstackai/dstack-playground.git")
+        """
+
+        self.local_repo_dir = local_repo_dir
+        self.repo_url = repo_url
+
+        if self.local_repo_dir is not None:
+            repo = git.Repo(self.local_repo_dir)
+            tracking_branch = repo.active_branch.tracking_branch()
+            if tracking_branch is None:
+                raise ValueError("No remote branch is configured")
+            self.repo_url = repo.remote(tracking_branch.remote_name).url
+            repo_data = RemoteRepoData.from_url(self.repo_url, parse_ssh_config=True)
+            repo_data.repo_branch = tracking_branch.remote_head
+            repo_data.repo_hash = tracking_branch.commit.hexsha
+            repo_data.repo_diff = repo.git.diff(
+                repo_data.repo_hash
+            )  # TODO: Doesn't support unstaged changes
+        elif self.repo_url is not None:
+            repo_data = RemoteRepoData.from_url(self.repo_url, parse_ssh_config=True)
+        elif repo_data is None:
+            raise ValueError("No remote repo data provided")
+
+        if repo_ref is None:
+            repo_ref = RepoRef(repo_id=slugify(repo_data.repo_name, repo_data.path("/")))
+        super().__init__(repo_ref, repo_data)
+
+    def get_workflows(
+        self, credentials: Optional[RemoteRepoCredentials] = None
+    ) -> Dict[str, Dict[str, Any]]:
+        if self.local_repo_dir is not None:
+            local_repo_dir = Path(self.local_repo_dir)
+        elif credentials is None:
+            raise RuntimeError("No credentials for remote only repo")
         else:
-            raise Exception("No identity file is specified")
+            temp_dir = tempfile.TemporaryDirectory()  # will be removed by garbage collector
+            local_repo_dir = Path(temp_dir.name)
+            _clone_remote_repo(local_repo_dir, self.repo_data, credentials, depth=1)
+        return load_workflows(local_repo_dir / ".dstack")
+
+
+def _clone_remote_repo(
+    dst: PathLike, repo_data: RemoteRepoData, repo_credentials: RemoteRepoCredentials, **kwargs
+):
+    env = kwargs.pop("env", {})
+    if repo_credentials.protocol == RepoProtocol.HTTPS:
+        env["GIT_TERMINAL_PROMPT"] = "0"
+    elif repo_credentials.protocol == RepoProtocol.SSH:
+        tmp_identity_file = tempfile.NamedTemporaryFile(
+            "w+b"
+        )  # will be removed by garbage collector
+        tmp_identity_file.write(repo_credentials.private_key.encode())
+        tmp_identity_file.seek(0)
+        env["GIT_SSH_COMMAND"] = make_ssh_command_for_git(tmp_identity_file.name)
+    git.Repo.clone_from(
+        url=repo_data.make_url(repo_credentials.protocol, repo_credentials.oauth_token),
+        to_path=dst,
+        env=env,
+        **kwargs,
+    )
+    # todo checkout branch/hash
```

### Comparing `dstack-0.7rc1/cli/dstack/core/request.py` & `dstack-0.8/cli/dstack/core/request.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/core/runners.py` & `dstack-0.8/cli/dstack/core/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/hub/background/tasks/resubmit_jobs.py` & `dstack-0.8/cli/dstack/hub/background/tasks/resubmit_jobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,27 +19,28 @@
     for project in projects:
         _resubmit_project_jobs(project)
 
 
 def _resubmit_project_jobs(project: Project):
     curr_time = get_milliseconds_since_epoch()
     backend = get_backend(project)
-    repo_heads = backend.list_repo_heads()
-    for repo_head in repo_heads:
+    for repo_head in backend.list_repo_heads():
         run_heads = backend.list_run_heads(
-            repo_address=repo_head,
+            repo_id=repo_head.repo_id,
             run_name=None,
             include_request_heads=True,
             interrupted_job_new_status=JobStatus.PENDING,
         )
         for run_head in run_heads:
-            job_heads = backend.list_job_heads(repo_address=repo_head, run_name=run_head.run_name)
+            job_heads = backend.list_job_heads(
+                repo_id=repo_head.repo_id, run_name=run_head.run_name
+            )
             for job_head in job_heads:
                 if (
                     job_head.status == JobStatus.PENDING
                     and curr_time - job_head.submitted_at > RESUBMISSION_INTERVAL * 1000
                 ):
-                    job = backend.get_job(repo_head, job_head.job_id)
+                    job = backend.get_job(repo_id=repo_head.repo_id, job_id=job_head.job_id)
                     backend.resubmit_job(
                         job=job,
                         failed_to_start_job_new_status=JobStatus.PENDING,
                     )
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/db/__init__.py` & `dstack-0.8/cli/dstack/hub/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/hub/db/models.py` & `dstack-0.8/cli/dstack/hub/db/models.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/hub/migration/env.py` & `dstack-0.8/cli/dstack/hub/migration/env.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/hub/migration/versions/3b900659c822_.py` & `dstack-0.8/cli/dstack/hub/migration/versions/3b900659c822_.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/hub/models/__init__.py` & `dstack-0.8/cli/dstack/hub/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from datetime import datetime
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Field
 from typing_extensions import Literal
 
-from dstack.core.job import Job, JobHead
-from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials
+from dstack.core.job import Job
+from dstack.core.repo import RemoteRepoCredentials, RepoSpec
 from dstack.core.secret import Secret
 from dstack.hub.security.utils import GlobalRole, ProjectRole
 
 
 class UserInfo(BaseModel):
     user_name: str
     global_role: GlobalRole
@@ -25,14 +26,22 @@
 
 
 class Member(BaseModel):
     user_name: str
     project_role: ProjectRole
 
 
+BackendType = Union[Literal["local"], Literal["aws"], Literal["gcp"]]
+
+
+class LocalProjectConfig(BaseModel):
+    type: Literal["local"] = "local"
+    path: Optional[str]
+
+
 class AWSProjectConfigPartial(BaseModel):
     type: Literal["aws"] = "aws"
     region_name: Optional[str]
     region_name_title: Optional[str]
     s3_bucket_name: Optional[str]
     ec2_subnet_id: Optional[str]
 
@@ -87,19 +96,21 @@
     pass
 
 
 class GCPProjectConfigWithCreds(GCPProjectConfig, GCPProjectCreds):
     pass
 
 
-AnyProjectConfig = Union[AWSProjectConfig, GCPProjectConfig]
+AnyProjectConfig = Union[LocalProjectConfig, AWSProjectConfig, GCPProjectConfig]
 AnyProjectConfigWithCredsPartial = Union[
-    AWSProjectConfigWithCredsPartial, GCPProjectConfigWithCredsPartial
+    LocalProjectConfig, AWSProjectConfigWithCredsPartial, GCPProjectConfigWithCredsPartial
+]
+AnyProjectConfigWithCreds = Union[
+    LocalProjectConfig, AWSProjectConfigWithCreds, GCPProjectConfigWithCreds
 ]
-AnyProjectConfigWithCreds = Union[AWSProjectConfigWithCreds, GCPProjectConfigWithCreds]
 
 
 class ProjectConfig(BaseModel):
     __root__: AnyProjectConfig = Field(..., discriminator="type")
 
 
 class ProjectConfigWithCredsPartial(BaseModel):
@@ -119,76 +130,88 @@
 class ProjectInfoWithCreds(BaseModel):
     project_name: str
     backend: ProjectConfigWithCreds
     members: List[Member] = []
 
 
 class AddTagRun(BaseModel):
-    repo_address: RepoAddress
+    repo_id: str
     tag_name: str
     run_name: str
     run_jobs: Optional[List[Job]]
 
 
 class AddTagPath(BaseModel):
-    repo_data: LocalRepoData
+    repo_spec: RepoSpec
     tag_name: str
     local_dirs: List[str]
 
 
 class StopRunners(BaseModel):
-    repo_address: RepoAddress
+    repo_id: str
     job_id: str
     abort: bool
 
 
 class SaveRepoCredentials(BaseModel):
-    repo_address: RepoAddress
-    repo_credentials: RepoCredentials
+    repo_id: str
+    repo_credentials: RemoteRepoCredentials
+
+
+class RepoHeadGet(BaseModel):
+    repo_id: str
 
 
 class ReposUpdate(BaseModel):
-    repo_address: RepoAddress
+    repo_spec: RepoSpec
     last_run_at: int
 
 
 class RunsList(BaseModel):
-    repo_address: RepoAddress
+    repo_id: str
     run_name: Optional[str]
     include_request_heads: Optional[bool]
 
 
+class JobHeadList(BaseModel):
+    repo_id: str
+    run_name: Optional[str]
+
+
 class JobsGet(BaseModel):
-    repo_address: RepoAddress
+    repo_id: str
     job_id: str
 
 
 class JobsList(BaseModel):
-    repo_address: RepoAddress
+    repo_id: str
     run_name: str
 
 
 class ArtifactsList(BaseModel):
-    repo_address: RepoAddress
+    repo_id: str
     run_name: str
 
 
 class SecretAddUpdate(BaseModel):
-    repo_address: RepoAddress
+    repo_id: str
     secret: Secret
 
 
 class PollLogs(BaseModel):
-    repo_address: RepoAddress
-    job_heads: List[JobHead]
-    start_time: int
-    attached: bool
+    repo_id: str
+    run_name: str
+    start_time: Optional[datetime]
+    end_time: Optional[datetime]
+    descending: bool = False
+    prev_event_id: Optional[str]
+    limit: int = Field(100, ge=0, le=1000)
 
 
-class LinkUpload(BaseModel):
+class StorageLink(BaseModel):
     object_key: str
 
 
 class ProjectDelete(BaseModel):
     projects: List[str] = []
 
 
@@ -204,20 +227,14 @@
 
 class AWSBucketProjectElementValue(BaseModel):
     name: str
     created: str
     region: str
 
 
-class AWSBucketProjectElementValue(BaseModel):
-    name: str
-    created: str
-    region: str
-
-
 class AWSBucketProjectElement(BaseModel):
     selected: Optional[str]
     values: List[AWSBucketProjectElementValue] = []
 
 
 class AWSProjectValues(BaseModel):
     type: Literal["aws"] = "aws"
@@ -243,25 +260,24 @@
     region: Optional[ProjectElement]
     zone: Optional[ProjectElement]
     bucket_name: Optional[ProjectElement]
     vpc_subnet: Optional[GCPVPCSubnetProjectElement]
 
 
 class ProjectValues(BaseModel):
-    __root__: Union[AWSProjectValues, GCPProjectValues] = Field(..., discriminator="type")
+    __root__: Union[None, AWSProjectValues, GCPProjectValues] = Field(..., discriminator="type")
 
 
 class UserPatch(BaseModel):
     global_role: GlobalRole
 
 
 class AddMembers(BaseModel):
     members: List[Member] = []
 
 
 class DeleteUsers(BaseModel):
     users: List[str] = []
 
 
-class UserRepoAddress(BaseModel):
-    username: str  # fixme: use auth username
-    repo_address: RepoAddress
+class FileObject(BaseModel):
+    object_key: str
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/repository/projects.py` & `dstack-0.8/cli/dstack/hub/repository/projects.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 from dstack.hub.models import (
     AWSProjectConfig,
     AWSProjectConfigWithCreds,
     AWSProjectCreds,
     GCPProjectConfig,
     GCPProjectConfigWithCreds,
     GCPProjectCreds,
+    LocalProjectConfig,
     Member,
     ProjectInfo,
     ProjectInfoWithCreds,
 )
 from dstack.hub.security.utils import ROLE_ADMIN
+from dstack.hub.services.backends.local import LocalConfigurator
 
 
 class ProjectManager:
     @staticmethod
     async def get_project_info_with_creds(project: Project) -> Optional[ProjectInfoWithCreds]:
         return _project2info(project=project, include_creds=True)
 
@@ -39,14 +41,26 @@
         project = _info2project(project_info)
         await ProjectManager.create(project, session=session)
         await ProjectManager._add_member(
             project, Member(user_name=user.name, project_role=ROLE_ADMIN)
         )
 
     @staticmethod
+    @reuse_or_make_session
+    async def create_local_project(
+        user: User, project_name: str, session: Optional[AsyncSession] = None
+    ):
+        project_info = ProjectInfoWithCreds(
+            project_name=project_name, backend=LocalProjectConfig()
+        )
+        await ProjectManager.create_project_from_info(
+            user=user, project_info=project_info, session=session
+        )
+
+    @staticmethod
     async def update_project_from_info(
         project_info: ProjectInfoWithCreds, session: Optional[AsyncSession] = None
     ):
         project = _info2project(project_info)
         await ProjectManager.update(project, session=session)
 
     @staticmethod
@@ -145,21 +159,24 @@
 
 def _info2project(project_info: ProjectInfoWithCreds) -> Project:
     project_info.backend = project_info.backend.__root__
     project = Project(
         name=project_info.project_name,
         backend=project_info.backend.type,
     )
-    if project_info.backend.type == "aws":
+    if project_info.backend.type == "local":
+        project.config = "{}"
+        project.auth = "{}"
+    elif project_info.backend.type == "aws":
         project_info.backend.s3_bucket_name = project_info.backend.s3_bucket_name.replace(
             "s3://", ""
         )
         project.config = AWSProjectConfig.parse_obj(project_info.backend).json()
         project.auth = AWSProjectCreds.parse_obj(project_info.backend).json()
-    if project_info.backend.type == "gcp":
+    elif project_info.backend.type == "gcp":
         project.config = GCPProjectConfig.parse_obj(project_info.backend).json()
         project.auth = GCPProjectCreds.parse_obj(project_info.backend).json()
     return project
 
 
 def _project2info(
     project: Project, include_creds: bool = False
@@ -168,24 +185,32 @@
     for member in project.members:
         members.append(
             Member(
                 user_name=member.user_name,
                 project_role=member.project_role,
             )
         )
-    backend = None
+    if project.backend == "local":
+        backend = _local(project)
     if project.backend == "aws":
         backend = _aws(project, include_creds=include_creds)
     if project.backend == "gcp":
         backend = _gcp(project, include_creds=include_creds)
     if include_creds:
         return ProjectInfoWithCreds(project_name=project.name, backend=backend, members=members)
     return ProjectInfo(project_name=project.name, backend=backend, members=members)
 
 
+def _local(project: Project) -> LocalProjectConfig:
+    config = LocalConfigurator().get_config_from_hub_config_data(
+        project.name, project.config, project.auth
+    )
+    return LocalProjectConfig(path=str(config.backend_dir))
+
+
 def _aws(
     project: Project, include_creds: bool
 ) -> Union[AWSProjectConfig, AWSProjectConfigWithCreds]:
     json_config = json.loads(project.config)
     region_name = json_config["region_name"]
     s3_bucket_name = json_config["s3_bucket_name"]
     ec2_subnet_id = json_config["ec2_subnet_id"]
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/repository/users.py` & `dstack-0.8/cli/dstack/hub/repository/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/artifacts.py` & `dstack-0.8/cli/dstack/hub/routers/artifacts.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 )
 
 
 @router.post("/{project_name}/artifacts/list")
 async def list_artifacts(project_name: str, body: ArtifactsList) -> List[Artifact]:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    return backend.list_run_artifact_files(repo_address=body.repo_address, run_name=body.run_name)
+    return backend.list_run_artifact_files(repo_id=body.repo_id, run_name=body.run_name)
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/jobs.py` & `dstack-0.8/cli/dstack/hub/routers/jobs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing import List, Optional
+from typing import List
 
 from fastapi import APIRouter, Depends
 
 from dstack.core.job import Job, JobHead
-from dstack.core.repo import RepoAddress
-from dstack.hub.models import JobsGet, JobsList
+from dstack.hub.db.models import User
+from dstack.hub.models import JobHeadList, JobsGet, JobsList
 from dstack.hub.routers.cache import get_backend
 from dstack.hub.routers.util import get_project
-from dstack.hub.security.permissions import ProjectMember
+from dstack.hub.security.permissions import Authenticated, ProjectMember
 
 router = APIRouter(prefix="/api/project", tags=["jobs"], dependencies=[Depends(ProjectMember())])
 
 
 @router.post("/{project_name}/jobs/create")
-async def create_job(project_name: str, job: Job):
+async def create_job(project_name: str, job: Job, user: User = Depends(Authenticated())) -> Job:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
+    job.hub_user_name = user.name
     backend.create_job(job=job)
+    return job
 
 
 @router.post("/{project_name}/jobs/get")
 async def get_job(project_name: str, body: JobsGet) -> Job:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    return backend.get_job(repo_address=body.repo_address, job_id=body.job_id)
+    return backend.get_job(repo_id=body.repo_id, job_id=body.job_id)
 
 
 @router.post("/{project_name}/jobs/list")
 async def list_job(project_name: str, body: JobsList) -> List[Job]:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    return backend.list_jobs(repo_address=body.repo_address, run_name=body.run_name)
+    return backend.list_jobs(repo_id=body.repo_id, run_name=body.run_name)
 
 
 @router.post("/{project_name}/jobs/list/heads")
-async def list_heads_job(
-    project_name: str, repo_address: RepoAddress, run_name: Optional[str] = None
-) -> List[JobHead]:
+async def list_job_heads(project_name: str, body: JobHeadList) -> List[JobHead]:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    return backend.list_job_heads(repo_address=repo_address, run_name=run_name)
+    return backend.list_job_heads(repo_id=body.repo_id, run_name=body.run_name)
 
 
 @router.post("/{project_name}/jobs/delete")
 async def delete_job(project_name: str, body: JobsGet):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    backend.delete_job_head(repo_address=body.repo_address, job_id=body.job_id)
+    backend.delete_job_head(repo_id=body.repo_id, job_id=body.job_id)
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/projects.py` & `dstack-0.8/cli/dstack/hub/routers/projects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import asyncio
 from typing import List, Tuple
 
 from fastapi import APIRouter, Body, Depends, HTTPException, status
 
-from dstack.api.backend import dict_backends
-from dstack.backend.base import Backend
-from dstack.core.error import HubConfigError
 from dstack.hub.db.models import Project, User
 from dstack.hub.models import (
     Member,
     ProjectConfigWithCredsPartial,
     ProjectDelete,
     ProjectInfo,
     ProjectInfoWithCreds,
@@ -20,30 +17,31 @@
 from dstack.hub.routers.util import error_detail, get_project
 from dstack.hub.security.permissions import (
     Authenticated,
     ProjectAdmin,
     ProjectMember,
     ensure_user_project_admin,
 )
+from dstack.hub.services.backends import get_configurator, local_backend_available
+from dstack.hub.services.backends.base import BackendConfigError, Configurator
 
 router = APIRouter(prefix="/api/projects", tags=["project"])
 
 
 @router.post("/backends/values")
 async def get_backend_config_values(
     config: ProjectConfigWithCredsPartial = Body(),
     user: User = Depends(Authenticated()),
 ) -> ProjectValues:
-    backend = _get_backend(config.__root__.type)
-    configurator = backend.get_configurator()
+    configurator = _get_backend_configurator(config.__root__.type)
     try:
         result = await asyncio.get_running_loop().run_in_executor(
             None, configurator.configure_hub, config.__root__.dict()
         )
-    except HubConfigError as e:
+    except BackendConfigError as e:
         _error_response_on_config_error(e, path_to_config=[])
     return result
 
 
 @router.get(
     "/list",
 )
@@ -61,21 +59,27 @@
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=[
                 error_detail(
                     "Project exists", code="project_name_not_unique", loc=["project_name"]
                 )
             ],
         )
-    backend = _get_backend(project_info.backend.__root__.type)
-    configurator = backend.get_configurator()
+    configurator = _get_backend_configurator(project_info.backend.__root__.type)
+    if configurator.name == "local" and not local_backend_available():
+        raise HTTPException(
+            status_code=status.HTTP_400_BAD_REQUEST,
+            detail=[
+                error_detail("Local backend not available", code="local_backend_not_available")
+            ],
+        )
     try:
         await asyncio.get_running_loop().run_in_executor(
             None, configurator.configure_hub, project_info.backend.__root__.dict()
         )
-    except HubConfigError as e:
+    except BackendConfigError as e:
         _error_response_on_config_error(e, path_to_config=["backend"])
     await ProjectManager.create_project_from_info(user=user, project_info=project_info)
     return project_info
 
 
 @router.delete("")
 async def delete_projects(body: ProjectDelete, user: User = Depends(Authenticated())):
@@ -115,38 +119,37 @@
 
 
 @router.patch("/{project_name}")
 async def update_project(
     project_info: ProjectInfoWithCreds = Body(),
     user_project: Tuple[User, Project] = Depends(ProjectAdmin()),
 ) -> ProjectInfoWithCreds:
-    backend = _get_backend(project_info.backend.__root__.type)
-    configurator = backend.get_configurator()
+    configurator = _get_backend_configurator(project_info.backend.__root__.type)
     try:
         await asyncio.get_running_loop().run_in_executor(
             None, configurator.configure_hub, project_info.backend.__root__.dict()
         )
-    except HubConfigError as e:
+    except BackendConfigError as e:
         _error_response_on_config_error(e, path_to_config=["backend"])
     await ProjectManager.update_project_from_info(project_info)
     clear_backend_cache(project_info.project_name)
     return project_info
 
 
-def _get_backend(backend_type: str) -> Backend:
-    backend = dict_backends(all_backend=True).get(backend_type)
-    if backend is None:
+def _get_backend_configurator(backend_type: str) -> Configurator:
+    configurator = get_configurator(backend_type)
+    if configurator is None:
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=error_detail(f"Unknown backend {backend_type}"),
         )
-    return backend
+    return configurator
 
 
-def _error_response_on_config_error(e: HubConfigError, path_to_config: List[str]):
+def _error_response_on_config_error(e: BackendConfigError, path_to_config: List[str]):
     if len(e.fields) > 0:
         error_details = [
             error_detail(e.message, code=e.code, loc=path_to_config + [f]) for f in e.fields
         ]
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=error_details,
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/repos.py` & `dstack-0.8/cli/dstack/hub/routers/repos.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,66 @@
+from typing import List
+
 from fastapi import APIRouter, Depends, HTTPException, status
 
-from dstack.core.repo import RepoAddress, RepoCredentials
-from dstack.hub.models import ReposUpdate, SaveRepoCredentials
+from dstack.core.repo import RemoteRepoCredentials, RepoHead, RepoRef
+from dstack.hub.models import RepoHeadGet, ReposUpdate, SaveRepoCredentials
 from dstack.hub.routers.cache import get_backend
 from dstack.hub.routers.util import error_detail, get_project
 from dstack.hub.security.permissions import ProjectMember
 
 router = APIRouter(prefix="/api/project", tags=["repos"], dependencies=[Depends(ProjectMember())])
 
 
+@router.post("/{project_name}/repos/heads/list")
+async def list_repo_heads(project_name: str) -> List[RepoHead]:
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
+    return backend.list_repo_heads()
+
+
+@router.post("/{project_name}/repos/heads/get")
+async def get_repo_head(project_name: str, body: RepoHeadGet) -> RepoHead:
+    project = await get_project(project_name=project_name)
+    backend = get_backend(project)
+    repo_heads = backend.list_repo_heads()
+    for repo_head in repo_heads:
+        if repo_head.repo_id == body.repo_id:
+            return repo_head
+    raise HTTPException(
+        status_code=status.HTTP_404_NOT_FOUND,
+        detail=error_detail("Repo not found"),
+    )
+
+
 @router.post("/{project_name}/repos/credentials/save")
 async def save_repo_credentials(
     project_name: str, save_repo_credentials_body: SaveRepoCredentials
 ):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
     backend.save_repo_credentials(
-        repo_address=save_repo_credentials_body.repo_address,
+        save_repo_credentials_body.repo_id,
         repo_credentials=save_repo_credentials_body.repo_credentials,
     )
 
 
 @router.post(
     "/{project_name}/repos/credentials/get",
 )
-async def get_repo_credentials(project_name: str, repo_address: RepoAddress) -> RepoCredentials:
+async def get_repo_credentials(project_name: str, repo_ref: RepoRef) -> RemoteRepoCredentials:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    repo_credentials = backend.get_repo_credentials(repo_address=repo_address)
+    repo_credentials = backend.get_repo_credentials(repo_ref.repo_id)
     if repo_credentials is None:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=error_detail("Repo credentials not found"),
         )
     return repo_credentials
 
 
 @router.post("/{project_name}/repos/update")
 async def update_repo(project_name: str, body: ReposUpdate):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    backend.update_repo_last_run_at(repo_address=body.repo_address, last_run_at=body.last_run_at)
+    backend.update_repo_last_run_at(body.repo_spec, last_run_at=body.last_run_at)
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/runners.py` & `dstack-0.8/cli/dstack/hub/routers/runners.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-from fastapi import APIRouter, Depends
+from fastapi import APIRouter, Depends, HTTPException, status
 
+from dstack.core.error import NoMatchingInstanceError
 from dstack.core.job import Job, JobStatus
 from dstack.hub.models import StopRunners
 from dstack.hub.routers.cache import get_backend
-from dstack.hub.routers.util import get_project
+from dstack.hub.routers.util import error_detail, get_project
 from dstack.hub.security.permissions import ProjectMember
 
 router = APIRouter(
     prefix="/api/project", tags=["runners"], dependencies=[Depends(ProjectMember())]
 )
 
 
 @router.post("/{project_name}/runners/run")
 async def run_runners(project_name: str, job: Job):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    backend.run_job(job=job, failed_to_start_job_new_status=JobStatus.PENDING)
+    try:
+        backend.run_job(job=job, failed_to_start_job_new_status=JobStatus.PENDING)
+    except NoMatchingInstanceError as e:
+        raise HTTPException(
+            status_code=status.HTTP_400_BAD_REQUEST,
+            detail=error_detail(e.message, code=NoMatchingInstanceError.code),
+        )
 
 
 @router.post("/{project_name}/runners/stop")
 async def stop_runners(project_name: str, body: StopRunners):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    backend.stop_job(repo_address=body.repo_address, job_id=body.job_id, abort=body.abort)
+    backend.stop_job(body.repo_id, abort=body.abort, job_id=body.job_id)
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/runs.py` & `dstack-0.8/cli/dstack/hub/routers/runs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-from typing import List, Union
+from typing import List
 
 from fastapi import APIRouter, Depends
 from fastapi.responses import PlainTextResponse
 
 from dstack.core.job import JobStatus
-from dstack.core.repo import RepoAddress
+from dstack.core.repo import RepoRef
 from dstack.core.run import RunHead
 from dstack.hub.models import RunsList
 from dstack.hub.routers.cache import get_backend
 from dstack.hub.routers.util import get_project
 from dstack.hub.security.permissions import ProjectMember
 
 router = APIRouter(prefix="/api/project", tags=["runs"], dependencies=[Depends(ProjectMember())])
 
 
 @router.post(
     "/{project_name}/runs/create",
     response_model=str,
     response_class=PlainTextResponse,
 )
-async def create_run(project_name: str, repo_address: RepoAddress) -> str:
+async def create_run(project_name: str, repo_ref: RepoRef) -> str:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    run_name = backend.create_run(repo_address=repo_address)
+    run_name = backend.create_run(repo_ref.repo_id)
     return run_name
 
 
 @router.post(
     "/{project_name}/runs/list",
-    response_model=List[RunHead],
 )
-async def list_run(project_name: str, body: RunsList):
+async def list_run(project_name: str, body: RunsList) -> List[RunHead]:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    run_name = backend.list_run_heads(
-        repo_address=body.repo_address,
+    run_heads = backend.list_run_heads(
+        repo_id=body.repo_id,
         run_name=body.run_name,
         include_request_heads=body.include_request_heads,
         interrupted_job_new_status=JobStatus.PENDING,
     )
-    return run_name
+    return run_heads
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/secrets.py` & `dstack-0.8/cli/dstack/hub/routers/secrets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from typing import List, Optional
+from typing import List
 
 from fastapi import APIRouter, Depends, HTTPException, status
 
-from dstack.core.repo import RepoAddress
+from dstack.core.repo import RepoRef
 from dstack.core.secret import Secret
 from dstack.hub.models import SecretAddUpdate
 from dstack.hub.routers.cache import get_backend
 from dstack.hub.routers.util import error_detail, get_project
 from dstack.hub.security.permissions import ProjectMember
 
 router = APIRouter(
     prefix="/api/project", tags=["secrets"], dependencies=[Depends(ProjectMember())]
 )
 
 
 @router.post("/{project_name}/secrets/list")
-async def list_secrets(project_name: str, repo_address: RepoAddress) -> List[str]:
+async def list_secrets(project_name: str, repo_ref: RepoRef) -> List[str]:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    return backend.list_secret_names(repo_address=repo_address)
+    return backend.list_secret_names(repo_ref.repo_id)
 
 
 @router.post("/{project_name}/secrets/add")
 async def add_secret(project_name: str, body: SecretAddUpdate):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    backend.add_secret(repo_address=body.repo_address, secret=body.secret)
+    backend.add_secret(body.repo_id, secret=body.secret)
 
 
 @router.post("/{project_name}/secrets/update")
 async def update_secret(project_name: str, body: SecretAddUpdate):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    backend.update_secret(repo_address=body.repo_address, secret=body.secret)
+    backend.update_secret(body.repo_id, secret=body.secret)
 
 
 @router.post("/{project_name}/secrets/{secret_name}/get")
-async def get_secret(project_name: str, secret_name: str, repo_address: RepoAddress) -> Secret:
+async def get_secret(project_name: str, secret_name: str, repo_ref: RepoRef) -> Secret:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    secret = backend.get_secret(repo_address=repo_address, secret_name=secret_name)
+    secret = backend.get_secret(repo_ref.repo_id, secret_name=secret_name)
     if secret is None:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND, detail=error_detail("Secret not found")
         )
     return secret
 
 
 @router.post("/{project_name}/secrets/{secret_name}/delete")
-async def delete_secret(project_name: str, secret_name: str, repo_address: RepoAddress):
+async def delete_secret(project_name: str, secret_name: str, repo_ref: RepoRef):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    backend.delete_secret(repo_address=repo_address, secret_name=secret_name)
+    backend.delete_secret(repo_ref.repo_id, secret_name=secret_name)
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/tags.py` & `dstack-0.8/cli/dstack/hub/routers/tags.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,63 @@
-from typing import List, Union
+from typing import List
 
 from fastapi import APIRouter, Depends, HTTPException, status
 
-from dstack.core.repo import RepoAddress
+from dstack.core.repo import RepoRef
 from dstack.core.tag import TagHead
 from dstack.hub.models import AddTagPath, AddTagRun
 from dstack.hub.routers.cache import get_backend
 from dstack.hub.routers.util import error_detail, get_project
 from dstack.hub.security.permissions import ProjectMember
 
 router = APIRouter(prefix="/api/project", tags=["tags"], dependencies=[Depends(ProjectMember())])
 
 
 @router.post(
     "/{project_name}/tags/list/heads",
     response_model=List[TagHead],
 )
-async def list_heads_tags(project_name: str, repo_address: RepoAddress):
+async def list_heads_tags(project_name: str, repo_ref: RepoRef):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    list_tag = backend.list_tag_heads(repo_address=repo_address)
+    list_tag = backend.list_tag_heads(repo_ref.repo_id)
     return list_tag
 
 
 @router.post(
     "/{project_name}/tags/{tag_name}",
     response_model=TagHead,
 )
-async def get_tag(project_name: str, tag_name: str, repo_address: RepoAddress) -> TagHead:
+async def get_tag(project_name: str, tag_name: str, repo_ref: RepoRef) -> TagHead:
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    tag = backend.get_tag_head(repo_address=repo_address, tag_name=tag_name)
+    tag = backend.get_tag_head(repo_ref.repo_id, tag_name=tag_name)
     if tag is None:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND, detail=error_detail("Tag not found")
         )
     return tag
 
 
 @router.post("/{project_name}/tags/{tag_name}/delete")
-async def delete_tag(project_name: str, tag_name: str, repo_address: RepoAddress):
+async def delete_tag(project_name: str, tag_name: str, repo_ref: RepoRef):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
-    tag = backend.get_tag_head(repo_address=repo_address, tag_name=tag_name)
-    backend.delete_tag_head(repo_address=repo_address, tag_head=tag)
+    tag = backend.get_tag_head(repo_ref.repo_id, tag_name=tag_name)
+    backend.delete_tag_head(repo_ref.repo_id, tag_head=tag)
 
 
 @router.post("/{project_name}/tags/add/run")
 async def add_tag_from_run(project_name: str, body: AddTagRun):
     project = await get_project(project_name=project_name)
     backend = get_backend(project)
     backend.add_tag_from_run(
-        repo_address=body.repo_address,
-        tag_name=body.tag_name,
-        run_name=body.run_name,
-        run_jobs=body.run_jobs,
+        body.repo_id, tag_name=body.tag_name, run_name=body.run_name, run_jobs=body.run_jobs
     )
 
 
 @router.post("/{project_name}/tags/add/path")
 async def add_tag_from_path(project_name: str, body: AddTagPath):
-    project = await get_project(project_name=project_name)
-    backend = get_backend(project)
-    backend.add_tag_from_local_dirs(
-        repo_data=body.repo_data, tag_name=body.tag_name, local_dirs=body.local_dirs
-    )
+    # project = await get_project(project_name=project_name)
+    # backend = get_backend(project)
+    # backend.add_tag_from_local_dirs(tag_name=body.tag_name, local_dirs=body.local_dirs)
+    raise NotImplementedError()
```

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/users.py` & `dstack-0.8/cli/dstack/hub/routers/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/hub/routers/util.py` & `dstack-0.8/cli/dstack/hub/routers/util.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/hub/security/permissions.py` & `dstack-0.8/cli/dstack/hub/security/permissions.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/providers/__init__.py` & `dstack-0.8/cli/dstack/providers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import importlib
 import shlex
 import sys
+import tempfile
 from abc import abstractmethod
 from argparse import ArgumentParser, Namespace
 from pkgutil import iter_modules
 from typing import Any, Dict, List, Optional, Union
 
-from dstack.api.repo import load_repo_data
-from dstack.backend.base import Backend
+import dstack.api.hub as hub
 from dstack.core.cache import CacheSpec
+from dstack.core.error import RepoNotInitializedError
 from dstack.core.job import (
     ArtifactSpec,
     DepSpec,
     GpusRequirements,
     Job,
     JobSpec,
     JobStatus,
     Requirements,
 )
-from dstack.core.repo import RepoAddress, RepoData
 from dstack.utils.common import _quoted, get_milliseconds_since_epoch
 from dstack.utils.interpolator import VariablesInterpolator
 
 DEFAULT_CPU = 2
 DEFAULT_MEM = "8GB"
 
 
@@ -119,31 +119,43 @@
         elif isinstance(obj, list):
             return [Provider._inject_context_recursively(interpolator, item) for item in obj]
         else:
             return obj
 
     def load(
         self,
-        backend: Backend,
-        provider_args: List[str],
+        hub_client: "hub.HubClient",
+        args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
+        ssh_key_pub: Optional[str] = None,
     ):
-        self.provider_args = provider_args
+        if getattr(args, "help", False):
+            self.help(workflow_name)
+            exit()  # todo: find a better place for this
+
+        self.provider_args = [] if args is None else args.args + args.unknown
         self.workflow_name = workflow_name
         self.provider_data = provider_data
         self.run_as_provider = not workflow_name
         self.run_name = run_name
+        self.ssh_key_pub = ssh_key_pub
         self.openssh_server = self.provider_data.get("ssh", False)
         self.parse_args()
+        if not self.ssh_key_pub:
+            if self.openssh_server or (
+                hub_client.get_project_backend_type() != "local" and not args.detach
+            ):
+                raise RepoNotInitializedError(
+                    "No valid SSH identity", project_name=hub_client.project
+                )
         self._inject_context()
-        self.dep_specs = self._dep_specs(backend)
+        self.dep_specs = self._dep_specs(hub_client)
         self.cache_specs = self._cache_specs()
-        self.ssh_key_pub = self.provider_data.get("ssh_key_pub")
         self.loaded = True
 
     @abstractmethod
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
         return None
 
     def help(self, workflow_name: Optional[str]):
@@ -212,30 +224,35 @@
             resources["interruptible"] = True
         if unknown_args:
             self.provider_data["run_args"] = unknown_args
 
     def parse_args(self):
         pass
 
-    def submit_jobs(self, backend: Backend, tag_name: str) -> List[Job]:
+    def submit_jobs(self, hub_client: "hub.HubClient", tag_name: str) -> List[Job]:
         if not self.loaded:
             raise Exception("The provider is not loaded")
         job_specs = self.create_job_specs()
-        repo_data = load_repo_data()
+
+        with tempfile.NamedTemporaryFile("w+b") as f:
+            repo_code_filename = hub_client.repo.repo_data.write_code_file(f)
+            f.seek(0)
+            hub_client._storage.upload_file(f.name, repo_code_filename, lambda _: ...)
+
         # [TODO] Handle master job
         jobs = []
         for i, job_spec in enumerate(job_specs):
             job = Job(
                 job_id=f"{self.run_name},{self.workflow_name or ''},{i}",
-                repo_data=repo_data,
+                repo_ref=hub_client.repo.repo_ref,
+                hub_user_name="",  # HUB will fill it later
+                repo_data=hub_client.repo.repo_data,
                 run_name=self.run_name,
                 workflow_name=self.workflow_name or None,
                 provider_name=self.provider_name,
-                local_repo_user_name=repo_data.local_repo_user_name,
-                local_repo_user_email=repo_data.local_repo_user_email,
                 status=JobStatus.SUBMITTED,
                 submitted_at=get_milliseconds_since_epoch(),
                 image_name=job_spec.image_name,
                 registry_auth=job_spec.registry_auth,
                 commands=job_spec.commands,
                 entrypoint=job_spec.entrypoint,
                 env=job_spec.env,
@@ -249,27 +266,25 @@
                 dep_specs=self.dep_specs,
                 master_job=job_spec.master_job,
                 app_specs=job_spec.app_specs,
                 runner_id=None,
                 request_id=None,
                 tag_name=tag_name,
                 ssh_key_pub=self.ssh_key_pub,
+                repo_code_filename=repo_code_filename,
             )
-            backend.submit_job(job)
+            hub_client.submit_job(job)
             jobs.append(job)
         if tag_name:
-            backend.add_tag_from_run(repo_data, tag_name, self.run_name, jobs)
+            hub_client.add_tag_from_run(tag_name, self.run_name, jobs)
         return jobs
 
-    def _dep_specs(self, backend: Backend) -> Optional[List[DepSpec]]:
+    def _dep_specs(self, hub_client: "hub.HubClient") -> Optional[List[DepSpec]]:
         if self.provider_data.get("deps"):
-            repo_data = load_repo_data()
-            return [
-                self._parse_dep_spec(dep, backend, repo_data) for dep in self.provider_data["deps"]
-            ]
+            return [self._parse_dep_spec(dep, hub_client) for dep in self.provider_data["deps"]]
         else:
             return None
 
     def _validate_local_path(self, path: str) -> str:
         if path == "~" or path.startswith("~/"):
             if not self.home_dir:
                 raise KeyError("home_dir is not defined, local path can't start with ~")
@@ -298,63 +313,55 @@
             if isinstance(item, str):
                 item = {"path": item}
             item["path"] = self._validate_local_path(item["path"])
             cache_specs.append(CacheSpec(**item))
         return cache_specs
 
     @staticmethod
-    def _parse_dep_spec(dep: Union[dict, str], backend: Backend, repo_data: RepoData) -> DepSpec:
+    def _parse_dep_spec(dep: Union[dict, str], hub_client) -> DepSpec:
         if isinstance(dep, str):
             mount = False
             if dep.startswith(":"):
                 tag_dep = True
                 dep = dep[1:]
             else:
                 tag_dep = False
         else:
             mount = dep.get("mount") is True
             tag_dep = dep.get("tag") is not None
             dep = dep.get("tag") or dep.get("workflow")
         t = dep.split("/")
         if len(t) == 1:
             if tag_dep:
-                return Provider._tag_dep(backend, repo_data, t[0], mount)
+                return Provider._tag_dep(hub_client, t[0], mount)
             else:
-                return Provider._workflow_dep(backend, repo_data, t[0], mount)
+                return Provider._workflow_dep(hub_client, t[0], mount)
         elif len(t) == 3:
             # This doesn't allow to refer to projects from other repos
-            repo_address = RepoAddress(
-                repo_host_name=repo_data.repo_host_name,
-                repo_port=repo_data.repo_port,
-                repo_user_name=t[0],
-                repo_name=t[1],
-            )
             if tag_dep:
-                return Provider._tag_dep(backend, repo_address, t[2], mount)
+                return Provider._tag_dep(hub_client, t[2], mount)
             else:
-                return Provider._workflow_dep(backend, repo_address, t[2], mount)
+                return Provider._workflow_dep(hub_client, t[2], mount)
         else:
             sys.exit(f"Invalid dep format: {dep}")
 
     @staticmethod
-    def _tag_dep(
-        backend: Backend, repo_address: RepoAddress, tag_name: str, mount: bool
-    ) -> DepSpec:
-        tag_head = backend.get_tag_head(repo_address, tag_name)
+    def _tag_dep(hub_client: "hub.HubClient", tag_name: str, mount: bool) -> DepSpec:
+        tag_head = hub_client.get_tag_head(tag_name)
         if tag_head:
-            return DepSpec(repo_address=repo_address, run_name=tag_head.run_name, mount=mount)
+            return DepSpec(
+                repo_ref=hub_client.repo.repo_ref, run_name=tag_head.run_name, mount=mount
+            )
         else:
-            sys.exit(f"Cannot find the tag '{tag_name}' in the '{repo_address.path()}' repo")
+            sys.exit(f"Cannot find the tag '{tag_name}' in the '{hub_client.repo.repo_id}' repo")
 
     @staticmethod
-    def _workflow_dep(
-        backend: Backend, repo_address: RepoAddress, workflow_name: str, mount: bool
-    ) -> DepSpec:
+    def _workflow_dep(hub_client: "hub.HubClient", workflow_name: str, mount: bool) -> DepSpec:
         job_heads = sorted(
-            backend.list_job_heads(repo_address),
+            hub_client.list_job_heads(),
             key=lambda j: j.submitted_at,
             reverse=True,
         )
         run_name = next(
             iter(
                 [
                     job_head.run_name
@@ -362,19 +369,19 @@
                     if job_head.workflow_name == workflow_name
                     and job_head.status == JobStatus.DONE
                 ]
             ),
             None,
         )
         if run_name:
-            return DepSpec(repo_address=repo_address, run_name=run_name, mount=mount)
+            return DepSpec(repo_ref=hub_client.repo.repo_ref, run_name=run_name, mount=mount)
         else:
             sys.exit(
                 f"Cannot find any successful workflow with the name '{workflow_name}' "
-                f"in the '{repo_address.path()}' repo"
+                f"in the '{hub_client.repo.repo_id}' repo"
             )
 
     def _env(self) -> Optional[Dict[str, str]]:
         if self.provider_data.get("env"):
             env = {}
             for e in self.provider_data.get("env"):
                 if "=" in e:
```

### Comparing `dstack-0.7rc1/cli/dstack/providers/_torchrun/main.py` & `dstack-0.8/cli/dstack/providers/_torchrun/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
 from dstack.backend.base import Backend
 from dstack.core.job import GpusRequirements, JobSpec, Requirements
 from dstack.providers import Provider
@@ -21,20 +21,21 @@
         self.nodes = None
         self.resources = None
         self.args = None
 
     def load(
         self,
         backend: Backend,
-        provider_args: List[str],
+        args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
+        ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, provider_args, workflow_name, provider_data, run_name)
+        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.script = self.provider_data.get("script") or self.provider_data.get("file")
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.python = self._safe_python_version("python")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.nodes = self.provider_data.get("nodes") or 1
```

### Comparing `dstack-0.7rc1/cli/dstack/providers/bash/main.py` & `dstack-0.8/cli/dstack/providers/bash/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
 from dstack import version
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
@@ -23,20 +23,21 @@
         self.commands = None
         self.image_name = None
         self.home_dir = "/root"
 
     def load(
         self,
         backend: Backend,
-        provider_args: List[str],
+        args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
+        ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, provider_args, workflow_name, provider_data, run_name)
+        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.python = self._safe_python_version("python")
         self.commands = self._get_list_data("commands")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.ports = self.provider_data.get("ports")
         self.resources = self._resources()
```

### Comparing `dstack-0.7rc1/cli/dstack/providers/code/main.py` & `dstack-0.8/cli/dstack/providers/code/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import uuid
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
 from dstack import version
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
@@ -11,34 +11,37 @@
 from dstack.providers import Provider
 
 
 class CodeProvider(Provider):
     def __init__(self):
         super().__init__("code")
         self.setup = None
+        self.ports = None
         self.python = None
         self.version = None
         self.requirements = None
         self.env = None
         self.artifact_specs = None
         self.working_dir = None
         self.resources = None
         self.image_name = None
         self.home_dir = "/root"
 
     def load(
         self,
         backend: Backend,
-        provider_args: List[str],
+        args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
+        ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, provider_args, workflow_name, provider_data, run_name)
+        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
+        self.ports = self.provider_data.get("ports")
         self.python = self._safe_python_version("python")
         self.version = self.provider_data.get("version") or "1.74.3"
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
         self.image_name = self._image_name()
@@ -46,36 +49,46 @@
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
         parser = ArgumentParser(
             prog="dstack run " + (workflow_name or self.provider_name),
             formatter_class=RichHelpFormatter,
         )
         self._add_base_args(parser)
         parser.add_argument("--ssh", action="store_true", dest="openssh_server")
+        parser.add_argument("-p", "--ports", metavar="PORT_COUNT", type=int)
         return parser
 
     def parse_args(self):
         parser = self._create_parser(self.workflow_name)
         args, unknown_args = parser.parse_known_args(self.provider_args)
         self._parse_base_args(args, unknown_args)
         if args.openssh_server:
             self.openssh_server = True
+        if args.ports:
+            self.provider_data["ports"] = args.ports
 
     def create_job_specs(self) -> List[JobSpec]:
         env = {}
         connection_token = uuid.uuid4().hex
         env["CONNECTION_TOKEN"] = connection_token
         apps = [
             AppSpec(
                 port_index=0,
                 app_name="code",
                 url_query_params={
                     "tkn": connection_token,
                 },
             )
         ]
+        for i in range(self.ports or 0):
+            apps.append(
+                AppSpec(
+                    port_index=i + 1,
+                    app_name="code" + (str(i + 1)),
+                )
+            )
         if self.openssh_server:
             apps.append(AppSpec(port_index=len(apps), app_name="openssh-server"))
         return [
             JobSpec(
                 image_name=self.image_name,
                 commands=self._commands(),
                 entrypoint=["/bin/bash", "-i", "-c"],
@@ -96,14 +109,21 @@
 
     def _commands(self):
         commands = []
         if self.env:
             self._extend_commands_with_env(commands, self.env)
         if self.openssh_server:
             self._extend_commands_with_openssh_server(commands, self.ssh_key_pub, 1)
+        commands.append("export _PORT=$PORT_0")
+        if self.ports:
+            for i in range(self.ports):
+                commands.append(f"export PORT_{i}=$PORT_{i + 1}")
+                commands.append(f"echo 'export PORT_{i}=\"$PORT_{i + 1}\"' >> ~/.bashrc")
+                commands.append(f'echo "The PORT_{i} port is mapped to http://0.0.0.0:$PORT_{i}"')
+            commands.append("echo")
         commands.extend(
             [
                 "pip install ipykernel -q",
                 "mkdir -p /tmp",
                 'if [ $(uname -m) = "aarch64" ]; then arch="arm64"; else arch="x64"; fi',
                 f"wget -q https://github.com/gitpod-io/openvscode-server/releases/download/"
                 f"openvscode-server-v{self.version}/openvscode-server-v{self.version}-linux-$arch.tar.gz -O "
@@ -112,14 +132,14 @@
                 f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --install-extension ms-python.python",
                 "rm /usr/bin/python2*",
             ]
         )
         if self.setup:
             commands.extend(self.setup)
         commands.append(
-            f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --port $PORT_0 --host 0.0.0.0 --connection-token $CONNECTION_TOKEN --default-folder /workflow"
+            f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --port $_PORT --host 0.0.0.0 --connection-token $CONNECTION_TOKEN --default-folder /workflow"
         )
         return commands
 
 
 def __provider__():
     return CodeProvider()
```

### Comparing `dstack-0.7rc1/cli/dstack/providers/docker/main.py` & `dstack-0.8/cli/dstack/providers/docker/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
 from dstack.core.job import JobSpec
@@ -21,20 +21,21 @@
         self.working_dir = None
         self.ports = None
         self.resources = None
 
     def load(
         self,
         backend: Backend,
-        provider_args: List[str],
+        args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
+        ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, provider_args, workflow_name, provider_data, run_name)
+        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.image_name = self.provider_data["image"]
         self.registry_auth = self.provider_data.get("registry_auth")
         self.commands = self._get_list_data("commands")
         self.entrypoint = self._get_entrypoint()
         if self.commands and self.entrypoint is None:  # commands not empty
             self.entrypoint = ["/bin/sh", "-i", "-c"]
         self.artifact_specs = self._artifact_specs()
```

### Comparing `dstack-0.7rc1/cli/dstack/providers/lab/main.py` & `dstack-0.8/cli/dstack/providers/lab/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import uuid
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
 from dstack import version
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
@@ -23,20 +23,21 @@
         self.resources = None
         self.image_name = None
         self.home_dir = "/root"
 
     def load(
         self,
         backend: Backend,
-        provider_args: List[str],
+        args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
+        ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, provider_args, workflow_name, provider_data, run_name)
+        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.python = self._safe_python_version("python")
         self.version = self.provider_data.get("version")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
```

### Comparing `dstack-0.7rc1/cli/dstack/providers/notebook/main.py` & `dstack-0.8/cli/dstack/providers/notebook/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import uuid
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional
 
 from rich_argparse import RichHelpFormatter
 
 from dstack import version
 from dstack.backend.base import Backend
 from dstack.core.app import AppSpec
@@ -23,20 +23,21 @@
         self.resources = None
         self.image_name = None
         self.home_dir = "/root"
 
     def load(
         self,
         backend: Backend,
-        provider_args: List[str],
+        args: Optional[Namespace],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
+        ssh_key_pub: Optional[str] = None,
     ):
-        super().load(backend, provider_args, workflow_name, provider_data, run_name)
+        super().load(backend, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.python = self._safe_python_version("python")
         self.version = self.provider_data.get("version")
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
```

### Comparing `dstack-0.7rc1/cli/dstack/utils/interpolator.py` & `dstack-0.8/cli/dstack/utils/interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack/utils/random_names.py` & `dstack-0.8/cli/dstack/utils/random_names.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/dstack.egg-info/SOURCES.txt` & `dstack-0.8/cli/dstack.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,35 +6,39 @@
 cli/dstack.egg-info/PKG-INFO
 cli/dstack.egg-info/SOURCES.txt
 cli/dstack.egg-info/dependency_links.txt
 cli/dstack.egg-info/entry_points.txt
 cli/dstack.egg-info/requires.txt
 cli/dstack.egg-info/top_level.txt
 cli/dstack/api/__init__.py
-cli/dstack/api/artifacts.py
-cli/dstack/api/backend.py
-cli/dstack/api/config.py
-cli/dstack/api/logs.py
-cli/dstack/api/repo.py
-cli/dstack/api/run.py
-cli/dstack/api/tags.py
+cli/dstack/api/repos.py
+cli/dstack/api/runs.py
+cli/dstack/api/hub/__init__.py
+cli/dstack/api/hub/_api_client.py
+cli/dstack/api/hub/_client.py
+cli/dstack/api/hub/_config.py
+cli/dstack/api/hub/_storage.py
+cli/dstack/api/hub/errors.py
+cli/dstack/api/internal/__init__.py
+cli/dstack/api/internal/backend.py
 cli/dstack/backend/__init__.py
 cli/dstack/backend/aws/__init__.py
 cli/dstack/backend/aws/compute.py
 cli/dstack/backend/aws/config.py
 cli/dstack/backend/aws/logs.py
 cli/dstack/backend/aws/repos.py
 cli/dstack/backend/aws/runners.py
 cli/dstack/backend/aws/secrets.py
 cli/dstack/backend/aws/storage.py
 cli/dstack/backend/aws/utils.py
 cli/dstack/backend/base/__init__.py
 cli/dstack/backend/base/artifacts.py
 cli/dstack/backend/base/cache.py
 cli/dstack/backend/base/compute.py
+cli/dstack/backend/base/config.py
 cli/dstack/backend/base/jobs.py
 cli/dstack/backend/base/logs.py
 cli/dstack/backend/base/repos.py
 cli/dstack/backend/base/runners.py
 cli/dstack/backend/base/runs.py
 cli/dstack/backend/base/secrets.py
 cli/dstack/backend/base/storage.py
@@ -42,67 +46,66 @@
 cli/dstack/backend/gcp/__init__.py
 cli/dstack/backend/gcp/compute.py
 cli/dstack/backend/gcp/config.py
 cli/dstack/backend/gcp/logs.py
 cli/dstack/backend/gcp/secrets.py
 cli/dstack/backend/gcp/storage.py
 cli/dstack/backend/gcp/utils.py
-cli/dstack/backend/hub/__init__.py
-cli/dstack/backend/hub/client.py
-cli/dstack/backend/hub/config.py
-cli/dstack/backend/hub/storage.py
 cli/dstack/backend/local/__init__.py
 cli/dstack/backend/local/artifacts.py
 cli/dstack/backend/local/compute.py
 cli/dstack/backend/local/config.py
 cli/dstack/backend/local/logs.py
 cli/dstack/backend/local/runners.py
 cli/dstack/backend/local/secrets.py
 cli/dstack/backend/local/storage.py
 cli/dstack/cli/__init__.py
 cli/dstack/cli/common.py
 cli/dstack/cli/config.py
+cli/dstack/cli/errors.py
 cli/dstack/cli/handlers.py
 cli/dstack/cli/main.py
 cli/dstack/cli/updates.py
 cli/dstack/cli/commands/__init__.py
 cli/dstack/cli/commands/config/__init__.py
 cli/dstack/cli/commands/cp/__init__.py
-cli/dstack/cli/commands/hub/__init__.py
 cli/dstack/cli/commands/init/__init__.py
 cli/dstack/cli/commands/logs/__init__.py
 cli/dstack/cli/commands/ls/__init__.py
 cli/dstack/cli/commands/prune/__init__.py
 cli/dstack/cli/commands/ps/__init__.py
-cli/dstack/cli/commands/pull/__init__.py
-cli/dstack/cli/commands/push/__init__.py
 cli/dstack/cli/commands/rm/__init__.py
 cli/dstack/cli/commands/run/__init__.py
 cli/dstack/cli/commands/run/ssh_tunnel.py
 cli/dstack/cli/commands/secrets/__init__.py
+cli/dstack/cli/commands/start/__init__.py
 cli/dstack/cli/commands/stop/__init__.py
 cli/dstack/cli/commands/tags/__init__.py
 cli/dstack/core/__init__.py
 cli/dstack/core/app.py
 cli/dstack/core/artifact.py
 cli/dstack/core/cache.py
-cli/dstack/core/config.py
 cli/dstack/core/dependents.py
 cli/dstack/core/error.py
 cli/dstack/core/instance.py
 cli/dstack/core/job.py
 cli/dstack/core/log_event.py
-cli/dstack/core/repo.py
 cli/dstack/core/request.py
 cli/dstack/core/run.py
 cli/dstack/core/runners.py
 cli/dstack/core/secret.py
 cli/dstack/core/storage.py
 cli/dstack/core/tag.py
 cli/dstack/core/userconfig.py
+cli/dstack/core/repo/__init__.py
+cli/dstack/core/repo/base.py
+cli/dstack/core/repo/head.py
+cli/dstack/core/repo/local.py
+cli/dstack/core/repo/remote.py
+cli/dstack/core/repo/spec.py
 cli/dstack/hub/__init__.py
 cli/dstack/hub/main.py
 cli/dstack/hub/background/__init__.py
 cli/dstack/hub/background/tasks/__init__.py
 cli/dstack/hub/background/tasks/resubmit_jobs.py
 cli/dstack/hub/db/__init__.py
 cli/dstack/hub/db/migrate.py
@@ -113,30 +116,40 @@
 cli/dstack/hub/migration/versions/__init__.py
 cli/dstack/hub/models/__init__.py
 cli/dstack/hub/repository/__init__.py
 cli/dstack/hub/repository/projects.py
 cli/dstack/hub/repository/users.py
 cli/dstack/hub/routers/__init__.py
 cli/dstack/hub/routers/artifacts.py
+cli/dstack/hub/routers/backends.py
 cli/dstack/hub/routers/cache.py
 cli/dstack/hub/routers/jobs.py
 cli/dstack/hub/routers/link.py
 cli/dstack/hub/routers/logs.py
 cli/dstack/hub/routers/projects.py
 cli/dstack/hub/routers/repos.py
 cli/dstack/hub/routers/runners.py
 cli/dstack/hub/routers/runs.py
 cli/dstack/hub/routers/secrets.py
+cli/dstack/hub/routers/storage.py
 cli/dstack/hub/routers/tags.py
 cli/dstack/hub/routers/users.py
 cli/dstack/hub/routers/util.py
 cli/dstack/hub/routers/workflows.py
 cli/dstack/hub/security/__init__.py
 cli/dstack/hub/security/permissions.py
 cli/dstack/hub/security/utils.py
+cli/dstack/hub/services/__init__.py
+cli/dstack/hub/services/backends/__init__.py
+cli/dstack/hub/services/backends/aws.py
+cli/dstack/hub/services/backends/base.py
+cli/dstack/hub/services/backends/gcp.py
+cli/dstack/hub/services/backends/local.py
+cli/dstack/hub/utils/__init__.py
+cli/dstack/hub/utils/logging.py
 cli/dstack/providers/__init__.py
 cli/dstack/providers/_torchrun/__init__.py
 cli/dstack/providers/_torchrun/main.py
 cli/dstack/providers/bash/__init__.py
 cli/dstack/providers/bash/main.py
 cli/dstack/providers/code/__init__.py
 cli/dstack/providers/code/main.py
@@ -145,26 +158,37 @@
 cli/dstack/providers/lab/__init__.py
 cli/dstack/providers/lab/main.py
 cli/dstack/providers/notebook/__init__.py
 cli/dstack/providers/notebook/main.py
 cli/dstack/schemas/__init__.py
 cli/dstack/utils/__init__.py
 cli/dstack/utils/common.py
+cli/dstack/utils/escape.py
+cli/dstack/utils/hash.py
 cli/dstack/utils/interpolator.py
 cli/dstack/utils/random_names.py
+cli/dstack/utils/ssh.py
+cli/dstack/utils/workflows.py
 cli/tests/__init__.py
 cli/tests/backend/__init__.py
 cli/tests/backend/base/__init__.py
 cli/tests/backend/base/test_logs.py
 cli/tests/hub/__init__.py
 cli/tests/hub/common.py
 cli/tests/hub/conftest.py
 cli/tests/hub/routers/__init__.py
 cli/tests/hub/routers/test_jobs.py
 cli/tests/hub/routers/test_projects.py
 cli/tests/hub/routers/test_users.py
+cli/tests/integration/__init__.py
+cli/tests/integration/common.py
+cli/tests/integration/conftest.py
+cli/tests/integration/test_commands.py
 cli/tests/providers/__init__.py
 cli/tests/providers/test_local_path.py
 cli/tests/providers/docker/__init__.py
 cli/tests/providers/docker/test_entrypoint.py
 cli/tests/utils/__init__.py
-cli/tests/utils/test_interpolator.py
+cli/tests/utils/escape.py
+cli/tests/utils/test_interpolator.py
+cli/tests/utils/test_merge_workflow_data.py
+cli/tests/utils/test_tarignore.py
```

### Comparing `dstack-0.7rc1/cli/tests/backend/base/test_logs.py` & `dstack-0.8/cli/tests/backend/base/test_logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/tests/hub/common.py` & `dstack-0.8/cli/tests/hub/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/tests/hub/routers/test_jobs.py` & `dstack-0.8/cli/tests/hub/routers/test_jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/tests/hub/routers/test_projects.py` & `dstack-0.8/cli/tests/hub/routers/test_projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/tests/hub/routers/test_users.py` & `dstack-0.8/cli/tests/hub/routers/test_users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/tests/providers/docker/test_entrypoint.py` & `dstack-0.8/cli/tests/providers/docker/test_entrypoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,78 @@
 import unittest
+from argparse import Namespace
 from typing import List, Optional
-from unittest.mock import patch
+from unittest import mock
 
-from dstack.backend.base import Backend
-from dstack.core.repo import LocalRepoData
+from dstack.core.repo import RemoteRepo
 from dstack.providers.docker.main import DockerProvider
 
 
-def load_repo_data():
-    return LocalRepoData(
-        repo_host_name="",
-        repo_user_name="",
-        repo_name="",
-        repo_branch="",
-        repo_hash="",
-        protocol="https",
-    )
-
-
 def create_provider_data(
     commands: Optional[List[str]] = None, entrypoint: Optional[str] = None
 ) -> dict:
     return {"image": "ubuntu:20.04", "commands": commands, "entrypoint": entrypoint}
 
 
-@patch("dstack.providers.load_repo_data", new=load_repo_data)
+args = Namespace(args=[], unknown=[], detach=True)
+
+
 class TestEntrypoint(unittest.TestCase):
-    @patch.multiple(Backend, __abstractmethods__=set())
     def setUp(self) -> None:
-        self.backend = Backend()
+        self.hub_client = mock.Mock()
+        self.hub_client.configure_mock(
+            repo=RemoteRepo(repo_url="https://github.com/dstackai/dstack-playground.git")
+        )
 
     def test_no_commands(self):
         provider = DockerProvider()
-        provider.load(self.backend, [], "dummy-workflow", create_provider_data(), "dummy-run-1")
-        for job in provider.submit_jobs(self.backend, ""):
+        provider.load(
+            self.hub_client, args, "dummy-workflow", create_provider_data(), "dummy-run-1"
+        )
+        for job in provider.submit_jobs(self.hub_client, ""):
             data = job.serialize()
             self.assertListEqual(data["commands"], [])
             self.assertEqual(data["entrypoint"], None)
 
     def test_no_entrypoint(self):
         commands = ["echo 123", "whoami"]
         provider = DockerProvider()
         provider.load(
-            self.backend,
-            [],
+            self.hub_client,
+            args,
             "dummy-workflow",
             create_provider_data(commands=commands),
             "dummy-run-1",
         )
-        for job in provider.submit_jobs(self.backend, ""):
+        for job in provider.submit_jobs(self.hub_client, ""):
             data = job.serialize()
             self.assertListEqual(data["commands"], commands)
             self.assertListEqual(data["entrypoint"], ["/bin/sh", "-i", "-c"])
 
     def test_only_entrypoint(self):
         provider = DockerProvider()
         provider.load(
-            self.backend,
-            [],
+            self.hub_client,
+            args,
             "dummy-workflow",
             create_provider_data(entrypoint="/bin/bash -ic"),
             "dummy-run-1",
         )
-        for job in provider.submit_jobs(self.backend, ""):
+        for job in provider.submit_jobs(self.hub_client, ""):
             data = job.serialize()
             self.assertListEqual(data["commands"], [])
             self.assertListEqual(data["entrypoint"], ["/bin/bash", "-ic"])
 
     def test_entrypoint_override(self):
         commands = ["echo 123", "whoami"]
         provider = DockerProvider()
         provider.load(
-            self.backend,
-            [],
+            self.hub_client,
+            args,
             "dummy-workflow",
             create_provider_data(commands=commands, entrypoint="/bin/bash -ic"),
             "dummy-run-1",
         )
-        for job in provider.submit_jobs(self.backend, ""):
+        for job in provider.submit_jobs(self.hub_client, ""):
             data = job.serialize()
             self.assertListEqual(data["commands"], commands)
             self.assertListEqual(data["entrypoint"], ["/bin/bash", "-ic"])
```

### Comparing `dstack-0.7rc1/cli/tests/providers/test_local_path.py` & `dstack-0.8/cli/tests/providers/test_local_path.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/cli/tests/utils/test_interpolator.py` & `dstack-0.8/cli/tests/utils/test_interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7rc1/setup.py` & `dstack-0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     entry_points={
         "console_scripts": ["dstack=dstack.cli.main:main"],
     },
     url="https://dstack.ai",
     project_urls={
         "Source": "https://github.com/dstackai/dstack",
     },
-    description="The hassle-free tool for managing ML workflows on any cloud platform.",
+    description="The easiest way to define ML workflows and run them on any cloud platform",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     python_requires=">=3.7",
     install_requires=[
         "pyyaml",
         "requests",
         "gitpython",
@@ -65,15 +65,15 @@
         "botocore",
         "python-dateutil",
         "paramiko",
         "git-url-parse",
         "rich",
         "rich-argparse",
         "fastapi",
-        "starlette",
+        "starlette>=0.26.0",
         "uvicorn",
         "pydantic",
         "sqlalchemy[asyncio]>=2.0.0",
         "websocket-client",
         "cursor",
         "simple-term-menu",
         "py-cpuinfo",
@@ -86,14 +86,16 @@
         "google-cloud-compute>=1.5.0",
         "google-cloud-secret-manager>=2.0.0",
         "google-cloud-logging>=2.0.0",
         "aiosqlite",
         "apscheduler",
         "alembic>=1.10.2",
         "typing-extensions>=4.0.0",
+        "file-read-backwards>=3.0.0",
+        "psutil>=5.0.0",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Programming Language :: Python :: 3",
     ],
```

