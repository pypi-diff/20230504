# Comparing `tmp/pz-rail-gpz-v1-0.1.0.tar.gz` & `tmp/pz-rail-gpz-v1-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-gpz-v1-0.1.0.tar", last modified: Thu Sep 22 23:05:32 2022, max compression
+gzip compressed data, was "pz-rail-gpz-v1-0.1.1.tar", last modified: Thu May  4 05:22:17 2023, max compression
```

## Comparing `pz-rail-gpz-v1-0.1.0.tar` & `pz-rail-gpz-v1-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.908194 pz-rail-gpz-v1-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.904194 pz-rail-gpz-v1-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.904194 pz-rail-gpz-v1-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-09-22 23:05:32.908194 pz-rail-gpz-v1-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.904194 pz-rail-gpz-v1-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     8787 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/examples/GPz_estimation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 23:05:32.908194 pz-rail-gpz-v1-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.904194 pz-rail-gpz-v1-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.904194 pz-rail-gpz-v1-0.1.0/src/pz_rail_gpz_v1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-09-22 23:05:32.000000 pz-rail-gpz-v1-0.1.0/src/pz_rail_gpz_v1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-09-22 23:05:32.000000 pz-rail-gpz-v1-0.1.0/src/pz_rail_gpz_v1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 23:05:32.000000 pz-rail-gpz-v1-0.1.0/src/pz_rail_gpz_v1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-22 23:05:32.000000 pz-rail-gpz-v1-0.1.0/src/pz_rail_gpz_v1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-22 23:05:32.000000 pz-rail-gpz-v1-0.1.0/src/pz_rail_gpz_v1.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.904194 pz-rail-gpz-v1-0.1.0/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.904194 pz-rail-gpz-v1-0.1.0/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.908194 pz-rail-gpz-v1-0.1.0/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (121)    21483 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/src/rail/estimation/algos/GPz.py
--rw-r--r--   0 runner    (1001) docker     (121)     7677 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/src/rail/estimation/algos/gpz_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.908194 pz-rail-gpz-v1-0.1.0/src/rail/estimation/algos/gpz_version/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/src/rail/estimation/algos/gpz_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-22 23:05:32.000000 pz-rail-gpz-v1-0.1.0/src/rail/estimation/algos/gpz_version/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 23:05:32.908194 pz-rail-gpz-v1-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-09-22 23:05:22.000000 pz-rail-gpz-v1-0.1.0/tests/test_gpz.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3314 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     8787 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/examples/GPz_estimation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (122)    21483 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/GPz.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/gpz_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/src/rail/gpz/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/src/rail/gpz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 05:22:16.000000 pz-rail-gpz-v1-0.1.1/src/rail/gpz/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/tests/test_gpz.py
```

### Comparing `pz-rail-gpz-v1-0.1.0/.github/workflows/main.yml` & `pz-rail-gpz-v1-0.1.1/.github/workflows/main.yml`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        pip install wheel numpy # For somoclu
         pip install .
         pip install flake8 pytest pytest-cov mockmpi pytest-timeout
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Test with pytest
       run: |
         python -m pytest --cov=rail.estimation.algos.gpz_v1 --cov-report=xml
     - name: Upload coverage to Codecov
```

### Comparing `pz-rail-gpz-v1-0.1.0/.github/workflows/pypi.yaml` & `pz-rail-gpz-v1-0.1.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.0/.gitignore` & `pz-rail-gpz-v1-0.1.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+_version.py
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `pz-rail-gpz-v1-0.1.0/LICENSE` & `pz-rail-gpz-v1-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.0/PKG-INFO` & `pz-rail-gpz-v1-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-gpz-v1
-Version: 0.1.0
+Version: 0.1.1
 Summary: RAIL GPz v1 (pure python) Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-gpz-v1-0.1.0/README.md` & `pz-rail-gpz-v1-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.0/examples/GPz_estimation_example.ipynb` & `pz-rail-gpz-v1-0.1.1/examples/GPz_estimation_example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.0/pyproject.toml` & `pz-rail-gpz-v1-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ]
 
 [build-system]
 requires = ["setuptools>=61", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
-write_to = "src/rail/estimation/algos/gpz_version/_version.py"
+write_to = "src/rail/gpz/_version.py"
 
 [tool.coverage.run]
 source = ["src/rail"]
 branch = false
 
 [tool.coverage.report]
 show_missing = true
```

### Comparing `pz-rail-gpz-v1-0.1.0/src/pz_rail_gpz_v1.egg-info/PKG-INFO` & `pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-gpz-v1
-Version: 0.1.0
+Version: 0.1.1
 Summary: RAIL GPz v1 (pure python) Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-gpz-v1-0.1.0/src/rail/estimation/algos/GPz.py` & `pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/GPz.py`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.0/src/rail/estimation/algos/gpz_v1.py` & `pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/gpz_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 """
 RAIL wrapping of Peter Hatfield's version of GPz, which
 can be found at:
 https://github.com/pwhatfield/GPz_py3
 """
 import numpy as np
 from ceci.config import StageParameter as Param
+from rail.core.common_params import SHARED_PARAMS
 from rail.estimation.estimator import CatEstimator, CatInformer
 from .GPz import GP, getOmega
 import qp
 
 
-def_filt = ['u', 'g', 'r', 'i', 'z', 'y']
-def_bands = [f"mag_{band}_lsst" for band in def_filt]
-def_err_bands = [f"mag_err_{band}_lsst" for band in def_filt]
-def_maglims = dict(mag_u_lsst=27.79,
-                   mag_g_lsst=29.04,
-                   mag_r_lsst=29.06,
-                   mag_i_lsst=28.62,
-                   mag_z_lsst=27.98,
-                   mag_y_lsst=27.05)
-
 
 def _prepare_data(data_dict, bands, err_bands, nondet_val, maglims, logflag):
     """Put data in 2D np array expected by GPz.
     For some reason they like to take the log of the magnitude errors, so
     have that as a boolean option.  Also replace nondetect vals for each
     band
     """
     numbands = len(bands)
     totrows = len(data_dict[bands[0]])
     data = np.empty([totrows, 2 * numbands])
     for i, (band, eband, lim) in enumerate(zip(bands, err_bands, maglims.values())):
         data[:, i] = data_dict[band]
-        mask = np.isclose(data_dict[band], nondet_val)
+        mask = np.bitwise_or(np.isclose(data_dict[band], nondet_val), np.isnan(data_dict[band]))
         data[:, i][mask] = lim
         if logflag:
             data[:, numbands + i] = np.log(data_dict[eband])
         else:  # pragma: no cover
             data[:, numbands + i] = data_dict[eband]
         data[:, numbands + i][mask] = 1.0
     return data
@@ -51,22 +42,22 @@
     -------
     gpz_model: model
       model file containing the trained GPz model to be used in estimate
       stage
     """
     name = "Inform_GPz_v1"
     config_options = CatInformer.config_options.copy()
-    config_options.update(nondetect_val=Param(float, 99.0, msg="value to be replaced with magnitude limit for non detects"),
-                          mag_lims=Param(dict, def_maglims, msg="magnitude limits for each band"),
+    config_options.update(nondetect_val=SHARED_PARAMS,
+                          mag_limits=SHARED_PARAMS,
                           trainfrac=Param(float, 0.75,
                                           msg="fraction of training data used to make tree, rest used to set best sigma"),
-                          seed=Param(int, 0, msg="Random number seed for NN training"),
-                          bands=Param(list, def_bands, msg="bands to use in estimation"),
-                          err_bands=Param(list, def_err_bands, msg="error column names to use in estimation"),
-                          redshift_col=Param(str, "redshift", msg="name for redshift column"),
+                          seed=Param(int, 87, msg="random seed"),
+                          bands=SHARED_PARAMS,
+                          err_bands=SHARED_PARAMS,
+                          redshift_col=SHARED_PARAMS,
                           gpz_method=Param(str, "VC", msg="method to be used in GPz, options are 'GL', 'VL', 'GD', 'VD', 'GC', and 'VC'"),
                           n_basis=Param(int, 50, msg="number of basis functions used"),
                           learn_jointly=Param(bool, True, msg="if True, jointly learns prior linear mean function"),
                           hetero_noise=Param(bool, True, msg="if True, learns heteroscedastic noise process, set False for point est."),
                           csl_method=Param(str, "normal", msg="cost sensitive learning type, 'balanced', 'normalized', or 'normal'"),
                           csl_binwidth=Param(float, 0.1, msg="width of bin for 'balanced' cost sensitive learning"),
                           pca_decorrelate=Param(bool, True, msg="if True, decorrelate data using PCA as preprocessing stage"),
@@ -85,16 +76,17 @@
         """
         train the GPz model after splitting train data into train/validation
         """
         if self.config.hdf5_groupname:
             training_data = self.get_data('input')[self.config.hdf5_groupname]
         else:  # pragma: no cover
             training_data = self.get_data('input')
+
         input_array = _prepare_data(training_data, self.config.bands, self.config.err_bands,
-                                    self.config.nondetect_val, self.config.mag_lims,
+                                    self.config.nondetect_val, self.config.mag_limits,
                                     self.config.log_errors)
 
         sz = np.expand_dims(training_data[self.config.redshift_col], -1)
         # need permutation mask to define training vs validation
         ngal = input_array.shape[0]
         print(f"ngal: {ngal}")
         ntrain = int(ngal * self.config.trainfrac)
@@ -124,34 +116,34 @@
 
 
 class GPz_v1(CatEstimator):
     """GPz_v1 estimator
     """
     name = "GPz_v1"
     config_options = CatEstimator.config_options.copy()
-    config_options.update(zmin=Param(float, 0.0, msg="min z"),
-                          zmax=Param(float, 3.0, msg="max_z"),
-                          nzbins=Param(int, 301, msg="num z bins"),
-                          nondetect_val=Param(float, 99.0, msg="value to be replaced with magnitude limit for non detects"),
-                          mag_lims=Param(dict, def_maglims, msg="magnitude limits for each band"),
-                          bands=Param(list, def_bands, msg="bands to use in estimation"),
-                          err_bands=Param(list, def_err_bands, msg="error column names to use in estimation"),
-                          redshift_col=Param(str, "redshift", msg="name for redshift column"),
+    config_options.update(zmin=SHARED_PARAMS,
+                          zmax=SHARED_PARAMS,
+                          nzbins=SHARED_PARAMS,
+                          nondetect_val=SHARED_PARAMS,
+                          mag_limits=SHARED_PARAMS,
+                          bands=SHARED_PARAMS,
+                          err_bands=SHARED_PARAMS,
+                          ref_band=SHARED_PARAMS,
                           log_errors=Param(bool, True, msg="if true, take log of magnitude errors"))
 
     def __init__(self, args, comm=None):
         """ Constructor:
         Do CatEstimator specific initialization """
         CatEstimator.__init__(self, args, comm=comm)
         self.zgrid = None
 
     def _process_chunk(self, start, end, data, first):
         print(f"Process {self.rank} estimating GPz PZ PDF for rows {start:,} - {end:,}")
         test_array = _prepare_data(data, self.config.bands, self.config.err_bands,
-                                   self.config.nondetect_val, self.config.mag_lims,
+                                   self.config.nondetect_val, self.config.mag_limits,
                                    self.config.log_errors)
 
         mu, totalV, modelV, noiseV, _ = self.model.predict(test_array)
         ens = qp.Ensemble(qp.stats.norm, data=dict(loc=mu, scale=totalV))
         zgrid = np.linspace(self.config.zmin, self.config.zmax, self.config.nzbins)
         zmode = ens.mode(grid=zgrid)
         ens.set_ancil(dict(zmode=zmode))
```

### Comparing `pz-rail-gpz-v1-0.1.0/tests/test_gpz.py` & `pz-rail-gpz-v1-0.1.1/tests/test_gpz.py`

 * *Files identical despite different names*

