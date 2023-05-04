# Comparing `tmp/androidtvremote2-0.0.7.tar.gz` & `tmp/androidtvremote2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androidtvremote2-0.0.7.tar", last modified: Sat Apr  8 05:09:10 2023, max compression
+gzip compressed data, was "androidtvremote2-0.0.8.tar", last modified: Thu May  4 11:44:10 2023, max compression
```

## Comparing `androidtvremote2-0.0.7.tar` & `androidtvremote2-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 05:09:10.742411 androidtvremote2-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-08 05:09:10.742411 androidtvremote2-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-08 05:09:10.742411 androidtvremote2-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 05:09:10.738412 androidtvremote2-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 05:09:10.742411 androidtvremote2-0.0.7/src/androidtvremote2/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/androidtv_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/certificate_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/polo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    19528 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/androidtvremote2/remotemessage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 05:09:10.742411 androidtvremote2-0.0.7/src/androidtvremote2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-08 05:09:10.000000 androidtvremote2-0.0.7/src/androidtvremote2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-08 05:09:10.000000 androidtvremote2-0.0.7/src/androidtvremote2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 05:09:10.000000 androidtvremote2-0.0.7/src/androidtvremote2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-08 05:09:10.000000 androidtvremote2-0.0.7/src/androidtvremote2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 05:09:10.000000 androidtvremote2-0.0.7/src/androidtvremote2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/src/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 05:09:10.742411 androidtvremote2-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-08 05:08:57.000000 androidtvremote2-0.0.7/tests/test_androidtv_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.218464 androidtvremote2-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/src/androidtvremote2/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15577 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/androidtv_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/certificate_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/polo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19528 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/androidtvremote2/remotemessage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 11:44:10.000000 androidtvremote2-0.0.8/src/androidtvremote2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/src/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:10.222464 androidtvremote2-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 11:43:58.000000 androidtvremote2-0.0.8/tests/test_androidtv_remote.py
```

### Comparing `androidtvremote2-0.0.7/LICENSE` & `androidtvremote2-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.7/PKG-INFO` & `androidtvremote2-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androidtvremote2
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for interacting with Android TV using the Android TV Remote protocol v2
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/androidtvremote2
 Project-URL: Bug Tracker, https://github.com/tronikos/androidtvremote2/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `androidtvremote2-0.0.7/README.md` & `androidtvremote2-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.7/pyproject.toml` & `androidtvremote2-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "androidtvremote2"
-version = "0.0.7"
+version = "0.0.8"
 license = {text = "Apache-2.0"}
 authors = [
     { name="tronikos", email="tronikos@gmail.com" },
 ]
 description = "A Python library for interacting with Android TV using the Android TV Remote protocol v2"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `androidtvremote2-0.0.7/src/androidtvremote2/androidtv_remote.py` & `androidtvremote2-0.0.8/src/androidtvremote2/androidtv_remote.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,26 +106,54 @@
             return None
         return self._remote_message_protocol.volume_info
 
     def add_is_on_updated_callback(self, callback: Callable) -> None:
         """Add a callback for when is_on is updated."""
         self._is_on_updated_callbacks.append(callback)
 
+    def remove_is_on_updated_callback(self, callback: Callable) -> None:
+        """Remove a callback previously added via add_is_on_updated_callback.
+
+        :raises ValueError: if callback not previously added.
+        """
+        self._is_on_updated_callbacks.remove(callback)
+
     def add_current_app_updated_callback(self, callback: Callable) -> None:
         """Add a callback for when current_app is updated."""
         self._current_app_updated_callbacks.append(callback)
 
+    def remove_current_app_updated_callback(self, callback: Callable) -> None:
+        """Remove a callback previously added via add_current_app_updated_callback.
+
+        :raises ValueError: if callback not previously added.
+        """
+        self._current_app_updated_callbacks.remove(callback)
+
     def add_volume_info_updated_callback(self, callback: Callable) -> None:
         """Add a callback for when volume_info is updated."""
         self._volume_info_updated_callbacks.append(callback)
 
+    def remove_volume_info_updated_callback(self, callback: Callable) -> None:
+        """Remove a callback previously added via add_volume_info_updated_callback.
+
+        :raises ValueError: if callback not previously added.
+        """
+        self._volume_info_updated_callbacks.remove(callback)
+
     def add_is_available_updated_callback(self, callback: Callable) -> None:
         """Add a callback for when the Android TV is ready to receive commands or is unavailable."""
         self._is_available_updated_callbacks.append(callback)
 
+    def remove_is_available_updated_callback(self, callback: Callable) -> None:
+        """Remove a callback previously added via add_is_available_updated_callback.
+
+        :raises ValueError: if callback not previously added.
+        """
+        self._is_available_updated_callbacks.remove(callback)
+
     async def async_generate_cert_if_missing(self) -> bool:
         """Generate client certificate and public key if missing.
 
         :returns: True if a new certificate was generated.
         """
         if os.path.isfile(self._certfile) and os.path.isfile(self._keyfile):
             return False
```

### Comparing `androidtvremote2-0.0.7/src/androidtvremote2/base.py` & `androidtvremote2-0.0.8/src/androidtvremote2/base.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.7/src/androidtvremote2/certificate_generator.py` & `androidtvremote2-0.0.8/src/androidtvremote2/certificate_generator.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.7/src/androidtvremote2/pairing.py` & `androidtvremote2-0.0.8/src/androidtvremote2/pairing.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.7/src/androidtvremote2/polo_pb2.py` & `androidtvremote2-0.0.8/src/androidtvremote2/polo_pb2.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.7/src/androidtvremote2/remote.py` & `androidtvremote2-0.0.8/src/androidtvremote2/remote.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.7/src/androidtvremote2/remotemessage_pb2.py` & `androidtvremote2-0.0.8/src/androidtvremote2/remotemessage_pb2.py`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.7/src/androidtvremote2.egg-info/PKG-INFO` & `androidtvremote2-0.0.8/src/androidtvremote2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: androidtvremote2
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for interacting with Android TV using the Android TV Remote protocol v2
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/androidtvremote2
 Project-URL: Bug Tracker, https://github.com/tronikos/androidtvremote2/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `androidtvremote2-0.0.7/src/androidtvremote2.egg-info/SOURCES.txt` & `androidtvremote2-0.0.8/src/androidtvremote2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.7/src/demo.py` & `androidtvremote2-0.0.8/src/demo.py`

 * *Files identical despite different names*

