# Comparing `tmp/gpt_json-0.1.1.tar.gz` & `tmp/gpt_json-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_json-0.1.1.tar", max compression
+gzip compressed data, was "gpt_json-0.1.2.tar", max compression
```

## Comparing `gpt_json-0.1.1.tar` & `gpt_json-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-04 00:34:05.309526 gpt_json-0.1.1/LICENSE
--rw-r--r--   0        0        0     4721 2023-05-04 00:34:05.309526 gpt_json-0.1.1/README.md
--rw-r--r--   0        0        0       63 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/enums.py
--rw-r--r--   0        0        0      145 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/exceptions.py
--rw-r--r--   0        0        0     8754 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/gpt.py
--rw-r--r--   0        0        0      479 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/models.py
--rw-r--r--   0        0        0     1478 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/parsers.py
--rw-r--r--   0        0        0     1723 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/prompts.py
--rw-r--r--   0        0        0        0 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/tests/__init__.py
--rw-r--r--   0        0        0      256 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/tests/shared.py
--rw-r--r--   0        0        0     5630 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/tests/test_gpt.py
--rw-r--r--   0        0        0      741 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/tests/test_parsers.py
--rw-r--r--   0        0        0     1181 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/tests/test_prompts.py
--rw-r--r--   0        0        0     1969 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/tests/test_truncation.py
--rw-r--r--   0        0        0     1725 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/truncation.py
--rw-r--r--   0        0        0      484 2023-05-04 00:34:05.313526 gpt_json-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5223 1970-01-01 00:00:00.000000 gpt_json-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 00:57:37.676658 gpt_json-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4721 2023-05-04 00:57:37.676658 gpt_json-0.1.2/README.md
+-rw-r--r--   0        0        0       63 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/enums.py
+-rw-r--r--   0        0        0      145 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/exceptions.py
+-rw-r--r--   0        0        0     9149 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/gpt.py
+-rw-r--r--   0        0        0      479 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/models.py
+-rw-r--r--   0        0        0     1478 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/parsers.py
+-rw-r--r--   0        0        0     1860 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/prompts.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/shared.py
+-rw-r--r--   0        0        0     6225 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/test_gpt.py
+-rw-r--r--   0        0        0      741 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/test_parsers.py
+-rw-r--r--   0        0        0     1189 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/test_prompts.py
+-rw-r--r--   0        0        0     1969 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/tests/test_truncation.py
+-rw-r--r--   0        0        0     1725 2023-05-04 00:57:37.676658 gpt_json-0.1.2/gpt_json/truncation.py
+-rw-r--r--   0        0        0      534 2023-05-04 00:57:37.676658 gpt_json-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 gpt_json-0.1.2/PKG-INFO
```

### Comparing `gpt_json-0.1.1/LICENSE` & `gpt_json-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.1/README.md` & `gpt_json-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.1/gpt_json/gpt.py` & `gpt_json-0.1.2/gpt_json/gpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import backoff
 import openai
 from openai.error import APIConnectionError, RateLimitError
 from openai.error import Timeout as OpenAITimeout
 from pydantic import BaseModel
 from tiktoken import encoding_for_model
+from typing import Any
 
 from gpt_json.models import GPTMessage, GPTModelVersion, ResponseType
 from gpt_json.parsers import find_json_response
 from gpt_json.truncation import fix_truncated_json
 from gpt_json.prompts import generate_schema_prompt
 
 import logging
@@ -61,15 +62,15 @@
             raise ValueError("GPTJSON needs to be instantiated with a schema model, like GPTJSON[MySchema](...args).")
 
         if get_origin(self.schema_model) in {list, List}:
             self.extract_type = ResponseType.LIST
         elif issubclass(self.schema_model, BaseModel):
             self.extract_type = ResponseType.DICTIONARY
         else:
-            raise ValueError("GPTJSON needs to be instantiated with either a schema or a list.")
+            raise ValueError("GPTJSON needs to be instantiated with either a pydantic.BaseModel schema or a list of those schemas.")
 
         if self.auto_trim:
             if "gpt-4" in self.model:
                 self.max_tokens = 8192 - auto_trim_response_overhead
             elif "gpt-3.5" in self.model:
                 self.max_tokens = 4096 - auto_trim_response_overhead
             else:
@@ -78,15 +79,21 @@
         self.schema_prompt = generate_schema_prompt(self.schema_model)
         self.api_key = api_key
 
     async def run(
         self,
         messages: list[GPTMessage],
         max_tokens: int | None = None,
+        format_variables: dict[str, Any] | None = None,
     ) -> SchemaType | None:
+        messages = [
+            self.fill_message_template(message, format_variables or {})
+            for message in messages
+        ]
+
         response = await self.submit_request(messages, max_tokens=max_tokens)
         logger.debug("------- RAW RESPONSE ----------")
         logger.debug(response["choices"])
         logger.debug("------- END RAW RESPONSE ----------")
         extracted_json = self.extract_json(response, self.extract_type)
 
         # Cast to schema model
@@ -140,19 +147,14 @@
         on_backoff=handle_backoff
     )
     async def submit_request(
         self,
         messages: list[GPTMessage],
         max_tokens: int | None,
     ):
-        messages = [
-            self.fill_message_template(message)
-            for message in messages
-        ]
-
         logger.debug("------- START MESSAGE ----------")
         logger.debug(messages)
         logger.debug("------- END MESSAGE ----------")
         if self.auto_trim:
             messages = self.trim_messages(messages, self.max_tokens)
 
         optional_parameters = {}
@@ -168,22 +170,28 @@
             ],
             temperature=self.temperature,
             timeout=self.timeout,
             api_key=self.api_key,
             **optional_parameters,
         )
 
-    def fill_message_template(self, message: GPTMessage):
+    def fill_message_template(self, message: GPTMessage, format_variables: dict[str, Any]):
+        content = message.content.format(
+            **{
+                SCHEMA_PROMPT_TEMPLATE_KEY: self.schema_prompt,
+            }
+        )
+
+        # We do this formatting in a separate pass so we can fill any template variables that might
+        # have been left in the pydantic field typehints
+        content = content.format(**format_variables)
+
         return replace(
             message,
-            content=message.content.format(
-                **{
-                    SCHEMA_PROMPT_TEMPLATE_KEY: self.schema_prompt,
-                }
-            ),
+            content=content,
         )
 
     def message_to_dict(self, message: GPTMessage):
         return {
             "role": message.role.value,
             "content": message.content
         }
```

### Comparing `gpt_json-0.1.1/gpt_json/parsers.py` & `gpt_json-0.1.2/gpt_json/parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.1/gpt_json/prompts.py` & `gpt_json-0.1.2/gpt_json/prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,17 @@
                 payload.append(f'"{key}": {" | ".join([arg.__name__.lower() for arg in annotation_arguments])}')
             elif issubclass(value.type_, BaseModel):
                 payload.append(f'"{key}": {generate_payload(value.type_)}')
             else:
                 payload.append(f'"{key}": {value.type_.__name__.lower()}')
             if value.field_info.description:
                 payload[-1] += f' // {value.field_info.description}'
-        return '{' + ', '.join(payload) + '}'
+        # All brackets are double defined so they will passthrough a call to `.format()` where we
+        # pass custom variables
+        return '{{\n' + ',\n'.join(payload) + '\n}}'
 
     origin = get_origin(schema)
     args = get_args(schema)
 
     if origin == list:
         if len(args) > 1:
             raise ValueError("Only one list schema is supported at this time")
```

### Comparing `gpt_json-0.1.1/gpt_json/tests/test_gpt.py` & `gpt_json-0.1.2/gpt_json/tests/test_gpt.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import openai
 import pytest
 
 from gpt_json.gpt import GPTJSON
 from gpt_json.models import GPTMessage, GPTMessageRole, GPTModelVersion
 from gpt_json.tests.shared import MySchema, MySubSchema
+from pydantic import BaseModel, Field
 
 
 def test_throws_error_if_no_model_specified():
     with pytest.raises(ValueError, match="needs to be instantiated with a schema model"):
         GPTJSON(None)
 
 
@@ -182,7 +183,26 @@
     output_messages = gpt.trim_messages(input_messages, n=8192)
 
     assert len(output_messages) == len(expected_output_messages)
 
     for output_message, expected_output_message in zip(output_messages, expected_output_messages):
         assert output_message.role == expected_output_message.role
         assert output_message.content == expected_output_message.content
+
+
+def test_fill_message_template():
+    class TestTemplateSchema(BaseModel):
+        template_field: str = Field(description="Max length {max_length}")
+
+    gpt = GPTJSON[TestTemplateSchema](None)
+    assert gpt.fill_message_template(
+        GPTMessage(
+            role=GPTMessageRole.USER,
+            content="My schema is here: {json_schema}"
+        ),
+        dict(
+            max_length=100,
+        )
+    ) == GPTMessage(
+        role=GPTMessageRole.USER,
+        content="My schema is here: {\n\"template_field\": str // Max length 100\n}"
+    )
```

### Comparing `gpt_json-0.1.1/gpt_json/tests/test_parsers.py` & `gpt_json-0.1.2/gpt_json/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.1/gpt_json/tests/test_prompts.py` & `gpt_json-0.1.2/gpt_json/tests/test_prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,38 +11,38 @@
 
 @pytest.mark.parametrize(
     "schema_definition,expected",
     [
         (
             MySchema,
             """
-            {
+            {{
                 "text": str,
                 "items": str[],
                 "numerical": int | float,
-                "sub_element": {
+                "sub_element": {{
                     "name": str
-                },
+                }},
                 "reason": bool // Explanation
-            }
+            }}
             """
         ),
         (
             list[MySchema],
             """
             [
-            {
+            {{
             "text": str,
             "items": str[],
             "numerical": int | float,
-            "sub_element": {
+            "sub_element": {{
                 "name": str
-            },
+            }},
             "reason": bool // Explanation
-            }, // Repeat for as many objects as are relevant
+            }}, // Repeat for as many objects as are relevant
             ]
             """
         )
     ]
 )
 def test_generate_schema_prompt(schema_definition, expected: str):
     assert strip_whitespace(generate_schema_prompt(schema_definition)) == strip_whitespace(expected)
```

### Comparing `gpt_json-0.1.1/gpt_json/tests/test_truncation.py` & `gpt_json-0.1.2/gpt_json/tests/test_truncation.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.1/gpt_json/truncation.py` & `gpt_json-0.1.2/gpt_json/truncation.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.1.1/PKG-INFO` & `gpt_json-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gpt-json
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: Structured and typehinted GPT responses in Python.
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
```

