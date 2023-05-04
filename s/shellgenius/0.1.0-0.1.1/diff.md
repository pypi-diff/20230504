# Comparing `tmp/shellgenius-0.1.0.tar.gz` & `tmp/shellgenius-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellgenius-0.1.0.tar", last modified: Thu May  4 17:09:07 2023, max compression
+gzip compressed data, was "shellgenius-0.1.1.tar", last modified: Thu May  4 18:16:00 2023, max compression
```

## Comparing `shellgenius-0.1.0.tar` & `shellgenius-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 17:09:07.795385 shellgenius-0.1.0/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.0/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3315 2023-05-04 17:09:07.795385 shellgenius-0.1.0/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3182 2023-05-04 17:05:13.000000 shellgenius-0.1.0/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-04 17:09:07.795385 shellgenius-0.1.0/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-04 17:05:33.000000 shellgenius-0.1.0/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 17:09:07.795385 shellgenius-0.1.0/shellgenius/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.0/shellgenius/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2996 2023-05-04 16:54:20.000000 shellgenius-0.1.0/shellgenius/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5534 2023-05-04 16:22:37.000000 shellgenius-0.1.0/shellgenius/gpt_integration.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 17:09:07.795385 shellgenius-0.1.0/shellgenius.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3315 2023-05-04 17:09:07.000000 shellgenius-0.1.0/shellgenius.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-05-04 17:09:07.000000 shellgenius-0.1.0/shellgenius.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-04 17:09:07.000000 shellgenius-0.1.0/shellgenius.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-04 17:09:07.000000 shellgenius-0.1.0/shellgenius.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      341 2023-05-04 17:09:07.000000 shellgenius-0.1.0/shellgenius.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-04 17:09:07.000000 shellgenius-0.1.0/shellgenius.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:16:00.954855 shellgenius-0.1.1/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.1/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3368 2023-05-04 18:16:00.954855 shellgenius-0.1.1/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3235 2023-05-04 18:15:13.000000 shellgenius-0.1.1/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-04 18:16:00.954855 shellgenius-0.1.1/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-04 18:15:52.000000 shellgenius-0.1.1/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:16:00.954855 shellgenius-0.1.1/shellgenius/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.1/shellgenius/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2981 2023-05-04 18:13:12.000000 shellgenius-0.1.1/shellgenius/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5522 2023-05-04 18:04:38.000000 shellgenius-0.1.1/shellgenius/gpt_integration.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 18:16:00.954855 shellgenius-0.1.1/shellgenius.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3368 2023-05-04 18:16:00.000000 shellgenius-0.1.1/shellgenius.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-05-04 18:16:00.000000 shellgenius-0.1.1/shellgenius.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-04 18:16:00.000000 shellgenius-0.1.1/shellgenius.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-04 18:16:00.000000 shellgenius-0.1.1/shellgenius.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      341 2023-05-04 18:16:00.000000 shellgenius-0.1.1/shellgenius.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-04 18:16:00.000000 shellgenius-0.1.1/shellgenius.egg-info/top_level.txt
```

### Comparing `shellgenius-0.1.0/LICENSE` & `shellgenius-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.0/PKG-INFO` & `shellgenius-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: shellgenius
-Version: 0.1.0
+Version: 0.1.1
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
 
 Powered by OpenAI's gpt-3.5-turbo AI model, ShellGenius generates accurate commands based on your input and provides step-by-step explanations to help you understand the underlying logic.
 
-![ShellGenius Demo](demo.gif)
+![ShellGenius Demo](assets/demo.gif)
 
 ## Table of Contents
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Examples](#examples)
 * [Limitations](#limitations)
@@ -122,7 +122,11 @@
 ## Limitations
 
 ShellGenius is powered by an AI model and may not always generate the most efficient or accurate commands. Exercise caution when executing commands, especially when working with sensitive data or critical systems.
 
 ## License
 
 ShellGenius is released under the [MIT License](LICENSE).
+
+___
+
+<https://github.com/sderev/shellgenius>
```

### Comparing `shellgenius-0.1.0/README.md` & `shellgenius-0.1.1/shellgenius.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+Metadata-Version: 2.1
+Name: shellgenius
+Version: 0.1.1
+Author: sderev
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
 
 Powered by OpenAI's gpt-3.5-turbo AI model, ShellGenius generates accurate commands based on your input and provides step-by-step explanations to help you understand the underlying logic.
 
-![ShellGenius Demo](demo.gif)
+![ShellGenius Demo](assets/demo.gif)
 
 ## Table of Contents
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Examples](#examples)
 * [Limitations](#limitations)
@@ -115,7 +122,11 @@
 ## Limitations
 
 ShellGenius is powered by an AI model and may not always generate the most efficient or accurate commands. Exercise caution when executing commands, especially when working with sensitive data or critical systems.
 
 ## License
 
 ShellGenius is released under the [MIT License](LICENSE).
+
+___
+
+<https://github.com/sderev/shellgenius>
```

### Comparing `shellgenius-0.1.0/setup.py` & `shellgenius-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="shellgenius",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "shellgenius = shellgenius.cli:shellgenius",
         ]
     },
```

### Comparing `shellgenius-0.1.0/shellgenius/cli.py` & `shellgenius-0.1.1/shellgenius/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     global live_markdown, live_markdown_text
     live_markdown_text += chunk
     live_markdown = Markdown(live_markdown_text)
     live.update(live_markdown)
 
 
 @click.command()
-@click.argument("command_description", required=True, type=str, nargs=-1)
+@click.argument("command_description", type=str, nargs=-1)
 def shellgenius(command_description):
     """
     Generate and optionally execute a shell command based on the given command description.
 
     Example:
         $ shellgenius create a new file called example.txt
         Generated command: touch example.txt
```

### Comparing `shellgenius-0.1.0/shellgenius/gpt_integration.py` & `shellgenius-0.1.1/shellgenius/gpt_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import json
 import openai
 import tiktoken
 import time
 
 
 def format_prompt(command_description):
     prompt = [
```

### Comparing `shellgenius-0.1.0/shellgenius.egg-info/PKG-INFO` & `shellgenius-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-Metadata-Version: 2.1
-Name: shellgenius
-Version: 0.1.0
-Author: sderev
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
 
 Powered by OpenAI's gpt-3.5-turbo AI model, ShellGenius generates accurate commands based on your input and provides step-by-step explanations to help you understand the underlying logic.
 
-![ShellGenius Demo](demo.gif)
+![ShellGenius Demo](assets/demo.gif)
 
 ## Table of Contents
 
 * [Installation](#installation)
 * [Usage](#usage)
 * [Examples](#examples)
 * [Limitations](#limitations)
@@ -122,7 +115,11 @@
 ## Limitations
 
 ShellGenius is powered by an AI model and may not always generate the most efficient or accurate commands. Exercise caution when executing commands, especially when working with sensitive data or critical systems.
 
 ## License
 
 ShellGenius is released under the [MIT License](LICENSE).
+
+___
+
+<https://github.com/sderev/shellgenius>
```

