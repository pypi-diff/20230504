# Comparing `tmp/stats_can-2.5.1.tar.gz` & `tmp/stats_can-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stats_can-2.5.1.tar", max compression
+gzip compressed data, was "stats_can-2.5.3.tar", max compression
```

## Comparing `stats_can-2.5.1.tar` & `stats_can-2.5.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35147 2021-03-11 01:57:22.754868 stats_can-2.5.1/LICENSE
--rw-r--r--   0        0        0     1076 2021-03-11 01:57:22.754868 stats_can-2.5.1/README.md
--rw-r--r--   0        0        0     1383 2021-03-11 01:57:22.758868 stats_can-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     1023 2021-03-11 01:57:22.758868 stats_can-2.5.1/src/stats_can/__init__.py
--rw-r--r--   0        0        0     7518 2021-03-11 01:57:22.758868 stats_can-2.5.1/src/stats_can/api_class.py
--rw-r--r--   0        0        0     3429 2021-03-11 01:57:22.758868 stats_can-2.5.1/src/stats_can/helpers.py
--rw-r--r--   0        0        0    22417 2021-03-11 01:57:22.758868 stats_can-2.5.1/src/stats_can/sc.py
--rw-r--r--   0        0        0     7190 2021-03-11 01:57:22.758868 stats_can-2.5.1/src/stats_can/scwds.py
--rw-r--r--   0        0        0     2032 2021-03-11 01:57:32.442753 stats_can-2.5.1/setup.py
--rw-r--r--   0        0        0     2073 2021-03-11 01:57:32.443122 stats_can-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-05-03 22:48:46.334181 stats_can-2.5.3/LICENSE
+-rw-r--r--   0        0        0     1076 2023-05-03 22:48:46.334181 stats_can-2.5.3/README.md
+-rw-r--r--   0        0        0     1383 2023-05-03 22:48:46.334181 stats_can-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1023 2023-05-03 22:48:46.334181 stats_can-2.5.3/src/stats_can/__init__.py
+-rw-r--r--   0        0        0     7518 2023-05-03 22:48:46.334181 stats_can-2.5.3/src/stats_can/api_class.py
+-rw-r--r--   0        0        0     3429 2023-05-03 22:48:46.334181 stats_can-2.5.3/src/stats_can/helpers.py
+-rw-r--r--   0        0        0    22417 2023-05-03 22:48:46.334181 stats_can-2.5.3/src/stats_can/sc.py
+-rw-r--r--   0        0        0     7190 2023-05-03 22:48:46.338181 stats_can-2.5.3/src/stats_can/scwds.py
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 stats_can-2.5.3/setup.py
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 stats_can-2.5.3/PKG-INFO
```

### Comparing `stats_can-2.5.1/LICENSE` & `stats_can-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stats_can-2.5.1/README.md` & `stats_can-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `stats_can-2.5.1/pyproject.toml` & `stats_can-2.5.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 [tool.poetry]
 name = "stats_can"
-version = "2.5.1"
+version = "2.5.3"
 description = "Read StatsCan data into python, mostly pandas dataframes"
 authors = ["Ian Preston"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/ianepreston/stats_can"
 repository = "https://github.com/ianepreston/stats_can"
 documentation = "https://stats-can.readthedocs.io"
 keywords = ["statistics", "Canada", "data", "API"]
 
 [tool.poetry.dependencies]
-python = ">=3.6.1,<4.0"
-requests = "^2.20"
-h5py = ">=2.10,<4.0"
-tables = "^3.6.1"
-tqdm = "^4.48.0"
-pandas = "^1.1.0"
-importlib_metadata = {version = ">=1.7,<4.0", python = "<3.8"}
+python = ">=3.8,<4.0"
+requests = ">=2.20"
+h5py = ">=2.10"
+tables = ">=3.6"
+tqdm = ">=4.48"
+pandas = ">=1.1"
+importlib-metadata = ">=6.0.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.2"
-flake8 = "^3.8.3"
-pandas-vet = "^0.2.2"
-black = "^20.8b1"
-coverage = {extras = ["toml"], version = "^5.4"}
-pytest-cov = "^2.11.1"
-codecov = "^2.1.8"
-flake8-bandit = "^2.1.2"
-flake8-bugbear = "^21.3.2"
-flake8-black = "^0.2.1"
-flake8-import-order = "^0.18.1"
-pytest-vcr = "^1.0.2"
-flake8-docstrings = "^1.5.0"
-sphinx = "^3.5.1"
-darglint = "^1.7.0"
-xdoctest = "^0.15.3"
-sphinx-autodoc-typehints = "^1.11.0"
-sphinx_rtd_theme = "^0.5.0"
-safety = "^1.9.0"
-freezegun = "^1.1.0"
+pytest = ">=7.3"
+flake8 = ">=5.0"
+pandas-vet = ">=0.2"
+black = ">=22.12"
+coverage = {extras = ["toml"], version = ">=7.2"}
+pytest-cov = ">=4.0"
+codecov = ">=2.1"
+flake8-bandit = ">=4.1"
+flake8-bugbear = ">=23.3"
+flake8-black = ">=0.3"
+flake8-import-order = ">=0.18"
+pytest-vcr = ">=1.0"
+flake8-docstrings = ">=1.7"
+sphinx = ">=6.1"
+darglint = ">=1.7"
+xdoctest = ">=1.1"
+sphinx-autodoc-typehints = ">=1.23"
+sphinx_rtd_theme = ">=1.2"
+safety = ">=2.3"
+freezegun = ">=1.2"
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = ">=2.21"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.run]
 branch = true
 source = ["stats_can"]
```

### Comparing `stats_can-2.5.1/src/stats_can/__init__.py` & `stats_can-2.5.3/src/stats_can/__init__.py`

 * *Files identical despite different names*

### Comparing `stats_can-2.5.1/src/stats_can/api_class.py` & `stats_can-2.5.3/src/stats_can/api_class.py`

 * *Files identical despite different names*

### Comparing `stats_can-2.5.1/src/stats_can/helpers.py` & `stats_can-2.5.3/src/stats_can/helpers.py`

 * *Files identical despite different names*

### Comparing `stats_can-2.5.1/src/stats_can/sc.py` & `stats_can-2.5.3/src/stats_can/sc.py`

 * *Files identical despite different names*

### Comparing `stats_can-2.5.1/src/stats_can/scwds.py` & `stats_can-2.5.3/src/stats_can/scwds.py`

 * *Files identical despite different names*

### Comparing `stats_can-2.5.1/setup.py` & `stats_can-2.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,36 +7,33 @@
 packages = \
 ['stats_can']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['h5py>=2.10,<4.0',
- 'pandas>=1.1.0,<2.0.0',
- 'requests>=2.20,<3.0',
- 'tables>=3.6.1,<4.0.0',
- 'tqdm>=4.48.0,<5.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib_metadata>=1.7,<4.0']}
+['h5py>=2.10',
+ 'importlib-metadata>=6.0.0',
+ 'pandas>=1.1',
+ 'requests>=2.20',
+ 'tables>=3.6',
+ 'tqdm>=4.48']
 
 setup_kwargs = {
     'name': 'stats-can',
-    'version': '2.5.1',
+    'version': '2.5.3',
     'description': 'Read StatsCan data into python, mostly pandas dataframes',
     'long_description': "# Python api for Statistics Canada New Data Model (NDM)\n\n[![Tests](https://github.com/ianepreston/stats_can/workflows/Tests/badge.svg)](https://github.com/ianepreston/stats_can/actions?workflow=Tests)\n[![Documentation Status](https://readthedocs.org/projects/stats-can/badge/?version=latest)](https://stats-can.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/ianepreston/stats_can/branch/master/graph/badge.svg)](https://codecov.io/gh/ianepreston/stats_can)\n[![PyPI version](https://badge.fury.io/py/stats-can.svg)](https://badge.fury.io/py/stats-can)\n[![Anaconda-Server Badge](https://anaconda.org/conda-forge/stats_can/badges/version.svg)](https://anaconda.org/conda-forge/stats_can)\n\nAPI documentation for StatsCan can be found here: https://www.statcan.gc.ca/eng/developers/wds\n\nIf you're looking for Table/Vector IDs to use in the app you can find them through this:\nhttps://www150.statcan.gc.ca/n1/en/type/data\n\nAnaconda package here:\nhttps://anaconda.org/conda-forge/stats_can\n\n\nDocumentation here:\nhttps://stats-can.readthedocs.io/en/latest/\n",
     'author': 'Ian Preston',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/ianepreston/stats_can',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6.1,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `stats_can-2.5.1/PKG-INFO` & `stats_can-2.5.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: stats-can
-Version: 2.5.1
+Version: 2.5.3
 Summary: Read StatsCan data into python, mostly pandas dataframes
 Home-page: https://github.com/ianepreston/stats_can
 License: GPL-3.0-or-later
 Keywords: statistics,Canada,data,API
 Author: Ian Preston
-Requires-Python: >=3.6.1,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: h5py (>=2.10,<4.0)
-Requires-Dist: importlib_metadata (>=1.7,<4.0); python_version < "3.8"
-Requires-Dist: pandas (>=1.1.0,<2.0.0)
-Requires-Dist: requests (>=2.20,<3.0)
-Requires-Dist: tables (>=3.6.1,<4.0.0)
-Requires-Dist: tqdm (>=4.48.0,<5.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: h5py (>=2.10)
+Requires-Dist: importlib-metadata (>=6.0.0)
+Requires-Dist: pandas (>=1.1)
+Requires-Dist: requests (>=2.20)
+Requires-Dist: tables (>=3.6)
+Requires-Dist: tqdm (>=4.48)
 Project-URL: Documentation, https://stats-can.readthedocs.io
 Project-URL: Repository, https://github.com/ianepreston/stats_can
 Description-Content-Type: text/markdown
 
 # Python api for Statistics Canada New Data Model (NDM)
 
 [![Tests](https://github.com/ianepreston/stats_can/workflows/Tests/badge.svg)](https://github.com/ianepreston/stats_can/actions?workflow=Tests)
```

