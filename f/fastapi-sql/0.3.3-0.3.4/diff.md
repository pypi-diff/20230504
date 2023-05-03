# Comparing `tmp/fastapi_sql-0.3.3.tar.gz` & `tmp/fastapi_sql-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sql-0.3.3.tar", max compression
+gzip compressed data, was "fastapi_sql-0.3.4.tar", max compression
```

## Comparing `fastapi_sql-0.3.3.tar` & `fastapi_sql-0.3.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2818 2023-05-03 16:42:04.761041 fastapi_sql-0.3.3/fastapi_sql/__init__.py
--rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.3/fastapi_sql/middleware.py
--rw-r--r--   0        0        0     1562 2023-04-29 15:43:30.819501 fastapi_sql-0.3.3/fastapi_sql/migrate.py
--rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.3/fastapi_sql/model.py
--rw-r--r--   0        0        0      417 2023-05-03 16:44:48.822864 fastapi_sql-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2933 2023-05-03 16:51:12.607686 fastapi_sql-0.3.4/fastapi_sql/__init__.py
+-rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.4/fastapi_sql/middleware.py
+-rw-r--r--   0        0        0     1562 2023-04-29 15:43:30.819501 fastapi_sql-0.3.4/fastapi_sql/migrate.py
+-rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.4/fastapi_sql/model.py
+-rw-r--r--   0        0        0      417 2023-05-03 16:51:32.403696 fastapi_sql-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.4/PKG-INFO
```

### Comparing `fastapi_sql-0.3.3/fastapi_sql/__init__.py` & `fastapi_sql-0.3.4/fastapi_sql/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import Any, Type
 
-from sqlalchemy.ext.asyncio import (AsyncEngine, AsyncSession, async_sessionmaker,
-                                    create_async_engine)
-from sqlalchemy import MetaData, Table, Column, Integer, Text, String, DateTime, Date, select, ForeignKey
-from sqlalchemy.sql import Select
-from sqlalchemy.orm import declarative_base
-from .model import Model as DefaultModel, DefaultMeta
-from .migrate import Migration
 from fastapi import FastAPI
+from sqlalchemy import (Boolean, Column, Date, DateTime, ForeignKey, Integer,
+                        MetaData, String, Text, select)
+from sqlalchemy.ext.asyncio import (AsyncEngine, AsyncSession,
+                                    async_sessionmaker, create_async_engine)
+from sqlalchemy.orm import declarative_base, relationship
+from sqlalchemy.sql import Select
+
 from .middleware import Middleware
+from .migrate import Migration
+from .model import DefaultMeta
+from .model import Model as DefaultModel
 
 
 class SQLAlchemy:
     __engine__: AsyncEngine
     session: AsyncSession
     __metadata__: MetaData = None
     migration = Migration
@@ -26,19 +29,21 @@
     
     middleware = Middleware
     
     Model: DefaultModel
     ForeignKey = ForeignKey
     
     Column = Column
+    Boolean = Boolean
     Integer = Integer
     Text = Text
     String = String
     DateTime = DateTime
     Date = Date
+    relationship = relationship
     
     def __init__(self, app: FastAPI = None, *, database_uri: str, session_options: 'dict[str,Any]' = {}, **kwargs
     ):
         self.__engine__ = create_async_engine(database_uri)
         self.__sessionmaker__ = async_sessionmaker(
                     bind=self.__engine__, 
                     autoflush=session_options.get('session_autoflush', True),
```

### Comparing `fastapi_sql-0.3.3/fastapi_sql/middleware.py` & `fastapi_sql-0.3.4/fastapi_sql/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.3/fastapi_sql/migrate.py` & `fastapi_sql-0.3.4/fastapi_sql/migrate.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.3/fastapi_sql/model.py` & `fastapi_sql-0.3.4/fastapi_sql/model.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.3/PKG-INFO` & `fastapi_sql-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

