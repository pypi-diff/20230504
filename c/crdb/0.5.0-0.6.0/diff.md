# Comparing `tmp/crdb-0.5.0.tar.gz` & `tmp/crdb-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crdb-0.5.0.tar", last modified: Sun Mar 12 16:46:37 2023, max compression
+gzip compressed data, was "crdb-0.6.0.tar", last modified: Thu May  4 19:31:48 2023, max compression
```

## Comparing `crdb-0.5.0.tar` & `crdb-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:46:37.671969 crdb-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-12 16:46:30.000000 crdb-0.5.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:46:37.667969 crdb-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:46:37.667969 crdb-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-12 16:46:30.000000 crdb-0.5.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-12 16:46:30.000000 crdb-0.5.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-12 16:46:30.000000 crdb-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-12 16:46:30.000000 crdb-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-12 16:46:30.000000 crdb-0.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-12 16:46:30.000000 crdb-0.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-12 16:46:30.000000 crdb-0.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-12 16:46:30.000000 crdb-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-12 16:46:30.000000 crdb-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-12 16:46:30.000000 crdb-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-03-12 16:46:37.671969 crdb-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-12 16:46:30.000000 crdb-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:46:37.667969 crdb-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-12 16:46:30.000000 crdb-0.5.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-12 16:46:30.000000 crdb-0.5.0/docs/build.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-12 16:46:30.000000 crdb-0.5.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-12 16:46:30.000000 crdb-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-12 16:46:30.000000 crdb-0.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-12 16:46:30.000000 crdb-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-12 16:46:30.000000 crdb-0.5.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-12 16:46:30.000000 crdb-0.5.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-12 16:46:30.000000 crdb-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-12 16:46:37.671969 crdb-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:46:37.667969 crdb-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:46:37.671969 crdb-0.5.0/src/crdb/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-12 16:46:30.000000 crdb-0.5.0/src/crdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-12 16:46:30.000000 crdb-0.5.0/src/crdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18459 2023-03-12 16:46:30.000000 crdb-0.5.0/src/crdb/_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-12 16:46:30.000000 crdb-0.5.0/src/crdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-03-12 16:46:30.000000 crdb-0.5.0/src/crdb/crdb_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-03-12 16:46:30.000000 crdb-0.5.0/src/crdb/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-12 16:46:30.000000 crdb-0.5.0/src/crdb/mpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-03-12 16:46:30.000000 crdb-0.5.0/src/crdb/solarsystem_abundances2003.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:46:37.671969 crdb-0.5.0/src/crdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-03-12 16:46:37.000000 crdb-0.5.0/src/crdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-12 16:46:37.000000 crdb-0.5.0/src/crdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 16:46:37.000000 crdb-0.5.0/src/crdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-12 16:46:37.000000 crdb-0.5.0/src/crdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-12 16:46:37.000000 crdb-0.5.0/src/crdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-12 16:46:37.000000 crdb-0.5.0/src/crdb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:46:37.671969 crdb-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-12 16:46:30.000000 crdb-0.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-12 16:46:30.000000 crdb-0.5.0/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-12 16:46:30.000000 crdb-0.5.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-12 16:46:30.000000 crdb-0.5.0/tests/test_mpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.391471 crdb-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-04 19:31:40.000000 crdb-0.6.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.387471 crdb-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.387471 crdb-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-04 19:31:40.000000 crdb-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 19:31:40.000000 crdb-0.6.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-04 19:31:40.000000 crdb-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 19:31:40.000000 crdb-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 19:31:40.000000 crdb-0.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-04 19:31:40.000000 crdb-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 19:31:40.000000 crdb-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-04 19:31:40.000000 crdb-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 19:31:40.000000 crdb-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-04 19:31:40.000000 crdb-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-04 19:31:48.391471 crdb-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-04 19:31:40.000000 crdb-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.387471 crdb-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-04 19:31:40.000000 crdb-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 19:31:48.391471 crdb-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.387471 crdb-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.391471 crdb-0.6.0/src/crdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/crdb_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/solarsystem_abundances2003.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.391471 crdb-0.6.0/src/crdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.391471 crdb-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 19:31:40.000000 crdb-0.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-04 19:31:40.000000 crdb-0.6.0/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 19:31:40.000000 crdb-0.6.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 19:31:40.000000 crdb-0.6.0/tests/test_mpl.py
```

### Comparing `crdb-0.5.0/.github/workflows/publish.yml` & `crdb-0.6.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/.github/workflows/test.yml` & `crdb-0.6.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/.gitignore` & `crdb-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/.pre-commit-config.yaml` & `crdb-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/CONTRIBUTING.rst` & `crdb-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/LICENSE` & `crdb-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/PKG-INFO` & `crdb-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.5.0
+Version: 0.6.0
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `crdb-0.5.0/README.rst` & `crdb-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/docs/conf.py` & `crdb-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/pyproject.toml` & `crdb-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,18 @@
     { email = "hans.dembinski@gmail.com" }
 ]
 readme = "README.rst"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
     # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: MIT License',
-    'Operating System :: Unix',
-    'Operating System :: POSIX',
-    'Operating System :: Microsoft :: Windows',
+    "Operating System :: OS Independent",
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
```

### Comparing `crdb-0.5.0/src/crdb/__init__.py` & `crdb-0.6.0/src/crdb/__init__.py`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/src/crdb/_lib.py` & `crdb-0.6.0/src/crdb/_lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import datetime
 import re
 import ssl
 import tempfile
 import urllib.request as rq
-import warnings
 from pathlib import Path
 from typing import Dict
 from typing import List
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
@@ -331,14 +330,15 @@
     "Ulysses",
     "Voyager",
 )
 
 
 def query(
     quantity: Union[str, Sequence[str]],
+    *,
     energy_type: str = "R",
     combo_level: int = 1,
     energy_convert_level: int = 1,
     flux_rescaling: float = 0.0,
     exp_dates: str = "",
     energy_start: float = 0.0,
     energy_stop: float = 0.0,
@@ -402,14 +402,17 @@
         expert option, users do not need to change this.
 
     Returns
     -------
 
     numpy record array with the database content
 
+    Energies are in GeV or GV. Solar modulation values are in MV. Distances are in
+    AU. Fluxes are in sr s m2 energy_unit.
+
     Raises
     ------
 
     ValueError
         An invalid parameter value triggers a ValueError.
 
     TimeoutError
@@ -455,26 +458,28 @@
         flux_rescaling=flux_rescaling,
         exp_dates=exp_dates,
         energy_start=energy_start,
         energy_stop=energy_stop,
         time_start=time_start,
         time_stop=time_stop,
         time_series=time_series,
-        format="",
+        format="csv",
         modulation=modulation,
         server_url=server_url,
     )
 
     data = _server_request(url, timeout)
 
     # check for errors and display them
     if len(data) == 1:
         raise ValueError(data[0])
 
-    return _convert(data)
+    table = _convert(data)
+
+    return table
 
 
 def _url(
     quantity: str,
     energy_type: str = "R",
     combo_level: int = 1,
     energy_convert_level: int = 1,
@@ -521,15 +526,15 @@
 
     if flux_rescaling < 0 or flux_rescaling > 2.5:
         raise ValueError(f"invalid flux_rescaling {flux_rescaling}")
 
     if time_series and time_series not in ("no", "only", "all"):
         raise ValueError(f"invalid time_series {time_series}")
 
-    if format and format not in ("usine", "galprop", "csv"):
+    if format and format not in ("usine", "galprop", "csv", "csv-asimport"):
         raise ValueError(f"invalid format {format}")
 
     if modulation and modulation not in ("USO05", "USO17", "GHE17"):
         raise ValueError(f"invalid modulation {modulation}")
 
     # do the query
     kwargs = {
@@ -587,52 +592,121 @@
         raise ValueError("empty server response")
 
     return data
 
 
 def _convert(data: List[str]) -> NDArray:
     # convert text to numpy record array
+
+    # Use this for csv-asimport or csv-extended when it becomes available
+    # fields set to None here are skipped during parsing
+    # fields = [
+    #     ("exp", "U64"),  # EXP-NAME
+    #     ("exp_type", "U16"),  # EXP-TYPE
+    #     None,  # EXP-HTML
+    #     None,  # EXP-STARTYEAR
+    #     ("sub_exp", "U100"),  # SUBEXP-NAME
+    #     None,  # SUBEXP-DESCRIPTION
+    #     ("e_relerr", "f8"),  # SUBEXP-ESCALE_RELERR
+    #     None,  # SUBEXP-INFO
+    #     ("distance", "f8"),  # SUBEXP-DISTANCE
+    #     ("datetime", "U64"),  # SUBEXP-DATES
+    #     ("ads", "U32"),  # PUBLI-HTML
+    #     None,  # PUBLI-DATAORIGIN
+    #     ("quantity", "U32"),  # DATA-QTY
+    #     ("e_axis", "U4"),  # DATA-EAXIS
+    #     ("e_mean", "f8"),  # DATA-E_MEAN
+    #     ("e_low", "f8"),  #  DATA-E_BIN_L
+    #     ("e_high", "f8"),  # DATA-E_BIN_U
+    #     ("value", "f8"),  # DATA-VAL
+    #     ("err_stat_minus", "f8"),  # DATA-VAL_ERRSTAT_L
+    #     ("err_stat_plus", "f8"),  # DATA-VAL_ERRSTAT_U
+    #     ("err_sys_minus", "f8"),  # DATA-VAL_ERRSYST_L
+    #     ("err_sys_plus", "f8"),  # DATA-VAL_ERRSYST_U
+    #     ("is_upper_limit", "?"),  # DATA-ISUPPERLIM
+    #     # ("phi", "f8"),
+    # ]
+
     fields = [
-        ("quantity", "U32"),
-        ("sub_exp", "U100"),
-        ("e_axis", "U4"),
-        ("e_mean", "f8"),
-        ("e_low", "f8"),
-        ("e_high", "f8"),
-        ("value", "f8"),
-        ("err_stat_minus", "f8"),
-        ("err_stat_plus", "f8"),
-        ("err_sys_minus", "f8"),
-        ("err_sys_plus", "f8"),
-        ("ads_url", "U32"),
-        ("phi_in_mv", "f8"),
-        ("distance_in_au", "f8"),
-        ("datetime", "U100"),
-        ("is_upper_limit", "?"),
+        ("quantity", "U32"),  # DATA-QTY
+        ("sub_exp", "U100"),  # SUBEXP-NAME
+        ("e_type", "U4"),  # DATA-EAXIS
+        ("e", "f8"),  # DATA-E_MEAN
+        ("e_bin", "f8", (2,)),  # EBIN_LOW, EBIN_HIGH
+        ("value", "f8"),  # QUANTITY VALUE
+        ("err_sta", "f8", (2,)),  # ERR_STAT-,  ERR_STAT+
+        ("err_sys", "f8", (2,)),  # ERR_SYST-, ERR_SYST+
+        ("ads", "U32"),  # ADS URL FOR PAPER REF
+        ("phi", "f8"),  # phi [MV]
+        ("distance", "f8"),  # DISTANCE [AU]
+        ("datetime", "U256"),  # DATIMES
+        ("is_upper_limit", "?"),  # IS UPPER LIMIT
     ]
 
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        table = np.loadtxt(data, fields)
+    mapping = []
+    for f in fields:
+        if f is None:
+            mapping.append(None)
+        if len(f) == 3:
+            for k in range(f[2][0]):
+                mapping.append((f[0], k))
+        else:
+            mapping.append(f[0])
+    fields = [x for x in fields if x is not None]
+
+    # workaround for invalid CSV format,
+    # to be replaced by standard parser
+    data2 = []
+    for iline, line in enumerate(data):
+        try:
+            line = line.strip()
+            if not line or line.startswith("#"):
+                continue
+            items = []
+            inquote = False
+            start = 0
+            for i, c in enumerate(line):
+                if c == '"':
+                    if inquote:
+                        items.append(line[start + 1 : i])
+                    else:
+                        start = i
+                    inquote = not inquote
+            data2.append(items)
+        except ValueError as e:
+            msg = f"{e.args[0]}\nCould not parse line {iline} {line}"
+            e.args = (msg,)
+            raise
+
+    table = np.recarray(len(data2), fields)
+    for idx, row in enumerate(data2):
+        for val, key in zip(row, mapping):
+            if key is None:
+                continue
+            if isinstance(key, tuple):
+                key, pos = key
+                table[idx][key][pos] = val
+            else:
+                table[idx][key] = val
 
     # workaround: replace &amp; in sub_exp strings
     sub_exps = np.unique(table["sub_exp"])
     code = "&amp;"
     for sub_exp in sub_exps:
         if code not in sub_exp:
             continue
         mask = table["sub_exp"] == sub_exp
         table["sub_exp"][mask] = sub_exp.replace(code, "&")
 
     # workaround: err_stat_minus or err_sys_minus may be negative
-    for x in ("stat", "sys"):
-        field = f"err_{x}_minus"
+    for x in ("sta", "sys"):
+        field = f"err_{x}"
         table[field] = np.abs(table[field])
 
-    return table.view(np.recarray)
+    return table
 
 
 def experiment_masks(
     table: NDArray, combine: Sequence[str] = COMBINE
 ) -> Dict[str, NDArray]:
     """
     Generate masks which select all points from each experiment.
@@ -680,15 +754,15 @@
 
 
 def reference_urls(table: NDArray) -> List[str]:
     """
     Return list of URLs to entries in the ADSABS database for datasets in table.
     """
     result = []
-    for key in sorted(np.unique(table["ads_url"])):
+    for key in sorted(np.unique(table.ads)):
         result.append(f"https://ui.adsabs.harvard.edu/abs/{key}")
     return result
 
 
 def bibliography(table: NDArray) -> Dict[str, str]:
     """
     Return dictionary that maps ADSABS keys in table to BibTex entries.
@@ -698,27 +772,27 @@
     try:
         from autobib.util import get_entry_online
     except ModuleNotFoundError as e:
         e.msg += ". Install autobib (`pip install autobib`) to use this function."
         raise
 
     result = {}
-    for adskey in sorted(np.unique(table["ads_url"])):
+    for adskey in sorted(np.unique(table.ads)):
         k, *r = get_entry_online(adskey)
         result[k] = "".join(r)
 
     return result
 
 
 @cachier.cachier(stale_after=datetime.timedelta(days=30))
 def all() -> NDArray:
     """
     Return the full raw CRDB database as a table.
     """
-    url = "https://lpsc.in2p3.fr/crdb/_export_all_data.php?format=usine"
+    url = "https://lpsc.in2p3.fr/crdb/_export_all_data.php?format=csv"
 
     try:
         context = ssl._create_unverified_context()
         response = rq.urlopen(url, context=context)
         connection_error = False
     except Exception:
         import traceback
@@ -732,22 +806,22 @@
             f"browser. If that works, something is wrong with url = '{url}', "
             "please report this as an issue at "
             "https://github.com/crdb-project/crdb/issues"
         )
 
     blocksize = 1024**2
     nbytes = 0
-    with tempfile.TemporaryFile() as f:
+    with tempfile.TemporaryFile(mode="w+") as f:
         while True:
             chunk = response.read(blocksize)
             nbytes += len(chunk)
             print(f"\r{nbytes / blocksize:.0f} Mb downloaded", end="", flush=True)
             if not chunk:
                 break
-            f.write(chunk)
+            f.write(chunk.decode())
         print()
         f.flush()
         f.seek(0)
         data = f.readlines()
 
     return _convert(data)
```

### Comparing `crdb-0.5.0/src/crdb/cli.py` & `crdb-0.6.0/src/crdb/cli.py`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/src/crdb/crdb_logo.png` & `crdb-0.6.0/src/crdb/crdb_logo.png`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/src/crdb/experimental.py` & `crdb-0.6.0/src/crdb/experimental.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,53 +58,52 @@
     Converted table.
     """
     ecn = energy_conversion_numbers()
 
     result = table.copy()
     for i, t in enumerate(result):
         z, a = ecn.get(t.quantity, (np.nan, np.nan))
-        if t.e_axis == "R":
+        if t.e_type == "R":
             if target == "R":
                 pass
             elif target == "EK":
                 _convert_energy(result, i, z)
-                result[i].e_axis = target
+                result[i].e_type = target
             elif target == "EKN":
                 _convert_energy(result, i, z / a)
-                result[i].e_axis = target
+                result[i].e_type = target
             else:
                 assert False
-        elif t.e_axis == "EK":
+        elif t.e_type == "EK":
             if target == "R":
                 _convert_energy(result, i, 1 / z)
-                result[i].e_axis = target
+                result[i].e_type = target
             elif target == "EK":
                 pass
             elif target == "EKN":
                 _convert_energy(result, i, 1 / a)
-                result[i].e_axis = target
+                result[i].e_type = target
             else:
                 assert False
-        elif t.e_axis == "EKN":
+        elif t.e_type == "EKN":
             if target == "R":
                 _convert_energy(result, i, a / z)
-                result[i].e_axis = target
+                result[i].e_type = target
             elif target == "EK":
                 _convert_energy(result, i, a)
-                result[i].e_axis = target
+                result[i].e_type = target
             elif target == "EKN":
                 pass
             else:
                 assert False
 
-    return result[~np.isnan(result.value) & (result.e_axis == target)]
+    return result[~np.isnan(result.value) & (result.e_type == target)]
 
 
 def _convert_energy(tab, mask, f):
-    tab[mask].e_mean *= f
-    tab[mask].e_low *= f
-    tab[mask].e_high *= f
+    if np.ndim(f) > 0:
+        f.shape = (len(f), 1)
+    tab[mask].e *= f
+    tab[mask].e_bin *= f
     tab[mask].value /= f
-    tab[mask].err_stat_minus /= f
-    tab[mask].err_stat_plus /= f
-    tab[mask].err_sys_minus /= f
-    tab[mask].err_sys_plus /= f
+    tab[mask].err_sta /= f
+    tab[mask].err_sys /= f
```

### Comparing `crdb-0.5.0/src/crdb/mpl.py` & `crdb-0.6.0/src/crdb/mpl.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     factor : array-like, optional
         Optional scaling factor for the y-coordinates. Default is 1.
     label : str, optional
         Optional label for the plot.
     sys_lw : float, optional
         Line width for the error bar that represents systematic uncertainties.
     """
-    x = table.e_mean
+    x = table.e
     y = table.value * factor
-    ye1 = table.err_stat_minus * factor, table.err_stat_plus * factor
-    ye2 = table.err_sys_minus * factor, table.err_sys_plus * factor
-    lines = plt.errorbar(table.e_mean, y, ye1, ls="none", label=label, **kwargs)[0]
+    ye1 = np.transpose(table.err_sta) * factor
+    ye2 = np.transpose(table.err_sys) * factor
+    lines = plt.errorbar(x, y, ye1, ls="none", label=label, **kwargs)[0]
     for key in ("color", "alpha", "lw", "marker"):
         if key in kwargs:
             del kwargs[key]
     plt.errorbar(
         x,
         y,
         ye2,
@@ -62,15 +62,15 @@
         Color of the text, default is '0.5'.
     kwargs :
         Other keyword arguments are forwarded to matplotlib.legend.Legend.
     """
     import matplotlib.legend as mlegend
     from matplotlib.patches import Patch
 
-    refs = np.sort(np.unique(table.ads_url))
+    refs = np.sort(np.unique(table.ads))
 
     ax = plt.gca()
     leg = mlegend.Legend(
         ax,
         handles=[Patch(color="none") for ref in refs],
         labels=refs,
         frameon=False,
```

### Comparing `crdb-0.5.0/src/crdb/solarsystem_abundances2003.dat` & `crdb-0.6.0/src/crdb/solarsystem_abundances2003.dat`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/src/crdb.egg-info/PKG-INFO` & `crdb-0.6.0/src/crdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.5.0
+Version: 0.6.0
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `crdb-0.5.0/src/crdb.egg-info/SOURCES.txt` & `crdb-0.6.0/src/crdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crdb-0.5.0/tests/test_experimental.py` & `crdb-0.6.0/tests/test_experimental.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     ecn = energy_conversion_numbers()
     assert_allclose(ecn["H"], (1, 1.000019), atol=1e-6)
     assert_allclose(ecn["He"], (2, 3.999834), atol=1e-6)
 
 
 def test_convert_energy():
     tab = all()
-    tab1 = tab[tab.e_axis == "R"]
+    tab1 = tab[tab.e_type == "R"]
     tab2 = convert_energy(tab1, "R")
     assert_equal(tab2, tab1)
     tab2 = convert_energy(tab1, "EK")
     assert len(tab2) > 0
     assert len(tab2) < len(tab1)
```

### Comparing `crdb-0.5.0/tests/test_lib.py` & `crdb-0.6.0/tests/test_lib.py`

 * *Files identical despite different names*

