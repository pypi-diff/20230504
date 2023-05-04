# Comparing `tmp/om_quant_fin-0.1.2.tar.gz` & `tmp/om_quant_fin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "om_quant_fin-0.1.2.tar", last modified: Thu May  4 19:32:23 2023, max compression
+gzip compressed data, was "om_quant_fin-0.1.3.tar", last modified: Thu May  4 19:37:35 2023, max compression
```

## Comparing `om_quant_fin-0.1.2.tar` & `om_quant_fin-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:32:23.877581 om_quant_fin-0.1.2/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2967 2023-05-04 19:32:23.877429 om_quant_fin-0.1.2/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2391 2023-05-04 19:30:48.000000 om_quant_fin-0.1.2/README.md
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:32:23.876490 om_quant_fin-0.1.2/om_quant_fin/
--rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-0.1.2/om_quant_fin/__init__.py
--rw-r--r--   0 leandroguerra   (501) staff       (20)     3999 2023-05-04 18:28:26.000000 om_quant_fin-0.1.2/om_quant_fin/om_quant_fin.py
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:32:23.877242 om_quant_fin-0.1.2/om_quant_fin.egg-info/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2967 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/SOURCES.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/dependency_links.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       35 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/requires.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/top_level.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-04 19:32:23.877633 om_quant_fin-0.1.2/setup.cfg
--rw-r--r--   0 leandroguerra   (501) staff       (20)     1066 2023-05-04 19:30:56.000000 om_quant_fin-0.1.2/setup.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:37:35.702292 om_quant_fin-0.1.3/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2971 2023-05-04 19:37:35.702123 om_quant_fin-0.1.3/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2395 2023-05-04 19:36:43.000000 om_quant_fin-0.1.3/README.md
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:37:35.701180 om_quant_fin-0.1.3/om_quant_fin/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-0.1.3/om_quant_fin/__init__.py
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     3999 2023-05-04 18:28:26.000000 om_quant_fin-0.1.3/om_quant_fin/om_quant_fin.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:37:35.701934 om_quant_fin-0.1.3/om_quant_fin.egg-info/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2971 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/SOURCES.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/dependency_links.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       35 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/requires.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/top_level.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-04 19:37:35.702352 om_quant_fin-0.1.3/setup.cfg
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     1066 2023-05-04 19:37:27.000000 om_quant_fin-0.1.3/setup.py
```

### Comparing `om_quant_fin-0.1.2/PKG-INFO` & `om_quant_fin-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: om_quant_fin
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple quantitative trading library for the OMNP Class
 Home-page: UNKNOWN
 Author: Outspoken Market
 Author-email: info@outspokenmarket.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
-# OM Quant lib
+# OM Quant Fin
 
-OM Quant is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
+OM Quant Fin is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
 
 ## Project Structure
 
 ```python
 om_quant_fin/               # Root directory of the project
 ├── om_quant_fin/           # Python package containing the library's code
 │   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
```

### Comparing `om_quant_fin-0.1.2/README.md` & `om_quant_fin-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# OM Quant lib
+# OM Quant Fin
 
-OM Quant is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
+OM Quant Fin is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
 
 ## Project Structure
 
 ```python
 om_quant_fin/               # Root directory of the project
 ├── om_quant_fin/           # Python package containing the library's code
 │   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
```

### Comparing `om_quant_fin-0.1.2/om_quant_fin/om_quant_fin.py` & `om_quant_fin-0.1.3/om_quant_fin/om_quant_fin.py`

 * *Files identical despite different names*

### Comparing `om_quant_fin-0.1.2/om_quant_fin.egg-info/PKG-INFO` & `om_quant_fin-0.1.3/om_quant_fin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: om-quant-fin
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple quantitative trading library for the OMNP Class
 Home-page: UNKNOWN
 Author: Outspoken Market
 Author-email: info@outspokenmarket.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
-# OM Quant lib
+# OM Quant Fin
 
-OM Quant is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
+OM Quant Fin is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
 
 ## Project Structure
 
 ```python
 om_quant_fin/               # Root directory of the project
 ├── om_quant_fin/           # Python package containing the library's code
 │   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
```

### Comparing `om_quant_fin-0.1.2/setup.py` & `om_quant_fin-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name = "om_quant_fin",
-    version = "0.1.2",
+    version = "0.1.3",
     packages = find_packages(),
     install_requires = [
         "yfinance",
         "pandas",
         "scikit-learn",
         "numpy"
     ],
```

