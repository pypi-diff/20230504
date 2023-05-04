# Comparing `tmp/oida-0.1.5.tar.gz` & `tmp/oida-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oida-0.1.5.tar", max compression
+gzip compressed data, was "oida-0.2.0.tar", max compression
```

## Comparing `oida-0.1.5.tar` & `oida-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3663 2023-04-20 08:33:56.049482 oida-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-20 08:33:56.049482 oida-0.1.5/oida/__init__.py
--rw-r--r--   0        0        0       65 2023-04-20 08:33:56.049482 oida-0.1.5/oida/__main__.py
--rw-r--r--   0        0        0      616 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/__init__.py
--rw-r--r--   0        0        0     1628 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/base.py
--rw-r--r--   0        0        0     6855 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/components.py
--rw-r--r--   0        0        0     4325 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/config.py
--rw-r--r--   0        0        0     1334 2023-04-20 08:33:56.049482 oida-0.1.5/oida/checkers/imports.py
--rw-r--r--   0        0        0      190 2023-04-20 08:33:56.049482 oida-0.1.5/oida/commands/__init__.py
--rw-r--r--   0        0        0     9720 2023-04-20 08:33:56.049482 oida-0.1.5/oida/commands/componentize.py
--rw-r--r--   0        0        0     1007 2023-04-20 08:33:56.049482 oida-0.1.5/oida/commands/config.py
--rw-r--r--   0        0        0     1177 2023-04-20 08:33:56.049482 oida-0.1.5/oida/commands/linter.py
--rw-r--r--   0        0        0     1502 2023-04-20 08:33:56.049482 oida-0.1.5/oida/config.py
--rw-r--r--   0        0        0     5568 2023-04-20 08:33:56.049482 oida-0.1.5/oida/config_generator.py
--rw-r--r--   0        0        0     1875 2023-04-20 08:33:56.049482 oida-0.1.5/oida/console.py
--rw-r--r--   0        0        0     3755 2023-04-20 08:33:56.049482 oida-0.1.5/oida/discovery.py
--rw-r--r--   0        0        0     1245 2023-04-20 08:33:56.049482 oida-0.1.5/oida/flake8.py
--rw-r--r--   0        0        0      548 2023-04-20 08:33:56.049482 oida-0.1.5/oida/module.py
--rw-r--r--   0        0        0      515 2023-04-20 08:33:56.049482 oida-0.1.5/oida/utils.py
--rw-r--r--   0        0        0     1869 2023-04-20 08:33:56.049482 oida-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 oida-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3663 2023-05-04 12:53:25.672179 oida-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 12:53:25.672179 oida-0.2.0/oida/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-04 12:53:25.672179 oida-0.2.0/oida/__main__.py
+-rw-r--r--   0        0        0      616 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/__init__.py
+-rw-r--r--   0        0        0     1628 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/base.py
+-rw-r--r--   0        0        0     7001 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/components.py
+-rw-r--r--   0        0        0     4325 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/config.py
+-rw-r--r--   0        0        0     1334 2023-05-04 12:53:25.672179 oida-0.2.0/oida/checkers/imports.py
+-rw-r--r--   0        0        0      190 2023-05-04 12:53:25.672179 oida-0.2.0/oida/commands/__init__.py
+-rw-r--r--   0        0        0     9720 2023-05-04 12:53:25.672179 oida-0.2.0/oida/commands/componentize.py
+-rw-r--r--   0        0        0     1007 2023-05-04 12:53:25.672179 oida-0.2.0/oida/commands/config.py
+-rw-r--r--   0        0        0     1177 2023-05-04 12:53:25.672179 oida-0.2.0/oida/commands/linter.py
+-rw-r--r--   0        0        0     1419 2023-05-04 12:53:25.672179 oida-0.2.0/oida/config.py
+-rw-r--r--   0        0        0     5568 2023-05-04 12:53:25.672179 oida-0.2.0/oida/config_generator.py
+-rw-r--r--   0        0        0     1875 2023-05-04 12:53:25.672179 oida-0.2.0/oida/console.py
+-rw-r--r--   0        0        0     3755 2023-05-04 12:53:25.672179 oida-0.2.0/oida/discovery.py
+-rw-r--r--   0        0        0     1245 2023-05-04 12:53:25.672179 oida-0.2.0/oida/flake8.py
+-rw-r--r--   0        0        0      548 2023-05-04 12:53:25.672179 oida-0.2.0/oida/module.py
+-rw-r--r--   0        0        0      985 2023-05-04 12:53:25.672179 oida-0.2.0/oida/utils.py
+-rw-r--r--   0        0        0     1869 2023-05-04 12:53:25.676179 oida-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 oida-0.2.0/PKG-INFO
```

### Comparing `oida-0.1.5/README.md` & `oida-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/checkers/__init__.py` & `oida-0.2.0/oida/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/checkers/base.py` & `oida-0.2.0/oida/checkers/base.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/checkers/components.py` & `oida-0.2.0/oida/checkers/components.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ast
 from contextlib import contextmanager
 from functools import reduce
 from typing import Any, Iterator
 
 from ..config import ComponentConfig, ProjectConfig
+from ..utils import path_in_glob_list
 from .base import Checker, Code
 
 
 class ComponentIsolationChecker(Checker):
     """
     Check that isolation between components are respected. That means that all
     imports from other components should be from the other component's top
@@ -66,40 +67,39 @@
 
         return False
 
     def is_access_allowed(self, path: list[str]) -> bool:
         """Check of access to this name is allowed, not considering ignored rules"""
         return len(path) <= 4
 
+    def is_violation_globally_silenced(self, path: list[str]) -> bool:
+        """Check if a name that's a violation is ignored globally."""
+
+        return path_in_glob_list(".".join(path), self.project_config.allowed_imports)
+
     def is_violation_silenced(self, path: list[str]) -> bool:
         """Check if a name that's a violation is ignored by component config"""
-        allowed_imports: tuple[str, ...] = (
-            getattr(self.component_config, "allowed_imports", None) or ()
+        allowed_imports: frozenset[str] = (
+            getattr(self.component_config, "allowed_imports", None) or frozenset()
         )
 
-        while path:
-            if ".".join(path) in allowed_imports:
-                return True
-            if ".".join(path[:-1]) + ".*" in allowed_imports:
-                return True
-
-            path = path[:-1]
-
-        # Name was not found in the list of allowed imports
-        return False
+        return path_in_glob_list(".".join(path), list(allowed_imports))
 
     def maybe_report_violation(self, full_name: str, node: ast.AST) -> None:
         """Check a fully qualified name"""
 
         path = full_name.split(".")
         if self.is_access_allowed(path):
             return
 
+        if self.is_violation_globally_silenced(path):
+            return
+
         # If access is not allowed we should record the reference even if the
-        # violation is silenced
+        # violation is silenced by the component config.
         self.referenced_imports.add(full_name)
 
         if self.is_violation_silenced(path):
             return
 
         self.report_violation(
             node, Code.ODA005, f'Private attribute "{full_name}" referenced'
```

### Comparing `oida-0.1.5/oida/checkers/config.py` & `oida-0.2.0/oida/checkers/config.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/checkers/imports.py` & `oida-0.2.0/oida/checkers/imports.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/commands/componentize.py` & `oida-0.2.0/oida/commands/componentize.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/commands/config.py` & `oida-0.2.0/oida/commands/config.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/commands/linter.py` & `oida-0.2.0/oida/commands/linter.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/config_generator.py` & `oida-0.2.0/oida/config_generator.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/console.py` & `oida-0.2.0/oida/console.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/discovery.py` & `oida-0.2.0/oida/discovery.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/flake8.py` & `oida-0.2.0/oida/flake8.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/oida/module.py` & `oida-0.2.0/oida/module.py`

 * *Files identical despite different names*

### Comparing `oida-0.1.5/pyproject.toml` & `oida-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oida"
-version = "0.1.5"
+version = "0.2.0"
 description = "Oida is Oda's linter that enforces code style and modularization in our Django projects."
 authors = ["Oda <tech@oda.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/oida"
 repository = "https://github.com/kolonialno/oida"
 classifiers = [
```

### Comparing `oida-0.1.5/PKG-INFO` & `oida-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oida
-Version: 0.1.5
+Version: 0.2.0
 Summary: Oida is Oda's linter that enforces code style and modularization in our Django projects.
 Home-page: https://github.com/kolonialno/oida
 License: MIT
 Author: Oda
 Author-email: tech@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

