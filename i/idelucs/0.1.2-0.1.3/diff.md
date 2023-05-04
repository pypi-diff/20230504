# Comparing `tmp/idelucs-0.1.2.tar.gz` & `tmp/idelucs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idelucs-0.1.2.tar", last modified: Wed May  3 22:49:13 2023, max compression
+gzip compressed data, was "idelucs-0.1.3.tar", last modified: Thu May  4 01:10:13 2023, max compression
```

## Comparing `idelucs-0.1.2.tar` & `idelucs-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 loan      (1000) loan      (1000)        0 2023-05-03 22:49:13.775825 idelucs-0.1.2/
--rw-rw-r--   0 loan      (1000) loan      (1000)      556 2023-05-03 22:49:13.775825 idelucs-0.1.2/PKG-INFO
-drwxrwxr-x   0 loan      (1000) loan      (1000)        0 2023-05-03 22:49:13.775825 idelucs-0.1.2/idelucs/
--rw-rw-r--   0 loan      (1000) loan      (1000)     3104 2022-09-27 18:27:35.000000 idelucs-0.1.2/idelucs/LossFunctions.py
--rw-r-----   0 loan      (1000) loan      (1000)     2584 2023-04-13 16:42:44.000000 idelucs-0.1.2/idelucs/PytorchUtils.py
--rw-r-----   0 loan      (1000) loan      (1000)     7524 2023-04-13 16:42:44.000000 idelucs-0.1.2/idelucs/ResNet.py
--rw-rw-r--   0 loan      (1000) loan      (1000)      355 2023-05-01 17:45:48.000000 idelucs-0.1.2/idelucs/__init__.py
--rw-r-----   0 loan      (1000) loan      (1000)    11548 2023-05-03 21:30:28.000000 idelucs-0.1.2/idelucs/__main__.py
--rw-rw-r--   0 loan      (1000) loan      (1000)   818957 2023-04-13 21:13:42.000000 idelucs-0.1.2/idelucs/kmers.c
--rw-r-----   0 loan      (1000) loan      (1000)     6731 2023-05-03 21:33:54.000000 idelucs-0.1.2/idelucs/models.py
--rw-r-----   0 loan      (1000) loan      (1000)    20627 2023-05-03 20:34:29.000000 idelucs-0.1.2/idelucs/utils.py
--rw-r-----   0 loan      (1000) loan      (1000)     2949 2023-05-03 21:28:49.000000 idelucs-0.1.2/idelucs/utils_GUI.py
-drwxrwxr-x   0 loan      (1000) loan      (1000)        0 2023-05-03 22:49:13.775825 idelucs-0.1.2/idelucs.egg-info/
--rw-rw-r--   0 loan      (1000) loan      (1000)      556 2023-05-03 22:49:13.000000 idelucs-0.1.2/idelucs.egg-info/PKG-INFO
--rw-rw-r--   0 loan      (1000) loan      (1000)      341 2023-05-03 22:49:13.000000 idelucs-0.1.2/idelucs.egg-info/SOURCES.txt
--rw-rw-r--   0 loan      (1000) loan      (1000)        1 2023-05-03 22:49:13.000000 idelucs-0.1.2/idelucs.egg-info/dependency_links.txt
--rw-rw-r--   0 loan      (1000) loan      (1000)        1 2023-05-03 22:49:13.000000 idelucs-0.1.2/idelucs.egg-info/not-zip-safe
--rw-rw-r--   0 loan      (1000) loan      (1000)        8 2023-05-03 22:49:13.000000 idelucs-0.1.2/idelucs.egg-info/top_level.txt
--rw-rw-r--   0 loan      (1000) loan      (1000)       38 2023-05-03 22:49:13.775825 idelucs-0.1.2/setup.cfg
--rw-rw-r--   0 loan      (1000) loan      (1000)     1562 2023-05-03 22:47:10.000000 idelucs-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:10:13.669082 idelucs-0.1.3/
+-rw-rw-rw-   0        0        0     1074 2023-05-04 00:59:28.000000 idelucs-0.1.3/LICENCE.md
+-rw-rw-rw-   0        0        0      608 2023-05-04 01:10:13.669082 idelucs-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-05-04 00:59:28.000000 idelucs-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 01:10:13.669082 idelucs-0.1.3/idelucs/
+-rw-rw-rw-   0        0        0     3104 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/LossFunctions.py
+-rw-rw-rw-   0        0        0     2584 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/PytorchUtils.py
+-rw-rw-rw-   0        0        0     7524 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/ResNet.py
+-rw-rw-rw-   0        0        0      355 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/__init__.py
+-rw-rw-rw-   0        0        0    11548 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/__main__.py
+-rw-rw-rw-   0        0        0   819037 2023-05-04 01:03:03.000000 idelucs-0.1.3/idelucs/kmers.c
+-rw-rw-rw-   0        0        0     6731 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/models.py
+-rw-rw-rw-   0        0        0    20627 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/utils.py
+-rw-rw-rw-   0        0        0     2949 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/utils_GUI.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:10:13.669082 idelucs-0.1.3/idelucs.egg-info/
+-rw-rw-rw-   0        0        0      608 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 01:10:13.669082 idelucs-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1529 2023-05-04 01:09:02.000000 idelucs-0.1.3/setup.py
```

### Comparing `idelucs-0.1.2/PKG-INFO` & `idelucs-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-Metadata-Version: 2.1
-Name: idelucs
-Version: 0.1.2
-Summary: My first Python package
-Author: Pablo Millan
-Author-email: <pmillana@uwaterloo.ca>
-Keywords: python,first package
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-
-My first Python package with a slightly longer description
+Metadata-Version: 2.1
+Name: idelucs
+Version: 0.1.3
+Summary: My first Python package
+Home-page: UNKNOWN
+Author: Pablo Millan
+Author-email: <pmillana@uwaterloo.ca>
+License: UNKNOWN
+Keywords: python,first package
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+License-File: LICENCE.md
+
+My first Python package with a slightly longer description
+
```

### Comparing `idelucs-0.1.2/idelucs/LossFunctions.py` & `idelucs-0.1.3/idelucs/LossFunctions.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.2/idelucs/PytorchUtils.py` & `idelucs-0.1.3/idelucs/PytorchUtils.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.2/idelucs/ResNet.py` & `idelucs-0.1.3/idelucs/ResNet.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.2/idelucs/__main__.py` & `idelucs-0.1.3/idelucs/__main__.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.2/idelucs/kmers.c` & `idelucs-0.1.3/idelucs/kmers.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "include_dirs": [
-            "/home/loan/dev_iDeLUCS/lib/python3.8/site-packages/numpy/core/include"
+            "C:\\Users\\pablo\\iDeLUCS_test\\lib\\site-packages\\numpy\\core\\include"
         ],
         "name": "idelucs.kmers",
         "sources": [
             "idelucs/kmers.pyx"
         ]
     },
     "module_name": "idelucs.kmers"
@@ -20,16 +20,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -98,15 +98,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -214,15 +214,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -253,15 +253,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -563,35 +563,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -966,15 +966,15 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "idelucs/kmers.pyx",
+  "idelucs\\kmers.pyx",
   "stringsource",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
   struct __pyx_memoryview_obj *memview;
   char *data;
@@ -1531,26 +1531,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -3925,15 +3925,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -5903,15 +5903,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -8206,15 +8206,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -8279,15 +8279,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -16482,15 +16482,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -17814,15 +17814,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -18119,15 +18119,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_idelucs__kmers) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -18862,28 +18862,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -19367,15 +19367,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -20245,15 +20245,15 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `idelucs-0.1.2/idelucs/models.py` & `idelucs-0.1.3/idelucs/models.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.2/idelucs/utils.py` & `idelucs-0.1.3/idelucs/utils.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.2/idelucs/utils_GUI.py` & `idelucs-0.1.3/idelucs/utils_GUI.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.2/idelucs.egg-info/PKG-INFO` & `idelucs-0.1.3/idelucs.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-Metadata-Version: 2.1
-Name: idelucs
-Version: 0.1.2
-Summary: My first Python package
-Author: Pablo Millan
-Author-email: <pmillana@uwaterloo.ca>
-Keywords: python,first package
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-
-My first Python package with a slightly longer description
+Metadata-Version: 2.1
+Name: idelucs
+Version: 0.1.3
+Summary: My first Python package
+Home-page: UNKNOWN
+Author: Pablo Millan
+Author-email: <pmillana@uwaterloo.ca>
+License: UNKNOWN
+Keywords: python,first package
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Unix
+License-File: LICENCE.md
+
+My first Python package with a slightly longer description
+
```

### Comparing `idelucs-0.1.2/setup.py` & `idelucs-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages, Extension
 from Cython.Build import cythonize
 
-VERSION = '0.1.2' 
+VERSION = '0.1.3' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 import numpy
 
 cython_directives = {
     'embedsignature': True,
 }
 
+
 extensions = cythonize([
     Extension(name='idelucs.kmers',
               sources=["idelucs/kmers.pyx"],
               include_dirs=[numpy.get_include()]),
 ], compiler_directives=cython_directives)
 
 
@@ -27,22 +28,22 @@
         author="Pablo Millan",
         author_email="<pmillana@uwaterloo.ca>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         zip_safe=False,            # Without these two options
         include_package_data=True, # PyInstaller may not find your C-Extensions
         packages=find_packages(),
-        install_requires=[], # add any additional packages that 
+        install_requires=["setuptools", "Cython"], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
-            "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
-            "Operating System :: Unix"
+            "Operating System :: Unix",
+
         ],
-        ext_modules=extensions
+	ext_modules=extensions
 )
```

