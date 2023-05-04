# Comparing `tmp/MirSerializer-1.0.4.tar.gz` & `tmp/MirSerializer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MirSerializer-1.0.4.tar", last modified: Thu May  4 17:22:14 2023, max compression
+gzip compressed data, was "MirSerializer-2.0.0.tar", last modified: Thu May  4 17:24:05 2023, max compression
```

## Comparing `MirSerializer-1.0.4.tar` & `MirSerializer-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 17:22:14.837479 MirSerializer-1.0.4/
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 17:22:14.837479 MirSerializer-1.0.4/MirSerializer/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       54 2023-05-04 17:21:45.000000 MirSerializer-1.0.4/MirSerializer/CONSTANTS.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      194 2023-05-04 17:21:45.000000 MirSerializer-1.0.4/MirSerializer/__init__.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      323 2023-05-04 17:21:45.000000 MirSerializer-1.0.4/MirSerializer/factory.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     7783 2023-05-04 17:21:45.000000 MirSerializer-1.0.4/MirSerializer/json_serializer.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     9174 2023-05-04 17:21:45.000000 MirSerializer-1.0.4/MirSerializer/packing.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     7971 2023-05-04 17:21:45.000000 MirSerializer-1.0.4/MirSerializer/xml_serializer.py
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 17:22:14.837479 MirSerializer-1.0.4/MirSerializer.egg-info/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 17:22:14.000000 MirSerializer-1.0.4/MirSerializer.egg-info/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      324 2023-05-04 17:22:14.000000 MirSerializer-1.0.4/MirSerializer.egg-info/SOURCES.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-04 17:22:14.000000 MirSerializer-1.0.4/MirSerializer.egg-info/dependency_links.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       14 2023-05-04 17:22:14.000000 MirSerializer-1.0.4/MirSerializer.egg-info/top_level.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 17:22:14.837479 MirSerializer-1.0.4/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-04 17:22:14.837479 MirSerializer-1.0.4/setup.cfg
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      287 2023-05-04 17:22:12.000000 MirSerializer-1.0.4/setup.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 17:24:05.863335 MirSerializer-2.0.0/
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 17:24:05.863335 MirSerializer-2.0.0/MirSerializer/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       54 2023-05-04 17:21:45.000000 MirSerializer-2.0.0/MirSerializer/CONSTANTS.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      194 2023-05-04 17:21:45.000000 MirSerializer-2.0.0/MirSerializer/__init__.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      351 2023-05-04 17:24:02.000000 MirSerializer-2.0.0/MirSerializer/factory.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     7797 2023-05-04 17:24:02.000000 MirSerializer-2.0.0/MirSerializer/json_serializer.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     9174 2023-05-04 17:21:45.000000 MirSerializer-2.0.0/MirSerializer/packing.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     7971 2023-05-04 17:21:45.000000 MirSerializer-2.0.0/MirSerializer/xml_serializer.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 17:24:05.863335 MirSerializer-2.0.0/MirSerializer.egg-info/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 17:24:05.000000 MirSerializer-2.0.0/MirSerializer.egg-info/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      324 2023-05-04 17:24:05.000000 MirSerializer-2.0.0/MirSerializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-04 17:24:05.000000 MirSerializer-2.0.0/MirSerializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       14 2023-05-04 17:24:05.000000 MirSerializer-2.0.0/MirSerializer.egg-info/top_level.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 17:24:05.863335 MirSerializer-2.0.0/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-04 17:24:05.863335 MirSerializer-2.0.0/setup.cfg
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      287 2023-05-04 17:24:02.000000 MirSerializer-2.0.0/setup.py
```

### Comparing `MirSerializer-1.0.4/MirSerializer/json_serializer.py` & `MirSerializer-2.0.0/MirSerializer/json_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from packing import convert, deconvert
+from MirSerializer.packing import convert, deconvert
 from MirSerializer.CONSTANTS import PRIMITIVE_TYPES
 
 
 class Json:
     def __init__(self):
         self._current_position = 0
         self._indent = 0
```

### Comparing `MirSerializer-1.0.4/MirSerializer/packing.py` & `MirSerializer-2.0.0/MirSerializer/packing.py`

 * *Files identical despite different names*

### Comparing `MirSerializer-1.0.4/MirSerializer/xml_serializer.py` & `MirSerializer-2.0.0/MirSerializer/xml_serializer.py`

 * *Files identical despite different names*

