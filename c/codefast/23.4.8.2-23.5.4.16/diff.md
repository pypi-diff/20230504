# Comparing `tmp/codefast-23.4.8.2.tar.gz` & `tmp/codefast-23.5.4.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefast-23.4.8.2.tar", last modified: Sat Apr  8 02:19:48 2023, max compression
+gzip compressed data, was "codefast-23.5.4.16.tar", last modified: Thu May  4 16:28:06 2023, max compression
```

## Comparing `codefast-23.4.8.2.tar` & `codefast-23.5.4.16.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-08 02:19:36.000000 codefast-23.4.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-08 02:19:48.427110 codefast-23.4.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-08 02:19:36.000000 codefast-23.4.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.419110 codefast-23.4.8.2/codefast/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.419110 codefast-23.4.8.2/codefast/asyncio/
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/asyncio/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/asyncio/asynclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/axe/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/axe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/axe/axe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/axe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/base/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/base/format_print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/betterargs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/betterargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/betterargs/abstractclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/cn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/concurrency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/concurrent/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/concurrent/fastapi_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/concurrent/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/decorators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/decorators/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2878 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/ds.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/experimental/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/experimental/nsq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/fio/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/fio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/fio/ffpb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/functools/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/functools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/functools/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/functools/subroutine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.423110 codefast-23.4.8.2/codefast/io/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3328 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/dblite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/osdb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3857 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/io/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/codefast/network/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/curl.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/richdownloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/network/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/codefast/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1223 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/factory_method.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3320 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/responsibility_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/patterns/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/codefast/supercell/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/supercell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.427110 codefast-23.4.8.2/codefast/types/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-04-08 02:19:36.000000 codefast-23.4.8.2/codefast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:19:48.419110 codefast-23.4.8.2/codefast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 02:19:48.000000 codefast-23.4.8.2/codefast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 02:19:48.427110 codefast-23.4.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-08 02:19:36.000000 codefast-23.4.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-04 16:27:53.000000 codefast-23.5.4.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 16:28:06.310782 codefast-23.5.4.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-04 16:27:53.000000 codefast-23.5.4.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/asyncio/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/asyncio/rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/axe/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/axe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/axe/axe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/axe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/base/format_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/betterargs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/betterargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/betterargs/abstractclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/concurrency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/concurrent/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2891 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/concurrent/fastapi_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/concurrent/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/decorators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/decorators/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2886 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/experimental/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      581 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/experimental/nsq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/fio/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/fio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/fio/ffpb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast/functools/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/functools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/functools/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/functools/subroutine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3328 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/dblite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/osdb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3857 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/io/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/richdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/network/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1223 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/factory_method.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3320 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/responsibility_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/patterns/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/supercell/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/supercell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/codefast/types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-04 16:27:53.000000 codefast-23.5.4.16/codefast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.306781 codefast-23.5.4.16/codefast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 16:28:05.000000 codefast-23.5.4.16/codefast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-04 16:28:06.000000 codefast-23.5.4.16/codefast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:28:05.000000 codefast-23.5.4.16/codefast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 16:28:05.000000 codefast-23.5.4.16/codefast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 16:28:05.000000 codefast-23.5.4.16/codefast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:28:06.310782 codefast-23.5.4.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-04 16:27:53.000000 codefast-23.5.4.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:28:06.310782 codefast-23.5.4.16/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:27:53.000000 codefast-23.5.4.16/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 16:27:53.000000 codefast-23.5.4.16/tests/test_unique_session.py
```

### Comparing `codefast-23.4.8.2/LICENSE` & `codefast-23.5.4.16/LICENSE`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/PKG-INFO` & `codefast-23.5.4.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefast
-Version: 23.4.8.2
+Version: 23.5.4.16
 Summary: A package for faster coding.
 Home-page: https://github.com/
 Author: Tommy
 Author-email: i@pm.me
 License: UNKNOWN
 Description: A package encapsulating a few frequently used functions for faster Python programming.
```

### Comparing `codefast-23.4.8.2/README.md` & `codefast-23.5.4.16/README.md`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/__init__.py` & `codefast-23.5.4.16/codefast/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/argparser.py` & `codefast-23.5.4.16/codefast/argparser.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/axe/axe.py` & `codefast-23.5.4.16/codefast/axe/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/axe.py` & `codefast-23.5.4.16/codefast/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/base/format_print.py` & `codefast-23.5.4.16/codefast/base/format_print.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/betterargs/abstractclient.py` & `codefast-23.5.4.16/codefast/betterargs/abstractclient.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/cn.py` & `codefast-23.5.4.16/codefast/cn.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/concurrency.py` & `codefast-23.5.4.16/codefast/concurrency.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/concurrent/fastapi_demo.py` & `codefast-23.5.4.16/codefast/concurrent/fastapi_demo.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/concurrent/scheduler.py` & `codefast-23.5.4.16/codefast/concurrent/scheduler.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/constants.py` & `codefast-23.5.4.16/codefast/constants.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/core.py` & `codefast-23.5.4.16/codefast/core.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/decorators/__init__.py` & `codefast-23.5.4.16/codefast/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/decorators/retry.py` & `codefast-23.5.4.16/codefast/decorators/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 import time
 from abc import abstractclassmethod
 from functools import wraps
 
-from codefast.logger import Logger
+from codefast.logger import get_logger
 
-logger = Logger()
+logger = get_logger()
 
 
 class Cleaner(object):
     def __init__(self, e, f) -> None:
         self.error = e
         self.func = f
```

### Comparing `codefast-23.4.8.2/codefast/ds.py` & `codefast-23.5.4.16/codefast/ds.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/experimental/nsq.py` & `codefast-23.5.4.16/codefast/experimental/nsq.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/fio/ffpb.py` & `codefast-23.5.4.16/codefast/fio/ffpb.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/frameworks/__init__.py` & `codefast-23.5.4.16/codefast/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/functools/subroutine.py` & `codefast-23.5.4.16/codefast/functools/subroutine.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/io/_json.py` & `codefast-23.5.4.16/codefast/io/_json.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/io/dblite.py` & `codefast-23.5.4.16/codefast/io/dblite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/io/file.py` & `codefast-23.5.4.16/codefast/io/file.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/io/osdb.py` & `codefast-23.5.4.16/codefast/io/osdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,18 @@
         except:
             yield from []
 
     def values(self) -> Iterator[str]:
         for k in fio.walk(self.value_path):
             yield fio.reads(k)
 
+    def items(self) -> Iterator[Tuple[str, str]]:
+        for k in self.keys():
+            yield (k, self.get(k))
+
     def pop(self, key: str) -> str:
         """ pop key-value
         """
         value = self.get(key)
         fio.rm(self.kpath(key))
         fio.rm(self.vpath(key))
         return value
@@ -131,7 +135,13 @@
         return self.pop(key)
 
     def __len__(self) -> int:
         return len([k for k in self.keys()])
 
     def __repr__(self) -> str:
         return 'osdb(%s)' % self.db_file
+
+    def __iter__(self) -> Iterator[str]:
+        return self.keys()
+    
+    def __contains__(self, key: str) -> bool:
+        return self.exists(key)
```

### Comparing `codefast-23.4.8.2/codefast/io/sqlite.py` & `codefast-23.5.4.16/codefast/io/sqlite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/logger.py` & `codefast-23.5.4.16/codefast/logger.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/math.py` & `codefast-23.5.4.16/codefast/math.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/network/curl.py` & `codefast-23.5.4.16/codefast/network/curl.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/network/factory.py` & `codefast-23.5.4.16/codefast/network/factory.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/network/richdownloader.py` & `codefast-23.5.4.16/codefast/network/richdownloader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/network/tools.py` & `codefast-23.5.4.16/codefast/network/tools.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/patterns/factory_method.py` & `codefast-23.5.4.16/codefast/patterns/factory_method.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/patterns/observer.py` & `codefast-23.5.4.16/codefast/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/patterns/pipeline.py` & `codefast-23.5.4.16/codefast/patterns/pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 #!/usr/bin/env python
-""" rss feed
-"""
 from typing import List, Tuple, Dict
 from abc import ABC, abstractmethod
 
 from codefast import logger as cf
 from codefast.exception import get_exception_str
 
 
-class Component(ABC):
+class BeeMaxin(ABC):
+    """ Base class for pipeline
+    """
+
     def __init__(self) -> None:
         super().__init__()
         self.print_log = True
 
     @abstractmethod
     def process(self, *args, **kwargs):
         pass
 
     def exec(self, *args, **kwargs):
         class_name = self.__class__.__name__
         file_name = self.__class__.__module__.split('.')[-1]
         if self.print_log:
             cf.info('pipeline starts exec [{}], args {}, kwargs {}'.format(
                 file_name + "." + class_name, args, kwargs))
-        results = self.process(*args, **kwargs)
+        honey = self.process(*args, **kwargs)
         if self.print_log:
-            cf.info('pipeline finish exec [{}], results: {}'.format(
-                class_name, results))
-        return results
+            cf.info('pipeline finish exec [{}], honey: {}'.format(
+                class_name, honey))
+        return honey
 
 
 class Pipeline(object):
-    def __init__(self, components: List[Component] = None):
-        self.components = components if components else []
+    def __init__(self, bee_swarm: List[Tuple[str, BeeMaxin]] = None):
+        self.bee_swarm = bee_swarm if bee_swarm else []
         self.source_input = None
 
-    def add(self, component: Component):
-        self.components.append(component)
+    def add(self, bee: Tuple[str, BeeMaxin]):
+        self.bee_swarm.append(bee)
         return self
 
     def set_source_input(self, source_input):
         self.source_input = source_input
         return self
 
+    def gather(self, args=None, forever=False):
+        while True:
+            honey = self.source_input or args
+            try:
+                for _, c in self.bee_swarm:
+                    if honey is not None:
+                        honey = c.exec(honey)
+                    else:
+                        honey = c.exec()
+            except Exception as e:
+                cf.error(get_exception_str(e))
+            if not forever:
+                return honey
+
     def process(self, args=None):
-        results = self.source_input
-        if not results:
-            results = args
-        try:
-            for c in self.components:
-                if results is not None:
-                    results = c.exec(results)
-                else:
-                    results = c.exec()
-        except Exception as e:
-            cf.error(get_exception_str(e))
-        return results
+        return self.gather(args)
```

### Comparing `codefast-23.4.8.2/codefast/patterns/responsibility_chain.py` & `codefast-23.5.4.16/codefast/patterns/responsibility_chain.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/reader.py` & `codefast-23.5.4.16/codefast/reader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/types/__init__.py` & `codefast-23.5.4.16/codefast/types/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.4.8.2/codefast/utils.py` & `codefast-23.5.4.16/codefast/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,60 @@
 # coding:utf-8
+import timeit
 import base64
 import csv
 import functools
 import hashlib
-import inspect
 import os
 import platform
 import signal
 import subprocess
 import sys
 import time
 import warnings
 from functools import wraps
-from pprint import pprint
 from typing import List
 
 import smart_open
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad, unpad
 
 from .logger import info
 
+import datetime
+import secrets
+
+
+def unid(suffix=None):
+    """
+    Generate a unique id
+    """
+    date = datetime.datetime.now().strftime('%Y%m%d-%H%M%S-%f')
+    url = secrets.token_urlsafe(8)
+    if suffix:
+        url += f'-{suffix}'
+    return f'{date}-{url}'
+
+
+def timeit_decorator(func_name=None):
+    def actual_decorator(func):
+        def wrapper(*args, **kwargs):
+            start_time = timeit.default_timer()
+            result = func(*args, **kwargs)
+            end_time = timeit.default_timer()
+            period = round(end_time - start_time, 2)
+            if not func_name:
+                name = func.__name__
+            else:
+                name = func_name
+            print(f"{name} took {period} seconds to execute.")
+            return result
+        return wrapper
+    return actual_decorator
+
 
 def chunks(l: list, n: int) -> list:
     """Yield successive n-sized chunks from l."""
     for i in range(0, len(l), n):
         yield l[i:i + n]
 
 
@@ -89,30 +119,17 @@
 
 
 class _os():
 
     def platform(self) -> str:
         return platform.platform().lower()
 
-
-# =========================================================== display
-def p(*s):
-    for i in s:
-        print(i)
-
-
-def pp(d: dict):
-    pprint(d)
-
-
-def sleep(countdown: int) -> None:
-    time.sleep(countdown)
+# =========================================================== IO
 
 
-# =========================================================== IO
 def show_func_name():
     p(f"\n--------------- {sys._getframe(1).f_code.co_name} ---------------")
 
 
 def smartopen(file_path: str):
     with smart_open.open(file_path) as f:
         return f.readlines()
@@ -285,34 +302,14 @@
 
         return func_with_retries
 
     return retry_decorator
 
 
 # -------------------------------------- End of decorators
-def wrap_mod(mod, deprecated):
-    """Return a wrapped object that warns about deprecated accesses"""
-    deprecated = set(deprecated)
-
-    class Wrapper(object):
-
-        def __getattr__(self, attr):
-            if attr in deprecated:
-                previous_frame = inspect.currentframe().f_back
-                Logger().info(str(previous_frame))
-                warnings.warn(f"Alias {attr} is deprecated")
-            return getattr(mod, attr)
-
-        def __setattr__(self, attr, value):
-            if attr in deprecated:
-                warnings.warn("Property %s is deprecated" % attr)
-            return setattr(mod, attr, value)
-
-    return Wrapper()
-
 
 def cipher(key: str, text: str) -> str:
     key = (key * 100)[:32]
     BLOCK_SIZE = 32
     _cipher = AES.new(key.encode('utf8'), AES.MODE_ECB)
     msg = _cipher.encrypt(pad(text.encode(), BLOCK_SIZE))
     return str(msg, encoding='latin-1')
```

### Comparing `codefast-23.4.8.2/codefast.egg-info/PKG-INFO` & `codefast-23.5.4.16/codefast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefast
-Version: 23.4.8.2
+Version: 23.5.4.16
 Summary: A package for faster coding.
 Home-page: https://github.com/
 Author: Tommy
 Author-email: i@pm.me
 License: UNKNOWN
 Description: A package encapsulating a few frequently used functions for faster Python programming.
```

### Comparing `codefast-23.4.8.2/codefast.egg-info/SOURCES.txt` & `codefast-23.5.4.16/codefast.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 codefast/utils.py
 codefast.egg-info/PKG-INFO
 codefast.egg-info/SOURCES.txt
 codefast.egg-info/dependency_links.txt
 codefast.egg-info/requires.txt
 codefast.egg-info/top_level.txt
 codefast/asyncio/__init__.py
-codefast/asyncio/asynclient.py
+codefast/asyncio/rabbitmq.py
 codefast/axe/__init__.py
 codefast/axe/axe.py
 codefast/base/__init__.py
 codefast/base/format_print.py
 codefast/betterargs/__init__.py
 codefast/betterargs/abstractclient.py
 codefast/concurrent/__init__.py
@@ -56,8 +56,10 @@
 codefast/patterns/__init__.py
 codefast/patterns/factory_method.py
 codefast/patterns/observer.py
 codefast/patterns/pipeline.py
 codefast/patterns/responsibility_chain.py
 codefast/patterns/singleton.py
 codefast/supercell/__init__.py
-codefast/types/__init__.py
+codefast/types/__init__.py
+tests/__init__.py
+tests/test_unique_session.py
```

### Comparing `codefast-23.4.8.2/setup.py` & `codefast-23.5.4.16/setup.py`

 * *Files identical despite different names*

