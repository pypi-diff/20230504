# Comparing `tmp/yolov5_sp-1.0.0.tar.gz` & `tmp/yolov5_sp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov5_sp-1.0.0.tar", last modified: Thu May  4 07:52:45 2023, max compression
+gzip compressed data, was "yolov5_sp-1.0.1.tar", last modified: Thu May  4 08:08:41 2023, max compression
```

## Comparing `yolov5_sp-1.0.0.tar` & `yolov5_sp-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 07:52:45.454719 yolov5_sp-1.0.0/
--rw-rw-rw-   0        0        0      595 2023-05-04 07:52:45.454719 yolov5_sp-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:01.000000 yolov5_sp-1.0.0/README.md
--rw-rw-rw-   0        0        0      588 2023-05-04 06:10:46.000000 yolov5_sp-1.0.0/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 07:52:45.454719 yolov5_sp-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1451 2023-05-04 07:52:24.000000 yolov5_sp-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:52:45.441051 yolov5_sp-1.0.0/yolov5_sp/
--rw-rw-rw-   0        0        0      178 2023-05-04 05:59:20.000000 yolov5_sp-1.0.0/yolov5_sp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:52:45.453716 yolov5_sp-1.0.0/yolov5_sp/utils/
--rw-rw-rw-   0        0        0      178 2023-05-04 06:00:33.000000 yolov5_sp-1.0.0/yolov5_sp/utils/__init__.py
--rw-rw-rw-   0        0        0     3774 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/activations.py
--rw-rw-rw-   0        0        0    11727 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/augmentations.py
--rw-rw-rw-   0        0        0     7080 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/autoanchor.py
--rw-rw-rw-   0        0        0     2248 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/callbacks.py
--rw-rw-rw-   0        0        0    44087 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/datasets.py
--rw-rw-rw-   0        0        0     6105 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/downloads.py
--rw-rw-rw-   0        0        0    34095 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/general.py
--rw-rw-rw-   0        0        0     4560 2023-02-07 12:04:41.000000 yolov5_sp-1.0.0/yolov5_sp/utils/log.py
--rw-rw-rw-   0        0        0     9719 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/loss.py
--rw-rw-rw-   0        0        0    13503 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/metrics.py
--rw-rw-rw-   0        0        0    19279 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/plots.py
--rw-rw-rw-   0        0        0     2822 2022-11-30 08:13:03.000000 yolov5_sp-1.0.0/yolov5_sp/utils/resize_and_pad.py
--rw-rw-rw-   0        0        0    14025 2022-06-10 09:11:53.000000 yolov5_sp-1.0.0/yolov5_sp/utils/torch_utils.py
--rw-rw-rw-   0        0        0     3172 2023-04-27 07:24:45.000000 yolov5_sp-1.0.0/yolov5_sp/yolov5.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:52:45.445068 yolov5_sp-1.0.0/yolov5_sp.egg-info/
--rw-rw-rw-   0        0        0      595 2023-05-04 07:52:45.000000 yolov5_sp-1.0.0/yolov5_sp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2023-05-04 07:52:45.000000 yolov5_sp-1.0.0/yolov5_sp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 07:52:45.000000 yolov5_sp-1.0.0/yolov5_sp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-04 07:52:45.000000 yolov5_sp-1.0.0/yolov5_sp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-05-04 07:52:45.000000 yolov5_sp-1.0.0/yolov5_sp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 07:52:45.000000 yolov5_sp-1.0.0/yolov5_sp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.651852 yolov5_sp-1.0.1/
+-rw-rw-rw-   0        0        0      595 2023-05-04 08:08:41.650850 yolov5_sp-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:12:01.000000 yolov5_sp-1.0.1/README.md
+-rw-rw-rw-   0        0        0      588 2023-05-04 06:10:46.000000 yolov5_sp-1.0.1/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 08:08:41.651852 yolov5_sp-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1451 2023-05-04 08:08:19.000000 yolov5_sp-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.636985 yolov5_sp-1.0.1/yolov5_sp/
+-rw-rw-rw-   0        0        0      178 2023-05-04 05:59:20.000000 yolov5_sp-1.0.1/yolov5_sp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.641849 yolov5_sp-1.0.1/yolov5_sp/models/
+-rw-rw-rw-   0        0        0      178 2023-05-04 08:07:52.000000 yolov5_sp-1.0.1/yolov5_sp/models/__init__.py
+-rw-rw-rw-   0        0        0    20093 2022-06-10 09:11:52.000000 yolov5_sp-1.0.1/yolov5_sp/models/common.py
+-rw-rw-rw-   0        0        0     4521 2022-06-10 09:11:52.000000 yolov5_sp-1.0.1/yolov5_sp/models/experimental.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.650850 yolov5_sp-1.0.1/yolov5_sp/utils/
+-rw-rw-rw-   0        0        0      178 2023-05-04 06:00:33.000000 yolov5_sp-1.0.1/yolov5_sp/utils/__init__.py
+-rw-rw-rw-   0        0        0     3774 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/activations.py
+-rw-rw-rw-   0        0        0    11727 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/augmentations.py
+-rw-rw-rw-   0        0        0     7080 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/autoanchor.py
+-rw-rw-rw-   0        0        0     2248 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/callbacks.py
+-rw-rw-rw-   0        0        0    44087 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/datasets.py
+-rw-rw-rw-   0        0        0     6105 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/downloads.py
+-rw-rw-rw-   0        0        0    34095 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/general.py
+-rw-rw-rw-   0        0        0     4560 2023-02-07 12:04:41.000000 yolov5_sp-1.0.1/yolov5_sp/utils/log.py
+-rw-rw-rw-   0        0        0     9719 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/loss.py
+-rw-rw-rw-   0        0        0    13503 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/metrics.py
+-rw-rw-rw-   0        0        0    19279 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/plots.py
+-rw-rw-rw-   0        0        0     2822 2022-11-30 08:13:03.000000 yolov5_sp-1.0.1/yolov5_sp/utils/resize_and_pad.py
+-rw-rw-rw-   0        0        0    14025 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/torch_utils.py
+-rw-rw-rw-   0        0        0     3172 2023-04-27 07:24:45.000000 yolov5_sp-1.0.1/yolov5_sp/yolov5.py
+drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.640836 yolov5_sp-1.0.1/yolov5_sp.egg-info/
+-rw-rw-rw-   0        0        0      595 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/top_level.txt
```

### Comparing `yolov5_sp-1.0.0/PKG-INFO` & `yolov5_sp-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5_sp
-Version: 1.0.0
+Version: 1.0.1
 Summary: yolov5-v5.0 general model
 Home-page: https://github.com/Easonshow
 Author: shaop
 Author-email: 13585800607@163.com
 Maintainer: shaop
 Maintainer-email: 13585800607@163.com
 License: MIT License
```

### Comparing `yolov5_sp-1.0.0/license.txt` & `yolov5_sp-1.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/setup.py` & `yolov5_sp-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yolov5_sp',  # 包名
-    version='1.0.0',  # 版本
+    version='1.0.1',  # 版本
     description="yolov5-v5.0 general model",  # 包简介
     long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='shaop',  # 作者
     author_email='13585800607@163.com',  # 作者邮件
     maintainer='shaop',  # 维护者
     maintainer_email='13585800607@163.com',  # 维护者邮件
```

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/activations.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/activations.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/augmentations.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/autoanchor.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/callbacks.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/datasets.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/downloads.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/general.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/general.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/log.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/log.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/loss.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/loss.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/metrics.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/plots.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/plots.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/resize_and_pad.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/resize_and_pad.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/utils/torch_utils.py` & `yolov5_sp-1.0.1/yolov5_sp/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp/yolov5.py` & `yolov5_sp-1.0.1/yolov5_sp/yolov5.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.0/yolov5_sp.egg-info/PKG-INFO` & `yolov5_sp-1.0.1/yolov5_sp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5-sp
-Version: 1.0.0
+Version: 1.0.1
 Summary: yolov5-v5.0 general model
 Home-page: https://github.com/Easonshow
 Author: shaop
 Author-email: 13585800607@163.com
 Maintainer: shaop
 Maintainer-email: 13585800607@163.com
 License: MIT License
```

### Comparing `yolov5_sp-1.0.0/yolov5_sp.egg-info/SOURCES.txt` & `yolov5_sp-1.0.1/yolov5_sp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 yolov5_sp/yolov5.py
 yolov5_sp.egg-info/PKG-INFO
 yolov5_sp.egg-info/SOURCES.txt
 yolov5_sp.egg-info/dependency_links.txt
 yolov5_sp.egg-info/entry_points.txt
 yolov5_sp.egg-info/requires.txt
 yolov5_sp.egg-info/top_level.txt
+yolov5_sp/models/__init__.py
+yolov5_sp/models/common.py
+yolov5_sp/models/experimental.py
 yolov5_sp/utils/__init__.py
 yolov5_sp/utils/activations.py
 yolov5_sp/utils/augmentations.py
 yolov5_sp/utils/autoanchor.py
 yolov5_sp/utils/callbacks.py
 yolov5_sp/utils/datasets.py
 yolov5_sp/utils/downloads.py
```

