# Comparing `tmp/autouri-0.4.3.tar.gz` & `tmp/autouri-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autouri-0.4.3.tar", last modified: Mon Nov  7 08:01:25 2022, max compression
+gzip compressed data, was "autouri-0.4.4.tar", last modified: Thu May  4 17:34:59 2023, max compression
```

## Comparing `autouri-0.4.3.tar` & `autouri-0.4.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-11-07 08:01:25.072928 autouri-0.4.3/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1067 2022-11-02 23:02:20.000000 autouri-0.4.3/LICENSE
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      521 2022-11-07 08:01:25.072928 autouri-0.4.3/PKG-INFO
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6202 2022-11-02 23:02:20.000000 autouri-0.4.3/README.md
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-11-07 08:01:25.064928 autouri-0.4.3/autouri/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      245 2022-11-07 06:58:55.000000 autouri-0.4.3/autouri/__init__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       61 2022-11-02 23:02:20.000000 autouri-0.4.3/autouri/__main__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     8515 2022-11-06 21:41:48.000000 autouri-0.4.3/autouri/abspath.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    25661 2022-11-06 21:41:48.000000 autouri-0.4.3/autouri/autouri.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     8757 2022-11-02 23:02:20.000000 autouri-0.4.3/autouri/cli.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    18245 2022-11-07 08:00:57.000000 autouri-0.4.3/autouri/gcsuri.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5761 2022-11-06 21:41:48.000000 autouri-0.4.3/autouri/httpurl.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3101 2022-11-03 20:03:29.000000 autouri-0.4.3/autouri/loc_aux.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1380 2022-11-06 21:41:48.000000 autouri-0.4.3/autouri/metadata.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1898 2022-11-02 23:02:20.000000 autouri-0.4.3/autouri/ntp_now.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    10963 2022-11-07 06:58:55.000000 autouri-0.4.3/autouri/s3uri.py
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-11-07 08:01:25.068928 autouri-0.4.3/autouri.egg-info/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      521 2022-11-07 08:01:24.000000 autouri-0.4.3/autouri.egg-info/PKG-INFO
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      660 2022-11-07 08:01:24.000000 autouri-0.4.3/autouri.egg-info/SOURCES.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        1 2022-11-07 08:01:24.000000 autouri-0.4.3/autouri.egg-info/dependency_links.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       99 2022-11-07 08:01:24.000000 autouri-0.4.3/autouri.egg-info/requires.txt
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       14 2022-11-07 08:01:24.000000 autouri-0.4.3/autouri.egg-info/top_level.txt
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-11-07 08:01:25.068928 autouri-0.4.3/bin/
--rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)      297 2022-11-02 23:02:20.000000 autouri-0.4.3/bin/autouri
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       38 2022-11-07 08:01:25.072928 autouri-0.4.3/setup.cfg
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1679 2022-11-06 21:41:48.000000 autouri-0.4.3/setup.py
-drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2022-11-07 08:01:25.072928 autouri-0.4.3/tests/
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        0 2022-11-02 23:02:20.000000 autouri-0.4.3/tests/__init__.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    10463 2022-11-06 21:41:48.000000 autouri-0.4.3/tests/conftest.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7403 2022-11-06 21:41:48.000000 autouri-0.4.3/tests/files.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    18621 2022-11-06 21:41:48.000000 autouri-0.4.3/tests/test_abspath.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2215 2022-11-02 23:02:20.000000 autouri-0.4.3/tests/test_autouri_localize.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3599 2022-11-02 23:02:20.000000 autouri-0.4.3/tests/test_autouri_lock.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    16624 2022-11-06 21:41:48.000000 autouri-0.4.3/tests/test_gcsuri.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    10559 2022-11-06 21:41:48.000000 autouri-0.4.3/tests/test_httpurl.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1204 2022-11-02 23:02:20.000000 autouri-0.4.3/tests/test_metadata.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1005 2022-11-06 21:41:48.000000 autouri-0.4.3/tests/test_ntp_now.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2075 2022-11-07 06:58:55.000000 autouri-0.4.3/tests/test_race_cond.py
--rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    15965 2022-11-06 21:41:48.000000 autouri-0.4.3/tests/test_s3uri.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 17:34:59.246863 autouri-0.4.4/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1067 2022-11-02 23:02:20.000000 autouri-0.4.4/LICENSE
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      521 2023-05-04 17:34:59.246863 autouri-0.4.4/PKG-INFO
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     6202 2022-11-02 23:02:20.000000 autouri-0.4.4/README.md
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 17:34:59.238863 autouri-0.4.4/autouri/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      245 2023-05-04 17:34:41.000000 autouri-0.4.4/autouri/__init__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       61 2022-11-02 23:02:20.000000 autouri-0.4.4/autouri/__main__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     8515 2022-11-06 21:41:48.000000 autouri-0.4.4/autouri/abspath.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    25661 2022-11-06 21:41:48.000000 autouri-0.4.4/autouri/autouri.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     8757 2022-11-02 23:02:20.000000 autouri-0.4.4/autouri/cli.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    18267 2023-05-04 17:34:41.000000 autouri-0.4.4/autouri/gcsuri.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     5761 2022-11-06 21:41:48.000000 autouri-0.4.4/autouri/httpurl.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3101 2022-11-03 20:03:29.000000 autouri-0.4.4/autouri/loc_aux.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1380 2022-11-06 21:41:48.000000 autouri-0.4.4/autouri/metadata.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1898 2022-11-02 23:02:20.000000 autouri-0.4.4/autouri/ntp_now.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    10985 2023-05-04 17:34:41.000000 autouri-0.4.4/autouri/s3uri.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 17:34:59.238863 autouri-0.4.4/autouri.egg-info/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      521 2023-05-04 17:34:58.000000 autouri-0.4.4/autouri.egg-info/PKG-INFO
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      660 2023-05-04 17:34:59.000000 autouri-0.4.4/autouri.egg-info/SOURCES.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        1 2023-05-04 17:34:58.000000 autouri-0.4.4/autouri.egg-info/dependency_links.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)      100 2023-05-04 17:34:58.000000 autouri-0.4.4/autouri.egg-info/requires.txt
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       14 2023-05-04 17:34:58.000000 autouri-0.4.4/autouri.egg-info/top_level.txt
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 17:34:59.238863 autouri-0.4.4/bin/
+-rwxrwxr-x   0 leepc12   (1000) leepc12   (1000)      297 2022-11-02 23:02:20.000000 autouri-0.4.4/bin/autouri
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)       38 2023-05-04 17:34:59.246863 autouri-0.4.4/setup.cfg
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1680 2023-05-04 17:34:41.000000 autouri-0.4.4/setup.py
+drwxrwxr-x   0 leepc12   (1000) leepc12   (1000)        0 2023-05-04 17:34:59.246863 autouri-0.4.4/tests/
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)        0 2022-11-02 23:02:20.000000 autouri-0.4.4/tests/__init__.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    10463 2022-11-06 21:41:48.000000 autouri-0.4.4/tests/conftest.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     7403 2022-11-06 21:41:48.000000 autouri-0.4.4/tests/files.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    18621 2022-11-06 21:41:48.000000 autouri-0.4.4/tests/test_abspath.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2215 2022-11-02 23:02:20.000000 autouri-0.4.4/tests/test_autouri_localize.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     3599 2022-11-02 23:02:20.000000 autouri-0.4.4/tests/test_autouri_lock.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    16624 2022-11-06 21:41:48.000000 autouri-0.4.4/tests/test_gcsuri.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    10559 2022-11-06 21:41:48.000000 autouri-0.4.4/tests/test_httpurl.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1204 2022-11-02 23:02:20.000000 autouri-0.4.4/tests/test_metadata.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     1005 2022-11-06 21:41:48.000000 autouri-0.4.4/tests/test_ntp_now.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)     2075 2022-11-07 06:58:55.000000 autouri-0.4.4/tests/test_race_cond.py
+-rw-rw-r--   0 leepc12   (1000) leepc12   (1000)    15965 2022-11-06 21:41:48.000000 autouri-0.4.4/tests/test_s3uri.py
```

### Comparing `autouri-0.4.3/LICENSE` & `autouri-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/PKG-INFO` & `autouri-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autouri
-Version: 0.4.3
+Version: 0.4.4
 Summary: Automatic localization for various URIs (s3://, gs://, http://, https:// and local path)
 Home-page: https://github.com/ENCODE-DCC/autouri
 Author: Jin wook Lee
 Author-email: leepc12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `autouri-0.4.3/README.md` & `autouri-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/autouri/abspath.py` & `autouri-0.4.4/autouri/abspath.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/autouri/autouri.py` & `autouri-0.4.4/autouri/autouri.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/autouri/cli.py` & `autouri-0.4.4/autouri/cli.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/autouri/gcsuri.py` & `autouri-0.4.4/autouri/gcsuri.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,41 +82,41 @@
         """To use self._poll_interval instead of poll_interval in args."""
         super().acquire(timeout=timeout, poll_interval=self._poll_interval)
 
     def _acquire(self):
         """Unlike GCSURI, this module does not use S3 Object locking.
         This will write id(self) on a .lock file.
         """
-        u = GCSURI(self._lock_file)
+        u = GCSURI(self.lock_file)
         str_id = str(id(self))
         try:
             if (
                 not u.exists
                 or now_utc().timestamp() > u.mtime + GCSURILock.LOCK_FILE_EXPIRATION_SEC
             ):
                 u.write(str_id, no_lock=True)
-                self._lock_file_fd = id(self)
+                self._context.lock_file_fd = id(self)
 
             elif u.read() == str_id:
-                self._lock_file_fd = id(self)
+                self._context.lock_file_fd = id(self)
 
         except Forbidden:
             raise
         except (NotFound, ClientError, ValueError):
             pass
         except TypeError:
             # this happens if file exists and failed to get metadata, so u.mtime is None
             pass
         return None
 
     def _release(self):
-        u = GCSURI(self._lock_file)
+        u = GCSURI(self.lock_file)
         try:
             u.rm(no_lock=True, silent=True)
-            self._lock_file_fd = None
+            self._context.lock_file_fd = None
         except (ClientError, ValueError):
             pass
         return None
 
 
 class GCSURI(URIBase):
     """
```

### Comparing `autouri-0.4.3/autouri/httpurl.py` & `autouri-0.4.4/autouri/httpurl.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/autouri/loc_aux.py` & `autouri-0.4.4/autouri/loc_aux.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/autouri/metadata.py` & `autouri-0.4.4/autouri/metadata.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/autouri/ntp_now.py` & `autouri-0.4.4/autouri/ntp_now.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/autouri/s3uri.py` & `autouri-0.4.4/autouri/s3uri.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,41 +46,41 @@
         """To use self._poll_interval instead of poll_interval in args."""
         super().acquire(timeout=timeout, poll_interval=self._poll_interval)
 
     def _acquire(self):
         """Unlike GCSURI, this module does not use S3 Object locking.
         This will write id(self) on a .lock file.
         """
-        u = S3URI(self._lock_file)
+        u = S3URI(self.lock_file)
         str_id = str(id(self))
         try:
             if (
                 not u.exists
                 or now_utc().timestamp() > u.mtime + S3URILock.LOCK_FILE_EXPIRATION_SEC
             ):
                 u.write(str_id, no_lock=True)
-                self._lock_file_fd = id(self)
+                self._context.lock_file_fd = id(self)
 
             elif u.read() == str_id:
-                self._lock_file_fd = id(self)
+                self._context.lock_file_fd = id(self)
 
         except ClientError as e:
             status = e.response["ResponseMetadata"]["HTTPStatusCode"]
             if status in (403,):
                 raise
         except TypeError:
             # this happens if file exists and failed to get metadata, so u.mtime is None
             pass
         return None
 
     def _release(self):
-        u = S3URI(self._lock_file)
+        u = S3URI(self.lock_file)
         try:
             u.rm(no_lock=True, silent=True)
-            self._lock_file_fd = None
+            self._context.lock_file_fd = None
         except ClientError:
             pass
         return None
 
 
 class S3URI(URIBase):
     """
```

### Comparing `autouri-0.4.3/autouri.egg-info/PKG-INFO` & `autouri-0.4.4/autouri.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autouri
-Version: 0.4.3
+Version: 0.4.4
 Summary: Automatic localization for various URIs (s3://, gs://, http://, https:// and local path)
 Home-page: https://github.com/ENCODE-DCC/autouri
 Author: Jin wook Lee
 Author-email: leepc12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `autouri-0.4.3/autouri.egg-info/SOURCES.txt` & `autouri-0.4.4/autouri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/setup.py` & `autouri-0.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,12 +55,12 @@
     install_requires=[
         "requests",
         "pyopenssl",
         "google-cloud-storage",
         "boto3",
         "awscli",
         "dateparser",
-        "filelock>=3.4.0",
+        "filelock>=3.12.0",
         "six>=1.13.0",
         "ntplib",
     ],
 )
```

### Comparing `autouri-0.4.3/tests/conftest.py` & `autouri-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/files.py` & `autouri-0.4.4/tests/files.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/test_abspath.py` & `autouri-0.4.4/tests/test_abspath.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/test_autouri_localize.py` & `autouri-0.4.4/tests/test_autouri_localize.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/test_autouri_lock.py` & `autouri-0.4.4/tests/test_autouri_lock.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/test_gcsuri.py` & `autouri-0.4.4/tests/test_gcsuri.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/test_httpurl.py` & `autouri-0.4.4/tests/test_httpurl.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/test_metadata.py` & `autouri-0.4.4/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/test_ntp_now.py` & `autouri-0.4.4/tests/test_ntp_now.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/test_race_cond.py` & `autouri-0.4.4/tests/test_race_cond.py`

 * *Files identical despite different names*

### Comparing `autouri-0.4.3/tests/test_s3uri.py` & `autouri-0.4.4/tests/test_s3uri.py`

 * *Files identical despite different names*

