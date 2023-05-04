# Comparing `tmp/caep-0.1.7.tar.gz` & `tmp/caep-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caep-0.1.7.tar", last modified: Fri Apr 21 06:55:30 2023, max compression
+gzip compressed data, was "caep-0.1.8.tar", last modified: Thu May  4 16:45:13 2023, max compression
```

## Comparing `caep-0.1.7.tar` & `caep-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-21 06:55:30.287869 caep-0.1.7/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-0.1.7/LICENSE
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-04-21 06:55:30.287869 caep-0.1.7/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9157 2023-03-28 14:28:15.000000 caep-0.1.7/README.md
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-21 06:55:30.284536 caep-0.1.7/caep/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-0.1.7/caep/__init__.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8171 2023-04-21 06:55:27.000000 caep-0.1.7/caep/config.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-0.1.7/caep/example.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1396 2023-03-28 05:50:28.000000 caep-0.1.7/caep/helpers.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11081 2023-01-30 11:31:45.000000 caep-0.1.7/caep/schema.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-0.1.7/caep/xdg.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-21 06:55:30.284536 caep-0.1.7/caep.egg-info/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      343 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       23 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/requires.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-04-21 06:55:30.000000 caep-0.1.7/caep.egg-info/top_level.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-0.1.7/caep.egg-info/zip-safe
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-04-21 06:55:30.287869 caep-0.1.7/setup.cfg
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      953 2023-04-21 06:55:27.000000 caep-0.1.7/setup.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-04-21 06:55:30.287869 caep-0.1.7/tests/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-0.1.7/tests/test_config.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1455 2023-03-28 05:50:28.000000 caep-0.1.7/tests/test_helpers.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    10271 2023-04-21 06:55:27.000000 caep-0.1.7/tests/test_schema.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-05-04 16:45:13.847711 caep-0.1.8/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-0.1.8/LICENSE
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-05-04 16:45:13.847711 caep-0.1.8/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9157 2023-03-28 14:28:15.000000 caep-0.1.8/README.md
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-05-04 16:45:13.844377 caep-0.1.8/caep/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-0.1.8/caep/__init__.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8171 2023-04-21 06:55:27.000000 caep-0.1.8/caep/config.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-0.1.8/caep/example.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1396 2023-03-28 05:50:28.000000 caep-0.1.8/caep/helpers.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2023-01-02 09:23:36.000000 caep-0.1.8/caep/py.typed
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11081 2023-01-30 11:31:45.000000 caep-0.1.8/caep/schema.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-0.1.8/caep/xdg.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-05-04 16:45:13.847711 caep-0.1.8/caep.egg-info/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      357 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       23 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/requires.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/top_level.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-0.1.8/caep.egg-info/zip-safe
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-05-04 16:45:13.847711 caep-0.1.8/setup.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      994 2023-05-04 16:45:10.000000 caep-0.1.8/setup.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-05-04 16:45:13.847711 caep-0.1.8/tests/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-0.1.8/tests/test_config.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1455 2023-03-28 05:50:28.000000 caep-0.1.8/tests/test_helpers.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    10271 2023-04-21 06:55:27.000000 caep-0.1.8/tests/test_schema.py
```

### Comparing `caep-0.1.7/LICENSE` & `caep-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caep-0.1.7/PKG-INFO` & `caep-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.7
+Version: 0.1.8
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caep-0.1.7/README.md` & `caep-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `caep-0.1.7/caep/config.py` & `caep-0.1.8/caep/config.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.7/caep/example.py` & `caep-0.1.8/caep/example.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.7/caep/helpers.py` & `caep-0.1.8/caep/helpers.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.7/caep/schema.py` & `caep-0.1.8/caep/schema.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.7/caep/xdg.py` & `caep-0.1.8/caep/xdg.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.7/caep.egg-info/PKG-INFO` & `caep-0.1.8/caep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.7
+Version: 0.1.8
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caep-0.1.7/setup.py` & `caep-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), "rb") as f:
     long_description = f.read().decode("utf-8")
 
 setup(
     name="caep",
-    version="0.1.7",
+    version="0.1.8",
     author="mnemonic AS",
     zip_safe=True,
     author_email="opensource@mnemonic.no",
     description="Config Argument Env Parser (CAEP)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="ISC",
     keywords="mnemonic",
     packages=["caep"],
     url="https://github.com/mnemonic-no/caep",
     python_requires=">=3.6, <4",
+    package_data={"caep": ["py.typed"]},
     install_requires=[
         "pydantic>=1.8.0,<2.0.0",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Topic :: Utilities",
         "License :: OSI Approved :: ISC License (ISCL)",
```

### Comparing `caep-0.1.7/tests/test_config.py` & `caep-0.1.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.7/tests/test_helpers.py` & `caep-0.1.8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.7/tests/test_schema.py` & `caep-0.1.8/tests/test_schema.py`

 * *Files identical despite different names*

