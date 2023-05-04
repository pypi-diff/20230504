# Comparing `tmp/for-django-projects-1.0.1.tar.gz` & `tmp/for-django-projects-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "for-django-projects-1.0.1.tar", last modified: Thu May  4 17:13:27 2023, max compression
+gzip compressed data, was "for-django-projects-1.0.2.tar", last modified: Thu May  4 17:17:40 2023, max compression
```

## Comparing `for-django-projects-1.0.1.tar` & `for-django-projects-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:13:27.250421 for-django-projects-1.0.1/
--rw-rw-rw-   0        0        0      970 2023-05-04 17:13:27.249420 for-django-projects-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-05-04 16:47:19.000000 for-django-projects-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 17:13:27.207069 for-django-projects-1.0.1/for_django_projects/
--rw-rw-rw-   0        0        0        0 2023-05-04 17:11:49.000000 for-django-projects-1.0.1/for_django_projects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:13:27.231124 for-django-projects-1.0.1/for_django_projects/alertas/
--rw-rw-rw-   0        0        0     1152 2022-11-22 19:35:13.000000 for-django-projects-1.0.1/for_django_projects/alertas/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:13:27.237305 for-django-projects-1.0.1/for_django_projects/form_utils/
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/__init__.py
--rw-rw-rw-   0        0        0      511 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/admin.py
--rw-rw-rw-   0        0        0     2457 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/fields.py
--rw-rw-rw-   0        0        0    10772 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/forms.py
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/models.py
--rw-rw-rw-   0        0        0      375 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:13:27.239321 for-django-projects-1.0.1/for_django_projects/form_utils/templatetags/
--rw-rw-rw-   0        0        0      118 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/templatetags/__init__.py
--rw-rw-rw-   0        0        0     3499 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/templatetags/form_utils.py
--rw-rw-rw-   0        0        0      555 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/utils.py
--rw-rw-rw-   0        0        0     4405 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/form_utils/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:13:27.243359 for-django-projects-1.0.1/for_django_projects/pwa/
--rw-rw-rw-   0        0        0       41 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/pwa/__init__.py
--rw-rw-rw-   0        0        0     4617 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/pwa/app_settings.py
--rw-rw-rw-   0        0        0       86 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/pwa/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:13:27.244439 for-django-projects-1.0.1/for_django_projects/pwa/templatetags/
--rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/pwa/templatetags/__init__.py
--rw-rw-rw-   0        0        0      732 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/pwa/templatetags/pwa.py
--rw-rw-rw-   0        0        0      358 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/pwa/urls.py
--rw-rw-rw-   0        0        0      616 2022-07-11 17:53:14.000000 for-django-projects-1.0.1/for_django_projects/pwa/views.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:13:27.248423 for-django-projects-1.0.1/for_django_projects/utils/
--rw-rw-rw-   0        0        0        0 2023-05-03 20:33:09.000000 for-django-projects-1.0.1/for_django_projects/utils/__init__.py
--rw-rw-rw-   0        0        0    24053 2023-05-04 14:09:27.000000 for-django-projects-1.0.1/for_django_projects/utils/custom_models.py
--rw-rw-rw-   0        0        0     3267 2023-05-04 14:09:27.000000 for-django-projects-1.0.1/for_django_projects/utils/decoradores.py
--rw-rw-rw-   0        0        0    18609 2023-05-04 14:15:47.000000 for-django-projects-1.0.1/for_django_projects/utils/funciones.py
--rw-rw-rw-   0        0        0     4732 2023-05-04 14:32:38.000000 for-django-projects-1.0.1/for_django_projects/utils/funciones_adicionales.py
--rw-rw-rw-   0        0        0     3117 2023-03-30 15:00:29.000000 for-django-projects-1.0.1/for_django_projects/utils/models_utils.py
--rw-rw-rw-   0        0        0     4058 2023-05-02 21:53:32.000000 for-django-projects-1.0.1/for_django_projects/utils/validadores.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:13:27.230114 for-django-projects-1.0.1/for_django_projects.egg-info/
--rw-rw-rw-   0        0        0      970 2023-05-04 17:13:27.000000 for-django-projects-1.0.1/for_django_projects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1309 2023-05-04 17:13:27.000000 for-django-projects-1.0.1/for_django_projects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:13:27.000000 for-django-projects-1.0.1/for_django_projects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2023-05-04 17:13:27.000000 for-django-projects-1.0.1/for_django_projects.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-04 17:13:27.000000 for-django-projects-1.0.1/for_django_projects.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 17:13:27.250421 for-django-projects-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-05-04 17:12:28.000000 for-django-projects-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/
+-rw-rw-rw-   0        0        0     1010 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-05-04 17:16:18.000000 for-django-projects-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.566758 for-django-projects-1.0.2/for_django_projects/
+-rw-rw-rw-   0        0        0        0 2023-05-04 17:11:49.000000 for-django-projects-1.0.2/for_django_projects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.582387 for-django-projects-1.0.2/for_django_projects/alertas/
+-rw-rw-rw-   0        0        0     1152 2022-11-22 19:35:13.000000 for-django-projects-1.0.2/for_django_projects/alertas/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.596398 for-django-projects-1.0.2/for_django_projects/form_utils/
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/__init__.py
+-rw-rw-rw-   0        0        0      511 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/admin.py
+-rw-rw-rw-   0        0        0     2457 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/fields.py
+-rw-rw-rw-   0        0        0    10772 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/forms.py
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/models.py
+-rw-rw-rw-   0        0        0      375 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.596398 for-django-projects-1.0.2/for_django_projects/form_utils/templatetags/
+-rw-rw-rw-   0        0        0      118 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     3499 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/templatetags/form_utils.py
+-rw-rw-rw-   0        0        0      555 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/utils.py
+-rw-rw-rw-   0        0        0     4405 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/form_utils/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/for_django_projects/pwa/
+-rw-rw-rw-   0        0        0       41 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/__init__.py
+-rw-rw-rw-   0        0        0     4617 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/app_settings.py
+-rw-rw-rw-   0        0        0       86 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/for_django_projects/pwa/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/templatetags/pwa.py
+-rw-rw-rw-   0        0        0      358 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/urls.py
+-rw-rw-rw-   0        0        0      616 2022-07-11 17:53:14.000000 for-django-projects-1.0.2/for_django_projects/pwa/views.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/for_django_projects/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-03 20:33:09.000000 for-django-projects-1.0.2/for_django_projects/utils/__init__.py
+-rw-rw-rw-   0        0        0    24053 2023-05-04 14:09:27.000000 for-django-projects-1.0.2/for_django_projects/utils/custom_models.py
+-rw-rw-rw-   0        0        0     3267 2023-05-04 14:09:27.000000 for-django-projects-1.0.2/for_django_projects/utils/decoradores.py
+-rw-rw-rw-   0        0        0    18609 2023-05-04 14:15:47.000000 for-django-projects-1.0.2/for_django_projects/utils/funciones.py
+-rw-rw-rw-   0        0        0     4732 2023-05-04 14:32:38.000000 for-django-projects-1.0.2/for_django_projects/utils/funciones_adicionales.py
+-rw-rw-rw-   0        0        0     3117 2023-03-30 15:00:29.000000 for-django-projects-1.0.2/for_django_projects/utils/models_utils.py
+-rw-rw-rw-   0        0        0     4058 2023-05-02 21:53:32.000000 for-django-projects-1.0.2/for_django_projects/utils/validadores.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:40.582387 for-django-projects-1.0.2/for_django_projects.egg-info/
+-rw-rw-rw-   0        0        0     1010 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1309 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-04 17:17:40.000000 for-django-projects-1.0.2/for_django_projects.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:17:40.598404 for-django-projects-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      919 2023-05-04 17:17:37.000000 for-django-projects-1.0.2/setup.py
```

### Comparing `for-django-projects-1.0.1/PKG-INFO` & `for-django-projects-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: for-django-projects
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package of libraries for Django projects
 Home-page: https://github.com/jasmanysanchez/for-django-projects
 Author: Jasmany Sanchez Mendez
 Author-email: jasmanysanchez97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,16 @@
 Requires [Django](https://www.djangoproject.com/) v2.2+ and [Python](https://www.python.org/) v3.6+ to run.
 
 Add apps in INSTALLED_APPS:
 
 ```sh
 INSTALLED_APPS = [
     ...
-    'form_utils',
-    'pwa'
+    'for_django_projects.form_utils',
+    'for_django_projects.pwa'
     ...
 ]
 ```
 
 ## License
 
 MIT
```

### Comparing `for-django-projects-1.0.1/for_django_projects/alertas/__init__.py` & `for-django-projects-1.0.2/for_django_projects/alertas/__init__.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/form_utils/fields.py` & `for-django-projects-1.0.2/for_django_projects/form_utils/fields.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/form_utils/forms.py` & `for-django-projects-1.0.2/for_django_projects/form_utils/forms.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/form_utils/templatetags/form_utils.py` & `for-django-projects-1.0.2/for_django_projects/form_utils/templatetags/form_utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/form_utils/utils.py` & `for-django-projects-1.0.2/for_django_projects/form_utils/utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/form_utils/widgets.py` & `for-django-projects-1.0.2/for_django_projects/form_utils/widgets.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/pwa/app_settings.py` & `for-django-projects-1.0.2/for_django_projects/pwa/app_settings.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/pwa/templatetags/pwa.py` & `for-django-projects-1.0.2/for_django_projects/pwa/templatetags/pwa.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/pwa/views.py` & `for-django-projects-1.0.2/for_django_projects/pwa/views.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/utils/custom_models.py` & `for-django-projects-1.0.2/for_django_projects/utils/custom_models.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/utils/decoradores.py` & `for-django-projects-1.0.2/for_django_projects/utils/decoradores.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/utils/funciones.py` & `for-django-projects-1.0.2/for_django_projects/utils/funciones.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/utils/funciones_adicionales.py` & `for-django-projects-1.0.2/for_django_projects/utils/funciones_adicionales.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/utils/models_utils.py` & `for-django-projects-1.0.2/for_django_projects/utils/models_utils.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects/utils/validadores.py` & `for-django-projects-1.0.2/for_django_projects/utils/validadores.py`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/for_django_projects.egg-info/PKG-INFO` & `for-django-projects-1.0.2/for_django_projects.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: for-django-projects
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package of libraries for Django projects
 Home-page: https://github.com/jasmanysanchez/for-django-projects
 Author: Jasmany Sanchez Mendez
 Author-email: jasmanysanchez97@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,16 @@
 Requires [Django](https://www.djangoproject.com/) v2.2+ and [Python](https://www.python.org/) v3.6+ to run.
 
 Add apps in INSTALLED_APPS:
 
 ```sh
 INSTALLED_APPS = [
     ...
-    'form_utils',
-    'pwa'
+    'for_django_projects.form_utils',
+    'for_django_projects.pwa'
     ...
 ]
 ```
 
 ## License
 
 MIT
```

### Comparing `for-django-projects-1.0.1/for_django_projects.egg-info/SOURCES.txt` & `for-django-projects-1.0.2/for_django_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `for-django-projects-1.0.1/setup.py` & `for-django-projects-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="for-django-projects",
-    version="1.0.1",
+    version="1.0.2",
     author="Jasmany Sanchez Mendez",
     author_email="jasmanysanchez97@gmail.com",
     description="Package of libraries for Django projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jasmanysanchez/for-django-projects",
     packages=setuptools.find_packages(),
@@ -17,19 +17,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         'Django>=2.2',
-        'django-appconf>=1.0.5',
         'django-select2>=7.7.1',
         'numpy>=1.24.3',
         'pandas>=2.0.1',
         'python-dateutil>=2.8.2',
-        'pytz>=2023.3',
-        'six>=1.16.0',
-        'sqlparse>=0.4.4',
-        'tzdata>=2023.3',
         'xlwt>=1.3.0',
     ],
 )
```

