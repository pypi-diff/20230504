# Comparing `tmp/MirSerializer-1.0.1.tar.gz` & `tmp/MirSerializer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MirSerializer-1.0.1.tar", last modified: Thu May  4 10:54:38 2023, max compression
+gzip compressed data, was "MirSerializer-1.0.2.tar", last modified: Thu May  4 11:01:22 2023, max compression
```

## Comparing `MirSerializer-1.0.1.tar` & `MirSerializer-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 10:54:38.627238 MirSerializer-1.0.1/
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 10:54:38.627238 MirSerializer-1.0.1/MirSerializer.egg-info/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 10:54:38.000000 MirSerializer-1.0.1/MirSerializer.egg-info/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      193 2023-05-04 10:54:38.000000 MirSerializer-1.0.1/MirSerializer.egg-info/SOURCES.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-04 10:54:38.000000 MirSerializer-1.0.1/MirSerializer.egg-info/dependency_links.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       31 2023-05-04 10:54:38.000000 MirSerializer-1.0.1/MirSerializer.egg-info/top_level.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 10:54:38.627238 MirSerializer-1.0.1/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     7769 2023-04-26 13:13:34.000000 MirSerializer-1.0.1/json_serializer.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-04 10:54:38.627238 MirSerializer-1.0.1/setup.cfg
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      339 2023-05-04 10:54:16.000000 MirSerializer-1.0.1/setup.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     7943 2023-04-30 12:33:51.000000 MirSerializer-1.0.1/xml_serializer.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 11:01:22.698001 MirSerializer-1.0.2/
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 11:01:22.698001 MirSerializer-1.0.2/MirSerializer.egg-info/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 11:01:22.000000 MirSerializer-1.0.2/MirSerializer.egg-info/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      215 2023-05-04 11:01:22.000000 MirSerializer-1.0.2/MirSerializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-04 11:01:22.000000 MirSerializer-1.0.2/MirSerializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       47 2023-05-04 11:01:22.000000 MirSerializer-1.0.2/MirSerializer.egg-info/top_level.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 11:01:22.698001 MirSerializer-1.0.2/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      323 2023-05-03 15:01:37.000000 MirSerializer-1.0.2/factory.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     7769 2023-04-26 13:13:34.000000 MirSerializer-1.0.2/json_serializer.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     9183 2023-05-04 10:13:04.000000 MirSerializer-1.0.2/packing.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-04 11:01:22.698001 MirSerializer-1.0.2/setup.cfg
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      361 2023-05-04 11:01:21.000000 MirSerializer-1.0.2/setup.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     7943 2023-04-30 12:33:51.000000 MirSerializer-1.0.2/xml_serializer.py
```

### Comparing `MirSerializer-1.0.1/json_serializer.py` & `MirSerializer-1.0.2/json_serializer.py`

 * *Files identical despite different names*

### Comparing `MirSerializer-1.0.1/xml_serializer.py` & `MirSerializer-1.0.2/xml_serializer.py`

 * *Files identical despite different names*

