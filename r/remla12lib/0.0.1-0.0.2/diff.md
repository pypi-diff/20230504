# Comparing `tmp/remla12lib-0.0.1.tar.gz` & `tmp/remla12lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla12lib-0.0.1.tar", last modified: Thu May  4 21:35:47 2023, max compression
+gzip compressed data, was "remla12lib-0.0.2.tar", last modified: Thu May  4 21:41:15 2023, max compression
```

## Comparing `remla12lib-0.0.1.tar` & `remla12lib-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:35:47.404224 remla12lib-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 21:35:47.404224 remla12lib-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 21:35:30.000000 remla12lib-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:35:47.404224 remla12lib-0.0.1/remla12lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 21:35:47.000000 remla12lib-0.0.1/remla12lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 21:35:47.000000 remla12lib-0.0.1/remla12lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:35:47.000000 remla12lib-0.0.1/remla12lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:35:47.000000 remla12lib-0.0.1/remla12lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:35:47.404224 remla12lib-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 21:35:30.000000 remla12lib-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:41:15.099553 remla12lib-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 21:41:15.099553 remla12lib-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-04 21:40:44.000000 remla12lib-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:41:15.099553 remla12lib-0.0.2/remla12lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 21:41:15.000000 remla12lib-0.0.2/remla12lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 21:41:15.000000 remla12lib-0.0.2/remla12lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:41:15.000000 remla12lib-0.0.2/remla12lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:41:15.000000 remla12lib-0.0.2/remla12lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:41:15.099553 remla12lib-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 21:40:44.000000 remla12lib-0.0.2/setup.py
```

