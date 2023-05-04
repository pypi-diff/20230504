# Comparing `tmp/hagis-0.5.1.tar.gz` & `tmp/hagis-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.5.1.tar", last modified: Thu May  4 16:32:00 2023, max compression
+gzip compressed data, was "hagis-0.5.2.tar", last modified: Thu May  4 17:45:11 2023, max compression
```

## Comparing `hagis-0.5.1.tar` & `hagis-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:32:00.210054 hagis-0.5.1/
--rw-rw-rw-   0        0        0      923 2023-05-04 16:32:00.208933 hagis-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 16:32:00.206928 hagis-0.5.1/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-04 16:32:00.000000 hagis-0.5.1/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-04 16:32:00.000000 hagis-0.5.1/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:32:00.000000 hagis-0.5.1/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-04 16:32:00.000000 hagis-0.5.1/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    20415 2023-05-04 16:30:32.000000 hagis-0.5.1/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-04 16:31:31.000000 hagis-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 16:32:00.210577 hagis-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 17:45:11.918082 hagis-0.5.2/
+-rw-rw-rw-   0        0        0      923 2023-05-04 17:45:11.916170 hagis-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 17:45:11.912626 hagis-0.5.2/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-04 17:45:11.000000 hagis-0.5.2/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-04 17:45:11.000000 hagis-0.5.2/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 17:45:11.000000 hagis-0.5.2/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-04 17:45:11.000000 hagis-0.5.2/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21207 2023-05-04 17:43:31.000000 hagis-0.5.2/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-04 17:44:08.000000 hagis-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 17:45:11.919524 hagis-0.5.2/setup.cfg
```

### Comparing `hagis-0.5.1/PKG-INFO` & `hagis-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.1
+Version: 0.5.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.1/hagis.egg-info/PKG-INFO` & `hagis-0.5.2/hagis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.1
+Version: 0.5.2
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.1/hagis.py` & `hagis-0.5.2/hagis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ A high availability GIS client. """
 import ast
-from _ast import Attribute, BoolOp, Call, Compare, Constant
+from _ast import Attribute, BoolOp, Call, Compare, Constant, Name
 from concurrent import futures
 from datetime import datetime
 from hashlib import md5
 from inspect import getsource, signature
 from itertools import chain, islice
 from json import dumps, loads
 from time import time
@@ -366,80 +366,93 @@
                 for rows in executor.map(get_more_rows, remaining_batches):
                     for row in rows:
                         yield self._map(row)
 
     def _to_sql(self, predicate: Callable[[T], bool]) -> str:
 
         class LambdaFinder(ast.NodeVisitor):
-
-            expression: ast.Lambda
-
-            def __init__(self, code: str) -> None:
+            def __init__(self, expression: Any) -> None:
                 super().__init__()
-                line = code.strip()
+                closure = expression.__closure__
+                if closure:
+                    self.freevars = dict(zip(expression.__code__.co_freevars, [x.cell_contents for x in closure]))
+                else:
+                    self.freevars = {}
+                line = getsource(expression).strip()
                 self.visit(ast.parse(f"{line}\n    pass" if line.endswith(":") else line))
 
             def visit_Lambda(self, node: ast.Lambda) -> Any:  # pylint: disable-all
                 self.expression = node
 
             @staticmethod
             def find(expression: Any):  # pylint: disable-all
-                return LambdaFinder(getsource(expression)).expression
+                visitor = LambdaFinder(expression)
+                return visitor.expression, visitor.freevars
 
         class LambdaVisitor(ast.NodeVisitor):
 
-            def __init__(self, expression: ast.expr, fields: Dict[str, str]):
+            def __init__(self, expression: ast.expr, freevars: Dict[str, Any], fields: Dict[str, str]):
                 super().__init__()
                 self._expressions: List[Union[LambdaVisitor, str]] = []
+                self._freevars = freevars
                 self._fields = fields
                 self.visit(expression)
 
             def visit_Attribute(self, node: Attribute) -> Any:
                 field_name = self._fields[node.attr]
                 self._expressions.append(field_name)
 
             def visit_BoolOp(self, node: BoolOp) -> Any:
                 self._expressions.append("(")
                 expressions: List[Union[LambdaVisitor, str]] = []
                 for value in node.values:
-                    expressions.append(LambdaVisitor(value, self._fields))
+                    expressions.append(LambdaVisitor(value, self._freevars, self._fields))
                     expressions.append(self._convert_op(node.op))
                 expressions.pop()
                 self._expressions.extend(expressions)
                 self._expressions.append(")")
 
             def visit_Call(self, node: Call) -> Any:
                 if not hasattr(node.func, "attr"):
                     self.generic_visit(node)
                     return
                 attr = node.func.attr  # type: ignore
                 if attr == "startswith":
                     field_name = self._fields[node.func.value.attr]  # type: ignore
-                    self._expressions.append(f"{field_name} LIKE '{node.args[0].value}%'")  # type: ignore
+                    self._expressions.append(f"{field_name} LIKE '{self._get_value(node.args[0])}%'")
                 elif attr == "endswith":
                     field_name = self._fields[node.func.value.attr]  # type: ignore
-                    self._expressions.append(f"{field_name} LIKE '%{node.args[0].value}'")  # type: ignore
+                    self._expressions.append(f"{field_name} LIKE '%{self._get_value(node.args[0])}'")
 
             def visit_Compare(self, node: Compare) -> Any:
                 op = node.ops[0]
                 if isinstance(op, ast.In):
                     field_name = self._fields[node.comparators[0].attr]  # type: ignore
-                    self._expressions.append(f"{field_name} LIKE '%{node.left.value}%'")  # type: ignore
+                    self._expressions.append(f"{field_name} LIKE '%{self._get_value(node.left)}%'")
                 else:
-                    self._expressions.append(LambdaVisitor(node.left, self._fields))
+                    self._expressions.append(LambdaVisitor(node.left, self._freevars, self._fields))
                     self._expressions.append(self._convert_op(node.ops[0]))
-                    self._expressions.append(LambdaVisitor(node.comparators[0], self._fields))
+                    self._expressions.append(LambdaVisitor(node.comparators[0], self._freevars, self._fields))
 
             def visit_Constant(self, node: Constant) -> Any:
-                if node.value is None:
-                    self._expressions.append("NULL")
-                elif isinstance(node.value, str):
-                    self._expressions.append(f"'{node.value}'")
-                else:
-                    self._expressions.append(node.value)
+                self._expressions.append(self._get_sql_value(node))
+
+            def visit_Name(self, node: Name) -> Any:
+                self._expressions.append(self._get_sql_value(node))
+
+            def _get_sql_value(self, node: Any) -> str:
+                value = self._get_value(node)
+                if value is None:
+                    return "NULL"
+                if isinstance(value, str):
+                    return f"'{value}'"
+                return str(value)
+
+            def _get_value(self, node: Any) -> Any:
+                return self._freevars[node.id] if isinstance(node, Name) else node.value
 
             def _convert_op(self, op: Any) -> str:
                 if isinstance(op, ast.And):
                     return "AND"
                 if isinstance(op, ast.Or):
                     return "OR"
                 if isinstance(op, ast.Is):
@@ -462,15 +475,18 @@
 
             def to_sql(self) -> str:
                 text = ""
                 for e in self._expressions:
                     text += e.to_sql() if isinstance(e, LambdaVisitor) else f" {e}"
                 return text
 
-        where_clause = LambdaVisitor(LambdaFinder.find(predicate), self._fields).to_sql().strip()
+        expression, freevars = LambdaFinder.find(predicate)
+
+        where_clause = LambdaVisitor(expression, freevars, self._fields).to_sql().strip()
+
         return where_clause
 
 
 class Point:  # pylint: disable=too-few-public-methods
     """ Point class.
     """
     x: float
```

### Comparing `hagis-0.5.1/pyproject.toml` & `hagis-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

