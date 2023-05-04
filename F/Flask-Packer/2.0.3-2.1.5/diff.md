# Comparing `tmp/Flask Packer-2.0.3.tar.gz` & `tmp/Flask Packer-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask Packer-2.0.3.tar", last modified: Thu May  4 12:25:04 2023, max compression
+gzip compressed data, was "Flask Packer-2.1.5.tar", last modified: Thu May  4 13:14:12 2023, max compression
```

## Comparing `Flask Packer-2.0.3.tar` & `Flask Packer-2.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 stan       (501) staff       (20)        0 2023-05-04 12:25:04.002912 Flask Packer-2.0.3/
-drwxr-xr-x   0 stan       (501) staff       (20)        0 2023-05-04 12:25:04.001226 Flask Packer-2.0.3/Flask_Packer.egg-info/
--rw-r--r--   0 stan       (501) staff       (20)      726 2023-05-04 12:25:03.000000 Flask Packer-2.0.3/Flask_Packer.egg-info/PKG-INFO
--rw-r--r--   0 stan       (501) staff       (20)      382 2023-05-04 12:25:03.000000 Flask Packer-2.0.3/Flask_Packer.egg-info/SOURCES.txt
--rw-r--r--   0 stan       (501) staff       (20)        1 2023-05-04 12:25:03.000000 Flask Packer-2.0.3/Flask_Packer.egg-info/dependency_links.txt
--rw-r--r--   0 stan       (501) staff       (20)       63 2023-05-04 12:25:03.000000 Flask Packer-2.0.3/Flask_Packer.egg-info/requires.txt
--rw-r--r--   0 stan       (501) staff       (20)       13 2023-05-04 12:25:03.000000 Flask Packer-2.0.3/Flask_Packer.egg-info/top_level.txt
--rw-r--r--   0 stan       (501) staff       (20)    35149 2023-05-02 19:07:11.000000 Flask Packer-2.0.3/LICENSE
--rw-r--r--   0 stan       (501) staff       (20)      726 2023-05-04 12:25:04.002987 Flask Packer-2.0.3/PKG-INFO
-drwxr-xr-x   0 stan       (501) staff       (20)        0 2023-05-04 12:25:04.002060 Flask Packer-2.0.3/flask_packer/
--rw-r--r--   0 stan       (501) staff       (20)       73 2023-05-04 12:23:48.000000 Flask Packer-2.0.3/flask_packer/__init__.py
--rw-r--r--   0 stan       (501) staff       (20)     1021 2023-05-04 12:23:48.000000 Flask Packer-2.0.3/flask_packer/_base.py
--rw-r--r--   0 stan       (501) staff       (20)      415 2023-05-04 12:23:48.000000 Flask Packer-2.0.3/flask_packer/_errors.py
--rw-r--r--   0 stan       (501) staff       (20)     6279 2023-05-04 12:23:48.000000 Flask Packer-2.0.3/flask_packer/_extension.py
-drwxr-xr-x   0 stan       (501) staff       (20)        0 2023-05-04 12:25:04.002726 Flask Packer-2.0.3/flask_packer/tags/
--rw-r--r--   0 stan       (501) staff       (20)       67 2023-05-04 12:03:22.000000 Flask Packer-2.0.3/flask_packer/tags/__init__.py
--rw-r--r--   0 stan       (501) staff       (20)     1093 2023-05-04 10:51:33.000000 Flask Packer-2.0.3/flask_packer/tags/css.py
--rw-r--r--   0 stan       (501) staff       (20)      659 2023-05-04 10:51:33.000000 Flask Packer-2.0.3/flask_packer/tags/js.py
--rw-r--r--   0 stan       (501) staff       (20)      130 2023-05-04 12:25:04.003224 Flask Packer-2.0.3/setup.cfg
--rw-r--r--   0 stan       (501) staff       (20)     1053 2023-05-04 12:24:46.000000 Flask Packer-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/Flask_Packer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 13:14:11.000000 Flask Packer-2.1.5/Flask_Packer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/flask_packer/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/flask_packer/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/tags/css.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/flask_packer/tags/js.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 13:14:12.015387 Flask Packer-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-04 13:13:57.000000 Flask Packer-2.1.5/setup.py
```

### Comparing `Flask Packer-2.0.3/Flask_Packer.egg-info/PKG-INFO` & `Flask Packer-2.1.5/Flask_Packer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Flask-Packer
-Version: 2.0.3
+Version: 2.1.5
 Summary: A Flask extension to bundle and compress CSS and JS files.
-Home-page: https://github.com/stan5079/flask-pack
+Home-page: https://github.com/stan5079/flask-packer
 Author: H.P. Mertens
 Author-email: stnmertens@gmail.com
 License: GNU General Public License v3.0
 Keywords: flask,packer,static,compress,bundle,minify,combine
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```

### Comparing `Flask Packer-2.0.3/LICENSE` & `Flask Packer-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask Packer-2.0.3/PKG-INFO` & `Flask Packer-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Flask Packer
-Version: 2.0.3
+Version: 2.1.5
 Summary: A Flask extension to bundle and compress CSS and JS files.
-Home-page: https://github.com/stan5079/flask-pack
+Home-page: https://github.com/stan5079/flask-packer
 Author: H.P. Mertens
 Author-email: stnmertens@gmail.com
 License: GNU General Public License v3.0
 Keywords: flask,packer,static,compress,bundle,minify,combine
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```

### Comparing `Flask Packer-2.0.3/flask_packer/_base.py` & `Flask Packer-2.1.5/flask_packer/_base.py`

 * *Files identical despite different names*

### Comparing `Flask Packer-2.0.3/flask_packer/_extension.py` & `Flask Packer-2.1.5/flask_packer/_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from flask import Flask, Blueprint
 from jinja2.ext import Extension
 from jinja2.nodes import CallBlock, Const
 from jinja2.parser import Parser
 from jinja2.runtime import Macro
 
 from flask_packer._errors import FileTypeUnsupported, FileNotFound
-from flask_packer.tags.css import CssTag
-from flask_packer.tags.js import JsTag
+from flask_packer.tags import CssTag, JsTag
 
 
 class Config(dict):
     def __init__(self, **kwargs) -> None:
         super().__init__()
         self.update(**kwargs)
```

### Comparing `Flask Packer-2.0.3/flask_packer/tags/css.py` & `Flask Packer-2.1.5/flask_packer/tags/css.py`

 * *Files identical despite different names*

### Comparing `Flask Packer-2.0.3/flask_packer/tags/js.py` & `Flask Packer-2.1.5/flask_packer/tags/js.py`

 * *Files identical despite different names*

### Comparing `Flask Packer-2.0.3/setup.py` & `Flask Packer-2.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,10 +23,10 @@
     description="A Flask extension to bundle and compress CSS and JS files.",
     install_requires=find_requirements(),
     keywords=["flask", "packer", "static", "compress", "bundle", "minify", "combine"],
     license="GNU General Public License v3.0",
     name="Flask Packer",
     packages=find_packages(),
     python_requires=">=3.10",
-    url="https://github.com/stan5079/flask-pack",
+    url="https://github.com/stan5079/flask-packer",
     version=__version__,
 )
```

