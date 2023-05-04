# Comparing `tmp/vectorGPTBot-0.1.1.tar.gz` & `tmp/vectorGPTBot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorGPTBot-0.1.1.tar", last modified: Thu May  4 15:46:48 2023, max compression
+gzip compressed data, was "vectorGPTBot-0.1.2.tar", last modified: Thu May  4 17:00:15 2023, max compression
```

## Comparing `vectorGPTBot-0.1.1.tar` & `vectorGPTBot-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0     1000     1000        0 2023-05-04 15:46:48.213184 vectorGPTBot-0.1.1/
--rwxrwxrwx   0     1000     1000      713 2023-05-04 15:46:48.209165 vectorGPTBot-0.1.1/PKG-INFO
--rwxrwxrwx   0     1000     1000       38 2023-05-04 15:46:48.215180 vectorGPTBot-0.1.1/setup.cfg
--rwxrwxrwx   0     1000     1000      929 2023-05-04 15:46:17.000000 vectorGPTBot-0.1.1/setup.py
-drwxrwxrwx   0     1000     1000        0 2023-05-04 15:46:47.968356 vectorGPTBot-0.1.1/vectorGPTBot/
-drwxrwxrwx   0     1000     1000        0 2023-05-04 15:46:48.167205 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/
--rwxrwxrwx   0     1000     1000      713 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000      252 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000       33 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000        1 2023-05-04 15:46:47.000000 vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/top_level.txt
+drwxrwxrwx   0     1000     1000        0 2023-05-04 17:00:15.148243 vectorGPTBot-0.1.2/
+-rwxrwxrwx   0     1000     1000      782 2023-05-04 17:00:15.143272 vectorGPTBot-0.1.2/PKG-INFO
+-rwxrwxrwx   0     1000     1000       38 2023-05-04 17:00:15.150272 vectorGPTBot-0.1.2/setup.cfg
+-rwxrwxrwx   0     1000     1000     1041 2023-05-04 16:59:57.000000 vectorGPTBot-0.1.2/setup.py
+drwxrwxrwx   0     1000     1000        0 2023-05-04 17:00:14.886402 vectorGPTBot-0.1.2/vectorGPTBot/
+drwxrwxrwx   0     1000     1000        0 2023-05-04 17:00:15.098523 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/
+-rwxrwxrwx   0     1000     1000      782 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      252 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       33 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        1 2023-05-04 17:00:14.000000 vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/top_level.txt
```

### Comparing `vectorGPTBot-0.1.1/PKG-INFO` & `vectorGPTBot-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: vectorGPTBot
-Version: 0.1.1
+Version: 0.1.2
 Summary: A sample vectorGPTBot
 Home-page: UNKNOWN
 Author: wstart
-License: MIT
+License: Apache License 2.0
 Keywords: vectorGPTBot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Description-Content-Type: text/markdown
 
-UNKNOWN
+A sample vectorGPTBot
```

### Comparing `vectorGPTBot-0.1.1/setup.py` & `vectorGPTBot-0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vectorGPTBot',
-    version='0.1.1',
+    version='0.1.2',
     author='wstart',
     description='A sample vectorGPTBot',
+    long_description='A sample vectorGPTBot',
+    long_description_content_type="text/markdown",
     packages=find_packages('vectorGPTBot'),
     package_dir={'': 'vectorGPTBot'},
     install_requires=[
         'chromadb',
         'modelscope',
         'transformers'
     ],
@@ -21,9 +23,9 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     keywords='vectorGPTBot',
-    license='MIT',
+    license='Apache License 2.0',
 )
```

### Comparing `vectorGPTBot-0.1.1/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO` & `vectorGPTBot-0.1.2/vectorGPTBot/vectorGPTBot.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: vectorGPTBot
-Version: 0.1.1
+Version: 0.1.2
 Summary: A sample vectorGPTBot
 Home-page: UNKNOWN
 Author: wstart
-License: MIT
+License: Apache License 2.0
 Keywords: vectorGPTBot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Description-Content-Type: text/markdown
 
-UNKNOWN
+A sample vectorGPTBot
```

