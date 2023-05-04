# Comparing `tmp/enrRiceTrait-1.4.0.tar.gz` & `tmp/enrRiceTrait-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enrRiceTrait-1.4.0.tar", last modified: Tue Apr 25 09:29:01 2023, max compression
+gzip compressed data, was "enrRiceTrait-1.4.2.tar", last modified: Thu May  4 14:51:06 2023, max compression
```

## Comparing `enrRiceTrait-1.4.0.tar` & `enrRiceTrait-1.4.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-25 09:29:01.984574 enrRiceTrait-1.4.0/
--rw-rw-r--   0 yao        (501) staff       (20)       53 2021-03-29 13:55:50.000000 enrRiceTrait-1.4.0/MANIFEST.in
--rw-r--r--   0 yao        (501) staff       (20)      599 2023-04-25 09:29:01.984320 enrRiceTrait-1.4.0/PKG-INFO
--rw-rw-r--   0 yao        (501) staff       (20)       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.4.0/README.md
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-25 09:29:01.944459 enrRiceTrait-1.4.0/enrRiceTrait/
--rw-r--r--   0 yao        (501) staff       (20)    24660 2023-04-25 08:51:28.000000 enrRiceTrait-1.4.0/enrRiceTrait/Enrichment.py
--rw-rw-r--   0 yao        (501) staff       (20)      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.4.0/enrRiceTrait/PTE_config.py
--rw-rw-r--   0 yao        (501) staff       (20)      222 2023-04-25 09:28:54.000000 enrRiceTrait-1.4.0/enrRiceTrait/__init__.py
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-25 09:29:01.967695 enrRiceTrait-1.4.0/enrRiceTrait/data/
--rw-rw-r--   0 yao        (501) staff       (20)  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.4.0/enrRiceTrait/data/Total_Association.txt
--rw-rw-r--   0 yao        (501) staff       (20)  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.4.0/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
-drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-04-25 09:29:01.945187 enrRiceTrait-1.4.0/enrRiceTrait.egg-info/
--rw-rw-r--   0 yao        (501) staff       (20)      599 2023-04-25 09:29:01.000000 enrRiceTrait-1.4.0/enrRiceTrait.egg-info/PKG-INFO
--rw-rw-r--   0 yao        (501) staff       (20)      337 2023-04-25 09:29:01.000000 enrRiceTrait-1.4.0/enrRiceTrait.egg-info/SOURCES.txt
--rw-rw-r--   0 yao        (501) staff       (20)        1 2023-04-25 09:29:01.000000 enrRiceTrait-1.4.0/enrRiceTrait.egg-info/dependency_links.txt
--rw-rw-r--   0 yao        (501) staff       (20)       13 2023-04-25 09:29:01.000000 enrRiceTrait-1.4.0/enrRiceTrait.egg-info/top_level.txt
--rw-r--r--   0 yao        (501) staff       (20)       38 2023-04-25 09:29:01.984645 enrRiceTrait-1.4.0/setup.cfg
--rw-rw-r--   0 yao        (501) staff       (20)     1085 2023-04-25 09:28:54.000000 enrRiceTrait-1.4.0/setup.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-04 14:51:06.251065 enrRiceTrait-1.4.2/
+-rw-rw-r--   0 yao        (501) staff       (20)       53 2021-03-29 13:55:50.000000 enrRiceTrait-1.4.2/MANIFEST.in
+-rw-r--r--   0 yao        (501) staff       (20)      599 2023-05-04 14:51:06.250734 enrRiceTrait-1.4.2/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)       92 2020-07-13 13:31:42.000000 enrRiceTrait-1.4.2/README.md
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-04 14:51:06.221454 enrRiceTrait-1.4.2/enrRiceTrait/
+-rw-r--r--   0 yao        (501) staff       (20)    24661 2023-05-01 16:31:03.000000 enrRiceTrait-1.4.2/enrRiceTrait/Enrichment.py
+-rw-rw-r--   0 yao        (501) staff       (20)      478 2021-03-29 14:59:32.000000 enrRiceTrait-1.4.2/enrRiceTrait/PTE_config.py
+-rw-rw-r--   0 yao        (501) staff       (20)      222 2023-05-01 16:29:51.000000 enrRiceTrait-1.4.2/enrRiceTrait/__init__.py
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-04 14:51:06.244154 enrRiceTrait-1.4.2/enrRiceTrait/data/
+-rw-rw-r--   0 yao        (501) staff       (20)  9834834 2021-03-27 15:22:16.000000 enrRiceTrait-1.4.2/enrRiceTrait/data/Total_Association.txt
+-rw-r--r--   0 yao        (501) staff       (20)  1074775 2023-04-25 14:00:56.000000 enrRiceTrait-1.4.2/enrRiceTrait/data/to.wto.ro.funRiceGene.obo
+-rw-rw-r--   0 yao        (501) staff       (20)  1090456 2021-03-25 12:59:06.000000 enrRiceTrait-1.4.2/enrRiceTrait/data/to.wto.ro.funRiceGene.wheat(do not change to rice).obo
+drwxr-xr-x   0 yao        (501) staff       (20)        0 2023-05-04 14:51:06.222581 enrRiceTrait-1.4.2/enrRiceTrait.egg-info/
+-rw-rw-r--   0 yao        (501) staff       (20)      599 2023-05-04 14:51:06.000000 enrRiceTrait-1.4.2/enrRiceTrait.egg-info/PKG-INFO
+-rw-rw-r--   0 yao        (501) staff       (20)      410 2023-05-04 14:51:06.000000 enrRiceTrait-1.4.2/enrRiceTrait.egg-info/SOURCES.txt
+-rw-rw-r--   0 yao        (501) staff       (20)        1 2023-05-04 14:51:06.000000 enrRiceTrait-1.4.2/enrRiceTrait.egg-info/dependency_links.txt
+-rw-rw-r--   0 yao        (501) staff       (20)       13 2023-05-04 14:51:06.000000 enrRiceTrait-1.4.2/enrRiceTrait.egg-info/top_level.txt
+-rw-r--r--   0 yao        (501) staff       (20)       38 2023-05-04 14:51:06.251156 enrRiceTrait-1.4.2/setup.cfg
+-rw-rw-r--   0 yao        (501) staff       (20)     1085 2023-05-01 16:29:51.000000 enrRiceTrait-1.4.2/setup.py
```

### Comparing `enrRiceTrait-1.4.0/PKG-INFO` & `enrRiceTrait-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrRiceTrait
-Version: 1.4.0
+Version: 1.4.2
 Summary: A python package for Rice Trait Enrichment.
 Home-page: https://github.com/YaoXinZhi/enrRiceTrait
 Author: xinzhi_yao
 Author-email: xinzhi_bioinfo@163.com
 License: UNKNOWN
 Description: # Plant Trait Enrichment Package  
         This is a python package for plant trait enrichment.
```

### Comparing `enrRiceTrait-1.4.0/enrRiceTrait/Enrichment.py` & `enrRiceTrait-1.4.2/enrRiceTrait/Enrichment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 # ! usr/bin/env python3
 """
 Created on 09/07/2020 下午4:15
 @Author: xinzhi yao
 """
 # 1. check if the package is complete.
-# python setup.py check
+# python3 setup.py check
 # 2. generate the package file.
 # python3 setup.py sdist bdist_wheel
 # only test
 # python3 -m twine upload --repository testpypi dist/*
 # upload to your pypi (obselate)
 # python3 setup.py register sdist upload -r http://pypi.org
 # 3. upload to your pypi (please delete the previously .tar.gz and .whl files.)
```

### Comparing `enrRiceTrait-1.4.0/enrRiceTrait/data/Total_Association.txt` & `enrRiceTrait-1.4.2/enrRiceTrait/data/Total_Association.txt`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.4.0/enrRiceTrait/data/to.wto.ro.funRiceGene.obo` & `enrRiceTrait-1.4.2/enrRiceTrait/data/to.wto.ro.funRiceGene.wheat(do not change to rice).obo`

 * *Files identical despite different names*

### Comparing `enrRiceTrait-1.4.0/enrRiceTrait.egg-info/PKG-INFO` & `enrRiceTrait-1.4.2/enrRiceTrait.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enrRiceTrait
-Version: 1.4.0
+Version: 1.4.2
 Summary: A python package for Rice Trait Enrichment.
 Home-page: https://github.com/YaoXinZhi/enrRiceTrait
 Author: xinzhi_yao
 Author-email: xinzhi_bioinfo@163.com
 License: UNKNOWN
 Description: # Plant Trait Enrichment Package  
         This is a python package for plant trait enrichment.
```

### Comparing `enrRiceTrait-1.4.0/setup.py` & `enrRiceTrait-1.4.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(
   name='enrRiceTrait',
-  version='1.4.0',
+  version='1.4.2',
   author='xinzhi_yao',
   author_email='xinzhi_bioinfo@163.com',
   description="A python package for Rice Trait Enrichment.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/YaoXinZhi/enrRiceTrait",
```

