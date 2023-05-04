# Comparing `tmp/ImageMagic-0.1.1.tar.gz` & `tmp/ImageMagic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageMagic-0.1.1.tar", last modified: Thu May  4 09:08:57 2023, max compression
+gzip compressed data, was "ImageMagic-0.1.2.tar", last modified: Thu May  4 09:29:50 2023, max compression
```

## Comparing `ImageMagic-0.1.1.tar` & `ImageMagic-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 09:08:57.316932 ImageMagic-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-05-04 09:08:57.316932 ImageMagic-0.1.1/ImageMagic.egg-info/
--rw-rw-rw-   0        0        0      245 2023-05-04 09:08:57.000000 ImageMagic-0.1.1/ImageMagic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-04 09:08:57.000000 ImageMagic-0.1.1/ImageMagic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:08:57.000000 ImageMagic-0.1.1/ImageMagic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-04 09:08:57.000000 ImageMagic-0.1.1/ImageMagic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:08:57.000000 ImageMagic-0.1.1/ImageMagic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      245 2023-05-04 09:08:57.316932 ImageMagic-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-05-04 05:13:53.000000 ImageMagic-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 09:08:57.316932 ImageMagic-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-05-04 08:30:48.000000 ImageMagic-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:29:50.312960 ImageMagic-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-05-04 09:29:50.312960 ImageMagic-0.1.2/ImageMagic.egg-info/
+-rw-rw-rw-   0        0        0      245 2023-05-04 09:29:50.000000 ImageMagic-0.1.2/ImageMagic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-04 09:29:50.000000 ImageMagic-0.1.2/ImageMagic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 09:29:50.000000 ImageMagic-0.1.2/ImageMagic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-04 09:29:50.000000 ImageMagic-0.1.2/ImageMagic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-04 09:29:50.000000 ImageMagic-0.1.2/ImageMagic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      245 2023-05-04 09:29:50.312960 ImageMagic-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2023-05-04 05:13:53.000000 ImageMagic-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 09:29:50.312960 ImageMagic-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-05-04 09:21:34.000000 ImageMagic-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:29:50.312960 ImageMagic-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 09:29:50.312960 ImageMagic-0.1.2/src/ImageMagic/
+-rw-rw-rw-   0        0        0     6183 2023-05-04 09:25:12.000000 ImageMagic-0.1.2/src/ImageMagic/Aocr.py
+-rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.2/src/ImageMagic/Atesseract.py
+-rw-rw-rw-   0        0        0    10110 2023-05-04 09:07:20.000000 ImageMagic-0.1.2/src/ImageMagic/Image.py
+-rw-rw-rw-   0        0        0      260 2023-05-04 09:25:10.000000 ImageMagic-0.1.2/src/ImageMagic/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-05-04 09:25:12.000000 ImageMagic-0.1.2/src/ImageMagic/_version.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 09:19:23.000000 ImageMagic-0.1.2/src/__init__.py
```

### Comparing `ImageMagic-0.1.1/LICENSE` & `ImageMagic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.1/README.md` & `ImageMagic-0.1.2/README.md`

 * *Files identical despite different names*

