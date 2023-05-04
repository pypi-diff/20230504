# Comparing `tmp/scrapere-0.1.0.tar.gz` & `tmp/scrapere-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.1.0.tar", last modified: Thu May  4 14:47:17 2023, max compression
+gzip compressed data, was "scrapere-0.1.1.tar", last modified: Thu May  4 14:59:40 2023, max compression
```

## Comparing `scrapere-0.1.0.tar` & `scrapere-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-04 14:47:17.709921 scrapere-0.1.0/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      177 2023-05-04 14:47:17.709921 scrapere-0.1.0/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      356 2023-05-04 10:42:22.000000 scrapere-0.1.0/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-04 14:47:17.705922 scrapere-0.1.0/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.0/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     4741 2023-05-04 10:04:57.000000 scrapere-0.1.0/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.0/scrapere/user-agents-unique.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-04 14:47:17.709921 scrapere-0.1.0/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      177 2023-05-04 14:47:17.000000 scrapere-0.1.0/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-04 14:47:17.000000 scrapere-0.1.0/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-04 14:47:17.000000 scrapere-0.1.0/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-04 14:47:17.000000 scrapere-0.1.0/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-04 14:47:17.000000 scrapere-0.1.0/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-04 14:47:17.709921 scrapere-0.1.0/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      403 2023-05-04 10:44:41.000000 scrapere-0.1.0/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-04 14:59:40.054894 scrapere-0.1.1/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      177 2023-05-04 14:59:40.054894 scrapere-0.1.1/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      356 2023-05-04 10:42:22.000000 scrapere-0.1.1/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-04 14:59:40.050894 scrapere-0.1.1/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.1/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     4741 2023-05-04 10:04:57.000000 scrapere-0.1.1/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.1/scrapere/user-agents-unique.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-04 14:59:40.054894 scrapere-0.1.1/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      177 2023-05-04 14:59:40.000000 scrapere-0.1.1/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-04 14:59:40.000000 scrapere-0.1.1/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-04 14:59:40.000000 scrapere-0.1.1/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-04 14:59:40.000000 scrapere-0.1.1/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-04 14:59:40.000000 scrapere-0.1.1/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-04 14:59:40.054894 scrapere-0.1.1/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      427 2023-05-04 14:59:32.000000 scrapere-0.1.1/setup.py
```

### Comparing `scrapere-0.1.0/scrapere/toolbox.py` & `scrapere-0.1.1/scrapere/toolbox.py`

 * *Files identical despite different names*

### Comparing `scrapere-0.1.0/scrapere/user-agents-unique.txt` & `scrapere-0.1.1/scrapere/user-agents-unique.txt`

 * *Files identical despite different names*

