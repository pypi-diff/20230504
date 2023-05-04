# Comparing `tmp/sqlsprinkler-python-GT3CH1-0.0.2.tar.gz` & `tmp/sqlsprinkler-python-GT3CH1-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsprinkler-python-GT3CH1-0.0.2.tar", last modified: Thu May  4 15:09:57 2023, max compression
+gzip compressed data, was "sqlsprinkler-python-GT3CH1-0.0.3.tar", last modified: Thu May  4 15:49:51 2023, max compression
```

## Comparing `sqlsprinkler-python-GT3CH1-0.0.2.tar` & `sqlsprinkler-python-GT3CH1-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:09:57.715071 sqlsprinkler-python-GT3CH1-0.0.2/
--rw-r--r--   0 gcpease  (1709703766) 1389146880     1068 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.2/LICENSE
--rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 15:09:57.715141 sqlsprinkler-python-GT3CH1-0.0.2/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) 1389146880      324 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.2/README.md
--rw-r--r--   0 gcpease  (1709703766) 1389146880       84 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.2/pyproject.toml
--rw-r--r--   0 gcpease  (1709703766) 1389146880      641 2023-05-04 15:09:57.722363 sqlsprinkler-python-GT3CH1-0.0.2/setup.cfg
--rw-r--r--   0 gcpease  (1709703766) 1389146880       68 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.2/setup.py
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:09:57.702692 sqlsprinkler-python-GT3CH1-0.0.2/src/
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:09:57.709378 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/
--rw-r--r--   0 gcpease  (1709703766) 1389146880      107 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/__init__.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880      222 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/api.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     5282 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/system.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     1975 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/zone.py
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:09:57.714325 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/
--rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 15:09:57.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) 1389146880      372 2023-05-04 15:09:57.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/SOURCES.txt
--rw-r--r--   0 gcpease  (1709703766) 1389146880        1 2023-05-04 15:09:57.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/dependency_links.txt
--rw-r--r--   0 gcpease  (1709703766) 1389146880       13 2023-05-04 15:09:57.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/top_level.txt
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:49:51.156944 sqlsprinkler-python-GT3CH1-0.0.3/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     1068 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.3/LICENSE
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 15:49:51.157022 sqlsprinkler-python-GT3CH1-0.0.3/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      324 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.3/README.md
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       84 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.3/pyproject.toml
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      641 2023-05-04 15:49:51.158872 sqlsprinkler-python-GT3CH1-0.0.3/setup.cfg
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       68 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.3/setup.py
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:49:51.149325 sqlsprinkler-python-GT3CH1-0.0.3/src/
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:49:51.154189 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      107 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/__init__.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      222 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/api.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     5209 2023-05-04 15:40:49.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/system.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     2407 2023-05-04 15:49:08.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/zone.py
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:49:51.156381 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 15:49:51.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      372 2023-05-04 15:49:51.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/SOURCES.txt
+-rw-r--r--   0 gcpease  (1709703766) 1389146880        1 2023-05-04 15:49:51.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/dependency_links.txt
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       13 2023-05-04 15:49:51.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/top_level.txt
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.2/LICENSE` & `sqlsprinkler-python-GT3CH1-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlsprinkler-python-GT3CH1-0.0.2/PKG-INFO` & `sqlsprinkler-python-GT3CH1-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.2/setup.cfg` & `sqlsprinkler-python-GT3CH1-0.0.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlsprinkler-python-GT3CH1
-version = 0.0.2
+version = 0.0.3
 author = Gavin Pease
 author_email = gavinpease@gmail.com
 description = A python library to control a SQLSprinkler system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GT3CH1/sqlsprinkler_python
 project_urls =
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/system.py` & `sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dataclasses import dataclass, field, asdict
 
-from typing import List
-
 import requests
-from sqlsprinkler import API, Zone
+from . import API, Zone
+
 
 class System:
     """ This class represents a SQL Sprinkler system. """
     zones = []
     system_state = False
     hostname = ""
 
@@ -21,20 +20,20 @@
         Gets the zones from the hostname.
         :return: None
         """
         print("Host {}".format(self.hostname))
         self.zones = self.get_zones()
         self.system_state = self.get_system_state()
 
-    def _fetch_zones(self) -> List[Zone]:
+    def _fetch_zones(self) -> [Zone]:
         """
         Fetches the zones from the hostname.
         :return: A list of zones.
         """
-        url = "{}/{}".format(self.hostname,API.ZONE_INFO_URL)
+        url = "{}/{}".format(self.hostname, API.ZONE_INFO_URL)
         print(url)
         request = requests.get(url)
         print(request)
         zone_list = []
         for zone in request.json():
             new_zone = Zone()
             new_zone.host = self.hostname
@@ -45,15 +44,15 @@
             new_zone.auto_off = zone['auto_off']
             new_zone.system_order = zone['system_order']
             new_zone.state = zone['state']
             new_zone.id = zone['id']
             zone_list.append(new_zone)
         return zone_list
 
-    def get_zones(self) -> List[Zone]:
+    def get_zones(self) -> [Zone]:
         """
         Returns the zones in the system.
         :return: A list of zones.
         """
         self.zones = self._fetch_zones()
         return self.zones
 
@@ -67,25 +66,25 @@
 
     def set_system_state(self, state: bool) -> None:
         """
         Sets the system state.
         :param state: The state to set.
         :return: None
         """
-        url = "{}/{}".format(self.hostname,API.SYSTEM_STATE_URL)
+        url = "{}/{}".format(self.hostname, API.SYSTEM_STATE_URL)
         request = requests.put(url, json={"system_enabled": state})
         if request.status_code != 200:
             raise Exception(f"Failed to set system state {state}")
         self._update_system_state()
 
     def _update_system_state(self) -> None:
         """
         Fetches the system state from the hostname.
         """
-        url = "{}/{}".format(self.hostname,API.SYSTEM_STATE_URL)
+        url = "{}/{}".format(self.hostname, API.SYSTEM_STATE_URL)
         print(url)
         request = requests.get(url).json()
         self.state = request["system_enabled"]
 
     def update_zone_state(self, zone_id: int, state: bool) -> None:
         """
         Updates the state of a zone.
@@ -111,20 +110,20 @@
     def add_zone(self, zone: Zone) -> None:
         """
         Adds a zone to the system.
         :param zone: The zone to add.
         :return: None
         """
         zone_to_add = {
-                "Name": zone.name,
-                "GPIO": zone.gpio,
-                "Time": zone.time,
-                "Enabled": zone.enabled,
-                "Autooff": zone.auto_off,
-                }
+            "Name": zone.name,
+            "GPIO": zone.gpio,
+            "Time": zone.time,
+            "Enabled": zone.enabled,
+            "Autooff": zone.auto_off,
+        }
         request = requests.post(f"{self.hostname}/{API.ZONE_URL}", json=zone_to_add)
         if request.status_code != 200:
             raise Exception(f"Failed to add zone {zone}")
         self.zones = self.get_zones()
 
     def delete_zone(self, zone_id: int) -> None:
         """
@@ -144,18 +143,17 @@
         """
         zone_to_update = self.get_zone_by_id(zone.id)
         if zone_to_update is None:
             raise Exception(f"Zone {zone.id} not found")
         zone.update(zone_to_update)
         self.zones = self.get_zones()
 
-    def update_zone_order(self, zone_order: List[int]) -> None:
+    def update_zone_order(self, zone_order: [int]) -> None:
         """
         Updates the order of the zones.
         :param: zone_order: The new order of the zones.
         :return: None
         """
         request = requests.put(f"{self.hostname}/{API.ZONE_ORDER_URL}", json={"order": zone_order})
         if request.status_code != 200:
             raise Exception(f"Failed to update zone order {zone_order}")
         self.zones = self.get_zones()
-
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/zone.py` & `sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/zone.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from dataclasses import field, dataclass
 
 import requests
-from sqlsprinkler import API
+from . import API
+
+
 @dataclass
 class Zone:
     """ This class represents a SQL Sprinkler zone. """
     host = "none"
     name: str = field(default_factory=str)
     gpio: int = field(default_factory=int)
     time: int = field(default_factory=int)
@@ -30,15 +32,15 @@
         Turns the zone off.
         :return: None
         """
         self.state = False
         # send request to API_ZONE_URL with ID and state
         requests.put(f"{self.host}/{API.ZONE_URL}", json={"id": self.id, "state": self.state})
 
-    def update(self, other) -> None:
+    def update_other(self, other) -> None:
         """
         Updates the state of the zone.
         :param other: The zone to update with.
         :return: None
         """
         self.name = other.name
         self.gpio = other.gpio
@@ -54,7 +56,20 @@
             "gpio": self.gpio,
             "time": self.time,
             "enabled": self.enabled,
             "auto_off": self.auto_off,
             "system_order": self.system_order
         }
         requests.put(f"{self.host}/{API.ZONE_UPDATE_URL}", json=zone_json)
+
+    def update(self) -> None:
+        url = "{}/{}/{}".format(self.host, API.ZONE_INFO_URL, self.id)
+        print(url)
+        req = requests.get(url).json()
+        print(req)
+        self.name = req['name']
+        self.gpio = req['gpio']
+        self.time = req['time']
+        self.enabled = req['enabled']
+        self.auto_off = req['auto_off']
+        self.system_order = req['system_order']
+        self.state = req['state']
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO` & `sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

