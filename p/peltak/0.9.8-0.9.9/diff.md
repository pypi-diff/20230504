# Comparing `tmp/peltak-0.9.8.tar.gz` & `tmp/peltak-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/peltak-0.9.8.tar", last modified: Thu Sep 10 01:21:28 2015, max compression
+gzip compressed data, was "dist/peltak-0.9.9.tar", last modified: Thu Sep 10 01:22:39 2015, max compression
```

## Comparing `peltak-0.9.8.tar` & `peltak-0.9.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:21:28.000000 peltak-0.9.8/
-drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak/
-drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak/actions/
--rw-r--r--   0 novo      (1000) novo      (1000)      440 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/actions/__init__.py
--rw-r--r--   0 novo      (1000) novo      (1000)     2036 2015-09-10 00:46:24.000000 peltak-0.9.8/peltak/actions/config.py
--rw-r--r--   0 novo      (1000) novo      (1000)     1019 2015-09-10 00:34:42.000000 peltak-0.9.8/peltak/actions/fetchtemplate.py
--rw-r--r--   0 novo      (1000) novo      (1000)     1192 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/actions/listactions.py
--rw-r--r--   0 novo      (1000) novo      (1000)     5279 2015-09-10 00:26:59.000000 peltak-0.9.8/peltak/actions/mr.py
--rw-r--r--   0 novo      (1000) novo      (1000)      706 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/actions/mrcleanup.py
--rw-r--r--   0 novo      (1000) novo      (1000)     1101 2015-09-10 00:26:59.000000 peltak-0.9.8/peltak/actions/mrget.py
--rw-r--r--   0 novo      (1000) novo      (1000)      727 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/actions/preview.py
--rw-r--r--   0 novo      (1000) novo      (1000)     1096 2015-09-10 00:26:59.000000 peltak-0.9.8/peltak/actions/push.py
--rw-r--r--   0 novo      (1000) novo      (1000)      388 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/actions/resetmr.py
--rw-r--r--   0 novo      (1000) novo      (1000)      370 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/actions/review.py
-drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak/common/
--rw-r--r--   0 novo      (1000) novo      (1000)       24 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/common/__init__.py
--rw-r--r--   0 novo      (1000) novo      (1000)     2229 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/common/cache.py
--rw-r--r--   0 novo      (1000) novo      (1000)     4079 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/common/prompt.py
--rw-r--r--   0 novo      (1000) novo      (1000)     2165 2015-09-10 00:34:42.000000 peltak-0.9.8/peltak/common/utils.py
-drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak/core/
--rw-r--r--   0 novo      (1000) novo      (1000)     1366 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/core/__init__.py
--rw-r--r--   0 novo      (1000) novo      (1000)     7794 2015-09-09 23:50:44.000000 peltak-0.9.8/peltak/core/api.py
--rw-r--r--   0 novo      (1000) novo      (1000)     1280 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/core/git.py
--rw-r--r--   0 novo      (1000) novo      (1000)     2896 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/core/template.py
-drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak/system/
--rw-r--r--   0 novo      (1000) novo      (1000)       24 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/system/__init__.py
--rw-r--r--   0 novo      (1000) novo      (1000)     2724 2015-09-10 00:26:59.000000 peltak-0.9.8/peltak/system/appcontext.py
--rw-r--r--   0 novo      (1000) novo      (1000)     1661 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/system/forms.py
--rw-r--r--   0 novo      (1000) novo      (1000)        0 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/__init__.py
--rw-r--r--   0 novo      (1000) novo      (1000)      515 2015-09-09 23:37:20.000000 peltak-0.9.8/peltak/config.py
--rwxr-xr-x   0 novo      (1000) novo      (1000)     3474 2015-09-10 00:26:59.000000 peltak-0.9.8/peltak/runner.py
-drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak.egg-info/
--rw-r--r--   0 novo      (1000) novo      (1000)     1097 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak.egg-info/PKG-INFO
--rw-r--r--   0 novo      (1000) novo      (1000)      800 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak.egg-info/SOURCES.txt
--rw-r--r--   0 novo      (1000) novo      (1000)        1 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak.egg-info/dependency_links.txt
--rw-r--r--   0 novo      (1000) novo      (1000)       47 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak.egg-info/entry_points.txt
--rw-r--r--   0 novo      (1000) novo      (1000)       21 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak.egg-info/requires.txt
--rw-r--r--   0 novo      (1000) novo      (1000)        7 2015-09-10 01:21:27.000000 peltak-0.9.8/peltak.egg-info/top_level.txt
--rw-r--r--   0 novo      (1000) novo      (1000)      371 2015-09-08 23:45:42.000000 peltak-0.9.8/README.rst
--rw-r--r--   0 novo      (1000) novo      (1000)     1114 2015-09-10 01:21:17.000000 peltak-0.9.8/setup.py
--rw-r--r--   0 novo      (1000) novo      (1000)     1097 2015-09-10 01:21:27.000000 peltak-0.9.8/PKG-INFO
--rw-r--r--   0 novo      (1000) novo      (1000)       59 2015-09-10 01:21:28.000000 peltak-0.9.8/setup.cfg
+drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:22:39.000000 peltak-0.9.9/
+drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak/
+drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak/actions/
+-rw-r--r--   0 novo      (1000) novo      (1000)      440 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/actions/__init__.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     2036 2015-09-10 00:46:24.000000 peltak-0.9.9/peltak/actions/config.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     1019 2015-09-10 00:34:42.000000 peltak-0.9.9/peltak/actions/fetchtemplate.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     1192 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/actions/listactions.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     5279 2015-09-10 00:26:59.000000 peltak-0.9.9/peltak/actions/mr.py
+-rw-r--r--   0 novo      (1000) novo      (1000)      706 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/actions/mrcleanup.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     1101 2015-09-10 00:26:59.000000 peltak-0.9.9/peltak/actions/mrget.py
+-rw-r--r--   0 novo      (1000) novo      (1000)      727 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/actions/preview.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     1096 2015-09-10 00:26:59.000000 peltak-0.9.9/peltak/actions/push.py
+-rw-r--r--   0 novo      (1000) novo      (1000)      388 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/actions/resetmr.py
+-rw-r--r--   0 novo      (1000) novo      (1000)      370 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/actions/review.py
+drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak/common/
+-rw-r--r--   0 novo      (1000) novo      (1000)       24 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/common/__init__.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     2229 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/common/cache.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     4079 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/common/prompt.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     2165 2015-09-10 00:34:42.000000 peltak-0.9.9/peltak/common/utils.py
+drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak/core/
+-rw-r--r--   0 novo      (1000) novo      (1000)     1366 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/core/__init__.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     7794 2015-09-09 23:50:44.000000 peltak-0.9.9/peltak/core/api.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     1280 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/core/git.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     2896 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/core/template.py
+drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak/system/
+-rw-r--r--   0 novo      (1000) novo      (1000)       24 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/system/__init__.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     2724 2015-09-10 00:26:59.000000 peltak-0.9.9/peltak/system/appcontext.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     1661 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/system/forms.py
+-rw-r--r--   0 novo      (1000) novo      (1000)        0 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/__init__.py
+-rw-r--r--   0 novo      (1000) novo      (1000)      515 2015-09-09 23:37:20.000000 peltak-0.9.9/peltak/config.py
+-rwxr-xr-x   0 novo      (1000) novo      (1000)     3474 2015-09-10 00:26:59.000000 peltak-0.9.9/peltak/runner.py
+drwxr-xr-x   0 novo      (1000) novo      (1000)        0 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak.egg-info/
+-rw-r--r--   0 novo      (1000) novo      (1000)     1115 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak.egg-info/PKG-INFO
+-rw-r--r--   0 novo      (1000) novo      (1000)      800 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak.egg-info/SOURCES.txt
+-rw-r--r--   0 novo      (1000) novo      (1000)        1 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak.egg-info/dependency_links.txt
+-rw-r--r--   0 novo      (1000) novo      (1000)       47 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak.egg-info/entry_points.txt
+-rw-r--r--   0 novo      (1000) novo      (1000)       21 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak.egg-info/requires.txt
+-rw-r--r--   0 novo      (1000) novo      (1000)        7 2015-09-10 01:22:39.000000 peltak-0.9.9/peltak.egg-info/top_level.txt
+-rw-r--r--   0 novo      (1000) novo      (1000)      371 2015-09-08 23:45:42.000000 peltak-0.9.9/README.rst
+-rw-r--r--   0 novo      (1000) novo      (1000)     1154 2015-09-10 01:22:25.000000 peltak-0.9.9/setup.py
+-rw-r--r--   0 novo      (1000) novo      (1000)     1115 2015-09-10 01:22:39.000000 peltak-0.9.9/PKG-INFO
+-rw-r--r--   0 novo      (1000) novo      (1000)       59 2015-09-10 01:22:39.000000 peltak-0.9.9/setup.cfg
```

### Comparing `peltak-0.9.8/peltak/actions/config.py` & `peltak-0.9.9/peltak/actions/config.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/actions/fetchtemplate.py` & `peltak-0.9.9/peltak/actions/fetchtemplate.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/actions/listactions.py` & `peltak-0.9.9/peltak/actions/listactions.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/actions/mr.py` & `peltak-0.9.9/peltak/actions/mr.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/actions/mrcleanup.py` & `peltak-0.9.9/peltak/actions/mrcleanup.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/actions/mrget.py` & `peltak-0.9.9/peltak/actions/mrget.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/actions/preview.py` & `peltak-0.9.9/peltak/actions/preview.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/actions/push.py` & `peltak-0.9.9/peltak/actions/push.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/common/cache.py` & `peltak-0.9.9/peltak/common/cache.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/common/prompt.py` & `peltak-0.9.9/peltak/common/prompt.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/common/utils.py` & `peltak-0.9.9/peltak/common/utils.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/core/__init__.py` & `peltak-0.9.9/peltak/core/__init__.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/core/api.py` & `peltak-0.9.9/peltak/core/api.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/core/git.py` & `peltak-0.9.9/peltak/core/git.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/core/template.py` & `peltak-0.9.9/peltak/core/template.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/system/appcontext.py` & `peltak-0.9.9/peltak/system/appcontext.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/system/forms.py` & `peltak-0.9.9/peltak/system/forms.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/config.py` & `peltak-0.9.9/peltak/config.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak/runner.py` & `peltak-0.9.9/peltak/runner.py`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/peltak.egg-info/PKG-INFO` & `peltak-0.9.9/peltak.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: peltak
-Version: 0.9.8
-Summary: Command line utility to improve your daily workflow.The main focus so far is making a gitlab merge request.
+Version: 0.9.9
+Summary: Command line utility to improve your daily workflow.The main focus so far is making a Gitlab merge request management easier.
 Home-page: http://github.com/novopl/peltak
 Author: Mateusz 'novo' Klos
 Author-email: novopl@gmail.com
 License: MIT
 Description: ###############################
         peltak - Improve your workflow
         ###############################
```

### Comparing `peltak-0.9.8/peltak.egg-info/SOURCES.txt` & `peltak-0.9.9/peltak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peltak-0.9.8/setup.py` & `peltak-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name = "peltak",
-    version = "0.9.8",
+    version = "0.9.9",
     author = "Mateusz 'novo' Klos",
     author_email = "novopl@gmail.com",
     license = "MIT",
     keywords = "project management git gitlab",
     url = "http://github.com/novopl/peltak",
     entry_points={
         'console_scripts': [
@@ -23,15 +23,16 @@
         'peltak',
         'peltak.actions',
         'peltak.common',
         'peltak.core',
         'peltak.system',
     ],
     description = ("Command line utility to improve your daily workflow."
-                   "The main focus so far is making a gitlab merge request."),
+                   "The main focus so far is making a Gitlab merge request"
+                   " management easier."),
     long_description=read('README.rst'),
     install_requires = [
         'six', 'libigor', 'requests'
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Topic :: Utilities",
```

### Comparing `peltak-0.9.8/PKG-INFO` & `peltak-0.9.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: peltak
-Version: 0.9.8
-Summary: Command line utility to improve your daily workflow.The main focus so far is making a gitlab merge request.
+Version: 0.9.9
+Summary: Command line utility to improve your daily workflow.The main focus so far is making a Gitlab merge request management easier.
 Home-page: http://github.com/novopl/peltak
 Author: Mateusz 'novo' Klos
 Author-email: novopl@gmail.com
 License: MIT
 Description: ###############################
         peltak - Improve your workflow
         ###############################
```

