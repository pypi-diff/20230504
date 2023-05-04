# Comparing `tmp/fonttoolsWB-0.1.3.tar.gz` & `tmp/fonttoolsWB-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fonttoolsWB-0.1.3.tar", last modified: Tue May  2 16:58:58 2023, max compression
+gzip compressed data, was "fonttoolsWB-0.1.4.tar", last modified: Thu May  4 11:53:52 2023, max compression
```

## Comparing `fonttoolsWB-0.1.3.tar` & `fonttoolsWB-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:58:58.219802 fonttoolsWB-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 16:58:56.000000 fonttoolsWB-0.1.3/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:58:58.214801 fonttoolsWB-0.1.3/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:58:58.216802 fonttoolsWB-0.1.3/Lib/fonttoolsWB/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-02 16:58:56.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:58:58.219802 fonttoolsWB-0.1.3/Lib/fonttoolsWB/data/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-02 16:58:56.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-05-02 16:58:56.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB/data/application.yml
--rw-rw-rw-   0 root         (0) root         (0)     1995 2023-05-02 16:58:56.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB/data/firstRun.py
--rw-rw-rw-   0 root         (0) root         (0)     9767 2023-05-02 16:58:56.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB/data/splashscreen.png
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-05-02 16:58:56.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:58:58.218802 fonttoolsWB-0.1.3/Lib/fonttoolsWB.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2305 2023-05-02 16:58:58.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-02 16:58:58.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 16:58:58.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-02 16:58:58.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-02 16:58:58.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-02 16:58:58.000000 fonttoolsWB-0.1.3/Lib/fonttoolsWB.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2305 2023-05-02 16:58:58.220802 fonttoolsWB-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-05-02 16:58:56.000000 fonttoolsWB-0.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2379 2023-05-02 16:58:58.221802 fonttoolsWB-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 16:58:56.000000 fonttoolsWB-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.952935 fonttoolsWB-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.946934 fonttoolsWB-0.1.4/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.949934 fonttoolsWB-0.1.4/Lib/fonttoolsWB/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.952935 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/application.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2379 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/firstRun.py
+-rw-rw-rw-   0 root         (0) root         (0)     9767 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/splashscreen.png
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.951934 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-05-04 11:53:52.952935 fonttoolsWB-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2379 2023-05-04 11:53:52.953935 fonttoolsWB-0.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/setup.py
```

### Comparing `fonttoolsWB-0.1.3/LICENSE` & `fonttoolsWB-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.1.3/Lib/fonttoolsWB/data/application.yml` & `fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/application.yml`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.1.3/Lib/fonttoolsWB/data/firstRun.py` & `fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/firstRun.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,19 +56,30 @@
 def setTheme():
     app = wx.GetApp()
     config = app.config
     config.SetPath("/Window/Panels/")
     for name, value in theme.items():
         config.WriteInt(name, value)
 
+def setExternalTools():
+    app = wx.GetApp()
+    config = app.config
+    config.SetPath("/Application/")
+    externalTools = config.Read("ExternalTools")
+    if externalTools:
+        return
+    config.Write("ExternalTools", "[{'name': 'FontTools Documentation', 'cmd': 'https://fonttools.readthedocs.io/en/latest/', 'folder': ''}]")
+
 
 def main():
     setTheme()
+    setExternalTools()
     makeScripts()
 
 
 if __name__ == "__main__":
     main()
     del setTheme
+    del setExternalTools
     del makeScripts
     del newScriptCode
     del theme
```

### Comparing `fonttoolsWB-0.1.3/Lib/fonttoolsWB/data/splashscreen.png` & `fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/splashscreen.png`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.1.3/Lib/fonttoolsWB.egg-info/PKG-INFO` & `fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fonttoolsWB
-Version: 0.1.3
+Version: 0.1.4
 Summary: FontTools WorkBench - Edit OpenType fonts as XML.
 Home-page: https://gitlab.com/workbench2/fonttoolsWB
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/fonttoolsWB
 Project-URL: Documentation, https://workbench2.gitlab.io/fonttoolsWB
 Project-URL: Tracker, https://gitlab.com/workbench2/fonttoolsWB/-/issues
@@ -44,15 +44,17 @@
 
 ## Installation
 
 ```shell
 pip install fonttoolsWB
 ```
 
-If you intend to write your own Python scripts for the FontTools Workbench, you may want to install additional plugins to aid in development. This can be done as follows:
+If you intend to write your own Python scripts for the FontTools Workbench, 
+you may want to install additional plugins to aid in development. 
+This can be done as follows:
 ```shell
 pip install fonttoolsWB[develop]
 ```
 
 After installation you find an executable in the usual location:
 - On Windows:
     
@@ -62,7 +64,17 @@
 
     `Lib/Frameworks/Python.framework/Versions/3.10/bin/fonttoolswb`
 
 The actual executable path may vary depending on your Python version 
 and installation location.
 
 Launch the executable to run the application.
+
+## Documentation
+
+For details read the [Documentation](https://workbench2.gitlab.io/fonttoolsWB/).
+
+## Sample
+
+Some sample scripts that you can run in the FontTools Workbench can be found 
+in the [snippets](https://gitlab.com/workbench2/fonttoolsWB/-/snippets) section 
+of the repository.
```

### Comparing `fonttoolsWB-0.1.3/PKG-INFO` & `fonttoolsWB-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fonttoolsWB
-Version: 0.1.3
+Version: 0.1.4
 Summary: FontTools WorkBench - Edit OpenType fonts as XML.
 Home-page: https://gitlab.com/workbench2/fonttoolsWB
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/fonttoolsWB
 Project-URL: Documentation, https://workbench2.gitlab.io/fonttoolsWB
 Project-URL: Tracker, https://gitlab.com/workbench2/fonttoolsWB/-/issues
@@ -44,15 +44,17 @@
 
 ## Installation
 
 ```shell
 pip install fonttoolsWB
 ```
 
-If you intend to write your own Python scripts for the FontTools Workbench, you may want to install additional plugins to aid in development. This can be done as follows:
+If you intend to write your own Python scripts for the FontTools Workbench, 
+you may want to install additional plugins to aid in development. 
+This can be done as follows:
 ```shell
 pip install fonttoolsWB[develop]
 ```
 
 After installation you find an executable in the usual location:
 - On Windows:
     
@@ -62,7 +64,17 @@
 
     `Lib/Frameworks/Python.framework/Versions/3.10/bin/fonttoolswb`
 
 The actual executable path may vary depending on your Python version 
 and installation location.
 
 Launch the executable to run the application.
+
+## Documentation
+
+For details read the [Documentation](https://workbench2.gitlab.io/fonttoolsWB/).
+
+## Sample
+
+Some sample scripts that you can run in the FontTools Workbench can be found 
+in the [snippets](https://gitlab.com/workbench2/fonttoolsWB/-/snippets) section 
+of the repository.
```

### Comparing `fonttoolsWB-0.1.3/README.md` & `fonttoolsWB-0.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 ## Installation
 
 ```shell
 pip install fonttoolsWB
 ```
 
-If you intend to write your own Python scripts for the FontTools Workbench, you may want to install additional plugins to aid in development. This can be done as follows:
+If you intend to write your own Python scripts for the FontTools Workbench, 
+you may want to install additional plugins to aid in development. 
+This can be done as follows:
 ```shell
 pip install fonttoolsWB[develop]
 ```
 
 After installation you find an executable in the usual location:
 - On Windows:
     
@@ -25,7 +27,17 @@
 
     `Lib/Frameworks/Python.framework/Versions/3.10/bin/fonttoolswb`
 
 The actual executable path may vary depending on your Python version 
 and installation location.
 
 Launch the executable to run the application.
+
+## Documentation
+
+For details read the [Documentation](https://workbench2.gitlab.io/fonttoolsWB/).
+
+## Sample
+
+Some sample scripts that you can run in the FontTools Workbench can be found 
+in the [snippets](https://gitlab.com/workbench2/fonttoolsWB/-/snippets) section 
+of the repository.
```

### Comparing `fonttoolsWB-0.1.3/setup.cfg` & `fonttoolsWB-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.3
+current_version = 0.1.4
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -55,15 +55,15 @@
 
 [options]
 packages = find:
 package_dir = 
 	=Lib
 python_requires = >=3.8,<3.11
 install_requires = 
-	wbBase>=0.1.56
+	wbBase>=0.1.58
 	wbpFonttools>=0.1.9
 	wbpLoglist>=0.1.5
 	wbpOutput>=0.1.9
 	wbpShell>=0.1.7
 	wbpTextedit>=0.1.6
 	wbpUItools>=0.1.9
```

