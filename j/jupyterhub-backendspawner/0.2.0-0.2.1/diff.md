# Comparing `tmp/jupyterhub-backendspawner-0.2.0.tar.gz` & `tmp/jupyterhub-backendspawner-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.2.0.tar", last modified: Tue May  2 14:45:54 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.2.1.tar", last modified: Thu May  4 08:33:26 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.2.0.tar` & `jupyterhub-backendspawner-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 14:45:54.753415 jupyterhub-backendspawner-0.2.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.2.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-02 14:45:54.753415 jupyterhub-backendspawner-0.2.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.2.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 14:45:54.753415 jupyterhub-backendspawner-0.2.0/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.2.0/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5149 2023-04-26 14:42:02.000000 jupyterhub-backendspawner-0.2.0/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17332 2023-04-26 11:16:17.000000 jupyterhub-backendspawner-0.2.0/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10295 2023-05-02 14:45:25.000000 jupyterhub-backendspawner-0.2.0/backendspawner/eventspawner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 14:45:54.753415 jupyterhub-backendspawner-0.2.0/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-02 14:45:54.000000 jupyterhub-backendspawner-0.2.0/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-02 14:45:54.000000 jupyterhub-backendspawner-0.2.0/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 14:45:54.000000 jupyterhub-backendspawner-0.2.0/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-02 14:45:54.000000 jupyterhub-backendspawner-0.2.0/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-02 14:45:54.000000 jupyterhub-backendspawner-0.2.0/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-02 14:45:54.753415 jupyterhub-backendspawner-0.2.0/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-02 14:45:35.000000 jupyterhub-backendspawner-0.2.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.2.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.2.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.2.1/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5149 2023-04-26 14:42:02.000000 jupyterhub-backendspawner-0.2.1/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17332 2023-04-26 11:16:17.000000 jupyterhub-backendspawner-0.2.1/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10207 2023-05-04 08:17:31.000000 jupyterhub-backendspawner-0.2.1/backendspawner/eventspawner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-04 08:33:26.000000 jupyterhub-backendspawner-0.2.1/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-04 08:33:26.057644 jupyterhub-backendspawner-0.2.1/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-04 08:17:37.000000 jupyterhub-backendspawner-0.2.1/setup.py
```

### Comparing `jupyterhub-backendspawner-0.2.0/LICENSE` & `jupyterhub-backendspawner-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.0/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.2.1/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.0/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.2.1/backendspawner/backendspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.0/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.2.1/backendspawner/eventspawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,16 +128,15 @@
         event = super().get_ready_event()
         ready_msg = f"Service {self.name} started."
         now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
         url = url_path_join(self.user.url, self.name, "/")
         event[
             "html_message"
         ] = f'<details><summary>{now}: {ready_msg}</summary>You will be redirected to <a href="{url}">{url}</a></details>'
-        if len(self.latest_events) == 0 or not self.latest_events[-1].get("ready"):
-            self.latest_events.append(event)
+        self.latest_events.append(event)
         return event
 
     cancelling_event = Union(
         [Dict(), Callable()],
         default_value={
             "failed": False,
             "ready": False,
```

### Comparing `jupyterhub-backendspawner-0.2.0/setup.py` & `jupyterhub-backendspawner-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.2.0",
+    version="0.2.1",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

