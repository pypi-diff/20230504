# Comparing `tmp/django-theme-academy-0.3.3.tar.gz` & `tmp/django-theme-academy-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-theme-academy-0.3.3.tar", last modified: Tue Mar 21 19:05:56 2023, max compression
+gzip compressed data, was "django-theme-academy-0.3.4.tar", last modified: Wed May  3 23:46:05 2023, max compression
```

## Comparing `django-theme-academy-0.3.3.tar` & `django-theme-academy-0.3.4.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.773847 django-theme-academy-0.3.3/
--rw-r--r--   0 glenn      (504) admin       (80)     1458 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/LICENSE.txt
--rw-r--r--   0 glenn      (504) admin       (80)      151 2023-02-01 18:15:07.000000 django-theme-academy-0.3.3/MANIFEST.in
--rw-r--r--   0 glenn      (504) admin       (80)     6431 2023-03-21 19:05:56.773895 django-theme-academy-0.3.3/PKG-INFO
--rw-r--r--   0 glenn      (504) admin       (80)     5532 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/README.md
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.770435 django-theme-academy-0.3.3/academy_theme/
--rw-r--r--   0 glenn      (504) admin       (80)       21 2023-03-21 19:04:13.000000 django-theme-academy-0.3.3/academy_theme/__init__.py
--rw-r--r--   0 glenn      (504) admin       (80)      130 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/apps.py
--rw-r--r--   0 glenn      (504) admin       (80)     1496 2023-02-01 18:15:07.000000 django-theme-academy-0.3.3/academy_theme/context_processors.py
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/models.py
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/py.typed
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.768702 django-theme-academy-0.3.3/academy_theme/static/
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.768898 django-theme-academy-0.3.3/academy_theme/static/academy_theme/
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.771286 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/
--rw-r--r--   0 glenn      (504) admin       (80)     3451 2023-02-01 18:15:07.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/_globals.scss
--rw-r--r--   0 glenn      (504) admin       (80)     3618 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/_mixins.scss
--rw-r--r--   0 glenn      (504) admin       (80)      711 2023-02-01 18:15:07.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/_page.scss
--rw-r--r--   0 glenn      (504) admin       (80)     1105 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/_ribbon.scss
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.771603 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/boostrap-5.1.3/
--rw-r--r--   0 glenn      (504) admin       (80)     4484 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/boostrap-5.1.3/_breakpoints.scss
--rw-r--r--   0 glenn      (504) admin       (80)    10621 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/boostrap-5.1.3/_functions.scss
--rw-r--r--   0 glenn      (504) admin       (80)    67864 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/boostrap-5.1.3/_variables.scss
--rw-r--r--   0 glenn      (504) admin       (80)     7542 2022-11-19 23:57:54.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/theme.css
--rw-r--r--   0 glenn      (504) admin       (80)     3009 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/theme.css.map
--rw-r--r--   0 glenn      (504) admin       (80)      315 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/theme.scss
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.772685 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/
--rw-r--r--   0 glenn      (504) admin       (80)    11518 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/android-chrome-192x192.png
--rw-r--r--   0 glenn      (504) admin       (80)    30901 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/android-chrome-512x512.png
--rw-r--r--   0 glenn      (504) admin       (80)    10286 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/apple-touch-icon.png
--rw-r--r--   0 glenn      (504) admin       (80)      624 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/favicon-16x16.png
--rw-r--r--   0 glenn      (504) admin       (80)     1425 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/favicon-32x32.png
--rw-r--r--   0 glenn      (504) admin       (80)    15406 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/favicon.ico
--rw-r--r--   0 glenn      (504) admin       (80)   135992 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/logo.png
--rw-r--r--   0 glenn      (504) admin       (80)    15629 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/logo.svg
--rw-r--r--   0 glenn      (504) admin       (80)      263 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/site.webmanifest
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.772784 django-theme-academy-0.3.3/academy_theme/static/academy_theme/js/
--rw-r--r--   0 glenn      (504) admin       (80)      173 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/static/academy_theme/js/theme.js
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.768986 django-theme-academy-0.3.3/academy_theme/templates/
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.772992 django-theme-academy-0.3.3/academy_theme/templates/academy_theme/
--rw-r--r--   0 glenn      (504) admin       (80)     1271 2023-02-01 18:15:07.000000 django-theme-academy-0.3.3/academy_theme/templates/academy_theme/base--wildewidgets.html
--rw-r--r--   0 glenn      (504) admin       (80)     5432 2023-03-21 19:02:41.000000 django-theme-academy-0.3.3/academy_theme/templates/academy_theme/base.html
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.773090 django-theme-academy-0.3.3/academy_theme/templates/academy_theme/templatetags/
--rw-r--r--   0 glenn      (504) admin       (80)      153 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/templates/academy_theme/templatetags/breadcrumb.html
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.773263 django-theme-academy-0.3.3/academy_theme/templatetags/
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/templatetags/__init__.py
--rw-r--r--   0 glenn      (504) admin       (80)      666 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/templatetags/academy_theme.py
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/urls.py
--rw-r--r--   0 glenn      (504) admin       (80)        0 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/views.py
--rw-r--r--   0 glenn      (504) admin       (80)     2287 2022-11-18 23:00:44.000000 django-theme-academy-0.3.3/academy_theme/wildewidgets.py
-drwxr-xr-x   0 glenn      (504) admin       (80)        0 2023-03-21 19:05:56.773755 django-theme-academy-0.3.3/django_theme_academy.egg-info/
--rw-r--r--   0 glenn      (504) admin       (80)     6431 2023-03-21 19:05:56.000000 django-theme-academy-0.3.3/django_theme_academy.egg-info/PKG-INFO
--rw-r--r--   0 glenn      (504) admin       (80)     1891 2023-03-21 19:05:56.000000 django-theme-academy-0.3.3/django_theme_academy.egg-info/SOURCES.txt
--rw-r--r--   0 glenn      (504) admin       (80)        1 2023-03-21 19:05:56.000000 django-theme-academy-0.3.3/django_theme_academy.egg-info/dependency_links.txt
--rw-r--r--   0 glenn      (504) admin       (80)       29 2023-03-21 19:05:56.000000 django-theme-academy-0.3.3/django_theme_academy.egg-info/requires.txt
--rw-r--r--   0 glenn      (504) admin       (80)       14 2023-03-21 19:05:56.000000 django-theme-academy-0.3.3/django_theme_academy.egg-info/top_level.txt
--rw-r--r--   0 glenn      (504) admin       (80)      723 2023-03-21 19:05:56.774151 django-theme-academy-0.3.3/setup.cfg
--rw-r--r--   0 glenn      (504) admin       (80)     1278 2023-03-21 19:04:13.000000 django-theme-academy-0.3.3/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.880132 django-theme-academy-0.3.4/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1458 2022-11-02 21:25:58.000000 django-theme-academy-0.3.4/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      151 2023-01-18 00:27:07.000000 django-theme-academy-0.3.4/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     6432 2023-05-03 23:46:05.880271 django-theme-academy-0.3.4/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5533 2023-01-28 00:45:26.000000 django-theme-academy-0.3.4/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.858660 django-theme-academy-0.3.4/academy_theme/
+-rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-05-03 23:45:50.000000 django-theme-academy-0.3.4/academy_theme/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      130 2022-11-02 16:35:25.000000 django-theme-academy-0.3.4/academy_theme/apps.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1496 2023-01-18 00:27:07.000000 django-theme-academy-0.3.4/academy_theme/context_processors.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)        0 2022-11-02 18:30:08.000000 django-theme-academy-0.3.4/academy_theme/models.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-02 16:42:36.000000 django-theme-academy-0.3.4/academy_theme/py.typed
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.850872 django-theme-academy-0.3.4/academy_theme/static/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.859570 django-theme-academy-0.3.4/academy_theme/static/academy_theme/
+-rw-r--r--   0 cmalek     (501) admin       (80)     6148 2022-11-02 19:00:49.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/.DS_Store
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.865030 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3451 2023-01-18 00:28:32.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/_globals.scss
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3618 2022-11-02 21:07:19.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/_mixins.scss
+-rw-rw-r--   0 cmalek     (501) admin       (80)      711 2023-01-18 00:27:07.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/_page.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)     1105 2023-01-18 00:29:49.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/_ribbon.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.867877 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/boostrap-5.1.3/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4484 2022-11-02 16:34:18.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/boostrap-5.1.3/_breakpoints.scss
+-rw-rw-r--   0 cmalek     (501) admin       (80)    10621 2022-11-02 16:34:18.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/boostrap-5.1.3/_functions.scss
+-rw-rw-r--   0 cmalek     (501) admin       (80)    67864 2022-11-02 16:34:18.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/boostrap-5.1.3/_variables.scss
+-rw-rw-r--   0 cmalek     (501) admin       (80)     7542 2023-01-18 00:27:04.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/theme.css
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3009 2022-11-17 00:40:47.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/theme.css.map
+-rw-rw-r--   0 cmalek     (501) admin       (80)      315 2022-11-02 16:34:18.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/theme.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.875228 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/
+-rw-rw-r--   0 cmalek     (501) admin       (80)    11518 2022-11-03 00:01:52.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/android-chrome-192x192.png
+-rw-rw-r--   0 cmalek     (501) admin       (80)    30901 2022-11-03 00:01:52.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/android-chrome-512x512.png
+-rw-rw-r--   0 cmalek     (501) admin       (80)    10286 2022-11-03 00:01:52.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/apple-touch-icon.png
+-rw-rw-r--   0 cmalek     (501) admin       (80)      624 2022-11-03 00:01:52.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/favicon-16x16.png
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1425 2022-11-03 00:01:52.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/favicon-32x32.png
+-rw-rw-r--   0 cmalek     (501) admin       (80)    15406 2022-11-03 00:01:52.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/favicon.ico
+-rw-r--r--   0 cmalek     (501) admin       (80)   135992 2022-11-02 19:08:53.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/logo.png
+-rw-rw-r--   0 cmalek     (501) admin       (80)    15629 2022-11-03 01:59:20.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/logo.svg
+-rw-rw-r--   0 cmalek     (501) admin       (80)      263 2022-11-03 00:01:52.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/site.webmanifest
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.875756 django-theme-academy-0.3.4/academy_theme/static/academy_theme/js/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      173 2022-11-02 16:34:18.000000 django-theme-academy-0.3.4/academy_theme/static/academy_theme/js/theme.js
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.852057 django-theme-academy-0.3.4/academy_theme/templates/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.876731 django-theme-academy-0.3.4/academy_theme/templates/academy_theme/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1271 2023-01-18 00:38:06.000000 django-theme-academy-0.3.4/academy_theme/templates/academy_theme/base--wildewidgets.html
+-rw-r--r--   0 cmalek     (501) admin       (80)     5451 2023-05-03 23:12:22.000000 django-theme-academy-0.3.4/academy_theme/templates/academy_theme/base.html
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.877097 django-theme-academy-0.3.4/academy_theme/templates/academy_theme/templatetags/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      153 2022-11-02 16:34:18.000000 django-theme-academy-0.3.4/academy_theme/templates/academy_theme/templatetags/breadcrumb.html
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.877738 django-theme-academy-0.3.4/academy_theme/templatetags/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-02 16:34:18.000000 django-theme-academy-0.3.4/academy_theme/templatetags/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      666 2022-11-02 16:45:48.000000 django-theme-academy-0.3.4/academy_theme/templatetags/academy_theme.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)        0 2022-11-02 18:30:15.000000 django-theme-academy-0.3.4/academy_theme/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)        0 2022-11-02 18:30:13.000000 django-theme-academy-0.3.4/academy_theme/views.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1381 2023-05-02 23:10:54.000000 django-theme-academy-0.3.4/academy_theme/wildewidgets.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:46:05.879830 django-theme-academy-0.3.4/django_theme_academy.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     6432 2023-05-03 23:46:05.000000 django-theme-academy-0.3.4/django_theme_academy.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1936 2023-05-03 23:46:05.000000 django-theme-academy-0.3.4/django_theme_academy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-05-03 23:46:05.000000 django-theme-academy-0.3.4/django_theme_academy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       29 2023-05-03 23:46:05.000000 django-theme-academy-0.3.4/django_theme_academy.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       14 2023-05-03 23:46:05.000000 django-theme-academy-0.3.4/django_theme_academy.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      796 2023-05-03 23:46:05.880949 django-theme-academy-0.3.4/setup.cfg
+-rw-r--r--   0 cmalek     (501) admin       (80)     1278 2023-05-03 23:45:50.000000 django-theme-academy-0.3.4/setup.py
```

### Comparing `django-theme-academy-0.3.3/LICENSE.txt` & `django-theme-academy-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/PKG-INFO` & `django-theme-academy-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-theme-academy
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Tabler-based, fixed left sidebar django theme.
 Home-page: https://github.com/caltechads/django-theme-academy
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: django
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -170,15 +170,15 @@
     brand_image: str = static("myapp/images/logo.png")
     brand_text: str = "My App"
     items: List[Tuple[str, str]] = [
         ('Home', 'myapp:home'),
     ]
 
 
-class BaseBreadcrumbs(BreadrumbBlock):
+class BaseBreadcrumbs(BreadcrumbBlock):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.add_breadcrumb('Home', reverse('myapp:home'))
 
 
 class WildewidgetsView(
     MenuMixin,
```

### Comparing `django-theme-academy-0.3.3/README.md` & `django-theme-academy-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     brand_image: str = static("myapp/images/logo.png")
     brand_text: str = "My App"
     items: List[Tuple[str, str]] = [
         ('Home', 'myapp:home'),
     ]
 
 
-class BaseBreadcrumbs(BreadrumbBlock):
+class BaseBreadcrumbs(BreadcrumbBlock):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.add_breadcrumb('Home', reverse('myapp:home'))
 
 
 class WildewidgetsView(
     MenuMixin,
```

### Comparing `django-theme-academy-0.3.3/academy_theme/context_processors.py` & `django-theme-academy-0.3.4/academy_theme/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/_globals.scss` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/_globals.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/_mixins.scss` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/_mixins.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/_page.scss` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/_page.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/_ribbon.scss` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/_ribbon.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/boostrap-5.1.3/_breakpoints.scss` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/boostrap-5.1.3/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/boostrap-5.1.3/_functions.scss` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/boostrap-5.1.3/_functions.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/boostrap-5.1.3/_variables.scss` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/boostrap-5.1.3/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/theme.css` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/theme.css`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/css/theme.css.map` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/css/theme.css.map`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/android-chrome-192x192.png` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/android-chrome-512x512.png` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/apple-touch-icon.png` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/favicon-16x16.png` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/favicon-32x32.png` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/favicon.ico` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/logo.png` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/static/academy_theme/images/logo.svg` & `django-theme-academy-0.3.4/academy_theme/static/academy_theme/images/logo.svg`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/templates/academy_theme/base--wildewidgets.html` & `django-theme-academy-0.3.4/academy_theme/templates/academy_theme/base--wildewidgets.html`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/academy_theme/templates/academy_theme/base.html` & `django-theme-academy-0.3.4/academy_theme/templates/academy_theme/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     <a href="#main-content-anchor">{% trans 'Skip to main content' %}</a>
   </div>
 
   <div id="shifted_contents" class="page">
 
     {# Ribbon #}
     <div class="ribbon_bar">
-      <div class="ribbon_bar__content container d-flex justify-content-between align-items-center">
+      <div class="ribbon_bar__content container-fluid d-flex justify-content-between align-items-center">
         <nav class="ribbon_bar__content__breadcrumbs d-none d-md-block">
           {% block breadcrumbs %}{% endblock %}
         </nav>
         {% block ribbon_bar_links %}
         <ul class="ribbon_bar__content__links d-flex align-self-center">
           <li>
             {% if user.is_authenticated %}
@@ -68,15 +68,15 @@
     <div>
       {% block secondary_menu %}{{submenu}}{% endblock %}
     </div>
 
     {# Page Content #}
     <div class="page__content">
       <a id="main-content-anchor"></a>
-        <section class="page__content {% block content_classes %}{% endblock %} {% if container_size %}{{container_size}}{% else %}container{% endif %}">
+        <section class="page__content__inner {% block content_classes %}{% endblock %} {% if container_size %}{{container_size}}{% else %}container-fluid{% endif %}">
         {% block messages %}
           <div class="messages d-flex-column pl-0">
             {% for message in messages %}
               <div class="messages__item alert alert-dismissible
                 {% if message.tags %}
                   {% if message.tags == 'success' %}
                     alert-success
```

### Comparing `django-theme-academy-0.3.3/academy_theme/templatetags/academy_theme.py` & `django-theme-academy-0.3.4/academy_theme/templatetags/academy_theme.py`

 * *Files identical despite different names*

### Comparing `django-theme-academy-0.3.3/django_theme_academy.egg-info/PKG-INFO` & `django-theme-academy-0.3.4/django_theme_academy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-theme-academy
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Tabler-based, fixed left sidebar django theme.
 Home-page: https://github.com/caltechads/django-theme-academy
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: django
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -170,15 +170,15 @@
     brand_image: str = static("myapp/images/logo.png")
     brand_text: str = "My App"
     items: List[Tuple[str, str]] = [
         ('Home', 'myapp:home'),
     ]
 
 
-class BaseBreadcrumbs(BreadrumbBlock):
+class BaseBreadcrumbs(BreadcrumbBlock):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.add_breadcrumb('Home', reverse('myapp:home'))
 
 
 class WildewidgetsView(
     MenuMixin,
```

### Comparing `django-theme-academy-0.3.3/django_theme_academy.egg-info/SOURCES.txt` & `django-theme-academy-0.3.4/django_theme_academy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 academy_theme/apps.py
 academy_theme/context_processors.py
 academy_theme/models.py
 academy_theme/py.typed
 academy_theme/urls.py
 academy_theme/views.py
 academy_theme/wildewidgets.py
+academy_theme/static/academy_theme/.DS_Store
 academy_theme/static/academy_theme/css/_globals.scss
 academy_theme/static/academy_theme/css/_mixins.scss
 academy_theme/static/academy_theme/css/_page.scss
 academy_theme/static/academy_theme/css/_ribbon.scss
 academy_theme/static/academy_theme/css/theme.css
 academy_theme/static/academy_theme/css/theme.css.map
 academy_theme/static/academy_theme/css/theme.scss
```

### Comparing `django-theme-academy-0.3.3/setup.cfg` & `django-theme-academy-0.3.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 	invalid-name,
 	too-few-public-methods,
 	attribute-defined-outside-init,
 	too-many-lines
 
 [mypy]
 python_executable = ~/.pyenv/shims/python
+exclude = (?x)(
+	^build$
+	| sandbox\/setup\.py$
+	| migrations\/.*.py$
+	)
 
 [mypy-sphinx_rtd_theme.*]
 ignore_missing_imports = True
 
 [mypy-setuptools.*]
 ignore_missing_imports = True
```

### Comparing `django-theme-academy-0.3.3/setup.py` & `django-theme-academy-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="django-theme-academy",
-    version="0.3.3",
+    version="0.3.4",
     packages=find_packages(),
     include_package_data=True,
     package_data={'academy_theme': ["py.typed"]},
     install_requires=[
         "django-wildewidgets >= 0.13.49"
     ],
     author="Caltech IMSS ADS",
```

