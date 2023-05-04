# Comparing `tmp/vtda-1.5.1-py3-none-any.whl.zip` & `tmp/vtda-1.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,29 @@
-Zip file size: 53589 bytes, number of entries: 26
--rw-rw-rw-  2.0 fat     2683 b- defN 23-Feb-11 15:15 vtda/__init__.py
+Zip file size: 55262 bytes, number of entries: 27
+-rw-rw-rw-  2.0 fat     2829 b- defN 23-May-04 08:32 vtda/__init__.py
 -rw-rw-rw-  2.0 fat     2020 b- defN 21-Dec-30 15:14 vtda/analysis/__init__.py
 -rw-rw-rw-  2.0 fat    29599 b- defN 22-Jul-04 09:45 vtda/analysis/base.py
 -rw-rw-rw-  2.0 fat    11168 b- defN 21-Jun-26 16:24 vtda/analysis/batch_calculate.py
 -rw-rw-rw-  2.0 fat    18504 b- defN 21-Nov-23 08:14 vtda/analysis/noise.py
 -rw-rw-rw-  2.0 fat    17769 b- defN 22-Jul-04 10:09 vtda/analysis/sperling.py
 -rw-rw-rw-  2.0 fat      876 b- defN 21-Nov-25 16:44 vtda/analysis/untitled1.py
 -rw-rw-rw-  2.0 fat    46938 b- defN 21-Dec-11 14:26 vtda/analysis/vehicle_dynamics.py
 -rw-rw-rw-  2.0 fat    33507 b- defN 21-Dec-30 15:10 vtda/analysis/vibration.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Nov-14 13:16 vtda/demo/__init__.py
 -rw-rw-rw-  2.0 fat     6396 b- defN 21-Nov-25 11:54 vtda/demo/algo.py
 -rw-rw-rw-  2.0 fat      100 b- defN 21-Nov-14 13:16 vtda/demo/demo_dxp_to_dasp.py
 -rw-rw-rw-  2.0 fat     1417 b- defN 21-Nov-16 15:23 vtda/demo/demo_sperling.py
 -rw-rw-rw-  2.0 fat     5779 b- defN 22-Apr-06 09:34 vtda/demo/demo_vibration_noise.py
 -rw-rw-rw-  2.0 fat      313 b- defN 21-Jun-12 08:28 vtda/read_data/__init__.py
+-rw-rw-rw-  2.0 fat     4133 b- defN 23-May-04 08:32 vtda/read_data/read_dasc.py
 -rw-rw-rw-  2.0 fat     9562 b- defN 22-Aug-14 11:25 vtda/read_data/read_dasp.py
 -rw-rw-rw-  2.0 fat     8813 b- defN 21-Nov-28 16:18 vtda/read_data/read_dxd.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Nov-14 13:16 vtda/test/__init__.py
 -rw-rw-rw-  2.0 fat     3043 b- defN 21-Jun-27 03:15 vtda/test/find_start_and_end.py
 -rw-rw-rw-  2.0 fat     2179 b- defN 21-Jun-14 14:47 vtda/test/test.py
 -rw-rw-rw-  2.0 fat      362 b- defN 21-Nov-11 12:14 vtda/util/__init__.py
 -rw-rw-rw-  2.0 fat    10650 b- defN 23-Feb-11 15:27 vtda/util/util.py
--rw-rw-rw-  2.0 fat      285 b- defN 23-Apr-23 02:47 vtda-1.5.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-23 02:47 vtda-1.5.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-23 02:47 vtda-1.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2073 b- defN 23-Apr-23 02:47 vtda-1.5.1.dist-info/RECORD
-26 files, 214138 bytes uncompressed, 50283 bytes compressed:  76.5%
+-rw-rw-rw-  2.0 fat      285 b- defN 23-May-04 08:32 vtda-1.5.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-May-04 08:32 vtda-1.5.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-04 08:32 vtda-1.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2157 b- defN 23-May-04 08:32 vtda-1.5.2.dist-info/RECORD
+27 files, 218501 bytes uncompressed, 51826 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -39,14 +39,17 @@
 
 Filename: vtda/demo/demo_vibration_noise.py
 Comment: 
 
 Filename: vtda/read_data/__init__.py
 Comment: 
 
+Filename: vtda/read_data/read_dasc.py
+Comment: 
+
 Filename: vtda/read_data/read_dasp.py
 Comment: 
 
 Filename: vtda/read_data/read_dxd.py
 Comment: 
 
 Filename: vtda/test/__init__.py
@@ -60,20 +63,20 @@
 
 Filename: vtda/util/__init__.py
 Comment: 
 
 Filename: vtda/util/util.py
 Comment: 
 
-Filename: vtda-1.5.1.dist-info/METADATA
+Filename: vtda-1.5.2.dist-info/METADATA
 Comment: 
 
-Filename: vtda-1.5.1.dist-info/WHEEL
+Filename: vtda-1.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: vtda-1.5.1.dist-info/top_level.txt
+Filename: vtda-1.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: vtda-1.5.1.dist-info/RECORD
+Filename: vtda-1.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vtda/__init__.py

```diff
@@ -1,23 +1,25 @@
 ﻿"""
 vtda
 Vibration Test Data Analysis
 """
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 __author__ = 'zhangshenglong'
 
 '''
 read_data
 '''
 from vtda.read_data.read_dasp import (
                                                read_dasp_data_single,
                                                read_dasp_data
                                             )
-
+from vtda.read_data.read_dasc import (
+                                               read_dasc_data
+                                            )
 
 from vtda.analysis.vibration import (                                                    
                                                 vibration_level,
                                                 frequency_vibration_level,
                                                 batch_vibration_level,
                                                 batch_frequency_vibration_level,
                                                 batch_octave_3,
```

## Comparing `vtda-1.5.1.dist-info/RECORD` & `vtda-1.5.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-vtda/__init__.py,sha256=MzCG3dCH8VRKTE079cUkL1G2QrdTJkhXGl5jNZ7XGtw,2683
+vtda/__init__.py,sha256=5KfBQItAKoinhfsFJlIa_ifhlo8AAyyCwNipsl5a2q4,2829
 vtda/analysis/__init__.py,sha256=zRVrAQv1k1Lq-aB4Wn04JyxmfjKLNA3bWQ75ExOSj3k,2020
 vtda/analysis/base.py,sha256=XSSvKP7ZChMKLc4hN8FWR2u-7Je1X0VcFN4o-8F2aPg,29599
 vtda/analysis/batch_calculate.py,sha256=BkCpaX1w6t9s9VGQy4QUWMJZbNrTJ7P9zYmrrQWgo-c,11168
 vtda/analysis/noise.py,sha256=5wIs3ZhWEHMEVTxqE7T3qgwHN2EvGsxfQCQajt9egXw,18504
 vtda/analysis/sperling.py,sha256=JwtBFQGyQ0OQPiJr34x7NYagfONVfFSA2JBsEj4rQ5M,17769
 vtda/analysis/untitled1.py,sha256=5-0Toujm65I0Eneie-8n-T2jOtbdWRNH18G7iI8ZGYI,876
 vtda/analysis/vehicle_dynamics.py,sha256=Xb8zl250jsbXi5t5XIGyRygogxBiEuum2TtokI6Nwjo,46938
 vtda/analysis/vibration.py,sha256=SZQWPGTqz_J_snceMzIYDt8MZKlpymRjwWOJN3nHV7s,33507
 vtda/demo/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vtda/demo/algo.py,sha256=CAMNv0sMmBTirhB8vQPv7ZIm-ZVcU6b7ZbjL2Q9gk4U,6396
 vtda/demo/demo_dxp_to_dasp.py,sha256=rKDvLYeOt93gbxAKfdib82f8xd2DyjH3OyzgVHqEjAU,100
 vtda/demo/demo_sperling.py,sha256=kzkwyRxnhQWMiygTKS6lfUNdweMybWwZIVX-3IT4zfo,1417
 vtda/demo/demo_vibration_noise.py,sha256=zs26UDey4j1fSQe8GNUHdHAwScdPIGlDy66JNzeOFUY,5779
 vtda/read_data/__init__.py,sha256=kWepW0h7WzFhQN90NpHY5kHPFM5QH8411cx284Outho,313
+vtda/read_data/read_dasc.py,sha256=bSz12iMvGRZbJFYplT7kcnI28IhXrj8H5QChMQPUg7U,4133
 vtda/read_data/read_dasp.py,sha256=nIpZ8UtzzxkvRE-rpl6dntNROLex8aZDKOyQPipDFcM,9562
 vtda/read_data/read_dxd.py,sha256=m3jX0YbbIElU3OSBq2ObXnl6cULHXbLp378knC8a-4w,8813
 vtda/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vtda/test/find_start_and_end.py,sha256=4_KG4ny2rINEo-j9GdWVu1OWtdGCzZNXAZsnv1jCpFg,3043
 vtda/test/test.py,sha256=OsyeOy8n6qaILK81wlGsut4k45EXHlNfB48gSly8JAs,2179
 vtda/util/__init__.py,sha256=giJ_UE71YWyBIc9aKW934Otilcdsy_FayKvMOaYpuDg,362
 vtda/util/util.py,sha256=PZJGYSFOIiSQnCB75z0LkU_AbYp7n-snzuaIUuUwdxI,10650
-vtda-1.5.1.dist-info/METADATA,sha256=A48QYZtAFsc6ejubadrYH_Bulfqk-c4stG01nV59tNo,285
-vtda-1.5.1.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-vtda-1.5.1.dist-info/top_level.txt,sha256=DnhjMA74wO4kU53vr91eo3C0r-6Od0RMXgWT6JreCq4,5
-vtda-1.5.1.dist-info/RECORD,,
+vtda-1.5.2.dist-info/METADATA,sha256=P1ypsjA2seoytJyOfiozo5RKyYUfWL-t5rFxBVsLmlM,285
+vtda-1.5.2.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+vtda-1.5.2.dist-info/top_level.txt,sha256=DnhjMA74wO4kU53vr91eo3C0r-6Od0RMXgWT6JreCq4,5
+vtda-1.5.2.dist-info/RECORD,,
```

