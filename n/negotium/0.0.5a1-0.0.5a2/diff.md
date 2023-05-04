# Comparing `tmp/negotium-0.0.5a1.tar.gz` & `tmp/negotium-0.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negotium-0.0.5a1.tar", last modified: Thu May  4 10:26:52 2023, max compression
+gzip compressed data, was "negotium-0.0.5a2.tar", last modified: Thu May  4 10:39:08 2023, max compression
```

## Comparing `negotium-0.0.5a1.tar` & `negotium-0.0.5a2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.0.5a1/.gitignore
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-04 10:26:52.763393 negotium-0.0.5a1/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.5a1/README.md
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.759392 negotium-0.0.5a1/negotium/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.5a1/negotium/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3466 2023-05-04 10:25:21.000000 negotium-0.0.5a1/negotium/base.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/negotium/mq/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.5a1/negotium/mq/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5256 2023-05-04 10:24:48.000000 negotium-0.0.5a1/negotium/mq/consumer.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.0.5a1/negotium/mq/publisher.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.5a1/negotium/settings.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.5a1/negotium/task.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/negotium/utils/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.5a1/negotium/utils/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.5a1/negotium/utils/logger.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/negotium.egg-info/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/SOURCES.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/dependency_links.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/requires.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-04 10:26:52.000000 negotium-0.0.5a1/negotium.egg-info/top_level.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      407 2023-05-04 10:26:23.000000 negotium-0.0.5a1/pyproject.toml
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.0.5a1/requirements.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-04 10:26:52.763393 negotium-0.0.5a1/setup.cfg
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:26:52.763393 negotium-0.0.5a1/tests/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.0.5a1/tests/__init__.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.075025 negotium-0.0.5a2/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.0.5a2/.gitignore
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-04 10:39:08.075025 negotium-0.0.5a2/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.5a2/README.md
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.071024 negotium-0.0.5a2/negotium/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.5a2/negotium/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3466 2023-05-04 10:25:21.000000 negotium-0.0.5a2/negotium/base.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.071024 negotium-0.0.5a2/negotium/mq/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.5a2/negotium/mq/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5450 2023-05-04 10:38:03.000000 negotium-0.0.5a2/negotium/mq/consumer.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.0.5a2/negotium/mq/publisher.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.5a2/negotium/settings.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.5a2/negotium/task.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.075025 negotium-0.0.5a2/negotium/utils/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.5a2/negotium/utils/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.5a2/negotium/utils/logger.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.071024 negotium-0.0.5a2/negotium.egg-info/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/SOURCES.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/dependency_links.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/requires.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/top_level.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      407 2023-05-04 10:38:58.000000 negotium-0.0.5a2/pyproject.toml
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.0.5a2/requirements.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-04 10:39:08.075025 negotium-0.0.5a2/setup.cfg
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.075025 negotium-0.0.5a2/tests/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.0.5a2/tests/__init__.py
```

### Comparing `negotium-0.0.5a1/PKG-INFO` & `negotium-0.0.5a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

### Comparing `negotium-0.0.5a1/README.md` & `negotium-0.0.5a2/README.md`

 * *Files identical despite different names*

### Comparing `negotium-0.0.5a1/negotium/base.py` & `negotium-0.0.5a2/negotium/base.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.5a1/negotium/mq/consumer.py` & `negotium-0.0.5a2/negotium/mq/consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,15 +98,18 @@
         args = body.get('args', [])
         kwargs = body.get('kwargs', {})
         is_scheduled = body.get('_is_scheduled')
         log(self.logfile, app_name, 
             f"{'[Scheduled] ' if is_scheduled else ''}Executing (task: {function_name})", level="INFO")
         
         # import
-        module = importlib.import_module(f"{package_name}.{module_name}", package_dir)
+        spec = importlib.util.spec_from_file_location(f"{module_name}.{function_name}", f"{package_dir}/{module_name}.py")
+        module = importlib.util.module_from_spec(spec)
+        sys.modules[f"{module_name}.{function_name}"] = module
+        spec.loader.exec_module(module)
         # get the function
         function = getattr(module, function_name)
         # execute the function
         try:
             res = function(*args, **kwargs)
             log(self.logfile, app_name, 
                 f"{'[Scheduled] ' if is_scheduled else ''}Result (task: {function_name}): {res}", level="INFO")
```

### Comparing `negotium-0.0.5a1/negotium/mq/publisher.py` & `negotium-0.0.5a2/negotium/mq/publisher.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.5a1/negotium/utils/logger.py` & `negotium-0.0.5a2/negotium/utils/logger.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.5a1/negotium.egg-info/PKG-INFO` & `negotium-0.0.5a2/negotium.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

