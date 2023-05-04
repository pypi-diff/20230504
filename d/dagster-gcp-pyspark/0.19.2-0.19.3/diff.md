# Comparing `tmp/dagster_gcp_pyspark-0.19.2.tar.gz` & `tmp/dagster_gcp_pyspark-0.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_gcp_pyspark-0.19.2.tar", last modified: Thu Apr 27 19:33:44 2023, max compression
+gzip compressed data, was "dagster_gcp_pyspark-0.19.3.tar", last modified: Thu May  4 17:52:33 2023, max compression
```

## Comparing `dagster_gcp_pyspark-0.19.2.tar` & `dagster_gcp_pyspark-0.19.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:33:44.868216 dagster_gcp_pyspark-0.19.2/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-04-27 18:30:35.000000 dagster_gcp_pyspark-0.19.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-27 18:30:35.000000 dagster_gcp_pyspark-0.19.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-27 19:33:44.868216 dagster_gcp_pyspark-0.19.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      143 2023-04-27 18:30:35.000000 dagster_gcp_pyspark-0.19.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:33:44.868216 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark/
--rw-r--r--   0 root         (0) root         (0)      402 2023-04-27 18:30:35.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:33:44.868216 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:35.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9884 2023-04-27 18:30:35.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 18:30:35.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-27 18:30:35.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:33:44.868216 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-27 19:33:44.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-04-27 19:33:44.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:33:44.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:33:44.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-27 19:33:44.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-27 19:33:44.000000 dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-27 19:33:44.872216 dagster_gcp_pyspark-0.19.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-27 18:30:35.000000 dagster_gcp_pyspark-0.19.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:33.116577 dagster_gcp_pyspark-0.19.3/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 17:52:33.116577 dagster_gcp_pyspark-0.19.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      143 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:33.112577 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:33.112577 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9900 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:52:33.112577 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-04 17:52:33.000000 dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-05-04 17:52:33.116577 dagster_gcp_pyspark-0.19.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-05-04 17:42:14.000000 dagster_gcp_pyspark-0.19.3/setup.py
```

### Comparing `dagster_gcp_pyspark-0.19.2/LICENSE` & `dagster_gcp_pyspark-0.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.19.2/PKG-INFO` & `dagster_gcp_pyspark-0.19.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_gcp_pyspark
-Version: 0.19.2
+Version: 0.19.3
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py` & `dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                     ]
                 )
             ),
         }
 
     def load_input(self, context: InputContext, table_slice: TableSlice, _) -> DataFrame:
         options = _get_bigquery_read_options(table_slice)
-        spark = SparkSession.builder.getOrCreate()
+        spark = SparkSession.builder.getOrCreate()  # type: ignore
 
         if table_slice.partition_dimensions and len(context.asset_partition_keys) == 0:
             return spark.createDataFrame([], StructType([]))
 
         df = (
             spark.read.format("bigquery")
             .options(**options)
```

### Comparing `dagster_gcp_pyspark-0.19.2/dagster_gcp_pyspark.egg-info/PKG-INFO` & `dagster_gcp_pyspark-0.19.3/dagster_gcp_pyspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pyspark
-Version: 0.19.2
+Version: 0.19.3
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.19.2/setup.py` & `dagster_gcp_pyspark-0.19.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.3.2",
-        "dagster-gcp==0.19.2",
+        "dagster==1.3.3",
+        "dagster-gcp==0.19.3",
         "pyspark",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

