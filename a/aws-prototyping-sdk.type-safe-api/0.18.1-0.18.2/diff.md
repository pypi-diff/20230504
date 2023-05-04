# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.18.1.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.18.1.tar", last modified: Thu May  4 05:10:54 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.18.2.tar", last modified: Thu May  4 06:18:26 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.18.1.tar` & `aws_prototyping_sdk.type_safe_api-0.18.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:54.799454 aws_prototyping_sdk.type_safe_api-0.18.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 05:10:45.000000 aws_prototyping_sdk.type_safe_api-0.18.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 05:10:45.000000 aws_prototyping_sdk.type_safe_api-0.18.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-04 05:10:54.799454 aws_prototyping_sdk.type_safe_api-0.18.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    55396 2023-05-04 05:10:45.000000 aws_prototyping_sdk.type_safe_api-0.18.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 05:10:45.000000 aws_prototyping_sdk.type_safe_api-0.18.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:54.799454 aws_prototyping_sdk.type_safe_api-0.18.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-04 05:10:45.000000 aws_prototyping_sdk.type_safe_api-0.18.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:54.795454 aws_prototyping_sdk.type_safe_api-0.18.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:54.795454 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:54.799454 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   288160 2023-05-04 05:10:45.000000 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:54.799454 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-04 05:10:45.000000 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   855054 2023-05-04 05:10:45.000000 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:45.000000 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:54.795454 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-04 05:10:54.000000 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 05:10:54.000000 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:54.000000 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-04 05:10:54.000000 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 05:10:54.000000 aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.326030 aws_prototyping_sdk.type_safe_api-0.18.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-04 06:18:26.326030 aws_prototyping_sdk.type_safe_api-0.18.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    55396 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 06:18:26.326030 aws_prototyping_sdk.type_safe_api-0.18.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   288160 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   855054 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.1/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.1/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.18.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.type_safe_api
-Version: 0.18.1
+Version: 0.18.2
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.1/README.md` & `aws_prototyping_sdk.type_safe_api-0.18.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.1/setup.py` & `aws_prototyping_sdk.type_safe_api-0.18.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.18.1",
+    "version": "0.18.2",
     "description": "@aws-prototyping-sdk/type-safe-api",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_prototyping_sdk.type_safe_api",
         "aws_prototyping_sdk.type_safe_api._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.type_safe_api._jsii": [
-            "type-safe-api@0.18.1.jsii.tgz"
+            "type-safe-api@0.18.2.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk/type_safe_api/__init__.py` & `aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.type-safe-api
-Version: 0.18.1
+Version: 0.18.2
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.1/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.1.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.2.jsii.tgz
```

