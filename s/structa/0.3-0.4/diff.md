# Comparing `tmp/structa-0.3.tar.gz` & `tmp/structa-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structa-0.3.tar", last modified: Wed Oct 27 23:57:00 2021, max compression
+gzip compressed data, was "structa-0.4.tar", last modified: Thu May  4 07:32:18 2023, max compression
```

## Comparing `structa-0.3.tar` & `structa-0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-10-27 23:57:00.237020 structa-0.3/
--rw-rw-r--   0 dave      (1000) dave      (1000)    18135 2021-08-17 00:17:29.000000 structa-0.3/LICENSE.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       39 2021-04-24 00:51:18.000000 structa-0.3/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     6526 2021-10-27 23:57:00.237020 structa-0.3/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     5444 2021-08-17 00:17:29.000000 structa-0.3/README.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1928 2021-10-27 23:57:00.237020 structa-0.3/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2021-08-17 00:17:29.000000 structa-0.3/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-10-27 23:57:00.233020 structa-0.3/structa/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-08-16 23:45:18.000000 structa-0.3/structa/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    28141 2021-10-27 21:28:55.000000 structa-0.3/structa/analyzer.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8104 2021-10-27 23:45:19.000000 structa-0.3/structa/chars.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3340 2021-10-27 21:28:55.000000 structa-0.3/structa/collections.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5434 2021-10-27 21:28:55.000000 structa-0.3/structa/conversions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      315 2021-10-27 21:28:55.000000 structa-0.3/structa/errors.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4581 2021-10-27 21:28:55.000000 structa-0.3/structa/format.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     9999 2021-10-27 21:28:55.000000 structa-0.3/structa/source.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    56608 2021-10-27 21:51:12.000000 structa-0.3/structa/types.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-10-27 23:57:00.237020 structa-0.3/structa/ui/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-08-16 23:45:18.000000 structa-0.3/structa/ui/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    14989 2021-10-27 23:46:40.000000 structa-0.3/structa/ui/cli.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    10453 2021-08-15 20:44:04.000000 structa-0.3/structa/ui/cli.xsl
--rw-rw-r--   0 dave      (1000) dave      (1000)     6260 2021-10-27 23:43:48.000000 structa-0.3/structa/xml.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2021-10-27 23:57:00.233020 structa-0.3/structa.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     6526 2021-10-27 23:57:00.000000 structa-0.3/structa.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      490 2021-10-27 23:57:00.000000 structa-0.3/structa.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2021-10-27 23:57:00.000000 structa-0.3/structa.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       49 2021-10-27 23:57:00.000000 structa-0.3/structa.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      132 2021-10-27 23:57:00.000000 structa-0.3/structa.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2021-10-27 23:57:00.000000 structa-0.3/structa.egg-info/top_level.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 07:32:18.908853 structa-0.4/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    18135 2021-11-03 10:16:17.000000 structa-0.4/LICENSE.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       39 2020-10-03 23:55:45.000000 structa-0.4/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7074 2023-05-04 07:32:18.908853 structa-0.4/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5818 2022-05-22 15:23:54.000000 structa-0.4/README.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2089 2023-05-04 07:32:18.912853 structa-0.4/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2021-11-03 10:16:17.000000 structa-0.4/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 07:32:18.900853 structa-0.4/structa/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2020-10-03 23:55:45.000000 structa-0.4/structa/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    29877 2023-05-03 22:49:46.000000 structa-0.4/structa/analyzer.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8104 2023-05-03 16:47:08.000000 structa-0.4/structa/chars.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3340 2023-05-03 16:47:08.000000 structa-0.4/structa/collections.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6179 2023-05-03 22:49:46.000000 structa-0.4/structa/conversions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      315 2023-05-03 16:47:08.000000 structa-0.4/structa/errors.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5372 2023-05-03 22:47:33.000000 structa-0.4/structa/format.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9999 2023-05-03 16:47:08.000000 structa-0.4/structa/source.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    57863 2023-05-03 22:49:46.000000 structa-0.4/structa/types.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 07:32:18.908853 structa-0.4/structa/ui/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-08-16 16:29:29.000000 structa-0.4/structa/ui/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    17314 2023-05-03 22:47:33.000000 structa-0.4/structa/ui/cli.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10453 2021-08-16 16:29:29.000000 structa-0.4/structa/ui/cli.xsl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6260 2023-05-03 16:47:08.000000 structa-0.4/structa/xml.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-04 07:32:18.904853 structa-0.4/structa.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7074 2023-05-04 07:32:17.000000 structa-0.4/structa.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      490 2023-05-04 07:32:18.000000 structa-0.4/structa.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-04 07:32:17.000000 structa-0.4/structa.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       48 2023-05-04 07:32:18.000000 structa-0.4/structa.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      132 2023-05-04 07:32:18.000000 structa-0.4/structa.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-05-04 07:32:18.000000 structa-0.4/structa.egg-info/top_level.txt
```

### Comparing `structa-0.3/LICENSE.txt` & `structa-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `structa-0.3/PKG-INFO` & `structa-0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: structa
-Version: 0.3
+Version: 0.4
 Summary: Analyzes data files for common structures
-Home-page: UNKNOWN
 Author: Dave Jones
 Author-email: dave@waveform.org.uk
 License: UNKNOWN
 Project-URL: Documentation, https://structa.readthedocs.io/
 Project-URL: Source Code, https://github.com/waveform80/structa
 Project-URL: Issue Tracker, https://github.com/waveform80/structa/issues
 Keywords: json yaml csv data analysis
@@ -18,26 +17,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.5
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: yaml
 License-File: LICENSE.txt
 
 =======
 structa
 =======
 
-structa is a small utility for analyzing repeating structures in large data
-sources. Typically this is something like a document oriented database in JSON
-format, or a CSV file of a database dump, or a YAML document.
+structa is a small, semi-magical utility for discerning the "overall structure"
+of large data files. Typically this is something like a document oriented
+database in JSON format, or a CSV file of a database dump, or a YAML document.
 
 
 Usage
 =====
 
 Use from the command line::
 
@@ -66,41 +69,47 @@
                 'craft': str range="ISS".."Tiangong",
                 'name': str range="Akihiko Hoshide".."Thomas Pesquet"
             }
         ]
     }
 
 
-The `Python Package Index`_ (PyPI) provides a JSON API for packages::
-
-    curl -s https://pypi.org/pypi/numpy/json | structa
+The `Python Package Index`_ (PyPI) provides a JSON API for packages. You can
+feed the JSON of several packages to ``structa`` to get an idea of the overall
+structure of these records (when structa is given multiple inputs on the same
+invocation, it assumes all have a common source)::
+
+    for pkg in numpy scipy pandas matplotlib structa; do
+        curl -s https://pypi.org/pypi/$pkg/json > $pkg.json
+    done
+    structa numpy.json scipy.json pandas.json matplotlib.json structa.json
 
 Output::
 
     {
         'info': { str: value },
-        'last_serial': int range=9.0M,
+        'last_serial': int range=11.9M..13.1M,
         'releases': {
-            str range="0.9.6".."1.9.3": [
+            str range="0.1".."3.5.1": [
                 {
                     'comment_text': str,
                     'digests': {
                         'md5': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
                         'sha256': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
                     },
                     'downloads': int range=-1,
                     'filename': str,
                     'has_sig': bool,
                     'md5_digest': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
                     'packagetype': str range="bdist_wheel".."sdist",
-                    'python_version': str range="2.5".."source",
+                    'python_version': str range="2.4".."source",
                     'requires_python': value,
-                    'size': int range=1.9M..24.5M,
-                    'upload_time': str of timestamp range=2006-12-02 02:07:43..2020-12-25 03:30:00 pattern=%Y-%m-%dT%H:%M:%S,
-                    'upload_time_iso_8601': str of timestamp range=2009-04-06 06:19:25..2020-12-25 03:30:00 pattern=%Y-%m-%dT%H:%M:%S.%f%z,
+                    'size': int range=39.3K..118.4M,
+                    'upload_time': str of timestamp range=2006-01-09 14:02:01..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S",
+                    'upload_time_iso_8601': str of timestamp range=2009-04-06 06:19:25..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S.%f%z",
                     'url': URL,
                     'yanked': bool,
                     'yanked_reason': value
                 }
             ]
         },
         'urls': [
@@ -110,27 +119,29 @@
                     'md5': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
                     'sha256': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
                 },
                 'downloads': int range=-1,
                 'filename': str,
                 'has_sig': bool,
                 'md5_digest': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
-                'packagetype': str range="bdist_wheel" pattern="bdist_wheel",
-                'python_version': str range="cp36".."pp36" pattern="Ip3d",
-                'requires_python': str range="&gt;=3.6" pattern="&gt;=3.6",
-                'size': int range=7.3M..15.4M,
-                'upload_time': str of timestamp range=2020-11-02 15:46:22..2020-11-02 16:18:20 pattern=%Y-%m-%dT%H:%M:%S,
-                'upload_time_iso_8601': str of timestamp range=2020-11-02 15:46:22..2020-11-02 16:18:20 pattern=%Y-%m-%dT%H:%M:%S.%f%z,
+                'packagetype': str range="bdist_wheel".."sdist",
+                'python_version': str range="cp310".."source",
+                'requires_python': value,
+                'size': int range=47.2K..55.6M,
+                'upload_time': str of timestamp range=2021-10-27 23:57:01..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S",
+                'upload_time_iso_8601': str of timestamp range=2021-10-27 23:57:01..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S.%f%z",
                 'url': URL,
                 'yanked': bool,
                 'yanked_reason': value
             }
-        ]
+        ],
+        'vulnerabilities': [ empty ]
     }
 
+
 The `Ubuntu Security Notices`_ database contains the list of all security
 issues in releases of Ubuntu (warning, this one takes some time to analyze and
 eats about a gigabyte of RAM while doing so)::
 
     curl -s https://usn.ubuntu.com/usn-db/database.json | structa
 
 Output::
```

### Comparing `structa-0.3/README.rst` & `structa-0.4/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 =======
 structa
 =======
 
-structa is a small utility for analyzing repeating structures in large data
-sources. Typically this is something like a document oriented database in JSON
-format, or a CSV file of a database dump, or a YAML document.
+structa is a small, semi-magical utility for discerning the "overall structure"
+of large data files. Typically this is something like a document oriented
+database in JSON format, or a CSV file of a database dump, or a YAML document.
 
 
 Usage
 =====
 
 Use from the command line::
 
@@ -37,41 +37,47 @@
                 'craft': str range="ISS".."Tiangong",
                 'name': str range="Akihiko Hoshide".."Thomas Pesquet"
             }
         ]
     }
 
 
-The `Python Package Index`_ (PyPI) provides a JSON API for packages::
-
-    curl -s https://pypi.org/pypi/numpy/json | structa
+The `Python Package Index`_ (PyPI) provides a JSON API for packages. You can
+feed the JSON of several packages to ``structa`` to get an idea of the overall
+structure of these records (when structa is given multiple inputs on the same
+invocation, it assumes all have a common source)::
+
+    for pkg in numpy scipy pandas matplotlib structa; do
+        curl -s https://pypi.org/pypi/$pkg/json > $pkg.json
+    done
+    structa numpy.json scipy.json pandas.json matplotlib.json structa.json
 
 Output::
 
     {
         'info': { str: value },
-        'last_serial': int range=9.0M,
+        'last_serial': int range=11.9M..13.1M,
         'releases': {
-            str range="0.9.6".."1.9.3": [
+            str range="0.1".."3.5.1": [
                 {
                     'comment_text': str,
                     'digests': {
                         'md5': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
                         'sha256': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
                     },
                     'downloads': int range=-1,
                     'filename': str,
                     'has_sig': bool,
                     'md5_digest': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
                     'packagetype': str range="bdist_wheel".."sdist",
-                    'python_version': str range="2.5".."source",
+                    'python_version': str range="2.4".."source",
                     'requires_python': value,
-                    'size': int range=1.9M..24.5M,
-                    'upload_time': str of timestamp range=2006-12-02 02:07:43..2020-12-25 03:30:00 pattern=%Y-%m-%dT%H:%M:%S,
-                    'upload_time_iso_8601': str of timestamp range=2009-04-06 06:19:25..2020-12-25 03:30:00 pattern=%Y-%m-%dT%H:%M:%S.%f%z,
+                    'size': int range=39.3K..118.4M,
+                    'upload_time': str of timestamp range=2006-01-09 14:02:01..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S",
+                    'upload_time_iso_8601': str of timestamp range=2009-04-06 06:19:25..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S.%f%z",
                     'url': URL,
                     'yanked': bool,
                     'yanked_reason': value
                 }
             ]
         },
         'urls': [
@@ -81,27 +87,29 @@
                     'md5': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
                     'sha256': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
                 },
                 'downloads': int range=-1,
                 'filename': str,
                 'has_sig': bool,
                 'md5_digest': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
-                'packagetype': str range="bdist_wheel" pattern="bdist_wheel",
-                'python_version': str range="cp36".."pp36" pattern="Ip3d",
-                'requires_python': str range="&gt;=3.6" pattern="&gt;=3.6",
-                'size': int range=7.3M..15.4M,
-                'upload_time': str of timestamp range=2020-11-02 15:46:22..2020-11-02 16:18:20 pattern=%Y-%m-%dT%H:%M:%S,
-                'upload_time_iso_8601': str of timestamp range=2020-11-02 15:46:22..2020-11-02 16:18:20 pattern=%Y-%m-%dT%H:%M:%S.%f%z,
+                'packagetype': str range="bdist_wheel".."sdist",
+                'python_version': str range="cp310".."source",
+                'requires_python': value,
+                'size': int range=47.2K..55.6M,
+                'upload_time': str of timestamp range=2021-10-27 23:57:01..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S",
+                'upload_time_iso_8601': str of timestamp range=2021-10-27 23:57:01..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S.%f%z",
                 'url': URL,
                 'yanked': bool,
                 'yanked_reason': value
             }
-        ]
+        ],
+        'vulnerabilities': [ empty ]
     }
 
+
 The `Ubuntu Security Notices`_ database contains the list of all security
 issues in releases of Ubuntu (warning, this one takes some time to analyze and
 eats about a gigabyte of RAM while doing so)::
 
     curl -s https://usn.ubuntu.com/usn-db/database.json | structa
 
 Output::
```

### Comparing `structa-0.3/setup.cfg` & `structa-0.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = structa
-version = 0.3
+version = 0.4
 description = Analyzes data files for common structures
 long_description = file: README.rst
 author = Dave Jones
 author_email = dave@waveform.org.uk
 project_urls = 
 	Documentation = https://structa.readthedocs.io/
 	Source Code = https://github.com/waveform80/structa
@@ -18,17 +18,21 @@
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
+python_requires = >=3.5
 install_requires = 
 	setuptools
 	lxml
 	chardet
 	blessings
 	tqdm
 	python-dateutil
```

### Comparing `structa-0.3/structa/analyzer.py` & `structa-0.4/structa/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # structa: an application for analyzing repetitive data structures
 #
-# Copyright (c) 2018-2021 Dave Jones <dave@waveform.org.uk>
+# Copyright (c) 2018-2023 Dave Jones <dave@waveform.org.uk>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import warnings
 from math import ceil
 from datetime import datetime, timedelta
 from fractions import Fraction
@@ -124,14 +124,19 @@
 
     :param numbers.Rational empty_threshold:
         The proportion of strings within a field (across repetitive structures)
         which can be blank without affecting the type match. Empty strings
         falling within this threshold will be discounted by the analysis. Valid
         values are between 0 and 1.
 
+    :param numbers.Rational null_threshold:
+        The proportion of values within a field (across repetitive structures)
+        which can be None (null in JSON parlance) without affecting the type
+        match. Valid values are between 0 and 1.
+
     :param int field_threshold:
         The minimum number of fields in a mapping before it will be treated as
         a "table" (a mapping of keys to records) rather than a record (a
         mapping of fields to values). Valid values are any positive integer.
 
     :param numbers.Rational merge_threshold:
         The proportion of fields within repetitive mappings that must match for
@@ -149,38 +154,60 @@
         values potentially represent epoch-based datetime values.
 
     :type max_timestamp: datetime.datetime or None
     :param max_timestamp:
         The maximum timestamp to use when determining whether floating point
         values potentially represent epoch-based datetime values.
 
+    :type epoch: datetime.datetime or None
+    :param epoch:
+        The epoch to use when converting numbers to datetime values. Defaults
+        to the UNIX epoch (1st January, 1970).
+
+    :type epoch_unit: datetime.timedelta or None
+    :param epoch_unit:
+        The unit of time used in numeric representations of datetime values.
+        Defaults to 1 second.
+
     :type progress: object or None
     :param progress:
         If specificed, must be an object with ``update`` and ``reset`` methods
         that will be called to provide progress feedback. See :attr:`progress`
         for further details.
     """
     def __init__(self, *, bad_threshold=Fraction(2, 100),
-                 empty_threshold=Fraction(98, 100), field_threshold=20,
+                 empty_threshold=Fraction(98, 100),
+                 null_threshold=Fraction(98, 100), field_threshold=20,
                  merge_threshold=Fraction(50, 100), max_numeric_len=30,
-                 strip_whitespace=False, min_timestamp=None,
-                 max_timestamp=None, progress=None):
+                 strip_whitespace=False,
+                 min_timestamp=None, max_timestamp=None,
+                 epoch=datetime.utcfromtimestamp(0),
+                 epoch_unit=timedelta(seconds=1),
+                 progress=None):
         self.bad_threshold = bad_threshold
         self.empty_threshold = empty_threshold
+        self.null_threshold = null_threshold
         self.field_threshold = field_threshold
         self.merge_threshold = merge_threshold
         self.max_numeric_len = max_numeric_len
         self.strip_whitespace = strip_whitespace
+        unix_epoch = datetime.utcfromtimestamp(0)
+        self.timestamp_offset = (epoch - unix_epoch).total_seconds()
+        self.timestamp_scale = epoch_unit.total_seconds()
         now = datetime.now()
         if min_timestamp is None:
             min_timestamp = now - relativedelta(years=20)
         if max_timestamp is None:
             max_timestamp = now + relativedelta(years=10)
-        self.min_timestamp = min_timestamp.timestamp()
-        self.max_timestamp = max_timestamp.timestamp()
+        self.min_timestamp = (
+            min_timestamp.timestamp() - self.timestamp_offset
+        ) / self.timestamp_scale
+        self.max_timestamp = (
+            max_timestamp.timestamp() - self.timestamp_offset
+        ) / self.timestamp_scale
         self._progress = progress
 
     @property
     def progress(self):
         """
         The object passed as the *progress* parameter on construction.
 
@@ -581,14 +608,21 @@
                         )
                     elif all(isinstance(item, tuple) for item in items):
                         # Deferred return from the special case above; this is
                         # where we've a pure sample of tuples as the keys of a
                         # dict but there're more than the field threshold
                         return Tuple(items)
 
+                # Ignore null (None) up to the null threshold; in the case
+                # the threshold is exceeded we assume there's not enough data
+                # to even determine the type
+                if None in sample:
+                    if sample[None] / len(items) > self.null_threshold:
+                        return Value(items)
+                    del sample[None]
                 # The following ordering is important; note that bool's domain
                 # is a subset of int's
                 if all(isinstance(value, bool) for value in sample):
                     return Bool(sample)
                 elif all(isinstance(value, int) for value in sample):
                     return self._match_possible_datetime(Int(sample))
                 elif all(isinstance(value, (int, float)) for value in sample):
@@ -714,21 +748,23 @@
         return the original *pattern*.
         """
         in_range = lambda n: self.min_timestamp <= n <= self.max_timestamp
         if (
                 isinstance(pattern, (Int, Float)) and
                 in_range(pattern.values.min) and
                 in_range(pattern.values.max)):
-            return DateTime.from_numbers(pattern)
+            return DateTime.from_numbers(pattern, offset=self.timestamp_offset,
+                                         scale=self.timestamp_scale)
         elif (
                 isinstance(pattern, StrRepr) and (
                     (
                         isinstance(pattern.content, Int) and
                         pattern.pattern == 'd'
                     ) or
                     isinstance(pattern.content, Float)
                 ) and
                 in_range(pattern.content.values.min) and
                 in_range(pattern.content.values.max)):
-            return DateTime.from_numbers(pattern)
+            return DateTime.from_numbers(pattern, offset=self.timestamp_offset,
+                                         scale=self.timestamp_scale)
         else:
             return pattern
```

### Comparing `structa-0.3/structa/chars.py` & `structa-0.4/structa/chars.py`

 * *Files identical despite different names*

### Comparing `structa-0.3/structa/collections.py` & `structa-0.4/structa/collections.py`

 * *Files identical despite different names*

### Comparing `structa-0.3/structa/conversions.py` & `structa-0.4/structa/conversions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # structa: an application for analyzing repetitive data structures
 #
-# Copyright (c) 2020-2021 Dave Jones <dave@waveform.org.uk>
+# Copyright (c) 2020-2023 Dave Jones <dave@waveform.org.uk>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import re
+from datetime import timedelta
 
 from dateutil.parser import parse
 from dateutil.relativedelta import relativedelta
 
 from .collections import Counter, FrozenCounter
 
 
@@ -64,99 +65,115 @@
             false: False,
             true:  True,
         }[s.strip().lower()]
     except KeyError:
         raise ValueError('not a valid bool {!r}'.format(s))
 
 
-_SUFFIXES = [
-    # This ordering is important; the minutes regex must be checked *before*
-    # the months regex as one is a legitimate subset of the other
-    ('microseconds', 'm(icro)?s(ec(ond)?s?)?'),
-    ('seconds',      's(ec(ond)?s?)?'),
-    ('minutes',      'mi(n(ute)?s?)?'),
-    ('hours',        'h((ou)?rs?)?'),
-    ('days',         'd(ays?)?'),
-    ('weeks',        'w((ee)?ks?)?'),
-    ('months',       'm(on(th)?s?)?'),
-    ('years',        'y((ea)?rs?)?'),
-]
-_SPANS = [
-    (span, re.compile(r'^(?:(?P<num>[+-]?\d+)\s*{}\b)'.format(suffix)))
-    for span, suffix in _SUFFIXES
-]
-
-
-def parse_duration(s):
-    """
-    Convert the string *s* to a :class:`~dateutil.relativedelta.relativedelta`.
-    The string must consist of white-space and/or comma separated values which
-    are a number followed by a suffix indicating duration. For example:
+_SPANS = {
+    span: re.compile(r'(?:(?P<num>[+-]?\d+)\s*{}\b)'.format(suffix))
+    for span, suffix in [
+        ('microseconds', '(micro|u|µ)s(ec(ond)?s?)?'),
+        ('milliseconds', '(milli|m)s(ec(ond)?s?)?'),
+        ('seconds',      's(ec(ond)?s?)?'),
+        ('minutes',      'mi(n(ute)?s?)?'),
+        ('hours',        'h((ou)?rs?)?'),
+        ('days',         'd(ays?)?'),
+        ('weeks',        'w((ee)?ks?)?'),
+        ('months',       'm((on)?ths?)?'),
+        ('years',        'y((ea)?rs?)?'),
+    ]
+}
+
+
+def parse_duration(s, delta_type=relativedelta):
+    """
+    Convert the string *s* to a :class:`~dateutil.relativedelta.relativedelta`
+    (by default) or a :class:`~datetime.timedelta` if requested by
+    *delta_type*. The string must consist of white-space and/or comma separated
+    values which are a number followed by a suffix indicating duration. For
+    example:
 
         >>> parse_duration('1s')
         relativedelta(seconds=+1)
         >>> parse_duration('5 minutes, 30 seconds')
         relativedelta(minutes=+5, seconds=+30)
         >>> parse_duration('1 year')
         relativedelta(years=+1)
+        >>> parse_duration('1 week, 1 day', delta_type=datetime.timedelta)
+        timedelta(days=8)
 
     Note that some suffixes like "m" can be ambiguous; using common
     abbreviations should avoid ambiguity:
 
         >>> parse_duration('1 m')
         relativedelta(months=+1)
         >>> parse_duration('1 min')
         relativedelta(minutes=+1)
-        >>> parse_duration('1 mon')
+        >>> parse_duration('1 mth')
         relativedelta(months=+1)
 
     The set of possible durations, and their recognized suffixes is as follows:
 
     * *Microseconds*: microseconds, microsecond, microsec, micros, micro,
+      useconds, usecond, usecs, usec, us, µseconds, µsecond, µsecs, µsec, µs
+
+    * *Milliseconds*: milliseconds, millisecond, millisec, millis, milli,
       mseconds, msecond, msecs, msec, ms
 
     * *Seconds*: seconds, second, secs, sec, s
 
     * *Minutes*: minutes, minute, mins, min, mi
 
     * *Hours*: hours, hour, hrs, hr, h
 
     * *Days*: days, day, d
 
     * *Weeks*: weeks, week, wks, wk, w
 
-    * *Months*: months, month, mons, mon, mths, mth, m
+    * *Months*: months, month, mons, mon, mths, mth, m (relativedelta only)
 
-    * *Years*: years, year, yrs, yr, y
+    * *Years*: years, year, yrs, yr, y (relativedelta only)
 
     If conversion fails, :exc:`ValueError` is raised.
     """
-    spans = {span: 0 for span, regex in _SPANS}
+    assert delta_type in (relativedelta, timedelta)
+    spans = {}
     t = s
-    while True:
-        t = t.lstrip(' \t\n,')
-        if not t:
-            return relativedelta(**spans)
-        for span, regex in _SPANS:
-            m = regex.search(t)
-            if m:
-                spans[span] += int(m.group('num'))
-                # XXX This only truncates from the start; that in turn means
-                # that things must be ordered year/month/day/hour/etc. Make
-                # the algorithm order agnostic
-                t = t[len(m.group(0)):]
+    for span, regex in _SPANS.items():
+        if delta_type is timedelta and span in ('months', 'years'):
+            continue
+        m = regex.search(t)
+        if m:
+            spans[span] = spans.get(span, 0) + int(m.group('num'))
+            t = (t[:m.start(0)] + t[m.end(0):]).strip(' \t\n,')
+            if not t:
                 break
-        else:
-            raise ValueError('invalid duration {}'.format(s))
+    if t:
+        raise ValueError('invalid duration {}'.format(s))
+    if delta_type is relativedelta:
+        spans['microseconds'] = (
+            spans.get('microseconds', 0) +
+            (spans.pop('milliseconds', 0) * 1000))
+    return delta_type(**spans)
+
+
+def parse_timestamp(s):
+    """
+    Convert the string *s* to a :class:`~datetime.datetime`. A
+    :exc:`ValueError` is raised if *s* is not a valid datetime representation.
+    """
+    return parse(s)
 
 
-def parse_duration_or_timestamp(s):
+def parse_duration_or_timestamp(s, delta_type=relativedelta):
     """
     Convert the string *s* to a :class:`~datetime.datetime` or a
-    :class:`~dateutil.relativedelta.relativedelta`. Duration conversion is
-    attempted to and, if this fails, date-time conversion is attempted. A
-    :exc:`ValueError` is raised if both conversions fail.
+    :class:`~dateutil.relativedelta.relativedelta` (or
+    :class:`~datetime.timedelta` if *duration_type* so specifies). Duration
+    conversion is attempted to and, if this fails, date-time conversion is
+    attempted. A :exc:`ValueError` is raised if both conversions fail.
     """
     try:
-        return parse_duration(s)
+        return parse_duration(s, delta_type=delta_type)
     except ValueError:
-        return parse(s)
+        return parse_timestamp(s)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `structa-0.3/structa/format.py` & `structa-0.4/structa/format.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # structa: an application for analyzing repetitive data structures
 #
-# Copyright (c) 2020-2021 Dave Jones <dave@waveform.org.uk>
+# Copyright (c) 2020-2023 Dave Jones <dave@waveform.org.uk>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 from math import log
 from itertools import tee
-from datetime import datetime
+from datetime import datetime, timedelta
 
 
 def pairwise(iterable):
     """
     Taken from the recipe in the documentation for :mod:`itertools`.
     """
     a, b = tee(iterable)
@@ -149,7 +149,33 @@
             int:        lambda: format_int(value),
             bool:       lambda: ('false', 'true')[value],
             str:        lambda: '"{}"'.format(value.replace('"', '""')),
             type(None): lambda: 'null',
         }[type(value)]()
     except KeyError:
         raise ValueError('invalid type for value {!r}'.format(value))
+
+
+def format_timestamp_numrepr(offset, scale):
+    delta = timedelta(seconds=scale)
+    simple = {
+        timedelta(**{name: 1}): name
+        for name in (
+            'microseconds',
+            'milliseconds',
+            'seconds',
+            'minutes',
+            'hours',
+            'days',
+            'weeks',
+        )
+    }
+    if offset % 86400:
+        epoch = datetime.utcfromtimestamp(offset).isoformat()
+    else:
+        epoch = datetime.utcfromtimestamp(offset).date().isoformat()
+    try:
+        return '{unit} since {epoch}'.format(unit=simple[delta], epoch=epoch)
+    except KeyError:
+        return 'seconds since {epoch} {op} {scale:g}'.format(
+            epoch=epoch, op=('*', '/')[scale >= 1],
+            scale=scale if scale >= 1 else (1 / scale))
```

### Comparing `structa-0.3/structa/source.py` & `structa-0.4/structa/source.py`

 * *Files identical despite different names*

### Comparing `structa-0.3/structa/types.py` & `structa-0.4/structa/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # structa: an application for analyzing repetitive data structures
 #
-# Copyright (c) 2018-2021 Dave Jones <dave@waveform.org.uk>
+# Copyright (c) 2018-2023 Dave Jones <dave@waveform.org.uk>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import math
 from copy import copy
 from numbers import Real
 from datetime import datetime
 from textwrap import indent, shorten
 from functools import partial, total_ordering
 from collections.abc import Mapping
 from operator import attrgetter
 
 from .collections import Counter, FrozenCounter
 from .conversions import try_conversion, parse_bool
-from .format import format_int, format_repr, format_sample
 from .xml import ElementFactory, xml, merge_siblings
+from .format import (
+    format_int,
+    format_repr,
+    format_sample,
+    format_timestamp_numrepr,
+)
 
 
 tag = ElementFactory()
 
 
 class Stats:
     """
@@ -901,34 +906,40 @@
         """
         conv = lambda s: datetime.strptime(s, pattern)
         return StrRepr(
             cls(try_conversion(iterable, conv, bad_threshold)),
             pattern=pattern)
 
     @classmethod
-    def from_numbers(cls, pattern):
+    def from_numbers(cls, pattern, offset=0, scale=1):
         """
         Class method for constructing an instance wrapped in a :class:`NumRepr`
         to indicate a numeric representation of a set of timestamps (e.g. day
-        offset from the UNIX epoch).
+        offset from the UNIX epoch). A different epoch may be specified as a
+        numeric *offset*, and a different epoch *scale* as a numeric number of
+        seconds). The default offset and scale are 0 and 1 which is equivalent
+        to a seconds offset from the UNIX epoch (i.e. a traditional UNIX
+        timestamp).
 
         Constructed with an *sample* of number, a *pattern* (which can be a
         :class:`StrRepr` instance if the numbers are themselves represented as
         strings, otherwise must be the :class:`Int` or :class:`Float` instance
         representing the numbers), and a *bad_threshold* of values which are
         permitted to fail conversion.
         """
         if isinstance(pattern, StrRepr):
             num_pattern = pattern.content
         else:
             num_pattern = pattern
         dt_counter = Counter()
         for value, count in num_pattern.values.sample.items():
-            dt_counter[datetime.fromtimestamp(value)] = count
-        result = NumRepr(cls(dt_counter), pattern=num_pattern.__class__)
+            dt_value = datetime.utcfromtimestamp((value * scale) + offset)
+            dt_counter[dt_value] = count
+        result = NumRepr(cls(dt_counter), pattern=(
+            num_pattern.__class__, scale, offset))
         if isinstance(pattern, StrRepr):
             return pattern.with_content(result)
         else:
             return result
 
     def __str__(self):
         return 'datetime range={min}..{max}'.format(
@@ -1170,20 +1181,20 @@
         if not isinstance(value, str):
             raise TypeError('{value!r} is not a str'.format(value=value))
         if isinstance(self.content, Bool):
             false, true = self.pattern.split('|', 1)
             value = parse_bool(value, false, true)
         elif isinstance(self.content, Int) or (
             isinstance(self.content, NumRepr) and
-            self.content.pattern is Int
+            self.content.pattern[0] is Int
         ):
             value = int(value, base=self.int_bases[self.pattern])
         elif isinstance(self.content, Float) or (
             isinstance(self.content, NumRepr) and
-            self.content.pattern is Float
+            self.content.pattern[0] is Float
         ):
             assert self.pattern == 'f'
             value = float(value)
         elif isinstance(self.content, DateTime):
             value = datetime.strptime(value, self.pattern)
         else:
             assert False, (
@@ -1195,44 +1206,60 @@
     """
     A numeric representation of an inner type. Typically used to wrap
     :class:`DateTime`. Descends from :class:`Repr`.
     """
     __slots__ = ()
 
     def __str__(self):
-        if self.pattern is Int:
-            template = 'int of {self.content}'
-        elif self.pattern is Float:
-            template = 'float of {self.content}'
-        else:
+        type_, scale, offset = self.pattern
+        try:
+            type_name = {Int: 'int', Float: 'float'}[type_]
+        except KeyError:
             assert False, 'str(num-repr) of {self.content!r}'.format(self=self)
-        return template.format(self=self)
+        return '{type_name} {numrepr} of {self.content}'.format(
+            self=self, type_name=type_name,
+            numrepr=format_timestamp_numrepr(offset, scale))
 
     def __xml__(self):
-        if self.pattern is Int:
-            return tag.intof(xml(self.content))
-        elif self.pattern is Float:
-            return tag.floatof(xml(self.content))
+        type_, scale, offset = self.pattern
+        if type_ is Int:
+            return tag.intof(xml(self.content), scale=scale, offset=offset)
+        elif type_ is Float:
+            return tag.floatof(xml(self.content), scale=scale, offset=offset)
         else:
             assert False, 'xml(num-repr) of {self.content!r}'.format(self=self)
 
     def __add__(self, other):
         if self == other:
-            if self.pattern is Float or other.pattern is Float:
-                pattern = Float
+            self_type, self_scale, self_offset = self.pattern
+            other_type, other_scale, other_offset = other.pattern
+            if self_type is Float or other_type is Float:
+                add_type = Float
             else:
-                pattern = Int
-            return NumRepr(self.content + other.content, pattern)
+                add_type = Int
+            return NumRepr(
+                self.content + other.content,
+                (add_type, self_scale, self_offset))
         return NotImplemented
 
+    def __eq__(self, other):
+        if not isinstance(other, NumRepr):
+            return NotImplemented
+        if super().__eq__(other) is not True:
+            return False
+        self_type, self_scale, self_offset = self.pattern
+        other_type, other_scale, other_offset = other.pattern
+        return (self_scale == other_scale) and (self_offset == other_offset)
+
     def validate(self, value):
         if not isinstance(value, Real):
             raise TypeError('{value!r} is not a number'.format(value=value))
         if isinstance(self.content, DateTime):
-            value = datetime.fromtimestamp(value)
+            type_, scale, offset = self.pattern
+            value = datetime.utcfromtimestamp((value * scale) + offset)
         else:
             assert False, (
                 'validating num-repr of {self.content!r}'.format(self=self))
         self.content.validate(value)
 
 
 class URL(Str):
```

### Comparing `structa-0.3/structa/ui/cli.py` & `structa-0.4/structa/ui/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 # structa: an application for analyzing repetitive data structures
 #
-# Copyright (c) 2020-2021 Dave Jones <dave@waveform.org.uk>
+# Copyright (c) 2020-2023 Dave Jones <dave@waveform.org.uk>
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 
 import os
+import re
 import sys
 import argparse
 import warnings
-from datetime import datetime
 from fractions import Fraction
+from datetime import datetime, timedelta
 
 from blessings import Terminal
 from tqdm import tqdm
 from pkg_resources import require
 
 from ..analyzer import Analyzer
 from ..errors import ValidationWarning
-from ..conversions import parse_duration_or_timestamp
 from ..types import sources_list, SourcesList
 from ..source import Source
 from ..xml import xml, get_transform
+from ..conversions import (
+    parse_duration,
+    parse_duration_or_timestamp,
+    parse_timestamp,
+)
+
+try:
+    import argcomplete
+except ImportError:
+    argcomplete = None
 
 
 def main(args=None):
     warnings.simplefilter('ignore', category=ValidationWarning)
     try:
         config = get_config(args)
         structure = get_structure(config)
@@ -100,14 +110,18 @@
         'proportion of "bad" data permitted in a field (default: %(default)s)')
     parser.add_argument(
         '-E', '--empty-threshold', type=num, metavar='NUM', default='99%',
         help="The proportion of string values permitted to be empty without "
         "preventing the pattern from being reported; the proportion of "
         '"empty" data permitted in a field (default: %(default)s)')
     parser.add_argument(
+        '-N', '--null-threshold', type=num, metavar='NUM', default='99%',
+        help="The proportion of values permitted to be null without "
+        "preventing type analysis (default: %(default)s)")
+    parser.add_argument(
         '--str-limit', type=num, metavar='NUM', default=20,
         help="The length beyond which only the lengths of strs will be "
         "reported; below this the actual value of the string will be "
         "displayed (default: %(default)s)")
     parser.add_argument(
         '--hide-count', action='store_false', dest='show_count',
         default=False)
@@ -159,14 +173,22 @@
         '--max-timestamp', type=max_timestamp, metavar='WHEN',
         default='10 years',
         help="The maximum timestamp to use when guessing whether floating "
         "point fields represent UNIX timestamps (default: %(default)s). Can "
         "be specified as an absolute timestamp (in ISO-8601 format) or a "
         "duration to be added to the current timestamp")
     parser.add_argument(
+        '--timestamps', type=timestamps, default='unix',
+        metavar='[UNIT since] EPOCH',
+        help="The units and epoch from which datetimes are measured. Can be "
+        "specified as a string in the form 'duration since timestamp' (for "
+        "example 'days since 1970-01-01' or 'seconds since 1900-01-01'), a "
+        "standalone timestamp (in ISO-8601 format), or one of the special "
+        'strings, "unix" or "excel" (default: %(default)s)')
+    parser.add_argument(
         '--max-numeric-len', type=int, metavar='LEN', default=30,
         help="The maximum number of characters that a number, integer or "
         "floating-point, may use in its representation within the file. "
         "Defaults to %(default)s")
     parser.add_argument(
         '--sample-bytes', type=size, metavar='SIZE', default='1m',
         help="The number of bytes to sample from the file for the purposes of "
@@ -200,14 +222,19 @@
     parser.add_argument(
         '--no-json-strict', action='store_false', dest='json_strict',
         help="Controls whether the JSON decoder permits control characters "
         "within strings, which isn't technically valid JSON. The default is "
         "to be strict and disallow such characters")
 
     parser.set_defaults(sample=b'', csv_dialect=None)
+    if int(os.environ.get('_ARGCOMPLETE', '0')):
+        if argcomplete:
+            argcomplete.autocomplete(parser)
+        else:
+            raise RuntimeError('missing argcomplete')
     return parser.parse_args(args)
 
 
 def get_structure(config):
     bar_format='{desc} {percentage:4.1f}%  {elapsed} [{bar}] {remaining}'
     with tqdm(config.file, leave=False, bar_format=bar_format, maxinterval=1) as progress:
         data = sources_list()
@@ -286,20 +313,23 @@
 
 class MyAnalyzer(Analyzer):
     @classmethod
     def from_config(cls, config, progress):
         return cls(
             bad_threshold=config.bad_threshold,
             empty_threshold=config.empty_threshold,
+            null_threshold=config.null_threshold,
             field_threshold=config.field_threshold,
             merge_threshold=config.merge_threshold,
             max_numeric_len=config.max_numeric_len,
             strip_whitespace=config.strip_whitespace,
             min_timestamp=config.min_timestamp,
             max_timestamp=config.max_timestamp,
+            epoch=config.timestamps[1],
+            epoch_unit=config.timestamps[0],
             progress=progress)
 
 
 class MySource(Source):
     @classmethod
     def from_config(cls, config, file):
         return cls(
@@ -328,14 +358,38 @@
 def max_timestamp(s, now=_start):
     t = parse_duration_or_timestamp(s)
     if isinstance(t, datetime):
         return t
     else:
         return now + t
 
+def timestamps(s):
+    try:
+        return {
+            # The Excel epoch is defined as 1900-01-01, but that is date "1"
+            # in Excel, rather than "0". Furthermore, for compat. with good
+            # ol' 1-2-3, 1900 was treated (incorrectly) as a leap-year leading
+            # to a +1 offset for all dates after 1900-02-28. Rather than
+            # emulate all that nonsense, we just use 1899-12-30 as the epoch
+            # which is good enough for all detection purposes (which is all
+            # structa cares about anyway)
+            'excel': (timedelta(days=1), datetime(1899, 12, 30)),
+            'unix':  (timedelta(seconds=1), datetime.utcfromtimestamp(0)),
+        }[s]
+    except KeyError:
+        fmt_re = re.compile(r'((?P<unit>\D+) since )?(?P<epoch>[^ ]+)')
+        m = fmt_re.match(s)
+        if not m:
+            raise ValueError('invalid timestamp representation {s}'.format(s=s))
+        if m.group('unit') is None:
+            unit = timedelta(seconds=1)
+        else:
+            unit = parse_duration('1' + m.group('unit'), delta_type=timedelta)
+        return unit, parse_timestamp(m.group('epoch'))
+
 def num(s):
     if s.endswith('%'):
         return Fraction(num(s[:-1]), 100)
     elif '/' in s:
         return Fraction(s)
     elif '.' in s or 'e' in s:
         return float(s)
```

### Comparing `structa-0.3/structa/ui/cli.xsl` & `structa-0.4/structa/ui/cli.xsl`

 * *Files identical despite different names*

### Comparing `structa-0.3/structa/xml.py` & `structa-0.4/structa/xml.py`

 * *Files identical despite different names*

### Comparing `structa-0.3/structa.egg-info/PKG-INFO` & `structa-0.4/structa.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: structa
-Version: 0.3
+Version: 0.4
 Summary: Analyzes data files for common structures
-Home-page: UNKNOWN
 Author: Dave Jones
 Author-email: dave@waveform.org.uk
 License: UNKNOWN
 Project-URL: Documentation, https://structa.readthedocs.io/
 Project-URL: Source Code, https://github.com/waveform80/structa
 Project-URL: Issue Tracker, https://github.com/waveform80/structa/issues
 Keywords: json yaml csv data analysis
@@ -18,26 +17,30 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.5
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: yaml
 License-File: LICENSE.txt
 
 =======
 structa
 =======
 
-structa is a small utility for analyzing repeating structures in large data
-sources. Typically this is something like a document oriented database in JSON
-format, or a CSV file of a database dump, or a YAML document.
+structa is a small, semi-magical utility for discerning the "overall structure"
+of large data files. Typically this is something like a document oriented
+database in JSON format, or a CSV file of a database dump, or a YAML document.
 
 
 Usage
 =====
 
 Use from the command line::
 
@@ -66,41 +69,47 @@
                 'craft': str range="ISS".."Tiangong",
                 'name': str range="Akihiko Hoshide".."Thomas Pesquet"
             }
         ]
     }
 
 
-The `Python Package Index`_ (PyPI) provides a JSON API for packages::
-
-    curl -s https://pypi.org/pypi/numpy/json | structa
+The `Python Package Index`_ (PyPI) provides a JSON API for packages. You can
+feed the JSON of several packages to ``structa`` to get an idea of the overall
+structure of these records (when structa is given multiple inputs on the same
+invocation, it assumes all have a common source)::
+
+    for pkg in numpy scipy pandas matplotlib structa; do
+        curl -s https://pypi.org/pypi/$pkg/json > $pkg.json
+    done
+    structa numpy.json scipy.json pandas.json matplotlib.json structa.json
 
 Output::
 
     {
         'info': { str: value },
-        'last_serial': int range=9.0M,
+        'last_serial': int range=11.9M..13.1M,
         'releases': {
-            str range="0.9.6".."1.9.3": [
+            str range="0.1".."3.5.1": [
                 {
                     'comment_text': str,
                     'digests': {
                         'md5': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
                         'sha256': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
                     },
                     'downloads': int range=-1,
                     'filename': str,
                     'has_sig': bool,
                     'md5_digest': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
                     'packagetype': str range="bdist_wheel".."sdist",
-                    'python_version': str range="2.5".."source",
+                    'python_version': str range="2.4".."source",
                     'requires_python': value,
-                    'size': int range=1.9M..24.5M,
-                    'upload_time': str of timestamp range=2006-12-02 02:07:43..2020-12-25 03:30:00 pattern=%Y-%m-%dT%H:%M:%S,
-                    'upload_time_iso_8601': str of timestamp range=2009-04-06 06:19:25..2020-12-25 03:30:00 pattern=%Y-%m-%dT%H:%M:%S.%f%z,
+                    'size': int range=39.3K..118.4M,
+                    'upload_time': str of timestamp range=2006-01-09 14:02:01..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S",
+                    'upload_time_iso_8601': str of timestamp range=2009-04-06 06:19:25..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S.%f%z",
                     'url': URL,
                     'yanked': bool,
                     'yanked_reason': value
                 }
             ]
         },
         'urls': [
@@ -110,27 +119,29 @@
                     'md5': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
                     'sha256': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
                 },
                 'downloads': int range=-1,
                 'filename': str,
                 'has_sig': bool,
                 'md5_digest': str pattern="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
-                'packagetype': str range="bdist_wheel" pattern="bdist_wheel",
-                'python_version': str range="cp36".."pp36" pattern="Ip3d",
-                'requires_python': str range="&gt;=3.6" pattern="&gt;=3.6",
-                'size': int range=7.3M..15.4M,
-                'upload_time': str of timestamp range=2020-11-02 15:46:22..2020-11-02 16:18:20 pattern=%Y-%m-%dT%H:%M:%S,
-                'upload_time_iso_8601': str of timestamp range=2020-11-02 15:46:22..2020-11-02 16:18:20 pattern=%Y-%m-%dT%H:%M:%S.%f%z,
+                'packagetype': str range="bdist_wheel".."sdist",
+                'python_version': str range="cp310".."source",
+                'requires_python': value,
+                'size': int range=47.2K..55.6M,
+                'upload_time': str of timestamp range=2021-10-27 23:57:01..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S",
+                'upload_time_iso_8601': str of timestamp range=2021-10-27 23:57:01..2022-03-10 16:45:20 pattern="%Y-%m-%dT%H:%M:%S.%f%z",
                 'url': URL,
                 'yanked': bool,
                 'yanked_reason': value
             }
-        ]
+        ],
+        'vulnerabilities': [ empty ]
     }
 
+
 The `Ubuntu Security Notices`_ database contains the list of all security
 issues in releases of Ubuntu (warning, this one takes some time to analyze and
 eats about a gigabyte of RAM while doing so)::
 
     curl -s https://usn.ubuntu.com/usn-db/database.json | structa
 
 Output::
```

