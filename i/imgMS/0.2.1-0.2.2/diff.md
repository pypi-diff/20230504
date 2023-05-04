# Comparing `tmp/imgMS-0.2.1.tar.gz` & `tmp/imgMS-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgMS-0.2.1.tar", last modified: Sun Mar 12 17:18:41 2023, max compression
+gzip compressed data, was "imgMS-0.2.2.tar", last modified: Thu May  4 15:34:46 2023, max compression
```

## Comparing `imgMS-0.2.1.tar` & `imgMS-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-03-12 17:18:41.318188 imgMS-0.2.1/
--rw-r--r--   0 nika       (501) staff       (20)     1066 2023-01-10 13:41:26.000000 imgMS-0.2.1/LICENSE
--rw-r--r--   0 nika       (501) staff       (20)     2852 2023-03-12 17:18:41.317753 imgMS-0.2.1/PKG-INFO
--rw-r--r--   0 nika       (501) staff       (20)     2084 2023-01-10 13:41:26.000000 imgMS-0.2.1/README.md
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-03-12 17:18:41.313601 imgMS-0.2.1/imgMS/
--rw-r--r--   0 nika       (501) staff       (20)    38940 2023-01-10 13:41:26.000000 imgMS-0.2.1/imgMS/MSData.py
--rw-r--r--   0 nika       (501) staff       (20)    13090 2023-03-12 16:49:41.000000 imgMS-0.2.1/imgMS/MSEval.py
--rw-r--r--   0 nika       (501) staff       (20)     3541 2023-03-12 16:49:41.000000 imgMS-0.2.1/imgMS/MSStats.py
--rw-r--r--   0 nika       (501) staff       (20)        0 2023-01-10 13:41:26.000000 imgMS-0.2.1/imgMS/__init__.py
--rw-r--r--   0 nika       (501) staff       (20)    12079 2023-01-10 13:41:26.000000 imgMS-0.2.1/imgMS/side_functions.py
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-03-12 17:18:41.316831 imgMS-0.2.1/imgMS.egg-info/
--rw-r--r--   0 nika       (501) staff       (20)     2852 2023-03-12 17:18:41.000000 imgMS-0.2.1/imgMS.egg-info/PKG-INFO
--rw-r--r--   0 nika       (501) staff       (20)      261 2023-03-12 17:18:41.000000 imgMS-0.2.1/imgMS.egg-info/SOURCES.txt
--rw-r--r--   0 nika       (501) staff       (20)        1 2023-03-12 17:18:41.000000 imgMS-0.2.1/imgMS.egg-info/dependency_links.txt
--rw-r--r--   0 nika       (501) staff       (20)       92 2023-03-12 17:18:41.000000 imgMS-0.2.1/imgMS.egg-info/requires.txt
--rw-r--r--   0 nika       (501) staff       (20)        6 2023-03-12 17:18:41.000000 imgMS-0.2.1/imgMS.egg-info/top_level.txt
--rw-r--r--   0 nika       (501) staff       (20)       38 2023-03-12 17:18:41.318376 imgMS-0.2.1/setup.cfg
--rw-r--r--   0 nika       (501) staff       (20)      953 2023-03-12 17:17:37.000000 imgMS-0.2.1/setup.py
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 15:34:46.978643 imgMS-0.2.2/
+-rw-r--r--   0 nika       (501) staff       (20)     1066 2023-01-10 13:41:26.000000 imgMS-0.2.2/LICENSE
+-rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 15:34:46.978320 imgMS-0.2.2/PKG-INFO
+-rw-r--r--   0 nika       (501) staff       (20)     2084 2023-01-10 13:41:26.000000 imgMS-0.2.2/README.md
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 15:34:46.974694 imgMS-0.2.2/imgMS/
+-rw-r--r--   0 nika       (501) staff       (20)    38940 2023-01-10 13:41:26.000000 imgMS-0.2.2/imgMS/MSData.py
+-rw-r--r--   0 nika       (501) staff       (20)    13469 2023-05-04 15:30:59.000000 imgMS-0.2.2/imgMS/MSEval.py
+-rw-r--r--   0 nika       (501) staff       (20)     3541 2023-03-12 16:49:41.000000 imgMS-0.2.2/imgMS/MSStats.py
+-rw-r--r--   0 nika       (501) staff       (20)        0 2023-01-10 13:41:26.000000 imgMS-0.2.2/imgMS/__init__.py
+-rw-r--r--   0 nika       (501) staff       (20)    12079 2023-01-10 13:41:26.000000 imgMS-0.2.2/imgMS/side_functions.py
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 15:34:46.977752 imgMS-0.2.2/imgMS.egg-info/
+-rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 15:34:46.000000 imgMS-0.2.2/imgMS.egg-info/PKG-INFO
+-rw-r--r--   0 nika       (501) staff       (20)      261 2023-05-04 15:34:46.000000 imgMS-0.2.2/imgMS.egg-info/SOURCES.txt
+-rw-r--r--   0 nika       (501) staff       (20)        1 2023-05-04 15:34:46.000000 imgMS-0.2.2/imgMS.egg-info/dependency_links.txt
+-rw-r--r--   0 nika       (501) staff       (20)       92 2023-05-04 15:34:46.000000 imgMS-0.2.2/imgMS.egg-info/requires.txt
+-rw-r--r--   0 nika       (501) staff       (20)        6 2023-05-04 15:34:46.000000 imgMS-0.2.2/imgMS.egg-info/top_level.txt
+-rw-r--r--   0 nika       (501) staff       (20)       38 2023-05-04 15:34:46.978781 imgMS-0.2.2/setup.cfg
+-rw-r--r--   0 nika       (501) staff       (20)      953 2023-05-04 15:32:05.000000 imgMS-0.2.2/setup.py
```

### Comparing `imgMS-0.2.1/LICENSE` & `imgMS-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.1/PKG-INFO` & `imgMS-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgMS
-Version: 0.2.1
+Version: 0.2.2
 Summary: Package for data reduction of LA-ICP-MS data.
 Home-page: https://github.com/nikadilli/imgMS
 Author: nikadilli
 Author-email: nikadilli@gmail.com
 License: LICENSE.txt
 Description: [![Documentation Status](https://readthedocs.org/projects/imgms/badge/?version=latest)](https://imgms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `imgMS-0.2.1/README.md` & `imgMS-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.1/imgMS/MSData.py` & `imgMS-0.2.2/imgMS/MSData.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.1/imgMS/MSEval.py` & `imgMS-0.2.2/imgMS/MSEval.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,41 +57,50 @@
         """
         cols_to_drop = []
 
         if instrument == 'Element':
             skipfooter = 4
             header = 1
             drop = 9
+            index_col = 0
         elif instrument == 'Agilent':
             skipfooter = 4
             header = 3
             drop = 3
+            index_col = 0
         elif instrument =='MC Nu-Sapphire':
             skipfooter = 0
-            header = 73
+            header = 14
             drop = 0
-            cols_to_drop = ['Cycle', 'ID code']
+            index_col = 1
+            cols_to_drop = ['Cycle', 'Section', 'Type', 'Trigger Status']
         else:
             skipfooter = 0
             header = 0
             drop = 0
+            index_col = 0
 
         if filetype == 'xlsx':
             imported = pd.ExcelFile(filename)
             data = imported.parse(
-                0, index_col=0, skipfooter=skipfooter, header=header)
+                0, index_col=index_col, skipfooter=skipfooter, header=header)
             data = data.drop(data.index[:drop], axis=0)
 
         elif filetype == 'csv':
-            data = pd.read_csv(filename, sep=',', index_col=0, skipfooter=skipfooter,
+            data = pd.read_csv(filename, sep=',', index_col=index_col, skipfooter=skipfooter,
                                header=header, engine='python')
 
         elif filetype == 'asc':
-            data = pd.read_csv(filename, sep='\t', index_col=0, skipfooter=skipfooter,
+        	try:
+            	data = pd.read_csv(filename, sep='\t', index_col=index_col, skipfooter=skipfooter,
                                header=header, engine='python')
+            except:
+            	data = pd.read_csv(filename, sep=',', index_col=index_col, skipfooter=skipfooter,
+                               header=header, engine='python')
+                               
             data = data.drop(data.index[:drop], axis=0)
             data.dropna(axis=1, how='all', inplace=True)
             data = data.apply(pd.to_numeric, errors='coerce')
 
         else:
             warnings.warn('File type not supported.')
```

### Comparing `imgMS-0.2.1/imgMS/MSStats.py` & `imgMS-0.2.2/imgMS/MSStats.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.1/imgMS/side_functions.py` & `imgMS-0.2.2/imgMS/side_functions.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.1/imgMS.egg-info/PKG-INFO` & `imgMS-0.2.2/imgMS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgMS
-Version: 0.2.1
+Version: 0.2.2
 Summary: Package for data reduction of LA-ICP-MS data.
 Home-page: https://github.com/nikadilli/imgMS
 Author: nikadilli
 Author-email: nikadilli@gmail.com
 License: LICENSE.txt
 Description: [![Documentation Status](https://readthedocs.org/projects/imgms/badge/?version=latest)](https://imgms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `imgMS-0.2.1/setup.py` & `imgMS-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='imgMS',
-    version='0.2.1',
+    version='0.2.2',
     author='nikadilli',
     author_email='nikadilli@gmail.com',
     url="https://github.com/nikadilli/imgMS",
     packages=setuptools.find_packages(),
     scripts=[],
     license='LICENSE.txt',
     description='Package for data reduction of LA-ICP-MS data.',
```

