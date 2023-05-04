# Comparing `tmp/ampapi-1.1.2.tar.gz` & `tmp/ampapi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampapi-1.1.2.tar", last modified: Sat Apr 29 04:17:39 2023, max compression
+gzip compressed data, was "ampapi-1.1.3.tar", last modified: Thu May  4 03:29:29 2023, max compression
```

## Comparing `ampapi-1.1.2.tar` & `ampapi-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-29 04:17:39.713090 ampapi-1.1.2/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1074 2023-04-29 04:12:37.000000 ampapi-1.1.2/LICENCE
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4131 2023-04-29 04:17:39.713090 ampapi-1.1.2/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     3620 2023-04-29 04:12:37.000000 ampapi-1.1.2/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-29 04:17:39.713090 ampapi-1.1.2/ampapi/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-04-29 04:12:37.000000 ampapi-1.1.2/ampapi/__init__.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)   160315 2023-04-29 04:17:25.000000 ampapi-1.1.2/ampapi/ampapi.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-04-29 04:17:39.713090 ampapi-1.1.2/ampapi.egg-info/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     4131 2023-04-29 04:17:39.000000 ampapi-1.1.2/ampapi.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-04-29 04:17:39.000000 ampapi-1.1.2/ampapi.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-04-29 04:17:39.000000 ampapi-1.1.2/ampapi.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-04-29 04:17:39.000000 ampapi-1.1.2/ampapi.egg-info/top_level.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2023-04-29 04:12:37.000000 ampapi-1.1.2/pyproject.toml
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-04-29 04:17:39.717090 ampapi-1.1.2/setup.cfg
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-04 03:29:29.137461 ampapi-1.1.3/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     1074 2023-05-04 03:26:52.000000 ampapi-1.1.3/LICENCE
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-05-04 03:29:29.137461 ampapi-1.1.3/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     3610 2023-05-04 03:26:52.000000 ampapi-1.1.3/README.md
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-04 03:29:29.137461 ampapi-1.1.3/ampapi/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        0 2023-05-04 03:26:52.000000 ampapi-1.1.3/ampapi/__init__.py
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)   160317 2023-05-04 03:27:51.000000 ampapi-1.1.3/ampapi/ampapi.py
+drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-04 03:29:29.137461 ampapi-1.1.3/ampapi.egg-info/
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)     4121 2023-05-04 03:29:29.000000 ampapi-1.1.3/ampapi.egg-info/PKG-INFO
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      198 2023-05-04 03:29:29.000000 ampapi-1.1.3/ampapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-05-04 03:29:29.000000 ampapi-1.1.3/ampapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)        7 2023-05-04 03:29:29.000000 ampapi-1.1.3/ampapi.egg-info/top_level.txt
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      111 2023-05-04 03:26:52.000000 ampapi-1.1.3/pyproject.toml
+-rw-rw-r--   0 dylan     (1000) dylan     (1000)      600 2023-05-04 03:29:29.137461 ampapi-1.1.3/setup.cfg
```

### Comparing `ampapi-1.1.2/LICENCE` & `ampapi-1.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `ampapi-1.1.2/PKG-INFO` & `ampapi-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -36,18 +36,18 @@
 pip install requests aiohttp json
 ```
 
 ## Async Example
 
 ```python
 import asyncio
-from ampapi.ampapi import AMPAPIAsync
+from ampapi.ampapi import AMPAPI
 
 async def start() -> None:
-    API = AMPAPIAsync("http://localhost:8080/")
+    API = AMPAPI("http://localhost:8080/")
 
     try:
         # The third parameter is either used for 2FA logins, or if no password is specified to use a remembered token from a previous login, or a service login token.
         loginResult = await API.Core_LoginAsync("admin", "myfancypassword123", "", False)
 
         if "success" in loginResult.keys() and loginResult["success"]:
             print("Login successful")
```

### Comparing `ampapi-1.1.2/README.md` & `ampapi-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 pip install requests aiohttp json
 ```
 
 ## Async Example
 
 ```python
 import asyncio
-from ampapi.ampapi import AMPAPIAsync
+from ampapi.ampapi import AMPAPI
 
 async def start() -> None:
-    API = AMPAPIAsync("http://localhost:8080/")
+    API = AMPAPI("http://localhost:8080/")
 
     try:
         # The third parameter is either used for 2FA logins, or if no password is specified to use a remembered token from a previous login, or a service login token.
         loginResult = await API.Core_LoginAsync("admin", "myfancypassword123", "", False)
 
         if "success" in loginResult.keys() and loginResult["success"]:
             print("Login successful")
```

### Comparing `ampapi-1.1.2/ampapi/ampapi.py` & `ampapi-1.1.3/ampapi/ampapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         headers = {'accept': 'text/javascript',}
         session = {"SESSIONID": self.sessionId}
         data_added = dict(session, **data)
 
         data_json = json.dumps(data_added)
 
         async with ClientSession() as session:
-            async with session.post(url=f'{self.dataSource}{endpoint}', headers=headers, data=data_json) as post:
+            async with session.post(url=f'{self.dataSource}/{endpoint}', headers=headers, data=data_json) as post:
                 response = await post.json()
                 post.close()
 
         return response
 
     def ADSModule_AddDatastore(self, newDatastore):
         """
@@ -4608,15 +4608,15 @@
             headers = {'accept': 'text/javascript',}
             session = {"SESSIONID": self.sessionId}
             data_added = dict(session, **data)
 
             data_json = json.dumps(data_added)
 
             async with ClientSession() as session:
-                async with session.post(url=f'{self.dataSource}{endpoint}', headers=headers, data=data_json) as post:
+                async with session.post(url=f'{self.dataSource}/{endpoint}', headers=headers, data=data_json) as post:
                     response = await post.json()
                     post.close()
 
             return response
         except Exception as e:
             # If retry is set to true, raise the exception
             if retry:
```

### Comparing `ampapi-1.1.2/ampapi.egg-info/PKG-INFO` & `ampapi-1.1.3/ampapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampapi
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python implemenation of the Cubecoders AMP API.
 Home-page: https://github.com/p0t4t0sandwich/ampapi-python
 Author: Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 Author-email: p0t4t0sandwich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -36,18 +36,18 @@
 pip install requests aiohttp json
 ```
 
 ## Async Example
 
 ```python
 import asyncio
-from ampapi.ampapi import AMPAPIAsync
+from ampapi.ampapi import AMPAPI
 
 async def start() -> None:
-    API = AMPAPIAsync("http://localhost:8080/")
+    API = AMPAPI("http://localhost:8080/")
 
     try:
         # The third parameter is either used for 2FA logins, or if no password is specified to use a remembered token from a previous login, or a service login token.
         loginResult = await API.Core_LoginAsync("admin", "myfancypassword123", "", False)
 
         if "success" in loginResult.keys() and loginResult["success"]:
             print("Login successful")
```

### Comparing `ampapi-1.1.2/setup.cfg` & `ampapi-1.1.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ampapi
-version = 1.1.2
+version = 1.1.3
 author = Dylan Sperrer - p0t4t0sandwich - ThePotatoKing#3452
 author_email = p0t4t0sandwich@gmail.com
 description = A Python implemenation of the Cubecoders AMP API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/p0t4t0sandwich/ampapi-python
 classifiers =
```

