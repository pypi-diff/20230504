# Comparing `tmp/slcl1butils-2023.5.3.tar.gz` & `tmp/slcl1butils-2023.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcl1butils-2023.5.3.tar", last modified: Wed May  3 12:03:02 2023, max compression
+gzip compressed data, was "slcl1butils-2023.5.4.tar", last modified: Thu May  4 13:31:30 2023, max compression
```

## Comparing `slcl1butils-2023.5.3.tar` & `slcl1butils-2023.5.4.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.092607 slcl1butils-2023.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.084607 slcl1butils-2023.5.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.084607 slcl1butils-2023.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 12:03:02.092607 slcl1butils-2023.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.080607 slcl1butils-2023.5.3/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.084607 slcl1butils-2023.5.3/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.084607 slcl1butils-2023.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.080607 slcl1butils-2023.5.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.084607 slcl1butils-2023.5.3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/_static/css/slcl1butils.css
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.084607 slcl1butils-2023.5.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/examples/display_a_IW_L1B_xspectra.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/get_polygons_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:03:02.092607 slcl1butils-2023.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.088607 slcl1butils-2023.5.3/slcl1butils/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.088607 slcl1butils-2023.5.3/slcl1butils/coloc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/coloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/coloc/coloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.088607 slcl1butils-2023.5.3/slcl1butils/compute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/compute/compute_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/compute/cwave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/compute/macs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/compute/stack_iw_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/compute/stack_wv_l1c_monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/conversion_polar_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/cwave_parameters_computation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/get_polygons_from_l1b.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.088607 slcl1butils-2023.5.3/slcl1butils/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/plotting/display_one_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/plotting/display_xspectra_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/raster_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.092607 slcl1butils-2023.5.3/slcl1butils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/spectrum_clockwise_to_trigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/spectrum_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/symmetrize_l1b_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-05-03 12:02:41.000000 slcl1butils-2023.5.3/slcl1butils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:03:02.088607 slcl1butils-2023.5.3/slcl1butils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 12:03:02.000000 slcl1butils-2023.5.3/slcl1butils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-03 12:03:02.000000 slcl1butils-2023.5.3/slcl1butils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:03:02.000000 slcl1butils-2023.5.3/slcl1butils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-03 12:03:02.000000 slcl1butils-2023.5.3/slcl1butils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 12:03:02.000000 slcl1butils-2023.5.3/slcl1butils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 12:03:02.000000 slcl1butils-2023.5.3/slcl1butils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.503541 slcl1butils-2023.5.4/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.503541 slcl1butils-2023.5.4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/_static/css/slcl1butils.css
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/display_a_IW_L1B_xspectra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/get_polygons_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.507541 slcl1butils-2023.5.4/slcl1butils/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils/coloc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/coloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/coloc/coloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/compute_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/cwave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/macs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/stack_iw_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/compute/stack_wv_l1c_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/conversion_polar_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/cwave_parameters_computation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/get_polygons_from_l1b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/display_one_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/display_xspectra_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/spectrum_clockwise_to_trigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/spectrum_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/symmetrize_l1b_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-04 13:31:14.000000 slcl1butils-2023.5.4/slcl1butils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:31:30.511541 slcl1butils-2023.5.4/slcl1butils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 13:31:30.000000 slcl1butils-2023.5.4/slcl1butils.egg-info/top_level.txt
```

### Comparing `slcl1butils-2023.5.3/.github/workflows/publish.yml` & `slcl1butils-2023.5.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/.gitignore` & `slcl1butils-2023.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/.pre-commit-config.yaml` & `slcl1butils-2023.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/LICENSE` & `slcl1butils-2023.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/PKG-INFO` & `slcl1butils-2023.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2023.5.3
+Version: 2023.5.4
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `slcl1butils-2023.5.3/docs/Makefile` & `slcl1butils-2023.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/docs/conf.py` & `slcl1butils-2023.5.4/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,28 +36,39 @@
     'nbsphinx',
     'jupyter_sphinx',
 ]
 # order by source
 autodoc_member_order = 'bysource'
 
 # Napoleon settings
-napoleon_google_docstring = True
+napoleon_google_docstring = False
 napoleon_numpy_docstring = True
 napoleon_include_init_with_doc = False
 napoleon_include_private_with_doc = False
 napoleon_include_special_with_doc = True
 napoleon_use_admonition_for_examples = False
 napoleon_use_admonition_for_notes = False
 napoleon_use_admonition_for_references = False
 napoleon_use_ivar = False
 napoleon_use_param = True
 napoleon_use_rtype = True
 napoleon_type_aliases = None
 
 
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/3/", None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
+    "numpy": ("https://numpy.org/doc/stable", None),
+    "dask": ("https://docs.dask.org/en/latest", None),
+    "xarray": ("https://docs.xarray.dev/en/latest/", None),
+    "rasterio": ("https://rasterio.readthedocs.io/en/latest/", None),
+    "datatree": ("https://xarray-datatree.readthedocs.io/en/latest/", None)
+}
+
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
```

### Comparing `slcl1butils-2023.5.3/docs/examples/display_a_IW_L1B_xspectra.ipynb` & `slcl1butils-2023.5.4/docs/examples/display_a_IW_L1B_xspectra.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb` & `slcl1butils-2023.5.4/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.4/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.4/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/docs/index.rst` & `slcl1butils-2023.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/docs/installing.rst` & `slcl1butils-2023.5.4/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/docs/oceanspectrumSAR.png` & `slcl1butils-2023.5.4/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/get_polygons_from_l1b.py` & `slcl1butils-2023.5.4/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/pyproject.toml` & `slcl1butils-2023.5.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "xarray",
     "numpy",
     "netCDF4",
     "shapely",
-    "xrft",
     "xarray-datatree",
     "importlib_resources",
     'tqdm'
 ]
 dynamic = ["version"]
 
 [build-system]
@@ -38,10 +37,10 @@
 profile = "black"
 skip_gitignore = true
 float_to_top = true
 default_section = "THIRDPARTY"
 known_first_party = "slcl1butils"
 
 [project.scripts]
-do_L1C_SAFE_from_L1B_SAFE = "slcl1butils.scripts.do_L1C_SAFE_from_L1B_SAFE:main"
+do_IW_L1C_SAFE_from_L1B_SAFE = "slcl1butils.scripts.do_IW_L1C_SAFE_from_L1B_SAFE:main"
 do_WV_L1C_SAFE_from_L1B_SAFE = "slcl1butils.scripts.do_WV_L1C_SAFE_from_L1B_SAFE:main"
 stack_WV_L1C_to_ZARR = 'slcl1butils.compute.stack_wv_l1c_monthly:main'
```

### Comparing `slcl1butils-2023.5.3/slcl1butils/coloc/coloc.py` & `slcl1butils-2023.5.4/slcl1butils/coloc/coloc.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/compute/compute_from_l1b.py` & `slcl1butils-2023.5.4/slcl1butils/compute/compute_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/compute/cwave.py` & `slcl1butils-2023.5.4/slcl1butils/compute/cwave.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/compute/macs.py` & `slcl1butils-2023.5.4/slcl1butils/compute/macs.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/compute/stack_iw_l1b.py` & `slcl1butils-2023.5.4/slcl1butils/compute/stack_iw_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/compute/stack_wv_l1c_monthly.py` & `slcl1butils-2023.5.4/slcl1butils/compute/stack_wv_l1c_monthly.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/conversion_polar_cartesian.py` & `slcl1butils-2023.5.4/slcl1butils/conversion_polar_cartesian.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/cwave_parameters_computation_example.ipynb` & `slcl1butils-2023.5.4/slcl1butils/cwave_parameters_computation_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/get_config.py` & `slcl1butils-2023.5.4/slcl1butils/get_config.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/get_polygons_from_l1b.py` & `slcl1butils-2023.5.4/slcl1butils/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py` & `slcl1butils-2023.5.4/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/plotting/display_one_spectra.py` & `slcl1butils-2023.5.4/slcl1butils/plotting/display_one_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/plotting/display_xspectra_grid.py` & `slcl1butils-2023.5.4/slcl1butils/plotting/display_xspectra_grid.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.4/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.4/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py` & `slcl1butils-2023.5.4/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/raster_readers.py` & `slcl1butils-2023.5.4/slcl1butils/raster_readers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.4/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.5.4/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.4/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/spectrum_clockwise_to_trigo.py` & `slcl1butils-2023.5.4/slcl1butils/spectrum_clockwise_to_trigo.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/spectrum_rotation.py` & `slcl1butils-2023.5.4/slcl1butils/spectrum_rotation.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils/symmetrize_l1b_spectra.py` & `slcl1butils-2023.5.4/slcl1butils/symmetrize_l1b_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.3/slcl1butils.egg-info/PKG-INFO` & `slcl1butils-2023.5.4/slcl1butils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2023.5.3
+Version: 2023.5.4
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `slcl1butils-2023.5.3/slcl1butils.egg-info/SOURCES.txt` & `slcl1butils-2023.5.4/slcl1butils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -52,10 +52,12 @@
 slcl1butils/plotting/__init__.py
 slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
 slcl1butils/plotting/display_one_spectra.py
 slcl1butils/plotting/display_xspectra_grid.py
 slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
 slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
 slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
-slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py
+slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
+slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
+slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
 slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
 slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
```

