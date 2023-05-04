# Comparing `tmp/mlb-fantasy-1.6.tar.gz` & `tmp/mlb-fantasy-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlb-fantasy-1.6.tar", last modified: Thu May  4 20:22:32 2023, max compression
+gzip compressed data, was "mlb-fantasy-1.7.tar", last modified: Thu May  4 20:26:05 2023, max compression
```

## Comparing `mlb-fantasy-1.6.tar` & `mlb-fantasy-1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:22:32.252276 mlb-fantasy-1.6/
--rw-r--r--   0 brian     (1000) brian     (1000)     1358 2023-05-04 20:22:32.252276 mlb-fantasy-1.6/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      994 2023-05-04 19:20:57.000000 mlb-fantasy-1.6/README.md
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:22:32.252276 mlb-fantasy-1.6/mlb_fantasy/
--rw-r--r--   0 brian     (1000) brian     (1000)        0 2023-05-04 17:45:29.000000 mlb-fantasy-1.6/mlb_fantasy/__init__.py
--rw-r--r--   0 brian     (1000) brian     (1000)     2785 2023-05-04 17:47:13.000000 mlb-fantasy-1.6/mlb_fantasy/main.py
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:22:32.252276 mlb-fantasy-1.6/mlb_fantasy.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)     1358 2023-05-04 20:22:32.000000 mlb-fantasy-1.6/mlb_fantasy.egg-info/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      274 2023-05-04 20:22:32.000000 mlb-fantasy-1.6/mlb_fantasy.egg-info/SOURCES.txt
--rw-r--r--   0 brian     (1000) brian     (1000)        1 2023-05-04 20:22:32.000000 mlb-fantasy-1.6/mlb_fantasy.egg-info/dependency_links.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       55 2023-05-04 20:22:32.000000 mlb-fantasy-1.6/mlb_fantasy.egg-info/entry_points.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       34 2023-05-04 20:22:32.000000 mlb-fantasy-1.6/mlb_fantasy.egg-info/requires.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       12 2023-05-04 20:22:32.000000 mlb-fantasy-1.6/mlb_fantasy.egg-info/top_level.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       38 2023-05-04 20:22:32.252276 mlb-fantasy-1.6/setup.cfg
--rw-r--r--   0 brian     (1000) brian     (1000)      622 2023-05-04 20:22:25.000000 mlb-fantasy-1.6/setup.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:26:05.962274 mlb-fantasy-1.7/
+-rw-r--r--   0 brian     (1000) brian     (1000)     1358 2023-05-04 20:26:05.962274 mlb-fantasy-1.7/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      994 2023-05-04 19:20:57.000000 mlb-fantasy-1.7/README.md
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:26:05.952274 mlb-fantasy-1.7/mlb_fantasy/
+-rw-r--r--   0 brian     (1000) brian     (1000)        0 2023-05-04 17:45:29.000000 mlb-fantasy-1.7/mlb_fantasy/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     2785 2023-05-04 17:47:13.000000 mlb-fantasy-1.7/mlb_fantasy/main.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:26:05.952274 mlb-fantasy-1.7/mlb_fantasy.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)     1358 2023-05-04 20:26:05.000000 mlb-fantasy-1.7/mlb_fantasy.egg-info/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      274 2023-05-04 20:26:05.000000 mlb-fantasy-1.7/mlb_fantasy.egg-info/SOURCES.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)        1 2023-05-04 20:26:05.000000 mlb-fantasy-1.7/mlb_fantasy.egg-info/dependency_links.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       55 2023-05-04 20:26:05.000000 mlb-fantasy-1.7/mlb_fantasy.egg-info/entry_points.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       34 2023-05-04 20:26:05.000000 mlb-fantasy-1.7/mlb_fantasy.egg-info/requires.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       12 2023-05-04 20:26:05.000000 mlb-fantasy-1.7/mlb_fantasy.egg-info/top_level.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       38 2023-05-04 20:26:05.962274 mlb-fantasy-1.7/setup.cfg
+-rw-r--r--   0 brian     (1000) brian     (1000)      691 2023-05-04 20:25:59.000000 mlb-fantasy-1.7/setup.py
```

### Comparing `mlb-fantasy-1.6/PKG-INFO` & `mlb-fantasy-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlb-fantasy
-Version: 1.6
+Version: 1.7
 Summary: MLB fantasy draft optimizer.  See README.md for more information.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # mlb-fantasy
         A MLB fantasy league tracker setup using MLB scores
         
         # How To Use
```

### Comparing `mlb-fantasy-1.6/README.md` & `mlb-fantasy-1.7/README.md`

 * *Files identical despite different names*

### Comparing `mlb-fantasy-1.6/mlb_fantasy/main.py` & `mlb-fantasy-1.7/mlb_fantasy/main.py`

 * *Files identical despite different names*

### Comparing `mlb-fantasy-1.6/mlb_fantasy.egg-info/PKG-INFO` & `mlb-fantasy-1.7/mlb_fantasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlb-fantasy
-Version: 1.6
+Version: 1.7
 Summary: MLB fantasy draft optimizer.  See README.md for more information.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # mlb-fantasy
         A MLB fantasy league tracker setup using MLB scores
         
         # How To Use
```

