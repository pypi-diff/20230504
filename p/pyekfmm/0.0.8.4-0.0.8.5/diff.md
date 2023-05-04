# Comparing `tmp/pyekfmm-0.0.8.4.tar.gz` & `tmp/pyekfmm-0.0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyekfmm-0.0.8.4.tar", last modified: Fri Feb 10 05:06:30 2023, max compression
+gzip compressed data, was "pyekfmm-0.0.8.5.tar", last modified: Thu May  4 16:18:22 2023, max compression
```

## Comparing `pyekfmm-0.0.8.4.tar` & `pyekfmm-0.0.8.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-02-10 05:06:30.922514 pyekfmm-0.0.8.4/
--rw-r--r--   0 chenyk     (501) staff       (20)    35149 2022-10-30 03:01:18.000000 pyekfmm-0.0.8.4/LICENSE
--rw-r--r--   0 chenyk     (501) staff       (20)     1153 2023-02-10 05:06:30.922117 pyekfmm-0.0.8.4/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)     2815 2023-02-01 21:02:32.000000 pyekfmm-0.0.8.4/README.md
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-02-10 05:06:30.915430 pyekfmm-0.0.8.4/pyekfmm/
--rw-r--r--   0 chenyk     (501) staff       (20)      579 2023-02-05 05:16:34.000000 pyekfmm-0.0.8.4/pyekfmm/__init__.py
--rw-r--r--   0 chenyk     (501) staff       (20)     3844 2022-10-30 03:01:18.000000 pyekfmm-0.0.8.4/pyekfmm/fmm.py
--rw-r--r--   0 chenyk     (501) staff       (20)     4068 2023-01-24 22:33:08.000000 pyekfmm-0.0.8.4/pyekfmm/fmmvti.py
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-02-10 05:06:30.921248 pyekfmm-0.0.8.4/pyekfmm/src/
--rw-r--r--   0 chenyk     (501) staff       (20)    42728 2023-01-29 23:15:17.000000 pyekfmm-0.0.8.4/pyekfmm/src/eikonal.c
--rw-r--r--   0 chenyk     (501) staff       (20)    52809 2023-02-06 21:50:44.000000 pyekfmm-0.0.8.4/pyekfmm/src/eikonalvti.c
--rw-r--r--   0 chenyk     (501) staff       (20)     8583 2023-02-05 06:09:13.000000 pyekfmm-0.0.8.4/pyekfmm/stream.py
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-02-10 05:06:30.919834 pyekfmm-0.0.8.4/pyekfmm.egg-info/
--rw-r--r--   0 chenyk     (501) staff       (20)     1153 2023-02-10 05:06:30.000000 pyekfmm-0.0.8.4/pyekfmm.egg-info/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)      328 2023-02-10 05:06:30.000000 pyekfmm-0.0.8.4/pyekfmm.egg-info/SOURCES.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-02-10 05:06:30.000000 pyekfmm-0.0.8.4/pyekfmm.egg-info/dependency_links.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-01-23 03:43:08.000000 pyekfmm-0.0.8.4/pyekfmm.egg-info/not-zip-safe
--rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-02-10 05:06:30.000000 pyekfmm-0.0.8.4/pyekfmm.egg-info/requires.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       29 2023-02-10 05:06:30.000000 pyekfmm-0.0.8.4/pyekfmm.egg-info/top_level.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-02-10 05:06:30.922652 pyekfmm-0.0.8.4/setup.cfg
--rw-r--r--   0 chenyk     (501) staff       (20)     1932 2023-02-10 05:05:45.000000 pyekfmm-0.0.8.4/setup.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-05-04 16:18:22.762181 pyekfmm-0.0.8.5/
+-rw-r--r--   0 chenyk     (501) staff       (20)    35149 2023-02-14 21:21:31.000000 pyekfmm-0.0.8.5/LICENSE
+-rw-r--r--   0 chenyk     (501) staff       (20)     1145 2023-05-04 16:18:22.761873 pyekfmm-0.0.8.5/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)     3009 2023-02-14 22:02:31.000000 pyekfmm-0.0.8.5/README.md
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-05-04 16:18:22.754963 pyekfmm-0.0.8.5/pyekfmm/
+-rw-r--r--   0 chenyk     (501) staff       (20)      579 2023-02-14 21:21:58.000000 pyekfmm-0.0.8.5/pyekfmm/__init__.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     3844 2023-02-14 21:21:58.000000 pyekfmm-0.0.8.5/pyekfmm/fmm.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4068 2023-02-14 21:21:58.000000 pyekfmm-0.0.8.5/pyekfmm/fmmvti.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-05-04 16:18:22.760613 pyekfmm-0.0.8.5/pyekfmm/src/
+-rw-r--r--   0 chenyk     (501) staff       (20)    42728 2023-02-14 21:21:58.000000 pyekfmm-0.0.8.5/pyekfmm/src/eikonal.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    52809 2023-02-14 21:21:58.000000 pyekfmm-0.0.8.5/pyekfmm/src/eikonalvti.c
+-rw-r--r--   0 chenyk     (501) staff       (20)     8583 2023-02-14 21:21:58.000000 pyekfmm-0.0.8.5/pyekfmm/stream.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-05-04 16:18:22.758674 pyekfmm-0.0.8.5/pyekfmm.egg-info/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1145 2023-05-04 16:18:22.000000 pyekfmm-0.0.8.5/pyekfmm.egg-info/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)      328 2023-05-04 16:18:22.000000 pyekfmm-0.0.8.5/pyekfmm.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-05-04 16:18:22.000000 pyekfmm-0.0.8.5/pyekfmm.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-02-14 21:24:49.000000 pyekfmm-0.0.8.5/pyekfmm.egg-info/not-zip-safe
+-rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-05-04 16:18:22.000000 pyekfmm-0.0.8.5/pyekfmm.egg-info/requires.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       29 2023-05-04 16:18:22.000000 pyekfmm-0.0.8.5/pyekfmm.egg-info/top_level.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-05-04 16:18:22.762313 pyekfmm-0.0.8.5/setup.cfg
+-rw-r--r--   0 chenyk     (501) staff       (20)     1924 2023-02-14 21:24:28.000000 pyekfmm-0.0.8.5/setup.py
```

### Comparing `pyekfmm-0.0.8.4/LICENSE` & `pyekfmm-0.0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.4/PKG-INFO` & `pyekfmm-0.0.8.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyekfmm
-Version: 0.0.8.4
+Version: 0.0.8.5
 Summary: Fast Marching Method for Traveltime Calculation
-Home-page: https://github.com/chenyk1990/pyekfmm
+Home-page: https://github.com/aaspip/pyekfmm
 Author: pyekfmm developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,exploration seismology,array seismology,traveltime,ray tracing,earthquake location,earthquake relocation,surface wave tomography,body wave tomography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -18,8 +18,8 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides-Extra: docs
 License-File: LICENSE
 
-Source code: https://github.com/chenyk1990/pyekfmm
+Source code: https://github.com/aaspip/pyekfmm
```

### Comparing `pyekfmm-0.0.8.4/README.md` & `pyekfmm-0.0.8.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 **Pyekfmm**
 ======
 
 ## Description
 
-**Pyekfmm** is an eikonal solver using the fast marching method.
+**Pyekfmm** is python package for 3D fast-marching-based traveltime calculation and its applications in seismology. The initial version of this package was held at https://github.com/chenyk1990/pyekfmm, which is no longer maintained.
 
 
 ## Reference
-    Chen et al. (2023). Pyekfmm: a python package for 3D traveltime calculation based on the fast marching method. in preparation
+    Chen et al. (2023). A python package for 3D fast-marching-based traveltime calculation and its applications in seismology, in preparation
     
 BibTeX:
 
 	@article{pyekfmm,
-	  title={Pyekfmm: a python package for 3D traveltime calculation based on the fast marching method},
+	  title={Pyekfmm: A python package for 3D fast-marching-based traveltime calculation and its applications in seismology},
 	  author={Chen et al.},
 	  journal={TBD},
 	  volume={TBD},
 	  number={TBD},
 	  issue={TBD},
 	  pages={in preparation},
 	  year={2023}
@@ -32,15 +32,15 @@
     (http://www.gnu.org/copyleft/gpl.html)   
 
 -----------
 
 ## Install
 Using the latest version
 
-    git clone https://github.com/chenyk1990/pyekfmm
+    git clone https://github.com/aaspip/pyekfmm
     cd pyekfmm
     pip install -v -e .
 or using Pypi
 
     pip install pyekfmm
 
 -----------
@@ -63,15 +63,15 @@
     Regarding any questions, bugs, developments, collaborations, please contact  
     Yangkang Chen
     chenyk2016@gmail.com
 
 -----------
 ## Gallery
 The gallery figures of the pyekfmm package can be found at
-    https://github.com/chenyk1990/gallery/tree/main/pyekfmm
+    https://github.com/aaspip/gallery/tree/main/pyekfmm
 Each figure in the gallery directory corresponds to a DEMO script in the "demo" directory with the exactly the same file name.
 
 These gallery figures are also presented below. 
 
 DEMO1 (test_1_constv.m)
 
 <img src='https://github.com/chenyk1990/gallery/blob/main/pyekfmm/test_1_constv.png' alt='DEMO1' width=960/>
```

### Comparing `pyekfmm-0.0.8.4/pyekfmm/__init__.py` & `pyekfmm-0.0.8.5/pyekfmm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.4/pyekfmm/fmm.py` & `pyekfmm-0.0.8.5/pyekfmm/fmm.py`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.4/pyekfmm/fmmvti.py` & `pyekfmm-0.0.8.5/pyekfmm/fmmvti.py`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.4/pyekfmm/src/eikonal.c` & `pyekfmm-0.0.8.5/pyekfmm/src/eikonal.c`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.4/pyekfmm/src/eikonalvti.c` & `pyekfmm-0.0.8.5/pyekfmm/src/eikonalvti.c`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.4/pyekfmm/stream.py` & `pyekfmm-0.0.8.5/pyekfmm/stream.py`

 * *Files identical despite different names*

### Comparing `pyekfmm-0.0.8.4/pyekfmm.egg-info/PKG-INFO` & `pyekfmm-0.0.8.5/pyekfmm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyekfmm
-Version: 0.0.8.4
+Version: 0.0.8.5
 Summary: Fast Marching Method for Traveltime Calculation
-Home-page: https://github.com/chenyk1990/pyekfmm
+Home-page: https://github.com/aaspip/pyekfmm
 Author: pyekfmm developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
 Keywords: seismology,exploration seismology,array seismology,traveltime,ray tracing,earthquake location,earthquake relocation,surface wave tomography,body wave tomography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -18,8 +18,8 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides-Extra: docs
 License-File: LICENSE
 
-Source code: https://github.com/chenyk1990/pyekfmm
+Source code: https://github.com/aaspip/pyekfmm
```

### Comparing `pyekfmm-0.0.8.4/setup.py` & `pyekfmm-0.0.8.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 # -*- encoding: utf8 -*-
 
 from setuptools import setup
 from distutils.core import Extension
 import numpy
 
 long_description = """
-Source code: https://github.com/chenyk1990/pyekfmm""".strip() 
+Source code: https://github.com/aaspip/pyekfmm""".strip() 
 
 eikonalc_module = Extension('eikonalc', sources=['pyekfmm/src/eikonal.c'], 
 										include_dirs=[numpy.get_include()])
 
 eikonalvtic_module = Extension('eikonalvtic', sources=['pyekfmm/src/eikonalvti.c'], 
 										include_dirs=[numpy.get_include()])
 
 setup(
     name="pyekfmm",
-    version="0.0.8.4",
+    version="0.0.8.5",
     license='GNU General Public License, Version 3 (GPLv3)',
     description="Fast Marching Method for Traveltime Calculation",
     long_description=long_description,
     author="pyekfmm developing team",
     author_email="chenyk2016@gmail.com",
-    url="https://github.com/chenyk1990/pyekfmm",
+    url="https://github.com/aaspip/pyekfmm",
     ext_modules=[eikonalc_module,eikonalvtic_module],
     packages=['pyekfmm'],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

