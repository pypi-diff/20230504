# Comparing `tmp/backend.ai-test-23.3.0a4.tar.gz` & `tmp/backend.ai-test-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-test-23.3.0a4.tar", last modified: Thu Mar 16 02:52:58 2023, max compression
+gzip compressed data, was "backend.ai-test-23.3.1.tar", last modified: Thu May  4 05:10:09 2023, max compression
```

## Comparing `backend.ai-test-23.3.0a4.tar` & `backend.ai-test-23.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.688093 backend.ai-test-23.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-16 02:52:58.688093 backend.ai-test-23.3.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.684093 backend.ai-test-23.3.0a4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.684093 backend.ai-test-23.3.0a4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.684093 backend.ai-test-23.3.0a4/ai/backend/test/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/ai/backend/test/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/ai/backend/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.684093 backend.ai-test-23.3.0a4/ai/backend/test/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/ai/backend/test/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/ai/backend/test/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/ai/backend/test/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/ai/backend/test/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/ai/backend/test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.688093 backend.ai-test-23.3.0a4/backend.ai_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-16 02:52:58.000000 backend.ai-test-23.3.0a4/backend.ai_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-16 02:52:58.000000 backend.ai-test-23.3.0a4/backend.ai_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:58.000000 backend.ai-test-23.3.0a4/backend.ai_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-16 02:52:58.000000 backend.ai-test-23.3.0a4/backend.ai_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:58.000000 backend.ai-test-23.3.0a4/backend.ai_test.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:58.000000 backend.ai-test-23.3.0a4/backend.ai_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-16 02:52:58.000000 backend.ai-test-23.3.0a4/backend.ai_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:52:58.000000 backend.ai-test-23.3.0a4/backend.ai_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:52:58.688093 backend.ai-test-23.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-16 02:52:57.000000 backend.ai-test-23.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/ai/backend/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/ai/backend/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/backend.ai_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/setup.py
```

### Comparing `backend.ai-test-23.3.0a4/PKG-INFO` & `backend.ai-test-23.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI Testing Toolkit
 
 Automated test suites to validate an installation and integration of clients and servers
```

### Comparing `backend.ai-test-23.3.0a4/ai/backend/test/cli/__main__.py` & `backend.ai-test-23.3.1/ai/backend/test/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.0a4/ai/backend/test/cli/utils.py` & `backend.ai-test-23.3.1/ai/backend/test/cli/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.0a4/backend.ai_test.egg-info/PKG-INFO` & `backend.ai-test-23.3.1/backend.ai_test.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI Testing Toolkit
 
 Automated test suites to validate an installation and integration of clients and servers
```

### Comparing `backend.ai-test-23.3.0a4/backend.ai_test.egg-info/SOURCES.txt` & `backend.ai-test-23.3.1/backend.ai_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.0a4/backend_shim.py` & `backend.ai-test-23.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.0a4/setup.py` & `backend.ai-test-23.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
     ],
     'description': 'Backend.AI Integration Test Suite',
     'entry_points': {
         'backendai_cli_v10': [
             'test = ai.backend.test.cli.__main__:main',
         ],
@@ -63,11 +63,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.0a4
+    'version': """23.03.1
 """,
     'zip_safe': False,
 })
```

