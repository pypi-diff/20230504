# Comparing `tmp/beaupy-3.5.3b0.tar.gz` & `tmp/beaupy-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaupy-3.5.3b0.tar", max compression
+gzip compressed data, was "beaupy-3.5.4.tar", max compression
```

## Comparing `beaupy-3.5.3b0.tar` & `beaupy-3.5.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1111 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/LICENSE
--rw-r--r--   0        0        0     8118 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/README.md
--rw-r--r--   0        0        0      260 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/__init__.py
--rwxr-xr-x   0        0        0    23689 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/_beaupy.py
--rw-r--r--   0        0        0     4059 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/_internals.py
--rw-r--r--   0        0        0      170 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/spinners/__init__.py
--rw-r--r--   0        0        0     2335 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/spinners/_spinners.py
--rw-r--r--   0        0        0     3664 2023-04-15 15:17:25.867836 beaupy-3.5.3b0/pyproject.toml
--rw-r--r--   0        0        0     9168 1970-01-01 00:00:00.000000 beaupy-3.5.3b0/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-04 21:37:51.073099 beaupy-3.5.4/LICENSE
+-rw-r--r--   0        0        0     8171 2023-05-04 21:37:51.073099 beaupy-3.5.4/README.md
+-rw-r--r--   0        0        0      260 2023-05-04 21:37:51.073099 beaupy-3.5.4/beaupy/__init__.py
+-rwxr-xr-x   0        0        0    23732 2023-05-04 21:37:51.073099 beaupy-3.5.4/beaupy/_beaupy.py
+-rw-r--r--   0        0        0     4059 2023-05-04 21:37:51.073099 beaupy-3.5.4/beaupy/_internals.py
+-rw-r--r--   0        0        0      170 2023-05-04 21:37:51.073099 beaupy-3.5.4/beaupy/spinners/__init__.py
+-rw-r--r--   0        0        0     2335 2023-05-04 21:37:51.073099 beaupy-3.5.4/beaupy/spinners/_spinners.py
+-rw-r--r--   0        0        0     3662 2023-05-04 21:37:51.077099 beaupy-3.5.4/pyproject.toml
+-rw-r--r--   0        0        0     9219 1970-01-01 00:00:00.000000 beaupy-3.5.4/PKG-INFO
```

### Comparing `beaupy-3.5.3b0/LICENSE` & `beaupy-3.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.3b0/README.md` & `beaupy-3.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 
 TUI elements shown in the above gif are the result of the follwing code:
 
 ```python
 import time
 from beaupy import confirm, prompt, select, select_multiple
 from beaupy.spinners import *
+from rich.console import Console
 
+console = Console()
 
 # Confirm a dialog
 if confirm("Will you take the ring to Mordor?"):
     names = [
         "Frodo Baggins",
         "Samwise Gamgee",
         "Legolas",
```

### Comparing `beaupy-3.5.3b0/beaupy/_beaupy.py` & `beaupy-3.5.4/beaupy/_beaupy.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,15 +361,15 @@
             show_from = (page - 1) * page_size
             show_to = min(show_from + page_size, len(options))
             rendered = (  # noqa: ECE001
                 '\n'.join(
                     [
                         _render_option_select_multiple(
                             option=preprocessor(option),
-                            ticked=i + show_from in ticked_indices,
+                            ticked=(i + show_from in ticked_indices) if pagination else (i in ticked_indices),
                             tick_character=tick_character,
                             tick_style=tick_style,
                             selected=i == (index % page_size if pagination else index),
                             cursor_style=cursor_style,
                         )
                         for i, option in enumerate(options[show_from:show_to] if pagination else options)
                     ]
```

### Comparing `beaupy-3.5.3b0/beaupy/_internals.py` & `beaupy-3.5.4/beaupy/_internals.py`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.3b0/beaupy/spinners/_spinners.py` & `beaupy-3.5.4/beaupy/spinners/_spinners.py`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.3b0/pyproject.toml` & `beaupy-3.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'beaupy'
-version = '3.5.3b0'
+version = '3.5.4'
 description = 'A library of elements for interactive TUIs in Python'
 authors = ['Peter Vyboch <pvyboch1@gmail.com>']
 license = 'MIT'
 repository = 'https://github.com/petereon/beaupy'
 readme = 'README.md'
 keywords = ["cli", "interactive", "console", "terminal", "interface"]
 classifiers = [
```

### Comparing `beaupy-3.5.3b0/PKG-INFO` & `beaupy-3.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaupy
-Version: 3.5.3b0
+Version: 3.5.4
 Summary: A library of elements for interactive TUIs in Python
 Home-page: https://github.com/petereon/beaupy
 License: MIT
 Keywords: cli,interactive,console,terminal,interface
 Author: Peter Vyboch
 Author-email: pvyboch1@gmail.com
 Requires-Python: >=3.7.8,<4.0.0
@@ -61,15 +61,17 @@
 
 TUI elements shown in the above gif are the result of the follwing code:
 
 ```python
 import time
 from beaupy import confirm, prompt, select, select_multiple
 from beaupy.spinners import *
+from rich.console import Console
 
+console = Console()
 
 # Confirm a dialog
 if confirm("Will you take the ring to Mordor?"):
     names = [
         "Frodo Baggins",
         "Samwise Gamgee",
         "Legolas",
```

