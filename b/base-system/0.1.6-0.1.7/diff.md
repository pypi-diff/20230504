# Comparing `tmp/base_system-0.1.6.tar.gz` & `tmp/base_system-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.1.6.tar", last modified: Thu Apr 27 09:05:45 2023, max compression
+gzip compressed data, was "base_system-0.1.7.tar", last modified: Thu May  4 02:34:12 2023, max compression
```

## Comparing `base_system-0.1.6.tar` & `base_system-0.1.7.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 09:05:45.821392 base_system-0.1.6/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.1.6/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.1.6/.pypirc
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 09:05:45.817390 base_system-0.1.6/BaseFunctionModule/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.1.6/BaseFunctionModule/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.6/BaseFunctionModule/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11888 2023-04-27 08:35:14.000000 base_system-0.1.6/BaseFunctionModule/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.1.6/BaseFunctionModule/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.6/BaseFunctionModule/wsgi.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.1.6/Dockerfile
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.1.6/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.1.6/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-04-27 09:05:45.821392 base_system-0.1.6/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.1.6/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 09:05:45.817390 base_system-0.1.6/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.1.6/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 09:05:45.821392 base_system-0.1.6/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.1.6/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.1.6/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.1.6/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    19403 2023-04-27 03:37:46.000000 base_system-0.1.6/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.1.6/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.1.6/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.1.6/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    32530 2023-04-27 02:23:46.000000 base_system-0.1.6/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11937 2023-04-27 02:23:47.000000 base_system-0.1.6/base_system/__pycache__/viewsets.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.1.6/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.1.6/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.1.6/base_system/auth.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 09:05:45.821392 base_system-0.1.6/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.1.6/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.1.6/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 09:05:45.821392 base_system-0.1.6/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.1.6/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    25401 2023-04-27 03:37:37.000000 base_system-0.1.6/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.1.6/base_system/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.1.6/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.1.6/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    71863 2023-04-27 02:23:42.000000 base_system-0.1.6/base_system/views.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14977 2023-04-25 05:48:42.000000 base_system-0.1.6/base_system/viewsets.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-04-27 09:05:45.817390 base_system-0.1.6/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-04-27 09:05:45.000000 base_system-0.1.6/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1243 2023-04-27 09:05:45.000000 base_system-0.1.6/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-04-27 09:05:45.000000 base_system-0.1.6/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-04-27 03:06:19.000000 base_system-0.1.6/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       82 2023-04-27 09:05:45.000000 base_system-0.1.6/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-04-27 09:05:45.000000 base_system-0.1.6/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.1.6/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.1.6/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.1.6/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.1.6/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-04-27 09:05:45.821392 base_system-0.1.6/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2602 2023-04-27 09:05:09.000000 base_system-0.1.6/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 02:34:12.816119 base_system-0.1.7/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.1.7/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.1.7/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 02:34:12.780099 base_system-0.1.7/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.1.7/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.7/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11870 2023-05-04 02:31:29.000000 base_system-0.1.7/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.1.7/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.7/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.1.7/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.1.7/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.1.7/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 02:34:12.816119 base_system-0.1.7/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.1.7/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 02:34:12.792105 base_system-0.1.7/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.1.7/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 02:34:12.804112 base_system-0.1.7/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.1.7/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.1.7/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.1.7/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19470 2023-05-04 02:30:30.000000 base_system-0.1.7/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.1.7/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.1.7/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.1.7/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    32530 2023-04-27 02:23:46.000000 base_system-0.1.7/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11937 2023-04-27 02:23:47.000000 base_system-0.1.7/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.1.7/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.1.7/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.1.7/base_system/auth.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 02:34:12.816119 base_system-0.1.7/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.1.7/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.1.7/base_system/migrations/0002_drugdirectory_code_medu_cur.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.1.7/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 02:34:12.816119 base_system-0.1.7/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.1.7/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.1.7/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    25505 2023-05-04 01:07:06.000000 base_system-0.1.7/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.1.7/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.1.7/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.1.7/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    71863 2023-04-27 02:23:42.000000 base_system-0.1.7/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    14977 2023-04-25 05:48:42.000000 base_system-0.1.7/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 02:34:12.792105 base_system-0.1.7/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 02:34:12.000000 base_system-0.1.7/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1365 2023-05-04 02:34:12.000000 base_system-0.1.7/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 02:34:12.000000 base_system-0.1.7/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-04-27 03:06:19.000000 base_system-0.1.7/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       82 2023-05-04 02:34:12.000000 base_system-0.1.7/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-04 02:34:12.000000 base_system-0.1.7/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.1.7/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.1.7/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.1.7/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.1.7/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-04 02:34:12.816119 base_system-0.1.7/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2602 2023-05-04 02:32:56.000000 base_system-0.1.7/setup.py
```

### Comparing `base_system-0.1.6/.gitignore` & `base_system-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/BaseFunctionModule/settings.py` & `base_system-0.1.7/BaseFunctionModule/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 
 ALLOWED_HOSTS = ['*']
 
 
 # Application definition
 
 INSTALLED_APPS = [
-    # 'django.contrib.admin',
-    # 'django.contrib.auth',
-    # 'django.contrib.contenttypes',
-    # 'django.contrib.sessions',
-    # 'django.contrib.messages',
-    # 'django.contrib.staticfiles',
-    # 'corsheaders',  # 解决跨域
-    # 'rest_framework',
-    # 'django_filters',
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'corsheaders',  # 解决跨域
+    'rest_framework',
+    'django_filters',
     'base_system',
 ]
 
 MIDDLEWARE = [
     'corsheaders.middleware.CorsMiddleware',  # 跨域问题解决
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
```

### Comparing `base_system-0.1.6/BaseFunctionModule/urls.py` & `base_system-0.1.7/BaseFunctionModule/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/LICENCE` & `base_system-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/PKG-INFO` & `base_system-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base_system
-Version: 0.1.6
+Version: 0.1.7
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.1.6/README.rst` & `base_system-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.1.7/base_system/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 27 03:37:37 2023 UTC, .py size: 25401 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 01ee 4964 3963 0000  a.........Id9c..
+00000000: 610d 0d0a 0000 0000 3a05 5364 a163 0000  a.......:.Sd.c..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ce01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6406 5a0c 4700  d.l.m.Z...d.Z.G.
@@ -851,15 +851,15 @@
 00003520: 0000 4e29 0872 1500 0000 7216 0000 0072  ..N).r....r....r
 00003530: 1700 0000 7205 0000 0072 3900 0000 723e  ....r....r9...r>
 00003540: 0000 005a 0d63 6174 6567 6f72 795f 6e61  ...Z.category_na
 00003550: 6d65 721b 0000 0072 1900 0000 7219 0000  mer....r....r...
 00003560: 0072 1900 0000 721a 0000 0072 b000 0000  .r....r....r....
 00003570: a201 0000 7306 0000 0008 0110 0112 0272  ....s..........r
 00003580: b000 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00003590: 0000 0000 0006 0000 0040 0000 0073 8e01  .........@...s..
+00003590: 0000 0000 0006 0000 0040 0000 0073 9e01  .........@...s..
 000035a0: 0000 6500 5a01 6400 5a02 6503 6a04 6401  ..e.Z.d.Z.e.j.d.
 000035b0: 6402 6403 6404 8d03 5a05 6503 6a04 6405  d.d.d...Z.e.j.d.
 000035c0: 6406 6403 6403 6407 8d04 5a06 6503 6a04  d.d.d.d...Z.e.j.
 000035d0: 6405 6408 6403 6403 6407 8d04 5a07 6503  d.d.d.d.d...Z.e.
 000035e0: 6a04 6405 6409 6403 6403 6407 8d04 5a08  j.d.d.d.d.d...Z.
 000035f0: 6503 6a04 640a 640b 6403 6403 640c 8d04  e.j.d.d.d.d.d...
 00003600: 5a09 6503 6a0a 650b 640d 6503 6a0c 640e  Z.e.j.e.d.e.j.d.
@@ -875,339 +875,343 @@
 000036a0: 8d04 5a17 6503 6a04 6417 640b 6403 6403  ..Z.e.j.d.d.d.d.
 000036b0: 640c 8d04 5a18 6503 6a19 6418 6403 6419  d...Z.e.j.d.d.d.
 000036c0: 8d02 5a1a 6503 6a04 641a 6405 6403 6403  ..Z.e.j.d.d.d.d.
 000036d0: 640c 8d04 5a1b 6503 6a04 641b 6405 6403  d...Z.e.j.d.d.d.
 000036e0: 6403 640c 8d04 5a1c 6503 6a04 641c 6405  d.d...Z.e.j.d.d.
 000036f0: 6403 6403 640c 8d04 5a1d 6503 6a04 6405  d.d.d...Z.e.j.d.
 00003700: 641d 6403 6403 6407 8d04 5a1e 6503 6a04  d.d.d.d...Z.e.j.
-00003710: 6405 641e 6403 6403 6407 8d04 5a1f 4700  d.d.d.d.d...Z.G.
-00003720: 641f 6420 8400 6420 8302 5a20 6421 5300  d.d ..d ..Z d!S.
-00003730: 2922 da0d 4472 7567 4469 7265 6374 6f72  )"..DrugDirector
-00003740: 79f5 0c00 0000 e88d afe5 9381 e7bc 96e7  y...............
-00003750: a081 7223 0000 0054 72ac 0000 0072 5100  ..r#...Tr....rQ.
-00003760: 0000 f50c 0000 00e8 8daf e593 81e5 908d  ................
-00003770: e7a7 b072 7a00 0000 f506 0000 00e8 a784  ...rz...........
-00003780: e6a0 bc75 0c00 0000 e59f bae6 9cac e58d  ...u............
-00003790: 95e4 bd8d 7512 0000 00e6 80bb e987 8fe5  ....u...........
-000037a0: 8d95 e4bd 8de7 bc96 e7a0 8172 5000 0000  ...........rP...
-000037b0: 7228 0000 00f5 0c00 0000 e588 b6e5 8982  r(..............
-000037c0: e7b1 bbe5 9e8b 7248 0000 00f5 0600 0000  ......rH........
-000037d0: e7b1 bbe5 88ab 72ad 0000 0075 0c00 0000  ......r....u....
-000037e0: e58d 95e4 bd8d e589 82e9 878f 7513 0000  ............u...
-000037f0: 00e8 aea1 e987 8f2f e99b b6e5 94ae e58d  ......./........
-00003800: 95e4 bd8d 7512 0000 00e8 aea1 e987 8fe5  ....u...........
-00003810: 8d95 e4bd 8de7 bc96 e7a0 81f5 0c00 0000  ................
-00003820: e5ba 93e5 ad98 e695 b0e9 878f 750c 0000  ............u...
-00003830: 00e5 ba93 e5ad 98e5 8d95 e4bd 8d75 0c00  .............u..
-00003840: 0000 e58c bbe4 bf9d e7b1 bbe5 88ab 750c  ..............u.
-00003850: 0000 00e5 869c e590 88e7 b1bb e588 ab75  ...............u
-00003860: 0f00 0000 e698 afe5 90a6 e698 afe5 9fba  ................
-00003870: e88d af72 1300 0000 750c 0000 00e9 ab98  ...r....u.......
-00003880: e58d b1e7 ad89 e7ba a775 1200 0000 e59b  .........u......
-00003890: bde5 aeb6 e8b4 afe6 a087 e7bc 96e7 a081  ................
-000038a0: 7512 0000 00e5 9bbd e5ae b6e8 b4af e6a0  u...............
-000038b0: 87e5 908d e7a7 b0f5 0600 0000 e4ba a7e5  ................
-000038c0: 9cb0 f50c 0000 00e7 949f e4ba a7e5 8e82  ................
-000038d0: e5ae b663 0000 0000 0000 0000 0000 0000  ...c............
-000038e0: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
-000038f0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-00003900: 0465 045a 0564 0353 0029 047a 1244 7275  .e.Z.d.S.).z.Dru
-00003910: 6744 6972 6563 746f 7279 2e4d 6574 615a  gDirectory.MetaZ
-00003920: 1162 735f 6472 7567 5f64 6972 6563 746f  .bs_drug_directo
-00003930: 7279 750c 0000 00e8 8daf e593 81e7 9bae  ryu.............
-00003940: e5bd 954e 7236 0000 0072 1900 0000 7219  ...Nr6...r....r.
-00003950: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00003960: 0000 cf01 0000 7306 0000 0008 0104 0104  ......s.........
-00003970: 0172 1b00 0000 4e29 2172 1500 0000 7216  .r....N)!r....r.
-00003980: 0000 0072 1700 0000 7205 0000 0072 3900  ...r....r....r9.
-00003990: 0000 da09 6472 7567 5f63 6f64 65da 0964  ....drug_code..d
-000039a0: 7275 675f 6e61 6d65 da09 7374 616e 6461  rug_name..standa
-000039b0: 7264 735a 0a74 6f74 616c 5f75 6e69 745a  rdsZ.total_unitZ
-000039c0: 0f74 6f74 616c 5f75 6e69 745f 636f 6465  .total_unit_code
-000039d0: 7241 0000 0072 a900 0000 da0a 444f 5f4e  rA...r......DO_N
-000039e0: 4f54 4849 4e47 da10 7072 6570 6172 6174  OTHING..preparat
-000039f0: 696f 6e5f 7479 7065 72b0 0000 00da 0863  ion_typer......c
-00003a00: 6174 6567 6f72 7972 ab00 0000 da09 6472  ategoryr......dr
-00003a10: 7567 5f74 7970 655a 0975 6e69 745f 646f  ug_typeZ.unit_do
-00003a20: 7365 5a0c 6d65 6173 7572 655f 756e 6974  seZ.measure_unit
-00003a30: 5a11 6d65 6173 7572 655f 756e 6974 5f63  Z.measure_unit_c
-00003a40: 6f64 655a 0a73 746f 636b 5f6c 6566 745a  odeZ.stock_leftZ
-00003a50: 0a73 746f 636b 5f75 6e69 745a 036d 6963  .stock_unitZ.mic
-00003a60: 5a0c 7263 635f 6361 7465 676f 7279 721f  Z.rcc_categoryr.
-00003a70: 0000 005a 0c69 735f 6573 7365 6e74 6961  ...Z.is_essentia
-00003a80: 6c5a 0868 725f 6c65 7665 6c5a 0767 625f  lZ.hr_levelZ.gb_
-00003a90: 636f 6465 5a07 6762 5f6e 616d 65da 0c6f  codeZ.gb_name..o
-00003aa0: 7269 6769 6e5f 706c 6163 65da 0c6d 616e  rigin_place..man
-00003ab0: 7566 6163 7475 7265 7272 1b00 0000 7219  ufacturerr....r.
-00003ac0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00003ad0: 0000 72b1 0000 00ac 0100 0073 4400 0000  ..r........sD...
-00003ae0: 0801 1001 1201 1201 1201 1201 0401 0201  ................
-00003af0: 0201 04fd 0605 0401 0201 0201 04fd 0605  ................
-00003b00: 0401 0201 0201 04fd 0605 1201 1201 1201  ................
-00003b10: 1201 1201 1201 1201 0e01 1201 1201 1201  ................
-00003b20: 1201 1202 72b1 0000 0063 0000 0000 0000  ....r....c......
-00003b30: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
-00003b40: 0000 733c 0000 0065 005a 0164 005a 0265  ..s<...e.Z.d.Z.e
-00003b50: 036a 0464 0164 0264 0364 048d 035a 0565  .j.d.d.d.d...Z.e
-00003b60: 036a 0464 0564 0664 0364 0364 078d 045a  .j.d.d.d.d.d...Z
-00003b70: 0647 0064 0864 0984 0064 0983 025a 0764  .G.d.d...d...Z.d
-00003b80: 0a53 0029 0bda 0c50 6861 726d 6163 7954  .S.)...PharmacyT
-00003b90: 7970 6572 2b00 0000 7223 0000 0054 72ac  yper+...r#...Tr.
-00003ba0: 0000 0072 2200 0000 7251 0000 0072 2800  ...r"...rQ...r(.
-00003bb0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00003bc0: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
-00003bd0: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-00003be0: 6504 5a05 6403 5300 2904 7a11 5068 6172  e.Z.d.S.).z.Phar
-00003bf0: 6d61 6379 5479 7065 2e4d 6574 615a 1062  macyType.MetaZ.b
-00003c00: 735f 7068 6172 6d61 6379 5f74 7970 65f5  s_pharmacy_type.
-00003c10: 0c00 0000 e88d afe6 88bf e7b1 bbe5 9e8b  ................
-00003c20: 4e72 3600 0000 7219 0000 0072 1900 0000  Nr6...r....r....
-00003c30: 7219 0000 0072 1a00 0000 721b 0000 00d9  r....r....r.....
-00003c40: 0100 0073 0600 0000 0801 0401 0401 721b  ...s..........r.
-00003c50: 0000 004e 72ae 0000 0072 1900 0000 7219  ...Nr....r....r.
-00003c60: 0000 0072 1900 0000 721a 0000 0072 c300  ...r....r....r..
-00003c70: 0000 d501 0000 7306 0000 0008 0110 0112  ......s.........
-00003c80: 0272 c300 0000 6300 0000 0000 0000 0000  .r....c.........
-00003c90: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
-00003ca0: 3c00 0000 6500 5a01 6400 5a02 6503 6a04  <...e.Z.d.Z.e.j.
-00003cb0: 6401 6402 6403 6404 8d03 5a05 6503 6a04  d.d.d.d...Z.e.j.
-00003cc0: 6405 6406 6403 6403 6407 8d04 5a06 4700  d.d.d.d.d...Z.G.
-00003cd0: 6408 6409 8400 6409 8302 5a07 640a 5300  d.d...d...Z.d.S.
-00003ce0: 290b da12 5068 6172 6d61 6379 456e 7465  )...PharmacyEnte
-00003cf0: 7270 7269 7365 722b 0000 0072 2300 0000  rpriser+...r#...
-00003d00: 5472 ac00 0000 7222 0000 0072 5100 0000  Tr....r"...rQ...
-00003d10: 7228 0000 0063 0000 0000 0000 0000 0000  r(...c..........
-00003d20: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
-00003d30: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00003d40: 025a 0465 045a 0564 0353 0029 047a 1750  .Z.e.Z.d.S.).z.P
-00003d50: 6861 726d 6163 7945 6e74 6572 7072 6973  harmacyEnterpris
-00003d60: 652e 4d65 7461 5a16 6273 5f70 6861 726d  e.MetaZ.bs_pharm
-00003d70: 6163 795f 656e 7465 7270 7269 7365 750c  acy_enterpriseu.
-00003d80: 0000 00e8 8daf e4bc 81e7 aea1 e790 864e  ...............N
-00003d90: 7236 0000 0072 1900 0000 7219 0000 0072  r6...r....r....r
-00003da0: 1900 0000 721a 0000 0072 1b00 0000 e301  ....r....r......
-00003db0: 0000 7306 0000 0008 0104 0104 0172 1b00  ..s..........r..
-00003dc0: 0000 4e72 ae00 0000 7219 0000 0072 1900  ..Nr....r....r..
-00003dd0: 0000 7219 0000 0072 1a00 0000 72c5 0000  ..r....r....r...
-00003de0: 00df 0100 0073 0600 0000 0801 1001 1202  .....s..........
-00003df0: 72c5 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00003e00: 0000 0000 0000 0600 0000 4000 0000 7386  ..........@...s.
-00003e10: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
-00003e20: 0164 0264 0364 048d 035a 0565 036a 0464  .d.d.d...Z.e.j.d
-00003e30: 0564 0664 0364 0364 078d 045a 0665 036a  .d.d.d.d...Z.e.j
-00003e40: 0765 0864 0865 036a 0964 098d 035a 0a65  .e.d.e.j.d...Z.e
-00003e50: 036a 0b64 0a64 0364 0364 0b8d 035a 0c65  .j.d.d.d.d...Z.e
-00003e60: 036a 0765 0d64 0c65 036a 0e64 0364 0d8d  .j.e.d.e.j.d.d..
-00003e70: 045a 0f65 036a 0765 1064 0e65 036a 0e64  .Z.e.j.e.d.e.j.d
-00003e80: 0364 0d8d 045a 1147 0064 0f64 1084 0064  .d...Z.G.d.d...d
-00003e90: 1083 025a 1264 1153 0029 12da 1250 6861  ...Z.d.S.)...Pha
-00003ea0: 726d 6163 794d 616e 6167 656d 656e 7475  rmacyManagementu
-00003eb0: 0c00 0000 e88d afe6 88bf e7bc 96e7 a081  ................
-00003ec0: 7223 0000 0054 72ac 0000 0075 0c00 0000  r#...Tr....u....
-00003ed0: e88d afe6 88bf e590 8de7 a7b0 7251 0000  ............rQ..
-00003ee0: 0072 2800 0000 72c4 0000 0072 4800 0000  .r(...r....rH...
-00003ef0: 750c 0000 00e8 8daf e688 bfe5 9cb0 e59d  u...............
-00003f00: 8072 2a00 0000 722f 0000 0072 3000 0000  .r*...r/...r0...
-00003f10: 750c 0000 00e6 8980 e5b1 9ee8 8daf e4bc  u...............
-00003f20: 8163 0000 0000 0000 0000 0000 0000 0000  .c..............
-00003f30: 0000 0100 0000 4000 0000 7318 0000 0065  ......@...s....e
-00003f40: 005a 0164 005a 0264 015a 0364 025a 0465  .Z.d.Z.d.Z.d.Z.e
-00003f50: 045a 0564 0353 0029 047a 1750 6861 726d  .Z.d.S.).z.Pharm
-00003f60: 6163 794d 616e 6167 656d 656e 742e 4d65  acyManagement.Me
-00003f70: 7461 5a16 6273 5f70 6861 726d 6163 795f  taZ.bs_pharmacy_
-00003f80: 6d61 6e61 6765 6d65 6e74 750c 0000 00e8  managementu.....
-00003f90: 8daf e688 bfe7 aea1 e790 864e 7236 0000  ...........Nr6..
-00003fa0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
-00003fb0: 721a 0000 0072 1b00 0000 f501 0000 7306  r....r........s.
-00003fc0: 0000 0008 0104 0104 0172 1b00 0000 4e29  .........r....N)
-00003fd0: 1372 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
-00003fe0: 7205 0000 0072 3900 0000 5a0d 7068 6172  r....r9...Z.phar
-00003ff0: 6d61 6379 5f63 6f64 655a 0d70 6861 726d  macy_codeZ.pharm
-00004000: 6163 795f 6e61 6d65 7241 0000 0072 c300  acy_namerA...r..
-00004010: 0000 72bd 0000 005a 0d70 6861 726d 6163  ..r....Z.pharmac
-00004020: 795f 7479 7065 723c 0000 0072 3f00 0000  y_typer<...r?...
-00004030: 7221 0000 0072 4200 0000 724a 0000 0072  r!...rB...rJ...r
-00004040: c500 0000 5a0a 656e 7465 7270 7269 7365  ....Z.enterprise
-00004050: 721b 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00004060: 1900 0000 721a 0000 0072 c600 0000 e901  ....r....r......
-00004070: 0000 7316 0000 0008 0110 0112 0104 0102  ..s.............
-00004080: 0102 0104 fd06 0510 0114 0114 0272 c600  .............r..
-00004090: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000040a0: 0000 0006 0000 0040 0000 0073 4e01 0000  .......@...sN...
-000040b0: 6500 5a01 6400 5a02 6503 6a04 6505 6401  e.Z.d.Z.e.j.e.d.
-000040c0: 6503 6a06 6402 6403 8d04 5a07 6503 6a08  e.j.d.d...Z.e.j.
-000040d0: 6404 6405 6402 6402 6406 8d04 5a09 6503  d.d.d.d.d...Z.e.
-000040e0: 6a08 6407 6408 6402 6402 6409 8d04 5a0a  j.d.d.d.d.d...Z.
-000040f0: 6503 6a08 6407 640a 6402 6402 6409 8d04  e.j.d.d.d.d.d...
-00004100: 5a0b 6503 6a08 6407 640b 6402 6402 6409  Z.e.j.d.d.d.d.d.
-00004110: 8d04 5a0c 6503 6a04 650d 640c 6503 6a0e  ..Z.e.j.e.d.e.j.
-00004120: 640d 8d03 5a0f 6503 6a04 6510 640e 6503  d...Z.e.j.e.d.e.
-00004130: 6a0e 640d 8d03 5a11 6503 6a04 6512 640f  j.d...Z.e.j.e.d.
-00004140: 6503 6a0e 640d 8d03 5a13 6503 6a08 6410  e.j.d...Z.e.j.d.
-00004150: 6411 6402 6402 6409 8d04 5a14 6503 6a08  d.d.d.d...Z.e.j.
-00004160: 6412 6413 6402 6402 6409 8d04 5a15 6503  d.d.d.d.d...Z.e.
-00004170: 6a04 6516 6414 6503 6a06 6402 6403 8d04  j.e.d.e.j.d.d...
-00004180: 5a17 6503 6a18 6415 6402 6402 6416 8d03  Z.e.j.d.d.d.d...
-00004190: 5a19 6503 6a1a 6417 6418 6402 6419 8d03  Z.e.j.d.d.d.d...
-000041a0: 5a1b 6503 6a08 6407 641a 6402 6402 6409  Z.e.j.d.d.d.d.d.
-000041b0: 8d04 5a1c 6503 6a1d 641b 6402 641c 8d02  ..Z.e.j.d.d.d...
-000041c0: 5a1e 6503 6a1d 641d 6402 641c 8d02 5a1f  Z.e.j.d.d.d...Z.
-000041d0: 6503 6a1d 641e 6402 641c 8d02 5a20 6503  e.j.d.d.d...Z e.
-000041e0: 6a1d 641f 6402 641c 8d02 5a21 4700 6420  j.d.d.d...Z!G.d 
-000041f0: 6421 8400 6421 8302 5a22 6422 5300 2923  d!..d!..Z"d"S.)#
-00004200: da0c 5068 6172 6d61 6379 4472 7567 750c  ..PharmacyDrugu.
-00004210: 0000 00e6 8980 e5b1 9ee8 8daf e688 bf54  ...............T
-00004220: 7230 0000 0072 b200 0000 7223 0000 0072  r0...r....r#...r
-00004230: 2800 0000 7251 0000 0072 b300 0000 727a  (...rQ...r....rz
-00004240: 0000 0072 b400 0000 7506 0000 00e5 8d95  ...r....u.......
-00004250: e4bd 8d72 b500 0000 7248 0000 0072 ad00  ...r....rH...r..
-00004260: 0000 72b6 0000 0072 8000 0000 72b8 0000  ..r....r....r...
-00004270: 00e9 c800 0000 72b9 0000 0072 2f00 0000  ......r....r/...
-00004280: 750c 0000 00e6 9c89 e695 88e6 97a5 e69c  u...............
-00004290: 9f72 1000 0000 72b7 0000 0072 0100 0000  .r....r....r....
-000042a0: 7279 0000 0075 0c00 0000 e8ae a1e9 878f  ry...u..........
-000042b0: e58d 95e4 bd8d 750c 0000 00e6 8890 e69c  ......u.........
-000042c0: ace5 8d95 e4bb b772 8f00 0000 750c 0000  .......r....u...
-000042d0: 00e6 8890 e69c ace9 8791 e9a2 9d75 0c00  .............u..
-000042e0: 0000 e99b b6e5 94ae e58d 95e4 bbb7 750c  ..............u.
-000042f0: 0000 00e9 9bb6 e594 aee9 8791 e9a2 9d63  ...............c
-00004300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004310: 0100 0000 4000 0000 7318 0000 0065 005a  ....@...s....e.Z
-00004320: 0164 005a 0264 015a 0364 025a 0465 045a  .d.Z.d.Z.d.Z.e.Z
-00004330: 0564 0353 0029 047a 1150 6861 726d 6163  .d.S.).z.Pharmac
-00004340: 7944 7275 672e 4d65 7461 5a10 6273 5f70  yDrug.MetaZ.bs_p
-00004350: 6861 726d 6163 795f 6472 7567 750d 0000  harmacy_drugu...
-00004360: 00e8 8daf e688 bf2d e88d afe5 9381 4e72  .......-......Nr
-00004370: 3600 0000 7219 0000 0072 1900 0000 7219  6...r....r....r.
-00004380: 0000 0072 1a00 0000 721b 0000 001b 0200  ...r....r.......
-00004390: 0073 0600 0000 0801 0401 0401 721b 0000  .s..........r...
-000043a0: 004e 2923 7215 0000 0072 1600 0000 7217  .N)#r....r....r.
-000043b0: 0000 0072 0500 0000 7241 0000 0072 c600  ...r....rA...r..
-000043c0: 0000 7242 0000 005a 0870 6861 726d 6163  ..rB...Z.pharmac
-000043d0: 7972 3900 0000 72ba 0000 0072 bb00 0000  yr9...r....r....
-000043e0: 72bc 0000 00da 0575 6e69 7473 72a9 0000  r......unitsr...
-000043f0: 0072 bd00 0000 72be 0000 0072 ab00 0000  .r....r....r....
-00004400: 72c0 0000 0072 b000 0000 72bf 0000 0072  r....r....r....r
-00004410: c100 0000 72c2 0000 0072 2100 0000 724a  ....r....r!...rJ
-00004420: 0000 0072 5f00 0000 5a0a 7661 6c69 645f  ...r_...Z.valid_
-00004430: 6461 7465 726f 0000 005a 1269 6e76 656e  datero...Z.inven
-00004440: 746f 7279 5f71 7561 6e74 6974 795a 106d  tory_quantityZ.m
-00004450: 6561 7375 7265 6d65 6e74 5f75 6e69 7472  easurement_unitr
-00004460: 4000 0000 5a0f 636f 7374 5f75 6e69 745f  @...Z.cost_unit_
-00004470: 7072 6963 655a 0b63 6f73 745f 616d 6f75  priceZ.cost_amou
-00004480: 6e74 5a11 7265 7461 696c 5f75 6e69 745f  ntZ.retail_unit_
-00004490: 7072 6963 655a 0d72 6574 6169 6c5f 616d  priceZ.retail_am
-000044a0: 6f75 6e74 721b 0000 0072 1900 0000 7219  ountr....r....r.
-000044b0: 0000 0072 1900 0000 721a 0000 0072 c700  ...r....r....r..
-000044c0: 0000 fb01 0000 733e 0000 0008 0114 0112  ......s>........
-000044d0: 0112 0112 0112 0104 0102 0102 0104 fd06  ................
-000044e0: 0504 0102 0102 0104 fd06 0504 0102 0102  ................
-000044f0: 0104 fd06 0512 0112 0114 0110 0110 0112  ................
-00004500: 010e 010e 010e 010e 0272 c700 0000 6300  .........r....c.
-00004510: 0000 0000 0000 0000 0000 0000 0000 0006  ................
-00004520: 0000 0040 0000 0073 b600 0000 6500 5a01  ...@...s....e.Z.
-00004530: 6400 5a02 6503 6a04 6401 6402 6403 8d02  d.Z.e.j.d.d.d...
-00004540: 5a05 6503 6a04 6401 6404 6403 8d02 5a06  Z.e.j.d.d.d...Z.
-00004550: 6503 6a04 6401 6405 6406 6406 6407 8d04  e.j.d.d.d.d.d...
-00004560: 5a07 6503 6a04 6401 6408 6403 8d02 5a08  Z.e.j.d.d.d...Z.
-00004570: 6503 6a04 6401 6409 6403 8d02 5a09 6503  e.j.d.d.d...Z.e.
-00004580: 6a04 640a 640b 6403 8d02 5a0a 6503 6a04  j.d.d.d...Z.e.j.
-00004590: 640a 640c 6403 8d02 5a0b 6503 6a0c 640d  d.d.d...Z.e.j.d.
-000045a0: 6406 6406 640e 8d03 5a0d 6503 6a0c 640f  d.d.d...Z.e.j.d.
-000045b0: 6406 6406 6410 8d03 5a0e 6503 6a0f 6411  d.d.d...Z.e.j.d.
-000045c0: 6406 6412 8d02 5a10 4700 6413 6414 8400  d.d...Z.G.d.d...
-000045d0: 6414 8302 5a11 6415 6416 8400 5a12 6417  d...Z.d.d...Z.d.
-000045e0: 5300 2918 da07 4170 6949 6e66 6f72 7600  S.)...ApiInforv.
-000045f0: 0000 72a1 0000 0072 7700 0000 750c 0000  ..r....rw...u...
-00004600: 00e8 afb7 e6b1 82e7 bc96 e7a0 8175 0c00  .............u..
-00004610: 0000 e8af b7e6 b182 e590 8de7 a7b0 5472  ..............Tr
-00004620: 7a00 0000 750c 0000 00e8 afb7 e6b1 82e6  z...u...........
-00004630: 96b9 e5bc 8f75 1200 0000 e8af b7e6 b182  .....u..........
-00004640: e695 b0e6 8dae e7b1 bbe5 9e8b 72c8 0000  ............r...
-00004650: 0075 1100 0000 6970 e59c b0e5 9d80 e688  .u....ip........
-00004660: 96e5 9f9f e590 8d75 0c00 0000 e8af b7e6  .......u........
-00004670: b182 e8b7 afe7 94b1 720a 0000 0072 0b00  ........r....r..
-00004680: 0000 720f 0000 0072 1000 0000 7212 0000  ..r....r....r...
-00004690: 0072 1300 0000 6300 0000 0000 0000 0000  .r....c.........
-000046a0: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-000046b0: 1c00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-000046c0: 6402 5a04 6504 5a05 6403 5a06 6404 5300  d.Z.e.Z.d.Z.d.S.
-000046d0: 2905 7a0c 4170 6949 6e66 6f2e 4d65 7461  ).z.ApiInfo.Meta
-000046e0: 5a0b 6273 5f61 7069 5f69 6e66 6f75 0c00  Z.bs_api_infou..
-000046f0: 0000 e68e a5e5 8fa3 e4bf a1e6 81af 2901  ..............).
-00004700: a902 da08 6f72 675f 636f 6465 da08 7265  ....org_code..re
-00004710: 715f 636f 6465 4e72 4b00 0000 7219 0000  q_codeNrK...r...
-00004720: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00004730: 721b 0000 002d 0200 0073 0800 0000 0801  r....-...s......
-00004740: 0401 0401 0401 721b 0000 0063 0300 0000  ......r....c....
-00004750: 0000 0000 0000 0000 0700 0000 0500 0000  ................
-00004760: 4300 0000 73ba 0000 0074 006a 016a 027c  C...s....t.j.j.|
-00004770: 0164 0119 007c 0264 028d 02a0 03a1 007d  .d...|.d.......}
-00004780: 037c 0372 a87c 036a 047c 036a 0517 007d  .|.r.|.j.|.j...}
-00004790: 047c 036a 0664 036b 0272 4274 076a 087c  .|.j.d.k.rBt.j.|
-000047a0: 047c 0164 048d 027d 056e 587c 036a 0664  .|.d...}.nX|.j.d
-000047b0: 056b 0272 5c74 076a 097c 047c 0164 068d  .k.r\t.j.|.|.d..
-000047c0: 027d 056e 3e7c 036a 0664 076b 0272 7674  .}.n>|.j.d.k.rvt
-000047d0: 076a 0a7c 047c 0164 088d 027d 056e 247c  .j.|.|.d...}.n$|
-000047e0: 036a 0664 096b 0272 8e74 076a 0b7c 0464  .j.d.k.r.t.j.|.d
-000047f0: 0a8d 017d 056e 0c74 076a 0c7c 0464 0a8d  ...}.n.t.j.|.d..
-00004800: 017d 0574 0da0 0e7c 056a 0fa1 017d 066e  .}.t...|.j...}.n
-00004810: 0e64 0b64 0c64 0d69 0064 0e9c 047d 067c  .d.d.d.i.d...}.|
-00004820: 0653 0029 0f4e 72a6 0000 0072 cb00 0000  .S.).Nr....r....
-00004830: da04 504f 5354 2902 728d 0000 00da 046a  ..POST).r......j
-00004840: 736f 6eda 0347 4554 2902 728d 0000 00da  son..GET).r.....
-00004850: 0670 6172 616d 73da 0350 5554 2902 728d  .params..PUT).r.
-00004860: 0000 00da 0464 6174 61da 0644 454c 4554  .....data..DELET
-00004870: 4529 0172 8d00 0000 4669 d107 0000 751e  E).r....Fi....u.
-00004880: 0000 00e4 b88d e5ad 98e5 9ca8 e5af b9e6  ................
-00004890: 8ea5 e58c bbe9 99a2 e4bf a1e6 81af efbc  ................
-000048a0: 8129 04da 0773 7563 6365 7373 72af 0000  .)...successr...
-000048b0: 00da 076d 6573 7361 6765 72d3 0000 0029  ...messager....)
-000048c0: 1072 ca00 0000 da07 6f62 6a65 6374 73da  .r......objects.
-000048d0: 0666 696c 7465 7272 6700 0000 da09 6970  .filterrg.....ip
-000048e0: 5f64 6f6d 6169 6e72 9100 0000 da0a 7265  _domainr......re
-000048f0: 715f 6d65 7468 6f64 da08 7265 7175 6573  q_method..reques
-00004900: 7473 da04 706f 7374 da03 6765 74da 0370  ts..post..get..p
-00004910: 7574 da06 6465 6c65 7465 da05 7061 7463  ut..delete..patc
-00004920: 6872 cf00 0000 da05 6c6f 6164 73da 0474  hr......loads..t
-00004930: 6578 7429 0772 2e00 0000 5a07 696e 5f64  ext).r....Z.in_d
-00004940: 6174 6172 cd00 0000 5a0c 6170 695f 696e  atar....Z.api_in
-00004950: 666f 5f6f 626a 5a07 636d 735f 7572 6cda  fo_objZ.cms_url.
-00004960: 0372 6573 5a08 7265 735f 6a73 6f6e 7219  .resZ.res_jsonr.
-00004970: 0000 0072 1900 0000 721a 0000 00da 0977  ...r....r......w
-00004980: 7269 7465 6261 636b 3502 0000 731e 0000  riteback5...s...
-00004990: 0000 0118 0104 010c 010a 0110 010a 0110  ................
-000049a0: 010a 0110 010a 010e 020c 010e 020e 017a  ...............z
-000049b0: 1141 7069 496e 666f 2e77 7269 7465 6261  .ApiInfo.writeba
-000049c0: 636b 4e29 1372 1500 0000 7216 0000 0072  ckN).r....r....r
-000049d0: 1700 0000 7205 0000 0072 3900 0000 72cc  ....r....r9...r.
-000049e0: 0000 0072 cd00 0000 5a08 7265 715f 6e61  ...r....Z.req_na
-000049f0: 6d65 72da 0000 0072 9000 0000 72d9 0000  mer....r....r...
-00004a00: 0072 9100 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00004a10: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-00004a20: 1b00 0000 72e4 0000 0072 1900 0000 7219  ....r....r....r.
-00004a30: 0000 0072 1900 0000 721a 0000 0072 ca00  ...r....r....r..
-00004a40: 0000 2102 0000 7318 0000 0008 010e 010e  ..!...s.........
-00004a50: 0112 010e 010e 010e 010e 0110 0110 010e  ................
-00004a60: 020e 0872 ca00 0000 2925 72cf 0000 00da  ...r....)%r.....
-00004a70: 026f 7372 db00 0000 da1a 646a 616e 676f  .osr......django
-00004a80: 2e63 6f6e 7472 6962 2e61 7574 682e 6d6f  .contrib.auth.mo
-00004a90: 6465 6c73 7202 0000 0072 0300 0000 da22  delsr....r....."
-00004aa0: 646a 616e 676f 2e63 6f6e 7472 6962 2e63  django.contrib.c
-00004ab0: 6f6e 7465 6e74 7479 7065 732e 6d6f 6465  ontenttypes.mode
-00004ac0: 6c73 7204 0000 00da 0964 6a61 6e67 6f2e  lsr......django.
-00004ad0: 6462 7205 0000 00da 0b64 6a61 6e67 6f2e  dbr......django.
-00004ae0: 636f 6e66 7206 0000 0072 5c00 0000 da05  confr....r\.....
-00004af0: 4d6f 6465 6c72 0900 0000 7221 0000 0072  Modelr....r!...r
-00004b00: 4600 0000 724d 0000 0072 4f00 0000 7262  F...rM...rO...rb
-00004b10: 0000 0072 7300 0000 727e 0000 0072 8b00  ...rs...r~...r..
-00004b20: 0000 7293 0000 0072 9600 0000 729d 0000  ..r....r....r...
-00004b30: 0072 a700 0000 72a8 0000 0072 a900 0000  .r....r....r....
-00004b40: 72ab 0000 0072 b000 0000 72b1 0000 0072  r....r....r....r
-00004b50: c300 0000 72c5 0000 0072 c600 0000 72c7  ....r....r....r.
-00004b60: 0000 0072 ca00 0000 7219 0000 0072 1900  ...r....r....r..
-00004b70: 0000 7219 0000 0072 1a00 0000 da08 3c6d  ..r....r......<m
-00004b80: 6f64 756c 653e 0100 0000 733c 0000 0008  odule>....s<....
-00004b90: 0108 0208 0110 010c 010c 010c 0204 0612  ................
-00004ba0: 0910 1e10 1c10 1410 2810 4a12 1a12 1b12  ........(.J.....
-00004bb0: 2310 1910 1110 1110 1110 1110 0a10 0a10  #...............
-00004bc0: 0a10 2910 0a10 0a10 1210 26              ..).......&
+00003710: 6405 641e 6403 6403 6407 8d04 5a1f 6503  d.d.d.d.d...Z.e.
+00003720: 6a04 641f 6405 6403 6420 8d03 5a20 4700  j.d.d.d.d ..Z G.
+00003730: 6421 6422 8400 6422 8302 5a21 6423 5300  d!d"..d"..Z!d#S.
+00003740: 2924 da0d 4472 7567 4469 7265 6374 6f72  )$..DrugDirector
+00003750: 79f5 0c00 0000 e88d afe5 9381 e7bc 96e7  y...............
+00003760: a081 7223 0000 0054 72ac 0000 0072 5100  ..r#...Tr....rQ.
+00003770: 0000 f50c 0000 00e8 8daf e593 81e5 908d  ................
+00003780: e7a7 b072 7a00 0000 f506 0000 00e8 a784  ...rz...........
+00003790: e6a0 bc75 0c00 0000 e59f bae6 9cac e58d  ...u............
+000037a0: 95e4 bd8d 7512 0000 00e6 80bb e987 8fe5  ....u...........
+000037b0: 8d95 e4bd 8de7 bc96 e7a0 8172 5000 0000  ...........rP...
+000037c0: 7228 0000 00f5 0c00 0000 e588 b6e5 8982  r(..............
+000037d0: e7b1 bbe5 9e8b 7248 0000 00f5 0600 0000  ......rH........
+000037e0: e7b1 bbe5 88ab 72ad 0000 0075 0c00 0000  ......r....u....
+000037f0: e58d 95e4 bd8d e589 82e9 878f 7513 0000  ............u...
+00003800: 00e8 aea1 e987 8f2f e99b b6e5 94ae e58d  ......./........
+00003810: 95e4 bd8d 7512 0000 00e8 aea1 e987 8fe5  ....u...........
+00003820: 8d95 e4bd 8de7 bc96 e7a0 81f5 0c00 0000  ................
+00003830: e5ba 93e5 ad98 e695 b0e9 878f 750c 0000  ............u...
+00003840: 00e5 ba93 e5ad 98e5 8d95 e4bd 8d75 0c00  .............u..
+00003850: 0000 e58c bbe4 bf9d e7b1 bbe5 88ab 750c  ..............u.
+00003860: 0000 00e5 869c e590 88e7 b1bb e588 ab75  ...............u
+00003870: 0f00 0000 e698 afe5 90a6 e698 afe5 9fba  ................
+00003880: e88d af72 1300 0000 750c 0000 00e9 ab98  ...r....u.......
+00003890: e58d b1e7 ad89 e7ba a775 1200 0000 e59b  .........u......
+000038a0: bde5 aeb6 e8b4 afe6 a087 e7bc 96e7 a081  ................
+000038b0: 7512 0000 00e5 9bbd e5ae b6e8 b4af e6a0  u...............
+000038c0: 87e5 908d e7a7 b0f5 0600 0000 e4ba a7e5  ................
+000038d0: 9cb0 f50c 0000 00e7 949f e4ba a7e5 8e82  ................
+000038e0: e5ae b675 1800 0000 e58d 95e6 aca1 e794  ...u............
+000038f0: a8e9 878f e58d 95e4 bd8d e7bc 96e7 a081  ................
+00003900: 728e 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00003910: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
+00003920: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00003930: 025a 0465 045a 0564 0353 0029 047a 1244  .Z.e.Z.d.S.).z.D
+00003940: 7275 6744 6972 6563 746f 7279 2e4d 6574  rugDirectory.Met
+00003950: 615a 1162 735f 6472 7567 5f64 6972 6563  aZ.bs_drug_direc
+00003960: 746f 7279 750c 0000 00e8 8daf e593 81e7  toryu...........
+00003970: 9bae e5bd 954e 7236 0000 0072 1900 0000  .....Nr6...r....
+00003980: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00003990: 1b00 0000 d001 0000 7306 0000 0008 0104  ........s.......
+000039a0: 0104 0172 1b00 0000 4e29 2272 1500 0000  ...r....N)"r....
+000039b0: 7216 0000 0072 1700 0000 7205 0000 0072  r....r....r....r
+000039c0: 3900 0000 da09 6472 7567 5f63 6f64 65da  9.....drug_code.
+000039d0: 0964 7275 675f 6e61 6d65 da09 7374 616e  .drug_name..stan
+000039e0: 6461 7264 735a 0a74 6f74 616c 5f75 6e69  dardsZ.total_uni
+000039f0: 745a 0f74 6f74 616c 5f75 6e69 745f 636f  tZ.total_unit_co
+00003a00: 6465 7241 0000 0072 a900 0000 da0a 444f  derA...r......DO
+00003a10: 5f4e 4f54 4849 4e47 da10 7072 6570 6172  _NOTHING..prepar
+00003a20: 6174 696f 6e5f 7479 7065 72b0 0000 00da  ation_typer.....
+00003a30: 0863 6174 6567 6f72 7972 ab00 0000 da09  .categoryr......
+00003a40: 6472 7567 5f74 7970 655a 0975 6e69 745f  drug_typeZ.unit_
+00003a50: 646f 7365 5a0c 6d65 6173 7572 655f 756e  doseZ.measure_un
+00003a60: 6974 5a11 6d65 6173 7572 655f 756e 6974  itZ.measure_unit
+00003a70: 5f63 6f64 655a 0a73 746f 636b 5f6c 6566  _codeZ.stock_lef
+00003a80: 745a 0a73 746f 636b 5f75 6e69 745a 036d  tZ.stock_unitZ.m
+00003a90: 6963 5a0c 7263 635f 6361 7465 676f 7279  icZ.rcc_category
+00003aa0: 721f 0000 005a 0c69 735f 6573 7365 6e74  r....Z.is_essent
+00003ab0: 6961 6c5a 0868 725f 6c65 7665 6c5a 0767  ialZ.hr_levelZ.g
+00003ac0: 625f 636f 6465 5a07 6762 5f6e 616d 65da  b_codeZ.gb_name.
+00003ad0: 0c6f 7269 6769 6e5f 706c 6163 65da 0c6d  .origin_place..m
+00003ae0: 616e 7566 6163 7475 7265 725a 0d63 6f64  anufacturerZ.cod
+00003af0: 655f 6d65 6475 5f63 7572 721b 0000 0072  e_medu_curr....r
+00003b00: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+00003b10: 0000 0072 b100 0000 ac01 0000 7346 0000  ...r........sF..
+00003b20: 0008 0110 0112 0112 0112 0112 0104 0102  ................
+00003b30: 0102 0104 fd06 0504 0102 0102 0104 fd06  ................
+00003b40: 0504 0102 0102 0104 fd06 0512 0112 0112  ................
+00003b50: 0112 0112 0112 0112 010e 0112 0112 0112  ................
+00003b60: 0112 0112 0110 0272 b100 0000 6300 0000  .......r....c...
+00003b70: 0000 0000 0000 0000 0000 0000 0006 0000  ................
+00003b80: 0040 0000 0073 3c00 0000 6500 5a01 6400  .@...s<...e.Z.d.
+00003b90: 5a02 6503 6a04 6401 6402 6403 6404 8d03  Z.e.j.d.d.d.d...
+00003ba0: 5a05 6503 6a04 6405 6406 6403 6403 6407  Z.e.j.d.d.d.d.d.
+00003bb0: 8d04 5a06 4700 6408 6409 8400 6409 8302  ..Z.G.d.d...d...
+00003bc0: 5a07 640a 5300 290b da0c 5068 6172 6d61  Z.d.S.)...Pharma
+00003bd0: 6379 5479 7065 722b 0000 0072 2300 0000  cyTyper+...r#...
+00003be0: 5472 ac00 0000 7222 0000 0072 5100 0000  Tr....r"...rQ...
+00003bf0: 7228 0000 0063 0000 0000 0000 0000 0000  r(...c..........
+00003c00: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
+00003c10: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00003c20: 025a 0465 045a 0564 0353 0029 047a 1150  .Z.e.Z.d.S.).z.P
+00003c30: 6861 726d 6163 7954 7970 652e 4d65 7461  harmacyType.Meta
+00003c40: 5a10 6273 5f70 6861 726d 6163 795f 7479  Z.bs_pharmacy_ty
+00003c50: 7065 f50c 0000 00e8 8daf e688 bfe7 b1bb  pe..............
+00003c60: e59e 8b4e 7236 0000 0072 1900 0000 7219  ...Nr6...r....r.
+00003c70: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+00003c80: 0000 da01 0000 7306 0000 0008 0104 0104  ......s.........
+00003c90: 0172 1b00 0000 4e72 ae00 0000 7219 0000  .r....Nr....r...
+00003ca0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00003cb0: 72c3 0000 00d6 0100 0073 0600 0000 0801  r........s......
+00003cc0: 1001 1202 72c3 0000 0063 0000 0000 0000  ....r....c......
+00003cd0: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+00003ce0: 0000 733c 0000 0065 005a 0164 005a 0265  ..s<...e.Z.d.Z.e
+00003cf0: 036a 0464 0164 0264 0364 048d 035a 0565  .j.d.d.d.d...Z.e
+00003d00: 036a 0464 0564 0664 0364 0364 078d 045a  .j.d.d.d.d.d...Z
+00003d10: 0647 0064 0864 0984 0064 0983 025a 0764  .G.d.d...d...Z.d
+00003d20: 0a53 0029 0bda 1250 6861 726d 6163 7945  .S.)...PharmacyE
+00003d30: 6e74 6572 7072 6973 6572 2b00 0000 7223  nterpriser+...r#
+00003d40: 0000 0054 72ac 0000 0072 2200 0000 7251  ...Tr....r"...rQ
+00003d50: 0000 0072 2800 0000 6300 0000 0000 0000  ...r(...c.......
+00003d60: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00003d70: 0073 1800 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00003d80: 5a03 6402 5a04 6504 5a05 6403 5300 2904  Z.d.Z.e.Z.d.S.).
+00003d90: 7a17 5068 6172 6d61 6379 456e 7465 7270  z.PharmacyEnterp
+00003da0: 7269 7365 2e4d 6574 615a 1662 735f 7068  rise.MetaZ.bs_ph
+00003db0: 6172 6d61 6379 5f65 6e74 6572 7072 6973  armacy_enterpris
+00003dc0: 6575 0c00 0000 e88d afe4 bc81 e7ae a1e7  eu..............
+00003dd0: 9086 4e72 3600 0000 7219 0000 0072 1900  ..Nr6...r....r..
+00003de0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00003df0: 00e4 0100 0073 0600 0000 0801 0401 0401  .....s..........
+00003e00: 721b 0000 004e 72ae 0000 0072 1900 0000  r....Nr....r....
+00003e10: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00003e20: c500 0000 e001 0000 7306 0000 0008 0110  ........s.......
+00003e30: 0112 0272 c500 0000 6300 0000 0000 0000  ...r....c.......
+00003e40: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
+00003e50: 0073 8600 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
+00003e60: 6a04 6401 6402 6403 6404 8d03 5a05 6503  j.d.d.d.d...Z.e.
+00003e70: 6a04 6405 6406 6403 6403 6407 8d04 5a06  j.d.d.d.d.d...Z.
+00003e80: 6503 6a07 6508 6408 6503 6a09 6409 8d03  e.j.e.d.e.j.d...
+00003e90: 5a0a 6503 6a0b 640a 6403 6403 640b 8d03  Z.e.j.d.d.d.d...
+00003ea0: 5a0c 6503 6a07 650d 640c 6503 6a0e 6403  Z.e.j.e.d.e.j.d.
+00003eb0: 640d 8d04 5a0f 6503 6a07 6510 640e 6503  d...Z.e.j.e.d.e.
+00003ec0: 6a0e 6403 640d 8d04 5a11 4700 640f 6410  j.d.d...Z.G.d.d.
+00003ed0: 8400 6410 8302 5a12 6411 5300 2912 da12  ..d...Z.d.S.)...
+00003ee0: 5068 6172 6d61 6379 4d61 6e61 6765 6d65  PharmacyManageme
+00003ef0: 6e74 750c 0000 00e8 8daf e688 bfe7 bc96  ntu.............
+00003f00: e7a0 8172 2300 0000 5472 ac00 0000 750c  ...r#...Tr....u.
+00003f10: 0000 00e8 8daf e688 bfe5 908d e7a7 b072  ...............r
+00003f20: 5100 0000 7228 0000 0072 c400 0000 7248  Q...r(...r....rH
+00003f30: 0000 0075 0c00 0000 e88d afe6 88bf e59c  ...u............
+00003f40: b0e5 9d80 722a 0000 0072 2f00 0000 7230  ....r*...r/...r0
+00003f50: 0000 0075 0c00 0000 e689 80e5 b19e e88d  ...u............
+00003f60: afe4 bc81 6300 0000 0000 0000 0000 0000  ....c...........
+00003f70: 0000 0000 0001 0000 0040 0000 0073 1800  .........@...s..
+00003f80: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00003f90: 5a04 6504 5a05 6403 5300 2904 7a17 5068  Z.e.Z.d.S.).z.Ph
+00003fa0: 6172 6d61 6379 4d61 6e61 6765 6d65 6e74  armacyManagement
+00003fb0: 2e4d 6574 615a 1662 735f 7068 6172 6d61  .MetaZ.bs_pharma
+00003fc0: 6379 5f6d 616e 6167 656d 656e 7475 0c00  cy_managementu..
+00003fd0: 0000 e88d afe6 88bf e7ae a1e7 9086 4e72  ..............Nr
+00003fe0: 3600 0000 7219 0000 0072 1900 0000 7219  6...r....r....r.
+00003ff0: 0000 0072 1a00 0000 721b 0000 00f6 0100  ...r....r.......
+00004000: 0073 0600 0000 0801 0401 0401 721b 0000  .s..........r...
+00004010: 004e 2913 7215 0000 0072 1600 0000 7217  .N).r....r....r.
+00004020: 0000 0072 0500 0000 7239 0000 005a 0d70  ...r....r9...Z.p
+00004030: 6861 726d 6163 795f 636f 6465 5a0d 7068  harmacy_codeZ.ph
+00004040: 6172 6d61 6379 5f6e 616d 6572 4100 0000  armacy_namerA...
+00004050: 72c3 0000 0072 bd00 0000 5a0d 7068 6172  r....r....Z.phar
+00004060: 6d61 6379 5f74 7970 6572 3c00 0000 723f  macy_typer<...r?
+00004070: 0000 0072 2100 0000 7242 0000 0072 4a00  ...r!...rB...rJ.
+00004080: 0000 72c5 0000 005a 0a65 6e74 6572 7072  ..r....Z.enterpr
+00004090: 6973 6572 1b00 0000 7219 0000 0072 1900  iser....r....r..
+000040a0: 0000 7219 0000 0072 1a00 0000 72c6 0000  ..r....r....r...
+000040b0: 00ea 0100 0073 1600 0000 0801 1001 1201  .....s..........
+000040c0: 0401 0201 0201 04fd 0605 1001 1401 1402  ................
+000040d0: 72c6 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000040e0: 0000 0000 0000 0600 0000 4000 0000 734e  ..........@...sN
+000040f0: 0100 0065 005a 0164 005a 0265 036a 0465  ...e.Z.d.Z.e.j.e
+00004100: 0564 0165 036a 0664 0264 038d 045a 0765  .d.e.j.d.d...Z.e
+00004110: 036a 0864 0464 0564 0264 0264 068d 045a  .j.d.d.d.d.d...Z
+00004120: 0965 036a 0864 0764 0864 0264 0264 098d  .e.j.d.d.d.d.d..
+00004130: 045a 0a65 036a 0864 0764 0a64 0264 0264  .Z.e.j.d.d.d.d.d
+00004140: 098d 045a 0b65 036a 0864 0764 0b64 0264  ...Z.e.j.d.d.d.d
+00004150: 0264 098d 045a 0c65 036a 0465 0d64 0c65  .d...Z.e.j.e.d.e
+00004160: 036a 0e64 0d8d 035a 0f65 036a 0465 1064  .j.d...Z.e.j.e.d
+00004170: 0e65 036a 0e64 0d8d 035a 1165 036a 0465  .e.j.d...Z.e.j.e
+00004180: 1264 0f65 036a 0e64 0d8d 035a 1365 036a  .d.e.j.d...Z.e.j
+00004190: 0864 1064 1164 0264 0264 098d 045a 1465  .d.d.d.d.d...Z.e
+000041a0: 036a 0864 1264 1364 0264 0264 098d 045a  .j.d.d.d.d.d...Z
+000041b0: 1565 036a 0465 1664 1465 036a 0664 0264  .e.j.e.d.e.j.d.d
+000041c0: 038d 045a 1765 036a 1864 1564 0264 0264  ...Z.e.j.d.d.d.d
+000041d0: 168d 035a 1965 036a 1a64 1764 1864 0264  ...Z.e.j.d.d.d.d
+000041e0: 198d 035a 1b65 036a 0864 0764 1a64 0264  ...Z.e.j.d.d.d.d
+000041f0: 0264 098d 045a 1c65 036a 1d64 1b64 0264  .d...Z.e.j.d.d.d
+00004200: 1c8d 025a 1e65 036a 1d64 1d64 0264 1c8d  ...Z.e.j.d.d.d..
+00004210: 025a 1f65 036a 1d64 1e64 0264 1c8d 025a  .Z.e.j.d.d.d...Z
+00004220: 2065 036a 1d64 1f64 0264 1c8d 025a 2147   e.j.d.d.d...Z!G
+00004230: 0064 2064 2184 0064 2183 025a 2264 2253  .d d!..d!..Z"d"S
+00004240: 0029 23da 0c50 6861 726d 6163 7944 7275  .)#..PharmacyDru
+00004250: 6775 0c00 0000 e689 80e5 b19e e88d afe6  gu..............
+00004260: 88bf 5472 3000 0000 72b2 0000 0072 2300  ..Tr0...r....r#.
+00004270: 0000 7228 0000 0072 5100 0000 72b3 0000  ..r(...rQ...r...
+00004280: 0072 7a00 0000 72b4 0000 0075 0600 0000  .rz...r....u....
+00004290: e58d 95e4 bd8d 72b5 0000 0072 4800 0000  ......r....rH...
+000042a0: 72ad 0000 0072 b600 0000 7280 0000 0072  r....r....r....r
+000042b0: b800 0000 e9c8 0000 0072 b900 0000 722f  .........r....r/
+000042c0: 0000 0075 0c00 0000 e69c 89e6 9588 e697  ...u............
+000042d0: a5e6 9c9f 7210 0000 0072 b700 0000 7201  ....r....r....r.
+000042e0: 0000 0072 7900 0000 750c 0000 00e8 aea1  ...ry...u.......
+000042f0: e987 8fe5 8d95 e4bd 8d75 0c00 0000 e688  .........u......
+00004300: 90e6 9cac e58d 95e4 bbb7 728f 0000 0075  ..........r....u
+00004310: 0c00 0000 e688 90e6 9cac e987 91e9 a29d  ................
+00004320: 750c 0000 00e9 9bb6 e594 aee5 8d95 e4bb  u...............
+00004330: b775 0c00 0000 e99b b6e5 94ae e987 91e9  .u..............
+00004340: a29d 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00004350: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
+00004360: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+00004370: 6504 5a05 6403 5300 2904 7a11 5068 6172  e.Z.d.S.).z.Phar
+00004380: 6d61 6379 4472 7567 2e4d 6574 615a 1062  macyDrug.MetaZ.b
+00004390: 735f 7068 6172 6d61 6379 5f64 7275 6775  s_pharmacy_drugu
+000043a0: 0d00 0000 e88d afe6 88bf 2de8 8daf e593  ..........-.....
+000043b0: 814e 7236 0000 0072 1900 0000 7219 0000  .Nr6...r....r...
+000043c0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+000043d0: 1c02 0000 7306 0000 0008 0104 0104 0172  ....s..........r
+000043e0: 1b00 0000 4e29 2372 1500 0000 7216 0000  ....N)#r....r...
+000043f0: 0072 1700 0000 7205 0000 0072 4100 0000  .r....r....rA...
+00004400: 72c6 0000 0072 4200 0000 5a08 7068 6172  r....rB...Z.phar
+00004410: 6d61 6379 7239 0000 0072 ba00 0000 72bb  macyr9...r....r.
+00004420: 0000 0072 bc00 0000 da05 756e 6974 7372  ...r......unitsr
+00004430: a900 0000 72bd 0000 0072 be00 0000 72ab  ....r....r....r.
+00004440: 0000 0072 c000 0000 72b0 0000 0072 bf00  ...r....r....r..
+00004450: 0000 72c1 0000 0072 c200 0000 7221 0000  ..r....r....r!..
+00004460: 0072 4a00 0000 725f 0000 005a 0a76 616c  .rJ...r_...Z.val
+00004470: 6964 5f64 6174 6572 6f00 0000 5a12 696e  id_datero...Z.in
+00004480: 7665 6e74 6f72 795f 7175 616e 7469 7479  ventory_quantity
+00004490: 5a10 6d65 6173 7572 656d 656e 745f 756e  Z.measurement_un
+000044a0: 6974 7240 0000 005a 0f63 6f73 745f 756e  itr@...Z.cost_un
+000044b0: 6974 5f70 7269 6365 5a0b 636f 7374 5f61  it_priceZ.cost_a
+000044c0: 6d6f 756e 745a 1172 6574 6169 6c5f 756e  mountZ.retail_un
+000044d0: 6974 5f70 7269 6365 5a0d 7265 7461 696c  it_priceZ.retail
+000044e0: 5f61 6d6f 756e 7472 1b00 0000 7219 0000  _amountr....r...
+000044f0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00004500: 72c7 0000 00fc 0100 0073 3e00 0000 0801  r........s>.....
+00004510: 1401 1201 1201 1201 1201 0401 0201 0201  ................
+00004520: 04fd 0605 0401 0201 0201 04fd 0605 0401  ................
+00004530: 0201 0201 04fd 0605 1201 1201 1401 1001  ................
+00004540: 1001 1201 0e01 0e01 0e01 0e02 72c7 0000  ............r...
+00004550: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00004560: 0000 0600 0000 4000 0000 73b6 0000 0065  ......@...s....e
+00004570: 005a 0164 005a 0265 036a 0464 0164 0264  .Z.d.Z.e.j.d.d.d
+00004580: 038d 025a 0565 036a 0464 0164 0464 038d  ...Z.e.j.d.d.d..
+00004590: 025a 0665 036a 0464 0164 0564 0664 0664  .Z.e.j.d.d.d.d.d
+000045a0: 078d 045a 0765 036a 0464 0164 0864 038d  ...Z.e.j.d.d.d..
+000045b0: 025a 0865 036a 0464 0164 0964 038d 025a  .Z.e.j.d.d.d...Z
+000045c0: 0965 036a 0464 0a64 0b64 038d 025a 0a65  .e.j.d.d.d...Z.e
+000045d0: 036a 0464 0a64 0c64 038d 025a 0b65 036a  .j.d.d.d...Z.e.j
+000045e0: 0c64 0d64 0664 0664 0e8d 035a 0d65 036a  .d.d.d.d...Z.e.j
+000045f0: 0c64 0f64 0664 0664 108d 035a 0e65 036a  .d.d.d.d...Z.e.j
+00004600: 0f64 1164 0664 128d 025a 1047 0064 1364  .d.d.d...Z.G.d.d
+00004610: 1484 0064 1483 025a 1164 1564 1684 005a  ...d...Z.d.d...Z
+00004620: 1264 1753 0029 18da 0741 7069 496e 666f  .d.S.)...ApiInfo
+00004630: 7276 0000 0072 a100 0000 7277 0000 0075  rv...r....rw...u
+00004640: 0c00 0000 e8af b7e6 b182 e7bc 96e7 a081  ................
+00004650: 750c 0000 00e8 afb7 e6b1 82e5 908d e7a7  u...............
+00004660: b054 727a 0000 0075 0c00 0000 e8af b7e6  .Trz...u........
+00004670: b182 e696 b9e5 bc8f 7512 0000 00e8 afb7  ........u.......
+00004680: e6b1 82e6 95b0 e68d aee7 b1bb e59e 8b72  ...............r
+00004690: c800 0000 7511 0000 0069 70e5 9cb0 e59d  ....u....ip.....
+000046a0: 80e6 8896 e59f 9fe5 908d 750c 0000 00e8  ..........u.....
+000046b0: afb7 e6b1 82e8 b7af e794 b172 0a00 0000  ...........r....
+000046c0: 720b 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+000046d0: 1200 0000 7213 0000 0063 0000 0000 0000  ....r....c......
+000046e0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+000046f0: 0000 731c 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00004700: 015a 0364 025a 0465 045a 0564 035a 0664  .Z.d.Z.e.Z.d.Z.d
+00004710: 0453 0029 057a 0c41 7069 496e 666f 2e4d  .S.).z.ApiInfo.M
+00004720: 6574 615a 0b62 735f 6170 695f 696e 666f  etaZ.bs_api_info
+00004730: 750c 0000 00e6 8ea5 e58f a3e4 bfa1 e681  u...............
+00004740: af29 01a9 02da 086f 7267 5f63 6f64 65da  .).....org_code.
+00004750: 0872 6571 5f63 6f64 654e 724b 0000 0072  .req_codeNrK...r
+00004760: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+00004770: 0000 0072 1b00 0000 2e02 0000 7308 0000  ...r........s...
+00004780: 0008 0104 0104 0104 0172 1b00 0000 6303  .........r....c.
+00004790: 0000 0000 0000 0000 0000 0007 0000 0005  ................
+000047a0: 0000 0043 0000 0073 ba00 0000 7400 6a01  ...C...s....t.j.
+000047b0: 6a02 7c01 6401 1900 7c02 6402 8d02 a003  j.|.d...|.d.....
+000047c0: a100 7d03 7c03 72a8 7c03 6a04 7c03 6a05  ..}.|.r.|.j.|.j.
+000047d0: 1700 7d04 7c03 6a06 6403 6b02 7242 7407  ..}.|.j.d.k.rBt.
+000047e0: 6a08 7c04 7c01 6404 8d02 7d05 6e58 7c03  j.|.|.d...}.nX|.
+000047f0: 6a06 6405 6b02 725c 7407 6a09 7c04 7c01  j.d.k.r\t.j.|.|.
+00004800: 6406 8d02 7d05 6e3e 7c03 6a06 6407 6b02  d...}.n>|.j.d.k.
+00004810: 7276 7407 6a0a 7c04 7c01 6408 8d02 7d05  rvt.j.|.|.d...}.
+00004820: 6e24 7c03 6a06 6409 6b02 728e 7407 6a0b  n$|.j.d.k.r.t.j.
+00004830: 7c04 640a 8d01 7d05 6e0c 7407 6a0c 7c04  |.d...}.n.t.j.|.
+00004840: 640a 8d01 7d05 740d a00e 7c05 6a0f a101  d...}.t...|.j...
+00004850: 7d06 6e0e 640b 640c 640d 6900 640e 9c04  }.n.d.d.d.i.d...
+00004860: 7d06 7c06 5300 290f 4e72 a600 0000 72cb  }.|.S.).Nr....r.
+00004870: 0000 00da 0450 4f53 5429 0272 8d00 0000  .....POST).r....
+00004880: da04 6a73 6f6e da03 4745 5429 0272 8d00  ..json..GET).r..
+00004890: 0000 da06 7061 7261 6d73 da03 5055 5429  ....params..PUT)
+000048a0: 0272 8d00 0000 da04 6461 7461 da06 4445  .r......data..DE
+000048b0: 4c45 5445 2901 728d 0000 0046 69d1 0700  LETE).r....Fi...
+000048c0: 0075 1e00 0000 e4b8 8de5 ad98 e59c a8e5  .u..............
+000048d0: afb9 e68e a5e5 8cbb e999 a2e4 bfa1 e681  ................
+000048e0: afef bc81 2904 5a07 7375 6363 6573 7372  ....).Z.successr
+000048f0: af00 0000 da07 6d65 7373 6167 6572 d300  ......messager..
+00004900: 0000 2910 72ca 0000 00da 076f 626a 6563  ..).r......objec
+00004910: 7473 da06 6669 6c74 6572 7267 0000 00da  ts..filterrg....
+00004920: 0969 705f 646f 6d61 696e 7291 0000 00da  .ip_domainr.....
+00004930: 0a72 6571 5f6d 6574 686f 64da 0872 6571  .req_method..req
+00004940: 7565 7374 73da 0470 6f73 74da 0367 6574  uests..post..get
+00004950: da03 7075 74da 0664 656c 6574 65da 0570  ..put..delete..p
+00004960: 6174 6368 72cf 0000 00da 056c 6f61 6473  atchr......loads
+00004970: da04 7465 7874 2907 722e 0000 005a 0769  ..text).r....Z.i
+00004980: 6e5f 6461 7461 72cd 0000 005a 0c61 7069  n_datar....Z.api
+00004990: 5f69 6e66 6f5f 6f62 6a5a 0763 6d73 5f75  _info_objZ.cms_u
+000049a0: 726c da03 7265 735a 0872 6573 5f6a 736f  rl..resZ.res_jso
+000049b0: 6e72 1900 0000 7219 0000 0072 1a00 0000  nr....r....r....
+000049c0: da09 7772 6974 6562 6163 6b36 0200 0073  ..writeback6...s
+000049d0: 1e00 0000 0001 1801 0401 0c01 0a01 1001  ................
+000049e0: 0a01 1001 0a01 1001 0a01 0e02 0c01 0e02  ................
+000049f0: 0e01 7a11 4170 6949 6e66 6f2e 7772 6974  ..z.ApiInfo.writ
+00004a00: 6562 6163 6b4e 2913 7215 0000 0072 1600  ebackN).r....r..
+00004a10: 0000 7217 0000 0072 0500 0000 7239 0000  ..r....r....r9..
+00004a20: 0072 cc00 0000 72cd 0000 005a 0872 6571  .r....r....Z.req
+00004a30: 5f6e 616d 6572 d900 0000 7290 0000 0072  _namer....r....r
+00004a40: d800 0000 7291 0000 0072 1c00 0000 721d  ....r....r....r.
+00004a50: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
+00004a60: 0000 721b 0000 0072 e300 0000 7219 0000  ..r....r....r...
+00004a70: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00004a80: 72ca 0000 0022 0200 0073 1800 0000 0801  r...."...s......
+00004a90: 0e01 0e01 1201 0e01 0e01 0e01 0e01 1001  ................
+00004aa0: 1001 0e02 0e08 72ca 0000 0029 2572 cf00  ......r....)%r..
+00004ab0: 0000 da02 6f73 72da 0000 005a 1a64 6a61  ....osr....Z.dja
+00004ac0: 6e67 6f2e 636f 6e74 7269 622e 6175 7468  ngo.contrib.auth
+00004ad0: 2e6d 6f64 656c 7372 0200 0000 7203 0000  .modelsr....r...
+00004ae0: 005a 2264 6a61 6e67 6f2e 636f 6e74 7269  .Z"django.contri
+00004af0: 622e 636f 6e74 656e 7474 7970 6573 2e6d  b.contenttypes.m
+00004b00: 6f64 656c 7372 0400 0000 da09 646a 616e  odelsr......djan
+00004b10: 676f 2e64 6272 0500 0000 da0b 646a 616e  go.dbr......djan
+00004b20: 676f 2e63 6f6e 6672 0600 0000 725c 0000  go.confr....r\..
+00004b30: 00da 054d 6f64 656c 7209 0000 0072 2100  ...Modelr....r!.
+00004b40: 0000 7246 0000 0072 4d00 0000 724f 0000  ..rF...rM...rO..
+00004b50: 0072 6200 0000 7273 0000 0072 7e00 0000  .rb...rs...r~...
+00004b60: 728b 0000 0072 9300 0000 7296 0000 0072  r....r....r....r
+00004b70: 9d00 0000 72a7 0000 0072 a800 0000 72a9  ....r....r....r.
+00004b80: 0000 0072 ab00 0000 72b0 0000 0072 b100  ...r....r....r..
+00004b90: 0000 72c3 0000 0072 c500 0000 72c6 0000  ..r....r....r...
+00004ba0: 0072 c700 0000 72ca 0000 0072 1900 0000  .r....r....r....
+00004bb0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00004bc0: 083c 6d6f 6475 6c65 3e01 0000 0073 3c00  .<module>....s<.
+00004bd0: 0000 0801 0802 0801 1001 0c01 0c01 0c02  ................
+00004be0: 0406 1209 101e 101c 1014 1028 104a 121a  ...........(.J..
+00004bf0: 121b 1223 1019 1011 1011 1011 1011 100a  ...#............
+00004c00: 100a 100a 102a 100a 100a 1012 1026       .....*.......&
```

### Comparing `base_system-0.1.6/base_system/__pycache__/serializers.cpython-39.pyc` & `base_system-0.1.7/base_system/__pycache__/serializers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/__pycache__/urls.cpython-39.pyc` & `base_system-0.1.7/base_system/__pycache__/urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/__pycache__/views.cpython-39.pyc` & `base_system-0.1.7/base_system/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/__pycache__/viewsets.cpython-39.pyc` & `base_system-0.1.7/base_system/__pycache__/viewsets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/auth.py` & `base_system-0.1.7/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/migrations/0001_initial.py` & `base_system-0.1.7/base_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/models.py` & `base_system-0.1.7/base_system/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,14 +455,15 @@
     rcc_category = models.CharField(verbose_name="农合类别", max_length=20, null=True, blank=True)
     is_essential = models.BooleanField(verbose_name="是否是基药", default=True)
     hr_level = models.CharField(verbose_name="高危等级", max_length=64, null=True, blank=True)
     gb_code = models.CharField(verbose_name="国家贯标编码", max_length=64, null=True, blank=True)
     gb_name = models.CharField(verbose_name="国家贯标名称", max_length=64, null=True, blank=True)
     origin_place = models.CharField(max_length=64, verbose_name="产地", null=True, blank=True)
     manufacturer = models.CharField(max_length=64, verbose_name="生产厂家", null=True, blank=True)
+    code_medu_cur = models.CharField(verbose_name="单次用量单位编码", max_length=64, null=True)
 
     class Meta:
         db_table = 'bs_drug_directory'
         verbose_name = '药品目录'
         verbose_name_plural = verbose_name
```

### Comparing `base_system-0.1.6/base_system/serializers.py` & `base_system-0.1.7/base_system/serializers.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/urls.py` & `base_system-0.1.7/base_system/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/views.py` & `base_system-0.1.7/base_system/views.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system/viewsets.py` & `base_system-0.1.7/base_system/viewsets.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/base_system.egg-info/PKG-INFO` & `base_system-0.1.7/base_system.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base-system
-Version: 0.1.6
+Version: 0.1.7
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.1.6/base_system.egg-info/SOURCES.txt` & `base_system-0.1.7/base_system.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -36,9 +36,11 @@
 base_system/__pycache__/models.cpython-39.pyc
 base_system/__pycache__/serializers.cpython-39.pyc
 base_system/__pycache__/tests.cpython-39.pyc
 base_system/__pycache__/urls.cpython-39.pyc
 base_system/__pycache__/views.cpython-39.pyc
 base_system/__pycache__/viewsets.cpython-39.pyc
 base_system/migrations/0001_initial.py
+base_system/migrations/0002_drugdirectory_code_medu_cur.py
 base_system/migrations/__init__.py
+base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
 base_system/migrations/__pycache__/__init__.cpython-39.pyc
```

### Comparing `base_system-0.1.6/init_data.json` & `base_system-0.1.7/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/manage.py` & `base_system-0.1.7/manage.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/requirements.txt` & `base_system-0.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/runtests.py` & `base_system-0.1.7/runtests.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.6/setup.py` & `base_system-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.1.6',
+    version='0.1.7',
     description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
     url="https://github.com/zcjwin",
```

