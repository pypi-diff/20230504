# Comparing `tmp/triad-0.8.6.tar.gz` & `tmp/triad-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triad-0.8.6.tar", last modified: Mon Apr 17 00:38:41 2023, max compression
+gzip compressed data, was "triad-0.8.7.tar", last modified: Thu May  4 06:59:47 2023, max compression
```

## Comparing `triad-0.8.6.tar` & `triad-0.8.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 00:38:01.000000 triad-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-17 00:38:41.933053 triad-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-17 00:38:01.000000 triad-0.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 00:38:41.933053 triad-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-17 00:38:01.000000 triad-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.929053 triad-0.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:01.000000 triad-0.8.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.929053 triad-0.8.6/tests/collections/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/test_function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.929053 triad-0.8.6/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/convert_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.929053 triad-0.8.6/tests/utils/dispatcher_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/dispatcher_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/dispatcher_examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/dispatcher_examples/invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_pyarrow_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-17 00:38:01.000000 triad-0.8.6/triad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 00:38:01.000000 triad-0.8.6/triad/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-17 00:38:01.000000 triad-0.8.6/triad/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    24206 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad_version/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 00:38:01.000000 triad-0.8.6/triad_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 06:59:09.000000 triad-0.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-04 06:59:47.371417 triad-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-04 06:59:09.000000 triad-0.8.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 06:59:47.371417 triad-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 06:59:09.000000 triad-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:09.000000 triad-0.8.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/tests/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/test_function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-04 06:59:09.000000 triad-0.8.7/tests/collections/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/convert_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/tests/utils/dispatcher_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/dispatcher_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/dispatcher_examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/dispatcher_examples/invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_pyarrow_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 06:59:09.000000 triad-0.8.7/tests/utils/test_threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.367417 triad-0.8.7/triad/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-04 06:59:09.000000 triad-0.8.7/triad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/triad/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-05-04 06:59:09.000000 triad-0.8.7/triad/collections/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 06:59:09.000000 triad-0.8.7/triad/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-04 06:59:09.000000 triad-0.8.7/triad/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/triad/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24206 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-04 06:59:09.000000 triad-0.8.7/triad/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/triad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 06:59:47.000000 triad-0.8.7/triad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:59:47.371417 triad-0.8.7/triad_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 06:59:09.000000 triad-0.8.7/triad_version/__init__.py
```

### Comparing `triad-0.8.6/LICENSE` & `triad-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/PKG-INFO` & `triad-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.6
+Version: 0.8.7
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
-Author: Han Wang
-Author-email: goodwanghan@gmail.com
+Author: The Fugue Development Team
+Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
         [![GitHub release](https://img.shields.io/github/release/fugue-project/triad.svg)](https://GitHub.com/fugue-project/triad)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/triad.svg)](https://pypi.python.org/pypi/triad/)
         [![PyPI license](https://img.shields.io/pypi/l/triad.svg)](https://pypi.python.org/pypi/triad/)
         [![PyPI version](https://badge.fury.io/py/triad.svg)](https://pypi.python.org/pypi/triad/)
@@ -24,14 +24,18 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.7
+        
+        * Fix pandas 2.0 warnings
+        
         ### 0.8.6
         
         * Fixed timestamp conversion for pandas 2.0
         
         ### 0.8.5
         
         * Ensure pandas 2.0 compatibility
@@ -218,15 +222,15 @@
         * Added basic utility functions
         * Types and schema are based on pyarrow
         * A better indexed and ordered dict
         * Added ParamDict
         
 Keywords: fugue util utils utility utilities
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `triad-0.8.6/README.md` & `triad-0.8.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 ```bash
 pip install triad
 ```
 
 
 ## Release History
 
+### 0.8.7
+
+* Fix pandas 2.0 warnings
+
 ### 0.8.6
 
 * Fixed timestamp conversion for pandas 2.0
 
 ### 0.8.5
 
 * Ensure pandas 2.0 compatibility
```

### Comparing `triad-0.8.6/setup.py` & `triad-0.8.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,30 +9,30 @@
     name="triad",
     version=__version__,
     packages=find_packages(),
     description="A collection of python utils for Fugue projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="Apache-2.0",
-    author="Han Wang",
-    author_email="goodwanghan@gmail.com",
+    author="The Fugue Development Team",
+    author_email="hello@fugue.ai",
     keywords="fugue util utils utility utilities",
     url="http://github.com/fugue-project/triad",
     install_requires=[
         "numpy",
         "pandas>=1.2.0",
         "six",
         "pyarrow",
         "fs",
         "importlib-metadata; python_version < '3.8'",
     ],
     extras_require={"ciso8601": ["ciso8601"]},
     classifiers=[
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `triad-0.8.6/tests/collections/test_dict.py` & `triad-0.8.7/tests/collections/test_dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/collections/test_fs.py` & `triad-0.8.7/tests/collections/test_fs.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/collections/test_function_wrapper.py` & `triad-0.8.7/tests/collections/test_function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/collections/test_schema.py` & `triad-0.8.7/tests/collections/test_schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_assertion.py` & `triad-0.8.7/tests/utils/test_assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_class_extension.py` & `triad-0.8.7/tests/utils/test_class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_convert.py` & `triad-0.8.7/tests/utils/test_convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_dispatcher.py` & `triad-0.8.7/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_hash.py` & `triad-0.8.7/tests/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_iter.py` & `triad-0.8.7/tests/utils/test_iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_pandas_like.py` & `triad-0.8.7/tests/utils/test_pandas_like.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_pyarrow.py` & `triad-0.8.7/tests/utils/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_pyarrow_convert.py` & `triad-0.8.7/tests/utils/test_pyarrow_convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_rename.py` & `triad-0.8.7/tests/utils/test_rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_schema.py` & `triad-0.8.7/tests/utils/test_schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_string.py` & `triad-0.8.7/tests/utils/test_string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/tests/utils/test_threading.py` & `triad-0.8.7/tests/utils/test_threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/collections/dict.py` & `triad-0.8.7/triad/collections/dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/collections/fs.py` & `triad-0.8.7/triad/collections/fs.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/collections/function_wrapper.py` & `triad-0.8.7/triad/collections/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/collections/schema.py` & `triad-0.8.7/triad/collections/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/assertion.py` & `triad-0.8.7/triad/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/class_extension.py` & `triad-0.8.7/triad/utils/class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/convert.py` & `triad-0.8.7/triad/utils/convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/dispatcher.py` & `triad-0.8.7/triad/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/entry_points.py` & `triad-0.8.7/triad/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/hash.py` & `triad-0.8.7/triad/utils/hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/iter.py` & `triad-0.8.7/triad/utils/iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/json.py` & `triad-0.8.7/triad/utils/json.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/pandas_like.py` & `triad-0.8.7/triad/utils/pandas_like.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         def _wrapper(df: T) -> T:
             return func(df.reset_index(drop=True))
 
         self.ensure_compatible(df)
         if len(cols) == 0:
             return func(df)
         return (
-            df.groupby(cols, dropna=False)
+            df.groupby(cols, dropna=False, group_keys=False)
             .apply(lambda df: _wrapper(df), **kwargs)
             .reset_index(drop=True)
         )
 
     def fillna_default(self, col: Any) -> Any:
         """Fill column with default values according to the dtype of the column.
```

### Comparing `triad-0.8.6/triad/utils/pyarrow.py` & `triad-0.8.7/triad/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/rename.py` & `triad-0.8.7/triad/utils/rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/schema.py` & `triad-0.8.7/triad/utils/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/string.py` & `triad-0.8.7/triad/utils/string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad/utils/threading.py` & `triad-0.8.7/triad/utils/threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.6/triad.egg-info/PKG-INFO` & `triad-0.8.7/triad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.6
+Version: 0.8.7
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
-Author: Han Wang
-Author-email: goodwanghan@gmail.com
+Author: The Fugue Development Team
+Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
         [![GitHub release](https://img.shields.io/github/release/fugue-project/triad.svg)](https://GitHub.com/fugue-project/triad)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/triad.svg)](https://pypi.python.org/pypi/triad/)
         [![PyPI license](https://img.shields.io/pypi/l/triad.svg)](https://pypi.python.org/pypi/triad/)
         [![PyPI version](https://badge.fury.io/py/triad.svg)](https://pypi.python.org/pypi/triad/)
@@ -24,14 +24,18 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.7
+        
+        * Fix pandas 2.0 warnings
+        
         ### 0.8.6
         
         * Fixed timestamp conversion for pandas 2.0
         
         ### 0.8.5
         
         * Ensure pandas 2.0 compatibility
@@ -218,15 +222,15 @@
         * Added basic utility functions
         * Types and schema are based on pyarrow
         * A better indexed and ordered dict
         * Added ParamDict
         
 Keywords: fugue util utils utility utilities
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `triad-0.8.6/triad.egg-info/SOURCES.txt` & `triad-0.8.7/triad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

