# Comparing `tmp/selfdiffusion-0.1.6.tar.gz` & `tmp/selfdiffusion-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfdiffusion-0.1.6.tar", max compression
+gzip compressed data, was "selfdiffusion-0.1.7.tar", max compression
```

## Comparing `selfdiffusion-0.1.6.tar` & `selfdiffusion-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-05-04 17:57:32.385329 selfdiffusion-0.1.6/LICENSE
--rw-r--r--   0        0        0     2658 2023-05-04 17:57:32.385329 selfdiffusion-0.1.6/README.md
--rw-r--r--   0        0        0      723 2023-05-04 17:57:32.385329 selfdiffusion-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       55 2023-05-04 17:57:32.385329 selfdiffusion-0.1.6/selfdiffusion/__init__.py
--rw-r--r--   0        0        0     2204 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/cli.py
--rw-r--r--   0        0        0      717 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/log.py
--rw-r--r--   0        0        0      747 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/sources/__init__.py
--rw-r--r--   0        0        0     4368 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/sources/bing.py
--rw-r--r--   0        0        0        0 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/transforms/__init__.py
--rw-r--r--   0        0        0      379 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/transforms/exceptions.py
--rw-r--r--   0        0        0     1745 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/transforms/ml.py
--rw-r--r--   0        0        0     2666 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/transforms/transforms.py
--rw-r--r--   0        0        0     1738 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/transforms/utils.py
--rw-r--r--   0        0        0     1458 2023-05-04 17:57:32.389329 selfdiffusion-0.1.6/selfdiffusion/utils.py
--rw-r--r--   0        0        0     3505 1970-01-01 00:00:00.000000 selfdiffusion-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2702 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/README.md
+-rw-r--r--   0        0        0      723 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/__init__.py
+-rw-r--r--   0        0        0     2204 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/cli.py
+-rw-r--r--   0        0        0      717 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/log.py
+-rw-r--r--   0        0        0      747 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/sources/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/sources/bing.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/transforms/__init__.py
+-rw-r--r--   0        0        0      379 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/transforms/exceptions.py
+-rw-r--r--   0        0        0     1745 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/transforms/ml.py
+-rw-r--r--   0        0        0     2666 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/transforms/transforms.py
+-rw-r--r--   0        0        0     1738 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/transforms/utils.py
+-rw-r--r--   0        0        0     1458 2023-05-04 18:13:59.026078 selfdiffusion-0.1.7/selfdiffusion/utils.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 selfdiffusion-0.1.7/PKG-INFO
```

### Comparing `selfdiffusion-0.1.6/LICENSE` & `selfdiffusion-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `selfdiffusion-0.1.6/README.md` & `selfdiffusion-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center" text-align="center">
-  <img src="https://github.com/La-Compagnie-Infonuagique/selfdiffusion/blob/master/assets/selfdiffusion.jpg" alt="self diffusion">
+  <img src="https://raw.githubusercontent.com/La-Compagnie-Infonuagique/selfdiffusion/aca5dc131f3162c2a0817a38a7d95b836a7faefc/assets/selfdiffusion.jpg" alt="self diffusion">
 </p>
 
 <div align="center">
   <h1>selfdiffusion</h1>
 </div>
 
 <p align="center">
```

### Comparing `selfdiffusion-0.1.6/pyproject.toml` & `selfdiffusion-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selfdiffusion"
-version = "0.1.6"
+version = "0.1.7"
 description = "Easily create datasets for diffusion models personalization"
 authors = ["Jonathan Pelletier <jonathan.pelletier-aafz@thecloudco.ca>"]
 repository = "https://github.com/La-Compagnie-Infonuagique/selfdiffusion"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `selfdiffusion-0.1.6/selfdiffusion/cli.py` & `selfdiffusion-0.1.7/selfdiffusion/cli.py`

 * *Files identical despite different names*

### Comparing `selfdiffusion-0.1.6/selfdiffusion/log.py` & `selfdiffusion-0.1.7/selfdiffusion/log.py`

 * *Files identical despite different names*

### Comparing `selfdiffusion-0.1.6/selfdiffusion/pipelines/__init__.py` & `selfdiffusion-0.1.7/selfdiffusion/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `selfdiffusion-0.1.6/selfdiffusion/sources/bing.py` & `selfdiffusion-0.1.7/selfdiffusion/sources/bing.py`

 * *Files identical despite different names*

### Comparing `selfdiffusion-0.1.6/selfdiffusion/transforms/ml.py` & `selfdiffusion-0.1.7/selfdiffusion/transforms/ml.py`

 * *Files identical despite different names*

### Comparing `selfdiffusion-0.1.6/selfdiffusion/transforms/transforms.py` & `selfdiffusion-0.1.7/selfdiffusion/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `selfdiffusion-0.1.6/selfdiffusion/transforms/utils.py` & `selfdiffusion-0.1.7/selfdiffusion/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `selfdiffusion-0.1.6/selfdiffusion/utils.py` & `selfdiffusion-0.1.7/selfdiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `selfdiffusion-0.1.6/PKG-INFO` & `selfdiffusion-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfdiffusion
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easily create datasets for diffusion models personalization
 Home-page: https://github.com/La-Compagnie-Infonuagique/selfdiffusion
 Author: Jonathan Pelletier
 Author-email: jonathan.pelletier-aafz@thecloudco.ca
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: ultralytics (>=8.0.66,<9.0.0)
 Project-URL: Repository, https://github.com/La-Compagnie-Infonuagique/selfdiffusion
 Description-Content-Type: text/markdown
 
 <p align="center" text-align="center">
-  <img src="https://github.com/La-Compagnie-Infonuagique/selfdiffusion/blob/master/assets/selfdiffusion.jpg" alt="self diffusion">
+  <img src="https://raw.githubusercontent.com/La-Compagnie-Infonuagique/selfdiffusion/aca5dc131f3162c2a0817a38a7d95b836a7faefc/assets/selfdiffusion.jpg" alt="self diffusion">
 </p>
 
 <div align="center">
   <h1>selfdiffusion</h1>
 </div>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: selfdiffusion Version: 0.1.6 Summary: Easily create
+Metadata-Version: 2.1 Name: selfdiffusion Version: 0.1.7 Summary: Easily create
 datasets for diffusion models personalization Home-page: https://github.com/La-
 Compagnie-Infonuagique/selfdiffusion Author: Jonathan Pelletier Author-email:
 jonathan.pelletier-aafz@thecloudco.ca Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.0.1,<9.0.0) Requires-Dist: exceptiongroup ; python_version < "3.11"
 Requires-Dist: face-recognition (>=1.3.0,<2.0.0) Requires-Dist: halo
```

