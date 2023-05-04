# Comparing `tmp/edwh_pipcompile_plugin-0.1.7.tar.gz` & `tmp/edwh_pipcompile_plugin-0.1.8.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.1.7.tar` & `edwh_pipcompile_plugin-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/README.md
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    10907 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/README.md
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.8/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.1.7/CHANGELOG.md` & `edwh_pipcompile_plugin-0.1.8/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.8 (2023-05-04)
+### Fix
+* **compile:** Allow multiple paths to be compiled at once. ([`2318a81`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/2318a81929ea2425845fb5569e018407a2a4cf52))
+
 ## v0.1.7 (2023-05-01)
 ### Fix
 * **upgrade:** `pip.upgrade` now actually includes the upgrade flag to pip-compile ([`8ada23d`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/8ada23df192f3813a6628c0ca77169dadae058ca))
 
 ## v0.1.6 (2023-04-17)
 ### Fix
 * **semver:** Semantic-release types should be a comma-separated string, not an array ([`4dd0394`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/4dd039434decb2ed8e2b1feff6a061f5bc49b4e3))
```

### Comparing `edwh_pipcompile_plugin-0.1.7/requirements-dev.txt` & `edwh_pipcompile_plugin-0.1.8/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.7/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.1.8/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,40 +227,41 @@
         re.MULTILINE | re.IGNORECASE,
     )
 
 
 ### ONLY @task's AFTER THIS!!!
 
 
-@task()
+@task(iterable=('path',))
 def compile(ctx, path, pypi_server=DEFAULT_SERVER):
     """
     Task (invoke pip.compile) to run pip-compile on one or more files (-f requirements1.in -f requirements2.in)
 
     Arguments:
         ctx (invoke.Context): invoke context
         path (str): path to directory to compile infiles or specific infile
         pypi_server (str): which server to get files from?
 
     Examples:
         pip.compile .
         pip.compile ./requirements.in
     """
+    paths = path
+    for path in paths:
+        files = _find_infiles(Path(path))
 
-    files = _find_infiles(Path(path))
-
-    args = {}
+        args = {}
 
-    if pypi_server:
-        args["i"] = pypi_server
+        if pypi_server:
+            args["i"] = pypi_server
 
-    for file in files:
-        _pip_compile(file, **args)
+        for file in files:
+            _pip_compile(file, **args)
 
-        success(f"Ran pip-compile! Check {in_to_out(file)}")
+            success(f"Ran pip-compile! Check {in_to_out(file)}")
 
 
 @task()
 def install(ctx, path, package, pypi_server=DEFAULT_SERVER):
     """
     Install a package to the .in file of the specified directory and re-compile the requirements.txt
     The command also checks if the command is already added and if it exists on the specified pypi server
```

### Comparing `edwh_pipcompile_plugin-0.1.7/LICENSE.txt` & `edwh_pipcompile_plugin-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.7/README.md` & `edwh_pipcompile_plugin-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.7/pyproject.toml` & `edwh_pipcompile_plugin-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.7/PKG-INFO` & `edwh_pipcompile_plugin-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.1.7
+Version: 0.1.8
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

