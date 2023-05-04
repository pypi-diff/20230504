# Comparing `tmp/pequenawebview-4.1.tar.gz` & `tmp/pequenawebview-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pequenawebview-4.1.tar", last modified: Thu May  4 09:52:27 2023, max compression
+gzip compressed data, was "pequenawebview-4.1.1.tar", last modified: Thu May  4 09:55:05 2023, max compression
```

## Comparing `pequenawebview-4.1.tar` & `pequenawebview-4.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 09:52:27.853671 pequenawebview-4.1/
--rw-rw-rw-   0        0        0     1547 2023-05-04 09:46:13.000000 pequenawebview-4.1/LICENSE.md
--rw-rw-rw-   0        0        0      391 2023-05-04 09:46:13.000000 pequenawebview-4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6262 2023-05-04 09:52:27.853671 pequenawebview-4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4876 2023-05-04 09:46:13.000000 pequenawebview-4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 09:52:27.555469 pequenawebview-4.1/pequenawebview.egg-info/
--rw-rw-rw-   0        0        0     6262 2023-05-04 09:52:27.000000 pequenawebview-4.1/pequenawebview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-05-04 09:52:27.000000 pequenawebview-4.1/pequenawebview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:52:27.000000 pequenawebview-4.1/pequenawebview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      342 2023-05-04 09:52:27.000000 pequenawebview-4.1/pequenawebview.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 09:52:27.000000 pequenawebview-4.1/pequenawebview.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 09:52:27.853671 pequenawebview-4.1/setup.cfg
--rw-rw-rw-   0        0        0     2802 2023-05-04 09:50:53.000000 pequenawebview-4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:52:27.570429 pequenawebview-4.1/webview/
--rw-rw-rw-   0        0        0    11680 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/__init__.py
--rw-rw-rw-   0        0        0     1753 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/event.py
--rw-rw-rw-   0        0        0     3064 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/guilib.py
--rw-rw-rw-   0        0        0     6995 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/http.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:52:27.581400 pequenawebview-4.1/webview/js/
--rw-rw-rw-   0        0        0       55 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/js/__init__.py
--rw-rw-rw-   0        0        0      172 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/js/alert.py
--rw-rw-rw-   0        0        0     3770 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/js/api.py
--rw-rw-rw-   0        0        0      533 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/js/css.py
--rw-rw-rw-   0        0        0    26935 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/js/dom.py
--rw-rw-rw-   0        0        0     1535 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/js/drag.py
--rw-rw-rw-   0        0        0      529 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/js/event.py
--rw-rw-rw-   0        0        0     8501 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/js/npo.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:52:27.766904 pequenawebview-4.1/webview/lib/
--rw-rw-rw-   0        0        0   423864 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/lib/Microsoft.Web.WebView2.Core.dll
--rw-rw-rw-   0        0        0     1642 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md
--rw-rw-rw-   0        0        0    37816 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll
--rw-rw-rw-   0        0        0     7168 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/lib/WebBrowserInterop.x64.dll
--rw-rw-rw-   0        0        0     7168 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/lib/WebBrowserInterop.x86.dll
-drwxrwxrwx   0        0        0        0 2023-05-04 09:52:27.779869 pequenawebview-4.1/webview/lib/arm64/
--rw-rw-rw-   0        0        0   132024 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/lib/arm64/WebView2Loader.dll
-drwxrwxrwx   0        0        0        0 2023-05-04 09:52:27.806797 pequenawebview-4.1/webview/lib/x64/
--rw-rw-rw-   0        0        0   158672 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/lib/x64/WebView2Loader.dll
-drwxrwxrwx   0        0        0        0 2023-05-04 09:52:27.839709 pequenawebview-4.1/webview/lib/x86/
--rw-rw-rw-   0        0        0   115128 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/lib/x86/WebView2Loader.dll
--rw-rw-rw-   0        0        0      784 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/localization.py
--rw-rw-rw-   0        0        0      567 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/menu.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:52:27.851676 pequenawebview-4.1/webview/platforms/
--rw-rw-rw-   0        0        0        0 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/platforms/__init__.py
--rw-rw-rw-   0        0        0    10950 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/platforms/cef.py
--rw-rw-rw-   0        0        0    44888 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/platforms/cocoa.py
--rw-rw-rw-   0        0        0     8044 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/platforms/edgechromium.py
--rw-rw-rw-   0        0        0    27442 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/platforms/gtk.py
--rw-rw-rw-   0        0        0     6600 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/platforms/mshtml.py
--rw-rw-rw-   0        0        0    32858 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/platforms/qt.py
--rw-rw-rw-   0        0        0    26900 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/platforms/winforms.py
--rw-rw-rw-   0        0        0      260 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/screen.py
--rw-rw-rw-   0        0        0     8751 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/util.py
--rw-rw-rw-   0        0        0    14348 2023-05-04 09:46:13.000000 pequenawebview-4.1/webview/window.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:55:05.853894 pequenawebview-4.1.1/
+-rw-rw-rw-   0        0        0     1547 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0      391 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6264 2023-05-04 09:55:05.852896 pequenawebview-4.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4876 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 09:55:05.789224 pequenawebview-4.1.1/pequenawebview.egg-info/
+-rw-rw-rw-   0        0        0     6264 2023-05-04 09:55:05.000000 pequenawebview-4.1.1/pequenawebview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-05-04 09:55:05.000000 pequenawebview-4.1.1/pequenawebview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 09:55:05.000000 pequenawebview-4.1.1/pequenawebview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      342 2023-05-04 09:55:05.000000 pequenawebview-4.1.1/pequenawebview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 09:55:05.000000 pequenawebview-4.1.1/pequenawebview.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 09:55:05.853894 pequenawebview-4.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2804 2023-05-04 09:55:02.000000 pequenawebview-4.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:55:05.813001 pequenawebview-4.1.1/webview/
+-rw-rw-rw-   0        0        0    11680 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/__init__.py
+-rw-rw-rw-   0        0        0     1753 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/event.py
+-rw-rw-rw-   0        0        0     3064 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/guilib.py
+-rw-rw-rw-   0        0        0     6995 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/http.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:55:05.824972 pequenawebview-4.1.1/webview/js/
+-rw-rw-rw-   0        0        0       55 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/js/__init__.py
+-rw-rw-rw-   0        0        0      172 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/js/alert.py
+-rw-rw-rw-   0        0        0     4196 2023-05-04 09:54:01.000000 pequenawebview-4.1.1/webview/js/api.py
+-rw-rw-rw-   0        0        0      533 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/js/css.py
+-rw-rw-rw-   0        0        0    26935 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/js/dom.py
+-rw-rw-rw-   0        0        0     1535 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/js/drag.py
+-rw-rw-rw-   0        0        0      529 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/js/event.py
+-rw-rw-rw-   0        0        0     8501 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/js/npo.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:55:05.832950 pequenawebview-4.1.1/webview/lib/
+-rw-rw-rw-   0        0        0   423864 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/lib/Microsoft.Web.WebView2.Core.dll
+-rw-rw-rw-   0        0        0     1642 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md
+-rw-rw-rw-   0        0        0    37816 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll
+-rw-rw-rw-   0        0        0     7168 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/lib/WebBrowserInterop.x64.dll
+-rw-rw-rw-   0        0        0     7168 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/lib/WebBrowserInterop.x86.dll
+drwxrwxrwx   0        0        0        0 2023-05-04 09:55:05.833948 pequenawebview-4.1.1/webview/lib/arm64/
+-rw-rw-rw-   0        0        0   132024 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/lib/arm64/WebView2Loader.dll
+drwxrwxrwx   0        0        0        0 2023-05-04 09:55:05.835942 pequenawebview-4.1.1/webview/lib/x64/
+-rw-rw-rw-   0        0        0   158672 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/lib/x64/WebView2Loader.dll
+drwxrwxrwx   0        0        0        0 2023-05-04 09:55:05.837937 pequenawebview-4.1.1/webview/lib/x86/
+-rw-rw-rw-   0        0        0   115128 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/lib/x86/WebView2Loader.dll
+-rw-rw-rw-   0        0        0      784 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/localization.py
+-rw-rw-rw-   0        0        0      567 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/menu.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:55:05.850902 pequenawebview-4.1.1/webview/platforms/
+-rw-rw-rw-   0        0        0        0 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/platforms/__init__.py
+-rw-rw-rw-   0        0        0    10950 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/platforms/cef.py
+-rw-rw-rw-   0        0        0    44888 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/platforms/cocoa.py
+-rw-rw-rw-   0        0        0     8044 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/platforms/edgechromium.py
+-rw-rw-rw-   0        0        0    27442 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/platforms/gtk.py
+-rw-rw-rw-   0        0        0     6600 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/platforms/mshtml.py
+-rw-rw-rw-   0        0        0    32858 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/platforms/qt.py
+-rw-rw-rw-   0        0        0    26900 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/platforms/winforms.py
+-rw-rw-rw-   0        0        0      260 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/screen.py
+-rw-rw-rw-   0        0        0     8751 2023-05-04 09:46:13.000000 pequenawebview-4.1.1/webview/util.py
+-rw-rw-rw-   0        0        0    15786 2023-05-04 09:54:26.000000 pequenawebview-4.1.1/webview/window.py
```

### Comparing `pequenawebview-4.1/LICENSE.md` & `pequenawebview-4.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/PKG-INFO` & `pequenawebview-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pequenawebview
-Version: 4.1
+Version: 4.1.1
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
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pequenawebview Version: 4.1 Summary: Build GUI for
-your Python program with JavaScript, HTML, and CSS. Home-page: https://
+Metadata-Version: 2.1 Name: pequenawebview Version: 4.1.1 Summary: Build GUI
+for your Python program with JavaScript, HTML, and CSS. Home-page: https://
 github.com/Borecjeborec1/pequenawebview Author: Roman Sirokov Author-email:
 roman@flowrl.com License: New BSD license Keywords: gui,webkit,html,web
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Operating System :: OS Independent Classifier:
 Environment :: MacOS X Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK Classifier: Environment ::
 X11 Applications :: Qt Classifier: Programming Language :: Python Classifier:
```

### Comparing `pequenawebview-4.1/README.md` & `pequenawebview-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/pequenawebview.egg-info/PKG-INFO` & `pequenawebview-4.1.1/pequenawebview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pequenawebview
-Version: 4.1
+Version: 4.1.1
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
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pequenawebview Version: 4.1 Summary: Build GUI for
-your Python program with JavaScript, HTML, and CSS. Home-page: https://
+Metadata-Version: 2.1 Name: pequenawebview Version: 4.1.1 Summary: Build GUI
+for your Python program with JavaScript, HTML, and CSS. Home-page: https://
 github.com/Borecjeborec1/pequenawebview Author: Roman Sirokov Author-email:
 roman@flowrl.com License: New BSD license Keywords: gui,webkit,html,web
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Operating System :: OS Independent Classifier:
 Environment :: MacOS X Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK Classifier: Environment ::
 X11 Applications :: Qt Classifier: Programming Language :: Python Classifier:
```

### Comparing `pequenawebview-4.1/pequenawebview.egg-info/SOURCES.txt` & `pequenawebview-4.1.1/pequenawebview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/setup.py` & `pequenawebview-4.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'Build GUI for your Python program with JavaScript, HTML, and CSS.'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Borecjeborec1/pequenawebview',
     keywords=['gui', 'webkit', 'html', 'web'],
     install_requires=install_requires,
     extras_require=extras_require,
-    version='4.1',
+    version='4.1.1',
     include_package_data=True,
     packages=['webview', 'webview.js', 'webview.platforms'],
     package_dir={'webview': 'webview'},
     package_data={
         'webview': [
             'webview/lib/WebBrowserInterop.x64.dll',
             'webview/lib/WebBrowserInterop.x86.dll',
```

### Comparing `pequenawebview-4.1/webview/__init__.py` & `pequenawebview-4.1.1/webview/__init__.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/event.py` & `pequenawebview-4.1.1/webview/event.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/guilib.py` & `pequenawebview-4.1.1/webview/guilib.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/http.py` & `pequenawebview-4.1.1/webview/http.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/js/api.py` & `pequenawebview-4.1.1/webview/js/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,16 +12,24 @@
             var funcBody =
                 "var __id = (Math.random() + '').substring(2); " +
                 "var promise = new Promise(function(resolve, reject) { " +
                     "window.pywebview._checkValue('" + funcName + "', resolve, reject, __id); " +
                 "}); " +
                 "window.pywebview._bridge.call('" + funcName + "', arguments, __id); " +
                 "return promise;"
-
-            window.pywebview.api[funcName] = new Function(params, funcBody)
+            var funcNameParts = funcName.split(".");
+            var currentApi = window.pywebview.api;
+            for (var j = 0; j < funcNameParts.length - 1; j++) {
+                var className = funcNameParts[j];
+                if (!currentApi[className]) {
+                    currentApi[className] = {};
+                }
+                currentApi = currentApi[className];
+            }
+            currentApi[funcNameParts[funcNameParts.length - 1]] = new Function(params, funcBody);
             window.pywebview._returnValues[funcName] = {}
         }
     },
 
     _bridge: {
         call: function (funcName, params, id) {
             switch(window.pywebview.platform) {
```

### Comparing `pequenawebview-4.1/webview/js/css.py` & `pequenawebview-4.1.1/webview/js/css.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/js/dom.py` & `pequenawebview-4.1.1/webview/js/dom.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/js/drag.py` & `pequenawebview-4.1.1/webview/js/drag.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/js/event.py` & `pequenawebview-4.1.1/webview/js/event.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/js/npo.py` & `pequenawebview-4.1.1/webview/js/npo.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/lib/Microsoft.Web.WebView2.Core.dll` & `pequenawebview-4.1.1/webview/lib/Microsoft.Web.WebView2.Core.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md` & `pequenawebview-4.1.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll` & `pequenawebview-4.1.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/lib/WebBrowserInterop.x64.dll` & `pequenawebview-4.1.1/webview/lib/WebBrowserInterop.x64.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/lib/WebBrowserInterop.x86.dll` & `pequenawebview-4.1.1/webview/lib/WebBrowserInterop.x86.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/lib/arm64/WebView2Loader.dll` & `pequenawebview-4.1.1/webview/lib/arm64/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/lib/x64/WebView2Loader.dll` & `pequenawebview-4.1.1/webview/lib/x64/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/lib/x86/WebView2Loader.dll` & `pequenawebview-4.1.1/webview/lib/x86/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/localization.py` & `pequenawebview-4.1.1/webview/localization.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/menu.py` & `pequenawebview-4.1.1/webview/menu.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/platforms/cef.py` & `pequenawebview-4.1.1/webview/platforms/cef.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/platforms/cocoa.py` & `pequenawebview-4.1.1/webview/platforms/cocoa.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/platforms/edgechromium.py` & `pequenawebview-4.1.1/webview/platforms/edgechromium.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/platforms/gtk.py` & `pequenawebview-4.1.1/webview/platforms/gtk.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/platforms/mshtml.py` & `pequenawebview-4.1.1/webview/platforms/mshtml.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/platforms/qt.py` & `pequenawebview-4.1.1/webview/platforms/qt.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/platforms/winforms.py` & `pequenawebview-4.1.1/webview/platforms/winforms.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/util.py` & `pequenawebview-4.1.1/webview/util.py`

 * *Files identical despite different names*

### Comparing `pequenawebview-4.1/webview/window.py` & `pequenawebview-4.1.1/webview/window.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,16 @@
                 raise WebViewException('Main window failed to start')
 
             if args[0].gui is None:
                 raise WebViewException('GUI is not initialized')
 
             return function(*args, **kwargs)
         except NameError as e:
-            raise WebViewException('Create a web view window first, before invoking this function')
+            raise WebViewException(
+                'Create a web view window first, before invoking this function')
 
     return wrapper
 
 
 def _shown_call(function):
     return _api_call(function, 'shown')
 
@@ -88,17 +89,17 @@
         self.transparent = transparent
         self.zoomable = zoomable
         self.draggable = draggable
         self.localization_override = localization
         self.vibrancy = vibrancy
 
         # Server config
-        self._http_port=http_port
-        self._server=server
-        self._server_args=server_args
+        self._http_port = http_port
+        self._server = server
+        self._server_args = server_args
 
         # HTTP server path magic
         self._url_prefix = None
         self._common_path = None
         self._server = None
 
         self._js_api = js_api
@@ -122,15 +123,16 @@
         self.gui = gui
 
         self.localization = original_localization.copy()
         if self.localization_override:
             self.localization.update(self.localization_override)
 
         if is_app(self.original_url) and (server is None or server == http.global_server):
-            prefix, common_path, server = http.start_server(urls=[self.original_url], http_port=self._http_port, server=self._server, **self._server_args)
+            prefix, common_path, server = http.start_server(
+                urls=[self.original_url], http_port=self._http_port, server=self._server, **self._server_args)
         elif server is None:
             server = http.global_server
 
         self._url_prefix = server.address if not server is None else None
         self._common_path = server.common_path if not server is None else None
         self._server = server
         self.js_api_endpoint = http.global_server.js_api_endpoint if not http.global_server is None else None
@@ -170,15 +172,16 @@
         if hasattr(self, 'gui') and self.gui != None:
             self.gui.set_on_top(self.uid, on_top)
 
     @_loaded_call
     def get_elements(self, selector):
         # check for GTK's WebKit2 version
         if hasattr(self.gui, 'old_webkit') and self.gui.old_webkit:
-            raise NotImplementedError('get_elements requires WebKit2 2.2 or greater')
+            raise NotImplementedError(
+                'get_elements requires WebKit2 2.2 or greater')
 
         code = """
             var elements = document.querySelectorAll('%s');
             var serializedElements = [];
 
             for (var i = 0; i < elements.length; i++) {
                 var node = pywebview.domJSON.toJSON(elements[i], {
@@ -198,15 +201,16 @@
         """
         Load a new URL into a previously created WebView window. This function must be invoked after WebView windows is
         created with create_window(). Otherwise an exception is thrown.
         :param url: url to load
         :param uid: uid of the target instance
         """
         if ((self._server is None) or (not self._server.running)) and ((is_app(url) or is_local_url(url))):
-            self._url_prefix, self._common_path, self.server = http.start_server([url])
+            self._url_prefix, self._common_path, self.server = http.start_server([
+                                                                                 url])
 
         self.real_url = self._resolve_url(url)
         self.gui.load_url(self.real_url, self.uid)
 
     @_shown_call
     def load_html(self, content, base_uri=base_uri()):
         """
@@ -216,15 +220,16 @@
         :param base_uri: Base URI for resolving links. Default is the directory of the application entry point.
         :param uid: uid of the target instance
         """
         self.gui.load_html(content, base_uri, self.uid)
 
     @_loaded_call
     def load_css(self, stylesheet):
-        code = css.src % stylesheet.replace('\n', '').replace('\r', '').replace('"', "'")
+        code = css.src % stylesheet.replace(
+            '\n', '').replace('\r', '').replace('"', "'")
         self.gui.evaluate_js(code, self.uid)
 
     @_shown_call
     def set_title(self, title):
         """
         Set a new title of the window
         """
@@ -268,15 +273,16 @@
     @_shown_call
     def set_window_size(self, width, height):
         """
         Resize window
         :param width: desired width of target window
         :param height: desired height of target window
         """
-        logger.warning('This function is deprecated and will be removed in future releases. Use resize() instead')
+        logger.warning(
+            'This function is deprecated and will be removed in future releases. Use resize() instead')
         self.resize(width, height)
 
     @_shown_call
     def resize(self, width, height, fix_point=FixPoint.NORTH | FixPoint.WEST):
         """
         Resize window
         :param width: desired width of target window
@@ -326,15 +332,16 @@
         :return: Return value of the evaluated code
         :callback: Optional callback function that will be called for resolved promises
         """
         unique_id = uuid1().hex
         self._callbacks[unique_id] = callback
 
         if self.gui.renderer == 'cef':
-            sync_eval = 'window.external.return_result(JSON.stringify(value), "{0}");'.format(unique_id,)
+            sync_eval = 'window.external.return_result(JSON.stringify(value), "{0}");'.format(
+                unique_id,)
         else:
             sync_eval = 'JSON.stringify(value);'
 
         if callback:
             escaped_script = """
                 var value = eval("{0}");
                 if (pywebview._isPromise(value)) {{
@@ -396,27 +403,55 @@
         func_list = []
 
         for func in functions:
             name = func.__name__
             self._functions[name] = func
 
             try:
-                params = list(inspect.getfullargspec(func).args) # Python 3
+                params = list(inspect.getfullargspec(func).args)  # Python 3
             except AttributeError:
                 params = list(inspect.getargspec(func).args)  # Python 2
 
-
             func_list.append({
                 'func': name,
                 'params': params
             })
 
         if self.events.loaded.is_set():
             self.evaluate_js('window.pywebview._createApi(%s)' % func_list)
 
+    def expose_class(self, cls):
+        if not inspect.isclass(cls):
+            raise TypeError('Parameter must be a class')
+
+        def get_methods(cls, prefix=cls.__name__):
+            func_list = []
+            for name, func in cls.__dict__.items():
+                if inspect.isclass(func):
+                    full_name = prefix + "." + name
+                    func_list.extend(get_methods(func, prefix=full_name))
+                elif callable(func) and not name.startswith('__'):
+                    full_name = prefix + "." + name
+                    self._functions[full_name] = func
+                    try:
+                        params = list(inspect.getfullargspec(
+                            func).args)  # Python 3
+                    except AttributeError:
+                        params = list(inspect.getargspec(
+                            func).args)  # Python 2
+                    func_list.append({
+                        'func': full_name,
+                        'params': params
+                    })
+            return func_list
+
+        func_list = get_methods(cls)
+        if self.events.loaded.is_set():
+            self.evaluate_js('window.pywebview._createApi(%s)' % func_list)
+
     def _resolve_url(self, url):
         if is_app(url):
             return self._url_prefix
         if is_local_url(url) and self._url_prefix and self._common_path is not None:
             filename = os.path.relpath(url, self._common_path)
             return urljoin(self._url_prefix, filename)
         else:
```

