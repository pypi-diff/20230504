# Comparing `tmp/polysplit-0.1.2.tar.gz` & `tmp/polysplit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polysplit-0.1.2.tar", last modified: Thu May  4 19:43:03 2023, max compression
+gzip compressed data, was "polysplit-0.1.3.tar", last modified: Thu May  4 20:05:52 2023, max compression
```

## Comparing `polysplit-0.1.2.tar` & `polysplit-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.408188 polysplit-0.1.2/
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.402845 polysplit-0.1.2/.github/
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.403772 polysplit-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      834 2023-02-20 05:22:23.000000 polysplit-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      595 2023-02-20 05:22:23.000000 polysplit-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      118 2023-04-23 22:51:26.000000 polysplit-0.1.2/.github/dependabot.yml
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.404189 polysplit-0.1.2/.github/workflows/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1154 2023-04-23 22:51:26.000000 polysplit-0.1.2/.github/workflows/build.yml
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       55 2023-04-23 22:51:26.000000 polysplit-0.1.2/.gitignore
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1986 2023-04-23 22:51:26.000000 polysplit-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1073 2023-02-20 05:22:23.000000 polysplit-0.1.2/LICENSE
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       44 2023-04-23 22:51:26.000000 polysplit-0.1.2/MANIFEST.in
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2225 2023-04-23 22:51:26.000000 polysplit-0.1.2/Makefile
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     4236 2023-05-04 19:43:03.407934 polysplit-0.1.2/PKG-INFO
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2107 2023-04-23 22:51:26.000000 polysplit-0.1.2/README.md
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.405043 polysplit-0.1.2/polysplit/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      362 2023-04-23 22:51:26.000000 polysplit-0.1.2/polysplit/__init__.py
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     8601 2023-04-23 22:51:26.000000 polysplit-0.1.2/polysplit/polysplit.py
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.407286 polysplit-0.1.2/polysplit/tests/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 22:51:26.000000 polysplit-0.1.2/polysplit/tests/__init__.py
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2497 2023-04-23 22:51:26.000000 polysplit-0.1.2/polysplit/tests/test_polysplit.py
-drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 19:43:03.406586 polysplit-0.1.2/polysplit.egg-info/
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     4236 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/PKG-INFO
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      507 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/SOURCES.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)        1 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/dependency_links.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      254 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/requires.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       10 2023-05-04 19:43:03.000000 polysplit-0.1.2/polysplit.egg-info/top_level.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2699 2023-05-04 19:31:08.000000 polysplit-0.1.2/pyproject.toml
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      224 2023-04-23 22:51:26.000000 polysplit-0.1.2/requirements.txt
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       38 2023-05-04 19:43:03.408277 polysplit-0.1.2/setup.cfg
--rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      347 2023-05-04 18:17:46.000000 polysplit-0.1.2/setup.py
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 20:05:52.358199 polysplit-0.1.3/
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 20:05:52.350741 polysplit-0.1.3/.github/
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 20:05:52.351839 polysplit-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      834 2023-02-20 05:22:23.000000 polysplit-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      595 2023-02-20 05:22:23.000000 polysplit-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      118 2023-04-23 22:51:26.000000 polysplit-0.1.3/.github/dependabot.yml
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 20:05:52.352542 polysplit-0.1.3/.github/workflows/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1154 2023-04-23 22:51:26.000000 polysplit-0.1.3/.github/workflows/build.yml
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       55 2023-04-23 22:51:26.000000 polysplit-0.1.3/.gitignore
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1986 2023-04-23 22:51:26.000000 polysplit-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1073 2023-02-20 05:22:23.000000 polysplit-0.1.3/LICENSE
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       44 2023-04-23 22:51:26.000000 polysplit-0.1.3/MANIFEST.in
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2225 2023-04-23 22:51:26.000000 polysplit-0.1.3/Makefile
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     4437 2023-05-04 20:05:52.357695 polysplit-0.1.3/PKG-INFO
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2330 2023-05-04 20:01:01.000000 polysplit-0.1.3/README.md
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 20:05:52.353823 polysplit-0.1.3/polysplit/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      362 2023-04-23 22:51:26.000000 polysplit-0.1.3/polysplit/__init__.py
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 20:05:52.355912 polysplit-0.1.3/polysplit/docs/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     1167 2023-05-03 21:42:04.000000 polysplit-0.1.3/polysplit/docs/conf.py
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     8601 2023-04-23 22:51:26.000000 polysplit-0.1.3/polysplit/polysplit.py
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 20:05:52.356896 polysplit-0.1.3/polysplit/tests/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)        0 2023-04-23 22:51:26.000000 polysplit-0.1.3/polysplit/tests/__init__.py
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2497 2023-04-23 22:51:26.000000 polysplit-0.1.3/polysplit/tests/test_polysplit.py
+drwxr-xr-x   0 yaroslavzakharov   (501) staff       (20)        0 2023-05-04 20:05:52.355616 polysplit-0.1.3/polysplit.egg-info/
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     4437 2023-05-04 20:05:52.000000 polysplit-0.1.3/polysplit.egg-info/PKG-INFO
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      521 2023-05-04 20:05:52.000000 polysplit-0.1.3/polysplit.egg-info/SOURCES.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)        1 2023-05-04 20:05:52.000000 polysplit-0.1.3/polysplit.egg-info/dependency_links.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      316 2023-05-04 20:05:52.000000 polysplit-0.1.3/polysplit.egg-info/requires.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       10 2023-05-04 20:05:52.000000 polysplit-0.1.3/polysplit.egg-info/top_level.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)     2491 2023-05-04 20:03:37.000000 polysplit-0.1.3/pyproject.toml
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)      224 2023-04-23 22:51:26.000000 polysplit-0.1.3/requirements.txt
+-rw-r--r--   0 yaroslavzakharov   (501) staff       (20)       38 2023-05-04 20:05:52.358295 polysplit-0.1.3/setup.cfg
```

### Comparing `polysplit-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `polysplit-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `polysplit-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.2/.github/workflows/build.yml` & `polysplit-0.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.2/CONTRIBUTING.md` & `polysplit-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.2/LICENSE` & `polysplit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.2/Makefile` & `polysplit-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.2/PKG-INFO` & `polysplit-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polysplit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library implementing a method for splitting a polygon into regions
 Author-email: Dmitrii Zakharov <d.zakharov@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Dmitrii Zakharov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,25 +33,25 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 Provides-Extra: develop
 License-File: LICENSE
 
 # polysplit
 
 A lightweight library for splitting polygons into regions based on proximity of points.\
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 ![issues](https://img.shields.io/github/issues/r1p71d3/polysplit)
 [![codecov](https://codecov.io/gh/r1p71d3/polysplit/branch/main/graph/badge.svg?token=8S2VJLZG7U)](https://codecov.io/gh/r1p71d3/polysplit)
 [![Build Status](https://github.com/r1p71d3/polysplit/actions/workflows/build.yml/badge.svg)](https://github.com/r1p71d3/polysplit/actions/workflows/build.yml)
+[![Documentation](https://img.shields.io/badge/docs-GitHub%20Pages-blue)](https://r1p71d3.github.io/polysplit/)
 
 
 ## Overview
 Map quantization is the procedure of dividing a continuous map into a number of discrete regions. The simplest approach that has been used for hundreds of years is to overlap the map with a square grid. However, this approach ignores the geographical features of the map, making it suboptimal for certain applications. With this project, I would like to propose a novel algorithm that organically divides any given map into regions based on the relative travel time between different areas.
 
 In its simple form, the proposed algorithm could be applied to a map (a polygon) with intraversible obstacles (holes). It works in 2 stages. In the first stage, the map is overlayed with a fine grid of $N$ points. Then, we calculate the shortest path (around the obstacles) betweeen every pair of points and construct the $N \times N$ distance matrix. In the second stage, we apply the k-medoids algorithm to the set of points, using the matrix from stage I as a distance function, and retrieve a set of $M$ centers. Finally, we construct a Voronoi graph around the centers, creating the regions.
 
@@ -70,7 +70,10 @@
 hole_coords = [(0.4, 0.4), (0.4, 0.6), (0.6, 0.6), (0.6, 0.4)]
 polygon = Polygon(outer_coords, [hole_coords])
 
 # Split the polygon
 regions = polysplit.polysplit_main(polygon, k=5, num_points=100, plot=True)
 print(regions)
 ```
+
+## Documentation
+You can find the most up-to-date documentation [here](https://r1p71d3.github.io/polysplit/).
```

### Comparing `polysplit-0.1.2/README.md` & `polysplit-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # polysplit
 
 A lightweight library for splitting polygons into regions based on proximity of points.\
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 ![issues](https://img.shields.io/github/issues/r1p71d3/polysplit)
 [![codecov](https://codecov.io/gh/r1p71d3/polysplit/branch/main/graph/badge.svg?token=8S2VJLZG7U)](https://codecov.io/gh/r1p71d3/polysplit)
 [![Build Status](https://github.com/r1p71d3/polysplit/actions/workflows/build.yml/badge.svg)](https://github.com/r1p71d3/polysplit/actions/workflows/build.yml)
+[![Documentation](https://img.shields.io/badge/docs-GitHub%20Pages-blue)](https://r1p71d3.github.io/polysplit/)
 
 
 ## Overview
 Map quantization is the procedure of dividing a continuous map into a number of discrete regions. The simplest approach that has been used for hundreds of years is to overlap the map with a square grid. However, this approach ignores the geographical features of the map, making it suboptimal for certain applications. With this project, I would like to propose a novel algorithm that organically divides any given map into regions based on the relative travel time between different areas.
 
 In its simple form, the proposed algorithm could be applied to a map (a polygon) with intraversible obstacles (holes). It works in 2 stages. In the first stage, the map is overlayed with a fine grid of $N$ points. Then, we calculate the shortest path (around the obstacles) betweeen every pair of points and construct the $N \times N$ distance matrix. In the second stage, we apply the k-medoids algorithm to the set of points, using the matrix from stage I as a distance function, and retrieve a set of $M$ centers. Finally, we construct a Voronoi graph around the centers, creating the regions.
 
@@ -27,7 +28,10 @@
 hole_coords = [(0.4, 0.4), (0.4, 0.6), (0.6, 0.6), (0.6, 0.4)]
 polygon = Polygon(outer_coords, [hole_coords])
 
 # Split the polygon
 regions = polysplit.polysplit_main(polygon, k=5, num_points=100, plot=True)
 print(regions)
 ```
+
+## Documentation
+You can find the most up-to-date documentation [here](https://r1p71d3.github.io/polysplit/).
```

### Comparing `polysplit-0.1.2/polysplit/polysplit.py` & `polysplit-0.1.3/polysplit/polysplit.py`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.2/polysplit/tests/test_polysplit.py` & `polysplit-0.1.3/polysplit/tests/test_polysplit.py`

 * *Files identical despite different names*

### Comparing `polysplit-0.1.2/polysplit.egg-info/PKG-INFO` & `polysplit-0.1.3/polysplit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polysplit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library implementing a method for splitting a polygon into regions
 Author-email: Dmitrii Zakharov <d.zakharov@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Dmitrii Zakharov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,25 +33,25 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 Provides-Extra: develop
 License-File: LICENSE
 
 # polysplit
 
 A lightweight library for splitting polygons into regions based on proximity of points.\
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 ![issues](https://img.shields.io/github/issues/r1p71d3/polysplit)
 [![codecov](https://codecov.io/gh/r1p71d3/polysplit/branch/main/graph/badge.svg?token=8S2VJLZG7U)](https://codecov.io/gh/r1p71d3/polysplit)
 [![Build Status](https://github.com/r1p71d3/polysplit/actions/workflows/build.yml/badge.svg)](https://github.com/r1p71d3/polysplit/actions/workflows/build.yml)
+[![Documentation](https://img.shields.io/badge/docs-GitHub%20Pages-blue)](https://r1p71d3.github.io/polysplit/)
 
 
 ## Overview
 Map quantization is the procedure of dividing a continuous map into a number of discrete regions. The simplest approach that has been used for hundreds of years is to overlap the map with a square grid. However, this approach ignores the geographical features of the map, making it suboptimal for certain applications. With this project, I would like to propose a novel algorithm that organically divides any given map into regions based on the relative travel time between different areas.
 
 In its simple form, the proposed algorithm could be applied to a map (a polygon) with intraversible obstacles (holes). It works in 2 stages. In the first stage, the map is overlayed with a fine grid of $N$ points. Then, we calculate the shortest path (around the obstacles) betweeen every pair of points and construct the $N \times N$ distance matrix. In the second stage, we apply the k-medoids algorithm to the set of points, using the matrix from stage I as a distance function, and retrieve a set of $M$ centers. Finally, we construct a Voronoi graph around the centers, creating the regions.
 
@@ -70,7 +70,10 @@
 hole_coords = [(0.4, 0.4), (0.4, 0.6), (0.6, 0.6), (0.6, 0.4)]
 polygon = Polygon(outer_coords, [hole_coords])
 
 # Split the polygon
 regions = polysplit.polysplit_main(polygon, k=5, num_points=100, plot=True)
 print(regions)
 ```
+
+## Documentation
+You can find the most up-to-date documentation [here](https://r1p71d3.github.io/polysplit/).
```

### Comparing `polysplit-0.1.2/pyproject.toml` & `polysplit-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 [build-system]
 requires = [
     "setuptools",
     "setuptools-scm",
     "wheel",
-    "black>=22",
-    "bump2version>=1.0.0",
-    "check-manifest",
-    "flake8>=3.7.8",
-    "flake8-black>=0.2.1",
-    "flake8-pyproject",
-    "mypy",
-    "pytest>=4.3.0",
-    "pytest-cov>=2.6.1",
-    "twine",
-    "matplotlib",
-    "shapely",
-    "numpy",
-    "scikit-learn>=1.2.1",
-    "scikit-learn-extra>=0.2.0",
-    "networkx"
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "polysplit"
 authors = [{name = "Dmitrii Zakharov", email = "d.zakharov@columbia.edu"}]
 description="A Python library implementing a method for splitting a polygon into regions"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.7"
 
-dependencies = []
+dependencies = [
+    "matplotlib",
+    "shapely",
+    "numpy",
+    "scikit-learn>=1.2.1",
+    "scikit-learn-extra>=0.2.0",
+    "networkx"
+]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

