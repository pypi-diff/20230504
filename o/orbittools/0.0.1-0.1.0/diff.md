# Comparing `tmp/orbittools-0.0.1.tar.gz` & `tmp/orbittools-0.1.0.tar.gz`

## Comparing `orbittools-0.0.1.tar` & `orbittools-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orbittools-0.0.1/src/orbittools/__init__.py
--rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 orbittools-0.0.1/src/orbittools/kepler.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 orbittools-0.0.1/src/orbittools/transforms.py
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 orbittools-0.0.1/LICENSE
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 orbittools-0.0.1/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 orbittools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 orbittools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orbittools-0.1.0/src/orbittools/__init__.py
+-rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 orbittools-0.1.0/src/orbittools/kepler.py
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 orbittools-0.1.0/src/orbittools/tle.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 orbittools-0.1.0/src/orbittools/transforms.py
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 orbittools-0.1.0/LICENSE
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 orbittools-0.1.0/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 orbittools-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 orbittools-0.1.0/PKG-INFO
```

### Comparing `orbittools-0.0.1/src/orbittools/kepler.py` & `orbittools-0.1.0/src/orbittools/kepler.py`

 * *Files identical despite different names*

### Comparing `orbittools-0.0.1/src/orbittools/transforms.py` & `orbittools-0.1.0/src/orbittools/transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import pandas as pd
-import apexpy
+# import apexpy
 from astropy.time import Time
 import astropy.coordinates as coord
 from astropy.coordinates import CartesianRepresentation
 from astropy import units as u
 from scipy.interpolate import lagrange, interp1d
 
 '''
@@ -15,15 +15,16 @@
 
 
 def itrf_to_geodetic_func(position_vectors):
     if np.any(np.isnan(position_vectors)):
         return {'lon': np.nan,
                 'lat': np.nan,
                 'height': np.nan}
-    astro_position = coord.ITRS(CartesianRepresentation(position_vectors*u.km))
+    astro_position = coord.ITRS(CartesianRepresentation(position_vectors,
+                                unit=u.km))
     geodetic_position = astro_position.earth_location.to_geodetic('WGS84')
     return {'lon': geodetic_position.lon.value,
             'lat': geodetic_position.lat.value,
             'height': geodetic_position.height.to(u.m).value}
 
 
 def itrf_to_geodetic(df_itrf):
@@ -33,49 +34,75 @@
                                  'z_itrf']].apply(itrf_to_geodetic_func,
                                                   axis=1,
                                                   result_type='expand')
                         ], axis=1)
     return df_out
 
 
-def geodetic_to_qd(df_geod):
-    A = apexpy.Apex(df_geod.index[0])
-    lat_qd, lon_qd = A.geo2qd(glat=df_geod['lat'],
-                              glon=df_geod['lon'],
-                              height=df_geod['height'])
-    mlt = A.mlon2mlt(mlon=lon_qd, datetime=df_geod.index.values)
-    df_new = df_geod.copy()
-    df_new['lon_qd'] = lon_qd
-    df_new['lat_qd'] = lat_qd
-    df_new['mlt'] = mlt
-    return df_new
+# def geodetic_to_qd(df_geod):
+#     A = apexpy.Apex(df_geod.index[0])
+#     lat_qd, lon_qd = A.geo2qd(glat=df_geod['lat'],
+#                               glon=df_geod['lon'],
+#                               height=df_geod['height'])
+#     mlt = A.mlon2mlt(mlon=lon_qd, datetime=df_geod.index.values)
+#     df_new = df_geod.copy()
+#     df_new['lon_qd'] = lon_qd
+#     df_new['lat_qd'] = lat_qd
+#     df_new['mlt'] = mlt
+#     return df_new
 
 
 def itrs_to_igrs(df_itrs):
+    t = Time(df_itrs.index)
     df_out = df_itrs.copy()
     itrs = coord.ITRS(x=df_itrs['x_itrf'].values*u.km,
                       y=df_itrs['y_itrf'].values*u.km,
                       z=df_itrs['z_itrf'].values*u.km,
                       v_x=df_itrs['vx_itrf'].values*u.km/u.second,
                       v_y=df_itrs['vy_itrf'].values*u.km/u.second,
                       v_z=df_itrs['vz_itrf'].values*u.km/u.second,
                       obstime=df_itrs.index)
-    gcrs_instance = coord.GCRS(obstime=df_itrs.index)
+    gcrs_instance = coord.GCRS(obstime=t)
     gcrs = itrs.transform_to(gcrs_instance)
     df_out['x_gcrs'] = gcrs.cartesian.x.to_value()
     df_out['y_gcrs'] = gcrs.cartesian.y.to_value()
     df_out['z_gcrs'] = gcrs.cartesian.z.to_value()
     df_out['vx_gcrs'] = gcrs.velocity.d_x.to_value()
     df_out['vy_gcrs'] = gcrs.velocity.d_y.to_value()
     df_out['vz_gcrs'] = gcrs.velocity.d_z.to_value()
     return df_out
 
 
+def igrs_to_itrs(df_igrs):
+    t = Time(df_igrs.index)
+    df_out = df_igrs.copy()
+    igrs = coord.GCRS(representation_type='cartesian',
+                      differential_type='cartesian',
+                      x=df_igrs['x_gcrs'].values*u.km,
+                      y=df_igrs['y_gcrs'].values*u.km,
+                      z=df_igrs['z_gcrs'].values*u.km,
+                      v_x=df_igrs['vx_gcrs'].values*u.km/u.second,
+                      v_y=df_igrs['vy_gcrs'].values*u.km/u.second,
+                      v_z=df_igrs['vz_gcrs'].values*u.km/u.second,
+                      obstime=df_igrs.index)
+    itrs_instance = coord.ITRS(obstime=t)
+    itrs = igrs.transform_to(itrs_instance)
+    df_out['x_itrf'] = itrs.cartesian.x.to_value()
+    df_out['y_itrf'] = itrs.cartesian.y.to_value()
+    df_out['z_itrf'] = itrs.cartesian.z.to_value()
+    df_out['vx_itrf'] = itrs.velocity.d_x.to_value()
+    df_out['vy_itrf'] = itrs.velocity.d_y.to_value()
+    df_out['vz_itrf'] = itrs.velocity.d_z.to_value()
+    return df_out
+
+
 def interpolate_orbit_to_freq(df_orbit, index, order=7, freq='10ms'):
     nlagrange = int((order-1)/2)
+    if (index-nlagrange) < 0 or index+nlagrange > len(df_orbit):
+        raise IndexError("Trying to interpolate out of bounds of input orbit")
     new_index = pd.date_range(df_orbit.index[index-nlagrange],
                               df_orbit.index[index+nlagrange], freq=freq)
     x = (df_orbit.index[index-nlagrange:index+nlagrange] -
          df_orbit.index[index])/pd.to_timedelta('1s')
     newx = (new_index - df_orbit.index[index])/pd.to_timedelta('1s')
     data = {}
     for column in [col for col in df_orbit.columns
@@ -122,32 +149,38 @@
                         columns=df_orbit.columns)
 
 
 def find_zero_crossings(df, column, resolution='10s'):
     before_zero_indices = np.where(np.diff(np.signbit(df[column])))[0]
     zero_crossings_datetimes = []
     for index in before_zero_indices:
-        highfreq_df = interpolate_orbit_to_freq(df, index, freq=resolution)
-        before_zero_indices2 = np.where(np.diff(np.signbit(
-                                        highfreq_df[column])))[0]
-        for index2 in before_zero_indices2:
-            if (highfreq_df.iloc[index2][column]
-                    < highfreq_df.iloc[index2+1][column]):
-                zero_crossings_datetimes.append(highfreq_df.iloc[index2])
-            else:
-                zero_crossings_datetimes.append(highfreq_df.iloc[index2+1])
+        try:
+            highfreq_df = interpolate_orbit_to_freq(df, index, freq=resolution)
+            before_zero_indices2 = np.where(np.diff(np.signbit(
+                                            highfreq_df[column])))[0]
+            for index2 in before_zero_indices2:
+                if (highfreq_df.iloc[index2][column]
+                        < highfreq_df.iloc[index2+1][column]):
+                    zero_crossings_datetimes.append(highfreq_df.iloc[index2])
+                else:
+                    zero_crossings_datetimes.append(highfreq_df.iloc[index2+1])
+        except IndexError:
+            print("Zero crossing too close to edge of input orbit.")
     return pd.DataFrame(zero_crossings_datetimes)
 
 
 def itrf_find_poles_and_nodes(df):
-    df_poles = find_zero_crossings(df, column='vz_itrf', resolution='10ms')
+    columns = ['x_itrf', 'y_itrf', 'z_itrf', 'vx_itrf', 'vy_itrf', 'vz_itrf']
+    df_poles = find_zero_crossings(df[columns], column='vz_itrf', resolution='10ms')
+    if len(df_poles) == 0:
+        return pd.DataFrame()
     df_poles['type'] = df_poles.apply(lambda row: 'N'
                                       if row['z_itrf'] > 0
                                       else 'S', axis=1)
-    df_equator = find_zero_crossings(df, column='z_itrf', resolution='10ms')
+    df_equator = find_zero_crossings(df[columns], column='z_itrf', resolution='10ms')
     df_equator['type'] = df_equator.apply(lambda row: 'A'
                                           if row['vz_itrf'] > 0
                                           else 'D', axis=1)
     df_out = pd.concat([df_poles, df_equator], axis=0).sort_index()
     df_out = itrf_to_geodetic(df_out)[['type', 'lon', 'lat', 'height']]
     astropy_times = Time(pd.to_datetime(df_out.index, utc=True))
     sunlons = coord.get_sun(astropy_times).itrs.spherical.lon.value
```

### Comparing `orbittools-0.0.1/LICENSE` & `orbittools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orbittools-0.0.1/pyproject.toml` & `orbittools-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "orbittools"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Eelco Doornbos", email="eelco.doornbos@knmi.nl" },
 ]
 description = "Some tools to generate and manipulate orbit ephemeris of satellites, mostly aimed at low Earth orbit"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,9 +16,7 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/eelcodoornbos/orbittools/"
 "Bug Tracker" = "https://gitlab.com/eelcodoornbos/orbittools/-/issues"
-
-
```

