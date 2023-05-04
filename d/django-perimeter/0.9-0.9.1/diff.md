# Comparing `tmp/django-perimeter-0.9.tar.gz` & `tmp/django-perimeter-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-perimeter-0.9.tar", last modified: Sat Apr  8 22:26:52 2017, max compression
+gzip compressed data, was "dist/django-perimeter-0.9.1.tar", last modified: Thu Jul  6 10:29:51 2017, max compression
```

## Comparing `django-perimeter-0.9.tar` & `django-perimeter-0.9.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/django_perimeter.egg-info/
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)        1 2017-04-08 22:26:52.000000 django-perimeter-0.9/django_perimeter.egg-info/dependency_links.txt
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     5539 2017-04-08 22:26:52.000000 django-perimeter-0.9/django_perimeter.egg-info/PKG-INFO
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)       12 2017-04-08 22:26:52.000000 django-perimeter-0.9/django_perimeter.egg-info/requires.txt
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1134 2017-04-08 22:26:52.000000 django-perimeter-0.9/django_perimeter.egg-info/SOURCES.txt
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)       19 2017-04-08 22:26:52.000000 django-perimeter-0.9/django_perimeter.egg-info/top_level.txt
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)      112 2017-04-08 22:20:53.000000 django-perimeter-0.9/MANIFEST.in
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/perimeter/
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)       60 2015-06-11 21:23:40.000000 django-perimeter-0.9/perimeter/__init__.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1227 2017-04-08 22:20:53.000000 django-perimeter-0.9/perimeter/admin.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)      305 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/compat.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1689 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/forms.py
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/perimeter/management/
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)       67 2015-05-05 21:22:07.000000 django-perimeter-0.9/perimeter/management/__init__.py
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/perimeter/management/commands/
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)       76 2015-05-05 21:22:07.000000 django-perimeter-0.9/perimeter/management/commands/__init__.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1961 2017-04-08 22:20:53.000000 django-perimeter-0.9/perimeter/management/commands/create_access_token.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)      419 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/management/commands/list_access_tokens.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     2623 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/middleware.py
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/perimeter/migrations/
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1729 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/migrations/0001_initial.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)      646 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/migrations/0002_auto_20150611_1234.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)      418 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/migrations/0003_auto_20150612_0151.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)      712 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/migrations/0004_auto_20170407_0639.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)        0 2015-06-11 21:23:57.000000 django-perimeter-0.9/perimeter/migrations/__init__.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     6639 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/models.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1990 2017-04-08 22:20:53.000000 django-perimeter-0.9/perimeter/settings.py
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/perimeter/templates/
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/perimeter/templates/perimeter/
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)      489 2017-04-08 22:20:53.000000 django-perimeter-0.9/perimeter/templates/perimeter/gateway.html
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/perimeter/tests/
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)       24 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/tests/__init__.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     3691 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/tests/test_forms.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1556 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/tests/test_functions.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     3556 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/tests/test_middleware.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     6431 2017-04-08 22:22:21.000000 django-perimeter-0.9/perimeter/tests/test_models.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1841 2017-04-08 22:22:44.000000 django-perimeter-0.9/perimeter/tests/test_views.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)      207 2017-04-08 22:20:53.000000 django-perimeter-0.9/perimeter/urls.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1748 2017-04-08 22:21:21.000000 django-perimeter-0.9/perimeter/views.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     5539 2017-04-08 22:26:52.000000 django-perimeter-0.9/PKG-INFO
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     4115 2017-04-08 22:21:21.000000 django-perimeter-0.9/README.rst
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)       38 2017-04-08 22:26:52.000000 django-perimeter-0.9/setup.cfg
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     1200 2017-04-08 22:26:30.000000 django-perimeter-0.9/setup.py
-drwxr-xr-x   0 hugorodgerbrown   (502) staff       (20)        0 2017-04-08 22:26:52.000000 django-perimeter-0.9/test_app/
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)       30 2015-05-05 21:22:07.000000 django-perimeter-0.9/test_app/__init__.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)       47 2015-05-05 21:22:07.000000 django-perimeter-0.9/test_app/models.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)     2662 2017-04-08 22:21:21.000000 django-perimeter-0.9/test_app/settings.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)        0 2015-05-05 21:22:07.000000 django-perimeter-0.9/test_app/tests.py
--rw-r--r--   0 hugorodgerbrown   (502) staff       (20)      369 2017-04-08 22:20:53.000000 django-perimeter-0.9/test_app/urls.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/django_perimeter.egg-info/
+-rw-r--r--   0 hugo       (501) staff       (20)        1 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/django_perimeter.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (501) staff       (20)     5541 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/django_perimeter.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)       12 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/django_perimeter.egg-info/requires.txt
+-rw-r--r--   0 hugo       (501) staff       (20)     1169 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/django_perimeter.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       19 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/django_perimeter.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (501) staff       (20)      112 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/MANIFEST.in
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/perimeter/
+-rw-r--r--   0 hugo       (501) staff       (20)       60 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1227 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/admin.py
+-rw-r--r--   0 hugo       (501) staff       (20)      305 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/compat.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1689 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/forms.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/perimeter/management/
+-rw-r--r--   0 hugo       (501) staff       (20)       67 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/management/__init__.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/perimeter/management/commands/
+-rw-r--r--   0 hugo       (501) staff       (20)       76 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/management/commands/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1961 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/management/commands/create_access_token.py
+-rw-r--r--   0 hugo       (501) staff       (20)      419 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/management/commands/list_access_tokens.py
+-rw-r--r--   0 hugo       (501) staff       (20)     2623 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/middleware.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/perimeter/migrations/
+-rw-r--r--   0 hugo       (501) staff       (20)     1725 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/migrations/0001_initial.py
+-rw-r--r--   0 hugo       (501) staff       (20)      645 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/migrations/0002_auto_20150611_1234.py
+-rw-r--r--   0 hugo       (501) staff       (20)      417 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/migrations/0003_auto_20150612_0151.py
+-rw-r--r--   0 hugo       (501) staff       (20)      712 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/migrations/0004_auto_20170407_0639.py
+-rw-r--r--   0 hugo       (501) staff       (20)        0 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/migrations/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)     6680 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/models.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1990 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/settings.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/perimeter/templates/
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/perimeter/templates/perimeter/
+-rw-r--r--   0 hugo       (501) staff       (20)      489 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/templates/perimeter/gateway.html
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/perimeter/tests/
+-rw-r--r--   0 hugo       (501) staff       (20)       24 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/tests/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)     3691 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/tests/test_forms.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1556 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/tests/test_functions.py
+-rw-r--r--   0 hugo       (501) staff       (20)     3556 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/tests/test_middleware.py
+-rw-r--r--   0 hugo       (501) staff       (20)      955 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/tests/test_migrations.py
+-rw-r--r--   0 hugo       (501) staff       (20)     6431 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/tests/test_models.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1841 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/tests/test_views.py
+-rw-r--r--   0 hugo       (501) staff       (20)      207 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/urls.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1748 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/perimeter/views.py
+-rw-r--r--   0 hugo       (501) staff       (20)     5541 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)     4115 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/README.rst
+-rw-r--r--   0 hugo       (501) staff       (20)       59 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/setup.cfg
+-rw-r--r--   0 hugo       (501) staff       (20)     1202 2017-07-06 10:27:21.000000 django-perimeter-0.9.1/setup.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2017-07-06 10:29:51.000000 django-perimeter-0.9.1/test_app/
+-rw-r--r--   0 hugo       (501) staff       (20)       30 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/test_app/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)       47 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/test_app/models.py
+-rw-r--r--   0 hugo       (501) staff       (20)     2662 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/test_app/settings.py
+-rw-r--r--   0 hugo       (501) staff       (20)        0 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/test_app/tests.py
+-rw-r--r--   0 hugo       (501) staff       (20)      369 2017-07-06 10:24:56.000000 django-perimeter-0.9.1/test_app/urls.py
```

### Comparing `django-perimeter-0.9/django_perimeter.egg-info/PKG-INFO` & `django-perimeter-0.9.1/django_perimeter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-perimeter
-Version: 0.9
+Version: 0.9.1
 Summary: Site-wide perimeter access control for Django projects.
 Home-page: https://github.com/yunojuno/django-perimeter
 Author: YunoJuno
 Author-email: code@yunojuno.com
 License: MIT
 Description: .. image:: https://badge.fury.io/py/django-perimeter.svg
             :target: https://badge.fury.io/py/django-perimeter
```

### Comparing `django-perimeter-0.9/django_perimeter.egg-info/SOURCES.txt` & `django-perimeter-0.9.1/django_perimeter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 perimeter/migrations/0004_auto_20170407_0639.py
 perimeter/migrations/__init__.py
 perimeter/templates/perimeter/gateway.html
 perimeter/tests/__init__.py
 perimeter/tests/test_forms.py
 perimeter/tests/test_functions.py
 perimeter/tests/test_middleware.py
+perimeter/tests/test_migrations.py
 perimeter/tests/test_models.py
 perimeter/tests/test_views.py
 test_app/__init__.py
 test_app/models.py
 test_app/settings.py
 test_app/tests.py
 test_app/urls.py
```

### Comparing `django-perimeter-0.9/perimeter/admin.py` & `django-perimeter-0.9.1/perimeter/admin.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/forms.py` & `django-perimeter-0.9.1/perimeter/forms.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/management/commands/create_access_token.py` & `django-perimeter-0.9.1/perimeter/management/commands/create_access_token.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/middleware.py` & `django-perimeter-0.9.1/perimeter/middleware.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/migrations/0001_initial.py` & `django-perimeter-0.9.1/perimeter/migrations/0001_initial.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,16 @@
                 ('created_by', models.ForeignKey(to=settings.AUTH_USER_MODEL, null=True)),
             ],
         ),
         migrations.CreateModel(
             name='AccessTokenUse',
             fields=[
                 ('id', models.AutoField(verbose_name='ID', serialize=False, auto_created=True, primary_key=True)),
-                ('user_email', models.EmailField(max_length=254, verbose_name=b'Token used by (email)')),
-                ('user_name', models.CharField(max_length=100, verbose_name=b'Token used by (name)')),
-                ('client_ip', models.CharField(max_length=15, verbose_name=b'IP address', blank=True)),
-                ('client_user_agent', models.CharField(max_length=150, verbose_name=b'User Agent', blank=True)),
+                ('user_email', models.EmailField(max_length=254, verbose_name='Token used by (email)')),
+                ('user_name', models.CharField(max_length=100, verbose_name='Token used by (name)')),
+                ('client_ip', models.CharField(max_length=15, verbose_name='IP address', blank=True)),
+                ('client_user_agent', models.CharField(max_length=150, verbose_name='User Agent', blank=True)),
                 ('timestamp', models.DateTimeField()),
                 ('token', models.ForeignKey(to='perimeter.AccessToken')),
             ],
         ),
     ]
```

### Comparing `django-perimeter-0.9/perimeter/migrations/0002_auto_20150611_1234.py` & `django-perimeter-0.9.1/perimeter/migrations/0002_auto_20150611_1234.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
             name='token',
             field=models.CharField(unique=True, max_length=50),
             preserve_default=True,
         ),
         migrations.AlterField(
             model_name='accesstokenuse',
             name='user_email',
-            field=models.EmailField(max_length=75, verbose_name=b'Token used by (email)'),
+            field=models.EmailField(max_length=75, verbose_name='Token used by (email)'),
             preserve_default=True,
         ),
     ]
```

### Comparing `django-perimeter-0.9/perimeter/migrations/0004_auto_20170407_0639.py` & `django-perimeter-0.9.1/perimeter/migrations/0004_auto_20170407_0639.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/models.py` & `django-perimeter-0.9.1/perimeter/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # -*- coding: utf-8 -*-
+from __future__ import unicode_literals
+
 import datetime
 import random
 
 from django.conf import settings
 from django.core.cache import cache
 from django.db import models
 from django.db.models.signals import post_save, post_delete
```

### Comparing `django-perimeter-0.9/perimeter/settings.py` & `django-perimeter-0.9.1/perimeter/settings.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/tests/test_forms.py` & `django-perimeter-0.9.1/perimeter/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/tests/test_functions.py` & `django-perimeter-0.9.1/perimeter/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/tests/test_middleware.py` & `django-perimeter-0.9.1/perimeter/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/tests/test_models.py` & `django-perimeter-0.9.1/perimeter/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/tests/test_views.py` & `django-perimeter-0.9.1/perimeter/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/perimeter/views.py` & `django-perimeter-0.9.1/perimeter/views.py`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/PKG-INFO` & `django-perimeter-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-perimeter
-Version: 0.9
+Version: 0.9.1
 Summary: Site-wide perimeter access control for Django projects.
 Home-page: https://github.com/yunojuno/django-perimeter
 Author: YunoJuno
 Author-email: code@yunojuno.com
 License: MIT
 Description: .. image:: https://badge.fury.io/py/django-perimeter.svg
             :target: https://badge.fury.io/py/django-perimeter
```

### Comparing `django-perimeter-0.9/README.rst` & `django-perimeter-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-perimeter-0.9/setup.py` & `django-perimeter-0.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 README = open(path.join(path.dirname(__file__), 'README.rst')).read()
 
 # allow setup.py to be run from any path
 chdir(path.normpath(path.join(path.abspath(__file__), pardir)))
 
 setup(
     name='django-perimeter',
-    version='0.9',
+    version='0.9.1',
     packages=find_packages(),
     include_package_data=True,
     license='MIT',
     description='Site-wide perimeter access control for Django projects.',
     long_description=README,
     url='https://github.com/yunojuno/django-perimeter',
     author='YunoJuno',
```

### Comparing `django-perimeter-0.9/test_app/settings.py` & `django-perimeter-0.9.1/test_app/settings.py`

 * *Files identical despite different names*

