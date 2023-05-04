# Comparing `tmp/PyTestLog2DB-0.2.4.tar.gz` & `tmp/PyTestLog2DB-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTestLog2DB-0.2.4.tar", last modified: Fri Apr 28 12:43:12 2023, max compression
+gzip compressed data, was "PyTestLog2DB-0.2.5.tar", last modified: Thu May  4 13:03:47 2023, max compression
```

## Comparing `PyTestLog2DB-0.2.4.tar` & `PyTestLog2DB-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:43:12.242620 PyTestLog2DB-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-28 12:43:12.242620 PyTestLog2DB-0.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:43:12.238620 PyTestLog2DB-0.2.4/PyTestLog2DB/
--rw-r--r--   0 runner    (1001) docker     (123)    42027 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/PyTestLog2DB/CDataBase.py
--rw-r--r--   0 runner    (1001) docker     (123)   606378 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/PyTestLog2DB/PyTestLog2DB.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/PyTestLog2DB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/PyTestLog2DB/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43431 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/PyTestLog2DB/pytestlog2db.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/PyTestLog2DB/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:43:12.242620 PyTestLog2DB-0.2.4/PyTestLog2DB/xsd/
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/PyTestLog2DB/xsd/junit.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:43:12.242620 PyTestLog2DB-0.2.4/PyTestLog2DB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-28 12:43:12.000000 PyTestLog2DB-0.2.4/PyTestLog2DB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 12:43:12.000000 PyTestLog2DB-0.2.4/PyTestLog2DB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:43:12.000000 PyTestLog2DB-0.2.4/PyTestLog2DB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 12:43:12.000000 PyTestLog2DB-0.2.4/PyTestLog2DB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 12:43:12.000000 PyTestLog2DB-0.2.4/PyTestLog2DB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:43:12.242620 PyTestLog2DB-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-28 12:41:01.000000 PyTestLog2DB-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/PyTestLog2DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    42027 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/CDataBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   532667 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/PyTestLog2DB.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43619 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/pytestlog2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/PyTestLog2DB/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/xsd/junit.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/setup.py
```

### Comparing `PyTestLog2DB-0.2.4/LICENSE` & `PyTestLog2DB-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.4/PKG-INFO` & `PyTestLog2DB-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTestLog2DB
-Version: 0.2.4
+Version: 0.2.5
 Summary: Imports pytest result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/python-pytestlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyTestLog2DB-0.2.4/PyTestLog2DB/CDataBase.py` & `PyTestLog2DB-0.2.5/PyTestLog2DB/CDataBase.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.4/PyTestLog2DB/__init__.py` & `PyTestLog2DB-0.2.5/PyTestLog2DB/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.4/PyTestLog2DB/__main__.py` & `PyTestLog2DB-0.2.5/PyTestLog2DB/__main__.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.4/PyTestLog2DB/pytestlog2db.py` & `PyTestLog2DB-0.2.5/PyTestLog2DB/pytestlog2db.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 import sys
 import colorama as col
 import json
 from lxml import etree
 from datetime import datetime, timedelta
 import platform 
 from pkg_resources import get_distribution
-import pytest
 
 from PyTestLog2DB.CDataBase import CDataBase
 from PyTestLog2DB.version import VERSION, VERSION_DATE
 
 PYTEST_DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%f"
 DB_DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -102,15 +101,23 @@
 **Returns:**
 
    / *Type*: str /
 
    Current PyTest and Python verions as testtool.\
    E.g: PyTest 6.2.5 (Python 3.9.0)
    """
-   return f"PyTest {get_distribution('pytest').version} (Python {platform.python_version()})"
+   sPytestVersion = "unknown_version"
+   # Try to get pytest version
+   # Incase pytest is not installed, set to 'unknown_version'
+   try:
+      sPytestVersion = get_distribution('pytest').version
+   except:
+      pass
+
+   return f"PyTest {sPytestVersion} (Python {platform.python_version()})"
 
 CONFIG_SCHEMA = {
    "components" : [str, dict],
    "variant"   : str,
    "version_sw": str,
    "version_hw": str,
    "version_test": str,
@@ -1244,15 +1251,15 @@
       db.vUpdateEvtbls()
       db.vFinishTestResult(_tbl_test_result_id)
       if args.append:
          db.vUpdateEvtbl(_tbl_test_result_id)
 
    # 5. Disconnect from database
    db.disconnect()
-   import_mode_msg = "append" if args.append else "written"
+   import_mode_msg = "appended" if args.append else "written"
    testcnt_msg = f"All {iTotalTestcase}" 
    extended_msg = "" 
    if (iTotalTestcase>iSuccessTestcase):
       testcnt_msg  = f"{iSuccessTestcase} of {iTotalTestcase}"
       extended_msg = f" {iTotalTestcase-iSuccessTestcase} test cases are skipped because of errors."
    Logger.log()
    Logger.log(f"{testcnt_msg} test cases are {import_mode_msg} to database successfully.{extended_msg}")
```

### Comparing `PyTestLog2DB-0.2.4/PyTestLog2DB/version.py` & `PyTestLog2DB-0.2.5/PyTestLog2DB/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of PyTestLog2DB
 #
-VERSION      = "0.2.4"
-VERSION_DATE = "27.04.2023"
+VERSION      = "0.2.5"
+VERSION_DATE = "04.05.2023"
```

### Comparing `PyTestLog2DB-0.2.4/PyTestLog2DB/xsd/junit.xsd` & `PyTestLog2DB-0.2.5/PyTestLog2DB/xsd/junit.xsd`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.4/PyTestLog2DB.egg-info/PKG-INFO` & `PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTestLog2DB
-Version: 0.2.4
+Version: 0.2.5
 Summary: Imports pytest result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/python-pytestlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyTestLog2DB-0.2.4/README.rst` & `PyTestLog2DB-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.4/setup.py` & `PyTestLog2DB-0.2.5/setup.py`

 * *Files identical despite different names*

