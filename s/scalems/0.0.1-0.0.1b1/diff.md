# Comparing `tmp/scalems-0.0.1.tar.gz` & `tmp/scalems-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalems-0.0.1.tar", last modified: Thu May  4 21:36:04 2023, max compression
+gzip compressed data, was "scalems-0.0.1b1.tar", last modified: Wed Apr 26 17:22:55 2023, max compression
```

## Comparing `scalems-0.0.1.tar` & `scalems-0.0.1b1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.790155 scalems-0.0.1/
--rw-r--r--   0 eric       (501) staff       (20)    26526 2022-10-13 13:53:44.000000 scalems-0.0.1/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)     3545 2023-05-04 21:36:04.789774 scalems-0.0.1/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2970 2022-12-15 15:31:32.000000 scalems-0.0.1/README.md
--rw-r--r--   0 eric       (501) staff       (20)     1969 2023-05-04 21:17:10.000000 scalems-0.0.1/pyproject.toml
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.747559 scalems-0.0.1/scalems.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     3545 2023-05-04 21:36:04.000000 scalems-0.0.1/scalems.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1424 2023-05-04 21:36:04.000000 scalems-0.0.1/scalems.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-04 21:36:04.000000 scalems-0.0.1/scalems.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       68 2023-05-04 21:36:04.000000 scalems-0.0.1/scalems.egg-info/entry_points.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-04 20:29:54.000000 scalems-0.0.1/scalems.egg-info/not-zip-safe
--rw-r--r--   0 eric       (501) staff       (20)      132 2023-05-04 21:36:04.000000 scalems-0.0.1/scalems.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)        8 2023-05-04 21:36:04.000000 scalems-0.0.1/scalems.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-04 21:36:04.790273 scalems-0.0.1/setup.cfg
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.736397 scalems-0.0.1/src/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.758868 scalems-0.0.1/src/scalems/
--rw-r--r--   0 eric       (501) staff       (20)     2995 2023-01-09 11:13:55.000000 scalems-0.0.1/src/scalems/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      553 2022-12-15 15:31:32.000000 scalems-0.0.1/src/scalems/_types.py
--rw-r--r--   0 eric       (501) staff       (20)       22 2023-05-04 21:36:04.000000 scalems-0.0.1/src/scalems/_version.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.761256 scalems-0.0.1/src/scalems/call/
--rw-r--r--   0 eric       (501) staff       (20)    17659 2023-04-25 16:17:43.000000 scalems-0.0.1/src/scalems/call/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      102 2023-03-08 08:35:01.000000 scalems-0.0.1/src/scalems/call/__main__.py
--rw-r--r--   0 eric       (501) staff       (20)    10755 2023-01-04 17:26:04.000000 scalems-0.0.1/src/scalems/commands.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.762327 scalems-0.0.1/src/scalems/context/
--rw-r--r--   0 eric       (501) staff       (20)     1879 2023-03-27 14:38:51.000000 scalems-0.0.1/src/scalems/context/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     2873 2023-01-09 11:14:17.000000 scalems-0.0.1/src/scalems/exceptions.py
--rw-r--r--   0 eric       (501) staff       (20)    27014 2023-04-25 15:56:49.000000 scalems-0.0.1/src/scalems/execution.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.763272 scalems-0.0.1/src/scalems/file/
--rw-r--r--   0 eric       (501) staff       (20)     8407 2023-04-25 15:55:46.000000 scalems-0.0.1/src/scalems/file/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    13542 2023-01-15 11:20:23.000000 scalems-0.0.1/src/scalems/identifiers.py
--rw-r--r--   0 eric       (501) staff       (20)    12930 2023-03-27 14:14:03.000000 scalems-0.0.1/src/scalems/invocation.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.767521 scalems-0.0.1/src/scalems/local/
--rw-r--r--   0 eric       (501) staff       (20)    10510 2023-03-22 15:39:49.000000 scalems-0.0.1/src/scalems/local/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      247 2022-12-15 15:31:32.000000 scalems-0.0.1/src/scalems/local/__main__.py
--rw-r--r--   0 eric       (501) staff       (20)    11347 2023-01-04 17:26:04.000000 scalems-0.0.1/src/scalems/local/operations.py
--rw-r--r--   0 eric       (501) staff       (20)     1906 2023-01-04 17:21:23.000000 scalems-0.0.1/src/scalems/logger.py
--rw-r--r--   0 eric       (501) staff       (20)    10204 2022-12-15 15:31:32.000000 scalems-0.0.1/src/scalems/messages.py
--rw-r--r--   0 eric       (501) staff       (20)       47 2021-08-27 15:59:17.000000 scalems-0.0.1/src/scalems/py.typed
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.769783 scalems-0.0.1/src/scalems/radical/
--rw-r--r--   0 eric       (501) staff       (20)     2552 2023-03-27 14:14:03.000000 scalems-0.0.1/src/scalems/radical/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      336 2023-01-18 10:57:59.000000 scalems-0.0.1/src/scalems/radical/__main__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.771541 scalems-0.0.1/src/scalems/radical/raptor/
--rw-r--r--   0 eric       (501) staff       (20)    62350 2023-04-25 16:17:43.000000 scalems-0.0.1/src/scalems/radical/raptor/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    90832 2023-04-25 16:17:43.000000 scalems-0.0.1/src/scalems/radical/runtime.py
--rw-r--r--   0 eric       (501) staff       (20)    22734 2022-12-15 15:31:32.000000 scalems-0.0.1/src/scalems/serialization.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.774179 scalems-0.0.1/src/scalems/store/
--rw-r--r--   0 eric       (501) staff       (20)    34546 2023-04-25 15:55:46.000000 scalems-0.0.1/src/scalems/store/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     5541 2023-01-15 11:20:23.000000 scalems-0.0.1/src/scalems/store/_lock.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.775723 scalems-0.0.1/src/scalems/subprocess/
--rw-r--r--   0 eric       (501) staff       (20)     1161 2022-12-15 15:31:32.000000 scalems-0.0.1/src/scalems/subprocess/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)    18289 2023-03-27 14:38:09.000000 scalems-0.0.1/src/scalems/subprocess/_subprocess.py
--rw-r--r--   0 eric       (501) staff       (20)      658 2023-01-04 17:26:04.000000 scalems-0.0.1/src/scalems/unique.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.777109 scalems-0.0.1/src/scalems/workflow/
--rw-r--r--   0 eric       (501) staff       (20)    62304 2023-04-25 16:17:37.000000 scalems-0.0.1/src/scalems/workflow/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.779913 scalems-0.0.1/src/scalems/wrappers/
--rw-r--r--   0 eric       (501) staff       (20)     8282 2021-09-07 15:49:13.000000 scalems-0.0.1/src/scalems/wrappers/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     7787 2023-01-04 17:26:04.000000 scalems-0.0.1/src/scalems/wrappers/gromacs.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-04 21:36:04.788961 scalems-0.0.1/tests/
--rw-r--r--   0 eric       (501) staff       (20)     3167 2023-03-08 08:35:01.000000 scalems-0.0.1/tests/test_call.py
--rw-r--r--   0 eric       (501) staff       (20)     7488 2023-04-25 15:55:46.000000 scalems-0.0.1/tests/test_context_datastore.py
--rw-r--r--   0 eric       (501) staff       (20)    12569 2022-12-15 15:31:32.000000 scalems-0.0.1/tests/test_datamodel.py
--rw-r--r--   0 eric       (501) staff       (20)    10029 2023-04-25 15:55:46.000000 scalems-0.0.1/tests/test_filereference.py
--rw-r--r--   0 eric       (501) staff       (20)      677 2022-12-15 15:31:32.000000 scalems-0.0.1/tests/test_messages.py
--rw-r--r--   0 eric       (501) staff       (20)     5894 2023-03-31 10:56:59.000000 scalems-0.0.1/tests/test_radical_runtime.py
--rw-r--r--   0 eric       (501) staff       (20)     3667 2023-04-25 15:56:02.000000 scalems-0.0.1/tests/test_raptor_utilities.py
--rwxr-xr-x   0 eric       (501) staff       (20)    22121 2023-04-25 16:17:43.000000 scalems-0.0.1/tests/test_rp_exec.py
--rwxr-xr-x   0 eric       (501) staff       (20)     4147 2023-03-27 14:14:03.000000 scalems-0.0.1/tests/test_rp_future.py
--rwxr-xr-x   0 eric       (501) staff       (20)     9938 2023-03-27 11:39:58.000000 scalems-0.0.1/tests/test_rp_venv.py
--rw-r--r--   0 eric       (501) staff       (20)     3057 2023-04-25 15:55:46.000000 scalems-0.0.1/tests/test_subprocess_exec.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.888139 scalems-0.0.1b1/
+-rw-r--r--   0 eric       (501) staff       (20)    26526 2022-10-13 13:53:44.000000 scalems-0.0.1b1/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)     3547 2023-04-26 17:22:55.887364 scalems-0.0.1b1/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2970 2022-12-15 15:31:32.000000 scalems-0.0.1b1/README.md
+-rw-r--r--   0 eric       (501) staff       (20)     1980 2023-04-25 16:19:05.000000 scalems-0.0.1b1/pyproject.toml
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.842546 scalems-0.0.1b1/scalems.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     3547 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1424 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       68 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/entry_points.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2022-12-05 14:25:19.000000 scalems-0.0.1b1/scalems.egg-info/not-zip-safe
+-rw-r--r--   0 eric       (501) staff       (20)      132 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)        8 2023-04-26 17:22:55.000000 scalems-0.0.1b1/scalems.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-04-26 17:22:55.888369 scalems-0.0.1b1/setup.cfg
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.832113 scalems-0.0.1b1/src/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.854713 scalems-0.0.1b1/src/scalems/
+-rw-r--r--   0 eric       (501) staff       (20)     2995 2023-01-09 11:13:55.000000 scalems-0.0.1b1/src/scalems/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      553 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/_types.py
+-rw-r--r--   0 eric       (501) staff       (20)       24 2023-04-26 17:22:55.000000 scalems-0.0.1b1/src/scalems/_version.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.856716 scalems-0.0.1b1/src/scalems/call/
+-rw-r--r--   0 eric       (501) staff       (20)    17659 2023-04-25 16:17:43.000000 scalems-0.0.1b1/src/scalems/call/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      102 2023-03-08 08:35:01.000000 scalems-0.0.1b1/src/scalems/call/__main__.py
+-rw-r--r--   0 eric       (501) staff       (20)    10755 2023-01-04 17:26:04.000000 scalems-0.0.1b1/src/scalems/commands.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.857789 scalems-0.0.1b1/src/scalems/context/
+-rw-r--r--   0 eric       (501) staff       (20)     1879 2023-03-27 14:38:51.000000 scalems-0.0.1b1/src/scalems/context/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     2873 2023-01-09 11:14:17.000000 scalems-0.0.1b1/src/scalems/exceptions.py
+-rw-r--r--   0 eric       (501) staff       (20)    27014 2023-04-25 15:56:49.000000 scalems-0.0.1b1/src/scalems/execution.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.858753 scalems-0.0.1b1/src/scalems/file/
+-rw-r--r--   0 eric       (501) staff       (20)     8407 2023-04-25 15:55:46.000000 scalems-0.0.1b1/src/scalems/file/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    13542 2023-01-15 11:20:23.000000 scalems-0.0.1b1/src/scalems/identifiers.py
+-rw-r--r--   0 eric       (501) staff       (20)    12930 2023-03-27 14:14:03.000000 scalems-0.0.1b1/src/scalems/invocation.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.864549 scalems-0.0.1b1/src/scalems/local/
+-rw-r--r--   0 eric       (501) staff       (20)    10510 2023-03-22 15:39:49.000000 scalems-0.0.1b1/src/scalems/local/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      247 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/local/__main__.py
+-rw-r--r--   0 eric       (501) staff       (20)    11347 2023-01-04 17:26:04.000000 scalems-0.0.1b1/src/scalems/local/operations.py
+-rw-r--r--   0 eric       (501) staff       (20)     1906 2023-01-04 17:21:23.000000 scalems-0.0.1b1/src/scalems/logger.py
+-rw-r--r--   0 eric       (501) staff       (20)    10204 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/messages.py
+-rw-r--r--   0 eric       (501) staff       (20)       47 2021-08-27 15:59:17.000000 scalems-0.0.1b1/src/scalems/py.typed
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.867459 scalems-0.0.1b1/src/scalems/radical/
+-rw-r--r--   0 eric       (501) staff       (20)     2552 2023-03-27 14:14:03.000000 scalems-0.0.1b1/src/scalems/radical/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      336 2023-01-18 10:57:59.000000 scalems-0.0.1b1/src/scalems/radical/__main__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.868488 scalems-0.0.1b1/src/scalems/radical/raptor/
+-rw-r--r--   0 eric       (501) staff       (20)    62350 2023-04-25 16:17:43.000000 scalems-0.0.1b1/src/scalems/radical/raptor/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    90832 2023-04-25 16:17:43.000000 scalems-0.0.1b1/src/scalems/radical/runtime.py
+-rw-r--r--   0 eric       (501) staff       (20)    22734 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/serialization.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.870496 scalems-0.0.1b1/src/scalems/store/
+-rw-r--r--   0 eric       (501) staff       (20)    34546 2023-04-25 15:55:46.000000 scalems-0.0.1b1/src/scalems/store/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     5541 2023-01-15 11:20:23.000000 scalems-0.0.1b1/src/scalems/store/_lock.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.872703 scalems-0.0.1b1/src/scalems/subprocess/
+-rw-r--r--   0 eric       (501) staff       (20)     1161 2022-12-15 15:31:32.000000 scalems-0.0.1b1/src/scalems/subprocess/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    18289 2023-03-27 14:38:09.000000 scalems-0.0.1b1/src/scalems/subprocess/_subprocess.py
+-rw-r--r--   0 eric       (501) staff       (20)      658 2023-01-04 17:26:04.000000 scalems-0.0.1b1/src/scalems/unique.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.873780 scalems-0.0.1b1/src/scalems/workflow/
+-rw-r--r--   0 eric       (501) staff       (20)    62304 2023-04-25 16:17:37.000000 scalems-0.0.1b1/src/scalems/workflow/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.875788 scalems-0.0.1b1/src/scalems/wrappers/
+-rw-r--r--   0 eric       (501) staff       (20)     8282 2021-09-07 15:49:13.000000 scalems-0.0.1b1/src/scalems/wrappers/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     7787 2023-01-04 17:26:04.000000 scalems-0.0.1b1/src/scalems/wrappers/gromacs.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-26 17:22:55.886387 scalems-0.0.1b1/tests/
+-rw-r--r--   0 eric       (501) staff       (20)     3167 2023-03-08 08:35:01.000000 scalems-0.0.1b1/tests/test_call.py
+-rw-r--r--   0 eric       (501) staff       (20)     7488 2023-04-25 15:55:46.000000 scalems-0.0.1b1/tests/test_context_datastore.py
+-rw-r--r--   0 eric       (501) staff       (20)    12569 2022-12-15 15:31:32.000000 scalems-0.0.1b1/tests/test_datamodel.py
+-rw-r--r--   0 eric       (501) staff       (20)    10029 2023-04-25 15:55:46.000000 scalems-0.0.1b1/tests/test_filereference.py
+-rw-r--r--   0 eric       (501) staff       (20)      677 2022-12-15 15:31:32.000000 scalems-0.0.1b1/tests/test_messages.py
+-rw-r--r--   0 eric       (501) staff       (20)     5894 2023-03-31 10:56:59.000000 scalems-0.0.1b1/tests/test_radical_runtime.py
+-rw-r--r--   0 eric       (501) staff       (20)     3667 2023-04-25 15:56:02.000000 scalems-0.0.1b1/tests/test_raptor_utilities.py
+-rwxr-xr-x   0 eric       (501) staff       (20)    22121 2023-04-25 16:17:43.000000 scalems-0.0.1b1/tests/test_rp_exec.py
+-rwxr-xr-x   0 eric       (501) staff       (20)     4147 2023-03-27 14:14:03.000000 scalems-0.0.1b1/tests/test_rp_future.py
+-rwxr-xr-x   0 eric       (501) staff       (20)     9938 2023-03-27 11:39:58.000000 scalems-0.0.1b1/tests/test_rp_venv.py
+-rw-r--r--   0 eric       (501) staff       (20)     3057 2023-04-25 15:55:46.000000 scalems-0.0.1b1/tests/test_subprocess_exec.py
```

### Comparing `scalems-0.0.1/LICENSE` & `scalems-0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/PKG-INFO` & `scalems-0.0.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalems
-Version: 0.0.1
+Version: 0.0.1b1
 Summary: Reference implementation of the SCALE-MS data flow scripting and graph execution API for molecular science computational research protocols.
 Author-email: SCALE-MS team <info@scalems.org>
 License: LGPL 2.1
 Project-URL: Source, https://github.com/SCALE-MS/scale-ms/
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `scalems-0.0.1/README.md` & `scalems-0.0.1b1/README.md`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/pyproject.toml` & `scalems-0.0.1b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.0", "versioningit~=2.0"]
+requires = ["setuptools>=61.0", "versioningit~=2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scalems"
 dynamic = ["version"]
 description = "Reference implementation of the SCALE-MS data flow scripting and graph execution API for molecular science computational research protocols."
 authors = [{ name = "SCALE-MS team", email = "info@scalems.org" }]
@@ -45,15 +45,15 @@
 
 [tool.setuptools.package-data]
 scalems = [
     "py.typed"
 ]
 
 [tool.versioningit]
-default-version = "0.0.1+unknown"
+default-version = "0.0.1b1+unknown"
 
 [tool.versioningit.format]
 distance = "{base_version}+{distance}.{vcs}{rev}"
 dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
 distance-dirty = "{base_version}+{distance}.{vcs}{rev}.dirty"
 
 [tool.versioningit.vcs]
```

### Comparing `scalems-0.0.1/scalems.egg-info/PKG-INFO` & `scalems-0.0.1b1/scalems.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalems
-Version: 0.0.1
+Version: 0.0.1b1
 Summary: Reference implementation of the SCALE-MS data flow scripting and graph execution API for molecular science computational research protocols.
 Author-email: SCALE-MS team <info@scalems.org>
 License: LGPL 2.1
 Project-URL: Source, https://github.com/SCALE-MS/scale-ms/
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `scalems-0.0.1/scalems.egg-info/SOURCES.txt` & `scalems-0.0.1b1/scalems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/__init__.py` & `scalems-0.0.1b1/src/scalems/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/_types.py` & `scalems-0.0.1b1/src/scalems/_types.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/call/__init__.py` & `scalems-0.0.1b1/src/scalems/call/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/commands.py` & `scalems-0.0.1b1/src/scalems/commands.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/context/__init__.py` & `scalems-0.0.1b1/src/scalems/context/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/exceptions.py` & `scalems-0.0.1b1/src/scalems/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/execution.py` & `scalems-0.0.1b1/src/scalems/execution.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/file/__init__.py` & `scalems-0.0.1b1/src/scalems/file/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/identifiers.py` & `scalems-0.0.1b1/src/scalems/identifiers.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/invocation.py` & `scalems-0.0.1b1/src/scalems/invocation.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/local/__init__.py` & `scalems-0.0.1b1/src/scalems/local/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/local/operations.py` & `scalems-0.0.1b1/src/scalems/local/operations.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/logger.py` & `scalems-0.0.1b1/src/scalems/logger.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/messages.py` & `scalems-0.0.1b1/src/scalems/messages.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/radical/__init__.py` & `scalems-0.0.1b1/src/scalems/radical/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/radical/raptor/__init__.py` & `scalems-0.0.1b1/src/scalems/radical/raptor/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/radical/runtime.py` & `scalems-0.0.1b1/src/scalems/radical/runtime.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/serialization.py` & `scalems-0.0.1b1/src/scalems/serialization.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/store/__init__.py` & `scalems-0.0.1b1/src/scalems/store/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/store/_lock.py` & `scalems-0.0.1b1/src/scalems/store/_lock.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/subprocess/__init__.py` & `scalems-0.0.1b1/src/scalems/subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/subprocess/_subprocess.py` & `scalems-0.0.1b1/src/scalems/subprocess/_subprocess.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/unique.py` & `scalems-0.0.1b1/src/scalems/unique.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/workflow/__init__.py` & `scalems-0.0.1b1/src/scalems/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/wrappers/__init__.py` & `scalems-0.0.1b1/src/scalems/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/src/scalems/wrappers/gromacs.py` & `scalems-0.0.1b1/src/scalems/wrappers/gromacs.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_call.py` & `scalems-0.0.1b1/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_context_datastore.py` & `scalems-0.0.1b1/tests/test_context_datastore.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_datamodel.py` & `scalems-0.0.1b1/tests/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_filereference.py` & `scalems-0.0.1b1/tests/test_filereference.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_messages.py` & `scalems-0.0.1b1/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_radical_runtime.py` & `scalems-0.0.1b1/tests/test_radical_runtime.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_raptor_utilities.py` & `scalems-0.0.1b1/tests/test_raptor_utilities.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_rp_exec.py` & `scalems-0.0.1b1/tests/test_rp_exec.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_rp_future.py` & `scalems-0.0.1b1/tests/test_rp_future.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_rp_venv.py` & `scalems-0.0.1b1/tests/test_rp_venv.py`

 * *Files identical despite different names*

### Comparing `scalems-0.0.1/tests/test_subprocess_exec.py` & `scalems-0.0.1b1/tests/test_subprocess_exec.py`

 * *Files identical despite different names*

