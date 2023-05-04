# Comparing `tmp/wbBase-0.1.56.tar.gz` & `tmp/wbBase-0.1.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbBase-0.1.56.tar", last modified: Tue May  2 09:43:09 2023, max compression
+gzip compressed data, was "wbBase-0.1.58.tar", last modified: Thu May  4 10:12:29 2023, max compression
```

## Comparing `wbBase-0.1.56.tar` & `wbBase-0.1.58.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.338598 wbBase-0.1.56/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 09:43:07.000000 wbBase-0.1.56/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.326597 wbBase-0.1.56/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.331597 wbBase-0.1.56/Lib/wbBase/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23487 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/application.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/applicationInfo.py
--rw-rw-rw-   0 root         (0) root         (0)    20585 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/applicationWindow.py
--rw-rw-rw-   0 root         (0) root         (0)   309800 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/artprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.335597 wbBase-0.1.56/Lib/wbBase/control/
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/externalToolConfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/externalToolConfigUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/filling.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/iePanel.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/propgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    47198 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/textEditControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.336598 wbBase-0.1.56/Lib/wbBase/dialog/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2342 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/dialog/multiSaveModifiedDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    20381 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/dialog/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.338598 wbBase-0.1.56/Lib/wbBase/document/
--rw-rw-rw-   0 root         (0) root         (0)    23492 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36999 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     8016 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/template.py
--rw-rw-rw-   0 root         (0) root         (0)     9208 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/view.py
--rw-rw-rw-   0 root         (0) root         (0)    21455 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/panelManager.py
--rw-rw-rw-   0 root         (0) root         (0)     3366 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/pluginManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/pluginManager_old.py
--rw-rw-rw-   0 root         (0) root         (0)     8814 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/scripting.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.333597 wbBase-0.1.56/Lib/wbBase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2708 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1027 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2708 2023-05-02 09:43:09.338598 wbBase-0.1.56/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-05-02 09:43:07.000000 wbBase-0.1.56/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-05-02 09:43:09.339598 wbBase-0.1.56/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 09:43:07.000000 wbBase-0.1.56/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.182245 wbBase-0.1.58/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-04 10:12:27.000000 wbBase-0.1.58/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.170244 wbBase-0.1.58/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.176245 wbBase-0.1.58/Lib/wbBase/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23569 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/applicationInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)    20622 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/applicationWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)   309800 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/artprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.179245 wbBase-0.1.58/Lib/wbBase/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/externalToolConfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/externalToolConfigUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/iePanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/propgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    47198 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/control/textEditControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.180245 wbBase-0.1.58/Lib/wbBase/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/dialog/multiSaveModifiedDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    20381 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/dialog/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.182245 wbBase-0.1.58/Lib/wbBase/document/
+-rw-rw-rw-   0 root         (0) root         (0)    23492 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36912 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     8016 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     9208 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/document/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    21455 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/panelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/pluginManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/pluginManager_old.py
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/scripting.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-04 10:12:27.000000 wbBase-0.1.58/Lib/wbBase/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 10:12:29.177245 wbBase-0.1.58/Lib/wbBase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-04 10:12:29.000000 wbBase-0.1.58/Lib/wbBase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-04 10:12:29.182245 wbBase-0.1.58/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-05-04 10:12:27.000000 wbBase-0.1.58/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-05-04 10:12:29.183245 wbBase-0.1.58/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-04 10:12:27.000000 wbBase-0.1.58/setup.py
```

### Comparing `wbBase-0.1.56/LICENSE` & `wbBase-0.1.58/LICENSE`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/application.py` & `wbBase-0.1.58/Lib/wbBase/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import time
 from argparse import ArgumentParser, Namespace
 from importlib import metadata, resources
 from io import BytesIO
 from typing import TYPE_CHECKING, ClassVar, List, Optional, Union
 
 import wx
-from appdirs import AppDirs
 from wx.adv import (
     SPLASH_CENTER_ON_SCREEN,
     SPLASH_NO_TIMEOUT,
     SplashScreen,
 )
 
 from .applicationInfo import ApplicationInfo
@@ -41,14 +40,17 @@
 
     from .applicationWindow import ApplicationWindow
     from .document.manager import DocumentManager
     from .panelManager import PanelManager
 
 log = logging.getLogger(__name__)
 
+AppInfo_None = 0
+AppInfo_AppName = 1
+AppInfo_VendorName = 2
 
 class ExtChangeTestTimer(wx.Timer):
     """
     Timer for test of external changes
     """
 
     @property
@@ -167,15 +169,14 @@
         self.allowMultipleInstances: bool = False
         self.info: ApplicationInfo = self._getAppInfo(info)
         self.cmdLineArguments: Namespace = self._getCmdLineArguments()
         self.extChangeTimerInterval: int = 60
         self.sharedDataDir: str = ""
         self.privateDataDir: str = ""
         self.globalObjects: List[str] = []
-        self.dirs = AppDirs(self.info.AppName, self.info.VendorName)
         wx.App.__init__(self, redirect=False, useBestVisual=True)
 
     def __repr__(self) -> str:
         return '<Application: "%s" by %s>' % (self.AppName, self.VendorName)
 
     # =========================================================================
     # Private methods
@@ -328,14 +329,15 @@
             "__file__",
             "__name__",
             "app",
             "wx",
         ]
         for attr in ("AppName", "AppDisplayName", "VendorName", "VendorDisplayName"):
             setattr(self, attr, getattr(self.info, attr))
+        self.Traits.StandardPaths.UseAppInfo(AppInfo_VendorName|AppInfo_AppName)
         if self.test:
             self.config = wx.FileConfig()
         else:
             self.config = self.Traits.CreateConfig()
         self.instanceChecker = wx.SingleInstanceChecker(
             f"{self.AppName}-{wx.GetUserId()}"
         )
@@ -552,15 +554,15 @@
             sys.exit(0)
         else:
             self.listenAndLoadTimer.Start(250)
 
     def prepareSharedDataFolder(self) -> None:
         self.splashMessage("Preparing shared data folder")
         cfg = self.config
-        defaultFolder = os.path.join(self.dirs.user_data_dir, "shared")
+        defaultFolder = os.path.join(self.Traits.StandardPaths.UserLocalDataDir, "shared")
         with wx.ConfigPathChanger(cfg, "/Application/SharedData/"):
             folder = cfg.Read("Dir", defaultFolder)
             url = cfg.Read("URL", "")
             pull_on_start = cfg.ReadBool("PullOnStart", False)
             if folder:
                 if not os.path.isdir(folder) and not self.test:
                     try:
@@ -612,15 +614,15 @@
                     wx.LogError(f"{e}")
         else:
             wx.LogWarning(" GIT not available\n\nShared Data will not be pulled!")
 
     def preparePrivateDataFolder(self) -> None:
         self.splashMessage("Preparing private data folder")
         cfg = self.config
-        defaultFolder = os.path.join(self.dirs.user_data_dir, "private")
+        defaultFolder = os.path.join(self.Traits.StandardPaths.UserLocalDataDir, "private")
         with wx.ConfigPathChanger(cfg, "/Application/PrivateData/"):
             folder = cfg.Read("Dir", defaultFolder)
             if not os.path.isdir(folder) and not self.test:
                 os.makedirs(folder)
             self.privateDataDir = folder
 
     def MacOpenFiles(self, fileNames) -> None:
```

### Comparing `wbBase-0.1.56/Lib/wbBase/applicationInfo.py` & `wbBase-0.1.58/Lib/wbBase/applicationInfo.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/applicationWindow.py` & `wbBase-0.1.58/Lib/wbBase/applicationWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,17 +306,18 @@
                     "Macro",
                 ),
             )
         for macroFolder in macroFolders:
             if not os.path.isdir(macroFolder):
                 os.makedirs(macroFolder)
             modulesPath = os.path.join(macroFolder, "_Modules")
-            if os.path.isdir(modulesPath):
-                if modulesPath not in sys.path:
-                    sys.path.insert(0, modulesPath)
+            if not os.path.isdir(modulesPath):
+                os.makedirs(modulesPath)
+            if modulesPath not in sys.path:
+                sys.path.insert(0, modulesPath)
         self.scriptsMenu = MacroMenu(folderList=macroFolders)
 
     def buildExtraMenu(self) -> None:
         mnu = self.extraMenu
         if mnu.MenuItemCount == 0:
             mnu.AppendSeparator()
             item = wx.MenuItem(
```

### Comparing `wbBase-0.1.56/Lib/wbBase/artprovider.py` & `wbBase-0.1.58/Lib/wbBase/artprovider.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/control/__init__.py` & `wbBase-0.1.58/Lib/wbBase/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/control/externalToolConfig.py` & `wbBase-0.1.58/Lib/wbBase/control/externalToolConfig.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/control/externalToolConfigUI.py` & `wbBase-0.1.58/Lib/wbBase/control/externalToolConfigUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/control/filling.py` & `wbBase-0.1.58/Lib/wbBase/control/filling.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/control/iePanel.py` & `wbBase-0.1.58/Lib/wbBase/control/iePanel.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/control/propgrid.py` & `wbBase-0.1.58/Lib/wbBase/control/propgrid.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/control/textEditControl.py` & `wbBase-0.1.58/Lib/wbBase/control/textEditControl.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/dialog/multiSaveModifiedDialog.py` & `wbBase-0.1.58/Lib/wbBase/dialog/multiSaveModifiedDialog.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py` & `wbBase-0.1.58/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/dialog/preferences.py` & `wbBase-0.1.58/Lib/wbBase/dialog/preferences.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/document/__init__.py` & `wbBase-0.1.58/Lib/wbBase/document/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/document/manager.py` & `wbBase-0.1.58/Lib/wbBase/document/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     Optional,
     Sequence,
     Tuple,
     Union,
     Iterable,
 )
 
-import appdirs
 import wx
 import wx.aui as aui
 
 from ..dialog.multiSaveModifiedDialog import MultiSaveModifiedDialog
 from . import (
     DOC_NEW,
     DOC_NO_VIEW,
@@ -635,15 +634,15 @@
 
     def SelectDocumentType(
         self, templates: Sequence[DocumentTemplate]
     ) -> Optional[DocumentTemplate]:
         """
         Returns a document template by asking the user (if there is more than
         one template). This function is used in :meth:`CreateDocument`.
-        
+
         :param templates: list of templates from which to choose a desired template.
         """
         if len(templates) == 0:
             return None
         elif len(templates) == 1:
             return templates[0]
         else:
@@ -721,15 +720,17 @@
         """
         :return: All open documents of the given documentType.
         """
         for doc in self.documents:
             if isinstance(doc, documentType):
                 yield doc
 
-    def ActivateView(self, view:View, activate: bool = True, deleting: bool = False) -> None:
+    def ActivateView(
+        self, view: View, activate: bool = True, deleting: bool = False
+    ) -> None:
         """
         Sets the current view.
 
         :param deleting: Currently not used
 
         """
         dbg(f"DocumentManager.ActivateView(view={view}, activate={activate})")
@@ -805,15 +806,15 @@
             if doc in self._docs:
                 doc.Destroy()
             return True
         return False
 
     def CloseDocuments(self, force: bool = True) -> bool:
         """
-        Closes all open documents by calling :meth:`CloseDocument` 
+        Closes all open documents by calling :meth:`CloseDocument`
         for every document.
         """
         dbg("DocumentManager.CloseDocuments()")
         if not force and self.modifiedDocumentsCount > 1:
             with MultiSaveModifiedDialog(self) as dlg:
                 dlg.ShowModal()
                 return True
@@ -850,30 +851,24 @@
         Called when there is an error opening a file.
         currently not used - remove?
         """
         wx.LogWarning("There is an error opening a file.")
 
     def _setupLogging(self) -> None:
         self.log.propagate = False
-        logFolder = appdirs.user_log_dir(
-            appname="Workbench", appauthor=self.app.VendorName
-        )
+        logFolder = os.path.dirname(self.app.Traits.StandardPaths.UserLocalDataDir)
         now = time.localtime()
         logFileFolder = os.path.join(
             logFolder, f"{now.tm_year}", f"{now.tm_year}.{now.tm_mon:02}"
         )
         if not os.path.isdir(logFileFolder):
             os.makedirs(logFileFolder)
-        logFileName = (
-            f"{now.tm_year}.{now.tm_mon:02}.{now.tm_mday:02}-documentLog.txt"
-        )
+        logFileName = f"{now.tm_year}.{now.tm_mon:02}.{now.tm_mday:02}-documentLog.txt"
         logFilePath = os.path.join(logFileFolder, logFileName)
-        docLogHandler = logging.FileHandler(
-            logFilePath, encoding="utf-8", delay=True
-        )
+        docLogHandler = logging.FileHandler(logFilePath, encoding="utf-8", delay=True)
         formatter = logging.Formatter(
             f"%(asctime)s\t{self.app.AppName}\t%(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
         )
         docLogHandler.setFormatter(formatter)
         self.log.addHandler(docLogHandler)
         self.log.setLevel(logging.INFO)
@@ -924,15 +919,15 @@
         # event.Skip()
         dbg("DocumentManager.on_file_save() -> done", indent=0)
 
     def on_file_saveall(self, event: wx.CommandEvent) -> None:
         """
         Event handler for menu :menuselection:`File --> Save All`
 
-        Saves all documents by calling :meth:`.Document.Save` method 
+        Saves all documents by calling :meth:`.Document.Save` method
         of every open document.
         """
         dbg("DocumentManager.on_file_saveall()")
         for document in self.documents:
             document.Save()
             # event.Skip()
```

### Comparing `wbBase-0.1.56/Lib/wbBase/document/notebook.py` & `wbBase-0.1.58/Lib/wbBase/document/notebook.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/document/template.py` & `wbBase-0.1.58/Lib/wbBase/document/template.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/document/view.py` & `wbBase-0.1.58/Lib/wbBase/document/view.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/panelManager.py` & `wbBase-0.1.58/Lib/wbBase/panelManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/pluginManager.py` & `wbBase-0.1.58/Lib/wbBase/pluginManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/pluginManager_old.py` & `wbBase-0.1.58/Lib/wbBase/pluginManager_old.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/scripting.py` & `wbBase-0.1.58/Lib/wbBase/scripting.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase/tools.py` & `wbBase-0.1.58/Lib/wbBase/tools.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/Lib/wbBase.egg-info/PKG-INFO` & `wbBase-0.1.58/Lib/wbBase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.56
+Version: 0.1.58
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.1.56/Lib/wbBase.egg-info/SOURCES.txt` & `wbBase-0.1.58/Lib/wbBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/PKG-INFO` & `wbBase-0.1.58/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.56
+Version: 0.1.58
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.1.56/README.md` & `wbBase-0.1.58/README.md`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.56/setup.cfg` & `wbBase-0.1.58/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.56
+current_version = 0.1.58
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -50,15 +50,14 @@
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
 python_requires = >=3.8,<3.11
 install_requires = 
-	appdirs>=1.4.4
 	wxpython>=4.2.0
 	GitPython>=3.1
 	PyYAML>=6.0
 	importlib_metadata;python_version<'3.10'
 
 [options.packages.find]
 where = Lib
```

