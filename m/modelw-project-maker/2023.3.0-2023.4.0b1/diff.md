# Comparing `tmp/modelw_project_maker-2023.3.0.tar.gz` & `tmp/modelw_project_maker-2023.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_project_maker-2023.3.0.tar", max compression
+gzip compressed data, was "modelw_project_maker-2023.4.0b1.tar", max compression
```

## Comparing `modelw_project_maker-2023.3.0.tar` & `modelw_project_maker-2023.4.0b1.tar`

### file list

```diff
@@ -1,70 +1,82 @@
--rw-r--r--   0        0        0     5377 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/README.md
--rw-r--r--   0        0        0     1344 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/__init__.py
--rw-r--r--   0        0        0     8748 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/__main__.py
--rw-r--r--   0        0        0       45 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/errors.py
--rw-r--r--   0        0        0      143 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/maker/__init__.py
--rw-r--r--   0        0        0     4470 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/maker/_api.py
--rw-r--r--   0        0        0     6518 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/maker/_base.py
--rw-r--r--   0        0        0      703 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/maker/_common.py
--rw-r--r--   0        0        0     3818 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/maker/_front.py
--rw-r--r--   0        0        0     3446 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/namer.py
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/py.typed
--rw-r--r--   0        0        0      178 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/.editorconfig
--rw-r--r--   0        0        0       27 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/.formatignore
--rw-r--r--   0        0        0     3034 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/.gitignore
--rw-r--r--   0        0        0       77 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/.prettierrc
--rw-r--r--   0        0        0     1488 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/README.md
--rw-r--r--   0        0        0     3034 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/.dockerignore
--rw-r--r--   0        0        0      381 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/.env-template
--rw-r--r--   0        0        0      181 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/Dockerfile
--rw-r--r--   0        0        0      236 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/Makefile
--rw-r--r--   0        0        0     1140 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/README.md
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
--rw-r--r--   0        0        0       93 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
--rw-r--r--   0        0        0     8589 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
--rw-r--r--   0        0        0     2818 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
--rw-r--r--   0        0        0     2036 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
--rw-r--r--   0        0        0      655 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
--rw-r--r--   0        0        0       92 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
--rw-r--r--   0        0        0      159 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
--rw-r--r--   0        0        0     3921 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
--rw-r--r--   0        0        0     3150 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
--rw-r--r--   0        0        0     1343 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
--rw-r--r--   0        0        0     2486 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
--rw-r--r--   0        0        0      194 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
--rw-r--r--   0        0        0      386 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
--rw-r--r--   0        0        0       70 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
--rw-r--r--   0        0        0      851 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
--rw-r--r--   0        0        0      273 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
--rw-r--r--   0        0        0      219 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
--rw-r--r--   0        0        0     2076 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
--rw-r--r--   0        0        0     1681 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
--rw-r--r--   0        0        0      443 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
--rwxr-xr-x   0        0        0      666 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/manage.py
--rwxr-xr-x   0        0        0      151 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/pmanage
--rw-r--r--   0        0        0   174544 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/poetry.lock
--rw-r--r--   0        0        0      824 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/pyproject.toml
--rw-r--r--   0        0        0     3034 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/.dockerignore
--rw-r--r--   0        0        0       38 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/.env-template
--rw-r--r--   0        0        0      332 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/.eslintrc.js
--rw-r--r--   0        0        0      185 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/Dockerfile
--rw-r--r--   0        0        0     1699 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/README.md
--rw-r--r--   0        0        0    11068 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/components/ServerTemplatedComponent.vue
--rw-r--r--   0        0        0      112 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/components/blocks/Title1.vue
--rw-r--r--   0        0        0     3212 2023-04-03 16:52:37.537774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/nuxt.config.js
--rw-r--r--   0        0        0  1525810 2023-04-03 16:52:37.545774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/package-lock.json
--rw-r--r--   0        0        0     1235 2023-04-03 16:52:37.545774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/package.json
--rw-r--r--   0        0        0     4248 2023-04-03 16:52:37.545774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/pages/*.vue
--rw-r--r--   0        0        0       80 2023-04-03 16:52:37.545774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
--rw-r--r--   0        0        0      311 2023-04-03 16:52:37.545774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/plugins/axios.js
--rw-r--r--   0        0        0       67 2023-04-03 16:52:37.545774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/vlang.yml
--rw-r--r--   0        0        0     7602 2023-04-03 16:52:37.533774 modelw_project_maker-2023.3.0/src/model_w/project_maker/template.py
--rw-r--r--   0        0        0     6728 1970-01-01 00:00:00.000000 modelw_project_maker-2023.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5377 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/README.md
+-rw-r--r--   0        0        0     1363 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/__init__.py
+-rw-r--r--   0        0        0     8748 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/__main__.py
+-rw-r--r--   0        0        0       45 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/errors.py
+-rw-r--r--   0        0        0      143 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/__init__.py
+-rw-r--r--   0        0        0     4470 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_api.py
+-rw-r--r--   0        0        0     6518 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_base.py
+-rw-r--r--   0        0        0      703 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_common.py
+-rw-r--r--   0        0        0     3909 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_front.py
+-rw-r--r--   0        0        0     3446 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/namer.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/py.typed
+-rw-r--r--   0        0        0      178 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.editorconfig
+-rw-r--r--   0        0        0       27 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.formatignore
+-rw-r--r--   0        0        0     3042 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.gitignore
+-rw-r--r--   0        0        0       77 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.prettierrc
+-rw-r--r--   0        0        0     1488 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/README.md
+-rw-r--r--   0        0        0     3034 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/.dockerignore
+-rw-r--r--   0        0        0      381 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/.env-template
+-rw-r--r--   0        0        0      181 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/Dockerfile
+-rw-r--r--   0        0        0      236 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/Makefile
+-rw-r--r--   0        0        0     1140 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
+-rw-r--r--   0        0        0     8589 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2818 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
+-rw-r--r--   0        0        0      655 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
+-rw-r--r--   0        0        0      233 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
+-rwxr-xr-x   0        0        0      755 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg
+-rwxr-xr-x   0        0        0      240 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/edit.svg
+-rwxr-xr-x   0        0        0      471 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-inverse.svg
+-rwxr-xr-x   0        0        0      844 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg
+-rwxr-xr-x   0        0        0      903 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg
+-rwxr-xr-x   0        0        0     1092 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg
+-rwxr-xr-x   0        0        0      658 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg
+-rwxr-xr-x   0        0        0      718 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg
+-rwxr-xr-x   0        0        0      485 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick.svg
+-rwxr-xr-x   0        0        0     2749 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg
+-rwxr-xr-x   0        0        0     2067 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg
+-rw-r--r--   0        0        0     1883 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html
+-rw-r--r--   0        0        0      159 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
+-rw-r--r--   0        0        0     3921 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
+-rw-r--r--   0        0        0     3150 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
+-rw-r--r--   0        0        0     1343 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
+-rw-r--r--   0        0        0     2486 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
+-rw-r--r--   0        0        0      194 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
+-rw-r--r--   0        0        0       70 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
+-rw-r--r--   0        0        0      851 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
+-rw-r--r--   0        0        0      273 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
+-rw-r--r--   0        0        0      219 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
+-rw-r--r--   0        0        0     2076 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
+-rw-r--r--   0        0        0     1681 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
+-rw-r--r--   0        0        0      443 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
+-rwxr-xr-x   0        0        0      666 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/manage.py
+-rwxr-xr-x   0        0        0      151 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/pmanage
+-rw-r--r--   0        0        0      863 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/pyproject.toml
+-rw-r--r--   0        0        0     3034 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.dockerignore
+-rw-r--r--   0        0        0      182 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.env-template
+-rw-r--r--   0        0        0      332 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.eslintrc.js
+-rw-r--r--   0        0        0        8 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.gitignore
+-rw-r--r--   0        0        0       13 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.nvmrc
+-rw-r--r--   0        0        0      185 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/Dockerfile
+-rw-r--r--   0        0        0     1599 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/README.md
+-rw-r--r--   0        0        0      112 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/components/blocks/title-1.vue
+-rw-r--r--   0        0        0    11485 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/components/server-templated-component.vue
+-rw-r--r--   0        0        0      558 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/nuxt.config.js
+-rw-r--r--   0        0        0      796 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/package.json
+-rw-r--r--   0        0        0     5202 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/pages/[...wagtail].vue
+-rw-r--r--   0        0        0       80 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
+-rw-r--r--   0        0        0      483 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/plugins/dom.client.ts
+-rw-r--r--   0        0        0      505 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/plugins/dom.server.ts
+-rw-r--r--   0        0        0     7602 2023-05-04 15:39:29.282121 modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template.py
+-rw-r--r--   0        0        0     6756 1970-01-01 00:00:00.000000 modelw_project_maker-2023.4.0b1/PKG-INFO
```

### Comparing `modelw_project_maker-2023.3.0/README.md` & `modelw_project_maker-2023.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/pyproject.toml` & `modelw_project_maker-2023.4.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-project-maker"
-version = "2023.3.0"
+version = "2023.4.0b1"
 packages = [
     {  include = "model_w/project_maker", from = "src" }
 ]
 
 description = "A tool to create Model-W-compliant projects"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
@@ -24,14 +24,15 @@
 ]
 
 [tool.poetry.scripts]
 project_maker = "model_w.project_maker.__main__:__main__"
 
 [tool.poetry.dependencies]
 python = "^3.10"
+setuptools = "*"
 rich = "^12.5.1"
 Unidecode = "^1.3.4"
 black = "^22.8.0"
 isort = "^5.10.1"
 tomlkit = "^0.11.4"
 node-edge = "^0.1.0b2"
 monoformat = "^0.1.0b3"
```

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/__main__.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/maker/_api.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_api.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/maker/_base.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_base.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/maker/_common.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_common.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/maker/_front.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/maker/_front.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,19 @@
         if not context["front"]["enable"]:
             return False
 
         if self.path_specs.match_file(path):
             return False
 
         if not context["api"]["wagtail"]:
-            if path.name in {"*.vue", "ServerTemplatedComponent.vue"}:
+            if path.name in {
+                "[...wagtail].vue",
+                "server-templated-component.vue",
+                "title-1.vue",
+            }:
                 return False
         else:
             if path.name == "no-wagtail-index.vue":
                 return False
 
         return True
```

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/namer.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/namer.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/.gitignore` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/README.md` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/.dockerignore` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/README.md` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/manage.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/manage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/api/pyproject.toml` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/api/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     # :: ENDIF
     # :: IF api__wagtail
     "wagtail",
     # :: ENDIF
     # :: IF api__wsgi
     "gunicorn",
     # :: ENDIF
-], version = "~2023.3.0"}
-drf-spectacular = {extras = ["sidecar"], version = "^0.26.1"}
+], version = ">=2023.4.0b1,<2023.7.0", allow-prereleases = true}
+drf-spectacular = {extras = ["sidecar"], version = "^0.26.2"}
 
 [tool.poetry.dev-dependencies]
 black = "*"
 isort = "*"
 ipython = "*"
 
 [tool.isort]
```

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/.dockerignore` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,15 @@
 .cache
 
 # next.js build output
 .next
 
 # nuxt.js build output
 .nuxt
+.output
 
 # Nuxt generate
 dist
 
 # vuepress build output
 .vuepress/dist
```

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/README.md` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,23 +11,20 @@
 ```js
 const user = await $axios.$get("/back/api/me/");
 ```
 
 Doing so will make sure that the call works both on server-side and client-side
 (as we're working with a SSR app here).
 
-The plugin found in [`plugins/axios.js`](./plugins/axios.js) will take care of
-adding the CSRF tokens so that Django doesn't go crazy.
-
 # :: IF api~~wagtail
 
 ## Wagtail
 
 The content pages are served by Wagtail on the Django side. This behavior is
-handled by the [catch-all page](./pages/*.vue) which will:
+handled by the [catch-all page](./pages/[...wagtail].vue) which will:
 
 1. Call the Wagtail API for the page we're trying to get
 2. If there is any error (404, 500, ...) the error will be rendered as a Nuxt
    error. The same goes with redirections.
 3. If the page is found, it will be rendered using the
    [`ServerTemplatedComponent`](./components/ServerTemplatedComponent.vue)
    component. It lets you declare Vue components that have their JS and CSS
@@ -37,10 +34,11 @@
 In order to render more components through the `ServerTemplatedComponent`, you
 must:
 
 1. Create the component itself (wherever you want), without defining a template
 2. In the component's default, add a `selector` property that will be used to
    find in the server-generated HTML the location(s) where this component needs
    to be inserted.
-3. Add this component to [`*.vue`](./pages/*.vue) in the `DEFS` constants.
+3. Add this component to [`[...wagtail].vue`](./pages/[...wagtail].vue) in the
+   `DEFS` constants.
 
 # :: ENDIF
```

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/components/ServerTemplatedComponent.vue` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/components/server-templated-component.vue`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
  *
  * @param tagName {string}
  * @return {string}
  */
 export function camelToSnake(tagName) {
     return tagName
         .split(/(?=[A-Z])/)
-        .filter((x) => x)
+        .filter((x) => !!x)
         .join("-")
         .toLowerCase();
 }
 
 /**
  * The extractContent expects a function that returns a DOM element from a full
  * document. This generates such a function which will extract content based
@@ -22,60 +22,72 @@
  * @return {function(*): *}
  */
 export function extractSelector(selector) {
     return (dom) => dom.querySelector(selector);
 }
 
 /**
- * Converts HTML source code into DOM-like content.
- *
- * On the server this uses the JSDOM lib while on the browser it uses the real
- * DOM API.
- *
- * @param html {string} HTML code you want to parse
- * @return {Document}
- */
-export function htmlToDom(html) {
-    if (process.client) {
-        const parser = new DOMParser();
-        return parser.parseFromString(html, "text/html");
-    } else {
-        const { JSDOM } = require("jsdom");
-        const { document: mockDocument } = new JSDOM(html).window;
-        return mockDocument;
-    }
-}
-
-/**
  * Returns all attributes from a DOM-like element as a dictionary
  */
 function elementToDict(el) {
     const out = {};
 
     for (const { name, value } of el.attributes || []) {
         out[name] = value;
     }
 
     return out;
 }
 
 const propWhitelist = [
-    "mounted",
-    "beforeMount",
+    /**
+    * These are options that comes from the optionApi
+    * that comes with the standard lifecycle of Vue2 and also part of vue3
+    * you can review it in this link https://vuejs.org/api/options-lifecycle.html
+    */
     "beforeCreate",
     "created",
+    "beforeMount",
+    "mounted",
     "beforeUpdate",
     "updated",
-    "beforeDestroy",
-    "destroyed",
+    "beforeUnmount",
+    "unmounted",
+    "setup",
     "data",
     "computed",
     "watch",
     "methods",
     "props",
+    "errorCaptured",
+    "serverPrefetch",
+    /**
+    * These are the methods needed for the composition api,
+    * they help to improve SSR and load speed of the pages.
+    * You can see more information in the next link:
+    * https://vuejs.org/api/composition-api-lifecycle.html#ondeactivated
+    */
+    "onMounted",
+    "onUpdated",
+    "onUnmounted",
+    "onBeforeMount",
+    "onBeforeUpdate",
+    "onBeforeUnmount",
+    "onErrorCaptured",
+    "onActivated",
+    "onDeactivated",
+    /**
+     * The following ones are only for development porpoise
+     */
+    "onRenderTracked",
+    "onRenderTriggered",
+    /**
+     * This is only SSR method
+     */
+    "onServerPrefetch"
 ];
 
 export default {
     props: {
         /**
          * HTML content to derive templates from
          */
@@ -99,24 +111,27 @@
          */
         extractContent: {
             type: Function,
             default: extractSelector("body"),
         },
     },
 
+    emits: ["head"],
+
     computed: {
         /**
          * Extracts all the information from the HTML provided as props:
          *
          * - Uses the "content" (as extracted by extractContent) to generate the
          *   templates for dynamic components (provided by componentsDefs)
          * - Also extracts meta-information from the head (see extractHead())
          */
         templates() {
-            const dom = htmlToDom(this.content);
+            const { $htmlToDom } = useNuxtApp();
+            const dom = $htmlToDom(this.content);
 
             const { contentExtract, components } = this.extractTemplates(dom);
             const head = this.extractHead(dom);
 
             return {
                 base: contentExtract.innerHTML,
                 components,
@@ -324,12 +339,12 @@
     /**
      * We use a render function to be able to provide our dynamic component
      * without having to register it. The dynamic component then becomes the
      * root node of this component and thus this component will be replaced
      * exactly by the HTML code of the content without any superfluous wrapping
      * div.
      */
-    render(createElement) {
-        return createElement(this.dynamicComponent);
+    render() {
+        return h(this.dynamicComponent);
     },
 };
 </script>
```

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template/front/pages/*.vue` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template/front/pages/[...wagtail].vue`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,17 @@
         :content="html"
         :components-defs="defs"
         @head="receiveHeadData"
     />
 </template>
 
 <script>
-import ServerTemplatedComponent from "~/components/ServerTemplatedComponent";
-import Title1 from "~/components/blocks/Title1";
+import { defineNuxtComponent } from "nuxt/app";
+import ServerTemplatedComponent from "~/components/server-templated-component.vue";
+import Title1 from "~/components/blocks/title-1.vue";
 
 /**
  * Put here all the components that you might want to render
  */
 const DEFS = {
     Title1,
 };
@@ -20,15 +21,15 @@
 /**
  * This is the "fall-back" page which will try to fetch and render a page from
  * the underlying Wagtail hosted in the API. Everything here is a sane default,
  * however you might want to customize it depending on your use.
  *
  * The thing you'll want to customize the most is most likely the defs list!
  */
-export default {
+export default defineNuxtComponent({
     components: {
         ServerTemplatedComponent,
     },
 
     /**
      * This is in charge of getting the HTML from the server.
      *
@@ -42,61 +43,80 @@
      * Let's note that this works slightly different depending on if we're
      * running on the server side or the client side. Indeed, on the server
      * you'll have a `$config.apiUrl` value which allows to hit directly the
      * internal API URL, while on the client this value will be undefined and
      * we'll hit the URL relatively to the root path using the `x-reach-api`
      * header to tell the proxy to get this page from the API for us.
      */
-    async asyncData({ $axios, $config, route, error, redirect, $sentry }) {
-        try {
-            return {
-                html: await $axios.$get(route.path, {
-                    baseURL: $config.apiUrl,
-                    headers: { "x-reach-api": "yes" },
-                    maxRedirects: 0,
-                    params: route.query,
-                    validateStatus(status) {
-                        return status === 200;
-                    },
-                }),
-            };
-        } catch (e) {
-            const { response: res } = e;
-
-            if (res) {
-                const isRedirect = res.status === 301 || res.status === 302;
-                const location = res.headers.location;
-
-                if (isRedirect) {
-                    if (location) {
-                        return redirect(res.status, location);
+    async asyncData({ $axios, $config, $router, ssrContext }) {
+        async function getAsyncData($axios, baseURL, path, query) {
+            try {
+                const headers = ssrContext?.event.node.req.headers ?? {};
+                headers["x-reach-api"] = "yes";
+                return {
+                    html: await $axios.$get(path, {
+                        baseURL,
+                        headers,
+                        maxRedirects: 0,
+                        params: query,
+                        validateStatus(status) {
+                            return status === 200;
+                        },
+                    }),
+                };
+            } catch (e) {
+                const { response: res } = e;
+
+                if (res) {
+                    const isRedirect = [301, 302, 307, 308].includes(
+                        res.status
+                    );
+                    const location = res.headers.location;
+
+                    if (isRedirect) {
+                        if (location) {
+                            return await getAsyncData(
+                                $axios,
+                                baseURL,
+                                location,
+                                query
+                            );
+                        } else {
+                            // $sentry.captureException(e);
+                            return createError({
+                                statusCode: res.status,
+                                message: "Invalid redirect",
+                            });
+                        }
                     } else {
-                        $sentry.captureException(e);
-                        return error({
+                        // $sentry.captureException(e);
+                        return createError({
                             statusCode: res.status,
-                            message: "Invalid redirect",
+                            message: res.statusText,
                         });
                     }
                 } else {
-                    $sentry.captureException(e);
-                    return error({
-                        statusCode: res.status,
-                        message: res.statusText,
+                    // $sentry.captureException(e);
+                    // eslint-disable-next-line
+                    console.error(e);
+                    return createError({
+                        statusCode: 500,
+                        message: "Unknown error",
                     });
                 }
-            } else {
-                $sentry.captureException(e);
-                // eslint-disable-next-line
-                console.error(e);
-                return error({
-                    statusCode: 500,
-                    message: "Unknown error",
-                });
             }
         }
+
+        const route = $router.currentRoute.value;
+        return await getAsyncData(
+            $axios,
+            process.browser ? undefined : $config.apiUrl,
+            route.path,
+            route.query
+        );
     },
 
     data() {
         return {
             /**
              * HTML code of the page
              */
@@ -109,34 +129,37 @@
         };
     },
 
     /**
      * Propagates the head data from the template into Nuxt's head system
      */
     head() {
-        return this.headData;
+        return this.headData ?? {};
     },
 
     computed: {
         /**
          * Exposes the defs
          */
         defs() {
             return DEFS;
         },
+
+        /**
+         * Whether the page is a draft
+         */
+        isPreview() {
+            return this.$route.path.replace(/^\/$/, "").endsWith("/preview");
+        },
     },
 
     methods: {
         /**
          * This serves to receive updates about the head data extracted by
          * ServerTemplatedComponent
          */
         receiveHeadData(head) {
             this.headData = head;
-
-            if (head.lang) {
-                this.$vlang.setLocale(head.lang);
-            }
         },
     },
-};
+});
 </script>
```

### Comparing `modelw_project_maker-2023.3.0/src/model_w/project_maker/template.py` & `modelw_project_maker-2023.4.0b1/src/model_w/project_maker/template.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2023.3.0/PKG-INFO` & `modelw_project_maker-2023.4.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-project-maker
-Version: 2023.3.0
+Version: 2023.4.0b1
 Summary: A tool to create Model-W-compliant projects
 Home-page: https://github.com/ModelW/project-maker
 License: WTFPL
 Keywords: model-w,django,nuxt,boilerplate,template
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<4.0
@@ -22,14 +22,15 @@
 Requires-Dist: Unidecode (>=1.3.4,<2.0.0)
 Requires-Dist: black (>=22.8.0,<23.0.0)
 Requires-Dist: isort (>=5.10.1,<6.0.0)
 Requires-Dist: monoformat (>=0.1.0b3,<0.2.0)
 Requires-Dist: node-edge (>=0.1.0b2,<0.2.0)
 Requires-Dist: pathspec (>=0.10.2,<0.11.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: setuptools
 Requires-Dist: tomlkit (>=0.11.4,<0.12.0)
 Project-URL: Documentation, https://github.com/ModelW/project-maker
 Project-URL: Repository, https://github.com/ModelW/project-maker
 Description-Content-Type: text/markdown
 
 # Model&nbsp;W Project Maker
```

