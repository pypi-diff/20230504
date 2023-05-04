# Comparing `tmp/PICNIK-0.1.7.tar.gz` & `tmp/PICNIK-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PICNIK-0.1.7.tar", max compression
+gzip compressed data, was "PICNIK-0.1.8.tar", max compression
```

## Comparing `PICNIK-0.1.7.tar` & `PICNIK-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2021-09-25 21:35:05.028501 PICNIK-0.1.7/LICENSE
--rw-r--r--   0        0        0     3757 2022-03-04 06:36:33.169397 PICNIK-0.1.7/README.md
--rw-r--r--   0        0        0    84067 2022-03-18 19:25:47.981210 PICNIK-0.1.7/picnik.py
--rw-r--r--   0        0        0      695 2023-05-04 00:56:38.007967 PICNIK-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4578 2023-05-04 00:59:08.315528 PICNIK-0.1.7/setup.py
--rw-r--r--   0        0        0     4676 2023-05-04 00:59:08.316328 PICNIK-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2021-09-25 21:35:05.028501 PICNIK-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3757 2022-03-04 06:36:33.169397 PICNIK-0.1.8/README.md
+-rw-r--r--   0        0        0    84067 2022-03-18 19:25:47.981210 PICNIK-0.1.8/picnik.py
+-rw-r--r--   0        0        0      695 2023-05-04 01:14:47.039371 PICNIK-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4578 2023-05-04 01:14:51.749279 PICNIK-0.1.8/setup.py
+-rw-r--r--   0        0        0     4676 2023-05-04 01:14:51.750071 PICNIK-0.1.8/PKG-INFO
```

### Comparing `PICNIK-0.1.7/LICENSE` & `PICNIK-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PICNIK-0.1.7/README.md` & `PICNIK-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `PICNIK-0.1.7/picnik.py` & `PICNIK-0.1.8/picnik.py`

 * *Files identical despite different names*

### Comparing `PICNIK-0.1.7/pyproject.toml` & `PICNIK-0.1.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PICNIK"
-version = "0.1.7"
+version = "0.1.8"
 description = "A package to make isoconversional computations for non-isothermal kinetics"
 authors = ["ErickErock <ramirez.orozco.erick@gmail.com>","Sergio Hernandez <sergiohzlz@ciencias.unam.mx>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/ErickErock/pICNIK"
 keywords = ["non-isothermal kinetics", "isoconversion","isoconversional computations"]
```

### Comparing `PICNIK-0.1.7/setup.py` & `PICNIK-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
  'matplotlib>=3.1.2,<4.0.0',
  'numpy>=1.19.1,<2.0.0',
  'pandas>=1.2.2,<2.0.0',
  'scipy>=1.6.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'picnik',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'A package to make isoconversional computations for non-isothermal kinetics',
     'long_description': '# pICNIK \n\npICNIK is a module with implemented isoconversional computations for non-isothermal kinetcis.\\\nThe package has an object oriented interface with two classes: DataExtraction and ActivationEnergy, with the purpose of managing the experimental data and computing activation energies  with the next isoconversional methods: \n\n- Ozawa-Flynn-Wall (OFW)\\\n- Kissinger-Akahira-Sunose (KAS)\\ \n- Friedman (Fr)\\\n- Vyazovkin (Vy)\\\n- Advanced method of Vyazovkin (aVy)\\\n\n\nThe repository consist in the following directories:\n- picnik.py. Contains the package\n- examples. Contains a script (example.py) which executes some commmands of picnik in order to ilustrate the suggested procedure. And three more directories which contain data to use with example.py:\n    - Constant_E. Simulated TGA data for a process with constant activation energy.\n    - Two_Steps. Simulated TGA data for a process with two steps, each with constant activation energy.\n    - Variable_E. Simulated TGA data for a process with variable activation energy.\n\n\n### Installation\n\n`picnik` can be installed from PyPi with `pip`:\n`$ pip install picnik`\n\n\n### DataExtractioin class\n\nIt has methods to open the .csv files containing the thermogravimetric data as pandas DataFrames for the experimental data, computing and adding the conversion for the process and the conversion rate as columns in the DataFrame.\\\nThe class also has methods for creating isoconversional DataFrames of time, temperature, conversion rates (for the OFW, KAS, Fr and Vy methods) and also "advanced" DataFrames of time and temperature (for the aVy method).\\\nExample:\n\n    import picnik as pnk\n \n    files = ["HR_1.csv","HR_2.csv",...,"HR_n.csv"]\n    xtr = pnk.DataExtraction()\n    Beta, T0 = xtr.read_files(files,encoding)\n    xtr.Conversion(T0,Tf)\n    TDF,tDF,dDF,TaDF,taDF = xtr.Isoconversion(advanced=(bool))\n    \n    \nThe DataFrames are also stored as attributes of the `xtr` object \n\n\n### ActivationEnergy class\n\nThis class has methods to compute the activation energies with the DataFrames created with the `xtr` object along with its associated error. The `Fr()`,`OFW()`,`KAS()` methods return a tuple of three, two and two elements respectively. The first element of the tuples is a numpy array containing the isoconversional activation energies. The second element contains the associated error within a 95\\% confidence interval. The third element in the case of the `Fr()` method is a numpy array containing the intercept of the Friedman method. The `Vy()` and `aVy()` only return a numpy array of isoconversional activation energies, the error associated to this methods are obtained with the `Vy_error()` and `aVy_error()` methods\nExample:\n\n    ace = pnk.ActivationEnergy(Beta,\n                               T0,\n                               TDF,\n                               dDF,\n                               TaDF,\n                               taDF)\n    E_Fr, E_OFW, E_KAS, E_Vy, E_aVy = ace.Fr(), ace.OFW(), ace.KAS(), ace.Vy(), ace.aVy()\n    \nThe constructor of this class needs six arguments, a list/array/tuple of Temperature rates, a list/array of initial temperatures and four DataFrames: one of temperature, one of convertsion rates and two "advanced" one of temperature and the other of time.\n\n### Exporting results\n\nThe DataExtractionclass also has a method to export the results as .csv or .xlsx files:\n\n    xtr.export_Ea(E_Fr = (Bool), \n                  E_OFW = (Bool), \n                  E_KAS = (Bool), \n                  E_Vy = (Bool), \n                  E_aVy = (Bool),\n                  file_t="xlsx" )\n\nSet to True the method which values want to be exported. Set `file_t` to `xlsx` to export results as as an Excel spreadsheet or to `csv` to export results as a CSV file.\n\n\n\n',
     'author': 'ErickErock',
     'author_email': 'ramirez.orozco.erick@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ErickErock/pICNIK',
```

### Comparing `PICNIK-0.1.7/PKG-INFO` & `PICNIK-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picnik
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to make isoconversional computations for non-isothermal kinetics
 Home-page: https://github.com/ErickErock/pICNIK
 License: MIT
 Keywords: non-isothermal kinetics,isoconversion,isoconversional computations
 Author: ErickErock
 Author-email: ramirez.orozco.erick@gmail.com
 Requires-Python: >=3.7,<4.0
```

