# Comparing `tmp/morphosamplers-0.0.5.tar.gz` & `tmp/morphosamplers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphosamplers-0.0.5.tar", last modified: Tue Feb 28 14:39:41 2023, max compression
+gzip compressed data, was "morphosamplers-0.0.7.tar", last modified: Thu May  4 14:34:47 2023, max compression
```

## Comparing `morphosamplers-0.0.5.tar` & `morphosamplers-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:41.690906 morphosamplers-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:41.690906 morphosamplers-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:41.690906 morphosamplers-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-02-28 14:39:41.690906 morphosamplers-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 14:39:41.690906 morphosamplers-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:41.686906 morphosamplers-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:41.690906 morphosamplers-0.0.5/src/morphosamplers/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/src/morphosamplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/src/morphosamplers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/src/morphosamplers/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/src/morphosamplers/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/src/morphosamplers/surface_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/src/morphosamplers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:41.690906 morphosamplers-0.0.5/src/morphosamplers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-02-28 14:39:41.000000 morphosamplers-0.0.5/src/morphosamplers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-02-28 14:39:41.000000 morphosamplers-0.0.5/src/morphosamplers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:39:41.000000 morphosamplers-0.0.5/src/morphosamplers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:39:41.000000 morphosamplers-0.0.5/src/morphosamplers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-28 14:39:41.000000 morphosamplers-0.0.5/src/morphosamplers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 14:39:41.000000 morphosamplers-0.0.5/src/morphosamplers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:39:41.690906 morphosamplers-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/tests/test_spline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-28 14:39:26.000000 morphosamplers-0.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.github_changelog_generator
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/examples/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/examples/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/src/morphosamplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/models/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/models/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/sample_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/point_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/pose_sampler_helical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/pose_sampler_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/test_point_sampler_equidistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_helical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/_sphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/point_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/pose_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/samplers/sphere_samplers/tests/test_point_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19179 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/surface_spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/src/morphosamplers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.070617 morphosamplers-0.0.7/src/morphosamplers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:34:46.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 14:34:47.000000 morphosamplers-0.0.7/src/morphosamplers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:34:47.074617 morphosamplers-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/tests/test_spline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-04 14:34:30.000000 morphosamplers-0.0.7/tox.ini
```

### Comparing `morphosamplers-0.0.5/.cruft.json` & `morphosamplers-0.0.7/.cruft.json`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.5/.github/workflows/ci.yml` & `morphosamplers-0.0.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.5/.github/workflows/cron.yml` & `morphosamplers-0.0.7/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.5/.gitignore` & `morphosamplers-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.5/.pre-commit-config.yaml` & `morphosamplers-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.5/LICENSE` & `morphosamplers-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.5/PKG-INFO` & `morphosamplers-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphosamplers
-Version: 0.0.5
+Version: 0.0.7
 Summary: A library for sampling image data along morphological objects such as splines and surfaces.
 Author: Kevin Yamauchi
 Author-email: kevin.yamauchi@gmail.com
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/kevinyamauchi/morphosamplers
 Project-URL: repository, https://github.com/kevinyamauchi/morphosamplers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `morphosamplers-0.0.5/README.md` & `morphosamplers-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.5/pyproject.toml` & `morphosamplers-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 dynamic = ["version"]
 dependencies = [
     "einops",
     "numpy",
     "psygnal",
     "pydantic",
     "scipy",
+    "typing-extensions"
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 test = [
     "pytest>=6.0",
```

### Comparing `morphosamplers-0.0.5/src/morphosamplers/sampler.py` & `morphosamplers-0.0.7/src/morphosamplers/sampler.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.5/src/morphosamplers/spline.py` & `morphosamplers-0.0.7/src/morphosamplers/spline.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import numpy as np
 from psygnal import EventedModel
 from pydantic import PrivateAttr, conint, root_validator, validator
 from scipy.interpolate import splev, splprep
 from scipy.spatial.transform import Rotation, Slerp
 
-from .utils import calculate_y_vectors_from_z_vectors, within_range, get_mask_limits
+from .utils import coaxial_y_vectors_from_z_vectors, within_range, get_mask_limits
 
 
 class NDimensionalSpline(EventedModel):
     """Model for multidimensional splines."""
 
     points: np.ndarray
     order: conint(ge=1, le=5) = 3
@@ -243,24 +243,24 @@
         return v
 
     def _prepare_spline(self):
         super()._prepare_spline()
         self._prepare_orientation_sampler()
 
     def _prepare_orientation_sampler(self):
-        """Prepare a sampler yielding smoothly varying orientations along the spline.
+        """Prepare a pose_sampler yielding smoothly varying orientations along the spline.
 
         This method constructs a set of rotation matrices which vary smoothly with
-        the spline coordinate `u`. A sampler is then prepared which can be queried at
+        the spline coordinate `u`. A pose_sampler is then prepared which can be queried at
         any point(s) along the spline coordinate `u` and the resulting rotations vary
         smoothly along the spline
         """
         u = np.linspace(0, 1, num=self._n_spline_samples)
         z = self._sample_spline_z(u)
-        y = calculate_y_vectors_from_z_vectors(z)
+        y = coaxial_y_vectors_from_z_vectors(z)
         x = np.cross(y, z)
         r = Rotation.from_matrix(np.stack([x, y, z], axis=-1))
         self._rotation_sampler = Slerp(u, r)
 
     def sample_orientations(
         self,
         u: Optional[Union[float, np.ndarray]] = None,
```

### Comparing `morphosamplers-0.0.5/src/morphosamplers/surface_spline.py` & `morphosamplers-0.0.7/src/morphosamplers/surface_spline.py`

 * *Files 5% similar despite different names*

```diff
@@ -309,25 +309,30 @@
         Tuple[np.array, np.array]
             Vertices coordinates (n, 3) and indices of vertices forming triangle faces (m, 3)
         """
         points = self.sample()
         rows, columns = self.grid_shape
         row_range = np.arange(rows)
         column_range = np.arange(columns)
+        shift = 0
+        if self.closed:
+            columns += 1
+            shift = 1
+            column_range = np.append(column_range, 0)
 
         # first half of triangles
-        first_index = np.repeat(row_range[:-1], columns - 1) * columns + np.tile(column_range[:-1], rows - 1)
-        second_index = np.repeat(row_range[1:], columns - 1) * columns + np.tile(column_range[:-1], rows - 1)
-        third_index = np.repeat(row_range[:-1], columns - 1) * columns + np.tile(column_range[1:], rows - 1)
+        first_index = np.repeat(row_range[:-1], columns - 1) * (columns - shift) + np.tile(column_range[:-1], rows - 1)
+        second_index = np.repeat(row_range[1:], columns - 1) * (columns - shift) + np.tile(column_range[:-1], rows - 1)
+        third_index = np.repeat(row_range[:-1], columns - 1) * (columns - shift) + np.tile(column_range[1:], rows - 1)
         triangles_1 = np.stack([first_index, second_index, third_index], axis=1)
 
         # second half
-        first_index = np.repeat(row_range[1:], columns - 1) * columns + np.tile(column_range[:-1], rows - 1)
-        second_index = np.repeat(row_range[1:], columns - 1) * columns + np.tile(column_range[1:], rows - 1)
-        third_index = np.repeat(row_range[:-1], columns - 1) * columns + np.tile(column_range[1:], rows - 1)
+        first_index = np.repeat(row_range[1:], columns - 1) * (columns - shift) + np.tile(column_range[:-1], rows - 1)
+        second_index = np.repeat(row_range[1:], columns - 1) * (columns - shift) + np.tile(column_range[1:], rows - 1)
+        third_index = np.repeat(row_range[:-1], columns - 1) * (columns - shift) + np.tile(column_range[1:], rows - 1)
         triangles_2 = np.stack([first_index, second_index, third_index], axis=1)
 
         all_triangles = np.concatenate([triangles_1, triangles_2])
         return points, all_triangles
 
 
 class HexSplineSurface(_SplineSurface):
```

### Comparing `morphosamplers-0.0.5/src/morphosamplers/utils.py` & `morphosamplers-0.0.7/src/morphosamplers/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         # perfectly aligned
         return vector
     proj_plane = vector - normal_component * plane_normal
     proj_plane /= np.linalg.norm(proj_plane)
     return proj_plane
 
 
-def calculate_y_vectors_from_z_vectors(
+def coaxial_y_vectors_from_z_vectors(
     z: np.ndarray,
     initial_y_vector: Union[np.ndarray, Tuple[float, float, float]] = (0.3234, 0.6543, 0.978),
 ) -> np.ndarray:
     """Calculate y vectors starting from z vectors.
 
     This function will return the set of unit vectors perpendicular to the z-vectors
     which are maximally coaxial to their neighbours. It assumes that z vectors (n, 3)
@@ -49,15 +49,15 @@
     z = z.copy()
     z /= np.linalg.norm(z, axis=1, keepdims=True)
     y = np.empty((len(z), 3))
 
     if np.dot(initial_y_vector, z[0]) == 1:
         raise ValueError('cannot generate y vectors because the provided initial_y_vector '
                          'and the first z vector are perfectly aligned.')
-    # normalise initial y vector so that dot product is the projection
+    # normalise initial y vector so that the subsequent dot product is a projection
     initial_y_vector = initial_y_vector / np.linalg.norm(initial_y_vector)
 
     # initialise first y
     y[0] = _project_vector_onto_plane(initial_y_vector, z[0])
 
     # update y vectors in order
     for i in range(len(y) - 1):
```

### Comparing `morphosamplers-0.0.5/src/morphosamplers.egg-info/PKG-INFO` & `morphosamplers-0.0.7/src/morphosamplers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphosamplers
-Version: 0.0.5
+Version: 0.0.7
 Summary: A library for sampling image data along morphological objects such as splines and surfaces.
 Author: Kevin Yamauchi
 Author-email: kevin.yamauchi@gmail.com
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/kevinyamauchi/morphosamplers
 Project-URL: repository, https://github.com/kevinyamauchi/morphosamplers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `morphosamplers-0.0.5/tests/test_sampling.py` & `morphosamplers-0.0.7/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.5/tests/test_spline_model.py` & `morphosamplers-0.0.7/tests/test_spline_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 
 def test_spline_orientations():
     points = np.array([[0, 0, 0], [0, 0, 1], [0, 0, 2], [0, 0, 3]])
     spline = Spline3D(points=points, order=3)
     pt = spline.sample(u=0)
     # lower atol, as it's very strict by default, much more than np.allclose
-    np.testing.assert_allclose(pt, 0, atol=1e-20)
+    np.testing.assert_allclose(pt, 0, atol=1e-8)
     ori = spline.sample_orientations(u=0)
     np.testing.assert_allclose(ori.apply([0, 0, 1]), [[0, 0, 1]])
 
 
 def test_spline_reverse():
     """After reversing the last input point is the start when sampling."""
     points = np.array([[0, 0, 0], [0, 0, 1], [0, 0, 2], [0, 0, 3]])
```

### Comparing `morphosamplers-0.0.5/tox.ini` & `morphosamplers-0.0.7/tox.ini`

 * *Files identical despite different names*

