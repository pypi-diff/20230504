# Comparing `tmp/cacholote-0.3.0.tar.gz` & `tmp/cacholote-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacholote-0.3.0.tar", last modified: Fri Apr 14 07:36:44 2023, max compression
+gzip compressed data, was "cacholote-0.3.1.tar", last modified: Thu May  4 15:02:22 2023, max compression
```

## Comparing `cacholote-0.3.0.tar` & `cacholote-0.3.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.774470 cacholote-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 07:36:30.000000 cacholote-0.3.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.766470 cacholote-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-14 07:36:30.000000 cacholote-0.3.0/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-14 07:36:30.000000 cacholote-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 07:36:30.000000 cacholote-0.3.0/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-14 07:36:30.000000 cacholote-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-14 07:36:30.000000 cacholote-0.3.0/DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 07:36:30.000000 cacholote-0.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-14 07:36:30.000000 cacholote-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 07:36:30.000000 cacholote-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-14 07:36:30.000000 cacholote-0.3.0/OBJECT-STORAGE-DESIGN.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-04-14 07:36:44.774470 cacholote-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-14 07:36:30.000000 cacholote-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/cacholote/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/extra_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-14 07:36:30.000000 cacholote-0.3.0/cacholote/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/cacholote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 07:36:44.000000 cacholote-0.3.0/cacholote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-14 07:36:30.000000 cacholote-0.3.0/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-14 07:36:30.000000 cacholote-0.3.0/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 07:36:30.000000 cacholote-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-14 07:36:30.000000 cacholote-0.3.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-14 07:36:30.000000 cacholote-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 07:36:44.774470 cacholote-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:44.770470 cacholote-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_01_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_10_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_20_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_30_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_40_xarray_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_50_io_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-14 07:36:30.000000 cacholote-0.3.0/tests/test_60_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 15:02:04.000000 cacholote-0.3.1/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.358105 cacholote-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.362105 cacholote-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-05-04 15:02:04.000000 cacholote-0.3.1/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-04 15:02:04.000000 cacholote-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-04 15:02:04.000000 cacholote-0.3.1/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-04 15:02:04.000000 cacholote-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 15:02:04.000000 cacholote-0.3.1/DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 15:02:04.000000 cacholote-0.3.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-05-04 15:02:04.000000 cacholote-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 15:02:04.000000 cacholote-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-04 15:02:04.000000 cacholote-0.3.1/OBJECT-STORAGE-DESIGN.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-05-04 15:02:22.366105 cacholote-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-04 15:02:04.000000 cacholote-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.362105 cacholote-0.3.1/cacholote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/extra_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-04 15:02:04.000000 cacholote-0.3.1/cacholote/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.362105 cacholote-0.3.1/cacholote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 15:02:22.000000 cacholote-0.3.1/cacholote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.362105 cacholote-0.3.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-04 15:02:04.000000 cacholote-0.3.1/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-04 15:02:04.000000 cacholote-0.3.1/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-04 15:02:04.000000 cacholote-0.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 15:02:04.000000 cacholote-0.3.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-04 15:02:04.000000 cacholote-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:02:22.366105 cacholote-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:02:22.366105 cacholote-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_01_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_10_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_20_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_30_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_40_xarray_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_50_io_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-04 15:02:04.000000 cacholote-0.3.1/tests/test_60_clean.py
```

### Comparing `cacholote-0.3.0/.cruft.json` & `cacholote-0.3.1/.cruft.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'abe10924d34c36556d1767e1833b88ea93df0e13'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "23164e60b3e44472716d3d46bcd3ef47bbf2e79a",
+    "commit": "abe10924d34c36556d1767e1833b88ea93df0e13",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/ecmwf-projects/cookiecutter-conda-package",
             "copyright_holder": "B-Open Solutions srl",
             "copyright_year": "2019",
             "integration_tests": "True",
             "mypy_strict": "True",
```

### Comparing `cacholote-0.3.0/.github/workflows/on-push.yml` & `cacholote-0.3.1/.github/workflows/on-push.yml`

 * *Files 1% similar despite different names*

```diff
@@ -133,19 +133,19 @@
     needs: [combine-environments, unit-tests]
     if: |
       success() && true
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
+        python-version: [3.8, 3.11]
+        extra: [-ci]
         include:
         - python-version: '3.10'
           extra: -integration
-        - python-version: '3.8'
-          extra: -ci
 
     steps:
     - uses: actions/checkout@v3
     - name: Download combined environments
       uses: actions/download-artifact@v3
       with:
         name: combined-environments
```

### Comparing `cacholote-0.3.0/.gitignore` & `cacholote-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/.pre-commit-config.yaml` & `cacholote-0.3.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   - id: black
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.8
   hooks:
   - id: blackdoc
     additional_dependencies: [black==22.3.0]
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.260
+  rev: v0.0.263
   hooks:
   - id: ruff
     args: [--fix]
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.16
   hooks:
   - id: mdformat
```

### Comparing `cacholote-0.3.0/DESIGN.rst` & `cacholote-0.3.1/DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/LICENSE` & `cacholote-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/Makefile` & `cacholote-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/OBJECT-STORAGE-DESIGN.rst` & `cacholote-0.3.1/OBJECT-STORAGE-DESIGN.rst`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/PKG-INFO` & `cacholote-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.3.0
+Version: 0.3.1
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.3.0/README.md` & `cacholote-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/cacholote/__init__.py` & `cacholote-0.3.1/cacholote/__init__.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/cacholote/cache.py` & `cacholote-0.3.1/cacholote/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 
 import datetime
 import functools
 import json
 import warnings
 from typing import Any, Callable, TypeVar, cast
 
-import sqlalchemy
+import sqlalchemy as sa
 import sqlalchemy.orm
 
 from . import clean, config, database, decode, encode
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 
 def _decode_and_update(
-    session: sqlalchemy.orm.Session,
+    session: sa.orm.Session,
     cache_entry: Any,
     settings: config.Settings,
 ) -> Any:
     result = decode.loads(cache_entry._result_as_string)
     cache_entry.counter = (cache_entry.counter or 0) + 1
     if settings.tag is not None:
         cache_entry.tag = settings.tag
@@ -68,16 +68,16 @@
             database.CacheEntry.expiration > datetime.datetime.utcnow(),
         ]
         if settings.expiration:
             # When expiration is provided, only get entries with matching expiration
             filters.append(database.CacheEntry.expiration == settings.expiration)
 
         with settings.sessionmaker() as session:
-            for cache_entry in (
-                session.query(database.CacheEntry)
+            for cache_entry in session.scalars(
+                sa.select(database.CacheEntry)
                 .filter(*filters)
                 .order_by(database.CacheEntry.timestamp.desc())
             ):
                 try:
                     return _decode_and_update(session, cache_entry, settings)
                 except decode.DecodeError as ex:
                     warnings.warn(str(ex), UserWarning)
```

### Comparing `cacholote-0.3.0/cacholote/clean.py` & `cacholote-0.3.1/cacholote/clean.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 # limitations under the License.
 
 import collections
 import datetime
 import functools
 import json
 import posixpath
-from typing import Any, Callable, Dict, Literal, Optional, Sequence, Set, Union
+from typing import Any, Callable, Dict, List, Literal, Optional, Sequence, Set, Union
 
-import sqlalchemy
+import sqlalchemy as sa
 import sqlalchemy.orm
 import structlog
 
 from . import config, database, encode, extra_encoders, utils
 
 LOGGER = structlog.get_logger()
 
 
 def _delete_cache_file(
     obj: Dict[str, Any],
-    session: Optional[sqlalchemy.orm.Session] = None,
+    session: Optional[sa.orm.Session] = None,
     cache_entry: Optional[database.CacheEntry] = None,
     sizes: Optional[Dict[str, int]] = None,
     dry_run: bool = False,
     logger: Optional[structlog.stdlib.BoundLogger] = None,
 ) -> Any:
     logger = logger or LOGGER
 
@@ -66,15 +66,15 @@
                             recursive=obj["args"][0]["type"] == "application/vnd+zarr",
                         )
 
     return obj
 
 
 def _delete_cache_entry(
-    session: sqlalchemy.orm.Session, cache_entry: database.CacheEntry
+    session: sa.orm.Session, cache_entry: database.CacheEntry
 ) -> None:
     # First, delete database entry
     session.delete(cache_entry)
     database._commit_or_rollback(session)
     # Then, delete files
     json.loads(cache_entry._result_as_string, object_hook=_delete_cache_file)
 
@@ -91,16 +91,16 @@
     *args: Any
         Argument of functions to delete from cache
     **kwargs: Any
         Keyword arguments of functions to delete from cache
     """
     hexdigest = encode._hexdigestify_python_call(func_to_del, *args, **kwargs)
     with config.get().sessionmaker() as session:
-        for cache_entry in session.query(database.CacheEntry).filter(
-            database.CacheEntry.key == hexdigest
+        for cache_entry in session.scalars(
+            sa.select(database.CacheEntry).filter(database.CacheEntry.key == hexdigest)
         ):
             _delete_cache_entry(session, cache_entry)
 
 
 class _Cleaner:
     def __init__(self, logger: structlog.stdlib.BoundLogger) -> None:
         fs, dirname = utils.get_cache_files_fs_dirname()
@@ -141,15 +141,15 @@
                 ):
                     files_to_skip.append(urlpath)
                     files_to_skip.append(urlpath.rsplit(".lock", 1)[0])
 
         unknown_sizes = {k: v for k, v in self.sizes.items() if k not in files_to_skip}
         if unknown_sizes:
             with config.get().sessionmaker() as session:
-                for cache_entry in session.query(database.CacheEntry):
+                for cache_entry in session.scalars(sa.select(database.CacheEntry)):
                     json.loads(
                         cache_entry._result_as_string,
                         object_hook=functools.partial(
                             _delete_cache_file,
                             sizes=unknown_sizes,
                             dry_run=True,
                             logger=self.logger,
@@ -191,46 +191,47 @@
     ) -> None:
         self.check_tags(tags_to_clean, tags_to_keep)
 
         # Filters
         filters = []
         if tags_to_keep is not None:
             filters.append(
-                sqlalchemy.or_(
+                sa.or_(
                     database.CacheEntry.tag.not_in(tags_to_keep),
                     database.CacheEntry.tag.is_not(None)
                     if None in tags_to_keep
                     else database.CacheEntry.tag.is_(None),
                 )
             )
         elif tags_to_clean is not None:
             filters.append(
-                sqlalchemy.or_(
+                sa.or_(
                     database.CacheEntry.tag.in_(tags_to_clean),
                     database.CacheEntry.tag.is_(None)
                     if None in tags_to_clean
                     else database.CacheEntry.tag.is_not(None),
                 )
             )
 
         # Sorters
+        sorters: List[sa.orm.InstrumentedAttribute[Any]] = []
         if method == "LRU":
-            sorters = [database.CacheEntry.timestamp, database.CacheEntry.counter]
+            sorters.extend([database.CacheEntry.timestamp, database.CacheEntry.counter])
         elif method == "LFU":
-            sorters = [database.CacheEntry.counter, database.CacheEntry.timestamp]
+            sorters.extend([database.CacheEntry.counter, database.CacheEntry.timestamp])
         else:
             raise ValueError("`method` must be 'LRU' or 'LFU'.")
         sorters.append(database.CacheEntry.expiration)
 
         # Clean database files
         if self.stop_cleaning(maxsize):
             return
         with config.get().sessionmaker() as session:
-            for cache_entry in (
-                session.query(database.CacheEntry).filter(*filters).order_by(*sorters)
+            for cache_entry in session.scalars(
+                sa.select(database.CacheEntry).filter(*filters).order_by(*sorters)
             ):
                 json.loads(
                     cache_entry._result_as_string,
                     object_hook=functools.partial(
                         _delete_cache_file,
                         session=session,
                         cache_entry=cache_entry,
```

### Comparing `cacholote-0.3.0/cacholote/config.py` & `cacholote-0.3.1/cacholote/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 import pathlib
 import tempfile
 from types import TracebackType
 from typing import Any, Dict, Literal, Optional, Tuple, Type, Union
 
 import fsspec
 import pydantic
-import sqlalchemy
+import sqlalchemy as sa
+import sqlalchemy.orm
 
 from . import database
 
 _SETTINGS: Optional[Settings] = None
 _DEFAULT_CACHE_DIR = pathlib.Path(tempfile.gettempdir()) / "cacholote"
 _DEFAULT_CACHE_DIR.mkdir(exist_ok=True)
 
@@ -54,15 +55,15 @@
 
     @pydantic.validator("create_engine_kwargs", allow_reuse=True)
     def validate_create_engine_kwargs(
         cls: pydantic.BaseSettings, create_engine_kwargs: Dict[str, Any]
     ) -> Dict[str, Any]:
         poolclass = create_engine_kwargs.get("poolclass")
         if isinstance(poolclass, str):
-            create_engine_kwargs["poolclass"] = getattr(sqlalchemy.pool, poolclass)
+            create_engine_kwargs["poolclass"] = getattr(sa.pool, poolclass)
         return create_engine_kwargs
 
     @pydantic.validator("return_cache_entry", allow_reuse=True)
     def validate_return_cache_entry(
         cls: pydantic.BaseSettings, return_cache_entry: bool, values: Dict[str, Any]
     ) -> bool:
         if return_cache_entry is True and values["use_cache"] is False:
@@ -86,21 +87,21 @@
             or str(database.ENGINE.url) != self.cache_db_urlpath
         ):
             database._set_engine_and_session(
                 self.cache_db_urlpath, self.create_engine_kwargs
             )
 
     @property
-    def engine(self) -> sqlalchemy.engine.Engine:
+    def engine(self) -> sa.engine.Engine:
         if database.ENGINE is None:
             raise ValueError(_CONFIG_NOT_SET_MSG)
         return database.ENGINE
 
     @property
-    def sessionmaker(self) -> sqlalchemy.orm.sessionmaker:  # type: ignore[type-arg]
+    def sessionmaker(self) -> sa.orm.sessionmaker:  # type: ignore[type-arg]
         if database.SESSIONMAKER is None:
             raise ValueError(_CONFIG_NOT_SET_MSG)
         return database.SESSIONMAKER
 
     class Config:
         case_sensitive = False
         env_prefix = "cacholote_"
```

### Comparing `cacholote-0.3.0/cacholote/decode.py` & `cacholote-0.3.1/cacholote/decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/cacholote/encode.py` & `cacholote-0.3.1/cacholote/encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/cacholote/extra_encoders.py` & `cacholote-0.3.1/cacholote/extra_encoders.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,30 @@
         mimetypes.add_type("application/x-grib", ext, strict=False)
     mimetypes.add_type("application/vnd+zarr", ".zarr", strict=False)
 
 
 _add_ext_to_mimetypes()
 
 
+def _guess_type(
+    fs: fsspec.AbstractFileSystem,
+    local_path: str,
+    default: str = "application/octet-stream",
+) -> str:
+    content_type: str = fs.info(local_path).get("ContentType", "")
+    if content_type:
+        return content_type
+
+    filetype, *_ = mimetypes.guess_type(local_path, strict=False)
+    if filetype is None and _HAS_MAGIC:
+        with fs.open(local_path, "rb") as f:
+            filetype = magic.from_buffer(f.read(), mime=True)
+    return filetype or default
+
+
 def _requires_xarray_and_dask(func: F) -> F:
     """Raise an error if `xarray` or `dask` are not installed."""
 
     @functools.wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         if not _HAS_XARRAY_AND_DASK:
             raise ValueError("please install 'xarray' and 'dask'")
@@ -85,29 +101,21 @@
     href: str
     file_checksum: int = pydantic.Field(..., alias="file:checksum")
     file_size: int = pydantic.Field(..., alias="file:size")
     file_local_path: str = pydantic.Field(..., alias="file:local_path")
 
 
 def _dictify_file(fs: fsspec.AbstractFileSystem, local_path: str) -> Dict[str, Any]:
-    filetype = mimetypes.guess_type(local_path, strict=False)[0]
-    if filetype is None and _HAS_MAGIC:
-        with fs.open(local_path, "rb") as f:
-            filetype = magic.from_buffer(f.read(), mime=True)
-            if filetype == "application/octet-stream":
-                filetype = None
-    filetype = filetype or "unknown"
-
+    href = posixpath.join(
+        config.get().cache_files_urlpath_readonly or config.get().cache_files_urlpath,
+        posixpath.basename(local_path),
+    )
     file_dict = {
-        "type": filetype,
-        "href": posixpath.join(
-            config.get().cache_files_urlpath_readonly
-            or config.get().cache_files_urlpath,
-            posixpath.basename(local_path),
-        ),
+        "type": _guess_type(fs, local_path),
+        "href": href,
         "file:checksum": fs.checksum(local_path),
         "file:size": fs.size(local_path),
         "file:local_path": local_path,
     }
 
     return FileInfoModel(**file_dict).dict(by_alias=True)
 
@@ -118,31 +126,31 @@
     validate: bool = False,
 ) -> Tuple[fsspec.AbstractFileSystem, str]:
     urlpath = file_json["file:local_path"]
     if storage_options is None:
         storage_options = config.get().cache_files_storage_options
 
     if not validate:
-        fs, _, _ = fsspec.get_fs_token_paths(urlpath, storage_options=storage_options)
+        fs, *_ = fsspec.get_fs_token_paths(urlpath, storage_options=storage_options)
         return (fs, urlpath)
 
     # Attempt to read from local_path
     try:
-        fs, _, _ = fsspec.get_fs_token_paths(urlpath, storage_options=storage_options)
+        fs, *_ = fsspec.get_fs_token_paths(urlpath, storage_options=storage_options)
     except:  # noqa: E722
         pass
     else:
         if fs.exists(urlpath):
             if fs.checksum(urlpath) == file_json["file:checksum"]:
                 return (fs, urlpath)
             raise ValueError("checksum mismatch")
 
     # Attempt to read from href
     urlpath = file_json["href"]
-    fs, _, _ = fsspec.get_fs_token_paths(urlpath)
+    fs, *_ = fsspec.get_fs_token_paths(urlpath)
     if fs.exists(urlpath):
         return (fs, urlpath)
 
     # Nothing worked
     raise ValueError(
         f"No such file or directory: {file_json['file:local_path']!r} nor {file_json['href']!r}"
     )
@@ -155,23 +163,23 @@
     fs, urlpath = _get_fs_and_urlpath(
         file_json, storage_options=storage_options, validate=True
     )
 
     if file_json["type"] == "application/vnd+zarr":
         filename_or_obj = fs.get_mapper(urlpath)
     else:
-        if fsspec.utils.get_protocol(urlpath) == "file":
+        if fs.protocol == "file":
             filename_or_obj = urlpath
         else:
             # Download local copy
-            protocol = fsspec.utils.get_protocol(urlpath)
+            protocols = [fs.protocol] if isinstance(fs.protocol, str) else fs.protocol
             with fsspec.open(
                 f"filecache::{urlpath}",
                 filecache={"same_names": True},
-                **{protocol: fs.storage_options},
+                **{protocol: fs.storage_options for protocol in protocols},
             ) as of:
                 filename_or_obj = of.name
     return xr.open_dataset(filename_or_obj, **kwargs)
 
 
 def decode_io_object(
     file_json: Dict[str, Any], storage_options: Dict[str, Any], **kwargs: Any
@@ -182,57 +190,49 @@
     return fs.open(urlpath, **kwargs)
 
 
 @_requires_xarray_and_dask
 def _maybe_store_xr_dataset(
     obj: "xr.Dataset", fs: fsspec.AbstractFileSystem, urlpath: str, filetype: str
 ) -> None:
-    with utils._Locker(fs, urlpath) as file_exists:
-        if not file_exists:
-            if filetype == "application/vnd+zarr":
-                # Write directly on any filesystem
-                mapper = fs.get_mapper(urlpath)
-                obj.to_zarr(mapper, consolidated=True)
+    if filetype == "application/vnd+zarr":
+        # Write directly on any filesystem
+        mapper = fs.get_mapper(urlpath)
+        obj.to_zarr(mapper, consolidated=True)
+    else:
+        # Need a tmp local copy to write on a different filesystem
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            tmpfilename = str(pathlib.Path(tmpdirname) / pathlib.Path(urlpath).name)
+
+            if filetype == "application/netcdf":
+                obj.to_netcdf(tmpfilename)
+            elif filetype == "application/x-grib":
+                import cfgrib.xarray_to_grib
+
+                cfgrib.xarray_to_grib.to_grib(obj, tmpfilename)
             else:
-                # Need a tmp local copy to write on a different filesystem
-                with tempfile.TemporaryDirectory() as tmpdirname:
-                    tmpfilename = str(
-                        pathlib.Path(tmpdirname) / pathlib.Path(urlpath).name
-                    )
-
-                    if filetype == "application/netcdf":
-                        obj.to_netcdf(tmpfilename)
-                    elif filetype == "application/x-grib":
-                        import cfgrib.xarray_to_grib
-
-                        cfgrib.xarray_to_grib.to_grib(obj, tmpfilename)
-                    else:
-                        # Should never get here! xarray_cache_type is checked in config.py
-                        raise ValueError(f"type {filetype!r} is NOT supported.")
-
-                    if fs == fsspec.filesystem("file"):
-                        fsspec.filesystem("file").mv(tmpfilename, urlpath)
-                    else:
-                        with fsspec.open(tmpfilename, "rb") as f_in, fs.open(
-                            urlpath, "wb"
-                        ) as f_out:
-                            utils.copy_buffered_file(f_in, f_out)
+                # Should never get here! xarray_cache_type is checked in config.py
+                raise ValueError(f"type {filetype!r} is NOT supported.")
+
+            _maybe_store_file_object(
+                fsspec.filesystem("file"), tmpfilename, fs, urlpath
+            )
 
 
 @_requires_xarray_and_dask
 def dictify_xr_dataset(obj: "xr.Dataset") -> Dict[str, Any]:
     """Encode a ``xr.Dataset`` to JSON deserialized data (``dict``)."""
     with dask.config.set({"tokenize.ensure-deterministic": True}):
         root = dask.base.tokenize(obj)  # type: ignore[no-untyped-call]
 
     filetype = config.get().xarray_cache_type
     ext = mimetypes.guess_extension(filetype, strict=False)
     urlpath_out = posixpath.join(config.get().cache_files_urlpath, f"{root}{ext}")
 
-    fs_out, _, _ = fsspec.get_fs_token_paths(
+    fs_out, *_ = fsspec.get_fs_token_paths(
         urlpath_out,
         storage_options=config.get().cache_files_storage_options,
     )
     _maybe_store_xr_dataset(obj, fs_out, urlpath_out, filetype)
 
     file_json = _dictify_file(fs_out, urlpath_out)
     kwargs: Dict[str, Any] = {"chunks": {}}
@@ -251,26 +251,32 @@
     fs_in: fsspec.AbstractFileSystem,
     urlpath_in: str,
     fs_out: fsspec.AbstractFileSystem,
     urlpath_out: str,
 ) -> None:
     with utils._Locker(fs_out, urlpath_out) as file_exists:
         if not file_exists:
+            kwargs = {}
+            content_type = _guess_type(fs_in, urlpath_in)
+            if content_type:
+                kwargs["ContentType"] = content_type
             if fs_in == fs_out:
                 if config.get().io_delete_original:
-                    fs_in.mv(urlpath_in, urlpath_out)
+                    fs_in.mv(urlpath_in, urlpath_out, **kwargs)
                 else:
-                    fs_in.cp(urlpath_in, urlpath_out)
+                    fs_in.cp(urlpath_in, urlpath_out, **kwargs)
+            elif fs_in.protocol == "file":
+                fs_out.put(urlpath_in, urlpath_out, **kwargs)
             else:
                 with fs_in.open(urlpath_in, "rb") as f_in, fs_out.open(
                     urlpath_out, "wb"
                 ) as f_out:
                     utils.copy_buffered_file(f_in, f_out)
-                if config.get().io_delete_original and fs_in.exists(urlpath_in):
-                    fs_in.rm(urlpath_in)
+    if config.get().io_delete_original and fs_in.exists(urlpath_in):
+        fs_in.rm(urlpath_in)
 
 
 def _maybe_store_io_object(
     f_in: _UNION_IO_TYPES,
     fs_out: fsspec.AbstractFileSystem,
     urlpath_out: str,
 ) -> None:
@@ -279,15 +285,15 @@
             f_out = fs_out.open(urlpath_out, "wb")
             utils.copy_buffered_file(f_in, f_out)
 
 
 def dictify_io_object(obj: _UNION_IO_TYPES) -> Dict[str, Any]:
     """Encode a file object to JSON deserialized data (``dict``)."""
     cache_files_urlpath = config.get().cache_files_urlpath
-    fs_out, _, _ = fsspec.get_fs_token_paths(
+    fs_out, *_ = fsspec.get_fs_token_paths(
         cache_files_urlpath,
         storage_options=config.get().cache_files_storage_options,
     )
 
     if hasattr(obj, "path") or hasattr(obj, "name"):
         urlpath_in = obj.path if hasattr(obj, "path") else obj.name  # type: ignore[union-attr]
         fs_in = getattr(obj, "fs", fsspec.filesystem("file"))
```

### Comparing `cacholote-0.3.0/cacholote/utils.py` & `cacholote-0.3.1/cacholote/utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/cacholote.egg-info/PKG-INFO` & `cacholote-0.3.1/cacholote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cacholote
-Version: 0.3.0
+Version: 0.3.1
 Summary: Efficiently cache calls to functions
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cacholote-0.3.0/cacholote.egg-info/SOURCES.txt` & `cacholote-0.3.1/cacholote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/docs/Makefile` & `cacholote-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/docs/conf.py` & `cacholote-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/docs/make.bat` & `cacholote-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/pyproject.toml` & `cacholote-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering"
 ]
 dependencies = [
   "fsspec",
   "pydantic[dotenv]",
-  "sqlalchemy",
+  "sqlalchemy>=2.0.9",
   "structlog"
 ]
 description = "Efficiently cache calls to functions"
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "cacholote"
 readme = "README.md"
```

### Comparing `cacholote-0.3.0/tests/conftest.py` & `cacholote-0.3.1/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,20 @@
 def initialize_s3() -> Generator[Dict[str, str], None, None]:
     pytest.importorskip("boto3")
     if "AWS_SECRET_ACCESS_KEY" not in os.environ:
         os.environ["AWS_SECRET_ACCESS_KEY"] = "foo"
     if "AWS_ACCESS_KEY_ID" not in os.environ:
         os.environ["AWS_ACCESS_KEY_ID"] = "foo"
     port = 5555
-    proc = subprocess.Popen(shlex.split(f"moto_server s3 -p {port}"))
+    proc = subprocess.Popen(
+        shlex.split(f"moto_server s3 -p {port}"),
+        stderr=subprocess.DEVNULL,
+        stdout=subprocess.DEVNULL,
+        stdin=subprocess.DEVNULL,
+    )
     endpoint_url = f"http://127.0.0.1:{port}/"
     wait_s3_up(endpoint_url)
     try:
         yield {"endpoint_url": endpoint_url}
     finally:
         proc.terminate()
         proc.wait()
```

### Comparing `cacholote-0.3.0/tests/test_01_settings.py` & `cacholote-0.3.1/tests/test_01_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import pathlib
 from typing import Any, Dict, Union
 
 import pytest
-import sqlalchemy
+import sqlalchemy as sa
 
 from cacholote import config
 
 
 def test_change_cache_db_urlpath(tmpdir: pathlib.Path) -> None:
     old_db = config.get().cache_db_urlpath
     new_db = "sqlite:///" + str(tmpdir / "dummy.db")
@@ -80,13 +80,13 @@
         assert config.get().io_delete_original is True
         assert str(config.get().engine.url) == "sqlite://"
     finally:
         os.environ.clear()
         os.environ.update(old_environ)
 
 
-@pytest.mark.parametrize("poolclass", ("NullPool", sqlalchemy.pool.NullPool))
-def test_set_poolclass(poolclass: Union[str, sqlalchemy.pool.Pool]) -> None:
+@pytest.mark.parametrize("poolclass", ("NullPool", sa.pool.NullPool))
+def test_set_poolclass(poolclass: Union[str, sa.pool.Pool]) -> None:
     config.set(create_engine_kwargs={"poolclass": poolclass})
     settings = config.get()
-    assert settings.create_engine_kwargs["poolclass"] == sqlalchemy.pool.NullPool
-    assert isinstance(settings.engine.pool, sqlalchemy.pool.NullPool)
+    assert settings.create_engine_kwargs["poolclass"] == sa.pool.NullPool
+    assert isinstance(settings.engine.pool, sa.pool.NullPool)
```

### Comparing `cacholote-0.3.0/tests/test_02_utils.py` & `cacholote-0.3.1/tests/test_02_utils.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/tests/test_10_decode.py` & `cacholote-0.3.1/tests/test_10_decode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/tests/test_20_encode.py` & `cacholote-0.3.1/tests/test_20_encode.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/tests/test_30_cache.py` & `cacholote-0.3.1/tests/test_30_cache.py`

 * *Files identical despite different names*

### Comparing `cacholote-0.3.0/tests/test_40_xarray_encoder.py` & `cacholote-0.3.1/tests/test_40_xarray_encoder.py`

 * *Files 19% similar despite different names*

```diff
@@ -119,30 +119,37 @@
 )
 def test_xr_corrupted_files(
     xarray_cache_type: str,
     ext: str,
     importorskip: str,
 ) -> None:
     pytest.importorskip(importorskip)
+    import dask
 
     config.set(xarray_cache_type=xarray_cache_type)
 
     # Cache file
     fs, dirname = utils.get_cache_files_fs_dirname()
     expected = get_grib_ds()
     cfunc = cache.cacheable(get_grib_ds)
     cfunc()
 
+    # Get cached file path
+    with dask.config.set({"tokenize.ensure-deterministic": True}):
+        root = dask.base.tokenize(expected)  # type: ignore[no-untyped-call]
+    cached_path = f"{dirname}/{root}{ext}"
+    assert fs.exists(cached_path)
+
     # Warn if file is corrupted
-    fs.touch(f"{dirname}/b8094ae0691cfa42c9b839679e162e3d{ext}", truncate=False)
-    touched_info = fs.info(f"{dirname}/b8094ae0691cfa42c9b839679e162e3d{ext}")
+    fs.touch(cached_path, truncate=False)
+    touched_info = fs.info(cached_path)
     with pytest.warns(UserWarning, match="checksum mismatch"):
         actual = cfunc()
     xr.testing.assert_identical(actual, expected)
-    assert fs.info(f"{dirname}/b8094ae0691cfa42c9b839679e162e3d{ext}") != touched_info
+    assert fs.info(cached_path) != touched_info
 
     # Warn if file is deleted
-    fs.rm(f"{dirname}/b8094ae0691cfa42c9b839679e162e3d{ext}", recursive=True)
+    fs.rm(cached_path, recursive=True)
     with pytest.warns(UserWarning, match="No such file or directory"):
         actual = cfunc()
     xr.testing.assert_identical(actual, expected)
-    assert fs.exists(f"{dirname}/b8094ae0691cfa42c9b839679e162e3d{ext}")
+    assert fs.exists(cached_path)
```

### Comparing `cacholote-0.3.0/tests/test_50_io_encoder.py` & `cacholote-0.3.1/tests/test_50_io_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 import fsspec
 import pytest
 import pytest_httpserver
 
 from cacholote import cache, config, decode, encode, extra_encoders, utils
 
 
-def open_url(url: str) -> fsspec.spec.AbstractBufferedFile:
-    with fsspec.open(url) as f:
+@cache.cacheable
+def cached_open(*args: Any, **kwargs: Any) -> fsspec.spec.AbstractBufferedFile:
+    with fsspec.open(*args, **kwargs) as f:
         return f
 
 
 @pytest.mark.parametrize("io_delete_original", [True, False])
 def test_dictify_io_object(tmpdir: pathlib.Path, io_delete_original: bool) -> None:
     # Define readonly dir
     readonly_dir = str(tmpdir / "readonly")
@@ -63,17 +64,22 @@
 def test_dictify_bytes_io_object(
     tmpdir: pathlib.Path, obj: Union[io.BytesIO, io.StringIO]
 ) -> None:
     actual = extra_encoders.dictify_io_object(obj)["args"]
     obj_hash = hashlib.md5(f"{hash(obj)}".encode()).hexdigest()
     local_path = f"{tmpdir}/cache_files/{obj_hash}"
     checksum = fsspec.filesystem("file").checksum(local_path)
+    type = (
+        "text/plain"
+        if importlib.util.find_spec("magic")
+        else "application/octet-stream"
+    )
     expected: Tuple[Dict[str, Any], ...] = (
         {
-            "type": "text/plain" if importlib.util.find_spec("magic") else "unknown",
+            "type": type,
             "href": local_path,
             "file:checksum": checksum,
             "file:size": 4,
             "file:local_path": local_path,
         },
         {},
     )
@@ -94,17 +100,16 @@
     # http server
     httpserver.expect_request("/test").respond_with_data(b"test")
     url = httpserver.url_for("/test")
     cached_basename = f"{fsspec.filesystem('http').checksum(url):x}"
 
     # cache http file
     fs, dirname = utils.get_cache_files_fs_dirname()
-    cfunc = cache.cacheable(open_url)
     for expected_counter in (1, 2):
-        result = cfunc(url)
+        result = cached_open(url)
 
         # Check hits
         cur.execute("SELECT counter FROM cache_entries", ())
         assert cur.fetchall() == [(expected_counter,)]
 
         # Check result
         assert result.read() == b"test"
@@ -120,35 +125,34 @@
     # http server
     httpserver.expect_request("/test").respond_with_data(b"test")
     url = httpserver.url_for("/test")
     cached_basename = f"{fsspec.filesystem('http').checksum(url):x}"
 
     # cache file
     fs, dirname = utils.get_cache_files_fs_dirname()
-    cfunc = cache.cacheable(open_url)
-    cfunc(url)
+    cached_open(url)
 
     # Warn if file is corrupted
     fs.touch(f"{dirname}/{cached_basename}")
     touched_info = fs.info(f"{dirname}/{cached_basename}")
     with pytest.warns(UserWarning, match="checksum mismatch"):
-        result = cfunc(url)
+        result = cached_open(url)
     assert result.read() == b"test"
     assert fs.info(f"{dirname}/{cached_basename}") != touched_info
 
     # Warn if file is deleted
     fs.rm(f"{dirname}/{cached_basename}")
     with pytest.warns(UserWarning, match="No such file or directory"):
-        result = cfunc(url)
+        result = cached_open(url)
     assert result.read() == b"test"
     assert fs.exists(f"{dirname}/{cached_basename}")
 
 
 def test_io_locker_warning(tmpdir: pathlib.Path) -> None:
-    cfunc = cache.cacheable(open)
+    cached_open = cache.cacheable(open)
 
     # Create tmpfile
     tmpfile = tmpdir / "test.txt"
     fsspec.filesystem("file").touch(tmpfile)
 
     # Acquire lock
     fs, dirname = utils.get_cache_files_fs_dirname()
@@ -156,16 +160,25 @@
     lock = f"{dirname}/{file_hash}.txt.lock"
     fs.touch(lock)
 
     def release_lock(fs: fsspec.AbstractFileSystem, lock: str) -> None:
         fs.rm(lock)
 
     # Threading
-    t1 = threading.Timer(0, cfunc, args=(tmpfile,))
+    t1 = threading.Timer(0, cached_open, args=(tmpfile,))
     t2 = threading.Timer(0.1, release_lock, args=(fs, lock))
     with pytest.warns(
         UserWarning, match=f"can NOT proceed until file is released: {lock!r}."
     ):
         t1.start()
         t2.start()
         t1.join()
         t2.join()
+
+
+@pytest.mark.parametrize("set_cache", ["cads"], indirect=True)
+def test_content_type(tmpdir: pathlib.Path, set_cache: str) -> None:
+    tmpfile = str(tmpdir / "test.grib")
+    fsspec.filesystem("file").touch(tmpfile)
+    fs, _ = utils.get_cache_files_fs_dirname()
+    cached_grib = cached_open(tmpfile)
+    assert fs.info(cached_grib)["ContentType"] == "application/x-grib"
```

### Comparing `cacholote-0.3.0/tests/test_60_clean.py` & `cacholote-0.3.1/tests/test_60_clean.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,61 +24,55 @@
     method: Literal["LRU", "LFU"],
 ) -> None:
     con = config.get().engine.raw_connection()
     cur = con.cursor()
     fs, dirname = utils.get_cache_files_fs_dirname()
 
     # Create files
-    paths = {}
     for algorithm in ("LRU", "LFU"):
         filename = tmpdir / f"{algorithm}.txt"
         fsspec.filesystem("file").pipe_file(filename, b"1")
-        file_hash = f"{fsspec.filesystem('file').checksum(filename):x}"
-        cachedname = f"{dirname}/{file_hash}.txt"
-        paths[algorithm] = cachedname
 
     # Copy to cache
-    open_url(tmpdir / "LRU.txt")
-    open_url(tmpdir / "LRU.txt")
-    open_url(tmpdir / "LFU.txt")
-    assert set(fs.ls(dirname)) == set(paths.values())
+    (lru_path,) = {open_url(tmpdir / "LRU.txt").path for _ in range(2)}
+    lfu_path = open_url(tmpdir / "LFU.txt").path
+    assert set(fs.ls(dirname)) == {lru_path, lfu_path}
 
     # Do not clean
     clean.clean_cache_files(2, method=method)
     cur.execute("SELECT * FROM cache_entries", ())
     nrows = len(cur.fetchall())
     assert nrows == fs.du(dirname) == 2
 
     # Delete one file
     clean.clean_cache_files(1, method=method)
     cur.execute("SELECT * FROM cache_entries", ())
     nrows = len(cur.fetchall())
     assert nrows == fs.du(dirname) == 1
-    assert not fs.exists(f"{dirname}/{paths[method]}.txt")
+    assert not fs.exists(lru_path if method == "LRU" else lfu_path)
 
 
 @pytest.mark.parametrize("delete_unknown_files", [True, False])
 def test_delete_unknown_files(tmpdir: pathlib.Path, delete_unknown_files: bool) -> None:
     fs, dirname = utils.get_cache_files_fs_dirname()
 
     # Create file
     tmpfile = tmpdir / "test.txt"
     fsspec.filesystem("file").pipe_file(tmpfile, b"1")
 
     # Copy to cache
-    open_url(tmpfile)
+    cached_file = open_url(tmpfile).path
 
     # Add unknown
     fs.put(str(tmpfile), f"{dirname}/unknown.txt")
 
     # Clean one file
     clean.clean_cache_files(1, delete_unknown_files=delete_unknown_files)
     if delete_unknown_files:
-        file_hash = f"{fs.checksum(tmpfile):x}"
-        assert fs.ls(dirname) == [f"{dirname}/{file_hash}.txt"]
+        assert fs.ls(dirname) == [cached_file]
     else:
         assert fs.ls(dirname) == [f"{dirname}/unknown.txt"]
 
 
 @pytest.mark.parametrize(
     "recursive,raises,final_size",
     [
@@ -104,62 +98,63 @@
     fs, dirname = utils.get_cache_files_fs_dirname()
 
     # Create file
     tmpfile = tmpdir / "test.txt"
     fsspec.filesystem("file").pipe_file(tmpfile, b"1")
 
     # Copy to cache
-    open_url(tmpfile)
+    cached_file = open_url(tmpfile).path
 
     # Add unknown and lock
     fs.put(str(tmpfile), f"{dirname}/unknown.txt")
     fs.touch(f"{dirname}/unknown.txt.lock")
 
     # Clean one file
     clean.clean_cache_files(
         1, delete_unknown_files=True, lock_validity_period=lock_validity_period
     )
     if lock_validity_period == 0:
-        file_hash = f"{fs.checksum(tmpfile):x}"
-        assert fs.ls(dirname) == [f"{dirname}/{file_hash}.txt"]
+        assert fs.ls(dirname) == [cached_file]
     else:
         assert set(fs.ls(dirname)) == {
             f"{dirname}/unknown.txt",
             f"{dirname}/unknown.txt.lock",
         }
 
 
 @pytest.mark.parametrize(
-    "tags_to_clean, tags_to_keep, expected",
+    "tags_to_clean, tags_to_keep, cleaned",
     [
-        ({None, "1"}, None, "2"),
-        ({None, "2"}, None, "1"),
-        ({"1", "2"}, None, None),
-        (None, {None}, None),
-        (None, {"1"}, "1"),
-        (None, {"2"}, "2"),
+        ({None, "1"}, None, {None, "1"}),
+        ({None, "2"}, None, {None, "2"}),
+        ({"1", "2"}, None, {"1", "2"}),
+        (None, {None}, {"1", "2"}),
+        (None, {"1"}, {None, "2"}),
+        (None, {"2"}, {None, "1"}),
     ],
 )
 def test_clean_tagged_files(
     tmpdir: pathlib.Path,
     tags_to_clean: Optional[Sequence[Optional[str]]],
     tags_to_keep: Optional[Sequence[Optional[str]]],
-    expected: Optional[str],
+    cleaned: Sequence[Optional[str]],
 ) -> None:
     fs, dirname = utils.get_cache_files_fs_dirname()
 
+    expected_ls = []
     for tag in [None, "1", "2"]:
         tmpfile = tmpdir / f"test_{tag}.txt"
         fsspec.filesystem("file").pipe_file(tmpfile, b"1")
         with config.set(tag=tag):
-            open_url(tmpfile)
+            cached_file = open_url(tmpfile).path
+        if tag not in cleaned:
+            expected_ls.append(cached_file)
 
     clean.clean_cache_files(1, tags_to_clean=tags_to_clean, tags_to_keep=tags_to_keep)
-    file_hash = f"{fs.checksum(tmpdir / f'test_{expected}.txt'):x}"
-    assert fs.ls(dirname) == [f"{dirname}/{file_hash}.txt"]
+    assert fs.ls(dirname) == expected_ls
 
 
 def test_clean_tagged_files_wrong_args() -> None:
     with pytest.raises(
         ValueError,
         match="tags_to_clean/keep are mutually exclusive.",
     ):
```

