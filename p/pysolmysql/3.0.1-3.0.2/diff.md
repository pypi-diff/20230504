# Comparing `tmp/pysolmysql-3.0.1.tar.gz` & `tmp/pysolmysql-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysolmysql-3.0.1.tar", last modified: Wed Apr  6 16:06:59 2022, max compression
+gzip compressed data, was "dist/pysolmysql-3.0.2.tar", last modified: Thu May  4 06:33:10 2023, max compression
```

## Comparing `pysolmysql-3.0.1.tar` & `pysolmysql-3.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/
--rw-r--r--   0 champax   (1000) champax   (1000)    32175 2019-07-18 13:12:52.000000 pysolmysql-3.0.1/LICENSE.md
--rw-r--r--   0 champax   (1000) champax   (1000)       26 2019-01-15 10:44:20.000000 pysolmysql-3.0.1/MANIFEST.in
--rw-r--r--   0 champax   (1000) champax   (1000)     4622 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/PKG-INFO
--rw-r--r--   0 champax   (1000) champax   (1000)     2938 2021-02-02 14:08:43.000000 pysolmysql-3.0.1/README.md
-drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql/
-drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql/Mysql/
--rw-r--r--   0 champax   (1000) champax   (1000)     8010 2022-04-06 16:06:03.000000 pysolmysql-3.0.1/pysolmysql/Mysql/MysqlApi.py
--rw-r--r--   0 champax   (1000) champax   (1000)      972 2019-01-15 10:44:20.000000 pysolmysql-3.0.1/pysolmysql/Mysql/__init__.py
-drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql/Pool/
--rw-r--r--   0 champax   (1000) champax   (1000)     1545 2019-08-27 14:26:53.000000 pysolmysql-3.0.1/pysolmysql/Pool/__init__.py
--rw-r--r--   0 champax   (1000) champax   (1000)     5528 2021-03-03 10:59:33.000000 pysolmysql-3.0.1/pysolmysql/Pool/base_pool.py
--rw-r--r--   0 champax   (1000) champax   (1000)    10613 2020-11-09 11:15:09.000000 pysolmysql-3.0.1/pysolmysql/Pool/mysql_pool.py
--rw-r--r--   0 champax   (1000) champax   (1000)      972 2019-01-15 10:44:20.000000 pysolmysql-3.0.1/pysolmysql/__init__.py
-drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql.egg-info/
--rw-r--r--   0 champax   (1000) champax   (1000)     4622 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql.egg-info/PKG-INFO
--rw-r--r--   0 champax   (1000) champax   (1000)      450 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql.egg-info/SOURCES.txt
--rw-r--r--   0 champax   (1000) champax   (1000)        1 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql.egg-info/dependency_links.txt
--rw-r--r--   0 champax   (1000) champax   (1000)        1 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql.egg-info/not-zip-safe
--rw-r--r--   0 champax   (1000) champax   (1000)       66 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql.egg-info/requires.txt
--rw-r--r--   0 champax   (1000) champax   (1000)       11 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/pysolmysql.egg-info/top_level.txt
--rw-r--r--   0 champax   (1000) champax   (1000)      108 2021-02-02 14:08:43.000000 pysolmysql-3.0.1/requirements.txt
--rw-r--r--   0 champax   (1000) champax   (1000)      136 2021-02-02 14:08:43.000000 pysolmysql-3.0.1/requirements_test.txt
--rw-r--r--   0 champax   (1000) champax   (1000)       38 2022-04-06 16:06:59.000000 pysolmysql-3.0.1/setup.cfg
--rw-r--r--   0 champax   (1000) champax   (1000)     3656 2022-04-06 16:05:30.000000 pysolmysql-3.0.1/setup.py
+drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/
+-rw-r--r--   0 champax   (1000) champax   (1000)    32175 2019-07-18 13:12:52.000000 pysolmysql-3.0.2/LICENSE.md
+-rw-r--r--   0 champax   (1000) champax   (1000)       26 2019-01-15 10:44:20.000000 pysolmysql-3.0.2/MANIFEST.in
+-rw-r--r--   0 champax   (1000) champax   (1000)     3636 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/PKG-INFO
+-rw-r--r--   0 champax   (1000) champax   (1000)     2938 2021-02-02 14:08:43.000000 pysolmysql-3.0.2/README.md
+drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/pysolmysql/
+drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/pysolmysql/Mysql/
+-rw-r--r--   0 champax   (1000) champax   (1000)     8010 2022-04-06 16:06:03.000000 pysolmysql-3.0.2/pysolmysql/Mysql/MysqlApi.py
+-rw-r--r--   0 champax   (1000) champax   (1000)      972 2019-01-15 10:44:20.000000 pysolmysql-3.0.2/pysolmysql/Mysql/__init__.py
+drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/pysolmysql/Pool/
+-rw-r--r--   0 champax   (1000) champax   (1000)     1545 2019-08-27 14:26:53.000000 pysolmysql-3.0.2/pysolmysql/Pool/__init__.py
+-rw-r--r--   0 champax   (1000) champax   (1000)     5528 2021-03-03 10:59:33.000000 pysolmysql-3.0.2/pysolmysql/Pool/base_pool.py
+-rw-r--r--   0 champax   (1000) champax   (1000)    10578 2023-05-04 06:32:24.000000 pysolmysql-3.0.2/pysolmysql/Pool/mysql_pool.py
+-rw-r--r--   0 champax   (1000) champax   (1000)      972 2019-01-15 10:44:20.000000 pysolmysql-3.0.2/pysolmysql/__init__.py
+drwxr-xr-x   0 champax   (1000) champax   (1000)        0 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/pysolmysql.egg-info/
+-rw-r--r--   0 champax   (1000) champax   (1000)     3636 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/pysolmysql.egg-info/PKG-INFO
+-rw-r--r--   0 champax   (1000) champax   (1000)      450 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/pysolmysql.egg-info/SOURCES.txt
+-rw-r--r--   0 champax   (1000) champax   (1000)        1 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/pysolmysql.egg-info/dependency_links.txt
+-rw-r--r--   0 champax   (1000) champax   (1000)        1 2023-05-04 06:29:17.000000 pysolmysql-3.0.2/pysolmysql.egg-info/not-zip-safe
+-rw-r--r--   0 champax   (1000) champax   (1000)       66 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/pysolmysql.egg-info/requires.txt
+-rw-r--r--   0 champax   (1000) champax   (1000)       11 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/pysolmysql.egg-info/top_level.txt
+-rw-r--r--   0 champax   (1000) champax   (1000)      108 2021-02-02 14:08:43.000000 pysolmysql-3.0.2/requirements.txt
+-rw-r--r--   0 champax   (1000) champax   (1000)      136 2021-02-02 14:08:43.000000 pysolmysql-3.0.2/requirements_test.txt
+-rw-r--r--   0 champax   (1000) champax   (1000)       38 2023-05-04 06:33:10.000000 pysolmysql-3.0.2/setup.cfg
+-rw-r--r--   0 champax   (1000) champax   (1000)     3656 2023-05-04 06:32:24.000000 pysolmysql-3.0.2/setup.py
```

### Comparing `pysolmysql-3.0.1/LICENSE.md` & `pysolmysql-3.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysolmysql-3.0.1/PKG-INFO` & `pysolmysql-3.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,147 @@
 Metadata-Version: 2.1
 Name: pysolmysql
-Version: 3.0.1
+Version: 3.0.2
 Summary: Simple MYSQL client Apis
 Home-page: https://knock.center
 Author: Laurent Champagnac
 Author-email: champagnac.laurent@gmail.com
 License: GPLv3
-Description: pysolmysql
-        ============
-        
-        Welcome to pysol
-        
-        Copyright (C) 2013/2017 Laurent Labatut / Laurent Champagnac
-        
-        pysolmysql is a set of simple MYSQL client Apis
-        
-        They are gevent based.
-        They rely on pymysql.
-        
-        Usage
-        ===============
-        
-        ```
-        d_conf = {
-            "host": "localhost",
-            "port": 3306,
-            "database": None,
-            "user": "root",
-            "password": "root",
-            "autocommit": True,
-        }
-                
-        ar = MysqlApi.exec_n(d_conf, "select user, host from mysql.user;")
-        
-        for d_record in ar:
-            logger.info("user=%s, host=%s", d_record["user"], d_record["host"])
-        ```
-        
-        Pool
-        ===============
-        
-        Now backed by a basic pool implementation, which support underlying backend clusters (mariadb galera for instance)
-        
-        This basic pool implementation is forked and adapted from :
-        - https://github.com/laurentL/django-mysql-geventpool-27
-        - https://github.com/shunsukeaihara/django-mysql-geventpool
-        
-        Pool max size
-        ===============
-        
-        Pool max size (default 10) can be specified using
-        ```
-        d_conf = {
-            "pool_max_size": 10,
-            ...
-        }
-        ```
-        
-        Possible backward compatibility issue:
-        - If the pool is maxed, an exception will be raised
-        
-        Multiple hosts
-        ===============
-        
-        Multiple hosts can be addressed in an active/active manner.
-        
-        Several hosts can be specified using :
-        - "hosts" list (preferred)
-        ```
-        d_conf = {
-            "hosts": ["localhost", "127.0.0.1"],
-            ...
-        }
-        ```
-        
-        - "host" comma separated list
-        ```
-        d_conf = {
-            "host": "localhost,127.0.0.1",
-            ...
-        }
-        ```
-        
-        - "host" single entry (backward compatible mode)
-        ```
-        d_conf = {
-            "host": "localhost",
-            ...
-        }
-        ```
-        
-        Source code
-        ===============
-        
-        - We are pep8 compliant (as far as we can, with some exemptions)
-        - We use a right margin of 360 characters (please don't talk me about 80 chars)
-        - All unittest files must begin with `test_` or `Test`, should implement setUp and tearDown methods
-        - All tests must adapt to any running directory
-        - The whole project is backed by gevent (http://www.gevent.org/)
-        - We use docstring (:return, :rtype, :param, :type etc), they are mandatory
-        - We use PyCharm "noinspection", feel free to use them
-        
-        Requirements
-        ===============
-        
-        - Debian 10 or greater, x64, Python 3.7
-        
-        Unittests
-        ===============
-        
-        To run unittests, you will need:
-        
-        - mysql installed and running, with root/root credentials
-        
-        License
-        ===============
-        
-        This program is free software; you can redistribute it and/or
-        modify it under the terms of the GNU General Public License
-        as published by the Free Software Foundation; either version 2
-        of the License, or (at your option) any later version.
-        
-        This program is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU General Public License for more details.
-        
-        You should have received a copy of the GNU General Public License
-        along with this program; if not, write to the Free Software
-        Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA
-        
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+pysolmysql
+============
+
+Welcome to pysol
+
+Copyright (C) 2013/2017 Laurent Labatut / Laurent Champagnac
+
+pysolmysql is a set of simple MYSQL client Apis
+
+They are gevent based.
+They rely on pymysql.
+
+Usage
+===============
+
+```
+d_conf = {
+    "host": "localhost",
+    "port": 3306,
+    "database": None,
+    "user": "root",
+    "password": "root",
+    "autocommit": True,
+}
+        
+ar = MysqlApi.exec_n(d_conf, "select user, host from mysql.user;")
+
+for d_record in ar:
+    logger.info("user=%s, host=%s", d_record["user"], d_record["host"])
+```
+
+Pool
+===============
+
+Now backed by a basic pool implementation, which support underlying backend clusters (mariadb galera for instance)
+
+This basic pool implementation is forked and adapted from :
+- https://github.com/laurentL/django-mysql-geventpool-27
+- https://github.com/shunsukeaihara/django-mysql-geventpool
+
+Pool max size
+===============
+
+Pool max size (default 10) can be specified using
+```
+d_conf = {
+    "pool_max_size": 10,
+    ...
+}
+```
+
+Possible backward compatibility issue:
+- If the pool is maxed, an exception will be raised
+
+Multiple hosts
+===============
+
+Multiple hosts can be addressed in an active/active manner.
+
+Several hosts can be specified using :
+- "hosts" list (preferred)
+```
+d_conf = {
+    "hosts": ["localhost", "127.0.0.1"],
+    ...
+}
+```
+
+- "host" comma separated list
+```
+d_conf = {
+    "host": "localhost,127.0.0.1",
+    ...
+}
+```
+
+- "host" single entry (backward compatible mode)
+```
+d_conf = {
+    "host": "localhost",
+    ...
+}
+```
+
+Source code
+===============
+
+- We are pep8 compliant (as far as we can, with some exemptions)
+- We use a right margin of 360 characters (please don't talk me about 80 chars)
+- All unittest files must begin with `test_` or `Test`, should implement setUp and tearDown methods
+- All tests must adapt to any running directory
+- The whole project is backed by gevent (http://www.gevent.org/)
+- We use docstring (:return, :rtype, :param, :type etc), they are mandatory
+- We use PyCharm "noinspection", feel free to use them
+
+Requirements
+===============
+
+- Debian 10 or greater, x64, Python 3.7
+
+Unittests
+===============
+
+To run unittests, you will need:
+
+- mysql installed and running, with root/root credentials
+
+License
+===============
+
+This program is free software; you can redistribute it and/or
+modify it under the terms of the GNU General Public License
+as published by the Free Software Foundation; either version 2
+of the License, or (at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program; if not, write to the Free Software
+Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA
+
+
+
+
```

### Comparing `pysolmysql-3.0.1/README.md` & `pysolmysql-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pysolmysql-3.0.1/pysolmysql/Mysql/MysqlApi.py` & `pysolmysql-3.0.2/pysolmysql/Mysql/MysqlApi.py`

 * *Files identical despite different names*

### Comparing `pysolmysql-3.0.1/pysolmysql/Mysql/__init__.py` & `pysolmysql-3.0.2/pysolmysql/Mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pysolmysql-3.0.1/pysolmysql/Pool/__init__.py` & `pysolmysql-3.0.2/pysolmysql/Pool/__init__.py`

 * *Files identical despite different names*

### Comparing `pysolmysql-3.0.1/pysolmysql/Pool/base_pool.py` & `pysolmysql-3.0.2/pysolmysql/Pool/base_pool.py`

 * *Files identical despite different names*

### Comparing `pysolmysql-3.0.1/pysolmysql/Pool/mysql_pool.py` & `pysolmysql-3.0.2/pysolmysql/Pool/mysql_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from pysolmeters.Meters import Meters
 
 from pysolmysql.Pool.base_pool import DatabaseConnectionPool
 
 logger = logging.getLogger(__name__)
 
 # Init random
-random.seed(a=struct.unpack('i', os.urandom(4)))
+random.seed()
 
 
 class MysqlConnectionPool(DatabaseConnectionPool):
     """
     Mysql connection pool, gevent compliant.
 
     This support multiple target hosts.
```

### Comparing `pysolmysql-3.0.1/pysolmysql/__init__.py` & `pysolmysql-3.0.2/pysolmysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pysolmysql-3.0.1/pysolmysql.egg-info/PKG-INFO` & `pysolmysql-3.0.2/pysolmysql.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,147 @@
 Metadata-Version: 2.1
 Name: pysolmysql
-Version: 3.0.1
+Version: 3.0.2
 Summary: Simple MYSQL client Apis
 Home-page: https://knock.center
 Author: Laurent Champagnac
 Author-email: champagnac.laurent@gmail.com
 License: GPLv3
-Description: pysolmysql
-        ============
-        
-        Welcome to pysol
-        
-        Copyright (C) 2013/2017 Laurent Labatut / Laurent Champagnac
-        
-        pysolmysql is a set of simple MYSQL client Apis
-        
-        They are gevent based.
-        They rely on pymysql.
-        
-        Usage
-        ===============
-        
-        ```
-        d_conf = {
-            "host": "localhost",
-            "port": 3306,
-            "database": None,
-            "user": "root",
-            "password": "root",
-            "autocommit": True,
-        }
-                
-        ar = MysqlApi.exec_n(d_conf, "select user, host from mysql.user;")
-        
-        for d_record in ar:
-            logger.info("user=%s, host=%s", d_record["user"], d_record["host"])
-        ```
-        
-        Pool
-        ===============
-        
-        Now backed by a basic pool implementation, which support underlying backend clusters (mariadb galera for instance)
-        
-        This basic pool implementation is forked and adapted from :
-        - https://github.com/laurentL/django-mysql-geventpool-27
-        - https://github.com/shunsukeaihara/django-mysql-geventpool
-        
-        Pool max size
-        ===============
-        
-        Pool max size (default 10) can be specified using
-        ```
-        d_conf = {
-            "pool_max_size": 10,
-            ...
-        }
-        ```
-        
-        Possible backward compatibility issue:
-        - If the pool is maxed, an exception will be raised
-        
-        Multiple hosts
-        ===============
-        
-        Multiple hosts can be addressed in an active/active manner.
-        
-        Several hosts can be specified using :
-        - "hosts" list (preferred)
-        ```
-        d_conf = {
-            "hosts": ["localhost", "127.0.0.1"],
-            ...
-        }
-        ```
-        
-        - "host" comma separated list
-        ```
-        d_conf = {
-            "host": "localhost,127.0.0.1",
-            ...
-        }
-        ```
-        
-        - "host" single entry (backward compatible mode)
-        ```
-        d_conf = {
-            "host": "localhost",
-            ...
-        }
-        ```
-        
-        Source code
-        ===============
-        
-        - We are pep8 compliant (as far as we can, with some exemptions)
-        - We use a right margin of 360 characters (please don't talk me about 80 chars)
-        - All unittest files must begin with `test_` or `Test`, should implement setUp and tearDown methods
-        - All tests must adapt to any running directory
-        - The whole project is backed by gevent (http://www.gevent.org/)
-        - We use docstring (:return, :rtype, :param, :type etc), they are mandatory
-        - We use PyCharm "noinspection", feel free to use them
-        
-        Requirements
-        ===============
-        
-        - Debian 10 or greater, x64, Python 3.7
-        
-        Unittests
-        ===============
-        
-        To run unittests, you will need:
-        
-        - mysql installed and running, with root/root credentials
-        
-        License
-        ===============
-        
-        This program is free software; you can redistribute it and/or
-        modify it under the terms of the GNU General Public License
-        as published by the Free Software Foundation; either version 2
-        of the License, or (at your option) any later version.
-        
-        This program is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU General Public License for more details.
-        
-        You should have received a copy of the GNU General Public License
-        along with this program; if not, write to the Free Software
-        Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA
-        
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+pysolmysql
+============
+
+Welcome to pysol
+
+Copyright (C) 2013/2017 Laurent Labatut / Laurent Champagnac
+
+pysolmysql is a set of simple MYSQL client Apis
+
+They are gevent based.
+They rely on pymysql.
+
+Usage
+===============
+
+```
+d_conf = {
+    "host": "localhost",
+    "port": 3306,
+    "database": None,
+    "user": "root",
+    "password": "root",
+    "autocommit": True,
+}
+        
+ar = MysqlApi.exec_n(d_conf, "select user, host from mysql.user;")
+
+for d_record in ar:
+    logger.info("user=%s, host=%s", d_record["user"], d_record["host"])
+```
+
+Pool
+===============
+
+Now backed by a basic pool implementation, which support underlying backend clusters (mariadb galera for instance)
+
+This basic pool implementation is forked and adapted from :
+- https://github.com/laurentL/django-mysql-geventpool-27
+- https://github.com/shunsukeaihara/django-mysql-geventpool
+
+Pool max size
+===============
+
+Pool max size (default 10) can be specified using
+```
+d_conf = {
+    "pool_max_size": 10,
+    ...
+}
+```
+
+Possible backward compatibility issue:
+- If the pool is maxed, an exception will be raised
+
+Multiple hosts
+===============
+
+Multiple hosts can be addressed in an active/active manner.
+
+Several hosts can be specified using :
+- "hosts" list (preferred)
+```
+d_conf = {
+    "hosts": ["localhost", "127.0.0.1"],
+    ...
+}
+```
+
+- "host" comma separated list
+```
+d_conf = {
+    "host": "localhost,127.0.0.1",
+    ...
+}
+```
+
+- "host" single entry (backward compatible mode)
+```
+d_conf = {
+    "host": "localhost",
+    ...
+}
+```
+
+Source code
+===============
+
+- We are pep8 compliant (as far as we can, with some exemptions)
+- We use a right margin of 360 characters (please don't talk me about 80 chars)
+- All unittest files must begin with `test_` or `Test`, should implement setUp and tearDown methods
+- All tests must adapt to any running directory
+- The whole project is backed by gevent (http://www.gevent.org/)
+- We use docstring (:return, :rtype, :param, :type etc), they are mandatory
+- We use PyCharm "noinspection", feel free to use them
+
+Requirements
+===============
+
+- Debian 10 or greater, x64, Python 3.7
+
+Unittests
+===============
+
+To run unittests, you will need:
+
+- mysql installed and running, with root/root credentials
+
+License
+===============
+
+This program is free software; you can redistribute it and/or
+modify it under the terms of the GNU General Public License
+as published by the Free Software Foundation; either version 2
+of the License, or (at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program; if not, write to the Free Software
+Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA
+
+
+
+
```

### Comparing `pysolmysql-3.0.1/setup.py` & `pysolmysql-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 # SETUP
 # ===========================
 
 p_name = "pysolmysql"
 p_author = "Laurent Champagnac"
 p_email = "champagnac.laurent@gmail.com"
 p_url = "https://knock.center"
-p_version = "3.0.1"
+p_version = "3.0.2"
 
 # Load
 req_list, dep_list = requirement_read("requirements.txt")
 test_req_list, _ = requirement_read("requirements_test.txt")
 
 setup(
```

