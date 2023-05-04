# Comparing `tmp/tilt-pitch-1.0.0.tar.gz` & `tmp/tilt-pitch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tilt-pitch-1.0.0.tar", last modified: Thu May  4 01:59:09 2023, max compression
+gzip compressed data, was "dist/tilt-pitch-1.0.1.tar", last modified: Thu May  4 02:14:36 2023, max compression
```

## Comparing `tilt-pitch-1.0.0.tar` & `tilt-pitch-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/abstractions/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/abstractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/abstractions/cloud_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/configuration/pitch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/models/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/models/json_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/models/tilt_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/pitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/azure_iothub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/brewersfriend_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/brewfather_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/grainfather_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/taplistio_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/test/test_tilt_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/pitch/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/pitch/abstractions/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/abstractions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/abstractions/cloud_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/pitch/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/configuration/pitch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/pitch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/models/json_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/models/tilt_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/pitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/pitch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/azure_iothub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/brewersfriend_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/brewfather_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/grainfather_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/taplistio_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/providers/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/pitch/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-04 02:14:08.000000 tilt-pitch-1.0.1/test/test_tilt_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/tilt_pitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/tilt_pitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/tilt_pitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/tilt_pitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/tilt_pitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 02:14:36.000000 tilt-pitch-1.0.1/tilt_pitch.egg-info/top_level.txt
```

### Comparing `tilt-pitch-1.0.0/LICENSE` & `tilt-pitch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/PKG-INFO` & `tilt-pitch-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilt-pitch
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple replacement for the Tilt Hydrometer mobile apps and TiltPi with lots of features
 Home-page: https://github.com/linjmeyer/tilt-pitch/
 Author: Lin Meyer
 Author-email: lin@linmeyer.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tilt-pitch-1.0.0/README.md` & `tilt-pitch-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/__main__.py` & `tilt-pitch-1.0.1/pitch/__main__.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/configuration/pitch_config.py` & `tilt-pitch-1.0.1/pitch/configuration/pitch_config.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/models/tilt_status.py` & `tilt-pitch-1.0.1/pitch/models/tilt_status.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/pitch.py` & `tilt-pitch-1.0.1/pitch/pitch.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/__init__.py` & `tilt-pitch-1.0.1/pitch/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/azure_iothub.py` & `tilt-pitch-1.0.1/pitch/providers/azure_iothub.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class AzureIoTHubCloudProvider(implements(CloudProviderBase)):
 
     def __init__(self, config: PitchConfig):
         self.config = config
         self.str_name = "Azure IoT Hub ({})".format(config.azure_iot_hub_connectionstring)
         self.rate_limiter = DeviceRateLimiter(rate=config.azure_iot_hub_limit_rate, period=config.azure_iot_hub_limit_period)
+
     def __str__(self):
         return self.str_name
 
     def start(self):
         pass
 
     async def send(self, tilt_status: TiltStatus):        
@@ -31,8 +32,9 @@
             print(f"Could not connect to IoT Hub: {e}.")
 
     def update(self, tilt_status: TiltStatus):
         self.rate_limiter.approve(tilt_status.color)
         asyncio.run(self.send(tilt_status))
 
     def enabled(self):
-        return True
+        enabled = True if self.config.azure_iot_hub_connectionstring else False
+        return enabled
```

### Comparing `tilt-pitch-1.0.0/pitch/providers/brewersfriend_custom_stream.py` & `tilt-pitch-1.0.1/pitch/providers/brewersfriend_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/brewfather_custom_stream.py` & `tilt-pitch-1.0.1/pitch/providers/brewfather_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/calibration.py` & `tilt-pitch-1.0.1/pitch/providers/calibration.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/file.py` & `tilt-pitch-1.0.1/pitch/providers/file.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/grainfather_custom_stream.py` & `tilt-pitch-1.0.1/pitch/providers/grainfather_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/influxdb.py` & `tilt-pitch-1.0.1/pitch/providers/influxdb.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/influxdb2.py` & `tilt-pitch-1.0.1/pitch/providers/influxdb2.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/prometheus.py` & `tilt-pitch-1.0.1/pitch/providers/prometheus.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/taplistio_custom_stream.py` & `tilt-pitch-1.0.1/pitch/providers/taplistio_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/providers/webhook.py` & `tilt-pitch-1.0.1/pitch/providers/webhook.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/rate_limiter.py` & `tilt-pitch-1.0.1/pitch/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/pitch/setup.py` & `tilt-pitch-1.0.1/pitch/setup.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/test/test_tilt_status.py` & `tilt-pitch-1.0.1/test/test_tilt_status.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.0/tilt_pitch.egg-info/PKG-INFO` & `tilt-pitch-1.0.1/tilt_pitch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilt-pitch
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple replacement for the Tilt Hydrometer mobile apps and TiltPi with lots of features
 Home-page: https://github.com/linjmeyer/tilt-pitch/
 Author: Lin Meyer
 Author-email: lin@linmeyer.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tilt-pitch-1.0.0/tilt_pitch.egg-info/SOURCES.txt` & `tilt-pitch-1.0.1/tilt_pitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

