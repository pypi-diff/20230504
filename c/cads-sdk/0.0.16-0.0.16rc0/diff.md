# Comparing `tmp/cads_sdk-0.0.16-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.16rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 55263 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-May-04 08:39 cads_sdk/__init__.py
+Zip file size: 55291 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     1268 b- defN 23-May-04 08:32 cads_sdk/__init__.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
 -rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
 -rw-rw-r--  2.0 unx    84386 b- defN 23-Apr-28 02:32 cads_sdk/nosql/converter.py
 -rw-rw-r--  2.0 unx    18788 b- defN 23-May-04 08:32 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
 -rw-rw-r--  2.0 unx      591 b- defN 23-Apr-09 13:11 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7126 b- defN 23-May-04 08:40 cads_sdk-0.0.16.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-04 08:40 cads_sdk-0.0.16.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-04 08:40 cads_sdk-0.0.16.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1479 b- defN 23-May-04 08:40 cads_sdk-0.0.16.dist-info/RECORD
-18 files, 274896 bytes uncompressed, 52857 bytes compressed:  80.8%
+-rw-rw-r--  2.0 unx     7129 b- defN 23-May-04 08:33 cads_sdk-0.0.16rc0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-04 08:33 cads_sdk-0.0.16rc0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-04 08:33 cads_sdk-0.0.16rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1491 b- defN 23-May-04 08:33 cads_sdk-0.0.16rc0.dist-info/RECORD
+18 files, 274914 bytes uncompressed, 52861 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.16.dist-info/METADATA
+Filename: cads_sdk-0.0.16rc0.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.16.dist-info/WHEEL
+Filename: cads_sdk-0.0.16rc0.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.16.dist-info/top_level.txt
+Filename: cads_sdk-0.0.16rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.16.dist-info/RECORD
+Filename: cads_sdk-0.0.16rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.16'
+__version__ = '0.0.16rc0'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## Comparing `cads_sdk-0.0.16.dist-info/METADATA` & `cads_sdk-0.0.16rc0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.16
+Version: 0.0.16rc0
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

## Comparing `cads_sdk-0.0.16.dist-info/RECORD` & `cads_sdk-0.0.16rc0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-cads_sdk/__init__.py,sha256=n9swgH74PFSUdagCm0R50BMamCTXBhjuJOSRr-D6SUM,1265
+cads_sdk/__init__.py,sha256=V8YJ3Nbiumdjlu_V5eyJuVSCL74q35XM_54kw8xSwHQ,1268
 cads_sdk/nosql/__init__.py,sha256=Yu2Zt5cpSXSLqIRAvIxaXOtoyj3yBisGTbnFlH4UD2A,1264
 cads_sdk/nosql/codec.py,sha256=Z0RdndLtSHAnqHOpDGE-Wb_jD9eIWvKiuX4Yj1KudX4,11231
 cads_sdk/nosql/converter.py,sha256=xpiAXwSVvJPaU_V3pMjdbCdEQFvWq1_Y1foR7YOg2sc,84386
 cads_sdk/nosql/display.py,sha256=xHwRIirQrpYsOuq4lQxgEPXa8LQTzc5GtnEbA_nSMnA,18788
 cads_sdk/nosql/etl.py,sha256=PWhXNWZyIFFEEvTIoUNuKK5cDqTy8A4FPn07BGMr0Vk,1187
 cads_sdk/nosql/utils.py,sha256=5y4Q5ydkesUteW_fqAc3ifwAlARvv9w58PWNyJz6iyA,591
 cads_sdk/petastorm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cads_sdk/petastorm/dataset_metadata.py,sha256=3sXVulFmpZEJC7mM0cwEXBVmB-0TD-U746ltLcsqIno,19967
 cads_sdk/petastorm/fs_utils.py,sha256=qFAzfi_VM4Rr2mBW8JsgxPUojLFFQGZI93MpI4sL_Xo,10508
 cads_sdk/petastorm/utils.py,sha256=CyeRPL_ih9wC1BdElvf1VknF1lBdNvJxgldSiU1OkFs,5427
 cads_sdk/pytorch/__init__.py,sha256=qyLEDZ_2BXLQBqievSj4wg2h4EQf9AdbIi_1SKFyIsM,22554
 cads_sdk/pytorch/codec.py,sha256=5XZulM21El-lsL3jZMexnJAHc2cIeRZj721PMuPhsJU,10653
 cads_sdk/pytorch/converter.py,sha256=lT2c3ix8Q35TEOUdFzlQVIzf7GfRklomwrdfRaXcY7k,78369
-cads_sdk-0.0.16.dist-info/METADATA,sha256=CM8yooVCPDZvXHDHEwTYddoPRcyeMLgFimXU8Rpme_Y,7126
-cads_sdk-0.0.16.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-cads_sdk-0.0.16.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
-cads_sdk-0.0.16.dist-info/RECORD,,
+cads_sdk-0.0.16rc0.dist-info/METADATA,sha256=dbTRcweyI9wLnZmGQft1_Kc19FjgNvePQbq7YRB5csc,7129
+cads_sdk-0.0.16rc0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+cads_sdk-0.0.16rc0.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
+cads_sdk-0.0.16rc0.dist-info/RECORD,,
```

