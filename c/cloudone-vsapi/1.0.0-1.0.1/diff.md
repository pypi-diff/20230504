# Comparing `tmp/cloudone-vsapi-1.0.0.tar.gz` & `tmp/cloudone-vsapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudone-vsapi-1.0.0.tar", last modified: Mon May  1 23:49:45 2023, max compression
+gzip compressed data, was "cloudone-vsapi-1.0.1.tar", last modified: Thu May  4 18:54:01 2023, max compression
```

## Comparing `cloudone-vsapi-1.0.0.tar` & `cloudone-vsapi-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-01 23:48:09.000000 cloudone-vsapi-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-01 23:48:09.000000 cloudone-vsapi-1.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-01 23:48:09.000000 cloudone-vsapi-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/amaas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:48:09.000000 cloudone-vsapi-1.0.0/amaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 23:48:09.000000 cloudone-vsapi-1.0.0/amaas/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/amaas/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-01 23:48:09.000000 cloudone-vsapi-1.0.0/amaas/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/amaas/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-01 23:48:09.000000 cloudone-vsapi-1.0.0/amaas/grpc/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/amaas/grpc/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-01 23:48:09.000000 cloudone-vsapi-1.0.0/amaas/grpc/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/amaas/grpc/protos/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-01 23:49:43.000000 cloudone-vsapi-1.0.0/amaas/grpc/protos/scan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-01 23:49:43.000000 cloudone-vsapi-1.0.0/amaas/grpc/protos/scan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-01 23:49:43.000000 cloudone-vsapi-1.0.0/amaas/grpc/protos/scan_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/cloudone_vsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-01 23:49:45.000000 cloudone-vsapi-1.0.0/cloudone_vsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-01 23:49:45.000000 cloudone-vsapi-1.0.0/cloudone_vsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:49:45.000000 cloudone-vsapi-1.0.0/cloudone_vsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-01 23:49:45.000000 cloudone-vsapi-1.0.0/cloudone_vsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 23:49:45.000000 cloudone-vsapi-1.0.0/cloudone_vsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-01 23:49:44.000000 cloudone-vsapi-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:49:45.878648 cloudone-vsapi-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-01 23:48:09.000000 cloudone-vsapi-1.0.0/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/grpc/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/grpc/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/amaas/grpc/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/amaas/grpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-04 18:53:58.000000 cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-04 18:53:58.000000 cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-04 18:53:58.000000 cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 18:54:01.000000 cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-04 18:54:01.413081 cloudone-vsapi-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-04 18:54:00.000000 cloudone-vsapi-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:54:01.409081 cloudone-vsapi-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-04 18:52:06.000000 cloudone-vsapi-1.0.1/tests/test_simple.py
```

### Comparing `cloudone-vsapi-1.0.0/LICENSE` & `cloudone-vsapi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.0/PKG-INFO` & `cloudone-vsapi-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudone-vsapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Trend Micro Cloud One VSAPI SDK for python
 Home-page: https://github.com/trendmicro/cloudone-antimalware-python-sdk
 Author: Trend Micro Cloud One Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudone-vsapi-1.0.0/README.md` & `cloudone-vsapi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.0/amaas/grpc/protos/scan_pb2.py` & `cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.0/amaas/grpc/protos/scan_pb2.pyi` & `cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.0/amaas/grpc/protos/scan_pb2_grpc.py` & `cloudone-vsapi-1.0.1/amaas/grpc/protos/scan_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.0/cloudone_vsapi.egg-info/PKG-INFO` & `cloudone-vsapi-1.0.1/cloudone_vsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudone-vsapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Trend Micro Cloud One VSAPI SDK for python
 Home-page: https://github.com/trendmicro/cloudone-antimalware-python-sdk
 Author: Trend Micro Cloud One Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudone-vsapi-1.0.0/setup.py` & `cloudone-vsapi-1.0.1/setup.py`

 * *Files identical despite different names*

