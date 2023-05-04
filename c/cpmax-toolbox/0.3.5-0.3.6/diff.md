# Comparing `tmp/cpmax_toolbox-0.3.5.tar.gz` & `tmp/cpmax_toolbox-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpmax_toolbox-0.3.5.tar", max compression
+gzip compressed data, was "cpmax_toolbox-0.3.6.tar", max compression
```

## Comparing `cpmax_toolbox-0.3.5.tar` & `cpmax_toolbox-0.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       38 2023-02-01 12:56:05.830314 cpmax_toolbox-0.3.5/cpmax_toolbox/__init__.py
--rw-r--r--   0        0        0     6451 2023-03-23 22:03:22.851073 cpmax_toolbox-0.3.5/cpmax_toolbox/analyzing.py
--rw-r--r--   0        0        0     9981 2023-03-14 13:57:32.685343 cpmax_toolbox-0.3.5/cpmax_toolbox/file_repair.py
--rw-r--r--   0        0        0    13047 2023-02-28 12:35:49.809546 cpmax_toolbox-0.3.5/cpmax_toolbox/vib_measurement.py
--rw-r--r--   0        0        0      531 2023-04-20 12:16:17.114416 cpmax_toolbox-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-01 08:47:07.339719 cpmax_toolbox-0.3.5/README.md
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.5/setup.py
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-02-01 12:56:05.830314 cpmax_toolbox-0.3.6/cpmax_toolbox/__init__.py
+-rw-r--r--   0        0        0     6451 2023-03-23 22:03:22.851073 cpmax_toolbox-0.3.6/cpmax_toolbox/analyzing.py
+-rw-r--r--   0        0        0    10026 2023-05-04 09:27:13.128389 cpmax_toolbox-0.3.6/cpmax_toolbox/file_repair.py
+-rw-r--r--   0        0        0    13047 2023-02-28 12:35:49.809546 cpmax_toolbox-0.3.6/cpmax_toolbox/vib_measurement.py
+-rw-r--r--   0        0        0      529 2023-05-04 09:28:17.246316 cpmax_toolbox-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-01 08:47:07.339719 cpmax_toolbox-0.3.6/README.md
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.6/setup.py
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.6/PKG-INFO
```

### Comparing `cpmax_toolbox-0.3.5/cpmax_toolbox/analyzing.py` & `cpmax_toolbox-0.3.6/cpmax_toolbox/analyzing.py`

 * *Files identical despite different names*

### Comparing `cpmax_toolbox-0.3.5/cpmax_toolbox/file_repair.py` & `cpmax_toolbox-0.3.6/cpmax_toolbox/file_repair.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         return "new_nanovib_recording"
 
     raise ValueError(
         f"Unknown format, cols are {cols_set} and header is {i} lines long"
     )
 
 
-def repair_file(p: typing.Union[Path, str]) -> Path:
+def repair_file(p: typing.Union[Path, str], correct_axis: bool = False) -> Path:
     """
     TODO test with broken files -> create broken files
 
     repair broken file and return viba ready file.
     possible types:
         sqlite_export -> fs?
         old_nanovib_recording
@@ -252,15 +252,15 @@
     geo_mean = (ax_mean**2 + rad_mean**2 + tor_mean**2) ** (1 / 2)
 
     logging.info(f"Mean Values - Geometric: {geo_mean:.2f}")
     tor_ratio = abs(tor_mean) / geo_mean
 
     logging.debug(f"Mean Values - Torsional Ratio: {tor_ratio:.2f}")
 
-    if tor_ratio < 0.9:
+    if tor_ratio < 0.9 and correct_axis:
         ax_ratio = abs(ax_mean) / geo_mean
         rad_ratio = abs(rad_mean) / geo_mean
         fitting_ax = "Axial" if ax_ratio > rad_ratio else "Radial"
 
         print(
             f"Torsionsachse zeigt nicht nach unten, stattdessen wird {fitting_ax} genutzt."
         )
```

### Comparing `cpmax_toolbox-0.3.5/cpmax_toolbox/vib_measurement.py` & `cpmax_toolbox-0.3.6/cpmax_toolbox/vib_measurement.py`

 * *Files identical despite different names*

### Comparing `cpmax_toolbox-0.3.5/pyproject.toml` & `cpmax_toolbox-0.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "cpmax-toolbox"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = ["JRoseCPMax <j.rose@cpmax.com>"]
 readme = "README.md"
 packages = [{include = "cpmax_toolbox"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">3.8,<3.9"
 requests = "^2.28.2"
 pytz = "^2022.7.1"
 pandas = "^1.5.3"
 scipy = "^1.10.1"
 rich = "^13.3.1"
 matplotlib = "^3.7.0"
```

### Comparing `cpmax_toolbox-0.3.5/setup.py` & `cpmax_toolbox-0.3.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,23 +13,23 @@
  'pytz>=2022.7.1,<2023.0.0',
  'requests>=2.28.2,<3.0.0',
  'rich>=13.3.1,<14.0.0',
  'scipy>=1.10.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'cpmax-toolbox',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': '',
     'long_description': '',
     'author': 'JRoseCPMax',
     'author_email': 'j.rose@cpmax.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
+    'python_requires': '>3.8,<3.9',
 }
 
 
 setup(**setup_kwargs)
```

