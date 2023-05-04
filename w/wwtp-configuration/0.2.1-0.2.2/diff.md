# Comparing `tmp/wwtp-configuration-0.2.1.tar.gz` & `tmp/wwtp-configuration-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwtp-configuration-0.2.1.tar", last modified: Wed Mar 15 18:07:07 2023, max compression
+gzip compressed data, was "wwtp-configuration-0.2.2.tar", last modified: Thu May  4 15:41:18 2023, max compression
```

## Comparing `wwtp-configuration-0.2.1.tar` & `wwtp-configuration-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:07:07.286329 wwtp-configuration-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-15 18:07:07.286329 wwtp-configuration-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:07:07.282329 wwtp-configuration-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/connection.rst
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/node.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/parse_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/tag.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/units.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/docs/visualize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-15 18:07:07.286329 wwtp-configuration-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:07:07.282329 wwtp-configuration-0.2.1/wwtp_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:07:07.286329 wwtp-configuration-0.2.1/wwtp_configuration/data/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/data/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/data/unit_definitions.txt
--rw-r--r--   0 runner    (1001) docker     (123)    71197 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    43566 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/parse_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    21039 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-03-15 18:07:03.000000 wwtp-configuration-0.2.1/wwtp_configuration/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 18:07:07.282329 wwtp-configuration-0.2.1/wwtp_configuration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-15 18:07:07.000000 wwtp-configuration-0.2.1/wwtp_configuration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-15 18:07:07.000000 wwtp-configuration-0.2.1/wwtp_configuration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 18:07:07.000000 wwtp-configuration-0.2.1/wwtp_configuration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 18:07:07.000000 wwtp-configuration-0.2.1/wwtp_configuration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-15 18:07:07.000000 wwtp-configuration-0.2.1/wwtp_configuration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-15 18:07:07.000000 wwtp-configuration-0.2.1/wwtp_configuration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:18.241913 wwtp-configuration-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-04 15:41:18.241913 wwtp-configuration-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:18.237913 wwtp-configuration-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/connection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/node.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/parse_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/tag.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/docs/visualize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 15:41:18.241913 wwtp-configuration-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:18.237913 wwtp-configuration-0.2.2/wwtp_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18364 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:18.241913 wwtp-configuration-0.2.2/wwtp_configuration/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/data/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/data/unit_definitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    71197 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43691 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/parse_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21039 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-04 15:41:12.000000 wwtp-configuration-0.2.2/wwtp_configuration/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:41:18.241913 wwtp-configuration-0.2.2/wwtp_configuration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-04 15:41:18.000000 wwtp-configuration-0.2.2/wwtp_configuration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 15:41:18.000000 wwtp-configuration-0.2.2/wwtp_configuration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:41:18.000000 wwtp-configuration-0.2.2/wwtp_configuration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:41:18.000000 wwtp-configuration-0.2.2/wwtp_configuration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-04 15:41:18.000000 wwtp-configuration-0.2.2/wwtp_configuration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 15:41:18.000000 wwtp-configuration-0.2.2/wwtp_configuration.egg-info/top_level.txt
```

### Comparing `wwtp-configuration-0.2.1/CONTRIBUTING.rst` & `wwtp-configuration-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/LICENSE` & `wwtp-configuration-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/PKG-INFO` & `wwtp-configuration-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwtp-configuration
-Version: 0.2.1
+Version: 0.2.2
 Summary: Class hierarchy to represent a wastewater treatment plant's configuration.
 Home-page: https://github.com/we3lab/wwtp-configuration
 Author: WE3 Lab
 Author-email: fchapin@stanford.edu
 License: UNKNOWN
 Keywords: wwtp-configuration
 Platform: UNKNOWN
```

### Comparing `wwtp-configuration-0.2.1/README.rst` & `wwtp-configuration-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/docs/Makefile` & `wwtp-configuration-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/docs/conf.py` & `wwtp-configuration-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/docs/index.rst` & `wwtp-configuration-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/docs/make.bat` & `wwtp-configuration-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/setup.py` & `wwtp-configuration-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "tox>=3.24.5",
     "Sphinx==4.2.0",
 ]
 
 requirements = [
     "pint==0.19.2",
     "networkx==2.8.5",
-    "pyvis==0.2.1",
+    "pyvis==0.2.2",
     "matplotlib==3.5.2",
     "pandas==1.4.0",
     "numpy==1.22.1"
 ]
 
 extra_requirements = {
     "setup": setup_requirements,
@@ -63,10 +63,10 @@
     python_requires=">=3.9",
     install_requires=requirements,
     setup_requires=setup_requirements,
     tests_require=test_requirements,
     extras_require=extra_requirements,
     test_suite="tests",
     url="https://github.com/we3lab/wwtp-configuration",
-    version="0.2.1",
+    version="0.2.2",
     zip_safe=False,
 )
```

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration/connection.py` & `wwtp-configuration-0.2.2/wwtp_configuration/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,24 @@
         Parameters
         ----------
         tag_name : str
             name of tag to remove
         """
         del self.tags[tag_name]
 
+    def get_tag(self, tag_name):
+        """Adds a tag to the node
+
+        Parameters
+        ----------
+        tag_name : str
+            Name of the tag to receive
+        """
+        return self.tags[tag_name]
+
     def get_source_id(self):
         """
         Returns
         -------
         str
             name of the source node
         """
```

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration/data/sample.json` & `wwtp-configuration-0.2.2/wwtp_configuration/data/sample.json`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration/node.py` & `wwtp-configuration-0.2.2/wwtp_configuration/node.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration/parse_json.py` & `wwtp-configuration-0.2.2/wwtp_configuration/parse_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,15 +683,18 @@
         Returns
         -------
         VirtualTag
             a Python object with the given ID and the values from `tag_info`
         """
         tag_list = []
         for subtag_id in tag_info["tags"]:
-            subtag = obj.get_tag(subtag_id, recurse=True)
+            if isinstance(obj, connection.Connection):
+                subtag = obj.get_tag(subtag_id)
+            else:
+                subtag = obj.get_tag(subtag_id, recurse=True)
             if subtag is None:
                 raise ValueError(
                     "Invalid Tag id {} in VirtualTag {}".format(subtag_id, tag_id)
                 )
             tag_list.append(subtag)
 
         try:
```

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration/tag.py` & `wwtp-configuration-0.2.2/wwtp_configuration/tag.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration/units.py` & `wwtp-configuration-0.2.2/wwtp_configuration/units.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration/utils.py` & `wwtp-configuration-0.2.2/wwtp_configuration/utils.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration/visualize.py` & `wwtp-configuration-0.2.2/wwtp_configuration/visualize.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration.egg-info/PKG-INFO` & `wwtp-configuration-0.2.2/wwtp_configuration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwtp-configuration
-Version: 0.2.1
+Version: 0.2.2
 Summary: Class hierarchy to represent a wastewater treatment plant's configuration.
 Home-page: https://github.com/we3lab/wwtp-configuration
 Author: WE3 Lab
 Author-email: fchapin@stanford.edu
 License: UNKNOWN
 Keywords: wwtp-configuration
 Platform: UNKNOWN
```

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration.egg-info/SOURCES.txt` & `wwtp-configuration-0.2.2/wwtp_configuration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.2.1/wwtp_configuration.egg-info/requires.txt` & `wwtp-configuration-0.2.2/wwtp_configuration.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 pint==0.19.2
 networkx==2.8.5
-pyvis==0.2.1
+pyvis==0.2.2
 matplotlib==3.5.2
 pandas==1.4.0
 numpy==1.22.1
 
 [all]
 pint==0.19.2
 networkx==2.8.5
-pyvis==0.2.1
+pyvis==0.2.2
 matplotlib==3.5.2
 pandas==1.4.0
 numpy==1.22.1
 black>=22.3.0
 flake8>=4.0.0
 codecov>=2.1.4
 pytest>=6.2.5
```

