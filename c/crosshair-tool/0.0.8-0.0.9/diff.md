# Comparing `tmp/crosshair-tool-0.0.8.tar.gz` & `tmp/crosshair-tool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crosshair-tool-0.0.8.tar", last modified: Fri Nov 27 16:36:29 2020, max compression
+gzip compressed data, was "dist/crosshair-tool-0.0.9.tar", last modified: Sat Jan 16 16:34:16 2021, max compression
```

## Comparing `crosshair-tool-0.0.8.tar` & `crosshair-tool-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2020-11-27 16:36:29.564325 crosshair-tool-0.0.8/
--rw-r--r--   0 pschanely   (501) staff       (20)    14311 2020-11-27 16:36:29.565022 crosshair-tool-0.0.8/PKG-INFO
--rw-r--r--   0 pschanely   (501) staff       (20)    11526 2020-11-25 02:13:03.000000 crosshair-tool-0.0.8/README.md
-drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2020-11-27 16:36:29.535837 crosshair-tool-0.0.8/crosshair/
--rw-r--r--   0 pschanely   (501) staff       (20)      282 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/__init__.py
--rw-r--r--   0 pschanely   (501) staff       (20)     6153 2020-11-22 01:03:21.000000 crosshair-tool-0.0.8/crosshair/abcstring.py
--rw-r--r--   0 pschanely   (501) staff       (20)    15438 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/condition_parser.py
--rw-r--r--   0 pschanely   (501) staff       (20)     4614 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/condition_parser_test.py
--rwxr-xr-x   0 pschanely   (501) staff       (20)    45914 2020-11-22 19:33:59.000000 crosshair-tool-0.0.8/crosshair/core.py
--rw-r--r--   0 pschanely   (501) staff       (20)      433 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/core_and_libs.py
--rw-r--r--   0 pschanely   (501) staff       (20)    21483 2020-11-24 03:32:11.000000 crosshair-tool-0.0.8/crosshair/core_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)      511 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/doctests_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)     6282 2020-02-24 11:00:56.000000 crosshair-tool-0.0.8/crosshair/dynamic_typing.py
--rw-r--r--   0 pschanely   (501) staff       (20)     3091 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/dynamic_typing_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)     7538 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/enforce.py
--rw-r--r--   0 pschanely   (501) staff       (20)     2336 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/enforce_test.py
-drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2020-11-27 16:36:29.546963 crosshair-tool-0.0.8/crosshair/examples/
--rw-r--r--   0 pschanely   (501) staff       (20)        0 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/examples/__init__.py
--rw-r--r--   0 pschanely   (501) staff       (20)     1476 2020-03-01 03:04:01.000000 crosshair-tool-0.0.8/crosshair/examples/arith.py
--rw-r--r--   0 pschanely   (501) staff       (20)     2103 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/examples/chess.py
--rw-r--r--   0 pschanely   (501) staff       (20)      764 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/examples/hash_consistent_with_equals.py
--rw-r--r--   0 pschanely   (501) staff       (20)      393 2020-02-27 14:55:35.000000 crosshair-tool-0.0.8/crosshair/examples/immutable_class.py
--rw-r--r--   0 pschanely   (501) staff       (20)      321 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/examples/nesting_inference.py
--rw-r--r--   0 pschanely   (501) staff       (20)     4036 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/examples/numpy_examples.py
--rw-r--r--   0 pschanely   (501) staff       (20)      707 2020-02-09 18:53:42.000000 crosshair-tool-0.0.8/crosshair/examples/rolling_average.py
--rw-r--r--   0 pschanely   (501) staff       (20)     3305 2020-02-09 14:29:50.000000 crosshair-tool-0.0.8/crosshair/examples/showcase.py
--rw-r--r--   0 pschanely   (501) staff       (20)     2583 2020-02-24 10:59:40.000000 crosshair-tool-0.0.8/crosshair/examples/tic_tac_toe.py
--rw-r--r--   0 pschanely   (501) staff       (20)     9811 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/fuzz_core_test.py
-drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2020-11-27 16:36:29.557327 crosshair-tool-0.0.8/crosshair/libimpl/
--rw-r--r--   0 pschanely   (501) staff       (20)      484 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/libimpl/__init__.py
--rw-r--r--   0 pschanely   (501) staff       (20)    65960 2020-11-27 10:23:01.000000 crosshair-tool-0.0.8/crosshair/libimpl/builtinslib.py
--rw-r--r--   0 pschanely   (501) staff       (20)    40374 2020-11-27 10:04:22.000000 crosshair-tool-0.0.8/crosshair/libimpl/builtinslib_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)     5703 2020-11-18 13:37:24.000000 crosshair-tool-0.0.8/crosshair/libimpl/collectionslib.py
--rw-r--r--   0 pschanely   (501) staff       (20)     6262 2020-11-18 13:46:49.000000 crosshair-tool-0.0.8/crosshair/libimpl/collectionslib_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)     4883 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/libimpl/datetimelib.py
--rw-r--r--   0 pschanely   (501) staff       (20)     3048 2020-10-04 15:50:59.000000 crosshair-tool-0.0.8/crosshair/libimpl/datetimelib_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)      355 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/libimpl/mathlib.py
--rw-r--r--   0 pschanely   (501) staff       (20)     1022 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/libimpl/mathlib_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)      598 2020-05-10 12:40:17.000000 crosshair-tool-0.0.8/crosshair/libimpl/randomlib.py
--rw-r--r--   0 pschanely   (501) staff       (20)    13846 2020-10-04 15:41:11.000000 crosshair-tool-0.0.8/crosshair/libimpl/relib.py
--rw-r--r--   0 pschanely   (501) staff       (20)     9618 2020-11-22 01:09:13.000000 crosshair-tool-0.0.8/crosshair/libimpl/relib_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)     1828 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/localhost_comms.py
--rw-r--r--   0 pschanely   (501) staff       (20)    19124 2020-11-24 03:47:29.000000 crosshair-tool-0.0.8/crosshair/main.py
--rw-r--r--   0 pschanely   (501) staff       (20)     5432 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/main_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)     8794 2020-02-28 19:02:19.000000 crosshair-tool-0.0.8/crosshair/objectproxy.py
--rw-r--r--   0 pschanely   (501) staff       (20)      671 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/objectproxy_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)    11135 2020-11-18 07:36:04.000000 crosshair-tool-0.0.8/crosshair/simplestructs.py
--rw-r--r--   0 pschanely   (501) staff       (20)     1573 2020-02-06 01:00:23.000000 crosshair-tool-0.0.8/crosshair/simplestructs_test.py
--rw-r--r--   0 pschanely   (501) staff       (20)    24272 2020-11-21 18:01:13.000000 crosshair-tool-0.0.8/crosshair/statespace.py
--rw-r--r--   0 pschanely   (501) staff       (20)     2335 2020-11-08 16:52:40.000000 crosshair-tool-0.0.8/crosshair/test_util.py
--rw-r--r--   0 pschanely   (501) staff       (20)     2534 2020-08-09 13:06:26.000000 crosshair-tool-0.0.8/crosshair/type_repo.py
--rw-r--r--   0 pschanely   (501) staff       (20)     8520 2020-11-22 19:30:26.000000 crosshair-tool-0.0.8/crosshair/util.py
-drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2020-11-27 16:36:29.562042 crosshair-tool-0.0.8/crosshair_tool.egg-info/
--rw-r--r--   0 pschanely   (501) staff       (20)    14311 2020-11-27 16:36:28.000000 crosshair-tool-0.0.8/crosshair_tool.egg-info/PKG-INFO
--rw-r--r--   0 pschanely   (501) staff       (20)     1628 2020-11-27 16:36:28.000000 crosshair-tool-0.0.8/crosshair_tool.egg-info/SOURCES.txt
--rw-r--r--   0 pschanely   (501) staff       (20)        1 2020-11-27 16:36:28.000000 crosshair-tool-0.0.8/crosshair_tool.egg-info/dependency_links.txt
--rw-r--r--   0 pschanely   (501) staff       (20)       51 2020-11-27 16:36:28.000000 crosshair-tool-0.0.8/crosshair_tool.egg-info/entry_points.txt
--rw-r--r--   0 pschanely   (501) staff       (20)       50 2020-11-27 16:36:28.000000 crosshair-tool-0.0.8/crosshair_tool.egg-info/requires.txt
--rw-r--r--   0 pschanely   (501) staff       (20)       10 2020-11-27 16:36:28.000000 crosshair-tool-0.0.8/crosshair_tool.egg-info/top_level.txt
--rw-r--r--   0 pschanely   (501) staff       (20)       78 2020-11-27 16:36:29.566100 crosshair-tool-0.0.8/setup.cfg
--rw-r--r--   0 pschanely   (501) staff       (20)     1340 2020-11-27 16:29:15.000000 crosshair-tool-0.0.8/setup.py
+drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2021-01-16 16:34:16.826913 crosshair-tool-0.0.9/
+-rw-r--r--   0 pschanely   (501) staff       (20)    15259 2021-01-16 16:34:16.826524 crosshair-tool-0.0.9/PKG-INFO
+-rw-r--r--   0 pschanely   (501) staff       (20)    12248 2021-01-16 15:09:07.000000 crosshair-tool-0.0.9/README.md
+drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2021-01-16 16:34:16.806994 crosshair-tool-0.0.9/crosshair/
+-rw-r--r--   0 pschanely   (501) staff       (20)      282 2020-11-18 07:36:04.000000 crosshair-tool-0.0.9/crosshair/__init__.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     6153 2020-11-22 01:03:21.000000 crosshair-tool-0.0.9/crosshair/abcstring.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    23494 2021-01-16 12:45:29.000000 crosshair-tool-0.0.9/crosshair/condition_parser.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     8195 2021-01-16 12:36:18.000000 crosshair-tool-0.0.9/crosshair/condition_parser_test.py
+-rwxr-xr-x   0 pschanely   (501) staff       (20)    49364 2021-01-15 03:46:22.000000 crosshair-tool-0.0.9/crosshair/core.py
+-rw-r--r--   0 pschanely   (501) staff       (20)      554 2020-12-24 14:04:57.000000 crosshair-tool-0.0.9/crosshair/core_and_libs.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    22880 2021-01-04 17:36:22.000000 crosshair-tool-0.0.9/crosshair/core_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     9539 2021-01-15 10:27:17.000000 crosshair-tool-0.0.9/crosshair/diff_behavior.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     4183 2021-01-16 02:17:06.000000 crosshair-tool-0.0.9/crosshair/diff_behavior_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)      511 2020-02-06 01:00:23.000000 crosshair-tool-0.0.9/crosshair/doctests_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     6282 2020-02-24 11:00:56.000000 crosshair-tool-0.0.9/crosshair/dynamic_typing.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     3091 2020-02-06 01:00:23.000000 crosshair-tool-0.0.9/crosshair/dynamic_typing_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     8880 2021-01-02 17:03:39.000000 crosshair-tool-0.0.9/crosshair/enforce.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     4608 2020-12-27 14:19:11.000000 crosshair-tool-0.0.9/crosshair/enforce_test.py
+drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2021-01-16 16:34:16.812373 crosshair-tool-0.0.9/crosshair/examples/
+-rw-r--r--   0 pschanely   (501) staff       (20)        0 2020-02-06 01:00:23.000000 crosshair-tool-0.0.9/crosshair/examples/__init__.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     1476 2020-03-01 03:04:01.000000 crosshair-tool-0.0.9/crosshair/examples/arith.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     2103 2020-02-06 01:00:23.000000 crosshair-tool-0.0.9/crosshair/examples/chess.py
+-rw-r--r--   0 pschanely   (501) staff       (20)      764 2020-02-06 01:00:23.000000 crosshair-tool-0.0.9/crosshair/examples/hash_consistent_with_equals.py
+-rw-r--r--   0 pschanely   (501) staff       (20)      393 2020-02-27 14:55:35.000000 crosshair-tool-0.0.9/crosshair/examples/immutable_class.py
+-rw-r--r--   0 pschanely   (501) staff       (20)      321 2020-02-06 01:00:23.000000 crosshair-tool-0.0.9/crosshair/examples/nesting_inference.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     4036 2020-02-06 01:00:23.000000 crosshair-tool-0.0.9/crosshair/examples/numpy_examples.py
+-rw-r--r--   0 pschanely   (501) staff       (20)      707 2020-02-09 18:53:42.000000 crosshair-tool-0.0.9/crosshair/examples/rolling_average.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     3305 2020-02-09 14:29:50.000000 crosshair-tool-0.0.9/crosshair/examples/showcase.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     2583 2021-01-16 15:08:52.000000 crosshair-tool-0.0.9/crosshair/examples/tic_tac_toe.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    11321 2021-01-06 05:53:39.000000 crosshair-tool-0.0.9/crosshair/fuzz_core_test.py
+drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2021-01-16 16:34:16.821773 crosshair-tool-0.0.9/crosshair/libimpl/
+-rw-r--r--   0 pschanely   (501) staff       (20)      484 2020-11-18 07:36:04.000000 crosshair-tool-0.0.9/crosshair/libimpl/__init__.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    70637 2021-01-14 14:07:19.000000 crosshair-tool-0.0.9/crosshair/libimpl/builtinslib.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    45119 2021-01-16 12:19:59.000000 crosshair-tool-0.0.9/crosshair/libimpl/builtinslib_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     5703 2020-11-18 13:37:24.000000 crosshair-tool-0.0.9/crosshair/libimpl/collectionslib.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     6262 2020-11-18 13:46:49.000000 crosshair-tool-0.0.9/crosshair/libimpl/collectionslib_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     4883 2020-11-18 07:36:04.000000 crosshair-tool-0.0.9/crosshair/libimpl/datetimelib.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     3084 2021-01-14 01:10:28.000000 crosshair-tool-0.0.9/crosshair/libimpl/datetimelib_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)      355 2020-11-29 14:57:52.000000 crosshair-tool-0.0.9/crosshair/libimpl/mathlib.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     1089 2020-12-20 18:35:07.000000 crosshair-tool-0.0.9/crosshair/libimpl/mathlib_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)      598 2020-05-10 12:40:17.000000 crosshair-tool-0.0.9/crosshair/libimpl/randomlib.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    14153 2021-01-07 23:31:51.000000 crosshair-tool-0.0.9/crosshair/libimpl/relib.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    10077 2021-01-08 03:13:50.000000 crosshair-tool-0.0.9/crosshair/libimpl/relib_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     1828 2020-02-06 01:00:23.000000 crosshair-tool-0.0.9/crosshair/localhost_comms.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    21281 2021-01-16 02:16:35.000000 crosshair-tool-0.0.9/crosshair/main.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     7121 2021-01-16 02:18:22.000000 crosshair-tool-0.0.9/crosshair/main_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     8794 2020-02-28 19:02:19.000000 crosshair-tool-0.0.9/crosshair/objectproxy.py
+-rw-r--r--   0 pschanely   (501) staff       (20)      671 2020-02-06 01:00:23.000000 crosshair-tool-0.0.9/crosshair/objectproxy_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    21448 2021-01-16 16:15:07.000000 crosshair-tool-0.0.9/crosshair/simplestructs.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     5670 2021-01-13 02:34:22.000000 crosshair-tool-0.0.9/crosshair/simplestructs_test.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    25561 2021-01-14 09:33:35.000000 crosshair-tool-0.0.9/crosshair/statespace.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     2765 2021-01-13 03:06:48.000000 crosshair-tool-0.0.9/crosshair/test_util.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     2534 2020-08-09 13:06:26.000000 crosshair-tool-0.0.9/crosshair/type_repo.py
+-rw-r--r--   0 pschanely   (501) staff       (20)    12414 2021-01-14 01:11:24.000000 crosshair-tool-0.0.9/crosshair/util.py
+-rw-r--r--   0 pschanely   (501) staff       (20)     3001 2021-01-03 19:17:35.000000 crosshair-tool-0.0.9/crosshair/util_test.py
+drwxr-xr-x   0 pschanely   (501) staff       (20)        0 2021-01-16 16:34:16.825845 crosshair-tool-0.0.9/crosshair_tool.egg-info/
+-rw-r--r--   0 pschanely   (501) staff       (20)    15259 2021-01-16 16:34:16.000000 crosshair-tool-0.0.9/crosshair_tool.egg-info/PKG-INFO
+-rw-r--r--   0 pschanely   (501) staff       (20)     1700 2021-01-16 16:34:16.000000 crosshair-tool-0.0.9/crosshair_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 pschanely   (501) staff       (20)        1 2021-01-16 16:34:16.000000 crosshair-tool-0.0.9/crosshair_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 pschanely   (501) staff       (20)       51 2021-01-16 16:34:16.000000 crosshair-tool-0.0.9/crosshair_tool.egg-info/entry_points.txt
+-rw-r--r--   0 pschanely   (501) staff       (20)       49 2021-01-16 16:34:16.000000 crosshair-tool-0.0.9/crosshair_tool.egg-info/requires.txt
+-rw-r--r--   0 pschanely   (501) staff       (20)       10 2021-01-16 16:34:16.000000 crosshair-tool-0.0.9/crosshair_tool.egg-info/top_level.txt
+-rw-r--r--   0 pschanely   (501) staff       (20)       38 2021-01-16 16:34:16.827029 crosshair-tool-0.0.9/setup.cfg
+-rw-r--r--   0 pschanely   (501) staff       (20)     1339 2021-01-16 15:09:07.000000 crosshair-tool-0.0.9/setup.py
```

### Comparing `crosshair-tool-0.0.8/PKG-INFO` & `crosshair-tool-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosshair-tool
-Version: 0.0.8
+Version: 0.0.9
 Summary: A static analysis tool for Python using symbolic execution.
 Home-page: https://github.com/pschanely/CrossHair
 Author: Phillip Schanely
 Author-email: pschanely+vE7F@gmail.com
 License: MIT
 Description: <img src="https://raw.githubusercontent.com/pschanely/CrossHair/master/doc/logo.png" width="5%" align="left">
         
@@ -12,36 +12,39 @@
         
         [![Join the chat at https://gitter.im/Cross_Hair/Lobby](https://badges.gitter.im/Cross_Hair/Lobby.svg)](https://gitter.im/Cross_Hair/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
         [![codecov](https://codecov.io/gh/pschanely/CrossHair/branch/master/graph/badge.svg)](https://codecov.io/gh/pschanely/CrossHair)
         [![Build Status](https://travis-ci.org/pschanely/CrossHair.svg?branch=master)](https://travis-ci.org/pschanely/CrossHair)
         
         An analysis tool for Python that blurs the line between testing and type systems.
         
-        > **_THE LATEST NEWS:_**  Now you can try out CrossHair in your browser at [crosshair-web.org](https://crosshair-web.org)!
+        > **_THE LATEST NEWS:_**  CrossHair is growing commands unrelated to contracts; compare the behavior of two functions with the [diffbehavior](https://raw.githubusercontent.com/pschanely/CrossHair/master/doc/diff_behavior.md) command!
         
         If you have functions with [type annotations](https://www.python.org/dev/peps/pep-0484/) and add some checks in a [PEP 316](https://www.python.org/dev/peps/pep-0316/)-inspired syntax, CrossHair will attempt to find counterexamples for you:
         
         ![Animated GIF demonstrating the verification of a python function](https://raw.githubusercontent.com/pschanely/CrossHair/master/doc/duplicate_list.gif)
         
         CrossHair works by repeatedly calling your functions with symbolic inputs.
         It uses an [SMT solver](https://en.wikipedia.org/wiki/Satisfiability_modulo_theories) (a kind of theorem prover) to explore viable execution paths and find counterexamples for you.
         This is not a new idea; an approach for Python was first described in [this paper](https://hoheinzollern.files.wordpress.com/2008/04/seer1.pdf).
         However, to my knowledge, CrossHair is the most complete implementation of the idea: it supports symbolic lists, dictionaries, sets, and custom/mutable objects.
         
-        > **_NOTE:_**  CrossHair is in a highly experimental state right now. You can help though - keep reading!
+        Try CrossHair right now, in your browser, at [crosshair-web.org](https://crosshair-web.org)!
+        
+        > **_NOTE:_**  CrossHair is in an experimental state right now. You can help though - keep reading!
         
         |Contents|
         |--------|
         |[Why Should I Use CrossHair?](#why-should-i-use-crosshair)|
         |[How to Write Contracts](#how-to-write-contracts)|
         |[Get Started](#get-started)|
         |[IDE Integrations](#ide-integrations)|
         |[Limitations](#limitations)|
         |[How Can I Help?](#how-can-i-help)|
         |[Contributors](#contributors)|
+        |[Change Log](#change-log)|
         |[Related Work](#related-work)|
         
         
         
         ## Why Should I Use CrossHair?
         
         **More precision.** Commonly, we care about more than just the type. Is it really any integer, or is it a **positive** integer? Is it any list, or does it have to be a non-empty list? CrossHair gives you that precision:
@@ -95,15 +98,15 @@
         
         You can find examples in the [examples/](https://github.com/pschanely/CrossHair/tree/master/crosshair/examples) directory 
         and try it in your browser at [crosshair-web.org](https://crosshair-web.org).
         
         
         ## Get Started
         
-        > **_NOTE:_**  CrossHair is in a highly experimental state right now. If you're using it, it's because you want it to succeed, want to help, or are just interested in the technology.
+        > **_NOTE:_**  CrossHair is in an experimental state right now. If you're using it, it's because you want it to succeed, want to help, or are just interested in the technology.
         
         CrossHair is supported only on Python 3.7+ and only on CPython (the most common Python implementation).
         
         Inside the development environment of the code you want to analyze (virtual environment, conda environment, etc), install:
         ```shell
         pip install crosshair-tool
         ```
@@ -127,22 +130,24 @@
         
         If you make a plugin for your favorite editor (please do!), submit a pull request to add it above. The `crosshair check [FILENAME]` command will yield results in the same format as the mypy type checker. (a non-zero exit for for errors, and lines formatted as `{FILENAME}:{LINE_NUMBER}:error:{MESSAGE}`)
         
         ## Limitations
         
         A (wildly incomplete) list of present limitations. Some of these will be lifted over time (your help is welcome!); some may never be lifted.
         
+        * Be aware that the absence of a counterexample does not guarantee that the property holds.
         * Symbolic values are implemented as Python proxy values. CrossHair monkey-patches the system to maintain a good illusion, but the illusion is not complete. For example,
           * Code that cares about the identity values (x is y) may not be correctly analyzed.
           * Code that cares about the types of values may not be correctly analyzed.
         * Only function and class definitions at the top level are analyzed. (i.e. not when nested inside other functions/classes)
         * Only deteministic behavior can be analyzed. (your code always does the same thing when starting with the same values)
           * CrossHair may produce a `NotDeterministic` error when it detects this.
+        * Be careful: CrossHair will actually run your code and may apply any arguments to it.
+          * If you run CrossHair on code calling [shutil.rmtree](https://docs.python.org/3/library/shutil.html#shutil.rmtree), you **will** destroy your filesystem.
         * Comsuming values of an iterator/generator in a pre- or post-condition will produce [unexpected behavior](https://github.com/pschanely/CrossHair/issues/9).
-        * Be aware that the absence of a counterexample does not guarantee that the property holds.
         * SMT sovlers have very different perspectives on hard problems and easy problems than humans.
           * Be prepared to be surprised both by what CrossHair can tell you, and what it cannot.
         
         ## How Can I Help?
         
         * [Try it out](#get-started) on your own python project! Be communicative about what does and doesn't work.
         * Participate (or just lurk) in the [gitter chat](https://gitter.im/Cross_Hair/Lobby).
@@ -154,20 +159,28 @@
         
         ## Contributors
         
         * [**Phil Schanely**](https://twitter.com/pschanely)
         * [**Edward Haigh**](https://github.com/oneEdoubleD)
         * [**Saul Shanabrook**](https://github.com/saulshanabrook/)
         
+        ## Change Log
+        
+        0.0.9
+        * Introduce [the diffbehavior command](https://raw.githubusercontent.com/pschanely/CrossHair/master/doc/diff_behavior.md) which finds inputs that distinguish the behavior of two functions.
+        * Upgrade to the latest release of z3 (4.8.9.0)
+        * Fix [an installation error](https://github.com/pschanely/CrossHair/issues/41) on windows.
+        * Fix a variety of other bugs.
+        
         ## Related Work
         
         |Technology|Relation|
         |---------:|:-------|
         | [dependent types](https://en.wikipedia.org/wiki/Dependent_type), [refinement types](https://en.wikipedia.org/wiki/Refinement_type) | CrossHair aims to provide many of the same capabilities as these advanced type systems. CrossHair is easier to learn (because it is just python), but is incomplete (it can't always tell you whether a condition holds). |
-        | [design by contract](https://en.wikipedia.org/wiki/Design_by_contract) | Unlike other systems and tools for contracts, CrossHair attempts to verify pre- and post-conditions before you run them. |
+        | [design by contract](https://en.wikipedia.org/wiki/Design_by_contract) | Unlike most tools for contracts, CrossHair attempts to verify pre-conditions and post-conditions before you run them. |
         | [fuzz testing](https://en.wikipedia.org/wiki/Fuzzing), [QuickCheck](https://en.wikipedia.org/wiki/QuickCheck), [property testing](https://en.wikipedia.org/wiki/Property_testing), [Hypothesis](https://hypothesis.readthedocs.io/) | CrossHair has many of the same goals as these tools. However, CrossHair uses an SMT solver to find inputs rather than the (typically) randomized approaches that these tools use. |
         | [concolic testing](https://en.wikipedia.org/wiki/Concolic_testing) | State-of-the-art fuzz testers employ SMT solvers in a similar fashion as CrossHair. |
         | [SMT solvers](https://en.wikipedia.org/wiki/Satisfiability_modulo_theories) | SMT solvers power many of the tools in this table. CrossHair uses [Z3](https://github.com/Z3Prover/z3). |
         | [angr](https://angr.io), [klee](https://klee.github.io/) | Symbolic execution of **binary** code. Unlike these tools, CrossHair models the semantics of Python directly. |
         | [PyExZ3](https://github.com/thomasjball/PyExZ3), [pySim](https://github.com/bannsec/pySym), [PEF](https://git.cs.famaf.unc.edu.ar/dbarsotti/pef) | Take approaches that are very similar to CrossHair, in various states of completeness. CrossHair is generally more perscriptive or product-like than these tools. |
         
 Platform: UNKNOWN
```

### Comparing `crosshair-tool-0.0.8/README.md` & `crosshair-tool-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,39 @@
 
 [![Join the chat at https://gitter.im/Cross_Hair/Lobby](https://badges.gitter.im/Cross_Hair/Lobby.svg)](https://gitter.im/Cross_Hair/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![codecov](https://codecov.io/gh/pschanely/CrossHair/branch/master/graph/badge.svg)](https://codecov.io/gh/pschanely/CrossHair)
 [![Build Status](https://travis-ci.org/pschanely/CrossHair.svg?branch=master)](https://travis-ci.org/pschanely/CrossHair)
 
 An analysis tool for Python that blurs the line between testing and type systems.
 
-> **_THE LATEST NEWS:_**  Now you can try out CrossHair in your browser at [crosshair-web.org](https://crosshair-web.org)!
+> **_THE LATEST NEWS:_**  CrossHair is growing commands unrelated to contracts; compare the behavior of two functions with the [diffbehavior](doc/diff_behavior.md) command!
 
 If you have functions with [type annotations](https://www.python.org/dev/peps/pep-0484/) and add some checks in a [PEP 316](https://www.python.org/dev/peps/pep-0316/)-inspired syntax, CrossHair will attempt to find counterexamples for you:
 
 ![Animated GIF demonstrating the verification of a python function](doc/duplicate_list.gif)
 
 CrossHair works by repeatedly calling your functions with symbolic inputs.
 It uses an [SMT solver](https://en.wikipedia.org/wiki/Satisfiability_modulo_theories) (a kind of theorem prover) to explore viable execution paths and find counterexamples for you.
 This is not a new idea; an approach for Python was first described in [this paper](https://hoheinzollern.files.wordpress.com/2008/04/seer1.pdf).
 However, to my knowledge, CrossHair is the most complete implementation of the idea: it supports symbolic lists, dictionaries, sets, and custom/mutable objects.
 
-> **_NOTE:_**  CrossHair is in a highly experimental state right now. You can help though - keep reading!
+Try CrossHair right now, in your browser, at [crosshair-web.org](https://crosshair-web.org)!
+
+> **_NOTE:_**  CrossHair is in an experimental state right now. You can help though - keep reading!
 
 |Contents|
 |--------|
 |[Why Should I Use CrossHair?](#why-should-i-use-crosshair)|
 |[How to Write Contracts](#how-to-write-contracts)|
 |[Get Started](#get-started)|
 |[IDE Integrations](#ide-integrations)|
 |[Limitations](#limitations)|
 |[How Can I Help?](#how-can-i-help)|
 |[Contributors](#contributors)|
+|[Change Log](#change-log)|
 |[Related Work](#related-work)|
 
 
 
 ## Why Should I Use CrossHair?
 
 **More precision.** Commonly, we care about more than just the type. Is it really any integer, or is it a **positive** integer? Is it any list, or does it have to be a non-empty list? CrossHair gives you that precision:
@@ -87,15 +90,15 @@
 
 You can find examples in the [examples/](https://github.com/pschanely/CrossHair/tree/master/crosshair/examples) directory 
 and try it in your browser at [crosshair-web.org](https://crosshair-web.org).
 
 
 ## Get Started
 
-> **_NOTE:_**  CrossHair is in a highly experimental state right now. If you're using it, it's because you want it to succeed, want to help, or are just interested in the technology.
+> **_NOTE:_**  CrossHair is in an experimental state right now. If you're using it, it's because you want it to succeed, want to help, or are just interested in the technology.
 
 CrossHair is supported only on Python 3.7+ and only on CPython (the most common Python implementation).
 
 Inside the development environment of the code you want to analyze (virtual environment, conda environment, etc), install:
 ```shell
 pip install crosshair-tool
 ```
@@ -119,22 +122,24 @@
 
 If you make a plugin for your favorite editor (please do!), submit a pull request to add it above. The `crosshair check [FILENAME]` command will yield results in the same format as the mypy type checker. (a non-zero exit for for errors, and lines formatted as `{FILENAME}:{LINE_NUMBER}:error:{MESSAGE}`)
 
 ## Limitations
 
 A (wildly incomplete) list of present limitations. Some of these will be lifted over time (your help is welcome!); some may never be lifted.
 
+* Be aware that the absence of a counterexample does not guarantee that the property holds.
 * Symbolic values are implemented as Python proxy values. CrossHair monkey-patches the system to maintain a good illusion, but the illusion is not complete. For example,
   * Code that cares about the identity values (x is y) may not be correctly analyzed.
   * Code that cares about the types of values may not be correctly analyzed.
 * Only function and class definitions at the top level are analyzed. (i.e. not when nested inside other functions/classes)
 * Only deteministic behavior can be analyzed. (your code always does the same thing when starting with the same values)
   * CrossHair may produce a `NotDeterministic` error when it detects this.
+* Be careful: CrossHair will actually run your code and may apply any arguments to it.
+  * If you run CrossHair on code calling [shutil.rmtree](https://docs.python.org/3/library/shutil.html#shutil.rmtree), you **will** destroy your filesystem.
 * Comsuming values of an iterator/generator in a pre- or post-condition will produce [unexpected behavior](https://github.com/pschanely/CrossHair/issues/9).
-* Be aware that the absence of a counterexample does not guarantee that the property holds.
 * SMT sovlers have very different perspectives on hard problems and easy problems than humans.
   * Be prepared to be surprised both by what CrossHair can tell you, and what it cannot.
 
 ## How Can I Help?
 
 * [Try it out](#get-started) on your own python project! Be communicative about what does and doesn't work.
 * Participate (or just lurk) in the [gitter chat](https://gitter.im/Cross_Hair/Lobby).
@@ -146,18 +151,26 @@
 
 ## Contributors
 
 * [**Phil Schanely**](https://twitter.com/pschanely)
 * [**Edward Haigh**](https://github.com/oneEdoubleD)
 * [**Saul Shanabrook**](https://github.com/saulshanabrook/)
 
+## Change Log
+
+0.0.9
+* Introduce [the diffbehavior command](doc/diff_behavior.md) which finds inputs that distinguish the behavior of two functions.
+* Upgrade to the latest release of z3 (4.8.9.0)
+* Fix [an installation error](https://github.com/pschanely/CrossHair/issues/41) on windows.
+* Fix a variety of other bugs.
+
 ## Related Work
 
 |Technology|Relation|
 |---------:|:-------|
 | [dependent types](https://en.wikipedia.org/wiki/Dependent_type), [refinement types](https://en.wikipedia.org/wiki/Refinement_type) | CrossHair aims to provide many of the same capabilities as these advanced type systems. CrossHair is easier to learn (because it is just python), but is incomplete (it can't always tell you whether a condition holds). |
-| [design by contract](https://en.wikipedia.org/wiki/Design_by_contract) | Unlike other systems and tools for contracts, CrossHair attempts to verify pre- and post-conditions before you run them. |
+| [design by contract](https://en.wikipedia.org/wiki/Design_by_contract) | Unlike most tools for contracts, CrossHair attempts to verify pre-conditions and post-conditions before you run them. |
 | [fuzz testing](https://en.wikipedia.org/wiki/Fuzzing), [QuickCheck](https://en.wikipedia.org/wiki/QuickCheck), [property testing](https://en.wikipedia.org/wiki/Property_testing), [Hypothesis](https://hypothesis.readthedocs.io/) | CrossHair has many of the same goals as these tools. However, CrossHair uses an SMT solver to find inputs rather than the (typically) randomized approaches that these tools use. |
 | [concolic testing](https://en.wikipedia.org/wiki/Concolic_testing) | State-of-the-art fuzz testers employ SMT solvers in a similar fashion as CrossHair. |
 | [SMT solvers](https://en.wikipedia.org/wiki/Satisfiability_modulo_theories) | SMT solvers power many of the tools in this table. CrossHair uses [Z3](https://github.com/Z3Prover/z3). |
 | [angr](https://angr.io), [klee](https://klee.github.io/) | Symbolic execution of **binary** code. Unlike these tools, CrossHair models the semantics of Python directly. |
 | [PyExZ3](https://github.com/thomasjball/PyExZ3), [pySim](https://github.com/bannsec/pySym), [PEF](https://git.cs.famaf.unc.edu.ar/dbarsotti/pef) | Take approaches that are very similar to CrossHair, in various states of completeness. CrossHair is generally more perscriptive or product-like than these tools. |
```

### Comparing `crosshair-tool-0.0.8/crosshair/abcstring.py` & `crosshair-tool-0.0.9/crosshair/abcstring.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/condition_parser_test.py` & `crosshair-tool-0.0.9/crosshair/enforce_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,137 @@
 import unittest
-from typing import cast, Generic, Optional, List, TypeVar
 
-from crosshair.condition_parser import *
+from crosshair.condition_parser import Pep316Parser
+from crosshair.enforce import *
+from crosshair.util import set_debug
+from typing import IO
 
 
-class Foo:
-    """A thingy.
-
-    Examples::
-        >>> 'blah'
-        'blah'
-
-    inv:: self.x >= 0
-
-    inv:
-        # a blank line with no indent is ok:
-
-        self.y >= 0
-    notasection:
-        self.z >= 0
-    """
-    x: int
-
-    def isready(self) -> bool:
-        """
-        Checks for readiness
-
-        post[]::
-            __return__ == (self.x == 0)
-        """
-        return self.x == 0
-
-
-def single_line_condition(x: int) -> int:
-    ''' post: __return__ >= x '''
-    return x
-
-
-def implies_condition(record: dict) -> object:
-    ''' post: implies('override' in record, _ == record['override']) '''
-    return record['override'] if 'override' in record else 42
-
-
-def raises_condition(record: dict) -> object:
+def foo(x: int) -> int:
     '''
-    raises: KeyError, OSError # comma , then junk
+    pre: 0 <= x <= 100
+    post: _ > x
     '''
-    raise KeyError('')
-
+    return x * 2
 
-def with_invalid_type_annotation(x: 'TypeThatIsNotDefined'):
-    pass
 
-class BaseClassExample:
+class Pokeable:
     '''
-    inv: True
+    inv: self.x >= 0
     '''
+    x: int = 1
 
+    def poke(self) -> None:
+        self.x += 1
 
-class SubClassExample(BaseClassExample):
-    def foo(self) -> int:
+    def pokeby(self, amount: int) -> None:
         '''
-        post: False
+        pre: amount >= 0
         '''
-        return 5
+        self.x += amount
 
 
-class ConditionParserTest(unittest.TestCase):
+def same_stream(stream: IO) -> IO:
+    ''' post: __old__.stream == _ '''
+    # It isn't possible to copy `stream` to make it available in `__old__`.
+    # In this case, enforcement will fail because __old__ won't contain it.
+    return stream
+
+class CoreTest(unittest.TestCase):
+
+    def test_enforce_and_unenforce(self) -> None:
+        env = {'foo': foo, 'bar': lambda x: x, 'baz': 42}
+        backup = env.copy()
+        with EnforcedConditions(Pep316Parser(), env, interceptor=lambda f: (lambda x: x * 3)):
+            self.assertIs(env['bar'], backup['bar'])
+            self.assertIs(env['baz'], 42)
+            self.assertIsNot(env['foo'], backup['foo'])
+            self.assertEqual(env['foo'](50), 150)  # type:ignore
+        self.assertIs(env['foo'], backup['foo'])
+
+    def test_enforce_conditions(self) -> None:
+        env = {'foo': foo}
+        self.assertEqual(foo(-1), -2)  # unchecked
+        with EnforcedConditions(Pep316Parser(), env):
+            self.assertEqual(env['foo'](50), 100)
+            with self.assertRaises(PreconditionFailed):
+                env['foo'](-1)
+            with self.assertRaises(PostconditionFailed):
+                env['foo'](0)
+
+    def test_class_enforce(self) -> None:
+        env = {'Pokeable': Pokeable}
+        old_id = id(Pokeable.poke)
+        Pokeable().pokeby(-1)  # no exception (yet!)
+        with EnforcedConditions(Pep316Parser(), env):
+            self.assertNotEqual(id(env['Pokeable'].poke), old_id)
+            Pokeable().poke()
+            with self.assertRaises(PreconditionFailed):
+                Pokeable().pokeby(-1)
+        self.assertEqual(id(env['Pokeable'].poke), old_id)
+
+    def test_enforce_on_uncopyable_value(self) -> None:
+        env = {'l': same_stream}
+        self.assertIs(same_stream(sys.stdout), sys.stdout)
+        with EnforcedConditions(Pep316Parser(), env):
+            with self.assertRaises(AttributeError):
+                env['l'](sys.stdout)
+
+class BaseFooable:
+    def foo(self, x: int):
+        ''' pre: x > 100 '''
+    def foo_only_in_super(self, x: int):
+        ''' pre: x > 100 '''
+    @classmethod
+    def class_foo(cls, x: int):
+        ''' pre: x > 100 '''
+    @staticmethod
+    def static_foo(x: int):
+        ''' pre: x > 100 '''
+
+class DerivedFooable(BaseFooable):
+    def foo(self, x: int):
+        ''' pre: x > 0 '''
+    @classmethod
+    def class_foo(cls, x: int):
+        ''' pre: x > 0 '''
+    @staticmethod
+    def static_foo(x: int):
+        ''' pre: x > 0 '''
+
+
+class TrickyCasesTest(unittest.TestCase):
+
+    def test_attrs_restored_properly(self) -> None:
+        orig_class_dict = DerivedFooable.__dict__.copy()
+        with EnforcedConditions(Pep316Parser(), {'DerivedFooable': DerivedFooable}):
+            pass
+        for k, v in orig_class_dict.items():
+            self.assertIs(DerivedFooable.__dict__[k], v, f'member "{k}" changed afer encforcement')
+
+    def test_enforcement_of_class_methods(self) -> None:
+        with EnforcedConditions(Pep316Parser(), {'DerivedFooable': BaseFooable}):
+            with self.assertRaises(PreconditionFailed):
+                BaseFooable.class_foo(50)
+        with EnforcedConditions(Pep316Parser(), {'DerivedFooable': DerivedFooable}):
+            DerivedFooable.class_foo(50)
+
+    def test_enforcement_of_static_methods(self) -> None:
+        with EnforcedConditions(Pep316Parser(), {'DerivedFooable': DerivedFooable}):
+            DerivedFooable.static_foo(50)
+            with self.assertRaises(PreconditionFailed):
+                BaseFooable.static_foo(50)
+
+    def test_super_method_enforced(self) -> None:
+        with EnforcedConditions(Pep316Parser(), {'DerivedFooable': DerivedFooable}):
+            with self.assertRaises(PreconditionFailed):
+                DerivedFooable().foo_only_in_super(50)
+            with self.assertRaises(PreconditionFailed):
+                DerivedFooable().foo(-1)
+            # Derived class has a weaker precondition, so this is OK:
+            DerivedFooable().foo(50)
 
-    def test_class_parse(self) -> None:
-        class_conditions = get_class_conditions(Foo)
-        self.assertEqual(set([c.expr_source for c in class_conditions.inv]),
-                         set(['self.x >= 0', 'self.y >= 0']))
-        self.assertEqual(set(class_conditions.methods.keys()),
-                         set(['isready']))
-        method = class_conditions.methods['isready']
-        self.assertEqual(set([c.expr_source for c in method.pre]),
-                         set(['self.x >= 0', 'self.y >= 0']))
-        self.assertEqual(set([c.expr_source for c in method.post]),
-                         set(['__return__ == (self.x == 0)', 'self.x >= 0', 'self.y >= 0']))
-
-    def test_single_line_condition(self) -> None:
-        conditions = get_fn_conditions(single_line_condition)
-        assert conditions is not None
-        self.assertEqual(set([c.expr_source for c in conditions.post]),
-                         set(['__return__ >= x']))
-
-    def test_implies_condition(self) -> None:
-        conditions = get_fn_conditions(implies_condition)
-        assert conditions is not None
-        # This shouldn't explode (avoid a KeyError on record['override']):
-        conditions.post[0].evaluate({'record': {}, '_': 0})
-
-    def test_raises_condition(self) -> None:
-        conditions = get_fn_conditions(raises_condition)
-        assert conditions is not None
-        self.assertEqual([], list(conditions.syntax_messages()))
-        self.assertEqual(set([KeyError, OSError]), conditions.raises)
-
-    def test_invariant_is_inherited(self) -> None:
-        class_conditions = get_class_conditions(SubClassExample)
-        self.assertEqual(set(class_conditions.methods.keys()), set(['foo']))
-        method = class_conditions.methods['foo']
-        self.assertEqual(set([c.expr_source for c in method.pre]),
-                         set(['True']))
-        self.assertEqual(set([c.expr_source for c in method.post]),
-                         set(['True', 'False']))
-
-    def test_builtin_conditions_are_null(self) -> None:
-        self.assertIsNone(get_fn_conditions(zip))
-
-    def test_fn_globals_on_builtin(self) -> None:
-        self.assertIs(fn_globals(zip), builtins.__dict__)
-
-    def test_resolve_signature(self) -> None:
-        sig, err = resolve_signature(with_invalid_type_annotation)
-        self.assertIsNotNone(err)
-        self.assertEqual("name 'TypeThatIsNotDefined' is not defined", err.message)
-        self.assertIsNone(sig)
-
-    def test_conditions_with_closure_references_and_string_type(self) -> None:
-        # This is a function that refers to something in its closure.
-        # Ensure we can still look up string-based types:
-        def referenced_fn():
-            return 4
-        def fn_with_closure(foo: "Foo"):
-            referenced_fn()
-        # Ensure we don't error trying to resolve "Foo":
-        get_fn_conditions(fn_with_closure)
-
-    def test_empty_vs_missing_mutations(self) -> None:
-        self.assertIsNone(parse_sections([(1,'post: True')], ('post',), '').mutable_expr)
-        self.assertEqual('', parse_sections([(1,'post[]: True')], ('post',), '').mutable_expr)
-
-    def test_set_self_type(self) -> None:
-        sig = inspect.signature(Foo.isready)
-        typed_sig = set_self_type(sig, Foo) 
-        self.assertEqual(typed_sig.parameters['self'].annotation, Foo)
 
 if __name__ == '__main__':
+    if ('-v' in sys.argv) or ('--verbose' in sys.argv):
+        set_debug(True)
     unittest.main()
```

### Comparing `crosshair-tool-0.0.8/crosshair/core.py` & `crosshair-tool-0.0.9/crosshair/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 
+# TODO: a hypothesis function def breaks crosshair when analyzing the file
 # TODO: Test with "from __future__ import annotations"
 # TODO: Test string-based typing annotations
+# TODO: Test @property decorated accessors with contracts
+# TODO: handle generic function signatures created by @overload decorators
 
 # *** Not prioritized for v0 ***
 # TODO: increase test coverage: TypeVar('T', int, str) vs bounded type vars
 # TODO: do not claim "unable to meet preconditions" when we have path timeouts
 # TODO: consider raises conditions (guaranteed to raise, guaranteed to not raise?)
 # TODO: precondition strengthening ban (Subclass constraint rule)
 # TODO: double-check counterexamples
@@ -35,49 +38,72 @@
 import typing
 
 import forbiddenfruit  # type: ignore
 import typing_inspect  # type: ignore
 import z3  # type: ignore
 
 from crosshair import dynamic_typing
-from crosshair.condition_parser import get_fn_conditions, get_class_conditions, ConditionExpr, Conditions, fn_globals, resolve_signature
-from crosshair.enforce import EnforcedConditions, PostconditionFailed
-from crosshair.statespace import TrackingStateSpace, StateSpace, HeapRef, SnapshotRef, SearchTreeNode, model_value_to_python, VerificationStatus, IgnoreAttempt, SinglePathNode, CallAnalysis, MessageType, AnalysisMessage
-from crosshair.util import CrosshairInternal, UnexploredPath, IdentityWrapper, AttributeHolder, CrosshairUnsupported
-from crosshair.util import debug, eval_friendly_repr, frame_summary_for_fn, samefile, set_debug
-from crosshair.util import extract_module_from_file, name_of_type, walk_qualname
+
+from crosshair.condition_parser import fn_globals
+from crosshair.condition_parser import CompositeConditionParser
+from crosshair.condition_parser import ConditionParser
+from crosshair.condition_parser import Pep316Parser
+from crosshair.condition_parser import IcontractParser
+from crosshair.condition_parser import resolve_signature
+from crosshair.condition_parser import Conditions
+from crosshair.condition_parser import ConditionExpr
+from crosshair.enforce import EnforcedConditions
+from crosshair.enforce import PostconditionFailed
+from crosshair.statespace import context_statespace
+from crosshair.statespace import optional_context_statespace
+from crosshair.statespace import AnalysisMessage
+from crosshair.statespace import CallAnalysis
+from crosshair.statespace import HeapRef
+from crosshair.statespace import MessageType
+from crosshair.statespace import SinglePathNode
+from crosshair.statespace import StateSpace
+from crosshair.statespace import StateSpaceContext
+from crosshair.statespace import TrackingStateSpace
+from crosshair.statespace import VerificationStatus
+from crosshair.util import debug
+from crosshair.util import eval_friendly_repr
+from crosshair.util import extract_module_from_file
+from crosshair.util import frame_summary_for_fn
+from crosshair.util import is_pure_python
+from crosshair.util import name_of_type
+from crosshair.util import samefile
+from crosshair.util import walk_qualname
+from crosshair.util import AttributeHolder
+from crosshair.util import CrosshairInternal
+from crosshair.util import CrosshairUnsupported
+from crosshair.util import DynamicScopeVar
+from crosshair.util import UnexploredPath
+from crosshair.util import IdentityWrapper
+from crosshair.util import IgnoreAttempt
 from crosshair.type_repo import get_subclass_map
 
 
 _MISSING = object()
 
-def is_pure(obj: object) -> bool:
-    if isinstance(obj, type):
-        return True if '__dict__' in dir(obj) else hasattr(obj, '__slots__')
-    elif callable(obj):
-        return inspect.isfunction(obj)  # isfunction selects "user-defined" functions only
-    else:
-        return True
-
 # TODO Unify common logic here with EnforcedConditions?
 class Patched:
     def __init__(self, enabled: Callable[[], bool]):
         self._patches = _PATCH_REGISTRATIONS
         self._enabled = enabled
         self._originals: Dict[IdentityWrapper, Dict[str, object]] = collections.defaultdict(dict)
 
     def set(self, target: object, key: str, value: object):
-        if is_pure(target):
+        if is_pure_python(target):
             target.__dict__[key] = value
         else:
             forbiddenfruit.curse(target, key, value)
 
     def patch(self, target: object, key: str, patched_fn: Callable):
         enabled = self._enabled
-        orig_fn = getattr(target, key, None)
+        orig_fn = target.__dict__.get(key, None)
         if orig_fn is None:
             self.set(target, key, patched_fn)
         else:
             def call_if_enabled(*a, **kw):
                 if enabled():
                     return patched_fn(*a, **kw)
                 else:
@@ -95,21 +121,21 @@
 
     def __exit__(self, exc_type, exc_value, tb) -> None:
         for target_wrapper, members in self._patches.items():
             container = target_wrapper.get()
             originals = self._originals[target_wrapper]
             for key, orig_val in originals.items():
                 if orig_val is _MISSING:
-                    delattr(container, key)
+                    del container.__dict__[key]
                 else:
                     self.set(container, key, orig_val)
 
 
 class ExceptionFilter:
-    analysis: 'CallAnalysis'
+    analysis: CallAnalysis
     ignore: bool = False
     ignore_with_confirmation: bool = False
     user_exc: Optional[Tuple[Exception, traceback.StackSummary]] = None
     expected_exceptions: Tuple[Type[BaseException], ...]
 
     def __init__(self, expected_exceptions: FrozenSet[Type[BaseException]] = frozenset()):
         self.expected_exceptions = (NotImplementedError,) + tuple(expected_exceptions)
@@ -124,19 +150,20 @@
         if isinstance(exc_value, (PostconditionFailed, IgnoreAttempt)):
             if isinstance(exc_value, PostconditionFailed):
                 # Postcondition : although this indicates a problem, it's with a
                 # subroutine; not this function.
                 # Usualy we want to ignore this because it will be surfaced more locally
                 # in the subroutine.
                 debug(
-                    F'Ignoring based on internal failed post condition: {exc_value}')
+                    f'Ignoring based on internal failed post condition: {exc_value}')
             self.ignore = True
             self.analysis = CallAnalysis()
             return True
         if isinstance(exc_value, self.expected_exceptions):
+            debug(f'Hit expected exception: {exc_value}')
             self.ignore = True
             self.analysis = CallAnalysis(VerificationStatus.CONFIRMED)
             return True
         if isinstance(exc_value, TypeError):
             exc_str = str(exc_value)
             if ('SmtStr' in exc_str or
                 'SmtInt' in exc_str or
@@ -213,36 +240,36 @@
         a = map(realize, a)
         kw = {k:realize(v) for (k, v) in kw.items()}
         return fn(*a, **kw)
     functools.update_wrapper(realizer, fn)
     return realizer
 
 _IMMUTABLE_TYPES = (int, float, complex, bool, tuple, frozenset, type(None))
-def forget_contents(value: object, space: StateSpace):
+def forget_contents(value: object):
     # TODO: pretty sure this doesn't work; need tests here.
     if hasattr(value, '__ch_forget_contents__'):
-        value.__ch_forget_contents__(space)  # type: ignore
+        value.__ch_forget_contents__()  # type: ignore
     elif hasattr(value, '__dict__'):
         for subvalue in value.__dict__.values():
-            forget_contents(subvalue, space)
+            forget_contents(subvalue)
     elif isinstance(value, _IMMUTABLE_TYPES):
         return # immutable
     else:
         # TODO: handle mutable values without __dict__
         raise CrosshairUnsupported
 
 
 class SmtProxyMarker(CrossHairValue):
     def __ch_pytype__(self):
         bases = type(self).__bases__
         assert len(bases) == 2 and bases[0] is SmtProxyMarker
         return bases[1]
-    def __ch_forget_contents__(self, space: StateSpace):
+    def __ch_forget_contents__(self):
         cls = self.__ch_pytype__()
-        clean = proxy_for_type(cls, space, space.uniq())
+        clean = proxy_for_type(cls, context_statespace().uniq())
         for name, val in self.__dict__.items():
             self.__dict__[name] = clean.__dict__[name]
 
 
 _SMT_PROXY_TYPES: Dict[type, type] = {}
 
 def get_smt_proxy_type(cls: type) -> type:
@@ -260,28 +287,27 @@
             if 'is not an acceptable base type' in str(e):
                 raise CrosshairUnsupported(f'Cannot subclass {cls_name}')
             else:
                 raise
         _SMT_PROXY_TYPES[cls] = proxy_cls
     return _SMT_PROXY_TYPES[cls]
 
-def make_fake_object(statespace: StateSpace, cls: type, varname: str) -> object:
+def make_fake_object(cls: type, varname: str) -> object:
     constructor = get_smt_proxy_type(cls)
-    debug(constructor)
     try:
         proxy = constructor()
     except TypeError as e:
         # likely the type has a __new__ that expects arguments
         raise CrosshairUnsupported(f'Unable to proxy {name_of_type(cls)}: {e}')
     for name, typ in get_type_hints(cls).items():
         origin = getattr(typ, '__origin__', None)
         if origin is Callable:
             continue
-        value = proxy_for_type(typ, statespace, varname +
-                               '.' + name + statespace.uniq())
+        value = proxy_for_type(typ, varname +
+                               '.' + name + context_statespace().uniq())
         object.__setattr__(proxy, name, value)
     return proxy
 
 
 def choose_type(space: StateSpace, from_type: Type) -> Type:
     subtypes = get_subclass_map()[from_type]
     # Note that this is written strangely to leverage the default
@@ -291,98 +317,105 @@
     for subtype in subtypes[:-1]:
         if not space.smt_fork():
             return choose_type(space, subtype)
     return choose_type(space, subtypes[-1])
 
 
 def get_constructor_params(cls: Type) -> Optional[Iterable[inspect.Parameter]]:
-    # TODO inspect __new__ as well
+    new_fn = cls.__new__
     init_fn = cls.__init__
-    if init_fn is object.__init__:
+    if (new_fn is not object.__new__ and
+        # Some superclasses like Generic[T] define __new__ with typless (*a,**kw)
+        # args. Skip if we don't have types on __new__.
+        # TODO: merge the type signatures of __init__ and __new__, pulling the
+        # most specific types from each.
+        len(get_type_hints(new_fn)) > 0):
+        sig, resolution_err = resolve_signature(new_fn)
+    elif init_fn is not object.__init__:
+        sig, resolution_err = resolve_signature(init_fn)
+    else:
         return ()
-    init_sig, resolution_err = resolve_signature(init_fn)
-    if init_sig is None:
+    if sig is None:
         return None
-    return list(init_sig.parameters.values())[1:]
+    return list(sig.parameters.values())[1:]
 
-def proxy_class_as_concrete(typ: Type, statespace: StateSpace,
-                            varname: str) -> object:
+def proxy_class_as_concrete(typ: Type, varname: str) -> object:
     '''
     Try aggressively to create an instance of a class with symbolic members.
     '''
     data_members = get_type_hints(typ)
 
     # Special handling for some magical types:
     if issubclass(typ, tuple):
-        args = {k: proxy_for_type(t, statespace, varname + '.' + k)
+        args = {k: proxy_for_type(t, varname + '.' + k)
                 for (k, t) in data_members.items()}
         return typ(**args) # type: ignore
-    elif sys.version_info >= (3, 8) and type(typ) is typing._TypedDictMeta:
+    elif sys.version_info >= (3, 8) and type(typ) is typing._TypedDictMeta:  # type: ignore
         optional_keys = getattr(typ, "__optional_keys__", ())
         keys = (k for k in data_members.keys()
-                if k not in optional_keys or statespace.smt_fork())
-        return {k: proxy_for_type(data_members[k], statespace,
+                if k not in optional_keys or context_statespace().smt_fork())
+        return {k: proxy_for_type(data_members[k],
                                   varname + '.' + k) for k in keys}
     constructor_params = get_constructor_params(typ)
     if constructor_params is None:
         debug(f'unable to create concrete instance of {typ} due to bad constructor')
         return _MISSING
     EMPTY = inspect.Parameter.empty
     args = {}
     for param in constructor_params:
         name = param.name
         smtname = varname + '.' + name
         annotation = param.annotation
         if annotation is not EMPTY:
-            args[name] = proxy_for_type(annotation, statespace, smtname)
+            args[name] = proxy_for_type(annotation, smtname)
         else:
             if param.default is EMPTY:
                 debug('unable to create concrete instance of', typ,
                       'due to lack of type annotation on', name)
                 return _MISSING
             else:
                 # TODO: consider whether we should fall back to a proxy
                 # instead of letting this slide. Or try both paths?
                 pass
     try:
         obj = typ(**args)
     except BaseException as e:
-        debug('unable to create concrete proxy with init:', e)
+        debug(f'unable to create concrete instance of {typ} with init: {e}')
         return _MISSING
 
     # Additionally, for any typed members, ensure that they are also
     # symbolic. (classes sometimes have valid states that are not directly
     # constructable)
     for (key, typ) in data_members.items():
         if isinstance(getattr(obj, key, None), CrossHairValue):
             continue
-        symbolic_value = proxy_for_type(typ, statespace, varname + '.' + key)
+        symbolic_value = proxy_for_type(typ, varname + '.' + key)
         try:
             setattr(obj, key, symbolic_value)
         except Exception as e:
             debug('Unable to assign symbolic value to concrete class:', e)
             # TODO: consider whether we should fall back to a proxy
             # instead of letting this slide. Or try both paths?
     return obj
 
 
-def proxy_for_class(typ: Type, space: StateSpace, varname: str, meet_class_invariants: bool) -> object:
+def proxy_for_class(typ: Type, varname: str, meet_class_invariants: bool) -> object:
     # if the class has data members, we attempt to create a concrete instance with
     # symbolic members; otherwise, we'll create an object proxy that emulates it.
-    obj = proxy_class_as_concrete(typ, space, varname)
+    obj = proxy_class_as_concrete(typ, varname)
     if obj is _MISSING:
         debug('Creating', typ, 'as an independent proxy class')
-        obj = make_fake_object(space, typ, varname)
+        obj = make_fake_object(typ, varname)
     else:
         debug('Creating', typ, 'with symbolic attribute assignments')
-    class_conditions = get_class_conditions(typ)
+    class_conditions = _CALLTREE_PARSER.get().get_class_conditions(typ)
     # symbolic custom classes may assume their invariants:
     if meet_class_invariants and class_conditions is not None:
         for inv_condition in class_conditions.inv:
-            if inv_condition.expr is None:
+            if inv_condition.evaluate is None:
                 continue
             isok = False
             with ExceptionFilter() as efilter:
                 isok = inv_condition.evaluate({'self': obj})
             if efilter.user_exc:
                 raise IgnoreAttempt(
                     f'Class proxy could not meet invariant "{inv_condition.expr_source}" on '
@@ -411,46 +444,48 @@
                   creator: Union[Type, Callable]) -> None:
     assert typ is origin_of(typ), \
             f'Only origin types may be registered, not "{typ}": try "{origin_of(typ)}" instead.'
     if typ in _SIMPLE_PROXIES:
         raise CrosshairInternal(f'Duplicate type "{typ}" registered')
     _SIMPLE_PROXIES[typ] = creator
 
-def proxy_for_type(typ: Type, space: StateSpace, varname: str,
+def proxy_for_type(typ: Type, varname: str,
                    meet_class_invariants=True,
                    allow_subtypes=False) -> object:
+    space = context_statespace()
     typ = normalize_pytype(typ)
     origin = origin_of(typ)
     type_args = type_args_of(typ)
     # special cases
     if isinstance(typ, type) and issubclass(typ, enum.Enum):
         enum_values = list(typ)  # type:ignore
         for enum_value in enum_values[:-1]:
             if space.smt_fork():
                 return enum_value
         return enum_values[-1]
     proxy_factory = _SIMPLE_PROXIES.get(origin)
     if proxy_factory:
         def recursive_proxy_factory(t: Type):
-            return proxy_for_type(t, space, varname + space.uniq(),
+            return proxy_for_type(t, varname + space.uniq(),
                                   allow_subtypes=allow_subtypes)
         recursive_proxy_factory.space = space  # type: ignore
         recursive_proxy_factory.pytype = typ  # type: ignore
         recursive_proxy_factory.varname = varname  # type: ignore
         return proxy_factory(recursive_proxy_factory, *type_args)
     if allow_subtypes and typ is not object:
         typ = choose_type(space, typ)
-    return proxy_for_class(typ, space, varname, meet_class_invariants)
+    return proxy_for_class(typ, varname, meet_class_invariants)
 
 
-def gen_args(sig: inspect.Signature, statespace: StateSpace) -> inspect.BoundArguments:
+def gen_args(sig: inspect.Signature) -> inspect.BoundArguments:
     args = sig.bind_partial()
+    space = context_statespace()
     for param in sig.parameters.values():
-        smt_name = param.name + statespace.uniq()
-        proxy_maker = lambda typ, **kw: proxy_for_type(typ, statespace, smt_name, allow_subtypes=True, **kw)
+        smt_name = param.name + space.uniq()
+        proxy_maker = lambda typ, **kw: proxy_for_type(typ, smt_name, allow_subtypes=True, **kw)
         has_annotation = (param.annotation != inspect.Parameter.empty)
         value: object
         if param.kind == inspect.Parameter.VAR_POSITIONAL:
             if has_annotation:
                 varargs_type = List[param.annotation]  # type: ignore
                 value = proxy_maker(varargs_type)
             else:
@@ -467,18 +502,18 @@
         else:
             is_self = param.name == 'self'
             # Object parameters should meet thier invariants iff they are not the
             # class under test ("self").
             meet_class_invariants = not is_self
             allow_subtypes = not is_self
             if has_annotation:
-                value = proxy_for_type(param.annotation, statespace, smt_name,
+                value = proxy_for_type(param.annotation, smt_name,
                                        meet_class_invariants, allow_subtypes)
             else:
-                value = proxy_for_type(cast(type, Any), statespace, smt_name,
+                value = proxy_for_type(cast(type, Any), smt_name,
                                        meet_class_invariants, allow_subtypes)
         debug('created proxy for', param.name, 'as type:', type(value))
         args.arguments[param.name] = value
     return args
 
 _UNABLE_TO_REPR = '<unable to repr>'
 def message_sort_key(m: AnalysisMessage) -> tuple:
@@ -500,30 +535,77 @@
         else:
             self.by_pos[key] = message
 
     def get(self) -> List[AnalysisMessage]:
         return [m for (k, m) in sorted(self.by_pos.items())]
 
 
+class AnalysisKind(enum.Enum):
+    PEP316 = 'PEP316'
+    icontract = 'icontract'
+    asserts = 'asserts'
+    hypothesis = 'hypothesis'
+
+
 @dataclass
 class AnalysisOptions:
     per_condition_timeout: float = 1.5
     per_path_timeout: float = 0.75
+    max_iterations: int = sys.maxsize  # TODO: use during check and expose on command line
     report_all: bool = False
+    analysis_kind: Sequence[AnalysisKind] = (AnalysisKind.PEP316,)
+
+    # Lazily-initialized values
+    _condition_parser: Optional[ConditionParser] = None
 
     # Transient members (not user-configurable):
     deadline: float = float('NaN')
     stats: Optional[collections.Counter] = None
 
+    # Helpers
+    def condition_parser(self) -> ConditionParser:
+        if self._condition_parser is None:
+            debug('Using parsers: ', self.analysis_kind)
+            _PARSER_MAP = {
+                AnalysisKind.PEP316: Pep316Parser,
+                AnalysisKind.icontract: IcontractParser,
+            }
+            self._condition_parser = CompositeConditionParser()
+            self._condition_parser.parsers.extend(
+                _PARSER_MAP[k](self._condition_parser) for k in self.analysis_kind)
+        assert self._condition_parser is not None
+        return self._condition_parser
+
+    def split_limits(
+            self, priority: float) -> Tuple['AnalysisOptions', 'AnalysisOptions']:
+        '''
+        pre: 0.0 <= priority <= 1.0
+        post: _[0].max_iterations + _[1].max_iterations == self.max_iterations
+        '''
+        options1 = replace(
+            self,
+            per_condition_timeout=self.per_condition_timeout * priority,
+            per_path_timeout=self.per_path_timeout * priority,
+            max_iterations=round(self.max_iterations * priority),
+            )
+        inv_priority = 1.0 - priority
+        options2 = replace(
+            self,
+            per_condition_timeout=self.per_condition_timeout * inv_priority,
+            per_path_timeout=self.per_path_timeout * inv_priority,
+            max_iterations=self.max_iterations - options1.max_iterations,
+        )
+        return (options1, options2)
+
     def incr(self, key: str):
         if self.stats is not None:
             self.stats[key] += 1
 
 
-_DEFAULT_OPTIONS = AnalysisOptions()
+DEFAULT_OPTIONS = AnalysisOptions()
 
 
 def analyzable_members(module: types.ModuleType) -> Iterator[Tuple[str, Union[Type, Callable]]]:
     module_name = module.__name__
     for name, member in inspect.getmembers(module):
         if not (inspect.isclass(member) or inspect.isfunction(member) or inspect.ismethod(member)):
             continue
@@ -531,26 +613,26 @@
             continue
         yield (name, member)
 
 
 def analyze_any(entity: object, options: AnalysisOptions) -> List[AnalysisMessage]:
     if inspect.ismethod(entity):
         # this should only happen for @classmethod; unwrap it:
-        entity = entity.__func__
+        entity = entity.__func__  # type: ignore
     if inspect.isclass(entity):
         return analyze_class(cast(Type, entity), options)
     elif inspect.isfunction(entity):
         self_class: Optional[type] = None
         fn = cast(Callable, entity)
         if fn.__name__ != fn.__qualname__:
             self_thing = walk_qualname(sys.modules[fn.__module__],
                                        fn.__qualname__.split('.')[-2])
             assert isinstance(self_thing, type)
             self_class = self_thing
-        return analyze_function(fn, options, self_type=self_class)
+        return analyze_function(fn, options, first_arg_type=self_class)
     elif inspect.ismodule(entity):
         return analyze_module(cast(types.ModuleType, entity), options)
     else:
         raise CrosshairInternal(
             'Entity type not analyzable: ' + str(type(entity)))
 
 
@@ -577,70 +659,72 @@
         if not samefile(message.filename, cls_file):
             return replace(message, filename=cls_file, line=cls_start_line)
         else:
             return message
     return clamp
 
 
-def analyze_class(cls: type, options: AnalysisOptions = _DEFAULT_OPTIONS) -> List[AnalysisMessage]:
+def analyze_class(cls: type, options: AnalysisOptions = DEFAULT_OPTIONS) -> List[AnalysisMessage]:
     debug('Analyzing class ', cls.__name__)
     messages = MessageCollector()
-    class_conditions = get_class_conditions(cls)
+    class_conditions = options.condition_parser().get_class_conditions(cls)
     for method, conditions in class_conditions.methods.items():
         if conditions.has_any():
             cur_messages = analyze_function(getattr(cls, method),
                                             options=options,
-                                            self_type=cls)
+                                            first_arg_type=cls)
             clamper = message_class_clamper(cls)
             messages.extend(map(clamper, cur_messages))
 
     return messages.get()
 
 
 def analyze_function(fn: Callable,
-                     options: AnalysisOptions = _DEFAULT_OPTIONS,
-                     self_type: Optional[type] = None) -> List[AnalysisMessage]:
+                     options: AnalysisOptions = DEFAULT_OPTIONS,
+                     first_arg_type: Optional[type] = None) -> List[AnalysisMessage]:
     debug('Analyzing ', fn.__name__)
     all_messages = MessageCollector()
 
-    if self_type is not None:
-        class_conditions = get_class_conditions(self_type)
+    if first_arg_type is not None:
+        class_conditions = options.condition_parser().get_class_conditions(first_arg_type)
         conditions = class_conditions.methods.get(fn.__name__)
         if conditions is None:
             debug('Skipping', fn.__name__, ' because it has no conditions')
             return []
     else:
-        conditions = get_fn_conditions(fn, self_type=self_type)
+        conditions = options.condition_parser().get_fn_conditions(fn, defining_class=first_arg_type)
         if conditions is None:
             debug('Skipping ', str(fn),
                   ': Unable to determine the function signature.')
             return []
 
-    for syntax_message in conditions.syntax_messages():
-        all_messages.append(AnalysisMessage(MessageType.SYNTAX_ERR,
-                                            syntax_message.message,
-                                            syntax_message.filename,
-                                            syntax_message.line_num, 0, ''))
-    conditions = conditions.compilable()
-    for post_condition in conditions.post:
-        messages = analyze_single_condition(fn, options, replace(
-            conditions, post=[post_condition]))
-        all_messages.extend(messages)
+    syntax_messages = list(conditions.syntax_messages())
+    if syntax_messages:
+        for syntax_message in syntax_messages:
+            all_messages.append(AnalysisMessage(MessageType.SYNTAX_ERR,
+                                                syntax_message.message,
+                                                syntax_message.filename,
+                                                syntax_message.line_num, 0, ''))
+    else:
+        for post_condition in conditions.post:
+            messages = analyze_single_condition(options, replace(
+                conditions, post=[post_condition]))
+            all_messages.extend(messages)
     return all_messages.get()
 
 
-def analyze_single_condition(fn: Callable,
-                             options: AnalysisOptions,
+def analyze_single_condition(options: AnalysisOptions,
                              conditions: Conditions) -> Sequence[AnalysisMessage]:
     debug('Analyzing postcondition: "', conditions.post[0].expr_source, '"')
     debug('assuming preconditions: ', ','.join(
         [p.expr_source for p in conditions.pre]))
-    options.deadline = time.time() + options.per_condition_timeout
+    options.deadline = time.monotonic() + options.per_condition_timeout
 
-    analysis = analyze_calltree(fn, options, conditions)
+    with _CALLTREE_PARSER.open(options.condition_parser()):
+        analysis = analyze_calltree(options, conditions)
 
     (condition,) = conditions.post
     addl_ctx = (' ' + condition.addl_context if condition.addl_context else '') + '.'
     if analysis.verification_status is VerificationStatus.UNKNOWN:
         message = 'Not confirmed' + addl_ctx
         analysis.messages = [AnalysisMessage(MessageType.CANNOT_CONFIRM, message,
                                              condition.filename, condition.line, 0, '')]
@@ -652,39 +736,37 @@
     return analysis.messages
 
 
 class ShortCircuitingContext:
     engaged = False
     intercepted = False
 
-    def __init__(self, space_getter: Callable[[], StateSpace]):
-        self.space_getter = space_getter
-
     def __enter__(self):
         assert not self.engaged
         self.engaged = True
 
     def __exit__(self, exc_type, exc_value, tb):
         assert self.engaged
         self.engaged = False
 
     def make_interceptor(self, original: Callable) -> Callable:
-        subconditions = get_fn_conditions(original)
+        subconditions = _CALLTREE_PARSER.get().get_fn_conditions(original)
         if subconditions is None:
             return original
         sig = subconditions.sig
 
         def wrapper(*a: object, **kw: Dict[str, object]) -> object:
             #debug('short circuit wrapper ', original)
-            if (not self.engaged) or self.space_getter().running_framework_code:
+            space = optional_context_statespace()
+            if (not self.engaged) or (not space) or space.running_framework_code:
                 return original(*a, **kw)
             # We *heavily* bias towards concrete execution, because it's often the case
             # that a single short-circuit will render the path useless. TODO: consider
             # decaying short-crcuit probability over time.
-            use_short_circuit = self.space_getter().fork_with_confirm_or_else(0.95)
+            use_short_circuit = space.fork_with_confirm_or_else(0.95)
             if not use_short_circuit:
                 #debug('short circuit: Choosing not to intercept', original)
                 return original(*a, **kw)
             try:
                 self.engaged = False
                 debug('short circuit: Short circuiting over a call to ', original)
                 self.intercepted = True
@@ -711,72 +793,75 @@
 
                 # adjust arguments that may have been mutated
                 assert subconditions is not None
                 bound = sig.bind(*a, **kw)
                 mutable_args = subconditions.mutable_args
                 for argname, arg in bound.arguments.items():
                     if mutable_args is None or argname in mutable_args:
-                        forget_contents(arg, self.space_getter())
+                        forget_contents(arg)
 
                 if return_type is type(None):
                     return None
                 # note that the enforcement wrapper ensures postconditions for us, so we
                 # can just return a free variable here.
-                return proxy_for_type(return_type, self.space_getter(), 'proxyreturn' + self.space_getter().uniq())
+                return proxy_for_type(return_type, 'proxyreturn' + space.uniq())
             finally:
                 self.engaged = True
         functools.update_wrapper(wrapper, original)
         return wrapper
 
+# Condition parsers may be needed at various places in the stack.
+# We configure them through the use of a magic threadlocal value:
+_CALLTREE_PARSER = DynamicScopeVar(ConditionParser, 'calltree parser')
+
 @dataclass
 class CallTreeAnalysis:
     messages: Sequence[AnalysisMessage]
     verification_status: VerificationStatus
     num_confirmed_paths: int = 0
 
-
-def analyze_calltree(fn: Callable,
-                     options: AnalysisOptions,
+def analyze_calltree(options: AnalysisOptions,
                      conditions: Conditions) -> CallTreeAnalysis:
+    fn = conditions.fn
     debug('Begin analyze calltree ', fn.__name__)
 
     all_messages = MessageCollector()
     search_root = SinglePathNode(True)
     space_exhausted = False
     failing_precondition: Optional[ConditionExpr] = conditions.pre[0] if conditions.pre else None
     failing_precondition_reason: str = ''
     num_confirmed_paths = 0
 
-    cur_space: List[StateSpace] = [cast(StateSpace, None)]
-    short_circuit = ShortCircuitingContext(lambda: cur_space[0])
     _ = get_subclass_map()  # ensure loaded
+    short_circuit = ShortCircuitingContext()
     top_analysis: Optional[CallAnalysis] = None
     enforced_conditions = EnforcedConditions(
+        options.condition_parser(),
         fn_globals(fn), builtin_patches(),
         interceptor=short_circuit.make_interceptor)
     def in_symbolic_mode():
-        return (cur_space[0] is not None and
-                not cur_space[0].running_framework_code)
+        space = optional_context_statespace()
+        return space and not space.running_framework_code
     patched = Patched(in_symbolic_mode)
     with enforced_conditions, patched, enforced_conditions.disabled_enforcement():
-        for i in itertools.count(1):
-            start = time.time()
+        for i in range(1, options.max_iterations + 1):
+            start = time.monotonic()
             if start > options.deadline:
                 debug('Exceeded condition timeout, stopping')
                 break
             options.incr('num_paths')
             debug('Iteration ', i)
             space = TrackingStateSpace(execution_deadline=start + options.per_path_timeout,
                                        model_check_timeout=options.per_path_timeout / 2,
                                        search_root=search_root)
-            cur_space[0] = space
             try:
                 # The real work happens here!:
-                call_analysis = attempt_call(
-                    conditions, space, fn, short_circuit, enforced_conditions)
+                with StateSpaceContext(space):
+                    call_analysis = attempt_call(
+                        conditions, fn, short_circuit, enforced_conditions)
                 if failing_precondition is not None:
                     cur_precondition = call_analysis.failing_precondition
                     if cur_precondition is None:
                         if call_analysis.verification_status is not None:
                             # We escaped the all the pre conditions on this try:
                             failing_precondition = None
                     elif (cur_precondition.line == failing_precondition.line and
@@ -836,28 +921,28 @@
                           addl_context: str = '') -> str:
     with eval_friendly_repr():
         call_desc = ''
         if return_val is not _MISSING:
             try:
                 repr_str = repr(return_val)
             except Exception as e:
-                if isinstance(e, IgnoreAttempt):
+                if isinstance(e, (IgnoreAttempt, UnexploredPath)):
                     raise
-                debug(f'Exception attempting to repr function output: {e}')
+                debug(f'Exception attempting to repr function output: ', traceback.format_exc())
                 repr_str = _UNABLE_TO_REPR
             if repr_str != 'None':
                 call_desc = call_desc + ' (which returns ' + repr_str + ')'
         messages: List[str] = []
         for argname, argval in list(bound_args.arguments.items()):
             try:
                 repr_str = repr(argval)
             except Exception as e:
-                if isinstance(e, IgnoreAttempt):
+                if isinstance(e, (IgnoreAttempt, UnexploredPath)):
                     raise
-                debug(f'Exception attempting to repr input "{argname}": {repr(e)}')
+                debug(f'Exception attempting to repr input "{argname}": ', traceback.format_exc())
                 repr_str = _UNABLE_TO_REPR
             messages.append(argname + ' = ' + repr_str)
         call_desc = fn_name + '(' + ', '.join(messages) + ')' + call_desc
 
         if addl_context:
             return addl_context + ' when calling ' + call_desc # ' and '.join(messages)
         elif messages:
@@ -893,18 +978,19 @@
             for key in set(itertools.chain(old_val.keys(), *new_val.keys())):
                 if (key in old_val) ^ (key in new_val):
                     return False
                 if not deep_eq(old_val.get(key, _UNEQUAL), new_val.get(key, _UNEQUAL), visiting):
                     return False
             return True
         elif isinstance(old_val, Iterable):
-            assert isinstance(new_val, Iterable)
+            assert isinstance(new_val, Sized)
             if isinstance(old_val, Sized):
                 if len(old_val) != len(new_val):
                     return False
+            assert isinstance(new_val, Iterable)
             return all(deep_eq(o, n, visiting) for (o, n) in
                        itertools.zip_longest(old_val, new_val, fillvalue=_UNEQUAL))
         elif type(old_val) is object:
             # deepclone'd object instances are close enough to equal for our purposes
             return True
         else:
             # hopefully this is just ints, bools, etc
@@ -940,19 +1026,19 @@
             except IndexError:
                 exprline = '<unknown>'
             detail = f'"{exprline}" yields {detail}'
             return AnalysisMessage(message_type, detail, self.filename, self.start_lineno, 0, tb)
 
 
 def attempt_call(conditions: Conditions,
-                 space: StateSpace,
                  fn: Callable,
                  short_circuit: ShortCircuitingContext,
                  enforced_conditions: EnforcedConditions) -> CallAnalysis:
-    bound_args = gen_args(conditions.sig, space)
+    space = context_statespace()
+    bound_args = gen_args(conditions.sig)
 
     msg_gen = MessageGenerator(fn)
     with space.framework():
         # TODO: looks wrong(-ish) to guard this with space.framework().
         # Copy on custom objects may require patched builtins. (datetime.timedelta is one such case)
         original_args = copy.deepcopy(bound_args)
     space.checkpoint()
```

### Comparing `crosshair-tool-0.0.8/crosshair/core_test.py` & `crosshair-tool-0.0.9/crosshair/core_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 import copy
 import dataclasses
 import re
 import sys
 import unittest
 from typing import *
 
+from crosshair.core import get_constructor_params
 from crosshair.core import make_fake_object
 from crosshair.core_and_libs import *
 from crosshair.test_util import check_ok
 from crosshair.test_util import check_exec_err
 from crosshair.test_util import check_post_err
 from crosshair.test_util import check_fail
 from crosshair.test_util import check_unknown
 from crosshair.test_util import check_messages
 from crosshair.util import set_debug
+from crosshair.statespace import StateSpaceContext
 from crosshair.statespace import SimpleStateSpace
 
 
 
 
 
 
 
 
 
 
 
 
-
-
 #
 # Begin fixed line number area.
 # Tests depend on the line number of the following section.
 #
 
 class Pokeable:
     '''
@@ -185,30 +185,53 @@
         _ == True
     '''
     if x == 0:
         return True
     else:
         return recursive_example(x - 1)
 
+class RegularInt:
+    def __new__(self, num: 'int'):
+        return num
+
+class UnitTests(unittest.TestCase):
+    def test_get_constructor_params_with_new(self) -> None:
+        self.assertIs(RegularInt(7), 7)
+        params = get_constructor_params(RegularInt)
+        self.assertEqual(len(params), 1)
+        self.assertEqual(params[0].name, 'num')
+        self.assertEqual(params[0].annotation, int)
+
+    def test_AnalysisOptions_split_limits(self) -> None:
+        options = AnalysisOptions(
+            per_path_timeout=10.0,
+            max_iterations=16)
+        part1, part2 = options.split_limits(0.1)
+        self.assertEqual(part1.per_path_timeout, 1.0)
+        self.assertEqual(part2.per_path_timeout, 9.0)
+        self.assertEqual(part1.max_iterations, 2)
+        self.assertEqual(part2.max_iterations, 14)
 
 class ProxiedObjectTest(unittest.TestCase):
     def test_proxy_type(self) -> None:
-        poke = make_fake_object(SimpleStateSpace(), Pokeable, 'ppoke')
-        self.assertIs(type(poke), Pokeable)
+        with StateSpaceContext(SimpleStateSpace()):
+            poke = make_fake_object(Pokeable, 'ppoke')
+            self.assertIs(type(poke), Pokeable)
 
     def test_copy(self) -> None:
-        poke1 = make_fake_object(SimpleStateSpace(), Pokeable, 'ppoke')
-        poke1.poke()
-        poke2 = copy.copy(poke1)
-        self.assertIsNot(poke1, poke2)
-        self.assertEqual(type(poke1), type(poke2))
-        self.assertIs(poke1.x, poke2.x)
-        poke1.poke()
-        self.assertIsNot(poke1.x, poke2.x)
-        self.assertNotEqual(str(poke1.x.var), str(poke2.x.var))
+        with StateSpaceContext(SimpleStateSpace()):
+            poke1 = make_fake_object(Pokeable, 'ppoke')
+            poke1.poke()
+            poke2 = copy.copy(poke1)
+            self.assertIsNot(poke1, poke2)
+            self.assertEqual(type(poke1), type(poke2))
+            self.assertIs(poke1.x, poke2.x)
+            poke1.poke()
+            self.assertIsNot(poke1.x, poke2.x)
+            self.assertNotEqual(str(poke1.x.var), str(poke2.x.var))
 
     def test_proxy_alone(self) -> None:
         def f(pokeable: Pokeable) -> None:
             '''
             post[pokeable]: pokeable.x > 0
             '''
             pokeable.poke()
@@ -647,14 +670,22 @@
             ''' inv: self.count == __old__.self.count '''
             count: int
             def add_one(self):
                 self.count += 1
         messages = analyze_class(FrozenApples)
         self.assertEqual(*check_messages(messages, state=MessageType.POST_FAIL))
 
+    def test_class_patching_is_undone(self) -> None:
+        # CrossHair does a lot of monkey matching of classes
+        # with contracts. Ensure that gets undone.
+        original_class = Person.__dict__.copy()
+        analyze_any(Person.a_regular_method, AnalysisOptions())
+        for k, v in original_class.items():
+            self.assertIs(Person.__dict__[k], v)
+
     def test_fallback_when_smt_values_out_themselves(self) -> None:
         def f(items: List[str]) -> str:
             ''' post: True '''
             return ','.join(items)
         self.assertEqual(*check_unknown(f))
 
     def test_fallback_when_regex_is_used(self) -> None:
```

### Comparing `crosshair-tool-0.0.8/crosshair/dynamic_typing.py` & `crosshair-tool-0.0.9/crosshair/dynamic_typing.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/dynamic_typing_test.py` & `crosshair-tool-0.0.9/crosshair/dynamic_typing_test.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/enforce.py` & `crosshair-tool-0.0.9/crosshair/enforce.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 import copy
 import inspect
 import functools
 import sys
 import traceback
 import types
 from typing import *
-
-from crosshair.condition_parser import Conditions, get_fn_conditions, ClassConditions, get_class_conditions, fn_globals
-from crosshair.util import IdentityWrapper, AttributeHolder
-
+from crosshair.condition_parser import fn_globals
+from crosshair.condition_parser import Conditions
+from crosshair.condition_parser import ClassConditions
+from crosshair.condition_parser import ConditionParser
+from crosshair.util import IdentityWrapper
+from crosshair.util import AttributeHolder
+from crosshair.util import debug
 
 class PreconditionFailed(BaseException):
     pass
 
 
 class PostconditionFailed(BaseException):
     pass
@@ -27,15 +30,15 @@
 def EnforcementWrapper(fn: Callable, conditions: Conditions, enforced: 'EnforcedConditions') -> Callable:
     signature = conditions.sig
 
     def wrapper(*a, **kw):
         fns_enforcing = enforced.fns_enforcing
         if fns_enforcing is None or fn in fns_enforcing:
             return fn(*a, **kw)
-        #print('Calling enforcement wrapper ', fn)
+        #debug('Calling enforcement wrapper ', fn, signature, 'with', a, kw)
         bound_args = signature.bind(*a, **kw)
         bound_args.apply_defaults()
         old = {}
         mutable_args = conditions.mutable_args
         mutable_args_remaining = set(mutable_args) if mutable_args is not None else set()
         for argname, argval in bound_args.arguments.items():
             try:
@@ -45,52 +48,74 @@
             if argname in mutable_args_remaining:
                 mutable_args_remaining.remove(argname)
         if mutable_args_remaining:
             raise PostconditionFailed('Unrecognized mutable argument(s) in postcondition: "{}"'.format(
                 ','.join(mutable_args_remaining)))
         with enforced.currently_enforcing(fn):
             for precondition in conditions.pre:
-                #print(' precondition eval ', precondition.expr_source)
+                #debug(' precondition eval ', precondition.expr_source)
+                # TODO: is fn_globals required here?
                 args = {**fn_globals(fn), **bound_args.arguments}
-                if not eval(precondition.expr, args):
+                if not precondition.evaluate(args):
                     raise PreconditionFailed(
                         f'Precondition "{precondition.expr_source}" was not satisfied '
                         f'before calling "{fn.__name__}"')
         ret = fn(*a, **kw)
         with enforced.currently_enforcing(fn):
             lcls = {**bound_args.arguments, '__return__': ret,
                     '_': ret, '__old__': AttributeHolder(old)}
             args = {**fn_globals(fn), **lcls}
             for postcondition in conditions.post:
-                #print(' postcondition eval ', postcondition.expr_source, fn, lcls['_'])
-                if postcondition.expr and not eval(postcondition.expr, args):
+                #debug(' postcondition eval ', postcondition.expr_source, fn, lcls['_'])
+                if postcondition.evaluate and not postcondition.evaluate(args):
                     raise PostconditionFailed('Postcondition failed at {}:{}'.format(
                         postcondition.filename, postcondition.line))
-        #print('Completed enforcement wrapper ', fn)
+        #debug('Completed enforcement wrapper ', fn)
         return ret
     functools.update_wrapper(wrapper, fn)
     return wrapper
 
 
 class EnforcedConditions:
-    def __init__(self, *envs, interceptor=lambda x: x):
+    def __init__(self,
+                 condition_parser: ConditionParser,
+                 *envs: Mapping[str, object],
+                 interceptor=lambda x: x):
+        self.condition_parser = condition_parser
         self.envs = envs
         self.interceptor = interceptor
         self.fns_enforcing: Optional[Set[Callable]] = set()
-        self.wrapper_map: Dict[Callable, Callable] = {}
-        self.original_map: Dict[IdentityWrapper[Callable], Callable] = {}
+        self.wrapper_map: Dict[object, Callable] = {}
+        self.original_map: Dict[IdentityWrapper[object], object] = {}
+
+    def _wrap_class(self, cls: type) -> None:
+        if not self.condition_parser.get_class_conditions(cls).has_any():
+            return
+        #debug('wrapping class ', cls)
+        for superclass in cls.mro():
+            super_conditions = self.condition_parser.get_class_conditions(superclass)
+            if super_conditions.has_any():
+                self._wrap_class_members(superclass, super_conditions)
 
-    def _wrap_class(self, cls: type, class_conditions: ClassConditions) -> None:
-        #print('wrapping class ', cls)
+    def _wrap_class_members(self, cls: type, class_conditions: ClassConditions) -> None:
         method_conditions = dict(class_conditions.methods)
-        for method_name, method in list(inspect.getmembers(cls, inspect.isfunction)):
+        for method_name, method in list(cls.__dict__.items()):
+            # Note that `method` is post-property resolution. Also grab the raw member:
+            raw_method = cls.__dict__.get(method_name)
+            if raw_method is None: # likely defined on a superclass
+                continue
             conditions = method_conditions.get(method_name)
             if conditions is None:
                 continue
-            wrapper = self._wrap_fn(method, conditions)
+            if isinstance(raw_method, (staticmethod, classmethod)):
+                inner_wrapper = self._wrap_fn(raw_method.__func__, raw_fn=raw_method, conditions=conditions)
+                wrapper: object = type(raw_method)(inner_wrapper)
+                self.original_map[IdentityWrapper(wrapper)] = raw_method
+            else:
+                wrapper = self._wrap_fn(method, raw_fn=raw_method, conditions=conditions)
             setattr(cls, method_name, wrapper)
 
     def _transform_singledispatch(self, fn, transformer):
         overloads = list(fn.registry.items())
         wrapped = functools.singledispatch(transformer(overloads[0][1]))
         for overload_typ, overload_fn in overloads[1:]:
             wrapped.register(overload_typ)(transformer(overload_fn))
@@ -140,17 +165,15 @@
                             v, self._wrap_fn)
                     else:
                         wrapper = self._wrap_fn(v)
                         if wrapper is v:
                             continue
                     next_env[k] = wrapper
                 elif isinstance(v, type):
-                    conditions = get_class_conditions(v)
-                    if conditions.has_any():
-                        self._wrap_class(v, conditions)
+                    self._wrap_class(v)
         for env, next_env in zip(self.envs, next_envs):
             env.update(next_env)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         next_envs = [env.copy() for env in self.envs]
         for env, next_env in zip(self.envs, next_envs):
@@ -166,29 +189,31 @@
         elif is_singledispatcher(value):
             return self._transform_singledispatch(value, self._unwrap)
         elif isinstance(value, type):
             self._unwrap_class(value)
         return value
 
     def _unwrap_class(self, cls: type):
-        for method_name, method in list(inspect.getmembers(cls, inspect.isfunction)):
+        for method_name, method in list(cls.__dict__.items()):
             if self.is_enforcement_wrapper(method):
                 setattr(cls, method_name,
                         self.original_map[IdentityWrapper(method)])
 
-    def _wrap_fn(self, fn: Callable, conditions: Optional[Conditions] = None) -> Callable:
-        wrapper = self.wrapper_map.get(fn)
+    def _wrap_fn(self, fn: Callable,
+                 raw_fn: object = None,
+                 conditions: Optional[Conditions] = None) -> Callable:
+        # `raw_fn` is the unresolved descriptor, as appropriate.
+        if raw_fn is None:
+            raw_fn = fn
+        wrapper = self.wrapper_map.get(raw_fn)
         if wrapper is not None:
             return wrapper
-        if self.is_enforcement_wrapper(fn):
-            return fn
-
-        conditions = conditions or get_fn_conditions(fn)
+        conditions = conditions or self.condition_parser.get_fn_conditions(fn)
         if conditions and conditions.has_any():
             wrapper = EnforcementWrapper(
                 self.interceptor(fn), conditions, self)
             functools.update_wrapper(wrapper, fn)
         else:
             wrapper = fn
-        self.wrapper_map[fn] = wrapper
-        self.original_map[IdentityWrapper(wrapper)] = fn
+        self.wrapper_map[raw_fn] = wrapper
+        self.original_map[IdentityWrapper(wrapper)] = raw_fn
         return wrapper
```

### Comparing `crosshair-tool-0.0.8/crosshair/enforce_test.py` & `crosshair-tool-0.0.9/crosshair/examples/chess.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,73 @@
-import unittest
+import dataclasses
 
-from crosshair.enforce import *
-from typing import IO
-
-
-def foo(x: int) -> int:
+@dataclasses.dataclass(init=False)
+class ChessPiece:
     '''
-    pre: 0 <= x <= 100
-    post: _ > x
+    inv: 0 <= self.x < 8
+    inv: 0 <= self.y < 8
     '''
-    return x * 2
+    x: int
+    y: int
+
+    def __init__(self, x: int, y: int):
+        '''
+        raises: ValueError
+        '''
+        if not (0 <= x < 8):
+            raise ValueError(f'x position "{x}" is invalid')
+        if not (0 <= y < 8):
+            raise ValueError(f'y position "{y}" is invalid')
+        self.x = x
+        self.y = y
 
+    def can_move_to(self, x: int, y: int) -> bool:
+        '''
+        Determines whether this piece can move to the given 
+        position (in a single turn).
 
-class Pokeable:
-    '''
-    inv: self.x >= 0
-    '''
-    x: int = 1
+        pre: (0 <= x < 8) and (0 <= y < 8)
 
-    def poke(self) -> None:
-        self.x += 1
+        #  It's never valid to "move" to your present location:
+        post: implies((x, y) == (self.x, self.y), not __return__)
+        '''
+        raise NotImplementedError
 
-    def pokeby(self, amount: int) -> None:
+class FreeChessPiece(ChessPiece):
+    def can_move_to(self, x: int, y: int) -> bool:
         '''
-        pre: amount >= 0
+        Most pieces (except the pawn) can move back to their
+        starting position after moving.
+        post: implies(_, type(self)(x, y).can_move_to(self.x, self.y))
         '''
-        self.x += amount
-
-
-def same_stream(stream: IO) -> int:
-    ''' post: __old__.stream == _ '''
-    # It isn't possible to copy `stream` to make it available in `__old__`.
-    # In this case, enforcement will fail because __old__ won't contain it.
-    return stream
-
-class CoreTest(unittest.TestCase):
-
-    def test_enforce_and_unenforce(self) -> None:
-        env = {'foo': foo, 'bar': lambda x: x, 'baz': 42}
-        backup = env.copy()
-        with EnforcedConditions(env, interceptor=lambda f: (lambda x: x * 3)):
-            self.assertIs(env['bar'], backup['bar'])
-            self.assertIs(env['baz'], 42)
-            self.assertIsNot(env['foo'], backup['foo'])
-            self.assertEqual(env['foo'](50), 150)  # type:ignore
-        self.assertIs(env['foo'], backup['foo'])
-
-    def test_enforce_conditions(self) -> None:
-        env = {'foo': foo}
-        self.assertEqual(foo(-1), -2)  # unchecked
-        with EnforcedConditions(env):
-            self.assertEqual(env['foo'](50), 100)
-            with self.assertRaises(PreconditionFailed):
-                env['foo'](-1)
-            with self.assertRaises(PostconditionFailed):
-                env['foo'](0)
-
-    def test_class_enforce(self) -> None:
-        env = {'Pokeable': Pokeable}
-        old_id = id(Pokeable.poke)
-        Pokeable().pokeby(-1)  # no exception (yet!)
-        with EnforcedConditions(env):
-            self.assertNotEqual(id(env['Pokeable'].poke), old_id)
-            Pokeable().poke()
-            with self.assertRaises(PreconditionFailed):
-                Pokeable().pokeby(-1)
-        self.assertEqual(id(env['Pokeable'].poke), old_id)
-
-    def test_enforce_on_uncopyable_value(self) -> None:
-        env = {'l': same_stream}
-        self.assertIs(same_stream(sys.stdout), sys.stdout)
-        with EnforcedConditions(env):
-            with self.assertRaises(AttributeError):
-                env['l'](sys.stdout)
+        return self.can_move_to(x, y)
+    
+def _board_is_symmetric(piece: ChessPiece, x: int, y: int):
+    '''
+    A method just for testing.
+    (you could put this is a test file if you like)
+
+    If the given piece can move to (x,y), then the equivalent
+    opponent's piece should be able to move to the mirrored position.
+    
+    pre: piece.can_move_to(x, y)
+    post: piece.can_move_to(7 - x, 7 - y)
+    '''
+    piece.x = 7 - piece.x
+    piece.y = 7 - piece.y
+
+
+
+class Pawn(ChessPiece):
+    def can_move_to(self, x: int, y: int) -> bool:
+        return ((x == self.x) and (y == 3) and
+                (x, y) != (self.x, self.y))
+
+class Rook(FreeChessPiece):
+    def can_move_to(self, x: int, y: int) -> bool:
+        return (x == self.x) ^ (y == self.y)
 
-if __name__ == '__main__':
-    unittest.main()
+class King(FreeChessPiece):
+    def can_move_to(self, x: int, y: int) -> bool:
+        return (abs(x - self.x) <= 1 and
+                abs(y - self.y) <= 1 and
+                (x, y) != (self.x, self.y))
```

### Comparing `crosshair-tool-0.0.8/crosshair/examples/arith.py` & `crosshair-tool-0.0.9/crosshair/examples/arith.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/examples/hash_consistent_with_equals.py` & `crosshair-tool-0.0.9/crosshair/examples/hash_consistent_with_equals.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/examples/numpy_examples.py` & `crosshair-tool-0.0.9/crosshair/examples/numpy_examples.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/examples/rolling_average.py` & `crosshair-tool-0.0.9/crosshair/examples/rolling_average.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/examples/showcase.py` & `crosshair-tool-0.0.9/crosshair/examples/showcase.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/examples/tic_tac_toe.py` & `crosshair-tool-0.0.9/crosshair/examples/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/builtinslib.py` & `crosshair-tool-0.0.9/crosshair/libimpl/builtinslib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import collections
 import contextlib
 import copy
 import enum
 import functools
 import io
-import operator
+import math
+from numbers import Number, Complex, Real, Rational, Integral
+import operator as ops
 import re
 import typing
 from typing import *
 import builtins as orig_builtins
 
 from crosshair.abcstring import AbcString
 from crosshair.core import register_patch
@@ -24,27 +26,31 @@
 from crosshair.core import type_args_of
 from crosshair.core import name_of_type
 from crosshair.core import with_realized_args
 from crosshair.objectproxy import ObjectProxy
 from crosshair.simplestructs import SimpleDict
 from crosshair.simplestructs import SequenceConcatenation
 from crosshair.simplestructs import SliceView
+from crosshair.simplestructs import ShellMutableMap
 from crosshair.simplestructs import ShellMutableSequence
+from crosshair.simplestructs import ShellMutableSet
+from crosshair.statespace import context_statespace
 from crosshair.statespace import StateSpace
 from crosshair.statespace import HeapRef
 from crosshair.statespace import SnapshotRef
 from crosshair.statespace import model_value_to_python
 from crosshair.type_repo import PYTYPE_SORT
 from crosshair.util import debug
 from crosshair.util import CrosshairInternal
 from crosshair.util import CrosshairUnsupported
 from crosshair.util import IgnoreAttempt
 from crosshair.util import is_iterable
 from crosshair.util import is_hashable
 
+import typing_inspect # type: ignore
 import z3 # type: ignore
 
 class _Missing(enum.Enum):
     value = 0
 
 _MISSING = _Missing.value
 
@@ -68,197 +74,73 @@
     '''
     while type(val) is SmtObject:
         val = cast(SmtObject, val)._wrapped()
     return val
 
 _SMT_FLOAT_SORT = z3.RealSort()  # difficulty getting the solver to use z3.Float64()
 
-_TYPE_TO_SMT_SORT = {
-    bool: z3.BoolSort(),
-    str: z3.StringSort(),
-    int: z3.IntSort(),
-    float: _SMT_FLOAT_SORT,
-}
-
-
 def possibly_missing_sort(sort):
     datatype = z3.Datatype('optional_' + str(sort) + '_')
     datatype.declare('missing')
     datatype.declare('present', ('valueat', sort))
     ret = datatype.create()
     return ret
 
-
-def type_to_smt_sort(t: Type) -> z3.SortRef:
-    t = normalize_pytype(t)
-    if t in _TYPE_TO_SMT_SORT:
-        return _TYPE_TO_SMT_SORT[t]
-    origin = origin_of(t)
-    if origin is type:
-        return PYTYPE_SORT
-    return HeapRef
-
-SmtGenerator = Callable[[StateSpace, type, Union[str, z3.ExprRef]], object]
-
-_PYTYPE_TO_WRAPPER_TYPE: Dict[type, SmtGenerator] = {}  # to be populated later
-_WRAPPER_TYPE_TO_PYTYPE: Dict[SmtGenerator, type] = {}
+SmtGenerator = Callable[[Union[str, z3.ExprRef], type], object]
 
 def origin_of(typ: Type) -> Type:
     typ = _WRAPPER_TYPE_TO_PYTYPE.get(typ, typ)
     if hasattr(typ, '__origin__'):
         return typ.__origin__
     return typ
 
-def crosshair_type_for_python_type(typ: Type) -> Optional[SmtGenerator]:
-    typ = normalize_pytype(typ)
-    origin = origin_of(typ)
-    return _PYTYPE_TO_WRAPPER_TYPE.get(origin)
-
-
-def smt_bool_to_int(a: z3.ExprRef) -> z3.ExprRef:
-    return z3.If(a, 1, 0)
-
-
+# TODO: refactor away casting in SMT-sapce:
 def smt_int_to_float(a: z3.ExprRef) -> z3.ExprRef:
     if _SMT_FLOAT_SORT == z3.Float64():
         return z3.fpRealToFP(z3.RNE(), z3.ToReal(a), _SMT_FLOAT_SORT)
     elif _SMT_FLOAT_SORT == z3.RealSort():
         return z3.ToReal(a)
     else:
         raise CrosshairInternal()
 
-
 def smt_bool_to_float(a: z3.ExprRef) -> z3.ExprRef:
     if _SMT_FLOAT_SORT == z3.Float64():
         return z3.If(a, z3.FPVal(1.0, _SMT_FLOAT_SORT), z3.FPVal(0.0, _SMT_FLOAT_SORT))
     elif _SMT_FLOAT_SORT == z3.RealSort():
         return z3.If(a, z3.RealVal(1), z3.RealVal(0))
     else:
         raise CrosshairInternal()
 
-_IMPLICIT_SORT_CONVERSIONS: Dict[Tuple[z3.SortRef, z3.SortRef], Callable[[z3.ExprRef], z3.ExprRef]] = {
-    (z3.BoolSort(), z3.IntSort()): smt_bool_to_int,
-    (z3.BoolSort(), _SMT_FLOAT_SORT): smt_bool_to_float,
-    (z3.IntSort(), _SMT_FLOAT_SORT): smt_int_to_float,
-}
-
-_LITERAL_PROMOTION_FNS = {
-    bool: z3.BoolVal,
-    int: z3.IntVal,
-    float: z3.RealVal if _SMT_FLOAT_SORT == z3.RealSort() else (lambda v: z3.FPVal(v, _SMT_FLOAT_SORT)),
-    str: z3.StringVal,
-}
-
 def smt_coerce(val: Any) -> z3.ExprRef:
     if isinstance(val, SmtBackedValue):
         return val.var
     return val
 
-def force_to_smt_sort(space: StateSpace, input_value: Any, desired_sort: z3.SortRef) -> z3.ExprRef:
-    ret = coerce_to_smt_sort(space, input_value, desired_sort)
-    if ret is None:
-        raise TypeError('Could not derive smt sort ' + str(desired_sort))
-    return ret
-
-def coerce_to_smt_sort(space: StateSpace, input_value: Any, desired_sort: z3.SortRef) -> Optional[z3.ExprRef]:
-    natural_value = None
-    input_value = typeable_value(input_value)
-    promotion_fn = _LITERAL_PROMOTION_FNS.get(type(input_value))
-    if isinstance(input_value, SmtBackedValue):
-        natural_value = input_value.var
-        if type(natural_value) is tuple:
-            # Many container types aren't described by a single z3 value:
-            return None
-    elif promotion_fn:
-        natural_value = promotion_fn(input_value)
-    elif isinstance(input_value, z3.ExprRef):
-        natural_value = input_value
-    natural_sort = natural_value.sort() if natural_value is not None else None
-    conversion_fn = _IMPLICIT_SORT_CONVERSIONS.get((natural_sort, desired_sort))
-    if conversion_fn:
-        return conversion_fn(natural_value)
-    if natural_sort == desired_sort:
-        return natural_value
-    if desired_sort == HeapRef:
-        return space.find_val_in_heap(input_value)
-    if desired_sort == PYTYPE_SORT and isinstance(input_value, type):
-        return space.type_repo.get_type(input_value)
-    return None
-
-
-def coerce_to_smt_var(space: StateSpace, v: Any) -> z3.ExprRef:
-    v = typeable_value(v)
-    if isinstance(v, SmtBackedValue):
-        return v.var
-    promotion_fn = _LITERAL_PROMOTION_FNS.get(type(v))
-    if promotion_fn:
-        return promotion_fn(v)
-    return space.find_val_in_heap(v)
-
-
-def smt_to_ch_value(space: StateSpace, snapshot: SnapshotRef, smt_val: z3.ExprRef, pytype: type) -> object:
-    def proxy_generator(typ: Type) -> object:
-        return proxy_for_type(typ, space, 'heapval' + str(typ) + space.uniq())
-    if smt_val.sort() == HeapRef:
-        return space.find_key_in_heap(smt_val, pytype, proxy_generator, snapshot)
-    ch_type = crosshair_type_for_python_type(pytype)
-    assert ch_type is not None
-    return ch_type(space, pytype, smt_val)
-
-
-def attr_on_ch_value(other: Any, statespace: StateSpace, attr: str) -> object:
-    if not isinstance(other, CrossHairValue):
-        smt_var = coerce_to_smt_var(statespace, other)
-        py_type = python_type(other)
-        Typ = crosshair_type_for_python_type(py_type)
-        if Typ is None:
-            raise TypeError
-        other = Typ(statespace, py_type, smt_var)
-    if not hasattr(other, attr):
-        raise TypeError
-    return getattr(other, attr)
-
 class SmtBackedValue(CrossHairValue):
-    def __init__(self, statespace: StateSpace, typ: Type, smtvar: object):
-        self.statespace = statespace
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type):
+        self.statespace = context_statespace()
         self.snapshot = SnapshotRef(-1)
         self.python_type = typ
-        if isinstance(smtvar, str):
+        if type(smtvar) is str:
             self.var = self.__init_var__(typ, smtvar)
         else:
             self.var = smtvar
             # TODO test that smtvar's sort matches expected?
 
     def __init_var__(self, typ, varname):
-        z3type = type_to_smt_sort(typ)
-        return z3.Const(varname, z3type)
+        raise CrosshairInternal(f'__init_var__ not implemented in {type(self)}')
 
     def __deepcopy__(self, memo):
         shallow = copy.copy(self)
         shallow.snapshot = self.statespace.current_snapshot()
         return shallow
 
     def __bool__(self):
         return NotImplemented
 
-    def __eq__(self, other):
-        coerced = coerce_to_smt_sort(self.statespace, other, self.var.sort())
-        if coerced is None:
-            return False
-        return SmtBool(self.statespace, bool, self.var == coerced)
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __req__(self, other):
-        return self.__eq__(other)
-
-    def __rne__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__ne__')(self)
-
     def __lt__(self, other):
         raise TypeError
 
     def __gt__(self, other):
         raise TypeError
 
     def __le__(self, other):
@@ -272,426 +154,700 @@
 
     def __sub__(self, other):
         raise TypeError
 
     def __mul__(self, other):
         raise TypeError
 
-    def __pow__(self, other):
+    def __pow__(self, other, mod=None):
         raise TypeError
 
     def __truediv__(self, other):
-        raise TypeError
+        return numeric_binop(ops.truediv, self, other)
 
     def __floordiv__(self, other):
         raise TypeError
 
     def __mod__(self, other):
         raise TypeError
 
-    def __and__(self, other):
-        raise TypeError
-
-    def __or__(self, other):
-        raise TypeError
-
-    def __xor__(self, other):
-        raise TypeError
-
     def __ch_pytype__(self):
         return self.python_type
 
     def __ch_realize__(self):
         return origin_of(self.python_type)(self)
 
     def __ch_forget_contents__(self, space: StateSpace):
-        clean_smt = type(self)(space, self.python_type,
-                               str(self.var) + space.uniq())
+        clean_smt = type(self)(str(self.var) + space.uniq(),
+                               self.python_type)
         self.var = clean_smt.var
 
-    def _binary_op(self, other, smt_op, py_op=None, expected_sort=None):
-        #debug(f'binary op ({smt_op}) on value of type {type(other)}')
-        left = self.var
-        if expected_sort is None:
-            expected_sort = type_to_smt_sort(self.python_type)
-        right = coerce_to_smt_sort(self.statespace, other, expected_sort)
-        if right is None:
-            return py_op(realize(self), realize(other))
-        try:
-            ret = smt_op(left, right)
-        except z3.z3types.Z3Exception as e:
-            debug('Raising z3 error as Python TypeError: ', str(e))
-            raise TypeError
-        return self.__class__(self.statespace, self.python_type, ret)
-
     def _unary_op(self, op):
-        return self.__class__(self.statespace, self.python_type, op(self.var))
+        # ...
+        return self.__class__(op(self.var), self.python_type)
 
 
-class SmtNumberAble(SmtBackedValue):
-    def _numeric_binary_smt_op(self, other, op) -> Optional[Tuple[z3.ExprRef, type]]:
-        other = typeable_value(other)
-        if type(other) is SmtBool:
-            # at a minimum, promote to an integer (in case both values are booleans)
-            other = convert(other, int)
-        l_val, r_val = convert_to_common_type(self, typeable_value(other))
-        l_pytype = python_type(l_val)
-        r_pytype = python_type(r_val)
-        if l_pytype != r_pytype:
-            return None
-        l_var = coerce_to_smt_var(self.statespace, l_val)
-        r_var = coerce_to_smt_var(self.statespace, r_val)
-        return (op(l_var, r_var), l_pytype)
-
-    def _numeric_binary_op(self, other, op, op_result_pytype=None):
-        if type(other) == complex:
-            return op(complex(self), complex(other))
-        result = self._numeric_binary_smt_op(other, op)
-        if result is None:
-            raise TypeError
-        smt_result, common_pytype = result
-        if op_result_pytype is not None:
-            common_pytype = op_result_pytype
-        cls = _PYTYPE_TO_WRAPPER_TYPE[common_pytype]
-        return cls(self.statespace, common_pytype, smt_result)
+class AtomicSmtValue(SmtBackedValue):
+    def __init_var__(self, typ, varname):
+        z3type = type(self)._ch_smt_sort()
+        return z3.Const(varname, z3type)
+
+    @classmethod
+    def _ch_smt_sort(cls) -> z3.SortRef:
+        raise CrosshairInternal(f'_ch_smt_sort not implemented in {cls}')
+
+    @classmethod
+    def _pytype(cls) -> Type:
+        raise CrosshairInternal(f'_pytype not implemented in {cls}')
+
+    @classmethod
+    def _smt_promote_literal(cls, val: object) -> Optional[z3.SortRef]:
+        raise CrosshairInternal(f'_smt_promote_literal not implemented in {cls}')
+
+    @classmethod
+    def _coerce_to_smt_sort(cls, input_value: Any) -> Optional[z3.ExprRef]:
+        input_value = typeable_value(input_value)
+        target_pytype = cls._pytype()
+
+        # check the likely cases first
+        if isinstance(input_value, cls):
+            return input_value.var
+        elif isinstance(input_value, target_pytype):
+            return cls._smt_promote_literal(input_value)
+
+        # see whether we can safely cast and retry
+        if isinstance(input_value, Number) and issubclass(cls, Number):
+            if isinstance(input_value, SmtBackedValue):
+                casting_fn_name = '__' + target_pytype.__name__ + '__'
+                converted = getattr(input_value, casting_fn_name)()
+                return cls._coerce_to_smt_sort(converted)
+            else: # non-symbolic
+                casted = target_pytype(input_value)
+                if casted == input_value:
+                    return cls._coerce_to_smt_sort(casted)
+
+        return None
+
+    def __eq__(self, other):
+        with self.statespace.framework():
+            coerced = type(self)._coerce_to_smt_sort(other)
+            if coerced is None:
+                return False
+            return SmtBool(self.var == coerced)
+
+
+_PYTYPE_TO_WRAPPER_TYPE: Dict[type, Tuple[Type[AtomicSmtValue], ...]] = {}  # to be populated later
+_WRAPPER_TYPE_TO_PYTYPE: Dict[SmtGenerator, type] = {}
+
+def crosshair_types_for_python_type(typ: Type) -> Tuple[Type[AtomicSmtValue], ...]:
+    typ = normalize_pytype(typ)
+    origin = origin_of(typ)
+    return _PYTYPE_TO_WRAPPER_TYPE.get(origin, ())
+
+def smt_to_ch_value(space: StateSpace, snapshot: SnapshotRef, smt_val: z3.ExprRef, pytype: type) -> object:
+    def proxy_generator(typ: Type) -> object:
+        return proxy_for_type(typ, 'heapval' + str(typ) + space.uniq())
+    if smt_val.sort() == HeapRef:
+        return space.find_key_in_heap(smt_val, pytype, proxy_generator, snapshot)
+    ch_type = crosshair_types_for_python_type(pytype)
+    assert ch_type
+    return ch_type[0](smt_val, pytype)
+
+def force_to_smt_sort(input_value: Any, desired_ch_type: Type[AtomicSmtValue]) -> z3.ExprRef:
+    ret = desired_ch_type._coerce_to_smt_sort(input_value)
+    if ret is None:
+        raise TypeError(f'Could not derive smt from {input_value}:{type(input_value)}')
+    return ret
+
+
+
+
+
+# The Python numeric tower is (at least to me) fairly confusing.
+# A summary here, with some example implementations:
+#
+# Number
+# |
+# Complex
+# | \- complex
+# Real
+# | \- float
+# Rational
+# | \- Fraction
+# Integral
+# |
+# int
+# |
+# bool   (yes, bool is a subtype of int!)
+#
+
+TypePair = Tuple[type, type]
+BinFn = Callable[[Number, Number], Number]
+OpHandler = Union[_Missing, Callable[[BinFn, Number, Number], Number]]
+
+_BIN_OPS: Dict[Tuple[BinFn, type, type], OpHandler] = {}
+_BIN_OPS_SEARCH_ORDER: List[Tuple[BinFn, type, type, OpHandler]] = []
+
+class FiniteFloat(float):
+    pass
+
+def numeric_binop(op: BinFn, a: Number, b: Number):
+    a_type, b_type = type(a), type(b)
+    binfn = _BIN_OPS.get((op, a_type, b_type))
+    if binfn is None:
+        for curop, cur_a_type, cur_b_type, curfn in reversed(_BIN_OPS_SEARCH_ORDER):
+            if op != curop:
+                continue
+            if (issubclass(a_type, cur_a_type) and
+                issubclass(b_type, cur_b_type)):
+                _BIN_OPS[(op, a_type, b_type)] = curfn  # cache concrete types for later
+                binfn = curfn
+                break
+        if binfn is None:
+            binfn = _MISSING
+            _BIN_OPS[(op, a_type, b_type)] = _MISSING
+    if binfn is _MISSING:
+        return NotImplemented
+    return binfn(op, a, b)
+
+def _binop_type_hints(fn: Callable):
+    hints = get_type_hints(fn)
+    a, b = hints['a'], hints['b']
+    if typing_inspect.get_origin(a) == Union:
+        a = typing_inspect.get_args(a)
+    else:
+        a = [a]
+    if typing_inspect.get_origin(b) == Union:
+        b = typing_inspect.get_args(b)
+    else:
+        b = [b]
+    return (a, b)
+
+def setup_promotion(fn: Callable[[Number, Number], Tuple[Number, Number]], reg_ops: Set[BinFn]):
+    a, b = _binop_type_hints(fn)
+    for a_type in a:
+        for b_type in b:
+            for op in reg_ops:
+                def forward(o, x, y):
+                    x2, y2 = fn(x, y)
+                    return numeric_binop(o, x2, y2)
+                def backward(o, x, y):
+                    y2, x2 = fn(y, x)
+                    return numeric_binop(o, x2, y2)
+                _BIN_OPS_SEARCH_ORDER.append((op, a_type, b_type, forward))
+                _BIN_OPS_SEARCH_ORDER.append((op, b_type, a_type, backward))
+
+_FLIPPED_OPS = {ops.ge: ops.le, ops.gt: ops.lt, ops.le: ops.ge, ops.lt: ops.gt}
+def setup_binop(fn: Callable[[BinFn, Number, Number], Number], reg_ops: Set[BinFn]):
+    a, b = _binop_type_hints(fn)
+    for a_type in a:
+        for b_type in b:
+            for op in reg_ops:
+                _BIN_OPS_SEARCH_ORDER.append((op, a_type, b_type, fn))
+
+                # Also, handle flipped comparisons transparently:
+                ## (a >= b)   <==>   (b <= a)
+                if op in (ops.ge, ops.gt, ops.le, ops.lt):
+                    def flipped(o, x, y):
+                        return fn(_FLIPPED_OPS[o], y, x)
+                    _BIN_OPS_SEARCH_ORDER.append((_FLIPPED_OPS[op], b_type, a_type, flipped))
+
+
+_COMPARISON_OPS: Set[BinFn] = {
+    ops.eq,
+    ops.ne,
+    ops.ge,
+    ops.gt,
+    ops.le,
+    ops.lt,
+}
+_ARITHMETIC_OPS: Set[BinFn] = {
+    ops.add,
+    ops.sub,
+    ops.mul,
+    ops.truediv,
+    ops.floordiv,
+    ops.mod,
+    ops.pow,
+}
+_BITWISE_OPS: Set[BinFn] = {
+    ops.and_,
+    ops.or_,
+    ops.xor,
+    ops.rshift,
+    ops.lshift,
+}
+
+def apply_smt(op: BinFn, x: z3.ExprRef, y: z3.ExprRef) -> z3.ExprRef:
+    # Mostly, z3 overloads operators and things just work.
+    # But some special cases need to be checked first.
+    if op in _ARITHMETIC_OPS:
+        if op in(ops.truediv, ops.floordiv, ops.mod):
+            if context_statespace().smt_fork(y == 0):
+                raise ZeroDivisionError('division by zero')
+            if op == ops.floordiv:
+                return z3.If(
+                    x % y == 0 or x >= 0, x / y,
+                    z3.If(y >= 0, x / y + 1, x / y - 1))
+        elif op == ops.pow:
+            if context_statespace().smt_fork(z3.And(x == 0, y < 0)):
+                raise ZeroDivisionError('zero cannot be raised to a negative power')
+    elif op in _BITWISE_OPS:
+        if op in (ops.lshift, ops.rshift):
+            if context_statespace().smt_fork(y < 0):
+                raise ValueError('negative shift count')
+            return x * (2 ** y) if op == ops.lshift else x / (2 ** y)
+    return op(x, y)
+
+
+_ARITHMETIC_AND_BITWISE_OPS = _ARITHMETIC_OPS.union(_BITWISE_OPS)
+_ARITHMETIC_AND_COMPARISON_OPS = _ARITHMETIC_OPS.union(_COMPARISON_OPS)
+_ALL_OPS = _ARITHMETIC_AND_COMPARISON_OPS.union(_BITWISE_OPS)
+
+def setup_binops():
+
+    # We check NaN and infitity immediately; not all
+    # symbolic floats support these cases.
+    def _(a: Real, b: float):
+        if math.isfinite(b):
+            return (a, FiniteFloat(b))  # type: ignore
+        if a > 0:  # type: ignore
+            return (1, b)  # type: ignore
+        elif a < 0:
+            return (-1, b)  # type: ignore
+        else:
+            return (0, b)  # type: ignore
+    setup_promotion(_, _ARITHMETIC_AND_COMPARISON_OPS)
 
+
+    # Implicitly upconvert symbolic bools to integers.
+    # Note that we don't want this when `other` is a boolean, but that
+    # case will be overridden in the booleans section below.
+    def _(a: SmtBool, b: Number):
+        return (SmtInt(z3.If(a.var, 1, 0)), b)
+    setup_promotion(_, _ALL_OPS)
+
+    # Implicitly upconvert symbolic ints to floats.
+    def _(a: SmtInt, b: Union[float, FiniteFloat, SmtFloat, complex]):
+        return (SmtFloat(z3.ToReal(a.var)), b)
+    setup_promotion(_, _ARITHMETIC_AND_COMPARISON_OPS)
+
+    # Implicitly upconvert native ints to floats.
+    def _(a: int, b: SmtFloat):
+        return (float(a), b)
+    setup_promotion(_, _ARITHMETIC_AND_COMPARISON_OPS)
+
+    # Implicitly upconvert native bools to ints.
+    def _(a: bool, b: Union[SmtInt, SmtFloat]):
+        return (int(a), b)
+    setup_promotion(_, _ARITHMETIC_AND_COMPARISON_OPS)
+
+
+    # complex
+    def _(op: BinFn, a: SmtNumberAble, b: complex):
+        return op(complex(a), b)
+    setup_binop(_, _ALL_OPS)
+
+    # float
+    def _(op: BinFn, a: SmtFloat, b: SmtFloat):
+        return SmtFloat(apply_smt(op, a.var, b.var))
+    setup_binop(_, _ARITHMETIC_OPS)
+    def _(op: BinFn, a: SmtFloat, b: SmtFloat):
+        return SmtBool(apply_smt(op, a.var, b.var))
+    setup_binop(_, _COMPARISON_OPS)
+    def _(op: BinFn, a: SmtFloat, b: FiniteFloat):
+        return SmtFloat(apply_smt(op, a.var, z3.RealVal(b)))
+    setup_binop(_, _ARITHMETIC_OPS)
+    def _(op: BinFn, a: FiniteFloat, b: SmtFloat):
+        return SmtFloat(apply_smt(op, z3.RealVal(a), b.var))
+    setup_binop(_, _ARITHMETIC_OPS)
+    def _(op: BinFn, a: SmtFloat, b: FiniteFloat):
+        return SmtBool(apply_smt(op, a.var, z3.RealVal(b)))
+    setup_binop(_, _COMPARISON_OPS)
+
+    # int
+    def _(op: BinFn, a: SmtInt, b: SmtInt):
+        return SmtInt(apply_smt(op, a.var, b.var))
+    setup_binop(_, _ARITHMETIC_AND_BITWISE_OPS)
+    def _(op: BinFn, a: SmtInt, b: SmtInt):
+        return SmtBool(apply_smt(op, a.var, b.var))
+    setup_binop(_, _COMPARISON_OPS)
+    def _(op: BinFn, a: SmtInt, b: int):
+        return SmtInt(apply_smt(op, a.var, z3.IntVal(b)))
+    setup_binop(_, _ARITHMETIC_AND_BITWISE_OPS)
+    def _(op: BinFn, a: int, b: SmtInt):
+        return SmtInt(apply_smt(op, z3.IntVal(a), b.var))
+    setup_binop(_, _ARITHMETIC_AND_BITWISE_OPS)
+    def _(op: BinFn, a: SmtInt, b: int):
+        return SmtBool(apply_smt(op, a.var, z3.IntVal(b)))
+    setup_binop(_, _COMPARISON_OPS)
+    def _(op: BinFn, a: Integral, b: Integral):  # Most bitwise operators require realization
+        return op(a.__index__(), b.__index__())  # type: ignore
+    setup_binop(_, {ops.and_, ops.or_, ops.xor})
+    def _(op: BinFn, a: Integral, b: Integral):  # Floor division over ints requires realization, at present
+        return op(a.__index__(), b.__index__())  # type: ignore
+    setup_binop(_, {ops.truediv})
+    def _(a: SmtInt, b: Number):  # Division over ints must produce float
+        return (a.__float__(), b)
+    setup_promotion(_, {ops.truediv})
+
+    # bool
+    def _(op: BinFn, a: SmtBool, b: SmtBool):
+        return SmtBool(apply_smt(op, a.var, b.var))
+    setup_binop(_, {ops.eq, ops.ne})
+    def _(op: BinFn, a: SmtBool, b: bool):
+        return SmtInt(apply_smt(op, a.var, z3.BoolVal(b)))
+    setup_binop(_, _ARITHMETIC_OPS)
+    def _(op: BinFn, a: bool, b: SmtBool):
+        return SmtInt(apply_smt(op, z3.BoolVal(a), b.var))
+    setup_binop(_, _ARITHMETIC_OPS)
+
+
+#
+#  END new numbers
+#
+
+
+class SmtNumberAble(SmtBackedValue, Real):
     def __pos__(self):
         return self
 
     def __neg__(self):
-        return self._unary_op(operator.neg)
+        return self._unary_op(ops.neg)
 
     def __abs__(self):
         return self._unary_op(lambda v: z3.If(v < 0, -v, v))
 
     def __lt__(self, other):
-        return self._numeric_binary_op(other, operator.lt, op_result_pytype=bool)
+        return numeric_binop(ops.lt, self, other)
 
     def __gt__(self, other):
-        return self._numeric_binary_op(other, operator.gt, op_result_pytype=bool)
+        return numeric_binop(ops.gt, self, other)
 
     def __le__(self, other):
-        return self._numeric_binary_op(other, operator.le, op_result_pytype=bool)
+        return numeric_binop(ops.le, self, other)
 
     def __ge__(self, other):
-        return self._numeric_binary_op(other, operator.ge, op_result_pytype=bool)
+        return numeric_binop(ops.ge, self, other)
 
     def __eq__(self, other):
-        # Note this is a little different than the other comparison operations, because
-        # equality doesn't raise TypeErrors on mismatched types
-        result = self._numeric_binary_smt_op(other, operator.eq)
-        if result is None:
-            return False
-        return SmtBool(self.statespace, bool, result[0])
+        return numeric_binop(ops.eq, self, other)
 
     def __add__(self, other):
-        return self._numeric_binary_op(other, operator.add)
+        return numeric_binop(ops.add, self, other)
+    def __radd__(self, other):
+        return numeric_binop(ops.add, other, self)
 
     def __sub__(self, other):
-        return self._numeric_binary_op(other, operator.sub)
+        return numeric_binop(ops.sub, self, other)
+    def __rsub__(self, other):
+        return numeric_binop(ops.sub, other, self)
 
     def __mul__(self, other):
-        if isinstance(other, (str, SmtStr, collections.abc.Sequence)):
-            return other.__mul__(self)
-        return self._numeric_binary_op(other, operator.mul)
-
-    def __pow__(self, other):
-        if other < 0 and self == 0:
-            raise ZeroDivisionError
-        return self._numeric_binary_op(other, operator.pow)
-
+        return numeric_binop(ops.mul, self, other)
     def __rmul__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__mul__')(self)
+        return numeric_binop(ops.mul, other, self)
 
-    def __radd__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__add__')(self)
+    def __pow__(self, other, mod=None):
+        if mod is not None:
+            return pow(realize(self), pow, mod)
+        return numeric_binop(ops.pow, self, other)
+    def __rpow__(self, other, mod=None):
+        if mod is not None:
+            return pow(other, realize(self), mod)
+        return numeric_binop(ops.pow, other, self)
 
-    def __rsub__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__sub__')(self)
+    def __lshift__(self, other):
+        return numeric_binop(ops.lshift, self, other)
+    def __rlshift__(self, other):
+        return numeric_binop(ops.lshift, other, self)
 
-    def __rtruediv__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__truediv__')(self)
+    def __rshift__(self, other):
+        return numeric_binop(ops.rshift, self, other)
+    def __rrshift__(self, other):
+        return numeric_binop(ops.rshift, other, self)
 
-    def __rfloordiv__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__floordiv__')(self)
 
-    def __rmod__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__mod__')(self)
+    def __and__(self, other):
+        return numeric_binop(ops.and_, self, other)
+    def __rand__(self, other):
+        return numeric_binop(ops.and_, other, self)
 
-    def __rdivmod__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__divmod__')(self)
+    def __or__(self, other):
+        return numeric_binop(ops.or_, self, other)
+    def __ror__(self, other):
+        return numeric_binop(ops.or_, other, self)
 
-    def __rpow__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__pow__')(self)
+    def __xor__(self, other):
+        return numeric_binop(ops.xor, self, other)
+    def __rxor__(self, other):
+        return numeric_binop(ops.xor, other, self)
 
-    def __rlshift__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__lshift__')(self)
+    def __rtruediv__(self, other):
+        return numeric_binop(ops.truediv, other, self)
 
-    def __rrshift__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__rshift__')(self)
+    def __floordiv__(self, other):
+        return numeric_binop(ops.floordiv, self, other)
+    def __rfloordiv__(self, other):
+        return numeric_binop(ops.floordiv, other, self)
 
-    def __rand__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__and__')(self)
+    def __mod__(self, other):
+        return numeric_binop(ops.mod, self, other)
+    def __rmod__(self, other):
+        return numeric_binop(ops.mod, other, self)
 
-    def __rxor__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__xor__')(self)
+    def __divmod__(self, other):
+        return (self // other, self % other)
+    def __rdivmod__(self, other):
+        return (other // self, other % self)
 
-    def __ror__(self, other):
-        return attr_on_ch_value(other, self.statespace, '__or__')(self)
 
-class SmtIntable(SmtNumberAble):
+class SmtIntable(SmtNumberAble, Integral):
     # bitwise operators
     def __invert__(self):
         return -(self + 1)
 
-    def __lshift__(self, other):
-        if other < 0:
-            raise ValueError('negative shift count')
-        return self * (2 ** other)
-
-    def __rshift__(self, other):
-        if other < 0:
-            raise ValueError('negative shift count')
-        return self // (2 ** other)
-
-    def _apply_bitwise(self, op: Callable, v1: int, v2: int) -> int:
-        if (not hasattr(v1, '__index__')) or (not hasattr(v2, '__index__')):
-            raise TypeError
-        return op(v1.__index__(), v2.__index__())
-
-    def __and__(self, other):
-        return self._apply_bitwise(operator.and_, self, other)
-
-    def __or__(self, other):
-        return self._apply_bitwise(operator.or_, self, other)
-
-    def __xor__(self, other):
-        return self._apply_bitwise(operator.xor, self, other)
+    def __floor__(self):
+        return self
+    def __ceil__(self):
+        return self
+    def __trunc__(self):
+        return self
 
-    def __truediv__(self, other):
-        return self.__float__() / other
+    def __mul__(self, other):
+        if isinstance(other, str):
+            # Create a symbolic string that regex-matches as a repetition.
+            space = self.statespace
+            count = self.var # z3.If(self.var >= 0, self.var, 0))
+            result = SmtStr(f'{self.var}_str{space.uniq()}')
+            space.add(z3.InRe(result.var, z3.Star(z3.Re(other))))
+            space.add(z3.Length(result.var) == len(other) * count)
+            return result
+        return numeric_binop(ops.mul, self, other)
+    __rmul__ = __mul__
 
-    def __divmod__(self, other):
-        return (self // other, self % other)
 
-    def __floordiv__(self, other):
-        if other == 0:
-            raise ZeroDivisionError()
-        if not isinstance(other, (bool, int, SmtInt, SmtBool)):
-            return realize(self) // realize(other)
-        return self._numeric_binary_op(other, lambda x, y: z3.If(
-            x % y == 0 or x >= 0, x / y, z3.If(y >= 0, x / y + 1, x / y - 1)))
+class SmtBool(AtomicSmtValue, SmtIntable):
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type = bool):
+        assert typ == bool
+        SmtBackedValue.__init__(self, smtvar, typ)
 
-    def __mod__(self, other):
-        if other == 0:
-            raise ZeroDivisionError()
-        if not isinstance(other, (bool, int, SmtInt, SmtBool)):
-            return realize(self) % realize(other)
-        return self._numeric_binary_op(other, operator.mod)
+    @classmethod
+    def _ch_smt_sort(cls) -> z3.SortRef:
+        return z3.BoolSort()
 
+    @classmethod
+    def _pytype(cls) -> Type:
+        return bool
 
-class SmtBool(SmtIntable):
-    def __init__(self, statespace: StateSpace, typ: Type, smtvar: object):
-        assert typ == bool
-        SmtBackedValue.__init__(self, statespace, typ, smtvar)
+    @classmethod
+    def _smt_promote_literal(cls, literal) -> Optional[z3.SortRef]:
+        if isinstance(literal, bool):
+            return z3.BoolVal(literal)
+        return None
 
     def __neg__(self):
-        return SmtInt(self.statespace, int, -smt_bool_to_int(self.var))
+        return SmtInt(z3.If(self.var, -1, 0))
 
     def __repr__(self):
         return self.__bool__().__repr__()
 
     def __hash__(self):
         return self.__bool__().__hash__()
 
     def __index__(self):
-        return SmtInt(self.statespace, int, smt_bool_to_int(self.var))
-
-    def __xor__(self, other):
-        return self._binary_op(other, z3.Xor)
+        return SmtInt(z3.If(self.var, 1, 0))
 
     def __bool__(self):
         return self.statespace.choose_possible(self.var)
 
     def __int__(self):
-        return SmtInt(self.statespace, int, smt_bool_to_int(self.var))
+        return SmtInt(z3.If(self.var, 1, 0))
 
     def __float__(self):
-        return SmtFloat(self.statespace, float, smt_bool_to_float(self.var))
+        return SmtFloat(smt_bool_to_float(self.var))
 
     def __complex__(self):
         return complex(self.__float__())
 
-    def __add__(self, other):
-        return self._numeric_binary_op(other, operator.add)
-
-    def __sub__(self, other):
-        return self._numeric_binary_op(other, operator.sub)
+    def __round__(self, ndigits=None):
+        return round(int(self), ndigits)
 
 
-class SmtInt(SmtIntable):
-    def __init__(self, statespace: StateSpace, typ: Type, smtvar: Union[str, z3.ArithRef]):
+class SmtInt(AtomicSmtValue, SmtIntable):
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type = int):
         assert typ == int
-        assert type(smtvar) != int
-        SmtIntable.__init__(self, statespace, typ, smtvar)
+        SmtIntable.__init__(self, smtvar, typ)
+
+    @classmethod
+    def _ch_smt_sort(cls) -> z3.SortRef:
+        return z3.IntSort()
+
+    @classmethod
+    def _pytype(cls) -> Type:
+        return int
+
+    @classmethod
+    def _smt_promote_literal(cls, literal) -> Optional[z3.SortRef]:
+        if isinstance(literal, int):
+            return z3.IntVal(literal)
+        return None
 
     def __repr__(self):
         return self.__index__().__repr__()
         # TODO: do a symbolic conversion!:
-        #return SmtStr(self.statespace, str, z3.IntToStr(self.var))
+        #return SmtStr(z3.IntToStr(self.var))
 
     def __hash__(self):
         return self.__index__().__hash__()
 
     def __float__(self):
-        return SmtFloat(self.statespace, float, smt_int_to_float(self.var))
+        return SmtFloat(smt_int_to_float(self.var))
 
     def __complex__(self):
         return complex(self.__float__())
 
     def __index__(self):
         #debug('WARNING: attempting to materialize symbolic integer. Trace:')
         # traceback.print_stack()
         if self == 0:
             return 0
         ret = self.statespace.find_model_value(self.var)
-        assert type(ret) is int
+        assert type(ret) is int, f'SmtInt with wrong SMT var type ({type(ret)})'
         return ret
 
     def __bool__(self):
-        return SmtBool(self.statespace, bool, self.var != 0).__bool__()
+        return SmtBool(self.var != 0).__bool__()
 
     def __int__(self):
         return self.__index__()
 
+    def __round__(self, ndigits=None):
+        if ndigits is None or ndigits >= 0:
+            return self # TODO: test
+        return round(self.__index__(), ndigits) # TODO: could do this symbolically
+
 
 _Z3_ONE_HALF = z3.RealVal("1/2")
 
 
-class SmtFloat(SmtNumberAble):
-    def __init__(self, statespace: StateSpace, typ: Type, smtvar: object):
-        assert typ == float
-        SmtBackedValue.__init__(self, statespace, typ, smtvar)
+class SmtFloat(AtomicSmtValue, SmtNumberAble):
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type = float):
+        assert typ == float, f'SmtFloat created with unexpected python type ({type(typ)})'
+        SmtBackedValue.__init__(self, smtvar, typ)
+
+    @classmethod
+    def _ch_smt_sort(cls) -> z3.SortRef:
+        return z3.RealSort()
+
+    @classmethod
+    def _pytype(cls) -> Type:
+        return float
+
+    @classmethod
+    def _smt_promote_literal(cls, literal) -> Optional[z3.SortRef]:
+        if isinstance(literal, float):
+            # return z3.FPVal(literal, _SMT_FLOAT_SORT)
+            return z3.RealVal(literal)
+        return None
 
     def __repr__(self):
         return self.statespace.find_model_value(self.var).__repr__()
 
     def __hash__(self):
         return self.statespace.find_model_value(self.var).__hash__()
 
     def __bool__(self):
-        return SmtBool(self.statespace, bool, self.var != 0).__bool__()
-    
+        return SmtBool(self.var != 0).__bool__()
+
+    def __int__(self):
+        var = self.var
+        return SmtInt(z3.If(var >= 0, z3.ToInt(var), -z3.ToInt(-var)))
+
     def __float__(self):
         return self.statespace.find_model_value(self.var).__float__()
 
     def __complex__(self):
         return complex(self.__float__())
 
     def __round__(self, ndigits=None):
         if ndigits is not None:
-            factor = 10 ** ndigits
+            factor = 10 ** realize(ndigits)  # realize to avoid exponentation-to-variable
             return round(self * factor) / factor
         else:
             var, floor, nearest = self.var, z3.ToInt(
                 self.var), z3.ToInt(self.var + _Z3_ONE_HALF)
-            return SmtInt(self.statespace, int, z3.If(var != floor + _Z3_ONE_HALF, nearest, z3.If(floor % 2 == 0, floor, floor + 1)))
+            return SmtInt(z3.If(var != floor + _Z3_ONE_HALF, nearest, z3.If(floor % 2 == 0, floor, floor + 1)))
 
     def __floor__(self):
-        return SmtInt(self.statespace, int, z3.ToInt(self.var))
+        return SmtInt(z3.ToInt(self.var))
 
     def __ceil__(self):
         var, floor = self.var, z3.ToInt(self.var)
-        return SmtInt(self.statespace, int, z3.If(var == floor, floor, floor + 1))
+        return SmtInt(z3.If(var == floor, floor, floor + 1))
 
     def __mod__(self, other):
         return realize(self) % realize(other) # TODO: z3 does not support modulo on reals
 
     def __trunc__(self):
         var, floor = self.var, z3.ToInt(self.var)
-        return SmtInt(self.statespace, int, z3.If(var >= 0, floor, floor + 1))
-
-    def __truediv__(self, other):
-        if other == 0:
-            raise ZeroDivisionError('division by zero')
-        return self._numeric_binary_op(other, operator.truediv)
+        return SmtInt(z3.If(var >= 0, floor, floor + 1))
 
 
-_CONVERSION_METHODS: Dict[Tuple[type, type], Any] = {
-    (bool, int): int,
-    (bool, float): float,
-    (bool, complex): complex,
-    (SmtBool, int): lambda i: SmtInt(i.statespace, int, smt_bool_to_int(i.var)),
-    (SmtBool, float): lambda i: SmtFloat(i.statespace, float, smt_bool_to_float(i.var)),
-    (SmtBool, complex): complex,
-    
-    (int, float): float,
-    (int, complex): complex,
-    (SmtInt, float): lambda i: SmtFloat(i.statespace, float, smt_int_to_float(i.var)),
-    (SmtInt, complex): complex,
-    
-    (float, complex): complex,
-    (SmtFloat, complex): complex,
-}
-
-def convert(val: object, target_type: type) -> object:
-    '''
-    Attempt to convert to the given type, as Python would perform
-    implicit conversion. Handles both crosshair and native values.
-    '''
-    orig_type = type(val)
-    converter = _CONVERSION_METHODS.get((orig_type, target_type))
-    if converter:
-        return converter(val)
-    return val
-
-def convert_to_common_type(val1: object, val2: object) -> Tuple[object, object]:
-    return (convert(val1, python_type(val2)),
-            convert(val2, python_type(val1)))
-
 class SmtDictOrSet(SmtBackedValue):
     '''
     TODO: Ordering is a challenging issue here.
     Modern pythons have in-order iteration for dictionaries but not sets.
     '''
-    def __init__(self, statespace: StateSpace, typ: Type, smtvar: object):
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type):
         self.key_pytype = normalize_pytype(type_arg_of(typ, 0))
-        self.smt_key_sort = type_to_smt_sort(self.key_pytype)
-        SmtBackedValue.__init__(self, statespace, typ, smtvar)
-        self.key_ch_type = crosshair_type_for_python_type(self.key_pytype)
+        ch_types = crosshair_types_for_python_type(self.key_pytype)
+        if ch_types:
+            self.ch_key_type: Optional[Type[AtomicSmtValue]] = ch_types[0]
+            self.smt_key_sort = self.ch_key_type._ch_smt_sort()
+        else:
+            self.ch_key_type = None
+            self.smt_key_sort = HeapRef
+        SmtBackedValue.__init__(self, smtvar, typ)
         self.statespace.add(self._len() >= 0)
 
     def _arr(self):
         return self.var[0]
 
     def _len(self):
         return self.var[1]
 
     def __len__(self):
-        return SmtInt(self.statespace, int, self._len())
+        return SmtInt(self._len())
 
     def __bool__(self):
-        return SmtBool(self.statespace, bool, self._len() != 0).__bool__()
+        return SmtBool(self._len() != 0).__bool__()
 
 
-class SmtDict(SmtDictOrSet, collections.abc.MutableMapping):
-    def __init__(self, space: StateSpace, typ: Type, smtvar: object):
+class SmtDict(SmtDictOrSet, collections.abc.Mapping):
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type):
+        space = context_statespace()
         self.val_pytype = normalize_pytype(type_arg_of(typ, 1))
-        self.smt_val_sort = type_to_smt_sort(self.val_pytype)
-        SmtDictOrSet.__init__(self, space, typ, smtvar)
-        self.val_ch_type = crosshair_type_for_python_type(self.val_pytype)
+        val_ch_types = crosshair_types_for_python_type(self.val_pytype)
+        if val_ch_types:
+            self.ch_val_type: Optional[Type[AtomicSmtValue]] = val_ch_types[0]
+            self.smt_val_sort = self.ch_val_type._ch_smt_sort()
+        else:
+            self.ch_val_type = None
+            self.smt_val_sort = HeapRef
+        SmtDictOrSet.__init__(self, smtvar, typ)
         arr_var = self._arr()
         len_var = self._len()
         self.val_missing_checker = arr_var.sort().range().recognizer(0)
         self.val_missing_constructor = arr_var.sort().range().constructor(0)
         self.val_constructor = arr_var.sort().range().constructor(1)
         self.val_accessor = arr_var.sort().range().accessor(1, 0)
         self.empty = z3.K(arr_var.sort().domain(),
                           self.val_missing_constructor())
-        self._iter_cache = []
+        self._iter_cache: List[z3.Const] = []
         space.add((arr_var == self.empty) == (len_var == 0))
         def list_can_be_iterated():
             list(self)
             return True
         space.defer_assumption('dict iteration is consistent with items', list_can_be_iterated)
 
     def __init_var__(self, typ, varname):
@@ -706,80 +862,63 @@
     def __eq__(self, other):
         (self_arr, self_len) = self.var
         has_heapref = smt_sort_has_heapref(
             self.var[1].sort()) or smt_sort_has_heapref(self.var[0].sort())
         if not has_heapref:
             if isinstance(other, SmtDict):
                 (other_arr, other_len) = other.var
-                return SmtBool(self.statespace, bool, z3.And(self_len == other_len, self_arr == other_arr))
+                return SmtBool(z3.And(self_len == other_len, self_arr == other_arr))
         # Manually check equality. Drive the loop from the (likely) concrete value 'other':
         if not isinstance(other, collections.abc.Mapping):
             return False
         if len(self) != len(other):
             return False
         for k, v in other.items():
-            if k not in self or self[k] != v:
+            self_v = self.get(k, _MISSING)
+            if self_v is _MISSING or self[k] != v:
                 return False
         return True
 
     def __repr__(self):
         return str(dict(self.items()))
 
-    def __setitem__(self, k, v):
-        missing = self.val_missing_constructor()
-        k = coerce_to_smt_sort(self.statespace, k, self.smt_key_sort)
-        v = coerce_to_smt_sort(self.statespace, v, self.smt_val_sort)
-        if k is None or v is None:
-            # TODO: dictionaries can become more losely typed as items are
-            # assigned. Dictionary is invariant, though, so we expect such cases
-            # to have been already caught by the type checker.
-            raise CrosshairUnsupported('dictionary assignment with conflicting types')
-        old_arr, old_len = self.var
-        new_len = z3.If(z3.Select(old_arr, k) == missing, old_len + 1, old_len)
-        self.var = (z3.Store(old_arr, k, self.val_constructor(v)), new_len)
-
-    def __delitem__(self, pykey):
-        missing = self.val_missing_constructor()
-        k = force_to_smt_sort(self.statespace, pykey, self.smt_key_sort)
-        old_arr, old_len = self.var
-        if SmtBool(self.statespace, bool, z3.Select(old_arr, k) == missing).__bool__():
-            raise KeyError(pykey)
-        if SmtBool(self.statespace, bool, self._len() == 0).__bool__():
-            raise IgnoreAttempt('SmtDict in inconsistent state')
-        self.var = (z3.Store(old_arr, k, missing), old_len - 1)
-
     def __getitem__(self, k):
         with self.statespace.framework():
-            smt_key = coerce_to_smt_sort(self.statespace, k, self.smt_key_sort)
+            smt_key = None
+            if self.ch_key_type:
+                smt_key = self.ch_key_type._coerce_to_smt_sort(k)
             if smt_key is None:
-                # A key of the wrong type cannot be present.
-                # Try to raise the right exception:
                 if getattr(k, '__hash__', None) is None:
                     raise TypeError("unhashable type")
-                else:
-                    raise KeyError(k)
+                for self_k in iter(self):
+                    if self_k == k:
+                        return self[self_k]
+                raise KeyError(k)
             possibly_missing = self._arr()[smt_key]
             is_missing = self.val_missing_checker(possibly_missing)
-            if SmtBool(self.statespace, bool, is_missing).__bool__():
+            if SmtBool(is_missing).__bool__():
                 raise KeyError(k)
-            if SmtBool(self.statespace, bool, self._len() == 0).__bool__():
+            if SmtBool(self._len() == 0).__bool__():
                 raise IgnoreAttempt('SmtDict in inconsistent state')
             return smt_to_ch_value(self.statespace,
                                    self.snapshot,
                                    self.val_accessor(possibly_missing),
                                    self.val_pytype)
 
+    def __reversed__(self):
+        return reversed(list(self))
+
     def __iter__(self):
         arr_var, len_var = self.var
         iter_cache = self._iter_cache
         space = self.statespace
         idx = 0
         arr_sort = self._arr().sort()
         is_missing = self.val_missing_checker
-        while SmtBool(space, bool, idx < len_var).__bool__():
+        while SmtBool(idx < len_var).__bool__():
             if not space.choose_possible(arr_var != self.empty, favor_true=True):
                 raise IgnoreAttempt('SmtDict in inconsistent state')
             k = z3.Const('k' + str(idx) + space.uniq(),
                          arr_sort.domain())
             v = z3.Const('v' + str(idx) + space.uniq(),
                          self.val_constructor.domain(0))
             remaining = z3.Const('remaining' + str(idx) +
@@ -806,34 +945,34 @@
             arr_var = remaining
         # In this conditional, we reconcile the parallel symbolic variables for length
         # and contents:
         if not space.choose_possible(arr_var == self.empty, favor_true=True):
             raise IgnoreAttempt('SmtDict in inconsistent state')
 
     def copy(self):
-        return SmtDict(self.statespace, self.python_type, self.var)
+        return SmtDict(self.var, self.python_type)
 
     # TODO: investigate this approach for type masquerading:
     # @property
     # def __class__(self):
     #    return dict
 
 
 class SmtSet(SmtDictOrSet, collections.abc.Set):
-    def __init__(self, statespace: StateSpace, typ: Type, smtvar: object):
-        SmtDictOrSet.__init__(self, statespace, typ, smtvar)
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type):
+        SmtDictOrSet.__init__(self, smtvar, typ)
         self.empty = z3.K(self._arr().sort().domain(), False)
         self.statespace.add((self._arr() == self.empty) == (self._len() == 0))
 
     def __eq__(self, other):
         (self_arr, self_len) = self.var
         if isinstance(other, SmtSet):
             (other_arr, other_len) = other.var
             if other_arr.sort() == self_arr.sort():
-                return SmtBool(self.statespace, bool, z3.And(self_len == other_len, self_arr == other_arr))
+                return SmtBool(z3.And(self_len == other_len, self_arr == other_arr))
         if not isinstance(other, (set, frozenset, SmtSet)):
             return False
         # Manually check equality. Drive size from the (likely) concrete value 'other':
         if len(self) != len(other):
             return False
         # Then iterate on self (iteration will create a lot of good symbolic constraints):
         for item in self:
@@ -848,39 +987,42 @@
                 return False
         return True
 
     def __init_var__(self, typ, varname):
         assert typ == self.python_type
         return (
             z3.Const(varname + '_map' + self.statespace.uniq(),
-                     z3.ArraySort(type_to_smt_sort(self.key_pytype),
-                                  z3.BoolSort())),
+                     z3.ArraySort(self.smt_key_sort, z3.BoolSort())),
             z3.Const(varname + '_len' + self.statespace.uniq(), z3.IntSort())
         )
 
-    def __contains__(self, raw_key):
-        converted_key = convert(raw_key, self.key_pytype) # handle implicit numeric conversions
-        k = coerce_to_smt_sort(self.statespace, converted_key, self._arr().sort().domain())
+    def __contains__(self, key):
+        if getattr(key, '__hash__', None) is None:
+            raise TypeError("unhashable type")
+        if self.ch_key_type:
+            k = self.ch_key_type._coerce_to_smt_sort(key)
+        else:
+            k = None
         if k is not None:
             present = self._arr()[k]
-            return SmtBool(self.statespace, bool, present)
+            return SmtBool(present)
         # Fall back to standard equality and iteration
         for self_item in self:
-            if self_item == raw_key:
+            if self_item == key:
                 return True
         return False
 
     def __iter__(self):
         arr_var, len_var = self.var
         idx = 0
         arr_sort = self._arr().sort()
         keys_on_heap = smt_sort_has_heapref(arr_sort.domain())
         already_yielded = []
-        while SmtBool(self.statespace, bool, idx < len_var).__bool__():
-            if SmtBool(self.statespace, bool, arr_var == self.empty).__bool__():
+        while SmtBool(idx < len_var).__bool__():
+            if SmtBool(arr_var == self.empty).__bool__():
                 raise IgnoreAttempt('SmtSet in inconsistent state')
             k = z3.Const('k' + str(idx) + self.statespace.uniq(),
                          arr_sort.domain())
             remaining = z3.Const('remaining' + str(idx) +
                                  self.statespace.uniq(), arr_sort)
             idx += 1
             self.statespace.add(arr_var == z3.Store(remaining, k, True))
@@ -892,15 +1034,15 @@
                     if ch_value == previous_value:
                         raise IgnoreAttempt('Duplicate items in set')
                 already_yielded.append(ch_value)
             yield ch_value
             arr_var = remaining
         # In this conditional, we reconcile the parallel symbolic variables for length
         # and contents:
-        if SmtBool(self.statespace, bool, arr_var != self.empty).__bool__():
+        if SmtBool(arr_var != self.empty).__bool__():
             raise IgnoreAttempt('SmtSet in inconsistent state')
 
     def _set_op(self, attr, other):
         # We need to check the type of other here, because builtin sets
         # do not accept iterable args (but the abc Set does)
         if isinstance(other, collections.abc.Set):
             return getattr(collections.abc.Set, attr)(self, other)
@@ -934,36 +1076,14 @@
         return self._set_op('__xor__', other)
     __rxor__ = __xor__
 
     def __sub__(self, other):
         return self._set_op('__sub__', other)
 
 
-class SmtMutableSet(SmtSet):
-    def __repr__(self):
-        return str(set(self))
-
-    @classmethod
-    def _from_iterable(cls, it):
-        # overrides collections.abc.Set's version
-        return set(it)
-
-    def add(self, k):
-        k = coerce_to_smt_var(self.statespace, k)
-        old_arr, old_len = self.var
-        new_len = z3.If(z3.Select(old_arr, k), old_len, old_len + 1)
-        self.var = (z3.Store(old_arr, k, True), new_len)
-
-    def discard(self, k):
-        k = coerce_to_smt_var(self.statespace, k)
-        old_arr, old_len = self.var
-        new_len = z3.If(z3.Select(old_arr, k), old_len - 1, old_len)
-        self.var = (z3.Store(old_arr, k, False), new_len)
-
-
 class SmtFrozenSet(SmtSet):
     def __repr__(self):
         return frozenset(self).__repr__()
 
     def __hash__(self):
         return frozenset(self).__hash__()
 
@@ -974,53 +1094,54 @@
 
 
 def process_slice_vs_symbolic_len(
         space: StateSpace,
         i: slice,
         smt_len: z3.ExprRef
 ) -> Union[z3.ExprRef, Tuple[z3.ExprRef, z3.ExprRef]]:
-    def normalize_symbolic_index(idx):
-        if isinstance(idx, int):
-            return idx if idx >= 0 else smt_len + idx
+    def normalize_symbolic_index(idx) -> z3.ExprRef:
+        if type(idx) is int:
+            return z3.IntVal(idx) if idx >= 0 else (smt_len + z3.IntVal(idx))
         else:
-            idx = force_to_smt_sort(space, idx, z3.IntSort())
+            idx = SmtInt._coerce_to_smt_sort(idx)
             return z3.If(idx >= 0, idx, smt_len + idx)
-    if isinstance(i, int) or isinstance(i, SmtInt):
-        smt_i = smt_coerce(i)
+    if isinstance(i, (int, SmtInt)):
+        smt_i = SmtInt._coerce_to_smt_sort(i)
         if space.smt_fork(z3.Or(smt_i >= smt_len, smt_i < -smt_len)):
             raise IndexError(f'index "{i}" is out of range')
-        smt_i = normalize_symbolic_index(smt_i)
-        return force_to_smt_sort(space, smt_i, z3.IntSort())
+        return normalize_symbolic_index(i)
     elif isinstance(i, slice):
-        smt_start, smt_stop, smt_step = (i.start, i.stop, i.step)
-        if smt_step not in (None, 1):
-            raise CrosshairUnsupported('slice steps not handled')
+        start, stop, step = (i.start, i.stop, i.step)
+        for x in (start, stop, step):
+            if (x is not None) and (not hasattr(x, '__index__')):
+                raise TypeError('slice indices must be integers or None or have an __index__ method')
+        if step not in (None, 1):
+            raise CrosshairUnsupported('slice steps not handled') # TODO: handle this!
         start = normalize_symbolic_index(
-            smt_start) if i.start is not None else 0
+            start) if i.start is not None else z3.IntVal(0)
         stop = normalize_symbolic_index(
-            smt_stop) if i.stop is not None else smt_len
-        return (force_to_smt_sort(space, start, z3.IntSort()),
-                force_to_smt_sort(space, stop, z3.IntSort()))
+            stop) if i.stop is not None else smt_len
+        return (start, stop)
     else:
         raise TypeError(
             'indices must be integers or slices, not ' + str(type(i)))
 
 
-class SmtSequence(SmtBackedValue):
+class SmtSequence(SmtBackedValue, collections.abc.Sequence):
     def __iter__(self):
         idx = 0
         while len(self) > idx:
             yield self[idx]
             idx += 1
 
     def __len__(self):
-        return SmtInt(self.statespace, int, z3.Length(self.var))
+        return SmtInt(z3.Length(self.var))
 
     def __bool__(self):
-        return SmtBool(self.statespace, bool, z3.Length(self.var) > 0).__bool__()
+        return SmtBool(z3.Length(self.var) > 0).__bool__()
 
     def __mul__(self, other):
         if not isinstance(other, int):
             raise TypeError("can't multiply by non-int")
         if other <= 0:
             return self[0:0]
         ret = self
@@ -1029,31 +1150,34 @@
         return ret
 
     def __rmul__(self, other):
         return self.__mul__(other)
 
 
 class SmtArrayBasedUniformTuple(SmtSequence):
-    def __init__(self, statespace: StateSpace, typ: Type, smtvar: Union[str, Tuple]):
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type):
         if type(smtvar) == str:
             pass
         else:
             assert type(smtvar) is tuple, f'incorrect type {type(smtvar)}'
             assert len(smtvar) == 2
+
         self.val_pytype = normalize_pytype(type_arg_of(typ, 0))
-        self.item_smt_sort = (HeapRef if pytype_uses_heap(self.val_pytype)
-                              else type_to_smt_sort(self.val_pytype))
-        self.key_pytype = int
-        SmtBackedValue.__init__(self, statespace, typ, smtvar)
+        ch_types = crosshair_types_for_python_type(self.val_pytype)
+        if ch_types:
+            self.ch_item_type: Optional[Type[AtomicSmtValue]] = ch_types[0]
+            self.item_smt_sort = self.ch_item_type._ch_smt_sort()
+        else:
+            self.ch_item_type = None
+            self.item_smt_sort = HeapRef
+
+        SmtBackedValue.__init__(self, smtvar, typ)
         arr_var = self._arr()
         len_var = self._len()
         self.statespace.add(len_var >= 0)
-        
-        self.val_ch_type = crosshair_type_for_python_type(self.val_pytype)
-        
 
     def __init_var__(self, typ, varname):
         assert typ == self.python_type
         arr_smt_type = z3.ArraySort(z3.IntSort(), self.item_smt_sort)
         return (
             z3.Const(varname + '_map' + self.statespace.uniq(), arr_smt_type),
             z3.Const(varname + '_len' + self.statespace.uniq(), z3.IntSort())
@@ -1062,19 +1186,19 @@
     def _arr(self):
         return self.var[0]
 
     def _len(self):
         return self.var[1]
 
     def __len__(self):
-        return SmtInt(self.statespace, int, self._len())
+        return SmtInt(self._len())
+
+    def __bool__(self) -> bool:
+        return SmtBool(self._len() != 0).__bool__()
 
-    def __bool__(self):
-        return SmtBool(self.statespace, bool, self._len() != 0).__bool__()
-    
     def __eq__(self, other):
         if self is other:
             return True
         (self_arr, self_len) = self.var
         if not is_iterable(other):
             return False
         if len(self) != len(other):
@@ -1094,39 +1218,43 @@
 
     def __delitem__(self, k):
         raise CrosshairInternal()
 
     def __iter__(self):
         arr_var, len_var = self.var
         idx = 0
-        while SmtBool(self.statespace, bool, idx < len_var).__bool__():
+        while SmtBool(idx < len_var).__bool__():
             yield smt_to_ch_value(self.statespace,
                                   self.snapshot,
                                   z3.Select(arr_var, idx),
                                   self.val_pytype)
             idx += 1
 
-    def __add__(self, other):
-        return SequenceConcatenation(self, other)
+    def __add__(self, other: object):
+        if isinstance(other, collections.abc.Sequence):
+            return SequenceConcatenation(self, other)
+        return NotImplemented
 
-    def __radd__(self, other):
-        return SequenceConcatenation(other, self)
+    def __radd__(self, other: object):
+        if isinstance(other, collections.abc.Sequence):
+            return SequenceConcatenation(other, self)
+        return NotImplemented
 
     def __contains__(self, other):
         space = self.statespace
         with space.framework():
             if not smt_sort_has_heapref(self.item_smt_sort):
-                smt_other = coerce_to_smt_sort(space, other, self.item_smt_sort)
+                smt_other = self.ch_item_type._coerce_to_smt_sort(other)
                 if smt_other is not None:
                     # OK to perform a symbolic comparison
                     idx = z3.Const('possible_idx' + space.uniq(), z3.IntSort())
                     idx_in_range = z3.Exists(idx, z3.And(0 <= idx,
                                                          idx < self._len(),
                                                          z3.Select(self._arr(), idx) == smt_other))
-                    return SmtBool(space, bool, idx_in_range)
+                    return SmtBool(idx_in_range)
             # Fall back to standard equality and iteration
             for self_item in self:
                 if self_item == other:
                     return True
             return False
 
     def __getitem__(self, i):
@@ -1134,16 +1262,16 @@
         with space.framework():
             if i == slice(None, None, None):
                 return self
             idx_or_pair = process_slice_vs_symbolic_len(space, i, self._len())
             if isinstance(idx_or_pair, tuple):
                 (start, stop) = idx_or_pair
                 (myarr, mylen) = self.var
-                start = SmtInt(space, int, start)
-                stop = SmtInt(space, int, smt_min(mylen, smt_coerce(stop)))
+                start = SmtInt(start)
+                stop = SmtInt(smt_min(mylen, smt_coerce(stop)))
                 return SliceView(self, start, stop)
             else:
                 smt_result = z3.Select(self._arr(), idx_or_pair)
                 return smt_to_ch_value(space, self.snapshot, smt_result, self.val_pytype)
 
     def insert(self, idx, obj):
         raise CrosshairUnsupported
@@ -1178,55 +1306,76 @@
             cur = self[i]
             if cur == value:
                 return cur
             i += 1
         raise ValueError(f'{value} is not in list')
 
 
-class SmtType(SmtBackedValue):
-    _realization : Optional[Type] = None
-    def __init__(self, statespace: StateSpace, typ: Type, smtvar: object):
+class SmtType(AtomicSmtValue, SmtBackedValue):
+    _realization: Optional[Type] = None
+
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type):
+        space = context_statespace()
         assert origin_of(typ) is type
         self.pytype_cap = origin_of(typ.__args__[0]) if hasattr(typ, '__args__') else object
         assert type(self.pytype_cap) is type
-        smt_cap = statespace.type_repo.get_type(self.pytype_cap)
-        SmtBackedValue.__init__(self, statespace, typ, smtvar)
-        statespace.add(statespace.type_repo.smt_issubclass(self.var, smt_cap))
+        smt_cap = space.type_repo.get_type(self.pytype_cap)
+        SmtBackedValue.__init__(self, smtvar, typ)
+        space.add(space.type_repo.smt_issubclass(self.var, smt_cap))
+
+    @classmethod
+    def _ch_smt_sort(cls) -> z3.SortRef:
+        return PYTYPE_SORT
+
+    @classmethod
+    def _pytype(cls) -> Type:
+        return type
+
+    @classmethod
+    def _smt_promote_literal(cls, literal) -> Optional[z3.SortRef]:
+        if isinstance(literal, type):
+            return context_statespace().type_repo.get_type(literal)
+        return None
+
     def _is_superclass_of_(self, other):
         if self is SmtType:
             return False
         if type(other) is SmtType:
             # Prefer it this way because only _is_subcless_of_ does the type cap lowering.
             return other._is_subclass_of_(self)
         space = self.statespace
         with space.framework():
-            coerced = coerce_to_smt_sort(space, other, self.var.sort())
+            coerced = SmtType._coerce_to_smt_sort(other)
             if coerced is None:
                 return False
-            return SmtBool(space, bool, space.type_repo.smt_issubclass(coerced, self.var))
+            return SmtBool(space.type_repo.smt_issubclass(coerced, self.var))
+
     def _is_subclass_of_(self, other):
         if self is SmtType:
             return False
         space = self.statespace
         with space.framework():
-            coerced = coerce_to_smt_sort(space, other, self.var.sort())
+            coerced = SmtType._coerce_to_smt_sort(other)
             if coerced is None:
                 return False
-            ret = SmtBool(space, bool, space.type_repo.smt_issubclass(self.var, coerced))
+            ret = SmtBool(space.type_repo.smt_issubclass(self.var, coerced))
             other_pytype = other.pytype_cap if type(other) is SmtType else other
             # consider lowering the type cap
             if other_pytype is not self.pytype_cap and issubclass(other_pytype, self.pytype_cap) and ret:
                 self.pytype_cap = other_pytype
             return ret
+
     def __ch_realize__(self):
         return self._realized()
+
     def _realized(self):
         if self._realization is None:
             self._realization = self._realize()
         return self._realization
+
     def _realize(self) -> Type:
         cap = self.pytype_cap
         space = self.statespace
         if cap is object:
             pytype_to_smt = space.type_repo.pytype_to_smt
             for pytype, smt_type in pytype_to_smt.items():
                 if not issubclass(pytype, cap):
@@ -1236,20 +1385,27 @@
             raise CrosshairUnsupported('Will not exhaustively attempt `object` types')
         else:
             subtype = choose_type(space, cap)
             smt_type = space.type_repo.get_type(subtype)
             if space.smt_fork(self.var != smt_type):
                 raise IgnoreAttempt
             return subtype
+
+    def __call__(self, *a, **kw):
+        return self._realized()(*a, **kw)
+
     def __bool__(self):
         return True
+
     def __copy__(self):
         return self if self._realization is None else self._realization
+
     def __repr__(self):
         return repr(self._realized())
+
     def __hash__(self):
         return hash(self._realized())
 
 
 class LazyObject(ObjectProxy):
     _inner: object = _MISSING
 
@@ -1268,40 +1424,40 @@
         if inner is _MISSING:
             # CrossHair will deepcopy for mutation checking.
             # That's usually bad for LazyObjects, which want to defer their
             # realization, so we simply don't do mutation checking for these
             # kinds of values right now.
             return self
         else:
-            return copy.deepcopy(self.wrapped())
+            return copy.deepcopy(inner) # self.wrapped())
 
 
 class SmtObject(LazyObject, CrossHairValue):
     '''
     An object with an unknown type.
     We lazily create a more specific smt-based value in hopes that an
     isinstance() check will be called before something is accessed on us.
     Note that this class is not an SmtBackedValue, but its _typ and _inner
     members can be.
     '''
-    def __init__(self, space: StateSpace, typ: Type, varname: object):
-        object.__setattr__(self, '_typ', SmtType(space, type, varname))
-        object.__setattr__(self, '_space', space)
-        object.__setattr__(self, '_varname', varname)
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type):
+        object.__setattr__(self, '_typ', SmtType(smtvar, type))
+        object.__setattr__(self, '_space', context_statespace())
+        object.__setattr__(self, '_varname', smtvar)
 
     def _realize(self):
         space = object.__getattribute__(self, '_space')
         varname = object.__getattribute__(self, '_varname')
 
         typ = object.__getattribute__(self, '_typ')
         pytype = realize(typ)
         debug('materializing symbolic object as an instance of', pytype)
         if pytype is object:
             return object()
-        return proxy_for_type(pytype, space, varname, allow_subtypes=False)
+        return proxy_for_type(pytype, varname, allow_subtypes=False)
 
     @property
     def python_type(self):
         return object.__getattribute__(self, '_typ')
 
     @property
     def __class__(self):
@@ -1311,51 +1467,61 @@
     def __class__(self, value):
         raise CrosshairUnsupported
 
 
 class SmtCallable(SmtBackedValue):
     __closure__ = None
 
-    def __init___(self, statespace: StateSpace, typ: Type, smtvar: object):
-        SmtBackedValue.__init__(self, statespace, typ, smtvar)
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type):
+        SmtBackedValue.__init__(self, smtvar, typ)
 
     def __bool__(self):
         return True
 
     def __eq__(self, other):
         return (self.var is other.var) if isinstance(other, SmtCallable) else False
 
     def __hash__(self):
         return id(self.var)
 
-    def __init_var__(self, typ, varname):
-        type_args = type_args_of(self.python_type)
+    def __init_var__(self, typ: type, varname):
+        type_args: Tuple[Any, ...] = type_args_of(self.python_type)
         if not type_args:
-            type_args = [..., Any]
+            type_args = (..., Any)
         (self.arg_pytypes, self.ret_pytype) = type_args
         if self.arg_pytypes == ...:
             raise CrosshairUnsupported
-        self.arg_ch_type = map(
-            crosshair_type_for_python_type, self.arg_pytypes)
-        self.ret_ch_type = crosshair_type_for_python_type(self.ret_pytype)
-        all_pytypes = tuple(self.arg_pytypes) + (self.ret_pytype,)
+        arg_ch_types = []
+        for arg_pytype in self.arg_pytypes:
+            ch_types = crosshair_types_for_python_type(arg_pytype)
+            if not ch_types:
+                raise CrosshairUnsupported
+            arg_ch_types.append(ch_types[0])
+        self.arg_ch_types = arg_ch_types
+        self.ret_ch_type = crosshair_types_for_python_type(self.ret_pytype)[0]
         return z3.Function(varname + self.statespace.uniq(),
-                           *map(type_to_smt_sort, self.arg_pytypes),
-                           type_to_smt_sort(self.ret_pytype))
+                           *[ch_type._ch_smt_sort() for ch_type in arg_ch_types],
+                           self.ret_ch_type._ch_smt_sort())
 
     def __ch_realize__(self):
         return self  # we don't realize callables right now
 
     def __call__(self, *args):
-        if len(args) != len(self.arg_pytypes):
+        space = self.statespace
+        if len(args) != len(self.arg_ch_types):
             raise TypeError('wrong number of arguments')
-        args = (coerce_to_smt_var(self.statespace, a) for a in args)
-        smt_ret = self.var(*args)
+        smt_args = []
+        for actual_arg, ch_type in zip(args, self.arg_ch_types):
+            smt_arg = ch_type._coerce_to_smt_sort(actual_arg)
+            if smt_arg is None:
+                raise TypeError
+            smt_args.append(smt_arg)
+        smt_ret = self.var(*smt_args)
         # TODO: detect that `smt_ret` might be a HeapRef here
-        return self.ret_ch_type(self.statespace, self.ret_pytype, smt_ret)
+        return self.ret_ch_type(smt_ret, self.ret_pytype)
 
     def __repr__(self):
         finterp = self.statespace.find_model_value_for_function(self.var)
         if finterp is None:
             # (z3 model completion will not interpret a function for me currently)
             return 'lambda *a: None'
         # 0-arg interpretations seem to be simply values:
@@ -1380,160 +1546,207 @@
     def __repr__(self):
         return tuple(self).__repr__()
 
     def __hash__(self):
         return tuple(self).__hash__()
 
 
-class SmtStr(SmtSequence, AbcString):
-    def __init__(self, statespace: StateSpace, typ: Type, smtvar: object):
+class SmtStr(AtomicSmtValue, SmtSequence, AbcString):
+    def __init__(self, smtvar: Union[str, z3.ExprRef], typ: Type = str):
         assert typ == str
-        SmtBackedValue.__init__(self, statespace, typ, smtvar)
+        SmtBackedValue.__init__(self, smtvar, typ)
         self.item_pytype = str
-        self.item_ch_type = SmtStr
+
+    @classmethod
+    def _ch_smt_sort(cls) -> z3.SortRef:
+        return z3.StringSort()
+
+    @classmethod
+    def _pytype(cls) -> Type:
+        return str
+
+    @classmethod
+    def _smt_promote_literal(cls, literal) -> Optional[z3.SortRef]:
+        if isinstance(literal, str):
+            return z3.StringVal(literal)
+        return None
 
     def __str__(self):
         return self.statespace.find_model_value(self.var)
 
     def __copy__(self):
-        return SmtStr(self.statespace, str, self.var)
+        return SmtStr(self.var)
 
     def __repr__(self):
         return repr(self.__str__())
 
     def __hash__(self):
         return hash(self.__str__())
 
     def __add__(self, other):
-        return self._binary_op(other, operator.add)
+        if isinstance(other, (SmtStr, str)):
+            return SmtStr(self.var + smt_coerce(other))
+        raise TypeError
 
     def __radd__(self, other):
-        return self._binary_op(other, lambda a, b: b + a)
+        if isinstance(other, (SmtStr, str)):
+            return SmtStr(smt_coerce(other) + self.var)
+        raise TypeError
 
     def __mul__(self, other):
         space = self.statespace
         # If repetition count is a literal, use that first:
-        if type(other) == int:
+        if isinstance(other, Integral):
             if other <= 1:
                 return self if other == 1 else ''
-            return SmtStr(space, str, z3.Concat(*[self.var for _ in range(other)]))
-        # Else, create a new symbolic string that regex-matches as a repetition.
-        # Z3 cannot do much with a symbolic regex, so we'll force ourselves into
-        # a concrete string.
-        concrete_self = self.__str__()
-        count = force_to_smt_sort(space, other, z3.IntSort())
-        result = SmtStr(space, str, str(self.var) + '_mul' + space.uniq())
-        space.add(z3.InRe(result.var, z3.Star(z3.Re(concrete_self))))
-        space.add(z3.Length(result.var) == len(concrete_self) * count)
-        return result
+            # Note that in SmtInt, we attempt string multiplication via regex.
+            # Z3 cannot do much with a symbolic regex, so we case-split on
+            # the repetition count.
+            return SmtStr(z3.Concat(*[self.var for _ in range(other)]))
+        return NotImplemented
+    __rmul__ = __mul__
 
     def __mod__(self, other):
         return self.__str__() % realize(other)
 
     def _cmp_op(self, other, op):
-        forced = force_to_smt_sort(self.statespace, other, self.var.sort())
-        return SmtBool(self.statespace, bool, op(self.var, forced))
+        forced = force_to_smt_sort(other, SmtStr)
+        return SmtBool(op(self.var, forced))
 
     def __lt__(self, other):
-        return self._cmp_op(other, operator.lt)
+        return self._cmp_op(other, ops.lt)
 
     def __le__(self, other):
-        return self._cmp_op(other, operator.le)
+        return self._cmp_op(other, ops.le)
 
     def __gt__(self, other):
-        return self._cmp_op(other, operator.gt)
+        return self._cmp_op(other, ops.gt)
 
     def __ge__(self, other):
-        return self._cmp_op(other, operator.ge)
+        return self._cmp_op(other, ops.ge)
 
     def __contains__(self, other):
-        forced = force_to_smt_sort(self.statespace, other, self.var.sort())
-        return SmtBool(self.statespace, bool, z3.Contains(self.var, forced))
+        forced = force_to_smt_sort(other, SmtStr)
+        return SmtBool(z3.Contains(self.var, forced))
 
     def __getitem__(self, i):
         idx_or_pair = process_slice_vs_symbolic_len(
             self.statespace, i, z3.Length(self.var))
         if isinstance(idx_or_pair, tuple):
             (start, stop) = idx_or_pair
             smt_result = z3.Extract(self.var, start, stop - start)
         else:
             smt_result = z3.Extract(self.var, idx_or_pair, 1)
-        return SmtStr(self.statespace, str, smt_result)
+        return SmtStr(smt_result)
 
     def find(self, substr, start=None, end=None):
-        if end is None:
-            return SmtInt(self.statespace, int,
-                          z3.IndexOf(self.var, smt_coerce(substr), start or 0))
-        else:
-            return self.__getitem__(slice(start, end, 1)).index(s)
+        smt_mystr = self.var
+        smt_substr = force_to_smt_sort(substr, SmtStr)
+        if end is not None:
+            end = force_to_smt_sort(end, SmtInt)
+            smt_mystr = z3.SubString(smt_mystr, 0, end)
+        start = 0 if start is None else force_to_smt_sort(start, SmtInt)
+        return SmtInt(z3.IndexOf(smt_mystr, smt_substr, start))
+
+    def index(self, substr, start=None, end=None):
+        idx = self.find(substr, start, end)
+        if idx == -1:
+            raise ValueError
+        return idx
+
+    def startswith(self, substr):
+        smt_substr = force_to_smt_sort(substr, SmtStr)
+        return SmtBool(z3.PrefixOf(smt_substr, self.var))
+
+    def endswith(self, substr):
+        smt_substr = force_to_smt_sort(substr, SmtStr)
+        return SmtBool(z3.SuffixOf(smt_substr, self.var))
+
+    def split(self, sep:Optional[str] = None, maxsplit:int = -1):
+        if sep is None:
+            return self.__str__().split(sep=sep, maxsplit=maxsplit)
+        smt_sep = force_to_smt_sort(sep, SmtStr)
+        if not isinstance(maxsplit, Integral):
+            raise TypeError
+        if maxsplit == 0:
+            return [self]
+        first_occurance = SmtInt(z3.IndexOf(self.var, smt_sep, 0))
+        if first_occurance == -1:
+            return [self]
+        ret = [self[:cast(int, first_occurance)]]
+        new_maxsplit = -1 if maxsplit == -1 else maxsplit - 1
+        ret.extend(self[first_occurance+1:].split(sep=sep, maxsplit=new_maxsplit))
+        return ret
 
 
 _CACHED_TYPE_ENUMS: Dict[FrozenSet[type], z3.SortRef] = {}
 
 
 _PYTYPE_TO_WRAPPER_TYPE = {
-    type(None): (lambda *a: None),
-    bool: SmtBool,
-    int: SmtInt,
-    float: SmtFloat,
-    str: SmtStr,
-    list: SmtList,
-    dict: SmtDict,
-    set: SmtMutableSet,
-    frozenset: SmtFrozenSet,
-    type: SmtType,
+    bool: (SmtBool,),
+    int: (SmtInt,),
+    float: (SmtFloat,),
+    str: (SmtStr,),
+    type: (SmtType,),
 }
 
 # Type ignore pending https://github.com/python/mypy/issues/6864
-_PYTYPE_TO_WRAPPER_TYPE[collections.abc.Callable] = SmtCallable  # type:ignore
+_PYTYPE_TO_WRAPPER_TYPE[collections.abc.Callable] = (SmtCallable,)  # type:ignore
 
 _WRAPPER_TYPE_TO_PYTYPE = dict((v, k)
-                               for (k, v) in _PYTYPE_TO_WRAPPER_TYPE.items())
+                               for (k, vs) in _PYTYPE_TO_WRAPPER_TYPE.items()
+                               for v in vs)
 
 
 #
 # Proxy making helpers
 #
 
 def make_union_choice(creator, *pytypes):
     for typ in pytypes[:-1]:
         if creator.space.smt_fork():
             return creator(typ)
     return creator(pytypes[-1])
 
 def make_optional_smt(smt_type):
     def make(creator, *type_args):
-        ret = smt_type(creator.space, creator.pytype, creator.varname)
+        ret = smt_type(creator.varname, creator.pytype)
         if creator.space.fork_parallel(false_probability=0.98):
             debug('Prematurely realizing', creator.pytype, 'value')
             ret = realize(ret)
         return ret
     return make
 
 def make_dictionary(creator, key_type = Any, value_type = Any):
     space, varname = creator.space, creator.varname
-    if smt_sort_has_heapref(type_to_smt_sort(key_type)):
+    if pytype_uses_heap(key_type):
         kv = proxy_for_type(List[Tuple[key_type, value_type]], # type: ignore
-                            space, varname + 'items', allow_subtypes=False)
+                            varname + 'items', allow_subtypes=False)
         orig_kv = kv[:]
         def ensure_keys_are_unique() -> bool:
             return len(set(k for k, _ in orig_kv)) == len(orig_kv)
         space.defer_assumption('dict keys are unique', ensure_keys_are_unique)
         return SimpleDict(kv)
-    return SmtDict(space, creator.pytype, varname)
+    return ShellMutableMap(SmtDict(varname, creator.pytype))
 
 def make_tuple(creator, *type_args):
     if not type_args:
         type_args = (object, ...)  # type: ignore
     if len(type_args) == 2 and type_args[1] == ...:
-        return SmtUniformTuple(creator.space, creator.pytype, creator.varname)
+        return SmtUniformTuple(creator.varname, creator.pytype)
     else:
-        return tuple(proxy_for_type(t, creator.space, creator.varname + '_at_' + str(idx), allow_subtypes=True)
+        return tuple(proxy_for_type(t, creator.varname + '_at_' + str(idx), allow_subtypes=True)
                      for (idx, t) in enumerate(type_args))
 
+def make_set(creator, *type_args):
+    if type_args:
+        return ShellMutableSet(creator(FrozenSet.__getitem__(*type_args)))
+    else:
+        return ShellMutableSet(creator(FrozenSet))
+
 def make_raiser(exc, *a) -> Callable:
     def do_raise(*ra, **rkw) -> NoReturn:
         raise exc(*a)
     return do_raise
 
 #
 # Monkey Patches
@@ -1667,15 +1880,15 @@
     return '[' + ', '.join(repr(x) for x in self) + ']'
 
 @functools.singledispatch
 def _max(*values, key=lambda x: x, default=_MISSING):
     return _max_iter(values, key=key, default=default)
 
 
-@_max.register(collections.Iterable)  # TODO: I think this explodes: max([1,2], [3], key=len)
+@_max.register(collections.abc.Iterable)  # TODO: I think this explodes: max([1,2], [3], key=len)
 def _max_iter(values: Iterable[_T], *, key: Callable = lambda x: x, default: Union[_Missing, _VT] = _MISSING) -> _T:
     '''
     pre: bool(values) or default is not _MISSING
     post[]::
       (_ in values) if default is _MISSING else True
       ((_ in values) or (_ is default)) if default is not _MISSING else True
     '''
@@ -1684,15 +1897,15 @@
 
 
 @functools.singledispatch
 def _min(*values, key=lambda x: x, default=_MISSING):
     return _min_iter(values, key=key, default=default)
 
 
-@_min.register(collections.Iterable)
+@_min.register(collections.abc.Iterable)
 def _min_iter(values: Iterable[_T], *, key: Callable = lambda x: x, default: Union[_Missing, _VT] = _MISSING) -> _T:
     '''
     pre: bool(values) or default is not _MISSING
     post[]::
       (_ in values) if default is _MISSING else True
       ((_ in values) or (_ is default)) if default is not _MISSING else True
     '''
@@ -1714,23 +1927,23 @@
     register_type(bool, make_optional_smt(SmtBool))
     register_type(int, make_optional_smt(SmtInt))
     register_type(float, make_optional_smt(SmtFloat))
     register_type(str, make_optional_smt(SmtStr))
     register_type(list, make_optional_smt(SmtList))
     register_type(dict, make_dictionary)
     register_type(tuple, make_tuple)
-    register_type(set, make_optional_smt(SmtMutableSet))
+    register_type(set, make_set)
     register_type(frozenset, make_optional_smt(SmtFrozenSet))
     register_type(type, make_optional_smt(SmtType))
     register_type(collections.abc.Callable, make_optional_smt(SmtCallable))
 
     # Most types are not directly modeled in the solver, rather they are built
     # on top of the modeled types. Such types are enumerated here:
     
-    register_type(object, lambda p: SmtObject(p.space, p.pytype, p.varname))
+    register_type(object, lambda p: SmtObject(p.varname, p.pytype))
     register_type(complex, lambda p: complex(p(float), p(float)))
     register_type(slice, lambda p: slice(p(Optional[int]), p(Optional[int]), p(Optional[int])))
     register_type(NoReturn, make_raiser(IgnoreAttempt, 'Attempted to short circuit a NoReturn function')) # type: ignore
     
     # AsyncContextManager, lambda p: p(contextlib.AbstractAsyncContextManager),
     # AsyncGenerator: ,
     # AsyncIterable,
@@ -1813,7 +2026,9 @@
 
     # TODO: override str.__new__ to make symbolic strings
 
     # Patches on list
     register_patch(orig_builtins.list, _list_index, 'index')
     # TODO: forbiddenfruit can't patch __repr__ yet:
     # register_patch(orig_builtins.list, _list_repr, '__repr__')
+
+    setup_binops()
```

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/builtinslib_test.py` & `crosshair-tool-0.0.9/crosshair/libimpl/builtinslib_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 import unittest
 from typing import *
 
 from crosshair.core import make_fake_object
 from crosshair.libimpl.builtinslib import SmtFloat
 from crosshair.libimpl.builtinslib import SmtInt
 from crosshair.libimpl.builtinslib import SmtList
-from crosshair.libimpl.builtinslib import crosshair_type_for_python_type
+from crosshair.libimpl.builtinslib import crosshair_types_for_python_type
 from crosshair.libimpl.builtinslib import _isinstance
 from crosshair.libimpl.builtinslib import _max
 from crosshair.core_and_libs import *
 from crosshair.test_util import check_ok
 from crosshair.test_util import check_exec_err
 from crosshair.test_util import check_post_err
 from crosshair.test_util import check_fail
 from crosshair.test_util import check_unknown
 from crosshair.util import set_debug
 from crosshair.statespace import SimpleStateSpace
+from crosshair.statespace import StateSpaceContext
 
 
 class Cat:
     def size(self) -> int:
         return 1
 class BiggerCat(Cat):
     def size(self) -> int:
@@ -51,26 +52,25 @@
 
 if sys.version_info >= (3, 8):
     class Movie(TypedDict):
         name: str
         year: int
 
 class UnitTests(unittest.TestCase):
-    def test_crosshair_type_for_python_type(self) -> None:
-        self.assertIs(crosshair_type_for_python_type(int), SmtInt)
-        self.assertIs(crosshair_type_for_python_type(List[int]), SmtList)
-        self.assertIs(crosshair_type_for_python_type(List[SmokeDetector]), SmtList)
-        self.assertIs(crosshair_type_for_python_type(SmokeDetector), None)
+    def test_crosshair_types_for_python_type(self) -> None:
+        self.assertEqual(crosshair_types_for_python_type(int), (SmtInt,))
+        self.assertEqual(crosshair_types_for_python_type(SmokeDetector), ())
 
     def test_isinstance(self):
-        f = SmtFloat(SimpleStateSpace(), float, 'f')
-        self.assertFalse(isinstance(f, float))
-        self.assertFalse(isinstance(f, int))
-        self.assertTrue(_isinstance(f, float))
-        self.assertFalse(_isinstance(f, int))
+        with StateSpaceContext(SimpleStateSpace()):
+            f = SmtFloat('f')
+            self.assertFalse(isinstance(f, float))
+            self.assertFalse(isinstance(f, int))
+            self.assertTrue(_isinstance(f, float))
+            self.assertFalse(_isinstance(f, int))
 
 
 class BooleanTest(unittest.TestCase):
 
     def test_simple_bool_with_fail(self) -> None:
         def f(a: bool, b: bool) -> bool:
             ''' post: _ == a '''
@@ -94,14 +94,20 @@
             '''
             pre: (not a) and (not d)
             post: _ == (a ^ b) or (c ^ d)
             '''
             return a or b or c or d
         self.assertEqual(*check_ok(f))
 
+    def test_bool_as_numbers(self) -> None:
+        def f(a: bool, b: bool) -> int:
+            ''' post: _ in (1, 2) '''
+            return (a * b) + True
+        self.assertEqual(*check_ok(f))
+
 
 class NumbersTest(unittest.TestCase):
 
     def test_simple_compare_ok(self) -> None:
         def f(i: List[int]) -> bool:
             '''
             pre: 10 < len(i)
@@ -144,14 +150,22 @@
             '''
             pre: i != 0
             post: _ > 0
             '''
             return (1 + i) + (1 - i) + (1 / i)
         self.assertEqual(*check_ok(f))
 
+    def test_int_minus_symbolic_fail(self) -> None:
+        def f(i: int) -> float:
+            '''
+            post: _ != 42
+            '''
+            return 1 - i
+        self.assertEqual(*check_fail(f))
+
     def test_int_div_fail(self) -> None:
         def f(a: int, b: int) -> int:
             ''' post: a <= _ <= b '''
             return (a + b) // 2
         self.assertEqual(*check_fail(f))
 
     def test_int_div_ok(self) -> None:
@@ -227,23 +241,41 @@
 
     def test_round_unknown(self) -> None:
         def f(num: float, ndigits: Optional[int]) -> float:
             '''
             post: isinstance(_, int) == (ndigits is None)
             '''
             return round(num, ndigits)
-        # TODO: this is unknown (z3 can't solve 10**x != 0 right now)
+        # TODO: this is unknown (rounding reals is hard)
         self.assertEqual(*check_unknown(f))
 
     def test_number_isinstance(self) -> None:
         def f(x: float) -> float:
             ''' post: isinstance(_, float) '''
             return x
         self.assertEqual(*check_ok(f))
 
+    def test_mismatched_types(self) -> None:
+        def f(x: float, y: list) -> float:
+            '''
+            pre: x == 1.0 and y == []
+            post: _ == 1
+            '''
+            return x + y
+        self.assertEqual(*check_exec_err(f, 'TypeError: unsupported operand type'))
+
+    def test_surprisingly_valid_types(self) -> None:
+        def f(x: bool) -> float:
+            '''
+            pre: x == True
+            post: _ == -2
+            '''
+            return ~x
+        self.assertEqual(*check_ok(f))
+
     def TODO_test_int_repr(self) -> None:
         def f(x: int) -> str:
             ''' post: len(_) != 3 '''
             return repr(x)
         self.assertEqual(*check_fail(f))
 
     def TODO_test_nonlinear(self) -> None:
@@ -302,21 +334,54 @@
 
     def test_prefixing_ok(self) -> None:
         def f(a: str, indent: bool) -> str:
             ''' post: len(_) == len(a) + (2 if indent else 0) '''
             return ('  ' if indent else '') + a
         self.assertEqual(*check_ok(f))
 
+    def test_find_with_limits_ok(self) -> None:
+        def f(a: str) -> int:
+            ''' post: _ == -1 '''
+            return a.find('abc', 1, 3)
+        self.assertEqual(*check_ok(f))
+
+    def test_index_err(self) -> None:
+        def f(s1: str, s2: str) -> int:
+            '''
+            pre: s1 == 'aba'
+            pre: 'ab' in s2
+            post: True
+            '''
+            return s1.index(s2)
+        # index() raises ValueError when a match isn't found:
+        self.assertEqual(*check_exec_err(f, 'ValueError'))
+
     def test_negative_index_slicing(self) -> None:
         def f(s: str) -> Tuple[str, str]:
             ''' post: sum(map(len, _)) == len(s) - 1 '''
             idx = s.find(':')
             return (s[:idx], s[idx + 1:])
         self.assertEqual(*check_fail(f))  # (fails when idx == -1)
 
+    def test_starts_and_ends_ok(self) -> None:
+        def f(s: str) -> str:
+            '''
+            pre: s == 'aba'
+            post: s.startswith('ab')
+            post: s.endswith('ba')
+            '''
+            return s
+        self.assertEqual(*check_ok(f))
+
+    def test_split_ok(self) -> None:
+        def f(s: str) -> list:
+            ''' post: len(_) in (1, 2) '''
+            return s.split(':', 1)
+        self.assertEqual(*check_ok(f))
+
     def test_str_comparison_fail(self) -> None:
         def f(s1: str, s2: str) -> bool:
             ''' post: _ '''
             return s1 >= s2
         self.assertEqual(*check_fail(f))
 
     def test_compare_ok(self) -> None:
@@ -567,15 +632,21 @@
     def test_index_error(self) -> None:
         def f(l: List[int], idx: int) -> int:
             '''
             pre: idx >= 0 and len(l) > 2
             post: True
             '''
             return l[idx]
-        self.assertEqual(*check_exec_err(f))
+        self.assertEqual(*check_exec_err(f, 'IndexError'))
+
+    def test_index_type_error(self) -> None:
+        def f(l: List[int]) -> int:
+            ''' post: True '''
+            return l[0.0:]
+        self.assertEqual(*check_exec_err(f, 'TypeError'))
 
     def test_index_ok(self) -> None:
         def f(l: List[int]) -> bool:
             '''
             pre: len(l) <= 3
             post: _ == (7 in l)
             '''
@@ -650,25 +721,43 @@
                 l[1] == 42
                 l[2] == 43
                 len(l) == 4
             '''
             l[1:-1] = [42, 43]
         self.assertEqual(*check_ok(f))
 
+    def test_slice_assignment_out_of_bounds(self) -> None:
+        def f(l: List[int], i: int) -> None:
+            '''
+            pre: i != -1
+            post: l == __old__.l[:i] + __old__.l[i+1:]
+            '''
+            l[i:i+1] = []
+        self.assertEqual(*check_unknown(f))
+
     def test_insert_ok(self) -> None:
         def f(l: List[int]) -> None:
             '''
             pre: len(l) == 4
             post[l]:
                 len(l) == 5
                 l[2] == 42
             '''
             l.insert(-2, 42)
         self.assertEqual(*check_ok(f))
 
+    def test_insert_with_conversions(self) -> None:
+        def f(l: List[Set[int]], a: bool, b: int) -> None:
+            '''
+            # self.insert(a,b) with {'a': True, 'b': 10, 'self': [{0}]}
+            post: True
+            '''
+            l.insert(a, b)
+        self.assertEqual(*check_ok(f))
+
     def test_pop_ok(self) -> None:
         def f(l: List[int]) -> None:
             '''
             pre: l == [4, 5]
             post: l == [4]
             '''
             l.pop()
@@ -706,14 +795,29 @@
             '''
             pre: len(l) == 5
             post[l]: len(l) == 4
             '''
             del l[2]
         self.assertEqual(*check_ok(f))
 
+    def test_item_delete_type_error(self) -> None:
+        def f(l: List[float]) -> None:
+            '''
+            pre: len(l) == 0
+            post: True
+            '''
+            del l[1.0]
+        self.assertEqual(*check_exec_err(f, 'TypeError'))
+
+    def test_item_delete_oob(self) -> None:
+        def f(l: List[float]) -> None:
+            ''' post: True '''
+            del l[1]
+        self.assertEqual(*check_exec_err(f, 'IndexError'))
+
     def test_sort_ok(self) -> None:
         def f(l: List[int]) -> None:
             '''
             pre: len(l) == 3
             post[l]: l[0] == min(l)
             '''
             l.sort()
@@ -749,14 +853,20 @@
         def f(a: Dict[int, str], k: int, v: str) -> None:
             '''
             post[a]: a[k] == v
             '''
             a[k] = v
         self.assertEqual(*check_ok(f))
 
+    def test_dict_get_with_defaults_ok(self) -> None:
+        def f(a: Dict[float, float]) -> float:
+            ''' post: (_ == 1.2) or (_ == a[42.42]) '''
+            return a.get(42.42, 1.2)
+        self.assertEqual(*check_ok(f))
+
     def test_dict_empty_bool(self) -> None:
         def f(a: Dict[int, str]) -> bool:
             '''
             post[a]: _ == True
             '''
             a[0] = 'zero'
             return bool(a)
@@ -791,15 +901,15 @@
             a[10] = 'ten'
             return list(a.__iter__())
         self.assertEqual(*check_fail(f))
 
     def test_dict_iter_ok(self) -> None:
         def f(a: Dict[int, str]) -> List[int]:
             '''
-            pre: len(a) < 4
+            pre: len(a) < 3
             post[a]: 10 in _
             '''
             a[10] = 'ten'
             return list(a.__iter__())
         self.assertEqual(*check_ok(f))
 
     def test_dict_to_string_ok(self) -> None:
@@ -825,14 +935,23 @@
         def f(a: Dict[str, int]) -> None:
             '''
             post[a]: True
             '''
             del a["42"]
         self.assertEqual(*check_exec_err(f))
 
+    def test_setdefault_float_int_comparison(self) -> None:
+        def f(a: Dict[int, int]):
+            '''
+            pre: a == {2: 0}
+            post: _ == 0
+            '''
+            return a.setdefault(2.0, {True: '0'})
+        self.assertEqual(*check_ok(f))
+
     def test_dicts_complex_contents(self) -> None:
         def f(d: Dict[Tuple[int, str], Tuple[float, int]]) -> int:
             '''
             post: _ > 0
             '''
             if (42, 'fourty-two') in d:
                 return d[(42, 'fourty-two')][1]
@@ -877,24 +996,28 @@
             '''
             pre: (1, 'one') in d
             post[d]: (1, 'one') not in d
             '''
             del d[(1, 'one')]
         self.assertEqual(*check_unknown(f))
 
-    def test_equality(self) -> None:
+    def test_equality_fail(self) -> None:
         def f(d: Dict[int, int]) -> Dict[int, int]:
             ''' post: _ != d '''
             d = d.copy()
             d[40] = 42
-            # extra check for positive equality:
-            assert d == {**d}
             return d
         self.assertEqual(*check_fail(f))
 
+    def test_equality_ok(self) -> None:
+        def f(d: Dict[int, int]) -> Dict[int, int]:
+            ''' post: _ == {**_} '''
+            return d
+        self.assertEqual(*check_unknown(f))
+
     def test_wrong_key_type(self) -> None:
         def f(d: Dict[int, int], s: str, i: int) -> bool:
             if i == 0:
                 del d[s]  # type: ignore
             elif i < 0:
                 d[s] = 7  # type: ignore
             else:
@@ -978,14 +1101,23 @@
             '''
             pre: 1 in m1 and 2 in m2
             post: _ != 10
             '''
             return m1[1] + m2[2]
         self.assertEqual(*check_fail(f))
 
+    def test_implicit_conversion_for_keys(self) -> None:
+        def f(m: Dict[float, float], b: bool, i: int):
+            '''
+            post: len(m) >= len(__old__.m)
+            '''
+            m[b] = 2.0
+            m[i] = 3.0
+        self.assertEqual(*check_ok(f))
+
     if sys.version_info >= (3, 8):
         def test_typed_dict_fail(self) -> None:
             def f(td: Movie):
                 ''' post: _['year'] != 2020 or _['name'] != "hi"'''
                 return td
             self.assertEqual(*check_fail(f))
 
@@ -1021,19 +1153,30 @@
         def f(a: Set[str], b: Set[str]) -> Set[str]:
             '''
             post: all(((i in a) or (i in b)) for i in _)
             '''
             return a | b
         self.assertEqual(*check_unknown(f))
 
-    def test_subtype_union(self) -> None:
+    def test_contains_different_but_equivalent(self) -> None:
         def f(s: Set[Union[int, str]]) -> None:
-            ''' post: not (42 in s and '42' in s) '''
+            '''
+            pre: "foobar" in s
+            post: (_ + "bar") in s
+            '''
+            return "foo"
+        self.assertEqual(*check_unknown(f))
+
+    # The heaprefs + deferred set assumptions make this too expensive.
+    # TODO: Optimize & re-enable
+    def TODO_test_subtype_union(self) -> None:
+        def f(s: Set[Union[int, str]]) -> None:
+            ''' post: not ((42 in s) and ('42' in s)) '''
             return s
-        self.assertEqual(*check_fail(f))
+        self.assertEqual(*check_fail(f, AnalysisOptions(per_condition_timeout=7.0)))
 
     def test_subset_compare_ok(self) -> None:
         # a >= b with {'a': {0.0, 1.0}, 'b': {2.0}}
         def f(s1: Set[float], s2: Set[float]) -> bool:
             '''
             pre: s1 == {0.0, 1.0}
             pre: s2 == {2.0}
@@ -1167,15 +1310,22 @@
             return issubclass(typ, str)
         self.assertEqual(*check_fail(f))
 
     def test_symbolic_types_without_literal_types(self) -> None:
         def f(typ1: Type, typ2: Type, typ3: Type):
             ''' post: implies(_, issubclass(typ1, typ3)) '''
             return issubclass(typ2, typ3) and typ2 != typ3
-        self.assertEqual(*check_fail(f))
+        self.assertEqual(*check_fail(f, AnalysisOptions(max_iterations=60,
+                                                        per_condition_timeout=10)))
+
+    def test_instance_creation(self) -> None:
+        def f(t: Type[Cat]):
+            ''' post: _.size() > 0 '''
+            return t()
+        self.assertEqual(*check_ok(f))
 
     def test_type_comparison(self) -> None:
         def f(t: Type) -> bool:
             ''' post: _ '''
             return t == int
         self.assertEqual(*check_fail(f))
 
@@ -1256,15 +1406,15 @@
             '''
             print(x)
             return True
         self.assertEqual(*check_ok(f))
 
     def test_dispatch(self):
         self.assertEqual(list(_max.registry.keys()), [
-                         object, collections.Iterable])
+                         object, collections.abc.Iterable])
 
     def test_repr_ok(self):
         def f(x: int) -> str:
             ''' post: len(_) == 0 or len(_) > 0 '''
             return repr(x)
         self.assertEqual(*check_ok(f))
```

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/collectionslib.py` & `crosshair-tool-0.0.9/crosshair/libimpl/collectionslib.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/collectionslib_test.py` & `crosshair-tool-0.0.9/crosshair/libimpl/collectionslib_test.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/datetimelib.py` & `crosshair-tool-0.0.9/crosshair/libimpl/datetimelib.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/datetimelib_test.py` & `crosshair-tool-0.0.9/crosshair/libimpl/datetimelib_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def test_datetime_fail(self) -> None:
         def f(dtime: datetime.datetime) -> int:
             '''
             post: _ != 22
             '''
             return dtime.second
-        self.assertEqual(*check_fail(f))
+        self.assertEqual(*check_fail(f, AnalysisOptions(max_iterations=60)))
 
     def test_timedelta_fail(self) -> None:
         def f(d: datetime.timedelta) -> int:
             '''
             post: _ != 9
             '''
             return d.seconds
```

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/mathlib_test.py` & `crosshair-tool-0.0.9/crosshair/libimpl/mathlib_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 from crosshair.test_util import check_fail
 from crosshair.test_util import check_unknown
 from crosshair.test_util import check_messages
 from crosshair.util import set_debug
 
 from crosshair.libimpl.builtinslib import SmtFloat
 from crosshair.statespace import SimpleStateSpace
+from crosshair.statespace import StateSpaceContext
 
 
 class MathLibTests(unittest.TestCase):
 
     def test_isfinite(self):
         space = SimpleStateSpace()
-        x = SmtFloat(space, float, 'symfloat')
-        with Patched(enabled=lambda: True):
+        with Patched(enabled=lambda: True), StateSpaceContext(space):
+            x = SmtFloat('symfloat')
             self.assertTrue(math.isfinite(x))
             self.assertTrue(math.isfinite(2.3))
             self.assertFalse(math.isfinite(float('nan')))
 
 
 if __name__ == '__main__':
     if ('-v' in sys.argv) or ('--verbose' in sys.argv):
```

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/randomlib.py` & `crosshair-tool-0.0.9/crosshair/libimpl/randomlib.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/relib.py` & `crosshair-tool-0.0.9/crosshair/libimpl/relib.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,27 +82,31 @@
             # extend this logic
             return z3.Range('0','9')
         raise ReUnhandled
     elif op is ANY and arg is None:
         # TODO: when z3 gets unicode string support, we'll need to
         # revise this logic
         if re.DOTALL & flags:
-            return z3.Range(chr(0), chr(255))
+            return z3.Range(z3.Unit(z3.BitVecVal(0, 8)), z3.Unit(z3.BitVecVal(255, 8)))
+            #return z3.Range(chr(0), chr(127))
         else:
-            return z3.Union(z3.Range(chr(0), chr(9)),
-                            z3.Range(chr(11), chr(255)))
+            return z3.Union(
+                z3.Range(z3.Unit(z3.BitVecVal(0, 8)), z3.Unit(z3.BitVecVal(9, 8))),
+                z3.Range(z3.Unit(z3.BitVecVal(11, 8)), z3.Unit(z3.BitVecVal(255, 8))))
     else:
         return None
 
 class _Match:
     def __init__(self,
                  groups: List[Tuple[Optional[str], int, Union[int, SmtInt]]]): # (name, start, end)
         self._groups = groups
         self.lastindex = None
         self.lastgroup = None
+    def __ch_realize__(self):
+        self._groups = [(name, realize(start), realize(end)) for name, start, enf in self._groups]
     def __bool__(self):
         return True
     def __repr__(self):
         return f'<re.Match object; span={self.span()!r}, match={self.group()!r}>'
     def __getitem__(self, idx):
         return self.group(idx)
     def _add_match(self, suffix_match):
```

### Comparing `crosshair-tool-0.0.8/crosshair/libimpl/relib_test.py` & `crosshair-tool-0.0.9/crosshair/libimpl/relib_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,31 +7,41 @@
 
 import z3  # type: ignore
 
 from crosshair.libimpl.builtinslib import SmtStr
 from crosshair.libimpl.relib import _match_pattern
 
 from crosshair.core_and_libs import *
+from crosshair.core import realize
+from crosshair.statespace import context_statespace
 from crosshair.statespace import SimpleStateSpace
+from crosshair.statespace import StateSpaceContext
 from crosshair.test_util import check_ok
 from crosshair.test_util import check_exec_err
 from crosshair.test_util import check_post_err
 from crosshair.test_util import check_fail
 from crosshair.test_util import check_unknown
 from crosshair.test_util import check_messages
 from crosshair.util import set_debug
 
 def eval_regex(re_string, flags, test_string, offset):
     py_patt = re.compile(re_string, flags)
-    space = SimpleStateSpace()
-    s = SmtStr(space, str, 'symstr')
+    space = context_statespace()
+    s = SmtStr('symstr' + space.uniq())
     space.add(s.var == z3.StringVal(test_string))
     return _match_pattern(py_patt, re_string, s, offset)
 
-class RegularExpressionTests(unittest.TestCase):
+class RegularExpressionUnitTests(unittest.TestCase):
+
+    def setUp(self):
+        self.space_ctx_ = StateSpaceContext(SimpleStateSpace())
+        self.space_ctx_.__enter__()
+
+    def tearDown(self):
+        self.space_ctx_.__exit__(None, None, None)
 
     def test_handle_simple(self):
         self.assertIsNotNone(eval_regex('abc', 0, 'abc', 0))
         self.assertIsNone(eval_regex('abc', 0, 'ab', 0))
 
     def test_handle_or(self):
         self.assertIsNotNone(eval_regex('a|bc', 0, 'bc', 0))
@@ -91,14 +101,43 @@
 
     def test_handle_nested_subgroups(self):
         self.assertIsNotNone(eval_regex('(a|b(xx))+(c)?', 0, 'bxxc', 0))
         self.assertEqual(eval_regex('(bxx)(c)?', 0, 'bxxc', 0).groups(), ('bxx', 'c'))
         self.assertEqual(eval_regex('(a|b(xx))+(c)?', 0, 'bxxc', 0).groups(), ('bxx', 'xx', 'c'))
         self.assertEqual(eval_regex('(a|b(xx))+(c)?', 0, 'a', 0).groups(), ('a', None, None))
 
+    def test_with_fuzzed_inputs(self) -> None:
+        rand = random.Random(253209)
+        def check(pattern, literal_string, offset):
+            flags = re.ASCII | re.DOTALL
+            sym_match = eval_regex(pattern, flags, literal_string, offset)
+            py_match = re.compile(pattern, flags).match(literal_string, offset)
+            if (sym_match is None) != (py_match is None):
+                self.assertEqual(py_match, sym_match)
+            if py_match is None:
+                return
+            self.assertEqual(py_match.span(), sym_match.span())
+            self.assertEqual(py_match.group(0), sym_match.group(0))
+            self.assertEqual(py_match.groups(), sym_match.groups())
+            self.assertEqual(py_match.pos, sym_match.pos)
+            self.assertEqual(py_match.endpos, sym_match.endpos)
+            self.assertEqual(py_match.lastgroup, sym_match.lastgroup)
+
+        for iter in range(100):
+            literal_string = ''.join(rand.choice(['a','5','_']) for _ in
+                                     range(rand.choice([0, 1, 1, 2, 2, 3, 4])))
+            pattern = ''.join(rand.choice(['a','5','.']) + rand.choice(['', '', '+', '*']) for _ in
+                              range(rand.choice([0, 1, 1, 2, 2])))
+            offset = rand.choice([0, 0, 0, 0, 1])
+            with self.subTest(msg=f'Trial {iter}: evaluating pattern "{pattern}" against "{literal_string}" at {offset}'):
+                check(pattern, literal_string, offset)
+
+
+class RegularExpressionTests(unittest.TestCase):
+
     def test_fullmatch_basic_fail(self) -> None:
         def f(s: str) -> Optional[re.Match]:
             ''' post: _ '''
             return re.compile('a').fullmatch(s)
         self.assertEqual(*check_fail(f))
 
     def test_star_fail(self) -> None:
@@ -160,15 +199,15 @@
             '''
             pre: len(s) == 1
             post: _
             '''
             return not re.compile('[a-z]').match(s)
         self.assertEqual(*check_fail(f))
 
-    def test_match_basic_fail(self) -> None:
+    def test_match_basic_fail2(self) -> None:
         def f(s: str) -> bool:
             ''' post: implies(_, len(s) <= 3) '''
             return re.compile('ab?c').match(s)
         self.assertEqual(*check_fail(f))
         
     def test_match_properties(self) -> None:
         test_string = '01ab9'
@@ -203,40 +242,14 @@
         number_re = re.compile(r'(-?(?:0|[1-9]\d*))(\.\d+)?([eE][-+]?\d+)?')
         def f(s:str):
             '''
             pre: len(s) == 4
             post: not _
             '''
             return bool(number_re.fullmatch(s))
-        self.assertEqual(*check_fail(f))
-
-    def test_with_fuzzed_inputs(self) -> None:
-        rand = random.Random(253209)
-        def check(pattern, literal_string, offset):
-            flags = re.ASCII | re.DOTALL
-            sym_match = eval_regex(pattern, flags, literal_string, offset)
-            py_match = re.compile(pattern, flags).match(literal_string, offset)
-            if (sym_match is None) != (py_match is None):
-                self.assertEqual(py_match, sym_match)
-            if py_match is None:
-                return
-            self.assertEqual(py_match.span(), sym_match.span())
-            self.assertEqual(py_match.group(0), sym_match.group(0))
-            self.assertEqual(py_match.groups(), sym_match.groups())
-            self.assertEqual(py_match.pos, sym_match.pos)
-            self.assertEqual(py_match.endpos, sym_match.endpos)
-            self.assertEqual(py_match.lastgroup, sym_match.lastgroup)
-
-        for iter in range(100):
-            literal_string = ''.join(rand.choice(['a','5','_']) for _ in
-                                     range(rand.choice([0, 1, 1, 2, 2, 3, 4])))
-            pattern = ''.join(rand.choice(['a','5','.']) + rand.choice(['', '', '+', '*']) for _ in
-                              range(rand.choice([0, 1, 1, 2, 2])))
-            offset = rand.choice([0, 0, 0, 0, 1])
-            with self.subTest(msg=f'Trial {iter}: evaluating pattern "{pattern}" against "{literal_string}" at {offset}'):
-                check(pattern, literal_string, offset)
+        self.assertEqual(*check_fail(f, AnalysisOptions(max_iterations=20, per_condition_timeout=10)))
 
 
 if __name__ == '__main__':
     if ('-v' in sys.argv) or ('--verbose' in sys.argv):
         set_debug(True)
     unittest.main()
```

### Comparing `crosshair-tool-0.0.8/crosshair/localhost_comms.py` & `crosshair-tool-0.0.9/crosshair/localhost_comms.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/main.py` & `crosshair-tool-0.0.9/crosshair/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,22 +14,35 @@
 import os.path
 import queue
 import shutil
 import signal
 import sys
 import time
 import traceback
+import types
 from typing import *
 from typing import TextIO
 
-from crosshair.localhost_comms import StateUpdater, read_states
-from crosshair.core_and_libs import AnalysisMessage, AnalysisOptions, MessageType, analyzable_members, analyze_module, analyze_any
+from crosshair.diff_behavior import diff_behavior
+from crosshair.core_and_libs import analyze_any
+from crosshair.core_and_libs import analyze_module
+from crosshair.core_and_libs import analyzable_members
+from crosshair.core_and_libs import AnalysisKind
+from crosshair.core_and_libs import AnalysisMessage
+from crosshair.core_and_libs import AnalysisOptions
+from crosshair.core_and_libs import MessageType
 from crosshair.util import debug, extract_module_from_file, set_debug, CrosshairInternal, load_file, load_by_qualname, NotFound, ErrorDuringImport
 import crosshair.core_and_libs
 
+def parse_analysis_kind(s: str) -> AnalysisKind:
+    try:
+        return AnalysisKind[s]
+    except KeyError:
+        raise ValueError
+
 def command_line_parser() -> argparse.ArgumentParser:
     common = argparse.ArgumentParser(add_help=False)
     common.add_argument('--verbose', '-v', action='store_true')
     common.add_argument('--per_path_timeout', type=float,
                         help='Maximum seconds to spend checking one execution path')
     common.add_argument('--per_condition_timeout', type=float,
                         help='Maximum seconds to spend checking the execution paths of one postcondition')
@@ -41,29 +54,41 @@
                               help='Output analysis results for all postconditions (not just failing ones)')
     check_parser.add_argument('file', metavar='F', type=str, nargs='+',
                               help='file or fully qualified module, class, or function')
     watch_parser = subparsers.add_parser(
         'watch', help='Continuously watch and analyze a directory', parents=[common])
     watch_parser.add_argument('directory', metavar='F', type=str, nargs='+',
                               help='file or directory to analyze')
-    showresults_parser = subparsers.add_parser(
-        'showresults', help='Display results from a currently running `watch` command', parents=[common])
-    showresults_parser.add_argument('file', metavar='F', type=str, nargs='+',
-                                    help='file or directory to analyze')
+    for subparser in (check_parser, watch_parser):
+        subparser.add_argument('--analysis_kind',
+                               type=parse_analysis_kind,
+                               nargs='*',
+                               default=(AnalysisKind.PEP316,),
+                               choices=list(k for k in AnalysisKind),
+                               help='Kinds of analysis to perform.')
+    diffbehavior_parser = subparsers.add_parser(
+        'diffbehavior', help='Find differences in behavior between two functions', parents=[common])
+    diffbehavior_parser.add_argument('fn1', type=str,
+                                     help='first module+function to compare (e.g. "mymodule.myfunc")')
+    diffbehavior_parser.add_argument('fn2', type=str,
+                                     help='second function to compare')
     return parser
 
 def mtime(path: str) -> Optional[float]:
     try:
         return os.stat(path).st_mtime
     except FileNotFoundError:
         return None
 
 def process_level_options(command_line_args: argparse.Namespace) -> AnalysisOptions:
     options = AnalysisOptions()
-    for optname in ('per_path_timeout', 'per_condition_timeout', 'report_all'):
+    if command_line_args.action == 'diffbehavior':
+        options.per_condition_timeout = 2.5
+        options.per_path_timeout = 30.0  # mostly, we don't want to time out paths
+    for optname in ('per_path_timeout', 'per_condition_timeout', 'report_all', 'analysis_kind'):
         arg_val = getattr(command_line_args, optname, False)
         if arg_val is not None:
             setattr(options, optname, arg_val)
     return options
 
 
 @dataclasses.dataclass(init=False)
@@ -93,36 +118,40 @@
 WorkItemOutput = Tuple[WatchedMember, Counter[str], List[AnalysisMessage]]
 
 def import_error_msg(err: ErrorDuringImport) -> AnalysisMessage:
     orig, frame = err.args
     return AnalysisMessage(MessageType.IMPORT_ERR, str(orig),
                            frame.filename, frame.lineno, 0, '')
 
+def pool_worker_process_item(item: WorkItemInput) -> Optional[Tuple[Counter[str], List[AnalysisMessage]]]:
+    filename, options, deadline = item
+    stats: Counter[str] = Counter()
+    options.stats = stats
+    try:
+        module = load_file(filename)
+    except NotFound as e:
+        debug(f'Not analyzing "{filename}" because sub-module import failed: {e}')
+        return None
+    except ErrorDuringImport as e:
+        debug(f'Not analyzing "{filename}" because import failed: {e}')
+        return (stats, [import_error_msg(e)])
+    messages = analyze_any(module, options)
+    return (stats, messages)
+
 def pool_worker_main(item: WorkItemInput, output: multiprocessing.queues.Queue) -> None:
     try:
         # TODO figure out a more reliable way to suppress this. Redirect output?
         # Ignore ctrl-c in workers to reduce noisy tracebacks (the parent will kill us):
         signal.signal(signal.SIGINT, signal.SIG_IGN)
 
-        if hasattr(os, 'nice'): # analysis should run at a low priority
+        if hasattr(os, 'nice'):  # analysis should run at a low priority
             os.nice(10)
         set_debug(False)
-        filename, options, deadline = item
-        stats: Counter[str] = Counter()
-        options.stats = stats
-        _, module_name = extract_module_from_file(filename)
-        try:
-            module = load_by_qualname(module_name)
-        except NotFound:
-            return
-        except ErrorDuringImport as e:
-            output.put((filename, stats, [import_error_msg(e)]))
-            debug(f'Not analyzing "{filename}" because import failed: {e}')
-            return
-        messages = analyze_any(module, options)
+        (stats, messages) = pool_worker_process_item(item)
+        filename = item[0]
         output.put((filename, stats, messages))
     except BaseException as e:
         raise CrosshairInternal(
             'Worker failed while analyzing ' + filename) from e
 
 
 class Pool:
@@ -185,14 +214,24 @@
 
 
 def worker_initializer():
     """Ignore CTRL+C in the worker process."""
     signal.signal(signal.SIGINT, signal.SIG_IGN)
 
 def analyzable_filename(filename: str) -> bool:
+    '''
+    >>> analyzable_filename('foo23.py')
+    True
+    >>> analyzable_filename('#foo.py')
+    False
+    >>> analyzable_filename('23foo.py')
+    False
+    >>> analyzable_filename('setup.py')
+    False
+    '''
     if not filename.endswith('.py'):
         return False
     lead_char = filename[0]
     if (not lead_char.isalpha()) and (not lead_char.isidentifier()):
         # (skip temporary editor files, backups, etc)
         debug(
             f'Skipping {filename} because it begins with a special character.')
@@ -220,17 +259,16 @@
     _paths: Set[str]
     _pool: Pool
     _modtimes: Dict[str, float]
     _options: AnalysisOptions
     _next_file_check: float = 0.0
     _change_flag: bool = False
 
-    def __init__(self, options: AnalysisOptions, files: Iterable[str], state_updater: StateUpdater):
+    def __init__(self, options: AnalysisOptions, files: Iterable[str]):
         self._paths = set(files)
-        self._state_updater = state_updater
         self._pool = self.startpool()
         self._modtimes = {}
         self._options = options
         _ = list(walk_paths(self._paths)) # just to force an exit if we can't find a path
 
     def startpool(self) -> Pool:
         return Pool(multiprocessing.cpu_count() - 1)
@@ -284,18 +322,14 @@
             else:
                 time.sleep(0.5)
                 max_condition_timeout *= 2
             for curstats, messages in self.run_iteration(max_condition_timeout):
                 debug('stats', curstats, messages)
                 stats.update(curstats)
                 if messages_merged(active_messages, messages):
-                    self._state_updater.update(json.dumps({
-                        'version': 1,
-                        'time': time.time(),
-                        'messages': [m.toJSON() for m in active_messages.values()]}))
                     linecache.checkcache()
                     clear_screen()
                     for message in active_messages.values():
                         lines = long_describe_message(message)
                         if lines is None:
                             continue
                         clear_line('-')
@@ -366,18 +400,17 @@
 def watch(args: argparse.Namespace, options: AnalysisOptions) -> int:
     # Avoid fork() because we've already imported the code we're watching:
     multiprocessing.set_start_method('spawn')
     if not args.directory:
         print('No files or directories given to watch', file=sys.stderr)
         return 1
     try:
-        with StateUpdater() as state_updater:
-            watcher = Watcher(options, args.directory, state_updater)
-            watcher.check_changed()
-            watcher.run_watch_loop()
+        watcher = Watcher(options, args.directory)
+        watcher.check_changed()
+        watcher.run_watch_loop()
     except KeyboardInterrupt:
         watcher._pool.terminate()
         print()
         print('I enjoyed working with you today!')
         return 0
 
 
@@ -426,32 +459,59 @@
             return '{}:{}:{}:{}'.format(message.filename, message.line, 'info', desc)
         return None
     if message.state == MessageType.POST_ERR:
         desc = 'Error while evaluating post condition: ' + desc
     return '{}:{}:{}:{}'.format(message.filename, message.line, 'error', desc)
 
 
-def showresults(args: argparse.Namespace, options: AnalysisOptions) -> int:
-    messages_by_file: Dict[str, List[AnalysisMessage]] = collections.defaultdict(list)
-    states = list(read_states())
-    for fname, content in states:
-        debug('Found watch state file at ', fname)
-        state = json.loads(content)
-        for message in state['messages']:
-            messages_by_file[message['filename']].append(AnalysisMessage.fromJSON(message))
-    debug('Found results for these files: [', ', '.join(messages_by_file.keys()), ']')
-    for name in walk_paths(args.file):
-        name = os.path.abspath(name)
-        debug('Checking file ', name)
-        for message in messages_by_file[name]:
-            desc = short_describe_message(message, options)
-            debug('Describing ', message)
-            if desc is not None:
-                print(desc)
-    return 0
+def diffbehavior(args: argparse.Namespace,
+                 options: AnalysisOptions,
+                 stdout: TextIO=sys.stdout,
+                 stderr: TextIO=sys.stderr) -> int:
+    def checked_load(qualname: str) -> Optional[types.FunctionType]:
+        try:
+            obj = load_by_qualname(qualname)
+            if isinstance(obj, types.FunctionType):
+                return obj
+            else:
+                raise Exception('Not a function')
+        except Exception as exc:
+            print(f'Unable to load "{qualname}": {exc}', file=stderr)
+            return None
+    (fn_name1, fn_name2) = (args.fn1, args.fn2)
+    fn1 = checked_load(fn_name1)
+    fn2 = checked_load(fn_name2)
+    if fn1 is None or fn2 is None:
+        return 2
+    options.stats = collections.Counter()
+    diffs = diff_behavior(fn1, fn2, options)
+    debug('stats', options.stats)
+    if isinstance(diffs, str):
+        print(diffs, file=stderr)
+        return 2
+    elif len(diffs) == 0:
+        num_paths = options.stats['num_paths']
+        exhausted = (options.stats['exhaustion'] > 0)
+        stdout.write(f'No differences found. (attempted {num_paths} iterations)\n')
+        if exhausted:
+            stdout.write('All paths exhausted, functions are likely the same!\n')
+        else:
+            stdout.write('Consider trying longer with: --per_condition_timeout=<seconds>\n')
+        return 0
+    else:
+        width = max(len(fn_name1), len(fn_name2)) + 2
+        for diff in diffs:
+            inputs = ', '.join(f'{k}={v}' for k,v in diff.args.items())
+            stdout.write(f'Given: ({inputs}),\n')
+            result1, result2 = diff.result1, diff.result2
+            differing_args = result1.get_differing_arg_mutations(result2)
+            stdout.write(f'{fn_name1.rjust(width)} : {result1.describe(differing_args)}\n')
+            stdout.write(f'{fn_name2.rjust(width)} : {result2.describe(differing_args)}\n')
+        return 1
+
 
 def check(args: argparse.Namespace, options: AnalysisOptions, stdout: TextIO) -> int:
     any_problems = False
     for name in args.file:
         entity: object
         try:
             entity = load_file(name) if name.endswith('.py') else load_by_qualname(name)
@@ -478,16 +538,16 @@
     set_debug(args.verbose)
     options = process_level_options(args)
     if sys.path and sys.path[0] != '':
         # fall back to current directory to look up modules
         sys.path.append('')
     if args.action == 'check':
         exitcode = check(args, options, sys.stdout)
-    elif args.action == 'showresults':
-        exitcode = showresults(args, options)
+    elif args.action == 'diffbehavior':
+        exitcode = diffbehavior(args, options)
     elif args.action == 'watch':
         exitcode = watch(args, options)
     else:
         print(f'Unknown action: "{args.action}"', file=sys.stderr)
         exitcode = 1
     sys.exit(exitcode)
```

### Comparing `crosshair-tool-0.0.8/crosshair/main_test.py` & `crosshair-tool-0.0.9/crosshair/main_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,23 @@
     if options is None:
         options = AnalysisOptions()
     buf: io.StringIO = io.StringIO()
     retcode = check(Namespace(file=files), options, buf)
     lines = [l for l in buf.getvalue().split('\n') if l]
     return retcode, lines
 
+def call_diffbehavior(fn1: str, fn2: str, options=None) -> Tuple[int, List[str]]:
+    if options is None:
+        options = AnalysisOptions()
+    buf: io.StringIO = io.StringIO()
+    errbuf: io.StringIO = io.StringIO()
+    retcode = diffbehavior(Namespace(fn1=fn1, fn2=fn2), options, buf, errbuf)
+    lines = [l for l in buf.getvalue().split('\n')+errbuf.getvalue().split('\n') if l]
+    return retcode, lines
+
 SIMPLE_FOO = {
             'foo.py': """
 def foofn(x: int) -> int:
   ''' post: _ == x '''
   return x + 1
 """
 }
@@ -165,11 +174,43 @@
 
     def test_check_circular_with_guard(self):
         simplefs(self.root, CIRCULAR_WITH_GUARD)
         with add_to_pypath(self.root):
             retcode, lines = call_check([join(self.root, 'first.py')])
             self.assertEqual(retcode, 0)
 
+    def test_diff_behavior_same(self):
+        simplefs(self.root, SIMPLE_FOO)
+        with add_to_pypath(self.root):
+            retcode, lines = call_diffbehavior('foo.foofn', 'foo.foofn')
+            self.assertEqual(retcode, 0)
+            self.assertEqual(lines, [
+                'No differences found. (attempted 2 iterations)',
+                'All paths exhausted, functions are likely the same!'
+            ])
+
+    def test_diff_behavior_different(self):
+        simplefs(self.root, {'foo.py': """
+def add(x: int, y: int) -> int:
+  return x + y
+def faultyadd(x: int, y: int) -> int:
+  return 42 if (x, y) == (10, 10) else x + y
+"""})
+        with add_to_pypath(self.root):
+            retcode, lines = call_diffbehavior('foo.add', 'foo.faultyadd')
+            self.assertEqual(retcode, 1)
+            self.assertEqual(
+                lines,
+                ['Given: (x=10, y=10),',
+                 '        foo.add : returns 20',
+                 '  foo.faultyadd : returns 42'])
+
+    def test_diff_behavior_error(self):
+        retcode, lines = call_diffbehavior('foo.unknown', 'foo.unknown')
+        self.assertEqual(retcode, 2)
+        retcode, lines = call_diffbehavior('foo.unknown', 'foo.unknown')
+        self.assertRegex(lines[0], '.*ModuleNotFoundError')
+
 if __name__ == '__main__':
     if ('-v' in sys.argv) or ('--verbose' in sys.argv):
         set_debug(True)
     unittest.main()
```

### Comparing `crosshair-tool-0.0.8/crosshair/objectproxy.py` & `crosshair-tool-0.0.9/crosshair/objectproxy.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/objectproxy_test.py` & `crosshair-tool-0.0.9/crosshair/objectproxy_test.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair/statespace.py` & `crosshair-tool-0.0.9/crosshair/statespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import ast
 import copy
 import enum
 import itertools
 import functools
 import random
 import time
+import threading
 import traceback
 from dataclasses import dataclass
 from typing import *
 
 import z3  # type: ignore
 
 from crosshair import dynamic_typing
-from crosshair.util import debug, PathTimeout, UnknownSatisfiability, CrosshairInternal, IgnoreAttempt, IdentityWrapper
+from crosshair.util import debug
+from crosshair.util import in_debug
+from crosshair.util import name_of_type
+from crosshair.util import tiny_stack
+from crosshair.util import CrosshairInternal
+from crosshair.util import IgnoreAttempt
+from crosshair.util import IdentityWrapper
+from crosshair.util import PathTimeout
+from crosshair.util import UnknownSatisfiability
 from crosshair.condition_parser import ConditionExpr
 from crosshair.type_repo import SmtTypeRepository
 
 
 @functools.total_ordering
 class MessageType(enum.Enum):
     CONFIRMED = 'confirmed'
@@ -97,14 +106,33 @@
         return ast.literal_eval(repr(value))
 
 
 class NotDeterministic(Exception):
     pass
 
 
+_THREAD_LOCALS = threading.local()
+class StateSpaceContext:
+    def __init__(self, space: 'StateSpace'):
+        self.space = space
+    def __enter__(self):
+        assert getattr(_THREAD_LOCALS, 'space', None) is None, 'Already in a state space context'
+        _THREAD_LOCALS.space = self.space
+    def __exit__(self, exc_type, exc_value, tb):
+        assert getattr(_THREAD_LOCALS, 'space', None) is self.space, 'State space was altered in context'
+        _THREAD_LOCALS.space = None
+
+def optional_context_statespace() -> Optional['StateSpace']:
+    return getattr(_THREAD_LOCALS, 'space', None)
+
+def context_statespace() -> 'StateSpace':
+    space = _THREAD_LOCALS.space
+    assert space is not None, 'Not in a state space context'
+    return space
+
 class WithFrameworkCode:
     def __init__(self, space: 'StateSpace'):
         self.space = space
         self.previous = None
 
     def __enter__(self):
         assert self.previous is None  # (this context is not re-entrant)
@@ -157,15 +185,15 @@
     def find_model_value(self, expr: z3.ExprRef) -> object:
         value = self.solver.model().evaluate(expr, model_completion=True)
         return model_value_to_python(value)
 
     def find_model_value_for_function(self, expr: z3.ExprRef) -> object:
         return self.solver.model()[expr]
 
-    def defer_assumption(self, assumption):
+    def defer_assumption(self, description: str, checker: Callable[[], bool]) -> None:
         raise NotImplementedError
 
     def check_deferred_assumptions(self):
         pass
 
     def add_value_to_heaps(self, ref: z3.ExprRef, typ: Type, value: object) -> None:
         for heap in self.heaps[:-1]:
@@ -178,19 +206,19 @@
         with self.framework():
             for (curref, curtyp, curval) in itertools.chain(*self.heaps[snapshot:]):
                 could_match = dynamic_typing.unify(curtyp, typ)
                 if not could_match:
                     continue
                 if self.smt_fork(curref == ref):
                     debug('HEAP key lookup ', ref, ': Found existing. ',
-                          'type:', type(curval), 'id:', id(curval)%1000)
+                          'type:', name_of_type(type(curval)), 'id:', id(curval)%1000)
                     return curval
             ret = proxy_generator(typ)
             debug('HEAP key lookup ', ref, ': Created new. ',
-                  'type:', type(ret), 'id:', id(ret)%1000)
+                  'type:', name_of_type(type(ret)), 'id:', id(ret) % 1000)
 
             #assert dynamic_typing.unify(python_type(ret), typ), 'proxy type was {} and type required was {}'.format(type(ret), typ)
             self.add_value_to_heaps(ref, typ, ret)
             return ret
 
     def find_val_in_heap(self, value: object) -> z3.ExprRef:
         lastheap = self.heaps[-1]
@@ -280,15 +308,15 @@
         return False
     def compute_result(self) -> Tuple[CallAnalysis, bool]:
         raise NotImplementedError
 
 def solver_is_sat(solver, *a) -> bool:
     ret = solver.check(*a)
     if ret == z3.unknown:
-        debug('Unknown satisfiability. Solver state follows:\n', solver)
+        debug('Unknown satisfiability. Solver state follows:\n', solver.sexpr())
         raise UnknownSatisfiability
     return ret == z3.sat
     
 def node_result(node: Optional[NodeLike]) -> Optional[CallAnalysis]:
     if node is None:
         return None
     return node.get_result()
@@ -367,14 +395,16 @@
 class ParallelNode(RandomizedBinaryPathNode):
     '''
     Chooses either path; the first complete result will be used.
     '''
     def __init__(self, false_probability: float):
         super().__init__()
         self._false_probability = false_probability
+    def __repr__(self):
+        return f'ParallelNode(false_frac={self._false_probability})'
     def compute_result(self) -> Tuple[CallAnalysis, bool]:
         self._simplify()
         pos_exhausted = self.positive.is_exhausted()
         neg_exhausted = self.negative.is_exhausted()
         if pos_exhausted and not node_status(self.positive) == VerificationStatus.UNKNOWN:
             return (self.positive.get_result(), True)
         if neg_exhausted and not node_status(self.negative) == VerificationStatus.UNKNOWN:
@@ -409,27 +439,31 @@
 class WorstResultNode(RandomizedBinaryPathNode):
     forced_path: Optional[bool] = None
     def __init__(self, rand: random.Random, expr: z3.ExprRef, solver: z3.Solver):
         RandomizedBinaryPathNode.__init__(self, rand)
         notexpr = z3.Not(expr)
         could_be_true = solver_is_sat(solver, expr)
         could_be_false = solver_is_sat(solver, notexpr)
-        #debug(expr, ' true?', could_be_true, ' false?', could_be_false)
         if (not could_be_true) and (not could_be_false):
             debug(' *** Reached impossible code path *** ')
             debug('Current solver state:\n', str(solver))
             raise CrosshairInternal('Reached impossible code path')
         elif not could_be_true:
             self.forced_path = False
         elif not could_be_false:
             self.forced_path = True
-        #self._dbgstr = str(expr) + ' forced=' + str(self.forced_path)
+        self._expr = expr  # note: this is only used for debugging
+
+    def _is_exhausted(self):
+        return ((self.positive.is_exhausted() and self.negative.is_exhausted()) or
+                (self.forced_path is True and self.positive.is_exhausted()) or
+                (self.forced_path is False and self.negative.is_exhausted()))
 
-    #def __str__(self):
-    #    return f'WorstResultNode({self._dbgstr})'
+    def __repr__(self):
+        return f'WorstResultNode({self._expr}{" : exhausted" if self._is_exhausted() else ""})'
     
     def choose(self, favor_true=False) -> Tuple[bool, NodeLike]:
         if self.forced_path is None:
             return RandomizedBinaryPathNode.choose(self, favor_true)
         return (self.forced_path, self.positive if self.forced_path else self.negative)
         
     def false_probability(self):
@@ -440,18 +474,15 @@
         #   biases for the last item in the union.
         # We pick a False value more than 2/3rds of the time to avoid
         # explosions while constructing binary-tree-like objects.
         return 0.75
 
     def compute_result(self) -> Tuple[CallAnalysis, bool]:
         self._simplify()
-        exhausted = (
-            (self.positive.is_exhausted() and self.negative.is_exhausted()) or
-            (self.forced_path is True and self.positive.is_exhausted()) or
-            (self.forced_path is False and self.negative.is_exhausted()))
+        exhausted = self._is_exhausted()
         if node_status(self.positive) == VerificationStatus.REFUTED or (self.forced_path is True):
             return (self.positive.get_result(), exhausted)
         if node_status(self.negative) == VerificationStatus.REFUTED or (self.forced_path is False):
             return (self.negative.get_result(), exhausted)
         return merge_node_results(self.positive.get_result(), self.positive.is_exhausted(), self.negative)
 
 class ModelValueNode(WorstResultNode):
@@ -495,15 +526,15 @@
         self.choices_made.append(node)
         ret, next_node = node.choose()
         self.search_position = next_node
         return ret
 
     def choose_possible(self, expr: z3.ExprRef, favor_true=False) -> bool:
         with self.framework():
-            if time.time() > self.execution_deadline:
+            if time.monotonic() > self.execution_deadline:
                 debug('Path execution timeout after making ',
                       len(self.choices_made), ' choices.')
                 raise PathTimeout
             notexpr = z3.Not(expr)
             if self.search_position.is_stem():
                 self.search_position = self.search_position.grow_into(
                     WorstResultNode(self._random, expr, self.solver))
@@ -545,18 +576,19 @@
                 if self.search_position.is_stem():
                     self.search_position = self.search_position.grow_into(ModelValueNode(self._random, expr, self.solver))
                 node = self.search_position.simplify()
                 assert isinstance(node, ModelValueNode)
                 (chosen, next_node) = node.choose(favor_true=True)
                 self.choices_made.append(node)
                 self.search_position = next_node
-                #if self.choose_possible(self, expr == node.condition_value, favor_true=False) -> bool:
                 if chosen:
                     self.solver.add(expr == node.condition_value)
-                    #debug('CHOOSE', expr == node.condition_value)
+                    if in_debug():
+                        debug('SMT realized symbolic:', expr == node.condition_value)
+                        debug('Realized at', tiny_stack())
                     return model_value_to_python(node.condition_value)
                 else:
                     self.solver.add(expr != node.condition_value)
     
     def find_model_value_for_function(self, expr: z3.ExprRef) -> object:
         # TODO: this need to go into a tree node that returns UNKNOWN or worse
         # (because it just returns one example function; it's not covering the space)
@@ -593,15 +625,16 @@
             assert isinstance(self.search_position, SearchTreeNode)
             self.search_position.exhausted = True
             self.search_position.result = analysis
         if not self.choices_made:
             return (analysis, True)
         for node in reversed(self.choices_made):
             node.update_result()
+        #debug('Path summary:', self.choices_made)
         first = self.choices_made[0]
         return (first.get_result(), first.is_exhausted())
 
 class SimpleStateSpace(TrackingStateSpace):
     def __init__(self):
         search_root = SinglePathNode(True)
-        super().__init__(time.time() + 10000.0, 10000.0, search_root)
+        super().__init__(time.monotonic() + 10000.0, 10000.0, search_root)
```

### Comparing `crosshair-tool-0.0.8/crosshair/test_util.py` & `crosshair-tool-0.0.9/crosshair/test_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 from dataclasses import replace
 import types
 
 from crosshair.core import analyze_function
 from crosshair.core import AnalysisMessage
 from crosshair.core import AnalysisOptions
 from crosshair.core import MessageType
+from crosshair.core import DEFAULT_OPTIONS
 from typing import *
 
 ComparableLists = Tuple[List, List]
 
-def check_fail(fn: Callable, options: Optional[AnalysisOptions]=None) -> ComparableLists:
+def check_fail(fn: Callable, options: AnalysisOptions=DEFAULT_OPTIONS) -> ComparableLists:
+    if options is DEFAULT_OPTIONS:
+        options = replace(options, max_iterations=20)
     messages = analyze_function(fn, options) if options else analyze_function(fn)
     return ([m.state for m in messages], [MessageType.POST_FAIL])
 
 
 def check_exec_err(fn: Callable, message_prefix='') -> ComparableLists:
-    messages = analyze_function(fn)
+    options = replace(DEFAULT_OPTIONS, max_iterations=20)
+    messages = analyze_function(fn, options)
     if all(m.message.startswith(message_prefix) for m in messages):
         return ([m.state for m in messages], [MessageType.EXEC_ERR])
     else:
         return ([(m.state, m.message) for m in messages], [(MessageType.EXEC_ERR, message_prefix)])
 
 
 def check_post_err(fn: Callable) -> ComparableLists:
-    return ([m.state for m in analyze_function(fn)], [MessageType.POST_ERR])
+    options = replace(DEFAULT_OPTIONS, max_iterations=20)
+    return ([m.state for m in analyze_function(fn, options)], [MessageType.POST_ERR])
 
 
 def check_unknown(fn: Callable) -> ComparableLists:
-    return ([(m.state, m.message, m.traceback) for m in analyze_function(fn)],
+    options = replace(DEFAULT_OPTIONS, max_iterations=40)
+    return ([(m.state, m.message, m.traceback) for m in analyze_function(fn, options)],
             [(MessageType.CANNOT_CONFIRM, 'Not confirmed.', '')])
 
 
-def check_ok(fn: Callable, options: Optional[AnalysisOptions]=None) -> ComparableLists:
+def check_ok(fn: Callable, options: AnalysisOptions=DEFAULT_OPTIONS) -> ComparableLists:
+    if options is DEFAULT_OPTIONS:
+        options = replace(options, per_condition_timeout=5)
     messages = analyze_function(fn, options) if options else analyze_function(fn)
     messages = [m for m in messages if m.state != MessageType.CONFIRMED]
     return (messages, [])
 
 
 def check_messages(msgs: List[AnalysisMessage], **kw) -> ComparableLists:
     if kw.get('state') != MessageType.CONFIRMED:
```

### Comparing `crosshair-tool-0.0.8/crosshair/type_repo.py` & `crosshair-tool-0.0.9/crosshair/type_repo.py`

 * *Files identical despite different names*

### Comparing `crosshair-tool-0.0.8/crosshair_tool.egg-info/PKG-INFO` & `crosshair-tool-0.0.9/crosshair_tool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosshair-tool
-Version: 0.0.8
+Version: 0.0.9
 Summary: A static analysis tool for Python using symbolic execution.
 Home-page: https://github.com/pschanely/CrossHair
 Author: Phillip Schanely
 Author-email: pschanely+vE7F@gmail.com
 License: MIT
 Description: <img src="https://raw.githubusercontent.com/pschanely/CrossHair/master/doc/logo.png" width="5%" align="left">
         
@@ -12,36 +12,39 @@
         
         [![Join the chat at https://gitter.im/Cross_Hair/Lobby](https://badges.gitter.im/Cross_Hair/Lobby.svg)](https://gitter.im/Cross_Hair/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
         [![codecov](https://codecov.io/gh/pschanely/CrossHair/branch/master/graph/badge.svg)](https://codecov.io/gh/pschanely/CrossHair)
         [![Build Status](https://travis-ci.org/pschanely/CrossHair.svg?branch=master)](https://travis-ci.org/pschanely/CrossHair)
         
         An analysis tool for Python that blurs the line between testing and type systems.
         
-        > **_THE LATEST NEWS:_**  Now you can try out CrossHair in your browser at [crosshair-web.org](https://crosshair-web.org)!
+        > **_THE LATEST NEWS:_**  CrossHair is growing commands unrelated to contracts; compare the behavior of two functions with the [diffbehavior](https://raw.githubusercontent.com/pschanely/CrossHair/master/doc/diff_behavior.md) command!
         
         If you have functions with [type annotations](https://www.python.org/dev/peps/pep-0484/) and add some checks in a [PEP 316](https://www.python.org/dev/peps/pep-0316/)-inspired syntax, CrossHair will attempt to find counterexamples for you:
         
         ![Animated GIF demonstrating the verification of a python function](https://raw.githubusercontent.com/pschanely/CrossHair/master/doc/duplicate_list.gif)
         
         CrossHair works by repeatedly calling your functions with symbolic inputs.
         It uses an [SMT solver](https://en.wikipedia.org/wiki/Satisfiability_modulo_theories) (a kind of theorem prover) to explore viable execution paths and find counterexamples for you.
         This is not a new idea; an approach for Python was first described in [this paper](https://hoheinzollern.files.wordpress.com/2008/04/seer1.pdf).
         However, to my knowledge, CrossHair is the most complete implementation of the idea: it supports symbolic lists, dictionaries, sets, and custom/mutable objects.
         
-        > **_NOTE:_**  CrossHair is in a highly experimental state right now. You can help though - keep reading!
+        Try CrossHair right now, in your browser, at [crosshair-web.org](https://crosshair-web.org)!
+        
+        > **_NOTE:_**  CrossHair is in an experimental state right now. You can help though - keep reading!
         
         |Contents|
         |--------|
         |[Why Should I Use CrossHair?](#why-should-i-use-crosshair)|
         |[How to Write Contracts](#how-to-write-contracts)|
         |[Get Started](#get-started)|
         |[IDE Integrations](#ide-integrations)|
         |[Limitations](#limitations)|
         |[How Can I Help?](#how-can-i-help)|
         |[Contributors](#contributors)|
+        |[Change Log](#change-log)|
         |[Related Work](#related-work)|
         
         
         
         ## Why Should I Use CrossHair?
         
         **More precision.** Commonly, we care about more than just the type. Is it really any integer, or is it a **positive** integer? Is it any list, or does it have to be a non-empty list? CrossHair gives you that precision:
@@ -95,15 +98,15 @@
         
         You can find examples in the [examples/](https://github.com/pschanely/CrossHair/tree/master/crosshair/examples) directory 
         and try it in your browser at [crosshair-web.org](https://crosshair-web.org).
         
         
         ## Get Started
         
-        > **_NOTE:_**  CrossHair is in a highly experimental state right now. If you're using it, it's because you want it to succeed, want to help, or are just interested in the technology.
+        > **_NOTE:_**  CrossHair is in an experimental state right now. If you're using it, it's because you want it to succeed, want to help, or are just interested in the technology.
         
         CrossHair is supported only on Python 3.7+ and only on CPython (the most common Python implementation).
         
         Inside the development environment of the code you want to analyze (virtual environment, conda environment, etc), install:
         ```shell
         pip install crosshair-tool
         ```
@@ -127,22 +130,24 @@
         
         If you make a plugin for your favorite editor (please do!), submit a pull request to add it above. The `crosshair check [FILENAME]` command will yield results in the same format as the mypy type checker. (a non-zero exit for for errors, and lines formatted as `{FILENAME}:{LINE_NUMBER}:error:{MESSAGE}`)
         
         ## Limitations
         
         A (wildly incomplete) list of present limitations. Some of these will be lifted over time (your help is welcome!); some may never be lifted.
         
+        * Be aware that the absence of a counterexample does not guarantee that the property holds.
         * Symbolic values are implemented as Python proxy values. CrossHair monkey-patches the system to maintain a good illusion, but the illusion is not complete. For example,
           * Code that cares about the identity values (x is y) may not be correctly analyzed.
           * Code that cares about the types of values may not be correctly analyzed.
         * Only function and class definitions at the top level are analyzed. (i.e. not when nested inside other functions/classes)
         * Only deteministic behavior can be analyzed. (your code always does the same thing when starting with the same values)
           * CrossHair may produce a `NotDeterministic` error when it detects this.
+        * Be careful: CrossHair will actually run your code and may apply any arguments to it.
+          * If you run CrossHair on code calling [shutil.rmtree](https://docs.python.org/3/library/shutil.html#shutil.rmtree), you **will** destroy your filesystem.
         * Comsuming values of an iterator/generator in a pre- or post-condition will produce [unexpected behavior](https://github.com/pschanely/CrossHair/issues/9).
-        * Be aware that the absence of a counterexample does not guarantee that the property holds.
         * SMT sovlers have very different perspectives on hard problems and easy problems than humans.
           * Be prepared to be surprised both by what CrossHair can tell you, and what it cannot.
         
         ## How Can I Help?
         
         * [Try it out](#get-started) on your own python project! Be communicative about what does and doesn't work.
         * Participate (or just lurk) in the [gitter chat](https://gitter.im/Cross_Hair/Lobby).
@@ -154,20 +159,28 @@
         
         ## Contributors
         
         * [**Phil Schanely**](https://twitter.com/pschanely)
         * [**Edward Haigh**](https://github.com/oneEdoubleD)
         * [**Saul Shanabrook**](https://github.com/saulshanabrook/)
         
+        ## Change Log
+        
+        0.0.9
+        * Introduce [the diffbehavior command](https://raw.githubusercontent.com/pschanely/CrossHair/master/doc/diff_behavior.md) which finds inputs that distinguish the behavior of two functions.
+        * Upgrade to the latest release of z3 (4.8.9.0)
+        * Fix [an installation error](https://github.com/pschanely/CrossHair/issues/41) on windows.
+        * Fix a variety of other bugs.
+        
         ## Related Work
         
         |Technology|Relation|
         |---------:|:-------|
         | [dependent types](https://en.wikipedia.org/wiki/Dependent_type), [refinement types](https://en.wikipedia.org/wiki/Refinement_type) | CrossHair aims to provide many of the same capabilities as these advanced type systems. CrossHair is easier to learn (because it is just python), but is incomplete (it can't always tell you whether a condition holds). |
-        | [design by contract](https://en.wikipedia.org/wiki/Design_by_contract) | Unlike other systems and tools for contracts, CrossHair attempts to verify pre- and post-conditions before you run them. |
+        | [design by contract](https://en.wikipedia.org/wiki/Design_by_contract) | Unlike most tools for contracts, CrossHair attempts to verify pre-conditions and post-conditions before you run them. |
         | [fuzz testing](https://en.wikipedia.org/wiki/Fuzzing), [QuickCheck](https://en.wikipedia.org/wiki/QuickCheck), [property testing](https://en.wikipedia.org/wiki/Property_testing), [Hypothesis](https://hypothesis.readthedocs.io/) | CrossHair has many of the same goals as these tools. However, CrossHair uses an SMT solver to find inputs rather than the (typically) randomized approaches that these tools use. |
         | [concolic testing](https://en.wikipedia.org/wiki/Concolic_testing) | State-of-the-art fuzz testers employ SMT solvers in a similar fashion as CrossHair. |
         | [SMT solvers](https://en.wikipedia.org/wiki/Satisfiability_modulo_theories) | SMT solvers power many of the tools in this table. CrossHair uses [Z3](https://github.com/Z3Prover/z3). |
         | [angr](https://angr.io), [klee](https://klee.github.io/) | Symbolic execution of **binary** code. Unlike these tools, CrossHair models the semantics of Python directly. |
         | [PyExZ3](https://github.com/thomasjball/PyExZ3), [pySim](https://github.com/bannsec/pySym), [PEF](https://git.cs.famaf.unc.edu.ar/dbarsotti/pef) | Take approaches that are very similar to CrossHair, in various states of completeness. CrossHair is generally more perscriptive or product-like than these tools. |
         
 Platform: UNKNOWN
```

### Comparing `crosshair-tool-0.0.8/crosshair_tool.egg-info/SOURCES.txt` & `crosshair-tool-0.0.9/crosshair_tool.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 README.md
-setup.cfg
 setup.py
 crosshair/__init__.py
 crosshair/abcstring.py
 crosshair/condition_parser.py
 crosshair/condition_parser_test.py
 crosshair/core.py
 crosshair/core_and_libs.py
 crosshair/core_test.py
+crosshair/diff_behavior.py
+crosshair/diff_behavior_test.py
 crosshair/doctests_test.py
 crosshair/dynamic_typing.py
 crosshair/dynamic_typing_test.py
 crosshair/enforce.py
 crosshair/enforce_test.py
 crosshair/fuzz_core_test.py
 crosshair/localhost_comms.py
@@ -21,14 +22,15 @@
 crosshair/objectproxy_test.py
 crosshair/simplestructs.py
 crosshair/simplestructs_test.py
 crosshair/statespace.py
 crosshair/test_util.py
 crosshair/type_repo.py
 crosshair/util.py
+crosshair/util_test.py
 crosshair/examples/__init__.py
 crosshair/examples/arith.py
 crosshair/examples/chess.py
 crosshair/examples/hash_consistent_with_equals.py
 crosshair/examples/immutable_class.py
 crosshair/examples/nesting_inference.py
 crosshair/examples/numpy_examples.py
```

### Comparing `crosshair-tool-0.0.8/setup.py` & `crosshair-tool-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import unittest
 
 setup(
     name='crosshair-tool',
-    version='0.0.8',
+    version='0.0.9',
     author='Phillip Schanely',
     author_email='pschanely+vE7F@gmail.com',
     packages=find_packages(),
     scripts=[],
     entry_points = {
         'console_scripts': ['crosshair=crosshair.main:main'],
     },
@@ -15,15 +15,15 @@
     license='MIT',
     description='A static analysis tool for Python using symbolic execution.',
     long_description=open('README.md').read().replace('doc/', 'https://raw.githubusercontent.com/pschanely/CrossHair/master/doc/'),
     long_description_content_type='text/markdown',
     install_requires=[
         'forbiddenfruit',
         'typing-inspect',
-        'z3-solver-crosshair',
+        'z3-solver==4.8.9.0',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

