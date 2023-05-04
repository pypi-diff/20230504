# Comparing `tmp/gridstatusio-0.1.0.tar.gz` & `tmp/gridstatusio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-_jecbuii/gridstatusio-0.1.0.tar", last modified: Sat Mar 11 23:38:26 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-ooox1f17/gridstatusio-0.2.0.tar", last modified: Thu May  4 19:55:00 2023, max compression
```

## Comparing `gridstatusio-0.1.0.tar` & `gridstatusio-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-03-11 23:38:12.000000 gridstatusio-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3335 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2023-03-11 23:38:12.000000 gridstatusio-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/gridstatusio/
--rw-r--r--   0 root         (0) root         (0)       77 2023-03-11 23:38:12.000000 gridstatusio-0.1.0/gridstatusio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-03-11 23:38:12.000000 gridstatusio-0.1.0/gridstatusio/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/gridstatusio/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 23:38:12.000000 gridstatusio-0.1.0/gridstatusio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-03-11 23:38:12.000000 gridstatusio-0.1.0/gridstatusio/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-11 23:38:12.000000 gridstatusio-0.1.0/gridstatusio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/gridstatusio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3335 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/gridstatusio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      342 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/gridstatusio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/gridstatusio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      177 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/gridstatusio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/gridstatusio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2220 2023-03-11 23:38:12.000000 gridstatusio-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-11 23:38:26.000000 gridstatusio-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      848 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8289 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/gs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/gridstatusio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/gridstatusio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-05-04 19:54:46.000000 gridstatusio-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 19:55:00.000000 gridstatusio-0.2.0/setup.cfg
```

### Comparing `gridstatusio-0.1.0/LICENSE` & `gridstatusio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.1.0/PKG-INFO` & `gridstatusio-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
@@ -30,62 +30,28 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # GridStatus.io Hosted API
 
-Python client for accessing the [GridStatusIO API](https://www.gridstatus.io/api).
+Python client for accessing the [GridStatus.io Hosted API](https://www.gridstatus.io/api).
 
 ## Installation
 
-Install the library using pip:
+You can install GridStatus.io Hosted API by running the following command in your terminal or command prompt:
 
 ```bash
 pip install gridstatusio
 ```
 
+## Getting Started
 
-## Usage
+Check out this example notebook: [Getting Started](/Examples/Getting%20Started.ipynb)
 
-### Set API Key
-To use the library, first set your API key:
+## Open Source
 
-```python
-import gridstatusio as gs
-
-gs.api_key  = '<YOUR-API-KEY>'
-```
-
-if you don't have an API, request one [here](https://www.gridstatus.io/api). 
-
-### List available datasets
-
-```python
-gs.list_datasets()
-```
-
-### Get specific date
-
-Request a dataset at a specific date
-
-```python
-gs.get_dataset(
-    dataset="isone/fuel_mix_clean",
-    date="2023-01-01",
-)
-```
-
-### Get data range
-
-```python
-df = gs.get_dataset(
-    dataset="isone/fuel_mix_clean",
-    start="2023-01-01",
-    end="2023-01-05",
-    verbose=True,
-)
-```
+If you prefer to use an open source library that fetches data directly from the source, you can check out the [github repo](https://github.com/kmax12/gridstatus). For more information on Hosted API vs Open Source API, please see this [guide](https://api.gridstatus.io/docs#section/Getting-Started/Open-Source)
 
 ## Get Help
 
 We'd love to answer any usage or data access questions! Please let us know by emailing us at contact@gridstatus.io
```

### Comparing `gridstatusio-0.1.0/gridstatusio.egg-info/PKG-INFO` & `gridstatusio-0.2.0/gridstatusio.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
@@ -30,62 +30,28 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # GridStatus.io Hosted API
 
-Python client for accessing the [GridStatusIO API](https://www.gridstatus.io/api).
+Python client for accessing the [GridStatus.io Hosted API](https://www.gridstatus.io/api).
 
 ## Installation
 
-Install the library using pip:
+You can install GridStatus.io Hosted API by running the following command in your terminal or command prompt:
 
 ```bash
 pip install gridstatusio
 ```
 
+## Getting Started
 
-## Usage
+Check out this example notebook: [Getting Started](/Examples/Getting%20Started.ipynb)
 
-### Set API Key
-To use the library, first set your API key:
+## Open Source
 
-```python
-import gridstatusio as gs
-
-gs.api_key  = '<YOUR-API-KEY>'
-```
-
-if you don't have an API, request one [here](https://www.gridstatus.io/api). 
-
-### List available datasets
-
-```python
-gs.list_datasets()
-```
-
-### Get specific date
-
-Request a dataset at a specific date
-
-```python
-gs.get_dataset(
-    dataset="isone/fuel_mix_clean",
-    date="2023-01-01",
-)
-```
-
-### Get data range
-
-```python
-df = gs.get_dataset(
-    dataset="isone/fuel_mix_clean",
-    start="2023-01-01",
-    end="2023-01-05",
-    verbose=True,
-)
-```
+If you prefer to use an open source library that fetches data directly from the source, you can check out the [github repo](https://github.com/kmax12/gridstatus). For more information on Hosted API vs Open Source API, please see this [guide](https://api.gridstatus.io/docs#section/Getting-Started/Open-Source)
 
 ## Get Help
 
 We'd love to answer any usage or data access questions! Please let us know by emailing us at contact@gridstatus.io
```

### Comparing `gridstatusio-0.1.0/pyproject.toml` & `gridstatusio-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 keywords = ["energy", "independent system operator"]
 license = {file = "LICENSE"}
 requires-python = ">=3.7,<4"
 dependencies = [
     "requests >= 2.28.1",
     "pandas >= 1.3.0",
     "tqdm >= 4.64.1",
+    "termcolor >= 1.1.0",
+    "gridstatus >= 0.20.0",
 ]
 
 [project.urls]
 "Source Code"= "https://github.com/kmax12/gridstatusio/"
 "Issue Tracker" = "https://github.com/kmax12/gridstatusio/issues"
 
 [project.optional-dependencies]
@@ -37,14 +39,17 @@
     "pytest-xdist == 3.0.2",
     "pytest-rerunfailures == 10.3",
 ]
 dev = [
     "ruff == 0.0.202",
     "black[jupyter] == 22.12.0",
     "pre-commit == 2.21.0",
+    "plotly",
+    "kaleido",
+    "nbformat",
 ]
 
 
 [tool.setuptools]
 include-package-data = true
 license-files = ["LICENSE"]
```

