# Comparing `tmp/OWR-2.6.0.tar.gz` & `tmp/OWR-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-2.6.0.tar", last modified: Thu May  4 14:10:43 2023, max compression
+gzip compressed data, was "OWR-2.6.1.tar", last modified: Thu May  4 14:18:29 2023, max compression
```

## Comparing `OWR-2.6.0.tar` & `OWR-2.6.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:10:43.617809 OWR-2.6.0/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 12:29:59.000000 OWR-2.6.0/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:10:43.617809 OWR-2.6.0/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     8319 2023-05-04 14:04:42.000000 OWR-2.6.0/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:10:43.617809 OWR-2.6.0/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-04 14:10:43.000000 OWR-2.6.0/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 14:10:43.617809 OWR-2.6.0/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-04 14:01:03.000000 OWR-2.6.0/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-04 14:10:43.617809 OWR-2.6.0/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      693 2023-05-04 14:09:49.000000 OWR-2.6.0/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:18:29.320929 OWR-2.6.1/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-04 12:29:59.000000 OWR-2.6.1/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:18:29.316929 OWR-2.6.1/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     8319 2023-05-04 14:14:15.000000 OWR-2.6.1/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:18:29.316929 OWR-2.6.1/OWR/data/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     5788 2023-05-04 14:14:15.000000 OWR-2.6.1/OWR/data/obscenity_words.json
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-04 14:18:29.316929 OWR-2.6.1/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-04 14:18:29.000000 OWR-2.6.1/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      306 2023-05-04 14:18:29.316929 OWR-2.6.1/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-04 14:14:15.000000 OWR-2.6.1/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-04 14:18:29.320929 OWR-2.6.1/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      747 2023-05-04 14:18:13.000000 OWR-2.6.1/setup.py
```

### Comparing `OWR-2.6.0/LICENSE` & `OWR-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-2.6.0/OWR/__init__.py` & `OWR-2.6.1/OWR/__init__.py`

 * *Files identical despite different names*

### Comparing `OWR-2.6.0/setup.py` & `OWR-2.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='2.6.0',
+    version='2.6.1',
     description='Obscene word recognition package',
     url='https://github.com/RuslanGaliullin/FFixTelegramBot/tree/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
+    package_data={'': ['data/obscenity_words.json']},
     include_package_data=True,
     install_requires=['scikit-learn',
                       'huggingsound',
                       'librosa',
                       'levenshtein',
                       'soundfile',
                       'fonetika',
```

