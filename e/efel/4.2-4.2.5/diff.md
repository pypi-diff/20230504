# Comparing `tmp/efel-4.2.tar.gz` & `tmp/efel-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-4.2.tar", last modified: Mon May  1 12:39:32 2023, max compression
+gzip compressed data, was "efel-4.2.5.tar", last modified: Thu May  4 12:10:02 2023, max compression
```

## Comparing `efel-4.2.tar` & `efel-4.2.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 12:39:32.315704 efel-4.2/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-01 12:39:30.000000 efel-4.2/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-05-01 12:39:30.000000 efel-4.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-05-01 12:39:30.000000 efel-4.2/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-05-01 12:39:30.000000 efel-4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-05-01 12:39:30.000000 efel-4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-01 12:39:32.315704 efel-4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-05-01 12:39:30.000000 efel-4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 12:39:32.319704 efel-4.2/efel/
--rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-05-01 12:39:30.000000 efel-4.2/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-05-01 12:39:30.000000 efel-4.2/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-05-01 12:39:32.319704 efel-4.2/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-05-01 12:39:30.000000 efel-4.2/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 12:39:32.315704 efel-4.2/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV4.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV4.h
--rw-r--r--   0 runner    (1001) docker     (122)   137180 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/efel.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/efel.h
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-05-01 12:39:30.000000 efel-4.2/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-05-01 12:39:30.000000 efel-4.2/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 12:39:32.315704 efel-4.2/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-01 12:39:30.000000 efel-4.2/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10308 2023-05-01 12:39:30.000000 efel-4.2/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-01 12:39:30.000000 efel-4.2/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 12:39:32.315704 efel-4.2/efel/units/
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-05-01 12:39:30.000000 efel-4.2/efel/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-05-01 12:39:30.000000 efel-4.2/efel/units/units.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 12:39:32.315704 efel-4.2/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-01 12:39:32.000000 efel-4.2/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-01 12:39:32.000000 efel-4.2/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 12:39:32.000000 efel-4.2/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-01 12:39:32.000000 efel-4.2/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 12:39:32.000000 efel-4.2/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-01 12:39:32.319704 efel-4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-05-01 12:39:30.000000 efel-4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-05-01 12:39:30.000000 efel-4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:10:02.699783 efel-4.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-04 12:10:00.000000 efel-4.2.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-05-04 12:10:00.000000 efel-4.2.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-05-04 12:10:00.000000 efel-4.2.5/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-05-04 12:10:00.000000 efel-4.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-05-04 12:10:00.000000 efel-4.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-04 12:10:02.699783 efel-4.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-05-04 12:10:00.000000 efel-4.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:10:02.703784 efel-4.2.5/efel/
+-rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-05-04 12:10:00.000000 efel-4.2.5/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-05-04 12:10:00.000000 efel-4.2.5/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-04 12:10:02.703784 efel-4.2.5/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-05-04 12:10:00.000000 efel-4.2.5/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:10:02.699783 efel-4.2.5/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV4.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV4.h
+-rw-r--r--   0 runner    (1001) docker     (122)   137180 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/efel.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/efel.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-05-04 12:10:00.000000 efel-4.2.5/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-05-04 12:10:00.000000 efel-4.2.5/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:10:02.699783 efel-4.2.5/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-04 12:10:00.000000 efel-4.2.5/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10309 2023-05-04 12:10:00.000000 efel-4.2.5/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-04 12:10:00.000000 efel-4.2.5/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:10:02.699783 efel-4.2.5/efel/units/
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-05-04 12:10:00.000000 efel-4.2.5/efel/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-05-04 12:10:00.000000 efel-4.2.5/efel/units/units.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 12:10:02.695782 efel-4.2.5/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-04 12:10:02.000000 efel-4.2.5/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-04 12:10:02.000000 efel-4.2.5/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 12:10:02.000000 efel-4.2.5/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-04 12:10:02.000000 efel-4.2.5/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 12:10:02.000000 efel-4.2.5/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-04 12:10:02.703784 efel-4.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-05-04 12:10:00.000000 efel-4.2.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-05-04 12:10:00.000000 efel-4.2.5/versioneer.py
```

### Comparing `efel-4.2/COPYING` & `efel-4.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `efel-4.2/COPYING.less` & `efel-4.2.5/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-4.2/LICENSE.txt` & `efel-4.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-4.2/PKG-INFO` & `efel-4.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.2
+Version: 4.2.5
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.2/README.md` & `efel-4.2.5/README.md`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/DependencyV5.txt` & `efel-4.2.5/efel/DependencyV5.txt`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/__init__.py` & `efel-4.2.5/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/api.py` & `efel-4.2.5/efel/api.py`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/DependencyTree.cpp` & `efel-4.2.5/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/DependencyTree.h` & `efel-4.2.5/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/FillFptrTable.cpp` & `efel-4.2.5/efel/cppcore/FillFptrTable.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/FillFptrTable.h` & `efel-4.2.5/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/Global.h` & `efel-4.2.5/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV1.cpp` & `efel-4.2.5/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV1.h` & `efel-4.2.5/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV2.cpp` & `efel-4.2.5/efel/cppcore/LibV2.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV2.h` & `efel-4.2.5/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV3.cpp` & `efel-4.2.5/efel/cppcore/LibV3.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV3.h` & `efel-4.2.5/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV4.cpp` & `efel-4.2.5/efel/cppcore/LibV4.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV4.h` & `efel-4.2.5/efel/cppcore/LibV4.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV5.cpp` & `efel-4.2.5/efel/cppcore/LibV5.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/LibV5.h` & `efel-4.2.5/efel/cppcore/LibV5.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/Utils.cpp` & `efel-4.2.5/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/Utils.h` & `efel-4.2.5/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/cfeature.cpp` & `efel-4.2.5/efel/cppcore/cfeature.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/cfeature.h` & `efel-4.2.5/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/cppcore.cpp` & `efel-4.2.5/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/eFELLogger.h` & `efel-4.2.5/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/efel.cpp` & `efel-4.2.5/efel/cppcore/efel.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/efel.h` & `efel-4.2.5/efel/cppcore/efel.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/mapoperations.cpp` & `efel-4.2.5/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/mapoperations.h` & `efel-4.2.5/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/cppcore/types.h` & `efel-4.2.5/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/io.py` & `efel-4.2.5/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/pyfeatures/__init__.py` & `efel-4.2.5/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/pyfeatures/pyfeatures.py` & `efel-4.2.5/efel/pyfeatures/pyfeatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
             up_indexes < stim_end_idx) & (up_indexes > down_indexes[0])]
         if len(up_indexes) < len(down_indexes):
             up_indexes = numpy.append(up_indexes, [stim_end_idx])
         max_hyperpol_duration = numpy.max(
             [time[up_indexes[k]] - time[down_idx] for k,
              down_idx in enumerate(down_indexes)])
 
-        # if it stays in hyperpolarzed stage for more than min_duration,
+        # if it stays in hyperpolarized stage for more than min_duration,
         # flag as depolarization block
         if max_hyperpol_duration > block_min_duration:
             return None
 
     return numpy.array([1])
```

### Comparing `efel-4.2/efel/settings.py` & `efel-4.2.5/efel/settings.py`

 * *Files identical despite different names*

### Comparing `efel-4.2/efel/units/units.json` & `efel-4.2.5/efel/units/units.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9655172413793104%*

 * *Differences: {"'depol_block_bool'": "'constant'",*

 * * "'initburst_sahp'": "'mV'",*

 * * "'initburst_sahp_ssse'": "'mV'",*

 * * "'initburst_sahp_vb'": "'mV'",*

 * * "'min_AHP_values'": "'mV'"}*

```diff
@@ -74,20 +74,24 @@
     "amp_drop_first_second": "mV",
     "amp_drop_second_last": "mV",
     "burst_mean_freq": "Hz",
     "burst_number": "constant",
     "check_AISInitiation": "constant",
     "current_base": "nA",
     "decay_time_constant_after_stim": "ms",
+    "depol_block_bool": "constant",
     "depolarized_base": "mV",
     "diff_max_duringstim": "mV",
     "diff_min_duringstim": "mV",
     "doublet_ISI": "ms",
     "fast_AHP": "mV",
     "fast_AHP_change": "constant",
+    "initburst_sahp": "mV",
+    "initburst_sahp_ssse": "mV",
+    "initburst_sahp_vb": "mV",
     "interburst_min_values": "mV",
     "interburst_voltage": "mV",
     "inv_fifth_ISI": "Hz",
     "inv_first_ISI": "Hz",
     "inv_fourth_ISI": "Hz",
     "inv_last_ISI": "Hz",
     "inv_second_ISI": "Hz",
@@ -96,14 +100,15 @@
     "irregularity_index": "ms",
     "max_amp_difference": "mV",
     "max_duringstim_from_voltage_base": "mV",
     "maximum_voltage": "mV",
     "maximum_voltage_from_voltagebase": "mV",
     "mean_AP_amplitude": "mV",
     "mean_frequency": "Hz",
+    "min_AHP_values": "mV",
     "min_between_peaks_values": "mV",
     "min_duringstim_from_voltage_base": "mV",
     "min_voltage_between_spikes": "mV",
     "minimum_voltage": "mV",
     "multiple_decay_time_constant_after_stim": "ms",
     "number_initial_spikes": "constant",
     "ohmic_input_resistance": "M\u03a9",
```

### Comparing `efel-4.2/efel.egg-info/PKG-INFO` & `efel-4.2.5/efel.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.2
+Version: 4.2.5
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.2/efel.egg-info/SOURCES.txt` & `efel-4.2.5/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-4.2/setup.py` & `efel-4.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `efel-4.2/versioneer.py` & `efel-4.2.5/versioneer.py`

 * *Files identical despite different names*

