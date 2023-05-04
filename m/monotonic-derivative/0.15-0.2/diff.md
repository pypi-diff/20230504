# Comparing `tmp/monotonic_derivative-0.15-py3-none-any.whl.zip` & `tmp/monotonic_derivative-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5962 bytes, number of entries: 8
--rw-r--r--  2.0 unx       62 b- defN 23-May-04 13:31 monotonic_derivative/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-May-04 13:31 monotonic_derivative/_version.py
--rw-r--r--  2.0 unx     4961 b- defN 23-May-04 13:31 monotonic_derivative/monotonic_derivative.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-04 13:31 monotonic_derivative-0.15.dist-info/LICENSE
--rw-r--r--  2.0 unx     5544 b- defN 23-May-04 13:31 monotonic_derivative-0.15.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 13:31 monotonic_derivative-0.15.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-04 13:31 monotonic_derivative-0.15.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      721 b- defN 23-May-04 13:31 monotonic_derivative-0.15.dist-info/RECORD
-8 files, 12490 bytes uncompressed, 4678 bytes compressed:  62.5%
+Zip file size: 5949 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       62 b- defN 23-May-04 13:39 monotonic_derivative/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 23-May-04 13:39 monotonic_derivative/_version.py
+-rw-r--r--  2.0 unx     4961 b- defN 23-May-04 13:39 monotonic_derivative/monotonic_derivative.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-04 13:39 monotonic_derivative-0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5543 b- defN 23-May-04 13:39 monotonic_derivative-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 13:39 monotonic_derivative-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-04 13:39 monotonic_derivative-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      716 b- defN 23-May-04 13:39 monotonic_derivative-0.2.dist-info/RECORD
+8 files, 12484 bytes uncompressed, 4675 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: monotonic_derivative/_version.py
 Comment: 
 
 Filename: monotonic_derivative/monotonic_derivative.py
 Comment: 
 
-Filename: monotonic_derivative-0.15.dist-info/LICENSE
+Filename: monotonic_derivative-0.2.dist-info/LICENSE
 Comment: 
 
-Filename: monotonic_derivative-0.15.dist-info/METADATA
+Filename: monotonic_derivative-0.2.dist-info/METADATA
 Comment: 
 
-Filename: monotonic_derivative-0.15.dist-info/WHEEL
+Filename: monotonic_derivative-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: monotonic_derivative-0.15.dist-info/top_level.txt
+Filename: monotonic_derivative-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: monotonic_derivative-0.15.dist-info/RECORD
+Filename: monotonic_derivative-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `monotonic_derivative-0.15.dist-info/LICENSE` & `monotonic_derivative-0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `monotonic_derivative-0.15.dist-info/METADATA` & `monotonic_derivative-0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monotonic-derivative
-Version: 0.15
+Version: 0.2
 Summary: Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
 Home-page: https://github.com/A-Wpro/monotonic_derivative
 Author: Adam Wecker
 Author-email: adam.wecker0@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `monotonic_derivative-0.15.dist-info/RECORD` & `monotonic_derivative-0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 monotonic_derivative/__init__.py,sha256=sg-3SHskyJO_R7p4t20v-3-lNwOfK1UvdyZdIQFaSVQ,62
 monotonic_derivative/_version.py,sha256=Ocdgg742iYHFtMFCdmehuyOv50Vi5zoxdYiZyxk8rf0,21
 monotonic_derivative/monotonic_derivative.py,sha256=dJmAxfbwKxRTZdjnqaah8vOvtBIZ1Ja-DDk-kd28nwQ,4961
-monotonic_derivative-0.15.dist-info/LICENSE,sha256=EinmopNDNxPsqfThux4bLlHGDGNqqsPtEuDyG8Fkxs4,1068
-monotonic_derivative-0.15.dist-info/METADATA,sha256=mY5EDqea2mv65BWCoRrpo69qXzsmcOGogW41FwR2qfA,5544
-monotonic_derivative-0.15.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-monotonic_derivative-0.15.dist-info/top_level.txt,sha256=ijWgMhFhMNJrrQT8Gv32YtxDENd2e_vWZU-NEK3kkfQ,21
-monotonic_derivative-0.15.dist-info/RECORD,,
+monotonic_derivative-0.2.dist-info/LICENSE,sha256=EinmopNDNxPsqfThux4bLlHGDGNqqsPtEuDyG8Fkxs4,1068
+monotonic_derivative-0.2.dist-info/METADATA,sha256=KmfOShsFo7wGOUO4YWNhaDHA_7_lopanrRaMlQxrCJQ,5543
+monotonic_derivative-0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+monotonic_derivative-0.2.dist-info/top_level.txt,sha256=ijWgMhFhMNJrrQT8Gv32YtxDENd2e_vWZU-NEK3kkfQ,21
+monotonic_derivative-0.2.dist-info/RECORD,,
```

