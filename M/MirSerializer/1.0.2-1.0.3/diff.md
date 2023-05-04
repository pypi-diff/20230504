# Comparing `tmp/MirSerializer-1.0.2.tar.gz` & `tmp/MirSerializer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MirSerializer-1.0.2.tar", last modified: Thu May  4 11:01:22 2023, max compression
+gzip compressed data, was "MirSerializer-1.0.3.tar", last modified: Thu May  4 15:52:48 2023, max compression
```

## Comparing `MirSerializer-1.0.2.tar` & `MirSerializer-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 11:01:22.698001 MirSerializer-1.0.2/
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 11:01:22.698001 MirSerializer-1.0.2/MirSerializer.egg-info/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 11:01:22.000000 MirSerializer-1.0.2/MirSerializer.egg-info/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      215 2023-05-04 11:01:22.000000 MirSerializer-1.0.2/MirSerializer.egg-info/SOURCES.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-04 11:01:22.000000 MirSerializer-1.0.2/MirSerializer.egg-info/dependency_links.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       47 2023-05-04 11:01:22.000000 MirSerializer-1.0.2/MirSerializer.egg-info/top_level.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 11:01:22.698001 MirSerializer-1.0.2/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      323 2023-05-03 15:01:37.000000 MirSerializer-1.0.2/factory.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     7769 2023-04-26 13:13:34.000000 MirSerializer-1.0.2/json_serializer.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     9183 2023-05-04 10:13:04.000000 MirSerializer-1.0.2/packing.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-04 11:01:22.698001 MirSerializer-1.0.2/setup.cfg
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      361 2023-05-04 11:01:21.000000 MirSerializer-1.0.2/setup.py
--rw-rw-r--   0 ilya      (1000) ilya      (1000)     7943 2023-04-30 12:33:51.000000 MirSerializer-1.0.2/xml_serializer.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 15:52:48.320055 MirSerializer-1.0.3/
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 15:52:48.320055 MirSerializer-1.0.3/MirSerializer/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       54 2023-04-25 15:56:43.000000 MirSerializer-1.0.3/MirSerializer/CONSTANTS.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      109 2023-05-04 15:41:02.000000 MirSerializer-1.0.3/MirSerializer/__init__.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      323 2023-05-03 15:01:37.000000 MirSerializer-1.0.3/MirSerializer/factory.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     7783 2023-05-04 15:52:14.000000 MirSerializer-1.0.3/MirSerializer/json_serializer.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     9174 2023-05-04 15:52:14.000000 MirSerializer-1.0.3/MirSerializer/packing.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     7971 2023-05-04 15:52:14.000000 MirSerializer-1.0.3/MirSerializer/xml_serializer.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-04 15:52:48.320055 MirSerializer-1.0.3/MirSerializer.egg-info/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 15:52:48.000000 MirSerializer-1.0.3/MirSerializer.egg-info/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      324 2023-05-04 15:52:48.000000 MirSerializer-1.0.3/MirSerializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-04 15:52:48.000000 MirSerializer-1.0.3/MirSerializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       14 2023-05-04 15:52:48.000000 MirSerializer-1.0.3/MirSerializer.egg-info/top_level.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      221 2023-05-04 15:52:48.320055 MirSerializer-1.0.3/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-04 15:52:48.320055 MirSerializer-1.0.3/setup.cfg
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      287 2023-05-04 15:52:42.000000 MirSerializer-1.0.3/setup.py
```

### Comparing `MirSerializer-1.0.2/json_serializer.py` & `MirSerializer-1.0.3/MirSerializer/json_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from packing import convert, deconvert
-from CONSTANTS import PRIMITIVE_TYPES
+from MirSerializer.CONSTANTS import PRIMITIVE_TYPES
 
 
 class Json:
     def __init__(self):
         self._current_position = 0
         self._indent = 0
```

### Comparing `MirSerializer-1.0.2/packing.py` & `MirSerializer-1.0.3/MirSerializer/packing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import builtins
 import types
-from CONSTANTS import PRIMITIVE_TYPES
+from MirSerializer.CONSTANTS import PRIMITIVE_TYPES
 from types import FunctionType, BuiltinFunctionType, LambdaType, CodeType, GetSetDescriptorType, \
-    MethodDescriptorType, WrapperDescriptorType
+    MethodDescriptorType
 
 
 def is_function(obj):
     return inspect.isfunction(obj) or inspect.ismethod(obj) or isinstance(obj, LambdaType)
 
 
 def is_iterable(obj):
```

### Comparing `MirSerializer-1.0.2/xml_serializer.py` & `MirSerializer-1.0.3/MirSerializer/xml_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from packing import convert, deconvert
-from CONSTANTS import PRIMITIVE_TYPES
+from MirSerializer.packing import convert, deconvert
+from MirSerializer.CONSTANTS import PRIMITIVE_TYPES
 
 
 class Xml:
     def __init__(self):
         self._dict_counter = 0
         self._current_position = 0
         self._indent = 0
```

