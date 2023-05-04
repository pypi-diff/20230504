# Comparing `tmp/idelucs-0.1.3.tar.gz` & `tmp/idelucs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idelucs-0.1.3.tar", last modified: Thu May  4 01:10:13 2023, max compression
+gzip compressed data, was "idelucs-0.1.4.tar", last modified: Thu May  4 01:19:03 2023, max compression
```

## Comparing `idelucs-0.1.3.tar` & `idelucs-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 01:10:13.669082 idelucs-0.1.3/
--rw-rw-rw-   0        0        0     1074 2023-05-04 00:59:28.000000 idelucs-0.1.3/LICENCE.md
--rw-rw-rw-   0        0        0      608 2023-05-04 01:10:13.669082 idelucs-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-05-04 00:59:28.000000 idelucs-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 01:10:13.669082 idelucs-0.1.3/idelucs/
--rw-rw-rw-   0        0        0     3104 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/LossFunctions.py
--rw-rw-rw-   0        0        0     2584 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/PytorchUtils.py
--rw-rw-rw-   0        0        0     7524 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/ResNet.py
--rw-rw-rw-   0        0        0      355 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/__init__.py
--rw-rw-rw-   0        0        0    11548 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/__main__.py
--rw-rw-rw-   0        0        0   819037 2023-05-04 01:03:03.000000 idelucs-0.1.3/idelucs/kmers.c
--rw-rw-rw-   0        0        0     6731 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/models.py
--rw-rw-rw-   0        0        0    20627 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/utils.py
--rw-rw-rw-   0        0        0     2949 2023-05-04 00:59:31.000000 idelucs-0.1.3/idelucs/utils_GUI.py
-drwxrwxrwx   0        0        0        0 2023-05-04 01:10:13.669082 idelucs-0.1.3/idelucs.egg-info/
--rw-rw-rw-   0        0        0      608 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 01:10:13.000000 idelucs-0.1.3/idelucs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 01:10:13.669082 idelucs-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1529 2023-05-04 01:09:02.000000 idelucs-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:19:03.585676 idelucs-0.1.4/
+-rw-rw-rw-   0        0        0     1074 2023-05-04 00:59:28.000000 idelucs-0.1.4/LICENCE.md
+-rw-rw-rw-   0        0        0      608 2023-05-04 01:19:03.585676 idelucs-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-05-04 00:59:28.000000 idelucs-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 01:19:03.570052 idelucs-0.1.4/idelucs/
+-rw-rw-rw-   0        0        0     3104 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/LossFunctions.py
+-rw-rw-rw-   0        0        0     2584 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/PytorchUtils.py
+-rw-rw-rw-   0        0        0     7524 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/ResNet.py
+-rw-rw-rw-   0        0        0      355 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/__init__.py
+-rw-rw-rw-   0        0        0    11548 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/__main__.py
+-rw-rw-rw-   0        0        0   819037 2023-05-04 01:03:03.000000 idelucs-0.1.4/idelucs/kmers.c
+-rw-rw-rw-   0        0        0     6731 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/models.py
+-rw-rw-rw-   0        0        0    20627 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/utils.py
+-rw-rw-rw-   0        0        0     2949 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/utils_GUI.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:19:03.585676 idelucs-0.1.4/idelucs.egg-info/
+-rw-rw-rw-   0        0        0      608 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      105 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 01:19:03.585676 idelucs-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1639 2023-05-04 01:18:40.000000 idelucs-0.1.4/setup.py
```

### Comparing `idelucs-0.1.3/LICENCE.md` & `idelucs-0.1.4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/PKG-INFO` & `idelucs-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idelucs
-Version: 0.1.3
+Version: 0.1.4
 Summary: My first Python package
 Home-page: UNKNOWN
 Author: Pablo Millan
 Author-email: <pmillana@uwaterloo.ca>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `idelucs-0.1.3/README.md` & `idelucs-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/idelucs/LossFunctions.py` & `idelucs-0.1.4/idelucs/LossFunctions.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/idelucs/PytorchUtils.py` & `idelucs-0.1.4/idelucs/PytorchUtils.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/idelucs/ResNet.py` & `idelucs-0.1.4/idelucs/ResNet.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/idelucs/__main__.py` & `idelucs-0.1.4/idelucs/__main__.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/idelucs/kmers.c` & `idelucs-0.1.4/idelucs/kmers.c`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/idelucs/models.py` & `idelucs-0.1.4/idelucs/models.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/idelucs/utils.py` & `idelucs-0.1.4/idelucs/utils.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/idelucs/utils_GUI.py` & `idelucs-0.1.4/idelucs/utils_GUI.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.3/idelucs.egg-info/PKG-INFO` & `idelucs-0.1.4/idelucs.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idelucs
-Version: 0.1.3
+Version: 0.1.4
 Summary: My first Python package
 Home-page: UNKNOWN
 Author: Pablo Millan
 Author-email: <pmillana@uwaterloo.ca>
 License: UNKNOWN
 Keywords: python,first package
 Platform: UNKNOWN
```

### Comparing `idelucs-0.1.3/setup.py` & `idelucs-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages, Extension
 from Cython.Build import cythonize
 
-VERSION = '0.1.3' 
+VERSION = '0.1.4' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 import numpy
 
 cython_directives = {
     'embedsignature': True,
@@ -28,15 +28,15 @@
         author="Pablo Millan",
         author_email="<pmillana@uwaterloo.ca>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         zip_safe=False,            # Without these two options
         include_package_data=True, # PyInstaller may not find your C-Extensions
         packages=find_packages(),
-        install_requires=["setuptools", "Cython"], # add any additional packages that 
+        install_requires=["setuptools", "Cython", "numpy","torch","cython","matplotlib", "pandas","torchvision","scikit-learn","scipy", "umap-learn","hdbscan"], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 3",
```

