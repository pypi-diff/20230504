# Comparing `tmp/simplepytorch-1.2.0.tar.gz` & `tmp/simplepytorch-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplepytorch-1.2.0.tar", last modified: Wed Mar  8 17:23:00 2023, max compression
+gzip compressed data, was "simplepytorch-1.3.0.tar", last modified: Thu May  4 15:20:22 2023, max compression
```

## Comparing `simplepytorch-1.2.0.tar` & `simplepytorch-1.3.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-03-08 17:23:00.753252 simplepytorch-1.2.0/
--rw-r--r--   0 alex      (1000) alex      (1000)     1068 2020-02-19 20:04:28.000000 simplepytorch-1.2.0/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     3298 2023-03-08 17:23:00.753252 simplepytorch-1.2.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     2847 2022-04-26 04:35:00.000000 simplepytorch-1.2.0/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-03-08 17:23:00.746585 simplepytorch-1.2.0/bin/
--rwxr-xr-x   0 alex      (1000) alex      (1000)       48 2021-01-20 01:32:25.000000 simplepytorch-1.2.0/bin/simplepytorch
--rwxr-xr-x   0 alex      (1000) alex      (1000)       90 2021-01-20 01:32:25.000000 simplepytorch-1.2.0/bin/simplepytorch_debug
--rwxr-xr-x   0 alex      (1000) alex      (1000)       80 2021-01-21 15:57:18.000000 simplepytorch-1.2.0/bin/simplepytorch_plot
--rw-r--r--   0 alex      (1000) alex      (1000)      248 2023-03-08 17:23:00.753252 simplepytorch-1.2.0/setup.cfg
--rwxr-xr-x   0 alex      (1000) alex      (1000)     1160 2023-03-08 17:22:59.000000 simplepytorch-1.2.0/setup.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-03-08 17:23:00.749919 simplepytorch-1.2.0/simplepytorch/
--rw-r--r--   0 alex      (1000) alex      (1000)       22 2023-03-08 17:22:59.000000 simplepytorch-1.2.0/simplepytorch/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)       70 2020-06-07 00:23:22.000000 simplepytorch-1.2.0/simplepytorch/__main__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1204 2022-04-25 14:00:07.000000 simplepytorch-1.2.0/simplepytorch/api.py
--rw-r--r--   0 alex      (1000) alex      (1000)      893 2020-02-19 20:04:28.000000 simplepytorch-1.2.0/simplepytorch/cache.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10311 2022-04-25 13:58:29.000000 simplepytorch-1.2.0/simplepytorch/cmdline.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-03-08 17:23:00.753252 simplepytorch-1.2.0/simplepytorch/datasets/
--rw-r--r--   0 alex      (1000) alex      (1000)     6406 2021-06-13 22:51:00.000000 simplepytorch-1.2.0/simplepytorch/datasets/BBBC038v1_microscopy.py
--rw-r--r--   0 alex      (1000) alex      (1000)      680 2023-03-08 17:21:22.000000 simplepytorch-1.2.0/simplepytorch/datasets/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1772 2020-02-19 20:04:28.000000 simplepytorch-1.2.0/simplepytorch/datasets/_shared.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10986 2022-11-26 10:17:09.000000 simplepytorch-1.2.0/simplepytorch/datasets/chexpert.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5543 2020-09-08 08:18:00.000000 simplepytorch-1.2.0/simplepytorch/datasets/drive.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2255 2021-09-22 22:34:28.000000 simplepytorch-1.2.0/simplepytorch/datasets/eyepacs.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1112 2021-09-22 22:34:44.000000 simplepytorch-1.2.0/simplepytorch/datasets/glob_image_dir.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3778 2020-02-19 20:04:28.000000 simplepytorch-1.2.0/simplepytorch/datasets/idrid.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16323 2022-05-16 13:41:31.000000 simplepytorch-1.2.0/simplepytorch/datasets/intel_mobileodt_cervical.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1623 2022-05-31 17:45:19.000000 simplepytorch-1.2.0/simplepytorch/datasets/kimeye.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4024 2020-02-19 20:04:28.000000 simplepytorch-1.2.0/simplepytorch/datasets/messidor.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1385 2020-02-19 20:04:28.000000 simplepytorch-1.2.0/simplepytorch/datasets/pickled_dicts.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1314 2022-04-13 00:39:21.000000 simplepytorch-1.2.0/simplepytorch/datasets/preprocess.py
--rw-r--r--   0 alex      (1000) alex      (1000)     9228 2022-04-25 16:29:13.000000 simplepytorch-1.2.0/simplepytorch/datasets/qualdr.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3277 2020-02-19 20:04:28.000000 simplepytorch-1.2.0/simplepytorch/datasets/rite.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1300 2020-02-19 20:04:28.000000 simplepytorch-1.2.0/simplepytorch/datasets/train_val_test_split.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1681 2020-02-19 20:04:28.000000 simplepytorch-1.2.0/simplepytorch/early_stopping.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16202 2022-04-25 13:56:13.000000 simplepytorch-1.2.0/simplepytorch/feedforward.py
--rw-r--r--   0 alex      (1000) alex      (1000)    17470 2022-04-25 23:56:47.000000 simplepytorch-1.2.0/simplepytorch/logging_tools.py
--rw-r--r--   0 alex      (1000) alex      (1000)    14296 2022-11-22 16:26:29.000000 simplepytorch-1.2.0/simplepytorch/metrics.py
--rwxr-xr-x   0 alex      (1000) alex      (1000)    21766 2023-02-07 12:06:45.000000 simplepytorch-1.2.0/simplepytorch/plot_perf.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6102 2022-05-01 10:43:51.000000 simplepytorch-1.2.0/simplepytorch/raytunelib.py
--rw-r--r--   0 alex      (1000) alex      (1000)    21206 2022-11-30 12:34:54.000000 simplepytorch-1.2.0/simplepytorch/result.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16501 2022-11-24 23:35:20.000000 simplepytorch-1.2.0/simplepytorch/trainlib.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-03-08 17:23:00.749919 simplepytorch-1.2.0/simplepytorch.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     3298 2023-03-08 17:23:00.000000 simplepytorch-1.2.0/simplepytorch.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     1229 2023-03-08 17:23:00.000000 simplepytorch-1.2.0/simplepytorch.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-03-08 17:23:00.000000 simplepytorch-1.2.0/simplepytorch.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-03-08 17:23:00.000000 simplepytorch-1.2.0/simplepytorch.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       14 2023-03-08 17:23:00.000000 simplepytorch-1.2.0/simplepytorch.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.863541 simplepytorch-1.3.0/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1068 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     3278 2023-05-04 15:20:22.863541 simplepytorch-1.3.0/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     2847 2022-04-26 04:35:00.000000 simplepytorch-1.3.0/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.856874 simplepytorch-1.3.0/bin/
+-rwxr-xr-x   0 alex      (1000) alex      (1000)       48 2021-01-20 01:32:25.000000 simplepytorch-1.3.0/bin/simplepytorch
+-rwxr-xr-x   0 alex      (1000) alex      (1000)       90 2021-01-20 01:32:25.000000 simplepytorch-1.3.0/bin/simplepytorch_debug
+-rwxr-xr-x   0 alex      (1000) alex      (1000)       80 2021-01-21 15:57:18.000000 simplepytorch-1.3.0/bin/simplepytorch_plot
+-rw-r--r--   0 alex      (1000) alex      (1000)      248 2023-05-04 15:20:22.863541 simplepytorch-1.3.0/setup.cfg
+-rwxr-xr-x   0 alex      (1000) alex      (1000)     1160 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.860208 simplepytorch-1.3.0/simplepytorch/
+-rw-r--r--   0 alex      (1000) alex      (1000)       22 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       70 2020-06-07 00:23:22.000000 simplepytorch-1.3.0/simplepytorch/__main__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1204 2022-04-25 14:00:07.000000 simplepytorch-1.3.0/simplepytorch/api.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      893 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/cache.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10311 2022-04-25 13:58:29.000000 simplepytorch-1.3.0/simplepytorch/cmdline.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.863541 simplepytorch-1.3.0/simplepytorch/datasets/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6406 2021-06-13 22:51:00.000000 simplepytorch-1.3.0/simplepytorch/datasets/BBBC038v1_microscopy.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      680 2023-03-08 17:21:22.000000 simplepytorch-1.3.0/simplepytorch/datasets/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1772 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/_shared.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10986 2022-11-26 10:17:09.000000 simplepytorch-1.3.0/simplepytorch/datasets/chexpert.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5543 2020-09-08 08:18:00.000000 simplepytorch-1.3.0/simplepytorch/datasets/drive.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2255 2021-09-22 22:34:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/eyepacs.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1112 2021-09-22 22:34:44.000000 simplepytorch-1.3.0/simplepytorch/datasets/glob_image_dir.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3778 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/idrid.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16323 2022-05-16 13:41:31.000000 simplepytorch-1.3.0/simplepytorch/datasets/intel_mobileodt_cervical.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1623 2022-05-31 17:45:19.000000 simplepytorch-1.3.0/simplepytorch/datasets/kimeye.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4024 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/messidor.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1385 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/pickled_dicts.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1314 2022-04-13 00:39:21.000000 simplepytorch-1.3.0/simplepytorch/datasets/preprocess.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9228 2022-04-25 16:29:13.000000 simplepytorch-1.3.0/simplepytorch/datasets/qualdr.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3277 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/rite.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1300 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/train_val_test_split.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1681 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/early_stopping.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16202 2022-04-25 13:56:13.000000 simplepytorch-1.3.0/simplepytorch/feedforward.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17470 2022-04-25 23:56:47.000000 simplepytorch-1.3.0/simplepytorch/logging_tools.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    14712 2023-05-04 15:00:05.000000 simplepytorch-1.3.0/simplepytorch/metrics.py
+-rwxr-xr-x   0 alex      (1000) alex      (1000)    21766 2023-02-07 12:06:45.000000 simplepytorch-1.3.0/simplepytorch/plot_perf.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6102 2022-05-01 10:43:51.000000 simplepytorch-1.3.0/simplepytorch/raytunelib.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    21377 2023-05-04 15:18:50.000000 simplepytorch-1.3.0/simplepytorch/result.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16501 2022-11-24 23:35:20.000000 simplepytorch-1.3.0/simplepytorch/trainlib.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.860208 simplepytorch-1.3.0/simplepytorch.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3278 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     1229 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       14 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/top_level.txt
```

### Comparing `simplepytorch-1.2.0/LICENSE` & `simplepytorch-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/PKG-INFO` & `simplepytorch-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: simplepytorch
-Version: 1.2.0
+Version: 1.3.0
 Summary: Setup and train deep nets with PyTorch. Opinionated and Simple.
 Home-page: https://github.com/adgaudio/simplepytorch
 Author: Alex Gaudio
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dataset_qualdr
 Provides-Extra: ray
 License-File: LICENSE
 
@@ -106,9 +105,7 @@
 
 data/messidor:
 Annotation_Base11.csv  Annotation_Base21.csv  Annotation_Base31.csv  Base11  Base21  Base31
 Annotation_Base12.csv  Annotation_Base22.csv  Annotation_Base32.csv  Base12  Base22  Base32
 Annotation_Base13.csv  Annotation_Base23.csv  Annotation_Base33.csv  Base13  Base23  Base33
 Annotation_Base14.csv  Annotation_Base24.csv  Annotation_Base34.csv  Base14  Base24  Base34
 ```
-
-
```

### Comparing `simplepytorch-1.2.0/README.md` & `simplepytorch-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/setup.py` & `simplepytorch-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 
 setup(
     name='simplepytorch',
-    version='1.2.0',
+    version='1.3.0',
     description='Setup and train deep nets with PyTorch. Opinionated and Simple.',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/adgaudio/simplepytorch",
     author='Alex Gaudio',
     license="MIT",
     classifiers=[
```

### Comparing `simplepytorch-1.2.0/simplepytorch/api.py` & `simplepytorch-1.3.0/simplepytorch/api.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/cache.py` & `simplepytorch-1.3.0/simplepytorch/cache.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/cmdline.py` & `simplepytorch-1.3.0/simplepytorch/cmdline.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/BBBC038v1_microscopy.py` & `simplepytorch-1.3.0/simplepytorch/datasets/BBBC038v1_microscopy.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/__init__.py` & `simplepytorch-1.3.0/simplepytorch/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/_shared.py` & `simplepytorch-1.3.0/simplepytorch/datasets/_shared.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/chexpert.py` & `simplepytorch-1.3.0/simplepytorch/datasets/chexpert.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/drive.py` & `simplepytorch-1.3.0/simplepytorch/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/eyepacs.py` & `simplepytorch-1.3.0/simplepytorch/datasets/eyepacs.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/glob_image_dir.py` & `simplepytorch-1.3.0/simplepytorch/datasets/glob_image_dir.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/idrid.py` & `simplepytorch-1.3.0/simplepytorch/datasets/idrid.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/intel_mobileodt_cervical.py` & `simplepytorch-1.3.0/simplepytorch/datasets/intel_mobileodt_cervical.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/kimeye.py` & `simplepytorch-1.3.0/simplepytorch/datasets/kimeye.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/messidor.py` & `simplepytorch-1.3.0/simplepytorch/datasets/messidor.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/pickled_dicts.py` & `simplepytorch-1.3.0/simplepytorch/datasets/pickled_dicts.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/preprocess.py` & `simplepytorch-1.3.0/simplepytorch/datasets/preprocess.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/qualdr.py` & `simplepytorch-1.3.0/simplepytorch/datasets/qualdr.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/rite.py` & `simplepytorch-1.3.0/simplepytorch/datasets/rite.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/datasets/train_val_test_split.py` & `simplepytorch-1.3.0/simplepytorch/datasets/train_val_test_split.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/early_stopping.py` & `simplepytorch-1.3.0/simplepytorch/early_stopping.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/feedforward.py` & `simplepytorch-1.3.0/simplepytorch/feedforward.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/logging_tools.py` & `simplepytorch-1.3.0/simplepytorch/logging_tools.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/metrics.py` & `simplepytorch-1.3.0/simplepytorch/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,16 @@
     yhat = torch.stack([1-yhat, yhat]).T.float()
     y = torch.stack([1-y, y]).T.float()
     return confusion_matrix_2D_input(y=y, yhat=yhat)
 
 
 def confusion_matrix_2D_input(y: torch.Tensor, yhat: torch.Tensor, normalize_y=False) -> torch.Tensor:
     """
-    Output a confusion matrix from 2D inputs.
+    Output a generalized confusion matrix from 2D inputs.  This is a
+    non-standard setting, supporting soft-assignment.
 
     Inputs are assumed either both LongTensor or both FloatTensor.  In the
     LongTensor setting, the columns of input arrays y and yhat are class index
     and the rows correspond to different (minibatch) samples.  In FloatTensor
     setting, read below to understand better what you're doing.
 
     How: Compute the outer product `y y_{hat}^T` for
@@ -87,19 +88,24 @@
     return torch.einsum('nm,no->mo', w, yhat)
 
 
 def confusion_matrix(y: torch.Tensor, yhat: torch.Tensor, num_classes:int
                      ) -> torch.Tensor:
     """
     A Confusion Matrix enables performance evaluation of a classifier model's
-    predictions.  This function works with multi-class or multi-label data, 1D
-    input vectors or 2-D inputs.  This class generalizes the confusion matrix,
-    so be careful to give inputs of correct type.  To match
-    `sklearn.metrics.confusion_matrix`, just ensure that `y` and `yhat` are
-    integer type rather than float.  Check your result matches expectation.
+    predictions.  This function works with multi-class (or to some extent
+    multi-label data), 1D input vectors or 2-D inputs.  This class generalizes
+    the confusion matrix, so be careful to give inputs of correct type.  To
+    match `sklearn.metrics.confusion_matrix`, just ensure that `y` and `yhat`
+    are integer type rather than float.  Check your result matches expectation.
+    Note that a confusion matrix for multi-label data generally outputs one
+    binary confusion matrix per class.  Analysis of multi-label data using this
+    function is somewhat particular because this function outputs only 1
+    confusion matrix. It does not implement
+    sklearn.metrics.multilabel_confusion_matrix.
 
     Each row index corresponds to a ground truth class.
     Each column index corresponds to predicted class.
 
     Standard example: Binary classification, where class "1" is positive, the
     output confusion matrix is:
```

### Comparing `simplepytorch-1.2.0/simplepytorch/plot_perf.py` & `simplepytorch-1.3.0/simplepytorch/plot_perf.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/raytunelib.py` & `simplepytorch-1.3.0/simplepytorch/raytunelib.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch/result.py` & `simplepytorch-1.3.0/simplepytorch/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,15 +360,15 @@
     """A result class for Multi-Label Binary Classification.
     Maintains one binary confusion matrix for each class and computes
     classification metrics from them.
 
     This class is useful to to aggregate results, for instance over the course
     of an epoch.
     """
-    ALL_METRICS = ('Loss', 'Num Samples', 'MCC', 'Precision', 'Recall', 'F1', 'Acc', 'BAcc', 'cm', 'ROC_AUC')  # 'y', 'yhat',
+    ALL_METRICS = ('Loss', 'Num Samples', 'MCC', 'Precision', 'Recall', 'F1', 'F1micro', 'Acc', 'BAcc', 'cm', 'ROC_AUC')  # 'y', 'yhat',
 
     @property
     def metrics(self):
         return self._metrics
 
     def __init__(self, class_names:list,
                  binarize_fn:Callable[[T.Tensor, float],T.Tensor]=None,
@@ -429,14 +429,19 @@
         return self._on_each_cm('MCC {class_name}', metrics.matthews_correlation_coeff)
 
     @property
     def f1(self):
         return self._on_each_cm('F1 {class_name}', lambda x: metrics.f1_score(x, mode='pos'))
 
     @property
+    def f1micro(self):
+        cm = sum(self._cms.values())
+        return {'F1 Micro-AVG': metrics.f1_score(cm, mode='pos').item()}
+
+    @property
     def precision(self):
         return self._on_each_cm(
             'Precision {class_name}', lambda x: metrics.precision(x, 'pos'))
 
     @property
     def recall(self):
         return self._on_each_cm(
@@ -472,26 +477,26 @@
                 continue
             try:
                 rv[key] = roc_auc_score(
                     y_true=yval, y_score=yhatval, average=None)
             except ValueError:
                 rv[key] = 0  # e.g. degenerate case when all classes are "0" or all are "1"
         if self.report_avg:
-            rv['ROC_AUC AVG'] = sum(rv.values()) / len(rv)
+            rv['ROC_AUC Macro-AVG'] = sum(rv.values()) / len(rv)
         return rv
 
     def _on_each_cm(self, metric_name, fn):
         rv = {}
         avg = 0
         for kls, cm in self._cms.items():
             val = fn(cm).item()
             rv[metric_name.format(class_name=kls)] = val
             avg += val/len(self._cms)
         if self.report_avg:
-            rv[metric_name.format(class_name='AVG')] = avg
+            rv[metric_name.format(class_name='Macro-AVG')] = avg
         return rv
 
     def update(self, yhat, y, loss) -> None:
         """Compute and store results given:
           `yhat` - model predictions of shape (B,C) for B=batch size and C=len(class_names)
           `y` - ground truth of shape (B,C)
           `loss` - training loss
```

### Comparing `simplepytorch-1.2.0/simplepytorch/trainlib.py` & `simplepytorch-1.3.0/simplepytorch/trainlib.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.2.0/simplepytorch.egg-info/PKG-INFO` & `simplepytorch-1.3.0/simplepytorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: simplepytorch
-Version: 1.2.0
+Version: 1.3.0
 Summary: Setup and train deep nets with PyTorch. Opinionated and Simple.
 Home-page: https://github.com/adgaudio/simplepytorch
 Author: Alex Gaudio
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dataset_qualdr
 Provides-Extra: ray
 License-File: LICENSE
 
@@ -106,9 +105,7 @@
 
 data/messidor:
 Annotation_Base11.csv  Annotation_Base21.csv  Annotation_Base31.csv  Base11  Base21  Base31
 Annotation_Base12.csv  Annotation_Base22.csv  Annotation_Base32.csv  Base12  Base22  Base32
 Annotation_Base13.csv  Annotation_Base23.csv  Annotation_Base33.csv  Base13  Base23  Base33
 Annotation_Base14.csv  Annotation_Base24.csv  Annotation_Base34.csv  Base14  Base24  Base34
 ```
-
-
```

### Comparing `simplepytorch-1.2.0/simplepytorch.egg-info/SOURCES.txt` & `simplepytorch-1.3.0/simplepytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

