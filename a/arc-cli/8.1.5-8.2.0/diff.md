# Comparing `tmp/arc_cli-8.1.5.tar.gz` & `tmp/arc_cli-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arc_cli-8.1.5.tar", max compression
+gzip compressed data, was "arc_cli-8.2.0.tar", max compression
```

## Comparing `arc_cli-8.1.5.tar` & `arc_cli-8.2.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      944 2023-04-24 02:20:30.375199 arc_cli-8.1.5/README.md
--rw-r--r--   0        0        0      719 2023-05-03 23:15:25.110255 arc_cli-8.1.5/arc/__init__.py
--rw-r--r--   0        0        0     1449 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/api.py
--rw-r--r--   0        0        0     6902 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/autocompletions.py
--rw-r--r--   0        0        0     2189 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/autoload.py
--rw-r--r--   0        0        0      114 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/color.py
--rw-r--r--   0        0        0     5732 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/config.py
--rw-r--r--   0        0        0      385 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/constants.py
--rw-r--r--   0        0        0      121 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/define/__init__.py
--rw-r--r--   0        0        0     1379 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/define/alias.py
--rw-r--r--   0        0        0     1768 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/define/classful.py
--rw-r--r--   0        0        0    17181 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/define/command.py
--rw-r--r--   0        0        0     3118 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/define/documentation.py
--rw-r--r--   0        0        0      219 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/define/param/__init__.py
--rw-r--r--   0        0        0     8036 2023-04-24 02:18:25.036233 arc_cli-8.1.5/arc/define/param/constructors.py
--rw-r--r--   0        0        0     3499 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/define/param/groups.py
--rw-r--r--   0        0        0     8706 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/define/param/param.py
--rw-r--r--   0        0        0     8549 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/define/param/param_definition.py
--rw-r--r--   0        0        0     3388 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/define/param/param_mixin.py
--rw-r--r--   0        0        0     1889 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/define/param/param_tree.py
--rw-r--r--   0        0        0     6314 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/errors.py
--rw-r--r--   0        0        0     1070 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/logging.py
--rw-r--r--   0        0        0    16336 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/parser.py
--rw-r--r--   0        0        0      402 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/__init__.py
--rw-r--r--   0        0        0     6168 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/ansi.py
--rw-r--r--   0        0        0     4681 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/box.py
--rw-r--r--   0        0        0     5128 2023-04-30 22:22:00.176143 arc_cli-8.1.5/arc/present/console.py
--rw-r--r--   0        0        0      187 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/data.py
--rw-r--r--   0        0        0     2126 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/drawing.py
--rw-r--r--   0        0        0     2748 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/formatters.py
--rw-r--r--   0        0        0     9078 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/help_formatter.py
--rw-r--r--   0        0        0     3024 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/joiner.py
--rw-r--r--   0        0        0       54 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/markdown/__init__.py
--rw-r--r--   0        0        0     6473 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/markdown/markdown_parser.py
--rw-r--r--   0        0        0     3754 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/markdown/nodes.py
--rw-r--r--   0        0        0     1632 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/out.py
--rw-r--r--   0        0        0      987 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/pager.py
--rw-r--r--   0        0        0     9825 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/table.py
--rw-r--r--   0        0        0     5182 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/present/wrap.py
--rw-r--r--   0        0        0      288 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/prompt/__init__.py
--rw-r--r--   0        0        0     3722 2023-04-30 19:31:15.828580 arc_cli-8.1.5/arc/prompt/helpers.py
--rw-r--r--   0        0        0     5926 2023-04-24 02:18:25.039567 arc_cli-8.1.5/arc/prompt/prompt.py
--rw-r--r--   0        0        0      812 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/prompt/prompts.py
--rw-r--r--   0        0        0     7019 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/prompt/questions.py
--rw-r--r--   0        0        0        0 2023-03-18 01:38:52.879777 arc_cli-8.1.5/arc/py.typed
--rw-r--r--   0        0        0      306 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/runtime/__init__.py
--rw-r--r--   0        0        0     2970 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/runtime/app.py
--rw-r--r--   0        0        0     2678 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/runtime/context.py
--rw-r--r--   0        0        0    12517 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/runtime/exec.py
--rw-r--r--   0        0        0     8240 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/runtime/init.py
--rw-r--r--   0        0        0     7402 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/runtime/middleware.py
--rw-r--r--   0        0        0      382 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/safe.py
--rw-r--r--   0        0        0     1866 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/suggest.py
--rw-r--r--   0        0        0      362 2023-04-30 19:42:21.213131 arc_cli-8.1.5/arc/types/__init__.py
--rw-r--r--   0        0        0    13898 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/aliases.py
--rw-r--r--   0        0        0      670 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/convert.py
--rw-r--r--   0        0        0      545 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/default.py
--rw-r--r--   0        0        0     4422 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/file.py
--rw-r--r--   0        0        0       79 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/middleware/__init__.py
--rw-r--r--   0        0        0     1403 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/middleware/observers.py
--rw-r--r--   0        0        0     2630 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/middleware/transformers.py
--rw-r--r--   0        0        0     4042 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/middleware/validators.py
--rw-r--r--   0        0        0     3486 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/network.py
--rw-r--r--   0        0        0      854 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/numbers.py
--rw-r--r--   0        0        0      860 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/path.py
--rw-r--r--   0        0        0     6881 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/semver.py
--rw-r--r--   0        0        0      877 2023-04-24 02:18:25.042900 arc_cli-8.1.5/arc/types/state.py
--rw-r--r--   0        0        0     1921 2023-04-24 02:18:25.046233 arc_cli-8.1.5/arc/types/strings.py
--rw-r--r--   0        0        0     2155 2023-04-24 02:18:25.046233 arc_cli-8.1.5/arc/types/type_arg.py
--rw-r--r--   0        0        0     2718 2023-04-24 02:18:25.046233 arc_cli-8.1.5/arc/types/type_info.py
--rw-r--r--   0        0        0     3176 2023-04-24 02:18:25.046233 arc_cli-8.1.5/arc/types/users.py
--rw-r--r--   0        0        0     2257 2023-04-24 02:18:25.046233 arc_cli-8.1.5/arc/typing.py
--rw-r--r--   0        0        0     1064 2023-05-03 23:15:25.766917 arc_cli-8.1.5/pyproject.toml
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 arc_cli-8.1.5/setup.py
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 arc_cli-8.1.5/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-04-24 02:20:30.375199 arc_cli-8.2.0/README.md
+-rw-r--r--   0        0        0      719 2023-05-04 02:59:16.987114 arc_cli-8.2.0/arc/__init__.py
+-rw-r--r--   0        0        0     1449 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/api.py
+-rw-r--r--   0        0        0     6902 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/autocompletions.py
+-rw-r--r--   0        0        0     2189 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/autoload.py
+-rw-r--r--   0        0        0      114 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/color.py
+-rw-r--r--   0        0        0     5732 2023-05-04 02:54:46.601724 arc_cli-8.2.0/arc/config.py
+-rw-r--r--   0        0        0      385 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/constants.py
+-rw-r--r--   0        0        0      121 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/__init__.py
+-rw-r--r--   0        0        0     1379 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/alias.py
+-rw-r--r--   0        0        0     1768 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/classful.py
+-rw-r--r--   0        0        0    17181 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/command.py
+-rw-r--r--   0        0        0     3118 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/documentation.py
+-rw-r--r--   0        0        0      219 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/param/__init__.py
+-rw-r--r--   0        0        0     8036 2023-04-24 02:18:25.036233 arc_cli-8.2.0/arc/define/param/constructors.py
+-rw-r--r--   0        0        0     3499 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/groups.py
+-rw-r--r--   0        0        0     8706 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/param.py
+-rw-r--r--   0        0        0     8549 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/param_definition.py
+-rw-r--r--   0        0        0     3388 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/param_mixin.py
+-rw-r--r--   0        0        0     1889 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/define/param/param_tree.py
+-rw-r--r--   0        0        0     6314 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/errors.py
+-rw-r--r--   0        0        0     1070 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/logging.py
+-rw-r--r--   0        0        0    16336 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/parser.py
+-rw-r--r--   0        0        0      402 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/__init__.py
+-rw-r--r--   0        0        0     6168 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/ansi.py
+-rw-r--r--   0        0        0     4681 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/box.py
+-rw-r--r--   0        0        0     5319 2023-05-04 02:58:09.317495 arc_cli-8.2.0/arc/present/console.py
+-rw-r--r--   0        0        0      187 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/data.py
+-rw-r--r--   0        0        0     2126 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/drawing.py
+-rw-r--r--   0        0        0     2748 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/formatters.py
+-rw-r--r--   0        0        0     9078 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/help_formatter.py
+-rw-r--r--   0        0        0     3024 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/joiner.py
+-rw-r--r--   0        0        0       54 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/markdown/__init__.py
+-rw-r--r--   0        0        0     6614 2023-05-04 02:56:40.521271 arc_cli-8.2.0/arc/present/markdown/markdown_parser.py
+-rw-r--r--   0        0        0     3894 2023-05-04 02:54:24.375128 arc_cli-8.2.0/arc/present/markdown/nodes.py
+-rw-r--r--   0        0        0     1632 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/out.py
+-rw-r--r--   0        0        0      987 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/pager.py
+-rw-r--r--   0        0        0     9825 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/table.py
+-rw-r--r--   0        0        0     5182 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/present/wrap.py
+-rw-r--r--   0        0        0      288 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/prompt/__init__.py
+-rw-r--r--   0        0        0     3722 2023-04-30 19:31:15.828580 arc_cli-8.2.0/arc/prompt/helpers.py
+-rw-r--r--   0        0        0     5926 2023-04-24 02:18:25.039567 arc_cli-8.2.0/arc/prompt/prompt.py
+-rw-r--r--   0        0        0      812 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/prompt/prompts.py
+-rw-r--r--   0        0        0     7019 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/prompt/questions.py
+-rw-r--r--   0        0        0        0 2023-03-18 01:38:52.879777 arc_cli-8.2.0/arc/py.typed
+-rw-r--r--   0        0        0      306 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/__init__.py
+-rw-r--r--   0        0        0     2970 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/app.py
+-rw-r--r--   0        0        0     2678 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/context.py
+-rw-r--r--   0        0        0    12517 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/exec.py
+-rw-r--r--   0        0        0     8240 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/init.py
+-rw-r--r--   0        0        0     7402 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/runtime/middleware.py
+-rw-r--r--   0        0        0      382 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/safe.py
+-rw-r--r--   0        0        0     1866 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/suggest.py
+-rw-r--r--   0        0        0      362 2023-04-30 19:42:21.213131 arc_cli-8.2.0/arc/types/__init__.py
+-rw-r--r--   0        0        0    13898 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/aliases.py
+-rw-r--r--   0        0        0      670 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/convert.py
+-rw-r--r--   0        0        0      545 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/default.py
+-rw-r--r--   0        0        0     4422 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/file.py
+-rw-r--r--   0        0        0       79 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/middleware/__init__.py
+-rw-r--r--   0        0        0     1403 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/middleware/observers.py
+-rw-r--r--   0        0        0     2630 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/middleware/transformers.py
+-rw-r--r--   0        0        0     4042 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/middleware/validators.py
+-rw-r--r--   0        0        0     3486 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/network.py
+-rw-r--r--   0        0        0      854 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/numbers.py
+-rw-r--r--   0        0        0      860 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/path.py
+-rw-r--r--   0        0        0     6881 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/semver.py
+-rw-r--r--   0        0        0      877 2023-04-24 02:18:25.042900 arc_cli-8.2.0/arc/types/state.py
+-rw-r--r--   0        0        0     1921 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/types/strings.py
+-rw-r--r--   0        0        0     2155 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/types/type_arg.py
+-rw-r--r--   0        0        0     2718 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/types/type_info.py
+-rw-r--r--   0        0        0     3176 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/types/users.py
+-rw-r--r--   0        0        0     2257 2023-04-24 02:18:25.046233 arc_cli-8.2.0/arc/typing.py
+-rw-r--r--   0        0        0     1021 2023-05-04 02:59:17.663776 arc_cli-8.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 arc_cli-8.2.0/setup.py
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 arc_cli-8.2.0/PKG-INFO
```

### Comparing `arc_cli-8.1.5/README.md` & `arc_cli-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/__init__.py` & `arc_cli-8.2.0/arc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "8.1.5"
+__version__ = "8.2.0"
 
 from arc import types, prompt, present, errors
 from arc.config import (
     ColorConfig,
     Config,
     LinksConfig,
     SuggestionConfig,
```

### Comparing `arc_cli-8.1.5/arc/api.py` & `arc_cli-8.2.0/arc/api.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/autocompletions.py` & `arc_cli-8.2.0/arc/autocompletions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/autoload.py` & `arc_cli-8.2.0/arc/autoload.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/config.py` & `arc_cli-8.2.0/arc/config.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/alias.py` & `arc_cli-8.2.0/arc/define/alias.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/classful.py` & `arc_cli-8.2.0/arc/define/classful.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/command.py` & `arc_cli-8.2.0/arc/define/command.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/documentation.py` & `arc_cli-8.2.0/arc/define/documentation.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/param/constructors.py` & `arc_cli-8.2.0/arc/define/param/constructors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/param/groups.py` & `arc_cli-8.2.0/arc/define/param/groups.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/param/param.py` & `arc_cli-8.2.0/arc/define/param/param.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/param/param_definition.py` & `arc_cli-8.2.0/arc/define/param/param_definition.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/param/param_mixin.py` & `arc_cli-8.2.0/arc/define/param/param_mixin.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/define/param/param_tree.py` & `arc_cli-8.2.0/arc/define/param/param_tree.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/errors.py` & `arc_cli-8.2.0/arc/errors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/logging.py` & `arc_cli-8.2.0/arc/logging.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/parser.py` & `arc_cli-8.2.0/arc/parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/ansi.py` & `arc_cli-8.2.0/arc/present/ansi.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/box.py` & `arc_cli-8.2.0/arc/present/box.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/console.py` & `arc_cli-8.2.0/arc/present/console.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,14 +129,18 @@
             objects.append(last)
 
         self.print(
             *objects,
             **kwargs,
         )
 
+    def rule(self, string: str = "", width: int = 80, **kwargs: t.Any) -> None:
+        """Display a horizontal rule to the user"""
+        self.print(string.center(width, "─"), **kwargs)
+
     def ok(self, *values: object, **kwargs: t.Any) -> None:
         """Display a successful message to the user"""
         self._decorate(*values, color=fg.GREEN, icon=self.icons["ok"], **kwargs)
 
     def err(self, *values: object, **kwargs: t.Any) -> None:
         """Display an unsuccessful message to the user"""
         self._decorate(*values, color=fg.RED, icon=self.icons["error"], **kwargs)
```

### Comparing `arc_cli-8.1.5/arc/present/drawing.py` & `arc_cli-8.2.0/arc/present/drawing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/formatters.py` & `arc_cli-8.2.0/arc/present/formatters.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/help_formatter.py` & `arc_cli-8.2.0/arc/present/help_formatter.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/joiner.py` & `arc_cli-8.2.0/arc/present/joiner.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/markdown/markdown_parser.py` & `arc_cli-8.2.0/arc/present/markdown/markdown_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Spacer,
     Strikethrough,
     Strong,
     Text,
     Underline,
     Unformatted,
     Colored,
+    HorizontalRule,
 )
 
 if t.TYPE_CHECKING:
     from arc.config import PresentConfig
 
 
 class InputDeque(deque[str]):
@@ -45,14 +46,17 @@
             if not curr:
                 stream.popleft()
                 continue
 
             if curr.startswith("#"):
                 stream.popleft()
                 nodes.append(self.parse_heading(curr))
+            elif curr.startswith("---"):
+                stream.popleft()
+                nodes.append(HorizontalRule())
             elif curr.startswith("-"):
                 nodes.append(self.parse_list(stream))
             elif curr == "```":
                 stream.popleft()
                 nodes.append(self.parse_unformatted(stream))
             else:
                 nodes.append(self.parse_paragraph(stream))
```

### Comparing `arc_cli-8.1.5/arc/present/markdown/nodes.py` & `arc_cli-8.2.0/arc/present/markdown/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,20 @@
     content: str
 
     def fmt(self, config: PresentConfig) -> str:
         return self.content + "\n\n"
 
 
 @dataclass
+class HorizontalRule(BlockNode):
+    def fmt(self, config: PresentConfig) -> str:
+        return "—" * config.width + "\n\n"
+
+
+@dataclass
 class Text(InlineNode):
     children: list[InlineNode]
 
     def fmt(self, config: PresentConfig) -> str:
         return Join.together(child.fmt(config) for child in self.children)
```

### Comparing `arc_cli-8.1.5/arc/present/out.py` & `arc_cli-8.2.0/arc/present/out.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/pager.py` & `arc_cli-8.2.0/arc/present/pager.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/table.py` & `arc_cli-8.2.0/arc/present/table.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/present/wrap.py` & `arc_cli-8.2.0/arc/present/wrap.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/prompt/helpers.py` & `arc_cli-8.2.0/arc/prompt/helpers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/prompt/prompt.py` & `arc_cli-8.2.0/arc/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/prompt/prompts.py` & `arc_cli-8.2.0/arc/prompt/prompts.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/prompt/questions.py` & `arc_cli-8.2.0/arc/prompt/questions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/runtime/app.py` & `arc_cli-8.2.0/arc/runtime/app.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/runtime/context.py` & `arc_cli-8.2.0/arc/runtime/context.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/runtime/exec.py` & `arc_cli-8.2.0/arc/runtime/exec.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/runtime/init.py` & `arc_cli-8.2.0/arc/runtime/init.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/runtime/middleware.py` & `arc_cli-8.2.0/arc/runtime/middleware.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/suggest.py` & `arc_cli-8.2.0/arc/suggest.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/aliases.py` & `arc_cli-8.2.0/arc/types/aliases.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/convert.py` & `arc_cli-8.2.0/arc/types/convert.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/default.py` & `arc_cli-8.2.0/arc/types/default.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/file.py` & `arc_cli-8.2.0/arc/types/file.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/middleware/observers.py` & `arc_cli-8.2.0/arc/types/middleware/observers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/middleware/transformers.py` & `arc_cli-8.2.0/arc/types/middleware/transformers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/middleware/validators.py` & `arc_cli-8.2.0/arc/types/middleware/validators.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/network.py` & `arc_cli-8.2.0/arc/types/network.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/numbers.py` & `arc_cli-8.2.0/arc/types/numbers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/path.py` & `arc_cli-8.2.0/arc/types/path.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/semver.py` & `arc_cli-8.2.0/arc/types/semver.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/state.py` & `arc_cli-8.2.0/arc/types/state.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/strings.py` & `arc_cli-8.2.0/arc/types/strings.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/type_arg.py` & `arc_cli-8.2.0/arc/types/type_arg.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/type_info.py` & `arc_cli-8.2.0/arc/types/type_info.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/types/users.py` & `arc_cli-8.2.0/arc/types/users.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/arc/typing.py` & `arc_cli-8.2.0/arc/typing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.1.5/pyproject.toml` & `arc_cli-8.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arc-cli"
-version = "8.1.5"
+version = "8.2.0"
 description = "A Regular CLI"
 authors = ["Sean Collings <seanrcollings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/arc"
 documentation = "https://arc.seanrcollings.com"
 keywords = ["CLI", "extendable", "easy", "arc"]
@@ -30,13 +30,10 @@
 types-PyYAML = "^6.0.1"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 Jinja2 = "3.0.3"
 mkdocs-awesome-pages-plugin = "^2.8.0"
 hypothesis = "^6.68.2"
 pygithub = "^1.58.1"
 
-[tool.poetry.scripts]
-cli = "cli:command"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `arc_cli-8.1.5/setup.py` & `arc_cli-8.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,24 @@
  'arc.runtime',
  'arc.types',
  'arc.types.middleware']
 
 package_data = \
 {'': ['*']}
 
-entry_points = \
-{'console_scripts': ['cli = cli:command']}
-
 setup_kwargs = {
     'name': 'arc-cli',
-    'version': '8.1.5',
+    'version': '8.2.0',
     'description': 'A Regular CLI',
     'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.9\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# [Docs](http://arc.seanrcollings.com)\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
     'author': 'Sean Collings',
     'author_email': 'seanrcollings@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/arc',
     'packages': packages,
     'package_data': package_data,
-    'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `arc_cli-8.1.5/PKG-INFO` & `arc_cli-8.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arc-cli
-Version: 8.1.5
+Version: 8.2.0
 Summary: A Regular CLI
 Home-page: https://github.com/seanrcollings/arc
 License: MIT
 Keywords: CLI,extendable,easy,arc
 Author: Sean Collings
 Author-email: seanrcollings@gmail.com
 Requires-Python: >=3.10,<4.0
```

