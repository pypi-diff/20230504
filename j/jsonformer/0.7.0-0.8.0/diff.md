# Comparing `tmp/jsonformer-0.7.0.tar.gz` & `tmp/jsonformer-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonformer-0.7.0.tar", max compression
+gzip compressed data, was "jsonformer-0.8.0.tar", max compression
```

## Comparing `jsonformer-0.7.0.tar` & `jsonformer-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2672 2023-05-03 15:24:03.720613 jsonformer-0.7.0/README.md
--rw-r--r--   0        0        0       85 2023-05-01 21:32:30.326739 jsonformer-0.7.0/jsonformer/__init__.py
--rw-r--r--   0        0        0     1037 2023-05-01 21:30:35.817333 jsonformer-0.7.0/jsonformer/example.py
--rw-r--r--   0        0        0      995 2023-05-01 17:24:41.244984 jsonformer-0.7.0/jsonformer/format.py
--rw-r--r--   0        0        0     1984 2023-05-01 17:24:41.245061 jsonformer-0.7.0/jsonformer/logits_processors.py
--rw-r--r--   0        0        0     7051 2023-05-03 15:50:58.799548 jsonformer-0.7.0/jsonformer/main.py
--rw-r--r--   0        0        0      476 2023-05-03 15:51:14.253333 jsonformer-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3327 1970-01-01 00:00:00.000000 jsonformer-0.7.0/setup.py
--rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 jsonformer-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2850 2023-05-04 16:48:52.075323 jsonformer-0.8.0/README.md
+-rw-r--r--   0        0        0       85 2023-05-01 21:32:30.326739 jsonformer-0.8.0/jsonformer/__init__.py
+-rw-r--r--   0        0        0     1081 2023-05-04 16:25:05.263995 jsonformer-0.8.0/jsonformer/example.py
+-rw-r--r--   0        0        0      995 2023-05-01 17:24:41.244984 jsonformer-0.8.0/jsonformer/format.py
+-rw-r--r--   0        0        0     1984 2023-05-01 17:24:41.245061 jsonformer-0.8.0/jsonformer/logits_processors.py
+-rw-r--r--   0        0        0     7197 2023-05-04 16:25:05.264416 jsonformer-0.8.0/jsonformer/main.py
+-rw-r--r--   0        0        0      476 2023-05-04 16:48:52.075655 jsonformer-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3507 1970-01-01 00:00:00.000000 jsonformer-0.8.0/setup.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 jsonformer-0.8.0/PKG-INFO
```

### Comparing `jsonformer-0.7.0/README.md` & `jsonformer-0.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.
 
 ### Problem: Getting models to output structured JSON is hard
 
 ### Solution: Only generate the content tokens and fill in the fixed tokens
 
+[![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/1rgs/jsonformer/blob/main/Jsonformer_example.ipynb)
+
 ![cover](img/cover4.png)
 
 Generating structured JSON from language models is a challenging task. The
 generated JSON must be syntactically correct, and it must conform to a schema
 that specifies the structure of the JSON.
 
 Current approaches to this problem are brittle and error-prone. They rely on prompt engineering, fine-tuning, and post-processing, but they still fail to generate syntactically correct JSON in many cases.
@@ -41,15 +43,15 @@
             "type": "array",
             "items": {"type": "string"}
         }
     }
 }
 
 prompt = "Generate a person's information based on the following schema:"
-jsonformer = Jsonformer(model, tokenizer, json_schema, prompt)
+jsonformer = Jsonformer(model, tokenizer, json_schema, prompt, device="cuda")
 generated_data = jsonformer()
 
 print(generated_data)
 ```
 
 ## Features
```

### Comparing `jsonformer-0.7.0/jsonformer/example.py` & `jsonformer-0.8.0/jsonformer/example.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from jsonformer.main import Jsonformer
 from transformers import (
     AutoModelForCausalLM,
     AutoTokenizer,
 )
 
 
-
 weather_schema = {
     "type": "object",
     "properties": {
         "temperature": {"type": "number"},
         "humidity": {
             "type": "number",
         },
@@ -22,25 +21,29 @@
             },
         },
     },
 }
 
 print("Loading model and tokenizer...")
 model_name = "databricks/dolly-v2-12b"
-model = AutoModelForCausalLM.from_pretrained(model_name, use_cache=True)
+
+model = AutoModelForCausalLM.from_pretrained(
+    model_name, use_cache=True, device_map="auto"
+)
 tokenizer = AutoTokenizer.from_pretrained(model_name, use_fast=True, use_cache=True)
 print("Loaded model and tokenizer")
 
 
 builder = Jsonformer(
     model=model,
     tokenizer=tokenizer,
     json_schema=weather_schema,
     prompt="generate the weather",
     debug=True,
+    device="cuda",
 )
 
 print("Generating...")
 output = builder()
 
 highlight_values(
     output,
```

### Comparing `jsonformer-0.7.0/jsonformer/format.py` & `jsonformer-0.8.0/jsonformer/format.py`

 * *Files identical despite different names*

### Comparing `jsonformer-0.7.0/jsonformer/logits_processors.py` & `jsonformer-0.8.0/jsonformer/logits_processors.py`

 * *Files identical despite different names*

### Comparing `jsonformer-0.7.0/jsonformer/main.py` & `jsonformer-0.8.0/jsonformer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
     def __init__(
         self,
         model: PreTrainedModel,
         tokenizer: PreTrainedTokenizer,
         json_schema: Dict[str, Any],
         prompt: str,
+        *,
+        device: str,
         debug: bool = False,
         max_array_length: int = 10,
         max_number_tokens: int = 6,
         temperature: float = 1.0,
         max_string_token_length: int = 10,
     ):
         self.model = model
@@ -33,24 +35,25 @@
         self.generation_marker = "|GENERATION|"
         self.debug_on = debug
         self.max_array_length = max_array_length
 
         self.max_number_tokens = max_number_tokens
         self.temperature = temperature
         self.max_string_token_length = max_string_token_length
+        self.device = device
 
     def debug(self, *args, **kwargs):
         if self.debug_on:
             print(*args, **kwargs)
 
     def generate_number(self) -> float:
         prompt = self.get_prompt()
         self.debug("[generate_number] prompt", prompt)
         response = self.model.generate(
-            self.tokenizer.encode(prompt, return_tensors="pt"),
+            self.tokenizer.encode(prompt, return_tensors="pt").to(self.model.device),
             max_new_tokens=self.max_number_tokens,
             num_return_sequences=1,
             logits_processor=[self.number_logit_processor],
             stopping_criteria=[self.number_stop_criteria],
             temperature=self.temperature,
             pad_token_id=self.tokenizer.eos_token_id,
         )
@@ -66,15 +69,15 @@
             return
 
     def generate_boolean(self) -> bool:
         prompt = self.get_prompt()
         self.debug("[generate_boolean] prompt", prompt)
 
         input_tensor = self.tokenizer.encode(prompt, return_tensors="pt")
-        output = self.model.forward(input_tensor)
+        output = self.model.forward(input_tensor.to(self.model.device))
         logits = output.logits[0, -1]
 
         true_token_id = self.tokenizer.convert_tokens_to_ids("true")
         false_token_id = self.tokenizer.convert_tokens_to_ids("false")
 
         true_logits = logits[true_token_id]
         false_logits = logits[false_token_id]
@@ -87,15 +90,15 @@
             print("Failed to generate a valid boolean value")
             return None
 
     def generate_string(self) -> str:
         prompt = self.get_prompt()
         self.debug("[generate_string] prompt", prompt)
         response = self.model.generate(
-            self.tokenizer.encode(prompt, return_tensors="pt"),
+            self.tokenizer.encode(prompt, return_tensors="pt").to(self.model.device),
             max_new_tokens=self.max_string_token_length,
             num_return_sequences=1,
             temperature=self.temperature,
             pad_token_id=self.tokenizer.eos_token_id,
         )
         response = self.tokenizer.decode(response[0], skip_special_tokens=True)
 
@@ -114,15 +117,15 @@
             obj[key] = self.generate_value(schema, obj, key)
         return obj
 
     def generate_value(
         self,
         schema: Dict[str, Any],
         obj: Union[Dict[str, Any], List[Any]],
-        key: str | None = None,
+        key: Union[str, None] = None,
     ) -> Any:
         schema_type = schema["type"]
         if schema_type == "number":
             if key:
                 obj[key] = self.generation_marker
             else:
                 obj.append(self.generation_marker)
@@ -158,22 +161,22 @@
             element = self.generate_value(item_schema, obj)
             obj[-1] = element
 
             obj.append(self.generation_marker)
             input_prompt = self.get_prompt()
             obj.pop()
             input_tensor = self.tokenizer.encode(input_prompt, return_tensors="pt")
-            output = self.model.forward(input_tensor)
+            output = self.model.forward(input_tensor.to(self.model.device))
             logits = output.logits[0, -1]
 
             close_bracket_token_id = self.tokenizer.convert_tokens_to_ids("]")
             comma_token_id = self.tokenizer.convert_tokens_to_ids(", ")
             close_bracket_logits = logits[close_bracket_token_id]
             comma_logits = logits[comma_token_id]
-        
+
             if close_bracket_logits > comma_logits:
                 break
 
         return obj
 
     def get_prompt(self):
         template = """{prompt}\nOutput result in the following JSON schema format:\n{schema}\nResult: {progress}"""
@@ -190,12 +193,11 @@
             progress=progress,
         )
 
         return prompt
 
     def __call__(self) -> Dict[str, Any]:
         self.value = {}
-
         generated_data = self.generate_object(
             self.json_schema["properties"], self.value
         )
         return generated_data
```

### Comparing `jsonformer-0.7.0/setup.py` & `jsonformer-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['termcolor>=2.3.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'jsonformer',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': '',
-    'long_description': '# Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.\n\n### Problem: Getting models to output structured JSON is hard\n\n### Solution: Only generate the content tokens and fill in the fixed tokens\n\n![cover](img/cover4.png)\n\nGenerating structured JSON from language models is a challenging task. The\ngenerated JSON must be syntactically correct, and it must conform to a schema\nthat specifies the structure of the JSON.\n\nCurrent approaches to this problem are brittle and error-prone. They rely on prompt engineering, fine-tuning, and post-processing, but they still fail to generate syntactically correct JSON in many cases.\n\nJsonformer is a new approach to this problem. In structured data, many tokens are fixed and predictable. Jsonformer is a wrapper around HuggingFace models that fills in the fixed tokens during the generation process, and only delegates the generation of content tokens to the language model. This makes it more efficient and bulletproof than existing approaches.\n\nThis currently supports a subset of JSON Schema. Below is a list of the supported schema types:\n\n- number\n- boolean\n- string\n- array\n- object\n\n## Example\n\n```python\nfrom jsonformer import Jsonformer\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\njson_schema = {\n    "type": "object",\n    "properties": {\n        "name": {"type": "string"},\n        "age": {"type": "number"},\n        "is_student": {"type": "boolean"},\n        "courses": {\n            "type": "array",\n            "items": {"type": "string"}\n        }\n    }\n}\n\nprompt = "Generate a person\'s information based on the following schema:"\njsonformer = Jsonformer(model, tokenizer, json_schema, prompt)\ngenerated_data = jsonformer()\n\nprint(generated_data)\n```\n\n## Features\n\n- Bulletproof JSON generation: Jsonformer ensures that the generated JSON is always syntactically correct and conforms to the specified schema.\n- Efficiency: By generating only the content tokens and filling in the fixed tokens, Jsonformer is more efficient than generating a full JSON string and parsing it.\n- Flexible and extendable: Jsonformer is built on top of the HuggingFace transformers library, making it compatible with any model that supports the HuggingFace interface.\n\n## Installation\n\n```bash\npip install jsonformer\n```\n\n## License\n\nJsonformer is released under the MIT License. You are free to use, modify, and distribute this software for any purpose, commercial or non-commercial, as long as the original copyright and license notice are included.\n',
+    'long_description': '# Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.\n\n### Problem: Getting models to output structured JSON is hard\n\n### Solution: Only generate the content tokens and fill in the fixed tokens\n\n[![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/1rgs/jsonformer/blob/main/Jsonformer_example.ipynb)\n\n![cover](img/cover4.png)\n\nGenerating structured JSON from language models is a challenging task. The\ngenerated JSON must be syntactically correct, and it must conform to a schema\nthat specifies the structure of the JSON.\n\nCurrent approaches to this problem are brittle and error-prone. They rely on prompt engineering, fine-tuning, and post-processing, but they still fail to generate syntactically correct JSON in many cases.\n\nJsonformer is a new approach to this problem. In structured data, many tokens are fixed and predictable. Jsonformer is a wrapper around HuggingFace models that fills in the fixed tokens during the generation process, and only delegates the generation of content tokens to the language model. This makes it more efficient and bulletproof than existing approaches.\n\nThis currently supports a subset of JSON Schema. Below is a list of the supported schema types:\n\n- number\n- boolean\n- string\n- array\n- object\n\n## Example\n\n```python\nfrom jsonformer import Jsonformer\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\njson_schema = {\n    "type": "object",\n    "properties": {\n        "name": {"type": "string"},\n        "age": {"type": "number"},\n        "is_student": {"type": "boolean"},\n        "courses": {\n            "type": "array",\n            "items": {"type": "string"}\n        }\n    }\n}\n\nprompt = "Generate a person\'s information based on the following schema:"\njsonformer = Jsonformer(model, tokenizer, json_schema, prompt, device="cuda")\ngenerated_data = jsonformer()\n\nprint(generated_data)\n```\n\n## Features\n\n- Bulletproof JSON generation: Jsonformer ensures that the generated JSON is always syntactically correct and conforms to the specified schema.\n- Efficiency: By generating only the content tokens and filling in the fixed tokens, Jsonformer is more efficient than generating a full JSON string and parsing it.\n- Flexible and extendable: Jsonformer is built on top of the HuggingFace transformers library, making it compatible with any model that supports the HuggingFace interface.\n\n## Installation\n\n```bash\npip install jsonformer\n```\n\n## License\n\nJsonformer is released under the MIT License. You are free to use, modify, and distribute this software for any purpose, commercial or non-commercial, as long as the original copyright and license notice are included.\n',
     'author': '1rgs',
     'author_email': 'rgsduke@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `jsonformer-0.7.0/PKG-INFO` & `jsonformer-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonformer
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 Author: 1rgs
 Author-email: rgsduke@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,14 +15,16 @@
 
 # Jsonformer: A Bulletproof Way to Generate Structured JSON from Language Models.
 
 ### Problem: Getting models to output structured JSON is hard
 
 ### Solution: Only generate the content tokens and fill in the fixed tokens
 
+[![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/1rgs/jsonformer/blob/main/Jsonformer_example.ipynb)
+
 ![cover](img/cover4.png)
 
 Generating structured JSON from language models is a challenging task. The
 generated JSON must be syntactically correct, and it must conform to a schema
 that specifies the structure of the JSON.
 
 Current approaches to this problem are brittle and error-prone. They rely on prompt engineering, fine-tuning, and post-processing, but they still fail to generate syntactically correct JSON in many cases.
@@ -56,15 +58,15 @@
             "type": "array",
             "items": {"type": "string"}
         }
     }
 }
 
 prompt = "Generate a person's information based on the following schema:"
-jsonformer = Jsonformer(model, tokenizer, json_schema, prompt)
+jsonformer = Jsonformer(model, tokenizer, json_schema, prompt, device="cuda")
 generated_data = jsonformer()
 
 print(generated_data)
 ```
 
 ## Features
```

