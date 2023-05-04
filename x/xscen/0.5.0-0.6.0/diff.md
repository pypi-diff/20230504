# Comparing `tmp/xscen-0.5.0.tar.gz` & `tmp/xscen-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xscen-0.5.0.tar", last modified: Tue Feb 28 21:18:25 2023, max compression
+gzip compressed data, was "xscen-0.6.0.tar", last modified: Thu May  4 21:12:29 2023, max compression
```

## Comparing `xscen-0.5.0.tar` & `xscen-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 21:18:25.640768 xscen-0.5.0/
--rw-r--r--   0 tjs       (1000) tjs       (1000)      765 2023-01-31 16:46:08.000000 xscen-0.5.0/AUTHORS.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)     5351 2022-08-11 22:30:42.000000 xscen-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)    11790 2023-02-28 21:08:59.000000 xscen-0.5.0/HISTORY.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)    11357 2022-07-28 20:50:19.000000 xscen-0.5.0/LICENSE
--rw-r--r--   0 tjs       (1000) tjs       (1000)      794 2022-12-22 16:54:39.000000 xscen-0.5.0/MANIFEST.in
--rw-r--r--   0 tjs       (1000) tjs       (1000)    20442 2023-02-28 21:18:25.640768 xscen-0.5.0/PKG-INFO
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1920 2022-12-22 16:54:39.000000 xscen-0.5.0/README.rst
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1379 2023-02-28 21:18:25.641768 xscen-0.5.0/setup.cfg
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2661 2023-02-28 21:12:22.000000 xscen-0.5.0/setup.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 21:18:25.622768 xscen-0.5.0/tests/
--rw-r--r--   0 tjs       (1000) tjs       (1000)       35 2022-07-28 20:50:19.000000 xscen-0.5.0/tests/__init__.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)      542 2022-12-22 16:54:39.000000 xscen-0.5.0/tests/conftest.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)      425 2022-08-11 22:30:42.000000 xscen-0.5.0/tests/test_xscen.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 21:18:25.629768 xscen-0.5.0/xscen/
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 21:18:25.633768 xscen-0.5.0/xscen/CVs/
--rw-r--r--   0 tjs       (1000) tjs       (1000)      175 2022-11-25 21:21:49.000000 xscen-0.5.0/xscen/CVs/frequency_to_timedelta.json
--rw-r--r--   0 tjs       (1000) tjs       (1000)      174 2022-11-25 21:21:49.000000 xscen-0.5.0/xscen/CVs/frequency_to_xrfreq.json
--rw-r--r--   0 tjs       (1000) tjs       (1000)      175 2022-07-28 20:50:19.000000 xscen-0.5.0/xscen/CVs/infer_resolution.json
--rw-r--r--   0 tjs       (1000) tjs       (1000)      194 2022-09-07 21:51:27.000000 xscen-0.5.0/xscen/CVs/resampling_methods.json
--rw-r--r--   0 tjs       (1000) tjs       (1000)      125 2022-07-28 20:50:19.000000 xscen-0.5.0/xscen/CVs/variable_names.json
--rw-r--r--   0 tjs       (1000) tjs       (1000)      221 2022-11-25 21:21:49.000000 xscen-0.5.0/xscen/CVs/xrfreq_to_frequency.json
--rw-r--r--   0 tjs       (1000) tjs       (1000)      203 2022-11-25 21:21:49.000000 xscen-0.5.0/xscen/CVs/xrfreq_to_timedelta.json
--rw-r--r--   0 tjs       (1000) tjs       (1000)     1369 2023-02-28 21:12:22.000000 xscen-0.5.0/xscen/__init__.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    22964 2023-02-28 19:53:29.000000 xscen-0.5.0/xscen/aggregate.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    10957 2022-12-22 16:54:39.000000 xscen-0.5.0/xscen/biasadjust.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    56347 2023-02-24 21:54:13.000000 xscen-0.5.0/xscen/catalog.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)     8027 2023-02-24 21:54:13.000000 xscen-0.5.0/xscen/config.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 21:18:25.633768 xscen-0.5.0/xscen/data/
--rw-r--r--   0 tjs       (1000) tjs       (1000)  1085105 2022-11-11 19:15:19.000000 xscen-0.5.0/xscen/data/IPCC_annual_global_tas.csv
--rw-r--r--   0 tjs       (1000) tjs       (1000)    12535 2022-12-22 16:54:39.000000 xscen-0.5.0/xscen/diagnostics.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)     9026 2023-02-24 21:54:13.000000 xscen-0.5.0/xscen/ensembles.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    54801 2023-02-24 21:54:13.000000 xscen-0.5.0/xscen/extract.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)     8126 2023-02-24 21:54:13.000000 xscen-0.5.0/xscen/indicators.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    18622 2022-12-22 16:54:39.000000 xscen-0.5.0/xscen/io.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)     4921 2022-12-22 16:54:39.000000 xscen-0.5.0/xscen/reduce.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    11601 2023-02-28 19:53:32.000000 xscen-0.5.0/xscen/regrid.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    10981 2022-12-22 16:54:39.000000 xscen-0.5.0/xscen/scripting.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)    34962 2023-02-24 21:54:13.000000 xscen-0.5.0/xscen/utils.py
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 21:18:25.639768 xscen-0.5.0/xscen/xclim_modules/
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2742 2022-12-22 16:54:39.000000 xscen-0.5.0/xscen/xclim_modules/conversions.py
--rw-r--r--   0 tjs       (1000) tjs       (1000)     2194 2022-11-11 19:15:19.000000 xscen-0.5.0/xscen/xclim_modules/conversions.yml
-drwxr-xr-x   0 tjs       (1000) tjs       (1000)        0 2023-02-28 21:18:25.631768 xscen-0.5.0/xscen.egg-info/
--rw-r--r--   0 tjs       (1000) tjs       (1000)    20442 2023-02-28 21:18:25.000000 xscen-0.5.0/xscen.egg-info/PKG-INFO
--rw-r--r--   0 tjs       (1000) tjs       (1000)      911 2023-02-28 21:18:25.000000 xscen-0.5.0/xscen.egg-info/SOURCES.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)        1 2023-02-28 21:18:25.000000 xscen-0.5.0/xscen.egg-info/dependency_links.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)        1 2022-08-04 14:19:29.000000 xscen-0.5.0/xscen.egg-info/not-zip-safe
--rw-r--r--   0 tjs       (1000) tjs       (1000)      180 2023-02-28 21:18:25.000000 xscen-0.5.0/xscen.egg-info/requires.txt
--rw-r--r--   0 tjs       (1000) tjs       (1000)        6 2023-02-28 21:18:25.000000 xscen-0.5.0/xscen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:29.570920 xscen-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-04 21:12:24.000000 xscen-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-04 21:12:24.000000 xscen-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16989 2023-05-04 21:12:24.000000 xscen-0.6.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 21:12:24.000000 xscen-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 21:12:24.000000 xscen-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29278 2023-05-04 21:12:29.570920 xscen-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-04 21:12:24.000000 xscen-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-04 21:12:29.570920 xscen-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-04 21:12:24.000000 xscen-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:29.566920 xscen-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 21:12:24.000000 xscen-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-04 21:12:24.000000 xscen-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-04 21:12:24.000000 xscen-0.6.0/tests/test_xscen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:29.566920 xscen-0.6.0/xscen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:29.566920 xscen-0.6.0/xscen/CVs/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/CVs/frequency_to_timedelta.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/CVs/frequency_to_xrfreq.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/CVs/infer_resolution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/CVs/resampling_methods.json
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/CVs/variable_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/CVs/xrfreq_to_frequency.json
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/CVs/xrfreq_to_timedelta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28823 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/biasadjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61143 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:29.566920 xscen-0.6.0/xscen/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1085105 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/data/IPCC_annual_global_tas.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52724 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18622 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36840 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:29.570920 xscen-0.6.0/xscen/xclim_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/xclim_modules/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-04 21:12:24.000000 xscen-0.6.0/xscen/xclim_modules/conversions.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:29.566920 xscen-0.6.0/xscen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29278 2023-05-04 21:12:29.000000 xscen-0.6.0/xscen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-04 21:12:29.000000 xscen-0.6.0/xscen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:12:29.000000 xscen-0.6.0/xscen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:12:29.000000 xscen-0.6.0/xscen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 21:12:29.000000 xscen-0.6.0/xscen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 21:12:29.000000 xscen-0.6.0/xscen.egg-info/top_level.txt
```

### Comparing `xscen-0.5.0/AUTHORS.rst` & `xscen-0.6.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/CONTRIBUTING.rst` & `xscen-0.6.0/CONTRIBUTING.rst`

 * *Files 3% similar despite different names*

```diff
@@ -140,26 +140,28 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 3.8, 3.9, and 3.10.
+3. The pull request should not break the templates.
+4. The pull request should work for Python 3.8, 3.9, and 3.10.
 
 Tips
 ----
 
 To run a subset of tests::
 
 $ pytest tests.test_xscen
 
 Versioning/Tagging
 ------------------
 
 A reminder for the maintainers on how to deploy.
 Make sure all your changes are committed (including an entry in HISTORY.rst).
+The templates must also be tested manually before each release.
 Then run::
 
 $ bumpversion patch # possible: major / minor / patch
 $ git push
 $ git push --tags
```

### Comparing `xscen-0.5.0/HISTORY.rst` & `xscen-0.6.0/HISTORY.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,72 @@
 =======
 History
 =======
 
+v0.6.0 (2023-05-04)
+-------------------
+Contributors to this version: Trevor James Smith (:user:`Zeitsperre`), Juliette Lavoie (:user:`juliettelavoie`), Pascal Bourgault (:user:`aulemahal`), Gabriel Rondeau-Genesse (:user:`RondeauG`).
+
+Announcements
+^^^^^^^^^^^^^
+* `xscen` is now offered as a conda package available through Anaconda.org. Refer to the installation documentation for more information. (:issue:`149`, :pull:`171`).
+* Deprecation: Release 0.6.0 of `xscen` will be the last version to support ``xscen.extract.clisops_subset``. Use ``xscen.spatial.subset`` instead. (:pull:`182`, :pull:`184`).
+* Deprecation: The argument `region`, used in multiple functions, has been slightly reformatted. Release 0.6.0 of `xscen` will be the last version to support the old format. (:issue:`99`, :issue:`101`, :pull:`184`).
+
+New features and enhancements
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+* New 'cos-lat' averaging in `spatial_mean`. (:issue:`94`, :pull:`125`).
+* Support for computing anomalies in `compute_deltas`.  (:pull:`165`).
+* Add function `diagnostics.measures_improvement_2d`. (:pull:`167`).
+* Add function ``regrid.create_bounds_rotated_pole`` and automatic use in ``regrid_dataset`` and ``spatial_mean``. This is temporary, while we wait for a functionning method in ``cf_xarray``. (:pull:`174`, :issue:`96`).
+* Add ``spatial`` submodule with functions ``creep_weights`` and ``creep_fill`` for filling NaNs using neighbours. (:pull:`174`).
+* Allow passing ``GeoDataFrame`` instances in ``spatial_mean``'s ``region`` argument, not only geospatial file paths. (:pull:`174`).
+* Allow searching for periods in `catalog.search`. (:issue:`123`, :pull:`170`).
+* Allow searching and extracting multiple frequencies for a given variable. (:issue:`168`, :pull:`170`).
+* New masking feature in ``extract_dataset``. (:issue:`180`, :pull:`182`).
+* New function ``xs.spatial.subset`` to replace ``xs.extract.clisops_subset`` and add method "sel". (:issue:`180`, :pull:`182`).
+* Add long_name attribute to diagnostics. ( :pull:`189`).
+* Added a new YAML-centric notebook (:issue:`8`, :pull:`191`).
+* New ``utils.standardize_periods`` to standardize that argument across multiple functions. (:issue:`87`, :pull:`192`).
+* New `coverage_kwargs` argument added to ``search_data_catalogs`` to allow modifying the default values of ``subset_file_coverage``. (:issue:`87`, :pull:`192`).
+
+Breaking changes
+^^^^^^^^^^^^^^^^
+* 'mean' averaging has been deprecated in `spatial_mean`. (:pull:`125`).
+* 'interp_coord' has been renamed to 'interp_centroid' in `spatial_mean`. (:pull:`125`).
+* The 'datasets' dimension of the output of ``diagnostics.measures_heatmap`` is renamed 'realization'. (:pull:`167`).
+* `_subset_file_coverage` was renamed `subset_file_coverage` and moved to ``catalog.py`` to prevent circular imports. (:pull:`170`).
+* `extract_dataset` doesn't fail when a variable is in the dataset, but not `variables_and_freqs`. (:pull:`185`).
+* The argument `period`, used in multiple function, is now always a single list, while `periods` is more flexible. (:issue:`87`, :pull:`192`).
+* The parameters `reference_period` and `simulation_period` of ``xscen.train`` and ``xscen.adjust`` were renamed `period/periods` to respect the point above. (:issue:`87`, :pull:`192`).
+
+Bug fixes
+^^^^^^^^^
+* Forbid pandas v1.5.3 in the environment files, as the linux conda build breaks the data catalog parser. (:issue:`161`, :pull:`162`).
+* Only return requested variables when using ``DataCatalog.to_dataset``. (:pull:`163`).
+* ``compute_indicators`` no longer crashes if less than 3 timesteps are produced. (:pull:`125`).
+* `xarray` is temporarily pinned below v2023.3.0 due to an API-breaking change. (:issue:`175`, :pull:`173`).
+* `xscen.utils.unstack_fill_nan`` can now handle datasets that have non dimension coordinates. (:issue:`156`, :pull:`175`).
+* `extract_dataset` now skips a simulation way earlier if the frequency doesn't match. (:pull:`170`).
+* `extract_dataset` now correctly tries to extract in reverse timedelta order. (:pull:`170`).
+* `compute_deltas` no longer creates all NaN values if the input dataset is in a non-standard calendar. (:pull:`188`).
+
+Internal changes
+^^^^^^^^^^^^^^^^
+* `xscen` now manages packaging for PyPi and TestPyPI via GitHub workflows. (:pull:`159`).
+* Pre-load coordinates in ``extract.clisops_subset`` (:pull:`163`).
+* Minimal documentation for templates. (:pull:`163`).
+* `xscen` is now indexed in `Zenodo <https://zenodo.org/>`_, under the `ouranos` community of projects. (:pull:`164`).
+* Added a few relevant `Shields <https://shields.io/>`_ to the README.rst. (:pull:`164`).
+* Better warning messages in ``_subset_file_coverage`` when coverage is insufficient. (:pull:`125`).
+* The top-level Makefile now includes a `linkcheck` recipe, and the ReadTheDocs configuration no longer reinstalls the `llvmlite` compiler library. (:pull:`173`).
+* The checkups on coverage and duplicates can now be skipped in `subset_file_coverage`. (:pull:`170`).
+* Changed the `ProjectCatalog` docstrings to make it more obvious that it needs to be created empty. (:issue:`99`, :pull:`184`).
+* Added parse_config to `creep_fill`, `creep_weights`, and `reduce_ensemble` (:pull:`191`).
+
 v0.5.0 (2023-02-28)
 -------------------
 Contributors to this version: Gabriel Rondeau-Genesse (:user:`RondeauG`), Juliette Lavoie (:user:`juliettelavoie`), Trevor James Smith (:user:`Zeitsperre`), Sarah Gammon (:user:`sg2475962`) and Pascal Bourgault (:user:`aulemahal`).
 
 New features and enhancements
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 * Possibility of excluding variables read from file from the catalog produced by ``parse_directory``. (:pull:`107`).
@@ -45,15 +106,15 @@
 * ``compute_deltas`` skips the unstacking step if there is no time dimension and cast object dimensions to string. (:pull:`9`)
 * Added the "2sem" frequency to the translations CVs. (:pull:`111`).
 * Skip files we can't read in ``parse_directory``. (:pull:`111`).
 * Fixed non-numpy-standard Docstrings. (:pull:`108`).
 * Added more metadata to package description on PyPI. (:pull:`108`).
 * Faster ``search_data_catalogs`` and ``extract_dataset`` through a faster ``DataCatalog.unique``, date parsing and a rewrite of the ``ensure_correct_time`` logic. (:pull:`127`).
 * The ``search_data_catalogs`` function now accepts `str` or `pathlib.Path` variables (in addition to lists of either data type) for performing catalog lookups. (:pull:`121`).
-* `produce_horizons` now supports fixed fields (pull:`139`).
+* `produce_horizons` now supports fixed fields (:pull:`139`).
 * Rewrite of ``unstack_dates`` for better performance with dask arrays. (:pull:`144`).
 
 v0.4.0 (2022-09-28)
 -------------------
 Contributors to this version: Gabriel Rondeau-Genesse (:user:`RondeauG`), Juliette Lavoie (:user:`juliettelavoie`), Trevor James Smith (:user:`Zeitsperre`) and Pascal Bourgault (:user:`aulemahal`).
 
 New features and enhancements
```

### Comparing `xscen-0.5.0/LICENSE` & `xscen-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/MANIFEST.in` & `xscen-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/PKG-INFO` & `xscen-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: xscen
-Version: 0.5.0
+Version: 0.6.0
 Summary: A climate change scenario-building analysis framework, built with xclim/xarray.
 Home-page: https://github.com/Ouranosinc/xscen
 Author: Gabriel Rondeau-Genesse
 Author-email: rondeau-genesse.gabriel@ouranos.ca
-License: UNKNOWN
 Project-URL: About Ouranos, https://www.ouranos.ca/en/
 Project-URL: Changelog, https://xscen.readthedocs.io/en/stable/history.html
 Project-URL: Issue tracker, https://github.com/Ouranosinc/xscen/issues
 Keywords: xscen
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -26,60 +24,139 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ============
 xscen |logo|
 ============
 
-|build| |docs| |black| |pre-commit|
+|pypi| |status| |build| |docs| |black| |pre-commit| |versions|
 
 A climate change scenario-building analysis framework, built with Intake-esm catalogs and xarray-based packages such as xclim and xESMF.
 
 For documentation concerning `xscen`, see: https://xscen.readthedocs.io/en/latest/
 
 Features
 --------
 * Supports workflows with YAML configuration files for better transparency, reproducibility, and long-term backups.
 * Intake_esm-based catalog to find and manage climate data.
 * Climate dataset extraction, subsetting, and temporal aggregation.
 * Calculate missing variables through Intake-esm's DerivedVariableRegistry.
 * Regridding with xESMF.
 * Bias adjustment with xclim.
 
+Installation
+------------
+
+Please refer to the `installation docs`_.
+
 Acknowledgments
 ---------------
 This package was created with Cookiecutter_ and the `Ouranosinc/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyfeldroy/cookiecutter-pypackage
 .. _`Ouranosinc/cookiecutter-pypackage`: https://github.com/Ouranosinc/cookiecutter-pypackage
+.. _installation docs: https://xscen.readthedocs.io/en/latest/installation.html
 
 .. |logo| image:: https://raw.githubusercontent.com/Ouranosinc/xscen/main/docs/_static/_images/xscen-logo-small.png
         :target: https://github.com/Ouranosinc/xscen
 
 .. |build| image:: https://github.com/Ouranosinc/xscen/actions/workflows/main.yml/badge.svg
         :target: https://github.com/Ouranosinc/xscen/actions/workflows/main.yml
         :alt: Build Status
 
+.. |pypi| image:: https://img.shields.io/pypi/v/xscen.svg
+        :target: https://pypi.python.org/pypi/xscen
+        :alt: Python Package Index Build
+
 .. |docs| image:: https://readthedocs.org/projects/xscen/badge/?version=latest
         :target: https://xscen.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/psf/black
         :alt: Python Black
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/Ouranosinc/xscen/main.svg
         :target: https://results.pre-commit.ci/latest/github/Ouranosinc/xscen/main
         :alt: pre-commit.ci status
 
+.. |versions| image:: https://img.shields.io/pypi/pyversions/xscen.svg
+        :target: https://pypi.python.org/pypi/xscen
+        :alt: Supported Python Versions
+
+.. |status| image:: https://www.repostatus.org/badges/latest/wip.svg
+        :target: https://www.repostatus.org/#wip
+        :alt: Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.
+
 
 =======
 History
 =======
 
+v0.6.0 (2023-05-04)
+-------------------
+Contributors to this version: Trevor James Smith (`@Zeitsperre <https://github.com/Zeitsperre>`_), Juliette Lavoie (`@juliettelavoie <https://github.com/juliettelavoie>`_), Pascal Bourgault (`@aulemahal <https://github.com/aulemahal>`_), Gabriel Rondeau-Genesse (`@RondeauG <https://github.com/RondeauG>`_).
+
+Announcements
+^^^^^^^^^^^^^
+* `xscen` is now offered as a conda package available through Anaconda.org. Refer to the installation documentation for more information. (`GH/149 <https://github.com/Ouranosinc/xscen/issues/149>`_, `PR/171 <https://github.com/Ouranosinc/xscen/pull/171>`_).
+* Deprecation: Release 0.6.0 of `xscen` will be the last version to support ``xscen.extract.clisops_subset``. Use ``xscen.spatial.subset`` instead. (`PR/182 <https://github.com/Ouranosinc/xscen/pull/182>`_, `PR/184 <https://github.com/Ouranosinc/xscen/pull/184>`_).
+* Deprecation: The argument `region`, used in multiple functions, has been slightly reformatted. Release 0.6.0 of `xscen` will be the last version to support the old format. (`GH/99 <https://github.com/Ouranosinc/xscen/issues/99>`_, `GH/101 <https://github.com/Ouranosinc/xscen/issues/101>`_, `PR/184 <https://github.com/Ouranosinc/xscen/pull/184>`_).
+
+New features and enhancements
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+* New 'cos-lat' averaging in `spatial_mean`. (`GH/94 <https://github.com/Ouranosinc/xscen/issues/94>`_, `PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* Support for computing anomalies in `compute_deltas`.  (`PR/165 <https://github.com/Ouranosinc/xscen/pull/165>`_).
+* Add function `diagnostics.measures_improvement_2d`. (`PR/167 <https://github.com/Ouranosinc/xscen/pull/167>`_).
+* Add function ``regrid.create_bounds_rotated_pole`` and automatic use in ``regrid_dataset`` and ``spatial_mean``. This is temporary, while we wait for a functionning method in ``cf_xarray``. (`PR/174 <https://github.com/Ouranosinc/xscen/pull/174>`_, `GH/96 <https://github.com/Ouranosinc/xscen/issues/96>`_).
+* Add ``spatial`` submodule with functions ``creep_weights`` and ``creep_fill`` for filling NaNs using neighbours. (`PR/174 <https://github.com/Ouranosinc/xscen/pull/174>`_).
+* Allow passing ``GeoDataFrame`` instances in ``spatial_mean``'s ``region`` argument, not only geospatial file paths. (`PR/174 <https://github.com/Ouranosinc/xscen/pull/174>`_).
+* Allow searching for periods in `catalog.search`. (`GH/123 <https://github.com/Ouranosinc/xscen/issues/123>`_, `PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* Allow searching and extracting multiple frequencies for a given variable. (`GH/168 <https://github.com/Ouranosinc/xscen/issues/168>`_, `PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* New masking feature in ``extract_dataset``. (`GH/180 <https://github.com/Ouranosinc/xscen/issues/180>`_, `PR/182 <https://github.com/Ouranosinc/xscen/pull/182>`_).
+* New function ``xs.spatial.subset`` to replace ``xs.extract.clisops_subset`` and add method "sel". (`GH/180 <https://github.com/Ouranosinc/xscen/issues/180>`_, `PR/182 <https://github.com/Ouranosinc/xscen/pull/182>`_).
+* Add long_name attribute to diagnostics. ( `PR/189 <https://github.com/Ouranosinc/xscen/pull/189>`_).
+* Added a new YAML-centric notebook (`GH/8 <https://github.com/Ouranosinc/xscen/issues/8>`_, `PR/191 <https://github.com/Ouranosinc/xscen/pull/191>`_).
+* New ``utils.standardize_periods`` to standardize that argument across multiple functions. (`GH/87 <https://github.com/Ouranosinc/xscen/issues/87>`_, `PR/192 <https://github.com/Ouranosinc/xscen/pull/192>`_).
+* New `coverage_kwargs` argument added to ``search_data_catalogs`` to allow modifying the default values of ``subset_file_coverage``. (`GH/87 <https://github.com/Ouranosinc/xscen/issues/87>`_, `PR/192 <https://github.com/Ouranosinc/xscen/pull/192>`_).
+
+Breaking changes
+^^^^^^^^^^^^^^^^
+* 'mean' averaging has been deprecated in `spatial_mean`. (`PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* 'interp_coord' has been renamed to 'interp_centroid' in `spatial_mean`. (`PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* The 'datasets' dimension of the output of ``diagnostics.measures_heatmap`` is renamed 'realization'. (`PR/167 <https://github.com/Ouranosinc/xscen/pull/167>`_).
+* `_subset_file_coverage` was renamed `subset_file_coverage` and moved to ``catalog.py`` to prevent circular imports. (`PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* `extract_dataset` doesn't fail when a variable is in the dataset, but not `variables_and_freqs`. (`PR/185 <https://github.com/Ouranosinc/xscen/pull/185>`_).
+* The argument `period`, used in multiple function, is now always a single list, while `periods` is more flexible. (`GH/87 <https://github.com/Ouranosinc/xscen/issues/87>`_, `PR/192 <https://github.com/Ouranosinc/xscen/pull/192>`_).
+* The parameters `reference_period` and `simulation_period` of ``xscen.train`` and ``xscen.adjust`` were renamed `period/periods` to respect the point above. (`GH/87 <https://github.com/Ouranosinc/xscen/issues/87>`_, `PR/192 <https://github.com/Ouranosinc/xscen/pull/192>`_).
+
+Bug fixes
+^^^^^^^^^
+* Forbid pandas v1.5.3 in the environment files, as the linux conda build breaks the data catalog parser. (`GH/161 <https://github.com/Ouranosinc/xscen/issues/161>`_, `PR/162 <https://github.com/Ouranosinc/xscen/pull/162>`_).
+* Only return requested variables when using ``DataCatalog.to_dataset``. (`PR/163 <https://github.com/Ouranosinc/xscen/pull/163>`_).
+* ``compute_indicators`` no longer crashes if less than 3 timesteps are produced. (`PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* `xarray` is temporarily pinned below v2023.3.0 due to an API-breaking change. (`GH/175 <https://github.com/Ouranosinc/xscen/issues/175>`_, `PR/173 <https://github.com/Ouranosinc/xscen/pull/173>`_).
+* `xscen.utils.unstack_fill_nan`` can now handle datasets that have non dimension coordinates. (`GH/156 <https://github.com/Ouranosinc/xscen/issues/156>`_, `PR/175 <https://github.com/Ouranosinc/xscen/pull/175>`_).
+* `extract_dataset` now skips a simulation way earlier if the frequency doesn't match. (`PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* `extract_dataset` now correctly tries to extract in reverse timedelta order. (`PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* `compute_deltas` no longer creates all NaN values if the input dataset is in a non-standard calendar. (`PR/188 <https://github.com/Ouranosinc/xscen/pull/188>`_).
+
+Internal changes
+^^^^^^^^^^^^^^^^
+* `xscen` now manages packaging for PyPi and TestPyPI via GitHub workflows. (`PR/159 <https://github.com/Ouranosinc/xscen/pull/159>`_).
+* Pre-load coordinates in ``extract.clisops_subset`` (`PR/163 <https://github.com/Ouranosinc/xscen/pull/163>`_).
+* Minimal documentation for templates. (`PR/163 <https://github.com/Ouranosinc/xscen/pull/163>`_).
+* `xscen` is now indexed in `Zenodo <https://zenodo.org/>`_, under the `ouranos` community of projects. (`PR/164 <https://github.com/Ouranosinc/xscen/pull/164>`_).
+* Added a few relevant `Shields <https://shields.io/>`_ to the README.rst. (`PR/164 <https://github.com/Ouranosinc/xscen/pull/164>`_).
+* Better warning messages in ``_subset_file_coverage`` when coverage is insufficient. (`PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* The top-level Makefile now includes a `linkcheck` recipe, and the ReadTheDocs configuration no longer reinstalls the `llvmlite` compiler library. (`PR/173 <https://github.com/Ouranosinc/xscen/pull/173>`_).
+* The checkups on coverage and duplicates can now be skipped in `subset_file_coverage`. (`PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* Changed the `ProjectCatalog` docstrings to make it more obvious that it needs to be created empty. (`GH/99 <https://github.com/Ouranosinc/xscen/issues/99>`_, `PR/184 <https://github.com/Ouranosinc/xscen/pull/184>`_).
+* Added parse_config to `creep_fill`, `creep_weights`, and `reduce_ensemble` (`PR/191 <https://github.com/Ouranosinc/xscen/pull/191>`_).
+
 v0.5.0 (2023-02-28)
 -------------------
 Contributors to this version: Gabriel Rondeau-Genesse (`@RondeauG <https://github.com/RondeauG>`_), Juliette Lavoie (`@juliettelavoie <https://github.com/juliettelavoie>`_), Trevor James Smith (`@Zeitsperre <https://github.com/Zeitsperre>`_), Sarah Gammon (`@sg2475962 <https://github.com/sg2475962>`_) and Pascal Bourgault (`@aulemahal <https://github.com/aulemahal>`_).
 
 New features and enhancements
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 * Possibility of excluding variables read from file from the catalog produced by ``parse_directory``. (`PR/107 <https://github.com/Ouranosinc/xscen/pull/107>`_).
@@ -119,15 +196,15 @@
 * ``compute_deltas`` skips the unstacking step if there is no time dimension and cast object dimensions to string. (`PR/9 <https://github.com/Ouranosinc/xscen/pull/9>`_)
 * Added the "2sem" frequency to the translations CVs. (`PR/111 <https://github.com/Ouranosinc/xscen/pull/111>`_).
 * Skip files we can't read in ``parse_directory``. (`PR/111 <https://github.com/Ouranosinc/xscen/pull/111>`_).
 * Fixed non-numpy-standard Docstrings. (`PR/108 <https://github.com/Ouranosinc/xscen/pull/108>`_).
 * Added more metadata to package description on PyPI. (`PR/108 <https://github.com/Ouranosinc/xscen/pull/108>`_).
 * Faster ``search_data_catalogs`` and ``extract_dataset`` through a faster ``DataCatalog.unique``, date parsing and a rewrite of the ``ensure_correct_time`` logic. (`PR/127 <https://github.com/Ouranosinc/xscen/pull/127>`_).
 * The ``search_data_catalogs`` function now accepts `str` or `pathlib.Path` variables (in addition to lists of either data type) for performing catalog lookups. (`PR/121 <https://github.com/Ouranosinc/xscen/pull/121>`_).
-* `produce_horizons` now supports fixed fields (pull:`139`).
+* `produce_horizons` now supports fixed fields (`PR/139 <https://github.com/Ouranosinc/xscen/pull/139>`_).
 * Rewrite of ``unstack_dates`` for better performance with dask arrays. (`PR/144 <https://github.com/Ouranosinc/xscen/pull/144>`_).
 
 v0.4.0 (2022-09-28)
 -------------------
 Contributors to this version: Gabriel Rondeau-Genesse (`@RondeauG <https://github.com/RondeauG>`_), Juliette Lavoie (`@juliettelavoie <https://github.com/juliettelavoie>`_), Trevor James Smith (`@Zeitsperre <https://github.com/Zeitsperre>`_) and Pascal Bourgault (`@aulemahal <https://github.com/aulemahal>`_).
 
 New features and enhancements
@@ -238,9 +315,7 @@
 Breaking changes
 ^^^^^^^^^^^^^^^^
 * N/A
 
 Internal changes
 ^^^^^^^^^^^^^^^^
 * N/A
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xscen-0.5.0/README.rst` & `xscen-0.6.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 ============
 xscen |logo|
 ============
 
-|build| |docs| |black| |pre-commit|
+|pypi| |status| |build| |docs| |black| |pre-commit| |versions|
 
 A climate change scenario-building analysis framework, built with Intake-esm catalogs and xarray-based packages such as xclim and xESMF.
 
 For documentation concerning `xscen`, see: https://xscen.readthedocs.io/en/latest/
 
 Features
 --------
 * Supports workflows with YAML configuration files for better transparency, reproducibility, and long-term backups.
 * Intake_esm-based catalog to find and manage climate data.
 * Climate dataset extraction, subsetting, and temporal aggregation.
 * Calculate missing variables through Intake-esm's DerivedVariableRegistry.
 * Regridding with xESMF.
 * Bias adjustment with xclim.
 
+Installation
+------------
+
+Please refer to the `installation docs`_.
+
 Acknowledgments
 ---------------
 This package was created with Cookiecutter_ and the `Ouranosinc/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyfeldroy/cookiecutter-pypackage
 .. _`Ouranosinc/cookiecutter-pypackage`: https://github.com/Ouranosinc/cookiecutter-pypackage
+.. _installation docs: https://xscen.readthedocs.io/en/latest/installation.html
 
 .. |logo| image:: https://raw.githubusercontent.com/Ouranosinc/xscen/main/docs/_static/_images/xscen-logo-small.png
         :target: https://github.com/Ouranosinc/xscen
 
 .. |build| image:: https://github.com/Ouranosinc/xscen/actions/workflows/main.yml/badge.svg
         :target: https://github.com/Ouranosinc/xscen/actions/workflows/main.yml
         :alt: Build Status
 
+.. |pypi| image:: https://img.shields.io/pypi/v/xscen.svg
+        :target: https://pypi.python.org/pypi/xscen
+        :alt: Python Package Index Build
+
 .. |docs| image:: https://readthedocs.org/projects/xscen/badge/?version=latest
         :target: https://xscen.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/psf/black
         :alt: Python Black
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/Ouranosinc/xscen/main.svg
         :target: https://results.pre-commit.ci/latest/github/Ouranosinc/xscen/main
         :alt: pre-commit.ci status
+
+.. |versions| image:: https://img.shields.io/pypi/pyversions/xscen.svg
+        :target: https://pypi.python.org/pypi/xscen
+        :alt: Supported Python Versions
+
+.. |status| image:: https://www.repostatus.org/badges/latest/wip.svg
+        :target: https://www.repostatus.org/#wip
+        :alt: Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xscen-0.5.0/setup.cfg` & `xscen-0.6.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.0
+current_version = 0.6.0
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+).(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
```

### Comparing `xscen-0.5.0/setup.py` & `xscen-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,30 +23,33 @@
 
 # This list are the minimum requirements for xscen
 # this is only meant to make `pip check` work
 # xscen dependencies can only be installed through conda-forge.
 requirements = [
     "cartopy",
     "cftime",
-    "clisops",
+    "cf_xarray>=0.7.6",
+    "clisops>=0.9.5",
     "dask",
     "flox",
     "fsspec",
     "geopandas",
     "h5netcdf",
     "intake",
     "intake-esm>=2022.9.18",
     "matplotlib",
     "netCDF4",
     "numpy",
-    "pandas",
+    "pandas!=1.5.3",
+    "pyarrow",  # Used when opening catalogs.
+    "pygeos",
     "pyyaml",
     "rechunker",
     "shapely",
-    "xarray",
+    "xarray<2023.3.0",  # See https://github.com/Ouranosinc/xscen/pull/173
     "xclim>=0.37",
     "xesmf>=0.7",  # This is not available on pypi.
     "zarr",
 ]
 
 setup(
     author="Gabriel Rondeau-Genesse",
@@ -76,10 +79,10 @@
         "About Ouranos": "https://www.ouranos.ca/en/",
         "Changelog": "https://xscen.readthedocs.io/en/stable/history.html",
         "Issue tracker": "https://github.com/Ouranosinc/xscen/issues",
     },
     test_suite="tests",
     tests_require=["pytest", "pytest-cov"],
     url="https://github.com/Ouranosinc/xscen",
-    version="0.5.0",
+    version="0.6.0",
     zip_safe=False,
 )
```

### Comparing `xscen-0.5.0/tests/conftest.py` & `xscen-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/xscen/__init__.py` & `xscen-0.6.0/xscen/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     ensembles,
     extract,
     indicators,
     io,
     reduce,
     regrid,
     scripting,
+    spatial,
     utils,
 )
 
 # Import top-level functions
 from .aggregate import *
 from .biasadjust import *
 from .catalog import DataCatalog, ProjectCatalog  # noqa
@@ -37,15 +38,15 @@
     send_mail_on_exit,
     timeout,
 )
 from .utils import clean_up
 
 __author__ = """Gabriel Rondeau-Genesse"""
 __email__ = "rondeau-genesse.gabriel@ouranos.ca"
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 
 # monkeypatch so that warnings.warn() doesn't mention itself
 def warning_on_one_line(
     message: str, category: Warning, filename: str, lineno: int, file=None, line=None
 ):  # noqa: D103
     return f"{filename}:{lineno}: {category.__name__}: {message}\n"
```

### Comparing `xscen-0.5.0/xscen/aggregate.py` & `xscen-0.6.0/xscen/aggregate.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 from pathlib import Path, PosixPath
 from types import ModuleType
 from typing import Sequence, Tuple, Union
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
+import pygeos
 import xarray as xr
+import xclim.core.calendar
 import xesmf as xe
 from shapely.geometry import Polygon
 from xclim.core.indicator import Indicator
 
 from .config import parse_config
-from .extract import clisops_subset
 from .indicators import compute_indicators
-from .utils import get_cat_attrs, unstack_dates
+from .spatial import subset
+from .utils import standardize_periods, unstack_dates
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "climatological_mean",
     "compute_deltas",
     "spatial_mean",
@@ -53,15 +55,15 @@
     min_periods : int
         For the rolling operation, minimum number of years required for a value to be computed.
         If left at None and the xrfreq is either QS or AS and doesn't start in January, min_periods will be one less than window.
         If left at None, it will be deemed the same as 'window'.
     interval : int
         Interval (in years) at which to provide an output.
     periods : list
-        list of [start, end] of continuous periods to be considered. This is needed when the time axis of ds contains some jumps in time.
+        Either [start, end] or list of [start, end] of continuous periods to be considered. This is needed when the time axis of ds contains some jumps in time.
         If None, the dataset will be considered continuous.
     to_level : str, optional
         The processing level to assign to the output.
         If None, the processing level of the inputs is preserved.
 
     Returns
     -------
@@ -86,26 +88,28 @@
 
     # Rolling will ignore jumps in time, so we want to raise an exception beforehand
     if (not all(ds_unstack.year.diff(dim="year", n=1) == 1)) & (periods is None):
         raise ValueError("Data is not continuous. Use the 'periods' argument.")
 
     # Compute temporal means
     concats = []
-    periods = periods or [[int(ds_unstack.year[0]), int(ds_unstack.year[-1])]]
+    periods = standardize_periods(
+        periods or [[int(ds_unstack.year[0]), int(ds_unstack.year[-1])]]
+    )
 
     window = window or int(periods[0][1]) - int(periods[0][0]) + 1
 
     if ds.attrs.get("cat:xrfreq") in freq_across_year and min_periods is None:
         min_periods = window - 1
     min_periods = min_periods or window
 
     for period in periods:
         # Rolling average
         ds_rolling = (
-            ds_unstack.sel(year=slice(str(period[0]), str(period[1])))
+            ds_unstack.sel(year=slice(period[0], period[1]))
             .rolling(year=window, min_periods=min_periods)
             .mean()
         )
 
         # Select every horizons in 'x' year intervals, starting from the first full windowed mean
         ds_rolling = ds_rolling.isel(
             year=slice(window - 1, None)
@@ -117,20 +121,37 @@
             dims=dict(year=ds_rolling.year),
         ).astype(str)
         ds_rolling = ds_rolling.assign_coords(horizon=horizons)
 
         # get back to 1D time
         ds_rolling = ds_rolling.stack(time=("year", "month", "day"))
         # rebuild time coord
-        time_coord = [
-            pd.to_datetime(f"{y - window + 1}, {m}, {d}")
-            for y, m, d in zip(
-                ds_rolling.year.values, ds_rolling.month.values, ds_rolling.day.values
+        if isinstance(ds.indexes["time"], pd.core.indexes.datetimes.DatetimeIndex):
+            time_coord = list(
+                pd.to_datetime(
+                    {
+                        "year": ds_rolling.year.values - window + 1,
+                        "month": ds_rolling.month.values,
+                        "day": ds_rolling.day.values,
+                    }
+                ).values
             )
-        ]
+        elif isinstance(ds.indexes["time"], xr.coding.cftimeindex.CFTimeIndex):
+            time_coord = [
+                xclim.core.calendar.datetime_classes[ds.time.dt.calendar](
+                    y - window + 1, m, d
+                )
+                for y, m, d in zip(
+                    ds_rolling.year.values,
+                    ds_rolling.month.values,
+                    ds_rolling.day.values,
+                )
+            ]
+        else:
+            raise ValueError("The type of 'time' could not be understood.")
         ds_rolling = ds_rolling.assign_coords(time=time_coord).transpose("time", ...)
 
         concats.extend([ds_rolling])
     ds_rolling = xr.concat(concats, dim="time", data_vars="minimal")
 
     # modify attrs and history
     for vv in ds_rolling.data_vars:
@@ -156,44 +177,60 @@
 
     return ds_rolling
 
 
 @parse_config
 def compute_deltas(
     ds: xr.Dataset,
-    reference_horizon: str,
+    reference_horizon: Union[str, xr.Dataset],
     *,
     kind: Union[str, dict] = "+",
     rename_variables: bool = True,
     to_level: str = "delta_climatology",
 ) -> xr.Dataset:
     """Compute deltas in comparison to a reference time period, respecting the temporal resolution of ds.
 
     Parameters
     ----------
     ds : xr.Dataset
         Dataset to use for the computation.
-    reference_horizon : str
-        YYYY-YYYY string corresponding to the 'horizon' coordinate of the reference period.
+    reference_horizon : str or xr.Dataset
+        Either a YYYY-YYYY string corresponding to the 'horizon' coordinate of the reference period, or a xr.Dataset containing the climatological mean.
     kind : str
         ['+', '/', '%'] Whether to provide absolute, relative, or percentage deltas.
         Can also be a dictionary separated per variable name.
     rename_variables : bool
         If True, '_delta_YYYY-YYYY' will be added to variable names.
     to_level : str, optional
         The processing level to assign to the output.
         If None, the processing level of the inputs is preserved.
 
     Returns
     -------
     xr.Dataset
         Returns a Dataset with the requested deltas.
     """
-    # Separate the reference from the other horizons
-    ref = ds.where(ds.horizon == reference_horizon, drop=True)
+    if isinstance(reference_horizon, str):
+        # Separate the reference from the other horizons
+        ref = ds.where(ds.horizon == reference_horizon, drop=True)
+    elif isinstance(reference_horizon, xr.Dataset):
+        ref = reference_horizon
+        if "horizon" in ref:
+            reference_horizon = np.unique(ref["horizon"])
+            if len(reference_horizon) != 1:
+                raise ValueError(
+                    "The reference dataset appears to contain multiple horizons."
+                )
+            reference_horizon = reference_horizon[0]
+        else:
+            reference_horizon = "unknown_horizon"
+    else:
+        raise ValueError(
+            "reference_horizon should be either a string or an xarray.Dataset."
+        )
 
     if "time" in ds:
         # Remove references to 'year' in REF
         ind = pd.MultiIndex.from_arrays(
             [ref.time.dt.month.values, ref.time.dt.day.values], names=["month", "day"]
         )
         ref = ref.assign(time=ind).unstack("time")
@@ -206,15 +243,15 @@
             ],
             names=["year", "month", "day"],
         )
         other_hz = ds.assign(time=ind).unstack("time")
 
     else:
         other_hz = ds
-        ref = ref.squeeze("horizon")
+        ref = ref.squeeze()
     deltas = xr.Dataset(coords=other_hz.coords, attrs=other_hz.attrs)
     # Calculate deltas
     for vv in list(ds.data_vars):
         v_name = (
             vv
             if rename_variables is False
             else f"{vv}_delta_{reference_horizon.replace('-', '_')}"
@@ -253,57 +290,73 @@
         )
         deltas[v_name].attrs["history"] = history
 
     if "time" in ds:
         # get back to 1D time
         deltas = deltas.stack(time=("year", "month", "day"))
         # rebuild time coord
-        time_coord = [
-            pd.to_datetime(f"{y}, {m}, {d}")
-            for y, m, d in zip(
-                deltas.year.values, deltas.month.values, deltas.day.values
+        if isinstance(ds.indexes["time"], pd.core.indexes.datetimes.DatetimeIndex):
+            time_coord = list(
+                pd.to_datetime(
+                    {
+                        "year": deltas.year.values,
+                        "month": deltas.month.values,
+                        "day": deltas.day.values,
+                    }
+                ).values
             )
-        ]
+        elif isinstance(ds.indexes["time"], xr.coding.cftimeindex.CFTimeIndex):
+            time_coord = [
+                xclim.core.calendar.datetime_classes[ds.time.dt.calendar](y, m, d)
+                for y, m, d in zip(
+                    deltas.year.values, deltas.month.values, deltas.day.values
+                )
+            ]
+        else:
+            raise ValueError("The type of 'time' could not be understood.")
+
         deltas = deltas.assign(time=time_coord).transpose("time", ...)
         deltas = deltas.reindex_like(ds)
 
     if to_level is not None:
         deltas.attrs["cat:processing_level"] = to_level
 
     return deltas
 
 
 @parse_config
 def spatial_mean(
     ds: xr.Dataset,
     method: str,
     *,
+    spatial_subset: bool = None,
     call_clisops: bool = False,
     region: dict = None,
     kwargs: dict = None,
     simplify_tolerance: float = None,
     to_domain: str = None,
     to_level: str = None,
 ) -> xr.Dataset:
     """Compute the spatial mean using a variety of available methods.
 
     Parameters
     ----------
     ds : xr.Dataset
         Dataset to use for the computation.
     method : str
-        'mean' will perform a .mean() over the spatial dimensions of the Dataset.
-        'interp_coord' will find the region's centroid (if coordinates are not fed through kwargs), then perform a .interp() over the spatial dimensions of the Dataset.
+        'cos-lat' will weight the area covered by each pixel using an approximation based on latitude.
+        'interp_centroid' will find the region's centroid (if coordinates are not fed through kwargs), then perform a .interp() over the spatial dimensions of the Dataset.
         The coordinate can also be directly fed to .interp() through the 'kwargs' argument below.
         'xesmf' will make use of xESMF's SpatialAverager. This will typically be more precise, especially for irregular regions, but can be much slower than other methods.
-    call_clisops : bool
-        If True, xscen.extraction.clisops_subset will be called prior to the other operations. This requires the 'region' argument.
+    spatial_subset : bool
+        If True, xscen.spatial.subset will be called prior to the other operations. This requires the 'region' argument.
+        If None, this will automatically become True if 'region' is provided and the subsetting method is either 'cos-lat' or 'mean'.
     region : dict
         Description of the region and the subsetting method (required fields listed in the Notes).
-        If method=='interp_coord', this is used to find the region's centroid.
+        If method=='interp_centroid', this is used to find the region's centroid.
         If method=='xesmf', the bounding box or shapefile is given to SpatialAverager.
     kwargs : dict
         Arguments to send to either mean(), interp() or SpatialAverager().
         For SpatialAverager, one can give `skipna` here, to be passed to the averager call itself.
     simplify_tolerance : float
         Precision (in degree) used to simplify a shapefile before sending it to SpatialAverager().
         The simpler the polygons, the faster the averaging, but it will lose some precision.
@@ -318,87 +371,160 @@
     -------
     xr.Dataset
         Returns a Dataset with the spatial dimensions averaged.
 
     Notes
     -----
     'region' required fields:
+        name: str
+            Region name used to overwrite domain in the catalog.
         method: str
-            ['gridpoint', 'bbox', shape']
-        <method>: dict
+            ['gridpoint', 'bbox', shape', 'sel']
+        tile_buffer: float, optional
+            Multiplier to apply to the model resolution. Only used if spatial_subset==True.
+        kwargs
             Arguments specific to the method used.
-        buffer: float, optional
-            Multiplier to apply to the model resolution. Only used if call_clisops==True.
 
     See Also
     --------
     xarray.Dataset.mean, xarray.Dataset.interp, xesmf.SpatialAverager
     """
     kwargs = kwargs or {}
-
-    # If requested, call xscen.extraction.clisops_subset prior to averaging
+    if method == "mean":
+        warnings.warn(
+            "xs.spatial_mean with method=='mean' is deprecated and will be abandoned in a future release. Use method=='cos-lat' instead for a more robust but similar method.",
+            category=FutureWarning,
+        )
+    elif method == "interp_coord":
+        warnings.warn(
+            "xs.spatial_mean with method=='interp_coord' is deprecated. Use method=='interp_centroid' instead.",
+            category=FutureWarning,
+        )
+        method = "interp_centroid"
     if call_clisops:
-        ds = clisops_subset(ds, region)
+        warnings.warn(
+            "call_clisops has been renamed and is deprecated. Use spatial_subset instead.",
+            category=FutureWarning,
+        )
+        spatial_subset = call_clisops
+
+    if (
+        (region is not None)
+        and (region["method"] in region)
+        and (isinstance(region[region["method"]], dict))
+    ):
+        warnings.warn(
+            "You seem to be using a deprecated version of region. Please use the new formatting.",
+            category=FutureWarning,
+        )
+        region = deepcopy(region)
+        if "buffer" in region:
+            region["tile_buffer"] = region.pop("buffer")
+        _kwargs = region.pop(region["method"])
+        region.update(_kwargs)
+
+    if (
+        (region is not None)
+        and (spatial_subset is None)
+        and (method in ["mean", "cos-lat"])
+    ):
+        logger.info("Automatically turning spatial_subset to True based on inputs.")
+        spatial_subset = True
+
+    # If requested, call xscen.spatial.subset prior to averaging
+    if spatial_subset:
+        ds = subset(ds, **region)
+
+    if method == "cos-lat":
+        if "latitude" not in ds.cf.coordinates:
+            raise ValueError(
+                "Could not determine the latitude name using CF conventions. "
+                "Use kwargs = {lat: str} to specify the coordinate name."
+            )
+
+        if "units" not in ds.cf["latitude"].attrs:
+            logger.warning(
+                f"{ds.attrs.get('cat:id', '')}: Latitude does not appear to have units. Make sure that the computation is right."
+            )
+        elif ds.cf["latitude"].attrs["units"] != "degrees_north":
+            logger.warning(
+                f"{ds.attrs.get('cat:id', '')}: Latitude units is '{ds.cf['latitude'].attrs['units']}', expected 'degrees_north'. "
+                f"Make sure that the computation is right."
+            )
+
+        if ((ds.cf["longitude"].min() < -160) & (ds.cf["longitude"].max() > 160)) or (
+            (ds.cf["longitude"].min() < 20) & (ds.cf["longitude"].max() > 340)
+        ):
+            logger.warning(
+                "The region appears to be crossing the -180/180° meridian. Bounds computation is currently bugged in cf_xarray. "
+                "Make sure that the computation is right."
+            )
+
+        ds = ds.cf.add_bounds(["longitude", "latitude"])
+        weights = xr.DataArray(
+            pygeos.area(
+                pygeos.polygons(pygeos.linearrings(ds.lon_bounds, ds.lat_bounds))
+            ),
+            dims=ds.cf["longitude"].dims,
+            coords=ds.cf["longitude"].coords,
+        ) * np.cos(np.deg2rad(ds.cf["latitude"]))
+
+        ds_agg = ds.weighted(weights).mean(
+            [d for d in ds.cf.axes["X"] + ds.cf.axes["Y"]], keep_attrs=True
+        )
+
+        # Prepare the History field
+        new_history = (
+            f"[{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}] "
+            f"weighted mean(dim={[d for d in ds.cf.axes['X'] + ds.cf.axes['Y']]}) using a 'cos-lat' approximation of areacella (in deg2)"
+        )
 
     # This simply calls .mean() over the spatial dimensions
-    if method == "mean":
+    elif method == "mean":
         if "dim" not in kwargs:
-            # Determine the X and Y names
-            spatial_dims = []
-            for d in ["X", "Y"]:
-                if d in ds.cf.axes:
-                    spatial_dims.extend([ds.cf[d].name])
-                elif (
-                    (d == "X")
-                    and ("longitude" in ds.cf.coordinates)
-                    and (len(ds[ds.cf.coordinates["longitude"][0]].dims) == 1)
-                ):
-                    spatial_dims.extend(ds.cf.coordinates["longitude"])
-                elif (
-                    (d == "Y")
-                    and ("latitude" in ds.cf.coordinates)
-                    and (len(ds[ds.cf.coordinates["latitude"][0]].dims) == 1)
-                ):
-                    spatial_dims.extend(ds.cf.coordinates["latitude"])
-            if len(spatial_dims) == 0:
-                raise ValueError(
-                    "Could not determine the spatial dimension(s) using CF conventions. Use kwargs = {dim: list} to specify on which dimension to perform the averaging."
-                )
-            kwargs["dim"] = spatial_dims
+            kwargs["dim"] = ds.cf.axes["X"] + ds.cf.axes["Y"]
 
         ds_agg = ds.mean(keep_attrs=True, **kwargs)
 
         # Prepare the History field
         new_history = (
             f"[{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}] "
             f"xarray.mean(dim={kwargs['dim']}) - xarray v{xr.__version__}"
         )
 
     # This calls .interp() to a pair of coordinates
-    elif method == "interp_coord":
+    elif method == "interp_centroid":
         # Find the centroid
-        if region is not None:
+        if region is None:
+            if ds.cf.axes["X"][0] not in kwargs:
+                kwargs[ds.cf.axes["X"][0]] = ds[ds.cf.axes["X"][0]].mean().values
+            if ds.cf.axes["Y"][0] not in kwargs:
+                kwargs[ds.cf.axes["Y"][0]] = ds[ds.cf.axes["Y"][0]].mean().values
+        else:
             if region["method"] == "gridpoint":
-                if len(region["gridpoint"]["lon"] != 1):
+                if len(region["lon"] != 1):
                     raise ValueError(
                         "Only a single location should be used with interp_centroid."
                     )
                 centroid = {
-                    "lon": region["gridpoint"]["lon"],
-                    "lat": region["gridpoint"]["lat"],
+                    "lon": region["lon"],
+                    "lat": region["lat"],
                 }
 
             elif region["method"] == "bbox":
                 centroid = {
-                    "lon": np.mean(region["bbox"]["lon_bnds"]),
-                    "lat": np.mean(region["bbox"]["lat_bnds"]),
+                    "lon": np.mean(region["lon_bnds"]),
+                    "lat": np.mean(region["lat_bnds"]),
                 }
 
             elif region["method"] == "shape":
-                s = gpd.read_file(region["shape"]["shape"])
+                if not isinstance(region["shape"], gpd.GeoDataFrame):
+                    s = gpd.read_file(region["shape"])
+                else:
+                    s = region["shape"]
                 if len(s != 1):
                     raise ValueError(
                         "Only a single polygon should be used with interp_centroid."
                     )
                 centroid = {"lon": s.centroid[0].x, "lat": s.centroid[0].y}
             else:
                 raise ValueError("'method' not understood.")
@@ -409,75 +535,92 @@
         new_history = (
             f"[{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}] "
             f"xarray.interp(**{kwargs}) - xarray v{xr.__version__}"
         )
 
     # Uses xesmf.SpatialAverager
     elif method == "xesmf":
+        logger.warning(
+            "A bug has been found with xesmf.SpatialAverager that appears to impact big regions. "
+            "Until this is fixed, make sure that the computation is right or use multiple smaller regions."
+        )
         # If the region is a bounding box, call shapely and geopandas to transform it into an input compatible with xesmf
         if region["method"] == "bbox":
             lon_point_list = [
-                region["bbox"]["lon_bnds"][0],
-                region["bbox"]["lon_bnds"][0],
-                region["bbox"]["lon_bnds"][1],
-                region["bbox"]["lon_bnds"][1],
+                region["lon_bnds"][0],
+                region["lon_bnds"][0],
+                region["lon_bnds"][1],
+                region["lon_bnds"][1],
             ]
             lat_point_list = [
-                region["bbox"]["lat_bnds"][0],
-                region["bbox"]["lat_bnds"][1],
-                region["bbox"]["lat_bnds"][1],
-                region["bbox"]["lat_bnds"][0],
+                region["lat_bnds"][0],
+                region["lat_bnds"][1],
+                region["lat_bnds"][1],
+                region["lat_bnds"][0],
             ]
 
             polygon_geom = Polygon(zip(lon_point_list, lat_point_list))
             polygon = gpd.GeoDataFrame(index=[0], geometry=[polygon_geom])
 
             # Prepare the History field
             new_history = (
                 f"[{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}] "
-                f"xesmf.SpatialAverager over {region['bbox']['lon_bnds']}{region['bbox']['lat_bnds']} - xESMF v{xe.__version__}"
+                f"xesmf.SpatialAverager over {region['lon_bnds']}{region['lat_bnds']} - xESMF v{xe.__version__}"
             )
 
         # If the region is a shapefile, open with geopandas
         elif region["method"] == "shape":
-            polygon = gpd.read_file(region["shape"]["shape"])
+            if not isinstance(region["shape"], gpd.GeoDataFrame):
+                polygon = gpd.read_file(region["shape"])
+            else:
+                polygon = region["shape"]
 
             # Simplify the geometries to a given tolerance, if needed.
             # The simpler the polygons, the faster the averaging, but it will lose some precision.
             if simplify_tolerance is not None:
                 polygon["geometry"] = polygon.simplify(
                     tolerance=simplify_tolerance, preserve_topology=True
                 )
 
             # Prepare the History field
             new_history = (
                 f"[{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}] "
-                f"xesmf.SpatialAverager over {Path(region['shape']['shape']).name} - xESMF v{xe.__version__}"
+                f"xesmf.SpatialAverager over {Path(region['shape']).name} - xESMF v{xe.__version__}"
             )
 
         else:
-            raise ValueError("'method' not understood.")
+            raise ValueError("'method' should be one of [bbox, shape].")
 
         kwargs_copy = deepcopy(kwargs)
         skipna = kwargs_copy.pop("skipna", False)
+
+        if (
+            ds.cf["longitude"].ndim == 2
+            and "longitude" not in ds.cf.bounds
+            and "rotated_pole" in ds
+        ):
+            from .regrid import create_bounds_rotated_pole
+
+            ds = ds.update(create_bounds_rotated_pole(ds))
+
         savg = xe.SpatialAverager(ds, polygon.geometry, **kwargs_copy)
         ds_agg = savg(ds, keep_attrs=True, skipna=skipna)
         extra_coords = {
             col: xr.DataArray(polygon[col], dims=("geom",))
             for col in polygon.columns
             if col != "geometry"
         }
         extra_coords["geom"] = xr.DataArray(polygon.index, dims=("geom",))
         ds_agg = ds_agg.assign_coords(**extra_coords)
         if len(polygon) == 1:
             ds_agg = ds_agg.squeeze("geom")
 
     else:
         raise ValueError(
-            "Subsetting method should be ['mean', 'interp_coord', 'xesmf']"
+            "Subsetting method should be ['cos-lat', 'interp_coord', 'xesmf']"
         )
 
     # History
     history = (
         new_history + " \n " + ds_agg.attrs["history"]
         if "history" in ds_agg.attrs
         else new_history
@@ -511,15 +654,15 @@
     Parameters
     ----------
     ds: xr.Dataset
       Input dataset with a time dimension.
     indicators:  Union[str, PosixPath, Sequence[Indicator], Sequence[Tuple[str, Indicator]]]
       Indicators to compute. It will be passed to the `indicators` argument of `xs.compute_indicators`.
     period: list
-      List of strings of format ['start_year', 'end_year'].
+      [start_year, end_year] of the period to be evaluated.
       If None, the whole time coordinate is used.
     to_level:
       The processing level to assign to the output.
       Use "{wl}", "{period0}" and "{period1}" in the string to dynamically include
       the first value of the `warminglevel` coord of ds if it exists, 'period[0]' and 'period[1]'.
 
     Returns
@@ -527,15 +670,16 @@
     xr.Dataset
         Horizon dataset.
     """
     if "warminglevel" in ds and len(ds.warminglevel) != 1:
         warnings.warn(
             "Input dataset should only have `warminglevel` coordinate of length 1."
         )
-    if period:
+    if period is not None:
+        period = standardize_periods(period, multiple=False)
         ds = ds.sel(time=slice(period[0], period[1])).load()
         window = int(period[1]) - int(period[0]) + 1
         if to_level:
             to_level = to_level.format(period0=period[0], period1=period[1])
     else:
         window = int(ds.time.dt.year[-1] - ds.time.dt.year[0]) + 1
         if to_level and "{wl}" not in to_level:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xscen-0.5.0/xscen/biasadjust.py` & `xscen-0.6.0/xscen/biasadjust.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # noqa: D100
 import logging
+import warnings
 from copy import deepcopy
 from typing import Optional, Union
 
 import xarray as xr
 import xclim as xc
 from xclim import sdba
 from xclim.core.calendar import convert_calendar, get_calendar
 from xclim.sdba import construct_moving_yearly_window, unpack_moving_yearly_window
 
 from .catalog import parse_from_ds
 from .config import parse_config
-from .utils import minimum_calendar
+from .utils import minimum_calendar, standardize_periods
 
 # TODO: Change all paths to PosixPath objects, including in the catalog?
 # TODO: Compute sometimes fails randomly (in debug, pretty much always). Also (detrend?) fails with pr. Investigate why.
 
 logger = logging.getLogger(__name__)
 
 
@@ -56,15 +57,15 @@
 
 
 @parse_config
 def train(
     dref: xr.Dataset,
     dhist: xr.Dataset,
     var: list,
-    reference_period: list,
+    period: list,
     *,
     method: str = "DetrendedQuantileMapping",
     group: Union[sdba.Grouper, str, dict] = {"group": "time.dayofyear", "window": 31},
     xclim_train_args: dict = None,
     maximal_calendar: str = "noleap",
     adapt_freq: Optional[dict] = None,
     jitter_under: Optional[dict] = None,
@@ -78,25 +79,25 @@
     ----------
     dref : xr.Dataset
       The target timeseries, on the reference period.
     dhist : xr.Dataset
       The timeseries to adjust, on the reference period.
     var : str
       Variable on which to do the adjustment
+    period : list
+      [start, end] of the reference period
     method : str
       Name of the `sdba.TrainAdjust` method of xclim.
     group : str or sdba.Grouper
       Grouping information
     xclim_train_args : dict
       Dict of arguments to pass to the `.train` of the adjustment object.
     maximal_calendar: str
       Maximal calendar dhist can be. The hierarchy: 360_day < noleap < standard < all_leap.
       If dhist's calendar is higher than maximal calendar, it will be converted to the maximal calendar.
-    reference_period : list
-      [start, end] of the reference period
     adapt_freq: dict, optional
       If given, a dictionary of args to pass to the frequency adaptation function.
     jitter_under: dict, optional
       If given, a dictionary of args to pass to `jitter_under_thresh`.
     jitter_over: dict, optional
       If given, a dictionary of args to pass to `jitter_over_thresh`.
     align_on: str, optional
@@ -122,16 +123,17 @@
         hist = dhist[var[0]]
 
     xclim_train_args = xclim_train_args or {}
     if method == "DetrendedQuantileMapping":
         xclim_train_args.setdefault("nquantiles", 15)
 
     # cut out the right period
-    hist = hist.sel(time=slice(*map(str, reference_period)))
-    ref = ref.sel(time=slice(*map(str, reference_period)))
+    period = standardize_periods(period, multiple=False)
+    hist = hist.sel(time=slice(period[0], period[1]))
+    ref = ref.sel(time=slice(period[0], period[1]))
 
     # convert calendar if necessary
     simcal = get_calendar(hist)
     refcal = get_calendar(ref)
     mincal = minimum_calendar(simcal, maximal_calendar)
     if simcal != mincal:
         hist = convert_calendar(hist, mincal, align_on=align_on)
@@ -183,15 +185,15 @@
     return ds
 
 
 @parse_config
 def adjust(
     dtrain: xr.Dataset,
     dsim: xr.Dataset,
-    simulation_period: list,
+    periods: list,
     xclim_adjust_args: dict,
     *,
     to_level: str = "biasadjusted",
     bias_adjust_institution: str = None,
     bias_adjust_project: str = None,
     moving_yearly_window: Optional[dict] = None,
     align_on: Optional[str] = "year",
@@ -201,16 +203,16 @@
 
     Parameters
     ----------
     dtrain : xr.Dataset
       A trained algorithm's dataset, as returned by `train`.
     dsim : xr.Dataset
       Simulated timeseries, projected period.
-    simulation_period : list
-      [start, end] of the simulation period. or list of list if we want to adjust different period one at a time.
+    periods : list
+      Either [start, end] or list of [start, end] of the simulation periods to be adjusted (one at a time).
     xclim_adjust_args : dict
       Dict of arguments to pass to the `.adjust` of the adjustment object.
     to_level : str, optional
       The processing level to assign to the output.
       Defaults to 'biasadjusted'
     bias_adjust_institution : str, optional
       The institution to assign to the output.
@@ -263,36 +265,33 @@
     simcal = get_calendar(sim)
     mincal = minimum_calendar(simcal, dtrain.attrs["train_params"]["maximal_calendar"])
     if simcal != mincal:
         sim = convert_calendar(sim, mincal, align_on=align_on)
 
     xclim_adjust_args = xclim_adjust_args or {}
     # do the adjustment for all the simulation_period lists
-    if isinstance(
-        simulation_period[0], str
-    ):  # if only one period, turn it into a list of list
-        simulation_period = [simulation_period]
+    periods = standardize_periods(periods)
     slices = []
-    for period in simulation_period:
-        sim = sim.sel(time=slice(period[0], period[1]))
+    for period in periods:
+        sim_sel = sim.sel(time=slice(period[0], period[1]))
 
         # adjust
         ADJ = sdba.adjustment.TrainAdjust.from_dataset(dtrain)
 
         if ("detrend" in xclim_adjust_args) and (
             isinstance(xclim_adjust_args["detrend"], dict)
         ):
             name, kwargs = list(xclim_adjust_args["detrend"].items())[0]
             kwargs = kwargs or {}
             kwargs.setdefault("group", ADJ.group)
             kwargs.setdefault("kind", ADJ.kind)
             xclim_adjust_args["detrend"] = getattr(sdba.detrending, name)(**kwargs)
 
         with xc.set_options(sdba_encode_cf=True, sdba_extra_output=False):
-            out = ADJ.adjust(sim, **xclim_adjust_args)
+            out = ADJ.adjust(sim_sel, **xclim_adjust_args)
             slices.extend([out])
     # put all the adjusted period back together
     dscen = xr.concat(slices, dim="time")
 
     _add_preprocessing_attr(dscen, dtrain.attrs["train_params"])
     dscen = xr.Dataset(data_vars={var: dscen}, attrs=dsim.attrs)
     # TODO: History, attrs, etc. (TODO kept from previous version of `biasadjust`)
```

### Comparing `xscen-0.5.0/xscen/catalog.py` & `xscen-0.6.0/xscen/catalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import cftime
 import dask
 import fsspec as fs
 import intake_esm
 import netCDF4
+import numpy as np
 import pandas as pd
 import tlz
 import xarray
 import xarray as xr
 import yaml
 from dask.diagnostics import ProgressBar
 from intake.source.utils import reverse_format
 from intake_esm.cat import ESMCatalogModel
 
 from .config import CONFIG, args_as_str, parse_config, recursive_update
 from .io import get_engine
-from .utils import CV, ensure_correct_time  # noqa
+from .utils import CV, ensure_correct_time, standardize_periods  # noqa
 
 logger = logging.getLogger(__name__)
 # Monkey patch for attribute names in the output of to_dataset_dict
 intake_esm.set_options(attrs_prefix="cat")
 
 
 __all__ = [
@@ -264,14 +265,28 @@
         group, in the same order as the arguments, and the sub-catalog.
         """
         for values in itertools.product(*self.unique(columns)):
             sim = self.search(**dict(zip(columns, values)))
             if sim:  # So we never yield empty catalogs
                 yield values, sim
 
+    def search(self, **columns):
+        """Modification of .search() to add the 'periods' keyword."""
+        periods = columns.pop("periods", False)
+        if len(columns) > 0:
+            cat = super().search(**columns)
+        else:
+            cat = self.__class__({"esmcat": self.esmcat.dict(), "df": self.esmcat._df})
+        if periods is not False:
+            periods = standardize_periods(periods)
+            cat.esmcat._df = subset_file_coverage(
+                cat.esmcat._df, periods=periods, coverage=0, duplicates_ok=True
+            )
+        return cat
+
     def drop_duplicates(self, columns: Optional[List[str]] = None):  # noqa: D102
         # In case variables are being added in an existing Zarr, append them
         if columns is None:
             columns = ["id", "path"]
 
         if len(self.df) > 0:
             # By default, duplicated will mark the later entries as True
@@ -364,15 +379,16 @@
 
         Ensemble preprocessing logic is taken from :py:func:`xclim.ensembles.create_ensemble`.
         When `create_ensemble_on` is given, the function ensures all entries have the correct time coordinate according to `xrfreq`.
 
         Parameters
         ----------
         concat_on : list of strings or str, optional
-          A list of catalog columns over which to concat the datasets (in addition to 'time'). Each will become a new dimension with the column values as coordinates.
+          A list of catalog columns over which to concat the datasets (in addition to 'time').
+          Each will become a new dimension with the column values as coordinates.
           Xarray concatenation rules apply and can be acted upon through `xarray_combine_by_coords_kwargs`.
         create_ensemble_on : list of strings or str, optional
           The given column values will be merged into a new id-like "realization" column, which will be concatenated over.
           The given columns are removed from the dataset id, so as to remove them from the groupby_attrs logic.
           Xarray concatenation rules apply and can be acted upon through `xarray_combine_by_coords_kwargs`.
         calendar : str, optional
           If `create_ensemble_on` is given, all datasets are converted to this calendar before concatenation.
@@ -389,14 +405,16 @@
         See Also
         --------
         intake_esm.core.esm_datastore.to_dataset_dict
         intake_esm.core.esm_datastore.to_dask
         xclim.ensembles.create_ensemble
         """
         cat = deepcopy(self)
+        # Put back what was removed by the copy...
+        cat._requested_variables = self._requested_variables
         preprocess = kwargs.get("preprocess")
 
         if isinstance(concat_on, str):
             concat_on = [concat_on]
         if isinstance(create_ensemble_on, str):
             create_ensemble_on = [create_ensemble_on]
         rm_from_id = (concat_on or []) + (create_ensemble_on or []) + ["realization"]
@@ -451,14 +469,19 @@
             unstacked = unstack_id(cat)
             cat.esmcat.df["id"] = cat.df.apply(
                 lambda row: _build_id(
                     row, [col for col in unstacked[row["id"]] if col not in rm_from_id]
                 ),
                 axis=1,
             )
+
+        if (N := len(cat.keys())) != 1:
+            raise ValueError(
+                f"Expected exactly one dataset, received {N} instead : {cat.keys()}"
+            )
         ds = cat.to_dask(preprocess=preprocess, **kwargs)
         return ds
 
 
 class ProjectCatalog(DataCatalog):
     """A DataCatalog with additional 'write' functionalities that can update and upload itself.
 
@@ -569,14 +592,15 @@
         project : dict-like
             Metadata to create the catalog, if required.
         overwrite : bool
             If this and 'create' are True, this will overwrite any existing JSON and CSV file with an empty catalog.
 
         Notes
         -----
+        New ProjectCatalog must first be created empty, using 'df' as the path to the future JSON file, then populated using .update().
         The dictionary in 'df' must have two keys: ‘esmcat’ and ‘df’.
         The ‘esmcat’ key must be a dict representation of the ESM catalog. This should follow the template used by xscen.catalog.esm_col_data.
         The ‘df’ key must be a Pandas DataFrame containing content that would otherwise be in the CSV file.
         """
         if create:
             if isinstance(df, (str, Path)) and (
                 not os.path.isfile(Path(df)) or overwrite
@@ -1525,7 +1549,109 @@
             raise ValueError(
                 "Not all elements of the columns are the same for a given ID!"
             )
 
         out[ids] = {attr: subset[attr].iloc[0] for attr in subset.columns}
 
     return out
+
+
+def subset_file_coverage(
+    df: pd.DataFrame,
+    periods: list,
+    *,
+    coverage: float = 0.99,
+    duplicates_ok: bool = False,
+) -> pd.DataFrame:
+    """Return a subset of files that overlap with the target periods.
+
+    The minimum resolution for periods is 1 hour.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+      List of files to be evaluated, with at least a date_start and date_end column,
+      which are expected to be `pd.Period` objects with `freq='H'`.
+    periods : list
+      Either [start, end] or list of [start, end] for the periods to be evaluated.
+    coverage : float
+      Percentage of hours that need to be covered in a given period for the dataset to be valid. Use 0 to ignore this checkup.
+    duplicates_ok: bool
+      If True, no checkup is done on possible duplicates.
+
+    Returns
+    -------
+    pd.DataFrame
+      Subset of files that overlap the targetted periods
+    """
+    periods = standardize_periods(periods)
+
+    # Create an Interval for each file
+    file_intervals = df.apply(
+        lambda r: pd.Interval(
+            left=r["date_start"].ordinal, right=r["date_end"].ordinal, closed="both"
+        ),
+        axis=1,
+    )
+
+    # Check for duplicated Intervals
+    if any(file_intervals.duplicated()) and duplicates_ok is False:
+        logging.warning(
+            f"{df['id'].iloc[0] + ': ' if 'id' in df.columns else ''}Time periods are overlapping."
+        )
+        return pd.DataFrame(columns=df.columns)
+
+    # Create an array of True/False
+    files_to_keep = np.zeros(len(file_intervals), dtype=bool)
+    for period in periods:
+        period_interval = pd.Interval(
+            left=date_parser(period[0], freq="H").ordinal,
+            right=date_parser(period[1], end_of_period=True, freq="H").ordinal,
+            closed="both",
+        )
+        files_in_range = file_intervals.apply(lambda r: period_interval.overlaps(r))
+
+        if len(df[files_in_range]) == 0:
+            logging.warning(
+                f"{df['id'].iloc[0] + ': ' if 'id' in df.columns else ''}Insufficient coverage (no files in range)."
+            )
+            return pd.DataFrame(columns=df.columns)
+
+        # Very rough guess of the coverage relative to the requested period,
+        # without having to open the files or checking day-by-day
+        if coverage > 0:
+            # Number of hours in the requested period
+            period_nb_hrs = date_parser(
+                period[1], end_of_period=True, freq="H"
+            ) - date_parser(period[0], freq="H")
+
+            # Sum of hours in all selected files, restricted by the requested period
+            guessed_nb_hrs_sum = (
+                df[files_in_range].apply(
+                    lambda x: np.min(
+                        [
+                            x["date_end"],
+                            date_parser(period[1], end_of_period=True, freq="H"),
+                        ]
+                    ),
+                    axis=1,
+                )
+                - df[files_in_range].apply(
+                    lambda x: np.max(
+                        [x["date_start"], date_parser(period[0], freq="H")]
+                    ),
+                    axis=1,
+                )
+            ).sum()
+
+            if guessed_nb_hrs_sum.nanos / period_nb_hrs.nanos < coverage:
+                logging.warning(
+                    f"{df['id'].iloc[0] + ': ' if 'id' in df.columns else ''}Insufficient coverage "
+                    f"(guessed at {guessed_nb_hrs_sum.nanos / period_nb_hrs.nanos:.1%})."
+                )
+                return pd.DataFrame(columns=df.columns)
+
+            files_to_keep = files_to_keep | files_in_range
+        else:
+            files_to_keep = files_to_keep | files_in_range
+
+    return df[files_to_keep]
```

### Comparing `xscen-0.5.0/xscen/config.py` & `xscen-0.6.0/xscen/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,15 @@
   applies the filter to any warnings. Only built-in warnings are supported.
 """
 import ast
 import builtins
 import collections.abc
 import inspect
 import logging.config
+import types
 import warnings
 from copy import deepcopy
 from functools import wraps
 from pathlib import Path
 from typing import Any, Tuple
 
 import xarray as xr
@@ -209,14 +210,15 @@
             if k in sig.parameters:
                 kwargs.setdefault(k, v)
         if CONFIG.get("print_it_all"):
             logger.debug(f"Modified kwargs : {kwargs}")
 
         return func(*args, **kwargs)
 
+    _wrapper.configurable = True
     if isinstance(func_or_cls, type):
         func_or_cls.__init__ = _wrapper
         return func_or_cls
     _wrapper: func_or_cls  # Fix a decorator bug in Pycharm 2022
     return _wrapper
 
 
@@ -230,7 +232,24 @@
         xr.set_options(**config)
     elif module == "warning":
         for category, action in config.items():
             if category == "all":
                 warnings.simplefilter(action)
             elif issubclass(getattr(builtins, category), builtins.Warning):
                 warnings.simplefilter(action, category=getattr(builtins, category))
+
+
+def get_configurable():
+    """Return a dictionary of all configurable functions and classes of xscen."""
+    import xscen as xs
+
+    configurable = {}
+    for module in dir(xs):
+        modobj = getattr(xs, module)
+        if isinstance(modobj, types.ModuleType):
+            for func in dir(modobj):
+                funcobj = getattr(modobj, func)
+                if getattr(funcobj, "configurable", False) or getattr(
+                    getattr(funcobj, "__init__", None), "configurable", False
+                ):
+                    configurable[f"xscen.{module}.{func}"] = funcobj
+    return configurable
```

### Comparing `xscen-0.5.0/xscen/data/IPCC_annual_global_tas.csv` & `xscen-0.6.0/xscen/data/IPCC_annual_global_tas.csv`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/xscen/diagnostics.py` & `xscen-0.6.0/xscen/diagnostics.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import xarray as xr
 from xclim.core.indicator import Indicator
 
 from .catalog import DataCatalog
 from .config import parse_config
 from .indicators import load_xclim_module
 from .io import save_to_zarr
-from .utils import change_units, unstack_fill_nan
+from .utils import change_units, clean_up, standardize_periods, unstack_fill_nan
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "fix_unphysical_values",
     "properties_and_measures",
     "measures_heatmap",
@@ -125,15 +125,15 @@
     ----------
     ds : xr.Dataset
         Input dataset.
     properties : Union[str, PosixPath, Sequence[Indicator], Sequence[Tuple[str, Indicator]]]
         Path to a YAML file that instructs on how to calculate properties.
         Can be the indicator module directly, or a sequence of indicators or a sequence of
         tuples (indicator name, indicator) as returned by `iter_indicators()`.
-    period : lst
+    period : list
         [start, end] of the period to be evaluated. The period will be selected on ds
         and dref_for_measure if it is given.
     unstack : bool
         Whether to unstack ds before computing the properties.
     rechunk : dict
         Dictionary of chunks to use for a rechunk before computing the properties.
     dref_for_measure : xr.Dataset
@@ -172,27 +172,26 @@
     try:
         N = len(properties)
     except TypeError:
         N = None
     else:
         logger.info(f"Computing {N} properties.")
 
+    period = standardize_periods(period, multiple=False)
     # select period for ds
     if period is not None and "time" in ds:
-        ds = ds.sel({"time": slice(str(period[0]), str(period[1]))})
+        ds = ds.sel({"time": slice(period[0], period[1])})
 
     # select periods for ref_measure
     if (
         dref_for_measure is not None
         and period is not None
         and "time" in dref_for_measure
     ):
-        dref_for_measure = dref_for_measure.sel(
-            {"time": slice(str(period[0]), str(period[1]))}
-        )
+        dref_for_measure = dref_for_measure.sel({"time": slice(period[0], period[1])})
 
     if unstack:
         ds = unstack_fill_nan(ds)
 
     if rechunk:
         ds = ds.chunk(rechunk)
 
@@ -208,15 +207,15 @@
             iden = ind.identifier
         # Make the call to xclim
         logger.info(f"{i} - Computing {iden}.")
         out = ind(ds=ds)
         vname = out.name
         prop[vname] = out
 
-        if period:
+        if period is not None:
             prop[vname].attrs["period"] = f"{period[0]}-{period[1]}"
 
         # calculate the measure if a reference dataset is given for the measure
         if dref_for_measure and vname in dref_for_measure:
             meas[vname] = ind.get_measure()(
                 sim=prop[vname], ref=dref_for_measure[vname]
             )
@@ -290,30 +289,34 @@
             if np.max(c) != np.min(c)
             else [0.5] * len(c)
             for c in hmap.T
         ]
     ).T
 
     name_of_datasets = name_of_datasets or list(range(1, hmap.shape[0] + 1))
-
     ds_hmap = xr.DataArray(
         hmap,
         coords={
-            "datasets": name_of_datasets,
+            "realization": name_of_datasets,
             "properties": list(meas_datasets[0].data_vars),
         },
-        dims=["datasets", "properties"],
+        dims=["realization", "properties"],
     )
     ds_hmap = ds_hmap.to_dataset(name="heatmap")
 
     ds_hmap.attrs = xr.core.merge.merge_attrs(
         [ds.attrs for ds in meas_datasets], combine_attrs="drop_conflicts"
     )
+    ds_hmap = clean_up(
+        ds=ds_hmap,
+        common_attrs_only=meas_datasets,
+    )
     ds_hmap.attrs["cat:processing_level"] = to_level
     ds_hmap.attrs.pop("cat:variable", None)
+    ds_hmap["heatmap"].attrs["long_name"] = "Ranking of measure performance"
 
     return ds_hmap
 
 
 def measures_improvement(
     meas_datasets: Union[list, dict], to_level: str = "diag-improved"
 ):
@@ -361,12 +364,54 @@
 
     ds_better = xr.DataArray(
         percent_better, coords={"properties": list(ds2.data_vars)}, dims="properties"
     )
 
     ds_better = ds_better.to_dataset(name="improved_grid_points")
 
+    ds_better["improved_grid_points"].attrs[
+        "long_name"
+    ] = "Fraction of improved grid cells"
     ds_better.attrs = ds2.attrs
     ds_better.attrs["cat:processing_level"] = to_level
     ds_better.attrs.pop("cat:variable", None)
 
     return ds_better
+
+
+def measures_improvement_2d(dict_input: dict, to_level: str = "diag-improved-2d"):
+    """
+    Create a 2D dataset with dimension `realization` showing the fraction of improved grid cell.
+
+    Parameters
+    ----------
+    dict_input: dict
+      If dict of datasets, the datasets should be the output of `measures_improvement`.
+      If dict of dict/list, the dict/list should be the input to `measures_improvement`.
+      The keys will be the values of the dimension `realization`.
+    to_level: str
+      Processing_level to assign to the output dataset.
+
+    Returns
+    -------
+    xr.Dataset
+      Dataset with extra `realization` coordinates.
+    """
+    merge = {}
+    for name, value in dict_input.items():
+        # if dataset, assume the value is already the output of `measures_improvement`
+        if isinstance(value, xr.Dataset):
+            out = value.expand_dims(dim={"realization": [name]})
+        # else, compute the `measures_improvement`
+        else:
+            out = measures_improvement(value).expand_dims(dim={"realization": [name]})
+        merge[name] = out
+    # put everything in one dataset with dim datasets
+    ds_merge = xr.concat(list(merge.values()), dim="realization")
+    ds_merge["realization"] = ds_merge["realization"].astype(str)
+    ds_merge = clean_up(
+        ds=ds_merge,
+        common_attrs_only=merge,
+    )
+    ds_merge.attrs["cat:processing_level"] = to_level
+
+    return ds_merge
```

### Comparing `xscen-0.5.0/xscen/ensembles.py` & `xscen-0.6.0/xscen/ensembles.py`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/xscen/extract.py` & `xscen-0.6.0/xscen/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # noqa: D100
 import datetime
 import logging
 import os
 import re
+import warnings
+from collections import defaultdict
 from copy import deepcopy
 from pathlib import Path
 from typing import Callable, List, Optional, Union
 
-import clisops.core.subset
 import numpy as np
 import pandas as pd
 import xarray as xr
 import xclim as xc
 from intake_esm.derived import DerivedVariableRegistry
 
 from .catalog import DataCatalog  # noqa
 from .catalog import (
     ID_COLUMNS,
     concat_data_catalogs,
-    date_parser,
     generate_id,
     parse_from_ds,
+    subset_file_coverage,
 )
 from .config import parse_config
 from .indicators import load_xclim_module, registry_from_module
+from .spatial import subset
 from .utils import CV
 from .utils import ensure_correct_time as _ensure_correct_time
-from .utils import natural_sort
+from .utils import natural_sort, standardize_periods
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
-    "clisops_subset",
     "extract_dataset",
     "resample",
     "search_data_catalogs",
     "subset_warming_level",
 ]
 
 
@@ -65,78 +66,21 @@
     xr.Dataset
         Subsetted Dataset.
 
     See Also
     --------
     clisops.core.subset.subset_gridpoint, clisops.core.subset.subset_bbox, clisops.core.subset.subset_shape
     """
-    if "buffer" in region.keys():
-        # estimate the model resolution
-        if len(ds.lon.dims) == 1:  # 1D lat-lon
-            lon_res = np.abs(ds.lon.diff("lon")[0].values)
-            lat_res = np.abs(ds.lat.diff("lat")[0].values)
-        else:
-            lon_res = np.abs(ds.lon[0, 0].values - ds.lon[0, 1].values)
-            lat_res = np.abs(ds.lat[0, 0].values - ds.lat[1, 0].values)
-
-    kwargs = deepcopy(region[region["method"]])
-
-    if region["method"] in ["gridpoint"]:
-        ds_subset = clisops.core.subset_gridpoint(ds, **kwargs)
-        new_history = (
-            f"[{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}] "
-            f"{region['method']} spatial subsetting on {len(region['gridpoint']['lon'])} coordinates - clisops v{clisops.__version__}"
-        )
-
-    elif region["method"] in ["bbox"]:
-        if "buffer" in region.keys():
-            # adjust the boundaries
-            kwargs["lon_bnds"] = (
-                kwargs["lon_bnds"][0] - lon_res * region["buffer"],
-                kwargs["lon_bnds"][1] + lon_res * region["buffer"],
-            )
-            kwargs["lat_bnds"] = (
-                kwargs["lat_bnds"][0] - lat_res * region["buffer"],
-                kwargs["lat_bnds"][1] + lat_res * region["buffer"],
-            )
-
-        if xc.core.utils.uses_dask(ds.cf["longitude"]):
-            ds[ds.cf["longitude"].name].load()
-        if xc.core.utils.uses_dask(ds.cf["latitude"]):
-            ds[ds.cf["latitude"].name].load()
-
-        ds_subset = clisops.core.subset_bbox(ds, **kwargs)
-        new_history = (
-            f"[{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}] "
-            f"{region['method']} spatial subsetting with {'buffer=' + str(region['buffer']) if 'buffer' in region else 'no buffer'}"
-            f", lon_bnds={np.array(region['bbox']['lon_bnds'])}, lat_bnds={np.array(region['bbox']['lat_bnds'])}"
-            f" - clisops v{clisops.__version__}"
-        )
-
-    elif region["method"] in ["shape"]:
-        if "buffer" in region.keys():
-            kwargs["buffer"] = np.max([lon_res, lat_res]) * region["buffer"]
-
-        ds_subset = clisops.core.subset_shape(ds, **kwargs)
-        new_history = (
-            f"[{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}] "
-            f"{region['method']} spatial subsetting with {'buffer=' + str(region['buffer']) if 'buffer' in region else 'no buffer'}"
-            f", shape={Path(region['shape']['shape']).name if isinstance(region['shape']['shape'], (str, Path)) else 'gpd.GeoDataFrame'}"
-            f" - clisops v{clisops.__version__}"
-        )
-
-    else:
-        raise ValueError("Subsetting type not recognized")
-
-    history = (
-        new_history + " \n " + ds_subset.attrs["history"]
-        if "history" in ds_subset.attrs
-        else new_history
+    warnings.warn(
+        "clisops_subset is deprecated and will not be available in future versions. "
+        "Use xscen.spatial.subset instead.",
+        category=FutureWarning,
     )
-    ds_subset.attrs["history"] = history
+
+    ds_subset = subset(ds, region=region)
 
     return ds_subset
 
 
 @parse_config
 def extract_dataset(
     catalog: DataCatalog,
@@ -146,32 +90,33 @@
     region: Optional[dict] = None,
     to_level: str = "extracted",
     ensure_correct_time: bool = True,
     xr_open_kwargs: dict = None,
     xr_combine_kwargs: dict = None,
     preprocess: Callable = None,
     resample_methods: Optional[dict] = None,
+    mask: Union[bool, xr.Dataset, xr.DataArray] = False,
 ) -> Union[dict, xr.Dataset]:
     """Take one element of the output of `search_data_catalogs` and returns a dataset, performing conversions and resampling as needed.
 
     Nothing is written to disk within this function.
 
     Parameters
     ----------
     catalog : DataCatalog
         Sub-catalog for a single dataset, one value of the output of `search_data_catalogs`.
     variables_and_freqs : dict
-        Variables and freqs, following a 'variable: xrfreq-compatible str' format.
+        Variables and freqs, following a 'variable: xrfreq-compatible str' format. A list of strings can also be provided.
         If None, it will be read from catalog._requested_variables and catalog._requested_variable_freqs
         (set by `variables_and_freqs` in `search_data_catalogs`)
     periods : list
-        [start, end] of the period to be evaluated (or a list of lists)
+        Either [start, end] or list of [start, end] for the periods to be evaluated.
         Will be read from catalog._requested_periods if None. Leave both None to extract everything.
     region : dict, optional
-        Description of the region and the subsetting method (required fields listed in the Notes).
+        Description of the region and the subsetting method (required fields listed in the Notes) used in `xscen.spatial.subset`.
     to_level : str
         The processing level to assign to the output.
         Defaults to 'extracted'
     ensure_correct_time : bool
         When True (default), even if the data has the correct frequency, its time coordinate is
         checked so that it exactly matches the frequency code (xrfreq). For example, daily data given at
         noon would be transformed to be given at midnight. If the time coordinate is invalid,
@@ -186,33 +131,39 @@
         If provided, call this function on each dataset prior to aggregation.
     resample_methods : dict, optional
         Dictionary where the keys are the variables and the values are the resampling method.
         Options for the resampling method are {'mean', 'min', 'max', 'sum', 'wind_direction'}.
         If the method is not given for a variable, it is guessed from the variable name and frequency,
         using the mapping in CVs/resampling_methods.json. If the variable is not found there,
         "mean" is used by default.
+    mask: xr.Dataset, bool
+        A mask that is applied to all variables and only keeps data where it is True.
+        Where the mask is False, variable values are replaced by NaNs.
+        The mask should have the same dimensions as the variables extracted.
+        If `mask` is a dataset, the dataset should have a variable named 'mask'.
+        If `mask` is True, it will expect a `mask` variable at xrfreq `fx` to have been extracted.
 
     Returns
     -------
     dict, xr.Dataset
         Dictionary (keys = xrfreq) with datasets containing all available and computed variables,
         subsetted to the region, everything resampled to the requested frequency.
         If there is a single frequency, a Dataset will be returned instead.
 
     Notes
     -----
     'region' fields:
         name: str
             Region name used to overwrite domain in the catalog.
         method: str
-            ['gridpoint', 'bbox', shape']
-        <method>: dict
-            Arguments specific to the method used.
-        buffer: float, optional
+            ['gridpoint', 'bbox', shape', 'sel']
+        tile_buffer: float, optional
             Multiplier to apply to the model resolution.
+        kwargs
+            Arguments specific to the method used.
 
     See Also
     --------
     intake_esm.core.esm_datastore.to_dataset_dict, xarray.open_dataset, xarray.combine_by_coords
     """
     resample_methods = resample_methods or {}
 
@@ -226,21 +177,27 @@
     if region is None and len(unique["domain"]) > 1:
         raise ValueError(
             "If a subset region is not given, the extraction catalog must have a unique domain."
         )
 
     if variables_and_freqs is None:
         try:
-            variables_and_freqs = dict(
-                zip(
-                    catalog._requested_variables_true, catalog._requested_variable_freqs
-                )
-            )
+            variables_and_freqs = defaultdict(list)
+            for a, b in zip(
+                catalog._requested_variables_true, catalog._requested_variable_freqs
+            ):
+                variables_and_freqs[a].extend([b])
         except ValueError:
             raise ValueError("Failed to determine the requested variables and freqs.")
+    else:
+        # Make everything a list
+        variables_and_freqs = {
+            k: [v] if not isinstance(v, list) else v
+            for k, v in variables_and_freqs.items()
+        }
 
     # Default arguments to send xarray
     xr_open_kwargs = xr_open_kwargs or {}
     xr_combine_kwargs = xr_combine_kwargs or {}
     xr_combine_kwargs.setdefault("data_vars", "minimal")
 
     # Open the catalog
@@ -249,42 +206,47 @@
         xarray_combine_by_coords_kwargs=xr_combine_kwargs,
         preprocess=preprocess,
         # Only print a progress bar when it is minimally useful
         progressbar=(len(catalog.keys()) > 1),
     )
 
     out_dict = {}
-    for xrfreq in pd.unique(list(variables_and_freqs.values())):
+    for xrfreq in pd.unique([x for y in variables_and_freqs.values() for x in y]):
         ds = xr.Dataset()
         attrs = {}
         # iterate on the datasets, in reverse timedelta order
         for key, ds_ts in sorted(
             ds_dict.items(),
-            key=lambda kv: CV.xrfreq_to_timedelta(
-                catalog[kv[0]].df.xrfreq.iloc[0], default="NAN"
+            key=lambda kv: pd.Timedelta(
+                CV.xrfreq_to_timedelta(catalog[kv[0]].df.xrfreq.iloc[0], default="NAN")
             ),
             reverse=True,
         ):
-            if "time" in ds_ts and ensure_correct_time:
-                # Expected freq (xrfreq is the wanted freq)
-                expfreq = catalog[key].df.xrfreq.iloc[0]
-                ds_ts = _ensure_correct_time(ds_ts, expfreq)
+            if "time" in ds_ts:
+                if pd.Timedelta(
+                    CV.xrfreq_to_timedelta(catalog[key].df.xrfreq.iloc[0])
+                ) > pd.Timedelta(CV.xrfreq_to_timedelta(xrfreq)):
+                    continue
+                if ensure_correct_time:
+                    # Expected freq (xrfreq is the wanted freq)
+                    expfreq = catalog[key].df.xrfreq.iloc[0]
+                    ds_ts = _ensure_correct_time(ds_ts, expfreq)
 
             for var_name, da in ds_ts.data_vars.items():
                 # Support for grid_mapping, crs, and other such variables
                 if len(da.dims) == 0 and var_name not in ds:
                     if bool(re.search("^|S[0-9]{1,4}$", str(da.dtype))):
                         da = da.astype("U")
                     ds = ds.assign({var_name: da})
                     continue
 
                 # TODO: 2nd part is a temporary fix until this is changed in intake_esm
                 if (
                     var_name in ds
-                    or variables_and_freqs.get(var_name) != xrfreq
+                    or xrfreq not in variables_and_freqs.get(var_name, [])
                     or var_name not in catalog._requested_variables_true
                 ):
                     continue
 
                 # TODO: This is a temporary fix for an xclim bug where the grid_mapping attribute is not transferred upon calculation
                 if (
                     var_name in catalog.derivedcat
@@ -306,32 +268,30 @@
                     )
                     if len(grid_mapping) == 1:
                         da.attrs["grid_mapping"] = grid_mapping[0]
                     elif len(grid_mapping) > 1:
                         raise ValueError("Multiple grid_mapping detected.")
 
                 if "time" not in da.dims or (
-                    catalog[key].df["xrfreq"].iloc[0] == variables_and_freqs[var_name]
+                    catalog[key].df["xrfreq"].iloc[0] == xrfreq
                 ):
                     ds = ds.assign({var_name: da})
                 else:  # check if it needs resampling
                     if pd.to_timedelta(
                         CV.xrfreq_to_timedelta(catalog[key].df["xrfreq"].iloc[0])
-                    ) < pd.to_timedelta(
-                        CV.xrfreq_to_timedelta(variables_and_freqs[var_name])
-                    ):
+                    ) < pd.to_timedelta(CV.xrfreq_to_timedelta(xrfreq)):
                         logger.info(
                             f"Resampling {var_name} from [{catalog[key].df['xrfreq'].iloc[0]}]"
-                            f" to [{variables_and_freqs[var_name]}]."
+                            f" to [{xrfreq}]."
                         )
                         ds = ds.assign(
                             {
                                 var_name: resample(
                                     da,
-                                    variables_and_freqs[var_name],
+                                    xrfreq,
                                     ds=ds_ts,
                                     method=resample_methods.get(var_name, None),
                                 )
                             }
                         )
                     else:
                         raise ValueError(
@@ -345,36 +305,68 @@
             ds.attrs["cat:frequency"] = "fx"
             ds.attrs["cat:xrfreq"] = "fx"
         else:
             ds.attrs["cat:xrfreq"] = xrfreq
             ds.attrs["cat:frequency"] = CV.xrfreq_to_frequency(xrfreq)
 
         # Subset time on the periods
-        if periods is None and hasattr(catalog, "_requested_periods"):
-            periods = catalog._requested_periods
-        if periods is not None and "time" in ds:
-            if not isinstance(periods[0], list):
-                periods = [periods]
+        periods_extract = deepcopy(periods)
+        if periods_extract is None and hasattr(catalog, "_requested_periods"):
+            periods_extract = catalog._requested_periods
+        if periods_extract is not None and "time" in ds:
+            periods_extract = standardize_periods(periods_extract)
             slices = []
-            for period in periods:
-                slices.extend([ds.sel({"time": slice(str(period[0]), str(period[1]))})])
+            for period in periods_extract:
+                slices.extend([ds.sel({"time": slice(period[0], period[1])})])
             ds = xr.concat(slices, dim="time", **xr_combine_kwargs)
 
-        # Custom call to clisops
+        # subset to the region
         if region is not None:
-            ds = clisops_subset(ds, region)
-            ds.attrs["cat:domain"] = region["name"]
+            if (region["method"] in region) and (
+                isinstance(region[region["method"]], dict)
+            ):
+                warnings.warn(
+                    "You seem to be using a deprecated version of region. Please use the new formatting.",
+                    category=FutureWarning,
+                )
+                region = deepcopy(region)
+                if "buffer" in region:
+                    region["tile_buffer"] = region.pop("buffer")
+                _kwargs = region.pop(region["method"])
+                region.update(_kwargs)
+
+            ds = subset(ds, **region)
 
         # add relevant attrs
         ds.attrs["cat:processing_level"] = to_level
         if "cat:variable" not in ds.attrs:
             ds.attrs["cat:variable"] = parse_from_ds(ds, ["variable"])["variable"]
 
         out_dict[xrfreq] = ds
 
+    if mask:
+        if isinstance(mask, xr.Dataset):
+            ds_mask = mask["mask"]
+        elif isinstance(mask, xr.DataArray):
+            ds_mask = mask
+        elif (
+            "fx" in out_dict and "mask" in out_dict["fx"]
+        ):  # get mask that was extracted above
+            ds_mask = out_dict["fx"]["mask"].copy()
+        else:
+            raise ValueError(
+                "No mask found. Either pass a xr.Dataset/xr.DataArray to the `mask` argument or pass a `dc` that includes a dataset with a variable named `mask`."
+            )
+
+        # iter over all xrfreq to apply the mask
+        for xrfreq, ds in out_dict.items():
+            out_dict[xrfreq] = ds.where(ds_mask)
+            if xrfreq == "fx":  # put back the mask
+                out_dict[xrfreq]["mask"] = ds_mask
+
     return out_dict
 
 
 def resample(
     da: xr.DataArray,
     target_frequency: str,
     *,
@@ -401,14 +393,29 @@
     -------
     xr.DataArray
         Resampled variable
 
     """
     var_name = da.name
 
+    initial_frequency = xr.infer_freq(da.time.dt.round("T")) or "undetected"
+    initial_frequency_td = pd.Timedelta(
+        CV.xrfreq_to_timedelta(xr.infer_freq(da.time.dt.round("T")), None)
+    )
+    if initial_frequency_td == pd.Timedelta("1D"):
+        logger.warning(
+            "You appear to be resampling daily data using extract_dataset. "
+            "It is advised to use compute_indicators instead, as it is far more robust."
+        )
+    elif initial_frequency_td > pd.Timedelta("1D"):
+        logger.warning(
+            "You appear to be resampling data that is coarser than daily. "
+            "Be aware that this is not currently explicitely supported by xscen and might result in erroneous manipulations."
+        )
+
     if method is None:
         if (
             target_frequency in CV.resampling_methods.dict
             and var_name in CV.resampling_methods.dict[target_frequency]
         ):
             method = CV.resampling_methods(target_frequency)[var_name]
             logger.info(
@@ -473,16 +480,14 @@
             out = ds[var_name]
 
     else:
         out = getattr(da.resample(time=target_frequency), method)(
             dim="time", keep_attrs=True
         )
 
-    initial_frequency = xr.infer_freq(da.time.dt.round("T")) or "undetected"
-
     new_history = (
         f"[{datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')}] {method} "
         f"resample from {initial_frequency} to {target_frequency} - xarray v{xr.__version__}"
     )
     history = (
         new_history + " \n " + out.attrs["history"]
         if "history" in out.attrs
@@ -500,14 +505,15 @@
     ],
     variables_and_freqs: dict,
     *,
     other_search_criteria: Optional[dict] = None,
     exclusions: dict = None,
     match_hist_and_fut: bool = False,
     periods: list = None,
+    coverage_kwargs: dict = None,
     id_columns: Optional[List[str]] = None,
     allow_resampling: bool = False,
     allow_conversion: bool = False,
     conversion_yaml: str = None,
     restrict_resolution: str = None,
     restrict_members: dict = None,
     restrict_warming_level: Union[dict, bool] = None,
@@ -515,23 +521,25 @@
     """Search through DataCatalogs.
 
     Parameters
     ----------
     data_catalogs : Union[Union[str, os.PathLike], List[Union[str, os.PathLike]], DataCatalog]
         DataCatalog (or multiple, in a list) or paths to JSON/CSV data catalogs. They must use the same columns and aggregation options.
     variables_and_freqs : dict
-        Variables and freqs to search for, following a 'variable: xr-freq-compatible-str' format.
+        Variables and freqs to search for, following a 'variable: xr-freq-compatible-str' format. A list of strings can also be provided.
     other_search_criteria : dict, optional
         Other criteria to search for in the catalogs' columns, following a 'column_name: list(subset)' format.
     exclusions : dict, optional
         Same as other_search_criteria, but for eliminating results.
     match_hist_and_fut: bool, optional
         If True, historical and future simulations will be combined into the same line, and search results lacking one of them will be rejected.
     periods : list
-        [start, end] of the period to be evaluated (or a list of lists).
+        Either [start, end] or list of [start, end] for the periods to be evaluated.
+    coverage_kwargs : dict
+        Arguments to pass to subset_file_coverage (only used when periods is not None).
     id_columns : list, optional
         List of columns used to create a id column. If None is given, the original
         "id" is left.
     allow_resampling : bool
          If True (default), variables with a higher time resolution than requested are considered.
     allow_conversion : bool
         If True (default) and if the requested variable cannot be found, intermediate variables are
@@ -653,139 +661,155 @@
             # Only fill in the missing IDs
             catalog.df["id"] = catalog.df["id"].fillna(ids)
 
     if catalog.df.empty:
         logger.warning("Found no match corresponding to the 'other' search criteria.")
         return {}
 
+    coverage_kwargs = coverage_kwargs or {}
+    periods = standardize_periods(periods)
+
     logger.info(f"Iterating over {len(catalog.unique('id'))} potential datasets.")
     # Loop on each dataset to assess whether they have all required variables
     # And select best freq/timedelta for each
     catalogs = {}
     if len(catalog) > 0:
         for (sim_id,), scat in catalog.iter_unique("id"):
             # Find all the entries that match search parameters
             varcats = []
-            for var_id, xrfreq in variables_and_freqs.items():
-                if xrfreq == "fx":
-                    varcat = scat.search(
-                        xrfreq=xrfreq,
-                        variable=var_id,
-                        require_all_on=["id", "xrfreq"],
-                    )
-                    if len(varcat) == 0:
-                        # Try searching in other experiments or members
-                        scat_id = {
-                            i: scat.df[i].iloc[0]
-                            for i in id_columns or ID_COLUMNS
-                            if i in scat.df.columns
-                        }
-                        scat_id.pop("experiment", None)
-                        scat_id.pop("member", None)
-                        varcat = catalog.search(
-                            **scat_id,
+            for var_id, xrfreqs in variables_and_freqs.items():
+                if isinstance(xrfreqs, str):
+                    xrfreqs = [xrfreqs]
+                for xrfreq in xrfreqs:
+                    if xrfreq == "fx":
+                        varcat = scat.search(
                             xrfreq=xrfreq,
                             variable=var_id,
                             require_all_on=["id", "xrfreq"],
                         )
-                        if len(varcat) > 1:
-                            varcat.esmcat._df = varcat.df.iloc[[0]]
-                        if len(varcat) == 1:
-                            logger.warning(
-                                f"Dataset {sim_id} doesn't have the fixed field {var_id}, but it can be acquired from {varcat.df['id'].iloc[0]}."
+                        if len(varcat) == 0:
+                            # Try searching in other experiments or members
+                            scat_id = {
+                                i: scat.df[i].iloc[0]
+                                for i in id_columns or ID_COLUMNS
+                                if i in scat.df.columns
+                            }
+                            scat_id.pop("experiment", None)
+                            scat_id.pop("member", None)
+                            varcat = catalog.search(
+                                **scat_id,
+                                xrfreq=xrfreq,
+                                variable=var_id,
+                                require_all_on=["id", "xrfreq"],
+                            )
+                            if len(varcat) > 1:
+                                varcat.esmcat._df = varcat.df.iloc[[0]]
+                            if len(varcat) == 1:
+                                logger.warning(
+                                    f"Dataset {sim_id} doesn't have the fixed field {var_id}, but it can be acquired from {varcat.df['id'].iloc[0]}."
+                                )
+                                for i in {"member", "experiment", "id"}.intersection(
+                                    varcat.df.columns
+                                ):
+                                    varcat.df.loc[:, i] = scat.df[i].iloc[0]
+
+                        # TODO: Temporary fix until this is changed in intake_esm
+                        varcat._requested_variables_true = [var_id]
+                        varcat._dependent_variables = list(
+                            set(varcat._requested_variables).difference(
+                                varcat._requested_variables_true
                             )
-                            for i in {"member", "experiment", "id"}.intersection(
-                                varcat.df.columns
-                            ):
-                                varcat.df.loc[:, i] = scat.df[i].iloc[0]
-
-                    # TODO: Temporary fix until this is changed in intake_esm
-                    varcat._requested_variables_true = [var_id]
-                    varcat._dependent_variables = list(
-                        set(varcat._requested_variables).difference(
-                            varcat._requested_variables_true
                         )
-                    )
-                else:
-                    # TODO: Add support for DerivedVariables that themselves require DerivedVariables
-                    # TODO: Add support for DerivedVariables that exist on different frequencies (e.g. 1hr 'pr' & 3hr 'tas')
-                    varcat = scat.search(
-                        variable=var_id, require_all_on=["id", "xrfreq"]
-                    )
-                    logger.debug(
-                        f"At var {var_id}, after search cat has {varcat.derivedcat.keys()}"
-                    )
-                    # TODO: Temporary fix until this is changed in intake_esm
-                    varcat._requested_variables_true = [var_id]
-                    varcat._dependent_variables = list(
-                        set(varcat._requested_variables).difference(
-                            varcat._requested_variables_true
+                    else:
+                        # TODO: Add support for DerivedVariables that themselves require DerivedVariables
+                        # TODO: Add support for DerivedVariables that exist on different frequencies (e.g. 1hr 'pr' & 3hr 'tas')
+                        varcat = scat.search(
+                            variable=var_id, require_all_on=["id", "xrfreq"]
+                        )
+                        logger.debug(
+                            f"At var {var_id}, after search cat has {varcat.derivedcat.keys()}"
+                        )
+                        # TODO: Temporary fix until this is changed in intake_esm
+                        varcat._requested_variables_true = [var_id]
+                        varcat._dependent_variables = list(
+                            set(varcat._requested_variables).difference(
+                                varcat._requested_variables_true
+                            )
                         )
-                    )
 
-                    # We want to match lines with the correct freq,
-                    # IF allow_resampling is True and xrfreq translates to a timedelta,
-                    # we also want those with (stricyly) higher temporal resolution
-                    same_frq = varcat.df.xrfreq == xrfreq
-                    td = pd.to_timedelta(CV.xrfreq_to_timedelta(xrfreq))
-                    varcat.df["timedelta"] = pd.to_timedelta(
-                        varcat.df.xrfreq.apply(CV.xrfreq_to_timedelta, default="NAN")
-                    )
-                    # else is joker (any timedelta)
-                    lower_frq = (
-                        np.less(varcat.df.timedelta, td) if pd.notnull(td) else False
-                    )
-                    varcat.esmcat._df = varcat.df[
-                        same_frq | (lower_frq & allow_resampling)
-                    ]
+                        # We want to match lines with the correct freq,
+                        # IF allow_resampling is True and xrfreq translates to a timedelta,
+                        # we also want those with (stricyly) higher temporal resolution
+                        same_frq = varcat.df.xrfreq == xrfreq
+                        td = pd.to_timedelta(CV.xrfreq_to_timedelta(xrfreq))
+                        varcat.df["timedelta"] = pd.to_timedelta(
+                            varcat.df.xrfreq.apply(
+                                CV.xrfreq_to_timedelta, default="NAN"
+                            )
+                        )
+                        # else is joker (any timedelta)
+                        lower_frq = (
+                            np.less(varcat.df.timedelta, td)
+                            if pd.notnull(td)
+                            else False
+                        )
+                        varcat.esmcat._df = varcat.df[
+                            same_frq | (lower_frq & allow_resampling)
+                        ]
 
-                    # For each dataset (id - xrfreq - processing_level - domain - variable), make sure that file availability covers the requested time periods
-                    if periods is not None and len(varcat) > 0:
-                        valid_tp = []
-                        for var, group in varcat.df.groupby(
-                            varcat.esmcat.aggregation_control.groupby_attrs
-                            + ["variable"]
-                        ):
-                            valid_tp.append(
-                                _subset_file_coverage(group, periods)
-                            )  # If valid, this returns the subset of files that cover the time period
-                        varcat.esmcat._df = pd.concat(valid_tp)
-
-                    # We now select the coarsest timedelta for each variable
-                    # we need to re-iterate over variables in case we used the registry (and thus there are multiple variables in varcat)
-                    rows = []
-                    for var, group in varcat.df.groupby("variable"):
-                        rows.append(group[group.timedelta == group.timedelta.max()])
-                    if rows:
-                        # check if the requested variable exists and if so, remove DeriveVariable references
-                        v_list = [rows[i]["variable"].iloc[0] for i in range(len(rows))]
-                        v_list_check = [
-                            var_id in v_list[i] for i in range(len(v_list))
-                        ]  # necessary in case a file has multiple variables
-                        if any(v_list_check):
-                            rows = [rows[v_list_check.index(True)]]
-                            varcat.derivedcat = DerivedVariableRegistry()
-                        varcat.esmcat._df = pd.concat(rows, ignore_index=True)
-                    else:
-                        varcat.esmcat._df = pd.DataFrame()
+                        # For each dataset (id - xrfreq - processing_level - domain - variable), make sure that file availability covers the requested time periods
+                        if periods is not None and len(varcat) > 0:
+                            valid_tp = []
+                            for var, group in varcat.df.groupby(
+                                varcat.esmcat.aggregation_control.groupby_attrs
+                                + ["variable"]
+                            ):
+                                valid_tp.append(
+                                    subset_file_coverage(
+                                        group, periods, **coverage_kwargs
+                                    )
+                                )  # If valid, this returns the subset of files that cover the time period
+                            varcat.esmcat._df = pd.concat(valid_tp)
+
+                        # We now select the coarsest timedelta for each variable
+                        # we need to re-iterate over variables in case we used the registry (and thus there are multiple variables in varcat)
+                        rows = []
+                        for var, group in varcat.df.groupby("variable"):
+                            rows.append(group[group.timedelta == group.timedelta.max()])
+                        if rows:
+                            # check if the requested variable exists and if so, remove DeriveVariable references
+                            v_list = [
+                                rows[i]["variable"].iloc[0] for i in range(len(rows))
+                            ]
+                            v_list_check = [
+                                var_id in v_list[i] for i in range(len(v_list))
+                            ]  # necessary in case a file has multiple variables
+                            if any(v_list_check):
+                                rows = [rows[v_list_check.index(True)]]
+                                varcat.derivedcat = DerivedVariableRegistry()
+                            varcat.esmcat._df = pd.concat(rows, ignore_index=True)
+                        else:
+                            varcat.esmcat._df = pd.DataFrame()
+
+                    if varcat.df.empty:
+                        logger.debug(
+                            f"Dataset {sim_id} doesn't have all needed variables (missing at least {var_id})."
+                        )
+                        break
+                    if "timedelta" in varcat.df.columns:
+                        varcat.df.drop(columns=["timedelta"], inplace=True)
+                    varcat._requested_variable_freqs = [xrfreq]
+                    varcats.append(varcat)
 
-                if varcat.df.empty:
-                    logger.debug(
-                        f"Dataset {sim_id} doesn't have all needed variables (missing at least {var_id})."
-                    )
-                    break
-                if "timedelta" in varcat.df.columns:
-                    varcat.df.drop(columns=["timedelta"], inplace=True)
-                varcat._requested_variable_freqs = [xrfreq]
-                varcats.append(varcat)
+                else:
+                    continue
+                break
             else:
                 catalogs[sim_id] = concat_data_catalogs(*varcats)
                 if periods is not None:
-                    if not isinstance(periods[0], list):
-                        periods = [periods]
                     catalogs[sim_id]._requested_periods = periods
 
     if len(catalogs) > 0:
         logger.info(
             f"Found {len(catalogs)} with all variables requested and corresponding to the criteria."
         )
     else:
@@ -822,15 +846,15 @@
        'cat:source' for global models or 'cat:driving_model' for regional models.
     wl : float
        Warming level.
        eg. 2 for a global warming level of +2 degree Celsius above the mean temperature of the `tas_baseline_period`.
     window : int
        Size of the rolling window in years over which to compute the warming level.
     tas_baseline_period : list
-       Base period. The warming is calculated with respect to this period. The default is ["1850", "1900"].
+       [start, end] of the base period. The warming is calculated with respect to it. The default is ["1850", "1900"].
     ignore_member : bool
        Whether to ignore the member when searching for the model run in tas_csv.
     tas_csv : str
        Path to a csv of annual global mean temperature with a row for each year and a column for each dataset.
        If None, it will default to data/IPCC_annual_global_tas.csv which was built from
        the IPCC atlas data from  Iturbide et al., 2020 (https://doi.org/10.5194/essd-12-2959-2020)
        and extra data from pilot models of MRCC5 and ClimEx.
@@ -847,14 +871,15 @@
     Returns
     -------
     xr.Dataset
         Warming level dataset.
     """
     if tas_baseline_period is None:
         tas_baseline_period = ["1850", "1900"]
+    tas_baseline_period = standardize_periods(tas_baseline_period, multiple=False)
 
     if tas_csv is None:
         tas_csv = Path(__file__).parent / "data/IPCC_annual_global_tas.csv"
 
     # get info on ds
     id_ds = ds.attrs["cat:id"]
     source_ds = (
@@ -951,15 +976,17 @@
         )
         ds_wl.warminglevel.attrs[
             "baseline"
         ] = f"{tas_baseline_period[0]}-{tas_baseline_period[1]}"
 
     if to_level is not None:
         ds_wl.attrs["cat:processing_level"] = to_level.format(
-            wl=wl, period0=tas_baseline_period[0], period1=tas_baseline_period[1]
+            wl=wl,
+            period0=tas_baseline_period[0],
+            period1=tas_baseline_period[1],
         )
 
     return ds_wl
 
 
 def _dispatch_historical_to_future(catalog: DataCatalog, id_columns: list):
     """Update a DataCatalog by recopying each "historical" entry to its corresponding future experiments.
@@ -1248,105 +1275,7 @@
     logger.info(
         f"Removing the following datasets because of the restriction for warming levels: {list(removed)}"
     )
 
     df = df.drop(columns=["csv_name"])
 
     return df
-
-
-def _subset_file_coverage(
-    df: pd.DataFrame, periods: list, *, coverage: float = 0.99
-) -> pd.DataFrame:
-    """Return a subset of files that overlap with the target period(s).
-
-    The minimum resolution for periods is 1 hour.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-      List of files to be evaluated, with at least a date_start and date_end column,
-      which are expected to be `pd.Period` objects with `freq='H'`.
-    periods : list
-      [start, end] of the period to be evaluated (or a list of lists)
-    coverage : float
-      Percentage of hours that need to be covered in a given period for the dataset to be valid
-
-    Returns
-    -------
-    pd.DataFrame
-      Subset of files that overlap the targetted period(s)
-    """
-    if not isinstance(periods[0], list):
-        periods = [periods]
-
-    # Create an Interval for each file
-    file_intervals = df.apply(
-        lambda r: pd.Interval(
-            left=r["date_start"].ordinal, right=r["date_end"].ordinal, closed="both"
-        ),
-        axis=1,
-    )
-
-    # Check for duplicated Intervals
-    if any(file_intervals.duplicated()):
-        logging.warning(
-            f"{df['id'].iloc[0] + ': ' if 'id' in df.columns else ''}Time periods are overlapping."
-        )
-        return pd.DataFrame(columns=df.columns)
-
-    # Create an array of True/False
-    files_to_keep = np.zeros(len(file_intervals), dtype=bool)
-    for period in periods:
-        period_interval = pd.Interval(
-            left=date_parser(str(period[0]), freq="H").ordinal,
-            right=date_parser(str(period[1]), end_of_period=True, freq="H").ordinal,
-            closed="both",
-        )
-        files_in_range = file_intervals.apply(lambda r: period_interval.overlaps(r))
-
-        # Very rough guess of the coverage relative to the requested period,
-        # without having to open the files or checking day-by-day
-        # This is only checking that you have the first and last time point, not that you have everything in between.
-
-        guessed_nb_hrs = np.min(
-            [
-                df[files_in_range]["date_end"].max(),
-                date_parser(str(period[1]), end_of_period=True, freq="H"),
-            ]
-        ) - np.max(
-            [
-                df[files_in_range]["date_start"].min(),
-                date_parser(str(period[0]), freq="H"),
-            ]
-        )
-
-        period_nb_hrs = date_parser(
-            str(period[1]), end_of_period=True, freq="H"
-        ) - date_parser(str(period[0]), freq="H")
-
-        # This checks the sum of hours in all selected files
-        if len(df[files_in_range]) != 0:
-            guessed_nb_hrs_sum = (
-                df[files_in_range]["date_end"] - df[files_in_range]["date_start"]
-            ).sum()
-        # if no files are selected and guessed_nb_hrs_sum=0, the division breaks the code.
-        # The warming will be called anyway even without this test.
-        else:
-            guessed_nb_hrs_sum = period_nb_hrs
-
-        if (
-            guessed_nb_hrs / period_nb_hrs < coverage
-            or len(df[files_in_range]) == 0
-            or guessed_nb_hrs_sum.nanos / period_nb_hrs.nanos < coverage
-        ):
-            logging.warning(
-                f"{df['id'].iloc[0] + ': ' if 'id' in df.columns else ''}Insufficient coverage."
-                f"% covered, min to max : {guessed_nb_hrs / period_nb_hrs:.1%}, "
-                f"% covered, sum of hours : {guessed_nb_hrs_sum.nanos / period_nb_hrs.nanos:.1%}, "
-                f"number of files in range : {len(df[files_in_range])}."
-            )
-            return pd.DataFrame(columns=df.columns)
-
-        files_to_keep = files_to_keep | files_in_range
-
-    return df[files_to_keep]
```

### Comparing `xscen-0.5.0/xscen/indicators.py` & `xscen-0.6.0/xscen/indicators.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import xclim as xc
 from intake_esm import DerivedVariableRegistry
 from xclim.core.indicator import Indicator
 from yaml import safe_load
 
 from xscen.config import parse_config
 
-from .utils import CV
+from .utils import CV, standardize_periods
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = ["compute_indicators", "load_xclim_module"]
 
 
@@ -78,15 +78,15 @@
         Dataset to use for the indicators.
     indicators : Union[str, PosixPath, Sequence[Indicator], Sequence[Tuple[str, Indicator]]]
         Path to a YAML file that instructs on how to calculate missing variables.
         Can also be only the "stem", if translations and custom indices are implemented.
         Can be the indicator module directly, or a sequence of indicators or a sequence of
         tuples (indicator name, indicator) as returned by `iter_indicators()`.
     periods : list
-        list of [start, end] of continuous periods over which to compute the indicators. This is needed when the time axis of ds contains some jumps in time.
+        Either [start, end] or list of [start, end] of continuous periods over which to compute the indicators. This is needed when the time axis of ds contains some jumps in time.
         If None, the dataset will be considered continuous.
     to_level : str, optional
         The processing level to assign to the output.
         If None, the processing level of the inputs is preserved.
 
     Returns
     -------
@@ -107,47 +107,77 @@
     try:
         N = len(indicators)
     except TypeError:
         N = None
     else:
         logger.info(f"Computing {N} indicators.")
 
+    def _infer_freq_from_meta(ind):
+        return (
+            ind.injected_parameters["freq"]
+            if "freq" in ind.injected_parameters
+            else ind.parameters["freq"]["default"]
+            if "freq" in ind.parameters
+            else ind.src_freq
+        )
+
+    periods = standardize_periods(periods)
+
     out_dict = dict()
     for i, ind in enumerate(indicators, 1):
         if isinstance(ind, tuple):
             iden, ind = ind
         else:
             iden = ind.identifier
         logger.info(f"{i} - Computing {iden}.")
 
         if periods is None:
             # Make the call to xclim
             out = ind(ds=ds)
 
             # Infer the indicator's frequency
-            freq = xr.infer_freq(out.time) if "time" in out.dims else "fx"
+            if "time" in out.dims:
+                if len(out.time) < 3:
+                    freq = _infer_freq_from_meta(ind)
+                else:
+                    freq = xr.infer_freq(out.time)
+            else:
+                freq = "fx"
 
         else:
             # Multiple time periods to concatenate
             concats = []
             for period in periods:
                 # Make the call to xclim
-                ds_subset = ds.sel(time=slice(str(period[0]), str(period[1])))
+                ds_subset = ds.sel(time=slice(period[0], period[1]))
                 tmp = ind(ds=ds_subset)
 
                 # Infer the indicator's frequency
-                freq = xr.infer_freq(tmp.time) if "time" in tmp.dims else "fx"
+                if "time" in tmp.dims:
+                    if len(tmp.time) < 3:
+                        freq = _infer_freq_from_meta(ind)
+                    else:
+                        freq = xr.infer_freq(tmp.time)
+                else:
+                    freq = "fx"
 
                 # In order to concatenate time periods, the indicator still needs a time dimension
                 if freq == "fx":
                     tmp = tmp.assign_coords({"time": ds_subset.time[0]})
 
                 concats.extend(tmp)
             out = xr.concat(concats, dim="time")
 
+        # Make sure that attributes have been kept for the dimensions and coordinates. Fixes a bug in xarray.
+        for c in set(list(out.coords) + list(out.dims)).intersection(
+            set(list(ds.coords) + list(ds.dims))
+        ):
+            if (out[c].attrs != ds[c].attrs) and (out[c].sizes == ds[c].sizes):
+                out[c].attrs = ds[c].attrs
+
         if "time" in out.dims:
             # cut the time axis to be within the same years as the input
             # for QS-DEC, xclim starts on DJF with time previous_year-12-01 with a nan as values. We want to cut this.
             # this should have no effect on YS and MS indicators
             out = out.sel(
                 time=slice(
                     str(ds.time[0].dt.year.values), str(ds.time[-1].dt.year.values)
```

### Comparing `xscen-0.5.0/xscen/io.py` & `xscen-0.6.0/xscen/io.py`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/xscen/reduce.py` & `xscen-0.6.0/xscen/reduce.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
     # Attributes
     criteria.attrs = {"long_name": "criteria for ensemble selection"}
 
     return criteria
 
 
+@parse_config
 def reduce_ensemble(data: xr.DataArray, method: str, kwargs: dict):  # noqa: D401
     """Wrapper for the ensemble reduction methods in xclim.ensembles.
 
     Parameters
     ----------
     data : xr.DataArray
         Selection criteria data : 2-D xr.DataArray with dimensions 'realization' and 'criteria'.
```

### Comparing `xscen-0.5.0/xscen/regrid.py` & `xscen-0.6.0/xscen/regrid.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import operator
 import os
 import warnings
 from copy import deepcopy
 from pathlib import PosixPath
 from typing import Optional, Union
 
+import cartopy.crs as ccrs
+import cf_xarray as cfxr
 import numpy as np
 import xarray as xr
 import xesmf as xe
 
 from .config import parse_config
 
 # TODO: Implement logging, warnings, etc.
@@ -306,18 +308,78 @@
         Arguments to send xe.Regridder().
 
     Returns
     -------
     xe.frontend.Regridder
         Regridder object
     """
+    if method.startswith("conservative"):
+        if (
+            ds_in.cf["longitude"].ndim == 2
+            and "longitude" not in ds_in.cf.bounds
+            and "rotated_pole" in ds_in
+        ):
+            ds_in = ds_in.update(create_bounds_rotated_pole(ds_in))
+        if (
+            ds_grid.cf["longitude"].ndim == 2
+            and "longitude" not in ds_grid.cf.bounds
+            and "rotated_pole" in ds_grid
+        ):
+            ds_grid = ds_grid.update(create_bounds_rotated_pole(ds_grid))
+
     regridder = xe.Regridder(
         ds_in=ds_in,
         ds_out=ds_grid,
         method=method,
         unmapped_to_nan=unmapped_to_nan,
         **kwargs,
     )
     if ~os.path.isfile(filename):
         regridder.to_netcdf(filename)
 
     return regridder
+
+
+def create_bounds_rotated_pole(ds):
+    """Create bounds for rotated pole datasets."""
+    ds = ds.cf.add_bounds(["rlat", "rlon"])
+
+    # In "vertices" format then expand to 2D. From (N, 2) to (N+1,) to (N+1, M+1)
+    rlatv1D = cfxr.bounds_to_vertices(ds.rlat_bounds, "bounds")
+    rlonv1D = cfxr.bounds_to_vertices(ds.rlon_bounds, "bounds")
+    rlatv = rlatv1D.expand_dims(rlon_vertices=rlonv1D).transpose(
+        "rlon_vertices", "rlat_vertices"
+    )
+    rlonv = rlonv1D.expand_dims(rlat_vertices=rlatv1D).transpose(
+        "rlon_vertices", "rlat_vertices"
+    )
+
+    # Get cartopy's crs for the projection
+    RP = ccrs.RotatedPole(
+        pole_longitude=ds.rotated_pole.grid_north_pole_longitude,
+        pole_latitude=ds.rotated_pole.grid_north_pole_latitude,
+        central_rotated_longitude=ds.rotated_pole.north_pole_grid_longitude,
+    )
+    PC = ccrs.PlateCarree()
+
+    # Project points
+    pts = PC.transform_points(RP, rlonv.values, rlatv.values)
+    lonv = rlonv.copy(data=pts[..., 0]).rename("lon_vertices")
+    latv = rlatv.copy(data=pts[..., 1]).rename("lat_vertices")
+
+    # Back to CF bounds format. From (N+1, M+1) to (4, N, M)
+    lonb = cfxr.vertices_to_bounds(lonv, ("bounds", "rlon", "rlat")).rename(
+        "lon_bounds"
+    )
+    latb = cfxr.vertices_to_bounds(latv, ("bounds", "rlon", "rlat")).rename(
+        "lat_bounds"
+    )
+
+    # Create dataset, set coords and attrs
+    ds_bnds = xr.merge([lonb, latb]).assign(
+        lon=ds.lon, lat=ds.lat, rotated_pole=ds.rotated_pole
+    )
+    ds_bnds["rlat"] = ds.rlat
+    ds_bnds["rlon"] = ds.rlon
+    ds_bnds.lat.attrs["bounds"] = "lat_bounds"
+    ds_bnds.lon.attrs["bounds"] = "lon_bounds"
+    return ds_bnds.transpose(*ds.lon.dims, "bounds")
```

### Comparing `xscen-0.5.0/xscen/scripting.py` & `xscen-0.6.0/xscen/scripting.py`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/xscen/utils.py` & `xscen-0.6.0/xscen/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "clean_up",
     "get_cat_attrs",
     "maybe_unstack",
     "minimum_calendar",
     "natural_sort",
     "publish_release_notes",
     "stack_drop_nans",
+    "standardize_periods",
     "translate_time_chunk",
     "unstack_fill_nan",
     "unstack_dates",
 ]
 
 
 def minimum_calendar(*calendars) -> str:
@@ -188,43 +189,70 @@
     xr.Dataset
       Same as `ds`, but `dim` has been unstacked to coordinates in `coords`.
       Missing elements are filled according to the defaults of `fill_value` of :py:meth:`xarray.Dataset.unstack`.
     """
     if coords is None:
         logger.info("Dataset unstacked using no coords argument.")
 
-    if isinstance(coords, (list, tuple)):
-        dims, crds = zip(*[(name, ds[name].load().values) for name in coords])
-    else:
+    if isinstance(coords, (str, os.PathLike)):
+        # find original shape in the attrs of one of the dimension
+        original_shape = "unknown"
+        for c in ds.coords:
+            if "original_shape" in ds[c].attrs:
+                original_shape = ds[c].attrs["original_shape"]
+        domain = ds.attrs.get("cat:domain", "unknown")
+        coords = coords.format(domain=domain, shape=original_shape)
+        logger.info(f"Dataset unstacked using {coords}.")
+        coords = xr.open_dataset(coords)
+        # separate coords that are dims or not
+        coords_and_dims = {
+            name: x for name, x in coords.coords.items() if name in coords.dims
+        }
+        coords_not_dims = {
+            name: x for name, x in coords.coords.items() if name not in coords.dims
+        }
+
         dims, crds = zip(
             *[
                 (name, crd.load().values)
                 for name, crd in ds.coords.items()
-                if crd.dims == (dim,)
+                if crd.dims == (dim,) and name in coords_and_dims
             ]
         )
+        out = (
+            ds.drop_vars(dims)
+            .assign_coords({dim: pd.MultiIndex.from_arrays(crds, names=dims)})
+            .unstack(dim)
+        )
 
-    out = (
-        ds.drop_vars(dims)
-        .assign_coords({dim: pd.MultiIndex.from_arrays(crds, names=dims)})
-        .unstack(dim)
-    )
+        # only reindex with the dims
+        out = out.reindex(**coords_and_dims)
+        # add back the coords that arent dims
+        for c in coords_not_dims:
+            out[c] = coords[c]
+    else:
+        if isinstance(coords, (list, tuple)):
+            dims, crds = zip(*[(name, ds[name].load().values) for name in coords])
+        else:
+            dims, crds = zip(
+                *[
+                    (name, crd.load().values)
+                    for name, crd in ds.coords.items()
+                    if crd.dims == (dim,)
+                ]
+            )
+
+        out = (
+            ds.drop_vars(dims)
+            .assign_coords({dim: pd.MultiIndex.from_arrays(crds, names=dims)})
+            .unstack(dim)
+        )
 
-    if not isinstance(coords, (list, tuple)) and coords is not None:
-        if isinstance(coords, (str, os.PathLike)):
-            # find original shape in the attrs of one of the dimension
-            original_shape = "unknown"
-            for c in ds.coords:
-                if "original_shape" in ds[c].attrs:
-                    original_shape = ds[c].attrs["original_shape"]
-            domain = ds.attrs.get("cat:domain", "unknown")
-            coords = coords.format(domain=domain, shape=original_shape)
-            logger.info(f"Dataset unstacked using {coords}.")
-            coords = xr.open_dataset(coords)
-        out = out.reindex(**coords.coords)
+        if not isinstance(coords, (list, tuple)) and coords is not None:
+            out = out.reindex(**coords.coords)
 
     for dim in dims:
         out[dim].attrs.update(ds[dim].attrs)
 
     return out
 
 
@@ -941,7 +969,36 @@
             )
         if (counts.isnull()).any().item():
             raise ValueError(
                 "The resampling count contains nans. There might be some missing data."
             )
         ds["time"] = counts.time
     return ds
+
+
+def standardize_periods(periods, multiple=True):
+    """Reformats 'periods' to a list of strings [['start', 'end'], ['start', 'end']]."""
+    if periods is None:
+        return periods
+
+    if not isinstance(periods[0], list):
+        periods = [periods]
+
+    for i in range(len(periods)):
+        if len(periods[i]) != 2:
+            raise ValueError(
+                "Each instance of 'periods' should be comprised of two elements: [start, end]."
+            )
+        if int(periods[i][0]) > int(periods[i][1]):
+            raise ValueError(
+                f"'periods' should be in chronological order, received {periods[i]}."
+            )
+        periods[i] = [str(p) for p in periods[i]]
+
+    if multiple:
+        return periods
+    else:
+        if len(periods) > 1:
+            raise ValueError(
+                f"'period' should be a single instance of [start, end], received {len(periods)}."
+            )
+        return periods[0]
```

### Comparing `xscen-0.5.0/xscen/xclim_modules/conversions.py` & `xscen-0.6.0/xscen/xclim_modules/conversions.py`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/xscen/xclim_modules/conversions.yml` & `xscen-0.6.0/xscen/xclim_modules/conversions.yml`

 * *Files identical despite different names*

### Comparing `xscen-0.5.0/xscen.egg-info/PKG-INFO` & `xscen-0.6.0/xscen.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: xscen
-Version: 0.5.0
+Version: 0.6.0
 Summary: A climate change scenario-building analysis framework, built with xclim/xarray.
 Home-page: https://github.com/Ouranosinc/xscen
 Author: Gabriel Rondeau-Genesse
 Author-email: rondeau-genesse.gabriel@ouranos.ca
-License: UNKNOWN
 Project-URL: About Ouranos, https://www.ouranos.ca/en/
 Project-URL: Changelog, https://xscen.readthedocs.io/en/stable/history.html
 Project-URL: Issue tracker, https://github.com/Ouranosinc/xscen/issues
 Keywords: xscen
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -26,60 +24,139 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ============
 xscen |logo|
 ============
 
-|build| |docs| |black| |pre-commit|
+|pypi| |status| |build| |docs| |black| |pre-commit| |versions|
 
 A climate change scenario-building analysis framework, built with Intake-esm catalogs and xarray-based packages such as xclim and xESMF.
 
 For documentation concerning `xscen`, see: https://xscen.readthedocs.io/en/latest/
 
 Features
 --------
 * Supports workflows with YAML configuration files for better transparency, reproducibility, and long-term backups.
 * Intake_esm-based catalog to find and manage climate data.
 * Climate dataset extraction, subsetting, and temporal aggregation.
 * Calculate missing variables through Intake-esm's DerivedVariableRegistry.
 * Regridding with xESMF.
 * Bias adjustment with xclim.
 
+Installation
+------------
+
+Please refer to the `installation docs`_.
+
 Acknowledgments
 ---------------
 This package was created with Cookiecutter_ and the `Ouranosinc/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyfeldroy/cookiecutter-pypackage
 .. _`Ouranosinc/cookiecutter-pypackage`: https://github.com/Ouranosinc/cookiecutter-pypackage
+.. _installation docs: https://xscen.readthedocs.io/en/latest/installation.html
 
 .. |logo| image:: https://raw.githubusercontent.com/Ouranosinc/xscen/main/docs/_static/_images/xscen-logo-small.png
         :target: https://github.com/Ouranosinc/xscen
 
 .. |build| image:: https://github.com/Ouranosinc/xscen/actions/workflows/main.yml/badge.svg
         :target: https://github.com/Ouranosinc/xscen/actions/workflows/main.yml
         :alt: Build Status
 
+.. |pypi| image:: https://img.shields.io/pypi/v/xscen.svg
+        :target: https://pypi.python.org/pypi/xscen
+        :alt: Python Package Index Build
+
 .. |docs| image:: https://readthedocs.org/projects/xscen/badge/?version=latest
         :target: https://xscen.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/psf/black
         :alt: Python Black
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/Ouranosinc/xscen/main.svg
         :target: https://results.pre-commit.ci/latest/github/Ouranosinc/xscen/main
         :alt: pre-commit.ci status
 
+.. |versions| image:: https://img.shields.io/pypi/pyversions/xscen.svg
+        :target: https://pypi.python.org/pypi/xscen
+        :alt: Supported Python Versions
+
+.. |status| image:: https://www.repostatus.org/badges/latest/wip.svg
+        :target: https://www.repostatus.org/#wip
+        :alt: Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.
+
 
 =======
 History
 =======
 
+v0.6.0 (2023-05-04)
+-------------------
+Contributors to this version: Trevor James Smith (`@Zeitsperre <https://github.com/Zeitsperre>`_), Juliette Lavoie (`@juliettelavoie <https://github.com/juliettelavoie>`_), Pascal Bourgault (`@aulemahal <https://github.com/aulemahal>`_), Gabriel Rondeau-Genesse (`@RondeauG <https://github.com/RondeauG>`_).
+
+Announcements
+^^^^^^^^^^^^^
+* `xscen` is now offered as a conda package available through Anaconda.org. Refer to the installation documentation for more information. (`GH/149 <https://github.com/Ouranosinc/xscen/issues/149>`_, `PR/171 <https://github.com/Ouranosinc/xscen/pull/171>`_).
+* Deprecation: Release 0.6.0 of `xscen` will be the last version to support ``xscen.extract.clisops_subset``. Use ``xscen.spatial.subset`` instead. (`PR/182 <https://github.com/Ouranosinc/xscen/pull/182>`_, `PR/184 <https://github.com/Ouranosinc/xscen/pull/184>`_).
+* Deprecation: The argument `region`, used in multiple functions, has been slightly reformatted. Release 0.6.0 of `xscen` will be the last version to support the old format. (`GH/99 <https://github.com/Ouranosinc/xscen/issues/99>`_, `GH/101 <https://github.com/Ouranosinc/xscen/issues/101>`_, `PR/184 <https://github.com/Ouranosinc/xscen/pull/184>`_).
+
+New features and enhancements
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+* New 'cos-lat' averaging in `spatial_mean`. (`GH/94 <https://github.com/Ouranosinc/xscen/issues/94>`_, `PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* Support for computing anomalies in `compute_deltas`.  (`PR/165 <https://github.com/Ouranosinc/xscen/pull/165>`_).
+* Add function `diagnostics.measures_improvement_2d`. (`PR/167 <https://github.com/Ouranosinc/xscen/pull/167>`_).
+* Add function ``regrid.create_bounds_rotated_pole`` and automatic use in ``regrid_dataset`` and ``spatial_mean``. This is temporary, while we wait for a functionning method in ``cf_xarray``. (`PR/174 <https://github.com/Ouranosinc/xscen/pull/174>`_, `GH/96 <https://github.com/Ouranosinc/xscen/issues/96>`_).
+* Add ``spatial`` submodule with functions ``creep_weights`` and ``creep_fill`` for filling NaNs using neighbours. (`PR/174 <https://github.com/Ouranosinc/xscen/pull/174>`_).
+* Allow passing ``GeoDataFrame`` instances in ``spatial_mean``'s ``region`` argument, not only geospatial file paths. (`PR/174 <https://github.com/Ouranosinc/xscen/pull/174>`_).
+* Allow searching for periods in `catalog.search`. (`GH/123 <https://github.com/Ouranosinc/xscen/issues/123>`_, `PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* Allow searching and extracting multiple frequencies for a given variable. (`GH/168 <https://github.com/Ouranosinc/xscen/issues/168>`_, `PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* New masking feature in ``extract_dataset``. (`GH/180 <https://github.com/Ouranosinc/xscen/issues/180>`_, `PR/182 <https://github.com/Ouranosinc/xscen/pull/182>`_).
+* New function ``xs.spatial.subset`` to replace ``xs.extract.clisops_subset`` and add method "sel". (`GH/180 <https://github.com/Ouranosinc/xscen/issues/180>`_, `PR/182 <https://github.com/Ouranosinc/xscen/pull/182>`_).
+* Add long_name attribute to diagnostics. ( `PR/189 <https://github.com/Ouranosinc/xscen/pull/189>`_).
+* Added a new YAML-centric notebook (`GH/8 <https://github.com/Ouranosinc/xscen/issues/8>`_, `PR/191 <https://github.com/Ouranosinc/xscen/pull/191>`_).
+* New ``utils.standardize_periods`` to standardize that argument across multiple functions. (`GH/87 <https://github.com/Ouranosinc/xscen/issues/87>`_, `PR/192 <https://github.com/Ouranosinc/xscen/pull/192>`_).
+* New `coverage_kwargs` argument added to ``search_data_catalogs`` to allow modifying the default values of ``subset_file_coverage``. (`GH/87 <https://github.com/Ouranosinc/xscen/issues/87>`_, `PR/192 <https://github.com/Ouranosinc/xscen/pull/192>`_).
+
+Breaking changes
+^^^^^^^^^^^^^^^^
+* 'mean' averaging has been deprecated in `spatial_mean`. (`PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* 'interp_coord' has been renamed to 'interp_centroid' in `spatial_mean`. (`PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* The 'datasets' dimension of the output of ``diagnostics.measures_heatmap`` is renamed 'realization'. (`PR/167 <https://github.com/Ouranosinc/xscen/pull/167>`_).
+* `_subset_file_coverage` was renamed `subset_file_coverage` and moved to ``catalog.py`` to prevent circular imports. (`PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* `extract_dataset` doesn't fail when a variable is in the dataset, but not `variables_and_freqs`. (`PR/185 <https://github.com/Ouranosinc/xscen/pull/185>`_).
+* The argument `period`, used in multiple function, is now always a single list, while `periods` is more flexible. (`GH/87 <https://github.com/Ouranosinc/xscen/issues/87>`_, `PR/192 <https://github.com/Ouranosinc/xscen/pull/192>`_).
+* The parameters `reference_period` and `simulation_period` of ``xscen.train`` and ``xscen.adjust`` were renamed `period/periods` to respect the point above. (`GH/87 <https://github.com/Ouranosinc/xscen/issues/87>`_, `PR/192 <https://github.com/Ouranosinc/xscen/pull/192>`_).
+
+Bug fixes
+^^^^^^^^^
+* Forbid pandas v1.5.3 in the environment files, as the linux conda build breaks the data catalog parser. (`GH/161 <https://github.com/Ouranosinc/xscen/issues/161>`_, `PR/162 <https://github.com/Ouranosinc/xscen/pull/162>`_).
+* Only return requested variables when using ``DataCatalog.to_dataset``. (`PR/163 <https://github.com/Ouranosinc/xscen/pull/163>`_).
+* ``compute_indicators`` no longer crashes if less than 3 timesteps are produced. (`PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* `xarray` is temporarily pinned below v2023.3.0 due to an API-breaking change. (`GH/175 <https://github.com/Ouranosinc/xscen/issues/175>`_, `PR/173 <https://github.com/Ouranosinc/xscen/pull/173>`_).
+* `xscen.utils.unstack_fill_nan`` can now handle datasets that have non dimension coordinates. (`GH/156 <https://github.com/Ouranosinc/xscen/issues/156>`_, `PR/175 <https://github.com/Ouranosinc/xscen/pull/175>`_).
+* `extract_dataset` now skips a simulation way earlier if the frequency doesn't match. (`PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* `extract_dataset` now correctly tries to extract in reverse timedelta order. (`PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* `compute_deltas` no longer creates all NaN values if the input dataset is in a non-standard calendar. (`PR/188 <https://github.com/Ouranosinc/xscen/pull/188>`_).
+
+Internal changes
+^^^^^^^^^^^^^^^^
+* `xscen` now manages packaging for PyPi and TestPyPI via GitHub workflows. (`PR/159 <https://github.com/Ouranosinc/xscen/pull/159>`_).
+* Pre-load coordinates in ``extract.clisops_subset`` (`PR/163 <https://github.com/Ouranosinc/xscen/pull/163>`_).
+* Minimal documentation for templates. (`PR/163 <https://github.com/Ouranosinc/xscen/pull/163>`_).
+* `xscen` is now indexed in `Zenodo <https://zenodo.org/>`_, under the `ouranos` community of projects. (`PR/164 <https://github.com/Ouranosinc/xscen/pull/164>`_).
+* Added a few relevant `Shields <https://shields.io/>`_ to the README.rst. (`PR/164 <https://github.com/Ouranosinc/xscen/pull/164>`_).
+* Better warning messages in ``_subset_file_coverage`` when coverage is insufficient. (`PR/125 <https://github.com/Ouranosinc/xscen/pull/125>`_).
+* The top-level Makefile now includes a `linkcheck` recipe, and the ReadTheDocs configuration no longer reinstalls the `llvmlite` compiler library. (`PR/173 <https://github.com/Ouranosinc/xscen/pull/173>`_).
+* The checkups on coverage and duplicates can now be skipped in `subset_file_coverage`. (`PR/170 <https://github.com/Ouranosinc/xscen/pull/170>`_).
+* Changed the `ProjectCatalog` docstrings to make it more obvious that it needs to be created empty. (`GH/99 <https://github.com/Ouranosinc/xscen/issues/99>`_, `PR/184 <https://github.com/Ouranosinc/xscen/pull/184>`_).
+* Added parse_config to `creep_fill`, `creep_weights`, and `reduce_ensemble` (`PR/191 <https://github.com/Ouranosinc/xscen/pull/191>`_).
+
 v0.5.0 (2023-02-28)
 -------------------
 Contributors to this version: Gabriel Rondeau-Genesse (`@RondeauG <https://github.com/RondeauG>`_), Juliette Lavoie (`@juliettelavoie <https://github.com/juliettelavoie>`_), Trevor James Smith (`@Zeitsperre <https://github.com/Zeitsperre>`_), Sarah Gammon (`@sg2475962 <https://github.com/sg2475962>`_) and Pascal Bourgault (`@aulemahal <https://github.com/aulemahal>`_).
 
 New features and enhancements
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 * Possibility of excluding variables read from file from the catalog produced by ``parse_directory``. (`PR/107 <https://github.com/Ouranosinc/xscen/pull/107>`_).
@@ -119,15 +196,15 @@
 * ``compute_deltas`` skips the unstacking step if there is no time dimension and cast object dimensions to string. (`PR/9 <https://github.com/Ouranosinc/xscen/pull/9>`_)
 * Added the "2sem" frequency to the translations CVs. (`PR/111 <https://github.com/Ouranosinc/xscen/pull/111>`_).
 * Skip files we can't read in ``parse_directory``. (`PR/111 <https://github.com/Ouranosinc/xscen/pull/111>`_).
 * Fixed non-numpy-standard Docstrings. (`PR/108 <https://github.com/Ouranosinc/xscen/pull/108>`_).
 * Added more metadata to package description on PyPI. (`PR/108 <https://github.com/Ouranosinc/xscen/pull/108>`_).
 * Faster ``search_data_catalogs`` and ``extract_dataset`` through a faster ``DataCatalog.unique``, date parsing and a rewrite of the ``ensure_correct_time`` logic. (`PR/127 <https://github.com/Ouranosinc/xscen/pull/127>`_).
 * The ``search_data_catalogs`` function now accepts `str` or `pathlib.Path` variables (in addition to lists of either data type) for performing catalog lookups. (`PR/121 <https://github.com/Ouranosinc/xscen/pull/121>`_).
-* `produce_horizons` now supports fixed fields (pull:`139`).
+* `produce_horizons` now supports fixed fields (`PR/139 <https://github.com/Ouranosinc/xscen/pull/139>`_).
 * Rewrite of ``unstack_dates`` for better performance with dask arrays. (`PR/144 <https://github.com/Ouranosinc/xscen/pull/144>`_).
 
 v0.4.0 (2022-09-28)
 -------------------
 Contributors to this version: Gabriel Rondeau-Genesse (`@RondeauG <https://github.com/RondeauG>`_), Juliette Lavoie (`@juliettelavoie <https://github.com/juliettelavoie>`_), Trevor James Smith (`@Zeitsperre <https://github.com/Zeitsperre>`_) and Pascal Bourgault (`@aulemahal <https://github.com/aulemahal>`_).
 
 New features and enhancements
@@ -238,9 +315,7 @@
 Breaking changes
 ^^^^^^^^^^^^^^^^
 * N/A
 
 Internal changes
 ^^^^^^^^^^^^^^^^
 * N/A
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xscen-0.5.0/xscen.egg-info/SOURCES.txt` & `xscen-0.6.0/xscen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 xscen/ensembles.py
 xscen/extract.py
 xscen/indicators.py
 xscen/io.py
 xscen/reduce.py
 xscen/regrid.py
 xscen/scripting.py
+xscen/spatial.py
 xscen/utils.py
 xscen.egg-info/PKG-INFO
 xscen.egg-info/SOURCES.txt
 xscen.egg-info/dependency_links.txt
 xscen.egg-info/not-zip-safe
 xscen.egg-info/requires.txt
 xscen.egg-info/top_level.txt
```

