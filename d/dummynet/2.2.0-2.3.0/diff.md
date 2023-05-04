# Comparing `tmp/dummynet-2.2.0-py2.py3-none-any.whl.zip` & `tmp/dummynet-2.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 12089 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      421 b- defN 23-May-02 07:21 dummynet/__init__.py
--rw-rw-r--  2.0 unx     9719 b- defN 23-May-02 08:15 dummynet/dummy_net.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-02 08:15 dummynet/errors.py
--rw-rw-r--  2.0 unx     3071 b- defN 23-May-02 08:15 dummynet/host_shell.py
--rw-rw-r--  2.0 unx      772 b- defN 22-Dec-25 13:20 dummynet/namespace_shell.py
--rw-rw-r--  2.0 unx      508 b- defN 23-May-02 07:21 dummynet/process.py
--rw-rw-r--  2.0 unx     9586 b- defN 23-May-02 08:15 dummynet/process_monitor.py
--rw-rw-r--  2.0 unx     4610 b- defN 23-May-02 08:15 dummynet/run_info.py
--rw-rw-r--  2.0 unx     1505 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/LICENSE.rst
--rw-rw-r--  2.0 unx     1948 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1022 b- defN 23-May-02 08:16 dummynet-2.2.0.dist-info/RECORD
-13 files, 35028 bytes uncompressed, 10395 bytes compressed:  70.3%
+Zip file size: 12086 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      421 b- defN 23-Jan-10 14:33 dummynet/__init__.py
+-rw-rw-r--  2.0 unx     9719 b- defN 23-May-04 07:33 dummynet/dummy_net.py
+-rw-rw-r--  2.0 unx     1754 b- defN 23-May-04 08:29 dummynet/errors.py
+-rw-rw-r--  2.0 unx     3071 b- defN 23-May-04 07:33 dummynet/host_shell.py
+-rw-rw-r--  2.0 unx      772 b- defN 22-Dec-22 13:38 dummynet/namespace_shell.py
+-rw-rw-r--  2.0 unx      508 b- defN 23-Jan-10 14:33 dummynet/process.py
+-rw-rw-r--  2.0 unx     9586 b- defN 23-May-04 07:33 dummynet/process_monitor.py
+-rw-rw-r--  2.0 unx     4610 b- defN 23-May-04 07:33 dummynet/run_info.py
+-rw-rw-r--  2.0 unx     1505 b- defN 23-May-04 09:02 dummynet-2.3.0.dist-info/LICENSE.rst
+-rw-rw-r--  2.0 unx     1948 b- defN 23-May-04 09:02 dummynet-2.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-04 09:02 dummynet-2.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-04 09:02 dummynet-2.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1022 b- defN 23-May-04 09:02 dummynet-2.3.0.dist-info/RECORD
+13 files, 35035 bytes uncompressed, 10392 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: dummynet/process_monitor.py
 Comment: 
 
 Filename: dummynet/run_info.py
 Comment: 
 
-Filename: dummynet-2.2.0.dist-info/LICENSE.rst
+Filename: dummynet-2.3.0.dist-info/LICENSE.rst
 Comment: 
 
-Filename: dummynet-2.2.0.dist-info/METADATA
+Filename: dummynet-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: dummynet-2.2.0.dist-info/WHEEL
+Filename: dummynet-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: dummynet-2.2.0.dist-info/top_level.txt
+Filename: dummynet-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dummynet-2.2.0.dist-info/RECORD
+Filename: dummynet-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dummynet/errors.py

```diff
@@ -31,15 +31,15 @@
 
 class DaemonExitError(DummyNetError):
     """Exception for when the process monitor is started with only
     daemon processes.
     """
 
     def __init__(self, process):
-        super().__init__(f"Unexpected daemon exit {process}")
+        super().__init__(f"Unexpected daemon exit: {process.info} ")
 
 
 class AllDaemonsError(DummyNetError):
     """Exception for when the process monitor is started with only
     daemon processes.
     """
```

## Comparing `dummynet-2.2.0.dist-info/LICENSE.rst` & `dummynet-2.3.0.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `dummynet-2.2.0.dist-info/METADATA` & `dummynet-2.3.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummynet
-Version: 2.2.0
+Version: 2.3.0
 Summary: A tool for creating dummy networks using network namespaces.
 Home-page: https://github.com/steinwurf/dummynet
 Author: Steinwurf ApS
 Author-email: contact@steinwurf.com
 License: BSD 3-clause "New" or "Revised" License
 Keywords: dummynet,network,namespace
 Platform: UNKNOWN
```

