# Comparing `tmp/network-analysis-0.0.2.tar.gz` & `tmp/network-analysis-0.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-analysis-0.0.2.tar", last modified: Thu May  4 16:43:36 2023, max compression
+gzip compressed data, was "network-analysis-0.0.2b0.tar", last modified: Thu May  4 17:17:19 2023, max compression
```

## Comparing `network-analysis-0.0.2.tar` & `network-analysis-0.0.2b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:43:36.947199 network-analysis-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 16:43:20.000000 network-analysis-0.0.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 16:43:36.947199 network-analysis-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:43:20.000000 network-analysis-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-04 16:43:20.000000 network-analysis-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:43:36.947199 network-analysis-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:43:36.943199 network-analysis-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:43:36.943199 network-analysis-0.0.2/src/network_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-04 16:43:36.000000 network-analysis-0.0.2/src/network_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-04 16:43:36.000000 network-analysis-0.0.2/src/network_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:43:36.000000 network-analysis-0.0.2/src/network_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 16:43:36.000000 network-analysis-0.0.2/src/network_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:43:36.947199 network-analysis-0.0.2/src/networkanalysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:43:20.000000 network-analysis-0.0.2/src/networkanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:43:36.947199 network-analysis-0.0.2/src/networkanalysis/ergm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:43:20.000000 network-analysis-0.0.2/src/networkanalysis/ergm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-04 16:43:20.000000 network-analysis-0.0.2/src/networkanalysis/ergm/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-04 16:43:20.000000 network-analysis-0.0.2/src/networkanalysis/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:43:36.947199 network-analysis-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-04 16:43:20.000000 network-analysis-0.0.2/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:17:19.739821 network-analysis-0.0.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 17:17:02.000000 network-analysis-0.0.2b0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-04 17:17:19.739821 network-analysis-0.0.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:17:02.000000 network-analysis-0.0.2b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-04 17:17:02.000000 network-analysis-0.0.2b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:17:19.739821 network-analysis-0.0.2b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:17:19.739821 network-analysis-0.0.2b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:17:19.739821 network-analysis-0.0.2b0/src/network_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-04 17:17:19.000000 network-analysis-0.0.2b0/src/network_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-04 17:17:19.000000 network-analysis-0.0.2b0/src/network_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:17:19.000000 network-analysis-0.0.2b0/src/network_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 17:17:19.000000 network-analysis-0.0.2b0/src/network_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:17:19.739821 network-analysis-0.0.2b0/src/networkanalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:17:02.000000 network-analysis-0.0.2b0/src/networkanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:17:19.739821 network-analysis-0.0.2b0/src/networkanalysis/ergm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 17:17:02.000000 network-analysis-0.0.2b0/src/networkanalysis/ergm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-04 17:17:02.000000 network-analysis-0.0.2b0/src/networkanalysis/ergm/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-04 17:17:02.000000 network-analysis-0.0.2b0/src/networkanalysis/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:17:19.739821 network-analysis-0.0.2b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-04 17:17:02.000000 network-analysis-0.0.2b0/tests/test_statistics.py
```

### Comparing `network-analysis-0.0.2/LICENCE` & `network-analysis-0.0.2b0/LICENCE`

 * *Files identical despite different names*

### Comparing `network-analysis-0.0.2/PKG-INFO` & `network-analysis-0.0.2b0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-analysis
-Version: 0.0.2
+Version: 0.0.2b0
 Summary: Work in progress...
 Author-email: Gabriel Fortin-Leblanc <gabriel.fortin-leblanc@umontreal.ca>
 Project-URL: Homepage, https://github.com/gabriel-fortin-leblanc/network-analysis
 Project-URL: Bug Tracker, https://github.com/gabriel-fortin-leblanc/network-analysis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `network-analysis-0.0.2/pyproject.toml` & `network-analysis-0.0.2b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "network-analysis"
-version = "0.0.2"
+version = "0.0.2-beta"
 authors = [
   { name="Gabriel Fortin-Leblanc", email="gabriel.fortin-leblanc@umontreal.ca" },
 ]
 description = "Work in progress..."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `network-analysis-0.0.2/src/network_analysis.egg-info/PKG-INFO` & `network-analysis-0.0.2b0/src/network_analysis.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-analysis
-Version: 0.0.2
+Version: 0.0.2b0
 Summary: Work in progress...
 Author-email: Gabriel Fortin-Leblanc <gabriel.fortin-leblanc@umontreal.ca>
 Project-URL: Homepage, https://github.com/gabriel-fortin-leblanc/network-analysis
 Project-URL: Bug Tracker, https://github.com/gabriel-fortin-leblanc/network-analysis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `network-analysis-0.0.2/src/networkanalysis/ergm/simulate.py` & `network-analysis-0.0.2b0/src/networkanalysis/ergm/simulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     :type ngraphs: Integer.
     :param param: The parameter of the model.
     :type param: Numpy array.
     :param stats_comp: The sufficient statistics computer.
     :type stats_comp: A callable object.
     :param init: The initial graph to start the chain, or the number of nodes.
     :type init: NetworkX graph., optional
-    :param burnin: The number of graphs to burn. If none is given, then no graphs will be burned., defaults to None
+    :param burnin: The number of graphs to burn. If none is given, then no
+    graphs will be burned., defaults to None
     :type burnin: _type_, optional
     """
     if type(init) is int:
         peek = nx.random_graphs.binomial_graph(init, 0.5)
     else:
         peek = init.copy()
     peek_stats = stats_comp(peek)
@@ -46,15 +47,15 @@
         )
 
     graphs = list()
     for _ in range(ngraphs):
         peek, peek_stats = _next_state(
             peek, peek_stats, stats_comp, param, nodes
         )
-        graphs.append(peek)
+        graphs.append(peek.copy())
 
     return graphs
 
 
 def _next_state(peek, peek_stats, stats_comp, param, nodes):
     u, v = random.sample(nodes, 2)
     in_graph = peek.has_edge(u, v)
```

### Comparing `network-analysis-0.0.2/src/networkanalysis/statistics.py` & `network-analysis-0.0.2b0/src/networkanalysis/statistics.py`

 * *Files identical despite different names*

### Comparing `network-analysis-0.0.2/tests/test_statistics.py` & `network-analysis-0.0.2b0/tests/test_statistics.py`

 * *Files identical despite different names*

