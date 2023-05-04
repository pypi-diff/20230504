# Comparing `tmp/pz-rail-hub-0.0.4.tar.gz` & `tmp/pz-rail-hub-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-hub-0.0.4.tar", last modified: Thu Sep 15 17:45:04 2022, max compression
+gzip compressed data, was "pz-rail-hub-0.0.5.tar", last modified: Thu May  4 06:06:16 2023, max compression
```

## Comparing `pz-rail-hub-0.0.4.tar` & `pz-rail-hub-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/src/pz_rail_hub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-09-15 17:45:04.000000 pz-rail-hub-0.0.4/src/pz_rail_hub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-15 17:45:04.000000 pz-rail-hub-0.0.4/src/pz_rail_hub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 17:45:04.000000 pz-rail-hub-0.0.4/src/pz_rail_hub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-15 17:45:04.000000 pz-rail-hub-0.0.4/src/pz_rail_hub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-15 17:45:04.000000 pz-rail-hub-0.0.4/src/pz_rail_hub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/src/rail/stages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-15 17:45:03.000000 pz-rail-hub-0.0.4/src/rail/stages/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:45:04.421721 pz-rail-hub-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-15 17:44:55.000000 pz-rail-hub-0.0.4/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2043 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/src/rail/stages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 06:06:15.000000 pz-rail-hub-0.0.5/src/rail/stages/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/tests/test_import.py
```

### Comparing `pz-rail-hub-0.0.4/.github/workflows/main.yml` & `pz-rail-hub-0.0.5/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

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
         python -m pytest --cov=./rail --cov-report=xml
     - name: Upload coverage to Codecov
```

### Comparing `pz-rail-hub-0.0.4/.github/workflows/pypi.yaml` & `pz-rail-hub-0.0.5/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.0.4/.gitignore` & `pz-rail-hub-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.0.4/LICENSE` & `pz-rail-hub-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.0.4/PKG-INFO` & `pz-rail-hub-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-hub
-Version: 0.0.4
+Version: 0.0.5
 Summary: RAIL top-level umbrella packages
 Author-email: The LSST DESC PZ WG <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-hub-0.0.4/pyproject.toml` & `pz-rail-hub-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
-    "pz-rail>=0.98.2",
-    "pz-rail-delight>=0.0.4",
-    "pz-rail-bpz>=0.0.6",
-    "pz-rail-flexzboost>=0.0.5",
+    "pz-rail>=0.98.4",
+    "pz-rail-bpz>=0.0.9",
+    "pz-rail-flexzboost>=0.0.9",
+    "pz-rail-gpz-v1>=0.1.1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage",
     "pylint",
     "pytest",
```

### Comparing `pz-rail-hub-0.0.4/src/pz_rail_hub.egg-info/PKG-INFO` & `pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-hub
-Version: 0.0.4
+Version: 0.0.5
 Summary: RAIL top-level umbrella packages
 Author-email: The LSST DESC PZ WG <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-hub-0.0.4/src/rail/stages/__init__.py` & `pz-rail-hub-0.0.5/src/rail/stages/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 from rail.estimation.algos.NZDir import *
 from rail.estimation.algos.knnpz import *
 from rail.estimation.algos.naiveStack import *
 from rail.estimation.algos.pointEstimateHist import *
 from rail.estimation.algos.pzflow import *
 from rail.estimation.algos.randomPZ import *
 from rail.estimation.algos.sklearn_nn import *
+from rail.estimation.algos.somocluSOM import *
 from rail.estimation.algos.trainZ import *
 from rail.estimation.algos.varInference import *
+from rail.estimation.algos.simpleSOM import *
 
 from rail.evaluation.evaluator import Evaluator
 
 try:
     from rail.estimation.algos.delightPZ import *
 except ImportError:  # pragma: no cover
     pass
@@ -32,9 +34,13 @@
     from rail.estimation.algos.bpz_lite import *
 except ImportError:  # pragma: no cover
     pass
 try:
     from rail.estimation.algos.flexzboost import *
 except ImportError:  # pragma: no cover
     pass
-    
+try:
+    from rail.estimation.algos.gpz_v1 import *
+except ImportError:  # pragma: no cover
+    pass
+ 
 from rail.evaluation import *
```

