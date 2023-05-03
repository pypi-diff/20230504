# Comparing `tmp/netsnmp-py-0.5.2.tar.gz` & `tmp/netsnmp-py-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netsnmp-py-0.5.2.tar", last modified: Wed Sep 26 22:00:22 2018, max compression
+gzip compressed data, was "netsnmp-py-0.6.tar", last modified: Wed May  3 22:37:57 2023, max compression
```

## Comparing `netsnmp-py-0.5.2.tar` & `netsnmp-py-0.6.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxr-x   0 xsx       (1000) xsx       (1000)        0 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/
--rwxrwxr-x   0 xsx       (1000) xsx       (1000)     2360 2018-09-26 22:00:19.000000 netsnmp-py-0.5.2/setup.py
-drwxrwxr-x   0 xsx       (1000) xsx       (1000)        0 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/netsnmp/
--rw-rw-r--   0 xsx       (1000) xsx       (1000)     1292 2016-01-23 04:55:07.000000 netsnmp-py-0.5.2/netsnmp/_api.h
--rwxrwxr-x   0 xsx       (1000) xsx       (1000)     2065 2015-12-27 06:27:57.000000 netsnmp-py-0.5.2/netsnmp/_hex.py
--rw-rw-r--   0 xsx       (1000) xsx       (1000)     7125 2017-04-28 21:39:00.000000 netsnmp-py-0.5.2/netsnmp/get_async.c
--rw-rw-r--   0 xsx       (1000) xsx       (1000)     2481 2015-12-14 23:31:09.000000 netsnmp-py-0.5.2/netsnmp/session.c
-drwxrwxr-x   0 xsx       (1000) xsx       (1000)        0 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/netsnmp/_dev/
--rwxrwxr-x   0 xsx       (1000) xsx       (1000)     1475 2015-12-28 06:11:32.000000 netsnmp-py-0.5.2/netsnmp/_dev/arris.py
--rwxrwxr-x   0 xsx       (1000) xsx       (1000)     1545 2015-12-28 06:12:11.000000 netsnmp-py-0.5.2/netsnmp/_dev/technicolor.py
--rwxrwxr-x   0 xsx       (1000) xsx       (1000)     1306 2015-12-28 06:11:50.000000 netsnmp-py-0.5.2/netsnmp/_dev/cisco.py
--rwxrwxr-x   0 xsx       (1000) xsx       (1000)     1420 2016-01-19 02:25:06.000000 netsnmp-py-0.5.2/netsnmp/_dev/__init__.py
--rw-rw-r--   0 xsx       (1000) xsx       (1000)     5383 2017-04-28 21:00:26.000000 netsnmp-py-0.5.2/netsnmp/interface.c
--rw-rw-r--   0 xsx       (1000) xsx       (1000)      148 2016-01-20 04:13:22.000000 netsnmp-py-0.5.2/netsnmp/__main__.py
--rw-rw-r--   0 xsx       (1000) xsx       (1000)     1814 2016-01-19 02:16:49.000000 netsnmp-py-0.5.2/netsnmp/_api.c
--rw-rw-r--   0 xsx       (1000) xsx       (1000)     6561 2017-04-28 21:00:26.000000 netsnmp-py-0.5.2/netsnmp/get.c
--rwxrwxr-x   0 xsx       (1000) xsx       (1000)     4703 2018-08-23 21:28:39.000000 netsnmp-py-0.5.2/netsnmp/__init__.py
--rw-rw-r--   0 xsx       (1000) xsx       (1000)       38 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/setup.cfg
--rw-rw-r--   0 xsx       (1000) xsx       (1000)      698 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/PKG-INFO
-drwxrwxr-x   0 xsx       (1000) xsx       (1000)        0 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/netsnmp_py.egg-info/
--rw-rw-r--   0 xsx       (1000) xsx       (1000)        8 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/netsnmp_py.egg-info/top_level.txt
--rw-rw-r--   0 xsx       (1000) xsx       (1000)      698 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/netsnmp_py.egg-info/PKG-INFO
--rw-rw-r--   0 xsx       (1000) xsx       (1000)        1 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/netsnmp_py.egg-info/dependency_links.txt
--rw-rw-r--   0 xsx       (1000) xsx       (1000)      399 2018-09-26 22:00:22.000000 netsnmp-py-0.5.2/netsnmp_py.egg-info/SOURCES.txt
+drwxrwxr-x   0 xsx       (1000) xsx       (1000)        0 2023-05-03 22:37:57.242852 netsnmp-py-0.6/
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)     1086 2023-05-03 22:18:45.000000 netsnmp-py-0.6/LICENSE
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)       23 2023-05-03 22:33:47.000000 netsnmp-py-0.6/MANIFEST.in
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)      677 2023-05-03 22:37:57.242852 netsnmp-py-0.6/PKG-INFO
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)     6179 2023-05-03 22:18:45.000000 netsnmp-py-0.6/README.md
+drwxrwxr-x   0 xsx       (1000) xsx       (1000)        0 2023-05-03 22:37:57.239519 netsnmp-py-0.6/netsnmp/
+-rwxrwxr-x   0 xsx       (1000) xsx       (1000)     4703 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/__init__.py
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)      148 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/__main__.py
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)     1814 2023-05-03 22:28:46.000000 netsnmp-py-0.6/netsnmp/_api.c
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)     1306 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/_api.h
+drwxrwxr-x   0 xsx       (1000) xsx       (1000)        0 2023-05-03 22:37:57.239519 netsnmp-py-0.6/netsnmp/_dev/
+-rwxrwxr-x   0 xsx       (1000) xsx       (1000)     1420 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/_dev/__init__.py
+-rwxrwxr-x   0 xsx       (1000) xsx       (1000)     1475 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/_dev/arris.py
+-rwxrwxr-x   0 xsx       (1000) xsx       (1000)     1306 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/_dev/cisco.py
+-rwxrwxr-x   0 xsx       (1000) xsx       (1000)     1545 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/_dev/technicolor.py
+-rwxrwxr-x   0 xsx       (1000) xsx       (1000)     2065 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/_hex.py
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)     6561 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/get.c
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)     7125 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/get_async.c
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)     5383 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/interface.c
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)     2481 2023-05-03 22:18:45.000000 netsnmp-py-0.6/netsnmp/session.c
+drwxrwxr-x   0 xsx       (1000) xsx       (1000)        0 2023-05-03 22:37:57.239519 netsnmp-py-0.6/netsnmp_py.egg-info/
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)      677 2023-05-03 22:37:57.000000 netsnmp-py-0.6/netsnmp_py.egg-info/PKG-INFO
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)      429 2023-05-03 22:37:57.000000 netsnmp-py-0.6/netsnmp_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)        1 2023-05-03 22:37:57.000000 netsnmp-py-0.6/netsnmp_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)        8 2023-05-03 22:37:57.000000 netsnmp-py-0.6/netsnmp_py.egg-info/top_level.txt
+-rw-rw-r--   0 xsx       (1000) xsx       (1000)       38 2023-05-03 22:37:57.242852 netsnmp-py-0.6/setup.cfg
+-rwxrwxr-x   0 xsx       (1000) xsx       (1000)     2358 2023-05-03 22:33:56.000000 netsnmp-py-0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `netsnmp-py-0.5.2/setup.py` & `netsnmp-py-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension, find_packages
 import os
 import re
 import sys
 
-VERSION="0.5.2"
+VERSION="0.6"
 
 intree=0
 
 _incdirs = ['./netsnmp']
 _libdirs = []
 
 args = sys.argv[:]
```

### Comparing `netsnmp-py-0.5.2/netsnmp/_api.h` & `netsnmp-py-0.6/netsnmp/_api.h`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 #if PY_MAJOR_VERSION >= 3
 #define Py_String PyUnicode_AsUTF8
 #else
 #define Py_String PyString_AsString
 #endif
 
-int _debug_level;
+static int _debug_level;
 
 /* Exceptions */
-PyObject *SNMPError;
+static PyObject *SNMPError;
 
 /* Functions */
 long long __py_attr_long (PyObject *obj, char *attr_name);
 void *__py_attr_void_ptr (PyObject *obj, char *attr_name);
 int __py_attr_get_string (PyObject *obj, char *attr_name, char **val, Py_ssize_t *len);
 int __py_attr_set_string (PyObject *obj, char *attr_name, char *val, size_t len);
```

### Comparing `netsnmp-py-0.5.2/netsnmp/_hex.py` & `netsnmp-py-0.6/netsnmp/_hex.py`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/get_async.c` & `netsnmp-py-0.6/netsnmp/get_async.c`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/session.c` & `netsnmp-py-0.6/netsnmp/session.c`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/_dev/arris.py` & `netsnmp-py-0.6/netsnmp/_dev/arris.py`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/_dev/technicolor.py` & `netsnmp-py-0.6/netsnmp/_dev/technicolor.py`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/_dev/cisco.py` & `netsnmp-py-0.6/netsnmp/_dev/cisco.py`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/_dev/__init__.py` & `netsnmp-py-0.6/netsnmp/_dev/__init__.py`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/interface.c` & `netsnmp-py-0.6/netsnmp/interface.c`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/_api.c` & `netsnmp-py-0.6/netsnmp/_api.c`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/get.c` & `netsnmp-py-0.6/netsnmp/get.c`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/netsnmp/__init__.py` & `netsnmp-py-0.6/netsnmp/__init__.py`

 * *Files identical despite different names*

### Comparing `netsnmp-py-0.5.2/PKG-INFO` & `netsnmp-py-0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: netsnmp-py
-Version: 0.5.2
+Version: 0.6
 Summary: Python NET-SNMP Bindings
 Home-page: https://github.com/xstaticxgpx/netsnmp-py3
+Download-URL: https://github.com/xstaticxgpx/netsnmp-py3/archive/v0.6.tar.gz
 Author: Gabe Pacuilla
 Author-email: root@un1x.su
 License: MIT License
-Download-URL: https://github.com/xstaticxgpx/netsnmp-py3/archive/v0.5.2.tar.gz
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
```

### Comparing `netsnmp-py-0.5.2/netsnmp_py.egg-info/PKG-INFO` & `netsnmp-py-0.6/netsnmp_py.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: netsnmp-py
-Version: 0.5.2
+Version: 0.6
 Summary: Python NET-SNMP Bindings
 Home-page: https://github.com/xstaticxgpx/netsnmp-py3
+Download-URL: https://github.com/xstaticxgpx/netsnmp-py3/archive/v0.6.tar.gz
 Author: Gabe Pacuilla
 Author-email: root@un1x.su
 License: MIT License
-Download-URL: https://github.com/xstaticxgpx/netsnmp-py3/archive/v0.5.2.tar.gz
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
```

