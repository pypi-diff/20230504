# Comparing `tmp/determined_common-0.22.0rc0-py3-none-any.whl.zip` & `tmp/determined_common-0.22.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 1814 bytes, number of entries: 6
--rw-r--r--  2.0 unx      235 b- defN 23-May-03 16:27 determined_common/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-May-03 16:27 determined_common/__version__.py
--rw-r--r--  2.0 unx      417 b- defN 23-May-03 16:27 determined_common-0.22.0rc0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 16:27 determined_common-0.22.0rc0.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-03 16:27 determined_common-0.22.0rc0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      525 b- defN 23-May-03 16:27 determined_common-0.22.0rc0.dist-info/RECORD
+-rw-r--r--  2.0 unx      235 b- defN 23-May-04 02:31 determined_common/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-May-04 02:31 determined_common/__version__.py
+-rw-r--r--  2.0 unx      417 b- defN 23-May-04 02:31 determined_common-0.22.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 02:31 determined_common-0.22.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-May-04 02:31 determined_common-0.22.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      525 b- defN 23-May-04 02:31 determined_common-0.22.0rc1.dist-info/RECORD
 6 files, 1314 bytes uncompressed, 846 bytes compressed:  35.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_common/__init__.py
 Comment: 
 
 Filename: determined_common/__version__.py
 Comment: 
 
-Filename: determined_common-0.22.0rc0.dist-info/METADATA
+Filename: determined_common-0.22.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: determined_common-0.22.0rc0.dist-info/WHEEL
+Filename: determined_common-0.22.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: determined_common-0.22.0rc0.dist-info/top_level.txt
+Filename: determined_common-0.22.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_common-0.22.0rc0.dist-info/RECORD
+Filename: determined_common-0.22.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_common/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.22.0-rc0"
+__version__ = "0.22.0-rc1"
```

## Comparing `determined_common-0.22.0rc0.dist-info/RECORD` & `determined_common-0.22.0rc1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 determined_common/__init__.py,sha256=cHo0m87BOaQx-d4abum7tAeKV_ukSvs3xkABM7R76OM,235
-determined_common/__version__.py,sha256=QYEOgKd2NTi5ivT8TFJTAx-w1gMBjMkPMbj2LLk2EBk,27
-determined_common-0.22.0rc0.dist-info/METADATA,sha256=DlJYzLQX6POBxZS4M5FtyD8-vYZ9a6E7q9GNhC3Db5o,417
-determined_common-0.22.0rc0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-determined_common-0.22.0rc0.dist-info/top_level.txt,sha256=CD1pq4FvMD2KEVXd1cFj6S6gCC-Th-FtDLBZojRsg98,18
-determined_common-0.22.0rc0.dist-info/RECORD,,
+determined_common/__version__.py,sha256=fTABuLLa5fjgUuX5JLbDDlMgr0t_yyWce1IytlmxZoQ,27
+determined_common-0.22.0rc1.dist-info/METADATA,sha256=Voro5Vz5X_v6XHvNXKJIIrdsB1jSr3nngfR-b7fKxek,417
+determined_common-0.22.0rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+determined_common-0.22.0rc1.dist-info/top_level.txt,sha256=CD1pq4FvMD2KEVXd1cFj6S6gCC-Th-FtDLBZojRsg98,18
+determined_common-0.22.0rc1.dist-info/RECORD,,
```

