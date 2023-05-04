# Comparing `tmp/py-strongly-typed-1.1.1.tar.gz` & `tmp/py-strongly-typed-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-strongly-typed-1.1.1.tar", last modified: Thu May  4 14:32:41 2023, max compression
+gzip compressed data, was "py-strongly-typed-1.1.2.tar", last modified: Thu May  4 14:48:14 2023, max compression
```

## Comparing `py-strongly-typed-1.1.1.tar` & `py-strongly-typed-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:32:41.616369 py-strongly-typed-1.1.1/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1070 2023-05-04 00:10:00.000000 py-strongly-typed-1.1.1/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)     5060 2023-05-04 14:32:41.616369 py-strongly-typed-1.1.1/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     4706 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.1/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:32:41.616369 py-strongly-typed-1.1.1/py_strongly_typed/
--rw-rw-r--   0 dev       (1000) dev       (1000)      268 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.1/py_strongly_typed/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      496 2023-05-04 04:08:39.000000 py-strongly-typed-1.1.1/py_strongly_typed/contracts.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      653 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.1/py_strongly_typed/decorators.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      317 2023-05-04 05:18:01.000000 py-strongly-typed-1.1.1/py_strongly_typed/exceptions.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1075 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.1/py_strongly_typed/typed_class.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:32:41.616369 py-strongly-typed-1.1.1/py_strongly_typed/use_cases/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-05-04 04:07:47.000000 py-strongly-typed-1.1.1/py_strongly_typed/use_cases/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3334 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.1/py_strongly_typed/use_cases/validate_annotations_use_case.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:32:41.616369 py-strongly-typed-1.1.1/py_strongly_typed.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)     5060 2023-05-04 14:32:41.000000 py-strongly-typed-1.1.1/py_strongly_typed.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      499 2023-05-04 14:32:41.000000 py-strongly-typed-1.1.1/py_strongly_typed.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-05-04 14:32:41.000000 py-strongly-typed-1.1.1/py_strongly_typed.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       45 2023-05-04 14:32:41.000000 py-strongly-typed-1.1.1/py_strongly_typed.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       18 2023-05-04 14:32:41.000000 py-strongly-typed-1.1.1/py_strongly_typed.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      121 2023-05-04 14:32:41.616369 py-strongly-typed-1.1.1/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      919 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.1/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:48:14.009960 py-strongly-typed-1.1.2/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1070 2023-05-04 00:10:00.000000 py-strongly-typed-1.1.2/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5116 2023-05-04 14:48:14.013960 py-strongly-typed-1.1.2/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4762 2023-05-04 14:46:14.000000 py-strongly-typed-1.1.2/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:48:14.009960 py-strongly-typed-1.1.2/py_strongly_typed/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      268 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.2/py_strongly_typed/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      496 2023-05-04 04:08:39.000000 py-strongly-typed-1.1.2/py_strongly_typed/contracts.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      653 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.2/py_strongly_typed/decorators.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      317 2023-05-04 05:18:01.000000 py-strongly-typed-1.1.2/py_strongly_typed/exceptions.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1075 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.2/py_strongly_typed/typed_class.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:48:14.009960 py-strongly-typed-1.1.2/py_strongly_typed/use_cases/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-05-04 04:07:47.000000 py-strongly-typed-1.1.2/py_strongly_typed/use_cases/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3334 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.2/py_strongly_typed/use_cases/validate_annotations_use_case.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:48:14.009960 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5116 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      499 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       45 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       18 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)      121 2023-05-04 14:48:14.013960 py-strongly-typed-1.1.2/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      919 2023-05-04 14:48:07.000000 py-strongly-typed-1.1.2/setup.py
```

### Comparing `py-strongly-typed-1.1.1/LICENSE` & `py-strongly-typed-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-strongly-typed-1.1.1/PKG-INFO` & `py-strongly-typed-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: py-strongly-typed
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python type enforcer
 Author: Christian Silva
 Author-email: chrislcontrol@hotmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/chrislcontrol/py-strongly-typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-![Supported Python Versions](https://img.shields.io/pypi/pyversions/py-strongly-typed)
+![Supported Python Versions](https://img.shields.io/badge/python-3.5%2B-brightgreen)
 ![pypi version](https://img.shields.io/pypi/v/py-strongly-typed)
 ![Last commit](https://img.shields.io/github/last-commit/chrislcontrol/py-strongly-typed)
 [![Downloads](https://pepy.tech/badge/py-strongly-typed/month)](https://pepy.tech/project/py-strongly-typed)
 
 What do I need?
 ===============
 - Python (3.5+)
@@ -169,8 +169,9 @@
    * Generics (example: List[str]) are not supported yet.
    * Typing using or operator will validate only first one. Example: providing str or int, 
 only str will be considered. To provide more than one expected type, use `|` operator or `Union`.
    * `*args` and `**kwargs` are not supported due to be impossible to provide typing annotations for them 
 without Generics.
 
 
-
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `py-strongly-typed-1.1.1/README.md` & `py-strongly-typed-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Supported Python Versions](https://img.shields.io/pypi/pyversions/py-strongly-typed)
+![Supported Python Versions](https://img.shields.io/badge/python-3.5%2B-brightgreen)
 ![pypi version](https://img.shields.io/pypi/v/py-strongly-typed)
 ![Last commit](https://img.shields.io/github/last-commit/chrislcontrol/py-strongly-typed)
 [![Downloads](https://pepy.tech/badge/py-strongly-typed/month)](https://pepy.tech/project/py-strongly-typed)
 
 What do I need?
 ===============
 - Python (3.5+)
@@ -156,8 +156,9 @@
    * Generics (example: List[str]) are not supported yet.
    * Typing using or operator will validate only first one. Example: providing str or int, 
 only str will be considered. To provide more than one expected type, use `|` operator or `Union`.
    * `*args` and `**kwargs` are not supported due to be impossible to provide typing annotations for them 
 without Generics.
 
 
-
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `py-strongly-typed-1.1.1/py_strongly_typed/decorators.py` & `py-strongly-typed-1.1.2/py_strongly_typed/decorators.py`

 * *Files identical despite different names*

### Comparing `py-strongly-typed-1.1.1/py_strongly_typed/typed_class.py` & `py-strongly-typed-1.1.2/py_strongly_typed/typed_class.py`

 * *Files identical despite different names*

### Comparing `py-strongly-typed-1.1.1/py_strongly_typed/use_cases/validate_annotations_use_case.py` & `py-strongly-typed-1.1.2/py_strongly_typed/use_cases/validate_annotations_use_case.py`

 * *Files identical despite different names*

### Comparing `py-strongly-typed-1.1.1/py_strongly_typed.egg-info/PKG-INFO` & `py-strongly-typed-1.1.2/py_strongly_typed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: py-strongly-typed
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python type enforcer
 Author: Christian Silva
 Author-email: chrislcontrol@hotmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/chrislcontrol/py-strongly-typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-![Supported Python Versions](https://img.shields.io/pypi/pyversions/py-strongly-typed)
+![Supported Python Versions](https://img.shields.io/badge/python-3.5%2B-brightgreen)
 ![pypi version](https://img.shields.io/pypi/v/py-strongly-typed)
 ![Last commit](https://img.shields.io/github/last-commit/chrislcontrol/py-strongly-typed)
 [![Downloads](https://pepy.tech/badge/py-strongly-typed/month)](https://pepy.tech/project/py-strongly-typed)
 
 What do I need?
 ===============
 - Python (3.5+)
@@ -169,8 +169,9 @@
    * Generics (example: List[str]) are not supported yet.
    * Typing using or operator will validate only first one. Example: providing str or int, 
 only str will be considered. To provide more than one expected type, use `|` operator or `Union`.
    * `*args` and `**kwargs` are not supported due to be impossible to provide typing annotations for them 
 without Generics.
 
 
-
+## License
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `py-strongly-typed-1.1.1/setup.py` & `py-strongly-typed-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description=long_description(),
     packages=find_packages(exclude=["*tests*"]),
     author='Christian Silva',
     author_email='chrislcontrol@hotmail.com',
     long_description_content_type='text/markdown',
     license='MIT License',
     python_requires=">=3.5",
-    version='1.1.1',
+    version='1.1.2',
     project_urls={
         "GitHub": "https://github.com/chrislcontrol/py-strongly-typed"
     },
     install_requires=[
         'wheel'
     ],
     extras_require={
```

