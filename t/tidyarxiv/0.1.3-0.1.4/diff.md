# Comparing `tmp/tidyarxiv-0.1.3.tar.gz` & `tmp/tidyarxiv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyarxiv-0.1.3.tar", max compression
+gzip compressed data, was "tidyarxiv-0.1.4.tar", max compression
```

## Comparing `tidyarxiv-0.1.3.tar` & `tidyarxiv-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3722 2023-05-02 23:40:53.218435 tidyarxiv-0.1.3/README.md
--rw-r--r--   0        0        0      469 2023-05-03 23:35:55.667537 tidyarxiv-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 23:35:31.688443 tidyarxiv-0.1.3/tidyarxiv/__init__.py
--rw-r--r--   0        0        0     4760 2023-05-03 23:32:04.509729 tidyarxiv-0.1.3/tidyarxiv/tidyarxiv.py
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 tidyarxiv-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3742 2023-05-03 23:39:59.316544 tidyarxiv-0.1.4/README.md
+-rw-r--r--   0        0        0      469 2023-05-03 23:40:24.293283 tidyarxiv-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 23:35:31.688443 tidyarxiv-0.1.4/tidyarxiv/__init__.py
+-rw-r--r--   0        0        0     4760 2023-05-03 23:32:04.509729 tidyarxiv-0.1.4/tidyarxiv/tidyarxiv.py
+-rw-r--r--   0        0        0     4250 1970-01-01 00:00:00.000000 tidyarxiv-0.1.4/PKG-INFO
```

### Comparing `tidyarxiv-0.1.3/README.md` & `tidyarxiv-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 A simple script to prepare your LaTeX paper for arXiv submission.
 
 # Description
 
-`arxiv` is a tiny script to run before publishing your paper on arXiv.
+`tidyarxiv` is a tiny script to run before publishing your paper on arXiv.
 
 First, you create an `.arxiv` configuration file within your project directory.
-Then you run `arxiv` on the root of your project directory.
+Then you run `tidyarxiv` on the root of your project directory.
 
-`arxiv` first copies over *only* the files you specify into a separate
+`tidyarxiv` first copies over *only* the files you specify into a separate
 temporary *staging* directory (first creating a list of all the files
 you choose to *include*, and then excluding all the files you choose
 to *exclude*, if any). It *filters* those files by removing unwanted
 TeX comments from the relevant files (typically .tex and .sty).
 
 Next, it builds your project within the staging directory to produce your
 final PDF file. Among the present files in the staging directory after
@@ -20,15 +20,15 @@
 to [arXiv](https://arxiv.org/).
 
 # Installing
 
 Install using pip:
 
 ```
-pip install arxiv
+pip install tidyarxiv
 ```
 
 # Requirements
 
 Python 3.10+
 
 # Config
@@ -70,15 +70,15 @@
   your target .tex filename. The default command is "latexmk -pdf %FILE%".
 
 # Running
 
 After installing and configuring, run in the root of your project directory:
 
 ```
-arxiv
+tidyarxiv
 ```
 
 # Features
 
 * Includes only the files you want, and excludes the files you don't want.
 * Removes LaTeX comments (anything after a "%", nothing more complex).
 * Gets rid of .bib files from the final tarball.
```

### Comparing `tidyarxiv-0.1.3/tidyarxiv/tidyarxiv.py` & `tidyarxiv-0.1.4/tidyarxiv/tidyarxiv.py`

 * *Files identical despite different names*

### Comparing `tidyarxiv-0.1.3/PKG-INFO` & `tidyarxiv-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidyarxiv
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple script to prepare your LaTeX paper for arXiv submission
 License: GPL-3.0-only
 Author: Dionysis Zindros
 Author-email: dionyziz@stanford.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -12,20 +12,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 A simple script to prepare your LaTeX paper for arXiv submission.
 
 # Description
 
-`arxiv` is a tiny script to run before publishing your paper on arXiv.
+`tidyarxiv` is a tiny script to run before publishing your paper on arXiv.
 
 First, you create an `.arxiv` configuration file within your project directory.
-Then you run `arxiv` on the root of your project directory.
+Then you run `tidyarxiv` on the root of your project directory.
 
-`arxiv` first copies over *only* the files you specify into a separate
+`tidyarxiv` first copies over *only* the files you specify into a separate
 temporary *staging* directory (first creating a list of all the files
 you choose to *include*, and then excluding all the files you choose
 to *exclude*, if any). It *filters* those files by removing unwanted
 TeX comments from the relevant files (typically .tex and .sty).
 
 Next, it builds your project within the staging directory to produce your
 final PDF file. Among the present files in the staging directory after
@@ -34,15 +34,15 @@
 to [arXiv](https://arxiv.org/).
 
 # Installing
 
 Install using pip:
 
 ```
-pip install arxiv
+pip install tidyarxiv
 ```
 
 # Requirements
 
 Python 3.10+
 
 # Config
@@ -84,15 +84,15 @@
   your target .tex filename. The default command is "latexmk -pdf %FILE%".
 
 # Running
 
 After installing and configuring, run in the root of your project directory:
 
 ```
-arxiv
+tidyarxiv
 ```
 
 # Features
 
 * Includes only the files you want, and excludes the files you don't want.
 * Removes LaTeX comments (anything after a "%", nothing more complex).
 * Gets rid of .bib files from the final tarball.
```

