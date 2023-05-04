# Comparing `tmp/fastapi_featureflags-0.4.6.tar.gz` & `tmp/fastapi_featureflags-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_featureflags-0.4.6.tar", last modified: Mon Apr 18 15:23:44 2022, max compression
+gzip compressed data, was "fastapi_featureflags-0.4.7.tar", last modified: Thu Mar  9 13:54:03 2023, max compression
```

## Comparing `fastapi_featureflags-0.4.6.tar` & `fastapi_featureflags-0.4.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 15:23:44.042069 fastapi_featureflags-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-04-18 15:23:44.042069 fastapi_featureflags-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 15:23:44.038069 fastapi_featureflags-0.4.6/fastapi_featureflags/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/fastapi_featureflags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/fastapi_featureflags/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/fastapi_featureflags/router.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 15:23:44.042069 fastapi_featureflags-0.4.6/fastapi_featureflags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-04-18 15:23:43.000000 fastapi_featureflags-0.4.6/fastapi_featureflags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-04-18 15:23:43.000000 fastapi_featureflags-0.4.6/fastapi_featureflags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-18 15:23:43.000000 fastapi_featureflags-0.4.6/fastapi_featureflags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-04-18 15:23:43.000000 fastapi_featureflags-0.4.6/fastapi_featureflags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-04-18 15:23:43.000000 fastapi_featureflags-0.4.6/fastapi_featureflags.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-18 15:23:44.042069 fastapi_featureflags-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 15:23:44.042069 fastapi_featureflags-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/tests/test_conf_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/tests/test_conf_from_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/tests/test_conf_from_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-04-18 15:23:30.000000 fastapi_featureflags-0.4.6/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/fastapi_featureflags/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/fastapi_featureflags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/fastapi_featureflags/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/fastapi_featureflags/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-09 13:54:02.000000 fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 13:54:03.025367 fastapi_featureflags-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_conf_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_conf_from_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_conf_from_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-09 13:53:41.000000 fastapi_featureflags-0.4.7/tests/test_types.py
```

### Comparing `fastapi_featureflags-0.4.6/LICENSE` & `fastapi_featureflags-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/PKG-INFO` & `fastapi_featureflags-0.4.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: fastapi_featureflags
-Version: 0.4.6
+Version: 0.4.7
 Summary: Feature Flags for FastAPI
 Home-page: https://github.com/Pytlicek/fastapi-featureflags
 Author: Tomas Pytel
 Author-email: pytlicek@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -89,9 +87,7 @@
 ### Contributing to fastapi-featureflags  
 As an open source project, fastapi-featureflags welcomes contributions of many forms.  
 Please read and follow our [Contributing to fastapi-featureflags](CONTRIBUTING.md)  
 
 ### Code of Conduct  
 As a contributor, you can help us keep the fastapi-featureflags project open and inclusive.  
 Please read and follow our [Code of Conduct](CODE_OF_CONDUCT.md)  
-
-
```

### Comparing `fastapi_featureflags-0.4.6/README.md` & `fastapi_featureflags-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/fastapi_featureflags/main.py` & `fastapi_featureflags-0.4.7/fastapi_featureflags/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/fastapi_featureflags/router.py` & `fastapi_featureflags-0.4.7/fastapi_featureflags/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/fastapi_featureflags.egg-info/PKG-INFO` & `fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: fastapi-featureflags
-Version: 0.4.6
+Version: 0.4.7
 Summary: Feature Flags for FastAPI
 Home-page: https://github.com/Pytlicek/fastapi-featureflags
 Author: Tomas Pytel
 Author-email: pytlicek@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -89,9 +87,7 @@
 ### Contributing to fastapi-featureflags  
 As an open source project, fastapi-featureflags welcomes contributions of many forms.  
 Please read and follow our [Contributing to fastapi-featureflags](CONTRIBUTING.md)  
 
 ### Code of Conduct  
 As a contributor, you can help us keep the fastapi-featureflags project open and inclusive.  
 Please read and follow our [Code of Conduct](CODE_OF_CONDUCT.md)  
-
-
```

### Comparing `fastapi_featureflags-0.4.6/fastapi_featureflags.egg-info/SOURCES.txt` & `fastapi_featureflags-0.4.7/fastapi_featureflags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/setup.py` & `fastapi_featureflags-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastapi_featureflags",
-    version="0.4.6",
+    version="0.4.7",
     author="Tomas Pytel",
     author_email="pytlicek@gmail.com",
     description="Feature Flags for FastAPI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Pytlicek/fastapi-featureflags",
     packages=setuptools.find_packages(),
```

### Comparing `fastapi_featureflags-0.4.6/tests/conftest.py` & `fastapi_featureflags-0.4.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/tests/test_conf.py` & `fastapi_featureflags-0.4.7/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/tests/test_conf_from_dict.py` & `fastapi_featureflags-0.4.7/tests/test_conf_from_dict.py`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/tests/test_conf_from_json.py` & `fastapi_featureflags-0.4.7/tests/test_conf_from_json.py`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/tests/test_conf_from_url.py` & `fastapi_featureflags-0.4.7/tests/test_conf_from_url.py`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/tests/test_routes.py` & `fastapi_featureflags-0.4.7/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `fastapi_featureflags-0.4.6/tests/test_types.py` & `fastapi_featureflags-0.4.7/tests/test_types.py`

 * *Files identical despite different names*

