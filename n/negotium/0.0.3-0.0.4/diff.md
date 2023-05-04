# Comparing `tmp/negotium-0.0.3.tar.gz` & `tmp/negotium-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negotium-0.0.3.tar", last modified: Wed May  3 21:54:21 2023, max compression
+gzip compressed data, was "negotium-0.0.4.tar", last modified: Thu May  4 07:51:50 2023, max compression
```

## Comparing `negotium-0.0.3.tar` & `negotium-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.0.3/.gitignore
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-03 21:54:21.601055 negotium-0.0.3/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.3/README.md
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.597054 negotium-0.0.3/negotium/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.3/negotium/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3314 2023-05-03 21:11:57.000000 negotium-0.0.3/negotium/base.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/negotium/mq/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.3/negotium/mq/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5197 2023-05-03 21:51:34.000000 negotium-0.0.3/negotium/mq/consumer.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.0.3/negotium/mq/publisher.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.3/negotium/settings.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.3/negotium/task.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/negotium/utils/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.3/negotium/utils/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.3/negotium/utils/logger.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/negotium.egg-info/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/SOURCES.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/dependency_links.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/requires.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/top_level.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      405 2023-05-03 21:54:08.000000 negotium-0.0.3/pyproject.toml
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.0.3/requirements.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-03 21:54:21.601055 negotium-0.0.3/setup.cfg
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/tests/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.0.3/tests/__init__.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.743941 negotium-0.0.4/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.0.4/.gitignore
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-04 07:51:50.743941 negotium-0.0.4/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.4/README.md
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.739939 negotium-0.0.4/negotium/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.4/negotium/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3314 2023-05-03 21:11:57.000000 negotium-0.0.4/negotium/base.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.739939 negotium-0.0.4/negotium/mq/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.4/negotium/mq/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5430 2023-05-04 07:50:30.000000 negotium-0.0.4/negotium/mq/consumer.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.0.4/negotium/mq/publisher.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.4/negotium/settings.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.4/negotium/task.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.743941 negotium-0.0.4/negotium/utils/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.4/negotium/utils/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.4/negotium/utils/logger.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.739939 negotium-0.0.4/negotium.egg-info/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/SOURCES.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/dependency_links.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/requires.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-04 07:51:50.000000 negotium-0.0.4/negotium.egg-info/top_level.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      405 2023-05-04 07:51:38.000000 negotium-0.0.4/pyproject.toml
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.0.4/requirements.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-04 07:51:50.743941 negotium-0.0.4/setup.cfg
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 07:51:50.743941 negotium-0.0.4/tests/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.0.4/tests/__init__.py
```

### Comparing `negotium-0.0.3/PKG-INFO` & `negotium-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.3
+Version: 0.0.4
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

### Comparing `negotium-0.0.3/README.md` & `negotium-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `negotium-0.0.3/negotium/base.py` & `negotium-0.0.4/negotium/base.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.3/negotium/mq/consumer.py` & `negotium-0.0.4/negotium/mq/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,20 @@
         is_scheduled = body.get('_is_scheduled')
         log(self.logfile, app_name, 
             f"{'[Scheduled] ' if is_scheduled else ''}Executing (task: {function_name})", level="INFO")
         
         # import the module
         module = importlib.import_module(f"{package_name}.{module_name}")
         # get the function
-        function = getattr(module, function_name)
+        try:
+            function = getattr(module, function_name)
+        except AttributeError:
+            log(self.logfile, app_name, 
+                f"{'[Scheduled] ' if is_scheduled else ''}Error (task: {function_name}): Function not found", level="ERROR")
+            return
         # execute the function
         try:
             res = function(*args, **kwargs)
             log(self.logfile, app_name, 
                 f"{'[Scheduled] ' if is_scheduled else ''}Result (task: {function_name}): {res}", level="INFO")
         except Exception as e:
             log(self.logfile, app_name,
```

### Comparing `negotium-0.0.3/negotium/mq/publisher.py` & `negotium-0.0.4/negotium/mq/publisher.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.3/negotium/utils/logger.py` & `negotium-0.0.4/negotium/utils/logger.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.3/negotium.egg-info/PKG-INFO` & `negotium-0.0.4/negotium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.3
+Version: 0.0.4
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

