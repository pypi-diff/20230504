# Comparing `tmp/mlb-fantasy-1.8.tar.gz` & `tmp/mlb-fantasy-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlb-fantasy-1.8.tar", last modified: Thu May  4 20:27:51 2023, max compression
+gzip compressed data, was "mlb-fantasy-1.9.tar", last modified: Thu May  4 20:28:48 2023, max compression
```

## Comparing `mlb-fantasy-1.8.tar` & `mlb-fantasy-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:27:51.182273 mlb-fantasy-1.8/
--rw-r--r--   0 brian     (1000) brian     (1000)     1358 2023-05-04 20:27:51.182273 mlb-fantasy-1.8/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      994 2023-05-04 19:20:57.000000 mlb-fantasy-1.8/README.md
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:27:51.182273 mlb-fantasy-1.8/mlb_fantasy/
--rw-r--r--   0 brian     (1000) brian     (1000)        0 2023-05-04 17:45:29.000000 mlb-fantasy-1.8/mlb_fantasy/__init__.py
--rw-r--r--   0 brian     (1000) brian     (1000)     2785 2023-05-04 17:47:13.000000 mlb-fantasy-1.8/mlb_fantasy/main.py
-drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:27:51.182273 mlb-fantasy-1.8/mlb_fantasy.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)     1358 2023-05-04 20:27:51.000000 mlb-fantasy-1.8/mlb_fantasy.egg-info/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1000)      274 2023-05-04 20:27:51.000000 mlb-fantasy-1.8/mlb_fantasy.egg-info/SOURCES.txt
--rw-r--r--   0 brian     (1000) brian     (1000)        1 2023-05-04 20:27:51.000000 mlb-fantasy-1.8/mlb_fantasy.egg-info/dependency_links.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       55 2023-05-04 20:27:51.000000 mlb-fantasy-1.8/mlb_fantasy.egg-info/entry_points.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       34 2023-05-04 20:27:51.000000 mlb-fantasy-1.8/mlb_fantasy.egg-info/requires.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       12 2023-05-04 20:27:51.000000 mlb-fantasy-1.8/mlb_fantasy.egg-info/top_level.txt
--rw-r--r--   0 brian     (1000) brian     (1000)       38 2023-05-04 20:27:51.182273 mlb-fantasy-1.8/setup.cfg
--rw-r--r--   0 brian     (1000) brian     (1000)      677 2023-05-04 20:27:47.000000 mlb-fantasy-1.8/setup.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:28:48.302273 mlb-fantasy-1.9/
+-rw-r--r--   0 brian     (1000) brian     (1000)     1358 2023-05-04 20:28:48.302273 mlb-fantasy-1.9/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      994 2023-05-04 19:20:57.000000 mlb-fantasy-1.9/README.md
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:28:48.302273 mlb-fantasy-1.9/mlb_fantasy/
+-rw-r--r--   0 brian     (1000) brian     (1000)        0 2023-05-04 17:45:29.000000 mlb-fantasy-1.9/mlb_fantasy/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1000)     2785 2023-05-04 17:47:13.000000 mlb-fantasy-1.9/mlb_fantasy/main.py
+drwxr-xr-x   0 brian     (1000) brian     (1000)        0 2023-05-04 20:28:48.302273 mlb-fantasy-1.9/mlb_fantasy.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)     1358 2023-05-04 20:28:48.000000 mlb-fantasy-1.9/mlb_fantasy.egg-info/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1000)      274 2023-05-04 20:28:48.000000 mlb-fantasy-1.9/mlb_fantasy.egg-info/SOURCES.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)        1 2023-05-04 20:28:48.000000 mlb-fantasy-1.9/mlb_fantasy.egg-info/dependency_links.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       55 2023-05-04 20:28:48.000000 mlb-fantasy-1.9/mlb_fantasy.egg-info/entry_points.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       34 2023-05-04 20:28:48.000000 mlb-fantasy-1.9/mlb_fantasy.egg-info/requires.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       12 2023-05-04 20:28:48.000000 mlb-fantasy-1.9/mlb_fantasy.egg-info/top_level.txt
+-rw-r--r--   0 brian     (1000) brian     (1000)       38 2023-05-04 20:28:48.302273 mlb-fantasy-1.9/setup.cfg
+-rw-r--r--   0 brian     (1000) brian     (1000)      604 2023-05-04 20:28:44.000000 mlb-fantasy-1.9/setup.py
```

### Comparing `mlb-fantasy-1.8/PKG-INFO` & `mlb-fantasy-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlb-fantasy
-Version: 1.8
+Version: 1.9
 Summary: MLB fantasy draft optimizer.  See README.md for more information.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # mlb-fantasy
         A MLB fantasy league tracker setup using MLB scores
         
         # How To Use
```

### Comparing `mlb-fantasy-1.8/README.md` & `mlb-fantasy-1.9/README.md`

 * *Files identical despite different names*

### Comparing `mlb-fantasy-1.8/mlb_fantasy/main.py` & `mlb-fantasy-1.9/mlb_fantasy/main.py`

 * *Files identical despite different names*

### Comparing `mlb-fantasy-1.8/mlb_fantasy.egg-info/PKG-INFO` & `mlb-fantasy-1.9/mlb_fantasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlb-fantasy
-Version: 1.8
+Version: 1.9
 Summary: MLB fantasy draft optimizer.  See README.md for more information.
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # mlb-fantasy
         A MLB fantasy league tracker setup using MLB scores
         
         # How To Use
```

### Comparing `mlb-fantasy-1.8/setup.py` & `mlb-fantasy-1.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-with open('requirements.txt') as f:
-    required = f.read().splitlines()
 
 setup(
     name='mlb-fantasy',
-    version='1.8',
+    version='1.9',
     description="MLB fantasy draft optimizer.  See README.md for more information.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'pybaseball==2.2.5',
```

