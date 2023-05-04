# Comparing `tmp/vspyplugin-1.3.1.tar.gz` & `tmp/vspyplugin-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vspyplugin-1.3.1.tar", last modified: Sun Mar 26 17:38:07 2023, max compression
+gzip compressed data, was "vspyplugin-1.3.2.tar", last modified: Thu May  4 21:57:36 2023, max compression
```

## Comparing `vspyplugin-1.3.1.tar` & `vspyplugin-1.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:07.315336 vspyplugin-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-26 17:38:07.315336 vspyplugin-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-26 17:38:07.315336 vspyplugin-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:07.311336 vspyplugin-1.3.1/vspyplugin/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:07.315336 vspyplugin-1.3.1/vspyplugin/coroutines/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/coroutines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/coroutines/coros.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/coroutines/frame_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/coroutines/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/coroutines/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/cython.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-26 17:37:44.000000 vspyplugin-1.3.1/vspyplugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:07.315336 vspyplugin-1.3.1/vspyplugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-26 17:38:07.000000 vspyplugin-1.3.1/vspyplugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-26 17:38:07.000000 vspyplugin-1.3.1/vspyplugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:38:07.000000 vspyplugin-1.3.1/vspyplugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-26 17:38:07.000000 vspyplugin-1.3.1/vspyplugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-26 17:38:07.000000 vspyplugin-1.3.1/vspyplugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-26 17:38:07.000000 vspyplugin-1.3.1/vspyplugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:36.044978 vspyplugin-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-04 21:57:36.044978 vspyplugin-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 21:57:36.044978 vspyplugin-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:36.044978 vspyplugin-1.3.2/vspyplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:36.044978 vspyplugin-1.3.2/vspyplugin/coroutines/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/coroutines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/coroutines/coros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/coroutines/frame_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/coroutines/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/coroutines/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/cython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-04 21:57:09.000000 vspyplugin-1.3.2/vspyplugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:36.044978 vspyplugin-1.3.2/vspyplugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-04 21:57:36.000000 vspyplugin-1.3.2/vspyplugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-04 21:57:36.000000 vspyplugin-1.3.2/vspyplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:57:36.000000 vspyplugin-1.3.2/vspyplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 21:57:36.000000 vspyplugin-1.3.2/vspyplugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 21:57:36.000000 vspyplugin-1.3.2/vspyplugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 21:57:36.000000 vspyplugin-1.3.2/vspyplugin.egg-info/top_level.txt
```

### Comparing `vspyplugin-1.3.1/LICENSE` & `vspyplugin-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/PKG-INFO` & `vspyplugin-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspyplugin
-Version: 1.3.1
+Version: 1.3.2
 Summary: Package for simplifying writing VapourSynth "plugins" in python.
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-pyplugin
 Project-URL: Documentation, https://vspyplugin.encode.moe/en/latest/
```

### Comparing `vspyplugin-1.3.1/README.md` & `vspyplugin-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/setup.cfg` & `vspyplugin-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/setup.py` & `vspyplugin-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/__init__.py` & `vspyplugin-1.3.2/vspyplugin/__init__.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/abstracts.py` & `vspyplugin-1.3.2/vspyplugin/abstracts.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/backends.py` & `vspyplugin-1.3.2/vspyplugin/backends.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/base.py` & `vspyplugin-1.3.2/vspyplugin/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
         annotations = set(func.__annotations__.keys()) - {'return'}
 
         if not annotations:
             raise CustomTypeError(f'{self.__class__.__name__}: You must type hint the function!', self.__class__)
 
         if annotations - this_args:
-            raise CustomTypeError(f'{self.__class__.__name__}: Unkown arguments specified!', self.__class__)
+            raise CustomTypeError(f'{self.__class__.__name__}: Unknown arguments specified!', self.__class__)
 
         miss_args = this_args - annotations
 
         if 'self' in annotations:
             func = partial(func, self)
             annotations.remove('self')
```

### Comparing `vspyplugin-1.3.1/vspyplugin/cli.py` & `vspyplugin-1.3.2/vspyplugin/cli.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/coroutines/coros.py` & `vspyplugin-1.3.2/vspyplugin/coroutines/coros.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/coroutines/frame_eval.py` & `vspyplugin-1.3.2/vspyplugin/coroutines/frame_eval.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/coroutines/funcs.py` & `vspyplugin-1.3.2/vspyplugin/coroutines/funcs.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/coroutines/types.py` & `vspyplugin-1.3.2/vspyplugin/coroutines/types.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/cuda.py` & `vspyplugin-1.3.2/vspyplugin/cuda.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/cupy.py` & `vspyplugin-1.3.2/vspyplugin/cupy.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/cython.py` & `vspyplugin-1.3.2/vspyplugin/cython.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/exceptions.py` & `vspyplugin-1.3.2/vspyplugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/numpy.py` & `vspyplugin-1.3.2/vspyplugin/numpy.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/types.py` & `vspyplugin-1.3.2/vspyplugin/types.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin/utils.py` & `vspyplugin-1.3.2/vspyplugin/utils.py`

 * *Files identical despite different names*

### Comparing `vspyplugin-1.3.1/vspyplugin.egg-info/PKG-INFO` & `vspyplugin-1.3.2/vspyplugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspyplugin
-Version: 1.3.1
+Version: 1.3.2
 Summary: Package for simplifying writing VapourSynth "plugins" in python.
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-pyplugin
 Project-URL: Documentation, https://vspyplugin.encode.moe/en/latest/
```

### Comparing `vspyplugin-1.3.1/vspyplugin.egg-info/SOURCES.txt` & `vspyplugin-1.3.2/vspyplugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

