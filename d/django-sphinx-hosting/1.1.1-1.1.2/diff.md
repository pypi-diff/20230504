# Comparing `tmp/django-sphinx-hosting-1.1.1.tar.gz` & `tmp/django-sphinx-hosting-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sphinx-hosting-1.1.1.tar", last modified: Wed May  3 17:41:44 2023, max compression
+gzip compressed data, was "django-sphinx-hosting-1.1.2.tar", last modified: Wed May  3 23:47:13 2023, max compression
```

## Comparing `django-sphinx-hosting-1.1.1.tar` & `django-sphinx-hosting-1.1.2.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.764959 django-sphinx-hosting-1.1.1/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.1.1/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.1.1/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-03 17:41:44.765136 django-sphinx-hosting-1.1.1/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.1.1/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.713972 django-sphinx-hosting-1.1.1/django_sphinx_hosting.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-03 17:41:44.000000 django-sphinx-hosting-1.1.1/django_sphinx_hosting.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     2653 2023-05-03 17:41:44.000000 django-sphinx-hosting-1.1.1/django_sphinx_hosting.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-05-03 17:41:44.000000 django-sphinx-hosting-1.1.1/django_sphinx_hosting.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-05-03 17:41:44.000000 django-sphinx-hosting-1.1.1/django_sphinx_hosting.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-05-03 17:41:44.000000 django-sphinx-hosting-1.1.1/django_sphinx_hosting.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1256 2023-05-03 17:41:44.766156 django-sphinx-hosting-1.1.1/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-05-03 17:41:24.000000 django-sphinx-hosting-1.1.1/setup.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.728165 django-sphinx-hosting-1.1.1/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-05-03 17:41:24.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.732405 django-sphinx-hosting-1.1.1/sphinx_hosting/api/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/api/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/api/apps.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4896 2023-03-28 15:50:00.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/api/serializers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1274 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/api/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8676 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/api/views.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/exc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/fields.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.733179 django-sphinx-hosting-1.1.1/sphinx_hosting/fixtures/
--rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/fixtures/classifiers.json
--rw-r--r--   0 cmalek     (501) admin       (80)      312 2023-05-03 16:48:22.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/form_fields.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6844 2023-05-03 16:47:46.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    21282 2023-05-03 17:28:20.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/importers.py
--rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/logging.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.733916 django-sphinx-hosting-1.1.1/sphinx_hosting/management/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/management/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.737274 django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2568 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/import_docs.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1626 2023-02-01 17:53:25.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/parse_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/print_classifier_tree.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2288 2023-02-01 17:06:33.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/print_doctree.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.748004 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/
--rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0001_initial.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0002_original_html.py
--rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0003_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0004_next_page_FK.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0005_orig_global_toc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0007_load_classifiers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0008_Version_archived.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0010_add_groups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0011_machinenamefield.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    31834 2023-05-03 16:51:48.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/models.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/py.typed
--rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/search_indexes.py
--rw-r--r--   0 cmalek     (501) admin       (80)      566 2023-03-24 21:26:47.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/signals.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.706636 django-sphinx-hosting-1.1.1/sphinx_hosting/static/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.707116 django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.753207 django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
--rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
--rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.754147 django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/images/
--rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.708149 django-sphinx-hosting-1.1.1/sphinx_hosting/templates/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.707789 django-sphinx-hosting-1.1.1/sphinx_hosting/templates/search/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.707952 django-sphinx-hosting-1.1.1/sphinx_hosting/templates/search/indexes/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.755659 django-sphinx-hosting-1.1.1/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
--rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.756501 django-sphinx-hosting-1.1.1/sphinx_hosting/templates/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/templates/sphinx_hosting/base.html
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/types.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1656 2023-05-03 17:07:06.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/urls.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-05-03 16:45:18.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/validators.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    20844 2023-04-28 17:09:25.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/views.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.762815 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/
--rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     6553 2023-04-27 20:10:51.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/classifier.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 17:41:44.764611 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/core/
--rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/core/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/core/basic.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4456 2023-05-02 23:23:03.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/navigation.py
--rw-r--r--   0 cmalek     (501) admin       (80)    14340 2023-05-03 16:34:33.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/project.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/search.py
--rw-r--r--   0 cmalek     (501) admin       (80)     7084 2023-04-27 20:42:19.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/sphinx_page.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/version.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.741470 django-sphinx-hosting-1.1.2/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.1.2/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.1.2/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-03 23:47:13.741603 django-sphinx-hosting-1.1.2/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.1.2/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.696610 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2739 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1256 2023-05-03 23:47:13.742649 django-sphinx-hosting-1.1.2/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-05-03 23:47:08.000000 django-sphinx-hosting-1.1.2/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.708709 django-sphinx-hosting-1.1.2/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-05-03 23:47:08.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.711676 django-sphinx-hosting-1.1.2/sphinx_hosting/api/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/apps.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4896 2023-03-28 15:50:00.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/serializers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1274 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8676 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/views.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/exc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/fields.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.712322 django-sphinx-hosting-1.1.2/sphinx_hosting/fixtures/
+-rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/fixtures/classifiers.json
+-rw-r--r--   0 cmalek     (501) admin       (80)      312 2023-05-03 16:48:22.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/form_fields.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     6919 2023-05-03 23:30:39.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    21728 2023-05-03 20:47:48.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/importers.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/logging.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.712963 django-sphinx-hosting-1.1.2/sphinx_hosting/management/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.717408 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2568 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/import_docs.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1626 2023-02-01 17:53:25.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/parse_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/print_classifier_tree.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2288 2023-02-01 17:06:33.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/print_doctree.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.726711 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/
+-rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0001_initial.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0002_original_html.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0003_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0004_next_page_FK.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0005_orig_global_toc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0007_load_classifiers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0008_Version_archived.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0010_add_groups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0011_machinenamefield.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    31885 2023-05-03 21:49:33.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/models.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/py.typed
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/search_indexes.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      566 2023-03-24 21:26:47.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/signals.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.691164 django-sphinx-hosting-1.1.2/sphinx_hosting/static/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.691537 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.731057 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
+-rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.731854 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/images/
+-rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.692301 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.691996 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/search/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.692116 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/search/indexes/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.732854 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.733492 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/sphinx_hosting/base.html
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.734555 django-sphinx-hosting-1.1.2/sphinx_hosting/templatetags/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/templatetags/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/templatetags/sphinx_hosting.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/types.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1656 2023-05-03 17:07:06.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/urls.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-05-03 16:45:18.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/validators.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    20844 2023-04-28 17:09:25.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/views.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.739659 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/classifier.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.741220 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/core/
+-rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/core/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/core/basic.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4709 2023-05-03 23:21:13.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/navigation.py
+-rw-r--r--   0 cmalek     (501) admin       (80)    14340 2023-05-03 16:34:33.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/project.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/search.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     7375 2023-05-03 22:49:20.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/sphinx_page.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/version.py
```

### Comparing `django-sphinx-hosting-1.1.1/LICENSE.txt` & `django-sphinx-hosting-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/PKG-INFO` & `django-sphinx-hosting-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.1.1
+Version: 1.1.2
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.1.1/README.md` & `django-sphinx-hosting-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/django_sphinx_hosting.egg-info/PKG-INFO` & `django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.1.1
+Version: 1.1.2
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.1.1/django_sphinx_hosting.egg-info/SOURCES.txt` & `django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
 sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
 sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
 sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
 sphinx_hosting/static/sphinx_hosting/images/logo.jpg
 sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
 sphinx_hosting/templates/sphinx_hosting/base.html
+sphinx_hosting/templatetags/__init__.py
+sphinx_hosting/templatetags/sphinx_hosting.py
 sphinx_hosting/wildewidgets/__init__.py
 sphinx_hosting/wildewidgets/classifier.py
 sphinx_hosting/wildewidgets/navigation.py
 sphinx_hosting/wildewidgets/project.py
 sphinx_hosting/wildewidgets/search.py
 sphinx_hosting/wildewidgets/sphinx_page.py
 sphinx_hosting/wildewidgets/version.py
```

### Comparing `django-sphinx-hosting-1.1.1/setup.cfg` & `django-sphinx-hosting-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/setup.py` & `django-sphinx-hosting-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="django-sphinx-hosting",
-    version="1.1.1",
+    version="1.1.2",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "django-braces >= 1.15.0",
         "django-crispy-forms>=1.14.0",
         "django-extensions >= 3.2.1",
         "django-filter >= 22.1",
```

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/api/serializers.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/api/urls.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/api/views.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/fields.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/fields.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/fixtures/classifiers.json` & `django-sphinx-hosting-1.1.2/sphinx_hosting/fixtures/classifiers.json`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/forms.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import Type
 
 from crispy_forms.helper import FormHelper
-from crispy_forms.layout import Submit, Layout, Field, Fieldset, ButtonHolder
+from crispy_forms.layout import Submit, Layout, Field, Fieldset, HTML, ButtonHolder
 
 from crispy_forms.bootstrap import FieldWithButtons
 from django import forms
 from django.db.models import Model
 from django.urls import reverse, reverse_lazy
 from haystack.forms import SearchForm
 
 from .models import Project
 
 
-
 class GlobalSearchForm(SearchForm):
     """
     This is the search form at the top of the sidebar, underneath the logo.  It is
     a subclass of :py:class:`haystack.forms.SearchForm`, and does a search of our
     haystack backend.
     """
 
@@ -28,15 +27,15 @@
         self.helper.form_show_labels = False
         # This is a reverse_lazy on purpose because the form gets instantiated as
         # the urlpatterns are being made
         self.helper.form_action = reverse_lazy('sphinx_hosting:search')
         self.helper.layout = Layout(
             FieldWithButtons(
                 Field('q', css_class='text-dark', placeholder='Search'),
-                Submit('submit', 'Search'),
+                HTML('<button type="submit" class="btn btn-primary"><span class="bi bi-search"></span></button>')
             )
         )
 
 
 class ProjectCreateForm(forms.ModelForm):
     """
     This is the form we use to create a new
```

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/importers.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/importers.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,18 +123,25 @@
         if filename not in self.name_map:
             raise KeyError(f'Sphinx docs TarFile has no file named "{filename}"')
         return cast(io.BufferedReader, package.extractfile(self.name_map[filename]))
 
     def _update_image_src(self, body: str) -> str:
         """
         Given an HTML body of a Sphinx page, update the ``<img src="path">``
-        references to point to the URLs for our uploaded
-        :py:class:`sphinx_hosting.models.SphinxImage` objects.  Also deal with
-        any lightboxes by converting them to the appropriate form to work with
-        Tabler lightboxes.
+        references to template tag expressions that load the actual image URL
+        from the :py:class:`sphinx_hosting.models.SphinxImage` objects at render time.
+
+        We need to defer filling in the URL of the image until render time
+        because of things like storing images in S3 and using time-limited S3
+        auth parameters to retrieve the image from a private bucket.  Those
+        parameters expire typically after an hour, so if we don't defer figuring
+        out the URL for our images, we end up storing a stale URL.
+
+        Also deal with any lightboxes by converting them to the appropriate form
+        to work with Tabler lightboxes.
 
         Args:
             body: the HTML body of a Sphinx document
 
         Returns:
             ``body`` with its ``<img>`` urls and lightbox attributes updated
         """
@@ -153,15 +160,15 @@
             lightbox.attrib['data-fslightbox'] = lightbox.attrib['data-lightbox']
             del lightbox.attrib['data-lightbox']
             if 'data-title' in lightbox.attrib:
                 lightbox.attrib['data-caption'] = lightbox.attrib['data-title']
                 del lightbox.attrib['data-title']
             src = re.sub(r'\.\./', '', lightbox.attrib['href'])
             if src in self.image_map:
-                lightbox.attrib['href'] = self.image_map[src].file.url
+                lightbox.attrib['href'] = f'{{% sphinximage_url {self.image_map[src].id} %}}'
         return lxml.html.tostring(html).decode('utf-8')
 
     def load_config(self, package: tarfile.TarFile) -> None:
         """
         Load the ``globalcontext.json`` file for later reference.
 
         Args:
```

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/import_docs.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/import_docs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/parse_globaltoc.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/parse_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/print_classifier_tree.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/print_classifier_tree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/management/commands/print_doctree.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/print_doctree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0001_initial.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0002_original_html.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0002_original_html.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0003_globaltoc.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0003_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0004_next_page_FK.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0004_next_page_FK.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0005_orig_global_toc.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0005_orig_global_toc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0007_load_classifiers.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0007_load_classifiers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0009_SphinxPage_searchable.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0009_SphinxPage_searchable.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0010_add_groups.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0010_add_groups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/migrations/0011_machinenamefield.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0011_machinenamefield.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/models.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,15 +837,15 @@
         ),
     )
     body: F = models.TextField(
         'Body',
         blank=True,
         help_text=_(
             'The body for the page, extracted from the page JSON, and modified to suit us.  '
-            'Some pages have no body.'
+            'Some pages have no body.  The body is actually stored as a Django template.'
         ),
     )
     orig_local_toc: F = models.TextField(
         'Local Table of Contents (original)',
         blank=True,
         null=True,
         default=None,
```

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/search_indexes.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/settings.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/settings.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/signals.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/signals.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss` & `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss` & `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss` & `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css` & `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss` & `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/static/sphinx_hosting/images/logo.jpg` & `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/templates/sphinx_hosting/base.html` & `django-sphinx-hosting-1.1.2/sphinx_hosting/templates/sphinx_hosting/base.html`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/urls.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/validators.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/validators.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/views.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/classifier.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,17 +109,19 @@
         self.add_block(
             HorizontalLayoutBlock(
                 LinkButton(name='classifier--submit', text='Filter Projects', color='primary'),
                 LinkButton(
                     name='classifier--clear',
                     text='Clear',
                     color='outline-secondary',
+                    css_class="mt-2 mt-xl-0"
                 ),
                 css_class='my-3',
-                justify='between'
+                justify='between',
+                flex_size='xl'
             )
         )
 
     def add_subtree(self, contents: UnorderedList, nodes: Dict[str, ClassifierNode]) -> None:
         """
         Add a subtree of classifier checkboxes.
```

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/navigation.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/navigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List, Optional, cast
 
 from crequest.middleware import CrequestMiddleware
 from django.contrib.auth.models import AbstractUser
 from django.http.request import HttpRequest
 from django.urls import reverse_lazy
 from wildewidgets import (
+    Block,
     BreadcrumbBlock,
     BreadcrumbItem,
     LinkedImage,
     Menu,
     MenuItem,
     TablerVerticalNavbar
 )
@@ -108,23 +109,27 @@
     :py:class:`sphinx_hosting.wildewidgets.search.GlobalSearchFormWidget`, our
     main menu :py:class:`SphinxHostingMainMenu`, possibly our utility menu
     :py:class:`SphinxHostingLookupsMenu` and finally the global navigation
     for a :py:class:`sphinx_hosting.models.Version` when we're reading our
     documentation.
     """
 
-    branding = LinkedImage(
-        image_src=LOGO_IMAGE,
-        image_width=LOGO_WIDTH,
-        image_alt=SITE_NAME,
-        css_class='d-flex justify-content-center',
-        url=LOGO_URL
+    hide_below_viewport: str = 'xl'
+    branding = Block(
+        LinkedImage(
+            image_src=LOGO_IMAGE,
+            image_width=LOGO_WIDTH,
+            image_alt=SITE_NAME,
+            css_class='d-flex justify-content-center',
+            url=LOGO_URL
+        ),
+        GlobalSearchFormWidget(css_class='ms-auto ms-xl-0 align-self-center mt-3 mt-xl-0'),
+        css_class='d-flex flex-row flex-xl-column justify-content-between flex-grow-1 flex-xl-grow-0'
     )
     contents = [
-        GlobalSearchFormWidget(),
         SphinxHostingMainMenu(),
         SphinxHostingLookupsMenu(),
     ]
     wide: bool = True
 
 
 class SphinxHostingBreadcrumbs(BreadcrumbBlock):
```

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/project.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/project.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/search.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/search.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/sphinx_page.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/sphinx_page.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Dict, List
 
+from django.template import Context, Template
 from wildewidgets import (
     Block,
     CardHeader,
     CardWidget,
     Column,
     FontIcon,
     HTMLWidget,
@@ -64,25 +65,28 @@
                     css_class='bg-azure-lt'
                 )
             )
 
 
 class SphinxPageBodyWidget(CardWidget):
     """
-    This widget holds the body of the page.
+    This widget holds the body of the page.  The body as stored in the model is
+    actually a Django template, so we retrieve the body, run it through the
+    Django template engine, and display the results.
 
     Args:
         page: the ``SphinxPage`` we are rendering
     """
 
     css_class: str = 'sphinxpage-body'
 
     def __init__(self, page: SphinxPage, **kwargs):
         super().__init__(**kwargs)
-        self.widget = HTMLWidget(html=page.body)
+        body = '{% load sphinx_hosting %}\n' + page.body
+        self.widget = HTMLWidget(html=Template(body).render(Context()))
 
 
 class SphinxPageTableOfContentsWidget(CardWidget):
     """
     This widget draws the in-page navigation -- the header hierarchy.
 
     Args:
```

### Comparing `django-sphinx-hosting-1.1.1/sphinx_hosting/wildewidgets/version.py` & `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/version.py`

 * *Files identical despite different names*

