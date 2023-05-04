# Comparing `tmp/flask_simplelogin-0.1.1.tar.gz` & `tmp/flask_simplelogin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_simplelogin-0.1.1.tar", max compression
+gzip compressed data, was "flask_simplelogin-0.1.2.tar", max compression
```

## Comparing `flask_simplelogin-0.1.1.tar` & `flask_simplelogin-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1068 2019-10-09 23:00:57.000000 flask_simplelogin-0.1.1/LICENSE
--rw-r--r--   0        0        0     1709 2021-08-25 19:17:49.140496 flask_simplelogin-0.1.1/README.md
--rw-r--r--   0        0        0    11143 2021-10-25 13:10:41.642248 flask_simplelogin-0.1.1/flask_simplelogin/__init__.py
--rw-r--r--   0        0        0     2393 2021-10-25 13:10:41.643782 flask_simplelogin-0.1.1/flask_simplelogin/templates/login.html
--rw-r--r--   0        0        0     2026 2021-10-25 13:10:41.682690 flask_simplelogin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2833 2021-10-25 13:13:14.831369 flask_simplelogin-0.1.1/setup.py
--rw-r--r--   0        0        0     3176 2021-10-25 13:13:14.831725 flask_simplelogin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2019-10-09 23:00:57.000000 flask_simplelogin-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1709 2023-05-04 16:16:30.063083 flask_simplelogin-0.1.2/README.md
+-rw-r--r--   0        0        0    11143 2023-05-04 16:16:30.085930 flask_simplelogin-0.1.2/flask_simplelogin/__init__.py
+-rw-r--r--   0        0        0     2393 2023-05-04 16:16:30.086305 flask_simplelogin-0.1.2/flask_simplelogin/templates/login.html
+-rw-r--r--   0        0        0     1898 2023-05-04 16:16:46.220336 flask_simplelogin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 flask_simplelogin-0.1.2/PKG-INFO
```

### Comparing `flask_simplelogin-0.1.1/LICENSE` & `flask_simplelogin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_simplelogin-0.1.1/README.md` & `flask_simplelogin-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_simplelogin-0.1.1/flask_simplelogin/__init__.py` & `flask_simplelogin-0.1.2/flask_simplelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_simplelogin-0.1.1/flask_simplelogin/templates/login.html` & `flask_simplelogin-0.1.2/flask_simplelogin/templates/login.html`

 * *Files identical despite different names*

### Comparing `flask_simplelogin-0.1.1/PKG-INFO` & `flask_simplelogin-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: flask-simplelogin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Flask Simple Login - Login Extension for Flask
 Home-page: https://github.com/flask-extensions/Flask-SimpleLogin
 License: MIT
 Author: Bruno Rocha
 Author-email: rochacbruno@users.noreply.github.com
 Maintainer: Eduardo Cuducos
 Maintainer-email: cuducos@users.noreply.github.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Requires-Dist: Flask (>=0.12)
-Requires-Dist: Flask-WTF (>=0.15.1,<0.16.0)
-Requires-Dist: Sphinx (>=4.1.2,<5.0.0); extra == "docs"
+Requires-Dist: Flask-WTF (>1.1)
+Requires-Dist: Sphinx (>=4.1.2,<5.0.0) ; extra == "docs"
 Requires-Dist: WTForms (>=2.1)
 Requires-Dist: click (>=8.0.1,<9.0.0)
-Requires-Dist: recommonmark (>=0.7.1,<0.8.0); extra == "docs"
-Requires-Dist: sphinx-markdown-tables (>=0.0.15,<0.0.16); extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0); extra == "docs"
+Requires-Dist: recommonmark (>=0.7.1,<0.8.0) ; extra == "docs"
+Requires-Dist: sphinx-markdown-tables (>=0.0.15,<0.0.16) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
 Project-URL: Repository, https://github.com/flask-extensions/Flask-SimpleLogin
 Description-Content-Type: text/markdown
 
 [![GitHub Actions](https://img.shields.io/github/workflow/status/flask-extensions/Flask-SimpleLogin/Tests?style=flat-square)](https://github.com/flask-extensions/Flask-SimpleLogin/actions/workflows/tests.yml)
 [![PyPI](https://img.shields.io/pypi/v/flask_simplelogin.svg?style=flat-square)](https://pypi.org/project/flask_simplelogin/)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/flask_simplelogin.svg?style=flat-square)](https://pypi.org/project/flask_simplelogin/)
 [![PyPI formats](https://img.shields.io/pypi/format/flask_simplelogin.svg?style=flat-square)](https://pypi.org/project/flask_simplelogin/)
```

