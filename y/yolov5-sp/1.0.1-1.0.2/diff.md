# Comparing `tmp/yolov5_sp-1.0.1.tar.gz` & `tmp/yolov5_sp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov5_sp-1.0.1.tar", last modified: Thu May  4 08:08:41 2023, max compression
+gzip compressed data, was "yolov5_sp-1.0.2.tar", last modified: Thu May  4 09:05:09 2023, max compression
```

## Comparing `yolov5_sp-1.0.1.tar` & `yolov5_sp-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.651852 yolov5_sp-1.0.1/
--rw-rw-rw-   0        0        0      595 2023-05-04 08:08:41.650850 yolov5_sp-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:01.000000 yolov5_sp-1.0.1/README.md
--rw-rw-rw-   0        0        0      588 2023-05-04 06:10:46.000000 yolov5_sp-1.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 08:08:41.651852 yolov5_sp-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1451 2023-05-04 08:08:19.000000 yolov5_sp-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.636985 yolov5_sp-1.0.1/yolov5_sp/
--rw-rw-rw-   0        0        0      178 2023-05-04 05:59:20.000000 yolov5_sp-1.0.1/yolov5_sp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.641849 yolov5_sp-1.0.1/yolov5_sp/models/
--rw-rw-rw-   0        0        0      178 2023-05-04 08:07:52.000000 yolov5_sp-1.0.1/yolov5_sp/models/__init__.py
--rw-rw-rw-   0        0        0    20093 2022-06-10 09:11:52.000000 yolov5_sp-1.0.1/yolov5_sp/models/common.py
--rw-rw-rw-   0        0        0     4521 2022-06-10 09:11:52.000000 yolov5_sp-1.0.1/yolov5_sp/models/experimental.py
-drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.650850 yolov5_sp-1.0.1/yolov5_sp/utils/
--rw-rw-rw-   0        0        0      178 2023-05-04 06:00:33.000000 yolov5_sp-1.0.1/yolov5_sp/utils/__init__.py
--rw-rw-rw-   0        0        0     3774 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/activations.py
--rw-rw-rw-   0        0        0    11727 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/augmentations.py
--rw-rw-rw-   0        0        0     7080 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/autoanchor.py
--rw-rw-rw-   0        0        0     2248 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/callbacks.py
--rw-rw-rw-   0        0        0    44087 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/datasets.py
--rw-rw-rw-   0        0        0     6105 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/downloads.py
--rw-rw-rw-   0        0        0    34095 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/general.py
--rw-rw-rw-   0        0        0     4560 2023-02-07 12:04:41.000000 yolov5_sp-1.0.1/yolov5_sp/utils/log.py
--rw-rw-rw-   0        0        0     9719 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/loss.py
--rw-rw-rw-   0        0        0    13503 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/metrics.py
--rw-rw-rw-   0        0        0    19279 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/plots.py
--rw-rw-rw-   0        0        0     2822 2022-11-30 08:13:03.000000 yolov5_sp-1.0.1/yolov5_sp/utils/resize_and_pad.py
--rw-rw-rw-   0        0        0    14025 2022-06-10 09:11:53.000000 yolov5_sp-1.0.1/yolov5_sp/utils/torch_utils.py
--rw-rw-rw-   0        0        0     3172 2023-04-27 07:24:45.000000 yolov5_sp-1.0.1/yolov5_sp/yolov5.py
-drwxrwxrwx   0        0        0        0 2023-05-04 08:08:41.640836 yolov5_sp-1.0.1/yolov5_sp.egg-info/
--rw-rw-rw-   0        0        0      595 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 08:08:41.000000 yolov5_sp-1.0.1/yolov5_sp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.670644 yolov5_sp-1.0.2/
+-rw-rw-rw-   0        0        0      595 2023-05-04 09:05:09.670644 yolov5_sp-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:12:01.000000 yolov5_sp-1.0.2/README.md
+-rw-rw-rw-   0        0        0      588 2023-05-04 06:10:46.000000 yolov5_sp-1.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 09:05:09.670644 yolov5_sp-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1485 2023-05-04 09:04:50.000000 yolov5_sp-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.654457 yolov5_sp-1.0.2/yolov5_sp/
+-rw-rw-rw-   0        0        0      178 2023-05-04 05:59:20.000000 yolov5_sp-1.0.2/yolov5_sp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.660457 yolov5_sp-1.0.2/yolov5_sp/models/
+-rw-rw-rw-   0        0        0      178 2023-05-04 08:07:52.000000 yolov5_sp-1.0.2/yolov5_sp/models/__init__.py
+-rw-rw-rw-   0        0        0    20133 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/models/common.py
+-rw-rw-rw-   0        0        0     4551 2023-05-04 09:04:38.000000 yolov5_sp-1.0.2/yolov5_sp/models/experimental.py
+-rw-rw-rw-   0        0        0    14693 2022-06-10 09:11:52.000000 yolov5_sp-1.0.2/yolov5_sp/models/yolo.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.669644 yolov5_sp-1.0.2/yolov5_sp/utils/
+-rw-rw-rw-   0        0        0      178 2023-05-04 06:00:33.000000 yolov5_sp-1.0.2/yolov5_sp/utils/__init__.py
+-rw-rw-rw-   0        0        0     3774 2022-06-10 09:11:53.000000 yolov5_sp-1.0.2/yolov5_sp/utils/activations.py
+-rw-rw-rw-   0        0        0    11747 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/augmentations.py
+-rw-rw-rw-   0        0        0     7110 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/autoanchor.py
+-rw-rw-rw-   0        0        0     2248 2022-06-10 09:11:53.000000 yolov5_sp-1.0.2/yolov5_sp/utils/callbacks.py
+-rw-rw-rw-   0        0        0    44157 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/datasets.py
+-rw-rw-rw-   0        0        0     6115 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/downloads.py
+-rw-rw-rw-   0        0        0    34125 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/general.py
+-rw-rw-rw-   0        0        0     4560 2023-02-07 12:04:41.000000 yolov5_sp-1.0.2/yolov5_sp/utils/log.py
+-rw-rw-rw-   0        0        0     9739 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/loss.py
+-rw-rw-rw-   0        0        0    13503 2022-06-10 09:11:53.000000 yolov5_sp-1.0.2/yolov5_sp/utils/metrics.py
+-rw-rw-rw-   0        0        0    19369 2023-05-04 09:03:39.000000 yolov5_sp-1.0.2/yolov5_sp/utils/plots.py
+-rw-rw-rw-   0        0        0     2822 2022-11-30 08:13:03.000000 yolov5_sp-1.0.2/yolov5_sp/utils/resize_and_pad.py
+-rw-rw-rw-   0        0        0    14025 2022-06-10 09:11:53.000000 yolov5_sp-1.0.2/yolov5_sp/utils/torch_utils.py
+-rw-rw-rw-   0        0        0     3202 2023-05-04 09:04:38.000000 yolov5_sp-1.0.2/yolov5_sp/yolov5.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:05:09.657457 yolov5_sp-1.0.2/yolov5_sp.egg-info/
+-rw-rw-rw-   0        0        0      595 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 09:05:09.000000 yolov5_sp-1.0.2/yolov5_sp.egg-info/top_level.txt
```

### Comparing `yolov5_sp-1.0.1/PKG-INFO` & `yolov5_sp-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5_sp
-Version: 1.0.1
+Version: 1.0.2
 Summary: yolov5-v5.0 general model
 Home-page: https://github.com/Easonshow
 Author: shaop
 Author-email: 13585800607@163.com
 Maintainer: shaop
 Maintainer-email: 13585800607@163.com
 License: MIT License
```

### Comparing `yolov5_sp-1.0.1/license.txt` & `yolov5_sp-1.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.1/setup.py` & `yolov5_sp-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yolov5_sp',  # 包名
-    version='1.0.1',  # 版本
+    version='1.0.2',  # 版本
     description="yolov5-v5.0 general model",  # 包简介
     long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='shaop',  # 作者
     author_email='13585800607@163.com',  # 作者邮件
     maintainer='shaop',  # 维护者
     maintainer_email='13585800607@163.com',  # 维护者邮件
@@ -23,14 +23,15 @@
     python_requires='>=3.6',  # 设置python版本要求
     install_requires=['opencv-python',
                       'numpy',
                       'pyyaml',
                       'pandas',
                       'requests',
                       'pillow',
-                      'tqdm'],  # 安装所需要的库
+                      'tqdm',
+                      'seaborn'],  # 安装所需要的库
     entry_points={
         'console_scripts': [
             ''],
     },  # 设置命令行工具(可不使用就可以注释掉)
 
 )
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/models/common.py` & `yolov5_sp-1.0.2/yolov5_sp/models/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 import pandas as pd
 import requests
 import torch
 import torch.nn as nn
 from PIL import Image
 from torch.cuda import amp
 
-from utils.datasets import exif_transpose, letterbox
-from utils.general import colorstr, increment_path, make_divisible, non_max_suppression, save_one_box, \
+from yolov5_sp.utils.datasets import exif_transpose, letterbox
+from yolov5_sp.utils.general import colorstr, increment_path, make_divisible, non_max_suppression, save_one_box, \
     scale_coords, xyxy2xywh
-from utils.plots import Annotator, colors
-from utils.torch_utils import time_sync
+from yolov5_sp.utils.plots import Annotator, colors
+from yolov5_sp.utils.torch_utils import time_sync
 
 LOGGER = logging.getLogger(__name__)
 
 
 def autopad(k, p=None):  # kernel, padding
     # Pad to 'same'
     if p is None:
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/models/experimental.py` & `yolov5_sp-1.0.2/yolov5_sp/models/experimental.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Experimental modules
 """
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from models.common import Conv
-from utils.downloads import attempt_download
+from yolov5_sp.models.common import Conv
+from yolov5_sp.utils.downloads import attempt_download
 
 
 class CrossConv(nn.Module):
     # Cross Convolution Downsample
     def __init__(self, c1, c2, k=3, s=1, g=1, e=1.0, shortcut=False):
         # ch_in, ch_out, kernel, stride, groups, expansion, shortcut
         super().__init__()
@@ -82,15 +82,15 @@
         # y = torch.stack(y).max(0)[0]  # max ensemble
         # y = torch.stack(y).mean(0)  # mean ensemble
         y = torch.cat(y, 1)  # nms ensemble
         return y, None  # inference, train output
 
 
 def attempt_load(weights, map_location=None, inplace=True, fuse=True):
-    from models.yolo import Detect, Model
+    from yolov5_sp.models.yolo import Detect, Model
 
     # Loads an ensemble of models weights=[a,b,c] or a single model weights=[a] or weights=a
     model = Ensemble()
     for w in weights if isinstance(weights, list) else [weights]:
         ckpt = torch.load(attempt_download(w), map_location=map_location)  # load
         if fuse:
             model.append(ckpt['ema' if ckpt.get('ema') else 'model'].float().fuse().eval())  # FP32 model
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/activations.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/activations.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/augmentations.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/augmentations.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import logging
 import math
 import random
 
 import cv2
 import numpy as np
 
-from utils.general import colorstr, segment2box, resample_segments, check_version
-from utils.metrics import bbox_ioa
+from yolov5_sp.utils.general import colorstr, segment2box, resample_segments, check_version
+from yolov5_sp.utils.metrics import bbox_ioa
 
 
 class Albumentations:
     # YOLOv5 Albumentations class (optional, only used if package is installed)
     def __init__(self):
         self.transform = None
         try:
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/autoanchor.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/autoanchor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import random
 
 import numpy as np
 import torch
 import yaml
 from tqdm import tqdm
 
-from utils.general import colorstr
+from yolov5_sp.utils.general import colorstr
 
 
 def check_anchor_order(m):
     # Check anchor order against stride order for YOLOv5 Detect() module m, and correct if necessary
     a = m.anchors.prod(-1).view(-1)  # anchor area
     da = a[-1] - a[0]  # delta a
     ds = m.stride[-1] - m.stride[0]  # delta s
@@ -72,15 +72,15 @@
             gen: generations to evolve anchors using genetic algorithm
             verbose: print all results
 
         Return:
             k: kmeans evolved anchors
 
         Usage:
-            from utils.autoanchor import *; _ = kmean_anchors()
+            from yolov5_sp.utils.autoanchor import *; _ = kmean_anchors()
     """
     from scipy.cluster.vq import kmeans
 
     thr = 1. / thr
     prefix = colorstr('autoanchor: ')
 
     def metric(k, wh):  # compute metrics
@@ -103,15 +103,15 @@
         for i, x in enumerate(k):
             print('%i,%i' % (round(x[0]), round(x[1])), end=',  ' if i < len(k) - 1 else '\n')  # use in *.cfg
         return k
 
     if isinstance(dataset, str):  # *.yaml file
         with open(dataset, errors='ignore') as f:
             data_dict = yaml.safe_load(f)  # model dict
-        from utils.datasets import LoadImagesAndLabels
+        from yolov5_sp.utils.datasets import LoadImagesAndLabels
         dataset = LoadImagesAndLabels(data_dict['train'], augment=True, rect=True)
 
     # Get label wh
     shapes = img_size * dataset.shapes / dataset.shapes.max(1, keepdims=True)
     wh0 = np.concatenate([l[:, 3:5] * s for s, l in zip(shapes, dataset.labels)])  # wh
 
     # Filter
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/callbacks.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/datasets.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 import torch
 import torch.nn.functional as F
 import yaml
 from PIL import Image, ExifTags
 from torch.utils.data import Dataset
 from tqdm import tqdm
 
-from utils.augmentations import Albumentations, augment_hsv, copy_paste, letterbox, mixup, random_perspective
-from utils.general import check_dataset, check_requirements, check_yaml, clean_str, segments2boxes, \
+from yolov5_sp.utils.augmentations import Albumentations, augment_hsv, copy_paste, letterbox, mixup, random_perspective
+from yolov5_sp.utils.general import check_dataset, check_requirements, check_yaml, clean_str, segments2boxes, \
     xywh2xyxy, xywhn2xyxy, xyxy2xywhn, xyn2xy
-from utils.torch_utils import torch_distributed_zero_first
+from yolov5_sp.utils.torch_utils import torch_distributed_zero_first
 
 # Parameters
 HELP_URL = 'https://github.com/ultralytics/yolov5/wiki/Train-Custom-Data'
 IMG_FORMATS = ['bmp', 'jpg', 'jpeg', 'png', 'tif', 'tiff', 'dng', 'webp', 'mpo']  # acceptable image suffixes
 VID_FORMATS = ['mov', 'avi', 'mp4', 'mpg', 'mpeg', 'm4v', 'wmv', 'mkv']  # acceptable video suffixes
 NUM_THREADS = min(8, os.cpu_count())  # number of multiprocessing threads
 
@@ -809,15 +809,15 @@
     # Flatten a recursive directory by bringing all files to top level
     new_path = Path(path + '_flat')
     create_folder(new_path)
     for file in tqdm(glob.glob(str(Path(path)) + '/**/*.*', recursive=True)):
         shutil.copyfile(file, new_path / Path(file).name)
 
 
-def extract_boxes(path='../datasets/coco128'):  # from utils.datasets import *; extract_boxes()
+def extract_boxes(path='../datasets/coco128'):  # from yolov5_sp.utils.datasets import *; extract_boxes()
     # Convert detection dataset into classification dataset, with one directory per class
     path = Path(path)  # images dir
     shutil.rmtree(path / 'classifier') if (path / 'classifier').is_dir() else None  # remove existing
     files = list(path.rglob('*.*'))
     n = len(files)  # number of files
     for im_file in tqdm(files, total=n):
         if im_file.suffix[1:] in IMG_FORMATS:
@@ -845,15 +845,15 @@
                     b[[0, 2]] = np.clip(b[[0, 2]], 0, w)  # clip boxes outside of image
                     b[[1, 3]] = np.clip(b[[1, 3]], 0, h)
                     assert cv2.imwrite(str(f), im[b[1]:b[3], b[0]:b[2]]), f'box failure in {f}'
 
 
 def autosplit(path='../datasets/coco128/images', weights=(0.9, 0.1, 0.0), annotated_only=False):
     """ Autosplit a dataset into train/val/test splits and save path/autosplit_*.txt files
-    Usage: from utils.datasets import *; autosplit()
+    Usage: from yolov5_sp.utils.datasets import *; autosplit()
     Arguments
         path:            Path to images directory
         weights:         Train, val, test weights (list, tuple)
         annotated_only:  Only use images with an annotated txt file
     """
     path = Path(path)  # images dir
     files = sum([list(path.rglob(f"*.{img_ext}")) for img_ext in IMG_FORMATS], [])  # image files only
@@ -916,16 +916,16 @@
         msg = f'{prefix}WARNING: Ignoring corrupted image and/or label {im_file}: {e}'
         return [None, None, None, None, nm, nf, ne, nc, msg]
 
 
 def dataset_stats(path='coco128.yaml', autodownload=False, verbose=False, profile=False, hub=False):
     """ Return dataset statistics dictionary with images and instances counts per split per class
     To run in parent directory: export PYTHONPATH="$PWD/yolov5"
-    Usage1: from utils.datasets import *; dataset_stats('coco128.yaml', autodownload=True)
-    Usage2: from utils.datasets import *; dataset_stats('../datasets/coco128_with_yaml.zip')
+    Usage1: from yolov5_sp.utils.datasets import *; dataset_stats('coco128.yaml', autodownload=True)
+    Usage2: from yolov5_sp.utils.datasets import *; dataset_stats('../datasets/coco128_with_yaml.zip')
     Arguments
         path:           Path to data.yaml or data.zip (with data.yaml inside data.zip)
         autodownload:   Attempt to download dataset if not found locally
         verbose:        Print stats dictionary
     """
 
     def round_labels(labels):
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/downloads.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/downloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     finally:
         if not file.exists() or file.stat().st_size < min_bytes:  # check
             file.unlink(missing_ok=True)  # remove partial downloads
             print(f"ERROR: {assert_msg}\n{error_msg}")
         print('')
 
 
-def attempt_download(file, repo='ultralytics/yolov5'):  # from utils.downloads import *; attempt_download()
+def attempt_download(file, repo='ultralytics/yolov5'):  # from yolov5_sp.utils.downloads import *; attempt_download()
     # Attempt file download if does not exist
     file = Path(str(file).strip().replace("'", ''))
 
     if not file.exists():
         # URL specified
         name = Path(urllib.parse.unquote(str(file))).name  # decode '%2F' to '/' etc.
         if str(file).startswith(('http:/', 'https:/')):  # download
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/general.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 import numpy as np
 import pandas as pd
 import pkg_resources as pkg
 import torch
 import torchvision
 import yaml
 
-from utils.downloads import gsutil_getsize
-from utils.metrics import box_iou, fitness
+from yolov5_sp.utils.downloads import gsutil_getsize
+from yolov5_sp.utils.metrics import box_iou, fitness
 
 # Settings
 torch.set_printoptions(linewidth=320, precision=5, profile='long')
 np.set_printoptions(linewidth=320, formatter={'float_kind': '{:11.5g}'.format})  # format short g, %precision=5
 pd.options.display.max_columns = 10
 cv2.setNumThreads(0)  # prevent OpenCV from multithreading (incompatible with PyTorch DataLoader)
 os.environ['NUMEXPR_MAX_THREADS'] = str(min(os.cpu_count(), 8))  # NumExpr max threads
@@ -694,15 +694,15 @@
         if (time.time() - t) > time_limit:
             print(f'WARNING: NMS time limit {time_limit}s exceeded')
             break  # time limit exceeded
 
     return output
 
 
-def strip_optimizer(f='best.pt', s=''):  # from utils.general import *; strip_optimizer()
+def strip_optimizer(f='best.pt', s=''):  # from yolov5_sp.utils.general import *; strip_optimizer()
     # Strip optimizer from 'f' to finalize training, optionally save as 's'
     x = torch.load(f, map_location=torch.device('cpu'))
     if x.get('ema'):
         x['model'] = x['ema']  # replace model with ema
     for k in 'optimizer', 'training_results', 'wandb_id', 'ema', 'updates':  # keys
         x[k] = None
     x['epoch'] = -1
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/log.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/log.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/loss.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 """
 Loss functions
 """
 
 import torch
 import torch.nn as nn
 
-from utils.metrics import bbox_iou
-from utils.torch_utils import is_parallel
+from yolov5_sp.utils.metrics import bbox_iou
+from yolov5_sp.utils.torch_utils import is_parallel
 
 
 def smooth_BCE(eps=0.1):  # https://github.com/ultralytics/yolov3/issues/238#issuecomment-598028441
     # return positive, negative label smoothing BCE targets
     return 1.0 - 0.5 * eps, 0.5 * eps
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/metrics.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/plots.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sn
 import torch
 from PIL import Image, ImageDraw, ImageFont
 
-from utils.general import user_config_dir, is_ascii, is_chinese, xywh2xyxy, xyxy2xywh
-from utils.metrics import fitness
+from yolov5_sp.utils.general import user_config_dir, is_ascii, is_chinese, xywh2xyxy, xyxy2xywh
+from yolov5_sp.utils.metrics import fitness
 
 # Settings
 CONFIG_DIR = user_config_dir()  # Ultralytics settings dir
 RANK = int(os.getenv('RANK', -1))
 matplotlib.rc('font', **{'size': 11})
 matplotlib.use('Agg')  # for writing to files only
 
@@ -41,15 +41,15 @@
         return (c[2], c[1], c[0]) if bgr else c
 
     @staticmethod
     def hex2rgb(h):  # rgb order (PIL)
         return tuple(int(h[1 + i:1 + i + 2], 16) for i in (0, 2, 4))
 
 
-colors = Colors()  # create instance for 'from utils.plots import colors'
+colors = Colors()  # create instance for 'from yolov5_sp.utils.plots import colors'
 
 
 def check_font(font='Arial.ttf', size=10):
     # Return a PIL TrueType Font, downloading to CONFIG_DIR if necessary
     font = Path(font)
     font = font if font.exists() else (CONFIG_DIR / font.name)
     try:
@@ -222,15 +222,15 @@
     plt.grid()
     plt.xlim(0, epochs)
     plt.ylim(0)
     plt.savefig(Path(save_dir) / 'LR.png', dpi=200)
     plt.close()
 
 
-def plot_val_txt():  # from utils.plots import *; plot_val()
+def plot_val_txt():  # from yolov5_sp.utils.plots import *; plot_val()
     # Plot val.txt histograms
     x = np.loadtxt('val.txt', dtype=np.float32)
     box = xyxy2xywh(x[:, :4])
     cx, cy = box[:, 0], box[:, 1]
 
     fig, ax = plt.subplots(1, 1, figsize=(6, 6), tight_layout=True)
     ax.hist2d(cx, cy, bins=600, cmax=10, cmin=0)
@@ -239,28 +239,28 @@
 
     fig, ax = plt.subplots(1, 2, figsize=(12, 6), tight_layout=True)
     ax[0].hist(cx, bins=600)
     ax[1].hist(cy, bins=600)
     plt.savefig('hist1d.png', dpi=200)
 
 
-def plot_targets_txt():  # from utils.plots import *; plot_targets_txt()
+def plot_targets_txt():  # from yolov5_sp.utils.plots import *; plot_targets_txt()
     # Plot targets.txt histograms
     x = np.loadtxt('targets.txt', dtype=np.float32).T
     s = ['x targets', 'y targets', 'width targets', 'height targets']
     fig, ax = plt.subplots(2, 2, figsize=(8, 8), tight_layout=True)
     ax = ax.ravel()
     for i in range(4):
         ax[i].hist(x[i], bins=100, label='%.3g +/- %.3g' % (x[i].mean(), x[i].std()))
         ax[i].legend()
         ax[i].set_title(s[i])
     plt.savefig('targets.jpg', dpi=200)
 
 
-def plot_val_study(file='', dir='', x=None):  # from utils.plots import *; plot_val_study()
+def plot_val_study(file='', dir='', x=None):  # from yolov5_sp.utils.plots import *; plot_val_study()
     # Plot file=study.txt generated by val.py (or plot all study*.txt in dir)
     save_dir = Path(file).parent if file else Path(dir)
     plot2 = False  # plot additional results
     if plot2:
         ax = plt.subplots(2, 4, figsize=(10, 6), tight_layout=True)[1].ravel()
 
     fig2, ax2 = plt.subplots(1, 1, figsize=(8, 4), tight_layout=True)
@@ -334,15 +334,15 @@
 
     plt.savefig(save_dir / 'labels.jpg', dpi=200)
     matplotlib.use('Agg')
     plt.close()
 
 
 def profile_idetection(start=0, stop=0, labels=(), save_dir=''):
-    # Plot iDetection '*.txt' per-image logs. from utils.plots import *; profile_idetection()
+    # Plot iDetection '*.txt' per-image logs. from yolov5_sp.utils.plots import *; profile_idetection()
     ax = plt.subplots(2, 4, figsize=(12, 6), tight_layout=True)[1].ravel()
     s = ['Images', 'Free Storage (GB)', 'RAM Usage (GB)', 'Battery', 'dt_raw (ms)', 'dt_smooth (ms)', 'real-world FPS']
     files = list(Path(save_dir).glob('frames*.txt'))
     for fi, f in enumerate(files):
         try:
             results = np.loadtxt(f, ndmin=2).T[:, 90:-30]  # clip first and last rows
             n = results.shape[1]  # number of rows
@@ -364,15 +364,15 @@
                     a.remove()
         except Exception as e:
             print('Warning: Plotting error for %s; %s' % (f, e))
     ax[1].legend()
     plt.savefig(Path(save_dir) / 'idetection_profile.png', dpi=200)
 
 
-def plot_evolve(evolve_csv='path/to/evolve.csv'):  # from utils.plots import *; plot_evolve()
+def plot_evolve(evolve_csv='path/to/evolve.csv'):  # from yolov5_sp.utils.plots import *; plot_evolve()
     # Plot evolve.csv hyp evolution results
     evolve_csv = Path(evolve_csv)
     data = pd.read_csv(evolve_csv)
     keys = [x.strip() for x in data.columns]
     x = data.values
     f = fitness(x)
     j = np.argmax(f)  # max fitness index
@@ -391,15 +391,15 @@
     f = evolve_csv.with_suffix('.png')  # filename
     plt.savefig(f, dpi=200)
     plt.close()
     print(f'Saved {f}')
 
 
 def plot_results(file='path/to/results.csv', dir=''):
-    # Plot training results.csv. Usage: from utils.plots import *; plot_results('path/to/results.csv')
+    # Plot training results.csv. Usage: from yolov5_sp.utils.plots import *; plot_results('path/to/results.csv')
     save_dir = Path(file).parent if file else Path(dir)
     fig, ax = plt.subplots(2, 5, figsize=(12, 6), tight_layout=True)
     ax = ax.ravel()
     files = list(save_dir.glob('results*.csv'))
     assert len(files), f'No results.csv files found in {save_dir.resolve()}, nothing to plot.'
     for fi, f in enumerate(files):
         try:
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/resize_and_pad.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/resize_and_pad.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.1/yolov5_sp/utils/torch_utils.py` & `yolov5_sp-1.0.2/yolov5_sp/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5_sp-1.0.1/yolov5_sp/yolov5.py` & `yolov5_sp-1.0.2/yolov5_sp/yolov5.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import shutil
 
 import numpy as np
 import cv2
 import yaml
 import torch
-from models.experimental import attempt_load
-from utils.general import check_img_size,non_max_suppression,scale_coords
-from utils.datasets import letterbox
+from yolov5_sp.models.experimental import attempt_load
+from yolov5_sp.utils.general import check_img_size,non_max_suppression,scale_coords
+from yolov5_sp.utils.datasets import letterbox
 
 
 class YoloV5_Six:
     def __init__(self, model_dir):
         self.model_dir = model_dir
         self.__dict__ = self.parse_model_params(self.model_dir)
         cuda = torch.cuda.is_available()
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp.egg-info/PKG-INFO` & `yolov5_sp-1.0.2/yolov5_sp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5-sp
-Version: 1.0.1
+Version: 1.0.2
 Summary: yolov5-v5.0 general model
 Home-page: https://github.com/Easonshow
 Author: shaop
 Author-email: 13585800607@163.com
 Maintainer: shaop
 Maintainer-email: 13585800607@163.com
 License: MIT License
```

### Comparing `yolov5_sp-1.0.1/yolov5_sp.egg-info/SOURCES.txt` & `yolov5_sp-1.0.2/yolov5_sp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 yolov5_sp.egg-info/dependency_links.txt
 yolov5_sp.egg-info/entry_points.txt
 yolov5_sp.egg-info/requires.txt
 yolov5_sp.egg-info/top_level.txt
 yolov5_sp/models/__init__.py
 yolov5_sp/models/common.py
 yolov5_sp/models/experimental.py
+yolov5_sp/models/yolo.py
 yolov5_sp/utils/__init__.py
 yolov5_sp/utils/activations.py
 yolov5_sp/utils/augmentations.py
 yolov5_sp/utils/autoanchor.py
 yolov5_sp/utils/callbacks.py
 yolov5_sp/utils/datasets.py
 yolov5_sp/utils/downloads.py
```

