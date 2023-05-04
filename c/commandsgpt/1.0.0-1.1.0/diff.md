# Comparing `tmp/commandsgpt-1.0.0.tar.gz` & `tmp/commandsgpt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandsgpt-1.0.0.tar", last modified: Mon May  1 21:11:35 2023, max compression
+gzip compressed data, was "commandsgpt-1.1.0.tar", last modified: Thu May  4 20:32:28 2023, max compression
```

## Comparing `commandsgpt-1.0.0.tar` & `commandsgpt-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 21:11:35.200758 commandsgpt-1.0.0/
--rw-rw-rw-   0        0        0     1114 2023-05-01 15:56:47.000000 commandsgpt-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    11722 2023-05-01 21:11:35.201769 commandsgpt-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     9754 2023-05-01 20:47:51.000000 commandsgpt-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 21:11:35.123292 commandsgpt-1.0.0/commands_gpt/
-drwxrwxrwx   0        0        0        0 2023-05-01 21:11:35.159213 commandsgpt-1.0.0/commands_gpt/commands_gpt/
--rw-rw-rw-   0        0        0        0 2023-05-01 20:57:36.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/__init__.py
--rw-rw-rw-   0        0        0      393 2023-05-01 02:22:04.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/chat.py
-drwxrwxrwx   0        0        0        0 2023-05-01 21:11:35.170630 commandsgpt-1.0.0/commands_gpt/commands_gpt/commands/
--rw-rw-rw-   0        0        0        0 2023-05-01 02:22:04.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/commands/__init__.py
--rw-rw-rw-   0        0        0     3496 2023-05-01 15:38:02.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/commands/commands_funcs.py
--rw-rw-rw-   0        0        0     4483 2023-05-01 15:34:34.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/commands/graphs.py
--rw-rw-rw-   0        0        0      415 2023-05-01 15:21:36.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/config.py
--rw-rw-rw-   0        0        0     5601 2023-05-01 16:26:24.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/instruction_recognition.py
--rw-rw-rw-   0        0        0      141 2023-05-01 02:22:04.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/models.py
--rw-rw-rw-   0        0        0     3619 2023-05-01 03:00:10.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/regex.py
--rw-rw-rw-   0        0        0       70 2023-05-01 02:22:04.000000 commandsgpt-1.0.0/commands_gpt/commands_gpt/static.py
-drwxrwxrwx   0        0        0        0 2023-05-01 21:11:35.198759 commandsgpt-1.0.0/commands_gpt/commandsgpt.egg-info/
--rw-rw-rw-   0        0        0    11722 2023-05-01 21:11:35.000000 commandsgpt-1.0.0/commands_gpt/commandsgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2023-05-01 21:11:35.000000 commandsgpt-1.0.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 21:11:35.000000 commandsgpt-1.0.0/commands_gpt/commandsgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 21:11:35.000000 commandsgpt-1.0.0/commands_gpt/commandsgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-01 19:42:32.000000 commandsgpt-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1007 2023-05-01 21:11:35.213225 commandsgpt-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/commands_gpt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/commands_gpt/commands_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/commands_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/instruction_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-04 20:32:28.000000 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-04 20:32:28.000000 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:32:28.000000 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 20:32:28.000000 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/setup.cfg
```

### Comparing `commandsgpt-1.0.0/LICENSE` & `commandsgpt-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [2023] [Martín Alexis Martínez Andrade]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) [2023] [Martín Alexis Martínez Andrade]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `commandsgpt-1.0.0/PKG-INFO` & `commandsgpt-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,311 +1,311 @@
-Metadata-Version: 2.1
-Name: commandsgpt
-Version: 1.0.0
-Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
-Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
-Author: Martín Alexis Martínez Andrade
-Author-email: alexis.martinez.contacto@gmail.com
-Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
-Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CommandsGPT
-
-An implementation of GPT-4 to recognize instructions. It recognizes which commands it must run to fulfill the user's instruction, using a graph where each node is a command and the data generated by each command can be passed to other commands.
-
-Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
-
-# Installation
-
-Install the packages inside of the requirements.txt file.
-
-```
-pip install commandsgpt
-```
-
-If you're using a virtual environment:
-```
-pipenv install commandsgpt
-```
-
-# Basic usage
-
-Create a `commands` dictionary that will store the commands described in natural language. Create the functions that will be called when the commands are executed (they must match the arguments and return values of the `commands` dict; the first parameter of these functions must be a Config object). Create a `command_name_to_func` dictionary that will take the name of a command and return the corresponding function.
-
-*Example of commands dictionary*
-```
-commands = {
-    "REQUEST_USER_INPUT": {
-        "description": "Asks the user to input data through the interface.",
-        "arguments": {
-            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
-        },
-        "generates_data": {
-            "input": {"description": "Data entered by the user", "type": "string"},
-        },
-    },
-    ...
-}
-```
-
-*Example of a command function*
-```
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
-    input_ = input(f"{message}\n*: ")
-    results = {
-        "input": input_,
-    }
-    return results
-```
-
-*Example of command_name_to_func dictionary*
-```
-command_name_to_func = {
-    "REQUEST_USER_INPUT": request_user_input_command,
-    ...
-}
-```
-
-Add the ***essential commands*** to your commands dictionaries.
-* These are the default commands that implement core logic to the model's thinking, like an IF command.
-* If you already defined your own core logic commands (IF command, THINK command, etc.), then you are free not to use them.
-
-```
-from commands_gpt.commands.commands_funcs import add_essential_commands
-add_essential_commands(commands, command_name_to_func)
-```
-
-Your `config` object: 
-```
-config = Config("gpt-4-0314", commands, command_name_to_func)
-```
-
-Create an instruction:
-
-```
-instruction = input("Enter your instruction: ")
-```
-
-Pass your instruction to the recognizer model:
-
-```
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
-)
-```
-
-Finally, execute the graph of commands:
-
-```
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
-```
-
-# Basic example
-
-```
-from typing import Any
-from pathlib import Path
-from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
-from commands_gpt.commands.graphs import execute_commands
-from commands_gpt.config import Config
-
-# Commands Natural Language Dict
-
-commands = {
-    "WRITE_TO_USER": {
-        "description": "Writes something to the interface to communicate with the user.",
-        "arguments": {
-            "content": {"description": "Content to write.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-    "REQUEST_USER_INPUT": {
-        "description": "Asks the user to input data through the interface.",
-        "arguments": {
-            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
-        },
-        "generates_data": {
-            "input": {"description": "Data entered by the user", "type": "string"},
-        },
-    },
-    "WRITE_FILE": {
-        "description": "Write a file.",
-        "arguments": {
-            "content": {"description": "Content that will be written.", "type": "string"},
-            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-}
-
-# Commands functions
-
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
-    # add newlines because regex data injection replaces newline characters
-    # by \\n substrings.
-    content_with_newlines = "\n".join(content.split("\\n"))
-    print(f">>> {content_with_newlines}")
-    return {}
-
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
-    input_ = input(f"{message}\n*: ")
-    results = {
-        "input": input_,
-    }
-    return results
-
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
-    file_dir = Path(file_path).parent
-    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
-    with open(file_path, "w+", encoding="utf-8") as f:
-        f.write(content)
-        f.close()
-    return {}
-
-# Command name to function dict
-command_name_to_func = {
-    "WRITE_TO_USER": write_to_user_command,
-    "REQUEST_USER_INPUT": request_user_input_command,
-    "WRITE_FILE": write_file_command,
-}
-
-from commands_gpt.commands.commands_funcs import add_essential_commands
-add_essential_commands(commands, command_name_to_func)
-
-chat_model = "gpt-4-0314"
-
-config = Config(chat_model, commands, command_name_to_func)
-
-instruction = input("Enter your prompt: ")
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
-)
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
-```
-
-# Adding custom commands
-
-You can add and modify your own custom commands by creating two dictionaries:
-
-* commands: The commands that the model can use, described in natural language. The keys are the name of the commands, and the values are dictionaries.
-
-    * The nested dictionaries have keys *description*, *arguments* and *generates_data*.
-
-    * **description**: Description of the command in natural language.
-
-    * **arguments**: Arguments that the function of the command receives. It's a dictionary which keys are the names of the arguments, and the values are dictionaries that describe the arguments. 
-
-        * The nested dictionaries have keys *description* and *type*.
-        * **description**: Description of the argument in natural language.
-
-
-        * **type**: Data type. E.g.: "string", "boolean", "int".
-
-    * **generates_data**: The data generated by the command that other commands will be able to access. It's a dictionary which keys are the names of the data field, and the values are dictionaries that describe the data field.
-
-        * The nested dictionaries have keys *description* and *type*.
-
-        * **description**: Description of the data field in natural language.
-
-        * **type**: Data type. E.g.: "string", "boolean", "int".
-
-***Example***
-```
-commands = {
-    "WRITE_TO_USER": {
-        "description": "Writes something to the interface to communicate with the user.",
-        "arguments": {
-            "content": {"description": "Content to write.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-    "REQUEST_USER_INPUT": {
-        "description": "Asks the user to input data through the interface.",
-        "arguments": {
-            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
-        },
-        "generates_data": {
-            "input": {"description": "Data entered by the user", "type": "string"},
-        },
-    },
-    "WRITE_FILE": {
-        "description": "Write a file.",
-        "arguments": {
-            "content": {"description": "Content that will be written.", "type": "string"},
-            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-}
-```
-
-* command_name_to_func: The keys of this dictionary are the name of the commands, and the values are the function.
-
-    * The name of the function is irrelevant.
-
-    * The first argument must be the Config object.
-
-    * The arguments must match the arguments from the commands dictionary.
-
-    * The return value must be a dictionary which keys must match the "generates_data" key.
-
-    * The data types must match the ones declared in the commands dictionary.
-
-***Example***
-```
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
-    # add newlines because regex data injection replaces newline characters
-    # by \\n substrings.
-    content_with_newlines = "\n".join(content.split("\\n"))
-    print(f">>> {content_with_newlines}")
-    return {}
-
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
-    input_ = input(f"{message}\n*: ")
-    results = {
-        "input": input_,
-    }
-    return results
-
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
-    file_dir = Path(file_path).parent
-    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
-    with open(file_path, "w+", encoding="utf-8") as f:
-        f.write(content)
-        f.close()
-    return {}
-
-# add your functions here
-command_name_to_func = {
-    "WRITE_TO_USER": write_to_user_command,
-    "REQUEST_USER_INPUT": request_user_input_command,
-    "WRITE_FILE": write_file_command,
-}
-```
-
-MIT License
-
-Copyright (c) [2023] [Martín Alexis Martínez Andrade]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Metadata-Version: 2.1
+Name: commandsgpt
+Version: 1.1.0
+Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
+Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
+Author: Martín Alexis Martínez Andrade
+Author-email: alexis.martinez.contacto@gmail.com
+Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
+Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CommandsGPT
+
+An implementation of GPT-4 to recognize instructions. It recognizes which commands it must run to fulfill the user's instruction, using a graph where each node is a command and the data generated by each command can be passed to other commands.
+
+Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
+
+# Installation
+
+Install the `commandsgpt` module.
+
+```
+pip install commandsgpt
+```
+
+If you're using a virtual environment:
+```
+pipenv install commandsgpt
+```
+
+# Basic usage
+
+Create a `commands` dictionary that will store the commands described in natural language. Create the functions that will be called when the commands are executed (they must match the arguments and return values of the `commands` dict; the first parameter of these functions must be a Config object). Create a `command_name_to_func` dictionary that will take the name of a command and return the corresponding function.
+
+*Example of commands dictionary*
+```
+commands = {
+    "REQUEST_USER_INPUT": {
+        "description": "Asks the user to input data through the interface.",
+        "arguments": {
+            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
+        },
+        "generates_data": {
+            "input": {"description": "Data entered by the user", "type": "string"},
+        },
+    },
+    ...
+}
+```
+
+*Example of a command function*
+```
+def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+    input_ = input(f"{message}\n*: ")
+    results = {
+        "input": input_,
+    }
+    return results
+```
+
+*Example of command_name_to_func dictionary*
+```
+command_name_to_func = {
+    "REQUEST_USER_INPUT": request_user_input_command,
+    ...
+}
+```
+
+Add the ***essential commands*** to your commands dictionaries.
+* These are the default commands that implement core logic to the model's thinking, like an IF command.
+* If you already defined your own core logic commands (IF command, THINK command, etc.), then you are free not to use them.
+
+```
+from commands_gpt.commands.commands_funcs import add_essential_commands
+add_essential_commands(commands, command_name_to_func)
+```
+
+Your `config` object: 
+```
+config = Config("gpt-4-0314", commands, command_name_to_func)
+```
+
+Create an instruction:
+
+```
+instruction = input("Enter your instruction: ")
+```
+
+Pass your instruction to the recognizer model:
+
+```
+graph, graph_data = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, config.commands, config.command_name_to_func,
+)
+```
+
+Finally, execute the graph of commands:
+
+```
+execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+```
+
+# Basic example
+
+```
+from typing import Any
+from pathlib import Path
+from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
+from commands_gpt.commands.graphs import execute_commands
+from commands_gpt.config import Config
+
+# Commands Natural Language Dict
+
+commands = {
+    "WRITE_TO_USER": {
+        "description": "Writes something to the interface to communicate with the user.",
+        "arguments": {
+            "content": {"description": "Content to write.", "type": "string"},
+        },
+        "generates_data": {},
+    },
+    "REQUEST_USER_INPUT": {
+        "description": "Asks the user to input data through the interface.",
+        "arguments": {
+            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
+        },
+        "generates_data": {
+            "input": {"description": "Data entered by the user", "type": "string"},
+        },
+    },
+    "WRITE_FILE": {
+        "description": "Write a file.",
+        "arguments": {
+            "content": {"description": "Content that will be written.", "type": "string"},
+            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
+        },
+        "generates_data": {},
+    },
+}
+
+# Commands functions
+
+def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+    # add newlines because regex data injection replaces newline characters
+    # by \\n substrings.
+    content_with_newlines = "\n".join(content.split("\\n"))
+    print(f">>> {content_with_newlines}")
+    return {}
+
+def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+    input_ = input(f"{message}\n*: ")
+    results = {
+        "input": input_,
+    }
+    return results
+
+def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+    file_dir = Path(file_path).parent
+    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
+    with open(file_path, "w+", encoding="utf-8") as f:
+        f.write(content)
+        f.close()
+    return {}
+
+# Command name to function dict
+command_name_to_func = {
+    "WRITE_TO_USER": write_to_user_command,
+    "REQUEST_USER_INPUT": request_user_input_command,
+    "WRITE_FILE": write_file_command,
+}
+
+from commands_gpt.commands.commands_funcs import add_essential_commands
+add_essential_commands(commands, command_name_to_func)
+
+chat_model = "gpt-4-0314"
+
+config = Config(chat_model, commands, command_name_to_func)
+
+instruction = input("Enter your prompt: ")
+graph, graph_data = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, config.commands, config.command_name_to_func,
+)
+execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+```
+
+# Adding custom commands
+
+You can add and modify your own custom commands by creating two dictionaries:
+
+* commands: The commands that the model can use, described in natural language. The keys are the name of the commands, and the values are dictionaries.
+
+    * The nested dictionaries have keys *description*, *arguments* and *generates_data*.
+
+    * **description**: Description of the command in natural language.
+
+    * **arguments**: Arguments that the function of the command receives. It's a dictionary which keys are the names of the arguments, and the values are dictionaries that describe the arguments. 
+
+        * The nested dictionaries have keys *description* and *type*.
+        * **description**: Description of the argument in natural language.
+
+
+        * **type**: Data type. E.g.: "string", "boolean", "int".
+
+    * **generates_data**: The data generated by the command that other commands will be able to access. It's a dictionary which keys are the names of the data field, and the values are dictionaries that describe the data field.
+
+        * The nested dictionaries have keys *description* and *type*.
+
+        * **description**: Description of the data field in natural language.
+
+        * **type**: Data type. E.g.: "string", "boolean", "int".
+
+***Example***
+```
+commands = {
+    "WRITE_TO_USER": {
+        "description": "Writes something to the interface to communicate with the user.",
+        "arguments": {
+            "content": {"description": "Content to write.", "type": "string"},
+        },
+        "generates_data": {},
+    },
+    "REQUEST_USER_INPUT": {
+        "description": "Asks the user to input data through the interface.",
+        "arguments": {
+            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
+        },
+        "generates_data": {
+            "input": {"description": "Data entered by the user", "type": "string"},
+        },
+    },
+    "WRITE_FILE": {
+        "description": "Write a file.",
+        "arguments": {
+            "content": {"description": "Content that will be written.", "type": "string"},
+            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
+        },
+        "generates_data": {},
+    },
+}
+```
+
+* command_name_to_func: The keys of this dictionary are the name of the commands, and the values are the function.
+
+    * The name of the function is irrelevant.
+
+    * The first argument must be the Config object.
+
+    * The arguments must match the arguments from the commands dictionary.
+
+    * The return value must be a dictionary which keys must match the "generates_data" key.
+
+    * The data types must match the ones declared in the commands dictionary.
+
+***Example***
+```
+def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+    # add newlines because regex data injection replaces newline characters
+    # by \\n substrings.
+    content_with_newlines = "\n".join(content.split("\\n"))
+    print(f">>> {content_with_newlines}")
+    return {}
+
+def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+    input_ = input(f"{message}\n*: ")
+    results = {
+        "input": input_,
+    }
+    return results
+
+def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+    file_dir = Path(file_path).parent
+    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
+    with open(file_path, "w+", encoding="utf-8") as f:
+        f.write(content)
+        f.close()
+    return {}
+
+# add your functions here
+command_name_to_func = {
+    "WRITE_TO_USER": write_to_user_command,
+    "REQUEST_USER_INPUT": request_user_input_command,
+    "WRITE_FILE": write_file_command,
+}
+```
+
+MIT License
+
+Copyright (c) [2023] [Martín Alexis Martínez Andrade]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `commandsgpt-1.0.0/README.md` & `commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,273 +1,311 @@
-# CommandsGPT
-
-An implementation of GPT-4 to recognize instructions. It recognizes which commands it must run to fulfill the user's instruction, using a graph where each node is a command and the data generated by each command can be passed to other commands.
-
-Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
-
-# Installation
-
-Install the packages inside of the requirements.txt file.
-
-```
-pip install commandsgpt
-```
-
-If you're using a virtual environment:
-```
-pipenv install commandsgpt
-```
-
-# Basic usage
-
-Create a `commands` dictionary that will store the commands described in natural language. Create the functions that will be called when the commands are executed (they must match the arguments and return values of the `commands` dict; the first parameter of these functions must be a Config object). Create a `command_name_to_func` dictionary that will take the name of a command and return the corresponding function.
-
-*Example of commands dictionary*
-```
-commands = {
-    "REQUEST_USER_INPUT": {
-        "description": "Asks the user to input data through the interface.",
-        "arguments": {
-            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
-        },
-        "generates_data": {
-            "input": {"description": "Data entered by the user", "type": "string"},
-        },
-    },
-    ...
-}
-```
-
-*Example of a command function*
-```
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
-    input_ = input(f"{message}\n*: ")
-    results = {
-        "input": input_,
-    }
-    return results
-```
-
-*Example of command_name_to_func dictionary*
-```
-command_name_to_func = {
-    "REQUEST_USER_INPUT": request_user_input_command,
-    ...
-}
-```
-
-Add the ***essential commands*** to your commands dictionaries.
-* These are the default commands that implement core logic to the model's thinking, like an IF command.
-* If you already defined your own core logic commands (IF command, THINK command, etc.), then you are free not to use them.
-
-```
-from commands_gpt.commands.commands_funcs import add_essential_commands
-add_essential_commands(commands, command_name_to_func)
-```
-
-Your `config` object: 
-```
-config = Config("gpt-4-0314", commands, command_name_to_func)
-```
-
-Create an instruction:
-
-```
-instruction = input("Enter your instruction: ")
-```
-
-Pass your instruction to the recognizer model:
-
-```
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
-)
-```
-
-Finally, execute the graph of commands:
-
-```
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
-```
-
-# Basic example
-
-```
-from typing import Any
-from pathlib import Path
-from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
-from commands_gpt.commands.graphs import execute_commands
-from commands_gpt.config import Config
-
-# Commands Natural Language Dict
-
-commands = {
-    "WRITE_TO_USER": {
-        "description": "Writes something to the interface to communicate with the user.",
-        "arguments": {
-            "content": {"description": "Content to write.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-    "REQUEST_USER_INPUT": {
-        "description": "Asks the user to input data through the interface.",
-        "arguments": {
-            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
-        },
-        "generates_data": {
-            "input": {"description": "Data entered by the user", "type": "string"},
-        },
-    },
-    "WRITE_FILE": {
-        "description": "Write a file.",
-        "arguments": {
-            "content": {"description": "Content that will be written.", "type": "string"},
-            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-}
-
-# Commands functions
-
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
-    # add newlines because regex data injection replaces newline characters
-    # by \\n substrings.
-    content_with_newlines = "\n".join(content.split("\\n"))
-    print(f">>> {content_with_newlines}")
-    return {}
-
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
-    input_ = input(f"{message}\n*: ")
-    results = {
-        "input": input_,
-    }
-    return results
-
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
-    file_dir = Path(file_path).parent
-    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
-    with open(file_path, "w+", encoding="utf-8") as f:
-        f.write(content)
-        f.close()
-    return {}
-
-# Command name to function dict
-command_name_to_func = {
-    "WRITE_TO_USER": write_to_user_command,
-    "REQUEST_USER_INPUT": request_user_input_command,
-    "WRITE_FILE": write_file_command,
-}
-
-from commands_gpt.commands.commands_funcs import add_essential_commands
-add_essential_commands(commands, command_name_to_func)
-
-chat_model = "gpt-4-0314"
-
-config = Config(chat_model, commands, command_name_to_func)
-
-instruction = input("Enter your prompt: ")
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
-)
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
-```
-
-# Adding custom commands
-
-You can add and modify your own custom commands by creating two dictionaries:
-
-* commands: The commands that the model can use, described in natural language. The keys are the name of the commands, and the values are dictionaries.
-
-    * The nested dictionaries have keys *description*, *arguments* and *generates_data*.
-
-    * **description**: Description of the command in natural language.
-
-    * **arguments**: Arguments that the function of the command receives. It's a dictionary which keys are the names of the arguments, and the values are dictionaries that describe the arguments. 
-
-        * The nested dictionaries have keys *description* and *type*.
-        * **description**: Description of the argument in natural language.
-
-
-        * **type**: Data type. E.g.: "string", "boolean", "int".
-
-    * **generates_data**: The data generated by the command that other commands will be able to access. It's a dictionary which keys are the names of the data field, and the values are dictionaries that describe the data field.
-
-        * The nested dictionaries have keys *description* and *type*.
-
-        * **description**: Description of the data field in natural language.
-
-        * **type**: Data type. E.g.: "string", "boolean", "int".
-
-***Example***
-```
-commands = {
-    "WRITE_TO_USER": {
-        "description": "Writes something to the interface to communicate with the user.",
-        "arguments": {
-            "content": {"description": "Content to write.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-    "REQUEST_USER_INPUT": {
-        "description": "Asks the user to input data through the interface.",
-        "arguments": {
-            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
-        },
-        "generates_data": {
-            "input": {"description": "Data entered by the user", "type": "string"},
-        },
-    },
-    "WRITE_FILE": {
-        "description": "Write a file.",
-        "arguments": {
-            "content": {"description": "Content that will be written.", "type": "string"},
-            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
-        },
-        "generates_data": {},
-    },
-}
-```
-
-* command_name_to_func: The keys of this dictionary are the name of the commands, and the values are the function.
-
-    * The name of the function is irrelevant.
-
-    * The first argument must be the Config object.
-
-    * The arguments must match the arguments from the commands dictionary.
-
-    * The return value must be a dictionary which keys must match the "generates_data" key.
-
-    * The data types must match the ones declared in the commands dictionary.
-
-***Example***
-```
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
-    # add newlines because regex data injection replaces newline characters
-    # by \\n substrings.
-    content_with_newlines = "\n".join(content.split("\\n"))
-    print(f">>> {content_with_newlines}")
-    return {}
-
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
-    input_ = input(f"{message}\n*: ")
-    results = {
-        "input": input_,
-    }
-    return results
-
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
-    file_dir = Path(file_path).parent
-    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
-    with open(file_path, "w+", encoding="utf-8") as f:
-        f.write(content)
-        f.close()
-    return {}
-
-# add your functions here
-command_name_to_func = {
-    "WRITE_TO_USER": write_to_user_command,
-    "REQUEST_USER_INPUT": request_user_input_command,
-    "WRITE_FILE": write_file_command,
-}
-```
+Metadata-Version: 2.1
+Name: commandsgpt
+Version: 1.1.0
+Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
+Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
+Author: Martín Alexis Martínez Andrade
+Author-email: alexis.martinez.contacto@gmail.com
+Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
+Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CommandsGPT
+
+An implementation of GPT-4 to recognize instructions. It recognizes which commands it must run to fulfill the user's instruction, using a graph where each node is a command and the data generated by each command can be passed to other commands.
+
+Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
+
+# Installation
+
+Install the `commandsgpt` module.
+
+```
+pip install commandsgpt
+```
+
+If you're using a virtual environment:
+```
+pipenv install commandsgpt
+```
+
+# Basic usage
+
+Create a `commands` dictionary that will store the commands described in natural language. Create the functions that will be called when the commands are executed (they must match the arguments and return values of the `commands` dict; the first parameter of these functions must be a Config object). Create a `command_name_to_func` dictionary that will take the name of a command and return the corresponding function.
+
+*Example of commands dictionary*
+```
+commands = {
+    "REQUEST_USER_INPUT": {
+        "description": "Asks the user to input data through the interface.",
+        "arguments": {
+            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
+        },
+        "generates_data": {
+            "input": {"description": "Data entered by the user", "type": "string"},
+        },
+    },
+    ...
+}
+```
+
+*Example of a command function*
+```
+def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+    input_ = input(f"{message}\n*: ")
+    results = {
+        "input": input_,
+    }
+    return results
+```
+
+*Example of command_name_to_func dictionary*
+```
+command_name_to_func = {
+    "REQUEST_USER_INPUT": request_user_input_command,
+    ...
+}
+```
+
+Add the ***essential commands*** to your commands dictionaries.
+* These are the default commands that implement core logic to the model's thinking, like an IF command.
+* If you already defined your own core logic commands (IF command, THINK command, etc.), then you are free not to use them.
+
+```
+from commands_gpt.commands.commands_funcs import add_essential_commands
+add_essential_commands(commands, command_name_to_func)
+```
+
+Your `config` object: 
+```
+config = Config("gpt-4-0314", commands, command_name_to_func)
+```
+
+Create an instruction:
+
+```
+instruction = input("Enter your instruction: ")
+```
+
+Pass your instruction to the recognizer model:
+
+```
+graph, graph_data = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, config.commands, config.command_name_to_func,
+)
+```
+
+Finally, execute the graph of commands:
+
+```
+execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+```
+
+# Basic example
+
+```
+from typing import Any
+from pathlib import Path
+from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
+from commands_gpt.commands.graphs import execute_commands
+from commands_gpt.config import Config
+
+# Commands Natural Language Dict
+
+commands = {
+    "WRITE_TO_USER": {
+        "description": "Writes something to the interface to communicate with the user.",
+        "arguments": {
+            "content": {"description": "Content to write.", "type": "string"},
+        },
+        "generates_data": {},
+    },
+    "REQUEST_USER_INPUT": {
+        "description": "Asks the user to input data through the interface.",
+        "arguments": {
+            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
+        },
+        "generates_data": {
+            "input": {"description": "Data entered by the user", "type": "string"},
+        },
+    },
+    "WRITE_FILE": {
+        "description": "Write a file.",
+        "arguments": {
+            "content": {"description": "Content that will be written.", "type": "string"},
+            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
+        },
+        "generates_data": {},
+    },
+}
+
+# Commands functions
+
+def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+    # add newlines because regex data injection replaces newline characters
+    # by \\n substrings.
+    content_with_newlines = "\n".join(content.split("\\n"))
+    print(f">>> {content_with_newlines}")
+    return {}
+
+def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+    input_ = input(f"{message}\n*: ")
+    results = {
+        "input": input_,
+    }
+    return results
+
+def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+    file_dir = Path(file_path).parent
+    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
+    with open(file_path, "w+", encoding="utf-8") as f:
+        f.write(content)
+        f.close()
+    return {}
+
+# Command name to function dict
+command_name_to_func = {
+    "WRITE_TO_USER": write_to_user_command,
+    "REQUEST_USER_INPUT": request_user_input_command,
+    "WRITE_FILE": write_file_command,
+}
+
+from commands_gpt.commands.commands_funcs import add_essential_commands
+add_essential_commands(commands, command_name_to_func)
+
+chat_model = "gpt-4-0314"
+
+config = Config(chat_model, commands, command_name_to_func)
+
+instruction = input("Enter your prompt: ")
+graph, graph_data = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, config.commands, config.command_name_to_func,
+)
+execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+```
+
+# Adding custom commands
+
+You can add and modify your own custom commands by creating two dictionaries:
+
+* commands: The commands that the model can use, described in natural language. The keys are the name of the commands, and the values are dictionaries.
+
+    * The nested dictionaries have keys *description*, *arguments* and *generates_data*.
+
+    * **description**: Description of the command in natural language.
+
+    * **arguments**: Arguments that the function of the command receives. It's a dictionary which keys are the names of the arguments, and the values are dictionaries that describe the arguments. 
+
+        * The nested dictionaries have keys *description* and *type*.
+        * **description**: Description of the argument in natural language.
+
+
+        * **type**: Data type. E.g.: "string", "boolean", "int".
+
+    * **generates_data**: The data generated by the command that other commands will be able to access. It's a dictionary which keys are the names of the data field, and the values are dictionaries that describe the data field.
+
+        * The nested dictionaries have keys *description* and *type*.
+
+        * **description**: Description of the data field in natural language.
+
+        * **type**: Data type. E.g.: "string", "boolean", "int".
+
+***Example***
+```
+commands = {
+    "WRITE_TO_USER": {
+        "description": "Writes something to the interface to communicate with the user.",
+        "arguments": {
+            "content": {"description": "Content to write.", "type": "string"},
+        },
+        "generates_data": {},
+    },
+    "REQUEST_USER_INPUT": {
+        "description": "Asks the user to input data through the interface.",
+        "arguments": {
+            "message": {"description": "Message displayed to the user related to the data that will be requested (example: 'Enter your age').", "type": "string"},
+        },
+        "generates_data": {
+            "input": {"description": "Data entered by the user", "type": "string"},
+        },
+    },
+    "WRITE_FILE": {
+        "description": "Write a file.",
+        "arguments": {
+            "content": {"description": "Content that will be written.", "type": "string"},
+            "file_path": {"description": "Complete path of the file that will be written.", "type": "string"},
+        },
+        "generates_data": {},
+    },
+}
+```
+
+* command_name_to_func: The keys of this dictionary are the name of the commands, and the values are the function.
+
+    * The name of the function is irrelevant.
+
+    * The first argument must be the Config object.
+
+    * The arguments must match the arguments from the commands dictionary.
+
+    * The return value must be a dictionary which keys must match the "generates_data" key.
+
+    * The data types must match the ones declared in the commands dictionary.
+
+***Example***
+```
+def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+    # add newlines because regex data injection replaces newline characters
+    # by \\n substrings.
+    content_with_newlines = "\n".join(content.split("\\n"))
+    print(f">>> {content_with_newlines}")
+    return {}
+
+def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+    input_ = input(f"{message}\n*: ")
+    results = {
+        "input": input_,
+    }
+    return results
+
+def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+    file_dir = Path(file_path).parent
+    assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
+    with open(file_path, "w+", encoding="utf-8") as f:
+        f.write(content)
+        f.close()
+    return {}
+
+# add your functions here
+command_name_to_func = {
+    "WRITE_TO_USER": write_to_user_command,
+    "REQUEST_USER_INPUT": request_user_input_command,
+    "WRITE_FILE": write_file_command,
+}
+```
+
+MIT License
+
+Copyright (c) [2023] [Martín Alexis Martínez Andrade]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `commandsgpt-1.0.0/commands_gpt/commands_gpt/commands/commands_funcs.py` & `commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/commands_funcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Callable
 
 from ..chat import get_answer_from_model
 from ..config import Config
+from .graphs import Graph, generate_graph_data
 
 ESSENTIAL_COMMANDS = {
     "THINK": {
         "description": "Generates a thought in your 'mind' without writing it down yet. This command allows you to create new ideas, reflect, and analyze information. For example, when asked to 'Write a three-paragraph article about Lenz's Law,' you would first use this command to generate the article and then use another to write it.",
         "arguments": {
             "about": {"description": "What to think about. Example: 'Three-paragraph article about Lenz's Law.'", "type": "string"},
         },
@@ -22,34 +23,34 @@
             "result": {"description": "Result of the condition: 0 or 1.", "type": "boolean"},
         },
     }
 }
 
 # Commands functions
 # Must be named 'LowercaseCommandName_command'
-# The first argument must be the Config object
+# The first argument must be the Config object, followed by the Graph object
 # The arguments must match the arguments from the ESSENTIAL_COMMANDS dictionary
 # The return value must be a dictionary which keys must match the "generates_data" keys
 # The data types must match the ones declared in the ESSENTIAL_COMMANDS dictionary
 
-def think_command(config: Config, about: str) -> dict[str, Any]:
+def think_command(config: Config, graph: Graph, about: str) -> dict[str, Any]:
     messages = [
         {
             "role": "system", 
             "content": "You are a model used when executing a 'THINK' command, which function is to reflect, think, write, or ideate."
         },
     ]
     thought = get_answer_from_model(about, config.chat_model, messages)
 
     results = {
         "thought": thought,
     }
     return results
 
-def if_command(config: Config, condition: str) -> dict[str, Any]:
+def if_command(config: Config, graph: Graph, condition: str) -> dict[str, Any]:
     messages = [
         {
             "role": "system", 
             "content": f"You are a model that evaluates conditions, both in natural language and symbolic language. Given a condition, you respond with the number «1» (true) or «0» (false). DO NOT write ANYTHING ELSE EVER.",
         },
     ]
     result = get_answer_from_model(condition, config.chat_model, messages)
```

### Comparing `commandsgpt-1.0.0/commands_gpt/commands_gpt/instruction_recognition.py` & `commandsgpt-1.1.0/commands_gpt/commands_gpt/instruction_recognition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 import openai
-import json
-from typing import Any, Callable
+from typing import Callable
 
-from .commands.graphs import CommandNode
 from .static import StaticVar
-from . import regex
-from .commands import graphs
+from .commands.graphs import Graph
 
-def recognize_instruction(instruction: str, model: str, commands: dict) -> dict[str, Any]:
+
+def recognize_instruction(instruction: str, model: str, commands: dict) -> str:
     """
     Analyzes an instruction and creates data to create a graph of commands
     that will fulfill the instruction.
 
     Args:
         instruction (str): The user's instruction.
         model (str): Name of the model.
         commands (dict): The commands that the model can use, described in
             natural language.
 
     Returns:
-        tuple: A dict containing keys:
-        
-            'commands_data': data of the commands (to create a graph).
-
-            'data_references': data references (data that will be injected).
-            
-            'raw_commands_data': string commands data (the answer from the instruction recognition model).
+        a string: commands data (the answer from the instruction recognition model).
     """
     messages = [
         {
         'role': 'system', 
         'content':
             """You are a tool that, based on the user's prompt, detects the series of commands that must be executed, arguments that each command will have, and the relationship between each command (for example, what data generated by a command will be used as an argument for another)."""
             """\n*IMPORTANT*: *WRITE in the LANGUAGE that the USER writes his/her prompt in*."""
@@ -66,19 +58,15 @@
     print("Recognizing...")
     response = openai.ChatCompletion.create(
         model=model, messages=messages,
     )
 
     raw_commands_data = StaticVar(response["choices"][0]["message"]["content"])
 
-    data_references = regex.find_data_references_indices(raw_commands_data.val)
-    commands_data = regex.nullify_all_data_references(raw_commands_data.val)
-    commands_data = json.loads(commands_data)
-
-    return {"commands_data": commands_data, "data_references": data_references,
-        "raw_commands_data": raw_commands_data}
+    return raw_commands_data
 
 def recognize_instruction_and_create_graph(prompt: str, model: str, 
         commands: dict[str, dict], command_name_to_func: dict[str, Callable]) -> \
-        tuple[dict[str, CommandNode], dict[str, Any]]:
-    graph_data = recognize_instruction(prompt, model, commands)
-    return graphs.build_dependency_graph(graph_data["commands_data"], commands, command_name_to_func), graph_data
+        Graph:
+    raw_commands_data = recognize_instruction(prompt, model, commands)
+    graph = Graph(raw_commands_data, commands, command_name_to_func)
+    return graph
```

### Comparing `commandsgpt-1.0.0/commands_gpt/commands_gpt/regex.py` & `commandsgpt-1.1.0/commands_gpt/commands_gpt/regex.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.0.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt` & `commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

