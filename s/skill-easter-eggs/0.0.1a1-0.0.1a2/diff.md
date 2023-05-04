# Comparing `tmp/skill-easter-eggs-0.0.1a1.tar.gz` & `tmp/skill-easter-eggs-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skill-easter-eggs-0.0.1a1.tar", last modified: Thu May  4 04:05:24 2023, max compression
+gzip compressed data, was "skill-easter-eggs-0.0.1a2.tar", last modified: Thu May  4 04:22:02 2023, max compression
```

## Comparing `skill-easter-eggs-0.0.1a1.tar` & `skill-easter-eggs-0.0.1a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-04 04:05:24.204865 skill-easter-eggs-0.0.1a1/
--rw-r--r--   0 Mike       (501) staff       (20)     1497 2023-05-04 03:00:00.000000 skill-easter-eggs-0.0.1a1/LICENSE
--rw-r--r--   0 Mike       (501) staff       (20)     1386 2023-05-04 04:05:24.204706 skill-easter-eggs-0.0.1a1/PKG-INFO
--rw-r--r--   0 Mike       (501) staff       (20)     1089 2023-05-04 02:48:31.000000 skill-easter-eggs-0.0.1a1/README.md
--rw-r--r--   0 Mike       (501) staff       (20)     6025 2023-05-04 04:05:00.000000 skill-easter-eggs-0.0.1a1/__init__.py
--rw-r--r--   0 Mike       (501) staff       (20)       38 2023-05-04 04:05:24.204924 skill-easter-eggs-0.0.1a1/setup.cfg
--rw-r--r--   0 Mike       (501) staff       (20)     3951 2023-05-04 04:03:16.000000 skill-easter-eggs-0.0.1a1/setup.py
-drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-04 04:05:24.204496 skill-easter-eggs-0.0.1a1/skill_easter_eggs.egg-info/
--rw-r--r--   0 Mike       (501) staff       (20)     1386 2023-05-04 04:05:24.000000 skill-easter-eggs-0.0.1a1/skill_easter_eggs.egg-info/PKG-INFO
--rw-r--r--   0 Mike       (501) staff       (20)      269 2023-05-04 04:05:24.000000 skill-easter-eggs-0.0.1a1/skill_easter_eggs.egg-info/SOURCES.txt
--rw-r--r--   0 Mike       (501) staff       (20)        1 2023-05-04 04:05:24.000000 skill-easter-eggs-0.0.1a1/skill_easter_eggs.egg-info/dependency_links.txt
--rw-r--r--   0 Mike       (501) staff       (20)       85 2023-05-04 04:05:24.000000 skill-easter-eggs-0.0.1a1/skill_easter_eggs.egg-info/entry_points.txt
--rw-r--r--   0 Mike       (501) staff       (20)       18 2023-05-04 04:05:24.000000 skill-easter-eggs-0.0.1a1/skill_easter_eggs.egg-info/top_level.txt
--rw-r--r--   0 Mike       (501) staff       (20)    10981 2023-05-04 03:42:39.000000 skill-easter-eggs-0.0.1a1/stardate.py
--rw-r--r--   0 Mike       (501) staff       (20)       24 2023-05-04 04:03:07.000000 skill-easter-eggs-0.0.1a1/version.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-04 04:22:02.624678 skill-easter-eggs-0.0.1a2/
+-rw-r--r--   0 Mike       (501) staff       (20)     1497 2023-05-04 03:00:00.000000 skill-easter-eggs-0.0.1a2/LICENSE
+-rw-r--r--   0 Mike       (501) staff       (20)     1386 2023-05-04 04:22:02.624519 skill-easter-eggs-0.0.1a2/PKG-INFO
+-rw-r--r--   0 Mike       (501) staff       (20)     1089 2023-05-04 02:48:31.000000 skill-easter-eggs-0.0.1a2/README.md
+-rw-r--r--   0 Mike       (501) staff       (20)     6020 2023-05-04 04:21:22.000000 skill-easter-eggs-0.0.1a2/__init__.py
+-rw-r--r--   0 Mike       (501) staff       (20)       38 2023-05-04 04:22:02.624745 skill-easter-eggs-0.0.1a2/setup.cfg
+-rw-r--r--   0 Mike       (501) staff       (20)     3951 2023-05-04 04:03:16.000000 skill-easter-eggs-0.0.1a2/setup.py
+drwxr-xr-x   0 Mike       (501) staff       (20)        0 2023-05-04 04:22:02.624122 skill-easter-eggs-0.0.1a2/skill_easter_eggs.egg-info/
+-rw-r--r--   0 Mike       (501) staff       (20)     1386 2023-05-04 04:22:02.000000 skill-easter-eggs-0.0.1a2/skill_easter_eggs.egg-info/PKG-INFO
+-rw-r--r--   0 Mike       (501) staff       (20)      269 2023-05-04 04:22:02.000000 skill-easter-eggs-0.0.1a2/skill_easter_eggs.egg-info/SOURCES.txt
+-rw-r--r--   0 Mike       (501) staff       (20)        1 2023-05-04 04:22:02.000000 skill-easter-eggs-0.0.1a2/skill_easter_eggs.egg-info/dependency_links.txt
+-rw-r--r--   0 Mike       (501) staff       (20)       85 2023-05-04 04:22:02.000000 skill-easter-eggs-0.0.1a2/skill_easter_eggs.egg-info/entry_points.txt
+-rw-r--r--   0 Mike       (501) staff       (20)       18 2023-05-04 04:22:02.000000 skill-easter-eggs-0.0.1a2/skill_easter_eggs.egg-info/top_level.txt
+-rw-r--r--   0 Mike       (501) staff       (20)    10981 2023-05-04 03:42:39.000000 skill-easter-eggs-0.0.1a2/stardate.py
+-rw-r--r--   0 Mike       (501) staff       (20)       24 2023-05-04 04:21:57.000000 skill-easter-eggs-0.0.1a2/version.py
```

### Comparing `skill-easter-eggs-0.0.1a1/LICENSE` & `skill-easter-eggs-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `skill-easter-eggs-0.0.1a1/PKG-INFO` & `skill-easter-eggs-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skill-easter-eggs
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: UNKNOWN
 Home-page: https://github.com/OpenVoiceOS/skill-easter-eggs
 Author: Jarbas
 Author-email: jarbas@openvoiceos.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skill-easter-eggs Version: 0.0.1a1 Summary: UNKNOWN
+Metadata-Version: 2.1 Name: skill-easter-eggs Version: 0.0.1a2 Summary: UNKNOWN
 Home-page: https://github.com/OpenVoiceOS/skill-easter-eggs Author: Jarbas
 Author-email: jarbas@openvoiceos.com License: BSD-3-Clause Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE ## Easter Eggs [!
 [Donate with Bitcoin](https://en.cryptobadges.io/badge/micro/
 1QJNhKM8tVv62XSUrST2vnaMXh5ADSyYP8)](https://en.cryptobadges.io/donate/
 1QJNhKM8tVv62XSUrST2vnaMXh5ADSyYP8) [![Donate](https://img.shields.io/badge/
 Donate-PayPal-green.svg)](https://paypal.me/jarbasai) [Patreon_donate_button]
```

### Comparing `skill-easter-eggs-0.0.1a1/README.md` & `skill-easter-eggs-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `skill-easter-eggs-0.0.1a1/__init__.py` & `skill-easter-eggs-0.0.1a2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 __author__ = "jarbas"
 
 
 class EasterEggsSkill(OVOSSkill):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.audio_service = AudioService(self.bus)
 
     def initialize(self):
         stardate_intent = IntentBuilder("StardateIntent").require("StardateKeyword").build()
         self.register_intent(stardate_intent, self.handle_stardate_intent)
 
         intent = IntentBuilder("PodBayDoorsIntent").require("PodBayDoorsKeyword").build()
         self.register_intent(intent, self.handle_pod_intent)
@@ -73,16 +74,14 @@
 
         intent = IntentBuilder("ArnoldIntent").require("ArnoldKeyword").build()
         self.register_intent(intent, self.handle_arnold_intent)
 
         intent = IntentBuilder("GladosIntent").require("GladosKeyword").build()
         self.register_intent(intent, self.handle_glados_intent)
 
-        self.audio_service = AudioService(self.emitter)
-
     def handle_stardate_intent(self, _):
         sd = Stardate().toStardate()
         self.speak_dialog("stardate", {"stardate": sd})
 
     def handle_pod_intent(self, _):
         self.speak_dialog("pod")
```

### Comparing `skill-easter-eggs-0.0.1a1/setup.py` & `skill-easter-eggs-0.0.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `skill-easter-eggs-0.0.1a1/skill_easter_eggs.egg-info/PKG-INFO` & `skill-easter-eggs-0.0.1a2/skill_easter_eggs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skill-easter-eggs
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: UNKNOWN
 Home-page: https://github.com/OpenVoiceOS/skill-easter-eggs
 Author: Jarbas
 Author-email: jarbas@openvoiceos.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skill-easter-eggs Version: 0.0.1a1 Summary: UNKNOWN
+Metadata-Version: 2.1 Name: skill-easter-eggs Version: 0.0.1a2 Summary: UNKNOWN
 Home-page: https://github.com/OpenVoiceOS/skill-easter-eggs Author: Jarbas
 Author-email: jarbas@openvoiceos.com License: BSD-3-Clause Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE ## Easter Eggs [!
 [Donate with Bitcoin](https://en.cryptobadges.io/badge/micro/
 1QJNhKM8tVv62XSUrST2vnaMXh5ADSyYP8)](https://en.cryptobadges.io/donate/
 1QJNhKM8tVv62XSUrST2vnaMXh5ADSyYP8) [![Donate](https://img.shields.io/badge/
 Donate-PayPal-green.svg)](https://paypal.me/jarbasai) [Patreon_donate_button]
```

### Comparing `skill-easter-eggs-0.0.1a1/stardate.py` & `skill-easter-eggs-0.0.1a2/stardate.py`

 * *Files identical despite different names*

