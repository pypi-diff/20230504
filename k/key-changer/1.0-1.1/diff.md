# Comparing `tmp/key_changer-1.0.tar.gz` & `tmp/key_changer-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_changer-1.0.tar", last modified: Fri Mar 25 06:07:35 2022, max compression
+gzip compressed data, was "key_changer-1.1.tar", last modified: Fri Mar 25 06:19:58 2022, max compression
```

## Comparing `key_changer-1.0.tar` & `key_changer-1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-03-25 06:07:35.065401 key_changer-1.0/
--rw-rw-rw-   0        0        0      473 2022-03-25 06:07:35.063406 key_changer-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-03-25 06:07:35.047448 key_changer-1.0/key_changer/
--rw-rw-rw-   0        0        0       28 2022-03-25 05:44:49.000000 key_changer-1.0/key_changer/__init__.py
--rw-rw-rw-   0        0        0     2282 2022-03-25 06:01:20.000000 key_changer-1.0/key_changer/main.py
-drwxrwxrwx   0        0        0        0 2022-03-25 06:07:35.060414 key_changer-1.0/key_changer.egg-info/
--rw-rw-rw-   0        0        0      473 2022-03-25 06:07:34.000000 key_changer-1.0/key_changer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2022-03-25 06:07:34.000000 key_changer-1.0/key_changer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-25 06:07:34.000000 key_changer-1.0/key_changer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-03-25 06:07:34.000000 key_changer-1.0/key_changer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2022-03-25 06:07:34.000000 key_changer-1.0/key_changer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-25 06:07:35.066408 key_changer-1.0/setup.cfg
--rw-rw-rw-   0        0        0      633 2022-03-25 06:07:10.000000 key_changer-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-25 06:19:58.190333 key_changer-1.1/
+-rw-rw-rw-   0        0        0      625 2022-03-25 06:19:58.189371 key_changer-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2022-03-25 06:16:01.000000 key_changer-1.1/README.md
+drwxrwxrwx   0        0        0        0 2022-03-25 06:19:58.174378 key_changer-1.1/key_changer/
+-rw-rw-rw-   0        0        0       28 2022-03-25 05:44:49.000000 key_changer-1.1/key_changer/__init__.py
+-rw-rw-rw-   0        0        0     2282 2022-03-25 06:01:20.000000 key_changer-1.1/key_changer/main.py
+drwxrwxrwx   0        0        0        0 2022-03-25 06:19:58.186345 key_changer-1.1/key_changer.egg-info/
+-rw-rw-rw-   0        0        0      625 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-03-25 06:19:58.191345 key_changer-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      594 2022-03-25 06:19:40.000000 key_changer-1.1/setup.py
```

### Comparing `key_changer-1.0/key_changer/main.py` & `key_changer-1.1/key_changer/main.py`

 * *Files identical despite different names*

