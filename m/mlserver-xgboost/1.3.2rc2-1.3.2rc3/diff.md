# Comparing `tmp/mlserver-xgboost-1.3.2rc2.tar.gz` & `tmp/mlserver-xgboost-1.3.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-xgboost-1.3.2rc2.tar", last modified: Wed May  3 09:47:27 2023, max compression
+gzip compressed data, was "mlserver-xgboost-1.3.2rc3.tar", last modified: Thu May  4 08:48:03 2023, max compression
```

## Comparing `mlserver-xgboost-1.3.2rc2.tar` & `mlserver-xgboost-1.3.2rc3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:47:27.012672 mlserver-xgboost-1.3.2rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-03 09:46:48.000000 mlserver-xgboost-1.3.2rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-03 09:47:27.012672 mlserver-xgboost-1.3.2rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-03 09:46:48.000000 mlserver-xgboost-1.3.2rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:47:27.012672 mlserver-xgboost-1.3.2rc2/mlserver_xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 09:46:48.000000 mlserver-xgboost-1.3.2rc2/mlserver_xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-03 09:46:48.000000 mlserver-xgboost-1.3.2rc2/mlserver_xgboost/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-03 09:46:48.000000 mlserver-xgboost-1.3.2rc2/mlserver_xgboost/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:47:27.012672 mlserver-xgboost-1.3.2rc2/mlserver_xgboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-03 09:47:26.000000 mlserver-xgboost-1.3.2rc2/mlserver_xgboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-03 09:47:26.000000 mlserver-xgboost-1.3.2rc2/mlserver_xgboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:47:26.000000 mlserver-xgboost-1.3.2rc2/mlserver_xgboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-03 09:47:26.000000 mlserver-xgboost-1.3.2rc2/mlserver_xgboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 09:47:26.000000 mlserver-xgboost-1.3.2rc2/mlserver_xgboost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 09:47:27.012672 mlserver-xgboost-1.3.2rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-03 09:46:48.000000 mlserver-xgboost-1.3.2rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:48:03.712250 mlserver-xgboost-1.3.2rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 08:47:23.000000 mlserver-xgboost-1.3.2rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-04 08:48:03.712250 mlserver-xgboost-1.3.2rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 08:47:23.000000 mlserver-xgboost-1.3.2rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:48:03.712250 mlserver-xgboost-1.3.2rc3/mlserver_xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 08:47:23.000000 mlserver-xgboost-1.3.2rc3/mlserver_xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 08:47:23.000000 mlserver-xgboost-1.3.2rc3/mlserver_xgboost/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-04 08:47:23.000000 mlserver-xgboost-1.3.2rc3/mlserver_xgboost/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:48:03.712250 mlserver-xgboost-1.3.2rc3/mlserver_xgboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-04 08:48:03.000000 mlserver-xgboost-1.3.2rc3/mlserver_xgboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 08:48:03.000000 mlserver-xgboost-1.3.2rc3/mlserver_xgboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:48:03.000000 mlserver-xgboost-1.3.2rc3/mlserver_xgboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 08:48:03.000000 mlserver-xgboost-1.3.2rc3/mlserver_xgboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 08:48:03.000000 mlserver-xgboost-1.3.2rc3/mlserver_xgboost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:48:03.712250 mlserver-xgboost-1.3.2rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-04 08:47:23.000000 mlserver-xgboost-1.3.2rc3/setup.py
```

### Comparing `mlserver-xgboost-1.3.2rc2/LICENSE` & `mlserver-xgboost-1.3.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-xgboost-1.3.2rc2/PKG-INFO` & `mlserver-xgboost-1.3.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-xgboost
-Version: 1.3.2rc2
+Version: 1.3.2rc3
 Summary: XGBoost runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # XGBoost runtime for MLServer
```

### Comparing `mlserver-xgboost-1.3.2rc2/README.md` & `mlserver-xgboost-1.3.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-xgboost-1.3.2rc2/mlserver_xgboost/xgboost.py` & `mlserver-xgboost-1.3.2rc3/mlserver_xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `mlserver-xgboost-1.3.2rc2/mlserver_xgboost.egg-info/PKG-INFO` & `mlserver-xgboost-1.3.2rc3/mlserver_xgboost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-xgboost
-Version: 1.3.2rc2
+Version: 1.3.2rc3
 Summary: XGBoost runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # XGBoost runtime for MLServer
```

### Comparing `mlserver-xgboost-1.3.2rc2/setup.py` & `mlserver-xgboost-1.3.2rc3/setup.py`

 * *Files identical despite different names*

