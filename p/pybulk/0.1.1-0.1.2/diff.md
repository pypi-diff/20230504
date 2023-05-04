# Comparing `tmp/pybulk-0.1.1.tar.gz` & `tmp/pybulk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybulk-0.1.1.tar", last modified: Tue Apr 18 09:55:00 2023, max compression
+gzip compressed data, was "dist/pybulk-0.1.2.tar", last modified: Thu May  4 06:36:49 2023, max compression
```

## Comparing `pybulk-0.1.1.tar` & `pybulk-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 09:54:30.000000 pybulk-0.1.1/
--rwxrwxrwx   0 root         (0) root         (0)     2912 2023-04-18 09:54:30.000000 pybulk-0.1.1/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 09:54:30.000000 pybulk-0.1.1/pybulk/
--rwxrwxrwx   0 root         (0) root         (0)     8939 2023-04-18 08:21:18.000000 pybulk-0.1.1/pybulk/base_db.py
--rwxrwxrwx   0 root         (0) root         (0)     7209 2023-04-18 09:08:08.000000 pybulk-0.1.1/pybulk/dbinterface.py
--rwxrwxrwx   0 root         (0) root         (0)      910 2023-04-18 09:11:54.000000 pybulk-0.1.1/pybulk/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 09:54:30.000000 pybulk-0.1.1/pybulk.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-18 09:54:29.000000 pybulk-0.1.1/pybulk.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)     2912 2023-04-18 09:54:29.000000 pybulk-0.1.1/pybulk.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-04-18 09:54:29.000000 pybulk-0.1.1/pybulk.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)      226 2023-04-18 09:54:30.000000 pybulk-0.1.1/pybulk.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-04-18 09:54:29.000000 pybulk-0.1.1/pybulk.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     1883 2023-04-18 09:53:20.000000 pybulk-0.1.1/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-18 09:54:30.000000 pybulk-0.1.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1060 2023-04-18 09:54:27.000000 pybulk-0.1.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:36:23.000000 pybulk-0.1.2/
+-rwxrwxrwx   0 root         (0) root         (0)     2854 2023-05-04 06:36:23.000000 pybulk-0.1.2/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk/
+-rwxrwxrwx   0 root         (0) root         (0)     8939 2023-04-18 08:21:18.000000 pybulk-0.1.2/pybulk/base_db.py
+-rwxrwxrwx   0 root         (0) root         (0)     7209 2023-04-18 09:08:08.000000 pybulk-0.1.2/pybulk/dbinterface.py
+-rwxrwxrwx   0 root         (0) root         (0)      945 2023-04-24 10:05:43.000000 pybulk-0.1.2/pybulk/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2854 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)      226 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1771 2023-04-25 10:08:41.000000 pybulk-0.1.2/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-04 06:36:23.000000 pybulk-0.1.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1059 2023-05-04 06:36:21.000000 pybulk-0.1.2/setup.py
```

### Comparing `pybulk-0.1.1/PKG-INFO` & `pybulk-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pybulk
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyBulk is a Python module that to allow simple and fast bulk data insertion into databases
 Home-page: https://github.com/MrLpk/pybulk
 Author: pengkailiao
 Author-email: pengkailiao@gmail.com
 License: UNKNOWN
 Description: # PyBulk 🚀
+        [简体中文](README_CN.md) | English
+        
         PyBulk is a Python module that wraps PyMySQL to allow simple and fast bulk data insertion into databases. With PyBulk, you can insert thousands of records into a database table in just a few lines of code.
         
         PyBulk builds on top of the PyMySQL library and connection pool to efficiently reuse connections and minimize latency. It handles all the low-level details of executing multiple INSERT statements while protecting your database from overload.
         
         Some of the main features of PyBulk include:
         * **Simple API**: Insert bulk data with just a few function calls. No complicated setup required.
         * **Speed**: Leverages PyMySQL's connection pool to quickly insert thousands of records.
-        * **Safety**: Limits the number of SQL queries executed at a time to protect your database from overload.
         * **Reliability**: Includes error handling and recovery mechanisms to handle transient database errors. Retries failed queries automatically.
         * **Support for REPLACE INTO**: Upsert support allows you to replace existing records in a table or insert new ones.
         * **Compatibility**: Works with MySQL, MariaDB and AWS RDS. Compatible with Python 2 and 3.
         
         PyBulk allows you to focus on your application's logic rather than spending time building infrastructure to handle database load. It is a robust but lightweight solution ideal for batch data processing applications. 
         ## 💾 Installation
```

### Comparing `pybulk-0.1.1/pybulk/base_db.py` & `pybulk-0.1.2/pybulk/base_db.py`

 * *Files identical despite different names*

### Comparing `pybulk-0.1.1/pybulk/dbinterface.py` & `pybulk-0.1.2/pybulk/dbinterface.py`

 * *Files identical despite different names*

### Comparing `pybulk-0.1.1/pybulk/__init__.py` & `pybulk-0.1.2/pybulk/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 """
     
 
 from .dbinterface import DBInterface
 
 def client(cfg=None, alchemy=True):
-    try:
-        from settings import db_config
-    except ModuleNotFoundError:
-        db_config = None
     if cfg is None:
-        cfg = db_config
+        try:
+            from settings import db_config
+            cfg = db_config
+        except (ModuleNotFoundError, ImportError):
+            db_config = None
     db = DBInterface(cfg, alchemy=alchemy)
     return db
```

### Comparing `pybulk-0.1.1/pybulk.egg-info/PKG-INFO` & `pybulk-0.1.2/pybulk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pybulk
-Version: 0.1.1
+Version: 0.1.2
 Summary: PyBulk is a Python module that to allow simple and fast bulk data insertion into databases
 Home-page: https://github.com/MrLpk/pybulk
 Author: pengkailiao
 Author-email: pengkailiao@gmail.com
 License: UNKNOWN
 Description: # PyBulk 🚀
+        [简体中文](README_CN.md) | English
+        
         PyBulk is a Python module that wraps PyMySQL to allow simple and fast bulk data insertion into databases. With PyBulk, you can insert thousands of records into a database table in just a few lines of code.
         
         PyBulk builds on top of the PyMySQL library and connection pool to efficiently reuse connections and minimize latency. It handles all the low-level details of executing multiple INSERT statements while protecting your database from overload.
         
         Some of the main features of PyBulk include:
         * **Simple API**: Insert bulk data with just a few function calls. No complicated setup required.
         * **Speed**: Leverages PyMySQL's connection pool to quickly insert thousands of records.
-        * **Safety**: Limits the number of SQL queries executed at a time to protect your database from overload.
         * **Reliability**: Includes error handling and recovery mechanisms to handle transient database errors. Retries failed queries automatically.
         * **Support for REPLACE INTO**: Upsert support allows you to replace existing records in a table or insert new ones.
         * **Compatibility**: Works with MySQL, MariaDB and AWS RDS. Compatible with Python 2 and 3.
         
         PyBulk allows you to focus on your application's logic rather than spending time building infrastructure to handle database load. It is a robust but lightweight solution ideal for batch data processing applications. 
         ## 💾 Installation
```

### Comparing `pybulk-0.1.1/README.md` & `pybulk-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-# PyBulk 🚀
-PyBulk is a Python module that wraps PyMySQL to allow simple and fast bulk data insertion into databases. With PyBulk, you can insert thousands of records into a database table in just a few lines of code.
-
-PyBulk builds on top of the PyMySQL library and connection pool to efficiently reuse connections and minimize latency. It handles all the low-level details of executing multiple INSERT statements while protecting your database from overload.
-
-Some of the main features of PyBulk include:
-* **Simple API**: Insert bulk data with just a few function calls. No complicated setup required.
-* **Speed**: Leverages PyMySQL's connection pool to quickly insert thousands of records.
-* **Safety**: Limits the number of SQL queries executed at a time to protect your database from overload.
-* **Reliability**: Includes error handling and recovery mechanisms to handle transient database errors. Retries failed queries automatically.
-* **Support for REPLACE INTO**: Upsert support allows you to replace existing records in a table or insert new ones.
-* **Compatibility**: Works with MySQL, MariaDB and AWS RDS. Compatible with Python 2 and 3.
-
-PyBulk allows you to focus on your application's logic rather than spending time building infrastructure to handle database load. It is a robust but lightweight solution ideal for batch data processing applications. 
-## 💾 Installation
-
-```
-pip install pybulk
-```
-
-## 🔧 Usage:
-```
-import pybulk
-
-cfg = {
-'host': 'localhost',
-'port':  3306,
-'user':  'root',
-'password': 'root',
-'db': 'info',
-'charset': 'utf8',
-}
-
-db = pybulk.client(cfg)
-
-my_data = [
-{'name': 'Peter', 'age': 21,},
-{'name': 'Harry', 'age': 35,},
-{'name': 'Mark', 'age': 40,},
-]
-
-db.push_data('student', my_data, size=2000)
-
-# You can also run sql in pybulk like:
-
-data = db.excute_sql('select * from school')
+# PyBulk 🚀
+[简体中文](README_CN.md) | English
+
+PyBulk is a Python module that wraps PyMySQL to allow simple and fast bulk data insertion into databases. With PyBulk, you can insert thousands of records into a database table in just a few lines of code.
+
+PyBulk builds on top of the PyMySQL library and connection pool to efficiently reuse connections and minimize latency. It handles all the low-level details of executing multiple INSERT statements while protecting your database from overload.
+
+Some of the main features of PyBulk include:
+* **Simple API**: Insert bulk data with just a few function calls. No complicated setup required.
+* **Speed**: Leverages PyMySQL's connection pool to quickly insert thousands of records.
+* **Reliability**: Includes error handling and recovery mechanisms to handle transient database errors. Retries failed queries automatically.
+* **Support for REPLACE INTO**: Upsert support allows you to replace existing records in a table or insert new ones.
+* **Compatibility**: Works with MySQL, MariaDB and AWS RDS. Compatible with Python 2 and 3.
+
+PyBulk allows you to focus on your application's logic rather than spending time building infrastructure to handle database load. It is a robust but lightweight solution ideal for batch data processing applications. 
+## 💾 Installation
+
+```
+pip install pybulk
+```
+
+## 🔧 Usage:
+```
+import pybulk
+
+cfg = {
+'host': 'localhost',
+'port':  3306,
+'user':  'root',
+'password': 'root',
+'db': 'info',
+'charset': 'utf8',
+}
+
+db = pybulk.client(cfg)
+
+my_data = [
+{'name': 'Peter', 'age': 21,},
+{'name': 'Harry', 'age': 35,},
+{'name': 'Mark', 'age': 40,},
+]
+
+db.push_data('student', my_data, size=2000)
+
+# You can also run sql in pybulk like:
+
+data = db.excute_sql('select * from school')
 ```
```

### Comparing `pybulk-0.1.1/setup.py` & `pybulk-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
  
  
 setuptools.setup(
     name='pybulk',
-    version="0.1.1",
+    version="0.1.2",
     author="pengkailiao",
     author_email="pengkailiao@gmail.com",
     description="PyBulk is a Python module that to allow simple and fast bulk data insertion into databases",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/MrLpk/pybulk",
     packages=setuptools.find_packages(),
@@ -24,11 +24,11 @@
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     # 依赖模块
     install_requires=[
         'PyMySQL>=0.9.3',
-        'SQLAlchemy>=1.3.15',
+        'SQLAlchemy>=1.3.8',
     ],
     python_requires='>=3.6',
 )
```

