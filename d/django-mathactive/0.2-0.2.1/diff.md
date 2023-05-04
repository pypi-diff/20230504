# Comparing `tmp/django-mathactive-0.2.tar.gz` & `tmp/django-mathactive-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mathactive-0.2.tar", last modified: Thu May  4 15:36:51 2023, max compression
+gzip compressed data, was "django-mathactive-0.2.1.tar", last modified: Thu May  4 16:47:10 2023, max compression
```

## Comparing `django-mathactive-0.2.tar` & `django-mathactive-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 15:36:51.800584 django-mathactive-0.2/
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)       38 2023-05-04 15:25:17.000000 django-mathactive-0.2/MANIFEST.in
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      834 2023-05-04 15:36:51.800584 django-mathactive-0.2/PKG-INFO
-drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 15:36:51.800584 django-mathactive-0.2/django_mathactive.egg-info/
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      834 2023-05-04 15:36:51.000000 django-mathactive-0.2/django_mathactive.egg-info/PKG-INFO
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      852 2023-05-04 15:36:51.000000 django-mathactive-0.2/django_mathactive.egg-info/SOURCES.txt
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)        1 2023-05-04 15:36:51.000000 django-mathactive-0.2/django_mathactive.egg-info/dependency_links.txt
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)       12 2023-05-04 15:36:51.000000 django-mathactive-0.2/django_mathactive.egg-info/requires.txt
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)       18 2023-05-04 15:36:51.000000 django-mathactive-0.2/django_mathactive.egg-info/top_level.txt
-drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 15:36:51.800584 django-mathactive-0.2/mathactive_django/
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)        0 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/__init__.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)       63 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/admin.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      165 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/apps.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      830 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/controllers.py
-drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 15:36:51.800584 django-mathactive-0.2/mathactive_django/data/
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      821 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/data/difficulty_start_stop_step.csv
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      164 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/data/question_templates.yaml
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      122 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/env_loader.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      854 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/generators.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      326 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/hints.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      291 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/logger.py
-drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 15:36:51.800584 django-mathactive-0.2/mathactive_django/microlessons/
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)     3054 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/microlessons/num_one.py
-drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 15:36:51.800584 django-mathactive-0.2/mathactive_django/migrations/
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      581 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/migrations/0001_initial.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)        0 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/migrations/__init__.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      432 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/models.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)     1616 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/questions.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      128 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/urls.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)     3277 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/utils.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      473 2023-05-03 11:14:27.000000 django-mathactive-0.2/mathactive_django/views.py
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)       88 2023-05-03 11:12:37.000000 django-mathactive-0.2/pyproject.toml
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)      868 2023-05-04 15:36:51.800584 django-mathactive-0.2/setup.cfg
--rw-r--r--   0 sviddo    (1000) sviddo    (1001)       37 2023-05-03 11:13:03.000000 django-mathactive-0.2/setup.py
+drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 16:47:10.105572 django-mathactive-0.2.1/
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)       38 2023-05-04 15:25:17.000000 django-mathactive-0.2.1/MANIFEST.in
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      836 2023-05-04 16:47:10.105572 django-mathactive-0.2.1/PKG-INFO
+drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 16:47:10.105572 django-mathactive-0.2.1/django_mathactive.egg-info/
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      836 2023-05-04 16:47:10.000000 django-mathactive-0.2.1/django_mathactive.egg-info/PKG-INFO
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      852 2023-05-04 16:47:10.000000 django-mathactive-0.2.1/django_mathactive.egg-info/SOURCES.txt
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)        1 2023-05-04 16:47:10.000000 django-mathactive-0.2.1/django_mathactive.egg-info/dependency_links.txt
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)       12 2023-05-04 16:47:10.000000 django-mathactive-0.2.1/django_mathactive.egg-info/requires.txt
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)       18 2023-05-04 16:47:10.000000 django-mathactive-0.2.1/django_mathactive.egg-info/top_level.txt
+drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 16:47:10.105572 django-mathactive-0.2.1/mathactive_django/
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)        0 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/__init__.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)       63 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/admin.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      165 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/apps.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      830 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/controllers.py
+drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 16:47:10.105572 django-mathactive-0.2.1/mathactive_django/data/
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      821 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/data/difficulty_start_stop_step.csv
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      164 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/data/question_templates.yaml
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      122 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/env_loader.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      854 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/generators.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      326 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/hints.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      291 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/logger.py
+drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 16:47:10.105572 django-mathactive-0.2.1/mathactive_django/microlessons/
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)     3054 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/microlessons/num_one.py
+drwxr-xr-x   0 sviddo    (1000) sviddo    (1001)        0 2023-05-04 16:47:10.105572 django-mathactive-0.2.1/mathactive_django/migrations/
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      581 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/migrations/0001_initial.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)        0 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/migrations/__init__.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      432 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/models.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)     1616 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/questions.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      128 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/urls.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)     3277 2023-05-03 11:14:27.000000 django-mathactive-0.2.1/mathactive_django/utils.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      473 2023-05-04 16:45:59.000000 django-mathactive-0.2.1/mathactive_django/views.py
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)       88 2023-05-03 11:12:37.000000 django-mathactive-0.2.1/pyproject.toml
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)      870 2023-05-04 16:47:10.105572 django-mathactive-0.2.1/setup.cfg
+-rw-r--r--   0 sviddo    (1000) sviddo    (1001)       37 2023-05-03 11:13:03.000000 django-mathactive-0.2.1/setup.py
```

### Comparing `django-mathactive-0.2/PKG-INFO` & `django-mathactive-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mathactive
-Version: 0.2
+Version: 0.2.1
 Summary: A Django version of mathactive repo
 Author: Vlad Snisar
 Author-email: vladyslavsnisar@proton.me
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
```

### Comparing `django-mathactive-0.2/django_mathactive.egg-info/PKG-INFO` & `django-mathactive-0.2.1/django_mathactive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mathactive
-Version: 0.2
+Version: 0.2.1
 Summary: A Django version of mathactive repo
 Author: Vlad Snisar
 Author-email: vladyslavsnisar@proton.me
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
```

### Comparing `django-mathactive-0.2/django_mathactive.egg-info/SOURCES.txt` & `django-mathactive-0.2.1/django_mathactive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-mathactive-0.2/mathactive_django/controllers.py` & `django-mathactive-0.2.1/mathactive_django/controllers.py`

 * *Files identical despite different names*

### Comparing `django-mathactive-0.2/mathactive_django/data/difficulty_start_stop_step.csv` & `django-mathactive-0.2.1/mathactive_django/data/difficulty_start_stop_step.csv`

 * *Files identical despite different names*

### Comparing `django-mathactive-0.2/mathactive_django/generators.py` & `django-mathactive-0.2.1/mathactive_django/generators.py`

 * *Files identical despite different names*

### Comparing `django-mathactive-0.2/mathactive_django/microlessons/num_one.py` & `django-mathactive-0.2.1/mathactive_django/microlessons/num_one.py`

 * *Files identical despite different names*

### Comparing `django-mathactive-0.2/mathactive_django/migrations/0001_initial.py` & `django-mathactive-0.2.1/mathactive_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mathactive-0.2/mathactive_django/questions.py` & `django-mathactive-0.2.1/mathactive_django/questions.py`

 * *Files identical despite different names*

### Comparing `django-mathactive-0.2/mathactive_django/utils.py` & `django-mathactive-0.2.1/mathactive_django/utils.py`

 * *Files identical despite different names*

### Comparing `django-mathactive-0.2/setup.cfg` & `django-mathactive-0.2.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-mathactive
-version = 0.2
+version = 0.2.1
 description = A Django version of mathactive repo
 author = Vlad Snisar
 author_email = vladyslavsnisar@proton.me
 license = BSD-3-Clause  # Example license
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

