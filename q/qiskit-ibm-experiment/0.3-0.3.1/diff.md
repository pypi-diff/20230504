# Comparing `tmp/qiskit-ibm-experiment-0.3.tar.gz` & `tmp/qiskit-ibm-experiment-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-experiment-0.3.tar", last modified: Sun Mar 19 08:47:15 2023, max compression
+gzip compressed data, was "qiskit-ibm-experiment-0.3.1.tar", last modified: Thu May  4 14:15:03 2023, max compression
```

## Comparing `qiskit-ibm-experiment-0.3.tar` & `qiskit-ibm-experiment-0.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:47:15.661365 qiskit-ibm-experiment-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-03-19 08:47:15.661365 qiskit-ibm-experiment-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:47:15.657365 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:47:15.657365 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:47:15.661365 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/experiment_rest_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:47:15.661365 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/device_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/experiment_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    68841 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/ibm_experiment_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:47:15.657365 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-03-19 08:47:15.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-19 08:47:15.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 08:47:15.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 08:47:15.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-19 08:47:15.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-19 08:47:15.000000 qiskit-ibm-experiment-0.3/qiskit_ibm_experiment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 08:47:15.661365 qiskit-ibm-experiment-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:47:15.661365 qiskit-ibm-experiment-0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:47:15.661365 qiskit-ibm-experiment-0.3/test/service/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/service/ibm_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/service/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/service/test_experiment_data_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    66547 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/service/test_experiment_server_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/service/test_local_experiment_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 08:47:15.661365 qiskit-ibm-experiment-0.3/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/utils/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-19 08:47:07.000000 qiskit-ibm-experiment-0.3/test/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.155968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.155968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.155968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/experiment_rest_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/device_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/experiment_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68992 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/ibm_experiment_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.155968 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 14:15:03.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 14:15:02.000000 qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/test/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/ibm_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/test_experiment_data_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66547 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/test_experiment_server_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/service/test_local_experiment_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:03.159968 qiskit-ibm-experiment-0.3.1/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/utils/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 14:14:55.000000 qiskit-ibm-experiment-0.3.1/test/utils/utils.py
```

### Comparing `qiskit-ibm-experiment-0.3/LICENSE.txt` & `qiskit-ibm-experiment-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/PKG-INFO` & `qiskit-ibm-experiment-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-experiment
-Version: 0.3
+Version: 0.3.1
 Summary: Qiskit IBM Experiment service for accessing the quantum experiment interface at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-experiment
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-experiment/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-experiment-0.3/README.md` & `qiskit-ibm-experiment-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/__init__.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/__init__.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/account.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/configuration.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/exceptions.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/management.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/accounts/storage.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/__init__.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/experiment.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/experiment_rest_adapter.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/experiment_rest_adapter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/local_client.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/local_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/client/session.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/client/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/exceptions.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/__init__.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/constants.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/device_component.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/device_component.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/experiment_dataclasses.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/experiment_dataclasses.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/ibm_experiment_service.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/ibm_experiment_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,28 +287,31 @@
         return self._api_client.devices()
 
     def create_experiment(
         self,
         data: ExperimentData,
         provider: Optional[Any] = None,
         json_encoder: Type[json.JSONEncoder] = json.JSONEncoder,
-    ) -> str:
+    ) -> dict:
         """Create a new experiment in the database.
 
         Args:
             data: The dataclass containing the experiment's data
             provider: The provider used when running the experiment
             json_encoder: Custom JSON encoder to use to encode the experiment.
 
         Returns:
             Experiment ID.
 
         Raises:
             IBMExperimentEntryExists: If the experiment already exits.
             IBMApiError: If the request to the server failed.
+
+        Returns:
+            The upload response data
         """
         if self.hgp is not None:
             try:
                 data.hub, data.group, data.project = self.hgp.split("/")
             except RuntimeError:
                 pass
 
@@ -335,30 +338,32 @@
                 "(passing a provider parameter enables inference of these values)"
             )
 
         with map_api_error(f"Experiment {data.experiment_id} creation failed."):
             response_data = self._api_client.experiment_upload(
                 json.dumps(api_data, cls=json_encoder)
             )
-        return response_data["uuid"]
+        return response_data
 
     def update_experiment(
         self,
         data: ExperimentData,
         json_encoder: Type[json.JSONEncoder] = json.JSONEncoder,
-    ) -> None:
+    ) -> dict:
         """Update an existing experiment.
 
         Args:
             data: The dataclass containing the experiment's data
             json_encoder: Custom JSON encoder to use to encode the experiment.
 
         Raises:
             IBMExperimentEntryNotFound: If the experiment does not exist.
             IBMApiError: If the request to the server failed.
+        Returns:
+            The update response data
         """
 
         api_data = self._experiment_data_to_api(data)
         unused_fields = [
             "uuid",
             "device_name",
             "group_id",
@@ -372,17 +377,18 @@
                 del api_data[field_name]
 
         if not data:
             logger.warning("update_experiment() called with nothing to update.")
             return
 
         with map_api_error(f"Experiment {data.experiment_id} update failed."):
-            self._api_client.experiment_update(
+            response_data = self._api_client.experiment_update(
                 data.experiment_id, json.dumps(api_data, cls=json_encoder)
             )
+            return response_data
 
     def create_or_update_experiment(
         self,
         data: ExperimentData,
         json_encoder: Type[json.JSONEncoder] = json.JSONEncoder,
         create: bool = True,
         max_attempts: int = 3,
```

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/service/utils.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/service/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment/version.py` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment.egg-info/PKG-INFO` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-experiment
-Version: 0.3
+Version: 0.3.1
 Summary: Qiskit IBM Experiment service for accessing the quantum experiment interface at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-experiment
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-experiment/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-experiment-0.3/qiskit_ibm_experiment.egg-info/SOURCES.txt` & `qiskit-ibm-experiment-0.3.1/qiskit_ibm_experiment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/setup.py` & `qiskit-ibm-experiment-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/test/__init__.py` & `qiskit-ibm-experiment-0.3.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/test/service/ibm_test_case.py` & `qiskit-ibm-experiment-0.3.1/test/service/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/test/service/test_experiment.py` & `qiskit-ibm-experiment-0.3.1/test/service/test_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/test/service/test_experiment_data_integration.py` & `qiskit-ibm-experiment-0.3.1/test/service/test_experiment_data_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/test/service/test_experiment_server_integration.py` & `qiskit-ibm-experiment-0.3.1/test/service/test_experiment_server_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/test/service/test_local_experiment_client.py` & `qiskit-ibm-experiment-0.3.1/test/service/test_local_experiment_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/test/utils/program.py` & `qiskit-ibm-experiment-0.3.1/test/utils/program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/test/utils/templates.py` & `qiskit-ibm-experiment-0.3.1/test/utils/templates.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3/test/utils/utils.py` & `qiskit-ibm-experiment-0.3.1/test/utils/utils.py`

 * *Files identical despite different names*

