# Comparing `tmp/opencmiss2cmlibs-0.1.2.tar.gz` & `tmp/opencmiss2cmlibs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss2cmlibs-0.1.2.tar", last modified: Tue May  2 03:30:43 2023, max compression
+gzip compressed data, was "opencmiss2cmlibs-0.1.3.tar", last modified: Wed May  3 23:31:21 2023, max compression
```

## Comparing `opencmiss2cmlibs-0.1.2.tar` & `opencmiss2cmlibs-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-02 03:30:43.223773 opencmiss2cmlibs-0.1.2/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      595 2023-03-27 09:14:03.000000 opencmiss2cmlibs-0.1.2/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1556 2023-05-02 03:30:43.223934 opencmiss2cmlibs-0.1.2/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      851 2023-04-18 07:04:17.000000 opencmiss2cmlibs-0.1.2/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       91 2023-03-28 00:57:24.000000 opencmiss2cmlibs-0.1.2/pyproject.toml
--rw-r--r--   0 hsor001  (1210695619) 1403514002      731 2023-05-02 03:30:43.224530 opencmiss2cmlibs-0.1.2/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002       69 2023-03-28 00:57:18.000000 opencmiss2cmlibs-0.1.2/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-02 03:30:43.206271 opencmiss2cmlibs-0.1.2/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-02 03:30:43.214558 opencmiss2cmlibs-0.1.2/src/libocm2cml/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:37:49.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6651 2023-03-28 08:02:24.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/btm_matcher.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     9983 2023-03-28 08:03:52.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/btm_utils.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6644 2023-03-28 07:55:22.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/fixer_base.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    14713 2023-03-28 07:55:22.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/fixer_util.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-02 03:30:43.215858 opencmiss2cmlibs-0.1.2/src/libocm2cml/fixes/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:30:01.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/fixes/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5880 2023-05-02 03:29:51.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/fixes/fix_imports.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     7055 2023-03-28 07:49:09.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/patcomp.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-02 03:30:43.220577 opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:40:03.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5970 2023-03-28 07:45:09.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/driver.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5565 2023-04-04 01:09:27.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/grammar.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1644 2023-03-28 07:49:35.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/literals.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     8159 2023-03-28 07:46:32.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/parse.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    13855 2023-04-04 01:13:18.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/pgen.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1320 2023-04-04 01:10:05.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/token.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    20916 2023-03-31 02:18:24.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/tokenize.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1254 2023-04-04 01:11:42.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pygram.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    28050 2023-03-28 07:43:56.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/pytree.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    27525 2023-03-28 07:59:16.000000 opencmiss2cmlibs-0.1.2/src/libocm2cml/refactor.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-02 03:30:43.222842 opencmiss2cmlibs-0.1.2/src/opencmiss2cmlibs.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1556 2023-05-02 03:30:42.000000 opencmiss2cmlibs-0.1.2/src/opencmiss2cmlibs.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      862 2023-05-02 03:30:43.000000 opencmiss2cmlibs-0.1.2/src/opencmiss2cmlibs.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-05-02 03:30:42.000000 opencmiss2cmlibs-0.1.2/src/opencmiss2cmlibs.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002      125 2023-05-02 03:30:42.000000 opencmiss2cmlibs-0.1.2/src/opencmiss2cmlibs.egg-info/entry_points.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       11 2023-05-02 03:30:42.000000 opencmiss2cmlibs-0.1.2/src/opencmiss2cmlibs.egg-info/top_level.txt
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-02 03:30:43.223133 opencmiss2cmlibs-0.1.2/tests/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3508 2023-03-30 20:42:48.000000 opencmiss2cmlibs-0.1.2/tests/test_import.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-03 23:31:21.005742 opencmiss2cmlibs-0.1.3/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      595 2023-03-27 09:14:03.000000 opencmiss2cmlibs-0.1.3/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1282 2023-05-03 23:31:21.006674 opencmiss2cmlibs-0.1.3/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      851 2023-04-18 07:04:17.000000 opencmiss2cmlibs-0.1.3/README.rst
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       91 2023-03-28 00:57:24.000000 opencmiss2cmlibs-0.1.3/pyproject.toml
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      735 2023-05-03 23:31:21.010833 opencmiss2cmlibs-0.1.3/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       69 2023-03-28 00:57:18.000000 opencmiss2cmlibs-0.1.3/setup.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-03 23:31:20.987447 opencmiss2cmlibs-0.1.3/src/
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-03 23:31:20.994500 opencmiss2cmlibs-0.1.3/src/libocm2cml/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:37:49.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     6651 2023-03-28 08:02:24.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/btm_matcher.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     9983 2023-03-28 08:03:52.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/btm_utils.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     6644 2023-03-28 07:55:22.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/fixer_base.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    14713 2023-03-28 07:55:22.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/fixer_util.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-03 23:31:20.995733 opencmiss2cmlibs-0.1.3/src/libocm2cml/fixes/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:30:01.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/fixes/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5880 2023-05-02 03:29:51.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/fixes/fix_imports.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     7055 2023-03-28 07:49:09.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/patcomp.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-03 23:31:20.999704 opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:40:03.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5970 2023-03-28 07:45:09.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/driver.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5565 2023-04-04 01:09:27.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/grammar.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1644 2023-03-28 07:49:35.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/literals.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     8159 2023-03-28 07:46:32.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/parse.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    13855 2023-04-04 01:13:18.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/pgen.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1320 2023-04-04 01:10:05.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/token.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    20916 2023-03-31 02:18:24.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/tokenize.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1254 2023-04-04 01:11:42.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pygram.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    28050 2023-03-28 07:43:56.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/pytree.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    27525 2023-03-28 07:59:16.000000 opencmiss2cmlibs-0.1.3/src/libocm2cml/refactor.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-03 23:31:21.001937 opencmiss2cmlibs-0.1.3/src/opencmiss2cmlibs.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1282 2023-05-03 23:31:20.000000 opencmiss2cmlibs-0.1.3/src/opencmiss2cmlibs.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      912 2023-05-03 23:31:20.000000 opencmiss2cmlibs-0.1.3/src/opencmiss2cmlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-05-03 23:31:20.000000 opencmiss2cmlibs-0.1.3/src/opencmiss2cmlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      124 2023-05-03 23:31:20.000000 opencmiss2cmlibs-0.1.3/src/opencmiss2cmlibs.egg-info/entry_points.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       11 2023-05-03 23:31:20.000000 opencmiss2cmlibs-0.1.3/src/opencmiss2cmlibs.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-05-03 23:31:21.004433 opencmiss2cmlibs-0.1.3/tests/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     2115 2023-04-04 01:19:31.000000 opencmiss2cmlibs-0.1.3/tests/test_argon_document.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     3508 2023-03-30 20:42:48.000000 opencmiss2cmlibs-0.1.3/tests/test_import.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      903 2023-04-04 01:15:05.000000 opencmiss2cmlibs-0.1.3/tests/test_syntax.py
```

### Comparing `opencmiss2cmlibs-0.1.2/LICENSE` & `opencmiss2cmlibs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/PKG-INFO` & `opencmiss2cmlibs-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: opencmiss2cmlibs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Application converting packages that use OpenCMISS-Zinc to CMLibs Zinc.
-Home-page: UNKNOWN
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: Apache Software License
-Description: OpenCMISS 2 CMLibs
-        ==================
-        
-        This tool is meant to help update code from using OpenCMISS python packages to CMLibs python packages.
-        It also contains a tool to upgrade Argon documents from OpenCMISS to CMLibs.
-        
-        Install with::
-        
-          pip install opencmiss2cmlibs
-        
-        Usage::
-        
-          opencmiss2cmlibs <directory-of-python-packge-to-update>
-        
-        This displays a diff of the changes on *stdout*.
-        To make the changes in-place and not create a backup file use::
-        
-          opencmiss2cmlibs -w -n <directory-of-python-packge-to-update>
-        
-        This form of the command is best suited for use with code that is under version control, Git or the like.
-        
-        To upgrade Argon documents us the following command::
-        
-          upgradeargondocuments <directory-containing-argon-files>
-        
-        This command will search through the directory tree looking for old Argon documents and convert them to new ones.
-        
 Keywords: continuum modelling
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
+
+OpenCMISS 2 CMLibs
+==================
+
+This tool is meant to help update code from using OpenCMISS python packages to CMLibs python packages.
+It also contains a tool to upgrade Argon documents from OpenCMISS to CMLibs.
+
+Install with::
+
+  pip install opencmiss2cmlibs
+
+Usage::
+
+  opencmiss2cmlibs <directory-of-python-packge-to-update>
+
+This displays a diff of the changes on *stdout*.
+To make the changes in-place and not create a backup file use::
+
+  opencmiss2cmlibs -w -n <directory-of-python-packge-to-update>
+
+This form of the command is best suited for use with code that is under version control, Git or the like.
+
+To upgrade Argon documents us the following command::
+
+  upgradeargondocuments <directory-containing-argon-files>
+
+This command will search through the directory tree looking for old Argon documents and convert them to new ones.
```

### Comparing `opencmiss2cmlibs-0.1.2/README.rst` & `opencmiss2cmlibs-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/setup.cfg` & `opencmiss2cmlibs-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = opencmiss2cmlibs
-version = attr: opencmiss2cmlibs.__version__
+version = attr: src.opencmiss2cmlibs.__version__
 description = Application converting packages that use OpenCMISS-Zinc to CMLibs Zinc.
 long_description = file: README.rst, LICENSE.rst
 keywords = continuum modelling
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: Apache Software License
```

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/btm_matcher.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/btm_matcher.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/btm_utils.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/btm_utils.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/fixer_base.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/fixer_base.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/fixer_util.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/fixer_util.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/fixes/fix_imports.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/fixes/fix_imports.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/patcomp.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/patcomp.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/driver.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/grammar.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/literals.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/parse.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/pgen.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/pgen.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/token.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/pgen2/tokenize.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/pgen2/tokenize.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/pygram.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/pygram.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/pytree.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/pytree.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/libocm2cml/refactor.py` & `opencmiss2cmlibs-0.1.3/src/libocm2cml/refactor.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.2/src/opencmiss2cmlibs.egg-info/PKG-INFO` & `opencmiss2cmlibs-0.1.3/src/opencmiss2cmlibs.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: opencmiss2cmlibs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Application converting packages that use OpenCMISS-Zinc to CMLibs Zinc.
-Home-page: UNKNOWN
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: Apache Software License
-Description: OpenCMISS 2 CMLibs
-        ==================
-        
-        This tool is meant to help update code from using OpenCMISS python packages to CMLibs python packages.
-        It also contains a tool to upgrade Argon documents from OpenCMISS to CMLibs.
-        
-        Install with::
-        
-          pip install opencmiss2cmlibs
-        
-        Usage::
-        
-          opencmiss2cmlibs <directory-of-python-packge-to-update>
-        
-        This displays a diff of the changes on *stdout*.
-        To make the changes in-place and not create a backup file use::
-        
-          opencmiss2cmlibs -w -n <directory-of-python-packge-to-update>
-        
-        This form of the command is best suited for use with code that is under version control, Git or the like.
-        
-        To upgrade Argon documents us the following command::
-        
-          upgradeargondocuments <directory-containing-argon-files>
-        
-        This command will search through the directory tree looking for old Argon documents and convert them to new ones.
-        
 Keywords: continuum modelling
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
+
+OpenCMISS 2 CMLibs
+==================
+
+This tool is meant to help update code from using OpenCMISS python packages to CMLibs python packages.
+It also contains a tool to upgrade Argon documents from OpenCMISS to CMLibs.
+
+Install with::
+
+  pip install opencmiss2cmlibs
+
+Usage::
+
+  opencmiss2cmlibs <directory-of-python-packge-to-update>
+
+This displays a diff of the changes on *stdout*.
+To make the changes in-place and not create a backup file use::
+
+  opencmiss2cmlibs -w -n <directory-of-python-packge-to-update>
+
+This form of the command is best suited for use with code that is under version control, Git or the like.
+
+To upgrade Argon documents us the following command::
+
+  upgradeargondocuments <directory-containing-argon-files>
+
+This command will search through the directory tree looking for old Argon documents and convert them to new ones.
```

### Comparing `opencmiss2cmlibs-0.1.2/src/opencmiss2cmlibs.egg-info/SOURCES.txt` & `opencmiss2cmlibs-0.1.3/src/opencmiss2cmlibs.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,8 +23,10 @@
 src/libocm2cml/pgen2/token.py
 src/libocm2cml/pgen2/tokenize.py
 src/opencmiss2cmlibs.egg-info/PKG-INFO
 src/opencmiss2cmlibs.egg-info/SOURCES.txt
 src/opencmiss2cmlibs.egg-info/dependency_links.txt
 src/opencmiss2cmlibs.egg-info/entry_points.txt
 src/opencmiss2cmlibs.egg-info/top_level.txt
-tests/test_import.py
+tests/test_argon_document.py
+tests/test_import.py
+tests/test_syntax.py
```

### Comparing `opencmiss2cmlibs-0.1.2/tests/test_import.py` & `opencmiss2cmlibs-0.1.3/tests/test_import.py`

 * *Files identical despite different names*

