# Comparing `tmp/imaginairy_normal_map-0.0.2-py3-none-any.whl.zip` & `tmp/imaginairy_normal_map-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7145 bytes, number of entries: 11
+Zip file size: 7208 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-May-04 06:14 imaginairy_normal_map/__init__.py
 -rw-r--r--  2.0 unx     5984 b- defN 23-May-04 06:14 imaginairy_normal_map/decoder.py
 -rw-r--r--  2.0 unx     1041 b- defN 23-May-04 06:14 imaginairy_normal_map/encoder.py
 -rw-r--r--  2.0 unx     3007 b- defN 23-May-04 06:14 imaginairy_normal_map/model.py
 -rw-r--r--  2.0 unx     1241 b- defN 23-May-04 06:14 imaginairy_normal_map/submodules.py
 -rw-r--r--  2.0 unx      277 b- defN 23-May-04 06:14 imaginairy_normal_map/utils.py
--rw-r--r--  2.0 unx     1102 b- defN 23-May-04 06:16 imaginairy_normal_map-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1918 b- defN 23-May-04 06:16 imaginairy_normal_map-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 06:16 imaginairy_normal_map-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-May-04 06:16 imaginairy_normal_map-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      986 b- defN 23-May-04 06:16 imaginairy_normal_map-0.0.2.dist-info/RECORD
-11 files, 15670 bytes uncompressed, 5445 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx     1102 b- defN 23-May-04 06:18 imaginairy_normal_map-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2139 b- defN 23-May-04 06:18 imaginairy_normal_map-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 06:18 imaginairy_normal_map-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-May-04 06:18 imaginairy_normal_map-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      986 b- defN 23-May-04 06:18 imaginairy_normal_map-0.0.3.dist-info/RECORD
+11 files, 15891 bytes uncompressed, 5508 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: imaginairy_normal_map/submodules.py
 Comment: 
 
 Filename: imaginairy_normal_map/utils.py
 Comment: 
 
-Filename: imaginairy_normal_map-0.0.2.dist-info/LICENSE
+Filename: imaginairy_normal_map-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: imaginairy_normal_map-0.0.2.dist-info/METADATA
+Filename: imaginairy_normal_map-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: imaginairy_normal_map-0.0.2.dist-info/WHEEL
+Filename: imaginairy_normal_map-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: imaginairy_normal_map-0.0.2.dist-info/top_level.txt
+Filename: imaginairy_normal_map-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: imaginairy_normal_map-0.0.2.dist-info/RECORD
+Filename: imaginairy_normal_map-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `imaginairy_normal_map-0.0.2.dist-info/LICENSE` & `imaginairy_normal_map-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `imaginairy_normal_map-0.0.2.dist-info/METADATA` & `imaginairy_normal_map-0.0.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaginairy-normal-map
-Version: 0.0.2
+Version: 0.0.3
 Summary: Image-to-normal-map 
 Author: Bryce Drennan
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch (>=1.7)
 Requires-Dist: torchvision
@@ -13,15 +13,15 @@
 
 # Image-to-Normal-Map
 **Create normal maps from images (using AI)**
 
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/estimating-and-exploiting-the-aleatoric/surface-normals-estimation-on-nyu-depth-v2-1)](https://paperswithcode.com/sota/surface-normals-estimation-on-nyu-depth-v2-1?p=estimating-and-exploiting-the-aleatoric)
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/estimating-and-exploiting-the-aleatoric/surface-normals-estimation-on-scannetv2)](https://paperswithcode.com/sota/surface-normals-estimation-on-scannetv2?p=estimating-and-exploiting-the-aleatoric)
 
-<img width=45% src="tests/oval-office-large.jpg"><img width=45% src="tests/oval-office-large-normal.jpg">
+<img src="https://raw.githubusercontent.com/brycedrennan/imaginairy-normal-map/6b3b1692cbdc21d55c84a01e0b7875df030b6d79/tests/oval-office-large.jpg" width=45% ><img src="https://raw.githubusercontent.com/brycedrennan/imaginairy-normal-map/6b3b1692cbdc21d55c84a01e0b7875df030b6d79/tests/oval-office-large-normal.jpg" width=45%>
 
 **Quick Start**
 ```bash
 pip install imaginairy-normal-map
 ```
 
 ```python
```

## Comparing `imaginairy_normal_map-0.0.2.dist-info/RECORD` & `imaginairy_normal_map-0.0.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 imaginairy_normal_map/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 imaginairy_normal_map/decoder.py,sha256=5Xbxv4z-qL31o8V53u_GgR0NIm0cRkBIJMYrfKJLrfU,5984
 imaginairy_normal_map/encoder.py,sha256=FIA175nJO7yzljh0SLOT4kpWAIxYPuXm0JqBUMxUtwQ,1041
 imaginairy_normal_map/model.py,sha256=DI-g0jjtZRvDlL_ci3lquiRQl7fNsPa2I6plpa_yuQY,3007
 imaginairy_normal_map/submodules.py,sha256=1HFwl-e9NZq6SzSRlk_zR6Nv8ZmYRDI-4tIgsD4qRew,1241
 imaginairy_normal_map/utils.py,sha256=2yNgfwKrcfQtdKfmwj3lXuuBcEjQz0SMwA8OeO93MK0,277
-imaginairy_normal_map-0.0.2.dist-info/LICENSE,sha256=5Jf22CHDXJOkpG0ObItqDG7hGbLXwkutL1Gt3gGzWc0,1102
-imaginairy_normal_map-0.0.2.dist-info/METADATA,sha256=9c7QhlVCEAvPFJvTyLaHmlpuOpctob06oren8wMGbWg,1918
-imaginairy_normal_map-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-imaginairy_normal_map-0.0.2.dist-info/top_level.txt,sha256=yKhlpj9jdvS5qufRP3Y8AUQJn3tiB4FIfZzQ0PtIqMw,22
-imaginairy_normal_map-0.0.2.dist-info/RECORD,,
+imaginairy_normal_map-0.0.3.dist-info/LICENSE,sha256=5Jf22CHDXJOkpG0ObItqDG7hGbLXwkutL1Gt3gGzWc0,1102
+imaginairy_normal_map-0.0.3.dist-info/METADATA,sha256=bGs-7qzFv7fcobW5r6VMspp_mwO3NLBQ0Pj7pOZDTUc,2139
+imaginairy_normal_map-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+imaginairy_normal_map-0.0.3.dist-info/top_level.txt,sha256=yKhlpj9jdvS5qufRP3Y8AUQJn3tiB4FIfZzQ0PtIqMw,22
+imaginairy_normal_map-0.0.3.dist-info/RECORD,,
```

