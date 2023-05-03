# Comparing `tmp/sports2d-0.0.1.tar.gz` & `tmp/sports2d-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.0.1.tar", last modified: Wed May  3 23:01:33 2023, max compression
+gzip compressed data, was "sports2d-0.0.2.tar", last modified: Wed May  3 23:15:54 2023, max compression
```

## Comparing `sports2d-0.0.1.tar` & `sports2d-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 23:01:33.104509 sports2d-0.0.1/
--rw-rw-rw-   0        0        0     1550 2023-02-05 04:03:13.000000 sports2d-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    14167 2023-05-03 23:01:33.105529 sports2d-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11462 2023-05-03 22:50:37.000000 sports2d-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 23:01:33.076475 sports2d-0.0.1/Sports2D/
-drwxrwxrwx   0        0        0        0 2023-05-03 23:01:33.079475 sports2d-0.0.1/Sports2D/Demo/
--rw-rw-rw-   0        0        0     3120 2023-05-03 22:48:24.000000 sports2d-0.0.1/Sports2D/Demo/Config_demo.toml
--rw-rw-rw-   0        0        0  2539508 2023-05-02 13:57:16.000000 sports2d-0.0.1/Sports2D/Demo/demo.mp4
--rw-rw-rw-   0        0        0     7515 2023-05-02 14:06:35.000000 sports2d-0.0.1/Sports2D/Sports2D.py
--rw-rw-rw-   0        0        0      110 2023-05-03 22:57:13.000000 sports2d-0.0.1/Sports2D/__init__.py
--rw-rw-rw-   0        0        0    22160 2023-05-03 22:48:13.000000 sports2d-0.0.1/Sports2D/compute_angles.py
--rw-rw-rw-   0        0        0    22224 2023-05-02 13:41:54.000000 sports2d-0.0.1/Sports2D/detect_pose.py
--rw-rw-rw-   0        0        0      113 2023-02-05 04:03:13.000000 sports2d-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1386 2023-05-03 23:01:33.106480 sports2d-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-02-05 04:03:13.000000 sports2d-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 23:01:33.104509 sports2d-0.0.1/sports2d.egg-info/
--rw-rw-rw-   0        0        0    14167 2023-05-03 23:01:33.000000 sports2d-0.0.1/sports2d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-05-03 23:01:33.000000 sports2d-0.0.1/sports2d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 23:01:33.000000 sports2d-0.0.1/sports2d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 23:01:32.000000 sports2d-0.0.1/sports2d.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       98 2023-05-03 23:01:33.000000 sports2d-0.0.1/sports2d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 23:01:33.000000 sports2d-0.0.1/sports2d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.842070 sports2d-0.0.2/
+-rw-rw-rw-   0        0        0     1550 2023-02-05 04:03:13.000000 sports2d-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    14167 2023-05-03 23:15:54.842070 sports2d-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11462 2023-05-03 23:15:23.000000 sports2d-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.791592 sports2d-0.0.2/Sports2D/
+drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.791592 sports2d-0.0.2/Sports2D/Demo/
+-rw-rw-rw-   0        0        0     3120 2023-05-03 22:48:24.000000 sports2d-0.0.2/Sports2D/Demo/Config_demo.toml
+-rw-rw-rw-   0        0        0  2539508 2023-05-02 13:57:16.000000 sports2d-0.0.2/Sports2D/Demo/demo.mp4
+-rw-rw-rw-   0        0        0     7515 2023-05-02 14:06:35.000000 sports2d-0.0.2/Sports2D/Sports2D.py
+drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.809572 sports2d-0.0.2/Sports2D/Utilities/
+-rw-rw-rw-   0        0        0    11135 2023-05-02 00:51:53.000000 sports2d-0.0.2/Sports2D/Utilities/Blazepose_runsave.py
+-rw-rw-rw-   0        0        0      108 2023-04-06 11:56:03.000000 sports2d-0.0.2/Sports2D/Utilities/__init__.py
+-rw-rw-rw-   0        0        0     4511 2023-05-01 19:27:34.000000 sports2d-0.0.2/Sports2D/Utilities/common.py
+-rw-rw-rw-   0        0        0     5086 2023-04-28 13:37:20.000000 sports2d-0.0.2/Sports2D/Utilities/filter.py
+-rw-rw-rw-   0        0        0    15791 2023-04-28 13:24:23.000000 sports2d-0.0.2/Sports2D/Utilities/skeletons.py
+-rw-rw-rw-   0        0        0      110 2023-05-03 22:57:13.000000 sports2d-0.0.2/Sports2D/__init__.py
+-rw-rw-rw-   0        0        0    22160 2023-05-03 22:48:13.000000 sports2d-0.0.2/Sports2D/compute_angles.py
+-rw-rw-rw-   0        0        0    22224 2023-05-02 13:41:54.000000 sports2d-0.0.2/Sports2D/detect_pose.py
+-rw-rw-rw-   0        0        0      113 2023-02-05 04:03:13.000000 sports2d-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1386 2023-05-03 23:15:54.848069 sports2d-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-02-05 04:03:13.000000 sports2d-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 23:15:54.841069 sports2d-0.0.2/sports2d.egg-info/
+-rw-rw-rw-   0        0        0    14167 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       98 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 23:15:54.000000 sports2d-0.0.2/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.0.1/LICENSE` & `sports2d-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.1/PKG-INFO` & `sports2d-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics
@@ -74,15 +74,15 @@
     ```
     pip install sports2d
     ```
 
 - OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
     Open an Anaconda prompt and create a virtual environment by typing:
     ```
-    conda create -n Sports2D python>=3.10 
+    conda create -n Sports2D python<=3.10 
     conda activate Sports2D
     pip install sports2d
     ```
 
 - OPTION 3: **Build from source and test the last changes:**\
      Open a terminal in the directory of your choice and clone the Sports2D repository.
      ```
```

### Comparing `sports2d-0.0.1/README.md` & `sports2d-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     ```
     pip install sports2d
     ```
 
 - OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
     Open an Anaconda prompt and create a virtual environment by typing:
     ```
-    conda create -n Sports2D python>=3.10 
+    conda create -n Sports2D python<=3.10 
     conda activate Sports2D
     pip install sports2d
     ```
 
 - OPTION 3: **Build from source and test the last changes:**\
      Open a terminal in the directory of your choice and clone the Sports2D repository.
      ```
```

### Comparing `sports2d-0.0.1/Sports2D/Demo/Config_demo.toml` & `sports2d-0.0.2/Sports2D/Demo/Config_demo.toml`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.1/Sports2D/Demo/demo.mp4` & `sports2d-0.0.2/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.1/Sports2D/Sports2D.py` & `sports2d-0.0.2/Sports2D/Sports2D.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.1/Sports2D/compute_angles.py` & `sports2d-0.0.2/Sports2D/compute_angles.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.1/Sports2D/detect_pose.py` & `sports2d-0.0.2/Sports2D/detect_pose.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.1/setup.cfg` & `sports2d-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 706f 7274 7332 640d 0a76 6572   = sports2d..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e31 0d0a 6175  sion = 0.0.1..au
+00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6175  sion = 0.0.2..au
 00000030: 7468 6f72 203d 2044 6176 6964 2050 6167  thor = David Pag
 00000040: 6e6f 6e0d 0a61 7574 686f 725f 656d 6169  non..author_emai
 00000050: 6c20 3d20 636f 6e74 6163 7440 6461 7669  l = contact@davi
 00000060: 642d 7061 676e 6f6e 2e63 6f6d 0d0a 6465  d-pagnon.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4465 7465  scription = Dete
 00000080: 6374 2070 6f73 6520 616e 6420 636f 6d70  ct pose and comp
 00000090: 7574 6520 3244 206a 6f69 6e74 2061 6e67  ute 2D joint ang
```

### Comparing `sports2d-0.0.1/sports2d.egg-info/PKG-INFO` & `sports2d-0.0.2/sports2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics
@@ -74,15 +74,15 @@
     ```
     pip install sports2d
     ```
 
 - OPTION 2: **Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html):** \
     Open an Anaconda prompt and create a virtual environment by typing:
     ```
-    conda create -n Sports2D python>=3.10 
+    conda create -n Sports2D python<=3.10 
     conda activate Sports2D
     pip install sports2d
     ```
 
 - OPTION 3: **Build from source and test the last changes:**\
      Open a terminal in the directory of your choice and clone the Sports2D repository.
      ```
```

