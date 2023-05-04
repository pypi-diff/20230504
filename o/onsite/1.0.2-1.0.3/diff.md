# Comparing `tmp/onsite-1.0.2.tar.gz` & `tmp/onsite-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onsite-1.0.2.tar", last modified: Thu Mar 30 06:26:08 2023, max compression
+gzip compressed data, was "onsite-1.0.3.tar", last modified: Thu May  4 05:22:44 2023, max compression
```

## Comparing `onsite-1.0.2.tar` & `onsite-1.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 06:26:08.380682 onsite-1.0.2/
--rw-rw-rw-   0        0        0     1094 2023-03-30 06:19:01.000000 onsite-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1938 2023-03-30 06:26:08.380682 onsite-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1534 2023-03-30 06:25:25.000000 onsite-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 06:26:08.297682 onsite-1.0.2/onsite/
--rw-rw-rw-   0        0        0        0 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/__init__.py
--rw-rw-rw-   0        0        0    24761 2023-03-30 06:19:12.000000 onsite-1.0.2/onsite/controller.py
--rw-rw-rw-   0        0        0     1833 2023-03-30 06:19:12.000000 onsite-1.0.2/onsite/env.py
--rw-rw-rw-   0        0        0     1329 2023-03-30 06:19:12.000000 onsite-1.0.2/onsite/observation.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:26:08.329681 onsite-1.0.2/onsite/opendrive2discretenet/
--rw-rw-rw-   0        0        0        0 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/__init__.py
--rw-rw-rw-   0        0        0    11497 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/converter.py
--rw-rw-rw-   0        0        0     2782 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/discrete_network.py
--rw-rw-rw-   0        0        0    18735 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/network.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:26:08.335682 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/
--rw-rw-rw-   0        0        0        0 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:26:08.367684 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/
--rw-rw-rw-   0        0        0        0 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/__init__.py
--rw-rw-rw-   0        0        0     2211 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/eulerspiral.py
--rw-rw-rw-   0        0        0     8552 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/geometry.py
--rw-rw-rw-   0        0        0     4115 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/junction.py
--rw-rw-rw-   0        0        0     2391 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/opendrive.py
--rw-rw-rw-   0        0        0     3417 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/road.py
--rw-rw-rw-   0        0        0      604 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadElevationProfile.py
--rw-rw-rw-   0        0        0     8581 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadLanes.py
--rw-rw-rw-   0        0        0     3755 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadLateralProfile.py
--rw-rw-rw-   0        0        0     5397 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadLink.py
--rw-rw-rw-   0        0        0     9660 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadPlanView.py
--rw-rw-rw-   0        0        0     1327 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/road_record.py
--rw-rw-rw-   0        0        0     2163 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadtype.py
--rw-rw-rw-   0        0        0    26573 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/parser.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:26:08.379682 onsite-1.0.2/onsite/opendrive2discretenet/plane_elements/
--rw-rw-rw-   0        0        0        0 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/plane_elements/__init__.py
--rw-rw-rw-   0        0        0     3896 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/plane_elements/border.py
--rw-rw-rw-   0        0        0     9672 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/plane_elements/plane.py
--rw-rw-rw-   0        0        0    11525 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/plane_elements/plane_group.py
--rw-rw-rw-   0        0        0      835 2023-03-30 06:19:01.000000 onsite-1.0.2/onsite/opendrive2discretenet/utils.py
--rw-rw-rw-   0        0        0     4373 2023-03-30 06:19:12.000000 onsite-1.0.2/onsite/recorder.py
--rw-rw-rw-   0        0        0     4063 2023-03-30 06:19:12.000000 onsite-1.0.2/onsite/scenarioOrganizer.py
--rw-rw-rw-   0        0        0    11914 2023-03-30 06:24:19.000000 onsite-1.0.2/onsite/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-03-30 06:26:08.317684 onsite-1.0.2/onsite.egg-info/
--rw-rw-rw-   0        0        0     1938 2023-03-30 06:26:08.000000 onsite-1.0.2/onsite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2023-03-30 06:26:08.000000 onsite-1.0.2/onsite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 06:26:08.000000 onsite-1.0.2/onsite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-03-30 06:26:08.000000 onsite-1.0.2/onsite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-30 06:26:08.000000 onsite-1.0.2/onsite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 06:26:08.380682 onsite-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-03-30 06:25:16.000000 onsite-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.260293 onsite-1.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-04-27 06:03:34.000000 onsite-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1999 2023-05-04 05:22:44.259294 onsite-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1595 2023-05-04 05:10:32.000000 onsite-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.223294 onsite-1.0.3/onsite/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/__init__.py
+-rw-rw-rw-   0        0        0    24362 2023-04-27 08:29:11.000000 onsite-1.0.3/onsite/controller.py
+-rw-rw-rw-   0        0        0     1833 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/env.py
+-rw-rw-rw-   0        0        0     1329 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/observation.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.240293 onsite-1.0.3/onsite/opendrive2discretenet/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/__init__.py
+-rw-rw-rw-   0        0        0    11497 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/converter.py
+-rw-rw-rw-   0        0        0     2782 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/discrete_network.py
+-rw-rw-rw-   0        0        0    18735 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/network.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.243294 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.255294 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/__init__.py
+-rw-rw-rw-   0        0        0     2211 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/eulerspiral.py
+-rw-rw-rw-   0        0        0     8552 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/geometry.py
+-rw-rw-rw-   0        0        0     4115 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/junction.py
+-rw-rw-rw-   0        0        0     2391 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/opendrive.py
+-rw-rw-rw-   0        0        0     3417 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/road.py
+-rw-rw-rw-   0        0        0      604 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadElevationProfile.py
+-rw-rw-rw-   0        0        0     8581 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLanes.py
+-rw-rw-rw-   0        0        0     3755 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLateralProfile.py
+-rw-rw-rw-   0        0        0     5397 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLink.py
+-rw-rw-rw-   0        0        0     9660 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadPlanView.py
+-rw-rw-rw-   0        0        0     1327 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/road_record.py
+-rw-rw-rw-   0        0        0     2163 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadtype.py
+-rw-rw-rw-   0        0        0    26573 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.259294 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/
+-rw-rw-rw-   0        0        0        0 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/__init__.py
+-rw-rw-rw-   0        0        0     3896 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/border.py
+-rw-rw-rw-   0        0        0     9672 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/plane.py
+-rw-rw-rw-   0        0        0    11525 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/plane_group.py
+-rw-rw-rw-   0        0        0      835 2023-04-27 06:03:34.000000 onsite-1.0.3/onsite/opendrive2discretenet/utils.py
+-rw-rw-rw-   0        0        0     4373 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/recorder.py
+-rw-rw-rw-   0        0        0     4063 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/scenarioOrganizer.py
+-rw-rw-rw-   0        0        0    11914 2023-04-27 06:04:56.000000 onsite-1.0.3/onsite/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:22:44.236294 onsite-1.0.3/onsite.egg-info/
+-rw-rw-rw-   0        0        0     1999 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1755 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 05:22:44.000000 onsite-1.0.3/onsite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 05:22:44.260293 onsite-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-05-04 05:10:59.000000 onsite-1.0.3/setup.py
```

### Comparing `onsite-1.0.2/LICENSE.txt` & `onsite-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/PKG-INFO` & `onsite-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: onsite
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool package for Onsite
 Home-page: https://gitee.com/huangyansmile/onsite-public
 Author: Huang Yan
 Author-email: huangyan520@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## 架构
 
 
 ## 更新说明
+- Version 1.0.3
+
+    比赛正式版，修复若干bug.
+
 - Version 1.0.2
 
     比赛正式版，修复若干bug.
 
 - Version 0.3.3
 
     稳定版，删除没有用的库.
```

### Comparing `onsite-1.0.2/README.md` & `onsite-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ## 架构
 
 
 ## 更新说明
+- Version 1.0.3
+
+    比赛正式版，修复若干bug.
+
 - Version 1.0.2
 
     比赛正式版，修复若干bug.
 
 - Version 0.3.3
 
     稳定版，删除没有用的库.
```

### Comparing `onsite-1.0.2/onsite/controller.py` & `onsite-1.0.3/onsite/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import os
 import xml.dom.minidom
 from lxml import etree
 import json
 import re
 import numpy as np
 import copy
-from shapely.ops import unary_union
 from shapely.geometry import Polygon
 from itertools import combinations
 
 
 class ReplayInfo():
     """用于存储回放测试中用以控制背景车辆的所有数据
         背景车轨迹信息 vehicle_traj
@@ -321,15 +320,15 @@
         new_observation = self._update_end_status(new_observation)
         if self.control_info.light_info:
             new_observation = self._update_light_info_to_t(new_observation)
         return new_observation
 
     def _action_cheaker(self, action):
         a = np.clip(action[0], -15, 15)
-        rad = np.clip(action[1], -0.2, 0.2)
+        rad = np.clip(action[1], -1, 1)
         return (a, rad)
 
     def _get_initial_observation(self) -> Observation:
         observation = Observation()
         # vehicle_info
         observation.vehicle_info["ego"] = self.control_info.ego_info
         observation = self._update_other_vehicles_to_t(observation)
@@ -453,26 +452,21 @@
         # 当测试时间大于0.5秒时，遍历所有车辆，绘制对应的多边形。这是因为数据问题，有些车辆在初始位置有重叠。也就是说0.5s以内不会判断是否碰撞。
         if observation.test_setting['t'] > 0.5:
             for index, vehi in observation.vehicle_info.items():
                 self.vehicle_index += [index]
                 poly_zip += [self._get_poly(vehi)]
 
         # 检测主车是否与背景车碰撞
-        self.graphics_dictionary = {}  # key为元组，用来存放两碰撞车辆的名称，values为两图形相交面积
         for a, b in combinations(poly_zip, 2):
             if self.vehicle_index[poly_zip.index(a)] == 'ego' or self.vehicle_index[poly_zip.index(b)] == 'ego':
-                self.graphics_dictionary[(poly_zip.index(a), poly_zip.index(b))] = a.intersection(b)
-        intersection_list = list(self.graphics_dictionary.values())
-        intersection = unary_union(intersection_list).area
-
-        # 如果并集面积>0，发生碰撞
-        if intersection > 0:
-            return True
-        else:
-            return False
+                if a.intersects(b):
+                    return True
+                else:
+                    continue
+        return False
 
     def _get_poly(self, vehicle: dict) -> Polygon:
         """根据车辆信息,通过shapely库绘制矩形。
 
         这是为了方便地使用shapely库判断场景中的车辆是否发生碰撞
         """
         # 从字典中取出数据，方便后续处理
```

### Comparing `onsite-1.0.2/onsite/env.py` & `onsite-1.0.3/onsite/env.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/observation.py` & `onsite-1.0.3/onsite/observation.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/converter.py` & `onsite-1.0.3/onsite/opendrive2discretenet/converter.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/discrete_network.py` & `onsite-1.0.3/onsite/opendrive2discretenet/discrete_network.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/network.py` & `onsite-1.0.3/onsite/opendrive2discretenet/network.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/eulerspiral.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/eulerspiral.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/geometry.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/geometry.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/junction.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/junction.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/opendrive.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/opendrive.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/road.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/road.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadElevationProfile.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadElevationProfile.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadLanes.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLanes.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadLateralProfile.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLateralProfile.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadLink.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadLink.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadPlanView.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadPlanView.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/road_record.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/road_record.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/elements/roadtype.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/elements/roadtype.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/opendriveparser/parser.py` & `onsite-1.0.3/onsite/opendrive2discretenet/opendriveparser/parser.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/plane_elements/border.py` & `onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/border.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/plane_elements/plane.py` & `onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/plane.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/plane_elements/plane_group.py` & `onsite-1.0.3/onsite/opendrive2discretenet/plane_elements/plane_group.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/opendrive2discretenet/utils.py` & `onsite-1.0.3/onsite/opendrive2discretenet/utils.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/recorder.py` & `onsite-1.0.3/onsite/recorder.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/scenarioOrganizer.py` & `onsite-1.0.3/onsite/scenarioOrganizer.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite/visualizer.py` & `onsite-1.0.3/onsite/visualizer.py`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/onsite.egg-info/PKG-INFO` & `onsite-1.0.3/onsite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: onsite
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool package for Onsite
 Home-page: https://gitee.com/huangyansmile/onsite-public
 Author: Huang Yan
 Author-email: huangyan520@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## 架构
 
 
 ## 更新说明
+- Version 1.0.3
+
+    比赛正式版，修复若干bug.
+
 - Version 1.0.2
 
     比赛正式版，修复若干bug.
 
 - Version 0.3.3
 
     稳定版，删除没有用的库.
```

### Comparing `onsite-1.0.2/onsite.egg-info/SOURCES.txt` & `onsite-1.0.3/onsite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onsite-1.0.2/setup.py` & `onsite-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="onsite", 
-    version="1.0.2",
+    version="1.0.3",
     author="Huang Yan",   
     author_email="huangyan520@tongji.edu.cn",   
     description="A tool package for Onsite",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitee.com/huangyansmile/onsite-public", 
     packages=setuptools.find_packages(),
```

