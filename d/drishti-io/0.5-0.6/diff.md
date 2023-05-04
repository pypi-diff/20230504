# Comparing `tmp/drishti-io-0.5.tar.gz` & `tmp/drishti-io-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drishti-io-0.5.tar", last modified: Wed Feb  8 23:39:56 2023, max compression
+gzip compressed data, was "drishti-io-0.6.tar", last modified: Thu May  4 17:58:17 2023, max compression
```

## Comparing `drishti-io-0.5.tar` & `drishti-io-0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jlbez      (501) staff       (20)        0 2023-02-08 23:39:56.715035 drishti-io-0.5/
--rw-r--r--   0 jlbez      (501) staff       (20)     2426 2022-09-12 16:41:34.000000 drishti-io-0.5/LICENSE
--rw-r--r--   0 jlbez      (501) staff       (20)       52 2022-10-10 21:37:54.000000 drishti-io-0.5/MANIFEST.in
--rw-r--r--   0 jlbez      (501) staff       (20)     3944 2023-02-08 23:39:56.714581 drishti-io-0.5/PKG-INFO
--rw-r--r--   0 jlbez      (501) staff       (20)     3389 2023-02-08 23:06:51.000000 drishti-io-0.5/README.md
-drwxr-xr-x   0 jlbez      (501) staff       (20)        0 2023-02-08 23:39:56.694402 drishti-io-0.5/drishti/
--rw-r--r--   0 jlbez      (501) staff       (20)        0 2022-08-16 20:59:07.000000 drishti-io-0.5/drishti/__init__.py
--rw-r--r--   0 jlbez      (501) staff       (20)    69294 2023-02-08 23:06:53.000000 drishti-io-0.5/drishti/main.py
-drwxr-xr-x   0 jlbez      (501) staff       (20)        0 2023-02-08 23:39:56.709351 drishti-io-0.5/drishti/snippets/
--rw-r--r--   0 jlbez      (501) staff       (20)        0 2022-08-16 22:45:17.000000 drishti-io-0.5/drishti/snippets/__init__.py
--rw-r--r--   0 jlbez      (501) staff       (20)      114 2022-08-01 15:20:53.000000 drishti-io-0.5/drishti/snippets/hdf5-alignment.c
--rw-r--r--   0 jlbez      (501) staff       (20)      500 2022-08-02 16:45:01.000000 drishti-io-0.5/drishti/snippets/hdf5-cache.c
--rw-r--r--   0 jlbez      (501) staff       (20)      168 2022-08-01 15:20:53.000000 drishti-io-0.5/drishti/snippets/hdf5-collective-metadata.c
--rw-r--r--   0 jlbez      (501) staff       (20)      707 2022-08-02 16:41:53.000000 drishti-io-0.5/drishti/snippets/hdf5-vol-async-read.c
--rw-r--r--   0 jlbez      (501) staff       (20)      809 2022-08-02 16:41:55.000000 drishti-io-0.5/drishti/snippets/hdf5-vol-async-write.c
--rw-r--r--   0 jlbez      (501) staff       (20)      249 2022-08-01 15:20:53.000000 drishti-io-0.5/drishti/snippets/lustre-striping.bash
--rw-r--r--   0 jlbez      (501) staff       (20)      160 2022-08-02 16:44:51.000000 drishti-io-0.5/drishti/snippets/mpi-io-collective-read.c
--rw-r--r--   0 jlbez      (501) staff       (20)      162 2022-08-02 16:44:48.000000 drishti-io-0.5/drishti/snippets/mpi-io-collective-write.c
--rw-r--r--   0 jlbez      (501) staff       (20)     1168 2022-08-02 16:44:24.000000 drishti-io-0.5/drishti/snippets/mpi-io-hints.bash
--rw-r--r--   0 jlbez      (501) staff       (20)      339 2022-08-02 16:44:43.000000 drishti-io-0.5/drishti/snippets/mpi-io-iread.c
--rw-r--r--   0 jlbez      (501) staff       (20)      337 2022-08-02 16:44:40.000000 drishti-io-0.5/drishti/snippets/mpi-io-iwrite.c
--rw-r--r--   0 jlbez      (501) staff       (20)      355 2022-08-15 20:19:17.000000 drishti-io-0.5/drishti/snippets/pnetcdf-hdf5-no-fill.c
-drwxr-xr-x   0 jlbez      (501) staff       (20)        0 2023-02-08 23:39:56.713884 drishti-io-0.5/drishti_io.egg-info/
--rw-r--r--   0 jlbez      (501) staff       (20)     3944 2023-02-08 23:39:56.000000 drishti-io-0.5/drishti_io.egg-info/PKG-INFO
--rw-r--r--   0 jlbez      (501) staff       (20)      776 2023-02-08 23:39:56.000000 drishti-io-0.5/drishti_io.egg-info/SOURCES.txt
--rw-r--r--   0 jlbez      (501) staff       (20)        1 2023-02-08 23:39:56.000000 drishti-io-0.5/drishti_io.egg-info/dependency_links.txt
--rw-r--r--   0 jlbez      (501) staff       (20)       46 2023-02-08 23:39:56.000000 drishti-io-0.5/drishti_io.egg-info/entry_points.txt
--rw-r--r--   0 jlbez      (501) staff       (20)       37 2023-02-08 23:39:56.000000 drishti-io-0.5/drishti_io.egg-info/requires.txt
--rw-r--r--   0 jlbez      (501) staff       (20)        8 2023-02-08 23:39:56.000000 drishti-io-0.5/drishti_io.egg-info/top_level.txt
--rw-r--r--   0 jlbez      (501) staff       (20)       37 2022-10-13 16:19:50.000000 drishti-io-0.5/requirements.txt
--rw-r--r--   0 jlbez      (501) staff       (20)       38 2023-02-08 23:39:56.715199 drishti-io-0.5/setup.cfg
--rw-r--r--   0 jlbez      (501) staff       (20)     1189 2023-02-08 23:39:36.000000 drishti-io-0.5/setup.py
+drwxr-xr-x   0 jlbez      (501) staff       (20)        0 2023-05-04 17:58:17.087438 drishti-io-0.6/
+-rw-r--r--   0 jlbez      (501) staff       (20)     2426 2023-05-04 16:55:01.000000 drishti-io-0.6/LICENSE
+-rw-r--r--   0 jlbez      (501) staff       (20)       52 2023-05-04 16:55:01.000000 drishti-io-0.6/MANIFEST.in
+-rw-r--r--   0 jlbez      (501) staff       (20)     3944 2023-05-04 17:58:17.086848 drishti-io-0.6/PKG-INFO
+-rw-r--r--   0 jlbez      (501) staff       (20)     3389 2023-05-04 16:55:01.000000 drishti-io-0.6/README.md
+drwxr-xr-x   0 jlbez      (501) staff       (20)        0 2023-05-04 17:58:17.069244 drishti-io-0.6/drishti/
+-rw-r--r--   0 jlbez      (501) staff       (20)        0 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/__init__.py
+-rw-r--r--   0 jlbez      (501) staff       (20)    69982 2023-05-04 17:07:37.000000 drishti-io-0.6/drishti/main.py
+drwxr-xr-x   0 jlbez      (501) staff       (20)        0 2023-05-04 17:58:17.082023 drishti-io-0.6/drishti/snippets/
+-rw-r--r--   0 jlbez      (501) staff       (20)        0 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/__init__.py
+-rw-r--r--   0 jlbez      (501) staff       (20)      114 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/hdf5-alignment.c
+-rw-r--r--   0 jlbez      (501) staff       (20)      500 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/hdf5-cache.c
+-rw-r--r--   0 jlbez      (501) staff       (20)      168 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/hdf5-collective-metadata.c
+-rw-r--r--   0 jlbez      (501) staff       (20)      707 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/hdf5-vol-async-read.c
+-rw-r--r--   0 jlbez      (501) staff       (20)      809 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/hdf5-vol-async-write.c
+-rw-r--r--   0 jlbez      (501) staff       (20)      249 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/lustre-striping.bash
+-rw-r--r--   0 jlbez      (501) staff       (20)      160 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/mpi-io-collective-read.c
+-rw-r--r--   0 jlbez      (501) staff       (20)      162 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/mpi-io-collective-write.c
+-rw-r--r--   0 jlbez      (501) staff       (20)     1168 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/mpi-io-hints.bash
+-rw-r--r--   0 jlbez      (501) staff       (20)      339 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/mpi-io-iread.c
+-rw-r--r--   0 jlbez      (501) staff       (20)      337 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/mpi-io-iwrite.c
+-rw-r--r--   0 jlbez      (501) staff       (20)      355 2023-05-04 16:55:01.000000 drishti-io-0.6/drishti/snippets/pnetcdf-hdf5-no-fill.c
+drwxr-xr-x   0 jlbez      (501) staff       (20)        0 2023-05-04 17:58:17.085924 drishti-io-0.6/drishti_io.egg-info/
+-rw-r--r--   0 jlbez      (501) staff       (20)     3944 2023-05-04 17:58:17.000000 drishti-io-0.6/drishti_io.egg-info/PKG-INFO
+-rw-r--r--   0 jlbez      (501) staff       (20)      776 2023-05-04 17:58:17.000000 drishti-io-0.6/drishti_io.egg-info/SOURCES.txt
+-rw-r--r--   0 jlbez      (501) staff       (20)        1 2023-05-04 17:58:17.000000 drishti-io-0.6/drishti_io.egg-info/dependency_links.txt
+-rw-r--r--   0 jlbez      (501) staff       (20)       46 2023-05-04 17:58:17.000000 drishti-io-0.6/drishti_io.egg-info/entry_points.txt
+-rw-r--r--   0 jlbez      (501) staff       (20)       37 2023-05-04 17:58:17.000000 drishti-io-0.6/drishti_io.egg-info/requires.txt
+-rw-r--r--   0 jlbez      (501) staff       (20)        8 2023-05-04 17:58:17.000000 drishti-io-0.6/drishti_io.egg-info/top_level.txt
+-rw-r--r--   0 jlbez      (501) staff       (20)       37 2023-05-04 16:55:01.000000 drishti-io-0.6/requirements.txt
+-rw-r--r--   0 jlbez      (501) staff       (20)       38 2023-05-04 17:58:17.087611 drishti-io-0.6/setup.cfg
+-rw-r--r--   0 jlbez      (501) staff       (20)     1188 2023-05-04 17:58:04.000000 drishti-io-0.6/setup.py
```

### Comparing `drishti-io-0.5/LICENSE` & `drishti-io-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drishti-io-0.5/PKG-INFO` & `drishti-io-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drishti-io
-Version: 0.5
+Version: 0.6
 Home-page: https://github.com/hpc-io/drishti
 Author: Jean Luca Bez, Suren Byna
 Author-email: jlbez@lbl.gov, sbyna@lbl.gov
 Keywords: drishti
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `drishti-io-0.5/README.md` & `drishti-io-0.6/README.md`

 * *Files identical despite different names*

### Comparing `drishti-io-0.5/drishti/main.py` & `drishti-io-0.6/drishti/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import io
 import sys
 import csv
 import time
 import json
 import shlex
+import shutil
 import datetime
 import argparse
 import subprocess
 
 import pandas as pd
 
 import darshan
@@ -238,14 +239,20 @@
         double_bytes = bytes_number / 1024.0
         i = i + 1
         bytes_number = bytes_number / 1024
 
     return str(round(double_bytes, 2)) + ' ' + tags[i] 
 
 
+def is_available(name):
+    """Check whether `name` is on PATH and marked as executable."""
+
+    return shutil.which(name) is not None
+
+
 def message(code, target, level, issue, recommendations=None, details=None):
     """
     Display the message on the screen with level, issue, and recommendation.
     """
     icon = ':arrow_forward:'
 
     if level in (HIGH, WARN):
@@ -302,18 +309,34 @@
 
         insights_total[RECOMMENDATIONS] += len(recommendations)
 
     return Group(
         *messages
     )
 
+
 def check_log_version(file, log_version, library_version):
     use_file = file
 
     if version.parse(log_version) < version.parse('3.4.0'):
+        # Check if darshan-convert is installed and available in the PATH
+        if not is_available('darshan-convert'):
+            console.print(
+                Panel(
+                    Padding(
+                        'Darshan file is using an old format and darshan-convert is not available in the PATH.',
+                        (1, 1)
+                    ),
+                    title='{}WARNING'.format('[orange1]'),
+                    title_align='left'
+                )
+            )
+
+            sys.exit(os.EX_DATAERR)
+
         use_file = os.path.basename(file.replace('.darshan', '.converted.darshan'))
 
         console.print(
             Panel(
                 Padding(
                     'Converting .darshan log from {} to 3.4.0: format: saving output file "{}" in the current working directory.'.format(
                         log_version,
```

### Comparing `drishti-io-0.5/drishti/snippets/hdf5-vol-async-read.c` & `drishti-io-0.6/drishti/snippets/hdf5-vol-async-read.c`

 * *Files identical despite different names*

### Comparing `drishti-io-0.5/drishti/snippets/hdf5-vol-async-write.c` & `drishti-io-0.6/drishti/snippets/hdf5-vol-async-write.c`

 * *Files identical despite different names*

### Comparing `drishti-io-0.5/drishti/snippets/mpi-io-hints.bash` & `drishti-io-0.6/drishti/snippets/mpi-io-hints.bash`

 * *Files identical despite different names*

### Comparing `drishti-io-0.5/drishti_io.egg-info/PKG-INFO` & `drishti-io-0.6/drishti_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drishti-io
-Version: 0.5
+Version: 0.6
 Home-page: https://github.com/hpc-io/drishti
 Author: Jean Luca Bez, Suren Byna
 Author-email: jlbez@lbl.gov, sbyna@lbl.gov
 Keywords: drishti
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `drishti-io-0.5/drishti_io.egg-info/SOURCES.txt` & `drishti-io-0.6/drishti_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drishti-io-0.5/setup.py` & `drishti-io-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setuptools.setup(
     name="drishti-io",
     keywords="drishti",
-    version="0.5",
+    version="0.6",
     author="Jean Luca Bez, Suren Byna",
     author_email="jlbez@lbl.gov, sbyna@lbl.gov",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hpc-io/drishti",
     install_requires=[
         'argparse',
         'pandas',
         'darshan',
-        'rich ==12.5.1',
+        'rich==12.5.1',
     ],
     packages=[
         'drishti'
     ],
     package_data={
         'drishti': [
             'drishti/snippets/*'
```

