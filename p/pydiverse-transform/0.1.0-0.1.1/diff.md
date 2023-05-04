# Comparing `tmp/pydiverse-transform-0.1.0.tar.gz` & `tmp/pydiverse-transform-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse-transform-0.1.0.tar", max compression
+gzip compressed data, was "pydiverse-transform-0.1.1.tar", max compression
```

## Comparing `pydiverse-transform-0.1.0.tar` & `pydiverse-transform-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1517 2022-08-30 10:14:23.006505 pydiverse-transform-0.1.0/LICENSE
--rw-r--r--   0        0        0      701 2022-09-02 13:53:34.518609 pydiverse-transform-0.1.0/README.md
--rw-r--r--   0        0        0     1473 2022-09-03 14:34:51.510018 pydiverse-transform-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       13 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      387 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/__init__.py
--rw-r--r--   0        0        0      108 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/__init__.py
--rw-r--r--   0        0        0     3470 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/alignment.py
--rw-r--r--   0        0        0     2797 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/column.py
--rw-r--r--   0        0        0     5082 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/dispatchers.py
--rw-r--r--   0        0        0      191 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/__init__.py
--rw-r--r--   0        0        0     1078 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/expressions.py
--rw-r--r--   0        0        0      682 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/lambda_getter.py
--rw-r--r--   0        0        0     4871 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/symbolic_expressions.py
--rw-r--r--   0        0        0     4854 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/translator.py
--rw-r--r--   0        0        0     1708 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/util.py
--rw-r--r--   0        0        0      530 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/functions.py
--rw-r--r--   0        0        0      135 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/__init__.py
--rw-r--r--   0        0        0      903 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/aggregate.py
--rw-r--r--   0        0        0     3590 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/core.py
--rw-r--r--   0        0        0     1694 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/logical.py
--rw-r--r--   0        0        0     2341 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/numeric.py
--rw-r--r--   0        0        0    17847 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/registry.py
--rw-r--r--   0        0        0      518 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/string.py
--rw-r--r--   0        0        0      334 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/window.py
--rw-r--r--   0        0        0     3806 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/table.py
--rw-r--r--   0        0        0    16509 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/table_impl.py
--rw-r--r--   0        0        0       84 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/util/__init__.py
--rw-r--r--   0        0        0     2605 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/util/bidict.py
--rw-r--r--   0        0        0     1134 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/util/ordered_set.py
--rw-r--r--   0        0        0     1892 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/util/util.py
--rw-r--r--   0        0        0    14626 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/core/verbs.py
--rw-r--r--   0        0        0       42 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/eager/__init__.py
--rw-r--r--   0        0        0      265 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/eager/eager_table.py
--rw-r--r--   0        0        0    21007 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/eager/pandas_table.py
--rw-r--r--   0        0        0       36 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/lazy/__init__.py
--rw-r--r--   0        0        0      454 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/lazy/lazy_table.py
--rw-r--r--   0        0        0    26358 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/lazy/sql_table.py
--rw-r--r--   0        0        0        0 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/util/__init__.py
--rw-r--r--   0        0        0      730 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.0/src/pydiverse/transform/util/testing.py
--rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 pydiverse-transform-0.1.0/setup.py
--rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 pydiverse-transform-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2022-08-30 10:14:23.006505 pydiverse-transform-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2325 2023-05-04 15:21:08.375883 pydiverse-transform-0.1.1/docs/package/README.md
+-rw-r--r--   0        0        0     1806 2023-05-04 15:21:54.335822 pydiverse-transform-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       13 2022-09-15 12:24:32.275027 pydiverse-transform-0.1.1/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      387 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/__init__.py
+-rw-r--r--   0        0        0      108 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/__init__.py
+-rw-r--r--   0        0        0     3470 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/alignment.py
+-rw-r--r--   0        0        0     2797 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/column.py
+-rw-r--r--   0        0        0     5082 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/dispatchers.py
+-rw-r--r--   0        0        0      191 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/__init__.py
+-rw-r--r--   0        0        0     1078 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/expressions.py
+-rw-r--r--   0        0        0      682 2022-09-15 12:24:32.275027 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/lambda_getter.py
+-rw-r--r--   0        0        0     4871 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/symbolic_expressions.py
+-rw-r--r--   0        0        0     4881 2023-05-04 13:58:19.766398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/translator.py
+-rw-r--r--   0        0        0     1708 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/util.py
+-rw-r--r--   0        0        0      530 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/functions.py
+-rw-r--r--   0        0        0      135 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/__init__.py
+-rw-r--r--   0        0        0      903 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/aggregate.py
+-rw-r--r--   0        0        0     3590 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/core.py
+-rw-r--r--   0        0        0     1694 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/logical.py
+-rw-r--r--   0        0        0     2341 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/numeric.py
+-rw-r--r--   0        0        0    17847 2022-09-15 12:24:32.275027 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/registry.py
+-rw-r--r--   0        0        0      518 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/string.py
+-rw-r--r--   0        0        0      334 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/window.py
+-rw-r--r--   0        0        0     3833 2023-05-04 13:58:19.758398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/table.py
+-rw-r--r--   0        0        0    16536 2023-05-04 13:58:19.802398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/table_impl.py
+-rw-r--r--   0        0        0       84 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/__init__.py
+-rw-r--r--   0        0        0     2637 2023-05-04 13:58:24.130390 pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/bidict.py
+-rw-r--r--   0        0        0     1161 2023-05-04 13:58:19.750398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/ordered_set.py
+-rw-r--r--   0        0        0     1892 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/util.py
+-rw-r--r--   0        0        0    14653 2023-05-04 13:58:19.790398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/verbs.py
+-rw-r--r--   0        0        0       42 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/eager/__init__.py
+-rw-r--r--   0        0        0      265 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/eager/eager_table.py
+-rw-r--r--   0        0        0    21007 2022-09-15 12:24:32.279027 pydiverse-transform-0.1.1/src/pydiverse/transform/eager/pandas_table.py
+-rw-r--r--   0        0        0       36 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/lazy/__init__.py
+-rw-r--r--   0        0        0      454 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/lazy/lazy_table.py
+-rw-r--r--   0        0        0    26997 2023-05-04 14:24:43.368130 pydiverse-transform-0.1.1/src/pydiverse/transform/lazy/sql_table.py
+-rw-r--r--   0        0        0        0 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/util/__init__.py
+-rw-r--r--   0        0        0      730 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/util/testing.py
+-rw-r--r--   0        0        0     3600 2023-05-04 15:24:47.800589 pydiverse-transform-0.1.1/setup.py
+-rw-r--r--   0        0        0     3322 2023-05-04 15:24:47.800854 pydiverse-transform-0.1.1/PKG-INFO
```

### Comparing `pydiverse-transform-0.1.0/LICENSE` & `pydiverse-transform-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/pyproject.toml` & `pydiverse-transform-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 [tool.poetry]
 name = "pydiverse-transform"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pipe based dataframe manipulation library that can also transform data on SQL databases"
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
+  "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
-readme = "README.md"
+readme = "docs/package/README.md"
 packages = [
 	{ include = "pydiverse", from = "src" }
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "Programming Language :: SQL",
   "Topic :: Database",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-numpy = "^1.23.1"
-pandas = "^1.4.3"
-SQLAlchemy = "^1.4.39"
+python = ">=3.9,<3.12"
+numpy = ">=1.23.1"
+pandas = ">=1.4.3"
+SQLAlchemy = ">=1.4.27"
 
 Sphinx = { version = "^5.1.1", optional = true }
 sphinx-rtd-theme = { version = "^1.0.0", optional = true }
 sphinxcontrib-apidoc = { version="^0.3.0", optional = true }
+# bigquery currently does not support sqlalchemy 2.0
+#sqlalchemy-bigquery = { version=">=1.4.4", optional = true }
+#google-auth = { version=">=2.9.1", optional = true }
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-apidoc"]
+#bigquery = ["sqlalchemy-bigquery", "google-auth"]
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pytest-xdist = "^2.5.0"
-black = "^22.6.0"
-pre-commit = "^2.20.0"
+pytest = ">=7.1.2"
+pytest-xdist = ">=2.5.0"
+psycopg2 = ">=2.9.3"
+black = "^23.3.0"
 isort = "^5.10.1"
+pre-commit = ">=2.20.0"
+pyodbc = ">=4.0.34"
 
 [tool.black]
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.venv
```

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/alignment.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/alignment.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/column.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/column.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/dispatchers.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/dispatchers.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/expressions.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/expressions.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/lambda_getter.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/lambda_getter.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/symbolic_expressions.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/symbolic_expressions.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/translator.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Generic, Iterable, TypeVar
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
+from collections.abc import Iterable
 
 from pydiverse.transform.core import column
 from pydiverse.transform.core.expressions import expressions
 from pydiverse.transform.core.ops import Operator, OPType, registry
 
 if TYPE_CHECKING:
     # noinspection PyUnresolvedReferences
```

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/expressions/util.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/util.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/functions.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/functions.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/aggregate.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/aggregate.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/core.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/core.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/logical.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/logical.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/numeric.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/numeric.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/registry.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/registry.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/ops/string.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/string.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/table.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from html import escape
-from typing import Generic, Iterable, TypeVar
+from typing import Generic, TypeVar
+from collections.abc import Iterable
 
 from pydiverse.transform.core import verbs
 from pydiverse.transform.core.column import Column, LambdaColumn
 from pydiverse.transform.core.expressions import SymbolicExpression
 from pydiverse.transform.core.table_impl import AbstractTableImpl
 
 ImplT = TypeVar("ImplT", bound=AbstractTableImpl)
```

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/table_impl.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/table_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import copy
 import dataclasses
 import uuid
 import warnings
-from typing import TYPE_CHECKING, Any, Callable, Generic, Iterable, TypeVar
+from typing import TYPE_CHECKING, Any, Callable, Generic, TypeVar
+from collections.abc import Iterable
 
 from pydiverse.transform.core.ops.registry import (
     OperatorRegistrationContextManager,
     OperatorRegistry,
 )
 from pydiverse.transform.core.util import bidict, ordered_set
```

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/util/bidict.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/bidict.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from typing import (
     Generic,
+    TypeVar,
+)
+from collections.abc import (
     ItemsView,
     Iterable,
     KeysView,
     Mapping,
     MutableMapping,
-    TypeVar,
     ValuesView,
 )
 
 KT = TypeVar("KT")
 VT = TypeVar("VT")
```

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/util/ordered_set.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/ordered_set.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import Iterable, MutableSet, TypeVar
+from typing import TypeVar
+from collections.abc import Iterable, MutableSet
 
 T = TypeVar("T")
 
 
 class ordered_set(MutableSet[T]):
     def __init__(self, values: Iterable[T] = tuple()):
         self.__data = {v: None for v in values}
```

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/util/util.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/util.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/core/verbs.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/core/verbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import functools
 from collections import ChainMap
-from typing import Dict, Iterable
+from typing import Dict
+from collections.abc import Iterable
 
 from .column import Column, LambdaColumn, generate_col_uuid
 from .dispatchers import builtin_verb
 from .expressions import SymbolicExpression
 from .expressions.util import iterate_over_expr
 from .table_impl import AbstractTableImpl, ColumnMetaData
 from .util import bidict, ordered_set, sign_peeler, translate_ordering
```

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/eager/pandas_table.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/eager/pandas_table.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/lazy/sql_table.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/lazy/sql_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
             share the same alignment hash unless they were derived from the
             same table(s) and are guaranteed to have the same number of columns
             in the same order. In other words: Two tables MUST only have the
             same alignment hash if a literal column derived from one of them
             can be used by the other table and produces the same result.
     """
 
-    def __init__(self, engine, table, _dtype_hints: dict[str, str] = None):
+    def __init__(
+        self, engine, table, dataset=None, _dtype_hints: dict[str, str] = None
+    ):
         self.engine = (
             sqlalchemy.create_engine(engine) if isinstance(engine, str) else engine
         )
         tbl = self._create_table(table, self.engine)
         # backend = self.engine.url.get_backend_name()
 
         columns = {
@@ -52,15 +54,22 @@
                 table=self,
                 dtype=self._get_dtype(col, hints=_dtype_hints),
             )
             for col in tbl.columns
         }
 
         self.replace_tbl(tbl, columns)
-        super().__init__(name=self.tbl.name, columns=columns)
+
+        name = self.tbl.name
+        if engine.dialect.name == "bigquery":
+            spl = self.tbl.name.split(".")
+            if len(spl) == 2:
+                name = spl[1]
+
+        super().__init__(name=name, columns=columns)
 
     def is_aligned_with(self, col: Column | LiteralColumn) -> bool:
         if isinstance(col, Column):
             if not isinstance(col.table, type(self)):
                 return False
             return col.table.alignment_hash == self.alignment_hash
 
@@ -90,28 +99,30 @@
             return tbl
 
         if not isinstance(tbl, str):
             raise ValueError(
                 "tbl must be a sqlalchemy Table or string, but was %s" % type(tbl)
             )
 
-        schema, table_name = tbl.split(".") if "." in tbl else [None, tbl]
+        spl = tbl.split(".") if "." in tbl else [None, tbl]
+        schema = spl[0]
+        table_name = ".".join(spl[1:])
 
         # TODO: pybigquery uses schema to mean project_id, so we cannot use
         #     siuba's classic breakdown "{schema}.{table_name}". Basically
         #     pybigquery uses "{schema=project_id}.{dataset_dot_table_name}" in its internal
         #     logic. An important side effect is that bigquery errors for
         #     `dataset`.`table`, but not `dataset.table`.
         if engine and engine.dialect.name == "bigquery":
             table_name = tbl
             schema = None
 
         return sqlalchemy.Table(
             table_name,
-            sqlalchemy.MetaData(bind=engine),
+            sqlalchemy.MetaData(),
             schema=schema,
             autoload_with=engine,
         )
 
     @staticmethod
     def _get_dtype(col: sqlalchemy.Column, hints: dict[str, str] = None) -> str:
         """Determine the dtype of a column.
@@ -232,15 +243,19 @@
         # Convert self.selects to SQLAlchemy Expressions
         s = []
         for name, uuid in self.selected_cols():
             sql_col = self.cols[uuid].compiled(self.sql_columns)
             if not isinstance(sql_col, sql.ColumnElement):
                 sql_col = sql.literal(sql_col)
             s.append(sql_col.label(name))
-        select = select.with_only_columns(s)
+        try:
+            select = select.with_only_columns(s)
+        except sqlalchemy.exc.ArgumentError:
+            # since sqlalchemy 2.0.0
+            select = select.with_only_columns(*s)
 
         # ORDER BY
         if self.order_bys:
             o = []
             for o_by in self.order_bys:
                 compiled, _ = self.compiler.translate(o_by.order)
                 col = compiled(self.sql_columns)
@@ -333,24 +348,30 @@
             name: self.cols[self.named_cols.fwd[name]].dtype for name in self.selects
         }
         return self.__class__(self.engine, subquery, _dtype_hints=dtype_hints)
 
     def collect(self):
         select = self.build_select()
         with self.engine.connect() as conn:
-            # Temporary fix for pandas bug (https://github.com/pandas-dev/pandas/issues/35484)
-            # Taken from siuba
-            from pandas.io import sql as _pd_sql
-
-            class _FixedSqlDatabase(_pd_sql.SQLDatabase):
-                def execute(self, *args, **kwargs):
-                    return self.connectable.execute(*args, **kwargs)
+            try:
+                # TODO: check for which pandas versions this is needed:
+                # Temporary fix for pandas bug (https://github.com/pandas-dev/pandas/issues/35484)
+                # Taken from siuba
+                from pandas.io import sql as _pd_sql
+
+                class _FixedSqlDatabase(_pd_sql.SQLDatabase):
+                    def execute(self, *args, **kwargs):
+                        return self.connectable.execute(*args, **kwargs)
+
+                sql_db = _FixedSqlDatabase(conn)
+                result = sql_db.read_sql(select).convert_dtypes()
+            except AttributeError:
+                import pandas as pd
 
-            sql_db = _FixedSqlDatabase(conn)
-            result = sql_db.read_sql(select).convert_dtypes()
+                result = pd.read_sql_query(select, con=conn)
 
         # Add metadata
         result.attrs["name"] = self.name
         return result
 
     def build_query(self) -> str:
         query = self.build_select()
@@ -445,15 +466,15 @@
 
     #### EXPRESSIONS ####
 
     class ExpressionCompiler(
         LazyTableImpl.ExpressionCompiler[
             "SQLTableImpl",
             TypedValue[
-                Callable[[Dict[uuid.UUID, sqlalchemy.Column]], sql.ColumnElement]
+                Callable[[dict[uuid.UUID, sqlalchemy.Column]], sql.ColumnElement]
             ],
         ]
     ):
         def _translate_col(self, expr, **kwargs):
             # Can either be a base SQL column, or a reference to an expression
             if expr.uuid in self.backend.sql_columns:
```

### Comparing `pydiverse-transform-0.1.0/src/pydiverse/transform/util/testing.py` & `pydiverse-transform-0.1.1/src/pydiverse/transform/util/testing.py`

 * *Files identical despite different names*

