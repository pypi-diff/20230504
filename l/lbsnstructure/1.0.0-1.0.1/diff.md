# Comparing `tmp/lbsnstructure-1.0.0.tar.gz` & `tmp/lbsnstructure-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbsnstructure-1.0.0.tar", last modified: Wed Apr 12 11:43:02 2023, max compression
+gzip compressed data, was "lbsnstructure-1.0.1.tar", last modified: Thu May  4 08:24:16 2023, max compression
```

## Comparing `lbsnstructure-1.0.0.tar` & `lbsnstructure-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:02.123729 lbsnstructure-1.0.0/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1227 2019-07-11 09:18:07.000000 lbsnstructure-1.0.0/.gitignore
--rwxrwxrwx   0 alex      (1000) alex      (1000)     1553 2020-02-28 07:54:54.000000 lbsnstructure-1.0.0/.gitlab-ci.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      409 2023-04-12 11:42:52.000000 lbsnstructure-1.0.0/CHANGELOG.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.0.0/LICENSE.md
--rw-r--r--   0 alex      (1000) alex      (1000)     2993 2023-04-12 11:43:02.124728 lbsnstructure-1.0.0/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)     2655 2019-10-21 11:34:47.000000 lbsnstructure-1.0.0/README.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)     4124 2019-07-11 09:18:07.000000 lbsnstructure-1.0.0/StructureTest.ipynb
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:01.943079 lbsnstructure-1.0.0/google/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:01.996643 lbsnstructure-1.0.0/google/protobuf/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     2754 2019-07-11 10:53:20.000000 lbsnstructure-1.0.0/google/protobuf/timestamp_pb2.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:02.103892 lbsnstructure-1.0.0/lbsnstructure/
--rw-rw-rw-   0 alex      (1000) alex      (1000)        0 2019-07-11 09:18:07.000000 lbsnstructure-1.0.0/lbsnstructure/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7923 2023-04-12 11:33:49.000000 lbsnstructure-1.0.0/lbsnstructure/interlinkage_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)    27308 2023-04-12 11:29:54.000000 lbsnstructure-1.0.0/lbsnstructure/social_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)    20143 2023-04-12 11:35:11.000000 lbsnstructure-1.0.0/lbsnstructure/spatial_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)    12612 2023-04-12 11:35:33.000000 lbsnstructure-1.0.0/lbsnstructure/temporal_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)    26683 2023-04-12 11:35:46.000000 lbsnstructure-1.0.0/lbsnstructure/topical_pb2.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)       22 2023-04-12 11:42:52.000000 lbsnstructure-1.0.0/lbsnstructure/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-12 11:43:02.121729 lbsnstructure-1.0.0/lbsnstructure.egg-info/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     2993 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/PKG-INFO
--rw-rw-rw-   0 alex      (1000) alex      (1000)      552 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/SOURCES.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/dependency_links.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2019-07-11 11:04:14.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/not-zip-safe
--rw-rw-rw-   0 alex      (1000) alex      (1000)        9 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/requires.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)       14 2023-04-12 11:42:59.000000 lbsnstructure-1.0.0/lbsnstructure.egg-info/top_level.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2023-04-12 11:43:02.126885 lbsnstructure-1.0.0/setup.cfg
--rw-rw-rw-   0 alex      (1000) alex      (1000)      909 2019-07-11 09:18:07.000000 lbsnstructure-1.0.0/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:24:16.567666 lbsnstructure-1.0.1/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1227 2019-07-11 09:18:07.000000 lbsnstructure-1.0.1/.gitignore
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     1553 2020-02-28 07:54:54.000000 lbsnstructure-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      588 2023-05-04 08:24:10.000000 lbsnstructure-1.0.1/CHANGELOG.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.0.1/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     2993 2023-05-04 08:24:16.567666 lbsnstructure-1.0.1/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     2655 2019-10-21 11:34:47.000000 lbsnstructure-1.0.1/README.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     4124 2019-07-11 09:18:07.000000 lbsnstructure-1.0.1/StructureTest.ipynb
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:24:16.442545 lbsnstructure-1.0.1/google/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:24:16.497971 lbsnstructure-1.0.1/google/protobuf/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1625 2023-05-04 08:22:28.000000 lbsnstructure-1.0.1/google/protobuf/duration_pb2.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1641 2023-05-04 08:22:28.000000 lbsnstructure-1.0.1/google/protobuf/timestamp_pb2.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:24:16.552227 lbsnstructure-1.0.1/lbsnstructure/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        0 2019-07-11 09:18:07.000000 lbsnstructure-1.0.1/lbsnstructure/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2703 2023-05-04 08:22:28.000000 lbsnstructure-1.0.1/lbsnstructure/interlinkage_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5527 2023-05-04 08:22:28.000000 lbsnstructure-1.0.1/lbsnstructure/social_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4172 2023-05-04 08:22:28.000000 lbsnstructure-1.0.1/lbsnstructure/spatial_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2693 2023-05-04 08:22:28.000000 lbsnstructure-1.0.1/lbsnstructure/temporal_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5006 2023-05-04 08:22:28.000000 lbsnstructure-1.0.1/lbsnstructure/topical_pb2.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       22 2023-05-04 08:24:10.000000 lbsnstructure-1.0.1/lbsnstructure/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 08:24:16.565161 lbsnstructure-1.0.1/lbsnstructure.egg-info/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     2993 2023-05-04 08:24:15.000000 lbsnstructure-1.0.1/lbsnstructure.egg-info/PKG-INFO
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      584 2023-05-04 08:24:15.000000 lbsnstructure-1.0.1/lbsnstructure.egg-info/SOURCES.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2023-05-04 08:24:15.000000 lbsnstructure-1.0.1/lbsnstructure.egg-info/dependency_links.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2019-07-11 11:04:14.000000 lbsnstructure-1.0.1/lbsnstructure.egg-info/not-zip-safe
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        9 2023-05-04 08:24:15.000000 lbsnstructure-1.0.1/lbsnstructure.egg-info/requires.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)       14 2023-05-04 08:24:15.000000 lbsnstructure-1.0.1/lbsnstructure.egg-info/top_level.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2023-05-04 08:24:16.571368 lbsnstructure-1.0.1/setup.cfg
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      909 2019-07-11 09:18:07.000000 lbsnstructure-1.0.1/setup.py
```

### Comparing `lbsnstructure-1.0.0/.gitignore` & `lbsnstructure-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.0/.gitlab-ci.yml` & `lbsnstructure-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.0/LICENSE.md` & `lbsnstructure-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.0/PKG-INFO` & `lbsnstructure-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.0.0
+Version: 1.0.1
 Summary: A common language independent and cross-network social-media data scheme.
 Home-page: https://gitlab.vgiscience.de/lbsn/concept
 Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
 Author-email: alexander.dunkel@tu-dresden.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `lbsnstructure-1.0.0/README.md` & `lbsnstructure-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.0/StructureTest.ipynb` & `lbsnstructure-1.0.1/StructureTest.ipynb`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.0/lbsnstructure.egg-info/PKG-INFO` & `lbsnstructure-1.0.1/lbsnstructure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.0.0
+Version: 1.0.1
 Summary: A common language independent and cross-network social-media data scheme.
 Home-page: https://gitlab.vgiscience.de/lbsn/concept
 Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
 Author-email: alexander.dunkel@tu-dresden.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `lbsnstructure-1.0.0/lbsnstructure.egg-info/SOURCES.txt` & `lbsnstructure-1.0.1/lbsnstructure.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .gitlab-ci.yml
 CHANGELOG.md
 LICENSE.md
 README.md
 StructureTest.ipynb
 setup.cfg
 setup.py
+google/protobuf/duration_pb2.py
 google/protobuf/timestamp_pb2.py
 lbsnstructure/__init__.py
 lbsnstructure/interlinkage_pb2.py
 lbsnstructure/social_pb2.py
 lbsnstructure/spatial_pb2.py
 lbsnstructure/temporal_pb2.py
 lbsnstructure/topical_pb2.py
```

### Comparing `lbsnstructure-1.0.0/setup.py` & `lbsnstructure-1.0.1/setup.py`

 * *Files identical despite different names*

