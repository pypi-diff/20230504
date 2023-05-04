# Comparing `tmp/robin_sd_download-0.3.4.tar.gz` & `tmp/robin_sd_download-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robin_sd_download-0.3.4.tar", last modified: Thu May  4 12:27:47 2023, max compression
+gzip compressed data, was "dist/robin_sd_download-0.3.5.tar", last modified: Thu May  4 12:56:37 2023, max compression
```

## Comparing `robin_sd_download-0.3.4.tar` & `robin_sd_download-0.3.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download/api_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/api_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/api_interaction/get_bearer_token.py
--rw-rw-rw-   0 root         (0) root         (0)     5452 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/api_interaction/get_software.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/api_interaction/get_software_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download/apt_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/apt_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1895 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/apt_interaction/ensure_hook.py
--rw-rw-rw-   0 root         (0) root         (0)     3864 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/apt_interaction/ensure_local_repo.py
--rw-rw-rw-   0 root         (0) root         (0)    15269 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/apt_interaction/offline_install.py
--rw-rw-rw-   0 root         (0) root         (0)     4768 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/apt_interaction/prepare_install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download/slack_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/slack_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2952 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/slack_interaction/slack_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/arg_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2220 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/sudo_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/version_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     5108 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1254 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/robin_sd_download.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:27:47.000000 robin_sd_download-0.3.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3747 2023-05-04 12:27:29.000000 robin_sd_download-0.3.4/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_bearer_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     5452 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_software.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_software_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/ensure_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)     3864 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/ensure_local_repo.py
+-rw-rw-rw-   0 root         (0) root         (0)    15269 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/offline_install.py
+-rw-rw-rw-   0 root         (0) root         (0)     4768 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/apt_interaction/prepare_install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/slack_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/slack_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/slack_interaction/slack_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/arg_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/sudo_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     2099 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/version_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5108 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/robin_sd_download.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 12:56:37.000000 robin_sd_download-0.3.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3747 2023-05-04 12:56:19.000000 robin_sd_download-0.3.5/tests/test.py
```

### Comparing `robin_sd_download-0.3.4/PKG-INFO` & `robin_sd_download-0.3.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_sd_download
-Version: 0.3.4
+Version: 0.3.5
 Summary: Package to download files to the Robin Radar API
 Home-page: https://bitbucket.org/robin-radar-systems/sd-api-download-pip-package.git
 Author: Robin Radar Systems
 Author-email: it-team@robinradar.com
 License: MIT
 Description: # robin-sd-download
```

### Comparing `robin_sd_download-0.3.4/robin_sd_download/api_interaction/get_bearer_token.py` & `robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_bearer_token.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/api_interaction/get_software.py` & `robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_software.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/api_interaction/get_software_info.py` & `robin_sd_download-0.3.5/robin_sd_download/api_interaction/get_software_info.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/apt_interaction/ensure_hook.py` & `robin_sd_download-0.3.5/robin_sd_download/apt_interaction/ensure_hook.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/apt_interaction/ensure_local_repo.py` & `robin_sd_download-0.3.5/robin_sd_download/apt_interaction/ensure_local_repo.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/apt_interaction/offline_install.py` & `robin_sd_download-0.3.5/robin_sd_download/apt_interaction/offline_install.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/apt_interaction/prepare_install.py` & `robin_sd_download-0.3.5/robin_sd_download/apt_interaction/prepare_install.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/slack_interaction/slack_handler.py` & `robin_sd_download-0.3.5/robin_sd_download/slack_interaction/slack_handler.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/arg_parse.py` & `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/arg_parse.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/logger.py` & `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/logger.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/sudo_file.py` & `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/sudo_file.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/version_checker.py` & `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/version_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 from pypi_simple.util import UnexpectedRepoVersionWarning
 
 from robin_sd_download.supportive_scripts import logger
 from robin_sd_download.supportive_scripts import yaml_parser
 from robin_sd_download import _version
 
 
-def check_latest_version(package_name: str = "robin-sd-download"):
+def check_latest_version():
     """Check if the latest version is installed and document how to update if needed."""
     config = yaml_parser.parse_config()
 
+    package_name = config['static']['app_name']
+
     current_version = _version.__version__
 
     pypi = PyPISimple()
 
     try:
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter(
```

### Comparing `robin_sd_download-0.3.4/robin_sd_download/supportive_scripts/yaml_parser.py` & `robin_sd_download-0.3.5/robin_sd_download/supportive_scripts/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/robin_sd_download.egg-info/PKG-INFO` & `robin_sd_download-0.3.5/robin_sd_download.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-sd-download
-Version: 0.3.4
+Version: 0.3.5
 Summary: Package to download files to the Robin Radar API
 Home-page: https://bitbucket.org/robin-radar-systems/sd-api-download-pip-package.git
 Author: Robin Radar Systems
 Author-email: it-team@robinradar.com
 License: MIT
 Description: # robin-sd-download
```

### Comparing `robin_sd_download-0.3.4/robin_sd_download.egg-info/SOURCES.txt` & `robin_sd_download-0.3.5/robin_sd_download.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/setup.py` & `robin_sd_download-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `robin_sd_download-0.3.4/tests/test.py` & `robin_sd_download-0.3.5/tests/test.py`

 * *Files identical despite different names*

