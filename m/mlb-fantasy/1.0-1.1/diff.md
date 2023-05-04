# Comparing `tmp/mlb-fantasy-1.0.tar.gz` & `tmp/mlb-fantasy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlb-fantasy-1.0.tar", last modified: Thu May  4 18:57:21 2023, max compression
+gzip compressed data, was "mlb-fantasy-1.1.tar", last modified: Thu May  4 19:09:04 2023, max compression
```

## Comparing `mlb-fantasy-1.0.tar` & `mlb-fantasy-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 18:57:21.882309 mlb-fantasy-1.0/
--rw-r--r--   0 brian     (1000) brian     (1000)      183 2023-05-04 18:57:21.882309 mlb-fantasy-1.0/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      978 2023-04-24 12:00:54.000000 mlb-fantasy-1.0/README.md
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 18:57:21.882309 mlb-fantasy-1.0/mlb_fantasy/
--rw-r--r--   0 brian     (1000) brian     (1000)        0 2023-05-04 17:45:29.000000 mlb-fantasy-1.0/mlb_fantasy/__init__.py
--rw-r--r--   0 brian     (1000) brian     (1000)     2785 2023-05-04 17:47:13.000000 mlb-fantasy-1.0/mlb_fantasy/main.py
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 18:57:21.882309 mlb-fantasy-1.0/mlb_fantasy.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)      183 2023-05-04 18:57:21.000000 mlb-fantasy-1.0/mlb_fantasy.egg-info/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      274 2023-05-04 18:57:21.000000 mlb-fantasy-1.0/mlb_fantasy.egg-info/SOURCES.txt
--rw-r--r--   0 brian     (1000) brian     (1000)        1 2023-05-04 18:57:21.000000 mlb-fantasy-1.0/mlb_fantasy.egg-info/dependency_links.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       55 2023-05-04 18:57:21.000000 mlb-fantasy-1.0/mlb_fantasy.egg-info/entry_points.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       51 2023-05-04 18:57:21.000000 mlb-fantasy-1.0/mlb_fantasy.egg-info/requires.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       12 2023-05-04 18:57:21.000000 mlb-fantasy-1.0/mlb_fantasy.egg-info/top_level.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       38 2023-05-04 18:57:21.882309 mlb-fantasy-1.0/setup.cfg
--rw-r--r--   0 brian     (1000) brian     (1000)      431 2023-05-04 17:06:25.000000 mlb-fantasy-1.0/setup.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 19:09:04.312304 mlb-fantasy-1.1/
+-rw-r--r--   0 brian     (1000) brian     (1000)      354 2023-05-04 19:09:04.312304 mlb-fantasy-1.1/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      441 2023-05-04 18:59:19.000000 mlb-fantasy-1.1/README.md
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 19:09:04.312304 mlb-fantasy-1.1/mlb_fantasy/
+-rw-r--r--   0 brian     (1000) brian     (1000)        0 2023-05-04 17:45:29.000000 mlb-fantasy-1.1/mlb_fantasy/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     2785 2023-05-04 17:47:13.000000 mlb-fantasy-1.1/mlb_fantasy/main.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 19:09:04.312304 mlb-fantasy-1.1/mlb_fantasy.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)      354 2023-05-04 19:09:04.000000 mlb-fantasy-1.1/mlb_fantasy.egg-info/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      274 2023-05-04 19:09:04.000000 mlb-fantasy-1.1/mlb_fantasy.egg-info/SOURCES.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)        1 2023-05-04 19:09:04.000000 mlb-fantasy-1.1/mlb_fantasy.egg-info/dependency_links.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       55 2023-05-04 19:09:04.000000 mlb-fantasy-1.1/mlb_fantasy.egg-info/entry_points.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       51 2023-05-04 19:09:04.000000 mlb-fantasy-1.1/mlb_fantasy.egg-info/requires.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       12 2023-05-04 19:09:04.000000 mlb-fantasy-1.1/mlb_fantasy.egg-info/top_level.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       38 2023-05-04 19:09:04.312304 mlb-fantasy-1.1/setup.cfg
+-rw-r--r--   0 brian     (1000) brian     (1000)      629 2023-05-04 19:08:52.000000 mlb-fantasy-1.1/setup.py
```

### Comparing `mlb-fantasy-1.0/mlb_fantasy/main.py` & `mlb-fantasy-1.1/mlb_fantasy/main.py`

 * *Files identical despite different names*

