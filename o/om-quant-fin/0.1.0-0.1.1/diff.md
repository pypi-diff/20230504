# Comparing `tmp/om_quant_fin-0.1.0.tar.gz` & `tmp/om_quant_fin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "om_quant_fin-0.1.0.tar", last modified: Thu May  4 19:15:08 2023, max compression
+gzip compressed data, was "om_quant_fin-0.1.1.tar", last modified: Thu May  4 19:22:31 2023, max compression
```

## Comparing `om_quant_fin-0.1.0.tar` & `om_quant_fin-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:15:08.383796 om_quant_fin-0.1.0/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2811 2023-05-04 19:15:08.383633 om_quant_fin-0.1.0/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2235 2023-05-04 19:11:42.000000 om_quant_fin-0.1.0/README.md
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:15:08.382656 om_quant_fin-0.1.0/om_quant_fin/
--rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-0.1.0/om_quant_fin/__init__.py
--rw-r--r--   0 leandroguerra   (501) staff       (20)     3999 2023-05-04 18:28:26.000000 om_quant_fin-0.1.0/om_quant_fin/om_quant_fin.py
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:15:08.383430 om_quant_fin-0.1.0/om_quant_fin.egg-info/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2811 2023-05-04 19:15:08.000000 om_quant_fin-0.1.0/om_quant_fin.egg-info/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-04 19:15:08.000000 om_quant_fin-0.1.0/om_quant_fin.egg-info/SOURCES.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-04 19:15:08.000000 om_quant_fin-0.1.0/om_quant_fin.egg-info/dependency_links.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       35 2023-05-04 19:15:08.000000 om_quant_fin-0.1.0/om_quant_fin.egg-info/requires.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-04 19:15:08.000000 om_quant_fin-0.1.0/om_quant_fin.egg-info/top_level.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-04 19:15:08.383863 om_quant_fin-0.1.0/setup.cfg
--rw-r--r--   0 leandroguerra   (501) staff       (20)     1066 2023-05-04 19:12:00.000000 om_quant_fin-0.1.0/setup.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:22:31.280940 om_quant_fin-0.1.1/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2907 2023-05-04 19:22:31.280776 om_quant_fin-0.1.1/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2331 2023-05-04 19:18:48.000000 om_quant_fin-0.1.1/README.md
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:22:31.279693 om_quant_fin-0.1.1/om_quant_fin/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-0.1.1/om_quant_fin/__init__.py
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     3999 2023-05-04 18:28:26.000000 om_quant_fin-0.1.1/om_quant_fin/om_quant_fin.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:22:31.280594 om_quant_fin-0.1.1/om_quant_fin.egg-info/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     2907 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/SOURCES.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/dependency_links.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       35 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/requires.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-04 19:22:31.000000 om_quant_fin-0.1.1/om_quant_fin.egg-info/top_level.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-04 19:22:31.280994 om_quant_fin-0.1.1/setup.cfg
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     1066 2023-05-04 19:21:45.000000 om_quant_fin-0.1.1/setup.py
```

### Comparing `om_quant_fin-0.1.0/PKG-INFO` & `om_quant_fin-0.1.1/om_quant_fin.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 Metadata-Version: 2.1
-Name: om_quant_fin
-Version: 0.1.0
+Name: om-quant-fin
+Version: 0.1.1
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
 
-# OM Quant Lib
+# OM Quant lib
 
-OM Quant Lib is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
+OM Quant is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
 
 ## Project Structure
 
-om_quant/                   # Diretório raiz do projeto
-├── om_quant /              # Python package
+```python
+om_quant_fin/                   # Diretório raiz do projeto
+├── om_quant_fin/              # Python package
 │   ├── __init__.py         # Marca o diretório como um package
-│   └── om_quant.py         # Contém as funções da sua lib
+│   └── om_quant_fin.py         # Contém as funções da sua lib
 ├── setup.py                # Fornece os metadados do package bem como suas dependências
 ├── .gitignore              # Lista os arquivos e pastas que não precisam ser registradas no git
 └── README.md               # Arquivo Markdown com a descrição do projeto, exemplos e outras informações
-
+```
 
 ## Features
 
 - Download stock data from Yahoo Finance
 - Calculate rolling Z-scores
 - Calculate rolling ratio of adjusted close and its mean
 - Calculate returns
 - Split data into training and test sets
 - Run a logistic regression model
+- Evaluates the model with AUC and Gini
 
 ## Installation
 
 Install the library using pip:
 
-pip install om_quant
+  pip install om_quant_fin
 
 ## Usage
 
-import my_quant_lib as mql
-import my_quant_lib as mql
+```python
+  import om_quant_fin as mql
+  import om_quant_fin as mql
 
 #Download stock data:
-data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
+  data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
 
 #Calculate rolling Z-score:
-z_score = mql.rolling_z_score(data["Adj Close"], window=20)
+  z_score = mql.rolling_z_score(data["Adj Close"], window=20)
 
 #Calculate rolling ratio:
-ratio = mql.rolling_ratio(data["Adj Close"], window=20)
+  ratio = mql.rolling_ratio(data["Adj Close"], window=20)
 
 #Calculate returns:
-returns = mql.calculate_returns(data["Adj Close"])
+  returns = mql.calculate_returns(data["Adj Close"])
 
 #Split data into training and test sets:
-train, test = mql.split_data(data, "2020-01-01", "2021-12-31", "2022-01-01", "2022-12-31")
+  train, test = mql.split_data(data, "2020-01-01", "2021-12-31", "2022-01-01", "2022-12-31")
 
 #Run a logistic regression model:
-predictions = mql.run_logistic_regression(X_train, y_train, X_test)
+  predictions = mql.run_logistic_regression(X_train, y_train, X_test)
 
+```
 ## License
 
 This project is licensed under the MIT License.
 
 This markdown file provides an overview of your project, its structure, features, installation, and usage instructions. It's a good starting point for users who want to learn about your library and how to use it. You can also include additional information, such as code examples, detailed explanations of the functions, and any other relevant information that you'd like to share.
```

### Comparing `om_quant_fin-0.1.0/README.md` & `om_quant_fin-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-# OM Quant Lib
+# OM Quant lib
 
-OM Quant Lib is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
+OM Quant is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
 
 ## Project Structure
 
-om_quant/                   # Diretório raiz do projeto
-├── om_quant /              # Python package
+```python
+om_quant_fin/                   # Diretório raiz do projeto
+├── om_quant_fin/              # Python package
 │   ├── __init__.py         # Marca o diretório como um package
-│   └── om_quant.py         # Contém as funções da sua lib
+│   └── om_quant_fin.py         # Contém as funções da sua lib
 ├── setup.py                # Fornece os metadados do package bem como suas dependências
 ├── .gitignore              # Lista os arquivos e pastas que não precisam ser registradas no git
 └── README.md               # Arquivo Markdown com a descrição do projeto, exemplos e outras informações
-
+```
 
 ## Features
 
 - Download stock data from Yahoo Finance
 - Calculate rolling Z-scores
 - Calculate rolling ratio of adjusted close and its mean
 - Calculate returns
 - Split data into training and test sets
 - Run a logistic regression model
+- Evaluates the model with AUC and Gini
 
 ## Installation
 
 Install the library using pip:
 
-pip install om_quant
+  pip install om_quant_fin
 
 ## Usage
 
-import my_quant_lib as mql
-import my_quant_lib as mql
+```python
+  import om_quant_fin as mql
+  import om_quant_fin as mql
 
 #Download stock data:
-data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
+  data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
 
 #Calculate rolling Z-score:
-z_score = mql.rolling_z_score(data["Adj Close"], window=20)
+  z_score = mql.rolling_z_score(data["Adj Close"], window=20)
 
 #Calculate rolling ratio:
-ratio = mql.rolling_ratio(data["Adj Close"], window=20)
+  ratio = mql.rolling_ratio(data["Adj Close"], window=20)
 
 #Calculate returns:
-returns = mql.calculate_returns(data["Adj Close"])
+  returns = mql.calculate_returns(data["Adj Close"])
 
 #Split data into training and test sets:
-train, test = mql.split_data(data, "2020-01-01", "2021-12-31", "2022-01-01", "2022-12-31")
+  train, test = mql.split_data(data, "2020-01-01", "2021-12-31", "2022-01-01", "2022-12-31")
 
 #Run a logistic regression model:
-predictions = mql.run_logistic_regression(X_train, y_train, X_test)
+  predictions = mql.run_logistic_regression(X_train, y_train, X_test)
 
+```
 ## License
 
 This project is licensed under the MIT License.
 
 This markdown file provides an overview of your project, its structure, features, installation, and usage instructions. It's a good starting point for users who want to learn about your library and how to use it. You can also include additional information, such as code examples, detailed explanations of the functions, and any other relevant information that you'd like to share.
```

### Comparing `om_quant_fin-0.1.0/om_quant_fin/om_quant_fin.py` & `om_quant_fin-0.1.1/om_quant_fin/om_quant_fin.py`

 * *Files identical despite different names*

### Comparing `om_quant_fin-0.1.0/om_quant_fin.egg-info/PKG-INFO` & `om_quant_fin-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 Metadata-Version: 2.1
-Name: om-quant-fin
-Version: 0.1.0
+Name: om_quant_fin
+Version: 0.1.1
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
 
-# OM Quant Lib
+# OM Quant lib
 
-OM Quant Lib is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
+OM Quant is a simple Python library for quantitative trading analysis. It provides functionality for downloading stock data, calculating various indicators, and running a logistic regression model with AUC and Gini metrics for model evaluation.
 
 ## Project Structure
 
-om_quant/                   # Diretório raiz do projeto
-├── om_quant /              # Python package
+```python
+om_quant_fin/                   # Diretório raiz do projeto
+├── om_quant_fin/              # Python package
 │   ├── __init__.py         # Marca o diretório como um package
-│   └── om_quant.py         # Contém as funções da sua lib
+│   └── om_quant_fin.py         # Contém as funções da sua lib
 ├── setup.py                # Fornece os metadados do package bem como suas dependências
 ├── .gitignore              # Lista os arquivos e pastas que não precisam ser registradas no git
 └── README.md               # Arquivo Markdown com a descrição do projeto, exemplos e outras informações
-
+```
 
 ## Features
 
 - Download stock data from Yahoo Finance
 - Calculate rolling Z-scores
 - Calculate rolling ratio of adjusted close and its mean
 - Calculate returns
 - Split data into training and test sets
 - Run a logistic regression model
+- Evaluates the model with AUC and Gini
 
 ## Installation
 
 Install the library using pip:
 
-pip install om_quant
+  pip install om_quant_fin
 
 ## Usage
 
-import my_quant_lib as mql
-import my_quant_lib as mql
+```python
+  import om_quant_fin as mql
+  import om_quant_fin as mql
 
 #Download stock data:
-data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
+  data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
 
 #Calculate rolling Z-score:
-z_score = mql.rolling_z_score(data["Adj Close"], window=20)
+  z_score = mql.rolling_z_score(data["Adj Close"], window=20)
 
 #Calculate rolling ratio:
-ratio = mql.rolling_ratio(data["Adj Close"], window=20)
+  ratio = mql.rolling_ratio(data["Adj Close"], window=20)
 
 #Calculate returns:
-returns = mql.calculate_returns(data["Adj Close"])
+  returns = mql.calculate_returns(data["Adj Close"])
 
 #Split data into training and test sets:
-train, test = mql.split_data(data, "2020-01-01", "2021-12-31", "2022-01-01", "2022-12-31")
+  train, test = mql.split_data(data, "2020-01-01", "2021-12-31", "2022-01-01", "2022-12-31")
 
 #Run a logistic regression model:
-predictions = mql.run_logistic_regression(X_train, y_train, X_test)
+  predictions = mql.run_logistic_regression(X_train, y_train, X_test)
 
+```
 ## License
 
 This project is licensed under the MIT License.
 
 This markdown file provides an overview of your project, its structure, features, installation, and usage instructions. It's a good starting point for users who want to learn about your library and how to use it. You can also include additional information, such as code examples, detailed explanations of the functions, and any other relevant information that you'd like to share.
```

### Comparing `om_quant_fin-0.1.0/setup.py` & `om_quant_fin-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name = "om_quant_fin",
-    version = "0.1.0",
+    version = "0.1.1",
     packages = find_packages(),
     install_requires = [
         "yfinance",
         "pandas",
         "scikit-learn",
         "numpy"
     ],
```

