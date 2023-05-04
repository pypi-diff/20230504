# Comparing `tmp/irene-pro-0.0.1.tar.gz` & `tmp/irene-pro-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene-pro-0.0.1.tar", last modified: Thu May  4 12:12:45 2023, max compression
+gzip compressed data, was "irene-pro-0.0.2.tar", last modified: Thu May  4 13:22:50 2023, max compression
```

## Comparing `irene-pro-0.0.1.tar` & `irene-pro-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 12:12:45.790504 irene-pro-0.0.1/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene-pro-0.0.1/LICENSE
--rw-rw-rw-   0        0        0        0 2023-05-04 09:36:27.000000 irene-pro-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1200 2023-05-04 12:12:45.788510 irene-pro-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-05-04 10:12:36.000000 irene-pro-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 12:12:45.765572 irene-pro-0.0.1/irene-pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 09:33:00.000000 irene-pro-0.0.1/irene-pro/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-04 09:32:48.000000 irene-pro-0.0.1/irene-pro/logic.py
--rw-rw-rw-   0        0        0    21669 2023-05-04 10:00:25.000000 irene-pro-0.0.1/irene-pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:12:45.784521 irene-pro-0.0.1/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1200 2023-05-04 12:12:44.000000 irene-pro-0.0.1/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-04 12:12:45.000000 irene-pro-0.0.1/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 12:12:44.000000 irene-pro-0.0.1/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-04 12:12:44.000000 irene-pro-0.0.1/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 12:12:44.000000 irene-pro-0.0.1/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      685 2023-05-04 11:34:23.000000 irene-pro-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 12:12:45.790504 irene-pro-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-05-04 12:10:08.000000 irene-pro-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:22:50.769770 irene-pro-0.0.2/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene-pro-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-05-04 09:36:27.000000 irene-pro-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1181 2023-05-04 13:22:50.768773 irene-pro-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-05-04 10:12:36.000000 irene-pro-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 13:22:50.748826 irene-pro-0.0.2/irene-pro/
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:21:03.000000 irene-pro-0.0.2/irene-pro/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 09:32:48.000000 irene-pro-0.0.2/irene-pro/logic.py
+-rw-rw-rw-   0        0        0    21669 2023-05-04 10:00:25.000000 irene-pro-0.0.2/irene-pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:22:50.766780 irene-pro-0.0.2/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1181 2023-05-04 13:22:50.000000 irene-pro-0.0.2/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-04 13:22:50.000000 irene-pro-0.0.2/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 13:22:50.000000 irene-pro-0.0.2/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-04 13:22:50.000000 irene-pro-0.0.2/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 13:22:50.000000 irene-pro-0.0.2/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:22:50.770770 irene-pro-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-05-04 13:22:01.000000 irene-pro-0.0.2/setup.py
```

### Comparing `irene-pro-0.0.1/PKG-INFO` & `irene-pro-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.1
-Summary: A small example package
+Version: 0.0.2
+Summary: Use customized GUI
 Author: Irene coldsober
-Author-email: irene <irene.study.2023@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 'irene-pro'
 
-This is my customized user interface which is rooted from tkinter package.
-nothing big that I did from here that is different from what already in tkinter, but I rather set my default parameters and 
-styles for those rooted to ttk, example Combobox.
-
-this is the first version, and later I will keep making extra-improvement including adding default icons to buttons and other
-cool stuffs until it will be large package or framework in coming years.
-
-=========how to use the package======
-from irene-pro import widgets, logic
-
-button = widgets.btn(master = root, text = 'send')
+# 'irene-pro'
+
+This is my customized user interface which is rooted from tkinter package.
+nothing big that I did from here that is different from what already in tkinter, but I rather set my default parameters and 
+styles for those rooted to ttk, example Combobox.
+
+this is the first version, and later I will keep making extra-improvement including adding default icons to buttons and other
+cool stuffs until it will be large package or framework in coming years.
+
+=========how to use the package======
+from irene-pro import widgets, logic
+
+button = widgets.btn(master = root, text = 'send')
 button.pack(side = LEFT)
```

### Comparing `irene-pro-0.0.1/README.md` & `irene-pro-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `irene-pro-0.0.1/irene-pro/widgets.py` & `irene-pro-0.0.2/irene-pro/widgets.py`

 * *Files identical despite different names*

### Comparing `irene-pro-0.0.1/irene_pro.egg-info/PKG-INFO` & `irene-pro-0.0.2/irene_pro.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.1
-Summary: A small example package
+Version: 0.0.2
+Summary: Use customized GUI
 Author: Irene coldsober
-Author-email: irene <irene.study.2023@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 'irene-pro'
 
-This is my customized user interface which is rooted from tkinter package.
-nothing big that I did from here that is different from what already in tkinter, but I rather set my default parameters and 
-styles for those rooted to ttk, example Combobox.
-
-this is the first version, and later I will keep making extra-improvement including adding default icons to buttons and other
-cool stuffs until it will be large package or framework in coming years.
-
-=========how to use the package======
-from irene-pro import widgets, logic
-
-button = widgets.btn(master = root, text = 'send')
+# 'irene-pro'
+
+This is my customized user interface which is rooted from tkinter package.
+nothing big that I did from here that is different from what already in tkinter, but I rather set my default parameters and 
+styles for those rooted to ttk, example Combobox.
+
+this is the first version, and later I will keep making extra-improvement including adding default icons to buttons and other
+cool stuffs until it will be large package or framework in coming years.
+
+=========how to use the package======
+from irene-pro import widgets, logic
+
+button = widgets.btn(master = root, text = 'send')
 button.pack(side = LEFT)
```

### Comparing `irene-pro-0.0.1/setup.py` & `irene-pro-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3127 0d0a 4445 5343 5249   '0.0.1'..DESCRI
+00000100: 2027 302e 302e 3227 0d0a 4445 5343 5249   '0.0.2'..DESCRI
 00000110: 5054 494f 4e20 3d20 2755 7365 2063 7573  PTION = 'Use cus
 00000120: 746f 6d69 7a65 6420 4755 4927 0d0a 4c4f  tomized GUI'..LO
 00000130: 4e47 5f44 4553 4352 4950 5449 4f4e 203d  NG_DESCRIPTION =
 00000140: 2027 4120 7061 636b 6167 6520 7468 6174   'A package that
 00000150: 2061 6c6c 6f77 7320 796f 7520 746f 2075   allows you to u
 00000160: 7365 2073 7479 6c65 7320 616e 6420 7769  se styles and wi
 00000170: 6467 6574 206f 6620 7375 7065 7220 6c65  dget of super le
```

