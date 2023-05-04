# Comparing `tmp/vectorGPTBot-0.1.0.tar.gz` & `tmp/vectorGPTBot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorGPTBot-0.1.0.tar", last modified: Thu May  4 15:38:11 2023, max compression
+gzip compressed data, was "vectorGPTBot-0.1.1.tar", last modified: Thu May  4 15:46:48 2023, max compression
```

## Comparing `vectorGPTBot-0.1.0.tar` & `vectorGPTBot-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0     1000     1000        0 2023-05-04 15:38:11.292241 vectorGPTBot-0.1.0/
--rwxrwxrwx   0     1000     1000      713 2023-05-04 15:38:11.288030 vectorGPTBot-0.1.0/PKG-INFO
--rwxrwxrwx   0     1000     1000       38 2023-05-04 15:38:11.293280 vectorGPTBot-0.1.0/setup.cfg
--rwxrwxrwx   0     1000     1000      929 2023-05-04 15:37:13.000000 vectorGPTBot-0.1.0/setup.py
-drwxrwxrwx   0     1000     1000        0 2023-05-04 15:38:11.048145 vectorGPTBot-0.1.0/vectorGPTBot/
-drwxrwxrwx   0     1000     1000        0 2023-05-04 15:38:11.239342 vectorGPTBot-0.1.0/vectorGPTBot/vectorGPTBot.egg-info/
--rwxrwxrwx   0     1000     1000      713 2023-05-04 15:38:10.000000 vectorGPTBot-0.1.0/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000      252 2023-05-04 15:38:10.000000 vectorGPTBot-0.1.0/vectorGPTBot/vectorGPTBot.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2023-05-04 15:38:10.000000 vectorGPTBot-0.1.0/vectorGPTBot/vectorGPTBot.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000       33 2023-05-04 15:38:10.000000 vectorGPTBot-0.1.0/vectorGPTBot/vectorGPTBot.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000        1 2023-05-04 15:38:10.000000 vectorGPTBot-0.1.0/vectorGPTBot/vectorGPTBot.egg-info/top_level.txt
+drwxrwxrwx   0     1000     1000        0 2023-05-04 15:46:48.213184 vectorGPTBot-0.1.1/
+-rwxrwxrwx   0     1000     1000      713 2023-05-04 15:46:48.209165 vectorGPTBot-0.1.1/PKG-INFO
+-rwxrwxrwx   0     1000     1000       38 2023-05-04 15:46:48.215180 vectorGPTBot-0.1.1/setup.cfg
+-rwxrwxrwx   0     1000     1000      929 2023-05-04 15:46:17.000000 vectorGPTBot-0.1.1/setup.py
+drwxrwxrwx   0     1000     1000        0 2023-05-04 15:46:47.968356 vectorGPTBot-0.1.1/vectorGPTBot/
+drwxrwxrwx   0     1000     1000        0 2023-05-04 15:46:48.167205 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/
+-rwxrwxrwx   0     1000     1000      713 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      252 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       33 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        1 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/top_level.txt
```

### Comparing `vectorGPTBot-0.1.0/PKG-INFO` & `vectorGPTBot-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorGPTBot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A sample vectorGPTBot
 Home-page: UNKNOWN
 Author: wstart
 License: MIT
 Keywords: vectorGPTBot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vectorGPTBot-0.1.0/setup.py` & `vectorGPTBot-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vectorGPTBot',
-    version='0.1.0',
+    version='0.1.1',
     author='wstart',
     description='A sample vectorGPTBot',
     packages=find_packages('vectorGPTBot'),
     package_dir={'': 'vectorGPTBot'},
     install_requires=[
         'chromadb',
         'modelscope',
```

### Comparing `vectorGPTBot-0.1.0/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO` & `vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorGPTBot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A sample vectorGPTBot
 Home-page: UNKNOWN
 Author: wstart
 License: MIT
 Keywords: vectorGPTBot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

