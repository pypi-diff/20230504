# Comparing `tmp/oe_common-1.7.1.1.tar.gz` & `tmp/oe_common-1.7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oe_common-1.7.1.1.tar", last modified: Tue Oct 25 22:47:24 2022, max compression
+gzip compressed data, was "oe_common-1.7.1.2.tar", last modified: Thu May  4 03:45:10 2023, max compression
```

## Comparing `oe_common-1.7.1.1.tar` & `oe_common-1.7.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2022-10-25 22:47:24.501629 oe_common-1.7.1.1/
--rw-r--r--   0 jok4r      (501) staff       (20)     1071 2022-04-04 01:36:13.000000 oe_common-1.7.1.1/LICENSE.txt
--rw-r--r--   0 jok4r      (501) staff       (20)    10141 2022-10-25 22:47:24.501280 oe_common-1.7.1.1/PKG-INFO
--rw-r--r--   0 jok4r      (501) staff       (20)     9824 2022-04-04 01:36:13.000000 oe_common-1.7.1.1/README.md
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2022-10-25 22:47:24.500501 oe_common-1.7.1.1/oe_common/
--rw-r--r--   0 jok4r      (501) staff       (20)       25 2022-04-04 01:36:13.000000 oe_common-1.7.1.1/oe_common/__init__.py
--rw-r--r--   0 jok4r      (501) staff       (20)    12938 2022-10-25 22:45:56.000000 oe_common-1.7.1.1/oe_common/oe_common.py
-drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2022-10-25 22:47:24.501111 oe_common-1.7.1.1/oe_common.egg-info/
--rw-r--r--   0 jok4r      (501) staff       (20)    10141 2022-10-25 22:47:24.000000 oe_common-1.7.1.1/oe_common.egg-info/PKG-INFO
--rw-r--r--   0 jok4r      (501) staff       (20)      207 2022-10-25 22:47:24.000000 oe_common-1.7.1.1/oe_common.egg-info/SOURCES.txt
--rw-r--r--   0 jok4r      (501) staff       (20)        1 2022-10-25 22:47:24.000000 oe_common-1.7.1.1/oe_common.egg-info/dependency_links.txt
--rw-r--r--   0 jok4r      (501) staff       (20)       10 2022-10-25 22:47:24.000000 oe_common-1.7.1.1/oe_common.egg-info/top_level.txt
--rw-r--r--   0 jok4r      (501) staff       (20)       38 2022-10-25 22:47:24.501659 oe_common-1.7.1.1/setup.cfg
--rw-r--r--   0 jok4r      (501) staff       (20)      528 2022-10-25 22:46:40.000000 oe_common-1.7.1.1/setup.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 03:45:10.443391 oe_common-1.7.1.2/
+-rw-r--r--   0 jok4r      (501) staff       (20)     1071 2022-04-04 01:36:13.000000 oe_common-1.7.1.2/LICENSE.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)    10141 2023-05-04 03:45:10.442157 oe_common-1.7.1.2/PKG-INFO
+-rw-r--r--   0 jok4r      (501) staff       (20)     9824 2022-04-04 01:36:13.000000 oe_common-1.7.1.2/README.md
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 03:45:10.441274 oe_common-1.7.1.2/oe_common/
+-rw-r--r--   0 jok4r      (501) staff       (20)       25 2022-04-04 01:36:13.000000 oe_common-1.7.1.2/oe_common/__init__.py
+-rw-r--r--   0 jok4r      (501) staff       (20)    12959 2023-05-04 03:44:31.000000 oe_common-1.7.1.2/oe_common/oe_common.py
+drwxr-xr-x   0 jok4r      (501) staff       (20)        0 2023-05-04 03:45:10.441962 oe_common-1.7.1.2/oe_common.egg-info/
+-rw-r--r--   0 jok4r      (501) staff       (20)    10141 2023-05-04 03:45:10.000000 oe_common-1.7.1.2/oe_common.egg-info/PKG-INFO
+-rw-r--r--   0 jok4r      (501) staff       (20)      207 2023-05-04 03:45:10.000000 oe_common-1.7.1.2/oe_common.egg-info/SOURCES.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)        1 2023-05-04 03:45:10.000000 oe_common-1.7.1.2/oe_common.egg-info/dependency_links.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)       10 2023-05-04 03:45:10.000000 oe_common-1.7.1.2/oe_common.egg-info/top_level.txt
+-rw-r--r--   0 jok4r      (501) staff       (20)       38 2023-05-04 03:45:10.443425 oe_common-1.7.1.2/setup.cfg
+-rw-r--r--   0 jok4r      (501) staff       (20)      528 2023-05-04 03:44:31.000000 oe_common-1.7.1.2/setup.py
```

### Comparing `oe_common-1.7.1.1/LICENSE.txt` & `oe_common-1.7.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oe_common-1.7.1.1/PKG-INFO` & `oe_common-1.7.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oe_common
-Version: 1.7.1.1
+Version: 1.7.1.2
 Summary: OeCommon
 Home-page: https://github.com/jok4r/oe_common
 Author: Dmitry Yakovlev
 Author-email: info@overhosting.ru
 License: MIT
 Requires: requests
 Requires: psutil
```

### Comparing `oe_common-1.7.1.1/README.md` & `oe_common-1.7.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oe_common-1.7.1.1/oe_common/oe_common.py` & `oe_common-1.7.1.2/oe_common/oe_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 def rm(*filename):
     filenames = [filename]
     if isinstance(filename, tuple):
         filenames = filename
 
     for f in filenames:
-        if os.path.isfile(f):
+        if os.path.isfile(f) or os.path.islink(f):
             os.remove(f)
         elif os.path.isdir(f):
             shutil.rmtree(f, ignore_errors=True)
 
 
 def replace_string_in_file(path, regex, replaced, flags=0):
     if os.path.isfile(path):
```

### Comparing `oe_common-1.7.1.1/oe_common.egg-info/PKG-INFO` & `oe_common-1.7.1.2/oe_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oe-common
-Version: 1.7.1.1
+Version: 1.7.1.2
 Summary: OeCommon
 Home-page: https://github.com/jok4r/oe_common
 Author: Dmitry Yakovlev
 Author-email: info@overhosting.ru
 License: MIT
 Requires: requests
 Requires: psutil
```

### Comparing `oe_common-1.7.1.1/setup.py` & `oe_common-1.7.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = f.read()
 
 with open('LICENSE.txt') as f:
     licence = f.read()
 
 setup(
     name='oe_common',
-    version='1.7.1.1',
+    version='1.7.1.2',
     author='Dmitry Yakovlev',
     author_email='info@overhosting.ru',
     description='OeCommon',
     long_description=readme,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
     packages=['oe_common'],
```

