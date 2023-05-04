# Comparing `tmp/appium_flutter_report-0.1.5.tar.gz` & `tmp/appium_flutter_report-0.1.6.tar.gz`

## Comparing `appium_flutter_report-0.1.5.tar` & `appium_flutter_report-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/.gitignore
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/ReportGenerator.iml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/misc.xml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/modules.xml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/vcs.xml
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/workspace.xml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/AppName_2023_12_30_17_57_55.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/files/placeholder
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/screenshots/placeholder
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/videos/placeholder
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/group_and_test.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/logger.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/report_generator.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/src/appium_flutter_report/test_case.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/test/main.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/test/crud/test_crud.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/test/login/test_login.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/.idea/.gitignore
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/.idea/ReportGenerator.iml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/.idea/misc.xml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/.idea/modules.xml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/response_sample/AppName_2023_12_30_17_57_55/AppName_2023_12_30_17_57_55.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/response_sample/AppName_2023_12_30_17_57_55/files/placeholder
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/response_sample/AppName_2023_12_30_17_57_55/screenshots/placeholder
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/response_sample/AppName_2023_12_30_17_57_55/videos/placeholder
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/src/appium_flutter_report/__init__.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/src/appium_flutter_report/group_and_test.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/src/appium_flutter_report/logger.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/src/appium_flutter_report/report_generator.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/src/appium_flutter_report/test_case.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/test/main.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/test/crud/test_crud.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/test/login/test_login.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 appium_flutter_report-0.1.6/PKG-INFO
```

### Comparing `appium_flutter_report-0.1.5/.idea/workspace.xml` & `appium_flutter_report-0.1.6/.idea/workspace.xml`

 * *Files 18% similar despite different names*

#### Comparing `appium_flutter_report-0.1.5/.idea/workspace.xml` & `appium_flutter_report-0.1.6/.idea/workspace.xml`

```diff
@@ -1,14 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="d74b248d-601e-4b9e-80fb-5b030921959d" name="Changes" comment=""/>
+    <list default="true" id="d74b248d-601e-4b9e-80fb-5b030921959d" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/appium_flutter_report/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/appium_flutter_report/__init__.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/appium_flutter_report/group_and_test.py" beforeDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
@@ -24,22 +28,22 @@
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2Owqkpc98EjOwKySeiXF9xVrrNv"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "git-widget-placeholder": "main",
-    "last_opened_file_path": "D:/AppiumContribution/AppiumFlutterReport/PythonReportGenerator",
-    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;main&quot;,
+    &quot;last_opened_file_path&quot;: &quot;D:/AppiumContribution/AppiumFlutterReport/PythonReportGenerator&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;
   }
-}]]></component>
+}</component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
       <recent name="D:\AppiumContribution\AppiumFlutterReport\PythonReportGenerator\AppName_2023_12_30_17_57_55\files"/>
       <recent name="D:\AppiumContribution\AppiumFlutterReport\PythonReportGenerator\AppName_2023_12_30_17_57_55\screenshots"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="D:\AppiumContribution\AppiumFlutterReport\PythonReportGenerator\src\apppium_flutter_report_generator"/>
```

### Comparing `appium_flutter_report-0.1.5/.idea/inspectionProfiles/Project_Default.xml` & `appium_flutter_report-0.1.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.5/response_sample/AppName_2023_12_30_17_57_55/AppName_2023_12_30_17_57_55.json` & `appium_flutter_report-0.1.6/response_sample/AppName_2023_12_30_17_57_55/AppName_2023_12_30_17_57_55.json`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.5/src/appium_flutter_report/__init__.py` & `appium_flutter_report-0.1.6/src/appium_flutter_report/__init__.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.5/src/appium_flutter_report/group_and_test.py` & `appium_flutter_report-0.1.6/src/appium_flutter_report/group_and_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from src.appium_flutter_report.report_generator import FlutterReportGenerator
-from src.appium_flutter_report.test_case import TestCaseData, Status
-from src.appium_flutter_report.logger import Logger
+from .report_generator import FlutterReportGenerator
+from .test_case import TestCaseData, Status
+from .logger import Logger
 import traceback
 
 
 def group(title: str, function_with_no_parameter, skip: bool = False):
     __create_test_case(title=title, testing=function_with_no_parameter, is_group=True,
                        skip=skip)
```

### Comparing `appium_flutter_report-0.1.5/src/appium_flutter_report/report_generator.py` & `appium_flutter_report-0.1.6/src/appium_flutter_report/report_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from src.appium_flutter_report.test_case import TestCaseData
+from .test_case import TestCaseData
 import json
 from appium import webdriver
 
 
 class FlutterReportGenerator:
     driver: webdriver.Remote
     app_name: str
```

### Comparing `appium_flutter_report-0.1.5/src/appium_flutter_report/test_case.py` & `appium_flutter_report-0.1.6/src/appium_flutter_report/test_case.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.5/test/main.py` & `appium_flutter_report-0.1.6/test/main.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.5/test/crud/test_crud.py` & `appium_flutter_report-0.1.6/test/crud/test_crud.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.5/test/login/test_login.py` & `appium_flutter_report-0.1.6/test/login/test_login.py`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.5/LICENSE` & `appium_flutter_report-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `appium_flutter_report-0.1.5/pyproject.toml` & `appium_flutter_report-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "appium_flutter_report"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Aaradhya Gopal Nepal", email="aradhya.1441@gmail.com" },
 ]
 description = "A package for generating Appium Flutter Report."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `appium_flutter_report-0.1.5/PKG-INFO` & `appium_flutter_report-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appium_flutter_report
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for generating Appium Flutter Report.
 Project-URL: Homepage, https://github.com/AradhyaNepal/AppiumFlutterReport/tree/main/PythonReportGenerator
 Project-URL: Bug Tracker, https://github.com/AradhyaNepal/AppiumFlutterReport/issues
 Author-email: Aaradhya Gopal Nepal <aradhya.1441@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

