# Comparing `tmp/xapi-python-0.1.2.tar.gz` & `tmp/xapi-python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xapi-python-0.1.2.tar", last modified: Wed May  3 10:24:53 2023, max compression
+gzip compressed data, was "xapi-python-0.1.3.tar", last modified: Thu May  4 10:12:39 2023, max compression
```

## Comparing `xapi-python-0.1.2.tar` & `xapi-python-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-03 10:24:53.668141 xapi-python-0.1.2/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.1.2/LICENSE
--rw-r--r--   0 pawel     (1000) pawel     (1000)     8203 2023-05-03 10:24:53.668141 xapi-python-0.1.2/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5898 2023-05-03 10:23:56.000000 xapi-python-0.1.2/README.md
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1232 2023-05-03 10:23:56.000000 xapi-python-0.1.2/pyproject.toml
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-05-03 10:24:53.668141 xapi-python-0.1.2/setup.cfg
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2023-05-03 10:23:56.000000 xapi-python-0.1.2/setup.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-03 10:24:53.668141 xapi-python-0.1.2/tests/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5121 2023-05-02 15:09:32.000000 xapi-python-0.1.2/tests/test_connect.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.1.2/tests/test_socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.1.2/tests/test_stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-29 10:20:03.000000 xapi-python-0.1.2/tests/test_xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-03 10:24:53.668141 xapi-python-0.1.2/xapi/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-05-03 10:23:56.000000 xapi-python-0.1.2/xapi/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2228 2023-05-03 10:23:56.000000 xapi-python-0.1.2/xapi/connection.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.1.2/xapi/enums.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      205 2023-04-29 11:41:41.000000 xapi-python-0.1.2/xapi/exceptions.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-29 11:38:37.000000 xapi-python-0.1.2/xapi/socket.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-29 11:39:31.000000 xapi-python-0.1.2/xapi/stream.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2209 2023-05-03 10:23:56.000000 xapi-python-0.1.2/xapi/xapi.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-03 10:24:53.668141 xapi-python-0.1.2/xapi_python.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     8203 2023-05-03 10:24:53.000000 xapi-python-0.1.2/xapi_python.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      376 2023-05-03 10:24:53.000000 xapi-python-0.1.2/xapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-05-03 10:24:53.000000 xapi-python-0.1.2/xapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-05-03 10:24:53.000000 xapi-python-0.1.2/xapi_python.egg-info/top_level.txt
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-04 10:12:39.830490 xapi-python-0.1.3/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1071 2023-04-25 04:51:26.000000 xapi-python-0.1.3/LICENSE
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8203 2023-05-04 10:12:39.830490 xapi-python-0.1.3/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5898 2023-05-03 10:23:56.000000 xapi-python-0.1.3/README.md
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1131 2023-05-03 10:40:10.000000 xapi-python-0.1.3/pyproject.toml
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2023-05-04 10:12:39.830490 xapi-python-0.1.3/setup.cfg
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1027 2023-05-03 10:38:51.000000 xapi-python-0.1.3/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-04 10:12:39.830490 xapi-python-0.1.3/tests/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5121 2023-05-02 15:09:32.000000 xapi-python-0.1.3/tests/test_connect.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7958 2023-04-26 11:15:10.000000 xapi-python-0.1.3/tests/test_socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4014 2023-04-27 05:35:22.000000 xapi-python-0.1.3/tests/test_stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1566 2023-04-29 10:20:03.000000 xapi-python-0.1.3/tests/test_xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-04 10:12:39.830490 xapi-python-0.1.3/xapi/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      338 2023-05-03 10:39:00.000000 xapi-python-0.1.3/xapi/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2228 2023-05-03 10:23:56.000000 xapi-python-0.1.3/xapi/connection.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1464 2023-04-24 14:52:49.000000 xapi-python-0.1.3/xapi/enums.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      205 2023-04-29 11:41:41.000000 xapi-python-0.1.3/xapi/exceptions.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     6640 2023-04-29 11:38:37.000000 xapi-python-0.1.3/xapi/socket.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2947 2023-04-29 11:39:31.000000 xapi-python-0.1.3/xapi/stream.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2209 2023-05-03 10:23:56.000000 xapi-python-0.1.3/xapi/xapi.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2023-05-04 10:12:39.830490 xapi-python-0.1.3/xapi_python.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     8203 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      410 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       19 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        5 2023-05-04 10:12:39.000000 xapi-python-0.1.3/xapi_python.egg-info/top_level.txt
```

### Comparing `xapi-python-0.1.2/LICENSE` & `xapi-python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/PKG-INFO` & `xapi-python-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
```

### Comparing `xapi-python-0.1.2/README.md` & `xapi-python-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/setup.py` & `xapi-python-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,10 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12"
     ],
     python_requires='>=3.7',
-    version="0.1.2",
+    version="0.1.3",
     packages=['xapi'],
 )
```

### Comparing `xapi-python-0.1.2/tests/test_connect.py` & `xapi-python-0.1.3/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/tests/test_socket.py` & `xapi-python-0.1.3/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/tests/test_stream.py` & `xapi-python-0.1.3/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/tests/test_xapi.py` & `xapi-python-0.1.3/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/xapi/connection.py` & `xapi-python-0.1.3/xapi/connection.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/xapi/enums.py` & `xapi-python-0.1.3/xapi/enums.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/xapi/socket.py` & `xapi-python-0.1.3/xapi/socket.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/xapi/stream.py` & `xapi-python-0.1.3/xapi/stream.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/xapi/xapi.py` & `xapi-python-0.1.3/xapi/xapi.py`

 * *Files identical despite different names*

### Comparing `xapi-python-0.1.2/xapi_python.egg-info/PKG-INFO` & `xapi-python-0.1.3/xapi_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xapi-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: The xStation5 API Python library
 Home-page: https://github.com/pawelkn/xapi-python
 Author: Paweł Knioła
 Author-email: Paweł Knioła <pawel.kn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Paweł Knioła
```

