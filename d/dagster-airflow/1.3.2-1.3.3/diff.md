# Comparing `tmp/dagster-airflow-1.3.2.tar.gz` & `tmp/dagster-airflow-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airflow-1.3.2.tar", last modified: Thu Apr 27 19:31:39 2023, max compression
+gzip compressed data, was "dagster-airflow-1.3.3.tar", last modified: Thu May  4 17:55:03 2023, max compression
```

## Comparing `dagster-airflow-1.3.2.tar` & `dagster-airflow-1.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:39.575825 dagster-airflow-1.3.2/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-27 19:31:39.579825 dagster-airflow-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:39.527825 dagster-airflow-1.3.2/dagster_airflow/
--rw-r--r--   0 root         (0) root         (0)     2474 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3759 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/airflow_dag_converter.py
--rw-r--r--   0 root         (0) root         (0)     7716 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/dagster_asset_factory.py
--rw-r--r--   0 root         (0) root         (0)     8158 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/dagster_factory.py
--rw-r--r--   0 root         (0) root         (0)     3896 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/dagster_job_factory.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/dagster_schedule_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:39.535825 dagster-airflow-1.3.2/dagster_airflow/hooks/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9161 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/hooks/dagster_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:39.543825 dagster-airflow-1.3.2/dagster_airflow/links/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)      851 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/links/dagster_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:39.547825 dagster-airflow-1.3.2/dagster_airflow/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/operators/dagster_operator.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/patch_airflow_example_dag.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:39.571825 dagster-airflow-1.3.2/dagster_airflow/resources/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3950 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/resources/airflow_db.py
--rw-r--r--   0 root         (0) root         (0)     3659 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/resources/airflow_ephemeral_db.py
--rw-r--r--   0 root         (0) root         (0)     4010 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/resources/airflow_persistent_db.py
--rw-r--r--   0 root         (0) root         (0)     4496 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/dagster_airflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:31:39.531825 dagster-airflow-1.3.2/dagster_airflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-04-27 19:31:39.000000 dagster-airflow-1.3.2/dagster_airflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-04-27 19:31:39.000000 dagster-airflow-1.3.2/dagster_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:31:39.000000 dagster-airflow-1.3.2/dagster_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      168 2023-04-27 19:31:39.000000 dagster-airflow-1.3.2/dagster_airflow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-27 19:31:39.000000 dagster-airflow-1.3.2/dagster_airflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-27 19:31:39.000000 dagster-airflow-1.3.2/dagster_airflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-04-27 19:31:39.583825 dagster-airflow-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2647 2023-04-27 18:30:35.000000 dagster-airflow-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:03.201619 dagster-airflow-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 17:55:03.201619 dagster-airflow-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:03.197619 dagster-airflow-1.3.3/dagster_airflow/
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/airflow_dag_converter.py
+-rw-r--r--   0 root         (0) root         (0)     7716 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/dagster_asset_factory.py
+-rw-r--r--   0 root         (0) root         (0)     8158 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/dagster_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3896 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/dagster_job_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/dagster_schedule_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:03.197619 dagster-airflow-1.3.3/dagster_airflow/hooks/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9138 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/hooks/dagster_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:03.197619 dagster-airflow-1.3.3/dagster_airflow/links/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      851 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/links/dagster_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:03.201619 dagster-airflow-1.3.3/dagster_airflow/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/operators/dagster_operator.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/patch_airflow_example_dag.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:03.201619 dagster-airflow-1.3.3/dagster_airflow/resources/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/resources/airflow_db.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/resources/airflow_ephemeral_db.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/resources/airflow_persistent_db.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/dagster_airflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:55:03.197619 dagster-airflow-1.3.3/dagster_airflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 17:55:03.000000 dagster-airflow-1.3.3/dagster_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-04 17:55:03.000000 dagster-airflow-1.3.3/dagster_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:55:03.000000 dagster-airflow-1.3.3/dagster_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-04 17:55:03.000000 dagster-airflow-1.3.3/dagster_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      469 2023-05-04 17:55:03.000000 dagster-airflow-1.3.3/dagster_airflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-04 17:55:03.000000 dagster-airflow-1.3.3/dagster_airflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-04 17:55:03.205619 dagster-airflow-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-05-04 17:42:14.000000 dagster-airflow-1.3.3/setup.py
```

### Comparing `dagster-airflow-1.3.2/LICENSE` & `dagster-airflow-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/PKG-INFO` & `dagster-airflow-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.3.2
+Version: 1.3.3
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dagster-airflow-1.3.2/dagster_airflow/__init__.py` & `dagster-airflow-1.3.3/dagster_airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/airflow_dag_converter.py` & `dagster-airflow-1.3.3/dagster_airflow/airflow_dag_converter.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/dagster_asset_factory.py` & `dagster-airflow-1.3.3/dagster_airflow/dagster_asset_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/dagster_factory.py` & `dagster-airflow-1.3.3/dagster_airflow/dagster_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/dagster_job_factory.py` & `dagster-airflow-1.3.3/dagster_airflow/dagster_job_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/dagster_schedule_factory.py` & `dagster-airflow-1.3.3/dagster_airflow/dagster_schedule_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/hooks/dagster_hook.py` & `dagster-airflow-1.3.3/dagster_airflow/hooks/dagster_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import time
 from typing import Any, Mapping, Optional, cast
 
 # Type errors ignored because some of these imports target deprecated modules for compatibility with
 # airflow 1.x and 2.x.
 import requests
 from airflow.exceptions import AirflowException
-from airflow.hooks.base_hook import BaseHook
+from airflow.hooks.base_hook import BaseHook  # type: ignore
 from airflow.models import Connection
-from dagster._core.storage.pipeline_run import DagsterRunStatus
+from dagster._core.storage.dagster_run import DagsterRunStatus
 
 from dagster_airflow.utils import is_airflow_2_loaded_in_environment
 
 
 class DagsterHook(BaseHook):
     conn_name_attr = "dagster_conn_id"
     default_conn_name = "dagster_default"
@@ -58,15 +58,15 @@
         deployment_name: Optional[str] = None,
         url: str = "",
         user_token: Optional[str] = None,
     ) -> None:
         if is_airflow_2_loaded_in_environment():
             super().__init__()
         else:
-            super().__init__(source=None)  # type: ignore  # (airflow 1 compat)
+            super().__init__(source=None)
         self.url = url
         self.user_token = user_token
         self.organization_id = organization_id
         self.deployment_name = deployment_name
         if (deployment_name or organization_id) and dagster_conn_id:
             raise AirflowException(
                 "Cannot set both dagster_conn_id and organization_id/deployment_name"
```

### Comparing `dagster-airflow-1.3.2/dagster_airflow/links/dagster_link.py` & `dagster-airflow-1.3.3/dagster_airflow/links/dagster_link.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/operators/dagster_operator.py` & `dagster-airflow-1.3.3/dagster_airflow/operators/dagster_operator.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/patch_airflow_example_dag.py` & `dagster-airflow-1.3.3/dagster_airflow/patch_airflow_example_dag.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/resources/airflow_db.py` & `dagster-airflow-1.3.3/dagster_airflow/resources/airflow_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,12 +89,12 @@
                     execution_date=execution_date,
                     run_type=DagRunType.MANUAL,
                     conf=self.dag_run_config,
                 )
             else:
                 dagrun = dag.create_dagrun(
                     run_id=f"dagster_airflow_run_{execution_date}",
-                    state=State.RUNNING,
+                    state=State.RUNNING,  # type: ignore
                     execution_date=execution_date,
                     conf=self.dag_run_config,
                 )
         return dagrun
```

### Comparing `dagster-airflow-1.3.2/dagster_airflow/resources/airflow_ephemeral_db.py` & `dagster-airflow-1.3.3/dagster_airflow/resources/airflow_ephemeral_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/resources/airflow_persistent_db.py` & `dagster-airflow-1.3.3/dagster_airflow/resources/airflow_persistent_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow/utils.py` & `dagster-airflow-1.3.3/dagster_airflow/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/dagster_airflow.egg-info/PKG-INFO` & `dagster-airflow-1.3.3/dagster_airflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.3.2
+Version: 1.3.3
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dagster-airflow-1.3.2/dagster_airflow.egg-info/SOURCES.txt` & `dagster-airflow-1.3.3/dagster_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.2/setup.py` & `dagster-airflow-1.3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airflow_tests*"]),
     install_requires=[
-        "dagster==1.3.2",
+        "dagster==1.3.3",
         "docker>=5.0.3,<6.0.0",
         "lazy_object_proxy",
         "pendulum",
     ],
     project_urls={
         # airflow will embed a link this in the providers page UI
         "project-url/documentation": "https://docs.dagster.io",
@@ -44,15 +44,15 @@
     extras_require={
         "kubernetes": ["kubernetes>=3.0.0", "cryptography>=2.0.0"],
         "test_airflow_2": [
             "apache-airflow>=2.0.0",
             "boto3>=1.26.7",
             "kubernetes>=10.0.1",
             "apache-airflow-providers-docker>=3.2.0,<4",
-            "apache-airflow-providers-apache-spark>=3.0.0,<4",
+            "apache-airflow-providers-apache-spark",
             # Logging messages are set to debug starting 4.1.1
             "apache-airflow-providers-http<4.1.1",
         ],
         "test_airflow_1": [
             "apache-airflow>=1.0.0,<2.0.0",
             "boto3>=1.26.7",
             "kubernetes>=10.0.1",
```

