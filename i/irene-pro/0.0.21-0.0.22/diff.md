# Comparing `tmp/irene_pro-0.0.21.tar.gz` & `tmp/irene_pro-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.21.tar", last modified: Thu May  4 13:28:37 2023, max compression
+gzip compressed data, was "irene_pro-0.0.22.tar", last modified: Thu May  4 13:32:25 2023, max compression
```

## Comparing `irene_pro-0.0.21.tar` & `irene_pro-0.0.22.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 13:28:37.154077 irene_pro-0.0.21/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.21/LICENSE
--rw-rw-rw-   0        0        0        0 2023-05-04 09:36:27.000000 irene_pro-0.0.21/MANIFEST.in
--rw-rw-rw-   0        0        0     1182 2023-05-04 13:28:37.152083 irene_pro-0.0.21/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-05-04 10:12:36.000000 irene_pro-0.0.21/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 13:28:37.136125 irene_pro-0.0.21/irene_pro/
--rw-rw-rw-   0        0        0       42 2023-05-04 13:21:03.000000 irene_pro-0.0.21/irene_pro/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-04 09:32:48.000000 irene_pro-0.0.21/irene_pro/logic.py
--rw-rw-rw-   0        0        0    21669 2023-05-04 10:00:25.000000 irene_pro-0.0.21/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:28:37.149091 irene_pro-0.0.21/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1182 2023-05-04 13:28:36.000000 irene_pro-0.0.21/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-04 13:28:36.000000 irene_pro-0.0.21/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 13:28:36.000000 irene_pro-0.0.21/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-04 13:28:36.000000 irene_pro-0.0.21/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 13:28:36.000000 irene_pro-0.0.21/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 13:28:37.154077 irene_pro-0.0.21/setup.cfg
--rw-rw-rw-   0        0        0     1146 2023-05-04 13:28:15.000000 irene_pro-0.0.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:32:25.505220 irene_pro-0.0.22/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.22/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-05-04 09:36:27.000000 irene_pro-0.0.22/MANIFEST.in
+-rw-rw-rw-   0        0        0     1182 2023-05-04 13:32:25.500234 irene_pro-0.0.22/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-05-04 10:12:36.000000 irene_pro-0.0.22/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 13:32:25.474303 irene_pro-0.0.22/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.22/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 09:32:48.000000 irene_pro-0.0.22/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    21669 2023-05-04 10:00:25.000000 irene_pro-0.0.22/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:32:25.494250 irene_pro-0.0.22/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1182 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 13:32:25.000000 irene_pro-0.0.22/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:32:25.508221 irene_pro-0.0.22/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2023-05-04 13:32:01.000000 irene_pro-0.0.22/setup.py
```

### Comparing `irene_pro-0.0.21/PKG-INFO` & `irene_pro-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.21
+Version: 0.0.22
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.21/README.md` & `irene_pro-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.21/irene_pro/widgets.py` & `irene_pro-0.0.22/irene_pro/widgets.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.21/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.22/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.21
+Version: 0.0.22
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.21/setup.py` & `irene_pro-0.0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3231 270d 0a44 4553 4352   '0.0.21'..DESCR
+00000100: 2027 302e 302e 3232 270d 0a44 4553 4352   '0.0.22'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

