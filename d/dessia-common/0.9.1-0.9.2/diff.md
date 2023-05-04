# Comparing `tmp/dessia_common-0.9.1.tar.gz` & `tmp/dessia_common-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dessia_common-0.9.1.tar", last modified: Wed Jul 20 14:09:00 2022, max compression
+gzip compressed data, was "dessia_common-0.9.2.tar", last modified: Thu Aug 18 15:37:21 2022, max compression
```

## Comparing `dessia_common-0.9.1.tar` & `dessia_common-0.9.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 14:09:00.488810 dessia_common-0.9.1/
--rw-r--r--   0 root         (0) root         (0)      263 2022-07-20 14:06:07.000000 dessia_common-0.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1205 2022-07-20 14:09:00.488810 dessia_common-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      644 2022-07-20 14:06:07.000000 dessia_common-0.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 14:09:00.464810 dessia_common-0.9.1/dessia_common/
--rw-r--r--   0 root         (0) root         (0)      220 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8120 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/breakdown.py
--rw-r--r--   0 root         (0) root         (0)    12546 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/cluster.py
--rwxr-xr-x   0 root         (0) root         (0)    41486 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/core.py
--rw-r--r--   0 root         (0) root         (0)     4564 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/displays.py
--rw-r--r--   0 root         (0) root         (0)      783 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/errors.py
--rw-r--r--   0 root         (0) root         (0)     8712 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/exports.py
--rw-r--r--   0 root         (0) root         (0)     3645 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/files.py
--rw-r--r--   0 root         (0) root         (0)    21858 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/forms.py
--rw-r--r--   0 root         (0) root         (0)     4975 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/generation.py
--rw-r--r--   0 root         (0) root         (0)     2175 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 14:09:00.468810 dessia_common-0.9.1/dessia_common/models/
--rw-r--r--   0 root         (0) root         (0)      230 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1266 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/cars.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 14:09:00.468810 dessia_common-0.9.1/dessia_common/models/data/
--rw-r--r--   0 root         (0) root         (0)    22608 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/data/cars.csv
--rw-r--r--   0 root         (0) root         (0)       35 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/data/seed_file.csv
--rw-r--r--   0 root         (0) root         (0)     1766 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/power_test.py
--rw-r--r--   0 root         (0) root         (0)     1710 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 14:09:00.468810 dessia_common-0.9.1/dessia_common/models/workflows/
--rw-r--r--   0 root         (0) root         (0)      249 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/workflows/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3885 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/workflows/forms_workflow.py
--rw-r--r--   0 root         (0) root         (0)      764 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/workflows/power_simulation.py
--rw-r--r--   0 root         (0) root         (0)     3284 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/workflows/vectored_workflow.py
--rw-r--r--   0 root         (0) root         (0)     3766 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/models/workflows/wokflow_exports.py
--rw-r--r--   0 root         (0) root         (0)     5158 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/optimization.py
--rw-r--r--   0 root         (0) root         (0)     8254 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/templates.py
--rw-r--r--   0 root         (0) root         (0)     6357 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/tests.py
--rw-r--r--   0 root         (0) root         (0)     1530 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/typings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 14:09:00.468810 dessia_common-0.9.1/dessia_common/utils/
--rw-r--r--   0 root         (0) root         (0)      108 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1964 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/utils/algebra.py
--rw-r--r--   0 root         (0) root         (0)     2917 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/utils/copy.py
--rw-r--r--   0 root         (0) root         (0)     5155 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/utils/diff.py
--rw-r--r--   0 root         (0) root         (0)     1981 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/utils/docstrings.py
--rw-r--r--   0 root         (0) root         (0)     1633 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/utils/interpolation.py
--rw-r--r--   0 root         (0) root         (0)    14971 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/utils/jsonschema.py
--rw-r--r--   0 root         (0) root         (0)    20104 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/utils/serialization.py
--rw-r--r--   0 root         (0) root         (0)    13789 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/utils/types.py
--rwxr-xr-x   0 root         (0) root         (0)    21271 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/vectored_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 14:09:00.468810 dessia_common-0.9.1/dessia_common/workflow/
--rw-r--r--   0 root         (0) root         (0)      173 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37812 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/workflow/blocks.py
--rw-r--r--   0 root         (0) root         (0)    83766 2022-07-20 14:06:07.000000 dessia_common-0.9.1/dessia_common/workflow/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 14:09:00.464810 dessia_common-0.9.1/dessia_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1205 2022-07-20 14:09:00.000000 dessia_common-0.9.1/dessia_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1616 2022-07-20 14:09:00.000000 dessia_common-0.9.1/dessia_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-20 14:09:00.000000 dessia_common-0.9.1/dessia_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2022-07-20 14:09:00.000000 dessia_common-0.9.1/dessia_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-07-20 14:09:00.000000 dessia_common-0.9.1/dessia_common.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 14:09:00.488810 dessia_common-0.9.1/scripts/
--rw-r--r--   0 root         (0) root         (0)     1046 2022-07-20 14:06:07.000000 dessia_common-0.9.1/scripts/compilation_test.py
--rw-r--r--   0 root         (0) root         (0) 22664612 2022-07-20 14:06:07.000000 dessia_common-0.9.1/scripts/debug_variable_values.py
--rw-r--r--   0 root         (0) root         (0)      342 2022-07-20 14:06:07.000000 dessia_common-0.9.1/scripts/dessia_object.py
--rw-r--r--   0 root         (0) root         (0)      518 2022-07-20 14:06:07.000000 dessia_common-0.9.1/scripts/simple_functions_workflow.py
--rw-r--r--   0 root         (0) root         (0)     4184 2022-07-20 14:06:07.000000 dessia_common-0.9.1/scripts/workflow_concatenate.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-20 14:09:00.488810 dessia_common-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4874 2022-07-20 14:06:07.000000 dessia_common-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 15:37:21.448422 dessia_common-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)      263 2022-08-18 15:34:46.000000 dessia_common-0.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1205 2022-08-18 15:37:21.448422 dessia_common-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      644 2022-08-18 15:34:46.000000 dessia_common-0.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 15:37:21.428422 dessia_common-0.9.2/dessia_common/
+-rw-r--r--   0 root         (0) root         (0)      220 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8120 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/breakdown.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/cluster.py
+-rwxr-xr-x   0 root         (0) root         (0)    41486 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/core.py
+-rw-r--r--   0 root         (0) root         (0)     5018 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/displays.py
+-rw-r--r--   0 root         (0) root         (0)      783 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/errors.py
+-rw-r--r--   0 root         (0) root         (0)     8717 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/exports.py
+-rw-r--r--   0 root         (0) root         (0)     3645 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/files.py
+-rw-r--r--   0 root         (0) root         (0)    21858 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/forms.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/generation.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 15:37:21.428422 dessia_common-0.9.2/dessia_common/models/
+-rw-r--r--   0 root         (0) root         (0)      230 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1266 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/cars.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 15:37:21.428422 dessia_common-0.9.2/dessia_common/models/data/
+-rw-r--r--   0 root         (0) root         (0)    22608 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/data/cars.csv
+-rw-r--r--   0 root         (0) root         (0)       35 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/data/seed_file.csv
+-rw-r--r--   0 root         (0) root         (0)     1766 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/power_test.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 15:37:21.428422 dessia_common-0.9.2/dessia_common/models/workflows/
+-rw-r--r--   0 root         (0) root         (0)      249 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/workflows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3885 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/workflows/forms_workflow.py
+-rw-r--r--   0 root         (0) root         (0)      764 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/workflows/power_simulation.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/workflows/vectored_workflow.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/models/workflows/wokflow_exports.py
+-rw-r--r--   0 root         (0) root         (0)     5158 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/optimization.py
+-rw-r--r--   0 root         (0) root         (0)     8254 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/templates.py
+-rw-r--r--   0 root         (0) root         (0)     6357 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/typings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 15:37:21.428422 dessia_common-0.9.2/dessia_common/utils/
+-rw-r--r--   0 root         (0) root         (0)      108 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/utils/algebra.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/utils/copy.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/utils/diff.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/utils/docstrings.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/utils/interpolation.py
+-rw-r--r--   0 root         (0) root         (0)    14971 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/utils/jsonschema.py
+-rw-r--r--   0 root         (0) root         (0)    20104 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/utils/serialization.py
+-rw-r--r--   0 root         (0) root         (0)    13789 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/utils/types.py
+-rwxr-xr-x   0 root         (0) root         (0)    21271 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/vectored_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 15:37:21.428422 dessia_common-0.9.2/dessia_common/workflow/
+-rw-r--r--   0 root         (0) root         (0)      173 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37823 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/workflow/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    83853 2022-08-18 15:34:46.000000 dessia_common-0.9.2/dessia_common/workflow/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 15:37:21.428422 dessia_common-0.9.2/dessia_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1205 2022-08-18 15:37:21.000000 dessia_common-0.9.2/dessia_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1616 2022-08-18 15:37:21.000000 dessia_common-0.9.2/dessia_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-18 15:37:21.000000 dessia_common-0.9.2/dessia_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2022-08-18 15:37:21.000000 dessia_common-0.9.2/dessia_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-08-18 15:37:21.000000 dessia_common-0.9.2/dessia_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 15:37:21.448422 dessia_common-0.9.2/scripts/
+-rw-r--r--   0 root         (0) root         (0)     1046 2022-08-18 15:34:46.000000 dessia_common-0.9.2/scripts/compilation_test.py
+-rw-r--r--   0 root         (0) root         (0) 22664612 2022-08-18 15:34:46.000000 dessia_common-0.9.2/scripts/debug_variable_values.py
+-rw-r--r--   0 root         (0) root         (0)      342 2022-08-18 15:34:46.000000 dessia_common-0.9.2/scripts/dessia_object.py
+-rw-r--r--   0 root         (0) root         (0)      518 2022-08-18 15:34:46.000000 dessia_common-0.9.2/scripts/simple_functions_workflow.py
+-rw-r--r--   0 root         (0) root         (0)     4184 2022-08-18 15:34:46.000000 dessia_common-0.9.2/scripts/workflow_concatenate.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-18 15:37:21.448422 dessia_common-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4874 2022-08-18 15:34:46.000000 dessia_common-0.9.2/setup.py
```

### Comparing `dessia_common-0.9.1/PKG-INFO` & `dessia_common-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dessia_common
-Version: 0.9.1
+Version: 0.9.2
 Summary: Common tools for DessIA software
 Home-page: https://github.com/Dessia-tech/dessia-common
 Author: Steven Masfaraud
 Author-email: masfaraud@dessia.tech
 License: UNKNOWN
 Description: # Dessia common
```

### Comparing `dessia_common-0.9.1/README.md` & `dessia_common-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/breakdown.py` & `dessia_common-0.9.2/dessia_common/breakdown.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/cluster.py` & `dessia_common-0.9.2/dessia_common/cluster.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/core.py` & `dessia_common-0.9.2/dessia_common/core.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/displays.py` & `dessia_common-0.9.2/dessia_common/displays.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 displays for dessia_common
 
 """
+import warnings
 import webbrowser
 import os
 import tempfile
 import inspect
 
-from typing import Union
+from typing import Union, List
 from networkx import DiGraph, Graph, kamada_kawai_layout
 from dessia_common.templates import visjs_template
 from dessia_common.typings import JsonSerializable
+from dessia_common.utils.types import is_sequence
 
 
 class DisplaySetting:
     def __init__(self, selector, type_, method, arguments=None, serialize_data: bool = False):
         """
         Describe what method to call to get a display
         """
@@ -39,21 +41,25 @@
         to method name
         """
         return DisplaySetting(selector=self.selector, type_=self.type, method=f'{attribute}.{self.method}',
                               arguments=self.arguments, serialize_data=serialize_data)
 
 
 class DisplayObject:
-    def __init__(self, type_: str, data: Union[JsonSerializable, str], reference_path: str = '',
-                 traceback: str = '', name: str = ''):
+    def __init__(self, type_: str, data: Union[JsonSerializable, List[JsonSerializable], str],
+                 reference_path: str = '', traceback: str = '', name: str = ''):
         """
         Container for data of display
         A traceback can be set if display fails to be generated.
         """
-
+        if type_ == "plot_data" and not is_sequence(data):
+            warnings.warn("A plot_data DisplayObject must be called with data as a sequence. "
+                          "Please return a list of PlotData objects as the result of plot_data method. "
+                          "Change have been made automatically", Warning)
+            data = [data]
         self.type_ = type_
         self.data = data
         self.traceback = traceback
         self.reference_path = reference_path
         self.name = name
 
         if data and type_ == 'markdown':
```

### Comparing `dessia_common-0.9.1/dessia_common/errors.py` & `dessia_common-0.9.2/dessia_common/errors.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/exports.py` & `dessia_common-0.9.2/dessia_common/exports.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,13 +243,13 @@
         for col in sheet.columns:
             width = min_width
             column = col[1].column_letter  # Get the column name
             # Since Openpyxl 2.6, the column name is  ".column_letter" as .column became the column number (1-based)
             for cell in col:
                 try:  # Necessary to avoid error on empty cells
                     if len(str(cell.value)) > width:
-                        width = len(cell.value)
+                        width = len(str(cell.value))
                 except AttributeError:
                     pass
             if width > 0:
                 adjusted_width = min((width + 0.5), max_width)
                 sheet.column_dimensions[column].width = adjusted_width
```

### Comparing `dessia_common-0.9.1/dessia_common/files.py` & `dessia_common-0.9.2/dessia_common/files.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/forms.py` & `dessia_common-0.9.2/dessia_common/forms.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/generation.py` & `dessia_common-0.9.2/dessia_common/generation.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/graph.py` & `dessia_common-0.9.2/dessia_common/graph.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/models/cars.py` & `dessia_common-0.9.2/dessia_common/models/cars.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/models/data/cars.csv` & `dessia_common-0.9.2/dessia_common/models/data/cars.csv`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/models/power_test.py` & `dessia_common-0.9.2/dessia_common/models/power_test.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/models/tests.py` & `dessia_common-0.9.2/dessia_common/models/tests.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/models/workflows/forms_workflow.py` & `dessia_common-0.9.2/dessia_common/models/workflows/forms_workflow.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/models/workflows/power_simulation.py` & `dessia_common-0.9.2/dessia_common/models/workflows/power_simulation.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/models/workflows/vectored_workflow.py` & `dessia_common-0.9.2/dessia_common/models/workflows/vectored_workflow.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/models/workflows/wokflow_exports.py` & `dessia_common-0.9.2/dessia_common/models/workflows/wokflow_exports.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/optimization.py` & `dessia_common-0.9.2/dessia_common/optimization.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/templates.py` & `dessia_common-0.9.2/dessia_common/templates.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/tests.py` & `dessia_common-0.9.2/dessia_common/tests.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/typings.py` & `dessia_common-0.9.2/dessia_common/typings.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/utils/algebra.py` & `dessia_common-0.9.2/dessia_common/utils/algebra.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/utils/copy.py` & `dessia_common-0.9.2/dessia_common/utils/copy.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/utils/diff.py` & `dessia_common-0.9.2/dessia_common/utils/diff.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/utils/docstrings.py` & `dessia_common-0.9.2/dessia_common/utils/docstrings.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/utils/interpolation.py` & `dessia_common-0.9.2/dessia_common/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/utils/jsonschema.py` & `dessia_common-0.9.2/dessia_common/utils/jsonschema.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/utils/serialization.py` & `dessia_common-0.9.2/dessia_common/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/utils/types.py` & `dessia_common-0.9.2/dessia_common/utils/types.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/vectored_objects.py` & `dessia_common-0.9.2/dessia_common/vectored_objects.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/dessia_common/workflow/blocks.py` & `dessia_common-0.9.2/dessia_common/workflow/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from dessia_common.utils.types import get_python_class_from_class_name, full_classname
 from dessia_common.utils.docstrings import parse_docstring, EMPTY_PARSED_ATTRIBUTE
 from dessia_common.errors import UntypedArgumentError
 from dessia_common.typings import JsonSerializable, MethodType, ClassMethodType
 from dessia_common.files import StringFile, BinaryFile
 
 from dessia_common.workflow.core import Block, Variable, TypedVariable, TypedVariableWithDefaultValue,\
-    set_block_variable_names_from_dict, Workflow, DisplaySetting
+    set_block_variable_names_from_dict, Workflow, DisplaySetting, DisplayObject
 
 
 def set_inputs_from_function(method, inputs=None):
     """
     Inspect given method argspecs and sets block inputs from it
     """
     if inputs is None:
@@ -638,34 +638,31 @@
         return Block.equivalent(self, other) and same_attributes and same_order
 
     def equivalent_hash(self):
         return sum(len(a) for a in self.attributes) + self.order
 
     def display_(self, local_values, **kwargs):
         import plot_data
-        # if 'reference_path' not in kwargs:
-        #     reference_path = 'output_value'  # TODO bof bof bof
-        # else:
-        #     reference_path = kwargs['reference_path']
-
+        reference_path = kwargs.get("reference_path", "")
         objects = local_values[self.inputs[self._displayable_input]]
         values = [{a: enhanced_deep_attr(o, a) for a in self.attributes} for o in objects]
         values2d = [{key: val[key]} for key in self.attributes[:2] for val in values]
         tooltip = plot_data.Tooltip(name='Tooltip', attributes=self.attributes)
 
         scatterplot = plot_data.Scatter(tooltip=tooltip, x_variable=self.attributes[0], y_variable=self.attributes[1],
                                         elements=values2d, name='Scatter Plot')
 
         parallelplot = plot_data.ParallelPlot(disposition='horizontal', axes=self.attributes,
                                               rgbs=[(192, 11, 11), (14, 192, 11), (11, 11, 192)], elements=values)
         objects = [scatterplot, parallelplot]
         sizes = [plot_data.Window(width=560, height=300), plot_data.Window(width=560, height=300)]
         multiplot = plot_data.MultiplePlots(elements=values, plots=objects, sizes=sizes,
                                             coords=[(0, 0), (0, 300)], name='Results plot')
-        return [multiplot.to_dict()]
+        display_object = DisplayObject(type_="plot_data", data=[multiplot.to_dict()], reference_path=reference_path)
+        return [display_object.to_dict()]
 
     def _display_settings(self, block_index: int, local_values: Dict[Variable, Any] = None) -> List[DisplaySetting]:
         display_settings = DisplaySetting(selector="display_" + str(block_index), type_="plot_data",
                                           method="block_display", serialize_data=True,
                                           arguments={'block_index': block_index, "display_index": 0})
         return [display_settings]
```

### Comparing `dessia_common-0.9.1/dessia_common/workflow/core.py` & `dessia_common-0.9.2/dessia_common/workflow/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1821,32 +1821,32 @@
         Returns found object
         """
         try:
             return DessiaObject._get_from_path(self, path)
         except ExtractionError:
             segments = path.split("/")
             first_segment = segments[1]
-            if first_segment == "values" and len(segments) == 3:
+            if first_segment == "values" and len(segments) >= 3:
                 varindex = int(segments[2])
                 variable = self.workflow.variables[varindex]
                 upstream = self.workflow.get_upstream_nbv(variable)
-                return self.values[upstream]
+                value = self.values[upstream]
+                if len(segments) > 3:
+                    return DessiaObject._get_from_path(value, f"#/{'/'.join(segments[3:])}")
+                return value
         raise NotImplementedError(f"WorkflowRun : Specific object from path method is not defined for path '{path}'")
 
     def _display_from_selector(self, selector: str, **kwargs) -> DisplayObject:
         """
         Generate the display from the selector
         """
         # TODO THIS IS A TEMPORARY DIRTY HOTFIX OVERWRITE.
         #  WE SHOULD IMPLEMENT A WAY TO GET RID OF REFERENCE PATH WITH URLS
         track = ""
-        if "reference_path" in kwargs:
-            refpath = kwargs["reference_path"]
-        else:
-            refpath = ""
+        refpath = kwargs.get("reference_path", "")
         if selector in ["documentation", "workflow"]:
             return self.workflow._display_from_selector(selector)
 
         if selector == "workflow-state":
             return DessiaObject._display_from_selector(self, selector)
 
         # Displays for blocks (getting reference path from block_display return)
```

### Comparing `dessia_common-0.9.1/dessia_common.egg-info/PKG-INFO` & `dessia_common-0.9.2/dessia_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dessia-common
-Version: 0.9.1
+Version: 0.9.2
 Summary: Common tools for DessIA software
 Home-page: https://github.com/Dessia-tech/dessia-common
 Author: Steven Masfaraud
 Author-email: masfaraud@dessia.tech
 License: UNKNOWN
 Description: # Dessia common
```

### Comparing `dessia_common-0.9.1/dessia_common.egg-info/SOURCES.txt` & `dessia_common-0.9.2/dessia_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/scripts/compilation_test.py` & `dessia_common-0.9.2/scripts/compilation_test.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/scripts/debug_variable_values.py` & `dessia_common-0.9.2/scripts/debug_variable_values.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/scripts/simple_functions_workflow.py` & `dessia_common-0.9.2/scripts/simple_functions_workflow.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/scripts/workflow_concatenate.py` & `dessia_common-0.9.2/scripts/workflow_concatenate.py`

 * *Files identical despite different names*

### Comparing `dessia_common-0.9.1/setup.py` & `dessia_common-0.9.2/setup.py`

 * *Files identical despite different names*

