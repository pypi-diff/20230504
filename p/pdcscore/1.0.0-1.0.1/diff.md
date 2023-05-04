# Comparing `tmp/pdcscore-1.0.0.tar.gz` & `tmp/pdcscore-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdcscore-1.0.0.tar", last modified: Thu May  4 05:08:52 2023, max compression
+gzip compressed data, was "pdcscore-1.0.1.tar", last modified: Thu May  4 05:18:26 2023, max compression
```

## Comparing `pdcscore-1.0.0.tar` & `pdcscore-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 05:08:52.928020 pdcscore-1.0.0/
--rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4664 2023-05-04 05:08:52.927020 pdcscore-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3528 2023-05-04 05:06:25.000000 pdcscore-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 05:08:52.903021 pdcscore-1.0.0/libname/
--rw-rw-rw-   0        0        0       28 2023-05-04 05:06:51.000000 pdcscore-1.0.0/libname/__init__.py
--rw-rw-rw-   0        0        0     3329 2023-05-04 05:07:44.000000 pdcscore-1.0.0/libname/pdccalculator.py
-drwxrwxrwx   0        0        0        0 2023-05-04 05:08:52.926019 pdcscore-1.0.0/pdcscore.egg-info/
--rw-rw-rw-   0        0        0     4664 2023-05-04 05:08:52.000000 pdcscore-1.0.0/pdcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-04 05:08:52.000000 pdcscore-1.0.0/pdcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 05:08:52.000000 pdcscore-1.0.0/pdcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 05:08:52.000000 pdcscore-1.0.0/pdcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 05:08:52.000000 pdcscore-1.0.0/pdcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 05:08:52.928020 pdcscore-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1502 2023-05-04 05:05:41.000000 pdcscore-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:18:26.031380 pdcscore-1.0.1/
+-rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4664 2023-05-04 05:18:26.030380 pdcscore-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3528 2023-05-04 05:06:25.000000 pdcscore-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 05:18:26.015373 pdcscore-1.0.1/libname/
+-rw-rw-rw-   0        0        0       28 2023-05-04 05:06:51.000000 pdcscore-1.0.1/libname/__init__.py
+-rw-rw-rw-   0        0        0     3329 2023-05-04 05:07:44.000000 pdcscore-1.0.1/libname/pdcscore.py
+drwxrwxrwx   0        0        0        0 2023-05-04 05:18:26.029379 pdcscore-1.0.1/pdcscore.egg-info/
+-rw-rw-rw-   0        0        0     4664 2023-05-04 05:18:25.000000 pdcscore-1.0.1/pdcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-05-04 05:18:25.000000 pdcscore-1.0.1/pdcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 05:18:25.000000 pdcscore-1.0.1/pdcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 05:18:25.000000 pdcscore-1.0.1/pdcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 05:18:25.000000 pdcscore-1.0.1/pdcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 05:18:26.031380 pdcscore-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1502 2023-05-04 05:17:55.000000 pdcscore-1.0.1/setup.py
```

### Comparing `pdcscore-1.0.0/LICENSE` & `pdcscore-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.0/PKG-INFO` & `pdcscore-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
```

### Comparing `pdcscore-1.0.0/README.md` & `pdcscore-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.0/libname/pdccalculator.py` & `pdcscore-1.0.1/libname/pdcscore.py`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.0/pdcscore.egg-info/PKG-INFO` & `pdcscore-1.0.1/pdcscore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
```

### Comparing `pdcscore-1.0.0/setup.py` & `pdcscore-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdcscore',
-    version='1.0.0',
+    version='1.0.1',
     description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # url='https://github.com/<username>/<repository>',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

