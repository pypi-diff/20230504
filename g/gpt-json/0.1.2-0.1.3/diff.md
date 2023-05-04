# Comparing `tmp/gpt_json-0.1.2.tar.gz` & `tmp/gpt_json-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_json-0.1.2.tar", max compression
+gzip compressed data, was "gpt_json-0.1.3.tar", max compression
```

## Comparing `gpt_json-0.1.2.tar` & `gpt_json-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-04 00:57:37.676658 gpt_json-0.1.2/LICENSE
--rw-r--r--   0        0        0     4721 2023-05-04 00:57:37.676658 gpt_json-0.1.2/README.md
--rw-r--r--   0        0        0       63 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/enums.py
--rw-r--r--   0        0        0      145 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/exceptions.py
--rw-r--r--   0        0        0     9149 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/gpt.py
--rw-r--r--   0        0        0      479 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/models.py
--rw-r--r--   0        0        0     1478 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/parsers.py
--rw-r--r--   0        0        0     1860 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/prompts.py
--rw-r--r--   0        0        0        0 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/__init__.py
--rw-r--r--   0        0        0      256 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/shared.py
--rw-r--r--   0        0        0     6225 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/test_gpt.py
--rw-r--r--   0        0        0      741 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/test_parsers.py
--rw-r--r--   0        0        0     1189 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/test_prompts.py
--rw-r--r--   0        0        0     1969 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/test_truncation.py
--rw-r--r--   0        0        0     1725 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/truncation.py
--rw-r--r--   0        0        0      534 2023-05-04 00:57:37.676658 gpt_json-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 gpt_json-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 01:14:22.536671 gpt_json-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4721 2023-05-04 01:14:22.536671 gpt_json-0.1.3/README.md
+-rw-r--r--   0        0        0       63 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/enums.py
+-rw-r--r--   0        0        0      145 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/exceptions.py
+-rw-r--r--   0        0        0     9422 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/gpt.py
+-rw-r--r--   0        0        0      479 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/models.py
+-rw-r--r--   0        0        0     1478 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/parsers.py
+-rw-r--r--   0        0        0     1860 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/prompts.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/tests/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/tests/shared.py
+-rw-r--r--   0        0        0     6264 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/tests/test_gpt.py
+-rw-r--r--   0        0        0      741 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/tests/test_parsers.py
+-rw-r--r--   0        0        0     1189 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/tests/test_prompts.py
+-rw-r--r--   0        0        0     1969 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/tests/test_truncation.py
+-rw-r--r--   0        0        0     1725 2023-05-04 01:14:22.540671 gpt_json-0.1.3/gpt_json/truncation.py
+-rw-r--r--   0        0        0      534 2023-05-04 01:14:22.540671 gpt_json-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 gpt_json-0.1.3/PKG-INFO
```

### Comparing `gpt_json-0.1.2/LICENSE` & `gpt_json-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.2/README.md` & `gpt_json-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.2/gpt_json/gpt.py` & `gpt_json-0.1.3/gpt_json/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,19 +171,23 @@
             temperature=self.temperature,
             timeout=self.timeout,
             api_key=self.api_key,
             **optional_parameters,
         )
 
     def fill_message_template(self, message: GPTMessage, format_variables: dict[str, Any]):
-        content = message.content.format(
-            **{
-                SCHEMA_PROMPT_TEMPLATE_KEY: self.schema_prompt,
-            }
-        )
+        auto_format = {
+            SCHEMA_PROMPT_TEMPLATE_KEY: self.schema_prompt,
+        }
+
+        # Regular quotes should passthrough to the next stage, except for our special keys
+        content = message.content.replace('{', '{{').replace('}', '}}')
+        for key in auto_format.keys():
+            content = content.replace("{{" + key + "}}", "{" + key + "}")
+        content = content.format(**auto_format)
 
         # We do this formatting in a separate pass so we can fill any template variables that might
         # have been left in the pydantic field typehints
         content = content.format(**format_variables)
 
         return replace(
             message,
```

### Comparing `gpt_json-0.1.2/gpt_json/parsers.py` & `gpt_json-0.1.3/gpt_json/parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.2/gpt_json/prompts.py` & `gpt_json-0.1.3/gpt_json/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.2/gpt_json/tests/test_gpt.py` & `gpt_json-0.1.3/gpt_json/tests/test_gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,16 +193,16 @@
     class TestTemplateSchema(BaseModel):
         template_field: str = Field(description="Max length {max_length}")
 
     gpt = GPTJSON[TestTemplateSchema](None)
     assert gpt.fill_message_template(
         GPTMessage(
             role=GPTMessageRole.USER,
-            content="My schema is here: {json_schema}"
+            content="Variable: {max_length}\nMy schema is here: {json_schema}"
         ),
         dict(
             max_length=100,
         )
     ) == GPTMessage(
         role=GPTMessageRole.USER,
-        content="My schema is here: {\n\"template_field\": str // Max length 100\n}"
+        content="Variable: 100\nMy schema is here: {\n\"template_field\": str // Max length 100\n}"
     )
```

### Comparing `gpt_json-0.1.2/gpt_json/tests/test_parsers.py` & `gpt_json-0.1.3/gpt_json/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.2/gpt_json/tests/test_prompts.py` & `gpt_json-0.1.3/gpt_json/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.2/gpt_json/tests/test_truncation.py` & `gpt_json-0.1.3/gpt_json/tests/test_truncation.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.2/gpt_json/truncation.py` & `gpt_json-0.1.3/gpt_json/truncation.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.2/pyproject.toml` & `gpt_json-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-json"
-version = "0.1.2"
+version = "0.1.3"
 description = "Structured and typehinted GPT responses in Python."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 packages = [{include = "gpt_json"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gpt_json-0.1.2/PKG-INFO` & `gpt_json-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-json
-Version: 0.1.2
+Version: 0.1.3
 Summary: Structured and typehinted GPT responses in Python.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

