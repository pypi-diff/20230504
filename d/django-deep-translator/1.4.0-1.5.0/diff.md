# Comparing `tmp/django-deep-translator-1.4.0.tar.gz` & `tmp/django-deep-translator-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-deep-translator-1.4.0.tar", last modified: Wed May  3 13:29:29 2023, max compression
+gzip compressed data, was "django-deep-translator-1.5.0.tar", last modified: Thu May  4 08:27:08 2023, max compression
```

## Comparing `django-deep-translator-1.4.0.tar` & `django-deep-translator-1.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:29.032721 django-deep-translator-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-03 13:29:29.032721 django-deep-translator-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:29.032721 django-deep-translator-1.4.0/django_deep_translator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/django_deep_translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/django_deep_translator/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:29.032721 django-deep-translator-1.4.0/django_deep_translator/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/django_deep_translator/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:29.032721 django-deep-translator-1.4.0/django_deep_translator/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/django_deep_translator/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/django_deep_translator/management/commands/translate_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/django_deep_translator/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/django_deep_translator/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:29.032721 django-deep-translator-1.4.0/django_deep_translator/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/django_deep_translator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/django_deep_translator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:29.032721 django-deep-translator-1.4.0/django_deep_translator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-03 13:29:28.000000 django-deep-translator-1.4.0/django_deep_translator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 13:29:29.000000 django-deep-translator-1.4.0/django_deep_translator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:29:28.000000 django-deep-translator-1.4.0/django_deep_translator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 13:29:28.000000 django-deep-translator-1.4.0/django_deep_translator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 13:29:28.000000 django-deep-translator-1.4.0/django_deep_translator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:29:29.032721 django-deep-translator-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:29.032721 django-deep-translator-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:17.000000 django-deep-translator-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:27:08.344101 django-deep-translator-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-04 08:27:08.344101 django-deep-translator-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:27:08.344101 django-deep-translator-1.5.0/django_deep_translator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/django_deep_translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/django_deep_translator/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:27:08.344101 django-deep-translator-1.5.0/django_deep_translator/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/django_deep_translator/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:27:08.344101 django-deep-translator-1.5.0/django_deep_translator/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/django_deep_translator/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/django_deep_translator/management/commands/translate_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/django_deep_translator/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/django_deep_translator/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:27:08.344101 django-deep-translator-1.5.0/django_deep_translator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/django_deep_translator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/django_deep_translator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:27:08.344101 django-deep-translator-1.5.0/django_deep_translator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-04 08:27:08.000000 django-deep-translator-1.5.0/django_deep_translator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-04 08:27:08.000000 django-deep-translator-1.5.0/django_deep_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:27:08.000000 django-deep-translator-1.5.0/django_deep_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 08:27:08.000000 django-deep-translator-1.5.0/django_deep_translator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 08:27:08.000000 django-deep-translator-1.5.0/django_deep_translator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:27:08.344101 django-deep-translator-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:27:08.344101 django-deep-translator-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:26:52.000000 django-deep-translator-1.5.0/tests/__init__.py
```

### Comparing `django-deep-translator-1.4.0/LICENSE` & `django-deep-translator-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-deep-translator-1.4.0/PKG-INFO` & `django-deep-translator-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-deep-translator
-Version: 1.4.0
+Version: 1.5.0
 Summary: Automatically translate the pot (`.po`) files generated by django's makemessages command built on top of python deep-translator package
 Home-page: https://github.com/wmo-raf/django-deep-translator
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -76,15 +76,14 @@
 ---
 
 Using a different Translation Service:
 
 ```python
     # default: 'django_deep_translator.services.GoogleTranslatorService'
     PO_TRANSLATOR_SERVICE = 'django_deep_translator.services.GoogleAPITranslatorService'
-    GOOGLE_TRANSLATE_KEY = '<google-api-key>'
 ```
 
 ---
 
 
 `PO_TRANSLATOR_SERVICE` accepts the following services with respective additional variables:
```

### Comparing `django-deep-translator-1.4.0/README.md` & `django-deep-translator-1.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 ---
 
 Using a different Translation Service:
 
 ```python
     # default: 'django_deep_translator.services.GoogleTranslatorService'
     PO_TRANSLATOR_SERVICE = 'django_deep_translator.services.GoogleAPITranslatorService'
-    GOOGLE_TRANSLATE_KEY = '<google-api-key>'
 ```
 
 ---
 
 
 `PO_TRANSLATOR_SERVICE` accepts the following services with respective additional variables:
```

### Comparing `django-deep-translator-1.4.0/django_deep_translator/management/commands/translate_messages.py` & `django-deep-translator-1.5.0/django_deep_translator/management/commands/translate_messages.py`

 * *Files identical despite different names*

### Comparing `django-deep-translator-1.4.0/django_deep_translator/services.py` & `django-deep-translator-1.5.0/django_deep_translator/services.py`

 * *Files identical despite different names*

### Comparing `django-deep-translator-1.4.0/django_deep_translator/utils.py` & `django-deep-translator-1.5.0/django_deep_translator/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,11 +32,11 @@
                           .format(val, setting_name, e.__class__.__name__, e))
     
 def get_translator():
     """
     Returns the default translator.
     """
     TranslatorService = getattr(settings, 'PO_TRANSLATOR_SERVICE',
-                                'translator.services.GoogleTranslatorService')
+                                'django_deep_translator.services.GoogleTranslatorService')
     
     translator = perform_import(TranslatorService, 'PO_TRANSLATOR_SERVICE')()
     return translator
```

### Comparing `django-deep-translator-1.4.0/django_deep_translator.egg-info/PKG-INFO` & `django-deep-translator-1.5.0/django_deep_translator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-deep-translator
-Version: 1.4.0
+Version: 1.5.0
 Summary: Automatically translate the pot (`.po`) files generated by django's makemessages command built on top of python deep-translator package
 Home-page: https://github.com/wmo-raf/django-deep-translator
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -76,15 +76,14 @@
 ---
 
 Using a different Translation Service:
 
 ```python
     # default: 'django_deep_translator.services.GoogleTranslatorService'
     PO_TRANSLATOR_SERVICE = 'django_deep_translator.services.GoogleAPITranslatorService'
-    GOOGLE_TRANSLATE_KEY = '<google-api-key>'
 ```
 
 ---
 
 
 `PO_TRANSLATOR_SERVICE` accepts the following services with respective additional variables:
```

### Comparing `django-deep-translator-1.4.0/django_deep_translator.egg-info/SOURCES.txt` & `django-deep-translator-1.5.0/django_deep_translator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-deep-translator-1.4.0/setup.py` & `django-deep-translator-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 install_requirements = parse_requirements(os.path.join(PROJECT_ROOT, 'requirements.txt'), session=uuid.uuid1())
 
 # e.g. ['django', 'google-api-python-client']
 requirements = [getattr(ir, 'requirement', str(getattr(ir, 'req', None))) for ir in install_requirements]
 
 setup(
     name='django-deep-translator',
-    version='1.4.0',
+    version='1.5.0',
     packages=find_packages(),
     install_requires=requirements,
     include_package_data=True,
     license='MIT License',
     description='Automatically translate the pot (`.po`) files generated by django\'s '
                 'makemessages command built on top of python deep-translator package',
     long_description=README,
```

