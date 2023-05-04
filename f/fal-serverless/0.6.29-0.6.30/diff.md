# Comparing `tmp/fal_serverless-0.6.29.tar.gz` & `tmp/fal_serverless-0.6.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.29.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.30.tar", max compression
```

## Comparing `fal_serverless-0.6.29.tar` & `fal_serverless-0.6.30.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/README.md
--rw-r--r--   0        0        0      975 2023-04-25 05:36:34.715945 fal_serverless-0.6.29/pyproject.toml
--rw-r--r--   0        0        0      335 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    17406 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2390 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5292 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    11653 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      158 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0      992 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    15210 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     3520 2023-04-25 05:35:11.326628 fal_serverless-0.6.29/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     1530 1970-01-01 00:00:00.000000 fal_serverless-0.6.29/setup.py
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 fal_serverless-0.6.29/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/README.md
+-rw-r--r--   0        0        0      998 2023-05-04 21:44:00.928261 fal_serverless-0.6.30/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    17406 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2390 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5292 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    11653 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0      172 2023-05-04 21:43:52.340291 fal_serverless-0.6.30/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      326 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     1534 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    15210 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     4368 2023-05-04 21:43:37.840340 fal_serverless-0.6.30/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 fal_serverless-0.6.30/setup.py
+-rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 fal_serverless-0.6.30/PKG-INFO
```

### Comparing `fal_serverless-0.6.29/pyproject.toml` & `fal_serverless-0.6.30/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.29"
+version = "0.6.30"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
 isolate = {version = "0.12.0", extras = ["build"]}
 grpcio = "^1.50.0"
 dill = "0.3.5.1"
-isolate-proto = "0.0.27"
+isolate-proto = "^0.0.27"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
 datadog-api-client = "^2.9.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
 colorama = "^0.4.6"
 portalocker = "^2.7.0"
 rich = "^13.3.2"
 
 # For 3.10 and later, importlib-metadata's newer versions are included in the standard library.
 importlib-metadata = { version = ">=4.4", python = "<3.10" }
-packaging = "^23.1"
+packaging = ">=21.3"
+pathspec = "^0.11.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 fal-serverless = "fal_serverless.cli:cli"
```

### Comparing `fal_serverless-0.6.29/src/fal_serverless/api.py` & `fal_serverless-0.6.30/src/fal_serverless/api.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.30/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.30/src/fal_serverless/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.30/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/cli.py` & `fal_serverless-0.6.30/src/fal_serverless/cli.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.30/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.30/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.30/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.30/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.30/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.30/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/sdk.py` & `fal_serverless-0.6.30/src/fal_serverless/sdk.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.29/src/fal_serverless/sync.py` & `fal_serverless-0.6.30/src/fal_serverless/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import hashlib
 import os
 import shutil
 import zipfile
 
+from pathspec import PathSpec
+
 from .api import isolated
 
 CHUNK_SIZE = 1024 * 1024 * 10  # 10 MB
 
 
 def _read_file_chunk(file_path: str, chunk_number: int) -> bytes:
     with open(file_path, "rb") as file:
@@ -58,26 +60,48 @@
 
 
 def _compute_directory_hash(dir_path: str) -> str:
     hash = hashlib.sha256()
     for root, _, files in os.walk(dir_path):
         for file in files:
             file_path = os.path.join(root, file)
-            with open(file_path, "rb") as f:
-                hash.update(f.read())
+            if file != ".fal_hash":
+                with open(file_path, "rb") as f:
+                    hash.update(f.read())
     return hash.hexdigest()
 
 
+def _load_gitignore_patterns(dir_path: str) -> list:
+    # TODO: consider looking at .gitignore files in child directories
+    gitignore_path = os.path.join(dir_path, ".gitignore")
+    if os.path.exists(gitignore_path):
+        with open(gitignore_path) as f:
+            gitignore_patterns = f.read().splitlines()
+    else:
+        gitignore_patterns = []
+    return gitignore_patterns
+
+
+def _is_ignored(file_path: str, gitignore_patterns: list[str]) -> bool:
+    pathspec = PathSpec.from_lines("gitwildmatch", gitignore_patterns)
+    return pathspec.match_file(file_path)
+
+
 def _zip_directory(dir_path: str, zip_path: str) -> None:
+    gitignore_patterns = _load_gitignore_patterns(dir_path)
+
     with zipfile.ZipFile(zip_path, "w", zipfile.ZIP_DEFLATED) as zipf:
         for root, _, files in os.walk(dir_path):
             for file in files:
                 file_path = os.path.join(root, file)
-                arcname = file_path[len(dir_path) :]
-                zipf.write(file_path, arcname)
+                relative_path = os.path.relpath(file_path, dir_path)
+
+                if not _is_ignored(relative_path, gitignore_patterns):
+                    arcname = relative_path
+                    zipf.write(file_path, arcname)
 
 
 def sync_dir(local_dir: str, remote_dir: str, force_upload=False) -> str:
     if not os.path.isabs(remote_dir) or not remote_dir.startswith("/data"):
         raise ValueError(
             "'remote_dir' must be an absolute path starting with `/data`, e.g. '/data/sync/my_dir'"
         )
```

### Comparing `fal_serverless-0.6.29/setup.py` & `fal_serverless-0.6.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,34 +18,35 @@
 ['auth0-python>=4.1.0,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
  'datadog-api-client>=2.9.0,<3.0.0',
  'dill==0.3.5.1',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
- 'isolate-proto==0.0.27',
+ 'isolate-proto>=0.0.27,<0.0.28',
  'isolate[build]==0.12.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
- 'packaging>=23.1,<24.0',
+ 'packaging>=21.3',
+ 'pathspec>=0.11.1,<0.12.0',
  'portalocker>=2.7.0,<3.0.0',
  'requests>=2.28.1,<3.0.0',
  'rich>=13.3.2,<14.0.0',
  'structlog>=22.3.0,<23.0.0',
  'typing-extensions==4.4']
 
 extras_require = \
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.29',
+    'version': '0.6.30',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fal_serverless-0.6.29/PKG-INFO` & `fal_serverless-0.6.30/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.29
+Version: 0.6.30
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,19 +15,20 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: datadog-api-client (>=2.9.0,<3.0.0)
 Requires-Dist: dill (==0.3.5.1)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
-Requires-Dist: isolate-proto (==0.0.27)
+Requires-Dist: isolate-proto (>=0.0.27,<0.0.28)
 Requires-Dist: isolate[build] (==0.12.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
-Requires-Dist: packaging (>=23.1,<24.0)
+Requires-Dist: packaging (>=21.3)
+Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Requires-Dist: typing-extensions (==4.4)
 Description-Content-Type: text/markdown
```

