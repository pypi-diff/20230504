# Comparing `tmp/vectorGPTBot-0.1.2.tar.gz` & `tmp/vectorGPTBot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorGPTBot-0.1.2.tar", last modified: Thu May  4 17:00:15 2023, max compression
+gzip compressed data, was "vectorGPTBot-0.1.4.tar", last modified: Thu May  4 17:20:24 2023, max compression
```

## Comparing `vectorGPTBot-0.1.2.tar` & `vectorGPTBot-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0     1000     1000        0 2023-05-04 17:00:15.148243 vectorGPTBot-0.1.2/
--rwxrwxrwx   0     1000     1000      782 2023-05-04 17:00:15.143272 vectorGPTBot-0.1.2/PKG-INFO
--rwxrwxrwx   0     1000     1000       38 2023-05-04 17:00:15.150272 vectorGPTBot-0.1.2/setup.cfg
--rwxrwxrwx   0     1000     1000     1041 2023-05-04 16:59:57.000000 vectorGPTBot-0.1.2/setup.py
-drwxrwxrwx   0     1000     1000        0 2023-05-04 17:00:14.886402 vectorGPTBot-0.1.2/vectorGPTBot/
-drwxrwxrwx   0     1000     1000        0 2023-05-04 17:00:15.098523 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/
--rwxrwxrwx   0     1000     1000      782 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000      252 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000       33 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000        1 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/top_level.txt
+drwxrwxrwx   0     1000     1000        0 2023-05-04 17:20:24.241232 vectorGPTBot-0.1.4/
+-rwxrwxrwx   0     1000     1000      782 2023-05-04 17:20:24.237705 vectorGPTBot-0.1.4/PKG-INFO
+-rwxrwxrwx   0     1000     1000       38 2023-05-04 17:20:24.242257 vectorGPTBot-0.1.4/setup.cfg
+-rwxrwxrwx   0     1000     1000     1041 2023-05-04 17:19:48.000000 vectorGPTBot-0.1.4/setup.py
+drwxrwxrwx   0     1000     1000        0 2023-05-04 17:20:24.043167 vectorGPTBot-0.1.4/vectorGPTBot/
+drwxrwxrwx   0     1000     1000        0 2023-05-04 17:20:24.209812 vectorGPTBot-0.1.4/vectorGPTBot/vectorGPTBot.egg-info/
+-rwxrwxrwx   0     1000     1000      782 2023-05-04 17:20:23.000000 vectorGPTBot-0.1.4/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      252 2023-05-04 17:20:23.000000 vectorGPTBot-0.1.4/vectorGPTBot/vectorGPTBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2023-05-04 17:20:23.000000 vectorGPTBot-0.1.4/vectorGPTBot/vectorGPTBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       33 2023-05-04 17:20:23.000000 vectorGPTBot-0.1.4/vectorGPTBot/vectorGPTBot.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        1 2023-05-04 17:20:23.000000 vectorGPTBot-0.1.4/vectorGPTBot/vectorGPTBot.egg-info/top_level.txt
```

### Comparing `vectorGPTBot-0.1.2/PKG-INFO` & `vectorGPTBot-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorGPTBot
-Version: 0.1.2
+Version: 0.1.4
 Summary: A sample vectorGPTBot
 Home-page: UNKNOWN
 Author: wstart
 License: Apache License 2.0
 Keywords: vectorGPTBot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vectorGPTBot-0.1.2/setup.py` & `vectorGPTBot-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vectorGPTBot',
-    version='0.1.2',
+    version='0.1.4',
     author='wstart',
     description='A sample vectorGPTBot',
     long_description='A sample vectorGPTBot',
     long_description_content_type="text/markdown",
     packages=find_packages('vectorGPTBot'),
     package_dir={'': 'vectorGPTBot'},
     install_requires=[
```

### Comparing `vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO` & `vectorGPTBot-0.1.4/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorGPTBot
-Version: 0.1.2
+Version: 0.1.4
 Summary: A sample vectorGPTBot
 Home-page: UNKNOWN
 Author: wstart
 License: Apache License 2.0
 Keywords: vectorGPTBot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

