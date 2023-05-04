# Comparing `tmp/memorious-2.5.0.tar.gz` & `tmp/memorious-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memorious-2.5.0.tar", last modified: Mon Feb 28 07:37:42 2022, max compression
+gzip compressed data, was "memorious-2.6.2.tar", last modified: Thu May  4 11:54:31 2023, max compression
```

## Comparing `memorious-2.5.0.tar` & `memorious-2.6.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 07:37:42.339621 memorious-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-02-28 07:35:28.000000 memorious-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-02-28 07:37:42.339621 memorious-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-02-28 07:35:28.000000 memorious-2.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 07:37:42.335621 memorious-2.5.0/memorious/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 07:37:42.335621 memorious-2.5.0/memorious/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/helpers/asp.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/helpers/dates.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/helpers/key.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/helpers/ocr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/helpers/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    29876 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/helpers/ua.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 07:37:42.335621 memorious-2.5.0/memorious/logic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/logic/check.py
--rw-r--r--   0 runner    (1001) docker     (121)     7655 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/logic/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     5154 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/logic/crawler.py
--rw-r--r--   0 runner    (1001) docker     (121)    13178 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/logic/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/logic/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/logic/mime.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/logic/stage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 07:37:42.335621 memorious-2.5.0/memorious/model/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/model/crawl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/model/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 07:37:42.339621 memorious-2.5.0/memorious/operations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8193 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/aleph.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/db.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3721 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/documentcloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/fetch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/ftm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/ftp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/initializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3763 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/store.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/operations/webdav.py
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 07:37:42.339621 memorious-2.5.0/memorious/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/test_crawler.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/test_documentcloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     5205 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6237 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/test_reporting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2269 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/tests/test_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-02-28 07:35:28.000000 memorious-2.5.0/memorious/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 07:37:42.335621 memorious-2.5.0/memorious.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-02-28 07:37:41.000000 memorious-2.5.0/memorious.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-02-28 07:37:42.000000 memorious-2.5.0/memorious.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 07:37:41.000000 memorious-2.5.0/memorious.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-02-28 07:37:42.000000 memorious-2.5.0/memorious.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 07:37:42.000000 memorious-2.5.0/memorious.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 07:37:25.000000 memorious-2.5.0/memorious.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-02-28 07:37:42.000000 memorious-2.5.0/memorious.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-28 07:37:42.000000 memorious-2.5.0/memorious.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-02-28 07:37:42.339621 memorious-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3657 2022-02-28 07:35:28.000000 memorious-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.941674 memorious-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 11:52:27.000000 memorious-2.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-04 11:54:31.941674 memorious-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-04 11:52:27.000000 memorious-2.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.933674 memorious-2.6.2/memorious/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.937674 memorious-2.6.2/memorious/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/asp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29876 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/ua.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.937674 memorious-2.6.2/memorious/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.937674 memorious-2.6.2/memorious/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/model/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/model/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.937674 memorious-2.6.2/memorious/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/documentcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/ftm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.941674 memorious-2.6.2/memorious/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_documentcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.933674 memorious-2.6.2/memorious.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:54:02.000000 memorious-2.6.2/memorious.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 11:54:31.941674 memorious-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-04 11:52:27.000000 memorious-2.6.2/setup.py
```

### Comparing `memorious-2.5.0/LICENSE` & `memorious-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/README.rst` & `memorious-2.6.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -35,13 +35,13 @@
 3. Write code for stage operations (optional)
 4. Test, rinse, repeat
 
 Documentation
 -------------
 
 The documentation for Memorious is available at
-`memorious.readthedocs.io <https://memorious.readthedocs.io/>`_.
+`alephdata.github.io/memorious <https://alephdata.github.io/memorious/>`_.
 Feel free to edit the source files in the ``docs`` folder and send pull requests for improvements.
 
 To build the documentation, inside the ``docs`` folder run ``make html``
 
 You'll find the resulting HTML files in /docs/_build/html.
```

### Comparing `memorious-2.5.0/memorious/__init__.py` & `memorious-2.6.2/memorious/__init__.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/cli.py` & `memorious-2.6.2/memorious/cli.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/core.py` & `memorious-2.6.2/memorious/core.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/exc.py` & `memorious-2.6.2/memorious/exc.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/helpers/__init__.py` & `memorious-2.6.2/memorious/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/helpers/asp.py` & `memorious-2.6.2/memorious/helpers/asp.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/helpers/dates.py` & `memorious-2.6.2/memorious/helpers/dates.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/helpers/ocr.py` & `memorious-2.6.2/memorious/helpers/ocr.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/helpers/rule.py` & `memorious-2.6.2/memorious/helpers/rule.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/helpers/ua.py` & `memorious-2.6.2/memorious/helpers/ua.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/logic/check.py` & `memorious-2.6.2/memorious/logic/check.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/logic/context.py` & `memorious-2.6.2/memorious/logic/context.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/logic/crawler.py` & `memorious-2.6.2/memorious/logic/crawler.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/logic/http.py` & `memorious-2.6.2/memorious/logic/http.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/logic/manager.py` & `memorious-2.6.2/memorious/logic/manager.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/logic/mime.py` & `memorious-2.6.2/memorious/logic/mime.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/logic/stage.py` & `memorious-2.6.2/memorious/logic/stage.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/model/crawl.py` & `memorious-2.6.2/memorious/model/crawl.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/model/queue.py` & `memorious-2.6.2/memorious/model/queue.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/aleph.py` & `memorious-2.6.2/memorious/operations/aleph.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/clean.py` & `memorious-2.6.2/memorious/operations/clean.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/db.py` & `memorious-2.6.2/memorious/operations/db.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/documentcloud.py` & `memorious-2.6.2/memorious/operations/documentcloud.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/extract.py` & `memorious-2.6.2/memorious/operations/extract.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/fetch.py` & `memorious-2.6.2/memorious/operations/fetch.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/ftm.py` & `memorious-2.6.2/memorious/operations/ftm.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/ftp.py` & `memorious-2.6.2/memorious/operations/ftp.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/initializers.py` & `memorious-2.6.2/memorious/operations/initializers.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/parse.py` & `memorious-2.6.2/memorious/operations/parse.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/store.py` & `memorious-2.6.2/memorious/operations/store.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/operations/webdav.py` & `memorious-2.6.2/memorious/operations/webdav.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/settings.py` & `memorious-2.6.2/memorious/settings.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/tests/conftest.py` & `memorious-2.6.2/memorious/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/tests/test_context.py` & `memorious-2.6.2/memorious/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/tests/test_crawler.py` & `memorious-2.6.2/memorious/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/tests/test_documentcloud.py` & `memorious-2.6.2/memorious/tests/test_documentcloud.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/tests/test_extract.py` & `memorious-2.6.2/memorious/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/tests/test_http.py` & `memorious-2.6.2/memorious/tests/test_http.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,132 @@
 import os
 import pytest
 from requests import Session, Response, Request
 from lxml import html, etree
 
 from memorious.logic.http import ContextHttpResponse
 
+HTTPBIN = os.environ.get("HTTPBIN", "https://proxy:443")
+
 
 class TestContextHttp(object):
     def test_session(self, http):
         assert isinstance(http.session, Session)
 
     def test_response(self, http):
-        response = http.get("https://httpbin.org/get")
+        response = http.get(f"{HTTPBIN}/get")
         assert isinstance(response, ContextHttpResponse)
         assert isinstance(response._response, Response)
 
     def test_response_lazy(self, http):
-        response = http.get("https://httpbin.org/get", lazy=True)
+        response = http.get(f"{HTTPBIN}/get", lazy=True)
         assert isinstance(response, ContextHttpResponse)
         assert response._response is None
 
 
 class TestContextHttpResponse(object):
     def test_fetch_response(self, http):
-        request = Request("GET", "https://httpbin.org/get")
+        request = Request("GET", f"{HTTPBIN}/get")
         context_http_response = ContextHttpResponse(http, request)
         file_path = context_http_response.fetch()
         assert os.path.exists(file_path)
 
     def test_contenttype(self, http):
-        request = Request("GET", "https://httpbin.org/get")
+        request = Request("GET", f"{HTTPBIN}/get")
         context_http_response = ContextHttpResponse(http, request)
         assert context_http_response.content_type == "application/json"
 
     def test_attachment(self, http):
         request = Request(
             "GET",
-            "https://httpbin.org/response-headers?Content-Type="
+            f"{HTTPBIN}/response-headers?Content-Type="
             "text/plain;%20charset=UTF-8&Content-Disposition=attachment;"
             "%20filename%3d%22test.json%22",
         )
         context_http_response = ContextHttpResponse(http, request)
         assert context_http_response.file_name == "test.json"
 
     @pytest.mark.parametrize(
         "url,encoding",
         [
-            ("https://httpbin.org/response-headers?charset=", "utf-8"),
+            (f"{HTTPBIN}/response-headers?charset=", "utf-8"),
             (
-                "https://httpbin.org/response-headers?content-type=text"
+                f"{HTTPBIN}/response-headers?content-type=text"
                 "/plain;%20charset=utf-16",
                 "utf-16",
             ),
             (
-                "https://httpbin.org/response-headers?Content-Type=text/"
+                f"{HTTPBIN}/response-headers?Content-Type=text/"
                 "plain;%20charset=utf-32",
                 "utf-32",
             ),
         ],
     )
     def test_encoding(self, url, encoding, http):
         request = Request("GET", url)
         context_http_response = ContextHttpResponse(http, request)
         assert context_http_response.encoding == encoding
 
     def test_request_id(self, http):
-        request = Request("GET", "https://httpbin.org/get", data={"hello": "world"})
+        request = Request("GET", f"{HTTPBIN}/get", data={"hello": "world"})
         context_http_response = ContextHttpResponse(http, request)
         assert context_http_response._request_id is None
         assert isinstance(context_http_response.request_id, str)
 
     def test_content(self, http):
         request = Request(
             "GET",
-            "https://httpbin.org/user-agent",
+            f"{HTTPBIN}/user-agent",
             headers={"User-Agent": "Memorious Test"},
         )
         context_http_response = ContextHttpResponse(http, request)
         assert isinstance(context_http_response.raw, bytes)
         assert isinstance(context_http_response.text, str)
         assert context_http_response.json == {"user-agent": "Memorious Test"}
 
     def test_html(self, http):
-        request = Request("GET", "https://httpbin.org/html")
+        request = Request("GET", f"{HTTPBIN}/html")
         context_http_response = ContextHttpResponse(http, request)
         assert isinstance(context_http_response.html, html.HtmlElement)
 
     def test_xml(self, http):
-        request = Request("GET", "https://httpbin.org/xml")
+        request = Request("GET", f"{HTTPBIN}/xml")
         context_http_response = ContextHttpResponse(http, request)
         assert isinstance(context_http_response.xml, etree._ElementTree)
 
     def test_apply_data(self, http):
         context_http_response = ContextHttpResponse(http)
         assert context_http_response.url is None
         assert context_http_response.status_code is None
         context_http_response.apply_data(
-            data={"status_code": 200, "url": "https://httpbin.org/get"}
+            data={"status_code": 200, "url": f"{HTTPBIN}/get"}
         )
-        assert context_http_response.url == "https://httpbin.org/get"
+        assert context_http_response.url == f"{HTTPBIN}/get"
         assert context_http_response.status_code == 200
 
     def test_deserialize(self, http):
-        data = {"status_code": 200, "url": "https://httpbin.org/get"}
+        data = {"status_code": 200, "url": f"{HTTPBIN}/get"}
         context_http_response = ContextHttpResponse.deserialize(http, data)
         assert isinstance(context_http_response, ContextHttpResponse)
-        assert context_http_response.url == "https://httpbin.org/get"
+        assert context_http_response.url == f"{HTTPBIN}/get"
         assert context_http_response.status_code == 200
 
     def test_close(self, http):
-        request = Request("GET", "https://httpbin.org/get")
+        request = Request("GET", f"{HTTPBIN}/get")
         context_http_response = ContextHttpResponse(http, request)
         file_path = context_http_response.fetch()
         assert os.path.exists(file_path)
         context_http_response.close()
         # assert not os.path.exists(file_path)
 
     @pytest.mark.parametrize(
         "url,status_code",
         [
-            ("https://httpbin.org/status/404", 404),
-            ("https://httpbin.org/status/500", 500),
-            ("https://httpbin.org/status/200", 200),
+            (f"{HTTPBIN}/status/404", 404),
+            (f"{HTTPBIN}/status/500", 500),
+            (f"{HTTPBIN}/status/200", 200),
         ],
     )
     def test_status_code(self, url, status_code, http):
         request = Request("GET", url)
         context_http_response = ContextHttpResponse(http, request)
         assert context_http_response.status_code == status_code
```

### Comparing `memorious-2.5.0/memorious/tests/test_manager.py` & `memorious-2.6.2/memorious/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/tests/test_operations.py` & `memorious-2.6.2/memorious/tests/test_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,57 +6,59 @@
 
 from memorious.core import tags, storage
 from memorious.operations.fetch import fetch, session
 from memorious.operations.parse import parse
 from memorious.operations.initializers import seed, sequence, dates, enumerate
 from memorious.operations.store import directory, cleanup_archive
 
+HTTPBIN = os.environ.get("HTTPBIN", "https://proxy:443")
+
 
 @pytest.mark.parametrize(
     "url,call_count",
     [
-        ("https://httpbin.org/html", 1),
+        (f"{HTTPBIN}/html", 1),
         ("https://occrp.org/", 0),
-        ("https://httpbin.org/status/418", 0),
+        (f"{HTTPBIN}/status/418", 0),
     ],
 )
 def test_fetch(url, call_count, context, mocker):
-    rules = {"pattern": "https://httpbin.org/*"}
+    rules = {"pattern": f"{HTTPBIN}/*"}
     context.params["rules"] = rules
     mocker.patch.object(context, "emit")
     fetch(context, {"url": url})
     assert context.emit.call_count == call_count
 
 
 def test_session(context, mocker):
     context.params["user"] = "user"
     context.params["password"] = "password"
     context.params["user_agent"] = "Godzilla Firehose 0.1"
-    context.params["url"] = "https://httpbin.org/get"
+    context.params["url"] = f"{HTTPBIN}/get"
     data = {"hello": "world"}
     mocker.patch.object(context.http, "save")
     mocker.patch.object(context, "emit")
 
     session(context, data)
 
     assert context.http.save.called_one_with()
     assert context.emit.called_one_with(data=data)
     assert context.http.session.headers["User-Agent"] == "Godzilla Firehose 0.1"
-    assert context.http.session.headers["Referer"] == "https://httpbin.org/get"
+    assert context.http.session.headers["Referer"] == f"{HTTPBIN}/get"
     assert context.http.session.auth == ("user", "password")
 
 
 def test_parse(context, mocker):
     url = "http://example.org/"
     result = context.http.get(url)
     data = result.serialize()
 
     mocker.patch.object(context, "emit")
 
-    rules = {"pattern": "https://httpbin.org/*"}
+    rules = {"pattern": f"{HTTPBIN}/*"}
     context.params["store"] = rules
     context.params["meta"] = {"title": ".//h1", "description": ".//p"}
     parse(context, data)
     assert context.emit.call_count == 1
     context.emit.assert_called_once_with(rule="fetch", data=ANY)
 
     # cleanup tags
@@ -74,35 +76,33 @@
 def test_parse_ftm(context, mocker):
     url = "https://www.occrp.org/en/daily/14082-riviera-maya-gang-members-sentenced-in-romania"
     result = context.http.get(url)
     data = result.serialize()
     context.params["schema"] = "Article"
     context.params["properties"] = {
         "title": './/meta[@property="og:title"]/@content',
-        "author": './/meta[@name="author"]/@content',
         "publishedAt": './/*[@class="date"]/text()',
         "description": './/meta[@property="og:description"]/@content',
     }
 
     parse(context, data)
 
     props = data["properties"]
 
     assert "Riviera Maya Gang Members Sentenced in Romania" in props["title"]
-    assert "Attila Biro" in props["author"]
     assert props["description"][0].startswith("A Bucharest court")
 
 
 def test_seed(context, mocker):
     context.params["url"] = None
-    context.params["urls"] = ["http://httpbin.org/status/%(status)s"]
+    context.params["urls"] = [f"{HTTPBIN}/status/%(status)s"]
     mocker.patch.object(context, "emit")
     seed(context, data={"status": 404})
     assert context.emit.call_count == 1
-    context.emit.assert_called_once_with(data={"url": "http://httpbin.org/status/404"})
+    context.emit.assert_called_once_with(data={"url": f"{HTTPBIN}/status/404"})
 
 
 def test_sequence(context, mocker):
     mocker.patch.object(context, "emit")
 
     context.params["start"] = 2
     context.params["stop"] = 11
@@ -152,15 +152,15 @@
     file_path = os.path.realpath(__file__)
     store_dir = os.path.normpath(
         os.path.join(file_path, "../testdata/data/store/occrp_web_site")
     )
     shutil.rmtree(store_dir, ignore_errors=True)
 
     # echo user-agent
-    url = "https://httpbin.org/user-agent"
+    url = f"{HTTPBIN}/user-agent"
     result = context.http.get(url, headers={"User-Agent": "Memorious Test"})
     data = result.serialize()
     directory(context, data)
 
     content_hash = data.get("content_hash")
 
     raw_file_path = os.path.join(store_dir, content_hash + ".data.json")
@@ -171,13 +171,13 @@
     with open(meta_file_path, "rb") as fh:
         assert json.load(fh)["content_hash"] == data["content_hash"]
     with open(raw_file_path, "rb") as fh:
         assert b'"user-agent": "Memorious Test"' in fh.read()
 
 
 def test_cleanup_archive(context):
-    url = "https://httpbin.org/user-agent"
+    url = f"{HTTPBIN}/user-agent"
     result = context.http.get(url, headers={"User-Agent": "Memorious Test"})
     data = result.serialize()
     assert storage.load_file(data["content_hash"]) is not None
     cleanup_archive(context, data)
     assert storage.load_file(data["content_hash"]) is None
```

### Comparing `memorious-2.5.0/memorious/tests/test_reporting.py` & `memorious-2.6.2/memorious/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/tests/test_rule.py` & `memorious-2.6.2/memorious/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious/worker.py` & `memorious-2.6.2/memorious/worker.py`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious.egg-info/SOURCES.txt` & `memorious-2.6.2/memorious.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/memorious.egg-info/entry_points.txt` & `memorious-2.6.2/memorious.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `memorious-2.5.0/setup.py` & `memorious-2.6.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="memorious",
-    version="2.5.0",
+    version="2.6.2",
     description="A minimalistic, recursive web crawling library for Python.",
-    long_description="",
+    long_description=long_description,
+    long_description_content_type="text/x-rst",
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
     ],
     keywords="",
     author="Organized Crime and Corruption Reporting Project",
@@ -34,15 +39,15 @@
         "PySocks == 1.7.1",
         "requests_ftp",
         "lxml >= 4",
         "normality >= 2.1.1, < 3.0.0",
         "tabulate",
         "python-dateutil >= 2.8.2, < 3.0.0",
         "dataset >= 1.0.8",
-        "servicelayer[google,amazon] == 1.19.0",
+        "servicelayer[google,amazon] == 1.20.7",
         "pantomime == 0.5.1",
         "alephclient >= 2.3.5",
         "followthemoney >= 2.3.1",
         "followthemoney-store >= 3.0.1",
         "dateparser",
         "stringcase",
         "flask",
```

