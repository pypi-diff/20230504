# Comparing `tmp/dbxconfig-5.0.3.tar.gz` & `tmp/dbxconfig-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-5.0.3.tar", last modified: Wed May  3 21:28:30 2023, max compression
+gzip compressed data, was "dbxconfig-5.0.4.tar", last modified: Wed May  3 23:22:50 2023, max compression
```

## Comparing `dbxconfig-5.0.3.tar` & `dbxconfig-5.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 21:28:30.171496 dbxconfig-5.0.3/
--rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 21:28:30.171496 dbxconfig-5.0.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4133 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 21:28:30.167497 dbxconfig-5.0.3/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      403 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3174 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4339 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6667 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/datallake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 21:28:30.167497 dbxconfig-5.0.3/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/dataset/_write.py
--rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/dataset/dataset_type.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 21:28:30.171496 dbxconfig-5.0.3/dbxconfig/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/dbxconfig/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 21:28:30.167497 dbxconfig-5.0.3/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 21:28:30.000000 dbxconfig-5.0.3/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      814 2023-05-03 21:28:30.000000 dbxconfig-5.0.3/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 21:28:30.000000 dbxconfig-5.0.3/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 21:28:30.000000 dbxconfig-5.0.3/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-03 21:28:30.000000 dbxconfig-5.0.3/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-03 21:28:30.000000 dbxconfig-5.0.3/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-03 21:28:30.171496 dbxconfig-5.0.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-03 21:27:37.000000 dbxconfig-5.0.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:22:50.425385 dbxconfig-5.0.4/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 23:22:50.425385 dbxconfig-5.0.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4133 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:22:50.417385 dbxconfig-5.0.4/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      403 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3174 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6667 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/datallake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:22:50.421385 dbxconfig-5.0.4/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/dataset/dataset_type.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:22:50.421385 dbxconfig-5.0.4/dbxconfig/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/dbxconfig/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-03 23:22:50.421385 dbxconfig-5.0.4/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4685 2023-05-03 23:22:50.000000 dbxconfig-5.0.4/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      814 2023-05-03 23:22:50.000000 dbxconfig-5.0.4/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 23:22:50.000000 dbxconfig-5.0.4/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-03 23:22:50.000000 dbxconfig-5.0.4/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-03 23:22:50.000000 dbxconfig-5.0.4/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-03 23:22:50.000000 dbxconfig-5.0.4/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-03 23:22:50.425385 dbxconfig-5.0.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-03 23:22:01.000000 dbxconfig-5.0.4/setup.py
```

### Comparing `dbxconfig-5.0.3/PKG-INFO` & `dbxconfig-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 5.0.3
+Version: 5.0.4
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-5.0.3/README.md` & `dbxconfig-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/_config.py` & `dbxconfig-5.0.4/dbxconfig/_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/_decorators.py` & `dbxconfig-5.0.4/dbxconfig/_decorators.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/_logging_config.py` & `dbxconfig-5.0.4/dbxconfig/_logging_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/_project.py` & `dbxconfig-5.0.4/dbxconfig/_project.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/_spark_context.py` & `dbxconfig-5.0.4/dbxconfig/_spark_context.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/_tables.py` & `dbxconfig-5.0.4/dbxconfig/_tables.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/_timeslice.py` & `dbxconfig-5.0.4/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/_utils.py` & `dbxconfig-5.0.4/dbxconfig/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import os
 import pkg_resources
 import logging
 
 
 YETL_CONFIG = "YETL_CONFIG"
 _ENCODING = "utf-8"
+_DBX_WORKSPACE_PATH = "/Workspace"
+_DBX_REPO_PATH = "/Workspace/Repos"
 
 
 class VersionNotFoundException(Exception):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
@@ -78,16 +80,26 @@
         path = os.path.join(root, path)
     _logger.debug(f"Absolute config path {path}")
     return path
 
 
 def get_config_path(project: str, path: str):
     _logger = logging.getLogger(__name__)
+
+    default_path = "."
+    if is_databricks():
+        if os.path.exists(_DBX_WORKSPACE_PATH):
+            default_path = f"{_DBX_WORKSPACE_PATH}"
+
+        if os.getcwd().startswith(_DBX_REPO_PATH):
+            repo_path = "/".join(os.getcwd().split("/")[0:5])
+            default_path = repo_path
+
     if not path:
-        path = os.getenv(YETL_CONFIG, "./config")
+        path = os.getenv(YETL_CONFIG, default_path)
     path = os.path.abspath(path)
     path = os.path.join(path, project)
     _logger.info(f"Absolute root config path {path}")
     return path
 
 
 def load_schema(path: str):
```

### Comparing `dbxconfig-5.0.3/dbxconfig/datallake.py` & `dbxconfig-5.0.4/dbxconfig/datallake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/dataset/_dataset.py` & `dbxconfig-5.0.4/dbxconfig/dataset/_dataset.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/dataset/_deltalake.py` & `dbxconfig-5.0.4/dbxconfig/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/dataset/_factory.py` & `dbxconfig-5.0.4/dbxconfig/dataset/_factory.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/dataset/_read.py` & `dbxconfig-5.0.4/dbxconfig/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig/workflow/_multi_threaded.py` & `dbxconfig-5.0.4/dbxconfig/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-5.0.4/dbxconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 5.0.3
+Version: 5.0.4
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-5.0.3/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-5.0.4/dbxconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbxconfig-5.0.3/setup.py` & `dbxconfig-5.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="5.0.3",
+    version="5.0.4",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

