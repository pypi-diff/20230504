# Comparing `tmp/tidyarxiv-0.1.2.tar.gz` & `tmp/tidyarxiv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyarxiv-0.1.2.tar", max compression
+gzip compressed data, was "tidyarxiv-0.1.3.tar", max compression
```

## Comparing `tidyarxiv-0.1.2.tar` & `tidyarxiv-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     3722 2023-05-02 23:40:53.218435 tidyarxiv-0.1.2/README.md
--rw-r--r--   0        0        0      469 2023-05-03 23:33:58.672503 tidyarxiv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4760 2023-05-03 23:32:04.509729 tidyarxiv-0.1.2/tidyarxiv/tidyarxiv.py
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 tidyarxiv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3722 2023-05-02 23:40:53.218435 tidyarxiv-0.1.3/README.md
+-rw-r--r--   0        0        0      469 2023-05-03 23:35:55.667537 tidyarxiv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 23:35:31.688443 tidyarxiv-0.1.3/tidyarxiv/__init__.py
+-rw-r--r--   0        0        0     4760 2023-05-03 23:32:04.509729 tidyarxiv-0.1.3/tidyarxiv/tidyarxiv.py
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 tidyarxiv-0.1.3/PKG-INFO
```

### Comparing `tidyarxiv-0.1.2/README.md` & `tidyarxiv-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tidyarxiv-0.1.2/tidyarxiv/tidyarxiv.py` & `tidyarxiv-0.1.3/tidyarxiv/tidyarxiv.py`

 * *Files identical despite different names*

### Comparing `tidyarxiv-0.1.2/PKG-INFO` & `tidyarxiv-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidyarxiv
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple script to prepare your LaTeX paper for arXiv submission
 License: GPL-3.0-only
 Author: Dionysis Zindros
 Author-email: dionyziz@stanford.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

