# Comparing `tmp/cpmax_toolbox-0.3.6.tar.gz` & `tmp/cpmax_toolbox-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpmax_toolbox-0.3.6.tar", max compression
+gzip compressed data, was "cpmax_toolbox-0.3.7.tar", max compression
```

## Comparing `cpmax_toolbox-0.3.6.tar` & `cpmax_toolbox-0.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       38 2023-02-01 12:56:05.830314 cpmax_toolbox-0.3.6/cpmax_toolbox/__init__.py
--rw-r--r--   0        0        0     6451 2023-03-23 22:03:22.851073 cpmax_toolbox-0.3.6/cpmax_toolbox/analyzing.py
--rw-r--r--   0        0        0    10026 2023-05-04 09:27:13.128389 cpmax_toolbox-0.3.6/cpmax_toolbox/file_repair.py
--rw-r--r--   0        0        0    13047 2023-02-28 12:35:49.809546 cpmax_toolbox-0.3.6/cpmax_toolbox/vib_measurement.py
--rw-r--r--   0        0        0      529 2023-05-04 09:28:17.246316 cpmax_toolbox-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-01 08:47:07.339719 cpmax_toolbox-0.3.6/README.md
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.6/setup.py
--rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-02-01 12:56:05.830314 cpmax_toolbox-0.3.7/cpmax_toolbox/__init__.py
+-rw-r--r--   0        0        0     6451 2023-03-23 22:03:22.851073 cpmax_toolbox-0.3.7/cpmax_toolbox/analyzing.py
+-rw-r--r--   0        0        0    10026 2023-05-04 09:27:13.128389 cpmax_toolbox-0.3.7/cpmax_toolbox/file_repair.py
+-rw-r--r--   0        0        0    13047 2023-02-28 12:35:49.809546 cpmax_toolbox-0.3.7/cpmax_toolbox/vib_measurement.py
+-rw-r--r--   0        0        0      530 2023-05-04 09:59:03.045229 cpmax_toolbox-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-01 08:47:07.339719 cpmax_toolbox-0.3.7/README.md
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.7/setup.py
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 cpmax_toolbox-0.3.7/PKG-INFO
```

### Comparing `cpmax_toolbox-0.3.6/cpmax_toolbox/analyzing.py` & `cpmax_toolbox-0.3.7/cpmax_toolbox/analyzing.py`

 * *Files identical despite different names*

### Comparing `cpmax_toolbox-0.3.6/cpmax_toolbox/file_repair.py` & `cpmax_toolbox-0.3.7/cpmax_toolbox/file_repair.py`

 * *Files identical despite different names*

### Comparing `cpmax_toolbox-0.3.6/cpmax_toolbox/vib_measurement.py` & `cpmax_toolbox-0.3.7/cpmax_toolbox/vib_measurement.py`

 * *Files identical despite different names*

### Comparing `cpmax_toolbox-0.3.6/pyproject.toml` & `cpmax_toolbox-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "cpmax-toolbox"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 authors = ["JRoseCPMax <j.rose@cpmax.com>"]
 readme = "README.md"
 packages = [{include = "cpmax_toolbox"}]
 
 [tool.poetry.dependencies]
-python = ">3.8,<3.9"
+python = ">=3.8,<3.9"
 requests = "^2.28.2"
 pytz = "^2022.7.1"
 pandas = "^1.5.3"
 scipy = "^1.10.1"
 rich = "^13.3.1"
 matplotlib = "^3.7.0"
```

### Comparing `cpmax_toolbox-0.3.6/setup.py` & `cpmax_toolbox-0.3.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,23 +13,23 @@
  'pytz>=2022.7.1,<2023.0.0',
  'requests>=2.28.2,<3.0.0',
  'rich>=13.3.1,<14.0.0',
  'scipy>=1.10.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'cpmax-toolbox',
-    'version': '0.3.6',
+    'version': '0.3.7',
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
-    'python_requires': '>3.8,<3.9',
+    'python_requires': '>=3.8,<3.9',
 }
 
 
 setup(**setup_kwargs)
```

