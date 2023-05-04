# Comparing `tmp/autumn8-1.0.3rc1.tar.gz` & `tmp/autumn8-1.0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.3rc1.tar", last modified: Thu May  4 13:35:46 2023, max compression
+gzip compressed data, was "autumn8-1.0.3rc2.tar", last modified: Thu May  4 15:15:22 2023, max compression
```

## Comparing `autumn8-1.0.3rc1.tar` & `autumn8-1.0.3rc2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.212260 autumn8-1.0.3rc1/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-04 13:24:26.000000 autumn8-1.0.3rc1/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-17 13:57:37.000000 autumn8-1.0.3rc1/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4910 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16112 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2866 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-04 13:24:26.000000 autumn8-1.0.3rc1/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-04 13:35:26.000000 autumn8-1.0.3rc1/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.3rc1/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.3rc1/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.3rc1/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.3rc1/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.3rc1/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.3rc1/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11865 2023-05-04 13:26:09.000000 autumn8-1.0.3rc1/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.3rc1/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.3rc1/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-04 13:24:26.000000 autumn8-1.0.3rc1/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.212260 autumn8-1.0.3rc1/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1412 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      132 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.643581 autumn8-1.0.3rc2/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 15:15:22.643581 autumn8-1.0.3rc2/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.613580 autumn8-1.0.3rc2/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-04 13:24:26.000000 autumn8-1.0.3rc2/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-17 13:57:37.000000 autumn8-1.0.3rc2/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4910 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16112 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2866 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-04 13:24:26.000000 autumn8-1.0.3rc2/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-04 15:13:05.000000 autumn8-1.0.3rc2/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.633580 autumn8-1.0.3rc2/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.3rc2/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.3rc2/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.3rc2/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.3rc2/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.3rc2/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.633580 autumn8-1.0.3rc2/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.633580 autumn8-1.0.3rc2/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.3rc2/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.633580 autumn8-1.0.3rc2/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11865 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.3rc2/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.3rc2/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-04 13:24:26.000000 autumn8-1.0.3rc2/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1412 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1959 2023-05-04 15:12:12.000000 autumn8-1.0.3rc2/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-04 15:15:22.643581 autumn8-1.0.3rc2/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.643581 autumn8-1.0.3rc2/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/tests/test_settings.py
```

### Comparing `autumn8-1.0.3rc1/PKG-INFO` & `autumn8-1.0.3rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.3rc1
+Version: 1.0.3rc2
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.3rc1/README.md` & `autumn8-1.0.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/analyze.py` & `autumn8-1.0.3rc2/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/cli_environment.py` & `autumn8-1.0.3rc2/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/commands/cloud.py` & `autumn8-1.0.3rc2/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/commands/models.py` & `autumn8-1.0.3rc2/autumn8/cli/commands/models.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/examples.py` & `autumn8-1.0.3rc2/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/interactive.py` & `autumn8-1.0.3rc2/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/main.py` & `autumn8-1.0.3rc2/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/options.py` & `autumn8-1.0.3rc2/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/pending_uploads.py` & `autumn8-1.0.3rc2/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/cli/validation.py` & `autumn8-1.0.3rc2/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/common/config/cloud_info.py` & `autumn8-1.0.3rc2/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/common/config/settings.py` & `autumn8-1.0.3rc2/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/common/config/supported_instances.py` & `autumn8-1.0.3rc2/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/common/types.py` & `autumn8-1.0.3rc2/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/env/__init__.py` & `autumn8-1.0.3rc2/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/examples/mnist.py` & `autumn8-1.0.3rc2/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/examples/model.py` & `autumn8-1.0.3rc2/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.3rc2/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.3rc2/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/__init__.py` & `autumn8-1.0.3rc2/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/api/cloud.py` & `autumn8-1.0.3rc2/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/api/lab.py` & `autumn8-1.0.3rc2/autumn8/lib/api/lab.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/api_creds.py` & `autumn8-1.0.3rc2/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/asyncio.py` & `autumn8-1.0.3rc2/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/http.py` & `autumn8-1.0.3rc2/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/logging.py` & `autumn8-1.0.3rc2/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/logging.yaml` & `autumn8-1.0.3rc2/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/package_resolver.py` & `autumn8-1.0.3rc2/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8/lib/service.py` & `autumn8-1.0.3rc2/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.3rc2/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.3rc1
+Version: 1.0.3rc2
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.3rc1/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.3rc2/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/pyproject.toml` & `autumn8-1.0.3rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "questionary>=1.10.0",
   "tqdm",
   "fastapi", # used for supporting one app 503 exception while cloudinfo is down - TODO remove
   "pyyaml",
   "jsonschema",
   "requests",
   "httpx",
-  "boto3-stubs[s3]",
+  "boto3-stubs[s3,sts]",
 ]
 # package_data={"autumn8.lib": ["logging.yaml"]},
 description = "Utilities to export models to the autumn8.ai service"
 readme = "README.md"
 dynamic = ["version"]
 
 # long_description=readme_content,
```

### Comparing `autumn8-1.0.3rc1/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.3rc2/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc1/tests/test_settings.py` & `autumn8-1.0.3rc2/tests/test_settings.py`

 * *Files identical despite different names*

