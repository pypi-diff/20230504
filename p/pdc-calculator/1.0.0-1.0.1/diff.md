# Comparing `tmp/pdc_calculator-1.0.0.tar.gz` & `tmp/pdc_calculator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdc_calculator-1.0.0.tar", last modified: Wed May  3 23:27:13 2023, max compression
+gzip compressed data, was "pdc_calculator-1.0.1.tar", last modified: Wed May  3 23:52:14 2023, max compression
```

## Comparing `pdc_calculator-1.0.0.tar` & `pdc_calculator-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 23:27:13.670103 pdc_calculator-1.0.0/
--rw-rw-rw-   0        0        0     4537 2023-05-03 23:27:13.669104 pdc_calculator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3514 2023-05-03 23:23:41.000000 pdc_calculator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 23:27:13.668107 pdc_calculator-1.0.0/pdc_calculator.egg-info/
--rw-rw-rw-   0        0        0     4537 2023-05-03 23:27:13.000000 pdc_calculator-1.0.0/pdc_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-03 23:27:13.000000 pdc_calculator-1.0.0/pdc_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 23:27:13.000000 pdc_calculator-1.0.0/pdc_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 23:27:13.000000 pdc_calculator-1.0.0/pdc_calculator.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 23:27:13.000000 pdc_calculator-1.0.0/pdc_calculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 23:27:13.670103 pdc_calculator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-05-03 23:27:03.000000 pdc_calculator-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 23:52:14.491764 pdc_calculator-1.0.1/
+-rw-rw-rw-   0        0        0     4573 2023-05-03 23:52:14.490765 pdc_calculator-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3542 2023-05-03 23:48:32.000000 pdc_calculator-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 23:52:14.489764 pdc_calculator-1.0.1/pdc_calculator.egg-info/
+-rw-rw-rw-   0        0        0     4573 2023-05-03 23:52:14.000000 pdc_calculator-1.0.1/pdc_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-03 23:52:14.000000 pdc_calculator-1.0.1/pdc_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 23:52:14.000000 pdc_calculator-1.0.1/pdc_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 23:52:14.000000 pdc_calculator-1.0.1/pdc_calculator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 23:52:14.000000 pdc_calculator-1.0.1/pdc_calculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 23:52:14.491764 pdc_calculator-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1494 2023-05-03 23:51:16.000000 pdc_calculator-1.0.1/setup.py
```

### Comparing `pdc_calculator-1.0.0/PKG-INFO` & `pdc_calculator-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pdc_calculator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to facilitate efficient calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
-Author: Daniel Famutimi
+Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -32,28 +32,38 @@
 Please use as described below:
 
 Parameters:
 
 dataframe - A pandas dataframe containing the required columns described below.
 
 patient_id_col - A unique patient identifier. Format = Accepts STRING or INTEGER
+
 drugname_col - The name of the drug being filled or drug class or Generic name, per usual PDC requirements. Format = STRING
+
 filldate_col - The date of the fill being dispensed. Format = DATE
+
 supply_days_col - Days of supply being dispensed at fill. Format = INTEGER
+
 mbr_elig_start_dt_col - First date of coverage eligiblity for patient or a reference start date. Format = DATE
+
 MBRELIGEND - Last date of coverage eligiblity for patient or a reference start date. Format = DATE
+
 Returns - A Pandas dataframe containing the following columns
 
 *patient_id_col - This will return a column name representing a unique patient identifier as provided in your original input dataframe. FORMAT = STRING
+
 *drugname_col - The name of the drug being filled or drug class or Generic name, as provided in input.
+
 DAYSCOVERED- The number of unique days of drug coverage, after shifting coverage to accommodate early refills. FORMAT = INTEGER
+
 TOTALDAYS - The total number of days in patient analysis window. Set to 0 if days of coverage is 0. FORMAT = INTEGER
+
 PDC_SCORE - The patient's PDC score, calculated as DAYSCOVERED / TOTALDAYS. Set to 0 if days of coverage is 0. FORMAT = FLOAT
 
-Usage
+USAGE EXAMPLE
 
 ```python
 
 #  Import required libraries
 import pandas as pd
 import numpy as np
 from pdc_calculator import PDC_Calculator
```

### Comparing `pdc_calculator-1.0.0/README.md` & `pdc_calculator-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,38 @@
 Please use as described below:
 
 Parameters:
 
 dataframe - A pandas dataframe containing the required columns described below.
 
 patient_id_col - A unique patient identifier. Format = Accepts STRING or INTEGER
+
 drugname_col - The name of the drug being filled or drug class or Generic name, per usual PDC requirements. Format = STRING
+
 filldate_col - The date of the fill being dispensed. Format = DATE
+
 supply_days_col - Days of supply being dispensed at fill. Format = INTEGER
+
 mbr_elig_start_dt_col - First date of coverage eligiblity for patient or a reference start date. Format = DATE
+
 MBRELIGEND - Last date of coverage eligiblity for patient or a reference start date. Format = DATE
+
 Returns - A Pandas dataframe containing the following columns
 
 *patient_id_col - This will return a column name representing a unique patient identifier as provided in your original input dataframe. FORMAT = STRING
+
 *drugname_col - The name of the drug being filled or drug class or Generic name, as provided in input.
+
 DAYSCOVERED- The number of unique days of drug coverage, after shifting coverage to accommodate early refills. FORMAT = INTEGER
+
 TOTALDAYS - The total number of days in patient analysis window. Set to 0 if days of coverage is 0. FORMAT = INTEGER
+
 PDC_SCORE - The patient's PDC score, calculated as DAYSCOVERED / TOTALDAYS. Set to 0 if days of coverage is 0. FORMAT = FLOAT
 
-Usage
+USAGE EXAMPLE
 
 ```python
 
 #  Import required libraries
 import pandas as pd
 import numpy as np
 from pdc_calculator import PDC_Calculator
```

### Comparing `pdc_calculator-1.0.0/pdc_calculator.egg-info/PKG-INFO` & `pdc_calculator-1.0.1/pdc_calculator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pdc-calculator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to facilitate efficient calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".
 Home-page: UNKNOWN
-Author: Daniel Famutimi
+Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: pdc calculator medication adherence
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -32,28 +32,38 @@
 Please use as described below:
 
 Parameters:
 
 dataframe - A pandas dataframe containing the required columns described below.
 
 patient_id_col - A unique patient identifier. Format = Accepts STRING or INTEGER
+
 drugname_col - The name of the drug being filled or drug class or Generic name, per usual PDC requirements. Format = STRING
+
 filldate_col - The date of the fill being dispensed. Format = DATE
+
 supply_days_col - Days of supply being dispensed at fill. Format = INTEGER
+
 mbr_elig_start_dt_col - First date of coverage eligiblity for patient or a reference start date. Format = DATE
+
 MBRELIGEND - Last date of coverage eligiblity for patient or a reference start date. Format = DATE
+
 Returns - A Pandas dataframe containing the following columns
 
 *patient_id_col - This will return a column name representing a unique patient identifier as provided in your original input dataframe. FORMAT = STRING
+
 *drugname_col - The name of the drug being filled or drug class or Generic name, as provided in input.
+
 DAYSCOVERED- The number of unique days of drug coverage, after shifting coverage to accommodate early refills. FORMAT = INTEGER
+
 TOTALDAYS - The total number of days in patient analysis window. Set to 0 if days of coverage is 0. FORMAT = INTEGER
+
 PDC_SCORE - The patient's PDC score, calculated as DAYSCOVERED / TOTALDAYS. Set to 0 if days of coverage is 0. FORMAT = FLOAT
 
-Usage
+USAGE EXAMPLE
 
 ```python
 
 #  Import required libraries
 import pandas as pd
 import numpy as np
 from pdc_calculator import PDC_Calculator
```

### Comparing `pdc_calculator-1.0.0/setup.py` & `pdc_calculator-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 file_path = os.path.join(dir_path, file_name)
 
 with open(file_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pdc_calculator',
-    version='1.0.0',
+    version='1.0.1',
     description='A package to facilitate efficient calculation of the medication adherence metric "Proportion of Days Covered" or "PDC".',
     long_description=long_description,
     long_description_content_type='text/markdown',
     # url='https://github.com/<username>/<repository>',
-    author='Daniel Famutimi',
+    author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

