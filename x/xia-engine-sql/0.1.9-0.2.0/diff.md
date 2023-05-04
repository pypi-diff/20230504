# Comparing `tmp/xia_engine_sql-0.1.9-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_sql-0.2.0-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 296211 bytes, number of entries: 7
--rw-r--r--  2.0 unx      171 b- defN 23-Feb-04 21:52 xia_engine_sql/__init__.py
--rw-r--r--  2.0 unx   817152 b- defN 23-Feb-04 21:56 xia_engine_sql/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      155 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      669 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      604 b- defN 23-Feb-04 21:56 xia_engine_sql-0.1.9.dist-info/RECORD
-7 files, 818865 bytes uncompressed, 295129 bytes compressed:  64.0%
+Zip file size: 247461 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      171 b- defN 23-May-04 20:22 xia_engine_sql/__init__.py
+-rw-r--r--  2.0 unx   695776 b- defN 23-May-04 20:22 xia_engine_sql/engine.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-May-04 20:22 xia_engine_sql-0.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      632 b- defN 23-May-04 20:22 xia_engine_sql-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-04 20:22 xia_engine_sql-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-04 20:22 xia_engine_sql-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      608 b- defN 23-May-04 20:22 xia_engine_sql-0.2.0.dist-info/RECORD
+7 files, 697462 bytes uncompressed, 246373 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_sql/__init__.py
 Comment: 
 
-Filename: xia_engine_sql/engine.cp39-win_amd64.pyd
+Filename: xia_engine_sql/engine.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_engine_sql-0.1.9.dist-info/LICENSE.txt
+Filename: xia_engine_sql-0.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_sql-0.1.9.dist-info/METADATA
+Filename: xia_engine_sql-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_sql-0.1.9.dist-info/WHEEL
+Filename: xia_engine_sql-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_sql-0.1.9.dist-info/top_level.txt
+Filename: xia_engine_sql-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_sql-0.1.9.dist-info/RECORD
+Filename: xia_engine_sql-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_sql/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_sql.engine import SqlEngine, SqliteEngine, SqliteConnectParam
 
 
 __all__ = [
     "SqlEngine", "SqliteEngine", "SqliteConnectParam"
 ]
 
-__version__ = "0.1.9"
+__version__ = "0.2.0"
```

## Comparing `xia_engine_sql-0.1.9.dist-info/METADATA` & `xia_engine_sql-0.2.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-engine-sql
-Version: 0.1.9
+Version: 0.2.0
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-sql/0.1.9/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-sql/0.2.0/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-engine
 
 .. image:: https://img.shields.io/pypi/v/xia-engine-sql.svg?color=blue
    :alt: PyPI-Server
@@ -26,9 +24,7 @@
 =============================
 
 Install the package::
 
     pip install xia-engine-sql
 
 
-
-
```

