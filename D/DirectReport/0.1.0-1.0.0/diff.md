# Comparing `tmp/DirectReport-0.1.0.tar.gz` & `tmp/DirectReport-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DirectReport-0.1.0.tar", last modified: Tue Apr 11 05:51:41 2023, max compression
+gzip compressed data, was "dist/DirectReport-1.0.0.tar", last modified: Thu May  4 03:49:36 2023, max compression
```

## Comparing `DirectReport-0.1.0.tar` & `DirectReport-1.0.0.tar`

### file list

```diff
@@ -1,53 +1,88 @@
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/
--rw-r--r--   0 christopherwebb   (501) staff       (20)       11 2023-04-11 05:47:22.000000 DirectReport-0.1.0/CONTRIBUTING.md
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/
--rw-r--r--   0 christopherwebb   (501) staff       (20)      602 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/__init__.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)      109 2023-03-22 09:20:35.000000 DirectReport-0.1.0/DirectReport/__main__.py
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/browserview/
--rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/browserview/__init__.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     1134 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/browserview/app.py
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/browserview/static/
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/browserview/static/css/
--rw-r--r--   0 christopherwebb   (501) staff       (20)      115 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/browserview/static/css/main.css
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/browserview/static/js/
--rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/browserview/static/js/index.js
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/browserview/templates/
--rw-r--r--   0 christopherwebb   (501) staff       (20)     1259 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/browserview/templates/404.html
--rw-r--r--   0 christopherwebb   (501) staff       (20)     1435 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/browserview/templates/base.html
--rw-r--r--   0 christopherwebb   (501) staff       (20)     2318 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/browserview/templates/detail.html
--rw-r--r--   0 christopherwebb   (501) staff       (20)      726 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/browserview/templates/index.html
--rw-r--r--   0 christopherwebb   (501) staff       (20)     1924 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/browserview/templates/list.html
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/commandline/
--rw-r--r--   0 christopherwebb   (501) staff       (20)       23 2023-03-22 09:20:35.000000 DirectReport-0.1.0/DirectReport/commandline/__init__.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     2674 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/commandline/commandline.py
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/database/
--rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/database/__init__.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     2580 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/database/daily_storage.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     3480 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/database/entry_storage.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     2515 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/database/weekly_storage.py
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/models/
--rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/models/__.init__.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     2158 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/models/entry.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     4236 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/models/list_builder.py
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport/tests/
--rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/tests/__init__.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     1379 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/tests/test_commandline.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     3668 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/tests/test_db.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)     1909 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/tests/test_list_builder.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)      810 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/tests/test_model.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)      390 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/tests/test_web.py
--rw-r--r--   0 christopherwebb   (501) staff       (20)      736 2023-04-11 05:47:22.000000 DirectReport-0.1.0/DirectReport/tests/test_weekly_storage.py
-drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport.egg-info/
--rw-r--r--   0 christopherwebb   (501) staff       (20)     3825 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport.egg-info/PKG-INFO
--rw-r--r--   0 christopherwebb   (501) staff       (20)     1265 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport.egg-info/SOURCES.txt
--rw-r--r--   0 christopherwebb   (501) staff       (20)        1 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport.egg-info/dependency_links.txt
--rw-r--r--   0 christopherwebb   (501) staff       (20)      142 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport.egg-info/requires.txt
--rw-r--r--   0 christopherwebb   (501) staff       (20)       13 2023-04-11 05:51:41.000000 DirectReport-0.1.0/DirectReport.egg-info/top_level.txt
--rw-r--r--   0 christopherwebb   (501) staff       (20)     1073 2023-03-15 07:44:50.000000 DirectReport-0.1.0/LICENSE
--rw-r--r--   0 christopherwebb   (501) staff       (20)      394 2023-04-11 05:47:22.000000 DirectReport-0.1.0/MANIFEST.in
--rw-r--r--   0 christopherwebb   (501) staff       (20)     2249 2023-04-11 05:47:22.000000 DirectReport-0.1.0/Makefile
--rw-r--r--   0 christopherwebb   (501) staff       (20)     3825 2023-04-11 05:51:41.000000 DirectReport-0.1.0/PKG-INFO
--rw-r--r--   0 christopherwebb   (501) staff       (20)     1773 2023-04-11 05:47:22.000000 DirectReport-0.1.0/README.md
--rw-r--r--   0 christopherwebb   (501) staff       (20)     2264 2023-04-11 05:47:22.000000 DirectReport-0.1.0/pyproject.toml
--rw-r--r--   0 christopherwebb   (501) staff       (20)       38 2023-04-11 05:51:41.000000 DirectReport-0.1.0/setup.cfg
--rw-r--r--   0 christopherwebb   (501) staff       (20)       61 2023-03-22 09:20:35.000000 DirectReport-0.1.0/setup.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     3997 2023-05-04 03:42:46.000000 DirectReport-1.0.0/CONTRIBUTING.md
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      168 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/__init__.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      149 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/__main__.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/browserview/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/browserview/__init__.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2578 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/browserview/app.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/browserview/static/
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/browserview/static/css/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      115 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/browserview/static/css/main.css
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/browserview/static/js/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      277 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/browserview/static/js/index.js
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/browserview/templates/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1259 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/browserview/templates/404.html
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1667 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/browserview/templates/base.html
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     8695 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/browserview/templates/detail.html
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1611 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/browserview/templates/index.html
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     6624 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/browserview/templates/list.html
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/commandline/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/commandline/__init__.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     5438 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/commandline/commandline.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/database/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)       63 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/database/__init__.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2351 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/database/blocker_storage.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     4432 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/database/daily_storage.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     4470 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/database/entry_storage.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2405 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/database/jira_storage.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2286 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/database/note_storage.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     4422 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/database/weekly_storage.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/models/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)       54 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/__init__.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/models/blocker_models/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/blocker_models/__init__.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1109 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/blocker_models/block_builder.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1134 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/blocker_models/blocker.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1532 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/daily_builder.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     4910 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/entry.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/models/jira_models/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/jira_models/__init__.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1231 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/jira_models/jira.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1056 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/jira_models/jira_builder.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2908 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/list_builder.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/models/note/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/note/__init__.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      784 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/note/note.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      651 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/note/note_builder.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2881 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/models/weekly_builder.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport/tests/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1876 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/tests/test_commandline.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     3485 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/tests/test_db.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)       23 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/tests/test_jira_data_store.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1007 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/tests/test_list_builder.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      725 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/tests/test_model.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      715 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/tests/test_web.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      714 2023-05-04 03:42:46.000000 DirectReport-1.0.0/DirectReport/tests/test_weekly_storage.py
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport.egg-info/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     4570 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport.egg-info/PKG-INFO
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2330 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport.egg-info/SOURCES.txt
+-rw-r--r--   0 christopherwebb   (501) staff       (20)        1 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport.egg-info/dependency_links.txt
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      142 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport.egg-info/requires.txt
+-rw-r--r--   0 christopherwebb   (501) staff       (20)       13 2023-05-04 03:49:36.000000 DirectReport-1.0.0/DirectReport.egg-info/top_level.txt
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1073 2023-05-04 03:42:46.000000 DirectReport-1.0.0/LICENSE
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      653 2023-05-04 03:42:46.000000 DirectReport-1.0.0/MANIFEST.in
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2697 2023-05-04 03:42:46.000000 DirectReport-1.0.0/Makefile
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     4570 2023-05-04 03:49:36.000000 DirectReport-1.0.0/PKG-INFO
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2518 2023-05-04 03:42:46.000000 DirectReport-1.0.0/README.md
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/docs/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2524 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/.nojekyll
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1227 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/Makefile
+-rwxr-xr-x   0 christopherwebb   (501) staff       (20)     1544 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/buildDocs.sh
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      804 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/make.bat
+drwxr-xr-x   0 christopherwebb   (501) staff       (20)        0 2023-05-04 03:49:36.000000 DirectReport-1.0.0/docs/source/
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      391 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/DirectReport.browserview.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      415 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/DirectReport.commandline.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1388 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/DirectReport.database.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      704 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/DirectReport.models.blocker_models.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      665 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/DirectReport.models.jira_models.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      596 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/DirectReport.models.note.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1094 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/DirectReport.models.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      319 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/DirectReport.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     1873 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/conf.py
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2213 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/index.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)       82 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/modules.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)      103 2023-05-04 03:42:46.000000 DirectReport-1.0.0/docs/source/setup.rst
+-rw-r--r--   0 christopherwebb   (501) staff       (20)     2263 2023-05-04 03:47:24.000000 DirectReport-1.0.0/pyproject.toml
+-rw-r--r--   0 christopherwebb   (501) staff       (20)       38 2023-05-04 03:49:36.000000 DirectReport-1.0.0/setup.cfg
+-rw-r--r--   0 christopherwebb   (501) staff       (20)       85 2023-05-04 03:45:07.000000 DirectReport-1.0.0/setup.py
```

### Comparing `DirectReport-0.1.0/DirectReport/browserview/templates/404.html` & `DirectReport-1.0.0/DirectReport/browserview/templates/404.html`

 * *Files identical despite different names*

### Comparing `DirectReport-0.1.0/DirectReport/browserview/templates/base.html` & `DirectReport-1.0.0/DirectReport/browserview/templates/base.html`

 * *Files 12% similar despite different names*

```diff
@@ -4,29 +4,30 @@
     <title>{% block title %}{% endblock %}</title>
     <meta charset="utf-8"/>
     <meta http-equiv="Content-type" content="text/html; charset=utf-8"/>
     <meta name="viewport" content="width=device-width, initial-scale=1"/>
     <script crossorigin src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
     <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
     <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
-    <script src="https://unpkg.com/browse/axios@1.3.5/dist/axios.min.js"></script>
-    <script src="https://cdn.tailwindcss.com"></script>
+    <script src="https://unpkg.com/axios@1.3.4/dist/axios.min.js"></script>
     <link rel="stylesheet" type="text/css" href="{{ url_for('static',filename='css/main.css') }}">
 </head>
 <header>
     <nav class="bg-gray-900 text-white w-screen">
-      <div class="px-14 py-6 flex w-full items-center">
-        <a class="ml-14 w-3/4 text-2xl font-bold" href="/">Direct Report.</a>
-        <!-- Nav Links -->
-        <ul class="flex px-6 font-semibold font-heading space-x-18">
-          <li><a class="px-6 text-1xl hover:text-gray-200" href="/">Home</a></li>
-          <li><a class="px-6 text-1xl hover:text-gray-200" href="/list">List</a></li>
-          <li><a class="px-6 text-1xl hover:text-gray-200" href="/wiki">Wiki</a></li>
-        </ul>
-      </div>
+        <div class="px-14 py-6 flex w-full items-center">
+            <a class="ml-14 w-3/4 text-2xl font-bold" href="/">DirectReport.</a>
+            <ul class="flex px-6 font-semibold font-heading space-x-18">
+                <li><a class="px-6 text-xl hover:text-gray-200" href="/">Home</a></li>
+                <li><a class="px-6 text-xl hover:text-gray-200" href="/new">New</a></li>
+                <li><a class="px-6 text-xl hover:text-gray-200" href="/list">List</a></li>
+                <li><a class="px-6 text-xl hover:text-gray-200" href="https://chriswebb09.github.io/DirectReport/">Documentation</a></li>
+            </ul>
+        </div>
     </nav>
 </header>
 <body>
 {% block content %}
 {% endblock %}
+<script src="https://cdn.tailwindcss.com?plugins=forms,typography,aspect-ratio"></script>
+<script src="https://unpkg.com/axios/dist/axios.min.js"></script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 
 
 
 
-Direct_Report.
+DirectReport.
     * Home
+    * New
     * List
-    * Wiki
+    * Documentation
 
 {% block content %} {% endblock %}
```

### Comparing `DirectReport-0.1.0/DirectReport/tests/test_db.py` & `DirectReport-1.0.0/DirectReport/tests/test_db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #!/usr/bin/env python3
 
 from DirectReport.models.entry import Entry
 from DirectReport.database.entry_storage import EntryStorage
-import os
-
-import tempfile
-import uuid
 from datetime import datetime
 from pathlib import Path
+import tempfile
+import pytest
+import uuid
 import sys
+import os
 
 file = Path(__file__).resolve()
 package_root_directory = file.parents[1]
 sys.path.append(str(package_root_directory))
-
 sys.path.append('.')
 
-import pytest
-
 
 @pytest.fixture
 def temp_db():
     db_fd, db_path = tempfile.mkstemp()
     yield db_path
     os.close(db_fd)
     os.remove(db_path)
@@ -38,15 +35,14 @@
     entry = Entry(
         uuid=uuid.uuid4(),
         topic="My topic",
         message="Test message",
         created_at=datetime.now(),
         modified_on=datetime.now(),
         week_uuid=uuid.uuid4(),
-        day_uuid=uuid.uuid4(),
     )
 
     storage.add_entry(entry)
     retrieved_entry = storage.get_entry(entry.uuid)
 
     assert entry.message == retrieved_entry.message
 
@@ -56,15 +52,14 @@
     entry = Entry(
         uuid=uuid.uuid4(),
         topic="Test Topic",
         message="Test message",
         created_at=datetime.now(),
         modified_on=datetime.now(),
         week_uuid=uuid.uuid4(),
-        day_uuid=uuid.uuid4(),
     )
     storage.add_entry(entry)
     entry.message = "Updated message"
     entry.modified_on = datetime.now()
     storage.update_entry(entry)
     retrieved_entry = storage.get_entry(entry.uuid)
     assert entry.message == retrieved_entry.message
@@ -75,15 +70,14 @@
     entry = Entry(
         uuid=uuid.uuid4(),
         topic="New Topic",
         message="Test message",
         created_at=datetime.now(),
         modified_on=datetime.now(),
         week_uuid=uuid.uuid4(),
-        day_uuid=uuid.uuid4(),
     )
 
     storage.add_entry(entry)
     storage.delete_entry(entry.uuid)
     retrieved_entry = storage.get_entry(entry.uuid)
 
     assert retrieved_entry is None
@@ -94,30 +88,28 @@
     entry1 = Entry(
         uuid=uuid.uuid4(),
         topic="New",
         message="Test message 1",
         created_at=datetime.now(),
         modified_on=datetime.now(),
         week_uuid=uuid.uuid4(),
-        day_uuid=uuid.uuid4(),
     )
     entry2 = Entry(
         uuid=uuid.uuid4(),
         topic="Topic new",
         message="Test message 2",
         created_at=datetime.now(),
         modified_on=datetime.now(),
         week_uuid=uuid.uuid4(),
-        day_uuid=uuid.uuid4(),
     )
 
     storage.add_entry(entry1)
     storage.add_entry(entry2)
 
-    entries = storage.get_all_entries()
+    entries = storage.list_all_entries()
     assert len(entries) == 2
     # assert entry1 in entries
     # assert entry2 in entries
 
 
 def test_get_entries_by_week(temp_db):
     storage = EntryStorage(temp_db)
@@ -125,24 +117,23 @@
     entry1 = Entry(
         uuid=uuid.uuid4(),
         topic="Topic",
         message="Test message 1",
         created_at=datetime.now(),
         modified_on=datetime.now(),
         week_uuid=week_uuid,
-        day_uuid=uuid.uuid4(),
     )
     entry2: Entry = Entry(
         uuid=uuid.uuid4(),
         topic="Topic 3",
         message="Test message 2",
         created_at=datetime.now(),
         modified_on=datetime.now(),
         week_uuid=uuid.uuid4(),
-        day_uuid=uuid.uuid4(),
     )
 
     storage.add_entry(entry1)
     storage.add_entry(entry2)
 
     entries = storage.get_entries_by_week(week_uuid)
+    # et_entries_by_week(week_uuid)
     assert len(entries) == 1
```

### Comparing `DirectReport-0.1.0/DirectReport/tests/test_weekly_storage.py` & `DirectReport-1.0.0/DirectReport/tests/test_weekly_storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from DirectReport.database.weekly_storage import WeekUUIDTable
-from DirectReport.models import list_builder
+#!/usr/bin/env python3
+
+import os
+import sys
 import tempfile
 import uuid
-import os
 from datetime import datetime
-import pytest
-import sys
 from pathlib import Path
+import pytest
+from DirectReport.database.weekly_storage import WeekUUIDTable
 
 file = Path(__file__).resolve()
 package_root_directory = file.parents[1]
 sys.path.append(str(package_root_directory))
-
 sys.path.append('.')
 
 
 @pytest.fixture
 def temp_db():
     db_fd, db_path = tempfile.mkstemp()
     yield db_path
```

### Comparing `DirectReport-0.1.0/DirectReport.egg-info/PKG-INFO` & `DirectReport-1.0.0/DirectReport.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DirectReport
-Version: 0.1.0
+Version: 1.0.0
 Summary: Direct Report
 Author-email: Christopher Webb <cdw2146@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Christopher Webb
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,22 +40,37 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 # DirectReport
 
 ![License](https://img.shields.io/github/license/chriswebb09/DirectReport)
 ![Issues](https://img.shields.io/github/issues/chriswebb09/DirectReport)
-[![codecov](https://codecov.io/gh/chriswebb09/DirectReport/branch/main/graph/badge.svg?token=E802G1JVJ5)](https://codecov.io/gh/chriswebb09/DirectReport)
+![codecov](https://codecov.io/gh/chriswebb09/DirectReport/branch/main/graph/badge.svg?token=E802G1JVJ5)
+![build](https://github.com/chriswebb09/DirectReport/actions/workflows/build.yml/badge.svg)
+![GitHub Latest Release](https://img.shields.io/github/v/release/chriswebb09/DirectReport?logo=github)
+![ReadTheDocs](https://readthedocs.org/projects/directreport/badge/?version=latest)
+
 
 # Overview
 
 Keep track of your accomplishments each day of the workweek, create a report of things you accomplished at the end of the week that you can email to manager.  Review progress each quarterly for more effective performance review.
 
+## Documentation 
+
+[Github Page](https://chriswebb09.github.io/DirectReport/)
+
 ## Installing
 
+### From Package Manager 
+
+Using pip: 
+`pip install DirectReport`
+
+### From Project Files: 
+
 This project uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
 - `make annotate`: run type checking using `mypy`
@@ -91,30 +106,48 @@
 
 ### Show-List
 
 
 #### Basic
 
 ```
- $ python DirectReport show-list
+ $ python DirectReport list
 ```
 
 
 #### All
 
 ```
-$ python DirectReport show-list --all
+$ python DirectReport list --all
  ```
  
- #### Daily
+#### Daily
  
  ```
-$ python DirectReport show-list --daily
+$ python DirectReport list --day
 ```
 
- #### Weekly
+#### Weekly
 
 ```
 
-$ python DirectReport show-list --weekly
+$ python DirectReport list --week
 
 ```
+
+## Web Interface
+
+### Home
+
+Web interface home page - WIP
+
+![Screenshot home page for web interface.](DirectReport/assets/web_interface.png)
+
+### List
+
+Web interface for list page - WIP
+
+![Screenshot list page for web interface.](DirectReport/assets/web_interface2.png)
+
+### Detail
+
+![Screenshot detail page for web interface.](DirectReport/assets/web_interface4.png)
```

### Comparing `DirectReport-0.1.0/LICENSE` & `DirectReport-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DirectReport-0.1.0/Makefile` & `DirectReport-1.0.0/Makefile`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+TMPREPO=/tmp/docs/DirectReport
+
 #########
 # BUILD #
 #########
 develop:  ## install dependencies and build library
 	python3 -m pip install Flask --user
 	python3 -m pip install -e .[develop]
 
@@ -12,15 +14,15 @@
 	python3 -m pip install --user .
 
 #########
 # LINTS #
 #########
 lint:  ## run static analysis with flake8
 	python3 -m black --check DirectReport setup.py
-	python3 -m flake8 DirectReport setup.py
+	python3 -m flake8 DirectReport setup.py --ignore=E501,F401,F403
 
 # Alias
 lints: lint
 
 format:  ## run autoformatting with black
 	python3 -m black DirectReport/ setup.py
 
@@ -37,18 +39,18 @@
 	python3 -m mypy ./DirectReport
 
 #########
 # TESTS #
 #########
 test:
     ## clean and run unit tests
-	python3 -m pytest -v DirectReport/tests
+	python3 -m pytest -v DirectReport/tests/
 
 coverage:  ## clean and run unit tests with coverage
-	python3 -m pytest -v DirectReport/tests --cov=DirectReport --cov-branch --cov-fail-under=60 --cov-report term-missing
+	python3 -m pytest -v DirectReport/tests --cov=DirectReport --cov-branch --cov-fail-under=5 --cov-report term-missing
 
 # Alias
 tests: test
 
 ###########
 # VERSION #
 ###########
@@ -73,14 +75,36 @@
 dist-check:
 	python3 -m twine check dist/*
 
 dist: clean build dist-build dist-check  ## Build dists
 
 publish:  # Upload python assets
 	echo "would usually run python -m twine upload dist/* --skip-existing"
+	
+########
+# PAGES #
+########
+
+docs:
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages:
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages git@github.com:chriswebb09/DirectReport.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/source/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
+
+serve:
+	cd docs/source/html; \
+	python3 -m http.server 9087
 
 #########
 # CLEAN #
 #########
 
 clean: ## clean the repository
 	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
```

### Comparing `DirectReport-0.1.0/PKG-INFO` & `DirectReport-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DirectReport
-Version: 0.1.0
+Version: 1.0.0
 Summary: Direct Report
 Author-email: Christopher Webb <cdw2146@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Christopher Webb
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,22 +40,37 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 # DirectReport
 
 ![License](https://img.shields.io/github/license/chriswebb09/DirectReport)
 ![Issues](https://img.shields.io/github/issues/chriswebb09/DirectReport)
-[![codecov](https://codecov.io/gh/chriswebb09/DirectReport/branch/main/graph/badge.svg?token=E802G1JVJ5)](https://codecov.io/gh/chriswebb09/DirectReport)
+![codecov](https://codecov.io/gh/chriswebb09/DirectReport/branch/main/graph/badge.svg?token=E802G1JVJ5)
+![build](https://github.com/chriswebb09/DirectReport/actions/workflows/build.yml/badge.svg)
+![GitHub Latest Release](https://img.shields.io/github/v/release/chriswebb09/DirectReport?logo=github)
+![ReadTheDocs](https://readthedocs.org/projects/directreport/badge/?version=latest)
+
 
 # Overview
 
 Keep track of your accomplishments each day of the workweek, create a report of things you accomplished at the end of the week that you can email to manager.  Review progress each quarterly for more effective performance review.
 
+## Documentation 
+
+[Github Page](https://chriswebb09.github.io/DirectReport/)
+
 ## Installing
 
+### From Package Manager 
+
+Using pip: 
+`pip install DirectReport`
+
+### From Project Files: 
+
 This project uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
 - `make annotate`: run type checking using `mypy`
@@ -91,30 +106,48 @@
 
 ### Show-List
 
 
 #### Basic
 
 ```
- $ python DirectReport show-list
+ $ python DirectReport list
 ```
 
 
 #### All
 
 ```
-$ python DirectReport show-list --all
+$ python DirectReport list --all
  ```
  
- #### Daily
+#### Daily
  
  ```
-$ python DirectReport show-list --daily
+$ python DirectReport list --day
 ```
 
- #### Weekly
+#### Weekly
 
 ```
 
-$ python DirectReport show-list --weekly
+$ python DirectReport list --week
 
 ```
+
+## Web Interface
+
+### Home
+
+Web interface home page - WIP
+
+![Screenshot home page for web interface.](DirectReport/assets/web_interface.png)
+
+### List
+
+Web interface for list page - WIP
+
+![Screenshot list page for web interface.](DirectReport/assets/web_interface2.png)
+
+### Detail
+
+![Screenshot detail page for web interface.](DirectReport/assets/web_interface4.png)
```

### Comparing `DirectReport-0.1.0/README.md` & `DirectReport-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 # DirectReport
 
 ![License](https://img.shields.io/github/license/chriswebb09/DirectReport)
 ![Issues](https://img.shields.io/github/issues/chriswebb09/DirectReport)
-[![codecov](https://codecov.io/gh/chriswebb09/DirectReport/branch/main/graph/badge.svg?token=E802G1JVJ5)](https://codecov.io/gh/chriswebb09/DirectReport)
+![codecov](https://codecov.io/gh/chriswebb09/DirectReport/branch/main/graph/badge.svg?token=E802G1JVJ5)
+![build](https://github.com/chriswebb09/DirectReport/actions/workflows/build.yml/badge.svg)
+![GitHub Latest Release](https://img.shields.io/github/v/release/chriswebb09/DirectReport?logo=github)
+![ReadTheDocs](https://readthedocs.org/projects/directreport/badge/?version=latest)
+
 
 # Overview
 
 Keep track of your accomplishments each day of the workweek, create a report of things you accomplished at the end of the week that you can email to manager.  Review progress each quarterly for more effective performance review.
 
+## Documentation 
+
+[Github Page](https://chriswebb09.github.io/DirectReport/)
+
 ## Installing
 
+### From Package Manager 
+
+Using pip: 
+`pip install DirectReport`
+
+### From Project Files: 
+
 This project uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
 - `make annotate`: run type checking using `mypy`
@@ -49,30 +64,48 @@
 
 ### Show-List
 
 
 #### Basic
 
 ```
- $ python DirectReport show-list
+ $ python DirectReport list
 ```
 
 
 #### All
 
 ```
-$ python DirectReport show-list --all
+$ python DirectReport list --all
  ```
  
- #### Daily
+#### Daily
  
  ```
-$ python DirectReport show-list --daily
+$ python DirectReport list --day
 ```
 
- #### Weekly
+#### Weekly
 
 ```
 
-$ python DirectReport show-list --weekly
+$ python DirectReport list --week
 
 ```
+
+## Web Interface
+
+### Home
+
+Web interface home page - WIP
+
+![Screenshot home page for web interface.](DirectReport/assets/web_interface.png)
+
+### List
+
+Web interface for list page - WIP
+
+![Screenshot list page for web interface.](DirectReport/assets/web_interface2.png)
+
+### Detail
+
+![Screenshot detail page for web interface.](DirectReport/assets/web_interface4.png)
```

### Comparing `DirectReport-0.1.0/pyproject.toml` & `DirectReport-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "DirectReport"
 authors = [{name = "Christopher Webb", email = "cdw2146@columbia.edu"}]
 description="Direct Report"
 readme = "README.md"
-version = "0.1.0"
+version = "1.0.0"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -58,21 +58,22 @@
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
 
 [tool.check-manifest]
 ignore = [
+    'Assets/*'
 ]
 
 [tool.flake8]
-ignore = ['E203', 'W503']
+ignore = ['E203', 'W503', 'F401']
 max-line-length=120
 exclude=[
-    'DirectReport/tests/*'
+    'tests/*'
 ]
 per-file-ignores= [
     'DirectReport/__init__.py:F401, F403'
 ]
 
 
 [tool.isort]
@@ -101,8 +102,8 @@
 # disallow_untyped_calls = true
 
 [tool.pytest.ini_options]
 pythonpath = [
   "."
 ]
 asyncio_mode = 'strict'
-testpaths = 'DirectReport/tests'
+testpaths = 'tests/'
```

