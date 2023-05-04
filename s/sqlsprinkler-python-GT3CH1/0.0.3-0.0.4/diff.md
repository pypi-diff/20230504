# Comparing `tmp/sqlsprinkler-python-GT3CH1-0.0.3.tar.gz` & `tmp/sqlsprinkler-python-GT3CH1-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsprinkler-python-GT3CH1-0.0.3.tar", last modified: Thu May  4 15:49:51 2023, max compression
+gzip compressed data, was "sqlsprinkler-python-GT3CH1-0.0.4.tar", last modified: Thu May  4 17:51:16 2023, max compression
```

## Comparing `sqlsprinkler-python-GT3CH1-0.0.3.tar` & `sqlsprinkler-python-GT3CH1-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:49:51.156944 sqlsprinkler-python-GT3CH1-0.0.3/
--rw-r--r--   0 gcpease  (1709703766) 1389146880     1068 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.3/LICENSE
--rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 15:49:51.157022 sqlsprinkler-python-GT3CH1-0.0.3/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) 1389146880      324 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.3/README.md
--rw-r--r--   0 gcpease  (1709703766) 1389146880       84 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.3/pyproject.toml
--rw-r--r--   0 gcpease  (1709703766) 1389146880      641 2023-05-04 15:49:51.158872 sqlsprinkler-python-GT3CH1-0.0.3/setup.cfg
--rw-r--r--   0 gcpease  (1709703766) 1389146880       68 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.3/setup.py
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:49:51.149325 sqlsprinkler-python-GT3CH1-0.0.3/src/
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:49:51.154189 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/
--rw-r--r--   0 gcpease  (1709703766) 1389146880      107 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/__init__.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880      222 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/api.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     5209 2023-05-04 15:40:49.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/system.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     2407 2023-05-04 15:49:08.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/zone.py
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:49:51.156381 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/
--rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 15:49:51.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) 1389146880      372 2023-05-04 15:49:51.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/SOURCES.txt
--rw-r--r--   0 gcpease  (1709703766) 1389146880        1 2023-05-04 15:49:51.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/dependency_links.txt
--rw-r--r--   0 gcpease  (1709703766) 1389146880       13 2023-05-04 15:49:51.000000 sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/top_level.txt
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 17:51:16.889926 sqlsprinkler-python-GT3CH1-0.0.4/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     1068 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.4/LICENSE
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 17:51:16.890118 sqlsprinkler-python-GT3CH1-0.0.4/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      324 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.4/README.md
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       84 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.4/pyproject.toml
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      641 2023-05-04 17:51:16.892518 sqlsprinkler-python-GT3CH1-0.0.4/setup.cfg
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       68 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.4/setup.py
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 17:51:16.863976 sqlsprinkler-python-GT3CH1-0.0.4/src/
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 17:51:16.880386 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      107 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/__init__.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      222 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/api.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     5505 2023-05-04 17:50:50.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/system.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     3087 2023-05-04 17:50:50.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/zone.py
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 17:51:16.889250 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 17:51:16.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      372 2023-05-04 17:51:16.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/SOURCES.txt
+-rw-r--r--   0 gcpease  (1709703766) 1389146880        1 2023-05-04 17:51:16.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/dependency_links.txt
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       13 2023-05-04 17:51:16.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/top_level.txt
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.3/LICENSE` & `sqlsprinkler-python-GT3CH1-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlsprinkler-python-GT3CH1-0.0.3/PKG-INFO` & `sqlsprinkler-python-GT3CH1-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.3/setup.cfg` & `sqlsprinkler-python-GT3CH1-0.0.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlsprinkler-python-GT3CH1
-version = 0.0.3
+version = 0.0.4
 author = Gavin Pease
 author_email = gavinpease@gmail.com
 description = A python library to control a SQLSprinkler system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GT3CH1/sqlsprinkler_python
 project_urls =
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/system.py` & `sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/system.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,14 +60,28 @@
         """
         Returns the system state.
         :return: The system state.
         """
         self._update_system_state()
         return self.state
 
+    def update(self):
+        """
+        Updates the system.
+        :return: None
+        """
+        self.zones = self._fetch_zones()
+        self._update_system_state()
+
+    def turn_on(self):
+        self.set_system_state(True)
+
+    def turn_off(self):
+        self.set_system_state(False)
+
     def set_system_state(self, state: bool) -> None:
         """
         Sets the system state.
         :param state: The state to set.
         :return: None
         """
         url = "{}/{}".format(self.hostname, API.SYSTEM_STATE_URL)
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler/zone.py` & `sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/zone.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,42 @@
         Turns the zone off.
         :return: None
         """
         self.state = False
         # send request to API_ZONE_URL with ID and state
         requests.put(f"{self.host}/{API.ZONE_URL}", json={"id": self.id, "state": self.state})
 
+    def enable(self):
+        self.enabled = True
+        self.update(self)
+
+    def disable(self):
+        self.enabled = False
+        self.update(self)
+
+    def set_time(self, time: int) -> None:
+        self.time = time
+        self.update(self)
+
+    def set_gpio(self, gpio: int) -> None:
+        self.gpio = gpio
+        self.update(self)
+
+    def set_name(self, name: str) -> None:
+        self.name = name
+        self.update(self)
+
+    def set_auto_off(self, auto_off: bool) -> None:
+        self.auto_off = auto_off
+        self.update(self)
+
+    def set_system_order(self, system_order: int) -> None:
+        self.system_order = system_order
+        self.update(self)
+
     def update_other(self, other) -> None:
         """
         Updates the state of the zone.
         :param other: The zone to update with.
         :return: None
         """
         self.name = other.name
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.3/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO` & `sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

