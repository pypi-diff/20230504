# Comparing `tmp/atsphinx-footnotes-0.1.0.tar.gz` & `tmp/atsphinx-footnotes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atsphinx-footnotes-0.1.0.tar", last modified: Thu May  4 18:32:45 2023, max compression
+gzip compressed data, was "atsphinx-footnotes-0.1.1.tar", last modified: Thu May  4 18:46:23 2023, max compression
```

## Comparing `atsphinx-footnotes-0.1.0.tar` & `atsphinx-footnotes-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      560 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/.editorconfig
--rw-r--r--   0        0        0     3338 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/.gitignore
--rw-r--r--   0        0        0      543 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      151 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/CHANGES.rst
--rw-r--r--   0        0        0     9161 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/LICENSE
--rw-r--r--   0        0        0      907 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/README.rst
--rw-r--r--   0        0        0      634 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      517 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/docs/conf.py
--rw-r--r--   0        0        0     1103 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/docs/make.bat
--rw-r--r--   0        0        0     1039 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      354 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/setup.cfg
--rw-r--r--   0        0        0      777 2023-05-04 18:32:40.786384 atsphinx-footnotes-0.1.0/src/atsphinx/footnotes.py
--rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 atsphinx-footnotes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      560 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/.editorconfig
+-rw-r--r--   0        0        0     3338 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/.gitignore
+-rw-r--r--   0        0        0      543 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      286 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/CHANGES.rst
+-rw-r--r--   0        0        0     9161 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/LICENSE
+-rw-r--r--   0        0        0      907 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/README.rst
+-rw-r--r--   0        0        0      634 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      517 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0     1103 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0      998 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/setup.cfg
+-rw-r--r--   0        0        0      777 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/src/atsphinx/footnotes.py
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 atsphinx-footnotes-0.1.1/PKG-INFO
```

### Comparing `atsphinx-footnotes-0.1.0/.editorconfig` & `atsphinx-footnotes-0.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.0/.gitignore` & `atsphinx-footnotes-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.0/.pre-commit-config.yaml` & `atsphinx-footnotes-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.0/LICENSE` & `atsphinx-footnotes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.0/README.rst` & `atsphinx-footnotes-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.0/docs/Makefile` & `atsphinx-footnotes-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.0/docs/conf.py` & `atsphinx-footnotes-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.0/docs/index.rst` & `atsphinx-footnotes-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.0/docs/make.bat` & `atsphinx-footnotes-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.0/pyproject.toml` & `atsphinx-footnotes-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "atsphinx-footnotes"
 authors = [{name = "Kazuya Takei", email = "myself@attakei.net"}]
 license = {file = "LICENSE"}
 classifiers = [
-  "Development Status :: 3 - Alpha",
-  "Development Status :: 7 - Inactive",
+  "Development Status :: 4 - Beta",
   "Framework :: Sphinx",
   "Framework :: Sphinx :: Extension",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
```

### Comparing `atsphinx-footnotes-0.1.0/src/atsphinx/footnotes.py` & `atsphinx-footnotes-0.1.1/src/atsphinx/footnotes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Powered footnotes extension for Sphinx."""
 from docutils import nodes
 from sphinx.application import Sphinx
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 def collect_footnotes(app: Sphinx, doctree: nodes.document):
     """Collect and display later all footnotes."""
     footnotes = nodes.section()
     for footnote in doctree.traverse(nodes.footnote):
         footnote.parent.remove(footnote)
```

### Comparing `atsphinx-footnotes-0.1.0/PKG-INFO` & `atsphinx-footnotes-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: atsphinx-footnotes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Powered footnotes extension for Sphinx.
 Author-email: Kazuya Takei <myself@attakei.net>
 Description-Content-Type: text/x-rst
-Classifier: Development Status :: 3 - Alpha
-Classifier: Development Status :: 7 - Inactive
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

