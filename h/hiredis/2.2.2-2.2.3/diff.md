# Comparing `tmp/hiredis-2.2.2.tar.gz` & `tmp/hiredis-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiredis-2.2.2.tar", last modified: Mon Feb 13 07:06:00 2023, max compression
+gzip compressed data, was "hiredis-2.2.3.tar", last modified: Thu May  4 10:11:11 2023, max compression
```

## Comparing `hiredis-2.2.2.tar` & `hiredis-2.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 07:06:00.501279 hiredis-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-02-13 07:05:56.000000 hiredis-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-02-13 07:05:56.000000 hiredis-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6699 2023-02-13 07:06:00.501279 hiredis-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5478 2023-02-13 07:05:56.000000 hiredis-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 07:06:00.497279 hiredis-2.2.2/hiredis/
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-02-13 07:05:56.000000 hiredis-2.2.2/hiredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      996 2023-02-13 07:05:56.000000 hiredis-2.2.2/hiredis/hiredis.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 07:05:56.000000 hiredis-2.2.2/hiredis/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-02-13 07:05:56.000000 hiredis-2.2.2/hiredis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 07:06:00.497279 hiredis-2.2.2/hiredis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6699 2023-02-13 07:06:00.000000 hiredis-2.2.2/hiredis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-02-13 07:06:00.000000 hiredis-2.2.2/hiredis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-13 07:06:00.000000 hiredis-2.2.2/hiredis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-02-13 07:06:00.000000 hiredis-2.2.2/hiredis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-13 07:06:00.501279 hiredis-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-02-13 07:05:56.000000 hiredis-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 07:06:00.497279 hiredis-2.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-02-13 07:05:56.000000 hiredis-2.2.2/src/hiredis.c
--rw-r--r--   0 runner    (1001) docker     (122)      651 2023-02-13 07:05:56.000000 hiredis-2.2.2/src/hiredis.h
--rw-r--r--   0 runner    (1001) docker     (122)     3456 2023-02-13 07:05:56.000000 hiredis-2.2.2/src/pack.c
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-02-13 07:05:56.000000 hiredis-2.2.2/src/pack.h
--rw-r--r--   0 runner    (1001) docker     (122)    15197 2023-02-13 07:05:56.000000 hiredis-2.2.2/src/reader.c
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-02-13 07:05:56.000000 hiredis-2.2.2/src/reader.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 07:06:00.497279 hiredis-2.2.2/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 07:06:00.501279 hiredis-2.2.2/vendor/hiredis/
--rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     2928 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/alloc.c
--rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/alloc.h
--rw-r--r--   0 runner    (1001) docker     (122)    33903 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/async.c
--rw-r--r--   0 runner    (1001) docker     (122)     6288 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/async.h
--rw-r--r--   0 runner    (1001) docker     (122)     3367 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/async_private.h
--rw-r--r--   0 runner    (1001) docker     (122)    10650 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/dict.c
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/dict.h
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/fmacros.h
--rw-r--r--   0 runner    (1001) docker     (122)    36760 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/hiredis.c
--rw-r--r--   0 runner    (1001) docker     (122)    13890 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/hiredis.h
--rw-r--r--   0 runner    (1001) docker     (122)     6079 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/hiredis_ssl.h
--rw-r--r--   0 runner    (1001) docker     (122)    20433 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/net.c
--rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/net.h
--rw-r--r--   0 runner    (1001) docker     (122)    23394 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/read.c
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/read.h
--rw-r--r--   0 runner    (1001) docker     (122)    40519 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/sds.c
--rw-r--r--   0 runner    (1001) docker     (122)     9238 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/sds.h
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/sdsalloc.h
--rw-r--r--   0 runner    (1001) docker     (122)     9889 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/sockcompat.c
--rw-r--r--   0 runner    (1001) docker     (122)     4409 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/sockcompat.h
--rw-r--r--   0 runner    (1001) docker     (122)    16930 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/ssl.c
--rw-r--r--   0 runner    (1001) docker     (122)    83938 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/test.c
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-02-13 07:05:57.000000 hiredis-2.2.2/vendor/hiredis/win32.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 10:11:11.304533 hiredis-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-05-04 10:11:05.000000 hiredis-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-04 10:11:05.000000 hiredis-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6699 2023-05-04 10:11:11.304533 hiredis-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5478 2023-05-04 10:11:05.000000 hiredis-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 10:11:11.296533 hiredis-2.2.3/hiredis/
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-05-04 10:11:05.000000 hiredis-2.2.3/hiredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-05-04 10:11:05.000000 hiredis-2.2.3/hiredis/hiredis.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 10:11:05.000000 hiredis-2.2.3/hiredis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-04 10:11:05.000000 hiredis-2.2.3/hiredis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 10:11:11.300533 hiredis-2.2.3/hiredis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6699 2023-05-04 10:11:11.000000 hiredis-2.2.3/hiredis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-04 10:11:11.000000 hiredis-2.2.3/hiredis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 10:11:11.000000 hiredis-2.2.3/hiredis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-04 10:11:11.000000 hiredis-2.2.3/hiredis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-04 10:11:11.304533 hiredis-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-05-04 10:11:05.000000 hiredis-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 10:11:11.300533 hiredis-2.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-05-04 10:11:05.000000 hiredis-2.2.3/src/hiredis.c
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-05-04 10:11:05.000000 hiredis-2.2.3/src/hiredis.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3456 2023-05-04 10:11:05.000000 hiredis-2.2.3/src/pack.c
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-04 10:11:05.000000 hiredis-2.2.3/src/pack.h
+-rw-r--r--   0 runner    (1001) docker     (122)    15547 2023-05-04 10:11:05.000000 hiredis-2.2.3/src/reader.c
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-04 10:11:05.000000 hiredis-2.2.3/src/reader.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 10:11:11.296533 hiredis-2.2.3/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 10:11:11.304533 hiredis-2.2.3/vendor/hiredis/
+-rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     2928 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/alloc.c
+-rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (122)    33903 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/async.c
+-rw-r--r--   0 runner    (1001) docker     (122)     6288 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/async.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3367 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/async_private.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10650 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/dict.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/dict.h
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/fmacros.h
+-rw-r--r--   0 runner    (1001) docker     (122)    36760 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/hiredis.c
+-rw-r--r--   0 runner    (1001) docker     (122)    13890 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/hiredis.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6079 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/hiredis_ssl.h
+-rw-r--r--   0 runner    (1001) docker     (122)    20433 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/net.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/net.h
+-rw-r--r--   0 runner    (1001) docker     (122)    23394 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/read.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/read.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40519 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/sds.c
+-rw-r--r--   0 runner    (1001) docker     (122)     9238 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/sds.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/sdsalloc.h
+-rw-r--r--   0 runner    (1001) docker     (122)     9889 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/sockcompat.c
+-rw-r--r--   0 runner    (1001) docker     (122)     4409 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/sockcompat.h
+-rw-r--r--   0 runner    (1001) docker     (122)    16930 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/ssl.c
+-rw-r--r--   0 runner    (1001) docker     (122)    83938 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/test.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-05-04 10:11:07.000000 hiredis-2.2.3/vendor/hiredis/win32.h
```

### Comparing `hiredis-2.2.2/LICENSE` & `hiredis-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/PKG-INFO` & `hiredis-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiredis
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python wrapper for hiredis
 Home-page: https://github.com/redis/hiredis-py
 Author: Jan-Erik Rediger, Pieter Noordhuis
 Author-email: janerik@fnordig.de, pcnoordhuis@gmail.com
 License: BSD
 Project-URL: Changes, https://github.com/redis/hiredis-py/releases
 Project-URL: Issue tracker, https://github.com/redis/hiredis-py/issues
```

### Comparing `hiredis-2.2.2/README.md` & `hiredis-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/hiredis/hiredis.pyi` & `hiredis-2.2.3/hiredis/hiredis.pyi`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/hiredis.egg-info/PKG-INFO` & `hiredis-2.2.3/hiredis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiredis
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python wrapper for hiredis
 Home-page: https://github.com/redis/hiredis-py
 Author: Jan-Erik Rediger, Pieter Noordhuis
 Author-email: janerik@fnordig.de, pcnoordhuis@gmail.com
 License: BSD
 Project-URL: Changes, https://github.com/redis/hiredis-py/releases
 Project-URL: Issue tracker, https://github.com/redis/hiredis-py/issues
```

### Comparing `hiredis-2.2.2/hiredis.egg-info/SOURCES.txt` & `hiredis-2.2.3/hiredis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/setup.py` & `hiredis-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/src/hiredis.c` & `hiredis-2.2.3/src/hiredis.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/src/hiredis.h` & `hiredis-2.2.3/src/hiredis.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/src/pack.c` & `hiredis-2.2.3/src/pack.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/src/reader.c` & `hiredis-2.2.3/src/reader.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #include "reader.h"
 
 #include <assert.h>
 
 static void Reader_dealloc(hiredis_ReaderObject *self);
+static int Reader_traverse(hiredis_ReaderObject *self, visitproc visit, void *arg);
 static int Reader_init(hiredis_ReaderObject *self, PyObject *args, PyObject *kwds);
 static PyObject *Reader_new(PyTypeObject *type, PyObject *args, PyObject *kwds);
 static PyObject *Reader_feed(hiredis_ReaderObject *self, PyObject *args);
 static PyObject *Reader_gets(hiredis_ReaderObject *self, PyObject *args);
 static PyObject *Reader_setmaxbuf(hiredis_ReaderObject *self, PyObject *arg);
 static PyObject *Reader_getmaxbuf(hiredis_ReaderObject *self);
 static PyObject *Reader_len(hiredis_ReaderObject *self);
@@ -40,17 +41,17 @@
     0,                            /*tp_as_mapping*/
     0,                            /*tp_hash */
     0,                            /*tp_call*/
     0,                            /*tp_str*/
     0,                            /*tp_getattro*/
     0,                            /*tp_setattro*/
     0,                            /*tp_as_buffer*/
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE, /*tp_flags*/
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HAVE_GC, /*tp_flags*/
     "Hiredis protocol reader",    /*tp_doc */
-    0,                            /*tp_traverse */
+    (traverseproc)Reader_traverse,/*tp_traverse */
     0,                            /*tp_clear */
     0,                            /*tp_richcompare */
     0,                            /*tp_weaklistoffset */
     0,                            /*tp_iter */
     0,                            /*tp_iternext */
     hiredis_ReaderMethods,        /*tp_methods */
     0,                            /*tp_members */
@@ -205,24 +206,32 @@
     createDoubleObject,  // void *(*createDoubleObject)(const redisReadTask*, double, char*, size_t);
     createNilObject,     // void *(*createNil)(const redisReadTask*);
     createBoolObject,    // void *(*createBoolObject)(const redisReadTask*, int);
     freeObject           // void (*freeObject)(void*);
 };
 
 static void Reader_dealloc(hiredis_ReaderObject *self) {
+    PyObject_GC_UnTrack(self);
     // we don't need to free self->encoding as the buffer is managed by Python
     // https://docs.python.org/3/c-api/arg.html#strings-and-buffers
     redisReaderFree(self->reader);
-    Py_XDECREF(self->protocolErrorClass);
-    Py_XDECREF(self->replyErrorClass);
-    Py_XDECREF(self->notEnoughDataObject);
+    Py_CLEAR(self->protocolErrorClass);
+    Py_CLEAR(self->replyErrorClass);
+    Py_CLEAR(self->notEnoughDataObject);
 
     ((PyObject *)self)->ob_type->tp_free((PyObject*)self);
 }
 
+static int Reader_traverse(hiredis_ReaderObject *self, visitproc visit, void *arg) {
+    Py_VISIT(self->protocolErrorClass);
+    Py_VISIT(self->replyErrorClass);
+    Py_VISIT(self->notEnoughDataObject);
+    return 0;
+}
+
 static int _Reader_set_exception(PyObject **target, PyObject *value) {
     int callable;
     callable = PyCallable_Check(value);
 
     if (callable == 0) {
         PyErr_SetString(PyExc_TypeError, "Expected a callable");
         return 0;
```

### Comparing `hiredis-2.2.2/src/reader.h` & `hiredis-2.2.3/src/reader.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/COPYING` & `hiredis-2.2.3/vendor/hiredis/COPYING`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/alloc.c` & `hiredis-2.2.3/vendor/hiredis/alloc.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/alloc.h` & `hiredis-2.2.3/vendor/hiredis/alloc.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/async.c` & `hiredis-2.2.3/vendor/hiredis/async.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/async.h` & `hiredis-2.2.3/vendor/hiredis/async.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/async_private.h` & `hiredis-2.2.3/vendor/hiredis/async_private.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/dict.c` & `hiredis-2.2.3/vendor/hiredis/dict.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/dict.h` & `hiredis-2.2.3/vendor/hiredis/dict.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/hiredis.c` & `hiredis-2.2.3/vendor/hiredis/hiredis.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/hiredis.h` & `hiredis-2.2.3/vendor/hiredis/hiredis.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/hiredis_ssl.h` & `hiredis-2.2.3/vendor/hiredis/hiredis_ssl.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/net.c` & `hiredis-2.2.3/vendor/hiredis/net.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/net.h` & `hiredis-2.2.3/vendor/hiredis/net.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/read.c` & `hiredis-2.2.3/vendor/hiredis/read.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/read.h` & `hiredis-2.2.3/vendor/hiredis/read.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/sds.c` & `hiredis-2.2.3/vendor/hiredis/sds.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/sds.h` & `hiredis-2.2.3/vendor/hiredis/sds.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/sdsalloc.h` & `hiredis-2.2.3/vendor/hiredis/sdsalloc.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/sockcompat.c` & `hiredis-2.2.3/vendor/hiredis/sockcompat.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/sockcompat.h` & `hiredis-2.2.3/vendor/hiredis/sockcompat.h`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/ssl.c` & `hiredis-2.2.3/vendor/hiredis/ssl.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/test.c` & `hiredis-2.2.3/vendor/hiredis/test.c`

 * *Files identical despite different names*

### Comparing `hiredis-2.2.2/vendor/hiredis/win32.h` & `hiredis-2.2.3/vendor/hiredis/win32.h`

 * *Files identical despite different names*

