# Comparing `tmp/yao-0.0.3.tar.gz` & `tmp/yao-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yao-0.0.3.tar", last modified: Fri Apr 21 11:21:32 2023, max compression
+gzip compressed data, was "yao-0.0.4.tar", last modified: Thu May  4 08:17:21 2023, max compression
```

## Comparing `yao-0.0.3.tar` & `yao-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.154589 yao-0.0.3/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-04-21 11:21:32.154396 yao-0.0.3/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)       38 2023-04-21 11:21:32.154639 yao-0.0.3/setup.cfg
--rw-r--r--   0 ke         (501) wheel        (0)      971 2023-04-21 11:17:18.000000 yao-0.0.3/setup.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.149113 yao-0.0.3/yao/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)    19246 2023-04-18 07:31:04.000000 yao-0.0.3/yao/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-04-18 07:31:04.000000 yao-0.0.3/yao/db.py
--rw-r--r--   0 ke         (501) wheel        (0)     7904 2023-04-18 07:31:04.000000 yao-0.0.3/yao/depends.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.150192 yao-0.0.3/yao/function/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/__init__.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.150719 yao-0.0.3/yao/function/annex/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/annex/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      187 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/annex/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/annex/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/annex/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.151339 yao-0.0.3/yao/function/appointment/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/appointment/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/appointment/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/appointment/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/appointment/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.151998 yao-0.0.3/yao/function/company/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/company/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      192 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/company/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/company/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/company/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.152548 yao-0.0.3/yao/function/department/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/department/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      189 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/department/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/department/main.py
--rw-r--r--   0 ke         (501) wheel        (0)      992 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/department/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.153096 yao-0.0.3/yao/function/log/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/log/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      169 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/log/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/log/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/log/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)      665 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-04-21 10:39:40.000000 yao-0.0.3/yao/function/model.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.153651 yao-0.0.3/yao/function/permission/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/permission/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      199 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/permission/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/permission/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/permission/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.154182 yao-0.0.3/yao/function/user/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/user/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/user/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/user/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-04-18 07:31:04.000000 yao-0.0.3/yao/function/user/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-04-18 07:31:04.000000 yao-0.0.3/yao/helpers.py
--rw-r--r--   0 ke         (501) wheel        (0)    11459 2023-04-18 07:31:04.000000 yao-0.0.3/yao/method.py
--rw-r--r--   0 ke         (501) wheel        (0)     1803 2023-04-18 07:31:04.000000 yao-0.0.3/yao/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-04-21 11:21:32.149781 yao-0.0.3/yao.egg-info/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/SOURCES.txt
--rw-r--r--   0 ke         (501) wheel        (0)        1 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/dependency_links.txt
--rw-r--r--   0 ke         (501) wheel        (0)      166 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/requires.txt
--rw-r--r--   0 ke         (501) wheel        (0)        4 2023-04-21 11:21:32.000000 yao-0.0.3/yao.egg-info/top_level.txt
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.041536 yao-0.0.4/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-05-04 08:17:21.041359 yao-0.0.4/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)       38 2023-05-04 08:17:21.041583 yao-0.0.4/setup.cfg
+-rw-r--r--   0 ke         (501) wheel        (0)      971 2023-05-04 08:10:53.000000 yao-0.0.4/setup.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.035617 yao-0.0.4/yao/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)    19246 2023-04-18 07:31:04.000000 yao-0.0.4/yao/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-04-18 07:31:04.000000 yao-0.0.4/yao/db.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8279 2023-05-04 06:26:02.000000 yao-0.0.4/yao/depends.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.036791 yao-0.0.4/yao/function/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/__init__.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.037446 yao-0.0.4/yao/function/annex/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/annex/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      187 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/annex/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/annex/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/annex/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.038024 yao-0.0.4/yao/function/appointment/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/appointment/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/appointment/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/appointment/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/appointment/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.038590 yao-0.0.4/yao/function/company/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/company/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      192 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/company/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/company/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/company/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.039163 yao-0.0.4/yao/function/department/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/department/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      189 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/department/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/department/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)      992 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/department/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.039924 yao-0.0.4/yao/function/log/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/log/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      169 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/log/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/log/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/log/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      665 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-04-21 10:39:40.000000 yao-0.0.4/yao/function/model.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.040589 yao-0.0.4/yao/function/permission/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/permission/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      199 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/permission/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/permission/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/permission/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.041151 yao-0.0.4/yao/function/user/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/user/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/user/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/user/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-04-18 07:31:04.000000 yao-0.0.4/yao/function/user/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-04-18 07:31:04.000000 yao-0.0.4/yao/helpers.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11459 2023-04-18 07:31:04.000000 yao-0.0.4/yao/method.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1868 2023-04-26 09:42:16.000000 yao-0.0.4/yao/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-05-04 08:17:21.036312 yao-0.0.4/yao.egg-info/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/SOURCES.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        1 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/dependency_links.txt
+-rw-r--r--   0 ke         (501) wheel        (0)      166 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/requires.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        4 2023-05-04 08:17:21.000000 yao-0.0.4/yao.egg-info/top_level.txt
```

### Comparing `yao-0.0.3/setup.py` & `yao-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yao",
-    version="0.0.3",
+    version="0.0.4",
     description="Dev",
     python_requires=">=3.9",
     author="Lsshu",
     author_email="admin@lsshu.cn",
     url="https://github.com/lsshu/yao",
     packages=find_packages(),
     long_description=long_description,
```

### Comparing `yao-0.0.3/yao/crud.py` & `yao-0.0.4/yao/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/db.py` & `yao-0.0.4/yao/db.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/depends.py` & `yao-0.0.4/yao/depends.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import asyncio
+from datetime import datetime
 from functools import wraps
 from typing import Optional, List, Union
 
 from fastapi import Depends, Security, APIRouter, Query, Request, HTTPException, status
 from fastapi.security import SecurityScopes, OAuth2PasswordBearer
 from fastapi.security.utils import get_authorization_scheme_param
 from sqlalchemy.orm import Session
@@ -129,15 +130,15 @@
     @wraps(callback)
     async def wrapper(*args, **kwargs):
         if "item" in kwargs and "auth" in kwargs:
             item = kwargs.get("item")
             auth = kwargs.get("auth")
             if hasattr(item, "prefix"):
                 item.prefix = item.prefix or auth.prefix
-                if hasattr(item, 'name'):
+                if hasattr(item, 'name') and item.name:
                     item.name = "%s@%s" % (item.prefix, item.name.replace("%s@" % item.prefix, ""))
                 kwargs.update({
                     "item": item
                 })
         response = await callback(*args, **kwargs) if asyncio.iscoroutinefunction(callback) else callback(*args, **kwargs)
         return response
 
@@ -162,21 +163,29 @@
             })
         response = await callback(*args, **kwargs) if asyncio.iscoroutinefunction(callback) else callback(*args, **kwargs)
         return response
 
     return wrapper
 
 
+class DateEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, datetime):
+            return obj.strftime("%Y-%m-%d %H:%M:%S")
+        else:
+            return json.JSONEncoder.default(self, obj)
+
+
 def log_to_database(session=None, scope=None, methods=None, item=None, auth=None, **kwargs):
     prefix = item.prefix if item and hasattr(item, "prefix") and item.prefix else auth.prefix if auth else None
     if ('post' in methods and scope[:5] == ".post") or 'patch' in methods:
-
         CrudFunctionLog.init().store(
             session=session,
-            item=SchemasStoreUpdateLog(prefix=prefix, scope=scope, methods=",".join(methods), data=item, username=auth.user.username),
+            item=SchemasStoreUpdateLog(prefix=prefix, scope=scope, methods=",".join(methods), data=json.loads(json.dumps(item.dict(exclude_unset=True), cls=DateEncoder)),
+                                       username=auth.user.username),
             close=False)
 
     if 'delete' in methods:
         CrudFunctionLog.init().store(
             session=session,
             item=SchemasStoreUpdateLog(prefix=prefix, scope=scope, methods=",".join(methods), data=kwargs.get('uuids'), username=auth.user.username),
             close=False)
```

### Comparing `yao-0.0.3/yao/function/annex/main.py` & `yao-0.0.4/yao/function/annex/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/annex/schema.py` & `yao-0.0.4/yao/function/annex/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/appointment/crud.py` & `yao-0.0.4/yao/function/appointment/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/appointment/main.py` & `yao-0.0.4/yao/function/appointment/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/appointment/schema.py` & `yao-0.0.4/yao/function/appointment/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/company/main.py` & `yao-0.0.4/yao/function/company/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/company/schema.py` & `yao-0.0.4/yao/function/company/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/department/main.py` & `yao-0.0.4/yao/function/department/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/department/schema.py` & `yao-0.0.4/yao/function/department/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/log/main.py` & `yao-0.0.4/yao/function/log/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/log/schema.py` & `yao-0.0.4/yao/function/log/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/main.py` & `yao-0.0.4/yao/function/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/model.py` & `yao-0.0.4/yao/function/model.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/permission/main.py` & `yao-0.0.4/yao/function/permission/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/permission/schema.py` & `yao-0.0.4/yao/function/permission/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/user/crud.py` & `yao-0.0.4/yao/function/user/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/user/main.py` & `yao-0.0.4/yao/function/user/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/function/user/schema.py` & `yao-0.0.4/yao/function/user/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/helpers.py` & `yao-0.0.4/yao/helpers.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/method.py` & `yao-0.0.4/yao/method.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.3/yao/schema.py` & `yao-0.0.4/yao/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union
+from typing import Optional, Union, List
 
 from pydantic import BaseModel, validator
 
 from config import SCHEMAS_SUCCESS_CODE, SCHEMAS_SUCCESS_STATUS, SCHEMAS_SUCCESS_MESSAGE, SCHEMAS_ERROR_CODE, SCHEMAS_ERROR_STATUS, SCHEMAS_ERROR_MESSAGE
 
 
 class Schemas(BaseModel):
@@ -56,7 +56,11 @@
 
 
 class SchemaParamsApi(SchemaPrefixNames):
     uuid: Optional[str] = None
 
     class Config:
         orm_mode = True
+
+
+class ModelUUIDS(BaseModel):
+    uuids: List[str] = None
```

### Comparing `yao-0.0.3/yao.egg-info/SOURCES.txt` & `yao-0.0.4/yao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

