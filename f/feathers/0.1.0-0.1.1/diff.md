# Comparing `tmp/feathers-0.1.0.tar.gz` & `tmp/feathers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feathers-0.1.0.tar", max compression
+gzip compressed data, was "feathers-0.1.1.tar", max compression
```

## Comparing `feathers-0.1.0.tar` & `feathers-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       29 2023-05-04 03:02:56.756859 feathers-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-04 03:02:56.757405 feathers-0.1.0/feathers/__init__.py
--rw-r--r--   0        0        0       53 2023-05-04 03:02:56.757817 feathers-0.1.0/feathers/__main__.py
--rw-r--r--   0        0        0      161 2023-05-04 03:02:56.758079 feathers-0.1.0/feathers/demo.py
--rw-r--r--   0        0        0       97 2023-05-04 03:02:56.758329 feathers-0.1.0/feathers/widgets/__init__.py
--rw-r--r--   0        0        0      118 2023-05-04 03:02:56.758599 feathers-0.1.0/feathers/widgets/help/__init__.py
--rw-r--r--   0        0        0      946 2023-05-04 03:02:56.758877 feathers-0.1.0/feathers/widgets/help/_base.py
--rw-r--r--   0        0        0     1744 2023-05-04 03:02:56.759134 feathers-0.1.0/feathers/widgets/help/_help.py
--rw-r--r--   0        0        0     5944 2023-05-04 03:02:56.759382 feathers-0.1.0/feathers/widgets/help/_long_help.py
--rw-r--r--   0        0        0      714 2023-05-04 03:02:56.759620 feathers-0.1.0/feathers/widgets/help/_models.py
--rw-r--r--   0        0        0     3702 2023-05-04 03:02:56.759897 feathers-0.1.0/feathers/widgets/help/_short_help.py
--rw-r--r--   0        0        0     1307 2023-05-04 03:02:56.760167 feathers-0.1.0/feathers/widgets/help/_utils.py
--rw-r--r--   0        0        0      833 2023-05-04 03:02:56.760511 feathers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 feathers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-04 04:58:16.361797 feathers-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/__main__.py
+-rw-r--r--   0        0        0      161 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/demo.py
+-rw-r--r--   0        0        0       97 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/__init__.py
+-rw-r--r--   0        0        0     1002 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_base.py
+-rw-r--r--   0        0        0     1684 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_help.py
+-rw-r--r--   0        0        0     5944 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_long_help.py
+-rw-r--r--   0        0        0      714 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_models.py
+-rw-r--r--   0        0        0     3948 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_short_help.py
+-rw-r--r--   0        0        0     1307 2023-05-04 04:58:16.361797 feathers-0.1.1/feathers/widgets/help/_utils.py
+-rw-r--r--   0        0        0      882 2023-05-04 04:58:16.361797 feathers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 feathers-0.1.1/PKG-INFO
```

### Comparing `feathers-0.1.0/feathers/widgets/help/_base.py` & `feathers-0.1.1/feathers/widgets/help/_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,13 +19,16 @@
         self.watch(self.screen, "focused", self.__reset)
         self.watch(self.screen, "stack_updates", self.__reset)
 
     @abstractmethod
     def _create_help(self) -> Text:
         pass
 
+    def _can_switch(self) -> bool:
+        return True
+
     def _get_entries_from_bindings(self) -> list[HelpEntry]:
         binding_entries = set([HelpEntry.from_binding(b) for (_, b) in self.app.namespace_bindings.values() if b.show])
         return sorted(list(binding_entries), key=lambda entry: entry.name)
 
     def __reset(self, _: Widget | None) -> None:
         self.update(self._create_help())
```

### Comparing `feathers-0.1.0/feathers/widgets/help/_help.py` & `feathers-0.1.1/feathers/widgets/help/_help.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from textual.app import ComposeResult
 from textual.widget import Widget
 from textual.widgets import ContentSwitcher
 
+from ._base import BaseHelp
 from ._long_help import LongHelp
 from ._models import HelpEntry
 from ._short_help import ShortHelp
 
 
 class Help(Widget):
     """A single and multi line mode help widget to display key bindings"""
@@ -33,23 +34,22 @@
         long_help_separator: str = "  ",
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
     ) -> None:
         super().__init__(name=name, id=id, classes=classes, disabled=disabled)
-        self.toggle_key = toggle_key
-        self.short_help_separator = short_help_separator
-        self.short_help_placeholder = short_help_placeholder
-        self.long_help_separator = long_help_separator
+
+        self._short_help: BaseHelp = ShortHelp("short-help", toggle_key, short_help_separator, short_help_placeholder)
+        self._long_help: BaseHelp = LongHelp("long-help", long_help_separator)
 
     def compose(self) -> ComposeResult:
         with ContentSwitcher(initial="short-help"):
-            yield ShortHelp("short-help", self.toggle_key, self.short_help_separator, self.short_help_placeholder)
-            yield LongHelp("long-help", self.long_help_separator)
+            yield self._short_help
+            yield self._long_help
 
     def toggle_view(self) -> None:
         switcher = self.query_one(ContentSwitcher)
-        if switcher.current == "short-help":
+        if switcher.current == "short-help" and self._short_help._can_switch():
             switcher.current = "long-help"
         else:
             switcher.current = "short-help"
```

### Comparing `feathers-0.1.0/feathers/widgets/help/_long_help.py` & `feathers-0.1.1/feathers/widgets/help/_long_help.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.0/feathers/widgets/help/_models.py` & `feathers-0.1.1/feathers/widgets/help/_models.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.0/feathers/widgets/help/_short_help.py` & `feathers-0.1.1/feathers/widgets/help/_short_help.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         separator: str,
         placeholder_text: str = "No key mappings found. Trying changing focus",
     ) -> None:
         super().__init__(id=id)
         self.toggle_key = toggle_key
         self.separator = separator
         self.placeholder_text: str = placeholder_text
+        self._can_switch_to_long_help: bool = False
 
     def __entry_text(self, entry: HelpEntry) -> Text:
         key_style = self.get_component_rich_style("shorthelp--key")
         description_style = self.get_component_rich_style("shorthelp--description")
         return Text.assemble((entry.name.lower(), key_style), (f" {entry.description.lower()}", description_style))
 
     def __get_placeholder_text(self) -> Text:
@@ -91,27 +92,33 @@
 
     def __has_long_help_entries(self, entries: list[HelpEntry]) -> bool:
         long_help_entries = self._get_entries_from_bindings()
         if self.toggle_key in long_help_entries:
             long_help_entries.remove(self.toggle_key)
         return bool(set(long_help_entries) - set(entries))
 
+    def _can_switch(self) -> bool:
+        return self._can_switch_to_long_help
+
     def _create_help(self) -> Text:
         text = Text(
             style=self.rich_style,
             no_wrap=True,
             overflow="ellipsis",
             justify="left",
             end="",
         )
 
         entries = self.__get_entries()
 
         if self.__has_long_help_entries(entries):
+            self._can_switch_to_long_help = True
             entries.append(self.toggle_key)
+        else:
+            self._can_switch_to_long_help = False
 
         if len(entries) == 0:
             return self.__get_placeholder_text()
 
         separator_style = self.get_component_rich_style("shorthelp--separator")
         separator = text.append(self.separator, separator_style)
```

### Comparing `feathers-0.1.0/feathers/widgets/help/_utils.py` & `feathers-0.1.1/feathers/widgets/help/_utils.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.0/pyproject.toml` & `feathers-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feathers"
-version = "0.1.0"
+version = "0.1.1"
 description = "Beautiful TUI components written on top of Textual"
 authors = ["Shashank Tomar <shashank004@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "feathers"}]
 repository = "https://github.com/shashanktomar/feathers"
 keywords = ["textual", "terminal", "TUI"]
@@ -17,14 +17,16 @@
 
 [tool.poetry.group.dev.dependencies]
 textual = {extras = ["dev"], version = "^0.22.3"}
 ruff = "^0.0.264"
 black = "^23.3.0"
 mypy = "^1.2.0"
 pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
```

### Comparing `feathers-0.1.0/PKG-INFO` & `feathers-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feathers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Beautiful TUI components written on top of Textual
 Home-page: https://github.com/shashanktomar/feathers
 License: MIT
 Keywords: textual,terminal,TUI
 Author: Shashank Tomar
 Author-email: shashank004@gmail.com
 Requires-Python: >=3.8,<4.0
```

