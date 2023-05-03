# Comparing `tmp/apache-airflow-providers-aerofoil-1.0.0.tar.gz` & `tmp/apache-airflow-providers-aerofoil-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-aerofoil-1.0.0.tar", last modified: Fri Apr 28 06:47:43 2023, max compression
+gzip compressed data, was "apache-airflow-providers-aerofoil-1.0.1.tar", last modified: Wed May  3 23:33:32 2023, max compression
```

## Comparing `apache-airflow-providers-aerofoil-1.0.0.tar` & `apache-airflow-providers-aerofoil-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.859321 apache-airflow-providers-aerofoil-1.0.0/
--rw-r--r--   0 anurag     (501) staff       (20)     1106 2022-11-03 06:35:07.000000 apache-airflow-providers-aerofoil-1.0.0/LICENSE.md
--rw-r--r--   0 anurag     (501) staff       (20)       47 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/MANIFEST.in
--rw-r--r--   0 anurag     (501) staff       (20)     3264 2023-04-28 06:47:43.859163 apache-airflow-providers-aerofoil-1.0.0/PKG-INFO
--rw-r--r--   0 anurag     (501) staff       (20)     3029 2022-11-03 19:43:51.000000 apache-airflow-providers-aerofoil-1.0.0/README.md
--rw-r--r--   0 anurag     (501) staff       (20)       38 2023-04-28 06:47:43.859360 apache-airflow-providers-aerofoil-1.0.0/setup.cfg
--rw-r--r--   0 anurag     (501) staff       (20)      904 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/setup.py
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.853875 apache-airflow-providers-aerofoil-1.0.0/src/
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.855379 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/
--rw-r--r--   0 anurag     (501) staff       (20)      510 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/__init__.py
--rw-r--r--   0 anurag     (501) staff       (20)     2206 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/aerofoil_backfill.py
--rw-r--r--   0 anurag     (501) staff       (20)     1680 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/aerofoil_plugin.py
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.855698 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/models/
--rw-r--r--   0 anurag     (501) staff       (20)     1768 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/models/backfill.py
--rw-r--r--   0 anurag     (501) staff       (20)      671 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/models/reset_dag.py
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.855854 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/operators/
--rw-r--r--   0 anurag     (501) staff       (20)      458 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/operators/bash.py
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.856030 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/sensors/
--rw-r--r--   0 anurag     (501) staff       (20)      450 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/sensors/backfill_sensor.py
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.853655 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.857112 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/aerofoil/
--rw-r--r--   0 anurag     (501) staff       (20)     8963 2022-10-13 19:48:40.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/aerofoil/backfill.html
--rw-r--r--   0 anurag     (501) staff       (20)     6827 2022-10-13 20:41:02.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/aerofoil/fake_success.html
--rw-r--r--   0 anurag     (501) staff       (20)     5231 2022-10-13 23:24:15.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/aerofoil/reset.html
--rw-r--r--   0 anurag     (501) staff       (20)        0 2022-04-05 12:52:39.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/aerofoil/restart.html
--rw-r--r--   0 anurag     (501) staff       (20)        0 2022-04-05 12:52:39.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/aerofoil/version.html
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.857219 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/utils/
--rw-r--r--   0 anurag     (501) staff       (20)      556 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/utils/web_utils.py
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.858189 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/
--rw-r--r--   0 anurag     (501) staff       (20)     3459 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/backfill_view.py
--rw-r--r--   0 anurag     (501) staff       (20)      463 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/mydags_view.py
--rw-r--r--   0 anurag     (501) staff       (20)     2645 2022-10-13 23:25:33.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/reset_view.py
--rw-r--r--   0 anurag     (501) staff       (20)     2448 2022-11-09 22:49:40.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/restart_view.py
--rw-r--r--   0 anurag     (501) staff       (20)      969 2022-07-26 09:26:16.000000 apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/version_view.py
-drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-04-28 06:47:43.859011 apache-airflow-providers-aerofoil-1.0.0/src/apache_airflow_providers_aerofoil.egg-info/
--rw-r--r--   0 anurag     (501) staff       (20)     3264 2023-04-28 06:47:43.000000 apache-airflow-providers-aerofoil-1.0.0/src/apache_airflow_providers_aerofoil.egg-info/PKG-INFO
--rw-r--r--   0 anurag     (501) staff       (20)     1010 2023-04-28 06:47:43.000000 apache-airflow-providers-aerofoil-1.0.0/src/apache_airflow_providers_aerofoil.egg-info/SOURCES.txt
--rw-r--r--   0 anurag     (501) staff       (20)        1 2023-04-28 06:47:43.000000 apache-airflow-providers-aerofoil-1.0.0/src/apache_airflow_providers_aerofoil.egg-info/dependency_links.txt
--rw-r--r--   0 anurag     (501) staff       (20)      148 2023-04-28 06:47:43.000000 apache-airflow-providers-aerofoil-1.0.0/src/apache_airflow_providers_aerofoil.egg-info/entry_points.txt
--rw-r--r--   0 anurag     (501) staff       (20)        9 2023-04-28 06:47:43.000000 apache-airflow-providers-aerofoil-1.0.0/src/apache_airflow_providers_aerofoil.egg-info/top_level.txt
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.141685 apache-airflow-providers-aerofoil-1.0.1/
+-rw-r--r--   0 anurag     (501) staff       (20)     1106 2022-11-03 06:35:07.000000 apache-airflow-providers-aerofoil-1.0.1/LICENSE.md
+-rw-r--r--   0 anurag     (501) staff       (20)       47 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/MANIFEST.in
+-rw-r--r--   0 anurag     (501) staff       (20)     3252 2023-05-03 23:33:32.141521 apache-airflow-providers-aerofoil-1.0.1/PKG-INFO
+-rw-r--r--   0 anurag     (501) staff       (20)     3017 2023-05-03 23:13:06.000000 apache-airflow-providers-aerofoil-1.0.1/README.md
+-rw-r--r--   0 anurag     (501) staff       (20)       38 2023-05-03 23:33:32.141731 apache-airflow-providers-aerofoil-1.0.1/setup.cfg
+-rw-r--r--   0 anurag     (501) staff       (20)      938 2023-05-03 23:32:29.000000 apache-airflow-providers-aerofoil-1.0.1/setup.py
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.137760 apache-airflow-providers-aerofoil-1.0.1/src/
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.138671 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/
+-rw-r--r--   0 anurag     (501) staff       (20)      510 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/__init__.py
+-rw-r--r--   0 anurag     (501) staff       (20)     2206 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/aerofoil_backfill.py
+-rw-r--r--   0 anurag     (501) staff       (20)     1680 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/aerofoil_plugin.py
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.138908 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/models/
+-rw-r--r--   0 anurag     (501) staff       (20)     1768 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/models/backfill.py
+-rw-r--r--   0 anurag     (501) staff       (20)      671 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/models/reset_dag.py
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.139068 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/operators/
+-rw-r--r--   0 anurag     (501) staff       (20)      458 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/operators/bash.py
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.139224 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/sensors/
+-rw-r--r--   0 anurag     (501) staff       (20)      450 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/sensors/backfill_sensor.py
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.137465 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.139812 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/aerofoil/
+-rw-r--r--   0 anurag     (501) staff       (20)     8963 2022-10-13 19:48:40.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/aerofoil/backfill.html
+-rw-r--r--   0 anurag     (501) staff       (20)     6827 2022-10-13 20:41:02.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/aerofoil/fake_success.html
+-rw-r--r--   0 anurag     (501) staff       (20)     5231 2022-10-13 23:24:15.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/aerofoil/reset.html
+-rw-r--r--   0 anurag     (501) staff       (20)        0 2022-04-05 12:52:39.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/aerofoil/restart.html
+-rw-r--r--   0 anurag     (501) staff       (20)        0 2022-04-05 12:52:39.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/aerofoil/version.html
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.139913 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/utils/
+-rw-r--r--   0 anurag     (501) staff       (20)      556 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/utils/web_utils.py
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.140609 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/
+-rw-r--r--   0 anurag     (501) staff       (20)     3459 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/backfill_view.py
+-rw-r--r--   0 anurag     (501) staff       (20)      463 2022-11-10 00:28:11.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/mydags_view.py
+-rw-r--r--   0 anurag     (501) staff       (20)     2645 2022-10-13 23:25:33.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/reset_view.py
+-rw-r--r--   0 anurag     (501) staff       (20)     2448 2022-11-09 22:49:40.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/restart_view.py
+-rw-r--r--   0 anurag     (501) staff       (20)      969 2022-07-26 09:26:16.000000 apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/version_view.py
+drwxr-xr-x   0 anurag     (501) staff       (20)        0 2023-05-03 23:33:32.141337 apache-airflow-providers-aerofoil-1.0.1/src/apache_airflow_providers_aerofoil.egg-info/
+-rw-r--r--   0 anurag     (501) staff       (20)     3252 2023-05-03 23:33:32.000000 apache-airflow-providers-aerofoil-1.0.1/src/apache_airflow_providers_aerofoil.egg-info/PKG-INFO
+-rw-r--r--   0 anurag     (501) staff       (20)     1010 2023-05-03 23:33:32.000000 apache-airflow-providers-aerofoil-1.0.1/src/apache_airflow_providers_aerofoil.egg-info/SOURCES.txt
+-rw-r--r--   0 anurag     (501) staff       (20)        1 2023-05-03 23:33:32.000000 apache-airflow-providers-aerofoil-1.0.1/src/apache_airflow_providers_aerofoil.egg-info/dependency_links.txt
+-rw-r--r--   0 anurag     (501) staff       (20)      148 2023-05-03 23:33:32.000000 apache-airflow-providers-aerofoil-1.0.1/src/apache_airflow_providers_aerofoil.egg-info/entry_points.txt
+-rw-r--r--   0 anurag     (501) staff       (20)        9 2023-05-03 23:33:32.000000 apache-airflow-providers-aerofoil-1.0.1/src/apache_airflow_providers_aerofoil.egg-info/top_level.txt
```

### Comparing `apache-airflow-providers-aerofoil-1.0.0/LICENSE.md` & `apache-airflow-providers-aerofoil-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/PKG-INFO` & `apache-airflow-providers-aerofoil-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-aerofoil
-Version: 1.0.0
+Version: 1.0.1
 Summary: A convenient add-on for Apache Airflow
 Author: Anuradha Chowdhary
 Author-email: mail@achowdhary.com
 Requires-Python: ~=3.7
 License-File: LICENSE.md
 
 # Aerofoil : Lifting Airflow
@@ -27,15 +27,15 @@
 ## Installation 
 ### Pre-requisite
 - Working Airflow installation.
 - works with any executor other than Sequential Executor or LocalExecutor (e.g. KubernetasExecutor, CeleryExecutor)
 - Requires a non-sqlite database in the backend.
 
 ### Install Instructions:
-- Clone this repo (the plugin is not yet available in pypi)
+- pip install apache-airflow-providers-aerofoil
 - Add rquired tables to Airflow Metadata DB by executing src/aerofoil/models.sql
 - Deploy DAG file in the src/aerofoil/aerofoil_backfill.py DAGs to  your Airflow (usually by putting the DAG in  Airflow's DAGs folder.
 - Make sure the *__aerofoil_backfill__* 
 - DAG is enabled.
 
 ## Backfilll Design:
 When the user submits a backfill, it creates an entry in the `aerofoil_backfill` backfill table. *__aerofoil_backfill__*  DAG is scheduled to run every minute (which can be changed, by modifying the DAG). The Sesor in the DAG, picks up the entries in the DB and create dynamic task for each entry. The Backfill job itself runs as a Bash command in the executor. This provides a flexible and executor agnostic design.
```

### Comparing `apache-airflow-providers-aerofoil-1.0.0/README.md` & `apache-airflow-providers-aerofoil-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ## Installation 
 ### Pre-requisite
 - Working Airflow installation.
 - works with any executor other than Sequential Executor or LocalExecutor (e.g. KubernetasExecutor, CeleryExecutor)
 - Requires a non-sqlite database in the backend.
 
 ### Install Instructions:
-- Clone this repo (the plugin is not yet available in pypi)
+- pip install apache-airflow-providers-aerofoil
 - Add rquired tables to Airflow Metadata DB by executing src/aerofoil/models.sql
 - Deploy DAG file in the src/aerofoil/aerofoil_backfill.py DAGs to  your Airflow (usually by putting the DAG in  Airflow's DAGs folder.
 - Make sure the *__aerofoil_backfill__* 
 - DAG is enabled.
 
 ## Backfilll Design:
 When the user submits a backfill, it creates an entry in the `aerofoil_backfill` backfill table. *__aerofoil_backfill__*  DAG is scheduled to run every minute (which can be changed, by modifying the DAG). The Sesor in the DAG, picks up the entries in the DB and create dynamic task for each entry. The Backfill job itself runs as a Bash command in the executor. This provides a flexible and executor agnostic design.
```

### Comparing `apache-airflow-providers-aerofoil-1.0.0/setup.py` & `apache-airflow-providers-aerofoil-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='apache-airflow-providers-aerofoil',
-    version='1.0.0',
+    version='1.0.1',
     description='A convenient add-on for Apache Airflow',
     long_description=read('README.md'),
     author='Anuradha Chowdhary',
     author_email='mail@achowdhary.com',
+    include_package_data=True,
     entry_points={
         'apache_airflow_provider': [
             'provider_info=aerofoil.__init__:get_provider_info'
         ],
         'airflow.plugins': [
             'aerofoil=aerofoil.aerofoil_plugin:AerofoilPlugin'
         ]
@@ -27,11 +28,11 @@
         'aerofoil',
         'aerofoil.models',
         'aerofoil.utils',
         'aerofoil.sensors',
         'aerofoil.operators',
         'aerofoil.views'
     ],
-
+   
     python_requires='~=3.7',
     package_dir={'': 'src'},
 )
```

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/aerofoil_backfill.py` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/aerofoil_backfill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/aerofoil_plugin.py` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/aerofoil_plugin.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/models/backfill.py` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/models/backfill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/models/reset_dag.py` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/models/reset_dag.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/aerofoil/backfill.html` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/aerofoil/backfill.html`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/aerofoil/fake_success.html` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/aerofoil/fake_success.html`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/templates/aerofoil/reset.html` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/templates/aerofoil/reset.html`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/utils/web_utils.py` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/utils/web_utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/backfill_view.py` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/backfill_view.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/reset_view.py` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/reset_view.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/restart_view.py` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/restart_view.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/aerofoil/views/version_view.py` & `apache-airflow-providers-aerofoil-1.0.1/src/aerofoil/views/version_view.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/apache_airflow_providers_aerofoil.egg-info/PKG-INFO` & `apache-airflow-providers-aerofoil-1.0.1/src/apache_airflow_providers_aerofoil.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-aerofoil
-Version: 1.0.0
+Version: 1.0.1
 Summary: A convenient add-on for Apache Airflow
 Author: Anuradha Chowdhary
 Author-email: mail@achowdhary.com
 Requires-Python: ~=3.7
 License-File: LICENSE.md
 
 # Aerofoil : Lifting Airflow
@@ -27,15 +27,15 @@
 ## Installation 
 ### Pre-requisite
 - Working Airflow installation.
 - works with any executor other than Sequential Executor or LocalExecutor (e.g. KubernetasExecutor, CeleryExecutor)
 - Requires a non-sqlite database in the backend.
 
 ### Install Instructions:
-- Clone this repo (the plugin is not yet available in pypi)
+- pip install apache-airflow-providers-aerofoil
 - Add rquired tables to Airflow Metadata DB by executing src/aerofoil/models.sql
 - Deploy DAG file in the src/aerofoil/aerofoil_backfill.py DAGs to  your Airflow (usually by putting the DAG in  Airflow's DAGs folder.
 - Make sure the *__aerofoil_backfill__* 
 - DAG is enabled.
 
 ## Backfilll Design:
 When the user submits a backfill, it creates an entry in the `aerofoil_backfill` backfill table. *__aerofoil_backfill__*  DAG is scheduled to run every minute (which can be changed, by modifying the DAG). The Sesor in the DAG, picks up the entries in the DB and create dynamic task for each entry. The Backfill job itself runs as a Bash command in the executor. This provides a flexible and executor agnostic design.
```

### Comparing `apache-airflow-providers-aerofoil-1.0.0/src/apache_airflow_providers_aerofoil.egg-info/SOURCES.txt` & `apache-airflow-providers-aerofoil-1.0.1/src/apache_airflow_providers_aerofoil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

