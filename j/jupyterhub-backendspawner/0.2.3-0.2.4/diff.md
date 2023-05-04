# Comparing `tmp/jupyterhub-backendspawner-0.2.3.tar.gz` & `tmp/jupyterhub-backendspawner-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.2.3.tar", last modified: Thu May  4 10:39:30 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.2.4.tar", last modified: Thu May  4 13:53:38 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.2.3.tar` & `jupyterhub-backendspawner-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:39:30.865236 jupyterhub-backendspawner-0.2.3/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.2.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 10:39:30.865236 jupyterhub-backendspawner-0.2.3/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.2.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:39:30.865236 jupyterhub-backendspawner-0.2.3/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.2.3/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5149 2023-04-26 14:42:02.000000 jupyterhub-backendspawner-0.2.3/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17736 2023-05-04 10:38:58.000000 jupyterhub-backendspawner-0.2.3/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10207 2023-05-04 08:17:31.000000 jupyterhub-backendspawner-0.2.3/backendspawner/eventspawner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:39:30.865236 jupyterhub-backendspawner-0.2.3/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 10:39:30.000000 jupyterhub-backendspawner-0.2.3/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-04 10:39:30.000000 jupyterhub-backendspawner-0.2.3/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-04 10:39:30.000000 jupyterhub-backendspawner-0.2.3/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-04 10:39:30.000000 jupyterhub-backendspawner-0.2.3/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-04 10:39:30.000000 jupyterhub-backendspawner-0.2.3/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-04 10:39:30.865236 jupyterhub-backendspawner-0.2.3/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-04 10:39:16.000000 jupyterhub-backendspawner-0.2.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 13:53:38.961510 jupyterhub-backendspawner-0.2.4/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.2.4/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 13:53:38.961510 jupyterhub-backendspawner-0.2.4/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.2.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 13:53:38.961510 jupyterhub-backendspawner-0.2.4/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.2.4/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.2.4/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17332 2023-05-04 13:52:37.000000 jupyterhub-backendspawner-0.2.4/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10525 2023-05-04 13:52:29.000000 jupyterhub-backendspawner-0.2.4/backendspawner/eventspawner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 13:53:38.961510 jupyterhub-backendspawner-0.2.4/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-04 13:53:38.000000 jupyterhub-backendspawner-0.2.4/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-04 13:53:38.000000 jupyterhub-backendspawner-0.2.4/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-04 13:53:38.000000 jupyterhub-backendspawner-0.2.4/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-04 13:53:38.000000 jupyterhub-backendspawner-0.2.4/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-04 13:53:38.000000 jupyterhub-backendspawner-0.2.4/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-04 13:53:38.961510 jupyterhub-backendspawner-0.2.4/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-04 13:53:19.000000 jupyterhub-backendspawner-0.2.4/setup.py
```

### Comparing `jupyterhub-backendspawner-0.2.3/LICENSE` & `jupyterhub-backendspawner-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.2.3/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.2.4/backendspawner/api_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,15 +99,20 @@
             if event["html_message"].startswith("<details><summary>"):
                 event[
                     "html_message"
                 ] = f"<details><summary>{now}: {event['html_message'][len('<details><summary>'):]}"
             else:
                 event["html_message"] = f"{now}: {event['html_message']}"
 
-        if event:
+        if not event or spawner._stop_pending:
+            self.set_header("Content-Type", "text/plain")
+            self.write("Bad Request")
+            self.set_status(400)
+            return
+        else:
             self.log.debug(
                 "APICall: SpawnUpdate",
                 extra={
                     "uuidcode": uuidcode,
                     "log_name": f"{user_name}:{server_name}",
                     "user": user_name,
                     "action": "spawnupdate",
@@ -116,19 +121,14 @@
             )
             spawner = user.spawners[server_name]
             if hasattr(spawner, "latest_events"):
                 spawner.latest_events.append(event)
             self.set_header("Content-Type", "text/plain")
             self.set_status(204)
             return
-        else:
-            self.set_header("Content-Type", "text/plain")
-            self.write("Bad Request - No event in request body.")
-            self.set_status(400)
-            return
 
 
 default_handlers.append((r"/api/users/progress/status/([^/]+)", SpawnEventsAPIHandler))
 default_handlers.append(
     (r"/api/users/progress/status/([^/]+)/([^/]+)", SpawnEventsAPIHandler)
 )
 default_handlers.append((r"/api/users/progress/update/([^/]+)", SpawnEventsAPIHandler))
```

### Comparing `jupyterhub-backendspawner-0.2.3/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.2.4/backendspawner/backendspawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -475,24 +475,14 @@
             # We've already sent a request to the backend.
             # There's no need to do it again.
             return
 
         # Prevent multiple requests to the backend
         self.already_stopped = True
 
-        # if Spawner.stop was called by a custom APIHandler, we have to
-        # set these variables here. If it's called via user.stop() stop_pending
-        # is already true
-        if not self._stop_pending:
-            self._spawn_pending = False
-            self._start_pending = False
-            self._check_pending = False
-            self.stop_polling()
-            self._stop_pending = True
-
         url = await self.get_request_url_stop()
         headers = await self.get_request_headers_stop()
         req = HTTPRequest(
             url=url,
             method="DELETE",
             headers=headers,
             **self.get_request_kwargs(),
```

### Comparing `jupyterhub-backendspawner-0.2.3/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.2.4/backendspawner/eventspawner.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,30 +181,36 @@
         now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
         event = {
             "progress": 99,
             "failed": False,
             "html_message": f"<details><summary>{now}: JupyterLab start failed. Deleting related resources...</summary>This may take a few seconds.</details>",
         }
         self.latest_events.append(event)
-        msg = "Unknown Error"
-        if hasattr(exception, "args") and len(exception.args) > 1:
-            msg = f"{exception.args[0]} - {exception.args[1]}"
+        summary = "Unknown Error"
+        details = ""
         if hasattr(exception, "args") and len(exception.args) > 2:
             try:
-                body = json.loads(exception.args[2].body.decode())
-                msg += f": {body}"
+                error = json.loads(exception.args[2].body.decode())
+                if "error" in error.keys() and "detailed_error" in error.keys():
+                    summary = error.get("error")
+                    details = error.get("detailed_error")
+                else:
+                    summary = f"{exception.args[0]} - {exception.args[1]}"
+                    details = str(error)
             except:
                 self.log.exception("Could not load detailed error message")
+        elif hasattr(exception, "args") and len(exception.args) > 1:
+            summary = f"{exception.args[0]} - {exception.args[1]}"
 
         async def _get_stop_event(spawner):
             now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
             event = {
                 "progress": 100,
                 "failed": True,
-                "html_message": f"<details><summary>{now}: JupyterLab stopped.</summary>{msg}</details>",
+                "html_message": f"<details><summary>{now}: {summary}</summary>{details}</details>",
             }
             return event
 
         self.stop_event = _get_stop_event
         return super().run_failed_spawn_request_hook(exception)
 
     def run_pre_spawn_hook(self):
@@ -276,7 +282,8 @@
                 event = await self.get_stop_event()
             elif callable(event):
                 event = await maybe_future(event(self))
             self.latest_events.append(event)
 
         if cancel:
             await self.cancel()
+
```

### Comparing `jupyterhub-backendspawner-0.2.3/setup.py` & `jupyterhub-backendspawner-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.2.3",
+    version="0.2.4",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

