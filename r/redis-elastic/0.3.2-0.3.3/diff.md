# Comparing `tmp/redis_elastic-0.3.2.tar.gz` & `tmp/redis_elastic-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_elastic-0.3.2.tar", last modified: Thu May  4 16:49:31 2023, max compression
+gzip compressed data, was "redis_elastic-0.3.3.tar", last modified: Thu May  4 16:56:20 2023, max compression
```

## Comparing `redis_elastic-0.3.2.tar` & `redis_elastic-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:49:31.195424 redis_elastic-0.3.2/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 16:49:31.191424 redis_elastic-0.3.2/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2801 2023-05-04 16:25:55.000000 redis_elastic-0.3.2/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:49:31.191424 redis_elastic-0.3.2/Warehouse/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-0.3.2/Warehouse/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4774 2023-05-02 22:59:48.000000 redis_elastic-0.3.2/Warehouse/redis_elastic.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:49:31.191424 redis_elastic-0.3.2/redis_elastic.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      251 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       70 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-04 16:49:31.000000 redis_elastic-0.3.2/redis_elastic.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-04 16:49:31.195424 redis_elastic-0.3.2/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      864 2023-05-04 16:48:58.000000 redis_elastic-0.3.2/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:56:20.596693 redis_elastic-0.3.3/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 16:56:20.596693 redis_elastic-0.3.3/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2801 2023-05-04 16:55:29.000000 redis_elastic-0.3.3/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:56:20.592693 redis_elastic-0.3.3/Warehouse/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-0.3.3/Warehouse/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4774 2023-05-02 22:59:48.000000 redis_elastic-0.3.3/Warehouse/redis_elastic.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 16:56:20.596693 redis_elastic-0.3.3/redis_elastic.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 16:56:20.000000 redis_elastic-0.3.3/redis_elastic.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      251 2023-05-04 16:56:20.000000 redis_elastic-0.3.3/redis_elastic.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-04 16:56:20.000000 redis_elastic-0.3.3/redis_elastic.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       60 2023-05-04 16:56:20.000000 redis_elastic-0.3.3/redis_elastic.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-04 16:56:20.000000 redis_elastic-0.3.3/redis_elastic.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-04 16:56:20.596693 redis_elastic-0.3.3/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      843 2023-05-04 16:54:33.000000 redis_elastic-0.3.3/setup.py
```

### Comparing `redis_elastic-0.3.2/PKG-INFO` & `redis_elastic-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: redis_elastic
-Version: 0.3.2
+Version: 0.3.3
 Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
 Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
 Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
 Author: Carlos Garcia Garcia
 Author-email: carlos.garcia1.gr1@icloud.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 0.3.1 (Stable release)
+version 0.3.3 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
```

### Comparing `redis_elastic-0.3.2/README.md` & `redis_elastic-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 0.3.1 (Stable release)
+version 0.3.3 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
```

### Comparing `redis_elastic-0.3.2/Warehouse/redis_elastic.py` & `redis_elastic-0.3.3/Warehouse/redis_elastic.py`

 * *Files identical despite different names*

### Comparing `redis_elastic-0.3.2/redis_elastic.egg-info/PKG-INFO` & `redis_elastic-0.3.3/redis_elastic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: redis-elastic
-Version: 0.3.2
+Version: 0.3.3
 Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
 Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
 Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
 Author: Carlos Garcia Garcia
 Author-email: carlos.garcia1.gr1@icloud.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 0.3.1 (Stable release)
+version 0.3.3 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
```

### Comparing `redis_elastic-0.3.2/setup.py` & `redis_elastic-0.3.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup
 
 readme = open("./README.md", "r")
 
 setup(
     name="redis_elastic",
-    version="0.3.2",
+    version="0.3.3",
     description="Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch",
     install_requires=[
         "psycopg2",
         "psycopg2-binary",
-        "functools",
         "redis",
         "elasticsearch==7.13.4",
         "pandas"
     ],
     long_description=readme.read(),
     long_description_content_type='text/markdown',
     author="Carlos Garcia Garcia",
```

