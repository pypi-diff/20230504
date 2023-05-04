# Comparing `tmp/fastapi_featureflags-0.4.7.tar.gz` & `tmp/fastapi_featureflags-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_featureflags-0.4.7.tar", last modified: Thu Mar  9 13:54:03 2023, max compression
+gzip compressed data, was "fastapi_featureflags-0.4.8.tar", max compression
```

## Comparing `fastapi_featureflags-0.4.7.tar` & `fastapi_featureflags-0.4.8.tar`

### file list

```diff
@@ -1,26 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/fastapi_featureflags/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/fastapi_featureflags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/fastapi_featureflags/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/fastapi_featureflags/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_conf_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_conf_from_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_conf_from_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_types.py
+-rw-r--r--   0        0        0     1068 2023-05-04 08:22:30.915134 fastapi_featureflags-0.4.8/LICENSE
+-rw-r--r--   0        0        0     3855 2023-05-04 08:22:30.915134 fastapi_featureflags-0.4.8/README.md
+-rw-r--r--   0        0        0       89 2023-05-04 08:22:30.915134 fastapi_featureflags-0.4.8/fastapi_featureflags/__init__.py
+-rw-r--r--   0        0        0     6284 2023-05-04 08:22:30.915134 fastapi_featureflags-0.4.8/fastapi_featureflags/main.py
+-rw-r--r--   0        0        0     1067 2023-05-04 08:22:30.915134 fastapi_featureflags-0.4.8/fastapi_featureflags/router.py
+-rw-r--r--   0        0        0     1400 2023-05-04 08:22:55.444660 fastapi_featureflags-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     4682 1970-01-01 00:00:00.000000 fastapi_featureflags-0.4.8/PKG-INFO
```

### Comparing `fastapi_featureflags-0.4.7/LICENSE` & `fastapi_featureflags-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.7/PKG-INFO` & `fastapi_featureflags-0.4.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
-Name: fastapi_featureflags
-Version: 0.4.7
+Name: fastapi-featureflags
+Version: 0.4.8
 Summary: Feature Flags for FastAPI
-Home-page: https://github.com/Pytlicek/fastapi-featureflags
 Author: Tomas Pytel
 Author-email: pytlicek@gmail.com
-Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7,<=3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: fastapi (>=0.95.1,<0.96.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
+Project-URL: Homepage, https://github.com/Pytlicek/ fastapi-featureflags
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![Test Python package](https://github.com/Pytlicek/fastapi-featureflags/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/Pytlicek/fastapi-featureflags/actions/workflows/python-package.yml) 
 [![codecov](https://codecov.io/gh/Pytlicek/fastapi-featureflags/branch/main/graph/badge.svg?token=CVULQJ2SSA)](https://codecov.io/gh/Pytlicek/fastapi-featureflags) 
 [![Upload Python Package to PyPI](https://github.com/Pytlicek/fastapi-featureflags/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Pytlicek/fastapi-featureflags/actions/workflows/python-publish.yml) 
 ![PythonVersions](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue) 
 [![Sourcery](https://img.shields.io/badge/Sourcery-enabled-brightgreen)](https://sourcery.ai) 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) 
@@ -87,7 +94,8 @@
 ### Contributing to fastapi-featureflags  
 As an open source project, fastapi-featureflags welcomes contributions of many forms.  
 Please read and follow our [Contributing to fastapi-featureflags](CONTRIBUTING.md)  
 
 ### Code of Conduct  
 As a contributor, you can help us keep the fastapi-featureflags project open and inclusive.  
 Please read and follow our [Code of Conduct](CODE_OF_CONDUCT.md)  
+
```

### Comparing `fastapi_featureflags-0.4.7/README.md` & `fastapi_featureflags-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.7/fastapi_featureflags/router.py` & `fastapi_featureflags-0.4.8/fastapi_featureflags/router.py`

 * *Files identical despite different names*

