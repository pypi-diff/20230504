# Comparing `tmp/Hashhound-0.3.tar.gz` & `tmp/Hashhound-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hashhound-0.3.tar", last modified: Thu May  4 12:27:32 2023, max compression
+gzip compressed data, was "Hashhound-0.4.tar", last modified: Thu May  4 12:29:44 2023, max compression
```

## Comparing `Hashhound-0.3.tar` & `Hashhound-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-04 12:27:32.172110 Hashhound-0.3/
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-04 12:27:32.172110 Hashhound-0.3/Hashhound.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)      275 2023-05-04 12:27:32.000000 Hashhound-0.3/Hashhound.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)      258 2023-05-04 12:27:32.000000 Hashhound-0.3/Hashhound.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 12:27:32.000000 Hashhound-0.3/Hashhound.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)       36 2023-05-04 12:27:32.000000 Hashhound-0.3/Hashhound.egg-info/entry_points.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 12:25:09.000000 Hashhound-0.3/Hashhound.egg-info/not-zip-safe
--rw-rw-r--   0 a         (1000) a         (1000)       10 2023-05-04 12:27:32.000000 Hashhound-0.3/Hashhound.egg-info/requires.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 12:27:32.000000 Hashhound-0.3/Hashhound.egg-info/top_level.txt
--rw-rw-r--   0 a         (1000) a         (1000)     1060 2023-05-04 12:24:22.000000 Hashhound-0.3/LICENSE
--rw-rw-r--   0 a         (1000) a         (1000)      275 2023-05-04 12:27:32.172110 Hashhound-0.3/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)       63 2023-05-04 12:24:22.000000 Hashhound-0.3/README.md
--rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-04 12:27:32.172110 Hashhound-0.3/setup.cfg
--rw-rw-r--   0 a         (1000) a         (1000)      445 2023-05-04 12:27:30.000000 Hashhound-0.3/setup.py
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-04 12:29:44.517012 Hashhound-0.4/
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-04 12:29:44.517012 Hashhound-0.4/Hashhound.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)      275 2023-05-04 12:29:44.000000 Hashhound-0.4/Hashhound.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)      258 2023-05-04 12:29:44.000000 Hashhound-0.4/Hashhound.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 12:29:44.000000 Hashhound-0.4/Hashhound.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)       41 2023-05-04 12:29:44.000000 Hashhound-0.4/Hashhound.egg-info/entry_points.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 12:25:09.000000 Hashhound-0.4/Hashhound.egg-info/not-zip-safe
+-rw-rw-r--   0 a         (1000) a         (1000)       10 2023-05-04 12:29:44.000000 Hashhound-0.4/Hashhound.egg-info/requires.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-04 12:29:44.000000 Hashhound-0.4/Hashhound.egg-info/top_level.txt
+-rw-rw-r--   0 a         (1000) a         (1000)     1060 2023-05-04 12:24:22.000000 Hashhound-0.4/LICENSE
+-rw-rw-r--   0 a         (1000) a         (1000)      275 2023-05-04 12:29:44.517012 Hashhound-0.4/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)       63 2023-05-04 12:24:22.000000 Hashhound-0.4/README.md
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-04 12:29:44.517012 Hashhound-0.4/setup.cfg
+-rw-rw-r--   0 a         (1000) a         (1000)      450 2023-05-04 12:29:26.000000 Hashhound-0.4/setup.py
```

### Comparing `Hashhound-0.3/LICENSE` & `Hashhound-0.4/LICENSE`

 * *Files identical despite different names*

