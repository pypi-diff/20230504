# Comparing `tmp/aps_common_libraries-1.0.2.tar.gz` & `tmp/aps_common_libraries-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps_common_libraries-1.0.2.tar", last modified: Tue Apr 11 22:35:08 2023, max compression
+gzip compressed data, was "aps_common_libraries-1.0.3.tar", last modified: Wed May  3 22:26:21 2023, max compression
```

## Comparing `aps_common_libraries-1.0.2.tar` & `aps_common_libraries-1.0.3.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.324373 aps_common_libraries-1.0.2/
--rw-rw-rw-   0 bishop    (1601)      907     1080 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.2/LICENSE
--rw-rw-rw-   0 bishop    (1601)      907    10366 2022-10-17 22:57:50.000000 aps_common_libraries-1.0.2/LICENSE.pdf
--rw-rw-rw-   0 bishop    (1601)      907       66 2022-10-17 22:57:24.000000 aps_common_libraries-1.0.2/MANIFEST.in
--rw-r--r--   0 bishop    (1601)      907      876 2023-04-11 22:35:08.323834 aps_common_libraries-1.0.2/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907       46 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.2/README.md
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.254948 aps_common_libraries-1.0.2/aps/
--rw-rw-rw-   0 bishop    (1601)      907     3471 2022-10-17 23:25:46.000000 aps_common_libraries-1.0.2/aps/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.262629 aps_common_libraries-1.0.2/aps/common/
--rw-rw-rw-   0 bishop    (1601)      907     3426 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.2/aps/common/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.265199 aps_common_libraries-1.0.2/aps/common/__test/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2023-02-17 17:17:14.000000 aps_common_libraries-1.0.2/aps/common/__test/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907      548 2023-02-17 17:54:05.000000 aps_common_libraries-1.0.2/aps/common/__test/test.py
--rw-rw-rw-   0 bishop    (1601)      907    10103 2022-11-23 21:10:21.000000 aps_common_libraries-1.0.2/aps/common/initializer.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.270137 aps_common_libraries-1.0.2/aps/common/io/
--rw-rw-rw-   0 bishop    (1601)      907     3344 2020-03-28 16:44:28.000000 aps_common_libraries-1.0.2/aps/common/io/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4627 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.2/aps/common/io/printout.py
--rw-rw-rw-   0 bishop    (1601)      907     4434 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.2/aps/common/io/tcp_client.py
--rw-rw-rw-   0 bishop    (1601)      907     8754 2022-10-17 22:43:33.000000 aps_common_libraries-1.0.2/aps/common/io/tiff_file.py
--rw-rw-rw-   0 bishop    (1601)      907    20742 2023-02-17 23:08:47.000000 aps_common_libraries-1.0.2/aps/common/logger.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.271532 aps_common_libraries-1.0.2/aps/common/measurment/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:27:18.000000 aps_common_libraries-1.0.2/aps/common/measurment/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.275503 aps_common_libraries-1.0.2/aps/common/measurment/beamline/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:31:01.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/__init__.py
--rw-r--r--   0 bishop    (1601)      907    10472 2023-03-29 01:21:24.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/image_collector.py
--rw-r--r--   0 bishop    (1601)      907    32561 2023-03-31 13:27:26.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/image_processor.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.294013 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/
--rw-rw-rw-   0 bishop    (1601)      907     5297 2022-10-28 18:51:12.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/SPINNet_estimate.py
--rw-rw-rw-   0 bishop    (1601)      907    45615 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/WXST.py
--rw-rw-rw-   0 bishop    (1601)      907     3453 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    15218 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/diffraction_process.py
--rw-rw-rw-   0 bishop    (1601)      907      872 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/euclidean_dist.py
--rw-rw-rw-   0 bishop    (1601)      907    19167 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/func.py
--rw-rw-rw-   0 bishop    (1601)      907    23426 2022-11-04 20:56:51.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/func_light.py
--rw-rw-rw-   0 bishop    (1601)      907     2315 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/gui_func.py
--rw-rw-rw-   0 bishop    (1601)      907     6834 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/integration.py
--rw-rw-rw-   0 bishop    (1601)      907    77489 2023-03-31 13:34:40.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/main.py
--rw-rw-rw-   0 bishop    (1601)      907     5964 2022-11-07 15:35:41.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/pattern_find.py
--rw-rw-rw-   0 bishop    (1601)      907     7296 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/pattern_propagate.py
--rw-rw-rw-   0 bishop    (1601)      907      184 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/utils.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.297579 aps_common_libraries-1.0.2/aps/common/ml/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-08 02:45:45.000000 aps_common_libraries-1.0.2/aps/common/ml/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     6469 2021-09-23 22:14:46.000000 aps_common_libraries-1.0.2/aps/common/ml/data_structures.py
--rw-rw-rw-   0 bishop    (1601)      907     4889 2021-12-22 20:56:40.000000 aps_common_libraries-1.0.2/aps/common/ml/mocks.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.301579 aps_common_libraries-1.0.2/aps/common/plot/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.2/aps/common/plot/__init__.py
--rw-r--r--   0 bishop    (1601)      907    44717 2023-04-08 13:27:45.000000 aps_common_libraries-1.0.2/aps/common/plot/gui.py
--rw-rw-rw-   0 bishop    (1601)      907     4639 2022-11-18 03:11:28.000000 aps_common_libraries-1.0.2/aps/common/plot/image.py
--rw-rw-rw-   0 bishop    (1601)      907     6365 2023-02-16 16:28:45.000000 aps_common_libraries-1.0.2/aps/common/plot/qt_application.py
--rw-rw-rw-   0 bishop    (1601)      907    16718 2023-02-16 16:35:31.000000 aps_common_libraries-1.0.2/aps/common/plotter.py
--rw-rw-rw-   0 bishop    (1601)      907     5129 2023-03-01 01:27:25.000000 aps_common_libraries-1.0.2/aps/common/registry.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.310701 aps_common_libraries-1.0.2/aps/common/scripts/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-10 21:26:33.000000 aps_common_libraries-1.0.2/aps/common/scripts/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     3533 2023-02-07 22:57:08.000000 aps_common_libraries-1.0.2/aps/common/scripts/abstract_command_line_script.py
--rw-rw-rw-   0 bishop    (1601)      907     3430 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.2/aps/common/scripts/generic_process_manager.py
--rw-rw-rw-   0 bishop    (1601)      907     7941 2023-02-17 23:04:17.000000 aps_common_libraries-1.0.2/aps/common/scripts/generic_qt_script.py
--rw-rw-rw-   0 bishop    (1601)      907     4121 2023-02-07 23:10:48.000000 aps_common_libraries-1.0.2/aps/common/scripts/script_data.py
--rw-rw-rw-   0 bishop    (1601)      907     4576 2022-11-10 17:23:20.000000 aps_common_libraries-1.0.2/aps/common/scripts/script_registry.py
--rw-rw-rw-   0 bishop    (1601)      907     4333 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.2/aps/common/singleton.py
--rw-rw-rw-   0 bishop    (1601)      907    10071 2022-11-28 18:33:01.000000 aps_common_libraries-1.0.2/aps/common/traffic_light.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.316307 aps_common_libraries-1.0.2/aps/common/widgets/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.2/aps/common/widgets/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4081 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.2/aps/common/widgets/close_app_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     5532 2023-02-27 21:48:03.000000 aps_common_libraries-1.0.2/aps/common/widgets/context_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     8506 2023-02-14 01:08:20.000000 aps_common_libraries-1.0.2/aps/common/widgets/generic_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     6095 2023-02-17 18:06:20.000000 aps_common_libraries-1.0.2/aps/common/widgets/log_stream_widget.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-04-11 22:35:08.322829 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/
--rw-rw-rw-   0 bishop    (1601)      907      876 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907     2130 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/SOURCES.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/dependency_links.txt
--rw-rw-rw-   0 bishop    (1601)      907       15 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/namespace_packages.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2022-10-17 23:01:46.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/not-zip-safe
--rw-rw-rw-   0 bishop    (1601)      907      150 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/requires.txt
--rw-rw-rw-   0 bishop    (1601)      907        4 2023-04-11 22:35:08.000000 aps_common_libraries-1.0.2/aps_common_libraries.egg-info/top_level.txt
--rw-r--r--   0 bishop    (1601)      907       38 2023-04-11 22:35:08.324585 aps_common_libraries-1.0.2/setup.cfg
--rw-r--r--   0 bishop    (1601)      907     5571 2023-04-11 22:34:49.000000 aps_common_libraries-1.0.2/setup.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.450199 aps_common_libraries-1.0.3/
+-rw-rw-rw-   0 bishop    (1601)      907     1080 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.3/LICENSE
+-rw-rw-rw-   0 bishop    (1601)      907    10366 2022-10-17 22:57:50.000000 aps_common_libraries-1.0.3/LICENSE.pdf
+-rw-rw-rw-   0 bishop    (1601)      907       66 2022-10-17 22:57:24.000000 aps_common_libraries-1.0.3/MANIFEST.in
+-rw-r--r--   0 bishop    (1601)      907      876 2023-05-03 22:26:21.449545 aps_common_libraries-1.0.3/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907       46 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.3/README.md
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.388129 aps_common_libraries-1.0.3/aps/
+-rw-rw-rw-   0 bishop    (1601)      907     3471 2022-10-17 23:25:46.000000 aps_common_libraries-1.0.3/aps/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.394898 aps_common_libraries-1.0.3/aps/common/
+-rw-rw-rw-   0 bishop    (1601)      907     3426 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.3/aps/common/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.396389 aps_common_libraries-1.0.3/aps/common/__test/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2023-02-17 17:17:14.000000 aps_common_libraries-1.0.3/aps/common/__test/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907      548 2023-02-17 17:54:05.000000 aps_common_libraries-1.0.3/aps/common/__test/test.py
+-rw-rw-rw-   0 bishop    (1601)      907    10103 2022-11-23 21:10:21.000000 aps_common_libraries-1.0.3/aps/common/initializer.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.399582 aps_common_libraries-1.0.3/aps/common/io/
+-rw-rw-rw-   0 bishop    (1601)      907     3344 2020-03-28 16:44:28.000000 aps_common_libraries-1.0.3/aps/common/io/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     4627 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.3/aps/common/io/printout.py
+-rw-rw-rw-   0 bishop    (1601)      907     4434 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.3/aps/common/io/tcp_client.py
+-rw-rw-rw-   0 bishop    (1601)      907     8754 2022-10-17 22:43:33.000000 aps_common_libraries-1.0.3/aps/common/io/tiff_file.py
+-rw-rw-rw-   0 bishop    (1601)      907    20742 2023-02-17 23:08:47.000000 aps_common_libraries-1.0.3/aps/common/logger.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.400336 aps_common_libraries-1.0.3/aps/common/measurment/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:27:18.000000 aps_common_libraries-1.0.3/aps/common/measurment/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.403180 aps_common_libraries-1.0.3/aps/common/measurment/beamline/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:31:01.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/__init__.py
+-rw-r--r--   0 bishop    (1601)      907    10472 2023-03-29 01:21:24.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/image_collector.py
+-rw-r--r--   0 bishop    (1601)      907    32561 2023-03-31 13:27:26.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/image_processor.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.418203 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/
+-rw-rw-rw-   0 bishop    (1601)      907     5297 2022-10-28 18:51:12.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/SPINNet_estimate.py
+-rw-rw-rw-   0 bishop    (1601)      907    45615 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/WXST.py
+-rw-rw-rw-   0 bishop    (1601)      907     3453 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    15218 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/diffraction_process.py
+-rw-rw-rw-   0 bishop    (1601)      907      872 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/euclidean_dist.py
+-rw-rw-rw-   0 bishop    (1601)      907    19167 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/func.py
+-rw-rw-rw-   0 bishop    (1601)      907    23426 2022-11-04 20:56:51.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/func_light.py
+-rw-rw-rw-   0 bishop    (1601)      907     2315 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/gui_func.py
+-rw-rw-rw-   0 bishop    (1601)      907     6834 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/integration.py
+-rw-rw-rw-   0 bishop    (1601)      907    77489 2023-03-31 13:34:40.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/main.py
+-rw-rw-rw-   0 bishop    (1601)      907     5964 2022-11-07 15:35:41.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/pattern_find.py
+-rw-rw-rw-   0 bishop    (1601)      907     7296 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/pattern_propagate.py
+-rw-rw-rw-   0 bishop    (1601)      907      184 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/utils.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.421613 aps_common_libraries-1.0.3/aps/common/ml/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-08 02:45:45.000000 aps_common_libraries-1.0.3/aps/common/ml/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     6469 2021-09-23 22:14:46.000000 aps_common_libraries-1.0.3/aps/common/ml/data_structures.py
+-rw-rw-rw-   0 bishop    (1601)      907     4889 2021-12-22 20:56:40.000000 aps_common_libraries-1.0.3/aps/common/ml/mocks.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.426529 aps_common_libraries-1.0.3/aps/common/plot/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.3/aps/common/plot/__init__.py
+-rw-r--r--   0 bishop    (1601)      907    44717 2023-04-08 13:27:45.000000 aps_common_libraries-1.0.3/aps/common/plot/gui.py
+-rw-rw-rw-   0 bishop    (1601)      907     4639 2022-11-18 03:11:28.000000 aps_common_libraries-1.0.3/aps/common/plot/image.py
+-rw-rw-rw-   0 bishop    (1601)      907     6365 2023-02-16 16:28:45.000000 aps_common_libraries-1.0.3/aps/common/plot/qt_application.py
+-rw-rw-rw-   0 bishop    (1601)      907    16718 2023-02-16 16:35:31.000000 aps_common_libraries-1.0.3/aps/common/plotter.py
+-rw-r--r--   0 bishop    (1601)      907     5229 2023-05-02 21:11:06.000000 aps_common_libraries-1.0.3/aps/common/reflection.py
+-rw-rw-rw-   0 bishop    (1601)      907     5129 2023-03-01 01:27:25.000000 aps_common_libraries-1.0.3/aps/common/registry.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.433643 aps_common_libraries-1.0.3/aps/common/scripts/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-10 21:26:33.000000 aps_common_libraries-1.0.3/aps/common/scripts/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     3533 2023-02-07 22:57:08.000000 aps_common_libraries-1.0.3/aps/common/scripts/abstract_command_line_script.py
+-rw-rw-rw-   0 bishop    (1601)      907     3430 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.3/aps/common/scripts/generic_process_manager.py
+-rw-rw-rw-   0 bishop    (1601)      907     7941 2023-02-17 23:04:17.000000 aps_common_libraries-1.0.3/aps/common/scripts/generic_qt_script.py
+-rw-rw-rw-   0 bishop    (1601)      907     4121 2023-02-07 23:10:48.000000 aps_common_libraries-1.0.3/aps/common/scripts/script_data.py
+-rw-rw-rw-   0 bishop    (1601)      907     4576 2022-11-10 17:23:20.000000 aps_common_libraries-1.0.3/aps/common/scripts/script_registry.py
+-rw-rw-rw-   0 bishop    (1601)      907     4333 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.3/aps/common/singleton.py
+-rw-rw-rw-   0 bishop    (1601)      907    10071 2022-11-28 18:33:01.000000 aps_common_libraries-1.0.3/aps/common/traffic_light.py
+-rw-r--r--   0 bishop    (1601)      907     3543 2023-05-03 14:01:58.000000 aps_common_libraries-1.0.3/aps/common/utilities.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.441075 aps_common_libraries-1.0.3/aps/common/widgets/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.3/aps/common/widgets/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     4081 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.3/aps/common/widgets/close_app_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     5532 2023-02-27 21:48:03.000000 aps_common_libraries-1.0.3/aps/common/widgets/context_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     8506 2023-02-14 01:08:20.000000 aps_common_libraries-1.0.3/aps/common/widgets/generic_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     6095 2023-02-17 18:06:20.000000 aps_common_libraries-1.0.3/aps/common/widgets/log_stream_widget.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-03 22:26:21.448412 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/
+-rw-rw-rw-   0 bishop    (1601)      907      876 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907     2179 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/SOURCES.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/dependency_links.txt
+-rw-rw-rw-   0 bishop    (1601)      907       15 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/namespace_packages.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2022-10-17 23:01:46.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/not-zip-safe
+-rw-rw-rw-   0 bishop    (1601)      907      150 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/requires.txt
+-rw-rw-rw-   0 bishop    (1601)      907        4 2023-05-03 22:26:21.000000 aps_common_libraries-1.0.3/aps_common_libraries.egg-info/top_level.txt
+-rw-r--r--   0 bishop    (1601)      907       38 2023-05-03 22:26:21.451750 aps_common_libraries-1.0.3/setup.cfg
+-rw-r--r--   0 bishop    (1601)      907     5571 2023-05-02 20:51:39.000000 aps_common_libraries-1.0.3/setup.py
```

### Comparing `aps_common_libraries-1.0.2/LICENSE` & `aps_common_libraries-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/LICENSE.pdf` & `aps_common_libraries-1.0.3/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/PKG-INFO` & `aps_common_libraries-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aps_common_libraries
-Version: 1.0.2
+Version: 1.0.3
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
```

### Comparing `aps_common_libraries-1.0.2/aps/__init__.py` & `aps_common_libraries-1.0.3/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/__init__.py` & `aps_common_libraries-1.0.3/aps/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/__test/__init__.py` & `aps_common_libraries-1.0.3/aps/common/__test/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/__test/test.py` & `aps_common_libraries-1.0.3/aps/common/__test/test.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/initializer.py` & `aps_common_libraries-1.0.3/aps/common/initializer.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/io/__init__.py` & `aps_common_libraries-1.0.3/aps/common/io/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/io/printout.py` & `aps_common_libraries-1.0.3/aps/common/io/printout.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/io/tcp_client.py` & `aps_common_libraries-1.0.3/aps/common/io/tcp_client.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/io/tiff_file.py` & `aps_common_libraries-1.0.3/aps/common/io/tiff_file.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/logger.py` & `aps_common_libraries-1.0.3/aps/common/logger.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/__init__.py` & `aps_common_libraries-1.0.3/aps/common/measurment/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/__init__.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/image_collector.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/image_collector.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/image_processor.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/image_processor.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/SPINNet_estimate.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/SPINNet_estimate.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/WXST.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/WXST.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/__init__.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/diffraction_process.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/diffraction_process.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/euclidean_dist.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/euclidean_dist.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/func.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/func.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/func_light.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/func_light.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/gui_func.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/gui_func.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/integration.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/integration.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/main.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/main.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/pattern_find.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/pattern_find.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/measurment/beamline/wf/pattern_propagate.py` & `aps_common_libraries-1.0.3/aps/common/measurment/beamline/wf/pattern_propagate.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/ml/__init__.py` & `aps_common_libraries-1.0.3/aps/common/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/ml/data_structures.py` & `aps_common_libraries-1.0.3/aps/common/ml/data_structures.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/ml/mocks.py` & `aps_common_libraries-1.0.3/aps/common/ml/mocks.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/plot/__init__.py` & `aps_common_libraries-1.0.3/aps/common/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/plot/gui.py` & `aps_common_libraries-1.0.3/aps/common/plot/gui.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/plot/image.py` & `aps_common_libraries-1.0.3/aps/common/plot/image.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/plot/qt_application.py` & `aps_common_libraries-1.0.3/aps/common/plot/qt_application.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/plotter.py` & `aps_common_libraries-1.0.3/aps/common/plotter.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/registry.py` & `aps_common_libraries-1.0.3/aps/common/registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/scripts/__init__.py` & `aps_common_libraries-1.0.3/aps/common/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/scripts/abstract_command_line_script.py` & `aps_common_libraries-1.0.3/aps/common/scripts/abstract_command_line_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/scripts/generic_process_manager.py` & `aps_common_libraries-1.0.3/aps/common/scripts/generic_process_manager.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/scripts/generic_qt_script.py` & `aps_common_libraries-1.0.3/aps/common/scripts/generic_qt_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/scripts/script_data.py` & `aps_common_libraries-1.0.3/aps/common/scripts/script_data.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/scripts/script_registry.py` & `aps_common_libraries-1.0.3/aps/common/scripts/script_registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/singleton.py` & `aps_common_libraries-1.0.3/aps/common/singleton.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/traffic_light.py` & `aps_common_libraries-1.0.3/aps/common/traffic_light.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/widgets/__init__.py` & `aps_common_libraries-1.0.3/aps/common/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/widgets/close_app_widget.py` & `aps_common_libraries-1.0.3/aps/common/widgets/close_app_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/widgets/context_widget.py` & `aps_common_libraries-1.0.3/aps/common/widgets/context_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/widgets/generic_widget.py` & `aps_common_libraries-1.0.3/aps/common/widgets/generic_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps/common/widgets/log_stream_widget.py` & `aps_common_libraries-1.0.3/aps/common/widgets/log_stream_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.2/aps_common_libraries.egg-info/PKG-INFO` & `aps_common_libraries-1.0.3/aps_common_libraries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aps-common-libraries
-Version: 1.0.2
+Version: 1.0.3
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
```

### Comparing `aps_common_libraries-1.0.2/aps_common_libraries.egg-info/SOURCES.txt` & `aps_common_libraries-1.0.3/aps_common_libraries.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 README.md
 setup.py
 aps/__init__.py
 aps/common/__init__.py
 aps/common/initializer.py
 aps/common/logger.py
 aps/common/plotter.py
+aps/common/reflection.py
 aps/common/registry.py
 aps/common/singleton.py
 aps/common/traffic_light.py
+aps/common/utilities.py
 aps/common/__test/__init__.py
 aps/common/__test/test.py
 aps/common/io/__init__.py
 aps/common/io/printout.py
 aps/common/io/tcp_client.py
 aps/common/io/tiff_file.py
 aps/common/measurment/__init__.py
```

### Comparing `aps_common_libraries-1.0.2/setup.py` & `aps_common_libraries-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'aps_common_libraries'
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 ISRELEASED = False
 
 DESCRIPTION = 'APS Common Libraries'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov'
```

