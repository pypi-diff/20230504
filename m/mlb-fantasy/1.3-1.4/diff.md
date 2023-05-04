# Comparing `tmp/mlb-fantasy-1.3.tar.gz` & `tmp/mlb-fantasy-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlb-fantasy-1.3.tar", last modified: Thu May  4 19:13:40 2023, max compression
+gzip compressed data, was "mlb-fantasy-1.4.tar", last modified: Thu May  4 19:15:26 2023, max compression
```

## Comparing `mlb-fantasy-1.3.tar` & `mlb-fantasy-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 19:13:40.272302 mlb-fantasy-1.3/
--rw-r--r--   0 brian     (1000) brian     (1000)      241 2023-05-04 19:13:40.272302 mlb-fantasy-1.3/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      441 2023-05-04 18:59:19.000000 mlb-fantasy-1.3/README.md
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 19:13:40.272302 mlb-fantasy-1.3/mlb_fantasy/
--rw-r--r--   0 brian     (1000) brian     (1000)        0 2023-05-04 17:45:29.000000 mlb-fantasy-1.3/mlb_fantasy/__init__.py
--rw-r--r--   0 brian     (1000) brian     (1000)     2785 2023-05-04 17:47:13.000000 mlb-fantasy-1.3/mlb_fantasy/main.py
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 19:13:40.272302 mlb-fantasy-1.3/mlb_fantasy.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)      241 2023-05-04 19:13:40.000000 mlb-fantasy-1.3/mlb_fantasy.egg-info/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      274 2023-05-04 19:13:40.000000 mlb-fantasy-1.3/mlb_fantasy.egg-info/SOURCES.txt
--rw-r--r--   0 brian     (1000) brian     (1000)        1 2023-05-04 19:13:40.000000 mlb-fantasy-1.3/mlb_fantasy.egg-info/dependency_links.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       55 2023-05-04 19:13:40.000000 mlb-fantasy-1.3/mlb_fantasy.egg-info/entry_points.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       51 2023-05-04 19:13:40.000000 mlb-fantasy-1.3/mlb_fantasy.egg-info/requires.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       12 2023-05-04 19:13:40.000000 mlb-fantasy-1.3/mlb_fantasy.egg-info/top_level.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       38 2023-05-04 19:13:40.272302 mlb-fantasy-1.3/setup.cfg
--rw-r--r--   0 brian     (1000) brian     (1000)      542 2023-05-04 19:13:36.000000 mlb-fantasy-1.3/setup.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 19:15:26.332302 mlb-fantasy-1.4/
+-rw-r--r--   0 brian     (1000) brian     (1000)      725 2023-05-04 19:15:26.332302 mlb-fantasy-1.4/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      441 2023-05-04 18:59:19.000000 mlb-fantasy-1.4/README.md
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 19:15:26.332302 mlb-fantasy-1.4/mlb_fantasy/
+-rw-r--r--   0 brian     (1000) brian     (1000)        0 2023-05-04 17:45:29.000000 mlb-fantasy-1.4/mlb_fantasy/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     2785 2023-05-04 17:47:13.000000 mlb-fantasy-1.4/mlb_fantasy/main.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 19:15:26.332302 mlb-fantasy-1.4/mlb_fantasy.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)      725 2023-05-04 19:15:26.000000 mlb-fantasy-1.4/mlb_fantasy.egg-info/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      274 2023-05-04 19:15:26.000000 mlb-fantasy-1.4/mlb_fantasy.egg-info/SOURCES.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)        1 2023-05-04 19:15:26.000000 mlb-fantasy-1.4/mlb_fantasy.egg-info/dependency_links.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       55 2023-05-04 19:15:26.000000 mlb-fantasy-1.4/mlb_fantasy.egg-info/entry_points.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       51 2023-05-04 19:15:26.000000 mlb-fantasy-1.4/mlb_fantasy.egg-info/requires.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       12 2023-05-04 19:15:26.000000 mlb-fantasy-1.4/mlb_fantasy.egg-info/top_level.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       38 2023-05-04 19:15:26.332302 mlb-fantasy-1.4/setup.cfg
+-rw-r--r--   0 brian     (1000) brian     (1000)      675 2023-05-04 19:15:23.000000 mlb-fantasy-1.4/setup.py
```

### Comparing `mlb-fantasy-1.3/mlb_fantasy/main.py` & `mlb-fantasy-1.4/mlb_fantasy/main.py`

 * *Files identical despite different names*

