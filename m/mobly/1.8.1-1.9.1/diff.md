# Comparing `tmp/mobly-1.8.1.tar.gz` & `tmp/mobly-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mobly-1.8.1.tar", last modified: Tue Nov  6 01:21:19 2018, max compression
+gzip compressed data, was "dist/mobly-1.9.1.tar", last modified: Mon Aug 12 22:56:51 2019, max compression
```

## Comparing `mobly-1.8.1.tar` & `mobly-1.9.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/
--rw-r--r--   0 angli    (245903) eng       (5000)      341 2018-11-06 01:21:19.000000 mobly-1.8.1/PKG-INFO
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/tools/
--rwxr-xr-x   0 angli    (245903) eng       (5000)     2302 2018-10-11 18:33:40.000000 mobly-1.8.1/tools/sl4a_shell.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     2675 2018-10-03 01:40:16.000000 mobly-1.8.1/tools/snippet_shell.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/mobly/
--rw-r--r--   0 angli    (245903) eng       (5000)     6301 2018-05-17 04:55:02.000000 mobly-1.8.1/mobly/suite_runner.py
--rw-r--r--   0 angli    (245903) eng       (5000)    35942 2018-10-24 17:03:49.000000 mobly-1.8.1/mobly/base_test.py
--rw-r--r--   0 angli    (245903) eng       (5000)     2291 2018-05-17 04:55:02.000000 mobly-1.8.1/mobly/signals.py
--rw-r--r--   0 angli    (245903) eng       (5000)     1967 2018-05-11 19:13:02.000000 mobly-1.8.1/mobly/runtime_test_info.py
--rw-r--r--   0 angli    (245903) eng       (5000)     6836 2018-10-04 06:52:05.000000 mobly-1.8.1/mobly/config_parser.py
--rw-r--r--   0 angli    (245903) eng       (5000)     5039 2018-10-11 18:46:17.000000 mobly-1.8.1/mobly/expects.py
--rw-r--r--   0 angli    (245903) eng       (5000)    22731 2018-10-11 23:25:24.000000 mobly-1.8.1/mobly/records.py
--rw-r--r--   0 angli    (245903) eng       (5000)      575 2017-07-17 19:05:37.000000 mobly-1.8.1/mobly/__init__.py
--rw-r--r--   0 angli    (245903) eng       (5000)     1051 2017-07-17 19:05:37.000000 mobly-1.8.1/mobly/keys.py
--rw-r--r--   0 angli    (245903) eng       (5000)     7054 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/logger.py
--rw-r--r--   0 angli    (245903) eng       (5000)    14301 2018-10-15 20:12:24.000000 mobly-1.8.1/mobly/utils.py
--rw-r--r--   0 angli    (245903) eng       (5000)    12674 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/test_runner.py
--rw-r--r--   0 angli    (245903) eng       (5000)     9153 2018-10-23 00:38:44.000000 mobly-1.8.1/mobly/controller_manager.py
--rw-r--r--   0 angli    (245903) eng       (5000)     9548 2017-10-24 07:03:54.000000 mobly-1.8.1/mobly/asserts.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/mobly/controllers/
--rw-r--r--   0 angli    (245903) eng       (5000)    35909 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device.py
--rw-r--r--   0 angli    (245903) eng       (5000)     4686 2018-06-25 21:31:48.000000 mobly-1.8.1/mobly/controllers/iperf_server.py
--rw-r--r--   0 angli    (245903) eng       (5000)      578 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/__init__.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/mobly/controllers/sniffer_lib/
--rw-r--r--   0 angli    (245903) eng       (5000)      578 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/sniffer_lib/__init__.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/mobly/controllers/sniffer_lib/local/
--rw-r--r--   0 angli    (245903) eng       (5000)     2181 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/sniffer_lib/local/tshark.py
--rw-r--r--   0 angli    (245903) eng       (5000)      578 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/sniffer_lib/local/__init__.py
--rw-r--r--   0 angli    (245903) eng       (5000)     5919 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/sniffer_lib/local/local_base.py
--rw-r--r--   0 angli    (245903) eng       (5000)     1975 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/sniffer_lib/local/tcpdump.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/mobly/controllers/android_device_lib/
--rw-r--r--   0 angli    (245903) eng       (5000)    12057 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/jsonrpc_client_base.py
--rw-r--r--   0 angli    (245903) eng       (5000)     1802 2018-04-05 18:41:13.000000 mobly-1.8.1/mobly/controllers/android_device_lib/snippet_event.py
--rw-r--r--   0 angli    (245903) eng       (5000)     5580 2018-10-24 16:58:42.000000 mobly-1.8.1/mobly/controllers/android_device_lib/service_manager.py
--rw-r--r--   0 angli    (245903) eng       (5000)    15521 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/android_device_lib/event_dispatcher.py
--rw-r--r--   0 angli    (245903) eng       (5000)      578 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/android_device_lib/__init__.py
--rw-r--r--   0 angli    (245903) eng       (5000)     2189 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/android_device_lib/fastboot.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     2774 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/jsonrpc_shell_base.py
--rw-r--r--   0 angli    (245903) eng       (5000)     6525 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/sl4a_client.py
--rw-r--r--   0 angli    (245903) eng       (5000)     6282 2018-10-22 17:58:14.000000 mobly-1.8.1/mobly/controllers/android_device_lib/callback_handler.py
--rw-r--r--   0 angli    (245903) eng       (5000)     1648 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/errors.py
--rw-r--r--   0 angli    (245903) eng       (5000)    14099 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/snippet_client.py
--rw-r--r--   0 angli    (245903) eng       (5000)    15174 2018-10-15 20:12:33.000000 mobly-1.8.1/mobly/controllers/android_device_lib/adb.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/mobly/controllers/android_device_lib/services/
--rw-r--r--   0 angli    (245903) eng       (5000)    10016 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/services/logcat.py
--rw-r--r--   0 angli    (245903) eng       (5000)      575 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/services/__init__.py
--rw-r--r--   0 angli    (245903) eng       (5000)     2069 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/services/sl4a_service.py
--rw-r--r--   0 angli    (245903) eng       (5000)     3200 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/services/base_service.py
--rw-r--r--   0 angli    (245903) eng       (5000)     6082 2018-10-11 18:33:40.000000 mobly-1.8.1/mobly/controllers/android_device_lib/services/snippet_management_service.py
--rw-r--r--   0 angli    (245903) eng       (5000)    31574 2018-06-25 21:31:48.000000 mobly-1.8.1/mobly/controllers/monsoon.py
--rw-r--r--   0 angli    (245903) eng       (5000)     5259 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/attenuator.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/mobly/controllers/attenuator_lib/
--rw-r--r--   0 angli    (245903) eng       (5000)     2696 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/attenuator_lib/telnet_scpi_client.py
--rw-r--r--   0 angli    (245903) eng       (5000)        0 2017-05-12 01:07:14.000000 mobly-1.8.1/mobly/controllers/attenuator_lib/__init__.py
--rw-r--r--   0 angli    (245903) eng       (5000)     5133 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/attenuator_lib/minicircuits.py
--rw-r--r--   0 angli    (245903) eng       (5000)    11590 2018-02-10 00:27:08.000000 mobly-1.8.1/mobly/controllers/sniffer.py
--rw-r--r--   0 angli    (245903) eng       (5000)    36974 2018-10-03 01:08:17.000000 mobly-1.8.1/mobly/base_instrumentation_test.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/tests/
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/tests/mobly/
--rwxr-xr-x   0 angli    (245903) eng       (5000)     2860 2018-10-04 06:52:05.000000 mobly-1.8.1/tests/mobly/test_suite_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)    52916 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/base_instrumentation_test_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     6333 2018-10-15 20:12:24.000000 mobly-1.8.1/tests/mobly/utils_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     1174 2018-02-10 00:27:08.000000 mobly-1.8.1/tests/mobly/asserts_test.py
--rw-r--r--   0 angli    (245903) eng       (5000)        0 2017-05-12 01:07:14.000000 mobly-1.8.1/tests/mobly/__init__.py
--rw-r--r--   0 angli    (245903) eng       (5000)     2392 2018-10-03 01:08:17.000000 mobly-1.8.1/tests/mobly/config_parser_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)    84819 2018-10-22 17:58:33.000000 mobly-1.8.1/tests/mobly/base_test_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)    11933 2018-10-04 06:52:05.000000 mobly-1.8.1/tests/mobly/test_runner_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)    11918 2018-10-23 00:38:44.000000 mobly-1.8.1/tests/mobly/controller_manager_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)      987 2018-04-16 17:07:32.000000 mobly-1.8.1/tests/mobly/logger_test.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/tests/mobly/controllers/
--rw-r--r--   0 angli    (245903) eng       (5000)        0 2017-05-12 01:07:14.000000 mobly-1.8.1/tests/mobly/controllers/__init__.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/
--rwxr-xr-x   0 angli    (245903) eng       (5000)    20921 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/snippet_client_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     1775 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/errors_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     8078 2018-07-19 18:18:30.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/jsonrpc_client_base_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     1379 2018-04-05 18:41:13.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/snippet_event_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     5594 2018-10-04 06:52:05.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/callback_handler_test.py
--rw-r--r--   0 angli    (245903) eng       (5000)        0 2017-05-12 01:07:14.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/__init__.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)    28062 2018-10-15 20:12:33.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/adb_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     7796 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/service_manager_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     4080 2018-04-16 17:07:32.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/sl4a_client_test.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/services/
--rwxr-xr-x   0 angli    (245903) eng       (5000)    21890 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/services/logcat_test.py
--rw-r--r--   0 angli    (245903) eng       (5000)        0 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/services/__init__.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     7625 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/services/snippet_management_service_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     2642 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/controllers/android_device_lib/services/sl4a_service_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)    34235 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/controllers/android_device_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)      985 2018-08-16 22:13:14.000000 mobly-1.8.1/tests/mobly/controllers/monsoon_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)    16770 2018-10-04 06:52:05.000000 mobly-1.8.1/tests/mobly/records_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     2820 2018-05-15 02:12:13.000000 mobly-1.8.1/tests/mobly/suite_runner_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)    10875 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/mobly/output_test.py
--rw-r--r--   0 angli    (245903) eng       (5000)        0 2017-05-12 01:07:14.000000 mobly-1.8.1/tests/__init__.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/tests/lib/
--rwxr-xr-x   0 angli    (245903) eng       (5000)      887 2017-05-12 01:07:14.000000 mobly-1.8.1/tests/lib/integration2_test.py
--rw-r--r--   0 angli    (245903) eng       (5000)     1928 2018-10-11 18:33:40.000000 mobly-1.8.1/tests/lib/mock_instrumentation_test.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     1018 2018-04-05 18:41:13.000000 mobly-1.8.1/tests/lib/integration3_test.py
--rw-r--r--   0 angli    (245903) eng       (5000)     1632 2018-10-04 06:52:05.000000 mobly-1.8.1/tests/lib/mock_second_controller.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)      940 2018-02-09 03:05:04.000000 mobly-1.8.1/tests/lib/teardown_class_failure_test.py
--rw-r--r--   0 angli    (245903) eng       (5000)        0 2017-05-12 01:07:14.000000 mobly-1.8.1/tests/lib/__init__.py
--rw-r--r--   0 angli    (245903) eng       (5000)     1308 2018-10-18 02:29:55.000000 mobly-1.8.1/tests/lib/mock_controller.py
--rw-r--r--   0 angli    (245903) eng       (5000)     1505 2017-08-21 19:00:11.000000 mobly-1.8.1/tests/lib/utils.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     2402 2018-02-10 00:27:08.000000 mobly-1.8.1/tests/lib/jsonrpc_client_test_base.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     3767 2018-02-10 00:27:08.000000 mobly-1.8.1/tests/lib/mock_android_device.py
--rwxr-xr-x   0 angli    (245903) eng       (5000)     1379 2018-03-26 22:54:36.000000 mobly-1.8.1/tests/lib/integration_test.py
-drwxr-xr-x   0 angli    (245903) eng       (5000)        0 2018-11-06 01:21:19.000000 mobly-1.8.1/mobly.egg-info/
--rw-r--r--   0 angli    (245903) eng       (5000)      341 2018-11-06 01:21:18.000000 mobly-1.8.1/mobly.egg-info/PKG-INFO
--rw-r--r--   0 angli    (245903) eng       (5000)     3800 2018-11-06 01:21:18.000000 mobly-1.8.1/mobly.egg-info/SOURCES.txt
--rw-r--r--   0 angli    (245903) eng       (5000)       81 2018-11-06 01:21:18.000000 mobly-1.8.1/mobly.egg-info/requires.txt
--rw-r--r--   0 angli    (245903) eng       (5000)       12 2018-11-06 01:21:18.000000 mobly-1.8.1/mobly.egg-info/top_level.txt
--rw-r--r--   0 angli    (245903) eng       (5000)        1 2018-11-06 01:21:18.000000 mobly-1.8.1/mobly.egg-info/dependency_links.txt
--rw-r--r--   0 angli    (245903) eng       (5000)     2889 2018-10-11 18:33:40.000000 mobly-1.8.1/README.md
--rwxr-xr-x   0 angli    (245903) eng       (5000)     2228 2018-11-06 01:20:34.000000 mobly-1.8.1/setup.py
--rw-r--r--   0 angli    (245903) eng       (5000)      166 2018-11-06 01:21:19.000000 mobly-1.8.1/setup.cfg
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)      333 2019-08-12 22:56:51.000000 mobly-1.9.1/PKG-INFO
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/tools/
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     2302 2019-06-07 18:19:21.000000 mobly-1.9.1/tools/sl4a_shell.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     2675 2019-06-07 18:19:21.000000 mobly-1.9.1/tools/snippet_shell.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     6475 2019-07-31 22:26:39.000000 mobly-1.9.1/mobly/suite_runner.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    36077 2019-08-07 23:15:51.000000 mobly-1.9.1/mobly/base_test.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     2292 2019-07-17 23:44:01.000000 mobly-1.9.1/mobly/signals.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     1967 2019-06-07 18:19:21.000000 mobly-1.9.1/mobly/runtime_test_info.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     6816 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/config_parser.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     5567 2019-07-17 23:44:01.000000 mobly-1.9.1/mobly/expects.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    23661 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/records.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)      575 2019-06-07 18:19:21.000000 mobly-1.9.1/mobly/__init__.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     1051 2019-06-07 18:19:21.000000 mobly-1.9.1/mobly/keys.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     7473 2019-08-04 07:55:57.000000 mobly-1.9.1/mobly/logger.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    18187 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/utils.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    12878 2019-08-07 23:15:51.000000 mobly-1.9.1/mobly/test_runner.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     9160 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controller_manager.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     9447 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/asserts.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly/controllers/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    37872 2019-07-30 01:16:18.000000 mobly-1.9.1/mobly/controllers/android_device.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     4686 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/iperf_server.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)      575 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/__init__.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly/controllers/sniffer_lib/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)      575 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/sniffer_lib/__init__.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly/controllers/sniffer_lib/local/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     2231 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/sniffer_lib/local/tshark.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)      575 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/sniffer_lib/local/__init__.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     5963 2019-07-23 01:42:35.000000 mobly-1.9.1/mobly/controllers/sniffer_lib/local/local_base.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     2011 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/sniffer_lib/local/tcpdump.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly/controllers/android_device_lib/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    12613 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/android_device_lib/jsonrpc_client_base.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     1841 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/android_device_lib/snippet_event.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     6306 2019-07-30 01:16:18.000000 mobly-1.9.1/mobly/controllers/android_device_lib/service_manager.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    15518 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/android_device_lib/event_dispatcher.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)      575 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/android_device_lib/__init__.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     2186 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/android_device_lib/fastboot.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     3085 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/android_device_lib/jsonrpc_shell_base.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     6501 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/android_device_lib/sl4a_client.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     6267 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/android_device_lib/callback_handler.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     1648 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/android_device_lib/errors.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    14794 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/android_device_lib/snippet_client.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    17740 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/android_device_lib/adb.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly/controllers/android_device_lib/services/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    10754 2019-07-31 22:26:39.000000 mobly-1.9.1/mobly/controllers/android_device_lib/services/logcat.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)      575 2019-06-07 18:19:21.000000 mobly-1.9.1/mobly/controllers/android_device_lib/services/__init__.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     2070 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/android_device_lib/services/sl4a_service.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     3200 2019-06-07 18:19:21.000000 mobly-1.9.1/mobly/controllers/android_device_lib/services/base_service.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     6082 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/android_device_lib/services/snippet_management_service.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    31655 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/monsoon.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     5256 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/attenuator.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly/controllers/attenuator_lib/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     2694 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/controllers/attenuator_lib/telnet_scpi_client.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)        0 2019-06-07 18:19:21.000000 mobly-1.9.1/mobly/controllers/attenuator_lib/__init__.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     5130 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/attenuator_lib/minicircuits.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    11584 2019-07-23 01:12:52.000000 mobly-1.9.1/mobly/controllers/sniffer.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)    37920 2019-07-23 18:54:14.000000 mobly-1.9.1/mobly/base_instrumentation_test.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/tests/
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/tests/mobly/
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     2903 2019-07-31 22:26:39.000000 mobly-1.9.1/tests/mobly/test_suite_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    52916 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/base_instrumentation_test_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     9092 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/utils_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     1174 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/asserts_test.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)        0 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/__init__.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     2392 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/config_parser_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    87562 2019-07-17 23:44:01.000000 mobly-1.9.1/tests/mobly/base_test_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    15075 2019-08-06 23:45:33.000000 mobly-1.9.1/tests/mobly/test_runner_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    11918 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controller_manager_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     3016 2019-08-04 07:55:57.000000 mobly-1.9.1/tests/mobly/logger_test.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/tests/mobly/controllers/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)        0 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/__init__.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    20949 2019-07-17 23:44:01.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/snippet_client_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     1775 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/errors_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     8083 2019-07-17 23:44:01.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/jsonrpc_client_base_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     1379 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/snippet_event_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     5594 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/callback_handler_test.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)        0 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/__init__.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    32690 2019-07-17 23:44:01.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/adb_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    15686 2019-07-30 01:16:18.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/service_manager_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     3554 2019-07-17 23:44:01.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/sl4a_client_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     4155 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/jsonrpc_shell_base_test.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/services/
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    26378 2019-07-31 22:26:39.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/services/logcat_test.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)        0 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/services/__init__.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     7625 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/services/snippet_management_service_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     2642 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/android_device_lib/services/sl4a_service_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    51122 2019-07-30 01:16:18.000000 mobly-1.9.1/tests/mobly/controllers/android_device_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)      985 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/controllers/monsoon_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    17014 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/mobly/records_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     4441 2019-07-31 22:26:39.000000 mobly-1.9.1/tests/mobly/suite_runner_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)    13616 2019-08-04 07:55:57.000000 mobly-1.9.1/tests/mobly/output_test.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/tests/lib/
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)      887 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/integration2_test.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     1928 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/mock_instrumentation_test.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     1018 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/integration3_test.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     1632 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/mock_second_controller.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)      940 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/teardown_class_failure_test.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)        0 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/__init__.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     1308 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/mock_controller.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     1505 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/utils.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     2402 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/jsonrpc_client_test_base.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     5321 2019-07-17 23:44:01.000000 mobly-1.9.1/tests/lib/mock_android_device.py
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     1379 2019-06-07 18:19:21.000000 mobly-1.9.1/tests/lib/integration_test.py
+drwxr-xr-x   0 angli    (245903) primarygroup (89939)        0 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly.egg-info/
+-rw-r--r--   0 angli    (245903) primarygroup (89939)      333 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly.egg-info/PKG-INFO
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     3852 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly.egg-info/SOURCES.txt
+-rw-r--r--   0 angli    (245903) primarygroup (89939)       81 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly.egg-info/requires.txt
+-rw-r--r--   0 angli    (245903) primarygroup (89939)       12 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly.egg-info/top_level.txt
+-rw-r--r--   0 angli    (245903) primarygroup (89939)        1 2019-08-12 22:56:51.000000 mobly-1.9.1/mobly.egg-info/dependency_links.txt
+-rw-r--r--   0 angli    (245903) primarygroup (89939)     3037 2019-06-07 18:19:21.000000 mobly-1.9.1/README.md
+-rwxr-xr-x   0 angli    (245903) primarygroup (89939)     2346 2019-08-12 22:56:32.000000 mobly-1.9.1/setup.py
+-rw-r--r--   0 angli    (245903) primarygroup (89939)      187 2019-08-12 22:56:51.000000 mobly-1.9.1/setup.cfg
```

### Comparing `mobly-1.8.1/tools/sl4a_shell.py` & `mobly-1.9.1/tools/sl4a_shell.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tools/snippet_shell.py` & `mobly-1.9.1/tools/snippet_shell.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly/suite_runner.py` & `mobly-1.9.1/mobly/suite_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,22 +51,21 @@
     Args:
         test_classes: List of python classes containing Mobly tests.
         argv: A list that is then parsed as cli args. If None, defaults to cli
             input.
     """
     # Parse cli args.
     parser = argparse.ArgumentParser(description='Mobly Suite Executable.')
-    parser.add_argument(
-        '-c',
-        '--config',
-        nargs=1,
-        type=str,
-        required=True,
-        metavar='<PATH>',
-        help='Path to the test configuration file.')
+    parser.add_argument('-c',
+                        '--config',
+                        nargs=1,
+                        type=str,
+                        required=True,
+                        metavar='<PATH>',
+                        help='Path to the test configuration file.')
     parser.add_argument(
         '--tests',
         '--test_case',
         nargs='+',
         type=str,
         metavar='[ClassA[.test_a] ClassB[.test_b] ...]',
         help='A list of test classes and optional tests to execute.')
@@ -75,36 +74,38 @@
     args = parser.parse_args(argv)
     # Load test config file.
     test_configs = config_parser.load_test_config_file(args.config[0])
 
     # Check the classes that were passed in
     for test_class in test_classes:
         if not issubclass(test_class, base_test.BaseTestClass):
-            logging.error('Test class %s does not extend '
-                          'mobly.base_test.BaseTestClass', test_class)
+            logging.error(
+                'Test class %s does not extend '
+                'mobly.base_test.BaseTestClass', test_class)
             sys.exit(1)
 
     # Find the full list of tests to execute
     selected_tests = compute_selected_tests(test_classes, args.tests)
 
     # Execute the suite
     ok = True
     for config in test_configs:
         runner = test_runner.TestRunner(config.log_path, config.test_bed_name)
-        for (test_class, tests) in selected_tests.items():
-            runner.add_test_class(config, test_class, tests)
-        try:
-            runner.run()
-            ok = runner.results.is_all_pass and ok
-        except signals.TestAbortAll:
-            pass
-        except:
-            logging.exception('Exception when executing %s.',
-                              config.test_bed_name)
-            ok = False
+        with runner.mobly_logger():
+            for (test_class, tests) in selected_tests.items():
+                runner.add_test_class(config, test_class, tests)
+            try:
+                runner.run()
+                ok = runner.results.is_all_pass and ok
+            except signals.TestAbortAll:
+                pass
+            except:
+                logging.exception('Exception when executing %s.',
+                                  config.test_bed_name)
+                ok = False
     if not ok:
         sys.exit(1)
 
 
 def compute_selected_tests(test_classes, selected_tests):
     """Computes tests to run for each class from selector strings.
```

### Comparing `mobly-1.8.1/mobly/base_test.py` & `mobly-1.9.1/mobly/base_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 STAGE_NAME_SETUP_TEST = 'setup_test'
 STAGE_NAME_TEARDOWN_TEST = 'teardown_test'
 STAGE_NAME_TEARDOWN_CLASS = 'teardown_class'
 STAGE_NAME_CLEAN_UP = 'clean_up'
 
 
 class Error(Exception):
-    """Raised for exceptions that occured in BaseTestClass."""
+    """Raised for exceptions that occurred in BaseTestClass."""
 
 
 class BaseTestClass(object):
     """Base class for all test classes to inherit from.
 
     This class gets all the controller objects from test_runner and executes
     the tests requested within itself.
@@ -110,20 +110,14 @@
         # Deprecated, use `self.current_test_info.name`.
         self.current_test_name = None
         self._generated_test_table = collections.OrderedDict()
         self._controller_manager = controller_manager.ControllerManager(
             class_name=self.TAG, controller_configs=configs.controller_configs)
         self.controller_configs = self._controller_manager.controller_configs
 
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *args):
-        self._safe_exec_func(self.clean_up)
-
     def unpack_userparams(self,
                           req_param_names=None,
                           opt_param_names=None,
                           **kwargs):
         """An optional function that unpacks user defined parameters into
         individual variables.
 
@@ -165,16 +159,17 @@
             setattr(self, name, self.user_params[name])
         for name in opt_param_names:
             if hasattr(self, name):
                 continue
             if name in self.user_params:
                 setattr(self, name, self.user_params[name])
             else:
-                logging.warning('Missing optional user param "%s" in '
-                                'configuration, continue.', name)
+                logging.warning(
+                    'Missing optional user param "%s" in '
+                    'configuration, continue.', name)
 
     def register_controller(self, module, required=True, min_number=1):
         """Loads a controller module and returns its loaded devices.
 
         A Mobly controller module is a Python lib that can be used to control
         a device, service, or equipment. To be Mobly compatible, a controller
         module needs to have the following members:
@@ -399,20 +394,20 @@
         parent_token = self.current_test_info.name
         # If the name of the stage is the same as the test name, in which case
         # the stage is class-level instead of test-level, use the class's
         # reference tag as the parent token instead.
         if parent_token == stage_name:
             parent_token = self.TAG
         logging.debug(
-            TEST_STAGE_BEGIN_LOG_TEMPLATE.format(
-                parent_token=parent_token, child_token=stage_name))
+            TEST_STAGE_BEGIN_LOG_TEMPLATE.format(parent_token=parent_token,
+                                                 child_token=stage_name))
         yield
         logging.debug(
-            TEST_STAGE_END_LOG_TEMPLATE.format(
-                parent_token=parent_token, child_token=stage_name))
+            TEST_STAGE_END_LOG_TEMPLATE.format(parent_token=parent_token,
+                                               child_token=stage_name))
 
     def _setup_test(self, test_name):
         """Proxy function to guarantee the base implementation of setup_test is
         called.
         """
         self.current_test_name = test_name
         with self._log_test_stage(STAGE_NAME_SETUP_TEST):
@@ -559,47 +554,43 @@
             content: dict, the data to add to summary file.
         """
         if 'timestamp' not in content:
             content['timestamp'] = utils.get_current_epoch_time()
         self.summary_writer.dump(content,
                                  records.TestSummaryEntryType.USER_DATA)
 
-    def exec_one_test(self, test_name, test_method, args=(), **kwargs):
+    def exec_one_test(self, test_name, test_method):
         """Executes one test and update test results.
 
         Executes setup_test, the test method, and teardown_test; then creates a
         records.TestResultRecord object with the execution information and adds
         the record to the test class's test results.
 
         Args:
-            test_name: Name of the test.
-            test_method: The test method.
-            args: A tuple of params.
-            kwargs: Extra kwargs.
+            test_name: string, Name of the test.
+            test_method: function, The test method to execute.
         """
         tr_record = records.TestResultRecord(test_name, self.TAG)
+        tr_record.uid = getattr(test_method, 'uid', None)
         tr_record.test_begin()
         self.current_test_info = runtime_test_info.RuntimeTestInfo(
             test_name, self.log_path, tr_record)
         expects.recorder.reset_internal_states(tr_record)
         logging.info('%s %s', TEST_CASE_TOKEN, test_name)
         # Did teardown_test throw an error.
         teardown_test_failed = False
         try:
             try:
                 try:
                     self._setup_test(test_name)
                 except signals.TestFailure as e:
-                    raise_with_traceback(
-                        signals.TestError(e.details, e.extras))
-                if args or kwargs:
-                    test_method(*args, **kwargs)
-                else:
-                    test_method()
-            except signals.TestPass:
+                    raise_with_traceback(signals.TestError(
+                        e.details, e.extras))
+                test_method()
+            except (signals.TestPass, signals.TestAbortSignal):
                 raise
             except Exception:
                 logging.exception('Exception occurred in %s.',
                                   self.current_test_name)
                 raise
             finally:
                 before_count = expects.recorder.error_count
@@ -620,15 +611,15 @@
             tr_record.test_fail(e)
         except signals.TestSkip as e:
             # Test skipped.
             tr_record.test_skip(e)
         except signals.TestAbortSignal as e:
             # Abort signals, pass along.
             tr_record.test_fail(e)
-            raise e
+            raise
         except signals.TestPass as e:
             # Explicit test pass.
             tr_record.test_pass(e)
         except Exception as e:
             # Exception happened during test.
             tr_record.test_error(e)
         else:
@@ -665,41 +656,55 @@
         caller_frames = inspect.getouterframes(current_frame, 2)
         for caller_frame in caller_frames[2:]:
             if caller_frame[3] == expected_func_name:
                 return
         raise Error('"%s" cannot be called outside of %s' %
                     (caller_frames[1][3], expected_func_name))
 
-    def generate_tests(self, test_logic, name_func, arg_sets):
+    def generate_tests(self, test_logic, name_func, arg_sets, uid_func=None):
         """Generates tests in the test class.
 
         This function has to be called inside a test class's
         `self.setup_generated_tests` function.
 
         Generated tests are not written down as methods, but as a list of
         parameter sets. This way we reduce code repetition and improve test
         scalability.
 
+        Users can provide an optional function to specify the UID of each test.
+        Not all generated tests are required to have UID.
+
         Args:
             test_logic: function, the common logic shared by all the generated
                 tests.
             name_func: function, generate a test name according to a set of
                 test arguments. This function should take the same arguments as
                 the test logic function.
             arg_sets: a list of tuples, each tuple is a set of arguments to be
                 passed to the test logic function and name function.
+            uid_func: function, an optional function that takes the same
+                arguments as the test logic function and returns a string that
+                is the corresponding UID.
         """
         self._assert_function_name_in_stack(STAGE_NAME_SETUP_GENERATED_TESTS)
+        root_msg = 'During test generation of "%s":' % test_logic.__name__
         for args in arg_sets:
             test_name = name_func(*args)
             if test_name in self.get_existing_test_names():
                 raise Error(
-                    'Test name "%s" already exists, cannot be duplicated!' %
-                    test_name)
+                    '%s Test name "%s" already exists, cannot be duplicated!' %
+                    (root_msg, test_name))
             test_func = functools.partial(test_logic, *args)
+            if uid_func is not None:
+                uid = uid_func(*args)
+                if uid is None:
+                    logging.warning('%s UID for arg set %s is None.', root_msg,
+                                    args)
+                else:
+                    setattr(test_func, 'uid', uid)
             self._generated_test_table[test_name] = test_func
 
     def _safe_exec_func(self, func, *args):
         """Executes a function with exception safeguard.
 
         This will let signals.TestAbortAll through so abort_all works in all
         procedure functions.
@@ -758,16 +763,16 @@
                 raise Error('Test method name %s does not follow naming '
                             'convention test_*, abort.' % test_name)
             if hasattr(self, test_name):
                 test_method = getattr(self, test_name)
             elif test_name in self._generated_test_table:
                 test_method = self._generated_test_table[test_name]
             else:
-                raise Error('%s does not have test method %s.' % (self.TAG,
-                                                                  test_name))
+                raise Error('%s does not have test method %s.' %
+                            (self.TAG, test_name))
             test_methods.append((test_name, test_method))
         return test_methods
 
     def _skip_remaining_tests(self, exception):
         """Marks any requested test that has not been executed in a class as
         skipped.
 
@@ -859,22 +864,7 @@
             self._controller_manager.unregister_controllers()
             if expects.recorder.has_error:
                 record.test_error()
                 record.update_record()
                 self.results.add_class_error(record)
                 self.summary_writer.dump(record.to_dict(),
                                          records.TestSummaryEntryType.RECORD)
-
-    def clean_up(self):
-        """.. deprecated:: 1.8.1
-
-        Use `teardown_class` instead.
-
-        A function that is executed upon completion of all tests selected in
-        the test class.
-
-        This function should clean up objects initialized in the constructor by
-        user.
-
-        Generally this should not be used as nothing should be instantiated
-        from the constructor of a test class.
-        """
```

### Comparing `mobly-1.8.1/mobly/signals.py` & `mobly-1.9.1/mobly/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,8 +73,8 @@
 
 
 class TestAbortAll(TestAbortSignal):
     """Raised when all subsequent tests should be aborted."""
 
 
 class ControllerError(Exception):
-    """Raised when an error occured in controller classes."""
+    """Raised when an error occurred in controller classes."""
```

### Comparing `mobly-1.8.1/mobly/runtime_test_info.py` & `mobly-1.9.1/mobly/runtime_test_info.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly/config_parser.py` & `mobly-1.9.1/mobly/config_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 def _validate_test_config(test_config):
     """Validates the raw configuration loaded from the config file.
 
     Making sure the required key 'TestBeds' is present.
     """
     required_key = keys.Config.key_testbed.value
     if required_key not in test_config:
-        raise MoblyConfigError(
-            'Required key %s missing in test config.' % required_key)
+        raise MoblyConfigError('Required key %s missing in test config.' %
+                               required_key)
 
 
 def _validate_testbed_name(name):
     """Validates the name of a test bed.
 
     Since test bed names are used as part of the test run id, it needs to meet
     certain requirements.
@@ -107,16 +107,16 @@
         tbs = []
         for tb in configs[keys.Config.key_testbed.value]:
             if tb[keys.Config.key_testbed_name.value] in tb_filters:
                 tbs.append(tb)
         if len(tbs) != len(tb_filters):
             raise MoblyConfigError(
                 'Expect to find %d test bed configs, found %d. Check if'
-                ' you have the correct test bed names.' % (len(tb_filters),
-                                                           len(tbs)))
+                ' you have the correct test bed names.' %
+                (len(tb_filters), len(tbs)))
         configs[keys.Config.key_testbed.value] = tbs
     mobly_params = configs.get(keys.Config.key_mobly_params.value, {})
     # Decide log path.
     log_path = mobly_params.get(keys.Config.key_log_path.value,
                                 _DEFAULT_LOG_PATH)
     if ENV_MOBLY_LOGPATH in os.environ:
         log_path = os.environ[ENV_MOBLY_LOGPATH]
@@ -148,15 +148,15 @@
         path: A string that is the full path to the config file, including the
             file name.
 
     Returns:
         A dict that represents info in the config file.
     """
     with io.open(utils.abs_path(path), 'r', encoding='utf-8') as f:
-        conf = yaml.load(f)
+        conf = yaml.safe_load(f)
         return conf
 
 
 class TestRunConfig(object):
     """The data class that holds all the information needed for a test run.
 
     Attributes:
```

### Comparing `mobly-1.8.1/mobly/expects.py` & `mobly-1.9.1/mobly/expects.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,32 @@
 import logging
 import time
 
 from mobly import asserts
 from mobly import records
 from mobly import signals
 
+# When used outside of a `base_test.BaseTestClass` context, such as when using
+# the `android_device` controller directly, the `expects.recorder`
+# `TestResultRecord` isn't set, which causes `expects` module methods to fail
+# from the missing record, so this provides a default, globally accessible
+# record for `expects` module to use as well as providing a way to get the
+# globally recorded errors.
+DEFAULT_TEST_RESULT_RECORD = records.TestResultRecord('mobly', 'global')
+
 
 class _ExpectErrorRecorder(object):
     """Singleton used to store errors caught via `expect_*` functions in test.
 
     This class is only instantiated once as a singleton. It holds a reference
     to the record object for the test currently executing.
     """
 
-    def __init__(self):
-        self.reset_internal_states()
+    def __init__(self, record=None):
+        self.reset_internal_states(record=record)
 
     def reset_internal_states(self, record=None):
         """Resets the internal state of the recorder.
 
         Args:
             record: records.TestResultRecord, the test record for a test.
         """
@@ -150,8 +158,8 @@
         msg = message or 'Got an unexpected exception'
         details = '%s: %s' % (msg, e_record.details)
         logging.exception(details)
         e_record.details = details
         recorder.add_error(e_record)
 
 
-recorder = _ExpectErrorRecorder()
+recorder = _ExpectErrorRecorder(DEFAULT_TEST_RESULT_RECORD)
```

### Comparing `mobly-1.8.1/mobly/records.py` & `mobly-1.9.1/mobly/records.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 """This module has classes for test result collection, and test result output.
 """
 
 import collections
 import copy
 import enum
+import functools
 import io
 import logging
 import sys
 import threading
 import time
 import traceback
 import yaml
@@ -30,14 +31,46 @@
 
 # File names for the output files.
 OUTPUT_FILE_INFO_LOG = 'test_log.INFO'
 OUTPUT_FILE_DEBUG_LOG = 'test_log.DEBUG'
 OUTPUT_FILE_SUMMARY = 'test_summary.yaml'
 
 
+class Error(Exception):
+    """Raised for errors in record module members."""
+
+
+def uid(uid):
+    """Decorator specifying the unique identifier (UID) of a test case.
+
+    The UID will be recorded in the test's record when executed by Mobly.
+
+    If you use any other decorator for the test method, you may want to use
+    this as the outer-most one.
+
+    Note a common UID system is the Universal Unitque Identifier (UUID), but
+    we are not limiting people to use UUID, hence the more generic name `UID`.
+
+    Args:
+        uid: string, the uid for the decorated test function.
+    """
+    if uid is None:
+        raise ValueError('UID cannot be None.')
+
+    def decorate(test_func):
+        @functools.wraps(test_func)
+        def wrapper(*args, **kwargs):
+            return test_func(*args, **kwargs)
+
+        setattr(wrapper, 'uid', uid)
+        return wrapper
+
+    return decorate
+
+
 class TestSummaryEntryType(enum.Enum):
     """Constants used to identify the type of entries in test summary file.
 
     Test summary file contains multiple yaml documents. In order to parse this
     file efficiently, the write adds the type of each entry when it writes the
     entry to the file.
 
@@ -120,20 +153,19 @@
             # For Python3, setting the encoding on yaml.safe_dump does not work
             # because Python3 file descriptors set an encoding by default, which
             # PyYAML uses instead of the encoding on yaml.safe_dump. So, the
             # encoding has to be set on the open call instead.
             with io.open(self._path, 'a', encoding='utf-8') as f:
                 # Use safe_dump here to avoid language-specific tags in final
                 # output.
-                yaml.safe_dump(
-                    new_content,
-                    f,
-                    explicit_start=True,
-                    allow_unicode=True,
-                    indent=4)
+                yaml.safe_dump(new_content,
+                               f,
+                               explicit_start=True,
+                               allow_unicode=True,
+                               indent=4)
 
 
 class TestResultEnums(object):
     """Enums used for TestResultRecord class.
 
     Includes the tokens to mark test result with, and the string names for each
     field in TestResultRecord.
```

### Comparing `mobly-1.8.1/mobly/__init__.py` & `mobly-1.9.1/mobly/__init__.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly/keys.py` & `mobly-1.9.1/mobly/keys.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly/logger.py` & `mobly-1.9.1/mobly/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 log_line_format = '%(asctime)s.%(msecs).03d %(levelname)s %(message)s'
 # The micro seconds are added by the format string above,
 # so the time format does not include ms.
 log_line_time_format = '%m-%d %H:%M:%S'
 log_line_timestamp_len = 18
 
-logline_timestamp_re = re.compile('\d\d-\d\d \d\d:\d\d:\d\d.\d\d\d')
+logline_timestamp_re = re.compile(r'\d\d-\d\d \d\d:\d\d:\d\d.\d\d\d')
 
 
 def _parse_logline_timestamp(t):
     """Parses a logline timestamp into a tuple.
 
     Args:
         t: Timestamp in logline format.
@@ -183,37 +183,44 @@
     """
     for h in list(logger.handlers):
         logger.removeHandler(h)
         if isinstance(h, logging.FileHandler):
             h.close()
 
 
-def create_latest_log_alias(actual_path):
+def create_latest_log_alias(actual_path, alias):
     """Creates a symlink to the latest test run logs.
 
     Args:
-        actual_path: The source directory where the latest test run's logs are.
+        actual_path: string, the source directory where the latest test run's
+            logs are.
+        alias: string, the name of the directory to contain the latest log
+            files.
     """
-    alias_path = os.path.join(os.path.dirname(actual_path), 'latest')
+    alias_path = os.path.join(os.path.dirname(actual_path), alias)
     utils.create_alias(actual_path, alias_path)
 
 
-def setup_test_logger(log_path, prefix=None, filename=None):
+def setup_test_logger(log_path, prefix=None, alias='latest'):
     """Customizes the root logger for a test run.
 
     Args:
-        log_path: Location of the report file.
-        prefix: A prefix for each log line in terminal.
-        filename: Name of the files. The default is the time the objects
-            are requested.
+        log_path: string, the location of the report file.
+        prefix: optional string, a prefix for each log line in terminal.
+        alias: optional string, The name of the alias to use for the latest log
+            directory. If a falsy value is provided, then the alias directory
+            will not be created, which is useful to save storage space when the
+            storage system (e.g. ZIP files) does not properly support
+            shortcut/symlinks.
     """
     utils.create_dir(log_path)
     _setup_test_logger(log_path, prefix)
     logging.info('Test output folder: "%s"', log_path)
-    create_latest_log_alias(log_path)
+    if alias:
+        create_latest_log_alias(log_path, alias=alias)
 
 
 def normalize_log_line_timestamp(log_line_timestamp):
     """Replace special characters in log line timestamp with normal characters.
 
     Args:
         log_line_timestamp: A string in the log line timestamp format. Obtained
```

### Comparing `mobly-1.8.1/mobly/utils.py` & `mobly-1.9.1/mobly/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from past.builtins import basestring
+
 import base64
 import concurrent.futures
 import datetime
 import io
 import logging
 import os
+import pipes
 import platform
 import portpicker
 import random
 import re
 import signal
 import string
 import subprocess
+import threading
 import time
 import traceback
 
 # File name length is limited to 255 chars on some OS, so we need to make sure
 # the file names we output fits within the limit.
 MAX_FILENAME_LEN = 255
 # Number of times to retry to get available port
@@ -279,14 +283,91 @@
             except Exception as exc:
                 logging.exception("{} generated an exception: {}".format(
                     params, traceback.format_exc()))
                 return_vals.append(exc)
         return return_vals
 
 
+def run_command(cmd,
+                stdout=None,
+                stderr=None,
+                shell=False,
+                timeout=None,
+                cwd=None,
+                env=None):
+    """Runs a command in a subprocess.
+
+    This function is very similar to subprocess.check_output. The main
+    difference is that it returns the return code and std error output as well
+    as supporting a timeout parameter.
+
+    Args:
+        cmd: string or list of strings, the command to run.
+            See subprocess.Popen() documentation.
+        stdout: file handle, the file handle to write std out to. If None is
+            given, then subprocess.PIPE is used. See subprocess.Popen()
+            documentation.
+        stdee: file handle, the file handle to write std err to. If None is
+            given, then subprocess.PIPE is used. See subprocess.Popen()
+            documentation.
+        shell: bool, True to run this command through the system shell,
+            False to invoke it directly. See subprocess.Popen() docs.
+        timeout: float, the number of seconds to wait before timing out.
+            If not specified, no timeout takes effect.
+        cwd: string, the path to change the child's current directory to before
+            it is executed. Note that this directory is not considered when
+            searching the executable, so you can't specify the program's path
+            relative to cwd.
+        env: dict, a mapping that defines the environment variables for the
+            new process. Default behavior is inheriting the current process'
+            environment.
+
+    Returns:
+        A 3-tuple of the consisting of the return code, the std output, and the
+            std error.
+
+    Raises:
+        psutil.TimeoutExpired: The command timed out.
+    """
+    # Only import psutil when actually needed.
+    # psutil may cause import error in certain env. This way the utils module
+    # doesn't crash upon import.
+    import psutil
+    if stdout is None:
+        stdout = subprocess.PIPE
+    if stderr is None:
+        stderr = subprocess.PIPE
+    process = psutil.Popen(cmd,
+                           stdout=stdout,
+                           stderr=stderr,
+                           shell=shell,
+                           cwd=cwd,
+                           env=env)
+    timer = None
+    timer_triggered = threading.Event()
+    if timeout and timeout > 0:
+        # The wait method on process will hang when used with PIPEs with large
+        # outputs, so use a timer thread instead.
+
+        def timeout_expired():
+            timer_triggered.set()
+            process.terminate()
+
+        timer = threading.Timer(timeout, timeout_expired)
+        timer.start()
+    # If the command takes longer than the timeout, then the timer thread
+    # will kill the subprocess, which will make it terminate.
+    (out, err) = process.communicate()
+    if timer is not None:
+        timer.cancel()
+    if timer_triggered.is_set():
+        raise psutil.TimeoutExpired(timeout, pid=process.pid)
+    return (process.returncode, out, err)
+
+
 def start_standing_subprocess(cmd, shell=False, env=None):
     """Starts a long-running subprocess.
 
     This is not a blocking call and the subprocess started by it should be
     explicitly terminated with stop_standing_subprocess.
 
     For short-running commands, you should use subprocess.check_call, which
@@ -300,21 +381,20 @@
             specified, inherits the current environment. See subprocess.Popen()
             docs.
 
     Returns:
         The subprocess that was started.
     """
     logging.debug('Starting standing subprocess with: %s', cmd)
-    proc = subprocess.Popen(
-        cmd,
-        stdin=subprocess.PIPE,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        shell=shell,
-        env=env)
+    proc = subprocess.Popen(cmd,
+                            stdin=subprocess.PIPE,
+                            stdout=subprocess.PIPE,
+                            stderr=subprocess.PIPE,
+                            shell=shell,
+                            env=env)
     # Leaving stdin open causes problems for input, e.g. breaking the
     # code.inspect() shell (http://stackoverflow.com/a/25512460/1612937), so
     # explicitly close it assuming it is not needed for standing subprocesses.
     proc.stdin.close()
     proc.stdin = None
     logging.debug('Started standing subprocess %d', proc.pid)
     return proc
@@ -381,24 +461,30 @@
 
 def wait_for_standing_subprocess(proc, timeout=None):
     """Waits for a subprocess started by start_standing_subprocess to finish
     or times out.
 
     Propagates the exception raised by the subprocess.wait(.) function.
     The subprocess.TimeoutExpired exception is raised if the process timed-out
-    rather then terminating.
+    rather than terminating.
 
     If no exception is raised: the subprocess terminated on its own. No need
     to call stop_standing_subprocess() to kill it.
 
     If an exception is raised: the subprocess is still alive - it did not
     terminate. Either call stop_standing_subprocess() to kill it, or call
     wait_for_standing_subprocess() to keep waiting for it to terminate on its
     own.
 
+    If the corresponding subprocess command generates a large amount of output
+    and this method is called with a timeout value, then the command can hang
+    indefinitely. See http://go/pylib/subprocess.html#subprocess.Popen.wait
+
+    This function does not support Python 2.
+
     Args:
         p: Subprocess to wait for.
         timeout: An integer number of seconds to wait before timing out.
     """
     proc.wait(timeout)
 
 
@@ -441,7 +527,22 @@
     """
     lines = output.decode('utf-8').strip().splitlines()
     results = []
     for line in lines:
         if re.search(regex, line):
             results.append(line.strip())
     return results
+
+
+def cli_cmd_to_string(args):
+    """Converts a cmd arg list to string.
+
+    Args:
+        args: list of strings, the arguments of a command.
+
+    Returns:
+        String representation of the command.
+    """
+    if isinstance(args, basestring):
+        # Return directly if it's already a string.
+        return args
+    return ' '.join([pipes.quote(arg) for arg in args])
```

### Comparing `mobly-1.8.1/mobly/test_runner.py` & `mobly-1.9.1/mobly/test_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 # limitations under the License.
 
 from __future__ import print_function
 from future import standard_library
 standard_library.install_aliases()
 
 import argparse
+import contextlib
 import inspect
 import logging
 import os
 import sys
 
 from mobly import base_test
 from mobly import config_parser
 from mobly import logger
 from mobly import records
 from mobly import signals
+from mobly import utils
 
 
 class Error(Exception):
     pass
 
 
 def main(argv=None):
@@ -67,26 +69,27 @@
     # Parse test specifiers if exist.
     tests = None
     if args.tests:
         tests = args.tests
     # Execute the test class with configs.
     ok = True
     for config in test_configs:
-        runner = TestRunner(
-            log_dir=config.log_path, test_bed_name=config.test_bed_name)
-        runner.add_test_class(config, test_class, tests)
-        try:
-            runner.run()
-            ok = runner.results.is_all_pass and ok
-        except signals.TestAbortAll:
-            pass
-        except:
-            logging.exception('Exception when executing %s.',
-                              config.test_bed_name)
-            ok = False
+        runner = TestRunner(log_dir=config.log_path,
+                            test_bed_name=config.test_bed_name)
+        with runner.mobly_logger():
+            runner.add_test_class(config, test_class, tests)
+            try:
+                runner.run()
+                ok = runner.results.is_all_pass and ok
+            except signals.TestAbortAll:
+                pass
+            except:
+                logging.exception('Exception when executing %s.',
+                                  config.test_bed_name)
+                ok = False
     if not ok:
         sys.exit(1)
 
 
 def parse_mobly_cli_args(argv):
     """Parses cli args that are consumed by Mobly.
 
@@ -101,41 +104,38 @@
             input.
 
     Returns:
         Namespace containing the parsed args.
     """
     parser = argparse.ArgumentParser(description='Mobly Test Executable.')
     group = parser.add_mutually_exclusive_group(required=True)
-    group.add_argument(
-        '-c',
-        '--config',
-        nargs=1,
-        type=str,
-        metavar='<PATH>',
-        help='Path to the test configuration file.')
+    group.add_argument('-c',
+                       '--config',
+                       nargs=1,
+                       type=str,
+                       metavar='<PATH>',
+                       help='Path to the test configuration file.')
     group.add_argument(
         '-l',
         '--list_tests',
         action='store_true',
         help='Print the names of the tests defined in a script without '
         'executing them.')
-    parser.add_argument(
-        '--tests',
-        '--test_case',
-        nargs='+',
-        type=str,
-        metavar='[test_a test_b...]',
-        help='A list of tests in the test class to execute.')
-    parser.add_argument(
-        '-tb',
-        '--test_bed',
-        nargs='+',
-        type=str,
-        metavar='[<TEST BED NAME1> <TEST BED NAME2> ...]',
-        help='Specify which test beds to run tests on.')
+    parser.add_argument('--tests',
+                        '--test_case',
+                        nargs='+',
+                        type=str,
+                        metavar='[test_a test_b...]',
+                        help='A list of tests in the test class to execute.')
+    parser.add_argument('-tb',
+                        '--test_bed',
+                        nargs='+',
+                        type=str,
+                        metavar='[<TEST BED NAME1> <TEST BED NAME2> ...]',
+                        help='Specify which test beds to run tests on.')
     if not argv:
         argv = sys.argv[1:]
     return parser.parse_known_args(argv)[0]
 
 
 def _find_test_class():
     """Finds the test class in a test script.
@@ -215,55 +215,44 @@
         """
         self._log_dir = log_dir
         self._test_bed_name = test_bed_name
 
         self.results = records.TestResult()
         self._test_run_infos = []
 
-        self._log_path = None
-
-    def setup_logger(self):
-        """Sets up logging for the next test run.
-
-        This is called automatically in 'run', so normally, this method doesn't
-        need to be called. Only use this method if you want to use Mobly's
-        logger before the test run starts.
-
-        .. code-block:: python
-
-            tr = TestRunner(...)
-            tr.setup_logger()
-            logging.info(...)
-            tr.run()
-
-        """
-        if self._log_path is not None:
-            return
+        # Set default logging values. Necessary if `run` is used outside of the
+        # `mobly_logger` context.
+        self._update_log_path()
 
+    def _update_log_path(self):
+        """Updates the logging values with the current timestamp."""
         self._start_time = logger.get_log_file_timestamp()
         self._log_path = os.path.join(self._log_dir, self._test_bed_name,
                                       self._start_time)
-        logger.setup_test_logger(self._log_path, self._test_bed_name)
 
-    def _teardown_logger(self):
-        """Tears down logging at the end of the test run.
+    @contextlib.contextmanager
+    def mobly_logger(self, alias='latest'):
+        """Starts and stops a logging context for a Mobly test run.
 
-        This is called automatically in 'run', so normally, this method doesn't
-        need to be called. Only use this to change the logger teardown
-        behaviour.
+        Args:
+          alias: optional string, the name of the latest log alias directory to
+              create. If a falsy value is specified, then the directory will not
+              be created.
 
-        Raises:
-            Error: if this is called before the logger is setup.
+        Yields:
+            The host file path where the logs for the test run are stored.
         """
-        if self._log_path is None:
-            raise Error('TestRunner._teardown_logger() called before '
-                        'TestRunner.setup_logger()!')
-
-        logger.kill_test_logger(logging.getLogger())
-        self._log_path = None
+        self._update_log_path()
+        logger.setup_test_logger(self._log_path,
+                                 self._test_bed_name,
+                                 alias=alias)
+        try:
+            yield self._log_path
+        finally:
+            logger.kill_test_logger(logging.getLogger())
 
     def add_test_class(self, config, test_class, tests=None, name_suffix=None):
         """Adds tests to the execution plan of this TestRunner.
 
         Args:
             config: config_parser.TestRunConfig, configuration to execute this
                 test class with.
@@ -278,84 +267,84 @@
             Error: if the provided config has a log_path or test_bed_name which
                 differs from the arguments provided to this TestRunner's
                 constructor.
         """
         if self._log_dir != config.log_path:
             raise Error(
                 'TestRunner\'s log folder is "%s", but a test config with a '
-                'different log folder ("%s") was added.' % (self._log_dir,
-                                                            config.log_path))
+                'different log folder ("%s") was added.' %
+                (self._log_dir, config.log_path))
         if self._test_bed_name != config.test_bed_name:
             raise Error(
                 'TestRunner\'s test bed is "%s", but a test config with a '
                 'different test bed ("%s") was added.' %
                 (self._test_bed_name, config.test_bed_name))
         self._test_run_infos.append(
-            TestRunner._TestRunInfo(
-                config=config,
-                test_class=test_class,
-                tests=tests,
-                test_class_name_suffix=name_suffix))
+            TestRunner._TestRunInfo(config=config,
+                                    test_class=test_class,
+                                    tests=tests,
+                                    test_class_name_suffix=name_suffix))
 
     def _run_test_class(self, config, test_class, tests=None):
         """Instantiates and executes a test class.
 
         If tests is None, the tests listed in self.tests will be executed
         instead. If self.tests is empty as well, every test in this test class
         will be executed.
 
         Args:
             config: A config_parser.TestRunConfig object.
             test_class: class, test class to execute.
             tests: Optional list of test names within the class to execute.
         """
-        with test_class(config) as test_instance:
-            logging.debug('Executing test class "%s" with config: %s',
-                          test_class.__name__, config)
-            try:
-                cls_result = test_instance.run(tests)
-                self.results += cls_result
-            except signals.TestAbortAll as e:
-                self.results += e.results
-                raise e
+        test_instance = test_class(config)
+        logging.debug('Executing test class "%s" with config: %s',
+                      test_class.__name__, config)
+        try:
+            cls_result = test_instance.run(tests)
+            self.results += cls_result
+        except signals.TestAbortAll as e:
+            self.results += e.results
+            raise e
 
     def run(self):
         """Executes tests.
 
         This will instantiate controller and test classes, execute tests, and
         print a summary.
 
         Raises:
             Error: if no tests have previously been added to this runner using
                 add_test_class(...).
         """
         if not self._test_run_infos:
             raise Error('No tests to execute.')
 
-        self.setup_logger()
+        # Ensure the log path exists. Necessary if `run` is used outside of the
+        # `mobly_logger` context.
+        utils.create_dir(self._log_path)
+
         summary_writer = records.TestSummaryWriter(
             os.path.join(self._log_path, records.OUTPUT_FILE_SUMMARY))
         try:
             for test_run_info in self._test_run_infos:
                 # Set up the test-specific config
                 test_config = test_run_info.config.copy()
                 test_config.log_path = self._log_path
                 test_config.summary_writer = summary_writer
                 test_config.test_class_name_suffix = test_run_info.test_class_name_suffix
                 try:
-                    self._run_test_class(
-                        config=test_config,
-                        test_class=test_run_info.test_class,
-                        tests=test_run_info.tests)
+                    self._run_test_class(config=test_config,
+                                         test_class=test_run_info.test_class,
+                                         tests=test_run_info.tests)
                 except signals.TestAbortAll as e:
                     logging.warning(
                         'Abort all subsequent test classes. Reason: %s', e)
                     raise
         finally:
             summary_writer.dump(self.results.summary_dict(),
                                 records.TestSummaryEntryType.SUMMARY)
             # Stop and show summary.
             msg = '\nSummary for test run %s@%s: %s\n' % (
                 self._test_bed_name, self._start_time,
                 self.results.summary_str())
             logging.info(msg.strip())
-            self._teardown_logger()
```

### Comparing `mobly-1.8.1/mobly/controller_manager.py` & `mobly-1.9.1/mobly/controller_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,16 +149,16 @@
 
         This will be called after each test class.
         """
         # TODO(xpconanfan): actually record these errors instead of just
         # logging them.
         for name, module in self._controller_modules.items():
             logging.debug('Destroying %s.', name)
-            with expects.expect_no_raises(
-                    'Exception occurred destroying %s.' % name):
+            with expects.expect_no_raises('Exception occurred destroying %s.' %
+                                          name):
                 module.destroy(self._controller_objects[name])
         self._controller_objects = collections.OrderedDict()
         self._controller_modules = {}
 
     def _create_controller_info_record(self, controller_module_name):
         """Creates controller info record for a particular controller type.
 
@@ -174,23 +174,25 @@
         """
         module = self._controller_modules[controller_module_name]
         controller_info = None
         try:
             controller_info = module.get_info(
                 copy.copy(self._controller_objects[controller_module_name]))
         except AttributeError:
-            logging.warning('No optional debug info found for controller '
-                            '%s. To provide it, implement `get_info`.',
-                            controller_module_name)
+            logging.warning(
+                'No optional debug info found for controller '
+                '%s. To provide it, implement `get_info`.',
+                controller_module_name)
         try:
             yaml.dump(controller_info)
         except TypeError:
-            logging.warning('The info of controller %s in class "%s" is not '
-                            'YAML serializable! Coercing it to string.',
-                            controller_module_name, self._class_name)
+            logging.warning(
+                'The info of controller %s in class "%s" is not '
+                'YAML serializable! Coercing it to string.',
+                controller_module_name, self._class_name)
             controller_info = str(controller_info)
         return records.ControllerInfoRecord(
             self._class_name, module.MOBLY_CONTROLLER_CONFIG_NAME,
             controller_info)
 
     def get_controller_info_records(self):
         """Get the info records for all the controller objects in the manager.
```

### Comparing `mobly-1.8.1/mobly/asserts.py` & `mobly-1.9.1/mobly/asserts.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,26 +39,26 @@
     Args:
         first: The first object to compare.
         second: The second object to compare.
         msg: A string that adds additional info about the failure.
         extras: An optional field for extra information to be included in
             test result.
     """
+    my_msg = None
     try:
         _pyunit_proxy.assertEqual(first, second)
-    except Exception as e:
-        # We have to catch all here for py2/py3 compatibility.
-        # In py2, assertEqual throws exceptions.AssertionError, which does not
-        # exist in py3. In py3, it throws unittest.case.failureException, which
-        # does not exist in py2. To accommodate using explicit catch complicates
-        # the code like hell, so I opted to catch all instead.
+    except AssertionError as e:
         my_msg = str(e)
         if msg:
             my_msg = "%s %s" % (my_msg, msg)
-        fail(my_msg, extras=extras)
+
+    # This raise statement is outside of the above except statement to prevent
+    # Python3's exception message from having two tracebacks.
+    if my_msg is not None:
+        raise signals.TestFailure(my_msg, extras=extras)
 
 
 def assert_raises(expected_exception, extras=None, *args, **kwargs):
     """Assert that an exception is raised when a function is called.
 
     If no exception is raised, test fail. If an exception is raised but not
     of the expected type, the exception is let through.
@@ -95,16 +95,17 @@
 
     Args:
         expected_exception: An exception class that is expected to be
             raised.
         extras: An optional field for extra information to be included in
             test result.
     """
-    context = _AssertRaisesContext(
-        expected_exception, expected_regex, extras=extras)
+    context = _AssertRaisesContext(expected_exception,
+                                   expected_regex,
+                                   extras=extras)
     return context
 
 
 def assert_true(expr, msg, extras=None):
     """Assert an expression evaluates to true, otherwise fail the test.
 
     Args:
@@ -274,25 +275,25 @@
 
     def __exit__(self, exc_type, exc_value, tb):
         if exc_type is None:
             try:
                 exc_name = self.expected.__name__
             except AttributeError:
                 exc_name = str(self.expected)
-            raise signals.TestFailure(
-                '%s not raised' % exc_name, extras=self.extras)
+            raise signals.TestFailure('%s not raised' % exc_name,
+                                      extras=self.extras)
         if not issubclass(exc_type, self.expected):
             # let unexpected exceptions pass through
             return False
         self.exception = exc_value  # store for later retrieval
         if self.expected_regexp is None:
             return True
 
         expected_regexp = self.expected_regexp
         if isinstance(expected_regexp, str):
             expected_regexp = re.compile(expected_regexp)
         if not expected_regexp.search(str(exc_value)):
             raise signals.TestFailure(
-                '"%s" does not match "%s"' % (expected_regexp.pattern,
-                                              str(exc_value)),
+                '"%s" does not match "%s"' %
+                (expected_regexp.pattern, str(exc_value)),
                 extras=self.extras)
         return True
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device.py` & `mobly-1.9.1/mobly/controllers/android_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 from mobly import logger as mobly_logger
 from mobly import utils
 from mobly.controllers.android_device_lib import adb
 from mobly.controllers.android_device_lib import errors
 from mobly.controllers.android_device_lib import fastboot
 from mobly.controllers.android_device_lib import service_manager
-from mobly.controllers.android_device_lib.services import sl4a_service
 from mobly.controllers.android_device_lib.services import logcat
 from mobly.controllers.android_device_lib.services import snippet_management_service
 
 # Convenience constant for the package of Mobly Bundled Snippets
 # (http://github.com/google/mobly-bundled-snippets).
 MBS_PACKAGE = 'com.google.android.mobly.snippet.bundled'
 
@@ -41,25 +40,40 @@
 _DEBUG_PREFIX_TEMPLATE = '[AndroidDevice|%s] %s'
 
 # Key name for adb logcat extra params in config file.
 ANDROID_DEVICE_ADB_LOGCAT_PARAM_KEY = 'adb_logcat_param'
 ANDROID_DEVICE_EMPTY_CONFIG_MSG = 'Configuration is empty, abort!'
 ANDROID_DEVICE_NOT_LIST_CONFIG_MSG = 'Configuration should be a list, abort!'
 
+# System properties that are cached by the `AndroidDevice.build_info` property.
+# The only properties on this list should be read-only system properties.
+CACHED_SYSTEM_PROPS = [
+    'ro.build.id',
+    'ro.build.type',
+    'ro.build.version.codename',
+    'ro.build.version.sdk',
+    'ro.build.product',
+    'ro.debuggable',
+    'ro.product.name',
+]
+
 # Keys for attributes in configs that alternate the controller module behavior.
 # If this is False for a device, errors from that device will be ignored
 # during `create`. Default is True.
 KEY_DEVICE_REQUIRED = 'required'
 DEFAULT_VALUE_DEVICE_REQUIRED = True
 # If True, logcat collection will not be started during `create`.
 # Default is False.
 KEY_SKIP_LOGCAT = 'skip_logcat'
 DEFAULT_VALUE_SKIP_LOGCAT = False
 SERVICE_NAME_LOGCAT = 'logcat'
 
+# Default name for bug reports taken without a specified test name.
+DEFAULT_BUG_REPORT_NAME = 'bugreport'
+
 # Default Timeout to wait for boot completion
 DEFAULT_TIMEOUT_BOOT_COMPLETION_SECOND = 15 * 60
 
 # Aliases of error types for backward compatibility.
 Error = errors.Error
 DeviceError = errors.DeviceError
 SnippetError = snippet_management_service.Error
@@ -89,29 +103,30 @@
         ads = get_instances(configs)
     else:
         raise Error('No valid config found in: %s' % configs)
     valid_ad_identifiers = list_adb_devices() + list_adb_devices_by_usb_id()
 
     for ad in ads:
         if ad.serial not in valid_ad_identifiers:
-            raise DeviceError(ad, 'Android device is specified in config but'
-                              ' is not attached.')
+            raise DeviceError(
+                ad, 'Android device is specified in config but is not '
+                'attached.')
     _start_services_on_ads(ads)
     return ads
 
 
 def destroy(ads):
     """Cleans up AndroidDevice objects.
 
     Args:
         ads: A list of AndroidDevice objects.
     """
     for ad in ads:
         try:
-            ad.stop_services()
+            ad.services.stop_all()
         except:
             ad.log.exception('Failed to clean up properly.')
 
 
 def get_info(ads):
     """Get information on a list of AndroidDevice objects.
 
@@ -124,33 +139,31 @@
     return [ad.device_info for ad in ads]
 
 
 def _start_services_on_ads(ads):
     """Starts long running services on multiple AndroidDevice objects.
 
     If any one AndroidDevice object fails to start services, cleans up all
-    existing AndroidDevice objects and their services.
+    AndroidDevice objects and their services.
 
     Args:
         ads: A list of AndroidDevice objects whose services to start.
     """
-    running_ads = []
     for ad in ads:
-        running_ads.append(ad)
         start_logcat = not getattr(ad, KEY_SKIP_LOGCAT,
                                    DEFAULT_VALUE_SKIP_LOGCAT)
         try:
-            ad.services.register(
-                SERVICE_NAME_LOGCAT, logcat.Logcat, start_service=start_logcat)
+            if start_logcat:
+                ad.services.logcat.start()
         except Exception:
             is_required = getattr(ad, KEY_DEVICE_REQUIRED,
                                   DEFAULT_VALUE_DEVICE_REQUIRED)
             if is_required:
                 ad.log.exception('Failed to start some services, abort!')
-                destroy(running_ads)
+                destroy(ads)
                 raise
             else:
                 ad.log.exception('Skipping this optional device because some '
                                  'services failed to start.')
 
 
 def _parse_device_list(device_list_str, key):
@@ -369,34 +382,40 @@
     if len(filtered) == 1:
         return filtered[0]
     else:
         serials = [ad.serial for ad in filtered]
         raise Error('More than one device matched: %s' % serials)
 
 
-def take_bug_reports(ads, test_name, begin_time, destination=None):
+def take_bug_reports(ads, test_name=None, begin_time=None, destination=None):
     """Takes bug reports on a list of android devices.
 
     If you want to take a bug report, call this function with a list of
     android_device objects in on_fail. But reports will be taken on all the
     devices in the list concurrently. Bug report takes a relative long
     time to take, so use this cautiously.
 
     Args:
         ads: A list of AndroidDevice instances.
         test_name: Name of the test method that triggered this bug report.
+            If None, the default name "bugreport" will be used.
         begin_time: timestamp taken when the test started, can be either
-            string or int.
+            string or int. If None, the current time will be used.
         destination: string, path to the directory where the bugreport
             should be saved.
     """
-    begin_time = mobly_logger.normalize_log_line_timestamp(str(begin_time))
+    if begin_time is None:
+        begin_time = mobly_logger.get_log_file_timestamp()
+    else:
+        begin_time = mobly_logger.normalize_log_line_timestamp(str(begin_time))
 
     def take_br(test_name, begin_time, ad, destination):
-        ad.take_bug_report(test_name, begin_time, destination=destination)
+        ad.take_bug_report(test_name=test_name,
+                           begin_time=begin_time,
+                           destination=destination)
 
     args = [(test_name, begin_time, ad, destination) for ad in ads]
     utils.concurrent_exec(take_br, args)
 
 
 class AndroidDevice(object):
     """Class representing an android device.
@@ -428,22 +447,26 @@
     def __init__(self, serial=''):
         self._serial = str(serial)
         # logging.log_path only exists when this is used in an Mobly test run.
         self._log_path_base = getattr(logging, 'log_path', '/tmp/logs')
         self._log_path = os.path.join(
             self._log_path_base, 'AndroidDevice%s' % self._normalized_serial)
         self._debug_tag = self._serial
-        self.log = AndroidDeviceLoggerAdapter(logging.getLogger(), {
-            'tag': self.debug_tag
-        })
+        self.log = AndroidDeviceLoggerAdapter(logging.getLogger(),
+                                              {'tag': self.debug_tag})
+        self._build_info = None
+        self._is_rebooting = False
         self.adb = adb.AdbProxy(serial)
         self.fastboot = fastboot.FastbootProxy(serial)
         if not self.is_bootloader and self.is_rootable:
             self.root_adb()
         self.services = service_manager.ServiceManager(self)
+        self.services.register(SERVICE_NAME_LOGCAT,
+                               logcat.Logcat,
+                               start_service=False)
         self.services.register(
             'snippets', snippet_management_service.SnippetManagementService)
         # Device info cache.
         self._user_added_device_info = {}
 
     def __repr__(self):
         return '<AndroidDevice|%s>' % self.debug_tag
@@ -618,62 +641,50 @@
             )
         if self._debug_tag == self.serial:
             self._debug_tag = new_serial
         self._serial = new_serial
         self.adb.serial = new_serial
         self.fastboot.serial = new_serial
 
-    def start_services(self, clear_log=True):
-        """.. deprecated:: 1.8
-
-        Use service manager `self.services` instead.
-
-        Starts long running services on the android device, like adb logcat
-        capture.
-        """
-        self.services.start_all()
-
-    def start_adb_logcat(self, clear_log=True):
-        """.. deprecated:: 1.8
-
-        Use `self.services.logcat.start` instead.
-        """
-        self.services.logcat.start()
-
-    def stop_adb_logcat(self):
-        """.. deprecated:: 1.8
-
-        Use `self.services.logcat.stop` instead.
-        """
-        self.services.logcat.stop()
-
-    def stop_services(self):
-        """.. deprecated:: 1.8
-
-        Use service manager `self.services` instead.
-
-        Stops long running services on the Android device."""
-        self.services.stop_all()
-
     @contextlib.contextmanager
     def handle_reboot(self):
         """Properly manage the service life cycle when the device needs to
         temporarily disconnect.
 
         The device can temporarily lose adb connection due to user-triggered
         reboot. Use this function to make sure the services
         started by Mobly are properly stopped and restored afterwards.
 
         For sample usage, see self.reboot().
         """
-        self.stop_services()
+        self.services.stop_all()
+        # On rooted devices, system properties may change on reboot, so disable
+        # the `build_info` cache by setting `_is_rebooting` to True and
+        # repopulate it after reboot.
+        # Note, this logic assumes that instance variable assignment in Python
+        # is atomic; otherwise, `threading` data structures would be necessary.
+        # Additionally, nesting calls to `handle_reboot` while changing the
+        # read-only property values during reboot will result in stale values.
+        self._is_rebooting = True
         try:
             yield
         finally:
             self.wait_for_boot_completion()
+            # On boot completion, invalidate the `build_info` cache since any
+            # value it had from before boot completion is potentially invalid.
+            # If the value gets set after the final invalidation and before
+            # setting`_is_rebooting` to True, then that's okay because the
+            # device has finished rebooting at that point, and values at that
+            # point should be valid.
+            # If the reboot fails for some reason, then `_is_rebooting` is never
+            # set to False, which means the `build_info` cache remains disabled
+            # until the next reboot. This is relatively okay because the
+            # `build_info` cache is only minimizes adb commands.
+            self._build_info = None
+            self._is_rebooting = False
             if self.is_rootable:
                 self.root_adb()
         self.services.start_all()
 
     @contextlib.contextmanager
     def handle_usb_disconnect(self):
         """Properly manage the service life cycle when USB is disconnected.
@@ -738,18 +749,29 @@
             A dict with the build info of this Android device, or None if the
             device is in bootloader mode.
         """
         if self.is_bootloader:
             self.log.error('Device is in fastboot mode, could not get build '
                            'info.')
             return
-        info = {}
-        info['build_id'] = self.adb.getprop('ro.build.id')
-        info['build_type'] = self.adb.getprop('ro.build.type')
-        return info
+        if self._build_info is None or self._is_rebooting:
+            info = {}
+            build_info = self.adb.getprops(CACHED_SYSTEM_PROPS)
+            info['build_id'] = build_info['ro.build.id']
+            info['build_type'] = build_info['ro.build.type']
+            info['build_version_codename'] = build_info.get(
+                'ro.build.version.codename', '')
+            info['build_version_sdk'] = build_info.get('ro.build.version.sdk',
+                                                       '')
+            info['build_product'] = build_info.get('ro.build.product', '')
+            info['debuggable'] = build_info.get('ro.debuggable', '')
+            info['product_name'] = build_info.get('ro.product.name', '')
+            self._build_info = info
+            return info
+        return self._build_info
 
     @property
     def is_bootloader(self):
         """True if the device is in bootloader mode.
         """
         return self.serial in list_fastboot_devices()
 
@@ -762,15 +784,15 @@
         except adb.AdbError:
             # Wait a bit and retry to work around adb flakiness for this cmd.
             time.sleep(0.2)
             return '0' == self.adb.shell('id -u').decode('utf-8').strip()
 
     @property
     def is_rootable(self):
-        return self.adb.getprop('ro.debuggable') == '1'
+        return self.build_info['debuggable'] == '1'
 
     @property
     def model(self):
         """The Android code name for the device.
         """
         # If device is in bootloader mode, get mode name from fastboot.
         if self.is_bootloader:
@@ -779,18 +801,18 @@
             # writes to stderr.
             lines = out.decode('utf-8').split('\n', 1)
             if lines:
                 tokens = lines[0].split(' ')
                 if len(tokens) > 1:
                     return tokens[1].lower()
             return None
-        model = self.adb.getprop('ro.build.product').lower()
+        model = self.build_info['build_product'].lower()
         if model == 'sprout':
             return model
-        return self.adb.getprop('ro.product.name').lower()
+        return self.build_info['product_name'].lower()
 
     def load_config(self, config):
         """Add attributes to the AndroidDevice object based on config.
 
         Args:
             config: A dictionary representing the configs.
 
@@ -850,46 +872,41 @@
             name: The attribute name the snippet server is attached with.
 
         Raises:
             SnippetError: The given snippet name is not registered.
         """
         self.services.snippets.remove_snippet_client(name)
 
-    def load_sl4a(self):
-        """.. deprecated:: 1.8
-
-        Directly register with service manager instead:
-        `self.services.register('sl4a', sl4a_service.Sl4aService)`
-
-        Register sl4a_service directly instead.
-
-        Start sl4a service on the Android device.
-
-        Launch sl4a server if not already running, spin up a session on the
-        server, and two connections to this session.
-        """
-        self.log.warning('`load_sl4a` is deprecated and scheduled for removal!'
-                         ' Register sl4a as a service instead.')
-        self.services.register('sl4a', sl4a_service.Sl4aService)
-
     def take_bug_report(self,
-                        test_name,
-                        begin_time,
+                        test_name=None,
+                        begin_time=None,
                         timeout=300,
                         destination=None):
         """Takes a bug report on the device and stores it in a file.
 
         Args:
             test_name: Name of the test method that triggered this bug report.
-            begin_time: Timestamp of when the test started.
+                If not set, then this will default to
+                android_device.DEFAULT_BUG_REPORT_NAME.
+            begin_time: Timestamp of when the test started. If not set, then
+                this will default to the current time.
             timeout: float, the number of seconds to wait for bugreport to
                 complete, default is 5min.
             destination: string, path to the directory where the bugreport
                 should be saved.
+
+        Returns:
+          A string containing the absolute path to the bug report on the host
+          machine.
         """
+        if test_name is None:
+            test_name = DEFAULT_BUG_REPORT_NAME
+        if begin_time is None:
+            begin_time = mobly_logger.get_log_file_timestamp()
+
         new_br = True
         try:
             stdout = self.adb.shell('bugreportz -v').decode('utf-8')
             # This check is necessary for builds before N, where adb shell's ret
             # code and stderr are not propagated properly.
             if 'not found' in stdout:
                 new_br = False
@@ -914,18 +931,20 @@
             if not out.startswith('OK'):
                 raise DeviceError(self, 'Failed to take bugreport: %s' % out)
             br_out_path = out.split(':')[1].strip()
             self.adb.pull([br_out_path, full_out_path])
         else:
             # shell=True as this command redirects the stdout to a local file
             # using shell redirection.
-            self.adb.bugreport(
-                ' > "%s"' % full_out_path, shell=True, timeout=timeout)
+            self.adb.bugreport(' > "%s"' % full_out_path,
+                               shell=True,
+                               timeout=timeout)
         self.log.info('Bugreport for %s taken at %s.', test_name,
                       full_out_path)
+        return full_out_path
 
     def run_iperf_client(self, server_host, extra_args=''):
         """Start iperf client on the device.
 
         Return status as true if iperf client start successfully.
         And data flow information as results.
 
@@ -957,15 +976,15 @@
         timeout_start = time.time()
 
         self.adb.wait_for_device(timeout=timeout)
         while time.time() < timeout_start + timeout:
             try:
                 if self.is_boot_completed():
                     return
-            except adb.AdbError:
+            except (adb.AdbError, adb.AdbTimeoutError):
                 # adb shell calls may fail during certain period of booting
                 # process, which is normal. Ignoring these errors.
                 pass
             time.sleep(5)
         raise DeviceError(self, 'Booting process timed out')
 
     def is_boot_completed(self):
@@ -983,21 +1002,20 @@
             self.log.debug('Is now adb detectable.')
             return True
         return False
 
     def reboot(self):
         """Reboots the device.
 
-        Terminate all sl4a sessions, reboot the device, wait for device to
-        complete booting, and restart an sl4a session.
-
-        This is a blocking method.
+        Generally one should use this method to reboot the device instead of
+        directly calling `adb.reboot`. Because this method gracefully handles
+        the teardown and restoration of running services.
 
-        This is probably going to print some error messages in console. Only
-        use if there's no other option.
+        This method is blocking and only returns when the reboot has completed
+        and the services restored.
 
         Raises:
             Error: Waiting for completion timed out.
         """
         if self.is_bootloader:
             self.fastboot.reboot()
             return
```

### Comparing `mobly-1.8.1/mobly/controllers/iperf_server.py` & `mobly-1.9.1/mobly/controllers/iperf_server.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly/controllers/__init__.py` & `mobly-1.9.1/mobly/controllers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
```

### Comparing `mobly-1.8.1/mobly/controllers/sniffer_lib/__init__.py` & `mobly-1.9.1/mobly/controllers/sniffer_lib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
```

### Comparing `mobly-1.8.1/mobly/controllers/sniffer_lib/local/tshark.py` & `mobly-1.9.1/mobly/controllers/sniffer_lib/local/tshark.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import shutil
 from mobly.controllers import sniffer
 from mobly.controllers.sniffer_lib.local import local_base
 
+
 class Sniffer(local_base.SnifferLocalBase):
     """This class defines a sniffer which uses tshark as its back-end
     """
 
     def __init__(self, config_path, logger, base_configs=None):
         """See base class documentation
         """
         self._executable_path = None
 
         super().__init__(config_path, logger, base_configs=base_configs)
 
         self._executable_path = (shutil.which("tshark")
                                  or shutil.which("/usr/local/bin/tshark"))
         if self._executable_path is None:
-            raise sniffer.SnifferError("Cannot find a path to the 'tshark' "
-                                 "executable (or to '/usr/local/bin/tshark')")
+            raise sniffer.SnifferError(
+                "Cannot find a path to the 'tshark' "
+                "executable (or to '/usr/local/bin/tshark')")
 
     def get_descriptor(self):
         """See base class documentation
         """
         return "local-tshark-{}-ch{}".format(self._interface)
 
     def get_subtype(self):
         """See base class documentation
         """
         return "tshark"
 
-    def _get_command_line(self, additional_args=None, duration=None,
+    def _get_command_line(self,
+                          additional_args=None,
+                          duration=None,
                           packet_count=None):
         cmd = "{} -i {} -w {}".format(self._executable_path, self._interface,
                                       self._temp_capture_file_path)
         if duration is not None:
             cmd = "{} -a duration:{}".format(cmd, duration)
         if packet_count is not None:
             cmd = "{} -c {}".format(cmd, packet_count)
```

### Comparing `mobly-1.8.1/mobly/controllers/sniffer_lib/local/__init__.py` & `mobly-1.9.1/mobly/controllers/sniffer_lib/local/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
```

### Comparing `mobly-1.8.1/mobly/controllers/sniffer_lib/local/local_base.py` & `mobly-1.9.1/mobly/controllers/sniffer_lib/local/local_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """
 Class for Local sniffers - i.e. running on the local machine.
 
 This class provides configuration for local interfaces but leaves
 the actual capture (sniff) to sub-classes.
 """
 
@@ -24,14 +23,15 @@
 import signal
 import subprocess
 import tempfile
 from mobly import logger
 from mobly import utils
 from mobly.controllers import sniffer
 
+
 class SnifferLocalBase(sniffer.Sniffer):
     """This class defines the common behaviors of WLAN sniffers running on
     WLAN interfaces of the local machine.
 
     Specific mechanisms to capture packets over the local WLAN interfaces are
     implemented by sub-classes of this class - i.e. it is not a final class.
     """
@@ -83,22 +83,23 @@
             final_configs.update(self._base_configs)
         if override_configs:
             final_configs.update(override_configs)
 
         if sniffer.Sniffer.CONFIG_KEY_CHANNEL in final_configs:
             try:
                 subprocess.check_call([
-                    'iwconfig',
-                    self._interface,
-                    'channel',
-                    str(final_configs[sniffer.Sniffer.CONFIG_KEY_CHANNEL])])
+                    'iwconfig', self._interface, 'channel',
+                    str(final_configs[sniffer.Sniffer.CONFIG_KEY_CHANNEL])
+                ])
             except Exception as err:
                 raise sniffer.ExecutionError(err)
 
-    def _get_command_line(self, additional_args=None, duration=None,
+    def _get_command_line(self,
+                          additional_args=None,
+                          duration=None,
                           packet_count=None):
         """Utility function to be implemented by every child class - which
         are the concrete sniffer classes. Each sniffer-specific class should
         derive the command line to execute its sniffer based on the specified
         arguments.
         """
         raise NotImplementedError("Base class should not be called directly!")
@@ -106,50 +107,54 @@
     def _post_process(self):
         """Utility function which is executed after a capture is done. It
         moves the capture file to the requested location.
         """
         self._process = None
         shutil.move(self._temp_capture_file_path, self._capture_file_path)
 
-    def start_capture(self, override_configs=None,
-                      additional_args=None, duration=None,
+    def start_capture(self,
+                      override_configs=None,
+                      additional_args=None,
+                      duration=None,
                       packet_count=None):
         """See base class documentation
         """
         if self._process is not None:
             raise sniffer.InvalidOperationError(
-                    "Trying to start a sniff while another is still running!")
+                "Trying to start a sniff while another is still running!")
         capture_dir = os.path.join(self._logger.log_path,
                                    "Sniffer-{}".format(self._interface))
         os.makedirs(capture_dir, exist_ok=True)
-        self._capture_file_path = os.path.join(capture_dir,
-                      "capture_{}.pcap".format(logger.get_log_file_timestamp()))
+        self._capture_file_path = os.path.join(
+            capture_dir,
+            "capture_{}.pcap".format(logger.get_log_file_timestamp()))
 
         self._pre_capture_config(override_configs)
         _, self._temp_capture_file_path = tempfile.mkstemp(suffix=".pcap")
 
         cmd = self._get_command_line(additional_args=additional_args,
-                                duration=duration, packet_count=packet_count)
+                                     duration=duration,
+                                     packet_count=packet_count)
 
         self._process = utils.start_standing_subprocess(cmd)
         return sniffer.ActiveCaptureContext(self, duration)
 
     def stop_capture(self):
         """See base class documentation
         """
         if self._process is None:
             raise sniffer.InvalidOperationError(
-                                      "Trying to stop a non-started process")
-        utils.stop_standing_subprocess(self._process, kill_signal=signal.SIGINT)
+                "Trying to stop a non-started process")
+        utils.stop_standing_subprocess(self._process)
         self._post_process()
 
     def wait_for_capture(self, timeout=None):
         """See base class documentation
         """
         if self._process is None:
             raise sniffer.InvalidOperationError(
-                                  "Trying to wait on a non-started process")
+                "Trying to wait on a non-started process")
         try:
             utils.wait_for_standing_subprocess(self._process, timeout)
             self._post_process()
         except subprocess.TimeoutExpired:
             self.stop_capture()
```

### Comparing `mobly-1.8.1/mobly/controllers/sniffer_lib/local/tcpdump.py` & `mobly-1.9.1/mobly/controllers/sniffer_lib/local/tcpdump.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import shutil
 from mobly.controllers import sniffer
 from mobly.controllers.sniffer_lib.local import local_base
 
+
 class Sniffer(local_base.SnifferLocalBase):
     """This class defines a sniffer which uses tcpdump as its back-end
     """
 
     def __init__(self, config_path, logger, base_configs=None):
         """See base class documentation
         """
         self._executable_path = None
 
         super().__init__(config_path, logger, base_configs=base_configs)
 
         self._executable_path = shutil.which("tcpdump")
         if self._executable_path is None:
             raise sniffer.SnifferError(
-                              "Cannot find a path to the 'tcpdump' executable")
+                "Cannot find a path to the 'tcpdump' executable")
 
     def get_descriptor(self):
         """See base class documentation
         """
         return "local-tcpdump-{}".format(self._interface)
 
     def get_subtype(self):
         """See base class documentation
         """
         return "tcpdump"
 
-    def _get_command_line(self, additional_args=None, duration=None,
+    def _get_command_line(self,
+                          additional_args=None,
+                          duration=None,
                           packet_count=None):
         cmd = "{} -i {} -w {}".format(self._executable_path, self._interface,
                                       self._temp_capture_file_path)
         if packet_count is not None:
             cmd = "{} -c {}".format(cmd, packet_count)
         if additional_args is not None:
             cmd = "{} {}".format(cmd, additional_args)
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/jsonrpc_client_base.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/jsonrpc_client_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,26 @@
                      identify events associated with a particular
                      CallbackHandler object.>
     }
 """
 
 from builtins import str
 
+# When the Python library `socket.create_connection` call is made, it indirectly
+# calls `import encodings.idna` through the `socket.getaddrinfo` method.
+# However, this chain of function calls is apparently not thread-safe in
+# embedded Python environments. So, pre-emptively import and cache the encoder.
+# See https://bugs.python.org/issue17305 for more details.
+try:
+    import encodings.idna
+except ImportError:
+    # Some implementations of Python (e.g. IronPython) do not support the`idna`
+    # encoding, so ignore import failures based on that.
+    pass
+
 import json
 import socket
 import threading
 
 from mobly.controllers.android_device_lib import callback_handler
 from mobly.controllers.android_device_lib import errors
 
@@ -323,16 +335,16 @@
                 ret_value=result['result'],
                 method_name=method,
                 ad=self._ad)
         return result['result']
 
     def disable_hidden_api_blacklist(self):
         """If necessary and possible, disables hidden api blacklist."""
-        version_codename = self._ad.adb.getprop('ro.build.version.codename')
-        sdk_version = int(self._ad.adb.getprop('ro.build.version.sdk'))
+        version_codename = self._ad.build_info['build_version_codename']
+        sdk_version = int(self._ad.build_info['build_version_sdk'])
         # we check version_codename in addition to sdk_version because P builds
         # in development report sdk_version 27, but still enforce the blacklist.
         if self._ad.is_rootable and (sdk_version >= 28
                                      or version_codename == 'P'):
             self._ad.adb.shell(
                 'settings put global hidden_api_blacklist_exemptions "*"')
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/snippet_event.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/snippet_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,18 @@
 
     Args:
         event_dict: a dictionary representing an event.
 
     Returns:
         A SnippetEvent object.
     """
-    return SnippetEvent(
-        callback_id=event_dict['callbackId'],
-        name=event_dict['name'],
-        creation_time=event_dict['time'],
-        data=event_dict['data'])
+    return SnippetEvent(callback_id=event_dict['callbackId'],
+                        name=event_dict['name'],
+                        creation_time=event_dict['time'],
+                        data=event_dict['data'])
 
 
 class SnippetEvent(object):
     """The class that represents callback events for mobly snippet library.
 
     Attributes:
         callback_id: string, the callback ID associated with the event.
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/service_manager.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/service_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Module for the manager of services."""
 # TODO(xpconanfan: move the device errors to a more generic location so
 # other device controllers like iOS can share it.
+import collections
 import inspect
 
 from mobly import expects
 from mobly.controllers.android_device_lib import errors
 from mobly.controllers.android_device_lib.services import base_service
 
 
@@ -29,15 +30,15 @@
     """Manager for services of AndroidDevice.
 
     A service is a long running process that involves an Android device, like
     adb logcat or Snippet.
     """
 
     def __init__(self, device):
-        self._service_objects = {}
+        self._service_objects = collections.OrderedDict()
         self._device = device
 
     def has_service_by_name(self, name):
         """Checks if the manager has a service registered with a specific name.
 
         Args:
             name: string, the name to look for.
@@ -108,41 +109,57 @@
         Errors occurred here will be recorded but not raised.
         """
         aliases = list(self._service_objects.keys())
         for alias in aliases:
             self.unregister(alias)
 
     def start_all(self):
-        """Starts all inactive service instances."""
+        """Starts all inactive service instances.
+
+        Services will be started in the order they were registered.
+        """
         for alias, service in self._service_objects.items():
             if not service.is_alive:
-                with expects.expect_no_raises(
-                        'Failed to start service "%s".' % alias):
+                with expects.expect_no_raises('Failed to start service "%s".' %
+                                              alias):
                     service.start()
 
     def stop_all(self):
-        """Stops all active service instances."""
-        for alias, service in self._service_objects.items():
+        """Stops all active service instances.
+
+        Services will be stopped in the reverse order they were registered.
+        """
+        # OrdereDict#items does not return a sequence in Python 3.4, so we have
+        # to do a list conversion here.
+        for alias, service in reversed(list(self._service_objects.items())):
             if service.is_alive:
-                with expects.expect_no_raises(
-                        'Failed to stop service "%s".' % alias):
+                with expects.expect_no_raises('Failed to stop service "%s".' %
+                                              alias):
                     service.stop()
 
     def pause_all(self):
-        """Pauses all service instances."""
-        for alias, service in self._service_objects.items():
-            with expects.expect_no_raises(
-                    'Failed to pause service "%s".' % alias):
+        """Pauses all service instances.
+
+        Services will be paused in the reverse order they were registered.
+        """
+        # OrdereDict#items does not return a sequence in Python 3.4, so we have
+        # to do a list conversion here.
+        for alias, service in reversed(list(self._service_objects.items())):
+            with expects.expect_no_raises('Failed to pause service "%s".' %
+                                          alias):
                 service.pause()
 
     def resume_all(self):
-        """Resumes all service instances."""
+        """Resumes all service instances.
+
+        Services will be resumed in the order they were registered.
+        """
         for alias, service in self._service_objects.items():
-            with expects.expect_no_raises(
-                    'Failed to pause service "%s".' % alias):
+            with expects.expect_no_raises('Failed to resume service "%s".' %
+                                          alias):
                 service.resume()
 
     def __getattr__(self, name):
         """Syntactic sugar to enable direct access of service objects by alias.
 
         Args:
             name: string, the alias a service object was registered under.
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/event_dispatcher.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/event_dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from concurrent.futures import ThreadPoolExecutor
@@ -108,16 +108,16 @@
         """
         if self.started:
             raise IllegalStateError(("Can't register service after polling is"
                                      " started"))
         self.lock.acquire()
         try:
             if event_name in self.handlers:
-                raise DuplicateError('A handler for {} already exists'.format(
-                    event_name))
+                raise DuplicateError(
+                    'A handler for {} already exists'.format(event_name))
             self.handlers[event_name] = (handler, args)
         finally:
             self.lock.release()
 
     def start(self):
         """Starts the event dispatcher.
 
@@ -178,16 +178,16 @@
         if not self.started:
             raise IllegalStateError(
                 "Dispatcher needs to be started before popping.")
 
         e_queue = self.get_event_q(event_name)
 
         if not e_queue:
-            raise TypeError("Failed to get an event queue for {}".format(
-                event_name))
+            raise TypeError(
+                "Failed to get an event queue for {}".format(event_name))
 
         try:
             # Block for timeout
             if timeout:
                 return e_queue.get(True, timeout)
             # Non-blocking poll for event
             elif timeout == 0:
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/__init__.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/fastboot.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/fastboot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from subprocess import Popen, PIPE
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/jsonrpc_shell_base.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/jsonrpc_shell_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,55 +11,61 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Shared library for frontends to jsonrpc servers."""
 from __future__ import print_function
 
 import code
+import os
 import pprint
 import sys
 
 from mobly.controllers import android_device
 
 
 class Error(Exception):
     pass
 
 
 class JsonRpcShellBase(object):
     def _start_services(self, console_env):
         """Starts the services needed by this client and adds them to console_env.
-  
+
         Must be implemented by subclasses.
         """
         raise NotImplemented()
 
     def _get_banner(self, serial):
         """Returns the user-friendly banner message to print before the console.
-  
+
         Must be implemented by subclasses.
         """
         raise NotImplemented()
 
     def load_device(self, serial=None):
         """Creates an AndroidDevice for the given serial number.
 
-        If no serial is given, it will be read from 'adb devices' if there is
-        only one.
+        If no serial is given, it will read from the ANDROID_SERIAL
+        environmental variable. If the environmental variable is not set, then
+        it will read from 'adb devices' if there is only one.
         """
         serials = android_device.list_adb_devices()
         if not serials:
             raise Error('No adb device found!')
         # No serial provided, try to pick up the device automatically.
         if not serial:
-            if len(serials) != 1:
+            env_serial = os.environ.get('ANDROID_SERIAL', None)
+            if env_serial is not None:
+                serial = env_serial
+            elif len(serials) == 1:
+                serial = serials[0]
+            else:
                 raise Error(
-                    'Expected one phone, but %d found. Use the -s flag.' %
-                    len(serials))
-            serial = serials[0]
+                    'Expected one phone, but %d found. Use the -s flag or '
+                    'specify ANDROID_SERIAL.' % len(serials))
         if serial not in serials:
             raise Error('Device "%s" is not found by adb.' % serial)
         ads = android_device.get_instances([serial])
         assert len(ads) == 1
         self._ad = ads[0]
 
     def start_console(self):
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/sl4a_client.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/sl4a_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
     def start_app_and_connect(self):
         """Overrides superclass."""
         # Check that sl4a is installed
         out = self._adb.shell('pm list package')
         if not utils.grep('com.googlecode.android_scripting', out):
             raise jsonrpc_client_base.AppStartError(
-                self._ad, '%s is not installed on %s' % (_APP_NAME,
-                                                         self._adb.serial))
+                self._ad,
+                '%s is not installed on %s' % (_APP_NAME, self._adb.serial))
         self.disable_hidden_api_blacklist()
 
         # sl4a has problems connecting after disconnection, so kill the apk and
         # try connecting again.
         try:
             self.stop_app()
         except Exception as e:
@@ -141,28 +141,27 @@
         while time.time() < expiration_time:
             self.log.debug('Attempting to start %s.', self.app_name)
             try:
                 self.connect()
                 started = True
                 break
             except:
-                self.log.debug(
-                    '%s is not yet running, retrying',
-                    self.app_name,
-                    exc_info=True)
+                self.log.debug('%s is not yet running, retrying',
+                               self.app_name,
+                               exc_info=True)
             time.sleep(1)
         if not started:
             raise jsonrpc_client_base.AppRestoreConnectionError(
                 self._ad, '%s failed to connect for %s at host port %s, '
                 'device port %s' % (self.app_name, self._adb.serial,
                                     self.host_port, self.device_port))
 
     def _start_event_client(self):
         # Start an EventDispatcher for the current sl4a session
         event_client = Sl4aClient(self._ad)
         event_client.host_port = self.host_port
         event_client.device_port = self.device_port
-        event_client.connect(
-            uid=self.uid, cmd=jsonrpc_client_base.JsonRpcCommand.CONTINUE)
+        event_client.connect(uid=self.uid,
+                             cmd=jsonrpc_client_base.JsonRpcCommand.CONTINUE)
         ed = event_dispatcher.EventDispatcher(event_client)
         ed.start()
         return ed
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/callback_handler.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/callback_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,16 @@
             raw_event = self._event_client.eventWaitAndGet(
                 self._id, event_name, timeout_ms)
         except Exception as e:
             if 'EventSnippetException: timeout.' in str(e):
                 raise TimeoutError(
                     self._ad,
                     'Timed out after waiting %ss for event "%s" triggered by'
-                    ' %s (%s).' % (timeout, event_name, self._method_name,
-                                   self._id))
+                    ' %s (%s).' %
+                    (timeout, event_name, self._method_name, self._id))
             raise
         return snippet_event.from_dict(raw_event)
 
     def waitForEvent(self, event_name, predicate, timeout=DEFAULT_TIMEOUT):
         """Wait for an event of a specific name that satisfies the predicate.
 
         This call will block until the expected event has been received or time
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/errors.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/errors.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/snippet_client.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/snippet_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """JSON RPC interface to Mobly Snippet Lib."""
 
+from __future__ import print_function
+
 import re
 import time
 
 from mobly import utils
 from mobly.controllers.android_device_lib import adb
 from mobly.controllers.android_device_lib import errors
 from mobly.controllers.android_device_lib import jsonrpc_client_base
@@ -36,16 +38,16 @@
 # protocol that are backwards compatible with the old protocol and don't break
 # existing clients.
 _PROTOCOL_MINOR_VERSION = 0
 
 _LAUNCH_CMD = ('%s am instrument -w -e action start %s/' +
                _INSTRUMENTATION_RUNNER_PACKAGE)
 
-_STOP_CMD = (
-    'am instrument -w -e action stop %s/' + _INSTRUMENTATION_RUNNER_PACKAGE)
+_STOP_CMD = ('am instrument -w -e action stop %s/' +
+             _INSTRUMENTATION_RUNNER_PACKAGE)
 
 # Test that uses UiAutomation requires the shell session to be maintained while
 # test is in progress. However, this requirement does not hold for the test that
 # deals with device USB disconnection (Once device disconnects, the shell
 # session that started the instrument ends, and UiAutomation fails with error:
 # "UiAutomation not connected"). To keep the shell session and redirect
 # stdin/stdout/stderr, use "setsid" or "nohup" while launching the
@@ -205,16 +207,16 @@
             self.connect()
         except:
             # Log the original error and raise AppRestoreConnectionError.
             self.log.exception('Failed to re-connect to app.')
             raise jsonrpc_client_base.AppRestoreConnectionError(
                 self._ad,
                 ('Failed to restore app connection for %s at host port %s, '
-                 'device port %s') % (self.package, self.host_port,
-                                      self.device_port))
+                 'device port %s') %
+                (self.package, self.host_port, self.device_port))
 
         # Because the previous connection was lost, update self._proc
         self._proc = None
         self._restore_event_client()
 
     def stop_app(self):
         # Kill the pending 'adb shell am instrument -w' process if there is one.
@@ -260,17 +262,17 @@
         # Check that the Mobly Snippet app is installed.
         out = self._adb.shell('pm list package')
         if not utils.grep('^package:%s$' % self.package, out):
             raise AppStartPreCheckError(self._ad,
                                         '%s is not installed.' % self.package)
         # Check that the app is instrumented.
         out = self._adb.shell('pm list instrumentation')
-        matched_out = utils.grep('^instrumentation:%s/%s' %
-                                 (self.package,
-                                  _INSTRUMENTATION_RUNNER_PACKAGE), out)
+        matched_out = utils.grep(
+            '^instrumentation:%s/%s' %
+            (self.package, _INSTRUMENTATION_RUNNER_PACKAGE), out)
         if not matched_out:
             raise AppStartPreCheckError(
                 self._ad,
                 '%s is installed, but it is not instrumented.' % self.package)
         match = re.search(r'^instrumentation:(.*)\/(.*) \(target=(.*)\)$',
                           matched_out[0])
         target_name = match.group(3)
@@ -332,7 +334,27 @@
                 continue
         self.log.warning(
             'No %s and %s commands available to launch instrument '
             'persistently, tests that depend on UiAutomator and '
             'at the same time performs USB disconnection may fail',
             _SETSID_COMMAND, _NOHUP_COMMAND)
         return ''
+
+    def help(self, print_output=True):
+        """Calls the help RPC, which returns the list of RPC calls available.
+
+        This RPC should normally be used in an interactive console environment
+        where the output should be printed instead of returned. Otherwise,
+        newlines will be escaped, which will make the output difficult to read.
+
+        Args:
+            print_output: A bool for whether the output should be printed.
+
+        Returns:
+            A str containing the help output otherwise None if print_output
+                wasn't set.
+        """
+        help_text = self._rpc('help')
+        if print_output:
+            print(help_text)
+        else:
+            return help_text
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/adb.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/adb.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,29 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from builtins import str
 from past.builtins import basestring
 
 import logging
-import pipes
 import psutil
 import subprocess
+import time
 import threading
 
+from mobly import utils
+
 # Command to use for running ADB commands.
 ADB = 'adb'
 
 # adb gets confused if we try to manage bound ports in parallel, so anything to
 # do with port forwarding must happen under this lock.
 ADB_PORT_LOCK = threading.Lock()
 
 # Qualified class name of the default instrumentation test runner.
 DEFAULT_INSTRUMENTATION_RUNNER = 'com.android.common.support.test.runner.AndroidJUnitRunner'
 
+# Adb getprop call should never take too long.
+DEFAULT_GETPROP_TIMEOUT_SEC = 5
+DEFAULT_GETPROPS_ATTEMPTS = 3
+DEFAULT_GETPROPS_RETRY_SLEEP_SEC = 1
+
 
 class Error(Exception):
     """Base error type for adb proxy module."""
 
 
 class AdbError(Error):
     """Raised when an adb command encounters an error.
@@ -54,16 +61,16 @@
         self.stdout = stdout
         self.stderr = stderr
         self.ret_code = ret_code
         self.serial = serial
 
     def __str__(self):
         return ('Error executing adb cmd "%s". ret: %d, stdout: %s, stderr: %s'
-                ) % (cli_cmd_to_string(self.cmd), self.ret_code, self.stdout,
-                     self.stderr)
+                ) % (utils.cli_cmd_to_string(
+                    self.cmd), self.ret_code, self.stdout, self.stderr)
 
 
 class AdbTimeoutError(Error):
     """Raised when an command did not complete within expected time.
 
     Args:
         cmd: list of strings, the adb command that timed out
@@ -76,15 +83,15 @@
     def __init__(self, cmd, timeout, serial=''):
         self.cmd = cmd
         self.timeout = timeout
         self.serial = serial
 
     def __str__(self):
         return 'Timed out executing command "%s" after %ss.' % (
-            cli_cmd_to_string(self.cmd), self.timeout)
+            utils.cli_cmd_to_string(self.cmd), self.timeout)
 
 
 def list_occupied_adb_ports():
     """Lists all the host ports occupied by adb forward.
 
     This is useful because adb will silently override the binding if an attempt
     to bind to a port already used by adb was made, instead of throwing binding
@@ -101,29 +108,14 @@
         tokens = line.split(' tcp:')
         if len(tokens) != 3:
             continue
         used_ports.append(int(tokens[1]))
     return used_ports
 
 
-def cli_cmd_to_string(args):
-    """Converts a cmd arg list to string.
-
-    Args:
-        args: list of strings, the arguments of a command.
-
-    Returns:
-        String representation of the command.
-    """
-    if isinstance(args, basestring):
-        # Return directly if it's already a string.
-        return args
-    return ' '.join([pipes.quote(arg) for arg in args])
-
-
 class AdbProxy(object):
     """Proxy class for ADB.
 
     For syntactic reasons, the '-' in adb commands need to be replaced with
     '_'. Can directly execute adb commands on an object:
     >> adb = AdbProxy(<serial>)
     >> adb.start_server()
@@ -163,42 +155,37 @@
             The output of the adb command run if exit code is 0.
 
         Raises:
             ValueError: timeout value is invalid.
             AdbError: The adb command exit code is not 0.
             AdbTimeoutError: The adb command timed out.
         """
-        proc = subprocess.Popen(
-            args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=shell)
-        process = psutil.Process(proc.pid)
         if timeout and timeout <= 0:
             raise ValueError('Timeout is not a positive value: %s' % timeout)
-        if timeout and timeout > 0:
-            try:
-                process.wait(timeout=timeout)
-            except psutil.TimeoutExpired:
-                process.terminate()
-                raise AdbTimeoutError(
-                    cmd=args, timeout=timeout, serial=self.serial)
+        try:
+            (ret, out, err) = utils.run_command(args,
+                                                shell=shell,
+                                                timeout=timeout)
+        except psutil.TimeoutExpired:
+            raise AdbTimeoutError(cmd=args,
+                                  timeout=timeout,
+                                  serial=self.serial)
 
-        (out, err) = proc.communicate()
         if stderr:
             stderr.write(err)
-        ret = proc.returncode
         logging.debug('cmd: %s, stdout: %s, stderr: %s, ret: %s',
-                      cli_cmd_to_string(args), out, err, ret)
+                      utils.cli_cmd_to_string(args), out, err, ret)
         if ret == 0:
             return out
         else:
-            raise AdbError(
-                cmd=args,
-                stdout=out,
-                stderr=err,
-                ret_code=ret,
-                serial=self.serial)
+            raise AdbError(cmd=args,
+                           stdout=out,
+                           stderr=err,
+                           ret_code=ret,
+                           serial=self.serial)
 
     def _execute_and_process_stdout(self, args, shell, handler):
         """Executes adb commands and processes the stdout with a handler.
 
         Args:
             args: string or list of strings, program arguments.
                 See subprocess.Popen() documentation.
@@ -208,20 +195,19 @@
 
         Returns:
             The stderr of the adb command run if exit code is 0.
 
         Raises:
             AdbError: The adb command exit code is not 0.
         """
-        proc = subprocess.Popen(
-            args,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            shell=shell,
-            bufsize=1)
+        proc = subprocess.Popen(args,
+                                stdout=subprocess.PIPE,
+                                stderr=subprocess.PIPE,
+                                shell=shell,
+                                bufsize=1)
         out = '[elided, processed via handler]'
         try:
             # Even if the process dies, stdout.readline still works
             # and will continue until it runs out of stdout to process.
             while True:
                 line = proc.stdout.readline()
                 if line:
@@ -234,15 +220,15 @@
             if unexpected_out:
                 out = '[unexpected stdout] %s' % unexpected_out
                 for line in unexpected_out.splitlines():
                     handler(line)
 
         ret = proc.returncode
         logging.debug('cmd: %s, stdout: %s, stderr: %s, ret: %s',
-                      cli_cmd_to_string(args), out, err, ret)
+                      utils.cli_cmd_to_string(args), out, err, ret)
         if ret == 0:
             return err
         else:
             raise AdbError(cmd=args, stdout=out, stderr=err, ret_code=ret)
 
     def _construct_adb_cmd(self, raw_name, args, shell):
         """Constructs an adb command with arguments for a subprocess call.
@@ -259,15 +245,15 @@
             The adb command in a format appropriate for subprocess. If shell is
                 True, then this is a string; otherwise, this is a list of
                 strings.
         """
         args = args or ''
         name = raw_name.replace('_', '-')
         if shell:
-            args = cli_cmd_to_string(args)
+            args = utils.cli_cmd_to_string(args)
             # Add quotes around "adb" in case the ADB path contains spaces. This
             # is pretty common on Windows (e.g. Program Files).
             if self.serial:
                 adb_cmd = '"%s" -s "%s" %s %s' % (ADB, self.serial, name, args)
             else:
                 adb_cmd = '"%s" %s %s' % (ADB, name, args)
         else:
@@ -280,37 +266,100 @@
                     adb_cmd.append(args)
                 else:
                     adb_cmd.extend(args)
         return adb_cmd
 
     def _exec_adb_cmd(self, name, args, shell, timeout, stderr):
         adb_cmd = self._construct_adb_cmd(name, args, shell=shell)
-        out = self._exec_cmd(
-            adb_cmd, shell=shell, timeout=timeout, stderr=stderr)
+        out = self._exec_cmd(adb_cmd,
+                             shell=shell,
+                             timeout=timeout,
+                             stderr=stderr)
         return out
 
     def _execute_adb_and_process_stdout(self, name, args, shell, handler):
         adb_cmd = self._construct_adb_cmd(name, args, shell=shell)
-        out = self._execute_and_process_stdout(
-            adb_cmd, shell=shell, handler=handler)
+        out = self._execute_and_process_stdout(adb_cmd,
+                                               shell=shell,
+                                               handler=handler)
         return out
 
+    def _parse_getprop_output(self, output):
+        """Parses the raw output of `adb shell getprop` into a dictionary.
+
+        Args:
+            output: byte str, the raw output of the `adb shell getprop` call.
+
+        Returns:
+            dict, name-value pairs of the properties.
+        """
+        output = output.decode('utf-8', errors='ignore').replace('\r\n', '\n')
+        results = {}
+        for line in output.split(']\n'):
+            if not line:
+                continue
+            try:
+                name, value = line.split(': ', 1)
+            except ValueError:
+                logging.debug('Failed to parse adb getprop line %s', line)
+                continue
+            name = name.strip()[1:-1]
+            # Remove any square bracket from either end of the value string.
+            if value and value[0] == '[':
+                value = value[1:]
+            results[name] = value
+        return results
+
     def getprop(self, prop_name):
         """Get a property of the device.
 
-        This is a convenience wrapper for "adb shell getprop xxx".
+        This is a convenience wrapper for `adb shell getprop xxx`.
 
         Args:
             prop_name: A string that is the name of the property to get.
 
         Returns:
             A string that is the value of the property, or None if the property
             doesn't exist.
         """
-        return self.shell('getprop %s' % prop_name).decode('utf-8').strip()
+        return self.shell(
+            ['getprop', prop_name],
+            timeout=DEFAULT_GETPROP_TIMEOUT_SEC).decode('utf-8').strip()
+
+    def getprops(self, prop_names):
+        """Get multiple properties of the device.
+
+        This is a convenience wrapper for `adb shell getprop`. Use this to
+        reduce the number of adb calls when getting multiple properties.
+
+        Args:
+            prop_names: list of strings, the names of the properties to get.
+
+        Returns:
+            A dict containing name-value pairs of the properties requested, if
+            they exist.
+        """
+        attempts = DEFAULT_GETPROPS_ATTEMPTS
+        results = {}
+        for attempt in range(attempts):
+            # The ADB getprop command can randomly return empty string, so try
+            # multiple times. This value should always be non-empty if the device
+            # in a working state.
+            raw_output = self.shell(['getprop'],
+                                    timeout=DEFAULT_GETPROP_TIMEOUT_SEC)
+            properties = self._parse_getprop_output(raw_output)
+            if properties:
+                for name in prop_names:
+                    if name in properties:
+                        results[name] = properties[name]
+                break
+            # Don't call sleep on the last attempt.
+            if attempt < attempts - 1:
+                time.sleep(DEFAULT_GETPROPS_RETRY_SLEEP_SEC)
+        return results
 
     def has_shell_command(self, command):
         """Checks to see if a given check command exists on the device.
 
         Args:
             command: A string that is the name of the command to check.
 
@@ -324,16 +373,19 @@
         except AdbError:
             # If the command doesn't exist, then 'command -v' can return
             # an exit code > 1.
             return False
 
     def forward(self, args=None, shell=False):
         with ADB_PORT_LOCK:
-            return self._exec_adb_cmd(
-                'forward', args, shell, timeout=None, stderr=None)
+            return self._exec_adb_cmd('forward',
+                                      args,
+                                      shell,
+                                      timeout=None,
+                                      stderr=None)
 
     def instrument(self, package, options=None, runner=None, handler=None):
         """Runs an instrumentation command on the device.
 
         This is a convenience wrapper to avoid parameter formatting.
 
         Example:
@@ -374,20 +426,19 @@
 
         instrumentation_command = 'am instrument -r -w %s %s/%s' % (
             options_string, package, runner)
         logging.info('AndroidDevice|%s: Executing adb shell %s', self.serial,
                      instrumentation_command)
         if handler is None:
             # Flow kept for backwards-compatibility reasons
-            self._exec_adb_cmd(
-                'shell',
-                instrumentation_command,
-                shell=False,
-                timeout=None,
-                stderr=None)
+            self._exec_adb_cmd('shell',
+                               instrumentation_command,
+                               shell=False,
+                               timeout=None,
+                               stderr=None)
         else:
             return self._execute_adb_and_process_stdout(
                 'shell', instrumentation_command, shell=False, handler=handler)
 
     def __getattr__(self, name):
         def adb_call(args=None, shell=False, timeout=None, stderr=None):
             """Wrapper for an ADB command.
@@ -401,11 +452,14 @@
                     If not specified, no timeout takes effect.
                 stderr: a Byte stream, like io.BytesIO, stderr of the command
                     will be written to this object if provided.
 
             Returns:
                 The output of the adb command run if exit code is 0.
             """
-            return self._exec_adb_cmd(
-                name, args, shell=shell, timeout=timeout, stderr=stderr)
+            return self._exec_adb_cmd(name,
+                                      args,
+                                      shell=shell,
+                                      timeout=timeout,
+                                      stderr=stderr)
 
         return adb_call
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/services/logcat.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/services/logcat.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 class Config(object):
     """Config object for logcat service.
 
     Attributes:
         clear_log: bool, clears the logcat before collection if True.
         logcat_params: string, extra params to be added to logcat command.
         output_file_path: string, the path on the host to write the log file
-            to. The service will automatically generate one if not specified.
+            to, including the actual filename. The service will automatically
+            generate one if not specified.
     """
 
     def __init__(self,
                  logcat_params=None,
                  clear_log=True,
                  output_file_path=None):
         self.clear_log = clear_log
@@ -57,15 +58,17 @@
     """
 
     def __init__(self, android_device, configs=None):
         super(Logcat, self).__init__(android_device, configs)
         self._ad = android_device
         self._adb_logcat_process = None
         self.adb_logcat_file_path = None
-        self._configs = configs if configs else Config()
+        # Logcat service uses a single config obj, using singular internal
+        # name: `_config`.
+        self._config = configs if configs else Config()
 
     def _enable_logpersist(self):
         """Attempts to enable logpersist daemon to persist logs."""
         # Logpersist is only allowed on rootable devices because of excessive
         # reads/writes for persisting logs.
         if not self._ad.is_rootable:
             return
@@ -105,30 +108,30 @@
 
         Args:
           current_test_info: `self.current_test_info` in a Mobly test.
         """
         self.pause()
         dest_path = current_test_info.output_path
         utils.create_dir(dest_path)
-        self._ad.log.debug('AdbLog exceprt location: %s', dest_path)
+        self._ad.log.debug('AdbLog excerpt location: %s', dest_path)
         shutil.move(self.adb_logcat_file_path, dest_path)
         self.resume()
 
     @property
     def is_alive(self):
         return True if self._adb_logcat_process else False
 
     def clear_adb_log(self):
         """Clears cached adb content."""
         try:
             self._ad.adb.logcat('-c')
         except adb.AdbError as e:
             # On Android O, the clear command fails due to a known bug.
             # Catching this so we don't crash from this Android issue.
-            if "failed to clear" in e.stderr:
+            if b'failed to clear' in e.stderr:
                 self._ad.log.warning(
                     'Encountered known Android error to clear logcat.')
             else:
                 raise
 
     def cat_adb_log(self, tag, begin_time):
         """Takes an excerpt of the adb logcat log from a certain time point to
@@ -153,16 +156,16 @@
         out_name = out_name.replace(':', '-')
         tag_len = utils.MAX_FILENAME_LEN - len(out_name)
         tag = tag[:tag_len]
         out_name = tag + out_name
         full_adblog_path = os.path.join(adb_excerpt_path, out_name)
         with io.open(full_adblog_path, 'w', encoding='utf-8') as out:
             in_file = self.adb_logcat_file_path
-            with io.open(
-                    in_file, 'r', encoding='utf-8', errors='replace') as f:
+            with io.open(in_file, 'r', encoding='utf-8',
+                         errors='replace') as f:
                 in_range = False
                 while True:
                     line = None
                     try:
                         line = f.readline()
                         if not line:
                             break
@@ -188,35 +191,52 @@
             Error, if the logcat service is running.
         """
         if self.is_alive:
             raise Error(
                 self._ad,
                 'Logcat thread is already running, cannot start another one.')
 
+    def update_config(self, new_config):
+        """Updates the configuration for the service.
+
+        The service needs to be stopped before updating, and explicitly started
+        after the update.
+
+        This will reset the service. Previous output files may be orphaned if
+        output path is changed.
+
+        Args:
+            new_config: Config, the new config to use.
+        """
+        self._assert_not_running()
+        self._ad.log.info('[LogcatService] Changing config from %s to %s',
+                          self._config, new_config)
+        self._config = new_config
+
     def start(self):
         """Starts a standing adb logcat collection.
 
         The collection runs in a separate subprocess and saves logs in a file.
         """
         self._assert_not_running()
-        if self._configs.clear_log:
+        if self._config.clear_log:
             self.clear_adb_log()
         self._start()
 
     def _start(self):
         """The actual logic of starting logcat."""
         self._enable_logpersist()
-        logcat_file_path = self._configs.output_file_path
+        logcat_file_path = self._config.output_file_path
         if not logcat_file_path:
             f_name = 'adblog,%s,%s.txt' % (self._ad.model,
                                            self._ad._normalized_serial)
             logcat_file_path = os.path.join(self._ad.log_path, f_name)
         utils.create_dir(os.path.dirname(logcat_file_path))
         cmd = '"%s" -s %s logcat -v threadtime %s >> "%s"' % (
-            adb.ADB, self._ad.serial, self._configs.logcat_params,
+            adb.ADB, self._ad.serial, self._config.logcat_params,
             logcat_file_path)
         process = utils.start_standing_subprocess(cmd, shell=True)
         self._adb_logcat_process = process
         self.adb_logcat_file_path = logcat_file_path
 
     def stop(self):
         """Stops the adb logcat service."""
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/services/__init__.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/services/sl4a_service.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/services/sl4a_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     Direct calls on the service object will forwarded to the client object as
     syntactic sugar. So `Sl4aService.doFoo()` is equivalent to
     `Sl4aClient.doFoo()`.
     """
 
     def __init__(self, device, configs=None):
-        del configs # Never used.
+        del configs  # Never used.
         self._ad = device
         self._sl4a_client = None
 
     @property
     def is_alive(self):
         return self._sl4a_client is not None
```

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/services/base_service.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/services/base_service.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly/controllers/android_device_lib/services/snippet_management_service.py` & `mobly-1.9.1/mobly/controllers/android_device_lib/services/snippet_management_service.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly/controllers/monsoon.py` & `mobly-1.9.1/mobly/controllers/monsoon.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     elif isinstance(configs[0], dict):
         # Configs is a list of dicts.
         objs = get_instances_with_configs(configs)
     elif isinstance(configs[0], int):
         # Configs is a list of ints representing serials.
         objs = get_instances(configs)
     else:
-        raise Error('No valid config found in: %s' % configs)
+        raise Exception('No valid config found in: %s' % configs)
     return objs
 
 
 def get_instances_with_configs(configs):
     """Create Monsoon instances from a list of dict configs.
 
     Each config should have the required key-value pair
@@ -375,16 +375,16 @@
                 self._coarse_ref = data[1][0]
             else:
                 logging.warning("Discarding data packet type=0x%02x", _type)
                 continue
 
             # See http://wiki/Main/MonsoonProtocol for details on these values.
             if self._coarse_ref != self._coarse_zero:
-                self._coarse_scale = 2.88 / (
-                    self._coarse_ref - self._coarse_zero)
+                self._coarse_scale = 2.88 / (self._coarse_ref -
+                                             self._coarse_zero)
             if self._fine_ref != self._fine_zero:
                 self._fine_scale = 0.0332 / (self._fine_ref - self._fine_zero)
 
     def _SendStruct(self, fmt, *args):
         """Pack a struct (without length or checksum) and send it.
         """
         data = struct.pack(fmt, *args)
@@ -522,15 +522,15 @@
             lines[5] != "Time" + ' ' * 7 + "Amp"
         ]
         if any(conditions):
             raise MonsoonError(err_msg)
         hz_str = lines[4].split()[2]
         hz = int(hz_str[:-2])
         voltage_str = lines[2].split()[1]
-        voltage = int(voltage[:-1])
+        voltage = int(voltage_str[:-1])
         lines = lines[6:]
         t = []
         v = []
         for l in lines:
             try:
                 timestamp, value = l.split(' ')
                 t.append(int(timestamp))
@@ -686,28 +686,28 @@
 
         Args:
             volt: Voltage to set the output to.
             ramp: If true, the output voltage will be increased gradually to
                 prevent tripping Monsoon overvoltage.
         """
         if ramp:
-            self.mon.RampVoltage(mon.start_voltage, volt)
+            self.mon.RampVoltage(self.mon.start_voltage, volt)
         else:
             self.mon.SetVoltage(volt)
 
     def set_max_current(self, cur):
         """Sets monsoon's max output current.
 
         Args:
             cur: The max current in A.
         """
         self.mon.SetMaxCurrent(cur)
 
     def set_max_init_current(self, cur):
-        """Sets the max power-up/inital current.
+        """Sets the max power-up/initial current.
 
         Args:
             cur: The max initial current allowed in mA.
         """
         self.mon.SetMaxPowerUpCurrent(cur)
 
     @property
@@ -794,20 +794,19 @@
                     if now - last_flush >= 0.99:  # flush every second
                         sys.stdout.flush()
                         last_flush = now
         except Exception as e:
             pass
         self.mon.StopDataCollection()
         try:
-            return MonsoonData(
-                current_values,
-                timestamps,
-                sample_hz,
-                voltage,
-                offset=sample_offset)
+            return MonsoonData(current_values,
+                               timestamps,
+                               sample_hz,
+                               voltage,
+                               offset=sample_offset)
         except:
             return None
 
     @timeout_decorator.timeout(60, use_signals=False)
     def usb(self, state):
         """Sets the monsoon's USB passthrough mode. This is specific to the
         USB port in front of the monsoon box which connects to the powered
```

### Comparing `mobly-1.8.1/mobly/controllers/attenuator.py` & `mobly-1.9.1/mobly/controllers/attenuator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Controller module for attenuators.
```

### Comparing `mobly-1.8.1/mobly/controllers/attenuator_lib/telnet_scpi_client.py` & `mobly-1.9.1/mobly/controllers/attenuator_lib/telnet_scpi_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Helper module for common telnet capability to communicate with
@@ -27,14 +27,15 @@
 
 
 class TelnetScpiClient(object):
     """This is an internal helper class for Telnet+SCPI command-based
     instruments. It should only be used by those implemention control libraries
     and not by any user code directly.
     """
+
     def __init__(self, tx_cmd_separator="\n", rx_cmd_separator="\n",
                  prompt=""):
         self._tn = None
         self.tx_cmd_separator = tx_cmd_separator
         self.rx_cmd_separator = rx_cmd_separator
         self.prompt = prompt
         self.host = None
@@ -73,11 +74,11 @@
             [_ascii_string("\S+" + self.rx_cmd_separator)], 1)
 
         if match_idx == -1:
             raise attenuator.Error(
                 "Telnet command failed to return valid data")
 
         ret_text = ret_text.decode()
-        ret_text = ret_text.strip(self.tx_cmd_separator + self.rx_cmd_separator
-                                  + self.prompt)
+        ret_text = ret_text.strip(self.tx_cmd_separator +
+                                  self.rx_cmd_separator + self.prompt)
 
         return ret_text
```

### Comparing `mobly-1.8.1/mobly/controllers/attenuator_lib/minicircuits.py` & `mobly-1.9.1/mobly/controllers/attenuator_lib/minicircuits.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """
 This module has the class for controlling Mini-Circuits RCDAT series
 attenuators over Telnet.
 
 See http://www.minicircuits.com/softwaredownload/Prog_Manual-6-Programmable_Attenuator.pdf
 """
 
@@ -26,14 +25,15 @@
 class AttenuatorDevice(object):
     """This provides a specific telnet-controlled implementation of
     AttenuatorDevice for Mini-Circuits RC-DAT attenuators.
 
     Attributes:
         path_count: The number of signal attenuation path this device has.
     """
+
     def __init__(self, path_count=1):
         self.path_count = path_count
         # The telnet client used to communicate with the attenuator device.
         self._telnet_client = telnet_scpi_client.TelnetScpiClient(
             tx_cmd_separator="\r\n", rx_cmd_separator="\r\n", prompt="")
 
     @property
```

### Comparing `mobly-1.8.1/mobly/controllers/sniffer.py` & `mobly-1.9.1/mobly/controllers/sniffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2016 Google Inc.
-# 
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
-# 
+#
 #     http://www.apache.org/licenses/LICENSE-2.0
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import importlib
@@ -37,17 +37,18 @@
         sniffer_type = c["Type"]
         sniffer_subtype = c["SubType"]
         interface = c["Interface"]
         base_configs = c["BaseConfigs"]
         module_name = "mobly.controllers.sniffer_lib.{}.{}".format(
             sniffer_type, sniffer_subtype)
         module = importlib.import_module(module_name)
-        objs.append(module.Sniffer(interface,
-                                   logging.getLogger(),
-                                   base_configs=base_configs))
+        objs.append(
+            module.Sniffer(interface,
+                           logging.getLogger(),
+                           base_configs=base_configs))
     return objs
 
 
 def destroy(objs):
     """Destroys the sniffers and terminates any ongoing capture sessions.
     """
     for sniffer in objs:
```

### Comparing `mobly-1.8.1/mobly/base_instrumentation_test.py` & `mobly-1.9.1/mobly/base_instrumentation_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     TEST = 'test'
     STREAM = 'stream'
 
 
 class _InstrumentationStatusCodes(object):
     """A mapping of instrumentation status codes to test method results.
 
-    When instrumentation runs, at various points ouput is created in a serias
+    When instrumentation runs, at various points output is created in a series
     of blocks that terminate as follows:
 
     .. code-block:: none
 
         INSTRUMENTATION_STATUS_CODE: 1
 
     These blocks typically have several status keys in them, and they indicate
@@ -167,15 +167,15 @@
     methods, a result line will appear as follows:
 
     .. code-block:: none
 
         INSTRUMENTATION_RESULT:
 
     If something wrong happened during the instrumentation run such as an
-    application under test crash, the the line will appear similarly as thus:
+    application under test crash, the line will appear similarly as thus:
 
     .. code-block:: none
 
         INSTRUMENTATION_RESULT: shortMsg=Process crashed.
 
     Since these keys indicate that something wrong has happened to the
     instrumentation run, they should be checked for explicitly.
@@ -223,15 +223,15 @@
     FAIL = 'FAILURES!!!'
     PASS = 'OK ('
 
 
 class _InstrumentationBlockStates(Enum):
     """States used for determing what the parser is currently parsing.
 
-    The parse always starts and ends a block in the UKNOWN state, which is
+    The parse always starts and ends a block in the UNKNOWN state, which is
     used to indicate that either a method or a result block (matching the
     METHOD and RESULT states respectively) are valid follow ups, which means
     that parser should be checking for a structure prefix that indicates which
     of those two states it should transition to. If the parser is in the
     METHOD state, then the parser will be parsing input into test methods.
     Otherwise, the parse can simply concatenate all the input to check for
     some final run completion signals.
@@ -269,15 +269,15 @@
     .. code-block:: none
 
       INSTRUMENTATION_STATUS: stack=...
       ...
 
     Because these keys are poentially very long, constant string contatention
     is potentially inefficent. Instead, this class builds up a buffer to store
-    the raw ouput until it is processed into an actual test result by the
+    the raw output until it is processed into an actual test result by the
     _InstrumentationBlockFormatter class.
 
     Additionally, this class also serves to store the parser state, which
     means that the BaseInstrumentationTestClass does not need to keep any
     potentially volatile instrumentation related state, so multiple
     instrumentation runs should have completely separate parsing states.
 
@@ -392,15 +392,15 @@
 
         For unknown keys, the key is added to the value list in order to
         better contextualize the value in the output.
 
         Args:
             structure_prefix: string, the structure prefix that was matched
                 and that needs to be removed.
-            key_line: string, the raw instrumentation ouput line that contains
+            key_line: string, the raw instrumentation output line that contains
                 the key-value pair.
         """
         self._empty = False
         key_value = self._remove_structure_prefix(
             structure_prefix,
             key_line,
         )
@@ -443,15 +443,15 @@
             new_state: _InstrumentationBlockStates, the state that the parser
                 should transition to.
 
         Returns:
             A new instrumentation block set to the new state, representing
             the start of parsing a new instrumentation test method.
             Alternatively, if the current instrumentation block represents the
-            start of parsing a new instrumentation block (state UKNOWN), then
+            start of parsing a new instrumentation block (state UNKNOWN), then
             this returns the current instrumentation block set to the now
             known parsing state.
         """
         if self.state == _InstrumentationBlockStates.UNKNOWN:
             self.state = new_state
             return self
         else:
@@ -524,15 +524,15 @@
             instrumentation test method. If parts are missing, then degrades
             steadily.
         """
         full_name_parts = [self._get_class(), self._get_name()]
         return '#'.join(filter(None, full_name_parts))
 
     def _get_details(self):
-        """Gets the ouput for the detail section of the TestResultRecord.
+        """Gets the output for the detail section of the TestResultRecord.
 
         Returns:
             A string to set for a TestResultRecord's details.
         """
         detail_parts = [self._get_full_name(), self._error_message]
         return '\n'.join(filter(None, detail_parts))
 
@@ -655,19 +655,22 @@
             return True
         elif _InstrumentationResultSignals.FAIL in extras:
             return False
         else:
             raise signals.TestError(details=error_message, extras=extras)
 
 
-class BaseInstrumentationTestClass(base_test.BaseTestClass):
-    """Base class for all instrumentation test claseses to inherit from.
+class InstrumentationTestMixin(object):
+    """A mixin for Mobly test classes to inherit from for instrumentation tests.
 
-    This class extends the BaseTestClass to add functionality to run and parse
-    the output of instrumentation runs.
+    This class should be used in a subclass of both BaseTestClass and this class
+    in order to provide instrumentation test capabilities. This mixin is
+    explicitly for the case where the underlying BaseTestClass cannot be
+    replaced with BaseInstrumentationTestClass. In general, prefer using
+    BaseInstrumentationTestClass instead.
 
     Attributes:
         DEFAULT_INSTRUMENTATION_OPTION_PREFIX: string, the default prefix for
             instrumentation params contained within user params.
         DEFAULT_INSTRUMENTATION_ERROR_MESSAGE: string, the default error
             message to set if something has prevented something in the
             instrumentation test run from completing properly.
@@ -747,15 +750,15 @@
             instrumentation_block: _InstrumentationBlock, the current
                 instrumentation block to finish.
             new_state: _InstrumentationBlockState, the next state for the
                 parser to transition to.
 
         Returns:
             The new instrumentation block to use for storing parsed
-            instrumentation ouput.
+            instrumentation output.
         """
         formatters = self._create_formatters(instrumentation_block, new_state)
         for formatter in formatters:
             test_record = formatter.create_test_record(self.TAG)
             if test_record:
                 self.results.add_record(test_record)
                 self.summary_writer.dump(test_record.to_dict(),
@@ -848,15 +851,15 @@
             )
         else:
             # This would only really execute if instrumentation failed to start.
             instrumentation_block.add_value(line)
             return instrumentation_block
 
     def _parse_line(self, instrumentation_block, line):
-        """Parses an arbitary line from the instrumentation output based upon
+        """Parses an arbitrary line from the instrumentation output based upon
         the current parser state.
 
         Args:
             instrumentation_block: _InstrumentationBlock, an instrumentation
                 block with any of the possible parser states.
             line: string, the raw instrumentation output line to parse
                 appropriately.
@@ -951,14 +954,29 @@
 
         def parse_instrumentation(raw_line):
             line = raw_line.rstrip().decode('utf-8')
             logging.info(line)
             instrumentation_block[0] = self._parse_line(
                 instrumentation_block[0], line)
 
-        device.adb.instrument(
-            package=package,
-            options=options,
-            runner=runner,
-            handler=parse_instrumentation)
+        device.adb.instrument(package=package,
+                              options=options,
+                              runner=runner,
+                              handler=parse_instrumentation)
 
         return self._finish_parsing(instrumentation_block[0])
+
+
+class BaseInstrumentationTestClass(InstrumentationTestMixin,
+                                   base_test.BaseTestClass):
+    """Base class for all instrumentation test classes to inherit from.
+
+    This class extends the BaseTestClass to add functionality to run and parse
+    the output of instrumentation runs.
+
+    Attributes:
+        DEFAULT_INSTRUMENTATION_OPTION_PREFIX: string, the default prefix for
+            instrumentation params contained within user params.
+        DEFAULT_INSTRUMENTATION_ERROR_MESSAGE: string, the default error
+            message to set if something has prevented something in the
+            instrumentation test run from completing properly.
+    """
```

### Comparing `mobly-1.8.1/tests/mobly/test_suite_test.py` & `mobly-1.9.1/tests/mobly/test_suite_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 
 class TestSuiteTest(unittest.TestCase):
     """Tests for use cases of creating Mobly test suites.
 
     Tests here target a combination of test_runner and base_test code.
     """
-
     def setUp(self):
         self.tmp_dir = tempfile.mkdtemp()
         self.mock_test_cls_configs = config_parser.TestRunConfig()
         self.summary_file = os.path.join(self.tmp_dir, 'summary.yaml')
         self.mock_test_cls_configs.summary_writer = records.TestSummaryWriter(
             self.summary_file)
         self.mock_test_cls_configs.log_path = self.tmp_dir
@@ -65,15 +64,16 @@
 
         class BarTest(base_test.BaseTestClass):
             def setup_class(cls2):
                 self.controller2 = cls2.register_controller(mock_controller)[0]
 
         tr = test_runner.TestRunner(self.tmp_dir,
                                     test_run_config.test_bed_name)
-        tr.add_test_class(test_run_config, FooTest)
-        tr.add_test_class(test_run_config, BarTest)
-        tr.run()
+        with tr.mobly_logger():
+            tr.add_test_class(test_run_config, FooTest)
+            tr.add_test_class(test_run_config, BarTest)
+            tr.run()
         self.assertIsNot(self.controller1, self.controller2)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mobly-1.8.1/tests/mobly/base_instrumentation_test_test.py` & `mobly-1.9.1/tests/mobly/base_instrumentation_test_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/mobly/utils_test.py` & `mobly-1.9.1/tests/mobly/utils_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,63 +33,130 @@
 class UtilsTest(unittest.TestCase):
     """This test class has unit tests for the implementation of everything
     under mobly.utils.
     """
 
     def setUp(self):
         system = platform.system()
-        self.sleep_cmd = 'timeout' if system == 'Windows' else 'sleep'
         self.tmp_dir = tempfile.mkdtemp()
 
     def tearDown(self):
         shutil.rmtree(self.tmp_dir)
 
+    def sleep_cmd(self, wait_secs):
+        if platform.system() == 'Windows':
+            python_code = ['import time', 'time.sleep(%s)' % wait_secs]
+            return ['python', '-c', 'exec("%s")' % r'\r\n'.join(python_code)]
+        else:
+            return ['sleep', str(wait_secs)]
+
+    def test_run_command(self):
+        (ret, out, err) = utils.run_command(self.sleep_cmd(0.01))
+        self.assertEqual(ret, 0)
+
+    def test_run_command_with_timeout(self):
+        (ret, out, err) = utils.run_command(self.sleep_cmd(0.01), timeout=4)
+        self.assertEqual(ret, 0)
+
+    def test_run_command_with_timeout_expired(self):
+        with self.assertRaises(psutil.TimeoutExpired):
+            _ = utils.run_command(self.sleep_cmd(4), timeout=0.01)
+
+    @mock.patch('threading.Timer')
+    @mock.patch('psutil.Popen')
+    def test_run_command_with_default_params(self, mock_Popen, mock_Timer):
+        mock_command = mock.MagicMock(spec=dict)
+        mock_proc = mock_Popen.return_value
+        mock_proc.communicate.return_value = ('fake_out', 'fake_err')
+        mock_proc.returncode = 0
+        out = utils.run_command(mock_command)
+        self.assertEqual(out, (0, 'fake_out', 'fake_err'))
+        mock_Popen.assert_called_with(
+            mock_command,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            shell=False,
+            cwd=None,
+            env=None,
+        )
+        mock_Timer.assert_not_called()
+
+    @mock.patch('threading.Timer')
+    @mock.patch('psutil.Popen')
+    def test_run_command_with_custom_params(self, mock_Popen, mock_Timer):
+        mock_command = mock.MagicMock(spec=dict)
+        mock_stdout = mock.MagicMock(spec=int)
+        mock_stderr = mock.MagicMock(spec=int)
+        mock_shell = mock.MagicMock(spec=bool)
+        mock_timeout = 1234
+        mock_env = mock.MagicMock(spec=dict)
+        mock_proc = mock_Popen.return_value
+        mock_proc.communicate.return_value = ('fake_out', 'fake_err')
+        mock_proc.returncode = 127
+        out = utils.run_command(
+            mock_command,
+            stdout=mock_stdout,
+            stderr=mock_stderr,
+            shell=mock_shell,
+            timeout=mock_timeout,
+            env=mock_env)
+        self.assertEqual(out, (127, 'fake_out', 'fake_err'))
+        mock_Popen.assert_called_with(
+            mock_command,
+            stdout=mock_stdout,
+            stderr=mock_stderr,
+            shell=mock_shell,
+            cwd=None,
+            env=mock_env,
+        )
+        mock_Timer.assert_called_with(1234, mock.ANY)
+
     def test_start_standing_subproc(self):
         try:
-            p = utils.start_standing_subprocess([self.sleep_cmd, '0.1'])
+            p = utils.start_standing_subprocess(self.sleep_cmd(0.01))
             p1 = psutil.Process(p.pid)
             self.assertTrue(p1.is_running())
         finally:
             p.stdout.close()
             p.stderr.close()
             p.wait()
 
     @mock.patch('subprocess.Popen')
     def test_start_standing_subproc_without_env(self, mock_Popen):
-        p = utils.start_standing_subprocess(self.sleep_cmd)
+        p = utils.start_standing_subprocess(self.sleep_cmd(0.01))
         mock_Popen.assert_called_with(
-            self.sleep_cmd,
+            self.sleep_cmd(0.01),
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             shell=False,
             env=None,
         )
 
     @mock.patch('subprocess.Popen')
     def test_start_standing_subproc_with_custom_env(self, mock_Popen):
         mock_env = mock.MagicMock(spec=dict)
-        p = utils.start_standing_subprocess(self.sleep_cmd, env=mock_env)
+        p = utils.start_standing_subprocess(self.sleep_cmd(0.01), env=mock_env)
         mock_Popen.assert_called_with(
-            self.sleep_cmd,
+            self.sleep_cmd(0.01),
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             shell=False,
             env=mock_env,
         )
 
     def test_stop_standing_subproc(self):
-        p = utils.start_standing_subprocess([self.sleep_cmd, '4'])
+        p = utils.start_standing_subprocess(self.sleep_cmd(4))
         p1 = psutil.Process(p.pid)
         utils.stop_standing_subprocess(p)
         self.assertFalse(p1.is_running())
 
     def test_stop_standing_subproc_wihtout_pipe(self):
-        p = subprocess.Popen([self.sleep_cmd, '4'])
+        p = subprocess.Popen(self.sleep_cmd(4))
         self.assertIsNone(p.stdout)
         p1 = psutil.Process(p.pid)
         utils.stop_standing_subprocess(p)
         self.assertFalse(p1.is_running())
 
     def test_create_dir(self):
         new_path = os.path.join(self.tmp_dir, 'haha')
@@ -166,10 +233,16 @@
         expected_base64_encoding = u'6YCa'
         with io.open(tmp_file_path, 'w', encoding='utf-8') as f:
             f.write(u'\u901a')
         self.assertEqual(
             utils.load_file_to_base64_str(tmp_file_path),
             expected_base64_encoding)
 
+    def test_cli_cmd_to_string(self):
+        cmd = ['"adb"', 'a b', 'c//']
+        self.assertEqual(utils.cli_cmd_to_string(cmd), '\'"adb"\' \'a b\' c//')
+        cmd = 'adb -s meme do something ab_cd'
+        self.assertEqual(utils.cli_cmd_to_string(cmd), cmd)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mobly-1.8.1/tests/mobly/asserts_test.py` & `mobly-1.9.1/tests/mobly/asserts_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/mobly/config_parser_test.py` & `mobly-1.9.1/tests/mobly/config_parser_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/mobly/base_test_test.py` & `mobly-1.9.1/tests/mobly/base_test_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,16 @@
 
             def test_never(self):
                 # This should not execute it's not on default test list.
                 never_call()
 
         bt_cls = MockBaseTest(self.mock_test_cls_configs)
         expected_msg = (
-            'Test method name not_a_test_something does not follow '
-            'naming convention test_\*, abort.')
+            r'Test method name not_a_test_something does not follow '
+            r'naming convention test_\*, abort.')
         with self.assertRaisesRegex(base_test.Error, expected_msg):
             bt_cls.run()
 
     def test_cli_test_selection_override_self_tests_list(self):
         class MockBaseTest(base_test.BaseTestClass):
             def __init__(self, controllers):
                 super(MockBaseTest, self).__init__(controllers)
@@ -182,16 +182,16 @@
 
             def test_never(self):
                 # This should not execute it's not selected by cmd line input.
                 never_call()
 
         bt_cls = MockBaseTest(self.mock_test_cls_configs)
         expected_msg = (
-            'Test method name not_a_test_something does not follow '
-            'naming convention test_\*, abort.')
+            r'Test method name not_a_test_something does not follow '
+            r'naming convention test_\*, abort.')
         with self.assertRaisesRegex(base_test.Error, expected_msg):
             bt_cls.run(test_names=["not_a_test_something"])
 
     def test_default_execution_of_all_tests(self):
         class MockBaseTest(base_test.BaseTestClass):
             def test_something(self):
                 pass
@@ -774,15 +774,15 @@
         self.assertEqual(len(actual_record.extra_errors), 1)
         extra_error = actual_record.extra_errors['teardown_test']
         self.assertIs(extra_error.exception, expected_extra_error)
         self.assertIsNotNone(extra_error.stacktrace)
         self.assertIsNone(actual_record.extras)
 
     def test_promote_extra_errors_to_termination_signal(self):
-        """If no termination singal is specified, use the first extra error as
+        """If no termination signal is specified, use the first extra error as
         the termination signal.
         """
         expected_extra_error = Exception('teardown_test Exception.')
 
         class MockBaseTest(base_test.BaseTestClass):
             def teardown_test(self):
                 raise expected_extra_error
@@ -1851,17 +1851,67 @@
             def logic(self, a, b):
                 pass
 
         bt_cls = MockBaseTest(self.mock_test_cls_configs)
         bt_cls.run()
         self.assertEqual(len(bt_cls.results.requested), 2)
         self.assertEqual(len(bt_cls.results.passed), 2)
+        self.assertIsNone(bt_cls.results.passed[0].uid)
+        self.assertIsNone(bt_cls.results.passed[1].uid)
         self.assertEqual(bt_cls.results.passed[0].test_name, 'test_1_2')
         self.assertEqual(bt_cls.results.passed[1].test_name, 'test_3_4')
 
+    def test_generate_tests_with_uid(self):
+        class MockBaseTest(base_test.BaseTestClass):
+            def setup_generated_tests(self):
+                self.generate_tests(
+                    test_logic=self.logic,
+                    name_func=self.name_gen,
+                    uid_func=self.uid_logic,
+                    arg_sets=[(1, 2), (3, 4)])
+
+            def name_gen(self, a, b):
+                return 'test_%s_%s' % (a, b)
+
+            def uid_logic(self, a, b):
+                return 'uid-%s-%s' % (a, b)
+
+            def logic(self, a, b):
+                pass
+
+        bt_cls = MockBaseTest(self.mock_test_cls_configs)
+        bt_cls.run()
+        self.assertEqual(bt_cls.results.passed[0].uid, 'uid-1-2')
+        self.assertEqual(bt_cls.results.passed[1].uid, 'uid-3-4')
+
+    def test_generate_tests_with_none_uid(self):
+        class MockBaseTest(base_test.BaseTestClass):
+            def setup_generated_tests(self):
+                self.generate_tests(
+                    test_logic=self.logic,
+                    name_func=self.name_gen,
+                    uid_func=self.uid_logic,
+                    arg_sets=[(1, 2), (3, 4)])
+
+            def name_gen(self, a, b):
+                return 'test_%s_%s' % (a, b)
+
+            def uid_logic(self, a, b):
+                if a == 1:
+                    return None
+                return 'uid-3-4'
+
+            def logic(self, a, b):
+                pass
+
+        bt_cls = MockBaseTest(self.mock_test_cls_configs)
+        bt_cls.run()
+        self.assertIsNone(bt_cls.results.passed[0].uid)
+        self.assertEqual(bt_cls.results.passed[1].uid, 'uid-3-4')
+
     def test_generate_tests_selected_run(self):
         class MockBaseTest(base_test.BaseTestClass):
             def setup_generated_tests(self):
                 self.generate_tests(
                     test_logic=self.logic,
                     name_func=self.name_gen,
                     arg_sets=[(1, 2), (3, 4)])
@@ -1921,15 +1971,16 @@
 
         bt_cls = MockBaseTest(self.mock_test_cls_configs)
         bt_cls.run()
         actual_record = bt_cls.results.error[0]
         self.assertEqual(actual_record.test_name, "setup_generated_tests")
         self.assertEqual(
             actual_record.details,
-            'Test name "ha" already exists, cannot be duplicated!')
+            'During test generation of "logic": Test name "ha" already exists'
+            ', cannot be duplicated!')
         expected_summary = ("Error 1, Executed 0, Failed 0, Passed 0, "
                             "Requested 0, Skipped 0")
         self.assertEqual(bt_cls.results.summary_str(), expected_summary)
 
     def test_write_user_data(self):
         content = {'a': 1}
 
@@ -1939,15 +1990,15 @@
 
         bt_cls = MockBaseTest(self.mock_test_cls_configs)
         bt_cls.run(test_names=["test_something"])
         actual_record = bt_cls.results.passed[0]
         self.assertEqual(actual_record.test_name, "test_something")
         hit = False
         with io.open(self.summary_file, 'r', encoding='utf-8') as f:
-            for c in yaml.load_all(f):
+            for c in yaml.safe_load_all(f):
                 if c['Type'] != records.TestSummaryEntryType.USER_DATA.value:
                     continue
                 hit = True
                 self.assertEqual(c['a'], content['a'])
                 self.assertIsNotNone(c['timestamp'])
         self.assertTrue(hit)
 
@@ -2044,10 +2095,39 @@
         self.assertEqual(record.test_name, 'clean_up')
         self.assertIsNotNone(record.begin_time)
         self.assertIsNotNone(record.end_time)
         expected_msg = ('Failed to collect controller info from '
                         'mock_controller: Some failure')
         self.assertEqual(record.details, expected_msg)
 
+    def test_uid(self):
+        class MockBaseTest(base_test.BaseTestClass):
+            @records.uid('some-uid')
+            def test_func(self):
+                pass
+
+        bt_cls = MockBaseTest(self.mock_test_cls_configs)
+        bt_cls.run()
+        actual_record = bt_cls.results.passed[0]
+        self.assertEqual(actual_record.uid, 'some-uid')
+
+    def test_uid_not_specified(self):
+        class MockBaseTest(base_test.BaseTestClass):
+            def test_func(self):
+                pass
+
+        bt_cls = MockBaseTest(self.mock_test_cls_configs)
+        bt_cls.run()
+        actual_record = bt_cls.results.passed[0]
+        self.assertIsNone(actual_record.uid)
+
+    def test_uid_is_none(self):
+        with self.assertRaisesRegex(ValueError, 'UID cannot be None.'):
+
+            class MockBaseTest(base_test.BaseTestClass):
+                @records.uid(None)
+                def not_a_test(self):
+                    pass
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mobly-1.8.1/tests/mobly/test_runner_test.py` & `mobly-1.9.1/tests/mobly/test_runner_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from tests.lib import integration3_test
 
 
 class TestRunnerTest(unittest.TestCase):
     """This test class has unit tests for the implementation of everything
     under mobly.test_runner.
     """
-
     def setUp(self):
         self.tmp_dir = tempfile.mkdtemp()
         self.base_mock_test_config = config_parser.TestRunConfig()
         self.base_mock_test_config.test_bed_name = 'SampleTestBed'
         self.base_mock_test_config.controller_configs = {}
         self.base_mock_test_config.user_params = {
             'icecream': 42,
@@ -75,19 +74,22 @@
             'magic': 'Magic1'
         }, {
             'serial': 'xxxx',
             'magic': 'Magic2'
         }]
         mock_test_config.controller_configs[mock_ctrlr_config_name] = my_config
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.add_test_class(mock_test_config, integration_test.IntegrationTest)
-        tr.run()
+        with tr.mobly_logger():
+            tr.add_test_class(mock_test_config,
+                              integration_test.IntegrationTest)
+            tr.run()
         self.assertTrue(
             mock_test_config.controller_configs[mock_ctrlr_config_name][0])
-        tr.run()
+        with tr.mobly_logger():
+            tr.run()
         results = tr.results.summary_dict()
         self.assertEqual(results['Requested'], 2)
         self.assertEqual(results['Executed'], 2)
         self.assertEqual(results['Passed'], 2)
         expected_info_dict = {
             'Controller Info': [{
                 'MyMagic': {
@@ -123,43 +125,72 @@
             'magic': 'Magic1'
         }, {
             'serial': 'xxxx',
             'magic': 'Magic2'
         }]
         mock_test_config.controller_configs[mock_ctrlr_config_name] = my_config
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.add_test_class(mock_test_config, integration_test.IntegrationTest)
-        tr.run()
+        with tr.mobly_logger():
+            tr.add_test_class(mock_test_config,
+                              integration_test.IntegrationTest)
+            tr.run()
         summary_path = os.path.join(logging.log_path,
                                     records.OUTPUT_FILE_SUMMARY)
         with io.open(summary_path, 'r', encoding='utf-8') as f:
-            summary_entries = list(yaml.load_all(f))
+            summary_entries = list(yaml.safe_load_all(f))
         self.assertEqual(len(summary_entries), 4)
         # Verify the first entry is the list of test names.
         self.assertEqual(summary_entries[0]['Type'],
                          records.TestSummaryEntryType.TEST_NAME_LIST.value)
         self.assertEqual(summary_entries[1]['Type'],
                          records.TestSummaryEntryType.RECORD.value)
         self.assertEqual(summary_entries[2]['Type'],
                          records.TestSummaryEntryType.CONTROLLER_INFO.value)
         self.assertEqual(summary_entries[3]['Type'],
                          records.TestSummaryEntryType.SUMMARY.value)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy(1))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy(1))
-    @mock.patch(
-        'mobly.controllers.android_device.list_adb_devices',
-        return_value=['1'])
-    @mock.patch(
-        'mobly.controllers.android_device.get_all_instances',
-        return_value=mock_android_device.get_mock_ads(1))
+    def test_run(self):
+        tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
+        self.base_mock_test_config.controller_configs[
+            mock_controller.MOBLY_CONTROLLER_CONFIG_NAME] = '*'
+        with tr.mobly_logger():
+            tr.add_test_class(self.base_mock_test_config,
+                              integration_test.IntegrationTest)
+            tr.run()
+        results = tr.results.summary_dict()
+        self.assertEqual(results['Requested'], 1)
+        self.assertEqual(results['Executed'], 1)
+        self.assertEqual(results['Passed'], 1)
+        self.assertEqual(len(tr.results.executed), 1)
+        record = tr.results.executed[0]
+        self.assertEqual(record.test_class, 'IntegrationTest')
+
+    def test_run_without_mobly_logger_context(self):
+        tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
+        self.base_mock_test_config.controller_configs[
+            mock_controller.MOBLY_CONTROLLER_CONFIG_NAME] = '*'
+        tr.add_test_class(self.base_mock_test_config,
+                          integration_test.IntegrationTest)
+        tr.run()
+        results = tr.results.summary_dict()
+        self.assertEqual(results['Requested'], 1)
+        self.assertEqual(results['Executed'], 1)
+        self.assertEqual(results['Passed'], 1)
+        self.assertEqual(len(tr.results.executed), 1)
+        record = tr.results.executed[0]
+        self.assertEqual(record.test_class, 'IntegrationTest')
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy(1))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy(1))
+    @mock.patch('mobly.controllers.android_device.list_adb_devices',
+                return_value=['1'])
+    @mock.patch('mobly.controllers.android_device.get_all_instances',
+                return_value=mock_android_device.get_mock_ads(1))
     def test_run_two_test_classes(self, mock_get_all, mock_list_adb,
                                   mock_fastboot, mock_adb):
         """Verifies that running more than one test class in one test run works
         properly.
 
         This requires using a built-in controller module. Using AndroidDevice
         module since it has all the mocks needed already.
@@ -174,21 +205,25 @@
             'magic': 'Magic2'
         }]
         mock_test_config.controller_configs[mock_ctrlr_config_name] = my_config
         mock_test_config.controller_configs['AndroidDevice'] = [{
             'serial': '1'
         }]
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.add_test_class(mock_test_config, integration2_test.Integration2Test)
-        tr.add_test_class(mock_test_config, integration_test.IntegrationTest)
-        tr.run()
+        with tr.mobly_logger():
+            tr.add_test_class(mock_test_config,
+                              integration2_test.Integration2Test)
+            tr.add_test_class(mock_test_config,
+                              integration_test.IntegrationTest)
+            tr.run()
         results = tr.results.summary_dict()
         self.assertEqual(results['Requested'], 2)
         self.assertEqual(results['Executed'], 2)
         self.assertEqual(results['Passed'], 2)
+        self.assertEqual(len(tr.results.executed), 2)
         # Tag of the test class defaults to the class name.
         record1 = tr.results.executed[0]
         record2 = tr.results.executed[1]
         self.assertEqual(record1.test_class, 'Integration2Test')
         self.assertEqual(record2.test_class, 'IntegrationTest')
 
     def test_run_two_test_classes_different_configs_and_aliases(self):
@@ -199,40 +234,42 @@
         config1.controller_configs[
             mock_controller.MOBLY_CONTROLLER_CONFIG_NAME] = [{
                 'serial': 'xxxx'
             }]
         config2 = config1.copy()
         config2.user_params['icecream'] = 10
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.add_test_class(
-            config1,
-            integration_test.IntegrationTest,
-            name_suffix='FirstConfig')
-        tr.add_test_class(
-            config2,
-            integration_test.IntegrationTest,
-            name_suffix='SecondConfig')
-        tr.run()
+        with tr.mobly_logger():
+            tr.add_test_class(config1,
+                              integration_test.IntegrationTest,
+                              name_suffix='FirstConfig')
+            tr.add_test_class(config2,
+                              integration_test.IntegrationTest,
+                              name_suffix='SecondConfig')
+            tr.run()
         results = tr.results.summary_dict()
         self.assertEqual(results['Requested'], 2)
         self.assertEqual(results['Executed'], 2)
         self.assertEqual(results['Passed'], 1)
         self.assertEqual(results['Failed'], 1)
         self.assertEqual(tr.results.failed[0].details, '10 != 42')
+        self.assertEqual(len(tr.results.executed), 2)
         record1 = tr.results.executed[0]
         record2 = tr.results.executed[1]
         self.assertEqual(record1.test_class, 'IntegrationTest_FirstConfig')
         self.assertEqual(record2.test_class, 'IntegrationTest_SecondConfig')
 
     def test_run_with_abort_all(self):
         mock_test_config = self.base_mock_test_config.copy()
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.add_test_class(mock_test_config, integration3_test.Integration3Test)
-        with self.assertRaises(signals.TestAbortAll):
-            tr.run()
+        with tr.mobly_logger():
+            tr.add_test_class(mock_test_config,
+                              integration3_test.Integration3Test)
+            with self.assertRaises(signals.TestAbortAll):
+                tr.run()
         results = tr.results.summary_dict()
         self.assertEqual(results['Requested'], 1)
         self.assertEqual(results['Executed'], 0)
         self.assertEqual(results['Passed'], 0)
         self.assertEqual(results['Failed'], 0)
 
     def test_add_test_class_mismatched_log_path(self):
@@ -251,35 +288,60 @@
                 test_runner.Error,
                 'TestRunner\'s test bed is "different_test_bed", but a test '
                 r'config with a different test bed \("%s"\) was added.' %
                 self.test_bed_name):
             tr.add_test_class(self.base_mock_test_config,
                               integration_test.IntegrationTest)
 
-    def test_teardown_logger_before_setup_logger(self):
-        tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        with self.assertRaisesRegex(
-                test_runner.Error,
-                'TestRunner\._teardown_logger\(\) called before '
-                'TestRunner\.setup_logger\(\)!'):
-            tr._teardown_logger()
-
     def test_run_no_tests(self):
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
         with self.assertRaisesRegex(test_runner.Error, 'No tests to execute.'):
             tr.run()
 
-    @mock.patch(
-        'mobly.test_runner._find_test_class',
-        return_value=type('SampleTest', (), {}))
-    @mock.patch(
-        'mobly.test_runner.config_parser.load_test_config_file',
-        return_value=[config_parser.TestRunConfig()])
+    @mock.patch('mobly.test_runner._find_test_class',
+                return_value=type('SampleTest', (), {}))
+    @mock.patch('mobly.test_runner.config_parser.load_test_config_file',
+                return_value=[config_parser.TestRunConfig()])
     @mock.patch('mobly.test_runner.TestRunner', return_value=mock.MagicMock())
     def test_main_parse_args(self, mock_test_runner, mock_config,
                              mock_find_test):
         test_runner.main(['-c', 'some/path/foo.yaml', '-b', 'hello'])
         mock_config.assert_called_with('some/path/foo.yaml', None)
 
+    @mock.patch('mobly.test_runner._find_test_class',
+                return_value=integration_test.IntegrationTest)
+    @mock.patch('sys.exit')
+    def test_main(self, mock_exit, mock_find_test):
+        tmp_file_path = os.path.join(self.tmp_dir, 'config.yml')
+        with io.open(tmp_file_path, 'w', encoding='utf-8') as f:
+            f.write(u"""
+                TestBeds:
+                    # A test bed where adb will find Android devices.
+                    - Name: SampleTestBed
+                      Controllers:
+                          MagicDevice: '*'
+                      TestParams:
+                          icecream: 42
+                          extra_param: 'haha'
+            """)
+        test_runner.main(['-c', tmp_file_path])
+        mock_exit.assert_not_called()
+
+    @mock.patch('mobly.test_runner._find_test_class',
+                return_value=integration_test.IntegrationTest)
+    @mock.patch('sys.exit')
+    def test_main_with_failures(self, mock_exit, mock_find_test):
+        tmp_file_path = os.path.join(self.tmp_dir, 'config.yml')
+        with io.open(tmp_file_path, 'w', encoding='utf-8') as f:
+            f.write(u"""
+                TestBeds:
+                    # A test bed where adb will find Android devices.
+                    - Name: SampleTestBed
+                      Controllers:
+                          MagicDevice: '*'
+            """)
+        test_runner.main(['-c', tmp_file_path])
+        mock_exit.assert_called_once_with(1)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mobly-1.8.1/tests/mobly/controller_manager_test.py` & `mobly-1.9.1/tests/mobly/controller_manager_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/mobly/logger_test.py` & `mobly-1.9.1/tests/mobly/controllers/monsoon_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-# Copyright 2016 Google Inc.
+# Copyright 2018 Google Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import unittest
-import pytz
+import platform
 
-from mobly import logger
+from future.tests.base import unittest
 
 
-class LoggerTest(unittest.TestCase):
-    """Verifies code in mobly.logger module.
-    """
+class MonsoonTest(unittest.TestCase):
+    @unittest.skipIf(platform.system() == 'Windows',
+                     'fcntl does not exist on Windows')
+    def test_monsoon_import(self):
+        # TODO: Replace 'fnctl' with a Windows equivalent when on Windows
+        from mobly.controllers import monsoon
 
-    def test_epoch_to_log_line_timestamp(self):
-        actual_stamp = logger.epoch_to_log_line_timestamp(
-            1469134262116, time_zone=pytz.utc)
-        self.assertEqual("07-21 20:51:02.116", actual_stamp)
 
-
-if __name__ == "__main__":
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/snippet_client_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/snippet_client_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,96 +12,70 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from builtins import str
 from builtins import bytes
 
 import mock
+import sys
 from future.tests.base import unittest
 
 from mobly.controllers.android_device_lib import adb
 from mobly.controllers.android_device_lib import jsonrpc_client_base
 from mobly.controllers.android_device_lib import snippet_client
 from tests.lib import jsonrpc_client_test_base
+from tests.lib import mock_android_device
 
 MOCK_PACKAGE_NAME = 'some.package.name'
 MOCK_MISSING_PACKAGE_NAME = 'not.installed'
 JSONRPC_BASE_CLASS = 'mobly.controllers.android_device_lib.jsonrpc_client_base.JsonRpcClientBase'
 
 
-class MockAdbProxy(object):
-    def __init__(self, **kwargs):
-        self.apk_not_installed = kwargs.get('apk_not_installed', False)
-        self.apk_not_instrumented = kwargs.get('apk_not_instrumented', False)
-        self.target_not_installed = kwargs.get('target_not_installed', False)
-
-    def shell(self, params, shell=False):
-        if 'pm list package' in params:
-            if self.apk_not_installed:
-                return b''
-            if self.target_not_installed and MOCK_MISSING_PACKAGE_NAME in params:
-                return b''
-            return bytes('package:%s' % MOCK_PACKAGE_NAME, 'utf-8')
-        elif 'pm list instrumentation' in params:
-            if self.apk_not_instrumented:
-                return b''
-            if self.target_not_installed:
-                return bytes('instrumentation:{p}/{r} (target={mp})'.format(
-                    p=MOCK_PACKAGE_NAME,
-                    r=snippet_client._INSTRUMENTATION_RUNNER_PACKAGE,
-                    mp=MOCK_MISSING_PACKAGE_NAME), 'utf-8')
-            return bytes('instrumentation:{p}/{r} (target={p})'.format(
-                p=MOCK_PACKAGE_NAME,
-                r=snippet_client._INSTRUMENTATION_RUNNER_PACKAGE), 'utf-8')
-        elif 'which' in params:
-            return b''
-
-    def getprop(self, params):
-        if params == 'ro.build.version.codename':
-            return 'Z'
-        elif params == 'ro.build.version.sdk':
-            return '28'
-
-    def __getattr__(self, name):
-        """All calls to the none-existent functions in adb proxy would
-        simply return the adb command string.
-        """
-
-        def adb_call(*args):
-            arg_str = ' '.join(str(elem) for elem in args)
-            return arg_str
+def get_print_function_name():
+    """Gets the name of the print function for mocking.
 
-        return adb_call
+    Returns:
+        A str representing the print function to mock.
+    """
+    if sys.version_info >= (3, 0):
+        return 'builtins.print'
+    else:
+        return '__builtin__.print'
 
 
 class SnippetClientTest(jsonrpc_client_test_base.JsonRpcClientTestBase):
     """Unit tests for mobly.controllers.android_device_lib.snippet_client.
     """
 
     def test_check_app_installed_normal(self):
         sc = self._make_client()
         sc._check_app_installed()
 
     def test_check_app_installed_fail_app_not_installed(self):
-        sc = self._make_client(MockAdbProxy(apk_not_installed=True))
+        sc = self._make_client(mock_android_device.MockAdbProxy())
         expected_msg = '.* %s is not installed.' % MOCK_PACKAGE_NAME
         with self.assertRaisesRegex(snippet_client.AppStartPreCheckError,
                                     expected_msg):
             sc._check_app_installed()
 
     def test_check_app_installed_fail_not_instrumented(self):
-        sc = self._make_client(MockAdbProxy(apk_not_instrumented=True))
+        sc = self._make_client(
+            mock_android_device.MockAdbProxy(
+                installed_packages=[MOCK_PACKAGE_NAME]))
         expected_msg = ('.* %s is installed, but it is not instrumented.' %
                         MOCK_PACKAGE_NAME)
         with self.assertRaisesRegex(snippet_client.AppStartPreCheckError,
                                     expected_msg):
             sc._check_app_installed()
 
     def test_check_app_installed_fail_target_not_installed(self):
-        sc = self._make_client(MockAdbProxy(target_not_installed=True))
+        sc = self._make_client(
+            mock_android_device.MockAdbProxy(instrumented_packages=[(
+                MOCK_PACKAGE_NAME, snippet_client.
+                _INSTRUMENTATION_RUNNER_PACKAGE, MOCK_MISSING_PACKAGE_NAME)]))
         expected_msg = ('.* Instrumentation target %s is not installed.' %
                         MOCK_MISSING_PACKAGE_NAME)
         with self.assertRaisesRegex(snippet_client.AppStartPreCheckError,
                                     expected_msg):
             sc._check_app_installed()
 
     @mock.patch('socket.create_connection')
@@ -205,17 +179,17 @@
         client = self._make_client(adb_proxy)
         client.stop_app()
         self.assertFalse(client.is_alive)
 
     @mock.patch('socket.create_connection')
     @mock.patch('mobly.controllers.android_device_lib.snippet_client.'
                 'SnippetClient.disconnect')
-    def test_snippet_stop_app_raises(self, mock_disconect,
+    def test_snippet_stop_app_raises(self, mock_disconnect,
                                      mock_create_connection):
-        mock_disconect.side_effect = Exception('ha')
+        mock_disconnect.side_effect = Exception('ha')
         adb_proxy = mock.MagicMock()
         adb_proxy.shell.return_value = b'OK (0 tests)'
         client = self._make_client(adb_proxy)
         client.host_port = 1
         with self.assertRaisesRegex(Exception, 'ha'):
             client.stop_app()
         adb_proxy.forward.assert_called_once_with(['--remove', 'tcp:1'])
@@ -445,18 +419,48 @@
                 b'',  # readline uses '' to mark EOF
             ])
         client = self._make_client()
         with self.assertRaisesRegex(jsonrpc_client_base.AppStartError,
                                     'Unexpected EOF waiting for app to start'):
             client.start_app_and_connect()
 
+    @mock.patch(get_print_function_name())
+    def test_help_rpc_when_printing_by_default(self, mock_print):
+        client = self._make_client()
+        mock_rpc = mock.MagicMock()
+        client._rpc = mock_rpc
+
+        result = client.help()
+        mock_rpc.assert_called_once_with('help')
+        self.assertEqual(None, result)
+        mock_print.assert_called_once_with(mock_rpc.return_value)
+
+    @mock.patch(get_print_function_name())
+    def test_help_rpc_when_not_printing(self, mock_print):
+        client = self._make_client()
+        mock_rpc = mock.MagicMock()
+        client._rpc = mock_rpc
+
+        result = client.help(print_output=False)
+        mock_rpc.assert_called_once_with('help')
+        self.assertEqual(mock_rpc.return_value, result)
+        mock_print.assert_not_called()
+
     def _make_client(self, adb_proxy=None):
-        adb_proxy = adb_proxy or MockAdbProxy()
+        adb_proxy = adb_proxy or mock_android_device.MockAdbProxy(
+            instrumented_packages=[(MOCK_PACKAGE_NAME, snippet_client.
+                                    _INSTRUMENTATION_RUNNER_PACKAGE,
+                                    MOCK_PACKAGE_NAME)])
         ad = mock.Mock()
         ad.adb = adb_proxy
+        ad.build_info = {
+            'build_version_codename':
+            ad.adb.getprop('ro.build.version.codename'),
+            'build_version_sdk': ad.adb.getprop('ro.build.version.sdk'),
+        }
         return snippet_client.SnippetClient(package=MOCK_PACKAGE_NAME, ad=ad)
 
     def _setup_mock_instrumentation_cmd(self, mock_start_standing_subprocess,
                                         resp_lines):
         mock_proc = mock_start_standing_subprocess()
         mock_proc.stdout.readline.side_effect = resp_lines
```

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/errors_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/errors_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/jsonrpc_client_base_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/jsonrpc_client_base_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 
 from mobly.controllers.android_device_lib import jsonrpc_client_base
 from tests.lib import jsonrpc_client_test_base
 
 
 class FakeRpcClient(jsonrpc_client_base.JsonRpcClientBase):
     def __init__(self):
-        super(FakeRpcClient, self).__init__(app_name='FakeRpcClient',
-            ad=mock.Mock())
+        super(FakeRpcClient, self).__init__(
+            app_name='FakeRpcClient', ad=mock.Mock())
 
 
 class JsonRpcClientBaseTest(jsonrpc_client_test_base.JsonRpcClientTestBase):
     """Unit tests for mobly.controllers.android_device_lib.jsonrpc_client_base.
     """
+
     @mock.patch('socket.create_connection')
     def test_open_timeout_io_error(self, mock_create_connection):
         """Test socket timeout with io error
 
         Test that if the net socket gives an io error, then the client
         will eventually exit with an IOError.
         """
@@ -95,15 +96,15 @@
         client.connect()
         self.assertEqual(client.uid, jsonrpc_client_base.UNKNOWN_UID)
 
     @mock.patch('socket.create_connection')
     def test_rpc_error_response(self, mock_create_connection):
         """Test rpc that is given an error response
 
-        Test that when an rpc recieves a reponse with an error will raised
+        Test that when an rpc receives a response with an error will raised
         an api error.
         """
         fake_file = self.setup_mock_socket_file(mock_create_connection)
 
         client = FakeRpcClient()
         client.connect()
 
@@ -112,15 +113,15 @@
         with self.assertRaisesRegex(jsonrpc_client_base.ApiError, '1'):
             client.some_rpc(1, 2, 3)
 
     @mock.patch('socket.create_connection')
     def test_rpc_callback_response(self, mock_create_connection):
         """Test rpc that is given a callback response.
 
-        Test that when an rpc recieves a callback reponse, a callback object is
+        Test that when an rpc receives a callback response, a callback object is
         created correctly.
         """
         fake_file = self.setup_mock_socket_file(mock_create_connection)
 
         client = FakeRpcClient()
         client.connect()
 
@@ -148,15 +149,15 @@
         with self.assertRaisesRegex(
                 jsonrpc_client_base.ProtocolError,
                 jsonrpc_client_base.ProtocolError.MISMATCHED_API_ID):
             client.some_rpc(1, 2, 3)
 
     @mock.patch('socket.create_connection')
     def test_rpc_no_response(self, mock_create_connection):
-        """Test rpc that does not get a reponse
+        """Test rpc that does not get a response
 
         Test that when an rpc does not get a response it throws a protocol
         error.
         """
         fake_file = self.setup_mock_socket_file(mock_create_connection)
 
         client = FakeRpcClient()
```

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/snippet_event_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/snippet_event_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/callback_handler_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/callback_handler_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/adb_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/adb_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -75,91 +75,84 @@
         mock_popen.return_value.stdout.readline.side_effect = ['']
 
         mock_proc.communicate = mock.Mock(
             return_value=('', MOCK_DEFAULT_STDERR.encode('utf-8')))
         mock_proc.returncode = 0
         return mock_popen
 
-    @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
-    @mock.patch('mobly.controllers.android_device_lib.adb.psutil.Process')
-    def test_exec_cmd_no_timeout_success(self, mock_psutil_process,
-                                         mock_Popen):
-        self._mock_process(mock_psutil_process, mock_Popen)
-
+    @mock.patch('mobly.utils.run_command')
+    def test_exec_cmd_no_timeout_success(self, mock_run_command):
+        mock_run_command.return_value = (0,
+                                         MOCK_DEFAULT_STDOUT.encode('utf-8'),
+                                         MOCK_DEFAULT_STDERR.encode('utf-8'))
         out = adb.AdbProxy()._exec_cmd(
             ['fake_cmd'], shell=False, timeout=None, stderr=None)
         self.assertEqual(MOCK_DEFAULT_STDOUT, out.decode('utf-8'))
+        mock_run_command.assert_called_with(
+            ['fake_cmd'], shell=False, timeout=None)
 
-    @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
-    @mock.patch('mobly.controllers.android_device_lib.adb.psutil.Process')
-    def test_exec_cmd_error_with_serial(self, mock_psutil_process, mock_popen):
-        self._mock_process(mock_psutil_process, mock_popen)
-        # update return code to indicate command execution error
-        mock_popen.return_value.returncode = 1
+    @mock.patch('mobly.utils.run_command')
+    def test_exec_cmd_error_with_serial(self, mock_run_command):
+        # Return 1 for retcode for error.
+        mock_run_command.return_value = (1,
+                                         MOCK_DEFAULT_STDOUT.encode('utf-8'),
+                                         MOCK_DEFAULT_STDERR.encode('utf-8'))
         mock_serial = 'ABCD1234'
         with self.assertRaisesRegex(adb.AdbError,
                                     'Error executing adb cmd .*') as context:
             adb.AdbProxy(mock_serial).fake_cmd()
         self.assertEqual(context.exception.serial, mock_serial)
         self.assertIn(mock_serial, context.exception.cmd)
 
-    @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
-    @mock.patch('mobly.controllers.android_device_lib.adb.psutil.Process')
-    def test_exec_cmd_error_without_serial(self, mock_psutil_process,
-                                           mock_popen):
-        self._mock_process(mock_psutil_process, mock_popen)
-        # update return code to indicate command execution error
-        mock_popen.return_value.returncode = 1
+    @mock.patch('mobly.utils.run_command')
+    def test_exec_cmd_error_without_serial(self, mock_run_command):
+        # Return 1 for retcode for error.
+        mock_run_command.return_value = (1,
+                                         MOCK_DEFAULT_STDOUT.encode('utf-8'),
+                                         MOCK_DEFAULT_STDERR.encode('utf-8'))
         with self.assertRaisesRegex(adb.AdbError,
                                     'Error executing adb cmd .*') as context:
             adb.AdbProxy()._exec_cmd(
                 ['fake_cmd'], shell=False, timeout=None, stderr=None)
         self.assertFalse(context.exception.serial)
+        mock_run_command.assert_called_with(
+            ['fake_cmd'], shell=False, timeout=None)
 
-    @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
-    @mock.patch('mobly.controllers.android_device_lib.adb.psutil.Process')
-    def test_exec_cmd_with_timeout_success(self, mock_psutil_process,
-                                           mock_popen):
-        self._mock_process(mock_psutil_process, mock_popen)
+    @mock.patch('mobly.utils.run_command')
+    def test_exec_cmd_with_timeout_success(self, mock_run_command):
+        mock_run_command.return_value = (0,
+                                         MOCK_DEFAULT_STDOUT.encode('utf-8'),
+                                         MOCK_DEFAULT_STDERR.encode('utf-8'))
 
         out = adb.AdbProxy()._exec_cmd(
             ['fake_cmd'], shell=False, timeout=1, stderr=None)
         self.assertEqual(MOCK_DEFAULT_STDOUT, out.decode('utf-8'))
+        mock_run_command.assert_called_with(
+            ['fake_cmd'], shell=False, timeout=1)
 
-    @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
-    @mock.patch('mobly.controllers.android_device_lib.adb.psutil.Process')
-    def test_exec_cmd_timed_out(self, mock_psutil_process, mock_popen):
-        self._mock_process(mock_psutil_process, mock_popen)
-        mock_psutil_process.return_value.wait.side_effect = (
-            adb.psutil.TimeoutExpired('Timed out'))
+    @mock.patch('mobly.utils.run_command')
+    def test_exec_cmd_timed_out(self, mock_run_command):
+        mock_run_command.side_effect = adb.psutil.TimeoutExpired('Timed out')
         mock_serial = '1234Abcd'
         with self.assertRaisesRegex(
                 adb.AdbTimeoutError, 'Timed out executing command "adb -s '
                 '1234Abcd fake-cmd" after 0.01s.') as context:
             adb.AdbProxy(mock_serial).fake_cmd(timeout=0.01)
         self.assertEqual(context.exception.serial, mock_serial)
         self.assertIn(mock_serial, context.exception.cmd)
 
-    @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
-    @mock.patch('mobly.controllers.android_device_lib.adb.psutil.Process')
-    def test_exec_cmd_timed_out_without_serial(self, mock_psutil_process,
-                                               mock_popen):
-        self._mock_process(mock_psutil_process, mock_popen)
-        mock_psutil_process.return_value.wait.side_effect = (
-            adb.psutil.TimeoutExpired('Timed out'))
+    @mock.patch('mobly.utils.run_command')
+    def test_exec_cmd_timed_out_without_serial(self, mock_run_command):
+        mock_run_command.side_effect = adb.psutil.TimeoutExpired('Timed out')
         with self.assertRaisesRegex(adb.AdbTimeoutError,
                                     'Timed out executing command "adb '
                                     'fake-cmd" after 0.01s.') as context:
             adb.AdbProxy().fake_cmd(timeout=0.01)
 
-    @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
-    @mock.patch('mobly.controllers.android_device_lib.adb.psutil.Process')
-    def test_exec_cmd_with_negative_timeout_value(self, mock_psutil_process,
-                                                  mock_popen):
-        self._mock_process(mock_psutil_process, mock_popen)
+    def test_exec_cmd_with_negative_timeout_value(self):
         with self.assertRaisesRegex(ValueError,
                                     'Timeout is not a positive value: -1'):
             adb.AdbProxy()._exec_cmd(
                 ['fake_cmd'], shell=False, timeout=-1, stderr=None)
 
     @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
     def test_execute_and_process_stdout_reads_stdout(self, mock_popen):
@@ -177,16 +170,16 @@
     def test_execute_and_process_stdout_reads_unexpected_stdout(
             self, mock_popen):
         unexpected_stdout = MOCK_DEFAULT_STDOUT.encode('utf-8')
 
         self._mock_execute_and_process_stdout_process(mock_popen)
         mock_handler = mock.MagicMock()
         mock_popen.return_value.communicate = mock.Mock(
-            return_value=(unexpected_stdout,
-                          MOCK_DEFAULT_STDERR.encode('utf-8')))
+            return_value=(unexpected_stdout, MOCK_DEFAULT_STDERR.encode(
+                'utf-8')))
 
         err = adb.AdbProxy()._execute_and_process_stdout(
             ['fake_cmd'], shell=False, handler=mock_handler)
         self.assertEqual(mock_handler.call_count, 1)
         mock_handler.assert_called_with(unexpected_stdout)
 
     @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
@@ -310,16 +303,16 @@
         adb_cmd = adb.AdbProxy()._construct_adb_cmd(
             'shell', ['ls /asdafsfd/asdf-asfd/asa'], shell=False)
         self.assertEqual(adb_cmd,
                          ['adb', 'shell', 'ls /asdafsfd/asdf-asfd/asa'])
 
     def test_construct_adb_cmd_with_special_characters(self):
         adb_cmd = adb.AdbProxy()._construct_adb_cmd(
-            'shell', ['a b', '"blah"', '\/\/'], shell=False)
-        self.assertEqual(adb_cmd, ['adb', 'shell', 'a b', '"blah"', "\/\/"])
+            'shell', ['a b', '"blah"', r'\/\/'], shell=False)
+        self.assertEqual(adb_cmd, ['adb', 'shell', 'a b', '"blah"', r"\/\/"])
 
     def test_construct_adb_cmd_with_serial(self):
         adb_cmd = adb.AdbProxy('12345')._construct_adb_cmd(
             'shell', 'arg1', shell=False)
         self.assertEqual(adb_cmd, ['adb', '-s', '12345', 'shell', 'arg1'])
 
     def test_construct_adb_cmd_with_list(self):
@@ -351,15 +344,15 @@
     def test_construct_adb_cmd_with_shell_true_with_one_arg_command_list(self):
         adb_cmd = adb.AdbProxy()._construct_adb_cmd(
             'shell', ['ls /asdafsfd/asdf-asfd/asa'], shell=True)
         self.assertEqual(adb_cmd, '"adb" shell \'ls /asdafsfd/asdf-asfd/asa\'')
 
     def test_construct_adb_cmd_with_shell_true_with_auto_quotes(self):
         adb_cmd = adb.AdbProxy()._construct_adb_cmd(
-            'shell', ['a b', '"blah"', '\/\/'], shell=True)
+            'shell', ['a b', '"blah"', r'\/\/'], shell=True)
         self.assertEqual(adb_cmd, '"adb" shell \'a b\' \'"blah"\' \'\\/\\/\'')
 
     def test_construct_adb_cmd_with_shell_true_with_serial(self):
         adb_cmd = adb.AdbProxy('12345')._construct_adb_cmd(
             'shell', 'arg1 arg2', shell=True)
         self.assertEqual(adb_cmd, '"adb" -s "12345" shell arg1 arg2')
 
@@ -435,26 +428,151 @@
                 adb.AdbProxy()._execute_adb_and_process_stdout(
                     'shell', mock_adb_args, shell=False, handler=mock_handler)
                 mock_construct_adb_cmd.assert_called_once_with(
                     'shell', mock_adb_args, shell=False)
                 mock_execute_and_process_stdout.assert_called_once_with(
                     mock_adb_cmd, shell=False, handler=mock_handler)
 
-    @mock.patch('mobly.controllers.android_device_lib.adb.subprocess.Popen')
-    @mock.patch('mobly.controllers.android_device_lib.adb.psutil.Process')
-    def test_exec_adb_cmd_with_stderr_pipe(self, mock_psutil_process,
-                                           mock_popen):
-        self._mock_process(mock_psutil_process, mock_popen)
+    @mock.patch('mobly.utils.run_command')
+    def test_exec_adb_cmd_with_stderr_pipe(self, mock_run_command):
+        mock_run_command.return_value = (0,
+                                         MOCK_DEFAULT_STDOUT.encode('utf-8'),
+                                         MOCK_DEFAULT_STDERR.encode('utf-8'))
         stderr_redirect = io.BytesIO()
         out = adb.AdbProxy().shell(
             'arg1 arg2', shell=True, stderr=stderr_redirect)
         self.assertEqual(MOCK_DEFAULT_STDOUT, out.decode('utf-8'))
         self.assertEqual(MOCK_DEFAULT_STDERR,
                          stderr_redirect.getvalue().decode('utf-8'))
 
+    def test_getprop(self):
+        with mock.patch.object(adb.AdbProxy, '_exec_cmd') as mock_exec_cmd:
+            mock_exec_cmd.return_value = b'blah'
+            self.assertEqual(adb.AdbProxy().getprop('haha'), 'blah')
+            mock_exec_cmd.assert_called_once_with(
+                ['adb', 'shell', 'getprop', 'haha'],
+                shell=False,
+                stderr=None,
+                timeout=adb.DEFAULT_GETPROP_TIMEOUT_SEC)
+
+    def test__parse_getprop_output_special_values(self):
+        mock_adb_output = (
+            b'[selinux.restorecon_recursive]: [/data/misc_ce/10]\n'
+            b'[selinux.abc]: [key: value]\n'  # "key: value" as value
+            b'[persist.sys.boot.reason.history]: [reboot,adb,1558549857\n'
+            b'reboot,factory_reset,1558483886\n'  # multi-line value
+            b'reboot,1558483823]\n'
+            b'[persist.something]: [haha\n'
+            b']\n'
+            b'[[wrapped.key]]: [[wrapped value]]\n'
+            b'[persist.byte]: [J\xaa\x8bb\xab\x9dP\x0f]\n'  # non-decodable
+        )
+        parsed_props = adb.AdbProxy()._parse_getprop_output(mock_adb_output)
+        expected_output = {
+            'persist.sys.boot.reason.history':
+            ('reboot,adb,1558549857\nreboot,factory_reset,1558483886\n'
+             'reboot,1558483823'),
+            'selinux.abc':
+            'key: value',
+            'persist.something':
+            'haha\n',
+            'selinux.restorecon_recursive':
+            '/data/misc_ce/10',
+            '[wrapped.key]':
+            '[wrapped value]',
+            'persist.byte':
+            'JbP\x0f',
+        }
+        self.assertEqual(parsed_props, expected_output)
+
+    def test__parse_getprop_output_malformat_output(self):
+        mock_adb_output = (
+            b'[selinux.restorecon_recursive][/data/misc_ce/10]\n'  # Malformat
+            b'[persist.sys.boot.reason]: [reboot,adb,1558549857]\n'
+            b'[persist.something]: [haha]\n')
+        parsed_props = adb.AdbProxy()._parse_getprop_output(mock_adb_output)
+        expected_output = {
+            'persist.sys.boot.reason': 'reboot,adb,1558549857',
+            'persist.something': 'haha'
+        }
+        self.assertEqual(parsed_props, expected_output)
+
+    def test__parse_getprop_output_special_line_separator(self):
+        mock_adb_output = (
+            b'[selinux.restorecon_recursive][/data/misc_ce/10]\r\n'  # Malformat
+            b'[persist.sys.boot.reason]: [reboot,adb,1558549857]\r\n'
+            b'[persist.something]: [haha]\r\n')
+        parsed_props = adb.AdbProxy()._parse_getprop_output(mock_adb_output)
+        expected_output = {
+            'persist.sys.boot.reason': 'reboot,adb,1558549857',
+            'persist.something': 'haha'
+        }
+        self.assertEqual(parsed_props, expected_output)
+
+    @mock.patch('time.sleep', return_value=mock.MagicMock())
+    def test_getprops(self, mock_sleep):
+        with mock.patch.object(adb.AdbProxy, '_exec_cmd') as mock_exec_cmd:
+            mock_exec_cmd.return_value = (
+                b'\n[sendbug.preferred.domain]: [google.com]\n'
+                b'[sys.uidcpupower]: []\n'
+                b'[sys.wifitracing.started]: [1]\n'
+                b'[telephony.lteOnCdmaDevice]: [1]\n\n')
+            actual_output = adb.AdbProxy().getprops([
+                'sys.wifitracing.started',  # "numeric" value
+                'sys.uidcpupower',  # empty value
+                'sendbug.preferred.domain',  # string value
+                'nonExistentProp'
+            ])
+            self.assertEqual(actual_output, {
+                'sys.wifitracing.started': '1',
+                'sys.uidcpupower': '',
+                'sendbug.preferred.domain': 'google.com'
+            })
+            mock_exec_cmd.assert_called_once_with(
+                ['adb', 'shell', 'getprop'],
+                shell=False,
+                stderr=None,
+                timeout=adb.DEFAULT_GETPROP_TIMEOUT_SEC)
+            mock_sleep.assert_not_called()
+
+    @mock.patch('time.sleep', return_value=mock.MagicMock())
+    def test_getprops_when_empty_string_randomly_returned(self, mock_sleep):
+        with mock.patch.object(adb.AdbProxy, '_exec_cmd') as mock_exec_cmd:
+            mock_exec_cmd.side_effect = [
+                b'', (b'\n[ro.build.id]: [AB42]\n'
+                      b'[ro.build.type]: [userdebug]\n\n')
+            ]
+            actual_output = adb.AdbProxy().getprops(['ro.build.id'])
+            self.assertEqual(actual_output, {
+                'ro.build.id': 'AB42',
+            })
+            self.assertEqual(mock_exec_cmd.call_count, 2)
+            mock_exec_cmd.assert_called_with(
+                ['adb', 'shell', 'getprop'],
+                shell=False,
+                stderr=None,
+                timeout=adb.DEFAULT_GETPROP_TIMEOUT_SEC)
+            self.assertEqual(mock_sleep.call_count, 1)
+            mock_sleep.assert_called_with(1)
+
+    @mock.patch('time.sleep', return_value=mock.MagicMock())
+    def test_getprops_when_empty_string_always_returned(self, mock_sleep):
+        with mock.patch.object(adb.AdbProxy, '_exec_cmd') as mock_exec_cmd:
+            mock_exec_cmd.return_value = b''
+            actual_output = adb.AdbProxy().getprops(['ro.build.id'])
+            self.assertEqual(actual_output, {})
+            self.assertEqual(mock_exec_cmd.call_count, 3)
+            mock_exec_cmd.assert_called_with(
+                ['adb', 'shell', 'getprop'],
+                shell=False,
+                stderr=None,
+                timeout=adb.DEFAULT_GETPROP_TIMEOUT_SEC)
+            self.assertEqual(mock_sleep.call_count, 2)
+            mock_sleep.assert_called_with(1)
+
     def test_forward(self):
         with mock.patch.object(adb.AdbProxy, '_exec_cmd') as mock_exec_cmd:
             adb.AdbProxy().forward(MOCK_SHELL_COMMAND)
 
     def test_instrument_without_parameters(self):
         """Verifies the AndroidDevice object's instrument command is correct in
         the basic case.
@@ -546,20 +664,14 @@
                 options=MOCK_INSTRUMENTATION_OPTIONS,
                 handler=mock_handler)
             mock_execute_and_process_stdout.assert_called_once_with(
                 ['adb', 'shell', MOCK_OPTIONS_INSTRUMENTATION_COMMAND],
                 shell=False,
                 handler=mock_handler)
 
-    def test_cli_cmd_to_string(self):
-        cmd = ['"adb"', 'a b', 'c//']
-        self.assertEqual(adb.cli_cmd_to_string(cmd), '\'"adb"\' \'a b\' c//')
-        cmd = 'adb -s meme do something ab_cd'
-        self.assertEqual(adb.cli_cmd_to_string(cmd), cmd)
-
     def test_has_shell_command_called_correctly(self):
         with mock.patch.object(adb.AdbProxy, '_exec_cmd') as mock_exec_cmd:
             mock_exec_cmd.return_value = MOCK_DEFAULT_COMMAND_OUTPUT
             adb.AdbProxy().has_shell_command(MOCK_SHELL_COMMAND)
             mock_exec_cmd.assert_called_once_with(
                 ['adb', 'shell', 'command', '-v', MOCK_SHELL_COMMAND],
                 shell=False,
```

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/sl4a_client_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/sl4a_client_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,42 +18,15 @@
 import mock
 from future.tests.base import unittest
 
 from mobly.controllers.android_device_lib import adb
 from mobly.controllers.android_device_lib import jsonrpc_client_base
 from mobly.controllers.android_device_lib import sl4a_client
 from tests.lib import jsonrpc_client_test_base
-
-
-class MockAdbProxy(object):
-    def __init__(self, **kwargs):
-        self.apk_not_installed = kwargs.get('apk_not_installed', False)
-
-    def shell(self, params, shell=False):
-        if 'pm list package' in params:
-            if self.apk_not_installed:
-                return bytes('', 'utf-8')
-            return bytes('package:com.googlecode.android_scripting', 'utf-8')
-
-    def getprop(self, params):
-        if params == 'ro.build.version.codename':
-            return 'Z'
-        elif params == 'ro.build.version.sdk':
-            return '28'
-
-    def __getattr__(self, name):
-        """All calls to the none-existent functions in adb proxy would
-        simply return the adb command string.
-        """
-
-        def adb_call(*args):
-            arg_str = ' '.join(str(elem) for elem in args)
-            return arg_str
-
-        return adb_call
+from tests.lib import mock_android_device
 
 
 class Sl4aClientTest(jsonrpc_client_test_base.JsonRpcClientTestBase):
     """Unit tests for mobly.controllers.android_device_lib.sl4a_client.
     """
 
     @mock.patch('socket.create_connection')
@@ -78,24 +51,30 @@
                 'utils.get_available_host_port')
     def test_app_not_installed(self, mock_get_port,
                                mock_start_standing_subprocess,
                                mock_create_connection):
         self.setup_mock_socket_file(mock_create_connection)
         self._setup_mock_instrumentation_cmd(
             mock_start_standing_subprocess, resp_lines=[b'\n'])
-        client = self._make_client(adb_proxy=MockAdbProxy(
-            apk_not_installed=True))
+        client = self._make_client(
+            adb_proxy=mock_android_device.MockAdbProxy())
         with self.assertRaisesRegex(jsonrpc_client_base.AppStartError,
                                     '.* SL4A is not installed on .*'):
             client.start_app_and_connect()
 
     def _make_client(self, adb_proxy=None):
-        adb_proxy = adb_proxy or MockAdbProxy()
+        adb_proxy = adb_proxy or mock_android_device.MockAdbProxy(
+            installed_packages=['com.googlecode.android_scripting'])
         ad = mock.Mock()
         ad.adb = adb_proxy
+        ad.build_info = {
+            'build_version_codename':
+            ad.adb.getprop('ro.build.version.codename'),
+            'build_version_sdk': ad.adb.getprop('ro.build.version.sdk'),
+        }
         return sl4a_client.Sl4aClient(ad=ad)
 
     def _setup_mock_instrumentation_cmd(self, mock_start_standing_subprocess,
                                         resp_lines):
         mock_proc = mock_start_standing_subprocess()
         mock_proc.stdout.readline.side_effect = resp_lines
```

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/services/logcat_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/services/logcat_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,24 +53,23 @@
 
 # Mock start and end time of the adb cat.
 MOCK_ADB_LOGCAT_BEGIN_TIME = '02-29 14:02:20.123'
 MOCK_ADB_LOGCAT_END_TIME = '02-29 14:02:22.000'
 
 # Mock AdbError for missing logpersist scripts
 MOCK_LOGPERSIST_STOP_MISSING_ADB_ERROR = adb.AdbError(
-    'logpersist.stop --clear', '',
+    'logpersist.stop --clear', b'',
     '/system/bin/sh: logpersist.stop: not found', 0)
 MOCK_LOGPERSIST_START_MISSING_ADB_ERROR = adb.AdbError(
-    'logpersist.start --clear', '',
-    '/system/bin/sh: logpersist.stop: not found', 0)
+    'logpersist.start --clear', b'',
+    b'/system/bin/sh: logpersist.stop: not found', 0)
 
 
 class LogcatTest(unittest.TestCase):
     """Tests for Logcat service and its integration with AndroidDevice."""
-
     def setUp(self):
         # Set log_path to logging since mobly logger setup is not called.
         if not hasattr(logging, 'log_path'):
             setattr(logging, 'log_path', '/tmp/logs')
         # Creates a temp dir to be used by tests in this test class.
         self.tmp_dir = tempfile.mkdtemp()
 
@@ -85,23 +84,21 @@
         self.assertIn(content, output)
 
     def AssertFileDoesNotContain(self, content, file_path):
         with open(file_path, 'r') as f:
             output = f.read()
         self.assertNotIn(content, output)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_start_and_stop(self, stop_proc_mock, start_proc_mock,
                             create_dir_mock, FastbootProxy, MockAdbProxy):
         """Verifies the steps of collecting adb logcat on an AndroidDevice
         object, including various function calls and the expected behaviors of
         the calls.
         """
@@ -129,23 +126,73 @@
         # Verify stop did the correct operations.
         logcat_service.stop()
         stop_proc_mock.assert_called_with('process')
         self.assertIsNone(logcat_service._adb_logcat_process)
         self.assertEqual(logcat_service.adb_logcat_file_path,
                          expected_log_path)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
+    @mock.patch('mobly.utils.stop_standing_subprocess')
+    def test_update_config(self, stop_proc_mock, start_proc_mock,
+                           create_dir_mock, FastbootProxy, MockAdbProxy):
+        mock_serial = '1'
+        ad = android_device.AndroidDevice(serial=mock_serial)
+        logcat_service = logcat.Logcat(ad)
+        logcat_service.start()
+        logcat_service.stop()
+        new_log_params = '-a -b -c'
+        new_file_path = 'some/path/log.txt'
+        new_config = logcat.Config(logcat_params=new_log_params,
+                                   output_file_path=new_file_path)
+        logcat_service.update_config(new_config)
+        logcat_service.start()
+        self.assertTrue(logcat_service._adb_logcat_process)
+        create_dir_mock.assert_has_calls([mock.call('some/path')])
+        expected_adb_cmd = ('"adb" -s 1 logcat -v threadtime -a -b -c >> '
+                            '"some/path/log.txt"')
+        start_proc_mock.assert_called_with(expected_adb_cmd, shell=True)
+        self.assertEqual(logcat_service.adb_logcat_file_path,
+                         'some/path/log.txt')
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.create_dir')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
+    @mock.patch('mobly.utils.stop_standing_subprocess')
+    def test_update_config_while_running(self, stop_proc_mock, start_proc_mock,
+                                         create_dir_mock, FastbootProxy,
+                                         MockAdbProxy):
+        mock_serial = '1'
+        ad = android_device.AndroidDevice(serial=mock_serial)
+        logcat_service = logcat.Logcat(ad)
+        logcat_service.start()
+        new_config = logcat.Config(logcat_params='-blah',
+                                   output_file_path='some/path/file.txt')
+        with self.assertRaisesRegex(
+                logcat.Error,
+                'Logcat thread is already running, cannot start another one'):
+            logcat_service.update_config(new_config)
+        self.assertTrue(logcat_service.is_alive)
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.create_dir')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     @mock.patch(
         'mobly.controllers.android_device_lib.services.logcat.Logcat.clear_adb_log',
         return_value=mock_android_device.MockAdbProxy('1'))
     def test_pause_and_resume(self, clear_adb_mock, stop_proc_mock,
                               start_proc_mock, create_dir_mock, FastbootProxy,
                               MockAdbProxy):
@@ -160,22 +207,20 @@
         stop_proc_mock.assert_called_with('process')
         self.assertIsNone(logcat_service._adb_logcat_process)
         clear_adb_mock.reset_mock()
         logcat_service.resume()
         self.assertTrue(logcat_service.is_alive)
         clear_adb_mock.assert_not_called()
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     @mock.patch(
         'mobly.controllers.android_device_lib.services.logcat.Logcat.clear_adb_log',
         return_value=mock_android_device.MockAdbProxy('1'))
     def test_logcat_service_create_excerpt(self, clear_adb_mock,
                                            stop_proc_mock, start_proc_mock,
                                            FastbootProxy, MockAdbProxy):
@@ -210,23 +255,21 @@
         expected_path2 = os.path.join(test_output_dir, 'test_bar-456',
                                       'adblog,fakemodel,1.txt')
         self.assertTrue(os.path.exists(expected_path2))
         self.AssertFileContains(FILE_CONTENT, expected_path2)
         self.AssertFileDoesNotContain(FILE_CONTENT, expected_path1)
         self.assertFalse(os.path.exists(logcat_service.adb_logcat_file_path))
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_take_logcat_with_extra_params(self, stop_proc_mock,
                                            start_proc_mock, create_dir_mock,
                                            FastbootProxy, MockAdbProxy):
         """Verifies the steps of collecting adb logcat on an AndroidDevice
         object, including various function calls and the expected behaviors of
         the calls.
@@ -245,42 +288,37 @@
         create_dir_mock.assert_called_with(os.path.dirname(expected_log_path))
         adb_cmd = '"adb" -s %s logcat -v threadtime -b radio >> %s'
         start_proc_mock.assert_called_with(
             adb_cmd % (ad.serial, '"%s"' % expected_log_path), shell=True)
         self.assertEqual(logcat_service.adb_logcat_file_path,
                          expected_log_path)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test_instantiation(self, MockFastboot, MockAdbProxy):
         """Verifies the AndroidDevice object's basic attributes are correctly
         set after instantiation.
         """
         mock_serial = 1
         ad = android_device.AndroidDevice(serial=mock_serial)
         logcat_service = logcat.Logcat(ad)
         self.assertIsNone(logcat_service._adb_logcat_process)
         self.assertIsNone(logcat_service.adb_logcat_file_path)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
-    @mock.patch(
-        'mobly.logger.get_log_line_timestamp',
-        return_value=MOCK_ADB_LOGCAT_END_TIME)
+    @mock.patch('mobly.logger.get_log_line_timestamp',
+                return_value=MOCK_ADB_LOGCAT_END_TIME)
     def test_cat_adb_log(self, mock_timestamp_getter, stop_proc_mock,
                          start_proc_mock, FastbootProxy, MockAdbProxy):
         """Verifies that AndroidDevice.cat_adb_log loads the correct adb log
         file, locates the correct adb log lines within the given time range,
         and writes the lines to the correct output file.
         """
         mock_serial = '1'
@@ -292,40 +330,37 @@
         # Expect error if attempted to cat adb log before starting adb logcat.
         expected_msg = ('.* Attempting to cat adb log when none'
                         ' has been collected.')
         with self.assertRaisesRegex(logcat.Error, expected_msg):
             logcat_service.cat_adb_log('some_test', MOCK_ADB_LOGCAT_BEGIN_TIME)
         logcat_service.start()
         utils.create_dir(ad.log_path)
-        mock_adb_log_path = os.path.join(ad.log_path, 'adblog,%s,%s.txt' %
-                                         (ad.model, ad.serial))
+        mock_adb_log_path = os.path.join(
+            ad.log_path, 'adblog,%s,%s.txt' % (ad.model, ad.serial))
         with io.open(mock_adb_log_path, 'w', encoding='utf-8') as f:
             f.write(MOCK_ADB_LOGCAT)
         logcat_service.cat_adb_log('some_test', MOCK_ADB_LOGCAT_BEGIN_TIME)
         cat_file_path = os.path.join(
             ad.log_path, 'AdbLogExcerpts',
             ('some_test,02-29 14-02-20.123,%s,%s.txt') % (ad.model, ad.serial))
         with io.open(cat_file_path, 'r', encoding='utf-8') as f:
             actual_cat = f.read()
         self.assertEqual(actual_cat, ''.join(MOCK_ADB_LOGCAT_CAT_RESULT))
         # Stops adb logcat.
         logcat_service.stop()
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
-    @mock.patch(
-        'mobly.logger.get_log_line_timestamp',
-        return_value=MOCK_ADB_LOGCAT_END_TIME)
+    @mock.patch('mobly.logger.get_log_line_timestamp',
+                return_value=MOCK_ADB_LOGCAT_END_TIME)
     def test_cat_adb_log_with_unicode(self, mock_timestamp_getter,
                                       stop_proc_mock, start_proc_mock,
                                       FastbootProxy, MockAdbProxy):
         """Verifies that AndroidDevice.cat_adb_log loads the correct adb log
         file, locates the correct adb log lines within the given time range,
         and writes the lines to the correct output file.
         """
@@ -338,139 +373,178 @@
         # Expect error if attempted to cat adb log before starting adb logcat.
         expected_msg = ('.* Attempting to cat adb log when none'
                         ' has been collected.')
         with self.assertRaisesRegex(logcat.Error, expected_msg):
             logcat_service.cat_adb_log('some_test', MOCK_ADB_LOGCAT_BEGIN_TIME)
         logcat_service.start()
         utils.create_dir(ad.log_path)
-        mock_adb_log_path = os.path.join(ad.log_path, 'adblog,%s,%s.txt' %
-                                         (ad.model, ad.serial))
+        mock_adb_log_path = os.path.join(
+            ad.log_path, 'adblog,%s,%s.txt' % (ad.model, ad.serial))
         with io.open(mock_adb_log_path, 'w', encoding='utf-8') as f:
             f.write(MOCK_ADB_UNICODE_LOGCAT)
         logcat_service.cat_adb_log('some_test', MOCK_ADB_LOGCAT_BEGIN_TIME)
         cat_file_path = os.path.join(
             ad.log_path, 'AdbLogExcerpts',
             ('some_test,02-29 14-02-20.123,%s,%s.txt') % (ad.model, ad.serial))
         with io.open(cat_file_path, 'r', encoding='utf-8') as f:
             actual_cat = f.read()
         self.assertEqual(actual_cat,
                          ''.join(MOCK_ADB_UNICODE_LOGCAT_CAT_RESULT))
         # Stops adb logcat.
         logcat_service.stop()
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock.MagicMock())
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock.MagicMock())
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test__enable_logpersist_with_logpersist(self, MockFastboot,
                                                 MockAdbProxy):
         mock_serial = '1'
         mock_adb_proxy = MockAdbProxy.return_value
-        # Set getprop to return '1' to indicate the device is rootable.
-        mock_adb_proxy.getprop.return_value = '1'
+        mock_adb_proxy.getprops.return_value = {
+            'ro.build.id': 'AB42',
+            'ro.build.type': 'userdebug',
+            'ro.debuggable': '1',
+        }
         mock_adb_proxy.has_shell_command.side_effect = lambda command: {
             'logpersist.start': True,
-            'logpersist.stop': True, }[command]
+            'logpersist.stop': True,
+        }[command]
         ad = android_device.AndroidDevice(serial=mock_serial)
         logcat_service = logcat.Logcat(ad)
         logcat_service._enable_logpersist()
         mock_adb_proxy.shell.assert_has_calls([
             mock.call('logpersist.stop --clear'),
             mock.call('logpersist.start'),
         ])
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock.MagicMock())
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock.MagicMock())
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    def test__enable_logpersist_with_user_build_device(self, MockFastboot,
+                                                       MockAdbProxy):
+        mock_serial = '1'
+        mock_adb_proxy = MockAdbProxy.return_value
+        mock_adb_proxy.getprops.return_value = {
+            'ro.build.id': 'AB42',
+            'ro.build.type': 'user',
+            'ro.debuggable': '0',
+        }
+        mock_adb_proxy.has_shell_command.side_effect = lambda command: {
+            'logpersist.start': True,
+            'logpersist.stop': True,
+        }[command]
+        ad = android_device.AndroidDevice(serial=mock_serial)
+        logcat_service = logcat.Logcat(ad)
+        logcat_service._enable_logpersist()
+        mock_adb_proxy.shell.assert_not_called()
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock.MagicMock())
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test__enable_logpersist_with_missing_all_logpersist(
             self, MockFastboot, MockAdbProxy):
         def adb_shell_helper(command):
             if command == 'logpersist.start':
                 raise MOCK_LOGPERSIST_START_MISSING_ADB_ERROR
             elif command == 'logpersist.stop --clear':
                 raise MOCK_LOGPERSIST_STOP_MISSING_ADB_ERROR
             else:
-                return ''
+                return b''
 
         mock_serial = '1'
         mock_adb_proxy = MockAdbProxy.return_value
-        mock_adb_proxy.getprop.return_value = 'userdebug'
+        mock_adb_proxy.getprops.return_value = {
+            'ro.build.id': 'AB42',
+            'ro.build.type': 'userdebug',
+            'ro.debuggable': '1',
+        }
         mock_adb_proxy.has_shell_command.side_effect = lambda command: {
             'logpersist.start': False,
-            'logpersist.stop': False, }[command]
+            'logpersist.stop': False,
+        }[command]
         mock_adb_proxy.shell.side_effect = adb_shell_helper
         ad = android_device.AndroidDevice(serial=mock_serial)
         logcat_service = logcat.Logcat(ad)
         logcat_service._enable_logpersist()
+        mock_adb_proxy.shell.assert_not_called()
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock.MagicMock())
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock.MagicMock())
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test__enable_logpersist_with_missing_logpersist_stop(
             self, MockFastboot, MockAdbProxy):
         def adb_shell_helper(command):
             if command == 'logpersist.stop --clear':
                 raise MOCK_LOGPERSIST_STOP_MISSING_ADB_ERROR
             else:
-                return ''
+                return b''
 
         mock_serial = '1'
         mock_adb_proxy = MockAdbProxy.return_value
-        mock_adb_proxy.getprop.return_value = 'userdebug'
+        mock_adb_proxy.getprops.return_value = {
+            'ro.build.id': 'AB42',
+            'ro.build.type': 'userdebug',
+            'ro.debuggable': '1',
+        }
         mock_adb_proxy.has_shell_command.side_effect = lambda command: {
             'logpersist.start': True,
-            'logpersist.stop': False, }[command]
+            'logpersist.stop': False,
+        }[command]
         mock_adb_proxy.shell.side_effect = adb_shell_helper
         ad = android_device.AndroidDevice(serial=mock_serial)
         logcat_service = logcat.Logcat(ad)
         logcat_service._enable_logpersist()
+        mock_adb_proxy.shell.assert_has_calls([
+            mock.call('logpersist.stop --clear'),
+        ])
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock.MagicMock())
-    @mock.patch('mobly.utils.stop_standing_subprocess')
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock.MagicMock())
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test__enable_logpersist_with_missing_logpersist_start(
             self, MockFastboot, MockAdbProxy):
         def adb_shell_helper(command):
             if command == 'logpersist.start':
                 raise MOCK_LOGPERSIST_START_MISSING_ADB_ERROR
             else:
-                return ''
+                return b''
 
         mock_serial = '1'
         mock_adb_proxy = MockAdbProxy.return_value
-        mock_adb_proxy.getprop.return_value = 'userdebug'
+        mock_adb_proxy.getprops.return_value = {
+            'ro.build.id': 'AB42',
+            'ro.build.type': 'userdebug',
+            'ro.debuggable': '1',
+        }
         mock_adb_proxy.has_shell_command.side_effect = lambda command: {
             'logpersist.start': False,
-            'logpersist.stop': True, }[command]
+            'logpersist.stop': True,
+        }[command]
         mock_adb_proxy.shell.side_effect = adb_shell_helper
         ad = android_device.AndroidDevice(serial=mock_serial)
         logcat_service = logcat.Logcat(ad)
         logcat_service._enable_logpersist()
+        mock_adb_proxy.shell.assert_not_called()
 
     @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy')
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test_clear_adb_log(self, MockFastboot, MockAdbProxy):
         mock_serial = '1'
         ad = android_device.AndroidDevice(serial=mock_serial)
         ad.adb.logcat = mock.MagicMock()
         ad.adb.logcat.side_effect = adb.AdbError(
             cmd='cmd',
-            stdout='',
-            stderr='failed to clear "main" log',
+            stdout=b'',
+            stderr=b'failed to clear "main" log',
             ret_code=1)
         logcat_service = logcat.Logcat(ad)
         logcat_service.clear_adb_log()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/services/snippet_management_service_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/services/snippet_management_service_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_lib/services/sl4a_service_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_lib/services/sl4a_service_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/mobly/controllers/android_device_test.py` & `mobly-1.9.1/tests/mobly/controllers/android_device_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -56,77 +56,69 @@
         """Removes the temp dir.
         """
         shutil.rmtree(self.tmp_dir)
 
     # Tests for android_device module functions.
     # These tests use mock AndroidDevice instances.
 
-    @mock.patch.object(
-        android_device,
-        'get_all_instances',
-        new=mock_android_device.get_all_instances)
-    @mock.patch.object(
-        android_device,
-        'list_adb_devices',
-        new=mock_android_device.list_adb_devices)
-    @mock.patch.object(
-        android_device,
-        'list_adb_devices_by_usb_id',
-        new=mock_android_device.list_adb_devices)
+    @mock.patch.object(android_device,
+                       'get_all_instances',
+                       new=mock_android_device.get_all_instances)
+    @mock.patch.object(android_device,
+                       'list_adb_devices',
+                       new=mock_android_device.list_adb_devices)
+    @mock.patch.object(android_device,
+                       'list_adb_devices_by_usb_id',
+                       new=mock_android_device.list_adb_devices)
     def test_create_with_pickup_all(self):
         pick_all_token = android_device.ANDROID_DEVICE_PICK_ALL_TOKEN
         actual_ads = android_device.create(pick_all_token)
         for actual, expected in zip(actual_ads,
                                     mock_android_device.get_mock_ads(5)):
             self.assertEqual(actual.serial, expected.serial)
 
-    @mock.patch.object(
-        android_device, 'get_instances', new=mock_android_device.get_instances)
-    @mock.patch.object(
-        android_device,
-        'list_adb_devices',
-        new=mock_android_device.list_adb_devices)
-    @mock.patch.object(
-        android_device,
-        'list_adb_devices_by_usb_id',
-        new=mock_android_device.list_adb_devices)
+    @mock.patch.object(android_device,
+                       'get_instances',
+                       new=mock_android_device.get_instances)
+    @mock.patch.object(android_device,
+                       'list_adb_devices',
+                       new=mock_android_device.list_adb_devices)
+    @mock.patch.object(android_device,
+                       'list_adb_devices_by_usb_id',
+                       new=mock_android_device.list_adb_devices)
     def test_create_with_string_list(self):
         string_list = [u'1', '2']
         actual_ads = android_device.create(string_list)
         for actual_ad, expected_serial in zip(actual_ads, ['1', '2']):
             self.assertEqual(actual_ad.serial, expected_serial)
 
-    @mock.patch.object(
-        android_device,
-        'get_instances_with_configs',
-        new=mock_android_device.get_instances_with_configs)
-    @mock.patch.object(
-        android_device,
-        'list_adb_devices',
-        new=mock_android_device.list_adb_devices)
-    @mock.patch.object(
-        android_device,
-        'list_adb_devices_by_usb_id',
-        new=mock_android_device.list_adb_devices)
+    @mock.patch.object(android_device,
+                       'get_instances_with_configs',
+                       new=mock_android_device.get_instances_with_configs)
+    @mock.patch.object(android_device,
+                       'list_adb_devices',
+                       new=mock_android_device.list_adb_devices)
+    @mock.patch.object(android_device,
+                       'list_adb_devices_by_usb_id',
+                       new=mock_android_device.list_adb_devices)
     def test_create_with_dict_list(self):
         string_list = [{'serial': '1'}, {'serial': '2'}]
         actual_ads = android_device.create(string_list)
         for actual_ad, expected_serial in zip(actual_ads, ['1', '2']):
             self.assertEqual(actual_ad.serial, expected_serial)
 
-    @mock.patch.object(
-        android_device,
-        'get_instances_with_configs',
-        new=mock_android_device.get_instances_with_configs)
-    @mock.patch.object(
-        android_device,
-        'list_adb_devices',
-        new=mock_android_device.list_adb_devices)
-    @mock.patch.object(
-        android_device, 'list_adb_devices_by_usb_id', return_value=['usb:1'])
+    @mock.patch.object(android_device,
+                       'get_instances_with_configs',
+                       new=mock_android_device.get_instances_with_configs)
+    @mock.patch.object(android_device,
+                       'list_adb_devices',
+                       new=mock_android_device.list_adb_devices)
+    @mock.patch.object(android_device,
+                       'list_adb_devices_by_usb_id',
+                       return_value=['usb:1'])
     def test_create_with_usb_id(self, mock_list_adb_devices_by_usb_id):
         string_list = [{'serial': '1'}, {'serial': '2'}, {'serial': 'usb:1'}]
         actual_ads = android_device.create(string_list)
         for actual_ad, expected_serial in zip(actual_ads, ['1', '2', 'usb:1']):
             self.assertEqual(actual_ad.serial, expected_serial)
 
     def test_create_with_empty_config(self):
@@ -169,450 +161,601 @@
         self.assertEqual(ad.serial, expected_serial)
 
     def test_get_device_success_with_serial_and_extra_field(self):
         ads = mock_android_device.get_mock_ads(5)
         expected_serial = '1'
         expected_h_port = 5555
         ads[1].h_port = expected_h_port
-        ad = android_device.get_device(
-            ads, serial=expected_serial, h_port=expected_h_port)
+        ad = android_device.get_device(ads,
+                                       serial=expected_serial,
+                                       h_port=expected_h_port)
         self.assertEqual(ad.serial, expected_serial)
         self.assertEqual(ad.h_port, expected_h_port)
 
     def test_get_device_no_match(self):
         ads = mock_android_device.get_mock_ads(5)
         expected_msg = ('Could not find a target device that matches condition'
                         ": {'serial': 5}.")
         with self.assertRaisesRegex(android_device.Error, expected_msg):
             ad = android_device.get_device(ads, serial=len(ads))
 
     def test_get_device_too_many_matches(self):
         ads = mock_android_device.get_mock_ads(5)
         target_serial = ads[1].serial = ads[0].serial
-        expected_msg = "More than one device matched: \['0', '0'\]"
+        expected_msg = r"More than one device matched: \['0', '0'\]"
         with self.assertRaisesRegex(android_device.Error, expected_msg):
             android_device.get_device(ads, serial=target_serial)
 
     def test_start_services_on_ads(self):
         """Makes sure when an AndroidDevice fails to start some services, all
         AndroidDevice objects get cleaned up.
         """
         msg = 'Some error happened.'
         ads = mock_android_device.get_mock_ads(3)
-        ads[0].services.register = mock.MagicMock()
-        ads[0].stop_services = mock.MagicMock()
-        ads[1].services.register = mock.MagicMock()
-        ads[1].stop_services = mock.MagicMock()
-        ads[2].services.register = mock.MagicMock(
+        for ad in ads:
+            ad.services.logcat.start = mock.MagicMock()
+            ad.services.stop_all = mock.MagicMock()
+            ad.skip_logcat = False
+            ad.is_required = True
+        ads[1].services.logcat.start = mock.MagicMock(
             side_effect=android_device.Error(msg))
-        ads[2].stop_services = mock.MagicMock()
         with self.assertRaisesRegex(android_device.Error, msg):
             android_device._start_services_on_ads(ads)
-        ads[0].stop_services.assert_called_once_with()
-        ads[1].stop_services.assert_called_once_with()
-        ads[2].stop_services.assert_called_once_with()
+        ads[0].services.stop_all.assert_called_once_with()
+        ads[1].services.stop_all.assert_called_once_with()
+        ads[2].services.stop_all.assert_called_once_with()
 
     def test_start_services_on_ads_skip_logcat(self):
         ads = mock_android_device.get_mock_ads(3)
         ads[0].services.logcat.start = mock.MagicMock()
         ads[1].services.logcat.start = mock.MagicMock()
         ads[2].services.logcat.start = mock.MagicMock(
             side_effect=Exception('Should not have called this.'))
         ads[2].skip_logcat = True
         android_device._start_services_on_ads(ads)
 
+    def test_take_bug_reports(self):
+        ads = mock_android_device.get_mock_ads(3)
+        android_device.take_bug_reports(ads, 'test_something', 'sometime')
+        ads[0].take_bug_report.assert_called_once_with(
+            test_name='test_something',
+            begin_time='sometime',
+            destination=None)
+        ads[1].take_bug_report.assert_called_once_with(
+            test_name='test_something',
+            begin_time='sometime',
+            destination=None)
+        ads[2].take_bug_report.assert_called_once_with(
+            test_name='test_something',
+            begin_time='sometime',
+            destination=None)
+
+    @mock.patch('mobly.logger.get_log_file_timestamp')
+    def test_take_bug_reports_with_none_values(self,
+                                               get_log_file_timestamp_mock):
+        mock_timestamp = '07-22-2019_17-55-30-765'
+        get_log_file_timestamp_mock.return_value = mock_timestamp
+        ads = mock_android_device.get_mock_ads(3)
+        android_device.take_bug_reports(ads)
+        ads[0].take_bug_report.assert_called_once_with(
+            test_name=None, begin_time=mock_timestamp, destination=None)
+        ads[1].take_bug_report.assert_called_once_with(
+            test_name=None, begin_time=mock_timestamp, destination=None)
+        ads[2].take_bug_report.assert_called_once_with(
+            test_name=None, begin_time=mock_timestamp, destination=None)
+
     # Tests for android_device.AndroidDevice class.
     # These tests mock out any interaction with the OS and real android device
     # in AndroidDeivce.
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test_AndroidDevice_instantiation(self, MockFastboot, MockAdbProxy):
         """Verifies the AndroidDevice object's basic attributes are correctly
         set after instantiation.
         """
         mock_serial = 1
         ad = android_device.AndroidDevice(serial=mock_serial)
         self.assertEqual(ad.serial, '1')
         self.assertEqual(ad.model, 'fakemodel')
         expected_lp = os.path.join(logging.log_path,
                                    'AndroidDevice%s' % mock_serial)
         self.assertEqual(ad.log_path, expected_lp)
+        self.assertIsNotNone(ad.services.logcat)
+        self.assertIsNotNone(ad.services.snippets)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test_AndroidDevice_build_info(self, MockFastboot, MockAdbProxy):
         """Verifies the AndroidDevice object's basic attributes are correctly
         set after instantiation.
         """
         ad = android_device.AndroidDevice(serial='1')
         build_info = ad.build_info
         self.assertEqual(build_info['build_id'], 'AB42')
         self.assertEqual(build_info['build_type'], 'userdebug')
-
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+        self.assertEqual(build_info['build_version_codename'], 'Z')
+        self.assertEqual(build_info['build_version_sdk'], '28')
+        self.assertEqual(build_info['build_product'], 'FakeModel')
+        self.assertEqual(build_info['product_name'], 'FakeModel')
+        self.assertEqual(build_info['debuggable'], '1')
+        self.assertEqual(len(build_info),
+                         len(android_device.CACHED_SYSTEM_PROPS))
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy(
+                    '1',
+                    mock_properties={
+                        'ro.build.id': 'AB42',
+                        'ro.build.type': 'userdebug',
+                    }))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    def test_AndroidDevice_build_info_with_minimal_properties(
+            self, MockFastboot, MockAdbProxy):
+        ad = android_device.AndroidDevice(serial='1')
+        build_info = ad.build_info
+        self.assertEqual(build_info['build_id'], 'AB42')
+        self.assertEqual(build_info['build_type'], 'userdebug')
+        self.assertEqual(build_info['build_version_codename'], '')
+        self.assertEqual(build_info['build_version_sdk'], '')
+        self.assertEqual(build_info['build_product'], '')
+        self.assertEqual(build_info['product_name'], '')
+        self.assertEqual(build_info['debuggable'], '')
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    def test_AndroidDevice_build_info_cached(self, MockFastboot, MockAdbProxy):
+        """Verifies the AndroidDevice object's basic attributes are correctly
+        set after instantiation.
+        """
+        ad = android_device.AndroidDevice(serial='1')
+        _ = ad.build_info
+        _ = ad.build_info
+        _ = ad.build_info
+        self.assertEqual(ad.adb.getprops_call_count, 1)
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy(
+                    '1',
+                    mock_properties={
+                        'ro.build.id': 'AB42',
+                        'ro.build.type': 'userdebug',
+                        'ro.debuggable': '1',
+                    }))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    def test_AndroidDevice_is_rootable_when_userdebug_device(
+            self, MockFastboot, MockAdbProxy):
+        ad = android_device.AndroidDevice(serial='1')
+        self.assertTrue(ad.is_rootable)
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy(
+                    '1',
+                    mock_properties={
+                        'ro.build.id': 'AB42',
+                        'ro.build.type': 'user',
+                        'ro.debuggable': '0',
+                    }))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    def test_AndroidDevice_is_rootable_when_user_device(
+            self, MockFastboot, MockAdbProxy):
+        ad = android_device.AndroidDevice(serial='1')
+        self.assertFalse(ad.is_rootable)
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test_AndroidDevice_device_info(self, MockFastboot, MockAdbProxy):
         ad = android_device.AndroidDevice(serial=1)
         device_info = ad.device_info
         self.assertEqual(device_info['serial'], '1')
         self.assertEqual(device_info['model'], 'fakemodel')
         self.assertEqual(device_info['build_info']['build_id'], 'AB42')
         self.assertEqual(device_info['build_info']['build_type'], 'userdebug')
         ad.add_device_info('sim_type', 'Fi')
         ad.add_device_info('build_id', 'CD42')
         device_info = ad.device_info
         self.assertEqual(device_info['user_added_info']['sim_type'], 'Fi')
         self.assertEqual(device_info['user_added_info']['build_id'], 'CD42')
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test_AndroidDevice_serial_is_valid(self, MockFastboot, MockAdbProxy):
         """Verifies that the serial is a primitive string type and serializable.
         """
         ad = android_device.AndroidDevice(serial=1)
         # In py2, checks that ad.serial is not the backported py3 str type,
         # which is not dumpable by yaml in py2.
         # In py3, new_str is equivalent to str, so this check is not
         # appropirate in py3.
         if sys.version_info < (3, 0):
             self.assertFalse(isinstance(ad.serial, new_str))
         self.assertTrue(isinstance(ad.serial, str))
         yaml.safe_dump(ad.serial)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy(1))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy(1))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy(1))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy(1))
     @mock.patch('mobly.utils.create_dir')
     def test_AndroidDevice_take_bug_report(self, create_dir_mock,
                                            FastbootProxy, MockAdbProxy):
         """Verifies AndroidDevice.take_bug_report calls the correct adb command
         and writes the bugreport file to the correct path.
         """
         mock_serial = '1'
         ad = android_device.AndroidDevice(serial=mock_serial)
-        ad.take_bug_report('test_something', 'sometime')
-        expected_path = os.path.join(
-            logging.log_path, 'AndroidDevice%s' % ad.serial, 'BugReports')
+        output_path = ad.take_bug_report(test_name='test_something',
+                                         begin_time='sometime')
+        expected_path = os.path.join(logging.log_path,
+                                     'AndroidDevice%s' % ad.serial,
+                                     'BugReports')
         create_dir_mock.assert_called_with(expected_path)
-
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1', fail_br=True))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+        self.assertEqual(
+            output_path,
+            os.path.join(expected_path, 'test_something,sometime,1.zip'))
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1',
+                                                              fail_br=True))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
     def test_AndroidDevice_take_bug_report_fail(self, create_dir_mock,
                                                 FastbootProxy, MockAdbProxy):
         """Verifies AndroidDevice.take_bug_report writes out the correct message
         when taking bugreport fails.
         """
         mock_serial = '1'
         ad = android_device.AndroidDevice(serial=mock_serial)
         expected_msg = '.* Failed to take bugreport.'
         with self.assertRaisesRegex(android_device.Error, expected_msg):
-            ad.take_bug_report('test_something', 'sometime')
+            ad.take_bug_report(test_name='test_something',
+                               begin_time='sometime')
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.create_dir')
+    @mock.patch('mobly.logger.get_log_file_timestamp')
+    def test_AndroidDevice_take_bug_report_without_args(
+            self, get_log_file_timestamp_mock, create_dir_mock, FastbootProxy,
+            MockAdbProxy):
+        get_log_file_timestamp_mock.return_value = '07-22-2019_17-53-34-450'
+        mock_serial = '1'
+        ad = android_device.AndroidDevice(serial=mock_serial)
+        output_path = ad.take_bug_report()
+        expected_path = os.path.join(logging.log_path,
+                                     'AndroidDevice%s' % ad.serial,
+                                     'BugReports')
+        self.assertEqual(
+            output_path,
+            os.path.join(expected_path,
+                         'bugreport,07-22-2019_17-53-34-450,1.zip'))
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.create_dir')
+    @mock.patch('mobly.logger.get_log_file_timestamp')
+    def test_AndroidDevice_take_bug_report_with_only_test_name(
+            self, get_log_file_timestamp_mock, create_dir_mock, FastbootProxy,
+            MockAdbProxy):
+        get_log_file_timestamp_mock.return_value = '07-22-2019_17-53-34-450'
+        mock_serial = '1'
+        ad = android_device.AndroidDevice(serial=mock_serial)
+        output_path = ad.take_bug_report(test_name='test_something')
+        expected_path = os.path.join(logging.log_path,
+                                     'AndroidDevice%s' % ad.serial,
+                                     'BugReports')
+        create_dir_mock.assert_called_with(expected_path)
+        self.assertEqual(
+            output_path,
+            os.path.join(expected_path,
+                         'test_something,07-22-2019_17-53-34-450,1.zip'))
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy(1))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy(1))
+    @mock.patch('mobly.utils.create_dir')
+    def test_AndroidDevice_take_bug_report_with_only_begin_time(
+            self, create_dir_mock, FastbootProxy, MockAdbProxy):
+        mock_serial = '1'
+        ad = android_device.AndroidDevice(serial=mock_serial)
+        output_path = ad.take_bug_report(begin_time='sometime')
+        expected_path = os.path.join(logging.log_path,
+                                     'AndroidDevice%s' % ad.serial,
+                                     'BugReports')
+        create_dir_mock.assert_called_with(expected_path)
+        self.assertEqual(
+            output_path, os.path.join(expected_path,
+                                      'bugreport,sometime,1.zip'))
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy(1))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy(1))
+    @mock.patch('mobly.utils.create_dir')
+    def test_AndroidDevice_take_bug_report_with_positional_args(
+            self, create_dir_mock, FastbootProxy, MockAdbProxy):
+        mock_serial = '1'
+        ad = android_device.AndroidDevice(serial=mock_serial)
+        output_path = ad.take_bug_report('test_something', 'sometime')
+        expected_path = os.path.join(logging.log_path,
+                                     'AndroidDevice%s' % ad.serial,
+                                     'BugReports')
+        create_dir_mock.assert_called_with(expected_path)
+        self.assertEqual(
+            output_path,
+            os.path.join(expected_path, 'test_something,sometime,1.zip'))
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
     def test_AndroidDevice_take_bug_report_with_destination(
             self, create_dir_mock, FastbootProxy, MockAdbProxy):
         mock_serial = '1'
         ad = android_device.AndroidDevice(serial=mock_serial)
         dest = tempfile.gettempdir()
-        ad.take_bug_report("test_something", "sometime", destination=dest)
+        output_path = ad.take_bug_report(test_name="test_something",
+                                         begin_time="sometime",
+                                         destination=dest)
         expected_path = os.path.join(dest)
         create_dir_mock.assert_called_with(expected_path)
-
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy(
-            '1', fail_br_before_N=True))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+        self.assertEqual(
+            output_path,
+            os.path.join(expected_path, 'test_something,sometime,1.zip'))
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy(
+                    '1', fail_br_before_N=True))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
-    def test_AndroidDevice_take_bug_report_fallback(
-            self, create_dir_mock, FastbootProxy, MockAdbProxy):
+    def test_AndroidDevice_take_bug_report_fallback(self, create_dir_mock,
+                                                    FastbootProxy,
+                                                    MockAdbProxy):
         """Verifies AndroidDevice.take_bug_report falls back to traditional
         bugreport on builds that do not have bugreportz.
         """
         mock_serial = '1'
         ad = android_device.AndroidDevice(serial=mock_serial)
-        ad.take_bug_report('test_something', 'sometime')
-        expected_path = os.path.join(
-            logging.log_path, 'AndroidDevice%s' % ad.serial, 'BugReports')
+        output_path = ad.take_bug_report(test_name='test_something',
+                                         begin_time='sometime')
+        expected_path = os.path.join(logging.log_path,
+                                     'AndroidDevice%s' % ad.serial,
+                                     'BugReports')
         create_dir_mock.assert_called_with(expected_path)
-
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+        self.assertEqual(
+            output_path,
+            os.path.join(expected_path, 'test_something,sometime,1.txt'))
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_AndroidDevice_change_log_path(self, stop_proc_mock,
                                            start_proc_mock, FastbootProxy,
                                            MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         old_path = ad.log_path
         new_log_path = tempfile.mkdtemp()
         ad.log_path = new_log_path
         self.assertTrue(os.path.exists(new_log_path))
         self.assertFalse(os.path.exists(old_path))
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_AndroidDevice_change_log_path_no_log_exists(
             self, stop_proc_mock, start_proc_mock, FastbootProxy,
             MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         old_path = ad.log_path
         new_log_path = tempfile.mkdtemp()
         ad.log_path = new_log_path
         self.assertTrue(os.path.exists(new_log_path))
         self.assertFalse(os.path.exists(old_path))
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('127.0.0.1:5557'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('127.0.0.1:5557')
+                )
     @mock.patch(
         'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
         return_value=mock_android_device.MockFastbootProxy('127.0.0.1:5557'))
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_AndroidDevice_with_reserved_character_in_serial_log_path(
             self, stop_proc_mock, start_proc_mock, FastbootProxy,
             MockAdbProxy):
         ad = android_device.AndroidDevice(serial='127.0.0.1:5557')
         base_log_path = os.path.basename(ad.log_path)
         self.assertEqual(base_log_path, 'AndroidDevice127.0.0.1-5557')
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_AndroidDevice_change_log_path_with_service(
             self, stop_proc_mock, start_proc_mock, creat_dir_mock,
             FastbootProxy, MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
-        ad.services.register('logcat', logcat.Logcat)
+        ad.services.logcat.start()
         new_log_path = tempfile.mkdtemp()
         expected_msg = '.* Cannot change `log_path` when there is service running.'
         with self.assertRaisesRegex(android_device.Error, expected_msg):
             ad.log_path = new_log_path
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_AndroidDevice_change_log_path_with_existing_file(
             self, stop_proc_mock, start_proc_mock, creat_dir_mock,
             FastbootProxy, MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         new_log_path = tempfile.mkdtemp()
         new_file_path = os.path.join(new_log_path, 'file.txt')
         with io.open(new_file_path, 'w', encoding='utf-8') as f:
             f.write(u'hahah.')
         expected_msg = '.* Logs already exist .*'
         with self.assertRaisesRegex(android_device.Error, expected_msg):
             ad.log_path = new_log_path
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_AndroidDevice_update_serial(self, stop_proc_mock, start_proc_mock,
                                          creat_dir_mock, FastbootProxy,
                                          MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         ad.update_serial('2')
         self.assertEqual(ad.serial, '2')
         self.assertEqual(ad.debug_tag, ad.serial)
         self.assertEqual(ad.adb.serial, ad.serial)
         self.assertEqual(ad.fastboot.serial, ad.serial)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch('mobly.utils.create_dir')
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_AndroidDevice_update_serial_with_service_running(
             self, stop_proc_mock, start_proc_mock, creat_dir_mock,
             FastbootProxy, MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
-        ad.services.register('logcat', logcat.Logcat)
+        ad.services.logcat.start()
         expected_msg = '.* Cannot change device serial number when there is service running.'
         with self.assertRaisesRegex(android_device.Error, expected_msg):
             ad.update_serial('2')
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch(
         'mobly.controllers.android_device_lib.snippet_client.SnippetClient')
     @mock.patch('mobly.utils.get_available_host_port')
     def test_AndroidDevice_load_snippet(self, MockGetPort, MockSnippetClient,
                                         MockFastboot, MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         ad.load_snippet('snippet', MOCK_SNIPPET_PACKAGE_NAME)
         self.assertTrue(hasattr(ad, 'snippet'))
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
-    @mock.patch('mobly.controllers.android_device_lib.sl4a_client.Sl4aClient')
-    @mock.patch('mobly.utils.get_available_host_port')
-    def test_AndroidDevice_load_sl4a(self, MockGetPort, MockSnippetClient,
-                                     MockFastboot, MockAdbProxy):
-        ad = android_device.AndroidDevice(serial='1')
-        ad.load_sl4a()
-        self.assertTrue(hasattr(ad, 'sl4a'))
-
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch(
         'mobly.controllers.android_device_lib.snippet_client.SnippetClient')
     @mock.patch('mobly.utils.get_available_host_port')
     def test_AndroidDevice_getattr(self, MockGetPort, MockSnippetClient,
                                    MockFastboot, MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         ad.load_snippet('snippet', MOCK_SNIPPET_PACKAGE_NAME)
         value = {'value': 42}
         actual_value = getattr(ad, 'some_attr', value)
         self.assertEqual(actual_value, value)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch(
         'mobly.controllers.android_device_lib.snippet_client.SnippetClient',
         return_value=MockSnippetClient)
     @mock.patch('mobly.utils.get_available_host_port')
-    def test_AndroidDevice_load_snippet_dup_package(
-            self, MockGetPort, MockSnippetClient, MockFastboot, MockAdbProxy):
+    def test_AndroidDevice_load_snippet_dup_package(self, MockGetPort,
+                                                    MockSnippetClient,
+                                                    MockFastboot,
+                                                    MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         ad.load_snippet('snippet', MOCK_SNIPPET_PACKAGE_NAME)
         expected_msg = ('Snippet package "%s" has already been loaded under '
                         'name "snippet".') % MOCK_SNIPPET_PACKAGE_NAME
         with self.assertRaisesRegex(android_device.Error, expected_msg):
             ad.load_snippet('snippet2', MOCK_SNIPPET_PACKAGE_NAME)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch(
         'mobly.controllers.android_device_lib.snippet_client.SnippetClient',
         return_value=MockSnippetClient)
     @mock.patch('mobly.utils.get_available_host_port')
     def test_AndroidDevice_load_snippet_dup_snippet_name(
             self, MockGetPort, MockSnippetClient, MockFastboot, MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         ad.load_snippet('snippet', MOCK_SNIPPET_PACKAGE_NAME)
-        expected_msg = '.* Attribute "snippet" already exists, please use a different name.'
+        expected_msg = ('.* Attribute "snippet" already exists, please use a '
+                        'different name.')
         with self.assertRaisesRegex(android_device.Error, expected_msg):
             ad.load_snippet('snippet', MOCK_SNIPPET_PACKAGE_NAME + 'haha')
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch(
         'mobly.controllers.android_device_lib.snippet_client.SnippetClient')
     @mock.patch('mobly.utils.get_available_host_port')
     def test_AndroidDevice_load_snippet_dup_attribute_name(
             self, MockGetPort, MockSnippetClient, MockFastboot, MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         expected_msg = ('Attribute "%s" already exists, please use a different'
                         ' name') % 'adb'
         with self.assertRaisesRegex(android_device.Error, expected_msg):
             ad.load_snippet('adb', MOCK_SNIPPET_PACKAGE_NAME)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch(
         'mobly.controllers.android_device_lib.snippet_client.SnippetClient')
     @mock.patch('mobly.utils.get_available_host_port')
     def test_AndroidDevice_load_snippet_start_app_fails(
             self, MockGetPort, MockSnippetClient, MockFastboot, MockAdbProxy):
         """Verifies that the correct exception is raised if start app failed.
 
@@ -627,20 +770,18 @@
             side_effect=Exception('stop failed.'))
         ad = android_device.AndroidDevice(serial='1')
         try:
             ad.load_snippet('snippet', MOCK_SNIPPET_PACKAGE_NAME)
         except Exception as e:
             assertIs(e, expected_e)
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch(
         'mobly.controllers.android_device_lib.snippet_client.SnippetClient')
     @mock.patch('mobly.utils.get_available_host_port')
     def test_AndroidDevice_unload_snippet(self, MockGetPort, MockSnippetClient,
                                           MockFastboot, MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
         ad.load_snippet('snippet', MOCK_SNIPPET_PACKAGE_NAME)
@@ -650,37 +791,34 @@
                 android_device.SnippetError,
                 '<AndroidDevice|1> No snippet registered with name "snippet"'):
             ad.unload_snippet('snippet')
         # Loading the same snippet again should succeed
         ad.load_snippet('snippet', MOCK_SNIPPET_PACKAGE_NAME)
         self.assertTrue(hasattr(ad, 'snippet'))
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     @mock.patch(
         'mobly.controllers.android_device_lib.snippet_client.SnippetClient')
     @mock.patch('mobly.utils.get_available_host_port')
-    def test_AndroidDevice_snippet_cleanup(
-            self, MockGetPort, MockSnippetClient, MockFastboot, MockAdbProxy):
+    def test_AndroidDevice_snippet_cleanup(self, MockGetPort,
+                                           MockSnippetClient, MockFastboot,
+                                           MockAdbProxy):
         ad = android_device.AndroidDevice(serial='1')
-        ad.start_services()
+        ad.services.start_all()
         ad.load_snippet('snippet', MOCK_SNIPPET_PACKAGE_NAME)
         ad.unload_snippet('snippet')
         self.assertFalse(hasattr(ad, 'snippet'))
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
     def test_AndroidDevice_debug_tag(self, MockFastboot, MockAdbProxy):
         mock_serial = '1'
         ad = android_device.AndroidDevice(serial=mock_serial)
         self.assertEqual(ad.debug_tag, '1')
         try:
             raise android_device.DeviceError(ad, 'Something')
         except android_device.DeviceError as e:
@@ -693,22 +831,20 @@
             self.assertEqual('<AndroidDevice|Mememe> Something', str(e))
         # Verify that repr is changed correctly.
         try:
             raise Exception(ad, 'Something')
         except Exception as e:
             self.assertEqual("(<AndroidDevice|Mememe>, 'Something')", str(e))
 
-    @mock.patch(
-        'mobly.controllers.android_device_lib.adb.AdbProxy',
-        return_value=mock_android_device.MockAdbProxy('1'))
-    @mock.patch(
-        'mobly.controllers.android_device_lib.fastboot.FastbootProxy',
-        return_value=mock_android_device.MockFastbootProxy('1'))
-    @mock.patch(
-        'mobly.utils.start_standing_subprocess', return_value='process')
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
     @mock.patch('mobly.utils.stop_standing_subprocess')
     def test_AndroidDevice_handle_usb_disconnect(self, stop_proc_mock,
                                                  start_proc_mock,
                                                  FastbootProxy, MockAdbProxy):
         class MockService(base_service.BaseService):
             def __init__(self, device, configs=None):
                 self._alive = False
@@ -730,19 +866,160 @@
                 self.pause_called = True
 
             def resume(self):
                 self._alive = True
                 self.resume_called = True
 
         ad = android_device.AndroidDevice(serial='1')
-        ad.start_services()
+        ad.services.start_all()
         ad.services.register('mock_service', MockService)
         with ad.handle_usb_disconnect():
             self.assertFalse(ad.services.is_any_alive)
             self.assertTrue(ad.services.mock_service.pause_called)
             self.assertFalse(ad.services.mock_service.resume_called)
         self.assertTrue(ad.services.is_any_alive)
         self.assertTrue(ad.services.mock_service.resume_called)
 
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
+    @mock.patch('mobly.utils.stop_standing_subprocess')
+    def test_AndroidDevice_handle_reboot(self, stop_proc_mock, start_proc_mock,
+                                         FastbootProxy, MockAdbProxy):
+        class MockService(base_service.BaseService):
+            def __init__(self, device, configs=None):
+                self._alive = False
+                self.pause_called = False
+                self.resume_called = False
+
+            @property
+            def is_alive(self):
+                return self._alive
+
+            def start(self, configs=None):
+                self._alive = True
+
+            def stop(self):
+                self._alive = False
+
+            def pause(self):
+                self._alive = False
+                self.pause_called = True
+
+            def resume(self):
+                self._alive = True
+                self.resume_called = True
+
+        ad = android_device.AndroidDevice(serial='1')
+        ad.services.start_all()
+        ad.services.register('mock_service', MockService)
+        with ad.handle_reboot():
+            self.assertFalse(ad.services.is_any_alive)
+            self.assertFalse(ad.services.mock_service.pause_called)
+            self.assertFalse(ad.services.mock_service.resume_called)
+        self.assertTrue(ad.services.is_any_alive)
+        self.assertFalse(ad.services.mock_service.resume_called)
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
+    @mock.patch('mobly.utils.stop_standing_subprocess')
+    def test_AndroidDevice_handle_reboot_changes_build_info(
+            self, stop_proc_mock, start_proc_mock, FastbootProxy,
+            MockAdbProxy):
+        ad = android_device.AndroidDevice(serial='1')
+        with ad.handle_reboot():
+            ad.adb.mock_properties['ro.build.type'] = 'user'
+            ad.adb.mock_properties['ro.debuggable'] = '0'
+        self.assertEqual(ad.build_info['build_type'], 'user')
+        self.assertEqual(ad.build_info['debuggable'], '0')
+        self.assertFalse(ad.is_rootable)
+        self.assertEqual(ad.adb.getprops_call_count, 2)
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch('mobly.utils.start_standing_subprocess',
+                return_value='process')
+    @mock.patch('mobly.utils.stop_standing_subprocess')
+    def test_AndroidDevice_handle_reboot_changes_build_info_with_caching(
+            self, stop_proc_mock, start_proc_mock, FastbootProxy,
+            MockAdbProxy):
+        ad = android_device.AndroidDevice(serial='1')  # Call getprops 1.
+        rootable_states = [ad.is_rootable]
+        with ad.handle_reboot():
+            rootable_states.append(ad.is_rootable)  # Call getprops 2.
+            ad.adb.mock_properties['ro.debuggable'] = '0'
+            rootable_states.append(ad.is_rootable)  # Call getprops 3.
+        # Call getprops 4, on context manager end.
+        rootable_states.append(ad.is_rootable)  # Cached call.
+        rootable_states.append(ad.is_rootable)  # Cached call.
+        self.assertEqual(ad.adb.getprops_call_count, 4)
+        self.assertEqual(rootable_states, [True, True, False, False, False])
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch(
+        'mobly.controllers.android_device.AndroidDevice.is_boot_completed',
+        side_effect=[
+            False, False,
+            adb.AdbTimeoutError(['adb', 'shell', 'getprop sys.boot_completed'],
+                                timeout=5,
+                                serial=1), True
+        ])
+    @mock.patch('time.sleep', return_value=None)
+    @mock.patch('time.time', side_effect=[0, 5, 10, 15, 20, 25, 30])
+    def test_AndroidDevice_wait_for_completion_completed(
+            self, MockTime, MockSleep, MockIsBootCompleted, FastbootProxy,
+            MockAdbProxy):
+        ad = android_device.AndroidDevice(serial='1')
+        raised = False
+        try:
+            ad.wait_for_boot_completion()
+        except (adb.AdbError, adb.AdbTimeoutError):
+            raised = True
+        self.assertFalse(
+            raised,
+            'adb.AdbError or adb.AdbTimeoutError exception raised but not handled.'
+        )
+
+    @mock.patch('mobly.controllers.android_device_lib.adb.AdbProxy',
+                return_value=mock_android_device.MockAdbProxy('1'))
+    @mock.patch('mobly.controllers.android_device_lib.fastboot.FastbootProxy',
+                return_value=mock_android_device.MockFastbootProxy('1'))
+    @mock.patch(
+        'mobly.controllers.android_device.AndroidDevice.is_boot_completed',
+        side_effect=[
+            False, False,
+            adb.AdbTimeoutError(['adb', 'shell', 'getprop sys.boot_completed'],
+                                timeout=5,
+                                serial=1), False, False, False, False
+        ])
+    @mock.patch('time.sleep', return_value=None)
+    @mock.patch('time.time', side_effect=[0, 5, 10, 15, 20, 25, 30])
+    def test_AndroidDevice_wait_for_completion_never_boot(
+            self, MockTime, MockSleep, MockIsBootCompleted, FastbootProxy,
+            MockAdbProxy):
+        ad = android_device.AndroidDevice(serial='1')
+        raised = False
+        try:
+            with self.assertRaises(android_device.DeviceError):
+                ad.wait_for_boot_completion(timeout=20)
+        except (adb.AdbError, adb.AdbTimeoutError):
+            raised = True
+        self.assertFalse(
+            raised,
+            'adb.AdbError or adb.AdbTimeoutError exception raised but not handled.'
+        )
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mobly-1.8.1/tests/mobly/controllers/monsoon_test.py` & `mobly-1.9.1/tests/lib/integration3_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # Copyright 2018 Google Inc.
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
+# Licensed under the Apache License, Version 2.0 (the 'License');
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
+# distributed under the License is distributed on an 'AS IS' BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import platform
+from mobly import asserts
+from mobly import base_test
+from mobly import test_runner
 
-from future.tests.base import unittest
 
+class Integration3Test(base_test.BaseTestClass):
+    """This test class is used to cause a failure in integration tests."""
 
-class MonsoonTest(unittest.TestCase):
-    @unittest.skipIf(platform.system() == 'Windows',
-                     'fcntl does not exist on Windows')
-    def test_monsoon_import(self):
-        # TODO: Replace 'fnctl' with a Windows equivalent when on Windows
-        from mobly.controllers import monsoon
+    def setup_class(self):
+        asserts.fail('Setup failure.')
+
+    def on_fail(self, record):
+        asserts.abort_all('Skip tests.')
+
+    def test_empty(self):
+        pass
 
 
 if __name__ == '__main__':
-    unittest.main()
+    test_runner.main()
```

### Comparing `mobly-1.8.1/tests/mobly/records_test.py` & `mobly-1.9.1/tests/mobly/records_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         record1 = records.TestResultRecord(self.tn)
         record1.test_begin()
         record1.test_fail(s)
         dump_path = os.path.join(self.tmp_path, 'ha.yaml')
         writer = records.TestSummaryWriter(dump_path)
         writer.dump(record1.to_dict(), records.TestSummaryEntryType.RECORD)
         with io.open(dump_path, 'r', encoding='utf-8') as f:
-            content = yaml.load(f)
+            content = yaml.safe_load(f)
             self.assertEqual(content['Type'],
                              records.TestSummaryEntryType.RECORD.value)
             self.assertEqual(content[records.TestResultEnums.RECORD_DETAILS],
                              self.details)
             self.assertEqual(content[records.TestResultEnums.RECORD_EXTRAS],
                              self.float_extra)
 
@@ -376,15 +376,15 @@
         record1 = records.TestResultRecord(self.tn)
         record1.test_begin()
         record1.test_fail(s)
         dump_path = os.path.join(self.tmp_path, 'ha.yaml')
         writer = records.TestSummaryWriter(dump_path)
         writer.dump(record1.to_dict(), records.TestSummaryEntryType.RECORD)
         with io.open(dump_path, 'r', encoding='utf-8') as f:
-            content = yaml.load(f)
+            content = yaml.safe_load(f)
             self.assertEqual(content['Type'],
                              records.TestSummaryEntryType.RECORD.value)
             self.assertEqual(content[records.TestResultEnums.RECORD_DETAILS],
                              unicode_details)
             self.assertEqual(content[records.TestResultEnums.RECORD_EXTRAS],
                              unicode_extras)
 
@@ -394,15 +394,15 @@
         user_data = [user_data1, user_data2]
         dump_path = os.path.join(self.tmp_path, 'ha.yaml')
         writer = records.TestSummaryWriter(dump_path)
         for data in user_data:
             writer.dump(data, records.TestSummaryEntryType.USER_DATA)
         with io.open(dump_path, 'r', encoding='utf-8') as f:
             contents = []
-            for c in yaml.load_all(f):
+            for c in yaml.safe_load_all(f):
                 contents.append(c)
         for content in contents:
             self.assertEqual(content['Type'],
                              records.TestSummaryEntryType.USER_DATA.value)
         self.assertEqual(contents[0]['a'], user_data1['a'])
         self.assertEqual(contents[1]['b'], user_data2['b'])
 
@@ -423,10 +423,17 @@
             'SomeClass', 'MockDevice', ['magicA', 'magicB'])
         tr.add_controller_info_record(controller_info)
         self.assertTrue(tr.controller_info[0])
         self.assertEqual(tr.controller_info[0].controller_name, 'MockDevice')
         self.assertEqual(tr.controller_info[0].controller_info,
                          ['magicA', 'magicB'])
 
+    def test_uid(self):
+        @records.uid('some-uuid')
+        def test_uid_helper():
+            """Dummy test used by `test_uid` for testing the uid decorator."""
+
+        self.assertEqual(test_uid_helper.uid, 'some-uuid')
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mobly-1.8.1/tests/mobly/output_test.py` & `mobly-1.9.1/tests/mobly/output_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     from win32com import client
 
 
 class OutputTest(unittest.TestCase):
     """This test class has unit tests for the implementation of Mobly's output
     files.
     """
-
     def setUp(self):
         self.tmp_dir = tempfile.mkdtemp()
         self.base_mock_test_config = config_parser.TestRunConfig()
         self.base_mock_test_config.test_bed_name = 'SampleTestBed'
         self.base_mock_test_config.controller_configs = {}
         self.base_mock_test_config.user_params = {
             'icecream': 42,
@@ -90,22 +89,28 @@
         with io.open(log_path, 'r', encoding='utf-8') as f:
             content = f.read()
             for item in whitelist:
                 self.assertIn(item, content)
             for item in blacklist:
                 self.assertNotIn(item, content)
 
+    def test_yields_logging_path(self):
+        tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
+        with tr.mobly_logger() as log_path:
+            self.assertEqual(log_path, logging.log_path)
+
     @unittest.skipIf(platform.system() == 'Windows',
                      'Symlinks are usually specific to Unix operating systems')
     def test_symlink(self):
         """Verifies the symlink is created and links properly."""
         mock_test_config = self.create_mock_test_config(
             self.base_mock_test_config)
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.setup_logger()
+        with tr.mobly_logger():
+            pass
         symlink = os.path.join(self.log_dir, self.test_bed_name, 'latest')
         self.assertEqual(os.readlink(symlink), logging.log_path)
 
     @unittest.skipIf(platform.system() != 'Windows',
                      'Shortcuts are specific to Windows operating systems')
     def test_shortcut(self):
         """Verifies the shortcut is created and links properly."""
@@ -113,153 +118,203 @@
                                      'latest.lnk')
         shell = client.Dispatch("WScript.Shell")
         shortcut = shell.CreateShortCut(shortcut_path)
         self.assertFalse(shortcut.Targetpath)
         mock_test_config = self.create_mock_test_config(
             self.base_mock_test_config)
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.setup_logger()
-        tr._teardown_logger()
+        with tr.mobly_logger():
+            pass
         shortcut = shell.CreateShortCut(shortcut_path)
         # Normalize paths for case and truncation
         normalized_shortcut_path = os.path.normcase(
             win32file.GetLongPathName(shortcut.Targetpath))
         normalized_logger_path = os.path.normcase(
             win32file.GetLongPathName(logging.log_path))
         self.assertEqual(normalized_shortcut_path, normalized_logger_path)
 
-    def test_setup_logger_before_run(self):
+    @mock.patch('mobly.utils.create_alias')
+    def test_mobly_logger_with_default_latest_log_alias(
+            self, mock_create_alias):
+        mock_test_config = self.create_mock_test_config(
+            self.base_mock_test_config)
+        tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
+        with tr.mobly_logger():
+            pass
+        expected_alias_dir = os.path.join(self.log_dir, self.test_bed_name,
+                                          'latest')
+        mock_create_alias.assert_called_once_with(logging.log_path,
+                                                  expected_alias_dir)
+
+    @mock.patch('mobly.utils.create_alias')
+    def test_mobly_logger_with_custom_latest_log_alias(self,
+                                                       mock_create_alias):
+        mock_test_config = self.create_mock_test_config(
+            self.base_mock_test_config)
+        tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
+        with tr.mobly_logger(alias='history'):
+            pass
+        expected_alias_dir = os.path.join(self.log_dir, self.test_bed_name,
+                                          'history')
+        mock_create_alias.assert_called_once_with(logging.log_path,
+                                                  expected_alias_dir)
+
+    @mock.patch('mobly.utils.create_alias')
+    def test_mobly_logger_skips_latest_log_alias_when_none(
+            self, mock_create_alias):
+        mock_test_config = self.create_mock_test_config(
+            self.base_mock_test_config)
+        tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
+        with tr.mobly_logger(alias=None):
+            pass
+        mock_create_alias.asset_not_called()
+
+    @mock.patch('mobly.utils.create_alias')
+    def test_mobly_logger_skips_latest_log_alias_when_empty(
+            self, mock_create_alias):
+        mock_test_config = self.create_mock_test_config(
+            self.base_mock_test_config)
+        tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
+        with tr.mobly_logger(alias=''):
+            pass
+        mock_create_alias.asset_not_called()
+
+    def test_logging_before_run(self):
         """Verifies the expected output files from a test run.
 
         * Files are correctly created.
         * Basic sanity checks of each output file.
         """
         mock_test_config = self.create_mock_test_config(
             self.base_mock_test_config)
         info_uuid = 'e098d4ff-4e90-4e08-b369-aa84a7ef90ec'
         debug_uuid = 'c6f1474e-960a-4df8-8305-1c5b8b905eca'
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.setup_logger()
-        logging.info(info_uuid)
-        logging.debug(debug_uuid)
-        tr.add_test_class(mock_test_config, integration_test.IntegrationTest)
-        tr.run()
+        with tr.mobly_logger():
+            logging.info(info_uuid)
+            logging.debug(debug_uuid)
+            tr.add_test_class(mock_test_config,
+                              integration_test.IntegrationTest)
+            tr.run()
         output_dir = logging.log_path
         (summary_file_path, debug_log_path,
          info_log_path) = self.assert_output_logs_exist(output_dir)
-        self.assert_log_contents(
-            debug_log_path, whitelist=[debug_uuid, info_uuid])
-        self.assert_log_contents(
-            info_log_path, whitelist=[info_uuid], blacklist=[debug_uuid])
+        self.assert_log_contents(debug_log_path,
+                                 whitelist=[debug_uuid, info_uuid])
+        self.assert_log_contents(info_log_path,
+                                 whitelist=[info_uuid],
+                                 blacklist=[debug_uuid])
 
-    @mock.patch(
-        'mobly.logger.get_log_file_timestamp', side_effect=str(time.time()))
+    @mock.patch('mobly.logger.get_log_file_timestamp',
+                side_effect=str(time.time()))
     def test_run_twice_for_two_sets_of_logs(self, mock_timestamp):
         """Verifies the expected output files from a test run.
 
         * Files are correctly created.
         * Basic sanity checks of each output file.
         """
         mock_test_config = self.create_mock_test_config(
             self.base_mock_test_config)
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
         tr.add_test_class(mock_test_config, integration_test.IntegrationTest)
-        tr.setup_logger()
-        tr.run()
+        with tr.mobly_logger():
+            tr.run()
         output_dir1 = logging.log_path
-        tr.run()
+        with tr.mobly_logger():
+            tr.run()
         output_dir2 = logging.log_path
         self.assertNotEqual(output_dir1, output_dir2)
         self.assert_output_logs_exist(output_dir1)
         self.assert_output_logs_exist(output_dir2)
 
-    @mock.patch(
-        'mobly.logger.get_log_file_timestamp', side_effect=str(time.time()))
+    @mock.patch('mobly.logger.get_log_file_timestamp',
+                side_effect=str(time.time()))
     def test_teardown_erases_logs(self, mock_timestamp):
         """Verifies the expected output files from a test run.
 
         * Files are correctly created.
         * Basic sanity checks of each output file.
         """
         mock_test_config = self.create_mock_test_config(
             self.base_mock_test_config)
         info_uuid1 = '0c3ebb06-700d-496e-b015-62652da9e451'
         debug_uuid1 = '0c3ebb06-700d-496e-b015-62652da9e451'
         info_uuid2 = '484ef7db-f2dd-4b76-a126-c2f263e3808c'
         debug_uuid2 = 'd564da87-c42f-49c3-b0bf-18fa97cf0218'
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
 
-        tr.setup_logger()
-        logging.info(info_uuid1)
-        logging.debug(debug_uuid1)
-        tr._teardown_logger()
+        with tr.mobly_logger():
+            logging.info(info_uuid1)
+            logging.debug(debug_uuid1)
         output_dir1 = logging.log_path
 
-        tr.setup_logger()
-        logging.info(info_uuid2)
-        logging.debug(debug_uuid2)
-        tr._teardown_logger()
+        with tr.mobly_logger():
+            logging.info(info_uuid2)
+            logging.debug(debug_uuid2)
         output_dir2 = logging.log_path
 
         self.assertNotEqual(output_dir1, output_dir2)
 
         (summary_file_path1, debug_log_path1,
          info_log_path1) = self.get_output_logs(output_dir1)
         (summary_file_path2, debug_log_path2,
          info_log_path2) = self.get_output_logs(output_dir2)
 
-        self.assert_log_contents(
-            debug_log_path1,
-            whitelist=[debug_uuid1, info_uuid1],
-            blacklist=[info_uuid2, debug_uuid2])
-        self.assert_log_contents(
-            debug_log_path2,
-            whitelist=[debug_uuid2, info_uuid2],
-            blacklist=[info_uuid1, debug_uuid1])
+        self.assert_log_contents(debug_log_path1,
+                                 whitelist=[debug_uuid1, info_uuid1],
+                                 blacklist=[info_uuid2, debug_uuid2])
+        self.assert_log_contents(debug_log_path2,
+                                 whitelist=[debug_uuid2, info_uuid2],
+                                 blacklist=[info_uuid1, debug_uuid1])
 
     def test_basic_output(self):
         """Verifies the expected output files from a test run.
 
         * Files are correctly created.
         * Basic sanity checks of each output file.
         """
         mock_test_config = self.create_mock_test_config(
             self.base_mock_test_config)
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.add_test_class(mock_test_config, integration_test.IntegrationTest)
-        tr.run()
+        with tr.mobly_logger():
+            tr.add_test_class(mock_test_config,
+                              integration_test.IntegrationTest)
+            tr.run()
         output_dir = logging.log_path
         (summary_file_path, debug_log_path,
          info_log_path) = self.assert_output_logs_exist(output_dir)
         summary_entries = []
         with io.open(summary_file_path, 'r', encoding='utf-8') as f:
-            for entry in yaml.load_all(f):
+            for entry in yaml.safe_load_all(f):
                 self.assertTrue(entry['Type'])
                 summary_entries.append(entry)
         self.assert_log_contents(debug_log_path, whitelist=['DEBUG', 'INFO'])
-        self.assert_log_contents(
-            info_log_path, whitelist=['INFO'], blacklist=['DEBUG'])
+        self.assert_log_contents(info_log_path,
+                                 whitelist=['INFO'],
+                                 blacklist=['DEBUG'])
 
     def test_teardown_class_output(self):
         """Verifies the summary file includes the failure record for
         teardown_class.
         """
         mock_test_config = self.base_mock_test_config.copy()
         tr = test_runner.TestRunner(self.log_dir, self.test_bed_name)
-        tr.add_test_class(mock_test_config,
-                          teardown_class_failure_test.TearDownClassFailureTest)
-        tr.run()
+        with tr.mobly_logger():
+            tr.add_test_class(
+                mock_test_config,
+                teardown_class_failure_test.TearDownClassFailureTest)
+            tr.run()
         output_dir = logging.log_path
         summary_file_path = os.path.join(output_dir,
                                          records.OUTPUT_FILE_SUMMARY)
         found = False
         with io.open(summary_file_path, 'r', encoding='utf-8') as f:
             raw_content = f.read()
             f.seek(0)
-            for entry in yaml.load_all(f):
+            for entry in yaml.safe_load_all(f):
                 if (entry['Type'] == 'Record'
                         and entry[records.TestResultEnums.RECORD_NAME] ==
                         'teardown_class'):
                     found = True
                     break
             self.assertTrue(
                 found,
```

### Comparing `mobly-1.8.1/tests/lib/integration2_test.py` & `mobly-1.9.1/tests/lib/integration2_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/lib/mock_instrumentation_test.py` & `mobly-1.9.1/tests/lib/mock_instrumentation_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/lib/mock_second_controller.py` & `mobly-1.9.1/tests/lib/mock_second_controller.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/lib/teardown_class_failure_test.py` & `mobly-1.9.1/tests/lib/teardown_class_failure_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/lib/mock_controller.py` & `mobly-1.9.1/tests/lib/mock_controller.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/lib/utils.py` & `mobly-1.9.1/tests/lib/utils.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/lib/jsonrpc_client_test_base.py` & `mobly-1.9.1/tests/lib/jsonrpc_client_test_base.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/tests/lib/integration_test.py` & `mobly-1.9.1/tests/lib/integration_test.py`

 * *Files identical despite different names*

### Comparing `mobly-1.8.1/mobly.egg-info/SOURCES.txt` & `mobly-1.9.1/mobly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 mobly/controllers/attenuator_lib/minicircuits.py
 mobly/controllers/attenuator_lib/telnet_scpi_client.py
 mobly/controllers/sniffer_lib/__init__.py
 mobly/controllers/sniffer_lib/local/__init__.py
 mobly/controllers/sniffer_lib/local/local_base.py
 mobly/controllers/sniffer_lib/local/tcpdump.py
 mobly/controllers/sniffer_lib/local/tshark.py
-tests/__init__.py
 tests/lib/__init__.py
 tests/lib/integration2_test.py
 tests/lib/integration3_test.py
 tests/lib/integration_test.py
 tests/lib/jsonrpc_client_test_base.py
 tests/lib/mock_android_device.py
 tests/lib/mock_controller.py
@@ -81,14 +80,15 @@
 tests/mobly/controllers/android_device_test.py
 tests/mobly/controllers/monsoon_test.py
 tests/mobly/controllers/android_device_lib/__init__.py
 tests/mobly/controllers/android_device_lib/adb_test.py
 tests/mobly/controllers/android_device_lib/callback_handler_test.py
 tests/mobly/controllers/android_device_lib/errors_test.py
 tests/mobly/controllers/android_device_lib/jsonrpc_client_base_test.py
+tests/mobly/controllers/android_device_lib/jsonrpc_shell_base_test.py
 tests/mobly/controllers/android_device_lib/service_manager_test.py
 tests/mobly/controllers/android_device_lib/sl4a_client_test.py
 tests/mobly/controllers/android_device_lib/snippet_client_test.py
 tests/mobly/controllers/android_device_lib/snippet_event_test.py
 tests/mobly/controllers/android_device_lib/services/__init__.py
 tests/mobly/controllers/android_device_lib/services/logcat_test.py
 tests/mobly/controllers/android_device_lib/services/sl4a_service_test.py
```

### Comparing `mobly-1.8.1/README.md` & `mobly-1.9.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
 While developed by Googlers, Mobly is not an official Google product.
 
 ## Compatibility
 
 Mobly is compatible with both *python 3.4+* and *python 2.7*.
 
+NOTE: As part of the bigger [communitiy initiative](https://python3statement.org/),
+we are planning to drop Python 2.7 support at the end of 2019.
+
 Mobly tests could run on the following platforms:
   - Ubuntu 14.04+
   - MacOS 10.6+
   - Windows 7+
 
 | Platform | Build Status |
 |----------|--------------|
```

### Comparing `mobly-1.8.1/setup.py` & `mobly-1.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,27 +48,28 @@
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 
 def main():
     setuptools.setup(
         name='mobly',
-        version='1.8.1',
+        version='1.9.1',
         maintainer='Ang Li',
         maintainer_email='mobly-github@googlegroups.com',
         description='Automation framework for special end-to-end test cases',
         license='Apache2.0',
         url='https://github.com/google/mobly',
-        download_url='https://github.com/google/mobly/tarball/1.8.1',
-        packages=setuptools.find_packages(),
+        download_url='https://github.com/google/mobly/tarball/1.9.1',
+        packages=setuptools.find_packages(exclude=['tests']),
         include_package_data=False,
         scripts=['tools/sl4a_shell.py', 'tools/snippet_shell.py'],
         tests_require=[
             'mock',
-            'pytest',
+            # Needed for supporting Python 2 because this release stopped supporting Python 2.
+            'pytest<5.0.0',
             'pytz',
         ],
         install_requires=install_requires,
         cmdclass={'test': PyTest},
     )
```

