# Comparing `tmp/gpt4pandas-0.1.tar.gz` & `tmp/gpt4pandas-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4pandas-0.1.tar", last modified: Wed May  3 21:49:44 2023, max compression
+gzip compressed data, was "gpt4pandas-0.2.tar", last modified: Wed May  3 22:04:54 2023, max compression
```

## Comparing `gpt4pandas-0.1.tar` & `gpt4pandas-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 21:49:44.112679 gpt4pandas-0.1/
--rw-rw-rw-   0        0        0    11558 2023-05-03 20:31:28.000000 gpt4pandas-0.1/LICENSE
--rw-rw-rw-   0        0        0     1364 2023-05-03 21:49:44.112679 gpt4pandas-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      992 2023-05-03 20:42:51.000000 gpt4pandas-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 21:49:44.098380 gpt4pandas-0.1/gpt4pandas/
--rw-rw-rw-   0        0        0     1554 2023-05-03 21:40:40.000000 gpt4pandas-0.1/gpt4pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 21:49:44.111680 gpt4pandas-0.1/gpt4pandas.egg-info/
--rw-rw-rw-   0        0        0     1364 2023-05-03 21:49:43.000000 gpt4pandas-0.1/gpt4pandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-03 21:49:44.000000 gpt4pandas-0.1/gpt4pandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 21:49:43.000000 gpt4pandas-0.1/gpt4pandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-03 21:49:43.000000 gpt4pandas-0.1/gpt4pandas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 21:49:43.000000 gpt4pandas-0.1/gpt4pandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 21:49:44.112679 gpt4pandas-0.1/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-05-03 20:53:28.000000 gpt4pandas-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:04:54.301727 gpt4pandas-0.2/
+-rw-rw-rw-   0        0        0    11558 2023-05-03 20:31:28.000000 gpt4pandas-0.2/LICENSE
+-rw-rw-rw-   0        0        0     5160 2023-05-03 22:04:54.301044 gpt4pandas-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4788 2023-05-03 22:04:38.000000 gpt4pandas-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 22:04:54.278483 gpt4pandas-0.2/gpt4pandas/
+-rw-rw-rw-   0        0        0     1554 2023-05-03 21:40:40.000000 gpt4pandas-0.2/gpt4pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 22:04:54.299531 gpt4pandas-0.2/gpt4pandas.egg-info/
+-rw-rw-rw-   0        0        0     5160 2023-05-03 22:04:54.000000 gpt4pandas-0.2/gpt4pandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-03 22:04:54.000000 gpt4pandas-0.2/gpt4pandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 22:04:54.000000 gpt4pandas-0.2/gpt4pandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-03 22:04:54.000000 gpt4pandas-0.2/gpt4pandas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 22:04:54.000000 gpt4pandas-0.2/gpt4pandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 22:04:54.301727 gpt4pandas-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-05-03 22:04:19.000000 gpt4pandas-0.2/setup.py
```

### Comparing `gpt4pandas-0.1/LICENSE` & `gpt4pandas-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4pandas-0.1/gpt4pandas/__init__.py` & `gpt4pandas-0.2/gpt4pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4pandas-0.1/setup.py` & `gpt4pandas-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='gpt4pandas',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     license='Apache License 2.0',
     description='A tool that uses the GPT4ALL language model and the Pandas library to answer questions about dataframes',
     author='ParisNeo (Saifeddine ALOUI)',
     author_email='aloui.seifeddine@gmail.com',
     keywords='pandas GPT4ALL QA',
     install_requires=[
```

