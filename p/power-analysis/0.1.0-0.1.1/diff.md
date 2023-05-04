# Comparing `tmp/power_analysis-0.1.0.tar.gz` & `tmp/power_analysis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power_analysis-0.1.0.tar", max compression
+gzip compressed data, was "power_analysis-0.1.1.tar", max compression
```

## Comparing `power_analysis-0.1.0.tar` & `power_analysis-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-05-04 03:56:39.960574 power_analysis-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-05-04 03:28:48.248048 power_analysis-0.1.0/power_analysis/__init__.py
--rw-r--r--   0        0        0     3272 2023-05-04 03:35:57.988674 power_analysis-0.1.0/power_analysis/power_analysis.py
--rw-r--r--   0        0        0      411 2023-05-04 04:19:22.298661 power_analysis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2153 2023-05-04 03:43:08.397709 power_analysis-0.1.0/README.md
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 power_analysis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-04 03:56:39.960574 power_analysis-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-04 03:28:48.248048 power_analysis-0.1.1/power_analysis/__init__.py
+-rw-r--r--   0        0        0     3272 2023-05-04 03:35:57.988674 power_analysis-0.1.1/power_analysis/modules.py
+-rw-r--r--   0        0        0      411 2023-05-04 04:41:32.486209 power_analysis-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2153 2023-05-04 04:29:40.389936 power_analysis-0.1.1/README.md
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 power_analysis-0.1.1/PKG-INFO
```

### Comparing `power_analysis-0.1.0/LICENSE` & `power_analysis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.0/power_analysis/power_analysis.py` & `power_analysis-0.1.1/power_analysis/modules.py`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.0/README.md` & `power_analysis-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # power-analysis 💪🔍
 
 `power-analysis` is a Python package for performing power analysis and calculating sample sizes for statistical models. The package provides classes for defining statistical models, performing power analysis, and calculating sample sizes for two-sample t-tests.
 
 ## Installation 📥
 
-You can install the `power-analysis` package using pip:
+You can install the `power_analysis` package using pip:
 
 ```bash
 pip install power-analysis
 ```
 
 ## Usage 🧑‍💻
```

### Comparing `power_analysis-0.1.0/PKG-INFO` & `power_analysis-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-analysis
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package allows you to perform power analysis computations
 License: MIT
 Author: Rodrigo Franco
 Author-email: franc703@umn.edu
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 
 # power-analysis 💪🔍
 
 `power-analysis` is a Python package for performing power analysis and calculating sample sizes for statistical models. The package provides classes for defining statistical models, performing power analysis, and calculating sample sizes for two-sample t-tests.
 
 ## Installation 📥
 
-You can install the `power-analysis` package using pip:
+You can install the `power_analysis` package using pip:
 
 ```bash
 pip install power-analysis
 ```
 
 ## Usage 🧑‍💻
```

