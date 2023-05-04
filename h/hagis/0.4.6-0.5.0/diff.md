# Comparing `tmp/hagis-0.4.6.tar.gz` & `tmp/hagis-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.4.6.tar", last modified: Sun Apr 30 17:54:31 2023, max compression
+gzip compressed data, was "hagis-0.5.0.tar", last modified: Thu May  4 16:05:52 2023, max compression
```

## Comparing `hagis-0.4.6.tar` & `hagis-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 17:54:31.293007 hagis-0.4.6/
--rw-rw-rw-   0        0        0      923 2023-04-30 17:54:31.293007 hagis-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 17:54:31.277005 hagis-0.4.6/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-30 17:54:31.000000 hagis-0.4.6/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-04-30 17:54:31.000000 hagis-0.4.6/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 17:54:31.000000 hagis-0.4.6/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-30 17:54:31.000000 hagis-0.4.6/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15263 2023-04-30 17:52:36.000000 hagis-0.4.6/hagis.py
--rw-rw-rw-   0        0        0      589 2023-04-30 17:53:24.000000 hagis-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 17:54:31.293007 hagis-0.4.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 16:05:52.932939 hagis-0.5.0/
+-rw-rw-rw-   0        0        0      923 2023-05-04 16:05:52.932438 hagis-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 16:05:52.929801 hagis-0.5.0/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-04 16:05:52.000000 hagis-0.5.0/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-04 16:05:52.000000 hagis-0.5.0/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:05:52.000000 hagis-0.5.0/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-04 16:05:52.000000 hagis-0.5.0/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    20384 2023-05-04 15:56:16.000000 hagis-0.5.0/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-04 16:02:56.000000 hagis-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:05:52.933935 hagis-0.5.0/setup.cfg
```

### Comparing `hagis-0.4.6/PKG-INFO` & `hagis-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.4.6
+Version: 0.5.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.4.6/hagis.egg-info/PKG-INFO` & `hagis-0.5.0/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.4.6
+Version: 0.5.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.4.6/hagis.py` & `hagis-0.5.0/hagis.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """ A high availability GIS client. """
+import ast
+from _ast import Attribute, BoolOp, Call, Compare, Constant
 from concurrent import futures
 from datetime import datetime
 from hashlib import md5
-from inspect import signature
+from inspect import getsource, signature
 from itertools import chain, islice
 from json import dumps, loads
 from time import time
 from types import SimpleNamespace
 from typing import Any, Callable, Dict, Generic, Iterator, List, Optional, Tuple, Type, TypeVar, Union
 from uuid import UUID
 from requests import post
@@ -114,29 +116,31 @@
         """ Sets the static token.
 
         Args:
             token (str): Token.
         """
         self._generate_token = lambda: token
 
-    def query(self, where_clause: Optional[str] = None, record_count: Optional[int] = None,
+    def query(self, where_clause: Union[str, Callable[[T], bool], None] = None, record_count: Optional[int] = None,
               wkid: Optional[int] = None, max_workers: Optional[int] = None, **kwargs: Any) -> Iterator[T]:
         """ Executes a query.
 
         Args:
             where_clause (str, optional): Where clause.  Defaults to None.
             record_count (Optional[int], optional): Maximum record count.  Defaults to None.
             wkid (Optional[int], optional): Spatial reference.  Defaults to None.
             max_workers (Optional[int], optional): Max worker count (degree of parallelism). Defaults to None.
 
         Yields:
             Iterator[T]: Items.
         """
         if not where_clause:
             where_clause = "1=1"
+        elif isinstance(where_clause, Callable):
+            where_clause = self._to_sql(where_clause)
 
         if record_count == 0:
             return
 
         if self._is_dynamic:
             # If dynamic, request all fields.
             fields = "*"
@@ -163,25 +167,27 @@
                         setattr(item, property_name, property_value)
                 else:
                     # Support for data classes and named tuples.
                     item = self._model(*dictionary.values())
 
                 yield item
 
-    def count(self, where_clause: Optional[str] = None) -> int:
+    def count(self, where_clause: Union[str, Callable[[T], bool], None] = None) -> int:
         """ Checks the number of items that match the where clause.
 
         Args:
             where_clause (str, optional): Where clause.  Defaults to None.
 
         Returns:
             int: Count.
         """
         if not where_clause:
             where_clause = "1=1"
+        elif isinstance(where_clause, Callable):
+            where_clause = self._to_sql(where_clause)
 
         obj = self._call("query", where=where_clause, returnCountOnly=True)
         return obj.count
 
     def find(self, oid: int, **kwargs: Any) -> Optional[T]:
         """ Finds the item by Object ID.
 
@@ -230,20 +236,26 @@
         """ Updates existing items on the remote server.
 
         Args:
             items (List[T]): Items to update.
         """
         self.apply_edits(updates=items, **kwargs)
 
-    def delete(self, where_clause: str, **kwargs: Any) -> None:
+    def delete(self, where_clause: Union[str, Callable[[T], bool]], **kwargs: Any) -> None:
         """ Deletes items based on a where clause.
 
         Args:
             where_clause (str): Where clause use for deleting.
         """
+        if not where_clause:
+            raise ValueError("Where clause is required for the delete operation.")
+
+        if isinstance(where_clause, Callable):
+            where_clause = self._to_sql(where_clause)
+
         self._call("deleteFeatures", where=where_clause, **kwargs)
 
     def generate_where_clause(self, *ids: Union[int, str, UUID], id_field: Optional[str] = None) -> str:
         """ Generates a where clause from a list of Object ID, Global ID or some other identifiers.
 
         Args:
             id_field (Optional[str], optional): Name of the ID field. Defaults to None.
@@ -351,14 +363,115 @@
             remaining_batches = [remaining_oids[i: i + size] for i in range(len(remaining_oids))[::size]]
 
             with futures.ThreadPoolExecutor(max_workers) as executor:
                 for rows in executor.map(get_more_rows, remaining_batches):
                     for row in rows:
                         yield self._map(row)
 
+    def _to_sql(self, predicate: Callable[[T], bool]) -> str:
+
+        class LambdaFinder(ast.NodeVisitor):
+
+            expression: ast.Lambda
+
+            def __init__(self, code: str) -> None:
+                super().__init__()
+                self.visit(ast.parse(f"{code}    pass" if code.strip().endswith(":") else code))
+
+            def visit_Lambda(self, node: ast.Lambda) -> Any:  # pylint: disable-all
+                self.expression = node
+
+            @staticmethod
+            def find(expression: Any):  # pylint: disable-all
+                return LambdaFinder(getsource(expression)).expression
+
+        class LambdaVisitor(ast.NodeVisitor):
+
+            def __init__(self, expression: ast.expr, fields: Dict[str, str]):
+                super().__init__()
+                self._expressions: List[Union[LambdaVisitor, str]] = []
+                self._fields = fields
+                self.visit(expression)
+
+            def visit_Attribute(self, node: Attribute) -> Any:
+                field_name = self._fields[node.attr]
+                self._expressions.append(field_name)
+
+            def visit_BoolOp(self, node: BoolOp) -> Any:
+                self._expressions.append("(")
+                expressions: List[Union[LambdaVisitor, str]] = []
+                for value in node.values:
+                    expressions.append(LambdaVisitor(value, self._fields))
+                    expressions.append(self._convert_op(node.op))
+                expressions.pop()
+                self._expressions.extend(expressions)
+                self._expressions.append(")")
+
+            def visit_Call(self, node: Call) -> Any:
+                if not hasattr(node.func, "attr"):
+                    self.generic_visit(node)
+                    return
+                attr = node.func.attr  # type: ignore
+                if attr == "startswith":
+                    field_name = self._fields[node.func.value.attr]  # type: ignore
+                    self._expressions.append(f"{field_name} LIKE '{node.args[0].value}%'")  # type: ignore
+                elif attr == "endswith":
+                    field_name = self._fields[node.func.value.attr]  # type: ignore
+                    self._expressions.append(f"{field_name} LIKE '%{node.args[0].value}'")  # type: ignore
+
+            def visit_Compare(self, node: Compare) -> Any:
+                op = node.ops[0]
+                if isinstance(op, ast.In):
+                    field_name = self._fields[node.comparators[0].attr]  # type: ignore
+                    self._expressions.append(f"{field_name} LIKE '%{node.left.value}%'")  # type: ignore
+                else:
+                    self._expressions.append(LambdaVisitor(node.left, self._fields))
+                    self._expressions.append(self._convert_op(node.ops[0]))
+                    self._expressions.append(LambdaVisitor(node.comparators[0], self._fields))
+
+            def visit_Constant(self, node: Constant) -> Any:
+                if node.value is None:
+                    self._expressions.append("NULL")
+                elif isinstance(node.value, str):
+                    self._expressions.append(f"'{node.value}'")
+                else:
+                    self._expressions.append(node.value)
+
+            def _convert_op(self, op: Any) -> str:
+                if isinstance(op, ast.And):
+                    return "AND"
+                if isinstance(op, ast.Or):
+                    return "OR"
+                if isinstance(op, ast.Is):
+                    return "IS"
+                if isinstance(op, ast.IsNot):
+                    return "IS NOT"
+                if isinstance(op, ast.Eq):
+                    return "="
+                if isinstance(op, ast.NotEq):
+                    return "<>"
+                if isinstance(op, ast.Gt):
+                    return ">"
+                if isinstance(op, ast.GtE):
+                    return ">="
+                if isinstance(op, ast.Lt):
+                    return "<"
+                if isinstance(op, ast.LtE):
+                    return "<="
+                return type(op).__name__
+
+            def to_sql(self) -> str:
+                text = ""
+                for e in self._expressions:
+                    text += e.to_sql() if isinstance(e, LambdaVisitor) else f" {e}"
+                return text
+
+        where_clause = LambdaVisitor(LambdaFinder.find(predicate), self._fields).to_sql().strip()
+        return where_clause
+
 
 class Point:  # pylint: disable=too-few-public-methods
     """ Point class.
     """
     x: float
     y: float
```

### Comparing `hagis-0.4.6/pyproject.toml` & `hagis-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.4.6"
+version = "0.5.0"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

