# Comparing `tmp/nsloader-0.9.0.tar.gz` & `tmp/nsloader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsloader-0.9.0.tar", last modified: Wed May  3 15:14:53 2023, max compression
+gzip compressed data, was "nsloader-1.0.0.tar", last modified: Wed May  3 23:24:55 2023, max compression
```

## Comparing `nsloader-0.9.0.tar` & `nsloader-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:14:53.615351 nsloader-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 15:14:32.000000 nsloader-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-03 15:14:53.615351 nsloader-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-03 15:14:32.000000 nsloader-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:14:53.611351 nsloader-0.9.0/nsloader/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 15:14:32.000000 nsloader-0.9.0/nsloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-03 15:14:32.000000 nsloader-0.9.0/nsloader/wsj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:14:53.611351 nsloader-0.9.0/nsloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-03 15:14:53.000000 nsloader-0.9.0/nsloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 15:14:53.000000 nsloader-0.9.0/nsloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:14:53.000000 nsloader-0.9.0/nsloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 15:14:53.000000 nsloader-0.9.0/nsloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 15:14:53.000000 nsloader-0.9.0/nsloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:14:53.615351 nsloader-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-03 15:14:32.000000 nsloader-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:14:53.611351 nsloader-0.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:14:32.000000 nsloader-0.9.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-03 15:14:32.000000 nsloader-0.9.0/test/test_wsj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:55.612482 nsloader-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 23:24:37.000000 nsloader-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-03 23:24:55.612482 nsloader-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-03 23:24:37.000000 nsloader-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:55.612482 nsloader-1.0.0/nsloader/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 23:24:37.000000 nsloader-1.0.0/nsloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-03 23:24:37.000000 nsloader-1.0.0/nsloader/wsj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:55.612482 nsloader-1.0.0/nsloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 23:24:55.000000 nsloader-1.0.0/nsloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 23:24:55.612482 nsloader-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-03 23:24:37.000000 nsloader-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:55.612482 nsloader-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:24:37.000000 nsloader-1.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-03 23:24:37.000000 nsloader-1.0.0/test/test_wsj.py
```

### Comparing `nsloader-0.9.0/LICENSE` & `nsloader-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nsloader-0.9.0/PKG-INFO` & `nsloader-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nsloader
-Version: 0.9.0
+Version: 1.0.0
 Summary: This script collects articles from Wall Street Journal and returns it in dict format.
 Home-page: https://github.com/new-village/nsloader
 Author: new-village
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nsloader  
-[![Test](https://github.com/new-village/nsloader/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/new-village/nsloader/actions/workflows/unittest.yaml)[![PyPI](https://badge.fury.io/py/nsloader.svg)](https://badge.fury.io/py/nsloader)  
+[![Test](https://github.com/new-village/nsloader/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/new-village/nsloader/actions/workflows/unittest.yaml) [![PyPI version](https://badge.fury.io/py/nsloader.svg)](https://badge.fury.io/py/nsloader)  
 This script collects articles from [Wall Street Journal](https://www.wsj.com/) and returns it in dict format.  
   
 ### Installing nsloader and Supported Versions
 ----------------------
 nsloader is not registered on the pypi. You have to download from github directly.
 ```
 $ python -m pip install nsloader
```

### Comparing `nsloader-0.9.0/README.md` & `nsloader-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # nsloader  
-[![Test](https://github.com/new-village/nsloader/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/new-village/nsloader/actions/workflows/unittest.yaml)[![PyPI](https://badge.fury.io/py/nsloader.svg)](https://badge.fury.io/py/nsloader)  
+[![Test](https://github.com/new-village/nsloader/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/new-village/nsloader/actions/workflows/unittest.yaml) [![PyPI version](https://badge.fury.io/py/nsloader.svg)](https://badge.fury.io/py/nsloader)  
 This script collects articles from [Wall Street Journal](https://www.wsj.com/) and returns it in dict format.  
   
 ### Installing nsloader and Supported Versions
 ----------------------
 nsloader is not registered on the pypi. You have to download from github directly.
 ```
 $ python -m pip install nsloader
```

### Comparing `nsloader-0.9.0/nsloader/wsj.py` & `nsloader-1.0.0/nsloader/wsj.py`

 * *Files identical despite different names*

### Comparing `nsloader-0.9.0/nsloader.egg-info/PKG-INFO` & `nsloader-1.0.0/nsloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nsloader
-Version: 0.9.0
+Version: 1.0.0
 Summary: This script collects articles from Wall Street Journal and returns it in dict format.
 Home-page: https://github.com/new-village/nsloader
 Author: new-village
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nsloader  
-[![Test](https://github.com/new-village/nsloader/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/new-village/nsloader/actions/workflows/unittest.yaml)[![PyPI](https://badge.fury.io/py/nsloader.svg)](https://badge.fury.io/py/nsloader)  
+[![Test](https://github.com/new-village/nsloader/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/new-village/nsloader/actions/workflows/unittest.yaml) [![PyPI version](https://badge.fury.io/py/nsloader.svg)](https://badge.fury.io/py/nsloader)  
 This script collects articles from [Wall Street Journal](https://www.wsj.com/) and returns it in dict format.  
   
 ### Installing nsloader and Supported Versions
 ----------------------
 nsloader is not registered on the pypi. You have to download from github directly.
 ```
 $ python -m pip install nsloader
```

### Comparing `nsloader-0.9.0/setup.py` & `nsloader-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='nsloader',
-    version='0.9.0',
+    version='1.0.0',
     author='new-village',
     url='https://github.com/new-village/nsloader',
     description='This script collects articles from Wall Street Journal and returns it in dict format.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['beautifulsoup4', 'selenium', 'webdriver_manager', 'chromedriver_binary'],
     packages=find_packages(),
```

### Comparing `nsloader-0.9.0/test/test_wsj.py` & `nsloader-1.0.0/test/test_wsj.py`

 * *Files identical despite different names*

