# Comparing `tmp/ctapipe_io_magic-0.5.0.tar.gz` & `tmp/ctapipe_io_magic-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctapipe_io_magic-0.5.0.tar", last modified: Wed Apr 26 09:00:49 2023, max compression
+gzip compressed data, was "ctapipe_io_magic-0.5.1.tar", last modified: Thu May  4 09:02:18 2023, max compression
```

## Comparing `ctapipe_io_magic-0.5.0.tar` & `ctapipe_io_magic-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/
--rw-r--r--   0 shari90   (1000) shari90   (1000)     1090 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/LICENSE
--rw-r--r--   0 shari90   (1000) shari90   (1000)      159 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/MANIFEST.in
--rw-r--r--   0 shari90   (1000) shari90   (1000)     6861 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/PKG-INFO
--rw-r--r--   0 shari90   (1000) shari90   (1000)     6590 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/README.md
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/ctapipe_io_magic/
--rw-r--r--   0 shari90   (1000) shari90   (1000)    69468 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/__init__.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      160 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/_version.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      420 2023-04-19 10:27:57.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/constants.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)     1069 2023-04-17 09:32:56.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/mars_datalevels.py
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/ctapipe_io_magic/resources/
--rw-r--r--   0 shari90   (1000) shari90   (1000)     7189 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/
--rw-r--r--   0 shari90   (1000) shari90   (1000)    12801 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_magic_event_source.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      193 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_mars_datalevels.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)     2557 2023-04-17 09:32:56.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_stage1.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      106 2023-04-17 09:32:56.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_version.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)      844 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic/version.py
-drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/
--rw-r--r--   0 shari90   (1000) shari90   (1000)     6861 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/PKG-INFO
--rw-r--r--   0 shari90   (1000) shari90   (1000)      731 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/SOURCES.txt
--rw-r--r--   0 shari90   (1000) shari90   (1000)        1 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/dependency_links.txt
--rw-r--r--   0 shari90   (1000) shari90   (1000)      251 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/requires.txt
--rw-r--r--   0 shari90   (1000) shari90   (1000)       17 2023-04-26 09:00:49.000000 ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/top_level.txt
--rw-r--r--   0 shari90   (1000) shari90   (1000)     2232 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/download_test_data.sh
--rw-r--r--   0 shari90   (1000) shari90   (1000)      331 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/environment.yml
--rw-r--r--   0 shari90   (1000) shari90   (1000)      157 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/eventsource_subclasses.py
--rw-r--r--   0 shari90   (1000) shari90   (1000)     1153 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/example_stage1_config.json
--rw-r--r--   0 shari90   (1000) shari90   (1000)      130 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.0/pyproject.toml
--rw-r--r--   0 shari90   (1000) shari90   (1000)      357 2023-04-26 09:00:49.659794 ctapipe_io_magic-0.5.0/setup.cfg
--rw-r--r--   0 shari90   (1000) shari90   (1000)      749 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.0/setup.py
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1090 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/LICENSE
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      159 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/MANIFEST.in
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     6914 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/PKG-INFO
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     6645 2023-05-04 08:57:20.000000 ctapipe_io_magic-0.5.1/README.md
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/ctapipe_io_magic/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)    74479 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/__init__.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      160 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/_version.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      420 2023-04-19 10:27:57.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/constants.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1069 2023-04-17 09:32:56.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/mars_datalevels.py
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/ctapipe_io_magic/resources/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     7189 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)    13436 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_magic_event_source.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      193 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_mars_datalevels.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     2685 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_stage1.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      106 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_version.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      844 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic/version.py
+drwxr-xr-x   0 shari90   (1000) shari90   (1000)        0 2023-05-04 09:02:18.179339 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     6914 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/PKG-INFO
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      774 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)        1 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)       66 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/entry_points.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      251 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/requires.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)       17 2023-05-04 09:02:18.000000 ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/top_level.txt
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     2232 2023-04-28 12:47:55.000000 ctapipe_io_magic-0.5.1/download_test_data.sh
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      335 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/environment.yml
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      123 2023-05-04 08:57:20.000000 ctapipe_io_magic-0.5.1/eventsource_subclasses.py
+-rw-r--r--   0 shari90   (1000) shari90   (1000)     1153 2023-04-26 08:57:04.000000 ctapipe_io_magic-0.5.1/example_stage1_config.json
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      130 2023-03-07 09:23:38.000000 ctapipe_io_magic-0.5.1/pyproject.toml
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      357 2023-05-04 09:02:18.189339 ctapipe_io_magic-0.5.1/setup.cfg
+-rw-r--r--   0 shari90   (1000) shari90   (1000)      846 2023-05-04 07:53:54.000000 ctapipe_io_magic-0.5.1/setup.py
```

### Comparing `ctapipe_io_magic-0.5.0/LICENSE` & `ctapipe_io_magic-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.0/PKG-INFO` & `ctapipe_io_magic-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ctapipe_io_magic
-Version: 0.5.0
+Version: 0.5.1
 Summary: ctapipe plugin for reading calibrated MAGIC files
 Home-page: https://github.com/cta-observatory/ctapipe_io_magic
 Author: Ievgen Vovk et al.
 Author-email: Ievgen.Vovk@mpp.mpg.de
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 ## *ctapipe* MAGIC event source
 
-EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.17.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
+EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.19.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
 
 #### Installation
 
 If *ctapipe* is already installed, the installation can be done via *pip* (the module is available in PyPI):
 
 ```bash
 pip install ctapipe_io_magic
@@ -121,8 +121,10 @@
 -   v0.4.1: added CI, refactoring of code, added tests, extract drive information once
 -   v0.4.2: added more tests, refactored code, allow the processing of all subruns from the same run at the same time (including drive information), correct de-rotation of quantities from the CORSIKA frame to the geographical frame, computation of bad pixels, modification of focal length to take into account the coma aberration, fix dowload of test data set
 -   v0.4.3: difference of arrival times between events read from ROOT files, used for effective observation time calculation
 -   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
 -   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
 -   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
 -   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
--   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the correct value used in MAGIC simulations (i.e. 16.97 meters)
+-   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the
+    correct value used in MAGIC simulations (i.e. 16.97 meters)
+-   v0.5.1: release compatible with ctapipe 0.19
```

### Comparing `ctapipe_io_magic-0.5.0/README.md` & `ctapipe_io_magic-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## *ctapipe* MAGIC event source
 
-EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.17.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
+EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.19.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
 
 #### Installation
 
 If *ctapipe* is already installed, the installation can be done via *pip* (the module is available in PyPI):
 
 ```bash
 pip install ctapipe_io_magic
@@ -107,8 +107,10 @@
 -   v0.4.1: added CI, refactoring of code, added tests, extract drive information once
 -   v0.4.2: added more tests, refactored code, allow the processing of all subruns from the same run at the same time (including drive information), correct de-rotation of quantities from the CORSIKA frame to the geographical frame, computation of bad pixels, modification of focal length to take into account the coma aberration, fix dowload of test data set
 -   v0.4.3: difference of arrival times between events read from ROOT files, used for effective observation time calculation
 -   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
 -   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
 -   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
 -   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
--   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the correct value used in MAGIC simulations (i.e. 16.97 meters)
+-   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the
+    correct value used in MAGIC simulations (i.e. 16.97 meters)
+-   v0.5.1: release compatible with ctapipe 0.19
```

### Comparing `ctapipe_io_magic-0.5.0/ctapipe_io_magic/__init__.py` & `ctapipe_io_magic-0.5.1/ctapipe_io_magic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,24 +51,20 @@
     MC_STEREO_AND_MONO_TRIGGER_PATTERN,
     MC_SUMT_TRIGGER_PATTERN,
     DATA_MONO_SUMT_TRIGGER_PATTERN,
     PEDESTAL_TRIGGER_PATTERN,
     DATA_STEREO_TRIGGER_PATTERN,
 )
 
-__all__ = [
-    'MAGICEventSource',
-    'MARSDataLevel',
-    '__version__'
-]
+__all__ = ["MAGICEventSource", "MARSDataLevel", "__version__"]
 
 logger = logging.getLogger(__name__)
 
 degrees_per_hour = 15.0
-seconds_per_hour = 3600.
+seconds_per_hour = 3600.0
 
 msec2sec = 1e-3
 nsec2sec = 1e-9
 
 mc_data_type = 256
 
 MAGIC_TO_CTA_EVENT_TYPE = {
@@ -78,18 +74,16 @@
     DATA_STEREO_TRIGGER_PATTERN: EventType.SUBARRAY,
     DATA_MONO_SUMT_TRIGGER_PATTERN: EventType.SUBARRAY,
     PEDESTAL_TRIGGER_PATTERN: EventType.SKY_PEDESTAL,
 }
 
 
 def load_camera_geometry():
-    ''' Load camera geometry from bundled resources of this repo '''
-    f = resource_filename(
-        'ctapipe_io_magic', 'resources/MAGICCam.camgeom.fits.gz'
-    )
+    """Load camera geometry from bundled resources of this repo"""
+    f = resource_filename("ctapipe_io_magic", "resources/MAGICCam.camgeom.fits.gz")
     Provenance().add_input_file(f, role="CameraGeometry")
     return CameraGeometry.from_table(f)
 
 
 class MissingDriveReportError(Exception):
     """
     Exception raised when a subrun does not have drive reports.
@@ -125,32 +119,30 @@
     telescope : int
         The number of the telescope
     use_pedestals : bool
         Flag indicating if pedestal events should be returned by the generator
     """
 
     process_run = Bool(
-        default_value=True,
-        help='Read all subruns from a given run.'
+        default_value=True, help="Read all subruns from a given run."
     ).tag(config=True)
 
     use_pedestals = Bool(
-        default_value=False,
-        help='Extract pedestal events instead of cosmic events.'
+        default_value=False, help="Extract pedestal events instead of cosmic events."
     ).tag(config=True)
 
     use_mc_mono_events = Bool(
         default_value=False,
-        help='Use mono events in MC stereo data (needed for mono analysis).'
+        help="Use mono events in MC stereo data (needed for mono analysis).",
     ).tag(config=True)
 
     focal_length_choice = UseEnum(
         FocalLengthKind,
         default_value=FocalLengthKind.EFFECTIVE,
-        help='Which focal length to use when constructing the SubarrayDescription.',
+        help="Which focal length to use when constructing the SubarrayDescription.",
     ).tag(config=True)
 
     def __init__(self, input_url=None, config=None, parent=None, **kwargs):
         """
         Constructor
 
         Parameters
@@ -165,20 +157,15 @@
             Set to None if no Tool to pass.
         kwargs: dict
             Additional parameters to be passed.
             NOTE: The file mask of the data to read can be passed with
             the 'input_url' parameter.
         """
 
-        super().__init__(
-            input_url=input_url,
-            config=config,
-            parent=parent,
-            **kwargs
-        )
+        super().__init__(input_url=input_url, config=config, parent=parent, **kwargs)
 
         path, name = os.path.split(os.path.abspath(self.input_url))
         info_tuple = self.get_run_info_from_name(name)
         run = info_tuple[0]
         telescope = info_tuple[2]
 
         regex = rf"\d{{8}}_M{telescope}_0{run}\.\d{{3}}_Y_.*\.root"
@@ -187,15 +174,18 @@
         reg_comp = re.compile(regex)
         reg_comp_mc = re.compile(regex_mc)
 
         ls = Path(path).iterdir()
         self.file_list_drive = []
 
         for file_path in ls:
-            if reg_comp.match(file_path.name) is not None or reg_comp_mc.match(file_path.name) is not None:
+            if (
+                reg_comp.match(file_path.name) is not None
+                or reg_comp_mc.match(file_path.name) is not None
+            ):
                 self.file_list_drive.append(file_path)
 
         self.file_list_drive.sort()
 
         if self.process_run:
             self.file_list = self.file_list_drive
         else:
@@ -217,20 +207,24 @@
 
         if self.is_simulation:
             self._simulation_config = self.parse_simulation_header()
 
         self.is_stereo, self.is_sumt = self.parse_data_info()
 
         if self.is_simulation and self.use_mc_mono_events and not self.is_stereo:
-            logger.warning("Processing mono simulation data with" \
-                " use_mc_mono_events=True. use_mc_mono_events will be ignored.")
+            logger.warning(
+                "Processing mono simulation data with"
+                " use_mc_mono_events=True. use_mc_mono_events will be ignored."
+            )
 
         if not self.is_simulation and self.use_mc_mono_events:
-            logger.warning("Processing real data with" \
-                " use_mc_mono_events=True. use_mc_mono_events will be ignored.")
+            logger.warning(
+                "Processing real data with"
+                " use_mc_mono_events=True. use_mc_mono_events will be ignored."
+            )
 
         # # Setting up the current run with the first run present in the data
         # self.current_run = self._set_active_run(run_number=0)
         self.current_run = None
 
         self._subarray_info = self.prepare_subarray_info()
 
@@ -300,15 +294,15 @@
             True if the masked files are MAGIC data runs, False otherwise.
         """
 
         is_magic_root_file = True
 
         try:
             with uproot.open(file_path) as input_data:
-                mandatory_trees = ['Events', 'RunHeaders', 'RunTails']
+                mandatory_trees = ["Events", "RunHeaders", "RunTails"]
                 trees_in_file = [tree in input_data for tree in mandatory_trees]
                 if not all(trees_in_file):
                     is_magic_root_file = False
         except ValueError:
             # uproot raises ValueError if the file is not a ROOT file
             is_magic_root_file = False
 
@@ -399,15 +393,15 @@
             run_number = None
             datalevel = MARSDataLevel.MELIBEA
             is_mc = True
         else:
             raise IndexError(
                 f"Can not identify the run number and type (data/MC) "
                 f"of the file {file_name}."
-                )
+            )
 
         return run_number, is_mc, telescope, datalevel
 
     def parse_run_info(self):
         """
         Parses run info from the TTrees in the ROOT file
 
@@ -420,31 +414,29 @@
         telescope_number: int
             Number of the telescope
         datalevel: MARSDataLevel
             Data level according to MARS
         """
 
         runinfo_array_list = [
-            'MRawRunHeader.fRunNumber',
-            'MRawRunHeader.fRunType',
-            'MRawRunHeader.fTelescopeNumber',
+            "MRawRunHeader.fRunNumber",
+            "MRawRunHeader.fRunType",
+            "MRawRunHeader.fTelescopeNumber",
         ]
 
         run_numbers = []
         is_simulation = []
         telescope_numbers = []
         datalevels = []
 
         for rootf in self.files_:
-
-            run_info = rootf['RunHeaders'].arrays(
-                runinfo_array_list, library="np")
-            run_number = int(run_info['MRawRunHeader.fRunNumber'][0])
-            run_type = int(run_info['MRawRunHeader.fRunType'][0])
-            telescope_number = int(run_info['MRawRunHeader.fTelescopeNumber'][0])
+            run_info = rootf["RunHeaders"].arrays(runinfo_array_list, library="np")
+            run_number = int(run_info["MRawRunHeader.fRunNumber"][0])
+            run_type = int(run_info["MRawRunHeader.fRunType"][0])
+            telescope_number = int(run_info["MRawRunHeader.fTelescopeNumber"][0])
 
             # a note about run numbers:
             # mono data has run numbers starting with 1 or 2 (telescope dependent)
             # stereo data has run numbers starting with 5
             # if both telescopes are taking data with no L3,
             # also in this case run number starts with 5 (e.g. muon runs)
 
@@ -459,19 +451,19 @@
             # none = 65535
 
             if run_type == mc_data_type:
                 is_mc = True
             else:
                 is_mc = False
 
-            events_tree = rootf['Events']
+            events_tree = rootf["Events"]
 
-            melibea_trees = ['MHadronness', 'MStereoParDisp', 'MEnergyEst']
-            superstar_trees = ['MHillas_1', 'MHillas_2', 'MStereoPar']
-            star_trees = ['MHillas']
+            melibea_trees = ["MHadronness", "MStereoParDisp", "MEnergyEst"]
+            superstar_trees = ["MHillas_1", "MHillas_2", "MStereoPar"]
+            star_trees = ["MHillas"]
 
             datalevel = MARSDataLevel.CALIBRATED
             events_keys = events_tree.keys()
             trees_in_file = [tree in events_keys for tree in melibea_trees]
             if all(trees_in_file):
                 datalevel = MARSDataLevel.MELIBEA
             trees_in_file = [tree in events_keys for tree in superstar_trees]
@@ -490,23 +482,26 @@
         is_simulation = np.unique(is_simulation).tolist()
         telescope_numbers = np.unique(telescope_numbers).tolist()
         datalevels = np.unique(datalevels).tolist()
 
         if len(is_simulation) > 1:
             raise ValueError(
                 "Loaded files contain both real data and simulation runs. \
-                 Please load only data OR Monte Carlos.")
+                 Please load only data OR Monte Carlos."
+            )
         if len(telescope_numbers) > 1:
             raise ValueError(
                 "Loaded files contain data from different telescopes. \
-                 Please load data belonging to the same telescope.")
+                 Please load data belonging to the same telescope."
+            )
         if len(datalevels) > 1:
             raise ValueError(
                 "Loaded files contain data at different datalevels. \
-                 Please load data belonging to the same datalevel.")
+                 Please load data belonging to the same datalevel."
+            )
 
         return run_numbers, is_simulation, telescope_numbers, datalevels
 
     def parse_data_info(self):
         """
         Check if data is stereo/mono and std trigger/SUMT
 
@@ -529,47 +524,55 @@
             # L1_table_mono = "L1_4NN"
             # L1_table_stereo = "L1_3NN"
 
             L3_table_nosumt = "L3T_L1L1_100_SYNC"
             L3_table_sumt = "L3T_SUMSUM_100_SYNC"
 
             for rootf in self.files_:
-
                 trigger_tree = rootf["Trigger"]
                 L3T_tree = rootf["L3T"]
 
                 # here we take the 2nd element (if possible) because sometimes
                 # the first trigger report has still the old prescaler values from a previous run
                 try:
-                    prescaler_array = trigger_tree["MTriggerPrescFact.fPrescFact"].array(library="np")
+                    prescaler_array = trigger_tree[
+                        "MTriggerPrescFact.fPrescFact"
+                    ].array(library="np")
                 except AssertionError:
-                    logger.warning("No prescaler info found. Will assume standard stereo data.")
+                    logger.warning(
+                        "No prescaler info found. Will assume standard stereo data."
+                    )
                     stereo = True
                     sumt = False
                     return stereo, sumt
 
                 prescaler_size = prescaler_array.size
                 if prescaler_size > 1:
                     prescaler = list(prescaler_array[1])
                 else:
                     prescaler = list(prescaler_array[0])
 
-                if prescaler == prescaler_mono_nosumt or prescaler == prescaler_mono_sumt:
+                if (
+                    prescaler == prescaler_mono_nosumt
+                    or prescaler == prescaler_mono_sumt
+                ):
                     stereo = False
                 elif prescaler == prescaler_stereo:
                     stereo = True
                 else:
                     stereo = True
 
                 sumt = False
                 if stereo:
                     # here we take the 2nd element for the same reason as above
                     # L3Table is empty for mono data i.e. taken with one telescope only
                     # if both telescopes take data with no L3, L3Table is filled anyway
-                    L3Table_array = L3T_tree["MReportL3T.fTablename"].array(library="np")
+                    L3Table_array = L3T_tree["MReportL3T.fTablename"].array(
+                        library="np"
+                    )
                     L3Table_size = L3Table_array.size
                     if L3Table_size > 1:
                         L3Table = L3Table_array[1]
                     else:
                         L3Table = L3Table_array[0]
 
                     if L3Table == L3_table_sumt:
@@ -584,44 +587,53 @@
 
                 is_stereo.append(stereo)
                 is_sumt.append(sumt)
 
         else:
             for rootf in self.files_:
                 # looking into MC data, when SumT is simulated, trigger pattern of all events is set to 32 (bit 5), except the first (set to 0)
-                trigger_pattern_array_unique = np.unique(rootf["Events"]["MTriggerPattern.fPrescaled"].array(library="np")[1:])
+                trigger_pattern_array_unique = np.unique(
+                    rootf["Events"]["MTriggerPattern.fPrescaled"].array(library="np")[
+                        1:
+                    ]
+                )
                 if len(trigger_pattern_array_unique) == 1:
                     if trigger_pattern_array_unique[0] == MC_SUMT_TRIGGER_PATTERN:
                         sumt = True
                     else:
                         sumt = False
                 else:
                     sumt = False
                 is_sumt.append(sumt)
 
                 # looking into MC data, MMcCorsikaRunHeader.fNumCT is set to 1 if mono, 2 if stereo
-                num_telescopes = rootf["RunHeaders"]["MMcCorsikaRunHeader.fNumCT"].array(library="np")[0]
+                num_telescopes = rootf["RunHeaders"][
+                    "MMcCorsikaRunHeader.fNumCT"
+                ].array(library="np")[0]
                 if num_telescopes == 1:
                     stereo = False
                 else:
                     stereo = True
 
                 is_stereo.append(stereo)
 
         is_stereo = np.unique(is_stereo).tolist()
         is_sumt = np.unique(is_sumt).tolist()
 
         if len(is_stereo) > 1:
             raise ValueError(
                 "Loaded files contain both stereo and mono data. \
-                 Please load only stereo or mono.")
+                 Please load only stereo or mono."
+            )
 
         if len(is_sumt) > 1:
-            logger.warning("Found data with both standard and Sum trigger. While this is \
-                not an issue, check that this is what you really want to do.")
+            logger.warning(
+                "Found data with both standard and Sum trigger. While this is \
+                not an issue, check that this is what you really want to do."
+            )
 
         return is_stereo[0], is_sumt[0]
 
     def prepare_subarray_info(self):
         """
         Fill SubarrayDescription container
 
@@ -637,93 +649,98 @@
         #    2: [-96.44, -96.77, 51.00] * u.m
         # }
 
         # MAGIC telescope positions in m wrt. to the center of MAGIC simulations, from
         # CORSIKA and reflector input card and recomputed (rotated) to be w.r.t. geographical North
         MAGIC_TEL_POSITIONS = {
             1: [34.99, -24.02, 0.00] * u.m,
-            2: [-34.99, 24.02, 0.00] * u.m
+            2: [-34.99, 24.02, 0.00] * u.m,
         }
 
         equivalent_focal_length = u.Quantity(16.97, u.m)
-        effective_focal_length = u.Quantity(17*1.0713, u.m)
+        effective_focal_length = u.Quantity(17 * 1.0713, u.m)
 
         OPTICS = OpticsDescription(
-            name='MAGIC',
+            name="MAGIC",
             size_type=SizeType.LST,
             n_mirrors=1,
             n_mirror_tiles=964,
             reflector_shape=ReflectorShape.PARABOLIC,
             equivalent_focal_length=equivalent_focal_length,
             effective_focal_length=effective_focal_length,
             mirror_area=u.Quantity(239.0, u.m**2),
         )
 
         if self.focal_length_choice is FocalLengthKind.EFFECTIVE:
             focal_length = effective_focal_length
         elif self.focal_length_choice is FocalLengthKind.EQUIVALENT:
             focal_length = equivalent_focal_length
         else:
-            raise ValueError(
-                f"Invalid focal length choice: {self.focal_length_choice}"
-            )
+            raise ValueError(f"Invalid focal length choice: {self.focal_length_choice}")
 
         # camera info from MAGICCam.camgeom.fits.gz file
         camera_geom = load_camera_geometry()
 
         n_pixels = camera_geom.n_pixels
 
         n_samples_array_list = ["MRawRunHeader.fNumSamplesHiGain"]
         n_samples_list = []
 
         for rootf in self.files_:
-            nsample_info = rootf['RunHeaders'].arrays(n_samples_array_list, library="np")
-            n_samples_file = int(nsample_info['MRawRunHeader.fNumSamplesHiGain'][0])
+            nsample_info = rootf["RunHeaders"].arrays(
+                n_samples_array_list, library="np"
+            )
+            n_samples_file = int(nsample_info["MRawRunHeader.fNumSamplesHiGain"][0])
             n_samples_list.append(n_samples_file)
 
         n_samples_list = np.unique(n_samples_list).tolist()
 
         if len(n_samples_list) > 1:
             raise ValueError(
                 "Loaded files contain different number of readout samples. \
-                 Please load files with the same readout configuration.")
+                 Please load files with the same readout configuration."
+            )
 
         n_samples = n_samples_list[0]
 
-        pulse_shape_lo_gain = np.array([0., 1., 2., 1., 0.])
-        pulse_shape_hi_gain = np.array([1., 2., 3., 2., 1.])
+        pulse_shape_lo_gain = np.array([0.0, 1.0, 2.0, 1.0, 0.0])
+        pulse_shape_hi_gain = np.array([1.0, 2.0, 3.0, 2.0, 1.0])
+
         pulse_shape = np.vstack((pulse_shape_lo_gain, pulse_shape_hi_gain))
         sampling_speed = u.Quantity(
-            self.files_[0]['RunHeaders']['MRawRunHeader.fSamplingFrequency'].array(library='np')[0]/1000,
-            u.GHz
+            self.files_[0]["RunHeaders"]["MRawRunHeader.fSamplingFrequency"].array(
+                library="np"
+            )[0]
+            / 1000,
+            u.GHz,
         )
         camera_readout = CameraReadout(
-            name='MAGICCam',
+            name="MAGICCam",
             sampling_rate=sampling_speed,
             reference_pulse_shape=pulse_shape,
             reference_pulse_sample_width=u.Quantity(0.5, u.ns),
             n_channels=1,
             n_pixels=n_pixels,
             n_samples=n_samples,
         )
 
-        camera = CameraDescription('MAGICCam', camera_geom, camera_readout)
+        camera = CameraDescription("MAGICCam", camera_geom, camera_readout)
 
         camera.geometry.frame = CameraFrame(focal_length=focal_length)
 
         MAGIC_TEL_DESCRIPTION = TelescopeDescription(
-            name='MAGIC', optics=OPTICS, camera=camera
+            name="MAGIC", optics=OPTICS, camera=camera
         )
 
         MAGIC_TEL_DESCRIPTIONS = {1: MAGIC_TEL_DESCRIPTION, 2: MAGIC_TEL_DESCRIPTION}
 
         subarray = SubarrayDescription(
-            name='MAGIC',
+            name="MAGIC",
             tel_positions=MAGIC_TEL_POSITIONS,
-            tel_descriptions=MAGIC_TEL_DESCRIPTIONS
+            tel_descriptions=MAGIC_TEL_DESCRIPTIONS,
         )
 
         if self.allowed_tels:
             subarray = subarray.select_subarray(self.allowed_tels)
 
         return subarray
 
@@ -742,15 +759,15 @@
         version_decoded: str
             Version decoded as major.minor.patch
         """
 
         major_version = version_encoded >> 16
         minor_version = (version_encoded % 65536) >> 8
         patch_version = (version_encoded % 65536) % 256
-        version_decoded = f'{major_version}.{minor_version}.{patch_version}'
+        version_decoded = f"{major_version}.{minor_version}.{patch_version}"
 
         return version_decoded
 
     def parse_metadata_info(self):
         """
         Parse metadata information from ROOT file
 
@@ -767,71 +784,90 @@
             - observation mode (real data only)
             - project name (real data only)
             - MARS version
             - ROOT version
         """
 
         metadatainfo_array_list_runheaders = [
-            'MRawRunHeader.fSubRunIndex',
-            'MRawRunHeader.fSourceRA',
-            'MRawRunHeader.fSourceDEC',
-            'MRawRunHeader.fSourceName[80]',
-            'MRawRunHeader.fObservationMode[60]',
-            'MRawRunHeader.fProjectName[100]',
+            "MRawRunHeader.fSubRunIndex",
+            "MRawRunHeader.fSourceRA",
+            "MRawRunHeader.fSourceDEC",
+            "MRawRunHeader.fSourceName[80]",
+            "MRawRunHeader.fObservationMode[60]",
+            "MRawRunHeader.fProjectName[100]",
         ]
 
         metadatainfo_array_list_runtails = [
-            'MMarsVersion_sorcerer.fMARSVersionCode',
-            'MMarsVersion_sorcerer.fROOTVersionCode',
+            "MMarsVersion_sorcerer.fMARSVersionCode",
+            "MMarsVersion_sorcerer.fROOTVersionCode",
         ]
 
         metadata = dict()
         metadata["file_list"] = self.file_list
-        metadata['run_numbers'] = self.run_id
-        metadata['is_simulation'] = self.is_simulation
-        metadata['telescope'] = self.telescope
-        metadata['subrun_number'] = []
-        metadata['source_ra'] = []
-        metadata['source_dec'] = []
-        metadata['source_name'] = []
-        metadata['observation_mode'] = []
-        metadata['project_name'] = []
-        metadata['mars_version_sorcerer'] = []
-        metadata['root_version_sorcerer'] = []
+        metadata["run_numbers"] = self.run_id
+        metadata["is_simulation"] = self.is_simulation
+        metadata["telescope"] = self.telescope
+        metadata["subrun_number"] = []
+        metadata["source_ra"] = []
+        metadata["source_dec"] = []
+        metadata["source_name"] = []
+        metadata["observation_mode"] = []
+        metadata["project_name"] = []
+        metadata["mars_version_sorcerer"] = []
+        metadata["root_version_sorcerer"] = []
 
         for rootf in self.files_:
-
-            meta_info_runh = rootf['RunHeaders'].arrays(
-                    metadatainfo_array_list_runheaders, library="np"
+            meta_info_runh = rootf["RunHeaders"].arrays(
+                metadatainfo_array_list_runheaders, library="np"
             )
 
-            metadata['subrun_number'].append(int(meta_info_runh['MRawRunHeader.fSubRunIndex'][0]))
-            metadata['source_ra'].append(
-                meta_info_runh['MRawRunHeader.fSourceRA'][0] / seconds_per_hour * degrees_per_hour * u.deg
+            metadata["subrun_number"].append(
+                int(meta_info_runh["MRawRunHeader.fSubRunIndex"][0])
             )
-            metadata['source_dec'].append(
-                meta_info_runh['MRawRunHeader.fSourceDEC'][0] / seconds_per_hour * u.deg
+            metadata["source_ra"].append(
+                meta_info_runh["MRawRunHeader.fSourceRA"][0]
+                / seconds_per_hour
+                * degrees_per_hour
+                * u.deg
+            )
+            metadata["source_dec"].append(
+                meta_info_runh["MRawRunHeader.fSourceDEC"][0] / seconds_per_hour * u.deg
             )
             if not self.is_simulation:
-                src_name_array = meta_info_runh['MRawRunHeader.fSourceName[80]'][0]
-                metadata['source_name'].append("".join([chr(item) for item in src_name_array if item != 0]))
-                obs_mode_array = meta_info_runh['MRawRunHeader.fObservationMode[60]'][0]
-                metadata['observation_mode'].append("".join([chr(item) for item in obs_mode_array if item != 0]))
-                project_name_array = meta_info_runh['MRawRunHeader.fProjectName[100]'][0]
-                metadata['project_name'].append("".join([chr(item) for item in project_name_array if item != 0]))
+                src_name_array = meta_info_runh["MRawRunHeader.fSourceName[80]"][0]
+                metadata["source_name"].append(
+                    "".join([chr(item) for item in src_name_array if item != 0])
+                )
+                obs_mode_array = meta_info_runh["MRawRunHeader.fObservationMode[60]"][0]
+                metadata["observation_mode"].append(
+                    "".join([chr(item) for item in obs_mode_array if item != 0])
+                )
+                project_name_array = meta_info_runh["MRawRunHeader.fProjectName[100]"][
+                    0
+                ]
+                metadata["project_name"].append(
+                    "".join([chr(item) for item in project_name_array if item != 0])
+                )
 
-            meta_info_runt = rootf['RunTails'].arrays(
-                metadatainfo_array_list_runtails,
-                library="np"
+            meta_info_runt = rootf["RunTails"].arrays(
+                metadatainfo_array_list_runtails, library="np"
             )
 
-            mars_version_encoded = int(meta_info_runt['MMarsVersion_sorcerer.fMARSVersionCode'][0])
-            root_version_encoded = int(meta_info_runt['MMarsVersion_sorcerer.fROOTVersionCode'][0])
-            metadata['mars_version_sorcerer'].append(self.decode_version_number(mars_version_encoded))
-            metadata['root_version_sorcerer'].append(self.decode_version_number(root_version_encoded))
+            mars_version_encoded = int(
+                meta_info_runt["MMarsVersion_sorcerer.fMARSVersionCode"][0]
+            )
+            root_version_encoded = int(
+                meta_info_runt["MMarsVersion_sorcerer.fROOTVersionCode"][0]
+            )
+            metadata["mars_version_sorcerer"].append(
+                self.decode_version_number(mars_version_encoded)
+            )
+            metadata["root_version_sorcerer"].append(
+                self.decode_version_number(root_version_encoded)
+            )
 
         return metadata
 
     def parse_simulation_header(self):
         """
         Parse the simulation information from the RunHeaders tree.
 
@@ -863,49 +899,103 @@
         # i.e. B y-component is 0
         # MAGIC_Bdec is the magnetic declination i.e. angle between magnetic and
         # geographic north, negative if pointing westwards, positive if pointing
         # eastwards
         # MAGIC_Binc is the magnetic field inclination
         MAGIC_Bx = u.Quantity(29.5, u.uT)
         MAGIC_Bz = u.Quantity(23.0, u.uT)
-        MAGIC_Btot = np.sqrt(MAGIC_Bx**2+MAGIC_Bz**2)
+        MAGIC_Btot = np.sqrt(MAGIC_Bx**2 + MAGIC_Bz**2)
         MAGIC_Bdec = u.Quantity(-7.0, u.deg).to(u.rad)
         MAGIC_Binc = u.Quantity(np.arctan2(-MAGIC_Bz.value, MAGIC_Bx.value), u.rad)
 
         simulation_config = dict()
 
         for rootf in self.files_:
-
-            run_header_tree = rootf['RunHeaders']
-            spectral_index = run_header_tree['MMcCorsikaRunHeader.fSlopeSpec'].array(library="np")[0]
-            e_low = run_header_tree['MMcCorsikaRunHeader.fELowLim'].array(library="np")[0]
-            e_high = run_header_tree['MMcCorsikaRunHeader.fEUppLim'].array(library="np")[0]
-            corsika_version = run_header_tree['MMcCorsikaRunHeader.fCorsikaVersion'].array(library="np")[0]
-            site_height = run_header_tree['MMcCorsikaRunHeader.fHeightLev[10]'].array(library="np")[0][0]
-            atm_model = run_header_tree['MMcCorsikaRunHeader.fAtmosphericModel'].array(library="np")[0]
+            run_header_tree = rootf["RunHeaders"]
+            spectral_index = run_header_tree["MMcCorsikaRunHeader.fSlopeSpec"].array(
+                library="np"
+            )[0]
+            e_low = run_header_tree["MMcCorsikaRunHeader.fELowLim"].array(library="np")[
+                0
+            ]
+            e_high = run_header_tree["MMcCorsikaRunHeader.fEUppLim"].array(
+                library="np"
+            )[0]
+            corsika_version = run_header_tree[
+                "MMcCorsikaRunHeader.fCorsikaVersion"
+            ].array(library="np")[0]
+            site_height = run_header_tree["MMcCorsikaRunHeader.fHeightLev[10]"].array(
+                library="np"
+            )[0][0]
+            atm_model = run_header_tree["MMcCorsikaRunHeader.fAtmosphericModel"].array(
+                library="np"
+            )[0]
             if self.mars_datalevel in [MARSDataLevel.CALIBRATED, MARSDataLevel.STAR]:
-                view_cone = run_header_tree['MMcRunHeader.fRandomPointingConeSemiAngle'].array(library="np")[0]
-                max_impact = run_header_tree['MMcRunHeader.fImpactMax'].array(library="np")[0]
-                n_showers = np.sum(run_header_tree['MMcRunHeader.fNumSimulatedShowers'].array(library="np"))
-                max_zd = run_header_tree['MMcRunHeader.fShowerThetaMax'].array(library="np")[0]
-                min_zd = run_header_tree['MMcRunHeader.fShowerThetaMin'].array(library="np")[0]
-                max_az = run_header_tree['MMcRunHeader.fShowerPhiMax'].array(library="np")[0]
-                min_az = run_header_tree['MMcRunHeader.fShowerPhiMin'].array(library="np")[0]
-                max_wavelength = run_header_tree['MMcRunHeader.fCWaveUpper'].array(library="np")[0]
-                min_wavelength = run_header_tree['MMcRunHeader.fCWaveLower'].array(library="np")[0]
-            elif self.mars_datalevel in [MARSDataLevel.SUPERSTAR, MARSDataLevel.MELIBEA]:
-                view_cone = run_header_tree['MMcRunHeader_1.fRandomPointingConeSemiAngle'].array(library="np")[0]
-                max_impact = run_header_tree['MMcRunHeader_1.fImpactMax'].array(library="np")[0]
-                n_showers = np.sum(run_header_tree['MMcRunHeader_1.fNumSimulatedShowers'].array(library="np"))
-                max_zd = run_header_tree['MMcRunHeader_1.fShowerThetaMax'].array(library="np")[0]
-                min_zd = run_header_tree['MMcRunHeader_1.fShowerThetaMin'].array(library="np")[0]
-                max_az = run_header_tree['MMcRunHeader_1.fShowerPhiMax'].array(library="np")[0]
-                min_az = run_header_tree['MMcRunHeader_1.fShowerPhiMin'].array(library="np")[0]
-                max_wavelength = run_header_tree['MMcRunHeader_1.fCWaveUpper'].array(library="np")[0]
-                min_wavelength = run_header_tree['MMcRunHeader_1.fCWaveLower'].array(library="np")[0]
+                view_cone = run_header_tree[
+                    "MMcRunHeader.fRandomPointingConeSemiAngle"
+                ].array(library="np")[0]
+                max_impact = run_header_tree["MMcRunHeader.fImpactMax"].array(
+                    library="np"
+                )[0]
+                n_showers = np.sum(
+                    run_header_tree["MMcRunHeader.fNumSimulatedShowers"].array(
+                        library="np"
+                    )
+                )
+                max_zd = run_header_tree["MMcRunHeader.fShowerThetaMax"].array(
+                    library="np"
+                )[0]
+                min_zd = run_header_tree["MMcRunHeader.fShowerThetaMin"].array(
+                    library="np"
+                )[0]
+                max_az = run_header_tree["MMcRunHeader.fShowerPhiMax"].array(
+                    library="np"
+                )[0]
+                min_az = run_header_tree["MMcRunHeader.fShowerPhiMin"].array(
+                    library="np"
+                )[0]
+                max_wavelength = run_header_tree["MMcRunHeader.fCWaveUpper"].array(
+                    library="np"
+                )[0]
+                min_wavelength = run_header_tree["MMcRunHeader.fCWaveLower"].array(
+                    library="np"
+                )[0]
+            elif self.mars_datalevel in [
+                MARSDataLevel.SUPERSTAR,
+                MARSDataLevel.MELIBEA,
+            ]:
+                view_cone = run_header_tree[
+                    "MMcRunHeader_1.fRandomPointingConeSemiAngle"
+                ].array(library="np")[0]
+                max_impact = run_header_tree["MMcRunHeader_1.fImpactMax"].array(
+                    library="np"
+                )[0]
+                n_showers = np.sum(
+                    run_header_tree["MMcRunHeader_1.fNumSimulatedShowers"].array(
+                        library="np"
+                    )
+                )
+                max_zd = run_header_tree["MMcRunHeader_1.fShowerThetaMax"].array(
+                    library="np"
+                )[0]
+                min_zd = run_header_tree["MMcRunHeader_1.fShowerThetaMin"].array(
+                    library="np"
+                )[0]
+                max_az = run_header_tree["MMcRunHeader_1.fShowerPhiMax"].array(
+                    library="np"
+                )[0]
+                min_az = run_header_tree["MMcRunHeader_1.fShowerPhiMin"].array(
+                    library="np"
+                )[0]
+                max_wavelength = run_header_tree["MMcRunHeader_1.fCWaveUpper"].array(
+                    library="np"
+                )[0]
+                min_wavelength = run_header_tree["MMcRunHeader_1.fCWaveLower"].array(
+                    library="np"
+                )[0]
 
             simulation_config[self.run_id] = SimulationConfigContainer(
                 corsika_version=corsika_version,
                 energy_range_min=u.Quantity(e_low, u.GeV).to(u.TeV),
                 energy_range_max=u.Quantity(e_high, u.GeV).to(u.TeV),
                 prod_site_alt=u.Quantity(site_height, u.cm).to(u.m),
                 spectral_index=spectral_index,
@@ -914,78 +1004,72 @@
                 # shower_reuse not written in the magic root file, but since the
                 # sim_events already include shower reuse we artificially set it
                 # to 1 (actually every shower reused 5 times for std MAGIC MC)
                 shower_prog_id=1,
                 prod_site_B_total=MAGIC_Btot,
                 prod_site_B_declination=MAGIC_Bdec,
                 prod_site_B_inclination=MAGIC_Binc,
-                max_alt=u.Quantity((90. - min_zd), u.deg).to(u.rad),
-                min_alt=u.Quantity((90. - max_zd), u.deg).to(u.rad),
+                max_alt=u.Quantity((90.0 - min_zd), u.deg).to(u.rad),
+                min_alt=u.Quantity((90.0 - max_zd), u.deg).to(u.rad),
                 max_az=u.Quantity(max_az, u.deg).to(u.rad),
                 min_az=u.Quantity(min_az, u.deg).to(u.rad),
                 max_viewcone_radius=view_cone * u.deg,
                 min_viewcone_radius=0.0 * u.deg,
                 max_scatter_range=u.Quantity(max_impact, u.cm).to(u.m),
                 min_scatter_range=0.0 * u.m,
                 atmosphere=atm_model,
                 corsika_wlen_min=min_wavelength * u.nm,
                 corsika_wlen_max=max_wavelength * u.nm,
             )
 
         return simulation_config
 
     def prepare_drive_information(self):
-
         drive_leaves = {
-            'mjd': 'MReportDrive.fMjd',
-            'zd': 'MReportDrive.fCurrentZd',
-            'az': 'MReportDrive.fCurrentAz',
-            'ra': 'MReportDrive.fRa',
-            'dec': 'MReportDrive.fDec',
+            "mjd": "MReportDrive.fMjd",
+            "zd": "MReportDrive.fCurrentZd",
+            "az": "MReportDrive.fCurrentAz",
+            "ra": "MReportDrive.fRa",
+            "dec": "MReportDrive.fDec",
         }
 
         # Getting the telescope drive info
         drive_data = {k: [] for k in drive_leaves.keys()}
 
         if self.process_run:
             rootfiles = self.files_
         else:
             rootfiles = [uproot.open(rootf) for rootf in self.file_list_drive]
 
         for rootf in rootfiles:
             drive = rootf["Drive"].arrays(drive_leaves.values(), library="np")
 
-            n_reports = len(drive['MReportDrive.fMjd'])
+            n_reports = len(drive["MReportDrive.fMjd"])
             if n_reports == 0:
-                raise MissingDriveReportError(f"File {rootf.file_path} does not have any drive report. " \
-                                              "Check if it was merpped correctly.")
+                raise MissingDriveReportError(
+                    f"File {rootf.file_path} does not have any drive report. "
+                    "Check if it was merpped correctly."
+                )
             elif n_reports < 3:
-                logger.warning(f"File {rootf.file_path} has only {n_reports} drive reports.")
+                logger.warning(
+                    f"File {rootf.file_path} has only {n_reports} drive reports."
+                )
 
             for key, leaf in drive_leaves.items():
                 drive_data[key].append(drive[leaf])
 
-        drive_data = {
-            k: np.concatenate(v)
-            for k, v in drive_data.items()
-        }
+        drive_data = {k: np.concatenate(v) for k, v in drive_data.items()}
 
         # convert unit as before (Better use astropy units!)
-        drive_data['ra'] *= degrees_per_hour
+        drive_data["ra"] *= degrees_per_hour
 
         # get only drive reports with unique times, otherwise interpolation fails.
-        _, unique_indices = np.unique(
-            drive_data['mjd'],
-            return_index=True
-        )
+        _, unique_indices = np.unique(drive_data["mjd"], return_index=True)
 
-        drive_data = {
-            k: v[unique_indices]
-            for k, v in drive_data.items()
-        }
+        drive_data = {k: v[unique_indices] for k, v in drive_data.items()}
 
         return drive_data
 
     def get_event_time_difference(self):
         """
         Get the trigger time differences of consecutive events.
         The time differences are computed considering all kind of events
@@ -998,22 +1082,21 @@
         time_diffs: astropy.units.quantity.Quantity
             Trigger time differences of consecutive events
         """
 
         time_diffs = np.array([])
 
         for uproot_file in self.files_:
-
-            event_info = uproot_file['Events'].arrays(
-                expressions=['MRawEvtHeader.fTimeDiff'],
-                cut=f'(MTriggerPattern.fPrescaled == {DATA_STEREO_TRIGGER_PATTERN})',
-                library='np',
+            event_info = uproot_file["Events"].arrays(
+                expressions=["MRawEvtHeader.fTimeDiff"],
+                cut=f"(MTriggerPattern.fPrescaled == {DATA_STEREO_TRIGGER_PATTERN})",
+                library="np",
             )
 
-            time_diffs = np.append(time_diffs, event_info['MRawEvtHeader.fTimeDiff'])
+            time_diffs = np.append(time_diffs, event_info["MRawEvtHeader.fTimeDiff"])
 
         time_diffs *= u.s
 
         return time_diffs
 
     @property
     def subarray(self):
@@ -1033,21 +1116,21 @@
 
     @property
     def simulation_config(self):
         return self._simulation_config
 
     @property
     def datalevels(self):
-        return (self.datalevel, )
+        return (self.datalevel,)
 
     @property
     def obs_ids(self):
         # ToCheck: will this be compatible in the future, e.g. with merged MC files
         return list(self.observation_blocks)
-
+        
     def _get_badrmspixel_mask(self, event):
         """
         Fetch bad RMS pixel mask for a given event.
 
         Parameters
         ----------
         event: ctapipe.containers.ArrayEventContainer
@@ -1078,15 +1161,14 @@
             else:
                 index = np.where(pedestal_times < event_time)[0][-1]
 
         badrmspixel_mask = []
         n_ped_types = len(event.mon.tel[tel_id].pedestal.charge_std)
 
         for i_ped_type in range(n_ped_types):
-
             charge_std = event.mon.tel[tel_id].pedestal.charge_std[i_ped_type][index]
 
             pix_step1 = np.logical_and(
                 charge_std > 0,
                 charge_std < 200,
             )
 
@@ -1107,30 +1189,32 @@
 
             if (n_pixels == 0) or (mean_step2 == 0):
                 badrmspixel_mask.append(np.zeros(len(charge_std), np.bool))
                 continue
 
             lolim_step1 = mean_step2 / pedestal_level
             uplim_step1 = mean_step2 * pedestal_level
-            lolim_step2 = mean_step2 - pedestal_level_variance * np.sqrt(var_step2 - mean_step2 ** 2)
-            uplim_step2 = mean_step2 + pedestal_level_variance * np.sqrt(var_step2 - mean_step2 ** 2)
+            lolim_step2 = mean_step2 - pedestal_level_variance * np.sqrt(
+                var_step2 - mean_step2**2
+            )
+            uplim_step2 = mean_step2 + pedestal_level_variance * np.sqrt(
+                var_step2 - mean_step2**2
+            )
 
             badrmspix_step1 = np.logical_or(
                 charge_std < lolim_step1,
                 charge_std > uplim_step1,
             )
 
             badrmspix_step2 = np.logical_or(
                 charge_std < lolim_step2,
                 charge_std > uplim_step2,
             )
 
-            badrmspixel_mask.append(
-                np.logical_or(badrmspix_step1, badrmspix_step2)
-            )
+            badrmspixel_mask.append(np.logical_or(badrmspix_step1, badrmspix_step2))
 
         return badrmspixel_mask
 
     def _set_active_run(self, uproot_file):
         """
         This internal method sets the run
         that will be used for data loading.
@@ -1144,18 +1228,18 @@
         -------
         run: dict
             - input_file: path to the input file
             - data: a MarsCalibratedRun object
         """
 
         run = dict()
-        run['input_file'] = uproot_file.file_path
+        run["input_file"] = uproot_file.file_path
 
         if self.mars_datalevel == MARSDataLevel.CALIBRATED:
-            run['data'] = MarsCalibratedRun(
+            run["data"] = MarsCalibratedRun(
                 uproot_file,
                 self.is_simulation,
                 self.is_stereo,
                 self.use_mc_mono_events,
                 self.is_sumt,
             )
 
@@ -1184,176 +1268,235 @@
         event: ctapipe.containers.ArrayEventContainer
             filled event container
         """
 
         # Data container - is initialized once, and data is replaced after each yield:
         event = ArrayEventContainer()
 
-        event.meta['origin'] = 'MAGIC'
-        event.meta['max_events'] = self.max_events
+        event.meta["origin"] = "MAGIC"
+        event.meta["max_events"] = self.max_events
         event.index.obs_id = self.obs_ids[0]
 
         tel_id = self.telescope
         event.trigger.tels_with_trigger = np.array([tel_id])
 
         counter = 0
 
         # Read the input files subrun-wise:
         for uproot_file in self.files_:
-
-            event.meta['input_file'] = uproot_file.file_path
+            event.meta["input_file"] = uproot_file.file_path
 
             self.current_run = self._set_active_run(uproot_file)
 
             if self.use_pedestals:
-                event_data = self.current_run['data'].pedestal_events
-                n_events = self.current_run['data'].n_pedestal_events
+                event_data = self.current_run["data"].pedestal_events
+                n_events = self.current_run["data"].n_pedestal_events
 
             else:
-                event_data = self.current_run['data'].cosmic_events
-                n_events = self.current_run['data'].n_cosmic_events
+                event_data = self.current_run["data"].cosmic_events
+                n_events = self.current_run["data"].n_cosmic_events
 
-            monitoring_data = self.current_run['data'].monitoring_data
+            monitoring_data = self.current_run["data"].monitoring_data
 
             # Set the pedestal information:
             # hardcoded number of pedestal events averaged over:
             # 500 for pedestal_from_extractor{_rndm}
             # 100 for pedestal_fundamental
             event.mon.tel[tel_id].pedestal.n_events = 500
-            event.mon.tel[tel_id].pedestal.sample_time = monitoring_data['pedestal_sample_time']
+            event.mon.tel[tel_id].pedestal.sample_time = monitoring_data[
+                "pedestal_sample_time"
+            ]
 
             event.mon.tel[tel_id].pedestal.charge_mean = [
-                monitoring_data['pedestal_fundamental']['mean'],
-                monitoring_data['pedestal_from_extractor']['mean'],
-                monitoring_data['pedestal_from_extractor_rndm']['mean'],
+                monitoring_data["pedestal_fundamental"]["mean"],
+                monitoring_data["pedestal_from_extractor"]["mean"],
+                monitoring_data["pedestal_from_extractor_rndm"]["mean"],
             ]
 
             event.mon.tel[tel_id].pedestal.charge_std = [
-                monitoring_data['pedestal_fundamental']['rms'],
-                monitoring_data['pedestal_from_extractor']['rms'],
-                monitoring_data['pedestal_from_extractor_rndm']['rms'],
+                monitoring_data["pedestal_fundamental"]["rms"],
+                monitoring_data["pedestal_from_extractor"]["rms"],
+                monitoring_data["pedestal_from_extractor_rndm"]["rms"],
             ]
 
             # Set the bad pixel information:
             event.mon.tel[tel_id].pixel_status.hardware_failing_pixels = np.reshape(
-                monitoring_data['bad_pixel'], (1, len(monitoring_data['bad_pixel']))
+                monitoring_data["bad_pixel"], (1, len(monitoring_data["bad_pixel"]))
             )
 
             if not self.is_simulation:
                 # Interpolate drive information:
                 drive_data = self.drive_information
-                n_drive_reports = len(drive_data['mjd'])
+                n_drive_reports = len(drive_data["mjd"])
 
                 if self.use_pedestals:
-                    logger.warning(f'Interpolating pedestals events information from {n_drive_reports} drive reports.')
+                    logger.warning(
+                        f"Interpolating pedestals events information from {n_drive_reports} drive reports."
+                    )
                 else:
-                    logger.warning(f'Interpolating cosmic events information from {n_drive_reports} drive reports.')
+                    logger.warning(
+                        f"Interpolating cosmic events information from {n_drive_reports} drive reports."
+                    )
 
-                first_drive_report_time = Time(drive_data['mjd'][0], scale='utc', format='mjd')
-                last_drive_report_time = Time(drive_data['mjd'][-1], scale='utc', format='mjd')
+                first_drive_report_time = Time(
+                    drive_data["mjd"][0], scale="utc", format="mjd"
+                )
+                last_drive_report_time = Time(
+                    drive_data["mjd"][-1], scale="utc", format="mjd"
+                )
 
-                logger.warning(f'Drive reports available from {first_drive_report_time.iso} to {last_drive_report_time.iso}.')
+                logger.warning(
+                    f"Drive reports available from {first_drive_report_time.iso} to {last_drive_report_time.iso}."
+                )
 
                 # Create azimuth and zenith angles interpolators:
                 drive_az_pointing_interpolator = scipy.interpolate.interp1d(
-                    drive_data['mjd'], drive_data['az'], fill_value='extrapolate'
+                    drive_data["mjd"], drive_data["az"], fill_value="extrapolate"
                 )
                 drive_zd_pointing_interpolator = scipy.interpolate.interp1d(
-                    drive_data['mjd'], drive_data['zd'], fill_value='extrapolate'
+                    drive_data["mjd"], drive_data["zd"], fill_value="extrapolate"
                 )
 
                 # Create RA and Dec interpolators:
                 drive_ra_pointing_interpolator = scipy.interpolate.interp1d(
-                    drive_data['mjd'], drive_data['ra'], fill_value='extrapolate'
+                    drive_data["mjd"], drive_data["ra"], fill_value="extrapolate"
                 )
                 drive_dec_pointing_interpolator = scipy.interpolate.interp1d(
-                    drive_data['mjd'], drive_data['dec'], fill_value='extrapolate'
+                    drive_data["mjd"], drive_data["dec"], fill_value="extrapolate"
                 )
 
                 # Interpolate the drive pointing to the event timestamps:
-                event_times = event_data['time'].mjd
+                event_times = event_data["time"].mjd
 
                 pointing_az = drive_az_pointing_interpolator(event_times)
                 pointing_zd = drive_zd_pointing_interpolator(event_times)
                 pointing_ra = drive_ra_pointing_interpolator(event_times)
                 pointing_dec = drive_dec_pointing_interpolator(event_times)
 
-                event_data['pointing_az'] = u.Quantity(pointing_az, u.deg)
-                event_data['pointing_alt'] = u.Quantity(90 - pointing_zd, u.deg)
-                event_data['pointing_ra'] = u.Quantity(pointing_ra, u.deg)
-                event_data['pointing_dec'] = u.Quantity(pointing_dec, u.deg)
+                event_data["pointing_az"] = u.Quantity(pointing_az, u.deg)
+                event_data["pointing_alt"] = u.Quantity(90 - pointing_zd, u.deg)
+                event_data["pointing_ra"] = u.Quantity(pointing_ra, u.deg)
+                event_data["pointing_dec"] = u.Quantity(pointing_dec, u.deg)
 
             # Loop over the events:
             for i_event in range(n_events):
-
                 event.count = counter
-                event.index.event_id = event_data['event_number'][i_event]
+                event.index.event_id = event_data["event_number"][i_event]
 
-                event.trigger.event_type = MAGIC_TO_CTA_EVENT_TYPE.get(event_data['trigger_pattern'][i_event])
+                event.trigger.event_type = MAGIC_TO_CTA_EVENT_TYPE.get(
+                    event_data["trigger_pattern"][i_event]
+                )
 
                 if not self.is_simulation:
-                    event.trigger.time = event_data['time'][i_event]
-                    event.trigger.tel[tel_id].time = event_data['time'][i_event]
+                    event.trigger.time = event_data["time"][i_event]
+                    event.trigger.tel[tel_id].time = event_data["time"][i_event]
 
                 if not self.use_pedestals:
                     badrmspixel_mask = self._get_badrmspixel_mask(event)
-                    event.mon.tel[tel_id].pixel_status.pedestal_failing_pixels = badrmspixel_mask
+                    event.mon.tel[
+                        tel_id
+                    ].pixel_status.pedestal_failing_pixels = badrmspixel_mask
 
                 # Set the telescope pointing container:
-                event.pointing.array_azimuth = event_data['pointing_az'][i_event].to(u.rad)
-                event.pointing.array_altitude = event_data['pointing_alt'][i_event].to(u.rad)
-                event.pointing.array_ra = event_data['pointing_ra'][i_event].to(u.rad)
-                event.pointing.array_dec = event_data['pointing_dec'][i_event].to(u.rad)
+                event.pointing.array_azimuth = event_data["pointing_az"][i_event].to(
+                    u.rad
+                )
+                event.pointing.array_altitude = event_data["pointing_alt"][i_event].to(
+                    u.rad
+                )
+                event.pointing.array_ra = event_data["pointing_ra"][i_event].to(u.rad)
+                event.pointing.array_dec = event_data["pointing_dec"][i_event].to(u.rad)
 
-                event.pointing.tel[tel_id].azimuth = event_data['pointing_az'][i_event].to(u.rad)
-                event.pointing.tel[tel_id].altitude = event_data['pointing_alt'][i_event].to(u.rad)
+                event.pointing.tel[tel_id].azimuth = event_data["pointing_az"][
+                    i_event
+                ].to(u.rad)
+                event.pointing.tel[tel_id].altitude = event_data["pointing_alt"][
+                    i_event
+                ].to(u.rad)
 
                 # Set event charge and peak positions per pixel:
-                event.dl1.tel[tel_id].image = event_data['image'][i_event]
-                event.dl1.tel[tel_id].peak_time = event_data['peak_time'][i_event]
+                event.dl1.tel[tel_id].image = event_data["image"][i_event]
+                event.dl1.tel[tel_id].peak_time = event_data["peak_time"][i_event]
 
                 # Set the simulated event container:
                 if self.is_simulation:
-
                     event.simulation = SimulatedEventContainer()
 
-                    event.simulation.shower.energy = event_data['mc_energy'][i_event].to(u.TeV)
-                    event.simulation.shower.shower_primary_id = 1 - event_data['mc_shower_primary_id'][i_event]
-                    event.simulation.shower.h_first_int = event_data['mc_h_first_int'][i_event].to(u.m)
-                    event.simulation.shower.x_max = event_data['mc_x_max'][i_event].to('g cm-2')
+                    event.simulation.shower.energy = event_data["mc_energy"][
+                        i_event
+                    ].to(u.TeV)
+                    event.simulation.shower.shower_primary_id = (
+                        1 - event_data["mc_shower_primary_id"][i_event]
+                    )
+                    event.simulation.shower.h_first_int = event_data["mc_h_first_int"][
+                        i_event
+                    ].to(u.m)
+                    event.simulation.shower.x_max = event_data["mc_x_max"][i_event].to(
+                        "g cm-2"
+                    )
 
                     # Convert the corsika coordinate (x-axis: magnetic north) to the geographical one.
                     # Rotate the corsika coordinate by the magnetic declination (= 7 deg):
-                    mfield_dec = self.simulation_config[self.obs_ids[0]]['prod_site_B_declination']
-
-                    event.simulation.shower.alt = u.Quantity(90, u.deg) - event_data['mc_theta'][i_event].to(u.deg)
-                    event.simulation.shower.az = u.Quantity(180, u.deg) - event_data['mc_phi'][i_event].to(u.deg) + mfield_dec
+                    mfield_dec = self.simulation_config[self.obs_ids[0]][
+                        "prod_site_B_declination"
+                    ]
+
+                    event.simulation.shower.alt = u.Quantity(90, u.deg) - event_data[
+                        "mc_theta"
+                    ][i_event].to(u.deg)
+                    event.simulation.shower.az = (
+                        u.Quantity(180, u.deg)
+                        - event_data["mc_phi"][i_event].to(u.deg)
+                        + mfield_dec
+                    )
 
                     if event.simulation.shower.az > u.Quantity(180, u.deg):
                         event.simulation.shower.az -= u.Quantity(360, u.deg)
 
-                    event.simulation.shower.core_x = event_data['mc_core_x'][i_event].to(u.m) * np.cos(mfield_dec) \
-                                                     + event_data['mc_core_y'][i_event].to(u.m) * np.sin(mfield_dec)
-
-                    event.simulation.shower.core_y = event_data['mc_core_y'][i_event].to(u.m) * np.cos(mfield_dec) \
-                                                     - event_data['mc_core_x'][i_event].to(u.m) * np.sin(mfield_dec)
+                    event.simulation.shower.core_x = event_data["mc_core_x"][
+                        i_event
+                    ].to(u.m) * np.cos(mfield_dec) + event_data["mc_core_y"][
+                        i_event
+                    ].to(
+                        u.m
+                    ) * np.sin(
+                        mfield_dec
+                    )
+
+                    event.simulation.shower.core_y = event_data["mc_core_y"][
+                        i_event
+                    ].to(u.m) * np.cos(mfield_dec) - event_data["mc_core_x"][
+                        i_event
+                    ].to(
+                        u.m
+                    ) * np.sin(
+                        mfield_dec
+                    )
 
                 yield event
                 counter += 1
 
         return
 
 
 class MarsCalibratedRun:
     """
     This class implements reading of cosmic and pedestal events,
     and monitoring data from a MAGIC calibrated subrun file.
     """
 
-    def __init__(self, uproot_file, is_mc, is_stereo, use_mc_mono_events, use_sumt_events, n_cam_pixels=1039):
+    def __init__(
+        self,
+        uproot_file,
+        is_mc,
+        is_stereo,
+        use_mc_mono_events,
+        use_sumt_events,
+        n_cam_pixels=1039,
+    ):
         """
         Constructor of the class. Loads an input uproot file
         and store the informaiton to constructor variables.
 
         Parameters
         ----------
         uproot_file: uproot.reading.ReadOnlyDirectory
@@ -1372,25 +1515,25 @@
         self.use_mc_mono_events = use_mc_mono_events
         self.use_sumt_events = use_sumt_events
         self.n_cam_pixels = n_cam_pixels
 
         # Load the input data:
         calib_data = self._load_data()
 
-        self.cosmic_events = calib_data['cosmic_events']
-        self.pedestal_events = calib_data['pedestal_events']
-        self.monitoring_data = calib_data['monitoring_data']
+        self.cosmic_events = calib_data["cosmic_events"]
+        self.pedestal_events = calib_data["pedestal_events"]
+        self.monitoring_data = calib_data["monitoring_data"]
 
     @property
     def n_cosmic_events(self):
-        return len(self.cosmic_events.get('trigger_pattern', []))
+        return len(self.cosmic_events.get("trigger_pattern", []))
 
     @property
     def n_pedestal_events(self):
-        return len(self.pedestal_events.get('trigger_pattern', []))
+        return len(self.pedestal_events.get("trigger_pattern", []))
 
     def _load_data(self):
         """
         This method loads cosmic and pedestal events, and monitoring data
         from an input calibrated file and returns them as a dictionary.
 
         Returns
@@ -1398,308 +1541,405 @@
         calib_data: dict
             A dictionary with the event properties,
             cosmic and pedestal events, and monitoring data
         """
 
         # Branches applicable for cosmic and pedestal events:
         common_branches = [
-            'MRawEvtHeader.fStereoEvtNumber',
-            'MRawEvtHeader.fDAQEvtNumber',
-            'MTriggerPattern.fPrescaled',
-            'MCerPhotEvt.fPixels.fPhot',
-            'MArrivalTime.fData',
+            "MRawEvtHeader.fStereoEvtNumber",
+            "MRawEvtHeader.fDAQEvtNumber",
+            "MTriggerPattern.fPrescaled",
+            "MCerPhotEvt.fPixels.fPhot",
+            "MArrivalTime.fData",
         ]
 
         # Branches applicable for MC events:
         mc_branches = [
-            'MMcEvt.fEnergy',
-            'MMcEvt.fTheta',
-            'MMcEvt.fPhi',
-            'MMcEvt.fPartId',
-            'MMcEvt.fZFirstInteraction',
-            'MMcEvt.fLongitmax',
-            'MMcEvt.fCoreX',
-            'MMcEvt.fCoreY',
+            "MMcEvt.fEnergy",
+            "MMcEvt.fTheta",
+            "MMcEvt.fPhi",
+            "MMcEvt.fPartId",
+            "MMcEvt.fZFirstInteraction",
+            "MMcEvt.fLongitmax",
+            "MMcEvt.fCoreX",
+            "MMcEvt.fCoreY",
         ]
 
         pointing_branches = [
-            'MPointingPos.fZd',
-            'MPointingPos.fAz',
-            'MPointingPos.fRa',
-            'MPointingPos.fDec',
-            'MPointingPos.fDevZd',
-            'MPointingPos.fDevAz',
-            'MPointingPos.fDevHa',
-            'MPointingPos.fDevDec',
+            "MPointingPos.fZd",
+            "MPointingPos.fAz",
+            "MPointingPos.fRa",
+            "MPointingPos.fDec",
+            "MPointingPos.fDevZd",
+            "MPointingPos.fDevAz",
+            "MPointingPos.fDevHa",
+            "MPointingPos.fDevDec",
         ]
 
         # Branches applicable for real data:
         timing_branches = [
-            'MTime.fMjd',
-            'MTime.fTime.fMilliSec',
-            'MTime.fNanoSec',
+            "MTime.fMjd",
+            "MTime.fTime.fMilliSec",
+            "MTime.fNanoSec",
         ]
 
         pedestal_time_branches = [
-            'MTimePedestals.fMjd',
-            'MTimePedestals.fTime.fMilliSec',
-            'MTimePedestals.fNanoSec',
+            "MTimePedestals.fMjd",
+            "MTimePedestals.fTime.fMilliSec",
+            "MTimePedestals.fNanoSec",
         ]
 
         pedestal_branches = [
-            'MPedPhotFundamental.fArray.fMean',
-            'MPedPhotFundamental.fArray.fRms',
-            'MPedPhotFromExtractor.fArray.fMean',
-            'MPedPhotFromExtractor.fArray.fRms',
-            'MPedPhotFromExtractorRndm.fArray.fMean',
-            'MPedPhotFromExtractorRndm.fArray.fRms',
+            "MPedPhotFundamental.fArray.fMean",
+            "MPedPhotFundamental.fArray.fRms",
+            "MPedPhotFromExtractor.fArray.fMean",
+            "MPedPhotFromExtractor.fArray.fRms",
+            "MPedPhotFromExtractorRndm.fArray.fMean",
+            "MPedPhotFromExtractorRndm.fArray.fRms",
         ]
 
         # Initialize the data container:
         calib_data = {
-            'cosmic_events': dict(),
-            'pedestal_events': dict(),
-            'monitoring_data': dict(),
+            "cosmic_events": dict(),
+            "pedestal_events": dict(),
+            "monitoring_data": dict(),
         }
 
         # Set event cuts:
         events_cut = dict()
 
         if self.is_mc:
             mc_trigger_pattern = MC_STEREO_AND_MONO_TRIGGER_PATTERN
             if self.use_sumt_events:
                 mc_trigger_pattern = MC_SUMT_TRIGGER_PATTERN
             if self.use_mc_mono_events or not self.is_stereo:
-                events_cut['cosmic_events'] = f'(MTriggerPattern.fPrescaled == {mc_trigger_pattern})'
+                events_cut[
+                    "cosmic_events"
+                ] = f"(MTriggerPattern.fPrescaled == {mc_trigger_pattern})"
             else:
-                events_cut['cosmic_events'] = f'(MTriggerPattern.fPrescaled == {mc_trigger_pattern})' \
-                                                          ' & (MRawEvtHeader.fStereoEvtNumber != 0)'
+                events_cut["cosmic_events"] = (
+                    f"(MTriggerPattern.fPrescaled == {mc_trigger_pattern})"
+                    " & (MRawEvtHeader.fStereoEvtNumber != 0)"
+                )
         else:
             data_trigger_pattern = DATA_STEREO_TRIGGER_PATTERN
             if not self.is_stereo:
                 if self.use_sumt_events:
                     data_trigger_pattern = DATA_MONO_SUMT_TRIGGER_PATTERN
                 else:
                     data_trigger_pattern = DATA_MONO_TRIGGER_PATTERN
-            events_cut['cosmic_events'] = f'(MTriggerPattern.fPrescaled == {data_trigger_pattern})'
+            events_cut[
+                "cosmic_events"
+            ] = f"(MTriggerPattern.fPrescaled == {data_trigger_pattern})"
             # Only for cosmic events because MC data do not have pedestal events:
-            events_cut['pedestal_events'] = f'(MTriggerPattern.fPrescaled == {PEDESTAL_TRIGGER_PATTERN})'
+            events_cut[
+                "pedestal_events"
+            ] = f"(MTriggerPattern.fPrescaled == {PEDESTAL_TRIGGER_PATTERN})"
 
         logger.info(f"Cosmic events selection: {events_cut['cosmic_events']}")
 
         # read common information from RunHeaders
-        sampling_speed = self.uproot_file['RunHeaders']['MRawRunHeader.fSamplingFrequency'].array(library='np')[0]/1000. # GHz
+        sampling_speed = (
+            self.uproot_file["RunHeaders"]["MRawRunHeader.fSamplingFrequency"].array(
+                library="np"
+            )[0]
+            / 1000.0
+        )  # GHz
 
         # Loop over the event types:
         event_types = events_cut.keys()
 
         for event_type in event_types:
-
             # Reading the information common to cosmic and pedestal events:
-            common_info = self.uproot_file['Events'].arrays(
+            common_info = self.uproot_file["Events"].arrays(
                 expressions=common_branches,
                 cut=events_cut[event_type],
-                library='np',
+                library="np",
             )
 
-            if common_info['MTriggerPattern.fPrescaled'].size == 0:
-                raise IndexError(f"No events survived after selection (cut: {events_cut[event_type]})")
+            if common_info["MTriggerPattern.fPrescaled"].size == 0:
+                raise IndexError(
+                    f"No events survived after selection (cut: {events_cut[event_type]})"
+                )
 
-            calib_data[event_type]['trigger_pattern'] = np.array(common_info['MTriggerPattern.fPrescaled'], dtype=int)
+            calib_data[event_type]["trigger_pattern"] = np.array(
+                common_info["MTriggerPattern.fPrescaled"], dtype=int
+            )
 
             # For stereo data, the event ID is simply given by MRawEvtHeader.fStereoEvtNumber
             # For data taken in mono however (i.e. only with one telescope in SA), fStereoEvtNumber
             # is always 0. So one should take fDAQEvtNumber instead. However this DAQ event id is reset
             # for each subrun. Given that each subrun has a maximum number of events which is ~17000
             # (set in the DAQ code), we create an artificial event ID by using the subrun number and
             # attaching the DAQ event id padded with 0 (to have 5 digits for the DAQ event id).
             # Like this we obtain an event id which is unique within a data run (like fStereoEvtNumber).
 
             if (self.is_mc and self.use_mc_mono_events) or not self.is_stereo:
-                subrun_id = self.uproot_file["RunHeaders"]['MRawRunHeader.fSubRunIndex'].array(library="np")[0]
-                calib_data[event_type]['event_number'] = np.array([f"{subrun_id}{daq_id:05}" for daq_id in common_info['MRawEvtHeader.fDAQEvtNumber']], dtype=int)
+                subrun_id = self.uproot_file["RunHeaders"][
+                    "MRawRunHeader.fSubRunIndex"
+                ].array(library="np")[0]
+                calib_data[event_type]["event_number"] = np.array(
+                    [
+                        f"{subrun_id}{daq_id:05}"
+                        for daq_id in common_info["MRawEvtHeader.fDAQEvtNumber"]
+                    ],
+                    dtype=int,
+                )
                 logger.info("Using fDAQEvtNumber to generate event IDs.")
             else:
-                calib_data[event_type]['event_number'] = np.array(common_info['MRawEvtHeader.fStereoEvtNumber'], dtype=int)
+                calib_data[event_type]["event_number"] = np.array(
+                    common_info["MRawEvtHeader.fStereoEvtNumber"], dtype=int
+                )
                 logger.info("Using fStereoEvtNumber to generate event IDs.")
 
             # Set pixel-wise charge and peak time information.
             # The length of the pixel array is 1183, but here only the first part of the pixel
             # information are extracted (i.e., for the current MAGIC camera geometry, the pixels
             # between 0 and 1039 are extracted, since the other part of pixels has only zeros):
-            calib_data[event_type]['image'] = np.array(common_info['MCerPhotEvt.fPixels.fPhot'].tolist())[:, :self.n_cam_pixels]
-            calib_data[event_type]['peak_time'] = np.array(common_info['MArrivalTime.fData'].tolist())[:, :self.n_cam_pixels]
-            calib_data[event_type]['peak_time']/=sampling_speed # [ns]
+            calib_data[event_type]["image"] = np.array(
+                common_info["MCerPhotEvt.fPixels.fPhot"].tolist()
+            )[:, : self.n_cam_pixels]
+            calib_data[event_type]["peak_time"] = np.array(
+                common_info["MArrivalTime.fData"].tolist()
+            )[:, : self.n_cam_pixels]
+            calib_data[event_type]["peak_time"] /= sampling_speed  # [ns]
 
             if self.is_mc:
-
                 # Reading the MC information:
-                mc_info = self.uproot_file['Events'].arrays(
+                mc_info = self.uproot_file["Events"].arrays(
                     expressions=mc_branches,
                     cut=events_cut[event_type],
-                    library='np',
+                    library="np",
                 )
 
                 # Note that the branch "MMcEvt.fPhi" seems to be the angle between the direction
                 # of the magnetic north and the momentum of a simulated primary particle, defined
                 # between -pi and pi, negative if the momentum pointing eastward, positive westward.
                 # The conversion to azimuth should be 180 - fPhi + magnetic_declination:
-                calib_data[event_type]['mc_energy'] = u.Quantity(mc_info['MMcEvt.fEnergy'], u.GeV)
-                calib_data[event_type]['mc_theta'] = u.Quantity(mc_info['MMcEvt.fTheta'], u.rad)
-                calib_data[event_type]['mc_phi'] = u.Quantity(mc_info['MMcEvt.fPhi'], u.rad)
-                calib_data[event_type]['mc_shower_primary_id'] = np.array(mc_info['MMcEvt.fPartId'], dtype=int)
-                calib_data[event_type]['mc_h_first_int'] = u.Quantity(mc_info['MMcEvt.fZFirstInteraction'], u.cm)
-                calib_data[event_type]['mc_x_max'] = u.Quantity(mc_info['MMcEvt.fLongitmax'], u.Unit('g cm-2'))
-                calib_data[event_type]['mc_core_x'] = u.Quantity(mc_info['MMcEvt.fCoreX'], u.cm)
-                calib_data[event_type]['mc_core_y'] = u.Quantity(mc_info['MMcEvt.fCoreY'], u.cm)
+                calib_data[event_type]["mc_energy"] = u.Quantity(
+                    mc_info["MMcEvt.fEnergy"], u.GeV
+                )
+                calib_data[event_type]["mc_theta"] = u.Quantity(
+                    mc_info["MMcEvt.fTheta"], u.rad
+                )
+                calib_data[event_type]["mc_phi"] = u.Quantity(
+                    mc_info["MMcEvt.fPhi"], u.rad
+                )
+                calib_data[event_type]["mc_shower_primary_id"] = np.array(
+                    mc_info["MMcEvt.fPartId"], dtype=int
+                )
+                calib_data[event_type]["mc_h_first_int"] = u.Quantity(
+                    mc_info["MMcEvt.fZFirstInteraction"], u.cm
+                )
+                calib_data[event_type]["mc_x_max"] = u.Quantity(
+                    mc_info["MMcEvt.fLongitmax"], u.Unit("g cm-2")
+                )
+                calib_data[event_type]["mc_core_x"] = u.Quantity(
+                    mc_info["MMcEvt.fCoreX"], u.cm
+                )
+                calib_data[event_type]["mc_core_y"] = u.Quantity(
+                    mc_info["MMcEvt.fCoreY"], u.cm
+                )
 
                 # Reading the telescope pointing information:
-                pointing = self.uproot_file['Events'].arrays(
+                pointing = self.uproot_file["Events"].arrays(
                     expressions=pointing_branches,
                     cut=events_cut[event_type],
-                    library='np',
+                    library="np",
                 )
 
-                pointing_az = pointing['MPointingPos.fAz'] - pointing['MPointingPos.fDevAz']
-                pointing_zd = pointing['MPointingPos.fZd'] - pointing['MPointingPos.fDevZd']
+                pointing_az = (
+                    pointing["MPointingPos.fAz"] - pointing["MPointingPos.fDevAz"]
+                )
+                pointing_zd = (
+                    pointing["MPointingPos.fZd"] - pointing["MPointingPos.fDevZd"]
+                )
 
                 # N.B. the positive sign here, as HA = local sidereal time - ra:
-                pointing_ra = (pointing['MPointingPos.fRa'] + pointing['MPointingPos.fDevHa']) * degrees_per_hour
-                pointing_dec = pointing['MPointingPos.fDec'] - pointing['MPointingPos.fDevDec']
+                pointing_ra = (
+                    pointing["MPointingPos.fRa"] + pointing["MPointingPos.fDevHa"]
+                ) * degrees_per_hour
+                pointing_dec = (
+                    pointing["MPointingPos.fDec"] - pointing["MPointingPos.fDevDec"]
+                )
 
-                calib_data[event_type]['pointing_az'] = u.Quantity(pointing_az, u.deg)
-                calib_data[event_type]['pointing_alt'] = u.Quantity(90 - pointing_zd, u.deg)
-                calib_data[event_type]['pointing_ra'] = u.Quantity(pointing_ra, u.deg)
-                calib_data[event_type]['pointing_dec'] = u.Quantity(pointing_dec, u.deg)
+                calib_data[event_type]["pointing_az"] = u.Quantity(pointing_az, u.deg)
+                calib_data[event_type]["pointing_alt"] = u.Quantity(
+                    90 - pointing_zd, u.deg
+                )
+                calib_data[event_type]["pointing_ra"] = u.Quantity(pointing_ra, u.deg)
+                calib_data[event_type]["pointing_dec"] = u.Quantity(pointing_dec, u.deg)
 
             else:
                 # Reading the event timing information:
-                timing_info = self.uproot_file['Events'].arrays(
+                timing_info = self.uproot_file["Events"].arrays(
                     expressions=timing_branches,
                     cut=events_cut[event_type],
-                    library='np',
+                    library="np",
                 )
 
                 # In order to keep the precision of timestamps, here the Decimal module is used.
                 # At the later steps, the precise information can be extracted by specifying
                 # the sub-format of value to 'long', i.e., Time.to_value(format='unix', subfmt='long'):
-                event_obs_day = Time(timing_info['MTime.fMjd'], format='mjd', scale='utc')
+                event_obs_day = Time(
+                    timing_info["MTime.fMjd"], format="mjd", scale="utc"
+                )
                 event_obs_day = np.round(event_obs_day.unix)
                 event_obs_day = np.array([Decimal(str(x)) for x in event_obs_day])
 
-                event_millisec = np.round(timing_info['MTime.fTime.fMilliSec'] * msec2sec, 3)
+                event_millisec = np.round(
+                    timing_info["MTime.fTime.fMilliSec"] * msec2sec, 3
+                )
                 event_millisec = np.array([Decimal(str(x)) for x in event_millisec])
 
-                event_nanosec = np.round(timing_info['MTime.fNanoSec'] * nsec2sec, 7)
+                event_nanosec = np.round(timing_info["MTime.fNanoSec"] * nsec2sec, 7)
                 event_nanosec = np.array([Decimal(str(x)) for x in event_nanosec])
 
                 event_time = event_obs_day + event_millisec + event_nanosec
-                calib_data[event_type]['time'] = Time(event_time, format='unix', scale='utc')
+                calib_data[event_type]["time"] = Time(
+                    event_time, format="unix", scale="utc"
+                )
 
         # Reading the monitoring data, both for real data and MC
         # In MAGIC simulations, pixel 0 is always set as bad
 
         # Reading the bad pixel information:
-        as_dtype = uproot.interpretation.numerical.AsDtype(np.dtype('>i4'))
+        as_dtype = uproot.interpretation.numerical.AsDtype(np.dtype(">i4"))
         as_jagged = uproot.interpretation.jagged.AsJagged(as_dtype)
 
-        badpixel_info = self.uproot_file['RunHeaders']['MBadPixelsCam.fArray.fInfo'].array(as_jagged, library='np')[0]
-        badpixel_info = badpixel_info.reshape((4, 1183), order='F')
+        badpixel_info = self.uproot_file["RunHeaders"][
+            "MBadPixelsCam.fArray.fInfo"
+        ].array(as_jagged, library="np")[0]
+        badpixel_info = badpixel_info.reshape((4, 1183), order="F")
 
         # now we have 4 axes:
         # 0st axis: empty (?)
         # 1st axis: Unsuitable pixels
         # 2nd axis: Uncalibrated pixels (says why pixel is unsuitable)
         # 3rd axis: Bad hardware pixels (says why pixel is unsuitable)
         # Each axis cointains a 32bit integer encoding more information about the specific problem
         # See MARS software, MBADPixelsPix.h for more information
         # Here we take the first axis:
         unsuitable_pixels_bit = badpixel_info[1]
         unsuitable_pixels = np.zeros(self.n_cam_pixels, dtype=bool)
 
         for i_pix in range(self.n_cam_pixels):
-            unsuitable_pixels[i_pix] = int('{:08b}'.format(unsuitable_pixels_bit[i_pix])[-2])
+            unsuitable_pixels[i_pix] = int(
+                "{:08b}".format(unsuitable_pixels_bit[i_pix])[-2]
+            )
 
-        calib_data['monitoring_data']['bad_pixel'] = unsuitable_pixels
+        calib_data["monitoring_data"]["bad_pixel"] = unsuitable_pixels
 
         # Try to read the Pedestals tree (soft fail if not present):
         try:
             if self.is_mc:
                 pedestal_branch_list = pedestal_branches
-                pedestal_info = self.uproot_file['Events'].arrays(
+                pedestal_info = self.uproot_file["Events"].arrays(
                     expressions=pedestal_branch_list,
-                    library='np',
+                    library="np",
                 )
             else:
                 pedestal_branch_list = pedestal_time_branches + pedestal_branches
 
-                pedestal_info = self.uproot_file['Pedestals'].arrays(
+                pedestal_info = self.uproot_file["Pedestals"].arrays(
                     expressions=pedestal_branch_list,
-                    library='np',
+                    library="np",
                 )
 
             # Set sample times of pedestal events:
             if self.is_mc:
-                calib_data['monitoring_data']['pedestal_sample_time'] = np.array([])
+                calib_data["monitoring_data"]["pedestal_sample_time"] = np.array([])
             else:
-                pedestal_obs_day = Time(pedestal_info['MTimePedestals.fMjd'], format='mjd', scale='utc')
+                pedestal_obs_day = Time(
+                    pedestal_info["MTimePedestals.fMjd"], format="mjd", scale="utc"
+                )
                 pedestal_obs_day = np.round(pedestal_obs_day.unix)
                 pedestal_obs_day = np.array([Decimal(str(x)) for x in pedestal_obs_day])
 
-                pedestal_millisec = np.round(pedestal_info['MTimePedestals.fTime.fMilliSec'] * msec2sec, 3)
-                pedestal_millisec = np.array([Decimal(str(x)) for x in pedestal_millisec])
+                pedestal_millisec = np.round(
+                    pedestal_info["MTimePedestals.fTime.fMilliSec"] * msec2sec, 3
+                )
+                pedestal_millisec = np.array(
+                    [Decimal(str(x)) for x in pedestal_millisec]
+                )
 
-                pedestal_nanosec = np.round(pedestal_info['MTimePedestals.fNanoSec'] * nsec2sec, 7)
+                pedestal_nanosec = np.round(
+                    pedestal_info["MTimePedestals.fNanoSec"] * nsec2sec, 7
+                )
                 pedestal_nanosec = np.array([Decimal(str(x)) for x in pedestal_nanosec])
 
-                pedestal_sample_time = pedestal_obs_day + pedestal_millisec + pedestal_nanosec
+                pedestal_sample_time = (
+                    pedestal_obs_day + pedestal_millisec + pedestal_nanosec
+                )
 
-                calib_data['monitoring_data']['pedestal_sample_time'] = Time(
-                    pedestal_sample_time, format='unix', scale='utc'
+                calib_data["monitoring_data"]["pedestal_sample_time"] = Time(
+                    pedestal_sample_time, format="unix", scale="utc"
                 )
 
             # Set the mean and RMS of pedestal charges:
-            calib_data['monitoring_data']['pedestal_fundamental'] = {
-                'mean': np.array(pedestal_info[f'MPedPhotFundamental.fArray.fMean'].tolist())[:, :self.n_cam_pixels],
-                'rms': np.array(pedestal_info[f'MPedPhotFundamental.fArray.fRms'].tolist())[:, :self.n_cam_pixels],
+            calib_data["monitoring_data"]["pedestal_fundamental"] = {
+                "mean": np.array(
+                    pedestal_info["MPedPhotFundamental.fArray.fMean"].tolist()
+                )[:, : self.n_cam_pixels],
+                "rms": np.array(
+                    pedestal_info["MPedPhotFundamental.fArray.fRms"].tolist()
+                )[:, : self.n_cam_pixels],
             }
-            calib_data['monitoring_data']['pedestal_from_extractor'] = {
-                'mean': np.array(pedestal_info[f'MPedPhotFromExtractor.fArray.fMean'].tolist())[:, :self.n_cam_pixels],
-                'rms': np.array(pedestal_info[f'MPedPhotFromExtractor.fArray.fRms'].tolist())[:, :self.n_cam_pixels],
+            calib_data["monitoring_data"]["pedestal_from_extractor"] = {
+                "mean": np.array(
+                    pedestal_info["MPedPhotFromExtractor.fArray.fMean"].tolist()
+                )[:, : self.n_cam_pixels],
+                "rms": np.array(
+                    pedestal_info["MPedPhotFromExtractor.fArray.fRms"].tolist()
+                )[:, : self.n_cam_pixels],
             }
-            calib_data['monitoring_data']['pedestal_from_extractor_rndm'] = {
-                'mean': np.array(pedestal_info[f'MPedPhotFromExtractorRndm.fArray.fMean'].tolist())[:, :self.n_cam_pixels],
-                'rms': np.array(pedestal_info[f'MPedPhotFromExtractorRndm.fArray.fRms'].tolist())[:, :self.n_cam_pixels],
+            calib_data["monitoring_data"]["pedestal_from_extractor_rndm"] = {
+                "mean": np.array(
+                    pedestal_info["MPedPhotFromExtractorRndm.fArray.fMean"].tolist()
+                )[:, : self.n_cam_pixels],
+                "rms": np.array(
+                    pedestal_info["MPedPhotFromExtractorRndm.fArray.fRms"].tolist()
+                )[:, : self.n_cam_pixels],
             }
 
         except KeyError:
-            logger.warning('The Pedestals tree is not present in the input file. Cleaning algorithm may fail.')
+            logger.warning(
+                "The Pedestals tree is not present in the input file. Cleaning algorithm may fail."
+            )
 
         if not self.is_mc:
             if self.is_stereo:
                 # Check for bit flips in the stereo event IDs:
                 uplim_total_jumps = 100
 
-                stereo_event_number = calib_data['cosmic_events']['event_number'].astype(int)
+                stereo_event_number = calib_data["cosmic_events"][
+                    "event_number"
+                ].astype(int)
                 number_difference = np.diff(stereo_event_number)
 
                 indices_flip = np.where(number_difference < 0)[0]
                 n_flips = len(indices_flip)
 
                 if n_flips > 0:
-
-                    logger.warning(f'Warning: detected {n_flips} bit flips in the input file')
+                    logger.warning(
+                        f"Warning: detected {n_flips} bit flips in the input file"
+                    )
                     total_jumped_number = 0
 
                     for i in indices_flip:
-
-                        jumped_number = stereo_event_number[i] - stereo_event_number[i+1]
+                        jumped_number = (
+                            stereo_event_number[i] - stereo_event_number[i + 1]
+                        )
                         total_jumped_number += jumped_number
 
-                        logger.warning(f'Jump of L3 number backward from {stereo_event_number[i]} to ' \
-                                       f'{stereo_event_number[i+1]}; total jumped number so far: {total_jumped_number}')
+                        logger.warning(
+                            f"Jump of L3 number backward from {stereo_event_number[i]} to "
+                            f"{stereo_event_number[i+1]}; total jumped number so far: {total_jumped_number}"
+                        )
 
                     if total_jumped_number > uplim_total_jumps:
-                        logger.warning(f'More than {uplim_total_jumps} jumps in the stereo trigger number; ' \
-                                       f'You may have to match events by timestamp at a later stage.')
+                        logger.warning(
+                            f"More than {uplim_total_jumps} jumps in the stereo trigger number; "
+                            f"You may have to match events by timestamp at a later stage."
+                        )
 
         return calib_data
```

### Comparing `ctapipe_io_magic-0.5.0/ctapipe_io_magic/mars_datalevels.py` & `ctapipe_io_magic-0.5.1/ctapipe_io_magic/mars_datalevels.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.0/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz` & `ctapipe_io_magic-0.5.1/ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.0/ctapipe_io_magic/tests/test_stage1.py` & `ctapipe_io_magic-0.5.1/ctapipe_io_magic/tests/test_stage1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,82 @@
 from pathlib import Path
 import os
 
 from ctapipe.io import read_table
 from ctapipe.containers import EventType
 import numpy as np
 
-test_data = Path(os.getenv('MAGIC_TEST_DATA', 'test_data')).absolute()
-test_cal_path = test_data / 'real/calibrated/20210314_M1_05095172.001_Y_CrabNebula-W0.40+035.root'
+test_data = Path(os.getenv("MAGIC_TEST_DATA", "test_data")).absolute()
+test_cal_path = (
+    test_data / "real/calibrated/20210314_M1_05095172.001_Y_CrabNebula-W0.40+035.root"
+)
 config = Path(".").absolute() / "example_stage1_config.json"
 
 
 def test_stage1_multiple_runs():
     """Test the ctapipe process tool can read in MAGIC real data using the event source"""
     from ctapipe.tools.process import ProcessorTool
     from ctapipe.core import run_tool
 
     tool = ProcessorTool()
-    output = test_data / 'real/calibrated/20210314_M1_05095172_Y_CrabNebula-W0.40+035.h5'
-
-    ret = run_tool(tool, argv=[
-        f'--input={test_cal_path}',
-        f'--output={output}',
-        f'--config={str(config)}',
-        "--camera-frame",
-    ])
+    output = (
+        test_data / "real/calibrated/20210314_M1_05095172_Y_CrabNebula-W0.40+035.h5"
+    )
+
+    ret = run_tool(
+        tool,
+        argv=[
+            f"--input={test_cal_path}",
+            f"--output={output}",
+            f"--config={str(config)}",
+            "--camera-frame",
+        ],
+    )
     assert ret == 0
 
-    parameters = read_table(output, '/dl1/event/telescope/parameters/tel_001')
+    parameters = read_table(output, "/dl1/event/telescope/parameters/tel_001")
     assert len(parameters) == 910
 
-    trigger = read_table(output, '/dl1/event/subarray/trigger')
+    trigger = read_table(output, "/dl1/event/subarray/trigger")
 
-    event_type_counts = np.bincount(trigger['event_type'])
+    event_type_counts = np.bincount(trigger["event_type"])
 
     # no pedestals expected, should be only physics data
     assert event_type_counts.sum() == 910
     assert event_type_counts[EventType.FLATFIELD.value] == 0
     assert event_type_counts[EventType.SKY_PEDESTAL.value] == 0
     assert event_type_counts[EventType.SUBARRAY.value] == 910
 
 
 def test_stage1_single_run():
     """Test the ctapipe process tool can read in MAGIC real data using the event source"""
     from ctapipe.tools.process import ProcessorTool
     from ctapipe.core import run_tool
 
     tool = ProcessorTool()
-    output = test_cal_path.with_suffix('.h5')
+    output = test_cal_path.with_suffix(".h5")
 
-    ret = run_tool(tool, argv=[
-        f'--input={test_cal_path}',
-        f'--output={output}',
-        f'--config={str(config)}',
-        "--MAGICEventSource.process_run=false",
-        "--allowed-tels=1",
-        "--camera-frame",
-    ])
+    ret = run_tool(
+        tool,
+        argv=[
+            f"--input={test_cal_path}",
+            f"--output={output}",
+            f"--config={str(config)}",
+            "--MAGICEventSource.process_run=false",
+            "--allowed-tels=1",
+            "--camera-frame",
+        ],
+    )
     assert ret == 0
 
-    parameters = read_table(output, '/dl1/event/telescope/parameters/tel_001')
+    parameters = read_table(output, "/dl1/event/telescope/parameters/tel_001")
     assert len(parameters) == 458
 
-    trigger = read_table(output, '/dl1/event/subarray/trigger')
+    trigger = read_table(output, "/dl1/event/subarray/trigger")
 
-    event_type_counts = np.bincount(trigger['event_type'])
+    event_type_counts = np.bincount(trigger["event_type"])
 
     # no pedestals expected, should be only physics data
     assert event_type_counts.sum() == 458
     assert event_type_counts[EventType.FLATFIELD.value] == 0
     assert event_type_counts[EventType.SKY_PEDESTAL.value] == 0
     assert event_type_counts[EventType.SUBARRAY.value] == 458
```

### Comparing `ctapipe_io_magic-0.5.0/ctapipe_io_magic/version.py` & `ctapipe_io_magic-0.5.1/ctapipe_io_magic/version.py`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/PKG-INFO` & `ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ctapipe-io-magic
-Version: 0.5.0
+Version: 0.5.1
 Summary: ctapipe plugin for reading calibrated MAGIC files
 Home-page: https://github.com/cta-observatory/ctapipe_io_magic
 Author: Ievgen Vovk et al.
 Author-email: Ievgen.Vovk@mpp.mpg.de
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 ## *ctapipe* MAGIC event source
 
-EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.17.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
+EventSource plugin for *ctapipe*, needed to read the calibrated data of the MAGIC telescope system. It requires the [*ctapipe*](https://github.com/cta-observatory/ctapipe) (v0.19.0) and [*uproot*](https://github.com/scikit-hep/uproot4) (>=5) packages to run.
 
 #### Installation
 
 If *ctapipe* is already installed, the installation can be done via *pip* (the module is available in PyPI):
 
 ```bash
 pip install ctapipe_io_magic
@@ -121,8 +121,10 @@
 -   v0.4.1: added CI, refactoring of code, added tests, extract drive information once
 -   v0.4.2: added more tests, refactored code, allow the processing of all subruns from the same run at the same time (including drive information), correct de-rotation of quantities from the CORSIKA frame to the geographical frame, computation of bad pixels, modification of focal length to take into account the coma aberration, fix dowload of test data set
 -   v0.4.3: difference of arrival times between events read from ROOT files, used for effective observation time calculation
 -   v0.4.4: changed units of peak_time from time slices (as stored in MARS) to nanoseconds
 -   v0.4.5: fixed automatic tests, add possibility to choose between effective and nominal focal length
 -   v0.4.6: add support to read in data taken in mono mode (full for real data, partial for MCs). Fixed bug in recognition of mono/stereo or standard trigger/SumT data (added also for MC)
 -   v0.4.7: add full support to read in real and MC data taken in mono mode, and with SumT. Added treatment of unsuitable pixels for MC data. Added readout of true XMax value from MC data (usually not available, filled with 0 otherwise)
--   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the correct value used in MAGIC simulations (i.e. 16.97 meters)
+-   v0.5.0: release compatible with ctapipe 0.17. Also, the equivalent focal length is set to the
+    correct value used in MAGIC simulations (i.e. 16.97 meters)
+-   v0.5.1: release compatible with ctapipe 0.19
```

### Comparing `ctapipe_io_magic-0.5.0/ctapipe_io_magic.egg-info/SOURCES.txt` & `ctapipe_io_magic-0.5.1/ctapipe_io_magic.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ctapipe_io_magic/_version.py
 ctapipe_io_magic/constants.py
 ctapipe_io_magic/mars_datalevels.py
 ctapipe_io_magic/version.py
 ctapipe_io_magic.egg-info/PKG-INFO
 ctapipe_io_magic.egg-info/SOURCES.txt
 ctapipe_io_magic.egg-info/dependency_links.txt
+ctapipe_io_magic.egg-info/entry_points.txt
 ctapipe_io_magic.egg-info/requires.txt
 ctapipe_io_magic.egg-info/top_level.txt
 ctapipe_io_magic/resources/MAGICCam.camgeom.fits.gz
 ctapipe_io_magic/tests/test_magic_event_source.py
 ctapipe_io_magic/tests/test_mars_datalevels.py
 ctapipe_io_magic/tests/test_stage1.py
 ctapipe_io_magic/tests/test_version.py
```

### Comparing `ctapipe_io_magic-0.5.0/download_test_data.sh` & `ctapipe_io_magic-0.5.1/download_test_data.sh`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.0/example_stage1_config.json` & `ctapipe_io_magic-0.5.1/example_stage1_config.json`

 * *Files identical despite different names*

### Comparing `ctapipe_io_magic-0.5.0/setup.py` & `ctapipe_io_magic-0.5.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 
 docs_require = [
     "sphinx~=4.2",
     "sphinx-automodapi",
     "sphinx_argparse",
     "sphinx_rtd_theme",
     "numpydoc",
-    "nbsphinx"
+    "nbsphinx",
 ]
 
 setup(
     use_scm_version={"write_to": os.path.join("ctapipe_io_magic", "_version.py")},
     packages=find_packages(),
     install_requires=[
-        'ctapipe~=0.17',
-        'astropy~=5.0',
-        'uproot~=5.0',
-        'numpy>=1.20',
+        "ctapipe~=0.19",
+        "astropy~=5.0",
+        "uproot~=5.0",
+        "numpy>=1.20",
     ],
     package_data={
-        'ctapipe_io_magic': ['resources/*'],
+        "ctapipe_io_magic": ["resources/*"],
     },
     extras_require={
         "all": tests_require + docs_require,
         "tests": tests_require,
         "docs": docs_require,
     },
-    setup_requires=['pytest_runner'],
+    setup_requires=["pytest_runner"],
+    entry_points={'ctapipe_io':['MAGICEventSource = ctapipe_io_magic:MAGICEventSource ']}   
 )
+
```

