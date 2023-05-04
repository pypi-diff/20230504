# Comparing `tmp/django-tequila-3.4.0.tar.gz` & `tmp/django-tequila-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tequila-3.4.0.tar", last modified: Thu Apr 14 13:53:11 2022, max compression
+gzip compressed data, was "django-tequila-4.0.0.tar", last modified: Thu May  4 15:38:44 2023, max compression
```

## Comparing `django-tequila-3.4.0.tar` & `django-tequila-4.0.0.tar`

### file list

```diff
@@ -1,88 +1,110 @@
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/
--rw-r--r--   0 del       (1000) del       (1000)       89 2017-09-15 15:05:00.000000 django-tequila-3.4.0/MANIFEST.in
--rw-rw-r--   0 del       (1000) del       (1000)     8105 2022-04-14 13:53:11.174038 django-tequila-3.4.0/PKG-INFO
--rw-rw-r--   0 del       (1000) del       (1000)     5620 2021-02-22 09:22:32.000000 django-tequila-3.4.0/README.rst
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.170038 django-tequila-3.4.0/django_tequila/
--rw-rw-r--   0 del       (1000) del       (1000)      126 2022-04-14 12:37:57.000000 django-tequila-3.4.0/django_tequila/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)     2546 2018-04-18 13:37:59.000000 django-tequila-3.4.0/django_tequila/admin.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.170038 django-tequila-3.4.0/django_tequila/django_backend/
--rw-rw-r--   0 del       (1000) del       (1000)    10725 2022-04-14 12:38:15.000000 django-tequila-3.4.0/django_tequila/django_backend/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)     4946 2022-04-14 12:42:41.000000 django-tequila-3.4.0/django_tequila/middleware.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.170038 django-tequila-3.4.0/django_tequila/tequila_auth_views/
--rw-r--r--   0 del       (1000) del       (1000)     3173 2020-04-23 12:46:45.000000 django-tequila-3.4.0/django_tequila/tequila_auth_views/__init__.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.170038 django-tequila-3.4.0/django_tequila/tequila_client/
--rw-r--r--   0 del       (1000) del       (1000)      232 2018-04-18 13:40:21.000000 django-tequila-3.4.0/django_tequila/tequila_client/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)     5055 2022-04-14 12:38:09.000000 django-tequila-3.4.0/django_tequila/tequila_client/client.py
--rw-r--r--   0 del       (1000) del       (1000)     2743 2020-02-26 08:00:25.000000 django-tequila-3.4.0/django_tequila/tequila_client/config.py
--rw-r--r--   0 del       (1000) del       (1000)      386 2021-01-15 14:07:40.000000 django-tequila-3.4.0/django_tequila/urls.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.170038 django-tequila-3.4.0/django_tequila.egg-info/
--rw-rw-r--   0 del       (1000) del       (1000)     8105 2022-04-14 13:53:11.000000 django-tequila-3.4.0/django_tequila.egg-info/PKG-INFO
--rw-rw-r--   0 del       (1000) del       (1000)     3421 2022-04-14 13:53:11.000000 django-tequila-3.4.0/django_tequila.egg-info/SOURCES.txt
--rw-rw-r--   0 del       (1000) del       (1000)        1 2022-04-14 13:53:11.000000 django-tequila-3.4.0/django_tequila.egg-info/dependency_links.txt
--rw-rw-r--   0 del       (1000) del       (1000)       15 2022-04-14 13:53:11.000000 django-tequila-3.4.0/django_tequila.egg-info/top_level.txt
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.170038 django-tequila-3.4.0/sample_app/
--rw-rw-r--   0 del       (1000) del       (1000)      627 2021-02-22 09:22:32.000000 django-tequila-3.4.0/sample_app/create_superadmin.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.170038 django-tequila-3.4.0/sample_app/python3-6-django-1/
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/
--rw-rw-r--   0 del       (1000) del       (1000)      103 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)        0 2021-02-01 09:59:21.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/admin.py
--rw-r--r--   0 del       (1000) del       (1000)   159744 2021-02-01 12:38:36.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/database.db
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/migrations/
--rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/migrations/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)        0 2021-02-01 09:59:21.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/models.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/requirements/
--rw-rw-r--   0 del       (1000) del       (1000)      158 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/requirements/base.txt
--rw-rw-r--   0 del       (1000) del       (1000)     3973 2021-02-01 10:07:33.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/settings.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/templates/
--rw-rw-r--   0 del       (1000) del       (1000)      603 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/templates/index.html
--rw-rw-r--   0 del       (1000) del       (1000)      167 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/templates/unprotected_view.html
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/tests/
--rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/tests/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)      271 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/tests/test_django.py
--rw-rw-r--   0 del       (1000) del       (1000)     2631 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/tests/test_selenium.py
--rw-rw-r--   0 del       (1000) del       (1000)      721 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/urls.py
--rw-rw-r--   0 del       (1000) del       (1000)     1122 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/views.py
--rw-rw-r--   0 del       (1000) del       (1000)      283 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/wsgi.py
--rw-rw-r--   0 del       (1000) del       (1000)      343 2021-02-22 09:22:32.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/docker-compose.yml
--rwxrwxr-x   0 del       (1000) del       (1000)      655 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/manage.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/
--rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)     1722 2021-02-22 09:22:32.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/admin.py
--rw-rw-r--   0 del       (1000) del       (1000)       97 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/apps.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/migrations/
--rw-rw-r--   0 del       (1000) del       (1000)     1329 2021-02-01 09:53:47.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/migrations/0001_initial.py
--rw-rw-r--   0 del       (1000) del       (1000)      483 2021-02-22 09:22:32.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/migrations/0002_auto_20210201_1010.py
--rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/migrations/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)     1239 2021-02-22 09:22:32.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/models.py
--rw-rw-r--   0 del       (1000) del       (1000)       60 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/tests.py
--rw-rw-r--   0 del       (1000) del       (1000)       63 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/views.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-8-django-2/
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-8-django-2/.pytest_cache/
--rw-r--r--   0 del       (1000) del       (1000)       37 2022-04-14 12:39:48.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/.pytest_cache/.gitignore
--rw-r--r--   0 del       (1000) del       (1000)      191 2022-04-14 12:39:48.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 del       (1000) del       (1000)      302 2022-04-14 12:39:48.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/.pytest_cache/README.md
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/
--rw-rw-r--   0 del       (1000) del       (1000)      103 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)      876 2021-02-20 11:38:24.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/admin.py
--rw-rw-rw-   0 del       (1000) del       (1000)   147456 2022-04-14 12:43:17.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/database.db
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/migrations/
--rw-rw-r--   0 del       (1000) del       (1000)     3394 2021-02-22 09:22:32.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/migrations/0001_initial.py
--rw-r--r--   0 del       (1000) del       (1000)        0 2021-02-20 11:38:34.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/migrations/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)     1703 2021-02-22 09:22:32.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/models.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/requirements/
--rw-rw-r--   0 del       (1000) del       (1000)      157 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/requirements/base.txt
--rw-rw-r--   0 del       (1000) del       (1000)     3877 2021-02-22 09:22:32.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/settings.py
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/templates/
--rw-rw-r--   0 del       (1000) del       (1000)      659 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/templates/index.html
--rw-rw-r--   0 del       (1000) del       (1000)      167 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/templates/unprotected_view.html
-drwxrwxr-x   0 del       (1000) del       (1000)        0 2022-04-14 13:53:11.174038 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/tests/
--rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/tests/__init__.py
--rw-rw-r--   0 del       (1000) del       (1000)      271 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/tests/test_django.py
--rw-rw-r--   0 del       (1000) del       (1000)     2631 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/tests/test_selenium.py
--rw-rw-r--   0 del       (1000) del       (1000)      721 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/urls.py
--rw-rw-r--   0 del       (1000) del       (1000)     1122 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/views.py
--rw-rw-r--   0 del       (1000) del       (1000)      283 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/wsgi.py
--rw-rw-r--   0 del       (1000) del       (1000)      362 2021-02-22 09:22:32.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/docker-compose.yml
--rwxrwxr-x   0 del       (1000) del       (1000)      655 2021-01-15 16:19:05.000000 django-tequila-3.4.0/sample_app/python3-8-django-2/manage.py
--rw-rw-r--   0 del       (1000) del       (1000)       38 2022-04-14 13:53:11.174038 django-tequila-3.4.0/setup.cfg
--rw-r--r--   0 del       (1000) del       (1000)     1306 2020-02-26 12:55:18.000000 django-tequila-3.4.0/setup.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.971518 django-tequila-4.0.0/
+-rw-rw-r--   0 del       (1000) del       (1000)      197 2021-01-21 13:03:12.000000 django-tequila-4.0.0/AUTHORS
+-rw-rw-r--   0 del       (1000) del       (1000)       89 2021-01-21 13:03:12.000000 django-tequila-4.0.0/MANIFEST.in
+-rw-rw-r--   0 del       (1000) del       (1000)     6496 2023-05-04 15:38:44.971518 django-tequila-4.0.0/PKG-INFO
+-rw-rw-r--   0 del       (1000) del       (1000)     5648 2023-05-04 15:32:07.000000 django-tequila-4.0.0/README.rst
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.959518 django-tequila-4.0.0/django_tequila/
+-rw-rw-r--   0 del       (1000) del       (1000)      126 2023-05-04 15:32:53.000000 django-tequila-4.0.0/django_tequila/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)     2617 2023-05-04 15:33:26.000000 django-tequila-4.0.0/django_tequila/admin.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/django_tequila/django_backend/
+-rw-rw-r--   0 del       (1000) del       (1000)    10725 2023-05-04 14:09:59.000000 django-tequila-4.0.0/django_tequila/django_backend/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)     4946 2023-05-04 14:09:59.000000 django-tequila-4.0.0/django_tequila/middleware.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/django_tequila/tequila_auth_views/
+-rw-rw-r--   0 del       (1000) del       (1000)     3213 2023-05-04 15:13:14.000000 django-tequila-4.0.0/django_tequila/tequila_auth_views/__init__.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/django_tequila/tequila_client/
+-rw-rw-r--   0 del       (1000) del       (1000)      232 2021-01-21 13:03:12.000000 django-tequila-4.0.0/django_tequila/tequila_client/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)     5055 2023-05-04 14:09:59.000000 django-tequila-4.0.0/django_tequila/tequila_client/client.py
+-rw-rw-r--   0 del       (1000) del       (1000)     2743 2021-01-21 13:03:12.000000 django-tequila-4.0.0/django_tequila/tequila_client/config.py
+-rw-rw-r--   0 del       (1000) del       (1000)      432 2023-05-04 15:13:14.000000 django-tequila-4.0.0/django_tequila/urls.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/django_tequila.egg-info/
+-rw-rw-r--   0 del       (1000) del       (1000)     6496 2023-05-04 15:38:44.000000 django-tequila-4.0.0/django_tequila.egg-info/PKG-INFO
+-rw-rw-r--   0 del       (1000) del       (1000)     4460 2023-05-04 15:38:44.000000 django-tequila-4.0.0/django_tequila.egg-info/SOURCES.txt
+-rw-rw-r--   0 del       (1000) del       (1000)        1 2023-05-04 15:38:44.000000 django-tequila-4.0.0/django_tequila.egg-info/dependency_links.txt
+-rw-rw-r--   0 del       (1000) del       (1000)       15 2023-05-04 15:38:44.000000 django-tequila-4.0.0/django_tequila.egg-info/top_level.txt
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/sample_app/
+-rw-rw-r--   0 del       (1000) del       (1000)      627 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/create_superadmin.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/sample_app/python3-6-django-1/
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/
+-rw-rw-r--   0 del       (1000) del       (1000)      103 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/admin.py
+-rw-r--rw-   0 del       (1000) del       (1000)   151552 2021-01-21 16:20:58.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/database.db
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/migrations/
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/migrations/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/models.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/requirements/
+-rw-rw-r--   0 del       (1000) del       (1000)      158 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/requirements/base.txt
+-rw-rw-r--   0 del       (1000) del       (1000)     3973 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/settings.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/templates/
+-rw-rw-r--   0 del       (1000) del       (1000)      603 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/templates/index.html
+-rw-rw-r--   0 del       (1000) del       (1000)      167 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/templates/unprotected_view.html
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/tests/
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/tests/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)      271 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/tests/test_django.py
+-rw-rw-r--   0 del       (1000) del       (1000)     2631 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/tests/test_selenium.py
+-rw-rw-r--   0 del       (1000) del       (1000)      721 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/urls.py
+-rw-rw-r--   0 del       (1000) del       (1000)     1122 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/views.py
+-rw-rw-r--   0 del       (1000) del       (1000)      283 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/wsgi.py
+-rw-rw-r--   0 del       (1000) del       (1000)      343 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/docker-compose.yml
+-rwxrwxr-x   0 del       (1000) del       (1000)      655 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/manage.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.963518 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)     1722 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/admin.py
+-rw-rw-r--   0 del       (1000) del       (1000)       97 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/apps.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.967518 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/migrations/
+-rw-rw-r--   0 del       (1000) del       (1000)     1329 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/migrations/0001_initial.py
+-rw-rw-r--   0 del       (1000) del       (1000)      483 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/migrations/0002_auto_20210201_1010.py
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/migrations/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)     1239 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/models.py
+-rw-rw-r--   0 del       (1000) del       (1000)       60 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/tests.py
+-rw-rw-r--   0 del       (1000) del       (1000)       63 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/views.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.967518 django-tequila-4.0.0/sample_app/python3-8-django-2/
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.967518 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/
+-rw-rw-r--   0 del       (1000) del       (1000)      103 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)      876 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/admin.py
+-rw-r--r--   0 del       (1000) del       (1000)   147456 2021-01-21 15:23:44.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/database.db
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.967518 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/migrations/
+-rw-rw-r--   0 del       (1000) del       (1000)     3394 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/migrations/0001_initial.py
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/migrations/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)     1703 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/models.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.967518 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/requirements/
+-rw-rw-r--   0 del       (1000) del       (1000)      157 2023-05-04 15:18:54.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/requirements/base.txt
+-rw-rw-r--   0 del       (1000) del       (1000)     3877 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/settings.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.967518 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/templates/
+-rw-rw-r--   0 del       (1000) del       (1000)      659 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/templates/index.html
+-rw-rw-r--   0 del       (1000) del       (1000)      167 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/templates/unprotected_view.html
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.967518 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/tests/
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/tests/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)      271 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/tests/test_django.py
+-rw-rw-r--   0 del       (1000) del       (1000)     2631 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/tests/test_selenium.py
+-rw-rw-r--   0 del       (1000) del       (1000)      721 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/urls.py
+-rw-rw-r--   0 del       (1000) del       (1000)     1122 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/views.py
+-rw-rw-r--   0 del       (1000) del       (1000)      283 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/wsgi.py
+-rw-rw-r--   0 del       (1000) del       (1000)      362 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/docker-compose.yml
+-rwxrwxr-x   0 del       (1000) del       (1000)      655 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-2/manage.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.967518 django-tequila-4.0.0/sample_app/python3-8-django-4/
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.967518 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2023-05-04 14:22:11.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)      876 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/admin.py
+-rw-rw-r--   0 del       (1000) del       (1000)      413 2023-05-04 14:32:15.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/asgi.py
+-rw-r--r--   0 del       (1000) del       (1000)   135168 2023-05-04 15:31:57.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/database.db
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.971518 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/migrations/
+-rw-r--r--   0 del       (1000) del       (1000)     3406 2023-05-04 15:30:57.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/migrations/0001_initial.py
+-rw-r--r--   0 del       (1000) del       (1000)        0 2023-05-04 15:30:57.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/migrations/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)     1703 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/models.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.971518 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/requirements/
+-rw-rw-r--   0 del       (1000) del       (1000)      178 2023-05-04 15:19:00.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/requirements/base.txt
+-rw-rw-r--   0 del       (1000) del       (1000)     4449 2023-05-04 15:15:23.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/settings.py
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.971518 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/templates/
+-rw-rw-r--   0 del       (1000) del       (1000)      659 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/templates/index.html
+-rw-rw-r--   0 del       (1000) del       (1000)      167 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/templates/unprotected_view.html
+drwxrwxr-x   0 del       (1000) del       (1000)        0 2023-05-04 15:38:44.971518 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/tests/
+-rw-rw-r--   0 del       (1000) del       (1000)        0 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/tests/__init__.py
+-rw-rw-r--   0 del       (1000) del       (1000)      271 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/tests/test_django.py
+-rw-rw-r--   0 del       (1000) del       (1000)     2631 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/tests/test_selenium.py
+-rw-rw-r--   0 del       (1000) del       (1000)     1359 2023-05-04 15:20:51.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/urls.py
+-rw-rw-r--   0 del       (1000) del       (1000)     1122 2021-01-21 13:03:12.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/views.py
+-rw-rw-r--   0 del       (1000) del       (1000)      413 2023-05-04 14:32:15.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/django_tequila_app/wsgi.py
+-rw-rw-r--   0 del       (1000) del       (1000)      362 2023-05-04 14:09:59.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/docker-compose.yml
+-rwxrwxr-x   0 del       (1000) del       (1000)      674 2023-05-04 14:44:40.000000 django-tequila-4.0.0/sample_app/python3-8-django-4/manage.py
+-rw-rw-r--   0 del       (1000) del       (1000)       38 2023-05-04 15:38:44.971518 django-tequila-4.0.0/setup.cfg
+-rw-rw-r--   0 del       (1000) del       (1000)     1306 2021-01-21 13:03:12.000000 django-tequila-4.0.0/setup.py
```

### Comparing `django-tequila-3.4.0/PKG-INFO` & `django-tequila-4.0.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,227 +1,206 @@
-Metadata-Version: 2.1
-Name: django-tequila
-Version: 3.4.0
-Summary: A Tequila authentication backend for django
-Home-page: https://github.com/epfl-idevelop/django-tequila
-Author: Julien Delasoie
-Author-email: julien.delasoie@epfl.ch
-License: LGPLv3
-Description: django-tequila
-        ==============
-        
-        `Tequila <http://tequila.epfl.ch/>`_ authentication for django.
-        
-        
-        Requirements
-        ============
-        
-        ``django-tequila`` needs the Django 2.2 LTS
-        
-        This project also expects a fully operational `Tequila <http://tequila.epfl.ch/>`_ server.
-        
-        Installation
-        ============
-        
-            pip install django-tequila
-        
-        Configuration
-        =============
-        
-        settings.py
-        -----------
-        
-        * Add at the end of your ``MIDDLEWARE_CLASSES``::
-        
-        	'django_tequila.middleware.TequilaMiddleware',
-        
-        * Add to ``INSTALLED_APPS``::
-        
-        	'django_tequila',
-        
-        * Add the line::
-        
-        	AUTHENTICATION_BACKENDS = ('django_tequila.django_backend.TequilaBackend',)
-        
-        * Set a name that will be displayed on the tequila login page::
-        
-        	TEQUILA_SERVICE_NAME = "django_tequila_service"
-        
-        * Finally, add / customize login/logout workflow ::
-        
-            LOGIN_URL = "/login"
-            LOGIN_REDIRECT_URL = "/"
-            LOGOUT_URL = '/'
-            LOGIN_REDIRECT_IF_NOT_ALLOWED = "/not_allowed"
-            LOGIN_REDIRECT_TEXT_IF_NOT_ALLOWED  = "Not allowed"
-        
-        urls.py
-        -------
-        
-        * Add these lines::
-        
-        	from django_tequila.urls import urlpatterns as django_tequila_urlpatterns
-        
-        	urlpatterns += django_tequila_urlpatterns
-        
-        Login/logout links
-        ------------------
-        
-        If you want the user to be redirected to a specific page after he logged/logout successfully, you have to add the 'next' parameter to your login url,
-        like the default Django authentication backend.
-        See `Django help for login-redirect-url <https://docs.djangoproject.com/en/dev/ref/settings/#login-redirect-url>`_ for more information.
-        
-        
-        Profile customization
-        ---------------------
-        You may want to keep some additional information about the user.
-        Take a look at `this page <http://docs.djangoproject.com/en/dev/topics/auth/#storing-additional-information-about-users>`_ for more information about profile customization.
-        
-        Here is an example for a profile for Django 2.0
-        
-        * Create a custom User model in your `models.py` (see ./sample_app/python3-8-django-2/django_tequila_app/models.py)
-        
-        * in your `settings.py`, tell django to use your model (see ./sample_app/python3-8-django-2/django_tequila_app/settings.py)::
-            AUTH_USER_MODEL = 'my_app.User'
-            TEQUILA_CUSTOM_USERNAME_ATTRIBUTE = "uniqueid"
-        
-        
-        * Update your database::
-        
-        	./manage.py syncdb
-        
-        Site Admin customizations
-        -------------------------
-        
-        - Add or modify your admin.py file, like ./sample_app/python3-8-django-2/django_tequila_app/admin.py
-        
-        
-        Additional tips and settings
-        ============================
-        
-        Advanced settings
-        -----------------
-        
-        * If you need to use your personal server, change this parameter::
-        
-        	TEQUILA_SERVER_URL = "https://tequila.epfl.ch"
-        
-        * You may want to create an inactive user when someone try to connect to your app. So you can manually control who access it.
-          If this is the case, add this line to `settings.py`::
-        
-        	TEQUILA_NEW_USER_INACTIVE = True
-        
-        * You may want to add some custom allow with Tequila.
-          If this is the case, add this line to `settings.py`::
-        
-        	TEQUILA_CONFIG_ALLOW = 'categorie=shibboleth'
-        
-          or, for multiple allow :
-        
-        	TEQUILA_CONFIG_ALLOW = 'categorie=shibboleth|categorie=epfl-old'
-        
-        * You may want to add some custom paramaters with Tequila.
-          If this is the case, add this line to `settings.py`::
-        
-        	TEQUILA_CONFIG_ADDITIONAL = {'allowedorgs': 'EPFL, UNIL'}
-        
-        * Everytime the user connect trought the Tequila process, he is redirected to an url
-          that has a 'key' paramter. For some esthetic reasons,you may want to remove this parameter,
-          so add this line to `settings.py`::
-        
-            TEQUILA_CLEAN_URL = True
-        
-          As it creates a redirect to the cleaned address and add an additional page hit, The value by default is False
-        
-        * You can force a strong authentication
-          so add this line to `settings.py`::
-        
-            TEQUILA_STRONG_AUTHENTICATION = True
-        
-          Default value is False
-        
-        * The only value that is truly unique is the sciper ('uniqueid' in Tequila). If your application
-          need a different usage, you can set to a different field (at your own risk though). You can add this line to `settings.py`::
-        
-            TEQUILA_CUSTOM_USERNAME_ATTRIBUTE = 'uniqueid'
-        
-          Ex. : username, email, etc.
-        
-          Default value is username
-        
-        * You may want to allow multiple hosts to fetch requested information.
-          If this is the case, add this line to `settings.py`::
-        
-            TEQUILA_ALLOWED_REQUEST_HOSTS = "the host ip"
-        
-          Ex. : "192.168.1.1|192.168.1.2"
-        
-          Default to None
-        
-        * You can allow guests to log in
-          so add this line to `settings.py`::
-        
-            TEQUILA_ALLOW_GUESTS = True
-        
-          Default value is False
-        
-        
-        Sample app
-        ===========
-        
-        You can find some django app examples in `./django-tequila/sample_app/python3-8-django-2`
-        Add a .env file like the  `./.env.sample` and the run it with Django 2, at the root of the project ::
-        
-            make build init-db
-        
-        
-        Or, for Django 1.11, prefix every make with the DOCKERFILES env set, like this ::
-        
-            DOCKERFILES='-f sample_app/python3-6-django-1/docker-compose.yml' make build init-db
-        
-        Then open `https://127.0.0.1/` in your browser
-        
-        Use `make stop` to shut it down
-        
-        Logging
-        -------
-        
-        Sometimes we struggle to get the aimed result, showing some log may help :
-        
-        * Add and customize as you need this logger to your settings ::
-        
-            'django_tequila': {
-                    'handlers': ['console'],
-                    'level': 'DEBUG',
-                },
-        
-        Debugging
-        ---------
-        
-        * The sample app can be used to debug. We use remote_pdb for this case. Set this snippet in the code ::
-        
-            from remote_pdb import RemotePdb
-            RemotePdb('127.0.0.1', 4445).set_trace()
-        
-        * Then go into the container ::
-        
-            make bash
-        
-        * Finally connect to the debug session with ::
-        
-            telnet 127.0.0.1 4445
-        
-        
-        \(c) All rights reserved. ECOLE POLYTECHNIQUE FEDERALE DE LAUSANNE, Switzerland, VPSI
-        
-Keywords: django,tequila,authentication
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
-Description-Content-Type: text/x-rst
+django-tequila
+==============
+
+`Tequila <http://tequila.epfl.ch/>`_ authentication for django.
+
+
+Requirements
+============
+
+``django-tequila`` needs the Django 3.2+ LTS
+
+This project also expects a fully operational `Tequila <http://tequila.epfl.ch/>`_ server.
+
+Installation
+============
+
+    pip install django-tequila
+
+Configuration
+=============
+
+settings.py
+-----------
+
+* Add at the end of your ``MIDDLEWARE_CLASSES``::
+
+	'django_tequila.middleware.TequilaMiddleware',
+
+* Add to ``INSTALLED_APPS``::
+
+	'django_tequila',
+
+* Add the line::
+
+	AUTHENTICATION_BACKENDS = ('django_tequila.django_backend.TequilaBackend',)
+
+* Set a name that will be displayed on the tequila login page::
+
+	TEQUILA_SERVICE_NAME = "django_tequila_service"
+
+* Finally, add / customize login/logout workflow ::
+
+    LOGIN_URL = "/login"
+    LOGIN_REDIRECT_URL = "/"
+    LOGOUT_URL = '/'
+    LOGIN_REDIRECT_IF_NOT_ALLOWED = "/not_allowed"
+    LOGIN_REDIRECT_TEXT_IF_NOT_ALLOWED  = "Not allowed"
+
+urls.py
+-------
+
+* Add these lines::
+
+	from django_tequila.urls import urlpatterns as django_tequila_urlpatterns
+
+	urlpatterns += django_tequila_urlpatterns
+
+Login/logout links
+------------------
+
+If you want the user to be redirected to a specific page after he logged/logout successfully, you have to add the 'next' parameter to your login url,
+like the default Django authentication backend.
+See `Django help for login-redirect-url <https://docs.djangoproject.com/en/dev/ref/settings/#login-redirect-url>`_ for more information.
+
+
+Profile customization
+---------------------
+You may want to keep some additional information about the user.
+Take a look at `this page <http://docs.djangoproject.com/en/dev/topics/auth/#storing-additional-information-about-users>`_ for more information about profile customization.
+
+Here is an example for a profile for Django 2.0
+
+* Create a custom User model in your `models.py` (see ./sample_app/python3-8-django-2/django_tequila_app/models.py)
+
+* in your `settings.py`, tell django to use your model (see ./sample_app/python3-8-django-2/django_tequila_app/settings.py)::
+    AUTH_USER_MODEL = 'my_app.User'
+    TEQUILA_CUSTOM_USERNAME_ATTRIBUTE = "uniqueid"
+
+
+* Update your database::
+
+	./manage.py syncdb
+
+Site Admin customizations
+-------------------------
+
+- Add or modify your admin.py file, like ./sample_app/python3-8-django-2/django_tequila_app/admin.py
+
+
+Additional tips and settings
+============================
+
+Advanced settings
+-----------------
+
+* If you need to use your personal server, change this parameter::
+
+	TEQUILA_SERVER_URL = "https://tequila.epfl.ch"
+
+* You may want to create an inactive user when someone try to connect to your app. So you can manually control who access it.
+  If this is the case, add this line to `settings.py`::
+
+	TEQUILA_NEW_USER_INACTIVE = True
+
+* You may want to add some custom allow with Tequila.
+  If this is the case, add this line to `settings.py`::
+
+	TEQUILA_CONFIG_ALLOW = 'categorie=shibboleth'
+
+  or, for multiple allow :
+
+	TEQUILA_CONFIG_ALLOW = 'categorie=shibboleth|categorie=epfl-old'
+
+* You may want to add some custom paramaters with Tequila.
+  If this is the case, add this line to `settings.py`::
+
+	TEQUILA_CONFIG_ADDITIONAL = {'allowedorgs': 'EPFL, UNIL'}
+
+* Everytime the user connect trought the Tequila process, he is redirected to an url
+  that has a 'key' parameter. For some esthetic reasons,you may want to remove this parameter,
+  so add this line to `settings.py`::
+
+    TEQUILA_CLEAN_URL = True
+
+  As it creates a redirect to the cleaned address and add an additional page hit, The value by default is False
+
+* You can force a strong authentication
+  so add this line to `settings.py`::
+
+    TEQUILA_STRONG_AUTHENTICATION = True
+
+  Default value is False
+
+* The only value that is truly unique is the sciper ('uniqueid' in Tequila). If your application
+  need a different usage, you can set to a different field (at your own risk though). You can add this line to `settings.py`::
+
+    TEQUILA_CUSTOM_USERNAME_ATTRIBUTE = 'uniqueid'
+
+  Ex. : username, email, etc.
+
+  Default value is username
+
+* You may want to allow multiple hosts to fetch requested information.
+  If this is the case, add this line to `settings.py`::
+
+    TEQUILA_ALLOWED_REQUEST_HOSTS = "the host ip"
+
+  Ex. : "192.168.1.1|192.168.1.2"
+
+  Default to None
+
+* You can allow guests to log in
+  so add this line to `settings.py`::
+
+    TEQUILA_ALLOW_GUESTS = True
+
+  Default value is False
+
+
+Sample app
+===========
+
+You can find some django app examples in `./django-tequila/sample_app/python3-8-django-4`
+Add a .env file like the  `./.env.sample` and the run it with Django 4, at the root of the project ::
+
+    make build init-db
+
+
+Or, for Django 1.11, prefix every make with the DOCKERFILES env set, like this ::
+
+    DOCKERFILES='-f sample_app/python3-6-django-1/docker-compose.yml' make build init-db
+
+Then open `https://127.0.0.1/` in your browser
+
+Use `make logs` if needed, or `make stop` to shut it down
+
+Logging
+-------
+
+Sometimes we struggle to get the aimed result, showing some log may help :
+
+* Add and customize as you need this logger to your settings ::
+
+    'django_tequila': {
+            'handlers': ['console'],
+            'level': 'DEBUG',
+        },
+
+Debugging
+---------
+
+* The sample app can be used to debug. We use remote_pdb for this case. Set this snippet in the code ::
+
+    from remote_pdb import RemotePdb
+    RemotePdb('127.0.0.1', 4445).set_trace()
+
+* Then go into the container ::
+
+    make bash
+
+* Finally connect to the debug session with ::
+
+    telnet 127.0.0.1 4445
+
+
+\(c) All rights reserved. ECOLE POLYTECHNIQUE FEDERALE DE LAUSANNE, Switzerland, VPSI
```

### Comparing `django-tequila-3.4.0/README.rst` & `django-tequila-4.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,39 @@
+Metadata-Version: 2.1
+Name: django-tequila
+Version: 4.0.0
+Summary: A Tequila authentication backend for django
+Home-page: https://github.com/epfl-idevelop/django-tequila
+Author: Julien Delasoie
+Author-email: julien.delasoie@epfl.ch
+License: LGPLv3
+Keywords: django,tequila,authentication
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
+Description-Content-Type: text/x-rst
+License-File: AUTHORS
+
 django-tequila
 ==============
 
 `Tequila <http://tequila.epfl.ch/>`_ authentication for django.
 
 
 Requirements
 ============
 
-``django-tequila`` needs the Django 2.2 LTS
+``django-tequila`` needs the Django 3.2+ LTS
 
 This project also expects a fully operational `Tequila <http://tequila.epfl.ch/>`_ server.
 
 Installation
 ============
 
     pip install django-tequila
@@ -113,15 +135,15 @@
 
 * You may want to add some custom paramaters with Tequila.
   If this is the case, add this line to `settings.py`::
 
 	TEQUILA_CONFIG_ADDITIONAL = {'allowedorgs': 'EPFL, UNIL'}
 
 * Everytime the user connect trought the Tequila process, he is redirected to an url
-  that has a 'key' paramter. For some esthetic reasons,you may want to remove this parameter,
+  that has a 'key' parameter. For some esthetic reasons,you may want to remove this parameter,
   so add this line to `settings.py`::
 
     TEQUILA_CLEAN_URL = True
 
   As it creates a redirect to the cleaned address and add an additional page hit, The value by default is False
 
 * You can force a strong authentication
@@ -156,27 +178,27 @@
 
   Default value is False
 
 
 Sample app
 ===========
 
-You can find some django app examples in `./django-tequila/sample_app/python3-8-django-2`
-Add a .env file like the  `./.env.sample` and the run it with Django 2, at the root of the project ::
+You can find some django app examples in `./django-tequila/sample_app/python3-8-django-4`
+Add a .env file like the  `./.env.sample` and the run it with Django 4, at the root of the project ::
 
     make build init-db
 
 
 Or, for Django 1.11, prefix every make with the DOCKERFILES env set, like this ::
 
     DOCKERFILES='-f sample_app/python3-6-django-1/docker-compose.yml' make build init-db
 
 Then open `https://127.0.0.1/` in your browser
 
-Use `make stop` to shut it down
+Use `make logs` if needed, or `make stop` to shut it down
 
 Logging
 -------
 
 Sometimes we struggle to get the aimed result, showing some log may help :
 
 * Add and customize as you need this logger to your settings ::
@@ -200,7 +222,9 @@
 
 * Finally connect to the debug session with ::
 
     telnet 127.0.0.1 4445
 
 
 \(c) All rights reserved. ECOLE POLYTECHNIQUE FEDERALE DE LAUSANNE, Switzerland, VPSI
+
+
```

### Comparing `django-tequila-3.4.0/django_tequila/admin.py` & `django-tequila-4.0.0/django_tequila/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from functools import update_wrapper
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.contrib.admin.sites import AdminSite
 from django.contrib.auth import REDIRECT_FIELD_NAME
 from django.http import HttpResponseForbidden, HttpResponseRedirect, QueryDict
+from django.utils.decorators import method_decorator
 from django.views.decorators.cache import never_cache
 from django.views.decorators.csrf import csrf_protect
 
 
 class TequilaAdminSite(AdminSite):
     def admin_view(self, view, cacheable=False):
         """
@@ -37,15 +38,15 @@
             inner = never_cache(inner)
         # We add csrf_protect here so this function can be used as a utility
         # function for any view, without having to repeat 'csrf_protect'.
         if not getattr(view, 'csrf_exempt', False):
             inner = csrf_protect(inner)
         return update_wrapper(inner, view)
 
-    @never_cache
+    @method_decorator(never_cache)
     def login(self, request, extra_context=None):
         """
         Don't display the login form, use the Tequila login process instead
         """
         # user is not logged, so redirect to the real login
         try:
             login_url = settings.LOGIN_URL
```

### Comparing `django-tequila-3.4.0/django_tequila/django_backend/__init__.py` & `django-tequila-4.0.0/django_tequila/django_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/django_tequila/middleware.py` & `django-tequila-4.0.0/django_tequila/middleware.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/django_tequila/tequila_auth_views/__init__.py` & `django-tequila-4.0.0/django_tequila/tequila_auth_views/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 """
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth import REDIRECT_FIELD_NAME
 
 from django.http import HttpResponse, HttpResponseRedirect
 from django.views.decorators.cache import never_cache
-from django.utils.http import is_safe_url
+from django.utils.http import url_has_allowed_host_and_scheme
 from django.conf import settings
 
 from django_tequila.tequila_client import TequilaClient
 from django_tequila.tequila_client import EPFLConfig
 
 
 
 User = get_user_model()
 
 
 def get_redirect_url(request):
     """Return the user-originating redirect URL if it's safe."""
     redirect_to = request.GET.get(REDIRECT_FIELD_NAME)
 
-    url_is_safe = is_safe_url(
+    url_is_safe = url_has_allowed_host_and_scheme(
         url=redirect_to,
         allowed_hosts=request.get_host(),
         require_https=request.is_secure(),
     )
     return redirect_to if url_is_safe else ''
```

### Comparing `django-tequila-3.4.0/django_tequila/tequila_client/client.py` & `django-tequila-4.0.0/django_tequila/tequila_client/client.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/django_tequila/tequila_client/config.py` & `django-tequila-4.0.0/django_tequila/tequila_client/config.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/django_tequila.egg-info/PKG-INFO` & `django-tequila-4.0.0/django_tequila.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,227 +1,230 @@
 Metadata-Version: 2.1
 Name: django-tequila
-Version: 3.4.0
+Version: 4.0.0
 Summary: A Tequila authentication backend for django
 Home-page: https://github.com/epfl-idevelop/django-tequila
 Author: Julien Delasoie
 Author-email: julien.delasoie@epfl.ch
 License: LGPLv3
-Description: django-tequila
-        ==============
-        
-        `Tequila <http://tequila.epfl.ch/>`_ authentication for django.
-        
-        
-        Requirements
-        ============
-        
-        ``django-tequila`` needs the Django 2.2 LTS
-        
-        This project also expects a fully operational `Tequila <http://tequila.epfl.ch/>`_ server.
-        
-        Installation
-        ============
-        
-            pip install django-tequila
-        
-        Configuration
-        =============
-        
-        settings.py
-        -----------
-        
-        * Add at the end of your ``MIDDLEWARE_CLASSES``::
-        
-        	'django_tequila.middleware.TequilaMiddleware',
-        
-        * Add to ``INSTALLED_APPS``::
-        
-        	'django_tequila',
-        
-        * Add the line::
-        
-        	AUTHENTICATION_BACKENDS = ('django_tequila.django_backend.TequilaBackend',)
-        
-        * Set a name that will be displayed on the tequila login page::
-        
-        	TEQUILA_SERVICE_NAME = "django_tequila_service"
-        
-        * Finally, add / customize login/logout workflow ::
-        
-            LOGIN_URL = "/login"
-            LOGIN_REDIRECT_URL = "/"
-            LOGOUT_URL = '/'
-            LOGIN_REDIRECT_IF_NOT_ALLOWED = "/not_allowed"
-            LOGIN_REDIRECT_TEXT_IF_NOT_ALLOWED  = "Not allowed"
-        
-        urls.py
-        -------
-        
-        * Add these lines::
-        
-        	from django_tequila.urls import urlpatterns as django_tequila_urlpatterns
-        
-        	urlpatterns += django_tequila_urlpatterns
-        
-        Login/logout links
-        ------------------
-        
-        If you want the user to be redirected to a specific page after he logged/logout successfully, you have to add the 'next' parameter to your login url,
-        like the default Django authentication backend.
-        See `Django help for login-redirect-url <https://docs.djangoproject.com/en/dev/ref/settings/#login-redirect-url>`_ for more information.
-        
-        
-        Profile customization
-        ---------------------
-        You may want to keep some additional information about the user.
-        Take a look at `this page <http://docs.djangoproject.com/en/dev/topics/auth/#storing-additional-information-about-users>`_ for more information about profile customization.
-        
-        Here is an example for a profile for Django 2.0
-        
-        * Create a custom User model in your `models.py` (see ./sample_app/python3-8-django-2/django_tequila_app/models.py)
-        
-        * in your `settings.py`, tell django to use your model (see ./sample_app/python3-8-django-2/django_tequila_app/settings.py)::
-            AUTH_USER_MODEL = 'my_app.User'
-            TEQUILA_CUSTOM_USERNAME_ATTRIBUTE = "uniqueid"
-        
-        
-        * Update your database::
-        
-        	./manage.py syncdb
-        
-        Site Admin customizations
-        -------------------------
-        
-        - Add or modify your admin.py file, like ./sample_app/python3-8-django-2/django_tequila_app/admin.py
-        
-        
-        Additional tips and settings
-        ============================
-        
-        Advanced settings
-        -----------------
-        
-        * If you need to use your personal server, change this parameter::
-        
-        	TEQUILA_SERVER_URL = "https://tequila.epfl.ch"
-        
-        * You may want to create an inactive user when someone try to connect to your app. So you can manually control who access it.
-          If this is the case, add this line to `settings.py`::
-        
-        	TEQUILA_NEW_USER_INACTIVE = True
-        
-        * You may want to add some custom allow with Tequila.
-          If this is the case, add this line to `settings.py`::
-        
-        	TEQUILA_CONFIG_ALLOW = 'categorie=shibboleth'
-        
-          or, for multiple allow :
-        
-        	TEQUILA_CONFIG_ALLOW = 'categorie=shibboleth|categorie=epfl-old'
-        
-        * You may want to add some custom paramaters with Tequila.
-          If this is the case, add this line to `settings.py`::
-        
-        	TEQUILA_CONFIG_ADDITIONAL = {'allowedorgs': 'EPFL, UNIL'}
-        
-        * Everytime the user connect trought the Tequila process, he is redirected to an url
-          that has a 'key' paramter. For some esthetic reasons,you may want to remove this parameter,
-          so add this line to `settings.py`::
-        
-            TEQUILA_CLEAN_URL = True
-        
-          As it creates a redirect to the cleaned address and add an additional page hit, The value by default is False
-        
-        * You can force a strong authentication
-          so add this line to `settings.py`::
-        
-            TEQUILA_STRONG_AUTHENTICATION = True
-        
-          Default value is False
-        
-        * The only value that is truly unique is the sciper ('uniqueid' in Tequila). If your application
-          need a different usage, you can set to a different field (at your own risk though). You can add this line to `settings.py`::
-        
-            TEQUILA_CUSTOM_USERNAME_ATTRIBUTE = 'uniqueid'
-        
-          Ex. : username, email, etc.
-        
-          Default value is username
-        
-        * You may want to allow multiple hosts to fetch requested information.
-          If this is the case, add this line to `settings.py`::
-        
-            TEQUILA_ALLOWED_REQUEST_HOSTS = "the host ip"
-        
-          Ex. : "192.168.1.1|192.168.1.2"
-        
-          Default to None
-        
-        * You can allow guests to log in
-          so add this line to `settings.py`::
-        
-            TEQUILA_ALLOW_GUESTS = True
-        
-          Default value is False
-        
-        
-        Sample app
-        ===========
-        
-        You can find some django app examples in `./django-tequila/sample_app/python3-8-django-2`
-        Add a .env file like the  `./.env.sample` and the run it with Django 2, at the root of the project ::
-        
-            make build init-db
-        
-        
-        Or, for Django 1.11, prefix every make with the DOCKERFILES env set, like this ::
-        
-            DOCKERFILES='-f sample_app/python3-6-django-1/docker-compose.yml' make build init-db
-        
-        Then open `https://127.0.0.1/` in your browser
-        
-        Use `make stop` to shut it down
-        
-        Logging
-        -------
-        
-        Sometimes we struggle to get the aimed result, showing some log may help :
-        
-        * Add and customize as you need this logger to your settings ::
-        
-            'django_tequila': {
-                    'handlers': ['console'],
-                    'level': 'DEBUG',
-                },
-        
-        Debugging
-        ---------
-        
-        * The sample app can be used to debug. We use remote_pdb for this case. Set this snippet in the code ::
-        
-            from remote_pdb import RemotePdb
-            RemotePdb('127.0.0.1', 4445).set_trace()
-        
-        * Then go into the container ::
-        
-            make bash
-        
-        * Finally connect to the debug session with ::
-        
-            telnet 127.0.0.1 4445
-        
-        
-        \(c) All rights reserved. ECOLE POLYTECHNIQUE FEDERALE DE LAUSANNE, Switzerland, VPSI
-        
 Keywords: django,tequila,authentication
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Description-Content-Type: text/x-rst
+License-File: AUTHORS
+
+django-tequila
+==============
+
+`Tequila <http://tequila.epfl.ch/>`_ authentication for django.
+
+
+Requirements
+============
+
+``django-tequila`` needs the Django 3.2+ LTS
+
+This project also expects a fully operational `Tequila <http://tequila.epfl.ch/>`_ server.
+
+Installation
+============
+
+    pip install django-tequila
+
+Configuration
+=============
+
+settings.py
+-----------
+
+* Add at the end of your ``MIDDLEWARE_CLASSES``::
+
+	'django_tequila.middleware.TequilaMiddleware',
+
+* Add to ``INSTALLED_APPS``::
+
+	'django_tequila',
+
+* Add the line::
+
+	AUTHENTICATION_BACKENDS = ('django_tequila.django_backend.TequilaBackend',)
+
+* Set a name that will be displayed on the tequila login page::
+
+	TEQUILA_SERVICE_NAME = "django_tequila_service"
+
+* Finally, add / customize login/logout workflow ::
+
+    LOGIN_URL = "/login"
+    LOGIN_REDIRECT_URL = "/"
+    LOGOUT_URL = '/'
+    LOGIN_REDIRECT_IF_NOT_ALLOWED = "/not_allowed"
+    LOGIN_REDIRECT_TEXT_IF_NOT_ALLOWED  = "Not allowed"
+
+urls.py
+-------
+
+* Add these lines::
+
+	from django_tequila.urls import urlpatterns as django_tequila_urlpatterns
+
+	urlpatterns += django_tequila_urlpatterns
+
+Login/logout links
+------------------
+
+If you want the user to be redirected to a specific page after he logged/logout successfully, you have to add the 'next' parameter to your login url,
+like the default Django authentication backend.
+See `Django help for login-redirect-url <https://docs.djangoproject.com/en/dev/ref/settings/#login-redirect-url>`_ for more information.
+
+
+Profile customization
+---------------------
+You may want to keep some additional information about the user.
+Take a look at `this page <http://docs.djangoproject.com/en/dev/topics/auth/#storing-additional-information-about-users>`_ for more information about profile customization.
+
+Here is an example for a profile for Django 2.0
+
+* Create a custom User model in your `models.py` (see ./sample_app/python3-8-django-2/django_tequila_app/models.py)
+
+* in your `settings.py`, tell django to use your model (see ./sample_app/python3-8-django-2/django_tequila_app/settings.py)::
+    AUTH_USER_MODEL = 'my_app.User'
+    TEQUILA_CUSTOM_USERNAME_ATTRIBUTE = "uniqueid"
+
+
+* Update your database::
+
+	./manage.py syncdb
+
+Site Admin customizations
+-------------------------
+
+- Add or modify your admin.py file, like ./sample_app/python3-8-django-2/django_tequila_app/admin.py
+
+
+Additional tips and settings
+============================
+
+Advanced settings
+-----------------
+
+* If you need to use your personal server, change this parameter::
+
+	TEQUILA_SERVER_URL = "https://tequila.epfl.ch"
+
+* You may want to create an inactive user when someone try to connect to your app. So you can manually control who access it.
+  If this is the case, add this line to `settings.py`::
+
+	TEQUILA_NEW_USER_INACTIVE = True
+
+* You may want to add some custom allow with Tequila.
+  If this is the case, add this line to `settings.py`::
+
+	TEQUILA_CONFIG_ALLOW = 'categorie=shibboleth'
+
+  or, for multiple allow :
+
+	TEQUILA_CONFIG_ALLOW = 'categorie=shibboleth|categorie=epfl-old'
+
+* You may want to add some custom paramaters with Tequila.
+  If this is the case, add this line to `settings.py`::
+
+	TEQUILA_CONFIG_ADDITIONAL = {'allowedorgs': 'EPFL, UNIL'}
+
+* Everytime the user connect trought the Tequila process, he is redirected to an url
+  that has a 'key' parameter. For some esthetic reasons,you may want to remove this parameter,
+  so add this line to `settings.py`::
+
+    TEQUILA_CLEAN_URL = True
+
+  As it creates a redirect to the cleaned address and add an additional page hit, The value by default is False
+
+* You can force a strong authentication
+  so add this line to `settings.py`::
+
+    TEQUILA_STRONG_AUTHENTICATION = True
+
+  Default value is False
+
+* The only value that is truly unique is the sciper ('uniqueid' in Tequila). If your application
+  need a different usage, you can set to a different field (at your own risk though). You can add this line to `settings.py`::
+
+    TEQUILA_CUSTOM_USERNAME_ATTRIBUTE = 'uniqueid'
+
+  Ex. : username, email, etc.
+
+  Default value is username
+
+* You may want to allow multiple hosts to fetch requested information.
+  If this is the case, add this line to `settings.py`::
+
+    TEQUILA_ALLOWED_REQUEST_HOSTS = "the host ip"
+
+  Ex. : "192.168.1.1|192.168.1.2"
+
+  Default to None
+
+* You can allow guests to log in
+  so add this line to `settings.py`::
+
+    TEQUILA_ALLOW_GUESTS = True
+
+  Default value is False
+
+
+Sample app
+===========
+
+You can find some django app examples in `./django-tequila/sample_app/python3-8-django-4`
+Add a .env file like the  `./.env.sample` and the run it with Django 4, at the root of the project ::
+
+    make build init-db
+
+
+Or, for Django 1.11, prefix every make with the DOCKERFILES env set, like this ::
+
+    DOCKERFILES='-f sample_app/python3-6-django-1/docker-compose.yml' make build init-db
+
+Then open `https://127.0.0.1/` in your browser
+
+Use `make logs` if needed, or `make stop` to shut it down
+
+Logging
+-------
+
+Sometimes we struggle to get the aimed result, showing some log may help :
+
+* Add and customize as you need this logger to your settings ::
+
+    'django_tequila': {
+            'handlers': ['console'],
+            'level': 'DEBUG',
+        },
+
+Debugging
+---------
+
+* The sample app can be used to debug. We use remote_pdb for this case. Set this snippet in the code ::
+
+    from remote_pdb import RemotePdb
+    RemotePdb('127.0.0.1', 4445).set_trace()
+
+* Then go into the container ::
+
+    make bash
+
+* Finally connect to the debug session with ::
+
+    telnet 127.0.0.1 4445
+
+
+\(c) All rights reserved. ECOLE POLYTECHNIQUE FEDERALE DE LAUSANNE, Switzerland, VPSI
+
+
```

### Comparing `django-tequila-3.4.0/django_tequila.egg-info/SOURCES.txt` & `django-tequila-4.0.0/django_tequila.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+AUTHORS
 MANIFEST.in
 README.rst
 setup.py
 django_tequila/__init__.py
 django_tequila/admin.py
 django_tequila/middleware.py
 django_tequila/urls.py
@@ -39,17 +40,14 @@
 sample_app/python3-6-django-1/userprofile/tests.py
 sample_app/python3-6-django-1/userprofile/views.py
 sample_app/python3-6-django-1/userprofile/migrations/0001_initial.py
 sample_app/python3-6-django-1/userprofile/migrations/0002_auto_20210201_1010.py
 sample_app/python3-6-django-1/userprofile/migrations/__init__.py
 sample_app/python3-8-django-2/docker-compose.yml
 sample_app/python3-8-django-2/manage.py
-sample_app/python3-8-django-2/.pytest_cache/.gitignore
-sample_app/python3-8-django-2/.pytest_cache/CACHEDIR.TAG
-sample_app/python3-8-django-2/.pytest_cache/README.md
 sample_app/python3-8-django-2/django_tequila_app/__init__.py
 sample_app/python3-8-django-2/django_tequila_app/admin.py
 sample_app/python3-8-django-2/django_tequila_app/database.db
 sample_app/python3-8-django-2/django_tequila_app/models.py
 sample_app/python3-8-django-2/django_tequila_app/settings.py
 sample_app/python3-8-django-2/django_tequila_app/urls.py
 sample_app/python3-8-django-2/django_tequila_app/views.py
@@ -57,8 +55,27 @@
 sample_app/python3-8-django-2/django_tequila_app/migrations/0001_initial.py
 sample_app/python3-8-django-2/django_tequila_app/migrations/__init__.py
 sample_app/python3-8-django-2/django_tequila_app/requirements/base.txt
 sample_app/python3-8-django-2/django_tequila_app/templates/index.html
 sample_app/python3-8-django-2/django_tequila_app/templates/unprotected_view.html
 sample_app/python3-8-django-2/django_tequila_app/tests/__init__.py
 sample_app/python3-8-django-2/django_tequila_app/tests/test_django.py
-sample_app/python3-8-django-2/django_tequila_app/tests/test_selenium.py
+sample_app/python3-8-django-2/django_tequila_app/tests/test_selenium.py
+sample_app/python3-8-django-4/docker-compose.yml
+sample_app/python3-8-django-4/manage.py
+sample_app/python3-8-django-4/django_tequila_app/__init__.py
+sample_app/python3-8-django-4/django_tequila_app/admin.py
+sample_app/python3-8-django-4/django_tequila_app/asgi.py
+sample_app/python3-8-django-4/django_tequila_app/database.db
+sample_app/python3-8-django-4/django_tequila_app/models.py
+sample_app/python3-8-django-4/django_tequila_app/settings.py
+sample_app/python3-8-django-4/django_tequila_app/urls.py
+sample_app/python3-8-django-4/django_tequila_app/views.py
+sample_app/python3-8-django-4/django_tequila_app/wsgi.py
+sample_app/python3-8-django-4/django_tequila_app/migrations/0001_initial.py
+sample_app/python3-8-django-4/django_tequila_app/migrations/__init__.py
+sample_app/python3-8-django-4/django_tequila_app/requirements/base.txt
+sample_app/python3-8-django-4/django_tequila_app/templates/index.html
+sample_app/python3-8-django-4/django_tequila_app/templates/unprotected_view.html
+sample_app/python3-8-django-4/django_tequila_app/tests/__init__.py
+sample_app/python3-8-django-4/django_tequila_app/tests/test_django.py
+sample_app/python3-8-django-4/django_tequila_app/tests/test_selenium.py
```

### Comparing `django-tequila-3.4.0/sample_app/create_superadmin.py` & `django-tequila-4.0.0/sample_app/create_superadmin.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/database.db` & `django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/database.db`

 * *Files 11% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -1,32 +1,35 @@
 PRAGMA foreign_keys=OFF;
 BEGIN TRANSACTION;
 CREATE TABLE IF NOT EXISTS "django_migrations" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "app" varchar(255) NOT NULL, "name" varchar(255) NOT NULL, "applied" datetime NOT NULL);
-INSERT INTO django_migrations VALUES(1,'contenttypes','0001_initial','2021-01-19 15:54:05.693972');
-INSERT INTO django_migrations VALUES(2,'auth','0001_initial','2021-01-19 15:54:05.724608');
-INSERT INTO django_migrations VALUES(3,'admin','0001_initial','2021-01-19 15:54:05.742355');
-INSERT INTO django_migrations VALUES(4,'admin','0002_logentry_remove_auto_add','2021-01-19 15:54:05.760272');
-INSERT INTO django_migrations VALUES(5,'contenttypes','0002_remove_content_type_name','2021-01-19 15:54:05.790698');
-INSERT INTO django_migrations VALUES(6,'auth','0002_alter_permission_name_max_length','2021-01-19 15:54:05.805372');
-INSERT INTO django_migrations VALUES(7,'auth','0003_alter_user_email_max_length','2021-01-19 15:54:05.822959');
-INSERT INTO django_migrations VALUES(8,'auth','0004_alter_user_username_opts','2021-01-19 15:54:05.839748');
-INSERT INTO django_migrations VALUES(9,'auth','0005_alter_user_last_login_null','2021-01-19 15:54:05.856728');
-INSERT INTO django_migrations VALUES(10,'auth','0006_require_contenttypes_0002','2021-01-19 15:54:05.861588');
-INSERT INTO django_migrations VALUES(11,'auth','0007_alter_validators_add_error_messages','2021-01-19 15:54:05.878524');
-INSERT INTO django_migrations VALUES(12,'auth','0008_alter_user_username_max_length','2021-01-19 15:54:05.895731');
-INSERT INTO django_migrations VALUES(13,'sessions','0001_initial','2021-01-19 15:54:05.907847');
-INSERT INTO django_migrations VALUES(14,'sites','0001_initial','2021-01-19 15:54:05.918996');
-INSERT INTO django_migrations VALUES(15,'sites','0002_alter_domain_unique','2021-01-19 15:54:05.932973');
-INSERT INTO django_migrations VALUES(16,'userprofile','0001_initial','2021-01-19 15:54:05.953892');
-INSERT INTO django_migrations VALUES(17,'userprofile','0002_auto_20210201_1010','2021-02-01 10:10:58.722634');
+INSERT INTO django_migrations VALUES(1,'contenttypes','0001_initial','2021-01-21 15:25:27.560894');
+INSERT INTO django_migrations VALUES(2,'auth','0001_initial','2021-01-21 15:25:27.608535');
+INSERT INTO django_migrations VALUES(3,'admin','0001_initial','2021-01-21 15:25:27.633686');
+INSERT INTO django_migrations VALUES(4,'admin','0002_logentry_remove_auto_add','2021-01-21 15:25:27.659985');
+INSERT INTO django_migrations VALUES(5,'contenttypes','0002_remove_content_type_name','2021-01-21 15:25:27.710927');
+INSERT INTO django_migrations VALUES(6,'auth','0002_alter_permission_name_max_length','2021-01-21 15:25:27.730631');
+INSERT INTO django_migrations VALUES(7,'auth','0003_alter_user_email_max_length','2021-01-21 15:25:27.758934');
+INSERT INTO django_migrations VALUES(8,'auth','0004_alter_user_username_opts','2021-01-21 15:25:27.786721');
+INSERT INTO django_migrations VALUES(9,'auth','0005_alter_user_last_login_null','2021-01-21 15:25:27.817946');
+INSERT INTO django_migrations VALUES(10,'auth','0006_require_contenttypes_0002','2021-01-21 15:25:27.824105');
+INSERT INTO django_migrations VALUES(11,'auth','0007_alter_validators_add_error_messages','2021-01-21 15:25:27.849606');
+INSERT INTO django_migrations VALUES(12,'auth','0008_alter_user_username_max_length','2021-01-21 15:25:27.878018');
+INSERT INTO django_migrations VALUES(13,'sessions','0001_initial','2021-01-21 15:25:27.896271');
+INSERT INTO django_migrations VALUES(14,'sites','0001_initial','2021-01-21 15:25:27.911659');
+INSERT INTO django_migrations VALUES(15,'sites','0002_alter_domain_unique','2021-01-21 15:25:27.929910');
+INSERT INTO django_migrations VALUES(16,'userprofile','0001_initial','2021-01-21 15:25:27.960808');
 CREATE TABLE IF NOT EXISTS "auth_group" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(80) NOT NULL UNIQUE);
 CREATE TABLE IF NOT EXISTS "auth_group_permissions" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "group_id" integer NOT NULL REFERENCES "auth_group" ("id"), "permission_id" integer NOT NULL REFERENCES "auth_permission__old" ("id"));
 CREATE TABLE IF NOT EXISTS "auth_user_groups" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "user_id" integer NOT NULL REFERENCES "auth_user__old" ("id"), "group_id" integer NOT NULL REFERENCES "auth_group" ("id"));
 CREATE TABLE IF NOT EXISTS "auth_user_user_permissions" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "user_id" integer NOT NULL REFERENCES "auth_user__old" ("id"), "permission_id" integer NOT NULL REFERENCES "auth_permission__old" ("id"));
 CREATE TABLE IF NOT EXISTS "django_admin_log" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "object_id" text NULL, "object_repr" varchar(200) NOT NULL, "action_flag" smallint unsigned NOT NULL, "change_message" text NOT NULL, "content_type_id" integer NULL REFERENCES "django_content_type__old" ("id"), "user_id" integer NOT NULL REFERENCES "auth_user__old" ("id"), "action_time" datetime NOT NULL);
+INSERT INTO django_admin_log VALUES(1,'3','UserProfile object',3,'',8,1,'2021-01-21 16:10:34.671390');
+INSERT INTO django_admin_log VALUES(2,'3','julien.delasoie',3,'',4,1,'2021-01-21 16:10:48.855741');
+INSERT INTO django_admin_log VALUES(3,'4','UserProfile object',3,'',8,1,'2021-01-21 16:13:39.974797');
+INSERT INTO django_admin_log VALUES(4,'4','julien.delasoie',3,'',4,1,'2021-01-21 16:13:52.941418');
 CREATE TABLE IF NOT EXISTS "django_content_type" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "app_label" varchar(100) NOT NULL, "model" varchar(100) NOT NULL);
 INSERT INTO django_content_type VALUES(1,'admin','logentry');
 INSERT INTO django_content_type VALUES(2,'auth','permission');
 INSERT INTO django_content_type VALUES(3,'auth','group');
 INSERT INTO django_content_type VALUES(4,'auth','user');
 INSERT INTO django_content_type VALUES(5,'contenttypes','contenttype');
 INSERT INTO django_content_type VALUES(6,'sessions','session');
@@ -54,29 +57,34 @@
 INSERT INTO auth_permission VALUES(19,7,'add_site','Can add site');
 INSERT INTO auth_permission VALUES(20,7,'change_site','Can change site');
 INSERT INTO auth_permission VALUES(21,7,'delete_site','Can delete site');
 INSERT INTO auth_permission VALUES(22,8,'add_userprofile','Can add user profile');
 INSERT INTO auth_permission VALUES(23,8,'change_userprofile','Can change user profile');
 INSERT INTO auth_permission VALUES(24,8,'delete_userprofile','Can delete user profile');
 CREATE TABLE IF NOT EXISTS "auth_user" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "password" varchar(128) NOT NULL, "last_login" datetime NULL, "is_superuser" bool NOT NULL, "first_name" varchar(30) NOT NULL, "last_name" varchar(30) NOT NULL, "email" varchar(254) NOT NULL, "is_staff" bool NOT NULL, "is_active" bool NOT NULL, "date_joined" datetime NOT NULL, "username" varchar(150) NOT NULL UNIQUE);
-INSERT INTO auth_user VALUES(3,'!Vh4rGKxrYBEus2L0k4bNyUVJWuCHaVbWazcrWKuz','2021-02-01 12:38:36.644942',1,'Julien','Delasoie','julien.delasoie@epfl.ch',1,1,'2021-02-01 10:10:59.399122','delasoie');
+INSERT INTO auth_user VALUES(1,'!IbQ9sgHyoxjeUeJhKQ9mcJP3IMJl4prgVjeqqQTp','2021-01-21 15:45:30.818068',1,'Julien','Delasoie','julien.delasoie@epfl.ch',1,1,'2021-01-21 15:25:29.419260','delasoie');
+INSERT INTO auth_user VALUES(2,'','2021-01-21 16:14:00.489227',0,'Julien-Ext','Delasoie-Ext','julien.delasoie@ubiko.ch',0,1,'2021-01-21 16:14:00.454700','julien.delasoie');
 CREATE TABLE IF NOT EXISTS "django_session" ("session_key" varchar(40) NOT NULL PRIMARY KEY, "session_data" text NOT NULL, "expire_date" datetime NOT NULL);
-INSERT INTO django_session VALUES('0e6zlhxnvhvd8e2g9d35oe91ymj8dzhd','N2JlM2QzNmFkNzkwOWIxNmFkMTM5NmE0MzYyMTQwNDE3OThjYzBmMzp7Il9hdXRoX3VzZXJfaWQiOiIzIiwiX2F1dGhfdXNlcl9iYWNrZW5kIjoiZGphbmdvX3RlcXVpbGEuZGphbmdvX2JhY2tlbmQuVGVxdWlsYUJhY2tlbmQiLCJfYXV0aF91c2VyX2hhc2giOiI4MzAzODlmYzE5MTkzMTM4NGIwNmEwZmFiZGE1Yjg4ZjZlZTA1NjdjIn0=','2021-02-15 12:38:36.650975');
+INSERT INTO django_session VALUES('lm0d0k1wtypxpwgme1oxlxknsgzkvto9','NDNhNGY1ZDUwMTFjMWE1YmNkMmZkY2Y0MmRmNWFhNmYzMjlkMDA4NTp7InRlc3Rjb29raWUiOiJ3b3JrZWQiLCJfYXV0aF91c2VyX2lkIjoiMSIsIl9hdXRoX3VzZXJfYmFja2VuZCI6ImRqYW5nb190ZXF1aWxhLmRqYW5nb19iYWNrZW5kLlRlcXVpbGFCYWNrZW5kIiwiX2F1dGhfdXNlcl9oYXNoIjoiMDljZjQ5ZTdjMDM2YWE5M2MyMjM4MDhhYjU5MjA3MjRkY2M0MjAwZiJ9','2021-02-04 15:43:56.657129');
+INSERT INTO django_session VALUES('ibbqgwlon6h4mraok5y9dt34vibl3cwd','MWViODRhNzE3ZDcxNzkwZWYxM2E4MjZjMmMwYmUzMmYxZjA1NmRkYzp7Il9hdXRoX3VzZXJfaWQiOiIyIiwiX2F1dGhfdXNlcl9iYWNrZW5kIjoiZGphbmdvX3RlcXVpbGEuZGphbmdvX2JhY2tlbmQuVGVxdWlsYUJhY2tlbmQiLCJfYXV0aF91c2VyX2hhc2giOiI4NzJjMjUwZGY2MzA1YjY3YzMyODNhNTMwZDIwMWVkMDc2NGE2MmQ2In0=','2021-02-04 16:14:00.498859');
 CREATE TABLE IF NOT EXISTS "django_site" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(50) NOT NULL, "domain" varchar(100) NOT NULL UNIQUE);
 INSERT INTO django_site VALUES(1,'example.com','example.com');
-CREATE TABLE IF NOT EXISTS "userprofile_userprofile" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "where" varchar(200) NULL, "units" text NULL, "group" text NULL, "classe" varchar(100) NULL, "statut" varchar(100) NULL, "memberof" text NULL, "user_id" integer NULL UNIQUE REFERENCES "auth_user" ("id"), "sciper" varchar(10) NULL UNIQUE);
-INSERT INTO userprofile_userprofile VALUES(3,'IDEV-FSD/IDEV/VPO-SI/EPFL/CH','idev-fsd','AA_test,Cartographie-Read,ChronosUtilisateurs,Collaborateurs-VPSI-INN,DIT,DIT_ServiceNOW_Agents,DjangoFamily,IDEV-JIRA,IDEVELOP,IDEVELOP-SICO-Guest,IDEVFSD-SICO-Guest,INSTANT-LAB2,WP-SuperAdmin,WP_Monitoring,accounts-tequila-example,actu-api-rest-consumers,alerts-wwp-prod,arh-epfl,awx-poc-openshift-wwp-test,book_calendar_room_DIT,book_calendar_room_INN,book_calendar_room_PB,boussole,c4science-tech,cold-wiki,dashboard-exopge-access,dit-sup.agents_otrs,docker-vpsi,eml-infoscience,exopge-openshift-users,gr-lsm-infoscience,idev-fsd-membres,idev-fsd-wordpress,idevfsd-test-conferences-wp-admins,infoscience-dev,infoscience-exports-role-editor,infoscience-exports-role-viewer,infoscience-librarians,infoscience-lmc,infoscience-mics,infoscience-superadmin,infoscience-upfahl,infoscience_LME,innovation,intranet-epfl,mediatheque-celum5,memento-api-rest-consumers,metrics-exopge-access,personnel-epfl,personnel-kis,poc-cms-rancher-admins,respinfo-epfl,sdf-gitlab,sdf-openshift,sdf-openstack,sre-epfl,vpsi-docker,vra_p_idevfsd,vra_p_peopl,wp-dev,wp-polylex-admins,wp-veritas-admins,wwp-infra-role-editor,wwp-infra-role-tag-image,wwp-infra-role-viewer,wwp-int-role-editor,wwp-int-role-viewer,wwp-members,wwp-role-editor,wwp-role-viewer,wwp-test-role-editor,wwp-test-role-viewer','Personnel technique/administratif','Personnel','S00167,S00188,S02104,S06362,S07309,S08502,S08780,S08781,S08782,S13906,S14034,S14089,U12635,U10000,S00000,S14149,S14235,S11115,S09180,S07954,S08652,S07431,S07414,S05034,S14375,S14368,U13030,U13028,S14524,S14590,S14717,S16412,S16455,S16524,S16510,S14835,S14320,S17367,S17456,S17591,S17207,S17124,S17876,S18064,S18110,S18492,S17128,S18482,S18723,S19119,S20418,S19590,S20620,S20697,S20797,S20882,S20477,S21068,S21137,S21316,S21520,S21474,S21476,S21477,S21479,S21480,S21470,S21471,S22104,S22268,S22409,S22426,S22451,S22274,S22874,S22639,S18944,S22954,S22979,S22980,S23510,S23511,S21473,S19070,S27282',3,'194044');
+CREATE TABLE IF NOT EXISTS "userprofile_userprofile" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "sciper" varchar(10) NULL, "where" varchar(200) NULL, "units" text NULL, "group" text NULL, "classe" varchar(100) NULL, "statut" varchar(100) NULL, "memberof" text NULL, "user_id" integer NULL UNIQUE REFERENCES "auth_user" ("id"));
+INSERT INTO userprofile_userprofile VALUES(1,'194044','IDEV-FSD/SI-IDEV/SI/EPFL/CH','idev-fsd','Cartographie-Read,Collaborateurs-VPSI-INN,DIT,DIT_ServiceNOW_Agents,DjangoFamily,IDEV-JIRA,IDEVELOP,IDEVELOP-SICO-Guest,INSTANT-LAB2,SI-Notif-Incident-Majeur,WP_Monitoring,book_calendar_room_DIT,book_calendar_room_INN,boussole,c4science-tech,dashboard-exopge-access,dit-sup.agents_otrs,eml-infoscience,exopge-openshift-users,gr-lsm-infoscience,infoscience-dev,infoscience-librarians,infoscience-lmc,infoscience-mics,infoscience-superadmin,infoscience-upfahl,infoscience_LME,innovation,intranet-epfl,mediatheque-celum5,metrics-exopge-access,personnel-epfl,personnel-kis,poc-cms-rancher-admins,respinfo-epfl,sdf-gitlab,sdf-openshift,sdf-openstack,sre-epfl,wwp-members,IDEVFSD-SICO-Guest,idev-fsd-wordpress,arh-epfl,vpsi-docker,docker-vpsi,book_calendar_room_PB,awx-poc-openshift-wwp-test,idev-fsd-membres,wp-dev,wwp-infra-role-tag-image,wwp-infra-role-viewer,wwp-int-role-editor,wwp-int-role-viewer,wwp-test-role-editor,wwp-test-role-viewer,wwp-role-editor,wwp-role-viewer,idevfsd-test-conferences-wp-admins,wp-veritas-admins,accounts-tequila-example,vra_p_peopl,vra_p_idevfsd,wp-polylex-admins,ChronosUtilisateurs,alerts-wwp-prod,AA_test,infoscience-exports-role-editor,infoscience-exports-role-viewer,actu-api-rest-consumers,memento-api-rest-consumers,wwp-infra-role-editor,WP-SuperAdmin,cold-wiki','Personnel technique/administratif','Personnel','S00167,S00188,S02104,S06362,S07309,S08502,S08780,S08781,S08782,S13906,S14034,S14089,U12635,U10000,S00000,S14149,S14235,S11115,S09180,S07954,S08652,S07431,S07414,S05034,S14375,S14368,U13030,U13028,S14524,S14590,S14717,S16412,S16455,S16524,S16510,S14835,S14320,S17367,S17456,S17591,S17207,S17124,S17876,S18064,S18110,S18492,S17128,S18482,S18723,S19119,S17040,S20418,S19590,S20620,S20697,S20797,S20882,S20477,S21068,S21137,S21316,S21520,S21474,S21476,S21477,S21479,S21480,S21470,S21471,S22104,S22268,S22409,S22426,S22451,S22274,S22874,S22639,S18944,S22954,S22979,S22980,S23510,S23511,S21473,S19070,S27282',1);
+INSERT INTO userprofile_userprofile VALUES(2,'G12011','EPFL-GUESTS/CH',NULL,NULL,NULL,'Externe','S00000,S00001',2);
+INSERT INTO userprofile_userprofile VALUES(7,NULL,NULL,NULL,NULL,NULL,NULL,NULL,NULL);
+INSERT INTO userprofile_userprofile VALUES(8,NULL,NULL,NULL,NULL,NULL,NULL,NULL,NULL);
 DELETE FROM sqlite_sequence;
-INSERT INTO sqlite_sequence VALUES('django_migrations',17);
-INSERT INTO sqlite_sequence VALUES('django_admin_log',0);
+INSERT INTO sqlite_sequence VALUES('django_migrations',16);
+INSERT INTO sqlite_sequence VALUES('django_admin_log',4);
 INSERT INTO sqlite_sequence VALUES('django_content_type',8);
 INSERT INTO sqlite_sequence VALUES('auth_permission',24);
-INSERT INTO sqlite_sequence VALUES('auth_user',3);
+INSERT INTO sqlite_sequence VALUES('auth_user',4);
 INSERT INTO sqlite_sequence VALUES('django_site',1);
-INSERT INTO sqlite_sequence VALUES('userprofile_userprofile',3);
+INSERT INTO sqlite_sequence VALUES('userprofile_userprofile',8);
 CREATE UNIQUE INDEX "auth_group_permissions_group_id_permission_id_0cd325b0_uniq" ON "auth_group_permissions" ("group_id", "permission_id");
 CREATE INDEX "auth_group_permissions_group_id_b120cbf9" ON "auth_group_permissions" ("group_id");
 CREATE INDEX "auth_group_permissions_permission_id_84c5c92e" ON "auth_group_permissions" ("permission_id");
 CREATE UNIQUE INDEX "auth_user_groups_user_id_group_id_94350c0c_uniq" ON "auth_user_groups" ("user_id", "group_id");
 CREATE INDEX "auth_user_groups_user_id_6a12ed8b" ON "auth_user_groups" ("user_id");
 CREATE INDEX "auth_user_groups_group_id_97559544" ON "auth_user_groups" ("group_id");
 CREATE UNIQUE INDEX "auth_user_user_permissions_user_id_permission_id_14a6b632_uniq" ON "auth_user_user_permissions" ("user_id", "permission_id");
@@ -84,8 +92,10 @@
 CREATE INDEX "auth_user_user_permissions_permission_id_1fbb5f2c" ON "auth_user_user_permissions" ("permission_id");
 CREATE INDEX "django_admin_log_content_type_id_c4bce8eb" ON "django_admin_log" ("content_type_id");
 CREATE INDEX "django_admin_log_user_id_c564eba6" ON "django_admin_log" ("user_id");
 CREATE UNIQUE INDEX "django_content_type_app_label_model_76bd3d3b_uniq" ON "django_content_type" ("app_label", "model");
 CREATE UNIQUE INDEX "auth_permission_content_type_id_codename_01ab375a_uniq" ON "auth_permission" ("content_type_id", "codename");
 CREATE INDEX "auth_permission_content_type_id_2f476e4b" ON "auth_permission" ("content_type_id");
 CREATE INDEX "django_session_expire_date_a5c62663" ON "django_session" ("expire_date");
+CREATE UNIQUE INDEX userprofile_userprofile_sciper_uindex
+	on userprofile_userprofile (sciper);
 COMMIT;
```

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/settings.py` & `django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/settings.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/templates/index.html` & `django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/templates/index.html`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/tests/test_selenium.py` & `django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/tests/test_selenium.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/urls.py` & `django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/urls.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/django_tequila_app/views.py` & `django-tequila-4.0.0/sample_app/python3-6-django-1/django_tequila_app/views.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/manage.py` & `django-tequila-4.0.0/sample_app/python3-6-django-1/manage.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/admin.py` & `django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/admin.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/migrations/0001_initial.py` & `django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-6-django-1/userprofile/models.py` & `django-tequila-4.0.0/sample_app/python3-6-django-1/userprofile/models.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/admin.py` & `django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/admin.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/database.db` & `django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/database.db`

 * *Files 8% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -1,30 +1,31 @@
 PRAGMA foreign_keys=OFF;
 BEGIN TRANSACTION;
 CREATE TABLE IF NOT EXISTS "django_migrations" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "app" varchar(255) NOT NULL, "name" varchar(255) NOT NULL, "applied" datetime NOT NULL);
-INSERT INTO django_migrations VALUES(1,'contenttypes','0001_initial','2021-02-20 11:38:35.151943');
-INSERT INTO django_migrations VALUES(2,'contenttypes','0002_remove_content_type_name','2021-02-20 11:38:35.163482');
-INSERT INTO django_migrations VALUES(3,'auth','0001_initial','2021-02-20 11:38:35.175600');
-INSERT INTO django_migrations VALUES(4,'auth','0002_alter_permission_name_max_length','2021-02-20 11:38:35.185261');
-INSERT INTO django_migrations VALUES(5,'auth','0003_alter_user_email_max_length','2021-02-20 11:38:35.193767');
-INSERT INTO django_migrations VALUES(6,'auth','0004_alter_user_username_opts','2021-02-20 11:38:35.200958');
-INSERT INTO django_migrations VALUES(7,'auth','0005_alter_user_last_login_null','2021-02-20 11:38:35.208672');
-INSERT INTO django_migrations VALUES(8,'auth','0006_require_contenttypes_0002','2021-02-20 11:38:35.213215');
-INSERT INTO django_migrations VALUES(9,'auth','0007_alter_validators_add_error_messages','2021-02-20 11:38:35.226515');
-INSERT INTO django_migrations VALUES(10,'auth','0008_alter_user_username_max_length','2021-02-20 11:38:35.233710');
-INSERT INTO django_migrations VALUES(11,'auth','0009_alter_user_last_name_max_length','2021-02-20 11:38:35.240810');
-INSERT INTO django_migrations VALUES(12,'auth','0010_alter_group_name_max_length','2021-02-20 11:38:35.248141');
-INSERT INTO django_migrations VALUES(13,'auth','0011_update_proxy_permissions','2021-02-20 11:38:35.256635');
-INSERT INTO django_migrations VALUES(14,'django_tequila_app','0001_initial','2021-02-20 11:38:35.265665');
-INSERT INTO django_migrations VALUES(15,'admin','0001_initial','2021-02-20 11:38:35.276597');
-INSERT INTO django_migrations VALUES(16,'admin','0002_logentry_remove_auto_add','2021-02-20 11:38:35.288471');
-INSERT INTO django_migrations VALUES(17,'admin','0003_logentry_add_action_flag_choices','2021-02-20 11:38:35.300986');
-INSERT INTO django_migrations VALUES(18,'sessions','0001_initial','2021-02-20 11:38:35.306771');
-INSERT INTO django_migrations VALUES(19,'sites','0001_initial','2021-02-20 11:38:35.313476');
-INSERT INTO django_migrations VALUES(20,'sites','0002_alter_domain_unique','2021-02-20 11:38:35.321563');
+INSERT INTO django_migrations VALUES(1,'contenttypes','0001_initial','2021-01-21 14:26:45.949846');
+INSERT INTO django_migrations VALUES(2,'contenttypes','0002_remove_content_type_name','2021-01-21 14:26:45.968518');
+INSERT INTO django_migrations VALUES(3,'auth','0001_initial','2021-01-21 14:26:45.993188');
+INSERT INTO django_migrations VALUES(4,'auth','0002_alter_permission_name_max_length','2021-01-21 14:26:46.010552');
+INSERT INTO django_migrations VALUES(5,'auth','0003_alter_user_email_max_length','2021-01-21 14:26:46.024629');
+INSERT INTO django_migrations VALUES(6,'auth','0004_alter_user_username_opts','2021-01-21 14:26:46.036816');
+INSERT INTO django_migrations VALUES(7,'auth','0005_alter_user_last_login_null','2021-01-21 14:26:46.051676');
+INSERT INTO django_migrations VALUES(8,'auth','0006_require_contenttypes_0002','2021-01-21 14:26:46.061169');
+INSERT INTO django_migrations VALUES(9,'auth','0007_alter_validators_add_error_messages','2021-01-21 14:26:46.074547');
+INSERT INTO django_migrations VALUES(10,'auth','0008_alter_user_username_max_length','2021-01-21 14:26:46.104431');
+INSERT INTO django_migrations VALUES(11,'auth','0009_alter_user_last_name_max_length','2021-01-21 14:26:46.115999');
+INSERT INTO django_migrations VALUES(12,'django_tequila_app','0001_initial','2021-01-21 14:26:46.130996');
+INSERT INTO django_migrations VALUES(13,'admin','0001_initial','2021-01-21 14:26:46.150107');
+INSERT INTO django_migrations VALUES(14,'admin','0002_logentry_remove_auto_add','2021-01-21 14:26:46.171994');
+INSERT INTO django_migrations VALUES(15,'admin','0003_logentry_add_action_flag_choices','2021-01-21 14:26:46.194380');
+INSERT INTO django_migrations VALUES(16,'auth','0010_alter_group_name_max_length','2021-01-21 14:26:46.212055');
+INSERT INTO django_migrations VALUES(17,'auth','0011_update_proxy_permissions','2021-01-21 14:26:46.233294');
+INSERT INTO django_migrations VALUES(18,'django_tequila_app','0002_auto_20210121_1359','2021-01-21 14:26:46.252855');
+INSERT INTO django_migrations VALUES(19,'sessions','0001_initial','2021-01-21 14:26:46.270627');
+INSERT INTO django_migrations VALUES(20,'sites','0001_initial','2021-01-21 14:26:46.281105');
+INSERT INTO django_migrations VALUES(21,'sites','0002_alter_domain_unique','2021-01-21 14:26:46.294732');
 CREATE TABLE IF NOT EXISTS "django_content_type" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "app_label" varchar(100) NOT NULL, "model" varchar(100) NOT NULL);
 INSERT INTO django_content_type VALUES(1,'admin','logentry');
 INSERT INTO django_content_type VALUES(2,'auth','permission');
 INSERT INTO django_content_type VALUES(3,'auth','group');
 INSERT INTO django_content_type VALUES(4,'contenttypes','contenttype');
 INSERT INTO django_content_type VALUES(5,'sessions','session');
 INSERT INTO django_content_type VALUES(6,'sites','site');
@@ -55,34 +56,32 @@
 INSERT INTO auth_permission VALUES(22,6,'change_site','Can change site');
 INSERT INTO auth_permission VALUES(23,6,'delete_site','Can delete site');
 INSERT INTO auth_permission VALUES(24,6,'view_site','Can view site');
 INSERT INTO auth_permission VALUES(25,7,'add_user','Can add user');
 INSERT INTO auth_permission VALUES(26,7,'change_user','Can change user');
 INSERT INTO auth_permission VALUES(27,7,'delete_user','Can delete user');
 INSERT INTO auth_permission VALUES(28,7,'view_user','Can view user');
-CREATE TABLE IF NOT EXISTS "auth_group" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(150) NOT NULL UNIQUE);
-CREATE TABLE IF NOT EXISTS "django_tequila_app_user" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "password" varchar(128) NOT NULL, "last_login" datetime NULL, "is_superuser" bool NOT NULL, "username" varchar(150) NOT NULL UNIQUE, "first_name" varchar(30) NOT NULL, "last_name" varchar(150) NOT NULL, "email" varchar(254) NOT NULL, "is_staff" bool NOT NULL, "is_active" bool NOT NULL, "date_joined" datetime NOT NULL, "sciper" varchar(10) NOT NULL UNIQUE, "where" varchar(200) NULL, "units" text NULL, "classe" varchar(100) NULL, "statut" varchar(100) NULL, "group" text NULL, "memberof" text NULL);
-INSERT INTO django_tequila_app_user VALUES(2,'','2021-02-20 11:48:07.222897',0,'julien.delasoie','Julien-Ext','Delasoie-Ext','julien.delasoie@ubiko.ch',0,1,'2021-02-20 11:48:07.201003','G12011','EPFL-GUESTS/CH',NULL,NULL,'Externe',NULL,'S00000,S00001');
-INSERT INTO django_tequila_app_user VALUES(5,'!YPKBdDgkjrvp1htCDDTy5XwS1AWyh44xOmQLu2lJ','2022-04-14 12:43:17.173154',1,'delasoie','Julien','Delasoie','julien.delasoie@epfl.ch',1,1,'2022-04-14 07:38:25.238007','194044','ISAS-FSD/ISAS/VPO-SI/EPFL/CH','isas-fsd','Personnel technique/administratif','Personnel','ChronosUtilisateurs,Collaborateurs-VPSI-INN,DIT,DIT_ServiceNOW_Agents,DjangoFamily,IDEV-JIRA,IDEVELOP-SICO-Guest,IDEVFSD-SICO-Guest,INSTANT-LAB2,PhD-annual-report-admin,PhD-annual-report-administrative-assistant,PhDAssess-Activity_Specify_Participants-Test,SI-Notif-Incident-Majeur-ServiceNow,WP-SuperAdmin,WP_Monitoring,accounts-tequila-example,actu-api-rest-consumers,alerts-wwp-prod,arh-epfl,awx-poc-openshift-wwp-test,book_calendar_room_INN,boussole,c4science-tech,cold-wiki,dashboard-exopge-access,dit-sup.agents_otrs,eml-infoscience,exopge-openshift-users,gr-lsm-infoscience,grafana-exopge-isacademia-org-editors,idev-fsd-membres,infoscience-dev,infoscience-exports-role-editor,infoscience-exports-role-viewer,infoscience-lmc,infoscience-mics,infoscience-superadmin,infoscience-upfahl,infoscience_LME,innovation,intranet-epfl,mediatheque-celum5,memento-api-rest-consumers,metrics-exopge-access,personnel-epfl,phd-assess-ops,phd-assess-role-editor,phd-assess-role-viewer,phd-assess-test-role-editor,phd-assess-test-role-viewer,poc-cms-rancher-admins,respinfo-epfl,sdf-openshift,sre-epfl,vra_p_svc0033,vra_p_svc0041,vra_p_svc1394,wikijs_r_idevfsd,wikijs_w_idevfsd,wp-dev,wp-polylex-admins,wp-veritas-admins,wwp-infra-role-editor,wwp-infra-role-tag-image,wwp-infra-role-viewer,wwp-int-role-editor,wwp-int-role-viewer,wwp-members,wwp-role-editor,wwp-role-viewer,wwp-test-role-editor,wwp-test-role-viewer,isas-fsd-wordpress,vra_p_svc0176,book_calendar_room_DIT','S00167,S00188,S06362,S08502,S08780,S08781,S08782,S14034,S14089,U12635,U10000,S00000,S14149,S14235,S11115,S09180,S07954,S08652,S07431,S07414,S05034,S14375,U13030,S14590,S16412,S16510,S14835,S14320,S17367,S17456,S17591,S17207,S17124,S17876,S18064,S18110,S18492,S17128,S18482,S18723,S19119,S20418,S19590,S20620,S20697,S21068,S21137,S21316,S21520,S21474,S21476,S21477,S21479,S21480,S21470,S21471,S22268,S22409,S22426,S22274,S22874,S22639,S22979,S22980,S23510,S23511,S21473,S19070,S27282,S27445,S27446,S19687,S28013,S22343,S27146,S28476,S28475,S28881,S28884,S28885,S28928,S28923,S28987,U14213,S22451,S14368');
 CREATE TABLE IF NOT EXISTS "django_tequila_app_user_groups" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "user_id" integer NOT NULL REFERENCES "django_tequila_app_user" ("id") DEFERRABLE INITIALLY DEFERRED, "group_id" integer NOT NULL REFERENCES "auth_group" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "django_tequila_app_user_user_permissions" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "user_id" integer NOT NULL REFERENCES "django_tequila_app_user" ("id") DEFERRABLE INITIALLY DEFERRED, "permission_id" integer NOT NULL REFERENCES "auth_permission" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "django_admin_log" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "action_time" datetime NOT NULL, "object_id" text NULL, "object_repr" varchar(200) NOT NULL, "change_message" text NOT NULL, "content_type_id" integer NULL REFERENCES "django_content_type" ("id") DEFERRABLE INITIALLY DEFERRED, "user_id" integer NOT NULL REFERENCES "django_tequila_app_user" ("id") DEFERRABLE INITIALLY DEFERRED, "action_flag" smallint unsigned NOT NULL CHECK ("action_flag" >= 0));
+CREATE TABLE IF NOT EXISTS "auth_group" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(150) NOT NULL UNIQUE);
+CREATE TABLE IF NOT EXISTS "django_tequila_app_user" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "password" varchar(128) NOT NULL, "last_login" datetime NULL, "is_superuser" bool NOT NULL, "username" varchar(150) NOT NULL UNIQUE, "first_name" varchar(30) NOT NULL, "last_name" varchar(150) NOT NULL, "email" varchar(254) NOT NULL, "is_staff" bool NOT NULL, "is_active" bool NOT NULL, "date_joined" datetime NOT NULL, "where" varchar(200) NULL, "units" text NULL, "classe" varchar(100) NULL, "statut" varchar(100) NULL, "group" text NULL, "memberof" text NULL, "sciper" varchar(10) NULL UNIQUE);
+INSERT INTO django_tequila_app_user VALUES(8,'!DmQQRDYvzUOaPrFwH7NL9vjez2ftHqqGdrlQPIpq','2021-01-21 15:23:44.269085',1,'delasoie','Julien','Delasoie','julien.delasoie@epfl.ch',1,1,'2021-01-21 14:55:20.112724','IDEV-FSD/SI-IDEV/SI/EPFL/CH','idev-fsd','Personnel technique/administratif','Personnel','Cartographie-Read,Collaborateurs-VPSI-INN,DIT,DIT_ServiceNOW_Agents,DjangoFamily,IDEV-JIRA,IDEVELOP,IDEVELOP-SICO-Guest,INSTANT-LAB2,SI-Notif-Incident-Majeur,WP_Monitoring,book_calendar_room_DIT,book_calendar_room_INN,boussole,c4science-tech,dashboard-exopge-access,dit-sup.agents_otrs,eml-infoscience,exopge-openshift-users,gr-lsm-infoscience,infoscience-dev,infoscience-librarians,infoscience-lmc,infoscience-mics,infoscience-superadmin,infoscience-upfahl,infoscience_LME,innovation,intranet-epfl,mediatheque-celum5,metrics-exopge-access,personnel-epfl,personnel-kis,poc-cms-rancher-admins,respinfo-epfl,sdf-gitlab,sdf-openshift,sdf-openstack,sre-epfl,wwp-members,IDEVFSD-SICO-Guest,idev-fsd-wordpress,arh-epfl,vpsi-docker,docker-vpsi,book_calendar_room_PB,awx-poc-openshift-wwp-test,idev-fsd-membres,wp-dev,wwp-infra-role-tag-image,wwp-infra-role-viewer,wwp-int-role-editor,wwp-int-role-viewer,wwp-test-role-editor,wwp-test-role-viewer,wwp-role-editor,wwp-role-viewer,idevfsd-test-conferences-wp-admins,wp-veritas-admins,accounts-tequila-example,vra_p_peopl,vra_p_idevfsd,wp-polylex-admins,ChronosUtilisateurs,alerts-wwp-prod,AA_test,infoscience-exports-role-editor,infoscience-exports-role-viewer,actu-api-rest-consumers,memento-api-rest-consumers,wwp-infra-role-editor,WP-SuperAdmin,cold-wiki','S00167,S00188,S02104,S06362,S07309,S08502,S08780,S08781,S08782,S13906,S14034,S14089,U12635,U10000,S00000,S14149,S14235,S11115,S09180,S07954,S08652,S07431,S07414,S05034,S14375,S14368,U13030,U13028,S14524,S14590,S14717,S16412,S16455,S16524,S16510,S14835,S14320,S17367,S17456,S17591,S17207,S17124,S17876,S18064,S18110,S18492,S17128,S18482,S18723,S19119,S17040,S20418,S19590,S20620,S20697,S20797,S20882,S20477,S21068,S21137,S21316,S21520,S21474,S21476,S21477,S21479,S21480,S21470,S21471,S22104,S22268,S22409,S22426,S22451,S22274,S22874,S22639,S18944,S22954,S22979,S22980,S23510,S23511,S21473,S19070,S27282','194044');
 CREATE TABLE IF NOT EXISTS "django_session" ("session_key" varchar(40) NOT NULL PRIMARY KEY, "session_data" text NOT NULL, "expire_date" datetime NOT NULL);
-INSERT INTO django_session VALUES('d078aj29rdku25zjtaaownfn4wdd33fi','NWJmMWNkZTc0YjcwMjRmNGVkYTBlMWY3ZjhiOTkyNTZmOTUxZjBjNTp7InRlc3Rjb29raWUiOiJ3b3JrZWQiLCJfYXV0aF91c2VyX2lkIjoiMyIsIl9hdXRoX3VzZXJfYmFja2VuZCI6ImRqYW5nb190ZXF1aWxhLmRqYW5nb19iYWNrZW5kLlRlcXVpbGFCYWNrZW5kIiwiX2F1dGhfdXNlcl9oYXNoIjoiODcyYzI1MGRmNjMwNWI2N2MzMjgzYTUzMGQyMDFlZDA3NjRhNjJkNiJ9','2021-03-06 11:50:26.054220');
-INSERT INTO django_session VALUES('vzvb7gu3w9mg5ndcfrgwdmuetyglclyk','NGY2NTQwYzYzMTU3NWQ5NTgwMjYyOTY0ZjY0ODMyMzI4MDZhOGZmNzp7InRlc3Rjb29raWUiOiJ3b3JrZWQiLCJfYXV0aF91c2VyX2lkIjoiNSIsIl9hdXRoX3VzZXJfYmFja2VuZCI6ImRqYW5nb190ZXF1aWxhLmRqYW5nb19iYWNrZW5kLlRlcXVpbGFCYWNrZW5kIiwiX2F1dGhfdXNlcl9oYXNoIjoiMmNjMGEzNmYwN2Y1NjczMjg4ZDRmNmJiZTlhYTA1ODJiMjI0ZmVmYyJ9','2022-04-28 12:43:17.181168');
+INSERT INTO django_session VALUES('pfwsbvxd12tgys116jd5nc97e7gskk83','NTVkNTczZTlhOTEwZmM3MTBjZGFlNzI5YzllMDQzYWQ2MjRjMzBkNDp7InRlc3Rjb29raWUiOiJ3b3JrZWQiLCJfYXV0aF91c2VyX2lkIjoiOCIsIl9hdXRoX3VzZXJfYmFja2VuZCI6ImRqYW5nb190ZXF1aWxhLmRqYW5nb19iYWNrZW5kLlRlcXVpbGFCYWNrZW5kIiwiX2F1dGhfdXNlcl9oYXNoIjoiOWVlNjI1YTU0MDY0NjllNDYwM2ZiNzFmM2Y3NDViYTRjMzU2Njk5NCJ9','2021-02-04 15:23:44.275671');
 CREATE TABLE IF NOT EXISTS "django_site" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(50) NOT NULL, "domain" varchar(100) NOT NULL UNIQUE);
 INSERT INTO django_site VALUES(1,'example.com','example.com');
 DELETE FROM sqlite_sequence;
-INSERT INTO sqlite_sequence VALUES('django_migrations',20);
+INSERT INTO sqlite_sequence VALUES('django_migrations',21);
 INSERT INTO sqlite_sequence VALUES('django_content_type',7);
 INSERT INTO sqlite_sequence VALUES('auth_permission',28);
-INSERT INTO sqlite_sequence VALUES('auth_group',0);
 INSERT INTO sqlite_sequence VALUES('django_admin_log',0);
+INSERT INTO sqlite_sequence VALUES('auth_group',0);
+INSERT INTO sqlite_sequence VALUES('django_tequila_app_user',8);
 INSERT INTO sqlite_sequence VALUES('django_site',1);
-INSERT INTO sqlite_sequence VALUES('django_tequila_app_user',5);
 CREATE UNIQUE INDEX "django_content_type_app_label_model_76bd3d3b_uniq" ON "django_content_type" ("app_label", "model");
 CREATE UNIQUE INDEX "auth_group_permissions_group_id_permission_id_0cd325b0_uniq" ON "auth_group_permissions" ("group_id", "permission_id");
 CREATE INDEX "auth_group_permissions_group_id_b120cbf9" ON "auth_group_permissions" ("group_id");
 CREATE INDEX "auth_group_permissions_permission_id_84c5c92e" ON "auth_group_permissions" ("permission_id");
 CREATE UNIQUE INDEX "auth_permission_content_type_id_codename_01ab375a_uniq" ON "auth_permission" ("content_type_id", "codename");
 CREATE INDEX "auth_permission_content_type_id_2f476e4b" ON "auth_permission" ("content_type_id");
 CREATE UNIQUE INDEX "django_tequila_app_user_groups_user_id_group_id_ca4020db_uniq" ON "django_tequila_app_user_groups" ("user_id", "group_id");
```

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/migrations/0001_initial.py` & `django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/models.py` & `django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/models.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/settings.py` & `django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/settings.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/templates/index.html` & `django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/templates/index.html`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/tests/test_selenium.py` & `django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/tests/test_selenium.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/urls.py` & `django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/urls.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/django_tequila_app/views.py` & `django-tequila-4.0.0/sample_app/python3-8-django-2/django_tequila_app/views.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/sample_app/python3-8-django-2/manage.py` & `django-tequila-4.0.0/sample_app/python3-8-django-2/manage.py`

 * *Files identical despite different names*

### Comparing `django-tequila-3.4.0/setup.py` & `django-tequila-4.0.0/setup.py`

 * *Files identical despite different names*

