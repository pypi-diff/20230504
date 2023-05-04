# Comparing `tmp/py-strongly-typed-1.1.2.tar.gz` & `tmp/py-strongly-typed-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-strongly-typed-1.1.2.tar", last modified: Thu May  4 14:48:14 2023, max compression
+gzip compressed data, was "py-strongly-typed-1.1.3.tar", last modified: Thu May  4 15:05:41 2023, max compression
```

## Comparing `py-strongly-typed-1.1.2.tar` & `py-strongly-typed-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:48:14.009960 py-strongly-typed-1.1.2/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1070 2023-05-04 00:10:00.000000 py-strongly-typed-1.1.2/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)     5116 2023-05-04 14:48:14.013960 py-strongly-typed-1.1.2/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     4762 2023-05-04 14:46:14.000000 py-strongly-typed-1.1.2/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:48:14.009960 py-strongly-typed-1.1.2/py_strongly_typed/
--rw-rw-r--   0 dev       (1000) dev       (1000)      268 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.2/py_strongly_typed/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      496 2023-05-04 04:08:39.000000 py-strongly-typed-1.1.2/py_strongly_typed/contracts.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      653 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.2/py_strongly_typed/decorators.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      317 2023-05-04 05:18:01.000000 py-strongly-typed-1.1.2/py_strongly_typed/exceptions.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1075 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.2/py_strongly_typed/typed_class.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:48:14.009960 py-strongly-typed-1.1.2/py_strongly_typed/use_cases/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-05-04 04:07:47.000000 py-strongly-typed-1.1.2/py_strongly_typed/use_cases/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     3334 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.2/py_strongly_typed/use_cases/validate_annotations_use_case.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 14:48:14.009960 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)     5116 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      499 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       45 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       18 2023-05-04 14:48:13.000000 py-strongly-typed-1.1.2/py_strongly_typed.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)      121 2023-05-04 14:48:14.013960 py-strongly-typed-1.1.2/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      919 2023-05-04 14:48:07.000000 py-strongly-typed-1.1.2/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 15:05:41.819524 py-strongly-typed-1.1.3/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1070 2023-05-04 00:10:00.000000 py-strongly-typed-1.1.3/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5129 2023-05-04 15:05:41.819524 py-strongly-typed-1.1.3/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4775 2023-05-04 15:05:32.000000 py-strongly-typed-1.1.3/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 15:05:41.819524 py-strongly-typed-1.1.3/py_strongly_typed/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      268 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.3/py_strongly_typed/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      496 2023-05-04 04:08:39.000000 py-strongly-typed-1.1.3/py_strongly_typed/contracts.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      653 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.3/py_strongly_typed/decorators.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      317 2023-05-04 05:18:01.000000 py-strongly-typed-1.1.3/py_strongly_typed/exceptions.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1075 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.3/py_strongly_typed/typed_class.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 15:05:41.819524 py-strongly-typed-1.1.3/py_strongly_typed/use_cases/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-05-04 04:07:47.000000 py-strongly-typed-1.1.3/py_strongly_typed/use_cases/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3334 2023-05-04 14:29:22.000000 py-strongly-typed-1.1.3/py_strongly_typed/use_cases/validate_annotations_use_case.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-05-04 15:05:41.819524 py-strongly-typed-1.1.3/py_strongly_typed.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     5129 2023-05-04 15:05:41.000000 py-strongly-typed-1.1.3/py_strongly_typed.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      499 2023-05-04 15:05:41.000000 py-strongly-typed-1.1.3/py_strongly_typed.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-05-04 15:05:41.000000 py-strongly-typed-1.1.3/py_strongly_typed.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       45 2023-05-04 15:05:41.000000 py-strongly-typed-1.1.3/py_strongly_typed.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       18 2023-05-04 15:05:41.000000 py-strongly-typed-1.1.3/py_strongly_typed.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)      121 2023-05-04 15:05:41.819524 py-strongly-typed-1.1.3/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      919 2023-05-04 15:00:03.000000 py-strongly-typed-1.1.3/setup.py
```

### Comparing `py-strongly-typed-1.1.2/LICENSE` & `py-strongly-typed-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-strongly-typed-1.1.2/PKG-INFO` & `py-strongly-typed-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-strongly-typed
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python type enforcer
 Author: Christian Silva
 Author-email: chrislcontrol@hotmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/chrislcontrol/py-strongly-typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -20,15 +20,15 @@
 ===============
 - Python (3.5+)
 
 
 Description
 ===========
 
-With typyd now typing annotations metters! Use this lib to validate provided args typing.
+With py-strongly-typed, now typing annotations metters! Use this lib to validate provided args typing.
 
 
 Be free to contribute with our [GitHub](https://github.com/chrislcontrol/typyd) project.
 
 
 
 Get Started
```

### Comparing `py-strongly-typed-1.1.2/README.md` & `py-strongly-typed-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ===============
 - Python (3.5+)
 
 
 Description
 ===========
 
-With typyd now typing annotations metters! Use this lib to validate provided args typing.
+With py-strongly-typed, now typing annotations metters! Use this lib to validate provided args typing.
 
 
 Be free to contribute with our [GitHub](https://github.com/chrislcontrol/typyd) project.
 
 
 
 Get Started
```

### Comparing `py-strongly-typed-1.1.2/py_strongly_typed/decorators.py` & `py-strongly-typed-1.1.3/py_strongly_typed/decorators.py`

 * *Files identical despite different names*

### Comparing `py-strongly-typed-1.1.2/py_strongly_typed/typed_class.py` & `py-strongly-typed-1.1.3/py_strongly_typed/typed_class.py`

 * *Files identical despite different names*

### Comparing `py-strongly-typed-1.1.2/py_strongly_typed/use_cases/validate_annotations_use_case.py` & `py-strongly-typed-1.1.3/py_strongly_typed/use_cases/validate_annotations_use_case.py`

 * *Files identical despite different names*

### Comparing `py-strongly-typed-1.1.2/py_strongly_typed.egg-info/PKG-INFO` & `py-strongly-typed-1.1.3/py_strongly_typed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-strongly-typed
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python type enforcer
 Author: Christian Silva
 Author-email: chrislcontrol@hotmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/chrislcontrol/py-strongly-typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -20,15 +20,15 @@
 ===============
 - Python (3.5+)
 
 
 Description
 ===========
 
-With typyd now typing annotations metters! Use this lib to validate provided args typing.
+With py-strongly-typed, now typing annotations metters! Use this lib to validate provided args typing.
 
 
 Be free to contribute with our [GitHub](https://github.com/chrislcontrol/typyd) project.
 
 
 
 Get Started
```

### Comparing `py-strongly-typed-1.1.2/setup.py` & `py-strongly-typed-1.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description=long_description(),
     packages=find_packages(exclude=["*tests*"]),
     author='Christian Silva',
     author_email='chrislcontrol@hotmail.com',
     long_description_content_type='text/markdown',
     license='MIT License',
     python_requires=">=3.5",
-    version='1.1.2',
+    version='1.1.3',
     project_urls={
         "GitHub": "https://github.com/chrislcontrol/py-strongly-typed"
     },
     install_requires=[
         'wheel'
     ],
     extras_require={
```

