# Comparing `tmp/dbxconfig-5.0.6.tar.gz` & `tmp/dbxconfig-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-5.0.6.tar", last modified: Wed May  3 23:39:00 2023, max compression
+gzip compressed data, was "dbxconfig-5.0.7.tar", last modified: Thu May  4 11:05:19 2023, max compression
```

## Comparing `dbxconfig-5.0.6.tar` & `dbxconfig-5.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:39:00.659147 dbxconfig-5.0.6/
--rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 23:39:00.659147 dbxconfig-5.0.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4133 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:39:00.655146 dbxconfig-5.0.6/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      403 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3148 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1588 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6667 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/datallake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:39:00.659147 dbxconfig-5.0.6/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/dataset/_write.py
--rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/dataset/dataset_type.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:39:00.659147 dbxconfig-5.0.6/dbxconfig/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/dbxconfig/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:39:00.659147 dbxconfig-5.0.6/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 23:39:00.000000 dbxconfig-5.0.6/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      814 2023-05-03 23:39:00.000000 dbxconfig-5.0.6/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 23:39:00.000000 dbxconfig-5.0.6/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 23:39:00.000000 dbxconfig-5.0.6/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-03 23:39:00.000000 dbxconfig-5.0.6/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-03 23:39:00.000000 dbxconfig-5.0.6/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-03 23:39:00.659147 dbxconfig-5.0.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-03 23:38:07.000000 dbxconfig-5.0.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 11:05:19.989234 dbxconfig-5.0.7/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-04 11:05:19.989234 dbxconfig-5.0.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4133 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 11:05:19.985234 dbxconfig-5.0.7/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      454 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3148 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6667 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/datallake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 11:05:19.989234 dbxconfig-5.0.7/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/dataset/dataset_type.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 11:05:19.989234 dbxconfig-5.0.7/dbxconfig/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/dbxconfig/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 11:05:19.985234 dbxconfig-5.0.7/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-04 11:05:19.000000 dbxconfig-5.0.7/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      814 2023-05-04 11:05:19.000000 dbxconfig-5.0.7/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-04 11:05:19.000000 dbxconfig-5.0.7/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-04 11:05:19.000000 dbxconfig-5.0.7/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-04 11:05:19.000000 dbxconfig-5.0.7/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-04 11:05:19.000000 dbxconfig-5.0.7/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-04 11:05:19.989234 dbxconfig-5.0.7/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-04 11:04:22.000000 dbxconfig-5.0.7/setup.py
```

### Comparing `dbxconfig-5.0.6/PKG-INFO` & `dbxconfig-5.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 5.0.6
+Version: 5.0.7
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-5.0.6/README.md` & `dbxconfig-5.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/_config.py` & `dbxconfig-5.0.7/dbxconfig/_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/_decorators.py` & `dbxconfig-5.0.7/dbxconfig/_decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # implicit, not referenced - must be the 1st import
 from ._logging_config import configure_logging
 import logging
 from ._config import Config
 from ._timeslice import Timeslice
 from ._stage_type import StageType
+from .dataset import DataSet
 
 
 def yetl_flow(
     stage: StageType,
     project: str,
     pipeline: str = None,
     config_path: str = None,
@@ -35,14 +36,23 @@
 
             config = Config(
                 project=project, pipeline=_pipeline, config_path=config_path
             )
             table_mapping = config.get_table_mapping(
                 timeslice=timeslice, stage=stage, table=table
             )
+
+            destination: DataSet = table_mapping.destination
+            sources = table_mapping.source
+            if isinstance(sources, dict):
+                for _, source in sources.items():
+                    config.set_checkpoint(source=source, destination=destination)
+            else:
+                config.set_checkpoint(source=sources, destination=destination)
+
             _logger.info(f"Calling function {function.__name__}")
             ret = function(
                 *args,
                 table_mapping=table_mapping,
                 **kwargs,
             )
             return ret
```

### Comparing `dbxconfig-5.0.6/dbxconfig/_logging_config.py` & `dbxconfig-5.0.7/dbxconfig/_logging_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/_project.py` & `dbxconfig-5.0.7/dbxconfig/_project.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/_spark_context.py` & `dbxconfig-5.0.7/dbxconfig/_spark_context.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/_tables.py` & `dbxconfig-5.0.7/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/_timeslice.py` & `dbxconfig-5.0.7/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/_utils.py` & `dbxconfig-5.0.7/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/datallake.py` & `dbxconfig-5.0.7/dbxconfig/datallake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/dataset/_dataset.py` & `dbxconfig-5.0.7/dbxconfig/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/dataset/_deltalake.py` & `dbxconfig-5.0.7/dbxconfig/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/dataset/_factory.py` & `dbxconfig-5.0.7/dbxconfig/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/dataset/_read.py` & `dbxconfig-5.0.7/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig/workflow/_multi_threaded.py` & `dbxconfig-5.0.7/dbxconfig/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-5.0.7/dbxconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 5.0.6
+Version: 5.0.7
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-5.0.6/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-5.0.7/dbxconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.6/setup.py` & `dbxconfig-5.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="5.0.6",
+    version="5.0.7",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

