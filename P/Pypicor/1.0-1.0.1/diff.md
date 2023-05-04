# Comparing `tmp/pypicor-1.0-py3.11.egg` & `tmp/Pypicor-1.0.1-py3.11.egg`

## zipinfo {}

```diff
@@ -1,13 +1,19 @@
-Zip file size: 4702 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      268 b- defN 23-May-04 13:54 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      190 b- defN 23-May-04 13:54 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-04 13:54 EGG-INFO/dependency_links.txt
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-04 13:54 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-04 13:54 EGG-INFO/zip-safe
+Zip file size: 8654 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat      270 b- defN 23-May-04 14:03 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      314 b- defN 23-May-04 14:03 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-04 14:03 EGG-INFO/dependency_links.txt
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-04 14:03 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-04 14:03 EGG-INFO/zip-safe
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-04 13:36 build/lib/pypicor/__init__.py
+-rw-rw-rw-  2.0 fat     2206 b- defN 23-May-04 10:51 build/lib/pypicor/baq.py
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-03 12:05 build/lib/pypicor/credentials.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-May-04 14:03 build/lib/pypicor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-  2.0 fat     3156 b- defN 23-May-04 14:03 build/lib/pypicor/__pycache__/baq.cpython-311.pyc
+-rw-rw-rw-  2.0 fat      274 b- defN 23-May-04 14:03 build/lib/pypicor/__pycache__/credentials.cpython-311.pyc
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-04 13:36 pypicor/__init__.py
 -rw-rw-rw-  2.0 fat     2206 b- defN 23-May-04 10:51 pypicor/baq.py
 -rw-rw-rw-  2.0 fat      110 b- defN 23-May-03 12:05 pypicor/credentials.py
--rw-rw-rw-  2.0 fat      154 b- defN 23-May-04 13:54 pypicor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-  2.0 fat     3146 b- defN 23-May-04 13:54 pypicor/__pycache__/baq.cpython-311.pyc
--rw-rw-rw-  2.0 fat      264 b- defN 23-May-04 13:54 pypicor/__pycache__/credentials.cpython-311.pyc
-11 files, 6349 bytes uncompressed, 3264 bytes compressed:  48.6%
+-rw-rw-rw-  2.0 fat      154 b- defN 23-May-04 14:03 pypicor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-  2.0 fat     3146 b- defN 23-May-04 14:03 pypicor/__pycache__/baq.cpython-311.pyc
+-rw-rw-rw-  2.0 fat      264 b- defN 23-May-04 14:03 pypicor/__pycache__/credentials.cpython-311.pyc
+17 files, 12396 bytes uncompressed, 6270 bytes compressed:  49.4%
```

## zipnote «TEMP»/diffoscope_1hrps6rp_/tmp2c9tly56_.zip

```diff
@@ -9,14 +9,32 @@
 
 Filename: EGG-INFO/top_level.txt
 Comment: 
 
 Filename: EGG-INFO/zip-safe
 Comment: 
 
+Filename: build/lib/pypicor/__init__.py
+Comment: 
+
+Filename: build/lib/pypicor/baq.py
+Comment: 
+
+Filename: build/lib/pypicor/credentials.py
+Comment: 
+
+Filename: build/lib/pypicor/__pycache__/__init__.cpython-311.pyc
+Comment: 
+
+Filename: build/lib/pypicor/__pycache__/baq.cpython-311.pyc
+Comment: 
+
+Filename: build/lib/pypicor/__pycache__/credentials.cpython-311.pyc
+Comment: 
+
 Filename: pypicor/__init__.py
 Comment: 
 
 Filename: pypicor/baq.py
 Comment: 
 
 Filename: pypicor/credentials.py
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,7 +1,7 @@
 Metadata-Version: 2.1
-Name: pypicor
-Version: 1.0
+Name: Pypicor
+Version: 1.0.1
 Summary: Python package with helpful things to use the Epicor API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,8 +1,12 @@
 setup.py
+Pypicor.egg-info/PKG-INFO
+Pypicor.egg-info/SOURCES.txt
+Pypicor.egg-info/dependency_links.txt
+Pypicor.egg-info/top_level.txt
 pypicor/__init__.py
 pypicor/baq.py
 pypicor/credentials.py
 pypicor.egg-info/PKG-INFO
 pypicor.egg-info/SOURCES.txt
 pypicor.egg-info/dependency_links.txt
 pypicor.egg-info/top_level.txt
```

## EGG-INFO/top_level.txt

```diff
@@ -1 +1,3 @@
+build
+dist
 pypicor
```

