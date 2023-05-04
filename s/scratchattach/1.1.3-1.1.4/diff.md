# Comparing `tmp/scratchattach-1.1.3.tar.gz` & `tmp/scratchattach-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.1.3.tar", last modified: Thu Mar 30 10:16:32 2023, max compression
+gzip compressed data, was "scratchattach-1.1.4.tar", last modified: Thu May  4 17:47:55 2023, max compression
```

## Comparing `scratchattach-1.1.3.tar` & `scratchattach-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 10:16:32.541222 scratchattach-1.1.3/
--rw-rw-rw-   0        0        0    22206 2023-03-30 10:16:32.540226 scratchattach-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    20877 2022-11-15 20:01:18.000000 scratchattach-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 10:16:32.487367 scratchattach-1.1.3/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-03-25 13:54:22.000000 scratchattach-1.1.3/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    12439 2023-03-30 10:15:18.000000 scratchattach-1.1.3/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    15263 2023-03-30 10:13:01.000000 scratchattach-1.1.3/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-03-25 13:54:22.000000 scratchattach-1.1.3/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      779 2023-03-25 13:54:22.000000 scratchattach-1.1.3/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6542 2023-03-25 13:54:22.000000 scratchattach-1.1.3/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18152 2023-03-25 13:54:22.000000 scratchattach-1.1.3/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17923 2023-03-25 13:54:22.000000 scratchattach-1.1.3/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9651 2023-03-25 13:54:22.000000 scratchattach-1.1.3/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25071 2023-03-25 15:35:18.000000 scratchattach-1.1.3/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:16:32.536266 scratchattach-1.1.3/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22206 2023-03-30 10:16:31.000000 scratchattach-1.1.3/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-03-30 10:16:32.000000 scratchattach-1.1.3/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 10:16:31.000000 scratchattach-1.1.3/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-03-30 10:16:31.000000 scratchattach-1.1.3/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-30 10:16:31.000000 scratchattach-1.1.3/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 10:16:32.541222 scratchattach-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-03-30 10:15:42.000000 scratchattach-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:47:55.286839 scratchattach-1.1.4/
+-rw-rw-rw-   0        0        0    21811 2023-05-04 17:47:55.285838 scratchattach-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    20499 2023-05-04 17:45:21.000000 scratchattach-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 17:47:55.214501 scratchattach-1.1.4/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    12798 2023-05-04 17:35:55.000000 scratchattach-1.1.4/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    15496 2023-05-04 17:24:58.000000 scratchattach-1.1.4/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      779 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6542 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18152 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17923 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9651 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25071 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:47:55.281296 scratchattach-1.1.4/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    21811 2023-05-04 17:47:54.000000 scratchattach-1.1.4/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-05-04 17:47:55.000000 scratchattach-1.1.4/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:47:54.000000 scratchattach-1.1.4/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-04 17:47:54.000000 scratchattach-1.1.4/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-04 17:47:54.000000 scratchattach-1.1.4/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:47:55.287210 scratchattach-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-05-04 16:38:08.000000 scratchattach-1.1.4/setup.py
```

### Comparing `scratchattach-1.1.3/PKG-INFO` & `scratchattach-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.3
+Version: 1.1.4
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -55,15 +55,15 @@
 
 session = scratch3.login("username", "password")
 ```
 
 `login()` returns a `Session` object that saves your login
 
 **Logging in with a sessionId:**
-*You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/#get-your-session-id)*
+*You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
 
 ```python
 import scratchattach as scratch3
 
 session = scratch3.Session("sessionId", username="username")
 ```
 
@@ -306,14 +306,15 @@
 project = scratch3.get_project("project_id")
 ```
 
 **Attributes:**
 ```python
 project.id  #Returns the project id
 project.url  #Returns the project url
+project.title #Returns the project title
 project.author  #Returns the username of the author
 project.comments_allowed  #Returns True if comments are enabled
 project.instructions
 project.notes  #Returns the 'Notes and Credits' section
 project.created  #Returns the date of the project creation
 project.last_modified  #Returns the date when the project was modified the last time
 project.share_date
@@ -597,24 +598,14 @@
 # Backpack
 
 ```python
 session.backpack(limit=20, offset=0) #Returns the contents of your backpack as dictionary
 session.delete_from_backpack("asset id") #Deletes an asset from your backpack
 ```
 
-# Get your session id
-
-This section explains how to get your Scratch session id from your browser cookies.
-
-1. Open scratch.mit.edu in your browser
-2. Click the ðŸ”’ icon in the URL bar, then click "Cookies"
-3. Then find a cookie called `scratchsessionid` (in the "scratch.mit.edu" Â» "Cookies" folder). The content of this cookie is your Scratch session id
-
-![](https://scratch3-assets.1tim.repl.co/template/cookies.png)
-
 # Contributors
 
 - Allmost all code by TimMcCool.
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scratchattach-1.1.3/README.md` & `scratchattach-1.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 session = scratch3.login("username", "password")
 ```
 
 `login()` returns a `Session` object that saves your login
 
 **Logging in with a sessionId:**
-*You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/#get-your-session-id)*
+*You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
 
 ```python
 import scratchattach as scratch3
 
 session = scratch3.Session("sessionId", username="username")
 ```
 
@@ -290,14 +290,15 @@
 project = scratch3.get_project("project_id")
 ```
 
 **Attributes:**
 ```python
 project.id  #Returns the project id
 project.url  #Returns the project url
+project.title #Returns the project title
 project.author  #Returns the username of the author
 project.comments_allowed  #Returns True if comments are enabled
 project.instructions
 project.notes  #Returns the 'Notes and Credits' section
 project.created  #Returns the date of the project creation
 project.last_modified  #Returns the date when the project was modified the last time
 project.share_date
@@ -581,24 +582,14 @@
 # Backpack
 
 ```python
 session.backpack(limit=20, offset=0) #Returns the contents of your backpack as dictionary
 session.delete_from_backpack("asset id") #Deletes an asset from your backpack
 ```
 
-# Get your session id
-
-This section explains how to get your Scratch session id from your browser cookies.
-
-1. Open scratch.mit.edu in your browser
-2. Click the 🔒 icon in the URL bar, then click "Cookies"
-3. Then find a cookie called `scratchsessionid` (in the "scratch.mit.edu" » "Cookies" folder). The content of this cookie is your Scratch session id
-
-![](https://scratch3-assets.1tim.repl.co/template/cookies.png)
-
 # Contributors
 
 - Allmost all code by TimMcCool.
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scratchattach-1.1.3/scratchattach/_cloud.py` & `scratchattach-1.1.4/scratchattach/_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from numpy import var
 import websocket
 import json
 import requests
 from threading import Thread
 import time
 from . import _exceptions
+import traceback
 
 class _CloudMixin:
 
     def __init__(self, *, project_id, username="python", session_id=None, cloud_host=None, _allow_non_numeric=False, _no_reconnect=False):
         self._session_id = session_id
         self._username = username
         try:
@@ -225,15 +226,22 @@
             if self.running:
                 data = get_cloud_logs(project_id = self.project_id, limit = 15)
                 if data != self.data:
                     for activity in data:
                         if activity in self.data:
                             break
                         if "on_"+activity["verb"][:-4] in self._events:
-                            self._events["on_"+activity["verb"][:-4]](self.Event(user=activity["user"], var=activity["name"][2:], name=activity["name"][2:], value=activity["value"], timestamp=activity["timestamp"]))
+                            try:
+                                self._events["on_"+activity["verb"][:-4]](self.Event(user=activity["user"], var=activity["name"][2:], name=activity["name"][2:], value=activity["value"], timestamp=activity["timestamp"]))
+                            except Exception as e:
+                                print("Caught error in cloud event - Full error below")
+                                try:
+                                    traceback.print_exc()
+                                except Exception:
+                                    print(e)
                 self.data = data
             else:
                 return
             time.sleep(self.update_interval)
 
     def stop(self):
         if self._thread is not None:
@@ -277,15 +285,15 @@
             except Exception:
                 try:
                     self.connection._connect(cloud_host=self.connection.cloud_host)
                     self.connection._handshake()
                 except Exception:
                     if "on_disconnect" in self._events:
                         self._events["on_disconnect"]()
-                        
+
 class WsCloudEvents(CloudEvents):
 
     def __init__(self, project_id, connection):
         self.data = []
         self._thread = None
         self.running = False
         self._events = {}
```

### Comparing `scratchattach-1.1.3/scratchattach/_cloud_requests.py` & `scratchattach-1.1.4/scratchattach/_cloud_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,39 +10,44 @@
 class CloudRequests:
 
     class Request:
         def __init__(self, **entries):
             self.__dict__.update(entries)
             self.id = self.request_id
 
+    def init_attributes(self):
+        self.last_requester = None
+        self.last_timestamp = 0
+        self.last_request_id = None
+
+        self.requests = {}
+        self.events = []
+
+        self.request_parts = {}
+        self.outputs = {}
+        self.respond_in_thread= False
+        self.current_var = 0
+        self.idle_since = 0
+
     def __init__(self, cloud_connection : _cloud.CloudConnection, *, used_cloud_vars = ["1","2","3","4","5","6","7","8","9"], ignore_exceptions=True, force_reconnect=True, _log_url="https://clouddata.scratch.mit.edu/logs", _packet_length=245):
         print("\033[1mIf you use CloudRequests in your Scratch project, please credit TimMcCool!\033[0m")
         if _log_url != "https://clouddata.scratch.mit.edu/logs":
             print("Warning: Log URL isn't the URL of Scratch's clouddata logs. Don't use the _log_url parameter unless you know what you are doing.")
         if _packet_length > 245:
             print("Warning: The packet length was set to a value higher than default (245). Your project most likely won't work on Scratch.")
+
         self.used_cloud_vars = used_cloud_vars
         self.connection = cloud_connection
         self.project_id = cloud_connection.project_id
 
         self.ignore_exceptions = ignore_exceptions
         self.log_url = _log_url
         self.packet_length = _packet_length
 
-        self.last_requester = None
-        self.last_timestamp = 0
-
-        self.requests = {}
-        self.events = []
-
-        self.request_parts = {}
-        self.outputs = {}
-        self.respond_in_thread= False
-        self.current_var = 0
-        self.idle_since = 0
+        self.init_attributes()
 
     def request(self, function=None, *, enabled=True, name=None, thread=False):
         def inner(function):
             if thread:
                 self.respond_in_thread = True
                 print("Warning: Running individual requests in threads increases CPU usage")
             self.requests[function.__name__ if name is None else name] = {"name":function.__name__ if name is None else name,"enabled":enabled,"on_call":function,"thread":thread}
@@ -99,14 +104,20 @@
 
     def event(self, function):
 
         self.events.append(function)
 
     def get_requester(self):
 
+        if self.last_requester is None:
+            logs = _cloud.get_cloud_logs(self.project_id, filter_by_var_named="TO_HOST")
+            activity = list(filter(lambda x : "."+self.last_request_id in x["value"], logs))
+            if len(activity) > 0:
+                self.last_requester = activity[0]["user"]
+
         return self.last_requester
 
     def get_timestamp(self):
 
         return self.last_timestamp
 
     def _respond(self, request_id, response, limit, *, force_reconnect=False, validation=2222):
@@ -150,15 +161,15 @@
                     self.current_var = 0
 
                 remaining_response = ""
                 time.sleep(0.1)
 
         self.idle_since = time.time()
 
-    def run(self, thread=False, data_from_websocket=False):
+    def run(self, thread=False, data_from_websocket=True):
         if data_from_websocket is True:
             events = _cloud.WsCloudEvents(self.project_id, _cloud.CloudConnection(project_id = self.project_id, username = self.connection._username, session_id=self.connection._session_id))
         else:
             events = _cloud.CloudEvents(self.project_id)
         if thread:
             thread = Thread(target=self._run, args=[events], kwargs={"data_from_websocket":data_from_websocket})
             thread.start()
@@ -302,14 +313,15 @@
 
                         if request not in self.requests:
                             print(f"Warning: Client received an unknown request called '{request}'")
                             self.call_event("on_unknown_request", [self.Request(name=request,request=request,requester=self.last_requester,timestamp=self.last_timestamp,arguments=arguments,request_id=request_id)])
                             continue
                         else:
                             req_obj = self.requests[request]
+                            self.last_request_id = request_id
                             if req_obj["thread"]:
                                 Thread(target=self.call_request, args=(request_id, req_obj, arguments)).start()
                             else:
                                 self.call_request(request_id, req_obj, arguments)
                 self.last_data = data
 
             output_ids = list(self.outputs.keys())
@@ -329,26 +341,15 @@
         self.used_cloud_vars = used_cloud_vars
         self.connection = cloud_connection
         self.project_id = cloud_connection.project_id
 
         self.ignore_exceptions = ignore_exceptions
         self.packet_length = _packet_length
 
-        self.last_requester = None
-        self.last_timestamp = 0
-
-        self.requests = {}
-        self.events = []
-
-        self.request_parts = {}
-        self.outputs = {}
-        self.respond_in_thread= False
-        self.current_var = 0
-        self.idle_since = 0
-
+        self.init_attributes()
 
     def get_requester(self):
         return None
 
     def run(self, thread=False, data_from_websocket=True):
         events = _cloud.TwCloudEvents(self.project_id)
         if thread:
```

### Comparing `scratchattach-1.1.3/scratchattach/_encoder.py` & `scratchattach-1.1.4/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.3/scratchattach/_exceptions.py` & `scratchattach-1.1.4/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.3/scratchattach/_forum.py` & `scratchattach-1.1.4/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.3/scratchattach/_project.py` & `scratchattach-1.1.4/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.3/scratchattach/_session.py` & `scratchattach-1.1.4/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.3/scratchattach/_studio.py` & `scratchattach-1.1.4/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.3/scratchattach/_user.py` & `scratchattach-1.1.4/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.3/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.1.4/scratchattach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.3
+Version: 1.1.4
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -55,15 +55,15 @@
 
 session = scratch3.login("username", "password")
 ```
 
 `login()` returns a `Session` object that saves your login
 
 **Logging in with a sessionId:**
-*You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/#get-your-session-id)*
+*You can get your session id from your browser's cookies. [More information](https://github.com/TimMcCool/scratchattach/wiki/Get-your-session-id)*
 
 ```python
 import scratchattach as scratch3
 
 session = scratch3.Session("sessionId", username="username")
 ```
 
@@ -306,14 +306,15 @@
 project = scratch3.get_project("project_id")
 ```
 
 **Attributes:**
 ```python
 project.id  #Returns the project id
 project.url  #Returns the project url
+project.title #Returns the project title
 project.author  #Returns the username of the author
 project.comments_allowed  #Returns True if comments are enabled
 project.instructions
 project.notes  #Returns the 'Notes and Credits' section
 project.created  #Returns the date of the project creation
 project.last_modified  #Returns the date when the project was modified the last time
 project.share_date
@@ -597,24 +598,14 @@
 # Backpack
 
 ```python
 session.backpack(limit=20, offset=0) #Returns the contents of your backpack as dictionary
 session.delete_from_backpack("asset id") #Deletes an asset from your backpack
 ```
 
-# Get your session id
-
-This section explains how to get your Scratch session id from your browser cookies.
-
-1. Open scratch.mit.edu in your browser
-2. Click the ðŸ”’ icon in the URL bar, then click "Cookies"
-3. Then find a cookie called `scratchsessionid` (in the "scratch.mit.edu" Â» "Cookies" folder). The content of this cookie is your Scratch session id
-
-![](https://scratch3-assets.1tim.repl.co/template/cookies.png)
-
 # Contributors
 
 - Allmost all code by TimMcCool.
 - See the GitHub repository for full list of contributors.
 - Create a pull request to contribute code yourself.
 
 # Support
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scratchattach-1.1.3/setup.py` & `scratchattach-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.3'
+VERSION = '1.1.4'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

