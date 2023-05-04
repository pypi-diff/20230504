# Comparing `tmp/openai-tools-0.0.0.1.tar.gz` & `tmp/openai-tools-0.0.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-tools-0.0.0.1.tar", last modified: Thu May  4 03:00:21 2023, max compression
+gzip compressed data, was "openai-tools-0.0.0.1.dev0.tar", last modified: Thu May  4 03:40:48 2023, max compression
```

## Comparing `openai-tools-0.0.0.1.tar` & `openai-tools-0.0.0.1.dev0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:00:21.519626 openai-tools-0.0.0.1/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     3093 2023-05-03 19:41:46.000000 openai-tools-0.0.0.1/.gitignore
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1/LICENSE
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2182 2023-05-04 03:00:21.519449 openai-tools-0.0.0.1/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)      236 2023-05-04 02:57:55.000000 openai-tools-0.0.0.1/Pipfile
--rw-r--r--   0 avsolatorio   (501) staff       (20)       11 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1/README.md
--rw-r--r--   0 avsolatorio   (501) staff       (20)     1258 2023-05-04 02:59:03.000000 openai-tools-0.0.0.1/pyproject.toml
--rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-05-04 03:00:21.519680 openai-tools-0.0.0.1/setup.cfg
--rw-r--r--   0 avsolatorio   (501) staff       (20)      128 2023-05-04 02:57:19.000000 openai-tools-0.0.0.1/setup.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:00:21.516424 openai-tools-0.0.0.1/src/
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:00:21.518051 openai-tools-0.0.0.1/src/openai_tools/
--rw-r--r--   0 avsolatorio   (501) staff       (20)       24 2023-05-03 19:41:11.000000 openai-tools-0.0.0.1/src/openai_tools/__init__.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     6936 2023-05-04 02:38:35.000000 openai-tools-0.0.0.1/src/openai_tools/prompt.py
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2281 2023-05-04 02:44:20.000000 openai-tools-0.0.0.1/src/openai_tools/utils.py
-drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:00:21.519177 openai-tools-0.0.0.1/src/openai_tools.egg-info/
--rw-r--r--   0 avsolatorio   (501) staff       (20)     2182 2023-05-04 03:00:21.000000 openai-tools-0.0.0.1/src/openai_tools.egg-info/PKG-INFO
--rw-r--r--   0 avsolatorio   (501) staff       (20)      341 2023-05-04 03:00:21.000000 openai-tools-0.0.0.1/src/openai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-05-04 03:00:21.000000 openai-tools-0.0.0.1/src/openai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       72 2023-05-04 03:00:21.000000 openai-tools-0.0.0.1/src/openai_tools.egg-info/requires.txt
--rw-r--r--   0 avsolatorio   (501) staff       (20)       23 2023-05-04 03:00:21.000000 openai-tools-0.0.0.1/src/openai_tools.egg-info/top_level.txt
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:40:48.641141 openai-tools-0.0.0.1.dev0/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     3093 2023-05-03 19:41:46.000000 openai-tools-0.0.0.1.dev0/.gitignore
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1075 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev0/LICENSE
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1342 2023-05-04 02:56:41.000000 openai-tools-0.0.0.1.dev0/Makefile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-04 03:40:48.640966 openai-tools-0.0.0.1.dev0/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      236 2023-05-04 02:57:55.000000 openai-tools-0.0.0.1.dev0/Pipfile
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       11 2023-05-03 19:36:38.000000 openai-tools-0.0.0.1.dev0/README.md
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     1258 2023-05-04 02:59:03.000000 openai-tools-0.0.0.1.dev0/pyproject.toml
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       38 2023-05-04 03:40:48.641192 openai-tools-0.0.0.1.dev0/setup.cfg
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      128 2023-05-04 02:57:19.000000 openai-tools-0.0.0.1.dev0/setup.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:40:48.638136 openai-tools-0.0.0.1.dev0/src/
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:40:48.639854 openai-tools-0.0.0.1.dev0/src/openai_tools/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       29 2023-05-04 03:40:07.000000 openai-tools-0.0.0.1.dev0/src/openai_tools/__init__.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     7162 2023-05-04 03:38:30.000000 openai-tools-0.0.0.1.dev0/src/openai_tools/prompt.py
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2788 2023-05-04 03:26:59.000000 openai-tools-0.0.0.1.dev0/src/openai_tools/utils.py
+drwxr-xr-x   0 avsolatorio   (501) staff       (20)        0 2023-05-04 03:40:48.640686 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/
+-rw-r--r--   0 avsolatorio   (501) staff       (20)     2187 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 avsolatorio   (501) staff       (20)      350 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)        1 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       72 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/requires.txt
+-rw-r--r--   0 avsolatorio   (501) staff       (20)       23 2023-05-04 03:40:48.000000 openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/top_level.txt
```

### Comparing `openai-tools-0.0.0.1/.gitignore` & `openai-tools-0.0.0.1.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1/LICENSE` & `openai-tools-0.0.0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1/PKG-INFO` & `openai-tools-0.0.0.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-tools
-Version: 0.0.0.1
+Version: 0.0.0.1.dev0
 Summary: A Python wrapper for managing OpenAI API.
 Author-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 Maintainer-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Aivin V. Solatorio
```

### Comparing `openai-tools-0.0.0.1/pyproject.toml` & `openai-tools-0.0.0.1.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-tools-0.0.0.1/src/openai_tools/prompt.py` & `openai-tools-0.0.0.1.dev0/src/openai_tools/prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import json
 from pathlib import Path
 import openai
 import backoff
 
 from jinja2 import Template
-from .utils import num_tokens_from_messages, build_prompt_id
+from .utils import num_tokens_from_messages, build_prompt_id, get_message_hash
 
 
 # Load the OpenAI API key from the environment variable.
 openai.api_key = os.environ.get('OPENAI_API_KEY')
 
 
 class OpenAIException(BaseException):
@@ -115,58 +115,63 @@
 
         # Create the message to send to the GPT-3 model.
         message = [
             dict(role="system", content=system_content),
             dict(role="user", content=content),
         ]
 
-        return message
+        message_hash = get_message_hash(message)
+
+        return dict(message=message, message_hash=message_hash)
 
     def send_prompt(self, user_content: str, user_template: str = None, system_content: str = None, metadata: dict = None, api_kwargs: dict = None, return_data: bool = False):
         """Send the prompt to the GPT-3 model.
         Args:
             variables (dict): The variables to classify.
         """
         if api_kwargs:
             api_kwargs = {**self.default_api_kwargs, **api_kwargs}
         else:
             api_kwargs = self.default_api_kwargs
 
-        message = self.build_message(
+        pack = self.build_message(
             user_content=user_content,
             user_template=user_template,
             system_content=system_content,
         )
+        message = pack["message"]
+        message_hash = pack["message_hash"]
+
+        # # Apply cleaning to the message.
+        # message = self._clean_message(message)
 
-        # Apply cleaning to the message.
-        message = self._clean_message(message)
+        # Create the directory for the prompt.
+        prompt_id = build_prompt_id(user_template, system_content, api_kwargs)
+        data_type_dir = self.payloads_dir / self.task_label / prompt_id
+        data_type_dir.mkdir(parents=True, exist_ok=True)
 
-        max_tokens = self.total_tokens -  self.calculate_prompt_tokens(message=message)
+        max_tokens = self.total_tokens - self.calculate_prompt_tokens(message=message)
         api_kwargs["max_tokens"] = max_tokens
 
         response = chat_completion_with_backoff(messages=message, **api_kwargs)
 
         data = dict(
             message=message,
             response=response,
             content=response["choices"][0]["message"]["content"],
             api_kwargs=api_kwargs,
             metadata=metadata or {},
+            message_hash=message_hash,
         )
 
         fid = f't{response["created"]}_{response["id"]}.json'
 
         if self.prompt_label is not None:
             fid = f'{self.prompt_label}_{fid}'
 
-        # Create the directory for the prompt.
-        prompt_id = build_prompt_id(user_template, system_content, api_kwargs)
-        data_type_dir = self.payloads_dir / self.task_label / prompt_id
-        data_type_dir.mkdir(parents=True, exist_ok=True)
-
         # Save the data to the file.
         (data_type_dir / fid).write_text(json.dumps(data, indent=2))
 
         if return_data:
             return data
```

### Comparing `openai-tools-0.0.0.1/src/openai_tools/utils.py` & `openai-tools-0.0.0.1.dev0/src/openai_tools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,7 +57,21 @@
 
     k_dict["system_content"] = system_content
     k_dict["user_template"] = user_template
 
     jkey = json.dumps(k_dict, sort_keys=True)
 
     return f"{uuid.UUID(hashlib.md5(jkey.encode('utf-8')).hexdigest())}"
+
+
+def get_message_hash(message):
+    """Returns a hash of the message."""
+    # https://platform.openai.com/docs/guides/chat/introduction
+    #
+    # The message is a list of dictionary objects, where each dictionary
+    # represents a message from a user or the system.
+
+    # The hash is calculated by converting the message to a JSON string,
+    # sorting the keys, and then hashing the JSON string.
+    jkey = json.dumps(message, sort_keys=True)
+
+    return hashlib.md5(jkey.encode('utf-8')).hexdigest()
```

### Comparing `openai-tools-0.0.0.1/src/openai_tools.egg-info/PKG-INFO` & `openai-tools-0.0.0.1.dev0/src/openai_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-tools
-Version: 0.0.0.1
+Version: 0.0.0.1.dev0
 Summary: A Python wrapper for managing OpenAI API.
 Author-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 Maintainer-email: "Aivin V. Solatorio" <avsolatorio@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Aivin V. Solatorio
```

