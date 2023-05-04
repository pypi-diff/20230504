# Comparing `tmp/googlegallary-0.4.0.tar.gz` & `tmp/googlegallary-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googlegallary-0.4.0.tar", last modified: Thu May  4 13:30:29 2023, max compression
+gzip compressed data, was "googlegallary-0.5.0.tar", last modified: Thu May  4 15:22:32 2023, max compression
```

## Comparing `googlegallary-0.4.0.tar` & `googlegallary-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 13:30:29.840695 googlegallary-0.4.0/
--rw-rw-rw-   0        0        0      107 2023-05-04 13:30:29.835685 googlegallary-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-05-04 08:13:02.000000 googlegallary-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 13:30:29.783345 googlegallary-0.4.0/googlegallary/
--rw-rw-rw-   0        0        0     1437 2023-05-04 13:25:08.000000 googlegallary-0.4.0/googlegallary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:30:29.835685 googlegallary-0.4.0/googlegallary.egg-info/
--rw-rw-rw-   0        0        0      107 2023-05-04 13:30:29.000000 googlegallary-0.4.0/googlegallary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-05-04 13:30:29.000000 googlegallary-0.4.0/googlegallary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 13:30:29.000000 googlegallary-0.4.0/googlegallary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-04 13:30:29.000000 googlegallary-0.4.0/googlegallary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-04 13:30:29.000000 googlegallary-0.4.0/googlegallary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 13:30:29.840695 googlegallary-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      493 2023-05-04 13:30:20.000000 googlegallary-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:22:32.850473 googlegallary-0.5.0/
+-rw-rw-rw-   0        0        0      136 2023-05-04 15:22:32.849146 googlegallary-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2023-05-04 08:13:02.000000 googlegallary-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 15:22:32.815857 googlegallary-0.5.0/googlegallary/
+-rw-rw-rw-   0        0        0     1437 2023-05-04 15:16:09.000000 googlegallary-0.5.0/googlegallary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:22:32.847854 googlegallary-0.5.0/googlegallary.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-04 15:22:32.000000 googlegallary-0.5.0/googlegallary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-04 15:22:32.000000 googlegallary-0.5.0/googlegallary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 15:22:32.000000 googlegallary-0.5.0/googlegallary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-04 15:22:32.000000 googlegallary-0.5.0/googlegallary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 15:22:32.850473 googlegallary-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      229 2023-05-04 15:21:51.000000 googlegallary-0.5.0/setup.py
```

### Comparing `googlegallary-0.4.0/googlegallary/__init__.py` & `googlegallary-0.5.0/googlegallary/__init__.py`

 * *Files identical despite different names*

