# Comparing `tmp/negotium-0.0.5a2.tar.gz` & `tmp/negotium-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negotium-0.0.5a2.tar", last modified: Thu May  4 10:39:08 2023, max compression
+gzip compressed data, was "negotium-0.1.0.tar", last modified: Thu May  4 11:15:38 2023, max compression
```

## Comparing `negotium-0.0.5a2.tar` & `negotium-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.075025 negotium-0.0.5a2/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.0.5a2/.gitignore
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-04 10:39:08.075025 negotium-0.0.5a2/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.5a2/README.md
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.071024 negotium-0.0.5a2/negotium/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.5a2/negotium/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3466 2023-05-04 10:25:21.000000 negotium-0.0.5a2/negotium/base.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.071024 negotium-0.0.5a2/negotium/mq/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.5a2/negotium/mq/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5450 2023-05-04 10:38:03.000000 negotium-0.0.5a2/negotium/mq/consumer.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.0.5a2/negotium/mq/publisher.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.5a2/negotium/settings.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.5a2/negotium/task.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.075025 negotium-0.0.5a2/negotium/utils/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.5a2/negotium/utils/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.5a2/negotium/utils/logger.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.071024 negotium-0.0.5a2/negotium.egg-info/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/SOURCES.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/dependency_links.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/requires.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-04 10:39:08.000000 negotium-0.0.5a2/negotium.egg-info/top_level.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      407 2023-05-04 10:38:58.000000 negotium-0.0.5a2/pyproject.toml
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.0.5a2/requirements.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-04 10:39:08.075025 negotium-0.0.5a2/setup.cfg
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 10:39:08.075025 negotium-0.0.5a2/tests/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.0.5a2/tests/__init__.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.1.0/.gitignore
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     2463 2023-05-04 11:15:38.324810 negotium-0.1.0/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     2296 2023-05-04 11:09:10.000000 negotium-0.1.0/README.md
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.320809 negotium-0.1.0/negotium/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.1.0/negotium/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3466 2023-05-04 10:25:21.000000 negotium-0.1.0/negotium/base.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/negotium/mq/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.1.0/negotium/mq/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5472 2023-05-04 10:41:07.000000 negotium-0.1.0/negotium/mq/consumer.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.1.0/negotium/mq/publisher.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.1.0/negotium/settings.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.1.0/negotium/task.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/negotium/utils/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.1.0/negotium/utils/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.1.0/negotium/utils/logger.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/negotium.egg-info/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     2463 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/SOURCES.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/dependency_links.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/requires.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/top_level.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      405 2023-05-04 11:15:16.000000 negotium-0.1.0/pyproject.toml
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.1.0/requirements.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-04 11:15:38.324810 negotium-0.1.0/setup.cfg
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/tests/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.1.0/tests/__init__.py
```

### Comparing `negotium-0.0.5a2/negotium/base.py` & `negotium-0.1.0/negotium/base.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.5a2/negotium/mq/consumer.py` & `negotium-0.1.0/negotium/mq/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,16 @@
             f"{'[Scheduled] ' if is_scheduled else ''}Executing (task: {function_name})", level="INFO")
         
         # import
         spec = importlib.util.spec_from_file_location(f"{module_name}.{function_name}", f"{package_dir}/{module_name}.py")
         module = importlib.util.module_from_spec(spec)
         sys.modules[f"{module_name}.{function_name}"] = module
         spec.loader.exec_module(module)
-        # get the function
-        function = getattr(module, function_name)
         # execute the function
+        function = getattr(module, function_name)
         try:
             res = function(*args, **kwargs)
             log(self.logfile, app_name, 
                 f"{'[Scheduled] ' if is_scheduled else ''}Result (task: {function_name}): {res}", level="INFO")
         except Exception as e:
             log(self.logfile, app_name, 
                 f"{'[Scheduled] ' if is_scheduled else ''}Error (task: {function_name}): {e}", level="ERROR")
@@ -128,16 +127,16 @@
         self._process_consume_scheduled.start()
 
         # register a signal handler
         signal.signal(signal.SIGINT, self._signal_handler)
         signal.signal(signal.SIGTERM, self._signal_handler)
 
         # wait for both processes to finish
-        # p.join()
-        # p2.join()
+        # self._process_consume.join()
+        # self._process_consume_scheduled.join()
 
     def _signal_handler(self, sig, frame):
         """Handle signals
         """
         # close the connection
         self.close()
         # exit
```

### Comparing `negotium-0.0.5a2/negotium/mq/publisher.py` & `negotium-0.1.0/negotium/mq/publisher.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.5a2/negotium/utils/logger.py` & `negotium-0.1.0/negotium/utils/logger.py`

 * *Files identical despite different names*

