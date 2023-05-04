# Comparing `tmp/ou_tm351_jl_extensions-0.1.0.tar.gz` & `tmp/ou_tm351_jl_extensions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_tm351_jl_extensions-0.1.0.tar", max compression
+gzip compressed data, was "ou_tm351_jl_extensions-0.1.1.tar", max compression
```

## Comparing `ou_tm351_jl_extensions-0.1.0.tar` & `ou_tm351_jl_extensions-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-05-04 16:29:03.023415 ou_tm351_jl_extensions-0.1.0/LICENSE
--rw-r--r--   0        0        0      413 2023-05-04 16:29:03.023415 ou_tm351_jl_extensions-0.1.0/README.md
--rw-r--r--   0        0        0     2388 2023-05-04 16:29:03.023415 ou_tm351_jl_extensions-0.1.0/ou_tm351_jl_extensions/__init__.py
--rw-r--r--   0        0        0      809 2023-05-04 16:29:03.023415 ou_tm351_jl_extensions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-04 19:23:34.100037 ou_tm351_jl_extensions-0.1.1/LICENSE
+-rw-r--r--   0        0        0      413 2023-05-04 19:23:34.100037 ou_tm351_jl_extensions-0.1.1/README.md
+-rw-r--r--   0        0        0     2388 2023-05-04 19:23:34.100037 ou_tm351_jl_extensions-0.1.1/ou_tm351_jl_extensions/__init__.py
+-rw-r--r--   0        0        0      874 2023-05-04 19:23:34.100037 ou_tm351_jl_extensions-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.1.1/PKG-INFO
```

### Comparing `ou_tm351_jl_extensions-0.1.0/LICENSE` & `ou_tm351_jl_extensions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.1.0/ou_tm351_jl_extensions/__init__.py` & `ou_tm351_jl_extensions-0.1.1/ou_tm351_jl_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.1.0/pyproject.toml` & `ou_tm351_jl_extensions-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "ou-tm351-jl-extensions"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Tony Hirst <tony.hirst@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ou_tm351_jl_extensions"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.8,<3.13"
 jupyterlab-ou-brand-extension = "^0.1.0"
 jupyterlab-cell-status-extension = "^0.1.3"
 jupyterlab-myst = "^1.1.3"
 jupyterlab-empinken-extension = "^0.1.1"
 jupyterlab-geojson = "^3.3.1"
 jupyterlab-skip-traceback = "^4.0.4"
 jupyterlab-git = "^0.41.0"
 jupytext = "^1.14.5"
 jupyter-archive = "^3.3.4"
 jupyterlab-spellchecker = "^0.7.3"
 jupyterlab-language-pack-fr-fr = "^3.6.post1"
 jupyterlab-language-pack-zh-cn = "^3.6.post1"
 jupyter-resource-usage = "^0.7.2"
 stickyland = "^0.2.1"
+jupyterlab-tour = "^3.1.4"
+jupyter-compare-view = "^0.2.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ou_tm351_jl_extensions-0.1.0/PKG-INFO` & `ou_tm351_jl_extensions-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: ou-tm351-jl-extensions
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Tony Hirst
 Author-email: tony.hirst@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jupyter-archive (>=3.3.4,<4.0.0)
+Requires-Dist: jupyter-compare-view (>=0.2.4,<0.3.0)
 Requires-Dist: jupyter-resource-usage (>=0.7.2,<0.8.0)
 Requires-Dist: jupyterlab-cell-status-extension (>=0.1.3,<0.2.0)
 Requires-Dist: jupyterlab-empinken-extension (>=0.1.1,<0.2.0)
 Requires-Dist: jupyterlab-geojson (>=3.3.1,<4.0.0)
 Requires-Dist: jupyterlab-git (>=0.41.0,<0.42.0)
 Requires-Dist: jupyterlab-language-pack-fr-fr (>=3.6.post1,<4.0)
 Requires-Dist: jupyterlab-language-pack-zh-cn (>=3.6.post1,<4.0)
 Requires-Dist: jupyterlab-myst (>=1.1.3,<2.0.0)
 Requires-Dist: jupyterlab-ou-brand-extension (>=0.1.0,<0.2.0)
 Requires-Dist: jupyterlab-skip-traceback (>=4.0.4,<5.0.0)
 Requires-Dist: jupyterlab-spellchecker (>=0.7.3,<0.8.0)
+Requires-Dist: jupyterlab-tour (>=3.1.4,<4.0.0)
 Requires-Dist: jupytext (>=1.14.5,<2.0.0)
 Requires-Dist: stickyland (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # ou-tm351-jl-extensions
 
 Recommended JupyterLab extensions for use in the OU TM351 module.
```

