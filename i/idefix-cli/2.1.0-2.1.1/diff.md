# Comparing `tmp/idefix_cli-2.1.0.tar.gz` & `tmp/idefix_cli-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-2.1.0.tar", last modified: Thu May  4 13:22:53 2023, max compression
+gzip compressed data, was "idefix_cli-2.1.1.tar", last modified: Thu May  4 16:24:17 2023, max compression
```

## Comparing `idefix_cli-2.1.0.tar` & `idefix_cli-2.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 13:22:53.000000 idefix_cli-2.1.0/idefix_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:22:53.310298 idefix_cli-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-04 13:22:43.000000 idefix_cli-2.1.0/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.624853 idefix_cli-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 16:24:17.624853 idefix_cli-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.616853 idefix_cli-2.1.1/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.620853 idefix_cli-2.1.1/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.616853 idefix_cli-2.1.1/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 16:24:17.000000 idefix_cli-2.1.1/idefix_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:24:17.624853 idefix_cli-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:24:17.620853 idefix_cli-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-04 16:24:05.000000 idefix_cli-2.1.1/tests/test_write.py
```

### Comparing `idefix_cli-2.1.0/LICENSE` & `idefix_cli-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/PKG-INFO` & `idefix_cli-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix_cli
-Version: 2.1.0
+Version: 2.1.1
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `idefix_cli-2.1.0/README.md` & `idefix_cli-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/__main__.py` & `idefix_cli-2.1.1/idefix_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/_backports.py` & `idefix_cli-2.1.1/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/_commands/clean.py` & `idefix_cli-2.1.1/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/_commands/clone.py` & `idefix_cli-2.1.1/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/_commands/conf.py` & `idefix_cli-2.1.1/idefix_cli/_commands/conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/_commands/read.py` & `idefix_cli-2.1.1/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/_commands/run.py` & `idefix_cli-2.1.1/idefix_cli/_commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             "Requires the code to be configured for MPI."
         ),
     )
     parser.add_argument(
         "--times",
         dest="multiplier",
         type=int,
-        default=-1,
+        default=None,
         help="multiplier for --one (use `--one --times 2` to run for 2 steps)",
     )
 
 
 def command(
     *unknown_args: str,
     directory: str = ".",
@@ -242,15 +242,15 @@
 
         output_sec["log"] = 1
 
         if len(output_types) > 0:
             for entry in output_types:
                 output_sec[entry] = 0  # output on every time step
 
-    multiplier = multiplier or 1
+    multiplier = multiplier or -1
 
     if time_step is not None:
         conf["TimeIntegrator"]["first_dt"] = time_step
     if duration is not None:
         print_warning("The --duration argument is deprecated. Use --tstop instead.")
         conf["TimeIntegrator"]["tstop"] = duration
     elif tstop is not None:
```

### Comparing `idefix_cli-2.1.0/idefix_cli/_commands/stamp.py` & `idefix_cli-2.1.1/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/_commands/switch.py` & `idefix_cli-2.1.1/idefix_cli/_commands/switch.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/_commands/write.py` & `idefix_cli-2.1.1/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli/lib.py` & `idefix_cli-2.1.1/idefix_cli/lib.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-2.1.1/idefix_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix-cli
-Version: 2.1.0
+Version: 2.1.1
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `idefix_cli-2.1.0/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-2.1.1/idefix_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/pyproject.toml` & `idefix_cli-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idefix_cli"
-version = "2.1.0"
+version = "2.1.1"
 description = "A CLI to automate mundane tasks with Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
```

### Comparing `idefix_cli-2.1.0/tests/test_app_structure.py` & `idefix_cli-2.1.1/tests/test_app_structure.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/tests/test_clean.py` & `idefix_cli-2.1.1/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/tests/test_clone.py` & `idefix_cli-2.1.1/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/tests/test_commons.py` & `idefix_cli-2.1.1/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/tests/test_conf.py` & `idefix_cli-2.1.1/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/tests/test_read.py` & `idefix_cli-2.1.1/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/tests/test_run.py` & `idefix_cli-2.1.1/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/tests/test_stamp.py` & `idefix_cli-2.1.1/tests/test_stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/tests/test_ux.py` & `idefix_cli-2.1.1/tests/test_ux.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.1.0/tests/test_write.py` & `idefix_cli-2.1.1/tests/test_write.py`

 * *Files identical despite different names*

