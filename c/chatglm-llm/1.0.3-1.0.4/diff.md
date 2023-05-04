# Comparing `tmp/chatglm-llm-1.0.3.tar.gz` & `tmp/chatglm-llm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.0.3.tar", last modified: Thu May  4 01:33:28 2023, max compression
+gzip compressed data, was "chatglm-llm-1.0.4.tar", last modified: Thu May  4 02:16:17 2023, max compression
```

## Comparing `chatglm-llm-1.0.3.tar` & `chatglm-llm-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1887 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/chatglm_llm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 01:30:33.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-04 01:33:28.000000 chatglm-llm-1.0.3/chatglm_llm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/chatglm_src/
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/chatglm_src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3963 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/chatglm_src/callbacks.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/chatglm_src/cmd.py
--rw-r--r--   0 root         (0) root         (0)    16989 2023-05-04 01:30:19.000000 chatglm-llm-1.0.3/chatglm_src/llm.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 01:33:28.289258 chatglm-llm-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      802 2023-05-04 01:33:21.000000 chatglm-llm-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-05-04 01:30:19.000000 chatglm-llm-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/chatglm_llm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 01:30:33.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-04 02:16:17.000000 chatglm-llm-1.0.4/chatglm_llm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/chatglm_src/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-04 01:30:19.000000 chatglm-llm-1.0.4/chatglm_src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-05-04 01:30:19.000000 chatglm-llm-1.0.4/chatglm_src/callbacks.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-04 01:30:19.000000 chatglm-llm-1.0.4/chatglm_src/cmd.py
+-rw-r--r--   0 root         (0) root         (0)    17117 2023-05-04 02:15:45.000000 chatglm-llm-1.0.4/chatglm_src/llm.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 02:16:17.377296 chatglm-llm-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      802 2023-05-04 02:15:53.000000 chatglm-llm-1.0.4/setup.py
```

### Comparing `chatglm-llm-1.0.3/README.md` & `chatglm-llm-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.0.3/chatglm_src/callbacks.py` & `chatglm-llm-1.0.4/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.0.3/chatglm_src/llm.py` & `chatglm-llm-1.0.4/chatglm_src/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # only load from local's path
 # default path is in ~/.cache/chatglm, if not exists, will download from huggingface'url :https://huggingface.co/THUDM/chatglm-6b
 # 
 """Common utility functions for working with LLM APIs."""
 import re
 from typing import List
 TODAY = datetime.datetime.now()
-PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}-{TODAY.day}"
+PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
 
 
 def enforce_stop_tokens(text: str, stop: List[str]) -> str:
     """Cut off the text as soon as any stop words occur."""
     return re.split("|".join(stop), text)[0]
 
 def auto_gc():
@@ -246,17 +246,19 @@
             self.history = self.history+[[None, current_completion]]
             return current_completion
         elif self.remote_host is not None :
             ws = create_connection(f"ws://{self.remote_host}:15000")
             # self.callback_manager =  langchain.callbacks.base.BaseCallbackManager(self.callbacks)
             self.callback_manager.set_handlers(self.callbacks)
             user_id = md5(time.asctime().encode()).hexdigest()
-            ws.send(json.dumps({"user_id":user_id, "password":PASSWORD}).encode())
+            ws.send(json.dumps({"user_id":user_id, "password":PASSWORD}))
+            # time.sleep(0.5)
             res = ws.recv()
             if res != "ok":
+                print(colored("[info]:","yellow") ,res)
                 raise Exception("password error")
             result = ''
             ws.send(json.dumps({"prompt":prompt, "history":self.history}))
             self.callback_manager.on_llm_start(
                 prompt,
                 None,
                 verbose=self.verbose
@@ -324,14 +326,15 @@
     llm = None
     @classmethod
     async def echo(cls,websocket):
         try:
             print(colored("[connected]","green"),":",websocket)
             no = 0
             async for message in websocket:
+                print(colored("[recv]","yellow") ,":",message)
                 if no == 0:
                     if await cls.user(message, websocket):
                         no += 1
                         continue
                     else:
                         await websocket.close()
                         break
```

### Comparing `chatglm-llm-1.0.3/setup.py` & `chatglm-llm-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-llm',
-    version='1.0.3',
+    version='1.0.4',
     description='chatglm llm',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
```

