# Comparing `tmp/sphinx_probs_rdf-0.4.0.tar.gz` & `tmp/sphinx_probs_rdf-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_probs_rdf-0.4.0.tar", last modified: Thu Apr 20 10:10:03 2023, max compression
+gzip compressed data, was "sphinx_probs_rdf-0.4.1.tar", last modified: Thu May  4 19:57:58 2023, max compression
```

## Comparing `sphinx_probs_rdf-0.4.0.tar` & `sphinx_probs_rdf-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.979920 sphinx_probs_rdf-0.4.0/
--rw-r--r--   0 rcl38      (502) staff       (20)     1078 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/LICENSE
--rw-r--r--   0 rcl38      (502) staff       (20)       50 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/MANIFEST.in
--rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-04-20 10:10:03.979978 sphinx_probs_rdf-0.4.0/PKG-INFO
--rw-r--r--   0 rcl38      (502) staff       (20)      485 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/README.rst
--rw-r--r--   0 rcl38      (502) staff       (20)      357 2023-04-20 10:10:03.982246 sphinx_probs_rdf-0.4.0/setup.cfg
--rw-r--r--   0 rcl38      (502) staff       (20)     1718 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/setup.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.963709 sphinx_probs_rdf-0.4.0/src/
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.971367 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/
--rw-r--r--   0 rcl38      (502) staff       (20)     4995 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/__init__.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.975383 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/_static/
--rw-r--r--   0 rcl38      (502) staff       (20)     2007 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/_static/system-definitions.css
--rw-r--r--   0 rcl38      (502) staff       (20)     1236 2023-04-18 17:07:21.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/builder.py
--rw-r--r--   0 rcl38      (502) staff       (20)    30726 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/directives.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1106 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/postprocess.py
--rw-r--r--   0 rcl38      (502) staff       (20)     7867 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/resolve.py
--rw-r--r--   0 rcl38      (502) staff       (20)       27 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/version.py
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.975004 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/
--rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/PKG-INFO
--rw-r--r--   0 rcl38      (502) staff       (20)      805 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 rcl38      (502) staff       (20)        1 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 rcl38      (502) staff       (20)        1 2022-09-21 10:32:32.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/not-zip-safe
--rw-r--r--   0 rcl38      (502) staff       (20)       71 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/requires.txt
--rw-r--r--   0 rcl38      (502) staff       (20)       17 2023-04-20 10:10:03.000000 sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/top_level.txt
-drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-04-20 10:10:03.979363 sphinx_probs_rdf-0.4.0/tests/
--rw-r--r--   0 rcl38      (502) staff       (20)     2843 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/tests/test_directive_options.py
--rw-r--r--   0 rcl38      (502) staff       (20)      661 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/tests/test_missing_process.py
--rw-r--r--   0 rcl38      (502) staff       (20)      892 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/tests/test_postprocess.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1360 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.0/tests/test_probs_rdf_builder_basic.py
--rw-r--r--   0 rcl38      (502) staff       (20)     3989 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/tests/test_probs_rdf_builder_myst.py
--rw-r--r--   0 rcl38      (502) staff       (20)     1204 2023-03-08 21:16:17.000000 sphinx_probs_rdf-0.4.0/tests/test_probs_rdf_builder_prefixes.py
--rw-r--r--   0 rcl38      (502) staff       (20)      848 2023-04-20 10:09:03.000000 sphinx_probs_rdf-0.4.0/tests/test_probs_system_directives.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.970972 sphinx_probs_rdf-0.4.1/
+-rw-r--r--   0 rcl38      (502) staff       (20)     1078 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/LICENSE
+-rw-r--r--   0 rcl38      (502) staff       (20)       50 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/MANIFEST.in
+-rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-05-04 19:57:58.971308 sphinx_probs_rdf-0.4.1/PKG-INFO
+-rw-r--r--   0 rcl38      (502) staff       (20)      485 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/README.rst
+-rw-r--r--   0 rcl38      (502) staff       (20)      357 2023-05-04 19:57:58.981897 sphinx_probs_rdf-0.4.1/setup.cfg
+-rw-r--r--   0 rcl38      (502) staff       (20)     1718 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/setup.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.879456 sphinx_probs_rdf-0.4.1/src/
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.892973 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/
+-rw-r--r--   0 rcl38      (502) staff       (20)     5019 2023-05-04 19:48:17.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/__init__.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.908862 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/_static/
+-rw-r--r--   0 rcl38      (502) staff       (20)     2007 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/_static/system-definitions.css
+-rw-r--r--   0 rcl38      (502) staff       (20)     1236 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/builder.py
+-rw-r--r--   0 rcl38      (502) staff       (20)    30726 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/directives.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1106 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/postprocess.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     7867 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/resolve.py
+-rw-r--r--   0 rcl38      (502) staff       (20)       27 2023-05-04 19:56:17.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/version.py
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.903427 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/
+-rw-r--r--   0 rcl38      (502) staff       (20)     1238 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 rcl38      (502) staff       (20)      805 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)        1 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)        1 2022-09-21 10:32:32.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 rcl38      (502) staff       (20)       71 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/requires.txt
+-rw-r--r--   0 rcl38      (502) staff       (20)       17 2023-05-04 19:57:58.000000 sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/top_level.txt
+drwxr-xr-x   0 rcl38      (502) staff       (20)        0 2023-05-04 19:57:58.965264 sphinx_probs_rdf-0.4.1/tests/
+-rw-r--r--   0 rcl38      (502) staff       (20)     2843 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/tests/test_directive_options.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      661 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/tests/test_missing_process.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      892 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/tests/test_postprocess.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1360 2022-09-21 10:31:49.000000 sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_basic.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     3989 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_myst.py
+-rw-r--r--   0 rcl38      (502) staff       (20)     1204 2023-03-08 21:16:17.000000 sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_prefixes.py
+-rw-r--r--   0 rcl38      (502) staff       (20)      848 2023-04-20 10:12:09.000000 sphinx_probs_rdf-0.4.1/tests/test_probs_system_directives.py
```

### Comparing `sphinx_probs_rdf-0.4.0/LICENSE` & `sphinx_probs_rdf-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/PKG-INFO` & `sphinx_probs_rdf-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_probs_rdf
-Version: 0.4.0
+Version: 0.4.1
 Summary: sphinx_probs_rdf is a sphinx extension which outputs RDF describing Processes and Objects using the PRObs ontology.
 Home-page: https://github.com/ricklupton/sphinx_probs_rdf
 Download-URL: https://pypi.org/project/sphinx_probs_rdf/
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 License: BSD
 Platform: any
```

### Comparing `sphinx_probs_rdf-0.4.0/setup.py` & `sphinx_probs_rdf-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/__init__.py` & `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 def read_external_graph(app: Sphinx, env):
     """Read in any data from external RDF files."""
     paths = env.config.probs_rdf_paths
     domain = cast(SystemDomain, env.get_domain("system"))
     g = domain.graph
     for p in paths:
-        domain.graph.parse(location=p, format="ttl")
+        domain.graph.parse(location=path.join(app.confdir, p), format="ttl")
 
     # Check if the external graph has duplicated any of our own prefix
     # definitions
     seen = set()
     bound_namespaces = list(g.namespace_manager.namespaces())
     g.namespace_manager.reset()
     for prefix, ns in bound_namespaces:
```

### Comparing `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/_static/system-definitions.css` & `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/_static/system-definitions.css`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/builder.py` & `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/builder.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/directives.py` & `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/directives.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/postprocess.py` & `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf/resolve.py` & `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf/resolve.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/PKG-INFO` & `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-probs-rdf
-Version: 0.4.0
+Version: 0.4.1
 Summary: sphinx_probs_rdf is a sphinx extension which outputs RDF describing Processes and Objects using the PRObs ontology.
 Home-page: https://github.com/ricklupton/sphinx_probs_rdf
 Download-URL: https://pypi.org/project/sphinx_probs_rdf/
 Author: Rick Lupton
 Author-email: mail@ricklupton.name
 License: BSD
 Platform: any
```

### Comparing `sphinx_probs_rdf-0.4.0/src/sphinx_probs_rdf.egg-info/SOURCES.txt` & `sphinx_probs_rdf-0.4.1/src/sphinx_probs_rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/tests/test_directive_options.py` & `sphinx_probs_rdf-0.4.1/tests/test_directive_options.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/tests/test_missing_process.py` & `sphinx_probs_rdf-0.4.1/tests/test_missing_process.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/tests/test_postprocess.py` & `sphinx_probs_rdf-0.4.1/tests/test_postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/tests/test_probs_rdf_builder_basic.py` & `sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_basic.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/tests/test_probs_rdf_builder_myst.py` & `sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_myst.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/tests/test_probs_rdf_builder_prefixes.py` & `sphinx_probs_rdf-0.4.1/tests/test_probs_rdf_builder_prefixes.py`

 * *Files identical despite different names*

### Comparing `sphinx_probs_rdf-0.4.0/tests/test_probs_system_directives.py` & `sphinx_probs_rdf-0.4.1/tests/test_probs_system_directives.py`

 * *Files identical despite different names*

