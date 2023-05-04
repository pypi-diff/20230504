# Comparing `tmp/om_quant_fin-0.1.3.tar.gz` & `tmp/om_quant_fin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "om_quant_fin-0.1.3.tar", last modified: Thu May  4 19:37:35 2023, max compression
+gzip compressed data, was "om_quant_fin-0.1.4.tar", last modified: Thu May  4 19:59:08 2023, max compression
```

## Comparing `om_quant_fin-0.1.3.tar` & `om_quant_fin-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:37:35.702292 om_quant_fin-0.1.3/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2971 2023-05-04 19:37:35.702123 om_quant_fin-0.1.3/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2395 2023-05-04 19:36:43.000000 om_quant_fin-0.1.3/README.md
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:37:35.701180 om_quant_fin-0.1.3/om_quant_fin/
--rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-0.1.3/om_quant_fin/__init__.py
--rw-r--r--   0 leandroguerra   (501) staff       (20)     3999 2023-05-04 18:28:26.000000 om_quant_fin-0.1.3/om_quant_fin/om_quant_fin.py
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:37:35.701934 om_quant_fin-0.1.3/om_quant_fin.egg-info/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2971 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/SOURCES.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/dependency_links.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       35 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/requires.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-04 19:37:35.000000 om_quant_fin-0.1.3/om_quant_fin.egg-info/top_level.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-04 19:37:35.702352 om_quant_fin-0.1.3/setup.cfg
--rw-r--r--   0 leandroguerra   (501) staff       (20)     1066 2023-05-04 19:37:27.000000 om_quant_fin-0.1.3/setup.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:59:08.141865 om_quant_fin-0.1.4/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2588 2023-05-04 19:59:08.141684 om_quant_fin-0.1.4/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2012 2023-05-04 19:58:47.000000 om_quant_fin-0.1.4/README.md
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:59:08.140711 om_quant_fin-0.1.4/om_quant_fin/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-0.1.4/om_quant_fin/__init__.py
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     3999 2023-05-04 18:28:26.000000 om_quant_fin-0.1.4/om_quant_fin/om_quant_fin.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:59:08.141487 om_quant_fin-0.1.4/om_quant_fin.egg-info/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2588 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/SOURCES.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/dependency_links.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       35 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/requires.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/top_level.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-04 19:59:08.141924 om_quant_fin-0.1.4/setup.cfg
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     1066 2023-05-04 19:58:56.000000 om_quant_fin-0.1.4/setup.py
```

### Comparing `om_quant_fin-0.1.3/PKG-INFO` & `om_quant_fin-0.1.4/om_quant_fin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: om_quant_fin
-Version: 0.1.3
+Name: om-quant-fin
+Version: 0.1.4
 Summary: A simple quantitative trading library for the OMNP Class
 Home-page: UNKNOWN
 Author: Outspoken Market
 Author-email: info@outspokenmarket.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -73,10 +73,8 @@
   predictions = mql.run_logistic_regression(X_train, y_train, X_test)
 
 ```
 ## License
 
 This project is licensed under the MIT License.
 
-This markdown file provides an overview of your project, its structure, features, installation, and usage instructions. It's a good starting point for users who want to learn about your library and how to use it. You can also include additional information, such as code examples, detailed explanations of the functions, and any other relevant information that you'd like to share.
-
```

### Comparing `om_quant_fin-0.1.3/README.md` & `om_quant_fin-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -55,9 +55,7 @@
 #Run a logistic regression model:
   predictions = mql.run_logistic_regression(X_train, y_train, X_test)
 
 ```
 ## License
 
 This project is licensed under the MIT License.
-
-This markdown file provides an overview of your project, its structure, features, installation, and usage instructions. It's a good starting point for users who want to learn about your library and how to use it. You can also include additional information, such as code examples, detailed explanations of the functions, and any other relevant information that you'd like to share.
```

### Comparing `om_quant_fin-0.1.3/om_quant_fin/om_quant_fin.py` & `om_quant_fin-0.1.4/om_quant_fin/om_quant_fin.py`

 * *Files identical despite different names*

### Comparing `om_quant_fin-0.1.3/om_quant_fin.egg-info/PKG-INFO` & `om_quant_fin-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: om-quant-fin
-Version: 0.1.3
+Name: om_quant_fin
+Version: 0.1.4
 Summary: A simple quantitative trading library for the OMNP Class
 Home-page: UNKNOWN
 Author: Outspoken Market
 Author-email: info@outspokenmarket.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -73,10 +73,8 @@
   predictions = mql.run_logistic_regression(X_train, y_train, X_test)
 
 ```
 ## License
 
 This project is licensed under the MIT License.
 
-This markdown file provides an overview of your project, its structure, features, installation, and usage instructions. It's a good starting point for users who want to learn about your library and how to use it. You can also include additional information, such as code examples, detailed explanations of the functions, and any other relevant information that you'd like to share.
-
```

### Comparing `om_quant_fin-0.1.3/setup.py` & `om_quant_fin-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name = "om_quant_fin",
-    version = "0.1.3",
+    version = "0.1.4",
     packages = find_packages(),
     install_requires = [
         "yfinance",
         "pandas",
         "scikit-learn",
         "numpy"
     ],
```

