# Comparing `tmp/dbqq-1.3.6.tar.gz` & `tmp/dbqq-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbqq-1.3.6.tar", last modified: Fri Apr 21 02:22:02 2023, max compression
+gzip compressed data, was "dbqq-1.3.7.tar", last modified: Thu May  4 13:05:05 2023, max compression
```

## Comparing `dbqq-1.3.6.tar` & `dbqq-1.3.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:02.026459 dbqq-1.3.6/
--rw-rw-rw-   0        0        0    14130 2023-04-21 02:22:02.025450 dbqq-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    13400 2023-04-21 02:01:14.000000 dbqq-1.3.6/README.md
--rw-rw-rw-   0        0        0     1083 2023-04-21 02:00:16.000000 dbqq-1.3.6/license.md
--rw-rw-rw-   0        0        0     1302 2023-04-21 02:21:41.000000 dbqq-1.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 02:22:02.027473 dbqq-1.3.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:01.903853 dbqq-1.3.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:01.929856 dbqq-1.3.6/src/dbqq/
--rw-rw-rw-   0        0        0      127 2023-04-21 02:00:57.000000 dbqq-1.3.6/src/dbqq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:01.962865 dbqq-1.3.6/src/dbqq/cli/
--rw-rw-rw-   0        0        0        0 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/cli/__init__.py
--rw-rw-rw-   0        0        0      968 2023-04-21 02:14:35.000000 dbqq-1.3.6/src/dbqq/cli/clean_connections.py
--rw-rw-rw-   0        0        0      713 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/cli/initialize_connections.py
--rw-rw-rw-   0        0        0     1295 2023-04-21 02:01:33.000000 dbqq-1.3.6/src/dbqq/cli/run_query.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:01.980871 dbqq-1.3.6/src/dbqq/connectors/
--rw-rw-rw-   0        0        0     1013 2023-04-21 02:01:01.000000 dbqq-1.3.6/src/dbqq/connectors/__init__.py
--rw-rw-rw-   0        0        0     7040 2023-04-21 02:14:45.000000 dbqq-1.3.6/src/dbqq/connectors/_base.py
--rw-rw-rw-   0        0        0     1778 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/connectors/_polar_connector.py
--rw-rw-rw-   0        0        0     5670 2023-04-21 02:21:20.000000 dbqq-1.3.6/src/dbqq/connectors/databricks.py
--rw-rw-rw-   0        0        0     2906 2023-04-21 02:21:20.000000 dbqq-1.3.6/src/dbqq/connectors/mssql.py
--rw-rw-rw-   0        0        0     4747 2023-04-21 02:21:20.000000 dbqq-1.3.6/src/dbqq/connectors/oracle.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:01.983870 dbqq-1.3.6/src/dbqq/data/
--rw-rw-rw-   0        0        0       46 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:01.990874 dbqq-1.3.6/src/dbqq/data/parsed/
--rw-rw-rw-   0        0        0       40 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/data/parsed/__init__.py
--rw-rw-rw-   0        0        0      822 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/data/parsed/sql.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:01.997874 dbqq-1.3.6/src/dbqq/security/
--rw-rw-rw-   0        0        0       86 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/security/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:02.010876 dbqq-1.3.6/src/dbqq/security/cli/
--rw-rw-rw-   0        0        0        0 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/security/cli/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/security/cli/decrypt_yaml.py
--rw-rw-rw-   0        0        0     1036 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/security/cli/encrypt_yaml.py
--rw-rw-rw-   0        0        0     1707 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/security/cli/write_keys.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:02.021880 dbqq-1.3.6/src/dbqq/security/functions/
--rw-rw-rw-   0        0        0      119 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/security/functions/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/security/functions/_functions.py
--rw-rw-rw-   0        0        0     4166 2023-04-21 02:00:16.000000 dbqq-1.3.6/src/dbqq/security/functions/_yaml.py
--rw-rw-rw-   0        0        0     2332 2023-04-21 02:15:05.000000 dbqq-1.3.6/src/dbqq/security/helpers.py
--rw-rw-rw-   0        0        0     5315 2023-04-21 02:14:19.000000 dbqq-1.3.6/src/dbqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:22:01.949863 dbqq-1.3.6/src/dbqq.egg-info/
--rw-rw-rw-   0        0        0    14130 2023-04-21 02:22:01.000000 dbqq-1.3.6/src/dbqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2023-04-21 02:22:01.000000 dbqq-1.3.6/src/dbqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 02:22:01.000000 dbqq-1.3.6/src/dbqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2023-04-21 02:22:01.000000 dbqq-1.3.6/src/dbqq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-04-21 02:22:01.000000 dbqq-1.3.6/src/dbqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-21 02:22:01.000000 dbqq-1.3.6/src/dbqq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.704118 dbqq-1.3.7/
+-rw-rw-rw-   0        0        0    14130 2023-05-04 13:05:05.702117 dbqq-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    13400 2023-05-04 12:58:55.000000 dbqq-1.3.7/README.md
+-rw-rw-rw-   0        0        0     1083 2023-05-04 12:58:55.000000 dbqq-1.3.7/license.md
+-rw-rw-rw-   0        0        0     1302 2023-05-04 13:04:37.000000 dbqq-1.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:05:05.705119 dbqq-1.3.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.567129 dbqq-1.3.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.598117 dbqq-1.3.7/src/dbqq/
+-rw-rw-rw-   0        0        0      127 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.633118 dbqq-1.3.7/src/dbqq/cli/
+-rw-rw-rw-   0        0        0        0 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/cli/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/cli/clean_connections.py
+-rw-rw-rw-   0        0        0      713 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/cli/initialize_connections.py
+-rw-rw-rw-   0        0        0     1295 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/cli/run_query.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.657124 dbqq-1.3.7/src/dbqq/connectors/
+-rw-rw-rw-   0        0        0     1013 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/__init__.py
+-rw-rw-rw-   0        0        0     7040 2023-05-04 13:00:30.000000 dbqq-1.3.7/src/dbqq/connectors/_base.py
+-rw-rw-rw-   0        0        0     1778 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/_polar_connector.py
+-rw-rw-rw-   0        0        0     5670 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/databricks.py
+-rw-rw-rw-   0        0        0     2906 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/mssql.py
+-rw-rw-rw-   0        0        0     4747 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/oracle.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.660119 dbqq-1.3.7/src/dbqq/data/
+-rw-rw-rw-   0        0        0       46 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.668117 dbqq-1.3.7/src/dbqq/data/parsed/
+-rw-rw-rw-   0        0        0       40 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/data/parsed/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/data/parsed/sql.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.673120 dbqq-1.3.7/src/dbqq/security/
+-rw-rw-rw-   0        0        0       86 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.688115 dbqq-1.3.7/src/dbqq/security/cli/
+-rw-rw-rw-   0        0        0        0 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/cli/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/cli/decrypt_yaml.py
+-rw-rw-rw-   0        0        0     1036 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/cli/encrypt_yaml.py
+-rw-rw-rw-   0        0        0     1707 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/cli/write_keys.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.699118 dbqq-1.3.7/src/dbqq/security/functions/
+-rw-rw-rw-   0        0        0      119 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/functions/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/functions/_functions.py
+-rw-rw-rw-   0        0        0     4166 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/functions/_yaml.py
+-rw-rw-rw-   0        0        0     2332 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/helpers.py
+-rw-rw-rw-   0        0        0     5315 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.619120 dbqq-1.3.7/src/dbqq.egg-info/
+-rw-rw-rw-   0        0        0    14130 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      339 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/top_level.txt
```

### Comparing `dbqq-1.3.6/PKG-INFO` & `dbqq-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbqq
-Version: 1.3.6
+Version: 1.3.7
 Summary: quickly connect to and query databases
 Author-email: Chris Mamon <chrisam1993@live.com>
 Project-URL: Homepage, https://github.com/Chr1sC0de/database-quick-query
 Project-URL: Bug Tracker, https://github.com/Chr1sC0de/database-quick-query/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dbqq-1.3.6/README.md` & `dbqq-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/license.md` & `dbqq-1.3.7/license.md`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/pyproject.toml` & `dbqq-1.3.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dbqq"
 description = "quickly connect to and query databases"
-version = "1.3.6"
+version = "1.3.7"
 readme = "README.md"
 dependencies = [
   "tabulate",
   "rsa",
   "pyaml",
   "polars",
   "databricks-sql-connector",
```

### Comparing `dbqq-1.3.6/src/dbqq/cli/clean_connections.py` & `dbqq-1.3.7/src/dbqq/cli/clean_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/cli/initialize_connections.py` & `dbqq-1.3.7/src/dbqq/cli/initialize_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/cli/run_query.py` & `dbqq-1.3.7/src/dbqq/cli/run_query.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/connectors/__init__.py` & `dbqq-1.3.7/src/dbqq/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/connectors/_base.py` & `dbqq-1.3.7/src/dbqq/connectors/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                 < self.cache_metadata.date_lower_bound
             ]
 
             for yaml_file in valid_files:
                 with open(yaml_file, "r") as f:
                     metadata = yaml.safe_load(f)
 
-                if query in metadata[self.meta.QUERY]:
+                if query == metadata[self.meta.QUERY]:
                     parquet_file = pt.Path(metadata[self.meta.PARQUETFILE])
                     if parquet_file.exists():
                         df = pl.scan_parquet(
                             parquet_file, **scan_parquet_kwargs
                         )
                         self.query_info.time_taken = metadata[
                             self.meta.TIMETAKEN
```

### Comparing `dbqq-1.3.6/src/dbqq/connectors/_polar_connector.py` & `dbqq-1.3.7/src/dbqq/connectors/_polar_connector.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/connectors/databricks.py` & `dbqq-1.3.7/src/dbqq/connectors/databricks.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/connectors/mssql.py` & `dbqq-1.3.7/src/dbqq/connectors/mssql.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/connectors/oracle.py` & `dbqq-1.3.7/src/dbqq/connectors/oracle.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/data/parsed/sql.py` & `dbqq-1.3.7/src/dbqq/data/parsed/sql.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/security/cli/decrypt_yaml.py` & `dbqq-1.3.7/src/dbqq/security/cli/decrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/security/cli/encrypt_yaml.py` & `dbqq-1.3.7/src/dbqq/security/cli/encrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/security/cli/write_keys.py` & `dbqq-1.3.7/src/dbqq/security/cli/write_keys.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/security/functions/_functions.py` & `dbqq-1.3.7/src/dbqq/security/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/security/functions/_yaml.py` & `dbqq-1.3.7/src/dbqq/security/functions/_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/security/helpers.py` & `dbqq-1.3.7/src/dbqq/security/helpers.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq/utils.py` & `dbqq-1.3.7/src/dbqq/utils.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.6/src/dbqq.egg-info/PKG-INFO` & `dbqq-1.3.7/src/dbqq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbqq
-Version: 1.3.6
+Version: 1.3.7
 Summary: quickly connect to and query databases
 Author-email: Chris Mamon <chrisam1993@live.com>
 Project-URL: Homepage, https://github.com/Chr1sC0de/database-quick-query
 Project-URL: Bug Tracker, https://github.com/Chr1sC0de/database-quick-query/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dbqq-1.3.6/src/dbqq.egg-info/SOURCES.txt` & `dbqq-1.3.7/src/dbqq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

