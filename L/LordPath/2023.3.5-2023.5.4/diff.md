# Comparing `tmp/LordPath-2023.3.5.tar.gz` & `tmp/LordPath-2023.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LordPath-2023.3.5.tar", last modified: Sun Mar 19 09:41:25 2023, max compression
+gzip compressed data, was "LordPath-2023.5.4.tar", last modified: Thu May  4 14:22:19 2023, max compression
```

## Comparing `LordPath-2023.3.5.tar` & `LordPath-2023.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-03-19 09:41:25.907663 LordPath-2023.3.5/
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-03-19 09:41:25.903724 LordPath-2023.3.5/LordPath/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     3203 2023-03-17 16:10:53.000000 LordPath-2023.3.5/LordPath/__init__.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      617 2022-12-09 23:13:08.000000 LordPath-2023.3.5/LordPath/dataset.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      577 2023-03-19 09:38:45.000000 LordPath-2023.3.5/LordPath/descriptors.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     6385 2023-03-17 16:32:55.000000 LordPath-2023.3.5/LordPath/filefolderclass.py
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-03-19 09:41:25.907046 LordPath-2023.3.5/LordPath/opener/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1004 2023-03-17 16:42:56.000000 LordPath-2023.3.5/LordPath/opener/__init__.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      328 2023-03-17 16:42:56.000000 LordPath-2023.3.5/LordPath/opener/base.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      868 2023-03-17 16:42:56.000000 LordPath-2023.3.5/LordPath/opener/json.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      864 2023-03-17 16:42:56.000000 LordPath-2023.3.5/LordPath/opener/pickle.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      490 2023-03-17 16:42:56.000000 LordPath-2023.3.5/LordPath/opener/toml.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1019 2023-03-16 23:58:05.000000 LordPath-2023.3.5/LordPath/opener/yaml.py
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-03-19 09:41:25.904853 LordPath-2023.3.5/LordPath.egg-info/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      463 2023-03-19 09:41:25.000000 LordPath-2023.3.5/LordPath.egg-info/PKG-INFO
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      427 2023-03-19 09:41:25.000000 LordPath-2023.3.5/LordPath.egg-info/SOURCES.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)        1 2023-03-19 09:41:25.000000 LordPath-2023.3.5/LordPath.egg-info/dependency_links.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       23 2023-03-19 09:41:25.000000 LordPath-2023.3.5/LordPath.egg-info/requires.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)        9 2023-03-19 09:41:25.000000 LordPath-2023.3.5/LordPath.egg-info/top_level.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      463 2023-03-19 09:41:25.907489 LordPath-2023.3.5/PKG-INFO
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       58 2023-03-19 09:41:22.000000 LordPath-2023.3.5/README.rst
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      533 2023-03-17 16:14:48.000000 LordPath-2023.3.5/pyproject.toml
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       38 2023-03-19 09:41:25.907708 LordPath-2023.3.5/setup.cfg
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-05-04 14:22:19.190334 LordPath-2023.5.4/
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-05-04 14:22:19.186067 LordPath-2023.5.4/LordPath/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     3203 2023-03-17 16:10:53.000000 LordPath-2023.5.4/LordPath/__init__.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      617 2022-12-09 23:13:08.000000 LordPath-2023.5.4/LordPath/dataset.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      583 2023-03-21 08:46:08.000000 LordPath-2023.5.4/LordPath/descriptors.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     6385 2023-03-17 16:32:55.000000 LordPath-2023.5.4/LordPath/filefolderclass.py
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-05-04 14:22:19.189660 LordPath-2023.5.4/LordPath/opener/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1051 2023-05-04 14:21:50.000000 LordPath-2023.5.4/LordPath/opener/__init__.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      328 2023-03-17 16:42:56.000000 LordPath-2023.5.4/LordPath/opener/base.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      868 2023-03-17 16:42:56.000000 LordPath-2023.5.4/LordPath/opener/json.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      864 2023-03-17 16:42:56.000000 LordPath-2023.5.4/LordPath/opener/pickle.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      490 2023-03-17 16:42:56.000000 LordPath-2023.5.4/LordPath/opener/toml.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1019 2023-03-16 23:58:05.000000 LordPath-2023.5.4/LordPath/opener/yaml.py
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-05-04 14:22:19.187396 LordPath-2023.5.4/LordPath.egg-info/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      463 2023-05-04 14:22:19.000000 LordPath-2023.5.4/LordPath.egg-info/PKG-INFO
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      427 2023-05-04 14:22:19.000000 LordPath-2023.5.4/LordPath.egg-info/SOURCES.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)        1 2023-05-04 14:22:19.000000 LordPath-2023.5.4/LordPath.egg-info/dependency_links.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       23 2023-05-04 14:22:19.000000 LordPath-2023.5.4/LordPath.egg-info/requires.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)        9 2023-05-04 14:22:19.000000 LordPath-2023.5.4/LordPath.egg-info/top_level.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      463 2023-05-04 14:22:19.190153 LordPath-2023.5.4/PKG-INFO
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       58 2023-03-19 09:41:22.000000 LordPath-2023.5.4/README.rst
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      516 2023-05-04 14:22:14.000000 LordPath-2023.5.4/pyproject.toml
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       38 2023-05-04 14:22:19.190380 LordPath-2023.5.4/setup.cfg
```

### Comparing `LordPath-2023.3.5/LordPath/__init__.py` & `LordPath-2023.5.4/LordPath/__init__.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.3.5/LordPath/dataset.py` & `LordPath-2023.5.4/LordPath/dataset.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.3.5/LordPath/descriptors.py` & `LordPath-2023.5.4/LordPath/descriptors.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     def __set_name__(self, owner, name):
         self.public_name = name
         self.private_name = '_' + name
 
     def __get__(self, instance, owner=None):
         if instance is None:
             return self
-        value = getattr(instance, self.private_name)
+        value = getattr(instance, self.private_name, None)
         return value
 
     def __set__(self, instance, value):
         if isinstance(value, str):
             value = Path(value)
         elif isinstance(value, (int, float)):
             value = Path(str(value))
```

### Comparing `LordPath-2023.3.5/LordPath/filefolderclass.py` & `LordPath-2023.5.4/LordPath/filefolderclass.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.3.5/LordPath/opener/__init__.py` & `LordPath-2023.5.4/LordPath/opener/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from .base import Opener
 from .. import read_file, save_file
 from . import yaml, json, pickle, toml
 
 
 def get_opener(file_ending):
+    file_ending = file_ending.replace('.', '')
     for cls in Opener.__subclasses__():
         if cls.check(file_ending):
             return cls
     return None
 
 
 def open_by_type(path: Path, ending=None, default=None):
```

### Comparing `LordPath-2023.3.5/LordPath/opener/json.py` & `LordPath-2023.5.4/LordPath/opener/json.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.3.5/LordPath/opener/pickle.py` & `LordPath-2023.5.4/LordPath/opener/pickle.py`

 * *Files identical despite different names*

### Comparing `LordPath-2023.3.5/LordPath/opener/yaml.py` & `LordPath-2023.5.4/LordPath/opener/yaml.py`

 * *Files identical despite different names*

