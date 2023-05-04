# Comparing `tmp/mo_files-6.375.23120-py2.py3-none-any.whl.zip` & `tmp/mo_files-6.384.23124-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15863 bytes, number of entries: 8
+Zip file size: 15860 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat    18788 b- defN 23-Apr-30 18:14 mo_files/__init__.py
 -rw-rw-rw-  2.0 fat      197 b- defN 22-Dec-05 22:50 mo_files/mimetype.py
 -rw-rw-rw-  2.0 fat    11814 b- defN 23-Apr-30 18:14 mo_files/url.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1603 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      649 b- defN 23-Apr-30 18:14 mo_files-6.375.23120.dist-info/RECORD
-8 files, 49895 bytes uncompressed, 14735 bytes compressed:  70.5%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-May-04 10:52 mo_files-6.384.23124.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-May-04 10:52 mo_files-6.384.23124.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-04 10:52 mo_files-6.384.23124.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-04 10:52 mo_files-6.384.23124.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      649 b- defN 23-May-04 10:52 mo_files-6.384.23124.dist-info/RECORD
+8 files, 49895 bytes uncompressed, 14732 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: mo_files/mimetype.py
 Comment: 
 
 Filename: mo_files/url.py
 Comment: 
 
-Filename: mo_files-6.375.23120.dist-info/LICENSE
+Filename: mo_files-6.384.23124.dist-info/LICENSE
 Comment: 
 
-Filename: mo_files-6.375.23120.dist-info/METADATA
+Filename: mo_files-6.384.23124.dist-info/METADATA
 Comment: 
 
-Filename: mo_files-6.375.23120.dist-info/WHEEL
+Filename: mo_files-6.384.23124.dist-info/WHEEL
 Comment: 
 
-Filename: mo_files-6.375.23120.dist-info/top_level.txt
+Filename: mo_files-6.384.23124.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_files-6.375.23120.dist-info/RECORD
+Filename: mo_files-6.384.23124.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mo_files-6.375.23120.dist-info/LICENSE` & `mo_files-6.384.23124.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_files-6.375.23120.dist-info/METADATA` & `mo_files-6.384.23124.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-files
-Version: 6.375.23120
+Version: 6.384.23124
 Summary: More Files! Steamlined for UTF8 and JSON.
 Home-page: https://github.com/klahnakoski/mo-files
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
@@ -12,19 +12,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots (==9.368.23092)
+Requires-Dist: mo-dots (==9.376.23121)
 Requires-Dist: mo-future (==7.340.23006)
-Requires-Dist: mo-json (==6.374.23120)
-Requires-Dist: mo-logs (==7.374.23120)
-Requires-Dist: mo-math (==7.368.23092)
+Requires-Dist: mo-json (==6.384.23124)
+Requires-Dist: mo-logs (==7.378.23124)
+Requires-Dist: mo-math (==7.378.23124)
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 
 # More Files!
 
 The `File` class makes the default assumption all files have cr-delimited unicode content that is UTF-8 encoded. This is great for JSON files. It also provides better operators over some common file manipulations.
```

## Comparing `mo_files-6.375.23120.dist-info/RECORD` & `mo_files-6.384.23124.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 mo_files/__init__.py,sha256=uRs0Mm7MvtvaWEdhfmoDl7kzqlWpNVEvGDJatYBfZmc,18788
 mo_files/mimetype.py,sha256=tXRCYszJ_FHg5-itrS28ZGbPnJ3KgrWAEaFKyPBEUYg,197
 mo_files/url.py,sha256=dUFjERY9SeZ2u5jB0zVyWPZGLPX9d9Wmt5fJbn9GGRA,11814
-mo_files-6.375.23120.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_files-6.375.23120.dist-info/METADATA,sha256=2Xk5Y04UTsMwTsY0VGmhrpgjPaEbr34mJdXCtixtXeA,1603
-mo_files-6.375.23120.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_files-6.375.23120.dist-info/top_level.txt,sha256=a9fidDIwv-DfFgyRS3H6__1vuNeUpplNr_0iLGosdBA,9
-mo_files-6.375.23120.dist-info/RECORD,,
+mo_files-6.384.23124.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_files-6.384.23124.dist-info/METADATA,sha256=ZD060wRfxdouFFAK9dFzfaaBuD2-phdBug4kkxuLz9Y,1603
+mo_files-6.384.23124.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_files-6.384.23124.dist-info/top_level.txt,sha256=a9fidDIwv-DfFgyRS3H6__1vuNeUpplNr_0iLGosdBA,9
+mo_files-6.384.23124.dist-info/RECORD,,
```

