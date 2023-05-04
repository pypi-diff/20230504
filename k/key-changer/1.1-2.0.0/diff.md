# Comparing `tmp/key_changer-1.1.tar.gz` & `tmp/key-changer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_changer-1.1.tar", last modified: Fri Mar 25 06:19:58 2022, max compression
+gzip compressed data, was "key-changer-2.0.0.tar", last modified: Thu May  4 14:43:58 2023, max compression
```

## Comparing `key_changer-1.1.tar` & `key-changer-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-03-25 06:19:58.190333 key_changer-1.1/
--rw-rw-rw-   0        0        0      625 2022-03-25 06:19:58.189371 key_changer-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      301 2022-03-25 06:16:01.000000 key_changer-1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-03-25 06:19:58.174378 key_changer-1.1/key_changer/
--rw-rw-rw-   0        0        0       28 2022-03-25 05:44:49.000000 key_changer-1.1/key_changer/__init__.py
--rw-rw-rw-   0        0        0     2282 2022-03-25 06:01:20.000000 key_changer-1.1/key_changer/main.py
-drwxrwxrwx   0        0        0        0 2022-03-25 06:19:58.186345 key_changer-1.1/key_changer.egg-info/
--rw-rw-rw-   0        0        0      625 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2022-03-25 06:19:57.000000 key_changer-1.1/key_changer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-25 06:19:58.191345 key_changer-1.1/setup.cfg
--rw-rw-rw-   0        0        0      594 2022-03-25 06:19:40.000000 key_changer-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:43:58.713415 key-changer-2.0.0/
+-rw-rw-rw-   0        0        0     1068 2023-05-04 14:01:57.000000 key-changer-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1535 2023-05-04 14:43:58.712416 key-changer-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2023-05-04 14:28:06.000000 key-changer-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 14:43:58.676415 key-changer-2.0.0/key_changer/
+-rw-rw-rw-   0        0        0      293 2023-05-04 14:01:57.000000 key-changer-2.0.0/key_changer/__init__.py
+-rw-rw-rw-   0        0        0     1392 2023-05-04 14:01:57.000000 key-changer-2.0.0/key_changer/__main__.py
+-rw-rw-rw-   0        0        0     1027 2023-05-04 14:01:57.000000 key-changer-2.0.0/key_changer/layout_map.py
+-rw-rw-rw-   0        0        0     2153 2023-05-04 14:01:57.000000 key-changer-2.0.0/key_changer/translate.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:43:58.708426 key-changer-2.0.0/key_changer.egg-info/
+-rw-rw-rw-   0        0        0     1535 2023-05-04 14:43:58.000000 key-changer-2.0.0/key_changer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-04 14:43:58.000000 key-changer-2.0.0/key_changer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:43:58.000000 key-changer-2.0.0/key_changer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-04 14:43:58.000000 key-changer-2.0.0/key_changer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 14:43:58.714416 key-changer-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-05-04 14:43:51.000000 key-changer-2.0.0/setup.py
```

