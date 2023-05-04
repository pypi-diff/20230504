# Comparing `tmp/SDTcloud-0.1.7.tar.gz` & `tmp/SDTcloud-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.1.7.tar", last modified: Thu May  4 08:04:44 2023, max compression
+gzip compressed data, was "SDTcloud-0.1.8.tar", last modified: Thu May  4 08:06:20 2023, max compression
```

## Comparing `SDTcloud-0.1.7.tar` & `SDTcloud-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:04:44.912683 SDTcloud-0.1.7/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 08:04:44.912532 SDTcloud-0.1.7/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.7/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:04:44.911625 SDTcloud-0.1.7/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.7/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)    10846 2023-05-04 08:04:22.000000 SDTcloud-0.1.7/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:04:44.912334 SDTcloud-0.1.7/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 08:04:44.000000 SDTcloud-0.1.7/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 08:04:44.000000 SDTcloud-0.1.7/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 08:04:44.000000 SDTcloud-0.1.7/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 08:04:44.000000 SDTcloud-0.1.7/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 08:04:44.912715 SDTcloud-0.1.7/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 08:04:42.000000 SDTcloud-0.1.7/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:06:20.198544 SDTcloud-0.1.8/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 08:06:20.198356 SDTcloud-0.1.8/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-05-04 01:12:59.000000 SDTcloud-0.1.8/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:06:20.196930 SDTcloud-0.1.8/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-05-04 01:12:59.000000 SDTcloud-0.1.8/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)    10861 2023-05-04 08:06:09.000000 SDTcloud-0.1.8/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-04 08:06:20.198063 SDTcloud-0.1.8/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-04 08:06:20.000000 SDTcloud-0.1.8/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-05-04 08:06:20.000000 SDTcloud-0.1.8/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-05-04 08:06:20.000000 SDTcloud-0.1.8/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-05-04 08:06:20.000000 SDTcloud-0.1.8/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-05-04 08:06:20.198588 SDTcloud-0.1.8/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-05-04 08:06:16.000000 SDTcloud-0.1.8/setup.py
```

### Comparing `SDTcloud-0.1.7/SDTcloud/sdtcloud.py` & `SDTcloud-0.1.8/SDTcloud/sdtcloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import getpass
 import json
+import sys
 import pandas as pd 
 
 from datetime import datetime, timezone, timedelta
 
 class SDTcloud():
     def __init__(self):
         print("Please enter your config information.")
@@ -51,15 +52,15 @@
             return 0, "500"
         elif status_code == 200:
             return 1, "Ok!!!, Status: 200"
         elif status_code == 201:
             return 2, "Created!!!, Status: 200"
         elif status_code == 204:
             print("No Content!!!, Status: 200")
-            exit()
+            sys.exit()
         else:
             return 0, ""
            
     def config(self, address, port):
         """ Setting config information.
 
         Args:
```

### Comparing `SDTcloud-0.1.7/setup.py` & `SDTcloud-0.1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.1.7",
+    version="0.1.8",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

