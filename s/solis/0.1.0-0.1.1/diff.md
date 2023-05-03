# Comparing `tmp/solis-0.1.0.tar.gz` & `tmp/solis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solis-0.1.0.tar", max compression
+gzip compressed data, was "solis-0.1.1.tar", max compression
```

## Comparing `solis-0.1.0.tar` & `solis-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1847 2023-05-03 22:04:17.748955 solis-0.1.0/README.md
--rw-r--r--   0        0        0      604 2023-05-03 21:14:35.214958 solis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 21:33:56.739635 solis-0.1.0/src/solis/__init__.py
--rw-r--r--   0        0        0     2004 2023-05-03 21:58:34.124284 solis-0.1.0/src/solis/cli.py
--rw-r--r--   0        0        0      125 2023-03-15 22:33:55.819344 solis-0.1.0/src/solis/exceptions.py
--rw-r--r--   0        0        0     9256 2023-05-03 21:59:48.005254 solis-0.1.0/src/solis/solis.py
--rw-r--r--   0        0        0      422 2023-03-17 13:16:07.409462 solis-0.1.0/src/solis/utils.py
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 solis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1847 2023-05-03 22:04:17.748955 solis-0.1.1/README.md
+-rw-r--r--   0        0        0      604 2023-05-03 22:24:16.898268 solis-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-15 21:33:56.739635 solis-0.1.1/src/solis/__init__.py
+-rw-r--r--   0        0        0     2004 2023-05-03 21:58:34.124284 solis-0.1.1/src/solis/cli.py
+-rw-r--r--   0        0        0      125 2023-03-15 22:33:55.819344 solis-0.1.1/src/solis/exceptions.py
+-rw-r--r--   0        0        0     9256 2023-05-03 21:59:48.005254 solis-0.1.1/src/solis/solis.py
+-rw-r--r--   0        0        0      422 2023-03-17 13:16:07.409462 solis-0.1.1/src/solis/utils.py
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 solis-0.1.1/PKG-INFO
```

### Comparing `solis-0.1.0/README.md` & `solis-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `solis-0.1.0/pyproject.toml` & `solis-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "solis"
-version = "0.1.0"
+version = "0.1.1"
 description = "A tool to control Solis Hybrid Inverters"
 authors = ["Dan Foster <dan@zem.org.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "solis", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
 asyncclick = "^8.1.3.4"
-zem-pysolarmanv5 = "^2.5.0rc1"
+zem-pysolarmanv5 = "^2.5.0rc2"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.990"
 flake8 = "^5.0.4"
 black = "^22.10.0"
 flake8-pyproject = "^1.1.0.post0"
```

### Comparing `solis-0.1.0/src/solis/cli.py` & `solis-0.1.1/src/solis/cli.py`

 * *Files identical despite different names*

### Comparing `solis-0.1.0/src/solis/solis.py` & `solis-0.1.1/src/solis/solis.py`

 * *Files identical despite different names*

### Comparing `solis-0.1.0/PKG-INFO` & `solis-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: solis
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to control Solis Hybrid Inverters
 License: MIT
 Author: Dan Foster
 Author-email: dan@zem.org.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncclick (>=8.1.3.4,<9.0.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: zem-pysolarmanv5 (>=2.5.0rc1,<3.0.0)
+Requires-Dist: zem-pysolarmanv5 (>=2.5.0rc2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Solis
 
 This is a Python module to interact with Solis Invertors connected via the Solarman v5 data loggers.
 
 It builds on top of the [pysolarmanv5](https://github.com/jmccrohan/pysolarmanv5/) module to provide structured data output that can be consumed without needing to the know the registers and data formats of the underlying device.
```

