# Comparing `tmp/ambient-package-update-23.5.4.tar.gz` & `tmp/ambient-package-update-23.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-package-update-23.5.4.tar", last modified: Thu May  4 12:00:31 2023, max compression
+gzip compressed data, was "ambient-package-update-23.5.5.tar", last modified: Thu May  4 14:01:38 2023, max compression
```

## Comparing `ambient-package-update-23.5.4.tar` & `ambient-package-update-23.5.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/.gitignore
--rw-r--r--   0        0        0      904 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      259 2023-05-04 11:59:17.650370 ambient-package-update-23.5.4/CHANGES.md
--rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/LICENSE.md
--rw-r--r--   0        0        0     1825 2023-05-03 14:09:31.363845 ambient-package-update-23.5.4/README.md
--rw-r--r--   0        0        0       93 2023-05-04 11:59:17.666000 ambient-package-update-23.5.4/ambient_package_update/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      396 2023-05-04 12:00:18.977729 ambient-package-update-23.5.4/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0     3526 2023-05-03 13:01:45.765213 ambient-package-update-23.5.4/main.py
--rw-r--r--   0        0        0     2472 2023-05-03 13:55:44.475467 ambient-package-update-23.5.4/pyproject.toml
--rw-r--r--   0        0        0     1820 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/requirements.txt
--rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/scripts/setup_venv.ps1
--rw-r--r--   0        0        0       82 2023-05-04 09:31:48.690822 ambient-package-update-23.5.4/templates/.coveragerc.tpl
--rw-r--r--   0        0        0      288 2023-05-04 09:25:12.333150 ambient-package-update-23.5.4/templates/.editorconfig.tpl
--rw-r--r--   0        0        0     1780 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      904 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/templates/.readthedocs.yml.tpl
--rw-r--r--   0        0        0     1121 2023-05-04 09:29:00.483983 ambient-package-update-23.5.4/templates/LICENSE.md.tpl
--rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     4625 2023-05-04 09:47:17.310181 ambient-package-update-23.5.4/templates/Readme.md.tpl
--rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     3580 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0       56 2023-05-04 09:29:24.289641 ambient-package-update-23.5.4/templates/pytest.init.tpl
--rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.4/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 ambient-package-update-23.5.4/PKG-INFO
+-rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/.gitignore
+-rw-r--r--   0        0        0      904 2023-05-04 13:34:24.555311 ambient-package-update-23.5.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      305 2023-05-04 14:01:17.467891 ambient-package-update-23.5.5/CHANGES.md
+-rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/LICENSE.md
+-rw-r--r--   0        0        0     1861 2023-05-04 13:44:21.438513 ambient-package-update-23.5.5/README.md
+-rw-r--r--   0        0        0       93 2023-05-04 14:00:38.526432 ambient-package-update-23.5.5/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      396 2023-05-04 14:00:38.526432 ambient-package-update-23.5.5/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0     3526 2023-05-03 13:01:45.765213 ambient-package-update-23.5.5/main.py
+-rw-r--r--   0        0        0     2550 2023-05-04 13:59:19.861070 ambient-package-update-23.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1820 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/requirements.txt
+-rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/scripts/setup_venv.ps1
+-rw-r--r--   0        0        0       82 2023-05-04 09:31:48.690822 ambient-package-update-23.5.5/templates/.coveragerc.tpl
+-rw-r--r--   0        0        0      288 2023-05-04 09:25:12.333150 ambient-package-update-23.5.5/templates/.editorconfig.tpl
+-rw-r--r--   0        0        0     1784 2023-05-04 13:49:38.761775 ambient-package-update-23.5.5/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      904 2023-05-04 13:34:24.540644 ambient-package-update-23.5.5/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/.readthedocs.yml.tpl
+-rw-r--r--   0        0        0     1121 2023-05-04 09:29:00.483983 ambient-package-update-23.5.5/templates/LICENSE.md.tpl
+-rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     4625 2023-05-04 09:47:17.310181 ambient-package-update-23.5.5/templates/Readme.md.tpl
+-rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     3742 2023-05-04 13:33:46.734472 ambient-package-update-23.5.5/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0       56 2023-05-04 09:29:24.289641 ambient-package-update-23.5.5/templates/pytest.init.tpl
+-rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.5/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 ambient-package-update-23.5.5/PKG-INFO
```

### Comparing `ambient-package-update-23.5.4/.gitignore` & `ambient-package-update-23.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/.pre-commit-config.yaml` & `ambient-package-update-23.5.5/.pre-commit-config.yaml`

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

### Comparing `ambient-package-update-23.5.4/LICENSE.md` & `ambient-package-update-23.5.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/README.md` & `ambient-package-update-23.5.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 ## Usage
 
 * python .\main.py render-templates [PACKAGE_NAME]
 
 todo:
 - write usage paragraph
+- docs how to create a new package
 - create template dirs if not existing (without .github/workflows it's failing)
 - package-readme hat dopplungen zu docs und enthält zeug, das nicht da drinstehen muss
 - ambient-toolbox branch löschen und nur rest von core da ablegen
 
 ## Contribution
 
 ### Publish to PyPi
```

### Comparing `ambient-package-update-23.5.4/ambient_package_update/metadata/package.py` & `ambient-package-update-23.5.5/ambient_package_update/metadata/package.py`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/main.py` & `ambient-package-update-23.5.5/main.py`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/pyproject.toml` & `ambient-package-update-23.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     'keyring~=23.13',
     # Linting
     'pre-commit~=3.2',
     'black~=23.3',
 ]
 
 [project.urls]
+'Homepage' = 'https://github.com/ambient-innovation/ambient-package-update/'
 'Documentation' = 'https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md'
 'Maintained by' = 'https://ambient.digital/'
 'Bugtracker' = 'https://github.com/ambient-innovation/ambient-package-update/issues'
 'Changelog' = 'https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md'
 
 [tool.black]
 line-length = 120
```

### Comparing `ambient-package-update-23.5.4/requirements.txt` & `ambient-package-update-23.5.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/templates/.github/workflows/ci.yml.tpl` & `ambient-package-update-23.5.5/templates/.github/workflows/ci.yml.tpl`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
   build:
     name: Python ${% raw %}{{ matrix.python-version }}{% endraw %}, django ${% raw %}{{ matrix.django-version }}{% endraw %}
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

### Comparing `ambient-package-update-23.5.4/templates/.pre-commit-config.yaml.tpl` & `ambient-package-update-23.5.5/templates/.pre-commit-config.yaml.tpl`

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

### Comparing `ambient-package-update-23.5.4/templates/.readthedocs.yml.tpl` & `ambient-package-update-23.5.5/templates/.readthedocs.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/templates/LICENSE.md.tpl` & `ambient-package-update-23.5.5/templates/LICENSE.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/templates/Readme.md.tpl` & `ambient-package-update-23.5.5/templates/Readme.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/templates/docs/Makefile.tpl` & `ambient-package-update-23.5.5/templates/docs/Makefile.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/templates/docs/conf.py.tpl` & `ambient-package-update-23.5.5/templates/docs/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/templates/docs/make.bat.tpl` & `ambient-package-update-23.5.5/templates/docs/make.bat.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.4/templates/pyproject.toml.tpl` & `ambient-package-update-23.5.5/templates/pyproject.toml.tpl`

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
@@ -41,14 +42,15 @@
    '{{ dependency }}',{% endfor %}
 ]{% endfor %}{% endif %}
 
 [tool.flit.module]
 name = "{{ package_name }}"
 
 [project.urls]
+'Homepage' = 'https://github.com/ambient-innovation/{{ package_name|replace("_", "-") }}/'
 'Documentation' = 'https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html'
 'Maintained by' = 'https://ambient.digital/'
 'Bugtracker' = 'https://github.com/ambient-innovation/{{ package_name|replace("_", "-") }}/issues'
 'Changelog' = 'https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/features/changelog.html'
 
 
 [tool.black]
@@ -100,25 +102,26 @@
 
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
 extras = {% for area, dependency_list in optional_dependencies.items() %}{{ area }},{% endfor %}
 commands =
     pytest --ds settings tests
 
 [gh-actions]
 python =
     3.8: py38
```

### Comparing `ambient-package-update-23.5.4/PKG-INFO` & `ambient-package-update-23.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-package-update
-Version: 23.5.4
+Version: 23.5.5
 Summary: Ambient package update tool for clean and swift maintenance
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,15 @@
 Requires-Dist: flit~=3.8
 Requires-Dist: keyring~=23.13
 Requires-Dist: pre-commit~=3.2
 Requires-Dist: black~=23.3
 Project-URL: Bugtracker, https://github.com/ambient-innovation/ambient-package-update/issues
 Project-URL: Changelog, https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md
 Project-URL: Documentation, https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md
+Project-URL: Homepage, https://github.com/ambient-innovation/ambient-package-update/
 Project-URL: Maintained by, https://ambient.digital/
 
 [![pypi](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.python.org/pypi/ambient-package-update/)
 [![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 
 # Ambient Package Update
 
@@ -45,14 +46,15 @@
 
 ## Usage
 
 * python .\main.py render-templates [PACKAGE_NAME]
 
 todo:
 - write usage paragraph
+- docs how to create a new package
 - create template dirs if not existing (without .github/workflows it's failing)
 - package-readme hat dopplungen zu docs und enthält zeug, das nicht da drinstehen muss
 - ambient-toolbox branch löschen und nur rest von core da ablegen
 
 ## Contribution
 
 ### Publish to PyPi
```

