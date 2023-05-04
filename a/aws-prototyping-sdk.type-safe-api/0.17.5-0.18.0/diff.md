# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.17.5.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.17.5.tar", last modified: Tue May  2 11:00:17 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.18.0.tar", last modified: Wed May  3 05:23:07 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.17.5.tar` & `aws_prototyping_sdk.type_safe_api-0.18.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:00:17.451845 aws_prototyping_sdk.type_safe_api-0.17.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 11:00:00.000000 aws_prototyping_sdk.type_safe_api-0.17.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 11:00:00.000000 aws_prototyping_sdk.type_safe_api-0.17.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-02 11:00:17.447845 aws_prototyping_sdk.type_safe_api-0.17.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    55396 2023-05-02 11:00:00.000000 aws_prototyping_sdk.type_safe_api-0.17.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 11:00:00.000000 aws_prototyping_sdk.type_safe_api-0.17.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:00:17.451845 aws_prototyping_sdk.type_safe_api-0.17.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-02 11:00:00.000000 aws_prototyping_sdk.type_safe_api-0.17.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:00:17.443845 aws_prototyping_sdk.type_safe_api-0.17.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:00:17.443845 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:00:17.447845 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   288160 2023-05-02 11:00:00.000000 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:00:17.447845 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-02 11:00:00.000000 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   855053 2023-05-02 11:00:00.000000 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.17.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:00:00.000000 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:00:17.443845 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-02 11:00:17.000000 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-02 11:00:17.000000 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:00:17.000000 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 11:00:17.000000 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 11:00:17.000000 aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:23:07.993815 aws_prototyping_sdk.type_safe_api-0.18.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 05:22:58.000000 aws_prototyping_sdk.type_safe_api-0.18.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 05:22:58.000000 aws_prototyping_sdk.type_safe_api-0.18.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-03 05:23:07.993815 aws_prototyping_sdk.type_safe_api-0.18.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    55396 2023-05-03 05:22:58.000000 aws_prototyping_sdk.type_safe_api-0.18.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-03 05:22:58.000000 aws_prototyping_sdk.type_safe_api-0.18.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 05:23:07.997815 aws_prototyping_sdk.type_safe_api-0.18.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-03 05:22:58.000000 aws_prototyping_sdk.type_safe_api-0.18.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:23:07.989814 aws_prototyping_sdk.type_safe_api-0.18.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:23:07.989814 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:23:07.993815 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   288160 2023-05-03 05:22:58.000000 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:23:07.993815 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-03 05:22:58.000000 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   855053 2023-05-03 05:22:58.000000 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:22:58.000000 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:23:07.993815 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-03 05:23:07.000000 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-03 05:23:07.000000 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:23:07.000000 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 05:23:07.000000 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 05:23:07.000000 aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.5/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.5/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.18.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.type_safe_api
-Version: 0.17.5
+Version: 0.18.0
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.5/README.md` & `aws_prototyping_sdk.type_safe_api-0.18.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.5/setup.py` & `aws_prototyping_sdk.type_safe_api-0.18.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.17.5",
+    "version": "0.18.0",
     "description": "@aws-prototyping-sdk/type-safe-api",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,28 +22,28 @@
     },
     "packages": [
         "aws_prototyping_sdk.type_safe_api",
         "aws_prototyping_sdk.type_safe_api._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.type_safe_api._jsii": [
-            "type-safe-api@0.17.5.jsii.tgz"
+            "type-safe-api@0.18.0.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.60.0, <3.0.0",
         "aws_prototyping_sdk.pdk_nag<1.0.0",
         "cdk-nag>=2.21.65, <3.0.0",
         "constructs>=10.1.222, <11.0.0",
         "jsii>=1.80.0, <2.0.0",
-        "projen>=0.71.27, <0.72.0",
+        "projen>=0.71.35, <0.72.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk/type_safe_api/__init__.py` & `aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk/type_safe_api/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.type-safe-api
-Version: 0.17.5
+Version: 0.18.0
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.17.5/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.18.0/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.17.5.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.0.jsii.tgz
```

