# Comparing `tmp/pequenawebview-4.1.2.tar.gz` & `tmp/pequenawebview-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pequenawebview-4.1.2.tar", last modified: Thu May  4 11:36:52 2023, max compression
+gzip compressed data, was "pequenawebview-4.1.3.tar", last modified: Thu May  4 18:44:57 2023, max compression
```

## Comparing `pequenawebview-4.1.2.tar` & `pequenawebview-4.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 11:36:52.417547 pequenawebview-4.1.2/
--rw-rw-rw-   0        0        0     1547 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/LICENSE.md
--rw-rw-rw-   0        0        0      391 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6264 2023-05-04 11:36:52.416550 pequenawebview-4.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4876 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 11:36:52.344742 pequenawebview-4.1.2/pequenawebview.egg-info/
--rw-rw-rw-   0        0        0     6264 2023-05-04 11:36:52.000000 pequenawebview-4.1.2/pequenawebview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-05-04 11:36:52.000000 pequenawebview-4.1.2/pequenawebview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 11:36:52.000000 pequenawebview-4.1.2/pequenawebview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      342 2023-05-04 11:36:52.000000 pequenawebview-4.1.2/pequenawebview.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 11:36:52.000000 pequenawebview-4.1.2/pequenawebview.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 11:36:52.417547 pequenawebview-4.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2825 2023-05-04 11:36:50.000000 pequenawebview-4.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 11:36:52.367701 pequenawebview-4.1.2/webview/
--rw-rw-rw-   0        0        0    11680 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/__init__.py
--rw-rw-rw-   0        0        0     1753 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/event.py
--rw-rw-rw-   0        0        0     3064 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/guilib.py
--rw-rw-rw-   0        0        0     6995 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/http.py
-drwxrwxrwx   0        0        0        0 2023-05-04 11:36:52.378652 pequenawebview-4.1.2/webview/js/
--rw-rw-rw-   0        0        0       55 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/js/__init__.py
--rw-rw-rw-   0        0        0      172 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/js/alert.py
--rw-rw-rw-   0        0        0     4196 2023-05-04 09:54:01.000000 pequenawebview-4.1.2/webview/js/api.py
--rw-rw-rw-   0        0        0      533 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/js/css.py
--rw-rw-rw-   0        0        0    26935 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/js/dom.py
--rw-rw-rw-   0        0        0     1535 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/js/drag.py
--rw-rw-rw-   0        0        0      529 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/js/event.py
--rw-rw-rw-   0        0        0     8501 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/js/npo.py
-drwxrwxrwx   0        0        0        0 2023-05-04 11:36:52.397601 pequenawebview-4.1.2/webview/lib/
--rw-rw-rw-   0        0        0   423864 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/lib/Microsoft.Web.WebView2.Core.dll
--rw-rw-rw-   0        0        0     1642 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/lib/Microsoft.Web.WebView2.LICENSE.md
--rw-rw-rw-   0        0        0    37816 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/lib/Microsoft.Web.WebView2.WinForms.dll
--rw-rw-rw-   0        0        0     7168 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/lib/WebBrowserInterop.x64.dll
--rw-rw-rw-   0        0        0     7168 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/lib/WebBrowserInterop.x86.dll
-drwxrwxrwx   0        0        0        0 2023-05-04 11:36:52.399603 pequenawebview-4.1.2/webview/lib/arm64/
--rw-rw-rw-   0        0        0   132024 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/lib/arm64/WebView2Loader.dll
-drwxrwxrwx   0        0        0        0 2023-05-04 11:36:52.400593 pequenawebview-4.1.2/webview/lib/x64/
--rw-rw-rw-   0        0        0   158672 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/lib/x64/WebView2Loader.dll
-drwxrwxrwx   0        0        0        0 2023-05-04 11:36:52.402588 pequenawebview-4.1.2/webview/lib/x86/
--rw-rw-rw-   0        0        0   115128 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/lib/x86/WebView2Loader.dll
--rw-rw-rw-   0        0        0      784 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/localization.py
--rw-rw-rw-   0        0        0      567 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/menu.py
-drwxrwxrwx   0        0        0        0 2023-05-04 11:36:52.415553 pequenawebview-4.1.2/webview/platforms/
--rw-rw-rw-   0        0        0        0 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/platforms/__init__.py
--rw-rw-rw-   0        0        0    10950 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/platforms/cef.py
--rw-rw-rw-   0        0        0    44888 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/platforms/cocoa.py
--rw-rw-rw-   0        0        0     8044 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/platforms/edgechromium.py
--rw-rw-rw-   0        0        0    27442 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/platforms/gtk.py
--rw-rw-rw-   0        0        0     6600 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/platforms/mshtml.py
--rw-rw-rw-   0        0        0    32858 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/platforms/qt.py
--rw-rw-rw-   0        0        0    26900 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/platforms/winforms.py
--rw-rw-rw-   0        0        0      260 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/screen.py
--rw-rw-rw-   0        0        0     8751 2023-05-04 09:46:13.000000 pequenawebview-4.1.2/webview/util.py
--rw-rw-rw-   0        0        0    15820 2023-05-04 11:36:06.000000 pequenawebview-4.1.2/webview/window.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:44:57.312514 pequenawebview-4.1.3/
+-rw-rw-rw-   0        0        0     1547 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/LICENSE.md
+-rw-rw-rw-   0        0        0      391 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6264 2023-05-04 18:44:57.311516 pequenawebview-4.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4876 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 18:44:57.235751 pequenawebview-4.1.3/pequenawebview.egg-info/
+-rw-rw-rw-   0        0        0     6264 2023-05-04 18:44:57.000000 pequenawebview-4.1.3/pequenawebview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-05-04 18:44:57.000000 pequenawebview-4.1.3/pequenawebview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 18:44:57.000000 pequenawebview-4.1.3/pequenawebview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      342 2023-05-04 18:44:57.000000 pequenawebview-4.1.3/pequenawebview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 18:44:57.000000 pequenawebview-4.1.3/pequenawebview.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 18:44:57.312514 pequenawebview-4.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2825 2023-05-04 18:44:54.000000 pequenawebview-4.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:44:57.257692 pequenawebview-4.1.3/webview/
+-rw-rw-rw-   0        0        0    11680 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/__init__.py
+-rw-rw-rw-   0        0        0     1753 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/event.py
+-rw-rw-rw-   0        0        0     3064 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/guilib.py
+-rw-rw-rw-   0        0        0     6995 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/http.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:44:57.270626 pequenawebview-4.1.3/webview/js/
+-rw-rw-rw-   0        0        0       55 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/js/__init__.py
+-rw-rw-rw-   0        0        0      172 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/js/alert.py
+-rw-rw-rw-   0        0        0     4196 2023-05-04 09:54:01.000000 pequenawebview-4.1.3/webview/js/api.py
+-rw-rw-rw-   0        0        0      533 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/js/css.py
+-rw-rw-rw-   0        0        0    26935 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/js/dom.py
+-rw-rw-rw-   0        0        0     1535 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/js/drag.py
+-rw-rw-rw-   0        0        0      529 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/js/event.py
+-rw-rw-rw-   0        0        0     8501 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/js/npo.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:44:57.286582 pequenawebview-4.1.3/webview/lib/
+-rw-rw-rw-   0        0        0   423864 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/lib/Microsoft.Web.WebView2.Core.dll
+-rw-rw-rw-   0        0        0     1642 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/lib/Microsoft.Web.WebView2.LICENSE.md
+-rw-rw-rw-   0        0        0    37816 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/lib/Microsoft.Web.WebView2.WinForms.dll
+-rw-rw-rw-   0        0        0     7168 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/lib/WebBrowserInterop.x64.dll
+-rw-rw-rw-   0        0        0     7168 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/lib/WebBrowserInterop.x86.dll
+drwxrwxrwx   0        0        0        0 2023-05-04 18:44:57.288578 pequenawebview-4.1.3/webview/lib/arm64/
+-rw-rw-rw-   0        0        0   132024 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/lib/arm64/WebView2Loader.dll
+drwxrwxrwx   0        0        0        0 2023-05-04 18:44:57.291569 pequenawebview-4.1.3/webview/lib/x64/
+-rw-rw-rw-   0        0        0   158672 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/lib/x64/WebView2Loader.dll
+drwxrwxrwx   0        0        0        0 2023-05-04 18:44:57.293564 pequenawebview-4.1.3/webview/lib/x86/
+-rw-rw-rw-   0        0        0   115128 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/lib/x86/WebView2Loader.dll
+-rw-rw-rw-   0        0        0      784 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/localization.py
+-rw-rw-rw-   0        0        0      567 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/menu.py
+drwxrwxrwx   0        0        0        0 2023-05-04 18:44:57.308524 pequenawebview-4.1.3/webview/platforms/
+-rw-rw-rw-   0        0        0        0 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/platforms/__init__.py
+-rw-rw-rw-   0        0        0    10950 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/platforms/cef.py
+-rw-rw-rw-   0        0        0    44888 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/platforms/cocoa.py
+-rw-rw-rw-   0        0        0     8044 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/platforms/edgechromium.py
+-rw-rw-rw-   0        0        0    27442 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/platforms/gtk.py
+-rw-rw-rw-   0        0        0     6600 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/platforms/mshtml.py
+-rw-rw-rw-   0        0        0    32858 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/platforms/qt.py
+-rw-rw-rw-   0        0        0    26900 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/platforms/winforms.py
+-rw-rw-rw-   0        0        0      260 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/screen.py
+-rw-rw-rw-   0        0        0     8751 2023-05-04 09:46:13.000000 pequenawebview-4.1.3/webview/util.py
+-rw-rw-rw-   0        0        0    15846 2023-05-04 18:44:46.000000 pequenawebview-4.1.3/webview/window.py
```

### Comparing `pequenawebview-4.1.2/LICENSE.md` & `pequenawebview-4.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/PKG-INFO` & `pequenawebview-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pequenawebview
-Version: 4.1.2
+Version: 4.1.3
 Summary: Build GUI for your Python program with JavaScript, HTML, and CSS.
 Home-page: https://github.com/Borecjeborec1/pequenawebview
 Author: Roman Sirokov
 Author-email: roman@flowrl.com
 License: New BSD license
 Keywords: gui,webkit,html,web
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pequenawebview Version: 4.1.2 Summary: Build GUI
+Metadata-Version: 2.1 Name: pequenawebview Version: 4.1.3 Summary: Build GUI
 for your Python program with JavaScript, HTML, and CSS. Home-page: https://
 github.com/Borecjeborec1/pequenawebview Author: Roman Sirokov Author-email:
 roman@flowrl.com License: New BSD license Keywords: gui,webkit,html,web
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Operating System :: OS Independent Classifier:
 Environment :: MacOS X Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK Classifier: Environment ::
```

### Comparing `pequenawebview-4.1.2/README.md` & `pequenawebview-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/pequenawebview.egg-info/PKG-INFO` & `pequenawebview-4.1.3/pequenawebview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pequenawebview
-Version: 4.1.2
+Version: 4.1.3
 Summary: Build GUI for your Python program with JavaScript, HTML, and CSS.
 Home-page: https://github.com/Borecjeborec1/pequenawebview
 Author: Roman Sirokov
 Author-email: roman@flowrl.com
 License: New BSD license
 Keywords: gui,webkit,html,web
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pequenawebview Version: 4.1.2 Summary: Build GUI
+Metadata-Version: 2.1 Name: pequenawebview Version: 4.1.3 Summary: Build GUI
 for your Python program with JavaScript, HTML, and CSS. Home-page: https://
 github.com/Borecjeborec1/pequenawebview Author: Roman Sirokov Author-email:
 roman@flowrl.com License: New BSD license Keywords: gui,webkit,html,web
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Operating System :: OS Independent Classifier:
 Environment :: MacOS X Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK Classifier: Environment ::
```

### Comparing `pequenawebview-4.1.2/pequenawebview.egg-info/SOURCES.txt` & `pequenawebview-4.1.3/pequenawebview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/setup.py` & `pequenawebview-4.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'bottle'
 ]
 
 
 with open('README.md') as fh:
     long_description = fh.read()
 
-VERSION = "4.1.2"
+VERSION = "4.1.3"
 
 setup(
     name='pequenawebview',
     author='Roman Sirokov',
     author_email='roman@flowrl.com',
     description=(
         'Build GUI for your Python program with JavaScript, HTML, and CSS.'),
```

### Comparing `pequenawebview-4.1.2/webview/__init__.py` & `pequenawebview-4.1.3/webview/__init__.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/event.py` & `pequenawebview-4.1.3/webview/event.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/guilib.py` & `pequenawebview-4.1.3/webview/guilib.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/http.py` & `pequenawebview-4.1.3/webview/http.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/js/api.py` & `pequenawebview-4.1.3/webview/js/api.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/js/css.py` & `pequenawebview-4.1.3/webview/js/css.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/js/dom.py` & `pequenawebview-4.1.3/webview/js/dom.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/js/drag.py` & `pequenawebview-4.1.3/webview/js/drag.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/js/event.py` & `pequenawebview-4.1.3/webview/js/event.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/js/npo.py` & `pequenawebview-4.1.3/webview/js/npo.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/lib/Microsoft.Web.WebView2.Core.dll` & `pequenawebview-4.1.3/webview/lib/Microsoft.Web.WebView2.Core.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/lib/Microsoft.Web.WebView2.LICENSE.md` & `pequenawebview-4.1.3/webview/lib/Microsoft.Web.WebView2.LICENSE.md`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/lib/Microsoft.Web.WebView2.WinForms.dll` & `pequenawebview-4.1.3/webview/lib/Microsoft.Web.WebView2.WinForms.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/lib/WebBrowserInterop.x64.dll` & `pequenawebview-4.1.3/webview/lib/WebBrowserInterop.x64.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/lib/WebBrowserInterop.x86.dll` & `pequenawebview-4.1.3/webview/lib/WebBrowserInterop.x86.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/lib/arm64/WebView2Loader.dll` & `pequenawebview-4.1.3/webview/lib/arm64/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/lib/x64/WebView2Loader.dll` & `pequenawebview-4.1.3/webview/lib/x64/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/lib/x86/WebView2Loader.dll` & `pequenawebview-4.1.3/webview/lib/x86/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/localization.py` & `pequenawebview-4.1.3/webview/localization.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/menu.py` & `pequenawebview-4.1.3/webview/menu.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/platforms/cef.py` & `pequenawebview-4.1.3/webview/platforms/cef.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/platforms/cocoa.py` & `pequenawebview-4.1.3/webview/platforms/cocoa.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/platforms/edgechromium.py` & `pequenawebview-4.1.3/webview/platforms/edgechromium.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/platforms/gtk.py` & `pequenawebview-4.1.3/webview/platforms/gtk.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/platforms/mshtml.py` & `pequenawebview-4.1.3/webview/platforms/mshtml.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/platforms/qt.py` & `pequenawebview-4.1.3/webview/platforms/qt.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/platforms/winforms.py` & `pequenawebview-4.1.3/webview/platforms/winforms.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/util.py` & `pequenawebview-4.1.3/webview/util.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1.2/webview/window.py` & `pequenawebview-4.1.3/webview/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,23 +400,23 @@
         if not all(map(callable, functions)):
             raise TypeError('Parameter must be a function')
 
         func_list = []
 
         for func in functions:
             name = func.__name__
-            self._functions[name] = func
+            self._functions["exposed." + name] = func
 
             try:
                 params = list(inspect.getfullargspec(func).args)  # Python 3
             except AttributeError:
                 params = list(inspect.getargspec(func).args)  # Python 2
 
             func_list.append({
-                'func': name,
+                'func': "exposed." + name,
                 'params': params
             })
 
         if self.events.loaded.is_set():
             self.evaluate_js('window.pywebview._createApi(%s)' % func_list)
 
     def expose_class(self, cls):
```

