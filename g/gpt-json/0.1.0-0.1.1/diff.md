# Comparing `tmp/gpt-json-0.1.0.tar.gz` & `tmp/gpt_json-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-json-0.1.0.tar", max compression
+gzip compressed data, was "gpt_json-0.1.1.tar", max compression
```

## Comparing `gpt-json-0.1.0.tar` & `gpt_json-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-03 21:30:21.275700 gpt-json-0.1.0/LICENSE
--rw-r--r--   0        0        0     3107 2023-05-03 23:53:27.329763 gpt-json-0.1.0/README.md
--rw-r--r--   0        0        0       63 2023-05-03 23:53:10.452836 gpt-json-0.1.0/gpt_json/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 23:53:10.452875 gpt-json-0.1.0/gpt_json/enums.py
--rw-r--r--   0        0        0      145 2023-05-03 23:53:10.453154 gpt-json-0.1.0/gpt_json/exceptions.py
--rw-r--r--   0        0        0     8367 2023-05-03 23:53:10.453282 gpt-json-0.1.0/gpt_json/gpt.py
--rw-r--r--   0        0        0      479 2023-05-03 23:53:10.453377 gpt-json-0.1.0/gpt_json/models.py
--rw-r--r--   0        0        0     1478 2023-05-03 23:53:10.453481 gpt-json-0.1.0/gpt_json/parsers.py
--rw-r--r--   0        0        0     1723 2023-05-03 23:53:10.453576 gpt-json-0.1.0/gpt_json/prompts.py
--rw-r--r--   0        0        0        0 2023-05-03 23:53:10.453611 gpt-json-0.1.0/gpt_json/tests/__init__.py
--rw-r--r--   0        0        0      256 2023-05-03 23:53:10.453740 gpt-json-0.1.0/gpt_json/tests/shared.py
--rw-r--r--   0        0        0     4157 2023-05-04 00:01:38.809451 gpt-json-0.1.0/gpt_json/tests/test_gpt.py
--rw-r--r--   0        0        0      741 2023-05-03 23:53:10.453931 gpt-json-0.1.0/gpt_json/tests/test_parsers.py
--rw-r--r--   0        0        0     1181 2023-05-03 23:53:10.454026 gpt-json-0.1.0/gpt_json/tests/test_prompts.py
--rw-r--r--   0        0        0     1969 2023-05-03 23:53:10.454113 gpt-json-0.1.0/gpt_json/tests/test_truncation.py
--rw-r--r--   0        0        0     1725 2023-05-03 23:53:10.454323 gpt-json-0.1.0/gpt_json/truncation.py
--rw-r--r--   0        0        0      484 2023-05-03 23:53:10.455121 gpt-json-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 gpt-json-0.1.0/setup.py
--rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 gpt-json-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 00:34:05.309526 gpt_json-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4721 2023-05-04 00:34:05.309526 gpt_json-0.1.1/README.md
+-rw-r--r--   0        0        0       63 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/enums.py
+-rw-r--r--   0        0        0      145 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/exceptions.py
+-rw-r--r--   0        0        0     8754 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/gpt.py
+-rw-r--r--   0        0        0      479 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/models.py
+-rw-r--r--   0        0        0     1478 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/parsers.py
+-rw-r--r--   0        0        0     1723 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/prompts.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/tests/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-04 00:34:05.309526 gpt_json-0.1.1/gpt_json/tests/shared.py
+-rw-r--r--   0        0        0     5630 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/tests/test_gpt.py
+-rw-r--r--   0        0        0      741 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/tests/test_parsers.py
+-rw-r--r--   0        0        0     1181 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/tests/test_prompts.py
+-rw-r--r--   0        0        0     1969 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/tests/test_truncation.py
+-rw-r--r--   0        0        0     1725 2023-05-04 00:34:05.313526 gpt_json-0.1.1/gpt_json/truncation.py
+-rw-r--r--   0        0        0      484 2023-05-04 00:34:05.313526 gpt_json-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5223 1970-01-01 00:00:00.000000 gpt_json-0.1.1/PKG-INFO
```

### Comparing `gpt-json-0.1.0/LICENSE` & `gpt_json-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-json-0.1.0/gpt_json/gpt.py` & `gpt_json-0.1.1/gpt_json/gpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,25 @@
 from tiktoken import encoding_for_model
 
 from gpt_json.models import GPTMessage, GPTModelVersion, ResponseType
 from gpt_json.parsers import find_json_response
 from gpt_json.truncation import fix_truncated_json
 from gpt_json.prompts import generate_schema_prompt
 
+import logging
+
+logger = logging.getLogger('my_logger')
+handler = logging.StreamHandler()
+formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+handler.setFormatter(formatter)
+logger.addHandler(handler)
+
 
 def handle_backoff(details):
-    print(
+    logger.warning(
         "Backing off {wait:0.1f} seconds after {tries} tries "
         "calling function {target} with args {args} and kwargs "
         "{kwargs}".format(**details)
     )
 
 SchemaType = TypeVar("SchemaType", bound=BaseModel)
 
@@ -72,17 +80,17 @@
 
     async def run(
         self,
         messages: list[GPTMessage],
         max_tokens: int | None = None,
     ) -> SchemaType | None:
         response = await self.submit_request(messages, max_tokens=max_tokens)
-        print("------- RAW RESPONSE ----------")
-        print(response["choices"])
-        print("------- END RAW RESPONSE ----------")
+        logger.debug("------- RAW RESPONSE ----------")
+        logger.debug(response["choices"])
+        logger.debug("------- END RAW RESPONSE ----------")
         extracted_json = self.extract_json(response, self.extract_type)
 
         # Cast to schema model
         if extracted_json is None:
             return None
 
         # Allow pydantic to handle the validation
@@ -96,15 +104,15 @@
         """
         Assumes one main block of results, either list of dictionary
 
         """
         choices = completion_response["choices"]
 
         if not choices:
-            print("No choices available, should report error...")
+            logger.warning("No choices available, should report error...")
             return None
 
         full_response = choices[0]["message"]["content"]
 
         extracted_response = find_json_response(full_response, extract_type)
         if extracted_response is None:
             return None
@@ -113,17 +121,17 @@
         extracted_response = extracted_response.replace("False", "false")
 
         fixed_response = fix_truncated_json(extracted_response)
 
         try:
             return json_loads(fixed_response)
         except JSONDecodeError as e:
-            print("Extracted", extracted_response)
-            print("Did parse", fixed_response)
-            print("JSON decode error, likely malformed json input", e)
+            logger.debug("Extracted", extracted_response)
+            logger.debug("Did parse", fixed_response)
+            logger.error("JSON decode error, likely malformed json input", e)
             return None
 
     # Most requests succeed on the first try but we wrap it locally here in case
     # there is some temporarily instability with the API. If there are longer periods
     # of instability, there should be system-wide retries in a daemon.
     @backoff.on_exception(
         backoff.expo,
@@ -137,17 +145,17 @@
         max_tokens: int | None,
     ):
         messages = [
             self.fill_message_template(message)
             for message in messages
         ]
 
-        print("------- START MESSAGE ----------")
-        print(messages)
-        print("------- END MESSAGE ----------")
+        logger.debug("------- START MESSAGE ----------")
+        logger.debug(messages)
+        logger.debug("------- END MESSAGE ----------")
         if self.auto_trim:
             messages = self.trim_messages(messages, self.max_tokens)
 
         optional_parameters = {}
 
         if max_tokens:
             optional_parameters["max_tokens"] = max_tokens
@@ -213,33 +221,34 @@
                 filtered_messages.append(message)
                 current_token_count += message_token_count
             else:
                 remaining_tokens = n - current_token_count
                 if remaining_tokens > 0:
                     cropped_message = enc.decode(tokens[:remaining_tokens])
                     filtered_messages.append(cropped_message)
+                current_token_count += remaining_tokens
                 break
 
         # Recreate the messages with our new text
         new_messages = [
             replace(
                 messages[i],
                 content=content,
             )
             for i, content in enumerate(filtered_messages)
         ]
 
         # Log a copy of the message array if we have to crop it
         if current_token_count != original_token_count:
-            print(
+            logger.debug(
                 f"Trimmed message from {original_token_count} to {current_token_count} tokens",
                 new_messages,
             )
         else:
-            print(f"Skipping trim ({original_token_count}) ({current_token_count})")
+            logger.debug(f"Skipping trim ({original_token_count}) ({current_token_count})")
 
         return new_messages
 
     def __class_getitem__(cls, item):
         new_cls = super().__class_getitem__(item)
         new_cls.schema_model = item
         return new_cls
```

### Comparing `gpt-json-0.1.0/gpt_json/parsers.py` & `gpt_json-0.1.1/gpt_json/parsers.py`

 * *Files identical despite different names*

### Comparing `gpt-json-0.1.0/gpt_json/prompts.py` & `gpt_json-0.1.1/gpt_json/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-json-0.1.0/gpt_json/tests/test_parsers.py` & `gpt_json-0.1.1/gpt_json/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `gpt-json-0.1.0/gpt_json/tests/test_prompts.py` & `gpt_json-0.1.1/gpt_json/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-json-0.1.0/gpt_json/tests/test_truncation.py` & `gpt_json-0.1.1/gpt_json/tests/test_truncation.py`

 * *Files identical despite different names*

### Comparing `gpt-json-0.1.0/gpt_json/truncation.py` & `gpt_json-0.1.1/gpt_json/truncation.py`

 * *Files identical despite different names*

### Comparing `gpt-json-0.1.0/PKG-INFO` & `gpt_json-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: gpt-json
-Version: 0.1.0
-Summary: 
-Author: Pierce Freeman
-Author-email: pierce@freeman.vc
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: openai (>=0.27.6,<0.28.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
-Description-Content-Type: text/markdown
-
 # gpt-json
 
 JSON is a beautiful format. It's both human readable and machine readable, which makes it a great format for structured output of LLMs (after all - LLMs are somewhere in the middle). `gpt-json` is a wrapper around GPT that allows for declarative definition of expected output format when you're trying to parse results into a downstream pipeline.
 
 Specifically it:
 - Relies on Pydantic schema definitions and type validations
 - Allows for defining both dictionaries and lists
@@ -93,13 +78,22 @@
 ```
 
 ```
 sentiment=1
 Detected sentiment: 1
 ```
 
+## Other Configurations
+
+The `GPTJSON` class supports other configuration parameters at initialization.
+
+| Parameter                   | Type                   | Description                                                                                                                                                                            |
+|-----------------------------|------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| model                       | GPTModelVersion \| str | (default: GPTModelVersion.GPT_4) - For convenience we provide the currently supported GPT model versions in the `GPTModelVersion` enum. You can also pass a string value if you want to use another more specific architecture.                                                                                                                                                       |
+| auto_trim                   | bool                   | (default: False) - If your input prompt is too long, perhaps because of dynamic injected content, will automatically truncate the text to create enough room for the model's response. |
+| auto_trim_response_overhead | int                    | (default: 0) - If you're using auto_trim, configures the max amount of tokens to allow in the model's response.                                                                        |
+
 ## Comparison to Other Libraries
 
 A non-exhaustive list of other libraries that address the same problem. None of them were fully compatible with my deployment (hence this library), but check them out:
 
-[jsonformer](https://github.com/1rgs/jsonformer) - Works with any Huggingface model, whereas `gpt-json` is specifically tailored towards the GPT-X family.
-
+[jsonformer](https://github.com/1rgs/jsonformer) - Works with any Huggingface model, whereas `gpt-json` is specifically tailored towards the GPT-X family. GPT doesn't output logit probabilities or allow fixed decoder templating so the same approach can't apply.
```

