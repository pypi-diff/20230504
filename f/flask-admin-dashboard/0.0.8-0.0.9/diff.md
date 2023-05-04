# Comparing `tmp/flask_admin_dashboard-0.0.8.tar.gz` & `tmp/flask_admin_dashboard-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_admin_dashboard-0.0.8.tar", last modified: Thu May  4 17:48:49 2023, max compression
+gzip compressed data, was "flask_admin_dashboard-0.0.9.tar", last modified: Thu May  4 17:51:10 2023, max compression
```

## Comparing `flask_admin_dashboard-0.0.8.tar` & `flask_admin_dashboard-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:48:49.090631 flask_admin_dashboard-0.0.8/
--rw-r--r--   0 will      (1000) will      (1000)       81 2023-05-04 17:43:07.000000 flask_admin_dashboard-0.0.8/MANIFEST.in
--rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 17:48:49.090631 flask_admin_dashboard-0.0.8/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)      227 2023-04-28 15:28:56.000000 flask_admin_dashboard-0.0.8/README.md
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:48:49.090631 flask_admin_dashboard-0.0.8/flask_admin_dashboard/
--rw-r--r--   0 will      (1000) will      (1000)       43 2023-04-27 20:30:54.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     4567 2023-04-28 18:53:23.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/admin_dashboard.py
--rw-r--r--   0 will      (1000) will      (1000)     2801 2023-04-26 18:04:44.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/models.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:48:49.090631 flask_admin_dashboard-0.0.8/flask_admin_dashboard/scripts/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:08.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/scripts/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)      542 2023-04-28 17:25:40.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/scripts/cli.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:48:49.090631 flask_admin_dashboard-0.0.8/flask_admin_dashboard/utilities/
--rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:38.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/utilities/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     3179 2022-06-15 20:05:15.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/utilities/cache.py
--rw-r--r--   0 will      (1000) will      (1000)     2230 2022-07-22 00:01:05.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/utilities/jsonhandler.py
--rw-r--r--   0 will      (1000) will      (1000)      648 2022-12-01 19:01:53.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/utilities/timehandler.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:48:49.090631 flask_admin_dashboard-0.0.8/flask_admin_dashboard/views/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:14.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/views/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     4034 2023-04-26 20:07:54.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/views/auth.py
--rw-r--r--   0 will      (1000) will      (1000)      843 2023-01-03 17:13:42.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard/views/logs.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:48:49.090631 flask_admin_dashboard-0.0.8/flask_admin_dashboard.egg-info/
--rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 17:48:49.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)      779 2023-05-04 17:48:49.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 17:48:49.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 will      (1000) will      (1000)       65 2023-05-04 17:48:49.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 will      (1000) will      (1000)      276 2023-05-04 17:48:49.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard.egg-info/requires.txt
--rw-r--r--   0 will      (1000) will      (1000)       22 2023-05-04 17:48:49.000000 flask_admin_dashboard-0.0.8/flask_admin_dashboard.egg-info/top_level.txt
--rw-r--r--   0 will      (1000) will      (1000)       38 2023-05-04 17:48:49.090631 flask_admin_dashboard-0.0.8/setup.cfg
--rw-r--r--   0 will      (1000) will      (1000)     1243 2023-05-04 17:48:46.000000 flask_admin_dashboard-0.0.8/setup.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:51:10.575049 flask_admin_dashboard-0.0.9/
+-rw-r--r--   0 will      (1000) will      (1000)       37 2023-05-04 17:50:55.000000 flask_admin_dashboard-0.0.9/MANIFEST.in
+-rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 17:51:10.575049 flask_admin_dashboard-0.0.9/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)      227 2023-04-28 15:28:56.000000 flask_admin_dashboard-0.0.9/README.md
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:51:10.575049 flask_admin_dashboard-0.0.9/flask_admin_dashboard/
+-rw-r--r--   0 will      (1000) will      (1000)       43 2023-04-27 20:30:54.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     4567 2023-04-28 18:53:23.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/admin_dashboard.py
+-rw-r--r--   0 will      (1000) will      (1000)     2801 2023-04-26 18:04:44.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/models.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:51:10.575049 flask_admin_dashboard-0.0.9/flask_admin_dashboard/scripts/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:08.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/scripts/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)      542 2023-04-28 17:25:40.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/scripts/cli.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:51:10.575049 flask_admin_dashboard-0.0.9/flask_admin_dashboard/utilities/
+-rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:38.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/utilities/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     3179 2022-06-15 20:05:15.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/utilities/cache.py
+-rw-r--r--   0 will      (1000) will      (1000)     2230 2022-07-22 00:01:05.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/utilities/jsonhandler.py
+-rw-r--r--   0 will      (1000) will      (1000)      648 2022-12-01 19:01:53.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/utilities/timehandler.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:51:10.575049 flask_admin_dashboard-0.0.9/flask_admin_dashboard/views/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:14.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/views/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     4034 2023-04-26 20:07:54.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/views/auth.py
+-rw-r--r--   0 will      (1000) will      (1000)      843 2023-01-03 17:13:42.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard/views/logs.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 17:51:10.575049 flask_admin_dashboard-0.0.9/flask_admin_dashboard.egg-info/
+-rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 17:51:10.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)      779 2023-05-04 17:51:10.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 17:51:10.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 will      (1000) will      (1000)       65 2023-05-04 17:51:10.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 will      (1000) will      (1000)      276 2023-05-04 17:51:10.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard.egg-info/requires.txt
+-rw-r--r--   0 will      (1000) will      (1000)       22 2023-05-04 17:51:10.000000 flask_admin_dashboard-0.0.9/flask_admin_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 will      (1000) will      (1000)       38 2023-05-04 17:51:10.575049 flask_admin_dashboard-0.0.9/setup.cfg
+-rw-r--r--   0 will      (1000) will      (1000)     1243 2023-05-04 17:51:08.000000 flask_admin_dashboard-0.0.9/setup.py
```

### Comparing `flask_admin_dashboard-0.0.8/PKG-INFO` & `flask_admin_dashboard-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_admin_dashboard
-Version: 0.0.8
+Version: 0.0.9
 Summary: Admin Dashboard for Flask
 Home-page: https://bitbucket.org/theapiguys/flask_admin_dashboard
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard/admin_dashboard.py` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard/admin_dashboard.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard/models.py` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard/models.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard/scripts/cli.py` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard/utilities/cache.py` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard/utilities/jsonhandler.py` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard/utilities/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard/utilities/timehandler.py` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard/utilities/timehandler.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard/views/auth.py` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard/views/auth.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard/views/logs.py` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard/views/logs.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard.egg-info/PKG-INFO` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-admin-dashboard
-Version: 0.0.8
+Version: 0.0.9
 Summary: Admin Dashboard for Flask
 Home-page: https://bitbucket.org/theapiguys/flask_admin_dashboard
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flask_admin_dashboard-0.0.8/flask_admin_dashboard.egg-info/SOURCES.txt` & `flask_admin_dashboard-0.0.9/flask_admin_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-0.0.8/setup.py` & `flask_admin_dashboard-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='flask_admin_dashboard',
-    version='0.0.8',
+    version='0.0.9',
     description='Admin Dashboard for Flask',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/flask_admin_dashboard',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

