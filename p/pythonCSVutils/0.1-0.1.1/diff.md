# Comparing `tmp/pythonCSVutils-0.1.tar.gz` & `tmp/pythonCSVutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonCSVutils-0.1.tar", last modified: Wed May  3 21:53:08 2023, max compression
+gzip compressed data, was "pythonCSVutils-0.1.1.tar", last modified: Thu May  4 17:17:41 2023, max compression
```

## Comparing `pythonCSVutils-0.1.tar` & `pythonCSVutils-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 21:53:08.740556 pythonCSVutils-0.1/
--rw-rw-rw-   0        0        0      271 2023-05-03 21:53:08.740556 pythonCSVutils-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 21:53:08.736555 pythonCSVutils-0.1/pythonCSVutils/
--rw-rw-rw-   0        0        0      239 2023-05-03 21:07:56.000000 pythonCSVutils-0.1/pythonCSVutils/__init__.py
--rw-rw-rw-   0        0        0     3010 2023-05-03 21:05:06.000000 pythonCSVutils-0.1/pythonCSVutils/csv_processor.py
--rw-rw-rw-   0        0        0      397 2023-05-03 21:07:02.000000 pythonCSVutils-0.1/pythonCSVutils/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:53:08.739555 pythonCSVutils-0.1/pythonCSVutils.egg-info/
--rw-rw-rw-   0        0        0      271 2023-05-03 21:53:08.000000 pythonCSVutils-0.1/pythonCSVutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-03 21:53:08.000000 pythonCSVutils-0.1/pythonCSVutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 21:53:08.000000 pythonCSVutils-0.1/pythonCSVutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 21:53:08.000000 pythonCSVutils-0.1/pythonCSVutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 21:53:08.741555 pythonCSVutils-0.1/setup.cfg
--rw-rw-rw-   0        0        0      397 2023-05-03 21:07:02.000000 pythonCSVutils-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:41.748107 pythonCSVutils-0.1.1/
+-rw-rw-rw-   0        0        0     2073 2023-05-04 17:17:41.748107 pythonCSVutils-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1757 2023-05-03 21:52:21.000000 pythonCSVutils-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:41.744104 pythonCSVutils-0.1.1/pythonCSVutils/
+-rw-rw-rw-   0        0        0      239 2023-05-03 21:07:56.000000 pythonCSVutils-0.1.1/pythonCSVutils/__init__.py
+-rw-rw-rw-   0        0        0     3010 2023-05-03 21:05:06.000000 pythonCSVutils-0.1.1/pythonCSVutils/csv_processor.py
+-rw-rw-rw-   0        0        0      557 2023-05-04 17:16:04.000000 pythonCSVutils-0.1.1/pythonCSVutils/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:17:41.747107 pythonCSVutils-0.1.1/pythonCSVutils.egg-info/
+-rw-rw-rw-   0        0        0     2073 2023-05-04 17:17:41.000000 pythonCSVutils-0.1.1/pythonCSVutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-04 17:17:41.000000 pythonCSVutils-0.1.1/pythonCSVutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:17:41.000000 pythonCSVutils-0.1.1/pythonCSVutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 17:17:41.000000 pythonCSVutils-0.1.1/pythonCSVutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:17:41.748107 pythonCSVutils-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-05-04 17:15:45.000000 pythonCSVutils-0.1.1/setup.py
```

### Comparing `pythonCSVutils-0.1/pythonCSVutils/csv_processor.py` & `pythonCSVutils-0.1.1/pythonCSVutils/csv_processor.py`

 * *Files identical despite different names*

