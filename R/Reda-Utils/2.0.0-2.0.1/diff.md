# Comparing `tmp/Reda_Utils-2.0.0-py2-none-any.whl.zip` & `tmp/Reda_Utils-2.0.1-py2-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5440 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    15113 b- defN 23-May-04 08:00 Reda_Utils/Reda_Utils.py
+Zip file size: 5433 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    15113 b- defN 23-May-04 08:07 Reda_Utils/Reda_Utils.py
 -rw-rw-r--  2.0 unx       17 b- defN 22-Sep-26 06:33 Reda_Utils/__init__.py
--rw-rw-r--  2.0 unx     1788 b- defN 23-May-04 08:02 Reda_Utils-2.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-04 08:02 Reda_Utils-2.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-May-04 08:02 Reda_Utils-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      469 b- defN 23-May-04 08:02 Reda_Utils-2.0.0.dist-info/RECORD
-6 files, 17490 bytes uncompressed, 4590 bytes compressed:  73.8%
+-rw-rw-r--  2.0 unx     1788 b- defN 23-May-04 08:09 Reda_Utils-2.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-04 08:09 Reda_Utils-2.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-04 08:09 Reda_Utils-2.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      469 b- defN 23-May-04 08:09 Reda_Utils-2.0.1.dist-info/RECORD
+6 files, 17490 bytes uncompressed, 4583 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: Reda_Utils/Reda_Utils.py
 Comment: 
 
 Filename: Reda_Utils/__init__.py
 Comment: 
 
-Filename: Reda_Utils-2.0.0.dist-info/METADATA
+Filename: Reda_Utils-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: Reda_Utils-2.0.0.dist-info/WHEEL
+Filename: Reda_Utils-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: Reda_Utils-2.0.0.dist-info/top_level.txt
+Filename: Reda_Utils-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: Reda_Utils-2.0.0.dist-info/RECORD
+Filename: Reda_Utils-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Reda_Utils/Reda_Utils.py

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/python
 
 """
 Autor: REDA KASTITE
-version: 1.1.0
+version: 2.0.1
 Python_version: 2.7.17
 """
 
 import os,rospy
 import requests
 import math
 import geometry_msgs.msg
```

## Comparing `Reda_Utils-2.0.0.dist-info/METADATA` & `Reda_Utils-2.0.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: Reda-Utils
-Version: 2.0.0
+Version: 2.0.1
 Summary: Paquete funciones utiles Navegacion Robot
 Home-page: https://github.com/r3dkas/Reda_Utils
 Author: Reda Kastite
 Author-email: reda_kastite@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 
 Autor: REDA KASTITE
-version: 2.0.0
+version: 2.0.1
 Python_version: 2.7.17
 
 Coleccion de funciones. 
 
     Contiene:
 
     + Funcion lectura de archivo de parametros con formato object y publicacion en param server. [leer_Config()]
```

