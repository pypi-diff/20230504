# Comparing `tmp/backend.ai-cli-23.3.0a4.tar.gz` & `tmp/backend.ai-cli-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-cli-23.3.0a4.tar", last modified: Thu Mar 16 02:52:59 2023, max compression
+gzip compressed data, was "backend.ai-cli-23.3.1.tar", last modified: Thu May  4 05:10:09 2023, max compression
```

## Comparing `backend.ai-cli-23.3.0a4.tar` & `backend.ai-cli-23.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.500127 backend.ai-cli-23.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-16 02:52:59.500127 backend.ai-cli-23.3.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.496127 backend.ai-cli-23.3.0a4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.496127 backend.ai-cli-23.3.0a4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.496127 backend.ai-cli-23.3.0a4/ai/backend/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/ai/backend/cli/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/ai/backend/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/ai/backend/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/ai/backend/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/ai/backend/cli/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/ai/backend/cli/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/ai/backend/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/ai/backend/cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/ai/backend/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.500127 backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:52:59.500127 backend.ai-cli-23.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-03-16 02:52:59.000000 backend.ai-cli-23.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/ai/backend/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/setup.py
```

### Comparing `backend.ai-cli-23.3.0a4/PKG-INFO` & `backend.ai-cli-23.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-cli
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Command Line Interface Helper
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
 
 # backend.ai-cli
 
 Unified command-line interface for Backend.AI
```

### Comparing `backend.ai-cli-23.3.0a4/ai/backend/cli/extensions.py` & `backend.ai-cli-23.3.1/ai/backend/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.0a4/ai/backend/cli/interaction.py` & `backend.ai-cli-23.3.1/ai/backend/cli/interaction.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.0a4/ai/backend/cli/loader.py` & `backend.ai-cli-23.3.1/ai/backend/cli/loader.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.0a4/ai/backend/cli/main.py` & `backend.ai-cli-23.3.1/ai/backend/cli/main.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/PKG-INFO` & `backend.ai-cli-23.3.1/backend.ai_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-cli
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Command Line Interface Helper
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
 
 # backend.ai-cli
 
 Unified command-line interface for Backend.AI
```

### Comparing `backend.ai-cli-23.3.0a4/backend.ai_cli.egg-info/SOURCES.txt` & `backend.ai-cli-23.3.1/backend.ai_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.0a4/backend_shim.py` & `backend.ai-cli-23.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.0a4/setup.py` & `backend.ai-cli-23.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
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
     'description': 'Backend.AI Command Line Interface Helper',
     'entry_points': {
         'console_scripts': [
             'backend.ai = ai.backend.cli.__main__:main',
         ],
     },
     'install_requires': (
         'attrs>=20.3',
-        """backend.ai-plugin==23.03.0a4
+        """backend.ai-plugin==23.03.1
 """,
         'click>=7.1.2',
     ),
     'license': 'MIT',
     'long_description': """# backend.ai-cli
 
 Unified command-line interface for Backend.AI
@@ -70,11 +70,11 @@
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

