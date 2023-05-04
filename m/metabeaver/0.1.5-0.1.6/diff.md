# Comparing `tmp/metabeaver-0.1.5.tar.gz` & `tmp/metabeaver-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.1.5.tar", last modified: Wed May  3 18:43:17 2023, max compression
+gzip compressed data, was "metabeaver-0.1.6.tar", last modified: Thu May  4 18:05:13 2023, max compression
```

## Comparing `metabeaver-0.1.5.tar` & `metabeaver-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:43:17.235403 metabeaver-0.1.5/
--rw-rw-rw-   0        0        0      221 2023-05-03 18:43:17.234404 metabeaver-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 18:43:17.200155 metabeaver-0.1.5/metabeaver/
-drwxrwxrwx   0        0        0        0 2023-05-03 18:43:17.222293 metabeaver-0.1.5/metabeaver/GoogleCloudPlatform/
-drwxrwxrwx   0        0        0        0 2023-05-03 18:43:17.226311 metabeaver-0.1.5/metabeaver/GoogleCloudPlatform/BigQuery/
--rw-rw-rw-   0        0        0     2913 2023-05-02 16:05:58.000000 metabeaver-0.1.5/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.5/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-02 11:50:11.000000 metabeaver-0.1.5/metabeaver/GoogleCloudPlatform/BigQuery/testingTables.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.5/metabeaver/GoogleCloudPlatform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:43:17.229300 metabeaver-0.1.5/metabeaver/InstallationScripts/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.5/metabeaver/InstallationScripts/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.1.5/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:43:17.230298 metabeaver-0.1.5/metabeaver/MetaProgramming/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.5/metabeaver/MetaProgramming/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:43:17.232300 metabeaver-0.1.5/metabeaver/Testing/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.5/metabeaver/Testing/__init__.py
--rw-rw-rw-   0        0        0     1804 2023-04-26 12:07:06.000000 metabeaver-0.1.5/metabeaver/Testing/concatenateDataXLSX.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.5/metabeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:43:17.220784 metabeaver-0.1.5/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      221 2023-05-03 18:43:17.000000 metabeaver-0.1.5/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-05-03 18:43:17.000000 metabeaver-0.1.5/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:43:17.000000 metabeaver-0.1.5/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-03 18:43:17.000000 metabeaver-0.1.5/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 18:43:17.000000 metabeaver-0.1.5/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 18:43:17.235403 metabeaver-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-05-03 18:42:10.000000 metabeaver-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.355059 metabeaver-0.1.6/
+-rw-rw-rw-   0        0        0      221 2023-05-04 18:05:13.354060 metabeaver-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.326463 metabeaver-0.1.6/metabeaver/
+drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.342538 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/
+drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.347543 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/BigQuery/
+-rw-rw-rw-   0        0        0     3142 2023-05-04 17:59:02.000000 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 11:50:11.000000 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/BigQuery/testingTables.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.349538 metabeaver-0.1.6/metabeaver/InstallationScripts/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/InstallationScripts/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.1.6/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.350535 metabeaver-0.1.6/metabeaver/MetaProgramming/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/MetaProgramming/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.353079 metabeaver-0.1.6/metabeaver/Testing/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/Testing/__init__.py
+-rw-rw-rw-   0        0        0     1804 2023-04-26 12:07:06.000000 metabeaver-0.1.6/metabeaver/Testing/concatenateDataXLSX.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.6/metabeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:05:13.341531 metabeaver-0.1.6/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 18:05:13.000000 metabeaver-0.1.6/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 18:05:13.355059 metabeaver-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-05-04 18:05:02.000000 metabeaver-0.1.6/setup.py
```

### Comparing `metabeaver-0.1.5/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py` & `metabeaver-0.1.6/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from typing import List
 import pandas as pd
 import numpy as np
 from google.cloud import bigquery
 
 
-def create_bigquery_table(project_id, tableset, table_name, schema):
+def create_bigquery_table(credentials, project_id, tableset, table_name, schema):
     """Creates a BigQuery table in the specified tableset with the given table name and schema.
 
     Args:
+        credentials (google.auth.credentials.Credentials): The credentials to use to authenticate with BigQuery.
         project_id (str): The project ID for the BigQuery table.
         tableset (str): The tableset to create the table in.
         table_name (str): The name for the new BigQuery table.
         schema (list[google.cloud.bigquery.SchemaField]): The schema for the new BigQuery table.
 
     Returns:
         google.cloud.bigquery.table.Table: The newly created BigQuery table.
     """
     # Create the BigQuery client
-    client = bigquery.Client(project=project_id)
+    client = bigquery.Client(project=project_id, credentials=credentials)
 
     # Get a reference to the table
     table_ref = client.dataset(tableset).table(table_name)
 
     # Create the table object
     table = bigquery.Table(table_ref, schema=schema)
 
     # Create the table in BigQuery
     table = client.create_table(table)
 
     # Return the new table object
     return table
 
 
+# Maps Python primitive types and numpy/panda types to BigQuery equivalents
 def create_schema(items: List, field_names: List[str]) -> List[bigquery.SchemaField]:
     """
     Creates a BigQuery schema based on a list of items.
 
     :param items: List of items to determine schema from.
     :param field_names: List of field names for each item in the list.
                         If not specified, default names are used.
```

### Comparing `metabeaver-0.1.5/metabeaver/InstallationScripts/autoGenerateRequirementsText.py` & `metabeaver-0.1.6/metabeaver/InstallationScripts/autoGenerateRequirementsText.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.1.5/metabeaver/Testing/concatenateDataXLSX.py` & `metabeaver-0.1.6/metabeaver/Testing/concatenateDataXLSX.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.1.5/metabeaver.egg-info/SOURCES.txt` & `metabeaver-0.1.6/metabeaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metabeaver-0.1.5/setup.py` & `metabeaver-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.1.5', # Major, minor, patch
+    version='0.1.6', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
         'numpy',
         'pandas',
         'google-cloud-core',
         'google-cloud-bigquery',
     ],
```

