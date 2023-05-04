# Comparing `tmp/ccdt-2.0.3.tar.gz` & `tmp/ccdt-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.0.3.tar", last modified: Thu Apr 27 07:14:14 2023, max compression
+gzip compressed data, was "ccdt-2.0.4.tar", last modified: Thu May  4 05:52:42 2023, max compression
```

## Comparing `ccdt-2.0.3.tar` & `ccdt-2.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.304269 ccdt-2.0.3/
--rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     4319 2023-04-27 07:14:14.303272 ccdt-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.270364 ccdt-2.0.3/ccdt/
--rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.3/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.282329 ccdt-2.0.3/ccdt/dataset/
--rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.3/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.285333 ccdt-2.0.3/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.3/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.3/ccdt/dataset/base_coco/coco.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.290310 ccdt-2.0.3/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.3/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.3/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    60692 2023-04-27 02:23:46.000000 ccdt-2.0.3/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.291310 ccdt-2.0.3/ccdt/dataset/logs/
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.3/ccdt/dataset/logs/__init__.py
--rw-rw-rw-   0        0        0    11356 2023-04-27 01:34:21.000000 ccdt-2.0.3/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.297289 ccdt-2.0.3/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      200 2023-04-17 07:06:14.000000 ccdt-2.0.3/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.3/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    10182 2023-04-25 10:32:57.000000 ccdt-2.0.3/ccdt/dataset/utils/labelme_load.py
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.3/ccdt/dataset/utils/logs.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.302251 ccdt-2.0.3/ccdt/video_tool/
--rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.3/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.3/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.3/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-04-27 07:14:14.279336 ccdt-2.0.3/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4319 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 07:14:14.000000 ccdt-2.0.3/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 07:14:14.304269 ccdt-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2278 2023-04-27 06:57:07.000000 ccdt-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.561290 ccdt-2.0.4/
+-rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4319 2023-05-04 05:52:42.560298 ccdt-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.501431 ccdt-2.0.4/ccdt/
+-rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.4/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.523372 ccdt-2.0.4/ccdt/dataset/
+-rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.4/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.528358 ccdt-2.0.4/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.4/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.4/ccdt/dataset/base_coco/coco.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.536337 ccdt-2.0.4/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.4/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.4/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0    60750 2023-05-04 05:50:19.000000 ccdt-2.0.4/ccdt/dataset/base_labelme/base_labelme.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.538357 ccdt-2.0.4/ccdt/dataset/logs/
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.4/ccdt/dataset/logs/__init__.py
+-rw-rw-rw-   0        0        0    11343 2023-04-27 08:58:08.000000 ccdt-2.0.4/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.549301 ccdt-2.0.4/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      200 2023-04-17 07:06:14.000000 ccdt-2.0.4/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.4/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    10182 2023-04-25 10:32:57.000000 ccdt-2.0.4/ccdt/dataset/utils/labelme_load.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.4/ccdt/dataset/utils/logs.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.556315 ccdt-2.0.4/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.4/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.4/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.4/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:52:42.517418 ccdt-2.0.4/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4319 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-04 05:52:42.000000 ccdt-2.0.4/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 05:52:42.562268 ccdt-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2278 2023-05-04 05:52:04.000000 ccdt-2.0.4/setup.py
```

### Comparing `ccdt-2.0.3/LICENSE` & `ccdt-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.3/PKG-INFO` & `ccdt-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.3
+Version: 2.0.4
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.3/README.md` & `ccdt-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.3/ccdt/dataset/base_coco/coco.py` & `ccdt-2.0.4/ccdt/dataset/base_coco/coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.3/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.0.4/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.3/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.0.4/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,19 +182,19 @@
         # print(property_tb)
         # print(num_tb)
         print(num_tb.get_string(title=title))
         print(property_tb.get_string(title=title))
 
     def split_list(self, parameter):
         """
-        将列表平均分成 extract_amount 份
+        将列表平均分成 extract_amount 份。同时把向下取整的余数自动多增加一份。
         :param parameter: 指定份数
         """
         random.shuffle(self.datasets)
-        avg = len(self.datasets) / float(parameter.extract_portion)
+        avg = len(self.datasets) // float(parameter.extract_portion)
         # result = []  # 分好后追加列表又会导致内存里面多了一份数据集
         last = 0.0
         index = 0
         while last < len(self.datasets):
             # result.append(self.datasets[int(last):int(last + avg)])
             # 直接传递列表到，save_labelme方法进行迭代后保存，省去了重写保存方法
             self.save_labelme(self.datasets[int(last):int(last + avg)], index, parameter.label_name)
```

### Comparing `ccdt-2.0.3/ccdt/dataset/main.py` & `ccdt-2.0.4/ccdt/dataset/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Time : 2023/3/30 16:23
 # @Author : Zhan Yong
 # @System : jk
 import argparse
 import ast
 from ccdt.dataset import *
-import json
 
 
 def parser_args():
     parser = argparse.ArgumentParser()
     parser.add_argument('input_datasets', type=ast.literal_eval, help="labelme数据集路径、coco数据集路径，列表字典传参")
     parser.add_argument('--output-dir', type=str, help="保存路径")
     # parser.add_argument('--replace-dir', type=str, help="替换路径")
```

### Comparing `ccdt-2.0.3/ccdt/dataset/utils/encoder.py` & `ccdt-2.0.4/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.3/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.0.4/ccdt/dataset/utils/labelme_load.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.3/ccdt/video_tool/split.py` & `ccdt-2.0.4/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.3/ccdt/video_tool/video_main.py` & `ccdt-2.0.4/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.3/ccdt.egg-info/PKG-INFO` & `ccdt-2.0.4/ccdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.3
+Version: 2.0.4
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.0.3/ccdt.egg-info/SOURCES.txt` & `ccdt-2.0.4/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.3/setup.py` & `ccdt-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.0.3',
+    version='2.0.4',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

