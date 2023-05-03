# Comparing `tmp/dreamai_pdf-0.0.6.tar.gz` & `tmp/dreamai_pdf-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_pdf-0.0.6.tar", last modified: Wed May  3 19:30:23 2023, max compression
+gzip compressed data, was "dreamai_pdf-0.0.7.tar", last modified: Wed May  3 23:24:13 2023, max compression
```

## Comparing `dreamai_pdf-0.0.6.tar` & `dreamai_pdf-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.6/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.6/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.6/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/dreamai_pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     5569 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.6/dreamai_pdf/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/parse.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2285 2023-05-03 19:29:50.000000 dreamai_pdf-0.0.6/dreamai_pdf/segment.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1683 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-03 19:30:23.000000 dreamai_pdf-0.0.6/dreamai_pdf.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2368 2023-05-03 19:29:46.000000 dreamai_pdf-0.0.6/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-03 19:30:23.711759 dreamai_pdf-0.0.6/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.6/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.7/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.7/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      138 2023-05-02 22:37:14.000000 dreamai_pdf-0.0.7/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/dreamai_pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     5569 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3434 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      494 2023-05-02 20:33:15.000000 dreamai_pdf-0.0.7/dreamai_pdf/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     9207 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/parse.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2285 2023-05-03 21:14:31.000000 dreamai_pdf-0.0.7/dreamai_pdf/segment.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      927 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      431 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-04-28 14:00:17.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2951 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-03 23:24:13.000000 dreamai_pdf-0.0.7/dreamai_pdf.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3636 2023-05-03 21:12:49.000000 dreamai_pdf-0.0.7/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-03 23:24:13.956343 dreamai_pdf-0.0.7/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.0.7/setup.py
```

### Comparing `dreamai_pdf-0.0.6/LICENSE` & `dreamai_pdf-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.6/PKG-INFO` & `dreamai_pdf-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_pdf
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.6/dreamai_pdf/_modidx.py` & `dreamai_pdf-0.0.7/dreamai_pdf/_modidx.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.6/dreamai_pdf/core.py` & `dreamai_pdf-0.0.7/dreamai_pdf/core.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.6/dreamai_pdf/parse.py` & `dreamai_pdf-0.0.7/dreamai_pdf/parse.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.6/dreamai_pdf/segment.py` & `dreamai_pdf-0.0.7/dreamai_pdf/segment.py`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.0.6/dreamai_pdf.egg-info/PKG-INFO` & `dreamai_pdf-0.0.7/dreamai_pdf.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-pdf
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library based on dreamai for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.0.6/setup.py` & `dreamai_pdf-0.0.7/setup.py`

 * *Files identical despite different names*

