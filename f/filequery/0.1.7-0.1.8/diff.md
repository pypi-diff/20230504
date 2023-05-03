# Comparing `tmp/filequery-0.1.7.tar.gz` & `tmp/filequery-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filequery-0.1.7.tar", last modified: Thu Mar 23 01:11:38 2023, max compression
+gzip compressed data, was "filequery-0.1.8.tar", last modified: Wed May  3 23:56:22 2023, max compression
```

## Comparing `filequery-0.1.7.tar` & `filequery-0.1.8.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-03-23 01:11:38.039143 filequery-0.1.7/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1818 2023-02-19 00:56:16.000000 filequery-0.1.7/.gitignore
--rw-rw-r--   0 markus    (1000) markus    (1000)     1070 2023-02-19 00:24:28.000000 filequery-0.1.7/LICENSE
--rw-rw-r--   0 markus    (1000) markus    (1000)      330 2023-02-25 04:29:27.000000 filequery-0.1.7/Makefile
--rw-rw-r--   0 markus    (1000) markus    (1000)     4092 2023-03-23 01:11:38.039143 filequery-0.1.7/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     3727 2023-03-23 01:10:40.000000 filequery-0.1.7/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-03-23 01:11:38.035143 filequery-0.1.7/example/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-03-23 01:11:38.035143 filequery-0.1.7/example/config_files/
--rw-rw-r--   0 markus    (1000) markus    (1000)       86 2023-03-10 02:53:30.000000 filequery-0.1.7/example/config_files/example0.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      115 2023-03-10 02:53:30.000000 filequery-0.1.7/example/config_files/example1.json
--rw-rw-r--   0 markus    (1000) markus    (1000)       94 2023-03-10 02:53:30.000000 filequery-0.1.7/example/config_files/example2.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      117 2023-03-10 02:53:30.000000 filequery-0.1.7/example/config_files/example3.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      155 2023-03-10 02:53:30.000000 filequery-0.1.7/example/config_files/example4.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      186 2023-03-23 01:10:40.000000 filequery-0.1.7/example/config_files/example5.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      147 2023-03-23 01:10:40.000000 filequery-0.1.7/example/config_files/example6.json
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-03-23 01:11:38.035143 filequery-0.1.7/example/data/
--rw-rw-r--   0 markus    (1000) markus    (1000)      353 2023-03-11 23:35:48.000000 filequery-0.1.7/example/data/json_test.json
--rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-02-24 02:58:55.000000 filequery-0.1.7/example/data/test.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)       69 2023-02-24 02:59:42.000000 filequery-0.1.7/example/data/test1.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)      231 2023-03-11 23:35:48.000000 filequery-0.1.7/example/json_list_test.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      200 2023-03-11 23:35:48.000000 filequery-0.1.7/example/json_test.json
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-03-23 01:11:38.039143 filequery-0.1.7/example/queries/
--rw-rw-r--   0 markus    (1000) markus    (1000)       75 2023-02-24 03:03:29.000000 filequery-0.1.7/example/queries/join.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.1.7/example/queries/json_csv_join.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.1.7/example/queries/json_query.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)      124 2023-02-27 01:13:38.000000 filequery-0.1.7/example/queries/multi_query.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-02-21 01:39:12.000000 filequery-0.1.7/example/test.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)      640 2023-03-23 01:10:40.000000 filequery-0.1.7/pyproject.toml
--rw-rw-r--   0 markus    (1000) markus    (1000)      602 2023-03-11 23:35:48.000000 filequery-0.1.7/requirements-dev.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       44 2023-03-11 23:35:48.000000 filequery-0.1.7/requirements.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-03-23 01:11:38.039143 filequery-0.1.7/setup.cfg
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-03-23 01:11:38.031143 filequery-0.1.7/src/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-03-23 01:11:38.039143 filequery-0.1.7/src/filequery/
--rw-rw-r--   0 markus    (1000) markus    (1000)     5211 2023-03-23 01:10:40.000000 filequery-0.1.7/src/filequery/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)       78 2023-02-18 23:29:05.000000 filequery-0.1.7/src/filequery/__main__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      230 2023-03-23 01:10:40.000000 filequery-0.1.7/src/filequery/file_query_args.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3056 2023-03-23 01:10:40.000000 filequery-0.1.7/src/filequery/filedb.py
--rw-rw-r--   0 markus    (1000) markus    (1000)       86 2023-03-11 23:35:48.000000 filequery-0.1.7/src/filequery/filetype.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     2035 2023-03-23 01:10:40.000000 filequery-0.1.7/src/filequery/queryresult.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-03-23 01:11:38.039143 filequery-0.1.7/src/filequery.egg-info/
--rw-rw-r--   0 markus    (1000) markus    (1000)     4092 2023-03-23 01:11:38.000000 filequery-0.1.7/src/filequery.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1028 2023-03-23 01:11:38.000000 filequery-0.1.7/src/filequery.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-03-23 01:11:38.000000 filequery-0.1.7/src/filequery.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       55 2023-03-23 01:11:38.000000 filequery-0.1.7/src/filequery.egg-info/entry_points.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       44 2023-03-23 01:11:38.000000 filequery-0.1.7/src/filequery.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       10 2023-03-23 01:11:38.000000 filequery-0.1.7/src/filequery.egg-info/top_level.txt
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-03-23 01:11:38.039143 filequery-0.1.7/tests/
--rw-rw-r--   0 markus    (1000) markus    (1000)        0 2023-02-19 00:27:10.000000 filequery-0.1.7/tests/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     8733 2023-03-23 01:10:40.000000 filequery-0.1.7/tests/test_filequery.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-03 23:56:22.199903 filequery-0.1.8/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1818 2023-02-19 00:56:16.000000 filequery-0.1.8/.gitignore
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1070 2023-02-19 00:24:28.000000 filequery-0.1.8/LICENSE
+-rw-rw-r--   0 markus    (1000) markus    (1000)      330 2023-02-25 04:29:27.000000 filequery-0.1.8/Makefile
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4264 2023-05-03 23:56:22.195903 filequery-0.1.8/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3899 2023-05-03 23:52:52.000000 filequery-0.1.8/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-03 23:56:22.187903 filequery-0.1.8/example/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-03 23:56:22.191903 filequery-0.1.8/example/config_files/
+-rw-rw-r--   0 markus    (1000) markus    (1000)       86 2023-03-10 02:53:30.000000 filequery-0.1.8/example/config_files/example0.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      115 2023-03-10 02:53:30.000000 filequery-0.1.8/example/config_files/example1.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)       94 2023-03-10 02:53:30.000000 filequery-0.1.8/example/config_files/example2.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      117 2023-03-10 02:53:30.000000 filequery-0.1.8/example/config_files/example3.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      155 2023-03-10 02:53:30.000000 filequery-0.1.8/example/config_files/example4.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      186 2023-03-23 01:10:40.000000 filequery-0.1.8/example/config_files/example5.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      147 2023-03-23 01:10:40.000000 filequery-0.1.8/example/config_files/example6.json
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-03 23:56:22.191903 filequery-0.1.8/example/data/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      353 2023-03-11 23:35:48.000000 filequery-0.1.8/example/data/json_test.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-02-24 02:58:55.000000 filequery-0.1.8/example/data/test.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)       69 2023-02-24 02:59:42.000000 filequery-0.1.8/example/data/test1.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)      231 2023-03-11 23:35:48.000000 filequery-0.1.8/example/json_list_test.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      200 2023-03-11 23:35:48.000000 filequery-0.1.8/example/json_test.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      260 2023-05-03 23:49:19.000000 filequery-0.1.8/example/ndjson_test.ndjson
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-03 23:56:22.195903 filequery-0.1.8/example/queries/
+-rw-rw-r--   0 markus    (1000) markus    (1000)       75 2023-02-24 03:03:29.000000 filequery-0.1.8/example/queries/join.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.1.8/example/queries/json_csv_join.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.1.8/example/queries/json_query.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)      124 2023-02-27 01:13:38.000000 filequery-0.1.8/example/queries/multi_query.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-02-21 01:39:12.000000 filequery-0.1.8/example/test.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)      640 2023-05-03 23:45:26.000000 filequery-0.1.8/pyproject.toml
+-rw-rw-r--   0 markus    (1000) markus    (1000)      602 2023-03-11 23:35:48.000000 filequery-0.1.8/requirements-dev.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       44 2023-03-11 23:35:48.000000 filequery-0.1.8/requirements.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-05-03 23:56:22.199903 filequery-0.1.8/setup.cfg
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-03 23:56:22.187903 filequery-0.1.8/src/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-03 23:56:22.195903 filequery-0.1.8/src/filequery/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     5211 2023-03-23 01:10:40.000000 filequery-0.1.8/src/filequery/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)       78 2023-02-18 23:29:05.000000 filequery-0.1.8/src/filequery/__main__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      230 2023-03-23 01:10:40.000000 filequery-0.1.8/src/filequery/file_query_args.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3192 2023-05-03 23:51:12.000000 filequery-0.1.8/src/filequery/filedb.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      101 2023-05-03 23:47:21.000000 filequery-0.1.8/src/filequery/filetype.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2035 2023-03-23 01:10:40.000000 filequery-0.1.8/src/filequery/queryresult.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-03 23:56:22.195903 filequery-0.1.8/src/filequery.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4264 2023-05-03 23:56:22.000000 filequery-0.1.8/src/filequery.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1055 2023-05-03 23:56:22.000000 filequery-0.1.8/src/filequery.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-05-03 23:56:22.000000 filequery-0.1.8/src/filequery.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       55 2023-05-03 23:56:22.000000 filequery-0.1.8/src/filequery.egg-info/entry_points.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       44 2023-05-03 23:56:22.000000 filequery-0.1.8/src/filequery.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       10 2023-05-03 23:56:22.000000 filequery-0.1.8/src/filequery.egg-info/top_level.txt
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-05-03 23:56:22.195903 filequery-0.1.8/tests/
+-rw-rw-r--   0 markus    (1000) markus    (1000)        0 2023-02-19 00:27:10.000000 filequery-0.1.8/tests/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     8959 2023-05-03 23:54:36.000000 filequery-0.1.8/tests/test_filequery.py
```

### Comparing `filequery-0.1.7/.gitignore` & `filequery-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `filequery-0.1.7/LICENSE` & `filequery-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `filequery-0.1.7/PKG-INFO` & `filequery-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filequery
-Version: 0.1.7
+Version: 0.1.8
 Summary: Query CSV and Parquet files using SQL
 Author-email: Markus Hutnik <markus@markushutnik.com>
 License: MIT
 Project-URL: repository, https://github.com/MarkyMan4/filequery
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -61,14 +61,18 @@
 ```bash
 filequery --filesdir example/data --query_file example/queries/json_csv_join.sql # SQL file joining data from JSON and CSV files
 ```
 ```bash
 filequery --filesdir example/test.csv --query 'select * from test; select sum(col3) from test;' # output multiple query results to multiple files
 ```
 
+```bash
+filequery --filename example/ndjson_test.ndjson --query 'select id, value, nested.subid, nested.subval from ndjson_test' # query nested JSON in an ndjson file
+```
+
 You can also provide a config file instead of specifying the arguments when running the command.
 
 ```bash
 filequery --config <path to config file>
 ```
 
 The config file should be a json file. See example config file contents below.
```

### Comparing `filequery-0.1.7/README.md` & `filequery-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 ```bash
 filequery --filesdir example/data --query_file example/queries/json_csv_join.sql # SQL file joining data from JSON and CSV files
 ```
 ```bash
 filequery --filesdir example/test.csv --query 'select * from test; select sum(col3) from test;' # output multiple query results to multiple files
 ```
 
+```bash
+filequery --filename example/ndjson_test.ndjson --query 'select id, value, nested.subid, nested.subval from ndjson_test' # query nested JSON in an ndjson file
+```
+
 You can also provide a config file instead of specifying the arguments when running the command.
 
 ```bash
 filequery --config <path to config file>
 ```
 
 The config file should be a json file. See example config file contents below.
```

### Comparing `filequery-0.1.7/pyproject.toml` & `filequery-0.1.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 description = "Query CSV and Parquet files using SQL"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 license = {text = "MIT"}
-version = "0.1.7"
+version = "0.1.8"
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.scripts]
 filequery = "filequery:fq_cli_handler"
```

### Comparing `filequery-0.1.7/requirements-dev.txt` & `filequery-0.1.8/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `filequery-0.1.7/src/filequery/__init__.py` & `filequery-0.1.8/src/filequery/__init__.py`

 * *Files identical despite different names*

### Comparing `filequery-0.1.7/src/filequery/filedb.py` & `filequery-0.1.8/src/filequery/filedb.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from .filetype import FileType
 from .queryresult import QueryResult
 from typing import List
 
 READ_FUNCS = {
     FileType.CSV: 'read_csv_auto',
     FileType.PARQUET: 'read_parquet',
-    FileType.JSON: 'read_json_auto'
+    FileType.JSON: 'read_json_auto',
+    FileType.NDJSON: 'read_ndjson_auto'
 }
 
 class FileDb:
     def __init__(self, filepath: str):
         """
         FileDb constructor
 
@@ -25,14 +26,16 @@
             base_filename = os.path.basename(filename).lower()
             filetype = FileType.CSV
             
             if base_filename.endswith('.parquet'):
                 filetype = FileType.PARQUET
             elif base_filename.endswith('.json'):
                 filetype = FileType.JSON
+            elif base_filename.endswith('.ndjson'):
+                filetype = FileType.NDJSON
             
             table_name = os.path.splitext(base_filename)[0]
             read_func = READ_FUNCS[filetype]
 
             self.db.execute(f"create table {table_name} as select * from {read_func}('{filename}');")
 
         if os.path.isdir(filepath):
```

### Comparing `filequery-0.1.7/src/filequery/queryresult.py` & `filequery-0.1.8/src/filequery/queryresult.py`

 * *Files identical despite different names*

### Comparing `filequery-0.1.7/src/filequery.egg-info/PKG-INFO` & `filequery-0.1.8/src/filequery.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filequery
-Version: 0.1.7
+Version: 0.1.8
 Summary: Query CSV and Parquet files using SQL
 Author-email: Markus Hutnik <markus@markushutnik.com>
 License: MIT
 Project-URL: repository, https://github.com/MarkyMan4/filequery
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -61,14 +61,18 @@
 ```bash
 filequery --filesdir example/data --query_file example/queries/json_csv_join.sql # SQL file joining data from JSON and CSV files
 ```
 ```bash
 filequery --filesdir example/test.csv --query 'select * from test; select sum(col3) from test;' # output multiple query results to multiple files
 ```
 
+```bash
+filequery --filename example/ndjson_test.ndjson --query 'select id, value, nested.subid, nested.subval from ndjson_test' # query nested JSON in an ndjson file
+```
+
 You can also provide a config file instead of specifying the arguments when running the command.
 
 ```bash
 filequery --config <path to config file>
 ```
 
 The config file should be a json file. See example config file contents below.
```

### Comparing `filequery-0.1.7/src/filequery.egg-info/SOURCES.txt` & `filequery-0.1.8/src/filequery.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Makefile
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 example/json_list_test.json
 example/json_test.json
+example/ndjson_test.ndjson
 example/test.csv
 example/config_files/example0.json
 example/config_files/example1.json
 example/config_files/example2.json
 example/config_files/example3.json
 example/config_files/example4.json
 example/config_files/example5.json
```

### Comparing `filequery-0.1.7/tests/test_filequery.py` & `filequery-0.1.8/tests/test_filequery.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,20 @@
                 test t1
                 inner join test1 t2
                 on t1.col1 = t2.col1;
         """)
 
         self.assertEqual(len(res.records), 2)
 
+    def test_ndjson_file(self):
+        fdb = FileDb('example/ndjson_test.ndjson')
+        res = fdb.exec_query('select id, value, nested.subid, nested.subval from ndjson_test')
+
+        self.assertEqual(len(res.records), 4)
+
 class TestFileQueryCli(unittest.TestCase):
 
     #####################################################
     # tests for invalid arguments
     #####################################################
 
     def test_no_filename_or_filesdir(self):
```

