# Comparing `tmp/cagpaint-0.1.0.tar.gz` & `tmp/cagpaint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagpaint-0.1.0.tar", last modified: Thu May  4 12:24:51 2023, max compression
+gzip compressed data, was "cagpaint-0.1.1.tar", last modified: Thu May  4 14:50:43 2023, max compression
```

## Comparing `cagpaint-0.1.0.tar` & `cagpaint-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 12:24:51.050377 cagpaint-0.1.0/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-20 07:40:57.000000 cagpaint-0.1.0/LICENSE
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 12:24:51.050377 cagpaint-0.1.0/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      242 2022-09-20 12:22:50.000000 cagpaint-0.1.0/README.md
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 12:24:51.050377 cagpaint-0.1.0/cagpaint.egg-info/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 12:24:51.000000 cagpaint-0.1.0/cagpaint.egg-info/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      154 2023-05-04 12:24:51.000000 cagpaint-0.1.0/cagpaint.egg-info/SOURCES.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-04 12:24:51.000000 cagpaint-0.1.0/cagpaint.egg-info/dependency_links.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-04 12:24:51.000000 cagpaint-0.1.0/cagpaint.egg-info/top_level.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)       38 2023-05-04 12:24:51.050377 cagpaint-0.1.0/setup.cfg
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      397 2023-05-04 12:23:54.000000 cagpaint-0.1.0/setup.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 14:50:43.417699 cagpaint-0.1.1/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-20 07:40:57.000000 cagpaint-0.1.1/LICENSE
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 14:50:43.417699 cagpaint-0.1.1/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      242 2022-09-20 12:22:50.000000 cagpaint-0.1.1/README.md
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-05-04 14:50:43.417699 cagpaint-0.1.1/cagpaint.egg-info/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      215 2023-05-04 14:50:43.000000 cagpaint-0.1.1/cagpaint.egg-info/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      154 2023-05-04 14:50:43.000000 cagpaint-0.1.1/cagpaint.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-04 14:50:43.000000 cagpaint-0.1.1/cagpaint.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-05-04 14:50:43.000000 cagpaint-0.1.1/cagpaint.egg-info/top_level.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)       38 2023-05-04 14:50:43.417699 cagpaint-0.1.1/setup.cfg
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      397 2023-05-04 14:49:48.000000 cagpaint-0.1.1/setup.py
```

### Comparing `cagpaint-0.1.0/LICENSE` & `cagpaint-0.1.1/LICENSE`

 * *Files identical despite different names*

