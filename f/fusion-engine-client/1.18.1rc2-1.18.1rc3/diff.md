# Comparing `tmp/fusion-engine-client-1.18.1rc2.tar.gz` & `tmp/fusion-engine-client-1.18.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.18.1rc2.tar", last modified: Tue Apr 25 23:02:31 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.18.1rc3.tar", last modified: Wed May  3 22:14:26 2023, max compression
```

## Comparing `fusion-engine-client-1.18.1rc2.tar` & `fusion-engine-client-1.18.1rc3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.586766 fusion-engine-client-1.18.1rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-25 23:02:31.586766 fusion-engine-client-1.18.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.574766 fusion-engine-client-1.18.1rc2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    13145 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.574766 fusion-engine-client-1.18.1rc2/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.578766 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   105922 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.578766 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55187 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.582766 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.582766 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.578766 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 23:02:31.000000 fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 23:02:31.586766 fusion-engine-client-1.18.1rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:02:31.586766 fusion-engine-client-1.18.1rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-04-25 23:01:44.000000 fusion-engine-client-1.18.1rc2/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13145 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   107613 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55470 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22860 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29544 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23392 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.628854 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 22:14:26.000000 fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:14:26.632854 fusion-engine-client-1.18.1rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-05-03 22:13:50.000000 fusion-engine-client-1.18.1rc3/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.18.1rc2/PKG-INFO` & `fusion-engine-client-1.18.1rc3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.18.1rc2
+Version: 1.18.1rc3
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.18.1rc2/README.md` & `fusion-engine-client-1.18.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/bin/p1_extract` & `fusion-engine-client-1.18.1rc3/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/bin/p1_print` & `fusion-engine-client-1.18.1rc3/bin/p1_print`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                 table_html += f'<td>{col_data[row_idx]}</td>'
 
         table_html += '</tr>'
     table_html += '''\
   </tbody>
 </table>
 '''
-    return table_html
+    return table_html.replace('\n', '')
 
 
 _page_template = '''\
 <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
 <html>
 <head>
   <meta content="text/html; charset=ISO-8859-1" http-equiv="content-type">
@@ -135,15 +135,20 @@
             'time_range': time_range,
             'max_messages': max_messages,
             'show_progress': True,
             'return_numpy': True
         }
 
         self.t0 = self.reader.t0
+        if self.t0 is None:
+            self.t0 = Timestamp()
+
         self.system_t0 = self.reader.get_system_t0()
+        if self.system_t0 is None:
+            self.system_t0 = np.nan
 
         self.plots = {}
         self.summary = ''
 
         self._mapbox_token_missing = False
 
         if self.output_dir is not None:
@@ -217,26 +222,15 @@
                 dgps_time = dgps_time[idx]
 
                 figure.layout.annotations[0].text += "<br>Decimated %dx" % step
             else:
                 p1_time = pose_data.p1_time
                 gps_time = pose_data.gps_time
 
-            def gps_sec_to_string(gps_time_sec):
-                if np.isnan(gps_time_sec):
-                    return "GPS: N/A<br>UTC: N/A"
-                else:
-                    SECS_PER_WEEK = 7 * 24 * 3600.0
-                    week = int(gps_time_sec / SECS_PER_WEEK)
-                    tow_sec = gps_time_sec - week * SECS_PER_WEEK
-                    utc_time = gpstime.fromgps(gps_time_sec)
-                    return "GPS: %d:%.3f (%.3f sec)<br>UTC: %s" %\
-                           (week, tow_sec, gps_time_sec, utc_time.strftime('%Y-%m-%d %H:%M:%S %Z'))
-
-            text = ['P1: %.3f sec<br>%s' % (p, gps_sec_to_string(g)) for p, g in zip(p1_time, gps_time)]
+            text = ['P1: %.3f sec<br>%s' % (p, self._gps_sec_to_string(g)) for p, g in zip(p1_time, gps_time)]
             figure.add_trace(go.Scattergl(x=time, y=np.full_like(time, 1), name='P1/GPS Time', text=text,
                                           mode='markers'),
                              1, 1)
 
             figure.add_trace(go.Scattergl(x=time, y=dp1_time, name='P1 Time Interval', text=text,
                                           mode='markers'),
                              2, 1)
@@ -1889,23 +1883,49 @@
         counts.append(None)
         percents.append(None)
 
         types.append('Total')
         counts.append('%d' % num_pose_messages)
         percents.append('')
 
-        types.append('Processed Duration')
-        counts.append('%.1f seconds' % processing_duration_sec)
-        percents.append('')
+        solution_type_table = _data_to_table(['Position Type', 'Count', 'Percent'], [types, counts, percents])
 
-        types.append('Total Log Duration')
-        counts.append('%.1f seconds' % log_duration_sec)
-        percents.append('')
+        # Determine the GPS start time if pose data is present. GPS time may not appear in the first pose update, and
+        # even if it does, t0 may not correspond with the first pose message if something else was output first. So just
+        # in case, we'll approximate the GPS time _at_ t0 if needed.
+        idx = find_first(~np.isnan(pose_data.gps_time))
+        if idx >= 0:
+            dt_p1_sec = pose_data.p1_time[idx] - float(self.t0)
+            t0_gps = Timestamp(pose_data.gps_time[idx]) - dt_p1_sec
+            # If the first pose is pretty close to t0, we'll assume the approximation is reasonably accurate and not
+            # bother reporting it.
+            t0_is_approx = dt_p1_sec > 10.0
+        else:
+            t0_gps = Timestamp()
+            t0_is_approx = False
 
-        solution_type_table = _data_to_table(['Position Type', 'Count', 'Percent'], [types, counts, percents])
+        # Create a table with log times and durations.
+        descriptions = [
+            'Start Time',
+            '',
+            '',
+            'Processed Duration',
+            'Total Log Duration',
+        ]
+        times = [
+            str(self.t0),
+            system_time_to_str(self.system_t0, is_seconds=True).replace(' time', ':'),
+            # Note: Temporarily replacing <br> so it doesn't get stripped by _data_to_table().
+            self._gps_sec_to_string(t0_gps) \
+                .replace('<br>', (' (approximated)' if t0_is_approx else '') + '<brbak>') \
+                .replace('<brbak>', '<br>'),
+            '%.1f seconds' % processing_duration_sec,
+            log_duration_sec,
+        ]
+        time_table = _data_to_table(['Description', 'Time'], [descriptions, times])
 
         # Create a table with the types and counts of each FusionEngine message type in the log.
         message_types, message_counts = np.unique(reduced_index['type'], return_counts=True)
         message_types = [MessageType.get_type_string(t) for t in message_types]
 
         message_counts = message_counts.tolist()
         message_types.append(None)
@@ -1917,33 +1937,36 @@
         message_table = _data_to_table(['Message Type', 'Count'], [message_types, message_counts])
 
         # Create a software version table.
         result = self.reader.read(message_types=[VersionInfoMessage.MESSAGE_TYPE], remove_nan_times=False,
                                   **self.params)
         if len(result[VersionInfoMessage.MESSAGE_TYPE].messages) != 0:
             version = result[VersionInfoMessage.MESSAGE_TYPE].messages[-1]
-            version_types = {'fw': 'Firmware', 'engine': 'FusionEngine', 'hw': 'Hardware', 'rx': 'GNSS Receiver'}
+            version_types = {'fw': 'Firmware', 'engine': 'FusionEngine', 'os': 'OS', 'rx': 'GNSS Receiver'}
             version_values = [str(vars(version)[k + '_version_str']) for k in version_types.keys()]
             version_table = _data_to_table(['Type', 'Version'], [list(version_types.values()), version_values])
         else:
             version_table = 'No version information.'
 
         # Now populate the summary.
         if self.summary != '':
             self.summary += '\n\n'
 
         args = {
             'message_table': message_table,
             'version_table': version_table,
             'solution_type_table': solution_type_table,
+            'time_table': time_table,
         }
 
         self.summary += """
 %(version_table)s
 
+%(time_table)s
+
 %(solution_type_table)s
 
 %(message_table)s
 """ % args
 
     def _add_page(self, name, html_body, title=None):
         if title is None:
@@ -2036,14 +2059,33 @@
             data = result[message_type]
             if len(data.p1_time) > 0:
                 selected_type = message_type_to_class[message_type]
                 break
         return selected_type
 
     @classmethod
+    def _gps_sec_to_string(cls, gps_time_sec):
+        if isinstance(gps_time_sec, Timestamp):
+            gps_time_sec = float(gps_time_sec)
+
+        if np.isnan(gps_time_sec):
+            return "GPS: N/A<br>UTC: N/A"
+        else:
+            SECS_PER_WEEK = 7 * 24 * 3600.0
+            week = int(gps_time_sec / SECS_PER_WEEK)
+            tow_sec = gps_time_sec - week * SECS_PER_WEEK
+            utc_time = gpstime.fromgps(gps_time_sec)
+
+            utc_time_str = utc_time.strftime('%Y-%m-%d %H:%M:%S')
+            utc_time_str += ('%.03f' % (utc_time.microsecond * 1e-6))[1:]
+
+            return "GPS: %d:%.3f (%.3f sec)<br>UTC: %s" %\
+                   (week, tow_sec, gps_time_sec, utc_time_str)
+
+    @classmethod
     def _get_measurement_time(cls, data, time_source: SystemTimeSource) -> np.ndarray:
         if time_source == SystemTimeSource.P1_TIME:
             return data.p1_time
         else:
             return data.measurement_time
 
     @classmethod
```

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,24 +205,27 @@
     PQTMVERNO = 1200
     PQTMVER = 1201
     PQTMGNSS = 1202
     PQTMVERNO_SUB = 1203
     PQTMVER_SUB = 1204
     PQTMTXT = 1205
 
+
 class IonoDelayModel(IntEnum):
     AUTO = 0
     OFF = 1
     KLOBUCHAR = 2
 
+
 class TropoDelayModel(IntEnum):
     AUTO = 0
     OFF = 1
     SAASTAMOINEN = 2
 
+
 def get_message_type_string(protocol: ProtocolType, message_id: int):
     if message_id == ALL_MESSAGES_ID:
         return 'ALL (%d)' % message_id
     else:
         enum = None
         try:
             if protocol == ProtocolType.NMEA:
@@ -1250,15 +1253,18 @@
         return result
 
     def __str__(self):
         return construct_message_to_string(
             message=self, construct=self.SetMessageRateConstruct,
             title=f'Set Message Output Rate Command',
             fields=['output_interface', 'protocol', 'message_id', 'rate', 'flags'],
-            value_to_string={'flags': lambda x: '0x%X' % x})
+            value_to_string={
+                'message_id': lambda x: get_message_type_string(protocol=self.protocol, message_id=x),
+                'flags': lambda x: '0x%X' % x
+            })
 
     @classmethod
     def calcsize(cls) -> int:
         return cls.SetMessageRateConstruct.sizeof()
 
 
 class GetMessageRate(MessagePayload):
@@ -1308,15 +1314,18 @@
                   f'message_id={self.message_id}]'
         return result
 
     def __str__(self):
         return construct_message_to_string(
             message=self, construct=self.GetMessageRateConstruct,
             title=f'Get Message Output Rate Command',
-            fields=['output_interface', 'protocol', 'request_source', 'message_id'])
+            fields=['output_interface', 'protocol', 'request_source', 'message_id'],
+            value_to_string={
+                'message_id': lambda x: get_message_type_string(protocol=self.protocol, message_id=x)
+            })
 
     @classmethod
     def calcsize(cls) -> int:
         return cls.GetMessageRateConstruct.sizeof()
 
 
 class RateResponseEntry(NamedTuple):
```

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,55 +357,55 @@
     MESSAGE_TYPE = MessageType.VERSION_INFO
     MESSAGE_VERSION = 0
 
     VersionInfoMessageConstruct = Struct(
         "system_time_ns" / Int64ul,
         "fw_version_length" / Int8ul,
         "engine_version_length" / Int8ul,
-        "hw_version_length" / Int8ul,
+        "os_version_length" / Int8ul,
         "rx_version_length" / Int8ul,
         Padding(4),
         "fw_version_str" / PaddedString(this.fw_version_length, 'utf8'),
         "engine_version_str" / PaddedString(this.engine_version_length, 'utf8'),
-        "hw_version_str" / PaddedString(this.hw_version_length, 'utf8'),
+        "os_version_str" / PaddedString(this.os_version_length, 'utf8'),
         "rx_version_str" / PaddedString(this.rx_version_length, 'utf8'),
     )
 
     def __init__(self):
         self.system_time_ns = 0
         self.fw_version_str = ""
         self.engine_version_str = ""
-        self.hw_version_str = ""
+        self.os_version_str = ""
         self.rx_version_str = ""
 
     def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
         values = dict(self.__dict__)
         values['fw_version_length'] = len(self.fw_version_str)
         values['engine_version_length'] = len(self.engine_version_str)
-        values['hw_version_length'] = len(self.hw_version_str)
+        values['os_version_length'] = len(self.os_version_str)
         values['rx_version_length'] = len(self.rx_version_str)
         packed_data = self.VersionInfoMessageConstruct.build(values)
         return PackedDataToBuffer(packed_data, buffer, offset, return_buffer)
 
     def unpack(self, buffer: bytes, offset: int = 0, message_version: int = MessagePayload._UNSPECIFIED_VERSION) -> int:
         parsed = self.VersionInfoMessageConstruct.parse(buffer[offset:])
         self.__dict__.update(parsed)
         return parsed._io.tell()
 
     def __repr__(self):
         result = super().__repr__()[:-1]
-        result += f', fw={self.fw_version_str}, engine={self.engine_version_str}, hw={self.hw_version_str} ' \
+        result += f', fw={self.fw_version_str}, engine={self.engine_version_str}, os={self.os_version_str} ' \
                   f'rx={self.rx_version_str}]'
         return result
 
     def __str__(self):
         string = f'Version Info @ %s\n' % system_time_to_str(self.system_time_ns)
         string += f'  Firmware: {self.fw_version_str}\n'
         string += f'  FusionEngine: {self.engine_version_str}\n'
-        string += f'  Hardware: {self.hw_version_str}\n'
+        string += f'  OS: {self.os_version_str}\n'
         string += f'  GNSS receiver: {self.rx_version_str}'
         return string
 
     def calcsize(self) -> int:
         return len(self.pack())
```

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/device.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/measurement_details.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/measurements.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/messages/timestamp.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client/utils/trace.py` & `fusion-engine-client-1.18.1rc3/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.18.1rc2
+Version: 1.18.1rc3
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.18.1rc2/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.18.1rc3/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/setup.py` & `fusion-engine-client-1.18.1rc3/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_config.py` & `fusion-engine-client-1.18.1rc3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_construct_utils.py` & `fusion-engine-client-1.18.1rc3/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_data_loader.py` & `fusion-engine-client-1.18.1rc3/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_decoder.py` & `fusion-engine-client-1.18.1rc3/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_encoder.py` & `fusion-engine-client-1.18.1rc3/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_enum_utils.py` & `fusion-engine-client-1.18.1rc3/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_file_index.py` & `fusion-engine-client-1.18.1rc3/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_message_defs.py` & `fusion-engine-client-1.18.1rc3/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.18.1rc3/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.18.1rc2/tests/test_time_range.py` & `fusion-engine-client-1.18.1rc3/tests/test_time_range.py`

 * *Files identical despite different names*

