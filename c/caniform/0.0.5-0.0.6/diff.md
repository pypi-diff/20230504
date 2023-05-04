# Comparing `tmp/caniform-0.0.5.tar.gz` & `tmp/caniform-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caniform-0.0.5.tar", last modified: Fri Nov  4 19:47:24 2022, max compression
+gzip compressed data, was "caniform-0.0.6.tar", last modified: Thu May  4 17:26:47 2023, max compression
```

## Comparing `caniform-0.0.5.tar` & `caniform-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2022-11-04 19:47:24.597086 caniform-0.0.5/
--rw-r--r--   0 dev        (501) staff       (20)     1112 2022-06-02 18:33:45.000000 caniform-0.0.5/LICENSE
--rw-r--r--   0 dev        (501) staff       (20)      610 2022-11-04 19:47:24.597248 caniform-0.0.5/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)       93 2022-06-02 18:36:10.000000 caniform-0.0.5/README.md
--rw-r--r--   0 dev        (501) staff       (20)      151 2022-06-07 15:32:34.000000 caniform-0.0.5/pyproject.toml
--rw-r--r--   0 dev        (501) staff       (20)      642 2022-11-04 19:47:24.598143 caniform-0.0.5/setup.cfg
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2022-11-04 19:47:24.590561 caniform-0.0.5/src/
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2022-11-04 19:47:24.594302 caniform-0.0.5/src/caniform/
--rw-r--r--   0 dev        (501) staff       (20)     7911 2022-11-04 19:45:36.000000 caniform-0.0.5/src/caniform/Extend.py
--rw-r--r--   0 dev        (501) staff       (20)        0 2022-06-02 18:32:13.000000 caniform-0.0.5/src/caniform/__init__.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2022-11-04 19:47:24.596764 caniform-0.0.5/src/caniform.egg-info/
--rw-r--r--   0 dev        (501) staff       (20)      610 2022-11-04 19:47:24.000000 caniform-0.0.5/src/caniform.egg-info/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)      234 2022-11-04 19:47:24.000000 caniform-0.0.5/src/caniform.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (501) staff       (20)        1 2022-11-04 19:47:24.000000 caniform-0.0.5/src/caniform.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (501) staff       (20)        9 2022-11-04 19:47:24.000000 caniform-0.0.5/src/caniform.egg-info/top_level.txt
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-04 17:26:47.717943 caniform-0.0.6/
+-rw-r--r--   0 dev        (501) staff       (20)     1112 2022-06-02 18:33:45.000000 caniform-0.0.6/LICENSE
+-rw-r--r--   0 dev        (501) staff       (20)      610 2023-05-04 17:26:47.718110 caniform-0.0.6/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)       93 2022-06-02 18:36:10.000000 caniform-0.0.6/README.md
+-rw-r--r--   0 dev        (501) staff       (20)      151 2022-06-07 15:32:34.000000 caniform-0.0.6/pyproject.toml
+-rw-r--r--   0 dev        (501) staff       (20)      642 2023-05-04 17:26:47.718906 caniform-0.0.6/setup.cfg
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-04 17:26:47.706837 caniform-0.0.6/src/
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-04 17:26:47.715801 caniform-0.0.6/src/caniform/
+-rw-r--r--   0 dev        (501) staff       (20)     8879 2023-05-04 17:16:03.000000 caniform-0.0.6/src/caniform/Extend.py
+-rw-r--r--   0 dev        (501) staff       (20)        0 2022-06-02 18:32:13.000000 caniform-0.0.6/src/caniform/__init__.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-04 17:26:47.717573 caniform-0.0.6/src/caniform.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)      610 2023-05-04 17:26:47.000000 caniform-0.0.6/src/caniform.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      234 2023-05-04 17:26:47.000000 caniform-0.0.6/src/caniform.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2023-05-04 17:26:47.000000 caniform-0.0.6/src/caniform.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (501) staff       (20)        9 2023-05-04 17:26:47.000000 caniform-0.0.6/src/caniform.egg-info/top_level.txt
```

### Comparing `caniform-0.0.5/LICENSE` & `caniform-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `caniform-0.0.5/PKG-INFO` & `caniform-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caniform
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package that extends the functionality of Pandas.
 Home-page: https://gitlab.com/tomathon/caniform/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/caniform/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caniform-0.0.5/setup.cfg` & `caniform-0.0.6/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = caniform
-version = 0.0.5
+version = 0.0.6
 author = tomathon
 author_email = tomathon.dev@pm.me
 description = A package that extends the functionality of Pandas.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/tomathon/caniform/
 project_urls =
```

### Comparing `caniform-0.0.5/src/caniform/Extend.py` & `caniform-0.0.6/src/caniform/Extend.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from sklearn.linear_model import LinearRegression
 import pandas as pd
 import numpy as np
 import re
+import json
+import requests
+from concurrent.futures import ThreadPoolExecutor
 
 
 
 
 
 @pd.api.extensions.register_dataframe_accessor("ext")
 class Extend:
@@ -216,7 +219,29 @@
 
     def apply_except(self, *args, func, **kwargs):
         ret_df = self._obj.copy()
         col_rem_lst = [*args]
         col_keep_lst = list(set(ret_df.columns) - set(col_rem_lst))
         ret_df[col_keep_lst] = ret_df[col_keep_lst].apply(func, **kwargs)
         return ret_df
+
+
+    def __make_dict_list(self, _df):
+        _df = _df.reset_index(drop = True)
+        return json.loads(json.dumps(list(_df.T.to_dict().values())))
+    
+    def __post_request(self, _payload_dict, _url, _headers):
+        payload_dict = json.dumps(_payload_dict)
+        return requests.post(
+            url = _url, 
+            headers = _headers,
+            data = payload_dict
+        )
+    
+    def post(self, endpoint, headers = None, n_max_workers = 10):
+        df = self._obj
+        headers = {"Accept-Charset": "UTF-8"} if headers is None else headers
+        payload_dict_list = self.__make_dict_list(df)
+        processes = []
+        with ThreadPoolExecutor(max_workers = n_max_workers) as executor:
+            for pdl in payload_dict_list:
+                processes.append(executor.submit(self.__post_request, _payload_dict = pdl, _url = endpoint, _headers = headers))
```

### Comparing `caniform-0.0.5/src/caniform.egg-info/PKG-INFO` & `caniform-0.0.6/src/caniform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caniform
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package that extends the functionality of Pandas.
 Home-page: https://gitlab.com/tomathon/caniform/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/caniform/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

