# Comparing `tmp/flask_admin_dashboard-1.0.4.tar.gz` & `tmp/flask_admin_dashboard-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_admin_dashboard-1.0.4.tar", last modified: Thu May  4 18:46:46 2023, max compression
+gzip compressed data, was "flask_admin_dashboard-1.0.5.tar", last modified: Thu May  4 18:51:11 2023, max compression
```

## Comparing `flask_admin_dashboard-1.0.4.tar` & `flask_admin_dashboard-1.0.5.tar`

### file list

```diff
@@ -1,51 +1,49 @@
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/
--rw-r--r--   0 will      (1000) will      (1000)       29 2023-05-04 18:06:25.000000 flask_admin_dashboard-1.0.4/MANIFEST.in
--rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)      227 2023-04-28 15:28:56.000000 flask_admin_dashboard-1.0.4/README.md
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/flask_admin_dashboard/
--rw-r--r--   0 will      (1000) will      (1000)       43 2023-04-27 20:30:54.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     4567 2023-04-28 18:53:23.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/admin_dashboard.py
--rw-r--r--   0 will      (1000) will      (1000)     2801 2023-04-26 18:04:44.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/models.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/flask_admin_dashboard/scripts/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:08.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/scripts/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)      542 2023-04-28 17:25:40.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/scripts/cli.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/flask_admin_dashboard/templates/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-05-04 18:36:42.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/templates/__init__.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/flask_admin_dashboard/utilities/
--rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:38.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/utilities/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     3179 2022-06-15 20:05:15.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/utilities/cache.py
--rw-r--r--   0 will      (1000) will      (1000)     2230 2022-07-22 00:01:05.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/utilities/jsonhandler.py
--rw-r--r--   0 will      (1000) will      (1000)      648 2022-12-01 19:01:53.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/utilities/timehandler.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/flask_admin_dashboard/views/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:14.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/views/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     4034 2023-04-26 20:07:54.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/views/auth.py
--rw-r--r--   0 will      (1000) will      (1000)      843 2023-01-03 17:13:42.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard/views/logs.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/
--rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)     1214 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 will      (1000) will      (1000)       65 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 will      (1000) will      (1000)      276 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/requires.txt
--rw-r--r--   0 will      (1000) will      (1000)       22 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/top_level.txt
--rw-r--r--   0 will      (1000) will      (1000)       38 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/setup.cfg
--rw-r--r--   0 will      (1000) will      (1000)     1266 2023-05-04 18:46:44.000000 flask_admin_dashboard-1.0.4/setup.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/static/
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/static/assets/
--rw-r--r--   0 will      (1000) will      (1000)    95818 2022-05-18 16:59:23.000000 flask_admin_dashboard-1.0.4/static/assets/Eo_circle_green_checkmark.svg.png
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/static/css/
--rw-r--r--   0 will      (1000) will      (1000)       81 2023-04-26 19:56:31.000000 flask_admin_dashboard-1.0.4/static/css/admin.css
--rw-r--r--   0 will      (1000) will      (1000)     3365 2022-05-18 16:59:23.000000 flask_admin_dashboard-1.0.4/static/css/login.css
--rw-r--r--   0 will      (1000) will      (1000)      364 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.4/static/css/main.css
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/static/js/
--rw-r--r--   0 will      (1000) will      (1000)     1188 2022-06-21 22:03:38.000000 flask_admin_dashboard-1.0.4/static/js/codemirror.js
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/templates/
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/templates/admin/
--rw-r--r--   0 will      (1000) will      (1000)     1742 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.4/templates/admin/authorization_status.html
--rw-r--r--   0 will      (1000) will      (1000)      114 2023-04-26 19:53:07.000000 flask_admin_dashboard-1.0.4/templates/admin/index.html
--rw-r--r--   0 will      (1000) will      (1000)     2974 2023-04-26 20:01:55.000000 flask_admin_dashboard-1.0.4/templates/admin/logs.html
--rw-r--r--   0 will      (1000) will      (1000)      275 2023-04-28 16:59:47.000000 flask_admin_dashboard-1.0.4/templates/admin/master.html
--rw-r--r--   0 will      (1000) will      (1000)     1278 2022-11-16 22:24:00.000000 flask_admin_dashboard-1.0.4/templates/admin/token_edit.html
--rw-r--r--   0 will      (1000) will      (1000)     1180 2022-11-16 20:50:44.000000 flask_admin_dashboard-1.0.4/templates/admin/tokens.html
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:46:46.972848 flask_admin_dashboard-1.0.4/templates/security/
--rw-r--r--   0 will      (1000) will      (1000)     2277 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.4/templates/security/login.html
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-05-04 18:50:22.000000 flask_admin_dashboard-1.0.5/MANIFEST.in
+-rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)      227 2023-04-28 15:28:56.000000 flask_admin_dashboard-1.0.5/README.md
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/flask_admin_dashboard/
+-rw-r--r--   0 will      (1000) will      (1000)       43 2023-04-27 20:30:54.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     4567 2023-04-28 18:53:23.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/admin_dashboard.py
+-rw-r--r--   0 will      (1000) will      (1000)     2801 2023-04-26 18:04:44.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/models.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/flask_admin_dashboard/scripts/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:08.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/scripts/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)      542 2023-04-28 17:25:40.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/scripts/cli.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/flask_admin_dashboard/utilities/
+-rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:38.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/utilities/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     3179 2022-06-15 20:05:15.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/utilities/cache.py
+-rw-r--r--   0 will      (1000) will      (1000)     2230 2022-07-22 00:01:05.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/utilities/jsonhandler.py
+-rw-r--r--   0 will      (1000) will      (1000)      648 2022-12-01 19:01:53.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/utilities/timehandler.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/flask_admin_dashboard/views/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:14.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/views/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     4034 2023-04-26 20:07:54.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/views/auth.py
+-rw-r--r--   0 will      (1000) will      (1000)      843 2023-01-03 17:13:42.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard/views/logs.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/
+-rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 18:51:11.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)     1170 2023-05-04 18:51:11.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 18:51:11.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 will      (1000) will      (1000)       65 2023-05-04 18:51:11.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 will      (1000) will      (1000)      276 2023-05-04 18:51:11.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/requires.txt
+-rw-r--r--   0 will      (1000) will      (1000)       22 2023-05-04 18:51:11.000000 flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 will      (1000) will      (1000)       38 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/setup.cfg
+-rw-r--r--   0 will      (1000) will      (1000)     1309 2023-05-04 18:51:07.000000 flask_admin_dashboard-1.0.5/setup.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/static/
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/static/assets/
+-rw-r--r--   0 will      (1000) will      (1000)    95818 2022-05-18 16:59:23.000000 flask_admin_dashboard-1.0.5/static/assets/Eo_circle_green_checkmark.svg.png
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/static/css/
+-rw-r--r--   0 will      (1000) will      (1000)       81 2023-04-26 19:56:31.000000 flask_admin_dashboard-1.0.5/static/css/admin.css
+-rw-r--r--   0 will      (1000) will      (1000)     3365 2022-05-18 16:59:23.000000 flask_admin_dashboard-1.0.5/static/css/login.css
+-rw-r--r--   0 will      (1000) will      (1000)      364 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.5/static/css/main.css
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/static/js/
+-rw-r--r--   0 will      (1000) will      (1000)     1188 2022-06-21 22:03:38.000000 flask_admin_dashboard-1.0.5/static/js/codemirror.js
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/templates/
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/templates/admin/
+-rw-r--r--   0 will      (1000) will      (1000)     1742 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.5/templates/admin/authorization_status.html
+-rw-r--r--   0 will      (1000) will      (1000)      114 2023-04-26 19:53:07.000000 flask_admin_dashboard-1.0.5/templates/admin/index.html
+-rw-r--r--   0 will      (1000) will      (1000)     2974 2023-04-26 20:01:55.000000 flask_admin_dashboard-1.0.5/templates/admin/logs.html
+-rw-r--r--   0 will      (1000) will      (1000)      275 2023-04-28 16:59:47.000000 flask_admin_dashboard-1.0.5/templates/admin/master.html
+-rw-r--r--   0 will      (1000) will      (1000)     1278 2022-11-16 22:24:00.000000 flask_admin_dashboard-1.0.5/templates/admin/token_edit.html
+-rw-r--r--   0 will      (1000) will      (1000)     1180 2022-11-16 20:50:44.000000 flask_admin_dashboard-1.0.5/templates/admin/tokens.html
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 18:51:11.286961 flask_admin_dashboard-1.0.5/templates/security/
+-rw-r--r--   0 will      (1000) will      (1000)     2277 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.5/templates/security/login.html
```

### Comparing `flask_admin_dashboard-1.0.4/PKG-INFO` & `flask_admin_dashboard-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_admin_dashboard
-Version: 1.0.4
+Version: 1.0.5
 Summary: Admin Dashboard for Flask
 Home-page: https://bitbucket.org/theapiguys/flask_admin_dashboard
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard/admin_dashboard.py` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard/admin_dashboard.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard/models.py` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard/models.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard/scripts/cli.py` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard/utilities/cache.py` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard/utilities/jsonhandler.py` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard/utilities/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard/utilities/timehandler.py` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard/utilities/timehandler.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard/views/auth.py` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard/views/auth.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard/views/logs.py` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard/views/logs.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/PKG-INFO` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-admin-dashboard
-Version: 1.0.4
+Version: 1.0.5
 Summary: Admin Dashboard for Flask
 Home-page: https://bitbucket.org/theapiguys/flask_admin_dashboard
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flask_admin_dashboard-1.0.4/flask_admin_dashboard.egg-info/SOURCES.txt` & `flask_admin_dashboard-1.0.5/flask_admin_dashboard.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 flask_admin_dashboard.egg-info/dependency_links.txt
 flask_admin_dashboard.egg-info/entry_points.txt
 flask_admin_dashboard.egg-info/not-zip-safe
 flask_admin_dashboard.egg-info/requires.txt
 flask_admin_dashboard.egg-info/top_level.txt
 flask_admin_dashboard/scripts/__init__.py
 flask_admin_dashboard/scripts/cli.py
-flask_admin_dashboard/templates/__init__.py
 flask_admin_dashboard/utilities/__init__.py
 flask_admin_dashboard/utilities/cache.py
 flask_admin_dashboard/utilities/jsonhandler.py
 flask_admin_dashboard/utilities/timehandler.py
 flask_admin_dashboard/views/__init__.py
 flask_admin_dashboard/views/auth.py
 flask_admin_dashboard/views/logs.py
```

### Comparing `flask_admin_dashboard-1.0.4/setup.py` & `flask_admin_dashboard-1.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='flask_admin_dashboard',
-    version='1.0.4',
+    version='1.0.5',
     description='Admin Dashboard for Flask',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/flask_admin_dashboard',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
     zip_safe = False,
-    packages=['flask_admin_dashboard'],
+    packages=find_packages(),
+    package_data={'': ['*.html', '*.js', '*.css']},
     include_package_data=True,
     install_requires=[
         "Flask==2.2.3",
         "email-validator",
         "python-dateutil",
         "Flask-Admin==1.6.1",
         "Flask-Security==3.0.0",
```

### Comparing `flask_admin_dashboard-1.0.4/static/assets/Eo_circle_green_checkmark.svg.png` & `flask_admin_dashboard-1.0.5/static/assets/Eo_circle_green_checkmark.svg.png`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/static/css/login.css` & `flask_admin_dashboard-1.0.5/static/css/login.css`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/static/js/codemirror.js` & `flask_admin_dashboard-1.0.5/static/js/codemirror.js`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/templates/admin/authorization_status.html` & `flask_admin_dashboard-1.0.5/templates/admin/authorization_status.html`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/templates/admin/logs.html` & `flask_admin_dashboard-1.0.5/templates/admin/logs.html`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/templates/admin/token_edit.html` & `flask_admin_dashboard-1.0.5/templates/admin/token_edit.html`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/templates/admin/tokens.html` & `flask_admin_dashboard-1.0.5/templates/admin/tokens.html`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.4/templates/security/login.html` & `flask_admin_dashboard-1.0.5/templates/security/login.html`

 * *Files identical despite different names*

