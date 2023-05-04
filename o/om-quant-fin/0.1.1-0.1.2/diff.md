# Comparing `tmp/om_quant_fin-0.1.1.tar.gz` & `tmp/om_quant_fin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "om_quant_fin-0.1.1.tar", last modified: Thu May  4 19:22:31 2023, max compression
+gzip compressed data, was "om_quant_fin-0.1.2.tar", last modified: Thu May  4 19:32:23 2023, max compression
```

## Comparing `om_quant_fin-0.1.1.tar` & `om_quant_fin-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:22:31.280940 om_quant_fin-0.1.1/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2907 2023-05-04 19:22:31.280776 om_quant_fin-0.1.1/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2331 2023-05-04 19:18:48.000000 om_quant_fin-0.1.1/README.md
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:22:31.279693 om_quant_fin-0.1.1/om_quant_fin/
--rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-0.1.1/om_quant_fin/__init__.py
--rw-r--r--   0 leandroguerra   (501) staff       (20)     3999 2023-05-04 18:28:26.000000 om_quant_fin-0.1.1/om_quant_fin/om_quant_fin.py
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:22:31.280594 om_quant_fin-0.1.1/om_quant_fin.egg-info/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2907 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/SOURCES.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/dependency_links.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       35 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/requires.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/top_level.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-04 19:22:31.280994 om_quant_fin-0.1.1/setup.cfg
--rw-r--r--   0 leandroguerra   (501) staff       (20)     1066 2023-05-04 19:21:45.000000 om_quant_fin-0.1.1/setup.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:32:23.877581 om_quant_fin-0.1.2/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2967 2023-05-04 19:32:23.877429 om_quant_fin-0.1.2/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2391 2023-05-04 19:30:48.000000 om_quant_fin-0.1.2/README.md
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:32:23.876490 om_quant_fin-0.1.2/om_quant_fin/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-0.1.2/om_quant_fin/__init__.py
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     3999 2023-05-04 18:28:26.000000 om_quant_fin-0.1.2/om_quant_fin/om_quant_fin.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:32:23.877242 om_quant_fin-0.1.2/om_quant_fin.egg-info/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2967 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/SOURCES.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/dependency_links.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       35 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/requires.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-04 19:32:23.000000 om_quant_fin-0.1.2/om_quant_fin.egg-info/top_level.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-04 19:32:23.877633 om_quant_fin-0.1.2/setup.cfg
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     1066 2023-05-04 19:30:56.000000 om_quant_fin-0.1.2/setup.py
```

### Comparing `om_quant_fin-0.1.1/PKG-INFO` & `om_quant_fin-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: om_quant_fin
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple quantitative trading library for the OMNP Class
 Home-page: UNKNOWN
 Author: Outspoken Market
 Author-email: info@outspokenmarket.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -18,21 +18,21 @@
 # OM Quant lib
 
 OM Quant is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
 
 ## Project Structure
 
 ```python
-om_quant_fin/                   # Diretório raiz do projeto
-├── om_quant_fin/              # Python package
-│   ├── __init__.py         # Marca o diretório como um package
-│   └── om_quant_fin.py         # Contém as funções da sua lib
-├── setup.py                # Fornece os metadados do package bem como suas dependências
-├── .gitignore              # Lista os arquivos e pastas que não precisam ser registradas no git
-└── README.md               # Arquivo Markdown com a descrição do projeto, exemplos e outras informações
+om_quant_fin/               # Root directory of the project
+├── om_quant_fin/           # Python package containing the library's code
+│   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
+│   └── om_quant_fin.py     # Contains library's functions
+├── setup.py                # Provides package metadata and dependencies for packaging and distribution
+├── .gitignore              # Lists files and folders that should not be tracked by Git
+└── README.md               # Markdown file with a description of the project, usage instructions, and other information
 ```
 
 ## Features
 
 - Download stock data from Yahoo Finance
 - Calculate rolling Z-scores
 - Calculate rolling ratio of adjusted close and its mean
@@ -41,21 +41,22 @@
 - Run a logistic regression model
 - Evaluates the model with AUC and Gini
 
 ## Installation
 
 Install the library using pip:
 
-  pip install om_quant_fin
+```python
+pip install om_quant_fin
+```
 
 ## Usage
 
 ```python
-  import om_quant_fin as mql
-  import om_quant_fin as mql
+import om_quant_fin as mql
 
 #Download stock data:
   data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
 
 #Calculate rolling Z-score:
   z_score = mql.rolling_z_score(data["Adj Close"], window=20)
```

### Comparing `om_quant_fin-0.1.1/README.md` & `om_quant_fin-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # OM Quant lib
 
 OM Quant is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
 
 ## Project Structure
 
 ```python
-om_quant_fin/                   # Diretório raiz do projeto
-├── om_quant_fin/              # Python package
-│   ├── __init__.py         # Marca o diretório como um package
-│   └── om_quant_fin.py         # Contém as funções da sua lib
-├── setup.py                # Fornece os metadados do package bem como suas dependências
-├── .gitignore              # Lista os arquivos e pastas que não precisam ser registradas no git
-└── README.md               # Arquivo Markdown com a descrição do projeto, exemplos e outras informações
+om_quant_fin/               # Root directory of the project
+├── om_quant_fin/           # Python package containing the library's code
+│   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
+│   └── om_quant_fin.py     # Contains library's functions
+├── setup.py                # Provides package metadata and dependencies for packaging and distribution
+├── .gitignore              # Lists files and folders that should not be tracked by Git
+└── README.md               # Markdown file with a description of the project, usage instructions, and other information
 ```
 
 ## Features
 
 - Download stock data from Yahoo Finance
 - Calculate rolling Z-scores
 - Calculate rolling ratio of adjusted close and its mean
@@ -24,21 +24,22 @@
 - Run a logistic regression model
 - Evaluates the model with AUC and Gini
 
 ## Installation
 
 Install the library using pip:
 
-  pip install om_quant_fin
+```python
+pip install om_quant_fin
+```
 
 ## Usage
 
 ```python
-  import om_quant_fin as mql
-  import om_quant_fin as mql
+import om_quant_fin as mql
 
 #Download stock data:
   data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
 
 #Calculate rolling Z-score:
   z_score = mql.rolling_z_score(data["Adj Close"], window=20)
```

### Comparing `om_quant_fin-0.1.1/om_quant_fin/om_quant_fin.py` & `om_quant_fin-0.1.2/om_quant_fin/om_quant_fin.py`

 * *Files identical despite different names*

### Comparing `om_quant_fin-0.1.1/om_quant_fin.egg-info/PKG-INFO` & `om_quant_fin-0.1.2/om_quant_fin.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: om-quant-fin
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple quantitative trading library for the OMNP Class
 Home-page: UNKNOWN
 Author: Outspoken Market
 Author-email: info@outspokenmarket.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -18,21 +18,21 @@
 # OM Quant lib
 
 OM Quant is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
 
 ## Project Structure
 
 ```python
-om_quant_fin/                   # Diretório raiz do projeto
-├── om_quant_fin/              # Python package
-│   ├── __init__.py         # Marca o diretório como um package
-│   └── om_quant_fin.py         # Contém as funções da sua lib
-├── setup.py                # Fornece os metadados do package bem como suas dependências
-├── .gitignore              # Lista os arquivos e pastas que não precisam ser registradas no git
-└── README.md               # Arquivo Markdown com a descrição do projeto, exemplos e outras informações
+om_quant_fin/               # Root directory of the project
+├── om_quant_fin/           # Python package containing the library's code
+│   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
+│   └── om_quant_fin.py     # Contains library's functions
+├── setup.py                # Provides package metadata and dependencies for packaging and distribution
+├── .gitignore              # Lists files and folders that should not be tracked by Git
+└── README.md               # Markdown file with a description of the project, usage instructions, and other information
 ```
 
 ## Features
 
 - Download stock data from Yahoo Finance
 - Calculate rolling Z-scores
 - Calculate rolling ratio of adjusted close and its mean
@@ -41,21 +41,22 @@
 - Run a logistic regression model
 - Evaluates the model with AUC and Gini
 
 ## Installation
 
 Install the library using pip:
 
-  pip install om_quant_fin
+```python
+pip install om_quant_fin
+```
 
 ## Usage
 
 ```python
-  import om_quant_fin as mql
-  import om_quant_fin as mql
+import om_quant_fin as mql
 
 #Download stock data:
   data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
 
 #Calculate rolling Z-score:
   z_score = mql.rolling_z_score(data["Adj Close"], window=20)
```

### Comparing `om_quant_fin-0.1.1/setup.py` & `om_quant_fin-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name = "om_quant_fin",
-    version = "0.1.1",
+    version = "0.1.2",
     packages = find_packages(),
     install_requires = [
         "yfinance",
         "pandas",
         "scikit-learn",
         "numpy"
     ],
```

