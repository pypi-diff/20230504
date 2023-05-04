# Comparing `tmp/pyowletapi-2023.5.5.tar.gz` & `tmp/pyowletapi-2023.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyowletapi-2023.5.5.tar", last modified: Wed May  3 15:01:48 2023, max compression
+gzip compressed data, was "pyowletapi-2023.5.7.tar", last modified: Thu May  4 14:42:03 2023, max compression
```

## Comparing `pyowletapi-2023.5.5.tar` & `pyowletapi-2023.5.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 15:01:48.721639 pyowletapi-2023.5.5/
--rw-rw-rw-   0        0        0     2175 2023-05-03 15:01:48.721639 pyowletapi-2023.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     1353 2023-05-02 10:29:46.000000 pyowletapi-2023.5.5/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-05-03 15:01:48.724639 pyowletapi-2023.5.5/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-05-03 15:00:29.000000 pyowletapi-2023.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:01:48.624933 pyowletapi-2023.5.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 15:01:48.651932 pyowletapi-2023.5.5/src/pyowletapi/
--rw-rw-rw-   0        0        0       17 2023-05-02 10:29:46.000000 pyowletapi-2023.5.5/src/pyowletapi/__init__.py
--rw-rw-rw-   0        0        0    10013 2023-05-03 10:53:08.000000 pyowletapi-2023.5.5/src/pyowletapi/api.py
--rw-rw-rw-   0        0        0      318 2023-05-03 10:36:51.000000 pyowletapi-2023.5.5/src/pyowletapi/exceptions.py
--rw-rw-rw-   0        0        0     4281 2023-05-03 14:32:12.000000 pyowletapi-2023.5.5/src/pyowletapi/owlet.py
--rw-rw-rw-   0        0        0     6935 2023-05-02 14:41:49.000000 pyowletapi-2023.5.5/src/pyowletapi/sock.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:01:48.718638 pyowletapi-2023.5.5/src/pyowletapi.egg-info/
--rw-rw-rw-   0        0        0     2175 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 15:01:48.000000 pyowletapi-2023.5.5/src/pyowletapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 14:42:03.823992 pyowletapi-2023.5.7/
+-rw-rw-rw-   0        0        0     2175 2023-05-04 14:42:03.824991 pyowletapi-2023.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1353 2023-05-02 10:29:46.000000 pyowletapi-2023.5.7/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.7/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-05-04 14:42:03.827004 pyowletapi-2023.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-05-04 14:41:59.000000 pyowletapi-2023.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:42:03.720990 pyowletapi-2023.5.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 14:42:03.745989 pyowletapi-2023.5.7/src/pyowletapi/
+-rw-rw-rw-   0        0        0       17 2023-05-02 10:29:46.000000 pyowletapi-2023.5.7/src/pyowletapi/__init__.py
+-rw-rw-rw-   0        0        0    10013 2023-05-04 14:27:41.000000 pyowletapi-2023.5.7/src/pyowletapi/api.py
+-rw-rw-rw-   0        0        0      318 2023-05-03 10:36:51.000000 pyowletapi-2023.5.7/src/pyowletapi/exceptions.py
+-rw-rw-rw-   0        0        0     4281 2023-05-04 14:27:51.000000 pyowletapi-2023.5.7/src/pyowletapi/owlet.py
+-rw-rw-rw-   0        0        0     7347 2023-05-04 14:37:50.000000 pyowletapi-2023.5.7/src/pyowletapi/sock.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:42:03.820990 pyowletapi-2023.5.7/src/pyowletapi.egg-info/
+-rw-rw-rw-   0        0        0     2175 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 14:42:03.000000 pyowletapi-2023.5.7/src/pyowletapi.egg-info/top_level.txt
```

### Comparing `pyowletapi-2023.5.5/PKG-INFO` & `pyowletapi-2023.5.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.5
+Version: 2023.5.7
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
 License: UNKNOWN
 Description: # Introduction
         
         First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
```

### Comparing `pyowletapi-2023.5.5/README.md` & `pyowletapi-2023.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pyowletapi-2023.5.5/setup.py` & `pyowletapi-2023.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
    
     name="pyowletapi",
-    version="2023.05.5",
+    version="2023.05.7",
     description="Owlet baby montior API wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RyanClark123/pyowletapi",
     author="Ryan Clark",
     classifiers=[ 
         "License :: OSI Approved :: MIT License",
```

### Comparing `pyowletapi-2023.5.5/src/pyowletapi/api.py` & `pyowletapi-2023.5.7/src/pyowletapi/api.py`

 * *Files identical despite different names*

### Comparing `pyowletapi-2023.5.5/src/pyowletapi/owlet.py` & `pyowletapi-2023.5.7/src/pyowletapi/owlet.py`

 * *Files identical despite different names*

### Comparing `pyowletapi-2023.5.5/src/pyowletapi/sock.py` & `pyowletapi-2023.5.7/src/pyowletapi/sock.py`

 * *Files 8% similar despite different names*

```diff
@@ -167,24 +167,31 @@
             raw_properties["LOW_BATT_ALRT"]["value"])
         properties['low_heart_rate_alert'] = bool(
             raw_properties["LOW_HR_ALRT"]["value"])
         properties['low_oxygen_alert'] = bool(
             raw_properties["LOW_OX_ALRT"]["value"])
         properties['ppg_log_file'] = bool(
             raw_properties["PPG_LOG_FILE"]["value"])
+        properties['firmware_update_available'] = bool(
+            raw_properties['FW_UPDATE_STATUS']['value'])
+        properties['lost_power_alert'] = bool(
+            raw_properties['LOST_POWER_ALRT']['value'])
+        properties['sock_disconnected'] = bool(
+            raw_properties['SOCK_DISCON_ALRT']['value'])
+        properties['sock_off'] = bool(raw_properties['SOCK_OFF']['value'])
 
         vitals = json.loads(raw_properties["REAL_TIME_VITALS"]["value"])
         properties['oxygen_saturation'] = float(vitals["ox"])
         properties['heart_rate'] = float(vitals["hr"])
         properties['moving'] = bool(vitals["mv"])
         properties['base_station_on'] = True if bool(
             vitals['bso']) or bool(vitals['chg']) else False
         properties['battery_percentage'] = float(vitals["bat"])
         properties['battery_minutes'] = float(vitals["btt"])
-        properties['charging'] = CHARGING_STATUSES[int(vitals['chg'])]
+        properties['charging'] = True if int(vitals['chg']) in [1,2] else False
         properties['signal_strength'] = float(vitals['rsi'])
         properties['last_updated'] = datetime.datetime.strptime(
             raw_properties["REAL_TIME_VITALS"]["data_updated_at"], '%Y-%m-%dT%H:%M:%SZ').strftime("%Y/%m/%d %H:%M:%S")
 
         return properties
 
     async def update_properties(self) -> tuple[dict[str, dict], dict[str:Union[bool, str, float]]]:
```

### Comparing `pyowletapi-2023.5.5/src/pyowletapi.egg-info/PKG-INFO` & `pyowletapi-2023.5.7/src/pyowletapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.5
+Version: 2023.5.7
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
 License: UNKNOWN
 Description: # Introduction
         
         First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
```

