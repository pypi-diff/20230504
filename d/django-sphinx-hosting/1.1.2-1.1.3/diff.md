# Comparing `tmp/django-sphinx-hosting-1.1.2.tar.gz` & `tmp/django-sphinx-hosting-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sphinx-hosting-1.1.2.tar", last modified: Wed May  3 23:47:13 2023, max compression
+gzip compressed data, was "django-sphinx-hosting-1.1.3.tar", last modified: Thu May  4 16:34:24 2023, max compression
```

## Comparing `django-sphinx-hosting-1.1.2.tar` & `django-sphinx-hosting-1.1.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.741470 django-sphinx-hosting-1.1.2/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.1.2/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.1.2/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-03 23:47:13.741603 django-sphinx-hosting-1.1.2/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.1.2/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.696610 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     2739 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-05-03 23:47:13.000000 django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1256 2023-05-03 23:47:13.742649 django-sphinx-hosting-1.1.2/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-05-03 23:47:08.000000 django-sphinx-hosting-1.1.2/setup.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.708709 django-sphinx-hosting-1.1.2/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-05-03 23:47:08.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.711676 django-sphinx-hosting-1.1.2/sphinx_hosting/api/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/apps.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4896 2023-03-28 15:50:00.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/serializers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1274 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8676 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/api/views.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/exc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/fields.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.712322 django-sphinx-hosting-1.1.2/sphinx_hosting/fixtures/
--rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/fixtures/classifiers.json
--rw-r--r--   0 cmalek     (501) admin       (80)      312 2023-05-03 16:48:22.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/form_fields.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6919 2023-05-03 23:30:39.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    21728 2023-05-03 20:47:48.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/importers.py
--rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/logging.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.712963 django-sphinx-hosting-1.1.2/sphinx_hosting/management/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.717408 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2568 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/import_docs.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1626 2023-02-01 17:53:25.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/parse_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/print_classifier_tree.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2288 2023-02-01 17:06:33.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/print_doctree.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.726711 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/
--rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0001_initial.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0002_original_html.py
--rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0003_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0004_next_page_FK.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0005_orig_global_toc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0007_load_classifiers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0008_Version_archived.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0010_add_groups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0011_machinenamefield.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    31885 2023-05-03 21:49:33.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/models.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/py.typed
--rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/search_indexes.py
--rw-r--r--   0 cmalek     (501) admin       (80)      566 2023-03-24 21:26:47.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/signals.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.691164 django-sphinx-hosting-1.1.2/sphinx_hosting/static/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.691537 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.731057 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
--rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
--rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.731854 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/images/
--rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.692301 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.691996 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/search/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.692116 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/search/indexes/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.732854 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
--rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.733492 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/templates/sphinx_hosting/base.html
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.734555 django-sphinx-hosting-1.1.2/sphinx_hosting/templatetags/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/templatetags/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/templatetags/sphinx_hosting.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/types.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1656 2023-05-03 17:07:06.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/urls.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-05-03 16:45:18.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/validators.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    20844 2023-04-28 17:09:25.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/views.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.739659 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/
--rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/classifier.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-03 23:47:13.741220 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/core/
--rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/core/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/core/basic.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4709 2023-05-03 23:21:13.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/navigation.py
--rw-r--r--   0 cmalek     (501) admin       (80)    14340 2023-05-03 16:34:33.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/project.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/search.py
--rw-r--r--   0 cmalek     (501) admin       (80)     7375 2023-05-03 22:49:20.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/sphinx_page.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/version.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.162365 django-sphinx-hosting-1.1.3/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.1.3/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.1.3/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-04 16:34:24.162580 django-sphinx-hosting-1.1.3/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.1.3/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.113960 django-sphinx-hosting-1.1.3/django_sphinx_hosting.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-04 16:34:23.000000 django-sphinx-hosting-1.1.3/django_sphinx_hosting.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2739 2023-05-04 16:34:24.000000 django-sphinx-hosting-1.1.3/django_sphinx_hosting.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-05-04 16:34:23.000000 django-sphinx-hosting-1.1.3/django_sphinx_hosting.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-05-04 16:34:23.000000 django-sphinx-hosting-1.1.3/django_sphinx_hosting.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-05-04 16:34:23.000000 django-sphinx-hosting-1.1.3/django_sphinx_hosting.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1256 2023-05-04 16:34:24.163726 django-sphinx-hosting-1.1.3/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-05-04 16:33:55.000000 django-sphinx-hosting-1.1.3/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.125833 django-sphinx-hosting-1.1.3/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-05-04 16:33:55.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.129333 django-sphinx-hosting-1.1.3/sphinx_hosting/api/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/api/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/api/apps.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4896 2023-03-28 15:50:00.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/api/serializers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1274 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/api/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8676 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/api/views.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/exc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/fields.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.130035 django-sphinx-hosting-1.1.3/sphinx_hosting/fixtures/
+-rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/fixtures/classifiers.json
+-rw-r--r--   0 cmalek     (501) admin       (80)      312 2023-05-03 16:48:22.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/form_fields.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     6919 2023-05-03 23:30:39.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    22276 2023-05-04 16:31:15.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/importers.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/logging.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.130674 django-sphinx-hosting-1.1.3/sphinx_hosting/management/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/management/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.134513 django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2568 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/import_docs.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1626 2023-02-01 17:53:25.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/parse_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/print_classifier_tree.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2288 2023-02-01 17:06:33.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/print_doctree.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.144654 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/
+-rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0001_initial.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0002_original_html.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0003_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0004_next_page_FK.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0005_orig_global_toc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0007_load_classifiers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0008_Version_archived.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0010_add_groups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0011_machinenamefield.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    31885 2023-05-03 21:49:33.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/models.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/py.typed
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/search_indexes.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      566 2023-03-24 21:26:47.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/signals.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.106958 django-sphinx-hosting-1.1.3/sphinx_hosting/static/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.107395 django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.149065 django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
+-rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.149920 django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/images/
+-rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.108324 django-sphinx-hosting-1.1.3/sphinx_hosting/templates/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.107977 django-sphinx-hosting-1.1.3/sphinx_hosting/templates/search/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.108111 django-sphinx-hosting-1.1.3/sphinx_hosting/templates/search/indexes/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.151183 django-sphinx-hosting-1.1.3/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.151951 django-sphinx-hosting-1.1.3/sphinx_hosting/templates/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/templates/sphinx_hosting/base.html
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.153345 django-sphinx-hosting-1.1.3/sphinx_hosting/templatetags/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/templatetags/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/templatetags/sphinx_hosting.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/types.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1656 2023-05-03 17:07:06.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/urls.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-05-03 16:45:18.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/validators.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    20844 2023-04-28 17:09:25.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/views.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.160114 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/classifier.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 16:34:24.162063 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/core/
+-rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/core/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/core/basic.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4709 2023-05-03 23:21:13.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/navigation.py
+-rw-r--r--   0 cmalek     (501) admin       (80)    14340 2023-05-03 16:34:33.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/project.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/search.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     7375 2023-05-03 22:49:20.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/sphinx_page.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/version.py
```

### Comparing `django-sphinx-hosting-1.1.2/LICENSE.txt` & `django-sphinx-hosting-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/PKG-INFO` & `django-sphinx-hosting-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.1.2
+Version: 1.1.3
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.1.2/README.md` & `django-sphinx-hosting-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/PKG-INFO` & `django-sphinx-hosting-1.1.3/django_sphinx_hosting.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.1.2
+Version: 1.1.3
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.1.2/django_sphinx_hosting.egg-info/SOURCES.txt` & `django-sphinx-hosting-1.1.3/django_sphinx_hosting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/setup.cfg` & `django-sphinx-hosting-1.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/setup.py` & `django-sphinx-hosting-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="django-sphinx-hosting",
-    version="1.1.2",
+    version="1.1.3",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "django-braces >= 1.15.0",
         "django-crispy-forms>=1.14.0",
         "django-extensions >= 3.2.1",
         "django-filter >= 22.1",
```

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/api/serializers.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/api/urls.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/api/views.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/fields.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/fields.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/fixtures/classifiers.json` & `django-sphinx-hosting-1.1.3/sphinx_hosting/fixtures/classifiers.json`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/forms.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/forms.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/importers.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/importers.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         if not body:
             return ''
         html = lxml.html.fromstring(body)
         images = html.cssselect('img')
         for image in images:
             src = re.sub(r'\.\./', '', image.attrib['src'])
             if src in self.image_map:
-                image.attrib['src'] = self.image_map[src].file.url
+                image.attrib['src'] = f'{{% sphinximage_url {self.image_map[src].id} %}}'
 
         # also deal with any lightbox <a>
         lightboxes = html.cssselect('a[data-lightbox]')
         for lightbox in lightboxes:
             lightbox.attrib['data-fslightbox'] = lightbox.attrib['data-lightbox']
             del lightbox.attrib['data-lightbox']
             if 'data-title' in lightbox.attrib:
@@ -327,14 +327,23 @@
                     tr.classes.discard('row-odd')
                 for div in table.cssselect('tbody > tr div.line'):
                     div.classes.discard('line')
                     div.classes.add('text-start')
                 for div in table.cssselect('tbody > tr p'):
                     div.classes.add('text-start')
             data['body'] = lxml.html.tostring(html).decode('utf-8')
+            # Unescape our template tags after lxml has converted our {% %}
+            # to entities.  The pattern we're looking for looks something
+            # like this::
+            #
+            #     %7B%%20sphinximage_url%2026%20%%7D
+            html = re.sub(r'%7B%%20', r'{% ', data['body'])
+            data['body'] = re.sub(r'%20([0-9]+)%20%%7D', r' \1 %}', html)
+            # Convert the weird paragraph symbols to actual paragraph symbols
+            data['body'] = re.sub(r'#61633;', r'para;', data['body'])
 
     def _fix_toc(self, data: Dict[str, Any]) -> None:
         """
         Update our page's local table of contents (``data['toc']`) to have the CSS
         classes we need in order for it to display properly.
 
         Args:
```

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/import_docs.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/import_docs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/parse_globaltoc.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/parse_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/print_classifier_tree.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/print_classifier_tree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/management/commands/print_doctree.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/management/commands/print_doctree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0001_initial.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0002_original_html.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0002_original_html.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0003_globaltoc.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0003_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0004_next_page_FK.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0004_next_page_FK.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0005_orig_global_toc.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0005_orig_global_toc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0007_load_classifiers.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0007_load_classifiers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0009_SphinxPage_searchable.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0009_SphinxPage_searchable.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0010_add_groups.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0010_add_groups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/migrations/0011_machinenamefield.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/migrations/0011_machinenamefield.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/models.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/models.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/search_indexes.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/settings.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/settings.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/signals.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/signals.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss` & `django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss` & `django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss` & `django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css` & `django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss` & `django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/static/sphinx_hosting/images/logo.jpg` & `django-sphinx-hosting-1.1.3/sphinx_hosting/static/sphinx_hosting/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/templates/sphinx_hosting/base.html` & `django-sphinx-hosting-1.1.3/sphinx_hosting/templates/sphinx_hosting/base.html`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/urls.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/validators.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/validators.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/views.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/classifier.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/classifier.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/navigation.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/navigation.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/project.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/project.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/search.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/search.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/sphinx_page.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/sphinx_page.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.2/sphinx_hosting/wildewidgets/version.py` & `django-sphinx-hosting-1.1.3/sphinx_hosting/wildewidgets/version.py`

 * *Files identical despite different names*

