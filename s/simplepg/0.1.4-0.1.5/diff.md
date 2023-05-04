# Comparing `tmp/simplepg-0.1.4.tar.gz` & `tmp/simplepg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplepg-0.1.4.tar", max compression
+gzip compressed data, was "simplepg-0.1.5.tar", max compression
```

## Comparing `simplepg-0.1.4.tar` & `simplepg-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10255 2023-01-03 08:38:50.251480 simplepg-0.1.4/LICENSE
--rw-r--r--   0        0        0      794 2023-05-02 13:51:42.564005 simplepg-0.1.4/README.md
--rw-r--r--   0        0        0     1214 2023-05-02 13:58:33.235465 simplepg-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       64 2023-01-03 08:40:33.148344 simplepg-0.1.4/simplepg/__init__.py
--rw-r--r--   0        0        0     6286 2023-05-02 13:57:41.082518 simplepg-0.1.4/simplepg/db.py
--rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 simplepg-0.1.4/setup.py
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 simplepg-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10255 2023-01-03 08:38:50.251480 simplepg-0.1.5/LICENSE
+-rw-r--r--   0        0        0      794 2023-05-02 13:51:42.564005 simplepg-0.1.5/README.md
+-rw-r--r--   0        0        0     1214 2023-05-04 12:57:55.445241 simplepg-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-01-03 08:40:33.148344 simplepg-0.1.5/simplepg/__init__.py
+-rw-r--r--   0        0        0     7023 2023-05-04 13:04:40.148648 simplepg-0.1.5/simplepg/db.py
+-rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 simplepg-0.1.5/setup.py
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 simplepg-0.1.5/PKG-INFO
```

### Comparing `simplepg-0.1.4/LICENSE` & `simplepg-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simplepg-0.1.4/README.md` & `simplepg-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `simplepg-0.1.4/pyproject.toml` & `simplepg-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplepg"
-version = "0.1.4"
+version = "0.1.5"
 description = "Simple PostgreSQL connections"
 authors = ["Mysterious Ben <datascience@tuta.io>"]
 exclude = [".git", ".gitignore", ".venv/", ".mypy_cache/", "__pycache__", ".eggs/"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `simplepg-0.1.4/simplepg/db.py` & `simplepg-0.1.5/simplepg/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 from contextlib import contextmanager
+from threading import Semaphore
 from time import sleep
 from typing import Callable, Dict, List, NamedTuple, Optional, Tuple, Union
 
 import psycopg2
 from loguru import logger
 from psycopg2 import pool
 from psycopg2.errors import InterfaceError, OperationalError
@@ -41,14 +42,36 @@
     records: List
     columns: List[str]
 
     def as_records(self) -> List[Dict]:
         return [dict(zip(self.columns, x)) for x in self.records]
 
 
+class ThreadedConnectionPool(pool.ThreadedConnectionPool):
+    """ThreadedConnectionPool with a semaphore to limit the number of connections"""
+
+    def __init__(self, minconn, maxconn, *args, **kwargs):
+        self._semaphore = Semaphore(maxconn)
+        super().__init__(minconn, maxconn, *args, **kwargs)
+
+    def getconn(self, *args, **kwargs):
+        self._semaphore.acquire()
+        try:
+            return super().getconn(*args, **kwargs)
+        except Exception as e:
+            self._semaphore.release()
+            raise e
+
+    def putconn(self, *args, **kwargs):
+        try:
+            super().putconn(*args, **kwargs)
+        finally:
+            self._semaphore.release()
+
+
 class DbConnection:
     """Postgres DB connection manager"""
 
     def __init__(
         self,
         user: str,
         password: str,
@@ -76,30 +99,30 @@
         """
 
         self.psycopg2_url = f"postgresql://{user}:{password}@{host}:{port}/{database}"
         self.connect_kwargs = connect_kwargs
         self.pool_min_connections = pool_min_connections
         self.pool_max_connections = pool_max_connections
         # self._conn = psycopg2.connect(self._psycopg2_url, **self._connect_kwargs)
-        self._conn_pool = pool.ThreadedConnectionPool(
+        self._conn_pool = ThreadedConnectionPool(
             self.pool_min_connections,
             self.pool_max_connections,
             self.psycopg2_url,
             **self.connect_kwargs,
         )
         self.postgres_reconnect_delay = postgres_reconnect_delay
 
     def is_valid(self) -> bool:
         return True
 
     def _reconnect(self):
         # self._conn.close()
         # self._conn = psycopg2.connect(self._psycopg2_url, **self._connect_kwargs)
         self._conn_pool.closeall()
-        self._conn_pool = pool.ThreadedConnectionPool(
+        self._conn_pool = ThreadedConnectionPool(
             self.pool_min_connections,
             self.pool_max_connections,
             self.psycopg2_url,
             **self.connect_kwargs,
         )
 
     @property
@@ -109,15 +132,16 @@
         try:
             yield conn
         except Exception as e:
             conn.rollback()
             raise e
         else:
             conn.commit()
-        self._conn_pool.putconn(conn)
+        finally:
+            self._conn_pool.putconn(conn)
 
     @_reconnect_retry
     def execute(self, sql: str, vars_: Optional[Union[List, Dict]] = None) -> int:
         """Execute an arbitrary SQL query
 
         Args:
             sql: an SQL statement
```

### Comparing `simplepg-0.1.4/setup.py` & `simplepg-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['loguru>=0.5.0,<0.6.0', 'psycopg2>=2.9.5,<3.0.0']
 
 setup_kwargs = {
     'name': 'simplepg',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Simple PostgreSQL connections',
     'long_description': '# SimplePG\n\nSimple PostgreSQL connections: a wrapper around psycopg2.\n\nFeatures:\n- Thread-safe connection pooling\n- Auto-reconnect on connection loss\n- Unified interface for execute, executemany, and execute_values\n\n## Installation\n\n```bash\npip install simplepg\n```\n\n## Example\n\n```python\nfrom simplepg import DbConnection\n\ndb = DbConnection(\n    user="postgres",\n    password="postgres",\n    host="localhost",\n    port=5432,\n    database="postgres",\n    connect_kwargs={},\n    pool_min_connections=1,\n    pool_max_connections=1,\n)\n\ndb.execute("CREATE TABLE test_table (id SERIAL PRIMARY KEY, name VARCHAR)")\ndb.execute_values("INSERT INTO test_table (name) VALUES %s", [("test1",), ("test2",)])\nrecords, columns = db.execute("SELECT * FROM test_table")\ndb.execute("DROP TABLE test_table")\n```\n',
     'author': 'Mysterious Ben',
     'author_email': 'datascience@tuta.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `simplepg-0.1.4/PKG-INFO` & `simplepg-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplepg
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple PostgreSQL connections
 License: Apache-2.0
 Author: Mysterious Ben
 Author-email: datascience@tuta.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

