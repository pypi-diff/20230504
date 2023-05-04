# Comparing `tmp/oh_einstein_temp_convert-0.0.8.tar.gz` & `tmp/oh_einstein_temp_convert-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oh_einstein_temp_convert-0.0.8.tar", last modified: Thu May  4 14:55:40 2023, max compression
+gzip compressed data, was "oh_einstein_temp_convert-1.0.0.tar", last modified: Thu May  4 15:01:42 2023, max compression
```

## Comparing `oh_einstein_temp_convert-0.0.8.tar` & `oh_einstein_temp_convert-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rowan     (1000) rowan     (1000)        0 2023-05-04 14:55:40.647790 oh_einstein_temp_convert-0.0.8/
--rw-rw-r--   0 rowan     (1000) rowan     (1000)    35129 2023-05-04 09:05:51.000000 oh_einstein_temp_convert-0.0.8/LICENSE
--rw-rw-r--   0 rowan     (1000) rowan     (1000)      103 2023-05-04 14:36:12.000000 oh_einstein_temp_convert-0.0.8/MANIFEST.in
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     5190 2023-05-04 14:55:40.647790 oh_einstein_temp_convert-0.0.8/PKG-INFO
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     4748 2023-05-04 13:29:55.000000 oh_einstein_temp_convert-0.0.8/README.md
--rw-rw-r--   0 rowan     (1000) rowan     (1000)       24 2023-05-04 14:50:59.000000 oh_einstein_temp_convert-0.0.8/Requirements.txt
-drwxrwxr-x   0 rowan     (1000) rowan     (1000)        0 2023-05-04 14:55:40.647790 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/
--rw-rw-r--   0 rowan     (1000) rowan     (1000)       67 2023-05-03 13:01:01.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/__init__.py
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     7909 2023-05-04 13:44:02.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/convert.py
-drwxrwxr-x   0 rowan     (1000) rowan     (1000)        0 2023-05-04 14:55:40.647790 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     1128 2023-05-02 13:45:13.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/GSC_QUANT.txt
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     1121 2023-04-12 10:39:09.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/LG_QUANT.txt
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     1139 2023-05-04 12:49:43.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/LWR_QUANT.txt
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     1122 2023-04-12 10:20:57.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/MIES_QUANT.txt
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     1129 2023-05-04 12:49:10.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/TL_QUANT.txt
-drwxrwxr-x   0 rowan     (1000) rowan     (1000)        0 2023-05-04 14:55:40.647790 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert.egg-info/
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     5190 2023-05-04 14:55:40.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert.egg-info/PKG-INFO
--rw-rw-r--   0 rowan     (1000) rowan     (1000)      586 2023-05-04 14:55:40.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert.egg-info/SOURCES.txt
--rw-rw-r--   0 rowan     (1000) rowan     (1000)        1 2023-05-04 14:55:40.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert.egg-info/dependency_links.txt
--rw-rw-r--   0 rowan     (1000) rowan     (1000)       24 2023-05-04 14:55:40.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert.egg-info/requires.txt
--rw-rw-r--   0 rowan     (1000) rowan     (1000)       25 2023-05-04 14:55:40.000000 oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert.egg-info/top_level.txt
--rw-rw-r--   0 rowan     (1000) rowan     (1000)       38 2023-05-04 14:55:40.647790 oh_einstein_temp_convert-0.0.8/setup.cfg
--rw-rw-r--   0 rowan     (1000) rowan     (1000)     2102 2023-05-04 14:54:11.000000 oh_einstein_temp_convert-0.0.8/setup.py
+drwxrwxr-x   0 rowan     (1000) rowan     (1000)        0 2023-05-04 15:01:42.061225 oh_einstein_temp_convert-1.0.0/
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)    35129 2023-05-04 09:05:51.000000 oh_einstein_temp_convert-1.0.0/LICENSE
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)      103 2023-05-04 14:36:12.000000 oh_einstein_temp_convert-1.0.0/MANIFEST.in
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     5190 2023-05-04 15:01:42.061225 oh_einstein_temp_convert-1.0.0/PKG-INFO
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     4748 2023-05-04 13:29:55.000000 oh_einstein_temp_convert-1.0.0/README.md
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)       24 2023-05-04 14:50:59.000000 oh_einstein_temp_convert-1.0.0/Requirements.txt
+drwxrwxr-x   0 rowan     (1000) rowan     (1000)        0 2023-05-04 15:01:42.057224 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)       67 2023-05-03 13:01:01.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/__init__.py
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     7909 2023-05-04 13:44:02.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/convert.py
+drwxrwxr-x   0 rowan     (1000) rowan     (1000)        0 2023-05-04 15:01:42.057224 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     1128 2023-05-02 13:45:13.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/GSC_QUANT.txt
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     1121 2023-04-12 10:39:09.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/LG_QUANT.txt
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     1139 2023-05-04 12:49:43.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/LWR_QUANT.txt
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     1122 2023-04-12 10:20:57.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/MIES_QUANT.txt
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     1129 2023-05-04 12:49:10.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/TL_QUANT.txt
+drwxrwxr-x   0 rowan     (1000) rowan     (1000)        0 2023-05-04 15:01:42.057224 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert.egg-info/
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     5190 2023-05-04 15:01:41.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert.egg-info/PKG-INFO
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)      586 2023-05-04 15:01:42.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert.egg-info/SOURCES.txt
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)        1 2023-05-04 15:01:41.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert.egg-info/dependency_links.txt
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)       24 2023-05-04 15:01:41.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert.egg-info/requires.txt
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)       25 2023-05-04 15:01:41.000000 oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert.egg-info/top_level.txt
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)       38 2023-05-04 15:01:42.061225 oh_einstein_temp_convert-1.0.0/setup.cfg
+-rw-rw-r--   0 rowan     (1000) rowan     (1000)     2102 2023-05-04 15:01:26.000000 oh_einstein_temp_convert-1.0.0/setup.py
```

### Comparing `oh_einstein_temp_convert-0.0.8/LICENSE` & `oh_einstein_temp_convert-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oh_einstein_temp_convert-0.0.8/PKG-INFO` & `oh_einstein_temp_convert-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oh_einstein_temp_convert
-Version: 0.0.8
+Version: 1.0.0
 Summary: Tool to convert temperatures OH*(6-2) between two sets of Einstein A coefficients.
 Author: Rowan Dayton-Oxland
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `oh_einstein_temp_convert-0.0.8/README.md` & `oh_einstein_temp_convert-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/convert.py` & `oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/convert.py`

 * *Files identical despite different names*

### Comparing `oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/GSC_QUANT.txt` & `oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/GSC_QUANT.txt`

 * *Files identical despite different names*

### Comparing `oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/LG_QUANT.txt` & `oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/LG_QUANT.txt`

 * *Files identical despite different names*

### Comparing `oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/LWR_QUANT.txt` & `oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/LWR_QUANT.txt`

 * *Files identical despite different names*

### Comparing `oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/MIES_QUANT.txt` & `oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/MIES_QUANT.txt`

 * *Files identical despite different names*

### Comparing `oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert/data/TL_QUANT.txt` & `oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert/data/TL_QUANT.txt`

 * *Files identical despite different names*

### Comparing `oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert.egg-info/PKG-INFO` & `oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oh-einstein-temp-convert
-Version: 0.0.8
+Version: 1.0.0
 Summary: Tool to convert temperatures OH*(6-2) between two sets of Einstein A coefficients.
 Author: Rowan Dayton-Oxland
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `oh_einstein_temp_convert-0.0.8/oh_einstein_temp_convert.egg-info/SOURCES.txt` & `oh_einstein_temp_convert-1.0.0/oh_einstein_temp_convert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oh_einstein_temp_convert-0.0.8/setup.py` & `oh_einstein_temp_convert-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     long_description = fh.read()
 
 with open("Requirements.txt", 'r') as fh:
 	requirements = [s.strip() for s in fh.readlines()] 
 
 setup(
     name="oh_einstein_temp_convert",
-    version="0.0.8",
+    version="1.0.0",
     author="Rowan Dayton-Oxland",
     description="Tool to convert temperatures OH*(6-2) between two sets of Einstein A coefficients.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
     classifiers=[
```

