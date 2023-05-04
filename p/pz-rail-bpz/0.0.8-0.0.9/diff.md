# Comparing `tmp/pz-rail-bpz-0.0.8.tar.gz` & `tmp/pz-rail-bpz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-bpz-0.0.8.tar", last modified: Mon May  1 22:21:09 2023, max compression
+gzip compressed data, was "pz-rail-bpz-0.0.9.tar", last modified: Thu May  4 05:26:18 2023, max compression
```

## Comparing `pz-rail-bpz-0.0.8.tar` & `pz-rail-bpz-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 22:21:09.440036 pz-rail-bpz-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (122)    27982 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_lite.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_version/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-01 22:21:08.000000 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_version/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/examples/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/examples/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/examples/estimation/configs/
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/src/rail/examples/estimation/configs/test_bpz.columns
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/tests/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (122)    10624 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/tests/validation_10gal.pq
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/bpz/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/src/rail/bpz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/rail/bpz/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/src/rail/bpz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (122)    26631 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/src/rail/estimation/algos/bpz_lite.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/examples_data/estimation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/src/rail/examples_data/estimation_data/configs/test_bpz.columns
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6104 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/tests/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10624 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/tests/validation_10gal.pq
```

### Comparing `pz-rail-bpz-0.0.8/.github/workflows/main.yml` & `pz-rail-bpz-0.0.9/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        pip install wheel numpy
         pip install .
         pip install flake8 pytest pytest-cov mockmpi pytest-timeout
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Test with pytest
       run: |
         python -m pytest --cov=rail.estimation.algos.bpz_lite --cov-report=xml
     - name: Upload coverage to Codecov
```

### Comparing `pz-rail-bpz-0.0.8/.github/workflows/pypi.yaml` & `pz-rail-bpz-0.0.9/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.8/.gitignore` & `pz-rail-bpz-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.8/LICENSE` & `pz-rail-bpz-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.8/PKG-INFO` & `pz-rail-bpz-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.0.8
+Version: 0.0.9
 Summary: RAIL BPZ Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-bpz-0.0.8/README.md` & `pz-rail-bpz-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.8/pyproject.toml` & `pz-rail-bpz-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ]
 
 [build-system]
 requires = ["setuptools>=61", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
-write_to = "src/rail/estimation/algos/bpz_version/_version.py"
+write_to = "src/rail/bpz/_version.py"
 
 [tool.setuptools.package-data]
 "rail.examples.estimation.configs" = ["*.columns"]
 
 [tool.coverage.run]
 source = ["src/rail"]
 branch = true
```

### Comparing `pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/PKG-INFO` & `pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.0.8
+Version: 0.0.9
 Summary: RAIL BPZ Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/SOURCES.txt` & `pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 .github/workflows/main.yml
 .github/workflows/pypi.yaml
 src/pz_rail_bpz.egg-info/PKG-INFO
 src/pz_rail_bpz.egg-info/SOURCES.txt
 src/pz_rail_bpz.egg-info/dependency_links.txt
 src/pz_rail_bpz.egg-info/requires.txt
 src/pz_rail_bpz.egg-info/top_level.txt
+src/rail/bpz/__init__.py
+src/rail/bpz/_version.py
+src/rail/bpz/utils.py
 src/rail/estimation/algos/bpz_lite.py
-src/rail/estimation/algos/bpz_version/__init__.py
-src/rail/estimation/algos/bpz_version/_version.py
-src/rail/estimation/algos/bpz_version/utils.py
-src/rail/examples/estimation/configs/test_bpz.columns
+src/rail/examples_data/estimation_data/configs/test_bpz.columns
 tests/test_algos.py
 tests/validation_10gal.pq
```

### Comparing `pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_lite.py` & `pz-rail-bpz-0.0.9/src/rail/estimation/algos/bpz_lite.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,25 +26,17 @@
 import scipy.integrate
 import glob
 import qp
 import tables_io
 from ceci.config import StageParameter as Param
 from rail.estimation.estimator import CatEstimator, CatInformer
 from rail.core.utils import RAILDIR
-from rail.estimation.algos.bpz_version.utils import RAIL_BPZ_DIR
+from rail.bpz.utils import RAIL_BPZ_DIR
+from rail.core.common_params import SHARED_PARAMS
 
-def_bands = ['u', 'g', 'r', 'i', 'z', 'y']
-def_bandnames = [f"mag_{band}_lsst" for band in def_bands]
-def_errnames = [f"mag_err_{band}_lsst" for band in def_bands]
-def_maglims = dict(mag_u_lsst=27.79,
-                   mag_g_lsst=29.04,
-                   mag_r_lsst=29.06,
-                   mag_i_lsst=28.62,
-                   mag_z_lsst=27.98,
-                   mag_y_lsst=27.05)
 
 
 def nzfunc(z, z0, alpha, km, m, m0):  # pragma: no cover
     zm = z0 + (km * (m - m0))
     return np.power(z, alpha) * np.exp(-1. * np.power((z / zm), alpha))
 
 
@@ -65,45 +57,44 @@
     For p(z|T,m) we have
     P(z|T,m) = f_x*z0_x^a *exp(-(z/zm_x)^a)
     where zm_x = z0_x*(km_x-m0)
     where f_x is the type fraction from p(T|m), and we fit for values of
     z0, km, and a for each type.  These parameters are then fed to the BPZ
     prior for use in the estimation stage.
     """
-    name = 'Inform_BPZ_lite'
+    name = "Inform_BPZ_lite"
     config_options = CatInformer.config_options.copy()
-    config_options.update(zmin=Param(float, 0.0, msg="min z for grid"),
-                          zmax=Param(float, 3.0, msg="max z for grid"),
-                          nzbins=Param(int, 301, msg="# of bins in zgrid"),
-                          band_names=Param(list, def_bandnames,
-                                           msg="band names to be used, *ASSUMED TO BE IN INCREASING WL ORDER!*"),
-                          band_err_names=Param(list, def_errnames,
-                                               msg="band error column names to be used * ASSUMED TO BE IN INCREASING WL ORDER!*"),
-                          nondetect_val=Param(float, 99.0, msg="value to be replaced with magnitude limit for non detects"),
+    config_options.update(zmin=SHARED_PARAMS,
+                          zmax=SHARED_PARAMS,
+                          nzbins=SHARED_PARAMS,
+                          nondetect_val=SHARED_PARAMS,
+                          mag_limits=SHARED_PARAMS,
+                          bands=SHARED_PARAMS,
+                          err_bands=SHARED_PARAMS,
+                          ref_band=SHARED_PARAMS,
+                          redshift_col=SHARED_PARAMS,   
                           data_path=Param(str, "None",
                                           msg="data_path (str): file path to the "
                                           "SED, FILTER, and AB directories.  If left to "
                                           "default `None` it will use the install "
-                                          "directory for rail + rail/examples/estimation/data"),
-                          columns_file=Param(str, os.path.join(RAIL_BPZ_DIR, 'rail/examples/estimation/configs/test_bpz.columns'),
+                                          "directory for rail + rail/examples_data/estimation_data/data"),
+                          columns_file=Param(str, os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
                                              msg="name of the file specifying the columns"),
-                          spectra_file=Param(str, 'SED/CWWSB4.list',
+                          spectra_file=Param(str, "SED/CWWSB4.list",
                                              msg="name of the file specifying the list of SEDs to use"),
                           m0=Param(float, 20.0, msg="reference apparent mag, used in prior param"),
                           nt_array=Param(list, [1, 2, 3], msg="list of integer number of templates per 'broad type', "
                                          "must be in same order as the template set, and must sum to the same number "
                                          "as the # of templates in the spectra file"),
                           mmin=Param(float, 18.0, msg="lowest apparent mag in ref band, lower values ignored"),
                           mmax=Param(float, 29.0, msg="highest apparent mag in ref band, higher values ignored"),
                           init_kt=Param(float, 0.3, msg="initial guess for kt in training"),
                           init_zo=Param(float, 0.4, msg="initial guess for z0 in training"),
                           init_alpha=Param(float, 1.8, msg="initial guess for alpha in training"),
                           init_km=Param(float, 0.1, msg="initial guess for km in training"),
-                          prior_band=Param(str, "mag_i_lsst", msg="referene band, which column to use in training prior"),
-                          redshift_col=Param(str, "redshift", msg="name for redshift column in training data"),
                           type_file=Param(str, "", msg="name of file with the broad type fits for the training data"))
 
     def __init__(self, args, comm=None):
         """Init function, init config stuff
         """
         CatInformer.__init__(self, args, comm=comm)
         self.fo_arr = None
@@ -138,15 +129,15 @@
             kt_init = np.array([self.config.init_kt])
         else:
             fo_init = np.ones(self.ntyp - 1) / (self.ntyp)
             kt_init = np.ones(self.ntyp - 1) * self.config.init_kt
         fracparams = np.hstack([fo_init, kt_init])
         # run scipy optimize to find best params
         # note that best fit vals are stored as "x" for some reason
-        frac_results = sciop.minimize(self._frac_likelihood, fracparams, method='nelder-mead').x
+        frac_results = sciop.minimize(self._frac_likelihood, fracparams, method="nelder-mead").x
         if self.ntyp == 1:
             self.fo_arr = np.array([frac_results[0]])
             self.kt_arr = np.array([frac_results[1]])
         else:
             self.fo_arr = frac_results[:self.ntyp - 1]
             self.kt_arr = frac_results[self.ntyp - 1:]
 
@@ -175,51 +166,51 @@
         zo_arr = np.ones(self.ntyp)
         a_arr = np.ones(self.ntyp)
         km_arr = np.ones(self.ntyp)
         for i in range(self.ntyp):
             print(f"minimizing for type {i}")
             self.typmask = (self.besttypes == i)
             dndzparams = np.hstack([self.config.init_zo, self.config.init_alpha, self.config.init_km])
-            result = sciop.minimize(self._dndz_likelihood, dndzparams, method='nelder-mead').x
+            result = sciop.minimize(self._dndz_likelihood, dndzparams, method="nelder-mead").x
             zo_arr[i] = result[0]
             a_arr[i] = result[1]
             km_arr[i] = result[2]
             print(f"best fit z0, alpha, km for type {i}: {result}")
         return zo_arr, km_arr, a_arr
 
     def _get_broad_type(self, ngal):
         typefile = self.config.type_file
         if typefile == "":  # pragma: no cover
             typedata = np.zeros(ngal, dtype=int)
         else:
-            typedata = tables_io.read(typefile)['types']  # pragma: no cover
+            typedata = tables_io.read(typefile)["types"]  # pragma: no cover
         numtypes = len(list(set(typedata)))
         return numtypes, typedata
 
     def run(self):
         """compute the best fit prior parameters
         """
         self.m0 = self.config.m0
         if self.config.hdf5_groupname:
-            training_data = self.get_data('input')[self.config.hdf5_groupname]
+            training_data = self.get_data("input")[self.config.hdf5_groupname]
         else:  # pragma: no cover
-            training_data = self.get_data('input')
+            training_data = self.get_data("input")
 
-        ngal = len(training_data[self.config.prior_band])
+        ngal = len(training_data[self.config.ref_band])
 
-        if self.config.prior_band not in training_data.keys():  # pragma: no cover
-            raise KeyError(f"prior_band {self.config.prior_band} not found in input data!")
+        if self.config.ref_band not in training_data.keys():  # pragma: no cover
+            raise KeyError(f"ref_band {self.config.ref_band} not found in input data!")
         if self.config.redshift_col not in training_data.keys():  # pragma: no cover
             raise KeyError(f"redshift column {self.config.redshift_col} not found in input data!")
 
         # cal function to get broad types
         Ntyp, broad_types = self._get_broad_type(ngal)
         self.ntyp = Ntyp
         # trim data to between mmin and mmax
-        ref_mags = training_data[self.config.prior_band]
+        ref_mags = training_data[self.config.ref_band]
         mask = ((ref_mags >= self.config.mmin) & (ref_mags <= self.config.mmax))
         self.mags = ref_mags[mask]
         # To not screw up likelihood calculation, set objs with mag
         # brighter than m0 to value of m0
         brightmask = (self.mags < self.m0)
         self.mags[brightmask] = self.m0
         self.szs = training_data[self.config.redshift_col][mask]
@@ -234,15 +225,15 @@
         print(self.kt_arr)
         zo_arr, km_arr, a_arr = self._find_dndz_params()
         a_arr = np.abs(a_arr)
 
         self.model = dict(fo_arr=self.fo_arr, kt_arr=self.kt_arr, zo_arr=zo_arr,
                           km_arr=km_arr, a_arr=a_arr, mo=self.config.m0,
                           nt_array=self.config.nt_array)
-        self.add_data('model', self.model)
+        self.add_data("model", self.model)
 
 
 class BPZ_lite(CatEstimator):
     """CatEstimator subclass to implement basic marginalized PDF for BPZ
     In addition to the marginalized redshift PDF, we also compute several
     ancillary quantities that will be stored in the ensemble ancil data:
     zmode: mode of the PDF
@@ -250,40 +241,38 @@
     tb: integer specifying the best-fit SED *at the redshift mode*
     todds: fraction of marginalized posterior prob. of best template,
     so lower numbers mean other templates could be better fits, likely
     at other redshifts
     """
     name = "BPZ_lite"
     config_options = CatEstimator.config_options.copy()
-    config_options.update(zmin=Param(float, 0.0, msg="min z for grid"),
-                          zmax=Param(float, 3.0, msg="max z for grid"),
+    config_options.update(zmin=SHARED_PARAMS,
+                          zmax=SHARED_PARAMS,
+                          nzbins=SHARED_PARAMS,
+                          nondetect_val=SHARED_PARAMS,
+                          mag_limits=SHARED_PARAMS,
+                          bands=SHARED_PARAMS,
+                          ref_band=SHARED_PARAMS,
+                          err_bands=SHARED_PARAMS,
+                          redshift_col=SHARED_PARAMS,   
                           dz=Param(float, 0.01, msg="delta z in grid"),
-                          nzbins=Param(int, 301, msg="# of bins in zgrid"),
-                          band_names=Param(list, def_bandnames,
-                                           msg="band names to be used, *ASSUMED TO BE IN INCREASING WL ORDER!*"),
-                          band_err_names=Param(list, def_errnames,
-                                               msg="band error column names to be used * ASSUMED TO BE IN INCREASING WL ORDER!*"),
-                          nondetect_val=Param(float, 99.0, msg="value to be replaced with magnitude limit for non detects"),
                           unobserved_val=Param(float, -99.0, msg="value to be replaced with zero flux and given large errors for non-observed filters"),
                           data_path=Param(str, "None",
                                           msg="data_path (str): file path to the "
                                           "SED, FILTER, and AB directories.  If left to "
                                           "default `None` it will use the install "
-                                          "directory for rail + ../examples/estimation/data"),
-                          columns_file=Param(str, os.path.join(RAIL_BPZ_DIR, 'rail/examples/estimation/configs/test_bpz.columns'),
+                                          "directory for rail + ../examples_data/estimation_data/data"),
+                          columns_file=Param(str, os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
                                              msg="name of the file specifying the columns"),
-                          spectra_file=Param(str, 'SED/CWWSB4.list',
+                          spectra_file=Param(str, "SED/CWWSB4.list",
                                              msg="name of the file specifying the list of SEDs to use"),
-                          madau_flag=Param(str, 'no',
+                          madau_flag=Param(str, "no",
                                            msg="set to 'yes' or 'no' to set whether to include intergalactic "
                                                "Madau reddening when constructing model fluxes"),
-                          mag_limits=Param(dict, def_maglims, msg="1 sigma mag limits"),
                           no_prior=Param(bool, "False", msg="set to True if you want to run with no prior"),
-                          prior_band=Param(str, 'mag_i_lsst',
-                                           msg="specifies which band the magnitude/type prior is trained in, e.g. 'i'"),
                           p_min=Param(float, 0.005,
                                       msg="BPZ sets all values of "
                                       "the PDF that are below p_min*peak_value to 0.0, "
                                       "p_min controls that fractional cutoff"),
                           gauss_kernel=Param(float, 0.0,
                                              msg="gauss_kernel (float): BPZ "
                                              "convolves the PDF with a kernel if this is set "
@@ -295,30 +284,30 @@
                                             "large chi^2 for very very bright objects"))
 
     def __init__(self, args, comm=None):
         """Constructor, build the CatEstimator, then do BPZ specific setup
         """
         CatEstimator.__init__(self, args, comm=comm)
 
-        datapath = self.config['data_path']
+        datapath = self.config["data_path"]
         if datapath is None or datapath == "None":
-            tmpdatapath = os.path.join(RAILDIR, "rail/examples/estimation/data")
+            tmpdatapath = os.path.join(RAILDIR, "rail/examples_data/estimation_data/data")
             os.environ["BPZDATAPATH"] = tmpdatapath
             self.data_path = tmpdatapath
         else:  # pragma: no cover
             self.data_path = datapath
-            os.environ['BPZDATAPATH'] = self.data_path
+            os.environ["BPZDATAPATH"] = self.data_path
         if not os.path.exists(self.data_path):  # pragma: no cover
             raise FileNotFoundError("BPZDATAPATH " + self.data_path + " does not exist! Check value of data_path in config file!")
 
         # check on bands, errs, and prior band
-        if len(self.config.band_names) != len(self.config.band_err_names):  # pragma: no cover
-            raise ValueError("Number of bands specified in band_names must be equal to number of mag errors specified in bad_err_names!")
-        if self.config.prior_band not in self.config.band_names:  # pragma: no cover
-            raise ValueError(f"prior band not found in bands specified in band_names: {str(self.config.band_names)}")
+        if len(self.config.bands) != len(self.config.err_bands):  # pragma: no cover
+            raise ValueError("Number of bands specified in bands must be equal to number of mag errors specified in err_bands!")
+        if self.config.ref_band not in self.config.bands:  # pragma: no cover
+            raise ValueError(f"reference band not found in bands specified in bands: {str(self.config.bands)}")
 
     def _initialize_run(self):
         super()._initialize_run()
 
         # If we are not the root process then we wait for
         # the root to (potentially) create all the templates before
         # reading them ourselves.
@@ -349,15 +338,15 @@
 
         # The redshift range we will evaluate on
         self.zgrid = np.linspace(self.config.zmin, self.config.zmax, self.config.nzbins)
         z = self.zgrid
 
         data_path = self.data_path
         columns_file = self.config.columns_file
-        ignore_rows = ['M_0', 'OTHER', 'ID', 'Z_S']
+        ignore_rows = ["M_0", "OTHER", "ID", "Z_S"]
         filters = [f for f in get_str(columns_file, 0) if f not in ignore_rows]
 
         spectra_file = os.path.join(data_path, self.config.spectra_file)
         spectra = [s[:-4] for s in get_str(spectra_file)]
 
         nt = len(spectra)
         nf = len(filters)
@@ -388,16 +377,16 @@
         new_file = f"{spectrum}.{filter_}.AB"
         print(f"  Generating new AB file {new_file}....")
         ABflux(spectrum, filter_, self.config.madau_flag)
 
     def _preprocess_magnitudes(self, data):
         from desc_bpz.bpz_tools_py3 import e_mag2frac
 
-        bands = self.config.band_names
-        errs = self.config.band_err_names
+        bands = self.config.bands
+        errs = self.config.err_bands
 
         fluxdict = {}
         
         # Load the magnitudes
         zp_frac = e_mag2frac(np.array(self.config.zp_errors))
 
         # replace non-detects with 99 and mag_err with lim_mag for consistency
@@ -481,15 +470,15 @@
         unobserved = np.isclose(mags, nonobserved)
         flux[unobserved] = 0.0
         flux_err[unobserved] = 1e108
 
         # Upate the flux dictionary with new things we have calculated
         fluxdict['flux'] = flux
         fluxdict['flux_err'] = flux_err
-        m_0_col = self.config.band_names.index(self.config.prior_band)
+        m_0_col = self.config.bands.index(self.config.ref_band)
         fluxdict['mag0'] = mags[:, m_0_col]
         
         return fluxdict
 
     def _estimate_pdf(self, flux_templates, kernel, flux, flux_err, mag_0, z):
         from desc_bpz.bpz_tools_py3 import p_c_z_t
         from desc_bpz.prior_from_dict import prior_function
@@ -550,14 +539,15 @@
     def _process_chunk(self, start, end, data, first):
         """
         Run BPZ on a chunk of data
         """
         # replace non-detects, traditional BPZ had nondet=99 and err = maglim
         # put in that format here
         test_data = self._preprocess_magnitudes(data)
+        m_0_col = self.config.bands.index(self.config.ref_band)
 
         nz = len(self.zgrid)
         ng = test_data['flux'].shape[0]
 
         # Set up Gauss kernel for extra smoothing, if needed
         if self.config.gauss_kernel > 0:  # pragma: no cover
             dz = self.config.dz
```

### Comparing `pz-rail-bpz-0.0.8/src/rail/examples/estimation/configs/test_bpz.columns` & `pz-rail-bpz-0.0.9/src/rail/examples_data/estimation_data/configs/test_bpz.columns`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.8/tests/test_algos.py` & `pz-rail-bpz-0.0.9/tests/test_algos.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import yaml
 import tables_io
 from rail.core.stage import RailStage
 from rail.core.data import DataStore, TableHandle
 from rail.core.utils import RAILDIR
 from rail.core.algo_utils import one_algo
 from rail.estimation.algos import bpz_lite
-from rail.estimation.algos.bpz_version.utils import RAIL_BPZ_DIR
+from rail.bpz.utils import RAIL_BPZ_DIR
 
 import scipy.special
 sci_ver_str = scipy.__version__.split('.')
 
-
-traindata = os.path.join(RAILDIR, "rail/examples/testdata/training_100gal.hdf5")
-validdata = os.path.join(RAILDIR, "rail/examples/testdata/validation_10gal.hdf5")
 parquetdata = "./tests/validation_10gal.pq"
+traindata = os.path.join(RAILDIR, 'rail/examples_data/testdata/training_100gal.hdf5')
+validdata = os.path.join(RAILDIR, 'rail/examples_data/testdata/validation_10gal.hdf5')
+
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
 
 @pytest.mark.parametrize(
     "ntarray",
     [[8], [4, 4]]
@@ -54,19 +54,19 @@
 
 def test_bpz_lite():
     train_config_dict = {}
     estim_config_dict = {'zmin': 0.0, 'zmax': 3.0,
                          'dz': 0.01,
                          'nzbins': 301,
                          'data_path': None,
-                         'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples/estimation/configs/test_bpz.columns"),
+                         'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
                          'spectra_file': "SED/CWWSB4.list",
                          'madau_flag': 'no',
                          'no_prior': False,
-                         'prior_band': 'mag_i_lsst',
+                         'ref_band': 'mag_i_lsst',
                          'prior_file': 'hdfn_gen',
                          'p_min': 0.005,
                          'gauss_kernel': 0.0,
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
                          'mag_err_min': 0.005,
                          'hdf5_groupname': 'photometry',
                          'nt_array': [8],
@@ -86,27 +86,26 @@
         ]
 )
 def test_bpz_wHDFN_prior(inputdata, groupname):
     estim_config_dict = {'zmin': 0.0, 'zmax': 3.0,
                          'dz': 0.01,
                          'nzbins': 301,
                          'data_path': None,
-                         'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples/estimation/configs/test_bpz.columns"),
+                         'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
                          'spectra_file': "SED/CWWSB4.list",
                          'madau_flag': 'no',
-                         'bands': 'ugrizy',
-                         'prior_band': 'mag_i_lsst',
+                         'ref_band': 'mag_i_lsst',
                          'prior_file': 'flat',
                          'p_min': 0.005,
                          'gauss_kernel': 0.1,
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
                          'mag_err_min': 0.005,
                          'hdf5_groupname': groupname,
                          'nt_array': [1, 2, 5],
-                         'model': os.path.join(RAILDIR, "rail/examples/estimation/CWW_HDFN_prior.pkl")}
+                         'model': os.path.join(RAILDIR, 'rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl')}
     zb_expected = np.array([0.18, 2.88, 0.12, 0.15, 2.97, 2.78, 0.11, 0.19,
                             2.98, 2.92])
 
     validation_data = DS.read_file('validation_data', TableHandle, inputdata)
     pz = bpz_lite.BPZ_lite.make_stage(name='bpz_hdfn', **estim_config_dict)
     results = pz.estimate(validation_data)
     assert np.isclose(results.data.ancil['zmode'], zb_expected).all()
@@ -116,19 +115,18 @@
 
 def test_bpz_lite_wkernel_flatprior():
     train_config_dict = {}
     estim_config_dict = {'zmin': 0.0, 'zmax': 3.0,
                          'dz': 0.01,
                          'nzbins': 301,
                          'data_path': None,
-                         'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples/estimation/configs/test_bpz.columns"),
+                         'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
                          'spectra_file': "SED/CWWSB4.list",
                          'madau_flag': 'no',
-                         'bands': 'ugrizy',
-                         'prior_band': 'mag_i_lsst',
+                         'ref_band': 'mag_i_lsst',
                          'prior_file': 'flat',
                          'p_min': 0.005,
                          'gauss_kernel': 0.1,
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
                          'mag_err_min': 0.005,
                          'hdf5_groupname': 'photometry'}
     # zb_expected = np.array([0.18, 2.88, 0.12, 0.15, 2.97, 2.78, 0.11, 0.19,
```

### Comparing `pz-rail-bpz-0.0.8/tests/validation_10gal.pq` & `pz-rail-bpz-0.0.9/tests/validation_10gal.pq`

 * *Files identical despite different names*

