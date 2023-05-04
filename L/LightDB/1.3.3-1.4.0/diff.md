# Comparing `tmp/LightDB-1.3.3.tar.gz` & `tmp/LightDB-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LightDB-1.3.3.tar", last modified: Thu Mar 30 02:57:02 2023, max compression
+gzip compressed data, was "LightDB-1.4.0.tar", last modified: Thu May  4 15:12:49 2023, max compression
```

## Comparing `LightDB-1.3.3.tar` & `LightDB-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 02:57:02.686315 LightDB-1.3.3/
-drwxrwxrwx   0        0        0        0 2023-03-30 02:57:02.665370 LightDB-1.3.3/LightDB.egg-info/
--rw-rw-rw-   0        0        0     2400 2023-03-30 02:57:02.000000 LightDB-1.3.3/LightDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-03-30 02:57:02.000000 LightDB-1.3.3/LightDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 02:57:02.000000 LightDB-1.3.3/LightDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-30 02:57:02.000000 LightDB-1.3.3/LightDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2400 2023-03-30 02:57:02.687316 LightDB-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2082 2023-03-30 02:52:29.000000 LightDB-1.3.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-30 02:57:02.684321 LightDB-1.3.3/lightdb/
--rw-rw-rw-   0        0        0     4684 2023-03-29 10:11:10.000000 LightDB-1.3.3/lightdb/LightDB.py
--rw-rw-rw-   0        0        0      238 2023-03-29 10:37:38.000000 LightDB-1.3.3/lightdb/__init__.py
--rw-rw-rw-   0        0        0       42 2023-03-30 02:57:02.689307 LightDB-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      416 2023-03-29 10:37:27.000000 LightDB-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:12:49.653065 LightDB-1.4.0/
+drwxrwxrwx   0        0        0        0 2023-05-04 15:12:49.649104 LightDB-1.4.0/LightDB.egg-info/
+-rw-rw-rw-   0        0        0     2400 2023-05-04 15:12:49.000000 LightDB-1.4.0/LightDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-05-04 15:12:49.000000 LightDB-1.4.0/LightDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 15:12:49.000000 LightDB-1.4.0/LightDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 15:12:49.000000 LightDB-1.4.0/LightDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2400 2023-05-04 15:12:49.654063 LightDB-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2082 2023-03-30 02:52:29.000000 LightDB-1.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-04 15:12:49.652069 LightDB-1.4.0/lightdb/
+-rw-rw-rw-   0        0        0       71 2023-05-04 15:09:54.000000 LightDB-1.4.0/lightdb/__init__.py
+-rw-rw-rw-   0        0        0     4651 2023-05-04 15:11:22.000000 LightDB-1.4.0/lightdb/core.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 15:12:49.658052 LightDB-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      416 2023-05-04 15:11:48.000000 LightDB-1.4.0/setup.py
```

### Comparing `LightDB-1.3.3/LightDB.egg-info/PKG-INFO` & `LightDB-1.4.0/LightDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LightDB
-Version: 1.3.3
+Version: 1.4.0
 Summary: Lightweight JSON Database for Python
 Home-page: https://github.com/Fl1yd/LightDB
 Download-URL: https://github.com/Fl1yd/LightDB/releases
 Author: Fl1yd
 Author-email: projects@fl1yd.su
 License: MIT
```

### Comparing `LightDB-1.3.3/PKG-INFO` & `LightDB-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LightDB
-Version: 1.3.3
+Version: 1.4.0
 Summary: Lightweight JSON Database for Python
 Home-page: https://github.com/Fl1yd/LightDB
 Download-URL: https://github.com/Fl1yd/LightDB/releases
 Author: Fl1yd
 Author-email: projects@fl1yd.su
 License: MIT
```

### Comparing `LightDB-1.3.3/README.rst` & `LightDB-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `LightDB-1.3.3/lightdb/LightDB.py` & `LightDB-1.4.0/lightdb/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""The main file for the LightDB project.
-
-:copyright: (c) 2021-2023 by Fl1yd.
-:license: MIT, see LICENSE for more details.
-"""
+"""A file that containing the main implementation of the LightDB database management system"""
 
 import json
 
 from pathlib import Path
 from typing import Dict, Any
```

