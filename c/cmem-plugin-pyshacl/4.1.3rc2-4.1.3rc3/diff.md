# Comparing `tmp/cmem_plugin_pyshacl-4.1.3rc2.tar.gz` & `tmp/cmem_plugin_pyshacl-4.1.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_pyshacl-4.1.3rc2.tar", max compression
+gzip compressed data, was "cmem_plugin_pyshacl-4.1.3rc3.tar", max compression
```

## Comparing `cmem_plugin_pyshacl-4.1.3rc2.tar` & `cmem_plugin_pyshacl-4.1.3rc3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11334 2023-05-04 11:24:17.401636 cmem_plugin_pyshacl-4.1.3rc2/LICENSE
--rw-r--r--   0        0        0     4970 2023-05-04 11:24:17.401636 cmem_plugin_pyshacl-4.1.3rc2/README-public.md
--rwxr-xr-x   0        0        0       46 2023-05-04 11:24:43.282086 cmem_plugin_pyshacl-4.1.3rc2/cmem_plugin_pyshacl/__init__.py
--rw-r--r--   0        0        0    27921 2023-05-04 11:24:17.401636 cmem_plugin_pyshacl-4.1.3rc2/cmem_plugin_pyshacl/plugin_pyshacl.py
--rw-r--r--   0        0        0     1875 2023-05-04 11:24:43.278086 cmem_plugin_pyshacl-4.1.3rc2/pyproject.toml
--rw-r--r--   0        0        0     6342 1970-01-01 00:00:00.000000 cmem_plugin_pyshacl-4.1.3rc2/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-05-04 11:26:42.509509 cmem_plugin_pyshacl-4.1.3rc3/LICENSE
+-rw-r--r--   0        0        0     4698 2023-05-04 11:26:42.509509 cmem_plugin_pyshacl-4.1.3rc3/README-public.md
+-rwxr-xr-x   0        0        0       46 2023-05-04 11:27:17.857667 cmem_plugin_pyshacl-4.1.3rc3/cmem_plugin_pyshacl/__init__.py
+-rw-r--r--   0        0        0    27921 2023-05-04 11:26:42.509509 cmem_plugin_pyshacl-4.1.3rc3/cmem_plugin_pyshacl/plugin_pyshacl.py
+-rw-r--r--   0        0        0     1875 2023-05-04 11:27:17.857667 cmem_plugin_pyshacl-4.1.3rc3/pyproject.toml
+-rw-r--r--   0        0        0     6070 1970-01-01 00:00:00.000000 cmem_plugin_pyshacl-4.1.3rc3/PKG-INFO
```

### Comparing `cmem_plugin_pyshacl-4.1.3rc2/LICENSE` & `cmem_plugin_pyshacl-4.1.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_pyshacl-4.1.3rc2/README-public.md` & `cmem_plugin_pyshacl-4.1.3rc3/README-public.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,14 @@
 
 ```
 cmemc admin workspace python install cmem-plugin-pyshacl
 ```
 
 [![eccenca Corporate Memory](https://img.shields.io/badge/eccenca-Corporate%20Memory-orange)](https://documentation.eccenca.com)
 
-## Development
-
-- Run [task](https://taskfile.dev/) to see all major development tasks.
-- Use [pre-commit](https://pre-commit.com/) to avoid errors before commit.
-- This repository was created with [this copier template](https://github.com/eccenca/cmem-plugin-template).
-
 ## Options
 
 ### Data graph URI
 
 The URI of the graph to be validated. The graph URI is selected from a list of graphs of types:
 - `di:Dataset`
 - `dsm:ThesaurusProject`
```

### Comparing `cmem_plugin_pyshacl-4.1.3rc2/cmem_plugin_pyshacl/plugin_pyshacl.py` & `cmem_plugin_pyshacl-4.1.3rc3/cmem_plugin_pyshacl/plugin_pyshacl.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_pyshacl-4.1.3rc2/pyproject.toml` & `cmem_plugin_pyshacl-4.1.3rc3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-pyshacl"
-version = "4.1.3rc2"
+version = "4.1.3rc3"
 license = "Apache-2.0"
 description = "Validate your Knowledge Graphs based on tests generated from SHACL shapes."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `cmem_plugin_pyshacl-4.1.3rc2/PKG-INFO` & `cmem_plugin_pyshacl-4.1.3rc3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-pyshacl
-Version: 4.1.3rc2
+Version: 4.1.3rc3
 Summary: Validate your Knowledge Graphs based on tests generated from SHACL shapes.
 Home-page: https://github.com/eccenca/cmem-plugin-pyshacl
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,SHACL
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
@@ -38,20 +38,14 @@
 
 ```
 cmemc admin workspace python install cmem-plugin-pyshacl
 ```
 
 [![eccenca Corporate Memory](https://img.shields.io/badge/eccenca-Corporate%20Memory-orange)](https://documentation.eccenca.com)
 
-## Development
-
-- Run [task](https://taskfile.dev/) to see all major development tasks.
-- Use [pre-commit](https://pre-commit.com/) to avoid errors before commit.
-- This repository was created with [this copier template](https://github.com/eccenca/cmem-plugin-template).
-
 ## Options
 
 ### Data graph URI
 
 The URI of the graph to be validated. The graph URI is selected from a list of graphs of types:
 - `di:Dataset`
 - `dsm:ThesaurusProject`
```

