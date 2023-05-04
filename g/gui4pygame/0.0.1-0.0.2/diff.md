# Comparing `tmp/gui4pygame-0.0.1.tar.gz` & `tmp/gui4pygame-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gui4pygame-0.0.1.tar", last modified: Thu May  4 17:39:50 2023, max compression
+gzip compressed data, was "gui4pygame-0.0.2.tar", last modified: Thu May  4 17:53:35 2023, max compression
```

## Comparing `gui4pygame-0.0.1.tar` & `gui4pygame-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:39:50.088776 gui4pygame-0.0.1/
--rw-rw-rw-   0        0        0      280 2023-05-04 17:39:50.088776 gui4pygame-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-04 17:39:50.057576 gui4pygame-0.0.1/gui4pygame/
--rw-rw-rw-   0        0        0       22 2023-05-04 17:27:06.000000 gui4pygame-0.0.1/gui4pygame/__init__.py
--rw-rw-rw-   0        0        0     5004 2023-05-04 17:24:23.000000 gui4pygame-0.0.1/gui4pygame/gui4pygame.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:39:50.073176 gui4pygame-0.0.1/gui4pygame.egg-info/
--rw-rw-rw-   0        0        0      280 2023-05-04 17:39:49.000000 gui4pygame-0.0.1/gui4pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-05-04 17:39:49.000000 gui4pygame-0.0.1/gui4pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:39:49.000000 gui4pygame-0.0.1/gui4pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 17:39:49.000000 gui4pygame-0.0.1/gui4pygame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 17:39:49.000000 gui4pygame-0.0.1/gui4pygame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 17:39:50.088776 gui4pygame-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      375 2023-05-04 17:37:41.000000 gui4pygame-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:53:35.297896 gui4pygame-0.0.2/
+-rw-rw-rw-   0        0        0      280 2023-05-04 17:53:35.297896 gui4pygame-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 17:53:35.266697 gui4pygame-0.0.2/gui4pygame/
+-rw-rw-rw-   0        0        0       26 2023-05-04 17:49:10.000000 gui4pygame-0.0.2/gui4pygame/__init__.py
+-rw-rw-rw-   0        0        0     5004 2023-05-04 17:24:23.000000 gui4pygame-0.0.2/gui4pygame/gui4pygame.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:53:35.297896 gui4pygame-0.0.2/gui4pygame.egg-info/
+-rw-rw-rw-   0        0        0      280 2023-05-04 17:53:34.000000 gui4pygame-0.0.2/gui4pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-05-04 17:53:34.000000 gui4pygame-0.0.2/gui4pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:53:34.000000 gui4pygame-0.0.2/gui4pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 17:53:34.000000 gui4pygame-0.0.2/gui4pygame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 17:53:34.000000 gui4pygame-0.0.2/gui4pygame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:53:35.297896 gui4pygame-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      375 2023-05-04 17:51:39.000000 gui4pygame-0.0.2/setup.py
```

### Comparing `gui4pygame-0.0.1/gui4pygame/gui4pygame.py` & `gui4pygame-0.0.2/gui4pygame/gui4pygame.py`

 * *Files identical despite different names*

