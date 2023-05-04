# Comparing `tmp/AegosPy-0.2.tar.gz` & `tmp/AegosPy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AegosPy-0.2.tar", last modified: Sun Apr 30 01:25:22 2023, max compression
+gzip compressed data, was "AegosPy-0.3.tar", last modified: Thu May  4 07:41:32 2023, max compression
```

## Comparing `AegosPy-0.2.tar` & `AegosPy-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 01:25:22.171182 AegosPy-0.2/
-drwxrwxrwx   0        0        0        0 2023-04-30 01:25:22.111853 AegosPy-0.2/AegosPy/
--rw-rw-rw-   0        0        0    15336 2023-04-30 01:24:17.000000 AegosPy-0.2/AegosPy/AegosPy.py
--rw-rw-rw-   0        0        0      281 2023-04-30 01:24:26.000000 AegosPy-0.2/AegosPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:25:22.164679 AegosPy-0.2/AegosPy.egg-info/
--rw-rw-rw-   0        0        0      277 2023-04-30 01:25:21.000000 AegosPy-0.2/AegosPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-04-30 01:25:21.000000 AegosPy-0.2/AegosPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 01:25:21.000000 AegosPy-0.2/AegosPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-30 01:25:21.000000 AegosPy-0.2/AegosPy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-04-30 01:25:21.000000 AegosPy-0.2/AegosPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      277 2023-04-30 01:25:22.166189 AegosPy-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-30 01:25:22.171182 AegosPy-0.2/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-04-30 01:24:58.000000 AegosPy-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:41:32.122776 AegosPy-0.3/
+drwxrwxrwx   0        0        0        0 2023-05-04 07:41:32.080357 AegosPy-0.3/AegosPy/
+-rw-rw-rw-   0        0        0    29934 2023-05-04 07:38:54.000000 AegosPy-0.3/AegosPy/AegosPy.py
+-rw-rw-rw-   0        0        0      319 2023-05-01 12:38:40.000000 AegosPy-0.3/AegosPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:41:32.118807 AegosPy-0.3/AegosPy.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-05-04 07:41:31.000000 AegosPy-0.3/AegosPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      277 2023-05-04 07:41:32.120781 AegosPy-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:41:32.122776 AegosPy-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-05-04 07:40:44.000000 AegosPy-0.3/setup.py
```

