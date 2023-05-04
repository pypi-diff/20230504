# Comparing `tmp/s7r-0.1.8.tar.gz` & `tmp/s7r-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s7r-0.1.8.tar", last modified: Thu May  4 16:16:33 2023, max compression
+gzip compressed data, was "s7r-0.1.9.tar", last modified: Thu May  4 16:18:45 2023, max compression
```

## Comparing `s7r-0.1.8.tar` & `s7r-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:16:33.126406 s7r-0.1.8/
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     5271 2023-05-04 16:16:33.126406 s7r-0.1.8/PKG-INFO
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     4542 2023-05-04 15:57:58.000000 s7r-0.1.8/README.md
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1130 2023-03-27 20:33:38.000000 s7r-0.1.8/pyproject.toml
-drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:16:33.122406 s7r-0.1.8/s7r.egg-info/
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     5271 2023-05-04 16:16:33.000000 s7r-0.1.8/s7r.egg-info/PKG-INFO
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      970 2023-05-04 16:16:33.000000 s7r-0.1.8/s7r.egg-info/SOURCES.txt
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        1 2023-05-04 16:16:33.000000 s7r-0.1.8/s7r.egg-info/dependency_links.txt
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       48 2023-05-04 16:16:33.000000 s7r-0.1.8/s7r.egg-info/entry_points.txt
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      171 2023-05-04 16:16:33.000000 s7r-0.1.8/s7r.egg-info/requires.txt
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       10 2023-05-04 16:16:33.000000 s7r-0.1.8/s7r.egg-info/top_level.txt
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       38 2023-05-04 16:16:33.126406 s7r-0.1.8/setup.cfg
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      947 2023-03-27 20:34:02.000000 s7r-0.1.8/setup.py
-drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:16:33.122406 s7r-0.1.8/sprinkler/
-drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:16:33.122406 s7r-0.1.8/sprinkler/.build/
-drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:16:33.126406 s7r-0.1.8/sprinkler/.build/assets/
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)   183620 2023-03-28 21:32:31.000000 s7r-0.1.8/sprinkler/.build/assets/index-8ee4f58f.js
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)   220138 2023-03-28 21:32:31.000000 s7r-0.1.8/sprinkler/.build/assets/index-dc24b5d6.css
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      470 2023-03-28 21:32:31.000000 s7r-0.1.8/sprinkler/.build/index.html
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       22 2023-05-04 16:16:25.000000 s7r-0.1.8/sprinkler/__init__.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    19365 2023-03-27 16:23:31.000000 s7r-0.1.8/sprinkler/cli.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1330 2023-03-28 18:24:35.000000 s7r-0.1.8/sprinkler/constants.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2117 2023-03-25 00:32:03.000000 s7r-0.1.8/sprinkler/db.py
-drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:16:33.126406 s7r-0.1.8/sprinkler/db_interfaces/
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      398 2023-03-25 21:55:52.000000 s7r-0.1.8/sprinkler/db_interfaces/__init__.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1627 2023-03-24 18:14:39.000000 s7r-0.1.8/sprinkler/db_interfaces/api_keys.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2035 2023-03-25 21:53:44.000000 s7r-0.1.8/sprinkler/db_interfaces/config.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     4734 2023-03-28 21:31:47.000000 s7r-0.1.8/sprinkler/db_interfaces/images.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        0 2023-03-24 17:23:19.000000 s7r-0.1.8/sprinkler/db_interfaces/py.typed
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     3212 2023-03-27 16:56:45.000000 s7r-0.1.8/sprinkler/db_interfaces/secrets.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     8308 2023-03-25 00:32:57.000000 s7r-0.1.8/sprinkler/db_interfaces/task_instances.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2673 2023-03-24 18:16:54.000000 s7r-0.1.8/sprinkler/db_interfaces/users.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1937 2023-03-27 16:42:21.000000 s7r-0.1.8/sprinkler/exceptions.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     5199 2023-03-27 18:40:25.000000 s7r-0.1.8/sprinkler/git.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        0 2023-03-23 14:49:56.000000 s7r-0.1.8/sprinkler/py.typed
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     6201 2023-03-28 17:39:12.000000 s7r-0.1.8/sprinkler/scheduler.py
-drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:16:33.126406 s7r-0.1.8/sprinkler/targets/
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      174 2023-03-24 22:38:46.000000 s7r-0.1.8/sprinkler/targets/__init__.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        0 2023-03-24 18:12:28.000000 s7r-0.1.8/sprinkler/targets/py.typed
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2578 2023-03-24 22:44:19.000000 s7r-0.1.8/sprinkler/targets/sprinkler_config.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2480 2023-03-24 22:41:27.000000 s7r-0.1.8/sprinkler/targets/task.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     9425 2023-03-25 21:04:27.000000 s7r-0.1.8/sprinkler/task_instance.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     4947 2023-03-25 21:05:04.000000 s7r-0.1.8/sprinkler/task_manager.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      279 2023-03-24 22:29:49.000000 s7r-0.1.8/sprinkler/utils.py
--rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    16029 2023-03-28 14:24:34.000000 s7r-0.1.8/sprinkler/webserver.py
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:18:45.982515 s7r-0.1.9/
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     5271 2023-05-04 16:18:45.982515 s7r-0.1.9/PKG-INFO
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     4542 2023-05-04 15:57:58.000000 s7r-0.1.9/README.md
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1130 2023-03-27 20:33:38.000000 s7r-0.1.9/pyproject.toml
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:18:45.982515 s7r-0.1.9/s7r.egg-info/
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     5271 2023-05-04 16:18:45.000000 s7r-0.1.9/s7r.egg-info/PKG-INFO
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      970 2023-05-04 16:18:45.000000 s7r-0.1.9/s7r.egg-info/SOURCES.txt
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        1 2023-05-04 16:18:45.000000 s7r-0.1.9/s7r.egg-info/dependency_links.txt
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       48 2023-05-04 16:18:45.000000 s7r-0.1.9/s7r.egg-info/entry_points.txt
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      171 2023-05-04 16:18:45.000000 s7r-0.1.9/s7r.egg-info/requires.txt
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       10 2023-05-04 16:18:45.000000 s7r-0.1.9/s7r.egg-info/top_level.txt
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       38 2023-05-04 16:18:45.982515 s7r-0.1.9/setup.cfg
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      947 2023-03-27 20:34:02.000000 s7r-0.1.9/setup.py
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:18:45.982515 s7r-0.1.9/sprinkler/
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:18:45.982515 s7r-0.1.9/sprinkler/.build/
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:18:45.982515 s7r-0.1.9/sprinkler/.build/assets/
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)   183620 2023-05-04 16:18:42.000000 s7r-0.1.9/sprinkler/.build/assets/index-8ee4f58f.js
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)   220138 2023-05-04 16:18:42.000000 s7r-0.1.9/sprinkler/.build/assets/index-dc24b5d6.css
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      470 2023-05-04 16:18:42.000000 s7r-0.1.9/sprinkler/.build/index.html
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)       22 2023-05-04 16:18:24.000000 s7r-0.1.9/sprinkler/__init__.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    19365 2023-03-27 16:23:31.000000 s7r-0.1.9/sprinkler/cli.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1330 2023-03-28 18:24:35.000000 s7r-0.1.9/sprinkler/constants.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2117 2023-03-25 00:32:03.000000 s7r-0.1.9/sprinkler/db.py
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:18:45.982515 s7r-0.1.9/sprinkler/db_interfaces/
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      398 2023-03-25 21:55:52.000000 s7r-0.1.9/sprinkler/db_interfaces/__init__.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1627 2023-03-24 18:14:39.000000 s7r-0.1.9/sprinkler/db_interfaces/api_keys.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2035 2023-03-25 21:53:44.000000 s7r-0.1.9/sprinkler/db_interfaces/config.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     4734 2023-03-28 21:31:47.000000 s7r-0.1.9/sprinkler/db_interfaces/images.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        0 2023-03-24 17:23:19.000000 s7r-0.1.9/sprinkler/db_interfaces/py.typed
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     3212 2023-03-27 16:56:45.000000 s7r-0.1.9/sprinkler/db_interfaces/secrets.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     8308 2023-03-25 00:32:57.000000 s7r-0.1.9/sprinkler/db_interfaces/task_instances.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2673 2023-03-24 18:16:54.000000 s7r-0.1.9/sprinkler/db_interfaces/users.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     1937 2023-03-27 16:42:21.000000 s7r-0.1.9/sprinkler/exceptions.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     5199 2023-03-27 18:40:25.000000 s7r-0.1.9/sprinkler/git.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        0 2023-03-23 14:49:56.000000 s7r-0.1.9/sprinkler/py.typed
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     6201 2023-03-28 17:39:12.000000 s7r-0.1.9/sprinkler/scheduler.py
+drwxrwxr-x   0 henryjones  (1000) henryjones  (1000)        0 2023-05-04 16:18:45.982515 s7r-0.1.9/sprinkler/targets/
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      174 2023-03-24 22:38:46.000000 s7r-0.1.9/sprinkler/targets/__init__.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)        0 2023-03-24 18:12:28.000000 s7r-0.1.9/sprinkler/targets/py.typed
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2578 2023-03-24 22:44:19.000000 s7r-0.1.9/sprinkler/targets/sprinkler_config.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     2480 2023-03-24 22:41:27.000000 s7r-0.1.9/sprinkler/targets/task.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     9425 2023-03-25 21:04:27.000000 s7r-0.1.9/sprinkler/task_instance.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)     4947 2023-03-25 21:05:04.000000 s7r-0.1.9/sprinkler/task_manager.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)      279 2023-03-24 22:29:49.000000 s7r-0.1.9/sprinkler/utils.py
+-rw-rw-r--   0 henryjones  (1000) henryjones  (1000)    16029 2023-03-28 14:24:34.000000 s7r-0.1.9/sprinkler/webserver.py
```

### Comparing `s7r-0.1.8/PKG-INFO` & `s7r-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s7r
-Version: 0.1.8
+Version: 0.1.9
 Summary: An easy to use job runner.
 Home-page: https://github.com/henryivesjones/sprinkler
 Author: Henry Jones
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: scheduler,task runner,task,job
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `s7r-0.1.8/README.md` & `s7r-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/pyproject.toml` & `s7r-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/s7r.egg-info/PKG-INFO` & `s7r-0.1.9/s7r.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s7r
-Version: 0.1.8
+Version: 0.1.9
 Summary: An easy to use job runner.
 Home-page: https://github.com/henryivesjones/sprinkler
 Author: Henry Jones
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: scheduler,task runner,task,job
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `s7r-0.1.8/s7r.egg-info/SOURCES.txt` & `s7r-0.1.9/s7r.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/setup.py` & `s7r-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/.build/assets/index-8ee4f58f.js` & `s7r-0.1.9/sprinkler/.build/assets/index-8ee4f58f.js`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/.build/assets/index-dc24b5d6.css` & `s7r-0.1.9/sprinkler/.build/assets/index-dc24b5d6.css`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/cli.py` & `s7r-0.1.9/sprinkler/cli.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/constants.py` & `s7r-0.1.9/sprinkler/constants.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/db.py` & `s7r-0.1.9/sprinkler/db.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/db_interfaces/api_keys.py` & `s7r-0.1.9/sprinkler/db_interfaces/api_keys.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/db_interfaces/config.py` & `s7r-0.1.9/sprinkler/db_interfaces/config.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/db_interfaces/images.py` & `s7r-0.1.9/sprinkler/db_interfaces/images.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/db_interfaces/secrets.py` & `s7r-0.1.9/sprinkler/db_interfaces/secrets.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/db_interfaces/task_instances.py` & `s7r-0.1.9/sprinkler/db_interfaces/task_instances.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/db_interfaces/users.py` & `s7r-0.1.9/sprinkler/db_interfaces/users.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/exceptions.py` & `s7r-0.1.9/sprinkler/exceptions.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/git.py` & `s7r-0.1.9/sprinkler/git.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/scheduler.py` & `s7r-0.1.9/sprinkler/scheduler.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/targets/sprinkler_config.py` & `s7r-0.1.9/sprinkler/targets/sprinkler_config.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/targets/task.py` & `s7r-0.1.9/sprinkler/targets/task.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/task_instance.py` & `s7r-0.1.9/sprinkler/task_instance.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/task_manager.py` & `s7r-0.1.9/sprinkler/task_manager.py`

 * *Files identical despite different names*

### Comparing `s7r-0.1.8/sprinkler/webserver.py` & `s7r-0.1.9/sprinkler/webserver.py`

 * *Files identical despite different names*

