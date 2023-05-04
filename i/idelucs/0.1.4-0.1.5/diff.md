# Comparing `tmp/idelucs-0.1.4.tar.gz` & `tmp/idelucs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idelucs-0.1.4.tar", last modified: Thu May  4 01:19:03 2023, max compression
+gzip compressed data, was "idelucs-0.1.5.tar", last modified: Thu May  4 14:13:05 2023, max compression
```

## Comparing `idelucs-0.1.4.tar` & `idelucs-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 01:19:03.585676 idelucs-0.1.4/
--rw-rw-rw-   0        0        0     1074 2023-05-04 00:59:28.000000 idelucs-0.1.4/LICENCE.md
--rw-rw-rw-   0        0        0      608 2023-05-04 01:19:03.585676 idelucs-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-05-04 00:59:28.000000 idelucs-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 01:19:03.570052 idelucs-0.1.4/idelucs/
--rw-rw-rw-   0        0        0     3104 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/LossFunctions.py
--rw-rw-rw-   0        0        0     2584 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/PytorchUtils.py
--rw-rw-rw-   0        0        0     7524 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/ResNet.py
--rw-rw-rw-   0        0        0      355 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/__init__.py
--rw-rw-rw-   0        0        0    11548 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/__main__.py
--rw-rw-rw-   0        0        0   819037 2023-05-04 01:03:03.000000 idelucs-0.1.4/idelucs/kmers.c
--rw-rw-rw-   0        0        0     6731 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/models.py
--rw-rw-rw-   0        0        0    20627 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/utils.py
--rw-rw-rw-   0        0        0     2949 2023-05-04 00:59:31.000000 idelucs-0.1.4/idelucs/utils_GUI.py
-drwxrwxrwx   0        0        0        0 2023-05-04 01:19:03.585676 idelucs-0.1.4/idelucs.egg-info/
--rw-rw-rw-   0        0        0      608 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      105 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 01:19:03.000000 idelucs-0.1.4/idelucs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 01:19:03.585676 idelucs-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1639 2023-05-04 01:18:40.000000 idelucs-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:13:05.859603 idelucs-0.1.5/
+-rw-rw-rw-   0        0        0     1074 2023-05-04 00:59:28.000000 idelucs-0.1.5/LICENCE.md
+-rw-rw-rw-   0        0        0      261 2023-05-04 14:13:05.858601 idelucs-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-05-04 00:59:28.000000 idelucs-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 14:13:05.802602 idelucs-0.1.5/idelucs/
+-rw-rw-rw-   0        0        0     3104 2023-05-04 00:59:31.000000 idelucs-0.1.5/idelucs/LossFunctions.py
+-rw-rw-rw-   0        0        0     2584 2023-05-04 00:59:31.000000 idelucs-0.1.5/idelucs/PytorchUtils.py
+-rw-rw-rw-   0        0        0     7524 2023-05-04 00:59:31.000000 idelucs-0.1.5/idelucs/ResNet.py
+-rw-rw-rw-   0        0        0      488 2023-05-04 13:31:56.000000 idelucs-0.1.5/idelucs/__init__.py
+-rw-rw-rw-   0        0        0    11548 2023-05-04 00:59:31.000000 idelucs-0.1.5/idelucs/__main__.py
+-rw-rw-rw-   0        0        0     6108 2023-05-04 00:59:31.000000 idelucs-0.1.5/idelucs/kmers.pyx
+-rw-rw-rw-   0        0        0     6731 2023-05-04 00:59:31.000000 idelucs-0.1.5/idelucs/models.py
+-rw-rw-rw-   0        0        0    20627 2023-05-04 00:59:31.000000 idelucs-0.1.5/idelucs/utils.py
+-rw-rw-rw-   0        0        0     2949 2023-05-04 00:59:31.000000 idelucs-0.1.5/idelucs/utils_GUI.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:13:05.856602 idelucs-0.1.5/idelucs.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-05-04 14:13:05.000000 idelucs-0.1.5/idelucs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-05-04 14:13:05.000000 idelucs-0.1.5/idelucs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:13:05.000000 idelucs-0.1.5/idelucs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-04 14:13:05.000000 idelucs-0.1.5/idelucs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      152 2023-05-04 14:13:05.000000 idelucs-0.1.5/idelucs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 14:13:05.000000 idelucs-0.1.5/idelucs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1166 2023-05-04 13:39:52.000000 idelucs-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 14:13:05.859603 idelucs-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      419 2023-05-04 14:10:49.000000 idelucs-0.1.5/setup.py
```

### Comparing `idelucs-0.1.4/LICENCE.md` & `idelucs-0.1.5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.4/README.md` & `idelucs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.4/idelucs/LossFunctions.py` & `idelucs-0.1.5/idelucs/LossFunctions.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.4/idelucs/PytorchUtils.py` & `idelucs-0.1.5/idelucs/PytorchUtils.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.4/idelucs/ResNet.py` & `idelucs-0.1.5/idelucs/ResNet.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.4/idelucs/__main__.py` & `idelucs-0.1.5/idelucs/__main__.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.4/idelucs/models.py` & `idelucs-0.1.5/idelucs/models.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.4/idelucs/utils.py` & `idelucs-0.1.5/idelucs/utils.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.4/idelucs/utils_GUI.py` & `idelucs-0.1.5/idelucs/utils_GUI.py`

 * *Files identical despite different names*

