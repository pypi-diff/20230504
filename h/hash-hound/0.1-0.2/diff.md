# Comparing `tmp/hash-hound-0.1.tar.gz` & `tmp/hash-hound-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hash-hound-0.1.tar", last modified: Thu May  4 12:41:56 2023, max compression
+gzip compressed data, was "hash-hound-0.2.tar", last modified: Thu May  4 17:08:29 2023, max compression
```

## Comparing `hash-hound-0.1.tar` & `hash-hound-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-04 12:41:56.721271 hash-hound-0.1/
--rw-rw-r--   0 a         (1000) a         (1000)     1060 2023-05-04 12:24:22.000000 hash-hound-0.1/LICENSE
--rw-rw-r--   0 a         (1000) a         (1000)      277 2023-05-04 12:41:56.721271 hash-hound-0.1/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)       63 2023-05-04 12:24:22.000000 hash-hound-0.1/README.md
--rw-rw-r--   0 a         (1000) a         (1000)      963 2023-05-04 12:37:59.000000 hash-hound-0.1/hash.py
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-04 12:41:56.721271 hash-hound-0.1/hash_hound.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)      277 2023-05-04 12:41:56.000000 hash-hound-0.1/hash_hound.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)      273 2023-05-04 12:41:56.000000 hash-hound-0.1/hash_hound.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 12:41:56.000000 hash-hound-0.1/hash_hound.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)       42 2023-05-04 12:41:56.000000 hash-hound-0.1/hash_hound.egg-info/entry_points.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 12:39:32.000000 hash-hound-0.1/hash_hound.egg-info/not-zip-safe
--rw-rw-r--   0 a         (1000) a         (1000)       10 2023-05-04 12:41:56.000000 hash-hound-0.1/hash_hound.egg-info/requires.txt
--rw-rw-r--   0 a         (1000) a         (1000)        5 2023-05-04 12:41:56.000000 hash-hound-0.1/hash_hound.egg-info/top_level.txt
--rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-04 12:41:56.721271 hash-hound-0.1/setup.cfg
--rw-rw-r--   0 a         (1000) a         (1000)      478 2023-05-04 12:41:51.000000 hash-hound-0.1/setup.py
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-04 17:08:29.484908 hash-hound-0.2/
+-rw-rw-r--   0 a         (1000) a         (1000)     1060 2023-05-04 12:24:22.000000 hash-hound-0.2/LICENSE
+-rw-rw-r--   0 a         (1000) a         (1000)      616 2023-05-04 17:08:29.484908 hash-hound-0.2/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)       63 2023-05-04 12:24:22.000000 hash-hound-0.2/README.md
+-rw-rw-r--   0 a         (1000) a         (1000)     1521 2023-05-04 17:05:15.000000 hash-hound-0.2/hash.py
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-04 17:08:29.484908 hash-hound-0.2/hash_hound.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)      616 2023-05-04 17:08:29.000000 hash-hound-0.2/hash_hound.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)      273 2023-05-04 17:08:29.000000 hash-hound-0.2/hash_hound.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 17:08:29.000000 hash-hound-0.2/hash_hound.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)       42 2023-05-04 17:08:29.000000 hash-hound-0.2/hash_hound.egg-info/entry_points.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 12:39:32.000000 hash-hound-0.2/hash_hound.egg-info/not-zip-safe
+-rw-rw-r--   0 a         (1000) a         (1000)       10 2023-05-04 17:08:29.000000 hash-hound-0.2/hash_hound.egg-info/requires.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        5 2023-05-04 17:08:29.000000 hash-hound-0.2/hash_hound.egg-info/top_level.txt
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-04 17:08:29.484908 hash-hound-0.2/setup.cfg
+-rw-rw-r--   0 a         (1000) a         (1000)      817 2023-05-04 17:06:45.000000 hash-hound-0.2/setup.py
```

### Comparing `hash-hound-0.1/LICENSE` & `hash-hound-0.2/LICENSE`

 * *Files identical despite different names*

