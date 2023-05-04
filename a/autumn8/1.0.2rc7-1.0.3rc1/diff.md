# Comparing `tmp/autumn8-1.0.2rc7.tar.gz` & `tmp/autumn8-1.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.2rc7.tar", last modified: Thu May  4 12:52:29 2023, max compression
+gzip compressed data, was "autumn8-1.0.3rc1.tar", last modified: Thu May  4 13:35:46 2023, max compression
```

## Comparing `autumn8-1.0.2rc7.tar` & `autumn8-1.0.3rc1.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.362130 autumn8-1.0.2rc7/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.362130 autumn8-1.0.2rc7/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7850 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-17 13:57:37.000000 autumn8-1.0.2rc7/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.362130 autumn8-1.0.2rc7/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4910 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16112 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2866 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-28 11:52:10.000000 autumn8-1.0.2rc7/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-04 12:52:03.000000 autumn8-1.0.2rc7/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3117 2023-05-04 12:50:51.000000 autumn8-1.0.2rc7/autumn8/common/config/s3.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.2rc7/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.2rc7/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.2rc7/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.2rc7/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.2rc7/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.2rc7/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10319 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.2rc7/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.2rc7/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4578 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.362130 autumn8-1.0.2rc7/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1440 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      132 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.212260 autumn8-1.0.3rc1/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-04 13:24:26.000000 autumn8-1.0.3rc1/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-17 13:57:37.000000 autumn8-1.0.3rc1/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4910 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16112 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2866 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-04 13:24:26.000000 autumn8-1.0.3rc1/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-04 13:35:26.000000 autumn8-1.0.3rc1/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.3rc1/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.3rc1/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.3rc1/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.3rc1/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.3rc1/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.222260 autumn8-1.0.3rc1/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.3rc1/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11865 2023-05-04 13:26:09.000000 autumn8-1.0.3rc1/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.3rc1/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-03 14:35:59.000000 autumn8-1.0.3rc1/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.3rc1/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.3rc1/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-04 13:24:26.000000 autumn8-1.0.3rc1/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.212260 autumn8-1.0.3rc1/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1412 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      132 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-04 13:35:46.000000 autumn8-1.0.3rc1/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-01 12:46:21.000000 autumn8-1.0.3rc1/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 13:35:46.232260 autumn8-1.0.3rc1/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.3rc1/tests/test_settings.py
```

### Comparing `autumn8-1.0.2rc7/PKG-INFO` & `autumn8-1.0.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.2rc7
+Version: 1.0.3rc1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.2rc7/README.md` & `autumn8-1.0.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/cli/analyze.py` & `autumn8-1.0.3rc1/autumn8/cli/analyze.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import importlib
 import os
 import sys
-from pathlib import Path
+from pathlib import Path, PurePosixPath
 
 from click import ClickException
 
 import autumn8
 from autumn8.lib import logging
 
 sys.path.append(os.getcwd())
@@ -150,16 +150,20 @@
     return dummy_input, model_file_name, framework
 
 
 def suggest_model_name(model_file_path: str):
     return Path(model_file_path).stem
 
 
-def filepath_is_a_link(filepath: str) -> bool:
-    return filepath.startswith("http://") or filepath.startswith("https://")
+def is_model_file_link_external(link: str) -> bool:
+    return (
+        link.startswith("http://")
+        or link.startswith("https://")
+        or link.startswith("s3://")
+    )
 
 
 def analyze_model_file(model_filepath_or_url: str, model_script_args=[]):
     extension = Path(model_filepath_or_url).suffixes[-1]
     is_source_annotated_model = False
 
     (
@@ -170,15 +174,15 @@
     _inferred_batch_size = None
     inferred_input_dims = []
 
     inferred_model_name = suggest_model_name(model_filepath_or_url)
     inferred_quantization = "FP32"
 
     if extension in [".py"]:
-        if filepath_is_a_link(model_filepath_or_url):
+        if is_model_file_link_external(model_filepath_or_url):
             raise ClickException(
                 "Hosted .py files are not supported yet - please download the script and run the CLI on it"
             )
         is_source_annotated_model = True
         dummy_input, model_file_name, framework = pack_annotated_script_model(
             model_filepath_or_url, model_script_args, inferred_model_name
         )
@@ -223,7 +227,11 @@
         model_filepath_or_url,
         inferred_model_name,
         framework,
         inferred_quantization,
         inferred_input_dims,
         is_source_annotated_model,
     )
+
+
+def s3path_join(*args: str):
+    return str(PurePosixPath(*args))
```

### Comparing `autumn8-1.0.2rc7/autumn8/cli/cli_environment.py` & `autumn8-1.0.3rc1/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/cli/commands/cloud.py` & `autumn8-1.0.3rc1/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/cli/commands/models.py` & `autumn8-1.0.3rc1/autumn8/cli/commands/models.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/cli/examples.py` & `autumn8-1.0.3rc1/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/cli/interactive.py` & `autumn8-1.0.3rc1/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/cli/main.py` & `autumn8-1.0.3rc1/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/cli/options.py` & `autumn8-1.0.3rc1/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/cli/pending_uploads.py` & `autumn8-1.0.3rc1/autumn8/cli/pending_uploads.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pickle
 from pathlib import Path
 
 import appdirs
 import click
 
 from autumn8.cli.cli_environment import CliEnvironment
-from autumn8.common.config.s3 import init_s3, init_s3_client
 
 APP_NAME = "autumn8"
 APP_AUTHOR = "autumn8"
 
 data_dir = appdirs.user_data_dir(APP_NAME, APP_AUTHOR)
 RESUMABLE_UPLOADS_PATH = os.path.join(data_dir, "uploads.pickle")
 
@@ -86,14 +85,15 @@
 
         return resume_args
 
     return None
 
 
 def get_mpu(environment: CliEnvironment, mpu_object_key: str, mpu_id: str):
+    raise NotImplementedError()
     s3 = init_s3(environment.value.s3_host)
 
     s3_bucket_name = environment.value.s3_bucket_name
 
     mpus = list(
         s3.Bucket(s3_bucket_name).multipart_uploads.filter(
             Prefix=mpu_object_key,
@@ -104,14 +104,17 @@
         if m.id == mpu_id:
             return m
 
     return None
 
 
 def abort_upload(environment: CliEnvironment, mpu_object_key: str, mpu_id: str):
+    # TODO: store permissions locally on the computer for resume, or re-request them for the same file somehow
+    # https://gitlab.com/Autumn8Inc/autodl/-/issues/192
+    raise NotImplementedError()
     mpu = get_mpu(environment, mpu_object_key, mpu_id)
     if mpu is None:
         click.echo(
             "The upload could not be found on S3. It may have already been aborted or completed."
         )
         return
```

### Comparing `autumn8-1.0.2rc7/autumn8/cli/validation.py` & `autumn8-1.0.3rc1/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/common/config/cloud_info.py` & `autumn8-1.0.3rc1/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/common/config/settings.py` & `autumn8-1.0.3rc1/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/common/config/supported_instances.py` & `autumn8-1.0.3rc1/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/common/types.py` & `autumn8-1.0.3rc1/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/env/__init__.py` & `autumn8-1.0.3rc1/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/examples/mnist.py` & `autumn8-1.0.3rc1/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/examples/model.py` & `autumn8-1.0.3rc1/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.3rc1/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.3rc1/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/lib/__init__.py` & `autumn8-1.0.3rc1/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/lib/api/cloud.py` & `autumn8-1.0.3rc1/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/lib/api/lab.py` & `autumn8-1.0.3rc1/autumn8/lib/api/lab.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import io
 import json
 from threading import Lock
 from typing import Any, Dict, List, Optional
 
 import appdirs
+from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
+
+import appdirs
+import boto3
+import httpx
 import requests
 from mypy_boto3_s3 import S3Client
 from mypy_boto3_s3.type_defs import PartTypeDef
+from mypy_boto3_sts.type_defs import CredentialsTypeDef
 from requests.auth import HTTPBasicAuth
 from tqdm.contrib.concurrent import thread_map
 
 from autumn8.cli import pending_uploads
-from autumn8.cli.analyze import filepath_is_a_link
+from autumn8.cli.analyze import is_model_file_link_external, s3path_join
 from autumn8.cli.cli_environment import CliEnvironment
-from autumn8.common.config.s3 import init_s3, init_s3_client, s3path_join
 from autumn8.lib import logging
 from autumn8.lib.api_creds import retrieve_api_creds
 from autumn8.lib.http import require_ok_response, url_with_params
 
 DEFAULT_MAX_UPLOAD_WORKERS = 4
 
 APP_NAME = "autumn8"
@@ -102,51 +107,110 @@
         auth=HTTPBasicAuth(*retrieve_api_creds()),
     )
 
     require_ok_response(response)
     return response.json()
 
 
+FileUploadFileType = Union[Literal["model"], Literal["input"]]
+
+
 def normal_or_multipart_upload(
-    environment,
-    s3_file_url,
-    f,
+    organization_id: int,
+    environment: CliEnvironment,
+    file: io.BufferedReader,
+    file_name: str,
+    file_type: FileUploadFileType,
     resume_args,
     id_key,
     mpu_id=None,
     max_upload_workers=DEFAULT_MAX_UPLOAD_WORKERS,
 ):
-    f.seek(0, 2)  # seek to end of file
-    total_bytes = f.tell()
-    f.seek(0)
+    file.seek(0, 2)  # seek to end of file
+    total_bytes = file.tell()
+    file.seek(0)
+
+    permissions = request_temporary_model_file_upload_permissions(
+        environment, organization_id, file_name, file_type
+    )
+
     # AWS dissallow multipart upload of files under 5MB
     if total_bytes < 6 * 1024**2:
-        normal_upload(environment, s3_file_url, f)
+        return normal_upload(environment, permissions, file)
     else:
-        multipart_upload(
+        return multipart_upload(
             environment=environment,
-            s3_file_url=s3_file_url,
-            file=f,
+            permissions=permissions,
+            file=file,
             resume_args=resume_args,
             id_key=id_key,
             mpu_id=mpu_id,
             max_upload_workers=max_upload_workers,
         )
 
 
-def normal_upload(environment: CliEnvironment, s3_file_url: str, f):
-    S3 = init_s3(environment.value.s3_host)
+class FileUploadPermissionsResponse(TypedDict):
+    message: str
+    object_key: str
+    bucket_name: str
+    credentials: CredentialsTypeDef
+
+
+def request_temporary_model_file_upload_permissions(
+    environment: CliEnvironment,
+    organization_id: int,
+    file_name: str,
+    file_type: FileUploadFileType,
+):
+    autodl_host = environment.value.app_host
+    api_route = f"{autodl_host}/api/lab/model/upload_sts"
+    response = requests.get(
+        url_with_params(
+            api_route,
+            {
+                "organization_id": organization_id,
+                "file_name": file_name,
+                "file_type": file_type,
+            },
+        ),
+        headers={"Content-Type": "application/json"},
+        auth=HTTPBasicAuth(*retrieve_api_creds()),
+    )
+
+    require_ok_response(response)
+    return FileUploadPermissionsResponse(response.json())
+
 
-    compatible_s3_file_url = get_hacked_legacy_backwards_compatible_s3_file_url(
-        environment.value.s3_bucket_root_folder, s3_file_url
+def get_s3_client_from_temporary_permissions(
+    environment: CliEnvironment, permissions: FileUploadPermissionsResponse
+):
+    credentials = permissions["credentials"]
+    S3 = boto3.resource(
+        "s3",
+        endpoint_url=environment.value.s3_host,
+        aws_access_key_id=credentials["AccessKeyId"],
+        aws_secret_access_key=credentials["SecretAccessKey"],
+        aws_session_token=credentials["SessionToken"],
     )
 
-    S3.Bucket(environment.value.s3_bucket_name).Object(
-        compatible_s3_file_url
-    ).upload_fileobj(f)
+    return S3
+
+
+def normal_upload(
+    environment: CliEnvironment,
+    permissions: FileUploadPermissionsResponse,
+    file,
+):
+    S3 = get_s3_client_from_temporary_permissions(environment, permissions)
+
+    object_key = permissions["object_key"]
+    S3.Bucket(permissions["bucket_name"]).Object(object_key).upload_fileobj(
+        file
+    )
+    return object_key
 
 
 def get_uploaded_parts(
     s3_client: S3Client, s3_bucket_name, s3_file_url, upload_id
 ) -> List[PartTypeDef]:
     res = s3_client.list_parts(
         Bucket=s3_bucket_name, Key=s3_file_url, UploadId=upload_id
@@ -192,15 +256,15 @@
             UploadId=mpu_id,
             PartNumber=part_number,
         )
 
 
 def multipart_upload(
     environment: CliEnvironment,
-    s3_file_url: str,
+    permissions: FileUploadPermissionsResponse,
     file,
     resume_args,
     id_key,
     mpu_id=None,
     max_upload_workers=DEFAULT_MAX_UPLOAD_WORKERS,
 ):
     file.seek(0, 2)  # seek to end of file
@@ -209,20 +273,19 @@
     # max total upload size is 100GB
     part_size_in_bytes = max(
         10 * 1024**2, total_bytes // 500
     )  # minimum part size on aws is 5MB, list part returns max 1000 parts
 
     # we have to use low-level API to be able to support
     # resumable uploads - https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpu-upload-object.html
-    s3_client = init_s3_client(environment.value.s3_host)
-    s3_bucket_name = environment.value.s3_bucket_name
-
-    compatible_s3_file_url = get_hacked_legacy_backwards_compatible_s3_file_url(
-        environment.value.s3_bucket_root_folder, s3_file_url
-    )
+    s3_client = get_s3_client_from_temporary_permissions(
+        environment, permissions
+    ).meta.client
+    s3_bucket_name = permissions["bucket_name"]
+    compatible_s3_file_url = permissions["object_key"]
 
     if mpu_id != None:
         print(f"Resuming upload with id {mpu_id}")
         parts_already_uploaded = {
             part["PartNumber"]: part
             for part in get_uploaded_parts(
                 s3_client, s3_bucket_name, compatible_s3_file_url, mpu_id
@@ -287,49 +350,41 @@
     s3_root_folder_name: Optional[str],
     s3_file_url: str,
 ):
     return s3path_join(s3_root_folder_name or "", s3_file_url)
 
 
 def post_model_file(
+    organization_id: int,
     environment: CliEnvironment,
-    bytes_or_filepath,
-    s3_file_url,
+    filepath_or_url: str,
+    file_type: FileUploadFileType,
     resume_args,
     id_key,
     upload_id=None,
     max_upload_workers=DEFAULT_MAX_UPLOAD_WORKERS,
 ):
-    if isinstance(bytes_or_filepath, io.BytesIO):
-        f = bytes_or_filepath
-        normal_or_multipart_upload(
-            environment,
-            s3_file_url,
-            f,
-            resume_args,
-            id_key,
-            upload_id,
+    if is_model_file_link_external(filepath_or_url):
+        # attaching directly without any reuploads
+        return filepath_or_url
+
+    file_name = os.path.basename(filepath_or_url)
+
+    with open(filepath_or_url, "rb") as file:
+        return normal_or_multipart_upload(
+            organization_id,
+            environment=environment,
+            file=file,
+            file_name=file_name,
+            file_type=file_type,
+            resume_args=resume_args,
+            id_key=id_key,
+            mpu_id=upload_id,
             max_upload_workers=max_upload_workers,
         )
-    else:
-        if filepath_is_a_link(bytes_or_filepath):
-            # attaching directly without any reuploads
-            assert bytes_or_filepath == s3_file_url
-            return
-
-        with open(bytes_or_filepath, "rb") as f:
-            normal_or_multipart_upload(
-                environment,
-                s3_file_url,
-                f,
-                resume_args,
-                id_key,
-                upload_id,
-                max_upload_workers=max_upload_workers,
-            )
 
 
 def async_prediction(
     environment: CliEnvironment, organization_id: int, model_id: int
 ):
     autodl_host = environment.value.app_host
     new_url = url_with_params(
```

### Comparing `autumn8-1.0.2rc7/autumn8/lib/api_creds.py` & `autumn8-1.0.3rc1/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/lib/asyncio.py` & `autumn8-1.0.3rc1/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/lib/http.py` & `autumn8-1.0.3rc1/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/lib/logging.py` & `autumn8-1.0.3rc1/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/lib/logging.yaml` & `autumn8-1.0.3rc1/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/lib/package_resolver.py` & `autumn8-1.0.3rc1/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/autumn8/lib/service.py` & `autumn8-1.0.3rc1/autumn8/lib/service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,77 @@
 import io
 import os
 import time
 import uuid
-from pathlib import Path
 from typing import Any, Dict, Optional
 
 from autumn8.cli import pending_uploads
-from autumn8.cli.analyze import filepath_is_a_link
+from autumn8.cli.analyze import is_model_file_link_external, s3path_join
 from autumn8.cli.cli_environment import CliEnvironment
-from autumn8.common.config.s3 import get_global_anon_s3_resource, s3path_join
 from autumn8.lib import api, logging
 
 DEFAULT_MAX_UPLOAD_WORKERS = 4
 
 logger = logging.getLogger(__name__)
 
 
 def resume_upload_model(upload_task):
-    s3 = get_global_anon_s3_resource()
+    raise NotImplementedError()
 
     try:
         return upload_model(**upload_task)
     except s3.meta.client.exceptions.NoSuchUpload:
         pending_uploads.abort_and_forget_upload(upload_task["run_id"])
 
 
 def upload_model(
     environment: CliEnvironment,
-    organization_id,
+    organization_id: int,
     model_config: Dict[str, Any],
     model_filepath_or_url: str,
     input_file_path: Optional[str],
     max_upload_workers: int = DEFAULT_MAX_UPLOAD_WORKERS,
     model_file_upload_id: Optional[str] = None,
     input_file_upload_id: Optional[str] = None,
     run_id: Optional[str] = None,
     **kwargs,
 ):
     if run_id is None:  # used for resuming upload
         run_id = str(uuid.uuid4())
-    if type(model_filepath_or_url) == io.BytesIO:
-        model_filepath_or_url.seek(0)
-        model_file_name = model_config["name"]  # TODO add extension?
-    else:
-        model_file_name = os.path.basename(model_filepath_or_url)
-
-    s3_bucket_root_folder = environment.value.s3_bucket_root_folder
-
-    model_type = None if "model_type" not in kwargs else kwargs["model_type"]
-
-    s3_file_url = kwargs.get("s3_file_url") or generate_s3_file_url(
-        organization_id=organization_id,
-        run_id=run_id,
-        model_file_name=model_file_name,
-        model_file=model_filepath_or_url,
-        s3_bucket_root_folder=s3_bucket_root_folder,
-        model_type=model_type,
-    )
-
-    s3_input_file_url = None
-    if input_file_path != None and len(input_file_path) > 0:
-        filename = Path(input_file_path).name
-        s3_input_file_url = kwargs.get(
-            "s3_input_file_url"
-        ) or generate_s3_input_file_url(
-            organization_id=organization_id,
-            run_id=run_id,
-            s3_bucket_root_folder=s3_bucket_root_folder,
-            filename=filename,
-        )
 
     function_args = locals()
 
     time_start = time.time()
     logger.info("Uploading the model files...")
-    api.lab.post_model_file(
-        environment,
-        model_filepath_or_url,
-        s3_file_url,
-        function_args,
-        "model_file_upload_id",
-        model_file_upload_id,
+    model_config["s3_file_url"] = api.lab.post_model_file(
+        organization_id=organization_id,
+        environment=environment,
+        filepath_or_url=model_filepath_or_url,
+        file_type="model",
+        resume_args=function_args,
+        id_key="model_file_upload_id",
+        upload_id=model_file_upload_id,
         max_upload_workers=max_upload_workers,
     )
-    model_config["s3_file_url"] = s3_file_url
     logger.debug("Model uploaded in %.03f seconds", time.time() - time_start)
 
     # TODO: support uploading inputs via links
-    if s3_input_file_url is not None:
+    if input_file_path != None and len(input_file_path) > 0:
         time_start = time.time()
         logger.info("Uploading the input files...")
-        api.lab.post_model_file(
-            environment,
-            input_file_path,
-            s3_input_file_url,
-            function_args,
-            "input_file_upload_id",
-            input_file_upload_id,
+        model_config["s3_input_file_url"] = api.lab.post_model_file(
+            organization_id=organization_id,
+            environment=environment,
+            filepath_or_url=input_file_path,
+            file_type="input",
+            resume_args=function_args,
+            id_key="input_file_upload_id",
+            upload_id=input_file_upload_id,
             max_upload_workers=max_upload_workers,
         )
-        model_config["s3_input_file_url"] = s3_input_file_url
         logger.debug(
             "Inputs uploaded in %.03f seconds", time.time() - time_start
         )
 
     logger.info("Creating the model entry in AutoDL...")
     model_post_response = api.lab.post_model(
         environment, organization_id, model_config
@@ -133,15 +101,15 @@
     organization_id,
     run_id,
     model_file_name,
     model_file,
     s3_bucket_root_folder,
     model_type,
 ):
-    if filepath_is_a_link(model_file):
+    if is_model_file_link_external(model_file):
         return model_file
 
     additional_extension = f".{model_type}" if model_type is not None else ""
     if s3_bucket_root_folder is None:
         s3_bucket_root_folder = ""
 
     return s3path_join(
```

### Comparing `autumn8-1.0.2rc7/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.3rc1/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.2rc7
+Version: 1.0.3rc1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.2rc7/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.3rc1/autumn8.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 autumn8/cli/commands/cloud.py
 autumn8/cli/commands/models.py
 autumn8/common/__init__.py
 autumn8/common/_version.py
 autumn8/common/types.py
 autumn8/common/config/__init__.py
 autumn8/common/config/cloud_info.py
-autumn8/common/config/s3.py
 autumn8/common/config/settings.py
 autumn8/common/config/supported_instances.py
 autumn8/env/__init__.py
 autumn8/env/app.py
 autumn8/env/cli.py
 autumn8/env/predictor.py
 autumn8/env/worker.py
```

### Comparing `autumn8-1.0.2rc7/pyproject.toml` & `autumn8-1.0.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.3rc1/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc7/tests/test_settings.py` & `autumn8-1.0.3rc1/tests/test_settings.py`

 * *Files identical despite different names*

