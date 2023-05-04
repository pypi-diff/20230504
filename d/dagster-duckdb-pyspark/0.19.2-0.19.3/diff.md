# Comparing `tmp/dagster-duckdb-pyspark-0.19.2.tar.gz` & `tmp/dagster-duckdb-pyspark-0.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pyspark-0.19.2.tar", last modified: Thu Apr 27 19:35:49 2023, max compression
+gzip compressed data, was "dagster-duckdb-pyspark-0.19.3.tar", last modified: Thu May  4 17:53:56 2023, max compression
```

## Comparing `dagster-duckdb-pyspark-0.19.2.tar` & `dagster-duckdb-pyspark-0.19.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:49.608616 dagster-duckdb-pyspark-0.19.2/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-27 18:30:35.000000 dagster-duckdb-pyspark-0.19.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-27 18:30:35.000000 dagster-duckdb-pyspark-0.19.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      637 2023-04-27 19:35:49.608616 dagster-duckdb-pyspark-0.19.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-27 18:30:35.000000 dagster-duckdb-pyspark-0.19.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:49.604616 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark/
--rw-r--r--   0 root         (0) root         (0)      382 2023-04-27 18:30:35.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7484 2023-04-27 18:30:35.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 18:30:35.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-27 18:30:35.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:49.608616 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      637 2023-04-27 19:35:49.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-04-27 19:35:49.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:35:49.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:35:49.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 19:35:49.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-27 19:35:49.000000 dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-04-27 19:35:49.680617 dagster-duckdb-pyspark-0.19.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1549 2023-04-27 18:30:35.000000 dagster-duckdb-pyspark-0.19.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:53:56.189155 dagster-duckdb-pyspark-0.19.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-04 17:42:14.000000 dagster-duckdb-pyspark-0.19.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-04 17:42:14.000000 dagster-duckdb-pyspark-0.19.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      637 2023-05-04 17:53:56.189155 dagster-duckdb-pyspark-0.19.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-04 17:42:14.000000 dagster-duckdb-pyspark-0.19.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:53:56.189155 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-04 17:42:14.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7500 2023-05-04 17:42:14.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 17:42:14.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-04 17:42:14.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:53:56.189155 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-05-04 17:53:56.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2023-05-04 17:53:56.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:53:56.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:53:56.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-04 17:53:56.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-04 17:53:56.000000 dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-04 17:53:56.189155 dagster-duckdb-pyspark-0.19.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-05-04 17:42:14.000000 dagster-duckdb-pyspark-0.19.3/setup.py
```

### Comparing `dagster-duckdb-pyspark-0.19.2/LICENSE` & `dagster-duckdb-pyspark-0.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.19.2/PKG-INFO` & `dagster-duckdb-pyspark-0.19.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.19.2
+Version: 0.19.3
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py` & `dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             }
         )
 
     def load_input(
         self, context: InputContext, table_slice: TableSlice, connection
     ) -> pyspark.sql.DataFrame:
         """Loads the return of the query as the correct type."""
-        spark = SparkSession.builder.getOrCreate()
+        spark = SparkSession.builder.getOrCreate()  # type: ignore
         if table_slice.partition_dimensions and len(context.asset_partition_keys) == 0:
             return spark.createDataFrame([], StructType([]))
 
         pd_df = connection.execute(DuckDbClient.get_select_statement(table_slice)).fetchdf()
         return spark.createDataFrame(pd_df)
 
     @property
```

### Comparing `dagster-duckdb-pyspark-0.19.2/dagster_duckdb_pyspark.egg-info/PKG-INFO` & `dagster-duckdb-pyspark-0.19.3/dagster_duckdb_pyspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.19.2
+Version: 0.19.3
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-pyspark-0.19.2/setup.py` & `dagster-duckdb-pyspark-0.19.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pyspark_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.2",
-        "dagster-duckdb==0.19.2",
+        "dagster==1.3.3",
+        "dagster-duckdb==0.19.3",
         # Pyspark 2.x is incompatible with Python 3.8+
         'pyspark>=3.0.0; python_version >= "3.8"',
         'pyspark>=2.0.2; python_version < "3.8"',
         "pandas<2",  # See: https://github.com/dagster-io/dagster/issues/13339
     ],
     zip_safe=False,
 )
```

