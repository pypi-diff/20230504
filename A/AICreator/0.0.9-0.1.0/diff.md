# Comparing `tmp/AICreator-0.0.9.tar.gz` & `tmp/AICreator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AICreator-0.0.9.tar", last modified: Thu May  4 15:26:25 2023, max compression
+gzip compressed data, was "AICreator-0.1.0.tar", last modified: Thu May  4 15:33:51 2023, max compression
```

## Comparing `AICreator-0.0.9.tar` & `AICreator-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 15:26:25.670800 AICreator-0.0.9/
-drwxrwxrwx   0        0        0        0 2023-05-04 15:26:25.663709 AICreator-0.0.9/AICreator.egg-info/
--rw-rw-rw-   0        0        0      559 2023-05-04 15:26:25.000000 AICreator-0.0.9/AICreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-05-04 15:26:25.000000 AICreator-0.0.9/AICreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 15:26:25.000000 AICreator-0.0.9/AICreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 15:26:25.000000 AICreator-0.0.9/AICreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-04 15:26:25.000000 AICreator-0.0.9/AICreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 15:26:25.664800 AICreator-0.0.9/AICreatorPackage/
--rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.0.9/AICreatorPackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 15:26:25.667798 AICreator-0.0.9/AICreatorPackage/functions/
--rw-rw-rw-   0        0        0      782 2023-05-04 15:26:03.000000 AICreator-0.0.9/AICreatorPackage/functions/AICreatorPackage.py
--rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.0.9/AICreatorPackage/functions/__init__.py
--rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.0.9/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2023-05-04 15:26:25.669802 AICreator-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.0.9/README.txt
--rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.0.9/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-04 15:26:25.670800 AICreator-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      675 2023-05-04 15:26:22.000000 AICreator-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:33:51.908297 AICreator-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-05-04 15:33:51.900649 AICreator-0.1.0/AICreator.egg-info/
+-rw-rw-rw-   0        0        0      559 2023-05-04 15:33:51.000000 AICreator-0.1.0/AICreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-05-04 15:33:51.000000 AICreator-0.1.0/AICreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 15:33:51.000000 AICreator-0.1.0/AICreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 15:33:51.000000 AICreator-0.1.0/AICreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-04 15:33:51.000000 AICreator-0.1.0/AICreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 15:33:51.902648 AICreator-0.1.0/AICreatorPackage/
+-rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.1.0/AICreatorPackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 15:33:51.905652 AICreator-0.1.0/AICreatorPackage/functions/
+-rw-rw-rw-   0        0        0      783 2023-05-04 15:33:04.000000 AICreator-0.1.0/AICreatorPackage/functions/AICreatorPackage.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.1.0/AICreatorPackage/functions/__init__.py
+-rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.1.0/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      559 2023-05-04 15:33:51.906651 AICreator-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.1.0/README.txt
+-rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.1.0/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 15:33:51.908297 AICreator-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-05-04 15:33:48.000000 AICreator-0.1.0/setup.py
```

### Comparing `AICreator-0.0.9/AICreator.egg-info/PKG-INFO` & `AICreator-0.1.0/AICreator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.0.9
+Version: 0.1.0
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.0.9/LICENCE.txt` & `AICreator-0.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `AICreator-0.0.9/PKG-INFO` & `AICreator-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.0.9
+Version: 0.1.0
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.0.9/setup.py` & `AICreator-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='AICreator',
-    version='0.0.9',
+    version='0.1.0',
     description='AI Creator Package By - oren',
     long_description=open('README.txt').read(),
     url='',
     author='oren',
     author_email='orennadle@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

