# Comparing `tmp/nowcasting_forecast-1.3.7.tar.gz` & `tmp/nowcasting_forecast-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_forecast-1.3.7.tar", last modified: Thu May  4 12:24:20 2023, max compression
+gzip compressed data, was "nowcasting_forecast-1.3.8.tar", last modified: Thu May  4 17:10:35 2023, max compression
```

## Comparing `nowcasting_forecast-1.3.7.tar` & `nowcasting_forecast-1.3.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:24:20.245618 nowcasting_forecast-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-04 12:24:20.245618 nowcasting_forecast-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:24:20.245618 nowcasting_forecast-1.3.7/nowcasting_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:24:20.245618 nowcasting_forecast-1.3.7/nowcasting_forecast/models/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/models/nwp_solar_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/models/sun.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/nowcasting_forecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:24:20.245618 nowcasting_forecast-1.3.7/nowcasting_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-04 12:24:20.000000 nowcasting_forecast-1.3.7/nowcasting_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-04 12:24:20.000000 nowcasting_forecast-1.3.7/nowcasting_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:24:20.000000 nowcasting_forecast-1.3.7/nowcasting_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 12:24:20.000000 nowcasting_forecast-1.3.7/nowcasting_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 12:24:20.000000 nowcasting_forecast-1.3.7/nowcasting_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:24:20.245618 nowcasting_forecast-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:24:20.245618 nowcasting_forecast-1.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-04 12:24:06.000000 nowcasting_forecast-1.3.7/tests/test_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.516060 nowcasting_forecast-1.3.8/nowcasting_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/nowcasting_forecast/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/nwp_solar_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/sun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/nowcasting_forecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 17:10:35.000000 nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:10:35.520061 nowcasting_forecast-1.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-04 17:10:21.000000 nowcasting_forecast-1.3.8/tests/test_batch.py
```

### Comparing `nowcasting_forecast-1.3.7/LICENSE` & `nowcasting_forecast-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/PKG-INFO` & `nowcasting_forecast-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_forecast
-Version: 1.3.7
+Version: 1.3.8
 Summary: Live forecast for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_forecast
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: artificial intelligence,forecast
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_forecast-1.3.7/README.md` & `nowcasting_forecast-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast/app.py` & `nowcasting_forecast-1.3.8/nowcasting_forecast/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast/batch.py` & `nowcasting_forecast-1.3.8/nowcasting_forecast/batch.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast/dataloader.py` & `nowcasting_forecast-1.3.8/nowcasting_forecast/dataloader.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast/models/hub.py` & `nowcasting_forecast-1.3.8/nowcasting_forecast/models/hub.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast/models/nwp_solar_simple.py` & `nowcasting_forecast-1.3.8/nowcasting_forecast/models/nwp_solar_simple.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast/models/sun.py` & `nowcasting_forecast-1.3.8/nowcasting_forecast/models/sun.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast/models/utils.py` & `nowcasting_forecast-1.3.8/nowcasting_forecast/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast/utils.py` & `nowcasting_forecast-1.3.8/nowcasting_forecast/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast.egg-info/PKG-INFO` & `nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-forecast
-Version: 1.3.7
+Version: 1.3.8
 Summary: Live forecast for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_forecast
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: artificial intelligence,forecast
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_forecast-1.3.7/nowcasting_forecast.egg-info/SOURCES.txt` & `nowcasting_forecast-1.3.8/nowcasting_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/setup.py` & `nowcasting_forecast-1.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/tests/test_app.py` & `nowcasting_forecast-1.3.8/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.7/tests/test_batch.py` & `nowcasting_forecast-1.3.8/tests/test_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,33 +28,31 @@
 def test_make_batches_mvp_v1(nwp_data, pv_yields_and_systems):
     with tempfile.TemporaryDirectory() as temp_dir:
         # save nwp data
         nwp_path = f"{temp_dir}/unittest.netcdf"
         nwp_data.to_netcdf(nwp_path, engine="h5netcdf")
         os.environ["NWP_PATH"] = nwp_path
 
+        now_5 = (
+            pd.Timestamp(datetime.now(tz=timezone.utc)).floor("5T").replace(tzinfo=None).isoformat()
+        )
+
         make_batches(
             config_filename="nowcasting_forecast/config/mvp_v1.yaml",
             temporary_dir=temp_dir,
             n_gsps=10,
         )
 
         assert os.path.exists(f"{temp_dir}/live")
         assert os.path.exists(f"{temp_dir}/live/spatial_and_temporal_locations_of_each_example.csv")
 
         locations = pd.read_csv(
             f"{temp_dir}/live/spatial_and_temporal_locations_of_each_example.csv"
         )
-        assert (
-            pd.to_datetime(locations.iloc[0].t0_datetime_utc).isoformat()
-            == pd.Timestamp(datetime.now(tz=timezone.utc))
-            .floor("5T")
-            .replace(tzinfo=None)
-            .isoformat()
-        )
+        assert pd.to_datetime(locations.iloc[0].t0_datetime_utc).isoformat() == now_5
 
 
 def test_make_batches_mvp_v2_just_sat_data(sat_data):
     with tempfile.TemporaryDirectory() as temp_dir:
         configuration = load_yaml_configuration("nowcasting_forecast/config/mvp_v2.yaml")
 
         configuration.input_data.nwp = None
@@ -95,14 +93,27 @@
             hrv_sat_data.to_zarr(store, compute=True)
         os.environ["HRV_SAT_PATH"] = hrv_sat_path
         sat_path = f"{temp_dir}/sat_unittest.zarr.zip"
         with zarr.ZipStore(sat_path) as store:
             sat_data.to_zarr(store, compute=True)
         os.environ["SAT_PATH"] = sat_path
 
+        now_5 = (
+            pd.Timestamp(datetime.now(tz=timezone.utc))
+            .floor("30T")
+            .replace(tzinfo=None)
+            .isoformat()
+        )
+        now_30 = (
+            pd.Timestamp(datetime.now(tz=timezone.utc))
+            .floor("30T")
+            .replace(tzinfo=None)
+            .isoformat()
+        )
+
         make_batches(
             config_filename="nowcasting_forecast/config/pvnet_v1.yaml",
             temporary_dir=temp_dir,
             n_gsps=10,
         )
 
         # open pv files and check there is something in there
@@ -112,25 +123,13 @@
         assert os.path.exists(f"{temp_dir}/live/gsp")
         assert os.path.exists(f"{temp_dir}/live/satellite")
         assert os.path.exists(f"{temp_dir}/live/hrvsatellite")
         assert os.path.exists(f"{temp_dir}/live/gsp/000000.nc")
         pv = xr.load_dataset(f"{temp_dir}/live/pv/000000.nc", engine="h5netcdf")
         pv = PV(pv)
         # assert pv.power_mw.max() > 0
-        assert (
-            pd.to_datetime(pv.time.values[0, -1]).isoformat()
-            == pd.Timestamp(datetime.now(tz=timezone.utc))
-            .floor("5T")
-            .replace(tzinfo=None)
-            .isoformat()
-        )
+        assert pd.to_datetime(pv.time.values[0, -1]).isoformat() == now_5
 
         gsp = xr.load_dataset(f"{temp_dir}/live/gsp/000000.nc", engine="h5netcdf")
         gsp = GSP(gsp)
         assert len(gsp.time.values[0]) == 5
-        assert (
-            pd.to_datetime(gsp.time.values[0, -1]).isoformat()
-            == pd.Timestamp(datetime.now(tz=timezone.utc))
-            .floor("30T")
-            .replace(tzinfo=None)
-            .isoformat()
-        )
+        assert pd.to_datetime(gsp.time.values[0, -1]).isoformat() == now_30
```

