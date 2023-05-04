# Comparing `tmp/myNeuropsydia-0.1.2.tar.gz` & `tmp/myNeuropsydia-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\myNeuropsydia-0.1.2.tar", last modified: Thu May  4 16:57:38 2023, max compression
+gzip compressed data, was "dist\myNeuropsydia-0.1.3.tar", last modified: Thu May  4 17:07:45 2023, max compression
```

## Comparing `myNeuropsydia-0.1.2.tar` & `myNeuropsydia-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:57:38.410536 myNeuropsydia-0.1.2/
--rw-rw-rw-   0        0        0      229 2023-05-04 16:57:38.409522 myNeuropsydia-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-05-04 08:12:17.000000 myNeuropsydia-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 16:57:38.406514 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/
--rw-rw-rw-   0        0        0      229 2023-05-04 16:57:37.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-05-04 16:57:38.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       62 2023-05-04 16:57:37.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-04 16:57:37.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:57:37.000000 myNeuropsydia-0.1.2/myNeuropsydia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 16:57:38.410536 myNeuropsydia-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-04 16:56:38.000000 myNeuropsydia-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:07:45.836947 myNeuropsydia-0.1.3/
+-rw-rw-rw-   0        0        0      229 2023-05-04 17:07:45.835949 myNeuropsydia-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-05-04 08:12:17.000000 myNeuropsydia-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 17:07:45.833949 myNeuropsydia-0.1.3/myNeuropsydia.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-05-04 17:07:45.000000 myNeuropsydia-0.1.3/myNeuropsydia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-05-04 17:07:45.000000 myNeuropsydia-0.1.3/myNeuropsydia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       62 2023-05-04 17:07:45.000000 myNeuropsydia-0.1.3/myNeuropsydia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-04 17:07:45.000000 myNeuropsydia-0.1.3/myNeuropsydia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:07:45.000000 myNeuropsydia-0.1.3/myNeuropsydia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:07:45.836947 myNeuropsydia-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-05-04 17:07:37.000000 myNeuropsydia-0.1.3/setup.py
```

### Comparing `myNeuropsydia-0.1.2/setup.py` & `myNeuropsydia-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import find_packages, setup
 
 setup(
     name='myNeuropsydia',
     packages=find_packages(),
-    version='0.1.2',
+    version='0.1.3',
     description='Partially fixed version of Neuropsydia library, a Python module for creating experiments, tasks and questionnaires',
     author='Laborde',
     license='ENS_Paris_Saclay',
     package_data = {
                 	"myNeuropsydia.files.font":["*.ttf", "*.otf"],
                 	"myNeuropsydia.files.binary":["*.png"],
                 	"myNeuropsydia.files.logo":["*.png"]},
```

