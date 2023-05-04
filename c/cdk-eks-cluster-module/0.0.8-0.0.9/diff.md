# Comparing `tmp/cdk-eks-cluster-module-0.0.8.tar.gz` & `tmp/cdk-eks-cluster-module-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-eks-cluster-module-0.0.8.tar", last modified: Wed May 18 10:07:30 2022, max compression
+gzip compressed data, was "cdk-eks-cluster-module-0.0.9.tar", last modified: Fri May 20 09:33:29 2022, max compression
```

## Comparing `cdk-eks-cluster-module-0.0.8.tar` & `cdk-eks-cluster-module-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 10:07:30.518287 cdk-eks-cluster-module-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-18 10:07:17.000000 cdk-eks-cluster-module-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-18 10:07:17.000000 cdk-eks-cluster-module-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6658 2022-05-18 10:07:30.518287 cdk-eks-cluster-module-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5717 2022-05-18 10:07:17.000000 cdk-eks-cluster-module-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-18 10:07:17.000000 cdk-eks-cluster-module-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-18 10:07:30.518287 cdk-eks-cluster-module-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-05-18 10:07:17.000000 cdk-eks-cluster-module-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 10:07:30.514287 cdk-eks-cluster-module-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 10:07:30.518287 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module/
--rw-r--r--   0 runner    (1001) docker     (121)    53079 2022-05-18 10:07:17.000000 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 10:07:30.518287 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-05-18 10:07:17.000000 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    58126 2022-05-18 10:07:17.000000 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module/_jsii/cdk-eks-cluster-module@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-18 10:07:17.000000 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 10:07:30.518287 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6658 2022-05-18 10:07:30.000000 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-18 10:07:30.000000 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-18 10:07:30.000000 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-18 10:07:30.000000 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-18 10:07:30.000000 cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 09:33:29.756156 cdk-eks-cluster-module-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-05-20 09:33:18.000000 cdk-eks-cluster-module-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-20 09:33:18.000000 cdk-eks-cluster-module-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6658 2022-05-20 09:33:29.756156 cdk-eks-cluster-module-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5717 2022-05-20 09:33:18.000000 cdk-eks-cluster-module-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-20 09:33:18.000000 cdk-eks-cluster-module-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-20 09:33:29.756156 cdk-eks-cluster-module-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-05-20 09:33:18.000000 cdk-eks-cluster-module-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 09:33:29.756156 cdk-eks-cluster-module-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 09:33:29.756156 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module/
+-rw-r--r--   0 runner    (1001) docker     (121)    53079 2022-05-20 09:33:18.000000 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 09:33:29.756156 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2022-05-20 09:33:18.000000 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58158 2022-05-20 09:33:18.000000 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module/_jsii/cdk-eks-cluster-module@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 09:33:18.000000 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 09:33:29.756156 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6658 2022-05-20 09:33:29.000000 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-20 09:33:29.000000 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 09:33:29.000000 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-05-20 09:33:29.000000 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-20 09:33:29.000000 cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module.egg-info/top_level.txt
```

### Comparing `cdk-eks-cluster-module-0.0.8/LICENSE` & `cdk-eks-cluster-module-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-eks-cluster-module-0.0.8/PKG-INFO` & `cdk-eks-cluster-module-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-eks-cluster-module
-Version: 0.0.8
+Version: 0.0.9
 Summary: @smallcase/cdk-eks-cluster-module
 Home-page: https://github.com/smallcase/cdk-eks-cluster-module.git
 Author: @InfraTeam<bharat.parmar@smallcase.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/smallcase/cdk-eks-cluster-module.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-eks-cluster-module-0.0.8/README.md` & `cdk-eks-cluster-module-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-eks-cluster-module-0.0.8/setup.py` & `cdk-eks-cluster-module-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-eks-cluster-module",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "@smallcase/cdk-eks-cluster-module",
     "license": "Apache-2.0",
     "url": "https://github.com/smallcase/cdk-eks-cluster-module.git",
     "long_description_content_type": "text/markdown",
     "author": "@InfraTeam<bharat.parmar@smallcase.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_eks_cluster_module",
         "cdk_eks_cluster_module._jsii"
     ],
     "package_data": {
         "cdk_eks_cluster_module._jsii": [
-            "cdk-eks-cluster-module@0.0.8.jsii.tgz"
+            "cdk-eks-cluster-module@0.0.9.jsii.tgz"
         ],
         "cdk_eks_cluster_module": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module/__init__.py` & `cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-cluster-module-0.0.8/src/cdk_eks_cluster_module.egg-info/PKG-INFO` & `cdk-eks-cluster-module-0.0.9/src/cdk_eks_cluster_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-eks-cluster-module
-Version: 0.0.8
+Version: 0.0.9
 Summary: @smallcase/cdk-eks-cluster-module
 Home-page: https://github.com/smallcase/cdk-eks-cluster-module.git
 Author: @InfraTeam<bharat.parmar@smallcase.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/smallcase/cdk-eks-cluster-module.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

