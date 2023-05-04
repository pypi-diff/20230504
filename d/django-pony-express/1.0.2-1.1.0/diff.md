# Comparing `tmp/django-pony-express-1.0.2.tar.gz` & `tmp/django-pony-express-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pony-express-1.0.2.tar", last modified: Thu May  4 10:16:56 2023, max compression
+gzip compressed data, was "django-pony-express-1.1.0.tar", last modified: Thu May  4 13:58:29 2023, max compression
```

## Comparing `django-pony-express-1.0.2.tar` & `django-pony-express-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2346 2023-05-03 13:52:42.132917 django-pony-express-1.0.2/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0       82 2023-05-04 10:15:00.669626 django-pony-express-1.0.2/.coveragerc
--rw-r--r--   0        0        0      288 2023-05-04 10:15:00.669626 django-pony-express-1.0.2/.editorconfig
--rw-r--r--   0        0        0     1696 2023-05-04 10:15:00.700870 django-pony-express-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3299 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/.gitignore
--rw-r--r--   0        0        0      904 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      551 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/.readthedocs.yml
--rw-r--r--   0        0        0      297 2023-05-04 10:16:33.609693 django-pony-express-1.0.2/CHANGES.md
--rw-r--r--   0        0        0     1107 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/LICENSE.md
--rw-r--r--   0        0        0      138 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/MANIFEST.in
--rw-r--r--   0        0        0     5227 2023-05-04 10:15:00.700870 django-pony-express-1.0.2/README.md
--rw-r--r--   0        0        0       82 2023-05-04 10:16:33.593983 django-pony-express-1.0.2/django_pony_express/__init__.py
--rw-r--r--   0        0        0      120 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/django_pony_express/errors.py
--rw-r--r--   0        0        0     1607 2023-05-03 13:32:01.959010 django-pony-express-1.0.2/django_pony_express/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/django_pony_express/services/__init__.py
--rw-r--r--   0        0        0    11273 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/django_pony_express/services/base.py
--rw-r--r--   0        0        0    10121 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/django_pony_express/services/tests.py
--rw-r--r--   0        0        0      654 2023-05-04 10:15:00.719977 django-pony-express-1.0.2/docs/Makefile
--rw-r--r--   0        0        0     2819 2023-05-04 10:15:00.716470 django-pony-express-1.0.2/docs/conf.py
--rw-r--r--   0        0        0       33 2023-05-03 13:34:58.443495 django-pony-express-1.0.2/docs/features/changelog.rst
--rw-r--r--   0        0        0     9661 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/docs/features/mail.md
--rw-r--r--   0        0        0     5069 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/docs/features/tests.md
--rw-r--r--   0        0        0      282 2023-05-03 13:49:39.022556 django-pony-express-1.0.2/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-05-04 10:15:00.716470 django-pony-express-1.0.2/docs/make.bat
--rw-r--r--   0        0        0      677 2023-05-02 10:13:55.084628 django-pony-express-1.0.2/manage.py
--rw-r--r--   0        0        0     3575 2023-05-04 10:15:00.685214 django-pony-express-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-04 10:15:00.700870 django-pony-express-1.0.2/pytest.init
--rw-r--r--   0        0        0     1682 2023-05-03 13:31:21.061433 django-pony-express-1.0.2/settings.py
--rw-r--r--   0        0        0       69 2023-05-04 10:15:00.700870 django-pony-express-1.0.2/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/testapp/__init__.py
--rw-r--r--   0        0        0      145 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/testapp/templates/testapp/test_email.html
--rw-r--r--   0        0        0      148 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/testapp/templates/testapp/test_email.txt
--rw-r--r--   0        0        0      144 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/testapp/urls.py
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/tests/files/testfile.txt
--rw-r--r--   0        0        0     9590 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/tests/test_email_test_service.py
--rw-r--r--   0        0        0    15614 2023-05-02 10:13:55.100253 django-pony-express-1.0.2/tests/test_mail_services.py
--rw-r--r--   0        0        0     7089 1970-01-01 00:00:00.000000 django-pony-express-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2346 2023-05-03 13:52:42.132917 django-pony-express-1.1.0/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0       82 2023-05-04 13:52:30.444591 django-pony-express-1.1.0/.coveragerc
+-rw-r--r--   0        0        0      288 2023-05-04 13:52:30.444591 django-pony-express-1.1.0/.editorconfig
+-rw-r--r--   0        0        0     1700 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3299 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/.gitignore
+-rw-r--r--   0        0        0      904 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      551 2023-05-04 13:52:30.451097 django-pony-express-1.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0      370 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/CHANGES.md
+-rw-r--r--   0        0        0     1107 2023-05-04 13:52:30.451097 django-pony-express-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-05-04 13:52:30.451097 django-pony-express-1.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     5227 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/README.md
+-rw-r--r--   0        0        0       85 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/django_pony_express/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/django_pony_express/errors.py
+-rw-r--r--   0        0        0     1607 2023-05-03 13:32:01.959010 django-pony-express-1.1.0/django_pony_express/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/django_pony_express/services/__init__.py
+-rw-r--r--   0        0        0    11273 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/django_pony_express/services/base.py
+-rw-r--r--   0        0        0    10121 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/django_pony_express/services/tests.py
+-rw-r--r--   0        0        0      654 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0     2819 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-05-03 13:34:58.443495 django-pony-express-1.1.0/docs/features/changelog.rst
+-rw-r--r--   0        0        0     9661 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/docs/features/mail.md
+-rw-r--r--   0        0        0     5069 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/docs/features/tests.md
+-rw-r--r--   0        0        0      282 2023-05-03 13:49:39.022556 django-pony-express-1.1.0/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0      677 2023-05-02 10:13:55.084628 django-pony-express-1.1.0/manage.py
+-rw-r--r--   0        0        0     3720 2023-05-04 13:58:11.972100 django-pony-express-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-04 13:52:30.451097 django-pony-express-1.1.0/pytest.init
+-rw-r--r--   0        0        0     1682 2023-05-03 13:31:21.061433 django-pony-express-1.1.0/settings.py
+-rw-r--r--   0        0        0       69 2023-05-04 13:52:30.466775 django-pony-express-1.1.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/testapp/__init__.py
+-rw-r--r--   0        0        0      145 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/testapp/templates/testapp/test_email.html
+-rw-r--r--   0        0        0      148 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/testapp/templates/testapp/test_email.txt
+-rw-r--r--   0        0        0      144 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/testapp/urls.py
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/tests/files/testfile.txt
+-rw-r--r--   0        0        0     9590 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/tests/test_email_test_service.py
+-rw-r--r--   0        0        0    15614 2023-05-02 10:13:55.100253 django-pony-express-1.1.0/tests/test_mail_services.py
+-rw-r--r--   0        0        0     7210 1970-01-01 00:00:00.000000 django-pony-express-1.1.0/PKG-INFO
```

### Comparing `django-pony-express-1.0.2/.ambient-package-update/metadata.py` & `django-pony-express-1.1.0/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/.github/workflows/ci.yml` & `django-pony-express-1.1.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
   build:
     name: Python ${{ matrix.python-version }}, django ${{ matrix.django-version }}
     runs-on: ubuntu-22.04
     strategy:
       matrix:
         python-version: [3.8, 3.9, '3.10', '3.11']
-        django-version: [22, 30, 31, 32, 40, 41]
+        django-version: [22, 30, 31, 32, 40, 41, 42]
 
         exclude:
           - python-version: '3.11'
             django-version: 40
           - python-version: '3.11'
             django-version: 32
           - python-version: '3.10'
```

### Comparing `django-pony-express-1.0.2/.gitignore` & `django-pony-express-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/.pre-commit-config.yaml` & `django-pony-express-1.1.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # you find the full pre-commit-tools docu under:
 # https://pre-commit.com/
 
 repos:
   - repo: https://github.com/ambv/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: [ --check, --diff, --config, ./pyproject.toml ]
         language_version: python3.11
         stages: [ push ]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.263'
+    rev: 'v0.0.264'
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.3.2
     hooks:
       - id: pyupgrade
         args: [ --py38-plus ]
         language_version: python3.11
         stages: [ push ]
 
   - repo: https://github.com/adamchainz/django-upgrade
```

### Comparing `django-pony-express-1.0.2/.readthedocs.yml` & `django-pony-express-1.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/LICENSE.md` & `django-pony-express-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/README.md` & `django-pony-express-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/django_pony_express/locale/de/LC_MESSAGES/django.po` & `django-pony-express-1.1.0/django_pony_express/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/django_pony_express/services/base.py` & `django-pony-express-1.1.0/django_pony_express/services/base.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/django_pony_express/services/tests.py` & `django-pony-express-1.1.0/django_pony_express/services/tests.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/docs/Makefile` & `django-pony-express-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/docs/conf.py` & `django-pony-express-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/docs/features/mail.md` & `django-pony-express-1.1.0/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/docs/features/tests.md` & `django-pony-express-1.1.0/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/docs/make.bat` & `django-pony-express-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/manage.py` & `django-pony-express-1.1.0/manage.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/pyproject.toml` & `django-pony-express-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
@@ -45,21 +46,22 @@
    'pre-commit~=3.2',
    'black~=23.3',
    'Django~=3.2',
    'sphinx==4.2.0',
    'sphinx-rtd-theme==1.0.0',
    'm2r2==0.3.1',
    'mistune<2.0.0',
-   'ambient-package-update~=23.5.1',
+   'ambient-package-update~=23.5.4',
 ]
 
 [tool.flit.module]
 name = "django_pony_express"
 
 [project.urls]
+'Homepage' = 'https://github.com/ambient-innovation/django-pony-express/'
 'Documentation' = 'https://django-pony-express.readthedocs.io/en/latest/index.html'
 'Maintained by' = 'https://ambient.digital/'
 'Bugtracker' = 'https://github.com/ambient-innovation/django-pony-express/issues'
 'Changelog' = 'https://django-pony-express.readthedocs.io/en/latest/features/changelog.html'
 
 
 [tool.black]
@@ -114,25 +116,26 @@
 
 # Assume Python 3.11
 target-version = "py311"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py{38,39,310,311}-django{22,30,31,32,40,41}
+envlist = py{38,39,310,311}-django{22,30,31,32,40,41,42}
 isolated_build = True
 
 [testenv]
 deps =
     django22: Django>=2.2.28,<3.0
     django30: Django>=3.0,<3.1
     django31: Django>=3.1,<3.2
     django32: Django>=3.2,<3.3
     django40: Django>=4.0,<4.1
     django41: Django>=4.1,<4.2
+    django42: Django>=4.2,<4.3
 extras = dev,
 commands =
     pytest --ds settings tests
 
 [gh-actions]
 python =
     3.8: py38
```

### Comparing `django-pony-express-1.0.2/settings.py` & `django-pony-express-1.1.0/settings.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/tests/test_email_test_service.py` & `django-pony-express-1.1.0/tests/test_email_test_service.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/tests/test_mail_services.py` & `django-pony-express-1.1.0/tests/test_mail_services.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.2/PKG-INFO` & `django-pony-express-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-pony-express
-Version: 1.0.2
+Version: 1.1.0
 Summary: Class-based emails including a test suite for Django
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -31,18 +32,19 @@
 Requires-Dist: pre-commit~=3.2 ; extra == "dev"
 Requires-Dist: black~=23.3 ; extra == "dev"
 Requires-Dist: Django~=3.2 ; extra == "dev"
 Requires-Dist: sphinx==4.2.0 ; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.0.0 ; extra == "dev"
 Requires-Dist: m2r2==0.3.1 ; extra == "dev"
 Requires-Dist: mistune<2.0.0 ; extra == "dev"
-Requires-Dist: ambient-package-update~=23.5.1 ; extra == "dev"
+Requires-Dist: ambient-package-update~=23.5.4 ; extra == "dev"
 Project-URL: Bugtracker, https://github.com/ambient-innovation/django-pony-express/issues
 Project-URL: Changelog, https://django-pony-express.readthedocs.io/en/latest/features/changelog.html
 Project-URL: Documentation, https://django-pony-express.readthedocs.io/en/latest/index.html
+Project-URL: Homepage, https://github.com/ambient-innovation/django-pony-express/
 Project-URL: Maintained by, https://ambient.digital/
 Provides-Extra: dev
 
 [![pypi](https://img.shields.io/pypi/v/django-pony-express.svg)](https://pypi.python.org/pypi/django-pony-express/)
 [![Downloads](https://pepy.tech/badge/django-pony-express)](https://pepy.tech/project/django-pony-express)
 [![Documentation Status](https://readthedocs.org/projects/django-pony-express/badge/?version=latest)](https://django-pony-express.readthedocs.io/en/latest/?badge=latest)
```

