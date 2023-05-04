# Comparing `tmp/auto_retrieval_plugin-0.1.2.tar.gz` & `tmp/auto_retrieval_plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_retrieval_plugin-0.1.2.tar", max compression
+gzip compressed data, was "auto_retrieval_plugin-0.1.3.tar", max compression
```

## Comparing `auto_retrieval_plugin-0.1.2.tar` & `auto_retrieval_plugin-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1063 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/LICENSE
--rw-r--r--   0        0        0     4144 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/README.md
--rw-r--r--   0        0        0      760 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/.well-known/ai-plugin.json
--rw-r--r--   0        0        0      760 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/.well-known/default-ai-plugin.json
--rw-r--r--   0        0        0      836 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/.well-known/logo.png
--rw-r--r--   0        0        0     4737 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/.well-known/openapi.yaml
--rw-r--r--   0        0        0        0 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/__init__.py
--rw-r--r--   0        0        0       98 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/config.yml
--rw-r--r--   0        0        0        0 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/__init__.py
--rw-r--r--   0        0        0     3070 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/datastore.py
--rw-r--r--   0        0        0      143 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/executor/Dockerfile
--rw-r--r--   0        0        0        0 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/executor/__init__.py
--rw-r--r--   0        0        0      161 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/executor/config.yml
--rw-r--r--   0        0        0     3193 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/executor/docarray_v1.py
--rw-r--r--   0        0        0     1284 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/factory.py
--rw-r--r--   0        0        0      777 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/flow.yml
--rw-r--r--   0        0        0    11289 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/gateway.py
--rw-r--r--   0        0        0        0 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/models/__init__.py
--rw-r--r--   0        0        0      642 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/models/api.py
--rw-r--r--   0        0        0     1460 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/models/models.py
--rw-r--r--   0        0        0    10022 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/retrieval_plugin.py
--rw-r--r--   0        0        0        0 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/__init__.py
--rw-r--r--   0        0        0     3016 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_json/README.md
--rw-r--r--   0        0        0        0 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_json/__init__.py
--rw-r--r--   0        0        0      630 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_json/example.json
--rw-r--r--   0        0        0     5396 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_json/process_json.py
--rw-r--r--   0        0        0     3091 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_jsonl/README.md
--rw-r--r--   0        0        0        0 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_jsonl/__init__.py
--rw-r--r--   0        0        0      879 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_jsonl/example.jsonl
--rw-r--r--   0        0        0     5293 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_jsonl/process_jsonl.py
--rw-r--r--   0        0        0     2699 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_zip/README.md
--rw-r--r--   0        0        0        0 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_zip/__init__.py
--rw-r--r--   0        0        0    53296 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_zip/example.zip
--rw-r--r--   0        0        0     5716 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_zip/process_zip.py
--rw-r--r--   0        0        0        0 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/__init__.py
--rw-r--r--   0        0        0     7625 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/chunks.py
--rw-r--r--   0        0        0      793 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/date.py
--rw-r--r--   0        0        0     1217 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/extract_metadata.py
--rw-r--r--   0        0        0     3682 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/file.py
--rw-r--r--   0        0        0     1879 2023-05-04 11:14:40.698602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/openai.py
--rw-r--r--   0        0        0     1358 2023-05-04 11:14:40.702602 auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/pii_detection.py
--rw-r--r--   0        0        0     1025 2023-05-04 11:14:40.702602 auto_retrieval_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5460 1970-01-01 00:00:00.000000 auto_retrieval_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4144 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0      286 2023-05-04 11:32:00.439164 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/.env
+-rw-r--r--   0        0        0      760 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/.well-known/ai-plugin.json
+-rw-r--r--   0        0        0      760 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/.well-known/default-ai-plugin.json
+-rw-r--r--   0        0        0      836 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/.well-known/logo.png
+-rw-r--r--   0        0        0     4737 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/.well-known/openapi.yaml
+-rw-r--r--   0        0        0        0 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/__init__.py
+-rw-r--r--   0        0        0       98 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/config.yml
+-rw-r--r--   0        0        0        0 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/__init__.py
+-rw-r--r--   0        0        0     3070 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/datastore.py
+-rw-r--r--   0        0        0      143 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/executor/Dockerfile
+-rw-r--r--   0        0        0        0 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/executor/__init__.py
+-rw-r--r--   0        0        0      161 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/executor/config.yml
+-rw-r--r--   0        0        0     3193 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/executor/docarray_v1.py
+-rw-r--r--   0        0        0     1284 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/factory.py
+-rw-r--r--   0        0        0      777 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/flow.yml
+-rw-r--r--   0        0        0    11289 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/gateway.py
+-rw-r--r--   0        0        0        0 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/models/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/models/api.py
+-rw-r--r--   0        0        0     1460 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/models/models.py
+-rw-r--r--   0        0        0    10092 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/retrieval_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/__init__.py
+-rw-r--r--   0        0        0     3016 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_json/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_json/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_json/example.json
+-rw-r--r--   0        0        0     5396 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_json/process_json.py
+-rw-r--r--   0        0        0     3091 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_jsonl/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_jsonl/__init__.py
+-rw-r--r--   0        0        0      879 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_jsonl/example.jsonl
+-rw-r--r--   0        0        0     5293 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_jsonl/process_jsonl.py
+-rw-r--r--   0        0        0     2699 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_zip/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_zip/__init__.py
+-rw-r--r--   0        0        0    53296 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_zip/example.zip
+-rw-r--r--   0        0        0     5716 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_zip/process_zip.py
+-rw-r--r--   0        0        0        0 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/__init__.py
+-rw-r--r--   0        0        0     7625 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/chunks.py
+-rw-r--r--   0        0        0      793 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/date.py
+-rw-r--r--   0        0        0     1217 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/extract_metadata.py
+-rw-r--r--   0        0        0     3682 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/file.py
+-rw-r--r--   0        0        0     1879 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/openai.py
+-rw-r--r--   0        0        0     1358 2023-05-04 11:30:12.792048 auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/pii_detection.py
+-rw-r--r--   0        0        0     1025 2023-05-04 11:30:12.796048 auto_retrieval_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5460 1970-01-01 00:00:00.000000 auto_retrieval_plugin-0.1.3/PKG-INFO
```

### Comparing `auto_retrieval_plugin-0.1.2/LICENSE` & `auto_retrieval_plugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/README.md` & `auto_retrieval_plugin-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/.well-known/ai-plugin.json` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/.well-known/ai-plugin.json`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/.well-known/default-ai-plugin.json` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/.well-known/default-ai-plugin.json`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/.well-known/logo.png` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/.well-known/logo.png`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/.well-known/openapi.yaml` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/.well-known/openapi.yaml`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/datastore.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/executor/docarray_v1.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/executor/docarray_v1.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/datastore/factory.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/datastore/factory.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/flow.yml` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/flow.yml`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/gateway.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/gateway.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/models/api.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/models/api.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/models/models.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/models/models.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/retrieval_plugin.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/retrieval_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from jcloud.api import deploy as deploy_flow
 from jcloud.flow import CloudFlow
 
 app = typer.Typer()
 
 current_file_path = Path(__file__).resolve()
 FLOW_PATH = current_file_path.parent / "flow.yml"
+ENV_FILE_PATH = current_file_path.parent / ".env"
 
 
 class UnsupportedExtensionError(Exception):
     pass
 
 
 class EmptyDirectoryError(Exception):
@@ -51,31 +52,31 @@
 def generate_bearer_token():
     payload = {"sub": random_string(), "iat": random_number()}
     return jwt.encode(payload, "my_secret", algorithm="HS256")
 
 
 def write_envs(new_envs):
     old_envs = {}
-    if os.path.exists("../.env"):
-        with open("../.env", "r") as f:
+    if os.path.exists(ENV_FILE_PATH):
+        with open(ENV_FILE_PATH, "r") as f:
             for line in f:
                 key, value = line.strip().split("=")
                 old_envs[key] = value
 
     env_vars = {**old_envs, **new_envs}
 
-    with open("../.env", "w") as f:
+    with open(ENV_FILE_PATH, "w") as f:
         for key, value in env_vars.items():
             f.write(f"{key}={value}\n")
             os.environ[key] = value
 
 
 def read_envs():
-    if os.path.exists("../.env"):
-        with open("../.env", "r") as f:
+    if os.path.exists(ENV_FILE_PATH):
+        with open(ENV_FILE_PATH, "r") as f:
             for line in f:
                 key, value = line.strip().split("=")
                 os.environ[key] = value
 
 
 def check_bearer_token(bearer_token: Optional[str] = None, generate: Optional[bool] = False):
     bearer_token = bearer_token or os.environ.get("RETRIEVAL_BEARER_TOKEN")
```

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_json/README.md` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_json/README.md`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_json/example.json` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_json/example.json`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_json/process_json.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_json/process_json.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_jsonl/README.md` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_jsonl/README.md`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_jsonl/example.jsonl` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_jsonl/example.jsonl`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_jsonl/process_jsonl.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_jsonl/process_jsonl.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_zip/README.md` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_zip/README.md`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_zip/example.zip` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_zip/example.zip`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/scripts/process_zip/process_zip.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/scripts/process_zip/process_zip.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/chunks.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/chunks.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/date.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/date.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/extract_metadata.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/extract_metadata.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/file.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/file.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/openai.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/openai.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/auto_retrieval_plugin/services/pii_detection.py` & `auto_retrieval_plugin-0.1.3/auto_retrieval_plugin/services/pii_detection.py`

 * *Files identical despite different names*

### Comparing `auto_retrieval_plugin-0.1.2/pyproject.toml` & `auto_retrieval_plugin-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-retrieval-plugin"
-version = "0.1.2"
+version = "0.1.3"
 description = "Create and host retrieval plugins for ChatGPT in one click"
 authors = ["saba <saba.sturua@jina.ai>", "johannes johannes.messner@jina.ai"]
 readme = "README.md"
 include = ["auto_retrieval_plugin/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `auto_retrieval_plugin-0.1.2/PKG-INFO` & `auto_retrieval_plugin-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-retrieval-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Create and host retrieval plugins for ChatGPT in one click
 Author: saba
 Author-email: saba.sturua@jina.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

