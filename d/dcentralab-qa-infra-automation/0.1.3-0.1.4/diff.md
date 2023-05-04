# Comparing `tmp/dcentralab_qa_infra_automation-0.1.3.tar.gz` & `tmp/dcentralab_qa_infra_automation-0.1.4.tar.gz`

## Comparing `dcentralab_qa_infra_automation-0.1.3.tar` & `dcentralab_qa_infra_automation-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,51 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/vcs.xml
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/BasePage.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-0.1.3/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-0.1.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/LICENSE` & `dcentralab_qa_infra_automation-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.3/pyproject.toml` & `dcentralab_qa_infra_automation-0.1.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-0.1.3/PKG-INFO` & `dcentralab_qa_infra_automation-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

