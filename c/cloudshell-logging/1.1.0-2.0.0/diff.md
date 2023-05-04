# Comparing `tmp/cloudshell-logging-1.1.0.zip` & `tmp/cloudshell-logging-2.0.0.zip`

## zipinfo {}

```diff
@@ -1,40 +1,57 @@
-Zip file size: 20420 bytes, number of entries: 38
-drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-12 14:14 cloudshell-logging-1.1.0/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell_logging.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/
--rw-r--r--  2.0 unx      734 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/setup.py
--rw-r--r--  2.0 unx        6 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/version.txt
--rw-r--r--  2.0 unx      238 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/PKG-INFO
--rw-r--r--  2.0 unx      118 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/dev_requirements.txt
--rw-r--r--  2.0 unx       44 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/test_requirements.txt
--rw-r--r--  2.0 unx       38 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/setup.cfg
--rw-r--r--  2.0 unx     4723 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/README.md
--rw-r--r--  2.0 unx        0 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/requirements.txt
--rw-r--r--  2.0 unx     1160 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/tox.ini
--rw-r--r--  2.0 unx       34 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/MANIFEST.in
--rw-r--r--  2.0 unx      238 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell_logging.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      852 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell_logging.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell_logging.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       17 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell_logging.egg-info/top_level.txt
-drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/logging/
--rw-r--r--  2.0 unx        0 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/logging/utils/
--rw-r--r--  2.0 unx    11952 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/logging/test_qs_logger.py
--rw-r--r--  2.0 unx     2332 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/logging/test_qs_config_parser.py
--rw-r--r--  2.0 unx        0 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/logging/__init__.py
--rw-r--r--  2.0 unx      297 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/logging/test_qs_config.ini
--rw-r--r--  2.0 unx     1013 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/logging/utils/test_error_handling_context_manager.py
--rw-r--r--  2.0 unx        0 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/tests/logging/utils/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/
--rw-r--r--  2.0 unx       76 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/utils/
--rw-r--r--  2.0 unx      543 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/qs_config.ini
--rw-r--r--  2.0 unx     2490 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/interprocess_logger.py
--rw-r--r--  2.0 unx     1107 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/qs_config_parser.py
--rw-r--r--  2.0 unx        0 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/__init__.py
--rw-r--r--  2.0 unx    11191 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/qs_logger.py
--rw-r--r--  2.0 unx     1061 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/utils/decorators.py
--rw-r--r--  2.0 unx     1096 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/utils/error_handling_context_manager.py
--rw-r--r--  2.0 unx        0 b- defN 21-Apr-12 14:14 cloudshell-logging-1.1.0/cloudshell/logging/utils/__init__.py
-38 files, 41361 bytes uncompressed, 13680 bytes compressed:  66.9%
+Zip file size: 48822 bytes, number of entries: 55
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/
+-rw-r--r--  2.0 unx    97622 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/LICENSE.htm
+-rw-r--r--  2.0 unx       18 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/test_requirements.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/version.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/setup.cfg
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/requirements.txt
+-rw-r--r--  2.0 unx      776 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/setup.py
+-rw-r--r--  2.0 unx       71 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/dev_requirements.txt
+-rw-r--r--  2.0 unx     4723 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/README.md
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tox.ini
+-rw-r--r--  2.0 unx       34 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx      254 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/
+-rw-r--r--  2.0 unx       76 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/
+-rw-r--r--  2.0 unx    13248 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/qs_logger.py
+-rw-r--r--  2.0 unx      970 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/qs_config_parser.py
+-rw-r--r--  2.0 unx     1537 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/context_filters.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/__init__.py
+-rw-r--r--  2.0 unx     1648 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/memory_handler.py
+-rw-r--r--  2.0 unx      712 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/qs_config.ini
+-rw-r--r--  2.0 unx      198 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/venv.py
+-rw-r--r--  2.0 unx      927 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/patch_logging_shutdown.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/error_handling_context_manager.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/__init__.py
+-rw-r--r--  2.0 unx      681 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/decorators.py
+-rw-r--r--  2.0 unx     1020 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/log_exec_info.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_debug_logs/
+-rw-r--r--  2.0 unx      287 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/conftest.py
+-rw-r--r--  2.0 unx     2505 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_memory_handler.py
+-rw-r--r--  2.0 unx     2290 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_qs_config_parser.py
+-rw-r--r--  2.0 unx    12256 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_qs_logger.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/__init__.py
+-rw-r--r--  2.0 unx      297 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_qs_config.ini
+-rw-r--r--  2.0 unx     1815 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_log_exec_info.py
+-rw-r--r--  2.0 unx     5264 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/test_getting_logger.py
+-rw-r--r--  2.0 unx      163 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/package_file.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/__init__.py
+-rw-r--r--  2.0 unx     1750 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/utils/test_command_logging.py
+-rw-r--r--  2.0 unx      923 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/utils/test_error_handling_context_manager.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/utils/__init__.py
+-rw-r--r--  2.0 unx      388 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_debug_logs/package_file.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_debug_logs/__init__.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_debug_logs/test_debug_logs_on_error.py
+-rw-r--r--  2.0 unx       17 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1474 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      254 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/dependency_links.txt
+55 files, 158291 bytes uncompressed, 38592 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,115 +1,166 @@
-Filename: cloudshell-logging-1.1.0/
+Filename: cloudshell-logging-2.0.0/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell_logging.egg-info/
+Filename: cloudshell-logging-2.0.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/
+Filename: cloudshell-logging-2.0.0/tests/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/
+Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/setup.py
+Filename: cloudshell-logging-2.0.0/LICENSE.htm
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/version.txt
+Filename: cloudshell-logging-2.0.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/PKG-INFO
+Filename: cloudshell-logging-2.0.0/version.txt
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/dev_requirements.txt
+Filename: cloudshell-logging-2.0.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/test_requirements.txt
+Filename: cloudshell-logging-2.0.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/setup.cfg
+Filename: cloudshell-logging-2.0.0/setup.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/README.md
+Filename: cloudshell-logging-2.0.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/requirements.txt
+Filename: cloudshell-logging-2.0.0/README.md
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tox.ini
+Filename: cloudshell-logging-2.0.0/tox.ini
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/MANIFEST.in
+Filename: cloudshell-logging-2.0.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell_logging.egg-info/PKG-INFO
+Filename: cloudshell-logging-2.0.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell_logging.egg-info/SOURCES.txt
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell_logging.egg-info/dependency_links.txt
+Filename: cloudshell-logging-2.0.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell_logging.egg-info/top_level.txt
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/logging/
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/qs_logger.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/__init__.py
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/qs_config_parser.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/logging/utils/
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/context_filters.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/logging/test_qs_logger.py
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/logging/test_qs_config_parser.py
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/memory_handler.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/logging/__init__.py
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/qs_config.ini
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/logging/test_qs_config.ini
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/venv.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/logging/utils/test_error_handling_context_manager.py
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/patch_logging_shutdown.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/tests/logging/utils/__init__.py
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/error_handling_context_manager.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/__init__.py
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/decorators.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/utils/
+Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/log_exec_info.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/qs_config.ini
+Filename: cloudshell-logging-2.0.0/tests/logging/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/interprocess_logger.py
+Filename: cloudshell-logging-2.0.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/qs_config_parser.py
+Filename: cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/__init__.py
+Filename: cloudshell-logging-2.0.0/tests/logging/utils/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/qs_logger.py
+Filename: cloudshell-logging-2.0.0/tests/logging/test_debug_logs/
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/utils/decorators.py
+Filename: cloudshell-logging-2.0.0/tests/logging/conftest.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/utils/error_handling_context_manager.py
+Filename: cloudshell-logging-2.0.0/tests/logging/test_memory_handler.py
 Comment: 
 
-Filename: cloudshell-logging-1.1.0/cloudshell/logging/utils/__init__.py
+Filename: cloudshell-logging-2.0.0/tests/logging/test_qs_config_parser.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/test_qs_logger.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/__init__.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/test_qs_config.ini
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/test_log_exec_info.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/test_getting_logger.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/package_file.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/__init__.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/utils/test_command_logging.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/utils/test_error_handling_context_manager.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/utils/__init__.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/test_debug_logs/package_file.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/test_debug_logs/__init__.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/tests/logging/test_debug_logs/test_debug_logs_on_error.py
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/top_level.txt
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/SOURCES.txt
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/PKG-INFO
+Comment: 
+
+Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-logging-1.1.0/setup.py` & `cloudshell-logging-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     required = f_required.read().splitlines()
 
 with open("test_requirements.txt") as f_tests:
     required_for_tests = f_tests.read().splitlines()
 
 setup(
     name="cloudshell-logging",
-    url="http://www.qualisystems.com/",
+    url="https://www.quali.com/",
     author="Quali",
     author_email="info@quali.com",
     packages=find_packages(),
     install_requires=required,
+    python_requires="~=3.7",
     tests_require=required_for_tests,
-    test_suite="nose.collector",
     version=version_from_file,
     description="QualiSystems Logger Package",
+    long_description="QualiSystems Logger Package",
     include_package_data=True,
 )
```

## Comparing `cloudshell-logging-1.1.0/README.md` & `cloudshell-logging-2.0.0/README.md`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-1.1.0/tox.ini` & `cloudshell-logging-2.0.0/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 # tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
-[DEFAULT]
-package-name = cloudshell.logging
-
 [tox]
 envlist =
-    py{27,37}-{master,dev}
+    py{37,39}-{master,dev}
     pre-commit
     build
 distshare = dist
 
 [testenv]
 skip_install:
     dev: true
 deps =
     master: -r test_requirements.txt
     dev: -r dev_requirements.txt
 commands =
-    nosetests --with-coverage --cover-package={[DEFAULT]package-name} tests
+    pytest --cov=cloudshell.logging tests --cov-report=xml
 
 [testenv:pre-commit]
-basepython = python3
 skip_install = true
 deps = pre-commit
 commands = pre-commit run --all-files --show-diff-on-failure
 
 [testenv:build]
 skip_install = true
-commands = python setup.py sdist --format zip
+commands =
+    python setup.py -q sdist --format zip
+    python setup.py -q bdist_wheel
 
 [isort]
-line_length = 88
-forced_separate = %(package-name)s,tests
-multi_line_output = 3
-include_trailing_comma = True
-combine_as_imports = 1
-skip = mibs
+profile=black
+forced_separate = cloudshell.logging,tests
 
 [flake8]
 max-line-length = 88
 ;we don't need have docstrings in every func, class and package
 ;and W503 is not PEP 8 compliant
 ignore = D100,D101,D102,D103,D104,D105,D107,D401,W503,E203
-exclude = mibs
```

## Comparing `cloudshell-logging-1.1.0/tests/logging/test_qs_logger.py` & `cloudshell-logging-2.0.0/tests/logging/test_qs_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,29 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
 """Tests for cloudshell.logging.qs_logger."""
 
 import logging
 import os
 import shutil
-import sys
+from logging import FileHandler
+from unittest import TestCase, mock
+from unittest.mock import MagicMock
 
 from cloudshell.logging import qs_logger
-from cloudshell.logging.interprocess_logger import MultiProcessingLog
-
-if sys.version_info >= (3, 0):
-    from unittest.mock import MagicMock
-    from unittest import TestCase, mock
-else:
-    from mock import MagicMock
-    import mock
-    from unittest import TestCase
-
+from cloudshell.logging.memory_handler import LimitedMemoryHandler
 
 CUR_DIR = os.path.dirname(__file__)
 full_settings = MagicMock(
     return_value={
         "LOG_PATH": "../../Logs",
         "TIME_FORMAT": "%d-%b-%Y--%H-%M-%S",
         "LOG_LEVEL": "ERROR",
         "LOG_PRIORITY": "ENV",
         "LOG_FORMAT": "%(asctime)s [%(levelname)s]: %(name)s %(module)s - "
         "%(funcName)-20s %(message)s",
+        "MEMORY_LOG_SIZE": 500,
     }
 )
 
 cut_settings = MagicMock(
     return_value={
         "TIME_FORMAT": "%d-%b-%Y--%H-%M-%S",
         "LOG_LEVEL": "ERROR",
@@ -74,18 +66,23 @@
         elif "QS_CONFIG" in os.environ:
             del os.environ["QS_CONFIG"]
 
         if self.log_path:
             os.putenv("LOG_PATH", self.log_path)
         elif "LOG_PATH" in os.environ:
             del os.environ["LOG_PATH"]
+        if "LOG_LEVEL" in os.environ:
+            del os.environ["LOG_LEVEL"]
 
         for logger in qs_logger._LOGGER_CONTAINER.values():
             for handler in logger.handlers:
                 handler.close()
+            logger.handlers.clear()
+
+        qs_logger._LOGGER_CONTAINER.clear()
 
         qs_logger.get_settings = self.get_settings
 
     @mock.patch.dict("cloudshell.logging.qs_logger.os.environ", {"LOG_LEVEL": "DEBUG"})
     def test_get_settings_priority_env_default_level(self):
         """Test suite for get_settings method.
 
@@ -96,14 +93,15 @@
             "UNIX_LOG_PATH": "/var/log/qualisystems",
             "DEFAULT_LOG_PATH": "../../Logs",
             "TIME_FORMAT": "%d-%b-%Y--%H-%M-%S",
             "LOG_LEVEL": qs_logger.DEFAULT_LEVEL,
             "LOG_PRIORITY": "ENV",
             "LOG_FORMAT": "%(asctime)s [%(levelname)s]: %(name)s %(module)s - "
             "%(funcName)-20s %(message)s",
+            "MEMORY_LOG_SIZE": 500,
         }
         names_to_remove = ["LOG_LEVEL"]
         modified_environ = {
             k: v for k, v in os.environ.items() if k not in names_to_remove
         }
         with mock.patch.dict(os.environ, modified_environ, clear=True):
             self.assertEqual(qs_logger.get_settings(), exp_response)
@@ -118,14 +116,15 @@
             "UNIX_LOG_PATH": "/var/log/qualisystems",
             "DEFAULT_LOG_PATH": "../../Logs",
             "TIME_FORMAT": "%d-%b-%Y--%H-%M-%S",
             "LOG_LEVEL": "DEBUG",
             "LOG_PRIORITY": "ENV",
             "LOG_FORMAT": "%(asctime)s [%(levelname)s]: %(name)s %(module)s - "
             "%(funcName)-20s %(message)s",
+            "MEMORY_LOG_SIZE": 500,
         }
         with mock.patch.dict(os.environ, {"LOG_LEVEL": "DEBUG"}):
             self.assertEqual(qs_logger.get_settings(), exp_response)
 
     @mock.patch("cloudshell.logging.qs_logger.QSConfigParser")
     def test_get_settings_default_log_level(self, parser_class):
         """Test suite for get_settings method.
@@ -136,14 +135,15 @@
         parser.get_config.return_value = {"LOG_PRIORITY": "WRONG_PRIORITY"}
 
         exp_response = {
             "TIME_FORMAT": qs_logger.DEFAULT_TIME_FORMAT,
             "LOG_LEVEL": qs_logger.DEFAULT_LEVEL,
             "LOG_PRIORITY": "WRONG_PRIORITY",
             "LOG_FORMAT": qs_logger.DEFAULT_FORMAT,
+            "MEMORY_LOG_SIZE": 500,
         }
 
         self.assertEqual(qs_logger.get_settings(), exp_response)
 
     @mock.patch("cloudshell.logging.qs_logger.QSConfigParser")
     def test_get_settings_log_level_from_config(self, parser_class):
         """Test suite for get_settings method.
@@ -157,14 +157,15 @@
         }
 
         exp_response = {
             "TIME_FORMAT": qs_logger.DEFAULT_TIME_FORMAT,
             "LOG_LEVEL": "CRITICAL",
             "LOG_PRIORITY": "CONFIG",
             "LOG_FORMAT": qs_logger.DEFAULT_FORMAT,
+            "MEMORY_LOG_SIZE": 500,
         }
 
         self.assertEqual(qs_logger.get_settings(), exp_response)
 
     @mock.patch("cloudshell.logging.qs_logger.os")
     def test_get_log_path_config_from_environment_variable(self, os):
         """Check that method will primarily return log path.
@@ -204,30 +205,30 @@
         result = qs_logger._get_log_path_config(config=config)
         # verify
         self.assertEqual(result, expected_path)
 
     def test_get_accessible_log_path_default_params(self):
         """Test suite for get_accessible_log_path method."""
         path = qs_logger.get_accessible_log_path()
-        self.assertRegexpMatches(
+        self.assertRegex(
             path,
             r"Logs[\\/]Autoload[\\/](.*[\\/])?default--\d{2}-\w+-"
             r"\d{4}--\d{2}-\d{2}-\d{2}\.log",
         )
         self.assertTrue(os.path.dirname(path))
 
     def test_get_accessible_log_path_path_creation(self):
         """Test suite for get_accessible_log_path method."""
         path = qs_logger.get_accessible_log_path()
         self.assertTrue(os.path.dirname(path))
 
     def test_get_accessible_log_path(self):
         """Test suite for get_accessible_log_path method."""
         path = qs_logger.get_accessible_log_path("reservation_id", "handler_name")
-        self.assertRegexpMatches(
+        self.assertRegex(
             path,
             r"Logs[\\/]reservation_id[\\/](.*[\\/])?"
             r"handler_name--\d{2}-\w+-\d{4}--\d{2}-\d{2}-\d{2}\.log",
         )
 
     def test_get_accessible_log_path_log_path_setting_missing(self):
         """Test suite for get_accessible_log_path method."""
@@ -242,39 +243,31 @@
             del os.environ["LOG_PATH"]
         qs_logger.get_settings = wrong_settings
         self.assertIsNone(qs_logger.get_accessible_log_path())
 
     def test_get_qs_logger_full_settings_default_params(self):
         """Test suite for get_qs_logger method."""
         qs_logger.get_settings = full_settings
-        self.assertTrue(
-            isinstance(qs_logger.get_qs_logger().handlers[0], MultiProcessingLog)
-        )
+        assert isinstance(qs_logger.get_qs_logger().handlers[0], FileHandler)
 
     def test_get_qs_logger_full_settings(self):
         """Test suite for get_qs_logger method."""
         qs_logger.get_settings = full_settings
-        self.assertTrue(
-            isinstance(
-                qs_logger.get_qs_logger(log_group="test1").handlers[0],
-                MultiProcessingLog,
-            )
-        )
+        assert isinstance(qs_logger.get_qs_logger("test1").handlers[0], FileHandler)
 
     def test_get_qs_logger_stream_handler(self):
         """Test suite for get_qs_logger method."""
         if "LOG_PATH" in os.environ:
             del os.environ["LOG_PATH"]
         qs_logger.get_settings = cut_settings
-        self.assertTrue(
-            isinstance(
-                qs_logger.get_qs_logger(log_group="stream").handlers[0],
-                logging.StreamHandler,
-            )
-        )
+
+        logger = qs_logger.get_qs_logger(log_group="stream")
+        # the logger has several handlers cause of previous tests
+        # but log records would be filtered by context
+        assert isinstance(logger.handlers[-1], logging.StreamHandler)
 
     def test_get_qs_logger_container_filling(self):
         """Test suite for get_qs_logger method."""
         qs_logger.get_settings = full_settings
         qs_logger.get_qs_logger()
         qs_logger.get_qs_logger(log_group="test1")
 
@@ -287,15 +280,20 @@
             sorted(qs_logger._LOGGER_CONTAINER.keys()),
             sorted(["Ungrouped", "test1", "test2"]),
         )
 
     def test_get_qs_logger_log_level_incorrect(self):
         os.environ["LOG_LEVEL"] = "INCORRECT"
         logger = qs_logger.get_qs_logger()
-        self.assertEqual(logger.level, getattr(logging, qs_logger.DEFAULT_LEVEL))
+        assert logger.level == logging.DEBUG
+        for hdrl in logger.handlers:
+            if isinstance(hdrl, LimitedMemoryHandler):
+                assert hdrl.level == logging.NOTSET
+            else:
+                assert hdrl.level == getattr(logging, qs_logger.DEFAULT_LEVEL)
 
     def test_normalize_buffer_decolorize(self):
         """Test suite for normalize_buffer method."""
         self.assertEqual(
             qs_logger.normalize_buffer(
                 "\033[1;32;40mGreenOnWhiteBack "
                 "\033[4;31mRedUnderscore "
```

## Comparing `cloudshell-logging-1.1.0/tests/logging/test_qs_config_parser.py` & `cloudshell-logging-2.0.0/tests/logging/test_qs_config_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
 """Tests for cloudshell.logging.qs_config_parser."""
 
 import os
 from unittest import TestCase
 
 from cloudshell.logging.qs_config_parser import QSConfigParser
```

## Comparing `cloudshell-logging-1.1.0/tests/logging/utils/test_error_handling_context_manager.py` & `cloudshell-logging-2.0.0/tests/logging/utils/test_error_handling_context_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-import sys
 from unittest import TestCase
+from unittest.mock import MagicMock, Mock
 
 from cloudshell.logging.utils.error_handling_context_manager import (
     ErrorHandlingContextManager,
 )
 
-if sys.version_info >= (3, 0):
-    from unittest.mock import MagicMock, Mock
-else:
-    from mock import MagicMock, Mock
-
 
 class TestErrorHandlingContextManager(TestCase):
     def test_log_written_when_exception_occurs(self):
         # Arrange
         logger = Mock()
         logger.error = MagicMock()
         try:
@@ -29,11 +24,11 @@
     def test_log_not_written_when_exception_not_thrown(self):
         # Arrange
         logger = Mock()
         logger.error = MagicMock()
 
         # Act
         with ErrorHandlingContextManager(logger=logger):
-            print("hello world")  # noqa: T001
+            print("hello world")  # noqa: T201
 
         # Assert
         logger.error.assert_not_called()
```

## Comparing `cloudshell-logging-1.1.0/cloudshell/logging/qs_config.ini` & `cloudshell-logging-2.0.0/cloudshell/logging/qs_config.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [Logging]
 ;Possible Log Levels: DEBUG, INFO, WARNING, ERROR, CRITICAL
 LOG_LEVEL='INFO'
 ;Possible Log Priorities: ENV, CONFIG
 ;ENV - get log level from environment variable specified in Execution Server customer.config
 ;CONFIG - get log level from current configuration file
 LOG_PRIORITY='ENV'
-LOG_FORMAT= '%(asctime)s [%(levelname)s]: %(name)s %(module)s - %(funcName)-20s %(message)s'
+LOG_FORMAT= '%(asctime)s [%(levelname)s]: %(threadName)s %(module)s - %(funcName)-20s %(message)s'
 TIME_FORMAT= '%d-%b-%Y--%H-%M-%S'
 WINDOWS_LOG_PATH='{ALLUSERSPROFILE}\QualiSystems\logs'
 UNIX_LOG_PATH='/var/log/qualisystems'
 DEFAULT_LOG_PATH='../../Logs'
+;Number of log records to keep in memory. On error log record they will be flushed to
+;separate file. File name is <log_file_name>-debug.log
+MEMORY_LOG_SIZE='500'
```

## Comparing `cloudshell-logging-1.1.0/cloudshell/logging/qs_config_parser.py` & `cloudshell-logging-2.0.0/cloudshell/logging/qs_config_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,20 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
+import configparser as ConfigParser
 import os
-import sys
 
 DEFAULT_CONFIG_PATH = "qs_config.ini"
 
-if sys.version_info >= (3, 0):
-    import configparser as ConfigParser
-else:
-    import ConfigParser
-
 
 class QSConfigParser:
     _configDict = None
 
     def __init__(self):
         self._config_parser = ConfigParser.RawConfigParser()
 
     def _get_full_config(self):
-        """  """
         config_file = os.getenv(
             "QS_CONFIG", os.path.join(os.path.dirname(__file__), DEFAULT_CONFIG_PATH)
         )
         config_dict = {}
         try:
             self._config_parser.read(config_file)
```

## Comparing `cloudshell-logging-1.1.0/cloudshell/logging/utils/error_handling_context_manager.py` & `cloudshell-logging-2.0.0/cloudshell/logging/utils/error_handling_context_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import traceback
 
 
-class ErrorHandlingContextManager(object):
+class ErrorHandlingContextManager:
     def __init__(self, logger):
         """Initializes an instance of ErrorHandlingContext.
 
         Allows proper logging on exception
         :param logger: Logger
         :type logger: Logger
         """
```

