# Comparing `tmp/openai-helper-0.2.0.tar.gz` & `tmp/openai-helper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-helper-0.2.0.tar", max compression
+gzip compressed data, was "openai-helper-0.2.1.tar", max compression
```

## Comparing `openai-helper-0.2.0.tar` & `openai-helper-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     7099 2023-03-28 19:57:26.769170 openai-helper-0.2.0/openai_helper/__init__.py
--rw-r--r--   0        0        0      168 2023-03-01 23:24:35.426289 openai-helper-0.2.0/openai_helper/bp/__init__.py
--rw-r--r--   0        0        0     3145 2023-03-28 16:40:16.611674 openai-helper-0.2.0/openai_helper/bp/openai_chat_completion.py
--rw-r--r--   0        0        0     3664 2023-03-01 22:37:49.356289 openai-helper-0.2.0/openai_helper/bp/openai_custom_model.py
--rw-r--r--   0        0        0     4752 2023-03-01 22:13:34.947789 openai-helper-0.2.0/openai_helper/bp/openai_text_completion.py
--rw-r--r--   0        0        0      745 2023-03-27 18:22:15.869933 openai-helper-0.2.0/openai_helper/dmo/__init__.py
--rw-r--r--   0        0        0     1542 2023-03-01 23:24:44.090788 openai-helper-0.2.0/openai_helper/dmo/chat_message_formatter.py
--rw-r--r--   0        0        0     7698 2022-12-08 01:40:33.067448 openai-helper-0.2.0/openai_helper/dmo/completion_event_extractor.py
--rw-r--r--   0        0        0     2566 2023-02-13 05:49:27.009400 openai-helper-0.2.0/openai_helper/dmo/etl_handle_textcompletions.py
--rw-r--r--   0        0        0     1351 2023-02-25 18:10:04.895458 openai-helper-0.2.0/openai_helper/dmo/etl_remove_emojis.py
--rw-r--r--   0        0        0     3095 2023-03-11 18:30:15.174565 openai-helper-0.2.0/openai_helper/dmo/etl_remove_listindicators.py
--rw-r--r--   0        0        0     2871 2023-03-14 16:16:21.916983 openai-helper-0.2.0/openai_helper/dmo/etl_remove_promptindicators.py
--rw-r--r--   0        0        0     1665 2022-11-16 18:34:53.819884 openai-helper-0.2.0/openai_helper/dmo/etl_replace_cliches.py
--rw-r--r--   0        0        0     1496 2022-09-29 21:43:12.370296 openai-helper-0.2.0/openai_helper/dmo/etl_replace_duplicatedinput.py
--rw-r--r--   0        0        0     4123 2023-04-27 00:12:55.039700 openai-helper-0.2.0/openai_helper/dmo/input_token_counter.py
--rw-r--r--   0        0        0     1172 2022-11-16 18:34:53.819381 openai-helper-0.2.0/openai_helper/dmo/no_openai_event.py
--rw-r--r--   0        0        0     1719 2022-11-16 18:14:14.917879 openai-helper-0.2.0/openai_helper/dmo/openai_connector.py
--rw-r--r--   0        0        0     6943 2023-03-01 23:21:18.381290 openai-helper-0.2.0/openai_helper/dmo/output_extractor_chat.py
--rw-r--r--   0        0        0     8110 2023-03-01 23:21:47.463789 openai-helper-0.2.0/openai_helper/dmo/output_extractor_text.py
--rw-r--r--   0        0        0      268 2023-03-16 18:41:15.424607 openai-helper-0.2.0/openai_helper/svc/__init__.py
--rw-r--r--   0        0        0     2985 2022-11-19 06:19:01.788211 openai-helper-0.2.0/openai_helper/svc/create_openai_answer.py
--rw-r--r--   0        0        0     2390 2023-03-25 05:55:44.937494 openai-helper-0.2.0/openai_helper/svc/extract_primary_topic.py
--rw-r--r--   0        0        0     2554 2022-11-16 18:34:53.819884 openai-helper-0.2.0/openai_helper/svc/extract_top_response.py
--rw-r--r--   0        0        0     5301 2023-03-28 16:40:16.616677 openai-helper-0.2.0/openai_helper/svc/run_chat_completion.py
--rw-r--r--   0        0        0     8919 2023-04-27 00:03:17.192201 openai-helper-0.2.0/openai_helper/svc/run_text_completion.py
--rw-r--r--   0        0        0     2191 2023-04-27 00:13:12.938200 openai-helper-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4102 2023-03-27 18:14:05.658957 openai-helper-0.2.0/README.md
--rw-r--r--   0        0        0     4903 2023-04-27 00:13:31.677200 openai-helper-0.2.0/setup.py
--rw-r--r--   0        0        0     4983 2023-04-27 00:13:31.677701 openai-helper-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7069 2023-05-03 23:47:33.313712 openai-helper-0.2.1/openai_helper/__init__.py
+-rw-r--r--   0        0        0      168 2023-03-01 23:24:35.426289 openai-helper-0.2.1/openai_helper/bp/__init__.py
+-rw-r--r--   0        0        0     3145 2023-03-28 16:40:16.611674 openai-helper-0.2.1/openai_helper/bp/openai_chat_completion.py
+-rw-r--r--   0        0        0     3664 2023-03-01 22:37:49.356289 openai-helper-0.2.1/openai_helper/bp/openai_custom_model.py
+-rw-r--r--   0        0        0     4752 2023-03-01 22:13:34.947789 openai-helper-0.2.1/openai_helper/bp/openai_text_completion.py
+-rw-r--r--   0        0        0      745 2023-03-27 18:22:15.869933 openai-helper-0.2.1/openai_helper/dmo/__init__.py
+-rw-r--r--   0        0        0     1542 2023-03-01 23:24:44.090788 openai-helper-0.2.1/openai_helper/dmo/chat_message_formatter.py
+-rw-r--r--   0        0        0     7698 2022-12-08 01:40:33.067448 openai-helper-0.2.1/openai_helper/dmo/completion_event_extractor.py
+-rw-r--r--   0        0        0     2566 2023-02-13 05:49:27.009400 openai-helper-0.2.1/openai_helper/dmo/etl_handle_textcompletions.py
+-rw-r--r--   0        0        0     1351 2023-02-25 18:10:04.895458 openai-helper-0.2.1/openai_helper/dmo/etl_remove_emojis.py
+-rw-r--r--   0        0        0     3095 2023-03-11 18:30:15.174565 openai-helper-0.2.1/openai_helper/dmo/etl_remove_listindicators.py
+-rw-r--r--   0        0        0     2871 2023-03-14 16:16:21.916983 openai-helper-0.2.1/openai_helper/dmo/etl_remove_promptindicators.py
+-rw-r--r--   0        0        0     1665 2022-11-16 18:34:53.819884 openai-helper-0.2.1/openai_helper/dmo/etl_replace_cliches.py
+-rw-r--r--   0        0        0     1496 2022-09-29 21:43:12.370296 openai-helper-0.2.1/openai_helper/dmo/etl_replace_duplicatedinput.py
+-rw-r--r--   0        0        0     4358 2023-05-03 23:55:05.690716 openai-helper-0.2.1/openai_helper/dmo/input_token_counter.py
+-rw-r--r--   0        0        0     1172 2022-11-16 18:34:53.819381 openai-helper-0.2.1/openai_helper/dmo/no_openai_event.py
+-rw-r--r--   0        0        0     1719 2022-11-16 18:14:14.917879 openai-helper-0.2.1/openai_helper/dmo/openai_connector.py
+-rw-r--r--   0        0        0     6943 2023-03-01 23:21:18.381290 openai-helper-0.2.1/openai_helper/dmo/output_extractor_chat.py
+-rw-r--r--   0        0        0     8110 2023-03-01 23:21:47.463789 openai-helper-0.2.1/openai_helper/dmo/output_extractor_text.py
+-rw-r--r--   0        0        0      268 2023-03-16 18:41:15.424607 openai-helper-0.2.1/openai_helper/svc/__init__.py
+-rw-r--r--   0        0        0     2985 2022-11-19 06:19:01.788211 openai-helper-0.2.1/openai_helper/svc/create_openai_answer.py
+-rw-r--r--   0        0        0     2390 2023-03-25 05:55:44.937494 openai-helper-0.2.1/openai_helper/svc/extract_primary_topic.py
+-rw-r--r--   0        0        0     2554 2022-11-16 18:34:53.819884 openai-helper-0.2.1/openai_helper/svc/extract_top_response.py
+-rw-r--r--   0        0        0     5301 2023-03-28 16:40:16.616677 openai-helper-0.2.1/openai_helper/svc/run_chat_completion.py
+-rw-r--r--   0        0        0     8919 2023-04-27 00:03:17.192201 openai-helper-0.2.1/openai_helper/svc/run_text_completion.py
+-rw-r--r--   0        0        0     2191 2023-05-03 23:54:42.483212 openai-helper-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4102 2023-03-27 18:14:05.658957 openai-helper-0.2.1/README.md
+-rw-r--r--   0        0        0     4903 2023-05-04 00:01:13.710212 openai-helper-0.2.1/setup.py
+-rw-r--r--   0        0        0     4983 2023-05-04 00:01:13.710712 openai-helper-0.2.1/PKG-INFO
```

### Comparing `openai-helper-0.2.0/openai_helper/__init__.py` & `openai-helper-0.2.1/openai_helper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,16 +191,15 @@
     try:
 
         bp = OpenAITextCompletion()
 
         d_result = bp.run(
             input_prompt=input_prompt,
             engine=engine,
-            temperature=temperature,
-            max_tokens=4096)
+            temperature=temperature)
 
         result = OutputExtractorText().process(
             input_text=input_prompt,
             d_result=d_result,
             remove_emojis=remove_emojis)
 
         if logger.isEnabledFor(logging.DEBUG):
```

### Comparing `openai-helper-0.2.0/openai_helper/bp/openai_chat_completion.py` & `openai-helper-0.2.1/openai_helper/bp/openai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/bp/openai_custom_model.py` & `openai-helper-0.2.1/openai_helper/bp/openai_custom_model.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/bp/openai_text_completion.py` & `openai-helper-0.2.1/openai_helper/bp/openai_text_completion.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/__init__.py` & `openai-helper-0.2.1/openai_helper/dmo/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/chat_message_formatter.py` & `openai-helper-0.2.1/openai_helper/dmo/chat_message_formatter.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/completion_event_extractor.py` & `openai-helper-0.2.1/openai_helper/dmo/completion_event_extractor.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/etl_handle_textcompletions.py` & `openai-helper-0.2.1/openai_helper/dmo/etl_handle_textcompletions.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/etl_remove_emojis.py` & `openai-helper-0.2.1/openai_helper/dmo/etl_remove_emojis.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/etl_remove_listindicators.py` & `openai-helper-0.2.1/openai_helper/dmo/etl_remove_listindicators.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/etl_remove_promptindicators.py` & `openai-helper-0.2.1/openai_helper/dmo/etl_remove_promptindicators.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/etl_replace_cliches.py` & `openai-helper-0.2.1/openai_helper/dmo/etl_replace_cliches.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/etl_replace_duplicatedinput.py` & `openai-helper-0.2.1/openai_helper/dmo/etl_replace_duplicatedinput.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/input_token_counter.py` & `openai-helper-0.2.1/openai_helper/dmo/input_token_counter.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from typing import List
 
 from tiktoken.core import Encoding
 from tiktoken import encoding_for_model
 
 from baseblock import BaseObject
 
+GPT35_TURBO_LATEST = 'gpt-3.5-turbo-0301'
+GPT4_LATEST = 'gpt-4-0314'
+
 
 class InputTokenCounter(BaseObject):
     """ Count Tokens accurately with Tiktoken
 
     Encoding Name       OpenAI Models
     cl100k_base	        gpt-4
                         gpt-3.5-turbo
@@ -29,14 +32,18 @@
     def __init__(self):
         """ Change Log
 
         Created:
             27-Mar-2023
             craigtrim@gmail.com
             *   https://github.com/craigtrim/openai-helper/issues/11
+        Updated:
+            3-May-2023
+            craigtrim@gmail.com
+            *   refactor model if/else conditions
         """
         BaseObject.__init__(self, __name__)
 
     def _cached_model(self,
                       model: str) -> Encoding:
         if model not in self.__d_encoding:
 
@@ -74,36 +81,39 @@
             int: the total tokens
         """
 
         if type(messages) == str:
             messages = [messages]
 
         if not model or not len(model):
-            model = 'gpt-3.5-turbo-0301'
+            model = GPT35_TURBO_LATEST
 
         encoding = self._cached_model(model)
 
-        if model == 'gpt-3.5-turbo':
-            self.logger.warning(
-                'Warning: gpt-3.5-turbo may change over time. Returning num tokens assuming gpt-3.5-turbo-0301.')
-            return self.process(messages, model='gpt-3.5-turbo-0301')
-
-        elif model == 'gpt-4':
-            self.logger.warning(
-                'Warning: gpt-4 may change over time. Returning num tokens assuming gpt-4-0314.')
-            return self.process(messages, model='gpt-4-0314')
-
-        elif model == 'gpt-3.5-turbo-0301':
-            # every message follows <|start|>{role/name}\n{content}<|end|>\n
+        if model == GPT35_TURBO_LATEST:
             tokens_per_message = 4
-            tokens_per_name = -1  # if there's a name, the role is omitted
 
-        elif model == 'gpt-4-0314':
+        elif model == GPT4_LATEST:
             tokens_per_message = 3
-            tokens_per_name = 1
+
+        elif model.startswith('gpt-3.5'):
+            if self.isEnabledForDebug:
+                self.logger.debug('\n'.join([
+                    'Model Assumption',
+                    f'\tSpecified Model: {model}',
+                    f'\tAssumed Model: {GPT35_TURBO_LATEST}']))
+            return self.process(messages=messages, model=GPT35_TURBO_LATEST)
+
+        elif model.startswith('gpt-4'):
+            if self.isEnabledForDebug:
+                self.logger.debug('\n'.join([
+                    'Model Assumption',
+                    f'\tSpecified Model: {model}',
+                    f'\tAssumed Model: {GPT4_LATEST}']))
+            return self.process(messages=messages, model=GPT4_LATEST)
 
         else:
             # raise NotImplementedError(
             #     f"""num_tokens_from_messages() is not implemented for model {model}. See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens.""")
             tokens_per_message = 4  # just some default ...
 
         num_tokens = 0
```

### Comparing `openai-helper-0.2.0/openai_helper/dmo/no_openai_event.py` & `openai-helper-0.2.1/openai_helper/dmo/no_openai_event.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/openai_connector.py` & `openai-helper-0.2.1/openai_helper/dmo/openai_connector.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/output_extractor_chat.py` & `openai-helper-0.2.1/openai_helper/dmo/output_extractor_chat.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/dmo/output_extractor_text.py` & `openai-helper-0.2.1/openai_helper/dmo/output_extractor_text.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/svc/create_openai_answer.py` & `openai-helper-0.2.1/openai_helper/svc/create_openai_answer.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/svc/extract_primary_topic.py` & `openai-helper-0.2.1/openai_helper/svc/extract_primary_topic.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/svc/extract_top_response.py` & `openai-helper-0.2.1/openai_helper/svc/extract_top_response.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/svc/run_chat_completion.py` & `openai-helper-0.2.1/openai_helper/svc/run_chat_completion.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/openai_helper/svc/run_text_completion.py` & `openai-helper-0.2.1/openai_helper/svc/run_text_completion.py`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/pyproject.toml` & `openai-helper-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "OpenAI Helper for Easy I/O"
 license = "MIT"
 name = "openai-helper"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 keywords = ["openai", "api", "utility"]
 repository = "https://github.com/craigtrim/openai-helper"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `openai-helper-0.2.0/README.md` & `openai-helper-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openai-helper-0.2.0/setup.py` & `openai-helper-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'openai>=0.27.0,<0.28.0', 'tiktoken']
 
 setup_kwargs = {
     'name': 'openai-helper',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'OpenAI Helper for Easy I/O',
     'long_description': '# OpenAI-Helper\nOpenAI Helper for Easy I/O\n\n## Github\nhttps://github.com/craigtrim/openai-helper\n\n## Usage\n\n###  Set the OpenAI credentials\n```python\nimport os\nos.environ[\'OPENAI_KEY\'] = "<encrypted key>"\nos.environ[\'OPENAI_ORG\'] = "<encrypted key>"\n```\n\nUse `CryptoBase.encrypt_str("...")` from https://pypi.org/project/baseblock/\n\n###  Initialize the OpenAI Helper:\n```python\nrun = OpenAITextCompletion().run\n```\nThis will connect to OpenAI and establish performant callbacks.\n\n### Call OpenAI:\n```python\nrun(input_prompt="Generate a one random number between 1 and 5000")\n```\n\nor\n```python\nrun(engine="text-ada-001",\n    temperature=1.0,\n    max_tokens=256,\n    input_prompt="Rewrite the input in grammatical English:\\n\\nInput: You believe I can help you understand what trust yourself? don\'t you?\\nOutput:\\n\\n")\n```\n\nThe output will contain both the input and output values:\n```json\n{\n   "input":{\n      "best_of":1,\n      "engine":"text-davinci-003",\n      "frequency_penalty":0.0,\n      "input_prompt":"Rewrite the input in grammatical English:\\n\\nInput: You believe I can help you understand what trust yourself? don\'t you?\\nOutput:\\n\\n",\n      "max_tokens":256,\n      "presence_penalty":2,\n      "temperature":1.0,\n      "timeout":5,\n      "top_p":1.0\n   },\n   "output":{\n      "choices":[\n         {\n            "finish_reason":"stop",\n            "index":0,\n            "logprobs":"None",\n            "text":"Don\'t you believe that I can help you understand trust in yourself?"\n         }\n      ],\n      "created":1659051242,\n      "id":"cmpl-5Z7IwXM5bCwWj8IuHaGnOLn6bCvHz",\n      "model":"text-ada-001",\n      "object":"text_completion",\n      "usage":{\n         "completion_tokens":17,\n         "prompt_tokens":32,\n         "total_tokens":49\n      }\n   }\n}\n```\n\n## Supported Parameters and Defaults\nThis method signature describes support:\n```python\ndef process(self,\n            input_prompt: str,\n            engine: str = None,\n            best_of: int = None,\n            temperature: float = None,\n            max_tokens: int = None,\n            top_p: float = None,\n            frequency_penalty: int = None,\n            presence_penalty: int = None) -> dict:\n    """ Run an OpenAI event\n\n    Args:\n        input_prompt (str): The Input Prompt to execute against OpenAI\n        engine (str, optional): The OpenAI model (engine) to run against. Defaults to None.\n            Options as of July, 2022 are:\n                \'text-davinci-003\'\n                \'text-curie-001\',\n                \'text-babbage-001\'\n                \'text-ada-001\'\n        best_of (int, optional): Generates Multiple Server-Side Combinations and only selects the best. Defaults to None.\n            This can really eat up OpenAI tokens so use with caution!\n        temperature (float, optional): Control Randomness; Scale is 0.0 - 1.0. Defaults to None.\n            Scale is 0.0 - 1.0\n            Lower values approach predictable outputs and determinate behavior\n            Higher values are more engaging but also less predictable\n            Use High Values cautiously\n        max_tokens (int, optional): The Maximum Number of tokens to generate. Defaults to None.\n            Requests can use up to 4,000 tokens (this takes the length of the input prompt into account)\n            The higher this value, the more each request will cost.\n        top_p (float, optional): Controls Diversity via Nucleus Sampling. Defaults to None.\n            no idea what this means\n        frequency_penalty (int, optional): How much to penalize new tokens based on their frequency in the text so far. Defaults to None.\n            Scale: 0.0 - 2.0.\n        presence_penalty (int, optional): Seems similar to frequency penalty. Defaults to None.\n\n    Returns:\n        dict: an output dictionary with two keys:\n            input: the input dictionary with validated parameters and default values where appropriate\n            output: the output event from OpenAI\n    """\n```\n\n## Counting Tokens (tiktoken)\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/openai-helper',
```

### Comparing `openai-helper-0.2.0/PKG-INFO` & `openai-helper-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-helper
-Version: 0.2.0
+Version: 0.2.1
 Summary: OpenAI Helper for Easy I/O
 Home-page: https://github.com/craigtrim/openai-helper
 License: MIT
 Keywords: openai,api,utility
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
```

