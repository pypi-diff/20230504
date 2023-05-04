# Comparing `tmp/negotium-0.0.4.tar.gz` & `tmp/negotium-0.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negotium-0.0.4.tar", last modified: Thu May  4 07:51:50 2023, max compression
+gzip compressed data, was "negotium-0.0.5a1.tar", last modified: Thu May  4 10:26:52 2023, max compression
```

## Comparing `negotium-0.0.4.tar` & `negotium-0.0.5a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.743941 negotium-0.0.4/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.0.4/.gitignore
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-04 07:51:50.743941 negotium-0.0.4/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.4/README.md
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.739939 negotium-0.0.4/negotium/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.4/negotium/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3314 2023-05-03 21:11:57.000000 negotium-0.0.4/negotium/base.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.739939 negotium-0.0.4/negotium/mq/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.4/negotium/mq/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5430 2023-05-04 07:50:30.000000 negotium-0.0.4/negotium/mq/consumer.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.0.4/negotium/mq/publisher.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.4/negotium/settings.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.4/negotium/task.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.743941 negotium-0.0.4/negotium/utils/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.4/negotium/utils/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.4/negotium/utils/logger.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.739939 negotium-0.0.4/negotium.egg-info/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/SOURCES.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/dependency_links.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/requires.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/top_level.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      405 2023-05-04 07:51:38.000000 negotium-0.0.4/pyproject.toml
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.0.4/requirements.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-04 07:51:50.743941 negotium-0.0.4/setup.cfg
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.743941 negotium-0.0.4/tests/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.0.4/tests/__init__.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.0.5a1/.gitignore
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-04 10:26:52.763393 negotium-0.0.5a1/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.5a1/README.md
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.759392 negotium-0.0.5a1/negotium/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.5a1/negotium/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3466 2023-05-04 10:25:21.000000 negotium-0.0.5a1/negotium/base.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/negotium/mq/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.5a1/negotium/mq/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5256 2023-05-04 10:24:48.000000 negotium-0.0.5a1/negotium/mq/consumer.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.0.5a1/negotium/mq/publisher.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.5a1/negotium/settings.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.5a1/negotium/task.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/negotium/utils/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.5a1/negotium/utils/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.5a1/negotium/utils/logger.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/negotium.egg-info/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/SOURCES.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/dependency_links.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/requires.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/top_level.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      407 2023-05-04 10:26:23.000000 negotium-0.0.5a1/pyproject.toml
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.0.5a1/requirements.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-04 10:26:52.763393 negotium-0.0.5a1/setup.cfg
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/tests/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.0.5a1/tests/__init__.py
```

### Comparing `negotium-0.0.4/PKG-INFO` & `negotium-0.0.5a1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.4
+Version: 0.0.5a1
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

### Comparing `negotium-0.0.4/README.md` & `negotium-0.0.5a1/README.md`

 * *Files identical despite different names*

### Comparing `negotium-0.0.4/negotium/base.py` & `negotium-0.0.5a1/negotium/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,23 +74,25 @@
         """
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         wrapper.delay = lambda *args, **kwargs: _delay(self.publisher, {
             'app_name': self.app_name,
+            'package_dir': '/'.join(inspect.getfile(func).split('/')[:-1]),
             'package_name': inspect.getfile(func).split('/')[-2],
             'module_name': inspect.getmodulename(inspect.getfile(func)),
             'function_name': func.__name__,
             'args': args,
             'kwargs': kwargs,
             'timestamp': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         })
         wrapper.apply_async = lambda eta, args: _apply_async(self.publisher, {
             'app_name': self.app_name,
+            'package_dir': '/'.join(inspect.getfile(func).split('/')[:-1]),
             'package_name': inspect.getfile(func).split('/')[-2],
             'module_name': inspect.getmodulename(inspect.getfile(func)),
             'function_name': func.__name__,
             'args': args,
             'timestamp': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         }, eta)
         return wrapper
```

### Comparing `negotium-0.0.4/negotium/mq/consumer.py` & `negotium-0.0.5a1/negotium/mq/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import redis
 import inspect
 import importlib
 import json
 import os
 import signal
+import sys
 import time
 from multiprocessing import Process
 
 from negotium.settings import DEFAULT_QUEUE, DEFAULT_SCHEDULER_QUEUE, DEFAULT_SCHEDULER_SORTED_SET
 from negotium.utils.logger import log
 
 
@@ -86,32 +87,28 @@
         """
         # log the message
         # extract dict from bytes
         body = json.loads(body)
 
         # get function arguments
         app_name = body.get('app_name')
+        package_dir = body.get('package_dir')
         package_name = body.get('package_name')
         module_name = body.get('module_name')
         function_name = body.get('function_name')
         args = body.get('args', [])
         kwargs = body.get('kwargs', {})
         is_scheduled = body.get('_is_scheduled')
         log(self.logfile, app_name, 
             f"{'[Scheduled] ' if is_scheduled else ''}Executing (task: {function_name})", level="INFO")
         
-        # import the module
-        module = importlib.import_module(f"{package_name}.{module_name}")
+        # import
+        module = importlib.import_module(f"{package_name}.{module_name}", package_dir)
         # get the function
-        try:
-            function = getattr(module, function_name)
-        except AttributeError:
-            log(self.logfile, app_name, 
-                f"{'[Scheduled] ' if is_scheduled else ''}Error (task: {function_name}): Function not found", level="ERROR")
-            return
+        function = getattr(module, function_name)
         # execute the function
         try:
             res = function(*args, **kwargs)
             log(self.logfile, app_name, 
                 f"{'[Scheduled] ' if is_scheduled else ''}Result (task: {function_name}): {res}", level="INFO")
         except Exception as e:
             log(self.logfile, app_name,
```

### Comparing `negotium-0.0.4/negotium/mq/publisher.py` & `negotium-0.0.5a1/negotium/mq/publisher.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.4/negotium/utils/logger.py` & `negotium-0.0.5a1/negotium/utils/logger.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.4/negotium.egg-info/PKG-INFO` & `negotium-0.0.5a1/negotium.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.4
+Version: 0.0.5a1
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

