# Comparing `tmp/zwtk-1.0.1-py3-none-any.whl.zip` & `tmp/zwtk-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 16395 bytes, number of entries: 19
+Zip file size: 21220 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat        0 b- defN 20-Jul-16 08:16 zwtk/__init__.py
--rw-rw-rw-  2.0 fat      286 b- defN 23-May-03 04:30 zwtk/__version__.py
+-rw-rw-rw-  2.0 fat      286 b- defN 23-May-04 00:49 zwtk/__version__.py
 -rw-rw-rw-  2.0 fat     1159 b- defN 23-May-02 02:51 zwtk/comm.py
 -rw-rw-rw-  2.0 fat     1453 b- defN 23-Feb-08 05:36 zwtk/config.py
 -rw-rw-rw-  2.0 fat     9392 b- defN 23-Feb-15 13:39 zwtk/dlso.py
 -rw-rw-rw-  2.0 fat     7478 b- defN 23-May-03 04:18 zwtk/fileutils.py
 -rw-rw-rw-  2.0 fat     1728 b- defN 23-May-02 11:44 zwtk/geoutils.py
 -rw-rw-rw-  2.0 fat      897 b- defN 23-May-03 04:20 zwtk/mprocessing.py
 -rw-rw-rw-  2.0 fat     2269 b- defN 21-Jul-27 09:50 zwtk/mthreading.py
 -rw-rw-rw-  2.0 fat      815 b- defN 23-May-03 04:29 zwtk/osutils.py
 -rw-rw-rw-  2.0 fat      261 b- defN 22-Mar-22 06:05 zwtk/rand.py
 -rw-rw-rw-  2.0 fat     1217 b- defN 23-May-02 11:44 zwtk/reutils.py
 -rw-rw-rw-  2.0 fat     4850 b- defN 22-May-23 04:27 zwtk/textutils.py
 -rw-rw-rw-  2.0 fat     6638 b- defN 23-Feb-08 05:36 zwtk/urlutils.py
--rw-rw-rw-  2.0 fat     1068 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      527 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1378 b- defN 23-May-03 04:30 zwtk-1.0.1.dist-info/RECORD
-19 files, 41513 bytes uncompressed, 14205 bytes compressed:  65.8%
+-rw-rw-rw-  2.0 fat    21001 b- defN 23-May-04 00:38 zwtk/zwsqlite.py
+-rw-rw-rw-  2.0 fat     1068 b- defN 23-May-04 00:49 zwtk-1.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      527 b- defN 23-May-04 00:49 zwtk-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 00:49 zwtk-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-04 00:49 zwtk-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1452 b- defN 23-May-04 00:49 zwtk-1.0.2.dist-info/RECORD
+20 files, 62588 bytes uncompressed, 18922 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -36,23 +36,26 @@
 
 Filename: zwtk/textutils.py
 Comment: 
 
 Filename: zwtk/urlutils.py
 Comment: 
 
-Filename: zwtk-1.0.1.dist-info/LICENSE
+Filename: zwtk/zwsqlite.py
 Comment: 
 
-Filename: zwtk-1.0.1.dist-info/METADATA
+Filename: zwtk-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: zwtk-1.0.1.dist-info/WHEEL
+Filename: zwtk-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: zwtk-1.0.1.dist-info/top_level.txt
+Filename: zwtk-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: zwtk-1.0.1.dist-info/RECORD
+Filename: zwtk-1.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: zwtk-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zwtk/__version__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 __title__ = 'zwtk'
 __description__ = 'Personal Python Utilities'
 __url__ = 'https://github.com/njzhaowei/zwtk'
 __author__ = 'Zhao Wei'
 __author_email__ = 'yewberry@163.com'
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2023 Zhao Wei. All rights reserved.'
```

## Comparing `zwtk-1.0.1.dist-info/LICENSE` & `zwtk-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zwtk-1.0.1.dist-info/RECORD` & `zwtk-1.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 zwtk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-zwtk/__version__.py,sha256=xosNaqiDX_35hEBr8wJ1-ARhVHh6CheDxnaWC6WJeQo,286
+zwtk/__version__.py,sha256=5gudhOG2beVv1klr9ree-tKJs1U9c426P9r5DWNuXyg,286
 zwtk/comm.py,sha256=OycFwe4kcxvSESh0EHsjuG6raipj_rfXqOn8-YpmGh8,1159
 zwtk/config.py,sha256=lFeXOV4SNoiofGN48ssAATA5yal_hWbE5xUd-AZNdyI,1453
 zwtk/dlso.py,sha256=ZP70mx88H6hMJxBlLxhFjU4cuyTc_QFyj-vZlJcKFoI,9392
 zwtk/fileutils.py,sha256=pBPFJg_hc6noGACbTQoEpWnic0i-rpTrqdyea0q5rvk,7478
 zwtk/geoutils.py,sha256=8ve3fz_7zgjNgcLLKC4DTxob9mmJLNsr4-i-U2amaCs,1728
 zwtk/mprocessing.py,sha256=-5IGrK87WKCgjp9-cqcu2cOL8_pOQRWPYdTf1gq1jec,897
 zwtk/mthreading.py,sha256=YDzai3v9Ne8NglFY4RvI-mDsMwgk1t-IxJx_YFwA9MA,2269
 zwtk/osutils.py,sha256=R62uDBTw_kQhQgkxG8V2Bu-OvX65418HrleM7Bgx24s,815
 zwtk/rand.py,sha256=NF97IN2QAcd5azH1I0CbdEAvou4QeCK510-zjvrawGo,261
 zwtk/reutils.py,sha256=fjw6A_MGI2EY10TuiEat4wpG6DfpwQVRbFFu0GmgDME,1217
 zwtk/textutils.py,sha256=ua6uxxB-wsIqRZHrdHbz7F391utpUHvzfF0pkHITPIw,4850
 zwtk/urlutils.py,sha256=TgXKbJhrSFMJAOd9K7c91L4LC1obzbfHdhnoehi1st8,6638
-zwtk-1.0.1.dist-info/LICENSE,sha256=u-k3pdS046rxrlusCu-PdSHHdF5pgn1GgR1IU0CfoyI,1068
-zwtk-1.0.1.dist-info/METADATA,sha256=lgP3itQW9Aq_DSgWtbKCUQ5TkHCFlQoY3PQBXx6OQYQ,527
-zwtk-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-zwtk-1.0.1.dist-info/top_level.txt,sha256=sZshqvNUx_xBkWVO93H3Nu-ACwaM6HhRtvErJtzxUTQ,5
-zwtk-1.0.1.dist-info/RECORD,,
+zwtk/zwsqlite.py,sha256=UxdPEhXPnvQFB7d0Tu4aHc39Bi8yTSxKpDPjya3WcB0,21001
+zwtk-1.0.2.dist-info/LICENSE,sha256=u-k3pdS046rxrlusCu-PdSHHdF5pgn1GgR1IU0CfoyI,1068
+zwtk-1.0.2.dist-info/METADATA,sha256=38a9iS_hR3svmWXUlcymAPsFbOClK8aRBz5ldu6qkgQ,527
+zwtk-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+zwtk-1.0.2.dist-info/top_level.txt,sha256=sZshqvNUx_xBkWVO93H3Nu-ACwaM6HhRtvErJtzxUTQ,5
+zwtk-1.0.2.dist-info/RECORD,,
```

