# Comparing `tmp/medical_image-0.0.8.tar.gz` & `tmp/medical_image-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medical_image-0.0.8.tar", last modified: Mon Mar 28 11:58:32 2022, max compression
+gzip compressed data, was "medical_image-0.0.9.tar", last modified: Mon Mar 28 13:16:47 2022, max compression
```

## Comparing `medical_image-0.0.8.tar` & `medical_image-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2022-03-28 11:58:32.624168 medical_image-0.0.8/
--rw-rw-r--   0 deep      (1000) deep      (1000)      303 2022-03-28 11:58:32.624168 medical_image-0.0.8/PKG-INFO
--rw-rw-r--   0 deep      (1000) deep      (1000)       16 2022-03-25 06:41:46.000000 medical_image-0.0.8/README.md
-drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2022-03-28 11:58:32.624168 medical_image-0.0.8/medical_image/
--rw-rw-r--   0 deep      (1000) deep      (1000)      116 2022-03-28 11:57:08.000000 medical_image-0.0.8/medical_image/__init__.py
--rw-rw-r--   0 deep      (1000) deep      (1000)    37439 2022-03-28 11:15:13.000000 medical_image-0.0.8/medical_image/generate_dcm.py
--rw-rw-r--   0 deep      (1000) deep      (1000)    19272 2022-03-28 11:04:31.000000 medical_image-0.0.8/medical_image/utils.py
-drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2022-03-28 11:58:32.624168 medical_image-0.0.8/medical_image.egg-info/
--rw-rw-r--   0 deep      (1000) deep      (1000)      303 2022-03-28 11:58:32.000000 medical_image-0.0.8/medical_image.egg-info/PKG-INFO
--rw-rw-r--   0 deep      (1000) deep      (1000)      281 2022-03-28 11:58:32.000000 medical_image-0.0.8/medical_image.egg-info/SOURCES.txt
--rw-rw-r--   0 deep      (1000) deep      (1000)        1 2022-03-28 11:58:32.000000 medical_image-0.0.8/medical_image.egg-info/dependency_links.txt
--rw-rw-r--   0 deep      (1000) deep      (1000)       93 2022-03-28 11:58:32.000000 medical_image-0.0.8/medical_image.egg-info/requires.txt
--rw-rw-r--   0 deep      (1000) deep      (1000)       14 2022-03-28 11:58:32.000000 medical_image-0.0.8/medical_image.egg-info/top_level.txt
--rw-rw-r--   0 deep      (1000) deep      (1000)       38 2022-03-28 11:58:32.624168 medical_image-0.0.8/setup.cfg
--rw-rw-r--   0 deep      (1000) deep      (1000)      804 2022-03-28 11:04:31.000000 medical_image-0.0.8/setup.py
+drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2022-03-28 13:16:47.488388 medical_image-0.0.9/
+-rw-rw-r--   0 deep      (1000) deep      (1000)      303 2022-03-28 13:16:47.484388 medical_image-0.0.9/PKG-INFO
+-rw-rw-r--   0 deep      (1000) deep      (1000)       16 2022-03-25 06:41:46.000000 medical_image-0.0.9/README.md
+drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2022-03-28 13:16:47.484388 medical_image-0.0.9/medical_image/
+-rw-rw-r--   0 deep      (1000) deep      (1000)      116 2022-03-28 13:16:30.000000 medical_image-0.0.9/medical_image/__init__.py
+-rw-rw-r--   0 deep      (1000) deep      (1000)    37439 2022-03-28 13:16:17.000000 medical_image-0.0.9/medical_image/generate_dcm.py
+-rw-rw-r--   0 deep      (1000) deep      (1000)    19272 2022-03-28 11:04:31.000000 medical_image-0.0.9/medical_image/utils.py
+drwxrwxr-x   0 deep      (1000) deep      (1000)        0 2022-03-28 13:16:47.484388 medical_image-0.0.9/medical_image.egg-info/
+-rw-rw-r--   0 deep      (1000) deep      (1000)      303 2022-03-28 13:16:47.000000 medical_image-0.0.9/medical_image.egg-info/PKG-INFO
+-rw-rw-r--   0 deep      (1000) deep      (1000)      281 2022-03-28 13:16:47.000000 medical_image-0.0.9/medical_image.egg-info/SOURCES.txt
+-rw-rw-r--   0 deep      (1000) deep      (1000)        1 2022-03-28 13:16:47.000000 medical_image-0.0.9/medical_image.egg-info/dependency_links.txt
+-rw-rw-r--   0 deep      (1000) deep      (1000)       93 2022-03-28 13:16:47.000000 medical_image-0.0.9/medical_image.egg-info/requires.txt
+-rw-rw-r--   0 deep      (1000) deep      (1000)       14 2022-03-28 13:16:47.000000 medical_image-0.0.9/medical_image.egg-info/top_level.txt
+-rw-rw-r--   0 deep      (1000) deep      (1000)       38 2022-03-28 13:16:47.488388 medical_image-0.0.9/setup.cfg
+-rw-rw-r--   0 deep      (1000) deep      (1000)      804 2022-03-28 11:04:31.000000 medical_image-0.0.9/setup.py
```

### Comparing `medical_image-0.0.8/medical_image/generate_dcm.py` & `medical_image-0.0.9/medical_image/generate_dcm.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         if self.write_version:
             msg += ' v.' + self.app_version
         mw, mh = mfont.getsize(msg)
         ## Logo
         # logo_w = self.logo.size[0] * result_json['Height'] * 0.55 / 2472
         # logo_h = self.logo.size[1] * result_json['Height'] * 0.55 / 2472
         logo_w = mw
-        logo_h = self.logo_size[1] * mw / self.logo_size[0]
+        logo_h = self.logo.size[1] * mw / self.logo.size[0]
         # x = (result_json['Width'] - logo_w) / 2
         x = result_json['Width'] * 0.97 - logo_w
         y = result_json['Height'] * 0.97 - logo_h
         paste_image(image, self.logo, x, y, logo_w, logo_h, 1)
 
         ## App Info
         # x = (result_json['Width'] - mw) / 2
```

### Comparing `medical_image-0.0.8/medical_image/utils.py` & `medical_image-0.0.9/medical_image/utils.py`

 * *Files identical despite different names*

### Comparing `medical_image-0.0.8/setup.py` & `medical_image-0.0.9/setup.py`

 * *Files identical despite different names*

