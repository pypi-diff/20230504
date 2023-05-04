# Comparing `tmp/myNeuropsydia-0.1.1.tar.gz` & `tmp/myNeuropsydia-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\myNeuropsydia-0.1.1.tar", last modified: Thu May  4 08:12:44 2023, max compression
+gzip compressed data, was "dist\myNeuropsydia-0.1.2.tar", last modified: Thu May  4 16:57:38 2023, max compression
```

## Comparing `myNeuropsydia-0.1.1.tar` & `myNeuropsydia-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 08:12:44.077046 myNeuropsydia-0.1.1/
--rw-rw-rw-   0        0        0      229 2023-05-04 08:12:44.076041 myNeuropsydia-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-05-04 08:12:17.000000 myNeuropsydia-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 08:12:44.074040 myNeuropsydia-0.1.1/myNeuropsydia.egg-info/
--rw-rw-rw-   0        0        0      229 2023-05-04 08:12:43.000000 myNeuropsydia-0.1.1/myNeuropsydia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-05-04 08:12:43.000000 myNeuropsydia-0.1.1/myNeuropsydia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       62 2023-05-04 08:12:43.000000 myNeuropsydia-0.1.1/myNeuropsydia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-04 08:12:43.000000 myNeuropsydia-0.1.1/myNeuropsydia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 08:12:43.000000 myNeuropsydia-0.1.1/myNeuropsydia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 08:12:44.077046 myNeuropsydia-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-04 08:10:53.000000 myNeuropsydia-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:57:38.410536 myNeuropsydia-0.1.2/
+-rw-rw-rw-   0        0        0      229 2023-05-04 16:57:38.409522 myNeuropsydia-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-05-04 08:12:17.000000 myNeuropsydia-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 16:57:38.406514 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-05-04 16:57:37.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-05-04 16:57:38.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       62 2023-05-04 16:57:37.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-04 16:57:37.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:57:37.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:57:38.410536 myNeuropsydia-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-05-04 16:56:38.000000 myNeuropsydia-0.1.2/setup.py
```

### Comparing `myNeuropsydia-0.1.1/setup.py` & `myNeuropsydia-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import find_packages, setup
 
 setup(
     name='myNeuropsydia',
     packages=find_packages(),
-    version='0.1.1',
+    version='0.1.2',
     description='Partially fixed version of Neuropsydia library, a Python module for creating experiments, tasks and questionnaires',
     author='Laborde',
     license='ENS_Paris_Saclay',
     package_data = {
                 	"myNeuropsydia.files.font":["*.ttf", "*.otf"],
                 	"myNeuropsydia.files.binary":["*.png"],
                 	"myNeuropsydia.files.logo":["*.png"]},
```

