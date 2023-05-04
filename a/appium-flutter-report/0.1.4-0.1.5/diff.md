# Comparing `tmp/appium_flutter_report-0.1.4.tar.gz` & `tmp/appium_flutter_report-0.1.5.tar.gz`

## Comparing `appium_flutter_report-0.1.4.tar` & `appium_flutter_report-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/.idea/.gitignore
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/.idea/ReportGenerator.iml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/.idea/misc.xml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/.idea/modules.xml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/.idea/vcs.xml
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/.idea/workspace.xml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/response_sample/AppName_2023_12_30_17_57_55/AppName_2023_12_30_17_57_55.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/response_sample/AppName_2023_12_30_17_57_55/files/placeholder
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/response_sample/AppName_2023_12_30_17_57_55/screenshots/placeholder
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/response_sample/AppName_2023_12_30_17_57_55/videos/placeholder
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/src/appium_flutter_report/__init__.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/src/appium_flutter_report/logger.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/src/appium_flutter_report/report_generator.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/src/appium_flutter_report/test_case.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/test/main.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/test/crud/test_crud.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/test/login/test_login.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/.gitignore
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/ReportGenerator.iml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/misc.xml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/modules.xml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/AppName_2023_12_30_17_57_55.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/files/placeholder
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/screenshots/placeholder
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/videos/placeholder
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/group_and_test.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/logger.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/report_generator.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/test_case.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/test/main.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/test/crud/test_crud.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/test/login/test_login.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/PKG-INFO
```

### Comparing `appium_flutter_report-0.1.4/.idea/workspace.xml` & `appium_flutter_report-0.1.5/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/.idea/inspectionProfiles/Project_Default.xml` & `appium_flutter_report-0.1.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/response_sample/AppName_2023_12_30_17_57_55/AppName_2023_12_30_17_57_55.json` & `appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/AppName_2023_12_30_17_57_55.json`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/src/appium_flutter_report/__init__.py` & `appium_flutter_report-0.1.5/src/appium_flutter_report/__init__.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/src/appium_flutter_report/logger.py` & `appium_flutter_report-0.1.5/src/appium_flutter_report/logger.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/src/appium_flutter_report/report_generator.py` & `appium_flutter_report-0.1.5/src/appium_flutter_report/report_generator.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/src/appium_flutter_report/test_case.py` & `appium_flutter_report-0.1.5/src/appium_flutter_report/test_case.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/test/main.py` & `appium_flutter_report-0.1.5/test/main.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/test/crud/test_crud.py` & `appium_flutter_report-0.1.5/test/crud/test_crud.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/test/login/test_login.py` & `appium_flutter_report-0.1.5/test/login/test_login.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/LICENSE` & `appium_flutter_report-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.4/pyproject.toml` & `appium_flutter_report-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "appium_flutter_report"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Aaradhya Gopal Nepal", email="aradhya.1441@gmail.com" },
 ]
 description = "A package for generating Appium Flutter Report."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `appium_flutter_report-0.1.4/PKG-INFO` & `appium_flutter_report-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appium_flutter_report
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for generating Appium Flutter Report.
 Project-URL: Homepage, https://github.com/AradhyaNepal/AppiumFlutterReport/tree/main/PythonReportGenerator
 Project-URL: Bug Tracker, https://github.com/AradhyaNepal/AppiumFlutterReport/issues
 Author-email: Aaradhya Gopal Nepal <aradhya.1441@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

