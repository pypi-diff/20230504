# Comparing `tmp/pyote-5.2.2.tar.gz` & `tmp/pyote-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyote-5.2.2.tar", last modified: Sat Apr 15 01:44:34 2023, max compression
+gzip compressed data, was "pyote-5.2.3.tar", last modified: Wed May  3 02:51:35 2023, max compression
```

## Comparing `pyote-5.2.2.tar` & `pyote-5.2.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 01:44:34.848413 pyote-5.2.2/
--rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.2.2/LICENSE
--rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1190 2023-04-15 01:44:34.848413 pyote-5.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.2.2/README.rst
--rw-rw-rw-   0        0        0       80 2023-04-15 01:44:34.849412 pyote-5.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2912 2023-02-11 21:30:43.000000 pyote-5.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 01:44:34.677877 pyote-5.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 01:44:34.687874 pyote-5.2.2/src/pyote.egg-info/
--rw-rw-rw-   0        0        0     1190 2023-04-15 01:44:34.000000 pyote-5.2.2/src/pyote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1690 2023-04-15 01:44:34.000000 pyote-5.2.2/src/pyote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 01:44:34.000000 pyote-5.2.2/src/pyote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.2.2/src/pyote.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      250 2023-04-15 01:44:34.000000 pyote-5.2.2/src/pyote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 01:44:34.000000 pyote-5.2.2/src/pyote.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 01:44:34.823404 pyote-5.2.2/src/pyoteapp/
--rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.2.2/src/pyoteapp/PYOTE.bat
--rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.2.2/src/pyoteapp/SER.py
--rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.2.2/src/pyoteapp/__init__.py
--rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.2.2/src/pyoteapp/autocorrtools.py
--rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.2.2/src/pyoteapp/blockIntegrateUtils.py
--rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.2.2/src/pyoteapp/checkForNewerVersion.py
--rw-rw-rw-   0        0        0    11897 2023-03-07 02:00:12.000000 pyote-5.2.2/src/pyoteapp/csvreader.py
--rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.2.2/src/pyoteapp/diffraction-table.p
--rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.2.2/src/pyoteapp/errorBarUtils.py
--rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.2.2/src/pyoteapp/example-penumbral.csv
--rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.2.2/src/pyoteapp/exponentialEdgeUtilities.py
--rw-rw-rw-   0        0        0     6829 2022-02-04 15:30:43.000000 pyote-5.2.2/src/pyoteapp/false_positive.py
--rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.2.2/src/pyoteapp/fixedPrecision.py
--rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.2.2/src/pyoteapp/genDiffraction.py
--rw-rw-rw-   0        0        0   371192 2023-04-12 22:16:10.000000 pyote-5.2.2/src/pyoteapp/gui.py
--rw-rw-rw-   0        0        0     2157 2022-07-18 16:06:30.000000 pyote-5.2.2/src/pyoteapp/helpDialog.py
--rw-rw-rw-   0        0        0    25777 2023-01-14 20:02:18.000000 pyote-5.2.2/src/pyoteapp/iterative_logl_functions.py
--rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.2.2/src/pyoteapp/likelihood_calculations.py
-drwxrwxrwx   0        0        0        0 2023-04-15 01:44:34.847419 pyote-5.2.2/src/pyoteapp/model-examples/
--rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.2.2/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.2.2/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.2.2/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.2.2/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
--rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.2.2/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.2.2/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.2.2/src/pyoteapp/model-help.pdf
--rw-rw-rw-   0        0        0     1456 2020-02-12 15:11:07.000000 pyote-5.2.2/src/pyoteapp/noiseUtils.py
--rw-rw-rw-   0        0        0   440959 2023-04-12 20:41:22.000000 pyote-5.2.2/src/pyoteapp/pyote-info.pdf
--rw-rw-rw-   0        0        0   429807 2023-04-12 22:09:16.000000 pyote-5.2.2/src/pyoteapp/pyote.py
--rw-rw-rw-   0        0        0    79632 2023-04-12 17:10:43.000000 pyote-5.2.2/src/pyoteapp/pyote_modelling_utility_functions.py
--rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.2.2/src/pyoteapp/run-pyote-mac.bat
--rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.2.2/src/pyoteapp/showVideoFrames.py
--rw-rw-rw-   0        0        0    24479 2022-07-16 15:57:50.000000 pyote-5.2.2/src/pyoteapp/solverUtils.py
--rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.2.2/src/pyoteapp/subframe_timing_utilities.py
--rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.2.2/src/pyoteapp/timestampDialog.py
--rw-rw-rw-   0        0        0    14839 2023-03-17 22:02:18.000000 pyote-5.2.2/src/pyoteapp/timestampUtils.py
--rw-rw-rw-   0        0        0       34 2023-04-15 01:42:41.000000 pyote-5.2.2/src/pyoteapp/version.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.614187 pyote-5.2.3/
+-rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.2.3/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1190 2023-05-03 02:51:35.614187 pyote-5.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.2.3/README.rst
+-rw-rw-rw-   0        0        0       80 2023-05-03 02:51:35.618196 pyote-5.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2912 2023-02-11 21:30:43.000000 pyote-5.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.518649 pyote-5.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.524634 pyote-5.2.3/src/pyote.egg-info/
+-rw-rw-rw-   0        0        0     1190 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1690 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.2.3/src/pyote.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      250 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 02:51:35.000000 pyote-5.2.3/src/pyote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.610199 pyote-5.2.3/src/pyoteapp/
+-rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.2.3/src/pyoteapp/PYOTE.bat
+-rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.2.3/src/pyoteapp/SER.py
+-rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.2.3/src/pyoteapp/__init__.py
+-rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.2.3/src/pyoteapp/autocorrtools.py
+-rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.2.3/src/pyoteapp/blockIntegrateUtils.py
+-rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.2.3/src/pyoteapp/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0    11897 2023-03-07 02:00:12.000000 pyote-5.2.3/src/pyoteapp/csvreader.py
+-rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.2.3/src/pyoteapp/diffraction-table.p
+-rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.2.3/src/pyoteapp/errorBarUtils.py
+-rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.2.3/src/pyoteapp/example-penumbral.csv
+-rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.2.3/src/pyoteapp/exponentialEdgeUtilities.py
+-rw-rw-rw-   0        0        0     6829 2022-02-04 15:30:43.000000 pyote-5.2.3/src/pyoteapp/false_positive.py
+-rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.2.3/src/pyoteapp/fixedPrecision.py
+-rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.2.3/src/pyoteapp/genDiffraction.py
+-rw-rw-rw-   0        0        0   371192 2023-04-12 22:16:10.000000 pyote-5.2.3/src/pyoteapp/gui.py
+-rw-rw-rw-   0        0        0     2157 2022-07-18 16:06:30.000000 pyote-5.2.3/src/pyoteapp/helpDialog.py
+-rw-rw-rw-   0        0        0    25547 2023-05-03 02:37:23.000000 pyote-5.2.3/src/pyoteapp/iterative_logl_functions.py
+-rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.2.3/src/pyoteapp/likelihood_calculations.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:51:35.613187 pyote-5.2.3/src/pyoteapp/model-examples/
+-rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.2.3/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.2.3/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.2.3/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.2.3/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
+-rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.2.3/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.2.3/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.2.3/src/pyoteapp/model-help.pdf
+-rw-rw-rw-   0        0        0     1646 2023-05-03 00:27:00.000000 pyote-5.2.3/src/pyoteapp/noiseUtils.py
+-rw-rw-rw-   0        0        0   441632 2023-05-03 02:49:09.000000 pyote-5.2.3/src/pyoteapp/pyote-info.pdf
+-rw-rw-rw-   0        0        0   428283 2023-05-03 00:27:00.000000 pyote-5.2.3/src/pyoteapp/pyote.py
+-rw-rw-rw-   0        0        0    79660 2023-05-03 00:27:00.000000 pyote-5.2.3/src/pyoteapp/pyote_modelling_utility_functions.py
+-rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.2.3/src/pyoteapp/run-pyote-mac.bat
+-rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.2.3/src/pyoteapp/showVideoFrames.py
+-rw-rw-rw-   0        0        0    23481 2023-05-03 00:27:00.000000 pyote-5.2.3/src/pyoteapp/solverUtils.py
+-rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.2.3/src/pyoteapp/subframe_timing_utilities.py
+-rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.2.3/src/pyoteapp/timestampDialog.py
+-rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.2.3/src/pyoteapp/timestampUtils.py
+-rw-rw-rw-   0        0        0       34 2023-04-20 22:40:23.000000 pyote-5.2.3/src/pyoteapp/version.py
```

### Comparing `pyote-5.2.2/LICENSE` & `pyote-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/PKG-INFO` & `pyote-5.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.2.2
+Version: 5.2.3
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.2.2/setup.py` & `pyote-5.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyote.egg-info/PKG-INFO` & `pyote-5.2.3/src/pyote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.2.2
+Version: 5.2.3
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.2.2/src/pyote.egg-info/SOURCES.txt` & `pyote-5.2.3/src/pyote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/SER.py` & `pyote-5.2.3/src/pyoteapp/SER.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/autocorrtools.py` & `pyote-5.2.3/src/pyoteapp/autocorrtools.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/blockIntegrateUtils.py` & `pyote-5.2.3/src/pyoteapp/blockIntegrateUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/checkForNewerVersion.py` & `pyote-5.2.3/src/pyoteapp/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/csvreader.py` & `pyote-5.2.3/src/pyoteapp/csvreader.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/diffraction-table.p` & `pyote-5.2.3/src/pyoteapp/diffraction-table.p`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/errorBarUtils.py` & `pyote-5.2.3/src/pyoteapp/errorBarUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/example-penumbral.csv` & `pyote-5.2.3/src/pyoteapp/example-penumbral.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/exponentialEdgeUtilities.py` & `pyote-5.2.3/src/pyoteapp/exponentialEdgeUtilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/false_positive.py` & `pyote-5.2.3/src/pyoteapp/false_positive.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/fixedPrecision.py` & `pyote-5.2.3/src/pyoteapp/fixedPrecision.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/genDiffraction.py` & `pyote-5.2.3/src/pyoteapp/genDiffraction.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/gui.py` & `pyote-5.2.3/src/pyoteapp/gui.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/helpDialog.py` & `pyote-5.2.3/src/pyoteapp/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/iterative_logl_functions.py` & `pyote-5.2.3/src/pyoteapp/iterative_logl_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,38 +215,36 @@
     sigma_b = 0.0
     sigma_a = 0.0
 
     r = left + min_event
 
     # Use numpy version of metric calculator to initialize iteration variables
 
-    # changed in 4.4.7
-    # b_s, b_s2, b_n, b_var = calc_metric_numpy(y[r + 1:right + 1])
-    b_s, b_s2, b_n, b_var = calc_metric_numpy(y[r:right + 1])
+    # B excludes y[r] and the extra point at right - but this is meaningless because r is incorrect at this point
+    b_s, b_s2, b_n, b_var = calc_metric_numpy(y[r + 1:right])
 
-    a_s, a_s2, a_n, a_var = calc_metric_numpy(y[left:r])
+    # A always excludes y[r]) - but this is meaningless because r is incorrect at this point
+    a_s, a_s2, a_n, a_var = calc_metric_numpy(y[left + 1:r])
 
     b = b_s / b_n
     a = a_s / a_n
 
     # Calculate metric for initial position of r
     metric = calc_metric()
     update_best_solution()
 
-    r_final = left + max_event
+    r_final = left + max_event - 1
 
     while r < r_final:
         # calc metric for next r position from current position
 
-        # changed in 4.4.7
-        # b_s, b_s2, b_n, b_var = sub_entry(y[r+1], b_s, b_s2, b_n, True)
-        b_s, b_s2, b_n, b_var = sub_entry(y[r], b_s, b_s2, b_n, True)
-
         a_s, a_s2, a_n, a_var = add_entry(y[r], a_s, a_s2, a_n, True)
         r += 1
+        b_s, b_s2, b_n, b_var = sub_entry(y[r], b_s, b_s2, b_n, True)
+
 
         metric = calc_metric()
         b = b_s / b_n
         a = a_s / a_n
 
         goodSolution = solution_is_better_than_straight_line(
                 y, left, right, -1, r, b, a, sqrt(b_var), sqrt(a_var), k=3)
@@ -310,44 +308,43 @@
     a_best = 0.0
     sigma_b = 0.0
     sigma_a = 0.0
 
     d = right - max_event  # Initial d position
 
     # Use numpy version of metric calculator to initialize iteration variables
+
+    # Excludes d from B - this is meaningless because d is incorrect at this point
     b_s, b_s2, b_n, b_var = calc_metric_numpy(y[left:d])
 
-    # changed in 4.4.7
-    # a_s, a_s2, a_n, a_var = calc_metric_numpy(y[d+1:right+1])
-    # a_s, a_s2, a_n, a_var = calc_metric_numpy(y[d:right+1])
-    # changed in 4.4.8
-    a_s, a_s2, a_n, a_var = calc_metric_numpy(y[d:right])
+    # Excludes d from A - this is meaningless because d is incorrect at this point
+    a_s, a_s2, a_n, a_var = calc_metric_numpy(y[d+1:right])
 
     b = b_s / b_n
     a = a_s / a_n
 
-    # print(b, a, b_n, a_n)
-
     # Calculate metric for initial position of d
     metric = calc_metric()
     update_best_solution()
 
     # d_final = right - min_event
     # changed in 4.4.7
     d_final = right - min_event + 1
 
     while d < d_final:
         # calc metric for next d position from current position
         b_s, b_s2, b_n, b_var = add_entry(y[d], b_s, b_s2, b_n, True)
 
         # changed in 4.4.7
         # a_s, a_s2, a_n, a_var = sub_entry(y[d+1], a_s, a_s2, a_n, True)
-        a_s, a_s2, a_n, a_var = sub_entry(y[d], a_s, a_s2, a_n, True)
+        # a_s, a_s2, a_n, a_var = sub_entry(y[d], a_s, a_s2, a_n, True)
 
         d += 1
+        a_s, a_s2, a_n, a_var = sub_entry(y[d], a_s, a_s2, a_n, True)
+
 
         metric = calc_metric()
         b = b_s / b_n
         a = a_s / a_n
 
         goodSolution = solution_is_better_than_straight_line(
             y, left, right, d, -1, b, a, sqrt(b_var), sqrt(a_var), k=3)
@@ -481,15 +478,14 @@
             r_max = r
             # ======= update_best_solution() ========
 
         solution_count += 1
 
     return d_max, r_max, b_max, a_max, sigma_b, sigma_a, max_metric, solution_count
 
-
 @njit  # cache=True gave pickling error
 def locate_event_from_d_and_r_ranges(
         y: np.ndarray, left: int, right: int, d_start: int, d_end: int,
         r_start: int,  r_end: int):
     """Finds the best size and location for event specified by d & r  ranges"""
 
     # The only time this function is called with a y containing 1 element
@@ -520,36 +516,32 @@
 
     while d <= d_end:
         # Use numpy version of metric calculator to initialize iteration
         # variables for current d and initial r_start
         r = r_start
 
         if d > left:
-            b_sl, b_s2l, b_nl, b_varl = calc_metric_numpy(y[left:d])
+            b_sl, b_s2l, b_nl, b_varl = calc_metric_numpy(y[left+1:d])
             # Lefthand wing
         else:
             b_sl = 0.0
             b_s2l = 0.0
             b_nl = 0
             b_varl = 0.0
 
-        # changed in 4.4.7
-        # b_sr, b_s2r, b_nr, b_varr = calc_metric_numpy(y[r+1:right+1])
-        b_sr, b_s2r, b_nr, b_varr = calc_metric_numpy(y[r:right+1])
+        b_sr, b_s2r, b_nr, b_varr = calc_metric_numpy(y[r+1:right])
 
         # Righthand wing
 
         b_s = b_sl + b_sr
         b_s2 = b_s2l + b_s2r
         b_n = b_nl + b_nr
         b_var = b_varl + b_varr
 
-        # changed in 4.4.7
-        # a_s, a_s2, a_n, a_var = calc_metric_numpy(y[d+1:r])
-        a_s, a_s2, a_n, a_var = calc_metric_numpy(y[d:r])
+        a_s, a_s2, a_n, a_var = calc_metric_numpy(y[d+1:r])
 
         # ============== calc_metric() =================
         max_var = max(a_var, b_var, MIN_FLOAT)
 
         if a_var <= 0.0:
             a_var = max_var
         if b_var <= 0.0:
@@ -584,19 +576,17 @@
             a_var_best = a_var
             b_n_best = b_n
             a_n_best = a_n
             # =========== update_best_solution() =======
 
         while r < r_end:
             b_s, b_s2, b_n, b_var = sub_entry(y[r], b_s, b_s2, b_n, True)
-            # changed in 4.4.8
-            # a_s, a_s2, a_n, a_var = add_entry(y[r-1], a_s, a_s2, a_n, True)
+            r += 1
             a_s, a_s2, a_n, a_var = add_entry(y[r], a_s, a_s2, a_n, True)
 
-            r += 1
             # ============== calc_metric() =================
             max_var = max(a_var, b_var, MIN_FLOAT)
 
             if a_var <= 0.0:
                 a_var = max_var
             if b_var <= 0.0:
                 b_var = max_var
```

### Comparing `pyote-5.2.2/src/pyoteapp/likelihood_calculations.py` & `pyote-5.2.3/src/pyoteapp/likelihood_calculations.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.2.3/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.2.3/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.2.3/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv` & `pyote-5.2.3/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.2.3/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.2.3/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/model-help.pdf` & `pyote-5.2.3/src/pyoteapp/model-help.pdf`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/noiseUtils.py` & `pyote-5.2.3/src/pyoteapp/noiseUtils.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,8 +51,13 @@
     if len(residuals) < 14:
         ans = [1.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
     else:
         ans = []
         for lag in range(11):
             ans.append(laggedCoef(residuals, lag))
 
-    return np.array(ans), len(x), np.std(residuals)
+    # This deals with no-noise test sets.
+    sigma = np.std(np.diff(np.array(y))) / np.sqrt(2.0)  # In place of: np.std(residuals)
+    if sigma == 0:
+        ans = [1.0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+
+    return np.array(ans), len(x), sigma
```

### Comparing `pyote-5.2.2/src/pyoteapp/pyote-info.pdf` & `pyote-5.2.3/src/pyoteapp/pyote-info.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 5% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,8 +1,17 @@
 Version history (PyOTE description – out of date - is at end)
+Version 5.2.3
+2 May 2023
+• Restores the calculation of timeDelta to 6 digit precision (it had been inadvertently
+limited to 4 digits by a previous change)
+•
+
+Fixes a bug in the calculation of flash edge times that was discovered when very high
+SNR recording was attempted
+
 Version 5.2.2
 13 April 2023
 • Adds diffraction modelling of an elliptical asteroid shape
 Version 5.2.1 27 March 2023
 • Fixed problem with VizieR loading from North American .xlsx caused by Occult
 sometimes putting a string in the asteroid field and sometimes an integer.
 •
@@ -33,24 +42,24 @@
 This was done so that the user is always made aware of the existence of multiple light
 curves read from the csv file.
 
 Version 5.1.6 11 February 2023
 • Fixes VizieR file preparation code to detect when lat or long is given with a + sign
 (common when input comes from reading a .xlsx file)and avoid adding a redundant +
 (double) character.
-•
+
+•
 
 Reverts to using pyqtgraph 0.12.4
 
 Version 5.1.0 7 February 2023
 • Changed the way data sets (lightcurves) read from a PyMovie csv file are selected for
 viewing. Whereas previously it was possible to specify a ‘prefix’ to be used when
 reading PyMovie csv files (such as ‘signal’ or ‘appsum’), it was not possible to mix-andmatch data sets with different prefixes. With this version, that now becomes possible.
-
-With this feature, it now becomes possible to demonstrate for yourself that there is no
+With this feature, it now becomes possible to demonstrate for yourself that there is no
 reason to process a target lightcurve in ‘aperture sum’ mode (no background
 subtraction) versus the regular ‘signal’ mode (where background subtraction is
 performed). Simply display the ‘signal’ and ‘appsum’ versions of a target lightcurve and
 use the y position spinBox on one of the curves until they overlap. This should show
 that during the event, the points almost exactly overlap, so event timing will be the
 same.
 •
@@ -84,23 +93,23 @@
 • model-examples folder is now being placed in the Documents folder rather than the
 Desktop folder.
 •
 
 Launch from python3 or python or py now detected and dealt with when checking PyPI
 repository for latest version.
 
-Version 5.0.2 8 January 2023
+Version 5.0.2 8 January 2023
 • Added timing problem report – counts of dropped readings; duplicated readings;
 cadence error. These appear in the log box (lower right corner) and are written to the
 log file.
 •
 
 Made D and R edge time calculations work properly even when there are dropped
+readings in the observation
 
-readings in the observation
 Version 5.0.0 6 January 2023
 • Added ability to specify a block size to be used during automatic block integration.
 When a block size is entered, the program will determine the best offset value to use
 for the integration.
 •
 
 Added a comprehensive set of lightcurve models together with tools to help automate
@@ -126,22 +135,22 @@
 using an additional color.
 Cadence jitter happens when high frame rates create a situation where frame recording cannot keep up and the traffic control implemented by the computer changes the
 arrival/timestamp time of frames so that some appear a little earlier and others a little
 late.
 Cadence jitter is defined as a timing discrepancy of between 20% and 80% of a frame
 time and is represented by a yellow line.
 Timing discrepancies greater than 80% of a frame time continue to be shown as a red
-line and are assumed to come from dropped frames. In any case, they deserve
+
+line and are assumed to come from dropped frames. In any case, they deserve
 attention.
 Version 4.8.8 7 August 2022
 • Added message at normal program close to the effect that QBasicTimer messages
 that appear after the program has closed are harmless artifacts of the order in which
 QUI elements are closed.
-
-Version 4.8.7 29 July 2022
+Version 4.8.7 29 July 2022
 • changed numpy version requirement to match that of PyMovie so that ultimately the
 two programs can share a virtual environment, thus saving much space.
 Version 4.8.6 23 July 2022
 • added instructions telling the user how to install a new version when one is found.
 There are instructions for pip based installations and pipenv installations
 Version 4.8.4
 • there are no changes. This is a new version just to test the change introduced in 4.8.3
@@ -169,23 +178,23 @@
 
 removes the writing of the startup batch file as a different method will be used in
 conjunction with pipenv.
 
 Version 4.7.9
 • disables the compiling to C code (which was done to increase execution speed) of
 routines used for finding an event using min/max size. There is compelling (but
-indirect) evidence that the C compiler on Win11 (and maybe only for the i5 processor)
+
+indirect) evidence that the C compiler on Win11 (and maybe only for the i5 processor)
 is generating incorrect code. This issue showed up recently with 2 users who had
 installed Win11 on i5 processor-based computer. On those machines, finding an event
 using min/max would always hang at 99% completion. Allowing the original Python
 code to be used instead of compiling to C-code resolved that issue. As finding an event
 using min/max size minimizes the number of candidate solutions naturally, the loss of
 speed is not so important – it’s fast enough.
-
-version 4.6.4
+version 4.6.4
 • made the 'camera response' checkbox (in the Settings/misc tab) sticky
 •
 
 corrected the log messaging about Donly, Ronly, DandR, and min/max directions to the
 solver consistent
 
 version 4.6.3
@@ -215,20 +224,23 @@
 have the side effect (on some computers – but none of mine) of suppressing the cursor
 change when hovering over a splitter. As this is confusing, the busy cursor feature has
 been removed.
 version 4.5.5
 • fixes a bug where, if a full D and R light-curve was split (trimmed) into a D-only and an
 R-only light-curve, the R-only result did not apply subframe timing adjustments
 version 4.5.4
-• cleans up the the first bin of the False-Positive histogram
+
+•
+
+cleans up the the first bin of the False-Positive histogram
+
 version 4.5.3
 • adds an option to validate a single point event to the Analysis tab. It uses the falsepositive test procedure to determine if the selected point had a non-zero chance to
 have been caused by baseline noise alone.
-
-version 4.5.2
+version 4.5.2
 • fixes a bug where transition points (only present in high SNR light-curves) were not
 properly ignored during calculation of event noise. This manifested itself most clearly in
 too large error bars for magDrop
 version 4.5.0
 • fixes a bug introduced with the NE3 code changes that inhibited sub-frame timing
 adjustments.
 version 4.4.9
@@ -254,30 +266,33 @@
 simple standard deviation metric
 •
 
 made it possible to select the points of the normalized target lightcurve to be included
 in the std metric
 
 version 4.3.6
-• added a simple metric as an aid to selecting an appropriate number of readings to use
+
+•
+
+added a simple metric as an aid to selecting an appropriate number of readings to use
 to smooth the reference curve used for normalization. It is printed in green whenever
 normalization is active. It is simply the standard deviation of the normalized target
 lightcurve. Although it is quite simple, it is a value that is minimized the more level and
 the less bumpy the normalized target curve is.
 When normalization is active, at each change, a pair of metrics are printed in the log
-
-panel.
+panel.
 The red metric is the Pearson R value of the correlation between the target lightcurve
 and the reference lightcurve; it should be maximized (using the X offset spinbox of the
 reference curve) at the point where the two curves are properly time-aligned. It is also
 affected by the smoothing interval, but this connection should be ignored.
 The green metric is the standard deviation of the target lightcurve – it is lowered when
 the target lightcurve has a minimum slope and the fewest and shallowest bumps. Use
 the spinbox for the number of readings in the smoothing interval to minimize this
 number.
+
 version 4.3.5
 • made the 'step-by' buttons radio buttons so that it is clear what the current step size is.
 •
 
 removed the automatic switch to the Lightcurve panel
 
 version 4.3.3
@@ -297,24 +312,27 @@
 version 4.3.1
 • fixes an error message that occurs during the initial installation of a version that has a
 change to the number of tabs in the GUI
 version 4.3.0
 • minor cosmetic cleanup to deal with Windows GUI differences (I hope it works – this is
 always a frustrating and mysterious area)
 version 4.2.9
-• adds the lightcurve used to the report generated during the detectability analysis
+
+•
+
+adds the lightcurve used to the report generated during the detectability analysis
+
 •
 
 automatically clears the effect of previous normailzation when the reference lightcurve
 is changed (or deselected)
 
 version 4.2.8
 • fixes 'trim problem'
-
-•
+•
 
 adds 'step by' buttons that change the smoothing interval spinbox step size.
 
 version 4.2.6
 • tidies up the lightcurve panel a bit and changes color samples for target and reference
 curves.
 version 4.2.5
@@ -352,22 +370,22 @@
 
 version 4.2.2
 • adds a new tab/panel for controlling the display of lightcurves. From the 'help button'
 on that tab:
 This panel allows up to 10 lightcurves to be displayed at the same time. If the csv file has
 more than 10 lightcurves, the first 10 are displayed.
 The target lightcurve is always drawn with bright blue dots.
-If a lightcurve is selected as a reference to be used for normalization, it is always
+
+If a lightcurve is selected as a reference to be used for normalization, it is always
 drawn with bright green dots.
 Unless a lightcurve is designated as a target (curve to be analyzed for an event) or is
 designated as a reference lightcurve, its dot color depends on the row it is in - every
 row has a unique color other than blue or green.
 Lightcurves can be displaced up or down using the Y offset spinner to control the
-
-displacement. This affects the display position only; the underlying values are not
+displacement. This affects the display position only; the underlying values are not
 affected. This facility was added to allow the separation of lightcurves that would
 otherwise overlap in a confusing manner.
 There can only be one lightcurve selected as target.
 There can be either 0 or 1 lightcurve selected as a reference for normalization.
 Normalization is applied whenever the normalization reference curve smoothing
 interval spinbox is changed from 0. Whenever this number is changed, a new
 normalization will result. If this number is returned to zero, all normalization is removed
@@ -399,27 +417,27 @@
 • fixes (hopefully) Win 11 issue involving the directory separator character \
 Win 10 accepts / as a separator – Win 11 apparently does not (unless there is some
 setting that will persuade Win 11 to accept either separator.
 version 4.1.8
 • adds option to write sample light-curve from detectability analysis to a csv file that be
 imported to PyOTE.
 version 4.1.7
-• adds the requirement to specify an observation duration when doing a detectability test
+
+•
+
+adds the requirement to specify an observation duration when doing a detectability test
+
 •
 
 during a detectability test, if a detectable event was found, a sample light-curve
 showing such an event is plotted, otherwise the normal False-Positive plot will be
 shown.
 
 version 4.1.6
-
-•
-
-reenables Cholesky failure messages (disabled for testing)
-
+• reenables Cholesky failure messages (disabled for testing)
 •
 
 Adds test to detectability routine so that the user cannot give an event duration that
 requires more points than are available in the observation.
 
 version 4.1.5
 • changed error bar calculation reporting so that the the value reported in the
@@ -465,28 +483,28 @@
 use whatever level of noise reduction you may need. It is recommended that you run
 your NE3 at a gamma of 0.75 (1.0 gamma is not available) AND that you use PyMovie
 to linearize the recording (i.e., invert the 0.75 gamma curve of the camera).
 
 •
 
 The D and R exponential curves each have their own time constant, measured in
-frames, that control the frame rate of exponential curve growth. The default values
+
+frames, that control the frame rate of exponential curve growth. The default values
 provided are usually enough to provide the starting point for a good fit. This starting
 point is used by PyOTE during a least-squares driven search for better time constant
 values. If the starting point given is too far from 'correct', the least-squares search may
 settle in a local minimum that produces a fit that is visually bad. In this case, change
 the starting value to something closer to 'correct' and try again.
-
 •
 
 When the exponential curve fit algorithm is in use, the light-curve plot PyOTE displays
-
-will be changed. Gone is the blue 'camera response' curve, replaced by brown dotted
+will be changed. Gone is the blue 'camera response' curve, replaced by brown dotted
 'theoretical' exponential edge curves that you can use to judge for yourself the
 goodness of a 'fit'.
+
 •
 
 You will probably want to use the most aggressive noise reduction in most cases, but
 make sure that your expected event duration is long enough that the D transition
 exponential curve has time to settle to the bottom event plus some time to allow a good
 determination of the event bottom intensity. At DNR:HIGH, your expected event time
 should be greater than 30 frames (1 second) to use this setting.
@@ -514,21 +532,21 @@
 version 4.0.8
 • fixes bug (introduced by a misspelling in version 4.0.7) that kept csv files with more
 than four apertures from runnig.
 version 4.0.7
 • adds the ability to select the PyMovie data column type to be analyzed. There are two
 main column types that are likely to be used: signal, which has background subtracted
 and appsum, which has no background subtracted – it's the raw mask pixels summed.
-Some others are available: avgbkd (shows the average pixel value in the aperture);
+
+Some others are available: avgbkd (shows the average pixel value in the aperture);
 stdbkg (shows the pixel noise in the background pixels in the aperture); nmaskpx
 (which shows the nuber of pixels in the sampling mask – there are times when this
 curve can be used to extrat event times).
 Note: this only applies to csv files generated by PyMovie.
-
-version 4.0.6
+version 4.0.6
 • minor GUI changes
 version 4.0.5
 • if you click outside the light-curve, the closest point will be toggled (so you don't have
 to zoom in to select the leftmost or rightmost point in a light-curve.
 •
 
 When baseline statistics are calculated, they are reported as baseline mean and
@@ -561,21 +579,21 @@
 
 version 4.0.2
 • removed a debug print statement that was inadvertently left in. It is responsible for the
 “mouse event” messages polluting the log file.
 version 4.0.1
 • increased width of detectibility plots to (hopefully) deal with Windows tendency to
 truncate the plots. If this doesn't work, then this will be a permanent feature (not a bug)
-for Win10 installations.
+
+for Win10 installations.
 version 4.0.0
 • detectibility graphics plots are now being being put in their own folder. The root folder is
 that of the directory where the light-curve came from. The plots will be found in
 lightCurveDirectory\DetectibilityPlots\
-
-In addition, if you supply a duration step size, which is the way to ask the detectibilty
+In addition, if you supply a duration step size, which is the way to ask the detectibilty
 calculator to step from the given duration down until an event of that duration fails the
 False-positive test, only the final plot (where False-positive became non-zero) will be
 plotted.
 All of the above is just to cut down on clutter in the light-curve directory and to only plot
 meaningful graphics generated during the minimum duration search.
 version 3.9.9
 • whew! 3.9.8 did solve the sizing issue. So it is safe to get back in the water so...
@@ -601,21 +619,21 @@
 sticky stuff.
 This version also removes the 'scrunch' of the lefthand button panel.
 version 3.9.6
 • another attempt fix the startup gui size issue on smaller legacy monitors. This version
 has a design size of 1900x1000. It may be necessary to delete the simple-ote.ini file
 that 'remembers' size and position settings. It is located in whatever directory PyOTE
 starts up in.
-version 3.9.5
+
+version 3.9.5
 • adds automation to the 'detectibility' calculator. If a duration step size is entered, a
 series of 'detectibility' calculations will be made at decreasing durations until the falsepositive probability becomes non-zero. A unique .png (incorporates duration and
 magDrop in the file name) will be written to the directory of the light-curve and the final
 plot where detection failed will be left on-screen.
-
-If the duration step size is left unfilled or is zero, a single 'detectibility' calculation will be
+If the duration step size is left unfilled or is zero, a single 'detectibility' calculation will be
 made as before.
 version 3.9.4
 • attempts to fix over-size initial gui.
 version 3.9.3
 • makes various improvements to the 'detectability' calculator to make it easier to use.
 version 3.9.2
 • adds a 'detectability' calculator for use in pre-planning event observation.
@@ -640,24 +658,21 @@
 • fixed a bug that sometimes kept events that contained a single point at the bottom from
 producing a report.
 version 3.8.7
 • changed the way curve to analyze and normalization curve are selected to make it less
 confusing. Now, if there is a conflict (same curve selected for analysis and
 normalization) the other one is set to 0 (a new value) to 'get it out of the way'. It may
 still be a little bit confusing when you need to crossover, but if you set the higher
-numbered curve first, it will be easy.
+
+numbered curve first, it will be easy.
 version 3.8.6
 • checks for only a single light-curve in the csv file which was causing a 'list index out of
 range' error message
 version 3.8.5
-
-•
-
-changed the way QGridLayout was referenced.
-
+• changed the way QGridLayout was referenced.
 version 3.8.4
 • changed the way QTableWidgetItem and QApplication were referenced to
 accommodate the latest Anaconda version, which has reorganized where those
 modules are stored. A similar change was made in version 3.7.6 and I do not know
 how this has gone uncorrected for so long – I hope that I have not missed something.
 version 3.8.3
 • adds display of light-curve name (if available in the csv file) to the curve-to-be-analyzed
@@ -684,22 +699,22 @@
 the flash itself adversely affects the baseline values. With this new tool, the regions of
 the baseline that are outside the 'flash-zone' can be specified. Look for a button
 labelled Mark baseline region located near the bottom-left of the GUI panel.
 This tool may also be useful for wind-gust situations, headlights from passing cars,
 bumping the telescope, etc. In the past, such accidents might have required extensive
 'clipping' of the light-curve to avoid the affected areas, with a consequent loss of
 information. Hopefully this tool will alleviate those situations.
-version 3.7.8
+
+version 3.7.8
 • added visible left, top, and bottom axes to main plot (with ticks to make easier to
 associate timestamp with point).
 version 3.7.7
 • if timestamps are available in the csv file, they are used as x axis labels in the main
 plot.
-
-version 3.7.6
+version 3.7.6
 • changed the way QMainWindow and Qapplication were referenced to accommodate
 the latest Anaconda version, which has reorganized where those modules are stored.
 This was causing a fatal startup error.
 version 3.7.5
 • changes the routine that looks for the latest version of PyOTE to one provided by Kia
 Getrost. His version contacts the PyPI repository via a json query and is the officially
 supported way to get version info. My version was based on a 'hack' that depended on
@@ -724,27 +739,25 @@
 • adds code line needed by any Mac users that are running Big Sur
 version 3.7.2
 • fixes bug that caused all analysis attempts to 'stall'
 version 3.7.1
 • fixed a bug in the r limb angle entry
 version 3.7.0
 • adds right-click help to ast speed label giving the equation to use if asteroid
-speed is not available but asteroid diameter and maximum duration are
+
+speed is not available but asteroid diameter and maximum duration are
 specified
 •
-version 3.6.8
 
 adds suggestion to right-click help on penumbral fit checkbox for how to find the
 penumbral curve csv file that is provided for practice purposes.
 
-•
-
-adds modeling of off centerline observations to lightcurve calibration curve
+version 3.6.8
+• adds modeling of off centerline observations to lightcurve calibration curve
 generation
-
 version 3.6.7
 • clarified the location of the Enable Manual Timestamp Entry checkbox in the
 pop-up message appears when there are no timestamps in the csv file.
 version 3.6.6
 • modified the lightcurve demo to show more clearly the camera exposure
 function and the star intensity function that are convolved with the diffraction
 lightcurve to produce the lightcurve as seen by the camera.
@@ -766,21 +779,19 @@
 … now writing numbers into numeric cells rather than text. This allows the cell
 formatting to control rounding, etc
 … if I can't write to the selected file, I ask whether you might have it open
 somewhere else already
 version 3.6.1
 • reduced number of digits in the error bar numbers to 2 written to the Asteroid
 Occultation Report Form so that the resulting number fits within the allotted cell
-size. (I'm told that Occult only uses 2 digits anyway.) I also updated the context
+
+size. (I'm told that Occult only uses 2 digits anyway.) I also updated the context
 help associated with the … fill Excel report button
 version 3.6.0
-
-•
-
-provides the ability to fill entries in the Excel spreadsheet Asteroid Occultation
+• provides the ability to fill entries in the Excel spreadsheet Asteroid Occultation
 Report Form from PyOTE results, thus eliminating transcription errors.
 A button to allow the user to activate this 'fill' has been added just to the right of
 
 the … write report button
 NOTE: the normal .xls report form that OccultWatcher creates and prefills (when
 requested) during your report to OccultWatcher ...
 … MUST BE CONVERTED to .xlsx for use by PyOTE!
@@ -800,20 +811,23 @@
 After filling in the exposure setting in the spreadsheet, double check the form but it is likely
 that it is ready for submission.
 version 3.5.9
 • fixed another bug in penumbral curve fit and removed diagnostic printouts.
 version 3.5.8
 • fixed a number of bugs in the penumbral curve fit code
 version 3.5.7
-• automatically turns off the display of the normalizing lightcurve when a
+
+•
+
+automatically turns off the display of the normalizing lightcurve when a
 normalization is performed. It was a source of confusion to leave the normalizing
 lightcurve visible because it was sometimes the case that the normalization
 appeared not to have occurred (when the normalization effect was
+subtle/minor).
 
-subtle/minor).
 version 3.5.6
 • fixed a bug that kept a user from selecting a new file to read if PyOTE had been
 started from PyMovie. Previously, it had only reopened the same file instead of
 giving the user a file select dialog to choose from.
 version 3.5.5
 • fixed a bug that kept occultations from being extracted from lightcurves 5 and
 up. The lightcurves above 4 could be viewed --- they just couldn't be processed
@@ -842,19 +856,19 @@
 PyOTE is to enable infrequent/inexperienced users to get dependable results
 without requiring in-depth understanding of the internal workings of the program,
 we have decided to make the end-point smoothing issue very apparent by doing
 an automatic 'trim' of the points affected by extrapolation.
 version 3.5.1
 • Added additional references to the North American Excel Spreadsheet report in
 the new section of the final report that bangs on about the start-of-exposure
-timing convention.
+
+timing convention.
 version 3.5.0
 • When PyMovie files are read, the aperture names are now being used in the
-
-data table (lower left panel) as column headings and used during the 'write csv'
+data table (lower left panel) as column headings and used during the 'write csv'
 process. This makes the format of the PyOTE csv file match the PyMovie
 format so that AOTA can read both PyMovie csv files AND PyOTE csv files.
 •
 
 NEW: when 'trims' have been placed, a 'write csv' process will honor those
 values and produce a 'trimmed' output file.
 
@@ -887,23 +901,20 @@
 16% of the time we can only report that the calculation could not be performed.
 The above observation suggests that reliable estimates of magDrop require that A be greater
 than std(A) --- that is the ad hoc reason that we have defined limMagDrop as we have.
 This value is substituted for a calculated magDrop whenever A is less than std(A), i.e.,
 whenever A is at or below std(A).
 limMagDrop values are reported with a leading > symbol to signify that that value is a
 limMagDrop value. They are easy to spot in the report.
-version 3.4.7
+
+version 3.4.7
 • Automatically loads the correct version of Adv2
 version 3.4.6
-
-•
-
-Adds AAV Version 2 file as a type that can be read (important when Do OCR
+• Adds AAV Version 2 file as a type that can be read (important when Do OCR
 check is enabled)
-
 version 3.4.5
 • Fixes block integration which was failing when more than 4 lightcurves were
 being processed.
 •
 
 Made use diff and Do OCR checkboxes sticky.
 
@@ -933,29 +944,29 @@
 checkboxes to control whether the underlying lightcurve is plotted, error bars are
 plotted, or edges are plotted --- a cleaner plot is the major result and you have
 better control over the 'look'
 •
 
 Added a checkbox to disable the automatic display of D and R frames from the
 video for OCR quality control checks. When there are no concerns about OCR
-reliability (true for me nearly all the time), it can be annoying to have to close the
-frames all the time.
 
+reliability (true for me nearly all the time), it can be annoying to have to close the
+frames all the time.
 •
 
 The BIG change is the addition of a penumbral curve fit procedure. It's a bit
-
-fiddly, so I included a test lightcurve with the download. I can't give you a
+fiddly, so I included a test lightcurve with the download. I can't give you a
 specific location for the file because it depends on details of your particular
 installation. Find where it is by searching for example-penumbral.csv When
 you find it, copy or move it to some other folder because if you process it where
 it resides, other files will get added in your installation directory --- we really don't
 want extraneous non-program files floating around in your installation directory.
 To learn how to use the new procedure (which is a bit 'fiddly'), right-click on the
 penumbral fit checkbox --- be patient; play around.
+
 version 3.4.0
 • Adds the ability to specify a diffraction lightcurve for use in timing the event. A
 new panel with edit boxes for asteroid/occulting body distance (in AU --astronomical units) and asteroid/shadow speed (in km per second) has been
 added. These values are needed in order to calculate a diffraction light curve.
 In addition to modeling diffraction effects, one can add the effect of a finite star
 disk to produce a penumbral curve. NOTE: PyOTE does not yet have the ability
 to correctly analyze a penumbral curve where it takes more than 1 or 2 readings
@@ -975,20 +986,20 @@
 prepare the .csv file that is currently being analyzed. .avi and .ser files are viewable in
 this manner as well as .fits files inside a FITS folder.
 If this button is disabled, it is because the .csv file did not come from PyMovie or
 Limovie or simply cannot be found/opened.
 This feature can/should be used as a final quality control check for a video that
 contains timestamps extracted using OCR. It is possible for OCR to fail in manner that
 is not detected by PyOTE because the program only verifies that there is a consistent
-step (delta time) between frames. If a high order digit in the timestamp has been
+
+step (delta time) between frames. If a high order digit in the timestamp has been
 consistently misread, substituting a 8 for a 9 in the minutes field for example, the steps
 can be consistent while the reported time of the event will be seriously in error.
 ALL time reporting is derived from the timestamp(s) associated with D and/or R (the
-
-integer values, not the sub-frame values). If those timestamps are correct, the reported
+integer values, not the sub-frame values). If those timestamps are correct, the reported
 times will be correct even when there may be a few missing or duplicated frames. So
 best practice is to enter the D frame value in the spin box and visually confirm that the
 timestamp that you can see is the same as that extracted by the OCR procedure.
 Repeat for R.
 Another use for this feature is to handle the case where there is a visual timestamp, but
 either OCR was not activated during the .csv preparation, or the timestamp overlay
 came from an unsupported VTI type. The workflow would be to let PyOTE find the D
@@ -1016,19 +1027,19 @@
 the size (duration) extracted from the actual observation, but with only correlated
 noise in the sample (the number of points in this sample is equal to the number
 of points used in the lightcurve extraction). 50,000 attempts are made to find
 the deepest event that appears (falsely) when there is only noise being
 analyzed. If the drop from the actual observation is greater than the maximum
 size of a 'false drop', we have some assurance that the event extracted from the
 actual observation did not happen 'by chance'.
-version 3.2.9
+
+version 3.2.9
 • Changed main plot so that the scroll wheel only zooms the x axis.
 • Changed lightcurve plot so that it conforms properly to 'start-of-exposure'.
-
-version 3.2.8
+version 3.2.8
 • Changed font size in help files --- it was fine for Mac but too big for Win10
 version 3.2.7
 • Removed the 'hover-for-help' and replaced it with a 'right-click-on-item' to get
 help. This scheme was introduced in PyMovie and I found it easier to use than
 the 'hover' scheme. In practice, the 'hover' popped up when it was not needed,
 so most users eventually disabled it. As a result, it became so tedious to look at
 help --- enable hover; hover; read; disable hover --- that the help system was
@@ -1060,20 +1071,19 @@
 LC3 == LC4 whenever there was an actual LC4. It was correct in the lightcurves
 themselves, so no observation analyses have been affected by this bug. It was
 cosmetic only.
 •
 
 Added support for the PyMovie csv format
 
-version 3.2.1
+version 3.2.1
 • this version makes PyOTE more robust to a common 'cockpit error' that users
 have been making with Tangra files. Specifically, if a Tangra csv file is opened
 in a spreadsheet program, then saved from that spreadsheet program, the
-
-original csv file gets modified and overwritten by the addition of empty fields at
+original csv file gets modified and overwritten by the addition of empty fields at
 every row sufficient to match the number of columns in the longest
 header/comment row --- the spreadsheet program did this to satisfy its internal
 requirement that every row have an equal number of columns. The result is
 superfluous commas at the end of data lines (that Tangra did NOT put there).
 Until this version, that 'butchered' file could not be read. This version adds code
 to parse data lines only up to the first non-empty column. Hopefully this will not
 have ramifications in the future (like a format change that has empty fields
@@ -1102,21 +1112,21 @@
 making corrections easy to do without requiring re-entry of all data.
 Also trapped is the case where a user has entered a custom frame time but failed to click the
 radio button indicating that it is to be used.
 version 3.1.5:
 • Added additional tests of candidate solutions against a straight line so that there
 should always be agreement between a solution found by a min/max event size
 search and a marked D and R region search of the same area.
-Previously it was possible for the min/max search, which searches the entire
+
+Previously it was possible for the min/max search, which searches the entire
 light curve, to be tripped up by what we call a 'competitor'. A 'competitor' is an
 'event' with good statistics. However, that 'competitor' may have a small
 magDrop and so later be rejected when we compare with a straight line solution.
 That 'competitor' would thus mask an event with slightly worse statistics but a
-
-larger magDrop. The change was to test every candidate against a straight line
+larger magDrop. The change was to test every candidate against a straight line
 during the search. This does make the search time longer, but not too much
 longer.
 version 3.1.4:
 • Fixed error in new dropped reading detection logic when light curve was
 processed in field mode.
 •
 
@@ -1154,24 +1164,24 @@
 the min event too large or the max event too small, the resulting 'solution' will be
 artificially constrained and thus be wrong. This situation is now detected and a
 log entry as well as a pop-up alert will tell the user to change the limits and try
 again.
 •
 
 Three magDrop values are now calculated for each confidence level: the largest
-magDrop calculated using B + err(B) along with A – err(A); the nominal
+
+magDrop calculated using B + err(B) along with A – err(A); the nominal
 magDrop calculated using B and A; the minimum magDrop calculated using
 B – err(b) along with A + err(A)
-
 •
 
 The labels on the Find Event button and the Calc Err Bar button were changed
-
-to more clearly suggest that after finding an 'event', one should then press the
+to more clearly suggest that after finding an 'event', one should then press the
 'report' button to the right in order to complete the process.
+
 version 3.1.0:
 • Added a Mac version of a pyote startup file. It is automatically placed on the
 Desktop the first time pyote is run. Double-clicking on that Desktop file icon will
 start pyote thereafter.
 version 3.0.8:
 • Added a Windows batch file to the distribution that, when executed, will startup
 pyote. The file is called PYOTE.bat and is automatically copied to
@@ -1197,25 +1207,22 @@
 curve. As such a click removes the color bars that result from the automatic
 block integration analysis, it seems intuitive to disable the Accept integration
 button at that time as well.
 version 2.1.5:
 • Disable the Accept integration button when user overrides an automatic block
 analysis with a manual block selection followed by a click on the Block integrate
 button.
-version 2.1.4:
+
+version 2.1.4:
 • Corrected a bug that kept manual selection of block integration from being
 performed after a refusal to accept the automatic block analysis results.
 version 2.1.3:
-
-•
-
-A minor change to how color bars are plotted when the automatic block
+• A minor change to how color bars are plotted when the automatic block
 integration feature is employed. The edges now appear between data points so
 the bands are easier to see, particularly for 2 point block sizes.
-
 version 2.1.2:
 • To ease usage of the automatic block integration feature, accepting the
 automatically determined block integration parameters no longer uses a modal
 query box, which interfered with the ability to explore/expand the light curve plot.
 Now there is separate button which gets enabled after an automatic block
 integration completes.
 version 2.1.1
@@ -1241,27 +1248,28 @@
 block integration. As a result, once block integration has been performed after a
 file read, it cannot be done again; a reread of the original file is now required.
 version 2.0.7
 This version provides several features to ease the processing of light curves that are
 timed with LED flashes from iPhones (John Grismore's AstroFlashTimer) or Android
 phones (Eric Couto's Occult Flash) rather than VTI timestamped files
 •
-•
 
 Adds a button to calculate the edge position of an LED timing flash.
-Adds a checkbox to enable/disable the tooltip messages that appear when a
-control is hovered over. Tooltip display defaults to 'enabled' because tooltips are
-an important aid for guiding users initially. Later, when such help is no longer
-needed, the user can turn them off (they are annoying when you don't need
-them).
 
 •
+
+•
 •
 •
 
+Adds a checkbox to enable/disable the tooltip messages that appear when a
+control is hovered over. Tooltip display defaults to 'enabled' because tooltips are
+an important aid for guiding users initially. Later, when such help is no longer
+needed, the user can turn them off (they are annoying when you don't need
+them).
 Adds the ability to select which light curve is to be analyzed. Previous versions
 would only analyze the first light curve for D and R events. This flexibility is
 useful in general, but was particularly needed to support LED flash timing.
 Adds a checkbox to force manual entry of timestamp info. This is useful when
 OCR on a VTI timed light curve has catastrophic errors. It is always employed
 when using LED flash timing.
 During the error bar calculation, it is possible for the Cholesky decomposition
@@ -1292,21 +1300,22 @@
 • detects and handles situations in which fewer than 14 baseline points are
 available for calculation of correlated noise coefficients. When fewer than 14
 points are available, the correlation coefficients are set to: [1, 0, …] (i.e.,
 coefficients are set to 'no correlated noise')
 version 2.0.2
 • Note: this version has many significant changes. If you lose confidence in this
 version, remember that you can always go back to version 1.47 by typing --pip install pyote==1.47
-in an Anaconda console. (Be sure to use double == signs in the command.)
+
+in an Anaconda console. (Be sure to use double == signs in the command.)
 •
 
 improved handling of D and R region selection so that one cannot enter an
 invalid configuration --- automatic corrections/changes are applied.
 
-•
+•
 
 incorporates a new 'solver' that no longer requires an initial estimation of
 baseline noise. This 'solver' is also much faster. With this 'solver', the two-pass
 modification added in version 1.46 is no longer needed.
 
 •
```

### Comparing `pyote-5.2.2/src/pyoteapp/pyote.py` & `pyote-5.2.3/src/pyoteapp/pyote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1201,35 +1201,35 @@
                     self.Lcp.metricLimitLeft = leftLimit
                     self.Lcp.metricLimitRight = rightLimit
                     self.showInfo(f'Metric will be calculated using data points from {leftLimit} to {rightLimit} inclusive.')
                 else:
                     self.showInfo(f'The reading numbers supplied are invalid.')
 
     def plotFamilyOfLightcurves(self):
-        def move_figure(f, x, y):
+        def move_figure(f, x, y):  # noqa
             backend = matplotlib.get_backend()
             if backend == 'TkAgg':
                 f.canvas.manager.window.wm_geometry("+%d+%d" % (x,y))
             elif backend == 'WXAgg':
                 f.canvas.manager.window.SetPosition((x,y))
             else:
                 f.canvas.manager.window.move(x,y)
 
-        def plot_curve_set(calculate_curves, x, yOut):
+        def plot_curve_set(calculate_curves, x, yOut):  # noqa
             fig = plt.figure(constrained_layout=False, figsize=(10, 8))
             fig.canvas.manager.set_window_title("Family plot")
-            ax1 = fig.add_subplot(1, 1, 1)  # lightcurve axes
+            ax1 = fig.add_subplot(1, 1, 1)  # noqa lightcurve axes
 
             self.showMsg("", blankLine=False)
             if calculate_curves:
                 self.showMsg(f'Initiating computations ...', bold=True, color='red', blankLine=False)
-            for i in range(1, numCurves + 1):
+            for i in range(1, numCurves + 1):  # noqa
                 if calculate_curves:
                     QtWidgets.QApplication.processEvents()
-                    x, y, D_edge, R_edge = generalizedDiffraction(LCP=self.Lcp, wavelength1=None, wavelength2=None,
+                    x, y, D_edge, R_edge = generalizedDiffraction(LCP=self.Lcp, wavelength1=None, wavelength2=None,  # noqa
                                                                   skip_central_calc=False)
                     if i == 1:
                         ax1.set_ylim(0, 1.1 * np.max(y))
 
                     yOut.append(y)
                 else:
                     y = yOut[i-1]
@@ -1340,15 +1340,14 @@
         else:
 
             sample_index_step = self.Lcp.shadow_speed * self.Lcp.frame_time / (x[1] - x[0])
 
             referenceCurveNumber = numCurves // 2 + 1
 
             noiseValues = []
-            noiseValue = None
             gotNoiseValue = True
             while gotNoiseValue:
                 if not noiseValues:
                     noiseValue, gotNoiseValue = QtWidgets.QInputDialog.getDouble(
                         self, ' ', 'First noise level (sigmaB) to use:', decimals=5)
                 else:
                     noiseValue, gotNoiseValue = QtWidgets.QInputDialog.getDouble(
@@ -1363,15 +1362,14 @@
             for value in noiseValues:
                 if value < 0:
                     self.showInfo(f'A noise level specified is negative --- aborting.')
                     return
 
             sampled_y = [[] for _ in range(numCurves)]
             xpts = []
-            i = 0
             sample_index = -sample_index_step
             i_limit = len(yVec[0])
             for k in range(numCurves):
                 while True:
                     sample_index += sample_index_step
                     i = round(sample_index)
                     if i >= i_limit:
@@ -2327,50 +2325,14 @@
                 return
         except ValueError as e:
             self.showInfo(f'wavelengthEdit: {e}')
             return
 
         self.processModelLightcurveCoreEdit()
 
-    # TODO Remove this experimental code
-    def sampleFamilyLightCurve(self, x_values_km, y_values):
-        # Build interpolation function. This is done to deal with the finite resolution of
-        # the 2048 point lightcurve
-        x_values_sec = x_values_km / self.Lcp.shadow_speed
-        x_values_sec -= x_values_sec[0]
-        tObsStart = convertTimeStringToTime(self.yTimes[0])
-        x_values_sec += self.modelTimeOffset + tObsStart
-
-        interpolator = interpolate.interp1d(x_values_sec, y_values)
-
-        sample_time = tObsStart
-
-        # x_vals will be reading numbers
-        x_vals = []
-        y_vals = []
-
-        while sample_time <= x_values_sec[-1]:
-            if sample_time >= x_values_sec[0]:
-                # Compute x_vals as reading number
-                x_vals.append(round((sample_time - tObsStart) / self.Lcp.frame_time))
-                y_vals.append(interpolator(sample_time))
-            sample_time += self.Lcp.frame_time
-            # This keeps us from from sampling the model curve past
-            # the end of the observation
-            if len(x_vals) >= self.dataLen:
-                break
-
-        if len(x_vals) == 0:
-            breakpoint()
-
-        x_samples = np.array(x_vals)
-        y_samples = np.array(y_vals)
-
-        return x_samples, y_samples
-
     def sampleModelLightcurve(self):
         # Build interpolation function. This is done to deal with the finite resolution of
         # the 2048 point lightcurve
         interpolator = interpolate.interp1d(self.modelPtsXsec, self.modelY)
 
         tObsStart = convertTimeStringToTime(self.yTimes[0])
         sample_time = tObsStart
@@ -2451,26 +2413,14 @@
         # aiccValue = aicc(log_likelihood, n=len(sigmaValues), k=1)
         # Remove this print statement
         # self.showMsg(f'log_likelihood: {log_likelihood:0.4f}  aicc: {aiccValue:0.4f}')
 
         matchingObsYvalues = np.array(matchingObsYvalues)
         modelYsamples = np.array(modelYsamples)
 
-        # TODO Experimental code to measure uncertainty in metric
-        # metrics = []
-        # test_noise = modelSigmaB * 0.2
-        # num_trials = 4000
-        # for i in range(num_trials):
-        #     renoisedObs = matchingObsYvalues + np.random.normal(0, test_noise, matchingObsYvalues.size)
-        #     noisedMetric = np.sum(((modelYsamples - renoisedObs) / np.sqrt(modelSigmaB**2 + test_noise**2))**2) / modelYsamples.size
-        #     metrics.append(noisedMetric)
-        #
-        # metrics = np.array(metrics)
-        # self.showMsg(f'mean metric: {np.mean(metrics):0.4f}   std metrics: {np.std(metrics):0.4f}')
-
         # We produce these values as a side effect - only used during edge-on-disk (penumbral) fits
         self.dMetric = np.sum(((modelYsamples[0:center_frame] - matchingObsYvalues[0:center_frame]) / modelSigmaB)**2) / modelYsamples.size
         self.rMetric = np.sum(((modelYsamples[center_frame:] - matchingObsYvalues[center_frame:]) / modelSigmaB)**2) / modelYsamples.size
 
         # totalMetric = np.sum(((modelYsamples - matchingObsYvalues) / modelSigmaB)**2) / modelYsamples.size
         totalMetric = self.dMetric + self.rMetric
 
@@ -7776,22 +7726,26 @@
         if R:
             R = trunc(floor(R))
 
         if not self.userDeterminedBaselineStats:
             self.corCoefs = []
 
         if D and R:
-            self.sigmaA = None
-            # self.corCoefs = []
+            # D - 1 is specified so that the D point is excluded from the noise and B level calculations
+            self.processBaselineNoiseFromIterativeSolution(self.left, D - 1)  # Left side
+            newBleft = self.B  # This is filled in by the above call
+
+            # R + 1 is specified so that the R point is excluded from the noise and B level calculations
+            self.processBaselineNoiseFromIterativeSolution(R + 1, self.right)  # Right side
+            newBright = self.B
 
-            self.processBaselineNoiseFromIterativeSolution(self.left, D - 1)
-
-            self.processBaselineNoiseFromIterativeSolution(R, self.right)
+            self.B = (newBleft + newBright) / 2
 
-            self.processEventNoiseFromIterativeSolution(D, R - 1)
+            # D + 1 and R -1 are used to excluded the D and R points from noise and A and B values
+            self.processEventNoiseFromIterativeSolution(D + 1, R - 1)
 
             # Try to warn user about the possible need for block integration by testing the lag 1
             # and lag 2 correlation coefficients.  The tests are just guesses on my part, so only
             # warnings are given.  Later, the Cholesky-Decomposition may fail because block integration
             # was really needed.  That is a fatal error but is trapped and the user alerted to the problem
 
             if len(self.corCoefs) > 1:
@@ -7808,29 +7762,19 @@
                             'This may be because the light curve needs some degree of block integration. '
                             'Failure to do a needed block integration allows point-to-point correlations caused by '
                             'the camera integration to artificially induce non-physical correlated noise.')
 
             if self.sigmaA is None:
                 self.sigmaA = self.sigmaB
         elif D:
-            self.sigmaA = None
-
             self.processBaselineNoiseFromIterativeSolution(self.left, D - 1)
-
-            self.processEventNoiseFromIterativeSolution(D, self.right)
-            if self.sigmaA is None:
-                self.sigmaA = self.sigmaB
+            self.processEventNoiseFromIterativeSolution(D+1, self.right)
         else:  # R only
-            self.sigmaA = None
-
-            self.processBaselineNoiseFromIterativeSolution(R, self.right)
-
+            self.processBaselineNoiseFromIterativeSolution(R+1, self.right)
             self.processEventNoiseFromIterativeSolution(self.left, R - 1)
-            if self.sigmaA is None:
-                self.sigmaA = self.sigmaB
 
         self.prettyPrintCorCoefs()
 
         return
 
     def try_to_get_solution(self):
         self.solution = None
@@ -8086,17 +8030,17 @@
             self.showMsg('Integer (non-subframe) solution...', blankLine=False)
             self.showMsg(
                 'sigB:%.2f  sigA:%.2f B:%.2f A:%.2f' %
                 (sigmaB, sigmaA, b, a),
                 blankLine=False)
             self.displaySolution(subframe=False)  # First solution
 
-            # This fills in self.sigmaB and self.sigmaA (incorrectly) but is useful
+            # This fills in self.sigmaB and self.sigmaA and self.B and self.A Also, it is useful
             # because it tests correlation coefficients to warn of the need for block integration
-            self.extract_noise_parameters_from_iterative_solution()
+            self.extract_noise_parameters_from_iterative_solution()  # This does proper exclusions at D and R
 
             DfitMetric = RfitMetric = 0.0
 
             if not self.ne3NotInUseRadioButton.isChecked():
                 # We're being asked to perform an exponential edge fit for the Night Eagle 3 camera
                 snr = b / sigmaB
                 if snr < 4.0:
@@ -8107,15 +8051,15 @@
                 self.showUnderlyingLightcurveCheckBox.setChecked(True)
                 resultFound, DfitMetric, RfitMetric = self.doExpFit(b, a)
                 if not resultFound:
                     return
 
             # Here is where we get sigmaB and sigmaA with the transition points excluded
             subDandR, new_b, new_a, newSigmaB, newSigmaA = subFrameAdjusted(
-                eventType=self.eventType, cand=(d, r), B=b, A=a,
+                eventType=self.eventType, cand=(d, r), B=self.B, A=self.A,
                 sigmaB=self.sigmaB, sigmaA=self.sigmaA, yValues=self.yValues,
                 left=self.left, right=self.right)
 
             if not self.ne3NotInUseRadioButton.isChecked():
                 if not self.dnrOffRadioButton.isChecked():
                     subDandR = self.solution
 
@@ -8940,26 +8884,26 @@
         self.showMsg('Event noise analysis done using ' + str(self.numNApts) +
                      ' points ---  sigmaA: ' + fp.to_precision(self.sigmaA, 4))
 
         self.newRedrawMainPlot()
 
     def processEventNoiseFromIterativeSolution(self, left, right):
 
-        if (right - left) < 9:
-            return
-
         assert left >= self.left
         assert right <= self.right
 
         self.eventXvals = []
         self.eventYvals = []
         for i in range(left, right + 1):
             self.eventXvals.append(i)
             self.eventYvals.append(self.yValues[i])
 
+        # Recalculate A with D and R points excluded
+        self.A = np.mean(self.eventYvals)
+
         _, self.numNApts, self.sigmaA = getCorCoefs(self.eventXvals,
                                                     self.eventYvals)
 
     def processBaselineNoise(self, secondPass=False):
 
         if len(self.selectedPoints) != 2:
             self.showInfo('Exactly two points must be selected for this operation')
@@ -9045,14 +8989,17 @@
 
         self.baselineXvals = []
         self.baselineYvals = []
         for i in range(left, right + 1):
             self.baselineXvals.append(i)
             self.baselineYvals.append(self.yValues[i])
 
+        # Recalculate baseline with D and R points excluded
+        self.B = np.mean(self.baselineYvals)
+
         if not self.userDeterminedBaselineStats:
             self.newCorCoefs, self.numNApts, sigB = getCorCoefs(self.baselineXvals,
                                                                 self.baselineYvals)
 
             if len(self.corCoefs) == 0:
                 self.corCoefs = np.ndarray(shape=(len(self.newCorCoefs),))
                 np.copyto(self.corCoefs, self.newCorCoefs)
```

### Comparing `pyote-5.2.2/src/pyoteapp/pyote_modelling_utility_functions.py` & `pyote-5.2.3/src/pyoteapp/pyote_modelling_utility_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1853,30 +1853,30 @@
             if n_sample_points > 1:
                 sample = np.repeat(1.0 / n_sample_points, n_sample_points)
                 camera_y = lightcurve_convolve(sample=sample, lightcurve=y,
                                                shift_needed=len(sample) - 1)
             else:
                 camera_y = y
 
-        # TODO Experimental - used to provide model light curves for test file generator
+        # TODO This is used to provide model light curves for test file generator and must be left in.
         model_dict = {'y': camera_y, 't_start': x[0] / LCP.shadow_speed, 't_end': x[-1] / LCP.shadow_speed}
         pickle.dump(model_dict, open("model_dict_diffraction.p", "wb"))
         # print(f'x[0]: {x[0]/LCP.shadow_speed:0.4f}  x[-1]: {x[-1]/LCP.shadow_speed:0.4f}')
         return x, camera_y, D_edge, R_edge
     else:
         raise Exception(f"Model '{model}' is unknown.")
 
     # Restore the infinity-ducking fudged values
     if LCP.D_limb_angle_degrees == 89.999:
         LCP.set('D_limb_angle_degrees', 90)
     if LCP.R_limb_angle_degrees == 89.999:
         LCP.set('R_limb_angle_degrees', 90)
 
     final_y = cameraIntegration(x, y, LCP)
-    # TODO Experimental - used to provide model light curves for test file generator
+    # TODO This is used to provide model light curves for test file generator and must be left in.
     model_dict = {'y': final_y, 't_start': x[0]/LCP.shadow_speed, 't_end':x[-1]/LCP.shadow_speed}
     pickle.dump(model_dict, open("model_dict_diffraction.p", "wb"))
     # print(f'x[0]: {x[0]/LCP.shadow_speed:0.4f}  x[-1]: {x[-1]/LCP.shadow_speed:0.4f}')
 
     return x, final_y, D_edge, R_edge
```

### Comparing `pyote-5.2.2/src/pyoteapp/showVideoFrames.py` & `pyote-5.2.3/src/pyoteapp/showVideoFrames.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/solverUtils.py` & `pyote-5.2.3/src/pyoteapp/solverUtils.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,27 +11,35 @@
 import numpy as np
 from pyoteapp.likelihood_calculations import cum_loglikelihood, aicc, logLikelihoodLine
 from pyoteapp.likelihood_calculations import loglikelihood
 from numba import njit
 
 
 def aicModelValue(*, obsValue=None, B=None, A=None, sigmaB=None, sigmaA=None):
-    assert(B >= A)
-    assert(sigmaA > 0.0)
-    assert(sigmaB > 0.0)
+    assert B >= A
+    # assert sigmaA > 0.0
+    # assert sigmaB > 0.0
+
     # This function determines if an observation point should categorized as a baseline (B)
     # point, an event (A) point, or a valid intermediate point using the Akaike Information Criterion
     # An intermediate point reflects a more complex model (higher dimension model)
     if obsValue >= B:
         return B  # Categorize as baseline point
     if obsValue <= A:
         return A  # Categorize as event point
     if B == A:
         return B
 
+    # We do this to allow test files with zero noise to be processed
+    if sigmaA == 0:
+        if sigmaB == 0:
+            return obsValue
+        else:
+            assert sigmaA > 0.0
+
     sigmaM = sigmaA + (sigmaB - sigmaA) * ((obsValue - A) / (B - A))
     loglB = loglikelihood(obsValue, B, sigmaB)
     loglM = loglikelihood(B, B, sigmaM) - 1.0  # The -1 is the aic model complexity 'penalty'
     loglA = loglikelihood(obsValue, A, sigmaA)
 
     if loglM > loglA and loglM > loglB:
         return obsValue  # Categorize as valid intermediate value
@@ -247,18 +255,20 @@
         # as the best estimate of B
         if R == right:
             B = yValues[R]
             sigmaB = 0.0
         else:
             # changed in 4.4.7
             # B = np.mean(yValues[R+1:right+1])
-            valuesToUse = [val for i, val in enumerate(yValues[R:right + 1]) if i not in tpList]
+            # Changed i to i + R in 5.2.3 to solve flash edge time problem
+            valuesToUse = [val for i, val in enumerate(yValues[R:right + 1]) if i + R not in tpList]
             B = np.mean(valuesToUse)
             sigmaB = np.std(valuesToUse)
-        valuesToUse = valuesToBeUsed(left, R)
+        # Changed to R - 1 in 5.2.3 to solve flash edge time problem
+        valuesToUse = valuesToBeUsed(left, R - 1)
         A = np.mean(valuesToUse)
         sigmaA = np.std(valuesToUse)
         if A >= B:
             A = B * 0.999
         return B, A, sigmaB, sigmaA
 
     else:
@@ -448,19 +458,14 @@
 
     # Here we add code so we can analyze light curves that may have sigmaB or
     #  sigmaA values of zero.  This happens when testing with artificial data
     #  but can also result from real light curves that may be clipped so that
     #  all B pixels have a constant value.  Limovie can produce a sigmaA=0
     # when a rectangular aperture is in use as well
 
-    if sigmaA == 0.0:
-        sigmaA = MIN_SIGMA
-    if sigmaB == 0.0:
-        sigmaB = MIN_SIGMA
-
     if eventType == 'Donly':
         if aicModelValue(obsValue=yValues[D], B=B, A=A, sigmaB=sigmaB, sigmaA=sigmaA) == yValues[D]:
             # If point at D categorizes as M (valid mid-point), do sub-frame
             # adjustment and exit
             adjD = adjustD()
             transitionPoints.append(D)
             B, A, sigmaB, sigmaA = newCalcBandA(yValues=yValues, tpList=transitionPoints,
@@ -520,70 +525,56 @@
             return [D, R], B, A, sigmaB, sigmaA
         if aicModelValue(
                 obsValue=yValues[D], B=B, A=A, sigmaB=sigmaB, sigmaA=sigmaA) == yValues[D]:
             # The point at D categorizes as M, do sub-frame adjustment; this
             # (finishes D)
             adjD = adjustD()
             transitionPoints.append(D)
-            B, A, sigmaB, sigmaA = newCalcBandA(yValues=yValues, tpList=transitionPoints,
-                                                left=left, right=right, cand=(D, R))
         elif aicModelValue(obsValue=yValues[D], B=B, A=A, sigmaB=sigmaB, sigmaA=sigmaA) == B:
             # The point at D categorizes as B, set D to D+1 and recalculate B and A
             D = D + 1
             adjD = D
             # It's possible that this new point qualifies as M --- so we check
             if aicModelValue(
                     obsValue=yValues[D], B=B, A=A, sigmaB=sigmaB,
                     sigmaA=sigmaA) == yValues[D]:
                 adjD = adjustD()
                 transitionPoints.append(D)
-                B, A, sigmaB, sigmaA = newCalcBandA(yValues=yValues, tpList=transitionPoints,
-                                                    left=left, right=right, cand=(D, R))
         elif aicModelValue(obsValue=yValues[D-1], B=B, A=A, sigmaB=sigmaB,
                            sigmaA=sigmaA) == yValues[D-1]:
             # The point at D categorizes as A, and we have found
             # that the point at D-1 categorizes as M, so set D to D-1 and
             # recalculate B and A
             D = D - 1
             adjD = adjustD()
             transitionPoints.append(D)
-            B, A, sigmaB, sigmaA = newCalcBandA(yValues=yValues, tpList=transitionPoints,
-                                                left=left, right=right, cand=(D, R))
 
         if aicModelValue(
                 obsValue=yValues[R], B=B, A=A, sigmaB=sigmaB, sigmaA=sigmaA) == yValues[R]:
             # The point at R categorizes as M, do sub-frame adjustment
             adjR = adjustR()
             transitionPoints.append(R)
-            B, A, sigmaB, sigmaA = newCalcBandA(yValues=yValues, tpList=transitionPoints,
-                                                left=left, right=right, cand=(D, R))
         elif aicModelValue(obsValue=yValues[R], B=B, A=A, sigmaB=sigmaB, sigmaA=sigmaA) == A:
             # The point at R categorizes as A, set R to R + 1 and recalculate B and A
             R = R + 1
             adjR = R
-            B, A, sigmaB, sigmaA = newCalcBandA(yValues=yValues, tpList=transitionPoints,
-                                                left=left, right=right, cand=(D, R))
             # It's possible that this new point qualifies as M --- so we check
             if aicModelValue(
                     obsValue=yValues[R], B=B, A=A, sigmaB=sigmaB,
                     sigmaA=sigmaA) == yValues[R]:
                 adjR = adjustR()
                 transitionPoints.append(R)
-                B, A, sigmaB, sigmaA = newCalcBandA(yValues=yValues, tpList=transitionPoints,
-                                                    left=left, right=right, cand=(D, R))
         elif aicModelValue(obsValue=yValues[R - 1], B=B, A=A, sigmaB=sigmaB,
                            sigmaA=sigmaA) == yValues[R - 1]:
             # The point at R categorizes as B, and we have found
             # that the point at R-1 categorizes as M, so set R to R-1 and
             # recalculate B and A
             R = R - 1
             adjR = adjustR()
             transitionPoints.append(R)
-            B, A, sigmaB, sigmaA = newCalcBandA(yValues=yValues, tpList=transitionPoints,
-                                                left=left, right=right, cand=(D, R))
         return [adjD, adjR], B, A, sigmaB, sigmaA
 
     else:
         raise Exception('Unrecognized event type')
 
 
 def solver(*, eventType=None, yValues=None,
```

### Comparing `pyote-5.2.2/src/pyoteapp/subframe_timing_utilities.py` & `pyote-5.2.3/src/pyoteapp/subframe_timing_utilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/timestampDialog.py` & `pyote-5.2.3/src/pyoteapp/timestampDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.2.2/src/pyoteapp/timestampUtils.py` & `pyote-5.2.3/src/pyoteapp/timestampUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,20 @@
 
 def improveTimeStep(outliers, deltaTime):
     validIntervals = [deltaTime[i] for i in range(len(deltaTime)) if i not in outliers]
     # Under some circumstances, OCR can be so bad that no valid intervals can
     # be found.  In that case, we return a timeStep of 0.0 and let the
     # program respond to this invalid value at a higher level.
     if validIntervals:
-        # Changed in 5.0.1
+        # Changed in 5.0.1  put back in 5.2.3
         # betterTimeStep = np.mean(validIntervals)
-        betterTimeStep = np.median(validIntervals)
+        # removed in 5.2.3
+        # betterTimeStep = np.median(validIntervals)
+        betterTimeStep = np.mean(validIntervals)
+
     else:
         betterTimeStep = 0.0
     return betterTimeStep
 
 
 def getTimeStepAndOutliers(timestamps, yValues, yStatus, VizieRdict=None):
```

