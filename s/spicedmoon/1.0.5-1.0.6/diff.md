# Comparing `tmp/spicedmoon-1.0.5.tar.gz` & `tmp/spicedmoon-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicedmoon-1.0.5.tar", last modified: Thu May  4 13:54:28 2023, max compression
+gzip compressed data, was "spicedmoon-1.0.6.tar", last modified: Thu May  4 14:45:11 2023, max compression
```

## Comparing `spicedmoon-1.0.5.tar` & `spicedmoon-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     1064 2023-05-02 10:46:38.000000 spicedmoon-1.0.5/LICENSE
--rw-rw-r--   0 javgat    (1000) javgat    (1000)        0 2023-05-02 10:46:38.000000 spicedmoon-1.0.5/MANIFEST.in
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/PKG-INFO
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     2948 2023-05-04 13:53:16.000000 spicedmoon-1.0.5/README.md
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      104 2023-05-02 10:46:38.000000 spicedmoon-1.0.5/pyproject.toml
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      804 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/setup.cfg
--rw-rw-r--   0 javgat    (1000) javgat    (1000)       37 2023-05-02 10:46:38.000000 spicedmoon-1.0.5/setup.py
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/src/
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/src/spicedmoon/
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      375 2023-05-04 13:53:58.000000 spicedmoon-1.0.5/src/spicedmoon/__init__.py
--rw-rw-r--   0 javgat    (1000) javgat    (1000)    31192 2023-05-04 13:53:46.000000 spicedmoon-1.0.5/src/spicedmoon/spicedmoon.py
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/src/spicedmoon.egg-info/
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/PKG-INFO
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      308 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/SOURCES.txt
--rw-rw-r--   0 javgat    (1000) javgat    (1000)        1 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/dependency_links.txt
--rw-rw-r--   0 javgat    (1000) javgat    (1000)       30 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/requires.txt
--rw-rw-r--   0 javgat    (1000) javgat    (1000)       11 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/top_level.txt
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 14:45:11.384532 spicedmoon-1.0.6/
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     1064 2023-05-02 10:46:38.000000 spicedmoon-1.0.6/LICENSE
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)        0 2023-05-02 10:46:38.000000 spicedmoon-1.0.6/MANIFEST.in
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 14:45:11.384532 spicedmoon-1.0.6/PKG-INFO
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     2948 2023-05-04 14:44:06.000000 spicedmoon-1.0.6/README.md
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      104 2023-05-02 10:46:38.000000 spicedmoon-1.0.6/pyproject.toml
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      804 2023-05-04 14:45:11.384532 spicedmoon-1.0.6/setup.cfg
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)       37 2023-05-02 10:46:38.000000 spicedmoon-1.0.6/setup.py
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 14:45:11.384532 spicedmoon-1.0.6/src/
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 14:45:11.384532 spicedmoon-1.0.6/src/spicedmoon/
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      375 2023-05-04 13:53:58.000000 spicedmoon-1.0.6/src/spicedmoon/__init__.py
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)    31176 2023-05-04 14:43:18.000000 spicedmoon-1.0.6/src/spicedmoon/spicedmoon.py
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 14:45:11.384532 spicedmoon-1.0.6/src/spicedmoon.egg-info/
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 14:45:11.000000 spicedmoon-1.0.6/src/spicedmoon.egg-info/PKG-INFO
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      308 2023-05-04 14:45:11.000000 spicedmoon-1.0.6/src/spicedmoon.egg-info/SOURCES.txt
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)        1 2023-05-04 14:45:11.000000 spicedmoon-1.0.6/src/spicedmoon.egg-info/dependency_links.txt
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)       30 2023-05-04 14:45:11.000000 spicedmoon-1.0.6/src/spicedmoon.egg-info/requires.txt
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)       11 2023-05-04 14:45:11.000000 spicedmoon-1.0.6/src/spicedmoon.egg-info/top_level.txt
```

### Comparing `spicedmoon-1.0.5/LICENSE` & `spicedmoon-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spicedmoon-1.0.5/PKG-INFO` & `spicedmoon-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spicedmoon
-Version: 1.0.5
+Version: 1.0.6
 Summary: Calculation of lunar data using NASA’s SPICE toolbox.
 Home-page: https://github.com/GOA-UVa/spicedmoon
 Author: Group of Atmospheric Optics (GOA-UVa), Universidad de Valladolid
 Author-email: gaton@goa.uva.es
 Project-URL: Bug Tracker, https://github.com/GOA-UVa/spicedmoon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spicedmoon
 
-![Version 1.0.5](https://img.shields.io/badge/version-1.0.5-informational)
+![Version 1.0.6](https://img.shields.io/badge/version-1.0.6-informational)
 ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
 
 Calculation of lunar data using NASA’s SPICE toolbox.
 
 This data includes:
 - Distance between the Sun and the Moon (in astronomical units)
 - Distance between the Sun and the Moon (in kilometers)
```

### Comparing `spicedmoon-1.0.5/README.md` & `spicedmoon-1.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # spicedmoon
 
-![Version 1.0.5](https://img.shields.io/badge/version-1.0.5-informational)
+![Version 1.0.6](https://img.shields.io/badge/version-1.0.6-informational)
 ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
 
 Calculation of lunar data using NASA’s SPICE toolbox.
 
 This data includes:
 - Distance between the Sun and the Moon (in astronomical units)
 - Distance between the Sun and the Moon (in kilometers)
```

### Comparing `spicedmoon-1.0.5/setup.cfg` & `spicedmoon-1.0.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spicedmoon
-version = 1.0.5
+version = 1.0.6
 author = Group of Atmospheric Optics (GOA-UVa), Universidad de Valladolid
 author_email = gaton@goa.uva.es
 description = Calculation of lunar data using NASA’s SPICE toolbox.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GOA-UVa/spicedmoon
 license_files = LICENSE
```

### Comparing `spicedmoon-1.0.5/src/spicedmoon/spicedmoon.py` & `spicedmoon-1.0.6/src/spicedmoon/spicedmoon.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,23 +267,23 @@
     state, _ = spice.spkezr("MOON", et_date, "MOON_ME", "NONE", "SUN")
     dist_sun_moon_km = math.sqrt(state[0]**2 + state[1]**2 + state[2]**2)
     dist_sun_moon_au = spice.convrt(dist_sun_moon_km, "KM", "AU")
 
 
     limit_lat_rad = math.pi/2
     if lat_sun_rad > limit_lat_rad:
-        lat_sun_rad -= limit_lat_rad*2
+        lat_sun_rad -= limit_lat_rad
     elif lat_sun_rad < -limit_lat_rad:
-        lat_sun_rad += limit_lat_rad*2
+        lat_sun_rad += limit_lat_rad
 
     limit_lon_rad = math.pi
     if lon_sun_rad > limit_lon_rad:
-        lon_sun_rad -= limit_lon_rad*2
+        lon_sun_rad -= limit_lon_rad
     elif lon_sun_rad < -limit_lon_rad:
-        lon_sun_rad += limit_lon_rad*2
+        lon_sun_rad += limit_lon_rad
 
     return MoonSunData(lon_sun_rad, lat_sun_rad, dist_sun_moon_km, dist_sun_moon_au)
 
 
 def _get_moon_data(utc_time: str, observer_name: str = _DEFAULT_OBSERVER_NAME,
                    observer_frame: str = _DEFAULT_OBSERVER_FRAME,
                    observer_zenith_name: str = _DEFAULT_OBSERVER_ZENITH_NAME,
@@ -363,23 +363,23 @@
     smd = _get_sun_moon_data(utc_time)
     lon_sun_rad = smd.lon_sun_rad
     dist_sun_moon_km = smd.dist_sun_moon_km
     dist_sun_moon_au = smd.dist_sun_moon_au
 
     limit_lat = 90
     if lat_obs > limit_lat:
-        lat_obs -= limit_lat*2
+        lat_obs -= limit_lat
     elif lat_obs < -limit_lat:
-        lat_obs += limit_lat*2
+        lat_obs += limit_lat
 
     limit_lon = 180
     if lon_obs > limit_lon:
-        lon_obs -= limit_lon*2
+        lon_obs -= limit_lon
     elif lon_obs < -limit_lon:
-        lon_obs += limit_lon*2
+        lon_obs += limit_lon
 
     moon_data = MoonData(dist_sun_moon_au, dist_sun_moon_km, dist_obs_moon, lon_sun_rad,
                          lat_obs, lon_obs, phase, azimuth, zenith)
     return moon_data
 
 
 def _get_moon_datas_id(utc_times: List[str], kernels_path: str,
```

### Comparing `spicedmoon-1.0.5/src/spicedmoon.egg-info/PKG-INFO` & `spicedmoon-1.0.6/src/spicedmoon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spicedmoon
-Version: 1.0.5
+Version: 1.0.6
 Summary: Calculation of lunar data using NASA’s SPICE toolbox.
 Home-page: https://github.com/GOA-UVa/spicedmoon
 Author: Group of Atmospheric Optics (GOA-UVa), Universidad de Valladolid
 Author-email: gaton@goa.uva.es
 Project-URL: Bug Tracker, https://github.com/GOA-UVa/spicedmoon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spicedmoon
 
-![Version 1.0.5](https://img.shields.io/badge/version-1.0.5-informational)
+![Version 1.0.6](https://img.shields.io/badge/version-1.0.6-informational)
 ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
 
 Calculation of lunar data using NASA’s SPICE toolbox.
 
 This data includes:
 - Distance between the Sun and the Moon (in astronomical units)
 - Distance between the Sun and the Moon (in kilometers)
```

