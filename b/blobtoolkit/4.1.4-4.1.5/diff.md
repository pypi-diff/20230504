# Comparing `tmp/blobtoolkit-4.1.4.tar.gz` & `tmp/blobtoolkit-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blobtoolkit-4.1.4.tar", last modified: Mon Apr 17 08:34:58 2023, max compression
+gzip compressed data, was "blobtoolkit-4.1.5.tar", last modified: Thu May  4 13:28:24 2023, max compression
```

## Comparing `blobtoolkit-4.1.4.tar` & `blobtoolkit-4.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:34:58.851912 blobtoolkit-4.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 08:34:43.000000 blobtoolkit-4.1.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 08:34:43.000000 blobtoolkit-4.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 08:34:43.000000 blobtoolkit-4.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-17 08:34:58.851912 blobtoolkit-4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-17 08:34:43.000000 blobtoolkit-4.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-17 08:34:58.851912 blobtoolkit-4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:34:58.847912 blobtoolkit-4.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:34:58.851912 blobtoolkit-4.1.4/src/blobtoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 08:34:58.000000 blobtoolkit-4.1.4/src/blobtoolkit.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:34:58.847912 blobtoolkit-4.1.4/src/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:34:58.847912 blobtoolkit-4.1.4/src/data/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/basic.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/meta.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:34:58.851912 blobtoolkit-4.1.4/src/data/schema/subschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/array.data.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/array.meta.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/assembly.basic.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/assembly.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/category.data.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/category.meta.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/fields.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/identifier.data.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/identifier.meta.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/multiarray.data.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/multiarray.meta.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/plot.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/reads.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/taxon.basic.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/taxon.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/variable.data.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 08:34:44.000000 blobtoolkit-4.1.4/src/data/schema/subschemas/variable.meta.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:28:24.902997 blobtoolkit-4.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-04 13:28:24.902997 blobtoolkit-4.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-04 13:28:24.906997 blobtoolkit-4.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:28:24.894997 blobtoolkit-4.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:28:24.902997 blobtoolkit-4.1.5/src/blobtoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 13:28:24.000000 blobtoolkit-4.1.5/src/blobtoolkit.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:28:24.894997 blobtoolkit-4.1.5/src/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:28:24.898997 blobtoolkit-4.1.5/src/data/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/basic.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/meta.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:28:24.902997 blobtoolkit-4.1.5/src/data/schema/subschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/array.data.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/array.meta.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/assembly.basic.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/assembly.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/category.data.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/category.meta.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/fields.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/identifier.data.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/identifier.meta.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/multiarray.data.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/multiarray.meta.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/plot.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/reads.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/taxon.basic.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/taxon.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/variable.data.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-04 13:28:11.000000 blobtoolkit-4.1.5/src/data/schema/subschemas/variable.meta.schema.json
```

### Comparing `blobtoolkit-4.1.4/LICENSE` & `blobtoolkit-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/PKG-INFO` & `blobtoolkit-4.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobtoolkit
-Version: 4.1.4
+Version: 4.1.5
 Summary: blobtoolkit
 Home-page: https://github.com/blobtoolkit/blobtoolkit
 Author: blobtoolkit
 Author-email: blobtoolkit@genomehubs.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blobtoolkit/blobtoolkit/issues
 Project-URL: Source, https://github.com/blobtoolkit/blobtoolkit
```

### Comparing `blobtoolkit-4.1.4/README.md` & `blobtoolkit-4.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# BlobToolKit (v4.1.4)
+# BlobToolKit (v4.1.5)
 
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![DOI](https://zenodo.org/badge/150091036.svg)](https://zenodo.org/badge/latestdoi/150091036)
 
 BlobToolKit is described in our [BlobToolKit paper](https://doi.org/10.1534/g3.119.400908):
 
 > BlobToolKit – Interactive quality assessment of genome assemblies
```

### Comparing `blobtoolkit-4.1.4/setup.cfg` & `blobtoolkit-4.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/setup.py` & `blobtoolkit-4.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="blobtoolkit",  # Required
-    version="4.1.4",
+    version="4.1.5",
     description="blobtoolkit",  # Optional
     long_description="blobtoolkit",  # Optional
     long_description_content_type="text/markdown",
     # long_description="%s\n%s"
     # % (
     #     re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
     #         "", read("README.rst")
```

### Comparing `blobtoolkit-4.1.4/src/blobtoolkit.egg-info/SOURCES.txt` & `blobtoolkit-4.1.5/src/blobtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/basic.schema.json` & `blobtoolkit-4.1.5/src/data/schema/basic.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/meta.schema.json` & `blobtoolkit-4.1.5/src/data/schema/meta.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/subschemas/assembly.basic.schema.json` & `blobtoolkit-4.1.5/src/data/schema/subschemas/assembly.basic.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/subschemas/assembly.schema.json` & `blobtoolkit-4.1.5/src/data/schema/subschemas/assembly.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/subschemas/category.data.schema.json` & `blobtoolkit-4.1.5/src/data/schema/subschemas/category.data.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/subschemas/fields.schema.json` & `blobtoolkit-4.1.5/src/data/schema/subschemas/fields.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/subschemas/multiarray.data.schema.json` & `blobtoolkit-4.1.5/src/data/schema/subschemas/multiarray.data.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/subschemas/multiarray.meta.schema.json` & `blobtoolkit-4.1.5/src/data/schema/subschemas/multiarray.meta.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/subschemas/plot.schema.json` & `blobtoolkit-4.1.5/src/data/schema/subschemas/plot.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/subschemas/reads.schema.json` & `blobtoolkit-4.1.5/src/data/schema/subschemas/reads.schema.json`

 * *Files identical despite different names*

### Comparing `blobtoolkit-4.1.4/src/data/schema/subschemas/variable.meta.schema.json` & `blobtoolkit-4.1.5/src/data/schema/subschemas/variable.meta.schema.json`

 * *Files identical despite different names*

