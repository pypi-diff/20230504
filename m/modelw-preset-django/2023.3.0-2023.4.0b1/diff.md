# Comparing `tmp/modelw_preset_django-2023.3.0.tar.gz` & `tmp/modelw_preset_django-2023.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_preset_django-2023.3.0.tar", max compression
+gzip compressed data, was "modelw_preset_django-2023.4.0b1.tar", max compression
```

## Comparing `modelw_preset_django-2023.3.0.tar` & `modelw_preset_django-2023.4.0b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      484 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/LICENSE
--rw-r--r--   0        0        0      277 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/README.md
--rw-r--r--   0        0        0     1870 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/pyproject.toml
--rw-r--r--   0        0        0    29199 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/src/model_w/preset/django/__init__.py
--rw-r--r--   0        0        0      400 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/src/model_w/preset/django/drf.py
--rw-r--r--   0        0        0        0 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/src/model_w/preset/django/env_helper/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/src/model_w/preset/django/env_helper/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/src/model_w/preset/django/env_helper/management/commands/__init__.py
--rw-r--r--   0        0        0     2994 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py
--rw-r--r--   0        0        0        0 2023-04-03 16:10:16.384088 modelw_preset_django-2023.3.0/src/model_w/preset/django/py.typed
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 modelw_preset_django-2023.3.0/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-05-04 14:54:08.716745 modelw_preset_django-2023.4.0b1/LICENSE
+-rw-r--r--   0        0        0      277 2023-05-04 14:54:08.716745 modelw_preset_django-2023.4.0b1/README.md
+-rw-r--r--   0        0        0     1903 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0    29199 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/__init__.py
+-rw-r--r--   0        0        0      400 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/drf.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/management/commands/__init__.py
+-rw-r--r--   0        0        0     2994 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/py.typed
+-rw-r--r--   0        0        0     2297 1970-01-01 00:00:00.000000 modelw_preset_django-2023.4.0b1/PKG-INFO
```

### Comparing `modelw_preset_django-2023.3.0/pyproject.toml` & `modelw_preset_django-2023.4.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-preset-django"
-version = "2023.3.0"
+version = "2023.4.0b1"
 packages = [
     {  include = "model_w/preset/django", from = "src" }
 ]
 
 description = "Model W preset for Django"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
@@ -20,14 +20,15 @@
 repository = "https://github.com/ModelW/preset-django"
 homepage = "https://github.com/ModelW/preset-django"
 
 keywords = ["django", "env", "configuration"]
 
 [tool.poetry.dependencies]
 python = '~3.10'
+setuptools = "*"
 Django = {version = "~4.1", extras = ["argon2"]}
 sentry-sdk = "~1.18"
 modelw-env-manager = "~1.0.0b2"
 coloredlogs = "~15.0"
 dj-database-url = "~1.3"
 django-postgres-extra = "~2.0"
 whitenoise = "~6.4"
@@ -54,12 +55,12 @@
 celery = ["celery", "django-celery-results"]
 channels = ["channels", "channels-redis"]
 wagtail = ["wagtail", "wand", "django-storages", "boto3"]
 storages = ["django-storages", "boto3"]
 gunicorn = ["gunicorn"]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `modelw_preset_django-2023.3.0/src/model_w/preset/django/__init__.py` & `modelw_preset_django-2023.4.0b1/src/model_w/preset/django/__init__.py`

 * *Files identical despite different names*

### Comparing `modelw_preset_django-2023.3.0/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py` & `modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py`

 * *Files identical despite different names*

### Comparing `modelw_preset_django-2023.3.0/PKG-INFO` & `modelw_preset_django-2023.4.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-preset-django
-Version: 2023.3.0
+Version: 2023.4.0b1
 Summary: Model W preset for Django
 Home-page: https://github.com/ModelW/preset-django
 License: WTFPL
 Keywords: django,env,configuration
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<3.11
@@ -34,14 +34,15 @@
 Requires-Dist: djangorestframework (>=3.14,<3.15)
 Requires-Dist: djangorestframework-gis (>=1.0,<1.1)
 Requires-Dist: gunicorn (>=20.1,<20.2) ; extra == "gunicorn"
 Requires-Dist: modelw-env-manager (>=1.0.0b2,<1.1.0)
 Requires-Dist: psycopg2 (>=2.9,<2.10)
 Requires-Dist: rich (>=13.3,<13.4)
 Requires-Dist: sentry-sdk (>=1.18,<1.19)
+Requires-Dist: setuptools
 Requires-Dist: wagtail (>=4.1,<4.2) ; extra == "wagtail"
 Requires-Dist: wand (>=0.6,<0.7) ; extra == "wagtail"
 Requires-Dist: whitenoise (>=6.4,<6.5)
 Project-URL: Repository, https://github.com/ModelW/preset-django
 Description-Content-Type: text/markdown
 
 # Model W &mdash; Django Preset
```

