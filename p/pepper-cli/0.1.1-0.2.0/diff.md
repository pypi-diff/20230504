# Comparing `tmp/pepper_cli-0.1.1.tar.gz` & `tmp/pepper_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepper_cli-0.1.1.tar", max compression
+gzip compressed data, was "pepper_cli-0.2.0.tar", max compression
```

## Comparing `pepper_cli-0.1.1.tar` & `pepper_cli-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1137 2023-04-14 03:09:12.769659 pepper_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0     4367 2023-04-14 03:09:12.769659 pepper_cli-0.1.1/README.md
--rw-r--r--   0        0        0    15389 2023-04-14 03:09:12.769659 pepper_cli-0.1.1/pepper_cli.py
--rw-r--r--   0        0        0      763 2023-04-14 03:09:12.769659 pepper_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4963 1970-01-01 00:00:00.000000 pepper_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-05-04 08:17:24.923856 pepper_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4367 2023-05-04 08:17:24.923856 pepper_cli-0.2.0/README.md
+-rw-r--r--   0        0        0    23251 2023-05-04 08:17:24.927856 pepper_cli-0.2.0/pepper_cli.py
+-rw-r--r--   0        0        0      828 2023-05-04 08:17:24.927856 pepper_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5030 1970-01-01 00:00:00.000000 pepper_cli-0.2.0/PKG-INFO
```

### Comparing `pepper_cli-0.1.1/LICENSE` & `pepper_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pepper_cli-0.1.1/README.md` & `pepper_cli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pepper_cli-0.1.1/pyproject.toml` & `pepper_cli-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "pepper-cli"
-version = "0.1.1"
+version = "0.2.0"
 description = "Get information about any PEP (Python Enhancement Proposal)"
 authors = ["Noah Tanner <50159154+kevinshome@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pywebview = { version = "*", optional = true }
 black = { version = "*", optional = true }
+bottle = { version = "*", optional = true }
 
 [tool.poetry.group.webview]
 optional = true
 
 [tool.poetry.group.dev]
 optional = true
 
@@ -24,12 +25,13 @@
 black = "*"
 
 [tool.poetry.scripts]
 pepper = "pepper_cli:main"
 
 [tool.poetry.extras]
 webview = ["pywebview"]
+offline = ["bottle"]
 dev = ["black"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pepper_cli-0.1.1/PKG-INFO` & `pepper_cli-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pepper-cli
-Version: 0.1.1
+Version: 0.2.0
 Summary: Get information about any PEP (Python Enhancement Proposal)
 License: MIT
 Author: Noah Tanner
 Author-email: 50159154+kevinshome@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
+Provides-Extra: offline
 Provides-Extra: webview
 Requires-Dist: black ; extra == "dev"
+Requires-Dist: bottle ; extra == "offline"
 Requires-Dist: pywebview ; extra == "webview"
 Description-Content-Type: text/markdown
 
 <img src="https://commedesgarcons.s-ul.eu/8NolAhU8" width="54%"></img> 
 <img src="https://commedesgarcons.s-ul.eu/FgxMAvXS" width="45%"></img> 
 
 <div align="center">
```

