# Comparing `tmp/findmyorder-1.1.6.tar.gz` & `tmp/findmyorder-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.1.6.tar", max compression
+gzip compressed data, was "findmyorder-1.2.4.tar", max compression
```

## Comparing `findmyorder-1.1.6.tar` & `findmyorder-1.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-03 19:44:59.875816 findmyorder-1.1.6/LICENSE
--rw-r--r--   0        0        0     2180 2023-05-03 19:44:59.875816 findmyorder-1.1.6/README.md
--rw-r--r--   0        0        0      113 2023-05-03 19:45:00.631827 findmyorder-1.1.6/findmyorder/__init__.py
--rw-r--r--   0        0        0      392 2023-05-03 19:44:59.875816 findmyorder-1.1.6/findmyorder/config.py
--rw-r--r--   0        0        0      566 2023-05-03 19:44:59.875816 findmyorder-1.1.6/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     4031 2023-05-03 19:44:59.875816 findmyorder-1.1.6/findmyorder/main.py
--rw-r--r--   0        0        0     1280 2023-05-03 19:45:00.631827 findmyorder-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 findmyorder-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-04 19:16:22.429576 findmyorder-1.2.4/LICENSE
+-rw-r--r--   0        0        0     2156 2023-05-04 19:16:22.429576 findmyorder-1.2.4/README.md
+-rw-r--r--   0        0        0      113 2023-05-04 19:16:23.117590 findmyorder-1.2.4/findmyorder/__init__.py
+-rw-r--r--   0        0        0      631 2023-05-04 19:16:22.429576 findmyorder-1.2.4/findmyorder/config.py
+-rw-r--r--   0        0        0      566 2023-05-04 19:16:22.429576 findmyorder-1.2.4/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     4031 2023-05-04 19:16:22.429576 findmyorder-1.2.4/findmyorder/main.py
+-rw-r--r--   0        0        0     1758 2023-05-04 19:16:23.117590 findmyorder-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2976 1970-01-01 00:00:00.000000 findmyorder-1.2.4/PKG-INFO
```

### Comparing `findmyorder-1.1.6/LICENSE` & `findmyorder-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.6/README.md` & `findmyorder-1.2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Find my order
 
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and parse order for trade execution. |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![🐍Build](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%90%8DBuild.yml/badge.svg?branch=main)](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%90%8DBuild.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
+|[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 
 
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
```

### Comparing `findmyorder-1.1.6/findmyorder/default_settings.toml` & `findmyorder-1.2.4/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.6/findmyorder/main.py` & `findmyorder-1.2.4/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.6/pyproject.toml` & `findmyorder-1.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.1.6"
+version = "1.2.4"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 
 
@@ -39,11 +39,23 @@
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","findmyorder/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
+commit_parser = "semantic_release.history.emoji_parser"
+use_textual_changelog_sections = true
+
+#patch_emoji
+# 🐛🚑🤖🏁🔒👽🔍💬🥅⚡♿🍏🐧
+#:ambulance:, :lock:, :bug:, :zap:, :goal_net:, :alien:, :wheelchair:, :speech_balloon:, :mag:, :apple:, :penguin:, :checkered_flag:, :robot:, :green_apple
+#minor_emoji
+#✨🥚🚸📱💄📈
+#:sparkles: ✨, :children_crossing:, :lipstick:, :iphone:, :egg:, :chart_with_upwards_trend
+#major_emoji¶
+#💥
+# :boom:
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `findmyorder-1.1.6/PKG-INFO` & `findmyorder-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.1.6
+Version: 1.2.4
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 
 # Find my order
 
 
 | <img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"> | A python package to identify and parse order for trade execution. |
 | ------------- | ------------- |
-|[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![🐍Build](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%90%8DBuild.yml/badge.svg?branch=main)](https://github.com/mraniki/findmyorder/actions/workflows/%F0%9F%90%8DBuild.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
+|[![Pypi](https://badgen.net/badge/icon/findmyorder?icon=pypi&label)](https://pypi.org/project/findmyorder/) ![Version](https://img.shields.io/pypi/v/findmyorder)<br>  ![Pypi](https://img.shields.io/pypi/dm/findmyorder)<br> [![Build](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/findmyorder/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/findmyorder/branch/dev/graph/badge.svg?token=4838MSZNCC)](https://codecov.io/gh/mraniki/findmyorder) | Find & Parse a trade order for execution|
 
 
 
 Key features:
 
 - Identify an order with word `BUY SELL LONG SHORT` or your own `Bull`, `to the moon`, `pump` via config file
 - Parse and return a structured order with action and instrument as mandatory
```

