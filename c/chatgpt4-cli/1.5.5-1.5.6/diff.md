# Comparing `tmp/chatgpt4-cli-1.5.5.tar.gz` & `tmp/chatgpt4-cli-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.5.5.tar", last modified: Wed Apr 26 10:55:23 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.5.6.tar", last modified: Thu May  4 10:36:23 2023, max compression
```

## Comparing `chatgpt4-cli-1.5.5.tar` & `chatgpt4-cli-1.5.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/GPTCLI/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/emage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32143 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/gptcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/GPTCLI/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 10:55:23.000000 chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:55:23.498772 chatgpt4-cli-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 10:55:01.000000 chatgpt4-cli-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:36:23.391187 chatgpt4-cli-1.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:36:23.387186 chatgpt4-cli-1.5.6/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32396 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-04 10:36:23.391187 chatgpt4-cli-1.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14274 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:36:23.391187 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 10:36:23.000000 chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:36:23.391187 chatgpt4-cli-1.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-04 10:36:00.000000 chatgpt4-cli-1.5.6/setup.py
```

### Comparing `chatgpt4-cli-1.5.5/GPTCLI/__init__.py` & `chatgpt4-cli-1.5.6/GPTCLI/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.5.5"
+__version__ = "1.5.6"
 __author__ = "Smartwa Caleb"
 __repo__ = "https://github.com/Simatwa/gpt-cli"
 __info__ = "Interact with ChatGPT and Bard at the terminal."
 
 import logging
 
 logging.basicConfig(
```

### Comparing `chatgpt4-cli-1.5.5/GPTCLI/addons.py` & `chatgpt4-cli-1.5.6/GPTCLI/addons.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from time import sleep
 from . import logging, getExc, __repo__, __author__, error_handler
 from threading import Thread as thr
 from sys import exit
 from fpdf import FPDF
 from json import loads
 import requests
+from datetime import datetime
 
 
 class file_parser:
     """Handles contents from text file"""
 
     def __init__(self, prompt):
         self.prompt = prompt
@@ -185,15 +186,15 @@
             return loads(resp.text)
         raise Exception("Prompts NOT found in path.")
 
     @error_handler()
     def main(self) -> None:
         if not self.contents:
             return
-        x = 1
+        x = 0
         self.pdf.set_text_color(255, 0, 0)
         self.pdf.set_font("Helvetica", size=18)
         self.pdf.cell(
             0,
             10,
             "Prompts for ChatGPT and Bard",
             align="C",
@@ -222,14 +223,19 @@
         self.pdf.add_link()
         self.pdf.cell(0, 10, msg, link=__repo__)
 
         self.pdf.ln()
         self.pdf.set_text_color(0, 0, 0)
         self.pdf.set_x((210 - self.pdf.get_string_width(__repo__)) / 2)
         self.pdf.cell(0, 10, __repo__)
+        self.pdf.ln()
+        self.pdf.set_font('Symbol',size=8)
+        time_stamp = f'Lastly auto-edited : {datetime.today().strftime("%d-%b-%Y %H:%M:%S %s")}'
+        self.pdf.set_x((210 - self.pdf.get_string_width(time_stamp)) / 2)
+        self.pdf.cell(0,10,time_stamp)
         self.pdf.output("all-acts.pdf")
         logging.info("Contents saved to 'all-acts.pdf'")
 
 
 if __name__ == "__main__":
     st = file_parser("I want you to debug this python code {f.test.py}")
     print(st.parse)
```

### Comparing `chatgpt4-cli-1.5.5/GPTCLI/bard.py` & `chatgpt4-cli-1.5.6/GPTCLI/bard.py`

 * *Files 17% similar despite different names*

```diff
@@ -52,7 +52,12 @@
         if stream and not self.args.disable_stream:
             for value in resp:
                 yield value
                 sleep(self.args.stream_interval)
         else:
             for val in resp:
                 yield val
+
+    def reset(self):
+        self.active_link.conversation_id = ""
+        self.active_link.response_id = ""
+        self.active_link.choice_id = ""
```

### Comparing `chatgpt4-cli-1.5.5/GPTCLI/emage.py` & `chatgpt4-cli-1.5.6/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.5/GPTCLI/gptcli.py` & `chatgpt4-cli-1.5.6/GPTCLI/gptcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -850,18 +850,24 @@
     def do__rollback(self, line):
         if line.isdigit():
             chatbot.rollback(int(line))
         self.do__prompt(self.prompt_disp)
     
     @error_handler()
     def do__reset(self, line):
-        if gpt4:
-            chatbot.reset(system_prompt=args.system_prompt)
+        if any([args.bard,'--bard' in line]) and not '--gpt4' in line:
+            self.bard.reset()
+            chat_gpt = 'Bard'
         else:
-            chatbot.reset()
+            if gpt4:
+                chatbot.reset(system_prompt=args.system_prompt)
+            else:
+                chatbot.reset()
+            chat_gpt = 'Bard'
+        logging.info(f'Chat reset successfully - {chat_gpt}')
         self.do__prompt(self.prompt_disp)
 
     def do__help(self, line):
         from .helper import help
 
         rich_print(
             Panel(Markdown(help),title='Help Info')
```

### Comparing `chatgpt4-cli-1.5.5/GPTCLI/helper.py` & `chatgpt4-cli-1.5.6/GPTCLI/helper.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.5/GPTCLI/image.py` & `chatgpt4-cli-1.5.6/GPTCLI/image.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.5/LICENSE` & `chatgpt4-cli-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.5/PKG-INFO` & `chatgpt4-cli-1.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.5
+Version: 1.5.6
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.5&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.6&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -367,7 +367,9 @@
 ## Acknowledgements
 
 1. [remo7777](https://github.com/remo7777/T-Header)
 
 2. [acheong08](https://github.com/acheong08/ChatGPT)
 
 3. [f](https://github.com/f/awesome-chatgpt-prompts)
+
+> **Note** Consider supporting this project by purchasing [Prompts for ChatGPT and Bard](https://payhip.com/b/zxQM0) ebook.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.5 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.6 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -148,8 +148,10 @@
 fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any
 **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-
 cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue prompt from a file - [x]
 Busy bar - [ ] Add prompts to the [prompts.csv](https://github.com/Simatwa/gpt-
 cli/edit/main/assets/prompts.csv) > Review [CHANGELOG](https://github.com/
 Simatwa/gpt-cli/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
 (https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
-acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
+acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts) >
+**Note** Consider supporting this project by purchasing [Prompts for ChatGPT
+and Bard](https://payhip.com/b/zxQM0) ebook.
```

### Comparing `chatgpt4-cli-1.5.5/README.md` & `chatgpt4-cli-1.5.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.5&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.6&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -340,7 +340,9 @@
 ## Acknowledgements
 
 1. [remo7777](https://github.com/remo7777/T-Header)
 
 2. [acheong08](https://github.com/acheong08/ChatGPT)
 
 3. [f](https://github.com/f/awesome-chatgpt-prompts)
+
+> **Note** Consider supporting this project by purchasing [Prompts for ChatGPT and Bard](https://payhip.com/b/zxQM0) ebook.
```

#### html2text {}

```diff
@@ -134,8 +134,10 @@
 fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any
 **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-
 cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue prompt from a file - [x]
 Busy bar - [ ] Add prompts to the [prompts.csv](https://github.com/Simatwa/gpt-
 cli/edit/main/assets/prompts.csv) > Review [CHANGELOG](https://github.com/
 Simatwa/gpt-cli/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
 (https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
-acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
+acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts) >
+**Note** Consider supporting this project by purchasing [Prompts for ChatGPT
+and Bard](https://payhip.com/b/zxQM0) ebook.
```

### Comparing `chatgpt4-cli-1.5.5/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.5.6/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.5
+Version: 1.5.6
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.5&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.6&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
@@ -367,7 +367,9 @@
 ## Acknowledgements
 
 1. [remo7777](https://github.com/remo7777/T-Header)
 
 2. [acheong08](https://github.com/acheong08/ChatGPT)
 
 3. [f](https://github.com/f/awesome-chatgpt-prompts)
+
+> **Note** Consider supporting this project by purchasing [Prompts for ChatGPT and Bard](https://payhip.com/b/zxQM0) ebook.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.5 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.6 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -148,8 +148,10 @@
 fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any
 **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-
 cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue prompt from a file - [x]
 Busy bar - [ ] Add prompts to the [prompts.csv](https://github.com/Simatwa/gpt-
 cli/edit/main/assets/prompts.csv) > Review [CHANGELOG](https://github.com/
 Simatwa/gpt-cli/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
 (https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
-acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
+acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts) >
+**Note** Consider supporting this project by purchasing [Prompts for ChatGPT
+and Bard](https://payhip.com/b/zxQM0) ebook.
```

### Comparing `chatgpt4-cli-1.5.5/setup.py` & `chatgpt4-cli-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         "numpy>=1.23.4",
         "colorama>=0.4.6",
         "openai>=0.26.4",
         "revChatGPT==4.0.6",
         "appdirs>=1.4.4",
         "requests>=2.28.2",
         "tabulate>=0.9.0",
-        "GoogleBard==0.0.7",
+        "GoogleBard==1.0.0",
         "fpdf==1.7.2",
     ],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
```

