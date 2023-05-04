# Comparing `tmp/pvbm-1.7.0.tar.gz` & `tmp/pvbm-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-1.7.0.tar", last modified: Thu May  4 16:41:13 2023, max compression
+gzip compressed data, was "pvbm-1.8.0.tar", last modified: Thu May  4 16:47:14 2023, max compression
```

## Comparing `pvbm-1.7.0.tar` & `pvbm-1.8.0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:41:13.030750 pvbm-1.7.0/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1269 2023-05-04 16:41:13.030574 pvbm-1.7.0/PKG-INFO
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:41:13.029501 pvbm-1.7.0/PVBM/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)    10404 2023-04-13 10:09:55.000000 pvbm-1.7.0/PVBM/FractalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     5257 2023-04-30 12:10:25.000000 pvbm-1.7.0/PVBM/GeometricalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-1.7.0/PVBM/__init__.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1007 2023-04-30 13:59:40.000000 pvbm-1.7.0/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:41:13.030381 pvbm-1.7.0/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1269 2023-05-04 16:41:12.000000 pvbm-1.7.0/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      226 2023-05-04 16:41:13.000000 pvbm-1.7.0/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:41:12.000000 pvbm-1.7.0/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-04 16:41:12.000000 pvbm-1.7.0/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-04 16:41:12.000000 pvbm-1.7.0/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-04 16:41:13.030798 pvbm-1.7.0/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-04 16:40:35.000000 pvbm-1.7.0/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:47:14.058326 pvbm-1.8.0/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1269 2023-05-04 16:47:14.058161 pvbm-1.8.0/PKG-INFO
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:47:14.055688 pvbm-1.8.0/PVBM/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)    10404 2023-04-13 10:09:55.000000 pvbm-1.8.0/PVBM/FractalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     5257 2023-04-30 12:10:25.000000 pvbm-1.8.0/PVBM/GeometricalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-1.8.0/PVBM/__init__.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:47:14.056993 pvbm-1.8.0/PVBM/helpers/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-1.8.0/PVBM/helpers/__init__.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-1.8.0/PVBM/helpers/branching2.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     8674 2023-04-30 12:24:25.000000 pvbm-1.8.0/PVBM/helpers/branching_angle.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-1.8.0/PVBM/helpers/tortuosity.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1007 2023-04-30 13:59:40.000000 pvbm-1.8.0/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-04 16:47:14.057934 pvbm-1.8.0/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1269 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      337 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-04 16:47:14.000000 pvbm-1.8.0/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-04 16:47:14.058365 pvbm-1.8.0/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-04 16:47:00.000000 pvbm-1.8.0/setup.py
```

### Comparing `pvbm-1.7.0/PKG-INFO` & `pvbm-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-1.7.0/PVBM/FractalAnalysis.py` & `pvbm-1.8.0/PVBM/FractalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-1.7.0/PVBM/GeometricalAnalysis.py` & `pvbm-1.8.0/PVBM/GeometricalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-1.7.0/README.md` & `pvbm-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pvbm-1.7.0/pvbm.egg-info/PKG-INFO` & `pvbm-1.8.0/pvbm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-1.7.0/setup.py` & `pvbm-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='1.7.0',
+    version='1.8.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```

