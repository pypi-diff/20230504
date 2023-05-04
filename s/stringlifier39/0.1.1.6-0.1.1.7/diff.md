# Comparing `tmp/stringlifier39-0.1.1.6.tar.gz` & `tmp/stringlifier39-0.1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringlifier39-0.1.1.6.tar", last modified: Thu Feb  9 07:58:56 2023, max compression
+gzip compressed data, was "stringlifier39-0.1.1.7.tar", last modified: Thu May  4 10:19:13 2023, max compression
```

## Comparing `stringlifier39-0.1.1.6.tar` & `stringlifier39-0.1.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-02-09 07:58:55.996788 stringlifier39-0.1.1.6/
--rw-r--r--   0 gv892691   (501) staff       (20)    11357 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/LICENSE
--rw-r--r--   0 gv892691   (501) staff       (20)      185 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/MANIFEST.in
--rw-r--r--   0 gv892691   (501) staff       (20)     4431 2023-02-09 07:58:55.979505 stringlifier39-0.1.1.6/PKG-INFO
--rw-r--r--   0 gv892691   (501) staff       (20)     3862 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/README.md
-drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-02-09 07:58:55.961532 stringlifier39-0.1.1.6/data/
--rw-r--r--   0 gv892691   (501) staff       (20)  2111205 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/data/enhanced-c.bestType
--rw-r--r--   0 gv892691   (501) staff       (20)       71 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/data/enhanced-c.conf
--rw-r--r--   0 gv892691   (501) staff       (20)      719 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/data/enhanced-c.encodings
--rw-r--r--   0 gv892691   (501) staff       (20)       38 2023-02-09 07:58:55.997040 stringlifier39-0.1.1.6/setup.cfg
--rw-r--r--   0 gv892691   (501) staff       (20)     1485 2023-02-09 07:58:47.000000 stringlifier39-0.1.1.6/setup.py
-drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-02-09 07:58:55.964134 stringlifier39-0.1.1.6/stringlifier/
--rw-r--r--   0 gv892691   (501) staff       (20)        0 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/stringlifier/__init__.py
--rw-r--r--   0 gv892691   (501) staff       (20)     7010 2023-02-09 07:09:06.000000 stringlifier39-0.1.1.6/stringlifier/api.py
-drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-02-09 07:58:55.967481 stringlifier39-0.1.1.6/stringlifier/modules/
--rw-r--r--   0 gv892691   (501) staff       (20)        0 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/stringlifier/modules/__init__.py
--rw-r--r--   0 gv892691   (501) staff       (20)    14075 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/stringlifier/modules/stringc.py
--rw-r--r--   0 gv892691   (501) staff       (20)    13331 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/stringlifier/modules/stringc2.py
--rw-r--r--   0 gv892691   (501) staff       (20)     4974 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.6/stringlifier/modules/training.py
--rw-r--r--   0 gv892691   (501) staff       (20)      349 2023-02-09 07:19:24.000000 stringlifier39-0.1.1.6/stringlifier/stringlifier_test.py
-drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-02-09 07:58:55.977626 stringlifier39-0.1.1.6/stringlifier39.egg-info/
--rw-r--r--   0 gv892691   (501) staff       (20)     4431 2023-02-09 07:58:55.000000 stringlifier39-0.1.1.6/stringlifier39.egg-info/PKG-INFO
--rw-r--r--   0 gv892691   (501) staff       (20)      546 2023-02-09 07:58:55.000000 stringlifier39-0.1.1.6/stringlifier39.egg-info/SOURCES.txt
--rw-r--r--   0 gv892691   (501) staff       (20)        1 2023-02-09 07:58:55.000000 stringlifier39-0.1.1.6/stringlifier39.egg-info/dependency_links.txt
--rw-r--r--   0 gv892691   (501) staff       (20)        1 2023-02-09 07:24:16.000000 stringlifier39-0.1.1.6/stringlifier39.egg-info/not-zip-safe
--rw-r--r--   0 gv892691   (501) staff       (20)       52 2023-02-09 07:58:55.000000 stringlifier39-0.1.1.6/stringlifier39.egg-info/requires.txt
--rw-r--r--   0 gv892691   (501) staff       (20)       13 2023-02-09 07:58:55.000000 stringlifier39-0.1.1.6/stringlifier39.egg-info/top_level.txt
+drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-05-04 10:19:13.230017 stringlifier39-0.1.1.7/
+-rw-r--r--   0 gv892691   (501) staff       (20)    11357 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/LICENSE
+-rw-r--r--   0 gv892691   (501) staff       (20)      185 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/MANIFEST.in
+-rw-r--r--   0 gv892691   (501) staff       (20)     4431 2023-05-04 10:19:13.229677 stringlifier39-0.1.1.7/PKG-INFO
+-rw-r--r--   0 gv892691   (501) staff       (20)     3862 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/README.md
+drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-05-04 10:19:13.199753 stringlifier39-0.1.1.7/data/
+-rw-r--r--   0 gv892691   (501) staff       (20)  2111205 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/data/enhanced-c.bestType
+-rw-r--r--   0 gv892691   (501) staff       (20)       71 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/data/enhanced-c.conf
+-rw-r--r--   0 gv892691   (501) staff       (20)      719 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/data/enhanced-c.encodings
+-rw-r--r--   0 gv892691   (501) staff       (20)       38 2023-05-04 10:19:13.230106 stringlifier39-0.1.1.7/setup.cfg
+-rw-r--r--   0 gv892691   (501) staff       (20)     1485 2023-05-04 10:10:37.000000 stringlifier39-0.1.1.7/setup.py
+drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-05-04 10:19:13.219605 stringlifier39-0.1.1.7/stringlifier/
+-rw-r--r--   0 gv892691   (501) staff       (20)        0 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/stringlifier/__init__.py
+-rw-r--r--   0 gv892691   (501) staff       (20)     7010 2023-02-09 07:09:06.000000 stringlifier39-0.1.1.7/stringlifier/api.py
+drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-05-04 10:19:13.223917 stringlifier39-0.1.1.7/stringlifier/modules/
+-rw-r--r--   0 gv892691   (501) staff       (20)        0 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/stringlifier/modules/__init__.py
+-rw-r--r--   0 gv892691   (501) staff       (20)    14075 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/stringlifier/modules/stringc.py
+-rw-r--r--   0 gv892691   (501) staff       (20)    13331 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/stringlifier/modules/stringc2.py
+-rw-r--r--   0 gv892691   (501) staff       (20)     4974 2023-02-09 06:35:45.000000 stringlifier39-0.1.1.7/stringlifier/modules/training.py
+-rw-r--r--   0 gv892691   (501) staff       (20)      349 2023-02-09 07:19:24.000000 stringlifier39-0.1.1.7/stringlifier/stringlifier_test.py
+drwxr-xr-x   0 gv892691   (501) staff       (20)        0 2023-05-04 10:19:13.228991 stringlifier39-0.1.1.7/stringlifier39.egg-info/
+-rw-r--r--   0 gv892691   (501) staff       (20)     4431 2023-05-04 10:19:13.000000 stringlifier39-0.1.1.7/stringlifier39.egg-info/PKG-INFO
+-rw-r--r--   0 gv892691   (501) staff       (20)      546 2023-05-04 10:19:13.000000 stringlifier39-0.1.1.7/stringlifier39.egg-info/SOURCES.txt
+-rw-r--r--   0 gv892691   (501) staff       (20)        1 2023-05-04 10:19:13.000000 stringlifier39-0.1.1.7/stringlifier39.egg-info/dependency_links.txt
+-rw-r--r--   0 gv892691   (501) staff       (20)        1 2023-02-09 07:24:16.000000 stringlifier39-0.1.1.7/stringlifier39.egg-info/not-zip-safe
+-rw-r--r--   0 gv892691   (501) staff       (20)       52 2023-05-04 10:19:13.000000 stringlifier39-0.1.1.7/stringlifier39.egg-info/requires.txt
+-rw-r--r--   0 gv892691   (501) staff       (20)       13 2023-05-04 10:19:13.000000 stringlifier39-0.1.1.7/stringlifier39.egg-info/top_level.txt
```

### Comparing `stringlifier39-0.1.1.6/LICENSE` & `stringlifier39-0.1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stringlifier39-0.1.1.6/PKG-INFO` & `stringlifier39-0.1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringlifier39
-Version: 0.1.1.6
+Version: 0.1.1.7
 Summary: Python module for detecting password, api keys hashes and any other string that resembles a randomly generated character sequence.
 Home-page: https://github.com/adobe/stringlifier
 Author: Multiple authors
 Author-email: garvit.ism@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `stringlifier39-0.1.1.6/README.md` & `stringlifier39-0.1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `stringlifier39-0.1.1.6/data/enhanced-c.bestType` & `stringlifier39-0.1.1.7/data/enhanced-c.bestType`

 * *Files identical despite different names*

### Comparing `stringlifier39-0.1.1.6/data/enhanced-c.encodings` & `stringlifier39-0.1.1.7/data/enhanced-c.encodings`

 * *Files identical despite different names*

### Comparing `stringlifier39-0.1.1.6/setup.py` & `stringlifier39-0.1.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     """ load requirements from a pip requirements file """
     lineiter = (line.strip() for line in open(filename))
     return [line for line in lineiter if line and not line.startswith("#")]
 
 dependencies = [
     "ipdb",
     "nptyping==1.3.0",
-    "numpy==1.19.1",
+    "numpy==1.22.3",
     "PyJWT",
     "torch",
     "tqdm"
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stringlifier39",
-    version="0.1.1.6",
+    version="0.1.1.7",
     author="Multiple authors",
     author_email="garvit.ism@gmail.com",
     description="Python module for detecting password, api keys hashes and any other string that resembles a randomly generated character sequence.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/adobe/stringlifier",
     packages=setuptools.find_packages(),
```

### Comparing `stringlifier39-0.1.1.6/stringlifier/api.py` & `stringlifier39-0.1.1.7/stringlifier/api.py`

 * *Files identical despite different names*

### Comparing `stringlifier39-0.1.1.6/stringlifier/modules/stringc.py` & `stringlifier39-0.1.1.7/stringlifier/modules/stringc.py`

 * *Files identical despite different names*

### Comparing `stringlifier39-0.1.1.6/stringlifier/modules/stringc2.py` & `stringlifier39-0.1.1.7/stringlifier/modules/stringc2.py`

 * *Files identical despite different names*

### Comparing `stringlifier39-0.1.1.6/stringlifier/modules/training.py` & `stringlifier39-0.1.1.7/stringlifier/modules/training.py`

 * *Files identical despite different names*

### Comparing `stringlifier39-0.1.1.6/stringlifier39.egg-info/PKG-INFO` & `stringlifier39-0.1.1.7/stringlifier39.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringlifier39
-Version: 0.1.1.6
+Version: 0.1.1.7
 Summary: Python module for detecting password, api keys hashes and any other string that resembles a randomly generated character sequence.
 Home-page: https://github.com/adobe/stringlifier
 Author: Multiple authors
 Author-email: garvit.ism@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `stringlifier39-0.1.1.6/stringlifier39.egg-info/SOURCES.txt` & `stringlifier39-0.1.1.7/stringlifier39.egg-info/SOURCES.txt`

 * *Files identical despite different names*

