# Comparing `tmp/fastapi_sql-0.3.6.tar.gz` & `tmp/fastapi_sql-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sql-0.3.6.tar", max compression
+gzip compressed data, was "fastapi_sql-0.3.7.tar", max compression
```

## Comparing `fastapi_sql-0.3.6.tar` & `fastapi_sql-0.3.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4091 2023-05-04 00:55:04.885829 fastapi_sql-0.3.6/fastapi_sql/__init__.py
--rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.6/fastapi_sql/middleware.py
--rw-r--r--   0        0        0     1787 2023-05-03 22:30:34.614632 fastapi_sql-0.3.6/fastapi_sql/migrate.py
--rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.6/fastapi_sql/model.py
--rw-r--r--   0        0        0      858 2023-05-03 22:45:05.948485 fastapi_sql-0.3.6/fastapi_sql/table.py
--rw-r--r--   0        0        0      417 2023-05-04 00:50:29.782073 fastapi_sql-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     4121 2023-05-04 01:14:02.125670 fastapi_sql-0.3.7/fastapi_sql/__init__.py
+-rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.7/fastapi_sql/middleware.py
+-rw-r--r--   0        0        0     1787 2023-05-03 22:30:34.614632 fastapi_sql-0.3.7/fastapi_sql/migrate.py
+-rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.7/fastapi_sql/model.py
+-rw-r--r--   0        0        0      858 2023-05-03 22:45:05.948485 fastapi_sql-0.3.7/fastapi_sql/table.py
+-rw-r--r--   0        0        0      417 2023-05-04 01:20:50.614458 fastapi_sql-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.7/PKG-INFO
```

### Comparing `fastapi_sql-0.3.6/fastapi_sql/__init__.py` & `fastapi_sql-0.3.7/fastapi_sql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Any, Type
 
-from fastapi import FastAPI
 import sqlalchemy as sa
+from fastapi import FastAPI
 from sqlalchemy import (Boolean, Column, Date, DateTime, ForeignKey, Integer,
                         MetaData, String, Text, select)
 from sqlalchemy.ext.asyncio import (AsyncEngine, AsyncSession,
                                     async_sessionmaker, create_async_engine)
-from sqlalchemy.orm import RelationshipProperty, declarative_base, relationship
+from sqlalchemy.orm import (RelationshipProperty, backref, declarative_base,
+                            relationship)
 from sqlalchemy.sql import Select
 
 from .middleware import Middleware
 from .migrate import Migration
 from .model import DefaultMeta
 from .model import Model as DefaultModel
 from .table import _Table
@@ -29,31 +30,32 @@
         "pk": "pk_%(table_name)s"
     }
     
     middleware = Middleware
     
     Model: DefaultModel
     ForeignKey = ForeignKey
+    backref = backref
     
     Column = Column
     Boolean = Boolean
     Integer = Integer
     Text = Text
     String = String
     DateTime = DateTime
     Date = Date
+    
     def relationship(
         self, *args: Any, **kwargs: Any
     ) -> RelationshipProperty[Any]:
         """A :func:`sqlalchemy.orm.relationship` that applies this extension's
         :attr:`Query` class for dynamic relationships and backrefs.
         .. versionchanged:: 3.0
             The :attr:`Query` class is set on ``backref``.
         """
-        self._set_rel_query(kwargs)
         return relationship(*args, **kwargs)
     
     def __init__(self, app: FastAPI = None, *, database_uri: str, session_options: 'dict[str,Any]' = {}, **kwargs
     ):
         self.__engine__ = create_async_engine(database_uri)
         self.__sessionmaker__ = async_sessionmaker(
                     bind=self.__engine__,
```

### Comparing `fastapi_sql-0.3.6/fastapi_sql/middleware.py` & `fastapi_sql-0.3.7/fastapi_sql/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.6/fastapi_sql/migrate.py` & `fastapi_sql-0.3.7/fastapi_sql/migrate.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.6/fastapi_sql/model.py` & `fastapi_sql-0.3.7/fastapi_sql/model.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.6/fastapi_sql/table.py` & `fastapi_sql-0.3.7/fastapi_sql/table.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.6/PKG-INFO` & `fastapi_sql-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

