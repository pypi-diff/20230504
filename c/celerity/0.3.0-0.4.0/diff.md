# Comparing `tmp/celerity-0.3.0.tar.gz` & `tmp/celerity-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celerity-0.3.0.tar", max compression
+gzip compressed data, was "celerity-0.4.0.tar", max compression
```

## Comparing `celerity-0.3.0.tar` & `celerity-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1075 2023-05-03 15:43:17.263886 celerity-0.3.0/LICENSE
--rw-r--r--   0        0        0     4346 2023-05-03 15:43:17.263886 celerity-0.3.0/README.md
--rw-r--r--   0        0        0     1830 2023-05-03 15:43:17.263886 celerity-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-03 15:43:17.263886 celerity-0.3.0/src/celerity/__init__.py
--rw-r--r--   0        0        0      684 2023-05-03 15:43:17.263886 celerity-0.3.0/src/celerity/astrometry.py
--rw-r--r--   0        0        0      997 2023-05-03 15:43:17.263886 celerity-0.3.0/src/celerity/constants.py
--rw-r--r--   0        0        0      714 2023-05-03 15:43:17.263886 celerity-0.3.0/src/celerity/seeing.py
--rw-r--r--   0        0        0     3771 2023-05-03 15:43:17.263886 celerity-0.3.0/src/celerity/temporal.py
--rw-r--r--   0        0        0      961 2023-05-03 15:43:17.263886 celerity-0.3.0/src/celerity/utilities.py
--rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 celerity-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-04 16:36:03.625378 celerity-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4346 2023-05-04 16:36:03.625378 celerity-0.4.0/README.md
+-rw-r--r--   0        0        0     1830 2023-05-04 16:36:03.625378 celerity-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/__init__.py
+-rw-r--r--   0        0        0     1752 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/astrometry.py
+-rw-r--r--   0        0        0      240 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/common.py
+-rw-r--r--   0        0        0      997 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/constants.py
+-rw-r--r--   0        0        0     1650 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/coordinates.py
+-rw-r--r--   0        0        0     2092 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/seeing.py
+-rw-r--r--   0        0        0     3771 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/temporal.py
+-rw-r--r--   0        0        0      961 2023-05-04 16:36:03.625378 celerity-0.4.0/src/celerity/utilities.py
+-rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 celerity-0.4.0/PKG-INFO
```

### Comparing `celerity-0.3.0/LICENSE` & `celerity-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celerity-0.3.0/README.md` & `celerity-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `celerity-0.3.0/pyproject.toml` & `celerity-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celerity"
-version = "0.3.0"
+version = "0.4.0"
 description = "Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations."
 authors = [
     "Michael J. Roberts <michael@observerly.com>"
 ]
 maintainers = [
     "Michael J. Roberts <michael@observerly.com>"
 ]
```

### Comparing `celerity-0.3.0/src/celerity/constants.py` & `celerity-0.4.0/src/celerity/constants.py`

 * *Files identical despite different names*

### Comparing `celerity-0.3.0/src/celerity/seeing.py` & `celerity-0.4.0/src/celerity/seeing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 import math
 
 
+def get_airmass(altitude: float) -> float:
+    """
+    Gets the airmass of an object at a given altitude using Pickering's formula.
+
+    Airmass is a measure of the amount of air along the line of sight when observing a star
+    or other celestial source from below Earth's atmosphere. It is formulated
+    as the integral of air density along the light ray.
+
+    :see: Pickering, K. A. (2002). "The Southern Limits of the Ancient Star Catalog" (PDF). DIO. 12 (1): 20-39.
+    :param: altitude: The altitude of the object in degrees.
+    :return: The airmass of the object.
+    """
+    return get_airmass_pickering(altitude)
+
+
 def get_airmass_pickering(altitude: float) -> float:
     """
     Gets the airmass of an object at a given altitude using Pickering's formula.
 
     Airmass is a measure of the amount of air along the line of sight when observing a star
     or other celestial source from below Earth's atmosphere. It is formulated
     as the integral of air density along the light ray.
@@ -12,7 +27,25 @@
     :see: Pickering, K. A. (2002). "The Southern Limits of the Ancient Star Catalog" (PDF). DIO. 12 (1): 20-39.
     :param: altitude: The altitude of the object in degrees.
     :return: The airmass of the object.
     """
     return 1 / math.sin(
         math.radians(altitude + 244 / (165 + (47 * math.pow(altitude, 1.1))))
     )
+
+
+def get_airmass_karstenyoung(altitude: float) -> float:
+    """
+    Gets the airmass of an object at a given altitude using Karsten & Young's formula.
+
+    Airmass is a measure of the amount of air along the line of sight when observing a star
+    or other celestial source from below Earth's atmosphere. It is formulated
+    as the integral of air density along the light ray.
+
+    :see: Kasten, F.; Young, A. T. (1989). "Revised optical air mass tables and approximation formula". Applied Optics. 28 (22): 4735-4738.
+    :param: altitude: The altitude of the object in degrees.
+    :return: The airmass of the object.
+    """
+    return 1 / (
+        math.sin(math.radians(altitude))
+        + 0.50572 * math.pow(altitude + 6.07995, -1.6364)
+    )
```

### Comparing `celerity-0.3.0/src/celerity/temporal.py` & `celerity-0.4.0/src/celerity/temporal.py`

 * *Files identical despite different names*

### Comparing `celerity-0.3.0/src/celerity/utilities.py` & `celerity-0.4.0/src/celerity/utilities.py`

 * *Files identical despite different names*

### Comparing `celerity-0.3.0/PKG-INFO` & `celerity-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celerity
-Version: 0.3.0
+Version: 0.4.0
 Summary: Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations.
 Home-page: https://github.com/michaelroberts/celerity
 Keywords: astronomy,astrometry,ephemeris
 Author: Michael J. Roberts
 Author-email: michael@observerly.com
 Maintainer: Michael J. Roberts
 Maintainer-email: michael@observerly.com
```

