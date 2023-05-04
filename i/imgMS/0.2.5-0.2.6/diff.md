# Comparing `tmp/imgMS-0.2.5.tar.gz` & `tmp/imgMS-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgMS-0.2.5.tar", last modified: Thu May  4 19:51:14 2023, max compression
+gzip compressed data, was "imgMS-0.2.6.tar", last modified: Thu May  4 19:55:00 2023, max compression
```

## Comparing `imgMS-0.2.5.tar` & `imgMS-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 19:51:14.301590 imgMS-0.2.5/
--rw-r--r--   0 nika       (501) staff       (20)     1066 2023-01-10 13:41:26.000000 imgMS-0.2.5/LICENSE
--rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 19:51:14.301266 imgMS-0.2.5/PKG-INFO
--rw-r--r--   0 nika       (501) staff       (20)     2084 2023-01-10 13:41:26.000000 imgMS-0.2.5/README.md
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 19:51:14.296650 imgMS-0.2.5/imgMS/
--rw-r--r--   0 nika       (501) staff       (20)    38940 2023-01-10 13:41:26.000000 imgMS-0.2.5/imgMS/MSData.py
--rw-r--r--   0 nika       (501) staff       (20)    13413 2023-05-04 19:48:24.000000 imgMS-0.2.5/imgMS/MSEval.py
--rw-r--r--   0 nika       (501) staff       (20)     3594 2023-05-04 15:53:03.000000 imgMS-0.2.5/imgMS/MSStats.py
--rw-r--r--   0 nika       (501) staff       (20)        0 2023-01-10 13:41:26.000000 imgMS-0.2.5/imgMS/__init__.py
--rw-r--r--   0 nika       (501) staff       (20)    12079 2023-01-10 13:41:26.000000 imgMS-0.2.5/imgMS/side_functions.py
-drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 19:51:14.300558 imgMS-0.2.5/imgMS.egg-info/
--rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 19:51:14.000000 imgMS-0.2.5/imgMS.egg-info/PKG-INFO
--rw-r--r--   0 nika       (501) staff       (20)      261 2023-05-04 19:51:14.000000 imgMS-0.2.5/imgMS.egg-info/SOURCES.txt
--rw-r--r--   0 nika       (501) staff       (20)        1 2023-05-04 19:51:14.000000 imgMS-0.2.5/imgMS.egg-info/dependency_links.txt
--rw-r--r--   0 nika       (501) staff       (20)       92 2023-05-04 19:51:14.000000 imgMS-0.2.5/imgMS.egg-info/requires.txt
--rw-r--r--   0 nika       (501) staff       (20)        6 2023-05-04 19:51:14.000000 imgMS-0.2.5/imgMS.egg-info/top_level.txt
--rw-r--r--   0 nika       (501) staff       (20)       38 2023-05-04 19:51:14.301735 imgMS-0.2.5/setup.cfg
--rw-r--r--   0 nika       (501) staff       (20)      953 2023-05-04 19:48:42.000000 imgMS-0.2.5/setup.py
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 19:55:00.591789 imgMS-0.2.6/
+-rw-r--r--   0 nika       (501) staff       (20)     1066 2023-01-10 13:41:26.000000 imgMS-0.2.6/LICENSE
+-rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 19:55:00.591363 imgMS-0.2.6/PKG-INFO
+-rw-r--r--   0 nika       (501) staff       (20)     2084 2023-01-10 13:41:26.000000 imgMS-0.2.6/README.md
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 19:55:00.586609 imgMS-0.2.6/imgMS/
+-rw-r--r--   0 nika       (501) staff       (20)    38940 2023-01-10 13:41:26.000000 imgMS-0.2.6/imgMS/MSData.py
+-rw-r--r--   0 nika       (501) staff       (20)    13416 2023-05-04 19:53:52.000000 imgMS-0.2.6/imgMS/MSEval.py
+-rw-r--r--   0 nika       (501) staff       (20)     3594 2023-05-04 15:53:03.000000 imgMS-0.2.6/imgMS/MSStats.py
+-rw-r--r--   0 nika       (501) staff       (20)        0 2023-01-10 13:41:26.000000 imgMS-0.2.6/imgMS/__init__.py
+-rw-r--r--   0 nika       (501) staff       (20)    12079 2023-01-10 13:41:26.000000 imgMS-0.2.6/imgMS/side_functions.py
+drwxr-xr-x   0 nika       (501) staff       (20)        0 2023-05-04 19:55:00.590135 imgMS-0.2.6/imgMS.egg-info/
+-rw-r--r--   0 nika       (501) staff       (20)     2852 2023-05-04 19:55:00.000000 imgMS-0.2.6/imgMS.egg-info/PKG-INFO
+-rw-r--r--   0 nika       (501) staff       (20)      261 2023-05-04 19:55:00.000000 imgMS-0.2.6/imgMS.egg-info/SOURCES.txt
+-rw-r--r--   0 nika       (501) staff       (20)        1 2023-05-04 19:55:00.000000 imgMS-0.2.6/imgMS.egg-info/dependency_links.txt
+-rw-r--r--   0 nika       (501) staff       (20)       92 2023-05-04 19:55:00.000000 imgMS-0.2.6/imgMS.egg-info/requires.txt
+-rw-r--r--   0 nika       (501) staff       (20)        6 2023-05-04 19:55:00.000000 imgMS-0.2.6/imgMS.egg-info/top_level.txt
+-rw-r--r--   0 nika       (501) staff       (20)       38 2023-05-04 19:55:00.591939 imgMS-0.2.6/setup.cfg
+-rw-r--r--   0 nika       (501) staff       (20)      953 2023-05-04 19:54:06.000000 imgMS-0.2.6/setup.py
```

### Comparing `imgMS-0.2.5/LICENSE` & `imgMS-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.5/PKG-INFO` & `imgMS-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgMS
-Version: 0.2.5
+Version: 0.2.6
 Summary: Package for data reduction of LA-ICP-MS data.
 Home-page: https://github.com/nikadilli/imgMS
 Author: nikadilli
 Author-email: nikadilli@gmail.com
 License: LICENSE.txt
 Description: [![Documentation Status](https://readthedocs.org/projects/imgms/badge/?version=latest)](https://imgms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `imgMS-0.2.5/README.md` & `imgMS-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.5/imgMS/MSData.py` & `imgMS-0.2.6/imgMS/MSData.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.5/imgMS/MSEval.py` & `imgMS-0.2.6/imgMS/MSEval.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             data = data.drop(data.index[:drop], axis=0)
 
         elif filetype == 'csv':
             data = pd.read_csv(filename, sep=',', index_col=index_col, skipfooter=skipfooter,
                                header=header, engine='python')
 
         elif filetype == 'asc':
-        	try:
+            try:
                 data = pd.read_csv(filename, sep='\t', index_col=index_col, skipfooter=skipfooter, header=header, engine='python')
             except:
                 data = pd.read_csv(filename, sep=',', index_col=index_col, skipfooter=skipfooter, header=header, engine='python')
                                
             data = data.drop(data.index[:drop], axis=0)
             data.dropna(axis=1, how='all', inplace=True)
             data = data.apply(pd.to_numeric, errors='coerce')
```

### Comparing `imgMS-0.2.5/imgMS/MSStats.py` & `imgMS-0.2.6/imgMS/MSStats.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.5/imgMS/side_functions.py` & `imgMS-0.2.6/imgMS/side_functions.py`

 * *Files identical despite different names*

### Comparing `imgMS-0.2.5/imgMS.egg-info/PKG-INFO` & `imgMS-0.2.6/imgMS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgMS
-Version: 0.2.5
+Version: 0.2.6
 Summary: Package for data reduction of LA-ICP-MS data.
 Home-page: https://github.com/nikadilli/imgMS
 Author: nikadilli
 Author-email: nikadilli@gmail.com
 License: LICENSE.txt
 Description: [![Documentation Status](https://readthedocs.org/projects/imgms/badge/?version=latest)](https://imgms.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `imgMS-0.2.5/setup.py` & `imgMS-0.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='imgMS',
-    version='0.2.5',
+    version='0.2.6',
     author='nikadilli',
     author_email='nikadilli@gmail.com',
     url="https://github.com/nikadilli/imgMS",
     packages=setuptools.find_packages(),
     scripts=[],
     license='LICENSE.txt',
     description='Package for data reduction of LA-ICP-MS data.',
```

