# Comparing `tmp/ImageMagic-0.1.3.tar.gz` & `tmp/ImageMagic-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageMagic-0.1.3.tar", last modified: Thu May  4 09:35:03 2023, max compression
+gzip compressed data, was "ImageMagic-0.1.5.tar", last modified: Thu May  4 13:03:12 2023, max compression
```

## Comparing `ImageMagic-0.1.3.tar` & `ImageMagic-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 09:35:03.627779 ImageMagic-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-05-04 09:35:03.612155 ImageMagic-0.1.3/ImageMagic/
--rw-rw-rw-   0        0        0     6183 2023-05-04 09:25:12.000000 ImageMagic-0.1.3/ImageMagic/Aocr.py
--rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.3/ImageMagic/Atesseract.py
--rw-rw-rw-   0        0        0    10110 2023-05-04 09:07:20.000000 ImageMagic-0.1.3/ImageMagic/Image.py
--rw-rw-rw-   0        0        0      260 2023-05-04 09:25:10.000000 ImageMagic-0.1.3/ImageMagic/__init__.py
--rw-rw-rw-   0        0        0       85 2023-05-04 09:25:12.000000 ImageMagic-0.1.3/ImageMagic/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:35:03.627779 ImageMagic-0.1.3/ImageMagic.egg-info/
--rw-rw-rw-   0        0        0      245 2023-05-04 09:35:03.000000 ImageMagic-0.1.3/ImageMagic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-04 09:35:03.000000 ImageMagic-0.1.3/ImageMagic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:35:03.000000 ImageMagic-0.1.3/ImageMagic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-04 09:35:03.000000 ImageMagic-0.1.3/ImageMagic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 09:35:03.000000 ImageMagic-0.1.3/ImageMagic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      245 2023-05-04 09:35:03.627779 ImageMagic-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-05-04 05:13:53.000000 ImageMagic-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 09:35:03.627779 ImageMagic-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-05-04 09:34:50.000000 ImageMagic-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/ImageMagic/
+-rw-rw-rw-   0        0        0     6184 2023-05-04 12:40:18.000000 ImageMagic-0.1.5/ImageMagic/Aocr.py
+-rw-rw-rw-   0        0        0    10110 2023-05-04 09:07:20.000000 ImageMagic-0.1.5/ImageMagic/Image.py
+-rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.5/ImageMagic/_Atesseract.py
+-rw-rw-rw-   0        0        0      260 2023-05-04 12:55:21.000000 ImageMagic-0.1.5/ImageMagic/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-05-04 09:25:12.000000 ImageMagic-0.1.5/ImageMagic/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/ImageMagic.egg-info/
+-rw-rw-rw-   0        0        0      245 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-04 13:03:12.000000 ImageMagic-0.1.5/ImageMagic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      245 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2023-05-04 09:42:24.000000 ImageMagic-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:03:12.953890 ImageMagic-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-05-04 13:03:00.000000 ImageMagic-0.1.5/setup.py
```

### Comparing `ImageMagic-0.1.3/ImageMagic/Aocr.py` & `ImageMagic-0.1.5/ImageMagic/Aocr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ImageMagic.Atesseract import *
+from ImageMagic._Atesseract import *
 from PIL import Image
 
 
 
 def image_to_text(filePath,lang='chi_sim',config='',nice=0,output_type=Output.STRING,timeout=0,):
 
     """
```

### Comparing `ImageMagic-0.1.3/ImageMagic/Atesseract.py` & `ImageMagic-0.1.5/ImageMagic/_Atesseract.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.3/ImageMagic/Image.py` & `ImageMagic-0.1.5/ImageMagic/Image.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.3/LICENSE` & `ImageMagic-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.3/README.md` & `ImageMagic-0.1.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 <div align="center">
   <img src="https://i.328888.xyz/2023/05/04/iPlOg8.png" width="500" height="450"><br>
 </div>
 
 # ImageMagic:一个简洁的图像（包括但不限于）处理库
-[![Pypi](https://img.shields.io/badge/pypi-0.1.0-blue)]()
+[![Pypi](https://img.shields.io/badge/pypi-0.1.3-blue)]()
 [![License](https://img.shields.io/badge/license-MIT-yellow)]()
 [![]()]()
 
 # 这是什么？
 ImageMagic是Python的一个包，提供简洁的图像（包括但不限于）处理功能，主要体现为简洁二字。
 
 # 获取
+1. 使用pip下载
+```
+pip install ImageMagic
+```
+
+2. 或者，你也可以从[源](https://github.com/asxez/ImageMagic)进行构建
 
 # 依赖
   - [PIL](https://github.com/python-pillow/Pillow)
   - [Tesseract-OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html)
-
+  - [numpy](https://github.com/numpy/numpy)
+  - [pandas](https://github.com/pandas-dev/pandas)
+  - ……
 
 # 许可证
 GNU GPL
 
 # 为ImageMagic做贡献
 欢迎所有贡献、错误报告、错误修复以及功能增强和想法。
```

