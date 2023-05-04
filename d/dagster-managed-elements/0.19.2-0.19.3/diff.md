# Comparing `tmp/dagster-managed-elements-0.19.2.tar.gz` & `tmp/dagster-managed-elements-0.19.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-managed-elements-0.19.2.tar", last modified: Thu Apr 27 19:35:23 2023, max compression
+gzip compressed data, was "dagster-managed-elements-0.19.3.tar", last modified: Thu May  4 17:53:08 2023, max compression
```

## Comparing `dagster-managed-elements-0.19.2.tar` & `dagster-managed-elements-0.19.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:23.288533 dagster-managed-elements-0.19.2/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-27 18:30:35.000000 dagster-managed-elements-0.19.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-27 18:30:35.000000 dagster-managed-elements-0.19.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      686 2023-04-27 19:35:23.288533 dagster-managed-elements-0.19.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-27 18:30:35.000000 dagster-managed-elements-0.19.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:23.284533 dagster-managed-elements-0.19.2/dagster_managed_elements/
--rw-r--r--   0 root         (0) root         (0)      202 2023-04-27 18:30:35.000000 dagster-managed-elements-0.19.2/dagster_managed_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6327 2023-04-27 18:30:35.000000 dagster-managed-elements-0.19.2/dagster_managed_elements/cli.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-04-27 18:30:35.000000 dagster-managed-elements-0.19.2/dagster_managed_elements/types.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-04-27 18:30:35.000000 dagster-managed-elements-0.19.2/dagster_managed_elements/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-27 18:30:35.000000 dagster-managed-elements-0.19.2/dagster_managed_elements/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:35:23.288533 dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-04-27 19:35:22.000000 dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2023-04-27 19:35:22.000000 dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:35:22.000000 dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-04-27 19:35:22.000000 dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:35:22.000000 dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 19:35:22.000000 dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-27 19:35:22.000000 dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-27 19:35:23.288533 dagster-managed-elements-0.19.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1518 2023-04-27 18:30:35.000000 dagster-managed-elements-0.19.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:53:07.996823 dagster-managed-elements-0.19.3/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-04 17:42:14.000000 dagster-managed-elements-0.19.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-04 17:42:14.000000 dagster-managed-elements-0.19.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-04 17:53:07.996823 dagster-managed-elements-0.19.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-04 17:42:14.000000 dagster-managed-elements-0.19.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:53:07.996823 dagster-managed-elements-0.19.3/dagster_managed_elements/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-04 17:42:14.000000 dagster-managed-elements-0.19.3/dagster_managed_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-05-04 17:42:14.000000 dagster-managed-elements-0.19.3/dagster_managed_elements/cli.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-05-04 17:42:14.000000 dagster-managed-elements-0.19.3/dagster_managed_elements/types.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-05-04 17:42:14.000000 dagster-managed-elements-0.19.3/dagster_managed_elements/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-04 17:42:14.000000 dagster-managed-elements-0.19.3/dagster_managed_elements/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:53:07.996823 dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-04 17:53:07.000000 dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2023-05-04 17:53:07.000000 dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:53:07.000000 dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-04 17:53:07.000000 dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:53:07.000000 dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 17:53:07.000000 dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-04 17:53:07.000000 dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-04 17:53:08.000823 dagster-managed-elements-0.19.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-05-04 17:42:14.000000 dagster-managed-elements-0.19.3/setup.py
```

### Comparing `dagster-managed-elements-0.19.2/LICENSE` & `dagster-managed-elements-0.19.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.2/PKG-INFO` & `dagster-managed-elements-0.19.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.19.2
+Version: 0.19.3
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-managed-elements-0.19.2/dagster_managed_elements/cli.py` & `dagster-managed-elements-0.19.3/dagster_managed_elements/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.2/dagster_managed_elements/types.py` & `dagster-managed-elements-0.19.3/dagster_managed_elements/types.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.2/dagster_managed_elements/utils.py` & `dagster-managed-elements-0.19.3/dagster_managed_elements/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/PKG-INFO` & `dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-managed-elements
-Version: 0.19.2
+Version: 0.19.3
 Summary: Package for Managed elements with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-managed-elements
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-managed-elements-0.19.2/dagster_managed_elements.egg-info/SOURCES.txt` & `dagster-managed-elements-0.19.3/dagster_managed_elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-managed-elements-0.19.2/setup.py` & `dagster-managed-elements-0.19.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_managed_elements_tests*"]),
-    install_requires=["dagster==1.3.2", "requests", "click_spinner"],
+    install_requires=["dagster==1.3.3", "requests", "click_spinner"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-managed-elements = dagster_managed_elements.cli:main",
             "dagster-me = dagster_managed_elements.cli:main",
         ]
     },
```

