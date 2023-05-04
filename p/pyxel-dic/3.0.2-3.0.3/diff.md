# Comparing `tmp/pyxel-dic-3.0.2.tar.gz` & `tmp/pyxel-dic-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxel-dic-3.0.2.tar", last modified: Mon Apr 17 15:15:22 2023, max compression
+gzip compressed data, was "pyxel-dic-3.0.3.tar", last modified: Thu May  4 10:15:22 2023, max compression
```

## Comparing `pyxel-dic-3.0.2.tar` & `pyxel-dic-3.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:22.737573 pyxel-dic-3.0.2/
--rw-rw-rw-   0        0        0     4930 2023-04-17 15:15:22.737573 pyxel-dic-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4250 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/README.md
--rw-rw-rw-   0        0        0      745 2023-04-17 15:14:03.000000 pyxel-dic-3.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      898 2023-04-17 15:15:22.743204 pyxel-dic-3.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:22.535867 pyxel-dic-3.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:22.695455 pyxel-dic-3.0.2/src/pyxel/
--rw-rw-rw-   0        0        0      332 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/__init__.py
--rw-rw-rw-   0        0        0    31183 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/camera.py
--rw-rw-rw-   0        0        0    24473 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/dic.py
--rw-rw-rw-   0        0        0     2317 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/exportpixmap.py
--rw-rw-rw-   0        0        0    13368 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/image.py
--rw-rw-rw-   0        0        0     9658 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/levelset.py
--rw-rw-rw-   0        0        0     3293 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/material.py
--rw-rw-rw-   0        0        0   124883 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/mesh.py
--rw-rw-rw-   0        0        0    17624 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/mesher.py
--rw-rw-rw-   0        0        0     6859 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/meshparser.py
--rw-rw-rw-   0        0        0     3245 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/utils.py
--rw-rw-rw-   0        0        0    16353 2023-04-17 15:11:38.000000 pyxel-dic-3.0.2/src/pyxel/vtktools.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:15:22.730933 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/
--rw-rw-rw-   0        0        0     4930 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 15:15:22.000000 pyxel-dic-3.0.2/src/pyxel_dic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 10:15:22.230199 pyxel-dic-3.0.3/
+-rw-rw-rw-   0        0        0     4930 2023-05-04 10:15:22.230199 pyxel-dic-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4250 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/README.md
+-rw-rw-rw-   0        0        0      745 2023-05-04 10:13:26.000000 pyxel-dic-3.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      898 2023-05-04 10:15:22.239755 pyxel-dic-3.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 10:15:21.883766 pyxel-dic-3.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 10:15:22.160737 pyxel-dic-3.0.3/src/pyxel/
+-rw-rw-rw-   0        0        0      332 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/__init__.py
+-rw-rw-rw-   0        0        0    31183 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/camera.py
+-rw-rw-rw-   0        0        0    24473 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/dic.py
+-rw-rw-rw-   0        0        0     2317 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/exportpixmap.py
+-rw-rw-rw-   0        0        0    13368 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/image.py
+-rw-rw-rw-   0        0        0     9658 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/levelset.py
+-rw-rw-rw-   0        0        0     3293 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/material.py
+-rw-rw-rw-   0        0        0   124883 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/mesh.py
+-rw-rw-rw-   0        0        0    17624 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/mesher.py
+-rw-rw-rw-   0        0        0     6859 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/meshparser.py
+-rw-rw-rw-   0        0        0     3245 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/utils.py
+-rw-rw-rw-   0        0        0    16353 2023-04-17 15:11:38.000000 pyxel-dic-3.0.3/src/pyxel/vtktools.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:15:22.222148 pyxel-dic-3.0.3/src/pyxel_dic.egg-info/
+-rw-rw-rw-   0        0        0     4930 2023-05-04 10:15:21.000000 pyxel-dic-3.0.3/src/pyxel_dic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-05-04 10:15:21.000000 pyxel-dic-3.0.3/src/pyxel_dic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:15:21.000000 pyxel-dic-3.0.3/src/pyxel_dic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-04 10:15:21.000000 pyxel-dic-3.0.3/src/pyxel_dic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-04 10:15:21.000000 pyxel-dic-3.0.3/src/pyxel_dic.egg-info/top_level.txt
```

### Comparing `pyxel-dic-3.0.2/PKG-INFO` & `pyxel-dic-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.0.2
+Version: 3.0.3
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: CeCILL
 Project-URL: Homepage, https://github.com/jcpassieux/pyxel
 Project-URL: Bug Tracker, https://github.com/jcpassieux/pyxel/issues
```

### Comparing `pyxel-dic-3.0.2/README.md` & `pyxel-dic-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/pyproject.toml` & `pyxel-dic-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyxel-dic"
-version = "3.0.2"
+version = "3.0.3"
 authors = [
   { name="JC Passieux", email="jc.passieux@gmail.com" },
 ]
 description = "Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyxel-dic-3.0.2/setup.cfg` & `pyxel-dic-3.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/camera.py` & `pyxel-dic-3.0.3/src/pyxel/camera.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/dic.py` & `pyxel-dic-3.0.3/src/pyxel/dic.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/exportpixmap.py` & `pyxel-dic-3.0.3/src/pyxel/exportpixmap.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/image.py` & `pyxel-dic-3.0.3/src/pyxel/image.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/levelset.py` & `pyxel-dic-3.0.3/src/pyxel/levelset.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/material.py` & `pyxel-dic-3.0.3/src/pyxel/material.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/mesh.py` & `pyxel-dic-3.0.3/src/pyxel/mesh.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/mesher.py` & `pyxel-dic-3.0.3/src/pyxel/mesher.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/meshparser.py` & `pyxel-dic-3.0.3/src/pyxel/meshparser.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/utils.py` & `pyxel-dic-3.0.3/src/pyxel/utils.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel/vtktools.py` & `pyxel-dic-3.0.3/src/pyxel/vtktools.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.0.2/src/pyxel_dic.egg-info/PKG-INFO` & `pyxel-dic-3.0.3/src/pyxel_dic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.0.2
+Version: 3.0.3
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: CeCILL
 Project-URL: Homepage, https://github.com/jcpassieux/pyxel
 Project-URL: Bug Tracker, https://github.com/jcpassieux/pyxel/issues
```

