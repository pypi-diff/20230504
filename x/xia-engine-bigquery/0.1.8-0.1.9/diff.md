# Comparing `tmp/xia_engine_bigquery-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_bigquery-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 475885 bytes, number of entries: 9
--rw-r--r--  2.0 unx      361 b- defN 23-Apr-26 10:42 xia_engine_bigquery/__init__.py
--rw-r--r--  2.0 unx   640000 b- defN 23-Apr-26 20:21 xia_engine_bigquery/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   299520 b- defN 23-Apr-26 20:21 xia_engine_bigquery/proto.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   294912 b- defN 23-Apr-26 20:19 xia_engine_bigquery/schema.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-26 20:21 xia_engine_bigquery-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      886 b- defN 23-Apr-26 20:21 xia_engine_bigquery-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-26 20:21 xia_engine_bigquery-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-26 20:21 xia_engine_bigquery-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      846 b- defN 23-Apr-26 20:21 xia_engine_bigquery-0.1.8.dist-info/RECORD
-9 files, 1236796 bytes uncompressed, 474403 bytes compressed:  61.6%
+Zip file size: 475010 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      361 b- defN 23-Apr-26 20:53 xia_engine_bigquery/__init__.py
+-rw-r--r--  2.0 unx   638464 b- defN 23-Apr-26 21:03 xia_engine_bigquery/engine.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   299520 b- defN 23-Apr-26 21:04 xia_engine_bigquery/proto.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   294912 b- defN 23-Apr-26 21:02 xia_engine_bigquery/schema.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-26 21:04 xia_engine_bigquery-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      886 b- defN 23-Apr-26 21:04 xia_engine_bigquery-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-26 21:04 xia_engine_bigquery-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-26 21:04 xia_engine_bigquery-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      846 b- defN 23-Apr-26 21:04 xia_engine_bigquery-0.1.9.dist-info/RECORD
+9 files, 1235260 bytes uncompressed, 473528 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_engine_bigquery/proto.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_engine_bigquery/schema.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.8.dist-info/LICENSE.txt
+Filename: xia_engine_bigquery-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.8.dist-info/METADATA
+Filename: xia_engine_bigquery-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.8.dist-info/WHEEL
+Filename: xia_engine_bigquery-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.8.dist-info/top_level.txt
+Filename: xia_engine_bigquery-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_bigquery-0.1.8.dist-info/RECORD
+Filename: xia_engine_bigquery-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_bigquery/__init__.py

```diff
@@ -5,8 +5,8 @@
 
 __all__ = [
     "DocToProto",
     "DocToSchema",
     "BigqueryWriteEngine", "BigqueryStreamEngine", "BigqueryAppendOnlyEngine"
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_engine_bigquery-0.1.8.dist-info/METADATA` & `xia_engine_bigquery-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-bigquery
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A Document Engine on Bigquery
-Home-page: https://develop.x-i-a.com/docs/xia-engine-bigquery/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-bigquery/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_bigquery-0.1.8.dist-info/RECORD` & `xia_engine_bigquery-0.1.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-xia_engine_bigquery/__init__.py,sha256=xXDUxFVdVPQmlEWukZfA2aAlxZMcyUTivwzxwoYpun4,361
-xia_engine_bigquery/engine.cp39-win_amd64.pyd,sha256=rvfHntEE9mv6ZsSPZgQw_g47jOwtrohojpzcKosiVM8,640000
-xia_engine_bigquery/proto.cp39-win_amd64.pyd,sha256=3XiOnLCiWFiM6eeBKZ-toeYa7xgpUcbYvPyuxskAANc,299520
-xia_engine_bigquery/schema.cp39-win_amd64.pyd,sha256=DeJm-o9XCUrcGCgKNwQG-vA2drBpyJmUAr_BsA6f0g4,294912
-xia_engine_bigquery-0.1.8.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_engine_bigquery-0.1.8.dist-info/METADATA,sha256=Sy2p2Mr8S9bN4etWLFPt5BrqOUquULl1-ajqeRFAHfU,886
-xia_engine_bigquery-0.1.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_bigquery-0.1.8.dist-info/top_level.txt,sha256=_yEmJhHpPT-DWURs_JBDhoK6nResg3ySwAYjmia8-Cg,20
-xia_engine_bigquery-0.1.8.dist-info/RECORD,,
+xia_engine_bigquery/__init__.py,sha256=P2Tb6uz48lSSeMrE3dGNpegHx3SyF3DA5x1v7rqJrZs,361
+xia_engine_bigquery/engine.cp39-win_amd64.pyd,sha256=OHocDgUGOlf5xoe9tcqkLojxruKIYoPQzh8PNH7Uqks,638464
+xia_engine_bigquery/proto.cp39-win_amd64.pyd,sha256=_NIko-dsX_ZGtTcPTSCMtpPziK4qTAdX7r5tuOM9Gn0,299520
+xia_engine_bigquery/schema.cp39-win_amd64.pyd,sha256=zfARIjkYNpVDzP1rFczM3_dr7Z5Aonh6wmFKXV91rmM,294912
+xia_engine_bigquery-0.1.9.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine_bigquery-0.1.9.dist-info/METADATA,sha256=Q2Fkt9X-zs3rF-ZyvS5L167toYK3FxRTdR9qWQSIS28,886
+xia_engine_bigquery-0.1.9.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_bigquery-0.1.9.dist-info/top_level.txt,sha256=_yEmJhHpPT-DWURs_JBDhoK6nResg3ySwAYjmia8-Cg,20
+xia_engine_bigquery-0.1.9.dist-info/RECORD,,
```

