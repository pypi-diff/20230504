# Comparing `tmp/mkdocs-entangled-plugin-0.1.0.tar.gz` & `tmp/mkdocs_entangled_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-entangled-plugin-0.1.0.tar", max compression
+gzip compressed data, was "mkdocs_entangled_plugin-0.2.0.tar", max compression
```

## Comparing `mkdocs-entangled-plugin-0.1.0.tar` & `mkdocs_entangled_plugin-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-11 13:56:19.460432 mkdocs-entangled-plugin-0.1.0/LICENSE
--rw-r--r--   0        0        0      910 2023-04-11 13:11:58.594143 mkdocs-entangled-plugin-0.1.0/README.md
--rw-r--r--   0        0        0       67 2023-04-11 12:37:11.656249 mkdocs-entangled-plugin-0.1.0/mkdocs_entangled/__init__.py
--rw-r--r--   0        0        0       79 2023-04-11 11:51:46.359682 mkdocs-entangled-plugin-0.1.0/mkdocs_entangled/config.py
--rw-r--r--   0        0        0     1519 2023-04-11 13:05:58.213092 mkdocs-entangled-plugin-0.1.0/mkdocs_entangled/mawk.py
--rw-r--r--   0        0        0     1173 2023-04-11 12:50:05.788664 mkdocs-entangled-plugin-0.1.0/mkdocs_entangled/on_page_markdown.py
--rw-r--r--   0        0        0      474 2023-04-11 11:50:06.214109 mkdocs-entangled-plugin-0.1.0/mkdocs_entangled/plugin.py
--rw-r--r--   0        0        0     2892 2023-04-11 12:23:16.750490 mkdocs-entangled-plugin-0.1.0/mkdocs_entangled/properties.py
--rw-r--r--   0        0        0        0 2023-04-11 08:08:07.687520 mkdocs-entangled-plugin-0.1.0/mkdocs_entangled/py.typed
--rw-r--r--   0        0        0      797 2023-04-11 13:56:53.325420 mkdocs-entangled-plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1771 2023-04-11 13:57:00.654425 mkdocs-entangled-plugin-0.1.0/setup.py
--rw-r--r--   0        0        0     1555 2023-04-11 13:57:00.654922 mkdocs-entangled-plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-03 23:56:27.577268 mkdocs_entangled_plugin-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1462 2023-05-03 23:56:27.577268 mkdocs_entangled_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0       67 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/config.py
+-rw-r--r--   0        0        0     3191 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/mawk.py
+-rw-r--r--   0        0        0     3007 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/on_page_markdown.py
+-rw-r--r--   0        0        0      474 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/plugin.py
+-rw-r--r--   0        0        0     2892 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/properties.py
+-rw-r--r--   0        0        0        0 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/py.typed
+-rw-r--r--   0        0        0      814 2023-05-03 23:56:27.581268 mkdocs_entangled_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 mkdocs_entangled_plugin-0.2.0/PKG-INFO
```

### Comparing `mkdocs-entangled-plugin-0.1.0/LICENSE` & `mkdocs_entangled_plugin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-entangled-plugin-0.1.0/mkdocs_entangled/properties.py` & `mkdocs_entangled_plugin-0.2.0/mkdocs_entangled/properties.py`

 * *Files identical despite different names*

### Comparing `mkdocs-entangled-plugin-0.1.0/pyproject.toml` & `mkdocs_entangled_plugin-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-entangled-plugin"
-version = "0.1.0"
+version = "0.2.0"
 description = "Plugin for MkDocs helping with rendering Entangled (entangled.github.io) projects."
 readme = "README.md"
 authors = ["Johan Hidding <j.hidding@esciencecenter.nl>"]
 license = "Apache 2.0"
 packages = [
     { include = "mkdocs_entangled" }
 ]
@@ -17,14 +17,15 @@
 mkdocs = "^1.4.2"
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.2.0"
 pytest = "^7.3.0"
 pytest-mypy = "^0.10.3"
 mkdocs-material = "^9.1.6"
+twine = "^4.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = ["--mypy"]
```

