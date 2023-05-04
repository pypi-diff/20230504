# Comparing `tmp/aij-webcam-1.0.6.tar.gz` & `tmp/aij-webcam-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.0.6.tar", last modified: Thu May  4 10:19:21 2023, max compression
+gzip compressed data, was "aij-webcam-1.0.7.tar", last modified: Thu May  4 10:22:10 2023, max compression
```

## Comparing `aij-webcam-1.0.6.tar` & `aij-webcam-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.6/README.md
--rw-rw-rw-   0        0        0     6452 2023-05-04 10:19:12.000000 aij-webcam-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      161 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 10:19:22.000000 aij-webcam-1.0.6/src/webcam/
--rw-rw-rw-   0        0        0    11878 2023-05-04 10:19:02.000000 aij-webcam-1.0.6/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.7/README.md
+-rw-rw-rw-   0        0        0     6452 2023-05-04 10:22:02.000000 aij-webcam-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      161 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 10:22:12.000000 aij-webcam-1.0.7/src/webcam/
+-rw-rw-rw-   0        0        0    12135 2023-05-04 10:21:52.000000 aij-webcam-1.0.7/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.0.6/LICENSE.txt` & `aij-webcam-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.6/PKG-INFO` & `aij-webcam-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.6
+Version: 1.0.7
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.6/README.md` & `aij-webcam-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.6/pyproject.toml` & `aij-webcam-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.6"
+version = "1.0.7"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-webcam-1.0.6/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.0.7/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.6
+Version: 1.0.7
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.6/src/webcam/__init__.py` & `aij-webcam-1.0.7/src/webcam/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,28 @@
     """
     Build the required setup to run AIJ
     """
     # get the user profile path
     user_profile = os.environ['USERPROFILE']
     _sep = os.path.sep
 
-    # create a directory named '.aij' in the user profile
-    os.mkdir(user_profile + _sep + '.aij')
+    # create a directory named '.aij' in the user profile if not exists
+    if not os.path.exists(user_profile + _sep + '.aij'):
+        os.mkdir(user_profile + _sep + '.aij')
 
-    # create a file named 'config.json' in the directory
-    with open(user_profile + _sep + '.aij' + _sep + 'config.json', 'w', encoding="utf-8") as json_file:
-        json_file.write('{}')
+    # create a file named 'config.json' in the directory if not exists
+    config_home = user_profile + _sep + '.aij' + _sep + 'config.json'
+    if not os.path.exists(config_home):
+        with open(config_home, 'w', encoding="utf-8") as json_file:
+            json_file.write('{}')
 
-    # create a folder named 'data' to store audio files
-    os.mkdir(user_profile + _sep + '.aij' + _sep + 'data')
+    # create a folder named 'data' to store audio files if not exists
+    audio_home = user_profile + _sep + '.aij' + _sep + 'data'
+    if not os.path.exists(audio_home):
+        os.mkdir(audio_home)
         
 
 # build the required setup to run AIJ
 build_setup()
 
 # Using OpenCV to display the image
 cap = cv2.VideoCapture(0)
```

