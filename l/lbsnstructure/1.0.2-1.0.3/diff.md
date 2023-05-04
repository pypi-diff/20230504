# Comparing `tmp/lbsnstructure-1.0.2.tar.gz` & `tmp/lbsnstructure-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbsnstructure-1.0.2.tar", last modified: Thu May  4 08:39:42 2023, max compression
+gzip compressed data, was "lbsnstructure-1.0.3.tar", last modified: Thu May  4 09:03:13 2023, max compression
```

## Comparing `lbsnstructure-1.0.2.tar` & `lbsnstructure-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:39:42.617323 lbsnstructure-1.0.2/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1227 2019-07-11 09:18:07.000000 lbsnstructure-1.0.2/.gitignore
--rwxrwxrwx   0 alex      (1000) alex      (1000)     1553 2020-02-28 07:54:54.000000 lbsnstructure-1.0.2/.gitlab-ci.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      758 2023-05-04 08:39:38.000000 lbsnstructure-1.0.2/CHANGELOG.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.0.2/LICENSE.md
--rw-r--r--   0 alex      (1000) alex      (1000)     2993 2023-05-04 08:39:42.617323 lbsnstructure-1.0.2/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)     2655 2019-10-21 11:34:47.000000 lbsnstructure-1.0.2/README.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)     4124 2019-07-11 09:18:07.000000 lbsnstructure-1.0.2/StructureTest.ipynb
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:39:42.430762 lbsnstructure-1.0.2/google/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:39:42.501469 lbsnstructure-1.0.2/google/protobuf/
--rw-r--r--   0 alex      (1000) alex      (1000)     1625 2023-05-04 08:22:28.000000 lbsnstructure-1.0.2/google/protobuf/duration_pb2.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1641 2023-05-04 08:22:28.000000 lbsnstructure-1.0.2/google/protobuf/timestamp_pb2.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:39:42.595450 lbsnstructure-1.0.2/lbsnstructure/
--rw-rw-rw-   0 alex      (1000) alex      (1000)      106 2023-05-04 08:38:19.000000 lbsnstructure-1.0.2/lbsnstructure/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2703 2023-05-04 08:22:28.000000 lbsnstructure-1.0.2/lbsnstructure/interlinkage_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5527 2023-05-04 08:22:28.000000 lbsnstructure-1.0.2/lbsnstructure/social_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4172 2023-05-04 08:22:28.000000 lbsnstructure-1.0.2/lbsnstructure/spatial_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2693 2023-05-04 08:22:28.000000 lbsnstructure-1.0.2/lbsnstructure/temporal_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5006 2023-05-04 08:22:28.000000 lbsnstructure-1.0.2/lbsnstructure/topical_pb2.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)       67 2023-05-04 08:39:38.000000 lbsnstructure-1.0.2/lbsnstructure/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:39:42.616027 lbsnstructure-1.0.2/lbsnstructure.egg-info/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     2993 2023-05-04 08:39:42.000000 lbsnstructure-1.0.2/lbsnstructure.egg-info/PKG-INFO
--rw-rw-rw-   0 alex      (1000) alex      (1000)      584 2023-05-04 08:39:42.000000 lbsnstructure-1.0.2/lbsnstructure.egg-info/SOURCES.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2023-05-04 08:39:42.000000 lbsnstructure-1.0.2/lbsnstructure.egg-info/dependency_links.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2019-07-11 11:04:14.000000 lbsnstructure-1.0.2/lbsnstructure.egg-info/not-zip-safe
--rw-rw-rw-   0 alex      (1000) alex      (1000)        9 2023-05-04 08:39:42.000000 lbsnstructure-1.0.2/lbsnstructure.egg-info/requires.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)       14 2023-05-04 08:39:42.000000 lbsnstructure-1.0.2/lbsnstructure.egg-info/top_level.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2023-05-04 08:39:42.617323 lbsnstructure-1.0.2/setup.cfg
--rw-rw-rw-   0 alex      (1000) alex      (1000)      909 2019-07-11 09:18:07.000000 lbsnstructure-1.0.2/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.703335 lbsnstructure-1.0.3/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1227 2019-07-11 09:18:07.000000 lbsnstructure-1.0.3/.gitignore
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     1553 2020-02-28 07:54:54.000000 lbsnstructure-1.0.3/.gitlab-ci.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      954 2023-05-04 09:03:09.000000 lbsnstructure-1.0.3/CHANGELOG.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.0.3/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     2993 2023-05-04 09:03:13.703335 lbsnstructure-1.0.3/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     2655 2019-10-21 11:34:47.000000 lbsnstructure-1.0.3/README.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     4124 2019-07-11 09:18:07.000000 lbsnstructure-1.0.3/StructureTest.ipynb
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.583050 lbsnstructure-1.0.3/google/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.617210 lbsnstructure-1.0.3/google/protobuf/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1625 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/google/protobuf/duration_pb2.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1641 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/google/protobuf/timestamp_pb2.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.689664 lbsnstructure-1.0.3/lbsnstructure/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      425 2023-05-04 09:00:50.000000 lbsnstructure-1.0.3/lbsnstructure/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2703 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/interlinkage_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5527 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/social_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4172 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/spatial_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2693 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/temporal_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5006 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/topical_pb2.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       67 2023-05-04 09:03:09.000000 lbsnstructure-1.0.3/lbsnstructure/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.700144 lbsnstructure-1.0.3/lbsnstructure.egg-info/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     2993 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/PKG-INFO
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      584 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/SOURCES.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/dependency_links.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2019-07-11 11:04:14.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/not-zip-safe
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        9 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/requires.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)       14 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/top_level.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2023-05-04 09:03:13.705952 lbsnstructure-1.0.3/setup.cfg
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      909 2019-07-11 09:18:07.000000 lbsnstructure-1.0.3/setup.py
```

### Comparing `lbsnstructure-1.0.2/.gitignore` & `lbsnstructure-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/.gitlab-ci.yml` & `lbsnstructure-1.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/CHANGELOG.md` & `lbsnstructure-1.0.3/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.3 (2023-05-04)
+### Fix
+* Make objects available in top-level namespace ([`9acb38b`](https://github.com/Sieboldianus/lbsnstructure-python/commit/9acb38b31544958daafc67ab358acd0e1cb1d4b1))
+
 ## v1.0.2 (2023-05-04)
 ### Fix
 * Version import path ([`4a11a9a`](https://github.com/Sieboldianus/lbsnstructure-python/commit/4a11a9a1a2bd498c8b2c9b2654752b1f6ffadb90))
 
 ## v1.0.1 (2023-05-04)
 ### Fix
 * Compile with protobuf 3.19.0 ([`be97942`](https://github.com/Sieboldianus/lbsnstructure-python/commit/be979426ca78963bc17d5309d4d5802b7f55e7bb))
```

### Comparing `lbsnstructure-1.0.2/LICENSE.md` & `lbsnstructure-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/PKG-INFO` & `lbsnstructure-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.0.2
+Version: 1.0.3
 Summary: A common language independent and cross-network social-media data scheme.
 Home-page: https://gitlab.vgiscience.de/lbsn/concept
 Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
 Author-email: alexander.dunkel@tu-dresden.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `lbsnstructure-1.0.2/README.md` & `lbsnstructure-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/StructureTest.ipynb` & `lbsnstructure-1.0.3/StructureTest.ipynb`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/google/protobuf/duration_pb2.py` & `lbsnstructure-1.0.3/google/protobuf/duration_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/google/protobuf/timestamp_pb2.py` & `lbsnstructure-1.0.3/google/protobuf/timestamp_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/lbsnstructure/interlinkage_pb2.py` & `lbsnstructure-1.0.3/lbsnstructure/interlinkage_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/lbsnstructure/social_pb2.py` & `lbsnstructure-1.0.3/lbsnstructure/social_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/lbsnstructure/spatial_pb2.py` & `lbsnstructure-1.0.3/lbsnstructure/spatial_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/lbsnstructure/temporal_pb2.py` & `lbsnstructure-1.0.3/lbsnstructure/temporal_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/lbsnstructure/topical_pb2.py` & `lbsnstructure-1.0.3/lbsnstructure/topical_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/lbsnstructure.egg-info/PKG-INFO` & `lbsnstructure-1.0.3/lbsnstructure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.0.2
+Version: 1.0.3
 Summary: A common language independent and cross-network social-media data scheme.
 Home-page: https://gitlab.vgiscience.de/lbsn/concept
 Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
 Author-email: alexander.dunkel@tu-dresden.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `lbsnstructure-1.0.2/lbsnstructure.egg-info/SOURCES.txt` & `lbsnstructure-1.0.3/lbsnstructure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.2/setup.py` & `lbsnstructure-1.0.3/setup.py`

 * *Files identical despite different names*

