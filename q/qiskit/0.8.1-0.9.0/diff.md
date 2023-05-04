# Comparing `tmp/qiskit-0.8.1.tar.gz` & `tmp/qiskit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit-0.8.1.tar", last modified: Wed May  1 16:24:43 2019, max compression
+gzip compressed data, was "dist/qiskit-0.9.0.tar", last modified: Fri May  3 02:35:28 2019, max compression
```

## Comparing `qiskit-0.8.1.tar` & `qiskit-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-05-01 16:24:43.000000 qiskit-0.8.1/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      989 2019-05-01 16:24:43.000000 qiskit-0.8.1/PKG-INFO
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5935 2019-02-22 16:35:47.000000 qiskit-0.8.1/README.md
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-05-01 16:24:43.000000 qiskit-0.8.1/qiskit.egg-info/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      989 2019-05-01 16:24:43.000000 qiskit-0.8.1/qiskit.egg-info/PKG-INFO
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      216 2019-05-01 16:24:43.000000 qiskit-0.8.1/qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2019-05-01 16:24:43.000000 qiskit-0.8.1/qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)       58 2019-05-01 16:24:43.000000 qiskit-0.8.1/qiskit.egg-info/requires.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2019-05-01 16:24:43.000000 qiskit-0.8.1/qiskit.egg-info/top_level.txt
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)       38 2019-05-01 16:24:43.000000 qiskit-0.8.1/setup.cfg
--rwxr-xr-x   0 computertreker  (1000) computertreker  (1000)     3702 2019-05-01 15:20:46.000000 qiskit-0.8.1/setup.py
-drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-05-01 16:24:43.000000 qiskit-0.8.1/test/
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)      765 2019-05-01 15:20:09.000000 qiskit-0.8.1/test/test_metapackage.py
--rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1257 2019-05-01 15:20:09.000000 qiskit-0.8.1/test/test_simulation.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-05-03 02:35:28.000000 qiskit-0.9.0/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      989 2019-05-03 02:35:28.000000 qiskit-0.9.0/PKG-INFO
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     5935 2019-02-22 16:35:47.000000 qiskit-0.9.0/README.md
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-05-03 02:35:28.000000 qiskit-0.9.0/qiskit.egg-info/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      989 2019-05-03 02:35:28.000000 qiskit-0.9.0/qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      216 2019-05-03 02:35:28.000000 qiskit-0.9.0/qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2019-05-03 02:35:28.000000 qiskit-0.9.0/qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      129 2019-05-03 02:35:28.000000 qiskit-0.9.0/qiskit.egg-info/requires.txt
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)        1 2019-05-03 02:35:28.000000 qiskit-0.9.0/qiskit.egg-info/top_level.txt
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)       38 2019-05-03 02:35:28.000000 qiskit-0.9.0/setup.cfg
+-rwxr-xr-x   0 computertreker  (1000) computertreker  (1000)     3794 2019-05-03 02:27:15.000000 qiskit-0.9.0/setup.py
+drwxr-xr-x   0 computertreker  (1000) computertreker  (1000)        0 2019-05-03 02:35:28.000000 qiskit-0.9.0/test/
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)      765 2019-05-01 20:21:59.000000 qiskit-0.9.0/test/test_metapackage.py
+-rw-r--r--   0 computertreker  (1000) computertreker  (1000)     1257 2019-05-01 20:21:59.000000 qiskit-0.9.0/test/test_simulation.py
```

### Comparing `qiskit-0.8.1/PKG-INFO` & `qiskit-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: qiskit
-Version: 0.8.1
+Version: 0.9.0
 Summary: Software for developing quantum computing programs
 Home-page: https://github.com/Qiskit/qiskit
 Author: Qiskit Development Team
 Author-email: qiskit@us.ibm.com
 License: Apache 2.0
 Description: Qiskit is a software development kit for writing quantum computing experiments, programs, and applications. Works with Python 3.5, 3.6, and 3.7
 Keywords: qiskit sdk quantum
```

### Comparing `qiskit-0.8.1/README.md` & `qiskit-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-0.8.1/qiskit.egg-info/PKG-INFO` & `qiskit-0.9.0/qiskit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: qiskit
-Version: 0.8.1
+Version: 0.9.0
 Summary: Software for developing quantum computing programs
 Home-page: https://github.com/Qiskit/qiskit
 Author: Qiskit Development Team
 Author-email: qiskit@us.ibm.com
 License: Apache 2.0
 Description: Qiskit is a software development kit for writing quantum computing experiments, programs, and applications. Works with Python 3.5, 3.6, and 3.7
 Keywords: qiskit sdk quantum
```

### Comparing `qiskit-0.8.1/setup.py` & `qiskit-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,23 @@
 import sys
 import subprocess
 
 from setuptools import setup
 from setuptools.command.install import install
 from setuptools.command.develop import develop
 
-qiskit_terra = "qiskit_terra==0.7.2"
+qiskit_terra = "qiskit_terra==0.8.0"
 
 requirements = [
     qiskit_terra,
-    "qiskit-aer==0.1.1",
-    "qiskit-ignis==0.1.0"
+    "qiskit-aer==0.2.0",
+    "qiskit-ibmq-provider==0.1.1",
+    "qiskit-ignis==0.1.1",
+    "qiskit-aqua==0.5.0",
+    "qiskit-chemistry==0.5.0"
 ]
 
 
 def _reinstall_terra():
     subprocess.check_call(
         [sys.executable, "-m", "pip", "install", "--no-deps", "-I", qiskit_terra])
 
@@ -70,15 +73,15 @@
 
 except:
     pass
 
 
 setup(
     name="qiskit",
-    version="0.8.1",
+    version="0.9.0",
     description="Software for developing quantum computing programs",
     long_description="Qiskit is a software development kit for writing "
                      "quantum computing experiments, programs, and "
                      "applications. Works with Python 3.5, 3.6, and 3.7",
     url="https://github.com/Qiskit/qiskit",
     author="Qiskit Development Team",
     author_email="qiskit@us.ibm.com",
```

### Comparing `qiskit-0.8.1/test/test_metapackage.py` & `qiskit-0.9.0/test/test_metapackage.py`

 * *Files identical despite different names*

### Comparing `qiskit-0.8.1/test/test_simulation.py` & `qiskit-0.9.0/test/test_simulation.py`

 * *Files identical despite different names*

