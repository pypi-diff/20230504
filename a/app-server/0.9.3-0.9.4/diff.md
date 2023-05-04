# Comparing `tmp/app_server-0.9.3.tar.gz` & `tmp/app_server-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_server-0.9.3.tar", last modified: Mon Mar 27 06:15:48 2023, max compression
+gzip compressed data, was "app_server-0.9.4.tar", last modified: Thu May  4 17:19:16 2023, max compression
```

## Comparing `app_server-0.9.3.tar` & `app_server-0.9.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:48.287639 app_server-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-27 06:15:36.000000 app_server-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-27 06:15:48.287639 app_server-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-27 06:15:36.000000 app_server-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-27 06:15:36.000000 app_server-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-27 06:15:48.287639 app_server-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 06:15:36.000000 app_server-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:48.283639 app_server-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:48.283639 app_server-0.9.3/src/app_server/
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:48.287639 app_server-0.9.3/src/app_server/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/storage/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:48.287639 app_server-0.9.3/src/app_server/storage/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/storage/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/storage/handlers/buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/storage/handlers/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/storage/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/storage/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:48.287639 app_server-0.9.3/src/app_server/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:48.287639 app_server-0.9.3/src/app_server/tasks/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/tasks/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63475 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/tasks/proto/cloudtasks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22213 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/tasks/proto/cloudtasks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32068 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/tasks/proto/queue_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    44125 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/tasks/proto/target_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/tasks/proto/task_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-03-27 06:15:36.000000 app_server-0.9.3/src/app_server/tasks/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:15:48.287639 app_server-0.9.3/src/app_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-27 06:15:48.000000 app_server-0.9.3/src/app_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-27 06:15:48.000000 app_server-0.9.3/src/app_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 06:15:48.000000 app_server-0.9.3/src/app_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-27 06:15:48.000000 app_server-0.9.3/src/app_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-27 06:15:48.000000 app_server-0.9.3/src/app_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 06:15:48.000000 app_server-0.9.3/src/app_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:16.077487 app_server-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 17:19:05.000000 app_server-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-04 17:19:16.077487 app_server-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-04 17:19:05.000000 app_server-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 17:19:05.000000 app_server-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-04 17:19:16.081487 app_server-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 17:19:05.000000 app_server-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:16.073487 app_server-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:16.073487 app_server-0.9.4/src/app_server/
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:16.077487 app_server-0.9.4/src/app_server/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/storage/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:16.077487 app_server-0.9.4/src/app_server/storage/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/storage/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/storage/handlers/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/storage/handlers/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/storage/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/storage/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:16.077487 app_server-0.9.4/src/app_server/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:16.077487 app_server-0.9.4/src/app_server/tasks/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/tasks/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63475 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/tasks/proto/cloudtasks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22213 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/tasks/proto/cloudtasks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32068 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/tasks/proto/queue_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44125 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/tasks/proto/target_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/tasks/proto/task_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-05-04 17:19:05.000000 app_server-0.9.4/src/app_server/tasks/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:19:16.073487 app_server-0.9.4/src/app_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-04 17:19:16.000000 app_server-0.9.4/src/app_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-04 17:19:16.000000 app_server-0.9.4/src/app_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:19:16.000000 app_server-0.9.4/src/app_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 17:19:16.000000 app_server-0.9.4/src/app_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 17:19:16.000000 app_server-0.9.4/src/app_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 17:19:16.000000 app_server-0.9.4/src/app_server.egg-info/top_level.txt
```

### Comparing `app_server-0.9.3/LICENSE` & `app_server-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/PKG-INFO` & `app_server-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app_server
-Version: 0.9.3
+Version: 0.9.4
 Summary: a lightweight web application launcher for gunicorn and static files.
 Home-page: https://github.com/XeoN-GHMB/app_server
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/XeoN-GHMB/app_server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `app_server-0.9.3/README.md` & `app_server-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/setup.cfg` & `app_server-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/__init__.py` & `app_server-0.9.4/src/app_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from werkzeug.utils import get_content_type
 from werkzeug.http import http_date, is_resource_modified
 from werkzeug._internal import _logger
 from werkzeug.urls import uri_to_iri, url_unquote
 
 
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 subprocesses = []
 
 class myWSGIRequestHandler(WSGIRequestHandler):
     def log_date_time_string(self):
         """Return the current time formatted for logging."""
         now = time.time()
@@ -99,15 +99,15 @@
             return opts
 
         self.targets = {
             f"{k}": _set_defaults(v) for k, v in targets.items()
         }
 
     def __call__(self, environ: "WSGIEnvironment", start_response: "StartResponse") -> t.Iterable[bytes]:
-        path = url_unquote(environ["PATH_INFO"])
+        path = get_path_info(environ, charset='utf-8', errors='replace')
         app = self.app
         for prefix, opts in self.targets.items():
             if path.startswith(prefix):
                 app = self.proxy_to(opts, path, prefix)
                 break
 
         return app(environ, start_response)
```

### Comparing `app_server-0.9.3/src/app_server/storage/__init__.py` & `app_server-0.9.4/src/app_server/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/storage/handlers/buckets.py` & `app_server-0.9.4/src/app_server/storage/handlers/buckets.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/storage/handlers/objects.py` & `app_server-0.9.4/src/app_server/storage/handlers/objects.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/storage/server.py` & `app_server-0.9.4/src/app_server/storage/server.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/storage/storage.py` & `app_server-0.9.4/src/app_server/storage/storage.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/tasks/__init__.py` & `app_server-0.9.4/src/app_server/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/tasks/proto/cloudtasks_pb2.py` & `app_server-0.9.4/src/app_server/tasks/proto/cloudtasks_pb2.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/tasks/proto/cloudtasks_pb2_grpc.py` & `app_server-0.9.4/src/app_server/tasks/proto/cloudtasks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/tasks/proto/queue_pb2.py` & `app_server-0.9.4/src/app_server/tasks/proto/queue_pb2.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/tasks/proto/target_pb2.py` & `app_server-0.9.4/src/app_server/tasks/proto/target_pb2.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/tasks/proto/task_pb2.py` & `app_server-0.9.4/src/app_server/tasks/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server/tasks/server.py` & `app_server-0.9.4/src/app_server/tasks/server.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.3/src/app_server.egg-info/PKG-INFO` & `app_server-0.9.4/src/app_server.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-server
-Version: 0.9.3
+Version: 0.9.4
 Summary: a lightweight web application launcher for gunicorn and static files.
 Home-page: https://github.com/XeoN-GHMB/app_server
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/XeoN-GHMB/app_server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `app_server-0.9.3/src/app_server.egg-info/SOURCES.txt` & `app_server-0.9.4/src/app_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

