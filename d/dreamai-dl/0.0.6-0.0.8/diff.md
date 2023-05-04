# Comparing `tmp/dreamai_dl-0.0.6.tar.gz` & `tmp/dreamai_dl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_dl-0.0.6.tar", last modified: Thu May  4 00:29:08 2023, max compression
+gzip compressed data, was "dreamai_dl-0.0.8.tar", last modified: Thu May  4 03:16:01 2023, max compression
```

## Comparing `dreamai_dl-0.0.6.tar` & `dreamai_dl-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_dl-0.0.6/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_dl-0.0.6/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      136 2023-05-02 16:23:03.000000 dreamai_dl-0.0.6/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/dreamai_dl/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-04 00:28:51.000000 dreamai_dl-0.0.6/dreamai_dl/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      708 2023-05-04 00:28:51.000000 dreamai_dl-0.0.6/dreamai_dl/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      165 2023-05-04 00:28:51.000000 dreamai_dl-0.0.6/dreamai_dl/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      690 2023-05-02 21:02:32.000000 dreamai_dl-0.0.6/dreamai_dl/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      724 2023-05-04 00:28:51.000000 dreamai_dl-0.0.6/dreamai_dl/utils.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/dreamai_dl.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      396 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       42 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 22:18:59.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2185 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       11 2023-05-04 00:29:08.000000 dreamai_dl-0.0.6/dreamai_dl.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2864 2023-05-04 00:27:32.000000 dreamai_dl-0.0.6/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-04 00:29:08.727478 dreamai_dl-0.0.6/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_dl-0.0.6/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_dl-0.0.8/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_dl-0.0.8/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      136 2023-05-02 16:23:03.000000 dreamai_dl-0.0.8/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/dreamai_dl/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-04 03:15:50.000000 dreamai_dl-0.0.8/dreamai_dl/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      708 2023-05-04 03:15:50.000000 dreamai_dl-0.0.8/dreamai_dl/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      165 2023-05-04 03:15:50.000000 dreamai_dl-0.0.8/dreamai_dl/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      690 2023-05-02 21:02:32.000000 dreamai_dl-0.0.8/dreamai_dl/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      724 2023-05-04 03:15:50.000000 dreamai_dl-0.0.8/dreamai_dl/utils.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/dreamai_dl.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      919 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      396 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       42 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 22:18:59.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       79 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       11 2023-05-04 03:16:01.000000 dreamai_dl-0.0.8/dreamai_dl.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      758 2023-05-04 03:04:21.000000 dreamai_dl-0.0.8/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-04 03:16:01.903475 dreamai_dl-0.0.8/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_dl-0.0.8/setup.py
```

### Comparing `dreamai_dl-0.0.6/LICENSE` & `dreamai_dl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.6/PKG-INFO` & `dreamai_dl-0.0.8/dreamai_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dreamai_dl
-Version: 0.0.6
+Name: dreamai-dl
+Version: 0.0.8
 Summary: Deep Learning tools based on dreamai.
 Home-page: https://github.com/HamzaFarhan/dreamai_dl
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_dl-0.0.6/dreamai_dl/_modidx.py` & `dreamai_dl-0.0.8/dreamai_dl/_modidx.py`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.6/dreamai_dl/imports.py` & `dreamai_dl-0.0.8/dreamai_dl/imports.py`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.6/dreamai_dl/utils.py` & `dreamai_dl-0.0.8/dreamai_dl/utils.py`

 * *Files identical despite different names*

### Comparing `dreamai_dl-0.0.6/dreamai_dl.egg-info/PKG-INFO` & `dreamai_dl-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dreamai-dl
-Version: 0.0.6
+Name: dreamai_dl
+Version: 0.0.8
 Summary: Deep Learning tools based on dreamai.
 Home-page: https://github.com/HamzaFarhan/dreamai_dl
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_dl-0.0.6/setup.py` & `dreamai_dl-0.0.8/setup.py`

 * *Files identical despite different names*

