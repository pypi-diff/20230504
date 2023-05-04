# Comparing `tmp/dcentralab_qa_infra_automation-0.1.4.tar.gz` & `tmp/dcentralab_qa_infra_automation-0.1.5.tar.gz`

## Comparing `dcentralab_qa_infra_automation-0.1.4.tar` & `dcentralab_qa_infra_automation-0.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/vcs.xml
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/BasePage.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/.idea/vcs.xml
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/BasePage.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.5/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.1.5/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-0.1.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/BasePage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/BasePage.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConfirmRequestPage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
 confirm request page
 
 @Author: Efrat Cohen
 @Date: 03.2023
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ConnectToWebsitePage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
 connect to website page
 
 @Author: Efrat Cohen
 @Date: 02.2023
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreatePasswordPage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 import pytest
 
 """
 create password page
 
 @Author: Efrat Cohen
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/CreateWalletPage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
 create or import wallet page
 
 @Author: Efrat Cohen
 @Date: 02.2023
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/ImportWalletPage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 import pytest
 
 """
 import wallet page
 
 @Author: Efrat Cohen
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/ReceiveCryptoToUsername.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WalletConnectedHomePage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-receive crypto to your username page
+wallet connected home page
 
 @Author: Efrat Cohen
-@Date: 02.2023
+@Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(text(),'Receive crypto to your username')]")
-DENY_BUTTON = (By.XPATH, "//*[contains(text(),'Deny')]")
+TITLE = (By.XPATH, "//*[contains(@class,'selected-account__name')]")
 
 
-class ReceiveCryptoToUsernamePage(BasePage):
+class WalletConnectedHomePage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
-        @return: true if on page, otherwise return false
+        :return: true if on page, otherwise return false
         """
         return self.is_element_exist(TITLE)
-
-    def click_on_deny(self):
-        self.click(DENY_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/coinbasePages/UseAnExistingWalletPage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
 use an existing wallet page
 
 @Author: Efrat Cohen
 @Date: 02.2023
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConfirmPage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
 confirm metamask wallet page
 
 @Author: Efrat Cohen
 @Date: 12.2022
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/CongratulationsPage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
 congratulations page
 
 @Author: Efrat Cohen
 @Date: 12.2022
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ConnectWithWalletPage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
 connect with metamask page
 
 @Author: Efrat Cohen
 @Date: 12.2022
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImportWalletPage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 import pytest
 
 """
 import wallet page
 
 @Author: Efrat Cohen
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/SwitchNetworkPage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-improve metamask page
+allow the site to switch the network page
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'metametrics-opt-in__title')]")
-I_AGREE_BUTTON = (By.XPATH, "//*[contains(text(),'I agree')]")
+TITLE = (By.XPATH, "//*[contains(text(),'Allow this site to switch the network?')]")
+SWITCH_NETWORK_BUTTON = (By.XPATH, "//*[contains(text(),'Switch network')]")
 
 
-class ImproveMetamaskPage(BasePage):
+class SwitchNetworkPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
         return self.is_element_exist(TITLE)
 
-    def click_on_i_agree_button(self):
+    def click_on_switch_network(self):
         """
-        click on i agree button
+        click on switch network button
         """
-        self.click(I_AGREE_BUTTON)
+        self.click(SWITCH_NETWORK_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/NewToMetamaskPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/ImproveMetamaskPage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
-new to metamask page
+improve metamask page
 
 @Author: Efrat Cohen
 @Date: 12.2022
 """
 
 """page locators"""
-TITLE = (By.XPATH, "//*[contains(@class,'select-action__body-header')]")
-IMPORT_WALLET_BUTTON = (By.XPATH, "//*[contains(text(),'Import wallet')]")
+TITLE = (By.XPATH, "//*[contains(@class,'metametrics-opt-in__title')]")
+I_AGREE_BUTTON = (By.XPATH, "//*[contains(text(),'I agree')]")
 
 
-class NewToMetamaskPage(BasePage):
+class ImproveMetamaskPage(BasePage):
 
     def __init__(self, driver):
         """ ctor - call to BasePage ctor for initialize """
         super().__init__(driver)
 
     def is_page_loaded(self):
         """
         check if on current page
         :return: true if on page, otherwise return false
         """
         return self.is_element_exist(TITLE)
 
-    def click_on_import_wallet(self):
+    def click_on_i_agree_button(self):
         """
-        click on import wallet
+        click on i agree button
         """
-        self.click(IMPORT_WALLET_BUTTON)
+        self.click(I_AGREE_BUTTON)
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/pages/metamaskPages/WelcomeToMetamaskPage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pages.BasePage import BasePage
+from dcentralab_qa_infra_automation.pages.BasePage import BasePage
 from selenium.webdriver.common.by import By
 
 """
 welcome to metamask page
 
 @Author: Efrat Cohen
 @Date: 12.2022
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/walletsActions/CoinbaseActions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import time
 
 import pytest
 from dcentralab_qa_infra_automation.utils.WalletsActionsInterface import WalletsActionsInterface
-from pages.coinbasePages.CreatePasswordPage import CreatePasswordPage
-from pages.coinbasePages.CreateWalletPage import CreateWalletPage
-from pages.coinbasePages.ImportWalletPage import ImportWalletPage
-from pages.coinbasePages.ReceiveCryptoToUsername import ReceiveCryptoToUsernamePage
-from pages.coinbasePages.UseAnExistingWalletPage import UseAnExistingWalletPage
+from dcentralab_qa_infra_automation.pages.coinbasePages.CreatePasswordPage import CreatePasswordPage
+from dcentralab_qa_infra_automation.pages.coinbasePages.CreateWalletPage import CreateWalletPage
+from dcentralab_qa_infra_automation.pages.coinbasePages.ImportWalletPage import ImportWalletPage
+from dcentralab_qa_infra_automation.pages.coinbasePages.ReceiveCryptoToUsername import ReceiveCryptoToUsernamePage
+from dcentralab_qa_infra_automation.pages.coinbasePages.UseAnExistingWalletPage import UseAnExistingWalletPage
 
 
 class CoinbaseActions(WalletsActionsInterface):
     """
     coinbase actions class
     this class implements wallet actions interface.
     """
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py` & `dcentralab_qa_infra_automation-0.1.5/src/dcentralab_qa_infra_automation/walletsActions/MetamaskActions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import time
 
 import pytest
 from dcentralab_qa_infra_automation.utils.WalletsActionsInterface import WalletsActionsInterface
 
-from pages.metamaskPages.ConfirmPage import ConfirmPage
-from pages.metamaskPages.ImportWalletPage import ImportWalletPage
-from pages.metamaskPages.CongratulationsPage import CongratulationsPage
-from pages.metamaskPages.ConnectWithWalletPage import ConnectWithMetamaskPage
-from pages.metamaskPages.ImproveMetamaskPage import ImproveMetamaskPage
-from pages.metamaskPages.NewToMetamaskPage import NewToMetamaskPage
-from pages.metamaskPages.SwitchNetworkPage import SwitchNetworkPage
-from pages.metamaskPages.WalletConnectedHomePage import WalletConnectedHomePage
-from pages.metamaskPages.WelcomeToMetamaskPage import WelcomeToMetamaskPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.ConfirmPage import ConfirmPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.ImportWalletPage import ImportWalletPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.CongratulationsPage import CongratulationsPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.ConnectWithWalletPage import ConnectWithMetamaskPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.ImproveMetamaskPage import ImproveMetamaskPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.NewToMetamaskPage import NewToMetamaskPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.SwitchNetworkPage import SwitchNetworkPage
+from dcentralab_qa_infra_automation.pages.metamaskPages.WalletConnectedHomePage import WalletConnectedHomePage
+from dcentralab_qa_infra_automation.pages.metamaskPages.WelcomeToMetamaskPage import WelcomeToMetamaskPage
 
 
 class MetamaskActions(WalletsActionsInterface):
 
     def __init__(self, driver):
         self.driver = driver
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/LICENSE` & `dcentralab_qa_infra_automation-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.4/pyproject.toml` & `dcentralab_qa_infra_automation-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-0.1.4/PKG-INFO` & `dcentralab_qa_infra_automation-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 0.1.4
+Version: 0.1.5
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

