# Comparing `tmp/cdk-vpc-module-0.0.7.tar.gz` & `tmp/cdk-vpc-module-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-vpc-module-0.0.7.tar", last modified: Mon Mar 27 15:20:34 2023, max compression
+gzip compressed data, was "cdk-vpc-module-0.0.8.tar", last modified: Thu May  4 11:44:21 2023, max compression
```

## Comparing `cdk-vpc-module-0.0.7.tar` & `cdk-vpc-module-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:20:34.937508 cdk-vpc-module-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-27 15:20:19.000000 cdk-vpc-module-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-27 15:20:19.000000 cdk-vpc-module-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-03-27 15:20:34.937508 cdk-vpc-module-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-03-27 15:20:19.000000 cdk-vpc-module-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-27 15:20:19.000000 cdk-vpc-module-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 15:20:34.937508 cdk-vpc-module-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-27 15:20:19.000000 cdk-vpc-module-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:20:34.937508 cdk-vpc-module-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:20:34.937508 cdk-vpc-module-0.0.7/src/cdk_vpc_module/
--rw-r--r--   0 runner    (1001) docker     (123)    33195 2023-03-27 15:20:19.000000 cdk-vpc-module-0.0.7/src/cdk_vpc_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:20:34.937508 cdk-vpc-module-0.0.7/src/cdk_vpc_module/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-27 15:20:19.000000 cdk-vpc-module-0.0.7/src/cdk_vpc_module/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30396 2023-03-27 15:20:19.000000 cdk-vpc-module-0.0.7/src/cdk_vpc_module/_jsii/cdk-vpc-module@0.0.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:20:19.000000 cdk-vpc-module-0.0.7/src/cdk_vpc_module/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:20:34.937508 cdk-vpc-module-0.0.7/src/cdk_vpc_module.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-03-27 15:20:34.000000 cdk-vpc-module-0.0.7/src/cdk_vpc_module.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-27 15:20:34.000000 cdk-vpc-module-0.0.7/src/cdk_vpc_module.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:20:34.000000 cdk-vpc-module-0.0.7/src/cdk_vpc_module.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-27 15:20:34.000000 cdk-vpc-module-0.0.7/src/cdk_vpc_module.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 15:20:34.000000 cdk-vpc-module-0.0.7/src/cdk_vpc_module.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:21.567969 cdk-vpc-module-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 11:44:05.000000 cdk-vpc-module-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 11:44:05.000000 cdk-vpc-module-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-05-04 11:44:21.567969 cdk-vpc-module-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-04 11:44:05.000000 cdk-vpc-module-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 11:44:05.000000 cdk-vpc-module-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:44:21.567969 cdk-vpc-module-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-04 11:44:05.000000 cdk-vpc-module-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:21.567969 cdk-vpc-module-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:21.567969 cdk-vpc-module-0.0.8/src/cdk_vpc_module/
+-rw-r--r--   0 runner    (1001) docker     (123)    33195 2023-05-04 11:44:05.000000 cdk-vpc-module-0.0.8/src/cdk_vpc_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:21.567969 cdk-vpc-module-0.0.8/src/cdk_vpc_module/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-04 11:44:05.000000 cdk-vpc-module-0.0.8/src/cdk_vpc_module/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30398 2023-05-04 11:44:05.000000 cdk-vpc-module-0.0.8/src/cdk_vpc_module/_jsii/cdk-vpc-module@0.0.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:44:05.000000 cdk-vpc-module-0.0.8/src/cdk_vpc_module/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:21.567969 cdk-vpc-module-0.0.8/src/cdk_vpc_module.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-05-04 11:44:20.000000 cdk-vpc-module-0.0.8/src/cdk_vpc_module.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-04 11:44:21.000000 cdk-vpc-module-0.0.8/src/cdk_vpc_module.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:44:20.000000 cdk-vpc-module-0.0.8/src/cdk_vpc_module.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 11:44:21.000000 cdk-vpc-module-0.0.8/src/cdk_vpc_module.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 11:44:21.000000 cdk-vpc-module-0.0.8/src/cdk_vpc_module.egg-info/top_level.txt
```

### Comparing `cdk-vpc-module-0.0.7/LICENSE` & `cdk-vpc-module-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-vpc-module-0.0.7/PKG-INFO` & `cdk-vpc-module-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-module
-Version: 0.0.7
+Version: 0.0.8
 Summary: @smallcase/cdk-vpc-module
 Home-page: https://github.com/smallcase/cdk-vpc-module.git
 Author: Bharat Parmar<bharat.parmar@smallcase.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/smallcase/cdk-vpc-module.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-vpc-module-0.0.7/README.md` & `cdk-vpc-module-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cdk-vpc-module-0.0.7/setup.py` & `cdk-vpc-module-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-vpc-module",
-    "version": "0.0.7",
+    "version": "0.0.8",
     "description": "@smallcase/cdk-vpc-module",
     "license": "Apache-2.0",
     "url": "https://github.com/smallcase/cdk-vpc-module.git",
     "long_description_content_type": "text/markdown",
     "author": "Bharat Parmar<bharat.parmar@smallcase.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_vpc_module",
         "cdk_vpc_module._jsii"
     ],
     "package_data": {
         "cdk_vpc_module._jsii": [
-            "cdk-vpc-module@0.0.7.jsii.tgz"
+            "cdk-vpc-module@0.0.8.jsii.tgz"
         ],
         "cdk_vpc_module": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-vpc-module-0.0.7/src/cdk_vpc_module/__init__.py` & `cdk-vpc-module-0.0.8/src/cdk_vpc_module/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-vpc-module-0.0.7/src/cdk_vpc_module.egg-info/PKG-INFO` & `cdk-vpc-module-0.0.8/src/cdk_vpc_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-module
-Version: 0.0.7
+Version: 0.0.8
 Summary: @smallcase/cdk-vpc-module
 Home-page: https://github.com/smallcase/cdk-vpc-module.git
 Author: Bharat Parmar<bharat.parmar@smallcase.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/smallcase/cdk-vpc-module.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

