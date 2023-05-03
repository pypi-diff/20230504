# Comparing `tmp/simple_othello-1.2.4-py3-none-any.whl.zip` & `tmp/simple_othello-1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6463 bytes, number of entries: 13
--rw-r--r--  2.0 unx       66 b- defN 23-Feb-23 14:27 simple_othello/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Feb-23 14:27 simple_othello/agent.py
--rw-r--r--  2.0 unx      148 b- defN 23-Feb-23 14:27 simple_othello/config.py
--rw-r--r--  2.0 unx      236 b- defN 23-Feb-23 14:27 simple_othello/env.py
--rw-r--r--  2.0 unx      692 b- defN 23-Feb-23 14:27 simple_othello/humanPlayer.py
--rw-r--r--  2.0 unx      866 b- defN 23-Feb-23 14:27 simple_othello/main.py
--rw-r--r--  2.0 unx     4774 b- defN 23-Feb-23 14:27 simple_othello/othello.py
--rw-r--r--  2.0 unx      588 b- defN 23-Feb-23 14:27 simple_othello/randomPlayer.py
--rw-r--r--  2.0 unx     1075 b- defN 23-Feb-23 14:27 simple_othello-1.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      786 b- defN 23-Feb-23 14:27 simple_othello-1.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-23 14:27 simple_othello-1.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Feb-23 14:27 simple_othello-1.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1068 b- defN 23-Feb-23 14:27 simple_othello-1.2.4.dist-info/RECORD
-13 files, 10555 bytes uncompressed, 4665 bytes compressed:  55.8%
+Zip file size: 6456 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       66 b- defN 23-May-03 23:25 simple_othello/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-May-03 23:25 simple_othello/agent.py
+-rw-r--r--  2.0 unx      148 b- defN 23-May-03 23:25 simple_othello/config.py
+-rw-r--r--  2.0 unx      236 b- defN 23-May-03 23:25 simple_othello/env.py
+-rw-r--r--  2.0 unx      692 b- defN 23-May-03 23:25 simple_othello/humanPlayer.py
+-rw-r--r--  2.0 unx      866 b- defN 23-May-03 23:25 simple_othello/main.py
+-rw-r--r--  2.0 unx     4807 b- defN 23-May-03 23:25 simple_othello/othello.py
+-rw-r--r--  2.0 unx      588 b- defN 23-May-03 23:25 simple_othello/randomPlayer.py
+-rw-r--r--  2.0 unx     1075 b- defN 23-May-03 23:25 simple_othello-1.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      765 b- defN 23-May-03 23:25 simple_othello-1.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 23:25 simple_othello-1.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-03 23:25 simple_othello-1.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1068 b- defN 23-May-03 23:25 simple_othello-1.2.5.dist-info/RECORD
+13 files, 10567 bytes uncompressed, 4658 bytes compressed:  55.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: simple_othello/othello.py
 Comment: 
 
 Filename: simple_othello/randomPlayer.py
 Comment: 
 
-Filename: simple_othello-1.2.4.dist-info/LICENSE
+Filename: simple_othello-1.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: simple_othello-1.2.4.dist-info/METADATA
+Filename: simple_othello-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: simple_othello-1.2.4.dist-info/WHEEL
+Filename: simple_othello-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: simple_othello-1.2.4.dist-info/top_level.txt
+Filename: simple_othello-1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_othello-1.2.4.dist-info/RECORD
+Filename: simple_othello-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_othello/othello.py

```diff
@@ -82,14 +82,15 @@
 class Othello:
     def __init__(self, CFG):
         self.CFG = CFG
         self.player = None
         self.state = None
         self.lines = 8  # 8x8 size board
         self.pass_player = {}
+        self.width = self.lines
 
     def reset(self):
         self.state = [[0 for _ in range(8)] for _ in range(8)]
         self.state[3][3] = 1  # second_player
         self.state[4][4] = 1
         self.state[3][4] = -1  # first_player
         self.state[4][3] = -1
```

## Comparing `simple_othello-1.2.4.dist-info/LICENSE` & `simple_othello-1.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simple_othello-1.2.4.dist-info/METADATA` & `simple_othello-1.2.5.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: simple-othello
-Version: 1.2.4
+Version: 1.2.5
 Summary: simple_othello
-Home-page: UNKNOWN
 Author: Michiyasu Uchiyama
 License: MIT
 Keywords: simple_othello othello reversi
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
@@ -15,9 +14,7 @@
 # simple_othello
 
 Udemyの教材で利用するためのオセロゲームプラットフォームです。<br>
 AlphaZeroの意外な構造　またはAlphaGoは如何にして棋譜データの利用を止めて自分の経験に頼るようになったか<br>
 https://www.udemy.com/course/alphazero/
 <br>
 ![readme](https://user-images.githubusercontent.com/26673104/215309416-cd0e5c9d-720d-410d-9384-21f63f35cfc1.png)
-
-
```

## Comparing `simple_othello-1.2.4.dist-info/RECORD` & `simple_othello-1.2.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 simple_othello/__init__.py,sha256=Dn8e9mF1S6xvU4b99akKq0oNQEPTBLfJk9R-GjYTIPM,66
 simple_othello/agent.py,sha256=WlEdOU7GCC3lHNOpolTiOOmKpEAUKf0lIoQawXM9s-c,149
 simple_othello/config.py,sha256=bUw5fEwHec5lRtPL6n27ytzRxp45IYEPGob-5Mkv9L8,148
 simple_othello/env.py,sha256=_LJzwbsrcipRvOkt4EwlpLRPJYJ0Usp6fGmOZGzkQF8,236
 simple_othello/humanPlayer.py,sha256=eoUuhRXgJI9xx69iZfWkghNeuofDMOHFfVrEzLzCCDA,692
 simple_othello/main.py,sha256=CP8uqF5G95SEKIibPFTkOxm7QuSOoqUT5YiZya-4uas,866
-simple_othello/othello.py,sha256=UjHVvbgAhcuyeASFaEI-WW-6xI_e03uiPj2_Pkdo8WY,4774
+simple_othello/othello.py,sha256=bkK7zmnzX9zg9G1eiCvE9D8ddkwjjcerW5M9HnpURA0,4807
 simple_othello/randomPlayer.py,sha256=o3I9Gj24IUM2fZA6DrNpmqTqRBS_h26WmsYAPWZdQjs,588
-simple_othello-1.2.4.dist-info/LICENSE,sha256=eULrrl2cQwqcVbHoSCQHVpYc3ArgsJveeUv2mcttjP4,1075
-simple_othello-1.2.4.dist-info/METADATA,sha256=TfY0FqfdGUyfLnUMp-ZdjVHIdl4GSsFL4dC68tqDCGo,786
-simple_othello-1.2.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-simple_othello-1.2.4.dist-info/top_level.txt,sha256=UJN6YunFaId75F3IYsJ7lfJvH0RJO0ua6ZBnopcCO2k,15
-simple_othello-1.2.4.dist-info/RECORD,,
+simple_othello-1.2.5.dist-info/LICENSE,sha256=eULrrl2cQwqcVbHoSCQHVpYc3ArgsJveeUv2mcttjP4,1075
+simple_othello-1.2.5.dist-info/METADATA,sha256=Ox04frvHU-hit1ZKED_cNusqvBZHb3NmXhc3LXlNNcE,765
+simple_othello-1.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+simple_othello-1.2.5.dist-info/top_level.txt,sha256=UJN6YunFaId75F3IYsJ7lfJvH0RJO0ua6ZBnopcCO2k,15
+simple_othello-1.2.5.dist-info/RECORD,,
```

