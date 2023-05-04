# Comparing `tmp/auto_retrieval_plugin-0.1.0.tar.gz` & `tmp/auto_retrieval_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_retrieval_plugin-0.1.0.tar", max compression
+gzip compressed data, was "auto_retrieval_plugin-0.1.1.tar", max compression
```

## Comparing `auto_retrieval_plugin-0.1.0.tar` & `auto_retrieval_plugin-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1063 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/LICENSE
--rw-r--r--   0        0        0     4144 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/README.md
--rw-r--r--   0        0        0      760 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/.well-known/ai-plugin.json
--rw-r--r--   0        0        0      760 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/.well-known/default-ai-plugin.json
--rw-r--r--   0        0        0      836 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/.well-known/logo.png
--rw-r--r--   0        0        0     4737 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/.well-known/openapi.yaml
--rw-r--r--   0        0        0        0 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/__init__.py
--rw-r--r--   0        0        0       98 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/config.yml
--rw-r--r--   0        0        0        0 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/__init__.py
--rw-r--r--   0        0        0     3070 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/datastore.py
--rw-r--r--   0        0        0      143 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/executor/Dockerfile
--rw-r--r--   0        0        0        0 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/executor/__init__.py
--rw-r--r--   0        0        0      161 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/executor/config.yml
--rw-r--r--   0        0        0     3193 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/executor/docarray_v1.py
--rw-r--r--   0        0        0     1284 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/factory.py
--rw-r--r--   0        0        0      777 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/flow.yml
--rw-r--r--   0        0        0    11289 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/gateway.py
--rw-r--r--   0        0        0        0 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/models/__init__.py
--rw-r--r--   0        0        0      642 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/models/api.py
--rw-r--r--   0        0        0     1460 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/models/models.py
--rw-r--r--   0        0        0     9949 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/retrieval_plugin.py
--rw-r--r--   0        0        0        0 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/__init__.py
--rw-r--r--   0        0        0     3016 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_json/README.md
--rw-r--r--   0        0        0        0 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_json/__init__.py
--rw-r--r--   0        0        0      630 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_json/example.json
--rw-r--r--   0        0        0     5396 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_json/process_json.py
--rw-r--r--   0        0        0     3091 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_jsonl/README.md
--rw-r--r--   0        0        0        0 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_jsonl/__init__.py
--rw-r--r--   0        0        0      879 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_jsonl/example.jsonl
--rw-r--r--   0        0        0     5293 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_jsonl/process_jsonl.py
--rw-r--r--   0        0        0     2699 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_zip/README.md
--rw-r--r--   0        0        0        0 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_zip/__init__.py
--rw-r--r--   0        0        0    53296 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_zip/example.zip
--rw-r--r--   0        0        0     5716 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_zip/process_zip.py
--rw-r--r--   0        0        0        0 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/__init__.py
--rw-r--r--   0        0        0     7625 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/chunks.py
--rw-r--r--   0        0        0      793 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/date.py
--rw-r--r--   0        0        0     1217 2023-05-04 09:18:30.434020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/extract_metadata.py
--rw-r--r--   0        0        0     3682 2023-05-04 09:18:30.438020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/file.py
--rw-r--r--   0        0        0     1879 2023-05-04 09:18:30.438020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/openai.py
--rw-r--r--   0        0        0     1358 2023-05-04 09:18:30.438020 auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/pii_detection.py
--rw-r--r--   0        0        0     1025 2023-05-04 09:18:30.438020 auto_retrieval_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5460 1970-01-01 00:00:00.000000 auto_retrieval_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4144 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0      760 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/.well-known/ai-plugin.json
+-rw-r--r--   0        0        0      760 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/.well-known/default-ai-plugin.json
+-rw-r--r--   0        0        0      836 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/.well-known/logo.png
+-rw-r--r--   0        0        0     4737 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/.well-known/openapi.yaml
+-rw-r--r--   0        0        0        0 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/__init__.py
+-rw-r--r--   0        0        0       98 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/config.yml
+-rw-r--r--   0        0        0        0 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/__init__.py
+-rw-r--r--   0        0        0     3070 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/datastore.py
+-rw-r--r--   0        0        0      143 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/executor/Dockerfile
+-rw-r--r--   0        0        0        0 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/executor/__init__.py
+-rw-r--r--   0        0        0      161 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/executor/config.yml
+-rw-r--r--   0        0        0     3193 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/executor/docarray_v1.py
+-rw-r--r--   0        0        0     1284 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/factory.py
+-rw-r--r--   0        0        0      777 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/flow.yml
+-rw-r--r--   0        0        0    11289 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/gateway.py
+-rw-r--r--   0        0        0        0 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/models/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-04 09:37:26.329742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/models/api.py
+-rw-r--r--   0        0        0     1460 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/models/models.py
+-rw-r--r--   0        0        0     9971 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/retrieval_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/__init__.py
+-rw-r--r--   0        0        0     3016 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_json/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_json/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_json/example.json
+-rw-r--r--   0        0        0     5396 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_json/process_json.py
+-rw-r--r--   0        0        0     3091 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_jsonl/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_jsonl/__init__.py
+-rw-r--r--   0        0        0      879 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_jsonl/example.jsonl
+-rw-r--r--   0        0        0     5293 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_jsonl/process_jsonl.py
+-rw-r--r--   0        0        0     2699 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_zip/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_zip/__init__.py
+-rw-r--r--   0        0        0    53296 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_zip/example.zip
+-rw-r--r--   0        0        0     5716 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_zip/process_zip.py
+-rw-r--r--   0        0        0        0 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/__init__.py
+-rw-r--r--   0        0        0     7625 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/chunks.py
+-rw-r--r--   0        0        0      793 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/date.py
+-rw-r--r--   0        0        0     1217 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/extract_metadata.py
+-rw-r--r--   0        0        0     3682 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/file.py
+-rw-r--r--   0        0        0     1879 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/openai.py
+-rw-r--r--   0        0        0     1358 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/pii_detection.py
+-rw-r--r--   0        0        0     1025 2023-05-04 09:37:26.333742 auto_retrieval_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5460 1970-01-01 00:00:00.000000 auto_retrieval_plugin-0.1.1/PKG-INFO
```

### Comparing `auto_retrieval_plugin-0.1.0/LICENSE` & `auto_retrieval_plugin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/README.md` & `auto_retrieval_plugin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/.well-known/ai-plugin.json` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/.well-known/ai-plugin.json`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/.well-known/default-ai-plugin.json` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/.well-known/default-ai-plugin.json`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/.well-known/logo.png` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/.well-known/logo.png`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/.well-known/openapi.yaml` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/.well-known/openapi.yaml`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/datastore.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/executor/docarray_v1.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/executor/docarray_v1.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/datastore/factory.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/datastore/factory.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/flow.yml` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/flow.yml`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/gateway.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/gateway.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/models/api.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/models/api.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/models/models.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/models/models.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/retrieval_plugin.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/retrieval_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import typer
 from docarray import DocumentArray
 from hubble.api import login as login_jina
 from jcloud.api import deploy as deploy_flow
 from jcloud.flow import CloudFlow
 
 app = typer.Typer()
-FLOW_PATH = 'flow.yml'
+FLOW_PATH = 'auto_retrieval_plugin/flow.yml'
 
 
 class UnsupportedExtensionError(Exception):
     pass
 
 
 class EmptyDirectoryError(Exception):
```

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_json/README.md` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_json/README.md`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_json/example.json` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_json/example.json`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_json/process_json.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_json/process_json.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_jsonl/README.md` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_jsonl/README.md`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_jsonl/example.jsonl` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_jsonl/example.jsonl`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_jsonl/process_jsonl.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_jsonl/process_jsonl.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_zip/README.md` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_zip/README.md`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_zip/example.zip` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_zip/example.zip`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/scripts/process_zip/process_zip.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/scripts/process_zip/process_zip.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/chunks.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/chunks.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/date.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/date.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/extract_metadata.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/extract_metadata.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/file.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/file.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/openai.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/openai.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/auto_retrieval_plugin/services/pii_detection.py` & `auto_retrieval_plugin-0.1.1/auto_retrieval_plugin/services/pii_detection.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.0/pyproject.toml` & `auto_retrieval_plugin-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-retrieval-plugin"
-version = "0.1.0"
+version = "0.1.1"
 description = "Create and host retrieval plugins for ChatGPT in one click"
 authors = ["saba <saba.sturua@jina.ai>", "johannes johannes.messner@jina.ai"]
 readme = "README.md"
 include = ["auto_retrieval_plugin/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `auto_retrieval_plugin-0.1.0/PKG-INFO` & `auto_retrieval_plugin-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-retrieval-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Create and host retrieval plugins for ChatGPT in one click
 Author: saba
 Author-email: saba.sturua@jina.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

