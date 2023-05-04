# Comparing `tmp/fastapi_sql-0.3.5.tar.gz` & `tmp/fastapi_sql-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sql-0.3.5.tar", max compression
+gzip compressed data, was "fastapi_sql-0.3.6.tar", max compression
```

## Comparing `fastapi_sql-0.3.5.tar` & `fastapi_sql-0.3.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     3352 2023-05-03 22:30:11.099145 fastapi_sql-0.3.5/fastapi_sql/__init__.py
--rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.5/fastapi_sql/middleware.py
--rw-r--r--   0        0        0     1787 2023-05-03 22:30:34.614632 fastapi_sql-0.3.5/fastapi_sql/migrate.py
--rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.5/fastapi_sql/model.py
--rw-r--r--   0        0        0      417 2023-05-03 22:35:01.229016 fastapi_sql-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     4091 2023-05-04 00:55:04.885829 fastapi_sql-0.3.6/fastapi_sql/__init__.py
+-rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.6/fastapi_sql/middleware.py
+-rw-r--r--   0        0        0     1787 2023-05-03 22:30:34.614632 fastapi_sql-0.3.6/fastapi_sql/migrate.py
+-rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.6/fastapi_sql/model.py
+-rw-r--r--   0        0        0      858 2023-05-03 22:45:05.948485 fastapi_sql-0.3.6/fastapi_sql/table.py
+-rw-r--r--   0        0        0      417 2023-05-04 00:50:29.782073 fastapi_sql-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.6/PKG-INFO
```

### Comparing `fastapi_sql-0.3.5/fastapi_sql/__init__.py` & `fastapi_sql-0.3.6/fastapi_sql/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import Any, Type
 
 from fastapi import FastAPI
+import sqlalchemy as sa
 from sqlalchemy import (Boolean, Column, Date, DateTime, ForeignKey, Integer,
                         MetaData, String, Text, select)
 from sqlalchemy.ext.asyncio import (AsyncEngine, AsyncSession,
                                     async_sessionmaker, create_async_engine)
-from sqlalchemy.orm import declarative_base, relationship, RelationshipProperty
+from sqlalchemy.orm import RelationshipProperty, declarative_base, relationship
 from sqlalchemy.sql import Select
 
 from .middleware import Middleware
 from .migrate import Migration
 from .model import DefaultMeta
 from .model import Model as DefaultModel
+from .table import _Table
 
 
 class SQLAlchemy:
     __engine__: AsyncEngine
     session: AsyncSession
     __metadata__: MetaData = None
     migration = Migration
@@ -59,14 +61,15 @@
                     expire_on_commit=session_options.get('expire_on_commit', True)
         )
         if kwargs.get('naming_convention') is not None:
             self.__naming_conventions__ = kwargs.get('naming_convention', {})
         if SQLAlchemy.__metadata__ is None:
             SQLAlchemy.__metadata__ = MetaData(naming_convention=self.__naming_conventions__)
         self.Model = self._make_declarative_base() # type: ignore
+        self.Table = self._make_table_class()
         self.__engine_uri__ = database_uri
         self.migration.cfg.set_main_option('sqlalchemy.url', database_uri)
         self.migration.cfg.config_file_name = 'alembic.ini'
         if app is not None:
             app.add_middleware(self.middleware, sqlalchemy=self)
             
     def init_app(self, app: FastAPI):
@@ -81,8 +84,23 @@
     def _make_declarative_base(self) -> 'type[DefaultModel]':
         model = declarative_base(
             metadata=self.__metadata__,
             cls=DefaultModel,
             name="Model",
             metaclass=DefaultMeta # type: ignore
         )
-        return model
+        return model
+    
+    def _make_table_class(self):
+        class Table(_Table):
+            def __new__(
+                cls, *args: Any, bind_key: str = None, **kwargs: Any
+            ) -> sa.Table:
+                # If a metadata arg is passed, go directly to the base Table. Also do
+                # this for no args so the correct error is shown.
+                if not args or (len(args) >= 2 and isinstance(args[1], MetaData)):
+                    return super().__new__(cls, *args, **kwargs)
+
+                metadata = self.__metadata__
+                return super().__new__(cls, *[args[0], metadata, *args[1:]], **kwargs)
+
+        return Table
```

### Comparing `fastapi_sql-0.3.5/fastapi_sql/middleware.py` & `fastapi_sql-0.3.6/fastapi_sql/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.5/fastapi_sql/migrate.py` & `fastapi_sql-0.3.6/fastapi_sql/migrate.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.5/fastapi_sql/model.py` & `fastapi_sql-0.3.6/fastapi_sql/model.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.5/PKG-INFO` & `fastapi_sql-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

