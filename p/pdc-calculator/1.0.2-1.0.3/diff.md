# Comparing `tmp/pdc_calculator-1.0.2.tar.gz` & `tmp/pdc_calculator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdc_calculator-1.0.2.tar", last modified: Thu May  4 00:10:46 2023, max compression
+gzip compressed data, was "pdc_calculator-1.0.3.tar", last modified: Thu May  4 01:10:40 2023, max compression
```

## Comparing `pdc_calculator-1.0.2.tar` & `pdc_calculator-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 00:10:46.161466 pdc_calculator-1.0.2/
--rw-rw-rw-   0        0        0     4665 2023-05-04 00:10:46.161466 pdc_calculator-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3634 2023-05-04 00:07:09.000000 pdc_calculator-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 00:10:46.158465 pdc_calculator-1.0.2/pdc_calculator.egg-info/
--rw-rw-rw-   0        0        0     4665 2023-05-04 00:10:46.000000 pdc_calculator-1.0.2/pdc_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-04 00:10:46.000000 pdc_calculator-1.0.2/pdc_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 00:10:46.000000 pdc_calculator-1.0.2/pdc_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 00:10:46.000000 pdc_calculator-1.0.2/pdc_calculator.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 00:10:46.000000 pdc_calculator-1.0.2/pdc_calculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 00:10:46.162466 pdc_calculator-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1494 2023-05-04 00:09:47.000000 pdc_calculator-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:10:40.074087 pdc_calculator-1.0.3/
+-rw-rw-rw-   0        0        0     4678 2023-05-04 01:10:40.073085 pdc_calculator-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3634 2023-05-04 00:07:09.000000 pdc_calculator-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 01:10:40.071086 pdc_calculator-1.0.3/pdc_calculator.egg-info/
+-rw-rw-rw-   0        0        0     4678 2023-05-04 01:10:39.000000 pdc_calculator-1.0.3/pdc_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-04 01:10:40.000000 pdc_calculator-1.0.3/pdc_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 01:10:39.000000 pdc_calculator-1.0.3/pdc_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 01:10:39.000000 pdc_calculator-1.0.3/pdc_calculator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 01:10:39.000000 pdc_calculator-1.0.3/pdc_calculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 01:10:40.074087 pdc_calculator-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1538 2023-05-04 01:10:27.000000 pdc_calculator-1.0.3/setup.py
```

### Comparing `pdc_calculator-1.0.2/PKG-INFO` & `pdc_calculator-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pdc_calculator
-Version: 1.0.2
-Summary: A package to facilitate efficient calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
+Version: 1.0.3
+Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pdc_calculator-1.0.2/README.md` & `pdc_calculator-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pdc_calculator-1.0.2/pdc_calculator.egg-info/PKG-INFO` & `pdc_calculator-1.0.3/pdc_calculator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pdc-calculator
-Version: 1.0.2
-Summary: A package to facilitate efficient calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
+Version: 1.0.3
+Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pdc_calculator-1.0.2/setup.py` & `pdc_calculator-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from setuptools import setup, find_packages
-
-from setuptools import setup, find_packages
-
 import os
 
 dir_path = r'C:\Users\famut'
 file_name = 'README.md'
 
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdc_calculator',
-    version='1.0.2',
-    description='A package to facilitate efficient calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
+    version='1.0.3',
+    description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # url='https://github.com/<username>/<repository>',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
     classifiers=[
@@ -32,13 +29,14 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
         'Topic :: Scientific/Engineering :: Information Analysis',
     ],
     keywords='pdc calculator medication adherence',
-    packages=find_packages(),
+    packages=find_packages(include=['pdc_calculator', 'pdc_calculator.*']),
+    include_package_data=True,
     install_requires=[
         'numpy',
         'pandas',
     ],
 )
```

