# Comparing `tmp/napari-spatialdata-0.2.1.tar.gz` & `tmp/napari-spatialdata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-spatialdata-0.2.1.tar", last modified: Thu May  4 11:08:23 2023, max compression
+gzip compressed data, was "napari-spatialdata-0.2.2.tar", last modified: Thu May  4 14:27:21 2023, max compression
```

## Comparing `napari-spatialdata-0.2.1.tar` & `napari-spatialdata-0.2.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.909586 napari-spatialdata-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/_templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/extensions/typed_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.913586 napari-spatialdata-0.2.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)  5521635 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/notebooks/spatialdata.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/docs/template_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.921587 napari-spatialdata-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/raster_points_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/raster_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/shape_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/examples/spatialdata_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.909586 napari-spatialdata-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/src/napari_spatialdata/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_categoricals_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_pkg_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/src/napari_spatialdata/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 11:08:23.000000 napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:23.925587 napari-spatialdata-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/test_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/test_spatialdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-04 11:08:03.000000 napari-spatialdata-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.263920 napari-spatialdata-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.267920 napari-spatialdata-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.267920 napari-spatialdata-0.2.2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.267920 napari-spatialdata-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.271920 napari-spatialdata-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.271920 napari-spatialdata-0.2.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/_templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.271920 napari-spatialdata-0.2.2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.271920 napari-spatialdata-0.2.2/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/extensions/typed_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.275920 napari-spatialdata-0.2.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2807648 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/notebooks/mibitof_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3449197 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/notebooks/nanostring_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  5522494 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/notebooks/spatialdata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/docs/template_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.283920 napari-spatialdata-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/examples/spatialdata_mibitof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/examples/spatialdata_nanostring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.267920 napari-spatialdata-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/src/napari_spatialdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_categoricals_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_pkg_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/src/napari_spatialdata/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 14:27:21.000000 napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:21.287921 napari-spatialdata-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/test_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/test_spatialdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-04 14:27:04.000000 napari-spatialdata-0.2.2/tox.ini
```

### Comparing `napari-spatialdata-0.2.1/.github/workflows/test_and_deploy.yml` & `napari-spatialdata-0.2.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/.gitignore` & `napari-spatialdata-0.2.2/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -98,7 +98,10 @@
 
 # files
 *.h5ad
 
 # docs
 /docs/generated/
 /docs/_build/
+
+# Tutorial data
+docs/notebooks/tutorial_data/
```

### Comparing `napari-spatialdata-0.2.1/.mypy.ini` & `napari-spatialdata-0.2.2/.mypy.ini`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/.napari/DESCRIPTION.md` & `napari-spatialdata-0.2.2/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/.pre-commit-config.yaml` & `napari-spatialdata-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/LICENSE` & `napari-spatialdata-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/PKG-INFO` & `napari-spatialdata-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.1
+Version: 0.2.2
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
```

### Comparing `napari-spatialdata-0.2.1/README.md` & `napari-spatialdata-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/docs/Makefile` & `napari-spatialdata-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/docs/_templates/autosummary/class.rst` & `napari-spatialdata-0.2.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/docs/conf.py` & `napari-spatialdata-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/docs/contributing.md` & `napari-spatialdata-0.2.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/docs/extensions/typed_returns.py` & `napari-spatialdata-0.2.2/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/docs/make.bat` & `napari-spatialdata-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/docs/notebooks/spatialdata.ipynb` & `napari-spatialdata-0.2.2/docs/notebooks/spatialdata.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961495535714285%*

 * *Differences: {"'cells'": "{3: {delete: ['attachments']}, 6: {delete: ['attachments']}, 7: {'execution_count': "*

 * *            "16, 'outputs': {0: {'text': {insert: [(0, "*

 * *            '"/Users/rahulbshrestha/projects/napari-spatialdata/src/napari_spatialdata/_view.py:216: '*

 * *            "FutureWarning: Private attribute access ('Selection._current') in this context (e.g. "*

 * *            'inside a plugin widget or dock widget) is deprecated and will be unavailable in '*

 * *            'version 0.5.0\\n"), (1, \'  layer = self._vie […]*

```diff
@@ -18,15 +18,14 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Import packages and data"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "There are two options to install napari-spatialdata:\n",
                 "\n",
                 "(1) Run `pip install napari-spatialdata`\n",
                 "\n",
@@ -76,42 +75,46 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Visualise in napari"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can instantiate the `Interactive` class with our {class}`spatialdata.SpatialData` object, and view it in Napari."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
+                        "/Users/rahulbshrestha/projects/napari-spatialdata/src/napari_spatialdata/_view.py:216: FutureWarning: Private attribute access ('Selection._current') in this context (e.g. inside a plugin widget or dock widget) is deprecated and will be unavailable in version 0.5.0\n",
+                        "  layer = self._viewer.layers.selection._current\n",
                         "/Users/rahulbshrestha/projects/napari-spatialdata/src/napari_spatialdata/_view.py:107: FutureWarning: Private attribute access ('Selection._current') in this context (e.g. inside a plugin widget or dock widget) is deprecated and will be unavailable in version 0.5.0\n",
-                        "  layer = self._viewer.layers.selection._current\n"
+                        "  layer = self._viewer.layers.selection._current\n",
+                        "2023-05-02 21:54:40.663 | INFO     | napari_spatialdata._categoricals_utils:_set_default_colors_for_categorical_obs:363 - the obs value 'Width' has more than 103 categories. Uniform 'grey' color will be used for all categories.\n",
+                        "2023-05-02 22:02:12.881 | INFO     | napari_spatialdata._scatterwidgets:plot:253 - Plotting coordinates.\n",
+                        "2023-05-02 22:02:20.842 | INFO     | napari_spatialdata._scatterwidgets:plot:253 - Plotting coordinates.\n",
+                        "2023-05-02 22:02:23.160 | INFO     | napari_spatialdata._scatterwidgets:plot:253 - Plotting coordinates.\n"
                     ]
                 }
             ],
             "source": [
                 "interactive = Interactive(sdata)\n",
                 "interactive.run()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This executes an empty Napari viewer. The SpatialData widget is in the bottom left hand corner and consists of two boxes, \"Coordinate System\" and \"Elements\". \n",
                 "\n",
                 "A {class}`spatialdata.SpatialData` object groups together five {obj}`spatialdata.models.SpatialElement`: Images (raster images), Labels (e.g. segmentation masks), Points (e.g. transcripts locations, molecular probes), Shapes (regions of interests, array capture locations etc.), and Table (where the molecular profiles and annotations are stored). Each SpatialElement can be associated with a coordinate system and the transformation required to align that element to it."
             ]
```

### Comparing `napari-spatialdata-0.2.1/docs/references.bib` & `napari-spatialdata-0.2.2/docs/references.bib`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/docs/template_usage.md` & `napari-spatialdata-0.2.2/docs/template_usage.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/pyproject.toml` & `napari-spatialdata-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/setup.cfg` & `napari-spatialdata-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/__init__.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/_categoricals_utils.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/_categoricals_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_pkg_constants.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_pkg_constants.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/_constants/_utils.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/_constants/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/_interactive.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/_interactive.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/_model.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/_model.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/_scatterwidgets.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/_scatterwidgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/_utils.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/_view.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,25 +216,19 @@
         layer = self._viewer.layers.selection._current
         if not isinstance(layer.metadata.get("adata", None), AnnData):
             raise NotImplementedError(":class:`anndata.AnnData` not found in any `layer.metadata`.")
 
         self.model.layer = layer
         # if layer is not None and "adata" in layer.metadata:
         self.model.adata = layer.metadata["adata"]
-        try:
-            self.model.scale = self.model.adata.uns[Key.uns.spatial][layer.metadata["library_id"]][
-                Key.uns.scalefactor_key
-            ][self.model.scale_key]
-        except KeyError:  # TODO
-            self.model.scale = 1.0
+
         if self.model.adata.shape == (0, 0):
             return
-        self.model.coordinates = np.insert(
-            self.model.adata.obsm[Key.obsm.spatial][:, ::-1][:, :2] * self.model.scale, 0, values=0, axis=1
-        )
+
+        self.model.coordinates = np.insert(self.model.adata.obsm[Key.obsm.spatial][:, ::-1][:, :2], 0, values=0, axis=1)
         if "points" in layer.metadata:
             self.model.points_coordinates = layer.metadata["points"].X
             self.model.points_var = layer.metadata["points"].obs["gene"]
             self.model.point_diameter = np.array([0.0] + [layer.metadata["point_diameter"]] * 2) * self.model.scale
         self.model.spot_diameter = np.array([0.0, 10.0, 10.0])
         self.model.labels_key = layer.metadata["labels_key"] if isinstance(layer, Labels) else None
         if "colormap" in layer.metadata:
```

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/_widgets.py` & `napari-spatialdata-0.2.2/src/napari_spatialdata/_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata/napari.yaml` & `napari-spatialdata-0.2.2/src/napari_spatialdata/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/PKG-INFO` & `napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.1
+Version: 0.2.2
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
```

### Comparing `napari-spatialdata-0.2.1/src/napari_spatialdata.egg-info/SOURCES.txt` & `napari-spatialdata-0.2.2/src/napari_spatialdata.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 docs/references.bib
 docs/references.md
 docs/template_usage.md
 docs/_static/.gitkeep
 docs/_templates/.gitkeep
 docs/_templates/autosummary/class.rst
 docs/extensions/typed_returns.py
+docs/notebooks/mibitof_analysis.ipynb
+docs/notebooks/nanostring_analysis.ipynb
 docs/notebooks/spatialdata.ipynb
 examples/README.md
-examples/raster_points_regions.py
-examples/raster_regions.py
-examples/shape_regions.py
-examples/spatialdata_interactive.py
+examples/spatialdata_mibitof.py
+examples/spatialdata_nanostring.py
 src/napari_spatialdata/__init__.py
 src/napari_spatialdata/_categoricals_utils.py
 src/napari_spatialdata/_interactive.py
 src/napari_spatialdata/_model.py
 src/napari_spatialdata/_scatterwidgets.py
 src/napari_spatialdata/_utils.py
 src/napari_spatialdata/_version.py
```

### Comparing `napari-spatialdata-0.2.1/tests/conftest.py` & `napari-spatialdata-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/tests/test_interactive.py` & `napari-spatialdata-0.2.2/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/tests/test_scatterwidgets.py` & `napari-spatialdata-0.2.2/tests/test_scatterwidgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/tests/test_spatialdata.py` & `napari-spatialdata-0.2.2/tests/test_spatialdata.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/tests/test_utils.py` & `napari-spatialdata-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.1/tox.ini` & `napari-spatialdata-0.2.2/tox.ini`

 * *Files identical despite different names*

