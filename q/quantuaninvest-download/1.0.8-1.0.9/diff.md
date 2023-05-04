# Comparing `tmp/quantuaninvest_download-1.0.8-py3-none-any.whl.zip` & `tmp/quantuaninvest_download-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 3247 bytes, number of entries: 7
+Zip file size: 3941 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-20 04:08 tool/__init__.py
 -rw-rw-rw-  2.0 fat     2248 b- defN 22-Nov-08 07:45 tool/download.py
 -rw-rw-rw-  2.0 fat     1752 b- defN 22-Nov-07 06:12 tool/get_data.py
--rw-rw-rw-  2.0 fat      242 b- defN 22-Nov-08 07:46 quantuaninvest_download-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Nov-08 07:46 quantuaninvest_download-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 22-Nov-08 07:46 quantuaninvest_download-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      576 b- defN 22-Nov-08 07:46 quantuaninvest_download-1.0.8.dist-info/RECORD
-7 files, 4915 bytes uncompressed, 2213 bytes compressed:  55.0%
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-10 07:15 tool/trade_functions/__init__.py
+-rw-rw-rw-  2.0 fat      787 b- defN 22-Nov-10 07:18 tool/trade_functions/position.py
+-rw-rw-rw-  2.0 fat      242 b- defN 22-Nov-10 07:19 quantuaninvest_download-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Nov-10 07:19 quantuaninvest_download-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 22-Nov-10 07:19 quantuaninvest_download-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      750 b- defN 22-Nov-10 07:19 quantuaninvest_download-1.0.9.dist-info/RECORD
+9 files, 5876 bytes uncompressed, 2627 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -3,20 +3,26 @@
 
 Filename: tool/download.py
 Comment: 
 
 Filename: tool/get_data.py
 Comment: 
 
-Filename: quantuaninvest_download-1.0.8.dist-info/METADATA
+Filename: tool/trade_functions/__init__.py
 Comment: 
 
-Filename: quantuaninvest_download-1.0.8.dist-info/WHEEL
+Filename: tool/trade_functions/position.py
 Comment: 
 
-Filename: quantuaninvest_download-1.0.8.dist-info/top_level.txt
+Filename: quantuaninvest_download-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: quantuaninvest_download-1.0.8.dist-info/RECORD
+Filename: quantuaninvest_download-1.0.9.dist-info/WHEEL
+Comment: 
+
+Filename: quantuaninvest_download-1.0.9.dist-info/top_level.txt
+Comment: 
+
+Filename: quantuaninvest_download-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `quantuaninvest_download-1.0.8.dist-info/RECORD` & `quantuaninvest_download-1.0.9.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
 tool/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tool/download.py,sha256=T3383wv_5Bv4TjzvEAFl2SwcuWA_cAM9hQGXe2QCvY8,2248
 tool/get_data.py,sha256=PQORXce2DCMUIoCJy4EpvZyM-hJIJG4KWWFNHWus5cA,1752
-quantuaninvest_download-1.0.8.dist-info/METADATA,sha256=wea_zYbSJ_sB1koT_y3mS3ME9FQZFIWjW5iUGOMxDr4,242
-quantuaninvest_download-1.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-quantuaninvest_download-1.0.8.dist-info/top_level.txt,sha256=Z5SN2a_Wr-UEOwAp1ap88PiygkuvFvTwl9QNgw7baG0,5
-quantuaninvest_download-1.0.8.dist-info/RECORD,,
+tool/trade_functions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tool/trade_functions/position.py,sha256=mumfqzDle87TtJtJdCkEbHKSORakX6gMxCuLBON2eI4,787
+quantuaninvest_download-1.0.9.dist-info/METADATA,sha256=ecNzHk-yWlELNsTbxlz3HciZq0SJn780ejYHzjStQ5w,242
+quantuaninvest_download-1.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+quantuaninvest_download-1.0.9.dist-info/top_level.txt,sha256=Z5SN2a_Wr-UEOwAp1ap88PiygkuvFvTwl9QNgw7baG0,5
+quantuaninvest_download-1.0.9.dist-info/RECORD,,
```

