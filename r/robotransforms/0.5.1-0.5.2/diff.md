# Comparing `tmp/robotransforms-0.5.1.tar.gz` & `tmp/robotransforms-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotransforms-0.5.1.tar", last modified: Wed May  3 23:35:05 2023, max compression
+gzip compressed data, was "robotransforms-0.5.2.tar", last modified: Thu May  4 21:54:38 2023, max compression
```

## Comparing `robotransforms-0.5.1.tar` & `robotransforms-0.5.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:35:05.893479 robotransforms-0.5.1/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.5.1/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.5.1/MANIFEST.in
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-05-03 23:35:05.893479 robotransforms-0.5.1/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-05-03 23:31:19.000000 robotransforms-0.5.1/README.md
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2023-05-03 23:34:03.000000 robotransforms-0.5.1/pyproject.toml
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:35:05.889479 robotransforms-0.5.1/robotransforms/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.5.1/robotransforms/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-05-03 23:34:21.000000 robotransforms-0.5.1/robotransforms/_version.py
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:35:05.893479 robotransforms-0.5.1/robotransforms/dead_reckon/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.5.1/robotransforms/dead_reckon/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8894 2023-05-03 23:28:26.000000 robotransforms-0.5.1/robotransforms/dead_reckon/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.5.1/robotransforms/dead_reckon/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.5.1/robotransforms/dead_reckon/dead_reckon.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6684 2023-05-03 23:28:26.000000 robotransforms-0.5.1/robotransforms/dead_reckon/dead_reckon_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.5.1/robotransforms/dead_reckon/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:35:05.893479 robotransforms-0.5.1/robotransforms/euclidean/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.5.1/robotransforms/euclidean/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8310 2023-05-03 23:28:26.000000 robotransforms-0.5.1/robotransforms/euclidean/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1566 2023-05-03 23:28:26.000000 robotransforms-0.5.1/robotransforms/euclidean/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11585 2023-05-03 23:28:26.000000 robotransforms-0.5.1/robotransforms/euclidean/euclidean.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14304 2023-05-03 23:28:26.000000 robotransforms-0.5.1/robotransforms/euclidean/euclidean_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6960 2023-05-03 23:28:26.000000 robotransforms-0.5.1/robotransforms/euclidean/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:35:05.893479 robotransforms-0.5.1/robotransforms/utils/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.5.1/robotransforms/utils/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.5.1/robotransforms/utils/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.5.1/robotransforms/utils/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.5.1/robotransforms/utils/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.5.1/robotransforms/utils/utils_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.5.1/robotransforms/utils/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-03 23:35:05.889479 robotransforms-0.5.1/robotransforms.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-05-03 23:35:05.000000 robotransforms-0.5.1/robotransforms.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-05-03 23:35:05.000000 robotransforms-0.5.1/robotransforms.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-03 23:35:05.000000 robotransforms-0.5.1/robotransforms.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-05-03 23:35:05.000000 robotransforms-0.5.1/robotransforms.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-05-03 23:35:05.000000 robotransforms-0.5.1/robotransforms.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-03 23:35:05.893479 robotransforms-0.5.1/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.5.1/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.364235 robotransforms-0.5.2/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.5.2/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.5.2/MANIFEST.in
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-05-04 21:54:38.364235 robotransforms-0.5.2/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-05-03 23:31:19.000000 robotransforms-0.5.2/README.md
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2023-05-03 23:34:03.000000 robotransforms-0.5.2/pyproject.toml
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.352235 robotransforms-0.5.2/robotransforms/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-05-04 21:53:50.000000 robotransforms-0.5.2/robotransforms/_version.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.360235 robotransforms-0.5.2/robotransforms/dead_reckon/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/dead_reckon/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8894 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/dead_reckon/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/dead_reckon/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.5.2/robotransforms/dead_reckon/dead_reckon.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6652 2023-05-04 21:53:40.000000 robotransforms-0.5.2/robotransforms/dead_reckon/dead_reckon_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.5.2/robotransforms/dead_reckon/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.364235 robotransforms-0.5.2/robotransforms/euclidean/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/euclidean/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8310 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/euclidean/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1566 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/euclidean/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11585 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/euclidean/euclidean.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14307 2023-05-04 15:04:49.000000 robotransforms-0.5.2/robotransforms/euclidean/euclidean_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6960 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/euclidean/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.364235 robotransforms-0.5.2/robotransforms/utils/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.5.2/robotransforms/utils/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/utils_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.360235 robotransforms-0.5.2/robotransforms.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-04 21:54:38.364235 robotransforms-0.5.2/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.5.2/setup.py
```

### Comparing `robotransforms-0.5.1/LICENSE` & `robotransforms-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/PKG-INFO` & `robotransforms-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.5.1
+Version: 0.5.2
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.5.1/robotransforms/dead_reckon/base.cpp` & `robotransforms-0.5.2/robotransforms/dead_reckon/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/dead_reckon/base.h` & `robotransforms-0.5.2/robotransforms/dead_reckon/base.h`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/dead_reckon/dead_reckon.py` & `robotransforms-0.5.2/robotransforms/dead_reckon/dead_reckon.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/dead_reckon/dead_reckon_pure.py` & `robotransforms-0.5.2/robotransforms/dead_reckon/dead_reckon_pure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import matplotlib.pyplot as plt
 
 from .. import euclidean as t
 # from ..euclidean import pure as t
 
 def DeadReckonStep(timestamp, dl, dr, Dq, vave, vdiff):
     return np.array([ timestamp, dl, dr, Dq[0], Dq[1], Dq[2], Dq[3], vave, vdiff ])
```

### Comparing `robotransforms-0.5.1/robotransforms/dead_reckon/wrapper.cpp` & `robotransforms-0.5.2/robotransforms/dead_reckon/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/euclidean/base.cpp` & `robotransforms-0.5.2/robotransforms/euclidean/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/euclidean/base.h` & `robotransforms-0.5.2/robotransforms/euclidean/base.h`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/euclidean/euclidean.py` & `robotransforms-0.5.2/robotransforms/euclidean/euclidean.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/euclidean/euclidean_pure.py` & `robotransforms-0.5.2/robotransforms/euclidean/euclidean_pure.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,17 +469,17 @@
         rq[2],
     ])
 
 def lrrv2lrQ(lrrv):
     q = rotvec2quat(lrrv[3:])
 
     return np.array([
-        lrq[0],
-        lrq[1],
-        lrq[2],
+        lrrv[0],
+        lrrv[1],
+        lrrv[2],
         q[0],
         q[1],
         q[2],
         q[3]
     ])
 
 def lrQ2lrrv(lrQ):
```

### Comparing `robotransforms-0.5.1/robotransforms/euclidean/wrapper.cpp` & `robotransforms-0.5.2/robotransforms/euclidean/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/utils/base.cpp` & `robotransforms-0.5.2/robotransforms/utils/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/utils/utils.py` & `robotransforms-0.5.2/robotransforms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/utils/utils_pure.py` & `robotransforms-0.5.2/robotransforms/utils/utils_pure.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms/utils/wrapper.cpp` & `robotransforms-0.5.2/robotransforms/utils/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/robotransforms.egg-info/PKG-INFO` & `robotransforms-0.5.2/robotransforms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.5.1
+Version: 0.5.2
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.5.1/robotransforms.egg-info/SOURCES.txt` & `robotransforms-0.5.2/robotransforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.1/setup.py` & `robotransforms-0.5.2/setup.py`

 * *Files identical despite different names*

