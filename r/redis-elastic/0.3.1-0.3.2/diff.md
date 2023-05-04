# Comparing `tmp/redis_elastic-0.3.1.tar.gz` & `tmp/redis_elastic-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_elastic-0.3.1.tar", last modified: Thu May  4 16:42:30 2023, max compression
+gzip compressed data, was "redis_elastic-0.3.2.tar", last modified: Thu May  4 16:49:31 2023, max compression
```

## Comparing `redis_elastic-0.3.1.tar` & `redis_elastic-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:42:30.305263 redis_elastic-0.3.1/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 16:42:30.305263 redis_elastic-0.3.1/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2801 2023-05-04 16:25:55.000000 redis_elastic-0.3.1/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:42:30.301263 redis_elastic-0.3.1/Warehouse/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-0.3.1/Warehouse/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4774 2023-05-02 22:59:48.000000 redis_elastic-0.3.1/Warehouse/redis_elastic.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:42:30.305263 redis_elastic-0.3.1/redis_elastic.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 16:42:30.000000 redis_elastic-0.3.1/redis_elastic.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      251 2023-05-04 16:42:30.000000 redis_elastic-0.3.1/redis_elastic.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-04 16:42:30.000000 redis_elastic-0.3.1/redis_elastic.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       74 2023-05-04 16:42:30.000000 redis_elastic-0.3.1/redis_elastic.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-04 16:42:30.000000 redis_elastic-0.3.1/redis_elastic.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-04 16:42:30.305263 redis_elastic-0.3.1/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      879 2023-05-04 16:42:20.000000 redis_elastic-0.3.1/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:49:31.195424 redis_elastic-0.3.2/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 16:49:31.191424 redis_elastic-0.3.2/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2801 2023-05-04 16:25:55.000000 redis_elastic-0.3.2/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:49:31.191424 redis_elastic-0.3.2/Warehouse/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-0.3.2/Warehouse/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4774 2023-05-02 22:59:48.000000 redis_elastic-0.3.2/Warehouse/redis_elastic.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:49:31.191424 redis_elastic-0.3.2/redis_elastic.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      251 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       70 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-04 16:49:31.195424 redis_elastic-0.3.2/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      864 2023-05-04 16:48:58.000000 redis_elastic-0.3.2/setup.py
```

### Comparing `redis_elastic-0.3.1/PKG-INFO` & `redis_elastic-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis_elastic
-Version: 0.3.1
+Version: 0.3.2
 Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
 Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
 Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
 Author: Carlos Garcia Garcia
 Author-email: carlos.garcia1.gr1@icloud.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `redis_elastic-0.3.1/README.md` & `redis_elastic-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `redis_elastic-0.3.1/Warehouse/redis_elastic.py` & `redis_elastic-0.3.2/Warehouse/redis_elastic.py`

 * *Files identical despite different names*

### Comparing `redis_elastic-0.3.1/redis_elastic.egg-info/PKG-INFO` & `redis_elastic-0.3.2/redis_elastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-elastic
-Version: 0.3.1
+Version: 0.3.2
 Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
 Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
 Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
 Author: Carlos Garcia Garcia
 Author-email: carlos.garcia1.gr1@icloud.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `redis_elastic-0.3.1/setup.py` & `redis_elastic-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup
 
 readme = open("./README.md", "r")
 
 setup(
     name="redis_elastic",
-    version="0.3.1",
+    version="0.3.2",
     description="Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch",
     install_requires=[
-        "ast",
         "psycopg2",
         "psycopg2-binary",
         "functools",
         "redis",
         "elasticsearch==7.13.4",
         "pandas"
     ],
```

