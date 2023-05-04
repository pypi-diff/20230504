# Comparing `tmp/tilt-pitch-0.9.1.tar.gz` & `tmp/tilt-pitch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tilt-pitch-0.9.1.tar", last modified: Mon Aug  9 16:24:35 2021, max compression
+gzip compressed data, was "dist/tilt-pitch-1.0.0.tar", last modified: Thu May  4 01:59:09 2023, max compression
```

## Comparing `tilt-pitch-0.9.1.tar` & `tilt-pitch-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16323 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15776 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/pitch/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/pitch/abstractions/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/abstractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/abstractions/cloud_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/pitch/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/configuration/pitch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/pitch/models/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/models/json_serialize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/models/tilt_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     7197 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/pitch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/pitch/providers/
--rw-r--r--   0 runner    (1001) docker     (121)      556 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/brewersfriend_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/brewfather_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/grainfather_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/taplistio_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)      897 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/providers/webhook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/pitch/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2021-08-09 16:24:05.000000 tilt-pitch-0.9.1/test/test_tilt_status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/tilt_pitch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16323 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/tilt_pitch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      912 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/tilt_pitch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/tilt_pitch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/tilt_pitch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-08-09 16:24:35.000000 tilt-pitch-0.9.1/tilt_pitch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/abstractions/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/abstractions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/abstractions/cloud_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/configuration/pitch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/models/json_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/models/tilt_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/pitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/pitch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/azure_iothub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/brewersfriend_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/brewfather_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/grainfather_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/taplistio_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/providers/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/pitch/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-04 01:58:36.000000 tilt-pitch-1.0.0/test/test_tilt_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 01:59:09.000000 tilt-pitch-1.0.0/tilt_pitch.egg-info/top_level.txt
```

### Comparing `tilt-pitch-0.9.1/LICENSE` & `tilt-pitch-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/PKG-INFO` & `tilt-pitch-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilt-pitch
-Version: 0.9.1
+Version: 1.0.0
 Summary: Simple replacement for the Tilt Hydrometer mobile apps and TiltPi with lots of features
 Home-page: https://github.com/linjmeyer/tilt-pitch/
 Author: Lin Meyer
 Author-email: lin@linmeyer.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -81,14 +81,17 @@
 | `influxdb2_bucket` (str) | Bucket to write data to in InfluxDB 2.0 | None/empty | `bucket_name`
 | `influxdb_timeout_seconds` (int) | Timeout of InfluxDB reads/writes | `5` | No example yet (PRs welcome!) |
 | `brewfather_custom_stream_url` (str) | URL of Brewfather Custom Stream | None/empty | No example yet (PRs welcome!) |
 | `grainfather_custom_stream_urls` (dict) | Dict of color (key) and URLs (value) | None/empty | [Example config](examples/grainfather/pitch.json) |
 | `grainfather_temp_unit` (str) | Temperature unit `F` or `C` for Grainfather | `F` |  [Example config](examples/grainfather/pitch.json) |
 | `brewersfriend_api_key` (str) | API Key for Brewer's Friend | None/empty | No example yet (PRs welcome!) |
 | `taplistio_url` (str) | URL of Taplist.io Tilt reporting webhook | None/empty | No example |
+| `azure_iot_hub_connectionstring` (str) | Azure IoT Hub Device Connection String | None/empty | [Example config](examples/azure_iot/readme.md) |
+| `azure_iot_hub_limit_rate` (int) | Rate limit according to selected IoT Hub tier. | 8000 | [Example config](examples/azure_iot/pitch.json) |
+| `azure_iot_hub_limit_period` (int) | Period during which to observe rate limit, defaults to one day. | 86400 | [Example config](examples/azure_iot/pitch.json) |
 | `{color}_name` (str) | Name of your brew, where {color} is the color of the Tilt (purple, red, etc) | Color (e.g. purple, red, etc) | No example yet (PRs welcome!) |
 | `{color}_original_gravity` (float) | Original gravity of the beer, where {color} is the color of the Tilt (purple, red, etc) | None/empty | No example yet (PRs welcome!) |
 | `{color}_temp_offset` (int) | Temperature offset to calibrate Tilt temperatures with a secondary reading [See Calibration](#Calibration) | 0 | No example yet (PRs welcome!) |
 | `{color}_gravity_offset` (float) | Gravity offset to calibrate Tilt temperatures with a secondary reading [See Calibration](#Calibration)  | 0 | No example yet (PRs welcome!) |
 
 ## Rate Limiting and Batching
 
@@ -131,14 +134,15 @@
 * [InfluxDb](#InfluxDB-Metrics)
 * [Webhook](#Webhook)
 * [JSON Log File](#JSON-Log-File)
 * [Brewfather](#Brewfather)
 * [Brewer's Friend](#BrewersFriend)
 * [Grainfather](#Grainfather)
 * [Taplist.io](#taplistio)
+* [Azure IoT Hub](#Azure-IoT-Hub)
 
 Don't see one you want, send a PR implementing [CloudProviderBase](https://github.com/linjmeyer/tilt-pitch/blob/master/pitch/abstractions/cloud_provider.py)
 
 ## Prometheus Metrics
 
 Prometheus metrics are hosted on port 8000 by default.  No rate limiting or batching is used for Prometheus.  
 
@@ -269,14 +273,22 @@
 
 ## Taplist.io
 
 Tilt data can be logged to [Taplist.io](https://taplist.io/) using the Tilt Integration feature.
 
 To setup, log into Taplist.io and visit _Account_ > _Integrations_ > _Tilt Hydrometer_. Copy the _Webhook URL_ value into your Pitch config as `taplistio_url`.
 
+## Azure IoT Hub
+
+Tilt data can be logged as IoT telemetry to Azure IoT hub and processed
+by a variety of services like Event Hubs, Stream Analytics and Power BI.
+
+To set up, follow the instructions at [Microsoft Learn](https://learn.microsoft.com/en-us/azure/iot-hub/iot-hub-create-through-portal)
+to configure the IoT hub and create a new device to receive your Tilt's measurements.
+
 # Examples
 
 See the examples directory for:
 
 * InfluxDB Grafana Dashboard
 * Running Pitch as a systemd service
 * pitch.json configuration file
```

### Comparing `tilt-pitch-0.9.1/README.md` & `tilt-pitch-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 | `influxdb2_bucket` (str) | Bucket to write data to in InfluxDB 2.0 | None/empty | `bucket_name`
 | `influxdb_timeout_seconds` (int) | Timeout of InfluxDB reads/writes | `5` | No example yet (PRs welcome!) |
 | `brewfather_custom_stream_url` (str) | URL of Brewfather Custom Stream | None/empty | No example yet (PRs welcome!) |
 | `grainfather_custom_stream_urls` (dict) | Dict of color (key) and URLs (value) | None/empty | [Example config](examples/grainfather/pitch.json) |
 | `grainfather_temp_unit` (str) | Temperature unit `F` or `C` for Grainfather | `F` |  [Example config](examples/grainfather/pitch.json) |
 | `brewersfriend_api_key` (str) | API Key for Brewer's Friend | None/empty | No example yet (PRs welcome!) |
 | `taplistio_url` (str) | URL of Taplist.io Tilt reporting webhook | None/empty | No example |
+| `azure_iot_hub_connectionstring` (str) | Azure IoT Hub Device Connection String | None/empty | [Example config](examples/azure_iot/readme.md) |
+| `azure_iot_hub_limit_rate` (int) | Rate limit according to selected IoT Hub tier. | 8000 | [Example config](examples/azure_iot/pitch.json) |
+| `azure_iot_hub_limit_period` (int) | Period during which to observe rate limit, defaults to one day. | 86400 | [Example config](examples/azure_iot/pitch.json) |
 | `{color}_name` (str) | Name of your brew, where {color} is the color of the Tilt (purple, red, etc) | Color (e.g. purple, red, etc) | No example yet (PRs welcome!) |
 | `{color}_original_gravity` (float) | Original gravity of the beer, where {color} is the color of the Tilt (purple, red, etc) | None/empty | No example yet (PRs welcome!) |
 | `{color}_temp_offset` (int) | Temperature offset to calibrate Tilt temperatures with a secondary reading [See Calibration](#Calibration) | 0 | No example yet (PRs welcome!) |
 | `{color}_gravity_offset` (float) | Gravity offset to calibrate Tilt temperatures with a secondary reading [See Calibration](#Calibration)  | 0 | No example yet (PRs welcome!) |
 
 ## Rate Limiting and Batching
 
@@ -115,14 +118,15 @@
 * [InfluxDb](#InfluxDB-Metrics)
 * [Webhook](#Webhook)
 * [JSON Log File](#JSON-Log-File)
 * [Brewfather](#Brewfather)
 * [Brewer's Friend](#BrewersFriend)
 * [Grainfather](#Grainfather)
 * [Taplist.io](#taplistio)
+* [Azure IoT Hub](#Azure-IoT-Hub)
 
 Don't see one you want, send a PR implementing [CloudProviderBase](https://github.com/linjmeyer/tilt-pitch/blob/master/pitch/abstractions/cloud_provider.py)
 
 ## Prometheus Metrics
 
 Prometheus metrics are hosted on port 8000 by default.  No rate limiting or batching is used for Prometheus.  
 
@@ -253,14 +257,22 @@
 
 ## Taplist.io
 
 Tilt data can be logged to [Taplist.io](https://taplist.io/) using the Tilt Integration feature.
 
 To setup, log into Taplist.io and visit _Account_ > _Integrations_ > _Tilt Hydrometer_. Copy the _Webhook URL_ value into your Pitch config as `taplistio_url`.
 
+## Azure IoT Hub
+
+Tilt data can be logged as IoT telemetry to Azure IoT hub and processed
+by a variety of services like Event Hubs, Stream Analytics and Power BI.
+
+To set up, follow the instructions at [Microsoft Learn](https://learn.microsoft.com/en-us/azure/iot-hub/iot-hub-create-through-portal)
+to configure the IoT hub and create a new device to receive your Tilt's measurements.
+
 # Examples
 
 See the examples directory for:
 
 * InfluxDB Grafana Dashboard
 * Running Pitch as a systemd service
 * pitch.json configuration file
```

### Comparing `tilt-pitch-0.9.1/pitch/__main__.py` & `tilt-pitch-1.0.0/pitch/__main__.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/configuration/pitch_config.py` & `tilt-pitch-1.0.0/pitch/configuration/pitch_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,18 @@
         self.taplistio_url = None
         # Brewersfriend
         self.brewersfriend_api_key = None
         self.brewersfriend_temp_unit = "F"
         # Grainfather
         self.grainfather_custom_stream_urls = None
         self.grainfather_temp_unit = "F"
+        # Azure IoT Hub
+        self.azure_iot_hub_connectionstring = None
+        self.azure_iot_hub_limit_rate = 8000 # free tier 8000msg per day
+        self.azure_iot_hub_limit_period = 86400 # free tier 8000msg per day
         # Load user inputs from config file
         self.update(data)
 
     def update(self, data: dict):
         self.__dict__.update(data)
 
     def get_original_gravity(self, color: str):
```

### Comparing `tilt-pitch-0.9.1/pitch/models/tilt_status.py` & `tilt-pitch-1.0.0/pitch/models/tilt_status.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/pitch.py` & `tilt-pitch-1.0.0/pitch/pitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
         PrometheusCloudProvider(config),
         FileCloudProvider(config),
         InfluxDbCloudProvider(config),
         InfluxDb2CloudProvider(config),
         BrewfatherCustomStreamCloudProvider(config),
         BrewersFriendCustomStreamCloudProvider(config),
         GrainfatherCustomStreamCloudProvider(config),
-        TaplistIOCloudProvider(config)
+        TaplistIOCloudProvider(config),
+        AzureIoTHubCloudProvider(config)
     ]
 
 # Queue for holding incoming scans
 pitch_q = queue.Queue(maxsize=config.queue_size)
 
 #############################################
 #############################################
```

### Comparing `tilt-pitch-0.9.1/pitch/providers/__init__.py` & `tilt-pitch-1.0.0/pitch/providers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,7 +4,8 @@
 from .influxdb import InfluxDbCloudProvider
 from .influxdb2 import InfluxDb2CloudProvider
 from .brewfather_custom_stream import BrewfatherCustomStreamCloudProvider
 from .brewersfriend_custom_stream import BrewersFriendCustomStreamCloudProvider
 from .calibration import CalibrationCloudProvider
 from .grainfather_custom_stream import GrainfatherCustomStreamCloudProvider
 from .taplistio_custom_stream import TaplistIOCloudProvider
+from .azure_iothub import AzureIoTHubCloudProvider
```

### Comparing `tilt-pitch-0.9.1/pitch/providers/brewersfriend_custom_stream.py` & `tilt-pitch-1.0.0/pitch/providers/brewersfriend_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/providers/brewfather_custom_stream.py` & `tilt-pitch-1.0.0/pitch/providers/brewfather_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/providers/calibration.py` & `tilt-pitch-1.0.0/pitch/providers/calibration.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/providers/file.py` & `tilt-pitch-1.0.0/pitch/providers/file.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/providers/grainfather_custom_stream.py` & `tilt-pitch-1.0.0/pitch/providers/grainfather_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/providers/influxdb.py` & `tilt-pitch-1.0.0/pitch/providers/influxdb.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/providers/influxdb2.py` & `tilt-pitch-1.0.0/pitch/providers/influxdb2.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/providers/prometheus.py` & `tilt-pitch-1.0.0/pitch/providers/prometheus.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/providers/taplistio_custom_stream.py` & `tilt-pitch-1.0.0/pitch/providers/taplistio_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/providers/webhook.py` & `tilt-pitch-1.0.0/pitch/providers/webhook.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/rate_limiter.py` & `tilt-pitch-1.0.0/pitch/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/pitch/setup.py` & `tilt-pitch-1.0.0/pitch/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,17 +19,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: POSIX :: Linux",
     ],
     python_requires='>=3.7',
-    install_requires=[
-        'pybluez',
-        'influxdb',
-        'prometheus_client',
-        'python-interface',
-        'jsonpickle',
-        'beacontools',
-        'pyfiglet'
-    ],
+    install_requires=REQUIREMENTS,
 )
```

### Comparing `tilt-pitch-0.9.1/test/test_tilt_status.py` & `tilt-pitch-1.0.0/test/test_tilt_status.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-0.9.1/tilt_pitch.egg-info/PKG-INFO` & `tilt-pitch-1.0.0/tilt_pitch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilt-pitch
-Version: 0.9.1
+Version: 1.0.0
 Summary: Simple replacement for the Tilt Hydrometer mobile apps and TiltPi with lots of features
 Home-page: https://github.com/linjmeyer/tilt-pitch/
 Author: Lin Meyer
 Author-email: lin@linmeyer.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -81,14 +81,17 @@
 | `influxdb2_bucket` (str) | Bucket to write data to in InfluxDB 2.0 | None/empty | `bucket_name`
 | `influxdb_timeout_seconds` (int) | Timeout of InfluxDB reads/writes | `5` | No example yet (PRs welcome!) |
 | `brewfather_custom_stream_url` (str) | URL of Brewfather Custom Stream | None/empty | No example yet (PRs welcome!) |
 | `grainfather_custom_stream_urls` (dict) | Dict of color (key) and URLs (value) | None/empty | [Example config](examples/grainfather/pitch.json) |
 | `grainfather_temp_unit` (str) | Temperature unit `F` or `C` for Grainfather | `F` |  [Example config](examples/grainfather/pitch.json) |
 | `brewersfriend_api_key` (str) | API Key for Brewer's Friend | None/empty | No example yet (PRs welcome!) |
 | `taplistio_url` (str) | URL of Taplist.io Tilt reporting webhook | None/empty | No example |
+| `azure_iot_hub_connectionstring` (str) | Azure IoT Hub Device Connection String | None/empty | [Example config](examples/azure_iot/readme.md) |
+| `azure_iot_hub_limit_rate` (int) | Rate limit according to selected IoT Hub tier. | 8000 | [Example config](examples/azure_iot/pitch.json) |
+| `azure_iot_hub_limit_period` (int) | Period during which to observe rate limit, defaults to one day. | 86400 | [Example config](examples/azure_iot/pitch.json) |
 | `{color}_name` (str) | Name of your brew, where {color} is the color of the Tilt (purple, red, etc) | Color (e.g. purple, red, etc) | No example yet (PRs welcome!) |
 | `{color}_original_gravity` (float) | Original gravity of the beer, where {color} is the color of the Tilt (purple, red, etc) | None/empty | No example yet (PRs welcome!) |
 | `{color}_temp_offset` (int) | Temperature offset to calibrate Tilt temperatures with a secondary reading [See Calibration](#Calibration) | 0 | No example yet (PRs welcome!) |
 | `{color}_gravity_offset` (float) | Gravity offset to calibrate Tilt temperatures with a secondary reading [See Calibration](#Calibration)  | 0 | No example yet (PRs welcome!) |
 
 ## Rate Limiting and Batching
 
@@ -131,14 +134,15 @@
 * [InfluxDb](#InfluxDB-Metrics)
 * [Webhook](#Webhook)
 * [JSON Log File](#JSON-Log-File)
 * [Brewfather](#Brewfather)
 * [Brewer's Friend](#BrewersFriend)
 * [Grainfather](#Grainfather)
 * [Taplist.io](#taplistio)
+* [Azure IoT Hub](#Azure-IoT-Hub)
 
 Don't see one you want, send a PR implementing [CloudProviderBase](https://github.com/linjmeyer/tilt-pitch/blob/master/pitch/abstractions/cloud_provider.py)
 
 ## Prometheus Metrics
 
 Prometheus metrics are hosted on port 8000 by default.  No rate limiting or batching is used for Prometheus.  
 
@@ -269,14 +273,22 @@
 
 ## Taplist.io
 
 Tilt data can be logged to [Taplist.io](https://taplist.io/) using the Tilt Integration feature.
 
 To setup, log into Taplist.io and visit _Account_ > _Integrations_ > _Tilt Hydrometer_. Copy the _Webhook URL_ value into your Pitch config as `taplistio_url`.
 
+## Azure IoT Hub
+
+Tilt data can be logged as IoT telemetry to Azure IoT hub and processed
+by a variety of services like Event Hubs, Stream Analytics and Power BI.
+
+To set up, follow the instructions at [Microsoft Learn](https://learn.microsoft.com/en-us/azure/iot-hub/iot-hub-create-through-portal)
+to configure the IoT hub and create a new device to receive your Tilt's measurements.
+
 # Examples
 
 See the examples directory for:
 
 * InfluxDB Grafana Dashboard
 * Running Pitch as a systemd service
 * pitch.json configuration file
```

### Comparing `tilt-pitch-0.9.1/tilt_pitch.egg-info/SOURCES.txt` & `tilt-pitch-1.0.0/tilt_pitch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pitch/abstractions/cloud_provider.py
 pitch/configuration/__init__.py
 pitch/configuration/pitch_config.py
 pitch/models/__init__.py
 pitch/models/json_serialize.py
 pitch/models/tilt_status.py
 pitch/providers/__init__.py
+pitch/providers/azure_iothub.py
 pitch/providers/brewersfriend_custom_stream.py
 pitch/providers/brewfather_custom_stream.py
 pitch/providers/calibration.py
 pitch/providers/file.py
 pitch/providers/grainfather_custom_stream.py
 pitch/providers/influxdb.py
 pitch/providers/influxdb2.py
```

