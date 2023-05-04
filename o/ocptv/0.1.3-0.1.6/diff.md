# Comparing `tmp/ocptv-0.1.3.tar.gz` & `tmp/ocptv-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocptv-0.1.3.tar", last modified: Tue May  2 17:09:41 2023, max compression
+gzip compressed data, was "ocptv-0.1.6.tar", last modified: Thu May  4 15:13:04 2023, max compression
```

## Comparing `ocptv-0.1.3.tar` & `ocptv-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,62 @@
-drwxr-xr-x   0 aeh       (1000) aeh       (1000)        0 2023-05-02 17:09:41.890747 ocptv-0.1.3/
--rw-r--r--   0 aeh       (1000) aeh       (1000)     1077 2023-04-15 18:06:24.000000 ocptv-0.1.3/LICENSE
--rw-r--r--   0 aeh       (1000) aeh       (1000)    10994 2023-05-02 17:09:41.889747 ocptv-0.1.3/PKG-INFO
--rw-r--r--   0 aeh       (1000) aeh       (1000)     8757 2023-05-02 17:08:31.000000 ocptv-0.1.3/README.md
-drwxr-xr-x   0 aeh       (1000) aeh       (1000)        0 2023-05-02 17:09:41.887747 ocptv-0.1.3/ocptv/
--rw-r--r--   0 aeh       (1000) aeh       (1000)      143 2023-04-16 20:22:53.000000 ocptv-0.1.3/ocptv/__init__.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)      998 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/api.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)      622 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/formatter.py
-drwxr-xr-x   0 aeh       (1000) aeh       (1000)        0 2023-05-02 17:09:41.889747 ocptv-0.1.3/ocptv/output/
--rw-r--r--   0 aeh       (1000) aeh       (1000)      642 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/output/__init__.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)     3643 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/output/config.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)    11209 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/output/dut.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)     4812 2023-05-02 17:07:05.000000 ocptv-0.1.3/ocptv/output/emit.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)     6421 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/output/measurement.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)    30138 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/output/objects.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)     9569 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/output/run.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)     6533 2023-05-02 17:07:05.000000 ocptv-0.1.3/ocptv/output/runtime_checks.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)     3712 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/output/source.py
--rw-r--r--   0 aeh       (1000) aeh       (1000)    14630 2023-05-02 17:08:31.000000 ocptv-0.1.3/ocptv/output/step.py
-drwxr-xr-x   0 aeh       (1000) aeh       (1000)        0 2023-05-02 17:09:41.888747 ocptv-0.1.3/ocptv.egg-info/
--rw-r--r--   0 aeh       (1000) aeh       (1000)    10994 2023-05-02 17:09:41.000000 ocptv-0.1.3/ocptv.egg-info/PKG-INFO
--rw-r--r--   0 aeh       (1000) aeh       (1000)      486 2023-05-02 17:09:41.000000 ocptv-0.1.3/ocptv.egg-info/SOURCES.txt
--rw-r--r--   0 aeh       (1000) aeh       (1000)        1 2023-05-02 17:09:41.000000 ocptv-0.1.3/ocptv.egg-info/dependency_links.txt
--rw-r--r--   0 aeh       (1000) aeh       (1000)       60 2023-05-02 17:09:41.000000 ocptv-0.1.3/ocptv.egg-info/requires.txt
--rw-r--r--   0 aeh       (1000) aeh       (1000)        6 2023-05-02 17:09:41.000000 ocptv-0.1.3/ocptv.egg-info/top_level.txt
--rw-r--r--   0 aeh       (1000) aeh       (1000)     1865 2023-05-02 17:08:31.000000 ocptv-0.1.3/pyproject.toml
--rw-r--r--   0 aeh       (1000) aeh       (1000)       38 2023-05-02 17:09:41.890747 ocptv-0.1.3/setup.cfg
-drwxr-xr-x   0 aeh       (1000) aeh       (1000)        0 2023-05-02 17:09:41.889747 ocptv-0.1.3/tests/
--rw-r--r--   0 aeh       (1000) aeh       (1000)      728 2023-04-16 20:22:53.000000 ocptv-0.1.3/tests/test_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:04.273066 ocptv-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 15:12:47.000000 ocptv-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 15:12:47.000000 ocptv-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-04 15:13:04.273066 ocptv-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-05-04 15:12:47.000000 ocptv-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:04.265066 ocptv-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-04 15:12:47.000000 ocptv-0.1.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 15:12:47.000000 ocptv-0.1.6/docs/output.config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-04 15:12:47.000000 ocptv-0.1.6/docs/output.dut.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23459 2023-05-04 15:12:47.000000 ocptv-0.1.6/docs/output.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-04 15:12:47.000000 ocptv-0.1.6/docs/output.measurement.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32154 2023-05-04 15:12:47.000000 ocptv-0.1.6/docs/output.objects.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-04 15:12:47.000000 ocptv-0.1.6/docs/output.run.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-04 15:12:47.000000 ocptv-0.1.6/docs/output.source.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-05-04 15:12:47.000000 ocptv-0.1.6/docs/output.step.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:04.269066 ocptv-0.1.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-04 15:12:47.000000 ocptv-0.1.6/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-04 15:12:47.000000 ocptv-0.1.6/examples/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-04 15:12:47.000000 ocptv-0.1.6/examples/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-04 15:12:47.000000 ocptv-0.1.6/examples/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-04 15:12:47.000000 ocptv-0.1.6/examples/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-04 15:12:47.000000 ocptv-0.1.6/examples/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-04 15:12:47.000000 ocptv-0.1.6/examples/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-05-04 15:12:47.000000 ocptv-0.1.6/examples/sample_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 15:12:47.000000 ocptv-0.1.6/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-04 15:12:47.000000 ocptv-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:13:04.273066 ocptv-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:04.265066 ocptv-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:04.269066 ocptv-0.1.6/src/ocptv/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:04.269066 ocptv-0.1.6/src/ocptv/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30138 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/runtime_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-05-04 15:12:47.000000 ocptv-0.1.6/src/ocptv/output/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:04.269066 ocptv-0.1.6/src/ocptv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-04 15:13:04.000000 ocptv-0.1.6/src/ocptv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-04 15:13:04.000000 ocptv-0.1.6/src/ocptv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:13:04.000000 ocptv-0.1.6/src/ocptv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 15:13:04.000000 ocptv-0.1.6/src/ocptv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 15:13:04.000000 ocptv-0.1.6/src/ocptv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:04.269066 ocptv-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:13:04.273066 ocptv-0.1.6/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/output/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/output/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/output/test_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/output/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/output/test_runtime_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/output/test_schema_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/output/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/output/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 15:12:47.000000 ocptv-0.1.6/tests/test_formatter.py
```

### Comparing `ocptv-0.1.3/LICENSE` & `ocptv-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/PKG-INFO` & `ocptv-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocptv
-Version: 0.1.3
+Version: 0.1.6
 Summary: OCP Test & Validation project api
 Author-email: OCP Test & Validation <ocp-test-validation@OCP-All.groups.io>
 License: MIT License
         
         Copyright (c) 2023 Open Compute Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -221,15 +221,15 @@
 $ python -m examples demo_diagnosis
 ```
 
 The [sample output file](https://github.com/opencomputeproject/ocp-diag-python/tree/dev/examples/sample_output.txt) shows a run of all demos. This is meant as documentation.
 
 ### Developer notes
 
-If you would like to contribute, please head over to [developer notes](https://github.com/opencomputeproject/ocp-diag-python/developer_notes.md) for instructions regarding setting up a development environment and more on submitting code.
+If you would like to contribute, please head over to [developer notes](https://github.com/opencomputeproject/ocp-diag-python/tree/dev/DEVELOPER_NOTES.md) for instructions regarding setting up a development environment and more on submitting code.
 
 ### Contact
 
 Feel free to start a new [discussion](https://github.com/opencomputeproject/ocp-diag-python/discussions), or otherwise post an [issue/request](https://github.com/opencomputeproject/ocp-diag-python/issues).
 
 An email contact is also available at: ocp-test-validation@OCP-All.groups.io
```

### Comparing `ocptv-0.1.3/README.md` & `ocptv-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 $ python -m examples demo_diagnosis
 ```
 
 The [sample output file](https://github.com/opencomputeproject/ocp-diag-python/tree/dev/examples/sample_output.txt) shows a run of all demos. This is meant as documentation.
 
 ### Developer notes
 
-If you would like to contribute, please head over to [developer notes](https://github.com/opencomputeproject/ocp-diag-python/developer_notes.md) for instructions regarding setting up a development environment and more on submitting code.
+If you would like to contribute, please head over to [developer notes](https://github.com/opencomputeproject/ocp-diag-python/tree/dev/DEVELOPER_NOTES.md) for instructions regarding setting up a development environment and more on submitting code.
 
 ### Contact
 
 Feel free to start a new [discussion](https://github.com/opencomputeproject/ocp-diag-python/discussions), or otherwise post an [issue/request](https://github.com/opencomputeproject/ocp-diag-python/issues).
 
 An email contact is also available at: ocp-test-validation@OCP-All.groups.io
```

### Comparing `ocptv-0.1.3/ocptv/api.py` & `ocptv-0.1.6/src/ocptv/api.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/formatter.py` & `ocptv-0.1.6/src/ocptv/formatter.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/__init__.py` & `ocptv-0.1.6/src/ocptv/output/__init__.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/config.py` & `ocptv-0.1.6/src/ocptv/output/config.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/dut.py` & `ocptv-0.1.6/src/ocptv/output/dut.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/emit.py` & `ocptv-0.1.6/src/ocptv/output/emit.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/measurement.py` & `ocptv-0.1.6/src/ocptv/output/measurement.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/objects.py` & `ocptv-0.1.6/src/ocptv/output/objects.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/run.py` & `ocptv-0.1.6/src/ocptv/output/run.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/runtime_checks.py` & `ocptv-0.1.6/src/ocptv/output/runtime_checks.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/source.py` & `ocptv-0.1.6/src/ocptv/output/source.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv/output/step.py` & `ocptv-0.1.6/src/ocptv/output/step.py`

 * *Files identical despite different names*

### Comparing `ocptv-0.1.3/ocptv.egg-info/PKG-INFO` & `ocptv-0.1.6/src/ocptv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocptv
-Version: 0.1.3
+Version: 0.1.6
 Summary: OCP Test & Validation project api
 Author-email: OCP Test & Validation <ocp-test-validation@OCP-All.groups.io>
 License: MIT License
         
         Copyright (c) 2023 Open Compute Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -221,15 +221,15 @@
 $ python -m examples demo_diagnosis
 ```
 
 The [sample output file](https://github.com/opencomputeproject/ocp-diag-python/tree/dev/examples/sample_output.txt) shows a run of all demos. This is meant as documentation.
 
 ### Developer notes
 
-If you would like to contribute, please head over to [developer notes](https://github.com/opencomputeproject/ocp-diag-python/developer_notes.md) for instructions regarding setting up a development environment and more on submitting code.
+If you would like to contribute, please head over to [developer notes](https://github.com/opencomputeproject/ocp-diag-python/tree/dev/DEVELOPER_NOTES.md) for instructions regarding setting up a development environment and more on submitting code.
 
 ### Contact
 
 Feel free to start a new [discussion](https://github.com/opencomputeproject/ocp-diag-python/discussions), or otherwise post an [issue/request](https://github.com/opencomputeproject/ocp-diag-python/issues).
 
 An email contact is also available at: ocp-test-validation@OCP-All.groups.io
```

### Comparing `ocptv-0.1.3/pyproject.toml` & `ocptv-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ocptv"
-version = "0.1.3"
+version = "0.1.6"
 description = "OCP Test & Validation project api"
 readme = "README.md"
 authors = [{ name = "OCP Test & Validation", email = "ocp-test-validation@OCP-All.groups.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,38 +29,38 @@
 
 [project.urls]
 "Homepage" = "https://github.com/opencomputeproject/ocp-diag-python"
 "Bug reports" = "https://github.com/opencomputeproject/ocp-diag-python/issues"
 "Source" = "https://github.com/opencomputeproject/ocp-diag-python"
 
 [tool.bumpver]
-current_version = "0.1.3"
+current_version = "0.1.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
-"ocptv/__init__.py" = [
+"src/ocptv/__init__.py" = [
     "{version}"
 ]
 
 [tool.pytest.ini_options]
-pythonpath = ["."]
+pythonpath = ["src"]
 addopts = "--cov=ocptv --cov-report term-missing tests/"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "ocptv"
-version = "0.1.3"
+version = "0.1.6"
 description = "OCP Test & Validation project api"
 authors = ["OCP Test & Validation <ocp-test-validation@OCP-All.groups.io>"]
```

### Comparing `ocptv-0.1.3/tests/test_formatter.py` & `ocptv-0.1.6/tests/test_formatter.py`

 * *Files identical despite different names*

