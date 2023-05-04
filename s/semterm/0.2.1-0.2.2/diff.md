# Comparing `tmp/semterm-0.2.1.tar.gz` & `tmp/semterm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semterm-0.2.1.tar", last modified: Wed May  3 03:11:23 2023, max compression
+gzip compressed data, was "semterm-0.2.2.tar", last modified: Thu May  4 05:58:50 2023, max compression
```

## Comparing `semterm-0.2.1.tar` & `semterm-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.883560 semterm-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-03 03:10:59.000000 semterm-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 03:10:59.000000 semterm-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 03:11:23.883560 semterm-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-03 03:10:59.000000 semterm-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 03:10:59.000000 semterm-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm/UI/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/UI/UserInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/UI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm/agent/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/MrklAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/TerminalAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/TerminalAgentExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/TerminalAgentPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/config/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.883560 semterm-0.2.1/semterm/langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/langchain_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/langchain_extensions/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/langchain_extensions/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.883560 semterm-0.2.1/semterm/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/SemanticTerminalManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/SemanticTerminalProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/TerminalOutputParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/TerminalTool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 03:11:23.883560 semterm-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-03 03:10:59.000000 semterm-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.199402 semterm-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-04 05:58:27.000000 semterm-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 05:58:27.000000 semterm-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-04 05:58:50.195402 semterm-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-04 05:58:27.000000 semterm-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-04 05:58:27.000000 semterm-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/UI/UserInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/UI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/MrklAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/TerminalAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/TerminalAgentExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/TerminalAgentPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/config/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/langchain_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/langchain_extensions/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/langchain_extensions/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/SemanticTerminalManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/SemanticTerminalProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/TerminalOutputParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/TerminalTool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:27.000000 semterm-0.2.2/semterm/terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:58:50.195402 semterm-0.2.2/semterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:58:50.000000 semterm-0.2.2/semterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:58:50.199402 semterm-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 05:58:27.000000 semterm-0.2.2/setup.py
```

### Comparing `semterm-0.2.1/LICENSE` & `semterm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `semterm-0.2.1/README.md` & `semterm-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SemTerm: The Semantic Terminal 🚀
+# SemTerm: The Semantic Terminal 🖥️🚀
 
 SemTerm is a groundbreaking command-line tool that harnesses the capabilities of Large Language Models to execute complex tasks using natural, conversational input.
 With SemTerm, you can run complex bash commands with a simple, intuitive instruction. 
 
 SemTerm offers a futuristic command-line experience currently available only for Linux and MacOS users.
 
 You can ask it things like
@@ -13,28 +13,21 @@
 semterm >  The size of the current directory is 146M.
 ```
 
 And pretty much anything else you can think of. You are only limited by your imagination. 💭
 
 Join our [Discord](https://discord.gg/TQSbWnck) to discuss SemTerm and help out with development!
 
-## Table of Contents 📚
-
-1. [Features](#features)
-2. [Requirements](#requirements)
-3. [Installation](#installation)
-4. [Usage](#usage)
-5. [Ideas for Future Development](#ideas-for-future-development)
-6. [Contribute](#contribute)
-7. [License](#license)
-
 ## Features 🌟
 
 * User-friendly semantic input
-* Harness the power of Large Language Models for complex shell commands
+* SemTerm has thoughts, observations and actions.
+* Can perform multiple shell commands at once
+* Can request more information from the user
+* sudo ability is currently being worked on and tested
 
 ## Requirements 🔧
 
 * Python 3.10
   * langchain
   * tiktoken
   * pexpect 
@@ -100,8 +93,8 @@
 
 By working together, we can refine SemTerm and create a more powerful, accurate, and efficient tool for everyone.
 
 Thank you for being a part of our journey, and we look forward to your valuable feedback and contributions!
 
 ## License ⚖️
 
-SemTerm is released under the [MIT License](LICENSE).
+SemTerm is released under the [MIT License](LICENSE).
```

### Comparing `semterm-0.2.1/semterm/agent/MrklAgent.py` & `semterm-0.2.2/semterm/agent/MrklAgent.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+import os
+
 from langchain.agents import load_tools
 from langchain.chat_models import ChatOpenAI
 from langchain.memory import ConversationEntityMemory
 
+from semterm.agent.TerminalAgentPrompt import PREFIX
 from semterm.config.Config import Config
 from semterm.agent.TerminalAgent import TerminalAgent
 from semterm.agent.TerminalAgentExecutor import TerminalAgentExecutor
+from semterm.terminal.TerminalOutputParser import TerminalOutputParser
 from semterm.terminal.TerminalTool import TerminalTool
 from semterm.terminal.SemanticTerminalManager import SemanticTerminalManager
 from semterm.langchain_extensions.tools import MistakeTool
 
 
 class MrklAgent:
     def __init__(self, config: Config):
@@ -42,15 +46,20 @@
             llm=self.llm,
             return_messages=True,
             chat_history_key="chat_history",
         )
 
     def initialize_agent(self):
         return TerminalAgent.from_llm_and_tools(
-            self.llm, self.tools, memory=self.memory, verbose=self.verbose
+            self.llm,
+            self.tools,
+            memory=self.memory,
+            system_message=PREFIX.format(current_directory=os.getcwd()),
+            output_parser=TerminalOutputParser(),
+            verbose=self.verbose,
         )
 
     def initialize_executor(self):
         return TerminalAgentExecutor.from_agent_and_tools(
             self.terminal_agent,
             self.tools,
             memory=self.memory,
```

### Comparing `semterm-0.2.1/semterm/agent/TerminalAgent.py` & `semterm-0.2.2/semterm/agent/TerminalAgent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 import os
 from abc import ABC
 from typing import Sequence, Optional, List, Tuple, Any
 from langchain import BasePromptTemplate
 from langchain.agents import (
     ConversationalChatAgent,
-    Agent,
     AgentOutputParser,
 )
-from langchain.callbacks import BaseCallbackManager
 from langchain.tools import BaseTool
 from pydantic import Field
 
 from .TerminalAgentPrompt import (
     PREFIX,
     SUFFIX,
     TEMPLATE_TOOL_RESPONSE,
 )
 from langchain.schema import (
     AgentAction,
     BaseOutputParser,
     BaseMessage,
     AIMessage,
-    HumanMessage,
-    BaseLanguageModel,
     SystemMessage,
 )
 from semterm.terminal.TerminalOutputParser import TerminalOutputParser
 
 
 class TerminalAgent(ConversationalChatAgent, ABC):
     output_parser: AgentOutputParser = Field(default_factory=TerminalOutputParser)
 
     @classmethod
-    def _get_default_output_parser(cls, **kwargs: Any) -> AgentOutputParser:
-        return TerminalOutputParser()
-
-    @classmethod
     def create_prompt(
         cls,
         tools: Sequence[BaseTool],
         system_message: str = PREFIX.format(current_directory=os.getcwd()),
         human_message: str = SUFFIX,
         input_variables: Optional[List[str]] = None,
         output_parser: Optional[BaseOutputParser] = None,
@@ -66,30 +58,7 @@
                 observation = observation.replace(action.tool_input, "")
             thoughts.append(AIMessage(content=action.log))
             system_message = SystemMessage(
                 content=TEMPLATE_TOOL_RESPONSE.format(observation=observation)
             )
             thoughts.append(system_message)
         return thoughts
-
-    @classmethod
-    def from_llm_and_tools(
-        cls,
-        llm: BaseLanguageModel,
-        tools: Sequence[BaseTool],
-        callback_manager: Optional[BaseCallbackManager] = None,
-        output_parser: Optional[AgentOutputParser] = None,
-        system_message: str = PREFIX.format(current_directory=os.getcwd()),
-        human_message: str = SUFFIX,
-        input_variables: Optional[List[str]] = None,
-        **kwargs: Any,
-    ) -> Agent:
-        return super().from_llm_and_tools(
-            llm=llm,
-            tools=tools,
-            callback_manager=callback_manager,
-            output_parser=output_parser or cls._get_default_output_parser(),
-            system_message=system_message,
-            human_message=human_message,
-            input_variables=input_variables,
-            **kwargs,
-        )
```

### Comparing `semterm-0.2.1/semterm/agent/TerminalAgentExecutor.py` & `semterm-0.2.2/semterm/agent/TerminalAgentExecutor.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.1/semterm/agent/TerminalAgentPrompt.py` & `semterm-0.2.2/semterm/agent/TerminalAgentPrompt.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.1/semterm/langchain_extensions/tools.py` & `semterm-0.2.2/semterm/langchain_extensions/tools.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.1/semterm/terminal/SemanticTerminalManager.py` & `semterm-0.2.2/semterm/terminal/SemanticTerminalManager.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.1/semterm/terminal/SemanticTerminalProcess.py` & `semterm-0.2.2/semterm/terminal/SemanticTerminalProcess.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.1/semterm/terminal/TerminalOutputParser.py` & `semterm-0.2.2/semterm/terminal/TerminalOutputParser.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.1/semterm/terminal/TerminalTool.py` & `semterm-0.2.2/semterm/terminal/TerminalTool.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.1/semterm.egg-info/SOURCES.txt` & `semterm-0.2.2/semterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semterm-0.2.1/setup.py` & `semterm-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="semterm",
-    version="0.2.1",
+    version="0.2.2",
     description="The Semantic Terminal",
     long_description="The Semantic Terminal",
     author="Lambrou",
     author_email="alexanderlambrou0602@gmail.com",
     packages=find_packages(),
     include_package_data=True,
     entry_points={
```

