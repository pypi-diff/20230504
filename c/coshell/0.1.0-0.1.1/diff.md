# Comparing `tmp/coshell-0.1.0.tar.gz` & `tmp/coshell-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coshell-0.1.0.tar", max compression
+gzip compressed data, was "coshell-0.1.1.tar", max compression
```

## Comparing `coshell-0.1.0.tar` & `coshell-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2023-05-04 03:53:16.891655 coshell-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-04 00:04:14.186261 coshell-0.1.0/coshell/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 00:05:00.322229 coshell-0.1.0/coshell/internal/__init__.py
--rw-r--r--   0        0        0      166 2023-05-04 01:34:16.391315 coshell-0.1.0/coshell/internal/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2261 2023-05-04 02:32:42.728979 coshell-0.1.0/coshell/internal/__pycache__/chat.cpython-311.pyc
--rw-r--r--   0        0        0     1112 2023-05-04 03:52:50.834360 coshell-0.1.0/coshell/internal/chat.py
--rw-r--r--   0        0        0      245 2023-05-04 00:13:33.370642 coshell-0.1.0/coshell/internal/cli.py
--rw-r--r--   0        0        0        0 2023-05-04 00:32:00.012465 coshell-0.1.0/coshell/internal/openai/__init__.py
--rw-r--r--   0        0        0      173 2023-05-04 01:34:16.400835 coshell-0.1.0/coshell/internal/openai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1500 2023-05-04 01:34:16.402633 coshell-0.1.0/coshell/internal/openai/__pycache__/api.cpython-311.pyc
--rw-r--r--   0        0        0     3151 2023-05-04 02:31:58.334782 coshell-0.1.0/coshell/internal/openai/__pycache__/chat_completions.cpython-311.pyc
--rw-r--r--   0        0        0     1939 2023-05-04 01:50:30.771863 coshell-0.1.0/coshell/internal/openai/__pycache__/endpoint.cpython-311.pyc
--rw-r--r--   0        0        0      567 2023-05-04 00:56:14.917461 coshell-0.1.0/coshell/internal/openai/api.py
--rw-r--r--   0        0        0     1125 2023-05-04 03:52:50.815997 coshell-0.1.0/coshell/internal/openai/chat_completions.py
--rw-r--r--   0        0        0      685 2023-05-04 03:52:50.805789 coshell-0.1.0/coshell/internal/openai/endpoint.py
--rw-r--r--   0        0        0     1326 2023-05-04 03:52:50.824848 coshell-0.1.0/coshell/main.py
--rw-r--r--   0        0        0      397 2023-05-04 03:57:18.619886 coshell-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 coshell-0.1.0/setup.py
--rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 coshell-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-04 03:53:16.891655 coshell-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 00:04:14.186261 coshell-0.1.1/coshell/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:05:00.322229 coshell-0.1.1/coshell/internal/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-04 01:34:16.391315 coshell-0.1.1/coshell/internal/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2261 2023-05-04 02:32:42.728979 coshell-0.1.1/coshell/internal/__pycache__/chat.cpython-311.pyc
+-rw-r--r--   0        0        0     1112 2023-05-04 03:52:50.834360 coshell-0.1.1/coshell/internal/chat.py
+-rw-r--r--   0        0        0      245 2023-05-04 00:13:33.370642 coshell-0.1.1/coshell/internal/cli.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:32:00.012465 coshell-0.1.1/coshell/internal/openai/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-04 01:34:16.400835 coshell-0.1.1/coshell/internal/openai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1500 2023-05-04 01:34:16.402633 coshell-0.1.1/coshell/internal/openai/__pycache__/api.cpython-311.pyc
+-rw-r--r--   0        0        0     3151 2023-05-04 02:31:58.334782 coshell-0.1.1/coshell/internal/openai/__pycache__/chat_completions.cpython-311.pyc
+-rw-r--r--   0        0        0     1939 2023-05-04 01:50:30.771863 coshell-0.1.1/coshell/internal/openai/__pycache__/endpoint.cpython-311.pyc
+-rw-r--r--   0        0        0      567 2023-05-04 00:56:14.917461 coshell-0.1.1/coshell/internal/openai/api.py
+-rw-r--r--   0        0        0     1125 2023-05-04 03:52:50.815997 coshell-0.1.1/coshell/internal/openai/chat_completions.py
+-rw-r--r--   0        0        0      685 2023-05-04 03:52:50.805789 coshell-0.1.1/coshell/internal/openai/endpoint.py
+-rw-r--r--   0        0        0     1326 2023-05-04 03:52:50.824848 coshell-0.1.1/coshell/main.py
+-rw-r--r--   0        0        0      395 2023-05-04 04:07:25.649289 coshell-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 coshell-0.1.1/setup.py
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 coshell-0.1.1/PKG-INFO
```

### Comparing `coshell-0.1.0/coshell/internal/__pycache__/chat.cpython-311.pyc` & `coshell-0.1.1/coshell/internal/__pycache__/chat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `coshell-0.1.0/coshell/internal/chat.py` & `coshell-0.1.1/coshell/internal/chat.py`

 * *Files identical despite different names*

### Comparing `coshell-0.1.0/coshell/internal/openai/__pycache__/api.cpython-311.pyc` & `coshell-0.1.1/coshell/internal/openai/__pycache__/api.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `coshell-0.1.0/coshell/internal/openai/__pycache__/chat_completions.cpython-311.pyc` & `coshell-0.1.1/coshell/internal/openai/__pycache__/chat_completions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `coshell-0.1.0/coshell/internal/openai/__pycache__/endpoint.cpython-311.pyc` & `coshell-0.1.1/coshell/internal/openai/__pycache__/endpoint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `coshell-0.1.0/coshell/internal/openai/api.py` & `coshell-0.1.1/coshell/internal/openai/api.py`

 * *Files identical despite different names*

### Comparing `coshell-0.1.0/coshell/internal/openai/chat_completions.py` & `coshell-0.1.1/coshell/internal/openai/chat_completions.py`

 * *Files identical despite different names*

### Comparing `coshell-0.1.0/coshell/internal/openai/endpoint.py` & `coshell-0.1.1/coshell/internal/openai/endpoint.py`

 * *Files identical despite different names*

### Comparing `coshell-0.1.0/coshell/main.py` & `coshell-0.1.1/coshell/main.py`

 * *Files identical despite different names*

### Comparing `coshell-0.1.0/setup.py` & `coshell-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.7,<2', 'pyperclip>=1.8.2,<2', 'requests>=2,<3']
 
 entry_points = \
-{'console_scripts': ['my_script = coshell.main:main']}
+{'console_scripts': ['coshell = coshell.main:main']}
 
 setup_kwargs = {
     'name': 'coshell',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '',
     'author': 'Joshua Wycuff',
     'author_email': 'josh.wycuff@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `coshell-0.1.0/PKG-INFO` & `coshell-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coshell
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Joshua Wycuff
 Author-email: josh.wycuff@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

