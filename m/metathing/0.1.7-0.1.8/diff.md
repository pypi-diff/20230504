# Comparing `tmp/metathing-0.1.7.tar.gz` & `tmp/metathing-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metathing-0.1.7.tar", last modified: Wed Apr 13 07:16:31 2022, max compression
+gzip compressed data, was "dist/metathing-0.1.8.tar", last modified: Wed Apr 13 07:21:13 2022, max compression
```

## Comparing `metathing-0.1.7.tar` & `metathing-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:16:31.000000 metathing-0.1.7/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2021-11-28 11:35:16.000000 metathing-0.1.7/LICENSE
--rw-r--r--   0 debian    (1000) debian    (1000)      189 2022-04-13 07:16:31.000000 metathing-0.1.7/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)       86 2021-11-28 11:35:16.000000 metathing-0.1.7/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:16:31.000000 metathing-0.1.7/metathing/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2021-11-13 18:23:50.000000 metathing-0.1.7/metathing/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      290 2021-11-13 18:23:51.000000 metathing-0.1.7/metathing/config.py
--rw-r--r--   0 debian    (1000) debian    (1000)    13692 2022-04-13 07:16:19.000000 metathing-0.1.7/metathing/device.py
--rw-r--r--   0 debian    (1000) debian    (1000)    10829 2021-12-17 09:00:21.000000 metathing-0.1.7/metathing/http.py
--rw-r--r--   0 debian    (1000) debian    (1000)      377 2021-12-15 04:04:47.000000 metathing-0.1.7/metathing/metathing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1787 2021-12-13 14:16:16.000000 metathing-0.1.7/metathing/mqtt.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3797 2022-03-29 00:32:33.000000 metathing-0.1.7/metathing/service.py
--rw-r--r--   0 debian    (1000) debian    (1000)      793 2021-12-13 21:44:36.000000 metathing-0.1.7/metathing/sql.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:16:31.000000 metathing-0.1.7/metathing.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)      189 2022-04-13 07:16:31.000000 metathing-0.1.7/metathing.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)      354 2022-04-13 07:16:31.000000 metathing-0.1.7/metathing.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2022-04-13 07:16:31.000000 metathing-0.1.7/metathing.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       10 2022-04-13 07:16:31.000000 metathing-0.1.7/metathing.egg-info/top_level.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2022-04-13 07:16:31.000000 metathing-0.1.7/setup.cfg
--rw-r--r--   0 debian    (1000) debian    (1000)      235 2022-04-13 07:16:29.000000 metathing-0.1.7/setup.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:16:31.000000 metathing-0.1.7/test/
--rw-r--r--   0 debian    (1000) debian    (1000)      812 2021-11-28 11:35:16.000000 metathing-0.1.7/test/test_basic.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1211 2021-11-28 11:35:16.000000 metathing-0.1.7/test/test_mqtt.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:21:13.000000 metathing-0.1.8/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2021-11-28 11:35:16.000000 metathing-0.1.8/LICENSE
+-rw-r--r--   0 debian    (1000) debian    (1000)      189 2022-04-13 07:21:13.000000 metathing-0.1.8/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)       86 2021-11-28 11:35:16.000000 metathing-0.1.8/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2021-11-13 18:23:50.000000 metathing-0.1.8/metathing/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      290 2021-11-13 18:23:51.000000 metathing-0.1.8/metathing/config.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    13705 2022-04-13 07:20:57.000000 metathing-0.1.8/metathing/device.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    10829 2021-12-17 09:00:21.000000 metathing-0.1.8/metathing/http.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      377 2021-12-15 04:04:47.000000 metathing-0.1.8/metathing/metathing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1787 2021-12-13 14:16:16.000000 metathing-0.1.8/metathing/mqtt.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3797 2022-03-29 00:32:33.000000 metathing-0.1.8/metathing/service.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      793 2021-12-13 21:44:36.000000 metathing-0.1.8/metathing/sql.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)      189 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)      354 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       10 2022-04-13 07:21:13.000000 metathing-0.1.8/metathing.egg-info/top_level.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       38 2022-04-13 07:21:13.000000 metathing-0.1.8/setup.cfg
+-rw-r--r--   0 debian    (1000) debian    (1000)      235 2022-04-13 07:21:09.000000 metathing-0.1.8/setup.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2022-04-13 07:21:13.000000 metathing-0.1.8/test/
+-rw-r--r--   0 debian    (1000) debian    (1000)      812 2021-11-28 11:35:16.000000 metathing-0.1.8/test/test_basic.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1211 2021-11-28 11:35:16.000000 metathing-0.1.8/test/test_mqtt.py
```

### Comparing `metathing-0.1.7/metathing/device.py` & `metathing-0.1.8/metathing/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 class DevProperty(CustomHandler):
     def initialize(self, dev, srv):
         self.dev = dev
         self.srv = srv
 
     def post(self, key: str):
         # self.write(self.dev.ReadProperty(key, content))
-        self.write(str(self.dev.resources[key]))
+        self.write(json.dumps({key:self.dev.resources[key]}))
 
 class DevService(CustomHandler):
     def initialize(self, dev, srv):
         self.dev = dev
         self.srv = srv
         
     def get(self, srv_name: str):
```

### Comparing `metathing-0.1.7/metathing/http.py` & `metathing-0.1.8/metathing/http.py`

 * *Files identical despite different names*

### Comparing `metathing-0.1.7/metathing/mqtt.py` & `metathing-0.1.8/metathing/mqtt.py`

 * *Files identical despite different names*

### Comparing `metathing-0.1.7/metathing/service.py` & `metathing-0.1.8/metathing/service.py`

 * *Files identical despite different names*

### Comparing `metathing-0.1.7/metathing/sql.py` & `metathing-0.1.8/metathing/sql.py`

 * *Files identical despite different names*

### Comparing `metathing-0.1.7/test/test_basic.py` & `metathing-0.1.8/test/test_basic.py`

 * *Files identical despite different names*

### Comparing `metathing-0.1.7/test/test_mqtt.py` & `metathing-0.1.8/test/test_mqtt.py`

 * *Files identical despite different names*

