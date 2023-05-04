# Comparing `tmp/XStatic-1.0.2.tar.gz` & `tmp/XStatic-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/XStatic-1.0.2.tar", last modified: Tue Sep 18 17:49:46 2018, max compression
+gzip compressed data, was "XStatic-1.0.3.tar", last modified: Thu May  4 10:45:26 2023, max compression
```

## Comparing `XStatic-1.0.2.tar` & `XStatic-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 tw        (1000) tw        (1000)        0 2018-09-18 17:49:46.000000 XStatic-1.0.2/
--rw-r--r--   0 tw        (1000) tw        (1000)     1569 2018-09-18 17:49:46.000000 XStatic-1.0.2/PKG-INFO
-drwxr-xr-x   0 tw        (1000) tw        (1000)        0 2018-09-18 17:49:46.000000 XStatic-1.0.2/xstatic/
-drwxr-xr-x   0 tw        (1000) tw        (1000)        0 2018-09-18 17:49:46.000000 XStatic-1.0.2/xstatic/pkg/
--rw-r--r--   0 tw        (1000) tw        (1000)      186 2018-09-18 15:32:15.000000 XStatic-1.0.2/xstatic/pkg/__init__.py
--rw-r--r--   0 tw        (1000) tw        (1000)      186 2018-09-18 15:31:57.000000 XStatic-1.0.2/xstatic/__init__.py
--rw-r--r--   0 tw        (1000) tw        (1000)     1796 2018-09-18 15:32:05.000000 XStatic-1.0.2/xstatic/main.py
-drwxr-xr-x   0 tw        (1000) tw        (1000)        0 2018-09-18 17:49:46.000000 XStatic-1.0.2/XStatic.egg-info/
--rw-r--r--   0 tw        (1000) tw        (1000)        1 2018-09-18 17:49:46.000000 XStatic-1.0.2/XStatic.egg-info/dependency_links.txt
--rw-r--r--   0 tw        (1000) tw        (1000)        8 2018-09-18 17:49:46.000000 XStatic-1.0.2/XStatic.egg-info/top_level.txt
--rw-r--r--   0 tw        (1000) tw        (1000)     1569 2018-09-18 17:49:46.000000 XStatic-1.0.2/XStatic.egg-info/PKG-INFO
--rw-r--r--   0 tw        (1000) tw        (1000)       20 2018-09-18 17:49:46.000000 XStatic-1.0.2/XStatic.egg-info/namespace_packages.txt
--rw-r--r--   0 tw        (1000) tw        (1000)      285 2018-09-18 17:49:46.000000 XStatic-1.0.2/XStatic.egg-info/SOURCES.txt
--rw-r--r--   0 tw        (1000) tw        (1000)        1 2018-09-18 17:35:32.000000 XStatic-1.0.2/XStatic.egg-info/not-zip-safe
--rw-r--r--   0 tw        (1000) tw        (1000)       38 2018-09-18 17:49:46.000000 XStatic-1.0.2/setup.cfg
--rw-r--r--   0 tw        (1000) tw        (1000)      587 2018-09-18 17:38:39.000000 XStatic-1.0.2/README.txt
--rw-r--r--   0 tw        (1000) tw        (1000)     1533 2018-09-18 17:33:42.000000 XStatic-1.0.2/setup.py
--rw-r--r--   0 tw        (1000) tw        (1000)      106 2018-09-18 15:19:16.000000 XStatic-1.0.2/MANIFEST.in
+drwxrwxr-x   0 sheep     (1000) sheep     (1000)        0 2023-05-04 10:45:26.215066 XStatic-1.0.3/
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)      255 2023-05-04 10:38:26.000000 XStatic-1.0.3/AUTHORS.txt
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)     1157 2023-05-04 10:38:26.000000 XStatic-1.0.3/LICENSE.txt
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)      175 2023-05-04 10:38:26.000000 XStatic-1.0.3/MANIFEST.in
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)     1406 2023-05-04 10:45:26.215066 XStatic-1.0.3/PKG-INFO
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)      587 2023-05-04 10:38:26.000000 XStatic-1.0.3/README.txt
+drwxrwxr-x   0 sheep     (1000) sheep     (1000)        0 2023-05-04 10:45:26.215066 XStatic-1.0.3/XStatic.egg-info/
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)     1406 2023-05-04 10:45:26.000000 XStatic-1.0.3/XStatic.egg-info/PKG-INFO
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)      425 2023-05-04 10:45:26.000000 XStatic-1.0.3/XStatic.egg-info/SOURCES.txt
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)        1 2023-05-04 10:45:26.000000 XStatic-1.0.3/XStatic.egg-info/dependency_links.txt
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)       20 2023-05-04 10:45:26.000000 XStatic-1.0.3/XStatic.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)        1 2023-05-04 10:41:52.000000 XStatic-1.0.3/XStatic.egg-info/not-zip-safe
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)        8 2023-05-04 10:45:26.000000 XStatic-1.0.3/XStatic.egg-info/top_level.txt
+drwxrwxr-x   0 sheep     (1000) sheep     (1000)        0 2023-05-04 10:45:26.215066 XStatic-1.0.3/docs/
+drwxrwxr-x   0 sheep     (1000) sheep     (1000)        0 2023-05-04 10:45:26.215066 XStatic-1.0.3/docs/source/
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)      332 2023-05-04 10:38:26.000000 XStatic-1.0.3/docs/source/index.rst
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)     2601 2023-05-04 10:38:26.000000 XStatic-1.0.3/docs/source/intro.rst
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)       98 2023-05-04 10:38:26.000000 XStatic-1.0.3/docs/source/license.rst
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)     6055 2023-05-04 10:38:26.000000 XStatic-1.0.3/docs/source/packaging.rst
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)     2164 2023-05-04 10:38:26.000000 XStatic-1.0.3/docs/source/using.rst
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)       38 2023-05-04 10:45:26.215066 XStatic-1.0.3/setup.cfg
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)     1554 2023-05-04 10:38:54.000000 XStatic-1.0.3/setup.py
+drwxrwxr-x   0 sheep     (1000) sheep     (1000)        0 2023-05-04 10:45:26.215066 XStatic-1.0.3/xstatic/
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)      186 2023-05-04 10:38:26.000000 XStatic-1.0.3/xstatic/__init__.py
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)     1796 2023-05-04 10:38:26.000000 XStatic-1.0.3/xstatic/main.py
+drwxrwxr-x   0 sheep     (1000) sheep     (1000)        0 2023-05-04 10:45:26.215066 XStatic-1.0.3/xstatic/pkg/
+-rw-rw-r--   0 sheep     (1000) sheep     (1000)      186 2023-05-04 10:38:26.000000 XStatic-1.0.3/xstatic/pkg/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `XStatic-1.0.2/PKG-INFO` & `XStatic-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: XStatic
-Version: 1.0.2
+Version: 1.0.3
 Summary: XStatic base package with minimal support code
 Home-page: https://github.com/xstatic-py/xstatic
 Author: Thomas Waldmann
 Author-email: tw@waldmann-edv.de
 License: MIT license
-Description: XStatic
-        -------
-        
-        The goal of XStatic family of packages is to provide static file packages
-        with minimal overhead - without selling you some dependencies you don't want.
-        
-        XStatic has some minimal support code for working with the XStatic-* packages.
-        
-        Docs: https://xstatic.readthedocs.io/
-        
-        Repository: https://github.com/xstatic-py/xstatic (base package)
-        
-        Find more stuff already packaged as xstatic package there:
-        
-        https://github.com/xstatic-py/
-        
-        https://pypi.org/search/?q=xstatic
-        
-        Licenses:
-        
-        * MIT license (for XStatic code)
-        * same license as packaged file (for static file packages)
-        
-        
 Keywords: xstatic static file resource python packages setuptools pypi require
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Software Distribution
+License-File: LICENSE.txt
+License-File: AUTHORS.txt
+
+XStatic
+-------
+
+The goal of XStatic family of packages is to provide static file packages
+with minimal overhead - without selling you some dependencies you don't want.
+
+XStatic has some minimal support code for working with the XStatic-* packages.
+
+Docs: https://xstatic.readthedocs.io/
+
+Repository: https://github.com/xstatic-py/xstatic (base package)
+
+Find more stuff already packaged as xstatic package there:
+
+https://github.com/xstatic-py/
+
+https://pypi.org/search/?q=xstatic
+
+Licenses:
+
+* MIT license (for XStatic code)
+* same license as packaged file (for static file packages)
+
```

### Comparing `XStatic-1.0.2/xstatic/main.py` & `XStatic-1.0.3/xstatic/main.py`

 * *Files identical despite different names*

### Comparing `XStatic-1.0.2/XStatic.egg-info/PKG-INFO` & `XStatic-1.0.3/XStatic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: XStatic
-Version: 1.0.2
+Version: 1.0.3
 Summary: XStatic base package with minimal support code
 Home-page: https://github.com/xstatic-py/xstatic
 Author: Thomas Waldmann
 Author-email: tw@waldmann-edv.de
 License: MIT license
-Description: XStatic
-        -------
-        
-        The goal of XStatic family of packages is to provide static file packages
-        with minimal overhead - without selling you some dependencies you don't want.
-        
-        XStatic has some minimal support code for working with the XStatic-* packages.
-        
-        Docs: https://xstatic.readthedocs.io/
-        
-        Repository: https://github.com/xstatic-py/xstatic (base package)
-        
-        Find more stuff already packaged as xstatic package there:
-        
-        https://github.com/xstatic-py/
-        
-        https://pypi.org/search/?q=xstatic
-        
-        Licenses:
-        
-        * MIT license (for XStatic code)
-        * same license as packaged file (for static file packages)
-        
-        
 Keywords: xstatic static file resource python packages setuptools pypi require
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Software Distribution
+License-File: LICENSE.txt
+License-File: AUTHORS.txt
+
+XStatic
+-------
+
+The goal of XStatic family of packages is to provide static file packages
+with minimal overhead - without selling you some dependencies you don't want.
+
+XStatic has some minimal support code for working with the XStatic-* packages.
+
+Docs: https://xstatic.readthedocs.io/
+
+Repository: https://github.com/xstatic-py/xstatic (base package)
+
+Find more stuff already packaged as xstatic package there:
+
+https://github.com/xstatic-py/
+
+https://pypi.org/search/?q=xstatic
+
+Licenses:
+
+* MIT license (for XStatic code)
+* same license as packaged file (for static file packages)
+
```

### Comparing `XStatic-1.0.2/README.txt` & `XStatic-1.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `XStatic-1.0.2/setup.py` & `XStatic-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 """
 XStatic - setup.py
 """
 
 import os
 
 from setuptools import setup, find_packages
+import pkg_resources
 
 # The README.txt file should be written in reST so that PyPI can use
 # it to generate your project's PyPI page. 
 readme_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'README.txt')
 
 with open(readme_path) as f:
     long_description = f.read()
 
 
 setup(
     name='XStatic',
-    version='1.0.2',
+    version='1.0.3',
     description='XStatic base package with minimal support code',
     long_description=long_description,
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
```

