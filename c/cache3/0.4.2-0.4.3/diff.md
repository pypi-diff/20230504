# Comparing `tmp/cache3-0.4.2.tar.gz` & `tmp/cache3-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cache3-0.4.2.tar", last modified: Wed Apr  5 03:51:24 2023, max compression
+gzip compressed data, was "cache3-0.4.3.tar", last modified: Thu May  4 17:50:44 2023, max compression
```

## Comparing `cache3-0.4.2.tar` & `cache3-0.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:51:24.832330 cache3-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-05 03:51:15.000000 cache3-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-05 03:51:24.832330 cache3-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-05 03:51:15.000000 cache3-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-05 03:51:24.836330 cache3-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-05 03:51:15.000000 cache3-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:51:24.828330 cache3-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:51:24.832330 cache3-0.4.2/src/cache3/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-05 03:51:15.000000 cache3-0.4.2/src/cache3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33850 2023-04-05 03:51:15.000000 cache3-0.4.2/src/cache3/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-04-05 03:51:15.000000 cache3-0.4.2/src/cache3/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-05 03:51:15.000000 cache3-0.4.2/src/cache3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:51:24.832330 cache3-0.4.2/src/cache3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-05 03:51:24.000000 cache3-0.4.2/src/cache3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-05 03:51:24.000000 cache3-0.4.2/src/cache3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 03:51:24.000000 cache3-0.4.2/src/cache3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 03:51:24.000000 cache3-0.4.2/src/cache3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 03:51:24.832330 cache3-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-04-05 03:51:15.000000 cache3-0.4.2/tests/test_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-05 03:51:15.000000 cache3-0.4.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-04-05 03:51:15.000000 cache3-0.4.2/tests/test_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-05 03:51:15.000000 cache3-0.4.2/tests/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-05 03:51:15.000000 cache3-0.4.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:50:44.943087 cache3-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 17:50:32.000000 cache3-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-04 17:50:44.943087 cache3-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-04 17:50:32.000000 cache3-0.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-04 17:50:44.947088 cache3-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-04 17:50:32.000000 cache3-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:50:44.943087 cache3-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:50:44.943087 cache3-0.4.3/src/cache3/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 17:50:32.000000 cache3-0.4.3/src/cache3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35535 2023-05-04 17:50:32.000000 cache3-0.4.3/src/cache3/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-05-04 17:50:32.000000 cache3-0.4.3/src/cache3/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-04 17:50:32.000000 cache3-0.4.3/src/cache3/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:50:44.943087 cache3-0.4.3/src/cache3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-04 17:50:44.000000 cache3-0.4.3/src/cache3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-04 17:50:44.000000 cache3-0.4.3/src/cache3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:50:44.000000 cache3-0.4.3/src/cache3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 17:50:44.000000 cache3-0.4.3/src/cache3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:50:44.943087 cache3-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-05-04 17:50:32.000000 cache3-0.4.3/tests/test_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-04 17:50:32.000000 cache3-0.4.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-04 17:50:32.000000 cache3-0.4.3/tests/test_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-04 17:50:32.000000 cache3-0.4.3/tests/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-04 17:50:32.000000 cache3-0.4.3/tests/test_utils.py
```

### Comparing `cache3-0.4.2/LICENSE` & `cache3-0.4.3/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021-2024 clarkmonkey@163.com
+Copyright (c) 2021-2023 clarkmonkey@163.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `cache3-0.4.2/PKG-INFO` & `cache3-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cache3
-Version: 0.4.2
+Version: 0.4.3
 Summary: A safe and lightweight cache library, written in pure-Python.
 Home-page: https://github.com/StKali/cache3
 Author: attr: cache3.__author__
 Author-email: clarkmonkey@163.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
@@ -23,15 +23,15 @@
 ===============================
 
 **cache3** is a MIT licensed  safe and lightweight cache library, written
 in pure-Python.
 
 .. image:: https://img.shields.io/badge/LICENSE-MIT-green
     :target: https://github.com/StKali/cache3/blob/master/LICENSE
-.. image:: https://img.shields.io/badge/version-0.3.3-informational
+.. image:: https://img.shields.io/badge/version-0.4.3-informational
     :target: https://pypi.org/project/cache3
 .. image:: https://img.shields.io/badge/python-3.5+-blueviolet
     :target: https://www.python.org
 
 cache3 is very tiny and completely implemented by the Python standard library without any third-party dependencies, so it can be easily embedded in any Python program or script.
 
 Installing
@@ -73,10 +73,10 @@
 - Source Code: https://github.com/StKali/cache3
 
 - Issue Tracker: https://github.com/StKali/cache3/issues
 
 License
 =======
 
-Copyright (c) 2020-2021 clarkmonkey@163.com
+Copyright (c) 2020-2023 clarkmonkey@163.com
 Licensed under the MIT License.
```

### Comparing `cache3-0.4.2/README.rst` & `cache3-0.4.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ===============================
 
 **cache3** is a MIT licensed  safe and lightweight cache library, written
 in pure-Python.
 
 .. image:: https://img.shields.io/badge/LICENSE-MIT-green
     :target: https://github.com/StKali/cache3/blob/master/LICENSE
-.. image:: https://img.shields.io/badge/version-0.3.3-informational
+.. image:: https://img.shields.io/badge/version-0.4.3-informational
     :target: https://pypi.org/project/cache3
 .. image:: https://img.shields.io/badge/python-3.5+-blueviolet
     :target: https://www.python.org
 
 cache3 is very tiny and completely implemented by the Python standard library without any third-party dependencies, so it can be easily embedded in any Python program or script.
 
 Installing
@@ -52,10 +52,10 @@
 - Source Code: https://github.com/StKali/cache3
 
 - Issue Tracker: https://github.com/StKali/cache3/issues
 
 License
 =======
 
-Copyright (c) 2020-2021 clarkmonkey@163.com
+Copyright (c) 2020-2023 clarkmonkey@163.com
 Licensed under the MIT License.
```

### Comparing `cache3-0.4.2/setup.cfg` & `cache3-0.4.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -26,20 +26,14 @@
 	= src
 packages = find:
 python_requires > = 3.5
 
 [options.packages.find]
 where = src
 
-[flake8]
-max-line-length = 100
-exclude = .git, .tox, build
-select = C, E, F, W, B, B950, I, N
-ignore = F401, E501
-
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [egg_info]
 tag_build =
```

### Comparing `cache3-0.4.2/src/cache3/__init__.py` & `cache3-0.4.3/src/cache3/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-# DATE: 2021/7/24
-# Author: clarkmonkey@163.com
+# date: 2021/7/24
+# author: clarkmonkey@163.com
 
 """
 Cache3 is a MIT licensed  safe and lightweight cache library, written in pure-Python.
 """
 
-from cache3.utils import lazy, LazyObject
+from cache3.util import lazy, LazyObject
 from cache3.disk import DiskCache, LazyDiskCache
 from cache3.memory import Cache, MiniCache, LazyCache
 
 __author__: str = 'St·Kali <clarkmonkey@163.com>'
-__name__: str = 'cache3'
+__name__: str = 'cache3'  # pylint: disable=redefined-builtin
 __email__: str = 'clarkmonkey@163.com'
-__version__: str = '0.4.2'
+__version__: str = '0.4.3'
 
 __all__: list = [
     'DiskCache', 'LazyDiskCache',
     'Cache', 'MiniCache', 'LazyCache',
     'LazyObject', 'lazy',
 ]
-
```

### Comparing `cache3-0.4.2/src/cache3/disk.py` & `cache3-0.4.3/src/cache3/disk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-# DATE: 2021/9/15
-# Author: clarkmonkey@163.com
+# date: 2021/9/15
+# author: clarkmonkey@163.com
 
 """ DiskCache
 
 SQLite and file system based caching.
 
 Provides the APIs of general caching systems. 
 At the same time, all data is stored in the disk (sqlite or data file), 
 so the inter-process data is safe and durable.
 
 The pickle protocol is used to complete the serialization and deserialization 
 of data. Can satisfy most objects in python.
 
-The cache elimination strategy is optional, and currently supports LRU, LFU, 
+The cache eviction policies are optional, and currently supports LRU, LFU,
 and FIFO. If these don't meet your needs, you can register your own cache 
 eviction policies by `evict_manager.register`.
 """
 
 import abc
 import pickle
 import warnings
-import functools
 import sys
 from contextlib import contextmanager
 from pathlib import Path
 from sqlite3.dbapi2 import Connection, Cursor, OperationalError
 from threading import local, get_ident
 from time import time as current, sleep
 from typing import Type, Optional, Dict, Any, List, Tuple, Callable, Iterable
 from os import makedirs, getpid, remove as rmfile, path as op
 from hashlib import md5
-from .utils import (
-    cached_property, empty, lazy, Time, TG, Number, get_expire, Cache3Error, Cache3Warning
+from .util import (
+    cached_property, empty, lazy, Time, TG, Number, get_expire, memoize, Cache3Error, Cache3Warning
 )
 
-
 QY: Type = Callable[[Any], Cursor]
 ROW: Type = Optional[Tuple[Any,...]]
-
 RAW: int = 0
 NUMBER: int = 1
 STRING: int = 2
 BYTES: int = 3
 PICKLE: int = 4
 
-
 if sys.version_info > (3, 10):
     from types import NoneType
 else:
     NoneType: Type = type(None)
 
 # Default filesystem charset
 _default_charset: str = 'UTF-8'
 # Default cache storage path
 _default_directory: str = '~/.cache3'
 # Default sqlite3 filename
 _default_name: str = 'default.sqlite3'
+# Default evict policy
+_default_evict_policy: str = 'lru'
 # SQLite pragma configs
 _default_pragmas: Dict[str, Any] = {
     'auto_vacuum': 1,
     'cache_size': 1 << 13,  # 8, 192 pages
     'journal_mode': 'wal',
     'threads': 4,  # SQLite work threads count
     'temp_store': 2,  # DEFAULT: 0 | FILE: 1 | MEMORY: 2
     'mmap_size': 1 << 26,  # 64MB
     'synchronous': 1,
 }
 
 
-class SQLiteEntry:
+class SQLiteManager:
     """ SQLite3 database interaction interface, responsible for connection management
-    and transaction commission """
+    and transaction commission.
+    """
 
     def __init__(
             self,
             path: str,
             name: str,
             isolation: Optional[str],
             timeout: int,
             pragmas: Optional[Dict[str, Any]] = None,
     ) -> None:
         self.path: str = path
         self.name: str = name
         self.timeout: int = timeout
         self.__local: local = local()
         self.__txn: Optional[int] = None
+        self._txn_id: Optional[int] = None
         self.__connect_configure: Dict[str, Any] = {
             'database': op.join(self.path, self.name),
             'isolation_level': isolation,
             'timeout': timeout
         }
         if not isinstance(pragmas, (dict, NoneType)):
             raise TypeError(
                 f'pragmas want dict object but get {type(pragmas)}'
             )
         self.__pragmas_sql: str = ';'.join(
-            'PRAGMA %s=%s' % item for
+            f'PRAGMA {item[0]}={item[1]}' for
             item in (pragmas or _default_pragmas).items()
         )
         if not self.created:
             init_cache_statements: List[str] = [
                 # cache table
                 'CREATE TABLE IF NOT EXISTS `cache`('
                 '`key` BLOB NOT NULL, '
@@ -120,19 +120,19 @@
 
                 # create info table
                 'CREATE TABLE IF NOT EXISTS `info`('
                 '`key` BLOB NOT NULL, '
                 '`value` BLOB'
                 ')',
 
-                # set count = 0
+                # create unique index
                 'CREATE UNIQUE INDEX IF NOT EXISTS `idx_info_key` '
                 'ON `info`(`key`)',
 
-                #
+                # set count = 0 and evict policy = lru
                 'INSERT INTO `info`(`key`, `value`) VALUES ("count", 0), ("evict", "lru")',
             ]
 
             init_script: str = ';'.join(init_cache_statements)
             _ = self.session.executescript(init_script)
 
     @property
@@ -144,15 +144,15 @@
             ('table', 'cache')
         ).fetchone()
         (count, ) = row
         return count == 1
 
     @property
     def session(self) -> Connection:
-        """ Create a sqlite link, every time you get a link, you need to judge 
+        """ Create a sqlite connection, every time you get a connection, you need to judge
         whether the current connection is independently occupied by a single thread 
         """
         local_pid: int = getattr(self.__local, 'pid', -1)
         current_pid: int = getpid()
         if local_pid != current_pid:
             self.close()
             self.__local.pid = current_pid
@@ -177,24 +177,32 @@
                         raise
                     sleep(0.001)
             # cached connection
             setattr(self.__local, 'session', session)
         return session
 
     def close(self) -> bool:
-
+        """ Close current active connection """
         session: Connection = getattr(self.__local, 'session', None)
         if session is None:
             return True
         session.close()
         setattr(self.__local, 'session', None)
         return True
 
     @contextmanager
     def transact(self, retry: bool = True) -> QY:
+        """ A context manager that will open a SQLite transaction
+
+        Args:
+            retry: Whether to retry until success after a failed transaction
+                rollback.
+        Returns:
+            return a handle to the transaction.
+        """
         sql: QY = self.session.execute
         tid: int = get_ident()
         txn_id: Optional[int] = self.__txn
 
         if tid == txn_id:
             begin: bool = False
         else:
@@ -236,25 +244,30 @@
                 'SELECT `value` ' 
                 'FROM `info` '
                 'WHERE `key` = ?',
                 (key, )
             ).fetchone()
             return row[0] if row else None
         # set
-        else:
-            return self.session.execute(
-                'INSERT INTO `info`(`key`, `value`) '
-                'VALUES (?, ?) '
-                'ON CONFLICT (`key`) '
-                'DO UPDATE SET `value` = ? ',
-                (key, value, value)
-            ).rowcount == 1
+        return self.session.execute(
+            'INSERT INTO `info`(`key`, `value`) '
+            'VALUES (?, ?) '
+            'ON CONFLICT (`key`) '
+            'DO UPDATE SET `value` = ? ',
+            (key, value, value)
+        ).rowcount == 1
 
 
 class PickleStore:
+    """ Determines how Python objects are stored in the DiskCache.
+
+    1) Simple objects will be stored in a way that SQLite natively supports,
+    2) Large or unsupported objects will be converted to Pickle objects and
+    stored as bytecode.
+    """
 
     def __init__(
             self,
             directory: str,
             protocol: int,
             raw_max_size: int,
             charset: str,
@@ -346,19 +359,17 @@
             return None
         with open(file, 'wb') as fd:
             _ = fd.write(data)
 
     def read(self, sig: str) -> Optional[bytes]:
 
         file: str = op.join(self.directory, sig)
-        # FIXME: the value reference by many key(s)
+        # TODO: the value reference by many key(s)
         if not op.exists(file):
-            warnings.warn(
-                f'stored file:{file} not found', Cache3Warning
-            )
+            warnings.warn(f'stored file:{file} not found', Cache3Warning)
             return None
         with open(file, 'rb') as fd:
             return fd.read()
 
     def delete(self, sig: str) -> bool:
         """ delete cached file
 
@@ -374,14 +385,16 @@
             return True
         except OSError:
             return False
 
 
 class EvictInterface(abc.ABC):
 
+    # The name of the cache eviction policy, which is the unique
+    # identifier of the cache in the ``EvictManager``
     name: str = ''
 
     @abc.abstractmethod
     def apply(self, sql: QY) -> bool:
         """ Will be called when the evict policy is set """
 
     @abc.abstractmethod
@@ -472,85 +485,87 @@
             '    ORDER BY `store` LIMIT ?'
             ')',
             (count,)
         ).rowcount
 
 
 class EvictManager(dict):
+    """ Manage all cached data eviction policies. """
 
     def register(self, evict: Type[EvictInterface]) -> None:
+        """ Does not guarantee data concurrent read and write security. """
 
+        # Check if the EvictInterface interface is followed
         if not issubclass(evict, EvictInterface):
             raise Cache3Error(
                 'evict must be inherit `EvictInterface` class'
             )
-
+        # Check if the name already exists
         if evict.name in self:
             raise Cache3Error(
                 f'has been registered evict named {evict.name!r}'
             )
-            
         self[evict.name] = evict
 
     def __missing__(self, key) -> None:
         raise Cache3Error(
             f'no register evict policy named {key!r}'
         )
 
 
-evict_manager = EvictManager({
+evict_manager: EvictManager = EvictManager({
     LRUEvict.name: LRUEvict,
     LFUEvict.name: LFUEvict,
     FIFOEvict.name: FIFOEvict,
 })
 
 
 class DiskCache:
     """ Disk cache based on sqlite and file system """
 
-    def __init__(
+    def __init__(   # pylint: disable=too-many-arguments
             self,
             directory: str = _default_directory,
             name: str = _default_name,
             max_size: int = 1 << 30,
             iter_size: int = 1 << 8,
-            evict_policy: str = 'lru',
+            evict_policy: str = _default_evict_policy,
             evict_size: int = 1 << 6,
             evict_time: Number = 2,
             charset: Optional[str] = None,
             protocol: int = pickle.HIGHEST_PROTOCOL,
             raw_max_size: int = 1 << 17,
             isolation: Optional[str] = None,
-            timeout: Time = 5,
+            timeout: Time = 10 * 60,
             pragmas: Optional[Dict[str, Any]] = None,
 
     ) -> None:
 
         self.directory: str = op.expandvars(op.expanduser(directory))
         if not op.exists(self.directory):
             makedirs(self.directory, exist_ok=True)
         
         self.name: str = name
         self.max_size: int = max_size
         self.evict_size: int = evict_size
         self.evict_time: Number = evict_time
+        self._evict: Optional[EvictInterface] = None
         self.iter_size: int = iter_size
         
-        # sqlite
-        self.sqlite: SQLiteEntry = SQLiteEntry(
+        # config sqlite session manager
+        self.sqlite: SQLiteManager = SQLiteManager(
             path=self.directory, 
             name=name,
             isolation=isolation,
             timeout=timeout,
             pragmas=pragmas or _default_pragmas,
         )
-        self._evict: Optional[EvictInterface] = None
+        # config evict policy
         self.config_evict(evict_policy)
-
-        # pickle storage
+        # config pickle storage
         self.store = PickleStore(
             directory=self.directory,
             protocol=protocol,
             raw_max_size=raw_max_size,
             charset=charset or _default_charset,
         )
 
@@ -563,14 +578,25 @@
             pre_evict: EvictInterface = evict_manager[pre_evict_policy]()
             pre_evict.unapply(sql)
             self._evict.apply(sql)
             self.sqlite.config('evict', evict_policy)
         return True
 
     def set(self, key: Any, value: Any, timeout: Time = None, tag: TG = None) -> bool:
+        """
+
+        Args:
+            key:
+            value:
+            timeout:
+            tag:
+
+        Returns:
+
+        """
 
         sk, kf = self.store.dumps(key)
         with self.sqlite.transact() as sql:
             row = sql(
                 'SELECT `rowid`'
                 'FROM `cache`'
                 'WHERE `key` = ? AND `tag` IS ?',
@@ -579,23 +605,34 @@
             sv, vf = self.store.dumps(value)
 
             # key existed but it is expired
             if row:
                 (rowid, ) = row
                 if self._update_row(sql, rowid, sv, vf, timeout, tag):
                     return True
+
             # key not found in cache
             else:
                 ok: bool = self._create_row(sql, sk, kf, sv, vf, timeout, tag)
                 if ok:
                     self._add_count(sql)
                     self.try_evict(sql)
                 return ok
 
     def get(self, key: Any, default: Any = None, tag: TG = None) -> Any:
+        """
+
+        Args:
+            key:
+            default:
+            tag:
+
+        Returns:
+
+        """
         sk, _ = self.store.dumps(key)
         sql = self.sqlite.session.execute
         row = sql(
             'SELECT `rowid`, `value`, `expire`, `vf` '
             'FROM `cache` '
             'WHERE `key` = ? AND `tag` IS ?',
             (sk, tag)
@@ -604,15 +641,15 @@
         if not row:
             # not found key in cache
             return default
 
         (rowid, sv, expire, vf) = row
         now: Time = current()
         if expire is not None and expire < now:
-            self._sub_count(sql)
+            # self._sub_count(sql)
             # key has expired
             return default
 
         sql(
             'UPDATE `cache` '
             'SET `access_count` = `access_count` + 1, `access` = ? '
             'WHERE `rowid` = ?',
@@ -629,37 +666,46 @@
             consistency of behavior
         """
 
         sks: List[Any] = [self.store.dumps(key)[0] for key in keys]
         snap: str = str('?, ' * len(sks)).strip(', ')
         rs: Cursor = self.sqlite.session.execute(
             'SELECT `key`, `value`, `vf` FROM `cache`'
-            'WHERE `key` IN (%s) AND `tag` IS ? ' % snap,
+            f'WHERE `key` IN ({snap}) AND `tag` IS ? ',
             (*sks, tag)
         )
 
         vs: dict = {sk: self.store.loads(sv, vf) for sk, sv, vf in rs}
-        result: dict = dict()
+        result: dict = {}
         for idx, key in enumerate(keys):
             v = vs.get(sks[idx], empty)
             if v is not empty:
                 result[key] = v
         return result
 
     def incr(self, key: Any, delta: Number = 1, tag: TG = None) -> Number:
-        """ int, float and (str/bytes) not serialize, so add in sql statement.
+        """ Increases the value by delta (default 1)
+
+        int, float and (str/bytes) not serialize, so add in sql statement.
 
         The increment operation should be implemented through SQLite,
         which is not safe at the Python language level
 
+        Args:
+            key: key literal value
+            delta: Increase in size
+
         Returns:
-            increment result value else raise 'Cache3Error' error.
-        """
+            The new value
 
-        sk, kf = self.store.dumps(key)
+        Raises:
+            KeyError: if the key does not exist or has been eliminated
+            TypeError: if value is not a number type
+        """
+        sk, _ = self.store.dumps(key)
         with self.sqlite.transact() as sql:
             row: ROW = sql(
                 'SELECT `value`, `vf` FROM `cache` '
                 'WHERE `key` = ? AND `tag` IS ? '
                 'AND (`expire` IS NULL OR `expire` > ?)',
                 (sk, tag, current())
             ).fetchone()
@@ -716,14 +762,15 @@
             '`expire` = ?, '
             '`access` = ?, '
             '`access_count` = ? '
             'WHERE `rowid` = ?',
             (sv, vf, tag, now, expire, now, 0, rowid)
         ).rowcount == 1
 
+    # pylint: disable=too-many-arguments
     @staticmethod
     def _create_row(sql: QY, sk: Any, kf: int, sv: Any, vf: int, timeout: Time, tag: TG) -> bool:
 
         now: Time = current()
         expire: Time = get_expire(timeout, now)
         return sql(
             'INSERT INTO `cache`('
@@ -752,14 +799,23 @@
         return True
 
     @cached_property
     def location(self) -> str:
         return (Path(self.directory) / self.name).as_posix()
 
     def ttl(self, key: Any, tag: TG = None) -> Time:
+        """
+
+        Args:
+            key:
+            tag:
+
+        Returns:
+
+        """
         sk, _ = self.store.dumps(key)
         row: ROW = self.sqlite.session.execute(
             'SELECT `expire` '
             'FROM `cache` '
             'WHERE `key` = ? '
             'AND `tag` IS ? '
             'AND (`expire` IS NULL OR `expire` > ?)',
@@ -769,14 +825,23 @@
             return -1
         (expire, ) = row
         if expire is None:
             return None
         return expire - current()
 
     def delete(self, key: Any, tag: TG = None) -> bool:
+        """
+
+        Args:
+            key:
+            tag:
+
+        Returns:
+
+        """
 
         sk, _ = self.store.dumps(key)
         with self.sqlite.transact() as sql:
             ok: bool = sql(
                 'DELETE FROM `cache` '
                 'WHERE `key` = ? AND `tag` IS ? ',
                 (sk, tag)
@@ -806,17 +871,26 @@
             row['sk'] = row['key']
             row['key'] = self.store.loads(row['key'], row['kf'])
             row['sv'] = row['value']
             row['value'] = self.store.loads(row['value'], row['vf'])
             return row
 
     def pop(self, key: Any, default: Any = None, tag: TG = None) -> Any:
+        """
+
+        Args:
+            key:
+            default:
+            tag:
+
+        Returns:
 
+        """
         sql: QY = self.sqlite.session.execute
-        sk, kf = self.store.dumps(key)
+        sk, _ = self.store.dumps(key)
         row: ROW = sql(
             'SELECT `rowid`, `value`, `vf` '
             'FROM `cache` '
             'WHERE `key` = ? '
             'AND `tag` IS ? '
             'AND (`expire` IS NULL OR `expire` > ?)',
             (sk, tag, current())
@@ -850,61 +924,42 @@
 
     @property
     def length(self) -> int:
         self.flush_length(current())
         return len(self)
     
     def has_key(self, key: Any, tag: TG = None) -> bool:
-        sk, kf = self.store.dumps(key)
+        """ Return True if the key in cache else False. """
+        sk, _ = self.store.dumps(key)
         return bool(self.sqlite.session.execute(
             'SELECT 1 FROM `cache` '
             'WHERE `key` = ? '
             'AND `tag` IS ? '
             'AND (`expire` IS NULL OR `expire` > ?)',
             (sk, tag, current())
         ).fetchone())
 
-    def touch(self, key: str, timeout: Time = None, tag: TG = None) -> bool:
+    def touch(self, key: Any, timeout: Time = None, tag: TG = None) -> bool:
         """ Renew the key. When the key does not exist, false will be returned """
         now: Time = current()
         new_expire: Time = get_expire(timeout, now)
         sk, _ = self.store.dumps(key)
         with self.sqlite.transact() as sql:
             return sql(
                 'UPDATE `cache` SET `expire` = ? '
                 'WHERE `key` = ? '
                 'AND `tag` IS ? '
                 'AND (`expire` IS NULL OR `expire` > ?)',
                 (new_expire, sk, tag, now)
             ).rowcount == 1
 
-    def memoize(self, timeout: Time = 24 * 60 * 60, tag: TG = None) -> Any:
-        """ The cache is decorated with the return value of the function,
-        and the timeout is available. """
-
-        def decorator(func: Optional[Callable] = None) -> Callable[[Callable[[Any], Any]], Any]:
-            """ Decorator created by memoize() for callable `func`."""
-            if not callable(func):
-                raise TypeError(
-                    'The `memoize` decorator should be called with a `timeout` parameter.'
-                )
-            @functools.wraps(func)
-            def wrapper(*args, **kwargs) -> Any:
-                """Wrapper for callable to cache arguments and return values."""
-                value: Any = self.get(func.__name__, empty, tag)
-                if value is empty:
-                    value: Any = func(*args, **kwargs)
-                    self.set(func.__name__, value, timeout, tag)
-                return value
-            return wrapper
-
-        return decorator
-
     def ex_set(self, key: Any, value: Any, timeout: Time = None, tag: TG = None) -> bool:
-
+        """ Write the key-value relationship when the data does not exist in the cache,
+        otherwise the set operation will be cancelled
+        """
         sk, kf = self.store.dumps(key)
         with self.sqlite.transact() as sql:
             row = sql(
                 'SELECT `rowid`, `expire` '
                 'FROM `cache` '
                 'WHERE `key` = ? '
                 'AND `tag` IS ?',
@@ -912,37 +967,40 @@
             ).fetchone()
             if row:
                 (rowid, expire) = row
                 if expire is None or expire > current():
                     return False
                 sv, vf = self.store.dumps(value)
                 return self._update_row(sql, rowid, sv, vf, timeout, tag)
-            else:
-                sv, vf = self.store.dumps(value)
-                ok: bool = self._create_row(sql, sk, kf, sv, vf, timeout, tag)
-                if ok:
-                    self._add_count(sql)
-                    self.try_evict(sql)
-                return ok
+            sv, vf = self.store.dumps(value)
+            ok: bool = self._create_row(sql, sk, kf, sv, vf, timeout, tag)
+            if ok:
+                self._add_count(sql)
+                self.try_evict(sql)
+            return ok
 
     def try_evict(self, sql) -> None:
+        """ try to evict expired data """
         if len(self) < self.max_size:
             return
         now: Time = current()
         sql(
             'DELETE FROM `cache` '
             'WHERE `expire` IS NOT NULL '
             'AND `expire` < ?',
             (now,)
         )
         self.flush_length(now)
         if len(self) >= self.max_size:
             _: int = self._evict.evict(sql, self.evict_size)
             
     def keys(self, tag: TG = empty) -> Iterable[Tuple[Any, str]]:
+        """ Returns all keys when tag is specified, otherwise it
+        returns both key and tag
+        """
         now: Time = current()
         n: int = self.length // self.iter_size + 1
         sql: QY = self.sqlite.session.execute
         if tag is empty:
             for i in range(n):
                 for line in sql(
                     'SELECT `key`, `kf`, `tag` '
@@ -964,15 +1022,18 @@
                     'ORDER BY `store` '
                     'LIMIT ? OFFSET ?',
                     (now, tag, self.iter_size, self.iter_size * i)
                 ):
                     if line:
                         yield self.store.loads(*line[:2])
 
-    def values(self, tag: TG = empty) -> Iterable[Tuple[Any, str]]:
+    def values(self, tag: TG = empty) -> Iterable[Tuple]:
+        """ Returns all values when tag is specified, otherwise it
+        returns both value and tag
+        """
         now: Time = current()
         n: int = self.length // self.iter_size + 1
         sql: QY = self.sqlite.session.execute
         if tag is empty:
             for i in range(n):
                 for line in sql(
                     'SELECT `value`, `vf`, `tag` '
@@ -994,16 +1055,22 @@
                     'ORDER BY `store` '
                     'LIMIT ? OFFSET ? ',
                     (now, tag, self.iter_size, self.iter_size * i)
                 ):
                     if line:
                         yield self.store.loads(*line)
 
-    def items(self, tag: TG = empty) -> Iterable[Tuple[Any, Any, str]]:
-        
+    def items(self, tag: TG = empty) -> Iterable[Tuple]:
+        """ Returns all key-value relationships under the tag namespace in
+        the cache database when tag is specified.
+        Otherwise, all key-value-tags in the database are returned.
+
+        Note: that whether tag is specified or not will determine the difference
+        in the return value
+        """
         now: Time = current()
         n: int = self.length // self.iter_size + 1
         sql: QY = self.sqlite.session.execute
         if tag is empty:
             for i in range(n):
                 for line in sql(
                     'SELECT `key`, `kf`, `value`, `vf`, `tag` '
@@ -1031,19 +1098,20 @@
 
     def __len__(self) -> int:
         (length, ) = self.sqlite.session.execute(
             'SELECT `value` '
             'FROM `info` '
             'WHERE `key` = "count"',
         ).fetchone()
-        return length
+        return length if length > 0 else 0
 
     def __repr__(self) -> str:
         return f'<DiskCache: {self.location}>'
 
+    memoize = memoize
     __delitem__ = delete
     __getitem__ = get
     __setitem__ = set
     __iter__ = keys
     __contains__ = has_key
```

### Comparing `cache3-0.4.2/src/cache3/memory.py` & `cache3-0.4.3/src/cache3/memory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-# DATE: 2021/7/24
-# Author: clarkmonkey@163.com
+# date: 2021/7/24
+# author: clarkmonkey@163.com
+
+""" memory
+
+"""
+
 import functools
 from collections import OrderedDict
 from contextlib import AbstractContextManager
 from threading import Lock
 from time import time as current
 from typing import Dict, Any, Iterable, Type, Optional, NoReturn, Tuple, Union, Callable, List
 
-from .utils import Time, TG, Number, get_expire, empty, lazy
+from .util import Time, TG, Number, get_expire, empty, lazy, memoize
 
 
 class NullContext(AbstractContextManager):
     """ Context manager that does no additional processing.
 
     Used as a stand-in for a normal context manager, when a particular
     block of code is only sometimes used with a normal context manager:
@@ -31,14 +36,19 @@
 
 
 LK: Type = Union[NullContext, Lock]
 SK: Type = Tuple[Any, TG]
 
 
 class MiniCache:
+    """ A simple dictionary-based in-memory cache that supports automatic
+    data elimination and does not support tag.
+
+    Cache is built based on minicache, but cache is tag-supported.
+    """
 
     def __init__(self, 
                 name: str, 
                 max_size: int = 1 << 30, 
                 evict_size: int = 16, 
                 evict_policy: str = 'lru',
                 thread_safe: bool = True,
@@ -66,15 +76,16 @@
 
     def get_many(self, keys: List[Any]) -> dict:
         res: dict = {} 
         with self._lock:
             for key in keys:
                 if self._has_expired(key):
                     self._del(key)
-            res[key] = self._cache[key]
+                else:
+                    res[key] = self._cache[key]
         return res
 
     def ex_set(self, key: Any, value: Any, timeout: Time = None) -> bool:
 
         with self._lock:
             if self._has_expired(key):
                 self._set(key, value, get_expire(timeout))
@@ -110,22 +121,25 @@
                     value: Any = func(*args, **kwargs)
                     self.set(func.__name__, value, timeout)
                 return value
             return wrapper
         return decorator
 
     def incr(self, key: Any, delta: Number = 1) -> Number:
+        """ Increases the value by delta (default 1) """
+
         with self._lock:
             if self._has_expired(key):
                 self._del(key)
                 raise KeyError(f'key {key!r} not found in cache')
             value = self._cache[key]
             if not isinstance(value, (int, float)) or not isinstance(delta, (int, float)):
                 raise TypeError(
-                    f'unsupported operand type(s) for +/-: {type(value)!r} and {type(delta)!r}'
+                    'unsupported operand type(s) for +/-: '
+                    f'{type(value)!r} and {type(delta)!r}'
                 )
             value += delta
             self._cache[key] = value
             self._cache.move_to_end(key, last=False)
         return value
 
     def decr(self, key: Any, delta: Number = 1) -> Number:
@@ -221,14 +235,15 @@
     def __missing__(self, key: Any) -> MiniCache:
         cache: MiniCache = MiniCache(f'{self.name}:{key}', *self.args, **self.kwargs)
         self[key] = cache
         return cache
 
 
 class Cache:
+    """ Memory-based cache instance """
     
     def __init__(self, name: str, *args, **kwargs) -> None:
         self.name: str = name
         def _factory() -> _Caches:
             return _Caches(name, *args, **kwargs)
         self._factory = _factory
         self._caches = _factory()
@@ -286,17 +301,17 @@
         ins = cache.inspect(key)
         if ins is not None:
             ins['tag'] = tag
         return ins
     
     def items(self, tag: TG = empty) -> Iterable[Tuple[Any, ...]]:
         if tag is empty:
-            for tag, cache in self._caches.items():
+            for _tag, cache in self._caches.items():
                 for m in cache.items():
-                    yield m[0], m[1], tag
+                    yield m[0], m[1], _tag
         else:
             cache = self._caches[tag]
             return cache.items()
 
     def keys(self, tag: TG = empty) -> Iterable[Any]:
         if tag is empty:
             for cache in self._caches.values():
@@ -311,44 +326,21 @@
             for cache in self._caches.values():
                 for v in cache.values():
                     yield v
         else:
             cache = self._caches[tag]
             return cache.values()
 
-    def memoize(self, timeout: Time = 24 * 60 * 60, tag: TG = None) -> Any:
-        """ The cache is decorated with the return value of the function,
-        and the timeout is available. """
-
-        def decorator(func: Optional[Callable] = None) -> Callable[[Callable[[Any], Any]], Any]:
-            """ Decorator created by memoize() for callable `func`."""
-            
-            if not callable(func):
-                raise TypeError(
-                    'The `memoize` decorator should be called with a `timeout` parameter.'
-                )
-
-            @functools.wraps(func)
-            def wrapper(*args, **kwargs) -> Any:
-                """Wrapper for callable to cache arguments and return values."""
-                value: Any = self.get(func.__name__, empty, tag)
-                if value is empty:
-                    value: Any = func(*args, **kwargs)
-                    self.set(func.__name__, value, timeout, tag)
-                return value
-            return wrapper
-
-        return decorator
-
     def __len__(self) -> int:
         return sum(len(cache) for cache in self._caches.values())
     
     def __repr__(self) -> str:
         return f'<Cache buckets:{len(self._caches)}>'
 
+    memoize = memoize
     __iter__ = keys
     __setitem__ = set
     __getitem__ = get
     __delitem__ = delete
     __contains__ = has_key
```

### Comparing `cache3-0.4.2/src/cache3/utils.py` & `cache3-0.4.3/src/cache3/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-# DATE: 2021/7/24
-# Author: clarkmonkey@163.com
+# date: 2021/7/24
+# author: clarkmonkey@163.com
 
+""" util
+Tools functions or classes for cache3
+"""
+
+import functools
 import operator
 from time import time as current
 from typing import Any, NoReturn, Optional, Callable, Type, Union
 
 # Compatible with multiple types.
 empty: Any = type('empty', (), {
     '__str__': lambda x: '<empty>',
@@ -28,39 +33,40 @@
 def get_expire(timeout: Time, now: Time = None) -> Time:
     """ Returns a timestamp representing the timeout time """
     if timeout is None:
         return None
     return (now or current()) + timeout
 
 
+# pylint: disable=invalid-name
 class cached_property:
     """ Decorator that converts a method with a single self argument into a
     property cached on the instance.
     """
     name: Optional[str] = None
 
     @staticmethod
-    def func(instance) -> NoReturn:
+    def func(instance) -> NoReturn:  # pylint: disable=method-hidden
         raise TypeError(
             'Cannot use cached_property instance without calling '
             '__set_name__() on it.'
         )
 
-    def __init__(self, func: Callable, name: Optional[str] = None) -> None:
+    def __init__(self, func: Callable, _: Optional[str] = None) -> None:
         self.real_func: Callable = func
         self.__doc__: str = getattr(func, '__doc__')
 
     def __set_name__(self, owner: Any, name: str) -> NoReturn:
         if self.name is None:
             self.name: str = name
             self.func: Callable = self.real_func
         elif name != self.name:
             raise TypeError(
-                "Cannot assign the same cached_property to two different names "
-                "(%r and %r)." % (self.name, name)
+                'Cannot assign the same cached_property to two different names '
+                f'({self.name!r} and {name!r}).'
             )
 
     def __get__(self, instance: Any, cls=None) -> Any:
         """
         Call the function and put the return value in instance.__dict__ so that
         subsequent attribute access on the instance returns the cached value
         instead of calling cached_property.__get__().
@@ -69,14 +75,15 @@
             return self
         res = instance.__dict__[self.name] = self.func(instance)
         return res
 
 
 def new_method_proxy(func) -> Callable:
     def inner(self, *args):
+        # pylint: disable=protected-access
         if self._wrapped is empty:
             self._setup()
         return func(self._wrapped, *args)
     return inner
 
 
 class LazyObject:
@@ -136,12 +143,38 @@
             repr_attr = self._setup_factory
         else:
             repr_attr = self._wrapped
         return f'{type(self).__name__}: {repr_attr!r}'
 
 
 def lazy(factory: Callable) -> Callable:
+
     def wrapper(*args, **kwrags):
         def init():
             return factory(*args, **kwrags)
         return LazyObject(init)
     return wrapper
+
+
+def memoize(self: Any, timeout: Time = 24 * 60 * 60, tag: TG = None) -> Any:
+    """ The cache is decorated with the return value of the function,
+    and the timeout is available. """
+
+    def decorator(func: Optional[Callable] = None) -> Callable[[Callable[[Any], Any]], Any]:
+        """ Decorator created by memoize() for callable `func`."""
+        if not callable(func):
+            raise TypeError(
+                'The `memoize` decorator should be called with a `timeout` parameter.'
+            )
+
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs) -> Any:
+            """Wrapper for callable to cache arguments and return values."""
+            value: Any = self.get(func.__name__, empty, tag)
+            if value is empty:
+                value: Any = func(*args, **kwargs)
+                self.set(func.__name__, value, timeout, tag)
+            return value
+
+        return wrapper
+
+    return decorator
```

### Comparing `cache3-0.4.2/src/cache3.egg-info/PKG-INFO` & `cache3-0.4.3/src/cache3.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cache3
-Version: 0.4.2
+Version: 0.4.3
 Summary: A safe and lightweight cache library, written in pure-Python.
 Home-page: https://github.com/StKali/cache3
 Author: attr: cache3.__author__
 Author-email: clarkmonkey@163.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
@@ -23,15 +23,15 @@
 ===============================
 
 **cache3** is a MIT licensed  safe and lightweight cache library, written
 in pure-Python.
 
 .. image:: https://img.shields.io/badge/LICENSE-MIT-green
     :target: https://github.com/StKali/cache3/blob/master/LICENSE
-.. image:: https://img.shields.io/badge/version-0.3.3-informational
+.. image:: https://img.shields.io/badge/version-0.4.3-informational
     :target: https://pypi.org/project/cache3
 .. image:: https://img.shields.io/badge/python-3.5+-blueviolet
     :target: https://www.python.org
 
 cache3 is very tiny and completely implemented by the Python standard library without any third-party dependencies, so it can be easily embedded in any Python program or script.
 
 Installing
@@ -73,10 +73,10 @@
 - Source Code: https://github.com/StKali/cache3
 
 - Issue Tracker: https://github.com/StKali/cache3/issues
 
 License
 =======
 
-Copyright (c) 2020-2021 clarkmonkey@163.com
+Copyright (c) 2020-2023 clarkmonkey@163.com
 Licensed under the MIT License.
```

### Comparing `cache3-0.4.2/tests/test_base_api.py` & `cache3-0.4.3/tests/test_base_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # date: 2023/2/15
+# author: clarkmonkey@163.com
 
 import pytest
-from cache3.utils import empty
+from cache3.util import empty
 from cache3 import MiniCache, Cache, DiskCache
 from shutil import rmtree
 from utils import rand_strings, rand_string
 
 params = pytest.mark.parametrize
 raises = pytest.raises
```

### Comparing `cache3-0.4.2/tests/test_cache.py` & `cache3-0.4.3/tests/test_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # date: 2023/2/15
+# author: clarkmonkey@163.com
+
 from random import randint
 from pathlib import Path
 from shutil import rmtree
 from cache3 import Cache, DiskCache
 from utils import rand_string, rand_strings
 cases = {
     rand_string(): list(rand_strings(randint(10, 60))) for _ in range(randint(4, 10))
@@ -51,7 +53,15 @@
             self.directory.mkdir(exist_ok=True, parents=True)
         self.cache = DiskCache((self.directory / 'test').as_posix())
 
     def teardown_class(self):
         self.cache.sqlite.close()
         rmtree(self.directory.as_posix())
 
+    def test_multi_get_expired(self):
+        self.cache.clear()
+        self.cache.max_size = 2
+        self.cache.set(1, 1, timeout=-1)
+        self.cache.get(1)
+        self.cache.get(1)
+        len(self.cache)
+
```

### Comparing `cache3-0.4.2/tests/test_disk.py` & `cache3-0.4.3/tests/test_disk.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # date: 2023/2/15
+# author: clarkmonkey@163.com
+
 import pickle
 from pathlib import Path
 from shutil import rmtree
 
 import pytest
-from cache3.disk import (SQLiteEntry, PickleStore, empty, BYTES, NUMBER, STRING, RAW, PICKLE, EvictManager,
-                         EvictInterface, LRUEvict, FIFOEvict, LFUEvict, DiskCache
-                         )
-from cache3.utils import Cache3Error, Cache3Warning
+from cache3.disk import (
+    SQLiteManager, PickleStore, empty, BYTES, NUMBER, STRING, RAW, PICKLE, EvictManager,
+    EvictInterface, LRUEvict, FIFOEvict, LFUEvict, DiskCache
+)
+from cache3.util import Cache3Error, Cache3Warning
 from sqlite3 import Connection
 from threading import Thread
 from utils import rand_string, rand_strings
 
 raises = pytest.raises
 warns = pytest.warns
 test_directory = Path('test_directory')
@@ -25,31 +28,31 @@
     test_directory.mkdir(exist_ok=True, parents=True)
 
 
 def teardown_module():
     rmtree(test_directory.as_posix())
 
 
-class TestSQLiteEntry:
+class TestSQLiteManager:
 
     def test_instance(self):
         test_dir = test_directory / f'test-disk-{rand_string()}'
         test_dir.mkdir(exist_ok=True, parents=True)
 
         # success
-        assert SQLiteEntry(test_dir.as_posix(), rand_string(), None, 5)
+        assert SQLiteManager(test_dir.as_posix(), rand_string(), None, 5)
         
         # invalid pragmas
         with raises(TypeError, match='pragmas want dict object but get .*'):
-            SQLiteEntry(test_dir.as_posix(), rand_string(), None, 5, pragmas=1)
+            SQLiteManager(test_dir.as_posix(), rand_string(), None, 5, pragmas=1)
 
     def test_session(self):
         test_dir = test_directory / f'test-disk-{rand_string()}'
         test_dir.mkdir(exist_ok=True, parents=True)
-        entry = SQLiteEntry(test_dir.as_posix(), rand_string(), None, 5)
+        entry = SQLiteManager(test_dir.as_posix(), rand_string(), None, 5)
         assert isinstance(entry.session, Connection)
         assert entry.close()
 
         def test_multi_threads(sqlite):
             _ = sqlite.session.execute(
                 'CREATE TABLE IF NOT EXISTS `test`('
                 '`key` BLOB,'
@@ -70,15 +73,15 @@
         ts = [Thread(target=test_multi_threads, args=(entry, )) for _ in range(10)]
         [t.start() for t in ts]
         [t.join() for t in ts]
     
     def test_config(self):
         test_dir = test_directory / f'test-disk-{rand_string()}'
         test_dir.mkdir(exist_ok=True, parents=True)
-        entry = SQLiteEntry(test_dir.as_posix(), rand_string(), None, 5)
+        entry = SQLiteManager(test_dir.as_posix(), rand_string(), None, 5)
         assert entry.config('name') is None
         assert entry.config('name',  'value')
         assert entry.config('name') == 'value'
 
 
 class TestPickleStore:
```

### Comparing `cache3-0.4.2/tests/test_memory.py` & `cache3-0.4.3/tests/test_memory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # date: 2023/2/15
+# author: clarkmonkey@163.com
 
 import time
 import pytest
 from cache3 import MiniCache, Cache
 from utils import rand_string, rand_strings
```

### Comparing `cache3-0.4.2/tests/test_utils.py` & `cache3-0.4.3/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # date: 2023/2/26
+# author: clarkmonkey@163.com
 
 import pytest
-from cache3.utils import cached_property, lazy, LazyObject
+from cache3.util import cached_property, lazy, LazyObject
 raises = pytest.raises
 
 
 class TestCachedProperty:
 
     def test_func_error(self):
         with raises(TypeError):
```

