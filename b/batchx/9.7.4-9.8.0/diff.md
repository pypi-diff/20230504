# Comparing `tmp/batchx-9.7.4.tar.gz` & `tmp/batchx-9.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchx-9.7.4.tar", last modified: Wed Apr 26 20:00:27 2023, max compression
+gzip compressed data, was "batchx-9.8.0.tar", last modified: Thu May  4 09:15:28 2023, max compression
```

## Comparing `batchx-9.7.4.tar` & `batchx-9.8.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:00:27.618768 batchx-9.7.4/
--rw-rw-rw-   0 root         (0) root         (0)        9 2020-04-16 12:00:00.000000 batchx-9.7.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 20:00:27.618768 batchx-9.7.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      740 2020-04-16 12:00:00.000000 batchx-9.7.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 batchx-9.7.4/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:00:27.614767 batchx-9.7.4/batchx/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 20:00:26.000000 batchx-9.7.4/batchx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6896 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/admin_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13599 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/admin_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5445 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/alert_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5601 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/alert_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6011 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/audit_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2459 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/audit_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7926 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/auth_pb2.py
--rw-r--r--   0 root         (0) root         (0)    18170 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/auth_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/billing_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/billing_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    48012 2023-04-26 20:00:26.000000 batchx-9.7.4/batchx/bx.py
--rw-r--r--   0 root         (0) root         (0)     5608 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/common_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/common_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3160 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/consumer_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/consumer_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/docker_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/docker_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4563 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/environment_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5829 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/environment_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    26120 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/filesystem_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28037 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/filesystem_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/health_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3893 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/health_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    26939 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/image_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22798 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/image_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    26615 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24930 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/log_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/log_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8460 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/organization_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16168 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/organization_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5606 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/picture_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7154 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/picture_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/profile_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/profile_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8419 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/provider_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7420 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/provider_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6509 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/tag_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9944 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/tag_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/token_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/token_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3911 2023-04-26 20:00:25.000000 batchx-9.7.4/batchx/user_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:00:27.618768 batchx-9.7.4/batchx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1011 2023-04-26 20:00:27.000000 batchx-9.7.4/batchx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1226 2023-04-26 20:00:27.000000 batchx-9.7.4/batchx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 20:00:27.000000 batchx-9.7.4/batchx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-26 20:00:27.000000 batchx-9.7.4/batchx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-26 20:00:27.000000 batchx-9.7.4/batchx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 20:00:27.618768 batchx-9.7.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 batchx-9.7.4/setup.py
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-26 20:00:26.000000 batchx-9.7.4/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:28.071695 batchx-9.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2020-04-16 12:00:00.000000 batchx-9.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-05-04 09:15:28.071695 batchx-9.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      740 2020-04-16 12:00:00.000000 batchx-9.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 batchx-9.8.0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:28.059695 batchx-9.8.0/batchx/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6896 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/admin_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13599 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/admin_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5445 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/alert_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5601 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/alert_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6011 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/audit_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/audit_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7926 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/auth_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    18170 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/auth_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/billing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/billing_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    48511 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/bx.py
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/common_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/common_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3160 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/consumer_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/consumer_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/docker_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/docker_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4563 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/environment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/environment_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    27864 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/filesystem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    29710 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/filesystem_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/health_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3893 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/health_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    26939 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/image_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22798 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/image_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    26615 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24930 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/log_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/log_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8460 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/organization_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16168 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/organization_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5606 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/picture_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7154 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/picture_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/profile_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/profile_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8419 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/provider_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/provider_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6509 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/tag_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/tag_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/token_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/token_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-05-04 09:15:26.000000 batchx-9.8.0/batchx/user_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 09:15:28.067695 batchx-9.8.0/batchx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-05-04 09:15:27.000000 batchx-9.8.0/batchx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-05-04 09:15:27.000000 batchx-9.8.0/batchx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 09:15:27.000000 batchx-9.8.0/batchx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-04 09:15:27.000000 batchx-9.8.0/batchx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 09:15:27.000000 batchx-9.8.0/batchx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 09:15:28.071695 batchx-9.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 batchx-9.8.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-04 09:15:26.000000 batchx-9.8.0/version
```

### Comparing `batchx-9.7.4/PKG-INFO` & `batchx-9.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchx
-Version: 9.7.4
+Version: 9.8.0
 Summary: Batchx Python API
 Home-page: https://github.com/batchx/api
 Author: Batchx
 Author-email: dev@batchx.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `batchx-9.7.4/README.md` & `batchx-9.8.0/README.md`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/admin_pb2.py` & `batchx-9.8.0/batchx/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/admin_pb2_grpc.py` & `batchx-9.8.0/batchx/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/alert_pb2.py` & `batchx-9.8.0/batchx/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/alert_pb2_grpc.py` & `batchx-9.8.0/batchx/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/audit_pb2.py` & `batchx-9.8.0/batchx/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/audit_pb2_grpc.py` & `batchx-9.8.0/batchx/audit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/auth_pb2.py` & `batchx-9.8.0/batchx/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/auth_pb2_grpc.py` & `batchx-9.8.0/batchx/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/billing_pb2.py` & `batchx-9.8.0/batchx/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/billing_pb2_grpc.py` & `batchx-9.8.0/batchx/billing_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/bx.py` & `batchx-9.8.0/batchx/bx.py`

 * *Files 2% similar despite different names*

```diff
@@ -603,14 +603,18 @@
         check()
         return make_call(filesystem_pb2_grpc.FilesystemServiceStub(channel).ListBlobs, request)
 
     def ListFolder(self, request):
         check()
         return make_call(filesystem_pb2_grpc.FilesystemServiceStub(channel).ListFolder, request)
 
+    def ListS3BucketFolder(self, request):
+        check()
+        return make_call(filesystem_pb2_grpc.FilesystemServiceStub(channel).ListS3BucketFolder, request)
+
     def ListS3Buckets(self, request):
         check()
         return make_call(filesystem_pb2_grpc.FilesystemServiceStub(channel).ListS3Buckets, request)
 
     def RemoveS3Bucket(self, request):
         check()
         return make_call(filesystem_pb2_grpc.FilesystemServiceStub(channel).RemoveS3Bucket, request)
@@ -708,14 +712,20 @@
 
     def ListFolderRequest(self, **kwargs):
         return filesystem_pb2.ListFolderRequest(**kwargs)
 
     def ListFolderResponse(self, **kwargs):
         return filesystem_pb2.ListFolderResponse(**kwargs)
 
+    def ListS3BucketFolderRequest(self, **kwargs):
+        return filesystem_pb2.ListS3BucketFolderRequest(**kwargs)
+
+    def ListS3BucketFolderResponse(self, **kwargs):
+        return filesystem_pb2.ListS3BucketFolderResponse(**kwargs)
+
     def ListS3BucketsRequest(self, **kwargs):
         return filesystem_pb2.ListS3BucketsRequest(**kwargs)
 
     def ListS3BucketsResponse(self, **kwargs):
         return filesystem_pb2.ListS3BucketsResponse(**kwargs)
 
     def Metadata(self, **kwargs):
@@ -729,14 +739,17 @@
 
     def ReportUploadStatusRequest(self, **kwargs):
         return filesystem_pb2.ReportUploadStatusRequest(**kwargs)
 
     def ReportUploadStatusResponse(self, **kwargs):
         return filesystem_pb2.ReportUploadStatusResponse(**kwargs)
 
+    def S3BucketObject(self, **kwargs):
+        return filesystem_pb2.S3BucketObject(**kwargs)
+
     def SetBlobStatusRequest(self, **kwargs):
         return filesystem_pb2.SetBlobStatusRequest(**kwargs)
 
     def SetBlobStatusResponse(self, **kwargs):
         return filesystem_pb2.SetBlobStatusResponse(**kwargs)
 
     def ShareFileRequest(self, **kwargs):
```

### Comparing `batchx-9.7.4/batchx/common_pb2.py` & `batchx-9.8.0/batchx/common_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/consumer_pb2.py` & `batchx-9.8.0/batchx/consumer_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/consumer_pb2_grpc.py` & `batchx-9.8.0/batchx/consumer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/docker_pb2.py` & `batchx-9.8.0/batchx/docker_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/environment_pb2.py` & `batchx-9.8.0/batchx/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/environment_pb2_grpc.py` & `batchx-9.8.0/batchx/environment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/filesystem_pb2.py` & `batchx-9.8.0/batchx/filesystem_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from . import log_pb2 as log__pb2
 from . import tag_pb2 as tag__pb2
 from . import common_pb2 as common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x66ilesystem.proto\x12\x11\x62\x61tchx.filesystem\x1a\tlog.proto\x1a\ttag.proto\x1a\x0c\x63ommon.proto\"\xd9\x01\n\x12\x41\x64\x64S3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\x12\x46\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x31.batchx.filesystem.AddS3BucketRequest.Credentials\x1aQ\n\x0b\x43redentials\x12\x13\n\x0b\x61\x63\x63\x65ssKeyId\x18\x01 \x01(\t\x12\x17\n\x0fsecretAccessKey\x18\x02 \x01(\t\x12\x14\n\x0csessionToken\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64S3BucketResponse\"+\n\x14ListS3BucketsRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\"\xbe\x02\n\x15ListS3BucketsResponse\x12?\n\x06\x62ucket\x18\x01 \x03(\x0b\x32/.batchx.filesystem.ListS3BucketsResponse.Bucket\x12@\n\x04user\x18\x02 \x03(\x0b\x32\x32.batchx.filesystem.ListS3BucketsResponse.UserEntry\x1a`\n\x06\x42ucket\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x13\n\x0bts_creation\x18\x04 \x01(\x03\x12\x0e\n\x06public\x18\x05 \x01(\x08\x1a@\n\tUserEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"A\n\x15RemoveS3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\"\x18\n\x16RemoveS3BucketResponse\"\xa9\x01\n\x10ShareFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.batchx.filesystem.ShareFileRequest.Type\"\x1e\n\x04Type\x12\t\n\x05SHARE\x10\x00\x12\x0b\n\x07UNSHARE\x10\x01\"\x13\n\x11ShareFileResponse\"j\n\x14SetBlobStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12-\n\x06status\x18\x03 \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\x17\n\x15SetBlobStatusResponse\"\xad\x05\n\x17ListBlobPointersRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12I\n\npagination\x18\x03 \x01(\x0b\x32\x35.batchx.filesystem.ListBlobPointersRequest.Pagination\x12G\n\tfiltering\x18\x04 \x01(\x0b\x32\x34.batchx.filesystem.ListBlobPointersRequest.Filtering\x12?\n\x05order\x18\x05 \x01(\x0b\x32\x30.batchx.filesystem.ListBlobPointersRequest.Order\x1a\xa3\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12N\n\x07memento\x18\x02 \x01(\x0b\x32=.batchx.filesystem.ListBlobPointersRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1aO\n\tFiltering\x12\r\n\x05owner\x18\x01 \x03(\t\x12\x33\n\x0bts_creation\x18\x02 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x1a\xa0\x01\n\x05Order\x12J\n\x08order_by\x18\x01 \x01(\x0e\x32\x38.batchx.filesystem.ListBlobPointersRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"\'\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bTS_CREATION\x10\x01\"\x8d\x02\n\x18ListBlobPointersResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12G\n\x06owners\x18\x03 \x03(\x0b\x32\x37.batchx.filesystem.ListBlobPointersResponse.OwnersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"\xf4\x06\n\x10ListBlobsRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x38\n\x05order\x18\x02 \x01(\x0b\x32).batchx.filesystem.ListBlobsRequest.Order\x12\x42\n\npagination\x18\x03 \x01(\x0b\x32..batchx.filesystem.ListBlobsRequest.Pagination\x12@\n\tfiltering\x18\x04 \x01(\x0b\x32-.batchx.filesystem.ListBlobsRequest.Filtering\x1a\xc9\x01\n\x05Order\x12\x43\n\x08order_by\x18\x01 \x01(\x0e\x32\x31.batchx.filesystem.ListBlobsRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"W\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08POINTERS\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x1a\x9e\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12G\n\x07memento\x18\x02 \x01(\x0b\x32\x36.batchx.filesystem.ListBlobsRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x19\n\x07Memento\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x1a\x9d\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12/\n\x08pointers\x18\x02 \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12.\n\x06length\x18\x03 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x33\n\x0bts_creation\x18\x04 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x05 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x32\n\x0b\x62lob_status\x18\x06 \x03(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\xfc\x01\n\x11ListBlobsResponse\x12%\n\x04\x62lob\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.Blob\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12>\n\x05users\x18\x03 \x03(\x0b\x32/.batchx.filesystem.ListBlobsResponse.UsersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"5\n\x0eGetBlobRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\"8\n\x0fGetBlobResponse\x12%\n\x04\x62lob\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.Blob\"\x83\x03\n\x04\x42lob\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12\x10\n\x08pointers\x18\x03 \x01(\x05\x12\x0e\n\x06length\x18\x04 \x01(\x03\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\x0c\n\x04user\x18\x07 \x01(\t\x12\x15\n\roriginal_path\x18\x08 \x01(\t\x12-\n\x06status\x18\t \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x16\n\x0ets_archivation\x18\n \x01(\x03\x12\x33\n\tmeta_info\x18\x0b \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a\x64\n\x08MetaInfo\x12\x0e\n\x06\x62inary\x18\x01 \x01(\x08\x12\x0c\n\x04gzip\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x63ompressed_size\x18\x03 \x01(\x03\x12\x12\n\nline_count\x18\x04 \x01(\x03\x12\x0b\n\x03new\x18\x05 \x01(\x08\"\x9a\x08\n\x11ListFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x11\n\trecursive\x18\x03 \x01(\x08\x12\x41\n\tfiltering\x18\x04 \x01(\x0b\x32..batchx.filesystem.ListFolderRequest.Filtering\x12\x43\n\npagination\x18\x05 \x01(\x0b\x32/.batchx.filesystem.ListFolderRequest.Pagination\x12\x39\n\x05order\x18\x06 \x01(\x0b\x32*.batchx.filesystem.ListFolderRequest.Order\x12\x18\n\x10user_environment\x18\x07 \x01(\t\x1a\xfa\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12\x12\n\nonly_ready\x18\x02 \x01(\x08\x12\x17\n\rexclude_files\x18\x03 \x01(\x08H\x00\x12\x19\n\x0f\x65xclude_folders\x18\x04 \x01(\x08H\x00\x12\'\n\x03tag\x18\x05 \x03(\x0b\x32\x1a.batchx.tag.TagCoordinates\x12\x33\n\x0bts_creation\x18\x06 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x07 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12.\n\x06length\x18\x08 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12/\n\x08pointers\x18\t \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12\x16\n\x0e\x66ilename_token\x18\n \x01(\tB\x06\n\x04Type\x1a\x9d\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12H\n\x07memento\x18\x02 \x01(\x0b\x32\x37.batchx.filesystem.ListFolderRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1a\xd4\x01\n\x05Order\x12\x44\n\x08order_by\x18\x01 \x01(\x0e\x32\x32.batchx.filesystem.ListFolderRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"a\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04PATH\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x12\x0c\n\x08POINTERS\x10\x05\"\x87\x02\n\x12ListFolderResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12\x41\n\x06owners\x18\x04 \x03(\x0b\x32\x31.batchx.filesystem.ListFolderResponse.OwnersEntry\x12*\n\tpage_info\x18\x05 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01J\x04\x08\x03\x10\x04\"\xb2\x01\n\x13\x43reateFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12G\n\tuser_data\x18\x03 \x03(\x0b\x32\x34.batchx.filesystem.CreateFolderRequest.UserDataEntry\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x14\x43reateFolderResponse\"8\n\x13\x44\x65leteFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x44\x65leteFolderResponse\"6\n\x11\x44\x65leteFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"8\n\x12\x44\x65leteFileResponse\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x12\x12\n\nother_refs\x18\x02 \x01(\x05\"3\n\x0eGetFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"b\n\x0fGetFileResponse\x12%\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.File\x12\"\n\x05owner\x18\x03 \x01(\x0b\x32\x13.batchx.common.UserJ\x04\x08\x02\x10\x03\"\xe4\x02\n\x04\x46ile\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0e\n\x06\x66older\x18\x03 \x01(\x08\x12-\n\x08metadata\x18\x04 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\r\n\x05owner\x18\x07 \x01(\t\x12.\n\x06status\x18\x08 \x01(\x0e\x32\x1e.batchx.filesystem.File.Status\x12\x10\n\x08pointers\x18\t \x01(\x05\x12\x32\n\x0b\x62lob_status\x18\n \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x13\n\x0bshared_with\x18\x0b \x03(\t\"1\n\x06Status\x12\t\n\x05READY\x10\x00\x12\r\n\tUPLOADING\x10\x01\x12\r\n\tIMPORTING\x10\x02\"V\n\x19ReportUploadStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x16\n\x0euploaded_bytes\x18\x03 \x01(\x03\"\x1c\n\x1aReportUploadStatusResponse\"8\n\x13\x43\x61ncelUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x43\x61ncelUploadResponse\"\xe8\x01\n\x08Metadata\x12\x0e\n\x06length\x18\x01 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12<\n\tuser_data\x18\x03 \x03(\x0b\x32).batchx.filesystem.Metadata.UserDataEntry\x12\x13\n\x0bpart_length\x18\x04 \x01(\x03\x12\x38\n\x0e\x62lob_meta_info\x18\x05 \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x16UploadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12-\n\x08metadata\x18\x03 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"\xa0\x01\n\x17UploadPresignedResponse\x12\x1a\n\x10\x61lready_uploaded\x18\x01 \x01(\x08H\x00\x12H\n\tpart_urls\x18\x02 \x01(\x0b\x32\x33.batchx.filesystem.UploadPresignedResponse.PartUrlsH\x00\x1a\x17\n\x08PartUrls\x12\x0b\n\x03url\x18\x01 \x03(\tB\x06\n\x04\x43\x61se\"h\n\x18\x44ownloadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\r\n\x05range\x18\x03 \x01(\t\x12\x0e\n\x04path\x18\x02 \x01(\tH\x00\x12\x10\n\x06\x64igest\x18\x04 \x01(\tH\x00\x42\x06\n\x04\x43\x61se\"W\n\x19\x44ownloadPresignedResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"o\n\x0b\x43opyRequest\x12\x1a\n\x12source_environment\x18\x01 \x01(\t\x12\x13\n\x0bsource_path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x13\n\x0btarget_path\x18\x04 \x01(\t\"L\n\x15\x43ompleteUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x10\n\x08part_md5\x18\x03 \x03(\t\"\x18\n\x16\x43ompleteUploadResponse*x\n\nBlobStatus\x12\x08\n\x04LIVE\x10\x00\x12\x15\n\x11LIVE_AND_ARCHIVED\x10\x01\x12\x0c\n\x08\x41RCHIVED\x10\x02\x12\r\n\tARCHIVING\x10\n\x12\x0c\n\x08UNLIVING\x10\x0b\x12\r\n\tRESTORING\x10\x0c\x12\x0f\n\x0bUNARCHIVING\x10\r2\xf8\r\n\x11\x46ilesystemService\x12U\n\x07GetFile\x12!.batchx.filesystem.GetFileRequest\x1a\".batchx.filesystem.GetFileResponse\"\x03\x90\x02\x01\x12m\n\x0fUploadPresigned\x12).batchx.filesystem.UploadPresignedRequest\x1a*.batchx.filesystem.UploadPresignedResponse\"\x03\x90\x02\x02\x12v\n\x12ReportUploadStatus\x12,.batchx.filesystem.ReportUploadStatusRequest\x1a-.batchx.filesystem.ReportUploadStatusResponse\"\x03\x90\x02\x02\x12\x64\n\x0c\x43\x61ncelUpload\x12&.batchx.filesystem.CancelUploadRequest\x1a\'.batchx.filesystem.CancelUploadResponse\"\x03\x90\x02\x01\x12n\n\x0e\x43ompleteUpload\x12(.batchx.filesystem.CompleteUploadRequest\x1a).batchx.filesystem.CompleteUploadResponse\"\x07\x90\x02\x02\x88\xa6\x1d\x02\x12s\n\x11\x44ownloadPresigned\x12+.batchx.filesystem.DownloadPresignedRequest\x1a,.batchx.filesystem.DownloadPresignedResponse\"\x03\x90\x02\x02\x12^\n\nDeleteFile\x12$.batchx.filesystem.DeleteFileRequest\x1a%.batchx.filesystem.DeleteFileResponse\"\x03\x90\x02\x02\x12j\n\nListFolder\x12$.batchx.filesystem.ListFolderRequest\x1a%.batchx.filesystem.ListFolderResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12g\n\tListBlobs\x12#.batchx.filesystem.ListBlobsRequest\x1a$.batchx.filesystem.ListBlobsResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12U\n\x07GetBlob\x12!.batchx.filesystem.GetBlobRequest\x1a\".batchx.filesystem.GetBlobResponse\"\x03\x90\x02\x01\x12g\n\rSetBlobStatus\x12\'.batchx.filesystem.SetBlobStatusRequest\x1a(.batchx.filesystem.SetBlobStatusResponse\"\x03\x90\x02\x01\x12|\n\x10ListBlobPointers\x12*.batchx.filesystem.ListBlobPointersRequest\x1a+.batchx.filesystem.ListBlobPointersResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12\x44\n\x04\x43opy\x12\x1e.batchx.filesystem.CopyRequest\x1a\x15.batchx.log.LogRecord\"\x03\x90\x02\x02\x30\x01\x12[\n\tShareFile\x12#.batchx.filesystem.ShareFileRequest\x1a$.batchx.filesystem.ShareFileResponse\"\x03\x90\x02\x02\x12\x61\n\x0b\x41\x64\x64S3Bucket\x12%.batchx.filesystem.AddS3BucketRequest\x1a&.batchx.filesystem.AddS3BucketResponse\"\x03\x90\x02\x02\x12g\n\rListS3Buckets\x12\'.batchx.filesystem.ListS3BucketsRequest\x1a(.batchx.filesystem.ListS3BucketsResponse\"\x03\x90\x02\x02\x12j\n\x0eRemoveS3Bucket\x12(.batchx.filesystem.RemoveS3BucketRequest\x1a).batchx.filesystem.RemoveS3BucketResponse\"\x03\x90\x02\x02\x1a\x0c\x82\x97\"\x02\x08\x32\x82\x97\"\x02\x10\x01\x42\"\n\x0fio.batchx.protoB\x0f\x46ilesystemProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x66ilesystem.proto\x12\x11\x62\x61tchx.filesystem\x1a\tlog.proto\x1a\ttag.proto\x1a\x0c\x63ommon.proto\"e\n\x19ListS3BucketFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\x12\x0e\n\x06\x66older\x18\x03 \x01(\t\x12\x0e\n\x06marker\x18\x04 \x01(\t\"d\n\x1aListS3BucketFolderResponse\x12\x32\n\x07objects\x18\x01 \x03(\x0b\x32!.batchx.filesystem.S3BucketObject\x12\x12\n\nnextMarker\x18\x02 \x01(\t\"\xd9\x01\n\x12\x41\x64\x64S3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\x12\x46\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x31.batchx.filesystem.AddS3BucketRequest.Credentials\x1aQ\n\x0b\x43redentials\x12\x13\n\x0b\x61\x63\x63\x65ssKeyId\x18\x01 \x01(\t\x12\x17\n\x0fsecretAccessKey\x18\x02 \x01(\t\x12\x14\n\x0csessionToken\x18\x03 \x01(\t\"\x15\n\x13\x41\x64\x64S3BucketResponse\"+\n\x14ListS3BucketsRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\"\xbe\x02\n\x15ListS3BucketsResponse\x12?\n\x06\x62ucket\x18\x01 \x03(\x0b\x32/.batchx.filesystem.ListS3BucketsResponse.Bucket\x12@\n\x04user\x18\x02 \x03(\x0b\x32\x32.batchx.filesystem.ListS3BucketsResponse.UserEntry\x1a`\n\x06\x42ucket\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x13\n\x0bts_creation\x18\x04 \x01(\x03\x12\x0e\n\x06public\x18\x05 \x01(\x08\x1a@\n\tUserEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"A\n\x15RemoveS3BucketRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x13\n\x0b\x62ucket_name\x18\x02 \x01(\t\"\x18\n\x16RemoveS3BucketResponse\"\xa9\x01\n\x10ShareFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.batchx.filesystem.ShareFileRequest.Type\"\x1e\n\x04Type\x12\t\n\x05SHARE\x10\x00\x12\x0b\n\x07UNSHARE\x10\x01\"\x13\n\x11ShareFileResponse\"j\n\x14SetBlobStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12-\n\x06status\x18\x03 \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\x17\n\x15SetBlobStatusResponse\"\xad\x05\n\x17ListBlobPointersRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12I\n\npagination\x18\x03 \x01(\x0b\x32\x35.batchx.filesystem.ListBlobPointersRequest.Pagination\x12G\n\tfiltering\x18\x04 \x01(\x0b\x32\x34.batchx.filesystem.ListBlobPointersRequest.Filtering\x12?\n\x05order\x18\x05 \x01(\x0b\x32\x30.batchx.filesystem.ListBlobPointersRequest.Order\x1a\xa3\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12N\n\x07memento\x18\x02 \x01(\x0b\x32=.batchx.filesystem.ListBlobPointersRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1aO\n\tFiltering\x12\r\n\x05owner\x18\x01 \x03(\t\x12\x33\n\x0bts_creation\x18\x02 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x1a\xa0\x01\n\x05Order\x12J\n\x08order_by\x18\x01 \x01(\x0e\x32\x38.batchx.filesystem.ListBlobPointersRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"\'\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bTS_CREATION\x10\x01\"\x8d\x02\n\x18ListBlobPointersResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12G\n\x06owners\x18\x03 \x03(\x0b\x32\x37.batchx.filesystem.ListBlobPointersResponse.OwnersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"\xf4\x06\n\x10ListBlobsRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x38\n\x05order\x18\x02 \x01(\x0b\x32).batchx.filesystem.ListBlobsRequest.Order\x12\x42\n\npagination\x18\x03 \x01(\x0b\x32..batchx.filesystem.ListBlobsRequest.Pagination\x12@\n\tfiltering\x18\x04 \x01(\x0b\x32-.batchx.filesystem.ListBlobsRequest.Filtering\x1a\xc9\x01\n\x05Order\x12\x43\n\x08order_by\x18\x01 \x01(\x0e\x32\x31.batchx.filesystem.ListBlobsRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"W\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08POINTERS\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x1a\x9e\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12G\n\x07memento\x18\x02 \x01(\x0b\x32\x36.batchx.filesystem.ListBlobsRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x19\n\x07Memento\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x1a\x9d\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12/\n\x08pointers\x18\x02 \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12.\n\x06length\x18\x03 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x33\n\x0bts_creation\x18\x04 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x05 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x32\n\x0b\x62lob_status\x18\x06 \x03(\x0e\x32\x1d.batchx.filesystem.BlobStatus\"\xfc\x01\n\x11ListBlobsResponse\x12%\n\x04\x62lob\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.Blob\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12>\n\x05users\x18\x03 \x03(\x0b\x32/.batchx.filesystem.ListBlobsResponse.UsersEntry\x12*\n\tpage_info\x18\x04 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x41\n\nUsersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01\"5\n\x0eGetBlobRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\"8\n\x0fGetBlobResponse\x12%\n\x04\x62lob\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.Blob\"\x83\x03\n\x04\x42lob\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12\x10\n\x08pointers\x18\x03 \x01(\x05\x12\x0e\n\x06length\x18\x04 \x01(\x03\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\x0c\n\x04user\x18\x07 \x01(\t\x12\x15\n\roriginal_path\x18\x08 \x01(\t\x12-\n\x06status\x18\t \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x16\n\x0ets_archivation\x18\n \x01(\x03\x12\x33\n\tmeta_info\x18\x0b \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a\x64\n\x08MetaInfo\x12\x0e\n\x06\x62inary\x18\x01 \x01(\x08\x12\x0c\n\x04gzip\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x63ompressed_size\x18\x03 \x01(\x03\x12\x12\n\nline_count\x18\x04 \x01(\x03\x12\x0b\n\x03new\x18\x05 \x01(\x08\"\x9a\x08\n\x11ListFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x11\n\trecursive\x18\x03 \x01(\x08\x12\x41\n\tfiltering\x18\x04 \x01(\x0b\x32..batchx.filesystem.ListFolderRequest.Filtering\x12\x43\n\npagination\x18\x05 \x01(\x0b\x32/.batchx.filesystem.ListFolderRequest.Pagination\x12\x39\n\x05order\x18\x06 \x01(\x0b\x32*.batchx.filesystem.ListFolderRequest.Order\x12\x18\n\x10user_environment\x18\x07 \x01(\t\x1a\xfa\x02\n\tFiltering\x12\x0c\n\x04user\x18\x01 \x03(\t\x12\x12\n\nonly_ready\x18\x02 \x01(\x08\x12\x17\n\rexclude_files\x18\x03 \x01(\x08H\x00\x12\x19\n\x0f\x65xclude_folders\x18\x04 \x01(\x08H\x00\x12\'\n\x03tag\x18\x05 \x03(\x0b\x32\x1a.batchx.tag.TagCoordinates\x12\x33\n\x0bts_creation\x18\x06 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12\x38\n\x10ts_last_modified\x18\x07 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12.\n\x06length\x18\x08 \x01(\x0b\x32\x1e.batchx.common.LongRangeFilter\x12/\n\x08pointers\x18\t \x01(\x0b\x32\x1d.batchx.common.IntRangeFilter\x12\x16\n\x0e\x66ilename_token\x18\n \x01(\tB\x06\n\x04Type\x1a\x9d\x01\n\nPagination\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12H\n\x07memento\x18\x02 \x01(\x0b\x32\x37.batchx.filesystem.ListFolderRequest.Pagination.Memento\x12\x19\n\x11\x63ompute_page_info\x18\x03 \x01(\x08\x1a\x17\n\x07Memento\x12\x0c\n\x04path\x18\x01 \x01(\t\x1a\xd4\x01\n\x05Order\x12\x44\n\x08order_by\x18\x01 \x01(\x0e\x32\x32.batchx.filesystem.ListFolderRequest.Order.OrderBy\x12\x11\n\torder_asc\x18\x02 \x01(\x08\x12\x0f\n\x07reverse\x18\x03 \x01(\x08\"a\n\x07OrderBy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04PATH\x10\x01\x12\n\n\x06LENGTH\x10\x02\x12\x0f\n\x0bTS_CREATION\x10\x03\x12\x14\n\x10TS_LAST_MODIFIED\x10\x04\x12\x0c\n\x08POINTERS\x10\x05\"\x87\x02\n\x12ListFolderResponse\x12%\n\x04\x66ile\x18\x01 \x03(\x0b\x32\x17.batchx.filesystem.File\x12\x11\n\tlast_page\x18\x02 \x01(\x08\x12\x41\n\x06owners\x18\x04 \x03(\x0b\x32\x31.batchx.filesystem.ListFolderResponse.OwnersEntry\x12*\n\tpage_info\x18\x05 \x01(\x0b\x32\x17.batchx.common.PageInfo\x1a\x42\n\x0bOwnersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.batchx.common.User:\x02\x38\x01J\x04\x08\x03\x10\x04\"\xb2\x01\n\x13\x43reateFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12G\n\tuser_data\x18\x03 \x03(\x0b\x32\x34.batchx.filesystem.CreateFolderRequest.UserDataEntry\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x16\n\x14\x43reateFolderResponse\"8\n\x13\x44\x65leteFolderRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x44\x65leteFolderResponse\"6\n\x11\x44\x65leteFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"8\n\x12\x44\x65leteFileResponse\x12\x0e\n\x06\x64igest\x18\x01 \x01(\t\x12\x12\n\nother_refs\x18\x02 \x01(\x05\"3\n\x0eGetFileRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"b\n\x0fGetFileResponse\x12%\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x17.batchx.filesystem.File\x12\"\n\x05owner\x18\x03 \x01(\x0b\x32\x13.batchx.common.UserJ\x04\x08\x02\x10\x03\"\xe4\x02\n\x04\x46ile\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0e\n\x06\x66older\x18\x03 \x01(\x08\x12-\n\x08metadata\x18\x04 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\x12\x13\n\x0bts_creation\x18\x05 \x01(\x03\x12\x18\n\x10ts_last_modified\x18\x06 \x01(\x03\x12\r\n\x05owner\x18\x07 \x01(\t\x12.\n\x06status\x18\x08 \x01(\x0e\x32\x1e.batchx.filesystem.File.Status\x12\x10\n\x08pointers\x18\t \x01(\x05\x12\x32\n\x0b\x62lob_status\x18\n \x01(\x0e\x32\x1d.batchx.filesystem.BlobStatus\x12\x13\n\x0bshared_with\x18\x0b \x03(\t\"1\n\x06Status\x12\t\n\x05READY\x10\x00\x12\r\n\tUPLOADING\x10\x01\x12\r\n\tIMPORTING\x10\x02\"\xe8\x02\n\x0eS3BucketObject\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0e\n\x06\x66older\x18\x02 \x01(\x08\x12\x0e\n\x06length\x18\x03 \x01(\x03\x12\x0c\n\x04\x65tag\x18\x04 \x01(\t\x12\x18\n\x10ts_last_modified\x18\x05 \x01(\x03\x12\x45\n\rstorage_class\x18\x06 \x01(\x0e\x32..batchx.filesystem.S3BucketObject.StorageClass\"\xb8\x01\n\x0cStorageClass\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08STANDARD\x10\x01\x12\x16\n\x12REDUCED_REDUNDANCY\x10\x02\x12\x0b\n\x07GLACIER\x10\x03\x12\x0f\n\x0bSTANDARD_IA\x10\x04\x12\x0e\n\nONEZONE_IA\x10\x05\x12\x17\n\x13INTELLIGENT_TIERING\x10\x06\x12\x10\n\x0c\x44\x45\x45P_ARCHIVE\x10\x07\x12\x0c\n\x08OUTPOSTS\x10\x08\x12\x0e\n\nGLACIER_IR\x10\t\"V\n\x19ReportUploadStatusRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x16\n\x0euploaded_bytes\x18\x03 \x01(\x03\"\x1c\n\x1aReportUploadStatusResponse\"8\n\x13\x43\x61ncelUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x16\n\x14\x43\x61ncelUploadResponse\"\xe8\x01\n\x08Metadata\x12\x0e\n\x06length\x18\x01 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x02 \x01(\t\x12<\n\tuser_data\x18\x03 \x03(\x0b\x32).batchx.filesystem.Metadata.UserDataEntry\x12\x13\n\x0bpart_length\x18\x04 \x01(\x03\x12\x38\n\x0e\x62lob_meta_info\x18\x05 \x01(\x0b\x32 .batchx.filesystem.Blob.MetaInfo\x1a/\n\rUserDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x16UploadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12-\n\x08metadata\x18\x03 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"\xa0\x01\n\x17UploadPresignedResponse\x12\x1a\n\x10\x61lready_uploaded\x18\x01 \x01(\x08H\x00\x12H\n\tpart_urls\x18\x02 \x01(\x0b\x32\x33.batchx.filesystem.UploadPresignedResponse.PartUrlsH\x00\x1a\x17\n\x08PartUrls\x12\x0b\n\x03url\x18\x01 \x03(\tB\x06\n\x04\x43\x61se\"h\n\x18\x44ownloadPresignedRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\r\n\x05range\x18\x03 \x01(\t\x12\x0e\n\x04path\x18\x02 \x01(\tH\x00\x12\x10\n\x06\x64igest\x18\x04 \x01(\tH\x00\x42\x06\n\x04\x43\x61se\"W\n\x19\x44ownloadPresignedResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.batchx.filesystem.Metadata\"o\n\x0b\x43opyRequest\x12\x1a\n\x12source_environment\x18\x01 \x01(\t\x12\x13\n\x0bsource_path\x18\x02 \x01(\t\x12\x1a\n\x12target_environment\x18\x03 \x01(\t\x12\x13\n\x0btarget_path\x18\x04 \x01(\t\"L\n\x15\x43ompleteUploadRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x10\n\x08part_md5\x18\x03 \x03(\t\"\x18\n\x16\x43ompleteUploadResponse*x\n\nBlobStatus\x12\x08\n\x04LIVE\x10\x00\x12\x15\n\x11LIVE_AND_ARCHIVED\x10\x01\x12\x0c\n\x08\x41RCHIVED\x10\x02\x12\r\n\tARCHIVING\x10\n\x12\x0c\n\x08UNLIVING\x10\x0b\x12\r\n\tRESTORING\x10\x0c\x12\x0f\n\x0bUNARCHIVING\x10\r2\xf0\x0e\n\x11\x46ilesystemService\x12U\n\x07GetFile\x12!.batchx.filesystem.GetFileRequest\x1a\".batchx.filesystem.GetFileResponse\"\x03\x90\x02\x01\x12m\n\x0fUploadPresigned\x12).batchx.filesystem.UploadPresignedRequest\x1a*.batchx.filesystem.UploadPresignedResponse\"\x03\x90\x02\x02\x12v\n\x12ReportUploadStatus\x12,.batchx.filesystem.ReportUploadStatusRequest\x1a-.batchx.filesystem.ReportUploadStatusResponse\"\x03\x90\x02\x02\x12\x64\n\x0c\x43\x61ncelUpload\x12&.batchx.filesystem.CancelUploadRequest\x1a\'.batchx.filesystem.CancelUploadResponse\"\x03\x90\x02\x01\x12n\n\x0e\x43ompleteUpload\x12(.batchx.filesystem.CompleteUploadRequest\x1a).batchx.filesystem.CompleteUploadResponse\"\x07\x90\x02\x02\x88\xa6\x1d\x02\x12s\n\x11\x44ownloadPresigned\x12+.batchx.filesystem.DownloadPresignedRequest\x1a,.batchx.filesystem.DownloadPresignedResponse\"\x03\x90\x02\x02\x12^\n\nDeleteFile\x12$.batchx.filesystem.DeleteFileRequest\x1a%.batchx.filesystem.DeleteFileResponse\"\x03\x90\x02\x02\x12j\n\nListFolder\x12$.batchx.filesystem.ListFolderRequest\x1a%.batchx.filesystem.ListFolderResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12g\n\tListBlobs\x12#.batchx.filesystem.ListBlobsRequest\x1a$.batchx.filesystem.ListBlobsResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12U\n\x07GetBlob\x12!.batchx.filesystem.GetBlobRequest\x1a\".batchx.filesystem.GetBlobResponse\"\x03\x90\x02\x01\x12g\n\rSetBlobStatus\x12\'.batchx.filesystem.SetBlobStatusRequest\x1a(.batchx.filesystem.SetBlobStatusResponse\"\x03\x90\x02\x01\x12|\n\x10ListBlobPointers\x12*.batchx.filesystem.ListBlobPointersRequest\x1a+.batchx.filesystem.ListBlobPointersResponse\"\x0f\x90\x02\x01\x82\xa6\x1d\x02\x08\x05\x82\xa6\x1d\x02\x10\x01\x12\x44\n\x04\x43opy\x12\x1e.batchx.filesystem.CopyRequest\x1a\x15.batchx.log.LogRecord\"\x03\x90\x02\x02\x30\x01\x12[\n\tShareFile\x12#.batchx.filesystem.ShareFileRequest\x1a$.batchx.filesystem.ShareFileResponse\"\x03\x90\x02\x02\x12\x61\n\x0b\x41\x64\x64S3Bucket\x12%.batchx.filesystem.AddS3BucketRequest\x1a&.batchx.filesystem.AddS3BucketResponse\"\x03\x90\x02\x02\x12g\n\rListS3Buckets\x12\'.batchx.filesystem.ListS3BucketsRequest\x1a(.batchx.filesystem.ListS3BucketsResponse\"\x03\x90\x02\x02\x12j\n\x0eRemoveS3Bucket\x12(.batchx.filesystem.RemoveS3BucketRequest\x1a).batchx.filesystem.RemoveS3BucketResponse\"\x03\x90\x02\x02\x12v\n\x12ListS3BucketFolder\x12,.batchx.filesystem.ListS3BucketFolderRequest\x1a-.batchx.filesystem.ListS3BucketFolderResponse\"\x03\x90\x02\x01\x1a\x0c\x82\x97\"\x02\x08\x32\x82\x97\"\x02\x10\x01\x42\"\n\x0fio.batchx.protoB\x0f\x46ilesystemProtob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'filesystem_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017io.batchx.protoB\017FilesystemProto'
@@ -68,146 +68,156 @@
   _FILESYSTEMSERVICE.methods_by_name['ShareFile']._serialized_options = b'\220\002\002'
   _FILESYSTEMSERVICE.methods_by_name['AddS3Bucket']._options = None
   _FILESYSTEMSERVICE.methods_by_name['AddS3Bucket']._serialized_options = b'\220\002\002'
   _FILESYSTEMSERVICE.methods_by_name['ListS3Buckets']._options = None
   _FILESYSTEMSERVICE.methods_by_name['ListS3Buckets']._serialized_options = b'\220\002\002'
   _FILESYSTEMSERVICE.methods_by_name['RemoveS3Bucket']._options = None
   _FILESYSTEMSERVICE.methods_by_name['RemoveS3Bucket']._serialized_options = b'\220\002\002'
-  _BLOBSTATUS._serialized_start=7058
-  _BLOBSTATUS._serialized_end=7178
-  _ADDS3BUCKETREQUEST._serialized_start=76
-  _ADDS3BUCKETREQUEST._serialized_end=293
-  _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_start=212
-  _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_end=293
-  _ADDS3BUCKETRESPONSE._serialized_start=295
-  _ADDS3BUCKETRESPONSE._serialized_end=316
-  _LISTS3BUCKETSREQUEST._serialized_start=318
-  _LISTS3BUCKETSREQUEST._serialized_end=361
-  _LISTS3BUCKETSRESPONSE._serialized_start=364
-  _LISTS3BUCKETSRESPONSE._serialized_end=682
-  _LISTS3BUCKETSRESPONSE_BUCKET._serialized_start=520
-  _LISTS3BUCKETSRESPONSE_BUCKET._serialized_end=616
-  _LISTS3BUCKETSRESPONSE_USERENTRY._serialized_start=618
-  _LISTS3BUCKETSRESPONSE_USERENTRY._serialized_end=682
-  _REMOVES3BUCKETREQUEST._serialized_start=684
-  _REMOVES3BUCKETREQUEST._serialized_end=749
-  _REMOVES3BUCKETRESPONSE._serialized_start=751
-  _REMOVES3BUCKETRESPONSE._serialized_end=775
-  _SHAREFILEREQUEST._serialized_start=778
-  _SHAREFILEREQUEST._serialized_end=947
-  _SHAREFILEREQUEST_TYPE._serialized_start=917
-  _SHAREFILEREQUEST_TYPE._serialized_end=947
-  _SHAREFILERESPONSE._serialized_start=949
-  _SHAREFILERESPONSE._serialized_end=968
-  _SETBLOBSTATUSREQUEST._serialized_start=970
-  _SETBLOBSTATUSREQUEST._serialized_end=1076
-  _SETBLOBSTATUSRESPONSE._serialized_start=1078
-  _SETBLOBSTATUSRESPONSE._serialized_end=1101
-  _LISTBLOBPOINTERSREQUEST._serialized_start=1104
-  _LISTBLOBPOINTERSREQUEST._serialized_end=1789
-  _LISTBLOBPOINTERSREQUEST_PAGINATION._serialized_start=1382
-  _LISTBLOBPOINTERSREQUEST_PAGINATION._serialized_end=1545
-  _LISTBLOBPOINTERSREQUEST_PAGINATION_MEMENTO._serialized_start=1522
-  _LISTBLOBPOINTERSREQUEST_PAGINATION_MEMENTO._serialized_end=1545
-  _LISTBLOBPOINTERSREQUEST_FILTERING._serialized_start=1547
-  _LISTBLOBPOINTERSREQUEST_FILTERING._serialized_end=1626
-  _LISTBLOBPOINTERSREQUEST_ORDER._serialized_start=1629
-  _LISTBLOBPOINTERSREQUEST_ORDER._serialized_end=1789
-  _LISTBLOBPOINTERSREQUEST_ORDER_ORDERBY._serialized_start=1750
-  _LISTBLOBPOINTERSREQUEST_ORDER_ORDERBY._serialized_end=1789
-  _LISTBLOBPOINTERSRESPONSE._serialized_start=1792
-  _LISTBLOBPOINTERSRESPONSE._serialized_end=2061
-  _LISTBLOBPOINTERSRESPONSE_OWNERSENTRY._serialized_start=1995
-  _LISTBLOBPOINTERSRESPONSE_OWNERSENTRY._serialized_end=2061
-  _LISTBLOBSREQUEST._serialized_start=2064
-  _LISTBLOBSREQUEST._serialized_end=2948
-  _LISTBLOBSREQUEST_ORDER._serialized_start=2298
-  _LISTBLOBSREQUEST_ORDER._serialized_end=2499
-  _LISTBLOBSREQUEST_ORDER_ORDERBY._serialized_start=2412
-  _LISTBLOBSREQUEST_ORDER_ORDERBY._serialized_end=2499
-  _LISTBLOBSREQUEST_PAGINATION._serialized_start=2502
-  _LISTBLOBSREQUEST_PAGINATION._serialized_end=2660
-  _LISTBLOBSREQUEST_PAGINATION_MEMENTO._serialized_start=2635
-  _LISTBLOBSREQUEST_PAGINATION_MEMENTO._serialized_end=2660
-  _LISTBLOBSREQUEST_FILTERING._serialized_start=2663
-  _LISTBLOBSREQUEST_FILTERING._serialized_end=2948
-  _LISTBLOBSRESPONSE._serialized_start=2951
-  _LISTBLOBSRESPONSE._serialized_end=3203
-  _LISTBLOBSRESPONSE_USERSENTRY._serialized_start=3138
-  _LISTBLOBSRESPONSE_USERSENTRY._serialized_end=3203
-  _GETBLOBREQUEST._serialized_start=3205
-  _GETBLOBREQUEST._serialized_end=3258
-  _GETBLOBRESPONSE._serialized_start=3260
-  _GETBLOBRESPONSE._serialized_end=3316
-  _BLOB._serialized_start=3319
-  _BLOB._serialized_end=3706
-  _BLOB_METAINFO._serialized_start=3606
-  _BLOB_METAINFO._serialized_end=3706
-  _LISTFOLDERREQUEST._serialized_start=3709
-  _LISTFOLDERREQUEST._serialized_end=4759
-  _LISTFOLDERREQUEST_FILTERING._serialized_start=4006
-  _LISTFOLDERREQUEST_FILTERING._serialized_end=4384
-  _LISTFOLDERREQUEST_PAGINATION._serialized_start=4387
-  _LISTFOLDERREQUEST_PAGINATION._serialized_end=4544
-  _LISTFOLDERREQUEST_PAGINATION_MEMENTO._serialized_start=1522
-  _LISTFOLDERREQUEST_PAGINATION_MEMENTO._serialized_end=1545
-  _LISTFOLDERREQUEST_ORDER._serialized_start=4547
-  _LISTFOLDERREQUEST_ORDER._serialized_end=4759
-  _LISTFOLDERREQUEST_ORDER_ORDERBY._serialized_start=4662
-  _LISTFOLDERREQUEST_ORDER_ORDERBY._serialized_end=4759
-  _LISTFOLDERRESPONSE._serialized_start=4762
-  _LISTFOLDERRESPONSE._serialized_end=5025
-  _LISTFOLDERRESPONSE_OWNERSENTRY._serialized_start=1995
-  _LISTFOLDERRESPONSE_OWNERSENTRY._serialized_end=2061
-  _CREATEFOLDERREQUEST._serialized_start=5028
-  _CREATEFOLDERREQUEST._serialized_end=5206
-  _CREATEFOLDERREQUEST_USERDATAENTRY._serialized_start=5159
-  _CREATEFOLDERREQUEST_USERDATAENTRY._serialized_end=5206
-  _CREATEFOLDERRESPONSE._serialized_start=5208
-  _CREATEFOLDERRESPONSE._serialized_end=5230
-  _DELETEFOLDERREQUEST._serialized_start=5232
-  _DELETEFOLDERREQUEST._serialized_end=5288
-  _DELETEFOLDERRESPONSE._serialized_start=5290
-  _DELETEFOLDERRESPONSE._serialized_end=5312
-  _DELETEFILEREQUEST._serialized_start=5314
-  _DELETEFILEREQUEST._serialized_end=5368
-  _DELETEFILERESPONSE._serialized_start=5370
-  _DELETEFILERESPONSE._serialized_end=5426
-  _GETFILEREQUEST._serialized_start=5428
-  _GETFILEREQUEST._serialized_end=5479
-  _GETFILERESPONSE._serialized_start=5481
-  _GETFILERESPONSE._serialized_end=5579
-  _FILE._serialized_start=5582
-  _FILE._serialized_end=5938
-  _FILE_STATUS._serialized_start=5889
-  _FILE_STATUS._serialized_end=5938
-  _REPORTUPLOADSTATUSREQUEST._serialized_start=5940
-  _REPORTUPLOADSTATUSREQUEST._serialized_end=6026
-  _REPORTUPLOADSTATUSRESPONSE._serialized_start=6028
-  _REPORTUPLOADSTATUSRESPONSE._serialized_end=6056
-  _CANCELUPLOADREQUEST._serialized_start=6058
-  _CANCELUPLOADREQUEST._serialized_end=6114
-  _CANCELUPLOADRESPONSE._serialized_start=6116
-  _CANCELUPLOADRESPONSE._serialized_end=6138
-  _METADATA._serialized_start=6141
-  _METADATA._serialized_end=6373
-  _METADATA_USERDATAENTRY._serialized_start=5159
-  _METADATA_USERDATAENTRY._serialized_end=5206
-  _UPLOADPRESIGNEDREQUEST._serialized_start=6375
-  _UPLOADPRESIGNEDREQUEST._serialized_end=6481
-  _UPLOADPRESIGNEDRESPONSE._serialized_start=6484
-  _UPLOADPRESIGNEDRESPONSE._serialized_end=6644
-  _UPLOADPRESIGNEDRESPONSE_PARTURLS._serialized_start=6613
-  _UPLOADPRESIGNEDRESPONSE_PARTURLS._serialized_end=6636
-  _DOWNLOADPRESIGNEDREQUEST._serialized_start=6646
-  _DOWNLOADPRESIGNEDREQUEST._serialized_end=6750
-  _DOWNLOADPRESIGNEDRESPONSE._serialized_start=6752
-  _DOWNLOADPRESIGNEDRESPONSE._serialized_end=6839
-  _COPYREQUEST._serialized_start=6841
-  _COPYREQUEST._serialized_end=6952
-  _COMPLETEUPLOADREQUEST._serialized_start=6954
-  _COMPLETEUPLOADREQUEST._serialized_end=7030
-  _COMPLETEUPLOADRESPONSE._serialized_start=7032
-  _COMPLETEUPLOADRESPONSE._serialized_end=7056
-  _FILESYSTEMSERVICE._serialized_start=7181
-  _FILESYSTEMSERVICE._serialized_end=8965
+  _FILESYSTEMSERVICE.methods_by_name['ListS3BucketFolder']._options = None
+  _FILESYSTEMSERVICE.methods_by_name['ListS3BucketFolder']._serialized_options = b'\220\002\001'
+  _BLOBSTATUS._serialized_start=7626
+  _BLOBSTATUS._serialized_end=7746
+  _LISTS3BUCKETFOLDERREQUEST._serialized_start=75
+  _LISTS3BUCKETFOLDERREQUEST._serialized_end=176
+  _LISTS3BUCKETFOLDERRESPONSE._serialized_start=178
+  _LISTS3BUCKETFOLDERRESPONSE._serialized_end=278
+  _ADDS3BUCKETREQUEST._serialized_start=281
+  _ADDS3BUCKETREQUEST._serialized_end=498
+  _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_start=417
+  _ADDS3BUCKETREQUEST_CREDENTIALS._serialized_end=498
+  _ADDS3BUCKETRESPONSE._serialized_start=500
+  _ADDS3BUCKETRESPONSE._serialized_end=521
+  _LISTS3BUCKETSREQUEST._serialized_start=523
+  _LISTS3BUCKETSREQUEST._serialized_end=566
+  _LISTS3BUCKETSRESPONSE._serialized_start=569
+  _LISTS3BUCKETSRESPONSE._serialized_end=887
+  _LISTS3BUCKETSRESPONSE_BUCKET._serialized_start=725
+  _LISTS3BUCKETSRESPONSE_BUCKET._serialized_end=821
+  _LISTS3BUCKETSRESPONSE_USERENTRY._serialized_start=823
+  _LISTS3BUCKETSRESPONSE_USERENTRY._serialized_end=887
+  _REMOVES3BUCKETREQUEST._serialized_start=889
+  _REMOVES3BUCKETREQUEST._serialized_end=954
+  _REMOVES3BUCKETRESPONSE._serialized_start=956
+  _REMOVES3BUCKETRESPONSE._serialized_end=980
+  _SHAREFILEREQUEST._serialized_start=983
+  _SHAREFILEREQUEST._serialized_end=1152
+  _SHAREFILEREQUEST_TYPE._serialized_start=1122
+  _SHAREFILEREQUEST_TYPE._serialized_end=1152
+  _SHAREFILERESPONSE._serialized_start=1154
+  _SHAREFILERESPONSE._serialized_end=1173
+  _SETBLOBSTATUSREQUEST._serialized_start=1175
+  _SETBLOBSTATUSREQUEST._serialized_end=1281
+  _SETBLOBSTATUSRESPONSE._serialized_start=1283
+  _SETBLOBSTATUSRESPONSE._serialized_end=1306
+  _LISTBLOBPOINTERSREQUEST._serialized_start=1309
+  _LISTBLOBPOINTERSREQUEST._serialized_end=1994
+  _LISTBLOBPOINTERSREQUEST_PAGINATION._serialized_start=1587
+  _LISTBLOBPOINTERSREQUEST_PAGINATION._serialized_end=1750
+  _LISTBLOBPOINTERSREQUEST_PAGINATION_MEMENTO._serialized_start=1727
+  _LISTBLOBPOINTERSREQUEST_PAGINATION_MEMENTO._serialized_end=1750
+  _LISTBLOBPOINTERSREQUEST_FILTERING._serialized_start=1752
+  _LISTBLOBPOINTERSREQUEST_FILTERING._serialized_end=1831
+  _LISTBLOBPOINTERSREQUEST_ORDER._serialized_start=1834
+  _LISTBLOBPOINTERSREQUEST_ORDER._serialized_end=1994
+  _LISTBLOBPOINTERSREQUEST_ORDER_ORDERBY._serialized_start=1955
+  _LISTBLOBPOINTERSREQUEST_ORDER_ORDERBY._serialized_end=1994
+  _LISTBLOBPOINTERSRESPONSE._serialized_start=1997
+  _LISTBLOBPOINTERSRESPONSE._serialized_end=2266
+  _LISTBLOBPOINTERSRESPONSE_OWNERSENTRY._serialized_start=2200
+  _LISTBLOBPOINTERSRESPONSE_OWNERSENTRY._serialized_end=2266
+  _LISTBLOBSREQUEST._serialized_start=2269
+  _LISTBLOBSREQUEST._serialized_end=3153
+  _LISTBLOBSREQUEST_ORDER._serialized_start=2503
+  _LISTBLOBSREQUEST_ORDER._serialized_end=2704
+  _LISTBLOBSREQUEST_ORDER_ORDERBY._serialized_start=2617
+  _LISTBLOBSREQUEST_ORDER_ORDERBY._serialized_end=2704
+  _LISTBLOBSREQUEST_PAGINATION._serialized_start=2707
+  _LISTBLOBSREQUEST_PAGINATION._serialized_end=2865
+  _LISTBLOBSREQUEST_PAGINATION_MEMENTO._serialized_start=2840
+  _LISTBLOBSREQUEST_PAGINATION_MEMENTO._serialized_end=2865
+  _LISTBLOBSREQUEST_FILTERING._serialized_start=2868
+  _LISTBLOBSREQUEST_FILTERING._serialized_end=3153
+  _LISTBLOBSRESPONSE._serialized_start=3156
+  _LISTBLOBSRESPONSE._serialized_end=3408
+  _LISTBLOBSRESPONSE_USERSENTRY._serialized_start=3343
+  _LISTBLOBSRESPONSE_USERSENTRY._serialized_end=3408
+  _GETBLOBREQUEST._serialized_start=3410
+  _GETBLOBREQUEST._serialized_end=3463
+  _GETBLOBRESPONSE._serialized_start=3465
+  _GETBLOBRESPONSE._serialized_end=3521
+  _BLOB._serialized_start=3524
+  _BLOB._serialized_end=3911
+  _BLOB_METAINFO._serialized_start=3811
+  _BLOB_METAINFO._serialized_end=3911
+  _LISTFOLDERREQUEST._serialized_start=3914
+  _LISTFOLDERREQUEST._serialized_end=4964
+  _LISTFOLDERREQUEST_FILTERING._serialized_start=4211
+  _LISTFOLDERREQUEST_FILTERING._serialized_end=4589
+  _LISTFOLDERREQUEST_PAGINATION._serialized_start=4592
+  _LISTFOLDERREQUEST_PAGINATION._serialized_end=4749
+  _LISTFOLDERREQUEST_PAGINATION_MEMENTO._serialized_start=1727
+  _LISTFOLDERREQUEST_PAGINATION_MEMENTO._serialized_end=1750
+  _LISTFOLDERREQUEST_ORDER._serialized_start=4752
+  _LISTFOLDERREQUEST_ORDER._serialized_end=4964
+  _LISTFOLDERREQUEST_ORDER_ORDERBY._serialized_start=4867
+  _LISTFOLDERREQUEST_ORDER_ORDERBY._serialized_end=4964
+  _LISTFOLDERRESPONSE._serialized_start=4967
+  _LISTFOLDERRESPONSE._serialized_end=5230
+  _LISTFOLDERRESPONSE_OWNERSENTRY._serialized_start=2200
+  _LISTFOLDERRESPONSE_OWNERSENTRY._serialized_end=2266
+  _CREATEFOLDERREQUEST._serialized_start=5233
+  _CREATEFOLDERREQUEST._serialized_end=5411
+  _CREATEFOLDERREQUEST_USERDATAENTRY._serialized_start=5364
+  _CREATEFOLDERREQUEST_USERDATAENTRY._serialized_end=5411
+  _CREATEFOLDERRESPONSE._serialized_start=5413
+  _CREATEFOLDERRESPONSE._serialized_end=5435
+  _DELETEFOLDERREQUEST._serialized_start=5437
+  _DELETEFOLDERREQUEST._serialized_end=5493
+  _DELETEFOLDERRESPONSE._serialized_start=5495
+  _DELETEFOLDERRESPONSE._serialized_end=5517
+  _DELETEFILEREQUEST._serialized_start=5519
+  _DELETEFILEREQUEST._serialized_end=5573
+  _DELETEFILERESPONSE._serialized_start=5575
+  _DELETEFILERESPONSE._serialized_end=5631
+  _GETFILEREQUEST._serialized_start=5633
+  _GETFILEREQUEST._serialized_end=5684
+  _GETFILERESPONSE._serialized_start=5686
+  _GETFILERESPONSE._serialized_end=5784
+  _FILE._serialized_start=5787
+  _FILE._serialized_end=6143
+  _FILE_STATUS._serialized_start=6094
+  _FILE_STATUS._serialized_end=6143
+  _S3BUCKETOBJECT._serialized_start=6146
+  _S3BUCKETOBJECT._serialized_end=6506
+  _S3BUCKETOBJECT_STORAGECLASS._serialized_start=6322
+  _S3BUCKETOBJECT_STORAGECLASS._serialized_end=6506
+  _REPORTUPLOADSTATUSREQUEST._serialized_start=6508
+  _REPORTUPLOADSTATUSREQUEST._serialized_end=6594
+  _REPORTUPLOADSTATUSRESPONSE._serialized_start=6596
+  _REPORTUPLOADSTATUSRESPONSE._serialized_end=6624
+  _CANCELUPLOADREQUEST._serialized_start=6626
+  _CANCELUPLOADREQUEST._serialized_end=6682
+  _CANCELUPLOADRESPONSE._serialized_start=6684
+  _CANCELUPLOADRESPONSE._serialized_end=6706
+  _METADATA._serialized_start=6709
+  _METADATA._serialized_end=6941
+  _METADATA_USERDATAENTRY._serialized_start=5364
+  _METADATA_USERDATAENTRY._serialized_end=5411
+  _UPLOADPRESIGNEDREQUEST._serialized_start=6943
+  _UPLOADPRESIGNEDREQUEST._serialized_end=7049
+  _UPLOADPRESIGNEDRESPONSE._serialized_start=7052
+  _UPLOADPRESIGNEDRESPONSE._serialized_end=7212
+  _UPLOADPRESIGNEDRESPONSE_PARTURLS._serialized_start=7181
+  _UPLOADPRESIGNEDRESPONSE_PARTURLS._serialized_end=7204
+  _DOWNLOADPRESIGNEDREQUEST._serialized_start=7214
+  _DOWNLOADPRESIGNEDREQUEST._serialized_end=7318
+  _DOWNLOADPRESIGNEDRESPONSE._serialized_start=7320
+  _DOWNLOADPRESIGNEDRESPONSE._serialized_end=7407
+  _COPYREQUEST._serialized_start=7409
+  _COPYREQUEST._serialized_end=7520
+  _COMPLETEUPLOADREQUEST._serialized_start=7522
+  _COMPLETEUPLOADREQUEST._serialized_end=7598
+  _COMPLETEUPLOADRESPONSE._serialized_start=7600
+  _COMPLETEUPLOADRESPONSE._serialized_end=7624
+  _FILESYSTEMSERVICE._serialized_start=7749
+  _FILESYSTEMSERVICE._serialized_end=9653
 # @@protoc_insertion_point(module_scope)
```

### Comparing `batchx-9.7.4/batchx/filesystem_pb2_grpc.py` & `batchx-9.8.0/batchx/filesystem_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,19 @@
                 response_deserializer=filesystem__pb2.ListS3BucketsResponse.FromString,
                 )
         self.RemoveS3Bucket = channel.unary_unary(
                 '/batchx.filesystem.FilesystemService/RemoveS3Bucket',
                 request_serializer=filesystem__pb2.RemoveS3BucketRequest.SerializeToString,
                 response_deserializer=filesystem__pb2.RemoveS3BucketResponse.FromString,
                 )
+        self.ListS3BucketFolder = channel.unary_unary(
+                '/batchx.filesystem.FilesystemService/ListS3BucketFolder',
+                request_serializer=filesystem__pb2.ListS3BucketFolderRequest.SerializeToString,
+                response_deserializer=filesystem__pb2.ListS3BucketFolderResponse.FromString,
+                )
 
 
 class FilesystemServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetFile(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -203,14 +208,20 @@
 
     def RemoveS3Bucket(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListS3BucketFolder(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_FilesystemServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetFile': grpc.unary_unary_rpc_method_handler(
                     servicer.GetFile,
                     request_deserializer=filesystem__pb2.GetFileRequest.FromString,
                     response_serializer=filesystem__pb2.GetFileResponse.SerializeToString,
@@ -291,14 +302,19 @@
                     response_serializer=filesystem__pb2.ListS3BucketsResponse.SerializeToString,
             ),
             'RemoveS3Bucket': grpc.unary_unary_rpc_method_handler(
                     servicer.RemoveS3Bucket,
                     request_deserializer=filesystem__pb2.RemoveS3BucketRequest.FromString,
                     response_serializer=filesystem__pb2.RemoveS3BucketResponse.SerializeToString,
             ),
+            'ListS3BucketFolder': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListS3BucketFolder,
+                    request_deserializer=filesystem__pb2.ListS3BucketFolderRequest.FromString,
+                    response_serializer=filesystem__pb2.ListS3BucketFolderResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'batchx.filesystem.FilesystemService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -589,7 +605,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/batchx.filesystem.FilesystemService/RemoveS3Bucket',
             filesystem__pb2.RemoveS3BucketRequest.SerializeToString,
             filesystem__pb2.RemoveS3BucketResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListS3BucketFolder(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/batchx.filesystem.FilesystemService/ListS3BucketFolder',
+            filesystem__pb2.ListS3BucketFolderRequest.SerializeToString,
+            filesystem__pb2.ListS3BucketFolderResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `batchx-9.7.4/batchx/health_pb2.py` & `batchx-9.8.0/batchx/health_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/health_pb2_grpc.py` & `batchx-9.8.0/batchx/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/image_pb2.py` & `batchx-9.8.0/batchx/image_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/image_pb2_grpc.py` & `batchx-9.8.0/batchx/image_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/job_pb2.py` & `batchx-9.8.0/batchx/job_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/job_pb2_grpc.py` & `batchx-9.8.0/batchx/job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/log_pb2.py` & `batchx-9.8.0/batchx/log_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/organization_pb2.py` & `batchx-9.8.0/batchx/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/organization_pb2_grpc.py` & `batchx-9.8.0/batchx/organization_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/picture_pb2.py` & `batchx-9.8.0/batchx/picture_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/picture_pb2_grpc.py` & `batchx-9.8.0/batchx/picture_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/profile_pb2.py` & `batchx-9.8.0/batchx/profile_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/provider_pb2.py` & `batchx-9.8.0/batchx/provider_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/provider_pb2_grpc.py` & `batchx-9.8.0/batchx/provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/tag_pb2.py` & `batchx-9.8.0/batchx/tag_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/tag_pb2_grpc.py` & `batchx-9.8.0/batchx/tag_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/token_pb2.py` & `batchx-9.8.0/batchx/token_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/token_pb2_grpc.py` & `batchx-9.8.0/batchx/token_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/user_pb2.py` & `batchx-9.8.0/batchx/user_pb2.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx/user_pb2_grpc.py` & `batchx-9.8.0/batchx/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/batchx.egg-info/PKG-INFO` & `batchx-9.8.0/batchx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchx
-Version: 9.7.4
+Version: 9.8.0
 Summary: Batchx Python API
 Home-page: https://github.com/batchx/api
 Author: Batchx
 Author-email: dev@batchx.com
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `batchx-9.7.4/batchx.egg-info/SOURCES.txt` & `batchx-9.8.0/batchx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batchx-9.7.4/setup.py` & `batchx-9.8.0/setup.py`

 * *Files identical despite different names*

