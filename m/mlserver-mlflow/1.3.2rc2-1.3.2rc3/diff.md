# Comparing `tmp/mlserver-mlflow-1.3.2rc2.tar.gz` & `tmp/mlserver-mlflow-1.3.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-mlflow-1.3.2rc2.tar", last modified: Wed May  3 09:47:22 2023, max compression
+gzip compressed data, was "mlserver-mlflow-1.3.2rc3.tar", last modified: Thu May  4 08:48:09 2023, max compression
```

## Comparing `mlserver-mlflow-1.3.2rc2.tar` & `mlserver-mlflow-1.3.2rc3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:47:22.172504 mlserver-mlflow-1.3.2rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-03 09:46:39.000000 mlserver-mlflow-1.3.2rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-03 09:47:22.172504 mlserver-mlflow-1.3.2rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-03 09:46:39.000000 mlserver-mlflow-1.3.2rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:47:22.172504 mlserver-mlflow-1.3.2rc2/mlserver_mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 09:46:39.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-03 09:46:39.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-03 09:46:39.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-03 09:46:39.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-03 09:46:39.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:47:22.172504 mlserver-mlflow-1.3.2rc2/mlserver_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-03 09:47:21.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-03 09:47:22.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:47:21.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 09:47:21.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 09:47:21.000000 mlserver-mlflow-1.3.2rc2/mlserver_mlflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 09:47:22.172504 mlserver-mlflow-1.3.2rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-03 09:46:39.000000 mlserver-mlflow-1.3.2rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:48:09.983187 mlserver-mlflow-1.3.2rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 08:47:20.000000 mlserver-mlflow-1.3.2rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-04 08:48:09.983187 mlserver-mlflow-1.3.2rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-04 08:47:20.000000 mlserver-mlflow-1.3.2rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:48:09.983187 mlserver-mlflow-1.3.2rc3/mlserver_mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-04 08:47:20.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-04 08:47:20.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-04 08:47:20.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-04 08:47:20.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 08:47:20.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:48:09.983187 mlserver-mlflow-1.3.2rc3/mlserver_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-04 08:48:09.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-04 08:48:09.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:48:09.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 08:48:09.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 08:48:09.000000 mlserver-mlflow-1.3.2rc3/mlserver_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:48:09.983187 mlserver-mlflow-1.3.2rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 08:47:20.000000 mlserver-mlflow-1.3.2rc3/setup.py
```

### Comparing `mlserver-mlflow-1.3.2rc2/LICENSE` & `mlserver-mlflow-1.3.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.3.2rc2/PKG-INFO` & `mlserver-mlflow-1.3.2rc3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-mlflow
-Version: 1.3.2rc2
+Version: 1.3.2rc3
 Summary: MLflow runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLflow runtime for MLServer
```

### Comparing `mlserver-mlflow-1.3.2rc2/README.md` & `mlserver-mlflow-1.3.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.3.2rc2/mlserver_mlflow/codecs.py` & `mlserver-mlflow-1.3.2rc3/mlserver_mlflow/codecs.py`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.3.2rc2/mlserver_mlflow/metadata.py` & `mlserver-mlflow-1.3.2rc3/mlserver_mlflow/metadata.py`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.3.2rc2/mlserver_mlflow/runtime.py` & `mlserver-mlflow-1.3.2rc3/mlserver_mlflow/runtime.py`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.3.2rc2/mlserver_mlflow.egg-info/PKG-INFO` & `mlserver-mlflow-1.3.2rc3/mlserver_mlflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-mlflow
-Version: 1.3.2rc2
+Version: 1.3.2rc3
 Summary: MLflow runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLflow runtime for MLServer
```

### Comparing `mlserver-mlflow-1.3.2rc2/setup.py` & `mlserver-mlflow-1.3.2rc3/setup.py`

 * *Files identical despite different names*

