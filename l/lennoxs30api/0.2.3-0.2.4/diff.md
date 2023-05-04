# Comparing `tmp/lennoxs30api-0.2.3.tar.gz` & `tmp/lennoxs30api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lennoxs30api-0.2.3.tar", last modified: Sun Apr 23 15:05:41 2023, max compression
+gzip compressed data, was "lennoxs30api-0.2.4.tar", last modified: Thu May  4 15:42:42 2023, max compression
```

## Comparing `lennoxs30api-0.2.3.tar` & `lennoxs30api-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-23 15:05:41.034974 lennoxs30api-0.2.3/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.3/LICENSE
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-04-23 15:05:41.032972 lennoxs30api-0.2.3/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.3/README.md
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-23 15:05:40.936972 lennoxs30api-0.2.3/lennoxs30api/
--rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/__init__.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     3188 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_ble.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_equipment.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_errors.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_home.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_period.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.3/lennoxs30api/lennox_schedule.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.3/lennoxs30api/message_logger.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     3903 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/metrics.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)   128419 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/s30api_async.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.3/lennoxs30api/s30exception.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2414 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/lennoxs30api/subscriber_base.py
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-04-23 15:05:41.015972 lennoxs30api-0.2.3/lennoxs30api.egg-info/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)      555 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/SOURCES.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/dependency_links.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/requires.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-04-23 15:05:40.000000 lennoxs30api-0.2.3/lennoxs30api.egg-info/top_level.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-04-23 15:05:41.035977 lennoxs30api-0.2.3/setup.cfg
--rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-04-23 14:36:07.000000 lennoxs30api-0.2.3/setup.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-05-04 15:42:42.388599 lennoxs30api-0.2.4/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.4/LICENSE
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-05-04 15:42:42.385604 lennoxs30api-0.2.4/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.4/README.md
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-05-04 15:42:42.305001 lennoxs30api-0.2.4/lennoxs30api/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-05-04 15:39:18.000000 lennoxs30api-0.2.4/lennoxs30api/__init__.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     3188 2023-04-23 14:36:07.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_ble.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_equipment.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_errors.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_home.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_period.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_schedule.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.4/lennoxs30api/message_logger.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     3903 2023-04-23 14:36:07.000000 lennoxs30api-0.2.4/lennoxs30api/metrics.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)   129341 2023-05-04 15:33:30.000000 lennoxs30api-0.2.4/lennoxs30api/s30api_async.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.4/lennoxs30api/s30exception.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2414 2023-04-23 14:36:07.000000 lennoxs30api-0.2.4/lennoxs30api/subscriber_base.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-05-04 15:42:42.368599 lennoxs30api-0.2.4/lennoxs30api.egg-info/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      555 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/requires.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/top_level.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-05-04 15:42:42.389602 lennoxs30api-0.2.4/setup.cfg
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-05-04 15:39:24.000000 lennoxs30api-0.2.4/setup.py
```

### Comparing `lennoxs30api-0.2.3/LICENSE` & `lennoxs30api-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/PKG-INFO` & `lennoxs30api-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.3
+Version: 0.2.4
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.3/README.md` & `lennoxs30api-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/lennox_ble.py` & `lennoxs30api-0.2.4/lennoxs30api/lennox_ble.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/lennox_equipment.py` & `lennoxs30api-0.2.4/lennoxs30api/lennox_equipment.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/lennox_errors.py` & `lennoxs30api-0.2.4/lennoxs30api/lennox_errors.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/lennox_home.py` & `lennoxs30api-0.2.4/lennoxs30api/lennox_home.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/lennox_period.py` & `lennoxs30api-0.2.4/lennoxs30api/lennox_period.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/lennox_schedule.py` & `lennoxs30api-0.2.4/lennoxs30api/lennox_schedule.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/message_logger.py` & `lennoxs30api-0.2.4/lennoxs30api/message_logger.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/metrics.py` & `lennoxs30api-0.2.4/lennoxs30api/metrics.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/s30api_async.py` & `lennoxs30api-0.2.4/lennoxs30api/s30api_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,16 @@
     LENNOX_DEHUMIDIFICATION_MODE_HIGH,
     LENNOX_DEHUMIDIFICATION_MODE_AUTO,
 }
 
 
 LENNOX_FEATURE_UNIT_MODEL_NUMBER: Final = 6
 LENNOX_FEATURE_UNIT_SERIAL_NUMBER: Final = 7
+LENNOX_FEATURE_CONTROL_MODEL_NUMBER: Final = 8
+LENNOX_FEATURE_CONTROL_SERIAL_NUMBER: Final = 9
 LENNOX_FEATURE_EQUIPMENT_TYPE_NAME: Final = 15
 
 LENNOX_PARAMETER_EQUIPMENT_NAME: Final = 18
 LENNOX_PARAMETER_SINGLE_SETPOINT_MODE: Final = 525
 
 LENNOX_EQUIPMENT_TYPE_SUBNET_CONTROLLER: Final = 0
 LENNOX_EQUIPMENT_TYPE_FURNACE: Final = 16
@@ -1501,20 +1503,28 @@
                 eq_equipment = equipment["equipment"]
                 if "equipType" in eq_equipment:
                     eq.equipType = eq_equipment["equipType"]
             for feature in equipment.get("equipment", {}).get("features", []):
                 if feature.get("feature", {}).get("fid") == LENNOX_FEATURE_EQUIPMENT_TYPE_NAME:
                     if "values" in feature["feature"]:
                         eq.equipment_type_name = feature["feature"]["values"][0]["value"]
-                if feature.get("feature", {}).get("fid") == LENNOX_FEATURE_UNIT_MODEL_NUMBER:
-                    if "values" in feature["feature"]:
-                        eq.unit_model_number = feature["feature"]["values"][0]["value"]
-                if feature.get("feature", {}).get("fid") == LENNOX_FEATURE_UNIT_SERIAL_NUMBER:
-                    if "values" in feature["feature"]:
-                        eq.unit_serial_number = feature["feature"]["values"][0]["value"]
+                if equipment_id == 0:
+                    if feature.get("feature", {}).get("fid") == LENNOX_FEATURE_CONTROL_MODEL_NUMBER:
+                        if "values" in feature["feature"]:
+                            eq.unit_model_number = feature["feature"]["values"][0]["value"]
+                    if feature.get("feature", {}).get("fid") == LENNOX_FEATURE_CONTROL_SERIAL_NUMBER:
+                        if "values" in feature["feature"]:
+                            eq.unit_serial_number = feature["feature"]["values"][0]["value"]
+                else:
+                    if feature.get("feature", {}).get("fid") == LENNOX_FEATURE_UNIT_MODEL_NUMBER:
+                        if "values" in feature["feature"]:
+                            eq.unit_model_number = feature["feature"]["values"][0]["value"]
+                    if feature.get("feature", {}).get("fid") == LENNOX_FEATURE_UNIT_SERIAL_NUMBER:
+                        if "values" in feature["feature"]:
+                            eq.unit_serial_number = feature["feature"]["values"][0]["value"]
             for parameter in equipment.get("equipment", {}).get("parameters", []):
                 # 525 is the parameter id for split-setpoint
                 if parameter.get("parameter", {}).get("pid") == LENNOX_PARAMETER_SINGLE_SETPOINT_MODE:
                     value = parameter["parameter"]["value"]
                     if value == 1 or value == "1":
                         self.single_setpoint_mode = True
                     else:
@@ -1576,15 +1586,19 @@
         return False
 
     @property
     def unique_id(self) -> str:
         # This returns a unique identifier.  When connected ot the cloud we use the sysid which is a GUID; when
         # connected to the LAN the sysid is alway "LCC" - which is not unique - so in this case we use the device serial number.
         if self.sysId == "LCC":
-            return self.serialNumber
+            # The S40 no longer populates the serial number, so get it from the unit_serial_number
+            if self.productType == "S40":
+                return self.equipment[0].unit_serial_number
+            else:
+                return self.serialNumber
         return self.sysId
 
     def config_complete(self) -> bool:
         if self.name is None:
             return False
         if self.api.isLANConnection and self.serialNumber is None:
             return False
```

### Comparing `lennoxs30api-0.2.3/lennoxs30api/s30exception.py` & `lennoxs30api-0.2.4/lennoxs30api/s30exception.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api/subscriber_base.py` & `lennoxs30api-0.2.4/lennoxs30api/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/lennoxs30api.egg-info/PKG-INFO` & `lennoxs30api-0.2.4/lennoxs30api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.3
+Version: 0.2.4
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.3/lennoxs30api.egg-info/SOURCES.txt` & `lennoxs30api-0.2.4/lennoxs30api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.3/setup.py` & `lennoxs30api-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lennoxs30api",
-    version="0.2.3",
+    version="0.2.4",
     description="API Wrapper for Lennox S30 Cloud and LAN API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PeteRager/lennoxs30api",
     author="Pete Rage",
     author_email="pete.rager@x.com",
     license="MIT",
```

