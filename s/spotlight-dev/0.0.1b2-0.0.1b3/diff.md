# Comparing `tmp/spotlight-dev-0.0.1b2.tar.gz` & `tmp/spotlight-dev-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-dev-0.0.1b2.tar", last modified: Wed May  3 23:10:20 2023, max compression
+gzip compressed data, was "spotlight-dev-0.0.1b3.tar", last modified: Thu May  4 15:38:54 2023, max compression
```

## Comparing `spotlight-dev-0.0.1b2.tar` & `spotlight-dev-0.0.1b3.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.561716 spotlight-dev-0.0.1b2/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-03 23:10:20.561716 spotlight-dev-0.0.1b2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 23:10:20.562716 spotlight-dev-0.0.1b2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.537714 spotlight-dev-0.0.1b2/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.537714 spotlight-dev-0.0.1b2/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.538714 spotlight-dev-0.0.1b2/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.539714 spotlight-dev-0.0.1b2/spotlight/api/job/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.541714 spotlight-dev-0.0.1b2/spotlight/api/job/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/job/view/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.542714 spotlight-dev-0.0.1b2/spotlight/api/organization/
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.543714 spotlight-dev-0.0.1b2/spotlight/api/organization/user/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/user/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.544715 spotlight-dev-0.0.1b2/spotlight/api/organization/view/
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/organization/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.545715 spotlight-dev-0.0.1b2/spotlight/api/rule/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1105 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.547715 spotlight-dev-0.0.1b2/spotlight/api/tag/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.548715 spotlight-dev-0.0.1b2/spotlight/api/tag/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/api/tag/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.548715 spotlight-dev-0.0.1b2/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.549715 spotlight-dev-0.0.1b2/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.550715 spotlight-dev-0.0.1b2/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.550715 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.551715 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.552715 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.553715 spotlight-dev-0.0.1b2/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.554715 spotlight-dev-0.0.1b2/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.554715 spotlight-dev-0.0.1b2/spotlight/core/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)     5930 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.555715 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.556716 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1506 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.557716 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/sql_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.558716 spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.559716 spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/asynchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/synchronously.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.560716 spotlight-dev-0.0.1b2/spotlight/pandas/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2189 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/pandas/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/pandas/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-05-03 23:10:08.000000 spotlight-dev-0.0.1b2/spotlight/pandas/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 23:10:20.561716 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3933 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-03 23:10:20.000000 spotlight-dev-0.0.1b2/spotlight_dev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.810874 spotlight-dev-0.0.1b3/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-04 15:38:54.809873 spotlight-dev-0.0.1b3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 15:38:54.810874 spotlight-dev-0.0.1b3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.784871 spotlight-dev-0.0.1b3/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.785872 spotlight-dev-0.0.1b3/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 15:38:40.000000 spotlight-dev-0.0.1b3/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.786872 spotlight-dev-0.0.1b3/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.787872 spotlight-dev-0.0.1b3/spotlight/api/job/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.788872 spotlight-dev-0.0.1b3/spotlight/api/job/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/job/view/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.790872 spotlight-dev-0.0.1b3/spotlight/api/organization/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.791872 spotlight-dev-0.0.1b3/spotlight/api/organization/user/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/user/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.792872 spotlight-dev-0.0.1b3/spotlight/api/organization/view/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/organization/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.794872 spotlight-dev-0.0.1b3/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1105 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.795872 spotlight-dev-0.0.1b3/spotlight/api/tag/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.796872 spotlight-dev-0.0.1b3/spotlight/api/tag/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/api/tag/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.796872 spotlight-dev-0.0.1b3/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 15:38:40.000000 spotlight-dev-0.0.1b3/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.798873 spotlight-dev-0.0.1b3/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.799873 spotlight-dev-0.0.1b3/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.799873 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.800873 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.801873 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.802873 spotlight-dev-0.0.1b3/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 15:38:40.000000 spotlight-dev-0.0.1b3/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.803873 spotlight-dev-0.0.1b3/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.803873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.803873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.804873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.805873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/sql_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.806873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.807873 spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/asynchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/synchronously.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.808874 spotlight-dev-0.0.1b3/spotlight/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2189 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/pandas/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/pandas/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2023-05-04 15:38:39.000000 spotlight-dev-0.0.1b3/spotlight/pandas/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 15:38:54.809873 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3933 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-04 15:38:54.000000 spotlight-dev-0.0.1b3/spotlight_dev.egg-info/top_level.txt
```

### Comparing `spotlight-dev-0.0.1b2/PKG-INFO` & `spotlight-dev-0.0.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b2/README.md` & `spotlight-dev-0.0.1b3/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/setup.py` & `spotlight-dev-0.0.1b3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     tag = subprocess.getoutput('git tag --sort=version:refname | tail -n1')
     commits = subprocess.getoutput(f'git rev-list {tag}..HEAD --count')
     return f'{tag}.{commits}'
 
 
 setuptools.setup(
     name="spotlight-dev",
-    version="0.0.1b2",
+    version="0.0.1b3",
     author="Spotlight",
     author_email="hello@spotlight.dev",
     description="Spotlight Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://alpha.dev",
     classifiers=[
```

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/auth/__util.py` & `spotlight-dev-0.0.1b3/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/auth/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/auth/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/job/__util.py` & `spotlight-dev-0.0.1b3/spotlight/api/job/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/job/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/job/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/job/model.py` & `spotlight-dev-0.0.1b3/spotlight/api/job/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/job/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/job/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/job/view/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/job/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/organization/__util.py` & `spotlight-dev-0.0.1b3/spotlight/api/organization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/organization/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/organization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/organization/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/organization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/organization/user/__util.py` & `spotlight-dev-0.0.1b3/spotlight/api/organization/user/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/organization/user/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/organization/user/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/organization/user/model.py` & `spotlight-dev-0.0.1b3/spotlight/api/organization/user/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/organization/user/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/organization/user/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/organization/view/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/organization/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/organization/view/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/organization/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/rule/__util.py` & `spotlight-dev-0.0.1b3/spotlight/api/rule/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/rule/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/rule/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/rule/model.py` & `spotlight-dev-0.0.1b3/spotlight/api/rule/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/rule/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/rule/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/tag/__util.py` & `spotlight-dev-0.0.1b3/spotlight/api/tag/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/tag/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/tag/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/tag/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/tag/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/tag/view/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/tag/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/api/tag/view/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/api/tag/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/base.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/config.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/date/function.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/__util.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/decorators/timeit.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/errors.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/function.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/metaclass/singleton.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/requests/asynchronous.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/common/requests/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/__init__.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/abstract.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/decorator.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/decorator.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/plugin/registry.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/plugin/registry.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/abstract.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/abstract.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         """
         pass
 
     @property
     @abstractmethod
     def sampling_fields(self) -> Optional[List[str]]:
         """
-        The name of the fields to sample when a rule fails
+        The name of the fields to sample when a rule doesn't succeed
         """
         pass
 
     @abstractmethod
     def to_dict(self) -> dict:
         """
         Converts a rule to dict for saving a Rule to the RuleResult metadata
```

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/rule/sql_rule.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/rule/sql_rule.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/execution/synchronous.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/execution/synchronous.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         plugin (AbstractPlugin): Plugin for running rules
         data (Any): The data being run through the pipeline
         rules(List[AbstractRule]): The rules being run on the data
 
     Returns:
         List[RuleResult]: The result of running the pipeline
     """
-    results = [plugin.apply_rule(data, rule) for rule in rules]
+    results = [_apply_rule(plugin, data, rule) for rule in rules]
     return results
 
 
 def _multiprocessing_pipeline(
     plugin: AbstractPlugin, data: Any, rules: List[AbstractRule], processes: int
 ) -> List[RuleResult]:
     """
@@ -72,9 +72,29 @@
         rules (List[AbstractRule]): The rules being run on the data
         processes (int): The number of process to spin up when running the rules concurrently
 
     Returns:
         List[RuleResult]: The result of running the pipeline
     """
     with Pool(processes=processes) as pool:
-        results = pool.map(lambda rule: plugin.apply_rule(data, rule), rules)
+        results = pool.map(lambda rule: _apply_rule(plugin, data, rule), rules)
     return results
+
+
+def _apply_rule(plugin: AbstractPlugin, data: Any, rule: AbstractRule) -> RuleResult:
+    """
+    Wrapper for logging purposes
+
+    Args:
+        plugin (AbstractPlugin): Plugin for running rules
+        data (Any): The data being run through the pipeline
+        rule (AbstractRule): The rule being run on the data
+
+    Returns:
+        RuleResult: The result of the rule
+    """
+    logger.debug(f"Running rule {rule.name}")
+    result = plugin.apply_rule(data, rule)
+    logger.info(
+        f"Rule completed [name={rule.name}, flagged_results={result.flagged_results}, threshold={rule.threshold}]: {result.status}"
+    )
+    return result
```

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/model/pipeline.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/asynchronously.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/asynchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/core/pipeline/utils/synchronously.py` & `spotlight-dev-0.0.1b3/spotlight/core/pipeline/utils/synchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/pandas/__util.py` & `spotlight-dev-0.0.1b3/spotlight/pandas/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/pandas/plugin.py` & `spotlight-dev-0.0.1b3/spotlight/pandas/plugin.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b2/spotlight/pandas/runners.py` & `spotlight-dev-0.0.1b3/spotlight/pandas/runners.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,30 +17,25 @@
     Args:
         data (pd.DataFrame): The data being tested
         rule (SQLRule): The rule being applied to the data
 
     Result:
         RuleResult: The result of the rule
     """
-    logger.debug(f"Running rule {rule.name}")
+    logger.debug(f"Running pandas sql rule {rule.name}")
     query = f"""
         SELECT *
         FROM data
         WHERE {rule.predicate}
     """
-
     start_time = current_timestamp()
     result = duckdb.query(query).to_df()
     end_time = current_timestamp()
-
+    logger.debug(f"Pandas sql rule {rule.name} completed")
     result = build_rule_result(rule, start_time, end_time, result)
-    logger.debug(f"Rule result: {result}")
-    logger.info(
-        f"Rule completed [name={rule.name}, flagged_results={result.flagged_results}, threshold={rule.threshold}]: {result.status}"
-    )
     return result
 
 
 def pandas_custom_code_rule_runner(
     data: pd.DataFrame, rule: AbstractCustomCodeRule
 ) -> RuleResult:
     """
@@ -49,19 +44,14 @@
     Args:
         data (pd.DataFrame): The data being tested
         rule (AbstractCustomCodeRule): The rule being applied to the data
 
     Result:
         RuleResult: The result of the rule
     """
-    logger.debug(f"Running rule {rule.name}")
-
+    logger.debug(f"Running pandas custom code rule {rule.name}")
     start_time = current_timestamp()
     result = rule.test(data)
     end_time = current_timestamp()
-
     result = build_rule_result(rule, start_time, end_time, result)
-    logger.debug(f"Rule result: {result}")
-    logger.info(
-        f"Rule completed [name={rule.name}, flagged_results={result.flagged_results}, threshold={rule.threshold}]: {result.status}"
-    )
+    logger.debug(f"Pandas custom code rule {rule.name} completed")
     return result
```

### Comparing `spotlight-dev-0.0.1b2/spotlight_dev.egg-info/PKG-INFO` & `spotlight-dev-0.0.1b3/spotlight_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b2/spotlight_dev.egg-info/SOURCES.txt` & `spotlight-dev-0.0.1b3/spotlight_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

