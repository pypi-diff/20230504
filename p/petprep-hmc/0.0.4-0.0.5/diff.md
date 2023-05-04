# Comparing `tmp/petprep_hmc-0.0.4.tar.gz` & `tmp/petprep_hmc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petprep_hmc-0.0.4.tar", last modified: Wed May  3 20:46:33 2023, max compression
+gzip compressed data, was "petprep_hmc-0.0.5.tar", last modified: Thu May  4 08:25:16 2023, max compression
```

## Comparing `petprep_hmc-0.0.4.tar` & `petprep_hmc-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-03 20:46:33.631157 petprep_hmc-0.0.4/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.4/LICENSE
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-03 20:46:33.630957 petprep_hmc-0.0.4/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     4576 2023-05-03 20:44:42.000000 petprep_hmc-0.0.4/README.md
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-03 20:46:33.629747 petprep_hmc-0.0.4/petprep_hmc/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.4/petprep_hmc/__init__.py
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-03 20:46:33.630449 petprep_hmc-0.0.4/petprep_hmc.egg-info/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      242 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/SOURCES.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/dependency_links.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      403 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/requires.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2023-05-03 20:46:33.000000 petprep_hmc-0.0.4/petprep_hmc.egg-info/top_level.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2023-05-03 20:46:33.631324 petprep_hmc-0.0.4/setup.cfg
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     1554 2023-05-03 20:44:10.000000 petprep_hmc-0.0.4/setup.py
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-03 20:46:33.630581 petprep_hmc-0.0.4/tests/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      510 2023-05-03 19:40:26.000000 petprep_hmc-0.0.4/tests/test_cli.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-04 08:25:16.776436 petprep_hmc-0.0.5/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.5/LICENSE
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-04 08:25:16.776273 petprep_hmc-0.0.5/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     4576 2023-05-03 20:44:42.000000 petprep_hmc-0.0.5/README.md
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-04 08:25:16.774854 petprep_hmc-0.0.5/petprep_hmc/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.5/petprep_hmc/__init__.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-04 08:25:16.775598 petprep_hmc-0.0.5/petprep_hmc.egg-info/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      242 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/SOURCES.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/dependency_links.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      422 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/requires.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/top_level.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2023-05-04 08:25:16.776514 petprep_hmc-0.0.5/setup.cfg
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     1584 2023-05-04 08:23:15.000000 petprep_hmc-0.0.5/setup.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-04 08:25:16.775876 petprep_hmc-0.0.5/tests/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      510 2023-05-03 19:40:26.000000 petprep_hmc-0.0.5/tests/test_cli.py
```

### Comparing `petprep_hmc-0.0.4/LICENSE` & `petprep_hmc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `petprep_hmc-0.0.4/PKG-INFO` & `petprep_hmc-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petprep_hmc
-Version: 0.0.4
+Version: 0.0.5
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.4/README.md` & `petprep_hmc-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `petprep_hmc-0.0.4/petprep_hmc.egg-info/PKG-INFO` & `petprep_hmc-0.0.5/petprep_hmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petprep-hmc
-Version: 0.0.4
+Version: 0.0.5
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.4/setup.py` & `petprep_hmc-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="petprep_hmc",
-    version="0.0.4",
+    version="0.0.5",
     description='PETPrep Head Motion Correction Workflow',
     author='Martin Norgaard',
     author_email='martin.noergaard@di.ku.dk',
     url='https://github.com/mnoergaard/petprep_hmc',
     packages=find_packages(),
     install_requires=[
         "click==8.1.3",
@@ -30,14 +30,15 @@
         "docopt==0.6.2",
         "formulaic==0.5.2",
         "interface-meta==1.3.0",
         "num2words==0.5.12",
         "pybids==0.15.6",
         "sqlalchemy==1.3.24",
         "wrapt==1.15.0",
+        "niworkflows==1.7.9",
     ],
     extras_require={
         "dev": [
             "pytest",
             # Add any other development/testing packages here
         ],
     },
```

