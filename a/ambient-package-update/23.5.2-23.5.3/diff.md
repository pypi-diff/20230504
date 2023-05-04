# Comparing `tmp/ambient-package-update-23.5.2.tar.gz` & `tmp/ambient-package-update-23.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-package-update-23.5.2.tar", last modified: Wed May  3 13:02:39 2023, max compression
+gzip compressed data, was "ambient-package-update-23.5.3.tar", last modified: Wed May  3 13:57:20 2023, max compression
```

## Comparing `ambient-package-update-23.5.2.tar` & `ambient-package-update-23.5.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/.gitignore
--rw-r--r--   0        0        0      904 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/LICENSE.md
--rw-r--r--   0        0        0     1695 2023-05-03 13:01:45.777494 ambient-package-update-23.5.2/README.md
--rw-r--r--   0        0        0       93 2023-05-03 13:01:45.765213 ambient-package-update-23.5.2/ambient_package_update/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      396 2023-05-03 13:01:45.749587 ambient-package-update-23.5.2/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0     3526 2023-05-03 13:01:45.765213 ambient-package-update-23.5.2/main.py
--rw-r--r--   0        0        0     2481 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/pyproject.toml
--rw-r--r--   0        0        0     1820 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/requirements.txt
--rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/scripts/setup_venv.ps1
--rw-r--r--   0        0        0     1780 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      904 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/.readthedocs.yml.tpl
--rw-r--r--   0        0        0     1104 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/LICENSE.md.tpl
--rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     4485 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/Readme.md.tpl
--rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     3580 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.2/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 ambient-package-update-23.5.2/PKG-INFO
+-rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/.gitignore
+-rw-r--r--   0        0        0      904 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      179 2023-05-03 13:54:59.114132 ambient-package-update-23.5.3/CHANGES.md
+-rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/LICENSE.md
+-rw-r--r--   0        0        0     1690 2023-05-03 13:55:44.475467 ambient-package-update-23.5.3/README.md
+-rw-r--r--   0        0        0       93 2023-05-03 13:54:59.104122 ambient-package-update-23.5.3/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      396 2023-05-03 13:01:45.749587 ambient-package-update-23.5.3/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0     3526 2023-05-03 13:01:45.765213 ambient-package-update-23.5.3/main.py
+-rw-r--r--   0        0        0     2472 2023-05-03 13:55:44.475467 ambient-package-update-23.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1820 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/requirements.txt
+-rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/scripts/setup_venv.ps1
+-rw-r--r--   0        0        0     1780 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      904 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/.readthedocs.yml.tpl
+-rw-r--r--   0        0        0     1104 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/LICENSE.md.tpl
+-rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     4623 2023-05-03 13:48:27.801512 ambient-package-update-23.5.3/templates/Readme.md.tpl
+-rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     3580 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.3/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 ambient-package-update-23.5.3/PKG-INFO
```

### Comparing `ambient-package-update-23.5.2/.gitignore` & `ambient-package-update-23.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/.pre-commit-config.yaml` & `ambient-package-update-23.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/LICENSE.md` & `ambient-package-update-23.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/ambient_package_update/metadata/package.py` & `ambient-package-update-23.5.3/ambient_package_update/metadata/package.py`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/main.py` & `ambient-package-update-23.5.3/main.py`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/pyproject.toml` & `ambient-package-update-23.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     'black~=23.3',
 ]
 
 [project.urls]
 'Documentation' = 'https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md'
 'Maintained by' = 'https://ambient.digital/'
 'Bugtracker' = 'https://github.com/ambient-innovation/ambient-package-update/issues'
-'Changelog' = 'https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md#Changelog'
+'Changelog' = 'https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md'
 
 [tool.black]
 line-length = 120
 multi_line_output = 3
 skip-string-normalization = true
 include_trailing_comma = true
```

### Comparing `ambient-package-update-23.5.2/requirements.txt` & `ambient-package-update-23.5.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/templates/.github/workflows/ci.yml.tpl` & `ambient-package-update-23.5.3/templates/.github/workflows/ci.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/templates/.pre-commit-config.yaml.tpl` & `ambient-package-update-23.5.3/templates/.pre-commit-config.yaml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/templates/.readthedocs.yml.tpl` & `ambient-package-update-23.5.3/templates/.readthedocs.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/templates/LICENSE.md.tpl` & `ambient-package-update-23.5.3/templates/LICENSE.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/templates/Readme.md.tpl` & `ambient-package-update-23.5.3/templates/Readme.md.tpl`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [![pypi](https://img.shields.io/pypi/v/{{ package_name|replace("_", "-") }}.svg)](https://pypi.python.org/pypi/{{ package_name|replace("_", "-") }}/)
 [![Downloads](https://pepy.tech/badge/{{ package_name|replace("_", "-") }})](https://pepy.tech/project/{{ package_name|replace("_", "-") }})
 [![Documentation Status](https://readthedocs.org/projects/{{ package_name|replace("_", "-") }}/badge/?version=latest)](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/?badge=latest)
 
-**{{ readme_content.tagline }}**
+{{ readme_content.tagline }}
 
-Full documentation for the project is available at [readthedocs.io](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html).
-
-Created and maintained by [Ambient Digital](https://ambient.digital).
-
----
+* [PyPI](https://pypi.org/project/{{ package_name|replace("_", "-") }}/)
+* [GitHub](https://github.com/ambient-innovation/{{ package_name|replace("_", "-") }})
+* [Full documentation](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html)
+* Creator & Maintainer: [Ambient Digital](https://ambient.digital)
 
 {{ readme_content.content }}
 
-# Installation
+## Installation
 
 - Install the package via pip:
 
   `pip install {{ package_name|replace("_", "-") }}`
 
   or via pipenv:
 
@@ -27,39 +26,39 @@
     ````
     INSTALLED_APPS = (
         ...
         '{{ package_name }}',
     )
      ````
 
-# Contribute
+## Contribute
 
-## Setup package for development
+### Setup package for development
 
 - Create a Python virtualenv and activate it
 - Install "pip-tools" with `pip install pip-tools`
 - Compile the requirements with `pip-compile --extra dev -o requirements.txt pyproject.toml --resolver=backtracking`
 - Sync the dependencies with your virtualenv with `pip-sync`
 
-## Add functionality
+### Add functionality
 
 - Create a new branch for your feature
 - Change the dependency in your requirements.txt to a local (editable) one that points to your local file system:
   `-e /Users/workspace/{{ package_name|replace("_", "-") }}` or via pip  `pip install -e /Users/workspace/{{ package_name|replace("_", "-") }}`
 - Ensure the code passes the tests
 - Create a pull request
 
-## Run tests
+### Run tests
 
 - Run tests
   ````
   pytest --ds settings tests
   ````
 
-## Git hooks (via pre-commit)
+### Git hooks (via pre-commit)
 
 We use pre-push hooks to ensure that only linted code reaches our remote repository and pipelines aren't triggered in
 vain.
 
 To enable the configured pre-push hooks, you need to [install](https://pre-commit.com/) pre-commit and run once:
 
     pre-commit install -t pre-push -t pre-commit --install-hooks
@@ -76,43 +75,43 @@
 
     pre-commit run ruff --all-files --hook-stage push
 
 Example: run all hooks of pre-push stage
 
     pre-commit run --all-files --hook-stage push
 
-## Update documentation
+### Update documentation
 
 - To build the documentation run: `sphinx-build docs/ docs/_build/html/`.
 - Open `docs/_build/html/index.html` to see the documentation.
 
-## Translation files
+### Translation files
 
 If you have added custom text, make sure to wrap it in `_()` where `_` is
 gettext_lazy (`from django.utils.translation import gettext_lazy as _`).
 
 How to create translation file:
 
-* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
+* Navigate to `{{ package_name|replace("_", "-") }}` (the inner directory!)
 * `python manage.py makemessages -l de`
-* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
+* Have a look at the new/changed files within `{{ package_name|replace("_", "-") }}/locale`
 
 How to compile translation files:
 
-* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
+* Navigate to `{{ package_name|replace("_", "-") }}` (the inner directory!)
 * `python manage.py compilemessages`
-* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
+* Have a look at the new/changed files within `{{ package_name|replace("_", "-") }}/locale`
 
-## Publish to ReadTheDocs.io
+### Publish to ReadTheDocs.io
 
 - Fetch the latest changes in GitHub mirror and push them
 - Trigger new build at ReadTheDocs.io (follow instructions in admin panel at RTD) if the GitHub webhook is not yet set
   up.
 
-## Publish to PyPi
+### Publish to PyPi
 
 - Update documentation about new/changed functionality
 
 - Update the `Changelog`
 
 - Increment version in main `__init__.py`
```

### Comparing `ambient-package-update-23.5.2/templates/docs/Makefile.tpl` & `ambient-package-update-23.5.3/templates/docs/Makefile.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/templates/docs/conf.py.tpl` & `ambient-package-update-23.5.3/templates/docs/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/templates/docs/make.bat.tpl` & `ambient-package-update-23.5.3/templates/docs/make.bat.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/templates/pyproject.toml.tpl` & `ambient-package-update-23.5.3/templates/pyproject.toml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.2/PKG-INFO` & `ambient-package-update-23.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-package-update
-Version: 23.5.2
+Version: 23.5.3
 Summary: Ambient package update tool for clean and swift maintenance
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Requires-Dist: typer~=0.7
 Requires-Dist: Jinja2~=3.1
 Requires-Dist: flit~=3.8
 Requires-Dist: keyring~=23.13
 Requires-Dist: pre-commit~=3.2
 Requires-Dist: black~=23.3
 Project-URL: Bugtracker, https://github.com/ambient-innovation/ambient-package-update/issues
-Project-URL: Changelog, https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md#Changelog
+Project-URL: Changelog, https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md
 Project-URL: Documentation, https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md
 Project-URL: Maintained by, https://ambient.digital/
 
 [![pypi](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.python.org/pypi/ambient-package-update/)
 [![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 
 # Ambient Package Update
@@ -72,12 +72,8 @@
 
   ```
   flit publish --repository testpypi
   ```
 
 ## Changelog
 
-**23.5.2**
-* Templates render a trailing newline (to conform with Python linting)
-
-**23.5.1**
-* Initial release
+Can be found at [GitHub](https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md).
```

