# Comparing `tmp/jupyterhub-backendspawner-0.2.1.tar.gz` & `tmp/jupyterhub-backendspawner-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.2.1.tar", last modified: Thu May  4 08:33:26 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.2.2.tar", last modified: Thu May  4 09:42:16 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.2.1.tar` & `jupyterhub-backendspawner-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.2.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.2.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.2.1/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5149 2023-04-26 14:42:02.000000 jupyterhub-backendspawner-0.2.1/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17332 2023-04-26 11:16:17.000000 jupyterhub-backendspawner-0.2.1/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10207 2023-05-04 08:17:31.000000 jupyterhub-backendspawner-0.2.1/backendspawner/eventspawner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-04 08:17:37.000000 jupyterhub-backendspawner-0.2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 09:42:16.466320 jupyterhub-backendspawner-0.2.2/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.2.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 09:42:16.466320 jupyterhub-backendspawner-0.2.2/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.2.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 09:42:16.466320 jupyterhub-backendspawner-0.2.2/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.2.2/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5149 2023-04-26 14:42:02.000000 jupyterhub-backendspawner-0.2.2/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17735 2023-05-04 09:41:27.000000 jupyterhub-backendspawner-0.2.2/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10207 2023-05-04 08:17:31.000000 jupyterhub-backendspawner-0.2.2/backendspawner/eventspawner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 09:42:16.466320 jupyterhub-backendspawner-0.2.2/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 09:42:16.000000 jupyterhub-backendspawner-0.2.2/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-04 09:42:16.000000 jupyterhub-backendspawner-0.2.2/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-04 09:42:16.000000 jupyterhub-backendspawner-0.2.2/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-04 09:42:16.000000 jupyterhub-backendspawner-0.2.2/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-04 09:42:16.000000 jupyterhub-backendspawner-0.2.2/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-04 09:42:16.466320 jupyterhub-backendspawner-0.2.2/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-04 09:42:04.000000 jupyterhub-backendspawner-0.2.2/setup.py
```

### Comparing `jupyterhub-backendspawner-0.2.1/LICENSE` & `jupyterhub-backendspawner-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.1/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.2.2/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.1/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.2.2/backendspawner/backendspawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,14 +475,24 @@
             # We've already sent a request to the backend.
             # There's no need to do it again.
             return
 
         # Prevent multiple requests to the backend
         self.already_stopped = True
 
+        # if Spawner.stop was called by a custom APIHandler, we have to
+        # set these variables here. If it's called via user.stop() stop_pending
+        # is already true
+        if not self.stop_pending:
+            self._spawn_pending = False
+            self._start_pending = False
+            self._check_pending = False
+            self.stop_polling()
+            self._stop_pending = True
+
         url = await self.get_request_url_stop()
         headers = await self.get_request_headers_stop()
         req = HTTPRequest(
             url=url,
             method="DELETE",
             headers=headers,
             **self.get_request_kwargs(),
```

### Comparing `jupyterhub-backendspawner-0.2.1/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.2.2/backendspawner/eventspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.1/setup.py` & `jupyterhub-backendspawner-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.2.1",
+    version="0.2.2",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

