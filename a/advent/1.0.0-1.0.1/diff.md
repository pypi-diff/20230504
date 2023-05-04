# Comparing `tmp/advent-1.0.0.tar.gz` & `tmp/advent-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advent-1.0.0.tar", last modified: Thu May  4 17:32:37 2023, max compression
+gzip compressed data, was "advent-1.0.1.tar", last modified: Thu May  4 18:33:31 2023, max compression
```

## Comparing `advent-1.0.0.tar` & `advent-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:32:37.070312 advent-1.0.0/
--rw-rw-rw-   0        0        0     1086 2023-05-04 15:53:38.000000 advent-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-05-04 17:32:37.070312 advent-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1180 2023-05-04 17:21:56.000000 advent-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 17:32:37.014302 advent-1.0.0/advent/
--rw-rw-rw-   0        0        0      307 2023-05-04 16:09:24.000000 advent-1.0.0/advent/__init__.py
--rw-rw-rw-   0        0        0      410 2023-05-04 16:15:30.000000 advent-1.0.0/advent/__main__.py
--rw-rw-rw-   0        0        0      624 2023-05-04 16:08:10.000000 advent-1.0.0/advent/errors.py
--rw-rw-rw-   0        0        0      671 2023-05-04 16:09:39.000000 advent-1.0.0/advent/functions.py
--rw-rw-rw-   0        0        0     1125 2023-05-04 16:30:06.000000 advent-1.0.0/advent/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:32:37.070312 advent-1.0.0/advent.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-05-04 17:32:36.000000 advent-1.0.0/advent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-05-04 17:32:36.000000 advent-1.0.0/advent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:32:36.000000 advent-1.0.0/advent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-04 17:32:36.000000 advent-1.0.0/advent.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-05-04 17:32:36.000000 advent-1.0.0/advent.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 17:32:36.000000 advent-1.0.0/advent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      624 2023-05-04 15:59:40.000000 advent-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 17:32:37.070312 advent-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 18:33:31.884276 advent-1.0.1/
+-rw-rw-rw-   0        0        0     1086 2023-05-04 15:53:38.000000 advent-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-05-04 18:33:31.884276 advent-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1180 2023-05-04 17:21:56.000000 advent-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 18:33:31.828268 advent-1.0.1/advent/
+-rw-rw-rw-   0        0        0      365 2023-05-04 18:29:28.000000 advent-1.0.1/advent/__init__.py
+-rw-rw-rw-   0        0        0      410 2023-05-04 16:15:30.000000 advent-1.0.1/advent/__main__.py
+-rw-rw-rw-   0        0        0      624 2023-05-04 16:08:10.000000 advent-1.0.1/advent/errors.py
+-rw-rw-rw-   0        0        0      671 2023-05-04 16:09:39.000000 advent-1.0.1/advent/functions.py
+-rw-rw-rw-   0        0        0     1125 2023-05-04 16:30:06.000000 advent-1.0.1/advent/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:33:31.876269 advent-1.0.1/advent.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-05-04 18:33:31.000000 advent-1.0.1/advent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-04 18:33:31.000000 advent-1.0.1/advent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 18:33:31.000000 advent-1.0.1/advent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-04 18:33:31.000000 advent-1.0.1/advent.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-05-04 18:33:31.000000 advent-1.0.1/advent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 18:33:31.000000 advent-1.0.1/advent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      624 2023-05-04 18:29:42.000000 advent-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 18:33:31.884276 advent-1.0.1/setup.cfg
```

### Comparing `advent-1.0.0/LICENSE` & `advent-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `advent-1.0.0/PKG-INFO` & `advent-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advent
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get your Advent of Code puzzle input and much more!
 Author-email: ravilnicki <ravilnicki@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ravilnicki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `advent-1.0.0/README.md` & `advent-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `advent-1.0.0/advent/errors.py` & `advent-1.0.1/advent/errors.py`

 * *Files identical despite different names*

### Comparing `advent-1.0.0/advent/functions.py` & `advent-1.0.1/advent/functions.py`

 * *Files identical despite different names*

### Comparing `advent-1.0.0/advent/parser.py` & `advent-1.0.1/advent/parser.py`

 * *Files identical despite different names*

### Comparing `advent-1.0.0/advent.egg-info/PKG-INFO` & `advent-1.0.1/advent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advent
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get your Advent of Code puzzle input and much more!
 Author-email: ravilnicki <ravilnicki@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ravilnicki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `advent-1.0.0/pyproject.toml` & `advent-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "advent"
-version = "1.0.0"
+version = "1.0.1"
 description = "Get your Advent of Code puzzle input and much more!"
 readme = "README.md"
 authors = [{ name = "ravilnicki", email = "ravilnicki@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

