# Comparing `tmp/hugchat-0.0.5.2.tar.gz` & `tmp/hugchat-0.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.5.2.tar", last modified: Wed May  3 15:57:41 2023, max compression
+gzip compressed data, was "hugchat-0.0.5.3.tar", last modified: Thu May  4 13:54:51 2023, max compression
```

## Comparing `hugchat-0.0.5.2.tar` & `hugchat-0.0.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:57:41.375097 hugchat-0.0.5.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.2/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2826 2023-05-03 15:57:41.375097 hugchat-0.0.5.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1806 2023-05-03 15:54:22.000000 hugchat-0.0.5.2/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-03 15:57:41.375097 hugchat-0.0.5.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1407 2023-05-03 15:55:47.000000 hugchat-0.0.5.2/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:57:41.371097 hugchat-0.0.5.2/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:57:41.371097 hugchat-0.0.5.2/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.2/src/hugchat/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.2/src/hugchat/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6265 2023-05-03 15:54:22.000000 hugchat-0.0.5.2/src/hugchat/hugchat.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:57:41.371097 hugchat-0.0.5.2/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2826 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-03 15:57:41.000000 hugchat-0.0.5.2/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 13:54:51.791249 hugchat-0.0.5.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2836 2023-05-04 13:54:51.791249 hugchat-0.0.5.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1816 2023-05-04 13:53:20.000000 hugchat-0.0.5.3/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-04 13:54:51.791249 hugchat-0.0.5.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1407 2023-05-04 13:53:59.000000 hugchat-0.0.5.3/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 13:54:51.783249 hugchat-0.0.5.3/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 13:54:51.787249 hugchat-0.0.5.3/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.3/src/hugchat/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.3/src/hugchat/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6405 2023-05-04 13:53:20.000000 hugchat-0.0.5.3/src/hugchat/hugchat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 13:54:51.791249 hugchat-0.0.5.3/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2836 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.5.2/LICENSE` & `hugchat-0.0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.5.2/PKG-INFO` & `hugchat-0.0.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,25 +19,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hugging-chat-api
+
 HuggingChat Python API
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
 
-##  How to Use
+## How to Use
 
 ### Basic mode
+
 ```bash
 pip install hugchat
 ```
 
 ```py
 from hugchat import hugchat
 chatbot = hugchat.ChatBot()
@@ -66,21 +68,20 @@
 - `stream`: Optional[bool]. Default is True
 - `use_cache`: Optional[bool]. Default is False
 - `is_retry`: Optional[bool]. Default is False
 - `retry_count`: Optional[int]. Number of retries for requesting huggingchat. Default is 5
 
 ### CLI mode
 
-> `version 0.0.5.1` or newer
+> `version 0.0.5.2` or newer
 
-You can use `cli mode` to test the repo:
+Simply run the following command in your terminal to start the CLI mode
 
-```python
-from hugchat import hugchat
-hugchat.cli()
+```bash
+python -m hugchat.cli
 ```
 
 Commands in cli mode:
 
 - `/new` : Create and switch to a new conversation.
 - `/ids` : Shows a list of all ID numbers and ID strings in current session.
 - `/switch <id>` : Switches to the ID number passed.
```

### Comparing `hugchat-0.0.5.2/README.md` & `hugchat-0.0.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # hugging-chat-api
+
 HuggingChat Python API
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
 
-##  How to Use
+## How to Use
 
 ### Basic mode
+
 ```bash
 pip install hugchat
 ```
 
 ```py
 from hugchat import hugchat
 chatbot = hugchat.ChatBot()
@@ -42,21 +44,20 @@
 - `stream`: Optional[bool]. Default is True
 - `use_cache`: Optional[bool]. Default is False
 - `is_retry`: Optional[bool]. Default is False
 - `retry_count`: Optional[int]. Number of retries for requesting huggingchat. Default is 5
 
 ### CLI mode
 
-> `version 0.0.5.1` or newer
+> `version 0.0.5.2` or newer
 
-You can use `cli mode` to test the repo:
+Simply run the following command in your terminal to start the CLI mode
 
-```python
-from hugchat import hugchat
-hugchat.cli()
+```bash
+python -m hugchat.cli
 ```
 
 Commands in cli mode:
 
 - `/new` : Create and switch to a new conversation.
 - `/ids` : Shows a list of all ID numbers and ID strings in current session.
 - `/switch <id>` : Switches to the ID number passed.
```

### Comparing `hugchat-0.0.5.2/setup.py` & `hugchat-0.0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.5.2",
+    version="0.0.5.3",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.0.5.2/src/hugchat/hugchat.py` & `hugchat-0.0.5.3/src/hugchat/hugchat.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         return list(self.conversation_id_list)
     
     def new_conversation(self) -> str:
         err_count = 0
         resp = ""
         while True:
             try:
-                resp = self.session.post(hf_url + "/conversation")
+                resp = self.session.post(hf_url + "/conversation", json={"model": "OpenAssistant/oasst-sft-6-llama-30b-xor"}, headers={"Content-Type": "application/json"})
+                # print(resp.text)
                 cid = json.loads(resp.text)['conversationId']
                 self.conversation_id_list.append(cid)
                 return cid
             except BaseException as e:
                 err_count += 1
                 print(f"[Error] Failed to create new conversation. Retrying... ({err_count})")
                 if err_count > 5:
```

### Comparing `hugchat-0.0.5.2/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.5.3/src/hugchat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,25 +19,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hugging-chat-api
+
 HuggingChat Python API
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
 
-##  How to Use
+## How to Use
 
 ### Basic mode
+
 ```bash
 pip install hugchat
 ```
 
 ```py
 from hugchat import hugchat
 chatbot = hugchat.ChatBot()
@@ -66,21 +68,20 @@
 - `stream`: Optional[bool]. Default is True
 - `use_cache`: Optional[bool]. Default is False
 - `is_retry`: Optional[bool]. Default is False
 - `retry_count`: Optional[int]. Number of retries for requesting huggingchat. Default is 5
 
 ### CLI mode
 
-> `version 0.0.5.1` or newer
+> `version 0.0.5.2` or newer
 
-You can use `cli mode` to test the repo:
+Simply run the following command in your terminal to start the CLI mode
 
-```python
-from hugchat import hugchat
-hugchat.cli()
+```bash
+python -m hugchat.cli
 ```
 
 Commands in cli mode:
 
 - `/new` : Create and switch to a new conversation.
 - `/ids` : Shows a list of all ID numbers and ID strings in current session.
 - `/switch <id>` : Switches to the ID number passed.
```

