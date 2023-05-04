# Comparing `tmp/ncache-0.2.tar.gz` & `tmp/ncache-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncache-0.2.tar", last modified: Tue May  2 09:33:09 2023, max compression
+gzip compressed data, was "ncache-0.3.tar", last modified: Thu May  4 05:27:42 2023, max compression
```

## Comparing `ncache-0.2.tar` & `ncache-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-02 09:33:09.215727 ncache-0.2/
--rw-r--r--   0 ok        (1000) ok        (1000)     1798 2023-05-02 09:33:09.215727 ncache-0.2/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)      988 2023-02-13 21:10:03.000000 ncache-0.2/README.md
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-02 09:33:09.213727 ncache-0.2/ncache/
--rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-02-16 19:17:55.000000 ncache-0.2/ncache/__init__.py
--rw-r--r--   0 ok        (1000) ok        (1000)     2443 2023-05-02 09:32:46.000000 ncache-0.2/ncache/ncache.py
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-02 09:33:09.215727 ncache-0.2/ncache.egg-info/
--rw-r--r--   0 ok        (1000) ok        (1000)     1798 2023-05-02 09:33:08.000000 ncache-0.2/ncache.egg-info/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)      178 2023-05-02 09:33:09.000000 ncache-0.2/ncache.egg-info/SOURCES.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-02 09:33:08.000000 ncache-0.2/ncache.egg-info/dependency_links.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        7 2023-05-02 09:33:08.000000 ncache-0.2/ncache.egg-info/top_level.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-02 09:33:09.215727 ncache-0.2/setup.cfg
--rw-r--r--   0 ok        (1000) ok        (1000)     1052 2023-02-16 19:35:29.000000 ncache-0.2/setup.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-04 05:27:42.402165 ncache-0.3/
+-rw-r--r--   0 ok        (1000) ok        (1000)     1790 2023-05-04 05:27:42.402165 ncache-0.3/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)      980 2023-05-02 17:26:56.000000 ncache-0.3/README.md
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-04 05:27:42.397165 ncache-0.3/ncache/
+-rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-02-16 19:17:55.000000 ncache-0.3/ncache/__init__.py
+-rw-r--r--   0 ok        (1000) ok        (1000)     2786 2023-05-02 17:55:46.000000 ncache-0.3/ncache/ncache.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-04 05:27:42.401165 ncache-0.3/ncache.egg-info/
+-rw-r--r--   0 ok        (1000) ok        (1000)     1790 2023-05-04 05:27:34.000000 ncache-0.3/ncache.egg-info/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)      178 2023-05-04 05:27:37.000000 ncache-0.3/ncache.egg-info/SOURCES.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-04 05:27:34.000000 ncache-0.3/ncache.egg-info/dependency_links.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        7 2023-05-04 05:27:34.000000 ncache-0.3/ncache.egg-info/top_level.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-04 05:27:42.402165 ncache-0.3/setup.cfg
+-rw-r--r--   0 ok        (1000) ok        (1000)     1052 2023-02-16 19:35:29.000000 ncache-0.3/setup.py
```

### Comparing `ncache-0.2/PKG-INFO` & `ncache-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ncache
-Version: 0.2
+Version: 0.3
 Summary: A simple and lightweight dictionary-based persistent cache for storing python objects.
 Home-page: https://github.com/rsusik/ncache
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Description: # Nano cache
         
         <p align="center">
         <a href="https://pypi.org/project/ncache" target="_blank">
             <img src="https://img.shields.io/pypi/v/ncache?color=%2334D058&label=pypi%20package" alt="Package version">
         </a>
-        <a href="https://github.com/rsusik/staticpie/blob/master/LICENSE" target="_blank">
-            <img src="https://img.shields.io/github/license/rsusik/staticpie" alt="Package version">
+        <a href="https://github.com/rsusik/ncache/blob/main/LICENSE" target="_blank">
+            <img src="https://img.shields.io/github/license/rsusik/ncache" alt="Package version">
         </a>
         </p>
         
         A simple and lightweight dictionary-based persistent cache for storing python objects.
         
         ## Installation:
```

### Comparing `ncache-0.2/README.md` & `ncache-0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Nano cache
 
 <p align="center">
 <a href="https://pypi.org/project/ncache" target="_blank">
     <img src="https://img.shields.io/pypi/v/ncache?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
-<a href="https://github.com/rsusik/staticpie/blob/master/LICENSE" target="_blank">
-    <img src="https://img.shields.io/github/license/rsusik/staticpie" alt="Package version">
+<a href="https://github.com/rsusik/ncache/blob/main/LICENSE" target="_blank">
+    <img src="https://img.shields.io/github/license/rsusik/ncache" alt="Package version">
 </a>
 </p>
 
 A simple and lightweight dictionary-based persistent cache for storing python objects.
 
 ## Installation:
```

### Comparing `ncache-0.2/ncache/ncache.py` & `ncache-0.3/ncache/ncache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import hashlib
 import pickle
+from pathlib import Path
 from typing import Any
 import os
 
-__version__ = '0.2'
+__version__ = '0.3'
 
 class Cache:
     def __init__(self, 
         filename:str, 
         nocache:bool=False, 
         tmpfilename:str=None # if None no temp file is created
     ):
         self.filename = filename
         if tmpfilename is None:
-            self.tmpfilename = self.filename
-        else:
-            self.tmpfilename = tmpfilename
+            tmpfilename = Path(filename).parent / f'~{Path(filename).name}.tmp'
+        self.tmpfilename = tmpfilename
         self.nocache = nocache
         self.cache = {}
+
+        def check_path(path:str):
+            if Path(path).is_dir():
+                raise Exception(f'Error: The path "{path}" is a difectory')
+        for p in [self.filename, self.tmpfilename]:
+            check_path(p)
+        
     
     def if_cache_on(alt_exception=None, alt_value=None):
         def wrapper(fun):
             def inner(self, *args, **kwargs):
                 if self.nocache == False:
                     return fun(self, *args, **kwargs)
                 else:
@@ -56,14 +63,18 @@
         with open(self.tmpfilename, 'wb') as f:
             pickle.dump(self.cache, f)
             os.rename(self.tmpfilename, self.filename)
 
     class NoCacheValue(Exception):
         pass
 
+    @property
+    def data(self)->dict:
+        return self.cache
+
     @if_cache_on(alt_exception=NoCacheValue())
     def get_value(self, obj:Any)->Any:
         _hash = self.get_hash(obj)
         if _hash in self.cache.keys():
             val = self.cache[_hash]
             copy_fun = getattr(val, 'copy', None)
             if callable(copy_fun):
```

### Comparing `ncache-0.2/ncache.egg-info/PKG-INFO` & `ncache-0.3/ncache.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ncache
-Version: 0.2
+Version: 0.3
 Summary: A simple and lightweight dictionary-based persistent cache for storing python objects.
 Home-page: https://github.com/rsusik/ncache
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Description: # Nano cache
         
         <p align="center">
         <a href="https://pypi.org/project/ncache" target="_blank">
             <img src="https://img.shields.io/pypi/v/ncache?color=%2334D058&label=pypi%20package" alt="Package version">
         </a>
-        <a href="https://github.com/rsusik/staticpie/blob/master/LICENSE" target="_blank">
-            <img src="https://img.shields.io/github/license/rsusik/staticpie" alt="Package version">
+        <a href="https://github.com/rsusik/ncache/blob/main/LICENSE" target="_blank">
+            <img src="https://img.shields.io/github/license/rsusik/ncache" alt="Package version">
         </a>
         </p>
         
         A simple and lightweight dictionary-based persistent cache for storing python objects.
         
         ## Installation:
```

### Comparing `ncache-0.2/setup.py` & `ncache-0.3/setup.py`

 * *Files identical despite different names*

