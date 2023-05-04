# Comparing `tmp/napari-spatialdata-0.1.0.tar.gz` & `tmp/napari-spatialdata-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-spatialdata-0.1.0.tar", last modified: Mon Aug 15 13:18:48 2022, max compression
+gzip compressed data, was "napari-spatialdata-0.2.1.tar", last modified: Thu May  4 11:08:23 2023, max compression
```

## Comparing `napari-spatialdata-0.1.0.tar` & `napari-spatialdata-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.442051 napari-spatialdata-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.434051 napari-spatialdata-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.438051 napari-spatialdata-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/.mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.438051 napari-spatialdata-0.1.0/.napari/
--rw-r--r--   0 runner    (1001) docker     (121)     4199 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4120 2022-08-15 13:18:48.442051 napari-spatialdata-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.438051 napari-spatialdata-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7505 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     9601 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7029 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.438051 napari-spatialdata-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/examples/raster_points_regions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/examples/raster_regions.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/examples/shape_regions.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-08-15 13:18:48.442051 napari-spatialdata-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.438051 napari-spatialdata-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.438051 napari-spatialdata-0.1.0/src/napari_spatialdata/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.438051 napari-spatialdata-0.1.0/src/napari_spatialdata/_constants/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/_constants/_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/_constants/_pkg_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/_constants/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10094 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5819 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8284 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/_view.py
--rw-r--r--   0 runner    (1001) docker     (121)    15578 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/src/napari_spatialdata/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.438051 napari-spatialdata-0.1.0/src/napari_spatialdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4120 2022-08-15 13:18:48.000000 napari-spatialdata-0.1.0/src/napari_spatialdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-08-15 13:18:48.000000 napari-spatialdata-0.1.0/src/napari_spatialdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 13:18:48.000000 napari-spatialdata-0.1.0/src/napari_spatialdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-15 13:18:48.000000 napari-spatialdata-0.1.0/src/napari_spatialdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-08-15 13:18:48.000000 napari-spatialdata-0.1.0/src/napari_spatialdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-15 13:18:48.000000 napari-spatialdata-0.1.0/src/napari_spatialdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:48.442051 napari-spatialdata-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4928 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4676 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-08-15 13:18:30.000000 napari-spatialdata-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.909586 napari-spatialdata-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/_templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/extensions/typed_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  5521635 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/notebooks/spatialdata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/template_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.921587 napari-spatialdata-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/raster_points_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/raster_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/shape_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/spatialdata_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.909586 napari-spatialdata-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/src/napari_spatialdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_categoricals_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_pkg_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/test_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/test_spatialdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tox.ini
```

### Comparing `napari-spatialdata-0.1.0/.github/workflows/test_and_deploy.yml` & `napari-spatialdata-0.2.1/.github/workflows/test_and_deploy.yml`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
-        platform: [ubuntu-latest] # [ubuntu-latest, windows-latest, macos-latest]
-        python-version: [3.8, "3.10"] # [3.8, 3.9, "3.10"]
+        platform: [ubuntu-latest, macos-latest] # [ubuntu-latest, windows-latest, macos-latest]
+        python-version: [3.9, "3.10"] # [3.8, 3.9, "3.10"]
 
     steps:
       - uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
```

### Comparing `napari-spatialdata-0.1.0/.gitignore` & `napari-spatialdata-0.2.1/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -94,7 +94,11 @@
 *.swp
 
 # vscode
 .vscode
 
 # files
 *.h5ad
+
+# docs
+/docs/generated/
+/docs/_build/
```

### Comparing `napari-spatialdata-0.1.0/.mypy.ini` & `napari-spatialdata-0.2.1/.mypy.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [mypy]
 mypy_path = napari-spatialdata
-python_version = 3.8
+python_version = 3.9
 plugins = numpy.typing.mypy_plugin
 
 ignore_errors = False
 warn_redundant_casts = True
 warn_unused_configs = True
 warn_unused_ignores = True
 
@@ -29,7 +29,10 @@
 error_summary = True
 
 [mypy-tests.*]
 ignore_errors = True
 
 [mypy-docs.*]
 ignore_errors = True
+
+[mypy-docs.extensions.*.py]
+ignore_errors = True
```

### Comparing `napari-spatialdata-0.1.0/.napari/DESCRIPTION.md` & `napari-spatialdata-0.2.1/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.1.0/LICENSE` & `napari-spatialdata-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.1.0/PKG-INFO` & `napari-spatialdata-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.1.0
+Version: 0.2.1
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
@@ -12,22 +12,22 @@
 Project-URL: User Support, https://github.com/scverse/napari-spatialdata/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: testing
+Provides-Extra: test
+Provides-Extra: doc
 License-File: LICENSE
 
 # napari-spatialdata
 
 [![License](https://img.shields.io/pypi/l/napari-spatialdata.svg?color=green)](https://github.com/scverse/napari-spatialdata/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-spatialdata.svg?color=green)](https://pypi.org/project/napari-spatialdata)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-spatialdata.svg?color=green)](https://python.org)
@@ -46,50 +46,53 @@
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/plugins/stable/index.html
 -->
 
-# UNDER DEVELOPMENT
+## Installation
 
-Clone repo and `pip install -e .`.
-Run examples e.g. `python shape_regions.py` or via notebook for the shape export function.
+You can install `napari-spatialdata` via [pip]:
 
-More documentation on usage will be added later on.
+    pip install napari-spatialdata
 
-Expect breaking changes.
+## Development Version
 
-## Installation
+You can install `napari-spatialdata` from Github with:
 
-You can install `napari-spatialdata` via [pip]:
+    pip install git+https://github.com/scverse/napari-spatialdata
 
-    pip install napari-spatialdata
+Or, you can also install in editable mode after cloning the repo by:
+
+    git clone https://github.com/scverse/napari-spatialdata
+    cd napari-spatialdata
+    pip install -e .
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-spatialdata" is free and open source software
 
 ## Issues
 
-If you encounter any problems, please [file an issue] along with a detailed description.
+If you encounter any problems, please file an [issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [mit]: http://opensource.org/licenses/MIT
 [bsd-3]: http://opensource.org/licenses/BSD-3-Clause
 [gnu gpl v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
 [gnu lgpl v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
 [apache software license 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [mozilla public license 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-[napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [pypi]: https://pypi.org/
+[issue]: https://github.com/scverse/napari-spatialdata/issues
```

### Comparing `napari-spatialdata-0.1.0/README.md` & `napari-spatialdata-0.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -18,50 +18,53 @@
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/plugins/stable/index.html
 -->
 
-# UNDER DEVELOPMENT
+## Installation
 
-Clone repo and `pip install -e .`.
-Run examples e.g. `python shape_regions.py` or via notebook for the shape export function.
+You can install `napari-spatialdata` via [pip]:
 
-More documentation on usage will be added later on.
+    pip install napari-spatialdata
 
-Expect breaking changes.
+## Development Version
 
-## Installation
+You can install `napari-spatialdata` from Github with:
 
-You can install `napari-spatialdata` via [pip]:
+    pip install git+https://github.com/scverse/napari-spatialdata
 
-    pip install napari-spatialdata
+Or, you can also install in editable mode after cloning the repo by:
+
+    git clone https://github.com/scverse/napari-spatialdata
+    cd napari-spatialdata
+    pip install -e .
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-spatialdata" is free and open source software
 
 ## Issues
 
-If you encounter any problems, please [file an issue] along with a detailed description.
+If you encounter any problems, please file an [issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [mit]: http://opensource.org/licenses/MIT
 [bsd-3]: http://opensource.org/licenses/BSD-3-Clause
 [gnu gpl v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
 [gnu lgpl v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
 [apache software license 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [mozilla public license 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-[napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [pypi]: https://pypi.org/
+[issue]: https://github.com/scverse/napari-spatialdata/issues
```

### Comparing `napari-spatialdata-0.1.0/examples/raster_points_regions.py` & `napari-spatialdata-0.2.1/examples/raster_points_regions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import napari
 import anndata as ad
+import napari
 
 adata = ad.read("./adata_nanostring_points.h5ad")
 
 img1 = adata.uns["spatial"]["1"]["images"]["hires"]
 img2 = adata.uns["spatial"]["2"]["images"]["hires"]
 
 label1 = adata.uns["spatial"]["1"]["images"]["segmentation"]
@@ -22,15 +22,14 @@
     name="image1",
 )
 viewer.add_labels(
     label1,
     name="label1",
     metadata={
         "adata": adata1,
-        "library_id": "1",
         "labels_key": "cell_ID",
         "points": points1,
         "point_diameter": 10,
     },  # adata in labels layer will color segments
 )
 viewer.add_image(
     img2,
@@ -38,15 +37,14 @@
     name="image2",
 )
 viewer.add_labels(
     label2,
     name="label2",
     metadata={
         "adata": adata2,
-        "library_id": "2",
         "labels_key": "cell_ID",
         "points": points2,
         "point_diameter": 10,
     },  # adata in labels layer will color segments
 )
 
 if __name__ == "__main__":
```

### Comparing `napari-spatialdata-0.1.0/examples/raster_regions.py` & `napari-spatialdata-0.2.1/examples/raster_regions.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,38 +12,37 @@
 img2 = adata.uns["spatial"]["point16"]["images"]["hires"].copy()
 label1 = adata.uns["spatial"]["point8"]["images"]["segmentation"].copy()
 label2 = adata.uns["spatial"]["point16"]["images"]["segmentation"].copy()
 adata1.obsm.pop("X_scanorama")
 adata2.obsm.pop("X_umap")
 adata1.obs.pop("batch")
 adata1 = adata1[:, 0:10].copy()
-adata1.obsm["obs_copy"] = adata1.obs.iloc[:, 0:5].copy()
 adata1.layers["counts"] = adata1.X.copy()
 
 viewer = napari.Viewer()
 viewer.add_image(
     img1,
     rgb=True,
     name="image1",
-    metadata={"adata": adata1, "library_id": "point8"},  # adata in image layers will plot points
+    metadata={"adata": adata1},  # adata in image layers will plot points
     scale=(1, 1),
 )
 viewer.add_labels(
     label1,
     name="label1",
     metadata={
         "adata": adata1,
-        "library_id": "point8",
         "labels_key": "cell_id",
+        "colormap": "inferno",
     },  # adata in labels layer will color segments
 )
 viewer.add_labels(
     label2,
     name="label2",
-    metadata={"adata": adata2, "library_id": "point16", "labels_key": "cell_id"},
+    metadata={"adata": adata2, "labels_key": "cell_id"},
 )
 
 viewer.scale_bar.visible = True
 viewer.scale_bar.unit = "um"
 
 if __name__ == "__main__":
     napari.run()
```

### Comparing `napari-spatialdata-0.1.0/setup.cfg` & `napari-spatialdata-0.2.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [metadata]
 name = napari-spatialdata
 url = https://github.com/scverse/napari-spatialdata.git
 author = giovanni palla
 author_email = giov.pll@gmail.com
-version = 0.1.0
 project_urls = 
 	Bug Tracker = https://github.com/scverse/napari-spatialdata/issues
 	Documentation = https://github.com/scverse/napari-spatialdata#README.md
 	Source Code = https://github.com/scverse/napari-spatialdata
 	User Support = https://github.com/scverse/napari-spatialdata/issues
 license = BSD-3-Clause
 description = Interactive visualization of spatial omics data with napari
@@ -16,47 +15,57 @@
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
 	Framework :: napari
 	Topic :: Software Development :: Testing
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Operating System :: OS Independent
 	License :: OSI Approved :: BSD License
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.8
+python_requires = >=3.9
 setup_requires = setuptools_scm
 install_requires = 
 	numpy
 	magicgui
 	qtpy
 	numba
 	anndata
 	scikit-image
-	squidpy
 	napari[all]
 	loguru
+	napari-matplotlib
+	scikit-learn
+	spatialdata
 package_dir = 
 	=src
 
 [options.extras_require]
-testing = 
+test = 
 	tox
 	pytest  # https://docs.pytest.org/en/latest/contents.html
 	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
 	pytest-qt  # https://pytest-qt.readthedocs.io/en/latest/
-	napari
 	pre-commit>=2.9.0
 	towncrier>=21.3.0
+doc = 
+	sphinx>=4
+	sphinx-book-theme>=0.3.3
+	myst-nb
+	sphinxcontrib-bibtex>=1.0.0
+	sphinx-autodoc-typehints
+	ipykernel
+	ipython
+	sphinx-copybutton
+	sphinx-qt-documentation
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 napari_spatiadata = napari.yaml
 
@@ -66,14 +75,11 @@
 
 [tool:pytest]
 python_files = test_*.py
 testpaths = tests/
 xfail_strict = true
 qt_api = pyqt5
 
-[flake8]
-max-line-length = 88
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `napari-spatialdata-0.1.0/src/napari_spatialdata/_constants/_pkg_constants.py` & `napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_pkg_constants.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.1.0/src/napari_spatialdata/_constants/_utils.py` & `napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from abc import ABC, ABCMeta
 from enum import Enum, EnumMeta
-from typing import Any, Dict, Type, Tuple, Callable
 from functools import wraps
+from typing import Any, Callable, Dict, Tuple, Type
 
 
 def _pretty_raise_enum(cls: Type["ModeEnum"], fun: Callable[..., Any]) -> Callable[..., Any]:
     @wraps(fun)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         try:
             return fun(*args, **kwargs)
         except ValueError as e:
             _cls, value, *_ = args
             e.args = (cls._format(value),)
             raise e
 
     if not issubclass(cls, ErrorFormatterABC):
         raise TypeError(f"Class `{cls}` must be subtype of `ErrorFormatterABC`.")
-    elif not len(cls.__members__):
+    elif not len(cls.__members__):  # noqa: RET506
         # empty enum, for class hierarchy
         return fun
 
     return wrapper
 
 
 class ErrorFormatterABC(ABC):
@@ -51,15 +51,15 @@
     def __call__(cls, *args: Any, **kw: Any) -> EnumMeta:  # type: ignore[override]
         if getattr(cls, "__error_format__", None) is None:
             raise TypeError(f"Can't instantiate class `{cls.__name__}` without `__error_format__` class attribute.")
         return super().__call__(*args, **kw)  # type: ignore[no-any-return]
 
     def __new__(cls, clsname: str, bases: Tuple[EnumMeta, ...], namespace: Dict[str, Any]) -> "ABCEnumMeta":
         res: ABCEnumMeta = super().__new__(cls, clsname, bases, namespace)  # type: ignore[arg-type]
-        res.__new__ = _pretty_raise_enum(res, res.__new__)  # type: ignore[assignment,arg-type]
+        res.__new__ = _pretty_raise_enum(res, res.__new__)  # type: ignore[method-assign,arg-type]
         return res
 
 
 class ModeEnum(ErrorFormatterABC, PrettyEnum, metaclass=ABCEnumMeta):
     """Enum which prints available values when invalid value has been passed."""
 
     @property
```

### Comparing `napari-spatialdata-0.1.0/src/napari_spatialdata/_model.py` & `napari-spatialdata-0.2.1/src/napari_spatialdata/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from typing import Any, Tuple, Union, Optional
-from dataclasses import field, dataclass
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Any, Optional, Tuple, Union
 
-from anndata import AnnData
-from napari.layers import Layer
-from napari.utils.events import Event, EmitterGroup
 import numpy as np
 import pandas as pd
+from anndata import AnnData
+from napari.layers import Layer
+from napari.utils.events import EmitterGroup, Event
 
-from napari_spatialdata._utils import NDArrayA, _ensure_dense_vector
 from napari_spatialdata._constants._constants import Symbol
 from napari_spatialdata._constants._pkg_constants import Key
+from napari_spatialdata._utils import NDArrayA, _ensure_dense_vector
 
 __all__ = ["ImageModel"]
 
 
 @dataclass
 class ImageModel:
     """Model which holds the data for interactive visualization."""
 
     events: EmitterGroup = field(init=False, default=None, repr=True)
     _layer: Layer = field(init=False, default=None, repr=True)
     _adata: AnnData = field(init=False, default=None, repr=True)
     _spatial_key: str = field(default=Key.obsm.spatial, repr=False)
-    _library_id: Optional[str] = field(init=False, default=None, repr=True)
     _adata_layer: Optional[str] = field(init=False, default=None, repr=False)
     _label_key: Optional[str] = field(default=None, repr=True)
     _coordinates: Optional[NDArrayA] = field(init=False, default=None, repr=True)
     _points_coordinates: Optional[NDArrayA] = field(init=False, default=None, repr=True)
     _points_var: Optional[pd.Series] = field(init=False, default=None, repr=True)
     _scale: Optional[float] = field(init=False, default=None)
 
@@ -61,16 +60,15 @@
         The available items.
         """
         if attr in ("obs", "obsm"):
             return tuple(map(str, getattr(self.adata, attr).keys()))
         if attr == "points":
             if self.points_var is not None:
                 return tuple(map(str, self.points_var.unique()))
-            else:
-                return tuple(["No points found."])  # noqa: C409
+            return tuple(["No points found."])  # noqa: C409
         return tuple(map(str, getattr(self.adata, attr).index))
 
     @_ensure_dense_vector
     def get_obs(
         self, name: str, **_: Any
     ) -> Tuple[Optional[Union[pd.Series, NDArrayA]], str]:  # TODO(giovp): fix docstring
         """
@@ -204,39 +202,33 @@
         return self._spatial_key
 
     @spatial_key.setter
     def spatial_key(self, key: str) -> None:
         self._spatial_key = key
 
     @property
-    def library_id(self) -> Optional[str]:  # noqa: D102
-        return self._library_id
-
-    @library_id.setter
-    def library_id(self, library_id: str) -> None:
-        self._library_id = library_id
-
-    @property
     def adata_layer(self) -> Optional[str]:  # noqa: D102
         return self._adata_layer
 
     @adata_layer.setter
     def adata_layer(self, adata_layer: str) -> None:
         self._adata_layer = adata_layer
 
     @property
     def coordinates(self) -> NDArrayA:  # noqa: D102
-        return self._coordinates
+        return self._coordinates  # type: ignore[return-value]
 
     @coordinates.setter
     def coordinates(self, coordinates: NDArrayA) -> None:
         self._coordinates = coordinates
 
     @property
     def points_coordinates(self) -> NDArrayA:  # noqa: D102
+        if TYPE_CHECKING:
+            assert self._points_coordinates is not None
         return self._points_coordinates
 
     @points_coordinates.setter
     def points_coordinates(self, points_coordinates: NDArrayA) -> None:
         self._points_coordinates = points_coordinates
 
     @property
@@ -252,27 +244,27 @@
         return self._scale
 
     @scale.setter
     def scale(self, scale: float) -> None:
         self._scale = scale
 
     @property
-    def spot_diameter(self) -> NDArrayA:  # noqa: D102
+    def spot_diameter(self) -> Union[NDArrayA, float]:  # noqa: D102
         return self._spot_diameter
 
     @spot_diameter.setter
-    def spot_diameter(self, spot_diameter: NDArrayA) -> None:
+    def spot_diameter(self, spot_diameter: Union[NDArrayA, float]) -> None:
         self._spot_diameter = spot_diameter
 
     @property
-    def point_diameter(self) -> NDArrayA:  # noqa: D102
+    def point_diameter(self) -> Union[NDArrayA, float]:  # noqa: D102
         return self._point_diameter
 
     @point_diameter.setter
-    def point_diameter(self, point_diameter: NDArrayA) -> None:
+    def point_diameter(self, point_diameter: Union[NDArrayA, float]) -> None:
         self._point_diameter = point_diameter
 
     @property
     def labels_key(self) -> Optional[str]:  # noqa: D102
         return self._labels_key
 
     @labels_key.setter
```

### Comparing `napari-spatialdata-0.1.0/src/napari_spatialdata/_utils.py` & `napari-spatialdata-0.2.1/src/napari_spatialdata/_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from __future__ import annotations
 
-from typing import Any, Tuple, Union, Callable, Optional, Sequence, TYPE_CHECKING
 from functools import wraps
+from typing import TYPE_CHECKING, Any, Callable, Optional, Sequence, Tuple, Union
 
-from numba import njit, prange
-from loguru import logger
+import numpy as np
+import pandas as pd
 from anndata import AnnData
-from scipy.sparse import issparse, spmatrix
-from scipy.spatial import KDTree
+from dask.dataframe.core import DataFrame as DaskDataFrame
+from geopandas import GeoDataFrame
+from loguru import logger
+from matplotlib.colors import is_color_like, to_rgb
+from multiscale_spatial_image.multiscale_spatial_image import MultiscaleSpatialImage
+from numba import njit, prange
 from pandas.api.types import infer_dtype, is_categorical_dtype
-from matplotlib.colors import to_hex, to_rgb
-from scanpy.plotting._utils import add_colors_for_categorical_sample_annotation
 from pandas.core.dtypes.common import (
     is_bool_dtype,
-    is_object_dtype,
-    is_string_dtype,
     is_integer_dtype,
     is_numeric_dtype,
+    is_object_dtype,
+    is_string_dtype,
 )
-import numpy as np
-import pandas as pd
+from scipy.sparse import issparse, spmatrix
+from scipy.spatial import KDTree
+from spatial_image import SpatialImage
+from spatialdata.models import SpatialElement
+from spatialdata.transformations import get_transformation
 
+from napari_spatialdata._categoricals_utils import (
+    add_colors_for_categorical_sample_annotation,
+)
 from napari_spatialdata._constants._pkg_constants import Key
 
 try:
     from numpy.typing import NDArray
 
     NDArrayA = NDArray[Any]
 except (ImportError, TypeError):
@@ -70,58 +78,87 @@
             raise ValueError(f"Expected 1-dimensional array, found `{res.ndim}`.")
 
         return (_min_max_norm(res) if normalize else res), fmt
 
     return decorator
 
 
-def _get_categorical(
+def _get_palette(
     adata: AnnData,
     key: str,
     palette: Optional[str] = None,
     vec: Optional[pd.Series] = None,
-) -> NDArrayA:
+) -> dict[Any, Any]:
+    if key not in adata.obs:
+        raise KeyError("Missing key!")  # TODO: Improve error message
 
-    if vec is not None:
-        if not is_categorical_dtype(vec):
-            raise TypeError(f"Expected a `categorical` type, found `{infer_dtype(vec)}`.")
-        if key in adata.obs:
-            logger.debug(f"Overwriting `adata.obs[{key!r}]`.")
+    return dict(zip(adata.obs[key].cat.categories, [to_rgb(i) for i in adata.uns[Key.uns.colors(key)]]))
 
-        adata.obs[key] = vec.values
+
+def _set_palette(
+    adata: AnnData,
+    key: str,
+    palette: Optional[str] = None,
+    vec: Optional[pd.Series] = None,
+) -> dict[Any, Any]:
+    if vec is not None and not is_categorical_dtype(vec):
+        raise TypeError(f"Expected a `categorical` type, found `{infer_dtype(vec)}`.")
 
     add_colors_for_categorical_sample_annotation(
-        adata, key=key, force_update_colors=palette is not None, palette=palette
+        adata,
+        key=key,
+        vec=vec,
+        force_update_colors=palette is not None,
+        palette=palette,  # type: ignore[arg-type]
     )
-    col_dict = dict(zip(adata.obs[key].cat.categories, [to_rgb(i) for i in adata.uns[Key.uns.colors(key)]]))
+    vec = vec if vec is not None else adata.obs[key]
+    #
+    return dict(zip(vec.cat.categories, [to_rgb(i) for i in adata.uns[Key.uns.colors(key)]]))
+
+
+def _get_categorical(
+    adata: AnnData,
+    key: str,
+    vec: Optional[pd.Series] = None,
+    palette: Optional[str] = None,
+    colordict: Union[pd.Series, dict[Any, Any], None] = None,
+) -> NDArrayA:
+    categorical = vec if vec is not None else adata.obs[key]
+    if not isinstance(colordict, dict):
+        col_dict = _set_palette(adata, key, palette, colordict)
+    else:
+        col_dict = colordict
+        for cat in colordict:
+            if cat not in categorical.cat.categories:
+                raise ValueError(
+                    f"The key `{cat}` in the given dictionary is not an existing category in anndata[`{key}`]."
+                )
+            elif not is_color_like(colordict[cat]):  # noqa: RET506
+                raise ValueError(f"`{colordict[cat]}` is not an acceptable color.")
 
-    return np.array([col_dict[v] for v in adata.obs[key]])
+    logger.debug(f"KEY: {key}")
+    return np.array([col_dict[v] for v in categorical])
 
 
-def _position_cluster_labels(coords: NDArrayA, clusters: pd.Series, colors: NDArrayA) -> dict[str, NDArrayA]:
+def _position_cluster_labels(coords: NDArrayA, clusters: pd.Series) -> dict[str, NDArrayA]:
     if not is_categorical_dtype(clusters):
         raise TypeError(f"Expected `clusters` to be `categorical`, found `{infer_dtype(clusters)}`.")
-
     coords = coords[:, 1:]
     df = pd.DataFrame(coords)
     df["clusters"] = clusters.values
     df = df.groupby("clusters")[[0, 1]].apply(lambda g: list(np.median(g.values, axis=0)))
-    df = pd.DataFrame(list(df), index=df.index)
+    df = pd.DataFrame(list(df), index=df.index).dropna()
     kdtree = KDTree(coords)
     clusters = np.full(len(coords), fill_value="", dtype=object)
     # index consists of the categories that need not be string
     clusters[kdtree.query(df.values)[1]] = df.index.astype(str)
-    # napari v0.4.9 - properties must be 1-D in napari/layers/points/points.py:581
-    colors = np.array([to_hex(col) for col in colors])
-    colors = np.array([col if not len(cl) else to_hex((0, 0, 0)) for cl, col in zip(clusters, colors)])
-    return {"clusters": clusters, "colors": colors}
+    return {"clusters": clusters}
 
 
 def _min_max_norm(vec: Union[spmatrix, NDArrayA]) -> NDArrayA:
-
     if issparse(vec):
         if TYPE_CHECKING:
             assert isinstance(vec, spmatrix)
         vec = vec.toarray().squeeze()
     vec = np.asarray(vec, dtype=np.float64)
     if vec.ndim != 1:
         raise ValueError(f"Expected `1` dimension, found `{vec.ndim}`.")
@@ -129,14 +166,35 @@
     maxx, minn = np.nanmax(vec), np.nanmin(vec)
 
     return (  # type: ignore[no-any-return]
         np.ones_like(vec) if np.isclose(minn, maxx) else ((vec - minn) / (maxx - minn))
     )
 
 
+def _get_transform(element: SpatialElement, coordinate_system_name: Optional[str] = None) -> NDArrayA:
+    affine: NDArrayA
+    transformations = get_transformation(element, get_all=True)
+    cs = transformations.keys().__iter__().__next__() if coordinate_system_name is None else coordinate_system_name
+    ct = transformations[cs]
+    affine = ct.to_affine_matrix(input_axes=("y", "x"), output_axes=("y", "x"))
+
+    if not isinstance(element, (SpatialImage, MultiscaleSpatialImage, AnnData, DaskDataFrame, GeoDataFrame)):
+        raise RuntimeError("Cannot get transform for {type(element)}")
+    # elif isinstance(element, (AnnData, DaskDataFrame, GeoDataFrame)):
+    #    return affine
+    #    from spatialdata.transformations import Affine, Sequence, MapAxis
+    #    new_affine = Sequence(
+    #        [MapAxis({"x": "y", "y": "x"}), Affine(affine, input_axes=("y", "x"), output_axes=("y", "x"))]
+    #    )
+    #    new_matrix = new_affine.to_affine_matrix(input_axes=("y", "x"), output_axes=("y", "x"))
+
+    #    return new_matrix
+    return affine
+
+
 @njit(cache=True, fastmath=True)
 def _point_inside_triangles(triangles: NDArrayA) -> np.bool_:
     # modified from napari
     AB = triangles[:, 1, :] - triangles[:, 0, :]
     AC = triangles[:, 2, :] - triangles[:, 0, :]
     BC = triangles[:, 2, :] - triangles[:, 1, :]
 
@@ -145,15 +203,15 @@
     s_BC = -BC[:, 0] * triangles[:, 1, 1] + BC[:, 1] * triangles[:, 1, 0] >= 0
 
     return np.any((s_AB != s_AC) & (s_AB == s_BC))
 
 
 @njit(parallel=True)
 def _points_inside_triangles(points: NDArrayA, triangles: NDArrayA) -> NDArrayA:
-    out = np.empty(  # type: ignore[var-annotated]
+    out = np.empty(
         len(
             points,
         ),
         dtype=np.bool_,
     )
     for i in prange(len(out)):
         out[i] = _point_inside_triangles(triangles - points[i])
```

### Comparing `napari-spatialdata-0.1.0/src/napari_spatialdata/_view.py` & `napari-spatialdata-0.2.1/src/napari_spatialdata/_view.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,151 @@
-from typing import Any, Optional, Sequence, FrozenSet
+from typing import Any, FrozenSet, Optional, Sequence
 
-from loguru import logger
-from anndata import AnnData
-from magicgui import magicgui
-from napari.layers import Layer, Labels
-from napari.viewer import Viewer
-from qtpy.QtWidgets import QLabel, QWidget, QComboBox, QVBoxLayout
-import numpy as np
 import napari
+import numpy as np
 import pandas as pd
+from anndata import AnnData
+from loguru import logger
+from napari.layers import Labels
+from napari.viewer import Viewer
+from qtpy.QtWidgets import (
+    QComboBox,
+    QGridLayout,
+    QLabel,
+    QPushButton,
+    QVBoxLayout,
+    QWidget,
+)
 
+from napari_spatialdata._constants._pkg_constants import Key
 from napari_spatialdata._model import ImageModel
+from napari_spatialdata._scatterwidgets import AxisWidgets, MatplotlibWidget
 from napari_spatialdata._utils import (
     NDArrayA,
     _get_categorical,
     _points_inside_triangles,
 )
 from napari_spatialdata._widgets import (
-    CBarWidget,
     AListWidget,
-    ObsmIndexWidget,
+    CBarWidget,
+    ComponentWidget,
     RangeSliderWidget,
 )
-from napari_spatialdata._constants._pkg_constants import Key
 
-__all__ = ["QtAdataViewWidget"]
+__all__ = ["QtAdataViewWidget", "QtAdataScatterWidget"]
 
 
-class QtAdataViewWidget(QWidget):
+class QtAdataScatterWidget(QWidget):
     """Adata viewer widget."""
 
     def __init__(self, viewer: Viewer):
         super().__init__()
 
         self._viewer = viewer
         self._model = ImageModel()
 
-        self._layer_selection_widget = magicgui(
-            self._select_layer,
-            layer={"choices": self._get_layer},
-            auto_call=True,
-            call_button=False,
+        self._select_layer()
+        self._viewer.layers.selection.events.changed.connect(self._select_layer)
+        self._viewer.layers.selection.events.changed.connect(self._on_selection)
+
+        self.setLayout(QGridLayout())
+
+        # Matplotlib
+
+        self.matplotlib_widget = MatplotlibWidget(self.viewer, self.model)
+        self.layout().addWidget(self.matplotlib_widget, 1, 0, 1, 3)
+
+        self.x_widget = AxisWidgets(self.viewer, self.model, "X-axis")
+        self.layout().addWidget(self.x_widget, 2, 0, 6, 1)
+
+        self.y_widget = AxisWidgets(self.viewer, self.model, "Y-axis")
+        self.layout().addWidget(self.y_widget, 2, 1, 6, 1)
+
+        self.color_widget = AxisWidgets(self.viewer, self.model, "Color", True)
+        self.layout().addWidget(self.color_widget, 2, 2, 6, 1)
+
+        self.plot_button_widget = QPushButton("Plot")
+        self.plot_button_widget.clicked.connect(
+            lambda: self.matplotlib_widget._onClick(
+                self.x_widget.widget.data,
+                self.y_widget.widget.data,
+                self.color_widget.widget.data,  # type:ignore[arg-type]
+                self.x_widget.getFormattedLabel(),
+                self.y_widget.getFormattedLabel(),
+                self.color_widget.getFormattedLabel(),
+            )
         )
-        self._layer_selection_widget()
+
+        self.export_button_widget = QPushButton("Export")
+        self.export_button_widget.clicked.connect(self.export)
+
+        self.layout().addWidget(self.plot_button_widget, 8, 0, 1, 2)
+        self.layout().addWidget(self.export_button_widget, 8, 2, 1, 2)
+
+        self.model.events.adata.connect(self._on_selection)
+
+    def export(self) -> None:
+        """Export shapes."""
+        if (self.matplotlib_widget.selector) is None or (self.matplotlib_widget.selector.exported_data is None):
+            raise ValueError("Data points haven't been selected from the matplotlib visualisation.")
+
+        self.matplotlib_widget.selector.export(self.model.adata)
+
+    def _on_selection(self, event: Optional[Any] = None) -> None:
+        self.x_widget.widget.clear()
+        self.y_widget.widget.clear()
+        self.color_widget.widget.clear()
+
+        self.x_widget.widget._onChange()
+        self.x_widget.component_widget._onChange()
+        self.y_widget.widget._onChange()
+        self.y_widget.component_widget._onChange()
+        self.color_widget.widget._onChange()
+        self.color_widget.component_widget._onChange()
+
+    def _select_layer(self) -> None:
+        """Napari layers."""
+        layer = self._viewer.layers.selection._current
+        if not isinstance(layer.metadata.get("adata", None), AnnData):
+            raise NotImplementedError(":class:`anndata.AnnData` not found in any `layer.metadata`.")
+
+        self.model.layer = layer
+        # if layer is not None and "adata" in layer.metadata:
+        self.model.adata = layer.metadata["adata"]
+
+    @property
+    def viewer(self) -> napari.Viewer:
+        """:mod:`napari` viewer."""
+        return self._viewer
+
+    @property
+    def model(self) -> ImageModel:
+        """:mod:`napari` viewer."""
+        return self._model
+
+    @property
+    def layernames(self) -> FrozenSet[str]:
+        """Names of :class:`napari.layers.Layer`."""
+        return frozenset(layer.name for layer in self.viewer.layers)
+
+
+class QtAdataViewWidget(QWidget):
+    """Adata viewer widget."""
+
+    def __init__(self, viewer: Viewer):
+        super().__init__()
+
+        self._viewer = viewer
+        self._model = ImageModel()
+
+        self._select_layer()
+        self._viewer.layers.selection.events.changed.connect(self._select_layer)
+        self._viewer.layers.selection.events.changed.connect(self._on_layer_update)
 
         self.setLayout(QVBoxLayout())
-        self.layout().addWidget(self._layer_selection_widget.native)
 
         # obs
         obs_label = QLabel("Observations:")
         obs_label.setToolTip("Keys in `adata.obs` containing cell observations.")
         self.obs_widget = AListWidget(self.viewer, self.model, attr="obs")
         self.layout().addWidget(obs_label)
         self.layout().addWidget(self.obs_widget)
@@ -72,15 +168,15 @@
         self.layout().addWidget(var_label)
         self.layout().addWidget(self.var_widget)
 
         # obsm
         obsm_label = QLabel("Obsm:")
         obsm_label.setToolTip("Keys in `adata.obsm` containing multidimensional cell information.")
         self.obsm_widget = AListWidget(self.viewer, self.model, attr="obsm", multiselect=False)
-        self.obsm_index_widget = ObsmIndexWidget(self.model)
+        self.obsm_index_widget = ComponentWidget(self.model, attr="obsm", max_visible=6)
         self.obsm_index_widget.setToolTip("Indices for current key in `adata.obsm`.")
         self.obsm_index_widget.currentTextChanged.connect(self.obsm_widget.setIndex)
         self.obsm_widget.itemClicked.connect(self.obsm_index_widget.addItems)
 
         self.layout().addWidget(obsm_label)
         self.layout().addWidget(self.obsm_widget)
         self.layout().addWidget(self.obsm_index_widget)
@@ -90,15 +186,15 @@
         var_points.setToolTip("Gene names from points.")
         self.var_points_widget = AListWidget(self.viewer, self.model, attr="points")
 
         self.layout().addWidget(var_points)
         self.layout().addWidget(self.var_points_widget)
 
         # scalebar
-        colorbar = CBarWidget()
+        colorbar = CBarWidget(model=self.model)
         self.slider = RangeSliderWidget(self.viewer, self.model, colorbar=colorbar)
         self._viewer.window.add_dock_widget(self.slider, area="left", name="slider")
         self._viewer.window.add_dock_widget(colorbar, area="left", name="colorbar")
         self.viewer.layers.selection.events.active.connect(self.slider._onLayerChange)
 
         self.viewer.bind_key("Shift-E", self.export)
         self.model.events.adata.connect(self._on_layer_update)
@@ -111,63 +207,59 @@
         self.adata_layer_widget.addItem("X", None)
         self.adata_layer_widget.addItems(self._get_adata_layer())
         self.obs_widget._onChange()
         self.var_widget._onChange()
         self.obsm_widget._onChange()
         self.var_points_widget._onChange()
 
-    def _select_layer(self, layer: Layer) -> None:
+    def _select_layer(self) -> None:
         """Napari layers."""
+        layer = self._viewer.layers.selection._current
+        if not isinstance(layer.metadata.get("adata", None), AnnData):
+            raise NotImplementedError(":class:`anndata.AnnData` not found in any `layer.metadata`.")
+
         self.model.layer = layer
         # if layer is not None and "adata" in layer.metadata:
         self.model.adata = layer.metadata["adata"]
-        self.model.library_id = layer.metadata["library_id"]
-        self.model.scale = self.model.adata.uns[Key.uns.spatial][self.model.library_id][Key.uns.scalefactor_key][
-            self.model.scale_key
-        ]
+        try:
+            self.model.scale = self.model.adata.uns[Key.uns.spatial][layer.metadata["library_id"]][
+                Key.uns.scalefactor_key
+            ][self.model.scale_key]
+        except KeyError:  # TODO
+            self.model.scale = 1.0
+        if self.model.adata.shape == (0, 0):
+            return
         self.model.coordinates = np.insert(
             self.model.adata.obsm[Key.obsm.spatial][:, ::-1][:, :2] * self.model.scale, 0, values=0, axis=1
         )
         if "points" in layer.metadata:
             self.model.points_coordinates = layer.metadata["points"].X
             self.model.points_var = layer.metadata["points"].obs["gene"]
             self.model.point_diameter = np.array([0.0] + [layer.metadata["point_diameter"]] * 2) * self.model.scale
-        self.model.spot_diameter = (
-            np.array([0.0] + [Key.uns.spot_diameter(self.model.adata, Key.obsm.spatial, self.model.library_id)] * 2)
-            * self.model.scale
-        )
+        self.model.spot_diameter = np.array([0.0, 10.0, 10.0])
         self.model.labels_key = layer.metadata["labels_key"] if isinstance(layer, Labels) else None
-
-    def _get_layer(self, combo_widget: QComboBox) -> Sequence[Optional[str]]:
-        adata_layers = []
-        for layer in self._viewer.layers:
-            if isinstance(layer.metadata.get("adata", None), AnnData):
-                adata_layers.append(layer)
-        if not len(adata_layers):
-            raise NotImplementedError(
-                "`AnnData` not found in any `layer.metadata`. This plugin requires `AnnData` in at least one layer."
-            )
-        return adata_layers
+        if "colormap" in layer.metadata:
+            self.model.cmap = layer.metadata["colormap"]
 
     def _get_adata_layer(self) -> Sequence[Optional[str]]:
         adata_layers = list(self.model.adata.layers.keys())
         if len(adata_layers):
             return adata_layers
         return [None]
 
     def export(self, _: napari.viewer.Viewer) -> None:
-        """Export shapes into :class:`AnnData` object."""
+        """Export shapes into :class:`anndata.AnnData` object."""
         for layer in self.viewer.layers:
             if not isinstance(layer, napari.layers.Shapes) or layer not in self.viewer.layers.selection:
                 continue
             if not len(layer.data):
                 logger.warn(f"Shape layer `{layer.name}` has no visible shapes.")
                 continue
 
-            key = f"{layer.name}_{self.model.layer.name}"
+            key = f"{layer.name}_{self.model.layer.name}"  # type:ignore[union-attr]
 
             logger.info(f"Adding `adata.obs[{key!r}]`\n       `adata.uns[{key!r}]['mesh']`.")
             self._save_shapes(layer, key=key)
             self._update_obs_items(key)
 
     def _save_shapes(self, layer: napari.layers.Shapes, key: str) -> None:
         shape_list = layer._data_view
@@ -198,9 +290,9 @@
     @property
     def model(self) -> ImageModel:
         """:mod:`napari` viewer."""
         return self._model
 
     @property
     def layernames(self) -> FrozenSet[str]:
-        """Names of :attr:`napari.Viewer.layers`."""
+        """Names of :class:`napari.layers.Layer`."""
         return frozenset(layer.name for layer in self.viewer.layers)
```

### Comparing `napari-spatialdata-0.1.0/src/napari_spatialdata/_widgets.py` & `napari-spatialdata-0.2.1/src/napari_spatialdata/_widgets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import Any, Union, Iterable, Optional, TYPE_CHECKING
 from functools import singledispatchmethod
+from typing import TYPE_CHECKING, Any, Iterable, Optional, Sequence, Union
 
-from qtpy import QtCore, QtWidgets
-from vispy import scene
+import matplotlib.pyplot as plt
+import napari
+import numpy as np
+import pandas as pd
 from loguru import logger
-from superqt import QRangeSlider
-from qtpy.QtCore import Qt, Signal
-from napari.layers import Image, Layer, Labels, Points
+from napari.layers import Image, Labels, Layer, Points
 from napari.viewer import Viewer
-from vispy.scene.widgets import ColorBarWidget
-from vispy.color.colormap import Colormap, MatplotlibColormap
+from qtpy import QtCore, QtWidgets
+from qtpy.QtCore import Qt, Signal
 from sklearn.preprocessing import MinMaxScaler
-import numpy as np
-import napari
-import pandas as pd
-import matplotlib.pyplot as plt
+from superqt import QRangeSlider
+from vispy import scene
+from vispy.color.colormap import Colormap, MatplotlibColormap
+from vispy.scene.widgets import ColorBarWidget
 
 from napari_spatialdata._model import ImageModel
 from napari_spatialdata._utils import (
     NDArrayA,
-    _min_max_norm,
     _get_categorical,
+    _min_max_norm,
     _position_cluster_labels,
+    _set_palette,
 )
 
-__all__ = ["AListWidget", "CBarWidget", "RangeSliderWidget", "ObsmIndexWidget", "CBarWidget"]
+__all__ = [
+    "AListWidget",
+    "CBarWidget",
+    "RangeSliderWidget",
+    "ComponentWidget",
+]
 
 # label string: attribute name
 # TODO(giovp): remove since layer controls private?
 _WIDGETS_TO_HIDE = {
     "symbol:": "symbolComboBox",
     "point size:": "sizeSlider",
     "face color:": "faceColorEdit",
@@ -94,47 +100,46 @@
     layerChanged = Signal()
 
     def __init__(self, viewer: Viewer, model: ImageModel, attr: str, **kwargs: Any):
         if attr not in ImageModel.VALID_ATTRIBUTES:
             raise ValueError(f"Invalid attribute `{attr}`. Valid options are `{sorted(ImageModel.VALID_ATTRIBUTES)}`.")
         super().__init__(viewer, **kwargs)
 
-        self.viewer = viewer
-        self.model = model
+        self._viewer = viewer
+        self._model = model
 
         self._attr = attr
         self._getter = getattr(self.model, f"get_{attr}")
 
         self.layerChanged.connect(self._onChange)
-
         self._onChange()
 
     def _onChange(self) -> None:
         self.clear()
         self.addItems(self.model.get_items(self._attr))
 
     def _onAction(self, items: Iterable[str]) -> None:
         for item in sorted(set(items)):
             try:
                 vec, name = self._getter(item, index=self.getIndex())
-            except Exception as e:  # noqa: B902
+            except Exception as e:  # noqa: BLE001
                 logger.error(e)
                 continue
             if vec.ndim == 2:
                 self.viewer.add_points(
                     vec,
                     name=name,
                     edge_color="white",
                     face_color="white",
                     size=self.model.point_diameter,
                     symbol=self.model.symbol,
                 )
             else:
                 properties = self._get_points_properties(vec, key=item, layer=self.model.layer)
-                if isinstance(self.model.layer, Image):
+                if isinstance(self.model.layer, (Image, Points)):
                     self.viewer.add_points(
                         self.model.coordinates,
                         name=name,
                         size=self.model.spot_diameter,
                         opacity=1,
                         face_colormap=self.model.cmap,
                         edge_colormap=self.model.cmap,
@@ -195,54 +200,67 @@
     def _(self, vec: NDArrayA, **kwargs: Any) -> dict[str, Any]:
         layer = kwargs.pop("layer", None)
         if layer is not None and isinstance(layer, Labels):
             cmap = plt.get_cmap(self.model.cmap)
             norm_vec = _min_max_norm(vec)
             color_vec = cmap(norm_vec)
             return {
-                "color": {k: v for k, v in zip(self.model.adata.obs[self.model.labels_key].values, color_vec)},
+                "color": dict(zip(self.model.adata.obs[self.model.labels_key].values, color_vec)),
                 "properties": {"value": vec},
                 "metadata": {"perc": (0, 100), "data": vec, "minmax": (np.nanmin(vec), np.nanmax(vec))},
             }
         return {
             "text": None,
             "face_color": "value",
             "properties": {"value": vec},
             "metadata": {"perc": (0, 100), "data": vec, "minmax": (np.nanmin(vec), np.nanmax(vec))},
         }
 
     @_get_points_properties.register(pd.Series)
     def _(self, vec: pd.Series, key: str, layer: Layer) -> dict[str, Any]:
-        face_color = _get_categorical(self.model.adata, key=key, palette=self.model.palette, vec=vec)
+        colortypes = _set_palette(self.model.adata, key=key, palette=self.model.palette, vec=vec)
+        face_color = _get_categorical(
+            self.model.adata, key=key, palette=self.model.palette, colordict=colortypes, vec=vec
+        )
         if layer is not None and isinstance(layer, Labels):
-            return {"color": {k: v for k, v in zip(self.model.adata.obs[self.model.labels_key].values, face_color)}}
+            return {"color": dict(zip(self.model.adata.obs[self.model.labels_key].values, face_color))}
 
-        cluster_labels = _position_cluster_labels(self.model.coordinates, vec, face_color)
+        cluster_labels = _position_cluster_labels(self.model.coordinates, vec)
         return {
-            # TODO(giovp): fix color
             "text": {
                 "string": "{clusters}",
                 "size": 24,
-                "color": "white",  # "color": cluster_labels["colors"], {"feature": "clusters", "colormap": "colors"},
+                "color": {"feature": "clusters", "colormap": colortypes},
                 "anchor": "center",
             },
             "face_color": face_color,
             "features": cluster_labels,
             "metadata": None,
         }
 
+    @property
+    def viewer(self) -> napari.Viewer:
+        """:mod:`napari` viewer."""
+        return self._viewer
+
+    @property
+    def model(self) -> ImageModel:
+        """:mod:`napari` viewer."""
+        return self._model
+
 
-class ObsmIndexWidget(QtWidgets.QComboBox):
-    def __init__(self, model: ImageModel, max_visible: int = 6, **kwargs: Any):
+class ComponentWidget(QtWidgets.QComboBox):
+    def __init__(self, model: ImageModel, attr: str, max_visible: int = 4, **kwargs: Any):
         super().__init__(**kwargs)
 
         self._model = model
         self.view().setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAsNeeded)
         self.setMaxVisibleItems(max_visible)
         self.setStyleSheet("combobox-popup: 0;")
+        self._attr = attr
 
     def addItems(self, texts: Union[QtWidgets.QListWidgetItem, int, Iterable[str]]) -> None:
         if isinstance(texts, QtWidgets.QListWidgetItem):
             try:
                 key = texts.text()
                 if isinstance(self._model.adata.obsm[key], pd.DataFrame):
                     texts = sorted(self._model.adata.obsm[key].select_dtypes(include=[np.number, "category"]).columns)
@@ -254,32 +272,79 @@
                 texts = 0
         if isinstance(texts, int):
             texts = tuple(str(i) for i in range(texts))
 
         self.clear()
         super().addItems(tuple(texts))
 
+    def setToolTip(self, click: str) -> None:
+        if click == "obsm":
+            super().setToolTip("Indices for current key in `adata.obsm`. Choose by clicking on item from obsm list.")
+        elif click == "var":
+            super().setToolTip("Keys in `adata.layers`.")
+        else:
+            super().setToolTip("")
+        return
+
+    def setAttribute(self, field: Optional[str]) -> None:
+        if field == self.attr:
+            return
+        self.attr = field
+        self._onChange()
+
+    def _onChange(self) -> None:
+        if self.attr == "var":
+            self.clear()
+            super().addItems(self._getAllLayers())
+        else:
+            self.clear()
+
+    def _onClickChange(self, clicked: Union[QtWidgets.QListWidgetItem, int, Iterable[str]]) -> None:
+        if self.attr == "obsm":
+            self.clear()
+            self.addItems(clicked)
+
+    def _getAllLayers(self) -> Sequence[Optional[str]]:
+        adata_layers = list(self._model.adata.layers.keys())
+        if len(adata_layers):
+            adata_layers.insert(0, "X")
+            return adata_layers
+        return ["X"]
+
+    @property
+    def attr(self) -> Optional[str]:
+        if TYPE_CHECKING:
+            assert isinstance(self._attr, str)
+        return self._attr
+
+    @attr.setter
+    def attr(self, field: Optional[str]) -> None:
+        if field not in ("var", "obs", "obsm"):
+            raise ValueError(f"{field} is not a valid adata field.")
+        self._attr = field
+
 
 class CBarWidget(QtWidgets.QWidget):
     FORMAT = "{0:0.2f}"
 
     cmapChanged = Signal(str)
     climChanged = Signal((float, float))
 
     def __init__(
         self,
+        model: ImageModel,
         cmap: str = "viridis",
         label: Optional[str] = None,
         width: Optional[int] = 250,
         height: Optional[int] = 50,
         **kwargs: Any,
     ):
         super().__init__(**kwargs)
 
-        self._cmap = cmap
+        self._model = model
 
         self._clim = (0.0, 1.0)
         self._oclim = self._clim
 
         self._width = width
         self._height = height
         self._label = label
@@ -323,15 +388,15 @@
         assert 0 <= maxx <= 1, f"Expected `maxx` to be in `[0, 1]`, found `{maxx}`"
 
         cm = MatplotlibColormap(cmap)
 
         return Colormap(cm[np.linspace(minn, maxx, len(cm.colors))], interpolation="linear")
 
     def getCmap(self) -> str:
-        return self._cmap
+        return self.cmap
 
     def onCmapChanged(self, value: str) -> None:
         # this does not trigger update for some reason...
         self._colorbar.cmap = self._create_colormap(value)
         self._colorbar._colorbar._update()
 
     def setClim(self, value: tuple[float, float]) -> None:
@@ -371,23 +436,23 @@
         # could also trigger it as self._colorbar.clim = self.getClim()
         # but the above option also updates geometry
         # cbarwidget->cbar->cbarvisual
         self._colorbar._colorbar._colorbar._update()
 
     @property
     def cmap(self) -> str:
-        return self._cmap
+        return self._model.cmap
 
 
 class RangeSliderWidget(QRangeSlider):
     def __init__(self, viewer: Viewer, model: ImageModel, colorbar: CBarWidget, **kwargs: Any):
         super().__init__(**kwargs)
 
-        self.viewer = viewer
-        self.model = model
+        self._viewer = viewer
+        self._model = model
         self._colorbar = colorbar
         self._cmap = plt.get_cmap(self._colorbar.cmap)
         self.setValue((0, 100))
         self.setSliderPosition((0, 100))
         self.setSingleStep(0.01)
         self.setOrientation(Qt.Horizontal)
         self.valueChanged.connect(self._onValueChange)
@@ -397,27 +462,27 @@
         if layer is not None:
             self._onValueChange((0, 100))
 
     def _onValueChange(self, percentile: tuple[float, float]) -> None:
         layer = self.viewer.layers.selection.active
         # TODO(michalk8): use constants
         if "data" not in layer.metadata:
-            return None
+            return None  # noqa: RET501
         v = layer.metadata["data"]
-        clipped = np.clip(v, *np.percentile(v, percentile))  # type: ignore[misc]
+        clipped = np.clip(v, *np.percentile(v, percentile))
 
         if isinstance(layer, Points):
             layer.metadata = {**layer.metadata, "perc": percentile}
             layer.face_color = "value"
             layer.properties = {"value": clipped}
             layer.refresh_colors()
         elif isinstance(layer, Labels):
             norm_vec = self._scale_vec(clipped)
             color_vec = self._cmap(norm_vec)
-            layer.color = {k: v for k, v in zip(layer.color.keys(), color_vec)}
+            layer.color = dict(zip(layer.color.keys(), color_vec))
             layer.properties = {"value": clipped}
             layer.refresh()
 
         self._colorbar.setOclim(layer.metadata["minmax"])
         self._colorbar.setClim((np.min(layer.properties["value"]), np.max(layer.properties["value"])))
         self._colorbar.update_color()
 
@@ -425,8 +490,18 @@
         ominn, omaxx = self._colorbar.getOclim()
         delta = omaxx - ominn + 1e-12
 
         minn, maxx = self._colorbar.getClim()
         minn = (minn - ominn) / delta
         maxx = (maxx - ominn) / delta
         scaler = MinMaxScaler(feature_range=(minn, maxx))
-        return scaler.fit_transform(vec.reshape(-1, 1))
+        return scaler.fit_transform(vec.reshape(-1, 1))  # type: ignore[no-any-return]
+
+    @property
+    def viewer(self) -> napari.Viewer:
+        """:mod:`napari` viewer."""
+        return self._viewer
+
+    @property
+    def model(self) -> ImageModel:
+        """:mod:`napari` viewer."""
+        return self._model
```

### Comparing `napari-spatialdata-0.1.0/src/napari_spatialdata.egg-info/PKG-INFO` & `napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.1.0
+Version: 0.2.1
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
@@ -12,22 +12,22 @@
 Project-URL: User Support, https://github.com/scverse/napari-spatialdata/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: testing
+Provides-Extra: test
+Provides-Extra: doc
 License-File: LICENSE
 
 # napari-spatialdata
 
 [![License](https://img.shields.io/pypi/l/napari-spatialdata.svg?color=green)](https://github.com/scverse/napari-spatialdata/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-spatialdata.svg?color=green)](https://pypi.org/project/napari-spatialdata)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-spatialdata.svg?color=green)](https://python.org)
@@ -46,50 +46,53 @@
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/plugins/stable/index.html
 -->
 
-# UNDER DEVELOPMENT
+## Installation
 
-Clone repo and `pip install -e .`.
-Run examples e.g. `python shape_regions.py` or via notebook for the shape export function.
+You can install `napari-spatialdata` via [pip]:
 
-More documentation on usage will be added later on.
+    pip install napari-spatialdata
 
-Expect breaking changes.
+## Development Version
 
-## Installation
+You can install `napari-spatialdata` from Github with:
 
-You can install `napari-spatialdata` via [pip]:
+    pip install git+https://github.com/scverse/napari-spatialdata
 
-    pip install napari-spatialdata
+Or, you can also install in editable mode after cloning the repo by:
+
+    git clone https://github.com/scverse/napari-spatialdata
+    cd napari-spatialdata
+    pip install -e .
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-spatialdata" is free and open source software
 
 ## Issues
 
-If you encounter any problems, please [file an issue] along with a detailed description.
+If you encounter any problems, please file an [issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [mit]: http://opensource.org/licenses/MIT
 [bsd-3]: http://opensource.org/licenses/BSD-3-Clause
 [gnu gpl v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
 [gnu lgpl v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
 [apache software license 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [mozilla public license 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-[napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [pypi]: https://pypi.org/
+[issue]: https://github.com/scverse/napari-spatialdata/issues
```

### Comparing `napari-spatialdata-0.1.0/tests/conftest.py` & `napari-spatialdata-0.2.1/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from abc import ABC, ABCMeta
-from typing import Any, Dict, Tuple, Callable, Optional
-from pathlib import Path
 from functools import wraps
+from pathlib import Path
+from typing import Any, Callable, Dict, Optional, Tuple
 
-from scipy import ndimage as ndi
-from loguru import logger
-from anndata import AnnData
-from skimage import data
-from matplotlib.testing.compare import compare_images
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
-import matplotlib.pyplot as plt
-
+from anndata import AnnData
+from loguru import logger
+from matplotlib.testing.compare import compare_images
 from napari_spatialdata._utils import NDArrayA
+from scipy import ndimage as ndi
+from skimage import data
 
 HERE: Path = Path(__file__).parent
 
 SEED = 42
 
 EXPECTED = HERE / "_images"
 ACTUAL = HERE / "figures"
 TOL = 50
 DPI = 40
 
 
 @pytest.fixture
 def adata_labels() -> AnnData:
-
     n_var = 50
 
     blobs, _ = _get_blobs_galaxy()
     seg = np.unique(blobs)[1:]
     n_obs_labels = len(seg)
     rng = np.random.default_rng(SEED)
 
@@ -51,21 +49,19 @@
                     "tissue_hires_scalef": 1,
                     "tissue_segmentation_scalef": 1,
                 }
             }
         }
     }
     obsm_labels = {"spatial": rng.integers(0, blobs.shape[0], size=(n_obs_labels, 2))}
-    adata_labels = generate_adata(n_var, obs_labels, obsm_labels, uns_labels)
-    return adata_labels
+    return generate_adata(n_var, obs_labels, obsm_labels, uns_labels)
 
 
 @pytest.fixture
 def adata_shapes() -> AnnData:
-
     n_obs_shapes = 100
     n_var = 50
     blobs, _ = _get_blobs_galaxy()
 
     rng = np.random.default_rng(SEED)
     obs_shapes = pd.DataFrame(
         {
@@ -82,24 +78,22 @@
                     "tissue_hires_scalef": 1,
                     "tissue_segmentation_scalef": 1,
                 }
             }
         }
     }
     obsm_shapes = {"spatial": rng.integers(0, blobs.shape[0], size=(n_obs_shapes, 2))}
-    adata_shapes = AnnData(
+    return AnnData(
         rng.normal(size=(n_obs_shapes, n_var)),
         dtype=np.float64,
         obs=obs_shapes,
         obsm=obsm_shapes,
         uns=uns_shapes,
     )
 
-    return adata_shapes
-
 
 @pytest.fixture
 def image():
     _, image = _get_blobs_galaxy()
     return image
 
 
@@ -113,22 +107,21 @@
     blobs = data.binary_blobs(seed=SEED)
     blobs = ndi.label(blobs)[0]
     return blobs, data.hubble_deep_field()[: blobs.shape[0], : blobs.shape[0]]
 
 
 def generate_adata(n_var: int, obs: pd.DataFrame, obsm: Dict[Any, Any], uns: Dict[Any, Any]) -> AnnData:
     rng = np.random.default_rng(SEED)
-    adata = AnnData(
+    return AnnData(
         rng.normal(size=(obs.shape[0], n_var)),
         obs=obs,
         obsm=obsm,
         uns=uns,
         dtype=np.float64,
     )
-    return adata
 
 
 class PlotTesterMeta(ABCMeta):
     def __new__(cls, clsname, superclasses, attributedict):
         for key, value in attributedict.items():
             if callable(value):
                 attributedict[key] = _decorate(value, clsname, name=key)
```

### Comparing `napari-spatialdata-0.1.0/tests/test_utils.py` & `napari-spatialdata-0.2.1/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,58 @@
-from typing import List
 import logging
+from typing import Any, List
 
-from anndata import AnnData
 import numpy as np
-import pandas as pd
 import pytest
-
+from anndata import AnnData
 from napari_spatialdata._utils import (
-    _min_max_norm,
     _get_categorical,
+    _get_transform,
+    _min_max_norm,
     _points_inside_triangles,
     _position_cluster_labels,
+    _set_palette,
 )
+from spatialdata.datasets import blobs
 
 
 def test_get_categorical(adata_labels: AnnData):
-
     assert _get_categorical(adata_labels, key="categorical").shape == (adata_labels.n_obs, 3)
 
 
+def test_set_palette(adata_labels: AnnData):
+    assert np.array_equal(
+        _get_categorical(adata_labels, key="categorical"),
+        _get_categorical(adata_labels, key="categorical", colordict=_set_palette(adata_labels, key="categorical")),
+    )
+
+
+def test_value_error(adata_labels: AnnData):
+    col_dict = _set_palette(adata_labels, key="categorical")
+    col_dict[1] = "non_existing_color"
+    with pytest.raises(ValueError) as err:
+        _get_categorical(adata_labels, key="categorical", colordict=col_dict)
+    assert "`non_existing_color` is not an acceptable color." in str(err.value)
+    col_dict[27] = col_dict.pop(1)
+    with pytest.raises(ValueError) as err:
+        _get_categorical(adata_labels, key="categorical", colordict=col_dict)
+    assert "The key `27` in the given dictionary is not an existing category in anndata[`categorical`]." in str(
+        err.value
+    )
+
+
 def test_position_cluster_labels(adata_labels: AnnData):
     from napari_spatialdata._model import ImageModel
 
     model = ImageModel()
     model.coordinates = np.insert(adata_labels.obsm["spatial"], 0, values=0, axis=1).copy()
     clusters = adata_labels.obs["categorical"]
-    colors = _get_categorical(adata_labels, key="categorical")
-
-    positions = _position_cluster_labels(model.coordinates, clusters, colors)
 
+    positions = _position_cluster_labels(model.coordinates, clusters)
     assert isinstance(positions["clusters"], np.ndarray)
-    assert isinstance(positions["colors"], np.ndarray)
-    assert positions["clusters"].shape == positions["colors"].shape
     assert np.unique(positions["clusters"].nonzero()).shape == adata_labels.obs["categorical"].cat.categories.shape
 
 
 @pytest.mark.parametrize("tri_coord", [[[0, 10, 20], [30, 40, 50]]])
 def test_points_inside_triangles(adata_shapes: AnnData, tri_coord: List[List[int]]):
     from napari_spatialdata._model import ImageModel
 
@@ -55,22 +72,30 @@
 
     assert out.shape[0] == model.coordinates.shape[0]
     assert out.any()
 
 
 @pytest.mark.parametrize("vec", [np.array([0, 0, 2]), np.array([1, 1, 0])])
 def test_min_max_norm(vec: np.ndarray) -> None:
-
     out = _min_max_norm(vec)
 
     assert out.shape == vec.shape
     assert (out.min(), out.max()) == (0, 1)
 
 
-def test_logger(caplog, adata_labels: AnnData):
+def test_logger(caplog, adata_labels: AnnData, make_napari_viewer: Any):
+    from napari_spatialdata._model import ImageModel
+    from napari_spatialdata._scatterwidgets import MatplotlibWidget
 
-    vec = pd.Series(["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"], dtype="category")
+    viewer = make_napari_viewer()
+    model = ImageModel()
 
-    _get_categorical(adata_labels, key="categorical", vec=vec)
+    m = MatplotlibWidget(viewer, model)
+    m._onClick(np.ones(10), np.ones(10), np.ones(10), "X", "Y", "Color")
 
     with caplog.at_level(logging.INFO):
-        assert "Overwriting `adata.obs" in caplog.records[0].message
+        assert "Plotting" in caplog.records[0].message
+
+
+def test_get_transform():
+    sdata = blobs()
+    assert (_get_transform(sdata.images["blobs_image"]) == np.identity(3)).all()
```

