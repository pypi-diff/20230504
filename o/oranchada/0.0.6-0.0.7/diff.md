# Comparing `tmp/oranchada-0.0.6.tar.gz` & `tmp/oranchada-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oranchada-0.0.6.tar", last modified: Fri Apr  7 22:13:46 2023, max compression
+gzip compressed data, was "oranchada-0.0.7.tar", last modified: Thu May  4 12:48:05 2023, max compression
```

## Comparing `oranchada-0.0.6.tar` & `oranchada-0.0.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.340067 oranchada-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-07 22:13:35.000000 oranchada-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-07 22:13:35.000000 oranchada-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-07 22:13:46.340067 oranchada-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-07 22:13:35.000000 oranchada-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-07 22:13:35.000000 oranchada-0.0.6/README.pypi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/oranchada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 22:13:46.000000 oranchada-0.0.6/oranchada.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/orangecontrib/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/orangecontrib/oranchada/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/orangecontrib/oranchada/base_widget/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/arithmetic_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/base_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/creator_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/filter_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/base_widget/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.332067 oranchada-0.0.6/orangecontrib/oranchada/processings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/processings/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/processings/add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/processings/gen_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.336067 oranchada-0.0.6/orangecontrib/oranchada/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/tests/process_spectra_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.336067 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.336067 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/icons/spectra.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.340067 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/arithmetics_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/fit_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/gen_spe.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/hht_sharpening.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:13:46.340067 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/icons/spectra.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_file_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_test_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/moving_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/process_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/remove_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/set_xaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-07 22:13:35.000000 oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 22:13:46.340067 oranchada-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-07 22:13:35.000000 oranchada-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.424214 oranchada-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-04 12:47:53.000000 oranchada-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 12:47:53.000000 oranchada-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 12:48:05.420214 oranchada-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-04 12:47:53.000000 oranchada-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-04 12:47:53.000000 oranchada-0.0.7/README.pypi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.408214 oranchada-0.0.7/oranchada.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 12:48:05.000000 oranchada-0.0.7/oranchada.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.408214 oranchada-0.0.7/orangecontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.408214 oranchada-0.0.7/orangecontrib/oranchada/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.412214 oranchada-0.0.7/orangecontrib/oranchada/base_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/arithmetic_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/creator_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/filter_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/base_widget/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.412214 oranchada-0.0.7/orangecontrib/oranchada/processings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/processings/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/processings/add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/processings/gen_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.412214 oranchada-0.0.7/orangecontrib/oranchada/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/tests/process_spectra_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.416214 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.416214 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/icons/spectra.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.420214 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/arithmetics_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/fit_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/gen_spe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/hht_sharpening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:48:05.420214 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/icons/spectra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_file_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_test_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/moving_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/process_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/remove_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/set_xaxis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-04 12:47:53.000000 oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:48:05.424214 oranchada-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-04 12:47:53.000000 oranchada-0.0.7/setup.py
```

### Comparing `oranchada-0.0.6/LICENSE` & `oranchada-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/PKG-INFO` & `oranchada-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oranchada
-Version: 0.0.6
+Version: 0.0.7
 Summary: Orange add-on for Raman spectroscopy
 Home-page: https://github.com/h2020charisma/oranchada
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,oranchada,orange3 add-on,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oranchada-0.0.6/README.md` & `oranchada-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/oranchada.egg-info/PKG-INFO` & `oranchada-0.0.7/oranchada.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oranchada
-Version: 0.0.6
+Version: 0.0.7
 Summary: Orange add-on for Raman spectroscopy
 Home-page: https://github.com/h2020charisma/oranchada
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,oranchada,orange3 add-on,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oranchada-0.0.6/oranchada.egg-info/SOURCES.txt` & `oranchada-0.0.7/oranchada.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/base_widget/base_widget.py` & `oranchada-0.0.7/orangecontrib/oranchada/base_widget/base_widget.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/base_widget/filter_widget.py` & `oranchada-0.0.7/orangecontrib/oranchada/base_widget/filter_widget.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/processings/add_baseline.py` & `oranchada-0.0.7/orangecontrib/oranchada/processings/add_baseline.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/processings/add_noise.py` & `oranchada-0.0.7/orangecontrib/oranchada/processings/add_noise.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/processings/gen_spe.py` & `oranchada-0.0.7/orangecontrib/oranchada/processings/gen_spe.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/tests/process_spectra_test.py` & `oranchada-0.0.7/orangecontrib/oranchada/tests/process_spectra_test.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_easy/icons/spectra.svg` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_easy/icons/spectra.svg`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/add_baseline.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/add_baseline.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/add_noise.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/add_noise.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/arithmetics_add.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/arithmetics_add.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/find_peaks.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/find_peaks.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/fit_peaks.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/fit_peaks.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,21 @@
         self.out_spe = list()
         for spe in self.in_spe:
             self.out_spe.append(
                 spe.fit_peaks_filter(profile=self.peak_profile, no_fit=not self.should_fit,
                                      vary_baseline=self.vary_baseline)
             )
         self.send_outputs()
-        dfs = [FitPeaksResult.loads(spe.result).to_dataframe_peaks() for spe in self.out_spe]
+        dfs = []
+        for spe in self.out_spe:
+            df = FitPeaksResult.loads(spe.result).to_dataframe_peaks()
+            fn = pd.Series([spe.meta['Original file']]*len(df))
+            fn.index = df.index
+            df['filename'] = fn
+            dfs.append(df)
         self.Outputs.peaks_out.send(table_from_frame(pd.concat(dfs)))
 
     def custom_plot(self, ax):
         if self.plot_individual_peaks:
             peaks_ax = ax.twinx()
         else:
             peaks_ax = ax
```

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/gen_spe.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/gen_spe.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/hht_sharpening.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/hht_sharpening.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/icons/spectra.svg` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/icons/spectra.svg`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_file.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_file.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_file_names.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_file_names.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/load_test_spectra.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/load_test_spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,11 +52,11 @@
 
     def select_filename(self):
         self.selected_filenames = [fn_item.text() for fn_item in self.list_box_filename.selectedItems()]
         self.auto_process()
 
     def process(self):
         self.out_spe = list()
-        for fn in self.selected_filenames:
+        for fn in data.prepend_prefix(self.selected_filenames):
             spe = rc2.spectrum.from_local_file(fn)
             self.out_spe.append(spe)
         self.send_outputs()
```

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/merger.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/merger.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/moving_minimum.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/moving_minimum.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/normalize.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/normalize.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/process_spectra.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/process_spectra.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/remove_spikes.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/remove_spikes.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/select.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/select.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/set_xaxis.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/set_xaxis.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.6/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py` & `oranchada-0.0.7/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         gui.doubleSpin(box, self, 'prominence', 0, 50000, decimals=2, step=1, callback=self.auto_process,
                        label='Prominence [×σ]')
         gui.spin(box, self, 'wlen', 0, 50000, step=1, callback=self.auto_process, label='wlen')
 
         gui.checkBox(box, self, "should_fit", "Should fit", callback=self.auto_process)
 
         gui.comboBox(box, self, 'poly_order', sendSelectedValue=True,
-                     items=['poly0', 'poly1', 'poly2', 'poly3', 'poly4'],
+                     items=['poly0', 'poly1', 'poly2', 'poly3', 'poly4', 'RBF thin-plate-spline'],
                      callback=self.auto_process
                      )
 
         self.combo = gui.comboBox(box, self, 'predefined_deltas', sendSelectedValue=True,
                                   items=[
                                       'Ne RS 532nm', 'Ne RS 633nm', 'Ne RS 785nm',
                                       'Ne WL 532nm', 'Ne WL 633nm', 'Ne WL 785nm',
@@ -84,28 +84,35 @@
             poly_order_num = 4
 
         self.out_spe = list()
         if len(self.in_spe) > 1:
             raise ValueError(f'Expects a single spectrum input. {len(self.in_spe)} found')
         for spe in self.in_spe:
             for iter in range(self.n_iters):
-                spe = spe.xcal_fine(ref=self.deltas_dict, poly_order=poly_order_num, should_fit=self.should_fit,
-                                    find_peaks_kw=dict(prominence=spe.y_noise*self.prominence, wlen=self.wlen))
+                if self.poly_order == 'RBF thin-plate-spline':
+                    spe = spe.xcal_fine_RBF(ref=self.deltas_dict, should_fit=self.should_fit,
+                                            find_peaks_kw=dict(prominence=spe.y_noise*self.prominence, wlen=self.wlen)
+                                            )
+                else:
+                    spe = spe.xcal_fine(ref=self.deltas_dict, poly_order=poly_order_num, should_fit=self.should_fit,
+                                        find_peaks_kw=dict(prominence=spe.y_noise*self.prominence, wlen=self.wlen))
             self.out_spe.append(spe)
         self.send_outputs()
 
     def custom_plot(self, ax):
         if not self.in_spe:
             return
         self.in_spe[0].plot(ax=self.axes[0])
         self.axes[0].twinx().stem(list(self.deltas_dict.keys()), list(self.deltas_dict.values()),
                                   basefmt='', linefmt='r:', label='reference')
-        self.axes[1].twinx().stem(list(self.deltas_dict.keys()), list(self.deltas_dict.values()),
-                                  basefmt='', linefmt='r:', label='reference')
-        x, y, yerr = self.diff(self.out_spe[0], self.deltas_dict)
+        ax1_twin = self.axes[1].twinx()
+        ax1_twin.stem(list(self.deltas_dict.keys()), list(self.deltas_dict.values()),
+                      basefmt='', linefmt='r:', label='reference')
+        x, x_exp, y, yerr = self.diff(self.out_spe[0], self.deltas_dict)
+        ax1_twin.plot([x, x_exp], [0, 0], 'r', lw=4)
         self.axes[2].errorbar(x, y, yerr, fmt='.:', label='difference')
         for a in self.axes:
             a.grid()
             a.legend()
         y_ub = y + yerr
         y_lb = y - yerr
         y_ub = np.mean(y_ub) + np.std(y_ub)*3
@@ -135,8 +142,8 @@
         else:
             spe_pos = np.array(list(cand.get_pos_ampl_dict().keys()))
             spe_pos_err = np.zeros_like(spe_pos)
 
         spe_pos_match_idx, ref_pos_match_idx = rc2utils.find_closest_pairs_idx(spe_pos, ref_pos)
         spe_pos_match = spe_pos[spe_pos_match_idx]
         ref_pos_match = ref_pos[ref_pos_match_idx]
-        return ref_pos_match, (spe_pos_match-ref_pos_match), spe_pos_err[spe_pos_match_idx]
+        return ref_pos_match, spe_pos_match, (spe_pos_match-ref_pos_match), spe_pos_err[spe_pos_match_idx]
```

### Comparing `oranchada-0.0.6/setup.py` & `oranchada-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from os import path, walk
 
 from setuptools import find_packages, setup
 
 NAME = 'oranchada'
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 DESCRIPTION = 'Orange add-on for Raman spectroscopy'
 README_FILE = path.join(path.dirname(__file__), 'README.pypi')
 LONG_DESCRIPTION = open(README_FILE, 'r', encoding='utf-8').read()
 LONG_DESCRIPTION_CONTENT_TYPE = 'text/markdown'
 URL = 'https://github.com/h2020charisma/oranchada'
 AUTHOR = 'IDEAconsult Ltd.'
@@ -38,15 +38,15 @@
 
 INSTALL_REQUIRES = [
     'Orange3>=3.31.0',
     'numpy>=1.18.0',
     'orange-canvas-core>=0.1.24',
     'orange-widget-base>=4.16.1',
     'pip>=9.0',  # same as for Orange 3.28
-    'ramanchada2~=0.0.4',
+    'ramanchada2~=0.0.5',
     'setuptools>=36.3',  # same as for Orange 3.28
     # 'AnyQt>=0.0.6',
     # 'bottleneck',
     # 'colorcet',
     # 'extranormal3 >=0.0.3',
     # 'h5py',
     # 'lmfit>=1.0.2',
```

