# Comparing `tmp/yerbamate-0.9.23.tar.gz` & `tmp/yerbamate-0.9.235.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yerbamate-0.9.23.tar", last modified: Wed May  3 21:05:38 2023, max compression
+gzip compressed data, was "yerbamate-0.9.235.tar", last modified: Wed May  3 22:47:29 2023, max compression
```

## Comparing `yerbamate-0.9.23.tar` & `yerbamate-0.9.235.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.459908 yerbamate-0.9.23/
--rw-r--r--   0 al        (1000) al        (1001)     1079 2023-04-08 19:56:23.000000 yerbamate-0.9.23/LICENSE
--rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.23/MANIFEST.in
--rw-r--r--   0 al        (1000) al        (1001)    11581 2023-05-03 21:05:38.460908 yerbamate-0.9.23/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1001)    10948 2023-04-08 19:56:23.000000 yerbamate-0.9.23/README.md
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.449909 yerbamate-0.9.23/packages/
--rw-r--r--   0 al        (1000) al        (1001)      112 2023-04-22 15:20:01.000000 yerbamate-0.9.23/packages/requirements.txt
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.450909 yerbamate-0.9.23/packages/yerbamate/
--rw-r--r--   0 al        (1000) al        (1001)      130 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.452909 yerbamate-0.9.23/packages/yerbamate/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      291 2023-04-08 19:57:52.000000 yerbamate-0.9.23/packages/yerbamate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     4429 2023-04-09 09:45:27.000000 yerbamate-0.9.23/packages/yerbamate/__pycache__/environment.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     8269 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/__pycache__/mate.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     9389 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.452909 yerbamate-0.9.23/packages/yerbamate/api/
--rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.453909 yerbamate-0.9.23/packages/yerbamate/api/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      153 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1427 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.453909 yerbamate-0.9.23/packages/yerbamate/api/data/
--rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.454908 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      197 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5655 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)    11315 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     3316 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     9460 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/module_manager.py
--rw-r--r--   0 al        (1000) al        (1001)    14686 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/module_repository.py
--rw-r--r--   0 al        (1000) al        (1001)     3447 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/package.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.454908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/
--rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.455908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      166 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1127 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.455908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/
--rw-r--r--   0 al        (1000) al        (1001)       35 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.456908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      217 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5521 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5734 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     5573 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/io.py
--rw-r--r--   0 al        (1000) al        (1001)     5130 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/local.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.456908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/
--rw-r--r--   0 al        (1000) al        (1001)       37 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.456908 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      220 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     2132 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1078 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/remote.py
--rw-r--r--   0 al        (1000) al        (1001)      365 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/sources/source.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.457908 yerbamate-0.9.23/packages/yerbamate/api/data/utils/
--rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.458908 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)      164 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)      540 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     1035 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     4487 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)      326 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/exp_util.py
--rw-r--r--   0 al        (1000) al        (1001)     1197 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/git_util.py
--rw-r--r--   0 al        (1000) al        (1001)     7395 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/data/utils/gitdir.py
--rw-r--r--   0 al        (1000) al        (1001)      869 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/api/mate_api.py
--rw-r--r--   0 al        (1000) al        (1001)      294 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/constants.py
--rw-r--r--   0 al        (1000) al        (1001)     5857 2023-05-03 21:03:55.000000 yerbamate-0.9.23/packages/yerbamate/environment.py
--rw-r--r--   0 al        (1000) al        (1001)     7829 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/mate.py
--rw-r--r--   0 al        (1000) al        (1001)    10611 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/mate_cli.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.458908 yerbamate-0.9.23/packages/yerbamate/utils/
--rw-r--r--   0 al        (1000) al        (1001)     1433 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/utils/__init__.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.459908 yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/
--rw-r--r--   0 al        (1000) al        (1001)     2016 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)      814 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     3761 2023-04-09 10:03:11.000000 yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 al        (1000) al        (1001)     2145 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/utils/bunch.py
--rw-r--r--   0 al        (1000) al        (1001)     1386 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/utils/git_url_parser.py
--rw-r--r--   0 al        (1000) al        (1001)     4419 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/utils/utils.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.459908 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/
--rw-r--r--   0 al        (1000) al        (1001)      601 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1001)      342 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) al        (1001)        1 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) al        (1001)       10 2023-04-08 19:56:23.000000 yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/top_level.txt
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.451908 yerbamate-0.9.23/packages/yerbamate.egg-info/
--rw-r--r--   0 al        (1000) al        (1001)    11581 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) al        (1001)     3195 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) al        (1001)        1 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) al        (1001)       82 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/requires.txt
--rw-r--r--   0 al        (1000) al        (1001)       10 2023-05-03 21:05:38.000000 yerbamate-0.9.23/packages/yerbamate.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) al        (1001)      107 2023-05-03 21:05:38.460908 yerbamate-0.9.23/setup.cfg
--rw-r--r--   0 al        (1000) al        (1001)     1278 2023-05-03 21:04:55.000000 yerbamate-0.9.23/setup.py
-drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 21:05:38.449909 yerbamate-0.9.23/src/
--rwxr-xr-x   0 al        (1000) al        (1001)       62 2023-04-08 19:56:23.000000 yerbamate-0.9.23/src/mate
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.119415 yerbamate-0.9.235/
+-rw-r--r--   0 al        (1000) al        (1001)     1079 2023-04-08 19:56:23.000000 yerbamate-0.9.235/LICENSE
+-rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.235/MANIFEST.in
+-rw-r--r--   0 al        (1000) al        (1001)    11582 2023-05-03 22:47:29.119415 yerbamate-0.9.235/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)    10948 2023-04-08 19:56:23.000000 yerbamate-0.9.235/README.md
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.108415 yerbamate-0.9.235/packages/
+-rw-r--r--   0 al        (1000) al        (1001)      112 2023-04-22 15:20:01.000000 yerbamate-0.9.235/packages/requirements.txt
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.109415 yerbamate-0.9.235/packages/yerbamate/
+-rw-r--r--   0 al        (1000) al        (1001)      130 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.111415 yerbamate-0.9.235/packages/yerbamate/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      291 2023-04-08 19:57:52.000000 yerbamate-0.9.235/packages/yerbamate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     4470 2023-05-03 21:23:06.000000 yerbamate-0.9.235/packages/yerbamate/__pycache__/environment.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     8269 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/__pycache__/mate.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9389 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.111415 yerbamate-0.9.235/packages/yerbamate/api/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.111415 yerbamate-0.9.235/packages/yerbamate/api/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      153 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1427 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.112415 yerbamate-0.9.235/packages/yerbamate/api/data/
+-rw-r--r--   0 al        (1000) al        (1001)       29 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.113415 yerbamate-0.9.235/packages/yerbamate/api/data/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      197 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5655 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)    11926 2023-05-03 21:24:59.000000 yerbamate-0.9.235/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3316 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     9460 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/module_manager.py
+-rw-r--r--   0 al        (1000) al        (1001)    15485 2023-05-03 21:24:50.000000 yerbamate-0.9.235/packages/yerbamate/api/data/module_repository.py
+-rw-r--r--   0 al        (1000) al        (1001)     3447 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/package.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.113415 yerbamate-0.9.235/packages/yerbamate/api/data/sources/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.113415 yerbamate-0.9.235/packages/yerbamate/api/data/sources/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      166 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1127 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.114415 yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/
+-rw-r--r--   0 al        (1000) al        (1001)       35 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.114415 yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      217 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5521 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5734 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     5573 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/io.py
+-rw-r--r--   0 al        (1000) al        (1001)     5130 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/local.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.115415 yerbamate-0.9.235/packages/yerbamate/api/data/sources/remote/
+-rw-r--r--   0 al        (1000) al        (1001)       37 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/remote/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.115415 yerbamate-0.9.235/packages/yerbamate/api/data/sources/remote/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      220 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/remote/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2132 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1078 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/remote/remote.py
+-rw-r--r--   0 al        (1000) al        (1001)      365 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/sources/source.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.116415 yerbamate-0.9.235/packages/yerbamate/api/data/utils/
+-rw-r--r--   0 al        (1000) al        (1001)        0 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/utils/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.117415 yerbamate-0.9.235/packages/yerbamate/api/data/utils/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)      164 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      540 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     1035 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     4487 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      326 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/utils/exp_util.py
+-rw-r--r--   0 al        (1000) al        (1001)     1197 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/utils/git_util.py
+-rw-r--r--   0 al        (1000) al        (1001)     7395 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/data/utils/gitdir.py
+-rw-r--r--   0 al        (1000) al        (1001)      869 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/api/mate_api.py
+-rw-r--r--   0 al        (1000) al        (1001)      294 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/constants.py
+-rw-r--r--   0 al        (1000) al        (1001)     5910 2023-05-03 22:46:41.000000 yerbamate-0.9.235/packages/yerbamate/environment.py
+-rw-r--r--   0 al        (1000) al        (1001)     7829 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/mate.py
+-rw-r--r--   0 al        (1000) al        (1001)    10611 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/mate_cli.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.118414 yerbamate-0.9.235/packages/yerbamate/utils/
+-rw-r--r--   0 al        (1000) al        (1001)     1433 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/utils/__init__.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.118414 yerbamate-0.9.235/packages/yerbamate/utils/__pycache__/
+-rw-r--r--   0 al        (1000) al        (1001)     2016 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)      814 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     3761 2023-04-09 10:03:11.000000 yerbamate-0.9.235/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 al        (1000) al        (1001)     2145 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/utils/bunch.py
+-rw-r--r--   0 al        (1000) al        (1001)     1386 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/utils/git_url_parser.py
+-rw-r--r--   0 al        (1000) al        (1001)     4419 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/utils/utils.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.119415 yerbamate-0.9.235/packages/yerbamate/yerbamate.egg-info/
+-rw-r--r--   0 al        (1000) al        (1001)      601 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/yerbamate.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)      342 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/yerbamate.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) al        (1001)        1 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/yerbamate.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) al        (1001)       10 2023-04-08 19:56:23.000000 yerbamate-0.9.235/packages/yerbamate/yerbamate.egg-info/top_level.txt
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.110415 yerbamate-0.9.235/packages/yerbamate.egg-info/
+-rw-r--r--   0 al        (1000) al        (1001)    11582 2023-05-03 22:47:28.000000 yerbamate-0.9.235/packages/yerbamate.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) al        (1001)     3195 2023-05-03 22:47:29.000000 yerbamate-0.9.235/packages/yerbamate.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) al        (1001)        1 2023-05-03 22:47:28.000000 yerbamate-0.9.235/packages/yerbamate.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) al        (1001)       82 2023-05-03 22:47:28.000000 yerbamate-0.9.235/packages/yerbamate.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) al        (1001)       10 2023-05-03 22:47:28.000000 yerbamate-0.9.235/packages/yerbamate.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) al        (1001)      107 2023-05-03 22:47:29.120415 yerbamate-0.9.235/setup.cfg
+-rw-r--r--   0 al        (1000) al        (1001)     1279 2023-05-03 22:47:18.000000 yerbamate-0.9.235/setup.py
+drwxr-xr-x   0 al        (1000) al        (1001)        0 2023-05-03 22:47:29.108415 yerbamate-0.9.235/src/
+-rwxr-xr-x   0 al        (1000) al        (1001)       62 2023-04-08 19:56:23.000000 yerbamate-0.9.235/src/mate
```

### Comparing `yerbamate-0.9.23/LICENSE` & `yerbamate-0.9.235/LICENSE`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/PKG-INFO` & `yerbamate-0.9.235/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: yerbamate
-Version: 0.9.23
+Version: 0.9.235
 Summary:  A python module and experiment manager for deep learning
 Home-page: https://github.com/oalee/yerbamate
 Author: Giulio Zani, Ali Rahimi
 Author-email: yerba.mate.dl@proton.me
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 style="color:green"><span style="color:green">Maté 🧉</span> your modular AI project and experiment manager</h1>
 
 <!-- Maté is a python project, package and experiment manager. Whether you are a
 seasoned deep learning researcher or just starting out, Maté provides you with
```

### Comparing `yerbamate-0.9.23/README.md` & `yerbamate-0.9.235/README.md`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/__pycache__/environment.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/__pycache__/environment.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr  9 09:45:16 2023 UTC, .py size: 5800 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2c89 3264 a816 0000  o.......,.2d....
+00000000: 6f0d 0d0a 0000 0000 3bcc 5264 e116 0000  o.......;.Rd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 5a05 4700 6403 6404  d.l.Z.d.Z.G.d.d.
 00000060: 8400 6404 6506 8303 5a07 6401 5300 2905  ..d.e...Z.d.S.).
 00000070: e900 0000 004e da03 656e 7663 0000 0000  .....N..envc....
@@ -10,268 +10,271 @@
 00000090: 0000 0000 7344 0000 0065 005a 0164 005a  ....sD...e.Z.d.Z
 000000a0: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
 000000b0: 0464 0564 0684 005a 0564 0764 0884 005a  .d.d...Z.d.d...Z
 000000c0: 0664 0964 0a84 005a 0787 0066 0164 0b64  .d.d...Z...f.d.d
 000000d0: 0c84 085a 0887 0004 005a 0953 0029 0dda  ...Z.....Z.S.)..
 000000e0: 0b45 6e76 6972 6f6e 6d65 6e74 6301 0000  .Environmentc...
 000000f0: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-00000100: 0043 0000 0073 2e01 0000 6401 7c00 5f00  .C...s....d.|._.
+00000100: 0043 0000 0073 3e01 0000 6401 7c00 5f00  .C...s>...d.|._.
 00000110: 6401 7c00 5f01 6401 7c00 5f02 6401 7c00  d.|._.d.|._.d.|.
 00000120: 5f03 6900 7c00 5f04 7a0b 7405 7c00 7406  _.i.|._.z.t.|.t.
 00000130: 6a07 6402 1900 6403 8303 0100 5700 6e04  j.d...d.....W.n.
-00000140: 0100 0100 0100 5900 7c00 a008 a100 7c00  ......Y.|.....|.
-00000150: 5f09 7406 6a07 4400 5d1e 7d01 6404 7c01  _.t.j.D.].}.d.|.
-00000160: 7601 722e 7127 7c01 a00a 6404 a101 5c02  v.r.q'|...d...\.
-00000170: 7d02 7d03 7c00 a00b 7c03 a101 7d03 7405  }.}.|...|...}.t.
-00000180: 7c00 7c02 7c03 8303 0100 7c03 7c00 6a04  |.|.|.....|.|.j.
-00000190: 7c02 3c00 7127 7406 6a07 6405 1900 7c00  |.<.q't.j.d...|.
-000001a0: 5f0c 6406 7c00 6a0c 7600 7271 740d 6a0e  _.d.|.j.v.rqt.j.
-000001b0: 6a0f 7406 6a07 6407 6408 8502 1900 8e00  j.t.j.d.d.......
-000001c0: 7c00 5f10 740d 6a0e a00f 7c00 6a09 6409  |._.t.j...|.j.d.
-000001d0: 7406 6a07 6407 1900 7406 6a07 640a 1900  t.j.d...t.j.d...
-000001e0: 640b 1700 a104 7c00 5f0c 6e17 7c00 6a0c  d.....|._.n.|.j.
-000001f0: a00a 640c a101 640d 6400 8502 1900 7c00  ..d...d.d.....|.
-00000200: 5f10 740d 6a0e 6a0f 7c00 6a10 8e00 6400  _.t.j.j.|.j...d.
-00000210: 640e 8502 1900 7c00 5f10 7c00 a011 a100  d.....|._.|.....
-00000220: 0100 7c00 6a02 7295 7c00 a012 a100 0100  ..|.j.r.|.......
-00000230: 6400 5300 6400 5300 290f 4e46 e901 0000  d.S.d.S.).NF....
-00000240: 0054 fa01 3d72 0100 0000 7a08 6269 6e2f  .T..=r....z.bin/
-00000250: 6d61 7465 e902 0000 00e9 0400 0000 5a0b  mate..........Z.
-00000260: 6578 7065 7269 6d65 6e74 73e9 0300 0000  experiments.....
-00000270: 7a03 2e70 79fa 012f e9fe ffff ffe9 fdff  z..py../........
-00000280: ffff 2913 5a07 7265 7374 6172 74da 0474  ..).Z.restart..t
-00000290: 6573 745a 0574 7261 696e da06 7361 6d70  estZ.train..samp
-000002a0: 6c65 da07 6870 6172 616d 73da 0773 6574  le..hparams..set
-000002b0: 6174 7472 da03 7379 73da 0461 7267 76da  attr..sys..argv.
-000002c0: 175f 456e 7669 726f 6e6d 656e 745f 5f66  ._Environment__f
-000002d0: 696e 645f 726f 6f74 da05 5f72 6f6f 74da  ind_root.._root.
-000002e0: 0573 706c 6974 da13 636f 6e76 6572 745f  .split..convert_
-000002f0: 7374 725f 746f 5f64 6174 61da 055f 7061  str_to_data.._pa
-00000300: 7468 da02 6f73 da04 7061 7468 da04 6a6f  th..os..path..jo
-00000310: 696e da04 6e61 6d65 da15 5f45 6e76 6972  in..name.._Envir
-00000320: 6f6e 6d65 6e74 5f5f 7365 745f 656e 76da  onment__set_env.
-00000330: 215f 456e 7669 726f 6e6d 656e 745f 5f67  !_Environment__g
-00000340: 656e 6572 6174 655f 6578 7065 7269 6d65  enerate_experime
-00000350: 6e74 2904 da04 7365 6c66 da03 6172 67da  nt)...self..arg.
-00000360: 036b 6579 da05 7661 6c75 65a9 0072 2100  .key..value..r!.
-00000370: 0000 fa3b 2f68 6f6d 652f 616c 2f47 6974  ...;/home/al/Git
-00000380: 4875 622f 7965 7262 616d 6174 652f 7061  Hub/yerbamate/pa
-00000390: 636b 6167 6573 2f79 6572 6261 6d61 7465  ckages/yerbamate
-000003a0: 2f65 6e76 6972 6f6e 6d65 6e74 2e70 79da  /environment.py.
-000003b0: 085f 5f69 6e69 745f 5f0e 0000 0073 3a00  .__init__....s:.
-000003c0: 0000 0603 0601 0601 0601 0601 0203 1601  ................
-000003d0: 0601 0201 0a02 0a03 0801 0201 0e01 0a01  ................
-000003e0: 0c01 0c01 0c02 0a01 1801 0601 1a01 08ff  ................
-000003f0: 1604 1801 0802 0602 0c01 04ff 7a14 456e  ............z.En
-00000400: 7669 726f 6e6d 656e 742e 5f5f 696e 6974  vironment.__init
-00000410: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
-00000420: 0000 000b 0000 0043 0000 0073 6000 0000  .......C...s`...
-00000430: 7a05 7400 7c01 8301 5700 5300 0400 7401  z.t.|...W.S...t.
-00000440: 792f 0100 0100 0100 7a07 7402 7c01 8301  y/......z.t.|...
-00000450: 5700 0600 5900 5300 0400 7401 792e 0100  W...Y.S...t.y...
-00000460: 0100 0100 7c01 6401 7600 7222 5900 5900  ....|.d.v.r"Y.Y.
-00000470: 6402 5300 7c01 6403 7600 722a 5900 5900  d.S.|.d.v.r*Y.Y.
-00000480: 6404 5300 5900 5900 7c01 5300 7700 7700  d.S.Y.Y.|.S.w.w.
-00000490: 2905 4e29 02da 0454 7275 65da 0474 7275  ).N)...True..tru
-000004a0: 6554 2902 da05 4661 6c73 65da 0566 616c  eT)...False..fal
-000004b0: 7365 4629 03da 0369 6e74 da0a 5661 6c75  seF)...int..Valu
-000004c0: 6545 7272 6f72 da05 666c 6f61 7429 0272  eError..float).r
-000004d0: 1d00 0000 da05 696e 7075 7472 2100 0000  ......inputr!...
-000004e0: 7221 0000 0072 2200 0000 7215 0000 0037  r!...r"...r....7
-000004f0: 0000 0073 1c00 0000 0201 0a01 0c01 0201  ...s............
-00000500: 0e01 0c01 0801 0801 0801 0801 04ff 0403  ................
-00000510: 02fa 02fd 7a1f 456e 7669 726f 6e6d 656e  ....z.Environmen
-00000520: 742e 636f 6e76 6572 745f 7374 725f 746f  t.convert_str_to
-00000530: 5f64 6174 6163 0100 0000 0000 0000 0000  _datac..........
-00000540: 0000 0300 0000 0700 0000 4300 0000 734e  ..........C...sN
-00000550: 0000 0074 00a0 01a1 007d 0174 006a 02a0  ...t.....}.t.j..
-00000560: 0374 006a 02a0 047c 0164 01a1 02a1 0172  .t.j...|.d.....r
-00000570: 2574 05a0 0674 0774 006a 02a0 047c 0164  %t...t.t.j...|.d
-00000580: 01a1 0264 0283 02a1 017d 0274 006a 02a0  ...d.....}.t.j..
-00000590: 047c 017c 0264 0319 00a1 0253 0064 0053  .|.|.d.....S.d.S
-000005a0: 0029 044e fa09 6d61 7465 2e6a 736f 6eda  .).N..mate.json.
-000005b0: 0172 da07 7072 6f6a 6563 7429 0872 1700  .r..project).r..
-000005c0: 0000 da06 6765 7463 7764 7218 0000 00da  ....getcwdr.....
-000005d0: 0665 7869 7374 7372 1900 0000 da04 6a73  .existsr......js
-000005e0: 6f6e da04 6c6f 6164 da04 6f70 656e 2903  on..load..open).
-000005f0: 721d 0000 0072 1800 0000 da04 636f 6e66  r....r......conf
-00000600: 7221 0000 0072 2100 0000 7222 0000 005a  r!...r!...r"...Z
-00000610: 0b5f 5f66 696e 645f 726f 6f74 4500 0000  .__find_rootE...
-00000620: 730a 0000 0008 0316 021a 0112 0204 027a  s..............z
-00000630: 1745 6e76 6972 6f6e 6d65 6e74 2e5f 5f66  .Environment.__f
-00000640: 696e 645f 726f 6f74 6301 0000 0000 0000  ind_rootc.......
-00000650: 0000 0000 0007 0000 0008 0000 0043 0000  .............C..
-00000660: 0073 ce00 0000 6700 6401 a201 7d01 6400  .s....g.d...}.d.
-00000670: 7d02 7c01 4400 5d0e 7d03 7c03 7c00 6a00  }.|.D.].}.|.|.j.
-00000680: 7600 7216 7c00 6a00 7c03 1900 7d02 0100  v.r.|.j.|...}...
-00000690: 6e01 7108 7c02 6400 7500 721d 6400 5300  n.q.|.d.u.r.d.S.
-000006a0: 7401 6a02 a003 7c02 a101 7328 7401 a004  t.j...|...s(t...
-000006b0: 7c02 a101 0100 7401 6a02 a005 7c02 6402  |.....t.j...|.d.
-000006c0: a102 7d04 7406 a007 7c00 6a08 7c04 a102  ..}.t...|.j.|...
-000006d0: 0100 7c00 6a09 6900 6b03 7265 7401 6a02  ..|.j.i.k.ret.j.
-000006e0: a005 7c02 6403 a102 7d05 740a 7c05 6404  ..|.d...}.t.|.d.
-000006f0: 8302 8f14 7d06 740b 6a0c 740d 7c00 6a09  ....}.t.j.t.|.j.
-00000700: 8301 7c06 6405 6406 8d03 0100 5700 6400  ..|.d.d.....W.d.
-00000710: 0400 0400 8303 0100 6400 5300 3100 735e  ........d.S.1.s^
-00000720: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
-00000730: 6400 5300 2907 4e29 06da 0772 6573 756c  d.S.).N)...resul
-00000740: 7473 5a0c 7265 7375 6c74 735f 7061 7468  tsZ.results_path
-00000750: 5a0b 7265 7375 6c74 735f 6469 72da 0473  Z.results_dir..s
-00000760: 6176 65da 0973 6176 655f 7061 7468 5a08  ave..save_pathZ.
-00000770: 7361 7665 5f64 6972 7a0d 6578 7065 7269  save_dirz.experi
-00000780: 6d65 6e74 2e70 797a 0f65 7870 6572 696d  ment.pyz.experim
-00000790: 656e 742e 6a73 6f6e da01 7772 0700 0000  ent.json..wr....
-000007a0: a901 da06 696e 6465 6e74 290e 7202 0000  ....indent).r...
-000007b0: 0072 1700 0000 7218 0000 0072 3000 0000  .r....r....r0...
-000007c0: da08 6d61 6b65 6469 7273 7219 0000 00da  ..makedirsr.....
-000007d0: 0673 6875 7469 6cda 0863 6f70 7966 696c  .shutil..copyfil
-000007e0: 6572 1600 0000 720e 0000 0072 3300 0000  er....r....r3...
-000007f0: 7231 0000 00da 0464 756d 70da 0464 6963  r1.....dump..dic
-00000800: 7429 0772 1d00 0000 7235 0000 00da 0672  t).r....r5.....r
-00000810: 6573 756c 7472 1f00 0000 5a09 7361 7665  esultr....Z.save
-00000820: 5f66 696c 655a 0b70 6172 616d 735f 6669  _fileZ.params_fi
-00000830: 6c65 da01 6672 2100 0000 7221 0000 0072  le..fr!...r!...r
-00000840: 2200 0000 5a15 5f5f 6765 6e65 7261 7465  "...Z.__generate
-00000850: 5f65 7870 6572 696d 656e 7451 0000 0073  _experimentQ...s
-00000860: 2600 0000 0802 0402 0801 0a01 0a01 0401  &...............
-00000870: 02fe 0803 0401 0c01 0a01 0e02 0e02 0a04  ................
-00000880: 0e01 0c03 1801 22ff 04fc 7a21 456e 7669  ......"...z!Envi
-00000890: 726f 6e6d 656e 742e 5f5f 6765 6e65 7261  ronment.__genera
-000008a0: 7465 5f65 7870 6572 696d 656e 7463 0100  te_experimentc..
-000008b0: 0000 0000 0000 0000 0000 0d00 0000 0900  ................
-000008c0: 0000 4300 0000 7360 0200 0074 006a 01a0  ..C...s`...t.j..
-000008d0: 0264 01a1 017d 0174 03a0 0474 057c 0164  .d...}.t...t.|.d
-000008e0: 0283 02a1 017d 0274 006a 01a0 0264 03a1  .....}.t.j...d..
-000008f0: 017d 0374 006a 01a0 067c 03a1 0173 5074  .}.t.j...|...sPt
-00000900: 0764 0483 0101 0074 087c 0276 0072 297c  .d.....t.|.v.r)|
-00000910: 0274 0819 00a0 09a1 007d 046e 0364 0567  .t.......}.n.d.g
-00000920: 017d 0464 0664 0784 007c 0444 0083 017d  .}.d.d...|.D...}
-00000930: 0574 057c 0364 0883 028f 107d 0674 036a  .t.|.d.....}.t.j
-00000940: 0a7c 057c 0664 0964 0a8d 0301 0057 0064  .|.|.d.d.....W.d
-00000950: 0004 0004 0083 0301 006e 0831 0073 4b77  .........n.1.sKw
-00000960: 0101 0001 0001 0059 0001 0074 057c 0364  .......Y...t.|.d
-00000970: 0283 028f 1f7d 067a 0774 03a0 047c 06a1  .....}.z.t...|..
-00000980: 017d 0757 006e 0f04 0074 036a 0b6a 0c79  .}.W.n...t.j.j.y
-00000990: 6c01 0001 0001 0064 0564 0b69 017d 0759  l......d.d.i.}.Y
-000009a0: 006e 0177 0057 0064 0004 0004 0083 0301  .n.w.W.d........
-000009b0: 006e 0831 0073 7777 0101 0001 0001 0059  .n.1.sww.......Y
-000009c0: 0001 0067 007d 0874 087c 0276 0072 a77c  ...g.}.t.|.v.r.|
-000009d0: 07a0 0da1 0044 005d 205c 027d 097d 0a7c  .....D.] \.}.}.|
-000009e0: 077c 0919 0064 0b6b 0272 a67c 0974 006a  .|...d.k.r.|.t.j
-000009f0: 0e76 0072 9d74 006a 0e7c 0919 007c 077c  .v.r.t.j.|...|.|
-00000a00: 093c 0071 867c 08a0 0f7c 09a1 0101 007c  .<.q.|...|.....|
-00000a10: 0a7c 077c 093c 0071 8674 107c 0883 0164  .|.|.<.q.t.|...d
-00000a20: 0c6b 0472 d674 0764 0d83 0101 007c 0844  .k.r.t.d.....|.D
-00000a30: 005d 197d 097c 097c 0274 0819 0076 0072  .].}.|.|.t...v.r
-00000a40: c17c 0274 0819 007c 0919 006e 0164 0e7d  .|.t...|...n.d.}
-00000a50: 0b74 077c 099b 0064 0f7c 0b9b 009d 0383  .t.|...d.|......
-00000a60: 0101 0071 b374 0764 1083 0101 0074 11a0  ...q.t.d.....t..
-00000a70: 1264 11a1 0101 0064 1267 017d 0c7c 0c44  .d.....d.g.}.|.D
-00000a80: 005d 387d 097c 097c 0776 0072 f574 006a  .]8}.|.|.v.r.t.j
-00000a90: 016a 027c 077c 0919 0067 017c 006a 13a0  .j.|.|...g.|.j..
-00000aa0: 1464 13a1 01a2 0152 008e 007c 077c 093c  .d.....R...|.|.<
-00000ab0: 0001 006e 1f74 006a 0ea0 157c 0964 00a1  ...n.t.j...|.d..
-00000ac0: 0264 0075 0190 0172 1374 006a 0ea0 157c  .d.u...r.t.j...|
-00000ad0: 0964 00a1 0264 0b6b 0390 0172 1374 006a  .d...d.k...r.t.j
-00000ae0: 0ea0 157c 09a1 017c 077c 093c 0001 006e  ...|...|.|.<...n
-00000af0: 0171 db74 107c 0783 0164 0c6b 0290 0172  .q.t.|...d.k...r
-00000b00: 2874 0764 1483 0101 0074 0764 1083 0101  (t.d.....t.d....
-00000b10: 0074 11a0 1264 11a1 0101 0074 167c 0064  .t...d.....t.|.d
-00000b20: 157c 0783 0301 0064 0053 0029 164e 722c  .|.....d.S.).Nr,
-00000b30: 0000 0072 2d00 0000 7a08 656e 762e 6a73  ...r-...z.env.js
-00000b40: 6f6e 7a40 456e 7669 726f 6e6d 656e 7420  onz@Environment 
-00000b50: 6669 6c65 206e 6f74 2066 6f75 6e64 2c20  file not found, 
-00000b60: 6372 6561 7469 6e67 206f 6e65 2077 6974  creating one wit
-00000b70: 6820 6465 6661 756c 7473 3a20 656e 762e  h defaults: env.
-00000b80: 6a73 6f6e 7235 0000 0063 0100 0000 0000  jsonr5...c......
-00000b90: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00000ba0: 0000 7312 0000 0069 007c 005d 057d 017c  ..s....i.|.].}.|
-00000bb0: 0164 0093 0271 0253 0029 01da 0072 2100  .d...q.S.)...r!.
-00000bc0: 0000 2902 da02 2e30 721f 0000 0072 2100  ..)....0r....r!.
-00000bd0: 0000 7221 0000 0072 2200 0000 da0a 3c64  ..r!...r".....<d
-00000be0: 6963 7463 6f6d 703e 7900 0000 7302 0000  ictcomp>y...s...
-00000bf0: 0012 007a 2945 6e76 6972 6f6e 6d65 6e74  ...z)Environment
-00000c00: 2e5f 5f73 6574 5f65 6e76 2e3c 6c6f 6361  .__set_env.<loca
-00000c10: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7238  ls>.<dictcomp>r8
-00000c20: 0000 0072 0700 0000 7239 0000 0072 4200  ...r....r9...rB.
-00000c30: 0000 7201 0000 007a 4745 6e76 6972 6f6e  ..r....zGEnviron
-00000c40: 6d65 6e74 2076 6172 6961 626c 6573 206e  ment variables n
-00000c50: 6f74 2066 6f75 6e64 2e20 5365 7420 7468  ot found. Set th
-00000c60: 656d 2069 6e20 656e 762e 6a73 6f6e 206f  em in env.json o
-00000c70: 7220 696e 2079 6f75 7220 7368 656c 6c2e  r in your shell.
-00000c80: 7a1d 5265 7175 6972 6564 2065 6e76 6972  z.Required envir
-00000c90: 6f6e 6d65 6e74 2076 6172 6961 626c 657a  onment variablez
-00000ca0: 0320 3a20 fa0a 4578 6974 696e 672e 2e2e  . : ..Exiting...
-00000cb0: 7204 0000 005a 0961 7574 6f5f 7361 7665  r....Z.auto_save
-00000cc0: 7209 0000 007a 5972 6573 756c 7473 2f73  r....zYresults/s
-00000cd0: 6176 655f 6469 722f 7361 7665 2065 6e76  ave_dir/save env
-00000ce0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00000cf0: 6520 6973 2065 6d70 7479 2e20 5365 7420  e is empty. Set 
-00000d00: 6974 2069 6e20 656e 762e 6a73 6f6e 206f  it in env.json o
-00000d10: 7220 696e 2079 6f75 7220 7368 656c 6c2e  r in your shell.
-00000d20: 7202 0000 0029 1772 1700 0000 7218 0000  r....).r....r...
-00000d30: 0072 1900 0000 7231 0000 0072 3200 0000  .r....r1...r2...
-00000d40: 7233 0000 0072 3000 0000 da05 7072 696e  r3...r0.....prin
-00000d50: 74da 0745 4e56 5f4b 4559 da04 6b65 7973  t..ENV_KEY..keys
-00000d60: 723e 0000 00da 0764 6563 6f64 6572 da0f  r>.....decoder..
-00000d70: 4a53 4f4e 4465 636f 6465 4572 726f 72da  JSONDecodeError.
-00000d80: 0569 7465 6d73 da07 656e 7669 726f 6eda  .items..environ.
-00000d90: 0661 7070 656e 64da 036c 656e 7210 0000  .append..lenr...
-00000da0: 00da 0465 7869 7472 1a00 0000 7214 0000  ...exitr....r...
-00000db0: 00da 0367 6574 720f 0000 0029 0d72 1d00  ...getr....).r..
-00000dc0: 0000 5a0e 6d61 7465 5f63 6f6e 665f 7061  ..Z.mate_conf_pa
-00000dd0: 7468 7234 0000 005a 0865 6e76 5f70 6174  thr4...Z.env_pat
-00000de0: 68da 0d72 6571 7569 7265 645f 6b65 7973  h..required_keys
-00000df0: 5a0b 6465 6675 616c 745f 656e 7672 4100  Z.defualt_envrA.
-00000e00: 0000 7202 0000 005a 0d65 6e76 5f6e 6f74  ..r....Z.env_not
-00000e10: 5f66 6f75 6e64 721f 0000 0072 2000 0000  _foundr....r ...
-00000e20: da04 6465 7363 5a0e 7365 6172 6368 5f72  ..descZ.search_r
-00000e30: 6573 756c 7473 7221 0000 0072 2100 0000  esultsr!...r!...
-00000e40: 7222 0000 005a 095f 5f73 6574 5f65 6e76  r"...Z.__set_env
-00000e50: 6c00 0000 736e 0000 000c 0110 010c 020c  l...sn..........
-00000e60: 0108 0108 020e 0106 020e 020c 0212 011c  ................
-00000e70: ff0c 0302 010e 0110 0104 0208 ff02 ff02  ................
-00000e80: 801c fd04 0808 0210 010c 010a 0110 010a  ................
-00000e90: 0308 0102 800c 0202 0102 0104 ff08 021c  ................
-00000ea0: 0114 0108 020a 0106 0308 0108 0124 0104  .............$..
-00000eb0: 0228 0110 0104 0202 800e 0202 0102 0104  .(..............
-00000ec0: ff08 020a 0110 027a 1545 6e76 6972 6f6e  .......z.Environ
-00000ed0: 6d65 6e74 2e5f 5f73 6574 5f65 6e76 6302  ment.__set_envc.
-00000ee0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000ef0: 0000 0003 0000 0073 6e00 0000 7c01 7c00  .......sn...|.|.
-00000f00: 7601 7231 7c01 7c00 6a00 7600 720e 7c00  v.r1|.|.j.v.r.|.
-00000f10: 6a00 7c01 1900 5300 7401 6a02 a003 7c01  j.|...S.t.j...|.
-00000f20: 6400 a102 7d02 7c02 6400 7500 731d 7c02  d...}.|.d.u.s.|.
-00000f30: 6401 6b02 722f 7404 6402 7c01 9b00 6403  d.k.r/t.d.|...d.
-00000f40: 9d03 8301 0100 7404 6404 8301 0100 7405  ......t.d.....t.
-00000f50: a006 6405 a101 0100 6e02 7c02 5300 7407  ..d.....n.|.S.t.
-00000f60: 8300 a008 7c01 a101 5300 2906 4e72 4200  ....|...S.).NrB.
-00000f70: 0000 7a15 456e 7669 726f 6e6d 656e 7420  ..z.Environment 
-00000f80: 7661 7269 6162 6c65 207a 3020 6e6f 7420  variable z0 not 
-00000f90: 666f 756e 642e 2053 6574 2069 7420 696e  found. Set it in
-00000fa0: 2065 6e76 2e6a 736f 6e20 6f72 2069 6e20   env.json or in 
-00000fb0: 796f 7572 2073 6865 6c6c 2e72 4500 0000  your shell.rE...
-00000fc0: 7204 0000 0029 0972 0200 0000 7217 0000  r....).r....r...
-00000fd0: 0072 4c00 0000 7250 0000 0072 4600 0000  .rL...rP...rF...
-00000fe0: 7210 0000 0072 4f00 0000 da05 7375 7065  r....rO.....supe
-00000ff0: 72da 0b5f 5f67 6574 6974 656d 5f5f 2903  r..__getitem__).
-00001000: 721d 0000 0072 1f00 0000 da03 7265 73a9  r....r......res.
-00001010: 01da 095f 5f63 6c61 7373 5f5f 7221 0000  ...__class__r!..
-00001020: 0072 2200 0000 7254 0000 00b0 0000 0073  .r"...rT.......s
-00001030: 1800 0000 0801 0a02 0a01 0e01 1002 0201  ................
-00001040: 0a01 04ff 0802 0c01 0402 0c02 7a17 456e  ............z.En
-00001050: 7669 726f 6e6d 656e 742e 5f5f 6765 7469  vironment.__geti
-00001060: 7465 6d5f 5f29 0ada 085f 5f6e 616d 655f  tem__)...__name_
-00001070: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00001080: 5f71 7561 6c6e 616d 655f 5f72 2300 0000  _qualname__r#...
-00001090: 7215 0000 0072 1200 0000 721c 0000 0072  r....r....r....r
-000010a0: 1b00 0000 7254 0000 00da 0d5f 5f63 6c61  ....rT.....__cla
-000010b0: 7373 6365 6c6c 5f5f 7221 0000 0072 2100  sscell__r!...r!.
-000010c0: 0000 7256 0000 0072 2200 0000 7203 0000  ..rV...r"...r...
-000010d0: 000c 0000 0073 0e00 0000 0800 0802 0829  .....s.........)
-000010e0: 080e 080c 081b 1444 7203 0000 0029 0872  .......Dr....).r
-000010f0: 3100 0000 7217 0000 0072 3c00 0000 7210  1...r....r<...r.
-00001100: 0000 00da 0469 7064 6272 4700 0000 723f  .....ipdbrG...r?
-00001110: 0000 0072 0300 0000 7221 0000 0072 2100  ...r....r!...r!.
-00001120: 0000 7221 0000 0072 2200 0000 da08 3c6d  ..r!...r".....<m
-00001130: 6f64 756c 653e 0100 0000 730e 0000 0008  odule>....s.....
-00001140: 0108 0108 0108 0108 0104 0314 03         .............
+00000140: 0100 0100 0100 5900 7406 6a07 6402 6400  ......Y.t.j.d.d.
+00000150: 8502 1900 7c00 5f08 7c00 a009 a100 7c00  ....|._.|.....|.
+00000160: 5f0a 7406 6a07 4400 5d1e 7d01 6404 7c01  _.t.j.D.].}.d.|.
+00000170: 7601 7236 712f 7c01 a00b 6404 a101 5c02  v.r6q/|...d...\.
+00000180: 7d02 7d03 7c00 a00c 7c03 a101 7d03 7405  }.}.|...|...}.t.
+00000190: 7c00 7c02 7c03 8303 0100 7c03 7c00 6a04  |.|.|.....|.|.j.
+000001a0: 7c02 3c00 712f 7406 6a07 6405 1900 7c00  |.<.q/t.j.d...|.
+000001b0: 5f0d 6406 7c00 6a0d 7600 7279 740e 6a0f  _.d.|.j.v.ryt.j.
+000001c0: 6a10 7406 6a07 6407 6408 8502 1900 8e00  j.t.j.d.d.......
+000001d0: 7c00 5f11 740e 6a0f a010 7c00 6a0a 6409  |._.t.j...|.j.d.
+000001e0: 7406 6a07 6407 1900 7406 6a07 640a 1900  t.j.d...t.j.d...
+000001f0: 640b 1700 a104 7c00 5f0d 6e17 7c00 6a0d  d.....|._.n.|.j.
+00000200: a00b 640c a101 640d 6400 8502 1900 7c00  ..d...d.d.....|.
+00000210: 5f11 740e 6a0f 6a10 7c00 6a11 8e00 6400  _.t.j.j.|.j...d.
+00000220: 640e 8502 1900 7c00 5f11 7c00 a012 a100  d.....|._.|.....
+00000230: 0100 7c00 6a02 729d 7c00 a013 a100 0100  ..|.j.r.|.......
+00000240: 6400 5300 6400 5300 290f 4e46 e901 0000  d.S.d.S.).NF....
+00000250: 0054 fa01 3d72 0100 0000 7a08 6269 6e2f  .T..=r....z.bin/
+00000260: 6d61 7465 e902 0000 00e9 0400 0000 5a0b  mate..........Z.
+00000270: 6578 7065 7269 6d65 6e74 73e9 0300 0000  experiments.....
+00000280: 7a03 2e70 79fa 012f e9fe ffff ffe9 fdff  z..py../........
+00000290: ffff 2914 5a07 7265 7374 6172 74da 0474  ..).Z.restart..t
+000002a0: 6573 745a 0574 7261 696e da06 7361 6d70  estZ.train..samp
+000002b0: 6c65 da07 6870 6172 616d 73da 0773 6574  le..hparams..set
+000002c0: 6174 7472 da03 7379 73da 0461 7267 76da  attr..sys..argv.
+000002d0: 0461 7267 73da 175f 456e 7669 726f 6e6d  .args.._Environm
+000002e0: 656e 745f 5f66 696e 645f 726f 6f74 da05  ent__find_root..
+000002f0: 5f72 6f6f 74da 0573 706c 6974 da13 636f  _root..split..co
+00000300: 6e76 6572 745f 7374 725f 746f 5f64 6174  nvert_str_to_dat
+00000310: 61da 055f 7061 7468 da02 6f73 da04 7061  a.._path..os..pa
+00000320: 7468 da04 6a6f 696e da04 6e61 6d65 da15  th..join..name..
+00000330: 5f45 6e76 6972 6f6e 6d65 6e74 5f5f 7365  _Environment__se
+00000340: 745f 656e 76da 215f 456e 7669 726f 6e6d  t_env.!_Environm
+00000350: 656e 745f 5f67 656e 6572 6174 655f 6578  ent__generate_ex
+00000360: 7065 7269 6d65 6e74 2904 da04 7365 6c66  periment)...self
+00000370: da03 6172 67da 036b 6579 da05 7661 6c75  ..arg..key..valu
+00000380: 65a9 0072 2200 0000 fa3b 2f68 6f6d 652f  e..r"....;/home/
+00000390: 616c 2f47 6974 4875 622f 7965 7262 616d  al/GitHub/yerbam
+000003a0: 6174 652f 7061 636b 6167 6573 2f79 6572  ate/packages/yer
+000003b0: 6261 6d61 7465 2f65 6e76 6972 6f6e 6d65  bamate/environme
+000003c0: 6e74 2e70 79da 085f 5f69 6e69 745f 5f0e  nt.py..__init__.
+000003d0: 0000 0073 3c00 0000 0603 0601 0601 0601  ...s<...........
+000003e0: 0601 0203 1601 0601 0201 1002 0a02 0a03  ................
+000003f0: 0801 0201 0e01 0a01 0c01 0c01 0c02 0a01  ................
+00000400: 1801 0601 1a01 08ff 1604 1801 0802 0602  ................
+00000410: 0c01 04ff 7a14 456e 7669 726f 6e6d 656e  ....z.Environmen
+00000420: 742e 5f5f 696e 6974 5f5f 6302 0000 0000  t.__init__c.....
+00000430: 0000 0000 0000 0002 0000 000b 0000 0043  ...............C
+00000440: 0000 0073 6000 0000 7a05 7400 7c01 8301  ...s`...z.t.|...
+00000450: 5700 5300 0400 7401 792f 0100 0100 0100  W.S...t.y/......
+00000460: 7a07 7402 7c01 8301 5700 0600 5900 5300  z.t.|...W...Y.S.
+00000470: 0400 7401 792e 0100 0100 0100 7c01 6401  ..t.y.......|.d.
+00000480: 7600 7222 5900 5900 6402 5300 7c01 6403  v.r"Y.Y.d.S.|.d.
+00000490: 7600 722a 5900 5900 6404 5300 5900 5900  v.r*Y.Y.d.S.Y.Y.
+000004a0: 7c01 5300 7700 7700 2905 4e29 02da 0454  |.S.w.w.).N)...T
+000004b0: 7275 65da 0474 7275 6554 2902 da05 4661  rue..trueT)...Fa
+000004c0: 6c73 65da 0566 616c 7365 4629 03da 0369  lse..falseF)...i
+000004d0: 6e74 da0a 5661 6c75 6545 7272 6f72 da05  nt..ValueError..
+000004e0: 666c 6f61 7429 0272 1e00 0000 da05 696e  float).r......in
+000004f0: 7075 7472 2200 0000 7222 0000 0072 2300  putr"...r"...r#.
+00000500: 0000 7216 0000 0039 0000 0073 1c00 0000  ..r....9...s....
+00000510: 0201 0a01 0c01 0201 0e01 0c01 0801 0801  ................
+00000520: 0801 0801 04ff 0403 02fa 02fd 7a1f 456e  ............z.En
+00000530: 7669 726f 6e6d 656e 742e 636f 6e76 6572  vironment.conver
+00000540: 745f 7374 725f 746f 5f64 6174 6163 0100  t_str_to_datac..
+00000550: 0000 0000 0000 0000 0000 0300 0000 0700  ................
+00000560: 0000 4300 0000 734e 0000 0074 00a0 01a1  ..C...sN...t....
+00000570: 007d 0174 006a 02a0 0374 006a 02a0 047c  .}.t.j...t.j...|
+00000580: 0164 01a1 02a1 0172 2574 05a0 0674 0774  .d.....r%t...t.t
+00000590: 006a 02a0 047c 0164 01a1 0264 0283 02a1  .j...|.d...d....
+000005a0: 017d 0274 006a 02a0 047c 017c 0264 0319  .}.t.j...|.|.d..
+000005b0: 00a1 0253 0064 0053 0029 044e fa09 6d61  ...S.d.S.).N..ma
+000005c0: 7465 2e6a 736f 6eda 0172 da07 7072 6f6a  te.json..r..proj
+000005d0: 6563 7429 0872 1800 0000 da06 6765 7463  ect).r......getc
+000005e0: 7764 7219 0000 00da 0665 7869 7374 7372  wdr......existsr
+000005f0: 1a00 0000 da04 6a73 6f6e da04 6c6f 6164  ......json..load
+00000600: da04 6f70 656e 2903 721e 0000 0072 1900  ..open).r....r..
+00000610: 0000 da04 636f 6e66 7222 0000 0072 2200  ....confr"...r".
+00000620: 0000 7223 0000 005a 0b5f 5f66 696e 645f  ..r#...Z.__find_
+00000630: 726f 6f74 4700 0000 730a 0000 0008 0316  rootG...s.......
+00000640: 021a 0112 0204 027a 1745 6e76 6972 6f6e  .......z.Environ
+00000650: 6d65 6e74 2e5f 5f66 696e 645f 726f 6f74  ment.__find_root
+00000660: 6301 0000 0000 0000 0000 0000 0007 0000  c...............
+00000670: 0008 0000 0043 0000 0073 d200 0000 6700  .....C...s....g.
+00000680: 6401 a201 7d01 6400 7d02 7c01 4400 5d0e  d...}.d.}.|.D.].
+00000690: 7d03 7c03 7c00 6a00 7600 7216 7c00 6a00  }.|.|.j.v.r.|.j.
+000006a0: 7c03 1900 7d02 0100 6e01 7108 7c02 6400  |...}...n.q.|.d.
+000006b0: 7500 721d 6400 5300 7401 6a02 a003 7c02  u.r.d.S.t.j...|.
+000006c0: a101 732a 7401 6a04 7c02 6402 6403 8d02  ..s*t.j.|.d.d...
+000006d0: 0100 7401 6a02 a005 7c02 6404 a102 7d04  ..t.j...|.d...}.
+000006e0: 7406 a007 7c00 6a08 7c04 a102 0100 7c00  t...|.j.|.....|.
+000006f0: 6a09 6900 6b03 7267 7401 6a02 a005 7c02  j.i.k.rgt.j...|.
+00000700: 6405 a102 7d05 740a 7c05 6406 8302 8f14  d...}.t.|.d.....
+00000710: 7d06 740b 6a0c 740d 7c00 6a09 8301 7c06  }.t.j.t.|.j...|.
+00000720: 6407 6408 8d03 0100 5700 6400 0400 0400  d.d.....W.d.....
+00000730: 8303 0100 6400 5300 3100 7360 7701 0100  ....d.S.1.s`w...
+00000740: 0100 0100 5900 0100 6400 5300 6400 5300  ....Y...d.S.d.S.
+00000750: 2909 4e29 06da 0772 6573 756c 7473 5a0c  ).N)...resultsZ.
+00000760: 7265 7375 6c74 735f 7061 7468 5a0b 7265  results_pathZ.re
+00000770: 7375 6c74 735f 6469 725a 0473 6176 655a  sults_dirZ.saveZ
+00000780: 0973 6176 655f 7061 7468 5a08 7361 7665  .save_pathZ.save
+00000790: 5f64 6972 5429 01da 0865 7869 7374 5f6f  _dirT)...exist_o
+000007a0: 6b7a 0d65 7870 6572 696d 656e 742e 7079  kz.experiment.py
+000007b0: 7a0f 6578 7065 7269 6d65 6e74 2e6a 736f  z.experiment.jso
+000007c0: 6eda 0177 7207 0000 00a9 01da 0669 6e64  n..wr........ind
+000007d0: 656e 7429 0e72 0200 0000 7218 0000 0072  ent).r....r....r
+000007e0: 1900 0000 7231 0000 00da 086d 616b 6564  ....r1.....maked
+000007f0: 6972 7372 1a00 0000 da06 7368 7574 696c  irsr......shutil
+00000800: da08 636f 7079 6669 6c65 7217 0000 0072  ..copyfiler....r
+00000810: 0e00 0000 7234 0000 0072 3200 0000 da04  ....r4...r2.....
+00000820: 6475 6d70 da04 6469 6374 2907 721e 0000  dump..dict).r...
+00000830: 0072 3600 0000 da06 7265 7375 6c74 7220  .r6.....resultr 
+00000840: 0000 005a 0973 6176 655f 6669 6c65 5a0b  ...Z.save_fileZ.
+00000850: 7061 7261 6d73 5f66 696c 65da 0166 7222  params_file..fr"
+00000860: 0000 0072 2200 0000 7223 0000 005a 155f  ...r"...r#...Z._
+00000870: 5f67 656e 6572 6174 655f 6578 7065 7269  _generate_experi
+00000880: 6d65 6e74 5300 0000 7326 0000 0008 0204  mentS...s&......
+00000890: 0208 010a 010a 0104 0102 fe08 0304 010c  ................
+000008a0: 010e 010e 020e 020a 040e 010c 0318 0122  ..............."
+000008b0: ff04 fc7a 2145 6e76 6972 6f6e 6d65 6e74  ...z!Environment
+000008c0: 2e5f 5f67 656e 6572 6174 655f 6578 7065  .__generate_expe
+000008d0: 7269 6d65 6e74 6301 0000 0000 0000 0000  rimentc.........
+000008e0: 0000 000d 0000 0009 0000 0043 0000 0073  ...........C...s
+000008f0: 6002 0000 7400 6a01 a002 6401 a101 7d01  `...t.j...d...}.
+00000900: 7403 a004 7405 7c01 6402 8302 a101 7d02  t...t.|.d.....}.
+00000910: 7400 6a01 a002 6403 a101 7d03 7400 6a01  t.j...d...}.t.j.
+00000920: a006 7c03 a101 7350 7407 6404 8301 0100  ..|...sPt.d.....
+00000930: 7408 7c02 7600 7229 7c02 7408 1900 a009  t.|.v.r)|.t.....
+00000940: a100 7d04 6e03 6405 6701 7d04 6406 6407  ..}.n.d.g.}.d.d.
+00000950: 8400 7c04 4400 8301 7d05 7405 7c03 6408  ..|.D...}.t.|.d.
+00000960: 8302 8f10 7d06 7403 6a0a 7c05 7c06 6409  ....}.t.j.|.|.d.
+00000970: 640a 8d03 0100 5700 6400 0400 0400 8303  d.....W.d.......
+00000980: 0100 6e08 3100 734b 7701 0100 0100 0100  ..n.1.sKw.......
+00000990: 5900 0100 7405 7c03 6402 8302 8f1f 7d06  Y...t.|.d.....}.
+000009a0: 7a07 7403 a004 7c06 a101 7d07 5700 6e0f  z.t...|...}.W.n.
+000009b0: 0400 7403 6a0b 6a0c 796c 0100 0100 0100  ..t.j.j.yl......
+000009c0: 6405 640b 6901 7d07 5900 6e01 7700 5700  d.d.i.}.Y.n.w.W.
+000009d0: 6400 0400 0400 8303 0100 6e08 3100 7377  d.........n.1.sw
+000009e0: 7701 0100 0100 0100 5900 0100 6700 7d08  w.......Y...g.}.
+000009f0: 7408 7c02 7600 72a7 7c07 a00d a100 4400  t.|.v.r.|.....D.
+00000a00: 5d20 5c02 7d09 7d0a 7c07 7c09 1900 640b  ] \.}.}.|.|...d.
+00000a10: 6b02 72a6 7c09 7400 6a0e 7600 729d 7400  k.r.|.t.j.v.r.t.
+00000a20: 6a0e 7c09 1900 7c07 7c09 3c00 7186 7c08  j.|...|.|.<.q.|.
+00000a30: a00f 7c09 a101 0100 7c0a 7c07 7c09 3c00  ..|.....|.|.|.<.
+00000a40: 7186 7410 7c08 8301 640c 6b04 72d6 7407  q.t.|...d.k.r.t.
+00000a50: 640d 8301 0100 7c08 4400 5d19 7d09 7c09  d.....|.D.].}.|.
+00000a60: 7c02 7408 1900 7600 72c1 7c02 7408 1900  |.t...v.r.|.t...
+00000a70: 7c09 1900 6e01 640e 7d0b 7407 7c09 9b00  |...n.d.}.t.|...
+00000a80: 640f 7c0b 9b00 9d03 8301 0100 71b3 7407  d.|.........q.t.
+00000a90: 6410 8301 0100 7411 a012 6411 a101 0100  d.....t...d.....
+00000aa0: 6412 6701 7d0c 7c0c 4400 5d38 7d09 7c09  d.g.}.|.D.]8}.|.
+00000ab0: 7c07 7600 72f5 7400 6a01 6a02 7c07 7c09  |.v.r.t.j.j.|.|.
+00000ac0: 1900 6701 7c00 6a13 a014 6413 a101 a201  ..g.|.j...d.....
+00000ad0: 5200 8e00 7c07 7c09 3c00 0100 6e1f 7400  R...|.|.<...n.t.
+00000ae0: 6a0e a015 7c09 6400 a102 6400 7501 9001  j...|.d...d.u...
+00000af0: 7213 7400 6a0e a015 7c09 6400 a102 640b  r.t.j...|.d...d.
+00000b00: 6b03 9001 7213 7400 6a0e a015 7c09 a101  k...r.t.j...|...
+00000b10: 7c07 7c09 3c00 0100 6e01 71db 7410 7c07  |.|.<...n.q.t.|.
+00000b20: 8301 640c 6b02 9001 7228 7407 6414 8301  ..d.k...r(t.d...
+00000b30: 0100 7407 6410 8301 0100 7411 a012 6411  ..t.d.....t...d.
+00000b40: a101 0100 7416 7c00 6415 7c07 8303 0100  ....t.|.d.|.....
+00000b50: 6400 5300 2916 4e72 2d00 0000 722e 0000  d.S.).Nr-...r...
+00000b60: 007a 0865 6e76 2e6a 736f 6e7a 4045 6e76  .z.env.jsonz@Env
+00000b70: 6972 6f6e 6d65 6e74 2066 696c 6520 6e6f  ironment file no
+00000b80: 7420 666f 756e 642c 2063 7265 6174 696e  t found, creatin
+00000b90: 6720 6f6e 6520 7769 7468 2064 6566 6175  g one with defau
+00000ba0: 6c74 733a 2065 6e76 2e6a 736f 6e72 3600  lts: env.jsonr6.
+00000bb0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00000bc0: 0000 0004 0000 0053 0000 0073 1200 0000  .......S...s....
+00000bd0: 6900 7c00 5d05 7d01 7c01 6400 9302 7102  i.|.].}.|.d...q.
+00000be0: 5300 2901 da00 7222 0000 0029 02da 022e  S.)...r"...)....
+00000bf0: 3072 2000 0000 7222 0000 0072 2200 0000  0r ...r"...r"...
+00000c00: 7223 0000 00da 0a3c 6469 6374 636f 6d70  r#.....<dictcomp
+00000c10: 3e7b 0000 0073 0200 0000 1200 7a29 456e  >{...s......z)En
+00000c20: 7669 726f 6e6d 656e 742e 5f5f 7365 745f  vironment.__set_
+00000c30: 656e 762e 3c6c 6f63 616c 733e 2e3c 6469  env.<locals>.<di
+00000c40: 6374 636f 6d70 3e72 3800 0000 7207 0000  ctcomp>r8...r...
+00000c50: 0072 3900 0000 7242 0000 0072 0100 0000  .r9...rB...r....
+00000c60: 7a47 456e 7669 726f 6e6d 656e 7420 7661  zGEnvironment va
+00000c70: 7269 6162 6c65 7320 6e6f 7420 666f 756e  riables not foun
+00000c80: 642e 2053 6574 2074 6865 6d20 696e 2065  d. Set them in e
+00000c90: 6e76 2e6a 736f 6e20 6f72 2069 6e20 796f  nv.json or in yo
+00000ca0: 7572 2073 6865 6c6c 2e7a 1d52 6571 7569  ur shell.z.Requi
+00000cb0: 7265 6420 656e 7669 726f 6e6d 656e 7420  red environment 
+00000cc0: 7661 7269 6162 6c65 7a03 203a 20fa 0a45  variablez. : ..E
+00000cd0: 7869 7469 6e67 2e2e 2e72 0400 0000 5a09  xiting...r....Z.
+00000ce0: 6175 746f 5f73 6176 6572 0900 0000 7a59  auto_saver....zY
+00000cf0: 7265 7375 6c74 732f 7361 7665 5f64 6972  results/save_dir
+00000d00: 2f73 6176 6520 656e 7669 726f 6e6d 656e  /save environmen
+00000d10: 7420 7661 7269 6162 6c65 2069 7320 656d  t variable is em
+00000d20: 7074 792e 2053 6574 2069 7420 696e 2065  pty. Set it in e
+00000d30: 6e76 2e6a 736f 6e20 6f72 2069 6e20 796f  nv.json or in yo
+00000d40: 7572 2073 6865 6c6c 2e72 0200 0000 2917  ur shell.r....).
+00000d50: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00000d60: 3200 0000 7233 0000 0072 3400 0000 7231  2...r3...r4...r1
+00000d70: 0000 00da 0570 7269 6e74 da07 454e 565f  .....print..ENV_
+00000d80: 4b45 59da 046b 6579 7372 3e00 0000 da07  KEY..keysr>.....
+00000d90: 6465 636f 6465 725a 0f4a 534f 4e44 6563  decoderZ.JSONDec
+00000da0: 6f64 6545 7272 6f72 da05 6974 656d 73da  odeError..items.
+00000db0: 0765 6e76 6972 6f6e da06 6170 7065 6e64  .environ..append
+00000dc0: da03 6c65 6e72 1000 0000 da04 6578 6974  ..lenr......exit
+00000dd0: 721b 0000 0072 1500 0000 da03 6765 7472  r....r......getr
+00000de0: 0f00 0000 290d 721e 0000 005a 0e6d 6174  ....).r....Z.mat
+00000df0: 655f 636f 6e66 5f70 6174 6872 3500 0000  e_conf_pathr5...
+00000e00: 5a08 656e 765f 7061 7468 da0d 7265 7175  Z.env_path..requ
+00000e10: 6972 6564 5f6b 6579 735a 0b64 6566 7561  ired_keysZ.defua
+00000e20: 6c74 5f65 6e76 7241 0000 0072 0200 0000  lt_envrA...r....
+00000e30: 5a0d 656e 765f 6e6f 745f 666f 756e 6472  Z.env_not_foundr
+00000e40: 2000 0000 7221 0000 005a 0464 6573 635a   ...r!...Z.descZ
+00000e50: 0e73 6561 7263 685f 7265 7375 6c74 7372  .search_resultsr
+00000e60: 2200 0000 7222 0000 0072 2300 0000 5a09  "...r"...r#...Z.
+00000e70: 5f5f 7365 745f 656e 766e 0000 0073 6e00  __set_envn...sn.
+00000e80: 0000 0c01 1001 0c02 0c01 0801 0802 0e01  ................
+00000e90: 0602 0e02 0c02 1201 1cff 0c03 0201 0e01  ................
+00000ea0: 1001 0402 08ff 02ff 0280 1cfd 0408 0802  ................
+00000eb0: 1001 0c01 0a01 1001 0a03 0801 0280 0c02  ................
+00000ec0: 0201 0201 04ff 0802 1c01 1401 0802 0a01  ................
+00000ed0: 0603 0801 0801 2401 0402 2801 1001 0402  ......$...(.....
+00000ee0: 0280 0e02 0201 0201 04ff 0802 0a01 1002  ................
+00000ef0: 7a15 456e 7669 726f 6e6d 656e 742e 5f5f  z.Environment.__
+00000f00: 7365 745f 656e 7663 0200 0000 0000 0000  set_envc........
+00000f10: 0000 0000 0300 0000 0400 0000 0300 0000  ................
+00000f20: 736e 0000 007c 017c 0076 0172 317c 017c  sn...|.|.v.r1|.|
+00000f30: 006a 0076 0072 0e7c 006a 007c 0119 0053  .j.v.r.|.j.|...S
+00000f40: 0074 016a 02a0 037c 0164 00a1 027d 027c  .t.j...|.d...}.|
+00000f50: 0264 0075 0073 1d7c 0264 016b 0272 2f74  .d.u.s.|.d.k.r/t
+00000f60: 0464 027c 019b 0064 039d 0383 0101 0074  .d.|...d.......t
+00000f70: 0464 0483 0101 0074 05a0 0664 05a1 0101  .d.....t...d....
+00000f80: 006e 027c 0253 0074 0783 00a0 087c 01a1  .n.|.S.t.....|..
+00000f90: 0153 0029 064e 7242 0000 007a 1545 6e76  .S.).NrB...z.Env
+00000fa0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00000fb0: 6520 7a30 206e 6f74 2066 6f75 6e64 2e20  e z0 not found. 
+00000fc0: 5365 7420 6974 2069 6e20 656e 762e 6a73  Set it in env.js
+00000fd0: 6f6e 206f 7220 696e 2079 6f75 7220 7368  on or in your sh
+00000fe0: 656c 6c2e 7245 0000 0072 0400 0000 2909  ell.rE...r....).
+00000ff0: 7202 0000 0072 1800 0000 724b 0000 0072  r....r....rK...r
+00001000: 4f00 0000 7246 0000 0072 1000 0000 724e  O...rF...r....rN
+00001010: 0000 00da 0573 7570 6572 da0b 5f5f 6765  .....super..__ge
+00001020: 7469 7465 6d5f 5f29 0372 1e00 0000 7220  titem__).r....r 
+00001030: 0000 00da 0372 6573 a901 da09 5f5f 636c  .....res....__cl
+00001040: 6173 735f 5f72 2200 0000 7223 0000 0072  ass__r"...r#...r
+00001050: 5200 0000 b200 0000 7318 0000 0008 010a  R.......s.......
+00001060: 020a 010e 0110 0202 010a 0104 ff08 020c  ................
+00001070: 0104 020c 027a 1745 6e76 6972 6f6e 6d65  .....z.Environme
+00001080: 6e74 2e5f 5f67 6574 6974 656d 5f5f 290a  nt.__getitem__).
+00001090: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000010a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000010b0: 6d65 5f5f 7224 0000 0072 1600 0000 7213  me__r$...r....r.
+000010c0: 0000 0072 1d00 0000 721c 0000 0072 5200  ...r....r....rR.
+000010d0: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+000010e0: 5f72 2200 0000 7222 0000 0072 5400 0000  _r"...r"...rT...
+000010f0: 7223 0000 0072 0300 0000 0c00 0000 730e  r#...r........s.
+00001100: 0000 0008 0008 0208 2b08 0e08 0c08 1b14  ........+.......
+00001110: 4472 0300 0000 2908 7232 0000 0072 1800  Dr....).r2...r..
+00001120: 0000 723c 0000 0072 1000 0000 5a04 6970  ..r<...r....Z.ip
+00001130: 6462 7247 0000 0072 3f00 0000 7203 0000  dbrG...r?...r...
+00001140: 0072 2200 0000 7222 0000 0072 2200 0000  .r"...r"...r"...
+00001150: 7223 0000 00da 083c 6d6f 6475 6c65 3e01  r#.....<module>.
+00001160: 0000 0073 0e00 0000 0801 0801 0801 0801  ...s............
+00001170: 0801 0403 1403                           ......
```

### Comparing `yerbamate-0.9.23/packages/yerbamate/__pycache__/mate.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/__pycache__/mate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/__pycache__/mate_cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/__pycache__/mate_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/__pycache__/module_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/__pycache__/module_repository.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr  8 19:56:23 2023 UTC, .py size: 14686 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e7c6 3164 5e39 0000  o.........1d^9..
+00000000: 6f0d 0d0a 0000 0000 22d1 5264 7d3c 0000  o.......".Rd}<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6402 6404 6c07 6d08 5a08 0100 6402  ..d.d.l.m.Z...d.
 00000070: 6405 6c09 6d0a 5a0a 0100 6402 6406 6c0b  d.l.m.Z...d.d.l.
@@ -293,416 +293,454 @@
 00001240: 0072 1300 0000 5a18 5f5f 6765 6e65 7261  .r....Z.__genera
 00001250: 7465 5f64 6570 735f 696e 5f64 6570 7468  te_deps_in_depth
 00001260: 8e00 0000 731c 0000 000e 0414 0102 010e  ....s...........
 00001270: 010c 0110 020c 0102 0108 030c 010a 020a  ................
 00001280: 0202 8004 f07a 294d 6f64 756c 6552 6570  .....z)ModuleRep
 00001290: 6f73 6974 6f72 792e 5f5f 6765 6e65 7261  ository.__genera
 000012a0: 7465 5f64 6570 735f 696e 5f64 6570 7468  te_deps_in_depth
-000012b0: 6301 0000 0000 0000 0000 0000 0011 0000  c...............
-000012c0: 000b 0000 000f 0000 0073 bc03 0000 7c00  .........s....|.
+000012b0: 6301 0000 0000 0000 0000 0000 0012 0000  c...............
+000012c0: 000b 0000 000f 0000 0073 4604 0000 7c00  .........sF...|.
 000012d0: a000 a100 0100 7c00 a001 a100 7d03 6700  ......|.....}.g.
 000012e0: 7d04 7c03 a002 a100 4400 5d2b 5c02 8900  }.|.....D.]+\...
 000012f0: 7d05 7403 7c05 8301 7401 7500 7225 7c04  }.t.|...t.u.r%|.
 00001300: a004 8700 6601 6401 6402 8408 7c05 4400  ....f.d.d...|.D.
 00001310: 8301 a101 0100 710e 7403 7c05 8301 7405  ......q.t.|...t.
 00001320: 7500 7239 7c04 a004 8700 6601 6403 6402  u.r9|.....f.d.d.
 00001330: 8408 7c05 a006 a100 4400 8301 a101 0100  ..|.....D.......
 00001340: 710e 6404 6402 8400 7c04 4400 8301 7d04  q.d.d...|.D...}.
-00001350: 7407 8300 7d06 7c06 a008 6405 a101 6406  t...}.|...d...d.
-00001360: 1900 7d07 7c06 a008 6405 a101 6407 1900  ..}.|...d...d...
-00001370: 7d08 7c04 4400 5d47 7d09 7c06 9b00 7c00  }.|.D.]G}.|...|.
-00001380: 6a09 6a0a 9b00 6405 7c09 6408 1900 9b00  j.j...d.|.d.....
-00001390: 6405 7c09 6409 1900 9b00 9d06 7c09 640a  d.|.d.......|.d.
-000013a0: 3c00 7c07 9b00 6405 7c08 9b00 6405 7c00  <.|...d.|...d.|.
-000013b0: 6a09 6a0a 9b00 6405 7c09 6408 1900 9b00  j.j...d.|.d.....
-000013c0: 6405 7c09 6409 1900 9b00 9d09 7c09 640b  d.|.d.......|.d.
-000013d0: 3c00 7c08 7c00 6a09 6a0a 6b02 729b 7c07  <.|.|.j.j.k.r.|.
-000013e0: 9b00 6405 7c08 9b00 6405 7c09 6408 1900  ..d.|...d.|.d...
-000013f0: 9b00 6405 7c09 6409 1900 9b00 9d07 7c09  ..d.|.d.......|.
-00001400: 640b 3c00 7154 7c04 4400 5d89 7d09 740b  d.<.qT|.D.].}.t.
-00001410: 6a0c a00d 7c00 6a09 6a0a 7c09 6408 1900  j...|.j.j.|.d...
-00001420: 7c09 6409 1900 640c a104 7d0a 740b 6a0c  |.d...d...}.t.j.
-00001430: a00d 7c00 6a09 6a0a 7c09 6408 1900 7c09  ..|.j.j.|.d...|.
-00001440: 6409 1900 640d a104 7d0b 740b 6a0c a00e  d...d...}.t.j...
-00001450: 7c0a a101 72df 740f 7c0a 640e 8302 8f0e  |...r.t.|.d.....
-00001460: 7d0c 7c0c a010 a100 7c09 640f 3c00 5700  }.|.....|.d.<.W.
-00001470: 6400 0400 0400 8303 0100 6e08 3100 73da  d.........n.1.s.
-00001480: 7701 0100 0100 0100 5900 0100 740b 6a0c  w.......Y...t.j.
-00001490: a00e 7c0b a101 9001 7217 740f 7c0b 640e  ..|.....r.t.|.d.
-000014a0: 8302 8f23 7d0c 640f 7c09 7600 72fe 7c09  ...#}.d.|.v.r.|.
-000014b0: 640f 0500 1900 7411 a012 7c0c a101 640f  d.....t...|...d.
-000014c0: 1900 3700 0300 3c00 6e09 7411 a012 7c0c  ..7...<.n.t...|.
-000014d0: a101 640f 1900 7c09 640f 3c00 5700 6400  ..d...|.d.<.W.d.
-000014e0: 0400 0400 8303 0100 6e09 3100 9001 7312  ........n.1...s.
-000014f0: 7701 0100 0100 0100 5900 0100 640f 7c09  w.......Y...d.|.
-00001500: 7600 9001 7227 6410 6402 8400 7c09 640f  v...r'd.d...|.d.
-00001510: 1900 4400 8301 7c09 640f 3c00 719e 7c04  ..D...|.d.<.q.|.
-00001520: 7d0d 6700 7d0d 740f 6411 6412 8302 8f10  }.g.}.t.d.d.....
-00001530: 7d0c 7411 6a13 7c04 7c0c 6407 6413 8d03  }.t.j.|.|.d.d...
-00001540: 0100 5700 6400 0400 0400 8303 0100 6e09  ..W.d.........n.
-00001550: 3100 9001 7345 7701 0100 0100 0100 5900  1...sEw.......Y.
-00001560: 0100 7c04 4400 5d42 7d09 640f 7c09 7600  ..|.D.]B}.d.|.v.
-00001570: 9001 727b 6700 7d0e 7c09 640f 1900 4400  ..r{g.}.|.d...D.
-00001580: 5d0f 7d0f 6414 7c0f 7600 9001 7262 9001  ].}.d.|.v...rb..
-00001590: 7159 7c0e a004 7c0f a101 0100 9001 7159  qY|...|.......qY
-000015a0: 7c0d a004 7c09 6409 1900 7c09 6408 1900  |...|.d...|.d...
-000015b0: 7c09 640b 1900 7c0e 6415 9c04 a101 0100  |.d...|.d.......
-000015c0: 9001 714c 7c0d a004 7c09 6409 1900 7c09  ..qL|...|.d...|.
-000015d0: 6408 1900 7c09 640b 1900 7c09 640f 1900  d...|.d...|.d...
-000015e0: 6415 9c04 a101 0100 9001 714c 7414 6a14  d.........qLt.j.
-000015f0: 7c0d 6416 6417 6418 6419 8d04 7d10 7414  |.d.d.d.d...}.t.
-00001600: 6a14 7c04 6416 641a 641b 641c 641d 8d05  j.|.d.d.d.d.d...
-00001610: 7d04 740f 641e 6412 8302 8f0d 7d0c 7c0c  }.t.d.d.....}.|.
-00001620: a015 7c04 a101 0100 5700 6400 0400 0400  ..|.....W.d.....
-00001630: 8303 0100 6e09 3100 9001 73b8 7701 0100  ....n.1...s.w...
-00001640: 0100 0100 5900 0100 740f 641f 6412 8302  ....Y...t.d.d...
-00001650: 8f0d 7d0c 7c0c a015 7c10 a101 0100 5700  ..}.|...|.....W.
-00001660: 6400 0400 0400 8303 0100 6e09 3100 9001  d.........n.1...
-00001670: 73d3 7701 0100 0100 0100 5900 0100 7416  s.w.......Y...t.
-00001680: 6420 8301 0100 6400 5300 2921 4e63 0100  d ....d.S.)!Nc..
-00001690: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-000016a0: 0000 1300 0000 f316 0000 0067 007c 005d  ...........g.|.]
-000016b0: 077d 0188 007c 0164 009c 0291 0271 0253  .}...|.d.....q.S
-000016c0: 00a9 0129 02da 0474 7970 65da 046e 616d  ...)...type..nam
-000016d0: 6572 1200 0000 a902 7254 0000 0072 6b00  er......rT...rk.
-000016e0: 0000 a901 da03 6b65 7972 1200 0000 7213  ......keyr....r.
-000016f0: 0000 0072 5600 0000 ae00 0000 f302 0000  ...rV...........
-00001700: 0016 007a 2d4d 6f64 756c 6552 6570 6f73  ...z-ModuleRepos
-00001710: 6974 6f72 792e 5f5f 6578 706f 7274 2e3c  itory.__export.<
-00001720: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00001730: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
-00001740: 0000 0005 0000 0013 0000 0072 6800 0000  ...........rh...
-00001750: 7269 0000 0072 1200 0000 726c 0000 0072  ri...r....rl...r
-00001760: 6d00 0000 7212 0000 0072 1300 0000 7256  m...r....r....rV
-00001770: 0000 00b0 0000 0072 6f00 0000 6301 0000  .......ro...c...
-00001780: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00001790: 0053 0000 00f3 1a00 0000 6700 7c00 5d09  .S........g.|.].
-000017a0: 7d01 7c01 4400 5d04 7d02 7c02 9103 7106  }.|.D.].}.|...q.
-000017b0: 7102 5300 7212 0000 0072 1200 0000 a903  q.S.r....r......
-000017c0: 7254 0000 005a 0773 7562 6c69 7374 da04  rT...Z.sublist..
-000017d0: 6974 656d 7212 0000 0072 1200 0000 7213  itemr....r....r.
-000017e0: 0000 0072 5600 0000 b400 0000 f302 0000  ...rV...........
-000017f0: 001a 00fa 012f e903 0000 0072 1800 0000  ...../.....r....
-00001800: 726a 0000 0072 6b00 0000 7236 0000 00da  rj...rk...r6....
-00001810: 0973 686f 7274 5f75 726c fa10 7265 7175  .short_url..requ
-00001820: 6972 656d 656e 7473 2e74 7874 fa11 6465  irements.txt..de
-00001830: 7065 6e64 656e 6369 6573 2e6a 736f 6e72  pendencies.jsonr
-00001840: 5200 0000 da0c 6465 7065 6e64 656e 6369  R.....dependenci
-00001850: 6573 6301 0000 0000 0000 0000 0000 0002  esc.............
-00001860: 0000 0006 0000 0053 0000 00f3 1800 0000  .......S........
-00001870: 6700 7c00 5d08 7d01 7c01 a000 6400 6401  g.|.].}.|...d.d.
-00001880: a102 9102 7102 5300 2902 725b 0000 0072  ....q.S.).r[...r
-00001890: 4400 0000 a901 da07 7265 706c 6163 6529  D.......replace)
-000018a0: 0272 5400 0000 da03 6465 7072 1200 0000  .rT.....depr....
-000018b0: 7212 0000 0072 1300 0000 7256 0000 00e1  r....r....rV....
-000018c0: 0000 0073 0600 0000 0600 0c01 06ff 7a0c  ...s..........z.
-000018d0: 6578 706f 7274 732e 6a73 6f6e 7217 0000  exports.jsonr...
-000018e0: 0072 1900 0000 7a07 2d2d 6578 7472 6129  .r....z.--extra)
-000018f0: 0472 6b00 0000 726a 0000 0072 7600 0000  .rk...rj...rv...
-00001900: 7279 0000 00da 046b 6579 73da 056c 6174  ry.....keys..lat
-00001910: 6578 da05 6e65 7665 7229 03da 0768 6561  ex..never)...hea
-00001920: 6465 7273 da08 7461 626c 6566 6d74 da09  ders..tablefmt..
-00001930: 7368 6f77 696e 6465 785a 0667 6974 6875  showindexZ.githu
-00001940: 62da 0661 6c77 6179 7354 2904 7281 0000  b..alwaysT).r...
-00001950: 0072 8200 0000 7283 0000 005a 1064 6973  .r....r....Z.dis
-00001960: 6162 6c65 5f6e 756d 7061 7273 657a 0965  able_numparsez.e
-00001970: 7870 6f72 742e 6d64 7a0b 6578 706f 7274  xport.mdz.export
-00001980: 732e 7465 787a 1545 7870 6f72 7465 6420  s.texz.Exported 
-00001990: 746f 2065 7870 6f72 742e 6d64 2917 da28  to export.md)..(
-000019a0: 5f4d 6f64 756c 6552 6570 6f73 6974 6f72  _ModuleRepositor
-000019b0: 795f 5f67 656e 6572 6174 655f 7375 625f  y__generate_sub_
-000019c0: 7069 705f 7265 7173 da04 6c69 7374 da05  pip_reqs..list..
-000019d0: 6974 656d 7372 6a00 0000 da06 6170 7065  itemsrj.....appe
-000019e0: 6e64 da04 6469 6374 727e 0000 0072 0500  nd..dictr~...r..
-000019f0: 0000 da05 7370 6c69 7472 0e00 0000 7216  ....splitr....r.
-00001a00: 0000 0072 2200 0000 7223 0000 0072 2a00  ...r"...r#...r*.
-00001a10: 0000 7224 0000 0072 2b00 0000 725c 0000  ..r$...r+...r\..
-00001a20: 0072 2c00 0000 da04 6c6f 6164 722d 0000  .r,.....loadr-..
-00001a30: 00da 0874 6162 756c 6174 6572 4700 0000  ...tabulaterG...
-00001a40: 7227 0000 0029 1172 1100 0000 7238 0000  r'...).r....r8..
-00001a50: 0072 3900 0000 da07 6d6f 6475 6c65 73da  .r9.....modules.
-00001a60: 0574 6162 6c65 da05 7661 6c75 655a 0862  .table..valueZ.b
-00001a70: 6173 655f 7572 6c5a 0975 7365 725f 6e61  ase_urlZ.user_na
-00001a80: 6d65 5a09 7265 706f 5f6e 616d 6572 7200  meZ.repo_namerr.
-00001a90: 0000 7223 0000 005a 0864 6570 5f70 6174  ..r#...Z.dep_pat
-00001aa0: 6872 3200 0000 5a06 6c74 6162 6c65 5a07  hr2...Z.ltableZ.
-00001ab0: 6e65 775f 6465 7072 7d00 0000 5a0b 6c61  new_depr}...Z.la
-00001ac0: 7465 785f 7461 626c 6572 1200 0000 726d  tex_tabler....rm
-00001ad0: 0000 0072 1300 0000 5a08 5f5f 6578 706f  ...r....Z.__expo
-00001ae0: 7274 a400 0000 73c2 0000 0008 0208 0204  rt....s.........
-00001af0: 0210 020c 011a 010c 011c 0102 800e 0406  ................
-00001b00: 040e 010e 0108 0122 0402 fe02 0102 ff2a  .......".......*
-00001b10: 0502 fe02 0102 ff0c 0520 0502 fe02 0102  ......... ......
-00001b20: ff02 8008 0506 0114 0104 ff06 0314 0104  ................
-00001b30: ff0c 040c 010e 011c ff0e 020c 0108 011c  ................
-00001b40: 0112 0202 801e fc0a 0706 0106 010a ff02  ................
-00001b50: 8004 0904 0b0c 0312 011e ff08 030a 0204  ................
-00001b60: 020c 010a 0104 010e 0104 0106 0206 0106  ................
-00001b70: 0102 0104 fc08 ff04 0906 0206 0106 0106  ................
-00001b80: 0104 fc08 ff04 0b02 0102 0102 0102 0106  ................
-00001b90: fc04 0802 0102 0102 0102 0102 0106 fb0c  ................
-00001ba0: 0a0c 011e ff0c 030c 011e ff0c 047a 194d  .............z.M
-00001bb0: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
-00001bc0: 5f5f 6578 706f 7274 6301 0000 0000 0000  __exportc.......
-00001bd0: 0000 0000 0005 0000 0006 0000 0043 0000  .............C..
-00001be0: 0073 8a00 0000 7c00 6a00 6a01 7d01 7c00  .s....|.j.j.}.|.
-00001bf0: a002 7c01 a101 0100 7403 a004 6401 a101  ..|.....t...d...
-00001c00: 4400 5d34 7d02 7c02 a005 6401 a101 7320  D.]4}.|...d...s 
-00001c10: 7c02 a005 6402 a101 7320 7c02 7c00 6a00  |...d...s |.|.j.
-00001c20: 6a01 6b02 7221 710e 7403 6a06 a007 6401  j.k.r!q.t.j...d.
-00001c30: 7c02 a102 7d03 7403 6a06 a008 7c03 a101  |...}.t.j...|...
-00001c40: 7242 7403 6a06 a007 6401 7c02 6403 a103  rBt.j...d.|.d...
-00001c50: 7d04 7403 6a06 a009 7c04 a101 733d 710e  }.t.j...|...s=q.
-00001c60: 7c00 a00a 7c03 a101 0100 710e 6400 5300  |...|.....q.d.S.
-00001c70: 2904 4e72 4600 0000 7262 0000 0072 1b00  ).NrF...rb...r..
-00001c80: 0000 290b 720e 0000 0072 1600 0000 7265  ..).r....r....re
-00001c90: 0000 0072 2200 0000 7248 0000 0072 6300  ...r"...rH...rc.
-00001ca0: 0000 7223 0000 0072 2a00 0000 7249 0000  ..r#...r*...rI..
-00001cb0: 0072 2400 0000 7264 0000 0072 6600 0000  .r$...rd...rf...
-00001cc0: 7212 0000 0072 1200 0000 7213 0000 005a  r....r....r....Z
-00001cd0: 175f 5f67 656e 6572 6174 655f 7375 625f  .__generate_sub_
-00001ce0: 7069 705f 7265 7173 3301 0000 7322 0000  pip_reqs3...s"..
-00001cf0: 0008 020a 010e 0208 0202 ff08 0202 fe0c  ................
-00001d00: 0302 020e 010c 0110 020c 0102 010a 0102  ................
-00001d10: 8004 f37a 284d 6f64 756c 6552 6570 6f73  ...z(ModuleRepos
-00001d20: 6974 6f72 792e 5f5f 6765 6e65 7261 7465  itory.__generate
-00001d30: 5f73 7562 5f70 6970 5f72 6571 7363 0200  _sub_pip_reqsc..
-00001d40: 0000 0000 0000 0000 0000 0e00 0000 0a00  ................
-00001d50: 0000 0300 0000 736e 0200 0064 0164 0284  ......sn...d.d..
-00001d60: 0074 00a0 0188 01a1 0144 0083 017d 0264  .t.......D...}.d
-00001d70: 0364 0284 007c 0244 0083 0164 0464 0284  .d...|.D...d.d..
-00001d80: 0074 00a0 0188 01a1 0144 0083 0117 0089  .t.......D......
-00001d90: 0087 0166 0164 0564 0284 087c 0244 0083  ...f.d.d...|.D..
-00001da0: 017d 0374 0264 0664 0284 007c 0344 0083  .}.t.d.d...|.D..
-00001db0: 0183 017d 0387 0066 0164 0764 0284 087c  ...}...f.d.d...|
-00001dc0: 0344 0083 017d 0374 0383 007d 047c 0464  .D...}.t...}.|.d
-00001dd0: 0075 0072 4374 0464 0883 0101 0064 0053  .u.rCt.d.....d.S
-00001de0: 0074 0283 007d 057c 0344 005d 5d7d 067c  .t...}.|.D.]]}.|
-00001df0: 06a0 0564 09a1 0172 5071 487c 006a 066a  ...d...rPqH|.j.j
-00001e00: 0767 017c 06a0 0864 0aa1 01a2 017d 077c  .g.|...d.....}.|
-00001e10: 0764 0b19 0064 0917 007c 0764 0b3c 0067  .d...d...|.d.<.g
-00001e20: 007c 06a0 0864 0aa1 01a2 017d 0874 006a  .|...d.....}.t.j
-00001e30: 09a0 0a74 006a 096a 0b7c 078e 00a1 0172  ...t.j.j.|.....r
-00001e40: 7d64 0ca0 0b7c 0764 0064 0b85 0219 00a1  }d...|.d.d......
-00001e50: 017d 096e 1d74 006a 09a0 0a74 006a 096a  .}.n.t.j...t.j.j
-00001e60: 0b7c 088e 00a1 0172 8e7c 0864 0d19 0064  .|.....r.|.d...d
-00001e70: 0c17 007d 096e 0c7c 006a 066a 0764 0c17  ...}.n.|.j.j.d..
-00001e80: 007c 06a0 0c64 0a64 0ca1 0217 007d 097c  .|...d.d.....}.|
-00001e90: 0472 a07c 047c 0917 007d 097c 05a0 0d7c  .r.|.|...}.|...|
-00001ea0: 09a1 0101 0071 4874 0e7c 0583 0164 0d6b  .....qHt.|...d.k
-00001eb0: 0272 ae64 0053 007a 3774 006a 09a0 0b88  .r.d.S.z7t.j....
-00001ec0: 0164 0ea1 027d 0a74 006a 09a0 0a7c 0aa1  .d...}.t.j...|..
-00001ed0: 0172 e274 0f7c 0a64 0f83 028f 187d 0b74  .r.t.|.d.....}.t
-00001ee0: 10a0 117c 0ba1 017d 0a64 107c 0a76 0072  ...|...}.d.|.v.r
-00001ef0: d07c 0a64 1019 007d 0c6e 0269 007d 0c57  .|.d...}.n.i.}.W
-00001f00: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
-00001f10: dc77 0101 0001 0001 0059 0001 006e 0269  .w.......Y...n.i
-00001f20: 007d 0c57 006e 1d04 0074 1290 0179 0201  .}.W.n...t...y..
-00001f30: 007d 0d01 007a 1074 0464 1188 019b 0064  .}...z.t.d.....d
-00001f40: 129d 0383 0101 0069 007d 0c57 0059 0064  .......i.}.W.Y.d
-00001f50: 007d 0d7e 0d6e 0564 007d 0d7e 0d77 0177  .}.~.n.d.}.~.w.w
-00001f60: 0074 0f74 006a 09a0 0b88 0164 0ea1 0264  .t.t.j.....d...d
-00001f70: 1383 028f 1f7d 0b74 137c 0583 017c 0c64  .....}.t.|...|.d
-00001f80: 149c 027d 0574 106a 147c 057c 0b64 1564  ...}.t.j.|.|.d.d
-00001f90: 168d 0301 0074 0464 1788 019b 009d 0283  .....t.d........
-00001fa0: 0101 0057 0064 0004 0004 0083 0301 0064  ...W.d.........d
-00001fb0: 0053 0031 0090 0173 3077 0101 0001 0001  .S.1...s0w......
-00001fc0: 0059 0001 0064 0053 0029 184e 6301 0000  .Y...d.S.).Nc...
-00001fd0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00001fe0: 0053 0000 0073 2200 0000 6700 7c00 5d0d  .S...s"...g.|.].
-00001ff0: 7d01 7c01 a000 6400 a101 7202 6401 7c01  }.|...d...r.d.|.
-00002000: 7601 7202 7c01 9102 7102 5300 2902 fa03  v.r.|...q.S.)...
-00002010: 2e70 7972 6200 0000 2901 da08 656e 6473  .pyrb...)...ends
-00002020: 7769 7468 a902 7254 0000 0072 3200 0000  with..rT...r2...
-00002030: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00002040: 5600 0000 4a01 0000 7302 0000 0022 007a  V...J...s....".z
-00002050: 414d 6f64 756c 6552 6570 6f73 6974 6f72  AModuleRepositor
-00002060: 792e 5f5f 6765 6e65 7261 7465 5f6d 6174  y.__generate_mat
-00002070: 655f 6465 7065 6e64 656e 6369 6573 2e3c  e_dependencies.<
-00002080: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00002090: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
-000020a0: 0000 0006 0000 0053 0000 0072 7a00 0000  .......S...rz...
-000020b0: 2902 7290 0000 0072 4400 0000 727b 0000  ).r....rD...r{..
-000020c0: 00a9 0272 5400 0000 da04 6669 6c65 7212  ...rT.....filer.
-000020d0: 0000 0072 1200 0000 7213 0000 0072 5600  ...r....r....rV.
-000020e0: 0000 4b01 0000 725a 0000 0063 0100 0000  ..K...rZ...c....
-000020f0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00002100: 5300 0000 7318 0000 0067 007c 005d 087d  S...s....g.|.].}
-00002110: 0164 007c 0176 0172 027c 0191 0271 0253  .d.|.v.r.|...q.S
-00002120: 0029 0172 6200 0000 7212 0000 0072 9200  .).rb...r....r..
-00002130: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00002140: 0072 5600 0000 4b01 0000 7304 0000 0006  .rV...K...s.....
-00002150: 0012 0163 0100 0000 0000 0000 0000 0000  ...c............
-00002160: 0200 0000 0700 0000 1300 0000 731e 0000  ............s...
-00002170: 0067 007c 005d 0b7d 0174 0074 016a 02a0  .g.|.].}.t.t.j..
-00002180: 0388 007c 01a1 0283 0191 0271 0253 0072  ...|.......q.S.r
-00002190: 1200 0000 2904 7204 0000 0072 2200 0000  ....).r....r"...
-000021a0: 7223 0000 0072 2a00 0000 7292 0000 0029  r#...r*...r....)
-000021b0: 0172 2300 0000 7212 0000 0072 1300 0000  .r#...r....r....
-000021c0: 7256 0000 004f 0100 0073 0200 0000 1e00  rV...O...s......
-000021d0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-000021e0: 0004 0000 0053 0000 0072 7000 0000 7212  .....S...rp...r.
-000021f0: 0000 0072 1200 0000 7271 0000 0072 1200  ...r....rq...r..
-00002200: 0000 7212 0000 0072 1300 0000 7256 0000  ..r....r....rV..
-00002210: 0052 0100 0072 7300 0000 6301 0000 0000  .R...rs...c.....
-00002220: 0000 0000 0000 0001 0000 0006 0000 0013  ................
-00002230: 0000 0073 2600 0000 6700 7c00 5d0f 8900  ...s&...g.|.]...
-00002240: 7400 8700 6601 6400 6401 8408 8801 4400  t...f.d.d.....D.
-00002250: 8301 8301 7302 8800 9102 7102 5300 2902  ....s.....q.S.).
-00002260: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00002270: 0004 0000 0013 0000 0073 1400 0000 6700  .........s....g.
-00002280: 7c00 5d06 7d01 7c01 8800 7600 9102 7102  |.].}.|...v...q.
-00002290: 5300 7212 0000 0072 1200 0000 7293 0000  S.r....r....r...
-000022a0: 00a9 01da 066d 6f64 756c 6572 1200 0000  .....moduler....
-000022b0: 7213 0000 0072 5600 0000 5801 0000 7302  r....rV...X...s.
-000022c0: 0000 0014 007a 4c4d 6f64 756c 6552 6570  .....zLModuleRep
-000022d0: 6f73 6974 6f72 792e 5f5f 6765 6e65 7261  ository.__genera
-000022e0: 7465 5f6d 6174 655f 6465 7065 6e64 656e  te_mate_dependen
-000022f0: 6369 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  cies.<locals>.<l
-00002300: 6973 7463 6f6d 703e 2e3c 6c69 7374 636f  istcomp>.<listco
-00002310: 6d70 3e29 01da 0361 6e79 2901 7254 0000  mp>)...any).rT..
-00002320: 0029 01da 0e6f 7269 6769 6e61 6c5f 6669  .)...original_fi
-00002330: 6c65 7372 9500 0000 7213 0000 0072 5600  lesr....r....rV.
-00002340: 0000 5501 0000 730c 0000 0006 0002 0214  ..U...s.........
-00002350: 0102 fd02 0106 ff7a 2c4e 6f20 6769 7420  .......z,No git 
-00002360: 7572 6c20 666f 756e 642c 2073 6b69 7070  url found, skipp
-00002370: 696e 6720 6465 7065 6e64 656e 6369 6573  ing dependencies
-00002380: 2e6a 736f 6e72 9000 0000 7246 0000 00e9  .jsonr....rF....
-00002390: ffff ffff 7274 0000 0072 0100 0000 7278  ....rt...r....rx
-000023a0: 0000 0072 5200 0000 da03 656e 767a 0e45  ...rR.....envz.E
-000023b0: 7272 6f72 2072 6561 6469 6e67 207a 202f  rror reading z /
-000023c0: 6465 7065 6e64 656e 6369 6573 2e6a 736f  dependencies.jso
-000023d0: 6e2c 2073 6b69 7070 696e 6720 656e 7672  n, skipping envr
-000023e0: 1700 0000 2902 7279 0000 0072 9a00 0000  ....).ry...r....
-000023f0: 7218 0000 0072 1900 0000 7a20 4765 6e65  r....r....z Gene
-00002400: 7261 7465 6420 6465 7065 6e64 656e 6369  rated dependenci
-00002410: 6573 2e6a 736f 6e20 666f 7220 2915 7222  es.json for ).r"
-00002420: 0000 0072 4800 0000 724d 0000 0072 0500  ...rH...rM...r..
-00002430: 0000 7227 0000 0072 9100 0000 720e 0000  ..r'...r....r...
-00002440: 0072 1600 0000 728a 0000 0072 2300 0000  .r....r....r#...
-00002450: 7224 0000 0072 2a00 0000 727c 0000 0072  r$...r*...r|...r
-00002460: 4e00 0000 725d 0000 0072 2b00 0000 722c  N...r]...r+...r,
-00002470: 0000 0072 8b00 0000 7231 0000 0072 8600  ...r....r1...r..
-00002480: 0000 722d 0000 0029 0e72 1100 0000 7223  ..r-...).r....r#
-00002490: 0000 00da 0566 696c 6573 5a10 7265 6c61  .....filesZ.rela
-000024a0: 7469 7665 5f69 6d70 6f72 7473 5a07 7572  tive_importsZ.ur
-000024b0: 6c5f 6769 74da 0464 6570 7372 9600 0000  l_git..depsr....
-000024c0: 5a05 7470 6174 685a 1273 6973 7465 725f  Z.tpathZ.sister_
-000024d0: 6d6f 6475 6c65 5f70 6174 6872 3600 0000  module_pathr6...
-000024e0: 5a09 6465 7073 5f6a 736f 6e72 3200 0000  Z.deps_jsonr2...
-000024f0: 729a 0000 0072 3400 0000 7212 0000 0029  r....r4...r....)
-00002500: 0272 9800 0000 7223 0000 0072 1300 0000  .r....r#...r....
-00002510: 5a1c 5f5f 6765 6e65 7261 7465 5f6d 6174  Z.__generate_mat
-00002520: 655f 6465 7065 6e64 656e 6369 6573 4701  e_dependenciesG.
-00002530: 0000 736e 0000 0014 0312 0108 0108 ff12  ..sn............
-00002540: 0402 020c 0104 ff0a 0402 0206 fe06 0608  ................
-00002550: 0208 0104 0106 0208 010a 0202 0114 0310  ................
-00002560: 010e 0214 0214 0214 010e 0118 0204 0208  ................
-00002570: 010c 010c 0204 0102 020e 020c 010c 010a  ................
-00002580: 0208 010a 0104 0202 801c fa02 8004 0904  ................
-00002590: 8010 0110 0110 0108 8002 fe16 040e 0110  ................
-000025a0: 0110 0124 fd7a 2d4d 6f64 756c 6552 6570  ...$.z-ModuleRep
-000025b0: 6f73 6974 6f72 792e 5f5f 6765 6e65 7261  ository.__genera
-000025c0: 7465 5f6d 6174 655f 6465 7065 6e64 656e  te_mate_dependen
-000025d0: 6369 6573 6302 0000 0000 0000 0000 0000  ciesc...........
-000025e0: 0009 0000 0006 0000 0043 0000 0073 b800  .........C...s..
-000025f0: 0000 7400 a001 7c01 a101 7d02 7400 a002  ..t...|...}.t...
-00002600: 7c02 a101 7d03 7c00 a003 7c01 a101 0100  |...}.|...|.....
-00002610: 6700 7d04 7c01 7c00 6a04 6a05 6b02 7224  g.}.|.|.j.j.k.r$
-00002620: 7400 a006 6401 7c03 6402 a103 0100 7c00  t...d.|.d.....|.
-00002630: a007 6401 a101 0100 6e1d 7400 a006 7408  ..d.....n.t...t.
-00002640: 6a09 a00a 7c01 6401 a102 7c03 6402 a103  j...|.d...|.d...
-00002650: 0100 7c00 a007 7408 6a09 a00a 7c01 6401  ..|...t.j...|.d.
-00002660: a102 a101 0100 740b 6403 7c01 9b00 9d02  ......t.d.|.....
-00002670: 8301 0100 7c03 4400 5d14 7d05 7c05 6404  ....|.D.].}.|.d.
-00002680: 1900 7d06 7c05 6405 1900 7d07 7c06 7c07  ..}.|.d...}.|.|.
-00002690: 6406 9c02 7d08 7c04 a00c 7c08 a101 0100  d...}.|...|.....
-000026a0: 7143 6407 7c04 6901 5300 2908 4e72 7700  qCd.|.i.S.).Nrw.
-000026b0: 0000 7a02 7e3d 7a1f 4765 6e65 7261 7465  ..z.~=z.Generate
-000026c0: 6420 7265 7175 6972 656d 656e 7473 2e74  d requirements.t
-000026d0: 7874 2066 6f72 2072 6b00 0000 da07 7665  xt for rk.....ve
-000026e0: 7273 696f 6e29 0272 6b00 0000 729d 0000  rsion).rk...r...
-000026f0: 00da 0370 6970 290d 7208 0000 005a 0f67  ...pip).r....Z.g
-00002700: 6574 5f61 6c6c 5f69 6d70 6f72 7473 5a10  et_all_importsZ.
-00002710: 6765 745f 696d 706f 7274 5f6c 6f63 616c  get_import_local
-00002720: da2d 5f4d 6f64 756c 6552 6570 6f73 6974  .-_ModuleReposit
-00002730: 6f72 795f 5f67 656e 6572 6174 655f 6d61  ory__generate_ma
-00002740: 7465 5f64 6570 656e 6465 6e63 6965 7372  te_dependenciesr
-00002750: 0e00 0000 7216 0000 005a 1a67 656e 6572  ....r....Z.gener
-00002760: 6174 655f 7265 7175 6972 656d 656e 7473  ate_requirements
-00002770: 5f66 696c 65da 305f 4d6f 6475 6c65 5265  _file.0_ModuleRe
-00002780: 706f 7369 746f 7279 5f5f 6164 645f 696e  pository__add_in
-00002790: 6465 785f 7572 6c5f 746f 5f72 6571 7569  dex_url_to_requi
-000027a0: 7265 6d65 6e74 7372 2200 0000 7223 0000  rementsr"...r#..
-000027b0: 0072 2a00 0000 7227 0000 0072 8800 0000  .r*...r'...r....
-000027c0: 2909 7211 0000 0072 2300 0000 da07 696d  ).r....r#.....im
-000027d0: 706f 7274 735a 1169 6d70 6f72 745f 696e  portsZ.import_in
-000027e0: 666f 5f6c 6f63 616c 5a0b 696d 706f 7274  fo_localZ.import
-000027f0: 5f69 6e66 6f5a 0269 6d72 6b00 0000 729d  _infoZ.imrk...r.
-00002800: 0000 00da 0372 6573 7212 0000 0072 1200  .....resr....r..
-00002810: 0000 7213 0000 005a 1b5f 5f67 656e 6572  ..r....Z.__gener
-00002820: 6174 655f 7069 705f 7265 7175 6972 656d  ate_pip_requirem
-00002830: 656e 7473 9301 0000 732c 0000 000a 030a  ents....s,......
-00002840: 030a 0204 020c 0204 0106 0104 ff0c 0304  ................
-00002850: 0310 0104 ff14 030e 0108 0208 0208 0102  ................
-00002860: 0302 0106 fe0c 0508 027a 2c4d 6f64 756c  .........z,Modul
-00002870: 6552 6570 6f73 6974 6f72 792e 5f5f 6765  eRepository.__ge
-00002880: 6e65 7261 7465 5f70 6970 5f72 6571 7569  nerate_pip_requi
-00002890: 7265 6d65 6e74 7372 9600 0000 6302 0000  rementsr....c...
-000028a0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-000028b0: 0043 0000 0073 1e00 0000 7c01 6400 6b02  .C...s....|.d.k.
-000028c0: 7209 7c00 6a00 a001 a100 5300 7c00 6a00  r.|.j.....S.|.j.
-000028d0: a002 7c01 a101 5300 720d 0000 0029 0372  ..|...S.r....).r
-000028e0: 1000 0000 da07 7375 6d6d 6172 7972 8600  ......summaryr..
-000028f0: 0000 2902 7211 0000 0072 9600 0000 7212  ..).r....r....r.
-00002900: 0000 0072 1200 0000 7213 0000 0072 8600  ...r....r....r..
-00002910: 0000 ba01 0000 7306 0000 0008 010a 010c  ......s.........
-00002920: 017a 154d 6f64 756c 6552 6570 6f73 6974  .z.ModuleReposit
-00002930: 6f72 792e 6c69 7374 6301 0000 0000 0000  ory.listc.......
-00002940: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00002950: 0073 0a00 0000 7c00 6a00 a001 a100 5300  .s....|.j.....S.
-00002960: 720d 0000 0029 0272 1000 0000 72a3 0000  r....).r....r...
-00002970: 0029 0172 1100 0000 7212 0000 0072 1200  .).r....r....r..
-00002980: 0000 7213 0000 00da 1067 6574 5f6d 6174  ..r......get_mat
-00002990: 655f 7375 6d6d 6172 79bf 0100 0073 0200  e_summary....s..
-000029a0: 0000 0a01 7a21 4d6f 6475 6c65 5265 706f  ....z!ModuleRepo
-000029b0: 7369 746f 7279 2e67 6574 5f6d 6174 655f  sitory.get_mate_
-000029c0: 7375 6d6d 6172 79da 0770 6163 6b61 6765  summary..package
-000029d0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000029e0: 0003 0000 0043 0000 0073 1000 0000 7c00  .....C...s....|.
-000029f0: 6a00 a001 7c01 a101 0100 6400 5300 720d  j...|.....d.S.r.
-00002a00: 0000 0029 0272 1000 0000 7237 0000 0029  ...).r....r7...)
-00002a10: 0272 1100 0000 72a5 0000 0072 1200 0000  .r....r....r....
-00002a20: 7212 0000 0072 1300 0000 7237 0000 00c2  r....r....r7....
-00002a30: 0100 0073 0200 0000 1001 7a20 4d6f 6475  ...s......z Modu
-00002a40: 6c65 5265 706f 7369 746f 7279 2e69 6e73  leRepository.ins
-00002a50: 7461 6c6c 5f70 6163 6b61 6765 2901 4672  tall_package).Fr
-00002a60: 0d00 0000 2916 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
-00002a70: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00002a80: 7175 616c 6e61 6d65 5f5f da04 626f 6f6c  qualname__..bool
-00002a90: 7214 0000 00da 0c73 7461 7469 636d 6574  r......staticmet
-00002aa0: 686f 64da 0373 7472 7235 0000 0072 3a00  hod..strr5...r:.
-00002ab0: 0000 7242 0000 0072 4100 0000 7286 0000  ..rB...rA...r...
-00002ac0: 0072 6000 0000 72a0 0000 0072 6500 0000  .r`...r....re...
-00002ad0: 7240 0000 0072 8500 0000 729f 0000 0072  r@...r....r....r
-00002ae0: 6400 0000 72a4 0000 0072 0900 0000 7237  d...r....r....r7
-00002af0: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00002b00: 0000 7213 0000 0072 0b00 0000 1400 0000  ..r....r........
-00002b10: 7324 0000 0008 0010 0102 0710 010e 2a0e  s$............*.
-00002b20: 0410 0612 120e 0e08 1d08 1600 7f08 1008  ................
-00002b30: 1408 4c10 2708 0512 0372 0b00 0000 2916  ..L.'....r....).
-00002b40: 722c 0000 0072 2200 0000 725e 0000 0072  r,...r"...r^...r
-00002b50: 2800 0000 728c 0000 005a 0e6d 6f64 756c  (...r....Z.modul
-00002b60: 655f 6d61 6e61 6765 7272 0300 0000 5a0e  e_managerr....Z.
-00002b70: 7574 696c 732e 6578 705f 7574 696c 7204  utils.exp_utilr.
-00002b80: 0000 005a 0e75 7469 6c73 2e67 6974 5f75  ...Z.utils.git_u
-00002b90: 7469 6c72 0500 0000 5a0e 736f 7572 6365  tilr....Z.source
-00002ba0: 732e 7265 6d6f 7465 7206 0000 005a 1373  s.remoter....Z.s
-00002bb0: 6f75 7263 6573 2e6c 6f63 616c 2e6c 6f63  ources.local.loc
-00002bc0: 616c 7207 0000 0072 0800 0000 72a5 0000  alr....r....r...
-00002bd0: 0072 0900 0000 da06 7479 7069 6e67 720a  .r......typingr.
-00002be0: 0000 00da 0469 7064 6272 0b00 0000 7212  .....ipdbr....r.
-00002bf0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00002c00: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002c10: 731e 0000 0008 0008 0108 0108 0108 020c  s...............
-00002c20: 020c 010c 010c 010c 010c 010c 020c 0108  ................
-00002c30: 0112 03                                  ...
+00001350: 7407 8300 7d06 7408 8300 7d07 7c07 a009  t...}.t...}.|...
+00001360: 6405 a101 6406 1900 7d08 7c07 a009 6405  d...d...}.|...d.
+00001370: a101 6407 1900 7d09 7c04 4400 5d47 7d0a  ..d...}.|.D.]G}.
+00001380: 7c07 9b00 7c00 6a0a 6a0b 9b00 6405 7c0a  |...|.j.j...d.|.
+00001390: 6408 1900 9b00 6405 7c0a 6409 1900 9b00  d.....d.|.d.....
+000013a0: 9d06 7c0a 640a 3c00 7c08 9b00 6405 7c09  ..|.d.<.|...d.|.
+000013b0: 9b00 6405 7c00 6a0a 6a0b 9b00 6405 7c0a  ..d.|.j.j...d.|.
+000013c0: 6408 1900 9b00 6405 7c0a 6409 1900 9b00  d.....d.|.d.....
+000013d0: 9d09 7c0a 640b 3c00 7c09 7c00 6a0a 6a0b  ..|.d.<.|.|.j.j.
+000013e0: 6b02 729e 7c08 9b00 6405 7c09 9b00 6405  k.r.|...d.|...d.
+000013f0: 7c0a 6408 1900 9b00 6405 7c0a 6409 1900  |.d.....d.|.d...
+00001400: 9b00 9d07 7c0a 640b 3c00 7157 7c04 4400  ....|.d.<.qW|.D.
+00001410: 5d91 7d0a 740c 6a0d a00e 7c00 6a0a 6a0b  ].}.t.j...|.j.j.
+00001420: 7c0a 6408 1900 7c0a 6409 1900 640c a104  |.d...|.d...d...
+00001430: 7d0b 740c 6a0d a00e 7c00 6a0a 6a0b 7c0a  }.t.j...|.j.j.|.
+00001440: 6408 1900 7c0a 6409 1900 640d a104 7d0c  d...|.d...d...}.
+00001450: 740c 6a0d a00f 7c0b a101 72e2 7410 7c0b  t.j...|...r.t.|.
+00001460: 640e 8302 8f0e 7d0d 7c0d a011 a100 7c0a  d.....}.|.....|.
+00001470: 640f 3c00 5700 6400 0400 0400 8303 0100  d.<.W.d.........
+00001480: 6e08 3100 73dd 7701 0100 0100 0100 5900  n.1.s.w.......Y.
+00001490: 0100 740c 6a0d a00f 7c0c a101 9001 721b  ..t.j...|.....r.
+000014a0: 7410 7c0c 640e 8302 8f24 7d0d 640f 7c0a  t.|.d....$}.d.|.
+000014b0: 7600 9001 7202 7c0a 640f 0500 1900 7412  v...r.|.d.....t.
+000014c0: a013 7c0d a101 640f 1900 3700 0300 3c00  ..|...d...7...<.
+000014d0: 6e09 7412 a013 7c0d a101 640f 1900 7c0a  n.t...|...d...|.
+000014e0: 640f 3c00 5700 6400 0400 0400 8303 0100  d.<.W.d.........
+000014f0: 6e09 3100 9001 7316 7701 0100 0100 0100  n.1...s.w.......
+00001500: 5900 0100 640f 7c0a 7600 9001 722b 6410  Y...d.|.v...r+d.
+00001510: 6402 8400 7c0a 640f 1900 4400 8301 7c0a  d...|.d...D...|.
+00001520: 640f 3c00 7c06 a014 7c0a 640f 1900 a101  d.<.|...|.d.....
+00001530: 0100 71a1 6411 6402 8400 7c06 4400 8301  ..q.d.d...|.D...
+00001540: 7d06 7415 7c06 6412 6413 8400 6414 6415  }.t.|.d.d...d.d.
+00001550: 8d03 7d06 6416 6402 8400 7c06 4400 8301  ..}.d.d...|.D...
+00001560: 7d06 7410 640c 6417 8302 8f15 7d0d 7c06  }.t.d.d.....}.|.
+00001570: 4400 5d0a 7d0e 7c0d a016 7c0e 6418 1700  D.].}.|...|.d...
+00001580: a101 0100 9001 7152 5700 6400 0400 0400  ......qRW.d.....
+00001590: 8303 0100 6e09 3100 9001 7368 7701 0100  ....n.1...shw...
+000015a0: 0100 0100 5900 0100 7c04 7d0f 6700 7d0f  ....Y...|.}.g.}.
+000015b0: 7410 6419 6417 8302 8f10 7d0d 7412 6a17  t.d.d.....}.t.j.
+000015c0: 7c04 7c0d 6407 641a 8d03 0100 5700 6400  |.|.d.d.....W.d.
+000015d0: 0400 0400 8303 0100 6e09 3100 9001 738a  ........n.1...s.
+000015e0: 7701 0100 0100 0100 5900 0100 7c04 4400  w.......Y...|.D.
+000015f0: 5d42 7d0a 640f 7c0a 7600 9001 72c0 6700  ]B}.d.|.v...r.g.
+00001600: 7d10 7c0a 640f 1900 4400 5d0f 7d0e 641b  }.|.d...D.].}.d.
+00001610: 7c0e 7600 9001 72a7 9001 719e 7c10 a004  |.v...r...q.|...
+00001620: 7c0e a101 0100 9001 719e 7c0f a004 7c0a  |.......q.|...|.
+00001630: 6409 1900 7c0a 6408 1900 7c0a 640b 1900  d...|.d...|.d...
+00001640: 7c10 641c 9c04 a101 0100 9001 7191 7c0f  |.d.........q.|.
+00001650: a004 7c0a 6409 1900 7c0a 6408 1900 7c0a  ..|.d...|.d...|.
+00001660: 640b 1900 7c0a 640f 1900 641c 9c04 a101  d...|.d...d.....
+00001670: 0100 9001 7191 7418 6a18 7c0f 641d 641e  ....q.t.j.|.d.d.
+00001680: 641f 6420 8d04 7d11 7418 6a18 7c04 641d  d.d ..}.t.j.|.d.
+00001690: 6421 6422 6414 6423 8d05 7d04 7410 6424  d!d"d.d#..}.t.d$
+000016a0: 6417 8302 8f0d 7d0d 7c0d a016 7c04 a101  d.....}.|...|...
+000016b0: 0100 5700 6400 0400 0400 8303 0100 6e09  ..W.d.........n.
+000016c0: 3100 9001 73fd 7701 0100 0100 0100 5900  1...s.w.......Y.
+000016d0: 0100 7410 6425 6417 8302 8f0d 7d0d 7c0d  ..t.d%d.....}.|.
+000016e0: a016 7c11 a101 0100 5700 6400 0400 0400  ..|.....W.d.....
+000016f0: 8303 0100 6e09 3100 9002 7318 7701 0100  ....n.1...s.w...
+00001700: 0100 0100 5900 0100 7419 6426 8301 0100  ....Y...t.d&....
+00001710: 6400 5300 2927 4e63 0100 0000 0000 0000  d.S.)'Nc........
+00001720: 0000 0000 0200 0000 0500 0000 1300 0000  ................
+00001730: f316 0000 0067 007c 005d 077d 0188 007c  .....g.|.].}...|
+00001740: 0164 009c 0291 0271 0253 00a9 0129 02da  .d.....q.S...)..
+00001750: 0474 7970 65da 046e 616d 6572 1200 0000  .type..namer....
+00001760: a902 7254 0000 0072 6b00 0000 a901 da03  ..rT...rk.......
+00001770: 6b65 7972 1200 0000 7213 0000 0072 5600  keyr....r....rV.
+00001780: 0000 ae00 0000 7302 0000 0016 007a 2d4d  ......s......z-M
+00001790: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
+000017a0: 5f5f 6578 706f 7274 2e3c 6c6f 6361 6c73  __export.<locals
+000017b0: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
+000017c0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+000017d0: 0013 0000 0072 6800 0000 7269 0000 0072  .....rh...ri...r
+000017e0: 1200 0000 726c 0000 0072 6d00 0000 7212  ....rl...rm...r.
+000017f0: 0000 0072 1300 0000 7256 0000 00b0 0000  ...r....rV......
+00001800: 0073 0600 0000 0600 0201 0eff 6301 0000  .s..........c...
+00001810: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00001820: 0053 0000 00f3 1a00 0000 6700 7c00 5d09  .S........g.|.].
+00001830: 7d01 7c01 4400 5d04 7d02 7c02 9103 7106  }.|.D.].}.|...q.
+00001840: 7102 5300 7212 0000 0072 1200 0000 a903  q.S.r....r......
+00001850: 7254 0000 005a 0773 7562 6c69 7374 da04  rT...Z.sublist..
+00001860: 6974 656d 7212 0000 0072 1200 0000 7213  itemr....r....r.
+00001870: 0000 0072 5600 0000 b500 0000 f302 0000  ...rV...........
+00001880: 001a 00fa 012f e903 0000 0072 1800 0000  ...../.....r....
+00001890: 726a 0000 0072 6b00 0000 7236 0000 00da  rj...rk...r6....
+000018a0: 0973 686f 7274 5f75 726c fa10 7265 7175  .short_url..requ
+000018b0: 6972 656d 656e 7473 2e74 7874 fa11 6465  irements.txt..de
+000018c0: 7065 6e64 656e 6369 6573 2e6a 736f 6e72  pendencies.jsonr
+000018d0: 5200 0000 da0c 6465 7065 6e64 656e 6369  R.....dependenci
+000018e0: 6573 6301 0000 0000 0000 0000 0000 0002  esc.............
+000018f0: 0000 0006 0000 0053 0000 00f3 1800 0000  .......S........
+00001900: 6700 7c00 5d08 7d01 7c01 a000 6400 6401  g.|.].}.|...d.d.
+00001910: a102 9102 7102 5300 2902 725b 0000 0072  ....q.S.).r[...r
+00001920: 4400 0000 a901 da07 7265 706c 6163 65a9  D.......replace.
+00001930: 0272 5400 0000 da03 6465 7072 1200 0000  .rT.....depr....
+00001940: 7212 0000 0072 1300 0000 7256 0000 00e4  r....r....rV....
+00001950: 0000 0073 0600 0000 0600 0c01 06ff 6301  ...s..........c.
+00001960: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001970: 0000 0053 0000 00f3 1800 0000 6700 7c00  ...S........g.|.
+00001980: 5d08 7d01 6400 7c01 7601 7202 7c01 9102  ].}.d.|.v.r.|...
+00001990: 7102 5300 2901 7a0e 6874 7470 733a 2f2f  q.S.).z.https://
+000019a0: 6769 7468 7562 7212 0000 0072 7c00 0000  githubr....r|...
+000019b0: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000019c0: 5600 0000 eb00 0000 725a 0000 0063 0100  V.......rZ...c..
+000019d0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000019e0: 0000 5300 0000 7308 0000 0064 017c 0076  ..S...s....d.|.v
+000019f0: 0053 0029 024e 7a11 2d2d 6578 7472 612d  .S.).Nz.--extra-
+00001a00: 696e 6465 782d 7572 6c72 1200 0000 2901  index-urlr....).
+00001a10: da01 7872 1200 0000 7212 0000 0072 1300  ..xr....r....r..
+00001a20: 0000 da08 3c6c 616d 6264 613e ee00 0000  ....<lambda>....
+00001a30: 7302 0000 0008 007a 2b4d 6f64 756c 6552  s......z+ModuleR
+00001a40: 6570 6f73 6974 6f72 792e 5f5f 6578 706f  epository.__expo
+00001a50: 7274 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  rt.<locals>.<lam
+00001a60: 6264 613e 5429 0272 6e00 0000 da07 7265  bda>T).rn.....re
+00001a70: 7665 7273 6563 0100 0000 0000 0000 0000  versec..........
+00001a80: 0000 0200 0000 0400 0000 5300 0000 7328  ..........S...s(
+00001a90: 0000 0067 007c 005d 107d 017c 0164 006b  ...g.|.].}.|.d.k
+00001aa0: 0373 107c 0164 016b 0373 107c 0164 026b  .s.|.d.k.s.|.d.k
+00001ab0: 0372 027c 0191 0271 0253 0029 0372 5b00  .r.|...q.S.).r[.
+00001ac0: 0000 fa01 2072 4400 0000 7212 0000 0072  .... rD...r....r
+00001ad0: 7c00 0000 7212 0000 0072 1200 0000 7213  |...r....r....r.
+00001ae0: 0000 0072 5600 0000 f000 0000 7302 0000  ...rV.......s...
+00001af0: 0028 0072 1700 0000 725b 0000 007a 0c65  .(.r....r[...z.e
+00001b00: 7870 6f72 7473 2e6a 736f 6e72 1900 0000  xports.jsonr....
+00001b10: 7a07 2d2d 6578 7472 6129 0472 6b00 0000  z.--extra).rk...
+00001b20: 726a 0000 0072 7500 0000 7278 0000 00da  rj...ru...rx....
+00001b30: 046b 6579 73da 056c 6174 6578 da05 6e65  .keys..latex..ne
+00001b40: 7665 7229 03da 0768 6561 6465 7273 da08  ver)...headers..
+00001b50: 7461 626c 6566 6d74 da09 7368 6f77 696e  tablefmt..showin
+00001b60: 6465 785a 0667 6974 6875 62da 0661 6c77  dexZ.github..alw
+00001b70: 6179 7329 0472 8600 0000 7287 0000 0072  ays).r....r....r
+00001b80: 8800 0000 5a10 6469 7361 626c 655f 6e75  ....Z.disable_nu
+00001b90: 6d70 6172 7365 7a09 6578 706f 7274 2e6d  mparsez.export.m
+00001ba0: 647a 0b65 7870 6f72 7473 2e74 6578 7a15  dz.exports.texz.
+00001bb0: 4578 706f 7274 6564 2074 6f20 6578 706f  Exported to expo
+00001bc0: 7274 2e6d 6429 1ada 285f 4d6f 6475 6c65  rt.md)..(_Module
+00001bd0: 5265 706f 7369 746f 7279 5f5f 6765 6e65  Repository__gene
+00001be0: 7261 7465 5f73 7562 5f70 6970 5f72 6571  rate_sub_pip_req
+00001bf0: 73da 046c 6973 74da 0569 7465 6d73 726a  s..list..itemsrj
+00001c00: 0000 00da 0661 7070 656e 64da 0464 6963  .....append..dic
+00001c10: 7472 8300 0000 724d 0000 0072 0500 0000  tr....rM...r....
+00001c20: da05 7370 6c69 7472 0e00 0000 7216 0000  ..splitr....r...
+00001c30: 0072 2200 0000 7223 0000 0072 2a00 0000  .r"...r#...r*...
+00001c40: 7224 0000 0072 2b00 0000 725c 0000 0072  r$...r+...r\...r
+00001c50: 2c00 0000 da04 6c6f 6164 da06 7570 6461  ,.....load..upda
+00001c60: 7465 da06 736f 7274 6564 7247 0000 0072  te..sortedrG...r
+00001c70: 2d00 0000 da08 7461 6275 6c61 7465 7227  -.....tabulater'
+00001c80: 0000 0029 1272 1100 0000 7238 0000 0072  ...).r....r8...r
+00001c90: 3900 0000 da07 6d6f 6475 6c65 73da 0574  9.....modules..t
+00001ca0: 6162 6c65 da05 7661 6c75 65da 0464 6570  able..value..dep
+00001cb0: 735a 0862 6173 655f 7572 6c5a 0975 7365  sZ.base_urlZ.use
+00001cc0: 725f 6e61 6d65 5a09 7265 706f 5f6e 616d  r_nameZ.repo_nam
+00001cd0: 6572 7100 0000 7223 0000 005a 0864 6570  erq...r#...Z.dep
+00001ce0: 5f70 6174 6872 3200 0000 727d 0000 005a  _pathr2...r}...Z
+00001cf0: 066c 7461 626c 655a 076e 6577 5f64 6570  .ltableZ.new_dep
+00001d00: 5a0b 6c61 7465 785f 7461 626c 6572 1200  Z.latex_tabler..
+00001d10: 0000 726d 0000 0072 1300 0000 5a08 5f5f  ..rm...r....Z.__
+00001d20: 6578 706f 7274 a400 0000 73dc 0000 0008  export....s.....
+00001d30: 0208 0204 0210 020c 011a 010c 010e 0106  ................
+00001d40: 0108 ff02 800e 0506 0306 020e 010e 0108  ................
+00001d50: 0122 0402 fe02 0102 ff2a 0502 fe02 0102  .".......*......
+00001d60: ff0c 0520 0502 fe02 0102 ff02 8008 0506  ... ............
+00001d70: 0114 0104 ff06 0314 0104 ff0c 040c 010e  ................
+00001d80: 011c ff0e 020c 010a 011c 0112 0202 801e  ................
+00001d90: fc0a 0806 0106 010a ff10 040e 0302 020a  ................
+00001da0: 0106 ff0e 030c 0308 0112 0102 ff1e ff04  ................
+00001db0: 0904 0a0c 0412 011e ff08 030a 0204 020c  ................
+00001dc0: 010a 0104 010e 0104 0106 0206 0106 0102  ................
+00001dd0: 0104 fc08 ff04 0906 0206 0106 0106 0104  ................
+00001de0: fc08 ff04 0b02 0102 0102 0102 0106 fc04  ................
+00001df0: 0802 0102 0102 0102 0102 0106 fb0c 0a0c  ................
+00001e00: 011e ff0c 030c 011e ff0c 037a 194d 6f64  ...........z.Mod
+00001e10: 756c 6552 6570 6f73 6974 6f72 792e 5f5f  uleRepository.__
+00001e20: 6578 706f 7274 6301 0000 0000 0000 0000  exportc.........
+00001e30: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
+00001e40: 8a00 0000 7c00 6a00 6a01 7d01 7c00 a002  ....|.j.j.}.|...
+00001e50: 7c01 a101 0100 7403 a004 6401 a101 4400  |.....t...d...D.
+00001e60: 5d34 7d02 7c02 a005 6401 a101 7320 7c02  ]4}.|...d...s |.
+00001e70: a005 6402 a101 7320 7c02 7c00 6a00 6a01  ..d...s |.|.j.j.
+00001e80: 6b02 7221 710e 7403 6a06 a007 6401 7c02  k.r!q.t.j...d.|.
+00001e90: a102 7d03 7403 6a06 a008 7c03 a101 7242  ..}.t.j...|...rB
+00001ea0: 7403 6a06 a007 6401 7c02 6403 a103 7d04  t.j...d.|.d...}.
+00001eb0: 7403 6a06 a009 7c04 a101 733d 710e 7c00  t.j...|...s=q.|.
+00001ec0: a00a 7c03 a101 0100 710e 6400 5300 2904  ..|.....q.d.S.).
+00001ed0: 4e72 4600 0000 7262 0000 0072 1b00 0000  NrF...rb...r....
+00001ee0: 290b 720e 0000 0072 1600 0000 7265 0000  ).r....r....re..
+00001ef0: 0072 2200 0000 7248 0000 0072 6300 0000  .r"...rH...rc...
+00001f00: 7223 0000 0072 2a00 0000 7249 0000 0072  r#...r*...rI...r
+00001f10: 2400 0000 7264 0000 0072 6600 0000 7212  $...rd...rf...r.
+00001f20: 0000 0072 1200 0000 7213 0000 005a 175f  ...r....r....Z._
+00001f30: 5f67 656e 6572 6174 655f 7375 625f 7069  _generate_sub_pi
+00001f40: 705f 7265 7173 4401 0000 7322 0000 0008  p_reqsD...s"....
+00001f50: 020a 010e 0208 0202 ff08 0202 fe0c 0302  ................
+00001f60: 020e 010c 0110 020c 0102 010a 0102 8004  ................
+00001f70: f37a 284d 6f64 756c 6552 6570 6f73 6974  .z(ModuleReposit
+00001f80: 6f72 792e 5f5f 6765 6e65 7261 7465 5f73  ory.__generate_s
+00001f90: 7562 5f70 6970 5f72 6571 7363 0200 0000  ub_pip_reqsc....
+00001fa0: 0000 0000 0000 0000 0e00 0000 0a00 0000  ................
+00001fb0: 0300 0000 736e 0200 0064 0164 0284 0074  ....sn...d.d...t
+00001fc0: 00a0 0188 01a1 0144 0083 017d 0264 0364  .......D...}.d.d
+00001fd0: 0284 007c 0244 0083 0164 0464 0284 0074  ...|.D...d.d...t
+00001fe0: 00a0 0188 01a1 0144 0083 0117 0089 0087  .......D........
+00001ff0: 0166 0164 0564 0284 087c 0244 0083 017d  .f.d.d...|.D...}
+00002000: 0374 0264 0664 0284 007c 0344 0083 0183  .t.d.d...|.D....
+00002010: 017d 0387 0066 0164 0764 0284 087c 0344  .}...f.d.d...|.D
+00002020: 0083 017d 0374 0383 007d 047c 0464 0075  ...}.t...}.|.d.u
+00002030: 0072 4374 0464 0883 0101 0064 0053 0074  .rCt.d.....d.S.t
+00002040: 0283 007d 057c 0344 005d 5d7d 067c 06a0  ...}.|.D.]]}.|..
+00002050: 0564 09a1 0172 5071 487c 006a 066a 0767  .d...rPqH|.j.j.g
+00002060: 017c 06a0 0864 0aa1 01a2 017d 077c 0764  .|...d.....}.|.d
+00002070: 0b19 0064 0917 007c 0764 0b3c 0067 007c  ...d...|.d.<.g.|
+00002080: 06a0 0864 0aa1 01a2 017d 0874 006a 09a0  ...d.....}.t.j..
+00002090: 0a74 006a 096a 0b7c 078e 00a1 0172 7d64  .t.j.j.|.....r}d
+000020a0: 0ca0 0b7c 0764 0064 0b85 0219 00a1 017d  ...|.d.d.......}
+000020b0: 096e 1d74 006a 09a0 0a74 006a 096a 0b7c  .n.t.j...t.j.j.|
+000020c0: 088e 00a1 0172 8e7c 0864 0d19 0064 0c17  .....r.|.d...d..
+000020d0: 007d 096e 0c7c 006a 066a 0764 0c17 007c  .}.n.|.j.j.d...|
+000020e0: 06a0 0c64 0a64 0ca1 0217 007d 097c 0472  ...d.d.....}.|.r
+000020f0: a07c 047c 0917 007d 097c 05a0 0d7c 09a1  .|.|...}.|...|..
+00002100: 0101 0071 4874 0e7c 0583 0164 0d6b 0272  ...qHt.|...d.k.r
+00002110: ae64 0053 007a 3774 006a 09a0 0b88 0164  .d.S.z7t.j.....d
+00002120: 0ea1 027d 0a74 006a 09a0 0a7c 0aa1 0172  ...}.t.j...|...r
+00002130: e274 0f7c 0a64 0f83 028f 187d 0b74 10a0  .t.|.d.....}.t..
+00002140: 117c 0ba1 017d 0a64 107c 0a76 0072 d07c  .|...}.d.|.v.r.|
+00002150: 0a64 1019 007d 0c6e 0269 007d 0c57 0064  .d...}.n.i.}.W.d
+00002160: 0004 0004 0083 0301 006e 0831 0073 dc77  .........n.1.s.w
+00002170: 0101 0001 0001 0059 0001 006e 0269 007d  .......Y...n.i.}
+00002180: 0c57 006e 1d04 0074 1290 0179 0201 007d  .W.n...t...y...}
+00002190: 0d01 007a 1074 0464 1188 019b 0064 129d  ...z.t.d.....d..
+000021a0: 0383 0101 0069 007d 0c57 0059 0064 007d  .....i.}.W.Y.d.}
+000021b0: 0d7e 0d6e 0564 007d 0d7e 0d77 0177 0074  .~.n.d.}.~.w.w.t
+000021c0: 0f74 006a 09a0 0b88 0164 0ea1 0264 1383  .t.j.....d...d..
+000021d0: 028f 1f7d 0b74 137c 0583 017c 0c64 149c  ...}.t.|...|.d..
+000021e0: 027d 0574 106a 147c 057c 0b64 1564 168d  .}.t.j.|.|.d.d..
+000021f0: 0301 0074 0464 1788 019b 009d 0283 0101  ...t.d..........
+00002200: 0057 0064 0004 0004 0083 0301 0064 0053  .W.d.........d.S
+00002210: 0031 0090 0173 3077 0101 0001 0001 0059  .1...s0w.......Y
+00002220: 0001 0064 0053 0029 184e 6301 0000 0000  ...d.S.).Nc.....
+00002230: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00002240: 0000 0073 2200 0000 6700 7c00 5d0d 7d01  ...s"...g.|.].}.
+00002250: 7c01 a000 6400 a101 720f 6401 7c01 7601  |...d...r.d.|.v.
+00002260: 7202 7c01 9102 7102 5300 2902 fa03 2e70  r.|...q.S.)....p
+00002270: 7972 6200 0000 2901 da08 656e 6473 7769  yrb...)...endswi
+00002280: 7468 a902 7254 0000 0072 3200 0000 7212  th..rT...r2...r.
+00002290: 0000 0072 1200 0000 7213 0000 0072 5600  ...r....r....rV.
+000022a0: 0000 5b01 0000 730c 0000 0008 0008 0102  ..[...s.........
+000022b0: ff08 0102 ff06 017a 414d 6f64 756c 6552  .......zAModuleR
+000022c0: 6570 6f73 6974 6f72 792e 5f5f 6765 6e65  epository.__gene
+000022d0: 7261 7465 5f6d 6174 655f 6465 7065 6e64  rate_mate_depend
+000022e0: 656e 6369 6573 2e3c 6c6f 6361 6c73 3e2e  encies.<locals>.
+000022f0: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
+00002300: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
+00002310: 0000 0072 7900 0000 2902 7298 0000 0072  ...ry...).r....r
+00002320: 4400 0000 727a 0000 00a9 0272 5400 0000  D...rz.....rT...
+00002330: da04 6669 6c65 7212 0000 0072 1200 0000  ..filer....r....
+00002340: 7213 0000 0072 5600 0000 5d01 0000 725a  r....rV...]...rZ
+00002350: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002360: 0200 0000 0400 0000 5300 0000 727e 0000  ........S...r~..
+00002370: 0029 0172 6200 0000 7212 0000 0072 9a00  .).rb...r....r..
+00002380: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00002390: 0072 5600 0000 5d01 0000 7304 0000 0006  .rV...]...s.....
+000023a0: 0012 0163 0100 0000 0000 0000 0000 0000  ...c............
+000023b0: 0200 0000 0700 0000 1300 0000 731e 0000  ............s...
+000023c0: 0067 007c 005d 0b7d 0174 0074 016a 02a0  .g.|.].}.t.t.j..
+000023d0: 0388 007c 01a1 0283 0191 0271 0253 0072  ...|.......q.S.r
+000023e0: 1200 0000 2904 7204 0000 0072 2200 0000  ....).r....r"...
+000023f0: 7223 0000 0072 2a00 0000 729a 0000 0029  r#...r*...r....)
+00002400: 0172 2300 0000 7212 0000 0072 1300 0000  .r#...r....r....
+00002410: 7256 0000 0061 0100 0073 0a00 0000 0600  rV...a...s......
+00002420: 0201 02ff 0c01 08ff 6301 0000 0000 0000  ........c.......
+00002430: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
+00002440: 0072 6f00 0000 7212 0000 0072 1200 0000  .ro...r....r....
+00002450: 7270 0000 0072 1200 0000 7212 0000 0072  rp...r....r....r
+00002460: 1300 0000 7256 0000 0065 0100 0072 7200  ....rV...e...rr.
+00002470: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00002480: 0000 0006 0000 0013 0000 0073 2600 0000  ...........s&...
+00002490: 6700 7c00 5d0f 8900 7400 8700 6601 6400  g.|.]...t...f.d.
+000024a0: 6401 8408 8801 4400 8301 8301 7302 8800  d.....D.....s...
+000024b0: 9102 7102 5300 2902 6301 0000 0000 0000  ..q.S.).c.......
+000024c0: 0000 0000 0002 0000 0004 0000 0013 0000  ................
+000024d0: 0073 1400 0000 6700 7c00 5d06 7d01 7c01  .s....g.|.].}.|.
+000024e0: 8800 7600 9102 7102 5300 7212 0000 0072  ..v...q.S.r....r
+000024f0: 1200 0000 729b 0000 00a9 01da 066d 6f64  ....r........mod
+00002500: 756c 6572 1200 0000 7213 0000 0072 5600  uler....r....rV.
+00002510: 0000 6b01 0000 7302 0000 0014 007a 4c4d  ..k...s......zLM
+00002520: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
+00002530: 5f5f 6765 6e65 7261 7465 5f6d 6174 655f  __generate_mate_
+00002540: 6465 7065 6e64 656e 6369 6573 2e3c 6c6f  dependencies.<lo
+00002550: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00002560: 2e3c 6c69 7374 636f 6d70 3e29 01da 0361  .<listcomp>)...a
+00002570: 6e79 2901 7254 0000 0029 01da 0e6f 7269  ny).rT...)...ori
+00002580: 6769 6e61 6c5f 6669 6c65 7372 9d00 0000  ginal_filesr....
+00002590: 7213 0000 0072 5600 0000 6801 0000 730c  r....rV...h...s.
+000025a0: 0000 0006 0002 0214 0102 fd02 0106 ff7a  ...............z
+000025b0: 2c4e 6f20 6769 7420 7572 6c20 666f 756e  ,No git url foun
+000025c0: 642c 2073 6b69 7070 696e 6720 6465 7065  d, skipping depe
+000025d0: 6e64 656e 6369 6573 2e6a 736f 6e72 9800  ndencies.jsonr..
+000025e0: 0000 7246 0000 00e9 ffff ffff 7273 0000  ..rF........rs..
+000025f0: 0072 0100 0000 7277 0000 0072 5200 0000  .r....rw...rR...
+00002600: da03 656e 767a 0e45 7272 6f72 2072 6561  ..envz.Error rea
+00002610: 6469 6e67 207a 202f 6465 7065 6e64 656e  ding z /dependen
+00002620: 6369 6573 2e6a 736f 6e2c 2073 6b69 7070  cies.json, skipp
+00002630: 696e 6720 656e 7672 1700 0000 2902 7278  ing envr....).rx
+00002640: 0000 0072 a200 0000 7218 0000 0072 1900  ...r....r....r..
+00002650: 0000 7a20 4765 6e65 7261 7465 6420 6465  ..z Generated de
+00002660: 7065 6e64 656e 6369 6573 2e6a 736f 6e20  pendencies.json 
+00002670: 666f 7220 2915 7222 0000 0072 4800 0000  for ).r"...rH...
+00002680: 724d 0000 0072 0500 0000 7227 0000 0072  rM...r....r'...r
+00002690: 9900 0000 720e 0000 0072 1600 0000 728f  ....r....r....r.
+000026a0: 0000 0072 2300 0000 7224 0000 0072 2a00  ...r#...r$...r*.
+000026b0: 0000 727b 0000 0072 4e00 0000 725d 0000  ..r{...rN...r]..
+000026c0: 0072 2b00 0000 722c 0000 0072 9000 0000  .r+...r,...r....
+000026d0: 7231 0000 0072 8b00 0000 722d 0000 0029  r1...r....r-...)
+000026e0: 0e72 1100 0000 7223 0000 00da 0566 696c  .r....r#.....fil
+000026f0: 6573 5a10 7265 6c61 7469 7665 5f69 6d70  esZ.relative_imp
+00002700: 6f72 7473 5a07 7572 6c5f 6769 7472 9700  ortsZ.url_gitr..
+00002710: 0000 729e 0000 005a 0574 7061 7468 5a12  ..r....Z.tpathZ.
+00002720: 7369 7374 6572 5f6d 6f64 756c 655f 7061  sister_module_pa
+00002730: 7468 7236 0000 005a 0964 6570 735f 6a73  thr6...Z.deps_js
+00002740: 6f6e 7232 0000 0072 a200 0000 7234 0000  onr2...r....r4..
+00002750: 0072 1200 0000 2902 72a0 0000 0072 2300  .r....).r....r#.
+00002760: 0000 7213 0000 005a 1c5f 5f67 656e 6572  ..r....Z.__gener
+00002770: 6174 655f 6d61 7465 5f64 6570 656e 6465  ate_mate_depende
+00002780: 6e63 6965 7358 0100 0073 7600 0000 0a03  nciesX...sv.....
+00002790: 0201 08ff 1202 0801 08ff 0a04 0201 06ff  ................
+000027a0: 0203 0c01 04ff 0a04 0202 06fe 0606 0802  ................
+000027b0: 0801 0401 0602 0801 0a02 0201 1403 1001  ................
+000027c0: 0e02 1402 1402 1401 0e01 1802 0402 0801  ................
+000027d0: 0c01 0c02 0401 0202 0e02 0c01 0c01 0a02  ................
+000027e0: 0801 0a01 0402 0280 1cfa 0280 0409 0480  ................
+000027f0: 1001 1001 1001 0880 02fe 1604 0e01 1001  ................
+00002800: 1001 24fd 7a2d 4d6f 6475 6c65 5265 706f  ..$.z-ModuleRepo
+00002810: 7369 746f 7279 2e5f 5f67 656e 6572 6174  sitory.__generat
+00002820: 655f 6d61 7465 5f64 6570 656e 6465 6e63  e_mate_dependenc
+00002830: 6965 7363 0200 0000 0000 0000 0000 0000  iesc............
+00002840: 0900 0000 0600 0000 4300 0000 73b8 0000  ........C...s...
+00002850: 0074 00a0 017c 01a1 017d 0274 00a0 027c  .t...|...}.t...|
+00002860: 02a1 017d 037c 00a0 037c 01a1 0101 0067  ...}.|...|.....g
+00002870: 007d 047c 017c 006a 046a 056b 0272 2474  .}.|.|.j.j.k.r$t
+00002880: 00a0 0664 017c 0364 02a1 0301 007c 00a0  ...d.|.d.....|..
+00002890: 0764 01a1 0101 006e 1d74 00a0 0674 086a  .d.....n.t...t.j
+000028a0: 09a0 0a7c 0164 01a1 027c 0364 02a1 0301  ...|.d...|.d....
+000028b0: 007c 00a0 0774 086a 09a0 0a7c 0164 01a1  .|...t.j...|.d..
+000028c0: 02a1 0101 0074 0b64 037c 019b 009d 0283  .....t.d.|......
+000028d0: 0101 007c 0344 005d 147d 057c 0564 0419  ...|.D.].}.|.d..
+000028e0: 007d 067c 0564 0519 007d 077c 067c 0764  .}.|.d...}.|.|.d
+000028f0: 069c 027d 087c 04a0 0c7c 08a1 0101 0071  ...}.|...|.....q
+00002900: 4364 077c 0469 0153 0029 084e 7276 0000  Cd.|.i.S.).Nrv..
+00002910: 007a 027e 3d7a 1f47 656e 6572 6174 6564  .z.~=z.Generated
+00002920: 2072 6571 7569 7265 6d65 6e74 732e 7478   requirements.tx
+00002930: 7420 666f 7220 726b 0000 00da 0776 6572  t for rk.....ver
+00002940: 7369 6f6e 2902 726b 0000 0072 a400 0000  sion).rk...r....
+00002950: da03 7069 7029 0d72 0800 0000 5a0f 6765  ..pip).r....Z.ge
+00002960: 745f 616c 6c5f 696d 706f 7274 735a 1067  t_all_importsZ.g
+00002970: 6574 5f69 6d70 6f72 745f 6c6f 6361 6cda  et_import_local.
+00002980: 2d5f 4d6f 6475 6c65 5265 706f 7369 746f  -_ModuleReposito
+00002990: 7279 5f5f 6765 6e65 7261 7465 5f6d 6174  ry__generate_mat
+000029a0: 655f 6465 7065 6e64 656e 6369 6573 720e  e_dependenciesr.
+000029b0: 0000 0072 1600 0000 5a1a 6765 6e65 7261  ...r....Z.genera
+000029c0: 7465 5f72 6571 7569 7265 6d65 6e74 735f  te_requirements_
+000029d0: 6669 6c65 da30 5f4d 6f64 756c 6552 6570  file.0_ModuleRep
+000029e0: 6f73 6974 6f72 795f 5f61 6464 5f69 6e64  ository__add_ind
+000029f0: 6578 5f75 726c 5f74 6f5f 7265 7175 6972  ex_url_to_requir
+00002a00: 656d 656e 7473 7222 0000 0072 2300 0000  ementsr"...r#...
+00002a10: 722a 0000 0072 2700 0000 728d 0000 0029  r*...r'...r....)
+00002a20: 0972 1100 0000 7223 0000 00da 0769 6d70  .r....r#.....imp
+00002a30: 6f72 7473 5a11 696d 706f 7274 5f69 6e66  ortsZ.import_inf
+00002a40: 6f5f 6c6f 6361 6c5a 0b69 6d70 6f72 745f  o_localZ.import_
+00002a50: 696e 666f 5a02 696d 726b 0000 0072 a400  infoZ.imrk...r..
+00002a60: 0000 da03 7265 7372 1200 0000 7212 0000  ....resr....r...
+00002a70: 0072 1300 0000 5a1b 5f5f 6765 6e65 7261  .r....Z.__genera
+00002a80: 7465 5f70 6970 5f72 6571 7569 7265 6d65  te_pip_requireme
+00002a90: 6e74 73a6 0100 0073 3000 0000 0a03 0a03  nts....s0.......
+00002aa0: 0a02 0402 0c02 0401 0601 04ff 0c03 0403  ................
+00002ab0: 1001 04ff 0403 0c01 04ff 0e02 0802 0802  ................
+00002ac0: 0801 0203 0201 06fe 0c05 0802 7a2c 4d6f  ............z,Mo
+00002ad0: 6475 6c65 5265 706f 7369 746f 7279 2e5f  duleRepository._
+00002ae0: 5f67 656e 6572 6174 655f 7069 705f 7265  _generate_pip_re
+00002af0: 7175 6972 656d 656e 7473 729e 0000 0063  quirementsr....c
+00002b00: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00002b10: 0300 0000 4300 0000 731e 0000 007c 0164  ....C...s....|.d
+00002b20: 006b 0272 097c 006a 00a0 01a1 0053 007c  .k.r.|.j.....S.|
+00002b30: 006a 00a0 027c 01a1 0153 0072 0d00 0000  .j...|...S.r....
+00002b40: 2903 7210 0000 00da 0773 756d 6d61 7279  ).r......summary
+00002b50: 728b 0000 0029 0272 1100 0000 729e 0000  r....).r....r...
+00002b60: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00002b70: 728b 0000 00ce 0100 0073 0600 0000 0801  r........s......
+00002b80: 0a01 0c01 7a15 4d6f 6475 6c65 5265 706f  ....z.ModuleRepo
+00002b90: 7369 746f 7279 2e6c 6973 7463 0100 0000  sitory.listc....
+00002ba0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00002bb0: 4300 0000 730a 0000 007c 006a 00a0 01a1  C...s....|.j....
+00002bc0: 0053 0072 0d00 0000 2902 7210 0000 0072  .S.r....).r....r
+00002bd0: aa00 0000 2901 7211 0000 0072 1200 0000  ....).r....r....
+00002be0: 7212 0000 0072 1300 0000 da10 6765 745f  r....r......get_
+00002bf0: 6d61 7465 5f73 756d 6d61 7279 d301 0000  mate_summary....
+00002c00: 7302 0000 000a 017a 214d 6f64 756c 6552  s......z!ModuleR
+00002c10: 6570 6f73 6974 6f72 792e 6765 745f 6d61  epository.get_ma
+00002c20: 7465 5f73 756d 6d61 7279 da07 7061 636b  te_summary..pack
+00002c30: 6167 6563 0200 0000 0000 0000 0000 0000  agec............
+00002c40: 0200 0000 0300 0000 4300 0000 7310 0000  ........C...s...
+00002c50: 007c 006a 00a0 017c 01a1 0101 0064 0053  .|.j...|.....d.S
+00002c60: 0072 0d00 0000 2902 7210 0000 0072 3700  .r....).r....r7.
+00002c70: 0000 2902 7211 0000 0072 ac00 0000 7212  ..).r....r....r.
+00002c80: 0000 0072 1200 0000 7213 0000 0072 3700  ...r....r....r7.
+00002c90: 0000 d601 0000 7302 0000 0010 017a 204d  ......s......z M
+00002ca0: 6f64 756c 6552 6570 6f73 6974 6f72 792e  oduleRepository.
+00002cb0: 696e 7374 616c 6c5f 7061 636b 6167 6529  install_package)
+00002cc0: 0146 720d 0000 0029 16da 085f 5f6e 616d  .Fr....)...__nam
+00002cd0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00002ce0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0462  .__qualname__..b
+00002cf0: 6f6f 6c72 1400 0000 da0c 7374 6174 6963  oolr......static
+00002d00: 6d65 7468 6f64 da03 7374 7272 3500 0000  method..strr5...
+00002d10: 723a 0000 0072 4200 0000 7241 0000 0072  r:...rB...rA...r
+00002d20: 8b00 0000 7260 0000 0072 a700 0000 7265  ....r`...r....re
+00002d30: 0000 0072 4000 0000 728a 0000 0072 a600  ...r@...r....r..
+00002d40: 0000 7264 0000 0072 ab00 0000 7209 0000  ..rd...r....r...
+00002d50: 0072 3700 0000 7212 0000 0072 1200 0000  .r7...r....r....
+00002d60: 7212 0000 0072 1300 0000 720b 0000 0014  r....r....r.....
+00002d70: 0000 0073 2400 0000 0800 1001 0207 1001  ...s$...........
+00002d80: 0e2a 0e04 1006 1212 0e0e 081d 0816 007f  .*..............
+00002d90: 0821 0814 084e 1028 0805 1203 720b 0000  .!...N.(....r...
+00002da0: 0029 1672 2c00 0000 7222 0000 0072 5e00  .).r,...r"...r^.
+00002db0: 0000 7228 0000 0072 9300 0000 5a0e 6d6f  ..r(...r....Z.mo
+00002dc0: 6475 6c65 5f6d 616e 6167 6572 7203 0000  dule_managerr...
+00002dd0: 005a 0e75 7469 6c73 2e65 7870 5f75 7469  .Z.utils.exp_uti
+00002de0: 6c72 0400 0000 5a0e 7574 696c 732e 6769  lr....Z.utils.gi
+00002df0: 745f 7574 696c 7205 0000 005a 0e73 6f75  t_utilr....Z.sou
+00002e00: 7263 6573 2e72 656d 6f74 6572 0600 0000  rces.remoter....
+00002e10: 5a13 736f 7572 6365 732e 6c6f 6361 6c2e  Z.sources.local.
+00002e20: 6c6f 6361 6c72 0700 0000 7208 0000 0072  localr....r....r
+00002e30: ac00 0000 7209 0000 00da 0674 7970 696e  ....r......typin
+00002e40: 6772 0a00 0000 da04 6970 6462 720b 0000  gr......ipdbr...
+00002e50: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00002e60: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00002e70: 0000 0073 1e00 0000 0800 0801 0801 0801  ...s............
+00002e80: 0802 0c02 0c01 0c01 0c01 0c01 0c01 0c02  ................
+00002e90: 0c01 0801 1203                           ......
```

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/__pycache__/package.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/module_manager.py` & `yerbamate-0.9.235/packages/yerbamate/api/data/module_manager.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/module_repository.py` & `yerbamate-0.9.235/packages/yerbamate/api/data/module_repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,21 +169,23 @@
 
         table = []
 
         for key, value in modules.items():
             if type(value) is list:
                 table.append([{"type": key, "name": name} for name in value])
             elif type(value) is dict:
-                table.append([{"type": key, "name": name} for name in value.keys()])
+                table.append([{"type": key, "name": name}
+                             for name in value.keys()])
 
         # ipdb.set_trace()
 
         table = [item for sublist in table for item in sublist]
 
         # add url to each item in table
+        deps = set()
 
         base_url = parse_url_from_git()
         user_name = base_url.split("/")[3]
         repo_name = base_url.split("/")[4]
         for item in table:
 
             item[
@@ -215,39 +217,55 @@
                     item["dependencies"] = f.readlines()
             if os.path.exists(dep_path):
                 with open(dep_path, "r") as f:
                     if "dependencies" in item:
                         item["dependencies"] += json.load(f)["dependencies"]
                     else:
                         item["dependencies"] = json.load(f)["dependencies"]
+
                     # item["module_dependencies"] = json.load(f)
 
             if "dependencies" in item:
                 item["dependencies"] = [
                     dep.replace("\n", "") for dep in item["dependencies"]
                 ]
 
-        # create latex table
+            deps.update(item["dependencies"])
 
-        # ipdb.set_trace()
-        # l_table = [t for t in table if t["type"] == "models"]
-        # remove url from table
+        # remove github urls from dependencies
+        deps = [dep for dep in deps if not "https://github" in dep]
+        # set index urls should be on top, sort so that --extra-index-url is on top
+        deps = sorted(
+            deps, key=lambda x: "--extra-index-url" in x, reverse=True)
+        # remove empty lines
+        deps = [dep for dep in deps if dep != "\n" or dep != " " or dep != ""]
+
+        # save deps in requirements.txt
+        with open("requirements.txt", "w") as f:
+            for dep in deps:
+                f.write(dep + "\n")
+
+            # create latex table
+
+            # ipdb.set_trace()
+            # l_table = [t for t in table if t["type"] == "models"]
+            # remove url from table
         ltable = table
         # for item in ltable:
         #     del item["url"]
         #     for dep in item["dependencies"]:
         #         if "--extra" in dep:
         #             item["dependencies"].remove(dep)
         #         # if "https" in dep:
 
-
         # create latex table
         # recreate table to remove url
         ltable = []
 
+        # combine dependenices, make a set, remove urls, and save as requirements.txt
 
         with open("exports.json", "w") as f:
             json.dump(table, f, indent=4)
 
         for item in table:
             # remove --extra from dep
             if "dependencies" in item:
@@ -297,15 +315,14 @@
 
         with open("export.md", "w") as f:
             f.write(table)
 
         with open("exports.tex", "w") as f:
             f.write(latex_table)
 
-
         print("Exported to export.md")
 
     def __generate_sub_pip_reqs(self):
 
         root_path = self.config.project
         self.__generate_deps_in_depth(root_path)
 
@@ -323,20 +340,22 @@
                 if not os.path.exists(init__path):
                     continue
                 self.__generate_pip_requirements(path)
 
     def __generate_mate_dependencies(self, path):
         # ipdb.set_trace()
 
-        files = [f for f in os.listdir(path) if f.endswith(".py") and "__" not in f]
+        files = [f for f in os.listdir(
+            path) if f.endswith(".py") and "__" not in f]
         original_files = [file.replace(".py", "") for file in files] + [
             f for f in os.listdir(path) if "__" not in f
         ]
 
-        relative_imports = [get_relative_imports(os.path.join(path, f)) for f in files]
+        relative_imports = [get_relative_imports(
+            os.path.join(path, f)) for f in files]
         # flatten array to unique set
         relative_imports = set(
             [item for sublist in relative_imports for item in sublist]
         )
 
         relative_imports = [
             module
@@ -418,15 +437,16 @@
             )
             self.__add_index_url_to_requirements("requirements.txt")
 
         else:
             pipreqs.generate_requirements_file(
                 os.path.join(path, "requirements.txt"), import_info_local, "~="
             )
-            self.__add_index_url_to_requirements(os.path.join(path, "requirements.txt"))
+            self.__add_index_url_to_requirements(
+                os.path.join(path, "requirements.txt"))
             print(f"Generated requirements.txt for {path}")
 
         for im in import_info_local:
 
             name = im["name"]
             version = im["version"]
```

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/package.py` & `yerbamate-0.9.235/packages/yerbamate/api/data/package.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/sources/__pycache__/source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/__pycache__/io.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/__pycache__/local.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/io.py` & `yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/io.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/sources/local/local.py` & `yerbamate-0.9.235/packages/yerbamate/api/data/sources/local/local.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/sources/remote/__pycache__/remote.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/sources/remote/remote.py` & `yerbamate-0.9.235/packages/yerbamate/api/data/sources/remote/remote.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/utils/__pycache__/exp_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/utils/__pycache__/git_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/api/data/utils/__pycache__/gitdir.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/utils/git_util.py` & `yerbamate-0.9.235/packages/yerbamate/api/data/utils/git_util.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/data/utils/gitdir.py` & `yerbamate-0.9.235/packages/yerbamate/api/data/utils/gitdir.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/api/mate_api.py` & `yerbamate-0.9.235/packages/yerbamate/api/mate_api.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/environment.py` & `yerbamate-0.9.235/packages/yerbamate/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.hparams = {}
 
         # set command to True
         try:
             setattr(self, sys.argv[1], True)
         except:
             pass
-        
+
         self.args = sys.argv[1:]
 
         self._root = self.__find_root()
 
         # parse python -m module train arg=1 arg2=2
         for arg in sys.argv:
             if "=" not in arg:
@@ -174,17 +174,21 @@
             sys.exit(1)
 
         setattr(self, "env", env)
 
     def __getitem__(self, key):
         if not key in self:
             # ipdb.set_trace()
+            res = os.environ.get(key, None)
+
+            if res is not None:
+                return res
+
             if key in self.env:
                 return self.env[key]
-            res = os.environ.get(key, None)
 
             if res is None or res == "":
                 print(
                     f"Environment variable {key} not found. Set it in env.json or in your shell.")
                 print("Exiting...")
                 sys.exit(1)
             else:
```

### Comparing `yerbamate-0.9.23/packages/yerbamate/mate.py` & `yerbamate-0.9.235/packages/yerbamate/mate.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/mate_cli.py` & `yerbamate-0.9.235/packages/yerbamate/mate_cli.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/utils/__init__.py` & `yerbamate-0.9.235/packages/yerbamate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/utils/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/utils/__pycache__/bunch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc` & `yerbamate-0.9.235/packages/yerbamate/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/utils/bunch.py` & `yerbamate-0.9.235/packages/yerbamate/utils/bunch.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/utils/git_url_parser.py` & `yerbamate-0.9.235/packages/yerbamate/utils/git_url_parser.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/utils/utils.py` & `yerbamate-0.9.235/packages/yerbamate/utils/utils.py`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate/yerbamate.egg-info/PKG-INFO` & `yerbamate-0.9.235/packages/yerbamate/yerbamate.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/packages/yerbamate.egg-info/PKG-INFO` & `yerbamate-0.9.235/packages/yerbamate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: yerbamate
-Version: 0.9.23
+Version: 0.9.235
 Summary:  A python module and experiment manager for deep learning
 Home-page: https://github.com/oalee/yerbamate
 Author: Giulio Zani, Ali Rahimi
 Author-email: yerba.mate.dl@proton.me
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 style="color:green"><span style="color:green">Maté 🧉</span> your modular AI project and experiment manager</h1>
 
 <!-- Maté is a python project, package and experiment manager. Whether you are a
 seasoned deep learning researcher or just starting out, Maté provides you with
```

### Comparing `yerbamate-0.9.23/packages/yerbamate.egg-info/SOURCES.txt` & `yerbamate-0.9.235/packages/yerbamate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yerbamate-0.9.23/setup.py` & `yerbamate-0.9.235/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 setup(
     name="yerbamate",
     description=" A python module and experiment manager for deep learning",
     author="Giulio Zani, Ali Rahimi",
     author_email="yerba.mate.dl@proton.me",
     url="https://github.com/oalee/yerbamate",
-    python_requires=">=3.8",
-    version="0.9.23",
+    python_requires=">=3.6",
+    version="0.9.235",
     packages=find_packages("packages", exclude=["tests"]),
     include_package_data=True,
     package_dir={"": "packages/"},
     license="Apache License 2.0",
     license_files=("LICENSE",),
     long_description=long_description,
     long_description_content_type='text/markdown',
```

