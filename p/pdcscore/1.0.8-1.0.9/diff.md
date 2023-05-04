# Comparing `tmp/pdcscore-1.0.8.tar.gz` & `tmp/pdcscore-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdcscore-1.0.8.tar", last modified: Thu May  4 16:34:20 2023, max compression
+gzip compressed data, was "pdcscore-1.0.9.tar", last modified: Thu May  4 16:47:51 2023, max compression
```

## Comparing `pdcscore-1.0.8.tar` & `pdcscore-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:34:20.580328 pdcscore-1.0.8/
--rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     4912 2023-05-04 16:34:20.580328 pdcscore-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3670 2023-05-04 15:57:03.000000 pdcscore-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 16:34:20.550944 pdcscore-1.0.8/pdcscore/
--rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.0.8/pdcscore/__init__.py
--rw-rw-rw-   0        0        0     3487 2023-05-04 06:22:38.000000 pdcscore-1.0.8/pdcscore/pdcscore.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:34:20.578329 pdcscore-1.0.8/pdcscore.egg-info/
--rw-rw-rw-   0        0        0     4912 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 16:34:20.000000 pdcscore-1.0.8/pdcscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 16:34:20.581330 pdcscore-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1608 2023-05-04 16:01:57.000000 pdcscore-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:47:51.758205 pdcscore-1.0.9/
+-rw-rw-rw-   0        0        0     1099 2023-05-04 02:23:33.000000 pdcscore-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4931 2023-05-04 16:47:51.758205 pdcscore-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3687 2023-05-04 16:46:18.000000 pdcscore-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 16:47:51.737174 pdcscore-1.0.9/pdcscore/
+-rw-rw-rw-   0        0        0       79 2023-05-04 06:00:07.000000 pdcscore-1.0.9/pdcscore/__init__.py
+-rw-rw-rw-   0        0        0     3487 2023-05-04 06:22:38.000000 pdcscore-1.0.9/pdcscore/pdcscore.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:47:51.756207 pdcscore-1.0.9/pdcscore.egg-info/
+-rw-rw-rw-   0        0        0     4931 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 16:47:51.000000 pdcscore-1.0.9/pdcscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:47:51.759212 pdcscore-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1608 2023-05-04 16:46:13.000000 pdcscore-1.0.9/setup.py
```

### Comparing `pdcscore-1.0.8/LICENSE` & `pdcscore-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.8/PKG-INFO` & `pdcscore-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
@@ -30,15 +30,15 @@
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 Current update is optimized for multiprocessing large datasets.
 
 Please use as described below:
 
-**PARAMETERS:**
+**INPUT PARAMETERS:**
 
 **dataframe** - *A pandas dataframe containing the required columns described below.*
 
 **patient_id_col** - *A unique patient identifier. Format = STRING or INTEGER*
 
 **drugname_col** - *The name of the drug being filled or drug class or Generic name, per usual PDC requirements. Format = STRING*
 
@@ -46,15 +46,17 @@
 
 **supply_days_col** - *Days of supply being dispensed at fill. Format = INTEGER*
 
 **mbr_elig_start_dt_col** - *First date of coverage eligiblity for patient or a reference START DATE. Format = DATE*
 
 **mbr_elig_end_dt_col** - *Last date of coverage eligiblity for patient or a reference END DATE. Format = DATE*
 
-**Returns** - *A Pandas dataframe containing the following columns*
+
+
+**OUTPUT DATAFRAME** - *A Pandas dataframe containing the following columns*
 
 **patient_id_col** - *This will return a column name representing a unique patient identifier as provided in original input dataframe. FORMAT = STRING*
 
 **drugname_col** - *The name of the drug being filled or drug class or Generic name, as provided in original input dataframe.*
 
 **DAYSCOVERED**- *The number of unique days of drug coverage, after shifting coverage to accommodate early refills. FORMAT = INTEGER*
```

### Comparing `pdcscore-1.0.8/README.md` & `pdcscore-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 Current update is optimized for multiprocessing large datasets.
 
 Please use as described below:
 
-**PARAMETERS:**
+**INPUT PARAMETERS:**
 
 **dataframe** - *A pandas dataframe containing the required columns described below.*
 
 **patient_id_col** - *A unique patient identifier. Format = STRING or INTEGER*
 
 **drugname_col** - *The name of the drug being filled or drug class or Generic name, per usual PDC requirements. Format = STRING*
 
@@ -20,15 +20,17 @@
 
 **supply_days_col** - *Days of supply being dispensed at fill. Format = INTEGER*
 
 **mbr_elig_start_dt_col** - *First date of coverage eligiblity for patient or a reference START DATE. Format = DATE*
 
 **mbr_elig_end_dt_col** - *Last date of coverage eligiblity for patient or a reference END DATE. Format = DATE*
 
-**Returns** - *A Pandas dataframe containing the following columns*
+
+
+**OUTPUT DATAFRAME** - *A Pandas dataframe containing the following columns*
 
 **patient_id_col** - *This will return a column name representing a unique patient identifier as provided in original input dataframe. FORMAT = STRING*
 
 **drugname_col** - *The name of the drug being filled or drug class or Generic name, as provided in original input dataframe.*
 
 **DAYSCOVERED**- *The number of unique days of drug coverage, after shifting coverage to accommodate early refills. FORMAT = INTEGER*
```

### Comparing `pdcscore-1.0.8/pdcscore/pdcscore.py` & `pdcscore-1.0.9/pdcscore/pdcscore.py`

 * *Files identical despite different names*

### Comparing `pdcscore-1.0.8/pdcscore.egg-info/PKG-INFO` & `pdcscore-1.0.9/pdcscore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdcscore
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
@@ -30,15 +30,15 @@
 
 This paper offers a gentle, yet detailed introduction to the topic, and will serve as a reference to anyone new to the subject.
 
 Current update is optimized for multiprocessing large datasets.
 
 Please use as described below:
 
-**PARAMETERS:**
+**INPUT PARAMETERS:**
 
 **dataframe** - *A pandas dataframe containing the required columns described below.*
 
 **patient_id_col** - *A unique patient identifier. Format = STRING or INTEGER*
 
 **drugname_col** - *The name of the drug being filled or drug class or Generic name, per usual PDC requirements. Format = STRING*
 
@@ -46,15 +46,17 @@
 
 **supply_days_col** - *Days of supply being dispensed at fill. Format = INTEGER*
 
 **mbr_elig_start_dt_col** - *First date of coverage eligiblity for patient or a reference START DATE. Format = DATE*
 
 **mbr_elig_end_dt_col** - *Last date of coverage eligiblity for patient or a reference END DATE. Format = DATE*
 
-**Returns** - *A Pandas dataframe containing the following columns*
+
+
+**OUTPUT DATAFRAME** - *A Pandas dataframe containing the following columns*
 
 **patient_id_col** - *This will return a column name representing a unique patient identifier as provided in original input dataframe. FORMAT = STRING*
 
 **drugname_col** - *The name of the drug being filled or drug class or Generic name, as provided in original input dataframe.*
 
 **DAYSCOVERED**- *The number of unique days of drug coverage, after shifting coverage to accommodate early refills. FORMAT = INTEGER*
```

### Comparing `pdcscore-1.0.8/setup.py` & `pdcscore-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdcscore',
-    version='1.0.8',
+    version='1.0.9',
     description='A package to facilitate efficient and accurate calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # url='https://github.com/<username>/<repository>',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

