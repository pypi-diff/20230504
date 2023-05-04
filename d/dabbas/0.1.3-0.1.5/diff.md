# Comparing `tmp/dabbas-0.1.3.tar.gz` & `tmp/dabbas-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dabbas-0.1.3.tar", last modified: Wed Apr 19 13:35:40 2023, max compression
+gzip compressed data, was "dabbas-0.1.5.tar", last modified: Thu May  4 10:31:13 2023, max compression
```

## Comparing `dabbas-0.1.3.tar` & `dabbas-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-04-19 13:35:40.065752 dabbas-0.1.3/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-04-19 13:35:40.065582 dabbas-0.1.3/PKG-INFO
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-04-19 13:35:40.063574 dabbas-0.1.3/dabbas.egg-info/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-04-19 13:35:40.000000 dabbas-0.1.3/dabbas.egg-info/PKG-INFO
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      255 2023-04-19 13:35:40.000000 dabbas-0.1.3/dabbas.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)        1 2023-04-19 13:35:40.000000 dabbas-0.1.3/dabbas.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       36 2023-04-19 13:35:40.000000 dabbas-0.1.3/dabbas.egg-info/entry_points.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       73 2023-04-19 13:35:40.000000 dabbas-0.1.3/dabbas.egg-info/requires.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)        3 2023-04-19 13:35:40.000000 dabbas-0.1.3/dabbas.egg-info/top_level.txt
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-04-19 13:35:40.065227 dabbas-0.1.3/db/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       86 2023-04-19 11:17:10.000000 dabbas-0.1.3/db/__init__.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2399 2023-04-19 03:44:35.000000 dabbas-0.1.3/db/cache.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      879 2023-04-19 13:20:31.000000 dabbas-0.1.3/db/connection.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2826 2023-04-19 05:59:36.000000 dabbas-0.1.3/db/main.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     9675 2023-04-19 13:33:28.000000 dabbas-0.1.3/db/map.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       38 2023-04-19 13:35:40.065798 dabbas-0.1.3/setup.cfg
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      808 2023-04-19 13:35:17.000000 dabbas-0.1.3/setup.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-04 10:31:13.948201 dabbas-0.1.5/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-04 10:31:13.948041 dabbas-0.1.5/PKG-INFO
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-04 10:31:13.945988 dabbas-0.1.5/atlas/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       21 2023-04-23 17:17:29.000000 dabbas-0.1.5/atlas/__init__.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     6280 2023-04-24 17:54:58.000000 dabbas-0.1.5/atlas/atlas.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     8113 2023-04-24 09:22:52.000000 dabbas-0.1.5/atlas/boundary.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1385 2023-04-23 19:44:53.000000 dabbas-0.1.5/atlas/db.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2793 2023-04-23 19:43:28.000000 dabbas-0.1.5/atlas/schema.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-04 10:31:13.946678 dabbas-0.1.5/dabbas/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      134 2023-04-19 15:30:00.000000 dabbas-0.1.5/dabbas/__init__.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2399 2023-04-19 03:44:35.000000 dabbas-0.1.5/dabbas/cache.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1079 2023-04-24 09:25:19.000000 dabbas-0.1.5/dabbas/connection.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2748 2023-04-19 15:29:41.000000 dabbas-0.1.5/dabbas/main.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     5366 2023-04-23 18:14:37.000000 dabbas-0.1.5/dabbas/map.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-04 10:31:13.947831 dabbas-0.1.5/dabbas.egg-info/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-04 10:31:13.000000 dabbas-0.1.5/dabbas.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      354 2023-05-04 10:31:13.000000 dabbas-0.1.5/dabbas.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)        1 2023-05-04 10:31:13.000000 dabbas-0.1.5/dabbas.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       58 2023-05-04 10:31:13.000000 dabbas-0.1.5/dabbas.egg-info/entry_points.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      101 2023-05-04 10:31:13.000000 dabbas-0.1.5/dabbas.egg-info/requires.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       13 2023-05-04 10:31:13.000000 dabbas-0.1.5/dabbas.egg-info/top_level.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       38 2023-05-04 10:31:13.948240 dabbas-0.1.5/setup.cfg
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      895 2023-05-04 10:31:09.000000 dabbas-0.1.5/setup.py
```

### Comparing `dabbas-0.1.3/db/cache.py` & `dabbas-0.1.5/dabbas/cache.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.3/db/connection.py` & `dabbas-0.1.5/dabbas/connection.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def connection_url():
     pg_user = os.environ['PG_USER']
     pg_password = os.environ['PG_PASSWORD']
     pg_host = os.environ['PG_HOST']
     pg_dbname = os.environ['PG_DBNAME']
     return f'postgresql://{pg_user}:{pg_password}@{pg_host}:5432/{pg_dbname}'
 
+
 def connect():
     pg_user = os.environ['PG_USER']
     pg_password = os.environ['PG_PASSWORD']
     pg_host = os.environ['PG_HOST']
     pg_dbname = os.environ['PG_DBNAME']
 
     import psycopg2
@@ -25,14 +26,23 @@
     return conn
 
 
 def query(sql):
     conn = connect()
     cur = conn.cursor()
 
-    # Execute query and fetch results
-    cur.execute(sql)
-    results = cur.fetchall()
-    cur.close()
-    conn.close()
-    return cur.description, results
+    try:
+        # Execute query and fetch results
+        cur.execute(sql)
+        results = cur.fetchall()
+        cur.close()
+        conn.close()
+    except Exception as e:
+        cur.close()
+        conn.close()
+        raise e
+    finally:
+        if cur is not None:
+            cur.close()
+        conn.close()
 
+    return cur.description, results
```

### Comparing `dabbas-0.1.3/db/main.py` & `dabbas-0.1.5/dabbas/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
 import subprocess
 import sys
 import argparse
 import os.path
-import pandas as pd
-
-from .connection import query
+from .map import read_sql
 
 
 def download(args):
-    cols, results = query(args.query)
     print('downloading')
-    pd.DataFrame(results, columns=[desc[0] for desc in cols]).to_csv(
+    print(args.query)
+    read_sql(args.query).to_csv(
         args.output_file, index=False)
 
 
 def upload(args):
     # Read environment variables
     pg_user = os.environ['PG_USER']
     pg_password = os.environ['PG_PASSWORD']
```

### Comparing `dabbas-0.1.3/setup.py` & `dabbas-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dabbas",
-    version="0.1.3",
+    version="0.1.5",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "db = db.main:main",
+            "dabbas = db.main:main",
         ],
     },
     install_requires=[
         "pandas_flavor",
         "SQLAlchemy",
         "pandas",
         "geopandas",
         "psycopg2-binary",
         "shapely",
-        "folium"
+        "folium",
+        "strawberry-graphql",
+        "supabase"
         # Add any required dependencies here
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

