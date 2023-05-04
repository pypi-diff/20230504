# Comparing `tmp/aib_logging-1.0.0.tar.gz` & `tmp/aib_logging-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aib_logging-1.0.0.tar", last modified: Tue May  2 09:29:02 2023, max compression
+gzip compressed data, was "aib_logging-1.0.1.tar", last modified: Thu May  4 06:19:54 2023, max compression
```

## Comparing `aib_logging-1.0.0.tar` & `aib_logging-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-02 09:29:02.563649 aib_logging-1.0.0/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.0/LICENSE.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-02 09:29:02.563649 aib_logging-1.0.0/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.0/README.md
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      623 2023-05-02 09:28:54.000000 aib_logging-1.0.0/pyproject.toml
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-02 09:29:02.564648 aib_logging-1.0.0/setup.cfg
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-02 09:29:02.558648 aib_logging-1.0.0/src/
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-02 09:29:02.560648 aib_logging-1.0.0/src/aib_logging/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.0/src/aib_logging/__init__.py
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    13057 2023-05-02 08:42:56.000000 aib_logging-1.0.0/src/aib_logging/logger.py
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-02 09:29:02.563649 aib_logging-1.0.0/src/aib_logging.egg-info/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/SOURCES.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/dependency_links.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       21 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/requires.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-02 09:29:02.000000 aib_logging-1.0.0/src/aib_logging.egg-info/top_level.txt
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-04 06:19:54.268240 aib_logging-1.0.1/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.1/LICENSE.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-04 06:19:54.268240 aib_logging-1.0.1/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.1/README.md
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      623 2023-05-04 06:17:30.000000 aib_logging-1.0.1/pyproject.toml
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-04 06:19:54.268240 aib_logging-1.0.1/setup.cfg
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-04 06:19:54.263240 aib_logging-1.0.1/src/
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-04 06:19:54.266240 aib_logging-1.0.1/src/aib_logging/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.1/src/aib_logging/__init__.py
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14191 2023-05-03 13:11:24.000000 aib_logging-1.0.1/src/aib_logging/logger.py
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-04 06:19:54.267240 aib_logging-1.0.1/src/aib_logging.egg-info/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-04 06:19:54.000000 aib_logging-1.0.1/src/aib_logging.egg-info/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-04 06:19:54.000000 aib_logging-1.0.1/src/aib_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-04 06:19:54.000000 aib_logging-1.0.1/src/aib_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       21 2023-05-04 06:19:54.000000 aib_logging-1.0.1/src/aib_logging.egg-info/requires.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-04 06:19:54.000000 aib_logging-1.0.1/src/aib_logging.egg-info/top_level.txt
```

### Comparing `aib_logging-1.0.0/LICENSE.txt` & `aib_logging-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aib_logging-1.0.0/PKG-INFO` & `aib_logging-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib_logging
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aib_logging-1.0.0/pyproject.toml` & `aib_logging-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aib_logging"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="akib Shaikh", email="shaikhakib.k@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aib_logging-1.0.0/src/aib_logging/logger.py` & `aib_logging-1.0.1/src/aib_logging/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,50 +17,70 @@
         OTHER="Other"
     
     class Severities(Enum):
         INFO="INFO"
         WARNING="WARNING"
         ERROR="ERROR"
 
-    def __init__(self, project:str, pipeline_name:str="", logger_name:str="aib_custom_logger"):
+    def __init__(
+        self, 
+        project:str, 
+        region:str,
+        pipeline_name:str="", 
+        logger_name:str="aib_custom_logger",
+        ):
         """
         This class use to add custom logs for vertex AI.
         class initialization with given project and pipeline name.
 
         ...
         Methods:
+        log(): to log basic info of pipeline/component status
         score_logs(): to log model performance score in custom logs.
         data_stat_log(): to log data statistic in custom logs.
         model_log(): to log model information in logs.
         ...
 
         Args:
             project(str): project id where your vertex AI pipeline running
+            region(str): Region of pipeline
             pipeline_name(str): name of pipeline
             logger_name(str): name of custom logger 
                 (default is aib_custom_logger)
         Returns:
             None
         """
         import logging
         import google.cloud.logging
         self.project=project
+        self.region=region
         self.pipeline_name=pipeline_name
         client = google.cloud.logging.Client(project=project)
         self.logger = client.logger(name=logger_name)
 
     def log(
         self,
         msg:str,
-        status:str='Running',
+        status:str='',
         severity:Severities=Severities.INFO,
-    ):
+        ):
+        """
+        Log basic information of pipeline and component.
+        Args:
+            msg(str): message to add in logs
+            status(str): status of component
+                default is empty string
+            severity(str): default is INFO
+        Returns:
+            None
+        """
         import inspect
         payload={
             "pipeline_run_name":self.pipeline_name,
+            "region":self.region,
             "project":self.project,
             "component_name": inspect.stack()[1].function,
             "Status":status,
             "message":msg,
         }
         self.logger.log_struct(payload, severity=severity.value)
 
@@ -178,14 +198,15 @@
         import inspect
         
         if model_type == 'classification':
             payload={
                 "pipeline_run_name":self.pipeline_name,
                 "component_name": inspect.stack()[1].function,
                 "project":self.project,
+                "region":self.region,
                 "category":category.value,
                 "action":action.value,
                 "model_name":model_name,
                 "model_version":model_version,
                 "data_subset":data_subset,
                 "model_type":model_type,
                 "accuracy_score":accuracy_score,
@@ -213,14 +234,15 @@
                 payload[key]=value
         
         if model_type == 'regression':
             payload={
                 "pipeline_run_name":self.pipeline_name,
                 "component_name": inspect.stack()[1].function,
                 "project":self.project,
+                "region":self.region,
                 "category":category.value,
                 "action":action.value,
                 "model_name":model_name,
                 "model_version":model_version,
                 "data_subset":data_subset,
                 "model_type":model_type,
                 "r2_score":r2_score,
@@ -238,14 +260,15 @@
                 payload[key]=value
         
         if model_type == 'clustering':
             payload={
                 "pipeline_run_name":self.pipeline_name,
                 "component_name": inspect.stack()[1].function,
                 "project":self.project,
+                "region":self.region,
                 "category":category.value,
                 "action":action.value,
                 "model_name":model_name,
                 "model_version":model_version,
                 "data_subset":data_subset,
                 "model_type":model_type,
                 "accuracy_score":accuracy_score,
@@ -270,14 +293,17 @@
         max_val:dict={},
         mean_val:dict={},
         std_val:dict={},
         count_val:dict={},
         percentile_25:dict={},
         percentile_50:dict={},
         percentile_75:dict={},
+        unique:dict={},
+        top:dict={},
+        freq:dict={},
         extra_labels:list=[],
         object:dict={},
         **kwargs
         ):
         """
         Method to log data statistic into logs
 
@@ -312,33 +338,43 @@
                 default is empty dict {},
             percentile_25(dict): 25% value of dataset column in key,value pair
                 default is empty dict {},
             percentile_50(dict): 50% value of dataset column in key,value pair
                 default is empty dict {},
             percentile_75(dict): 75% value of dataset column in key,value pair
                 default is empty dict {},
+            unique(dict): unique values for categorical column
+                default is empty dict {},
+            top(dict): top value for categorical column
+                default is empty dict {},
+            freq(dict): frequency of value in categorical column
+                default is empty dict {},
             extra_labels:list=[],
             object:dict={},
             **kwargs
         """
         import inspect
         payload={
             "pipeline_run_name":self.pipeline_name,
             "component_name": inspect.stack()[1].function,
             "project":self.project,
+            "region":self.region,
             "category":category.value,
             "action":action.value,
             "min":min_val,
             "max":max_val,
             "count":count_val,
             "mean":mean_val,
             "std":std_val,
             "percentile_25":percentile_25,
             "percentile_50":percentile_50,
             "percentile_75":percentile_75,
+            "unique":unique,
+            "top":top,
+            "freq":freq,
             "extra_labels":extra_labels,
             "message":msg,
             "object":object
         }
         for key, value in kwargs.items():
                 payload[key]=value
         # Send the Log request
```

### Comparing `aib_logging-1.0.0/src/aib_logging.egg-info/PKG-INFO` & `aib_logging-1.0.1/src/aib_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib-logging
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

