# Comparing `tmp/mxtools-1.0.3.tar.gz` & `tmp/mxtools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxtools-1.0.3.tar", last modified: Tue Apr 18 14:42:23 2023, max compression
+gzip compressed data, was "mxtools-1.0.4.tar", last modified: Thu May  4 19:59:33 2023, max compression
```

## Comparing `mxtools-1.0.3.tar` & `mxtools-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 14:42:12.000000 mxtools-1.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-18 14:42:12.000000 mxtools-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-18 14:42:12.000000 mxtools-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-18 14:42:12.000000 mxtools-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-18 14:42:23.524594 mxtools-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-18 14:42:12.000000 mxtools-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.520594 mxtools-1.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/min_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-18 14:42:12.000000 mxtools-1.0.3/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/mxtools/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 14:42:23.524594 mxtools-1.0.3/mxtools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/eiger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/governor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/raster_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/scans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/mxtools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/tests/test_examples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/vector_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-04-18 14:42:12.000000 mxtools-1.0.3/mxtools/zebra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:42:23.524594 mxtools-1.0.3/mxtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 14:42:23.000000 mxtools-1.0.3/mxtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-18 14:42:12.000000 mxtools-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 14:42:12.000000 mxtools-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-18 14:42:23.524594 mxtools-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-18 14:42:12.000000 mxtools-1.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68714 2023-04-18 14:42:12.000000 mxtools-1.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:59:33.332628 mxtools-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 19:59:17.000000 mxtools-1.0.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-04 19:59:17.000000 mxtools-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-04 19:59:17.000000 mxtools-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-04 19:59:17.000000 mxtools-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 19:59:33.332628 mxtools-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-04 19:59:17.000000 mxtools-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:59:33.328627 mxtools-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 19:59:17.000000 mxtools-1.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-04 19:59:17.000000 mxtools-1.0.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:59:33.328627 mxtools-1.0.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-05-04 19:59:17.000000 mxtools-1.0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-04 19:59:17.000000 mxtools-1.0.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 19:59:17.000000 mxtools-1.0.4/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-04 19:59:17.000000 mxtools-1.0.4/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 19:59:17.000000 mxtools-1.0.4/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 19:59:17.000000 mxtools-1.0.4/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:59:33.332628 mxtools-1.0.4/mxtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-04 19:59:33.332628 mxtools-1.0.4/mxtools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/eiger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/governor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/raster_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/scans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:59:33.332628 mxtools-1.0.4/mxtools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/tests/test_examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/vector_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-05-04 19:59:17.000000 mxtools-1.0.4/mxtools/zebra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:59:33.332628 mxtools-1.0.4/mxtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 19:59:33.000000 mxtools-1.0.4/mxtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-04 19:59:33.000000 mxtools-1.0.4/mxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:59:33.000000 mxtools-1.0.4/mxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 19:59:33.000000 mxtools-1.0.4/mxtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 19:59:33.000000 mxtools-1.0.4/mxtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 19:59:33.000000 mxtools-1.0.4/mxtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-04 19:59:17.000000 mxtools-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 19:59:17.000000 mxtools-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-04 19:59:33.332628 mxtools-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-04 19:59:17.000000 mxtools-1.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68714 2023-05-04 19:59:17.000000 mxtools-1.0.4/versioneer.py
```

### Comparing `mxtools-1.0.3/CONTRIBUTING.rst` & `mxtools-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/LICENSE` & `mxtools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/PKG-INFO` & `mxtools-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxtools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Common code for the MX beamlines at NSLS-II (AMX, FMX).
 Home-page: https://github.com/NSLS-II-AMX/mxtools
 Author: Jun Aishima
 Author-email: jaishima@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mxtools-1.0.3/docs/Makefile` & `mxtools-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/docs/make.bat` & `mxtools-1.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/docs/source/conf.py` & `mxtools-1.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/docs/source/min_versions.rst` & `mxtools-1.0.4/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/mxtools/eiger.py` & `mxtools-1.0.4/mxtools/eiger.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/mxtools/flyer.py` & `mxtools-1.0.4/mxtools/flyer.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,27 +166,23 @@
             return hf.get(f"entry/sample/goniometer/{field}")[()]
 
     def unstage(self):
         ttime.sleep(1.0)
         self.detector.unstage()
 
     def update_parameters(self, *args, **kwargs):
-        if self.detector.cam.armed.get() == 1:
-            raise RuntimeError("Detector must be unarmed in order to begin collection.")
-        self.detector_arm(**kwargs)
         self.configure_detector(**kwargs)
         self.configure_vector(**kwargs)
         self.configure_zebra(**kwargs)
 
     def configure_detector(self, **kwargs):
         file_prefix = kwargs["file_prefix"]
         data_directory_name = kwargs["data_directory_name"]
         self.detector.file.external_name.put(file_prefix)
         self.detector.file.write_path_template = data_directory_name
-        self.detector.file.file_write_images_per_file.put(500)
 
     def configure_vector(self, *args, **kwargs):
         angle_start = kwargs["angle_start"]
         scanWidth = kwargs["scan_width"]
         imgWidth = kwargs["img_width"]
         exposurePeriodPerImage = kwargs["exposure_period_per_image"]
         protocol = kwargs.get("protocol", "standard")
@@ -262,43 +258,43 @@
         self.detector.cam.file_owner_grp.put(grp.getgrgid(os.getgid())[0])
         self.detector.cam.file_perms.put(420)
         file_prefix_minus_directory = str(file_prefix)
         file_prefix_minus_directory = file_prefix_minus_directory.split("/")[-1]
 
         self.detector.cam.acquire_time.put(exposure_per_image)
         self.detector.cam.acquire_period.put(exposure_per_image)
+        # Trigger mode set before num_images due to updates in Eiger REST API
+        self.detector.cam.trigger_mode.put(eiger.EXTERNAL_SERIES)
         self.detector.cam.num_images.put(num_images)
         self.detector.cam.num_triggers.put(1)
         self.detector.cam.file_path.put(data_directory_name)
         self.detector.cam.fw_name_pattern.put(f"{file_prefix_minus_directory}_$id")
 
         self.detector.cam.sequence_id.put(file_number_start)
 
         # originally from detector_set_fileheader
         self.detector.cam.beam_center_x.put(x_beam)
         self.detector.cam.beam_center_y.put(y_beam)
         self.detector.cam.omega_incr.put(width)
         self.detector.cam.omega_start.put(start)
         self.detector.cam.wavelength.put(wavelength)
         self.detector.cam.det_distance.put(det_distance_m)
-        self.detector.cam.trigger_mode.put(eiger.EXTERNAL_SERIES)
 
-        start_arm = ttime.time()
+        self.detector.file.file_write_images_per_file.put(500)
 
         def armed_callback(value, old_value, **kwargs):
             if old_value == 0 and value == 1:
                 return True
             return False
 
         status = SubscriptionStatus(self.detector.cam.armed, armed_callback, run=False)
 
         self.detector.cam.acquire.put(1)
 
-        status.wait()
-        logger.info(f"arm time = {ttime.time() - start_arm}")
+        return status
 
     def setup_vector_program(
         self, num_images, angle_start, angle_end, x_um, y_um, z_um, exposure_period_per_image
     ):
         self.vector.num_frames.put(num_images)
         self.vector.start.omega.put(angle_start)
         self.vector.end.omega.put(angle_end)
```

### Comparing `mxtools-1.0.3/mxtools/governor.py` & `mxtools-1.0.4/mxtools/governor.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/mxtools/handlers.py` & `mxtools-1.0.4/mxtools/handlers.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/mxtools/raster_flyer.py` & `mxtools-1.0.4/mxtools/raster_flyer.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,44 +126,42 @@
         self.detector.cam.file_owner_grp.put(grp.getgrgid(os.getgid())[0])
         self.detector.cam.file_perms.put(420)
         file_prefix_minus_directory = str(file_prefix)
         file_prefix_minus_directory = file_prefix_minus_directory.split("/")[-1]
 
         self.detector.cam.acquire_time.put(exposure_per_image)
         self.detector.cam.acquire_period.put(exposure_per_image)
+        # Setting trigger mode before num_triggers due to change in Eiger REST API change
+        self.detector.cam.trigger_mode.put(eiger.EXTERNAL_ENABLE)
         self.detector.cam.num_triggers.put(total_num_images)
         self.detector.cam.file_path.put(data_directory_name)
         self.detector.cam.fw_name_pattern.put(f"{file_prefix_minus_directory}_$id")
 
         self.detector.cam.sequence_id.put(file_number_start)
 
         # originally from detector_set_fileheader
         self.detector.cam.beam_center_x.put(x_beam)
         self.detector.cam.beam_center_y.put(y_beam)
         self.detector.cam.omega_incr.put(width)
         self.detector.cam.omega_start.put(start)
         self.detector.cam.wavelength.put(wavelength)
         self.detector.cam.det_distance.put(det_distance_m)
-        self.detector.cam.trigger_mode.put(eiger.EXTERNAL_ENABLE)
 
         self.detector.file.file_write_images_per_file.put(num_images_per_file)
 
-        start_arm = ttime.time()
-
         def armed_callback(value, old_value, **kwargs):
             if old_value == 0 and value == 1:
                 return True
             return False
 
         status = SubscriptionStatus(self.detector.cam.armed, armed_callback, run=False)
 
         self.detector.cam.acquire.put(1)
 
-        status.wait()
-        logger.info(f"arm time = {ttime.time() - start_arm}")
+        return status
 
     def describe_collect(self):
         return {"stream_name": {}}
 
     def collect(self):
         logger.debug("raster_flyer.collect(): going to unstage now")
         yield {"data": {}, "timestamps": {}, "time": 0, "seq_num": 0}
```

### Comparing `mxtools-1.0.3/mxtools/scans.py` & `mxtools-1.0.4/mxtools/scans.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/mxtools/vector_program.py` & `mxtools-1.0.4/mxtools/vector_program.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/mxtools/zebra.py` & `mxtools-1.0.4/mxtools/zebra.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/mxtools.egg-info/PKG-INFO` & `mxtools-1.0.4/mxtools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxtools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Common code for the MX beamlines at NSLS-II (AMX, FMX).
 Home-page: https://github.com/NSLS-II-AMX/mxtools
 Author: Jun Aishima
 Author-email: jaishima@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mxtools-1.0.3/mxtools.egg-info/SOURCES.txt` & `mxtools-1.0.4/mxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/setup.py` & `mxtools-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `mxtools-1.0.3/versioneer.py` & `mxtools-1.0.4/versioneer.py`

 * *Files identical despite different names*

