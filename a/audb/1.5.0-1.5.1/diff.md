# Comparing `tmp/audb-1.5.0.tar.gz` & `tmp/audb-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audb-1.5.0.tar", last modified: Thu Apr 27 13:01:57 2023, max compression
+gzip compressed data, was "audb-1.5.1.tar", last modified: Thu May  4 08:11:49 2023, max compression
```

## Comparing `audb-1.5.0.tar` & `audb-1.5.1.tar`

### file list

```diff
@@ -1,90 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.085238 audb-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.073238 audb-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.077238 audb-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-27 13:01:43.000000 audb-1.5.0/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 13:01:43.000000 audb-1.5.0/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-27 13:01:43.000000 audb-1.5.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-27 13:01:43.000000 audb-1.5.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 13:01:43.000000 audb-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 13:01:43.000000 audb-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-27 13:01:43.000000 audb-1.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-27 13:01:43.000000 audb-1.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 13:01:43.000000 audb-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-04-27 13:01:57.085238 audb-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-27 13:01:43.000000 audb-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.077238 audb-1.5.0/audb/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-27 13:01:43.000000 audb-1.5.0/audb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/audb/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/define.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/audb/core/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/etc/audb.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/flavor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    49096 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/load_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-27 13:01:43.000000 audb-1.5.0/audb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/audb/info/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-27 13:01:43.000000 audb-1.5.0/audb/info/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.077238 audb-1.5.0/audb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-04-27 13:01:56.000000 audb-1.5.0/audb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-27 13:01:57.000000 audb-1.5.0/audb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:01:56.000000 audb-1.5.0/audb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 13:01:56.000000 audb-1.5.0/audb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 13:01:56.000000 audb-1.5.0/audb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.073238 audb-1.5.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 13:01:43.000000 audb-1.5.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-27 13:01:43.000000 audb-1.5.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 13:01:43.000000 audb-1.5.0/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 13:01:43.000000 audb-1.5.0/docs/api-src/audb.info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-27 13:01:43.000000 audb-1.5.0/docs/api-src/audb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-27 13:01:43.000000 audb-1.5.0/docs/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-27 13:01:43.000000 audb-1.5.0/docs/caching.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 13:01:43.000000 audb-1.5.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-27 13:01:43.000000 audb-1.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-27 13:01:43.000000 audb-1.5.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 13:01:43.000000 audb-1.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-27 13:01:43.000000 audb-1.5.0/docs/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 13:01:43.000000 audb-1.5.0/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-27 13:01:43.000000 audb-1.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-27 13:01:43.000000 audb-1.5.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-04-27 13:01:43.000000 audb-1.5.0/docs/load.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-27 13:01:43.000000 audb-1.5.0/docs/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.081238 audb-1.5.0/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-27 13:01:43.000000 audb-1.5.0/docs/pics/load.dot
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 13:01:43.000000 audb-1.5.0/docs/pics/publish.dot
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-27 13:01:43.000000 audb-1.5.0/docs/publish.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-27 13:01:43.000000 audb-1.5.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 13:01:43.000000 audb-1.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 13:01:43.000000 audb-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-27 13:01:57.085238 audb-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 13:01:43.000000 audb-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:01:57.085238 audb-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-27 13:01:43.000000 audb-1.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 13:01:43.000000 audb-1.5.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_flavor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    22469 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_load_on_demand.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_lock_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    40591 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-27 13:01:43.000000 audb-1.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.821748 audb-1.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.809748 audb-1.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.809748 audb-1.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-04 08:11:28.000000 audb-1.5.1/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-04 08:11:28.000000 audb-1.5.1/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-04 08:11:28.000000 audb-1.5.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-04 08:11:28.000000 audb-1.5.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-04 08:11:28.000000 audb-1.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 08:11:28.000000 audb-1.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-05-04 08:11:28.000000 audb-1.5.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-04 08:11:28.000000 audb-1.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-04 08:11:28.000000 audb-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-05-04 08:11:49.821748 audb-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 08:11:28.000000 audb-1.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.809748 audb-1.5.1/audb/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-04 08:11:28.000000 audb-1.5.1/audb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.813748 audb-1.5.1/audb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.813748 audb-1.5.1/audb/core/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/etc/audb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/flavor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49197 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/load_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26205 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-04 08:11:28.000000 audb-1.5.1/audb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.813748 audb-1.5.1/audb/info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-04 08:11:28.000000 audb-1.5.1/audb/info/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.809748 audb-1.5.1/audb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-05-04 08:11:49.000000 audb-1.5.1/audb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-04 08:11:49.000000 audb-1.5.1/audb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:11:49.000000 audb-1.5.1/audb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 08:11:49.000000 audb-1.5.1/audb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 08:11:49.000000 audb-1.5.1/audb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.817748 audb-1.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.809748 audb-1.5.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.817748 audb-1.5.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 08:11:28.000000 audb-1.5.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-04 08:11:28.000000 audb-1.5.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 08:11:28.000000 audb-1.5.1/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.817748 audb-1.5.1/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-04 08:11:28.000000 audb-1.5.1/docs/api-src/audb.info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 08:11:28.000000 audb-1.5.1/docs/api-src/audb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-04 08:11:28.000000 audb-1.5.1/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-04 08:11:28.000000 audb-1.5.1/docs/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 08:11:28.000000 audb-1.5.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-04 08:11:28.000000 audb-1.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 08:11:28.000000 audb-1.5.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 08:11:28.000000 audb-1.5.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-04 08:11:28.000000 audb-1.5.1/docs/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 08:11:28.000000 audb-1.5.1/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-04 08:11:28.000000 audb-1.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-04 08:11:28.000000 audb-1.5.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-04 08:11:28.000000 audb-1.5.1/docs/load.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-04 08:11:28.000000 audb-1.5.1/docs/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.817748 audb-1.5.1/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-04 08:11:28.000000 audb-1.5.1/docs/pics/load.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-04 08:11:28.000000 audb-1.5.1/docs/pics/publish.dot
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-04 08:11:28.000000 audb-1.5.1/docs/publish.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-04 08:11:28.000000 audb-1.5.1/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 08:11:28.000000 audb-1.5.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 08:11:28.000000 audb-1.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-04 08:11:49.821748 audb-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-04 08:11:28.000000 audb-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:11:49.817748 audb-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-04 08:11:28.000000 audb-1.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 08:11:28.000000 audb-1.5.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22469 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_load_on_demand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_lock_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40560 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-04 08:11:28.000000 audb-1.5.1/tests/test_remove.py
```

### Comparing `audb-1.5.0/.github/workflows/doc.yml` & `audb-1.5.1/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/.github/workflows/flake8.yml` & `audb-1.5.1/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/.github/workflows/publish.yml` & `audb-1.5.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/.github/workflows/test.yml` & `audb-1.5.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/CHANGELOG.rst` & `audb-1.5.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.5.1 (2023-05-04)
+--------------------------
+
+* Changed: require ``audeer>=1.20.0``
+* Fixed: ``audb.load()``,
+  ``audb.load_to()``,
+  ``audb.load_media()``,
+  and ``audb.remove_media()``
+  were failing with ``audeer==1.20.0``
+  under Windows
+
+
 Version 1.5.0 (2023-04-27)
 --------------------------
 
 * Added: support loading and publishing
   of database attachments
   (``audformat.Attachment``)
 * Added: ``audb.load_attachment()``
```

### Comparing `audb-1.5.0/CONTRIBUTING.rst` & `audb-1.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/LICENSE` & `audb-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/PKG-INFO` & `audb-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audb
-Version: 1.5.0
+Version: 1.5.1
 Summary: Load and publish databases in audformat
 Home-page: https://audeering.github.io/audb/
 Author: Johannes Wagner, Hagen Wierstorf
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audb/
 Description: ====
@@ -59,14 +59,26 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.5.1 (2023-05-04)
+        --------------------------
+        
+        * Changed: require ``audeer>=1.20.0``
+        * Fixed: ``audb.load()``,
+          ``audb.load_to()``,
+          ``audb.load_media()``,
+          and ``audb.remove_media()``
+          were failing with ``audeer==1.20.0``
+          under Windows
+        
+        
         Version 1.5.0 (2023-04-27)
         --------------------------
         
         * Added: support loading and publishing
           of database attachments
           (``audformat.Attachment``)
         * Added: ``audb.load_attachment()``
```

### Comparing `audb-1.5.0/README.rst` & `audb-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/__init__.py` & `audb-1.5.1/audb/__init__.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/core/api.py` & `audb-1.5.1/audb/core/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,14 +509,21 @@
                     ):
 
                         files_in_archive = backend.get_archive(
                             remote_archive,
                             db_root,
                             version,
                         )
+
+                        if os.name == 'nt':  # pragma: no cover
+                            files_in_archive = [
+                                file.replace(os.path.sep, '/')
+                                for file in files_in_archive
+                            ]
+
                         # skip if file was already deleted
                         if file in files_in_archive:
                             os.remove(os.path.join(db_root, file))
                             files_in_archive.remove(file)
                             backend.put_archive(
                                 db_root,
                                 files_in_archive,
```

### Comparing `audb-1.5.0/audb/core/cache.py` & `audb-1.5.1/audb/core/cache.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/core/config.py` & `audb-1.5.1/audb/core/config.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/core/conftest.py` & `audb-1.5.1/audb/core/conftest.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/core/define.py` & `audb-1.5.1/audb/core/define.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/core/dependencies.py` & `audb-1.5.1/audb/core/dependencies.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/core/flavor.py` & `audb-1.5.1/audb/core/flavor.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/core/info.py` & `audb-1.5.1/audb/core/info.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/core/load.py` & `audb-1.5.1/audb/core/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,16 @@
         files = backend.get_archive(
             archive,
             db_root_tmp,
             version,
             tmp_root=db_root_tmp,
         )
         for file in files:
+            if os.name == 'nt':  # pragma: no cover
+                file = file.replace(os.sep, '/')
             if flavor is not None:
                 bit_depth = deps.bit_depth(file)
                 channels = deps.channels(file)
                 sampling_rate = deps.sampling_rate(file)
                 src_path = os.path.join(db_root_tmp, file)
                 file = flavor.destination(file)
                 dst_path = os.path.join(db_root_tmp, file)
```

### Comparing `audb-1.5.0/audb/core/load_to.py` & `audb-1.5.1/audb/core/load_to.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         if only_metadata:
             files = deps.tables
         else:
             files = deps.attachments + deps.files
         for file in files:
             full_file = os.path.join(db_root, file)
             if os.path.exists(full_file):
-                checksum = utils.md5(full_file)
+                checksum = audeer.md5(full_file)
                 if checksum != deps.checksum(file):
                     if os.path.isdir(full_file):
                         audeer.rmdir(full_file)
                     else:
                         os.remove(full_file)
 
     # load database header without tables from backend
```

### Comparing `audb-1.5.0/audb/core/lock.py` & `audb-1.5.1/audb/core/lock.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb/core/publish.py` & `audb-1.5.1/audb/core/publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import audbackend
 import audeer
 import audformat
 import audiofile
 
 from audb.core import define
-from audb.core import utils
 from audb.core.api import dependencies
 from audb.core.dependencies import Dependencies
 from audb.core.repository import Repository
 
 
 def _check_for_duplicates(
         db: audformat.Database,
@@ -140,15 +139,15 @@
                 #
                 # Attachment is not in deps,
                 # but its path does not exist on disk either.
                 # We call its `files` property
                 # which raises a FileNotFoundError in this case
                 db.attachments[attachment_id].files
         else:
-            checksum = utils.md5(audeer.path(db_root, path))
+            checksum = audeer.md5(audeer.path(db_root, path))
             if (
                     path not in deps
                     or checksum != deps.checksum(path)
             ):
                 deps._add_attachment(
                     file=path,
                     version=version,
@@ -192,29 +191,29 @@
             # assert lowercase file extensions
             ext = audeer.file_extension(file)
             if ext.lower() != ext:
                 raise RuntimeError(
                     "The file extension of a media file must be lowercase, "
                     f"but '{file}' includes at least one uppercase letter."
                 )
-            checksum = audbackend.md5(path)
+            checksum = audeer.md5(path)
             if file in archives:
                 archive = archives[file]
             else:
                 archive = audeer.uid(from_string=file.replace('\\', '/'))
             values = _media_values(
                 db_root,
                 file,
                 version,
                 archive,
                 checksum,
             )
             add_media.append(values)
         elif not deps.removed(file):
-            checksum = audbackend.md5(path)
+            checksum = audeer.md5(path)
             if checksum != deps.checksum(file):
                 archive = deps.archive(file)
                 values = _media_values(
                     db_root,
                     file,
                     version,
                     archive,
@@ -262,15 +261,15 @@
     tables = []
     for table in audeer.progress_bar(
             list(db),
             desc='Find tables',
             disable=not verbose,
     ):
         file = f'db.{table}.csv'
-        checksum = audbackend.md5(os.path.join(db_root, file))
+        checksum = audeer.md5(os.path.join(db_root, file))
         if file not in deps or checksum != deps.checksum(file):
             deps._add_meta(file, version, table, checksum)
             tables.append(table)
 
     return tables
 
 
@@ -661,15 +660,15 @@
             previous_deps = dependencies(
                 db.name,
                 version=previous_version,
                 cache_root=cache_root,
                 verbose=verbose,
             )
             previous_deps.save(previous_deps_path)
-            if audbackend.md5(deps_path) != audbackend.md5(previous_deps_path):
+            if audeer.md5(deps_path) != audeer.md5(previous_deps_path):
                 raise RuntimeError(
                     f"You want to depend on '{previous_version}' "
                     f"of {db.name}, "
                     f"but the MD5 sum of your "
                     f"'{define.DEPENDENCIES_FILE}' file "
                     f"in {db_root} "
                     f"does not match the MD5 sum of the corresponding file "
```

### Comparing `audb-1.5.0/audb/info/__init__.py` & `audb-1.5.1/audb/info/__init__.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/audb.egg-info/PKG-INFO` & `audb-1.5.1/audb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audb
-Version: 1.5.0
+Version: 1.5.1
 Summary: Load and publish databases in audformat
 Home-page: https://audeering.github.io/audb/
 Author: Johannes Wagner, Hagen Wierstorf
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audb/
 Description: ====
@@ -59,14 +59,26 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.5.1 (2023-05-04)
+        --------------------------
+        
+        * Changed: require ``audeer>=1.20.0``
+        * Fixed: ``audb.load()``,
+          ``audb.load_to()``,
+          ``audb.load_media()``,
+          and ``audb.remove_media()``
+          were failing with ``audeer==1.20.0``
+          under Windows
+        
+        
         Version 1.5.0 (2023-04-27)
         --------------------------
         
         * Added: support loading and publishing
           of database attachments
           (``audformat.Attachment``)
         * Added: ``audb.load_attachment()``
```

### Comparing `audb-1.5.0/audb.egg-info/SOURCES.txt` & `audb-1.5.1/audb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,9 +67,8 @@
 tests/test_flavor.py
 tests/test_info.py
 tests/test_load.py
 tests/test_load_on_demand.py
 tests/test_lock.py
 tests/test_lock_db.py
 tests/test_publish.py
-tests/test_remove.py
-tests/test_utils.py
+tests/test_remove.py
```

### Comparing `audb-1.5.0/docs/_templates/autosummary/class.rst` & `audb-1.5.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/authentication.rst` & `audb-1.5.1/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/caching.rst` & `audb-1.5.1/docs/caching.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/conf.py` & `audb-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/configuration.rst` & `audb-1.5.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/dependencies.rst` & `audb-1.5.1/docs/dependencies.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/index.rst` & `audb-1.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/install.rst` & `audb-1.5.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/load.rst` & `audb-1.5.1/docs/load.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/overview.rst` & `audb-1.5.1/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/pics/load.dot` & `audb-1.5.1/docs/pics/load.dot`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/pics/publish.dot` & `audb-1.5.1/docs/pics/publish.dot`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/publish.rst` & `audb-1.5.1/docs/publish.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/docs/quickstart.rst` & `audb-1.5.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/setup.cfg` & `audb-1.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
 install_requires = 
 	audbackend >=0.3.17, <1.0.0
-	audeer >=1.18.0
+	audeer >=1.20.0
 	audformat >=0.16.1
 	audiofile >=1.0.0
 	audobject >=0.5.0
 	audresample >=0.1.6
 	filelock
 	oyaml
 python_requires = >=3.8
```

### Comparing `audb-1.5.0/tests/conftest.py` & `audb-1.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_api.py` & `audb-1.5.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_cache.py` & `audb-1.5.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_config.py` & `audb-1.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_convert.py` & `audb-1.5.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_dependencies.py` & `audb-1.5.1/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_filter.py` & `audb-1.5.1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_flavor.py` & `audb-1.5.1/tests/test_flavor.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_info.py` & `audb-1.5.1/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_load.py` & `audb-1.5.1/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_load_on_demand.py` & `audb-1.5.1/tests/test_load_on_demand.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_lock.py` & `audb-1.5.1/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_lock_db.py` & `audb-1.5.1/tests/test_lock_db.py`

 * *Files identical despite different names*

### Comparing `audb-1.5.0/tests/test_publish.py` & `audb-1.5.1/tests/test_publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import re
 import shutil
 
 import numpy as np
 import pandas as pd
 import pytest
 
-import audbackend
 import audeer
 import audformat.testing
 import audiofile
 
 import audb
 
 
@@ -425,15 +424,15 @@
         - number_of_media_archives
     )
     for archive in set(archives.values()):
         assert archive in deps.archives
 
     # Check checksums of attachment files
     for path in deps.attachments:
-        expected_checksum = audb.core.utils.md5(audeer.path(db.root, path))
+        expected_checksum = audeer.md5(audeer.path(db.root, path))
         assert deps.checksum(path) == expected_checksum
 
     db = audb.load(
         DB_NAME,
         version=version,
         full_path=False,
         num_workers=pytest.NUM_WORKERS,
@@ -456,15 +455,15 @@
     assert df[df.index == DB_NAME]['version'][0] == latest_version
 
     for file in db.files:
         name = archives[file] if file in archives else file
         file_path = backend.join(db.name, 'media', name)
         backend.exists(file_path, version)
         path = os.path.join(dbs[version], file)
-        assert deps.checksum(file) == audbackend.md5(path)
+        assert deps.checksum(file) == audeer.md5(path)
         if deps.format(file) in [
             audb.core.define.Format.WAV,
             audb.core.define.Format.FLAC,
         ]:
             assert deps.bit_depth(file) == audiofile.bit_depth(path)
             assert deps.channels(file) == audiofile.channels(path)
             assert deps.duration(file) == audiofile.duration(path)
```

### Comparing `audb-1.5.0/tests/test_remove.py` & `audb-1.5.1/tests/test_remove.py`

 * *Files identical despite different names*

