# Comparing `tmp/MarkMyImage-0.1.7.tar.gz` & `tmp/MarkMyImage-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarkMyImage-0.1.7.tar", last modified: Thu Apr 27 12:38:34 2023, max compression
+gzip compressed data, was "MarkMyImage-0.1.8.tar", last modified: Thu May  4 20:21:27 2023, max compression
```

## Comparing `MarkMyImage-0.1.7.tar` & `MarkMyImage-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/
-drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/MarkMyImage/
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     4135 2023-04-27 12:36:14.000000 MarkMyImage-0.1.7/MarkMyImage/__init__.py
-drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/MarkMyImage.egg-info/
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     2208 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/PKG-INFO
--rw-rw-r--   0 alatas    (1001) alatas    (1001)      254 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/SOURCES.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)        1 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/dependency_links.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       41 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/entry_points.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       14 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/requires.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       12 2023-04-27 12:38:34.000000 MarkMyImage-0.1.7/MarkMyImage.egg-info/top_level.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     2208 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/PKG-INFO
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     1595 2023-04-27 12:38:10.000000 MarkMyImage-0.1.7/README.md
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       38 2023-04-27 12:38:34.875712 MarkMyImage-0.1.7/setup.cfg
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     1013 2023-04-27 12:38:33.000000 MarkMyImage-0.1.7/setup.py
+drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-05-04 20:21:27.601268 MarkMyImage-0.1.8/
+drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-05-04 20:21:27.601268 MarkMyImage-0.1.8/MarkMyImage/
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     3752 2023-05-04 20:19:25.000000 MarkMyImage-0.1.8/MarkMyImage/__init__.py
+drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-05-04 20:21:27.601268 MarkMyImage-0.1.8/MarkMyImage.egg-info/
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     2208 2023-05-04 20:21:27.000000 MarkMyImage-0.1.8/MarkMyImage.egg-info/PKG-INFO
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)      254 2023-05-04 20:21:27.000000 MarkMyImage-0.1.8/MarkMyImage.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)        1 2023-05-04 20:21:27.000000 MarkMyImage-0.1.8/MarkMyImage.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       41 2023-05-04 20:21:27.000000 MarkMyImage-0.1.8/MarkMyImage.egg-info/entry_points.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)        7 2023-05-04 20:21:27.000000 MarkMyImage-0.1.8/MarkMyImage.egg-info/requires.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       12 2023-05-04 20:21:27.000000 MarkMyImage-0.1.8/MarkMyImage.egg-info/top_level.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     2208 2023-05-04 20:21:27.601268 MarkMyImage-0.1.8/PKG-INFO
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     1595 2023-04-27 12:38:10.000000 MarkMyImage-0.1.8/README.md
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       38 2023-05-04 20:21:27.601268 MarkMyImage-0.1.8/setup.cfg
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     1003 2023-05-04 20:20:36.000000 MarkMyImage-0.1.8/setup.py
```

### Comparing `MarkMyImage-0.1.7/MarkMyImage/__init__.py` & `MarkMyImage-0.1.8/MarkMyImage/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,23 @@
 import os
 import argparse
 import logging
 from PIL import Image, ImageEnhance, ImageFile
-import pyheif
 
 ImageFile.LOAD_TRUNCATED_IMAGES = True
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
 def apply_transparency(watermark, transparency):
     alpha = watermark.split()[3]
     alpha = ImageEnhance.Brightness(alpha).enhance(transparency)
     watermark.putalpha(alpha)
     return watermark
 
 
-def open_heic_image(image_path):
-    heif_file = pyheif.read(image_path)
-    return Image.frombytes(
-        heif_file.mode,
-        heif_file.size,
-        heif_file.data,
-        "raw",
-        heif_file.mode,
-    )
-
-
 def add_watermark(input_folder, watermark_path, output_folder, position, transparency, rotation_angle, logo_scale):
     if not os.path.exists(output_folder):
         logging.info(f"Specified output_folder does not exist, it will be created -> {output_folder}.")
         os.makedirs(output_folder)
 
     try:
         watermark = Image.open(watermark_path).convert("RGBA")
@@ -40,25 +28,22 @@
         logging.error(f"Unable to open watermark file: {watermark_path}")
         return
 
     watermark = apply_transparency(watermark, transparency)
 
     for item in os.listdir(input_folder):
 
-        if not item.endswith((".jpg", ".jpeg", ".png", ".heic")):
-            logging.info(f"File {item} is not supported. Only jpg, jpeg, heic and png files allowed")
+        if not item.endswith((".jpg", ".jpeg", ".png")):
+            logging.info(f"File {item} is not supported. Only jpg, jpeg and png files allowed")
             continue
 
         logging.info(f'Processing image: {item}')
         image_path = os.path.join(input_folder, item)
         try:
-            if item.lower().endswith(".heic"):
-                img = open_heic_image(image_path).convert("RGB")
-            else:
-                img = Image.open(image_path).convert("RGB")
+            img = Image.open(image_path).convert("RGB")
         except IOError:
             logging.error(f"Unable to open image file: {image_path}")
             continue
 
         # Adjust logo size in relation to the image size
         ratio = min(img.width, img.height) * logo_scale / max(watermark.width, watermark.height)
         new_size = (int(watermark.width * ratio), int(watermark.height * ratio))
```

### Comparing `MarkMyImage-0.1.7/MarkMyImage.egg-info/PKG-INFO` & `MarkMyImage-0.1.8/MarkMyImage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarkMyImage
-Version: 0.1.7
+Version: 0.1.8
 Summary: Add a watermark to all images in a folder.
 Author: Lomezno
 Author-email: dbwspain@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MarkMyImage-0.1.7/PKG-INFO` & `MarkMyImage-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarkMyImage
-Version: 0.1.7
+Version: 0.1.8
 Summary: Add a watermark to all images in a folder.
 Author: Lomezno
 Author-email: dbwspain@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MarkMyImage-0.1.7/README.md` & `MarkMyImage-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `MarkMyImage-0.1.7/setup.py` & `MarkMyImage-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MarkMyImage",
-    version="0.1.7",
+    version="0.1.8",
     description="Add a watermark to all images in a folder.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Lomezno",
     author_email="dbwspain@gmail.com",
     packages=find_packages(),
-    install_requires=["Pillow", "pyheif"],
+    install_requires=["Pillow"],
     entry_points={
         "console_scripts": [
             "mmi=MarkMyImage:main",
         ],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
```

