# Comparing `tmp/AegosPy-0.3.tar.gz` & `tmp/AegosPy-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AegosPy-0.3.tar", last modified: Thu May  4 07:41:32 2023, max compression
+gzip compressed data, was "AegosPy-0.4.tar", last modified: Thu May  4 07:46:41 2023, max compression
```

## Comparing `AegosPy-0.3.tar` & `AegosPy-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 07:41:32.122776 AegosPy-0.3/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:41:32.080357 AegosPy-0.3/AegosPy/
--rw-rw-rw-   0        0        0    29934 2023-05-04 07:38:54.000000 AegosPy-0.3/AegosPy/AegosPy.py
--rw-rw-rw-   0        0        0      319 2023-05-01 12:38:40.000000 AegosPy-0.3/AegosPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:41:32.118807 AegosPy-0.3/AegosPy.egg-info/
--rw-rw-rw-   0        0        0      277 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      277 2023-05-04 07:41:32.120781 AegosPy-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-04 07:41:32.122776 AegosPy-0.3/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-05-04 07:40:44.000000 AegosPy-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:46:41.469097 AegosPy-0.4/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:46:41.403411 AegosPy-0.4/AegosPy/
+-rw-rw-rw-   0        0        0    29934 2023-05-04 07:38:54.000000 AegosPy-0.4/AegosPy/AegosPy.py
+-rw-rw-rw-   0        0        0      393 2023-05-04 07:46:04.000000 AegosPy-0.4/AegosPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:46:41.460120 AegosPy-0.4/AegosPy.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-05-04 07:46:41.000000 AegosPy-0.4/AegosPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      277 2023-05-04 07:46:41.465107 AegosPy-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:46:41.470095 AegosPy-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-05-04 07:46:25.000000 AegosPy-0.4/setup.py
```

### Comparing `AegosPy-0.3/AegosPy/AegosPy.py` & `AegosPy-0.4/AegosPy/AegosPy.py`

 * *Files identical despite different names*

