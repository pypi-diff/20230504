# Comparing `tmp/aij-webcam-1.0.1.tar.gz` & `tmp/aij-webcam-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.0.1.tar", last modified: Thu May  4 09:33:06 2023, max compression
+gzip compressed data, was "aij-webcam-1.0.2.tar", last modified: Thu May  4 09:42:19 2023, max compression
```

## Comparing `aij-webcam-1.0.1.tar` & `aij-webcam-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.1/README.md
--rw-rw-rw-   0        0        0     6310 2023-05-04 09:32:52.000000 aij-webcam-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 09:33:08.000000 aij-webcam-1.0.1/src/webcam/
--rw-rw-rw-   0        0        0      152 2023-05-04 09:32:04.000000 aij-webcam-1.0.1/src/webcam/__init__.py
--rw-rw-rw-   0        0        0     9334 2023-05-04 09:21:02.000000 aij-webcam-1.0.1/src/webcam/player.py
+drwxrwxrwx   0        0        0        0 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-webcam-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-03 23:28:50.000000 aij-webcam-1.0.2/README.md
+-rw-rw-rw-   0        0        0     6310 2023-05-04 09:42:04.000000 aij-webcam-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 09:42:20.000000 aij-webcam-1.0.2/src/webcam/
+-rw-rw-rw-   0        0        0     9656 2023-05-04 09:41:56.000000 aij-webcam-1.0.2/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.0.1/LICENSE.txt` & `aij-webcam-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.1/PKG-INFO` & `aij-webcam-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.1
+Version: 1.0.2
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.0.1/README.md` & `aij-webcam-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.0.1/pyproject.toml` & `aij-webcam-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.1"
+version = "1.0.2"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-webcam-1.0.1/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.0.2/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.0.1
+Version: 1.0.2
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

