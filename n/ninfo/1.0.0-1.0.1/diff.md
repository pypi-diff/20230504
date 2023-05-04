# Comparing `tmp/ninfo-1.0.0.tar.gz` & `tmp/ninfo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninfo-1.0.0.tar", last modified: Thu May  4 18:15:25 2023, max compression
+gzip compressed data, was "ninfo-1.0.1.tar", last modified: Thu May  4 18:54:53 2023, max compression
```

## Comparing `ninfo-1.0.0.tar` & `ninfo-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.206552 ninfo-1.0.0/
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1084 2023-01-31 15:07:15.000000 ninfo-1.0.0/LICENSE
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       32 2023-01-31 15:07:15.000000 ninfo-1.0.0/MANIFEST.in
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     5538 2023-05-04 18:15:25.206552 ninfo-1.0.0/PKG-INFO
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     4925 2023-01-31 15:07:15.000000 ninfo-1.0.0/README.md
-drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.202552 ninfo-1.0.0/ninfo/
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)    14652 2023-05-04 18:03:17.000000 ninfo-1.0.0/ninfo/__init__.py
-drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.206552 ninfo-1.0.0/ninfo/helpers/
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        0 2023-01-31 15:07:15.000000 ninfo-1.0.0/ninfo/helpers/__init__.py
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1869 2023-01-31 15:07:15.000000 ninfo-1.0.0/ninfo/helpers/splunk.py
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     3686 2023-01-31 15:22:07.000000 ninfo-1.0.0/ninfo/util.py
-drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.206552 ninfo-1.0.0/ninfo.egg-info/
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     5538 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/PKG-INFO
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      398 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/SOURCES.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        1 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/dependency_links.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       37 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/entry_points.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        1 2023-01-31 15:09:13.000000 ninfo-1.0.0/ninfo.egg-info/not-zip-safe
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      120 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/requires.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        6 2023-05-04 18:15:25.000000 ninfo-1.0.0/ninfo.egg-info/top_level.txt
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1350 2023-05-04 18:03:17.000000 ninfo-1.0.0/pyproject.toml
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       38 2023-05-04 18:15:25.206552 ninfo-1.0.0/setup.cfg
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      523 2023-05-04 18:03:17.000000 ninfo-1.0.0/setup.py
-drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:15:25.206552 ninfo-1.0.0/tests/
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      841 2023-01-31 15:07:15.000000 ninfo-1.0.0/tests/test_clone.py
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1515 2023-01-31 15:07:15.000000 ninfo-1.0.0/tests/test_ninfo.py
--rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     2724 2023-01-31 15:07:15.000000 ninfo-1.0.0/tests/test_util.py
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:54:53.320525 ninfo-1.0.1/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1084 2023-01-31 15:07:15.000000 ninfo-1.0.1/LICENSE
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       32 2023-01-31 15:07:15.000000 ninfo-1.0.1/MANIFEST.in
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     5538 2023-05-04 18:54:53.320525 ninfo-1.0.1/PKG-INFO
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     4925 2023-01-31 15:07:15.000000 ninfo-1.0.1/README.md
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:54:53.316525 ninfo-1.0.1/ninfo/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)    14673 2023-05-04 18:53:58.000000 ninfo-1.0.1/ninfo/__init__.py
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:54:53.320525 ninfo-1.0.1/ninfo/helpers/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        0 2023-01-31 15:07:15.000000 ninfo-1.0.1/ninfo/helpers/__init__.py
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1869 2023-01-31 15:07:15.000000 ninfo-1.0.1/ninfo/helpers/splunk.py
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     3686 2023-01-31 15:22:07.000000 ninfo-1.0.1/ninfo/util.py
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:54:53.320525 ninfo-1.0.1/ninfo.egg-info/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     5538 2023-05-04 18:54:53.000000 ninfo-1.0.1/ninfo.egg-info/PKG-INFO
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      398 2023-05-04 18:54:53.000000 ninfo-1.0.1/ninfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        1 2023-05-04 18:54:53.000000 ninfo-1.0.1/ninfo.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       37 2023-05-04 18:54:53.000000 ninfo-1.0.1/ninfo.egg-info/entry_points.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        1 2023-01-31 15:09:13.000000 ninfo-1.0.1/ninfo.egg-info/not-zip-safe
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      120 2023-05-04 18:54:53.000000 ninfo-1.0.1/ninfo.egg-info/requires.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)        6 2023-05-04 18:54:53.000000 ninfo-1.0.1/ninfo.egg-info/top_level.txt
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1350 2023-05-04 18:53:58.000000 ninfo-1.0.1/pyproject.toml
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)       38 2023-05-04 18:54:53.320525 ninfo-1.0.1/setup.cfg
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      523 2023-05-04 18:53:58.000000 ninfo-1.0.1/setup.py
+drwxrwxr-x   0 rgoggin  (353944) rgoggin  (353944)        0 2023-05-04 18:54:53.320525 ninfo-1.0.1/tests/
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)      841 2023-01-31 15:07:15.000000 ninfo-1.0.1/tests/test_clone.py
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     1515 2023-01-31 15:07:15.000000 ninfo-1.0.1/tests/test_ninfo.py
+-rw-rw-r--   0 rgoggin  (353944) rgoggin  (353944)     2724 2023-01-31 15:07:15.000000 ninfo-1.0.1/tests/test_util.py
```

### Comparing `ninfo-1.0.0/LICENSE` & `ninfo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ninfo-1.0.0/PKG-INFO` & `ninfo-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninfo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Plugin based information gathering library
 Author-email: Justin Azoff <justin.azoff@gmail.com>, Ryan Goggin <support@ryangoggin.net>
 Project-URL: Homepage, https://github.com/ninfo-py/ninfo
 Keywords: ninfo,search
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ninfo-1.0.0/README.md` & `ninfo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ninfo-1.0.0/ninfo/__init__.py` & `ninfo-1.0.1/ninfo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pkg_resources import iter_entry_points
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 import memcache
 import logging
 
 logger = logging.getLogger("ninfo")
 
 import os
@@ -422,15 +422,15 @@
             context_options[ctxt_name] = ctxt_value
         else:
             args.append(arg)
 
     plugins = options.plugins or None
     json_output = []
     for arg in args:
-        if len(args) != 1:
+        if len(args) != 1 and not options.json:
             print("=== %s === " % (arg,))
         if options.json:
             json_output.append({"arg": arg, "data": p.get_info_dict(arg, plugins=plugins, options=context_options)})
         else:
             p.show_info(arg, plugins=plugins, options=context_options)
 
     if options.json:
```

### Comparing `ninfo-1.0.0/ninfo/helpers/splunk.py` & `ninfo-1.0.1/ninfo/helpers/splunk.py`

 * *Files identical despite different names*

### Comparing `ninfo-1.0.0/ninfo/util.py` & `ninfo-1.0.1/ninfo/util.py`

 * *Files identical despite different names*

### Comparing `ninfo-1.0.0/ninfo.egg-info/PKG-INFO` & `ninfo-1.0.1/ninfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninfo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Plugin based information gathering library
 Author-email: Justin Azoff <justin.azoff@gmail.com>, Ryan Goggin <support@ryangoggin.net>
 Project-URL: Homepage, https://github.com/ninfo-py/ninfo
 Keywords: ninfo,search
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ninfo-1.0.0/pyproject.toml` & `ninfo-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ninfo"
-version = "1.0.0"
+version = "1.0.1"
 description = "Plugin based information gathering library"
 readme = "README.md"
 authors = [{ name = "Justin Azoff", email = "justin.azoff@gmail.com" }, { name = "Ryan Goggin", email = "support@ryangoggin.net" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -31,15 +31,15 @@
 [project.urls]
 Homepage = "https://github.com/ninfo-py/ninfo"
 
 [project.scripts]
 ninfo = "ninfo:main"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `ninfo-1.0.0/setup.py` & `ninfo-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='ninfo',
-    version='1.0.0',
+    version='1.0.1',
     zip_safe=False,
     description="Plugin based information gathering library",
     packages = find_packages(exclude=["tests"]),
     include_package_data=True,
     install_requires=[
         "Mako",
         "python-memcached",
```

### Comparing `ninfo-1.0.0/tests/test_clone.py` & `ninfo-1.0.1/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `ninfo-1.0.0/tests/test_ninfo.py` & `ninfo-1.0.1/tests/test_ninfo.py`

 * *Files identical despite different names*

### Comparing `ninfo-1.0.0/tests/test_util.py` & `ninfo-1.0.1/tests/test_util.py`

 * *Files identical despite different names*

