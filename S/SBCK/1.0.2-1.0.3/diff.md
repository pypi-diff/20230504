# Comparing `tmp/SBCK-1.0.2.tar.gz` & `tmp/SBCK-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SBCK-1.0.2.tar", last modified: Wed May  3 08:11:21 2023, max compression
+gzip compressed data, was "SBCK-1.0.3.tar", last modified: Thu May  4 08:29:34 2023, max compression
```

## Comparing `SBCK-1.0.2.tar` & `SBCK-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,70 @@
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:11:21.054848 SBCK-1.0.2/
--rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-07-22 12:49:53.000000 SBCK-1.0.2/COPYING
--rw-r--r--   0 yrobin     (501) staff       (20)     7542 2023-05-03 08:11:21.054719 SBCK-1.0.2/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)     7523 2023-05-03 08:10:19.000000 SBCK-1.0.2/README.md
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-03 08:11:21.054538 SBCK-1.0.2/SBCK.egg-info/
--rw-r--r--   0 yrobin     (501) staff       (20)     7542 2023-05-03 08:11:21.000000 SBCK-1.0.2/SBCK.egg-info/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)     3401 2023-05-03 08:11:21.000000 SBCK-1.0.2/SBCK.egg-info/SOURCES.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-03 08:11:21.000000 SBCK-1.0.2/SBCK.egg-info/dependency_links.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-03 08:11:21.000000 SBCK-1.0.2/SBCK.egg-info/not-zip-safe
--rw-r--r--   0 yrobin     (501) staff       (20)       37 2023-05-03 08:11:21.000000 SBCK-1.0.2/SBCK.egg-info/requires.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        5 2023-05-03 08:11:21.000000 SBCK-1.0.2/SBCK.egg-info/top_level.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-03 08:11:21.054881 SBCK-1.0.2/setup.cfg
--rw-r--r--   0 yrobin     (501) staff       (20)     6124 2023-05-03 08:10:35.000000 SBCK-1.0.2/setup.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 08:29:34.730491 SBCK-1.0.3/
+-rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-07-22 12:49:53.000000 SBCK-1.0.3/COPYING
+-rw-r--r--   0 yrobin     (501) staff       (20)       75 2023-05-04 08:18:20.000000 SBCK-1.0.3/MANIFEST.in
+-rw-r--r--   0 yrobin     (501) staff       (20)     8620 2023-05-04 08:29:34.730285 SBCK-1.0.3/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)     7751 2023-05-04 08:21:32.000000 SBCK-1.0.3/README.md
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 08:29:34.721551 SBCK-1.0.3/SBCK/
+-rw-r--r--   0 yrobin     (501) staff       (20)     4410 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__AR2D2.py
+-rwxr-xr-x   0 yrobin     (501) staff       (20)    15418 2022-12-08 14:06:34.000000 SBCK-1.0.3/SBCK/__CDFt.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2852 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__ECBC.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2507 2022-10-13 05:36:33.000000 SBCK-1.0.3/SBCK/__IdBC.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     6267 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__MBCn.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     4650 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__MRec.py
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     4239 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__OTC.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3560 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__QDM.py
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     5515 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__QM.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2581 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__QMrs.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     4648 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__R2D2.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2865 2022-10-13 05:36:22.000000 SBCK-1.0.3/SBCK/__RBC.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3103 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__TSMBC.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2045 2023-03-21 07:36:05.000000 SBCK-1.0.3/SBCK/__XClimPPP.py
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     6238 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__dOTC.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3963 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/__dTSMBC.py
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     1250 2022-10-13 06:37:37.000000 SBCK-1.0.3/SBCK/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1041 2023-05-04 08:09:27.000000 SBCK-1.0.3/SBCK/__release.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 08:29:34.722047 SBCK-1.0.3/SBCK/datasets/
+-rw-r--r--   0 yrobin     (501) staff       (20)     1042 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/datasets/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     7350 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/datasets/__multivariates.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2605 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/datasets/__univariates.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 08:29:34.723516 SBCK-1.0.3/SBCK/metrics/
+-rw-r--r--   0 yrobin     (501) staff       (20)     1671 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/metrics/__chebyshev.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1616 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/metrics/__decorators.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1932 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/metrics/__energy.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1329 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/metrics/__entropy.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1223 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/metrics/__euclidean.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      979 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/metrics/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1224 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/metrics/__manhattan.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1955 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/metrics/__minkowski.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2108 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/metrics/__wasserstein.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 08:29:34.725183 SBCK-1.0.3/SBCK/ppp/
+-rw-r--r--   0 yrobin     (501) staff       (20)     5267 2023-04-06 07:36:11.000000 SBCK-1.0.3/SBCK/ppp/__PPPDiffRef.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    10424 2023-05-02 08:16:51.000000 SBCK-1.0.3/SBCK/ppp/__PPPLinkFunction.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     4789 2022-10-18 08:38:55.000000 SBCK-1.0.3/SBCK/ppp/__PPPNanValues.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3310 2023-05-02 08:24:56.000000 SBCK-1.0.3/SBCK/ppp/__PPPSSR.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1411 2023-04-06 07:28:37.000000 SBCK-1.0.3/SBCK/ppp/__PPPSys.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     6400 2023-03-21 07:37:00.000000 SBCK-1.0.3/SBCK/ppp/__PrePostProcessing.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1085 2022-10-19 07:29:22.000000 SBCK-1.0.3/SBCK/ppp/__checkf.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1540 2023-04-13 14:02:14.000000 SBCK-1.0.3/SBCK/ppp/__init__.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 08:29:34.726696 SBCK-1.0.3/SBCK/tools/
+-rw-r--r--   0 yrobin     (501) staff       (20)     1679 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/__Dist.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     6867 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/__OT.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3540 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/__Shift.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1644 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/__SlopeStoppingCriteria.py
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     1960 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/__bin_width_estimator.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1664 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    12112 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/__rv_extend.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    13439 2022-10-13 13:15:52.000000 SBCK-1.0.3/SBCK/tools/__shuffle.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 08:29:34.730067 SBCK-1.0.3/SBCK/tools/src/
+-rw-r--r--   0 yrobin     (501) staff       (20)     3460 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/src/NetworkSimplex.hpp
+-rw-r--r--   0 yrobin     (501) staff       (20)    65876 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/src/NetworkSimplexLemon.hpp
+-rw-r--r--   0 yrobin     (501) staff       (20)     6614 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/src/SparseHist.hpp
+-rw-r--r--   0 yrobin     (501) staff       (20)     3012 2022-07-22 12:49:53.000000 SBCK-1.0.3/SBCK/tools/src/tools.cpp
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-04 08:29:34.728435 SBCK-1.0.3/SBCK.egg-info/
+-rw-r--r--   0 yrobin     (501) staff       (20)     8620 2023-05-04 08:29:34.000000 SBCK-1.0.3/SBCK.egg-info/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)     2539 2023-05-04 08:29:34.000000 SBCK-1.0.3/SBCK.egg-info/SOURCES.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-04 08:29:34.000000 SBCK-1.0.3/SBCK.egg-info/dependency_links.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-04 08:29:34.000000 SBCK-1.0.3/SBCK.egg-info/not-zip-safe
+-rw-r--r--   0 yrobin     (501) staff       (20)       37 2023-05-04 08:29:34.000000 SBCK-1.0.3/SBCK.egg-info/requires.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        5 2023-05-04 08:29:34.000000 SBCK-1.0.3/SBCK.egg-info/top_level.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-04 08:29:34.730532 SBCK-1.0.3/setup.cfg
+-rw-r--r--   0 yrobin     (501) staff       (20)     6352 2023-05-04 08:22:22.000000 SBCK-1.0.3/setup.py
```

### Comparing `SBCK-1.0.2/COPYING` & `SBCK-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `SBCK-1.0.2/PKG-INFO` & `SBCK-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: SBCK
-Version: 1.0.2
+Version: 1.0.3
 Summary: Statistical Bias Correction Kit
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU General Public License v3
 Platform: linux
 Platform: macosx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # SBCK (Statistical Bias Correction Kit)
 
 ## Features
@@ -34,46 +38,58 @@
 - TSMBC method [15], for autocorrelations.
 
 ## How to select a bias correction method ?
 
 This summary of ability of each method to perform a bias correction is proposed by François, (2020). Please refer to
 this article for further interpretation.
 
-| Characteristics                             | CDF-t   | R2D2   | dOTC   | MBCn   | MRec   |
-|---------------------------------------------| :-----: | :----: | :----: | :----: | :----: |
-| Correction of univariate dist. prop.        | Yes     | Yes    | Yes    | Yes    | Yes    |
-| Modification of correlations of the model   | No      | Yes    | Yes    | Yes    | Yes    |
-| Capacity to correct inter-var. prop.        | No      | Yes    | Yes    | Yes    | Yes    |
-| Capacity to correct spatial prop.           | No      | Yes    | Yes    | ~      | ~      |
-| Capacity to correct temporal prop.          | No      | No     | No     | No     | No     |
-| Preserve the rank structure of the model    | Yes     | ~      | ~      | ~      | ~      |
-| Capacity to correct small geographical area | n.a.    | Yes    | Yes    | Yes    | Yes    |
-| Capacity to correct large geographical area | n.a.    | ~      | ~      | ~      | No     |
-| Allow for change of the multi-dim. prop.    | Yes     | No     | Yes    | ~      | Yes    |
+| Characteristics                             | CDF-t              | R2D2               | dOTC               | MBCn               | MRec               |
+|---------------------------------------------| :----------------: | :----------------: | :----------------: | :----------------: | :----------------: |
+| Correction of univariate dist. prop.        |  Yes               |  Yes               |  Yes               |  Yes               |  Yes               |
+| Modification of correlations of the model   |  No                |  Yes               |  Yes               |  Yes               |  Yes               |
+| Capacity to correct inter-var. prop.        |  No                |  Yes               |  Yes               |  Yes               |  Yes               |
+| Capacity to correct spatial prop.           |  No                |  Yes               |  Yes               |  ~                 |  ~                 |
+| Capacity to correct temporal prop.          |  No                |  No                |  No                |  No                |  No                |
+| Preserve the rank structure of the model    |  Yes               |  ~                 |  ~                 |  ~                 |  ~                 |
+| Capacity to correct small geographical area | n.a.               |  Yes               |  Yes               |  Yes               |  Yes               |
+| Capacity to correct large geographical area | n.a.               |  ~                 |  ~                 |  ~                 |  No                |
+| Allow for change of the multi-dim. prop.    |  Yes               |  No                |  Yes               |  ~                 |  Yes               |
 
 
 ## Python instruction
 
 Requires:
 - python3
 - [Eigen](http://eigen.tuxfamily.org/index.php?title=Main_Page)
 - numpy
 - scipy
 - pybind11
 
-For python, just use the command:
+You can install from pypi:
 ```
+pip3 install SBCK
+```
+
+Or from sources:
+```
+git clone https://github.com/yrobink/SBCK-python.git
+cd SBCK
 pip3 install .
 ```
 
 If the Eigen library is not found, use:
 ```
 pip3 install . eigen="path-to-eigen"
 ```
 
+## Acknowledgements
+
+Thanks to [[Trevor James Smith]](https://github.com/Zeitsperre) for his help with the publication on pypi.
+
+
 ## License
 
 Copyright(c) 2021 / 2023 Yoann Robin
 
 This file is part of SBCK.
 
 SBCK is free software: you can redistribute it and/or modify
```

### Comparing `SBCK-1.0.2/README.md` & `SBCK-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,24 +37,36 @@
 Requires:
 - python3
 - [Eigen](http://eigen.tuxfamily.org/index.php?title=Main_Page)
 - numpy
 - scipy
 - pybind11
 
-For python, just use the command:
+You can install from pypi:
 ```
+pip3 install SBCK
+```
+
+Or from sources:
+```
+git clone https://github.com/yrobink/SBCK-python.git
+cd SBCK
 pip3 install .
 ```
 
 If the Eigen library is not found, use:
 ```
 pip3 install . eigen="path-to-eigen"
 ```
 
+## Acknowledgements
+
+Thanks to [[Trevor James Smith]](https://github.com/Zeitsperre) for his help with the publication on pypi.
+
+
 ## License
 
 Copyright(c) 2021 / 2023 Yoann Robin
 
 This file is part of SBCK.
 
 SBCK is free software: you can redistribute it and/or modify
```

### Comparing `SBCK-1.0.2/SBCK.egg-info/PKG-INFO` & `SBCK-1.0.3/SBCK.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: SBCK
-Version: 1.0.2
+Version: 1.0.3
 Summary: Statistical Bias Correction Kit
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU General Public License v3
 Platform: linux
 Platform: macosx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # SBCK (Statistical Bias Correction Kit)
 
 ## Features
@@ -34,46 +38,58 @@
 - TSMBC method [15], for autocorrelations.
 
 ## How to select a bias correction method ?
 
 This summary of ability of each method to perform a bias correction is proposed by François, (2020). Please refer to
 this article for further interpretation.
 
-| Characteristics                             | CDF-t   | R2D2   | dOTC   | MBCn   | MRec   |
-|---------------------------------------------| :-----: | :----: | :----: | :----: | :----: |
-| Correction of univariate dist. prop.        | Yes     | Yes    | Yes    | Yes    | Yes    |
-| Modification of correlations of the model   | No      | Yes    | Yes    | Yes    | Yes    |
-| Capacity to correct inter-var. prop.        | No      | Yes    | Yes    | Yes    | Yes    |
-| Capacity to correct spatial prop.           | No      | Yes    | Yes    | ~      | ~      |
-| Capacity to correct temporal prop.          | No      | No     | No     | No     | No     |
-| Preserve the rank structure of the model    | Yes     | ~      | ~      | ~      | ~      |
-| Capacity to correct small geographical area | n.a.    | Yes    | Yes    | Yes    | Yes    |
-| Capacity to correct large geographical area | n.a.    | ~      | ~      | ~      | No     |
-| Allow for change of the multi-dim. prop.    | Yes     | No     | Yes    | ~      | Yes    |
+| Characteristics                             | CDF-t              | R2D2               | dOTC               | MBCn               | MRec               |
+|---------------------------------------------| :----------------: | :----------------: | :----------------: | :----------------: | :----------------: |
+| Correction of univariate dist. prop.        |  Yes               |  Yes               |  Yes               |  Yes               |  Yes               |
+| Modification of correlations of the model   |  No                |  Yes               |  Yes               |  Yes               |  Yes               |
+| Capacity to correct inter-var. prop.        |  No                |  Yes               |  Yes               |  Yes               |  Yes               |
+| Capacity to correct spatial prop.           |  No                |  Yes               |  Yes               |  ~                 |  ~                 |
+| Capacity to correct temporal prop.          |  No                |  No                |  No                |  No                |  No                |
+| Preserve the rank structure of the model    |  Yes               |  ~                 |  ~                 |  ~                 |  ~                 |
+| Capacity to correct small geographical area | n.a.               |  Yes               |  Yes               |  Yes               |  Yes               |
+| Capacity to correct large geographical area | n.a.               |  ~                 |  ~                 |  ~                 |  No                |
+| Allow for change of the multi-dim. prop.    |  Yes               |  No                |  Yes               |  ~                 |  Yes               |
 
 
 ## Python instruction
 
 Requires:
 - python3
 - [Eigen](http://eigen.tuxfamily.org/index.php?title=Main_Page)
 - numpy
 - scipy
 - pybind11
 
-For python, just use the command:
+You can install from pypi:
 ```
+pip3 install SBCK
+```
+
+Or from sources:
+```
+git clone https://github.com/yrobink/SBCK-python.git
+cd SBCK
 pip3 install .
 ```
 
 If the Eigen library is not found, use:
 ```
 pip3 install . eigen="path-to-eigen"
 ```
 
+## Acknowledgements
+
+Thanks to [[Trevor James Smith]](https://github.com/Zeitsperre) for his help with the publication on pypi.
+
+
 ## License
 
 Copyright(c) 2021 / 2023 Yoann Robin
 
 This file is part of SBCK.
 
 SBCK is free software: you can redistribute it and/or modify
```

### Comparing `SBCK-1.0.2/setup.py` & `SBCK-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 import os
 import sys
 import sysconfig
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 import setuptools
+from pathlib import Path
 
 
 #####################
 ## User Eigen path ##
 #####################
 
 eigen_usr_include = ""
@@ -45,15 +46,16 @@
 if i_eigen > -1:
 	del sys.argv[i_eigen]
 	
 ############################
 ## Python path resolution ##
 ############################
 
-here = os.path.abspath( os.path.dirname(__file__) )
+cpath = Path(__file__).parent
+
 
 ################################################################
 ## Some class and function to compile with Eigen and pybind11 ##
 ################################################################
 
 class get_pybind_include(object):##{{{
 	"""Helper class to determine the pybind11 include path
@@ -144,15 +146,15 @@
 ##########################
 ## Extension to compile ##
 ##########################
 
 ext_modules = [
 	Extension(
 		"SBCK.tools.__tools_cpp",
-		[ os.path.join(here, 'SBCK/tools/src/tools.cpp') ],
+		[ str(cpath / 'SBCK/tools/src/tools.cpp') ],
 		include_dirs=[
 			# Path to pybind11 headers
 			get_eigen_include(eigen_usr_include),
 			get_pybind_include(),
 			get_pybind_include(user=True)
 		],
 		language='c++',
@@ -177,25 +179,25 @@
 	"SBCK.datasets"
 ]
 
 ########################
 ## Infos from release ##
 ########################
 
-with open( os.path.join( here , "SBCK" , "__release.py" ) , "r" ) as f:
-	lines = f.readlines()
-exec("".join(lines))
+exec( (cpath / "SBCK" / "__release.py").read_text() )
 
 
 #################
 ## Description ##
 #################
-from pathlib import Path
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README-pypi.md").read_text()
+long_description = (cpath / "README.md").read_text()
+long_description = long_description.replace(":heavy_check_mark:"," Yes              ")
+long_description = long_description.replace(":x: "," No ")
+long_description = long_description.replace(":warning:"," ~       ")
+
 
 #######################
 ## And now the setup ##
 #######################
 
 setup(
 	name         = name,
@@ -210,18 +212,22 @@
 	classifiers      = [
 		"Development Status :: 5 - Production/Stable",
 		"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 		"Natural Language :: English",
 		"Operating System :: MacOS :: MacOS X",
 		"Operating System :: POSIX :: Linux",
 		"Programming Language :: Python :: 3",
+		"Programming Language :: Python :: 3.7",
+		"Programming Language :: Python :: 3.8",
+		"Programming Language :: Python :: 3.9",
+		"Programming Language :: Python :: 3.10",
 		"Topic :: Scientific/Engineering :: Mathematics"
 	],
 	ext_modules      = ext_modules,
 	install_requires = [ "numpy" , "scipy" , "matplotlib" , "pybind11>=2.2" ],
 	cmdclass         = {'build_ext': BuildExt},
 	zip_safe         = False,
 	packages         = list_packages,
-	package_dir      = { "SBCK" : os.path.join(here, "SBCK") }
+	package_dir      = { "SBCK" : "./SBCK" }
 )
```

