# Comparing `tmp/base_system-0.1.9.tar.gz` & `tmp/base_system-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.1.9.tar", last modified: Thu May  4 07:47:47 2023, max compression
+gzip compressed data, was "base_system-0.2.0.tar", last modified: Thu May  4 07:57:42 2023, max compression
```

## Comparing `base_system-0.1.9.tar` & `base_system-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:47:47.957538 base_system-0.1.9/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.1.9/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.1.9/.pypirc
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:47:47.889504 base_system-0.1.9/BaseFunctionModule/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.1.9/BaseFunctionModule/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.9/BaseFunctionModule/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11868 2023-05-04 07:40:22.000000 base_system-0.1.9/BaseFunctionModule/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.1.9/BaseFunctionModule/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.1.9/BaseFunctionModule/wsgi.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.1.9/Dockerfile
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.1.9/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.1.9/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 07:47:47.957538 base_system-0.1.9/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.1.9/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:47:47.913516 base_system-0.1.9/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.1.9/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:47:47.945532 base_system-0.1.9/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.1.9/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.1.9/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.1.9/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    19474 2023-05-04 07:38:28.000000 base_system-0.1.9/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.1.9/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.1.9/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.1.9/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    32490 2023-05-04 07:38:29.000000 base_system-0.1.9/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11946 2023-05-04 07:38:29.000000 base_system-0.1.9/base_system/__pycache__/viewsets.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.1.9/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.1.9/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.1.9/base_system/auth.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:47:47.949534 base_system-0.1.9/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.1.9/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.1.9/base_system/migrations/0002_drugdirectory_code_medu_cur.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.1.9/base_system/migrations/0003_alter_extragroup_hospital.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.1.9/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:47:47.957538 base_system-0.1.9/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.1.9/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.1.9/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.1.9/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.1.9/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    25523 2023-05-04 07:38:11.000000 base_system-0.1.9/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.1.9/base_system/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.1.9/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.1.9/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    71807 2023-05-04 03:13:44.000000 base_system-0.1.9/base_system/views.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14983 2023-05-04 07:38:11.000000 base_system-0.1.9/base_system/viewsets.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:47:47.929524 base_system-0.1.9/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 07:47:47.000000 base_system-0.1.9/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1586 2023-05-04 07:47:47.000000 base_system-0.1.9/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 07:47:47.000000 base_system-0.1.9/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.1.9/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-04 07:47:47.000000 base_system-0.1.9/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-04 07:47:47.000000 base_system-0.1.9/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.1.9/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.1.9/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.1.9/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.1.9/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-04 07:47:47.957538 base_system-0.1.9/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-04 07:46:32.000000 base_system-0.1.9/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:57:42.989385 base_system-0.2.0/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.0/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.0/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:57:42.969359 base_system-0.2.0/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.0/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.0/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11868 2023-05-04 07:40:22.000000 base_system-0.2.0/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.0/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.0/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.0/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.0/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.0/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 07:57:42.985380 base_system-0.2.0/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.0/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:57:42.973364 base_system-0.2.0/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.0/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:57:42.981375 base_system-0.2.0/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.0/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.0/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.0/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19474 2023-05-04 07:38:28.000000 base_system-0.2.0/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.2.0/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.0/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.2.0/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    32490 2023-05-04 07:38:29.000000 base_system-0.2.0/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11946 2023-05-04 07:38:29.000000 base_system-0.2.0/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.0/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.0/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.0/base_system/auth.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:57:42.981375 base_system-0.2.0/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.0/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.0/base_system/migrations/0002_drugdirectory_code_medu_cur.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.0/base_system/migrations/0003_alter_extragroup_hospital.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.0/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:57:42.985380 base_system-0.2.0/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.0/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.0/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.0/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.0/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    25523 2023-05-04 07:38:11.000000 base_system-0.2.0/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.2.0/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.0/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.2.0/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    71807 2023-05-04 03:13:44.000000 base_system-0.2.0/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    14993 2023-05-04 07:55:49.000000 base_system-0.2.0/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 07:57:42.977370 base_system-0.2.0/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 07:57:42.000000 base_system-0.2.0/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1586 2023-05-04 07:57:42.000000 base_system-0.2.0/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 07:57:42.000000 base_system-0.2.0/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.0/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-04 07:57:42.000000 base_system-0.2.0/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-04 07:57:42.000000 base_system-0.2.0/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.0/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.0/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.0/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.0/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-04 07:57:42.989385 base_system-0.2.0/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-04 07:55:49.000000 base_system-0.2.0/setup.py
```

### Comparing `base_system-0.1.9/.gitignore` & `base_system-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/BaseFunctionModule/settings.py` & `base_system-0.2.0/BaseFunctionModule/settings.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/BaseFunctionModule/urls.py` & `base_system-0.2.0/BaseFunctionModule/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/LICENCE` & `base_system-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/PKG-INFO` & `base_system-0.2.0/base_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: base_system
-Version: 0.1.9
+Name: base-system
+Version: 0.2.0
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.1.9/README.rst` & `base_system-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.2.0/base_system/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/__pycache__/serializers.cpython-39.pyc` & `base_system-0.2.0/base_system/__pycache__/serializers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/__pycache__/urls.cpython-39.pyc` & `base_system-0.2.0/base_system/__pycache__/urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/__pycache__/views.cpython-39.pyc` & `base_system-0.2.0/base_system/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/__pycache__/viewsets.cpython-39.pyc` & `base_system-0.2.0/base_system/__pycache__/viewsets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/auth.py` & `base_system-0.2.0/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/migrations/0001_initial.py` & `base_system-0.2.0/base_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/migrations/0003_alter_extragroup_hospital.py` & `base_system-0.2.0/base_system/migrations/0003_alter_extragroup_hospital.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc` & `base_system-0.2.0/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc` & `base_system-0.2.0/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc` & `base_system-0.2.0/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/models.py` & `base_system-0.2.0/base_system/models.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/serializers.py` & `base_system-0.2.0/base_system/serializers.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/urls.py` & `base_system-0.2.0/base_system/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/views.py` & `base_system-0.2.0/base_system/views.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/base_system/viewsets.py` & `base_system-0.2.0/base_system/viewsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,18 +111,18 @@
     #     data["total_permissions"] = self.serializer_permission(total_permissions)
     #     return Response(data=data, status=status.HTTP_200_OK)
     @transaction.atomic
     def create(self, request, *args, **kwargs):
         msec_str = datetime.datetime.now().strftime('%f')
         extra, group_data = self.check_data(request.data)
         # 创建角色及相关及权限
-        new_group = Group.objects.filter(name=group_data["name"])
+        new_group = Group.objects.filter(name=group_data["role_name"])
         if new_group:
             return Response(data={"msg": "角色已经存在"}, status=210)
-        group = Group.objects.create(name=f'{msec_str}_'+group_data["name"])
+        group = Group.objects.create(name=f'{msec_str}_'+group_data["role_name"])
         group.permissions.set(group_data["permission_ids"])
         group.save()
         # 创建用户附加信息
         # extra = ExtraGroup.objects.create(group_id=group.pk, **extra)
         extra['group']=group.pk
 
         serializer = ExtraGroupSerializer(data=extra)
```

### Comparing `base_system-0.1.9/base_system.egg-info/PKG-INFO` & `base_system-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: base-system
-Version: 0.1.9
+Name: base_system
+Version: 0.2.0
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.1.9/base_system.egg-info/SOURCES.txt` & `base_system-0.2.0/base_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/init_data.json` & `base_system-0.2.0/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/manage.py` & `base_system-0.2.0/manage.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/requirements.txt` & `base_system-0.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/runtests.py` & `base_system-0.2.0/runtests.py`

 * *Files identical despite different names*

### Comparing `base_system-0.1.9/setup.py` & `base_system-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.1.9',
+    version='0.2.0',
     description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
     url="https://github.com/zcjwin",
```

