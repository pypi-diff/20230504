# Comparing `tmp/sports2d-0.0.2.tar.gz` & `tmp/sports2d-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.0.2.tar", last modified: Wed May  3 23:15:54 2023, max compression
+gzip compressed data, was "sports2d-0.0.5.tar", last modified: Thu May  4 09:35:09 2023, max compression
```

## Comparing `sports2d-0.0.2.tar` & `sports2d-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.842070 sports2d-0.0.2/
--rw-rw-rw-   0        0        0     1550 2023-02-05 04:03:13.000000 sports2d-0.0.2/LICENSE
--rw-rw-rw-   0        0        0    14167 2023-05-03 23:15:54.842070 sports2d-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    11462 2023-05-03 23:15:23.000000 sports2d-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.791592 sports2d-0.0.2/Sports2D/
-drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.791592 sports2d-0.0.2/Sports2D/Demo/
--rw-rw-rw-   0        0        0     3120 2023-05-03 22:48:24.000000 sports2d-0.0.2/Sports2D/Demo/Config_demo.toml
--rw-rw-rw-   0        0        0  2539508 2023-05-02 13:57:16.000000 sports2d-0.0.2/Sports2D/Demo/demo.mp4
--rw-rw-rw-   0        0        0     7515 2023-05-02 14:06:35.000000 sports2d-0.0.2/Sports2D/Sports2D.py
-drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.809572 sports2d-0.0.2/Sports2D/Utilities/
--rw-rw-rw-   0        0        0    11135 2023-05-02 00:51:53.000000 sports2d-0.0.2/Sports2D/Utilities/Blazepose_runsave.py
--rw-rw-rw-   0        0        0      108 2023-04-06 11:56:03.000000 sports2d-0.0.2/Sports2D/Utilities/__init__.py
--rw-rw-rw-   0        0        0     4511 2023-05-01 19:27:34.000000 sports2d-0.0.2/Sports2D/Utilities/common.py
--rw-rw-rw-   0        0        0     5086 2023-04-28 13:37:20.000000 sports2d-0.0.2/Sports2D/Utilities/filter.py
--rw-rw-rw-   0        0        0    15791 2023-04-28 13:24:23.000000 sports2d-0.0.2/Sports2D/Utilities/skeletons.py
--rw-rw-rw-   0        0        0      110 2023-05-03 22:57:13.000000 sports2d-0.0.2/Sports2D/__init__.py
--rw-rw-rw-   0        0        0    22160 2023-05-03 22:48:13.000000 sports2d-0.0.2/Sports2D/compute_angles.py
--rw-rw-rw-   0        0        0    22224 2023-05-02 13:41:54.000000 sports2d-0.0.2/Sports2D/detect_pose.py
--rw-rw-rw-   0        0        0      113 2023-02-05 04:03:13.000000 sports2d-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1386 2023-05-03 23:15:54.848069 sports2d-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-02-05 04:03:13.000000 sports2d-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.841069 sports2d-0.0.2/sports2d.egg-info/
--rw-rw-rw-   0        0        0    14167 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       98 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.484331 sports2d-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-04 09:34:51.000000 sports2d-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-05-04 09:35:09.484331 sports2d-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-04 09:34:51.000000 sports2d-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.476331 sports2d-0.0.5/Sports2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.476331 sports2d-0.0.5/Sports2D/Demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Demo/Config_demo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Demo/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Sports2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.484331 sports2d-0.0.5/Sports2D/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/Utilities/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/compute_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21688 2023-05-04 09:34:51.000000 sports2d-0.0.5/Sports2D/detect_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 09:34:51.000000 sports2d-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-04 09:35:09.484331 sports2d-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 09:34:51.000000 sports2d-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:35:09.484331 sports2d-0.0.5/sports2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 09:35:09.000000 sports2d-0.0.5/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.0.2/LICENSE` & `sports2d-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, perfanalytics
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, perfanalytics
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sports2d-0.0.2/PKG-INFO` & `sports2d-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,274 +1,275 @@
-Metadata-Version: 2.1
-Name: sports2d
-Version: 0.0.2
-Summary: Detect pose and compute 2D joint angles from a video.
-Home-page: https://github.com/davidpagnon/Sports2D
-Author: David Pagnon
-Author-email: contact@david-pagnon.com
-License: BSD 3-Clause License
-Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
-Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
-Requires-Python: <=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<!-- 
-[![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
-[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D) \
-[![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
-[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
-[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
-[![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
--->
-
-
-# Sports2D
-
-**`Sports2D` lets you compute 2D joint and segment angles from a single video.**
-
- </br>
- </br>
-
-<img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
-
-`Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
-`Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
-If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.
-
-`Announcement:` Apps with GUI will be released for Windows, Linux, MacOS, as well as Android and iOS.
-Mobile versions will only support simple exploratory analysis. This involves single-person angle computation, in a potentially less accurate and tunable way.
-
-
-## Contents
-1. [Installation and Demonstration](#installation-and-demonstration)
-   1. [Installation](#installation)
-   2. [Demonstration: Detect pose and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles)
-2. [Go further](#go-further)
-   1. [Use on your own videos](#use-on-your-own-videos)
-   2. [Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-multi-person-more-accurate-analysis)
-   3. [Advanced-settings](#advanced-settings)
-   4. [How it works](#how-it-works)
-3. [How to cite and how to contribute](#how-to-cite-and-how-to-contribute)
-
-
-## Installation and Demonstration
-
-### Installation
-
-- OPTION 1: **Quick install:** \
-    Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
-    ```
-    pip install sports2d
-    ```
-
-- OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
-    Open an Anaconda prompt and create a virtual environment by typing:
-    ```
-    conda create -n Sports2D python<=3.10 
-    conda activate Sports2D
-    pip install sports2d
-    ```
-
-- OPTION 3: **Build from source and test the last changes:**\
-     Open a terminal in the directory of your choice and clone the Sports2D repository.
-     ```
-     git clone https://github.com/davidpagnon/sports2d.git
-     cd sports2d
-     pip install .
-     ```
-
-
-### Demonstration: Detect pose and compute 2D angles
-
-Open a terminal, enter `pip show sports2d`, check sports2d package location. \
-Copy this path and go to the Demo folder by typing `cd <path>\Sports2D\Demo`. \
-Type `ipython`, and test the following code:
-```
-from Sports2D import Sports2D
-Sports2D.detect_pose('Config_demo.toml')
-Sports2D.compute_angles('Config_demo.toml')
-```
-
-<img src="Content/demo_blazepose_terminal.png" width="760">
-
-
-You should obtain a video with the overlaid 2D joint positions, and angle text values. This output is also provided as an image folder.\
-You should additionally obtain the same information as time series, stored in .csv files. These files can be opened with any spreadsheet software, or with the Pandas Python library for example.\
-In addition, you will get the original OpenPose-like json coordinates files.
-
-<img src="Content/demo_blazepose_results.png" width="760">
-
-
-## Go further
-
-### Use on your own videos
-
-1. Copy-paste `Config_demo.toml` in the directory of your video.
-
-2. Open it with any text editor.\
-Replace the `video_file` value with the name of your video.
-
-3. Open a terminal or an Anaconda prompt, type:
-   ```
-   cd <Path/to/video/directory>
-   conda activate Sports2D (skip if you did not install with Anaconda)
-   ipython
-   ```
-   ```
-   from Sports2D import Sports2D
-   Sports2D.detect_pose('Config_demo.toml')
-   Sports2D.compute_angles('Config_demo.toml')
-   ```
-
-*Optionally:* If your video is not in the same folder as `Config_demo.toml`, specify its location in `video_dir`.\
-Similarly, if you launch Sports2D in an other directory, specify the location of the config file this way: `Sports2D.detect_pose(<path_to_Config_demo.toml>)`\
-In `pose`, specify the use of BlazePose or OpenPose as joint detectors: this will be detailed in the next section.\
-In `compute_angles`, select your angles of interest.
-
-
-### Use OpenPose for multi-person, more accurate analysis
-
-OpenPose is slower than OpenPose, but more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
-
-1. **Install OpenPose** (instructions [there](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md)). \
-*Windows portable demo works fine.*
-
-2. If you want even more accurate results, use the BODY_25B experimental model instead of the standard BODY_25 one. This requires manually [downloading the model](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md). You can optionally download from there the BODY_135 model which will let you compute wrist flexion and hand segment angle, however this will be much slower.
-
-3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
-
-*N.B.:* If you want to benefit from the capabilities of OpenPose but do not manage to install it, you can use the `Colab notebook` version.\
-Note that your data will be sent to the Google servers, which do not follow the European GDPR requirements regarding privacy.
-**COMING SOON**
-
-
-### Advanced settings
-
-1. `Config_demo.toml` → `pose_advanced`: These settings are only taken into account if OpenPose is used.
-   1. `load_pose`: If you need to change some settings but have already run a pose estimation, you can set this to `true` in order to not regenerate the json pose files.
-
-   2. `save_vid` and `save_img`: You can choose whether you want to save the resulting video and images. If set to `false`, only pose and angle `.csv` files will be generated.
-
-   3. `interp_gap_smaller_than`: Gaps are interpolated only if they are not too wide.
-   
-   4. `filter`: `true` or `false`. If `true`, you can choose among `Butterworth`, `Gaussian`, `LOESS`, or `Median`, and specify their parameters.\
-   Beware that the appearance of the unfiltered skeleton may not match the filtered coordinates and angles.
-
-   5. `show_plots`: Displays a window with tabs corresponding to the coordinates of each detected point. This may cause Python to crash.
-
-2. `Config_demo.toml` → `compute_angles_advanced`: These settings are taken into account both with BlazePose and OpenPose.
-   1. `save_vid` and `save_img`: Cf `pose_advanced`.
-
-   2. `filter`: Cf `pose_advanced`.
-
-   3. `show_plots`: Cf `pose_advanced`.
-
-   <img src="Content/demo_show_plots.png" width="760">
-
-*N.B.:* The settings and results of all analyses are stored int the `logs.txt` file, which can be found in in the sports2d installation folder (`pip show sports2d` to find the path).
-
-
-
-### How it works
-
-#### Pose detection:
-
-BlazePose or OpenPose are used to detect joint centers from a video.
-
-If `BlazePose` is used, only one person can be detected.\
-No interpolation nor filtering options are available. Not plotting available.
-
-If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
-Sequences of missing data are interpolated if they are less than N frames long.\
-Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
-
-
-#### Angle computation:
-
-Joint and segment angles are computed from csv position files.\
-If a person suddently faces the other way, this change of direction is taken into account.\
-Resulting angles can be filtered in the same way as point coordinates, and they can also be plotted.
-
-**Joint angle conventions:**
-- Ankle dorsiflexion: Between heel and big toe, and ankle and knee
-- Knee flexion: Between hip, knee, and ankle 
-- Hip flexion: Between knee, hip, and shoulder
-- Shoulder flexion: Between hip, shoulder, and elbow
-- Elbow flexion: Between wrist, elbow, and shoulder
-
-**Segment angle conventions:**\
-Angles are measured anticlockwise between the horizontal and the segment.
-- Foot: Between heel and big toe
-- Shank: Between knee and ankle
-- Thigh: Between hip and knee
-- Arm: Between shoulder and elbow
-- Forearm: Between elbow and wrist
-- Trunk: Between shoulder midpoint and hip midpoint
-
-## How to cite and how to contribute
-
-### How to cite
-If you use this code or data, please cite [Pagnon, 2023].
-
-     @misc{Pagnon2023,
-       author = {Pagnon, David},
-       title = {Sports2D - Angles from monocular video},
-       year = {2013},
-       publisher = {GitHub},
-       journal = {GitHub repository},
-       howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
-     }
-
-### How to contribute
-I would happily welcome any proposal for new features, code improvement, and more!\
-If you want to contribute to Sports2D, please follow [this guide](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to fork, modify and push code, and submit a pull request. I would appreciate it if you provided as much useful information as possible about how you modified the code, and a rationale for why you're making this pull request. Please also specify on which operating system and on which python version you have tested the code.
-
-*Here is a to-do list, for general guidance purposes only:*
-> <li> <b>GUI applications:</b> For Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with <a href="https://kivy.org">Kivy</a>.</li>
-> <li> <b>Pose refinement:</b> Click and move badly estimated 2D points. See <a href="https://www.youtube.com/watch?v=bEuBKB7eqmk">DeepLabCut</a> for inspiration.
-> <li> <b>Include OpenPose in Sports2D:</b> For example, <a href="https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile">Dockerize</a> it. Otherwise, run Sports2D in a <a href="https://colab.research.google.com/github/hardik0/AI-basketball-analysis-on-google-colab/blob/master/AI_basketball_analysis_google_colab.ipynb">Colab notebook</a>.
-> <li> <b>Constrain points</b> to OpenSim skeletal model for better angle estimation. Cf <a href="https://github.com/perfanalytics/pose2sim">Pose2Sim</a>, but in 2D.
-
-BSD 3-Clause License
-
-Copyright (c) 2022, perfanalytics
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Metadata-Version: 2.1
+Name: sports2d
+Version: 0.0.5
+Summary: Detect pose and compute 2D joint angles from a video.
+Home-page: https://github.com/davidpagnon/Sports2D
+Author: David Pagnon
+Author-email: contact@david-pagnon.com
+License: BSD 3-Clause License
+Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
+Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
+Requires-Python: <=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<!-- 
+[![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
+[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D) \
+[![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
+[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
+[![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
+-->
+
+
+# Sports2D
+
+**`Sports2D` lets you compute 2D joint and segment angles from a single video.**
+
+ </br>
+ </br>
+
+<img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
+
+`Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
+`Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
+If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.
+
+`Announcement:` Apps with GUI will be released for Windows, Linux, MacOS, as well as Android and iOS.
+Mobile versions will only support simple exploratory analysis. This involves single-person angle computation, in a potentially less accurate and tunable way.
+
+
+## Contents
+1. [Installation and Demonstration](#installation-and-demonstration)
+   1. [Installation](#installation)
+   2. [Demonstration: Detect pose and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles)
+2. [Go further](#go-further)
+   1. [Use on your own videos](#use-on-your-own-videos)
+   2. [Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-multi-person-more-accurate-analysis)
+   3. [Advanced-settings](#advanced-settings)
+   4. [How it works](#how-it-works)
+3. [How to cite and how to contribute](#how-to-cite-and-how-to-contribute)
+
+
+## Installation and Demonstration
+
+### Installation
+
+- OPTION 1: **Quick install:** \
+    Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
+    ```
+    pip install sports2d
+    ```
+
+- OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
+    Open an Anaconda prompt and create a virtual environment by typing:
+    ```
+    conda create -n Sports2D python<=3.10 
+    conda activate Sports2D
+    pip install sports2d
+    ```
+
+- OPTION 3: **Build from source and test the last changes:**\
+     Open a terminal in the directory of your choice and clone the Sports2D repository.
+     ```
+     git clone https://github.com/davidpagnon/sports2d.git
+     cd sports2d
+     pip install .
+     ```
+
+
+### Demonstration: Detect pose and compute 2D angles
+
+Open a terminal, enter `pip show sports2d`, check sports2d package location. \
+Copy this path and go to the Demo folder by typing `cd <path>\Sports2D\Demo`. \
+Type `ipython`, and test the following code:
+```
+from Sports2D import Sports2D
+Sports2D.detect_pose('Config_demo.toml')
+Sports2D.compute_angles('Config_demo.toml')
+```
+
+<img src="Content/demo_blazepose_terminal.png" width="760">
+
+
+You should obtain a video with the overlaid 2D joint positions, and angle text values. This output is also provided as an image folder.\
+You should additionally obtain the same information as time series, stored in .csv files. These files can be opened with any spreadsheet software, or with the Pandas Python library for example.\
+In addition, you will get the original OpenPose-like json coordinates files.
+
+<img src="Content/demo_blazepose_results.png" width="760">
+
+
+## Go further
+
+### Use on your own videos
+
+1. Copy-paste `Config_demo.toml` in the directory of your video.
+
+2. Open it with any text editor.\
+Replace the `video_file` value with the name of your video.
+
+3. Open a terminal or an Anaconda prompt, type:
+   ```
+   cd <Path/to/video/directory>
+   conda activate Sports2D (skip if you did not install with Anaconda)
+   ipython
+   ```
+   ```
+   from Sports2D import Sports2D
+   Sports2D.detect_pose('Config_demo.toml')
+   Sports2D.compute_angles('Config_demo.toml')
+   ```
+
+*Optionally:* If your video is not in the same folder as `Config_demo.toml`, specify its location in `video_dir`.\
+Similarly, if you launch Sports2D in an other directory, specify the location of the config file this way: `Sports2D.detect_pose(<path_to_Config_demo.toml>)`\
+In `pose`, specify the use of BlazePose or OpenPose as joint detectors: this will be detailed in the next section.\
+In `compute_angles`, select your angles of interest.
+
+
+### Use OpenPose for multi-person, more accurate analysis
+
+OpenPose is slower than OpenPose, but more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
+
+1. **Install OpenPose** (instructions [there](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md)). \
+*Windows portable demo works fine.*
+
+2. If you want even more accurate results, use the BODY_25B experimental model instead of the standard BODY_25 one. This requires manually [downloading the model](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md). You can optionally download from there the BODY_135 model which will let you compute wrist flexion and hand segment angle, however this will be much slower.
+
+3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
+
+*N.B.:* If you want to benefit from the capabilities of OpenPose but do not manage to install it, you can use the `Colab notebook` version.\
+Note that your data will be sent to the Google servers, which do not follow the European GDPR requirements regarding privacy.
+**COMING SOON**
+
+<img src="Content/demo_blazepose_results.png" width="760">
+
+### Advanced settings
+
+1. `Config_demo.toml` → `pose_advanced`: These settings are only taken into account if OpenPose is used.
+   1. `load_pose`: If you need to change some settings but have already run a pose estimation, you can set this to `true` in order to not regenerate the json pose files.
+
+   2. `save_vid` and `save_img`: You can choose whether you want to save the resulting video and images. If set to `false`, only pose and angle `.csv` files will be generated.
+
+   3. `interp_gap_smaller_than`: Gaps are interpolated only if they are not too wide.
+   
+   4. `filter`: `true` or `false`. If `true`, you can choose among `Butterworth`, `Gaussian`, `LOESS`, or `Median`, and specify their parameters.\
+   Beware that the appearance of the unfiltered skeleton may not match the filtered coordinates and angles.
+
+   5. `show_plots`: Displays a window with tabs corresponding to the coordinates of each detected point. This may cause Python to crash.
+
+2. `Config_demo.toml` → `compute_angles_advanced`: These settings are taken into account both with BlazePose and OpenPose.
+   1. `save_vid` and `save_img`: Cf `pose_advanced`.
+
+   2. `filter`: Cf `pose_advanced`.
+
+   3. `show_plots`: Cf `pose_advanced`.
+
+   <img src="Content/demo_show_plots.png" width="760">
+
+*N.B.:* The settings and results of all analyses are stored int the `logs.txt` file, which can be found in in the sports2d installation folder (`pip show sports2d` to find the path).
+
+
+
+### How it works
+
+#### Pose detection:
+
+BlazePose or OpenPose are used to detect joint centers from a video.
+
+If `BlazePose` is used, only one person can be detected.\
+No interpolation nor filtering options are available. Not plotting available.
+
+If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
+Sequences of missing data are interpolated if they are less than N frames long.\
+Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
+
+
+#### Angle computation:
+
+Joint and segment angles are computed from csv position files.\
+If a person suddently faces the other way, this change of direction is taken into account.\
+Resulting angles can be filtered in the same way as point coordinates, and they can also be plotted.
+
+**Joint angle conventions:**
+- Ankle dorsiflexion: Between heel and big toe, and ankle and knee
+- Knee flexion: Between hip, knee, and ankle 
+- Hip flexion: Between knee, hip, and shoulder
+- Shoulder flexion: Between hip, shoulder, and elbow
+- Elbow flexion: Between wrist, elbow, and shoulder
+
+**Segment angle conventions:**\
+Angles are measured anticlockwise between the horizontal and the segment.
+- Foot: Between heel and big toe
+- Shank: Between knee and ankle
+- Thigh: Between hip and knee
+- Arm: Between shoulder and elbow
+- Forearm: Between elbow and wrist
+- Trunk: Between shoulder midpoint and hip midpoint
+
+## How to cite and how to contribute
+
+### How to cite
+If you use this code or data, please cite [Pagnon, 2023].
+
+     @misc{Pagnon2023,
+       author = {Pagnon, David},
+       title = {Sports2D - Angles from monocular video},
+       year = {2013},
+       publisher = {GitHub},
+       journal = {GitHub repository},
+       howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
+     }
+
+### How to contribute
+I would happily welcome any proposal for new features, code improvement, and more!\
+If you want to contribute to Sports2D, please follow [this guide](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to fork, modify and push code, and submit a pull request. I would appreciate it if you provided as much useful information as possible about how you modified the code, and a rationale for why you're making this pull request. Please also specify on which operating system and on which python version you have tested the code.
+
+*Here is a to-do list, for general guidance purposes only:*
+> <li> <b>GUI applications:</b> For Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with <a href="https://kivy.org">Kivy</a>.</li>
+> <li> <b>Pose refinement:</b> Click and move badly estimated 2D points. See <a href="https://www.youtube.com/watch?v=bEuBKB7eqmk">DeepLabCut</a> for inspiration.
+> <li> <b>Include OpenPose in Sports2D:</b> For example, <a href="https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile">Dockerize</a> it. Otherwise, run Sports2D in a <a href="https://colab.research.google.com/github/hardik0/AI-basketball-analysis-on-google-colab/blob/master/AI_basketball_analysis_google_colab.ipynb">Colab notebook</a>.
+> <li> <b>Constrain points</b> to OpenSim skeletal model for better angle estimation. Cf <a href="https://github.com/perfanalytics/pose2sim">Pose2Sim</a>, but in 2D.
+
+BSD 3-Clause License
+
+Copyright (c) 2022, perfanalytics
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sports2d-0.0.2/README.md` & `sports2d-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,217 +1,218 @@
-<!-- 
-[![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
-[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D) \
-[![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
-[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
-[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
-[![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
--->
-
-
-# Sports2D
-
-**`Sports2D` lets you compute 2D joint and segment angles from a single video.**
-
- </br>
- </br>
-
-<img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
-
-`Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
-`Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
-If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.
-
-`Announcement:` Apps with GUI will be released for Windows, Linux, MacOS, as well as Android and iOS.
-Mobile versions will only support simple exploratory analysis. This involves single-person angle computation, in a potentially less accurate and tunable way.
-
-
-## Contents
-1. [Installation and Demonstration](#installation-and-demonstration)
-   1. [Installation](#installation)
-   2. [Demonstration: Detect pose and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles)
-2. [Go further](#go-further)
-   1. [Use on your own videos](#use-on-your-own-videos)
-   2. [Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-multi-person-more-accurate-analysis)
-   3. [Advanced-settings](#advanced-settings)
-   4. [How it works](#how-it-works)
-3. [How to cite and how to contribute](#how-to-cite-and-how-to-contribute)
-
-
-## Installation and Demonstration
-
-### Installation
-
-- OPTION 1: **Quick install:** \
-    Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
-    ```
-    pip install sports2d
-    ```
-
-- OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
-    Open an Anaconda prompt and create a virtual environment by typing:
-    ```
-    conda create -n Sports2D python<=3.10 
-    conda activate Sports2D
-    pip install sports2d
-    ```
-
-- OPTION 3: **Build from source and test the last changes:**\
-     Open a terminal in the directory of your choice and clone the Sports2D repository.
-     ```
-     git clone https://github.com/davidpagnon/sports2d.git
-     cd sports2d
-     pip install .
-     ```
-
-
-### Demonstration: Detect pose and compute 2D angles
-
-Open a terminal, enter `pip show sports2d`, check sports2d package location. \
-Copy this path and go to the Demo folder by typing `cd <path>\Sports2D\Demo`. \
-Type `ipython`, and test the following code:
-```
-from Sports2D import Sports2D
-Sports2D.detect_pose('Config_demo.toml')
-Sports2D.compute_angles('Config_demo.toml')
-```
-
-<img src="Content/demo_blazepose_terminal.png" width="760">
-
-
-You should obtain a video with the overlaid 2D joint positions, and angle text values. This output is also provided as an image folder.\
-You should additionally obtain the same information as time series, stored in .csv files. These files can be opened with any spreadsheet software, or with the Pandas Python library for example.\
-In addition, you will get the original OpenPose-like json coordinates files.
-
-<img src="Content/demo_blazepose_results.png" width="760">
-
-
-## Go further
-
-### Use on your own videos
-
-1. Copy-paste `Config_demo.toml` in the directory of your video.
-
-2. Open it with any text editor.\
-Replace the `video_file` value with the name of your video.
-
-3. Open a terminal or an Anaconda prompt, type:
-   ```
-   cd <Path/to/video/directory>
-   conda activate Sports2D (skip if you did not install with Anaconda)
-   ipython
-   ```
-   ```
-   from Sports2D import Sports2D
-   Sports2D.detect_pose('Config_demo.toml')
-   Sports2D.compute_angles('Config_demo.toml')
-   ```
-
-*Optionally:* If your video is not in the same folder as `Config_demo.toml`, specify its location in `video_dir`.\
-Similarly, if you launch Sports2D in an other directory, specify the location of the config file this way: `Sports2D.detect_pose(<path_to_Config_demo.toml>)`\
-In `pose`, specify the use of BlazePose or OpenPose as joint detectors: this will be detailed in the next section.\
-In `compute_angles`, select your angles of interest.
-
-
-### Use OpenPose for multi-person, more accurate analysis
-
-OpenPose is slower than OpenPose, but more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
-
-1. **Install OpenPose** (instructions [there](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md)). \
-*Windows portable demo works fine.*
-
-2. If you want even more accurate results, use the BODY_25B experimental model instead of the standard BODY_25 one. This requires manually [downloading the model](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md). You can optionally download from there the BODY_135 model which will let you compute wrist flexion and hand segment angle, however this will be much slower.
-
-3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
-
-*N.B.:* If you want to benefit from the capabilities of OpenPose but do not manage to install it, you can use the `Colab notebook` version.\
-Note that your data will be sent to the Google servers, which do not follow the European GDPR requirements regarding privacy.
-**COMING SOON**
-
-
-### Advanced settings
-
-1. `Config_demo.toml` → `pose_advanced`: These settings are only taken into account if OpenPose is used.
-   1. `load_pose`: If you need to change some settings but have already run a pose estimation, you can set this to `true` in order to not regenerate the json pose files.
-
-   2. `save_vid` and `save_img`: You can choose whether you want to save the resulting video and images. If set to `false`, only pose and angle `.csv` files will be generated.
-
-   3. `interp_gap_smaller_than`: Gaps are interpolated only if they are not too wide.
-   
-   4. `filter`: `true` or `false`. If `true`, you can choose among `Butterworth`, `Gaussian`, `LOESS`, or `Median`, and specify their parameters.\
-   Beware that the appearance of the unfiltered skeleton may not match the filtered coordinates and angles.
-
-   5. `show_plots`: Displays a window with tabs corresponding to the coordinates of each detected point. This may cause Python to crash.
-
-2. `Config_demo.toml` → `compute_angles_advanced`: These settings are taken into account both with BlazePose and OpenPose.
-   1. `save_vid` and `save_img`: Cf `pose_advanced`.
-
-   2. `filter`: Cf `pose_advanced`.
-
-   3. `show_plots`: Cf `pose_advanced`.
-
-   <img src="Content/demo_show_plots.png" width="760">
-
-*N.B.:* The settings and results of all analyses are stored int the `logs.txt` file, which can be found in in the sports2d installation folder (`pip show sports2d` to find the path).
-
-
-
-### How it works
-
-#### Pose detection:
-
-BlazePose or OpenPose are used to detect joint centers from a video.
-
-If `BlazePose` is used, only one person can be detected.\
-No interpolation nor filtering options are available. Not plotting available.
-
-If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
-Sequences of missing data are interpolated if they are less than N frames long.\
-Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
-
-
-#### Angle computation:
-
-Joint and segment angles are computed from csv position files.\
-If a person suddently faces the other way, this change of direction is taken into account.\
-Resulting angles can be filtered in the same way as point coordinates, and they can also be plotted.
-
-**Joint angle conventions:**
-- Ankle dorsiflexion: Between heel and big toe, and ankle and knee
-- Knee flexion: Between hip, knee, and ankle 
-- Hip flexion: Between knee, hip, and shoulder
-- Shoulder flexion: Between hip, shoulder, and elbow
-- Elbow flexion: Between wrist, elbow, and shoulder
-
-**Segment angle conventions:**\
-Angles are measured anticlockwise between the horizontal and the segment.
-- Foot: Between heel and big toe
-- Shank: Between knee and ankle
-- Thigh: Between hip and knee
-- Arm: Between shoulder and elbow
-- Forearm: Between elbow and wrist
-- Trunk: Between shoulder midpoint and hip midpoint
-
-## How to cite and how to contribute
-
-### How to cite
-If you use this code or data, please cite [Pagnon, 2023].
-
-     @misc{Pagnon2023,
-       author = {Pagnon, David},
-       title = {Sports2D - Angles from monocular video},
-       year = {2013},
-       publisher = {GitHub},
-       journal = {GitHub repository},
-       howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
-     }
-
-### How to contribute
-I would happily welcome any proposal for new features, code improvement, and more!\
-If you want to contribute to Sports2D, please follow [this guide](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to fork, modify and push code, and submit a pull request. I would appreciate it if you provided as much useful information as possible about how you modified the code, and a rationale for why you're making this pull request. Please also specify on which operating system and on which python version you have tested the code.
-
-*Here is a to-do list, for general guidance purposes only:*
-> <li> <b>GUI applications:</b> For Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with <a href="https://kivy.org">Kivy</a>.</li>
-> <li> <b>Pose refinement:</b> Click and move badly estimated 2D points. See <a href="https://www.youtube.com/watch?v=bEuBKB7eqmk">DeepLabCut</a> for inspiration.
-> <li> <b>Include OpenPose in Sports2D:</b> For example, <a href="https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile">Dockerize</a> it. Otherwise, run Sports2D in a <a href="https://colab.research.google.com/github/hardik0/AI-basketball-analysis-on-google-colab/blob/master/AI_basketball_analysis_google_colab.ipynb">Colab notebook</a>.
-> <li> <b>Constrain points</b> to OpenSim skeletal model for better angle estimation. Cf <a href="https://github.com/perfanalytics/pose2sim">Pose2Sim</a>, but in 2D.
+<!-- 
+[![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
+[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D) \
+[![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
+[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
+[![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
+-->
+
+
+# Sports2D
+
+**`Sports2D` lets you compute 2D joint and segment angles from a single video.**
+
+ </br>
+ </br>
+
+<img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
+
+`Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
+`Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
+If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.
+
+`Announcement:` Apps with GUI will be released for Windows, Linux, MacOS, as well as Android and iOS.
+Mobile versions will only support simple exploratory analysis. This involves single-person angle computation, in a potentially less accurate and tunable way.
+
+
+## Contents
+1. [Installation and Demonstration](#installation-and-demonstration)
+   1. [Installation](#installation)
+   2. [Demonstration: Detect pose and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles)
+2. [Go further](#go-further)
+   1. [Use on your own videos](#use-on-your-own-videos)
+   2. [Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-multi-person-more-accurate-analysis)
+   3. [Advanced-settings](#advanced-settings)
+   4. [How it works](#how-it-works)
+3. [How to cite and how to contribute](#how-to-cite-and-how-to-contribute)
+
+
+## Installation and Demonstration
+
+### Installation
+
+- OPTION 1: **Quick install:** \
+    Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
+    ```
+    pip install sports2d
+    ```
+
+- OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
+    Open an Anaconda prompt and create a virtual environment by typing:
+    ```
+    conda create -n Sports2D python<=3.10 
+    conda activate Sports2D
+    pip install sports2d
+    ```
+
+- OPTION 3: **Build from source and test the last changes:**\
+     Open a terminal in the directory of your choice and clone the Sports2D repository.
+     ```
+     git clone https://github.com/davidpagnon/sports2d.git
+     cd sports2d
+     pip install .
+     ```
+
+
+### Demonstration: Detect pose and compute 2D angles
+
+Open a terminal, enter `pip show sports2d`, check sports2d package location. \
+Copy this path and go to the Demo folder by typing `cd <path>\Sports2D\Demo`. \
+Type `ipython`, and test the following code:
+```
+from Sports2D import Sports2D
+Sports2D.detect_pose('Config_demo.toml')
+Sports2D.compute_angles('Config_demo.toml')
+```
+
+<img src="Content/demo_blazepose_terminal.png" width="760">
+
+
+You should obtain a video with the overlaid 2D joint positions, and angle text values. This output is also provided as an image folder.\
+You should additionally obtain the same information as time series, stored in .csv files. These files can be opened with any spreadsheet software, or with the Pandas Python library for example.\
+In addition, you will get the original OpenPose-like json coordinates files.
+
+<img src="Content/demo_blazepose_results.png" width="760">
+
+
+## Go further
+
+### Use on your own videos
+
+1. Copy-paste `Config_demo.toml` in the directory of your video.
+
+2. Open it with any text editor.\
+Replace the `video_file` value with the name of your video.
+
+3. Open a terminal or an Anaconda prompt, type:
+   ```
+   cd <Path/to/video/directory>
+   conda activate Sports2D (skip if you did not install with Anaconda)
+   ipython
+   ```
+   ```
+   from Sports2D import Sports2D
+   Sports2D.detect_pose('Config_demo.toml')
+   Sports2D.compute_angles('Config_demo.toml')
+   ```
+
+*Optionally:* If your video is not in the same folder as `Config_demo.toml`, specify its location in `video_dir`.\
+Similarly, if you launch Sports2D in an other directory, specify the location of the config file this way: `Sports2D.detect_pose(<path_to_Config_demo.toml>)`\
+In `pose`, specify the use of BlazePose or OpenPose as joint detectors: this will be detailed in the next section.\
+In `compute_angles`, select your angles of interest.
+
+
+### Use OpenPose for multi-person, more accurate analysis
+
+OpenPose is slower than OpenPose, but more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
+
+1. **Install OpenPose** (instructions [there](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md)). \
+*Windows portable demo works fine.*
+
+2. If you want even more accurate results, use the BODY_25B experimental model instead of the standard BODY_25 one. This requires manually [downloading the model](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md). You can optionally download from there the BODY_135 model which will let you compute wrist flexion and hand segment angle, however this will be much slower.
+
+3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
+
+*N.B.:* If you want to benefit from the capabilities of OpenPose but do not manage to install it, you can use the `Colab notebook` version.\
+Note that your data will be sent to the Google servers, which do not follow the European GDPR requirements regarding privacy.
+**COMING SOON**
+
+<img src="Content/demo_blazepose_results.png" width="760">
+
+### Advanced settings
+
+1. `Config_demo.toml` → `pose_advanced`: These settings are only taken into account if OpenPose is used.
+   1. `load_pose`: If you need to change some settings but have already run a pose estimation, you can set this to `true` in order to not regenerate the json pose files.
+
+   2. `save_vid` and `save_img`: You can choose whether you want to save the resulting video and images. If set to `false`, only pose and angle `.csv` files will be generated.
+
+   3. `interp_gap_smaller_than`: Gaps are interpolated only if they are not too wide.
+   
+   4. `filter`: `true` or `false`. If `true`, you can choose among `Butterworth`, `Gaussian`, `LOESS`, or `Median`, and specify their parameters.\
+   Beware that the appearance of the unfiltered skeleton may not match the filtered coordinates and angles.
+
+   5. `show_plots`: Displays a window with tabs corresponding to the coordinates of each detected point. This may cause Python to crash.
+
+2. `Config_demo.toml` → `compute_angles_advanced`: These settings are taken into account both with BlazePose and OpenPose.
+   1. `save_vid` and `save_img`: Cf `pose_advanced`.
+
+   2. `filter`: Cf `pose_advanced`.
+
+   3. `show_plots`: Cf `pose_advanced`.
+
+   <img src="Content/demo_show_plots.png" width="760">
+
+*N.B.:* The settings and results of all analyses are stored int the `logs.txt` file, which can be found in in the sports2d installation folder (`pip show sports2d` to find the path).
+
+
+
+### How it works
+
+#### Pose detection:
+
+BlazePose or OpenPose are used to detect joint centers from a video.
+
+If `BlazePose` is used, only one person can be detected.\
+No interpolation nor filtering options are available. Not plotting available.
+
+If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
+Sequences of missing data are interpolated if they are less than N frames long.\
+Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
+
+
+#### Angle computation:
+
+Joint and segment angles are computed from csv position files.\
+If a person suddently faces the other way, this change of direction is taken into account.\
+Resulting angles can be filtered in the same way as point coordinates, and they can also be plotted.
+
+**Joint angle conventions:**
+- Ankle dorsiflexion: Between heel and big toe, and ankle and knee
+- Knee flexion: Between hip, knee, and ankle 
+- Hip flexion: Between knee, hip, and shoulder
+- Shoulder flexion: Between hip, shoulder, and elbow
+- Elbow flexion: Between wrist, elbow, and shoulder
+
+**Segment angle conventions:**\
+Angles are measured anticlockwise between the horizontal and the segment.
+- Foot: Between heel and big toe
+- Shank: Between knee and ankle
+- Thigh: Between hip and knee
+- Arm: Between shoulder and elbow
+- Forearm: Between elbow and wrist
+- Trunk: Between shoulder midpoint and hip midpoint
+
+## How to cite and how to contribute
+
+### How to cite
+If you use this code or data, please cite [Pagnon, 2023].
+
+     @misc{Pagnon2023,
+       author = {Pagnon, David},
+       title = {Sports2D - Angles from monocular video},
+       year = {2013},
+       publisher = {GitHub},
+       journal = {GitHub repository},
+       howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
+     }
+
+### How to contribute
+I would happily welcome any proposal for new features, code improvement, and more!\
+If you want to contribute to Sports2D, please follow [this guide](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to fork, modify and push code, and submit a pull request. I would appreciate it if you provided as much useful information as possible about how you modified the code, and a rationale for why you're making this pull request. Please also specify on which operating system and on which python version you have tested the code.
+
+*Here is a to-do list, for general guidance purposes only:*
+> <li> <b>GUI applications:</b> For Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with <a href="https://kivy.org">Kivy</a>.</li>
+> <li> <b>Pose refinement:</b> Click and move badly estimated 2D points. See <a href="https://www.youtube.com/watch?v=bEuBKB7eqmk">DeepLabCut</a> for inspiration.
+> <li> <b>Include OpenPose in Sports2D:</b> For example, <a href="https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile">Dockerize</a> it. Otherwise, run Sports2D in a <a href="https://colab.research.google.com/github/hardik0/AI-basketball-analysis-on-google-colab/blob/master/AI_basketball_analysis_google_colab.ipynb">Colab notebook</a>.
+> <li> <b>Constrain points</b> to OpenSim skeletal model for better angle estimation. Cf <a href="https://github.com/perfanalytics/pose2sim">Pose2Sim</a>, but in 2D.
```

### Comparing `sports2d-0.0.2/Sports2D/Demo/Config_demo.toml` & `sports2d-0.0.5/Sports2D/Demo/Config_demo.toml`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-###############################################################################
-## SPORTS2D PROJECT PARAMETERS                                               ##
-###############################################################################
-
-# Configure your project parameters here
-
-
-[project]
-video_dir = '' # BETWEEN SINGLE QUOTES! # If empty, project dir is current dir
-video_file = 'demo.mp4'
-
-
-[pose]
-pose_algo = 'BLAZEPOSE' # 'OPENPOSE' or 'BLAZEPOSE' 
-# OpenPose is more accurate and supports multi-person detection, but needs to be installed separately	
-# Coming soon: 'deeplabcut', 'alphapose'
-	
-	[pose.BLAZEPOSE]
-	# 0,1,2. 2 is slightly slower but more accurate
-	model_complexity = 2 
-		
-	[pose.OPENPOSE]
-	# Install OpenPose from https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md
-	# BODY_25 is standard, BODY_25B is more accurate but requires downloading the model from 
-	# https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md
-	openpose_model = 'BODY_25B' 
-	
-	# Installation path of openpose (between single quotes) 
-	openpose_path = 'D:\softs\openpose-1.6.0-binaries-win64-gpu-flir-3d_recommended\openpose'
-	
-
-[compute_angles]
-# Select joint angles among
-# ['Right ankle', 'Left ankle', 'Right knee', 'Left knee', 'Right hip', 'Left hip', 'Right shoulder', 'Left shoulder', 'Right elbow', 'Left elbow', 'Right wrist', 'Left wrist']
-joint_angles = ['Right ankle', 'Left ankle', 'Right knee', 'Left knee', 'Right hip', 'Left hip', 'Right shoulder', 'Left shoulder', 'Right elbow', 'Left elbow']
-
-# Select segment angles among
-# ['Right foot', 'Left foot', 'Right shank', 'Left shank', 'Right thigh', 'Left thigh', 'Trunk', 'Right arm', 'Left arm', 'Right forearm', 'Left forearm', 'Right hand', 'Left hand']
-segment_angles = ['Right foot', 'Left foot', 'Right shank', 'Left shank', 'Right thigh', 'Left thigh', 'Trunk', 'Right arm', 'Left arm', 'Right forearm', 'Left forearm']
-
-   	
-	
-
-# ADVANCED CONFIGURATION
-	
-[pose_advanced] # only for OPENPOSE
-load_pose = false # else proceed to detection
-save_vid = true
-save_img = true
-interp_gap_smaller_than = 5 # do not interpolate bigger gaps
-filter = true
-show_plots = false
-filter_type = 'butterworth' # butterworth, gaussian, LOESS, median
-   [pose_advanced.butterworth]
-   order = 4 
-   cut_off_frequency = 6 # Hz
-   [pose_advanced.gaussian]
-   sigma_kernel = 1 #px
-   [pose_advanced.loess]
-   nb_values_used = 5 # = fraction of data used * nb frames
-   [pose_advanced.median]
-   kernel_size = 3
-
-
-[compute_angles_advanced] # for OPENPOSE and BLAZEPOSE
-save_img = true
-save_vid = true
-filter = false
-show_plots = false
-filter_type = 'butterworth' # butterworth, gaussian, LOESS, median
-   [compute_angles_advanced.butterworth]
-   order = 4 
-   cut_off_frequency = 6 # Hz
-   [compute_angles_advanced.gaussian]
-   sigma_kernel = 1 #px
-   [compute_angles_advanced.loess]
-   nb_values_used = 5 # = fraction of data used * nb frames
-   [compute_angles_advanced.median]
-   kernel_size = 3
+###############################################################################
+## SPORTS2D PROJECT PARAMETERS                                               ##
+###############################################################################
+
+# Configure your project parameters here
+
+
+[project]
+video_dir = '' # BETWEEN SINGLE QUOTES! # If empty, project dir is current dir
+video_file = 'demo.mp4'
+
+
+[pose]
+pose_algo = 'BLAZEPOSE' # 'OPENPOSE' or 'BLAZEPOSE' 
+# OpenPose is more accurate and supports multi-person detection, but needs to be installed separately	
+# Coming soon: 'deeplabcut', 'alphapose'
+	
+	[pose.BLAZEPOSE]
+	# 0,1,2. 2 is slightly slower but more accurate
+	model_complexity = 2 
+		
+	[pose.OPENPOSE]
+	# Install OpenPose from https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md
+	# BODY_25 is standard, BODY_25B is more accurate but requires downloading the model from 
+	# https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md
+	openpose_model = 'BODY_25B' 
+	
+	# Installation path of openpose (between single quotes) 
+	openpose_path = 'D:\softs\openpose-1.6.0-binaries-win64-gpu-flir-3d_recommended\openpose'
+	
+
+[compute_angles]
+# Select joint angles among
+# ['Right ankle', 'Left ankle', 'Right knee', 'Left knee', 'Right hip', 'Left hip', 'Right shoulder', 'Left shoulder', 'Right elbow', 'Left elbow', 'Right wrist', 'Left wrist']
+joint_angles = ['Right ankle', 'Left ankle', 'Right knee', 'Left knee', 'Right hip', 'Left hip', 'Right shoulder', 'Left shoulder', 'Right elbow', 'Left elbow']
+
+# Select segment angles among
+# ['Right foot', 'Left foot', 'Right shank', 'Left shank', 'Right thigh', 'Left thigh', 'Trunk', 'Right arm', 'Left arm', 'Right forearm', 'Left forearm', 'Right hand', 'Left hand']
+segment_angles = ['Right foot', 'Left foot', 'Right shank', 'Left shank', 'Right thigh', 'Left thigh', 'Trunk', 'Right arm', 'Left arm', 'Right forearm', 'Left forearm']
+
+   	
+	
+
+# ADVANCED CONFIGURATION
+	
+[pose_advanced] # only for OPENPOSE
+load_pose = false # else proceed to detection
+save_vid = true
+save_img = true
+interp_gap_smaller_than = 5 # do not interpolate bigger gaps
+filter = true
+show_plots = false
+filter_type = 'butterworth' # butterworth, gaussian, LOESS, median
+   [pose_advanced.butterworth]
+   order = 4 
+   cut_off_frequency = 6 # Hz
+   [pose_advanced.gaussian]
+   sigma_kernel = 1 #px
+   [pose_advanced.loess]
+   nb_values_used = 5 # = fraction of data used * nb frames
+   [pose_advanced.median]
+   kernel_size = 3
+
+
+[compute_angles_advanced] # for OPENPOSE and BLAZEPOSE
+save_img = true
+save_vid = true
+filter = false
+show_plots = false
+filter_type = 'butterworth' # butterworth, gaussian, LOESS, median
+   [compute_angles_advanced.butterworth]
+   order = 4 
+   cut_off_frequency = 6 # Hz
+   [compute_angles_advanced.gaussian]
+   sigma_kernel = 1 #px
+   [compute_angles_advanced.loess]
+   nb_values_used = 5 # = fraction of data used * nb frames
+   [compute_angles_advanced.median]
+   kernel_size = 3
```

### Comparing `sports2d-0.0.2/Sports2D/Demo/demo.mp4` & `sports2d-0.0.5/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.2/Sports2D/Sports2D.py` & `sports2d-0.0.5/Sports2D/Sports2D.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-
-'''
-    ##############################################################
-    ## SPORTS2D                                                 ##
-    ##############################################################
-    
-    This repository provides a workflow to compute 2D markerless
-    joint and segment angles from videos. 
-    These angles can be plotted and processed with any 
-    spreadsheet software or programming language.
-    
-    This is a headless version, but apps will be released 
-    for Windows, Linux, MacOS, as well as Android and iOS.
-    Mobile versions will only support exploratory joint detection 
-    from BlazePose, hence less accurately and less tunable.
-    
-    If you need to detect several persons and want more accurate results, 
-    you can install and use OpenPose: 
-    https://github.com/CMU-Perceptual-Computing-Lab/openpose
-    
-    -----
-    Sports2D installation:
-    -----
-    Optional: 
-    - Install Miniconda
-    - Open a Anaconda Prompt and type: 
-    `conda create -n Sports2D python>=3.7`
-    `conda activate Sports2D`
-    pip install 
-    
-    - Open a python prompt and type `pip install sports2d`
-    - `pip show sports2d`
-    - Adjust your settings (in particular video path) in `Config_demo.toml`
-    - ```from Sports2D import Sports2D
-    Sports2D.detect_pose('Config_demo.toml')
-    Sports2D.compute_angles('Config_demo.toml')```
-    
-    -----
-    /!\ Warning /!\
-    -----
-    - The angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.
-    - It will only lead to acceptable results if the persons move in the 2D plane (sagittal plane).
-    - The persons need to be filmed as perpendicularly as possible from their side.
-    If you need research-grade markerless joint kinematics, consider using several cameras,
-    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
-    https://github.com/perfanalytics/pose2sim
-    
-    -----
-    Pose detection:
-    -----
-    Detect joint centers from a video with OpenPose or BlazePose.
-    Save a 2D csv position file per person, and optionally json files, image files, and video files.
-    
-    If OpenPose is used, multiple persons can be consistently detected across frames.
-    Interpolates sequences of missing data if they are less than N frames long.
-    Optionally filters results with Butterworth, gaussian, median, or loess filter.
-    Optionally displays figures.
-
-    If BlazePose is used, only one person can be detected.
-    No interpolation nor filtering options available. Not plotting available.
-    
-    -----
-    Angle computation:
-    -----
-    Compute joint and segment angles from csv position files.
-    Automatically adjust angles when person switches to face the other way.
-    Save a 2D csv angle file per person.
-    Optionally filters results with Butterworth, gaussian, median, or loess filter.
-    Optionally displays figures.
-    Optionally saves images and video with overlaid angles.
-
-    Joint angle conventions:
-    - Ankle dorsiflexion: Between heel and big toe, and ankle and knee
-    - Knee flexion: Between hip, knee, and ankle 
-    - Hip flexion: Between knee, hip, and shoulder
-    - Shoulder flexion: Between hip, shoulder, and elbow
-    - Elbow flexion: Between wrist, elbow, and shoulder
-
-    Segment angle conventions:
-    Angles are measured anticlockwise between the horizontal and the segment.
-    - Foot: Between heel and big toe
-    - Shank: Between ankle and knee
-    - Thigh: Between hip and knee
-    - Arm: Between shoulder and elbow
-    - Forearm: Between elbow and wrist
-    - Trunk: Between hip midpoint and shoulder midpoint
-    
-    -----
-    To-do list:
-    -----
-    - GUI applications for all platforms (with Kivy: https://kivy.org/)
-    - Pose refinement: click and move badly estimated 2D points (cf DeepLabCut: https://www.youtube.com/watch?v=bEuBKB7eqmk)
-    - Include OpenPose in Sports2D (dockerize it cf https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile)
-    - Constrain points to OpenSim skeletal model for better angle estimation (cf Pose2Sim but in 2D https://github.com/perfanalytics/pose2sim)
-    
-'''
-
-
-## INIT
-import toml
-import os
-import time
-import cv2
-from pathlib import Path
-import logging, logging.handlers
-
-with open(Path('logs.txt'), 'a+') as log_f: pass
-logging.basicConfig(format='%(message)s', level=logging.INFO, 
-    handlers = [logging.handlers.TimedRotatingFileHandler(Path('logs.txt'), when='D', interval=7), logging.StreamHandler()]) 
-
-
-## AUTHORSHIP INFORMATION
-__author__ = "David Pagnon"
-__copyright__ = "Copyright 2023, Sports2D"
-__credits__ = ["David Pagnon"]
-__license__ = "BSD 3-Clause License"
-__version__ = "0.1"
-__maintainer__ = "David Pagnon"
-__email__ = "contact@david-pagnon.com"
-__status__ = "Development"
-
-
-## FUNCTIONS
-def read_config_file(config):
-    '''
-    Read configation file.
-    '''
-
-    config_dict = toml.load(config)
-    return config_dict
-
-
-def base_params(config_dict):
-    '''
-    Retrieve sequence name and frames to be analyzed.
-    '''
-
-    video_dir = Path(config_dict.get('project').get('video_dir')).resolve()
-    if video_dir == '': video_dir = os.getcwd()
-    video_file = Path(config_dict.get('project').get('video_file'))
-    
-    video = cv2.VideoCapture(str(video_dir / video_file))
-    frame_rate = video.get(cv2.CAP_PROP_FPS)
-    video.release()
-
-    return video_dir, video_file, frame_rate
-
-
-def detect_pose(config='Config_demo.toml'):
-    '''
-    Compute 2D pose from video.
-    Save 2D csv file, and optionally json files, image files, and video file.
-    Optionally interpolates missing data, filters them, and displays figures.
-    '''
-
-    from Sports2D.detect_pose import detect_pose_fun
-    
-    config_dict = read_config_file(config)
-    _, video_file, _ = base_params(config_dict)
-    
-    logging.info("\n\n---------------------------------------------------------------------")
-    logging.info(f"Detect pose for video {video_file}")
-    logging.info("---------------------------------------------------------------------")
-    start = time.time()
-    
-    detect_pose_fun(config_dict)
-    
-    end = time.time()
-    logging.info(f'Pose detection took {end-start:.2f} s.')
-    
-    
-def compute_angles(config='Config_demo.toml'):
-    '''
-    Compute joint and segment angles from 2D points coordinates in csv file.
-    Save csv file.
-    Optionally interpolates missing data, filters them, and displays figures.
-    '''
-
-    from Sports2D.compute_angles import compute_angles_fun
-
-    config_dict = read_config_file(config)
-    _, video_file, _ = base_params(config_dict)
-    joint_angles = config_dict.get('compute_angles').get('joint_angles')
-    segment_angles = config_dict.get('compute_angles').get('segment_angles')
-
-    logging.info("\n\n---------------------------------------------------------------------")
-    logging.info(f"Compute angles for video {video_file} ")
-    logging.info(f"for {joint_angles}")
-    logging.info(f"and {segment_angles}.")
-    logging.info("---------------------------------------------------------------------")
-    start = time.time()
-    
-    compute_angles_fun(config_dict)
-    
-    end = time.time()
-    logging.info(f'Joint and segment computation took {end-start:.2f} s.')
-    
-    
-
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+
+'''
+    ##############################################################
+    ## SPORTS2D                                                 ##
+    ##############################################################
+    
+    This repository provides a workflow to compute 2D markerless
+    joint and segment angles from videos. 
+    These angles can be plotted and processed with any 
+    spreadsheet software or programming language.
+    
+    This is a headless version, but apps will be released 
+    for Windows, Linux, MacOS, as well as Android and iOS.
+    Mobile versions will only support exploratory joint detection 
+    from BlazePose, hence less accurately and less tunable.
+    
+    If you need to detect several persons and want more accurate results, 
+    you can install and use OpenPose: 
+    https://github.com/CMU-Perceptual-Computing-Lab/openpose
+    
+    -----
+    Sports2D installation:
+    -----
+    Optional: 
+    - Install Miniconda
+    - Open a Anaconda Prompt and type: 
+    `conda create -n Sports2D python>=3.7`
+    `conda activate Sports2D`
+    pip install 
+    
+    - Open a python prompt and type `pip install sports2d`
+    - `pip show sports2d`
+    - Adjust your settings (in particular video path) in `Config_demo.toml`
+    - ```from Sports2D import Sports2D
+    Sports2D.detect_pose('Config_demo.toml')
+    Sports2D.compute_angles('Config_demo.toml')```
+    
+    -----
+    /!\ Warning /!\
+    -----
+    - The angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.
+    - It will only lead to acceptable results if the persons move in the 2D plane (sagittal plane).
+    - The persons need to be filmed as perpendicularly as possible from their side.
+    If you need research-grade markerless joint kinematics, consider using several cameras,
+    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
+    https://github.com/perfanalytics/pose2sim
+    
+    -----
+    Pose detection:
+    -----
+    Detect joint centers from a video with OpenPose or BlazePose.
+    Save a 2D csv position file per person, and optionally json files, image files, and video files.
+    
+    If OpenPose is used, multiple persons can be consistently detected across frames.
+    Interpolates sequences of missing data if they are less than N frames long.
+    Optionally filters results with Butterworth, gaussian, median, or loess filter.
+    Optionally displays figures.
+
+    If BlazePose is used, only one person can be detected.
+    No interpolation nor filtering options available. Not plotting available.
+    
+    -----
+    Angle computation:
+    -----
+    Compute joint and segment angles from csv position files.
+    Automatically adjust angles when person switches to face the other way.
+    Save a 2D csv angle file per person.
+    Optionally filters results with Butterworth, gaussian, median, or loess filter.
+    Optionally displays figures.
+    Optionally saves images and video with overlaid angles.
+
+    Joint angle conventions:
+    - Ankle dorsiflexion: Between heel and big toe, and ankle and knee
+    - Knee flexion: Between hip, knee, and ankle 
+    - Hip flexion: Between knee, hip, and shoulder
+    - Shoulder flexion: Between hip, shoulder, and elbow
+    - Elbow flexion: Between wrist, elbow, and shoulder
+
+    Segment angle conventions:
+    Angles are measured anticlockwise between the horizontal and the segment.
+    - Foot: Between heel and big toe
+    - Shank: Between ankle and knee
+    - Thigh: Between hip and knee
+    - Arm: Between shoulder and elbow
+    - Forearm: Between elbow and wrist
+    - Trunk: Between hip midpoint and shoulder midpoint
+    
+    -----
+    To-do list:
+    -----
+    - GUI applications for all platforms (with Kivy: https://kivy.org/)
+    - Pose refinement: click and move badly estimated 2D points (cf DeepLabCut: https://www.youtube.com/watch?v=bEuBKB7eqmk)
+    - Include OpenPose in Sports2D (dockerize it cf https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile)
+    - Constrain points to OpenSim skeletal model for better angle estimation (cf Pose2Sim but in 2D https://github.com/perfanalytics/pose2sim)
+    
+'''
+
+
+## INIT
+import toml
+import os
+import time
+import cv2
+from pathlib import Path
+import logging, logging.handlers
+
+with open(Path('logs.txt'), 'a+') as log_f: pass
+logging.basicConfig(format='%(message)s', level=logging.INFO, 
+    handlers = [logging.handlers.TimedRotatingFileHandler(Path('logs.txt'), when='D', interval=7), logging.StreamHandler()]) 
+
+
+## AUTHORSHIP INFORMATION
+__author__ = "David Pagnon"
+__copyright__ = "Copyright 2023, Sports2D"
+__credits__ = ["David Pagnon"]
+__license__ = "BSD 3-Clause License"
+__version__ = "0.1"
+__maintainer__ = "David Pagnon"
+__email__ = "contact@david-pagnon.com"
+__status__ = "Development"
+
+
+## FUNCTIONS
+def read_config_file(config):
+    '''
+    Read configation file.
+    '''
+
+    config_dict = toml.load(config)
+    return config_dict
+
+
+def base_params(config_dict):
+    '''
+    Retrieve sequence name and frames to be analyzed.
+    '''
+
+    video_dir = Path(config_dict.get('project').get('video_dir')).resolve()
+    if video_dir == '': video_dir = os.getcwd()
+    video_file = Path(config_dict.get('project').get('video_file'))
+    
+    video = cv2.VideoCapture(str(video_dir / video_file))
+    frame_rate = video.get(cv2.CAP_PROP_FPS)
+    video.release()
+
+    return video_dir, video_file, frame_rate
+
+
+def detect_pose(config='Config_demo.toml'):
+    '''
+    Compute 2D pose from video.
+    Save 2D csv file, and optionally json files, image files, and video file.
+    Optionally interpolates missing data, filters them, and displays figures.
+    '''
+
+    from Sports2D.detect_pose import detect_pose_fun
+    
+    config_dict = read_config_file(config)
+    _, video_file, _ = base_params(config_dict)
+    
+    logging.info("\n\n---------------------------------------------------------------------")
+    logging.info(f"Detect pose for video {video_file}")
+    logging.info("---------------------------------------------------------------------")
+    start = time.time()
+    
+    detect_pose_fun(config_dict)
+    
+    end = time.time()
+    logging.info(f'Pose detection took {end-start:.2f} s.')
+    
+    
+def compute_angles(config='Config_demo.toml'):
+    '''
+    Compute joint and segment angles from 2D points coordinates in csv file.
+    Save csv file.
+    Optionally interpolates missing data, filters them, and displays figures.
+    '''
+
+    from Sports2D.compute_angles import compute_angles_fun
+
+    config_dict = read_config_file(config)
+    _, video_file, _ = base_params(config_dict)
+    joint_angles = config_dict.get('compute_angles').get('joint_angles')
+    segment_angles = config_dict.get('compute_angles').get('segment_angles')
+
+    logging.info("\n\n---------------------------------------------------------------------")
+    logging.info(f"Compute angles for video {video_file} ")
+    logging.info(f"for {joint_angles}")
+    logging.info(f"and {segment_angles}.")
+    logging.info("---------------------------------------------------------------------")
+    start = time.time()
+    
+    compute_angles_fun(config_dict)
+    
+    end = time.time()
+    logging.info(f'Joint and segment computation took {end-start:.2f} s.')
+    
+    
+
```

### Comparing `sports2d-0.0.2/Sports2D/Utilities/Blazepose_runsave.py` & `sports2d-0.0.5/Sports2D/Utilities/Blazepose_runsave.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-
-'''
-    ########################################################
-    ## Run BlazePose and save coordinates                 ##
-    ########################################################
-    
-    Runs BlazePose (Mediapipe) on a video
-    Saves coordinates to OpenPose format (json files) or DeepLabCut format (csv or h5 table)
-    Optionally displays and saves images with keypoints overlayed
-
-    N.B.: First install mediapipe: `pip install mediapipe`
-    You may also need to install tables: `pip install tables`
-        
-    Usage: 
-    python -m Blazepose_runsave -i "<input_file>" --display --save_images --save_video --to_csv --to_h5 --to_json --model_complexity 2 -o "<output_folder>"
-    OR python -m Blazepose_runsave -i "<input_file>" --display --to_json --save_images 
-    OR python -m Blazepose_runsave -i "<input_file>" -dJs
-    OR from Pose2Sim.Utilities import Blazepose_runsave; Blazepose_runsave.blazepose_detec_func(input_file=r'input_file', save_images=True, to_json=True, model_complexity=2)
-'''
-
-
-## INIT
-import cv2
-import mediapipe as mp
-import os
-import logging
-import pandas as pd
-import numpy as np
-import json
-import argparse
-
-mp_drawing = mp.solutions.drawing_utils
-mp_drawing_styles = mp.solutions.drawing_styles
-mp_pose = mp.solutions.pose
-
-
-## AUTHORSHIP INFORMATION
-__author__ = "David Pagnon"
-__copyright__ = "Copyright 2022, Pose2Sim"
-__credits__ = ["David Pagnon"]
-__license__ = "BSD 3-Clause License"
-__version__ = "0.1"
-__maintainer__ = "David Pagnon"
-__email__ = "contact@david-pagnon.com"
-__status__ = "Development"
-
-
-## FUNCTIONS
-def save_to_csv_or_h5(kpt_list, output_folder, video_name, to_csv, to_h5):
-    '''
-    Saves blazepose keypoint coordinates to csv or h5 file, 
-    in the DeepLabCut format.
-
-    INPUTS:
-    - kpt_list: List of lists of keypoints X and Y coordinates and likelihood, for each frame
-    - output_folder: Folder where to save the csv or h5 file
-    - video_name: Name of the video
-    - to_csv: Boolean, whether to save to csv
-    - to_h5: Boolean, whether to save to h5
-
-    OUTPUTS:
-    - Creation of csv or h5 file in output_folder
-    '''
-    
-    # Prepare dataframe file
-    scorer = ['DavidPagnon']*len(mp_pose.PoseLandmark)*3
-    individuals = ['person']*len(mp_pose.PoseLandmark)*3
-    bodyparts = [[p]*3 for p in ['Nose', 'LEyeInner', 'LEye', 'LEyeOuter', 'REyeInner', 'REye', 'REyeOuter', 'LEar', 'REar', 'LMouth', 'RMouth', 'LShoulder', 'RShoulder', 'LElbow', 'RElbow', 'LWrist', 'RWrist', 'LPinky', 'RPinky', 'LIndex', 'RIndex', 'LThumb', 'RThumb', 'LHip', 'RHip', 'LKnee', 'RKnee', 'LAnkle', 'RAnkle', 'LHeel', 'RHeel', 'LBigToe', 'RBigToe']]
-    bodyparts = [item for sublist in bodyparts for item in sublist]
-    coords = ['x', 'y', 'likelihood']*len(mp_pose.PoseLandmark)
-
-    tuples = list(zip(scorer, individuals, bodyparts, coords))
-    index_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'bodyparts', 'coords'])
-    df = pd.DataFrame(np.array(kpt_list).T, index=index_csv).T
-
-    if to_csv:
-        csv_file = os.path.join(output_folder, video_name+'_BLAZEPOSE_points.csv')
-        logging.info(f'Saving csv file in {csv_file}.')
-        df.to_csv(csv_file, sep=',', index=True, lineterminator='\n')
-
-    if to_h5:
-        h5_file = os.path.join(output_folder, video_name+'_BLAZEPOSE_points.h5')
-        df.to_hdf(h5_file, index=True, key='BLAZEPOSE_detection')
-
-
-def save_to_json(kpt_list, output_folder, video_name):
-    '''
-    Saves blazepose keypoint coordinates to json file, 
-    in the OpenPose format.
-
-    INPUTS:
-    - kpt_list: List of lists of keypoints X and Y coordinates and likelihood, for each frame
-    - output_folder: Folder where to save the csv or h5 file
-    - video_name: Name of the video
-
-    OUTPUTS:
-    - Creation of json files in output_folder/json_folder    
-    '''
-
-    json_folder = os.path.join(output_folder, video_name + '_BLAZEPOSE_json')
-    if not os.path.exists(json_folder):
-        os.mkdir(json_folder)
-
-    # json preparation
-    json_dict = {'version':1.3, 'people':[]}
-    json_dict['people'] = [{'person_id':[-1], 
-                    'pose_keypoints_2d': [], 
-                    'face_keypoints_2d': [], 
-                    'hand_left_keypoints_2d':[], 
-                    'hand_right_keypoints_2d':[], 
-                    'pose_keypoints_3d':[], 
-                    'face_keypoints_3d':[], 
-                    'hand_left_keypoints_3d':[], 
-                    'hand_right_keypoints_3d':[]}]
-    
-    # write each h5 line in json file
-    for frame, kpt in enumerate(kpt_list):
-        json_dict['people'][0]['pose_keypoints_2d'] = kpt
-        json_file = os.path.join(json_folder, video_name+'_BLAZEPOSE.'+str(frame).zfill(5)+'.json')
-        with open(json_file, 'w') as js_f:
-            js_f.write(json.dumps(json_dict))
-
-
-def blazepose_detec_func(**args):
-    '''
-    Runs BlazePose (Mediapipe) on a video
-    Saves coordinates to OpenPose format (json files) or DeepLabCut format (csv or h5 table)
-    Optionally displays and saves images with keypoints overlayed
-
-    N.B.: First install mediapipe: `pip install mediapipe`
-    You may also need to install tables: `pip install tables`
-        
-    Usage: 
-    python -m Blazepose_runsave -i "<input_file>" --display --save_images --save_video --to_csv --to_h5 --to_json --model_complexity 2 -o "<output_folder>"
-    OR python -m Blazepose_runsave -i "<input_file>" --display --to_json --save_images
-    OR python -m Blazepose_runsave -i "<input_file>" -dJs
-    OR from Pose2Sim.Utilities import Blazepose_runsave; Blazepose_runsave.blazepose_detec_func(input_file=r'input_file', save_images=True, to_json=True, model_complexity=2)
-    '''
-
-    # Retrieve arguments
-    video_input = os.path.realpath(args.get('input_file'))
-    video_dir = os.path.dirname(video_input)
-    video_name = os.path.splitext(os.path.basename(video_input))[0]
-    output_folder = args.get('output_folder')
-
-    display = args.get('display')
-    save_images = args.get('save_images')
-    save_video = args.get('save_video')
-
-    to_csv = args.get('to_csv')
-    to_h5 = args.get('to_h5')
-    to_json = args.get('to_json')
-    
-    model_complexity = int(args.get('model_complexity'))
-    if 'model_complexity' not in vars(): model_complexity=2
-
-    if to_csv or to_h5 or to_json or save_images or save_video:
-        if output_folder == None: 
-            output_folder = video_dir
-        if not os.path.exists(os.path.realpath(output_folder)):
-            os.mkdir(os.path.realpath(output_folder))
-    
-    # Run Blazepose
-    cap = cv2.VideoCapture(video_input)
-    W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
-    fps = cap.get(cv2.CAP_PROP_FPS)
-    count = 0
-    kpt_list = []
-    with mp_pose.Pose(min_detection_confidence=0.5, min_tracking_confidence=0.5, model_complexity=model_complexity) as pose:
-        logging.info(f'Detecting 2D joint positions with BlazePose for {video_input}.')
-        logging.info('Only one person can be detected by BlazePose. No interpolation nor filtering options available. Not plotting available.')
-        if save_images and save_video:
-            logging.info(f'Saving images and video in {output_folder}.')
-        if save_images and not save_video:
-            logging.info(f'Saving images in {output_folder}.')
-        if not save_images and save_video:
-            logging.info(f'Saving video in {output_folder}.')
-
-        while cap.isOpened():
-            ret, frame = cap.read()
-            if ret == True:  
-                # Blazepose detection
-                results = pose.process(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB))            
-                try:
-                    kpt = [[p.x*W, p.y*H, p.visibility] for p in results.pose_landmarks.landmark]
-                    kpt = [item for sublist in kpt for item in sublist]  
-
-                    mp_drawing.draw_landmarks(frame, results.pose_landmarks, mp_pose.POSE_CONNECTIONS, landmark_drawing_spec=mp_drawing_styles.get_default_pose_landmarks_style())
-                except:
-                    print(f'No person detected by BlazePose on frame {count}')
-                    kpt=[np.nan*3*33]
-
-                # Display images
-                if display: 
-                    cv2.imshow('frame', frame)
-                    if cv2.waitKey(30) & 0xFF == ord('q'):
-                        break
-
-                # Save images
-                if save_images: 
-                    images_folder = os.path.join(output_folder, video_name + '_BLAZEPOSE_img')
-                    if not os.path.exists(images_folder):
-                        os.mkdir(images_folder)
-                    cv2.imwrite(os.path.join(images_folder, video_name+'_BLAZEPOSE.'+str(count).zfill(5)+'.png'), frame)
-
-                # Save video
-                if save_video:
-                    if count == 0:
-                        fourcc = cv2.VideoWriter_fourcc(*'mp4v')
-                        writer = cv2.VideoWriter(os.path.join(output_folder, video_name+'_BLAZEPOSE.mp4'), fourcc, fps, (int(W), int(H)))
-                    writer.write(frame)
-
-                # Store coordinates
-                if to_csv or to_h5 or to_json:
-                    kpt_list.append(kpt)
-
-                count += 1
-                
-            else:
-                break
-
-        cap.release()
-        if save_video:
-            writer.release()    
-        cv2.destroyAllWindows()
-
-    # Save coordinates
-    if to_csv or to_h5:
-        save_to_csv_or_h5(kpt_list, output_folder, video_name, to_csv, to_h5)
-   
-    if to_json:
-        save_to_json(kpt_list, output_folder, video_name)
-    
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser()
-    parser.add_argument('-i', '--input_file', required = True, help='input video file')
-    parser.add_argument('-C', '--to_csv', required=False, action='store_true', help='save coordinates to csv')
-    parser.add_argument('-H', '--to_h5', required=False, action='store_true', help='save coordinates to h5')
-    parser.add_argument('-J', '--to_json', required=False, action='store_true', help='save coordinates to json')
-    parser.add_argument('-d', '--display', required = False, action='store_true', help='display images with overlayed coordinates')
-    parser.add_argument('-s', '--save_images', required = False, action='store_true', help='save images with overlayed coordinates')
-    parser.add_argument('-v', '--save_video', required = False, action='store_true', help='save video with overlayed coordinates')
-    parser.add_argument('-m', '--model_complexity', required = False, default = 2, help='model complexity. 0: fastest but less accurate, 2: most accurate but slowest')
-    parser.add_argument('-o', '--output_folder', required=False, help='output folder for coordinates and images')
-    
-    args = vars(parser.parse_args())
-    
-    blazepose_detec_func(**args)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+
+'''
+    ########################################################
+    ## Run BlazePose and save coordinates                 ##
+    ########################################################
+    
+    Runs BlazePose (Mediapipe) on a video
+    Saves coordinates to OpenPose format (json files) or DeepLabCut format (csv or h5 table)
+    Optionally displays and saves images with keypoints overlayed
+
+    N.B.: First install mediapipe: `pip install mediapipe`
+    You may also need to install tables: `pip install tables`
+        
+    Usage: 
+    python -m Blazepose_runsave -i "<input_file>" --display --save_images --save_video --to_csv --to_h5 --to_json --model_complexity 2 -o "<output_folder>"
+    OR python -m Blazepose_runsave -i "<input_file>" --display --to_json --save_images 
+    OR python -m Blazepose_runsave -i "<input_file>" -dJs
+    OR from Pose2Sim.Utilities import Blazepose_runsave; Blazepose_runsave.blazepose_detec_func(input_file=r'input_file', save_images=True, to_json=True, model_complexity=2)
+'''
+
+
+## INIT
+import cv2
+import mediapipe as mp
+import os
+import logging
+import pandas as pd
+import numpy as np
+import json
+import argparse
+
+mp_drawing = mp.solutions.drawing_utils
+mp_drawing_styles = mp.solutions.drawing_styles
+mp_pose = mp.solutions.pose
+
+
+## AUTHORSHIP INFORMATION
+__author__ = "David Pagnon"
+__copyright__ = "Copyright 2022, Pose2Sim"
+__credits__ = ["David Pagnon"]
+__license__ = "BSD 3-Clause License"
+__version__ = "0.1"
+__maintainer__ = "David Pagnon"
+__email__ = "contact@david-pagnon.com"
+__status__ = "Development"
+
+
+## FUNCTIONS
+def save_to_csv_or_h5(kpt_list, output_folder, video_name, to_csv, to_h5):
+    '''
+    Saves blazepose keypoint coordinates to csv or h5 file, 
+    in the DeepLabCut format.
+
+    INPUTS:
+    - kpt_list: List of lists of keypoints X and Y coordinates and likelihood, for each frame
+    - output_folder: Folder where to save the csv or h5 file
+    - video_name: Name of the video
+    - to_csv: Boolean, whether to save to csv
+    - to_h5: Boolean, whether to save to h5
+
+    OUTPUTS:
+    - Creation of csv or h5 file in output_folder
+    '''
+    
+    # Prepare dataframe file
+    scorer = ['DavidPagnon']*len(mp_pose.PoseLandmark)*3
+    individuals = ['person']*len(mp_pose.PoseLandmark)*3
+    bodyparts = [[p]*3 for p in ['Nose', 'LEyeInner', 'LEye', 'LEyeOuter', 'REyeInner', 'REye', 'REyeOuter', 'LEar', 'REar', 'LMouth', 'RMouth', 'LShoulder', 'RShoulder', 'LElbow', 'RElbow', 'LWrist', 'RWrist', 'LPinky', 'RPinky', 'LIndex', 'RIndex', 'LThumb', 'RThumb', 'LHip', 'RHip', 'LKnee', 'RKnee', 'LAnkle', 'RAnkle', 'LHeel', 'RHeel', 'LBigToe', 'RBigToe']]
+    bodyparts = [item for sublist in bodyparts for item in sublist]
+    coords = ['x', 'y', 'likelihood']*len(mp_pose.PoseLandmark)
+
+    tuples = list(zip(scorer, individuals, bodyparts, coords))
+    index_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'bodyparts', 'coords'])
+    df = pd.DataFrame(np.array(kpt_list).T, index=index_csv).T
+
+    if to_csv:
+        csv_file = os.path.join(output_folder, video_name+'_BLAZEPOSE_points.csv')
+        logging.info(f'Saving csv file in {csv_file}.')
+        df.to_csv(csv_file, sep=',', index=True, lineterminator='\n')
+
+    if to_h5:
+        h5_file = os.path.join(output_folder, video_name+'_BLAZEPOSE_points.h5')
+        df.to_hdf(h5_file, index=True, key='BLAZEPOSE_detection')
+
+
+def save_to_json(kpt_list, output_folder, video_name):
+    '''
+    Saves blazepose keypoint coordinates to json file, 
+    in the OpenPose format.
+
+    INPUTS:
+    - kpt_list: List of lists of keypoints X and Y coordinates and likelihood, for each frame
+    - output_folder: Folder where to save the csv or h5 file
+    - video_name: Name of the video
+
+    OUTPUTS:
+    - Creation of json files in output_folder/json_folder    
+    '''
+
+    json_folder = os.path.join(output_folder, video_name + '_BLAZEPOSE_json')
+    if not os.path.exists(json_folder):
+        os.mkdir(json_folder)
+
+    # json preparation
+    json_dict = {'version':1.3, 'people':[]}
+    json_dict['people'] = [{'person_id':[-1], 
+                    'pose_keypoints_2d': [], 
+                    'face_keypoints_2d': [], 
+                    'hand_left_keypoints_2d':[], 
+                    'hand_right_keypoints_2d':[], 
+                    'pose_keypoints_3d':[], 
+                    'face_keypoints_3d':[], 
+                    'hand_left_keypoints_3d':[], 
+                    'hand_right_keypoints_3d':[]}]
+    
+    # write each h5 line in json file
+    for frame, kpt in enumerate(kpt_list):
+        json_dict['people'][0]['pose_keypoints_2d'] = kpt
+        json_file = os.path.join(json_folder, video_name+'_BLAZEPOSE.'+str(frame).zfill(5)+'.json')
+        with open(json_file, 'w') as js_f:
+            js_f.write(json.dumps(json_dict))
+
+
+def blazepose_detec_func(**args):
+    '''
+    Runs BlazePose (Mediapipe) on a video
+    Saves coordinates to OpenPose format (json files) or DeepLabCut format (csv or h5 table)
+    Optionally displays and saves images with keypoints overlayed
+
+    N.B.: First install mediapipe: `pip install mediapipe`
+    You may also need to install tables: `pip install tables`
+        
+    Usage: 
+    python -m Blazepose_runsave -i "<input_file>" --display --save_images --save_video --to_csv --to_h5 --to_json --model_complexity 2 -o "<output_folder>"
+    OR python -m Blazepose_runsave -i "<input_file>" --display --to_json --save_images
+    OR python -m Blazepose_runsave -i "<input_file>" -dJs
+    OR from Pose2Sim.Utilities import Blazepose_runsave; Blazepose_runsave.blazepose_detec_func(input_file=r'input_file', save_images=True, to_json=True, model_complexity=2)
+    '''
+
+    # Retrieve arguments
+    video_input = os.path.realpath(args.get('input_file'))
+    video_dir = os.path.dirname(video_input)
+    video_name = os.path.splitext(os.path.basename(video_input))[0]
+    output_folder = args.get('output_folder')
+
+    display = args.get('display')
+    save_images = args.get('save_images')
+    save_video = args.get('save_video')
+
+    to_csv = args.get('to_csv')
+    to_h5 = args.get('to_h5')
+    to_json = args.get('to_json')
+    
+    model_complexity = int(args.get('model_complexity'))
+    if 'model_complexity' not in vars(): model_complexity=2
+
+    if to_csv or to_h5 or to_json or save_images or save_video:
+        if output_folder == None: 
+            output_folder = video_dir
+        if not os.path.exists(os.path.realpath(output_folder)):
+            os.mkdir(os.path.realpath(output_folder))
+    
+    # Run Blazepose
+    cap = cv2.VideoCapture(video_input)
+    W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
+    fps = cap.get(cv2.CAP_PROP_FPS)
+    count = 0
+    kpt_list = []
+    with mp_pose.Pose(min_detection_confidence=0.5, min_tracking_confidence=0.5, model_complexity=model_complexity) as pose:
+        logging.info(f'Detecting 2D joint positions with BlazePose for {video_input}.')
+        logging.info('Only one person can be detected by BlazePose. No interpolation nor filtering options available. Not plotting available.')
+        if save_images and save_video:
+            logging.info(f'Saving images and video in {output_folder}.')
+        if save_images and not save_video:
+            logging.info(f'Saving images in {output_folder}.')
+        if not save_images and save_video:
+            logging.info(f'Saving video in {output_folder}.')
+
+        while cap.isOpened():
+            ret, frame = cap.read()
+            if ret == True:  
+                # Blazepose detection
+                results = pose.process(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB))            
+                try:
+                    kpt = [[p.x*W, p.y*H, p.visibility] for p in results.pose_landmarks.landmark]
+                    kpt = [item for sublist in kpt for item in sublist]  
+
+                    mp_drawing.draw_landmarks(frame, results.pose_landmarks, mp_pose.POSE_CONNECTIONS, landmark_drawing_spec=mp_drawing_styles.get_default_pose_landmarks_style())
+                except:
+                    print(f'No person detected by BlazePose on frame {count}')
+                    kpt=[np.nan*3*33]
+
+                # Display images
+                if display: 
+                    cv2.imshow('frame', frame)
+                    if cv2.waitKey(30) & 0xFF == ord('q'):
+                        break
+
+                # Save images
+                if save_images: 
+                    images_folder = os.path.join(output_folder, video_name + '_BLAZEPOSE_img')
+                    if not os.path.exists(images_folder):
+                        os.mkdir(images_folder)
+                    cv2.imwrite(os.path.join(images_folder, video_name+'_BLAZEPOSE.'+str(count).zfill(5)+'.png'), frame)
+
+                # Save video
+                if save_video:
+                    if count == 0:
+                        fourcc = cv2.VideoWriter_fourcc(*'mp4v')
+                        writer = cv2.VideoWriter(os.path.join(output_folder, video_name+'_BLAZEPOSE.mp4'), fourcc, fps, (int(W), int(H)))
+                    writer.write(frame)
+
+                # Store coordinates
+                if to_csv or to_h5 or to_json:
+                    kpt_list.append(kpt)
+
+                count += 1
+                
+            else:
+                break
+
+        cap.release()
+        if save_video:
+            writer.release()    
+        cv2.destroyAllWindows()
+
+    # Save coordinates
+    if to_csv or to_h5:
+        save_to_csv_or_h5(kpt_list, output_folder, video_name, to_csv, to_h5)
+   
+    if to_json:
+        save_to_json(kpt_list, output_folder, video_name)
+    
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-i', '--input_file', required = True, help='input video file')
+    parser.add_argument('-C', '--to_csv', required=False, action='store_true', help='save coordinates to csv')
+    parser.add_argument('-H', '--to_h5', required=False, action='store_true', help='save coordinates to h5')
+    parser.add_argument('-J', '--to_json', required=False, action='store_true', help='save coordinates to json')
+    parser.add_argument('-d', '--display', required = False, action='store_true', help='display images with overlayed coordinates')
+    parser.add_argument('-s', '--save_images', required = False, action='store_true', help='save images with overlayed coordinates')
+    parser.add_argument('-v', '--save_video', required = False, action='store_true', help='save video with overlayed coordinates')
+    parser.add_argument('-m', '--model_complexity', required = False, default = 2, help='model complexity. 0: fastest but less accurate, 2: most accurate but slowest')
+    parser.add_argument('-o', '--output_folder', required=False, help='output folder for coordinates and images')
+    
+    args = vars(parser.parse_args())
+    
+    blazepose_detec_func(**args)
```

### Comparing `sports2d-0.0.2/Sports2D/Utilities/common.py` & `sports2d-0.0.5/Sports2D/Utilities/common.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-
-'''
-    ##################################################
-    ## Common classes and functions                 ##
-    ##################################################
-    
-    - A class for displaying several matplotlib figures in tabs.
-    - A function for interpolating sequences with missing data. 
-    It does not interpolate sequences of more than N contiguous missing data.
-
-'''
-
-
-## INIT
-import sys
-import numpy as np
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
-from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
-from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, QTabWidget, QVBoxLayout
-from scipy import interpolate
-
-
-## AUTHORSHIP INFORMATION
-__author__ = "David Pagnon"
-__copyright__ = "Copyright 2023, Sports2D"
-__credits__ = ["David Pagnon"]
-__license__ = "BSD 3-Clause License"
-__version__ = "0.1"
-__maintainer__ = "David Pagnon"
-__email__ = "contact@david-pagnon.com"
-__status__ = "Development"
-
-
-## CLASSES
-class plotWindow():
-    '''
-    Display several figures in tabs
-    Taken from https://github.com/superjax/plotWindow/blob/master/plotWindow.py
-
-    USAGE:
-    pw = plotWindow()
-    f = plt.figure()
-    plt.plot(x1, y1)
-    pw.addPlot("1", f)
-    f = plt.figure()
-    plt.plot(x2, y2)
-    pw.addPlot("2", f)
-    '''
-
-    def __init__(self, parent=None):
-        self.app = QApplication(sys.argv)
-        self.MainWindow = QMainWindow()
-        self.MainWindow.__init__()
-        self.MainWindow.setWindowTitle("Multitabs figure")
-        self.canvases = []
-        self.figure_handles = []
-        self.toolbar_handles = []
-        self.tab_handles = []
-        self.current_window = -1
-        self.tabs = QTabWidget()
-        self.MainWindow.setCentralWidget(self.tabs)
-        self.MainWindow.resize(1280, 720)
-        self.MainWindow.show()
-
-    def addPlot(self, title, figure):
-        new_tab = QWidget()
-        layout = QVBoxLayout()
-        new_tab.setLayout(layout)
-
-        figure.subplots_adjust(left=0.1, right=0.99, bottom=0.1, top=0.91, wspace=0.2, hspace=0.2)
-        new_canvas = FigureCanvas(figure)
-        new_toolbar = NavigationToolbar(new_canvas, new_tab)
-
-        layout.addWidget(new_canvas)
-        layout.addWidget(new_toolbar)
-        self.tabs.addTab(new_tab, title)
-
-        self.toolbar_handles.append(new_toolbar)
-        self.canvases.append(new_canvas)
-        self.figure_handles.append(figure)
-        self.tab_handles.append(new_tab)
-
-    def show(self):
-        self.app.exec_() 
-        
-        
-## FUNCTIONS
-def interpolate_zeros_nans(col, *args):
-    '''
-    Interpolate missing points (of value zero),
-    unless more than N contiguous values are missing.
-
-    INPUTS:
-    - col: pandas column of coordinates
-    - args[0] = N: max number of contiguous bad values, above which they won't be interpolated
-    - args[1] = kind: 'linear', 'slinear', 'quadratic', 'cubic'. Default: 'cubic'
-
-    OUTPUT:
-    - col_interp: interpolated pandas column
-    '''
-
-    if len(args)==2:
-        N, kind = args
-    if len(args)==1:
-        N = np.inf
-        kind = args[0]
-    if not args:
-        N = np.inf
-    
-    # Interpolate nans
-    mask = ~(np.isnan(col) | col.eq(0)) # true where nans or zeros
-    idx_good = np.where(mask)[0]
-    if len(idx_good)>5:
-        if 'kind' not in locals(): # 'linear', 'slinear', 'quadratic', 'cubic'
-            f_interp = interpolate.interp1d(idx_good, col[idx_good], kind="linear", fill_value='extrapolate', bounds_error=False)
-        else:
-            f_interp = interpolate.interp1d(idx_good, col[idx_good], kind=kind, fill_value='extrapolate', bounds_error=False)
-        col_interp = np.where(mask, col, f_interp(col.index)) #replace at false index with interpolated values
-    
-        # Reintroduce nans if lenght of sequence > N
-        idx_notgood = np.where(~mask)[0]
-        gaps = np.where(np.diff(idx_notgood) > 1)[0] + 1 # where the indices of true are not contiguous
-        sequences = np.split(idx_notgood, gaps)
-        if sequences[0].size>0:
-            for seq in sequences:
-                if len(seq) > N: # values to exclude from interpolation are set to false when they are too long 
-                    col_interp[seq] = np.nan
-                    
-    else:
-        col_interp = col.copy()
-    
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+
+'''
+    ##################################################
+    ## Common classes and functions                 ##
+    ##################################################
+    
+    - A class for displaying several matplotlib figures in tabs.
+    - A function for interpolating sequences with missing data. 
+    It does not interpolate sequences of more than N contiguous missing data.
+
+'''
+
+
+## INIT
+import sys
+import numpy as np
+from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
+from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, QTabWidget, QVBoxLayout
+from scipy import interpolate
+
+
+## AUTHORSHIP INFORMATION
+__author__ = "David Pagnon"
+__copyright__ = "Copyright 2023, Sports2D"
+__credits__ = ["David Pagnon"]
+__license__ = "BSD 3-Clause License"
+__version__ = "0.1"
+__maintainer__ = "David Pagnon"
+__email__ = "contact@david-pagnon.com"
+__status__ = "Development"
+
+
+## CLASSES
+class plotWindow():
+    '''
+    Display several figures in tabs
+    Taken from https://github.com/superjax/plotWindow/blob/master/plotWindow.py
+
+    USAGE:
+    pw = plotWindow()
+    f = plt.figure()
+    plt.plot(x1, y1)
+    pw.addPlot("1", f)
+    f = plt.figure()
+    plt.plot(x2, y2)
+    pw.addPlot("2", f)
+    '''
+
+    def __init__(self, parent=None):
+        self.app = QApplication(sys.argv)
+        self.MainWindow = QMainWindow()
+        self.MainWindow.__init__()
+        self.MainWindow.setWindowTitle("Multitabs figure")
+        self.canvases = []
+        self.figure_handles = []
+        self.toolbar_handles = []
+        self.tab_handles = []
+        self.current_window = -1
+        self.tabs = QTabWidget()
+        self.MainWindow.setCentralWidget(self.tabs)
+        self.MainWindow.resize(1280, 720)
+        self.MainWindow.show()
+
+    def addPlot(self, title, figure):
+        new_tab = QWidget()
+        layout = QVBoxLayout()
+        new_tab.setLayout(layout)
+
+        figure.subplots_adjust(left=0.1, right=0.99, bottom=0.1, top=0.91, wspace=0.2, hspace=0.2)
+        new_canvas = FigureCanvas(figure)
+        new_toolbar = NavigationToolbar(new_canvas, new_tab)
+
+        layout.addWidget(new_canvas)
+        layout.addWidget(new_toolbar)
+        self.tabs.addTab(new_tab, title)
+
+        self.toolbar_handles.append(new_toolbar)
+        self.canvases.append(new_canvas)
+        self.figure_handles.append(figure)
+        self.tab_handles.append(new_tab)
+
+    def show(self):
+        self.app.exec_() 
+        
+        
+## FUNCTIONS
+def interpolate_zeros_nans(col, *args):
+    '''
+    Interpolate missing points (of value zero),
+    unless more than N contiguous values are missing.
+
+    INPUTS:
+    - col: pandas column of coordinates
+    - args[0] = N: max number of contiguous bad values, above which they won't be interpolated
+    - args[1] = kind: 'linear', 'slinear', 'quadratic', 'cubic'. Default: 'cubic'
+
+    OUTPUT:
+    - col_interp: interpolated pandas column
+    '''
+
+    if len(args)==2:
+        N, kind = args
+    if len(args)==1:
+        N = np.inf
+        kind = args[0]
+    if not args:
+        N = np.inf
+    
+    # Interpolate nans
+    mask = ~(np.isnan(col) | col.eq(0)) # true where nans or zeros
+    idx_good = np.where(mask)[0]
+    if len(idx_good)>5:
+        if 'kind' not in locals(): # 'linear', 'slinear', 'quadratic', 'cubic'
+            f_interp = interpolate.interp1d(idx_good, col[idx_good], kind="linear", fill_value='extrapolate', bounds_error=False)
+        else:
+            f_interp = interpolate.interp1d(idx_good, col[idx_good], kind=kind, fill_value='extrapolate', bounds_error=False)
+        col_interp = np.where(mask, col, f_interp(col.index)) #replace at false index with interpolated values
+    
+        # Reintroduce nans if lenght of sequence > N
+        idx_notgood = np.where(~mask)[0]
+        gaps = np.where(np.diff(idx_notgood) > 1)[0] + 1 # where the indices of true are not contiguous
+        sequences = np.split(idx_notgood, gaps)
+        if sequences[0].size>0:
+            for seq in sequences:
+                if len(seq) > N: # values to exclude from interpolation are set to false when they are too long 
+                    col_interp[seq] = np.nan
+                    
+    else:
+        col_interp = col.copy()
+    
     return col_interp
```

### Comparing `sports2d-0.0.2/Sports2D/Utilities/filter.py` & `sports2d-0.0.5/Sports2D/Utilities/filter.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-
-'''
-    ##################################################
-    ## Filter TRC files                             ##
-    ##################################################
-    
-    Filters pandans columns or numpy arrays.
-    Available filters: Butterworth, Gaussian, LOESS, Median.
-    
-    Usage: 
-    col_filtered = filter1d(col, *filter_options)
-    filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
-                        bool        str             int                         int                    int         int                     int                 int
-    
-'''
-
-
-## INIT
-import numpy as np
-from scipy import signal
-from scipy.ndimage import gaussian_filter1d
-from statsmodels.nonparametric.smoothers_lowess import lowess
-
-
-## AUTHORSHIP INFORMATION
-__author__ = "David Pagnon"
-__copyright__ = "Copyright 2021, Pose2Sim"
-__credits__ = ["David Pagnon"]
-__license__ = "BSD 3-Clause License"
-__version__ = "0.1"
-__maintainer__ = "David Pagnon"
-__email__ = "contact@david-pagnon.com"
-__status__ = "Development"
-
-
-
-## FUNCTIONS
-def butterworth_filter_1d(col, args):
-    '''
-    1D Zero-phase Butterworth filter (dual pass)
-    Deals with nans
-
-    INPUT:
-    - col: numpy array
-    - order: int
-    - cutoff: int
-    - framerate: int
-
-    OUTPUT
-    - col_filtered: Filtered pandas dataframe column
-    '''
-
-    order, cutoff, framerate = args
-    
-    b, a = signal.butter(order/2, cutoff/(framerate/2), 'low', analog = False) 
-    padlen = 3 * max(len(a), len(b))
-    
-    # split into sequences of not nans
-    col_filtered = col.copy()
-    mask = np.isnan(col_filtered) | col_filtered.eq(0)
-    falsemask_indices = np.where(~mask)[0]
-    gaps = np.where(np.diff(falsemask_indices) > 1)[0] + 1 
-    idx_sequences = np.split(falsemask_indices, gaps)
-    if idx_sequences[0].size > 0:
-        idx_sequences_to_filter = [seq for seq in idx_sequences if len(seq) > padlen]
-    
-        # Filter each of the selected sequences
-        for seq_f in idx_sequences_to_filter:
-            col_filtered[seq_f] = signal.filtfilt(b, a, col_filtered[seq_f])
-    
-    return col_filtered
-
-
-def gaussian_filter_1d(col, kernel):
-    '''
-    1D Gaussian filter
-
-    INPUT:
-    - col: numpy array
-    - kernel: Sigma kernel value (int)
-
-    OUTPUT
-    - col_filtered: Filtered pandas dataframe column
-    '''
-
-    col_filtered = gaussian_filter1d(col, kernel)
-
-    return col_filtered
-    
-
-def loess_filter_1d(col, kernel):
-    '''
-    1D LOWESS filter (Locally Weighted Scatterplot Smoothing)
-
-    INPUT:
-    - col: numpy array
-    - kernel: Kernel value: window length used for smoothing (int)
-    NB: frac = kernel / frames_number
-
-    OUTPUT
-    - col_filtered: Filtered pandas dataframe column
-    '''
-    
-    # split into sequences of not nans
-    col_filtered = col.copy()
-    mask = np.isnan(col_filtered) 
-    falsemask_indices = np.where(~mask)[0]
-    gaps = np.where(np.diff(falsemask_indices) > 1)[0] + 1 
-    idx_sequences = np.split(falsemask_indices, gaps)
-    if idx_sequences[0].size > 0:
-        idx_sequences_to_filter = [seq for seq in idx_sequences if len(seq) > kernel]
-    
-        # Filter each of the selected sequences
-        for seq_f in idx_sequences_to_filter:
-            col_filtered[seq_f] = lowess(col_filtered[seq_f], seq_f, is_sorted=True, frac=kernel/len(seq_f), it=0)[:,1]
-    
-    return col_filtered
-    
-
-def median_filter_1d(col, kernel):
-    '''
-    1D median filter
-
-    INPUT:
-    - col: numpy array
-    - kernel: window size (int)
-    
-    OUTPUT
-    - col_filtered: Filtered pandas dataframe column
-    '''
-    
-    col_filtered = signal.medfilt(col, kernel_size=kernel)
-
-    return col_filtered
-    
-
-def filter1d(col, *filter_options):
-    '''
-    Choose filter type and filter column
-
-    INPUT:
-    - col: Pandas dataframe column
-    - filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
-    
-    OUTPUT
-    - col_filtered: Filtered pandas dataframe column
-    '''
-    
-    filter_type = filter_options[1]
-    if filter_type == 'butterworth':
-        args = (filter_options[2], filter_options[3], filter_options[4])
-    if filter_type == 'gaussian':
-        args = (filter_options[5])
-    if filter_type == 'loess':
-        args = (filter_options[6])
-    if filter_type == 'median':
-        args = (filter_options[7])
-        
-    # Choose filter
-    filter_mapping = {
-        'butterworth': butterworth_filter_1d, 
-        'gaussian': gaussian_filter_1d, 
-        'loess': loess_filter_1d, 
-        'median': median_filter_1d
-        }
-    filter_fun = filter_mapping[filter_type]
-    
-    # Filter column
-    col_filtered = filter_fun(col, args)
-
-    return col_filtered
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+
+'''
+    ##################################################
+    ## Filter TRC files                             ##
+    ##################################################
+    
+    Filters pandans columns or numpy arrays.
+    Available filters: Butterworth, Gaussian, LOESS, Median.
+    
+    Usage: 
+    col_filtered = filter1d(col, *filter_options)
+    filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
+                        bool        str             int                         int                    int         int                     int                 int
+    
+'''
+
+
+## INIT
+import numpy as np
+from scipy import signal
+from scipy.ndimage import gaussian_filter1d
+from statsmodels.nonparametric.smoothers_lowess import lowess
+
+
+## AUTHORSHIP INFORMATION
+__author__ = "David Pagnon"
+__copyright__ = "Copyright 2021, Pose2Sim"
+__credits__ = ["David Pagnon"]
+__license__ = "BSD 3-Clause License"
+__version__ = "0.1"
+__maintainer__ = "David Pagnon"
+__email__ = "contact@david-pagnon.com"
+__status__ = "Development"
+
+
+
+## FUNCTIONS
+def butterworth_filter_1d(col, args):
+    '''
+    1D Zero-phase Butterworth filter (dual pass)
+    Deals with nans
+
+    INPUT:
+    - col: numpy array
+    - order: int
+    - cutoff: int
+    - framerate: int
+
+    OUTPUT
+    - col_filtered: Filtered pandas dataframe column
+    '''
+
+    order, cutoff, framerate = args
+    
+    b, a = signal.butter(order/2, cutoff/(framerate/2), 'low', analog = False) 
+    padlen = 3 * max(len(a), len(b))
+    
+    # split into sequences of not nans
+    col_filtered = col.copy()
+    mask = np.isnan(col_filtered) | col_filtered.eq(0)
+    falsemask_indices = np.where(~mask)[0]
+    gaps = np.where(np.diff(falsemask_indices) > 1)[0] + 1 
+    idx_sequences = np.split(falsemask_indices, gaps)
+    if idx_sequences[0].size > 0:
+        idx_sequences_to_filter = [seq for seq in idx_sequences if len(seq) > padlen]
+    
+        # Filter each of the selected sequences
+        for seq_f in idx_sequences_to_filter:
+            col_filtered[seq_f] = signal.filtfilt(b, a, col_filtered[seq_f])
+    
+    return col_filtered
+
+
+def gaussian_filter_1d(col, kernel):
+    '''
+    1D Gaussian filter
+
+    INPUT:
+    - col: numpy array
+    - kernel: Sigma kernel value (int)
+
+    OUTPUT
+    - col_filtered: Filtered pandas dataframe column
+    '''
+
+    col_filtered = gaussian_filter1d(col, kernel)
+
+    return col_filtered
+    
+
+def loess_filter_1d(col, kernel):
+    '''
+    1D LOWESS filter (Locally Weighted Scatterplot Smoothing)
+
+    INPUT:
+    - col: numpy array
+    - kernel: Kernel value: window length used for smoothing (int)
+    NB: frac = kernel / frames_number
+
+    OUTPUT
+    - col_filtered: Filtered pandas dataframe column
+    '''
+    
+    # split into sequences of not nans
+    col_filtered = col.copy()
+    mask = np.isnan(col_filtered) 
+    falsemask_indices = np.where(~mask)[0]
+    gaps = np.where(np.diff(falsemask_indices) > 1)[0] + 1 
+    idx_sequences = np.split(falsemask_indices, gaps)
+    if idx_sequences[0].size > 0:
+        idx_sequences_to_filter = [seq for seq in idx_sequences if len(seq) > kernel]
+    
+        # Filter each of the selected sequences
+        for seq_f in idx_sequences_to_filter:
+            col_filtered[seq_f] = lowess(col_filtered[seq_f], seq_f, is_sorted=True, frac=kernel/len(seq_f), it=0)[:,1]
+    
+    return col_filtered
+    
+
+def median_filter_1d(col, kernel):
+    '''
+    1D median filter
+
+    INPUT:
+    - col: numpy array
+    - kernel: window size (int)
+    
+    OUTPUT
+    - col_filtered: Filtered pandas dataframe column
+    '''
+    
+    col_filtered = signal.medfilt(col, kernel_size=kernel)
+
+    return col_filtered
+    
+
+def filter1d(col, *filter_options):
+    '''
+    Choose filter type and filter column
+
+    INPUT:
+    - col: Pandas dataframe column
+    - filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
+    
+    OUTPUT
+    - col_filtered: Filtered pandas dataframe column
+    '''
+    
+    filter_type = filter_options[1]
+    if filter_type == 'butterworth':
+        args = (filter_options[2], filter_options[3], filter_options[4])
+    if filter_type == 'gaussian':
+        args = (filter_options[5])
+    if filter_type == 'loess':
+        args = (filter_options[6])
+    if filter_type == 'median':
+        args = (filter_options[7])
+        
+    # Choose filter
+    filter_mapping = {
+        'butterworth': butterworth_filter_1d, 
+        'gaussian': gaussian_filter_1d, 
+        'loess': loess_filter_1d, 
+        'median': median_filter_1d
+        }
+    filter_fun = filter_mapping[filter_type]
+    
+    # Filter column
+    col_filtered = filter_fun(col, args)
+
+    return col_filtered
```

### Comparing `sports2d-0.0.2/Sports2D/compute_angles.py` & `sports2d-0.0.5/Sports2D/compute_angles.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,501 +1,501 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-
-'''
-    ##############################################################
-    ## Compute joint and segment angles from csv position files ##
-    ##############################################################
-
-    Compute joint and segment angles from csv position files.
-    Automatically adjust angles when person switches to face the other way.
-    Save a 2D csv angle file per person.
-    Optionally filters results with Butterworth, gaussian, median, or loess filter.
-    Optionally displays figures.
-    Optionally saves images and video with overlaid angles.
-
-    Joint angle conventions:
-    - Ankle dorsiflexion: Between heel and big toe, and ankle and knee
-    - Knee flexion: Between hip, knee, and ankle 
-    - Hip flexion: Between knee, hip, and shoulder
-    - Shoulder flexion: Between hip, shoulder, and elbow
-    - Elbow flexion: Between wrist, elbow, and shoulder
-
-    Segment angle conventions:
-    Angles are measured anticlockwise between the horizontal and the segment.
-    - Foot: Between heel and big toe
-    - Shank: Between ankle and knee
-    - Thigh: Between hip and knee
-    - Arm: Between shoulder and elbow
-    - Forearm: Between elbow and wrist
-    - Trunk: Between hip midpoint and shoulder midpoint
-    
-    /!\ Warning /!\
-    - The angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.
-    - It will lead to reliable results only if the persons move in the 2D plane (sagittal plane).
-    - The persons need to be filmed as perpendicularly as possible from their side.
-    If you need research-grade markerless joint kinematics, consider using several cameras,
-    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
-    https://github.com/perfanalytics/pose2sim
-    
-    INPUTS:
-    - one or several position csv files
-    - a dictionary obtained from a configuration file (.toml extension)
-    - a skeleton model
-    
-    OUTPUTS:
-    - one csv file for joint and segment angles per detected person
-    - a logs.txt file 
-
-'''    
-
-
-## INIT
-import logging
-import os
-from pathlib import Path
-import pandas as pd
-import numpy as np
-import cv2
-import matplotlib.pyplot as plt
-from Sports2D.Sports2D import base_params
-from Sports2D.Utilities import filter, common
-from Sports2D.Utilities.skeletons import *
-
-
-## AUTHORSHIP INFORMATION
-__author__ = "David Pagnon"
-__copyright__ = "Copyright 2023, Sports2D"
-__credits__ = ["David Pagnon"]
-__license__ = "BSD 3-Clause License"
-__version__ = "0.1"
-__maintainer__ = "David Pagnon"
-__email__ = "contact@david-pagnon.com"
-__status__ = "Development"
-
-
-
-# CONSTANTS
-# dict: name: points, extra, offset, invert. 
-# Most angles are multiplied by -1 because the OpenCV y axis points down.
-joint_angle_dict = { 
-    'Right ankle': [['RHeel', 'RBigToe', 'RAnkle', 'RKnee'], 'dorsiflexion', -90, -1],
-    'Left ankle': [['LHeel', 'LBigToe', 'LAnkle', 'LKnee'], 'dorsiflexion', -90, -1],
-    'Right knee': [['RHip', 'RKnee', 'RAnkle'], 'flexion', -180, -1],
-    'Left knee': [['LHip', 'LKnee', 'LAnkle'], 'flexion', -180, -1],
-    'Right hip': [['RKnee', 'RHip', 'RShoulder'], 'flexion', -180, -1],
-    'Left hip': [['LKnee', 'LHip', 'LShoulder'], 'flexion', -180, -1],
-    'Right shoulder': [['RHip', 'RShoulder', 'RElbow'], 'flexion', 0, 1],
-    'Left shoulder': [['LHip', 'LShoulder', 'LElbow'], 'flexion', 0, 1],
-    'Right elbow': [['RWrist', 'RElbow', 'RShoulder'], 'flexion', -180, -1],
-    'Left elbow': [['LWrist', 'LElbow', 'LShoulder'], 'flexion', -180, -1],
-    'Right wrist': [['RIndex', 'RWrist', 'RElbow'], 'flexion', -180, -1],
-    'Left wrist': [['LIndex', 'LWrist', 'LElbow'], 'flexion', -180, -1]
-    }
-
-segment_angle_dict = {     
-    'Right foot': [['RHeel', 'RBigToe'], 'horizontal', 0, -1],
-    'Left foot': [['LHeel', 'LBigToe'], 'horizontal', 0, -1],
-    'Right shank': [['RKnee', 'RAnkle'], 'horizontal', 0, -1],
-    'Left shank': [['LKnee', 'LAnkle'], 'horizontal', 0, -1],
-    'Right thigh': [['RHip', 'RKnee'], 'horizontal', 0, -1],
-    'Left thigh': [['LHip', 'LKnee'], 'horizontal', 0, -1],
-    'Trunk': [['RShoulder', 'RHip'], 'horizontal', 0, 1],
-    'Right arm': [['RShoulder', 'RElbow'], 'horizontal', 0, -1],
-    'Left arm': [['LShoulder', 'LElbow'], 'horizontal', 0, -1],
-    'Right forearm': [['RElbow', 'RWrist'], 'horizontal', 0, -1],
-    'Left forearm': [['LElbow', 'LWrist'], 'horizontal', 0, -1],
-    'Right hand': [['RWrist', 'RIndex'], 'horizontal', 0, -1],
-    'Left hand': [['LWrist', 'LIndex'], 'horizontal', 0, -1]
-    }
-    
-
-# FUNCTIONS
-def display_figures_fun(df_list):
-    '''
-    Displays filtered and unfiltered data for comparison
-    /!\ Crashes on the third window...
-
-    INPUTS:
-    - df_list: list of dataframes of angles
-
-    OUTPUT:
-    - matplotlib window with tabbed figures for each angle
-    '''
-    
-    angle_names = df_list[0].columns.get_level_values(2)
-    
-    pw = common.plotWindow()
-    for id, angle in enumerate(angle_names): # angles
-        f = plt.figure()
-        
-        plt.plot()
-        [plt.plot(df_list[0].index, df.iloc[:,id], label=['unfiltered' if i==0 else 'filtered' if i==1 else ''][0]) for i,df in enumerate(df_list)]
-        plt.ylabel(angle) # nom angle
-        plt.legend()
-
-        pw.addPlot(angle, f)
-    
-    pw.show()
-    
-    
-def points2D_to_angles(points_list):
-    '''
-    If len(points_list)==2, computes clockwise angle of ab vector w.r.t. horizontal (e.g. RBigToe-RHeel) 
-    If len(points_list)==3, computes clockwise angle from a to c around b (e.g. Neck, Hip, Knee) 
-    If len(points_list)==4, computes clockwise angle between vectors ab and cd (e.g. CHip-Neck, RHip-RKnee)
-    
-    If parameters are float, returns a float between 0.0 and 360.0
-    If parameters are arrays, returns an array of floats between 0.0 and 360.0
-    '''
-    
-    ax, ay = points_list[0]
-    bx, by = points_list[1]
-    
-    if len(points_list)==2:
-        ux, uy = bx-ax, by-ay
-        vx, vy = 1,0
-
-    if len(points_list)==3:
-        cx, cy = points_list[2]
-        ux, uy = ax-bx, ay-by
-        vx, vy = cx-bx, cy-by
-    
-    if len(points_list)==4:
-        cx, cy = points_list[2]
-        dx, dy = points_list[3]
-        ux, uy = bx-ax, by-ay
-        vx, vy = dx-cx, dy-cy
-            
-    ang = np.array(np.degrees(np.arctan2(uy, ux) - np.arctan2(vy, vx)))
-    
-    return ang
-            
-
-def flip_left_right_direction(df_points):
-    '''
-    Inverts X coordinates to get consistent angles when person changes direction and goes to the left.
-    The person is deemed to go to the left when their toes are to the left of their heels.
-    
-    INPUT:
-    - df_points: dataframe of pose detection
-    
-    OUTPUT:
-    - df_points: dataframe of pose detection with flipped X coordinates
-    '''
-    
-    righ_orientation = df_points.iloc[:,df_points.columns.get_level_values(2)=='RBigToe'].iloc[:,0] - df_points.iloc[:,df_points.columns.get_level_values(2)=='RHeel'].iloc[:,0]
-    left_orientation = df_points.iloc[:,df_points.columns.get_level_values(2)=='LBigToe'].iloc[:,0] - df_points.iloc[:,df_points.columns.get_level_values(2)=='LHeel'].iloc[:,0]
-    orientation = righ_orientation + left_orientation
-    df_points.iloc[:,1::3] = df_points.iloc[:,1::3] * np.where(orientation>=0, 1, -1).reshape(-1,1)
-    
-    return df_points
-            
-
-def joint_angles_series_from_points(df_points, angle_params):
-    '''
-    Obtain joint angle series from point series.
-    
-    INPUT: 
-    - df_points: dataframe of pose detection, from csv
-    - angle_params: dictionary specifying which points to use, and what offset and multiplying factor to use
-    
-    OUTPUT:
-    - ang_series: array of time series of the considered angle
-    '''
-    
-    # Retrieve points
-    keypt_series = []
-    for k in angle_params[0]:
-        keypt_series += [df_points.iloc[:,df_points.columns.get_level_values(2)==k].iloc[:,:2]]
-
-    # Compute angles
-    points_list = [k.values.T for k in keypt_series]
-    ang_series = points2D_to_angles(points_list)
-    ang_series += angle_params[2]
-    ang_series *= angle_params[3]
-    ang_series = np.where(ang_series>180,ang_series-360,ang_series)
-    ang_series = np.where((ang_series==0) | (ang_series==90) | (ang_series==180), +0, ang_series)
-
-    
-    return ang_series
-
-
-def segment_angles_series_from_points(df_points, angle_params, segment):
-    '''
-    Obtain segment angle series w/r horizontal from point series.
-    For trunk segment: mean of the angles between RHip-RShoulder and LHip-LShoulder
-    
-    INPUT: 
-    - df_points: dataframe of pose detection, from csv
-    - angle_params: dictionary specifying which points to use, and what offset and multiplying factor to use
-    - segment: which segment angle is considered
-    
-    OUTPUT:
-    - ang_series: array of time series of the considered angle
-    '''
-    
-    # Retrieve points
-    keypt_series = []
-    for k in angle_params[0]:
-        keypt_series += [df_points.iloc[:,df_points.columns.get_level_values(2)==k].iloc[:,:2]]
-    points_list = [k.values.T for k in keypt_series]
-    
-    # Compute angles
-    ang_series = points2D_to_angles(points_list)
-    ang_series += angle_params[2]
-    ang_series *= angle_params[3]
-    ang_series = np.where(ang_series>180,ang_series-360,ang_series)
-    
-    # For trunk: mean between angles RHip-RShoulder and LHip-LShoulder
-    if segment == 'Trunk':
-        ang_seriesR = ang_series
-        angle_params[0] = [a.replace('R','L') for a in angle_params[0]]
-        keypt_series = []
-        for k in angle_params[0]:
-            keypt_series += [df_points.iloc[:,df_points.columns.get_level_values(2)==k].iloc[:,:2]]
-        # Compute angles
-        points_list = [k.values.T for k in keypt_series]
-        ang_series = points2D_to_angles(points_list)
-        ang_series += angle_params[2]
-        ang_series *= angle_params[3]
-        ang_series = np.mean((ang_seriesR, ang_series), axis=0)
-        ang_series = np.where(ang_series>180,ang_series-360,ang_series)
-        
-    return ang_series
-    
-    
-def overlay_angles(frame, df_angles_list_frame):
-    '''
-    Overlays a text box for each detected person with joint and segment angles
-    
-    INPUT:
-    - frame: a frame opened with OpenCV
-    - df_angles_list_frame: list of one frame for all angles
-    '''
-    
-    cmap = plt.cm.hsv
-    font = cv2.FONT_HERSHEY_SIMPLEX
-    for i, angles_frame_person in enumerate(df_angles_list_frame):
-        for ang_nb in range(len(angles_frame_person)):
-            # Angle label
-            frame = cv2.putText(frame, 
-                angles_frame_person.index[ang_nb][2] + ':',
-                (10+250*i, 15+15*ang_nb), 
-                font, 0.5, 
-                (np.array(cmap((i+1)/len(df_angles_list_frame)))*255).tolist(), 
-                1, 
-                cv2.LINE_4)
-            # Angle value
-            frame = cv2.putText(frame, 
-                str(round(angles_frame_person[ang_nb],1)),
-                (150+250*i, 15+15*ang_nb), 
-                font, 0.5, 
-                (np.array(cmap((i+1)/len(df_angles_list_frame)))*255).tolist(), 
-                1, 
-                cv2.LINE_4)
-            # Progress bar
-            x_ang = int(angles_frame_person[ang_nb]*50/180)
-            if x_ang > 0:
-                sub_frame = frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i : 170+250*i+x_ang ]
-                white_rect = np.ones(sub_frame.shape, dtype=np.uint8) * 255
-                res = cv2.addWeighted(sub_frame, 0.6, white_rect, 0.4, 1.0)
-                frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i : 170+250*i+x_ang ] = res
-            elif x_ang < 0:
-                sub_frame = frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i+x_ang : 170+250*i ]
-                white_rect = np.ones(sub_frame.shape, dtype=np.uint8) * 255
-                res = cv2.addWeighted(sub_frame, 0.6, white_rect, 0.4, 1.0)
-                frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i+x_ang : 170+250*i ] = res
-        
-    return frame
-    
-    
-def compute_angles_fun(config_dict):
-    '''
-    Compute joint and segment angles from csv position files.
-    Automatically adjust angles when person switches to face the other way.
-    Save a 2D csv angle file per person.
-    Optionally filters results with Butterworth, gaussian, median, or loess filter.
-    Optionally displays figures.
-
-    Joint angle conventions:
-    - Ankle dorsiflexion: Between heel and big toe, and ankle and knee
-    - Knee flexion: Between hip, knee, and ankle 
-    - Hip flexion: Between knee, hip, and shoulder
-    - Shoulder flexion: Between hip, shoulder, and elbow
-    - Elbow flexion: Between wrist, elbow, and shoulder
-
-    Segment angle conventions:
-    Angles are measured anticlockwise between the horizontal and the segment.
-    - Foot: Between heel and big toe
-    - Shank: Between ankle and knee
-    - Thigh: Between hip and knee
-    - Arm: Between shoulder and elbow
-    - Forearm: Between elbow and wrist
-    - Trunk: Between hip midpoint and shoulder midpoint
-    
-    /!\ Warning /!\
-    - The angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.
-    - It will lead to reliable results only if the persons move in the 2D plane (sagittal plane).
-    - The persons need to be filmed as perpendicularly as possible from their side.
-    If you need research-grade markerless joint kinematics, consider using several cameras,
-    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
-    https://github.com/perfanalytics/pose2sim
-
-    INPUTS:
-    - one or several position csv files
-    - a dictionary obtained from a configuration file (.toml extension)
-    - a skeleton model
-    
-    OUTPUTS:
-    - one csv file for joint and segment angles per detected person
-    - a logs.txt file 
-    '''
-    
-    # Retrieve parameters
-    video_dir, video_file, frame_rate = base_params(config_dict)
-    pose_algo = config_dict.get('pose').get('pose_algo')
-    if pose_algo == 'OPENPOSE':
-        pose_model = config_dict.get('pose').get('OPENPOSE').get('openpose_model')
-    elif pose_algo == 'BLAZEPOSE':
-        pose_model = 'BLAZEPOSE'
-    joint_angles = config_dict.get('compute_angles').get('joint_angles')
-    segment_angles = config_dict.get('compute_angles').get('segment_angles')
-    angle_nb = len(joint_angles) + len(segment_angles)
-    
-    show_plots = config_dict.get('compute_angles_advanced').get('show_plots')
-    do_filter = config_dict.get('compute_angles_advanced').get('filter')
-    filter_type = config_dict.get('compute_angles_advanced').get('filter_type')
-    butterworth_filter_order = config_dict.get('compute_angles_advanced').get('butterworth').get('order')
-    butterworth_filter_cutoff = config_dict.get('compute_angles_advanced').get('butterworth').get('cut_off_frequency')
-    gaussian_filter_kernel = config_dict.get('compute_angles_advanced').get('gaussian').get('sigma_kernel')
-    loess_filter_kernel = config_dict.get('compute_angles_advanced').get('loess').get('nb_values_used')
-    median_filter_kernel = config_dict.get('compute_angles_advanced').get('median').get('kernel_size')
-    filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
-    
-    show_angles_img = config_dict.get('compute_angles_advanced').get('save_img')
-    show_angles_vid = config_dict.get('compute_angles_advanced').get('save_vid')
-    
-    # Find csv position files in video_dir, search pose_model and video_file.stem
-    logging.info(f'Retrieving csv position files in {video_dir}...')
-    csv_paths = list(video_dir.glob(f'*{video_file.stem}_{pose_model}_*points*.csv'))
-    logging.info(f'{len(csv_paths)} persons found.')
-
-    # Compute angles
-    df_angles_list = []
-    for i, c in enumerate(csv_paths):
-        # Prepare angle csv header
-        scorer = ['DavidPagnon']*angle_nb
-        individuals = [f'person{i}']*angle_nb
-        angs = joint_angles + segment_angles
-        coords = [joint_angle_dict.get(j)[1] for j in joint_angles] + [segment_angle_dict.get(s)[1] for s in segment_angles]
-        tuples = list(zip(scorer, individuals, angs, coords))
-        index_angs_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'angs', 'coords'])    
-
-        # Compute angles for each person, for each angle, with each required keypoint position
-        logging.info(f'Person {i}: Computing 2D joint and segment angles.')
-        with open(c) as c_f:
-            df_points = pd.read_csv(c_f, header=[0,1,2,3])
-            
-            # Flip along x when feet oriented to the left
-            df_points = flip_left_right_direction(df_points)
-            
-            # Joint angles
-            joint_angle_series = []
-            for j in joint_angles: 
-                angle_params = joint_angle_dict.get(j)
-                j_ang_series = joint_angles_series_from_points(df_points, angle_params)
-                joint_angle_series += [j_ang_series]
-    
-            # Segment angles
-            segment_angle_series = []
-            for s in segment_angles:
-                angle_params = segment_angle_dict.get(s)
-                s_ang_series = segment_angles_series_from_points(df_points, angle_params, s)
-                segment_angle_series += [s_ang_series]
-            
-            angle_series = joint_angle_series + segment_angle_series
-            df_angles = []
-            df_angles += [pd.DataFrame(angle_series, index=index_angs_csv).T]
-            
-            # Filter
-            if filter_options[0]:
-                filter_type = filter_options[1]
-                if filter_type == 'butterworth':
-                    args = f'Butterworth filter, {filter_options[2]}th order, {filter_options[3]} Hz.'
-                if filter_type == 'gaussian':
-                    args = f'Gaussian filter, Sigma kernel {filter_options[5]}'
-                if filter_type == 'loess':
-                    args = f'LOESS filter, window size of {filter_options[6]} frames.'
-                if filter_type == 'median':
-                    args = f'Median filter, kernel of {filter_options[7]}.'
-                logging.info(f'Person {i}: Filtering with {args}.')
-                df_angles[0].replace(0, np.nan, inplace=True)
-                df_angles += [df_angles[0].copy()]
-                df_angles[1] = df_angles[1].apply(filter.filter1d, axis=0, args=filter_options)
-            df_angles[-1].replace(np.nan, 0, inplace=True)
-               
-            # Creation of the csv files
-            csv_angle_path = c.parent / (c.stem.replace('points', 'angles') + '.csv')
-            logging.info(f'Person {i}: Saving csv angle file in {csv_angle_path}.')
-            df_angles[-1].to_csv(csv_angle_path, sep=',', index=True, lineterminator='\n')
-            
-            # Display figures
-            if show_plots:
-                logging.info(f'Person {i}: Displaying figures.')
-                display_figures_fun(df_angles)
-
-            df_angles_list += [df_angles[-1]]
-
-    # Add angles to vid and img
-    if show_angles_img or show_angles_vid:
-        video_base = Path(video_dir / video_file)
-        img_pose = video_base.parent / (video_base.stem + '_' + pose_model + '_img')
-        video_pose = video_base.parent / (video_base.stem + '_' + pose_model + '.mp4')
-        video_pose2 = video_base.parent / (video_base.stem + '_' + pose_model + '2.mp4')
-        
-        if show_angles_vid:
-            cap = [cv2.VideoCapture(str(video_pose)) if Path.exists(video_pose) else cv2.VideoCapture(str(video_base))][0]
-            fps = cap.get(cv2.CAP_PROP_FPS)
-            W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
-            fourcc = cv2.VideoWriter_fourcc(*'mp4v')
-            writer = cv2.VideoWriter(str(video_pose2), fourcc, fps, (int(W), int(H)))
-        
-        # Preferentially from pose image files
-        frames_img = list(img_pose.glob('*'))
-        if len(frames_img)>0:
-            for frame_nb in range(df_angles_list[0].shape[0]):
-                df_angles_list_frame = [df_angles_list[n].iloc[frame_nb,:] for n in range(len(df_angles_list))]
-                frame = cv2.imread(str(frames_img[frame_nb]))
-                frame = overlay_angles(frame, df_angles_list_frame)
-                if show_angles_img:
-                    cv2.imwrite(str(frames_img[frame_nb]), frame)
-                if show_angles_vid:
-                    writer.write(frame)
-            writer.release()
-                
-        # Else from pose video (or base video if pose video does not exist)
-        elif Path.exists(video_base) or Path.exists(video_pose):
-            frame_nb = 0
-            while cap.isOpened():
-                ret, frame = cap.read()
-                if ret == True:
-                    df_angles_list_frame = [df_angles_list[n].iloc[frame_nb,:] for n in range(len(df_angles_list))]
-                    frame = overlay_angles(frame, df_angles_list_frame)
-                    if show_angles_img:
-                        if frame_nb==0: img_pose.mkdir(parents=True, exist_ok=True)
-                        cv2.imwrite(str(img_pose / (video_base.stem + '_' + pose_model + '.' + str(frame_nb).zfill(5)+'.png')), frame)
-                    if show_angles_vid:
-                        writer.write(frame)
-                    frame_nb+=1
-                else:
-                    break
-        
-        cap.release()
-        writer.release()
-        if show_angles_vid:
-            if Path.exists(video_pose): os.remove(video_pose)
-            os.rename(video_pose2,video_pose)
-            if Path.exists(video_pose2): os.remove(video_pose2)
-
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+
+'''
+    ##############################################################
+    ## Compute joint and segment angles from csv position files ##
+    ##############################################################
+
+    Compute joint and segment angles from csv position files.
+    Automatically adjust angles when person switches to face the other way.
+    Save a 2D csv angle file per person.
+    Optionally filters results with Butterworth, gaussian, median, or loess filter.
+    Optionally displays figures.
+    Optionally saves images and video with overlaid angles.
+
+    Joint angle conventions:
+    - Ankle dorsiflexion: Between heel and big toe, and ankle and knee
+    - Knee flexion: Between hip, knee, and ankle 
+    - Hip flexion: Between knee, hip, and shoulder
+    - Shoulder flexion: Between hip, shoulder, and elbow
+    - Elbow flexion: Between wrist, elbow, and shoulder
+
+    Segment angle conventions:
+    Angles are measured anticlockwise between the horizontal and the segment.
+    - Foot: Between heel and big toe
+    - Shank: Between ankle and knee
+    - Thigh: Between hip and knee
+    - Arm: Between shoulder and elbow
+    - Forearm: Between elbow and wrist
+    - Trunk: Between hip midpoint and shoulder midpoint
+    
+    /!\ Warning /!\
+    - The angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.
+    - It will lead to reliable results only if the persons move in the 2D plane (sagittal plane).
+    - The persons need to be filmed as perpendicularly as possible from their side.
+    If you need research-grade markerless joint kinematics, consider using several cameras,
+    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
+    https://github.com/perfanalytics/pose2sim
+    
+    INPUTS:
+    - one or several position csv files
+    - a dictionary obtained from a configuration file (.toml extension)
+    - a skeleton model
+    
+    OUTPUTS:
+    - one csv file for joint and segment angles per detected person
+    - a logs.txt file 
+
+'''    
+
+
+## INIT
+import logging
+import os
+from pathlib import Path
+import pandas as pd
+import numpy as np
+import cv2
+import matplotlib.pyplot as plt
+from Sports2D.Sports2D import base_params
+from Sports2D.Utilities import filter, common
+from Sports2D.Utilities.skeletons import *
+
+
+## AUTHORSHIP INFORMATION
+__author__ = "David Pagnon"
+__copyright__ = "Copyright 2023, Sports2D"
+__credits__ = ["David Pagnon"]
+__license__ = "BSD 3-Clause License"
+__version__ = "0.1"
+__maintainer__ = "David Pagnon"
+__email__ = "contact@david-pagnon.com"
+__status__ = "Development"
+
+
+
+# CONSTANTS
+# dict: name: points, extra, offset, invert. 
+# Most angles are multiplied by -1 because the OpenCV y axis points down.
+joint_angle_dict = { 
+    'Right ankle': [['RHeel', 'RBigToe', 'RAnkle', 'RKnee'], 'dorsiflexion', -90, -1],
+    'Left ankle': [['LHeel', 'LBigToe', 'LAnkle', 'LKnee'], 'dorsiflexion', -90, -1],
+    'Right knee': [['RHip', 'RKnee', 'RAnkle'], 'flexion', -180, -1],
+    'Left knee': [['LHip', 'LKnee', 'LAnkle'], 'flexion', -180, -1],
+    'Right hip': [['RKnee', 'RHip', 'RShoulder'], 'flexion', -180, -1],
+    'Left hip': [['LKnee', 'LHip', 'LShoulder'], 'flexion', -180, -1],
+    'Right shoulder': [['RHip', 'RShoulder', 'RElbow'], 'flexion', 0, 1],
+    'Left shoulder': [['LHip', 'LShoulder', 'LElbow'], 'flexion', 0, 1],
+    'Right elbow': [['RWrist', 'RElbow', 'RShoulder'], 'flexion', -180, -1],
+    'Left elbow': [['LWrist', 'LElbow', 'LShoulder'], 'flexion', -180, -1],
+    'Right wrist': [['RIndex', 'RWrist', 'RElbow'], 'flexion', -180, -1],
+    'Left wrist': [['LIndex', 'LWrist', 'LElbow'], 'flexion', -180, -1]
+    }
+
+segment_angle_dict = {     
+    'Right foot': [['RHeel', 'RBigToe'], 'horizontal', 0, -1],
+    'Left foot': [['LHeel', 'LBigToe'], 'horizontal', 0, -1],
+    'Right shank': [['RKnee', 'RAnkle'], 'horizontal', 0, -1],
+    'Left shank': [['LKnee', 'LAnkle'], 'horizontal', 0, -1],
+    'Right thigh': [['RHip', 'RKnee'], 'horizontal', 0, -1],
+    'Left thigh': [['LHip', 'LKnee'], 'horizontal', 0, -1],
+    'Trunk': [['RShoulder', 'RHip'], 'horizontal', 0, 1],
+    'Right arm': [['RShoulder', 'RElbow'], 'horizontal', 0, -1],
+    'Left arm': [['LShoulder', 'LElbow'], 'horizontal', 0, -1],
+    'Right forearm': [['RElbow', 'RWrist'], 'horizontal', 0, -1],
+    'Left forearm': [['LElbow', 'LWrist'], 'horizontal', 0, -1],
+    'Right hand': [['RWrist', 'RIndex'], 'horizontal', 0, -1],
+    'Left hand': [['LWrist', 'LIndex'], 'horizontal', 0, -1]
+    }
+    
+
+# FUNCTIONS
+def display_figures_fun(df_list):
+    '''
+    Displays filtered and unfiltered data for comparison
+    /!\ Crashes on the third window...
+
+    INPUTS:
+    - df_list: list of dataframes of angles
+
+    OUTPUT:
+    - matplotlib window with tabbed figures for each angle
+    '''
+    
+    angle_names = df_list[0].columns.get_level_values(2)
+    
+    pw = common.plotWindow()
+    for id, angle in enumerate(angle_names): # angles
+        f = plt.figure()
+        
+        plt.plot()
+        [plt.plot(df_list[0].index, df.iloc[:,id], label=['unfiltered' if i==0 else 'filtered' if i==1 else ''][0]) for i,df in enumerate(df_list)]
+        plt.ylabel(angle) # nom angle
+        plt.legend()
+
+        pw.addPlot(angle, f)
+    
+    pw.show()
+    
+    
+def points2D_to_angles(points_list):
+    '''
+    If len(points_list)==2, computes clockwise angle of ab vector w.r.t. horizontal (e.g. RBigToe-RHeel) 
+    If len(points_list)==3, computes clockwise angle from a to c around b (e.g. Neck, Hip, Knee) 
+    If len(points_list)==4, computes clockwise angle between vectors ab and cd (e.g. CHip-Neck, RHip-RKnee)
+    
+    If parameters are float, returns a float between 0.0 and 360.0
+    If parameters are arrays, returns an array of floats between 0.0 and 360.0
+    '''
+    
+    ax, ay = points_list[0]
+    bx, by = points_list[1]
+    
+    if len(points_list)==2:
+        ux, uy = bx-ax, by-ay
+        vx, vy = 1,0
+
+    if len(points_list)==3:
+        cx, cy = points_list[2]
+        ux, uy = ax-bx, ay-by
+        vx, vy = cx-bx, cy-by
+    
+    if len(points_list)==4:
+        cx, cy = points_list[2]
+        dx, dy = points_list[3]
+        ux, uy = bx-ax, by-ay
+        vx, vy = dx-cx, dy-cy
+            
+    ang = np.array(np.degrees(np.arctan2(uy, ux) - np.arctan2(vy, vx)))
+    
+    return ang
+            
+
+def flip_left_right_direction(df_points):
+    '''
+    Inverts X coordinates to get consistent angles when person changes direction and goes to the left.
+    The person is deemed to go to the left when their toes are to the left of their heels.
+    
+    INPUT:
+    - df_points: dataframe of pose detection
+    
+    OUTPUT:
+    - df_points: dataframe of pose detection with flipped X coordinates
+    '''
+    
+    righ_orientation = df_points.iloc[:,df_points.columns.get_level_values(2)=='RBigToe'].iloc[:,0] - df_points.iloc[:,df_points.columns.get_level_values(2)=='RHeel'].iloc[:,0]
+    left_orientation = df_points.iloc[:,df_points.columns.get_level_values(2)=='LBigToe'].iloc[:,0] - df_points.iloc[:,df_points.columns.get_level_values(2)=='LHeel'].iloc[:,0]
+    orientation = righ_orientation + left_orientation
+    df_points.iloc[:,1::3] = df_points.iloc[:,1::3] * np.where(orientation>=0, 1, -1).reshape(-1,1)
+    
+    return df_points
+            
+
+def joint_angles_series_from_points(df_points, angle_params):
+    '''
+    Obtain joint angle series from point series.
+    
+    INPUT: 
+    - df_points: dataframe of pose detection, from csv
+    - angle_params: dictionary specifying which points to use, and what offset and multiplying factor to use
+    
+    OUTPUT:
+    - ang_series: array of time series of the considered angle
+    '''
+    
+    # Retrieve points
+    keypt_series = []
+    for k in angle_params[0]:
+        keypt_series += [df_points.iloc[:,df_points.columns.get_level_values(2)==k].iloc[:,:2]]
+
+    # Compute angles
+    points_list = [k.values.T for k in keypt_series]
+    ang_series = points2D_to_angles(points_list)
+    ang_series += angle_params[2]
+    ang_series *= angle_params[3]
+    ang_series = np.where(ang_series>180,ang_series-360,ang_series)
+    ang_series = np.where((ang_series==0) | (ang_series==90) | (ang_series==180), +0, ang_series)
+
+    
+    return ang_series
+
+
+def segment_angles_series_from_points(df_points, angle_params, segment):
+    '''
+    Obtain segment angle series w/r horizontal from point series.
+    For trunk segment: mean of the angles between RHip-RShoulder and LHip-LShoulder
+    
+    INPUT: 
+    - df_points: dataframe of pose detection, from csv
+    - angle_params: dictionary specifying which points to use, and what offset and multiplying factor to use
+    - segment: which segment angle is considered
+    
+    OUTPUT:
+    - ang_series: array of time series of the considered angle
+    '''
+    
+    # Retrieve points
+    keypt_series = []
+    for k in angle_params[0]:
+        keypt_series += [df_points.iloc[:,df_points.columns.get_level_values(2)==k].iloc[:,:2]]
+    points_list = [k.values.T for k in keypt_series]
+    
+    # Compute angles
+    ang_series = points2D_to_angles(points_list)
+    ang_series += angle_params[2]
+    ang_series *= angle_params[3]
+    ang_series = np.where(ang_series>180,ang_series-360,ang_series)
+    
+    # For trunk: mean between angles RHip-RShoulder and LHip-LShoulder
+    if segment == 'Trunk':
+        ang_seriesR = ang_series
+        angle_params[0] = [a.replace('R','L') for a in angle_params[0]]
+        keypt_series = []
+        for k in angle_params[0]:
+            keypt_series += [df_points.iloc[:,df_points.columns.get_level_values(2)==k].iloc[:,:2]]
+        # Compute angles
+        points_list = [k.values.T for k in keypt_series]
+        ang_series = points2D_to_angles(points_list)
+        ang_series += angle_params[2]
+        ang_series *= angle_params[3]
+        ang_series = np.mean((ang_seriesR, ang_series), axis=0)
+        ang_series = np.where(ang_series>180,ang_series-360,ang_series)
+        
+    return ang_series
+    
+    
+def overlay_angles(frame, df_angles_list_frame):
+    '''
+    Overlays a text box for each detected person with joint and segment angles
+    
+    INPUT:
+    - frame: a frame opened with OpenCV
+    - df_angles_list_frame: list of one frame for all angles
+    '''
+    
+    cmap = plt.cm.hsv
+    font = cv2.FONT_HERSHEY_SIMPLEX
+    for i, angles_frame_person in enumerate(df_angles_list_frame):
+        for ang_nb in range(len(angles_frame_person)):
+            # Angle label
+            frame = cv2.putText(frame, 
+                angles_frame_person.index[ang_nb][2] + ':',
+                (10+250*i, 15+15*ang_nb), 
+                font, 0.5, 
+                (np.array(cmap((i+1)/len(df_angles_list_frame)))*255).tolist(), 
+                1, 
+                cv2.LINE_4)
+            # Angle value
+            frame = cv2.putText(frame, 
+                str(round(angles_frame_person[ang_nb],1)),
+                (150+250*i, 15+15*ang_nb), 
+                font, 0.5, 
+                (np.array(cmap((i+1)/len(df_angles_list_frame)))*255).tolist(), 
+                1, 
+                cv2.LINE_4)
+            # Progress bar
+            x_ang = int(angles_frame_person[ang_nb]*50/180)
+            if x_ang > 0:
+                sub_frame = frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i : 170+250*i+x_ang ]
+                white_rect = np.ones(sub_frame.shape, dtype=np.uint8) * 255
+                res = cv2.addWeighted(sub_frame, 0.6, white_rect, 0.4, 1.0)
+                frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i : 170+250*i+x_ang ] = res
+            elif x_ang < 0:
+                sub_frame = frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i+x_ang : 170+250*i ]
+                white_rect = np.ones(sub_frame.shape, dtype=np.uint8) * 255
+                res = cv2.addWeighted(sub_frame, 0.6, white_rect, 0.4, 1.0)
+                frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i+x_ang : 170+250*i ] = res
+        
+    return frame
+    
+    
+def compute_angles_fun(config_dict):
+    '''
+    Compute joint and segment angles from csv position files.
+    Automatically adjust angles when person switches to face the other way.
+    Save a 2D csv angle file per person.
+    Optionally filters results with Butterworth, gaussian, median, or loess filter.
+    Optionally displays figures.
+
+    Joint angle conventions:
+    - Ankle dorsiflexion: Between heel and big toe, and ankle and knee
+    - Knee flexion: Between hip, knee, and ankle 
+    - Hip flexion: Between knee, hip, and shoulder
+    - Shoulder flexion: Between hip, shoulder, and elbow
+    - Elbow flexion: Between wrist, elbow, and shoulder
+
+    Segment angle conventions:
+    Angles are measured anticlockwise between the horizontal and the segment.
+    - Foot: Between heel and big toe
+    - Shank: Between ankle and knee
+    - Thigh: Between hip and knee
+    - Arm: Between shoulder and elbow
+    - Forearm: Between elbow and wrist
+    - Trunk: Between hip midpoint and shoulder midpoint
+    
+    /!\ Warning /!\
+    - The angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.
+    - It will lead to reliable results only if the persons move in the 2D plane (sagittal plane).
+    - The persons need to be filmed as perpendicularly as possible from their side.
+    If you need research-grade markerless joint kinematics, consider using several cameras,
+    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
+    https://github.com/perfanalytics/pose2sim
+
+    INPUTS:
+    - one or several position csv files
+    - a dictionary obtained from a configuration file (.toml extension)
+    - a skeleton model
+    
+    OUTPUTS:
+    - one csv file for joint and segment angles per detected person
+    - a logs.txt file 
+    '''
+    
+    # Retrieve parameters
+    video_dir, video_file, frame_rate = base_params(config_dict)
+    pose_algo = config_dict.get('pose').get('pose_algo')
+    if pose_algo == 'OPENPOSE':
+        pose_model = config_dict.get('pose').get('OPENPOSE').get('openpose_model')
+    elif pose_algo == 'BLAZEPOSE':
+        pose_model = 'BLAZEPOSE'
+    joint_angles = config_dict.get('compute_angles').get('joint_angles')
+    segment_angles = config_dict.get('compute_angles').get('segment_angles')
+    angle_nb = len(joint_angles) + len(segment_angles)
+    
+    show_plots = config_dict.get('compute_angles_advanced').get('show_plots')
+    do_filter = config_dict.get('compute_angles_advanced').get('filter')
+    filter_type = config_dict.get('compute_angles_advanced').get('filter_type')
+    butterworth_filter_order = config_dict.get('compute_angles_advanced').get('butterworth').get('order')
+    butterworth_filter_cutoff = config_dict.get('compute_angles_advanced').get('butterworth').get('cut_off_frequency')
+    gaussian_filter_kernel = config_dict.get('compute_angles_advanced').get('gaussian').get('sigma_kernel')
+    loess_filter_kernel = config_dict.get('compute_angles_advanced').get('loess').get('nb_values_used')
+    median_filter_kernel = config_dict.get('compute_angles_advanced').get('median').get('kernel_size')
+    filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
+    
+    show_angles_img = config_dict.get('compute_angles_advanced').get('save_img')
+    show_angles_vid = config_dict.get('compute_angles_advanced').get('save_vid')
+    
+    # Find csv position files in video_dir, search pose_model and video_file.stem
+    logging.info(f'Retrieving csv position files in {video_dir}...')
+    csv_paths = list(video_dir.glob(f'*{video_file.stem}_{pose_model}_*points*.csv'))
+    logging.info(f'{len(csv_paths)} persons found.')
+
+    # Compute angles
+    df_angles_list = []
+    for i, c in enumerate(csv_paths):
+        # Prepare angle csv header
+        scorer = ['DavidPagnon']*angle_nb
+        individuals = [f'person{i}']*angle_nb
+        angs = joint_angles + segment_angles
+        coords = [joint_angle_dict.get(j)[1] for j in joint_angles] + [segment_angle_dict.get(s)[1] for s in segment_angles]
+        tuples = list(zip(scorer, individuals, angs, coords))
+        index_angs_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'angs', 'coords'])    
+
+        # Compute angles for each person, for each angle, with each required keypoint position
+        logging.info(f'Person {i}: Computing 2D joint and segment angles.')
+        with open(c) as c_f:
+            df_points = pd.read_csv(c_f, header=[0,1,2,3])
+            
+            # Flip along x when feet oriented to the left
+            df_points = flip_left_right_direction(df_points)
+            
+            # Joint angles
+            joint_angle_series = []
+            for j in joint_angles: 
+                angle_params = joint_angle_dict.get(j)
+                j_ang_series = joint_angles_series_from_points(df_points, angle_params)
+                joint_angle_series += [j_ang_series]
+    
+            # Segment angles
+            segment_angle_series = []
+            for s in segment_angles:
+                angle_params = segment_angle_dict.get(s)
+                s_ang_series = segment_angles_series_from_points(df_points, angle_params, s)
+                segment_angle_series += [s_ang_series]
+            
+            angle_series = joint_angle_series + segment_angle_series
+            df_angles = []
+            df_angles += [pd.DataFrame(angle_series, index=index_angs_csv).T]
+            
+            # Filter
+            if filter_options[0]:
+                filter_type = filter_options[1]
+                if filter_type == 'butterworth':
+                    args = f'Butterworth filter, {filter_options[2]}th order, {filter_options[3]} Hz.'
+                if filter_type == 'gaussian':
+                    args = f'Gaussian filter, Sigma kernel {filter_options[5]}'
+                if filter_type == 'loess':
+                    args = f'LOESS filter, window size of {filter_options[6]} frames.'
+                if filter_type == 'median':
+                    args = f'Median filter, kernel of {filter_options[7]}.'
+                logging.info(f'Person {i}: Filtering with {args}.')
+                df_angles[0].replace(0, np.nan, inplace=True)
+                df_angles += [df_angles[0].copy()]
+                df_angles[1] = df_angles[1].apply(filter.filter1d, axis=0, args=filter_options)
+            df_angles[-1].replace(np.nan, 0, inplace=True)
+               
+            # Creation of the csv files
+            csv_angle_path = c.parent / (c.stem.replace('points', 'angles') + '.csv')
+            logging.info(f'Person {i}: Saving csv angle file in {csv_angle_path}.')
+            df_angles[-1].to_csv(csv_angle_path, sep=',', index=True, lineterminator='\n')
+            
+            # Display figures
+            if show_plots:
+                logging.info(f'Person {i}: Displaying figures.')
+                display_figures_fun(df_angles)
+
+            df_angles_list += [df_angles[-1]]
+
+    # Add angles to vid and img
+    if show_angles_img or show_angles_vid:
+        video_base = Path(video_dir / video_file)
+        img_pose = video_base.parent / (video_base.stem + '_' + pose_model + '_img')
+        video_pose = video_base.parent / (video_base.stem + '_' + pose_model + '.mp4')
+        video_pose2 = video_base.parent / (video_base.stem + '_' + pose_model + '2.mp4')
+        
+        if show_angles_vid:
+            cap = [cv2.VideoCapture(str(video_pose)) if Path.exists(video_pose) else cv2.VideoCapture(str(video_base))][0]
+            fps = cap.get(cv2.CAP_PROP_FPS)
+            W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
+            fourcc = cv2.VideoWriter_fourcc(*'mp4v')
+            writer = cv2.VideoWriter(str(video_pose2), fourcc, fps, (int(W), int(H)))
+        
+        # Preferentially from pose image files
+        frames_img = list(img_pose.glob('*'))
+        if len(frames_img)>0:
+            for frame_nb in range(df_angles_list[0].shape[0]):
+                df_angles_list_frame = [df_angles_list[n].iloc[frame_nb,:] for n in range(len(df_angles_list))]
+                frame = cv2.imread(str(frames_img[frame_nb]))
+                frame = overlay_angles(frame, df_angles_list_frame)
+                if show_angles_img:
+                    cv2.imwrite(str(frames_img[frame_nb]), frame)
+                if show_angles_vid:
+                    writer.write(frame)
+            writer.release()
+                
+        # Else from pose video (or base video if pose video does not exist)
+        elif Path.exists(video_base) or Path.exists(video_pose):
+            frame_nb = 0
+            while cap.isOpened():
+                ret, frame = cap.read()
+                if ret == True:
+                    df_angles_list_frame = [df_angles_list[n].iloc[frame_nb,:] for n in range(len(df_angles_list))]
+                    frame = overlay_angles(frame, df_angles_list_frame)
+                    if show_angles_img:
+                        if frame_nb==0: img_pose.mkdir(parents=True, exist_ok=True)
+                        cv2.imwrite(str(img_pose / (video_base.stem + '_' + pose_model + '.' + str(frame_nb).zfill(5)+'.png')), frame)
+                    if show_angles_vid:
+                        writer.write(frame)
+                    frame_nb+=1
+                else:
+                    break
+        
+        cap.release()
+        writer.release()
+        if show_angles_vid:
+            if Path.exists(video_pose): os.remove(video_pose)
+            os.rename(video_pose2,video_pose)
+            if Path.exists(video_pose2): os.remove(video_pose2)
+
     logging.info(f'Done.')
```

### Comparing `sports2d-0.0.2/Sports2D/detect_pose.py` & `sports2d-0.0.5/Sports2D/detect_pose.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,541 +1,541 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-
-'''
-    ##############################################################
-    ## Compute angles from 2D pose detection                    ##
-    ##############################################################
-    
-    Detect joint centers from a video with OpenPose or BlazePose.
-    Save a 2D csv position file per person, and optionally json files, image files, and video files.
-    
-    If OpenPose is used, multiple persons can be consistently detected across frames.
-    Interpolates sequences of missing data if they are less than N frames long.
-    Optionally filters results with Butterworth, gaussian, median, or loess filter.
-    Optionally displays figures.
-
-    If BlazePose is used, only one person can be detected.
-    No interpolation nor filtering options available. Not plotting available.
-
-    /!\ Warning /!\
-    - The pose detection is only as good as the pose estimation algorithm, i.e., it is not perfect.
-    - It will lead to reliable results only if the persons move in the 2D plane (sagittal plane).
-    - The persons need to be filmed as perpendicularly as possible from their side.
-    If you need research-grade markerless joint kinematics, consider using several cameras,
-    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
-    https://github.com/perfanalytics/pose2sim
-   
-    INPUTS:
-    - a video
-    - a dictionary obtained from a configuration file (.toml extension)
-    - a skeleton model
-    
-    OUTPUTS:
-    - one csv file of joint coordinates per detected person
-    - optionally json directory, image directory, video
-    - a logs.txt file 
-
-'''    
-
-
-## INIT
-import os
-import logging
-from pathlib import Path
-import json
-import subprocess
-import itertools as it
-import numpy as np
-import pandas as pd
-import cv2
-import matplotlib.pyplot as plt
-import matplotlib as mpl
-mpl.use('qt5agg')
-mpl.rc('figure', max_open_warning=0)
-from Sports2D.Sports2D import base_params
-from Sports2D.Utilities import Blazepose_runsave, filter, common
-from Sports2D.Utilities.skeletons import *
-
-
-## AUTHORSHIP INFORMATION
-__author__ = "David Pagnon"
-__copyright__ = "Copyright 2023, Sports2D"
-__credits__ = ["David Pagnon"]
-__license__ = "BSD 3-Clause License"
-__version__ = "0.1"
-__maintainer__ = "David Pagnon"
-__email__ = "contact@david-pagnon.com"
-__status__ = "Development"
-
-
-# FUNCTIONS
-def display_figures_fun(df_list):
-    '''
-    Displays filtered and unfiltered data for comparison
-    /!\ Crashes on the third window...
-
-    INPUTS:
-    - df_list: list of dataframes of 3N columns, only 3i and 3i+1 are displayed
-
-    OUTPUT:
-    - matplotlib window with tabbed figures for each keypoint
-    '''
-    
-    keypoints_names = df_list[0].columns.get_level_values(2)[1::3]
-    
-    pw = common.plotWindow()
-    for id, keypoint in enumerate(keypoints_names):
-        f = plt.figure()
-        
-        axX = plt.subplot(211)
-        [plt.plot(df_list[0].index, df.iloc[:,id*3], label=['unfiltered' if i==0 else 'filtered' if i==1 else ''][0]) for i,df in enumerate(df_list)]
-        plt.setp(axX.get_xticklabels(), visible=False)
-        axX.set_ylabel(keypoint+' X')
-        plt.legend()
-
-        axY = plt.subplot(212)
-        [plt.plot(df_list[0].index, df.iloc[:,id*3+1]) for df in df_list]
-        plt.setp(axY.get_xticklabels(), visible=False)
-        axY.set_ylabel(keypoint+' Y')
-
-        pw.addPlot(keypoint, f)
-    
-    pw.show()
-    
-    
-def euclidean_distance(q1, q2):
-    '''
-    Euclidean distance between 2 points (N-dim).
-
-    INPUTS:
-    - q1: list of N_dimensional coordinates of point
-    - q2: idem
-
-    OUTPUTS:
-    - euc_dist: float. Euclidian distance between q1 and q2
-    '''
-
-    q1 = np.array(q1)
-    q2 = np.array(q2)
-    dist = q2 - q1
-
-    euc_dist = np.sqrt(np.sum( [d**2 for d in dist]))
-
-    return euc_dist
-
-    
-def min_with_single_indices(L, T):
-    '''
-    Let L be a list (size s) with T associated tuple indices (size s).
-    Select the smallest values of L, considering that 
-    the next smallest value cannot have the same numbers 
-    in the associated tuple as any of the previous ones.
-
-    Example:
-    L = [  20,   27,  51,    33,   43,   23,   37,   24,   4,   68,   84,    3  ]
-    T = list(it.product(range(2),range(3)))
-      = [(0,0),(0,1),(0,2),(0,3),(1,0),(1,1),(1,2),(1,3),(2,0),(2,1),(2,2),(2,3)]
-
-    - 1st smallest value: 3 with tuple (2,3), index 11
-    - 2nd smallest value when excluding indices [(0,0),(0,1),(0,2),X,(1,0),(1,1),(1,2),X,X,X,X,X]:
-    20 with tuple (0,0), index 0
-    - 3rd smallest value when excluding [X,X,X,X,X,(1,1),(1,2),X,X,X,X,X]:
-    23 with tuple (1,1), index 5
-    
-    INPUTS:
-    - L: list (size s)
-    - T: T associated tuple indices (size s)
-
-    OUTPUTS: 
-    - minL: list of smallest values of L, considering constraints on tuple indices
-    - argminL: list of indices of smallest values of L
-    - T_minL: list of tuples associated with smallest values of L
-    '''
-
-    minL = [np.min(L)]
-    argminL = [np.argmin(L)]
-    T_minL = [T[argminL[0]]]
-    
-    mask_tokeep = np.array([True for t in T])
-    i=0
-    while mask_tokeep.any()==True:
-        mask_tokeep = mask_tokeep & np.array([t[0]!=T_minL[i][0] and t[1]!=T_minL[i][1] for t in T])
-        if mask_tokeep.any()==True:
-            indicesL_tokeep = np.where(mask_tokeep)[0]
-            minL += [np.min(np.array(L)[indicesL_tokeep])]
-            argminL += [indicesL_tokeep[np.argmin(np.array(L)[indicesL_tokeep])]]
-            T_minL += (T[argminL[i+1]],)
-            i+=1
-    
-    return minL, argminL, T_minL
-    
-    
-def sort_people(keyptpre, keypt, nb_persons_to_detect):
-    '''
-    Associate persons across frames
-    Persons' indices are sometimes swapped when changing frame
-    A person is associated to another in the next frame when they are at a small distance
-    
-    INPUTS:
-    - keyptpre: array of shape K, L, M with K the number of detected persons,
-    L the number of detected keypoints, M their 2D coordinates + confidence
-    for the previous frame
-    - keypt: idem keyptpre, for current frame
-    
-    OUTPUT:
-    - keypt: array with reordered persons
-    '''
-    
-    # Generate possible person correspondences across frames
-    personsIDs_comb = list(it.product(range(len(keyptpre)),range(len(keypt))))
-    # Compute distance between persons from one frame to another
-    frame_by_frame_dist = []
-    for comb in personsIDs_comb:
-        frame_by_frame_dist += [np.mean([euclidean_distance(i,j) for (i,j) in zip(keyptpre[comb[0]][:,:2],keypt[comb[1]][:,:2])])]
-    # sort correspondences by distance
-    _, index_best_comb, _ = min_with_single_indices(frame_by_frame_dist, personsIDs_comb)
-    index_best_comb.sort()
-    personsIDs_sorted = np.array(personsIDs_comb)[index_best_comb][:,1]
-    # rearrange persons
-    keypt = np.array(keypt)[personsIDs_sorted]
-    
-    return keypt
-
-
-def json_to_csv(json_path, pose_model, interp_gap_smaller_than, filter_options, show_plots):
-    '''
-    Converts frame-by-frame json coordinate files 
-    to one csv files per detected person
-
-    INPUTS:
-    - json_path: directory path of json files
-    - pose_model: string, to get tree from skeletons.py
-    - interp_gap_smaller_than: integer, maximum number of missing frames for conducting interpolation
-    - filter_options: list, options for filtering
-    - show_plots: boolean, show plots or not
-
-    OUTPUTS:
-    - Creation of one csv files per detected person
-    '''
-        
-    # Retrieve keypoint names from model
-    model = eval(pose_model)
-    keypoints_ids = [node.id for _, _, node in RenderTree(model) if node.id!=None]
-    keypoints_names = [node.name for _, _, node in RenderTree(model) if node.id!=None]
-    keypoints_names_rearranged = [y for x,y in sorted(zip(keypoints_ids,keypoints_names))]
-    keypoints_nb = len(keypoints_ids)
-       
-    # Retrieve coordinates
-    logging.info('Sorting people across frames.')
-    json_fnames = list(json_path.glob('*.json'))
-    nb_persons_to_detect = max([len(json.load(open(json_fname))['people']) for json_fname in json_fnames])
-    Coords = [np.array([]).reshape(0,keypoints_nb*3)] * nb_persons_to_detect
-    for json_fname in json_fnames:    # for each frame
-        with open(json_fname) as json_f:
-            json_file = json.load(json_f)
-            keypt = []
-            # Retrieve coords for this frame 
-            for ppl in range(len(json_file['people'])):  # for each detected person
-                keypt += [np.asarray(json_file['people'][ppl]['pose_keypoints_2d']).reshape(-1,3)]
-            keypt = np.array(keypt)
-            # Make sure keypt is as large as the number of persons that need to be detected
-            if len(keypt) < nb_persons_to_detect:
-                empty_keypt_to_add = np.concatenate( [[ np.zeros([25,3]) ]] * (nb_persons_to_detect-len(keypt)) )
-                keypt = np.concatenate([keypt, empty_keypt_to_add])
-            if 'keyptpre' not in locals():
-                keyptpre = keypt
-            # Associate persons across frames
-            keypt = sort_people(keyptpre, keypt, nb_persons_to_detect)
-            # Concatenate to coordinates of previous frames
-            for i in range(nb_persons_to_detect): 
-                Coords[i] = np.vstack([Coords[i], keypt[i].reshape(-1)])
-            keyptpre = keypt
-    logging.info(f'{nb_persons_to_detect} persons found.')
-    
-    # Inject coordinates in dataframes and save
-    for i in range(nb_persons_to_detect): 
-        # Prepare csv header
-        scorer = ['DavidPagnon']*keypoints_nb*3
-        individuals = [f'person{i}']*keypoints_nb*3
-        bodyparts = [[p]*3 for p in keypoints_names_rearranged]
-        bodyparts = [item for sublist in bodyparts for item in sublist]
-        coords = ['x', 'y', 'likelihood']*keypoints_nb
-        tuples = list(zip(scorer, individuals, bodyparts, coords))
-        index_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'bodyparts', 'coords'])
-    
-        # Interpolate
-        logging.info(f'Person {i}: Interpolating missing sequences if they are smaller than {interp_gap_smaller_than} frames.')
-        df_list=[]
-        df_list += [pd.DataFrame(Coords[i].T, index=index_csv).T]
-        df_list[0] = df_list[0].apply(common.interpolate_zeros_nans, axis=0, args = [interp_gap_smaller_than, 'linear'])
-        
-        # Filter
-        if filter_options[0]:
-            filter_type = filter_options[1]
-            if filter_type == 'butterworth':
-                args = f'Butterworth filter, {filter_options[2]}th order, {filter_options[3]} Hz.'
-            if filter_type == 'gaussian':
-                args = f'Gaussian filter, Sigma kernel {filter_options[5]}'
-            if filter_type == 'loess':
-                args = f'LOESS filter, window size of {filter_options[6]} frames.'
-            if filter_type == 'median':
-                args = f'Median filter, kernel of {filter_options[7]}.'
-            logging.info(f'Person {i}: Filtering with {args}.')
-            df_list[0].replace(0, np.nan, inplace=True)
-            df_list += [df_list[0].copy()]
-            df_list[1] = df_list[1].apply(filter.filter1d, axis=0, args=filter_options)
-        df_list[-1].replace(np.nan, 0, inplace=True)
-           
-        # Save csv
-        csv_path = json_path.parent / Path(json_path.name[:-5]+f'_person{i}_points.csv')
-        logging.info(f'Person {i}: Saving csv position file in {csv_path}.')
-        df_list[-1].to_csv(csv_path, sep=',', index=True, lineterminator='\n')
-        
-        # Display figures
-        if show_plots:
-            logging.info(f'Person {i}: Displaying figures.')
-            display_figures_fun(df_list)
-            
-
-def draw_bounding_box(X, Y, img):
-    '''
-    Draw bounding boxes and person ID
-    around list of lists of X and Y coordinates
-    
-    INPUTS:
-    - X: list of list of x coordinates
-    - Y: list of list of y coordinates
-    - img: opencv image
-    
-    OUTPUT:
-    - img: image with rectangles and person IDs
-    '''
-    
-    cmap = plt.cm.hsv
-    
-    # Draw rectangles
-    [cv2.rectangle(img, 
-        (np.nanmin(x).astype(int)-25, np.nanmin(y).astype(int)-25), 
-        (np.nanmax(x).astype(int)+25, np.nanmax(y).astype(int)+25), 
-        (np.array(cmap((i+1)/len(X)))*255).tolist(), 
-        2) 
-        for i,(x,y) in enumerate(zip(X,Y))]
- 
-    # Write person ID
-    [cv2.putText(img, str(i),
-        (np.nanmin(x).astype(int), np.nanmin(y).astype(int)), 
-        cv2.FONT_HERSHEY_SIMPLEX, 1,
-        (np.array(cmap((i+1)/len(X)))*255).tolist(),
-        2, cv2.LINE_AA) 
-        for i,(x,y) in enumerate(zip(X,Y))]
-    
-    return img
-
-
-def draw_keypts_skel(X, Y, img, *pose_model):
-    '''
-    Draws keypoints and optionally skeleton for each person
-
-    INPUTS:
-    - X: list of list of x coordinates
-    - Y: list of list of y coordinates
-    - img: opencv image
-    
-    OUTPUT:
-    - img: image with keypoints and skeleton
-    '''
-    
-    model = eval(pose_model[0])
-    cmap = plt.cm.hsv
-    
-    # Draw keypoints (same color for same keypoint)
-    for (x,y) in zip(X,Y):
-        [cv2.circle(img, (int(x[i]), int(y[i])), 5,
-            (255,255,255),
-            -1)
-            for i in range(len(x))
-            if not (np.isnan(x[i]) or np.isnan(y[i]))]
-    
-    # Draw skeleton
-    if pose_model != None:
-        eval(pose_model[0])
-        # Get (unique) pairs between which to draw a line
-        node_pairs = []
-        for data_i in PreOrderIter(model.root, filter_=lambda node: node.is_leaf):
-            node_branches = [node_i.id for node_i in data_i.path[1:]]
-            node_pairs += [[node_branches[i],node_branches[i+1]] for i in range(len(node_branches)-1)]
-        node_pairs = [list(x) for x in set(tuple(x) for x in node_pairs)]
-        # Draw lines
-        for (x,y) in zip(X,Y):
-            [cv2.line(img,
-            (int(x[n[0]]), int(y[n[0]])), (int(x[n[1]]), int(y[n[1]])),
-            (np.array(cmap((i+1)/len(node_pairs)))*255).tolist(), 
-            2)
-            for i, n in enumerate(node_pairs)
-            if not (np.isnan(x[n[0]]) or np.isnan(y[n[0]]) or np.isnan(x[n[1]]) or np.isnan(y[n[1]]))]
-    
-    return img
-
-
-def save_imgvid_reID(video_path, save_vid=1, save_img=1, *pose_model):
-    '''
-    Displays json 2d detections overlayed on original raw images.
-    High confidence keypoints are green, low confidence ones are red.
-     
-    Note: See 'json_display_without_img.py' if you only want to display the
-    json coordinates on an animated graph or if don't have the original raw
-    images.
-    
-    Usage: 
-    json_display_with_img -j "<json_folder>" -i "<raw_img_folder>"
-    json_display_with_img -j "<json_folder>" -i "<raw_img_folder>" -o "<output_img_folder>" -d True -s True
-    import json_display_with_img; json_display_with_img.json_display_with_img_func(json_folder=r'<json_folder>', raw_img_folder=r'<raw_img_folder>')
-    '''
-            
-   # Find csv position files, prepare video and image saving paths
-    pose_model = pose_model[0]
-    csv_paths = list(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*refined*.csv'))
-    if csv_paths == []:
-        csv_paths = list(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*.csv'))
-        
-    # Open csv files
-    coords = []
-    for c in csv_paths:
-        with open(c) as c_f:
-            coords += [pd.read_csv(c_f, header=[0,1,2,3])]
-
-    # Open video frame by frame
-    cap = cv2.VideoCapture(str(video_path))
-    W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
-    fps = cap.get(cv2.CAP_PROP_FPS)
-    if (cap.isOpened()== False): 
-        print("Error opening video stream or file")
-    if save_vid:
-        video_pose_path = video_path.parent / (video_path.stem + '_' + pose_model + '.mp4')
-        fourcc = cv2.VideoWriter_fourcc(*'mp4v')
-        writer = cv2.VideoWriter(str(video_pose_path), fourcc, fps, (int(W), int(H)))
-    if save_img:
-        img_pose_path = video_path.parent / (video_path.stem + '_' + pose_model + '_img')
-        img_pose_path.mkdir(parents=True, exist_ok=True)  
-        
-    f = 0
-    while(cap.isOpened()):
-        ret, frame = cap.read()
-        if ret == True:
-            X = [np.array(coord.iloc[f,1::3]) for coord in coords]
-            X = [np.where(x==0., np.nan, x) for x in X]
-            Y = [np.array(coord.iloc[f,2::3]) for coord in coords]
-            Y = [np.where(y==0., np.nan, y) for y in Y]
-
-            # Draw bounding box
-            frame = draw_bounding_box(X, Y, frame)
-
-            # Draw keypoints and skeleton
-            frame = draw_keypts_skel(X, Y, frame, pose_model)
-            
-            # Save video and images
-            if save_vid:
-                writer.write(frame)
-            if save_img:
-                cv2.imwrite(str( img_pose_path / (video_path.stem+'_'+pose_model+'.'+str(f).zfill(5)+'.png' )), frame)
-
-        else: 
-            break
-        f += 1
-    cap.release()
-    writer.release()
-
-
-def detect_pose_fun(config_dict):
-    '''
-    Detect joint centers from a video with OpenPose or BlazePose.
-    Save a 2D csv file per person, and optionally json files, image files, and video file.
-    
-    If OpenPose is used, multiple persons can be consistently detected across frames.
-    Interpolates sequences of missing data if they are less than N frames long.
-    Optionally filters results with Butterworth, gaussian, median, or loess filter.
-    Optionally displays figures.
-
-    If BlazePose is used, only one person can be detected.
-    No interpolation nor filtering options available. Not plotting available.
-
-    /!\ Warning /!\
-    - The pose detection is only as good as the pose estimation algorithm, i.e., it is not perfect.
-    - It will lead to reliable results only if the persons move in the 2D plane (sagittal plane).
-    - The persons need to be filmed as perpendicularly as possible from their side.
-    If you need research-grade markerless joint kinematics, consider using several cameras,
-    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
-    https://github.com/perfanalytics/pose2sim
-        
-    INPUTS:
-    - a video
-    - a dictionary obtained from a configuration file (.toml extension)
-    - a skeleton model
-    
-    OUTPUTS:
-    - one csv file of joint coordinates per detected person
-    - optionally json directory, image directory, video
-    - a logs.txt file 
-    '''
-    
-    # Retrieve parameters
-    root_dir = os.getcwd()
-    video_dir, video_file, frame_rate = base_params(config_dict)
-    pose_algo = config_dict.get('pose').get('pose_algo')
-    
-    load_pose = config_dict.get('pose_advanced').get('load_pose')
-    save_vid = config_dict.get('pose_advanced').get('save_vid')
-    save_img = config_dict.get('pose_advanced').get('save_img')
-    interp_gap_smaller_than = config_dict.get('pose_advanced').get('interp_gap_smaller_than')
-    
-    show_plots = config_dict.get('pose_advanced').get('show_plots')
-    do_filter = config_dict.get('pose_advanced').get('filter')
-    filter_type = config_dict.get('pose_advanced').get('filter_type')
-    butterworth_filter_order = config_dict.get('pose_advanced').get('butterworth').get('order')
-    butterworth_filter_cutoff = config_dict.get('pose_advanced').get('butterworth').get('cut_off_frequency')
-    gaussian_filter_kernel = config_dict.get('pose_advanced').get('gaussian').get('sigma_kernel')
-    loess_filter_kernel = config_dict.get('pose_advanced').get('loess').get('nb_values_used')
-    median_filter_kernel = config_dict.get('pose_advanced').get('median').get('kernel_size')
-    filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
-    
-    video_file_stem = video_file.stem
-    video_path = video_dir / video_file
-
-    if pose_algo == 'OPENPOSE':
-        pose_model = config_dict.get('pose').get('OPENPOSE').get('openpose_model')
-        json_path = video_dir / '_'.join((video_file_stem,pose_model,'json'))
-        
-        # Pose detection skipped if load existing json files
-        if load_pose and list(json_path.glob('*'))>0:
-            pass
-        else:
-            logging.info(f'Detecting 2D joint positions with OpenPose model {pose_model}, for {video_file}.')
-            json_path.mkdir(parents=True, exist_ok=True)
-            openpose_path = config_dict.get('pose').get('OPENPOSE').get('openpose_path')
-            os.chdir(openpose_path)
-            subprocess.run(["bin\OpenPoseDemo.exe", "--video", video_path, \
-                "--model_pose", pose_model, \
-                "--write_json", json_path, \
-                "--render_pose", "0", "--display", "0"])
-            os.chdir(root_dir)
-        
-    # Sort people and save to csv, optionally display plot
-        json_to_csv(json_path, pose_model, interp_gap_smaller_than, filter_options, show_plots)
-        
-    # Save images and files after reindentification
-        if save_img and save_vid:
-            logging.info(f'Saving images and video in {video_dir}.')
-        if save_img and not save_vid:
-            logging.info(f'Saving images in {video_dir}.')
-        if not save_img and save_vid:
-            logging.info(f'Saving video in {video_dir}.')
-        if save_vid or save_img:
-            save_imgvid_reID(video_path, save_vid, save_img, pose_model)
-   
-     
-    elif pose_algo == 'BLAZEPOSE':
-        model_complexity = config_dict.get('pose').get('BLAZEPOSE').get('model_complexity')
-        Blazepose_runsave.blazepose_detec_func(input_file=video_path, save_images=save_img, to_json=True, save_video=save_vid, to_csv=True, model_complexity=model_complexity)
-
-    logging.info(f'Done.')
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+
+'''
+    ##############################################################
+    ## Compute angles from 2D pose detection                    ##
+    ##############################################################
+    
+    Detect joint centers from a video with OpenPose or BlazePose.
+    Save a 2D csv position file per person, and optionally json files, image files, and video files.
+    
+    If OpenPose is used, multiple persons can be consistently detected across frames.
+    Interpolates sequences of missing data if they are less than N frames long.
+    Optionally filters results with Butterworth, gaussian, median, or loess filter.
+    Optionally displays figures.
+
+    If BlazePose is used, only one person can be detected.
+    No interpolation nor filtering options available. Not plotting available.
+
+    /!\ Warning /!\
+    - The pose detection is only as good as the pose estimation algorithm, i.e., it is not perfect.
+    - It will lead to reliable results only if the persons move in the 2D plane (sagittal plane).
+    - The persons need to be filmed as perpendicularly as possible from their side.
+    If you need research-grade markerless joint kinematics, consider using several cameras,
+    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
+    https://github.com/perfanalytics/pose2sim
+   
+    INPUTS:
+    - a video
+    - a dictionary obtained from a configuration file (.toml extension)
+    - a skeleton model
+    
+    OUTPUTS:
+    - one csv file of joint coordinates per detected person
+    - optionally json directory, image directory, video
+    - a logs.txt file 
+
+'''    
+
+
+## INIT
+import os
+import logging
+from pathlib import Path
+import json
+import subprocess
+import itertools as it
+import numpy as np
+import pandas as pd
+import cv2
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+mpl.use('qt5agg')
+mpl.rc('figure', max_open_warning=0)
+from Sports2D.Sports2D import base_params
+from Sports2D.Utilities import Blazepose_runsave, filter, common
+from Sports2D.Utilities.skeletons import *
+
+
+## AUTHORSHIP INFORMATION
+__author__ = "David Pagnon"
+__copyright__ = "Copyright 2023, Sports2D"
+__credits__ = ["David Pagnon"]
+__license__ = "BSD 3-Clause License"
+__version__ = "0.1"
+__maintainer__ = "David Pagnon"
+__email__ = "contact@david-pagnon.com"
+__status__ = "Development"
+
+
+# FUNCTIONS
+def display_figures_fun(df_list):
+    '''
+    Displays filtered and unfiltered data for comparison
+    /!\ Crashes on the third window...
+
+    INPUTS:
+    - df_list: list of dataframes of 3N columns, only 3i and 3i+1 are displayed
+
+    OUTPUT:
+    - matplotlib window with tabbed figures for each keypoint
+    '''
+    
+    keypoints_names = df_list[0].columns.get_level_values(2)[1::3]
+    
+    pw = common.plotWindow()
+    for id, keypoint in enumerate(keypoints_names):
+        f = plt.figure()
+        
+        axX = plt.subplot(211)
+        [plt.plot(df_list[0].index, df.iloc[:,id*3], label=['unfiltered' if i==0 else 'filtered' if i==1 else ''][0]) for i,df in enumerate(df_list)]
+        plt.setp(axX.get_xticklabels(), visible=False)
+        axX.set_ylabel(keypoint+' X')
+        plt.legend()
+
+        axY = plt.subplot(212)
+        [plt.plot(df_list[0].index, df.iloc[:,id*3+1]) for df in df_list]
+        plt.setp(axY.get_xticklabels(), visible=False)
+        axY.set_ylabel(keypoint+' Y')
+
+        pw.addPlot(keypoint, f)
+    
+    pw.show()
+    
+    
+def euclidean_distance(q1, q2):
+    '''
+    Euclidean distance between 2 points (N-dim).
+
+    INPUTS:
+    - q1: list of N_dimensional coordinates of point
+    - q2: idem
+
+    OUTPUTS:
+    - euc_dist: float. Euclidian distance between q1 and q2
+    '''
+
+    q1 = np.array(q1)
+    q2 = np.array(q2)
+    dist = q2 - q1
+
+    euc_dist = np.sqrt(np.sum( [d**2 for d in dist]))
+
+    return euc_dist
+
+    
+def min_with_single_indices(L, T):
+    '''
+    Let L be a list (size s) with T associated tuple indices (size s).
+    Select the smallest values of L, considering that 
+    the next smallest value cannot have the same numbers 
+    in the associated tuple as any of the previous ones.
+
+    Example:
+    L = [  20,   27,  51,    33,   43,   23,   37,   24,   4,   68,   84,    3  ]
+    T = list(it.product(range(2),range(3)))
+      = [(0,0),(0,1),(0,2),(0,3),(1,0),(1,1),(1,2),(1,3),(2,0),(2,1),(2,2),(2,3)]
+
+    - 1st smallest value: 3 with tuple (2,3), index 11
+    - 2nd smallest value when excluding indices [(0,0),(0,1),(0,2),X,(1,0),(1,1),(1,2),X,X,X,X,X]:
+    20 with tuple (0,0), index 0
+    - 3rd smallest value when excluding [X,X,X,X,X,(1,1),(1,2),X,X,X,X,X]:
+    23 with tuple (1,1), index 5
+    
+    INPUTS:
+    - L: list (size s)
+    - T: T associated tuple indices (size s)
+
+    OUTPUTS: 
+    - minL: list of smallest values of L, considering constraints on tuple indices
+    - argminL: list of indices of smallest values of L
+    - T_minL: list of tuples associated with smallest values of L
+    '''
+
+    minL = [np.min(L)]
+    argminL = [np.argmin(L)]
+    T_minL = [T[argminL[0]]]
+    
+    mask_tokeep = np.array([True for t in T])
+    i=0
+    while mask_tokeep.any()==True:
+        mask_tokeep = mask_tokeep & np.array([t[0]!=T_minL[i][0] and t[1]!=T_minL[i][1] for t in T])
+        if mask_tokeep.any()==True:
+            indicesL_tokeep = np.where(mask_tokeep)[0]
+            minL += [np.min(np.array(L)[indicesL_tokeep])]
+            argminL += [indicesL_tokeep[np.argmin(np.array(L)[indicesL_tokeep])]]
+            T_minL += (T[argminL[i+1]],)
+            i+=1
+    
+    return minL, argminL, T_minL
+    
+    
+def sort_people(keyptpre, keypt, nb_persons_to_detect):
+    '''
+    Associate persons across frames
+    Persons' indices are sometimes swapped when changing frame
+    A person is associated to another in the next frame when they are at a small distance
+    
+    INPUTS:
+    - keyptpre: array of shape K, L, M with K the number of detected persons,
+    L the number of detected keypoints, M their 2D coordinates + confidence
+    for the previous frame
+    - keypt: idem keyptpre, for current frame
+    
+    OUTPUT:
+    - keypt: array with reordered persons
+    '''
+    
+    # Generate possible person correspondences across frames
+    personsIDs_comb = list(it.product(range(len(keyptpre)),range(len(keypt))))
+    # Compute distance between persons from one frame to another
+    frame_by_frame_dist = []
+    for comb in personsIDs_comb:
+        frame_by_frame_dist += [np.mean([euclidean_distance(i,j) for (i,j) in zip(keyptpre[comb[0]][:,:2],keypt[comb[1]][:,:2])])]
+    # sort correspondences by distance
+    _, index_best_comb, _ = min_with_single_indices(frame_by_frame_dist, personsIDs_comb)
+    index_best_comb.sort()
+    personsIDs_sorted = np.array(personsIDs_comb)[index_best_comb][:,1]
+    # rearrange persons
+    keypt = np.array(keypt)[personsIDs_sorted]
+    
+    return keypt
+
+
+def json_to_csv(json_path, pose_model, interp_gap_smaller_than, filter_options, show_plots):
+    '''
+    Converts frame-by-frame json coordinate files 
+    to one csv files per detected person
+
+    INPUTS:
+    - json_path: directory path of json files
+    - pose_model: string, to get tree from skeletons.py
+    - interp_gap_smaller_than: integer, maximum number of missing frames for conducting interpolation
+    - filter_options: list, options for filtering
+    - show_plots: boolean, show plots or not
+
+    OUTPUTS:
+    - Creation of one csv files per detected person
+    '''
+        
+    # Retrieve keypoint names from model
+    model = eval(pose_model)
+    keypoints_ids = [node.id for _, _, node in RenderTree(model) if node.id!=None]
+    keypoints_names = [node.name for _, _, node in RenderTree(model) if node.id!=None]
+    keypoints_names_rearranged = [y for x,y in sorted(zip(keypoints_ids,keypoints_names))]
+    keypoints_nb = len(keypoints_ids)
+       
+    # Retrieve coordinates
+    logging.info('Sorting people across frames.')
+    json_fnames = list(json_path.glob('*.json'))
+    nb_persons_to_detect = max([len(json.load(open(json_fname))['people']) for json_fname in json_fnames])
+    Coords = [np.array([]).reshape(0,keypoints_nb*3)] * nb_persons_to_detect
+    for json_fname in json_fnames:    # for each frame
+        with open(json_fname) as json_f:
+            json_file = json.load(json_f)
+            keypt = []
+            # Retrieve coords for this frame 
+            for ppl in range(len(json_file['people'])):  # for each detected person
+                keypt += [np.asarray(json_file['people'][ppl]['pose_keypoints_2d']).reshape(-1,3)]
+            keypt = np.array(keypt)
+            # Make sure keypt is as large as the number of persons that need to be detected
+            if len(keypt) < nb_persons_to_detect:
+                empty_keypt_to_add = np.concatenate( [[ np.zeros([25,3]) ]] * (nb_persons_to_detect-len(keypt)) )
+                keypt = np.concatenate([keypt, empty_keypt_to_add])
+            if 'keyptpre' not in locals():
+                keyptpre = keypt
+            # Associate persons across frames
+            keypt = sort_people(keyptpre, keypt, nb_persons_to_detect)
+            # Concatenate to coordinates of previous frames
+            for i in range(nb_persons_to_detect): 
+                Coords[i] = np.vstack([Coords[i], keypt[i].reshape(-1)])
+            keyptpre = keypt
+    logging.info(f'{nb_persons_to_detect} persons found.')
+    
+    # Inject coordinates in dataframes and save
+    for i in range(nb_persons_to_detect): 
+        # Prepare csv header
+        scorer = ['DavidPagnon']*keypoints_nb*3
+        individuals = [f'person{i}']*keypoints_nb*3
+        bodyparts = [[p]*3 for p in keypoints_names_rearranged]
+        bodyparts = [item for sublist in bodyparts for item in sublist]
+        coords = ['x', 'y', 'likelihood']*keypoints_nb
+        tuples = list(zip(scorer, individuals, bodyparts, coords))
+        index_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'bodyparts', 'coords'])
+    
+        # Interpolate
+        logging.info(f'Person {i}: Interpolating missing sequences if they are smaller than {interp_gap_smaller_than} frames.')
+        df_list=[]
+        df_list += [pd.DataFrame(Coords[i].T, index=index_csv).T]
+        df_list[0] = df_list[0].apply(common.interpolate_zeros_nans, axis=0, args = [interp_gap_smaller_than, 'linear'])
+        
+        # Filter
+        if filter_options[0]:
+            filter_type = filter_options[1]
+            if filter_type == 'butterworth':
+                args = f'Butterworth filter, {filter_options[2]}th order, {filter_options[3]} Hz.'
+            if filter_type == 'gaussian':
+                args = f'Gaussian filter, Sigma kernel {filter_options[5]}'
+            if filter_type == 'loess':
+                args = f'LOESS filter, window size of {filter_options[6]} frames.'
+            if filter_type == 'median':
+                args = f'Median filter, kernel of {filter_options[7]}.'
+            logging.info(f'Person {i}: Filtering with {args}.')
+            df_list[0].replace(0, np.nan, inplace=True)
+            df_list += [df_list[0].copy()]
+            df_list[1] = df_list[1].apply(filter.filter1d, axis=0, args=filter_options)
+        df_list[-1].replace(np.nan, 0, inplace=True)
+           
+        # Save csv
+        csv_path = json_path.parent / Path(json_path.name[:-5]+f'_person{i}_points.csv')
+        logging.info(f'Person {i}: Saving csv position file in {csv_path}.')
+        df_list[-1].to_csv(csv_path, sep=',', index=True, lineterminator='\n')
+        
+        # Display figures
+        if show_plots:
+            logging.info(f'Person {i}: Displaying figures.')
+            display_figures_fun(df_list)
+            
+
+def draw_bounding_box(X, Y, img):
+    '''
+    Draw bounding boxes and person ID
+    around list of lists of X and Y coordinates
+    
+    INPUTS:
+    - X: list of list of x coordinates
+    - Y: list of list of y coordinates
+    - img: opencv image
+    
+    OUTPUT:
+    - img: image with rectangles and person IDs
+    '''
+    
+    cmap = plt.cm.hsv
+    
+    # Draw rectangles
+    [cv2.rectangle(img, 
+        (np.nanmin(x).astype(int)-25, np.nanmin(y).astype(int)-25), 
+        (np.nanmax(x).astype(int)+25, np.nanmax(y).astype(int)+25), 
+        (np.array(cmap((i+1)/len(X)))*255).tolist(), 
+        2) 
+        for i,(x,y) in enumerate(zip(X,Y))]
+ 
+    # Write person ID
+    [cv2.putText(img, str(i),
+        (np.nanmin(x).astype(int), np.nanmin(y).astype(int)), 
+        cv2.FONT_HERSHEY_SIMPLEX, 1,
+        (np.array(cmap((i+1)/len(X)))*255).tolist(),
+        2, cv2.LINE_AA) 
+        for i,(x,y) in enumerate(zip(X,Y))]
+    
+    return img
+
+
+def draw_keypts_skel(X, Y, img, *pose_model):
+    '''
+    Draws keypoints and optionally skeleton for each person
+
+    INPUTS:
+    - X: list of list of x coordinates
+    - Y: list of list of y coordinates
+    - img: opencv image
+    
+    OUTPUT:
+    - img: image with keypoints and skeleton
+    '''
+    
+    model = eval(pose_model[0])
+    cmap = plt.cm.hsv
+    
+    # Draw keypoints (same color for same keypoint)
+    for (x,y) in zip(X,Y):
+        [cv2.circle(img, (int(x[i]), int(y[i])), 5,
+            (255,255,255),
+            -1)
+            for i in range(len(x))
+            if not (np.isnan(x[i]) or np.isnan(y[i]))]
+    
+    # Draw skeleton
+    if pose_model != None:
+        eval(pose_model[0])
+        # Get (unique) pairs between which to draw a line
+        node_pairs = []
+        for data_i in PreOrderIter(model.root, filter_=lambda node: node.is_leaf):
+            node_branches = [node_i.id for node_i in data_i.path[1:]]
+            node_pairs += [[node_branches[i],node_branches[i+1]] for i in range(len(node_branches)-1)]
+        node_pairs = [list(x) for x in set(tuple(x) for x in node_pairs)]
+        # Draw lines
+        for (x,y) in zip(X,Y):
+            [cv2.line(img,
+            (int(x[n[0]]), int(y[n[0]])), (int(x[n[1]]), int(y[n[1]])),
+            (np.array(cmap((i+1)/len(node_pairs)))*255).tolist(), 
+            2)
+            for i, n in enumerate(node_pairs)
+            if not (np.isnan(x[n[0]]) or np.isnan(y[n[0]]) or np.isnan(x[n[1]]) or np.isnan(y[n[1]]))]
+    
+    return img
+
+
+def save_imgvid_reID(video_path, save_vid=1, save_img=1, *pose_model):
+    '''
+    Displays json 2d detections overlayed on original raw images.
+    High confidence keypoints are green, low confidence ones are red.
+     
+    Note: See 'json_display_without_img.py' if you only want to display the
+    json coordinates on an animated graph or if don't have the original raw
+    images.
+    
+    Usage: 
+    json_display_with_img -j "<json_folder>" -i "<raw_img_folder>"
+    json_display_with_img -j "<json_folder>" -i "<raw_img_folder>" -o "<output_img_folder>" -d True -s True
+    import json_display_with_img; json_display_with_img.json_display_with_img_func(json_folder=r'<json_folder>', raw_img_folder=r'<raw_img_folder>')
+    '''
+            
+   # Find csv position files, prepare video and image saving paths
+    pose_model = pose_model[0]
+    csv_paths = list(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*refined*.csv'))
+    if csv_paths == []:
+        csv_paths = list(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*.csv'))
+        
+    # Open csv files
+    coords = []
+    for c in csv_paths:
+        with open(c) as c_f:
+            coords += [pd.read_csv(c_f, header=[0,1,2,3])]
+
+    # Open video frame by frame
+    cap = cv2.VideoCapture(str(video_path))
+    W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
+    fps = cap.get(cv2.CAP_PROP_FPS)
+    if (cap.isOpened()== False): 
+        print("Error opening video stream or file")
+    if save_vid:
+        video_pose_path = video_path.parent / (video_path.stem + '_' + pose_model + '.mp4')
+        fourcc = cv2.VideoWriter_fourcc(*'mp4v')
+        writer = cv2.VideoWriter(str(video_pose_path), fourcc, fps, (int(W), int(H)))
+    if save_img:
+        img_pose_path = video_path.parent / (video_path.stem + '_' + pose_model + '_img')
+        img_pose_path.mkdir(parents=True, exist_ok=True)  
+        
+    f = 0
+    while(cap.isOpened()):
+        ret, frame = cap.read()
+        if ret == True:
+            X = [np.array(coord.iloc[f,1::3]) for coord in coords]
+            X = [np.where(x==0., np.nan, x) for x in X]
+            Y = [np.array(coord.iloc[f,2::3]) for coord in coords]
+            Y = [np.where(y==0., np.nan, y) for y in Y]
+
+            # Draw bounding box
+            frame = draw_bounding_box(X, Y, frame)
+
+            # Draw keypoints and skeleton
+            frame = draw_keypts_skel(X, Y, frame, pose_model)
+            
+            # Save video and images
+            if save_vid:
+                writer.write(frame)
+            if save_img:
+                cv2.imwrite(str( img_pose_path / (video_path.stem+'_'+pose_model+'.'+str(f).zfill(5)+'.png' )), frame)
+
+        else: 
+            break
+        f += 1
+    cap.release()
+    writer.release()
+
+
+def detect_pose_fun(config_dict):
+    '''
+    Detect joint centers from a video with OpenPose or BlazePose.
+    Save a 2D csv file per person, and optionally json files, image files, and video file.
+    
+    If OpenPose is used, multiple persons can be consistently detected across frames.
+    Interpolates sequences of missing data if they are less than N frames long.
+    Optionally filters results with Butterworth, gaussian, median, or loess filter.
+    Optionally displays figures.
+
+    If BlazePose is used, only one person can be detected.
+    No interpolation nor filtering options available. Not plotting available.
+
+    /!\ Warning /!\
+    - The pose detection is only as good as the pose estimation algorithm, i.e., it is not perfect.
+    - It will lead to reliable results only if the persons move in the 2D plane (sagittal plane).
+    - The persons need to be filmed as perpendicularly as possible from their side.
+    If you need research-grade markerless joint kinematics, consider using several cameras,
+    and constraining angles to a biomechanically accurate model. See Pose2Sim for example: 
+    https://github.com/perfanalytics/pose2sim
+        
+    INPUTS:
+    - a video
+    - a dictionary obtained from a configuration file (.toml extension)
+    - a skeleton model
+    
+    OUTPUTS:
+    - one csv file of joint coordinates per detected person
+    - optionally json directory, image directory, video
+    - a logs.txt file 
+    '''
+    
+    # Retrieve parameters
+    root_dir = os.getcwd()
+    video_dir, video_file, frame_rate = base_params(config_dict)
+    pose_algo = config_dict.get('pose').get('pose_algo')
+    
+    load_pose = config_dict.get('pose_advanced').get('load_pose')
+    save_vid = config_dict.get('pose_advanced').get('save_vid')
+    save_img = config_dict.get('pose_advanced').get('save_img')
+    interp_gap_smaller_than = config_dict.get('pose_advanced').get('interp_gap_smaller_than')
+    
+    show_plots = config_dict.get('pose_advanced').get('show_plots')
+    do_filter = config_dict.get('pose_advanced').get('filter')
+    filter_type = config_dict.get('pose_advanced').get('filter_type')
+    butterworth_filter_order = config_dict.get('pose_advanced').get('butterworth').get('order')
+    butterworth_filter_cutoff = config_dict.get('pose_advanced').get('butterworth').get('cut_off_frequency')
+    gaussian_filter_kernel = config_dict.get('pose_advanced').get('gaussian').get('sigma_kernel')
+    loess_filter_kernel = config_dict.get('pose_advanced').get('loess').get('nb_values_used')
+    median_filter_kernel = config_dict.get('pose_advanced').get('median').get('kernel_size')
+    filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
+    
+    video_file_stem = video_file.stem
+    video_path = video_dir / video_file
+
+    if pose_algo == 'OPENPOSE':
+        pose_model = config_dict.get('pose').get('OPENPOSE').get('openpose_model')
+        json_path = video_dir / '_'.join((video_file_stem,pose_model,'json'))
+        
+        # Pose detection skipped if load existing json files
+        if load_pose and len(list(json_path.glob('*')))>0:
+            pass
+        else:
+            logging.info(f'Detecting 2D joint positions with OpenPose model {pose_model}, for {video_file}.')
+            json_path.mkdir(parents=True, exist_ok=True)
+            openpose_path = config_dict.get('pose').get('OPENPOSE').get('openpose_path')
+            os.chdir(openpose_path)
+            subprocess.run(["bin\OpenPoseDemo.exe", "--video", video_path, \
+                "--model_pose", pose_model, \
+                "--write_json", json_path, \
+                "--render_pose", "0", "--display", "0"])
+            os.chdir(root_dir)
+        
+    # Sort people and save to csv, optionally display plot
+        json_to_csv(json_path, pose_model, interp_gap_smaller_than, filter_options, show_plots)
+        
+    # Save images and files after reindentification
+        if save_img and save_vid:
+            logging.info(f'Saving images and video in {video_dir}.')
+        if save_img and not save_vid:
+            logging.info(f'Saving images in {video_dir}.')
+        if not save_img and save_vid:
+            logging.info(f'Saving video in {video_dir}.')
+        if save_vid or save_img:
+            save_imgvid_reID(video_path, save_vid, save_img, pose_model)
+   
+     
+    elif pose_algo == 'BLAZEPOSE':
+        model_complexity = config_dict.get('pose').get('BLAZEPOSE').get('model_complexity')
+        Blazepose_runsave.blazepose_detec_func(input_file=video_path, save_images=save_img, to_json=True, save_video=save_vid, to_csv=True, model_complexity=model_complexity)
+
+    logging.info(f'Done.')
```

### Comparing `sports2d-0.0.2/sports2d.egg-info/PKG-INFO` & `sports2d-0.0.5/sports2d.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,274 +1,275 @@
-Metadata-Version: 2.1
-Name: sports2d
-Version: 0.0.2
-Summary: Detect pose and compute 2D joint angles from a video.
-Home-page: https://github.com/davidpagnon/Sports2D
-Author: David Pagnon
-Author-email: contact@david-pagnon.com
-License: BSD 3-Clause License
-Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
-Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
-Requires-Python: <=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<!-- 
-[![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
-[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D) \
-[![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
-[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
-[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
-[![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
-[![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
--->
-
-
-# Sports2D
-
-**`Sports2D` lets you compute 2D joint and segment angles from a single video.**
-
- </br>
- </br>
-
-<img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
-
-`Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
-`Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
-If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.
-
-`Announcement:` Apps with GUI will be released for Windows, Linux, MacOS, as well as Android and iOS.
-Mobile versions will only support simple exploratory analysis. This involves single-person angle computation, in a potentially less accurate and tunable way.
-
-
-## Contents
-1. [Installation and Demonstration](#installation-and-demonstration)
-   1. [Installation](#installation)
-   2. [Demonstration: Detect pose and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles)
-2. [Go further](#go-further)
-   1. [Use on your own videos](#use-on-your-own-videos)
-   2. [Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-multi-person-more-accurate-analysis)
-   3. [Advanced-settings](#advanced-settings)
-   4. [How it works](#how-it-works)
-3. [How to cite and how to contribute](#how-to-cite-and-how-to-contribute)
-
-
-## Installation and Demonstration
-
-### Installation
-
-- OPTION 1: **Quick install:** \
-    Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
-    ```
-    pip install sports2d
-    ```
-
-- OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
-    Open an Anaconda prompt and create a virtual environment by typing:
-    ```
-    conda create -n Sports2D python<=3.10 
-    conda activate Sports2D
-    pip install sports2d
-    ```
-
-- OPTION 3: **Build from source and test the last changes:**\
-     Open a terminal in the directory of your choice and clone the Sports2D repository.
-     ```
-     git clone https://github.com/davidpagnon/sports2d.git
-     cd sports2d
-     pip install .
-     ```
-
-
-### Demonstration: Detect pose and compute 2D angles
-
-Open a terminal, enter `pip show sports2d`, check sports2d package location. \
-Copy this path and go to the Demo folder by typing `cd <path>\Sports2D\Demo`. \
-Type `ipython`, and test the following code:
-```
-from Sports2D import Sports2D
-Sports2D.detect_pose('Config_demo.toml')
-Sports2D.compute_angles('Config_demo.toml')
-```
-
-<img src="Content/demo_blazepose_terminal.png" width="760">
-
-
-You should obtain a video with the overlaid 2D joint positions, and angle text values. This output is also provided as an image folder.\
-You should additionally obtain the same information as time series, stored in .csv files. These files can be opened with any spreadsheet software, or with the Pandas Python library for example.\
-In addition, you will get the original OpenPose-like json coordinates files.
-
-<img src="Content/demo_blazepose_results.png" width="760">
-
-
-## Go further
-
-### Use on your own videos
-
-1. Copy-paste `Config_demo.toml` in the directory of your video.
-
-2. Open it with any text editor.\
-Replace the `video_file` value with the name of your video.
-
-3. Open a terminal or an Anaconda prompt, type:
-   ```
-   cd <Path/to/video/directory>
-   conda activate Sports2D (skip if you did not install with Anaconda)
-   ipython
-   ```
-   ```
-   from Sports2D import Sports2D
-   Sports2D.detect_pose('Config_demo.toml')
-   Sports2D.compute_angles('Config_demo.toml')
-   ```
-
-*Optionally:* If your video is not in the same folder as `Config_demo.toml`, specify its location in `video_dir`.\
-Similarly, if you launch Sports2D in an other directory, specify the location of the config file this way: `Sports2D.detect_pose(<path_to_Config_demo.toml>)`\
-In `pose`, specify the use of BlazePose or OpenPose as joint detectors: this will be detailed in the next section.\
-In `compute_angles`, select your angles of interest.
-
-
-### Use OpenPose for multi-person, more accurate analysis
-
-OpenPose is slower than OpenPose, but more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
-
-1. **Install OpenPose** (instructions [there](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md)). \
-*Windows portable demo works fine.*
-
-2. If you want even more accurate results, use the BODY_25B experimental model instead of the standard BODY_25 one. This requires manually [downloading the model](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md). You can optionally download from there the BODY_135 model which will let you compute wrist flexion and hand segment angle, however this will be much slower.
-
-3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
-
-*N.B.:* If you want to benefit from the capabilities of OpenPose but do not manage to install it, you can use the `Colab notebook` version.\
-Note that your data will be sent to the Google servers, which do not follow the European GDPR requirements regarding privacy.
-**COMING SOON**
-
-
-### Advanced settings
-
-1. `Config_demo.toml` → `pose_advanced`: These settings are only taken into account if OpenPose is used.
-   1. `load_pose`: If you need to change some settings but have already run a pose estimation, you can set this to `true` in order to not regenerate the json pose files.
-
-   2. `save_vid` and `save_img`: You can choose whether you want to save the resulting video and images. If set to `false`, only pose and angle `.csv` files will be generated.
-
-   3. `interp_gap_smaller_than`: Gaps are interpolated only if they are not too wide.
-   
-   4. `filter`: `true` or `false`. If `true`, you can choose among `Butterworth`, `Gaussian`, `LOESS`, or `Median`, and specify their parameters.\
-   Beware that the appearance of the unfiltered skeleton may not match the filtered coordinates and angles.
-
-   5. `show_plots`: Displays a window with tabs corresponding to the coordinates of each detected point. This may cause Python to crash.
-
-2. `Config_demo.toml` → `compute_angles_advanced`: These settings are taken into account both with BlazePose and OpenPose.
-   1. `save_vid` and `save_img`: Cf `pose_advanced`.
-
-   2. `filter`: Cf `pose_advanced`.
-
-   3. `show_plots`: Cf `pose_advanced`.
-
-   <img src="Content/demo_show_plots.png" width="760">
-
-*N.B.:* The settings and results of all analyses are stored int the `logs.txt` file, which can be found in in the sports2d installation folder (`pip show sports2d` to find the path).
-
-
-
-### How it works
-
-#### Pose detection:
-
-BlazePose or OpenPose are used to detect joint centers from a video.
-
-If `BlazePose` is used, only one person can be detected.\
-No interpolation nor filtering options are available. Not plotting available.
-
-If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
-Sequences of missing data are interpolated if they are less than N frames long.\
-Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
-
-
-#### Angle computation:
-
-Joint and segment angles are computed from csv position files.\
-If a person suddently faces the other way, this change of direction is taken into account.\
-Resulting angles can be filtered in the same way as point coordinates, and they can also be plotted.
-
-**Joint angle conventions:**
-- Ankle dorsiflexion: Between heel and big toe, and ankle and knee
-- Knee flexion: Between hip, knee, and ankle 
-- Hip flexion: Between knee, hip, and shoulder
-- Shoulder flexion: Between hip, shoulder, and elbow
-- Elbow flexion: Between wrist, elbow, and shoulder
-
-**Segment angle conventions:**\
-Angles are measured anticlockwise between the horizontal and the segment.
-- Foot: Between heel and big toe
-- Shank: Between knee and ankle
-- Thigh: Between hip and knee
-- Arm: Between shoulder and elbow
-- Forearm: Between elbow and wrist
-- Trunk: Between shoulder midpoint and hip midpoint
-
-## How to cite and how to contribute
-
-### How to cite
-If you use this code or data, please cite [Pagnon, 2023].
-
-     @misc{Pagnon2023,
-       author = {Pagnon, David},
-       title = {Sports2D - Angles from monocular video},
-       year = {2013},
-       publisher = {GitHub},
-       journal = {GitHub repository},
-       howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
-     }
-
-### How to contribute
-I would happily welcome any proposal for new features, code improvement, and more!\
-If you want to contribute to Sports2D, please follow [this guide](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to fork, modify and push code, and submit a pull request. I would appreciate it if you provided as much useful information as possible about how you modified the code, and a rationale for why you're making this pull request. Please also specify on which operating system and on which python version you have tested the code.
-
-*Here is a to-do list, for general guidance purposes only:*
-> <li> <b>GUI applications:</b> For Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with <a href="https://kivy.org">Kivy</a>.</li>
-> <li> <b>Pose refinement:</b> Click and move badly estimated 2D points. See <a href="https://www.youtube.com/watch?v=bEuBKB7eqmk">DeepLabCut</a> for inspiration.
-> <li> <b>Include OpenPose in Sports2D:</b> For example, <a href="https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile">Dockerize</a> it. Otherwise, run Sports2D in a <a href="https://colab.research.google.com/github/hardik0/AI-basketball-analysis-on-google-colab/blob/master/AI_basketball_analysis_google_colab.ipynb">Colab notebook</a>.
-> <li> <b>Constrain points</b> to OpenSim skeletal model for better angle estimation. Cf <a href="https://github.com/perfanalytics/pose2sim">Pose2Sim</a>, but in 2D.
-
-BSD 3-Clause License
-
-Copyright (c) 2022, perfanalytics
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Metadata-Version: 2.1
+Name: sports2d
+Version: 0.0.5
+Summary: Detect pose and compute 2D joint angles from a video.
+Home-page: https://github.com/davidpagnon/Sports2D
+Author: David Pagnon
+Author-email: contact@david-pagnon.com
+License: BSD 3-Clause License
+Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
+Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
+Requires-Python: <=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<!-- 
+[![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
+[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D) \
+[![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
+[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
+[![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
+-->
+
+
+# Sports2D
+
+**`Sports2D` lets you compute 2D joint and segment angles from a single video.**
+
+ </br>
+ </br>
+
+<img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
+
+`Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
+`Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
+If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.
+
+`Announcement:` Apps with GUI will be released for Windows, Linux, MacOS, as well as Android and iOS.
+Mobile versions will only support simple exploratory analysis. This involves single-person angle computation, in a potentially less accurate and tunable way.
+
+
+## Contents
+1. [Installation and Demonstration](#installation-and-demonstration)
+   1. [Installation](#installation)
+   2. [Demonstration: Detect pose and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles)
+2. [Go further](#go-further)
+   1. [Use on your own videos](#use-on-your-own-videos)
+   2. [Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-multi-person-more-accurate-analysis)
+   3. [Advanced-settings](#advanced-settings)
+   4. [How it works](#how-it-works)
+3. [How to cite and how to contribute](#how-to-cite-and-how-to-contribute)
+
+
+## Installation and Demonstration
+
+### Installation
+
+- OPTION 1: **Quick install:** \
+    Open a terminal. Type `python -V` to make sure python '>=3.7 <=3.10' is installed, and then:
+    ```
+    pip install sports2d
+    ```
+
+- OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
+    Open an Anaconda prompt and create a virtual environment by typing:
+    ```
+    conda create -n Sports2D python<=3.10 
+    conda activate Sports2D
+    pip install sports2d
+    ```
+
+- OPTION 3: **Build from source and test the last changes:**\
+     Open a terminal in the directory of your choice and clone the Sports2D repository.
+     ```
+     git clone https://github.com/davidpagnon/sports2d.git
+     cd sports2d
+     pip install .
+     ```
+
+
+### Demonstration: Detect pose and compute 2D angles
+
+Open a terminal, enter `pip show sports2d`, check sports2d package location. \
+Copy this path and go to the Demo folder by typing `cd <path>\Sports2D\Demo`. \
+Type `ipython`, and test the following code:
+```
+from Sports2D import Sports2D
+Sports2D.detect_pose('Config_demo.toml')
+Sports2D.compute_angles('Config_demo.toml')
+```
+
+<img src="Content/demo_blazepose_terminal.png" width="760">
+
+
+You should obtain a video with the overlaid 2D joint positions, and angle text values. This output is also provided as an image folder.\
+You should additionally obtain the same information as time series, stored in .csv files. These files can be opened with any spreadsheet software, or with the Pandas Python library for example.\
+In addition, you will get the original OpenPose-like json coordinates files.
+
+<img src="Content/demo_blazepose_results.png" width="760">
+
+
+## Go further
+
+### Use on your own videos
+
+1. Copy-paste `Config_demo.toml` in the directory of your video.
+
+2. Open it with any text editor.\
+Replace the `video_file` value with the name of your video.
+
+3. Open a terminal or an Anaconda prompt, type:
+   ```
+   cd <Path/to/video/directory>
+   conda activate Sports2D (skip if you did not install with Anaconda)
+   ipython
+   ```
+   ```
+   from Sports2D import Sports2D
+   Sports2D.detect_pose('Config_demo.toml')
+   Sports2D.compute_angles('Config_demo.toml')
+   ```
+
+*Optionally:* If your video is not in the same folder as `Config_demo.toml`, specify its location in `video_dir`.\
+Similarly, if you launch Sports2D in an other directory, specify the location of the config file this way: `Sports2D.detect_pose(<path_to_Config_demo.toml>)`\
+In `pose`, specify the use of BlazePose or OpenPose as joint detectors: this will be detailed in the next section.\
+In `compute_angles`, select your angles of interest.
+
+
+### Use OpenPose for multi-person, more accurate analysis
+
+OpenPose is slower than OpenPose, but more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
+
+1. **Install OpenPose** (instructions [there](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md)). \
+*Windows portable demo works fine.*
+
+2. If you want even more accurate results, use the BODY_25B experimental model instead of the standard BODY_25 one. This requires manually [downloading the model](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md). You can optionally download from there the BODY_135 model which will let you compute wrist flexion and hand segment angle, however this will be much slower.
+
+3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
+
+*N.B.:* If you want to benefit from the capabilities of OpenPose but do not manage to install it, you can use the `Colab notebook` version.\
+Note that your data will be sent to the Google servers, which do not follow the European GDPR requirements regarding privacy.
+**COMING SOON**
+
+<img src="Content/demo_blazepose_results.png" width="760">
+
+### Advanced settings
+
+1. `Config_demo.toml` → `pose_advanced`: These settings are only taken into account if OpenPose is used.
+   1. `load_pose`: If you need to change some settings but have already run a pose estimation, you can set this to `true` in order to not regenerate the json pose files.
+
+   2. `save_vid` and `save_img`: You can choose whether you want to save the resulting video and images. If set to `false`, only pose and angle `.csv` files will be generated.
+
+   3. `interp_gap_smaller_than`: Gaps are interpolated only if they are not too wide.
+   
+   4. `filter`: `true` or `false`. If `true`, you can choose among `Butterworth`, `Gaussian`, `LOESS`, or `Median`, and specify their parameters.\
+   Beware that the appearance of the unfiltered skeleton may not match the filtered coordinates and angles.
+
+   5. `show_plots`: Displays a window with tabs corresponding to the coordinates of each detected point. This may cause Python to crash.
+
+2. `Config_demo.toml` → `compute_angles_advanced`: These settings are taken into account both with BlazePose and OpenPose.
+   1. `save_vid` and `save_img`: Cf `pose_advanced`.
+
+   2. `filter`: Cf `pose_advanced`.
+
+   3. `show_plots`: Cf `pose_advanced`.
+
+   <img src="Content/demo_show_plots.png" width="760">
+
+*N.B.:* The settings and results of all analyses are stored int the `logs.txt` file, which can be found in in the sports2d installation folder (`pip show sports2d` to find the path).
+
+
+
+### How it works
+
+#### Pose detection:
+
+BlazePose or OpenPose are used to detect joint centers from a video.
+
+If `BlazePose` is used, only one person can be detected.\
+No interpolation nor filtering options are available. Not plotting available.
+
+If `OpenPose` is used, multiple persons can be consistently detected across frames. A person is matched to another in the next frame when their average point clouds are at a small euclidian distance.\
+Sequences of missing data are interpolated if they are less than N frames long.\
+Resulting coordinates can be filtered with Butterworth, gaussian, median, or loess filter. They can also be plotted.
+
+
+#### Angle computation:
+
+Joint and segment angles are computed from csv position files.\
+If a person suddently faces the other way, this change of direction is taken into account.\
+Resulting angles can be filtered in the same way as point coordinates, and they can also be plotted.
+
+**Joint angle conventions:**
+- Ankle dorsiflexion: Between heel and big toe, and ankle and knee
+- Knee flexion: Between hip, knee, and ankle 
+- Hip flexion: Between knee, hip, and shoulder
+- Shoulder flexion: Between hip, shoulder, and elbow
+- Elbow flexion: Between wrist, elbow, and shoulder
+
+**Segment angle conventions:**\
+Angles are measured anticlockwise between the horizontal and the segment.
+- Foot: Between heel and big toe
+- Shank: Between knee and ankle
+- Thigh: Between hip and knee
+- Arm: Between shoulder and elbow
+- Forearm: Between elbow and wrist
+- Trunk: Between shoulder midpoint and hip midpoint
+
+## How to cite and how to contribute
+
+### How to cite
+If you use this code or data, please cite [Pagnon, 2023].
+
+     @misc{Pagnon2023,
+       author = {Pagnon, David},
+       title = {Sports2D - Angles from monocular video},
+       year = {2013},
+       publisher = {GitHub},
+       journal = {GitHub repository},
+       howpublished = {\url{https://github.com/davidpagnon/Sports2D}},
+     }
+
+### How to contribute
+I would happily welcome any proposal for new features, code improvement, and more!\
+If you want to contribute to Sports2D, please follow [this guide](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) on how to fork, modify and push code, and submit a pull request. I would appreciate it if you provided as much useful information as possible about how you modified the code, and a rationale for why you're making this pull request. Please also specify on which operating system and on which python version you have tested the code.
+
+*Here is a to-do list, for general guidance purposes only:*
+> <li> <b>GUI applications:</b> For Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with <a href="https://kivy.org">Kivy</a>.</li>
+> <li> <b>Pose refinement:</b> Click and move badly estimated 2D points. See <a href="https://www.youtube.com/watch?v=bEuBKB7eqmk">DeepLabCut</a> for inspiration.
+> <li> <b>Include OpenPose in Sports2D:</b> For example, <a href="https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile">Dockerize</a> it. Otherwise, run Sports2D in a <a href="https://colab.research.google.com/github/hardik0/AI-basketball-analysis-on-google-colab/blob/master/AI_basketball_analysis_google_colab.ipynb">Colab notebook</a>.
+> <li> <b>Constrain points</b> to OpenSim skeletal model for better angle estimation. Cf <a href="https://github.com/perfanalytics/pose2sim">Pose2Sim</a>, but in 2D.
+
+BSD 3-Clause License
+
+Copyright (c) 2022, perfanalytics
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sports2d-0.0.2/sports2d.egg-info/SOURCES.txt` & `sports2d-0.0.5/sports2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

