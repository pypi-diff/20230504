# Comparing `tmp/autumn8-1.0.3rc2.tar.gz` & `tmp/autumn8-1.0.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.3rc2.tar", last modified: Thu May  4 15:15:22 2023, max compression
+gzip compressed data, was "autumn8-1.0.3rc3.tar", last modified: Thu May  4 15:35:04 2023, max compression
```

## Comparing `autumn8-1.0.3rc2.tar` & `autumn8-1.0.3rc3.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.643581 autumn8-1.0.3rc2/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 15:15:22.643581 autumn8-1.0.3rc2/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.613580 autumn8-1.0.3rc2/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-04 13:24:26.000000 autumn8-1.0.3rc2/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-17 13:57:37.000000 autumn8-1.0.3rc2/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4910 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16112 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2866 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-04 13:24:26.000000 autumn8-1.0.3rc2/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-04 15:13:05.000000 autumn8-1.0.3rc2/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.3rc2/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.633580 autumn8-1.0.3rc2/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.3rc2/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.3rc2/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.3rc2/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.3rc2/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.3rc2/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.633580 autumn8-1.0.3rc2/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.633580 autumn8-1.0.3rc2/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.3rc2/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.633580 autumn8-1.0.3rc2/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11865 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.3rc2/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-04 14:29:39.000000 autumn8-1.0.3rc2/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.3rc2/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.3rc2/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-04 13:24:26.000000 autumn8-1.0.3rc2/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.623580 autumn8-1.0.3rc2/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1412 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-04 15:15:22.000000 autumn8-1.0.3rc2/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1959 2023-05-04 15:12:12.000000 autumn8-1.0.3rc2/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-04 15:15:22.643581 autumn8-1.0.3rc2/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:15:22.643581 autumn8-1.0.3rc2/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.3rc2/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.114351 autumn8-1.0.3rc3/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 15:35:04.114351 autumn8-1.0.3rc3/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.3rc3/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.104351 autumn8-1.0.3rc3/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.3rc3/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.104351 autumn8-1.0.3rc3/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.3rc3/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.3rc3/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-04 13:24:26.000000 autumn8-1.0.3rc3/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-17 13:57:37.000000 autumn8-1.0.3rc3/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.104351 autumn8-1.0.3rc3/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4109 2023-05-04 15:33:49.000000 autumn8-1.0.3rc3/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16909 2023-05-04 15:33:49.000000 autumn8-1.0.3rc3/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.3rc3/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1795 2023-05-04 15:33:49.000000 autumn8-1.0.3rc3/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-05-01 12:46:21.000000 autumn8-1.0.3rc3/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.3rc3/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-04 13:24:26.000000 autumn8-1.0.3rc3/autumn8/cli/pending_uploads.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.104351 autumn8-1.0.3rc3/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.3rc3/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-04 15:34:08.000000 autumn8-1.0.3rc3/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.104351 autumn8-1.0.3rc3/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.3rc3/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.3rc3/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.3rc3/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.3rc3/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.3rc3/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.114351 autumn8-1.0.3rc3/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.3rc3/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.3rc3/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.3rc3/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.3rc3/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.3rc3/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.114351 autumn8-1.0.3rc3/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.3rc3/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.3rc3/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.3rc3/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.3rc3/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.3rc3/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.3rc3/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.114351 autumn8-1.0.3rc3/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.3rc3/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.114351 autumn8-1.0.3rc3/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.3rc3/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3637 2023-05-04 15:33:49.000000 autumn8-1.0.3rc3/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12578 2023-05-04 15:34:18.000000 autumn8-1.0.3rc3/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.3rc3/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-05-04 15:33:49.000000 autumn8-1.0.3rc3/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.3rc3/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.3rc3/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-04 13:24:26.000000 autumn8-1.0.3rc3/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.104351 autumn8-1.0.3rc3/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 15:35:04.000000 autumn8-1.0.3rc3/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1343 2023-05-04 15:35:04.000000 autumn8-1.0.3rc3/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-04 15:35:04.000000 autumn8-1.0.3rc3/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-04 15:35:04.000000 autumn8-1.0.3rc3/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-04 15:35:04.000000 autumn8-1.0.3rc3/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-04 15:35:04.000000 autumn8-1.0.3rc3/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-04 15:34:18.000000 autumn8-1.0.3rc3/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-04 15:35:04.114351 autumn8-1.0.3rc3/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.3rc3/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:35:04.114351 autumn8-1.0.3rc3/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.3rc3/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.3rc3/tests/test_settings.py
```

### Comparing `autumn8-1.0.3rc2/PKG-INFO` & `autumn8-1.0.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.3rc2
+Version: 1.0.3rc3
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.3rc2/README.md` & `autumn8-1.0.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/cli/analyze.py` & `autumn8-1.0.3rc3/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/cli/cli_environment.py` & `autumn8-1.0.3rc3/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/cli/commands/cloud.py` & `autumn8-1.0.3rc3/autumn8/cli/commands/cloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import json
 from typing import Optional
 
 import click
 import questionary
 
-import autumn8.lib.api.cloud as cloud_api
 from autumn8.cli import options
 from autumn8.cli.cli_environment import CliEnvironment
-from autumn8.cli.interactive import (
-    normalize_args,
-    validate_and_ask_about_schedule,
-)
+from autumn8.cli.interactive import normalize_args
 from autumn8.common.config.settings import CloudServiceProvider
 from autumn8.common.types import Sla
 from autumn8.lib import logging
+from autumn8.lib.api import cloud
 
 logger = logging.getLogger(__name__)
 
 
 @click.group(context_settings={"token_normalize_func": normalize_args})
 def cloud_commands_group():
     pass
@@ -40,15 +37,15 @@
     model_id: int,
     environment: CliEnvironment,
     cloud_provider: CloudServiceProvider,
     quiet,
 ):
     """List running deployments."""
     logger.info("Fetching the list of deployments...")
-    deployments = cloud_api.get_running_deployments(
+    deployments = cloud.get_running_deployments(
         organization_id,
         environment,
         model_id=model_id,
         service_provider=cloud_provider,
     )
 
     click.echo(json.dumps(deployments, indent=4))
@@ -72,88 +69,61 @@
     "--model_id",
     prompt=True,
     type=int,
     help="Model ID to deploy",
     # TODO: add a better interactive prompt listing all available models
 )
 @click.option(
-    "-s/-i",
-    "should_schedule",
-    "--schedule/--immediate",
-    is_flag=True,
-    default=False,
-    help="Schedule the deployment to run in the future",
-)
-@click.option(
-    "--schedule_on",
-    type=str,
-    help="Schedule the deployment on given date",
-)
-@click.option(
-    "--deployment_id",
-    type=str,
-    help="Update an existing deployment, retaining its URL",
-)
-@click.option(
     "-b",
     "--deploy_best",
     "autopick_machine_by_best_sla",
     type=click.Choice(list(Sla), case_sensitive=False),
     help="Let Autumn8 pick the server type automatically for the deployment",
 )
 @options.use_cloud_provider_picker(
     # prompt disabled, as only A8F works atm
     optional=True,
     default_value=CloudServiceProvider.AUTUMN8,
 )
 def deploy(
     organization_id: int,
     model_id: int,
-    should_schedule: bool,
-    schedule_on: Optional[str],
-    deployment_id: Optional[str],
     machine_type: Optional[str],
     environment: CliEnvironment,
     cloud_provider: CloudServiceProvider,
     autopick_machine_by_best_sla: Optional[Sla],
     quiet,
 ):
     """Deploy a model from AutoDL onto cloud."""
 
     if machine_type is None and autopick_machine_by_best_sla is None:
         machine_type = questionary.text(
             message="Machine type (ie. c5.2xlarge)"
-        ).unsafe_ask()
-
-    schedule_on = validate_and_ask_about_schedule(should_schedule, schedule_on)
+        ).ask()
 
     logger.info(
         "Launching a new deployment with %s...",
         machine_type or f"best {autopick_machine_by_best_sla}",
     )
     if machine_type is not None:
-        deployments = cloud_api.deploy(
+        deployments = cloud.deploy(
             organization_id,
             environment,
             machine_type=machine_type,
             service_provider=cloud_provider,
-            schedule_on=schedule_on,
-            deployment_id=deployment_id,
             model_id=model_id,
         )
     else:
         assert autopick_machine_by_best_sla is not None
 
-        deployments = cloud_api.deploy_by_best_sla(
+        deployments = cloud.deploy_by_best_sla(
             organization_id,
             environment,
             best_sla=autopick_machine_by_best_sla,
             service_provider=cloud_provider,
-            schedule_on=schedule_on,
-            deployment_id=deployment_id,
             model_id=model_id,
         )
 
     click.echo(json.dumps(deployments, indent=4))
 
 
 @cloud_commands_group.command()
@@ -175,11 +145,11 @@
     organization_id: int,
     deployment_id: str,
     environment: CliEnvironment,
     cloud_provider: CloudServiceProvider,
     quiet,
 ):
     """Terminate a running deployment."""
-    response = cloud_api.terminate_deployment(
+    response = cloud.terminate_deployment(
         organization_id, environment, deployment_id, cloud_provider
     )
     click.echo(json.dumps(response, indent=4))
```

### Comparing `autumn8-1.0.3rc2/autumn8/cli/commands/models.py` & `autumn8-1.0.3rc3/autumn8/cli/commands/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 import time
 import uuid
 import zipfile
 from configparser import NoOptionError, NoSectionError
 from typing import List, Optional
 
 import click
+import jsonschema
 import questionary
+from jsonschema import validate
 
 from autumn8.cli import options
 from autumn8.cli.analyze import analyze_model_file, suggest_model_name
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.cli.examples import example_model_names
 from autumn8.cli.interactive import (
     announce_model_upload_response,
     normalize_args,
 )
-from autumn8.cli.validation import validate_input_dims_json, validate_input_file
 from autumn8.common.config.settings import supported_quants
 from autumn8.lib import api_creds, logging
 from autumn8.lib import service as autodl
 from autumn8.lib.api import lab
 
 USER_ID_LENGTH = len(str(uuid.uuid4()))
 API_KEY_LENGTH = 32
@@ -82,14 +83,56 @@
         logger.info(f"API Key: {api_key}")
 
     api_creds.store_api_creds(user_id, api_key)
     user_data = lab.fetch_user_data(environment)
     logger.info(f"Credentials set up successfully for {user_data['email']}!")
 
 
+INPUT_DIMS_JSONSCHEMA = {
+    "type": "array",
+    "minItems": 1,
+    "items": {
+        "type": "array",
+        "minItems": 1,
+        "items": {"type": "number"},
+    },
+}
+
+
+def validate_input_dims_json(jsonString):
+    if jsonString == "":
+        return True
+
+    try:
+        jsonData = json.loads(jsonString)
+        validate(instance=jsonData, schema=INPUT_DIMS_JSONSCHEMA)
+    except (
+        jsonschema.exceptions.ValidationError,
+        json.decoder.JSONDecodeError,
+    ):
+        return False
+    return True
+
+
+def validate_input_file(path):
+    if not os.path.exists(path):
+        return False
+
+    if not os.path.isfile(path):
+        return False
+
+    try:
+        with open(path, "r") as f:
+            jsonData = json.load(f)
+
+    except json.decoder.JSONDecodeError:
+        return False
+    return True
+
+
 def normalize_input_dims_for_api(input_dims):
     if not input_dims:
         return None
 
     inputs = json.loads(input_dims)
     inputs = [[str(dim) for dim in input] for input in inputs]
     return json.dumps(inputs, separators=(",", ":"))
```

### Comparing `autumn8-1.0.3rc2/autumn8/cli/examples.py` & `autumn8-1.0.3rc3/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/cli/interactive.py` & `autumn8-1.0.3rc3/autumn8/cli/interactive.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import datetime
 import json
-from typing import Optional
 
 import click
 import questionary
 from questionary import Choice
 
-from autumn8.cli.validation import IsoDatetimeValidator
 from autumn8.lib import logging
 from autumn8.lib.api.lab import fetch_user_data
 
 logger = logging.getLogger(__name__)
 
 
 def normalize_args(name: str):
@@ -59,36 +56,7 @@
     return announce_json_response({"model_details": model_upload_response})
 
 
 def announce_json_response(model_upload_response):
     logger.info("")  # newline
     logger.info("Done!")
     click.echo(json.dumps(model_upload_response, indent=4))
-
-
-def validate_and_ask_about_schedule(
-    should_schedule: bool, schedule_on: Optional[str]
-) -> Optional[str]:
-    if schedule_on is not None:
-        try:
-            IsoDatetimeValidator.validate_string(schedule_on)
-            return schedule_on
-        except questionary.ValidationError as exc:
-            click.echo(
-                f"ERROR: '{schedule_on}' is not a valid date specification"
-            )
-            click.echo(exc.message + "\n")
-
-    if should_schedule or schedule_on is not None:
-        prefill_value = (
-            datetime.datetime.now().astimezone().replace(microsecond=0)
-            + datetime.timedelta(minutes=5)
-        ).isoformat()
-
-        return questionary.text(
-            "Pick time to schedule the model to deploy on\n"
-            + f"(ie. in 5 minutes it will be '{prefill_value}')\n",
-            default=schedule_on or prefill_value,
-            validate=IsoDatetimeValidator,
-        ).unsafe_ask()
-
-    return None
```

### Comparing `autumn8-1.0.3rc2/autumn8/cli/main.py` & `autumn8-1.0.3rc3/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/cli/options.py` & `autumn8-1.0.3rc3/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/cli/pending_uploads.py` & `autumn8-1.0.3rc3/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/common/config/cloud_info.py` & `autumn8-1.0.3rc3/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/common/config/settings.py` & `autumn8-1.0.3rc3/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/common/config/supported_instances.py` & `autumn8-1.0.3rc3/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/common/types.py` & `autumn8-1.0.3rc3/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/env/__init__.py` & `autumn8-1.0.3rc3/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/examples/mnist.py` & `autumn8-1.0.3rc3/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/examples/model.py` & `autumn8-1.0.3rc3/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.3rc3/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.3rc3/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/lib/__init__.py` & `autumn8-1.0.3rc3/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/lib/api/cloud.py` & `autumn8-1.0.3rc3/autumn8/lib/api/cloud.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import requests
 from requests.auth import HTTPBasicAuth
 
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.common.config.settings import CloudServiceProvider
 from autumn8.common.types import Sla
+from autumn8.lib.api.lab import require_ok_response, url_with_params
 from autumn8.lib.api_creds import retrieve_api_creds
-from autumn8.lib.http import require_ok_response, url_with_params
 
 DEFAULT_API_TIMEOUT = 60
 
 
 def get_running_deployments(
     organization_id: int,
     environment: CliEnvironment,
@@ -40,26 +40,22 @@
 
 
 def deploy_by_best_sla(
     organization_id: int,
     environment: CliEnvironment,
     model_id: int,
     best_sla: Sla,
-    schedule_on: Optional[str],
-    deployment_id: Optional[str],
     service_provider: CloudServiceProvider,
 ):
     autodl_host = environment.value.app_host
 
     params = {
         "organization_id": organization_id,
         "model_id": model_id,
         "best_sla": best_sla.value,
-        "schedule_on": schedule_on,
-        "deployment_id": deployment_id,
         "cloud_service_provider": service_provider.value,
     }
 
     print("sending", params)
 
     deployments_api_route = f"{autodl_host}/api/cloud/deployments/by_sla"
     response = requests.post(
@@ -74,26 +70,22 @@
 
 
 def deploy(
     organization_id: int,
     environment: CliEnvironment,
     model_id: int,
     machine_type: str,
-    schedule_on: Optional[str],
-    deployment_id: Optional[str],
     service_provider: CloudServiceProvider,
 ):
     autodl_host = environment.value.app_host
 
     params = {
         "organization_id": organization_id,
         "model_id": model_id,
         "machine_type": machine_type,
-        "schedule_on": schedule_on,
-        "deployment_id": deployment_id,
         "cloud_service_provider": service_provider.value,
     }
 
     deployments_api_route = f"{autodl_host}/api/cloud/deployments"
     response = requests.post(
         url_with_params(deployments_api_route, params),
         headers={"Content-Type": "application/json"},
```

### Comparing `autumn8-1.0.3rc2/autumn8/lib/api/lab.py` & `autumn8-1.0.3rc3/autumn8/lib/api/lab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,63 @@
 import io
 import json
+import os
+import urllib
+import urllib.parse
+from http import HTTPStatus
 from threading import Lock
-from typing import Any, Dict, List, Optional
-
-import appdirs
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
 import appdirs
 import boto3
-import httpx
 import requests
 from mypy_boto3_s3 import S3Client
 from mypy_boto3_s3.type_defs import PartTypeDef
 from mypy_boto3_sts.type_defs import CredentialsTypeDef
 from requests.auth import HTTPBasicAuth
 from tqdm.contrib.concurrent import thread_map
 
 from autumn8.cli import pending_uploads
 from autumn8.cli.analyze import is_model_file_link_external, s3path_join
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.lib import logging
 from autumn8.lib.api_creds import retrieve_api_creds
-from autumn8.lib.http import require_ok_response, url_with_params
 
 DEFAULT_MAX_UPLOAD_WORKERS = 4
 
 APP_NAME = "autumn8"
 APP_AUTHOR = "autumn8"
 
 logger = logging.getLogger(__name__)
 
 data_dir = appdirs.user_data_dir(APP_NAME, APP_AUTHOR)
 
 
+def url_with_params(url: str, params: Dict[str, Union[str, int]]):
+    url_parse = urllib.parse.urlparse(url)
+    url_new_query = urllib.parse.urlencode(params)
+    url_parse = url_parse._replace(query=url_new_query)
+
+    new_url = urllib.parse.urlunparse(url_parse)
+    return new_url
+
+
+def require_ok_response(
+    response: Union[requests.Response, httpx.Response]
+) -> None:
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        raise Exception(
+            f"Received response {response.status_code}:\n{response.text}\n\nUser not authenticated; please run `autumn8-cli login` to authorize your CLI"
+        )
+    if response.status_code != HTTPStatus.OK:
+        raise Exception(
+            f"Received response {response.status_code}:\n{response.text}"
+        )
+
+
 def fetch_user_data(environment: CliEnvironment):
     user_id, api_key = None, None
     autodl_host = environment.value.app_host
     try:
         user_id, api_key = retrieve_api_creds()
     except:
         raise Exception(
```

### Comparing `autumn8-1.0.3rc2/autumn8/lib/api_creds.py` & `autumn8-1.0.3rc3/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/lib/logging.py` & `autumn8-1.0.3rc3/autumn8/lib/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # pyright: reportWildcardImportFromLibrary=false
 # pylint: disable=wildcard-import,unused-wildcard-import
 
 import logging
 import logging.config
 import os
 from logging import *
-from logging import Logger
 from logging import getLogger as oldGetLogger
 from typing import Optional
 
 import yaml
 
 with open(
     os.path.join(os.path.dirname(__file__), ".", "logging.yaml"),
```

### Comparing `autumn8-1.0.3rc2/autumn8/lib/logging.yaml` & `autumn8-1.0.3rc3/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/lib/package_resolver.py` & `autumn8-1.0.3rc3/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8/lib/service.py` & `autumn8-1.0.3rc3/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.3rc3/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.3rc2
+Version: 1.0.3rc3
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.3rc2/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.3rc3/autumn8.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 autumn8/cli/analyze.py
 autumn8/cli/cli_environment.py
 autumn8/cli/examples.py
 autumn8/cli/interactive.py
 autumn8/cli/main.py
 autumn8/cli/options.py
 autumn8/cli/pending_uploads.py
-autumn8/cli/validation.py
 autumn8/cli/commands/cloud.py
 autumn8/cli/commands/models.py
 autumn8/common/__init__.py
 autumn8/common/_version.py
 autumn8/common/types.py
 autumn8/common/config/__init__.py
 autumn8/common/config/cloud_info.py
@@ -36,16 +35,14 @@
 autumn8/examples/loadMnist.py
 autumn8/examples/mnist.py
 autumn8/examples/model.py
 autumn8/examples/sbert-alpha.py
 autumn8/examples/tensorflow_custom_layers.py
 autumn8/lib/__init__.py
 autumn8/lib/api_creds.py
-autumn8/lib/asyncio.py
-autumn8/lib/http.py
 autumn8/lib/logging.py
 autumn8/lib/logging.yaml
 autumn8/lib/package_resolver.py
 autumn8/lib/service.py
 autumn8/lib/api/__init__.py
 autumn8/lib/api/cloud.py
 autumn8/lib/api/lab.py
```

### Comparing `autumn8-1.0.3rc2/pyproject.toml` & `autumn8-1.0.3rc3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
   "appdirs",
   "wheel>=0.31.0",
   "boto3>=1.20.15",
   "click>=8.0.1",
   "questionary>=1.10.0",
   "requests",
   "httpx",
-  "tqdm"
+  "tqdm",
+  "boto3-stubs[s3,sts]",
 ]
 
 [project]
 name = "autumn8"
 authors = [{ name = "Autumn8", email = "team@autumn8.ai" }]
 requires-python = ">=3.8"
 # packages=find_namespace_packages(include=["autumn8", "autumn8.*"]),
```

### Comparing `autumn8-1.0.3rc2/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.3rc3/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc2/tests/test_settings.py` & `autumn8-1.0.3rc3/tests/test_settings.py`

 * *Files identical despite different names*

