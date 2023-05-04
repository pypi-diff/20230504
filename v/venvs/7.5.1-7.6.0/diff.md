# Comparing `tmp/venvs-7.5.1.tar.gz` & `tmp/venvs-7.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venvs-7.5.1.tar", last modified: Wed Mar  1 11:47:35 2023, max compression
+gzip compressed data, was "venvs-7.6.0.tar", last modified: Sun Apr  2 18:41:16 2023, max compression
```

## Comparing `venvs-7.5.1.tar` & `venvs-7.6.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:47:35.742719 venvs-7.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-01 11:47:25.000000 venvs-7.5.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-01 11:47:25.000000 venvs-7.5.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:47:35.738719 venvs-7.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-01 11:47:25.000000 venvs-7.5.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-01 11:47:25.000000 venvs-7.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:47:35.738719 venvs-7.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-03-01 11:47:25.000000 venvs-7.5.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-01 11:47:25.000000 venvs-7.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-01 11:47:25.000000 venvs-7.5.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-01 11:47:25.000000 venvs-7.5.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-03-01 11:47:35.742719 venvs-7.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-03-01 11:47:25.000000 venvs-7.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-01 11:47:25.000000 venvs-7.5.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:47:35.742719 venvs-7.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-01 11:47:25.000000 venvs-7.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-01 11:47:25.000000 venvs-7.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-01 11:47:25.000000 venvs-7.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-01 11:47:25.000000 venvs-7.5.1/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-01 11:47:25.000000 venvs-7.5.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-01 11:47:25.000000 venvs-7.5.1/docs/spelling-wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-01 11:47:25.000000 venvs-7.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-01 11:47:25.000000 venvs-7.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-01 11:47:35.742719 venvs-7.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-03-01 11:47:25.000000 venvs-7.5.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:47:35.742719 venvs-7.5.1/venvs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:47:35.742719 venvs-7.5.1/venvs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21635 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/tests/test_converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/tests/test_find.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/tests/test_temporary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-03-01 11:47:25.000000 venvs-7.5.1/venvs/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:47:35.742719 venvs-7.5.1/venvs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-03-01 11:47:35.000000 venvs-7.5.1/venvs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-01 11:47:35.000000 venvs-7.5.1/venvs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 11:47:35.000000 venvs-7.5.1/venvs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-01 11:47:35.000000 venvs-7.5.1/venvs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-01 11:47:35.000000 venvs-7.5.1/venvs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-01 11:47:35.000000 venvs-7.5.1/venvs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:41:16.701156 venvs-7.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-02 18:41:06.000000 venvs-7.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-02 18:41:06.000000 venvs-7.6.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:41:16.685156 venvs-7.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-02 18:41:06.000000 venvs-7.6.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-02 18:41:06.000000 venvs-7.6.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-02 18:41:06.000000 venvs-7.6.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:41:16.685156 venvs-7.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-02 18:41:06.000000 venvs-7.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-02 18:41:06.000000 venvs-7.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-02 18:41:06.000000 venvs-7.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-02 18:41:06.000000 venvs-7.6.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-04-02 18:41:16.701156 venvs-7.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-02 18:41:06.000000 venvs-7.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-02 18:41:06.000000 venvs-7.6.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:41:16.689156 venvs-7.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-02 18:41:06.000000 venvs-7.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-02 18:41:06.000000 venvs-7.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-02 18:41:06.000000 venvs-7.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-02 18:41:06.000000 venvs-7.6.0/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-02 18:41:06.000000 venvs-7.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-02 18:41:06.000000 venvs-7.6.0/docs/spelling-wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-02 18:41:06.000000 venvs-7.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-02 18:41:06.000000 venvs-7.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-02 18:41:16.701156 venvs-7.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-02 18:41:06.000000 venvs-7.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:41:16.693157 venvs-7.6.0/venvs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:41:16.701156 venvs-7.6.0/venvs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21635 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/tests/test_converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/tests/test_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/tests/test_temporary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-02 18:41:06.000000 venvs-7.6.0/venvs/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 18:41:16.697157 venvs-7.6.0/venvs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-04-02 18:41:16.000000 venvs-7.6.0/venvs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-02 18:41:16.000000 venvs-7.6.0/venvs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 18:41:16.000000 venvs-7.6.0/venvs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-02 18:41:16.000000 venvs-7.6.0/venvs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-02 18:41:16.000000 venvs-7.6.0/venvs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-02 18:41:16.000000 venvs-7.6.0/venvs.egg-info/top_level.txt
```

### Comparing `venvs-7.5.1/.github/workflows/ci.yml` & `venvs-7.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/.pre-commit-config.yaml` & `venvs-7.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/COPYING` & `venvs-7.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/PKG-INFO` & `venvs-7.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venvs
-Version: 7.5.1
+Version: 7.6.0
 Summary: "A simpler tool for creating venvs in a central location"
 Home-page: https://github.com/Julian/venvs
 Author: "Julian Berman"
 Author-email: "Julian+venvs@GrayVines.com"
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `venvs-7.5.1/README.rst` & `venvs-7.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/docs/Makefile` & `venvs-7.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/docs/conf.py` & `venvs-7.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/docs/requirements.txt` & `venvs-7.6.0/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/requirements.txt` & `venvs-7.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/setup.cfg` & `venvs-7.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/tox.ini` & `venvs-7.6.0/tox.ini`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/_config.py` & `venvs-7.6.0/venvs/_config.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/common.py` & `venvs-7.6.0/venvs/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from itertools import chain
 from shutil import which
 import os
 import platform
 import subprocess
 import sys
-import sysconfig
 
 from filesystems.click import PATH
 import attr
 import click
 import filesystems.native
 
 
@@ -174,15 +173,15 @@
     "--filesystem",
     default=filesystems.native.FS(),
     type=lambda value: value,
 )
 _LINK_DIR = click.option(
     "--link-dir",
     default=filesystems.Path.from_string(
-        sysconfig.get_path("scripts", "posix_user"),
+        os.path.expanduser("~/.local/bin/"),
     ),
     type=PATH,
     help="The directory to link scripts into.",
 )
 
 _EX_OK = getattr(os, "EX_OK", 0)
 _EX_USAGE = getattr(os, "EX_USAGE", 64)
```

### Comparing `venvs-7.5.1/venvs/converge.py` & `venvs-7.6.0/venvs/converge.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/create.py` & `venvs-7.6.0/venvs/create.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/find.py` & `venvs-7.6.0/venvs/find.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/remove.py` & `venvs-7.6.0/venvs/remove.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/tests/test_common.py` & `venvs-7.6.0/venvs/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/tests/test_config.py` & `venvs-7.6.0/venvs/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/tests/test_converge.py` & `venvs-7.6.0/venvs/tests/test_converge.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/tests/test_create.py` & `venvs-7.6.0/venvs/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/tests/test_find.py` & `venvs-7.6.0/venvs/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/tests/test_remove.py` & `venvs-7.6.0/venvs/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/tests/test_temporary.py` & `venvs-7.6.0/venvs/tests/test_temporary.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs/tests/utils.py` & `venvs-7.6.0/venvs/tests/utils.py`

 * *Files identical despite different names*

### Comparing `venvs-7.5.1/venvs.egg-info/PKG-INFO` & `venvs-7.6.0/venvs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venvs
-Version: 7.5.1
+Version: 7.6.0
 Summary: "A simpler tool for creating venvs in a central location"
 Home-page: https://github.com/Julian/venvs
 Author: "Julian Berman"
 Author-email: "Julian+venvs@GrayVines.com"
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `venvs-7.5.1/venvs.egg-info/SOURCES.txt` & `venvs-7.6.0/venvs.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 codecov.yml
 pyproject.toml
 requirements.txt
 setup.cfg
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
+.github/release.yml
 .github/workflows/ci.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/requirements.in
 docs/requirements.txt
 docs/spelling-wordlist.txt
```

