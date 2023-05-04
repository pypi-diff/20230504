# Comparing `tmp/feltlabs-0.5.1.tar.gz` & `tmp/feltlabs-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feltlabs-0.5.1.tar", last modified: Fri Dec 23 22:27:02 2022, max compression
+gzip compressed data, was "feltlabs-0.5.2.tar", last modified: Thu May  4 15:58:46 2023, max compression
```

## Comparing `feltlabs-0.5.1.tar` & `feltlabs-0.5.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 22:27:02.368719 feltlabs-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-23 22:26:05.000000 feltlabs-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2022-12-23 22:27:02.364719 feltlabs-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2022-12-23 22:26:05.000000 feltlabs-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 22:27:02.364719 feltlabs-0.5.1/feltlabs/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 22:27:02.364719 feltlabs-0.5.1/feltlabs/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/algorithm/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/algorithm/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 22:27:02.364719 feltlabs-0.5.1/feltlabs/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/json_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 22:27:02.364719 feltlabs-0.5.1/feltlabs/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/models/analytics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/models/sklearn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 22:27:02.364719 feltlabs-0.5.1/feltlabs/core/models/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/models/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/models/tensorflow/cnn_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/models/tensorflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/randomness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-23 22:26:05.000000 feltlabs-0.5.1/feltlabs/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 22:27:02.364719 feltlabs-0.5.1/feltlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2022-12-23 22:27:02.000000 feltlabs-0.5.1/feltlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2022-12-23 22:27:02.000000 feltlabs-0.5.1/feltlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 22:27:02.000000 feltlabs-0.5.1/feltlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-23 22:27:02.000000 feltlabs-0.5.1/feltlabs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 22:27:02.000000 feltlabs-0.5.1/feltlabs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-23 22:27:02.000000 feltlabs-0.5.1/feltlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-23 22:27:02.000000 feltlabs-0.5.1/feltlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2022-12-23 22:26:05.000000 feltlabs-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 22:27:02.368719 feltlabs-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2022-12-23 22:26:05.000000 feltlabs-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 22:27:02.364719 feltlabs-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/test_aggregation_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/test_aggregation_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/test_cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/test_data_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/test_import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/test_json_with_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/test_multi_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/test_solo_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2022-12-23 22:26:05.000000 feltlabs-0.5.1/tests/test_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:58:46.022770 feltlabs-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 15:57:40.000000 feltlabs-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-04 15:58:46.022770 feltlabs-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-04 15:57:40.000000 feltlabs-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:58:46.014770 feltlabs-0.5.2/feltlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:58:46.018770 feltlabs-0.5.2/feltlabs/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/algorithm/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/algorithm/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:58:46.018770 feltlabs-0.5.2/feltlabs/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/json_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:58:46.018770 feltlabs-0.5.2/feltlabs/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/models/analytics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/models/sklearn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:58:46.018770 feltlabs-0.5.2/feltlabs/core/models/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/models/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/models/tensorflow/cnn_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/models/tensorflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/randomness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-04 15:57:40.000000 feltlabs-0.5.2/feltlabs/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:58:46.018770 feltlabs-0.5.2/feltlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-04 15:58:45.000000 feltlabs-0.5.2/feltlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-04 15:58:45.000000 feltlabs-0.5.2/feltlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:58:45.000000 feltlabs-0.5.2/feltlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-04 15:58:45.000000 feltlabs-0.5.2/feltlabs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:58:45.000000 feltlabs-0.5.2/feltlabs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-04 15:58:45.000000 feltlabs-0.5.2/feltlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 15:58:45.000000 feltlabs-0.5.2/feltlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-04 15:57:40.000000 feltlabs-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:58:46.022770 feltlabs-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-04 15:57:40.000000 feltlabs-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:58:46.022770 feltlabs-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/test_aggregation_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/test_aggregation_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/test_cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/test_data_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/test_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/test_json_with_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/test_multi_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/test_solo_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-04 15:57:40.000000 feltlabs-0.5.2/tests/test_training.py
```

### Comparing `feltlabs-0.5.1/LICENSE` & `feltlabs-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/PKG-INFO` & `feltlabs-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feltlabs
-Version: 0.5.1
+Version: 0.5.2
 Summary: FELT python package intended for running federated learning on Ocean protocol.
 Home-page: https://feltlabs.ai/
 Author: FELT Labs
 Maintainer: FELT Labs
 Maintainer-email: info@bretahajek.com
 License: GPL-3.0 License
 Project-URL: Bug Tracker, https://github.com/FELT-Labs/feltlabs.py/issues
```

### Comparing `feltlabs-0.5.1/README.md` & `feltlabs-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/algorithm/aggregate.py` & `feltlabs-0.5.2/feltlabs/algorithm/aggregate.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/algorithm/train.py` & `feltlabs-0.5.2/feltlabs/algorithm/train.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/config.py` & `feltlabs-0.5.2/feltlabs/config.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/cryptography.py` & `feltlabs-0.5.2/feltlabs/core/cryptography.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/data.py` & `feltlabs-0.5.2/feltlabs/core/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,15 +70,20 @@
     """
     data_array = []
     if config.download_models:
         with config.custom_data_path.open("r") as f:
             conf = json.load(f)
 
         for url in conf["model_urls"]:
-            res = requests.get(url)
+            if isinstance(url, dict):
+                res = requests.get(**url)
+            elif isinstance(url, str):
+                res = requests.get(url)
+            else:
+                raise Exception(f"Invalid model URL (type {type(url)}): {url}")
             data_array.append(res.content)
 
     else:
         # Models passed as dataset
         for dataset in get_datasets(config).values():
             for file_path, _ in dataset.files:
                 with open(file_path, "rb") as f:
```

### Comparing `feltlabs-0.5.1/feltlabs/core/json_handler.py` & `feltlabs-0.5.2/feltlabs/core/json_handler.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/models/analytics_model.py` & `feltlabs-0.5.2/feltlabs/core/models/analytics_model.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/models/base_model.py` & `feltlabs-0.5.2/feltlabs/core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/models/sklearn_model.py` & `feltlabs-0.5.2/feltlabs/core/models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/models/tensorflow/cnn_network.py` & `feltlabs-0.5.2/feltlabs/core/models/tensorflow/cnn_network.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/models/tensorflow_model.py` & `feltlabs-0.5.2/feltlabs/core/models/tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/ocean.py` & `feltlabs-0.5.2/feltlabs/core/ocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     Returns:
         dictionary mapping dataset DID to dataset loading config
     """
     did_folders = [(p, p.name) for p in config.input_folder.iterdir() if p.is_dir()]
 
     datasets = {}
     for folder, did in did_folders:
-        datasets = {did: DatasetConfig()}
+        datasets[did] = DatasetConfig()
 
         for path in folder.glob("**/*"):
             if path.is_file() and _is_dataset_config(path):
                 datasets[did].parse_config(path)
             elif path.is_file():
                 datasets[did].add_file(path)
```

### Comparing `feltlabs-0.5.1/feltlabs/core/prompts.py` & `feltlabs-0.5.2/feltlabs/core/prompts.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/randomness.py` & `feltlabs-0.5.2/feltlabs/core/randomness.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/core/storage.py` & `feltlabs-0.5.2/feltlabs/core/storage.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs/model.py` & `feltlabs-0.5.2/feltlabs/model.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/feltlabs.egg-info/PKG-INFO` & `feltlabs-0.5.2/feltlabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feltlabs
-Version: 0.5.1
+Version: 0.5.2
 Summary: FELT python package intended for running federated learning on Ocean protocol.
 Home-page: https://feltlabs.ai/
 Author: FELT Labs
 Maintainer: FELT Labs
 Maintainer-email: info@bretahajek.com
 License: GPL-3.0 License
 Project-URL: Bug Tracker, https://github.com/FELT-Labs/feltlabs.py/issues
```

### Comparing `feltlabs-0.5.1/feltlabs.egg-info/SOURCES.txt` & `feltlabs-0.5.2/feltlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/pyproject.toml` & `feltlabs-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/setup.py` & `feltlabs-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 
 requirements = parse_requirements(PATH / "requirements.txt")
 
 
 setup(
     name="feltlabs",
-    version="0.5.1",
+    version="0.5.2",
     packages=find_packages(),
     maintainer="FELT Labs",
     maintainer_email="info@bretahajek.com",
     description=DOCLINES[0],
     long_description="\n".join(DOCLINES[2:]),
     long_description_content_type="text/markdown",
     keywords=["Federated Learning", "Web3", "Machine Learning"],
```

### Comparing `feltlabs-0.5.1/tests/test_aggregation_analytics.py` & `feltlabs-0.5.2/tests/test_aggregation_analytics.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/tests/test_aggregation_sklearn.py` & `feltlabs-0.5.2/tests/test_aggregation_sklearn.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/tests/test_cryptography.py` & `feltlabs-0.5.2/tests/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/tests/test_data_load.py` & `feltlabs-0.5.2/tests/test_data_load.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/tests/test_import_export.py` & `feltlabs-0.5.2/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/tests/test_json_with_numpy.py` & `feltlabs-0.5.2/tests/test_json_with_numpy.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/tests/test_multi_analytics.py` & `feltlabs-0.5.2/tests/test_multi_analytics.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/tests/test_solo_training.py` & `feltlabs-0.5.2/tests/test_solo_training.py`

 * *Files identical despite different names*

### Comparing `feltlabs-0.5.1/tests/test_training.py` & `feltlabs-0.5.2/tests/test_training.py`

 * *Files identical despite different names*

