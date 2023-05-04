# Comparing `tmp/rpgPy-0.8.0.tar.gz` & `tmp/rpgPy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rpgPy-0.8.0.tar", last modified: Wed Feb 24 14:13:22 2021, max compression
+gzip compressed data, was "dist/rpgPy-0.9.0.tar", last modified: Fri Sep  3 07:48:23 2021, max compression
```

## Comparing `rpgPy-0.8.0.tar` & `rpgPy-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-24 14:13:22.000000 rpgPy-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-02-24 14:13:07.000000 rpgPy-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2021-02-24 14:13:22.000000 rpgPy-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-02-24 14:13:07.000000 rpgPy-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-02-24 14:13:07.000000 rpgPy-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-24 14:13:22.000000 rpgPy-0.8.0/rpgPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2021-02-24 14:13:22.000000 rpgPy-0.8.0/rpgPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-02-24 14:13:22.000000 rpgPy-0.8.0/rpgPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-24 14:13:22.000000 rpgPy-0.8.0/rpgPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      330 2021-02-24 14:13:22.000000 rpgPy-0.8.0/rpgPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-02-24 14:13:22.000000 rpgPy-0.8.0/rpgPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2021-02-24 14:13:07.000000 rpgPy-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-24 14:13:22.000000 rpgPy-0.8.0/rpgpy/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-02-24 14:13:07.000000 rpgPy-0.8.0/rpgpy/version.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-02-24 14:13:07.000000 rpgPy-0.8.0/rpgpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14675 2021-02-24 14:13:07.000000 rpgPy-0.8.0/rpgpy/data.pyx
--rw-r--r--   0 runner    (1001) docker     (121)  1285233 2021-02-24 14:13:22.000000 rpgPy-0.8.0/rpgpy/data.c
--rw-r--r--   0 runner    (1001) docker     (121)     4834 2021-02-24 14:13:07.000000 rpgPy-0.8.0/rpgpy/spcutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-02-24 14:13:07.000000 rpgPy-0.8.0/rpgpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13166 2021-02-24 14:13:07.000000 rpgPy-0.8.0/rpgpy/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     4316 2021-02-24 14:13:07.000000 rpgPy-0.8.0/rpgpy/header.py
--rw-r--r--   0 runner    (1001) docker     (121)     5284 2021-02-24 14:13:07.000000 rpgPy-0.8.0/rpgpy/nc.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-24 14:13:22.000000 rpgPy-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 07:48:23.000000 rpgPy-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-03 07:48:23.000000 rpgPy-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4382 2021-09-03 07:48:23.000000 rpgPy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-09-03 07:48:10.000000 rpgPy-0.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-09-03 07:48:10.000000 rpgPy-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     3088 2021-09-03 07:48:10.000000 rpgPy-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 07:48:23.000000 rpgPy-0.9.0/rpgPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2021-09-03 07:48:23.000000 rpgPy-0.9.0/rpgPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-09-03 07:48:22.000000 rpgPy-0.9.0/rpgPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4382 2021-09-03 07:48:22.000000 rpgPy-0.9.0/rpgPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-03 07:48:22.000000 rpgPy-0.9.0/rpgPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-03 07:48:22.000000 rpgPy-0.9.0/rpgPy.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 07:48:23.000000 rpgPy-0.9.0/rpgpy/
+-rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-09-03 07:48:10.000000 rpgPy-0.9.0/rpgpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7578 2021-09-03 07:48:10.000000 rpgPy-0.9.0/rpgpy/nc.py
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-09-03 07:48:10.000000 rpgPy-0.9.0/rpgpy/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4834 2021-09-03 07:48:10.000000 rpgPy-0.9.0/rpgpy/spcutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)  1285634 2021-09-03 07:48:22.000000 rpgPy-0.9.0/rpgpy/data.c
+-rw-r--r--   0 runner    (1001) docker     (121)    13166 2021-09-03 07:48:10.000000 rpgPy-0.9.0/rpgpy/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4316 2021-09-03 07:48:10.000000 rpgPy-0.9.0/rpgpy/header.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-09-03 07:48:10.000000 rpgPy-0.9.0/rpgpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14675 2021-09-03 07:48:10.000000 rpgPy-0.9.0/rpgpy/data.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-09-03 07:48:10.000000 rpgPy-0.9.0/MANIFEST.in
```

### Comparing `rpgPy-0.8.0/PKG-INFO` & `rpgPy-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rpgPy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Cython code for reading binary files from RPG cloud radar.
 Home-page: https://github.com/actris-cloudnet/rpgpy
 Author: Simo Tukiainen
 Author-email: simo.tukiainen@fmi.fi
 License: MIT License
 Description: # rpgPy
         
         ![](https://github.com/actris-cloudnet/rpgpy/workflows/RpgPy%20CI/badge.svg)
         [![PyPI version](https://badge.fury.io/py/rpgPy.svg)](https://badge.fury.io/py/rpgPy)
         
-        RpgPy is a Python / Cython software for reading [RPG cloud radar](https://www.radiometer-physics.de/products/microwave-remote-sensing-instruments/94-ghz-fmcw-doppler-cloud-radar/) Level 0 and Level 1 binary files.
+        RpgPy is a Python / Cython software for reading [RPG cloud radar](https://www.radiometer-physics.de/products/microwave-remote-sensing-instruments/94-ghz-fmcw-doppler-cloud-radar/) Level 0 and Level 1 binary files and converting to netCDF4.
         
         # Installation
         
         ## From PyPI
         ```
         $ python3 -m pip install rpgpy
         ```
@@ -41,33 +41,47 @@
         >>> header, data = read_rpg('rpg_file.LV0')
         ```
         By default, the ```header``` and ```data``` dictionary key names are taken from the RPG manual. Optionally, 
         more explicit key names can be chosen:
         ```python
         >>> header, data = read_rpg('rpg_file.LV0', rpg_names=False)
         ```
-        ### Converting to NetCDF4
+        ### Converting single file to single netCDF4
         ```python
         >>> from rpgpy import rpg2nc
         >>> rpg2nc('rpg_file.LV0', 'rpg_file.nc')
         ```
         This works for both Level 0 and Level 1 files.
         
         In addition to the default global attributes, it is possible to provide 
         additional ones via a dictionary:
         ```python
         >>> attr = {'attr1': 'foo', 'attr2': 42}
         >>> rpg2nc('rpg_file.LV0', 'rpg_file.nc', global_attr=attr)
         ```
+        
+        ### Converting multiple files to single netCDF4
         Several RPG files can be concatenated to singe netCDF file using wildcard.
         With Level 0 data, this can lead to a very large netCDF file.
         ```python
         >>> rpg2nc('/path/to/files/*.LV0', 'huge_file.nc')
         ```
         
+        ### Converting multiple files to corresponding netCDF4 files
+        Several RPG files can be converted to corresponding individual netCDF4 files using `rpg2nc_multi` function.
+        Every file with extension `.LV0`, `.lv0`, `.LV1` or `.lv1` in every subdirectory of the specified path will be converted.  
+        Optionally, the user can exclude Level 0 files by switching the argument of `include_lv0` parameter to `False`.
+        ```python
+        >>> from rpgpy import rpg2nc_multi
+        >>> rpg2nc_multi('/path/to/myfiles', include_lv0=True, base_name"foo")
+        ```
+        If no path is made explicit, the function will by default take as argument the current directory
+        and write the converted files in it.  
+        If the parameter `base_name` is specified, the function will rename the new files as `basename_oldname`.
+        
         ## Tests
         Run unit tests:
         ```
         (venv) $ pytest
         ```
         
         Run end-to-end tests:
```

### Comparing `rpgPy-0.8.0/setup.py` & `rpgPy-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `rpgPy-0.8.0/rpgPy.egg-info/PKG-INFO` & `rpgPy-0.9.0/rpgPy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rpgPy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Cython code for reading binary files from RPG cloud radar.
 Home-page: https://github.com/actris-cloudnet/rpgpy
 Author: Simo Tukiainen
 Author-email: simo.tukiainen@fmi.fi
 License: MIT License
 Description: # rpgPy
         
         ![](https://github.com/actris-cloudnet/rpgpy/workflows/RpgPy%20CI/badge.svg)
         [![PyPI version](https://badge.fury.io/py/rpgPy.svg)](https://badge.fury.io/py/rpgPy)
         
-        RpgPy is a Python / Cython software for reading [RPG cloud radar](https://www.radiometer-physics.de/products/microwave-remote-sensing-instruments/94-ghz-fmcw-doppler-cloud-radar/) Level 0 and Level 1 binary files.
+        RpgPy is a Python / Cython software for reading [RPG cloud radar](https://www.radiometer-physics.de/products/microwave-remote-sensing-instruments/94-ghz-fmcw-doppler-cloud-radar/) Level 0 and Level 1 binary files and converting to netCDF4.
         
         # Installation
         
         ## From PyPI
         ```
         $ python3 -m pip install rpgpy
         ```
@@ -41,33 +41,47 @@
         >>> header, data = read_rpg('rpg_file.LV0')
         ```
         By default, the ```header``` and ```data``` dictionary key names are taken from the RPG manual. Optionally, 
         more explicit key names can be chosen:
         ```python
         >>> header, data = read_rpg('rpg_file.LV0', rpg_names=False)
         ```
-        ### Converting to NetCDF4
+        ### Converting single file to single netCDF4
         ```python
         >>> from rpgpy import rpg2nc
         >>> rpg2nc('rpg_file.LV0', 'rpg_file.nc')
         ```
         This works for both Level 0 and Level 1 files.
         
         In addition to the default global attributes, it is possible to provide 
         additional ones via a dictionary:
         ```python
         >>> attr = {'attr1': 'foo', 'attr2': 42}
         >>> rpg2nc('rpg_file.LV0', 'rpg_file.nc', global_attr=attr)
         ```
+        
+        ### Converting multiple files to single netCDF4
         Several RPG files can be concatenated to singe netCDF file using wildcard.
         With Level 0 data, this can lead to a very large netCDF file.
         ```python
         >>> rpg2nc('/path/to/files/*.LV0', 'huge_file.nc')
         ```
         
+        ### Converting multiple files to corresponding netCDF4 files
+        Several RPG files can be converted to corresponding individual netCDF4 files using `rpg2nc_multi` function.
+        Every file with extension `.LV0`, `.lv0`, `.LV1` or `.lv1` in every subdirectory of the specified path will be converted.  
+        Optionally, the user can exclude Level 0 files by switching the argument of `include_lv0` parameter to `False`.
+        ```python
+        >>> from rpgpy import rpg2nc_multi
+        >>> rpg2nc_multi('/path/to/myfiles', include_lv0=True, base_name"foo")
+        ```
+        If no path is made explicit, the function will by default take as argument the current directory
+        and write the converted files in it.  
+        If the parameter `base_name` is specified, the function will rename the new files as `basename_oldname`.
+        
         ## Tests
         Run unit tests:
         ```
         (venv) $ pytest
         ```
         
         Run end-to-end tests:
```

### Comparing `rpgPy-0.8.0/README.md` & `rpgPy-0.9.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # rpgPy
 
 ![](https://github.com/actris-cloudnet/rpgpy/workflows/RpgPy%20CI/badge.svg)
 [![PyPI version](https://badge.fury.io/py/rpgPy.svg)](https://badge.fury.io/py/rpgPy)
 
-RpgPy is a Python / Cython software for reading [RPG cloud radar](https://www.radiometer-physics.de/products/microwave-remote-sensing-instruments/94-ghz-fmcw-doppler-cloud-radar/) Level 0 and Level 1 binary files.
+RpgPy is a Python / Cython software for reading [RPG cloud radar](https://www.radiometer-physics.de/products/microwave-remote-sensing-instruments/94-ghz-fmcw-doppler-cloud-radar/) Level 0 and Level 1 binary files and converting to netCDF4.
 
 # Installation
 
 ## From PyPI
 ```
 $ python3 -m pip install rpgpy
 ```
@@ -33,33 +33,47 @@
 >>> header, data = read_rpg('rpg_file.LV0')
 ```
 By default, the ```header``` and ```data``` dictionary key names are taken from the RPG manual. Optionally, 
 more explicit key names can be chosen:
 ```python
 >>> header, data = read_rpg('rpg_file.LV0', rpg_names=False)
 ```
-### Converting to NetCDF4
+### Converting single file to single netCDF4
 ```python
 >>> from rpgpy import rpg2nc
 >>> rpg2nc('rpg_file.LV0', 'rpg_file.nc')
 ```
 This works for both Level 0 and Level 1 files.
 
 In addition to the default global attributes, it is possible to provide 
 additional ones via a dictionary:
 ```python
 >>> attr = {'attr1': 'foo', 'attr2': 42}
 >>> rpg2nc('rpg_file.LV0', 'rpg_file.nc', global_attr=attr)
 ```
+
+### Converting multiple files to single netCDF4
 Several RPG files can be concatenated to singe netCDF file using wildcard.
 With Level 0 data, this can lead to a very large netCDF file.
 ```python
 >>> rpg2nc('/path/to/files/*.LV0', 'huge_file.nc')
 ```
 
+### Converting multiple files to corresponding netCDF4 files
+Several RPG files can be converted to corresponding individual netCDF4 files using `rpg2nc_multi` function.
+Every file with extension `.LV0`, `.lv0`, `.LV1` or `.lv1` in every subdirectory of the specified path will be converted.  
+Optionally, the user can exclude Level 0 files by switching the argument of `include_lv0` parameter to `False`.
+```python
+>>> from rpgpy import rpg2nc_multi
+>>> rpg2nc_multi('/path/to/myfiles', include_lv0=True, base_name"foo")
+```
+If no path is made explicit, the function will by default take as argument the current directory
+and write the converted files in it.  
+If the parameter `base_name` is specified, the function will rename the new files as `basename_oldname`.
+
 ## Tests
 Run unit tests:
 ```
 (venv) $ pytest
 ```
 
 Run end-to-end tests:
```

### Comparing `rpgPy-0.8.0/rpgpy/data.pyx` & `rpgPy-0.9.0/rpgpy/data.pyx`

 * *Files identical despite different names*

### Comparing `rpgPy-0.8.0/rpgpy/data.c` & `rpgPy-0.9.0/rpgpy/data.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-/* Generated by Cython 0.29.22 */
+/* Generated by Cython 0.29.24 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "rpgpy.data",
         "sources": [
             "rpgpy/data.pyx"
         ]
     },
     "module_name": "rpgpy.data"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_22"
-#define CYTHON_HEX_VERSION 0x001D16F0
+#define CYTHON_ABI "0_29_24"
+#define CYTHON_HEX_VERSION 0x001D18F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -435,25 +437,33 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
+  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
+  #else
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
   #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
+  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #endif
   #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
@@ -1713,14 +1723,58 @@
 static CYTHON_INLINE PyObject *__pyx_capsule_create(void *p, const char *sig);
 
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
+/* IsLittleEndian.proto */
+static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
+
+/* BufferFormatCheck.proto */
+static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
+static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
+                              __Pyx_BufFmt_StackElem* stack,
+                              __Pyx_TypeInfo* type);
+
+/* TypeInfoCompare.proto */
+static int __pyx_typeinfo_cmp(__Pyx_TypeInfo *a, __Pyx_TypeInfo *b);
+
+/* MemviewSliceValidateAndInit.proto */
+static int __Pyx_ValidateAndInit_memviewslice(
+                int *axes_specs,
+                int c_or_f_flag,
+                int buf_flags,
+                int ndim,
+                __Pyx_TypeInfo *dtype,
+                __Pyx_BufFmt_StackElem stack[],
+                __Pyx_memviewslice *memviewslice,
+                PyObject *original_obj);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_int(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_unsigned_int(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_char(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_float(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_float(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_char(PyObject *, int writable_flag);
+
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_char(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_char(const char *itemp, PyObject *obj);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_float(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_float(const char *itemp, PyObject *obj);
@@ -1766,58 +1820,14 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
-/* IsLittleEndian.proto */
-static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
-
-/* BufferFormatCheck.proto */
-static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
-static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
-                              __Pyx_BufFmt_StackElem* stack,
-                              __Pyx_TypeInfo* type);
-
-/* TypeInfoCompare.proto */
-static int __pyx_typeinfo_cmp(__Pyx_TypeInfo *a, __Pyx_TypeInfo *b);
-
-/* MemviewSliceValidateAndInit.proto */
-static int __Pyx_ValidateAndInit_memviewslice(
-                int *axes_specs,
-                int c_or_f_flag,
-                int buf_flags,
-                int ndim,
-                __Pyx_TypeInfo *dtype,
-                __Pyx_BufFmt_StackElem stack[],
-                __Pyx_memviewslice *memviewslice,
-                PyObject *original_obj);
-
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_int(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_unsigned_int(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_char(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_float(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_float(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_char(PyObject *, int writable_flag);
-
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
@@ -26238,19 +26248,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("data", __pyx_methods, __pyx_k_RPG_cloud_radar_binary_reader_in, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -27079,15 +27087,15 @@
 #endif
 #endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -29825,64 +29833,960 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+/* IsLittleEndian */
+static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
+{
+  union {
+    uint32_t u32;
+    uint8_t u8[4];
+  } S;
+  S.u32 = 0x01020304;
+  return S.u8[0] == 4;
+}
+
+/* BufferFormatCheck */
+static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
+                              __Pyx_BufFmt_StackElem* stack,
+                              __Pyx_TypeInfo* type) {
+  stack[0].field = &ctx->root;
+  stack[0].parent_offset = 0;
+  ctx->root.type = type;
+  ctx->root.name = "buffer dtype";
+  ctx->root.offset = 0;
+  ctx->head = stack;
+  ctx->head->field = &ctx->root;
+  ctx->fmt_offset = 0;
+  ctx->head->parent_offset = 0;
+  ctx->new_packmode = '@';
+  ctx->enc_packmode = '@';
+  ctx->new_count = 1;
+  ctx->enc_count = 0;
+  ctx->enc_type = 0;
+  ctx->is_complex = 0;
+  ctx->is_valid_array = 0;
+  ctx->struct_alignment = 0;
+  while (type->typegroup == 'S') {
+    ++ctx->head;
+    ctx->head->field = type->fields;
+    ctx->head->parent_offset = 0;
+    type = type->fields->type;
+  }
+}
+static int __Pyx_BufFmt_ParseNumber(const char** ts) {
+    int count;
+    const char* t = *ts;
+    if (*t < '0' || *t > '9') {
+      return -1;
+    } else {
+        count = *t++ - '0';
+        while (*t >= '0' && *t <= '9') {
+            count *= 10;
+            count += *t++ - '0';
+        }
+    }
+    *ts = t;
+    return count;
+}
+static int __Pyx_BufFmt_ExpectNumber(const char **ts) {
+    int number = __Pyx_BufFmt_ParseNumber(ts);
+    if (number == -1)
+        PyErr_Format(PyExc_ValueError,\
+                     "Does not understand character buffer dtype format string ('%c')", **ts);
+    return number;
+}
+static void __Pyx_BufFmt_RaiseUnexpectedChar(char ch) {
+  PyErr_Format(PyExc_ValueError,
+               "Unexpected format string character: '%c'", ch);
+}
+static const char* __Pyx_BufFmt_DescribeTypeChar(char ch, int is_complex) {
+  switch (ch) {
+    case '?': return "'bool'";
+    case 'c': return "'char'";
+    case 'b': return "'signed char'";
+    case 'B': return "'unsigned char'";
+    case 'h': return "'short'";
+    case 'H': return "'unsigned short'";
+    case 'i': return "'int'";
+    case 'I': return "'unsigned int'";
+    case 'l': return "'long'";
+    case 'L': return "'unsigned long'";
+    case 'q': return "'long long'";
+    case 'Q': return "'unsigned long long'";
+    case 'f': return (is_complex ? "'complex float'" : "'float'");
+    case 'd': return (is_complex ? "'complex double'" : "'double'");
+    case 'g': return (is_complex ? "'complex long double'" : "'long double'");
+    case 'T': return "a struct";
+    case 'O': return "Python object";
+    case 'P': return "a pointer";
+    case 's': case 'p': return "a string";
+    case 0: return "end";
+    default: return "unparseable format string";
+  }
+}
+static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return 2;
+    case 'i': case 'I': case 'l': case 'L': return 4;
+    case 'q': case 'Q': return 8;
+    case 'f': return (is_complex ? 8 : 4);
+    case 'd': return (is_complex ? 16 : 8);
+    case 'g': {
+      PyErr_SetString(PyExc_ValueError, "Python does not define a standard format string size for long double ('g')..");
+      return 0;
+    }
+    case 'O': case 'P': return sizeof(void*);
+    default:
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+}
+static size_t __Pyx_BufFmt_TypeCharToNativeSize(char ch, int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return sizeof(short);
+    case 'i': case 'I': return sizeof(int);
+    case 'l': case 'L': return sizeof(long);
+    #ifdef HAVE_LONG_LONG
+    case 'q': case 'Q': return sizeof(PY_LONG_LONG);
+    #endif
+    case 'f': return sizeof(float) * (is_complex ? 2 : 1);
+    case 'd': return sizeof(double) * (is_complex ? 2 : 1);
+    case 'g': return sizeof(long double) * (is_complex ? 2 : 1);
+    case 'O': case 'P': return sizeof(void*);
+    default: {
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+  }
+}
+typedef struct { char c; short x; } __Pyx_st_short;
+typedef struct { char c; int x; } __Pyx_st_int;
+typedef struct { char c; long x; } __Pyx_st_long;
+typedef struct { char c; float x; } __Pyx_st_float;
+typedef struct { char c; double x; } __Pyx_st_double;
+typedef struct { char c; long double x; } __Pyx_st_longdouble;
+typedef struct { char c; void *x; } __Pyx_st_void_p;
+#ifdef HAVE_LONG_LONG
+typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
+#endif
+static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
+    case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
+    case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
+#ifdef HAVE_LONG_LONG
+    case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
+#endif
+    case 'f': return sizeof(__Pyx_st_float) - sizeof(float);
+    case 'd': return sizeof(__Pyx_st_double) - sizeof(double);
+    case 'g': return sizeof(__Pyx_st_longdouble) - sizeof(long double);
+    case 'P': case 'O': return sizeof(__Pyx_st_void_p) - sizeof(void*);
+    default:
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+}
+/* These are for computing the padding at the end of the struct to align
+   on the first member of the struct. This will probably the same as above,
+   but we don't have any guarantees.
+ */
+typedef struct { short x; char c; } __Pyx_pad_short;
+typedef struct { int x; char c; } __Pyx_pad_int;
+typedef struct { long x; char c; } __Pyx_pad_long;
+typedef struct { float x; char c; } __Pyx_pad_float;
+typedef struct { double x; char c; } __Pyx_pad_double;
+typedef struct { long double x; char c; } __Pyx_pad_longdouble;
+typedef struct { void *x; char c; } __Pyx_pad_void_p;
+#ifdef HAVE_LONG_LONG
+typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
+#endif
+static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
+    case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
+    case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
+#ifdef HAVE_LONG_LONG
+    case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
+#endif
+    case 'f': return sizeof(__Pyx_pad_float) - sizeof(float);
+    case 'd': return sizeof(__Pyx_pad_double) - sizeof(double);
+    case 'g': return sizeof(__Pyx_pad_longdouble) - sizeof(long double);
+    case 'P': case 'O': return sizeof(__Pyx_pad_void_p) - sizeof(void*);
+    default:
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+}
+static char __Pyx_BufFmt_TypeCharToGroup(char ch, int is_complex) {
+  switch (ch) {
+    case 'c':
+        return 'H';
+    case 'b': case 'h': case 'i':
+    case 'l': case 'q': case 's': case 'p':
+        return 'I';
+    case '?': case 'B': case 'H': case 'I': case 'L': case 'Q':
+        return 'U';
+    case 'f': case 'd': case 'g':
+        return (is_complex ? 'C' : 'R');
+    case 'O':
+        return 'O';
+    case 'P':
+        return 'P';
+    default: {
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+  }
+}
+static void __Pyx_BufFmt_RaiseExpected(__Pyx_BufFmt_Context* ctx) {
+  if (ctx->head == NULL || ctx->head->field == &ctx->root) {
+    const char* expected;
+    const char* quote;
+    if (ctx->head == NULL) {
+      expected = "end";
+      quote = "";
+    } else {
+      expected = ctx->head->field->type->name;
+      quote = "'";
+    }
+    PyErr_Format(PyExc_ValueError,
+                 "Buffer dtype mismatch, expected %s%s%s but got %s",
+                 quote, expected, quote,
+                 __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex));
+  } else {
+    __Pyx_StructField* field = ctx->head->field;
+    __Pyx_StructField* parent = (ctx->head - 1)->field;
+    PyErr_Format(PyExc_ValueError,
+                 "Buffer dtype mismatch, expected '%s' but got %s in '%s.%s'",
+                 field->type->name, __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex),
+                 parent->type->name, field->name);
+  }
+}
+static int __Pyx_BufFmt_ProcessTypeChunk(__Pyx_BufFmt_Context* ctx) {
+  char group;
+  size_t size, offset, arraysize = 1;
+  if (ctx->enc_type == 0) return 0;
+  if (ctx->head->field->type->arraysize[0]) {
+    int i, ndim = 0;
+    if (ctx->enc_type == 's' || ctx->enc_type == 'p') {
+        ctx->is_valid_array = ctx->head->field->type->ndim == 1;
+        ndim = 1;
+        if (ctx->enc_count != ctx->head->field->type->arraysize[0]) {
+            PyErr_Format(PyExc_ValueError,
+                         "Expected a dimension of size %zu, got %zu",
+                         ctx->head->field->type->arraysize[0], ctx->enc_count);
+            return -1;
+        }
+    }
+    if (!ctx->is_valid_array) {
+      PyErr_Format(PyExc_ValueError, "Expected %d dimensions, got %d",
+                   ctx->head->field->type->ndim, ndim);
+      return -1;
+    }
+    for (i = 0; i < ctx->head->field->type->ndim; i++) {
+      arraysize *= ctx->head->field->type->arraysize[i];
+    }
+    ctx->is_valid_array = 0;
+    ctx->enc_count = 1;
+  }
+  group = __Pyx_BufFmt_TypeCharToGroup(ctx->enc_type, ctx->is_complex);
+  do {
+    __Pyx_StructField* field = ctx->head->field;
+    __Pyx_TypeInfo* type = field->type;
+    if (ctx->enc_packmode == '@' || ctx->enc_packmode == '^') {
+      size = __Pyx_BufFmt_TypeCharToNativeSize(ctx->enc_type, ctx->is_complex);
+    } else {
+      size = __Pyx_BufFmt_TypeCharToStandardSize(ctx->enc_type, ctx->is_complex);
+    }
+    if (ctx->enc_packmode == '@') {
+      size_t align_at = __Pyx_BufFmt_TypeCharToAlignment(ctx->enc_type, ctx->is_complex);
+      size_t align_mod_offset;
+      if (align_at == 0) return -1;
+      align_mod_offset = ctx->fmt_offset % align_at;
+      if (align_mod_offset > 0) ctx->fmt_offset += align_at - align_mod_offset;
+      if (ctx->struct_alignment == 0)
+          ctx->struct_alignment = __Pyx_BufFmt_TypeCharToPadding(ctx->enc_type,
+                                                                 ctx->is_complex);
+    }
+    if (type->size != size || type->typegroup != group) {
+      if (type->typegroup == 'C' && type->fields != NULL) {
+        size_t parent_offset = ctx->head->parent_offset + field->offset;
+        ++ctx->head;
+        ctx->head->field = type->fields;
+        ctx->head->parent_offset = parent_offset;
+        continue;
+      }
+      if ((type->typegroup == 'H' || group == 'H') && type->size == size) {
+      } else {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return -1;
+      }
+    }
+    offset = ctx->head->parent_offset + field->offset;
+    if (ctx->fmt_offset != offset) {
+      PyErr_Format(PyExc_ValueError,
+                   "Buffer dtype mismatch; next field is at offset %" CYTHON_FORMAT_SSIZE_T "d but %" CYTHON_FORMAT_SSIZE_T "d expected",
+                   (Py_ssize_t)ctx->fmt_offset, (Py_ssize_t)offset);
+      return -1;
+    }
+    ctx->fmt_offset += size;
+    if (arraysize)
+      ctx->fmt_offset += (arraysize - 1) * size;
+    --ctx->enc_count;
+    while (1) {
+      if (field == &ctx->root) {
+        ctx->head = NULL;
+        if (ctx->enc_count != 0) {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return -1;
+        }
+        break;
+      }
+      ctx->head->field = ++field;
+      if (field->type == NULL) {
+        --ctx->head;
+        field = ctx->head->field;
+        continue;
+      } else if (field->type->typegroup == 'S') {
+        size_t parent_offset = ctx->head->parent_offset + field->offset;
+        if (field->type->fields->type == NULL) continue;
+        field = field->type->fields;
+        ++ctx->head;
+        ctx->head->field = field;
+        ctx->head->parent_offset = parent_offset;
+        break;
+      } else {
+        break;
+      }
+    }
+  } while (ctx->enc_count);
+  ctx->enc_type = 0;
+  ctx->is_complex = 0;
+  return 0;
+}
+static PyObject *
+__pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
+{
+    const char *ts = *tsp;
+    int i = 0, number, ndim;
+    ++ts;
+    if (ctx->new_count != 1) {
+        PyErr_SetString(PyExc_ValueError,
+                        "Cannot handle repeated arrays in format string");
+        return NULL;
+    }
+    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+    ndim = ctx->head->field->type->ndim;
+    while (*ts && *ts != ')') {
+        switch (*ts) {
+            case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
+            default:  break;
+        }
+        number = __Pyx_BufFmt_ExpectNumber(&ts);
+        if (number == -1) return NULL;
+        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i])
+            return PyErr_Format(PyExc_ValueError,
+                        "Expected a dimension of size %zu, got %d",
+                        ctx->head->field->type->arraysize[i], number);
+        if (*ts != ',' && *ts != ')')
+            return PyErr_Format(PyExc_ValueError,
+                                "Expected a comma in format string, got '%c'", *ts);
+        if (*ts == ',') ts++;
+        i++;
+    }
+    if (i != ndim)
+        return PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
+                            ctx->head->field->type->ndim, i);
+    if (!*ts) {
+        PyErr_SetString(PyExc_ValueError,
+                        "Unexpected end of format string, expected ')'");
+        return NULL;
+    }
+    ctx->is_valid_array = 1;
+    ctx->new_count = 1;
+    *tsp = ++ts;
+    return Py_None;
+}
+static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts) {
+  int got_Z = 0;
+  while (1) {
+    switch(*ts) {
+      case 0:
+        if (ctx->enc_type != 0 && ctx->head == NULL) {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return NULL;
+        }
+        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+        if (ctx->head != NULL) {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return NULL;
+        }
+        return ts;
+      case ' ':
+      case '\r':
+      case '\n':
+        ++ts;
+        break;
+      case '<':
+        if (!__Pyx_Is_Little_Endian()) {
+          PyErr_SetString(PyExc_ValueError, "Little-endian buffer not supported on big-endian compiler");
+          return NULL;
+        }
+        ctx->new_packmode = '=';
+        ++ts;
+        break;
+      case '>':
+      case '!':
+        if (__Pyx_Is_Little_Endian()) {
+          PyErr_SetString(PyExc_ValueError, "Big-endian buffer not supported on little-endian compiler");
+          return NULL;
+        }
+        ctx->new_packmode = '=';
+        ++ts;
+        break;
+      case '=':
+      case '@':
+      case '^':
+        ctx->new_packmode = *ts++;
+        break;
+      case 'T':
+        {
+          const char* ts_after_sub;
+          size_t i, struct_count = ctx->new_count;
+          size_t struct_alignment = ctx->struct_alignment;
+          ctx->new_count = 1;
+          ++ts;
+          if (*ts != '{') {
+            PyErr_SetString(PyExc_ValueError, "Buffer acquisition: Expected '{' after 'T'");
+            return NULL;
+          }
+          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+          ctx->enc_type = 0;
+          ctx->enc_count = 0;
+          ctx->struct_alignment = 0;
+          ++ts;
+          ts_after_sub = ts;
+          for (i = 0; i != struct_count; ++i) {
+            ts_after_sub = __Pyx_BufFmt_CheckString(ctx, ts);
+            if (!ts_after_sub) return NULL;
+          }
+          ts = ts_after_sub;
+          if (struct_alignment) ctx->struct_alignment = struct_alignment;
+        }
+        break;
+      case '}':
+        {
+          size_t alignment = ctx->struct_alignment;
+          ++ts;
+          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+          ctx->enc_type = 0;
+          if (alignment && ctx->fmt_offset % alignment) {
+            ctx->fmt_offset += alignment - (ctx->fmt_offset % alignment);
+          }
+        }
+        return ts;
+      case 'x':
+        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+        ctx->fmt_offset += ctx->new_count;
+        ctx->new_count = 1;
+        ctx->enc_count = 0;
+        ctx->enc_type = 0;
+        ctx->enc_packmode = ctx->new_packmode;
+        ++ts;
+        break;
+      case 'Z':
+        got_Z = 1;
+        ++ts;
+        if (*ts != 'f' && *ts != 'd' && *ts != 'g') {
+          __Pyx_BufFmt_RaiseUnexpectedChar('Z');
+          return NULL;
+        }
+        CYTHON_FALLTHROUGH;
+      case '?': case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
+      case 'l': case 'L': case 'q': case 'Q':
+      case 'f': case 'd': case 'g':
+      case 'O': case 'p':
+        if ((ctx->enc_type == *ts) && (got_Z == ctx->is_complex) &&
+            (ctx->enc_packmode == ctx->new_packmode) && (!ctx->is_valid_array)) {
+          ctx->enc_count += ctx->new_count;
+          ctx->new_count = 1;
+          got_Z = 0;
+          ++ts;
+          break;
+        }
+        CYTHON_FALLTHROUGH;
+      case 's':
+        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+        ctx->enc_count = ctx->new_count;
+        ctx->enc_packmode = ctx->new_packmode;
+        ctx->enc_type = *ts;
+        ctx->is_complex = got_Z;
+        ++ts;
+        ctx->new_count = 1;
+        got_Z = 0;
+        break;
+      case ':':
+        ++ts;
+        while(*ts != ':') ++ts;
+        ++ts;
+        break;
+      case '(':
+        if (!__pyx_buffmt_parse_array(ctx, &ts)) return NULL;
+        break;
+      default:
+        {
+          int number = __Pyx_BufFmt_ExpectNumber(&ts);
+          if (number == -1) return NULL;
+          ctx->new_count = (size_t)number;
+        }
+    }
+  }
+}
+
+/* TypeInfoCompare */
+  static int
+__pyx_typeinfo_cmp(__Pyx_TypeInfo *a, __Pyx_TypeInfo *b)
+{
+    int i;
+    if (!a || !b)
+        return 0;
+    if (a == b)
+        return 1;
+    if (a->size != b->size || a->typegroup != b->typegroup ||
+            a->is_unsigned != b->is_unsigned || a->ndim != b->ndim) {
+        if (a->typegroup == 'H' || b->typegroup == 'H') {
+            return a->size == b->size;
+        } else {
+            return 0;
+        }
+    }
+    if (a->ndim) {
+        for (i = 0; i < a->ndim; i++)
+            if (a->arraysize[i] != b->arraysize[i])
+                return 0;
+    }
+    if (a->typegroup == 'S') {
+        if (a->flags != b->flags)
+            return 0;
+        if (a->fields || b->fields) {
+            if (!(a->fields && b->fields))
+                return 0;
+            for (i = 0; a->fields[i].type && b->fields[i].type; i++) {
+                __Pyx_StructField *field_a = a->fields + i;
+                __Pyx_StructField *field_b = b->fields + i;
+                if (field_a->offset != field_b->offset ||
+                    !__pyx_typeinfo_cmp(field_a->type, field_b->type))
+                    return 0;
+            }
+            return !a->fields[i].type && !b->fields[i].type;
+        }
+    }
+    return 1;
+}
+
+/* MemviewSliceValidateAndInit */
+  static int
+__pyx_check_strides(Py_buffer *buf, int dim, int ndim, int spec)
+{
+    if (buf->shape[dim] <= 1)
+        return 1;
+    if (buf->strides) {
+        if (spec & __Pyx_MEMVIEW_CONTIG) {
+            if (spec & (__Pyx_MEMVIEW_PTR|__Pyx_MEMVIEW_FULL)) {
+                if (unlikely(buf->strides[dim] != sizeof(void *))) {
+                    PyErr_Format(PyExc_ValueError,
+                                 "Buffer is not indirectly contiguous "
+                                 "in dimension %d.", dim);
+                    goto fail;
+                }
+            } else if (unlikely(buf->strides[dim] != buf->itemsize)) {
+                PyErr_SetString(PyExc_ValueError,
+                                "Buffer and memoryview are not contiguous "
+                                "in the same dimension.");
+                goto fail;
+            }
+        }
+        if (spec & __Pyx_MEMVIEW_FOLLOW) {
+            Py_ssize_t stride = buf->strides[dim];
+            if (stride < 0)
+                stride = -stride;
+            if (unlikely(stride < buf->itemsize)) {
+                PyErr_SetString(PyExc_ValueError,
+                                "Buffer and memoryview are not contiguous "
+                                "in the same dimension.");
+                goto fail;
+            }
+        }
+    } else {
+        if (unlikely(spec & __Pyx_MEMVIEW_CONTIG && dim != ndim - 1)) {
+            PyErr_Format(PyExc_ValueError,
+                         "C-contiguous buffer is not contiguous in "
+                         "dimension %d", dim);
+            goto fail;
+        } else if (unlikely(spec & (__Pyx_MEMVIEW_PTR))) {
+            PyErr_Format(PyExc_ValueError,
+                         "C-contiguous buffer is not indirect in "
+                         "dimension %d", dim);
+            goto fail;
+        } else if (unlikely(buf->suboffsets)) {
+            PyErr_SetString(PyExc_ValueError,
+                            "Buffer exposes suboffsets but no strides");
+            goto fail;
+        }
+    }
+    return 1;
+fail:
+    return 0;
+}
+static int
+__pyx_check_suboffsets(Py_buffer *buf, int dim, CYTHON_UNUSED int ndim, int spec)
+{
+    if (spec & __Pyx_MEMVIEW_DIRECT) {
+        if (unlikely(buf->suboffsets && buf->suboffsets[dim] >= 0)) {
+            PyErr_Format(PyExc_ValueError,
+                         "Buffer not compatible with direct access "
+                         "in dimension %d.", dim);
+            goto fail;
+        }
+    }
+    if (spec & __Pyx_MEMVIEW_PTR) {
+        if (unlikely(!buf->suboffsets || (buf->suboffsets[dim] < 0))) {
+            PyErr_Format(PyExc_ValueError,
+                         "Buffer is not indirectly accessible "
+                         "in dimension %d.", dim);
+            goto fail;
+        }
+    }
+    return 1;
+fail:
+    return 0;
+}
+static int
+__pyx_verify_contig(Py_buffer *buf, int ndim, int c_or_f_flag)
+{
+    int i;
+    if (c_or_f_flag & __Pyx_IS_F_CONTIG) {
+        Py_ssize_t stride = 1;
+        for (i = 0; i < ndim; i++) {
+            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
+                PyErr_SetString(PyExc_ValueError,
+                    "Buffer not fortran contiguous.");
+                goto fail;
+            }
+            stride = stride * buf->shape[i];
+        }
+    } else if (c_or_f_flag & __Pyx_IS_C_CONTIG) {
+        Py_ssize_t stride = 1;
+        for (i = ndim - 1; i >- 1; i--) {
+            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
+                PyErr_SetString(PyExc_ValueError,
+                    "Buffer not C contiguous.");
+                goto fail;
+            }
+            stride = stride * buf->shape[i];
+        }
+    }
+    return 1;
+fail:
+    return 0;
+}
+static int __Pyx_ValidateAndInit_memviewslice(
+                int *axes_specs,
+                int c_or_f_flag,
+                int buf_flags,
+                int ndim,
+                __Pyx_TypeInfo *dtype,
+                __Pyx_BufFmt_StackElem stack[],
+                __Pyx_memviewslice *memviewslice,
+                PyObject *original_obj)
+{
+    struct __pyx_memoryview_obj *memview, *new_memview;
+    __Pyx_RefNannyDeclarations
+    Py_buffer *buf;
+    int i, spec = 0, retval = -1;
+    __Pyx_BufFmt_Context ctx;
+    int from_memoryview = __pyx_memoryview_check(original_obj);
+    __Pyx_RefNannySetupContext("ValidateAndInit_memviewslice", 0);
+    if (from_memoryview && __pyx_typeinfo_cmp(dtype, ((struct __pyx_memoryview_obj *)
+                                                            original_obj)->typeinfo)) {
+        memview = (struct __pyx_memoryview_obj *) original_obj;
+        new_memview = NULL;
+    } else {
+        memview = (struct __pyx_memoryview_obj *) __pyx_memoryview_new(
+                                            original_obj, buf_flags, 0, dtype);
+        new_memview = memview;
+        if (unlikely(!memview))
+            goto fail;
+    }
+    buf = &memview->view;
+    if (unlikely(buf->ndim != ndim)) {
+        PyErr_Format(PyExc_ValueError,
+                "Buffer has wrong number of dimensions (expected %d, got %d)",
+                ndim, buf->ndim);
+        goto fail;
+    }
+    if (new_memview) {
+        __Pyx_BufFmt_Init(&ctx, stack, dtype);
+        if (unlikely(!__Pyx_BufFmt_CheckString(&ctx, buf->format))) goto fail;
+    }
+    if (unlikely((unsigned) buf->itemsize != dtype->size)) {
+        PyErr_Format(PyExc_ValueError,
+                     "Item size of buffer (%" CYTHON_FORMAT_SSIZE_T "u byte%s) "
+                     "does not match size of '%s' (%" CYTHON_FORMAT_SSIZE_T "u byte%s)",
+                     buf->itemsize,
+                     (buf->itemsize > 1) ? "s" : "",
+                     dtype->name,
+                     dtype->size,
+                     (dtype->size > 1) ? "s" : "");
+        goto fail;
+    }
+    if (buf->len > 0) {
+        for (i = 0; i < ndim; i++) {
+            spec = axes_specs[i];
+            if (unlikely(!__pyx_check_strides(buf, i, ndim, spec)))
+                goto fail;
+            if (unlikely(!__pyx_check_suboffsets(buf, i, ndim, spec)))
+                goto fail;
+        }
+        if (unlikely(buf->strides && !__pyx_verify_contig(buf, ndim, c_or_f_flag)))
+            goto fail;
+    }
+    if (unlikely(__Pyx_init_memviewslice(memview, ndim, memviewslice,
+                                         new_memview != NULL) == -1)) {
+        goto fail;
+    }
+    retval = 0;
+    goto no_fail;
+fail:
+    Py_XDECREF(new_memview);
+    retval = -1;
+no_fail:
+    __Pyx_RefNannyFinishContext();
+    return retval;
+}
+
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_int(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
+                                                 PyBUF_RECORDS_RO | writable_flag, 1,
+                                                 &__Pyx_TypeInfo_int, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_unsigned_int(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
+                                                 PyBUF_RECORDS_RO | writable_flag, 1,
+                                                 &__Pyx_TypeInfo_unsigned_int, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_char(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
+                                                 PyBUF_RECORDS_RO | writable_flag, 1,
+                                                 &__Pyx_TypeInfo_char, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
+                                                 PyBUF_RECORDS_RO | writable_flag, 3,
+                                                 &__Pyx_TypeInfo_float, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_float(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
+                                                 PyBUF_RECORDS_RO | writable_flag, 1,
+                                                 &__Pyx_TypeInfo_float, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_float(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
+                                                 PyBUF_RECORDS_RO | writable_flag, 2,
+                                                 &__Pyx_TypeInfo_float, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_char(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
+                                                 PyBUF_RECORDS_RO | writable_flag, 2,
+                                                 &__Pyx_TypeInfo_char, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
 /* MemviewDtypeToObject */
-static CYTHON_INLINE PyObject *__pyx_memview_get_char(const char *itemp) {
+  static CYTHON_INLINE PyObject *__pyx_memview_get_char(const char *itemp) {
     return (PyObject *) __Pyx_PyInt_From_char(*(char *) itemp);
 }
 static CYTHON_INLINE int __pyx_memview_set_char(const char *itemp, PyObject *obj) {
     char value = __Pyx_PyInt_As_char(obj);
     if ((value == (char)-1) && PyErr_Occurred())
         return 0;
     *(char *) itemp = value;
     return 1;
 }
 
 /* MemviewDtypeToObject */
-static CYTHON_INLINE PyObject *__pyx_memview_get_float(const char *itemp) {
+  static CYTHON_INLINE PyObject *__pyx_memview_get_float(const char *itemp) {
     return (PyObject *) PyFloat_FromDouble(*(float *) itemp);
 }
 static CYTHON_INLINE int __pyx_memview_set_float(const char *itemp, PyObject *obj) {
     float value = __pyx_PyFloat_AsFloat(obj);
     if ((value == (float)-1) && PyErr_Occurred())
         return 0;
     *(float *) itemp = value;
     return 1;
 }
 
 /* MemviewDtypeToObject */
-static CYTHON_INLINE PyObject *__pyx_memview_get_int(const char *itemp) {
+  static CYTHON_INLINE PyObject *__pyx_memview_get_int(const char *itemp) {
     return (PyObject *) __Pyx_PyInt_From_int(*(int *) itemp);
 }
 static CYTHON_INLINE int __pyx_memview_set_int(const char *itemp, PyObject *obj) {
     int value = __Pyx_PyInt_As_int(obj);
     if ((value == (int)-1) && PyErr_Occurred())
         return 0;
     *(int *) itemp = value;
     return 1;
 }
 
 /* MemviewDtypeToObject */
-static CYTHON_INLINE PyObject *__pyx_memview_get_unsigned_int(const char *itemp) {
+  static CYTHON_INLINE PyObject *__pyx_memview_get_unsigned_int(const char *itemp) {
     return (PyObject *) __Pyx_PyInt_From_unsigned_int(*(unsigned int *) itemp);
 }
 static CYTHON_INLINE int __pyx_memview_set_unsigned_int(const char *itemp, PyObject *obj) {
     unsigned int value = __Pyx_PyInt_As_unsigned_int(obj);
     if ((value == (unsigned int)-1) && PyErr_Occurred())
         return 0;
     *(unsigned int *) itemp = value;
     return 1;
 }
 
 /* MemviewSliceCopyTemplate */
-static __Pyx_memviewslice
+  static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object)
 {
     __Pyx_RefNannyDeclarations
     int i;
@@ -29941,15 +30845,15 @@
     __Pyx_XDECREF(temp_int);
     __Pyx_XDECREF(array_obj);
     __Pyx_RefNannyFinishContext();
     return new_mvs;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -30137,15 +31041,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -30175,15 +31079,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const char neg_one = (char) -1, const_zero = (char) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -30213,15 +31117,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(char),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
+  static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const char neg_one = (char) -1, const_zero = (char) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -30409,15 +31313,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to char");
     return (char) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -30447,15 +31351,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(unsigned int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *x) {
+  static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -30643,15 +31547,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to unsigned int");
     return (unsigned int) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_short(short value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_short(short value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const short neg_one = (short) -1, const_zero = (short) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -30681,15 +31585,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(short),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -30877,15 +31781,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
+  static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -31073,15 +31977,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to size_t");
     return (size_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -31110,910 +32014,14 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
-/* IsLittleEndian */
-static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
-{
-  union {
-    uint32_t u32;
-    uint8_t u8[4];
-  } S;
-  S.u32 = 0x01020304;
-  return S.u8[0] == 4;
-}
-
-/* BufferFormatCheck */
-static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
-                              __Pyx_BufFmt_StackElem* stack,
-                              __Pyx_TypeInfo* type) {
-  stack[0].field = &ctx->root;
-  stack[0].parent_offset = 0;
-  ctx->root.type = type;
-  ctx->root.name = "buffer dtype";
-  ctx->root.offset = 0;
-  ctx->head = stack;
-  ctx->head->field = &ctx->root;
-  ctx->fmt_offset = 0;
-  ctx->head->parent_offset = 0;
-  ctx->new_packmode = '@';
-  ctx->enc_packmode = '@';
-  ctx->new_count = 1;
-  ctx->enc_count = 0;
-  ctx->enc_type = 0;
-  ctx->is_complex = 0;
-  ctx->is_valid_array = 0;
-  ctx->struct_alignment = 0;
-  while (type->typegroup == 'S') {
-    ++ctx->head;
-    ctx->head->field = type->fields;
-    ctx->head->parent_offset = 0;
-    type = type->fields->type;
-  }
-}
-static int __Pyx_BufFmt_ParseNumber(const char** ts) {
-    int count;
-    const char* t = *ts;
-    if (*t < '0' || *t > '9') {
-      return -1;
-    } else {
-        count = *t++ - '0';
-        while (*t >= '0' && *t <= '9') {
-            count *= 10;
-            count += *t++ - '0';
-        }
-    }
-    *ts = t;
-    return count;
-}
-static int __Pyx_BufFmt_ExpectNumber(const char **ts) {
-    int number = __Pyx_BufFmt_ParseNumber(ts);
-    if (number == -1)
-        PyErr_Format(PyExc_ValueError,\
-                     "Does not understand character buffer dtype format string ('%c')", **ts);
-    return number;
-}
-static void __Pyx_BufFmt_RaiseUnexpectedChar(char ch) {
-  PyErr_Format(PyExc_ValueError,
-               "Unexpected format string character: '%c'", ch);
-}
-static const char* __Pyx_BufFmt_DescribeTypeChar(char ch, int is_complex) {
-  switch (ch) {
-    case '?': return "'bool'";
-    case 'c': return "'char'";
-    case 'b': return "'signed char'";
-    case 'B': return "'unsigned char'";
-    case 'h': return "'short'";
-    case 'H': return "'unsigned short'";
-    case 'i': return "'int'";
-    case 'I': return "'unsigned int'";
-    case 'l': return "'long'";
-    case 'L': return "'unsigned long'";
-    case 'q': return "'long long'";
-    case 'Q': return "'unsigned long long'";
-    case 'f': return (is_complex ? "'complex float'" : "'float'");
-    case 'd': return (is_complex ? "'complex double'" : "'double'");
-    case 'g': return (is_complex ? "'complex long double'" : "'long double'");
-    case 'T': return "a struct";
-    case 'O': return "Python object";
-    case 'P': return "a pointer";
-    case 's': case 'p': return "a string";
-    case 0: return "end";
-    default: return "unparseable format string";
-  }
-}
-static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return 2;
-    case 'i': case 'I': case 'l': case 'L': return 4;
-    case 'q': case 'Q': return 8;
-    case 'f': return (is_complex ? 8 : 4);
-    case 'd': return (is_complex ? 16 : 8);
-    case 'g': {
-      PyErr_SetString(PyExc_ValueError, "Python does not define a standard format string size for long double ('g')..");
-      return 0;
-    }
-    case 'O': case 'P': return sizeof(void*);
-    default:
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-}
-static size_t __Pyx_BufFmt_TypeCharToNativeSize(char ch, int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return sizeof(short);
-    case 'i': case 'I': return sizeof(int);
-    case 'l': case 'L': return sizeof(long);
-    #ifdef HAVE_LONG_LONG
-    case 'q': case 'Q': return sizeof(PY_LONG_LONG);
-    #endif
-    case 'f': return sizeof(float) * (is_complex ? 2 : 1);
-    case 'd': return sizeof(double) * (is_complex ? 2 : 1);
-    case 'g': return sizeof(long double) * (is_complex ? 2 : 1);
-    case 'O': case 'P': return sizeof(void*);
-    default: {
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-  }
-}
-typedef struct { char c; short x; } __Pyx_st_short;
-typedef struct { char c; int x; } __Pyx_st_int;
-typedef struct { char c; long x; } __Pyx_st_long;
-typedef struct { char c; float x; } __Pyx_st_float;
-typedef struct { char c; double x; } __Pyx_st_double;
-typedef struct { char c; long double x; } __Pyx_st_longdouble;
-typedef struct { char c; void *x; } __Pyx_st_void_p;
-#ifdef HAVE_LONG_LONG
-typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
-#endif
-static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
-    case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
-    case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
-#ifdef HAVE_LONG_LONG
-    case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
-#endif
-    case 'f': return sizeof(__Pyx_st_float) - sizeof(float);
-    case 'd': return sizeof(__Pyx_st_double) - sizeof(double);
-    case 'g': return sizeof(__Pyx_st_longdouble) - sizeof(long double);
-    case 'P': case 'O': return sizeof(__Pyx_st_void_p) - sizeof(void*);
-    default:
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-}
-/* These are for computing the padding at the end of the struct to align
-   on the first member of the struct. This will probably the same as above,
-   but we don't have any guarantees.
- */
-typedef struct { short x; char c; } __Pyx_pad_short;
-typedef struct { int x; char c; } __Pyx_pad_int;
-typedef struct { long x; char c; } __Pyx_pad_long;
-typedef struct { float x; char c; } __Pyx_pad_float;
-typedef struct { double x; char c; } __Pyx_pad_double;
-typedef struct { long double x; char c; } __Pyx_pad_longdouble;
-typedef struct { void *x; char c; } __Pyx_pad_void_p;
-#ifdef HAVE_LONG_LONG
-typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
-#endif
-static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
-    case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
-    case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
-#ifdef HAVE_LONG_LONG
-    case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
-#endif
-    case 'f': return sizeof(__Pyx_pad_float) - sizeof(float);
-    case 'd': return sizeof(__Pyx_pad_double) - sizeof(double);
-    case 'g': return sizeof(__Pyx_pad_longdouble) - sizeof(long double);
-    case 'P': case 'O': return sizeof(__Pyx_pad_void_p) - sizeof(void*);
-    default:
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-}
-static char __Pyx_BufFmt_TypeCharToGroup(char ch, int is_complex) {
-  switch (ch) {
-    case 'c':
-        return 'H';
-    case 'b': case 'h': case 'i':
-    case 'l': case 'q': case 's': case 'p':
-        return 'I';
-    case '?': case 'B': case 'H': case 'I': case 'L': case 'Q':
-        return 'U';
-    case 'f': case 'd': case 'g':
-        return (is_complex ? 'C' : 'R');
-    case 'O':
-        return 'O';
-    case 'P':
-        return 'P';
-    default: {
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-  }
-}
-static void __Pyx_BufFmt_RaiseExpected(__Pyx_BufFmt_Context* ctx) {
-  if (ctx->head == NULL || ctx->head->field == &ctx->root) {
-    const char* expected;
-    const char* quote;
-    if (ctx->head == NULL) {
-      expected = "end";
-      quote = "";
-    } else {
-      expected = ctx->head->field->type->name;
-      quote = "'";
-    }
-    PyErr_Format(PyExc_ValueError,
-                 "Buffer dtype mismatch, expected %s%s%s but got %s",
-                 quote, expected, quote,
-                 __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex));
-  } else {
-    __Pyx_StructField* field = ctx->head->field;
-    __Pyx_StructField* parent = (ctx->head - 1)->field;
-    PyErr_Format(PyExc_ValueError,
-                 "Buffer dtype mismatch, expected '%s' but got %s in '%s.%s'",
-                 field->type->name, __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex),
-                 parent->type->name, field->name);
-  }
-}
-static int __Pyx_BufFmt_ProcessTypeChunk(__Pyx_BufFmt_Context* ctx) {
-  char group;
-  size_t size, offset, arraysize = 1;
-  if (ctx->enc_type == 0) return 0;
-  if (ctx->head->field->type->arraysize[0]) {
-    int i, ndim = 0;
-    if (ctx->enc_type == 's' || ctx->enc_type == 'p') {
-        ctx->is_valid_array = ctx->head->field->type->ndim == 1;
-        ndim = 1;
-        if (ctx->enc_count != ctx->head->field->type->arraysize[0]) {
-            PyErr_Format(PyExc_ValueError,
-                         "Expected a dimension of size %zu, got %zu",
-                         ctx->head->field->type->arraysize[0], ctx->enc_count);
-            return -1;
-        }
-    }
-    if (!ctx->is_valid_array) {
-      PyErr_Format(PyExc_ValueError, "Expected %d dimensions, got %d",
-                   ctx->head->field->type->ndim, ndim);
-      return -1;
-    }
-    for (i = 0; i < ctx->head->field->type->ndim; i++) {
-      arraysize *= ctx->head->field->type->arraysize[i];
-    }
-    ctx->is_valid_array = 0;
-    ctx->enc_count = 1;
-  }
-  group = __Pyx_BufFmt_TypeCharToGroup(ctx->enc_type, ctx->is_complex);
-  do {
-    __Pyx_StructField* field = ctx->head->field;
-    __Pyx_TypeInfo* type = field->type;
-    if (ctx->enc_packmode == '@' || ctx->enc_packmode == '^') {
-      size = __Pyx_BufFmt_TypeCharToNativeSize(ctx->enc_type, ctx->is_complex);
-    } else {
-      size = __Pyx_BufFmt_TypeCharToStandardSize(ctx->enc_type, ctx->is_complex);
-    }
-    if (ctx->enc_packmode == '@') {
-      size_t align_at = __Pyx_BufFmt_TypeCharToAlignment(ctx->enc_type, ctx->is_complex);
-      size_t align_mod_offset;
-      if (align_at == 0) return -1;
-      align_mod_offset = ctx->fmt_offset % align_at;
-      if (align_mod_offset > 0) ctx->fmt_offset += align_at - align_mod_offset;
-      if (ctx->struct_alignment == 0)
-          ctx->struct_alignment = __Pyx_BufFmt_TypeCharToPadding(ctx->enc_type,
-                                                                 ctx->is_complex);
-    }
-    if (type->size != size || type->typegroup != group) {
-      if (type->typegroup == 'C' && type->fields != NULL) {
-        size_t parent_offset = ctx->head->parent_offset + field->offset;
-        ++ctx->head;
-        ctx->head->field = type->fields;
-        ctx->head->parent_offset = parent_offset;
-        continue;
-      }
-      if ((type->typegroup == 'H' || group == 'H') && type->size == size) {
-      } else {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return -1;
-      }
-    }
-    offset = ctx->head->parent_offset + field->offset;
-    if (ctx->fmt_offset != offset) {
-      PyErr_Format(PyExc_ValueError,
-                   "Buffer dtype mismatch; next field is at offset %" CYTHON_FORMAT_SSIZE_T "d but %" CYTHON_FORMAT_SSIZE_T "d expected",
-                   (Py_ssize_t)ctx->fmt_offset, (Py_ssize_t)offset);
-      return -1;
-    }
-    ctx->fmt_offset += size;
-    if (arraysize)
-      ctx->fmt_offset += (arraysize - 1) * size;
-    --ctx->enc_count;
-    while (1) {
-      if (field == &ctx->root) {
-        ctx->head = NULL;
-        if (ctx->enc_count != 0) {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return -1;
-        }
-        break;
-      }
-      ctx->head->field = ++field;
-      if (field->type == NULL) {
-        --ctx->head;
-        field = ctx->head->field;
-        continue;
-      } else if (field->type->typegroup == 'S') {
-        size_t parent_offset = ctx->head->parent_offset + field->offset;
-        if (field->type->fields->type == NULL) continue;
-        field = field->type->fields;
-        ++ctx->head;
-        ctx->head->field = field;
-        ctx->head->parent_offset = parent_offset;
-        break;
-      } else {
-        break;
-      }
-    }
-  } while (ctx->enc_count);
-  ctx->enc_type = 0;
-  ctx->is_complex = 0;
-  return 0;
-}
-static PyObject *
-__pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
-{
-    const char *ts = *tsp;
-    int i = 0, number, ndim;
-    ++ts;
-    if (ctx->new_count != 1) {
-        PyErr_SetString(PyExc_ValueError,
-                        "Cannot handle repeated arrays in format string");
-        return NULL;
-    }
-    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-    ndim = ctx->head->field->type->ndim;
-    while (*ts && *ts != ')') {
-        switch (*ts) {
-            case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
-            default:  break;
-        }
-        number = __Pyx_BufFmt_ExpectNumber(&ts);
-        if (number == -1) return NULL;
-        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i])
-            return PyErr_Format(PyExc_ValueError,
-                        "Expected a dimension of size %zu, got %d",
-                        ctx->head->field->type->arraysize[i], number);
-        if (*ts != ',' && *ts != ')')
-            return PyErr_Format(PyExc_ValueError,
-                                "Expected a comma in format string, got '%c'", *ts);
-        if (*ts == ',') ts++;
-        i++;
-    }
-    if (i != ndim)
-        return PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
-                            ctx->head->field->type->ndim, i);
-    if (!*ts) {
-        PyErr_SetString(PyExc_ValueError,
-                        "Unexpected end of format string, expected ')'");
-        return NULL;
-    }
-    ctx->is_valid_array = 1;
-    ctx->new_count = 1;
-    *tsp = ++ts;
-    return Py_None;
-}
-static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts) {
-  int got_Z = 0;
-  while (1) {
-    switch(*ts) {
-      case 0:
-        if (ctx->enc_type != 0 && ctx->head == NULL) {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return NULL;
-        }
-        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-        if (ctx->head != NULL) {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return NULL;
-        }
-        return ts;
-      case ' ':
-      case '\r':
-      case '\n':
-        ++ts;
-        break;
-      case '<':
-        if (!__Pyx_Is_Little_Endian()) {
-          PyErr_SetString(PyExc_ValueError, "Little-endian buffer not supported on big-endian compiler");
-          return NULL;
-        }
-        ctx->new_packmode = '=';
-        ++ts;
-        break;
-      case '>':
-      case '!':
-        if (__Pyx_Is_Little_Endian()) {
-          PyErr_SetString(PyExc_ValueError, "Big-endian buffer not supported on little-endian compiler");
-          return NULL;
-        }
-        ctx->new_packmode = '=';
-        ++ts;
-        break;
-      case '=':
-      case '@':
-      case '^':
-        ctx->new_packmode = *ts++;
-        break;
-      case 'T':
-        {
-          const char* ts_after_sub;
-          size_t i, struct_count = ctx->new_count;
-          size_t struct_alignment = ctx->struct_alignment;
-          ctx->new_count = 1;
-          ++ts;
-          if (*ts != '{') {
-            PyErr_SetString(PyExc_ValueError, "Buffer acquisition: Expected '{' after 'T'");
-            return NULL;
-          }
-          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-          ctx->enc_type = 0;
-          ctx->enc_count = 0;
-          ctx->struct_alignment = 0;
-          ++ts;
-          ts_after_sub = ts;
-          for (i = 0; i != struct_count; ++i) {
-            ts_after_sub = __Pyx_BufFmt_CheckString(ctx, ts);
-            if (!ts_after_sub) return NULL;
-          }
-          ts = ts_after_sub;
-          if (struct_alignment) ctx->struct_alignment = struct_alignment;
-        }
-        break;
-      case '}':
-        {
-          size_t alignment = ctx->struct_alignment;
-          ++ts;
-          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-          ctx->enc_type = 0;
-          if (alignment && ctx->fmt_offset % alignment) {
-            ctx->fmt_offset += alignment - (ctx->fmt_offset % alignment);
-          }
-        }
-        return ts;
-      case 'x':
-        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-        ctx->fmt_offset += ctx->new_count;
-        ctx->new_count = 1;
-        ctx->enc_count = 0;
-        ctx->enc_type = 0;
-        ctx->enc_packmode = ctx->new_packmode;
-        ++ts;
-        break;
-      case 'Z':
-        got_Z = 1;
-        ++ts;
-        if (*ts != 'f' && *ts != 'd' && *ts != 'g') {
-          __Pyx_BufFmt_RaiseUnexpectedChar('Z');
-          return NULL;
-        }
-        CYTHON_FALLTHROUGH;
-      case '?': case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
-      case 'l': case 'L': case 'q': case 'Q':
-      case 'f': case 'd': case 'g':
-      case 'O': case 'p':
-        if ((ctx->enc_type == *ts) && (got_Z == ctx->is_complex) &&
-            (ctx->enc_packmode == ctx->new_packmode) && (!ctx->is_valid_array)) {
-          ctx->enc_count += ctx->new_count;
-          ctx->new_count = 1;
-          got_Z = 0;
-          ++ts;
-          break;
-        }
-        CYTHON_FALLTHROUGH;
-      case 's':
-        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-        ctx->enc_count = ctx->new_count;
-        ctx->enc_packmode = ctx->new_packmode;
-        ctx->enc_type = *ts;
-        ctx->is_complex = got_Z;
-        ++ts;
-        ctx->new_count = 1;
-        got_Z = 0;
-        break;
-      case ':':
-        ++ts;
-        while(*ts != ':') ++ts;
-        ++ts;
-        break;
-      case '(':
-        if (!__pyx_buffmt_parse_array(ctx, &ts)) return NULL;
-        break;
-      default:
-        {
-          int number = __Pyx_BufFmt_ExpectNumber(&ts);
-          if (number == -1) return NULL;
-          ctx->new_count = (size_t)number;
-        }
-    }
-  }
-}
-
-/* TypeInfoCompare */
-  static int
-__pyx_typeinfo_cmp(__Pyx_TypeInfo *a, __Pyx_TypeInfo *b)
-{
-    int i;
-    if (!a || !b)
-        return 0;
-    if (a == b)
-        return 1;
-    if (a->size != b->size || a->typegroup != b->typegroup ||
-            a->is_unsigned != b->is_unsigned || a->ndim != b->ndim) {
-        if (a->typegroup == 'H' || b->typegroup == 'H') {
-            return a->size == b->size;
-        } else {
-            return 0;
-        }
-    }
-    if (a->ndim) {
-        for (i = 0; i < a->ndim; i++)
-            if (a->arraysize[i] != b->arraysize[i])
-                return 0;
-    }
-    if (a->typegroup == 'S') {
-        if (a->flags != b->flags)
-            return 0;
-        if (a->fields || b->fields) {
-            if (!(a->fields && b->fields))
-                return 0;
-            for (i = 0; a->fields[i].type && b->fields[i].type; i++) {
-                __Pyx_StructField *field_a = a->fields + i;
-                __Pyx_StructField *field_b = b->fields + i;
-                if (field_a->offset != field_b->offset ||
-                    !__pyx_typeinfo_cmp(field_a->type, field_b->type))
-                    return 0;
-            }
-            return !a->fields[i].type && !b->fields[i].type;
-        }
-    }
-    return 1;
-}
-
-/* MemviewSliceValidateAndInit */
-  static int
-__pyx_check_strides(Py_buffer *buf, int dim, int ndim, int spec)
-{
-    if (buf->shape[dim] <= 1)
-        return 1;
-    if (buf->strides) {
-        if (spec & __Pyx_MEMVIEW_CONTIG) {
-            if (spec & (__Pyx_MEMVIEW_PTR|__Pyx_MEMVIEW_FULL)) {
-                if (unlikely(buf->strides[dim] != sizeof(void *))) {
-                    PyErr_Format(PyExc_ValueError,
-                                 "Buffer is not indirectly contiguous "
-                                 "in dimension %d.", dim);
-                    goto fail;
-                }
-            } else if (unlikely(buf->strides[dim] != buf->itemsize)) {
-                PyErr_SetString(PyExc_ValueError,
-                                "Buffer and memoryview are not contiguous "
-                                "in the same dimension.");
-                goto fail;
-            }
-        }
-        if (spec & __Pyx_MEMVIEW_FOLLOW) {
-            Py_ssize_t stride = buf->strides[dim];
-            if (stride < 0)
-                stride = -stride;
-            if (unlikely(stride < buf->itemsize)) {
-                PyErr_SetString(PyExc_ValueError,
-                                "Buffer and memoryview are not contiguous "
-                                "in the same dimension.");
-                goto fail;
-            }
-        }
-    } else {
-        if (unlikely(spec & __Pyx_MEMVIEW_CONTIG && dim != ndim - 1)) {
-            PyErr_Format(PyExc_ValueError,
-                         "C-contiguous buffer is not contiguous in "
-                         "dimension %d", dim);
-            goto fail;
-        } else if (unlikely(spec & (__Pyx_MEMVIEW_PTR))) {
-            PyErr_Format(PyExc_ValueError,
-                         "C-contiguous buffer is not indirect in "
-                         "dimension %d", dim);
-            goto fail;
-        } else if (unlikely(buf->suboffsets)) {
-            PyErr_SetString(PyExc_ValueError,
-                            "Buffer exposes suboffsets but no strides");
-            goto fail;
-        }
-    }
-    return 1;
-fail:
-    return 0;
-}
-static int
-__pyx_check_suboffsets(Py_buffer *buf, int dim, CYTHON_UNUSED int ndim, int spec)
-{
-    if (spec & __Pyx_MEMVIEW_DIRECT) {
-        if (unlikely(buf->suboffsets && buf->suboffsets[dim] >= 0)) {
-            PyErr_Format(PyExc_ValueError,
-                         "Buffer not compatible with direct access "
-                         "in dimension %d.", dim);
-            goto fail;
-        }
-    }
-    if (spec & __Pyx_MEMVIEW_PTR) {
-        if (unlikely(!buf->suboffsets || (buf->suboffsets[dim] < 0))) {
-            PyErr_Format(PyExc_ValueError,
-                         "Buffer is not indirectly accessible "
-                         "in dimension %d.", dim);
-            goto fail;
-        }
-    }
-    return 1;
-fail:
-    return 0;
-}
-static int
-__pyx_verify_contig(Py_buffer *buf, int ndim, int c_or_f_flag)
-{
-    int i;
-    if (c_or_f_flag & __Pyx_IS_F_CONTIG) {
-        Py_ssize_t stride = 1;
-        for (i = 0; i < ndim; i++) {
-            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
-                PyErr_SetString(PyExc_ValueError,
-                    "Buffer not fortran contiguous.");
-                goto fail;
-            }
-            stride = stride * buf->shape[i];
-        }
-    } else if (c_or_f_flag & __Pyx_IS_C_CONTIG) {
-        Py_ssize_t stride = 1;
-        for (i = ndim - 1; i >- 1; i--) {
-            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
-                PyErr_SetString(PyExc_ValueError,
-                    "Buffer not C contiguous.");
-                goto fail;
-            }
-            stride = stride * buf->shape[i];
-        }
-    }
-    return 1;
-fail:
-    return 0;
-}
-static int __Pyx_ValidateAndInit_memviewslice(
-                int *axes_specs,
-                int c_or_f_flag,
-                int buf_flags,
-                int ndim,
-                __Pyx_TypeInfo *dtype,
-                __Pyx_BufFmt_StackElem stack[],
-                __Pyx_memviewslice *memviewslice,
-                PyObject *original_obj)
-{
-    struct __pyx_memoryview_obj *memview, *new_memview;
-    __Pyx_RefNannyDeclarations
-    Py_buffer *buf;
-    int i, spec = 0, retval = -1;
-    __Pyx_BufFmt_Context ctx;
-    int from_memoryview = __pyx_memoryview_check(original_obj);
-    __Pyx_RefNannySetupContext("ValidateAndInit_memviewslice", 0);
-    if (from_memoryview && __pyx_typeinfo_cmp(dtype, ((struct __pyx_memoryview_obj *)
-                                                            original_obj)->typeinfo)) {
-        memview = (struct __pyx_memoryview_obj *) original_obj;
-        new_memview = NULL;
-    } else {
-        memview = (struct __pyx_memoryview_obj *) __pyx_memoryview_new(
-                                            original_obj, buf_flags, 0, dtype);
-        new_memview = memview;
-        if (unlikely(!memview))
-            goto fail;
-    }
-    buf = &memview->view;
-    if (unlikely(buf->ndim != ndim)) {
-        PyErr_Format(PyExc_ValueError,
-                "Buffer has wrong number of dimensions (expected %d, got %d)",
-                ndim, buf->ndim);
-        goto fail;
-    }
-    if (new_memview) {
-        __Pyx_BufFmt_Init(&ctx, stack, dtype);
-        if (unlikely(!__Pyx_BufFmt_CheckString(&ctx, buf->format))) goto fail;
-    }
-    if (unlikely((unsigned) buf->itemsize != dtype->size)) {
-        PyErr_Format(PyExc_ValueError,
-                     "Item size of buffer (%" CYTHON_FORMAT_SSIZE_T "u byte%s) "
-                     "does not match size of '%s' (%" CYTHON_FORMAT_SSIZE_T "u byte%s)",
-                     buf->itemsize,
-                     (buf->itemsize > 1) ? "s" : "",
-                     dtype->name,
-                     dtype->size,
-                     (dtype->size > 1) ? "s" : "");
-        goto fail;
-    }
-    if (buf->len > 0) {
-        for (i = 0; i < ndim; i++) {
-            spec = axes_specs[i];
-            if (unlikely(!__pyx_check_strides(buf, i, ndim, spec)))
-                goto fail;
-            if (unlikely(!__pyx_check_suboffsets(buf, i, ndim, spec)))
-                goto fail;
-        }
-        if (unlikely(buf->strides && !__pyx_verify_contig(buf, ndim, c_or_f_flag)))
-            goto fail;
-    }
-    if (unlikely(__Pyx_init_memviewslice(memview, ndim, memviewslice,
-                                         new_memview != NULL) == -1)) {
-        goto fail;
-    }
-    retval = 0;
-    goto no_fail;
-fail:
-    Py_XDECREF(new_memview);
-    retval = -1;
-no_fail:
-    __Pyx_RefNannyFinishContext();
-    return retval;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_int(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 1,
-                                                 &__Pyx_TypeInfo_int, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_unsigned_int(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 1,
-                                                 &__Pyx_TypeInfo_unsigned_int, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_char(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 1,
-                                                 &__Pyx_TypeInfo_char, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 3,
-                                                 &__Pyx_TypeInfo_float, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_float(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 1,
-                                                 &__Pyx_TypeInfo_float, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_float(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 2,
-                                                 &__Pyx_TypeInfo_float, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_char(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 2,
-                                                 &__Pyx_TypeInfo_char, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
     char ctversion[4], rtversion[4];
     PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
     if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
```

### Comparing `rpgPy-0.8.0/rpgpy/spcutil.py` & `rpgPy-0.9.0/rpgpy/spcutil.py`

 * *Files identical despite different names*

### Comparing `rpgPy-0.8.0/rpgpy/utils.py` & `rpgPy-0.9.0/rpgpy/utils.py`

 * *Files identical despite different names*

### Comparing `rpgPy-0.8.0/rpgpy/metadata.py` & `rpgPy-0.9.0/rpgpy/metadata.py`

 * *Files identical despite different names*

### Comparing `rpgPy-0.8.0/rpgpy/header.py` & `rpgPy-0.9.0/rpgpy/header.py`

 * *Files identical despite different names*

