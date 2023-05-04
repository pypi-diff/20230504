# Comparing `tmp/autumn8-1.0.2rc6.tar.gz` & `tmp/autumn8-1.0.2rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.2rc6.tar", last modified: Mon Apr 17 12:40:32 2023, max compression
+gzip compressed data, was "autumn8-1.0.2rc7.tar", last modified: Thu May  4 12:52:29 2023, max compression
```

## Comparing `autumn8-1.0.2rc6.tar` & `autumn8-1.0.2rc7.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.546841 autumn8-1.0.2rc6/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-04-17 12:40:32.546841 autumn8-1.0.2rc6/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-04-12 20:32:46.000000 autumn8-1.0.2rc6/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.526841 autumn8-1.0.2rc6/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.2rc6/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.536841 autumn8-1.0.2rc6/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.2rc6/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.2rc6/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7850 2023-04-12 20:01:39.000000 autumn8-1.0.2rc6/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-11 12:01:33.000000 autumn8-1.0.2rc6/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.536841 autumn8-1.0.2rc6/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4910 2023-04-17 12:24:37.000000 autumn8-1.0.2rc6/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16112 2023-04-14 19:00:02.000000 autumn8-1.0.2rc6/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.2rc6/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2866 2023-04-14 19:00:02.000000 autumn8-1.0.2rc6/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-04-12 20:32:46.000000 autumn8-1.0.2rc6/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-04-14 18:31:04.000000 autumn8-1.0.2rc6/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-11 12:01:33.000000 autumn8-1.0.2rc6/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-04-14 19:00:02.000000 autumn8-1.0.2rc6/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.536841 autumn8-1.0.2rc6/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-04-12 20:32:46.000000 autumn8-1.0.2rc6/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-04-17 12:32:20.000000 autumn8-1.0.2rc6/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.536841 autumn8-1.0.2rc6/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-04-12 20:32:46.000000 autumn8-1.0.2rc6/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-04-13 17:44:29.000000 autumn8-1.0.2rc6/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-14 19:01:47.000000 autumn8-1.0.2rc6/autumn8/common/config/s3.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.2rc6/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65037 2023-04-13 20:11:36.000000 autumn8-1.0.2rc6/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-04-12 20:32:46.000000 autumn8-1.0.2rc6/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.536841 autumn8-1.0.2rc6/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.2rc6/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.2rc6/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.2rc6/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.2rc6/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.2rc6/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.536841 autumn8-1.0.2rc6/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.2rc6/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.2rc6/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.2rc6/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.2rc6/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.2rc6/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.2rc6/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.546841 autumn8-1.0.2rc6/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-11 12:01:33.000000 autumn8-1.0.2rc6/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.546841 autumn8-1.0.2rc6/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.2rc6/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-04-17 12:34:33.000000 autumn8-1.0.2rc6/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10319 2023-04-17 12:34:48.000000 autumn8-1.0.2rc6/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.2rc6/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-04-17 12:34:31.000000 autumn8-1.0.2rc6/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-04-14 19:00:02.000000 autumn8-1.0.2rc6/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-11 12:01:33.000000 autumn8-1.0.2rc6/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.2rc6/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4578 2023-04-12 20:01:39.000000 autumn8-1.0.2rc6/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.526841 autumn8-1.0.2rc6/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-04-17 12:40:32.000000 autumn8-1.0.2rc6/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1417 2023-04-17 12:40:32.000000 autumn8-1.0.2rc6/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-04-17 12:40:32.000000 autumn8-1.0.2rc6/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-04-17 12:40:32.000000 autumn8-1.0.2rc6/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      132 2023-04-17 12:40:32.000000 autumn8-1.0.2rc6/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-04-17 12:40:32.000000 autumn8-1.0.2rc6/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-04-12 20:59:17.000000 autumn8-1.0.2rc6/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-04-17 12:40:32.546841 autumn8-1.0.2rc6/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.2rc6/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-04-17 12:40:32.546841 autumn8-1.0.2rc6/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.2rc6/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.2rc6/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.362130 autumn8-1.0.2rc7/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.362130 autumn8-1.0.2rc7/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7850 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-17 13:57:37.000000 autumn8-1.0.2rc7/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.362130 autumn8-1.0.2rc7/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4910 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16112 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2866 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3126 2023-04-28 11:52:10.000000 autumn8-1.0.2rc7/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-04 12:52:03.000000 autumn8-1.0.2rc7/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3117 2023-05-04 12:50:51.000000 autumn8-1.0.2rc7/autumn8/common/config/s3.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.2rc7/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.2rc7/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.2rc7/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.2rc7/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.2rc7/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.2rc7/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    10319 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.2rc7/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-03 14:35:59.000000 autumn8-1.0.2rc7/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.2rc7/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.2rc7/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4578 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.362130 autumn8-1.0.2rc7/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1440 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      132 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-04 12:52:29.000000 autumn8-1.0.2rc7/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-01 12:46:21.000000 autumn8-1.0.2rc7/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 12:52:29.372130 autumn8-1.0.2rc7/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.2rc7/tests/test_settings.py
```

### Comparing `autumn8-1.0.2rc6/PKG-INFO` & `autumn8-1.0.2rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.2rc6
+Version: 1.0.2rc7
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.2rc6/README.md` & `autumn8-1.0.2rc7/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/analyze.py` & `autumn8-1.0.2rc7/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/cli_environment.py` & `autumn8-1.0.2rc7/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/commands/cloud.py` & `autumn8-1.0.2rc7/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/commands/models.py` & `autumn8-1.0.2rc7/autumn8/cli/commands/models.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/examples.py` & `autumn8-1.0.2rc7/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/interactive.py` & `autumn8-1.0.2rc7/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/main.py` & `autumn8-1.0.2rc7/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/options.py` & `autumn8-1.0.2rc7/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/pending_uploads.py` & `autumn8-1.0.2rc7/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/cli/validation.py` & `autumn8-1.0.2rc7/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/common/config/cloud_info.py` & `autumn8-1.0.2rc7/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/common/config/s3.py` & `autumn8-1.0.2rc7/autumn8/common/config/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # from botocore.config import Config
 
 
 AUTODL_S3_REGION = "us-east-1"
 
 # TODO: unify all S3 endpoints into a single variable
 S3_SERVICE_HOST_URL = os.environ.get(
-    "BENCHMARK_AWS_S3_HOST_URL", "https://s3-accelerate.amazonaws.com"
+    "CORE_S3_HOST_URL", "https://s3-accelerate.amazonaws.com"
 )
 
 
 def init_authorized_s3(access_key: str, secret: str) -> S3ServiceResource:
     return boto3.resource(
         "s3",
         region_name=AUTODL_S3_REGION,
```

### Comparing `autumn8-1.0.2rc6/autumn8/common/config/settings.py` & `autumn8-1.0.2rc7/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/common/config/supported_instances.py` & `autumn8-1.0.2rc7/autumn8/common/config/supported_instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -312,230 +312,249 @@
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="AMD EPYC",
             cores=2,
             hyperthreading=True,
             predictor_target="c5a.large",
             predictor_num_threads=1,
             ram=4,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5a.xlarge",
             family="c5a",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="AMD EPYC",
             cores=4,
             hyperthreading=True,
             predictor_target="c5a.xlarge",
             predictor_num_threads=2,
             ram=8,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5a.2xlarge",
             family="c5a",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="AMD EPYC",
             cores=8,
             hyperthreading=True,
             predictor_target="c5a.2xlarge",
             predictor_num_threads=4,
             ram=16,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5a.4xlarge",
             family="c5a",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="AMD EPYC",
             cores=16,
             hyperthreading=True,
             predictor_target="c5a.4xlarge",
             predictor_num_threads=8,
             ram=32,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5a.8xlarge",
             family="c5a",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="AMD EPYC",
             cores=32,
             hyperthreading=True,
             predictor_target="c5a.8xlarge",
             predictor_num_threads=16,
             ram=64,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5a.12xlarge",
             family="c5a",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="AMD EPYC",
             cores=48,
             hyperthreading=True,
             predictor_target="c5a.12xlarge",
             predictor_num_threads=24,
             ram=96,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5a.16xlarge",
             family="c5a",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="AMD EPYC",
             cores=64,
             hyperthreading=True,
             predictor_target="c5a.16xlarge",
             predictor_num_threads=32,
             ram=128,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5a.24xlarge",
             family="c5a",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="AMD EPYC",
             cores=96,
             hyperthreading=True,
             predictor_target="c5a.24xlarge",
             predictor_num_threads=48,
             ram=192,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5n.large",
             family="c5n",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=2,
             hyperthreading=True,
             predictor_target="c5n.large",
             predictor_num_threads=2,
             ram=5.25,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5n.xlarge",
             family="c5n",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=4,
             hyperthreading=True,
             predictor_target="c5n.xlarge",
             predictor_num_threads=4,
             ram=10.5,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5n.2xlarge",
             family="c5n",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=8,
             hyperthreading=True,
             predictor_target="c5n.2xlarge",
             predictor_num_threads=8,
             ram=21,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5n.4xlarge",
             family="c5n",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=16,
             hyperthreading=True,
             predictor_target="c5n.4xlarge",
             predictor_num_threads=16,
             ram=42,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5n.9xlarge",
             family="c5n",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=36,
             hyperthreading=True,
             predictor_target="c5n.9xlarge",
             predictor_num_threads=36,
             ram=96,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="c5n.18xlarge",
             family="c5n",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/c5/",
             hw="Intel Xeon",
             cores=72,
             hyperthreading=True,
             predictor_target="c5n.18xlarge",
             predictor_num_threads=72,
             ram=192,
+            is_supported_by_a8f=True,
             aws_govcloud=True,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t2.small",
             family="t2",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t2/",
             hw="AMD EPYC",
             cores=1,
             hyperthreading=True,
             predictor_target="t2.small",
             predictor_num_threads=1,
             ram=2,
+            is_supported_by_a8f=True,
             aws_govcloud="US West only",
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t2.medium",
             family="t2",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t2/",
             hw="AMD EPYC",
             cores=2,
             hyperthreading=True,
             predictor_target="t2.medium",
             predictor_num_threads=2,
             ram=4,
+            is_supported_by_a8f=True,
             aws_govcloud="US West only",
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t2.large",
             family="t2",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t2/",
             hw="AMD EPYC",
             cores=2,
             hyperthreading=True,
             predictor_target="t2.large",
             predictor_num_threads=2,
             ram=8,
+            is_supported_by_a8f=True,
             aws_govcloud="US West only",
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t2.xlarge",
             family="t2",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t2/",
             hw="AMD EPYC",
             cores=4,
             hyperthreading=True,
             predictor_target="t2.xlarge",
             predictor_num_threads=4,
             ram=16,
+            is_supported_by_a8f=True,
             aws_govcloud="US West only",
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t2.2xlarge",
             family="t2",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t2/",
             hw="AMD EPYC",
             cores=8,
             hyperthreading=True,
             predictor_target="t2.2xlarge",
             predictor_num_threads=8,
             ram=32,
+            is_supported_by_a8f=True,
             aws_govcloud="US West only",
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="t3.small",
             family="t3",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/t3/",
             hw="Intel Xeon Platinum",
@@ -941,15 +960,16 @@
             cores=8,
             hyperthreading=False,
             hardcoded_usd_per_hr=0.752,
             predictor_target="g4ad.2xlarge",
             predictor_num_threads=8,
             ram=32,
             gpuram=16,
-            is_supported_by_a8f=True,
+            # TODO: gradually enable instances on staging while adding more a8f support
+            is_supported_by_a8f=False,
             aws_govcloud=False,
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="p3.2xlarge",
             family="p3",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/p3/",
             hw="NVIDIA V100 GPUs",
@@ -970,14 +990,15 @@
             hw="NVIDIA K80 GPUs",
             cores=4,
             hyperthreading=False,
             predictor_target="p2.xlarge",
             predictor_num_threads=4,
             ram=61,
             gpuram=24,
+            is_supported_by_a8f=False,
             aws_govcloud="US West only",
         ),
         **amazon_cloud_info_service.build_keyed_instance_description(
             label="p3.8xlarge",
             family="p3",
             instance_description_link="https://aws.amazon.com/ec2/instance-types/p3/",
             hw="NVIDIA V100 GPUs",
```

### Comparing `autumn8-1.0.2rc6/autumn8/common/types.py` & `autumn8-1.0.2rc7/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/env/__init__.py` & `autumn8-1.0.2rc7/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/examples/mnist.py` & `autumn8-1.0.2rc7/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/examples/model.py` & `autumn8-1.0.2rc7/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.2rc7/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.2rc7/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/lib/__init__.py` & `autumn8-1.0.2rc7/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/lib/api/cloud.py` & `autumn8-1.0.2rc7/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/lib/api/lab.py` & `autumn8-1.0.2rc7/autumn8/lib/api/lab.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/lib/api_creds.py` & `autumn8-1.0.2rc7/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/lib/http.py` & `autumn8-1.0.2rc7/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/lib/logging.py` & `autumn8-1.0.2rc7/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/lib/logging.yaml` & `autumn8-1.0.2rc7/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/lib/package_resolver.py` & `autumn8-1.0.2rc7/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8/lib/service.py` & `autumn8-1.0.2rc7/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.2rc7/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.2rc6
+Version: 1.0.2rc7
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.2rc6/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.2rc7/autumn8.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 autumn8/examples/loadMnist.py
 autumn8/examples/mnist.py
 autumn8/examples/model.py
 autumn8/examples/sbert-alpha.py
 autumn8/examples/tensorflow_custom_layers.py
 autumn8/lib/__init__.py
 autumn8/lib/api_creds.py
+autumn8/lib/asyncio.py
 autumn8/lib/http.py
 autumn8/lib/logging.py
 autumn8/lib/logging.yaml
 autumn8/lib/package_resolver.py
 autumn8/lib/service.py
 autumn8/lib/api/__init__.py
 autumn8/lib/api/cloud.py
```

### Comparing `autumn8-1.0.2rc6/pyproject.toml` & `autumn8-1.0.2rc7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.2rc7/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.2rc6/tests/test_settings.py` & `autumn8-1.0.2rc7/tests/test_settings.py`

 * *Files identical despite different names*

