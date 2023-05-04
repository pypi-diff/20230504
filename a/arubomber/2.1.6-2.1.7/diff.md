# Comparing `tmp/arubomber-2.1.6.tar.gz` & `tmp/arubomber-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arubomber-2.1.6.tar", last modified: Mon Jan 30 18:38:54 2023, max compression
+gzip compressed data, was "arubomber-2.1.7.tar", last modified: Thu May  4 12:23:42 2023, max compression
```

## Comparing `arubomber-2.1.6.tar` & `arubomber-2.1.7.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-30 18:38:54.805376 arubomber-2.1.6/
--rw-rw-rw-   0        0        0     1091 2022-10-08 16:25:44.000000 arubomber-2.1.6/LICENSE
--rw-rw-rw-   0        0        0     3071 2023-01-30 18:38:54.805376 arubomber-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2406 2023-01-30 18:27:42.000000 arubomber-2.1.6/README.md
--rw-rw-rw-   0        0        0      110 2022-10-08 16:48:30.000000 arubomber-2.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      771 2023-01-30 18:38:54.809373 arubomber-2.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-30 18:38:53.068541 arubomber-2.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-01-30 18:38:54.049038 arubomber-2.1.6/src/arubomber.egg-info/
--rw-rw-rw-   0        0        0     3071 2023-01-30 18:38:53.000000 arubomber-2.1.6/src/arubomber.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-01-30 18:38:53.000000 arubomber-2.1.6/src/arubomber.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-30 18:38:53.000000 arubomber-2.1.6/src/arubomber.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-30 18:38:53.000000 arubomber-2.1.6/src/arubomber.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-30 18:38:54.749014 arubomber-2.1.6/src/bomber/
--rw-rw-rw-   0        0        0      296 2022-11-06 11:56:09.000000 arubomber-2.1.6/src/bomber/__init__.py
--rw-rw-rw-   0        0        0   116893 2023-01-30 18:29:50.000000 arubomber-2.1.6/src/bomber/bomber.py
--rw-rw-rw-   0        0        0   116893 2023-01-30 18:30:13.000000 arubomber-2.1.6/src/bomber/linux.py
--rw-rw-rw-   0        0        0   116893 2023-01-30 18:30:28.000000 arubomber-2.1.6/src/bomber/win.py
--rw-rw-rw-   0        0        0   116893 2023-01-30 18:30:18.000000 arubomber-2.1.6/src/bomber/windows.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:23:42.233993 arubomber-2.1.7/
+-rw-rw-rw-   0        0        0     1091 2022-10-08 16:25:44.000000 arubomber-2.1.7/LICENSE
+-rw-rw-rw-   0        0        0     3071 2023-05-04 12:23:42.234994 arubomber-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2406 2023-05-04 12:20:34.000000 arubomber-2.1.7/README.md
+-rw-rw-rw-   0        0        0      110 2022-10-08 16:48:30.000000 arubomber-2.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      771 2023-05-04 12:23:42.247985 arubomber-2.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 12:23:42.134055 arubomber-2.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 12:23:42.214006 arubomber-2.1.7/src/arubomber.egg-info/
+-rw-rw-rw-   0        0        0     3071 2023-05-04 12:23:42.000000 arubomber-2.1.7/src/arubomber.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-04 12:23:42.000000 arubomber-2.1.7/src/arubomber.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 12:23:42.000000 arubomber-2.1.7/src/arubomber.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 12:23:42.000000 arubomber-2.1.7/src/arubomber.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 12:23:42.229997 arubomber-2.1.7/src/bomber/
+-rw-rw-rw-   0        0        0        0 2023-05-04 12:16:27.000000 arubomber-2.1.7/src/bomber/__init__.py
+-rw-rw-rw-   0        0        0    37552 2023-05-04 12:09:52.000000 arubomber-2.1.7/src/bomber/bomber.py
```

### Comparing `arubomber-2.1.6/LICENSE` & `arubomber-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arubomber-2.1.6/PKG-INFO` & `arubomber-2.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arubomber
-Version: 2.1.6
+Version: 2.1.7
 Summary: SMS Bomber Project.
 Home-page: https://github.com/Aru-Ofc-git/ARU-BOMBER.git
 Author: Ariful Islam Arman
 Author-email: arifulislamarman02@gmail.com
 Project-URL: Bug Tracker, https://github.com/Aru-Ofc-git
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 <!-- CIRCLE_TOOLS -->
 <!-- CODED BY ARU -->
 
 <div align="center" >
   <h1>SMS BOMBING SYSTEM</h1>
 </div>
 <p align="center">
-  <img src="https://img.shields.io/badge/Version-2.1.6-orange?style=for-the-badge">
+  <img src="https://img.shields.io/badge/Version-2.1.7-orange?style=for-the-badge">
   <img src="https://img.shields.io/github/license/Aru-Ofc-git/ARU-BOMBER?style=for-the-badge">
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/badge/Author-ARU-green?style=flat-square">
   <img src="https://img.shields.io/badge/Open%20Source-NO-green?style=flat-square">
   <img src="https://img.shields.io/badge/Written%20In-Python-green?style=flat-square">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: arubomber Version: 2.1.6 Summary: SMS Bomber
+Metadata-Version: 2.1 Name: arubomber Version: 2.1.7 Summary: SMS Bomber
 Project. Home-page: https://github.com/Aru-Ofc-git/ARU-BOMBER.git Author:
 Ariful Islam Arman Author-email: arifulislamarman02@gmail.com Project-URL: Bug
 Tracker, https://github.com/Aru-Ofc-git Classifier: Development Status :: 5 -
 Production/Stable Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.5 Classifier: Programming Language ::
 Python Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE
                        ****** SMS BOMBING SYSTEM ******
-[https://img.shields.io/badge/Version-2.1.6-orange?style=for-the-badge] [https:
+[https://img.shields.io/badge/Version-2.1.7-orange?style=for-the-badge] [https:
   //img.shields.io/github/license/Aru-Ofc-git/ARU-BOMBER?style=for-the-badge]
   [https://img.shields.io/badge/Author-ARU-green?style=flat-square] [https://
    img.shields.io/badge/Open%20Source-NO-green?style=flat-square] [https://
        img.shields.io/badge/Written%20In-Python-green?style=flat-square]
              **** If You need any Help please connect with us ****
 `` ð¡ Get in Touch ``
 [LinkedIn] [Instagram] [Twitter] [Spotify] [YouTube] [DEV.to] [Gmail] [Github]
```

### Comparing `arubomber-2.1.6/README.md` & `arubomber-2.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!-- CIRCLE_TOOLS -->
 <!-- CODED BY ARU -->
 
 <div align="center" >
   <h1>SMS BOMBING SYSTEM</h1>
 </div>
 <p align="center">
-  <img src="https://img.shields.io/badge/Version-2.1.6-orange?style=for-the-badge">
+  <img src="https://img.shields.io/badge/Version-2.1.7-orange?style=for-the-badge">
   <img src="https://img.shields.io/github/license/Aru-Ofc-git/ARU-BOMBER?style=for-the-badge">
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/badge/Author-ARU-green?style=flat-square">
   <img src="https://img.shields.io/badge/Open%20Source-NO-green?style=flat-square">
   <img src="https://img.shields.io/badge/Written%20In-Python-green?style=flat-square">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 
                        ****** SMS BOMBING SYSTEM ******
-[https://img.shields.io/badge/Version-2.1.6-orange?style=for-the-badge] [https:
+[https://img.shields.io/badge/Version-2.1.7-orange?style=for-the-badge] [https:
   //img.shields.io/github/license/Aru-Ofc-git/ARU-BOMBER?style=for-the-badge]
   [https://img.shields.io/badge/Author-ARU-green?style=flat-square] [https://
    img.shields.io/badge/Open%20Source-NO-green?style=flat-square] [https://
        img.shields.io/badge/Written%20In-Python-green?style=flat-square]
              **** If You need any Help please connect with us ****
 `` ð¡ Get in Touch ``
 [LinkedIn] [Instagram] [Twitter] [Spotify] [YouTube] [DEV.to] [Gmail] [Github]
```

### Comparing `arubomber-2.1.6/setup.cfg` & `arubomber-2.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7275 626f 6d62 6572 0d0a 7665   = arubomber..ve
-00000020: 7273 696f 6e20 3d20 322e 312e 360d 0a61  rsion = 2.1.6..a
+00000020: 7273 696f 6e20 3d20 322e 312e 370d 0a61  rsion = 2.1.7..a
 00000030: 7574 686f 7220 3d20 4172 6966 756c 2049  uthor = Ariful I
 00000040: 736c 616d 2041 726d 616e 0d0a 6175 7468  slam Arman..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 7269 6675  or_email = arifu
 00000060: 6c69 736c 616d 6172 6d61 6e30 3240 676d  lislamarman02@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2053 4d53 2042 6f6d 6265  tion = SMS Bombe
 00000090: 7220 5072 6f6a 6563 742e 0d0a 6c6f 6e67  r Project...long
```

### Comparing `arubomber-2.1.6/src/arubomber.egg-info/PKG-INFO` & `arubomber-2.1.7/src/arubomber.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arubomber
-Version: 2.1.6
+Version: 2.1.7
 Summary: SMS Bomber Project.
 Home-page: https://github.com/Aru-Ofc-git/ARU-BOMBER.git
 Author: Ariful Islam Arman
 Author-email: arifulislamarman02@gmail.com
 Project-URL: Bug Tracker, https://github.com/Aru-Ofc-git
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 <!-- CIRCLE_TOOLS -->
 <!-- CODED BY ARU -->
 
 <div align="center" >
   <h1>SMS BOMBING SYSTEM</h1>
 </div>
 <p align="center">
-  <img src="https://img.shields.io/badge/Version-2.1.6-orange?style=for-the-badge">
+  <img src="https://img.shields.io/badge/Version-2.1.7-orange?style=for-the-badge">
   <img src="https://img.shields.io/github/license/Aru-Ofc-git/ARU-BOMBER?style=for-the-badge">
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/badge/Author-ARU-green?style=flat-square">
   <img src="https://img.shields.io/badge/Open%20Source-NO-green?style=flat-square">
   <img src="https://img.shields.io/badge/Written%20In-Python-green?style=flat-square">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: arubomber Version: 2.1.6 Summary: SMS Bomber
+Metadata-Version: 2.1 Name: arubomber Version: 2.1.7 Summary: SMS Bomber
 Project. Home-page: https://github.com/Aru-Ofc-git/ARU-BOMBER.git Author:
 Ariful Islam Arman Author-email: arifulislamarman02@gmail.com Project-URL: Bug
 Tracker, https://github.com/Aru-Ofc-git Classifier: Development Status :: 5 -
 Production/Stable Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.5 Classifier: Programming Language ::
 Python Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE
                        ****** SMS BOMBING SYSTEM ******
-[https://img.shields.io/badge/Version-2.1.6-orange?style=for-the-badge] [https:
+[https://img.shields.io/badge/Version-2.1.7-orange?style=for-the-badge] [https:
   //img.shields.io/github/license/Aru-Ofc-git/ARU-BOMBER?style=for-the-badge]
   [https://img.shields.io/badge/Author-ARU-green?style=flat-square] [https://
    img.shields.io/badge/Open%20Source-NO-green?style=flat-square] [https://
        img.shields.io/badge/Written%20In-Python-green?style=flat-square]
              **** If You need any Help please connect with us ****
 `` ð¡ Get in Touch ``
 [LinkedIn] [Instagram] [Twitter] [Spotify] [YouTube] [DEV.to] [Gmail] [Github]
```

