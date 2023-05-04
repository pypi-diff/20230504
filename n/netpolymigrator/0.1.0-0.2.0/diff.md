# Comparing `tmp/netpolymigrator-0.1.0.tar.gz` & `tmp/netpolymigrator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpolymigrator-0.1.0.tar", last modified: Thu May  4 02:19:32 2023, max compression
+gzip compressed data, was "netpolymigrator-0.2.0.tar", last modified: Thu May  4 15:26:02 2023, max compression
```

## Comparing `netpolymigrator-0.1.0.tar` & `netpolymigrator-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 sanjeevganjihal   (501) staff       (20)        0 2023-05-04 02:19:32.669154 netpolymigrator-0.1.0/
--rw-r--r--   0 sanjeevganjihal   (501) staff       (20)      734 2023-05-04 02:19:32.668743 netpolymigrator-0.1.0/PKG-INFO
-drwxr-xr-x   0 sanjeevganjihal   (501) staff       (20)        0 2023-05-04 02:19:32.668071 netpolymigrator-0.1.0/netpolymigrator.egg-info/
--rw-r--r--   0 sanjeevganjihal   (501) staff       (20)      734 2023-05-04 02:19:32.000000 netpolymigrator-0.1.0/netpolymigrator.egg-info/PKG-INFO
--rw-r--r--   0 sanjeevganjihal   (501) staff       (20)      244 2023-05-04 02:19:32.000000 netpolymigrator-0.1.0/netpolymigrator.egg-info/SOURCES.txt
--rw-r--r--   0 sanjeevganjihal   (501) staff       (20)        1 2023-05-04 02:19:32.000000 netpolymigrator-0.1.0/netpolymigrator.egg-info/dependency_links.txt
--rw-r--r--   0 sanjeevganjihal   (501) staff       (20)       60 2023-05-04 02:19:32.000000 netpolymigrator-0.1.0/netpolymigrator.egg-info/entry_points.txt
--rw-r--r--   0 sanjeevganjihal   (501) staff       (20)       30 2023-05-04 02:19:32.000000 netpolymigrator-0.1.0/netpolymigrator.egg-info/requires.txt
--rw-r--r--   0 sanjeevganjihal   (501) staff       (20)        1 2023-05-04 02:19:32.000000 netpolymigrator-0.1.0/netpolymigrator.egg-info/top_level.txt
--rw-r--r--   0 sanjeevganjihal   (501) staff       (20)       38 2023-05-04 02:19:32.669283 netpolymigrator-0.1.0/setup.cfg
--rw-r--r--   0 sanjeevganjihal   (501) staff       (20)     1063 2023-05-04 02:17:14.000000 netpolymigrator-0.1.0/setup.py
+drwxr-xr-x   0 sanjeevganjihal   (501) staff       (20)        0 2023-05-04 15:26:02.292169 netpolymigrator-0.2.0/
+-rw-r--r--   0 sanjeevganjihal   (501) staff       (20)      734 2023-05-04 15:26:02.291323 netpolymigrator-0.2.0/PKG-INFO
+drwxr-xr-x   0 sanjeevganjihal   (501) staff       (20)        0 2023-05-04 15:26:02.289965 netpolymigrator-0.2.0/netpolymigrator.egg-info/
+-rw-r--r--   0 sanjeevganjihal   (501) staff       (20)      734 2023-05-04 15:26:02.000000 netpolymigrator-0.2.0/netpolymigrator.egg-info/PKG-INFO
+-rw-r--r--   0 sanjeevganjihal   (501) staff       (20)      244 2023-05-04 15:26:02.000000 netpolymigrator-0.2.0/netpolymigrator.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjeevganjihal   (501) staff       (20)        1 2023-05-04 15:26:02.000000 netpolymigrator-0.2.0/netpolymigrator.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjeevganjihal   (501) staff       (20)       60 2023-05-04 15:26:02.000000 netpolymigrator-0.2.0/netpolymigrator.egg-info/entry_points.txt
+-rw-r--r--   0 sanjeevganjihal   (501) staff       (20)       30 2023-05-04 15:26:02.000000 netpolymigrator-0.2.0/netpolymigrator.egg-info/requires.txt
+-rw-r--r--   0 sanjeevganjihal   (501) staff       (20)        1 2023-05-04 15:26:02.000000 netpolymigrator-0.2.0/netpolymigrator.egg-info/top_level.txt
+-rw-r--r--   0 sanjeevganjihal   (501) staff       (20)       38 2023-05-04 15:26:02.292467 netpolymigrator-0.2.0/setup.cfg
+-rw-r--r--   0 sanjeevganjihal   (501) staff       (20)     1063 2023-05-04 15:24:49.000000 netpolymigrator-0.2.0/setup.py
```

### Comparing `netpolymigrator-0.1.0/PKG-INFO` & `netpolymigrator-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpolymigrator
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool to migrate Calico and Cilium network policies to Kubernetes native network policies
 Home-page: https://github.com/sanjeevrg89/NetPolyMigrator
 Author: Sanjeev Ganjihal
 Author-email: sanjeevrg7@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netpolymigrator-0.1.0/netpolymigrator.egg-info/PKG-INFO` & `netpolymigrator-0.2.0/netpolymigrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpolymigrator
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool to migrate Calico and Cilium network policies to Kubernetes native network policies
 Home-page: https://github.com/sanjeevrg89/NetPolyMigrator
 Author: Sanjeev Ganjihal
 Author-email: sanjeevrg7@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netpolymigrator-0.1.0/setup.py` & `netpolymigrator-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="netpolymigrator",
-    version="0.1.0",
+    version="0.2.0",
     author="Sanjeev Ganjihal",
     author_email="sanjeevrg7@gmail.com",
     description="A tool to migrate Calico and Cilium network policies to Kubernetes native network policies",
     url="https://github.com/sanjeevrg89/NetPolyMigrator",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

