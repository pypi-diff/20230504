# Comparing `tmp/xia_fields-0.3.6-cp39-none-win_amd64.whl.zip` & `tmp/xia_fields-0.3.7-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 459779 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1177 b- defN 23-Apr-16 10:11 xia_fields/__init__.py
--rw-r--r--  2.0 unx   366080 b- defN 23-Apr-16 10:15 xia_fields/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   415232 b- defN 23-Apr-16 10:16 xia_fields/fields.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   387584 b- defN 23-Apr-16 10:17 xia_fields/fields_ext.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-16 10:17 xia_fields-0.3.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3308 b- defN 23-Apr-16 10:17 xia_fields-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-16 10:17 xia_fields-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-16 10:17 xia_fields-0.3.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      770 b- defN 23-Apr-16 10:17 xia_fields-0.3.6.dist-info/RECORD
-9 files, 1174413 bytes uncompressed, 458453 bytes compressed:  61.0%
+Zip file size: 459800 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1177 b- defN 23-May-04 05:14 xia_fields/__init__.py
+-rw-r--r--  2.0 unx   366080 b- defN 23-May-04 05:18 xia_fields/base.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   415232 b- defN 23-May-04 05:19 xia_fields/fields.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   387584 b- defN 23-May-04 05:20 xia_fields/fields_ext.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-May-04 05:20 xia_fields-0.3.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3308 b- defN 23-May-04 05:20 xia_fields-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-04 05:20 xia_fields-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-04 05:20 xia_fields-0.3.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      770 b- defN 23-May-04 05:20 xia_fields-0.3.7.dist-info/RECORD
+9 files, 1174413 bytes uncompressed, 458474 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_fields/fields.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_fields/fields_ext.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_fields-0.3.6.dist-info/LICENSE.txt
+Filename: xia_fields-0.3.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_fields-0.3.6.dist-info/METADATA
+Filename: xia_fields-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: xia_fields-0.3.6.dist-info/WHEEL
+Filename: xia_fields-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: xia_fields-0.3.6.dist-info/top_level.txt
+Filename: xia_fields-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_fields-0.3.6.dist-info/RECORD
+Filename: xia_fields-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_fields/__init__.py

```diff
@@ -14,8 +14,8 @@
     "JsonField", "DictField", "CompressedStringField",
     "Int64Field", "Int32Field", "SFixed64Field", "SFixed32Field",
     "UInt64Field", "UInt32Field", "Fixed64Field", "Fixed32Field",
     "DoubleField", "DateField", "TimestampField", "TimeField", "DateTimeField",
     "OsEnvironField"
 ]
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
```

## Comparing `xia_fields-0.3.6.dist-info/METADATA` & `xia_fields-0.3.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-fields
-Version: 0.3.6
+Version: 0.3.7
 Summary: X-I-A Field Protocol
-Home-page: https://develop.x-i-a.com/docs/xia-fields/0.3.6/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-fields/0.3.7/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_fields-0.3.6.dist-info/RECORD` & `xia_fields-0.3.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-xia_fields/__init__.py,sha256=vaTNovq-98Dfl_nFk4lFsiUy3iyl8U7VO9XSPdjQXdY,1177
-xia_fields/base.cp39-win_amd64.pyd,sha256=bBi58pGoXHjX3Zl_rPGIfXGiAoNBZy71_owakfwOCUA,366080
-xia_fields/fields.cp39-win_amd64.pyd,sha256=rr7bmgzMN7urspap-yHRSzYRsVn8S8j-j9uTVRVj0eo,415232
-xia_fields/fields_ext.cp39-win_amd64.pyd,sha256=EDVj6ZJtICvk8CqX5ZW_TbX6fn31_HIhSaXQuQ0h9X4,387584
-xia_fields-0.3.6.dist-info/LICENSE.txt,sha256=WB-w9CuI3gzpFzRjX4F3eIZ56mg24bUewXiu42z75DU,152
-xia_fields-0.3.6.dist-info/METADATA,sha256=a39UB_d3_wPKsg5_5iGqaZOfVAHNWU543ZiEPxn7SR0,3308
-xia_fields-0.3.6.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_fields-0.3.6.dist-info/top_level.txt,sha256=pXvwXCVXR-n1PTScNVgqx5GAlG0H2tIpu7XuuswUrng,11
-xia_fields-0.3.6.dist-info/RECORD,,
+xia_fields/__init__.py,sha256=f1kqAQI2RHNiKEcgXcVOu6OESdGGjqztnivpr2wRsW0,1177
+xia_fields/base.cp39-win_amd64.pyd,sha256=7a5J-1BrDPIGsGEdfMZjIansYOO_6R_gzwA-flM1BWo,366080
+xia_fields/fields.cp39-win_amd64.pyd,sha256=F3gQYxbPxGGkEMbm8OIaZ4N_RZC9x41WbeLQ0LzlmrI,415232
+xia_fields/fields_ext.cp39-win_amd64.pyd,sha256=EvU9I-pUj1slKzojTwvlGrQCqG0zv33UtN6jrPilNug,387584
+xia_fields-0.3.7.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_fields-0.3.7.dist-info/METADATA,sha256=KdMd7BYDAIMpBSdxBmBSw-ao4cX9MrzPuDv2N2Pi3eo,3308
+xia_fields-0.3.7.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_fields-0.3.7.dist-info/top_level.txt,sha256=pXvwXCVXR-n1PTScNVgqx5GAlG0H2tIpu7XuuswUrng,11
+xia_fields-0.3.7.dist-info/RECORD,,
```

