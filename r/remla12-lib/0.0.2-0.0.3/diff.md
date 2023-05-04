# Comparing `tmp/remla12-lib-0.0.2.tar.gz` & `tmp/remla12-lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla12-lib-0.0.2.tar", last modified: Thu May  4 18:30:46 2023, max compression
+gzip compressed data, was "remla12-lib-0.0.3.tar", last modified: Thu May  4 18:36:28 2023, max compression
```

## Comparing `remla12-lib-0.0.2.tar` & `remla12-lib-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:30:46.206689 remla12-lib-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 18:30:46.206689 remla12-lib-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-04 18:30:34.000000 remla12-lib-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:30:46.206689 remla12-lib-0.0.2/remla12_lib/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 18:30:34.000000 remla12-lib-0.0.2/remla12_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-04 18:30:34.000000 remla12-lib-0.0.2/remla12_lib/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:30:46.206689 remla12-lib-0.0.2/remla12_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 18:30:46.000000 remla12-lib-0.0.2/remla12_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 18:30:46.000000 remla12-lib-0.0.2/remla12_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:30:46.000000 remla12-lib-0.0.2/remla12_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 18:30:46.000000 remla12-lib-0.0.2/remla12_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:30:46.206689 remla12-lib-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-04 18:30:34.000000 remla12-lib-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:36:28.930293 remla12-lib-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 18:36:28.930293 remla12-lib-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-04 18:36:06.000000 remla12-lib-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:36:28.930293 remla12-lib-0.0.3/remla12_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 18:36:06.000000 remla12-lib-0.0.3/remla12_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-04 18:36:06.000000 remla12-lib-0.0.3/remla12_lib/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:36:28.930293 remla12-lib-0.0.3/remla12_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-04 18:36:28.000000 remla12-lib-0.0.3/remla12_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 18:36:28.000000 remla12-lib-0.0.3/remla12_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:36:28.000000 remla12-lib-0.0.3/remla12_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 18:36:28.000000 remla12-lib-0.0.3/remla12_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:36:28.930293 remla12-lib-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-04 18:36:06.000000 remla12-lib-0.0.3/setup.py
```

