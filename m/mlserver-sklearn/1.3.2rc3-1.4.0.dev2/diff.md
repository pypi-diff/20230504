# Comparing `tmp/mlserver-sklearn-1.3.2rc3.tar.gz` & `tmp/mlserver-sklearn-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-sklearn-1.3.2rc3.tar", last modified: Thu May  4 08:48:10 2023, max compression
+gzip compressed data, was "mlserver-sklearn-1.4.0.dev2.tar", last modified: Thu May  4 09:30:47 2023, max compression
```

## Comparing `mlserver-sklearn-1.3.2rc3.tar` & `mlserver-sklearn-1.4.0.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:48:10.315810 mlserver-sklearn-1.3.2rc3/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 08:47:24.000000 mlserver-sklearn-1.3.2rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-04 08:48:10.315810 mlserver-sklearn-1.3.2rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 08:47:24.000000 mlserver-sklearn-1.3.2rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:48:10.315810 mlserver-sklearn-1.3.2rc3/mlserver_sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 08:47:24.000000 mlserver-sklearn-1.3.2rc3/mlserver_sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-04 08:47:24.000000 mlserver-sklearn-1.3.2rc3/mlserver_sklearn/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 08:47:24.000000 mlserver-sklearn-1.3.2rc3/mlserver_sklearn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:48:10.315810 mlserver-sklearn-1.3.2rc3/mlserver_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-04 08:48:10.000000 mlserver-sklearn-1.3.2rc3/mlserver_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 08:48:10.000000 mlserver-sklearn-1.3.2rc3/mlserver_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:48:10.000000 mlserver-sklearn-1.3.2rc3/mlserver_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 08:48:10.000000 mlserver-sklearn-1.3.2rc3/mlserver_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 08:48:10.000000 mlserver-sklearn-1.3.2rc3/mlserver_sklearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:48:10.315810 mlserver-sklearn-1.3.2rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-04 08:47:24.000000 mlserver-sklearn-1.3.2rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 09:30:47.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:47.094384 mlserver-sklearn-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/setup.py
```

### Comparing `mlserver-sklearn-1.3.2rc3/LICENSE` & `mlserver-sklearn-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-sklearn-1.3.2rc3/PKG-INFO` & `mlserver-sklearn-1.4.0.dev2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-sklearn
-Version: 1.3.2rc3
+Version: 1.4.0.dev2
 Summary: Scikit-Learn runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Scikit-Learn runtime for MLServer
```

### Comparing `mlserver-sklearn-1.3.2rc3/README.md` & `mlserver-sklearn-1.4.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-sklearn-1.3.2rc3/mlserver_sklearn/sklearn.py` & `mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/sklearn.py`

 * *Files identical despite different names*

### Comparing `mlserver-sklearn-1.3.2rc3/mlserver_sklearn.egg-info/PKG-INFO` & `mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-sklearn
-Version: 1.3.2rc3
+Version: 1.4.0.dev2
 Summary: Scikit-Learn runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Scikit-Learn runtime for MLServer
```

### Comparing `mlserver-sklearn-1.3.2rc3/setup.py` & `mlserver-sklearn-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

