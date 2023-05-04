# Comparing `tmp/backend.ai-kernel-helper-23.3.0a4.tar.gz` & `tmp/backend.ai-kernel-helper-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-helper-23.3.0a4.tar", last modified: Thu Mar 16 02:52:59 2023, max compression
+gzip compressed data, was "backend.ai-kernel-helper-23.3.1.tar", last modified: Thu May  4 05:10:09 2023, max compression
```

## Comparing `backend.ai-kernel-helper-23.3.0a4.tar` & `backend.ai-kernel-helper-23.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.084109 backend.ai-kernel-helper-23.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:52:58.000000 backend.ai-kernel-helper-23.3.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-16 02:52:59.084109 backend.ai-kernel-helper-23.3.0a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.084109 backend.ai-kernel-helper-23.3.0a4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.084109 backend.ai-kernel-helper-23.3.0a4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.084109 backend.ai-kernel-helper-23.3.0a4/ai/backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:52:58.000000 backend.ai-kernel-helper-23.3.0a4/ai/backend/helpers/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-16 02:52:58.000000 backend.ai-kernel-helper-23.3.0a4/ai/backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-16 02:52:58.000000 backend.ai-kernel-helper-23.3.0a4/ai/backend/helpers/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:52:59.084109 backend.ai-kernel-helper-23.3.0a4/backend.ai_kernel_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-16 02:52:59.000000 backend.ai-kernel-helper-23.3.0a4/backend.ai_kernel_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-16 02:52:59.000000 backend.ai-kernel-helper-23.3.0a4/backend.ai_kernel_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:59.000000 backend.ai-kernel-helper-23.3.0a4/backend.ai_kernel_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:59.000000 backend.ai-kernel-helper-23.3.0a4/backend.ai_kernel_helper.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:52:59.000000 backend.ai-kernel-helper-23.3.0a4/backend.ai_kernel_helper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-16 02:52:59.000000 backend.ai-kernel-helper-23.3.0a4/backend.ai_kernel_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:52:59.000000 backend.ai-kernel-helper-23.3.0a4/backend.ai_kernel_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:52:58.000000 backend.ai-kernel-helper-23.3.0a4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:52:59.084109 backend.ai-kernel-helper-23.3.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-16 02:52:58.000000 backend.ai-kernel-helper-23.3.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.462789 backend.ai-kernel-helper-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 05:10:09.462789 backend.ai-kernel-helper-23.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.458789 backend.ai-kernel-helper-23.3.1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.458789 backend.ai-kernel-helper-23.3.1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.458789 backend.ai-kernel-helper-23.3.1/ai/backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/ai/backend/helpers/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/ai/backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/ai/backend/helpers/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.462789 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:09.462789 backend.ai-kernel-helper-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/setup.py
```

### Comparing `backend.ai-kernel-helper-23.3.0a4/PKG-INFO` & `backend.ai-kernel-helper-23.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
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
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI In-kernel Helper Package
```

### Comparing `backend.ai-kernel-helper-23.3.0a4/ai/backend/helpers/package.py` & `backend.ai-kernel-helper-23.3.1/ai/backend/helpers/package.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-helper-23.3.0a4/backend.ai_kernel_helper.egg-info/PKG-INFO` & `backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 23.3.0a4
+Version: 23.3.1
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
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
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI In-kernel Helper Package
```

### Comparing `backend.ai-kernel-helper-23.3.0a4/backend_shim.py` & `backend.ai-kernel-helper-23.3.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-helper-23.3.0a4/setup.py` & `backend.ai-kernel-helper-23.3.1/setup.py`

 * *Files 2% similar despite different names*

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
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI Kernel Runner Prebuilt Binaries Package',
     'install_requires': (
         'types-pkg_resources',
     ),
     'license': 'LGPLv3',
@@ -39,11 +39,11 @@
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

