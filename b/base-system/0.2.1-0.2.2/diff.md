# Comparing `tmp/base_system-0.2.1.tar.gz` & `tmp/base_system-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.2.1.tar", last modified: Thu May  4 08:19:49 2023, max compression
+gzip compressed data, was "base_system-0.2.2.tar", last modified: Thu May  4 08:35:25 2023, max compression
```

## Comparing `base_system-0.2.1.tar` & `base_system-0.2.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:19:49.179086 base_system-0.2.1/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.1/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.1/.pypirc
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:19:49.163074 base_system-0.2.1/BaseFunctionModule/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.1/BaseFunctionModule/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.1/BaseFunctionModule/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11868 2023-05-04 07:40:22.000000 base_system-0.2.1/BaseFunctionModule/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.1/BaseFunctionModule/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.1/BaseFunctionModule/wsgi.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.1/Dockerfile
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.1/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.1/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 08:19:49.179086 base_system-0.2.1/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.1/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:19:49.167077 base_system-0.2.1/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.1/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:19:49.171080 base_system-0.2.1/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.1/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.1/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.1/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    19488 2023-05-04 08:07:15.000000 base_system-0.2.1/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.2.1/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.1/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.2.1/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    32490 2023-05-04 07:38:29.000000 base_system-0.2.1/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11925 2023-05-04 08:07:17.000000 base_system-0.2.1/base_system/__pycache__/viewsets.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.1/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.1/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.1/base_system/auth.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:19:49.171080 base_system-0.2.1/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.1/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.1/base_system/migrations/0002_drugdirectory_code_medu_cur.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.1/base_system/migrations/0003_alter_extragroup_hospital.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.1/base_system/migrations/0004_alter_extragroup_role_name.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.1/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:19:49.179086 base_system-0.2.1/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.1/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.1/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.1/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.1/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    25535 2023-05-04 08:07:06.000000 base_system-0.2.1/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.2.1/base_system/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.1/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.2.1/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    71807 2023-05-04 03:13:44.000000 base_system-0.2.1/base_system/views.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14932 2023-05-04 08:07:06.000000 base_system-0.2.1/base_system/viewsets.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:19:49.167077 base_system-0.2.1/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 08:19:48.000000 base_system-0.2.1/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1644 2023-05-04 08:19:49.000000 base_system-0.2.1/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 08:19:48.000000 base_system-0.2.1/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.1/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-04 08:19:48.000000 base_system-0.2.1/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-04 08:19:48.000000 base_system-0.2.1/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.1/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.1/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.1/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.1/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-04 08:19:49.179086 base_system-0.2.1/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-04 08:02:47.000000 base_system-0.2.1/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.982753 base_system-0.2.2/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.2/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.2/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.938723 base_system-0.2.2/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.2/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.2/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11868 2023-05-04 07:40:22.000000 base_system-0.2.2/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.2/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.2/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.2/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.2/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.2/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 08:35:25.982753 base_system-0.2.2/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.2/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.946728 base_system-0.2.2/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.2/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.966742 base_system-0.2.2/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.2/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.2/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.2/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19488 2023-05-04 08:07:15.000000 base_system-0.2.2/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    26400 2023-04-27 02:23:07.000000 base_system-0.2.2/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.2/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3040 2023-04-27 02:24:02.000000 base_system-0.2.2/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    32490 2023-05-04 07:38:29.000000 base_system-0.2.2/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11925 2023-05-04 08:07:17.000000 base_system-0.2.2/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.2/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.2/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.2/base_system/auth.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.974747 base_system-0.2.2/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.2/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.2/base_system/migrations/0002_drugdirectory_code_medu_cur.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.2/base_system/migrations/0003_alter_extragroup_hospital.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.2/base_system/migrations/0004_alter_extragroup_role_name.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.2/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.978750 base_system-0.2.2/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.2/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.2/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.2/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.2/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    25535 2023-05-04 08:07:06.000000 base_system-0.2.2/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    22810 2023-04-27 02:23:04.000000 base_system-0.2.2/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.2/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3855 2023-04-27 02:23:59.000000 base_system-0.2.2/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    71807 2023-05-04 03:13:44.000000 base_system-0.2.2/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    14978 2023-05-04 08:34:21.000000 base_system-0.2.2/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-04 08:35:25.954734 base_system-0.2.2/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1644 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.2/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-04 08:35:25.000000 base_system-0.2.2/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.2/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.2/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.2/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.2/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-04 08:35:25.982753 base_system-0.2.2/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-04 08:34:21.000000 base_system-0.2.2/setup.py
```

### Comparing `base_system-0.2.1/.gitignore` & `base_system-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/BaseFunctionModule/settings.py` & `base_system-0.2.2/BaseFunctionModule/settings.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/BaseFunctionModule/urls.py` & `base_system-0.2.2/BaseFunctionModule/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/LICENCE` & `base_system-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/PKG-INFO` & `base_system-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base_system
-Version: 0.2.1
+Version: 0.2.2
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.1/README.rst` & `base_system-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.2.2/base_system/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/__pycache__/serializers.cpython-39.pyc` & `base_system-0.2.2/base_system/__pycache__/serializers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/__pycache__/urls.cpython-39.pyc` & `base_system-0.2.2/base_system/__pycache__/urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/__pycache__/views.cpython-39.pyc` & `base_system-0.2.2/base_system/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/__pycache__/viewsets.cpython-39.pyc` & `base_system-0.2.2/base_system/__pycache__/viewsets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/auth.py` & `base_system-0.2.2/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/migrations/0001_initial.py` & `base_system-0.2.2/base_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/migrations/0003_alter_extragroup_hospital.py` & `base_system-0.2.2/base_system/migrations/0003_alter_extragroup_hospital.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc` & `base_system-0.2.2/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc` & `base_system-0.2.2/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc` & `base_system-0.2.2/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/models.py` & `base_system-0.2.2/base_system/models.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/serializers.py` & `base_system-0.2.2/base_system/serializers.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/urls.py` & `base_system-0.2.2/base_system/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/views.py` & `base_system-0.2.2/base_system/views.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/base_system/viewsets.py` & `base_system-0.2.2/base_system/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         # data = dict(data)
         extra["note"] = data.get("note")
         extra["is_active"] = data.get("is_active", 1)
         extra["hospital"] = data.get("hospital_id")
         extra["order_by"] = data.get("order_by")
         extra["created_user"] = data.get("created_user")
         extra["role_code"] = data.get("role_code")
+        extra["role_name"] = data.get("name")
         serializer = ExtraGroupSerializer(data=extra)
         serializer.is_valid(raise_exception=True)
         extra = serializer.data
 
         # 校验角色数据
         group_data = dict()
         permissions = data.get("permission_ids")
```

### Comparing `base_system-0.2.1/base_system.egg-info/PKG-INFO` & `base_system-0.2.2/base_system.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base-system
-Version: 0.2.1
+Version: 0.2.2
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.1/base_system.egg-info/SOURCES.txt` & `base_system-0.2.2/base_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/init_data.json` & `base_system-0.2.2/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/manage.py` & `base_system-0.2.2/manage.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/requirements.txt` & `base_system-0.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/runtests.py` & `base_system-0.2.2/runtests.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.1/setup.py` & `base_system-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.2.1',
+    version='0.2.2',
     description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
     url="https://github.com/zcjwin",
```

