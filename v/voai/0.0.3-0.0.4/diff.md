# Comparing `tmp/voai-0.0.3.tar.gz` & `tmp/voai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voai-0.0.3.tar", last modified: Mon Apr 10 10:36:57 2023, max compression
+gzip compressed data, was "voai-0.0.4.tar", last modified: Thu May  4 17:09:40 2023, max compression
```

## Comparing `voai-0.0.3.tar` & `voai-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 10:36:57.533541 voai-0.0.3/
--rw-rw-rw-   0        0        0    11558 2023-04-09 17:36:21.000000 voai-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      947 2023-04-10 10:36:57.532542 voai-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-04-10 10:36:02.000000 voai-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 10:36:57.533541 voai-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-04-10 10:36:09.000000 voai-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 10:36:57.528043 voai-0.0.3/voai/
-drwxrwxrwx   0        0        0        0 2023-04-10 10:36:57.531548 voai-0.0.3/voai/voai.egg-info/
--rw-rw-rw-   0        0        0      947 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-10 10:36:57.000000 voai-0.0.3/voai/voai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2848 2023-04-10 10:31:17.000000 voai-0.0.3/voai/voai.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:09:40.535068 voai-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2023-04-09 17:36:21.000000 voai-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1396 2023-05-04 17:09:40.534067 voai-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      917 2023-05-04 17:07:57.000000 voai-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:09:40.535068 voai-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2023-05-04 17:09:01.000000 voai-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 17:09:40.528067 voai-0.0.4/voai/
+drwxrwxrwx   0        0        0        0 2023-05-04 17:09:40.533067 voai-0.0.4/voai/voai.egg-info/
+-rw-rw-rw-   0        0        0     1396 2023-05-04 17:09:40.000000 voai-0.0.4/voai/voai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-05-04 17:09:40.000000 voai-0.0.4/voai/voai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:09:40.000000 voai-0.0.4/voai/voai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-04 17:09:40.000000 voai-0.0.4/voai/voai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-04 17:09:40.000000 voai-0.0.4/voai/voai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4248 2023-05-04 16:40:31.000000 voai-0.0.4/voai/voai.py
```

### Comparing `voai-0.0.3/LICENSE` & `voai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voai-0.0.3/setup.py` & `voai-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 import sys
 
 classifiers = [
   "Operating System :: OS Independent",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
 ]
@@ -14,15 +14,15 @@
     sys.stderr.write(
         f"""Current python version ({CURRENT_VERSION[0]}.{CURRENT_VERSION[1]}) is lower than required ({REQUIRED_VERSION[0]}.{REQUIRED_VERSION[1]})
         """
     )
 
 setup(
     name="voai",
-    version="0.0.3",
+    version="0.0.4",
     description="A tool designed for working with 🧑‍💻ChatGPT API🧑‍💻",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/CURVoid/voai",
     author="VOID",
     license="APACHE 2.0", 
     keywords=["chatgpt", "gpt", "chat", "voai", "openai", "ai"],
```

