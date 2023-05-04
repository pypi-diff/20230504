# Comparing `tmp/chatsnack-0.1.1.tar.gz` & `tmp/chatsnack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatsnack-0.1.1.tar", max compression
+gzip compressed data, was "chatsnack-0.1.2.tar", max compression
```

## Comparing `chatsnack-0.1.1.tar` & `chatsnack-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3795 2023-04-15 22:05:43.794976 chatsnack-0.1.1/chatsnack/__init__.py
--rw-r--r--   0        0        0     4377 2023-04-20 15:54:25.082285 chatsnack-0.1.1/chatsnack/aiwrapper.py
--rw-r--r--   0        0        0     1498 2023-04-09 18:26:53.563580 chatsnack-0.1.1/chatsnack/asynchelpers.py
--rw-r--r--   0        0        0     4314 2023-04-15 22:37:13.637936 chatsnack-0.1.1/chatsnack/chat/__init__.py
--rw-r--r--   0        0        0     7251 2023-04-20 00:43:48.231066 chatsnack-0.1.1/chatsnack/chat/mixin_messages.py
--rw-r--r--   0        0        0     1822 2023-04-20 16:16:53.508658 chatsnack-0.1.1/chatsnack/chat/mixin_params.py
--rw-r--r--   0        0        0     6192 2023-04-20 02:48:35.762239 chatsnack-0.1.1/chatsnack/chat/mixin_query.py
--rw-r--r--   0        0        0     3345 2023-04-23 15:02:14.751611 chatsnack-0.1.1/chatsnack/chat/mixin_serialization.py
--rw-r--r--   0        0        0      929 2023-04-09 15:02:47.382274 chatsnack-0.1.1/chatsnack/defaults.py
--rw-r--r--   0        0        0     1306 2023-04-09 15:11:16.782131 chatsnack-0.1.1/chatsnack/fillings.py
--rw-r--r--   0        0        0       25 2023-04-09 16:04:20.190406 chatsnack-0.1.1/chatsnack/packs/__init__.py
--rw-r--r--   0        0        0    19461 2023-04-14 02:01:22.528095 chatsnack-0.1.1/chatsnack/packs/default_packs/ChatsnackHelper.yml
--rw-r--r--   0        0        0      762 2023-04-14 02:00:30.545934 chatsnack-0.1.1/chatsnack/packs/default_packs/Chester.yml
--rw-r--r--   0        0        0      811 2023-04-14 01:57:06.309659 chatsnack-0.1.1/chatsnack/packs/default_packs/Confectioner.yml
--rw-r--r--   0        0        0      889 2023-04-14 01:57:06.272212 chatsnack-0.1.1/chatsnack/packs/default_packs/Data.yml
--rw-r--r--   0        0        0      736 2023-04-14 01:57:06.293264 chatsnack-0.1.1/chatsnack/packs/default_packs/Jane.yml
--rw-r--r--   0        0        0      905 2023-04-14 01:57:06.327853 chatsnack-0.1.1/chatsnack/packs/default_packs/Jolly.yml
--rw-r--r--   0        0        0      948 2023-04-20 16:08:12.961032 chatsnack-0.1.1/chatsnack/packs/default_packs/Summarizer.yml
--rw-r--r--   0        0        0     2831 2023-04-11 01:07:43.121823 chatsnack-0.1.1/chatsnack/packs/module_help_vendor.py
--rw-r--r--   0        0        0     4028 2023-04-20 15:50:28.683064 chatsnack-0.1.1/chatsnack/packs/snackpacks.py
--rw-r--r--   0        0        0     1229 2023-04-06 15:39:54.021402 chatsnack-0.1.1/chatsnack/txtformat.py
--rw-r--r--   0        0        0     3976 2023-04-20 00:41:01.746999 chatsnack-0.1.1/chatsnack/yamlformat.py
--rw-r--r--   0        0        0     1091 2023-04-14 18:33:08.190283 chatsnack-0.1.1/LICENSE
--rw-r--r--   0        0        0     1005 2023-04-23 14:59:28.992433 chatsnack-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9118 2023-04-16 02:49:38.675864 chatsnack-0.1.1/README.md
--rw-r--r--   0        0        0    10040 1970-01-01 00:00:00.000000 chatsnack-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3795 2023-04-15 22:05:43.794976 chatsnack-0.1.2/chatsnack/__init__.py
+-rw-r--r--   0        0        0     5793 2023-04-23 19:18:42.180282 chatsnack-0.1.2/chatsnack/aiwrapper.py
+-rw-r--r--   0        0        0     1498 2023-04-09 18:26:53.563580 chatsnack-0.1.2/chatsnack/asynchelpers.py
+-rw-r--r--   0        0        0     4486 2023-04-29 02:58:40.680324 chatsnack-0.1.2/chatsnack/chat/__init__.py
+-rw-r--r--   0        0        0     6844 2023-04-29 03:01:10.662761 chatsnack-0.1.2/chatsnack/chat/mixin_messages.py
+-rw-r--r--   0        0        0     4948 2023-04-29 14:36:32.098051 chatsnack-0.1.2/chatsnack/chat/mixin_params.py
+-rw-r--r--   0        0        0     6966 2023-04-29 03:01:48.045271 chatsnack-0.1.2/chatsnack/chat/mixin_query.py
+-rw-r--r--   0        0        0     3345 2023-04-23 15:02:14.751611 chatsnack-0.1.2/chatsnack/chat/mixin_serialization.py
+-rw-r--r--   0        0        0      929 2023-04-09 15:02:47.382274 chatsnack-0.1.2/chatsnack/defaults.py
+-rw-r--r--   0        0        0     1306 2023-04-09 15:11:16.782131 chatsnack-0.1.2/chatsnack/fillings.py
+-rw-r--r--   0        0        0       25 2023-04-09 16:04:20.190406 chatsnack-0.1.2/chatsnack/packs/__init__.py
+-rw-r--r--   0        0        0    19461 2023-04-14 02:01:22.528095 chatsnack-0.1.2/chatsnack/packs/default_packs/ChatsnackHelper.yml
+-rw-r--r--   0        0        0      762 2023-04-14 02:00:30.545934 chatsnack-0.1.2/chatsnack/packs/default_packs/Chester.yml
+-rw-r--r--   0        0        0      811 2023-04-14 01:57:06.309659 chatsnack-0.1.2/chatsnack/packs/default_packs/Confectioner.yml
+-rw-r--r--   0        0        0      889 2023-04-14 01:57:06.272212 chatsnack-0.1.2/chatsnack/packs/default_packs/Data.yml
+-rw-r--r--   0        0        0      736 2023-04-14 01:57:06.293264 chatsnack-0.1.2/chatsnack/packs/default_packs/Jane.yml
+-rw-r--r--   0        0        0      905 2023-04-14 01:57:06.327853 chatsnack-0.1.2/chatsnack/packs/default_packs/Jolly.yml
+-rw-r--r--   0        0        0     1244 2023-04-23 18:55:56.684760 chatsnack-0.1.2/chatsnack/packs/default_packs/Summarizer.yml
+-rw-r--r--   0        0        0     2877 2023-05-03 23:27:38.108990 chatsnack-0.1.2/chatsnack/packs/module_help_vendor.py
+-rw-r--r--   0        0        0     4028 2023-04-20 15:50:28.683064 chatsnack-0.1.2/chatsnack/packs/snackpacks.py
+-rw-r--r--   0        0        0     1229 2023-04-06 15:39:54.021402 chatsnack-0.1.2/chatsnack/txtformat.py
+-rw-r--r--   0        0        0     3976 2023-04-20 00:41:01.746999 chatsnack-0.1.2/chatsnack/yamlformat.py
+-rw-r--r--   0        0        0     1091 2023-04-14 18:33:08.190283 chatsnack-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1005 2023-05-04 00:33:19.775893 chatsnack-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9186 2023-04-29 00:10:57.640242 chatsnack-0.1.2/README.md
+-rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 chatsnack-0.1.2/PKG-INFO
```

### Comparing `chatsnack-0.1.1/chatsnack/__init__.py` & `chatsnack-0.1.2/chatsnack/__init__.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/aiwrapper.py` & `chatsnack-0.1.2/chatsnack/aiwrapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         user = "_not_set"
     # prompt will be in JSON format, let us translate it to a python list
     # if the prompt is a list already, we will just use it as is
     if isinstance(prompt, list):
         messages = prompt
     else:
         messages = json.loads(prompt)
-    logger.debug("""Chat Query:
+    logger.trace("""Chat Query:
     Prompt: {0}
     Model: {2}, Max Tokens: {3}, Stop: {5}, Temperature: {1}, Top-P: {4}, Presence Penalty {6}, Frequency Penalty: {7}, N: {8}, Stream: {9}, User: {10}
     """,prompt, temperature, engine, max_tokens, top_p, stop, presence_penalty, frequency_penalty, n, stream, user)
     response = await openai.ChatCompletion.acreate(model=engine,
                                             messages=messages,
                                             max_tokens=max_tokens,
                                             temperature=temperature,
@@ -91,7 +91,36 @@
                             frequency_penalty=frequency_penalty,
                             stop=stop,
                             n=n,
                             stream=stream,
                             user=user)
 
     return _trimmed_fetch_chat_response(resp, n)
+
+# TODO: Add back support for content classification (i.e. is this text NSFW?)
+# TODO: Consider adding support for other local language models
+
+# Structure of this code is based on some methods from github.com/OthersideAI/chronology
+# licensed under this MIT License:
+######
+# MIT License
+#
+# Copyright (c) 2020 OthersideAI
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#######
```

### Comparing `chatsnack-0.1.1/chatsnack/asynchelpers.py` & `chatsnack-0.1.2/chatsnack/asynchelpers.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/chat/__init__.py` & `chatsnack-0.1.2/chatsnack/chat/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,45 +12,48 @@
 from .mixin_params import ChatParams, ChatParamsMixin
 from .mixin_serialization import DatafileMixin, ChatSerializationMixin
 
 
 
 ########################################################################################################################
 # Core datafile classes of Plunkychat
-# (1) Chat, high-level class that symbolizes a prompt/request, can reference other Chat objects to create a chain
+# (1) Chat, high-level class that symbolizes a prompt/request/response, can reference other Chat objects to chain
 # (2) ChatParams, used only in Chat, includes parameters like engine name and other OpenAI params.
-# (3) Text, this is a text blob we save to disk, can be used as a reference inside chat messages (vending machine)
+# (3) Text, this is a text blob we save to disk, can be used as a reference inside chat messages ('snack fillings')
 
-# just a little hack to remove the schema enforcement warning from datafiles
 @datafile(CHATSNACK_BASE_DIR + "/{self.name}.txt", manual=True)
 class Text(DatafileMixin):
     name: str
     content: Optional[str] = None
-    # TODO: All Text and Chat objects should automatically be added to the vending machine (even if not saved to disk)
+    # TODO: All Text and Chat objects should automatically be added as snack fillings (even if not saved to disk)
 
 
 @datafile(CHATSNACK_BASE_DIR + "/{self.name}.yml", manual=True, init=False)
-class Chat(ChatParamsMixin, ChatQueryMixin, ChatSerializationMixin):
+class Chat(ChatQueryMixin, ChatSerializationMixin):
     """ A chat prompt that can be expanded into a chat ⭐"""
     # title should be just like above but with a GUID at the end
     name: str = field(default_factory=lambda: f"_ChatPrompt-{datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}-{uuid.uuid4()}")
     params: Optional[ChatParams] = None
+    # ChatMessage is more of a hack class to avoid datafiles schema reference issues for dict serialization
     messages: List[ChatMessage] = field(default_factory=lambda: [])
 
-    # we want to be able to support passing in a system message as well as the datafile fields
     def __init__(self, *args, **kwargs):
         """ 
         Initializes the chat prompt
+        :param args: if we get one arg, we'll assume it's the system message
+                        if we get two args, the first is the name and the second is the system message
+
+        :param kwargs: (keyword arguments are as follows)
         :param name: the name of the chat prompt (optional, defaults to _ChatPrompt-<date>-<uuid>)
         :param params: the engine parameters (optional, defaults to None)
         :param messages: the messages (optional, defaults to [])
         :param system: the initial system message (optional, defaults to None)
         """
 
-        # get name from kwargs
+        # get name from kwargs, if it's there
         if "name" in kwargs:
             self.name = kwargs["name"]
         else:
             # if we get two args, the first is the name and the second is the system message
             if len(args) == 2:
                 self.name = args[0]
             else:
```

### Comparing `chatsnack-0.1.1/chatsnack/chat/mixin_messages.py` & `chatsnack-0.1.2/chatsnack/chat/mixin_messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,24 +91,14 @@
         if len(self.messages) > 0:
             last_message = self.messages[-1]
             return last_message[list(last_message.keys())[-1]]
         else:
             return None
 
     @property
-    def response(self) -> str:
-        """ Returns the value of the last assistant message in the chat prompt ⭐"""
-        last_assistant_message = None
-        for _message in self.messages:
-            message = self._msg_dict(_message)
-            if "assistant" in message:
-                last_assistant_message = message["assistant"]
-        return last_assistant_message
-
-    @property
     def system_message(self) -> str:
         """ Returns the first system message, if any """
         # get the first message that has a key of "system"
         for _message in self.messages:
             message = self._msg_dict(_message)
             if "system" in message:
                 return message["system"]
@@ -153,8 +143,7 @@
                     if include_chatprompt is None:
                         raise ValueError(f"Could not find 'include' prompt with name: {content}")
                     # get_expanded_messages from the include_chatprompt and add them to the new_messages, they're already formatted how we want
                     new_messages.extend(include_chatprompt.get_messages())
                 else:
                     new_messages.append({"role": role, "content": content})
         return new_messages
-
```

### Comparing `chatsnack-0.1.1/chatsnack/chat/mixin_query.py` & `chatsnack-0.1.2/chatsnack/chat/mixin_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import asyncio
 import json
 import uuid
 from datetime import datetime
+from typing import Dict, List, Optional
 
 from loguru import logger
+from datafiles import datafile
 
 from ..asynchelpers import aformatter
 from ..aiwrapper import cleaned_chat_completion
 from ..fillings import filling_machine
 
 from .mixin_messages import ChatMessagesMixin
+from .mixin_params import ChatParamsMixin
 
-
-class ChatQueryMixin(ChatMessagesMixin):
+class ChatQueryMixin(ChatMessagesMixin, ChatParamsMixin):
     # async method that gathers will execute an async format method on every message in the chat prompt and gather the results into a final json string
     async def _gather_format(self, format_coro, **kwargs) -> str:
         new_messages = self.get_messages()
 
         # we now apply the format_coro to the content of each message in each dictionary in the list
         coros = []
         for message in new_messages:
@@ -55,14 +57,26 @@
         prompt = await prompter._build_final_prompt(additional_vars)
         if self.params is None:
             return prompt, await cleaned_chat_completion(prompt)
         else:
             pparams = prompter.params._get_non_none_params()
             return prompt, await cleaned_chat_completion(prompt, **pparams)
 
+    @property
+    def response(self) -> str:
+        """ Returns the value of the last assistant message in the chat prompt ⭐"""
+        last_assistant_message = None
+        for _message in self.messages:
+            message = self._msg_dict(_message)
+            if "assistant" in message:
+                last_assistant_message = message["assistant"]
+        # filter the response if we have a pattern
+        last_assistant_message = self.filter_by_pattern(last_assistant_message)
+        return last_assistant_message
+
     def __call__(self, usermsg=None, **additional_vars) -> object:
         """ Executes the query as-is and returns a Chat object with the response, shortcut for Chat.chat()"""
         if usermsg is not None:
             additional_vars["__user"] = usermsg
         return self.chat(**additional_vars)
  
     def ask(self, usermsg=None, **additional_vars) -> str:
@@ -82,14 +96,16 @@
             additional_vars["__user"] = usermsg
         return asyncio.run(self.chat_a(**additional_vars))
     async def ask_a(self, usermsg=None, **additional_vars) -> str:
         """ Executes the query as-is, async version of ask()"""
         if usermsg is not None:
             additional_vars["__user"] = usermsg
         _, response = await self._submit_for_response_and_prompt(**additional_vars)
+        # filter the response if we have a pattern
+        response = self.filter_by_pattern(response)
         return response
     async def chat_a(self, usermsg=None, **additional_vars) -> object:
         """ Executes the query as-is, and returns a ChatPrompt object that contains the response. Async version of chat()"""
         if usermsg is not None:
             additional_vars["__user"] = usermsg
         prompt, response = await self._submit_for_response_and_prompt(**additional_vars)
         # create a new chatprompt with the new name, copy it from this one
```

### Comparing `chatsnack-0.1.1/chatsnack/chat/mixin_serialization.py` & `chatsnack-0.1.2/chatsnack/chat/mixin_serialization.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/defaults.py` & `chatsnack-0.1.2/chatsnack/defaults.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/fillings.py` & `chatsnack-0.1.2/chatsnack/fillings.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/packs/default_packs/ChatsnackHelper.yml` & `chatsnack-0.1.2/chatsnack/packs/default_packs/ChatsnackHelper.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/packs/default_packs/Chester.yml` & `chatsnack-0.1.2/chatsnack/packs/default_packs/Chester.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/packs/default_packs/Confectioner.yml` & `chatsnack-0.1.2/chatsnack/packs/default_packs/Confectioner.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/packs/default_packs/Data.yml` & `chatsnack-0.1.2/chatsnack/packs/default_packs/Data.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/packs/default_packs/Jane.yml` & `chatsnack-0.1.2/chatsnack/packs/default_packs/Jane.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/packs/default_packs/Jolly.yml` & `chatsnack-0.1.2/chatsnack/packs/default_packs/Jolly.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/packs/default_packs/Summarizer.yml` & `chatsnack-0.1.2/chatsnack/packs/default_packs/Summarizer.yml`

 * *Files 20% similar despite different names*

```diff
@@ -8,10 +8,13 @@
       concise summararies of any text document.
       (2) Elaborate on 3 more protips used by the world's best summarizers to
       avoid losing important details and context.
       (3) Now specifically consider the user's input. Use your expertise and your own guidance,
       describe in great detail how an author could apply that wisdom to summarize the user's 
       text properly. What considerations come to mind? What is the user expecting?
       (4) Finally, use everything above to author a concise summary of the user's input that will
-      delight them with your summarization skills. The summary should be prefixed with 
-      "CONCISE_SUMMARY:" on a line by itself.
+      delight them with your summarization skills. Ensure you include all significant events and 
+      details from the passage while maintaining a logical flow and coherence.Pay attention to the
+      tone and engagement in the original passage, and try to reflect that in the summary to 
+      create a more enjoyable reading experience.
+      Finally summary should be prefixed with "CONCISE_SUMMARY:" on a line by itself.
```

### Comparing `chatsnack-0.1.1/chatsnack/packs/module_help_vendor.py` & `chatsnack-0.1.2/chatsnack/packs/module_help_vendor.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 
     return output
 
 def _process_function(func, cls=None):
     output = []
 
     signature = inspect.signature(func)
-    params = ', '.join(f"{name}{': ' + param.annotation.__name__ if param.annotation is not inspect.Parameter.empty else ''}" for name, param in signature.parameters.items())
+    params = ', '.join(f"{name}{': ' + param.annotation.__name__ if (param.annotation is not inspect.Parameter.empty and hasattr(param.annotation, '__name__')) else ''}" for name, param in signature.parameters.items())
+
 
     func_name = f"{cls.__name__}.{func.__name__}" if cls else func.__name__
 
     output.append(f"\n{func_name}({params})")
     docstring = get_docstring(func)
     if docstring:
         output.append(f'"""\n{docstring}"""')
```

### Comparing `chatsnack-0.1.1/chatsnack/packs/snackpacks.py` & `chatsnack-0.1.2/chatsnack/packs/snackpacks.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/txtformat.py` & `chatsnack-0.1.2/chatsnack/txtformat.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/chatsnack/yamlformat.py` & `chatsnack-0.1.2/chatsnack/yamlformat.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/LICENSE` & `chatsnack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.1/pyproject.toml` & `chatsnack-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatsnack"
-version = "0.1.1"
+version = "0.1.2"
 description = "chatsnack is the easiest Python library for rapid development with OpenAI's ChatGPT API. It provides an intuitive interface for creating and managing chat-based prompts and responses, making it convenient to build complex, interactive conversations with AI."
 authors = ["Mattie Casper"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `chatsnack-0.1.1/README.md` & `chatsnack-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 ## Setup
 
 ### Got snack?
 
 Install the `chatsnack` package from PyPI:
 
 ```bash
+# requires Python 3.10+
 pip install chatsnack
 ```
 
 ### Got keys?
 
-Add your OpenAI API key to your .env file. If you don't have a .env file, the library will create a new one for you. You can use env.template.cataclysm as an example.
+Add your OpenAI API key to your .env file. If you don't have a .env file, the library will create a new one for you in the local directory.
 
 ### Learn More!
-Read more below, watch the [video](https://youtu.be/ZK8fUuQDgZ4) or check out the [Getting Started notebook](notebooks/).
+Read more below, watch the [intro video](https://www.youtube.com/watch?v=Yjwi54rHrhw) or check out the [Getting Started notebook](notebooks/).
 
 ## Usage
 
 ### Enjoy a Quick Snack
 
 Easiest way to get going with `chatsnack` is with built-in snack packs. Each pack is a singleton ready to mingleton.
 
@@ -129,15 +130,15 @@
   print(midnightsnack.ask())
   ```
   > *"POPSICLE."*
     
 
 #### Adjusting Cooking Temperatures
 
-By default, `gpt-3.5-turbo` is the default chat API with a default temperature of `0.5`. If you prefer, you can change OpenAI parameters for each chat, such as the engine and temperature:
+By default, `gpt-3.5-turbo` is the default chat API with a default temperature of `0.7`. If you prefer, you can change OpenAI parameters for each chat, such as the engine and temperature:
 
 ```python
 from chatsnack import Chat
 wisechat = Chat("Respond with professional writing based on the user query.")
 wisechat.user("Author an alliterative poem about good snacks to eat with coffee.")
 wisechat.engine = "gpt-4"
 wisechat.temperature = 0.8
@@ -188,15 +189,15 @@
 
 ##### Quick Assistants
 
 Also, `.asst()` is an alias shortcut for `.assistant()` if you want you code to align cleanly with other 4-letter `.user()` and `.chat()` calls.
 
 ##### Binge-chaining
 
-If you're feeling wild, you can actually call any chat (like a function) and it'll submit the chat and continue, just like `.chat()`. This allows even more terse chaining. This can come in handy when you're looking for 
+If you're feeling wild, you can actually call any chat (like a function) and it'll submit the chat and continue, just like `.chat()`. This allows even more terse chaining. This can come in handy when you're looking for chain-of-thought prompting or prewriting priming.
 
 ```python
 popcorn = (
     Chat("Respond with the certainty and creativity of a professional writer.")
     ("Explain 3 rules to writing a clever poem that amazes your friends.") 
     ("Using those tips, write a scrumptious poem about popcorn.")
 )
```

### Comparing `chatsnack-0.1.1/PKG-INFO` & `chatsnack-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatsnack
-Version: 0.1.1
+Version: 0.1.2
 Summary: chatsnack is the easiest Python library for rapid development with OpenAI's ChatGPT API. It provides an intuitive interface for creating and managing chat-based prompts and responses, making it convenient to build complex, interactive conversations with AI.
 License: MIT
 Author: Mattie Casper
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -31,23 +31,24 @@
 ## Setup
 
 ### Got snack?
 
 Install the `chatsnack` package from PyPI:
 
 ```bash
+# requires Python 3.10+
 pip install chatsnack
 ```
 
 ### Got keys?
 
-Add your OpenAI API key to your .env file. If you don't have a .env file, the library will create a new one for you. You can use env.template.cataclysm as an example.
+Add your OpenAI API key to your .env file. If you don't have a .env file, the library will create a new one for you in the local directory.
 
 ### Learn More!
-Read more below, watch the [video](https://youtu.be/ZK8fUuQDgZ4) or check out the [Getting Started notebook](notebooks/).
+Read more below, watch the [intro video](https://www.youtube.com/watch?v=Yjwi54rHrhw) or check out the [Getting Started notebook](notebooks/).
 
 ## Usage
 
 ### Enjoy a Quick Snack
 
 Easiest way to get going with `chatsnack` is with built-in snack packs. Each pack is a singleton ready to mingleton.
 
@@ -154,15 +155,15 @@
   print(midnightsnack.ask())
   ```
   > *"POPSICLE."*
     
 
 #### Adjusting Cooking Temperatures
 
-By default, `gpt-3.5-turbo` is the default chat API with a default temperature of `0.5`. If you prefer, you can change OpenAI parameters for each chat, such as the engine and temperature:
+By default, `gpt-3.5-turbo` is the default chat API with a default temperature of `0.7`. If you prefer, you can change OpenAI parameters for each chat, such as the engine and temperature:
 
 ```python
 from chatsnack import Chat
 wisechat = Chat("Respond with professional writing based on the user query.")
 wisechat.user("Author an alliterative poem about good snacks to eat with coffee.")
 wisechat.engine = "gpt-4"
 wisechat.temperature = 0.8
@@ -213,15 +214,15 @@
 
 ##### Quick Assistants
 
 Also, `.asst()` is an alias shortcut for `.assistant()` if you want you code to align cleanly with other 4-letter `.user()` and `.chat()` calls.
 
 ##### Binge-chaining
 
-If you're feeling wild, you can actually call any chat (like a function) and it'll submit the chat and continue, just like `.chat()`. This allows even more terse chaining. This can come in handy when you're looking for 
+If you're feeling wild, you can actually call any chat (like a function) and it'll submit the chat and continue, just like `.chat()`. This allows even more terse chaining. This can come in handy when you're looking for chain-of-thought prompting or prewriting priming.
 
 ```python
 popcorn = (
     Chat("Respond with the certainty and creativity of a professional writer.")
     ("Explain 3 rules to writing a clever poem that amazes your friends.") 
     ("Using those tips, write a scrumptious poem about popcorn.")
 )
```

