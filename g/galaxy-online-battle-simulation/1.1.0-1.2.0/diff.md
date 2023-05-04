# Comparing `tmp/galaxy-online-battle-simulation-1.1.0.tar.gz` & `tmp/galaxy-online-battle-simulation-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-online-battle-simulation-1.1.0.tar", last modified: Wed Nov  9 09:08:31 2022, max compression
+gzip compressed data, was "galaxy-online-battle-simulation-1.2.0.tar", last modified: Thu May  4 08:48:38 2023, max compression
```

## Comparing `galaxy-online-battle-simulation-1.1.0.tar` & `galaxy-online-battle-simulation-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,42 @@
-drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2022-11-09 09:08:31.055350 galaxy-online-battle-simulation-1.1.0/
--rw-rw-r--   0 adminator  (1000) adminator  (1000)     1105 2022-10-25 13:01:55.000000 galaxy-online-battle-simulation-1.1.0/LICENSE
--rw-rw-r--   0 adminator  (1000) adminator  (1000)       39 2022-10-25 10:38:44.000000 galaxy-online-battle-simulation-1.1.0/MANIFEST.in
--rw-rw-r--   0 adminator  (1000) adminator  (1000)     8676 2022-11-09 09:08:31.055350 galaxy-online-battle-simulation-1.1.0/PKG-INFO
--rw-rw-r--   0 adminator  (1000) adminator  (1000)     6949 2022-11-09 07:46:03.000000 galaxy-online-battle-simulation-1.1.0/README.md
--rw-rw-r--   0 adminator  (1000) adminator  (1000)      769 2022-11-09 08:00:30.000000 galaxy-online-battle-simulation-1.1.0/pyproject.toml
--rw-rw-r--   0 adminator  (1000) adminator  (1000)       38 2022-11-09 09:08:31.055350 galaxy-online-battle-simulation-1.1.0/setup.cfg
-drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2022-11-09 09:08:31.051350 galaxy-online-battle-simulation-1.1.0/src/
-drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2022-11-09 09:08:31.055350 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/
--rw-rw-r--   0 adminator  (1000) adminator  (1000)     1205 2022-11-09 08:01:09.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/__init__.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    23587 2022-10-31 18:32:45.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/__main__.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    96074 2022-11-08 17:48:30.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/battle_simulation.py
-drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2022-11-09 09:08:31.055350 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/
--rw-rw-r--   0 adminator  (1000) adminator  (1000)        0 2022-10-07 14:40:28.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/__init__.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    16148 2022-10-22 05:30:37.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/basic_game_entity.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    19703 2022-10-25 06:36:38.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/building.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    24876 2022-11-08 18:39:06.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/config.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)     6137 2022-11-01 05:13:03.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/damage.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    12715 2022-10-24 11:17:12.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/module_and_bonuses.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    11492 2022-10-25 06:43:03.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/planet.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    11694 2022-10-24 15:23:06.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/rocket.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    28513 2022-11-08 17:45:54.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/spacefleet.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)     9927 2022-11-01 04:58:27.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/spaceship.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)     1166 2022-10-20 09:03:22.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/utility.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    82580 2022-11-09 06:17:39.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/context.py
--rw-rw-r--   0 adminator  (1000) adminator  (1000)    15952 2022-11-09 09:04:25.000000 galaxy-online-battle-simulation-1.1.0/src/battlesimulation/data.json
-drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2022-11-09 09:08:31.055350 galaxy-online-battle-simulation-1.1.0/src/galaxy_online_battle_simulation.egg-info/
--rw-rw-r--   0 adminator  (1000) adminator  (1000)     8676 2022-11-09 09:08:31.000000 galaxy-online-battle-simulation-1.1.0/src/galaxy_online_battle_simulation.egg-info/PKG-INFO
--rw-rw-r--   0 adminator  (1000) adminator  (1000)     1010 2022-11-09 09:08:31.000000 galaxy-online-battle-simulation-1.1.0/src/galaxy_online_battle_simulation.egg-info/SOURCES.txt
--rw-rw-r--   0 adminator  (1000) adminator  (1000)        1 2022-11-09 09:08:31.000000 galaxy-online-battle-simulation-1.1.0/src/galaxy_online_battle_simulation.egg-info/dependency_links.txt
--rw-rw-r--   0 adminator  (1000) adminator  (1000)       68 2022-11-09 09:08:31.000000 galaxy-online-battle-simulation-1.1.0/src/galaxy_online_battle_simulation.egg-info/entry_points.txt
--rw-rw-r--   0 adminator  (1000) adminator  (1000)       17 2022-11-09 09:08:31.000000 galaxy-online-battle-simulation-1.1.0/src/galaxy_online_battle_simulation.egg-info/top_level.txt
+drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2023-05-04 08:48:38.619315 galaxy-online-battle-simulation-1.2.0/
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     1105 2022-10-25 13:01:55.000000 galaxy-online-battle-simulation-1.2.0/LICENSE
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)       39 2022-10-25 10:38:44.000000 galaxy-online-battle-simulation-1.2.0/MANIFEST.in
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     8676 2023-05-04 08:48:38.619315 galaxy-online-battle-simulation-1.2.0/PKG-INFO
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     6949 2022-11-09 07:46:03.000000 galaxy-online-battle-simulation-1.2.0/README.md
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)      769 2023-05-04 07:55:46.000000 galaxy-online-battle-simulation-1.2.0/pyproject.toml
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)       38 2023-05-04 08:48:38.619315 galaxy-online-battle-simulation-1.2.0/setup.cfg
+drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2023-05-04 08:48:38.615315 galaxy-online-battle-simulation-1.2.0/src/
+drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2023-05-04 08:48:38.615315 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     1205 2023-05-04 07:55:36.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/__init__.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    23587 2022-10-31 18:32:45.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/__main__.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    99925 2023-05-04 07:43:01.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/battle_simulation.py
+drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2023-05-04 08:48:38.619315 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)        0 2022-10-07 14:40:28.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/__init__.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    16148 2022-10-22 05:30:37.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/basic_game_entity.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    19703 2022-10-25 06:36:38.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/building.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    24871 2022-12-11 19:45:03.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/config.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     6137 2022-11-01 05:13:03.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/damage.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    14861 2023-05-04 07:41:05.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/module_and_bonuses.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    11492 2022-10-25 06:43:03.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/planet.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    11694 2022-10-24 15:23:06.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/rocket.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    29168 2022-12-09 05:29:24.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/spacefleet.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     9927 2022-11-01 04:58:27.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/spaceship.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     1166 2022-10-20 09:03:22.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/utility.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    86612 2023-05-04 07:50:28.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/context.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    15952 2022-11-09 09:04:25.000000 galaxy-online-battle-simulation-1.2.0/src/battlesimulation/data.json
+drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2023-05-04 08:48:38.619315 galaxy-online-battle-simulation-1.2.0/src/galaxy_online_battle_simulation.egg-info/
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     8676 2023-05-04 08:48:38.000000 galaxy-online-battle-simulation-1.2.0/src/galaxy_online_battle_simulation.egg-info/PKG-INFO
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     1262 2023-05-04 08:48:38.000000 galaxy-online-battle-simulation-1.2.0/src/galaxy_online_battle_simulation.egg-info/SOURCES.txt
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)        1 2023-05-04 08:48:38.000000 galaxy-online-battle-simulation-1.2.0/src/galaxy_online_battle_simulation.egg-info/dependency_links.txt
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)       68 2023-05-04 08:48:38.000000 galaxy-online-battle-simulation-1.2.0/src/galaxy_online_battle_simulation.egg-info/entry_points.txt
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)       17 2023-05-04 08:48:38.000000 galaxy-online-battle-simulation-1.2.0/src/galaxy_online_battle_simulation.egg-info/top_level.txt
+drwxrwxr-x   0 adminator  (1000) adminator  (1000)        0 2023-05-04 08:48:38.619315 galaxy-online-battle-simulation-1.2.0/tests/
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    12621 2022-10-25 06:26:33.000000 galaxy-online-battle-simulation-1.2.0/tests/test_anti_enemy_finder.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     2777 2022-10-14 05:43:34.000000 galaxy-online-battle-simulation-1.2.0/tests/test_buildings_planet.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     1358 2022-12-09 10:26:49.000000 galaxy-online-battle-simulation-1.2.0/tests/test_combinations.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     6374 2022-10-24 04:49:20.000000 galaxy-online-battle-simulation-1.2.0/tests/test_context.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     3857 2022-10-21 10:12:07.000000 galaxy-online-battle-simulation-1.2.0/tests/test_context_helper.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)    13013 2022-10-25 06:23:15.000000 galaxy-online-battle-simulation-1.2.0/tests/test_custom_data.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     1018 2022-10-08 09:45:33.000000 galaxy-online-battle-simulation-1.2.0/tests/test_fleet_copy.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     3540 2023-05-04 07:51:43.000000 galaxy-online-battle-simulation-1.2.0/tests/test_fleet_vs_fleet.py
+-rw-rw-r--   0 adminator  (1000) adminator  (1000)     2994 2022-10-14 05:43:00.000000 galaxy-online-battle-simulation-1.2.0/tests/test_fleet_vs_rockets.py
```

### Comparing `galaxy-online-battle-simulation-1.1.0/LICENSE` & `galaxy-online-battle-simulation-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/PKG-INFO` & `galaxy-online-battle-simulation-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-online-battle-simulation
-Version: 1.1.0
+Version: 1.2.0
 Summary: Module for simulation of different battles in the online space strategy game Galaxy Online.
 Author: fadedness
 License: The MIT License (MIT)
         Copyright © 2022 fadedness https://t.me/fadedness
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `galaxy-online-battle-simulation-1.1.0/README.md` & `galaxy-online-battle-simulation-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/pyproject.toml` & `galaxy-online-battle-simulation-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=58.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "galaxy-online-battle-simulation"
-version = "1.1.0"
+version = "1.2.0"
 description = "Module for simulation of different battles in the online space strategy game Galaxy Online."
 readme = "README.md"
 authors = [{ name = "fadedness" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/__init__.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 from battlesimulation.components.config import _GlobalGameParameters
 
 _GGP: _GlobalGameParameters = None
 _debug_printing = False
 _debug_limit_variables = True
```

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/__main__.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/__main__.py`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/battle_simulation.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/battle_simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,42 +105,42 @@
             if overbonus1 > battlesimulation._GGP.thold_max:
                 overbonus1 = battlesimulation._GGP.thold_max - 1
             elif overbonus2 > battlesimulation._GGP.thold_max:
                 overbonus2 = battlesimulation._GGP.thold_max - 1
         return (overbonus1, overbonus2)
 
     def _finalize_bonuses_mods(self, fleet1: SpaceFleet, fleet2: SpaceFleet = None, \
-            sequence: tuple = ("module","superiority","damage"), \
-            combination_method_for_mods: tuple = ("add", "add", "multiply"), \
+            sequence: tuple = ("module","superiority","damage","elder"), \
+            combination_method_for_mods: tuple = ("add", "add", "add", "add"), \
             truncate_to: int = 6) -> None:
         """Combines bonuses from Modules with from Modules attack/defense damage specific and with superiority bonus.
 
             You can change order and method of combinations.
             Also if you omit Fleet 2, bonuses for Fleet 1 will be combined without superiority.
         """
 
-        if isinstance(sequence, tuple) and len(sequence) == 3 and "module" in sequence \
-                and "superiority" in sequence and "damage" in sequence:
+        if isinstance(sequence, tuple) and len(sequence) == 4 and "module" in sequence \
+                and "superiority" in sequence and "damage" in sequence and "elder" in sequence:
             # ok
             pass
         else:
             # set the defaults
             debug_print("Invalid input for sequence. Using defaults.")
-            sequence = ("module","superiority","damage")
-        if isinstance(combination_method_for_mods, tuple) and len(combination_method_for_mods) == 3:
+            sequence = ("module","superiority","damage","elder")
+        if isinstance(combination_method_for_mods, tuple) and len(combination_method_for_mods) == 4:
             for item in combination_method_for_mods:
                 if item not in ("add","multiply"):
                     # set the defaults
                     debug_print("Invalid input for combination_method_for_mods. Using defaults.")
-                    combination_method_for_mods = ("add", "add", "multiply")
+                    combination_method_for_mods = ("add", "add", "add")
                     break
         else:
             # set the defaults
             debug_print("Invalid input for combination_method_for_mods. Using defaults.")
-            combination_method_for_mods = ("add", "add", "multiply")
+            combination_method_for_mods = ("add", "add", "add", "add")
         if isinstance(fleet1, SpaceFleet) and isinstance(fleet2, SpaceFleet):
             superiority = self._calc_superiority(fleet1, fleet2)
             fleet1.modules.calc_final_damage_mods(superiority[0], *combination_method_for_mods, sequence, truncate_to)
             fleet2.modules.calc_final_damage_mods(superiority[1], *combination_method_for_mods, sequence, truncate_to)
         elif isinstance(fleet1, SpaceFleet) and fleet2 is None:
             fleet1.modules.calc_final_damage_mods(1.0, *combination_method_for_mods, sequence, truncate_to)
 
@@ -992,14 +992,82 @@
             # otherwise round up them here
             if full_attack:
                 result = against_turrets + against_rockets
             else:
                 result = _my_round_up(against_turrets + against_rockets)
             return result
 
+    def __test_spaceship_double_combinations_to_beat_enemy_minimum(self, ss_id_1: int, ss_id_2: int, fleet1: SpaceFleet, fleet2: SpaceFleet):
+        """"""
+
+        ss_id_step_rate = 0.01
+
+        fleet1_copy = fleet1.make_a_copy_of_self()
+        fleet1_copy.coef_cost_of_dead = fleet1.coef_cost_of_dead
+        fleet1_copy.coef_build_time_of_dead = fleet1.coef_build_time_of_dead
+        fleet1_copy.modules.calc_final_damage_mods(1.0)
+
+        fleet2_copy = fleet2.make_a_copy_of_self()
+
+        ss_id_1_minimum = self._find_suitable_spaceship_to_beat_enemy_minimum(ss_id_1, fleet1_copy.modules, fleet2_copy)
+        fleet1_copy.set_fleet(((ss_id_1, ss_id_1_minimum)))
+        superiority = self._calc_superiority(fleet1_copy, fleet2_copy)
+        approximate_fleet1_superiority = superiority[0]
+        #ss_id_2_minimum = self._find_suitable_spaceship_to_beat_enemy_minimum(ss_id_2, fleet1_copy.modules, fleet2)
+
+        ss_id_1_step = int(ss_id_1_minimum * ss_id_step_rate)
+        ss_id_cap_stop = ss_id_1_minimum // 2
+        ss_id_cap = 0
+        ss_id_1_total = ss_id_1_minimum + ss_id_1_step
+        ss_id_2_total = 0
+        ss_quantities_to_test = []
+        ss_1 = Spaceship(ss_id_1, ss_id_1_minimum)
+        ss_1_damage_one_spaceship = ss_1.attack * (ss_1.accuracy / 100) * fleet1_copy.modules.final_attack_damage_mods[ss_1.damage_type_id]
+        ss_1_damage = ss_1_damage_one_spaceship * ss_1.quantity
+        ss_1_damage_step = ss_1_damage_one_spaceship * ss_id_1_step
+        ss_2 = Spaceship(ss_id_2)
+        final_results = []
+        while 1:
+            if ss_id_cap + ss_id_1_step > ss_id_cap_stop:
+                break
+            ss_id_cap += ss_id_1_step
+            ss_id_1_total -= ss_id_1_step
+            ss_1_damage -= ss_1_damage_step
+            ss_1_damage_array = DamageArray()
+            ss_1_damage_array.add_damage(Damage(ss_1.damage_type_id, ss_1_damage))
+            fleet2_copy_temp = fleet2.make_a_copy_of_self()
+            fleet2_copy_temp.modules.calc_final_damage_mods(superiority[1])
+            fleet2_copy_temp._temp_incoming_damage_array = ss_1_damage_array
+            self._recursive_deal_damage_simple_fleet_vs_damage_array(fleet2_copy_temp)
+            damage_needed = 0
+            for ss in fleet2_copy_temp:
+                ss: Spaceship
+                damage_needed += ss.quantity * ss.defenses[ss_1.damage_type_id]
+            ss_id_2_step = _my_round_up(damage_needed / (ss_2.attack * (ss.accuracy / 100) * fleet1_copy.modules.final_attack_damage_mods[ss_2.damage_type_id]))
+            ss_id_2_total += ss_id_2_step
+            fleet1_copy_temp = fleet1_copy.make_a_copy_of_self()
+            fleet1_copy_temp.set_fleet([(ss_id_1, ss_id_1_total), (ss_id_2, ss_id_2_total)])
+            fleet2_copy_temp = fleet2_copy.make_a_copy_of_self()
+            self.simulate(fleet1_copy_temp, fleet2_copy_temp, Planet())
+            print(f"\n\nFleet 1:\n{fleet1_copy_temp.filtered_alive_str}\n\nFleet 2:\n{fleet2_copy_temp.filtered_alive_str}\n\n")
+            #battlesimulation._debug_printing = False
+            while 1:
+                ss_id_2_total += 1
+                fleet1_copy_temp = fleet1_copy.make_a_copy_of_self()
+                fleet1_copy_temp.set_fleet([(ss_id_1, ss_id_1_total), (ss_id_2, ss_id_2_total)])
+                fleet2_copy_temp = fleet2.make_a_copy_of_self()
+                self.simulate(fleet1_copy_temp, fleet2_copy_temp, Planet())
+                print(f"\n\nFleet 1:\n{fleet1_copy_temp.filtered_alive_str}\n\nFleet 2:\n{fleet2_copy_temp.filtered_alive_str}\n\n")
+                if not fleet2_copy_temp.is_populated:
+                    break
+            #battlesimulation._debug_printing = True
+            final_results.append((ss_id_1_total, ss_id_2_total, fleet1_copy_temp.antirating))
+
+        return final_results
+
     def _get_basic_vars_for_old_bombardment(self, spaceship_module: ModuleAndBonuses, planet: Planet) -> dict:
         """Old Bombardment Mechanic, returns a dict with values of Planetary Defenses."""
 
         if isinstance(spaceship_module, ModuleAndBonuses) and isinstance(planet, Planet) and \
                 isinstance(planet.rockets, RocketArray) and isinstance(planet.buildings, BuildingArray):
             # calculate Valkyries needed to pass Turrets and Rockets
             spaceship_module.calc_final_damage_mods(1.0)
```

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/basic_game_entity.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/basic_game_entity.py`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/building.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/building.py`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/config.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     "Spaceships": {
         1: {
             "id": 1,
             "name": "Геркулес",
             "name_en": "Hercules",
             "damage_type_id": 2,
             "attack": 25,
-            "defense": 275,
-            "defenses": { 1: 330, 2: 275, 3: 220, 4: 248, 5: 303 },
+            "defense": 75,
+            "defenses": { 1: 90, 2: 75, 3: 60, 4: 68, 5: 83 },
             "weight": 10,
             "attack_priority": 250,
             "defense_priority": 250,
             "speed": 5,
             "calc_speed": 2.56,
             "price": 500,
             "build_time": 300,
@@ -554,8 +554,8 @@
         new_modules.update({int(mod_id): data["Modules"][mod_id].copy()})
     new_data.update({"Modules": deepcopy(new_modules)})
     new_resources = {}
     for res_id in data["Resources"]:
         new_resources.update({int(res_id): data["Resources"][res_id].copy()})
     new_data.update({"Resources": deepcopy(new_resources)})
     new_data.update({"Globals": deepcopy(data["Globals"])})
-    return new_data
+    return new_data
```

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/damage.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/damage.py`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/module_and_bonuses.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/module_and_bonuses.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
     def __init__(self) -> None:
         self.attack_damage_mods = {}
         self.defense_damage_mods = {}
         self.final_attack_damage_mods = {}
         self.final_defense_damage_mods = {}
         self.final_no_superiority_defense_damage_mods = {}
+        self.elder_bonus_attack = 1.0
+        self.elder_bonus_defense = 1.0
+        self.elder_bonus_speed = 1.0
         self._reinit()
 
     def _reinit(self):
         self.id = -1
         self.level = 1
         self.attack = 1.0
         self.defense = 1.0
@@ -142,26 +145,72 @@
         if target == "attack":
             self.attack_damage_mods.update(result)
         elif target == "defense":
             self.defense_damage_mods.update(result)
         else:
             pass
 
+    def elder_buff_attack(self):
+        """Sets elder attack bonus to 1.5 (+50%)"""
+
+        self.elder_bonus_attack = 1.5
+
+    def elder_debuff_attack(self):
+        """Sets elder attack bonus to 0.5 (-50%)"""
+
+        self.elder_bonus_attack = 0.5
+
+    def reset_elder_attack(self):
+        """Sets elder attack bonus to 1.0 (+0%)"""
+
+        self.elder_bonus_attack = 1.0
+
+    def elder_buff_defense(self):
+        """Sets elder defense bonus to 1.5 (+50%)"""
+
+        self.elder_bonus_defense = 1.5
+
+    def elder_debuff_defense(self):
+        """Sets elder defense bonus to 0.5 (-50%)"""
+
+        self.elder_bonus_defense = 0.5
+
+    def reset_elder_defense(self):
+        """Sets elder defense bonus to 1.0 (+0%)"""
+
+        self.elder_bonus_defense = 1.0
+
+    def elder_buff_speed(self):
+        """Sets elder speed bonus to 1.5 (+50%)"""
+
+        self.elder_bonus_speed = 1.5
+
+    def elder_debuff_speed(self):
+        """Sets elder speed bonus to 0.5 (-50%)"""
+
+        self.elder_bonus_speed = 0.5
+
+    def reset_elder_speed(self):
+        """Sets elder speed bonus to 1.0 (+0%)"""
+
+        self.elder_bonus_speed = 1.0
+
     def calc_final_damage_mods(self, superiority: float, combination_module: str = "add", \
             combination_superiority: str = "add", combination_damage: str = "add", \
-            sequence: Union[list,tuple] = ("module","superiority","damage"), \
+            combination_elder: str = "add", \
+            sequence: Union[list,tuple] = ("module","superiority","damage","elder"), \
             truncate_to: int = 6) -> None:
         """Combines bonuses from Modules with from Modules attack/defense damage specific and with superiority bonus.
 
             There are two ways to combine bonuses: add percentage or multiply fractions.
             Also you can define the order in which those combinations will be done.
         """
 
         if isinstance(superiority, float) and superiority >= 1.0 and \
-                (isinstance(sequence, list) or isinstance(sequence, tuple)) and len(sequence) == 3:
+                (isinstance(sequence, list) or isinstance(sequence, tuple)) and len(sequence) == 4:
             result_attack = {}
             result_defense = {}
             result_no_superiority_defense = {}
             for id in battlesimulation._GGP.types_damage:
                 result_attack.update({id:1.0})
                 result_defense.update({id:1.0})
                 result_no_superiority_defense.update({id:1.0})
@@ -200,14 +249,28 @@
                         for id in result_attack:
                             result_attack[id] *= self.attack_damage_mods[id]
                             result_defense[id] *= self.defense_damage_mods[id]
                             result_no_superiority_defense[id] *= self.defense_damage_mods[id]
                     else:
                         # don't combine damage mods
                         pass
+                elif operation == "elder":
+                    if combination_elder == "add":
+                        for id in result_attack:
+                            result_attack[id] += self.elder_bonus_attack - 1
+                            result_defense[id] += self.elder_bonus_defense - 1
+                            result_no_superiority_defense[id] += self.elder_bonus_defense - 1
+                    elif combination_elder == "multiply":
+                        for id in result_attack:
+                            result_attack[id] *= self.elder_bonus_attack
+                            result_defense[id] *= self.elder_bonus_defense
+                            result_no_superiority_defense[id] *= self.elder_bonus_defense
+                    else:
+                        # don't combine elder bonuses
+                        pass
             for id in result_attack:
                 result_attack[id] = _my_truncate(result_attack[id], truncate_to)
                 if result_attack[id] <= 0:
                     result_attack[id] = 0.000001
                 result_defense[id] = _my_truncate(result_defense[id], truncate_to)
                 result_no_superiority_defense[id] = _my_truncate(result_no_superiority_defense[id], truncate_to)
                 if result_defense[id] <= 0:
```

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/planet.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/planet.py`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/rocket.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/rocket.py`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/spacefleet.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/spacefleet.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         self.incoming_damage_array: DamageArray = None
         # this is for storing turret passive damage to us           DamageArray()
         self.incoming_turrets_damage: DamageArray = None
         # this is for storing shield generator EMP burst damage     DamageArray()
         self.incoming_emp_shield_damage: DamageArray = None
         # this is for my gui module to store this Fleet's leftover damage, dealt to opposite Fleet 2
         self._leftover_damage: DamageArray = None
+        self.coef_cost_of_dead = 1.0
+        self.coef_build_time_of_dead = 1.0
         self._reinit()
 
     def _reinit(self) -> None:
         """Resets SpaceFleet's modules, stored incoming damage arrays and spaceships."""
 
         self._reinit_spaceships()
         self.custom_name = "SpaceFleet"
@@ -539,14 +541,30 @@
         result = 0
         for ss in self:
             if isinstance(ss, Spaceship):
                 result += ss.build_time_of_dead
         return result
 
     @property
+    def antirating(self) -> Union[float,int]:
+        """Antirating of dead spaceships.
+
+            return: result of sum of cost and build time of dead, each multiplied by it's coef (default is 1.0 for both).
+        """
+
+        cost_of_dead = 0
+        build_time_of_dead = 0
+        for ss in self:
+            if isinstance(ss, Spaceship):
+                cost_of_dead += ss.cost_of_dead
+                build_time_of_dead += ss.build_time_of_dead
+
+        return cost_of_dead * self.coef_cost_of_dead + build_time_of_dead * self.coef_build_time_of_dead
+
+    @property
     def filtered_str(self) -> str:
         """Different short string of current spaceships quantities in self."""
 
         text = "Spacefleet: ["
         for ss in self:
             if isinstance(ss, Spaceship):
                 if ss.quantity:
```

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/spaceship.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/spaceship.py`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/components/utility.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/components/utility.py`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/context.py` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -713,14 +713,149 @@
 
         if isinstance(self._fleet_3, SpaceFleet) and isinstance(self._fleet_3.modules, ModuleAndBonuses):
             if (isinstance(data, list) or isinstance(data, tuple)):
                 self._fleet_3.set_module_defense_damage_mods(data)
             elif isinstance(data, dict):
                 self._fleet_3.set_module_defense_damage_mods(data)
 
+    def set_fleet_1_elder_buff_attack(self):
+        """Sets elder attack bonus to 1.5 (+50%)"""
+
+        self._fleet_1.modules.elder_buff_attack()
+
+    def set_fleet_1_elder_debuff_attack(self):
+        """Sets elder attack bonus to 0.5 (-50%)"""
+
+        self._fleet_1.modules.elder_debuff_attack()
+
+    def reset_fleet_1_elder_attack(self):
+        """Sets elder attack bonus to 1.0 (+0%)"""
+
+        self._fleet_1.modules.reset_elder_attack()
+
+    def set_fleet_1_elder_buff_defense(self):
+        """Sets elder defense bonus to 1.5 (+50%)"""
+
+        self._fleet_1.modules.elder_buff_defense()
+
+    def set_fleet_1_elder_debuff_defense(self):
+        """Sets elder defense bonus to 0.5 (-50%)"""
+
+        self._fleet_1.modules.elder_debuff_defense()
+
+    def reset_fleet_1_elder_defense(self):
+        """Sets elder defense bonus to 1.0 (+0%)"""
+
+        self._fleet_1.modules.reset_elder_defense()
+
+    def set_fleet_1_elder_buff_speed(self):
+        """Sets elder speed bonus to 1.5 (+50%)"""
+
+        self._fleet_1.modules.elder_buff_speed()
+
+    def set_fleet_1_elder_debuff_speed(self):
+        """Sets elder speed bonus to 0.5 (-50%)"""
+
+        self._fleet_1.modules.elder_debuff_speed()
+
+    def reset_fleet_1_elder_speed(self):
+        """Sets elder speed bonus to 1.0 (+0%)"""
+
+        self._fleet_1.modules.reset_elder_speed()
+
+    def set_fleet_2_elder_buff_attack(self):
+        """Sets elder attack bonus to 1.5 (+50%)"""
+
+        self._fleet_2.modules.elder_buff_attack()
+
+    def set_fleet_2_elder_debuff_attack(self):
+        """Sets elder attack bonus to 0.5 (-50%)"""
+
+        self._fleet_2.modules.elder_debuff_attack()
+
+    def reset_fleet_2_elder_attack(self):
+        """Sets elder attack bonus to 1.0 (+0%)"""
+
+        self._fleet_2.modules.reset_elder_attack()
+
+    def set_fleet_2_elder_buff_defense(self):
+        """Sets elder defense bonus to 1.5 (+50%)"""
+
+        self._fleet_2.modules.elder_buff_defense()
+
+    def set_fleet_2_elder_debuff_defense(self):
+        """Sets elder defense bonus to 0.5 (-50%)"""
+
+        self._fleet_2.modules.elder_debuff_defense()
+
+    def reset_fleet_2_elder_defense(self):
+        """Sets elder defense bonus to 1.0 (+0%)"""
+
+        self._fleet_2.modules.reset_elder_defense()
+
+    def set_fleet_2_elder_buff_speed(self):
+        """Sets elder speed bonus to 1.5 (+50%)"""
+
+        self._fleet_2.modules.elder_buff_speed()
+
+    def set_fleet_2_elder_debuff_speed(self):
+        """Sets elder speed bonus to 0.5 (-50%)"""
+
+        self._fleet_2.modules.elder_debuff_speed()
+
+    def reset_fleet_2_elder_speed(self):
+        """Sets elder speed bonus to 1.0 (+0%)"""
+
+        self._fleet_2.modules.reset_elder_speed()
+
+    def set_fleet_3_elder_buff_attack(self):
+        """Sets elder attack bonus to 1.5 (+50%)"""
+
+        self._fleet_3.modules.elder_buff_attack()
+
+    def set_fleet_3_elder_debuff_attack(self):
+        """Sets elder attack bonus to 0.5 (-50%)"""
+
+        self._fleet_3.modules.elder_debuff_attack()
+
+    def reset_fleet_3_elder_attack(self):
+        """Sets elder attack bonus to 1.0 (+0%)"""
+
+        self._fleet_3.modules.reset_elder_attack()
+
+    def set_fleet_3_elder_buff_defense(self):
+        """Sets elder defense bonus to 1.5 (+50%)"""
+
+        self._fleet_3.modules.elder_buff_defense()
+
+    def set_fleet_3_elder_debuff_defense(self):
+        """Sets elder defense bonus to 0.5 (-50%)"""
+
+        self._fleet_3.modules.elder_debuff_defense()
+
+    def reset_fleet_3_elder_defense(self):
+        """Sets elder defense bonus to 1.0 (+0%)"""
+
+        self._fleet_3.modules.reset_elder_defense()
+
+    def set_fleet_3_elder_buff_speed(self):
+        """Sets elder speed bonus to 1.5 (+50%)"""
+
+        self._fleet_3.modules.elder_buff_speed()
+
+    def set_fleet_3_elder_debuff_speed(self):
+        """Sets elder speed bonus to 0.5 (-50%)"""
+
+        self._fleet_3.modules.elder_debuff_speed()
+
+    def reset_fleet_3_elder_speed(self):
+        """Sets elder speed bonus to 1.0 (+0%)"""
+
+        self._fleet_3.modules.reset_elder_speed()
+
     def set_planet(self, planet_type: int, planet_size: int, turrets_lvl: int = False) -> None:
         """Sets Planet's mandatory params.
 
             turrets_lvl = False if you are going to set buildings or
             int number = sum of all turrets levels;
 
             planet_type in (1,...,7,9,12,15) and
```

### Comparing `galaxy-online-battle-simulation-1.1.0/src/battlesimulation/data.json` & `galaxy-online-battle-simulation-1.2.0/src/battlesimulation/data.json`

 * *Files identical despite different names*

### Comparing `galaxy-online-battle-simulation-1.1.0/src/galaxy_online_battle_simulation.egg-info/PKG-INFO` & `galaxy-online-battle-simulation-1.2.0/src/galaxy_online_battle_simulation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-online-battle-simulation
-Version: 1.1.0
+Version: 1.2.0
 Summary: Module for simulation of different battles in the online space strategy game Galaxy Online.
 Author: fadedness
 License: The MIT License (MIT)
         Copyright © 2022 fadedness https://t.me/fadedness
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `galaxy-online-battle-simulation-1.1.0/src/galaxy_online_battle_simulation.egg-info/SOURCES.txt` & `galaxy-online-battle-simulation-1.2.0/src/galaxy_online_battle_simulation.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -18,8 +18,17 @@
 src/battlesimulation/components/spacefleet.py
 src/battlesimulation/components/spaceship.py
 src/battlesimulation/components/utility.py
 src/galaxy_online_battle_simulation.egg-info/PKG-INFO
 src/galaxy_online_battle_simulation.egg-info/SOURCES.txt
 src/galaxy_online_battle_simulation.egg-info/dependency_links.txt
 src/galaxy_online_battle_simulation.egg-info/entry_points.txt
-src/galaxy_online_battle_simulation.egg-info/top_level.txt
+src/galaxy_online_battle_simulation.egg-info/top_level.txt
+tests/test_anti_enemy_finder.py
+tests/test_buildings_planet.py
+tests/test_combinations.py
+tests/test_context.py
+tests/test_context_helper.py
+tests/test_custom_data.py
+tests/test_fleet_copy.py
+tests/test_fleet_vs_fleet.py
+tests/test_fleet_vs_rockets.py
```

