# Comparing `tmp/wagtail_cblocks-0.4.0.tar.gz` & `tmp/wagtail_cblocks-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_cblocks-0.4.0.tar", last modified: Sun Apr  2 17:20:27 2023, max compression
+gzip compressed data, was "wagtail_cblocks-0.4.1.tar", last modified: Thu May  4 14:02:30 2023, max compression
```

## Comparing `wagtail_cblocks-0.4.0.tar` & `wagtail_cblocks-0.4.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.571221 wagtail_cblocks-0.4.0/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      319 2021-03-04 09:52:17.000000 wagtail_cblocks-0.4.0/.editorconfig
--rw-r--r--   0 jerome    (1000) jerome    (1000)      263 2022-03-09 15:21:21.000000 wagtail_cblocks-0.4.0/.gitignore
--rw-r--r--   0 jerome    (1000) jerome    (1000)      730 2022-10-27 10:58:22.000000 wagtail_cblocks-0.4.0/.gitlab-ci.yml
--rw-r--r--   0 jerome    (1000) jerome    (1000)      607 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2201 2023-04-02 17:17:50.000000 wagtail_cblocks-0.4.0/CHANGELOG.md
--rw-r--r--   0 jerome    (1000) jerome    (1000)    35149 2021-03-04 09:51:01.000000 wagtail_cblocks-0.4.0/LICENSE
--rw-r--r--   0 jerome    (1000) jerome    (1000)      108 2021-03-04 09:56:09.000000 wagtail_cblocks-0.4.0/MANIFEST.in
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1103 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/Makefile
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4832 2023-04-02 17:20:27.571221 wagtail_cblocks-0.4.0/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3788 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/README.md
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1740 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/noxfile.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      793 2022-03-09 14:08:45.000000 wagtail_cblocks-0.4.0/pyproject.toml
--rw-r--r--   0 jerome    (1000) jerome    (1000)       53 2022-03-09 14:08:45.000000 wagtail_cblocks-0.4.0/requirements-dev.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)       32 2022-03-09 14:08:45.000000 wagtail_cblocks-0.4.0/requirements-test.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1170 2023-04-02 17:20:27.571221 wagtail_cblocks-0.4.0/setup.cfg
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.567221 wagtail_cblocks-0.4.0/tests/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-04 15:56:35.000000 wagtail_cblocks-0.4.0/tests/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      160 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/tests/conftest.py
--rwxr-xr-x   0 jerome    (1000) jerome    (1000)      378 2022-03-31 09:47:32.000000 wagtail_cblocks-0.4.0/tests/manage.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.567221 wagtail_cblocks-0.4.0/tests/migrations/
--rw-r--r--   0 jerome    (1000) jerome    (1000)    96025 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/tests/migrations/0001_initial.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-04 16:37:56.000000 wagtail_cblocks-0.4.0/tests/migrations/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1977 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/tests/models.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2417 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/tests/settings.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.563221 wagtail_cblocks-0.4.0/tests/templates/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.567221 wagtail_cblocks-0.4.0/tests/templates/tests/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.567221 wagtail_cblocks-0.4.0/tests/templates/tests/blocks/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      195 2021-08-17 12:43:58.000000 wagtail_cblocks-0.4.0/tests/templates/tests/blocks/hero_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      406 2021-08-16 16:09:20.000000 wagtail_cblocks-0.4.0/tests/templates/tests/blocks/row_columns_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      849 2021-08-16 16:09:20.000000 wagtail_cblocks-0.4.0/tests/templates/tests/standard_page.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1971 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/tests/test_admin.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)    10682 2022-03-09 13:45:36.000000 wagtail_cblocks-0.4.0/tests/test_blocks.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      445 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/tests/test_factories.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      524 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/tests/urls.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.567221 wagtail_cblocks-0.4.0/wagtail_cblocks/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-02 16:06:36.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     8851 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/blocks.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      681 2021-03-08 21:24:51.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/factories.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.563221 wagtail_cblocks-0.4.0/wagtail_cblocks/locale/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.563221 wagtail_cblocks-0.4.0/wagtail_cblocks/locale/fr/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.567221 wagtail_cblocks-0.4.0/wagtail_cblocks/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1253 2022-03-24 10:55:23.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1646 2022-03-31 09:50:25.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.563221 wagtail_cblocks-0.4.0/wagtail_cblocks/static/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.563221 wagtail_cblocks-0.4.0/wagtail_cblocks/static/wagtail_cblocks/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.567221 wagtail_cblocks-0.4.0/wagtail_cblocks/static/wagtail_cblocks/css/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      149 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/static/wagtail_cblocks/css/editor.css
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.563221 wagtail_cblocks-0.4.0/wagtail_cblocks/templates/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.571221 wagtail_cblocks-0.4.0/wagtail_cblocks/templates/wagtail_cblocks/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.571221 wagtail_cblocks-0.4.0/wagtail_cblocks/templates/wagtail_cblocks/block_forms/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      750 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/templates/wagtail_cblocks/block_forms/link_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      115 2021-08-16 16:09:20.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/templates/wagtail_cblocks/button_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      336 2021-03-10 15:54:52.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/templates/wagtail_cblocks/columns_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)       77 2021-03-03 09:07:28.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/templates/wagtail_cblocks/heading_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      402 2021-03-10 09:29:05.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/templates/wagtail_cblocks/image_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)       12 2021-03-03 09:07:35.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/templates/wagtail_cblocks/paragraph_block.html
--rw-r--r--   0 jerome    (1000) jerome    (1000)      297 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.0/wagtail_cblocks/wagtail_hooks.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-04-02 17:20:27.567221 wagtail_cblocks-0.4.0/wagtail_cblocks.egg-info/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4832 2023-04-02 17:20:27.000000 wagtail_cblocks-0.4.0/wagtail_cblocks.egg-info/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1393 2023-04-02 17:20:27.000000 wagtail_cblocks-0.4.0/wagtail_cblocks.egg-info/SOURCES.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)        1 2023-04-02 17:20:27.000000 wagtail_cblocks-0.4.0/wagtail_cblocks.egg-info/dependency_links.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)       55 2023-04-02 17:20:27.000000 wagtail_cblocks-0.4.0/wagtail_cblocks.egg-info/requires.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)       16 2023-04-02 17:20:27.000000 wagtail_cblocks-0.4.0/wagtail_cblocks.egg-info/top_level.txt
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      319 2021-03-04 09:52:17.000000 wagtail_cblocks-0.4.1/.editorconfig
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      263 2022-03-09 15:21:21.000000 wagtail_cblocks-0.4.1/.gitignore
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      784 2023-05-04 13:28:04.000000 wagtail_cblocks-0.4.1/.gitlab-ci.yml
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      607 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2328 2023-05-04 14:01:36.000000 wagtail_cblocks-0.4.1/CHANGELOG.md
+-rw-r--r--   0 jerome    (1000) jerome    (1000)    35149 2021-03-04 09:51:01.000000 wagtail_cblocks-0.4.1/LICENSE
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      108 2021-03-04 09:56:09.000000 wagtail_cblocks-0.4.1/MANIFEST.in
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1103 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/Makefile
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     4864 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/PKG-INFO
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     3807 2023-05-04 13:29:40.000000 wagtail_cblocks-0.4.1/README.md
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2076 2023-05-04 13:26:21.000000 wagtail_cblocks-0.4.1/noxfile.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      793 2022-03-09 14:08:45.000000 wagtail_cblocks-0.4.1/pyproject.toml
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       53 2022-03-09 14:08:45.000000 wagtail_cblocks-0.4.1/requirements-dev.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       32 2022-03-09 14:08:45.000000 wagtail_cblocks-0.4.1/requirements-test.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1180 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/setup.cfg
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.245506 wagtail_cblocks-0.4.1/tests/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-04 15:56:35.000000 wagtail_cblocks-0.4.1/tests/__init__.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      160 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/conftest.py
+-rwxr-xr-x   0 jerome    (1000) jerome    (1000)      378 2022-03-31 09:47:32.000000 wagtail_cblocks-0.4.1/tests/manage.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.245506 wagtail_cblocks-0.4.1/tests/migrations/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)    96025 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/migrations/0001_initial.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-04 16:37:56.000000 wagtail_cblocks-0.4.1/tests/migrations/__init__.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1977 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/models.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     2417 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/settings.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/tests/templates/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/tests/templates/tests/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/tests/templates/tests/blocks/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      195 2021-08-17 12:43:58.000000 wagtail_cblocks-0.4.1/tests/templates/tests/blocks/hero_block.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      406 2021-08-16 16:09:20.000000 wagtail_cblocks-0.4.1/tests/templates/tests/blocks/row_columns_block.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      849 2021-08-16 16:09:20.000000 wagtail_cblocks-0.4.1/tests/templates/tests/standard_page.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1971 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/test_admin.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)    10682 2022-03-09 13:45:36.000000 wagtail_cblocks-0.4.1/tests/test_blocks.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      445 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/test_factories.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      524 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/tests/urls.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/wagtail_cblocks/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-02 16:06:36.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/__init__.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     8851 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/blocks.py
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      681 2021-03-08 21:24:51.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/factories.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1253 2022-03-24 10:55:23.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1646 2022-03-31 09:50:25.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/static/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/static/wagtail_cblocks/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/wagtail_cblocks/static/wagtail_cblocks/css/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      149 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/static/wagtail_cblocks/css/editor.css
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.237506 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.253506 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/block_forms/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      750 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/block_forms/link_block.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      115 2021-08-16 16:09:20.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/button_block.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      336 2021-03-10 15:54:52.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/columns_block.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       77 2021-03-03 09:07:28.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/heading_block.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      402 2021-03-10 09:29:05.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/image_block.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       12 2021-03-03 09:07:35.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/paragraph_block.html
+-rw-r--r--   0 jerome    (1000) jerome    (1000)      297 2023-04-02 17:16:33.000000 wagtail_cblocks-0.4.1/wagtail_cblocks/wagtail_hooks.py
+drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2023-05-04 14:02:30.249506 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     4864 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/PKG-INFO
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     1393 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)        1 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       52 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/requires.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)       16 2023-05-04 14:02:30.000000 wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/top_level.txt
```

### Comparing `wagtail_cblocks-0.4.0/.gitlab-ci.yml` & `wagtail_cblocks-0.4.1/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,19 @@
   coverage: '/TOTAL *(?:\d+) *(?:\d+) *(?:\d+) *(?:\d+) *(\d+%)/'
 
 test-py310:
   image: python:3.10
   script:
     - nox
 
+test-py311:
+  image: python:3.11
+  script:
+    - nox
+
 lint:
   image: python:3.9
   variables:
     PRE_COMMIT_HOME: ${CI_PROJECT_DIR}/.cache/pre-commit
   cache:
     paths:
       - ${PRE_COMMIT_HOME}
```

### Comparing `wagtail_cblocks-0.4.0/.pre-commit-config.yaml` & `wagtail_cblocks-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/CHANGELOG.md` & `wagtail_cblocks-0.4.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 0.4.1 - 2023-05-04
+
+This release only removes the Wagtail's maximum supported version to prevent
+conflicting dependencies.
+
 ## 0.4.0 - 2023-04-02
 ### Changed
 - Drop support for Wagtail < 4.1 LTS
 
 ### Fixed
 - Update CSS tweaks in the admin for `LinkBlock` and remove `ColumnsBlock` ones
 - Remove the help icon from the admin form of `LinkBlock` to fit default rendering
```

### Comparing `wagtail_cblocks-0.4.0/LICENSE` & `wagtail_cblocks-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/Makefile` & `wagtail_cblocks-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/PKG-INFO` & `wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_cblocks
-Version: 0.4.0
+Name: wagtail-cblocks
+Version: 0.4.1
 Summary: Collection of StreamField blocks for Wagtail
 Author: Cliss XXI
 Author-email: contact@cliss21.com
 License: AGPLv3+
 Project-URL: Bug Tracker, https://framagit.org/cliss21/wagtail-cblocks/-/issues
 Project-URL: Source Code, https://framagit.org/cliss21/wagtail-cblocks
 Keywords: wagtail,blocks,streamfield
@@ -13,17 +13,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: factories
 License-File: LICENSE
 
 # wagtail-cblocks
 
@@ -32,17 +32,17 @@
 **Warning!** This project is still early on in its development lifecycle. It is
 possible for breaking changes to occur between versions until reaching a stable
 1.0. Feedback and pull requests are welcome.
 
 ## Requirements
 
 wagtail-cblocks requires the following:
-- **Wagtail** (4.1 LTS, 4.2)
-- **Django** (3.2, 4.0, 4.1)
-- **Python 3** (3.7, 3.8, 3.9, 3.10)
+- **Wagtail** (4.1 LTS, 4.2, 5.0)
+- **Django** (3.2 LTS, 4.1, 4.2 LTS)
+- **Python 3** (3.7, 3.8, 3.9, 3.10, 3.11)
 
 ## Installation
 
 1. Install using ``pip``:
    ```shell
    $ pip install wagtail-cblocks
    ```
```

### Comparing `wagtail_cblocks-0.4.0/README.md` & `wagtail_cblocks-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 **Warning!** This project is still early on in its development lifecycle. It is
 possible for breaking changes to occur between versions until reaching a stable
 1.0. Feedback and pull requests are welcome.
 
 ## Requirements
 
 wagtail-cblocks requires the following:
-- **Wagtail** (4.1 LTS, 4.2)
-- **Django** (3.2, 4.0, 4.1)
-- **Python 3** (3.7, 3.8, 3.9, 3.10)
+- **Wagtail** (4.1 LTS, 4.2, 5.0)
+- **Django** (3.2 LTS, 4.1, 4.2 LTS)
+- **Python 3** (3.7, 3.8, 3.9, 3.10, 3.11)
 
 ## Installation
 
 1. Install using ``pip``:
    ```shell
    $ pip install wagtail-cblocks
    ```
```

### Comparing `wagtail_cblocks-0.4.0/noxfile.py` & `wagtail_cblocks-0.4.1/noxfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
 
 import nox
 
 nox.options.sessions = [
     'tests_wagtail41',
     'tests_wagtail42',
+    'tests_wagtail50',
 ]
 
 dj32 = nox.param('3.2', id='dj32')
-dj40 = nox.param('4.0', id='dj40')
 dj41 = nox.param('4.1', id='dj41')
+dj42 = nox.param('4.2', id='dj42')
 
 
 def install_and_run_tests(session):
     session.install('-r', 'requirements-test.txt')
     session.install('-e', '.[factories]')
     tests = session.posargs or ['tests/']
     session.run(
@@ -24,34 +25,44 @@
         *tests,
         env={'COVERAGE_FILE': f'.coverage.{session.name}'},
     )
     session.notify('coverage')
 
 
 @nox.session
-@nox.parametrize('django', [dj32, dj40, dj41])
+@nox.parametrize('django', [dj32, dj41])
 def tests_wagtail41(session, django):
     if django != '3.2' and sys.version_info.minor < 8:
         session.skip("Django >=4.0 requires Python 3.8+")
     session.install(f'django=={django}')
     session.install('wagtail==4.1')
     install_and_run_tests(session)
 
 
 @nox.session
-@nox.parametrize('django', [dj32, dj40, dj41])
+@nox.parametrize('django', [dj32, dj41])
 def tests_wagtail42(session, django):
     if django != '3.2' and sys.version_info.minor < 8:
         session.skip("Django >=4.0 requires Python 3.8+")
     session.install(f'django=={django}')
     session.install('wagtail==4.2')
     install_and_run_tests(session)
 
 
 @nox.session
+@nox.parametrize('django', [dj32, dj41, dj42])
+def tests_wagtail50(session, django):
+    if django != '3.2' and sys.version_info.minor < 8:
+        session.skip("Django >=4.0 requires Python 3.8+")
+    session.install(f'django=={django}')
+    session.install('wagtail==5.0')
+    install_and_run_tests(session)
+
+
+@nox.session
 def coverage(session):
     session.install('coverage[toml]')
     session.run('coverage', 'combine')
     session.run('coverage', 'report', '--show-missing')
     session.run('coverage', 'xml')
     session.run('coverage', 'erase')
```

### Comparing `wagtail_cblocks-0.4.0/pyproject.toml` & `wagtail_cblocks-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/setup.cfg` & `wagtail_cblocks-0.4.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Affero General Public License v3
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Framework :: Django
 	Framework :: Wagtail
-	Framework :: Wagtail :: 2
 keywords = 
 	wagtail
 	blocks
 	streamfield
 
 [options]
 packages = wagtail_cblocks
 install_requires = 
-	wagtail >=2.15,<5
+	wagtail >=2.15
 python_requires = >=3.7,<4
 include_package_data = True
 
 [options.extras_require]
 factories = 
 	wagtail-factories >=4.0.0
```

### Comparing `wagtail_cblocks-0.4.0/tests/migrations/0001_initial.py` & `wagtail_cblocks-0.4.1/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/tests/models.py` & `wagtail_cblocks-0.4.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/tests/settings.py` & `wagtail_cblocks-0.4.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/tests/templates/tests/standard_page.html` & `wagtail_cblocks-0.4.1/tests/templates/tests/standard_page.html`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/tests/test_admin.py` & `wagtail_cblocks-0.4.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/tests/test_blocks.py` & `wagtail_cblocks-0.4.1/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/tests/urls.py` & `wagtail_cblocks-0.4.1/tests/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/wagtail_cblocks/blocks.py` & `wagtail_cblocks-0.4.1/wagtail_cblocks/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/wagtail_cblocks/factories.py` & `wagtail_cblocks-0.4.1/wagtail_cblocks/factories.py`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/wagtail_cblocks/locale/fr/LC_MESSAGES/django.mo` & `wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/wagtail_cblocks/locale/fr/LC_MESSAGES/django.po` & `wagtail_cblocks-0.4.1/wagtail_cblocks/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/wagtail_cblocks/templates/wagtail_cblocks/block_forms/link_block.html` & `wagtail_cblocks-0.4.1/wagtail_cblocks/templates/wagtail_cblocks/block_forms/link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_cblocks-0.4.0/wagtail_cblocks.egg-info/PKG-INFO` & `wagtail_cblocks-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail-cblocks
-Version: 0.4.0
+Name: wagtail_cblocks
+Version: 0.4.1
 Summary: Collection of StreamField blocks for Wagtail
 Author: Cliss XXI
 Author-email: contact@cliss21.com
 License: AGPLv3+
 Project-URL: Bug Tracker, https://framagit.org/cliss21/wagtail-cblocks/-/issues
 Project-URL: Source Code, https://framagit.org/cliss21/wagtail-cblocks
 Keywords: wagtail,blocks,streamfield
@@ -13,17 +13,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: factories
 License-File: LICENSE
 
 # wagtail-cblocks
 
@@ -32,17 +32,17 @@
 **Warning!** This project is still early on in its development lifecycle. It is
 possible for breaking changes to occur between versions until reaching a stable
 1.0. Feedback and pull requests are welcome.
 
 ## Requirements
 
 wagtail-cblocks requires the following:
-- **Wagtail** (4.1 LTS, 4.2)
-- **Django** (3.2, 4.0, 4.1)
-- **Python 3** (3.7, 3.8, 3.9, 3.10)
+- **Wagtail** (4.1 LTS, 4.2, 5.0)
+- **Django** (3.2 LTS, 4.1, 4.2 LTS)
+- **Python 3** (3.7, 3.8, 3.9, 3.10, 3.11)
 
 ## Installation
 
 1. Install using ``pip``:
    ```shell
    $ pip install wagtail-cblocks
    ```
```

### Comparing `wagtail_cblocks-0.4.0/wagtail_cblocks.egg-info/SOURCES.txt` & `wagtail_cblocks-0.4.1/wagtail_cblocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

