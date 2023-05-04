# Comparing `tmp/maxbot-0.1.0b1-py3-none-any.whl.zip` & `tmp/maxbot-0.1.0b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -39,13 +39,13 @@
 -rw-r--r--  2.0 unx    10833 b- defN 80-Jan-01 00:00 maxbot/resources.py
 -rw-r--r--  2.0 unx     4728 b- defN 80-Jan-01 00:00 maxbot/rpc.py
 -rw-r--r--  2.0 unx     8844 b- defN 80-Jan-01 00:00 maxbot/scenarios.py
 -rw-r--r--  2.0 unx    16929 b- defN 80-Jan-01 00:00 maxbot/schemas.py
 -rw-r--r--  2.0 unx     4164 b- defN 80-Jan-01 00:00 maxbot/state_store.py
 -rw-r--r--  2.0 unx     1051 b- defN 80-Jan-01 00:00 maxbot/user_locks.py
 -rw-r--r--  2.0 unx    14851 b- defN 80-Jan-01 00:00 maxbot/xml.py
--rw-r--r--  2.0 unx     1055 b- defN 80-Jan-01 00:00 maxbot-0.1.0b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7688 b- defN 80-Jan-01 00:00 maxbot-0.1.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 maxbot-0.1.0b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 maxbot-0.1.0b1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     3851 b- defN 16-Jan-01 00:00 maxbot-0.1.0b1.dist-info/RECORD
+-rw-r--r--  2.0 unx     1055 b- defN 80-Jan-01 00:00 maxbot-0.1.0b2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7688 b- defN 80-Jan-01 00:00 maxbot-0.1.0b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 maxbot-0.1.0b2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 maxbot-0.1.0b2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     3851 b- defN 16-Jan-01 00:00 maxbot-0.1.0b2.dist-info/RECORD
 49 files, 301499 bytes uncompressed, 85371 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -126,23 +126,23 @@
 
 Filename: maxbot/user_locks.py
 Comment: 
 
 Filename: maxbot/xml.py
 Comment: 
 
-Filename: maxbot-0.1.0b1.dist-info/LICENSE
+Filename: maxbot-0.1.0b2.dist-info/LICENSE
 Comment: 
 
-Filename: maxbot-0.1.0b1.dist-info/METADATA
+Filename: maxbot-0.1.0b2.dist-info/METADATA
 Comment: 
 
-Filename: maxbot-0.1.0b1.dist-info/WHEEL
+Filename: maxbot-0.1.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: maxbot-0.1.0b1.dist-info/entry_points.txt
+Filename: maxbot-0.1.0b2.dist-info/entry_points.txt
 Comment: 
 
-Filename: maxbot-0.1.0b1.dist-info/RECORD
+Filename: maxbot-0.1.0b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `maxbot-0.1.0b1.dist-info/LICENSE` & `maxbot-0.1.0b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `maxbot-0.1.0b1.dist-info/METADATA` & `maxbot-0.1.0b2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxbot
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Maxbot is an open source library and framework for creating conversational apps.
 Home-page: https://maxbot.ai
 License: MIT
 Keywords: maxbot,conversational-apps,nlp,conversational-ai,bot,chatbot,text-bot,voice-bot,botkit,chatbot-framework
 Author: Maxbot team
 Author-email: hello@maxbot.ai
 Maintainer: Maxbot team
```

## Comparing `maxbot-0.1.0b1.dist-info/RECORD` & `maxbot-0.1.0b2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 maxbot/resources.py,sha256=k_Z86NjC-ha3QSMgaMWeKmQ4SrQl8fVoOfJHOFxlYfo,10833
 maxbot/rpc.py,sha256=Ph8SeI7aTTIV0MpvLVurz2AYkq5xrJS-q1gjqNalqUs,4728
 maxbot/scenarios.py,sha256=rb4etJUcoN9LOU7jn8_ZetOHGiRpBtkOeusBW81Hy1c,8844
 maxbot/schemas.py,sha256=374wYhTWUdVvE1Od45bz9cmk6wLP_IRGjd93YU0uacc,16929
 maxbot/state_store.py,sha256=yaPLekUo4czgMSTGBkSRi_IjolIvSp2urwKj51sS5pY,4164
 maxbot/user_locks.py,sha256=_FnI_G4sPwjTaXiEw7Sj9tkiV_UGmhgF-F8H4vFudBA,1051
 maxbot/xml.py,sha256=R6RmyotAI43CEPINyUNI-sFHdNciz0YzboezA3QIZgA,14851
-maxbot-0.1.0b1.dist-info/LICENSE,sha256=g6TcBHQ6jwWbD2xQGQYGtK0pvcb4G2gx0f8B7QschKI,1055
-maxbot-0.1.0b1.dist-info/METADATA,sha256=O2fzsUI8kdt6yjH3YJuRYvDQhZULbaL7laGlr2eFvMA,7688
-maxbot-0.1.0b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-maxbot-0.1.0b1.dist-info/entry_points.txt,sha256=BORdoo0s_bCrrWHTB-b4Sykb1KPIErzt7c-Oc0Uu4zw,42
-maxbot-0.1.0b1.dist-info/RECORD,,
+maxbot-0.1.0b2.dist-info/LICENSE,sha256=g6TcBHQ6jwWbD2xQGQYGtK0pvcb4G2gx0f8B7QschKI,1055
+maxbot-0.1.0b2.dist-info/METADATA,sha256=nwAfJq4193g1yj7pnuBTc4Aaj5jGBUw541d0PmG7t00,7688
+maxbot-0.1.0b2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+maxbot-0.1.0b2.dist-info/entry_points.txt,sha256=BORdoo0s_bCrrWHTB-b4Sykb1KPIErzt7c-Oc0Uu4zw,42
+maxbot-0.1.0b2.dist-info/RECORD,,
```

