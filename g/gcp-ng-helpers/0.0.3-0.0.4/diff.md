# Comparing `tmp/gcp_ng_helpers-0.0.3.tar.gz` & `tmp/gcp_ng_helpers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_ng_helpers-0.0.3.tar", last modified: Tue Mar 21 07:04:25 2023, max compression
+gzip compressed data, was "gcp_ng_helpers-0.0.4.tar", last modified: Thu May  4 12:51:57 2023, max compression
```

## Comparing `gcp_ng_helpers-0.0.3.tar` & `gcp_ng_helpers-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 07:04:25.125210 gcp_ng_helpers-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-21 07:04:13.000000 gcp_ng_helpers-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-21 07:04:25.125210 gcp_ng_helpers-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-21 07:04:13.000000 gcp_ng_helpers-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 07:04:25.125210 gcp_ng_helpers-0.0.3/gcp_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 07:04:13.000000 gcp_ng_helpers-0.0.3/gcp_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 07:04:25.125210 gcp_ng_helpers-0.0.3/gcp_helpers/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 07:04:13.000000 gcp_ng_helpers-0.0.3/gcp_helpers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-03-21 07:04:13.000000 gcp_ng_helpers-0.0.3/gcp_helpers/functions/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-21 07:04:13.000000 gcp_ng_helpers-0.0.3/gcp_helpers/functions/routers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 07:04:25.125210 gcp_ng_helpers-0.0.3/gcp_ng_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-21 07:04:25.000000 gcp_ng_helpers-0.0.3/gcp_ng_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-21 07:04:25.000000 gcp_ng_helpers-0.0.3/gcp_ng_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 07:04:25.000000 gcp_ng_helpers-0.0.3/gcp_ng_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-21 07:04:25.000000 gcp_ng_helpers-0.0.3/gcp_ng_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-21 07:04:25.000000 gcp_ng_helpers-0.0.3/gcp_ng_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-21 07:04:13.000000 gcp_ng_helpers-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-21 07:04:25.125210 gcp_ng_helpers-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:57.887110 gcp_ng_helpers-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-04 12:51:42.000000 gcp_ng_helpers-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-04 12:51:57.887110 gcp_ng_helpers-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-04 12:51:42.000000 gcp_ng_helpers-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:57.883110 gcp_ng_helpers-0.0.4/gcp_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:42.000000 gcp_ng_helpers-0.0.4/gcp_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:57.883110 gcp_ng_helpers-0.0.4/gcp_helpers/cloud_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 12:51:42.000000 gcp_ng_helpers-0.0.4/gcp_helpers/cloud_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-04 12:51:42.000000 gcp_ng_helpers-0.0.4/gcp_helpers/cloud_tasks/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:57.883110 gcp_ng_helpers-0.0.4/gcp_helpers/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:42.000000 gcp_ng_helpers-0.0.4/gcp_helpers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-04 12:51:42.000000 gcp_ng_helpers-0.0.4/gcp_helpers/functions/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-04 12:51:42.000000 gcp_ng_helpers-0.0.4/gcp_helpers/functions/routers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:57.887110 gcp_ng_helpers-0.0.4/gcp_ng_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-04 12:51:57.000000 gcp_ng_helpers-0.0.4/gcp_ng_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-04 12:51:57.000000 gcp_ng_helpers-0.0.4/gcp_ng_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:51:57.000000 gcp_ng_helpers-0.0.4/gcp_ng_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 12:51:57.000000 gcp_ng_helpers-0.0.4/gcp_ng_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 12:51:57.000000 gcp_ng_helpers-0.0.4/gcp_ng_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-04 12:51:42.000000 gcp_ng_helpers-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-04 12:51:57.887110 gcp_ng_helpers-0.0.4/setup.cfg
```

### Comparing `gcp_ng_helpers-0.0.3/LICENSE` & `gcp_ng_helpers-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.3/PKG-INFO` & `gcp_ng_helpers-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gcp_ng_helpers
-Version: 0.0.3
-Summary: Various helper function for Google Cloud services
+Version: 0.0.4
+Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gcp_ng_helpers-0.0.3/README.md` & `gcp_ng_helpers-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.3/gcp_helpers/functions/decorators.py` & `gcp_ng_helpers-0.0.4/gcp_helpers/functions/decorators.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.3/gcp_helpers/functions/routers.py` & `gcp_ng_helpers-0.0.4/gcp_helpers/functions/routers.py`

 * *Files identical despite different names*

### Comparing `gcp_ng_helpers-0.0.3/gcp_ng_helpers.egg-info/PKG-INFO` & `gcp_ng_helpers-0.0.4/gcp_ng_helpers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gcp-ng-helpers
-Version: 0.0.3
-Summary: Various helper function for Google Cloud services
+Version: 0.0.4
+Summary: Various helper functions for Google Cloud services
 Home-page: https://github.com/NGhostClub/gcp-helpers
 Author: Dmitriy Tischenko aka NGhost
 Author-email: nghostik@gmail.com
 Project-URL: Source, https://github.com/NGhostClub/gcp-helpers
 Project-URL: Bug Tracker, https://github.com/NGhostClub/gcp-helpers/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gcp_ng_helpers-0.0.3/setup.cfg` & `gcp_ng_helpers-0.0.4/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 license_file = LICENSE
 name = gcp_ng_helpers
-version = 0.0.3
+version = 0.0.4
 author = Dmitriy Tischenko aka NGhost
 author_email = nghostik@gmail.com
-description = Various helper function for Google Cloud services
+description = Various helper functions for Google Cloud services
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/NGhostClub/gcp-helpers
 project_urls = 
 	Source = https://github.com/NGhostClub/gcp-helpers
 	Bug Tracker = https://github.com/NGhostClub/gcp-helpers/issues
 classifiers = 
@@ -17,17 +17,19 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = 
 	gcp_helpers
 	gcp_helpers.functions
+	gcp_helpers.cloud_tasks
 python_requires = >=3.10
 install_requires = 
 	flask
+	google-cloud-tasks
 
 [options.packages.find]
 where = gcp_helpers
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

