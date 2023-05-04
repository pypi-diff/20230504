# Comparing `tmp/spicedmoon-1.0.3.tar.gz` & `tmp/spicedmoon-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicedmoon-1.0.3.tar", last modified: Thu Sep  1 10:16:27 2022, max compression
+gzip compressed data, was "spicedmoon-1.0.4.tar", last modified: Thu May  4 11:55:11 2023, max compression
```

## Comparing `spicedmoon-1.0.3.tar` & `spicedmoon-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2022-09-01 10:16:27.219885 spicedmoon-1.0.3/
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     1064 2022-05-03 10:38:31.000000 spicedmoon-1.0.3/LICENSE
--rw-rw-r--   0 javgat    (1000) javgat    (1000)        0 2022-03-04 09:24:01.000000 spicedmoon-1.0.3/MANIFEST.in
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2022-09-01 10:16:27.219885 spicedmoon-1.0.3/PKG-INFO
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     2948 2022-09-01 10:16:03.000000 spicedmoon-1.0.3/README.md
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      104 2022-03-04 09:24:01.000000 spicedmoon-1.0.3/pyproject.toml
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      804 2022-09-01 10:16:27.219885 spicedmoon-1.0.3/setup.cfg
--rw-rw-r--   0 javgat    (1000) javgat    (1000)       37 2022-03-04 09:24:01.000000 spicedmoon-1.0.3/setup.py
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2022-09-01 10:16:27.215885 spicedmoon-1.0.3/src/
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2022-09-01 10:16:27.219885 spicedmoon-1.0.3/src/spicedmoon/
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      287 2022-03-15 14:42:51.000000 spicedmoon-1.0.3/src/spicedmoon/__init__.py
--rw-rw-r--   0 javgat    (1000) javgat    (1000)    21899 2022-09-01 10:15:35.000000 spicedmoon-1.0.3/src/spicedmoon/spicedmoon.py
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2022-09-01 10:16:27.219885 spicedmoon-1.0.3/src/spicedmoon.egg-info/
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2022-09-01 10:16:27.000000 spicedmoon-1.0.3/src/spicedmoon.egg-info/PKG-INFO
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      308 2022-09-01 10:16:27.000000 spicedmoon-1.0.3/src/spicedmoon.egg-info/SOURCES.txt
--rw-rw-r--   0 javgat    (1000) javgat    (1000)        1 2022-09-01 10:16:27.000000 spicedmoon-1.0.3/src/spicedmoon.egg-info/dependency_links.txt
--rw-rw-r--   0 javgat    (1000) javgat    (1000)       30 2022-09-01 10:16:27.000000 spicedmoon-1.0.3/src/spicedmoon.egg-info/requires.txt
--rw-rw-r--   0 javgat    (1000) javgat    (1000)       11 2022-09-01 10:16:27.000000 spicedmoon-1.0.3/src/spicedmoon.egg-info/top_level.txt
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     1064 2023-05-02 10:46:38.000000 spicedmoon-1.0.4/LICENSE
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)        0 2023-05-02 10:46:38.000000 spicedmoon-1.0.4/MANIFEST.in
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/PKG-INFO
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     2948 2023-05-04 11:54:27.000000 spicedmoon-1.0.4/README.md
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      104 2023-05-02 10:46:38.000000 spicedmoon-1.0.4/pyproject.toml
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      804 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/setup.cfg
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)       37 2023-05-02 10:46:38.000000 spicedmoon-1.0.4/setup.py
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 11:55:11.260690 spicedmoon-1.0.4/src/
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/src/spicedmoon/
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      345 2023-05-04 11:50:53.000000 spicedmoon-1.0.4/src/spicedmoon/__init__.py
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)    24555 2023-05-04 11:50:28.000000 spicedmoon-1.0.4/src/spicedmoon/spicedmoon.py
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/src/spicedmoon.egg-info/
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/PKG-INFO
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      308 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/SOURCES.txt
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)        1 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/dependency_links.txt
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)       30 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/requires.txt
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)       11 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/top_level.txt
```

### Comparing `spicedmoon-1.0.3/LICENSE` & `spicedmoon-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spicedmoon-1.0.3/PKG-INFO` & `spicedmoon-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spicedmoon
-Version: 1.0.3
+Version: 1.0.4
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
 
-![Version 1.0.3](https://img.shields.io/badge/version-1.0.3-informational)
+![Version 1.0.4](https://img.shields.io/badge/version-1.0.4-informational)
 ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
 
 Calculation of lunar data using NASA’s SPICE toolbox.
 
 This data includes:
 - Distance between the Sun and the Moon (in astronomical units)
 - Distance between the Sun and the Moon (in kilometers)
```

### Comparing `spicedmoon-1.0.3/README.md` & `spicedmoon-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # spicedmoon
 
-![Version 1.0.3](https://img.shields.io/badge/version-1.0.3-informational)
+![Version 1.0.4](https://img.shields.io/badge/version-1.0.4-informational)
 ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
 
 Calculation of lunar data using NASA’s SPICE toolbox.
 
 This data includes:
 - Distance between the Sun and the Moon (in astronomical units)
 - Distance between the Sun and the Moon (in kilometers)
```

### Comparing `spicedmoon-1.0.3/setup.cfg` & `spicedmoon-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spicedmoon
-version = 1.0.3
+version = 1.0.4
 author = Group of Atmospheric Optics (GOA-UVa), Universidad de Valladolid
 author_email = gaton@goa.uva.es
 description = Calculation of lunar data using NASA’s SPICE toolbox.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GOA-UVa/spicedmoon
 license_files = LICENSE
```

### Comparing `spicedmoon-1.0.3/src/spicedmoon/spicedmoon.py` & `spicedmoon-1.0.4/src/spicedmoon/spicedmoon.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Calculation of lunar data using NASA's SPICE toolbox.
 
 It exports the following functions:
 
     * get_moon_datas - Calculates needed MoonData from SPICE toolbox
     * get_moon_datas_from_extra_kernels - Calculates needed MoonData from SPICE toolbox
         and using data from extra kernels for the observer body
+    * get_sun_moon_datas - Calculates solar selenographic coordinates.
 """
 
 """___Built-In Modules___"""
 from dataclasses import dataclass
 import os
 import math
 from typing import List, Union
@@ -72,14 +73,34 @@
     lon_sun_rad: float
     lat_obs: float
     lon_obs: float
     mpa_deg: float
     azimuth: float
     zenith: float
 
+@dataclass
+class MoonSunData:
+    """Dataclass with information of the relation between the Sun and the Moon.
+
+    Attributes
+    ----------
+    lon_sun_rad: float
+        Selenographic longitude of the Sun in radians
+    lat_sun_rad: float
+        Selenographic latitude of the Sun in radians
+    dist_sun_moon_km: float
+        Distance between the Sun and the Moon in km
+    dist_sun_moon_au: float
+        Distance between the Sun and the Moon in AU
+    """
+    lon_sun_rad: float
+    lat_sun_rad: float
+    dist_sun_moon_km: float
+    dist_sun_moon_au: float
+
 def _furnsh_safer(k_path: str):
     """
     Perfroms the SPICE furnsh_c function, but in case that it fails it tries again after a small time
     interval.
 
     Furnsh has produced an error once, very rarely, but it can be solved trying again, so this is what this
     function solves.
@@ -180,14 +201,46 @@
         pol_rad = 6356.7519 # Earth polar radius
         alt_km = altitude/1000
         flattening = (eq_rad - pol_rad)/eq_rad
         pos_iau_earth = spice.pgrrec('EARTH', math.radians(lon), math.radians(lat), alt_km,
                                      eq_rad, flattening)
         self.states = _calculate_states(ets, pos_iau_earth, delta_t, source_frame, target_frame)
 
+
+def _get_sun_moon_data(utc_time: str):
+    et_date = spice.str2et(utc_time)
+    m_eq_rad = 1738.1
+    m_pol_rad = 1736
+    flattening = (m_eq_rad-m_pol_rad)/m_eq_rad
+    # Calculate selenographic longitude of sun
+    sun_spoint, _, _ = spice.subslr("INTERCEPT/ELLIPSOID", "MOON", et_date, 'MOON_ME',
+                                    "NONE", "SUN")
+    lon_sun_rad, lat_sun_rad, _ = spice.recpgr("MOON", sun_spoint, m_eq_rad, flattening)
+
+    # Calculate the distance between sun and moon (AU)
+    state, _ = spice.spkezr("MOON", et_date, "MOON_ME", "NONE", "SUN")
+    dist_sun_moon_km = math.sqrt(state[0]**2 + state[1]**2 + state[2]**2)
+    dist_sun_moon_au = spice.convrt(dist_sun_moon_km, "KM", "AU")
+
+
+    limit_lat_rad = math.pi/2
+    if lat_sun_rad > limit_lat_rad:
+        lat_sun_rad -= limit_lat_rad*2
+    elif lat_sun_rad < -limit_lat_rad:
+        lat_sun_rad += limit_lat_rad*2
+
+    limit_lon_rad = math.pi
+    if lon_sun_rad > limit_lon_rad:
+        lon_sun_rad -= limit_lon_rad*2
+    elif lon_sun_rad < -limit_lon_rad:
+        lon_sun_rad += limit_lon_rad*2
+
+    return MoonSunData(lon_sun_rad, lat_sun_rad, dist_sun_moon_km, dist_sun_moon_au)
+
+
 def _get_moon_data(utc_time: str, observer_name: str = _DEFAULT_OBSERVER_NAME,
                    observer_frame: str = _DEFAULT_OBSERVER_FRAME,
                    observer_zenith_name: str = _DEFAULT_OBSERVER_ZENITH_NAME,
                    correct_zenith_azimuth: bool = False, longitude: float = 0,
                    colat: float = 0) -> MoonData:
     """Calculation of the moon data for the given utc_time for the loaded observer
 
@@ -215,17 +268,18 @@
     Returns
     -------
     MoonData
         Moon data obtained from SPICE toolbox
     """
     et_date = spice.str2et(utc_time)
 
-    _, radios_luna = spice.bodvrd("MOON", "RADII", 3)
-    m_eq_rad = radios_luna[0] # 1738.1 # Moon Equatorial Radius
-    m_pol_rad = radios_luna[2] # 1736 # Moon polar radius
+    #_, radios_luna = spice.bodvrd("MOON", "RADII", 3)
+    # The ones obtained with bodvrd are not correct
+    m_eq_rad = 1738.1 #radios_luna[0] # Moon Equatorial Radius
+    m_pol_rad = 1736 #radios_luna[2] # Moon polar radius
     flattening = (m_eq_rad-m_pol_rad)/m_eq_rad
 
     # Calculate moon zenith and azimuth
     state_zenith, _ = spice.spkezr("MOON", et_date, observer_frame, "NONE", observer_zenith_name)
     rectan_zenith = np.split(state_zenith, 2)[0]
     if correct_zenith_azimuth:
         lon_rad = (longitude+180) * spice.rpd()
@@ -251,50 +305,40 @@
         phase = -phase
 
     # Calculate selenographic coordinates of the observer
     lon_obs, lat_obs, _ = spice.recpgr("MOON", spoint, m_eq_rad, flattening)
     lon_obs = lon_obs * spice.dpr()
     lat_obs = lat_obs * spice.dpr()
 
-    # Calculate selenographic longitude of sun
-    sun_spoint, _, _ = spice.subslr("INTERCEPT/ELLIPSOID", "MOON", et_date, 'MOON_ME',
-                                    "NONE", "SUN")
-    lon_sun_rad, _, _ = spice.recpgr("MOON", sun_spoint, m_eq_rad, flattening)
-
     # Calculate the distance between observer and moon (KM)
     state, _ = spice.spkezr("MOON", et_date, "MOON_ME", "NONE", observer_name)
     dist_obs_moon = math.sqrt(state[0]**2 + state[1]**2 + state[2]**2)
 
-    # Calculate the distance between sun and moon (AU)
-    state, _ = spice.spkezr("MOON", et_date, "MOON_ME", "NONE", "SUN")
-    dist_sun_moon_km = math.sqrt(state[0]**2 + state[1]**2 + state[2]**2)
-    dist_sun_moon_au = spice.convrt(dist_sun_moon_km, "KM", "AU")
+    smd = _get_sun_moon_data(utc_time)
+    lon_sun_rad = smd.lon_sun_rad
+    dist_sun_moon_km = smd.dist_sun_moon_km
+    dist_sun_moon_au = smd.dist_sun_moon_au
 
     limit_lat = 90
     if lat_obs > limit_lat:
         lat_obs -= limit_lat*2
     elif lat_obs < -limit_lat:
         lat_obs += limit_lat*2
 
     limit_lon = 180
     if lon_obs > limit_lon:
         lon_obs -= limit_lon*2
     elif lon_obs < -limit_lon:
         lon_obs += limit_lon*2
 
-    limit_lon_rad = math.pi
-    if lon_sun_rad > limit_lon_rad:
-        lon_sun_rad -= limit_lon_rad*2
-    elif lon_sun_rad < -limit_lon_rad:
-        lon_sun_rad += limit_lon_rad*2
-
     moon_data = MoonData(dist_sun_moon_au, dist_sun_moon_km, dist_obs_moon, lon_sun_rad,
                          lat_obs, lon_obs, phase, azimuth, zenith)
     return moon_data
 
+
 def _get_moon_datas_id(utc_times: List[str], kernels_path: str,
                        observer_id: int, observer_frame: str,
                        custom_kernel_dir: str,
                        correct_zenith_azimuth: bool = False,
                        latitude: float = 0, longitude: float = 0,
                        earth_as_zenith_observer: bool = False) -> List[MoonData]:
     """Calculation of needed MoonDatas from SPICE toolbox
@@ -353,14 +397,15 @@
             correct_zenith_azimuth, lon, colat)
         moon_datas.append(new_md)
 
     spice.kclear()
 
     return moon_datas
 
+
 def _create_earth_point_kernel(utc_times: List[str], kernels_path: str, lat: int, lon: int,
                                altitude: float, id_code: int, custom_kernel_dir: str) -> None:
     """Creates a SPK custom kernel file containing the data of a point on Earth's surface
 
     Parameters
     ----------
     utc_times : list of str
@@ -412,26 +457,28 @@
     spice.spkw09(handle, obs.point_id, center, target_frame,
                  ets[0], ets[-1], '0', polynomial_degree, len(ets),
                  obs.states.tolist(), ets.tolist())
     spice.spkcls(handle)
 
     spice.kclear()
 
+
 def _remove_custom_kernel_file(kernels_path: str) -> None:
     """Remove the custom SPK kernel file if it exists
 
     Parameters
     ----------
     kernels_path : str
         Path where the SPICE kernels are stored
     """
     custom_kernel_path = os.path.join(kernels_path, CUSTOM_KERNEL_NAME)
     if os.path.exists(custom_kernel_path):
         os.remove(custom_kernel_path)
 
+
 def _dt_to_str(dts: Union[List[datetime], List[str]]) -> List[str]:
     """Convert a list of datetimes into a list of string dates in a valid format.
     
     Parameters
     ----------
     dts: list of datetimes | list of str
         List of datetimes that will be converted to utc_times. They must be timezone aware.
@@ -448,14 +495,45 @@
         if isinstance(dt, datetime):
             dt_utc = dt.astimezone(timezone.utc)
             utc_times.append(dt_utc.strftime("%Y-%m-%d %H:%M:%S"))
         else:
             utc_times.append(dt)
     return utc_times
 
+
+def get_sun_moon_datas(times: Union[List[str], List[datetime]], kernels_path: str) -> List[MoonSunData]:
+    """
+    Obtain solar selenographic coordinates of at multiple times.
+
+    times : list of str | list of datetime
+        Times at which the lunar data will be calculated.
+        If they are str, they must be in a valid UTC format allowed by SPICE, such as
+        %Y-%m-%d %H:%M:%S.
+        If they are datetimes they must be timezone aware, or they will be understood
+        as computer local time.
+    kernels_path : str
+        Path where the SPICE kernels are stored
+    """
+    utc_times = _dt_to_str(times)
+    if(len(utc_times) == 0):
+        return []
+    kernels = ["moon_pa_de421_1900-2050.bpc", "moon_080317.tf",
+               "pck00010.tpc", "naif0011.tls", "de421.bsp", "earth_assoc_itrf93.tf",
+               "earth_latest_high_prec.bpc", "earth_070425_370426_predict.bpc"]
+    for kernel in kernels:
+        k_path = os.path.join(kernels_path, kernel)
+        _furnsh_safer(k_path)
+    
+    msds = []
+    for utc_time in utc_times:
+        msd = _get_sun_moon_data(utc_time)
+        msds.append(msd)
+    spice.kclear()
+    return msds
+
 def get_moon_datas_from_extra_kernels(times: Union[List[str], List[datetime]], kernels_path: str,
                                       extra_kernels: List[str], extra_kernels_path: str,
                                       observer_name: str, observer_frame: str,
                                       earth_as_zenith_observer: bool = False
                                       ) -> List[MoonData]:
     """Calculation of needed Moon data from SPICE toolbox
 
@@ -508,14 +586,15 @@
         moon_datas.append(_get_moon_data(utc_time, observer_name, observer_frame,
             zenith_observer))
 
     spice.kclear()
 
     return moon_datas
 
+
 def get_moon_datas(lat: float, lon: float, altitude: float,
                    times: Union[List[str], List[datetime]],
                    kernels_path: str, correct_zenith_azimuth: bool = True,
                    observer_frame: str = "ITRF93",
                    earth_as_zenith_observer: bool = False, custom_kernel_path: str = None,
                    ) -> List[MoonData]:
     """Calculation of needed Moon data from SPICE toolbox
@@ -535,14 +614,17 @@
         Times at which the lunar data will be calculated.
         If they are str, they must be in a valid UTC format allowed by SPICE, such as
         %Y-%m-%d %H:%M:%S.
         If they are datetimes they must be timezone aware, or they will be understood
         as computer local time.
     kernels_path : str
         Path where the SPICE kernels are stored
+    correct_zenith_azimuth : bool
+        In case that it's calculated without using the extra kernels, the coordinates should be
+        corrected rotating them into the correct location.
     observer_frame : str
         Observer frame that will be used in the calculations of the azimuth and zenith.
     earth_as_zenith_observer : bool
         If True the Earth will be used as the observer for the zenith and azimuth calculation.
         Otherwise it will be the actual observer. By default is False.
     custom_kernel_path: str
         Path of the kernel custom.bsp that will be edited by the library, not only read.
```

### Comparing `spicedmoon-1.0.3/src/spicedmoon.egg-info/PKG-INFO` & `spicedmoon-1.0.4/src/spicedmoon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spicedmoon
-Version: 1.0.3
+Version: 1.0.4
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
 
-![Version 1.0.3](https://img.shields.io/badge/version-1.0.3-informational)
+![Version 1.0.4](https://img.shields.io/badge/version-1.0.4-informational)
 ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
 
 Calculation of lunar data using NASA’s SPICE toolbox.
 
 This data includes:
 - Distance between the Sun and the Moon (in astronomical units)
 - Distance between the Sun and the Moon (in kilometers)
```

