# Comparing `tmp/pdcscore-1.0.7.tar.gz` & `tmp/pdcscore-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdcscore-1.0.7.tar", last modified: Thu May  4 14:04:00 2023, max compression
+gzip compressed data, was "pdcscore-1.0.8.tar", last modified: Thu May  4 16:34:20 2023, max compression
```

## Comparing `pdcscore-1.0.7.tar` & `pdcscore-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 14:04:00.899325 pdcscore-1.0.7/
--rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     4793 2023-05-04 14:04:00.899325 pdcscore-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3661 2023-05-04 14:03:32.000000 pdcscore-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 14:04:00.882325 pdcscore-1.0.7/pdcscore/
--rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.0.7/pdcscore/__init__.py
--rw-rw-rw-   0        0        0     3487 2023-05-04 06:22:38.000000 pdcscore-1.0.7/pdcscore/pdcscore.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:04:00.897326 pdcscore-1.0.7/pdcscore.egg-info/
--rw-rw-rw-   0        0        0     4793 2023-05-04 14:04:00.000000 pdcscore-1.0.7/pdcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-04 14:04:00.000000 pdcscore-1.0.7/pdcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 14:04:00.000000 pdcscore-1.0.7/pdcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 14:04:00.000000 pdcscore-1.0.7/pdcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 14:04:00.000000 pdcscore-1.0.7/pdcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 14:04:00.899325 pdcscore-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1502 2023-05-04 14:01:21.000000 pdcscore-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:34:20.580328 pdcscore-1.0.8/
+-rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4912 2023-05-04 16:34:20.580328 pdcscore-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3670 2023-05-04 15:57:03.000000 pdcscore-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 16:34:20.550944 pdcscore-1.0.8/pdcscore/
+-rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.0.8/pdcscore/__init__.py
+-rw-rw-rw-   0        0        0     3487 2023-05-04 06:22:38.000000 pdcscore-1.0.8/pdcscore/pdcscore.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:34:20.578329 pdcscore-1.0.8/pdcscore.egg-info/
+-rw-rw-rw-   0        0        0     4912 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:34:20.581330 pdcscore-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1608 2023-05-04 16:01:57.000000 pdcscore-1.0.8/setup.py
```

### Comparing `pdcscore-1.0.7/LICENSE` & `pdcscore-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.7/PKG-INFO` & `pdcscore-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -42,15 +44,15 @@
 
 **filldate_col** - *The date of the fill being dispensed. Format = DATE*
 
 **supply_days_col** - *Days of supply being dispensed at fill. Format = INTEGER*
 
 **mbr_elig_start_dt_col** - *First date of coverage eligiblity for patient or a reference START DATE. Format = DATE*
 
-**MBRELIGEND** - *Last date of coverage eligiblity for patient or a reference END DATE. Format = DATE*
+**mbr_elig_end_dt_col** - *Last date of coverage eligiblity for patient or a reference END DATE. Format = DATE*
 
 **Returns** - *A Pandas dataframe containing the following columns*
 
 **patient_id_col** - *This will return a column name representing a unique patient identifier as provided in original input dataframe. FORMAT = STRING*
 
 **drugname_col** - *The name of the drug being filled or drug class or Generic name, as provided in original input dataframe.*
```

### Comparing `pdcscore-1.0.7/README.md` & `pdcscore-1.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 **filldate_col** - *The date of the fill being dispensed. Format = DATE*
 
 **supply_days_col** - *Days of supply being dispensed at fill. Format = INTEGER*
 
 **mbr_elig_start_dt_col** - *First date of coverage eligiblity for patient or a reference START DATE. Format = DATE*
 
-**MBRELIGEND** - *Last date of coverage eligiblity for patient or a reference END DATE. Format = DATE*
+**mbr_elig_end_dt_col** - *Last date of coverage eligiblity for patient or a reference END DATE. Format = DATE*
 
 **Returns** - *A Pandas dataframe containing the following columns*
 
 **patient_id_col** - *This will return a column name representing a unique patient identifier as provided in original input dataframe. FORMAT = STRING*
 
 **drugname_col** - *The name of the drug being filled or drug class or Generic name, as provided in original input dataframe.*
```

### Comparing `pdcscore-1.0.7/pdcscore/pdcscore.py` & `pdcscore-1.0.8/pdcscore/pdcscore.py`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.7/pdcscore.egg-info/PKG-INFO` & `pdcscore-1.0.8/pdcscore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -42,15 +44,15 @@
 
 **filldate_col** - *The date of the fill being dispensed. Format = DATE*
 
 **supply_days_col** - *Days of supply being dispensed at fill. Format = INTEGER*
 
 **mbr_elig_start_dt_col** - *First date of coverage eligiblity for patient or a reference START DATE. Format = DATE*
 
-**MBRELIGEND** - *Last date of coverage eligiblity for patient or a reference END DATE. Format = DATE*
+**mbr_elig_end_dt_col** - *Last date of coverage eligiblity for patient or a reference END DATE. Format = DATE*
 
 **Returns** - *A Pandas dataframe containing the following columns*
 
 **patient_id_col** - *This will return a column name representing a unique patient identifier as provided in original input dataframe. FORMAT = STRING*
 
 **drugname_col** - *The name of the drug being filled or drug class or Generic name, as provided in original input dataframe.*
```

### Comparing `pdcscore-1.0.7/setup.py` & `pdcscore-1.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdcscore',
-    version='1.0.7',
+    version='1.0.8',
     description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # url='https://github.com/<username>/<repository>',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
+        'Intended Audience :: Healthcare Industry',
+        'Intended Audience :: System Administrators',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

