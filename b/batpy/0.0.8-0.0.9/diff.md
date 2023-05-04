# Comparing `tmp/batpy-0.0.8.tar.gz` & `tmp/batpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batpy-0.0.8.tar", max compression
+gzip compressed data, was "batpy-0.0.9.tar", max compression
```

## Comparing `batpy-0.0.8.tar` & `batpy-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1073 2023-05-03 16:25:10.787139 batpy-0.0.8/LICENSE
--rw-r--r--   0        0        0     4365 2023-05-03 16:25:10.787139 batpy-0.0.8/README.md
--rw-r--r--   0        0        0     1825 2023-05-03 16:26:03.139271 batpy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      172 2023-05-03 16:25:10.791139 batpy-0.0.8/src/batpy/__init__.py
--rw-r--r--   0        0        0     5157 2023-05-03 16:25:10.791139 batpy-0.0.8/src/batpy/batpac_battery.py
--rw-r--r--   0        0        0    27747 2023-05-03 16:25:10.791139 batpy-0.0.8/src/batpy/batpac_tool.py
--rw-r--r--   0        0        0     2158 2023-05-03 16:25:10.791139 batpy-0.0.8/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml
--rw-r--r--   0        0        0    30586 2023-05-03 16:25:10.791139 batpy-0.0.8/src/batpy/data/batpy_batpac_config.toml
--rw-r--r--   0        0        0    83193 2023-05-03 16:25:10.791139 batpy-0.0.8/src/batpy/data/batpy_batpac_user_input_cells.toml
--rw-r--r--   0        0        0    48369 2023-05-03 16:25:10.795139 batpy-0.0.8/src/batpy/data/batpy_batteries_config.toml
--rw-r--r--   0        0        0     2177 2023-05-03 16:25:10.795139 batpy-0.0.8/src/batpy/is_version_compatible.py
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 batpy-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-04 11:50:54.051104 batpy-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4365 2023-05-04 11:50:54.051104 batpy-0.0.9/README.md
+-rw-r--r--   0        0        0     1825 2023-05-04 11:51:27.531087 batpy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/__init__.py
+-rw-r--r--   0        0        0     5157 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/batpac_battery.py
+-rw-r--r--   0        0        0    27747 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/batpac_tool.py
+-rw-r--r--   0        0        0     2158 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    30586 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/data/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    83193 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/data/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    48369 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/data/batpy_batteries_config.toml
+-rw-r--r--   0        0        0     2177 2023-05-04 11:50:54.055104 batpy-0.0.9/src/batpy/is_version_compatible.py
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 batpy-0.0.9/PKG-INFO
```

### Comparing `batpy-0.0.8/LICENSE` & `batpy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `batpy-0.0.8/README.md` & `batpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `batpy-0.0.8/pyproject.toml` & `batpy-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batpy"
-version = "0.0.8"
+version = "0.0.9"
 description = "A python package to read, write, and calculate batteries in the BatPaC tool."
 authors = ["Raphael Ginster <r.ginster@tu-braunschweig.de>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://rginster.github.io/batpy/"
 repository = "https://github.com/rginster/batpy"
```

### Comparing `batpy-0.0.8/src/batpy/batpac_battery.py` & `batpy-0.0.9/src/batpy/batpac_battery.py`

 * *Files identical despite different names*

### Comparing `batpy-0.0.8/src/batpy/batpac_tool.py` & `batpy-0.0.9/src/batpy/batpac_tool.py`

 * *Files identical despite different names*

### Comparing `batpy-0.0.8/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml` & `batpy-0.0.9/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.8/src/batpy/data/batpy_batpac_config.toml` & `batpy-0.0.9/src/batpy/data/batpy_batpac_config.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.8/src/batpy/data/batpy_batpac_user_input_cells.toml` & `batpy-0.0.9/src/batpy/data/batpy_batpac_user_input_cells.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.8/src/batpy/data/batpy_batteries_config.toml` & `batpy-0.0.9/src/batpy/data/batpy_batteries_config.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.8/src/batpy/is_version_compatible.py` & `batpy-0.0.9/src/batpy/is_version_compatible.py`

 * *Files identical despite different names*

### Comparing `batpy-0.0.8/PKG-INFO` & `batpy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package to read, write, and calculate batteries in the BatPaC tool.
 Home-page: https://github.com/rginster/batpy
 License: MIT
 Author: Raphael Ginster
 Author-email: r.ginster@tu-braunschweig.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

