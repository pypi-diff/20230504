# Comparing `tmp/yolov5_sp-1.0.2.tar.gz` & `tmp/yolov5_sp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov5_sp-1.0.2.tar", last modified: Thu May  4 09:05:09 2023, max compression
+gzip compressed data, was "yolov5_sp-1.0.3.tar", last modified: Thu May  4 10:30:16 2023, max compression
```

## Comparing `yolov5_sp-1.0.2.tar` & `yolov5_sp-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.670644 yolov5_sp-1.0.2/
--rw-rw-rw-   0        0        0      595 2023-05-04 09:05:09.670644 yolov5_sp-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:01.000000 yolov5_sp-1.0.2/README.md
--rw-rw-rw-   0        0        0      588 2023-05-04 06:10:46.000000 yolov5_sp-1.0.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 09:05:09.670644 yolov5_sp-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1485 2023-05-04 09:04:50.000000 yolov5_sp-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.654457 yolov5_sp-1.0.2/yolov5_sp/
--rw-rw-rw-   0        0        0      178 2023-05-04 05:59:20.000000 yolov5_sp-1.0.2/yolov5_sp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.660457 yolov5_sp-1.0.2/yolov5_sp/models/
--rw-rw-rw-   0        0        0      178 2023-05-04 08:07:52.000000 yolov5_sp-1.0.2/yolov5_sp/models/__init__.py
--rw-rw-rw-   0        0        0    20133 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/models/common.py
--rw-rw-rw-   0        0        0     4551 2023-05-04 09:04:38.000000 yolov5_sp-1.0.2/yolov5_sp/models/experimental.py
--rw-rw-rw-   0        0        0    14693 2022-06-10 09:11:52.000000 yolov5_sp-1.0.2/yolov5_sp/models/yolo.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.669644 yolov5_sp-1.0.2/yolov5_sp/utils/
--rw-rw-rw-   0        0        0      178 2023-05-04 06:00:33.000000 yolov5_sp-1.0.2/yolov5_sp/utils/__init__.py
--rw-rw-rw-   0        0        0     3774 2022-06-10 09:11:53.000000 yolov5_sp-1.0.2/yolov5_sp/utils/activations.py
--rw-rw-rw-   0        0        0    11747 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/augmentations.py
--rw-rw-rw-   0        0        0     7110 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/autoanchor.py
--rw-rw-rw-   0        0        0     2248 2022-06-10 09:11:53.000000 yolov5_sp-1.0.2/yolov5_sp/utils/callbacks.py
--rw-rw-rw-   0        0        0    44157 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/datasets.py
--rw-rw-rw-   0        0        0     6115 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/downloads.py
--rw-rw-rw-   0        0        0    34125 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/general.py
--rw-rw-rw-   0        0        0     4560 2023-02-07 12:04:41.000000 yolov5_sp-1.0.2/yolov5_sp/utils/log.py
--rw-rw-rw-   0        0        0     9739 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/loss.py
--rw-rw-rw-   0        0        0    13503 2022-06-10 09:11:53.000000 yolov5_sp-1.0.2/yolov5_sp/utils/metrics.py
--rw-rw-rw-   0        0        0    19369 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/plots.py
--rw-rw-rw-   0        0        0     2822 2022-11-30 08:13:03.000000 yolov5_sp-1.0.2/yolov5_sp/utils/resize_and_pad.py
--rw-rw-rw-   0        0        0    14025 2022-06-10 09:11:53.000000 yolov5_sp-1.0.2/yolov5_sp/utils/torch_utils.py
--rw-rw-rw-   0        0        0     3202 2023-05-04 09:04:38.000000 yolov5_sp-1.0.2/yolov5_sp/yolov5.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.657457 yolov5_sp-1.0.2/yolov5_sp.egg-info/
--rw-rw-rw-   0        0        0      595 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 10:30:15.997522 yolov5_sp-1.0.3/
+-rw-rw-rw-   0        0        0      595 2023-05-04 10:30:15.996522 yolov5_sp-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:12:01.000000 yolov5_sp-1.0.3/README.md
+-rw-rw-rw-   0        0        0      588 2023-05-04 06:10:46.000000 yolov5_sp-1.0.3/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:30:15.997522 yolov5_sp-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1485 2023-05-04 10:29:22.000000 yolov5_sp-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:30:15.979516 yolov5_sp-1.0.3/yolov5_sp/
+-rw-rw-rw-   0        0        0      178 2023-05-04 05:59:20.000000 yolov5_sp-1.0.3/yolov5_sp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:30:15.984528 yolov5_sp-1.0.3/yolov5_sp/configs/
+-rw-rw-rw-   0        0        0        0 2023-04-07 02:54:35.000000 yolov5_sp-1.0.3/yolov5_sp/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:30:15.986514 yolov5_sp-1.0.3/yolov5_sp/models/
+-rw-rw-rw-   0        0        0      178 2023-05-04 08:07:52.000000 yolov5_sp-1.0.3/yolov5_sp/models/__init__.py
+-rw-rw-rw-   0        0        0    20133 2023-05-04 09:03:39.000000 yolov5_sp-1.0.3/yolov5_sp/models/common.py
+-rw-rw-rw-   0        0        0     4551 2023-05-04 09:04:38.000000 yolov5_sp-1.0.3/yolov5_sp/models/experimental.py
+-rw-rw-rw-   0        0        0    14693 2022-06-10 09:11:52.000000 yolov5_sp-1.0.3/yolov5_sp/models/yolo.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:30:15.995515 yolov5_sp-1.0.3/yolov5_sp/utils/
+-rw-rw-rw-   0        0        0      178 2023-05-04 06:00:33.000000 yolov5_sp-1.0.3/yolov5_sp/utils/__init__.py
+-rw-rw-rw-   0        0        0     3774 2022-06-10 09:11:53.000000 yolov5_sp-1.0.3/yolov5_sp/utils/activations.py
+-rw-rw-rw-   0        0        0    11747 2023-05-04 09:03:39.000000 yolov5_sp-1.0.3/yolov5_sp/utils/augmentations.py
+-rw-rw-rw-   0        0        0     7110 2023-05-04 09:03:39.000000 yolov5_sp-1.0.3/yolov5_sp/utils/autoanchor.py
+-rw-rw-rw-   0        0        0     2248 2022-06-10 09:11:53.000000 yolov5_sp-1.0.3/yolov5_sp/utils/callbacks.py
+-rw-rw-rw-   0        0        0    44157 2023-05-04 09:03:39.000000 yolov5_sp-1.0.3/yolov5_sp/utils/datasets.py
+-rw-rw-rw-   0        0        0     6115 2023-05-04 09:03:39.000000 yolov5_sp-1.0.3/yolov5_sp/utils/downloads.py
+-rw-rw-rw-   0        0        0    34125 2023-05-04 09:03:39.000000 yolov5_sp-1.0.3/yolov5_sp/utils/general.py
+-rw-rw-rw-   0        0        0     4560 2023-02-07 12:04:41.000000 yolov5_sp-1.0.3/yolov5_sp/utils/log.py
+-rw-rw-rw-   0        0        0     9739 2023-05-04 09:03:39.000000 yolov5_sp-1.0.3/yolov5_sp/utils/loss.py
+-rw-rw-rw-   0        0        0    13503 2022-06-10 09:11:53.000000 yolov5_sp-1.0.3/yolov5_sp/utils/metrics.py
+-rw-rw-rw-   0        0        0    19369 2023-05-04 09:03:39.000000 yolov5_sp-1.0.3/yolov5_sp/utils/plots.py
+-rw-rw-rw-   0        0        0     2822 2022-11-30 08:13:03.000000 yolov5_sp-1.0.3/yolov5_sp/utils/resize_and_pad.py
+-rw-rw-rw-   0        0        0    14025 2022-06-10 09:11:53.000000 yolov5_sp-1.0.3/yolov5_sp/utils/torch_utils.py
+-rw-rw-rw-   0        0        0     3205 2023-05-04 10:21:26.000000 yolov5_sp-1.0.3/yolov5_sp/yolov5.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:30:15.983527 yolov5_sp-1.0.3/yolov5_sp.egg-info/
+-rw-rw-rw-   0        0        0      595 2023-05-04 10:30:15.000000 yolov5_sp-1.0.3/yolov5_sp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2023-05-04 10:30:15.000000 yolov5_sp-1.0.3/yolov5_sp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:30:15.000000 yolov5_sp-1.0.3/yolov5_sp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-04 10:30:15.000000 yolov5_sp-1.0.3/yolov5_sp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2023-05-04 10:30:15.000000 yolov5_sp-1.0.3/yolov5_sp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 10:30:15.000000 yolov5_sp-1.0.3/yolov5_sp.egg-info/top_level.txt
```

### Comparing `yolov5_sp-1.0.2/PKG-INFO` & `yolov5_sp-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5_sp
-Version: 1.0.2
+Version: 1.0.3
 Summary: yolov5-v5.0 general model
 Home-page: https://github.com/Easonshow
 Author: shaop
 Author-email: 13585800607@163.com
 Maintainer: shaop
 Maintainer-email: 13585800607@163.com
 License: MIT License
```

### Comparing `yolov5_sp-1.0.2/license.txt` & `yolov5_sp-1.0.3/license.txt`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/setup.py` & `yolov5_sp-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yolov5_sp',  # 包名
-    version='1.0.2',  # 版本
+    version='1.0.3',  # 版本
     description="yolov5-v5.0 general model",  # 包简介
     long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='shaop',  # 作者
     author_email='13585800607@163.com',  # 作者邮件
     maintainer='shaop',  # 维护者
     maintainer_email='13585800607@163.com',  # 维护者邮件
```

### Comparing `yolov5_sp-1.0.2/yolov5_sp/models/common.py` & `yolov5_sp-1.0.3/yolov5_sp/models/common.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/models/experimental.py` & `yolov5_sp-1.0.3/yolov5_sp/models/experimental.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/models/yolo.py` & `yolov5_sp-1.0.3/yolov5_sp/models/yolo.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/activations.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/activations.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/augmentations.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/autoanchor.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/callbacks.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/datasets.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/downloads.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/general.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/general.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/log.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/log.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/loss.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/loss.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/metrics.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/plots.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/plots.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/resize_and_pad.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/resize_and_pad.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/utils/torch_utils.py` & `yolov5_sp-1.0.3/yolov5_sp/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.2/yolov5_sp/yolov5.py` & `yolov5_sp-1.0.3/yolov5_sp/yolov5.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,20 +58,20 @@
                     res_dict["box"] = torch.Tensor(xyxy).tolist()
                     pred_res.append(res_dict)
             else:
                 pred_res = [{'class_label': None, 'conf': None, 'box': None}]
         return pred_res
 
 if __name__ == "__main__":
-    image_folder = '/home/sp/data/iphone14/2023-04-21-imgs'
+    image_folder = r'E:\ahs_project_code\ahs_test_code\cut\test_data'
 
     for image in os.listdir(image_folder):
         image_path = os.path.join(image_folder,image)
         pred_img = cv2.imdecode(np.fromfile(image_path,dtype=np.uint8),cv2.IMREAD_COLOR)
-        yolov5 = YoloV5_Six('0','../configs')
+        yolov5 = YoloV5_Six('configs')
         re_list = yolov5.infer(pred_img)
         print(re_list)
```

### Comparing `yolov5_sp-1.0.2/yolov5_sp.egg-info/PKG-INFO` & `yolov5_sp-1.0.3/yolov5_sp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5-sp
-Version: 1.0.2
+Version: 1.0.3
 Summary: yolov5-v5.0 general model
 Home-page: https://github.com/Easonshow
 Author: shaop
 Author-email: 13585800607@163.com
 Maintainer: shaop
 Maintainer-email: 13585800607@163.com
 License: MIT License
```

### Comparing `yolov5_sp-1.0.2/yolov5_sp.egg-info/SOURCES.txt` & `yolov5_sp-1.0.3/yolov5_sp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 yolov5_sp/yolov5.py
 yolov5_sp.egg-info/PKG-INFO
 yolov5_sp.egg-info/SOURCES.txt
 yolov5_sp.egg-info/dependency_links.txt
 yolov5_sp.egg-info/entry_points.txt
 yolov5_sp.egg-info/requires.txt
 yolov5_sp.egg-info/top_level.txt
+yolov5_sp/configs/__init__.py
 yolov5_sp/models/__init__.py
 yolov5_sp/models/common.py
 yolov5_sp/models/experimental.py
 yolov5_sp/models/yolo.py
 yolov5_sp/utils/__init__.py
 yolov5_sp/utils/activations.py
 yolov5_sp/utils/augmentations.py
```

