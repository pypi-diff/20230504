# Comparing `tmp/spicedmoon-1.0.4.tar.gz` & `tmp/spicedmoon-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicedmoon-1.0.4.tar", last modified: Thu May  4 11:55:11 2023, max compression
+gzip compressed data, was "spicedmoon-1.0.5.tar", last modified: Thu May  4 13:54:28 2023, max compression
```

## Comparing `spicedmoon-1.0.4.tar` & `spicedmoon-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     1064 2023-05-02 10:46:38.000000 spicedmoon-1.0.4/LICENSE
--rw-rw-r--   0 javgat    (1000) javgat    (1000)        0 2023-05-02 10:46:38.000000 spicedmoon-1.0.4/MANIFEST.in
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/PKG-INFO
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     2948 2023-05-04 11:54:27.000000 spicedmoon-1.0.4/README.md
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      104 2023-05-02 10:46:38.000000 spicedmoon-1.0.4/pyproject.toml
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      804 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/setup.cfg
--rw-rw-r--   0 javgat    (1000) javgat    (1000)       37 2023-05-02 10:46:38.000000 spicedmoon-1.0.4/setup.py
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 11:55:11.260690 spicedmoon-1.0.4/src/
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/src/spicedmoon/
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      345 2023-05-04 11:50:53.000000 spicedmoon-1.0.4/src/spicedmoon/__init__.py
--rw-rw-r--   0 javgat    (1000) javgat    (1000)    24555 2023-05-04 11:50:28.000000 spicedmoon-1.0.4/src/spicedmoon/spicedmoon.py
-drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 11:55:11.264690 spicedmoon-1.0.4/src/spicedmoon.egg-info/
--rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/PKG-INFO
--rw-rw-r--   0 javgat    (1000) javgat    (1000)      308 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/SOURCES.txt
--rw-rw-r--   0 javgat    (1000) javgat    (1000)        1 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/dependency_links.txt
--rw-rw-r--   0 javgat    (1000) javgat    (1000)       30 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/requires.txt
--rw-rw-r--   0 javgat    (1000) javgat    (1000)       11 2023-05-04 11:55:11.000000 spicedmoon-1.0.4/src/spicedmoon.egg-info/top_level.txt
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     1064 2023-05-02 10:46:38.000000 spicedmoon-1.0.5/LICENSE
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)        0 2023-05-02 10:46:38.000000 spicedmoon-1.0.5/MANIFEST.in
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/PKG-INFO
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     2948 2023-05-04 13:53:16.000000 spicedmoon-1.0.5/README.md
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      104 2023-05-02 10:46:38.000000 spicedmoon-1.0.5/pyproject.toml
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      804 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/setup.cfg
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)       37 2023-05-02 10:46:38.000000 spicedmoon-1.0.5/setup.py
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/src/
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/src/spicedmoon/
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      375 2023-05-04 13:53:58.000000 spicedmoon-1.0.5/src/spicedmoon/__init__.py
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)    31192 2023-05-04 13:53:46.000000 spicedmoon-1.0.5/src/spicedmoon/spicedmoon.py
+drwxrwxr-x   0 javgat    (1000) javgat    (1000)        0 2023-05-04 13:54:28.112579 spicedmoon-1.0.5/src/spicedmoon.egg-info/
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)     3523 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/PKG-INFO
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)      308 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/SOURCES.txt
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)        1 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/dependency_links.txt
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)       30 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/requires.txt
+-rw-rw-r--   0 javgat    (1000) javgat    (1000)       11 2023-05-04 13:54:28.000000 spicedmoon-1.0.5/src/spicedmoon.egg-info/top_level.txt
```

### Comparing `spicedmoon-1.0.4/LICENSE` & `spicedmoon-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spicedmoon-1.0.4/PKG-INFO` & `spicedmoon-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spicedmoon
-Version: 1.0.4
+Version: 1.0.5
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
 
-![Version 1.0.4](https://img.shields.io/badge/version-1.0.4-informational)
+![Version 1.0.5](https://img.shields.io/badge/version-1.0.5-informational)
 ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
 
 Calculation of lunar data using NASA’s SPICE toolbox.
 
 This data includes:
 - Distance between the Sun and the Moon (in astronomical units)
 - Distance between the Sun and the Moon (in kilometers)
```

### Comparing `spicedmoon-1.0.4/README.md` & `spicedmoon-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # spicedmoon
 
-![Version 1.0.4](https://img.shields.io/badge/version-1.0.4-informational)
+![Version 1.0.5](https://img.shields.io/badge/version-1.0.5-informational)
 ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
 
 Calculation of lunar data using NASA’s SPICE toolbox.
 
 This data includes:
 - Distance between the Sun and the Moon (in astronomical units)
 - Distance between the Sun and the Moon (in kilometers)
```

### Comparing `spicedmoon-1.0.4/setup.cfg` & `spicedmoon-1.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spicedmoon
-version = 1.0.4
+version = 1.0.5
 author = Group of Atmospheric Optics (GOA-UVa), Universidad de Valladolid
 author_email = gaton@goa.uva.es
 description = Calculation of lunar data using NASA’s SPICE toolbox.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GOA-UVa/spicedmoon
 license_files = LICENSE
```

### Comparing `spicedmoon-1.0.4/src/spicedmoon/spicedmoon.py` & `spicedmoon-1.0.5/src/spicedmoon/spicedmoon.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 It exports the following functions:
 
     * get_moon_datas - Calculates needed MoonData from SPICE toolbox
     * get_moon_datas_from_extra_kernels - Calculates needed MoonData from SPICE toolbox
         and using data from extra kernels for the observer body
     * get_sun_moon_datas - Calculates solar selenographic coordinates.
+    * get_moon_datas_from_moon - Calculates needed MoonData from SPICE toolbox from selenographic coordinates
 """
 
 """___Built-In Modules___"""
 from dataclasses import dataclass
 import os
 import math
 from typing import List, Union
@@ -31,14 +32,15 @@
 __created__ = "2022/03/03"
 __maintainer__ = "Javier Gatón Herguedas"
 __email__ = "gaton@goa.uva.es"
 __status__ = "Development"
 
 CUSTOM_KERNEL_NAME = "custom.bsp"
 EARTH_ID_CODE = 399
+MOON_ID_CODE = 301
 
 _DEFAULT_OBSERVER_NAME = "Observer"
 _DEFAULT_OBSERVER_FRAME = "Observer_LOCAL_LEVEL"
 _DEFAULT_OBSERVER_ZENITH_NAME = "EARTH"
 
 @dataclass
 class MoonData:
@@ -112,29 +114,29 @@
     """
     try:
         spice.furnsh(k_path)
     except:
         time.sleep(2)
         spice.furnsh(k_path)
 
-def _calculate_states(ets: np.ndarray, pos_iau_earth: np.ndarray, delta_t: float,
+def _calculate_states(ets: np.ndarray, pos_iau: np.ndarray, delta_t: float,
                       source_frame: str, target_frame: str) -> np.ndarray:
     """
     Returns a ndarray containing the states of a point referencing the target frame.
 
     The states array is a time-ordered array of geometric states (x, y, z, dx/dt, dy/dt, dz/dt,
     in kilometers and kilometers per second) of body relative to center, specified relative
     to frame. Useful for spice function "spkw09_c", for example.
 
     Parameters
     ----------
     ets : np.ndarray
         Array of TDB seconds from J2000 (et dates) of which the data will be taken
-    pos_iau_earth : np.ndarray
-        Rectangular coordinates of the point, referencing IAU_EARTH frame.
+    pos_iau : np.ndarray
+        Rectangular coordinates of the point, referencing IAU frame.
     delta_t : float
         TDB seconds between states
     source_frame : str
         Name of the frame to transform from.
     target_frame : str
         Name of the frame which the location will be referencing.
 
@@ -145,23 +147,23 @@
     """
     num_coordinates = 3
     n_state_attributes = 6
     states = np.zeros((len(ets), n_state_attributes))
     for i, et_value in enumerate(ets):
         states[i, :num_coordinates] = np.dot(
             spice.pxform(source_frame, target_frame, et_value),
-            pos_iau_earth)
+            pos_iau)
 
     for i in range(len(ets) - 1):
         states[i, num_coordinates:] = (states[i + 1, :num_coordinates] -
                                        states[i, :num_coordinates]) / delta_t
 
     pos_np1 = np.dot(
         spice.pxform(source_frame, target_frame, ets[-1] + delta_t),
-        pos_iau_earth)
+        pos_iau)
     states[-1, num_coordinates:] = (pos_np1 - states[-1, :num_coordinates]) / delta_t
     return states
 
 @dataclass
 class _EarthLocation():
     """
     Data for the creation of an observer point on earth surface
@@ -202,14 +204,59 @@
         alt_km = altitude/1000
         flattening = (eq_rad - pol_rad)/eq_rad
         pos_iau_earth = spice.pgrrec('EARTH', math.radians(lon), math.radians(lat), alt_km,
                                      eq_rad, flattening)
         self.states = _calculate_states(ets, pos_iau_earth, delta_t, source_frame, target_frame)
 
 
+@dataclass
+class _MoonLocation():
+    """
+    Data for the creation of an observer point on Moon's surface
+
+    Attributes
+    ----------
+    point_id : int
+        ID code that will be associated with the point on Moon's surface
+    states : np.ndarray of float64
+        Array of geometric states of body relative to center
+    """
+    __slots__ = ['point_id', 'states']
+    def __init__(self, point_id: int, lat: float, lon: float, altitude: float, ets: np.ndarray,
+                 delta_t: float, source_frame: str, target_frame: str):
+        """
+        Parameters
+        ----------
+        point_id : int
+            ID code that will be associated with the point on Moon's surface
+        lat : float
+            Geographic latitude of the observer point
+        lon : float
+            Geographic longitude of the observer point
+        altitude : float
+            Altitude over the sea level in meters.
+        ets : np.ndarray
+            Array of TDB seconds from J2000 (et dates) of which the data will be taken
+        delta_t : float
+            TDB seconds between states
+        source_frame : str
+            Name of the frame to transform from.
+        target_frame : str
+            Name of the frame which the location will be referencing.
+        """
+        self.point_id = point_id
+        eq_rad = 1738.1 # Moon equatorial radius
+        pol_rad = 1736 # Moon polar radius
+        alt_km = altitude/1000
+        flattening = (eq_rad - pol_rad)/eq_rad
+        pos_iau_moon = spice.pgrrec('MOON', math.radians(lon), math.radians(lat), alt_km,
+                                     eq_rad, flattening)
+        self.states = _calculate_states(ets, pos_iau_moon, delta_t, source_frame, target_frame)
+
+
 def _get_sun_moon_data(utc_time: str):
     et_date = spice.str2et(utc_time)
     m_eq_rad = 1738.1
     m_pol_rad = 1736
     flattening = (m_eq_rad-m_pol_rad)/m_eq_rad
     # Calculate selenographic longitude of sun
     sun_spoint, _, _ = spice.subslr("INTERCEPT/ELLIPSOID", "MOON", et_date, 'MOON_ME',
@@ -458,14 +505,75 @@
                  ets[0], ets[-1], '0', polynomial_degree, len(ets),
                  obs.states.tolist(), ets.tolist())
     spice.spkcls(handle)
 
     spice.kclear()
 
 
+def _create_moon_point_kernel(utc_times: List[str], kernels_path: str, lat: int, lon: int,
+                               altitude: float, id_code: int, custom_kernel_dir: str) -> None:
+    """Creates a SPK custom kernel file containing the data of a point on Earth's surface
+
+    Parameters
+    ----------
+    utc_times : list of str
+        Times at which the lunar data will be calculated, in a valid UTC DateTime format
+    kernels_path : str
+        Path where the SPICE kernels are stored
+    lat : float
+        Geographic latitude (in degrees) of the location.
+    lon : float
+        Geographic longitude (in degrees) of the location.
+    altitude : float
+        Altitude over the sea level in meters.
+    id_code : int
+        ID code that will be associated with the point on Earth's surface
+    custom_kernel_dir: str
+        Path where the writable custom kernel custom.bsp will be stored.
+    """
+    kernels = ["moon_pa_de421_1900-2050.bpc", "moon_080317.tf",
+               "pck00010.tpc", "naif0011.tls", "earth_assoc_itrf93.tf",
+               "de421.bsp", "earth_latest_high_prec.bpc", "earth_070425_370426_predict.bpc"]
+    for kernel in kernels:
+        k_path = os.path.join(kernels_path, kernel)
+        _furnsh_safer(k_path)
+
+    polynomial_degree = 5
+    # Degree of the lagrange polynomials that will be used to interpolate the states
+    delta_t = 1 # TDB seconds between states. Arbitrary.
+    min_states_polynomial = polynomial_degree + 1
+    # Min # states that are required to define a polynomial of that degree
+    ets = np.array([])
+    left_states = int(min_states_polynomial/2)
+    right_states = left_states + min_states_polynomial%2
+    for utc_time in utc_times:
+        et0 = spice.str2et(utc_time)
+        etprev = et0 - delta_t * left_states
+        etf = et0 + delta_t * right_states
+        ets_t = np.arange(etprev, etf, delta_t)
+        for et_t in ets_t:
+            if et_t not in ets:
+                index = np.searchsorted(ets, et_t)
+                ets = np.insert(ets, index, et_t)
+
+    target_frame = source_frame = 'MOON_ME'
+    obs = _MoonLocation(id_code, lat, lon, altitude, ets, delta_t, source_frame, target_frame)
+
+    custom_kernel_path = os.path.join(custom_kernel_dir, CUSTOM_KERNEL_NAME)
+    handle = spice.spkopn(custom_kernel_path, 'SPK_file', 0)
+
+    center = MOON_ID_CODE
+    spice.spkw09(handle, obs.point_id, center, target_frame,
+                 ets[0], ets[-1], '0', polynomial_degree, len(ets),
+                 obs.states.tolist(), ets.tolist())
+    spice.spkcls(handle)
+
+    spice.kclear()
+
+
 def _remove_custom_kernel_file(kernels_path: str) -> None:
     """Remove the custom SPK kernel file if it exists
 
     Parameters
     ----------
     kernels_path : str
         Path where the SPICE kernels are stored
@@ -640,7 +748,58 @@
     utc_times = _dt_to_str(times)
     if(len(utc_times) == 0):
         return []
     _remove_custom_kernel_file(custom_kernel_path)
     _create_earth_point_kernel(utc_times, kernels_path, lat, lon, altitude, id_code, custom_kernel_path)
     return _get_moon_datas_id(utc_times, kernels_path, id_code, observer_frame, custom_kernel_path,
         correct_zenith_azimuth, lat, lon, earth_as_zenith_observer)
+
+
+def get_moon_datas_from_moon(lat: float, lon: float, altitude: float,
+                   times: Union[List[str], List[datetime]],
+                   kernels_path: str, correct_zenith_azimuth: bool = True,
+                   observer_frame: str = "MOON_ME", custom_kernel_path: str = None,
+                   ) -> List[MoonData]:
+    """Calculation of needed Moon data from SPICE toolbox
+
+    Moon phase angle, selenographic coordinates and distance from observer point to moon.
+    Selenographic longitude and distance from sun to moon.
+
+    Parameters
+    ----------
+    lat : float
+        Geographic latitude (in degrees) of the location.
+    lon : float
+        Geographic longitude (in degrees) of the location.
+    altitude : float
+        Altitude over the sea level in meters.
+    times : list of str | list of datetime
+        Times at which the lunar data will be calculated.
+        If they are str, they must be in a valid UTC format allowed by SPICE, such as
+        %Y-%m-%d %H:%M:%S.
+        If they are datetimes they must be timezone aware, or they will be understood
+        as computer local time.
+    kernels_path : str
+        Path where the SPICE kernels are stored
+    correct_zenith_azimuth : bool
+        In case that it's calculated without using the extra kernels, the coordinates should be
+        corrected rotating them into the correct location.
+    observer_frame : str
+        Observer frame that will be used in the calculations of the azimuth and zenith.
+    custom_kernel_path: str
+        Path of the kernel custom.bsp that will be edited by the library, not only read.
+        If none, it will be the same as kernels_path.
+    Returns
+    -------
+    list of MoonData
+        Moon data obtained from SPICE toolbox
+    """
+    if custom_kernel_path == None:
+        custom_kernel_path = kernels_path
+    id_code = 301100
+    utc_times = _dt_to_str(times)
+    if(len(utc_times) == 0):
+        return []
+    _remove_custom_kernel_file(custom_kernel_path)
+    _create_moon_point_kernel(utc_times, kernels_path, lat, lon, altitude, id_code, custom_kernel_path)
+    return _get_moon_datas_id(utc_times, kernels_path, id_code, observer_frame, custom_kernel_path,
+        correct_zenith_azimuth, lat, lon, False)
```

### Comparing `spicedmoon-1.0.4/src/spicedmoon.egg-info/PKG-INFO` & `spicedmoon-1.0.5/src/spicedmoon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spicedmoon
-Version: 1.0.4
+Version: 1.0.5
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
 
-![Version 1.0.4](https://img.shields.io/badge/version-1.0.4-informational)
+![Version 1.0.5](https://img.shields.io/badge/version-1.0.5-informational)
 ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
 
 Calculation of lunar data using NASA’s SPICE toolbox.
 
 This data includes:
 - Distance between the Sun and the Moon (in astronomical units)
 - Distance between the Sun and the Moon (in kilometers)
```

