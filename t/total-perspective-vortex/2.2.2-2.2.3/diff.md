# Comparing `tmp/total-perspective-vortex-2.2.2.tar.gz` & `tmp/total-perspective-vortex-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "total-perspective-vortex-2.2.2.tar", last modified: Tue Apr 25 14:42:11 2023, max compression
+gzip compressed data, was "total-perspective-vortex-2.2.3.tar", last modified: Thu May  4 12:52:08 2023, max compression
```

## Comparing `total-perspective-vortex-2.2.2.tar` & `total-perspective-vortex-2.2.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_destinations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_merge_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_params_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_resubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_mapper_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)    15774 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tests/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 14:42:11.000000 total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/tpv/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/tpv/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/dryrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.205328 total-perspective-vortex-2.2.2/tpv/commands/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/commands/test/mock_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/tpv/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34887 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:11.209328 total-perspective-vortex-2.2.2/tpv/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 14:41:57.000000 total-perspective-vortex-2.2.2/tpv/rules/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_merge_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_params_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_mapper_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tests/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 12:52:08.000000 total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/tpv/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/tpv/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/dryrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.209073 total-perspective-vortex-2.2.3/tpv/commands/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/commands/test/mock_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/tpv/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34887 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:52:08.213074 total-perspective-vortex-2.2.3/tpv/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-04 12:51:55.000000 total-perspective-vortex-2.2.3/tpv/rules/gateway.py
```

### Comparing `total-perspective-vortex-2.2.2/LICENSE` & `total-perspective-vortex-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/PKG-INFO` & `total-perspective-vortex-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.2.2
+Version: 2.2.3
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.2.2/README.md` & `total-perspective-vortex-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/setup.py` & `total-perspective-vortex-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_entity.py` & `total-perspective-vortex-2.2.3/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_basic.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_basic.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_context.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_context.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_destinations.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_destinations.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_inheritance.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_inheritance.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_merge_multiple.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_merge_multiple.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_params_specific.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_params_specific.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_rank.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_rank.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_resubmit.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_resubmit.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_role.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_role.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_rules.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_rules.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_sample.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_sample.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_mapper_user.py` & `total-perspective-vortex-2.2.3/tests/test_mapper_user.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_scenarios.py` & `total-perspective-vortex-2.2.3/tests/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tests/test_shell.py` & `total-perspective-vortex-2.2.3/tests/test_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,7 +285,18 @@
         job_config = os.path.join(os.path.dirname(__file__), 'fixtures/job_conf_dry_run.yml')
         tpv_config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-rules.yml')
         output = self.call_shell_command(
             "tpv", "dry-run", "--job-conf", job_config, "--input-size", "6", "--user", "krikkitrobot@planetkrikkit.org",
             tpv_config)
         self.assertTrue("name: TEST_JOB_SLOTS_USER" in output,
                         f"Expected 'name: TEST_JOB_SLOTS_USER' in destination\n{output}")
+        
+    def test_dry_run_tool_with_version(self):
+        job_config = os.path.join(os.path.dirname(__file__), 'fixtures/job_conf_dry_run.yml')
+        tpv_config = os.path.join(os.path.dirname(__file__), 'fixtures/mapping-rules.yml')
+        output = self.call_shell_command(
+            "tpv", "dry-run", "--job-conf", job_config, "--input-size", "6", "--user", "krikkitrobot@planetkrikkit.org",
+            "--tool", "toolshed.g2.bx.psu.edu/repos/iuc/bwameth/bwameth/42",
+            tpv_config)
+        self.assertTrue("bwameth_is_great" in output,
+                        f"Expected 'bwameth_is_great' in destination\n{output}")
+
```

### Comparing `total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/PKG-INFO` & `total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-perspective-vortex
-Version: 2.2.2
+Version: 2.2.3
 Summary: A library for routing entities (jobs, users or groups) to destinations in Galaxy
 Home-page: https://github.com/galaxyproject/total-perspective-vortex
 Author: Galaxy and GVL projects
 Author-email: help@genome.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `total-perspective-vortex-2.2.2/total_perspective_vortex.egg-info/SOURCES.txt` & `total-perspective-vortex-2.2.3/total_perspective_vortex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tpv/commands/formatter.py` & `total-perspective-vortex-2.2.3/tpv/commands/formatter.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tpv/commands/linter.py` & `total-perspective-vortex-2.2.3/tpv/commands/linter.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tpv/commands/shell.py` & `total-perspective-vortex-2.2.3/tpv/commands/shell.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tpv/commands/test/mock_galaxy.py` & `total-perspective-vortex-2.2.3/tpv/commands/test/mock_galaxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import hashlib
+
 from galaxy.model import mapping
 from galaxy.job_metrics import JobMetrics
 from galaxy.jobs import JobConfiguration
 from galaxy.util import bunch
 from galaxy.web_stack import ApplicationStack
 
 
@@ -72,18 +74,21 @@
                 create_tables=True
             )
         self.application_stack = ApplicationStack(app=self)
         self.job_config = JobConfiguration(self)
 
 
 class User:
-    def __init__(self, username, email, roles=[]):
+    def __init__(self, username, email, roles=[], id=None):
         self.username = username
         self.email = email
         self.roles = [Role(name) for name in roles]
+        self.id = id or int(
+            hashlib.sha256(f"{self.username}".encode("utf-8")).hexdigest(), 16
+        ) % 1000000
 
     def all_roles(self):
         """
         Return a unique list of Roles associated with this user or any of their groups.
         """
         return self.roles
```

### Comparing `total-perspective-vortex-2.2.2/tpv/core/entities.py` & `total-perspective-vortex-2.2.3/tpv/core/entities.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tpv/core/helpers.py` & `total-perspective-vortex-2.2.3/tpv/core/helpers.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tpv/core/loader.py` & `total-perspective-vortex-2.2.3/tpv/core/loader.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tpv/core/mapper.py` & `total-perspective-vortex-2.2.3/tpv/core/mapper.py`

 * *Files identical despite different names*

### Comparing `total-perspective-vortex-2.2.2/tpv/rules/gateway.py` & `total-perspective-vortex-2.2.3/tpv/rules/gateway.py`

 * *Files identical despite different names*

