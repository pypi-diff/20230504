# Comparing `tmp/betweens-0.0.1.tar.gz` & `tmp/betweens-0.1.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betweens-0.0.1.tar", last modified: Wed May  3 12:27:24 2023, max compression
+gzip compressed data, was "betweens-0.1.1.dev1.tar", last modified: Thu May  4 10:21:35 2023, max compression
```

## Comparing `betweens-0.0.1.tar` & `betweens-0.1.1.dev1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 12:27:24.752941 betweens-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      637 2023-05-03 12:27:24.752941 betweens-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-03 12:21:11.000000 betweens-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 12:27:24.752941 betweens-0.0.1/betweens/
--rw-rw-rw-   0        0        0      347 2023-05-03 12:10:26.000000 betweens-0.0.1/betweens/__init__.py
--rw-rw-rw-   0        0        0     1678 2023-05-03 12:10:19.000000 betweens-0.0.1/betweens/betweens.py
--rw-rw-rw-   0        0        0      128 2023-05-03 10:18:54.000000 betweens-0.0.1/betweens/version.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:27:24.752941 betweens-0.0.1/betweens.egg-info/
--rw-rw-rw-   0        0        0      637 2023-05-03 12:27:24.000000 betweens-0.0.1/betweens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-03 12:27:24.000000 betweens-0.0.1/betweens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 12:27:24.000000 betweens-0.0.1/betweens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 12:27:24.000000 betweens-0.0.1/betweens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 12:27:24.752941 betweens-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-03 12:27:04.000000 betweens-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:21:35.270693 betweens-0.1.1.dev1/
+-rw-rw-rw-   0        0        0     1091 2023-05-03 12:21:47.000000 betweens-0.1.1.dev1/LICENSE
+-rw-rw-rw-   0        0        0       13 2023-05-04 10:16:44.000000 betweens-0.1.1.dev1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1166 2023-05-04 10:21:35.270693 betweens-0.1.1.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-03 12:21:11.000000 betweens-0.1.1.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 10:21:35.255052 betweens-0.1.1.dev1/betweens/
+-rw-rw-rw-   0        0        0      347 2023-05-03 12:10:26.000000 betweens-0.1.1.dev1/betweens/__init__.py
+-rw-rw-rw-   0        0        0     1678 2023-05-03 12:10:19.000000 betweens-0.1.1.dev1/betweens/betweens.py
+-rw-rw-rw-   0        0        0      128 2023-05-03 10:18:54.000000 betweens-0.1.1.dev1/betweens/version.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:21:35.270693 betweens-0.1.1.dev1/betweens.egg-info/
+-rw-rw-rw-   0        0        0     1166 2023-05-04 10:21:35.000000 betweens-0.1.1.dev1/betweens.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-04 10:21:35.000000 betweens-0.1.1.dev1/betweens.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:21:35.000000 betweens-0.1.1.dev1/betweens.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 10:21:35.000000 betweens-0.1.1.dev1/betweens.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      150 2023-05-04 10:20:34.000000 betweens-0.1.1.dev1/new.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:21:35.270693 betweens-0.1.1.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     1506 2023-05-04 10:20:43.000000 betweens-0.1.1.dev1/setup.py
```

### Comparing `betweens-0.0.1/LICENSE` & `betweens-0.1.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `betweens-0.0.1/betweens/betweens.py` & `betweens-0.1.1.dev1/betweens/betweens.py`

 * *Files identical despite different names*

