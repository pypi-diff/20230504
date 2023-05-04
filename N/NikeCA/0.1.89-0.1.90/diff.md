# Comparing `tmp/NikeCA-0.1.89.tar.gz` & `tmp/NikeCA-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.89.tar", last modified: Wed May  3 21:35:53 2023, max compression
+gzip compressed data, was "NikeCA-0.1.90.tar", last modified: Thu May  4 17:13:58 2023, max compression
```

## Comparing `NikeCA-0.1.89.tar` & `NikeCA-0.1.90.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 21:35:53.957646 NikeCA-0.1.89/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.89/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 21:35:53.957148 NikeCA-0.1.89/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.89/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-03 21:35:53.957765 NikeCA-0.1.89/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-03 21:35:25.000000 NikeCA-0.1.89/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 21:35:53.948017 NikeCA-0.1.89/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 21:35:53.949882 NikeCA-0.1.89/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 21:35:53.950760 NikeCA-0.1.89/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 21:35:53.953749 NikeCA-0.1.89/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6070 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-03 21:35:53.956597 NikeCA-0.1.89/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-03 21:35:53.000000 NikeCA-0.1.89/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-03 21:35:53.000000 NikeCA-0.1.89/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-03 21:35:53.000000 NikeCA-0.1.89/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-03 21:35:53.000000 NikeCA-0.1.89/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-03 21:35:53.000000 NikeCA-0.1.89/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    24675 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14422 2023-05-03 04:38:16.000000 NikeCA-0.1.89/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    12713 2023-05-03 18:56:04.000000 NikeCA-0.1.89/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.89/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-04 17:13:58.988154 NikeCA-0.1.90/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.1.90/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-04 17:13:58.987767 NikeCA-0.1.90/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.1.90/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-04 17:13:58.988290 NikeCA-0.1.90/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-04 17:13:30.000000 NikeCA-0.1.90/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-04 17:13:58.977808 NikeCA-0.1.90/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-04 17:13:58.979934 NikeCA-0.1.90/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3969 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-04 17:13:58.981379 NikeCA-0.1.90/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-04 17:13:58.983973 NikeCA-0.1.90/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6070 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-04 17:13:58.987179 NikeCA-0.1.90/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18012 2023-05-04 17:13:58.000000 NikeCA-0.1.90/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-04 17:13:58.000000 NikeCA-0.1.90/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-04 17:13:58.000000 NikeCA-0.1.90/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-04 17:13:58.000000 NikeCA-0.1.90/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-04 17:13:58.000000 NikeCA-0.1.90/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      415 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23873 2023-05-04 17:11:39.000000 NikeCA-0.1.90/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.1.90/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.1.90/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.1.90/src/__init__.py
```

### Comparing `NikeCA-0.1.89/LICENSE` & `NikeCA-0.1.90/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/PKG-INFO` & `NikeCA-0.1.90/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.89
+Version: 0.1.90
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.89/README.md` & `NikeCA-0.1.90/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/setup.py` & `NikeCA-0.1.90/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.89',
+	version='0.1.90',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"Dashboards/__init__",
```

### Comparing `NikeCA-0.1.89/src/Dashboards/Dashboards.py` & `NikeCA-0.1.90/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.1.90/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.1.90/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.1.90/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.90/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.89
+Version: 0.1.90
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.89/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.1.90/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.90/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/NikeQA.py` & `NikeCA-0.1.90/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/NikeSF.py` & `NikeCA-0.1.90/src/NikeSF.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 
     # Constructor
     def __init__(self, username: str, warehouse: str, role: str, database: str = None, schema: str = None,
                  table: str = None, column_name: str = None, col_and_or: str = 'AND', get_ex_val: bool = None,
                  like_flag: bool = False, sample_table: bool = False, sample_val: bool = False,
                  table_sample: dict = None, dtypes_conv=None, query='', separate_dataframes: bool = False,
                  tables: list | str | None = None, save_path: str | None = None, date_min: str | None = None,
-                 date_max: str | None = None, column_filters: list | None = None, polars: bool = False,
-                 filter_schemas: list | None = None, recursive: bool = False):
+                 date_max: str | None = None, column_filters: list | None = None, polars: bool = False):
         """
         Parameters:
 
             username (str): The Snowflake account username.
             warehouse (str): The Snowflake warehouse to use.
             role (str): The Snowflake role to use.
             database (str, optional): The Snowflake database to use (default is None).
@@ -241,30 +240,14 @@
     def polars(self):
         return self.__polars
 
     @polars.setter
     def polars(self, value):
         self.__polars = value
 
-    @property
-    def filter_schemas(self):
-        return self.__filter_schemas
-
-    @filter_schemas.setter
-    def filter_schemas(self, value):
-        self.__filter_schemas = value
-
-    @property
-    def recursive(self):
-        return self.__recursive
-
-    @recursive.setter
-    def recursive(self, value):
-        self.__recursive = value
-
     def build_search_query(self
                            , inp_db: str = None
                            , schema: str = None
                            , table: str = None
                            , column_name=None
                            , like_flag: bool = False
                            , col_and_or: str = 'AND'
@@ -499,16 +482,14 @@
                                tables: str | list | None = None,
                                username: str | None = None,
                                warehouse: str | None = None,
                                role: str | None = None,
                                database: str | None = None,
                                schema: str | list | None = None,
                                save_path: str = None,
-                               filter_schemas: list | None = None,
-                               recursive: bool = False
                                ):
 
         """
 
         :param recursive:
         :param filter_schemas:
         :param save_path:
@@ -531,23 +512,18 @@
             role = self.__role
         if database is None:
             database = self.__database
         if schema is None:
             schema = self.__schema
         if save_path is None:
             save_path = self.__save_path
-        if filter_schemas is None:
-            filter_schemas = self.__filter_schemas
-        if not recursive:
-            recursive = self.__recursive
 
         return SnowflakeData.snowflake_dependencies(self, tables=tables, username=username,
                                                     warehouse=warehouse, role=role, database=database,
-                                                    schema=schema, save_path=save_path, filter_schemas=filter_schemas,
-                                                    recursive=recursive)
+                                                    schema=schema, save_path=save_path)
 
     def imp_summary_dashboard(self
                               , username: str | None = None
                               , warehouse: str | None = None
                               , database: str | None = None
                               , role: str | None = None
                               , date_min: str = '1900-01-01'
```

### Comparing `NikeCA-0.1.89/src/_BuildSearchQuery.py` & `NikeCA-0.1.90/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/_GitHub.py` & `NikeCA-0.1.90/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/_QA.py` & `NikeCA-0.1.90/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/_SearchFiles.py` & `NikeCA-0.1.90/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.89/src/_SnowflakeData.py` & `NikeCA-0.1.90/src/_SnowflakeData.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,24 +111,21 @@
                     print(f"Could not pull {row['COLUMN_NAME']} for table: {row['TABLE_NAME']}")
                     print(e)
                     continue
 
         return results_fin
 
     def snowflake_dependencies(self, tables: str | list, username: str, warehouse: str, role: str,
-                               database: str | None = None, schema: str | list | None = None, save_path: str = None,
-                               filter_schemas: list | None = None, recursive: bool = False):
+                               database: str | None = None, schema: str | list | None = None, save_path: str = None):
 
         return _SnowflakeDependencies.SnowflakeDependencies.snowflake_dependencies(self, tables=tables,
                                                                                    username=username,
                                                                                    warehouse=warehouse, role=role,
                                                                                    database=database, schema=schema,
-                                                                                   save_path=save_path,
-                                                                                   filter_schemas=filter_schemas,
-                                                                                   recursive=recursive)
+                                                                                   save_path=save_path)
 
     def optimize_tbl_mem(self, username: str, warehouse: str, role: str, database: str = None, schema: str = None,
                          table_name: str = None, pull_all_cols=True, run_debugging: bool = False,
                          query=None):
 
         import numpy as np
         from NikeQA import QA
```

### Comparing `NikeCA-0.1.89/src/_SnowflakePull.py` & `NikeCA-0.1.90/src/_SnowflakePull.py`

 * *Files identical despite different names*

