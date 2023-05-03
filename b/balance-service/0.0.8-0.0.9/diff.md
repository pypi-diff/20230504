# Comparing `tmp/balance_service-0.0.8.tar.gz` & `tmp/balance_service-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/service/service/dist/.tmp-w_0nu3ey/balance_service-0.0.8.tar", last modified: Sat Mar 18 23:59:07 2023, max compression
+gzip compressed data, was "/home/runner/work/service/service/dist/.tmp-xprfadj3/balance_service-0.0.9.tar", last modified: Fri Mar 31 20:39:41 2023, max compression
```

## Comparing `balance_service-0.0.8.tar` & `balance_service-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-18 23:59:07.000000 balance_service-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)      499 2023-03-18 23:59:07.000000 balance_service-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      187 2023-03-18 23:58:57.000000 balance_service-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-18 23:59:07.000000 balance_service-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2023-03-18 23:58:57.000000 balance_service-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/balance_service/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-18 23:58:57.000000 balance_service-0.0.8/src/balance_service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/balance_service/interfaces/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-18 23:58:57.000000 balance_service-0.0.8/src/balance_service/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1150 2023-03-18 23:58:57.000000 balance_service-0.0.8/src/balance_service/interfaces/boto_s3.py
--rw-r--r--   0 runner    (1001) docker     (116)     1344 2023-03-18 23:58:57.000000 balance_service-0.0.8/src/balance_service/interfaces/nubank.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/balance_service/repositories/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-18 23:58:57.000000 balance_service-0.0.8/src/balance_service/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      323 2023-03-18 23:58:57.000000 balance_service-0.0.8/src/balance_service/repositories/bank.py
--rw-r--r--   0 runner    (1001) docker     (116)      324 2023-03-18 23:58:57.000000 balance_service-0.0.8/src/balance_service/repositories/user.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/balance_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      499 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/balance_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      518 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/balance_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/balance_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/balance_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2023-03-18 23:59:07.000000 balance_service-0.0.8/src/balance_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-31 20:39:41.000000 balance_service-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      499 2023-03-31 20:39:41.000000 balance_service-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      187 2023-03-31 20:39:22.000000 balance_service-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-31 20:39:41.000000 balance_service-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1069 2023-03-31 20:39:22.000000 balance_service-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/balance_service/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-31 20:39:22.000000 balance_service-0.0.9/src/balance_service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/balance_service/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-31 20:39:22.000000 balance_service-0.0.9/src/balance_service/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1433 2023-03-31 20:39:22.000000 balance_service-0.0.9/src/balance_service/interfaces/boto_s3.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1344 2023-03-31 20:39:22.000000 balance_service-0.0.9/src/balance_service/interfaces/nubank.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/balance_service/repositories/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-31 20:39:22.000000 balance_service-0.0.9/src/balance_service/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      323 2023-03-31 20:39:22.000000 balance_service-0.0.9/src/balance_service/repositories/bank.py
+-rw-r--r--   0 runner    (1001) docker     (116)      324 2023-03-31 20:39:22.000000 balance_service-0.0.9/src/balance_service/repositories/user.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/balance_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      499 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/balance_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      518 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/balance_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/balance_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/balance_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2023-03-31 20:39:41.000000 balance_service-0.0.9/src/balance_service.egg-info/top_level.txt
```

### Comparing `balance_service-0.0.8/setup.py` & `balance_service-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `balance_service-0.0.8/src/balance_service/interfaces/boto_s3.py` & `balance_service-0.0.9/src/balance_service/interfaces/boto_s3.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,39 +7,46 @@
         pass
 
     @abstractmethod
     def authenticate(self):
         pass
 
     @abstractmethod
-    def upload_file(self, file_path: str, file_path_new: str):
+    def upload_file(self, bucket_path: str, file_path: str, file_path_new: str):
         pass
 
     @abstractmethod
-    def download_file(self, file_path: str, file_path_new: str):
+    def download_file(self, bucket_path: str, file_path: str, file_path_new: str):
         pass
 
     @abstractmethod
-    def has_file(self, file_path: str) -> bool:
+    def has_file(self, bucket_path: str, file_path: str) -> bool:
         pass
 
 
 class BotoS3:
     def __init__(self, interactor_service):
         self.interactor_service = interactor_service
 
     def upload_file(self,
+                    bucket_path: str,
                     file_path: str,
                     file_path_new: str):
         self.interactor_service.upload_file(
+            bucket_path=bucket_path,
             file_path=file_path,
             file_path_new=file_path_new,)
 
     def download_file(self,
+                      bucket_path: str,
                       file_path: str,
                       file_path_new: str):
         self.interactor_service.download_file(
+            bucket_path=bucket_path,
             file_path=file_path,
             file_path_new=file_path_new,)
 
-    def has_file(self, file_path: str) -> bool:
-        return self.interactor_service.has_file(file_path=file_path)
+    def has_file(self, bucket_path: str, file_path: str) -> bool:
+        return self.interactor_service.has_file(
+            bucket_path=bucket_path,
+            file_path=file_path
+        )
```

### Comparing `balance_service-0.0.8/src/balance_service/interfaces/nubank.py` & `balance_service-0.0.9/src/balance_service/interfaces/nubank.py`

 * *Files identical despite different names*

### Comparing `balance_service-0.0.8/src/balance_service.egg-info/SOURCES.txt` & `balance_service-0.0.9/src/balance_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

