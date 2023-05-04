# Comparing `tmp/pybulk-0.1.2.tar.gz` & `tmp/pybulk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybulk-0.1.2.tar", last modified: Thu May  4 06:36:49 2023, max compression
+gzip compressed data, was "dist/pybulk-0.1.3.tar", last modified: Thu May  4 06:53:21 2023, max compression
```

## Comparing `pybulk-0.1.2.tar` & `pybulk-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:36:23.000000 pybulk-0.1.2/
--rwxrwxrwx   0 root         (0) root         (0)     2854 2023-05-04 06:36:23.000000 pybulk-0.1.2/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk/
--rwxrwxrwx   0 root         (0) root         (0)     8939 2023-04-18 08:21:18.000000 pybulk-0.1.2/pybulk/base_db.py
--rwxrwxrwx   0 root         (0) root         (0)     7209 2023-04-18 09:08:08.000000 pybulk-0.1.2/pybulk/dbinterface.py
--rwxrwxrwx   0 root         (0) root         (0)      945 2023-04-24 10:05:43.000000 pybulk-0.1.2/pybulk/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)     2854 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)      226 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-04 06:36:23.000000 pybulk-0.1.2/pybulk.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     1771 2023-04-25 10:08:41.000000 pybulk-0.1.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-04 06:36:23.000000 pybulk-0.1.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1059 2023-05-04 06:36:21.000000 pybulk-0.1.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:52:55.000000 pybulk-0.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)     2854 2023-05-04 06:52:55.000000 pybulk-0.1.3/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk/
+-rwxrwxrwx   0 root         (0) root         (0)     8939 2023-04-18 08:21:18.000000 pybulk-0.1.3/pybulk/base_db.py
+-rwxrwxrwx   0 root         (0) root         (0)     7209 2023-04-18 09:08:08.000000 pybulk-0.1.3/pybulk/dbinterface.py
+-rwxrwxrwx   0 root         (0) root         (0)      951 2023-05-04 06:52:06.000000 pybulk-0.1.3/pybulk/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2854 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)      226 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-04 06:52:55.000000 pybulk-0.1.3/pybulk.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1771 2023-04-25 10:08:41.000000 pybulk-0.1.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-04 06:52:55.000000 pybulk-0.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1059 2023-05-04 06:52:27.000000 pybulk-0.1.3/setup.py
```

### Comparing `pybulk-0.1.2/PKG-INFO` & `pybulk-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybulk
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyBulk is a Python module that to allow simple and fast bulk data insertion into databases
 Home-page: https://github.com/MrLpk/pybulk
 Author: pengkailiao
 Author-email: pengkailiao@gmail.com
 License: UNKNOWN
 Description: # PyBulk 🚀
         [简体中文](README_CN.md) | English
```

### Comparing `pybulk-0.1.2/pybulk/base_db.py` & `pybulk-0.1.3/pybulk/base_db.py`

 * *Files identical despite different names*

### Comparing `pybulk-0.1.2/pybulk/dbinterface.py` & `pybulk-0.1.3/pybulk/dbinterface.py`

 * *Files identical despite different names*

### Comparing `pybulk-0.1.2/pybulk/__init__.py` & `pybulk-0.1.3/pybulk/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,13 +35,13 @@
     
 
 from .dbinterface import DBInterface
 
 def client(cfg=None, alchemy=True):
     if cfg is None:
         try:
-            from settings import db_config
-            cfg = db_config
+            from settings import DATABASE_CONFIG
+            cfg = DATABASE_CONFIG
         except (ModuleNotFoundError, ImportError):
-            db_config = None
+            cfg = None
     db = DBInterface(cfg, alchemy=alchemy)
     return db
```

### Comparing `pybulk-0.1.2/pybulk.egg-info/PKG-INFO` & `pybulk-0.1.3/pybulk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybulk
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyBulk is a Python module that to allow simple and fast bulk data insertion into databases
 Home-page: https://github.com/MrLpk/pybulk
 Author: pengkailiao
 Author-email: pengkailiao@gmail.com
 License: UNKNOWN
 Description: # PyBulk 🚀
         [简体中文](README_CN.md) | English
```

### Comparing `pybulk-0.1.2/README.md` & `pybulk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pybulk-0.1.2/setup.py` & `pybulk-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
  
  
 setuptools.setup(
     name='pybulk',
-    version="0.1.2",
+    version="0.1.3",
     author="pengkailiao",
     author_email="pengkailiao@gmail.com",
     description="PyBulk is a Python module that to allow simple and fast bulk data insertion into databases",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/MrLpk/pybulk",
     packages=setuptools.find_packages(),
```

