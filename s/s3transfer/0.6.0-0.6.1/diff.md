# Comparing `tmp/s3transfer-0.6.0.tar.gz` & `tmp/s3transfer-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3transfer-0.6.0.tar", last modified: Tue May 31 18:37:19 2022, max compression
+gzip compressed data, was "dist/s3transfer-0.6.1.tar", last modified: Thu May  4 19:39:46 2023, max compression
```

## Comparing `s3transfer-0.6.0.tar` & `s3transfer-0.6.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:37:19.371464 s3transfer-0.6.0/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-05-31 18:34:54.000000 s3transfer-0.6.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       81 2022-05-31 18:32:38.000000 s3transfer-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       83 2022-05-31 18:32:38.000000 s3transfer-0.6.0/NOTICE.txt
--rw-r--r--   0 root         (0) root         (0)     1491 2022-05-31 18:37:19.371464 s3transfer-0.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      664 2022-05-31 18:34:54.000000 s3transfer-0.6.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-31 18:34:54.000000 s3transfer-0.6.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:37:19.371464 s3transfer-0.6.0/s3transfer/
--rw-r--r--   0 root         (0) root         (0)    29040 2022-05-31 18:37:19.000000 s3transfer-0.6.0/s3transfer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15635 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/bandwidth.py
--rw-r--r--   0 root         (0) root         (0)     2970 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/compat.py
--rw-r--r--   0 root         (0) root         (0)      910 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/constants.py
--rw-r--r--   0 root         (0) root         (0)    13601 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/copies.py
--rw-r--r--   0 root         (0) root         (0)    22174 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/crt.py
--rw-r--r--   0 root         (0) root         (0)     2557 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/delete.py
--rw-r--r--   0 root         (0) root         (0)    28103 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/download.py
--rw-r--r--   0 root         (0) root         (0)     1065 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    21157 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/futures.py
--rw-r--r--   0 root         (0) root         (0)    28311 2022-05-31 18:37:19.000000 s3transfer-0.6.0/s3transfer/manager.py
--rw-r--r--   0 root         (0) root         (0)    36267 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/processpool.py
--rw-r--r--   0 root         (0) root         (0)     3569 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/subscribers.py
--rw-r--r--   0 root         (0) root         (0)    16191 2022-05-31 18:34:54.000000 s3transfer-0.6.0/s3transfer/tasks.py
--rw-r--r--   0 root         (0) root         (0)    30395 2022-05-31 18:37:19.000000 s3transfer-0.6.0/s3transfer/upload.py
--rw-r--r--   0 root         (0) root         (0)    27262 2022-05-31 18:37:19.000000 s3transfer-0.6.0/s3transfer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:37:19.371464 s3transfer-0.6.0/s3transfer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1491 2022-05-31 18:37:19.000000 s3transfer-0.6.0/s3transfer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1580 2022-05-31 18:37:19.000000 s3transfer-0.6.0/s3transfer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-31 18:37:19.000000 s3transfer-0.6.0/s3transfer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2022-05-31 18:37:19.000000 s3transfer-0.6.0/s3transfer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-05-31 18:37:19.000000 s3transfer-0.6.0/s3transfer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      229 2022-05-31 18:37:19.371464 s3transfer-0.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1398 2022-05-31 18:37:19.000000 s3transfer-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:37:19.371464 s3transfer-0.6.0/tests/
--rw-r--r--   0 root         (0) root         (0)    17082 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:37:19.371464 s3transfer-0.6.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)      561 2022-05-31 18:32:38.000000 s3transfer-0.6.0/tests/functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20068 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/functional/test_copy.py
--rw-r--r--   0 root         (0) root         (0)    10018 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/functional/test_crt.py
--rw-r--r--   0 root         (0) root         (0)     2588 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/functional/test_delete.py
--rw-r--r--   0 root         (0) root         (0)    19716 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/functional/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7324 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/functional/test_manager.py
--rw-r--r--   0 root         (0) root         (0)    10436 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/functional/test_processpool.py
--rw-r--r--   0 root         (0) root         (0)    24269 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/functional/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     1417 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/functional/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:37:19.371464 s3transfer-0.6.0/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     4396 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2989 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/integration/test_copy.py
--rw-r--r--   0 root         (0) root         (0)    12859 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/integration/test_crt.py
--rw-r--r--   0 root         (0) root         (0)     1130 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/integration/test_delete.py
--rw-r--r--   0 root         (0) root         (0)    10935 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/integration/test_download.py
--rw-r--r--   0 root         (0) root         (0)     5667 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/integration/test_processpool.py
--rw-r--r--   0 root         (0) root         (0)    11964 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/integration/test_s3transfer.py
--rw-r--r--   0 root         (0) root         (0)     7969 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/integration/test_upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-31 18:37:19.371464 s3transfer-0.6.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      561 2022-05-31 18:32:38.000000 s3transfer-0.6.0/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17445 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_bandwidth.py
--rw-r--r--   0 root         (0) root         (0)     3498 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_compat.py
--rw-r--r--   0 root         (0) root         (0)     6144 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_copies.py
--rw-r--r--   0 root         (0) root         (0)     6833 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_crt.py
--rw-r--r--   0 root         (0) root         (0)     2184 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_delete.py
--rw-r--r--   0 root         (0) root         (0)    35481 2022-05-31 18:37:19.000000 s3transfer-0.6.0/tests/unit/test_download.py
--rw-r--r--   0 root         (0) root         (0)    26415 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_futures.py
--rw-r--r--   0 root         (0) root         (0)     5757 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_manager.py
--rw-r--r--   0 root         (0) root         (0)    26153 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_processpool.py
--rw-r--r--   0 root         (0) root         (0)    28834 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_s3transfer.py
--rw-r--r--   0 root         (0) root         (0)     3197 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_subscribers.py
--rw-r--r--   0 root         (0) root         (0)    30724 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_tasks.py
--rw-r--r--   0 root         (0) root         (0)    26006 2022-05-31 18:34:54.000000 s3transfer-0.6.0/tests/unit/test_upload.py
--rw-r--r--   0 root         (0) root         (0)    42332 2022-05-31 18:37:19.000000 s3transfer-0.6.0/tests/unit/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:39:46.000000 s3transfer-0.6.1/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-05-04 19:35:46.000000 s3transfer-0.6.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-04 19:35:46.000000 s3transfer-0.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-04 19:35:46.000000 s3transfer-0.6.1/NOTICE.txt
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-04 19:39:46.000000 s3transfer-0.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-04 19:35:46.000000 s3transfer-0.6.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-04 19:35:46.000000 s3transfer-0.6.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:39:46.000000 s3transfer-0.6.1/s3transfer/
+-rw-r--r--   0 root         (0) root         (0)    29040 2023-05-04 19:39:46.000000 s3transfer-0.6.1/s3transfer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15635 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/bandwidth.py
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/compat.py
+-rw-r--r--   0 root         (0) root         (0)      910 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/constants.py
+-rw-r--r--   0 root         (0) root         (0)    14361 2023-05-04 19:39:46.000000 s3transfer-0.6.1/s3transfer/copies.py
+-rw-r--r--   0 root         (0) root         (0)    22174 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/crt.py
+-rw-r--r--   0 root         (0) root         (0)     2557 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/delete.py
+-rw-r--r--   0 root         (0) root         (0)    28103 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/download.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    21157 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/futures.py
+-rw-r--r--   0 root         (0) root         (0)    28311 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/manager.py
+-rw-r--r--   0 root         (0) root         (0)    36267 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/processpool.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/subscribers.py
+-rw-r--r--   0 root         (0) root         (0)    16191 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/tasks.py
+-rw-r--r--   0 root         (0) root         (0)    30395 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/upload.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2023-05-04 19:35:46.000000 s3transfer-0.6.1/s3transfer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:39:46.000000 s3transfer-0.6.1/s3transfer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-04 19:39:46.000000 s3transfer-0.6.1/s3transfer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-05-04 19:39:46.000000 s3transfer-0.6.1/s3transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 19:39:46.000000 s3transfer-0.6.1/s3transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-04 19:39:46.000000 s3transfer-0.6.1/s3transfer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-04 19:39:46.000000 s3transfer-0.6.1/s3transfer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-04 19:39:46.000000 s3transfer-0.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-05-04 19:39:46.000000 s3transfer-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:39:46.000000 s3transfer-0.6.1/tests/
+-rw-r--r--   0 root         (0) root         (0)    17082 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:39:46.000000 s3transfer-0.6.1/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)      561 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25787 2023-05-04 19:39:46.000000 s3transfer-0.6.1/tests/functional/test_copy.py
+-rw-r--r--   0 root         (0) root         (0)    10018 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/functional/test_crt.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/functional/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)    19716 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/functional/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7324 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/functional/test_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10436 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/functional/test_processpool.py
+-rw-r--r--   0 root         (0) root         (0)    24269 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/functional/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/functional/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:39:46.000000 s3transfer-0.6.1/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     4510 2023-05-04 19:39:46.000000 s3transfer-0.6.1/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/integration/test_copy.py
+-rw-r--r--   0 root         (0) root         (0)    12859 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/integration/test_crt.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/integration/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)    10935 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/integration/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     5667 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/integration/test_processpool.py
+-rw-r--r--   0 root         (0) root         (0)    11964 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/integration/test_s3transfer.py
+-rw-r--r--   0 root         (0) root         (0)     7969 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/integration/test_upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 19:39:46.000000 s3transfer-0.6.1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      561 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17445 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_bandwidth.py
+-rw-r--r--   0 root         (0) root         (0)     3498 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_compat.py
+-rw-r--r--   0 root         (0) root         (0)     7166 2023-05-04 19:39:46.000000 s3transfer-0.6.1/tests/unit/test_copies.py
+-rw-r--r--   0 root         (0) root         (0)     6833 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_crt.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)    35481 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_download.py
+-rw-r--r--   0 root         (0) root         (0)    26415 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_futures.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_manager.py
+-rw-r--r--   0 root         (0) root         (0)    26153 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_processpool.py
+-rw-r--r--   0 root         (0) root         (0)    28834 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_s3transfer.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_subscribers.py
+-rw-r--r--   0 root         (0) root         (0)    30724 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_tasks.py
+-rw-r--r--   0 root         (0) root         (0)    26006 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-05-04 19:35:46.000000 s3transfer-0.6.1/tests/unit/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `s3transfer-0.6.0/LICENSE.txt` & `s3transfer-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/PKG-INFO` & `s3transfer-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3transfer
-Version: 0.6.0
+Version: 0.6.1
 Summary: An Amazon S3 Transfer Manager
 Home-page: https://github.com/boto/s3transfer
 Author: Amazon Web Services
 Author-email: kyknapp1@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >= 3.7
 Provides-Extra: crt
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 =====================================================
 s3transfer - An Amazon S3 Transfer Manager for Python
```

### Comparing `s3transfer-0.6.0/README.rst` & `s3transfer-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/__init__.py` & `s3transfer-0.6.1/s3transfer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     ReadTimeoutError,
 )
 
 import s3transfer.compat
 from s3transfer.exceptions import RetriesExceededError, S3UploadFailedError
 
 __author__ = 'Amazon Web Services'
-__version__ = '0.6.0'
+__version__ = '0.6.1'
 
 
 class NullHandler(logging.Handler):
     def emit(self, record):
         pass
```

### Comparing `s3transfer-0.6.0/s3transfer/bandwidth.py` & `s3transfer-0.6.1/s3transfer/bandwidth.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/compat.py` & `s3transfer-0.6.1/s3transfer/compat.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/constants.py` & `s3transfer-0.6.1/s3transfer/constants.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/copies.py` & `s3transfer-0.6.1/s3transfer/copies.py`

 * *Files 15% similar despite different names*

```diff
@@ -216,28 +216,31 @@
             # callbacks.
             size = self._get_transfer_size(
                 part_size,
                 part_number - 1,
                 num_parts,
                 transfer_future.meta.size,
             )
+            # Get the checksum algorithm of the multipart request.
+            checksum_algorithm = call_args.extra_args.get("ChecksumAlgorithm")
             part_futures.append(
                 self._transfer_coordinator.submit(
                     request_executor,
                     CopyPartTask(
                         transfer_coordinator=self._transfer_coordinator,
                         main_kwargs={
                             'client': client,
                             'copy_source': call_args.copy_source,
                             'bucket': call_args.bucket,
                             'key': call_args.key,
                             'part_number': part_number,
                             'extra_args': extra_part_args,
                             'callbacks': progress_callbacks,
                             'size': size,
+                            'checksum_algorithm': checksum_algorithm,
                         },
                         pending_main_kwargs={
                             'upload_id': create_multipart_future
                         },
                     ),
                 )
             )
@@ -327,42 +330,53 @@
         bucket,
         key,
         upload_id,
         part_number,
         extra_args,
         callbacks,
         size,
+        checksum_algorithm=None,
     ):
         """
         :param client: The client to use when calling PutObject
         :param copy_source: The CopySource parameter to use
         :param bucket: The name of the bucket to upload to
         :param key: The name of the key to upload to
         :param upload_id: The id of the upload
         :param part_number: The number representing the part of the multipart
             upload
         :param extra_args: A dictionary of any extra arguments that may be
             used in the upload.
         :param callbacks: List of callbacks to call after copy part
         :param size: The size of the transfer. This value is passed into
             the callbacks
+        :param checksum_algorithm: The algorithm that was used to create the multipart
+            upload
 
         :rtype: dict
         :returns: A dictionary representing a part::
 
             {'Etag': etag_value, 'PartNumber': part_number}
 
             This value can be appended to a list to be used to complete
-            the multipart upload.
+            the multipart upload. If a checksum is in the response,
+            it will also be included.
         """
         response = client.upload_part_copy(
             CopySource=copy_source,
             Bucket=bucket,
             Key=key,
             UploadId=upload_id,
             PartNumber=part_number,
-            **extra_args
+            **extra_args,
         )
         for callback in callbacks:
             callback(bytes_transferred=size)
         etag = response['CopyPartResult']['ETag']
-        return {'ETag': etag, 'PartNumber': part_number}
+        part_metadata = {'ETag': etag, 'PartNumber': part_number}
+        if checksum_algorithm:
+            checksum_member = f'Checksum{checksum_algorithm.upper()}'
+            if checksum_member in response['CopyPartResult']:
+                part_metadata[checksum_member] = response['CopyPartResult'][
+                    checksum_member
+                ]
+        return part_metadata
```

### Comparing `s3transfer-0.6.0/s3transfer/crt.py` & `s3transfer-0.6.1/s3transfer/crt.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/delete.py` & `s3transfer-0.6.1/s3transfer/delete.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/download.py` & `s3transfer-0.6.1/s3transfer/download.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/exceptions.py` & `s3transfer-0.6.1/s3transfer/exceptions.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/futures.py` & `s3transfer-0.6.1/s3transfer/futures.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/manager.py` & `s3transfer-0.6.1/s3transfer/manager.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/processpool.py` & `s3transfer-0.6.1/s3transfer/processpool.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/subscribers.py` & `s3transfer-0.6.1/s3transfer/subscribers.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/tasks.py` & `s3transfer-0.6.1/s3transfer/tasks.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/upload.py` & `s3transfer-0.6.1/s3transfer/upload.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer/utils.py` & `s3transfer-0.6.1/s3transfer/utils.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/s3transfer.egg-info/PKG-INFO` & `s3transfer-0.6.1/s3transfer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3transfer
-Version: 0.6.0
+Version: 0.6.1
 Summary: An Amazon S3 Transfer Manager
 Home-page: https://github.com/boto/s3transfer
 Author: Amazon Web Services
 Author-email: kyknapp1@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >= 3.7
 Provides-Extra: crt
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 =====================================================
 s3transfer - An Amazon S3 Transfer Manager for Python
```

### Comparing `s3transfer-0.6.0/s3transfer.egg-info/SOURCES.txt` & `s3transfer-0.6.1/s3transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/setup.py` & `s3transfer-0.6.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,9 +41,10 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `s3transfer-0.6.0/tests/__init__.py` & `s3transfer-0.6.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/functional/__init__.py` & `s3transfer-0.6.1/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/functional/test_copy.py` & `s3transfer-0.6.1/tests/functional/test_copy.py`

 * *Files 16% similar despite different names*

```diff
@@ -196,14 +196,37 @@
             expected_copy_params=expected_copy_object
         )
 
         future = self.manager.copy(**self.create_call_kwargs())
         future.result()
         self.stubber.assert_no_pending_responses()
 
+    def test_copy_with_checksum(self):
+        self.extra_args['ChecksumAlgorithm'] = 'crc32'
+        expected_head_params = {
+            'Bucket': 'mysourcebucket',
+            'Key': 'mysourcekey',
+        }
+        expected_copy_object = {
+            'Bucket': self.bucket,
+            'Key': self.key,
+            'CopySource': self.copy_source,
+            'ChecksumAlgorithm': 'crc32',
+        }
+        self.add_head_object_response(expected_params=expected_head_params)
+        self.add_successful_copy_responses(
+            expected_copy_params=expected_copy_object
+        )
+
+        call_kwargs = self.create_call_kwargs()
+        call_kwargs['extra_args'] = self.extra_args
+        future = self.manager.copy(**call_kwargs)
+        future.result()
+        self.stubber.assert_no_pending_responses()
+
     def test_copy_with_extra_args(self):
         self.extra_args['MetadataDirective'] = 'REPLACE'
 
         expected_head_params = {
             'Bucket': 'mysourcebucket',
             'Key': 'mysourcekey',
         }
@@ -298,24 +321,25 @@
         super().setUp()
         self.config = TransferConfig(
             max_request_concurrency=1,
             multipart_threshold=1,
             multipart_chunksize=4,
         )
         self._manager = TransferManager(self.client, self.config)
+        self.multipart_id = 'my-upload-id'
 
     def create_stubbed_responses(self):
         return [
             {
                 'method': 'head_object',
                 'service_response': {'ContentLength': len(self.content)},
             },
             {
                 'method': 'create_multipart_upload',
-                'service_response': {'UploadId': 'my-upload-id'},
+                'service_response': {'UploadId': self.multipart_id},
             },
             {
                 'method': 'upload_part_copy',
                 'service_response': {'CopyPartResult': {'ETag': 'etag-1'}},
             },
             {
                 'method': 'upload_part_copy',
@@ -324,29 +348,105 @@
             {
                 'method': 'upload_part_copy',
                 'service_response': {'CopyPartResult': {'ETag': 'etag-3'}},
             },
             {'method': 'complete_multipart_upload', 'service_response': {}},
         ]
 
+    def add_get_head_response_with_default_expected_params(
+        self, extra_expected_params=None
+    ):
+        expected_params = {
+            'Bucket': 'mysourcebucket',
+            'Key': 'mysourcekey',
+        }
+        if extra_expected_params:
+            expected_params.update(extra_expected_params)
+        response = self.create_stubbed_responses()[0]
+        response['expected_params'] = expected_params
+        self.stubber.add_response(**response)
+
+    def add_create_multipart_response_with_default_expected_params(
+        self, extra_expected_params=None
+    ):
+        expected_params = {'Bucket': self.bucket, 'Key': self.key}
+        if extra_expected_params:
+            expected_params.update(extra_expected_params)
+        response = self.create_stubbed_responses()[1]
+        response['expected_params'] = expected_params
+        self.stubber.add_response(**response)
+
+    def add_upload_part_copy_responses_with_default_expected_params(
+        self, extra_expected_params=None
+    ):
+        ranges = [
+            'bytes=0-5242879',
+            'bytes=5242880-10485759',
+            'bytes=10485760-13107199',
+        ]
+        upload_part_responses = self.create_stubbed_responses()[2:-1]
+        for i, range_val in enumerate(ranges):
+            upload_part_response = upload_part_responses[i]
+            expected_params = {
+                'Bucket': self.bucket,
+                'Key': self.key,
+                'CopySource': self.copy_source,
+                'UploadId': self.multipart_id,
+                'PartNumber': i + 1,
+                'CopySourceRange': range_val,
+            }
+            if extra_expected_params:
+                if 'ChecksumAlgorithm' in extra_expected_params:
+                    name = extra_expected_params['ChecksumAlgorithm']
+                    checksum_member = 'Checksum%s' % name.upper()
+                    response = upload_part_response['service_response']
+                    response['CopyPartResult'][checksum_member] = 'sum%s==' % (
+                        i + 1
+                    )
+                else:
+                    expected_params.update(extra_expected_params)
+
+            upload_part_response['expected_params'] = expected_params
+            self.stubber.add_response(**upload_part_response)
+
+    def add_complete_multipart_response_with_default_expected_params(
+        self, extra_expected_params=None
+    ):
+        expected_params = {
+            'Bucket': self.bucket,
+            'Key': self.key,
+            'UploadId': self.multipart_id,
+            'MultipartUpload': {
+                'Parts': [
+                    {'ETag': 'etag-1', 'PartNumber': 1},
+                    {'ETag': 'etag-2', 'PartNumber': 2},
+                    {'ETag': 'etag-3', 'PartNumber': 3},
+                ]
+            },
+        }
+        if extra_expected_params:
+            expected_params.update(extra_expected_params)
+
+        response = self.create_stubbed_responses()[-1]
+        response['expected_params'] = expected_params
+        self.stubber.add_response(**response)
+
     def create_expected_progress_callback_info(self):
         # Note that last read is from the empty sentinel indicating
         # that the stream is done.
         return [
             {'bytes_transferred': MIN_UPLOAD_CHUNKSIZE},
             {'bytes_transferred': MIN_UPLOAD_CHUNKSIZE},
             {'bytes_transferred': self.half_chunksize},
         ]
 
     def add_create_multipart_upload_response(self):
         self.stubber.add_response(**self.create_stubbed_responses()[1])
 
     def _get_expected_params(self):
-        upload_id = 'my-upload-id'
-
         # Add expected parameters to the head object
         expected_head_params = {
             'Bucket': 'mysourcebucket',
             'Key': 'mysourcekey',
         }
 
         # Add expected parameters for the create multipart
@@ -364,25 +464,25 @@
         ]
         for i, range_val in enumerate(ranges):
             expected_copy_params.append(
                 {
                     'Bucket': self.bucket,
                     'Key': self.key,
                     'CopySource': self.copy_source,
-                    'UploadId': upload_id,
+                    'UploadId': self.multipart_id,
                     'PartNumber': i + 1,
                     'CopySourceRange': range_val,
                 }
             )
 
         # Add expected parameters for the complete multipart
         expected_complete_mpu_params = {
             'Bucket': self.bucket,
             'Key': self.key,
-            'UploadId': upload_id,
+            'UploadId': self.multipart_id,
             'MultipartUpload': {
                 'Parts': [
                     {'ETag': 'etag-1', 'PartNumber': 1},
                     {'ETag': 'etag-2', 'PartNumber': 2},
                     {'ETag': 'etag-3', 'PartNumber': 3},
                 ]
             },
@@ -437,14 +537,62 @@
 
         call_kwargs = self.create_call_kwargs()
         call_kwargs['extra_args'] = self.extra_args
         future = self.manager.copy(**call_kwargs)
         future.result()
         self.stubber.assert_no_pending_responses()
 
+    def test_copy_passes_checksums(self):
+        # This extra argument should be added to the head object,
+        # the create multipart upload, and upload part copy.
+        self.extra_args['ChecksumAlgorithm'] = 'sha256'
+
+        self.add_get_head_response_with_default_expected_params()
+
+        # ChecksumAlgorithm should be passed on the create_multipart call
+        self.add_create_multipart_response_with_default_expected_params(
+            self.extra_args,
+        )
+
+        # ChecksumAlgorithm should be passed to the upload_part_copy calls
+        self.add_upload_part_copy_responses_with_default_expected_params(
+            self.extra_args,
+        )
+
+        # The checksums should be used in the complete call like etags
+        self.add_complete_multipart_response_with_default_expected_params(
+            extra_expected_params={
+                'MultipartUpload': {
+                    'Parts': [
+                        {
+                            'ETag': 'etag-1',
+                            'PartNumber': 1,
+                            'ChecksumSHA256': 'sum1==',
+                        },
+                        {
+                            'ETag': 'etag-2',
+                            'PartNumber': 2,
+                            'ChecksumSHA256': 'sum2==',
+                        },
+                        {
+                            'ETag': 'etag-3',
+                            'PartNumber': 3,
+                            'ChecksumSHA256': 'sum3==',
+                        },
+                    ]
+                }
+            }
+        )
+
+        call_kwargs = self.create_call_kwargs()
+        call_kwargs['extra_args'] = self.extra_args
+        future = self.manager.copy(**call_kwargs)
+        future.result()
+        self.stubber.assert_no_pending_responses()
+
     def test_copy_blacklists_args_to_create_multipart(self):
         # This argument can never be used for multipart uploads
         self.extra_args['MetadataDirective'] = 'COPY'
 
         head_params, add_copy_kwargs = self._get_expected_params()
         self.add_head_object_response(expected_params=head_params)
         self.add_successful_copy_responses(**add_copy_kwargs)
@@ -524,15 +672,15 @@
         # Add the abort multipart to ensure it gets cleaned up on failure
         self.stubber.add_response(
             'abort_multipart_upload',
             service_response={},
             expected_params={
                 'Bucket': self.bucket,
                 'Key': self.key,
-                'UploadId': 'my-upload-id',
+                'UploadId': self.multipart_id,
             },
         )
 
         future = self.manager.copy(**self.create_call_kwargs())
         with self.assertRaisesRegex(ClientError, 'ArbitraryFailure'):
             future.result()
         self.stubber.assert_no_pending_responses()
```

### Comparing `s3transfer-0.6.0/tests/functional/test_crt.py` & `s3transfer-0.6.1/tests/functional/test_crt.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/functional/test_delete.py` & `s3transfer-0.6.1/tests/functional/test_delete.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/functional/test_download.py` & `s3transfer-0.6.1/tests/functional/test_download.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/functional/test_manager.py` & `s3transfer-0.6.1/tests/functional/test_manager.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/functional/test_processpool.py` & `s3transfer-0.6.1/tests/functional/test_processpool.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/functional/test_upload.py` & `s3transfer-0.6.1/tests/functional/test_upload.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/functional/test_utils.py` & `s3transfer-0.6.1/tests/functional/test_utils.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/integration/__init__.py` & `s3transfer-0.6.1/tests/integration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         cls.region = 'us-west-2'
         cls.session = botocore.session.get_session()
         cls.client = cls.session.create_client('s3', cls.region)
         cls.bucket_name = random_bucket_name()
         cls.client.create_bucket(
             Bucket=cls.bucket_name,
             CreateBucketConfiguration={'LocationConstraint': cls.region},
+            ObjectOwnership='ObjectWriter',
         )
+        cls.client.delete_public_access_block(Bucket=cls.bucket_name)
 
     def setUp(self):
         self.files = FileCreator()
 
     def tearDown(self):
         self.files.remove_all()
```

### Comparing `s3transfer-0.6.0/tests/integration/test_copy.py` & `s3transfer-0.6.1/tests/integration/test_copy.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/integration/test_crt.py` & `s3transfer-0.6.1/tests/integration/test_crt.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/integration/test_delete.py` & `s3transfer-0.6.1/tests/integration/test_delete.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/integration/test_download.py` & `s3transfer-0.6.1/tests/integration/test_download.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/integration/test_processpool.py` & `s3transfer-0.6.1/tests/integration/test_processpool.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/integration/test_s3transfer.py` & `s3transfer-0.6.1/tests/integration/test_s3transfer.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/integration/test_upload.py` & `s3transfer-0.6.1/tests/integration/test_upload.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/__init__.py` & `s3transfer-0.6.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_bandwidth.py` & `s3transfer-0.6.1/tests/unit/test_bandwidth.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_compat.py` & `s3transfer-0.6.1/tests/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_copies.py` & `s3transfer-0.6.1/tests/unit/test_copies.py`

 * *Files 12% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     def setUp(self):
         super().setUp()
         self.copy_source_range = 'bytes=5-9'
         self.extra_args['CopySourceRange'] = self.copy_source_range
         self.upload_id = 'myuploadid'
         self.part_number = 1
         self.result_etag = 'my-etag'
+        self.checksum_sha1 = 'my-checksum_sha1'
 
     def get_copy_task(self, **kwargs):
         default_kwargs = {
             'client': self.client,
             'copy_source': self.copy_source,
             'bucket': self.bucket,
             'key': self.key,
@@ -129,14 +130,43 @@
         )
         task = self.get_copy_task()
         self.assertEqual(
             task(), {'PartNumber': self.part_number, 'ETag': self.result_etag}
         )
         self.stubber.assert_no_pending_responses()
 
+    def test_main_with_checksum(self):
+        self.stubber.add_response(
+            'upload_part_copy',
+            service_response={
+                'CopyPartResult': {
+                    'ETag': self.result_etag,
+                    'ChecksumSHA1': self.checksum_sha1,
+                }
+            },
+            expected_params={
+                'Bucket': self.bucket,
+                'Key': self.key,
+                'CopySource': self.copy_source,
+                'UploadId': self.upload_id,
+                'PartNumber': self.part_number,
+                'CopySourceRange': self.copy_source_range,
+            },
+        )
+        task = self.get_copy_task(checksum_algorithm="sha1")
+        self.assertEqual(
+            task(),
+            {
+                'PartNumber': self.part_number,
+                'ETag': self.result_etag,
+                'ChecksumSHA1': self.checksum_sha1,
+            },
+        )
+        self.stubber.assert_no_pending_responses()
+
     def test_extra_args(self):
         self.extra_args['RequestPayer'] = 'requester'
         self.stubber.add_response(
             'upload_part_copy',
             service_response={'CopyPartResult': {'ETag': self.result_etag}},
             expected_params={
                 'Bucket': self.bucket,
```

### Comparing `s3transfer-0.6.0/tests/unit/test_crt.py` & `s3transfer-0.6.1/tests/unit/test_crt.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_delete.py` & `s3transfer-0.6.1/tests/unit/test_delete.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_download.py` & `s3transfer-0.6.1/tests/unit/test_download.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_futures.py` & `s3transfer-0.6.1/tests/unit/test_futures.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_manager.py` & `s3transfer-0.6.1/tests/unit/test_manager.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_processpool.py` & `s3transfer-0.6.1/tests/unit/test_processpool.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_s3transfer.py` & `s3transfer-0.6.1/tests/unit/test_s3transfer.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_subscribers.py` & `s3transfer-0.6.1/tests/unit/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_tasks.py` & `s3transfer-0.6.1/tests/unit/test_tasks.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_upload.py` & `s3transfer-0.6.1/tests/unit/test_upload.py`

 * *Files identical despite different names*

### Comparing `s3transfer-0.6.0/tests/unit/test_utils.py` & `s3transfer-0.6.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

