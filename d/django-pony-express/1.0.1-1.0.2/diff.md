# Comparing `tmp/django-pony-express-1.0.1.tar.gz` & `tmp/django-pony-express-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pony-express-1.0.1.tar", last modified: Wed May  3 13:59:39 2023, max compression
+gzip compressed data, was "django-pony-express-1.0.2.tar", last modified: Thu May  4 10:16:56 2023, max compression
```

## Comparing `django-pony-express-1.0.1.tar` & `django-pony-express-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0     2346 2023-05-03 13:52:42.132917 django-pony-express-1.0.1/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0     1696 2023-05-03 13:52:48.910530 django-pony-express-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3299 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/.gitignore
--rw-r--r--   0        0        0      904 2023-05-03 13:52:48.888852 django-pony-express-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      551 2023-05-03 13:52:48.888852 django-pony-express-1.0.1/.readthedocs.yml
--rw-r--r--   0        0        0      254 2023-05-03 13:44:27.245582 django-pony-express-1.0.1/CHANGES.md
--rw-r--r--   0        0        0     1090 2023-05-03 13:52:48.888852 django-pony-express-1.0.1/LICENSE.md
--rw-r--r--   0        0        0      138 2023-05-03 13:52:48.888852 django-pony-express-1.0.1/MANIFEST.in
--rw-r--r--   0        0        0     5272 2023-05-03 13:52:48.894859 django-pony-express-1.0.1/README.md
--rw-r--r--   0        0        0       85 2023-05-03 13:44:27.226098 django-pony-express-1.0.1/django_pony_express/__init__.py
--rw-r--r--   0        0        0      120 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/django_pony_express/errors.py
--rw-r--r--   0        0        0     1607 2023-05-03 13:32:01.959010 django-pony-express-1.0.1/django_pony_express/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/django_pony_express/services/__init__.py
--rw-r--r--   0        0        0    11273 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/django_pony_express/services/base.py
--rw-r--r--   0        0        0    10121 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/django_pony_express/services/tests.py
--rw-r--r--   0        0        0      654 2023-05-03 13:52:48.910530 django-pony-express-1.0.1/docs/Makefile
--rw-r--r--   0        0        0     2819 2023-05-03 13:52:48.910530 django-pony-express-1.0.1/docs/conf.py
--rw-r--r--   0        0        0       33 2023-05-03 13:34:58.443495 django-pony-express-1.0.1/docs/features/changelog.rst
--rw-r--r--   0        0        0     9661 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/docs/features/mail.md
--rw-r--r--   0        0        0     5069 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/docs/features/tests.md
--rw-r--r--   0        0        0      282 2023-05-03 13:49:39.022556 django-pony-express-1.0.1/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-05-03 13:52:48.910530 django-pony-express-1.0.1/docs/make.bat
--rw-r--r--   0        0        0      677 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/manage.py
--rw-r--r--   0        0        0     3575 2023-05-03 13:52:48.894859 django-pony-express-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1682 2023-05-03 13:31:21.061433 django-pony-express-1.0.1/settings.py
--rw-r--r--   0        0        0       69 2023-05-03 13:52:48.894859 django-pony-express-1.0.1/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/testapp/__init__.py
--rw-r--r--   0        0        0      145 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/testapp/templates/testapp/test_email.html
--rw-r--r--   0        0        0      148 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/testapp/templates/testapp/test_email.txt
--rw-r--r--   0        0        0      144 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/testapp/urls.py
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/tests/files/testfile.txt
--rw-r--r--   0        0        0     9590 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/tests/test_email_test_service.py
--rw-r--r--   0        0        0    15614 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/tests/test_mail_services.py
--rw-r--r--   0        0        0     7134 1970-01-01 00:00:00.000000 django-pony-express-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2346 2023-05-03 13:52:42.132917 django-pony-express-1.0.2/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0       82 2023-05-04 10:15:00.669626 django-pony-express-1.0.2/.coveragerc
+-rw-r--r--   0        0        0      288 2023-05-04 10:15:00.669626 django-pony-express-1.0.2/.editorconfig
+-rw-r--r--   0        0        0     1696 2023-05-04 10:15:00.700870 django-pony-express-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3299 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/.gitignore
+-rw-r--r--   0        0        0      904 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      551 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0      297 2023-05-04 10:16:33.609693 django-pony-express-1.0.2/CHANGES.md
+-rw-r--r--   0        0        0     1107 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     5227 2023-05-04 10:15:00.700870 django-pony-express-1.0.2/README.md
+-rw-r--r--   0        0        0       82 2023-05-04 10:16:33.593983 django-pony-express-1.0.2/django_pony_express/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/django_pony_express/errors.py
+-rw-r--r--   0        0        0     1607 2023-05-03 13:32:01.959010 django-pony-express-1.0.2/django_pony_express/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/django_pony_express/services/__init__.py
+-rw-r--r--   0        0        0    11273 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/django_pony_express/services/base.py
+-rw-r--r--   0        0        0    10121 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/django_pony_express/services/tests.py
+-rw-r--r--   0        0        0      654 2023-05-04 10:15:00.719977 django-pony-express-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0     2819 2023-05-04 10:15:00.716470 django-pony-express-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-05-03 13:34:58.443495 django-pony-express-1.0.2/docs/features/changelog.rst
+-rw-r--r--   0        0        0     9661 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/docs/features/mail.md
+-rw-r--r--   0        0        0     5069 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/docs/features/tests.md
+-rw-r--r--   0        0        0      282 2023-05-03 13:49:39.022556 django-pony-express-1.0.2/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-05-04 10:15:00.716470 django-pony-express-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0      677 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/manage.py
+-rw-r--r--   0        0        0     3575 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-04 10:15:00.700870 django-pony-express-1.0.2/pytest.init
+-rw-r--r--   0        0        0     1682 2023-05-03 13:31:21.061433 django-pony-express-1.0.2/settings.py
+-rw-r--r--   0        0        0       69 2023-05-04 10:15:00.700870 django-pony-express-1.0.2/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/testapp/__init__.py
+-rw-r--r--   0        0        0      145 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/testapp/templates/testapp/test_email.html
+-rw-r--r--   0        0        0      148 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/testapp/templates/testapp/test_email.txt
+-rw-r--r--   0        0        0      144 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/testapp/urls.py
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/tests/files/testfile.txt
+-rw-r--r--   0        0        0     9590 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/tests/test_email_test_service.py
+-rw-r--r--   0        0        0    15614 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/tests/test_mail_services.py
+-rw-r--r--   0        0        0     7089 1970-01-01 00:00:00.000000 django-pony-express-1.0.2/PKG-INFO
```

### Comparing `django-pony-express-1.0.1/.ambient-package-update/metadata.py` & `django-pony-express-1.0.2/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/.github/workflows/ci.yml` & `django-pony-express-1.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/.gitignore` & `django-pony-express-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/.pre-commit-config.yaml` & `django-pony-express-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/.readthedocs.yml` & `django-pony-express-1.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/LICENSE.md` & `django-pony-express-1.0.2/LICENSE.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2012-2023 Ambient
+Copyright (c) 2012-2023 Ambient Innovation: GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-pony-express-1.0.1/README.md` & `django-pony-express-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ## Contribute
 
 ### Setup package for development
 
 - Create a Python virtualenv and activate it
 - Install "pip-tools" with `pip install pip-tools`
-- Compile the requirements with `pip-compile --extra dev -o requirements.txt pyproject.toml --resolver=backtracking`
+- Compile the requirements with `pip-compile --extra dev, -o requirements.txt pyproject.toml --resolver=backtracking`
 - Sync the dependencies with your virtualenv with `pip-sync`
 
 ### Add functionality
 
 - Create a new branch for your feature
 - Change the dependency in your requirements.txt to a local (editable) one that points to your local file system:
   `-e /Users/workspace/django-pony-express` or via pip  `pip install -e /Users/workspace/django-pony-express`
@@ -109,23 +109,23 @@
 ### Translation files
 
 If you have added custom text, make sure to wrap it in `_()` where `_` is
 gettext_lazy (`from django.utils.translation import gettext_lazy as _`).
 
 How to create translation file:
 
-* Navigate to `django-pony-express` (the inner directory!)
+* Navigate to `django-pony-express`
 * `python manage.py makemessages -l de`
-* Have a look at the new/changed files within `django-pony-express/locale`
+* Have a look at the new/changed files within `django_pony_express/locale`
 
 How to compile translation files:
 
-* Navigate to `django-pony-express` (the inner directory!)
+* Navigate to `django-pony-express`
 * `python manage.py compilemessages`
-* Have a look at the new/changed files within `django-pony-express/locale`
+* Have a look at the new/changed files within `django_pony_express/locale`
 
 ### Publish to ReadTheDocs.io
 
 - Fetch the latest changes in GitHub mirror and push them
 - Trigger new build at ReadTheDocs.io (follow instructions in admin panel at RTD) if the GitHub webhook is not yet set
   up.
```

### Comparing `django-pony-express-1.0.1/django_pony_express/locale/de/LC_MESSAGES/django.po` & `django-pony-express-1.0.2/django_pony_express/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/django_pony_express/services/base.py` & `django-pony-express-1.0.2/django_pony_express/services/base.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/django_pony_express/services/tests.py` & `django-pony-express-1.0.2/django_pony_express/services/tests.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/docs/Makefile` & `django-pony-express-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/docs/conf.py` & `django-pony-express-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/docs/features/mail.md` & `django-pony-express-1.0.2/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/docs/features/tests.md` & `django-pony-express-1.0.2/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/docs/make.bat` & `django-pony-express-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/manage.py` & `django-pony-express-1.0.2/manage.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/pyproject.toml` & `django-pony-express-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/settings.py` & `django-pony-express-1.0.2/settings.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/tests/test_email_test_service.py` & `django-pony-express-1.0.2/tests/test_email_test_service.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/tests/test_mail_services.py` & `django-pony-express-1.0.2/tests/test_mail_services.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.1/PKG-INFO` & `django-pony-express-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pony-express
-Version: 1.0.1
+Version: 1.0.2
 Summary: Class-based emails including a test suite for Django
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
@@ -98,15 +98,15 @@
 
 ## Contribute
 
 ### Setup package for development
 
 - Create a Python virtualenv and activate it
 - Install "pip-tools" with `pip install pip-tools`
-- Compile the requirements with `pip-compile --extra dev -o requirements.txt pyproject.toml --resolver=backtracking`
+- Compile the requirements with `pip-compile --extra dev, -o requirements.txt pyproject.toml --resolver=backtracking`
 - Sync the dependencies with your virtualenv with `pip-sync`
 
 ### Add functionality
 
 - Create a new branch for your feature
 - Change the dependency in your requirements.txt to a local (editable) one that points to your local file system:
   `-e /Users/workspace/django-pony-express` or via pip  `pip install -e /Users/workspace/django-pony-express`
@@ -153,23 +153,23 @@
 ### Translation files
 
 If you have added custom text, make sure to wrap it in `_()` where `_` is
 gettext_lazy (`from django.utils.translation import gettext_lazy as _`).
 
 How to create translation file:
 
-* Navigate to `django-pony-express` (the inner directory!)
+* Navigate to `django-pony-express`
 * `python manage.py makemessages -l de`
-* Have a look at the new/changed files within `django-pony-express/locale`
+* Have a look at the new/changed files within `django_pony_express/locale`
 
 How to compile translation files:
 
-* Navigate to `django-pony-express` (the inner directory!)
+* Navigate to `django-pony-express`
 * `python manage.py compilemessages`
-* Have a look at the new/changed files within `django-pony-express/locale`
+* Have a look at the new/changed files within `django_pony_express/locale`
 
 ### Publish to ReadTheDocs.io
 
 - Fetch the latest changes in GitHub mirror and push them
 - Trigger new build at ReadTheDocs.io (follow instructions in admin panel at RTD) if the GitHub webhook is not yet set
   up.
```

