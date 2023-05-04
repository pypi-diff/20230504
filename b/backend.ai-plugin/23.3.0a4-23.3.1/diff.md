# Comparing `tmp/backend.ai-plugin-23.3.0a4.tar.gz` & `tmp/backend.ai-plugin-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-plugin-23.3.0a4.tar", last modified: Thu Mar 16 02:52:58 2023, max compression
+gzip compressed data, was "backend.ai-plugin-23.3.1.tar", last modified: Thu May  4 05:10:10 2023, max compression
```

## Comparing `backend.ai-plugin-23.3.0a4.tar` & `backend.ai-plugin-23.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.676092 backend.ai-plugin-23.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:52:57.000000 backend.ai-plugin-23.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-16 02:52:58.676092 backend.ai-plugin-23.3.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.676092 backend.ai-plugin-23.3.0a4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.676092 backend.ai-plugin-23.3.0a4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.676092 backend.ai-plugin-23.3.0a4/ai/backend/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:52:57.000000 backend.ai-plugin-23.3.0a4/ai/backend/plugin/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-16 02:52:57.000000 backend.ai-plugin-23.3.0a4/ai/backend/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-03-16 02:52:57.000000 backend.ai-plugin-23.3.0a4/ai/backend/plugin/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:52:57.000000 backend.ai-plugin-23.3.0a4/ai/backend/plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:58.676092 backend.ai-plugin-23.3.0a4/backend.ai_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-16 02:52:58.000000 backend.ai-plugin-23.3.0a4/backend.ai_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-16 02:52:58.000000 backend.ai-plugin-23.3.0a4/backend.ai_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:58.000000 backend.ai-plugin-23.3.0a4/backend.ai_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:58.000000 backend.ai-plugin-23.3.0a4/backend.ai_plugin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:58.000000 backend.ai-plugin-23.3.0a4/backend.ai_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:52:58.000000 backend.ai-plugin-23.3.0a4/backend.ai_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:52:57.000000 backend.ai-plugin-23.3.0a4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:52:58.676092 backend.ai-plugin-23.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-16 02:52:57.000000 backend.ai-plugin-23.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.038780 backend.ai-plugin-23.3.1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.038780 backend.ai-plugin-23.3.1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/ai/backend/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/ai/backend/plugin/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/ai/backend/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/ai/backend/plugin/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/ai/backend/plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/setup.py
```

### Comparing `backend.ai-plugin-23.3.0a4/PKG-INFO` & `backend.ai-plugin-23.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Plugin Subsystem
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
 
 Backend.AI Plugin Subsystem
 ===========================
```

### Comparing `backend.ai-plugin-23.3.0a4/ai/backend/plugin/entrypoint.py` & `backend.ai-plugin-23.3.1/ai/backend/plugin/entrypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,18 @@
                 # - Adding PYTHONPATH with plugin src directories in `./py` results in
                 #   *duplicate* scan results from the remaining `.egg-info` directory (pkg metadata)
                 #   and the `setup.cfg` scan results.
                 # TODO: compare the plugin versions as well? (need to remember version with entrypoints)
                 continue
             else:
                 raise RuntimeError(
-                    f"Detected a duplicate plugin entrypoint name {entrypoint.name!r} "
-                    f"from {existing_entrypoint.value} and {entrypoint.value}",
+                    (
+                        f"Detected a duplicate plugin entrypoint name {entrypoint.name!r} "
+                        f"from {existing_entrypoint.value} and {entrypoint.value}"
+                    ),
                 )
         existing_names[entrypoint.name] = entrypoint
         yield entrypoint
 
 
 def match_plugin_list(entry_path: str, plugin_list: set[str]) -> bool:
     """
```

### Comparing `backend.ai-plugin-23.3.0a4/backend.ai_plugin.egg-info/PKG-INFO` & `backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Plugin Subsystem
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
 
 Backend.AI Plugin Subsystem
 ===========================
```

### Comparing `backend.ai-plugin-23.3.0a4/backend_shim.py` & `backend.ai-plugin-23.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-23.3.0a4/setup.py` & `backend.ai-plugin-23.3.1/setup.py`

 * *Files 5% similar despite different names*

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
     'description': 'Backend.AI Plugin Subsystem',
     'install_requires': (
     ),
     'license': 'MIT',
     'long_description': """Backend.AI Plugin Subsystem
@@ -45,11 +45,11 @@
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

