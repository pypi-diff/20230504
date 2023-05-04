# Comparing `tmp/classreg-0.0.1.tar.gz` & `tmp/classreg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\classreg-0.0.1.tar", last modified: Sat Apr 29 13:51:40 2023, max compression
+gzip compressed data, was "dist\classreg-0.0.2.tar", last modified: Thu May  4 10:07:32 2023, max compression
```

## Comparing `classreg-0.0.1.tar` & `classreg-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 13:51:40.069305 classreg-0.0.1/
--rw-rw-rw-   0        0        0      534 2023-04-29 13:51:40.069305 classreg-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-04-29 08:44:47.000000 classreg-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 13:51:39.959782 classreg-0.0.1/classreg/
--rw-rw-rw-   0        0        0       56 2023-04-29 13:43:59.000000 classreg-0.0.1/classreg/__init__.py
--rw-rw-rw-   0        0        0    13443 2023-04-29 13:42:06.000000 classreg-0.0.1/classreg/mod.py
-drwxrwxrwx   0        0        0        0 2023-04-29 13:51:40.061954 classreg-0.0.1/classreg.egg-info/
--rw-rw-rw-   0        0        0      534 2023-04-29 13:51:38.000000 classreg-0.0.1/classreg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-04-29 13:51:39.000000 classreg-0.0.1/classreg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 13:51:38.000000 classreg-0.0.1/classreg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-29 13:51:38.000000 classreg-0.0.1/classreg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 13:51:38.000000 classreg-0.0.1/classreg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 13:51:40.069305 classreg-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      705 2023-04-29 13:50:30.000000 classreg-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:07:32.244867 classreg-0.0.2/
+-rw-rw-rw-   0        0        0      534 2023-05-04 10:07:32.244867 classreg-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-04-29 08:44:47.000000 classreg-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 10:07:32.209583 classreg-0.0.2/classreg/
+-rw-rw-rw-   0        0        0      105 2023-05-04 10:05:12.000000 classreg-0.0.2/classreg/__init__.py
+-rw-rw-rw-   0        0        0    29300 2023-05-04 10:02:09.000000 classreg-0.0.2/classreg/mod.py
+drwxrwxrwx   0        0        0        0 2023-05-04 10:07:32.242869 classreg-0.0.2/classreg.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-05-04 10:07:31.000000 classreg-0.0.2/classreg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-04 10:07:31.000000 classreg-0.0.2/classreg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 10:07:31.000000 classreg-0.0.2/classreg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-04 10:07:31.000000 classreg-0.0.2/classreg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 10:07:31.000000 classreg-0.0.2/classreg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 10:07:32.246161 classreg-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      705 2023-05-04 09:30:24.000000 classreg-0.0.2/setup.py
```

### Comparing `classreg-0.0.1/PKG-INFO` & `classreg-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: classreg
-Version: 0.0.1
+Version: 0.0.2
 Summary: data analysis
 Home-page: UNKNOWN
 Author: Yizhan
 Author-email: boy87511@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: data analysis
```

### Comparing `classreg-0.0.1/classreg.egg-info/PKG-INFO` & `classreg-0.0.2/classreg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: classreg
-Version: 0.0.1
+Version: 0.0.2
 Summary: data analysis
 Home-page: UNKNOWN
 Author: Yizhan
 Author-email: boy87511@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: data analysis
```

### Comparing `classreg-0.0.1/setup.py` & `classreg-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='classreg',
-    version='0.0.1',
+    version='0.0.2',
     description='data analysis',
     author='Yizhan',
     author_email='boy87511@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
```

