# Comparing `tmp/linear_segment-1.0.0.tar.gz` & `tmp/linear_segment-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linear_segment-1.0.0.tar", max compression
+gzip compressed data, was "linear_segment-1.1.0.tar", max compression
```

## Comparing `linear_segment-1.0.0.tar` & `linear_segment-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 linear_segment-1.0.0/LICENSE.md
--rwxr-xr-x   0        0        0     1254 2023-05-04 19:54:32.603957 linear_segment-1.0.0/README.md
--rw-r--r--   0        0        0     3165 2023-04-17 20:47:05.102440 linear_segment-1.0.0/build.py
--rw-r--r--   0        0        0      516 2023-04-28 02:21:21.661728 linear_segment-1.0.0/linear_segment/__init__.py
--rw-r--r--   0        0        0      360 2022-01-03 18:39:41.000000 linear_segment-1.0.0/linear_segment/bcpseg/__init__.py
--rw-r--r--   0        0        0   277568 2023-05-04 20:11:41.909053 linear_segment-1.0.0/linear_segment/bcpseg/bcp_segment.cpython-310-darwin.so
--rw-r--r--   0        0        0     1645 2023-01-20 21:31:50.305716 linear_segment-1.0.0/linear_segment/bcpseg/bcp_segment.pxd
--rw-r--r--   0        0        0     4661 2023-01-20 21:31:40.405370 linear_segment-1.0.0/linear_segment/bcpseg/bcp_segment.pyx
--rw-r--r--   0        0        0     6467 2023-01-20 21:19:10.647095 linear_segment-1.0.0/linear_segment/bcpseg/offline_bcp.c
--rw-r--r--   0        0        0      961 2023-01-20 21:21:47.447343 linear_segment-1.0.0/linear_segment/bcpseg/offline_bcp.h
--rw-r--r--   0        0        0     8800 2023-04-20 02:41:55.640952 linear_segment-1.0.0/linear_segment/bcpseg/online_bcp.c
--rw-r--r--   0        0        0     1431 2023-01-20 21:20:50.904296 linear_segment-1.0.0/linear_segment/bcpseg/online_bcp.h
--rw-r--r--   0        0        0     1701 2021-02-11 22:36:12.000000 linear_segment-1.0.0/linear_segment/bcpseg/utilities.c
--rwxr-xr-x   0        0        0      278 2023-01-22 03:11:51.518864 linear_segment-1.0.0/linear_segment/cbseg/__init__.py
--rwxr-xr-x   0        0        0     2793 2023-01-22 02:18:08.520477 linear_segment-1.0.0/linear_segment/cbseg/cbs.h
--rwxr-xr-x   0        0        0     3806 2022-05-10 18:30:51.000000 linear_segment-1.0.0/linear_segment/cbseg/cbs_labeled.c
--rwxr-xr-x   0        0        0     4011 2023-01-22 02:20:03.158112 linear_segment-1.0.0/linear_segment/cbseg/cbs_structs.c
--rw-r--r--   0        0        0   279200 2023-05-04 20:11:41.909404 linear_segment-1.0.0/linear_segment/cbseg/cbseg.cpython-310-darwin.so
--rwxr-xr-x   0        0        0     2504 2023-01-22 02:19:27.213561 linear_segment-1.0.0/linear_segment/cbseg/cbseg.pxd
--rwxr-xr-x   0        0        0     6096 2023-04-17 20:15:15.471887 linear_segment-1.0.0/linear_segment/cbseg/cbseg.pyx
--rwxr-xr-x   0        0        0     2186 2019-08-27 17:01:40.000000 linear_segment-1.0.0/linear_segment/cbseg/utilities.c
--rw-r--r--   0        0        0     1679 2023-04-28 02:20:34.141366 linear_segment-1.0.0/linear_segment/segment.py
--rw-r--r--   0        0        0     2217 2023-05-04 19:55:03.406458 linear_segment-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2951 1970-01-01 00:00:00.000000 linear_segment-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 linear_segment-1.1.0/LICENSE.md
+-rwxr-xr-x   0        0        0     1254 2023-05-04 19:54:32.603957 linear_segment-1.1.0/README.md
+-rw-r--r--   0        0        0     3165 2023-04-17 20:47:05.102440 linear_segment-1.1.0/build.py
+-rw-r--r--   0        0        0      516 2023-05-04 20:35:45.630303 linear_segment-1.1.0/linear_segment/__init__.py
+-rw-r--r--   0        0        0      130 2023-05-04 20:36:02.637573 linear_segment-1.1.0/linear_segment/bcpseg/__init__.py
+-rw-r--r--   0        0        0   277568 2023-05-04 20:13:39.856965 linear_segment-1.1.0/linear_segment/bcpseg/bcp_segment.cpython-310-darwin.so
+-rw-r--r--   0        0        0     1645 2023-01-20 21:31:50.305716 linear_segment-1.1.0/linear_segment/bcpseg/bcp_segment.pxd
+-rw-r--r--   0        0        0     4661 2023-01-20 21:31:40.405370 linear_segment-1.1.0/linear_segment/bcpseg/bcp_segment.pyx
+-rw-r--r--   0        0        0     6467 2023-01-20 21:19:10.647095 linear_segment-1.1.0/linear_segment/bcpseg/offline_bcp.c
+-rw-r--r--   0        0        0      961 2023-01-20 21:21:47.447343 linear_segment-1.1.0/linear_segment/bcpseg/offline_bcp.h
+-rw-r--r--   0        0        0     8800 2023-04-20 02:41:55.640952 linear_segment-1.1.0/linear_segment/bcpseg/online_bcp.c
+-rw-r--r--   0        0        0     1431 2023-01-20 21:20:50.904296 linear_segment-1.1.0/linear_segment/bcpseg/online_bcp.h
+-rw-r--r--   0        0        0     1701 2021-02-11 22:36:12.000000 linear_segment-1.1.0/linear_segment/bcpseg/utilities.c
+-rwxr-xr-x   0        0        0      261 2023-05-04 20:35:32.689020 linear_segment-1.1.0/linear_segment/cbseg/__init__.py
+-rwxr-xr-x   0        0        0     2793 2023-01-22 02:18:08.520477 linear_segment-1.1.0/linear_segment/cbseg/cbs.h
+-rwxr-xr-x   0        0        0     3806 2022-05-10 18:30:51.000000 linear_segment-1.1.0/linear_segment/cbseg/cbs_labeled.c
+-rwxr-xr-x   0        0        0     4011 2023-01-22 02:20:03.158112 linear_segment-1.1.0/linear_segment/cbseg/cbs_structs.c
+-rw-r--r--   0        0        0   279200 2023-05-04 20:13:39.857338 linear_segment-1.1.0/linear_segment/cbseg/cbseg.cpython-310-darwin.so
+-rwxr-xr-x   0        0        0     2504 2023-01-22 02:19:27.213561 linear_segment-1.1.0/linear_segment/cbseg/cbseg.pxd
+-rwxr-xr-x   0        0        0     6096 2023-04-17 20:15:15.471887 linear_segment-1.1.0/linear_segment/cbseg/cbseg.pyx
+-rwxr-xr-x   0        0        0     2186 2019-08-27 17:01:40.000000 linear_segment-1.1.0/linear_segment/cbseg/utilities.c
+-rw-r--r--   0        0        0     1679 2023-04-28 02:20:34.141366 linear_segment-1.1.0/linear_segment/segment.py
+-rw-r--r--   0        0        0     2217 2023-05-04 20:36:22.750799 linear_segment-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2951 1970-01-01 00:00:00.000000 linear_segment-1.1.0/PKG-INFO
```

### Comparing `linear_segment-1.0.0/LICENSE.md` & `linear_segment-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/README.md` & `linear_segment-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/build.py` & `linear_segment-1.1.0/build.py`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/__init__.py` & `linear_segment-1.1.0/linear_segment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import absolute_import
 from .segment import segment
 from .bcpseg.bcp_segment import bcpseg
 from .bcpseg.bcp_segment import get_include
 from .cbseg.cbseg import determine_cbs_stat, determine_t_stat, determine_cbs, cbs_segment, validate, init_segment
 
 # This is extracted automatically by the top-level setup.py.
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 __author__ = "Kyle S. Smith"
 
 __doc__ = """\
 
 linear_segment
 ==============
```

### Comparing `linear_segment-1.0.0/linear_segment/bcpseg/bcp_segment.cpython-310-darwin.so` & `linear_segment-1.1.0/linear_segment/bcpseg/bcp_segment.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/bcpseg/bcp_segment.pxd` & `linear_segment-1.1.0/linear_segment/bcpseg/bcp_segment.pxd`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/bcpseg/bcp_segment.pyx` & `linear_segment-1.1.0/linear_segment/bcpseg/bcp_segment.pyx`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/bcpseg/offline_bcp.c` & `linear_segment-1.1.0/linear_segment/bcpseg/offline_bcp.c`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/bcpseg/offline_bcp.h` & `linear_segment-1.1.0/linear_segment/bcpseg/offline_bcp.h`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/bcpseg/online_bcp.c` & `linear_segment-1.1.0/linear_segment/bcpseg/online_bcp.c`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/bcpseg/online_bcp.h` & `linear_segment-1.1.0/linear_segment/bcpseg/online_bcp.h`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/bcpseg/utilities.c` & `linear_segment-1.1.0/linear_segment/bcpseg/utilities.c`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/cbseg/cbs.h` & `linear_segment-1.1.0/linear_segment/cbseg/cbs.h`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/cbseg/cbs_labeled.c` & `linear_segment-1.1.0/linear_segment/cbseg/cbs_labeled.c`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/cbseg/cbs_structs.c` & `linear_segment-1.1.0/linear_segment/cbseg/cbs_structs.c`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/cbseg/cbseg.cpython-310-darwin.so` & `linear_segment-1.1.0/linear_segment/cbseg/cbseg.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/cbseg/cbseg.pxd` & `linear_segment-1.1.0/linear_segment/cbseg/cbseg.pxd`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/cbseg/cbseg.pyx` & `linear_segment-1.1.0/linear_segment/cbseg/cbseg.pyx`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/cbseg/utilities.c` & `linear_segment-1.1.0/linear_segment/cbseg/utilities.c`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/linear_segment/segment.py` & `linear_segment-1.1.0/linear_segment/segment.py`

 * *Files identical despite different names*

### Comparing `linear_segment-1.0.0/pyproject.toml` & `linear_segment-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linear_segment"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python package for Bayesian Change Point and Circular Binary Segmentation"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/linear_segment"
 documentation = "https://www.biosciencestack.com/static/linear_segment/docs/index.html"
 keywords = ["cython", "bayesian", "changepoint", "circular", "segment", "c"]
 readme = 'README.md'
```

### Comparing `linear_segment-1.0.0/PKG-INFO` & `linear_segment-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-segment
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python package for Bayesian Change Point and Circular Binary Segmentation
 Home-page: https://github.com/kylessmith/linear_segment
 License: GPL-2.0-or-later
 Keywords: cython,bayesian,changepoint,circular,segment,c
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
```

