# Comparing `tmp/SalesforceMinu-0.0.2.tar.gz` & `tmp/SalesforceMinu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalesforceMinu-0.0.2.tar", last modified: Tue Apr 25 20:15:38 2023, max compression
+gzip compressed data, was "SalesforceMinu-0.0.3.tar", last modified: Thu May  4 16:44:44 2023, max compression
```

## Comparing `SalesforceMinu-0.0.2.tar` & `SalesforceMinu-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 20:15:38.332517 SalesforceMinu-0.0.2/
--rw-rw-rw-   0        0        0      419 2023-04-25 20:15:38.331518 SalesforceMinu-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-04-25 17:20:16.000000 SalesforceMinu-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 20:15:38.316676 SalesforceMinu-0.0.2/SalesforceMinu/
--rw-rw-rw-   0        0        0     4100 2023-04-25 19:40:31.000000 SalesforceMinu-0.0.2/SalesforceMinu/Funciones.py
--rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.2/SalesforceMinu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 20:15:38.330520 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 20:15:38.332517 SalesforceMinu-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-04-25 20:14:24.000000 SalesforceMinu-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:44:44.165763 SalesforceMinu-0.0.3/
+-rw-rw-rw-   0        0        0      419 2023-05-04 16:44:44.165763 SalesforceMinu-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-04-25 17:20:16.000000 SalesforceMinu-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 16:44:44.142089 SalesforceMinu-0.0.3/SalesforceMinu/
+-rw-rw-rw-   0        0        0     4120 2023-05-04 16:39:03.000000 SalesforceMinu-0.0.3/SalesforceMinu/Funciones.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.3/SalesforceMinu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:44:44.164768 SalesforceMinu-0.0.3/SalesforceMinu.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-04 16:44:43.000000 SalesforceMinu-0.0.3/SalesforceMinu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-04 16:44:44.000000 SalesforceMinu-0.0.3/SalesforceMinu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:44:43.000000 SalesforceMinu-0.0.3/SalesforceMinu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 16:44:43.000000 SalesforceMinu-0.0.3/SalesforceMinu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 16:44:43.000000 SalesforceMinu-0.0.3/SalesforceMinu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:44:44.165763 SalesforceMinu-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-05-04 16:41:06.000000 SalesforceMinu-0.0.3/setup.py
```

### Comparing `SalesforceMinu-0.0.2/SalesforceMinu/Funciones.py` & `SalesforceMinu-0.0.3/SalesforceMinu/Funciones.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # OBTENEMOS IDs DEL DATAFRAME
 def get_dataframe_ids(df, nam_or, title = 'id'):
     ids_df = []
     for i in range(len(nam_or)):
-        data = df[df['name'] == nam_or[i]][title]
+        data = df[df['name'].str.lower() == nam_or[i].lower()][title]
         ids_df.append(data[data.index[0]])
     return ids_df
 
 # OBTENER NOMBRES DE UN DATAFRAME
 def get_names_list(df, title = 'name'):
     if len(df[title]) == 1:
         names = df[title].get(1)
```

### Comparing `SalesforceMinu-0.0.2/setup.py` & `SalesforceMinu-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 PACKAGE_NAME = 'SalesforceMinu' 
 AUTHOR = 'Corchado Ramos Itzae Balam' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'g7_corc18@ens.cnyn.unam.mx' 
 URL = 'https://github.com/BalamCor?tab=repositories' 
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para extraer datos de minu en salesforce'
```

