# Comparing `tmp/ASCE-0.0.7.tar.gz` & `tmp/ASCE-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCE-0.0.7.tar", last modified: Wed May  3 22:17:17 2023, max compression
+gzip compressed data, was "ASCE-0.0.8.tar", last modified: Wed May  3 22:25:19 2023, max compression
```

## Comparing `ASCE-0.0.7.tar` & `ASCE-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 22:17:17.574354 ASCE-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-05-03 22:17:17.545355 ASCE-0.0.7/ASCE/
--rw-rw-rw-   0        0        0    11885 2023-05-03 21:46:46.000000 ASCE-0.0.7/ASCE/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 22:17:17.568354 ASCE-0.0.7/ASCE.egg-info/
--rw-rw-rw-   0        0        0      544 2023-05-03 22:17:17.000000 ASCE-0.0.7/ASCE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-05-03 22:17:17.000000 ASCE-0.0.7/ASCE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 22:17:17.000000 ASCE-0.0.7/ASCE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 22:17:17.000000 ASCE-0.0.7/ASCE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1061 2023-05-03 21:46:45.000000 ASCE-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      544 2023-05-03 22:17:17.572355 ASCE-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-05-03 21:46:46.000000 ASCE-0.0.7/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 22:17:17.575353 ASCE-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-05-03 22:16:45.000000 ASCE-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:25:19.444898 ASCE-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-05-03 22:25:19.415896 ASCE-0.0.8/ASCE/
+-rw-rw-rw-   0        0        0    11885 2023-05-03 21:46:46.000000 ASCE-0.0.8/ASCE/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:25:19.439897 ASCE-0.0.8/ASCE.egg-info/
+-rw-rw-rw-   0        0        0      837 2023-05-03 22:25:19.000000 ASCE-0.0.8/ASCE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-05-03 22:25:19.000000 ASCE-0.0.8/ASCE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 22:25:19.000000 ASCE-0.0.8/ASCE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 22:25:19.000000 ASCE-0.0.8/ASCE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1061 2023-05-03 21:46:45.000000 ASCE-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      837 2023-05-03 22:25:19.443896 ASCE-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2023-05-03 22:22:56.000000 ASCE-0.0.8/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 22:25:19.445897 ASCE-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      939 2023-05-03 22:24:58.000000 ASCE-0.0.8/setup.py
```

### Comparing `ASCE-0.0.7/ASCE/__init__.py` & `ASCE-0.0.8/ASCE/__init__.py`

 * *Files identical despite different names*

### Comparing `ASCE-0.0.7/LICENSE` & `ASCE-0.0.8/LICENSE`

 * *Files identical despite different names*

