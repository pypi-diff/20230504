# Comparing `tmp/slippistats-0.1.1.tar.gz` & `tmp/slippistats-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippistats-0.1.1.tar", last modified: Wed May  3 00:09:23 2023, max compression
+gzip compressed data, was "slippistats-0.1.2.tar", last modified: Thu May  4 00:44:18 2023, max compression
```

## Comparing `slippistats-0.1.1.tar` & `slippistats-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.152197 slippistats-0.1.1/
--rw-rw-rw-   0        0        0     1084 2023-04-28 03:43:11.000000 slippistats-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5002 2023-05-03 00:09:23.106398 slippistats-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3271 2023-05-02 01:59:46.000000 slippistats-0.1.1/README.md
--rw-rw-rw-   0        0        0      605 2023-05-03 00:08:40.000000 slippistats-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 00:09:23.152197 slippistats-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      728 2023-04-25 21:47:20.000000 slippistats-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.047388 slippistats-0.1.1/slippistats/
--rw-rw-rw-   0        0        0      315 2023-04-28 04:43:30.000000 slippistats-0.1.1/slippistats/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-04-25 21:47:20.000000 slippistats-0.1.1/slippistats/controller.py
-drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.085394 slippistats-0.1.1/slippistats/enums/
--rw-rw-rw-   0        0        0      361 2023-04-28 04:10:10.000000 slippistats-0.1.1/slippistats/enums/__init__.py
--rw-rw-rw-   0        0        0     2739 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/enums/attack.py
--rw-rw-rw-   0        0        0     5670 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/enums/character.py
--rw-rw-rw-   0        0        0     6161 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/enums/item.py
--rw-rw-rw-   0        0        0     3309 2023-04-26 00:48:25.000000 slippistats-0.1.1/slippistats/enums/stage.py
--rw-rw-rw-   0        0        0    51488 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/enums/state.py
--rw-rw-rw-   0        0        0    61534 2023-04-25 21:47:23.000000 slippistats-0.1.1/slippistats/event.py
--rw-rw-rw-   0        0        0     2719 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/game.py
--rw-rw-rw-   0        0        0      394 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/log.py
--rw-rw-rw-   0        0        0     5691 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/metadata.py
--rw-rw-rw-   0        0        0    12567 2023-04-28 04:58:24.000000 slippistats-0.1.1/slippistats/parse.py
-drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.099898 slippistats-0.1.1/slippistats/stats/
--rw-rw-rw-   0        0        0      153 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/stats/__init__.py
--rw-rw-rw-   0        0        0    13781 2023-05-02 02:16:47.000000 slippistats-0.1.1/slippistats/stats/combo_computer.py
--rw-rw-rw-   0        0        0    17798 2023-04-25 21:47:23.000000 slippistats-0.1.1/slippistats/stats/common.py
--rw-rw-rw-   0        0        0    11145 2023-04-25 21:47:23.000000 slippistats-0.1.1/slippistats/stats/computer.py
--rw-rw-rw-   0        0        0    33926 2023-04-26 01:15:54.000000 slippistats-0.1.1/slippistats/stats/stat_types.py
--rw-rw-rw-   0        0        0    35890 2023-04-27 08:10:16.000000 slippistats-0.1.1/slippistats/stats/stats_computer.py
--rw-rw-rw-   0        0        0     3417 2023-04-25 21:47:21.000000 slippistats-0.1.1/slippistats/util.py
-drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.069893 slippistats-0.1.1/slippistats.egg-info/
--rw-rw-rw-   0        0        0     5002 2023-05-03 00:09:22.000000 slippistats-0.1.1/slippistats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      793 2023-05-03 00:09:23.000000 slippistats-0.1.1/slippistats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 00:09:22.000000 slippistats-0.1.1/slippistats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-03 00:09:22.000000 slippistats-0.1.1/slippistats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 00:09:22.000000 slippistats-0.1.1/slippistats.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 00:09:23.103398 slippistats-0.1.1/test/
--rw-rw-rw-   0        0        0        0 2022-12-29 08:44:12.000000 slippistats-0.1.1/test/__init__.py
--rw-rw-rw-   0        0        0    16245 2023-04-25 21:47:22.000000 slippistats-0.1.1/test/replays_test.py
+drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.398912 slippistats-0.1.2/
+-rw-rw-rw-   0        0        0     1084 2023-04-28 03:43:11.000000 slippistats-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5002 2023-05-04 00:44:18.397412 slippistats-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3271 2023-05-02 01:59:46.000000 slippistats-0.1.2/README.md
+-rw-rw-rw-   0        0        0      605 2023-05-04 00:43:55.000000 slippistats-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 00:44:18.398912 slippistats-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      728 2023-04-25 21:47:20.000000 slippistats-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.329900 slippistats-0.1.2/slippistats/
+-rw-rw-rw-   0        0        0      315 2023-04-28 04:43:30.000000 slippistats-0.1.2/slippistats/__init__.py
+-rw-rw-rw-   0        0        0     2912 2023-04-25 21:47:20.000000 slippistats-0.1.2/slippistats/controller.py
+drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.371408 slippistats-0.1.2/slippistats/enums/
+-rw-rw-rw-   0        0        0      361 2023-04-28 04:10:10.000000 slippistats-0.1.2/slippistats/enums/__init__.py
+-rw-rw-rw-   0        0        0     2739 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/enums/attack.py
+-rw-rw-rw-   0        0        0     5670 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/enums/character.py
+-rw-rw-rw-   0        0        0     6161 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/enums/item.py
+-rw-rw-rw-   0        0        0     3309 2023-04-26 00:48:25.000000 slippistats-0.1.2/slippistats/enums/stage.py
+-rw-rw-rw-   0        0        0    51534 2023-05-04 00:42:26.000000 slippistats-0.1.2/slippistats/enums/state.py
+-rw-rw-rw-   0        0        0    61331 2023-05-04 00:42:26.000000 slippistats-0.1.2/slippistats/event.py
+-rw-rw-rw-   0        0        0     2719 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/game.py
+-rw-rw-rw-   0        0        0      394 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/log.py
+-rw-rw-rw-   0        0        0     5691 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/metadata.py
+-rw-rw-rw-   0        0        0    12567 2023-05-04 00:41:23.000000 slippistats-0.1.2/slippistats/parse.py
+drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.386410 slippistats-0.1.2/slippistats/stats/
+-rw-rw-rw-   0        0        0      153 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/stats/__init__.py
+-rw-rw-rw-   0        0        0    13781 2023-05-04 00:41:23.000000 slippistats-0.1.2/slippistats/stats/combo_computer.py
+-rw-rw-rw-   0        0        0    18117 2023-05-04 00:42:26.000000 slippistats-0.1.2/slippistats/stats/common.py
+-rw-rw-rw-   0        0        0    11145 2023-04-25 21:47:23.000000 slippistats-0.1.2/slippistats/stats/computer.py
+-rw-rw-rw-   0        0        0    33926 2023-04-26 01:15:54.000000 slippistats-0.1.2/slippistats/stats/stat_types.py
+-rw-rw-rw-   0        0        0    38543 2023-05-04 00:42:26.000000 slippistats-0.1.2/slippistats/stats/stats_computer.py
+-rw-rw-rw-   0        0        0     3417 2023-04-25 21:47:21.000000 slippistats-0.1.2/slippistats/util.py
+drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.356905 slippistats-0.1.2/slippistats.egg-info/
+-rw-rw-rw-   0        0        0     5002 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-04 00:44:18.000000 slippistats-0.1.2/slippistats.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 00:44:18.392911 slippistats-0.1.2/test/
+-rw-rw-rw-   0        0        0        0 2022-12-29 08:44:12.000000 slippistats-0.1.2/test/__init__.py
+-rw-rw-rw-   0        0        0    16926 2023-05-04 00:42:26.000000 slippistats-0.1.2/test/replays_test.py
```

### Comparing `slippistats-0.1.1/LICENSE.txt` & `slippistats-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/PKG-INFO` & `slippistats-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slippistats
-Version: 0.1.1
+Version: 0.1.2
 Summary: Stats library for SSBM replay files
 Home-page: https://github.com/Walnut356/py-slippi-stats
 Author: Walnut
 Author-email: Walnut356 <walnut356@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 melkor
```

### Comparing `slippistats-0.1.1/README.md` & `slippistats-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/pyproject.toml` & `slippistats-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2273 6c69 7070 6973  .name = "slippis
 00000070: 7461 7473 220d 0a61 7574 686f 7273 203d  tats"..authors =
 00000080: 205b 0d0a 2020 2020 7b6e 616d 6520 3d20   [..    {name = 
 00000090: 2257 616c 6e75 7433 3536 222c 2065 6d61  "Walnut356", ema
 000000a0: 696c 203d 2022 7761 6c6e 7574 3335 3640  il = "walnut356@
 000000b0: 676d 6169 6c2e 636f 6d22 7d0d 0a5d 0d0a  gmail.com"}..]..
-000000c0: 7665 7273 696f 6e20 3d20 2230 2e31 2e31  version = "0.1.1
+000000c0: 7665 7273 696f 6e20 3d20 2230 2e31 2e32  version = "0.1.2
 000000d0: 220d 0a64 6570 656e 6465 6e63 6965 7320  "..dependencies 
 000000e0: 3d20 5b0d 0a20 2020 2022 7079 2d75 626a  = [..    "py-ubj
 000000f0: 736f 6e7e 3d30 2e31 3622 2c0d 0a20 2020  son~=0.16",..   
 00000100: 2022 747a 6c6f 6361 6c7e 3d34 2e33 222c   "tzlocal~=4.3",
 00000110: 0d0a 2020 2020 2270 6f6c 6172 737e 3d30  ..    "polars~=0
 00000120: 2e31 372e 3922 2c0d 0a5d 0d0a 636c 6173  .17.9",..]..clas
 00000130: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..
```

### Comparing `slippistats-0.1.1/setup.py` & `slippistats-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/controller.py` & `slippistats-0.1.2/slippistats/controller.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/enums/attack.py` & `slippistats-0.1.2/slippistats/enums/attack.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/enums/character.py` & `slippistats-0.1.2/slippistats/enums/character.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/enums/item.py` & `slippistats-0.1.2/slippistats/enums/item.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/enums/stage.py` & `slippistats-0.1.2/slippistats/enums/stage.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/enums/state.py` & `slippistats-0.1.2/slippistats/enums/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,14 +218,16 @@
     AERIAL_ATTACK_END = 74
     FALL_SPECIAL_START = 35
     FALL_SPECIAL_END = 37
     AERIAL_LAND_LAG_START = 70
     AERIAL_LAND_LAG_END = 74
     ACTIONABLE_AIR_START = 25
     ACTIONABLE_AIR_END = 34
+    THROWN_START = 239
+    THROWN_END = 243
 
     # Command Grabs
     COMMAND_GRAB_RANGE1_START = 266
     COMMAND_GRAB_RANGE1_END = 304
 
     COMMAND_GRAB_RANGE2_START = 327
     COMMAND_GRAB_RANGE2_END = 338
```

### Comparing `slippistats-0.1.1/slippistats/event.py` & `slippistats-0.1.2/slippistats/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1010,15 +1010,15 @@
                             state_age=state_age,
                             position=position,
                             direction=direction,
                             damage=damage,
                             shield_health=shield_health,
                             stocks=stocks,
                             most_recent_hit=last_attack_landed,
-                            last_hit_by=last_hit_by if last_hit_by < 4 else None,
+                            last_hit_by=last_hit_by,
                             combo_count=combo_count,
                         )
 
                     try:  # v2.0.0
                         flags = [
                             Field1(*unpack_uint8(read(1))),
                             Field2(*unpack_uint8(read(1))),
@@ -1040,15 +1040,15 @@
                             state_age=state_age,
                             position=position,
                             direction=direction,
                             damage=damage,
                             shield_health=shield_health,
                             stocks=stocks,
                             most_recent_hit=last_attack_landed,
-                            last_hit_by=last_hit_by if last_hit_by < 4 else None,
+                            last_hit_by=last_hit_by,
                             combo_count=combo_count,
                         )
 
                     try:  # v2.1.0
                         (hurtbox_status,) = unpack_uint8(read(1))
                     except struct.error:
                         return cls(
@@ -1057,15 +1057,15 @@
                             state_age=state_age,
                             position=position,
                             direction=direction,
                             damage=damage,
                             shield_health=shield_health,
                             stocks=stocks,
                             most_recent_hit=last_attack_landed,
-                            last_hit_by=last_hit_by if last_hit_by < 4 else None,
+                            last_hit_by=last_hit_by,
                             combo_count=combo_count,
                             flags=flags,
                             misc_timer=misc_timer,
                             airborne=airborne,
                             last_ground_id=last_ground_id,
                             jumps=jumps,
                             l_cancel=l_cancel,
@@ -1083,15 +1083,15 @@
                             state_age=state_age,
                             position=position,
                             direction=direction,
                             damage=damage,
                             shield_health=shield_health,
                             stocks=stocks,
                             most_recent_hit=last_attack_landed,
-                            last_hit_by=last_hit_by if last_hit_by < 4 else None,
+                            last_hit_by=last_hit_by,
                             combo_count=combo_count,
                             flags=flags,
                             misc_timer=misc_timer,
                             airborne=airborne,
                             last_ground_id=last_ground_id,
                             jumps=jumps,
                             l_cancel=l_cancel,
@@ -1107,15 +1107,15 @@
                             state_age=state_age,
                             position=position,
                             direction=direction,
                             damage=damage,
                             shield_health=shield_health,
                             stocks=stocks,
                             most_recent_hit=last_attack_landed,
-                            last_hit_by=last_hit_by if last_hit_by < 4 else None,
+                            last_hit_by=last_hit_by,
                             combo_count=combo_count,
                             flags=flags,
                             misc_timer=misc_timer,
                             airborne=airborne,
                             last_ground_id=last_ground_id,
                             jumps=jumps,
                             l_cancel=l_cancel,
@@ -1134,15 +1134,15 @@
                             state_age=state_age,
                             position=position,
                             direction=direction,
                             damage=damage,
                             shield_health=shield_health,
                             stocks=stocks,
                             most_recent_hit=last_attack_landed,
-                            last_hit_by=last_hit_by if last_hit_by < 4 else None,
+                            last_hit_by=last_hit_by,
                             combo_count=combo_count,
                             flags=flags,
                             misc_timer=misc_timer,
                             airborne=airborne,
                             last_ground_id=last_ground_id,
                             jumps=jumps,
                             l_cancel=l_cancel,
@@ -1159,15 +1159,15 @@
                         state_age=state_age,
                         position=position,
                         direction=direction,
                         damage=damage,
                         shield_health=shield_health,
                         stocks=stocks,
                         most_recent_hit=last_attack_landed,
-                        last_hit_by=last_hit_by if last_hit_by < 4 else None,
+                        last_hit_by=last_hit_by,
                         combo_count=combo_count,
                         flags=flags,
                         misc_timer=misc_timer,
                         airborne=airborne,
                         last_ground_id=last_ground_id,
                         jumps=jumps,
                         l_cancel=l_cancel,
```

### Comparing `slippistats-0.1.1/slippistats/game.py` & `slippistats-0.1.2/slippistats/game.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/metadata.py` & `slippistats-0.1.2/slippistats/metadata.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/parse.py` & `slippistats-0.1.2/slippistats/parse.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/stats/combo_computer.py` & `slippistats-0.1.2/slippistats/stats/combo_computer.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/stats/common.py` & `slippistats-0.1.2/slippistats/stats/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 from ..enums.stage import Stage
 from ..enums.state import (
     ActionRange,
     ActionState,
     Field2,
     Field4,
 )
+from ..enums.attack import Attack
 from ..event import Frame, Position, Velocity
 from ..util import IntEnum
 
 # ---------------------------------------------------------------------------- #
 #                                 State Helpers                                #
 # ---------------------------------------------------------------------------- #
 
 
 def just_entered_state(
-    action_state: int | Callable,
+    action_state: int | Callable[[int], bool],
     curr_state: ActionState | int,
     prev_state: ActionState | int,
 ) -> bool:
     # TODO test this
     if isinstance(action_state, Callable):
         return action_state(curr_state) and not action_state(prev_state)
 
@@ -74,14 +75,15 @@
 
 
 def is_damaged(action_state: int) -> bool:
     """Takes action state, returns whether or not the player is in a damaged state.
     This includes all generic variants."""
     return (
         (ActionRange.DAMAGE_START <= action_state <= ActionRange.DAMAGE_END)
+        # TODO probably include DAMAGE_FALL as well?
         or action_state == ActionState.DOWN_DAMAGE_U
         or action_state == ActionState.DOWN_DAMAGE_D
     )  # Jab reset states, prevents combo counter from ignoring them if not checking hitstun
 
 
 def is_in_hitstun(flags: list[IntEnum]) -> bool:
     """Takes StateFlags, returns whether or not the hitstun bitflag is active.
@@ -483,14 +485,20 @@
 def calc_damage_taken(curr_frame: Frame.Port.Data.Post, prev_frame: Frame.Port.Data.Post) -> float:
     """Takes current and previous frames, returns float of the difference in damage between the two"""
     percent = curr_frame.percent
     prev_percent = prev_frame.percent
 
     return percent - prev_percent
 
+THROW_STATE_TO_ATTACK = {
+    ActionState.THROW_F : Attack.FORWARD_THROW,
+    ActionState.THROW_B : Attack.BACK_THROW,
+    ActionState.THROW_HI : Attack.UP_THROW,
+    ActionState.THROW_LW : Attack.DOWN_THROW,
+}
 
 # ---------------------------------------------------------------------------- #
 #                                Output Helpers                                #
 # ---------------------------------------------------------------------------- #
 
 
 def get_playback_header() -> dict:
```

### Comparing `slippistats-0.1.1/slippistats/stats/computer.py` & `slippistats-0.1.2/slippistats/stats/computer.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/stats/stat_types.py` & `slippistats-0.1.2/slippistats/stats/stat_types.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats/stats/stats_computer.py` & `slippistats-0.1.2/slippistats/stats/stats_computer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,24 @@
     ActionState,
     LCancel,
 )
 from ..event import Attack, Buttons
 from ..game import Game
 from ..util import Port, try_enum
 from .common import (
+    THROW_STATE_TO_ATTACK,
     JoystickRegion,
     TechType,
     get_angle,
     get_joystick_region,
     get_post_di_angle,
     get_post_di_velocity,
     get_tech_type,
     is_damaged,
+    is_downed,
     is_dying,
     is_fastfalling,
     is_in_hitlag,
     is_in_hitstun,
     is_ledge_action,
     is_offstage,
     is_shielding,
@@ -402,40 +404,81 @@
                 require at least replay version 3.5.0, got replay version {self.replay_version}.""",
                 RuntimeWarning,
             )
 
         for i, player_frame in enumerate(player.frames):
             if i == 0:
                 continue
+            if i == 3073:
+                pass
             prev_player_frame = player.frames[i - 1]
             opponent_frame = opponent.frames[i]
 
+            # This is for the throw check, as we want the state before the grab rather than the state before the throw
+            # deals damage.
+            if (
+                player_frame.post.state == ActionState.CAPTURE_PULLED_HI
+                or player_frame.post.state == ActionState.CAPTURE_PULLED_LW
+            ) and not (
+                prev_player_frame.post.state == ActionState.CAPTURE_PULLED_HI
+                or prev_player_frame.post.state == ActionState.CAPTURE_PULLED_LW
+            ):
+                pre_grab_state = prev_player_frame.post.state
+
             # right now i don't care about shield SDI/ASDI but i may change this down the line
             # it requires slightly different logic
             in_hitlag = is_in_hitlag(player_frame.post.flags) and not is_shielding(prev_player_frame.post.state)
             was_in_hitlag = is_in_hitlag(prev_player_frame.post.flags) and not is_shielding(
                 prev_player_frame.post.state
             )
 
             # this whole block basically calculates DI and KB trajectories and outputs the event
             if not in_hitlag:
-                if was_in_hitlag and self._take_hit_state is not None:
+                # Not every throw puts the player in hitlag, so we need a bespoke check to catch them.
+                # TODO check how KB and DI velocities look just before/during/after the grabbed -> thrown transition
+                if (
+                    (  # the downed and teching checks are necessary for things like fox's dthrow where the opponent goes
+                        # straight from capture throw -> downed/tech state
+                        is_damaged(player_frame.post.state)
+                        or is_downed(player_frame.post.state)
+                        or is_teching(player_frame.post.state)
+                    )
+                    and just_took_damage(player_frame.post.percent, player_frame.pre.percent)
+                    and (ActionRange.THROWN_START <= prev_player_frame.post.state <= ActionRange.THROWN_END)
+                ):
+                    self._take_hit_state = TakeHitData(
+                        frame_index=i,
+                        stocks_remaining=player_frame.post.stocks_remaining,
+                        last_hit_by=try_enum(Attack, opponent_frame.post.most_recent_hit),
+                        state_before_hit=pre_grab_state,
+                        start_pos=player_frame.post.position,
+                        percent=player_frame.post.percent,
+                        grounded=not player_frame.post.is_airborne,
+                    )
+                    if knockback_check:
+                        self._take_hit_state.kb_velocity = player_frame.post.knockback_velocity
+                        self._take_hit_state.kb_angle = degrees(get_angle(player_frame.post.knockback_velocity))
+                    else:
+                        self._take_hit_state.kb_velocity = None
+                        self._take_hit_state.kb_angle = None
+
+                    self._take_hit_state.crouch_cancel = False
+                if self._take_hit_state is not None:
                     self._take_hit_state.end_pos = prev_player_frame.post.position
 
                     effective_stick = player_frame.pre.joystick
                     match get_joystick_region(player_frame.pre.joystick):
                         case JoystickRegion.UP:
                             effective_stick.x = 0
                         case JoystickRegion.DOWN:
                             effective_stick.x = 0
                         case JoystickRegion.LEFT:
                             effective_stick.y = 0
                         case JoystickRegion.RIGHT:
                             effective_stick.y = 0
-
                         case JoystickRegion.DEAD_ZONE:
                             effective_stick.x = 0
                             effective_stick.y = 0
                         case _:
                             pass
 
                     self._take_hit_state.di_stick_pos = effective_stick
@@ -468,15 +511,18 @@
 
                     self._take_hit_state._find_valid_sdi()
 
                     player.stats.take_hits.append(self._take_hit_state)
                     self._take_hit_state = None
                 continue
 
-            if not was_in_hitlag and just_took_damage(player_frame.post.percent, prev_player_frame.post.percent):
+            if (not was_in_hitlag) and just_took_damage(player_frame.post.percent, player_frame.pre.percent):
+                if try_enum(Attack, opponent_frame.post.most_recent_hit) == 0:
+                    pass
+
                 self._take_hit_state = TakeHitData(
                     frame_index=i,
                     stocks_remaining=player_frame.post.stocks_remaining,
                     last_hit_by=try_enum(Attack, opponent_frame.post.most_recent_hit),
                     state_before_hit=player.frames[i - 1].post.state,
                     start_pos=player_frame.post.position,
                     percent=player_frame.post.percent,
```

### Comparing `slippistats-0.1.1/slippistats/util.py` & `slippistats-0.1.2/slippistats/util.py`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/slippistats.egg-info/PKG-INFO` & `slippistats-0.1.2/slippistats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slippistats
-Version: 0.1.1
+Version: 0.1.2
 Summary: Stats library for SSBM replay files
 Home-page: https://github.com/Walnut356/py-slippi-stats
 Author: Walnut
 Author-email: Walnut356 <walnut356@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 melkor
```

### Comparing `slippistats-0.1.1/slippistats.egg-info/SOURCES.txt` & `slippistats-0.1.2/slippistats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slippistats-0.1.1/test/replays_test.py` & `slippistats-0.1.2/test/replays_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -396,14 +396,23 @@
                         is_shot_launched=None,
                         charge_power=None,
                         owner=None,
                         )
                 }
             )
 
+    def test_throw_detection(self):
+        throws = StatsComputer(self._game(R"fox_throws")).stats_compute()[1].stats.take_hits.to_polars()
+        throws = throws.select(pl.col("character"), pl.col("opnt_character"), pl.col("frame_index"), pl.col("last_hit_by"))
+        assert(throws.frame_equal(pl.read_parquet(R"test/data/fox_throws.parquet")))
+        throws = StatsComputer(self._game(R"falcon_throws")).stats_compute()[1].stats.take_hits.to_polars()
+        throws = throws.select(pl.col("character"), pl.col("opnt_character"), pl.col("frame_index"), pl.col("last_hit_by"))
+        assert(throws.frame_equal(pl.read_parquet(R"test/data/falcon_throws.parquet")))
+
+
     # def test_wavedash_data(self):
     #     wavedashes = StatsComputer(self._game("wavedash"))
     #     wavedashes = wavedashes.wavedash_compute(player=wavedashes.players[0]).to_polars()
     #     assert (wavedashes.frame_equal(pl.read_parquet(Path(r'test\data\wavedash.parquet'))))
 
     # def test_dash_data(self):
     #     dashes = StatsComputer(self._game("dash"))
```

