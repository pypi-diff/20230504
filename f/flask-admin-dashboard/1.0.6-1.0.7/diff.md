# Comparing `tmp/flask_admin_dashboard-1.0.6.tar.gz` & `tmp/flask_admin_dashboard-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_admin_dashboard-1.0.6.tar", last modified: Thu May  4 19:03:26 2023, max compression
+gzip compressed data, was "flask_admin_dashboard-1.0.7.tar", last modified: Thu May  4 19:09:23 2023, max compression
```

## Comparing `flask_admin_dashboard-1.0.6.tar` & `flask_admin_dashboard-1.0.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/
--rw-r--r--   0 will      (1000) will      (1000)      164 2023-05-04 19:03:24.000000 flask_admin_dashboard-1.0.6/MANIFEST.in
--rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)      227 2023-04-28 15:28:56.000000 flask_admin_dashboard-1.0.6/README.md
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/
--rw-r--r--   0 will      (1000) will      (1000)       43 2023-04-27 20:30:54.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     4567 2023-04-28 18:53:23.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/admin_dashboard.py
--rw-r--r--   0 will      (1000) will      (1000)     2801 2023-04-26 18:04:44.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/models.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/scripts/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:08.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/scripts/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)      542 2023-04-28 17:25:40.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/scripts/cli.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/assets/
--rw-r--r--   0 will      (1000) will      (1000)    95818 2022-05-18 16:59:23.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/assets/Eo_circle_green_checkmark.svg.png
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/css/
--rw-r--r--   0 will      (1000) will      (1000)       81 2023-04-26 19:56:31.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/css/admin.css
--rw-r--r--   0 will      (1000) will      (1000)     3365 2022-05-18 16:59:23.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/css/login.css
--rw-r--r--   0 will      (1000) will      (1000)      364 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/css/main.css
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/js/
--rw-r--r--   0 will      (1000) will      (1000)     1188 2022-06-21 22:03:38.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/js/codemirror.js
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/
--rw-r--r--   0 will      (1000) will      (1000)     1742 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/authorization_status.html
--rw-r--r--   0 will      (1000) will      (1000)      114 2023-04-26 19:53:07.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/index.html
--rw-r--r--   0 will      (1000) will      (1000)     2974 2023-04-26 20:01:55.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/logs.html
--rw-r--r--   0 will      (1000) will      (1000)      275 2023-04-28 16:59:47.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/master.html
--rw-r--r--   0 will      (1000) will      (1000)     1278 2022-11-16 22:24:00.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/token_edit.html
--rw-r--r--   0 will      (1000) will      (1000)     1180 2022-11-16 20:50:44.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/tokens.html
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/security/
--rw-r--r--   0 will      (1000) will      (1000)     2277 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/security/login.html
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/utilities/
--rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:38.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/utilities/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     3179 2022-06-15 20:05:15.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/utilities/cache.py
--rw-r--r--   0 will      (1000) will      (1000)     2230 2022-07-22 00:01:05.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/utilities/jsonhandler.py
--rw-r--r--   0 will      (1000) will      (1000)      648 2022-12-01 19:01:53.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/utilities/timehandler.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard/views/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:14.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/views/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     4034 2023-04-26 20:07:54.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/views/auth.py
--rw-r--r--   0 will      (1000) will      (1000)      843 2023-01-03 17:13:42.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard/views/logs.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/
--rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 19:03:26.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)     1434 2023-05-04 19:03:26.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 19:03:26.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 will      (1000) will      (1000)       65 2023-05-04 19:03:26.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/not-zip-safe
--rw-r--r--   0 will      (1000) will      (1000)      276 2023-05-04 19:03:26.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/requires.txt
--rw-r--r--   0 will      (1000) will      (1000)       22 2023-05-04 19:03:26.000000 flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/top_level.txt
--rw-r--r--   0 will      (1000) will      (1000)       38 2023-05-04 19:03:26.969408 flask_admin_dashboard-1.0.6/setup.cfg
--rw-r--r--   0 will      (1000) will      (1000)     1309 2023-05-04 18:58:30.000000 flask_admin_dashboard-1.0.6/setup.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/
+-rw-r--r--   0 will      (1000) will      (1000)      164 2023-05-04 19:03:24.000000 flask_admin_dashboard-1.0.7/MANIFEST.in
+-rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)      227 2023-04-28 15:28:56.000000 flask_admin_dashboard-1.0.7/README.md
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/
+-rw-r--r--   0 will      (1000) will      (1000)       43 2023-04-27 20:30:54.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     4613 2023-05-04 19:09:04.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/admin_dashboard.py
+-rw-r--r--   0 will      (1000) will      (1000)     2801 2023-04-26 18:04:44.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/models.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/scripts/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:22:08.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/scripts/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)      542 2023-04-28 17:25:40.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/scripts/cli.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.780439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/assets/
+-rw-r--r--   0 will      (1000) will      (1000)    95818 2022-05-18 16:59:23.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/assets/Eo_circle_green_checkmark.svg.png
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/css/
+-rw-r--r--   0 will      (1000) will      (1000)       81 2023-04-26 19:56:31.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/css/admin.css
+-rw-r--r--   0 will      (1000) will      (1000)     3365 2022-05-18 16:59:23.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/css/login.css
+-rw-r--r--   0 will      (1000) will      (1000)      364 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/css/main.css
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/js/
+-rw-r--r--   0 will      (1000) will      (1000)     1188 2022-06-21 22:03:38.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/js/codemirror.js
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.780439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/
+-rw-r--r--   0 will      (1000) will      (1000)     1742 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/authorization_status.html
+-rw-r--r--   0 will      (1000) will      (1000)      114 2023-04-26 19:53:07.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/index.html
+-rw-r--r--   0 will      (1000) will      (1000)     2974 2023-04-26 20:01:55.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/logs.html
+-rw-r--r--   0 will      (1000) will      (1000)      275 2023-04-28 16:59:47.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/master.html
+-rw-r--r--   0 will      (1000) will      (1000)     1278 2022-11-16 22:24:00.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/token_edit.html
+-rw-r--r--   0 will      (1000) will      (1000)     1180 2022-11-16 20:50:44.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/tokens.html
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/security/
+-rw-r--r--   0 will      (1000) will      (1000)     2277 2022-11-15 17:26:17.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/security/login.html
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/utilities/
+-rw-r--r--   0 will      (1000) will      (1000)       45 2023-04-27 19:48:38.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/utilities/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     3179 2022-06-15 20:05:15.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/utilities/cache.py
+-rw-r--r--   0 will      (1000) will      (1000)     2230 2022-07-22 00:01:05.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/utilities/jsonhandler.py
+-rw-r--r--   0 will      (1000) will      (1000)      648 2022-12-01 19:01:53.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/utilities/timehandler.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard/views/
+-rw-r--r--   0 will      (1000) will      (1000)        0 2023-04-27 18:35:14.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/views/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     4034 2023-04-26 20:07:54.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/views/auth.py
+-rw-r--r--   0 will      (1000) will      (1000)      843 2023-01-03 17:13:42.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard/views/logs.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/
+-rw-r--r--   0 will      (1000) will      (1000)      517 2023-05-04 19:09:23.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)     1434 2023-05-04 19:09:23.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 19:09:23.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 will      (1000) will      (1000)       65 2023-05-04 19:09:23.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 will      (1000) will      (1000)        1 2023-05-04 18:46:46.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/not-zip-safe
+-rw-r--r--   0 will      (1000) will      (1000)      276 2023-05-04 19:09:23.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/requires.txt
+-rw-r--r--   0 will      (1000) will      (1000)       22 2023-05-04 19:09:23.000000 flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 will      (1000) will      (1000)       38 2023-05-04 19:09:23.790439 flask_admin_dashboard-1.0.7/setup.cfg
+-rw-r--r--   0 will      (1000) will      (1000)     1309 2023-05-04 19:09:11.000000 flask_admin_dashboard-1.0.7/setup.py
```

### Comparing `flask_admin_dashboard-1.0.6/PKG-INFO` & `flask_admin_dashboard-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_admin_dashboard
-Version: 1.0.6
+Version: 1.0.7
 Summary: Admin Dashboard for Flask
 Home-page: https://bitbucket.org/theapiguys/flask_admin_dashboard
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/admin_dashboard.py` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/admin_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,18 @@
         else:
             pw_match = False
             while not pw_match:
                 password = prompt("Password", type=click.STRING, hide_input=False)
                 confirm_pw = prompt("Re-Enter Password", type=click.STRING, hide_input=False)
                 if password == confirm_pw:
                     user_datastore.create_user(username=username, password=password)
-                    user = user_datastore.find_user(username)
+                    user = user_datastore.find_user(username=username)
                     user_datastore.add_role_to_user(user, role)
                     db.session.commit()
+                    pw_match = True
                 else:
                     print("Password did not match.")
 
     if not os.path.exists(LOGS_DIR):
         os.makedirs(LOGS_DIR)
 
     templates_src = Path.joinpath(Path(PACKAGE_DIR), f'templates')
```

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/models.py` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/models.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/scripts/cli.py` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/assets/Eo_circle_green_checkmark.svg.png` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/assets/Eo_circle_green_checkmark.svg.png`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/css/login.css` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/css/login.css`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/static/js/codemirror.js` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/static/js/codemirror.js`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/authorization_status.html` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/authorization_status.html`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/logs.html` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/logs.html`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/token_edit.html` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/token_edit.html`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/admin/tokens.html` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/admin/tokens.html`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/templates/security/login.html` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/templates/security/login.html`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/utilities/cache.py` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/utilities/jsonhandler.py` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/utilities/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/utilities/timehandler.py` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/utilities/timehandler.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/views/auth.py` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/views/auth.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard/views/logs.py` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard/views/logs.py`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/PKG-INFO` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-admin-dashboard
-Version: 1.0.6
+Version: 1.0.7
 Summary: Admin Dashboard for Flask
 Home-page: https://bitbucket.org/theapiguys/flask_admin_dashboard
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flask_admin_dashboard-1.0.6/flask_admin_dashboard.egg-info/SOURCES.txt` & `flask_admin_dashboard-1.0.7/flask_admin_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_admin_dashboard-1.0.6/setup.py` & `flask_admin_dashboard-1.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='flask_admin_dashboard',
-    version='1.0.6',
+    version='1.0.7',
     description='Admin Dashboard for Flask',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/flask_admin_dashboard',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```
