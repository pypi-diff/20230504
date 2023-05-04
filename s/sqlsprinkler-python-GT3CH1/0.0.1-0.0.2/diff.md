# Comparing `tmp/sqlsprinkler-python-GT3CH1-0.0.1.tar.gz` & `tmp/sqlsprinkler-python-GT3CH1-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsprinkler-python-GT3CH1-0.0.1.tar", last modified: Thu May  4 14:41:39 2023, max compression
+gzip compressed data, was "sqlsprinkler-python-GT3CH1-0.0.2.tar", last modified: Thu May  4 15:09:57 2023, max compression
```

## Comparing `sqlsprinkler-python-GT3CH1-0.0.1.tar` & `sqlsprinkler-python-GT3CH1-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2023-05-04 14:41:39.254459 sqlsprinkler-python-GT3CH1-0.0.1/
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     1068 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.1/LICENSE
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      830 2023-05-04 14:41:39.254524 sqlsprinkler-python-GT3CH1-0.0.1/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      324 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.1/README.md
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)       84 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.1/pyproject.toml
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      641 2023-05-04 14:41:39.259857 sqlsprinkler-python-GT3CH1-0.0.1/setup.cfg
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)       68 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.1/setup.py
-drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2023-05-04 14:41:39.247318 sqlsprinkler-python-GT3CH1-0.0.1/src/
-drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2023-05-04 14:41:39.251325 sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler/
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler/__init__.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler/system.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler/zone.py
-drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2023-05-04 14:41:39.254143 sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler_python_GT3CH1.egg-info/
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      830 2023-05-04 14:41:39.000000 sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      348 2023-05-04 14:41:39.000000 sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler_python_GT3CH1.egg-info/SOURCES.txt
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        1 2023-05-04 14:41:39.000000 sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler_python_GT3CH1.egg-info/dependency_links.txt
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)       13 2023-05-04 14:41:39.000000 sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler_python_GT3CH1.egg-info/top_level.txt
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:09:57.715071 sqlsprinkler-python-GT3CH1-0.0.2/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     1068 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.2/LICENSE
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 15:09:57.715141 sqlsprinkler-python-GT3CH1-0.0.2/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      324 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.2/README.md
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       84 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.2/pyproject.toml
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      641 2023-05-04 15:09:57.722363 sqlsprinkler-python-GT3CH1-0.0.2/setup.cfg
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       68 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.2/setup.py
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:09:57.702692 sqlsprinkler-python-GT3CH1-0.0.2/src/
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:09:57.709378 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      107 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/__init__.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      222 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/api.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     5282 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/system.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     1975 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler/zone.py
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 15:09:57.714325 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 15:09:57.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      372 2023-05-04 15:09:57.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/SOURCES.txt
+-rw-r--r--   0 gcpease  (1709703766) 1389146880        1 2023-05-04 15:09:57.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/dependency_links.txt
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       13 2023-05-04 15:09:57.000000 sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/top_level.txt
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.1/LICENSE` & `sqlsprinkler-python-GT3CH1-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlsprinkler-python-GT3CH1-0.0.1/PKG-INFO` & `sqlsprinkler-python-GT3CH1-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.1/setup.cfg` & `sqlsprinkler-python-GT3CH1-0.0.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlsprinkler-python-GT3CH1
-version = 0.0.1
+version = 0.0.2
 author = Gavin Pease
 author_email = gavinpease@gmail.com
 description = A python library to control a SQLSprinkler system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GT3CH1/sqlsprinkler_python
 project_urls =
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.1/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO` & `sqlsprinkler-python-GT3CH1-0.0.2/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

