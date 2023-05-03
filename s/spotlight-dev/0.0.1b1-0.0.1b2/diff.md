# Comparing `tmp/spotlight-dev-0.0.1b1.tar.gz` & `tmp/spotlight-dev-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-dev-0.0.1b1.tar", last modified: Wed Apr 26 18:04:38 2023, max compression
+gzip compressed data, was "spotlight-dev-0.0.1b2.tar", last modified: Wed May  3 23:10:20 2023, max compression
```

## Comparing `spotlight-dev-0.0.1b1.tar` & `spotlight-dev-0.0.1b2.tar`

### file list

```diff
@@ -1,113 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.586662 spotlight-dev-0.0.1b1/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-04-26 18:04:38.586662 spotlight-dev-0.0.1b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 18:04:38.586662 spotlight-dev-0.0.1b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.542659 spotlight-dev-0.0.1b1/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.542659 spotlight-dev-0.0.1b1/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.544659 spotlight-dev-0.0.1b1/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.546659 spotlight-dev-0.0.1b1/spotlight/api/job/
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2975 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2629 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.549660 spotlight-dev-0.0.1b1/spotlight/api/job/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/job/view/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.551660 spotlight-dev-0.0.1b1/spotlight/api/rule/
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4007 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3565 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.554660 spotlight-dev-0.0.1b1/spotlight/api/tag/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4659 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/model.py
--rw-rw-rw-   0 root         (0) root         (0)     4134 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.557660 spotlight-dev-0.0.1b1/spotlight/api/tag/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/api/tag/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.558660 spotlight-dev-0.0.1b1/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.563661 spotlight-dev-0.0.1b1/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.564661 spotlight-dev-0.0.1b1/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.564661 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.567661 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.570661 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.571661 spotlight-dev-0.0.1b1/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.573661 spotlight-dev-0.0.1b1/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.573661 spotlight-dev-0.0.1b1/spotlight/core/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)     5930 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.574662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.576662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1506 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.578662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/sql_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.579662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.581662 spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/asynchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/synchronously.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.583662 spotlight-dev-0.0.1b1/spotlight/pandas/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/pandas/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/pandas/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-04-26 18:04:25.000000 spotlight-dev-0.0.1b1/spotlight/pandas/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 18:04:38.585662 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3252 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-26 18:04:38.000000 spotlight-dev-0.0.1b1/spotlight_dev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.561716 spotlight-dev-0.0.1b2/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-03 23:10:20.561716 spotlight-dev-0.0.1b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 23:10:20.562716 spotlight-dev-0.0.1b2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.537714 spotlight-dev-0.0.1b2/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.537714 spotlight-dev-0.0.1b2/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.538714 spotlight-dev-0.0.1b2/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.539714 spotlight-dev-0.0.1b2/spotlight/api/job/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.541714 spotlight-dev-0.0.1b2/spotlight/api/job/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.542714 spotlight-dev-0.0.1b2/spotlight/api/organization/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.543714 spotlight-dev-0.0.1b2/spotlight/api/organization/user/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.544715 spotlight-dev-0.0.1b2/spotlight/api/organization/view/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.545715 spotlight-dev-0.0.1b2/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1105 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.547715 spotlight-dev-0.0.1b2/spotlight/api/tag/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.548715 spotlight-dev-0.0.1b2/spotlight/api/tag/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.548715 spotlight-dev-0.0.1b2/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.549715 spotlight-dev-0.0.1b2/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.550715 spotlight-dev-0.0.1b2/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.550715 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.551715 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.552715 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.553715 spotlight-dev-0.0.1b2/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.554715 spotlight-dev-0.0.1b2/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.554715 spotlight-dev-0.0.1b2/spotlight/core/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.555715 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.556716 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.557716 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/sql_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.558716 spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.559716 spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/asynchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/synchronously.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.560716 spotlight-dev-0.0.1b2/spotlight/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2189 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/pandas/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/pandas/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/pandas/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.561716 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3933 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/top_level.txt
```

### Comparing `spotlight-dev-0.0.1b1/PKG-INFO` & `spotlight-dev-0.0.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b1/README.md` & `spotlight-dev-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/setup.py` & `spotlight-dev-0.0.1b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     tag = subprocess.getoutput('git tag --sort=version:refname | tail -n1')
     commits = subprocess.getoutput(f'git rev-list {tag}..HEAD --count')
     return f'{tag}.{commits}'
 
 
 setuptools.setup(
     name="spotlight-dev",
-    version="0.0.1b1",
+    version="0.0.1b2",
     author="Spotlight",
     author_email="hello@spotlight.dev",
     description="Spotlight Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://alpha.dev",
     classifiers=[
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/auth/__util.py` & `spotlight-dev-0.0.1b2/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/auth/asynchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/auth/synchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/job/__util.py` & `spotlight-dev-0.0.1b2/spotlight/api/rule/__util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-from spotlight.api.model import SearchRequest
-from spotlight.api.job.model import JobRequest
+import json
+from typing import List
 
+from spotlight.api.model import SearchRequest, LookupRequest
+from spotlight.api.rule.model import RuleRequest
 
-def _get_job_request_info(id: str) -> dict:
-    return {"endpoint": f"config/spotlight/job/{id}"}
 
+def _get_rule_request_info(id: str) -> dict:
+    return {"endpoint": f"dq/rule/{id}"}
 
-def _get_jobs_request_info() -> dict:
-    return {"endpoint": f"config/spotlight/job"}
 
+def _get_rules_request_info() -> dict:
+    return {"endpoint": f"dq/rule"}
 
-def _search_jobs_request_info(request: SearchRequest) -> dict:
-    return {"endpoint": f"config/spotlight/job", "json": request.request_dict()}
 
+def _get_all_rules_by_tags_request_info(request: LookupRequest) -> dict:
+    return {"endpoint": f"dq/rule", "json": request.request_dict()}
 
-def _create_job_request_info(request: JobRequest) -> dict:
-    return {"endpoint": f"config/spotlight/job", "json": request.request_dict()}
 
+def _search_rules_request_info(request: SearchRequest) -> dict:
+    return {"endpoint": f"dq/rule", "json": request.request_dict()}
 
-def _update_job_request_info(id: str, request: JobRequest) -> dict:
-    return {"endpoint": f"config/spotlight/job/{id}", "json": request.request_dict()}
 
+def _create_rule_request_info(request: RuleRequest) -> dict:
+    return {"endpoint": f"dq/rule", "json": request.request_dict()}
 
-def _delete_job_request_info(id: str) -> dict:
-    return {"endpoint": f"config/spotlight/job/{id}"}
 
+def _update_rule_request_info(id: str, request: RuleRequest) -> dict:
+    return {"endpoint": f"dq/rule/{id}", "json": request.request_dict()}
 
-def _get_job_tags_request_info() -> dict:
-    return {"endpoint": f"config/spotlight/job/tags"}
+
+def _declarative_update_rule_tags_request_info(id: str, tag_ids: List[str]) -> dict:
+    return {"endpoint": f"dq/rule/{id}/tag", "json": tag_ids}
+
+
+def _delete_rule_request_info(id: str) -> dict:
+    return {"endpoint": f"dq/rule/{id}"}
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/job/asynchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/job/asynchronous.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from spotlight.api.job.__util import (
     _get_job_request_info,
     _get_jobs_request_info,
     _create_job_request_info,
     _update_job_request_info,
     _delete_job_request_info,
     _search_jobs_request_info,
-    _get_job_tags_request_info,
 )
 from spotlight.api.job.model import JobRequest
 from spotlight.core.common.decorators import async_data_request
 
 from spotlight.core.common.requests import (
     __async_get_request,
     __async_post_request,
@@ -105,19 +104,7 @@
         id (str): Job ID
 
     Returns:
         None
     """
     request_info = _delete_job_request_info(id)
     return await __async_delete_request(**request_info)
-
-
-@async_data_request
-async def async_get_job_tags() -> List[str]:
-    """
-    Asynchronously get all the tags used by jobs
-
-    Returns:
-        List[str]: A list of all the tags used for jobs
-    """
-    request_info = _get_job_tags_request_info()
-    return await __async_get_request(**request_info)
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/job/model.py` & `spotlight-dev-0.0.1b2/spotlight/api/job/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/job/synchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/job/synchronous.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from spotlight.api.job.__util import (
     _get_job_request_info,
     _get_jobs_request_info,
     _create_job_request_info,
     _update_job_request_info,
     _delete_job_request_info,
     _search_jobs_request_info,
-    _get_job_tags_request_info,
 )
 from spotlight.api.job.model import JobRequest
 from spotlight.core.common.decorators import data_request
 
 from spotlight.core.common.requests import (
     __get_request,
     __post_request,
@@ -105,19 +104,7 @@
         id (str): Job ID
 
     Returns:
         None
     """
     request_info = _delete_job_request_info(id)
     return __delete_request(**request_info)
-
-
-@data_request
-def get_job_tags() -> List[str]:
-    """
-    Get all the tags used by jobs
-
-    Returns:
-        List[str]: A list of all the tags used for jobs
-    """
-    request_info = _get_job_tags_request_info()
-    return __get_request(**request_info)
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/job/view/asynchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/job/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/rule/asynchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/rule/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from spotlight.api.rule.__util import (
     _get_rule_request_info,
     _get_rules_request_info,
     _create_rule_request_info,
     _update_rule_request_info,
     _delete_rule_request_info,
     _search_rules_request_info,
-    _get_rule_tags_request_info,
     _declarative_update_rule_tags_request_info,
     _get_all_rules_by_tags_request_info,
 )
 from spotlight.api.rule.model import RuleRequest
 from spotlight.core.common.decorators import async_data_request
 
 from spotlight.core.common.requests import (
@@ -138,19 +137,7 @@
         id (str): Rule ID
 
     Returns:
         None
     """
     request_info = _delete_rule_request_info(id)
     return await __async_delete_request(**request_info)
-
-
-@async_data_request
-async def async_get_rule_tags() -> List[str]:
-    """
-    Asynchronously get all the tags used by rules
-
-    Returns:
-        List[str]: A list of all the tags used for rules
-    """
-    request_info = _get_rule_tags_request_info()
-    return await __async_get_request(**request_info)
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/rule/model.py` & `spotlight-dev-0.0.1b2/spotlight/api/rule/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 
 class RuleRequest(Base):
     name: str
     predicate: str
     description: Optional[str] = Field(default=None)
     threshold: Optional[int] = Field(default=None)
     severity: Optional[Severity] = Field(default=Severity.ERROR)
+    sampling_fields: Optional[List[str]] = Field(default=None)
 
 
 class RuleResponse(Base):
     id: str
     name: str
     description: Optional[str]
     predicate: str
     threshold: int
     severity: Severity
+    sampling_fields: List[str]
     created_by: str
     created_at: int
     updated_by: Optional[str]
     updated_at: Optional[int]
 
 
 class RuleTagResponse(Base):
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/rule/synchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/rule/synchronous.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from spotlight.api.rule.__util import (
     _get_rule_request_info,
     _get_rules_request_info,
     _create_rule_request_info,
     _update_rule_request_info,
     _delete_rule_request_info,
     _search_rules_request_info,
-    _get_rule_tags_request_info,
     _declarative_update_rule_tags_request_info,
     _get_all_rules_by_tags_request_info,
 )
 from spotlight.api.rule.model import RuleRequest
 from spotlight.core.common.decorators import data_request
 from spotlight.core.common.requests import (
     __get_request,
@@ -135,19 +134,7 @@
         id (str): Rule ID
 
     Returns:
         None
     """
     request_info = _delete_rule_request_info(id)
     return __delete_request(**request_info)
-
-
-@data_request
-def get_rule_tags() -> List[str]:
-    """
-    Get all the tags used by rules
-
-    Returns:
-        List[str]: A list of all the tags used for rules
-    """
-    request_info = _get_rule_tags_request_info()
-    return __get_request(**request_info)
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/tag/__util.py` & `spotlight-dev-0.0.1b2/spotlight/api/tag/__util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 from spotlight.api.model import SearchRequest, LookupRequest
 from spotlight.api.tag.model import TagRequest
 
 
 def _get_tag_request_info(id: str) -> dict:
-    return {"endpoint": f"config/spotlight/tag/{id}"}
+    return {"endpoint": f"dq/tag/{id}"}
 
 
 def _get_tag_by_name_request_info(name: str) -> dict:
-    return {"endpoint": f"config/spotlight/tag", "params": {"name": name}}
+    return {"endpoint": f"dq/tag", "params": {"name": name}}
 
 
 def _get_tags_request_info() -> dict:
-    return {"endpoint": f"config/spotlight/tag"}
+    return {"endpoint": f"dq/tag"}
 
 
 def _get_tags_by_lookup_request_info(request: LookupRequest) -> dict:
-    return {"endpoint": f"config/spotlight/tag", "json": request.request_dict()}
+    return {"endpoint": f"dq/tag", "json": request.request_dict()}
 
 
 def _get_tags_by_rule_id_request_info(rule_id: str) -> dict:
-    return {"endpoint": f"config/spotlight/tag", "params": {"rule_id": rule_id}}
+    return {"endpoint": f"dq/tag", "params": {"rule_id": rule_id}}
 
 
 def _search_tags_request_info(request: SearchRequest) -> dict:
-    return {"endpoint": f"config/spotlight/tag", "json": request.request_dict()}
+    return {"endpoint": f"dq/tag", "json": request.request_dict()}
 
 
 def _create_tag_request_info(request: TagRequest) -> dict:
-    return {"endpoint": f"config/spotlight/tag", "json": request.request_dict()}
+    return {"endpoint": f"dq/tag", "json": request.request_dict()}
 
 
 def _update_tag_request_info(id: str, request: TagRequest) -> dict:
-    return {"endpoint": f"config/spotlight/tag/{id}", "json": request.request_dict()}
+    return {"endpoint": f"dq/tag/{id}", "json": request.request_dict()}
 
 
 def _delete_tag_request_info(id: str) -> dict:
-    return {"endpoint": f"config/spotlight/tag/{id}"}
-
-
-def _get_tag_tags_request_info() -> dict:
-    return {"endpoint": f"config/spotlight/tag/tags"}
+    return {"endpoint": f"dq/tag/{id}"}
 
 
 def _unique_tag_name_request_info(name: str) -> dict:
     return {
-        "endpoint": f"config/spotlight/tag/unique",
+        "endpoint": f"dq/tag/unique",
         "params": {"tag_name": name},
     }
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/tag/asynchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/tag/asynchronous.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     _create_tag_request_info,
     _update_tag_request_info,
     _delete_tag_request_info,
     _search_tags_request_info,
     _unique_tag_name_request_info,
     _get_tag_by_name_request_info,
     _get_tags_by_rule_id_request_info,
-    _get_tag_tags_request_info,
     _get_tags_by_lookup_request_info,
 )
 from spotlight.api.tag.model import TagRequest
 from spotlight.core.common.decorators import async_data_request
 
 from spotlight.core.common.requests import (
     __async_get_request,
@@ -155,26 +154,14 @@
         None
     """
     request_info = _delete_tag_request_info(id)
     return await __async_delete_request(**request_info)
 
 
 @async_data_request
-async def async_get_tag_tags() -> List[str]:
-    """
-    Asynchronously get all the tags used by tags
-
-    Returns:
-        List[str]: A list of all the tags used for tags
-    """
-    request_info = _get_tag_tags_request_info()
-    return await __async_get_request(**request_info)
-
-
-@async_data_request
 async def async_is_tag_name_unique(tag_name: str) -> bool:
     """
     Asynchronously checks to see if the tag name is unique
 
     Args:
         tag_name (str): The new tag name that is being tested
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/tag/synchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/tag/synchronous.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     _get_tag_by_name_request_info,
     _get_tags_request_info,
     _get_tags_by_rule_id_request_info,
     _search_tags_request_info,
     _create_tag_request_info,
     _update_tag_request_info,
     _delete_tag_request_info,
-    _get_tag_tags_request_info,
     _unique_tag_name_request_info,
     _get_tags_by_lookup_request_info,
 )
 from spotlight.api.tag.model import TagRequest
 from spotlight.core.common.decorators import data_request
 
 from spotlight.core.common.requests import (
@@ -155,26 +154,14 @@
         None
     """
     request_info = _delete_tag_request_info(id)
     return __delete_request(**request_info)
 
 
 @data_request
-def get_tag_tags() -> List[str]:
-    """
-    Get all the tags used by tags
-
-    Returns:
-        List[str]: A list of all the tags used for tags
-    """
-    request_info = _get_tag_tags_request_info()
-    return __get_request(**request_info)
-
-
-@data_request
 def is_tag_name_unique(tag_name: str) -> bool:
     """
     Checks to see if the tag name is unique
 
     Args:
         tag_name (str): The new tag name that is being tested
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/tag/view/asynchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/tag/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/api/tag/view/synchronous.py` & `spotlight-dev-0.0.1b2/spotlight/api/tag/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/base.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/config.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/date/function.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/__util.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/decorators/timeit.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/errors.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/function.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/metaclass/singleton.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/requests/asynchronous.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/common/requests/synchronous.py` & `spotlight-dev-0.0.1b2/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/__init__.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/abstract.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/decorator.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/decorator.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/plugin/registry.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/registry.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/abstract.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/abstract.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, List, Optional
 
 from spotlight.core.common.enum import Severity
 from spotlight.core.pipeline.execution.rule.enum import RuleTypes
 
 
 class AbstractRule(ABC):
     @property
@@ -26,16 +26,24 @@
     @abstractmethod
     def severity(self) -> Severity:
         """
         The severity of a rule when it fails
         """
         pass
 
+    @property
     @abstractmethod
-    def to_dict(self):
+    def sampling_fields(self) -> Optional[List[str]]:
+        """
+        The name of the fields to sample when a rule fails
+        """
+        pass
+
+    @abstractmethod
+    def to_dict(self) -> dict:
         """
         Converts a rule to dict for saving a Rule to the RuleResult metadata
         """
         pass
 
     def _properties(self) -> dict:
         """
@@ -49,14 +57,18 @@
 
 
 class AbstractCustomCodeRule(AbstractRule, ABC):
     @property
     def name(self) -> str:
         return self.__class__.__name__
 
+    @property
+    def sampling_fields(self) -> Optional[List[str]]:
+        return []
+
     def to_dict(self):
         props = self._properties()
         props.update({"type": RuleTypes.CUSTOM_CODE.value})
         return props
 
     @abstractmethod
     def test(self, data: Any) -> Any:
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/rule/sql_rule.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/sql_rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,53 @@
+from typing import Optional, List
+
 from spotlight.api.rule.model import RuleResponse
 from spotlight.core.common.enum import Severity
 from spotlight.core.pipeline.execution.rule.abstract import AbstractRule
 from spotlight.core.pipeline.execution.rule.enum import RuleTypes
 
 
 class SQLRule(AbstractRule):
     def __init__(
         self,
         name: str,
         predicate: str,
         threshold: int,
         severity: Severity,
+        sampling_fields: Optional[List[str]] = None,
     ):
         self._name = name
         self.predicate = predicate
         self._threshold = threshold
         self._severity = severity
+        self._sampling_fields = sampling_fields
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def threshold(self) -> int:
         return self._threshold
 
     @property
     def severity(self) -> Severity:
         return self._severity
 
+    @property
+    def sampling_fields(self) -> Optional[List[str]]:
+        return self._sampling_fields
+
     def to_dict(self):
         props = self._properties()
         props.update({"type": RuleTypes.SQL.value, "predicate": self.predicate})
         return props
 
     @classmethod
     def from_rule_response(cls, rule: RuleResponse) -> "SQLRule":
         return cls(
             name=rule.name,
             predicate=rule.predicate,
             threshold=rule.threshold,
             severity=Severity(rule.severity),
+            sampling_fields=rule.sampling_fields,
         )
```

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/execution/synchronous.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/model/pipeline.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/asynchronously.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/asynchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/core/pipeline/utils/synchronously.py` & `spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/synchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/pandas/plugin.py` & `spotlight-dev-0.0.1b2/spotlight/pandas/plugin.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight/pandas/runners.py` & `spotlight-dev-0.0.1b2/spotlight/pandas/runners.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b1/spotlight_dev.egg-info/PKG-INFO` & `spotlight-dev-0.0.1b2/spotlight_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b1/spotlight_dev.egg-info/SOURCES.txt` & `spotlight-dev-0.0.1b2/spotlight_dev.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,30 @@
 spotlight/api/job/model.py
 spotlight/api/job/synchronous.py
 spotlight/api/job/view/__init__.py
 spotlight/api/job/view/__util.py
 spotlight/api/job/view/asynchronous.py
 spotlight/api/job/view/model.py
 spotlight/api/job/view/synchronous.py
+spotlight/api/organization/__init__.py
+spotlight/api/organization/__util.py
+spotlight/api/organization/asynchronous.py
+spotlight/api/organization/model.py
+spotlight/api/organization/synchronous.py
+spotlight/api/organization/user/__init__.py
+spotlight/api/organization/user/__util.py
+spotlight/api/organization/user/asynchronous.py
+spotlight/api/organization/user/enum.py
+spotlight/api/organization/user/model.py
+spotlight/api/organization/user/synchronous.py
+spotlight/api/organization/view/__init__.py
+spotlight/api/organization/view/__util.py
+spotlight/api/organization/view/asynchronous.py
+spotlight/api/organization/view/model.py
+spotlight/api/organization/view/synchronous.py
 spotlight/api/rule/__init__.py
 spotlight/api/rule/__util.py
 spotlight/api/rule/asynchronous.py
 spotlight/api/rule/model.py
 spotlight/api/rule/synchronous.py
 spotlight/api/tag/__init__.py
 spotlight/api/tag/__util.py
```

