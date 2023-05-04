# Comparing `tmp/cdk-stacksets-0.0.93.tar.gz` & `tmp/cdk-stacksets-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-stacksets-0.0.93.tar", last modified: Wed May  3 00:15:56 2023, max compression
+gzip compressed data, was "cdk-stacksets-0.0.94.tar", last modified: Thu May  4 00:17:08 2023, max compression
```

## Comparing `cdk-stacksets-0.0.93.tar` & `cdk-stacksets-0.0.94.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:15:56.614392 cdk-stacksets-0.0.93/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 00:15:42.000000 cdk-stacksets-0.0.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 00:15:42.000000 cdk-stacksets-0.0.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-03 00:15:56.614392 cdk-stacksets-0.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-03 00:15:42.000000 cdk-stacksets-0.0.93/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 00:15:42.000000 cdk-stacksets-0.0.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 00:15:56.614392 cdk-stacksets-0.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-03 00:15:42.000000 cdk-stacksets-0.0.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:15:56.610392 cdk-stacksets-0.0.93/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:15:56.610392 cdk-stacksets-0.0.93/src/cdk_stacksets/
--rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-05-03 00:15:42.000000 cdk-stacksets-0.0.93/src/cdk_stacksets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:15:56.610392 cdk-stacksets-0.0.93/src/cdk_stacksets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-03 00:15:42.000000 cdk-stacksets-0.0.93/src/cdk_stacksets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71059 2023-05-03 00:15:42.000000 cdk-stacksets-0.0.93/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.93.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:15:42.000000 cdk-stacksets-0.0.93/src/cdk_stacksets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:15:56.610392 cdk-stacksets-0.0.93/src/cdk_stacksets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-03 00:15:56.000000 cdk-stacksets-0.0.93/src/cdk_stacksets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 00:15:56.000000 cdk-stacksets-0.0.93/src/cdk_stacksets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:15:56.000000 cdk-stacksets-0.0.93/src/cdk_stacksets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 00:15:56.000000 cdk-stacksets-0.0.93/src/cdk_stacksets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 00:15:56.000000 cdk-stacksets-0.0.93/src/cdk_stacksets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:17:08.951476 cdk-stacksets-0.0.94/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 00:16:53.000000 cdk-stacksets-0.0.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 00:16:53.000000 cdk-stacksets-0.0.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-04 00:17:08.951476 cdk-stacksets-0.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-04 00:16:53.000000 cdk-stacksets-0.0.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 00:16:53.000000 cdk-stacksets-0.0.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 00:17:08.951476 cdk-stacksets-0.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 00:16:53.000000 cdk-stacksets-0.0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:17:08.947476 cdk-stacksets-0.0.94/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:17:08.951476 cdk-stacksets-0.0.94/src/cdk_stacksets/
+-rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-05-04 00:16:53.000000 cdk-stacksets-0.0.94/src/cdk_stacksets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:17:08.951476 cdk-stacksets-0.0.94/src/cdk_stacksets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-04 00:16:53.000000 cdk-stacksets-0.0.94/src/cdk_stacksets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71057 2023-05-04 00:16:53.000000 cdk-stacksets-0.0.94/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.94.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:16:53.000000 cdk-stacksets-0.0.94/src/cdk_stacksets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:17:08.951476 cdk-stacksets-0.0.94/src/cdk_stacksets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-04 00:17:08.000000 cdk-stacksets-0.0.94/src/cdk_stacksets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-04 00:17:08.000000 cdk-stacksets-0.0.94/src/cdk_stacksets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:17:08.000000 cdk-stacksets-0.0.94/src/cdk_stacksets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 00:17:08.000000 cdk-stacksets-0.0.94/src/cdk_stacksets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 00:17:08.000000 cdk-stacksets-0.0.94/src/cdk_stacksets.egg-info/top_level.txt
```

### Comparing `cdk-stacksets-0.0.93/LICENSE` & `cdk-stacksets-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.93/PKG-INFO` & `cdk-stacksets-0.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.93
+Version: 0.0.94
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-stacksets-0.0.93/README.md` & `cdk-stacksets-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.93/setup.py` & `cdk-stacksets-0.0.94/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-stacksets",
-    "version": "0.0.93",
+    "version": "0.0.94",
     "description": "cdk-stacksets",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-stacksets.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_stacksets",
         "cdk_stacksets._jsii"
     ],
     "package_data": {
         "cdk_stacksets._jsii": [
-            "cdk-stacksets@0.0.93.jsii.tgz"
+            "cdk-stacksets@0.0.94.jsii.tgz"
         ],
         "cdk_stacksets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-stacksets-0.0.93/src/cdk_stacksets/__init__.py` & `cdk-stacksets-0.0.94/src/cdk_stacksets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.93/src/cdk_stacksets.egg-info/PKG-INFO` & `cdk-stacksets-0.0.94/src/cdk_stacksets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.93
+Version: 0.0.94
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

