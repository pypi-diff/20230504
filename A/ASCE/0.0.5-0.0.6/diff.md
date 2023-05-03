# Comparing `tmp/ASCE-0.0.5.tar.gz` & `tmp/ASCE-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCE-0.0.5.tar", last modified: Wed May  3 21:52:38 2023, max compression
+gzip compressed data, was "ASCE-0.0.6.tar", last modified: Wed May  3 22:02:03 2023, max compression
```

## Comparing `ASCE-0.0.5.tar` & `ASCE-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 21:52:38.832459 ASCE-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-03 21:52:38.785568 ASCE-0.0.5/ASCE/
--rw-rw-rw-   0        0        0    11885 2023-05-03 21:46:46.000000 ASCE-0.0.5/ASCE/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:52:38.816828 ASCE-0.0.5/ASCE.egg-info/
--rw-rw-rw-   0        0        0      501 2023-05-03 21:52:38.000000 ASCE-0.0.5/ASCE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-05-03 21:52:38.000000 ASCE-0.0.5/ASCE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 21:52:38.000000 ASCE-0.0.5/ASCE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 21:52:38.000000 ASCE-0.0.5/ASCE.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 21:52:38.000000 ASCE-0.0.5/ASCE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1061 2023-05-03 21:46:45.000000 ASCE-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      501 2023-05-03 21:52:38.832459 ASCE-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-05-03 21:46:46.000000 ASCE-0.0.5/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 21:52:38.832459 ASCE-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-05-03 21:52:32.000000 ASCE-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:02:03.789281 ASCE-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-03 22:02:03.758021 ASCE-0.0.6/ASCE/
+-rw-rw-rw-   0        0        0    11885 2023-05-03 21:46:46.000000 ASCE-0.0.6/ASCE/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:02:03.789281 ASCE-0.0.6/ASCE.egg-info/
+-rw-rw-rw-   0        0        0      501 2023-05-03 22:02:03.000000 ASCE-0.0.6/ASCE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2023-05-03 22:02:03.000000 ASCE-0.0.6/ASCE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 22:02:03.000000 ASCE-0.0.6/ASCE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 22:02:03.000000 ASCE-0.0.6/ASCE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1061 2023-05-03 21:46:45.000000 ASCE-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      501 2023-05-03 22:02:03.789281 ASCE-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2023-05-03 21:46:46.000000 ASCE-0.0.6/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 22:02:03.789281 ASCE-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      638 2023-05-03 22:01:46.000000 ASCE-0.0.6/setup.py
```

### Comparing `ASCE-0.0.5/ASCE/__init__.py` & `ASCE-0.0.6/ASCE/__init__.py`

 * *Files identical despite different names*

### Comparing `ASCE-0.0.5/LICENSE` & `ASCE-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ASCE-0.0.5/README.txt` & `ASCE-0.0.6/README.txt`

 * *Files identical despite different names*

### Comparing `ASCE-0.0.5/setup.py` & `ASCE-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,19 +6,18 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ASCE',
-  version='0.0.5',
+  version='0.0.6',
 #   description='A fast library/similar to numpy',
 #   long_description=open('README.txt').read()
   url='',  
   author='CZB ASCE GROUP',
   author_email='sandrine.sila@net.usj.edu.lb',
   license='MIT', 
   classifiers=classifiers,
   keywords='library', 
-  packages=find_packages(),
-  install_requires=['math'] 
+  packages=find_packages()
 )
```

