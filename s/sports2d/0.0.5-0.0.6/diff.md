# Comparing `tmp/sports2d-0.0.5.tar.gz` & `tmp/sports2d-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.0.5.tar", last modified: Thu May  4 09:35:09 2023, max compression
+gzip compressed data, was "sports2d-0.0.6.tar", last modified: Thu May  4 21:07:43 2023, max compression
```

## Comparing `sports2d-0.0.5.tar` & `sports2d-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.484331 sports2d-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-04 09:34:51.000000 sports2d-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-05-04 09:35:09.484331 sports2d-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-04 09:34:51.000000 sports2d-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.476331 sports2d-0.0.5/Sports2D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.476331 sports2d-0.0.5/Sports2D/Demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Demo/Config_demo.toml
--rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Demo/demo.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Sports2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.484331 sports2d-0.0.5/Sports2D/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/Blazepose_runsave.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/compute_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    21688 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/detect_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 09:34:51.000000 sports2d-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-04 09:35:09.484331 sports2d-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 09:34:51.000000 sports2d-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.484331 sports2d-0.0.5/sports2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:07:43.292979 sports2d-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-04 21:07:19.000000 sports2d-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-05-04 21:07:43.292979 sports2d-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-04 21:07:19.000000 sports2d-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:07:43.288979 sports2d-0.0.6/Sports2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:07:43.288979 sports2d-0.0.6/Sports2D/Demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/Demo/Config_demo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/Demo/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/Sports2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:07:43.292979 sports2d-0.0.6/Sports2D/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/Utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/Utilities/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/Utilities/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/Utilities/test_with_blazepose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/compute_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21697 2023-05-04 21:07:19.000000 sports2d-0.0.6/Sports2D/detect_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 21:07:19.000000 sports2d-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-04 21:07:43.292979 sports2d-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-04 21:07:19.000000 sports2d-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:07:43.292979 sports2d-0.0.6/sports2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-05-04 21:07:43.000000 sports2d-0.0.6/sports2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-04 21:07:43.000000 sports2d-0.0.6/sports2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:07:43.000000 sports2d-0.0.6/sports2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:07:43.000000 sports2d-0.0.6/sports2d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 21:07:43.000000 sports2d-0.0.6/sports2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 21:07:43.000000 sports2d-0.0.6/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.0.5/LICENSE` & `sports2d-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.5/PKG-INFO` & `sports2d-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.0.5
+Version: 0.0.6
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
-Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics
+Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
-Requires-Python: <=3.10
+Requires-Python: <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<!-- 
+
 [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
-[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D) \
-[![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
-[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
+[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)\
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+
+<!-- [![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
+[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
 [![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
+[![DOI](https://zenodo.org/badge/501642916.svg)](https://zenodo.org/badge/latestdoi/501642916)
 -->
 
 
 # Sports2D
 
 **`Sports2D` lets you compute 2D joint and segment angles from a single video.**
 
@@ -65,29 +67,30 @@
 3. [How to cite and how to contribute](#how-to-cite-and-how-to-contribute)
 
 
 ## Installation and Demonstration
 
 ### Installation
 
-- OPTION 1: **Quick install:** \
+- OPTION 1: **Quick install** \
     Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
     ```
     pip install sports2d
     ```
 
-- OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
+- OPTION 2: **Safer install with Anaconda**\
+    Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):\
     Open an Anaconda prompt and create a virtual environment by typing:
     ```
     conda create -n Sports2D python<=3.10 
     conda activate Sports2D
     pip install sports2d
     ```
 
-- OPTION 3: **Build from source and test the last changes:**\
+- OPTION 3: **Build from source and test the last changes**\
      Open a terminal in the directory of your choice and clone the Sports2D repository.
      ```
      git clone https://github.com/davidpagnon/sports2d.git
      cd sports2d
      pip install .
      ```
 
@@ -151,15 +154,15 @@
 
 3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
 
 *N.B.:* If you want to benefit from the capabilities of OpenPose but do not manage to install it, you can use the `Colab notebook` version.\
 Note that your data will be sent to the Google servers, which do not follow the European GDPR requirements regarding privacy.
 **COMING SOON**
 
-<img src="Content/demo_blazepose_results.png" width="760">
+<img src="Content/demo_openpose_results.png" width="760">
 
 ### Advanced settings
 
 1. `Config_demo.toml` → `pose_advanced`: These settings are only taken into account if OpenPose is used.
    1. `load_pose`: If you need to change some settings but have already run a pose estimation, you can set this to `true` in order to not regenerate the json pose files.
 
    2. `save_vid` and `save_img`: You can choose whether you want to save the resulting video and images. If set to `false`, only pose and angle `.csv` files will be generated.
@@ -223,16 +226,16 @@
 ## How to cite and how to contribute
 
 ### How to cite
 If you use this code or data, please cite [Pagnon, 2023].
 
      @misc{Pagnon2023,
        author = {Pagnon, David},
-       title = {Sports2D - Angles from monocular video},
-       year = {2013},
+       title = {Sports2D - Angles from video},
+       year = {2023},
        publisher = {GitHub},
        journal = {GitHub repository},
        howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
      }
 
 ### How to contribute
 I would happily welcome any proposal for new features, code improvement, and more!\
```

### Comparing `sports2d-0.0.5/README.md` & `sports2d-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-<!-- 
+
 [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
-[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D) \
-[![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
-[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
+[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)\
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+
+<!-- [![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
+[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
 [![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
+[![DOI](https://zenodo.org/badge/501642916.svg)](https://zenodo.org/badge/latestdoi/501642916)
 -->
 
 
 # Sports2D
 
 **`Sports2D` lets you compute 2D joint and segment angles from a single video.**
 
@@ -38,29 +40,30 @@
 3. [How to cite and how to contribute](#how-to-cite-and-how-to-contribute)
 
 
 ## Installation and Demonstration
 
 ### Installation
 
-- OPTION 1: **Quick install:** \
+- OPTION 1: **Quick install** \
     Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
     ```
     pip install sports2d
     ```
 
-- OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
+- OPTION 2: **Safer install with Anaconda**\
+    Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):\
     Open an Anaconda prompt and create a virtual environment by typing:
     ```
     conda create -n Sports2D python<=3.10 
     conda activate Sports2D
     pip install sports2d
     ```
 
-- OPTION 3: **Build from source and test the last changes:**\
+- OPTION 3: **Build from source and test the last changes**\
      Open a terminal in the directory of your choice and clone the Sports2D repository.
      ```
      git clone https://github.com/davidpagnon/sports2d.git
      cd sports2d
      pip install .
      ```
 
@@ -124,15 +127,15 @@
 
 3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
 
 *N.B.:* If you want to benefit from the capabilities of OpenPose but do not manage to install it, you can use the `Colab notebook` version.\
 Note that your data will be sent to the Google servers, which do not follow the European GDPR requirements regarding privacy.
 **COMING SOON**
 
-<img src="Content/demo_blazepose_results.png" width="760">
+<img src="Content/demo_openpose_results.png" width="760">
 
 ### Advanced settings
 
 1. `Config_demo.toml` → `pose_advanced`: These settings are only taken into account if OpenPose is used.
    1. `load_pose`: If you need to change some settings but have already run a pose estimation, you can set this to `true` in order to not regenerate the json pose files.
 
    2. `save_vid` and `save_img`: You can choose whether you want to save the resulting video and images. If set to `false`, only pose and angle `.csv` files will be generated.
@@ -196,16 +199,16 @@
 ## How to cite and how to contribute
 
 ### How to cite
 If you use this code or data, please cite [Pagnon, 2023].
 
      @misc{Pagnon2023,
        author = {Pagnon, David},
-       title = {Sports2D - Angles from monocular video},
-       year = {2013},
+       title = {Sports2D - Angles from video},
+       year = {2023},
        publisher = {GitHub},
        journal = {GitHub repository},
        howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
      }
 
 ### How to contribute
 I would happily welcome any proposal for new features, code improvement, and more!\
```

### Comparing `sports2d-0.0.5/Sports2D/Demo/Config_demo.toml` & `sports2d-0.0.6/Sports2D/Demo/Config_demo.toml`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.5/Sports2D/Demo/demo.mp4` & `sports2d-0.0.6/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.5/Sports2D/Sports2D.py` & `sports2d-0.0.6/Sports2D/Sports2D.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.5/Sports2D/Utilities/Blazepose_runsave.py` & `sports2d-0.0.6/Sports2D/Utilities/Blazepose_runsave.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.5/Sports2D/Utilities/common.py` & `sports2d-0.0.6/Sports2D/Utilities/common.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.5/Sports2D/Utilities/filter.py` & `sports2d-0.0.6/Sports2D/Utilities/filter.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.5/Sports2D/Utilities/skeletons.py` & `sports2d-0.0.6/Sports2D/Utilities/skeletons.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.5/Sports2D/compute_angles.py` & `sports2d-0.0.6/Sports2D/compute_angles.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.5/Sports2D/detect_pose.py` & `sports2d-0.0.6/Sports2D/detect_pose.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,14 @@
 import subprocess
 import itertools as it
 import numpy as np
 import pandas as pd
 import cv2
 import matplotlib.pyplot as plt
 import matplotlib as mpl
-mpl.use('qt5agg')
-mpl.rc('figure', max_open_warning=0)
 from Sports2D.Sports2D import base_params
 from Sports2D.Utilities import Blazepose_runsave, filter, common
 from Sports2D.Utilities.skeletons import *
 
 
 ## AUTHORSHIP INFORMATION
 __author__ = "David Pagnon"
@@ -78,14 +76,17 @@
     INPUTS:
     - df_list: list of dataframes of 3N columns, only 3i and 3i+1 are displayed
 
     OUTPUT:
     - matplotlib window with tabbed figures for each keypoint
     '''
     
+    mpl.use('qt5agg')
+    mpl.rc('figure', max_open_warning=0)
+
     keypoints_names = df_list[0].columns.get_level_values(2)[1::3]
     
     pw = common.plotWindow()
     for id, keypoint in enumerate(keypoints_names):
         f = plt.figure()
         
         axX = plt.subplot(211)
```

### Comparing `sports2d-0.0.5/setup.cfg` & `sports2d-0.0.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = sports2d
-version = 0.0.5
+version = 0.0.6
 author = David Pagnon
 author_email = contact@david-pagnon.com
 description = Detect pose and compute 2D joint angles from a video.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/davidpagnon/Sports2D
-keywords = markerless, kinematics, OpenPose, BlazePose, joint angles, 2D, biomechanics
+keywords = markerless, kinematics, OpenPose, BlazePose, joint angles, 2D, biomechanics, sports, sports-analytics
 license = BSD 3-Clause License
 license_files = LICENSE
 platform = any
 classifiers = 
 	Programming Language :: Python :: 3
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
@@ -25,15 +25,15 @@
 	Topic :: Multimedia :: Graphics
 	Topic :: Multimedia :: Graphics :: 3D Modeling
 project_urls = 
 	Bug Tracker = https://github.com/davidpagnon/Sports2D/issues
 
 [options]
 zip_safe = False
-python_requires = <=3.10
+python_requires = <3.11
 install_requires = 
 	ipython
 	toml
 	numpy
 	pandas>=1.5
 	scipy
 	anytree
```

### Comparing `sports2d-0.0.5/sports2d.egg-info/PKG-INFO` & `sports2d-0.0.6/sports2d.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.0.5
+Version: 0.0.6
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
-Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics
+Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
-Requires-Python: <=3.10
+Requires-Python: <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<!-- 
+
 [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
-[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D) \
-[![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
-[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
+[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)\
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+
+<!-- [![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
+[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
 [![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
+[![DOI](https://zenodo.org/badge/501642916.svg)](https://zenodo.org/badge/latestdoi/501642916)
 -->
 
 
 # Sports2D
 
 **`Sports2D` lets you compute 2D joint and segment angles from a single video.**
 
@@ -65,29 +67,30 @@
 3. [How to cite and how to contribute](#how-to-cite-and-how-to-contribute)
 
 
 ## Installation and Demonstration
 
 ### Installation
 
-- OPTION 1: **Quick install:** \
+- OPTION 1: **Quick install** \
     Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
     ```
     pip install sports2d
     ```
 
-- OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
+- OPTION 2: **Safer install with Anaconda**\
+    Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):\
     Open an Anaconda prompt and create a virtual environment by typing:
     ```
     conda create -n Sports2D python<=3.10 
     conda activate Sports2D
     pip install sports2d
     ```
 
-- OPTION 3: **Build from source and test the last changes:**\
+- OPTION 3: **Build from source and test the last changes**\
      Open a terminal in the directory of your choice and clone the Sports2D repository.
      ```
      git clone https://github.com/davidpagnon/sports2d.git
      cd sports2d
      pip install .
      ```
 
@@ -151,15 +154,15 @@
 
 3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
 
 *N.B.:* If you want to benefit from the capabilities of OpenPose but do not manage to install it, you can use the `Colab notebook` version.\
 Note that your data will be sent to the Google servers, which do not follow the European GDPR requirements regarding privacy.
 **COMING SOON**
 
-<img src="Content/demo_blazepose_results.png" width="760">
+<img src="Content/demo_openpose_results.png" width="760">
 
 ### Advanced settings
 
 1. `Config_demo.toml` → `pose_advanced`: These settings are only taken into account if OpenPose is used.
    1. `load_pose`: If you need to change some settings but have already run a pose estimation, you can set this to `true` in order to not regenerate the json pose files.
 
    2. `save_vid` and `save_img`: You can choose whether you want to save the resulting video and images. If set to `false`, only pose and angle `.csv` files will be generated.
@@ -223,16 +226,16 @@
 ## How to cite and how to contribute
 
 ### How to cite
 If you use this code or data, please cite [Pagnon, 2023].
 
      @misc{Pagnon2023,
        author = {Pagnon, David},
-       title = {Sports2D - Angles from monocular video},
-       year = {2013},
+       title = {Sports2D - Angles from video},
+       year = {2023},
        publisher = {GitHub},
        journal = {GitHub repository},
        howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
      }
 
 ### How to contribute
 I would happily welcome any proposal for new features, code improvement, and more!\
```

### Comparing `sports2d-0.0.5/sports2d.egg-info/SOURCES.txt` & `sports2d-0.0.6/sports2d.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 Sports2D/Demo/Config_demo.toml
 Sports2D/Demo/demo.mp4
 Sports2D/Utilities/Blazepose_runsave.py
 Sports2D/Utilities/__init__.py
 Sports2D/Utilities/common.py
 Sports2D/Utilities/filter.py
 Sports2D/Utilities/skeletons.py
+Sports2D/Utilities/test_with_blazepose.py
 sports2d.egg-info/PKG-INFO
 sports2d.egg-info/SOURCES.txt
 sports2d.egg-info/dependency_links.txt
 sports2d.egg-info/not-zip-safe
 sports2d.egg-info/requires.txt
 sports2d.egg-info/top_level.txt
```

