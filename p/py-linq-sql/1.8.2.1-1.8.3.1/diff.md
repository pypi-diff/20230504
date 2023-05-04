# Comparing `tmp/py_linq_sql-1.8.2.1.tar.gz` & `tmp/py_linq_sql-1.8.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_linq_sql-1.8.2.1.tar", max compression
+gzip compressed data, was "py_linq_sql-1.8.3.1.tar", max compression
```

## Comparing `py_linq_sql-1.8.2.1.tar` & `py_linq_sql-1.8.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    13863 2023-02-09 11:20:10.641920 py_linq_sql-1.8.2.1/LICENSE.md
--rw-r--r--   0        0        0    13621 2023-03-27 09:48:59.357368 py_linq_sql-1.8.2.1/README.md
--rw-r--r--   0        0        0     2180 2023-03-28 19:41:49.934189 py_linq_sql-1.8.2.1/py_linq_sql/__init__.py
--rw-r--r--   0        0        0       58 2023-02-09 11:20:10.661920 py_linq_sql-1.8.2.1/py_linq_sql/build_request/__init__.py
--rw-r--r--   0        0        0     8599 2023-02-09 11:20:10.661920 py_linq_sql-1.8.2.1/py_linq_sql/build_request/alter.py
--rw-r--r--   0        0        0     7090 2023-02-09 11:20:10.661920 py_linq_sql-1.8.2.1/py_linq_sql/build_request/build.py
--rw-r--r--   0        0        0    18390 2023-03-28 19:41:49.934189 py_linq_sql-1.8.2.1/py_linq_sql/build_request/consult.py
--rw-r--r--   0        0        0     3042 2023-02-09 11:20:10.661920 py_linq_sql-1.8.2.1/py_linq_sql/build_request/consult_aggregate.py
--rw-r--r--   0        0        0     6607 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/build_request/consult_context.py
--rw-r--r--   0        0        0     4581 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/build_request/consult_terminal.py
--rw-r--r--   0        0        0     3399 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/build_request/one.py
--rw-r--r--   0        0        0       60 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/config/__init__.py
--rw-r--r--   0        0        0     5292 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/config/config.py
--rw-r--r--   0        0        0       50 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/exception/__init__.py
--rw-r--r--   0        0        0    12084 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/exception/exception.py
--rw-r--r--   0        0        0        0 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/py.typed
--rw-r--r--   0        0        0       88 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/sql_enumerable/__init__.py
--rw-r--r--   0        0        0    55500 2023-02-15 10:32:33.463229 py_linq_sql-1.8.2.1/py_linq_sql/sql_enumerable/sql_enumerable.py
--rw-r--r--   0        0        0       56 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/__init__.py
--rw-r--r--   0        0        0       31 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/classes/__init__.py
--rw-r--r--   0        0        0     2497 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/classes/enum.py
--rw-r--r--   0        0        0    33396 2023-03-28 19:41:49.938189 py_linq_sql-1.8.2.1/py_linq_sql/utils/classes/magicdotpath.py
--rw-r--r--   0        0        0    13358 2023-02-15 10:32:33.463229 py_linq_sql-1.8.2.1/py_linq_sql/utils/classes/op_and_func_of_mdp.py
--rw-r--r--   0        0        0     4293 2023-02-09 14:30:57.412659 py_linq_sql-1.8.2.1/py_linq_sql/utils/classes/other_classes.py
--rw-r--r--   0        0        0     1560 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/db.py
--rw-r--r--   0        0        0    11053 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/execute.py
--rw-r--r--   0        0        0       33 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/__init__.py
--rw-r--r--   0        0        0     3699 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/aggregate_functions.py
--rw-r--r--   0        0        0     3286 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/join_functions.py
--rw-r--r--   0        0        0     3147 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_hyperb_functions.py
--rw-r--r--   0        0        0    11744 2023-02-15 10:32:33.463229 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_maths_functions.py
--rw-r--r--   0        0        0      843 2023-03-27 09:48:24.429142 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_other_functions.py
--rw-r--r--   0        0        0     1810 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_str_functions.py
--rw-r--r--   0        0        0     8601 2023-02-15 10:32:33.467229 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_trigo_functions.py
--rw-r--r--   0        0        0     7818 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/other_functions.py
--rw-r--r--   0        0        0     6205 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/path_functions.py
--rw-r--r--   0        0        0     2388 2023-02-09 11:20:10.665920 py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/predicate_functions.py
--rw-r--r--   0        0        0     5414 2023-03-28 19:41:49.938189 py_linq_sql-1.8.2.1/pyproject.toml
--rw-r--r--   0        0        0    15090 1970-01-01 00:00:00.000000 py_linq_sql-1.8.2.1/setup.py
--rw-r--r--   0        0        0    14794 1970-01-01 00:00:00.000000 py_linq_sql-1.8.2.1/PKG-INFO
+-rw-r--r--   0        0        0    13863 2023-02-09 11:20:10.641920 py_linq_sql-1.8.3.1/LICENSE.md
+-rw-r--r--   0        0        0    13621 2023-03-30 09:53:07.893915 py_linq_sql-1.8.3.1/README.md
+-rw-r--r--   0        0        0     2180 2023-05-04 08:57:57.458763 py_linq_sql-1.8.3.1/py_linq_sql/__init__.py
+-rw-r--r--   0        0        0       58 2023-02-09 11:20:10.661920 py_linq_sql-1.8.3.1/py_linq_sql/build_request/__init__.py
+-rw-r--r--   0        0        0     8599 2023-02-09 11:20:10.661920 py_linq_sql-1.8.3.1/py_linq_sql/build_request/alter.py
+-rw-r--r--   0        0        0     7090 2023-02-09 11:20:10.661920 py_linq_sql-1.8.3.1/py_linq_sql/build_request/build.py
+-rw-r--r--   0        0        0    18390 2023-03-28 19:41:49.934189 py_linq_sql-1.8.3.1/py_linq_sql/build_request/consult.py
+-rw-r--r--   0        0        0     3042 2023-02-09 11:20:10.661920 py_linq_sql-1.8.3.1/py_linq_sql/build_request/consult_aggregate.py
+-rw-r--r--   0        0        0     6607 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/build_request/consult_context.py
+-rw-r--r--   0        0        0     4581 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/build_request/consult_terminal.py
+-rw-r--r--   0        0        0     3399 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/build_request/one.py
+-rw-r--r--   0        0        0       60 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/config/__init__.py
+-rw-r--r--   0        0        0     5292 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/config/config.py
+-rw-r--r--   0        0        0       50 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/exception/__init__.py
+-rw-r--r--   0        0        0    12084 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/exception/exception.py
+-rw-r--r--   0        0        0        0 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/py.typed
+-rw-r--r--   0        0        0       88 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/sql_enumerable/__init__.py
+-rw-r--r--   0        0        0    55948 2023-03-30 09:52:19.577498 py_linq_sql-1.8.3.1/py_linq_sql/sql_enumerable/sql_enumerable.py
+-rw-r--r--   0        0        0       56 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/__init__.py
+-rw-r--r--   0        0        0       31 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/classes/__init__.py
+-rw-r--r--   0        0        0     2497 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/classes/enum.py
+-rw-r--r--   0        0        0    33396 2023-03-30 09:54:36.094712 py_linq_sql-1.8.3.1/py_linq_sql/utils/classes/magicdotpath.py
+-rw-r--r--   0        0        0    13358 2023-02-15 10:32:33.463229 py_linq_sql-1.8.3.1/py_linq_sql/utils/classes/op_and_func_of_mdp.py
+-rw-r--r--   0        0        0     4293 2023-02-09 14:30:57.412659 py_linq_sql-1.8.3.1/py_linq_sql/utils/classes/other_classes.py
+-rw-r--r--   0        0        0     1560 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/db.py
+-rw-r--r--   0        0        0    11053 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/execute.py
+-rw-r--r--   0        0        0       33 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/__init__.py
+-rw-r--r--   0        0        0     3699 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/aggregate_functions.py
+-rw-r--r--   0        0        0     3286 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/join_functions.py
+-rw-r--r--   0        0        0     3147 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_hyperb_functions.py
+-rw-r--r--   0        0        0    11744 2023-02-15 10:32:33.463229 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_maths_functions.py
+-rw-r--r--   0        0        0      843 2023-03-30 09:52:31.421599 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_other_functions.py
+-rw-r--r--   0        0        0     1810 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_str_functions.py
+-rw-r--r--   0        0        0     8601 2023-02-15 10:32:33.467229 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_trigo_functions.py
+-rw-r--r--   0        0        0     7818 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/other_functions.py
+-rw-r--r--   0        0        0     6205 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/path_functions.py
+-rw-r--r--   0        0        0     2388 2023-02-09 11:20:10.665920 py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/predicate_functions.py
+-rw-r--r--   0        0        0     5414 2023-05-04 08:57:57.458763 py_linq_sql-1.8.3.1/pyproject.toml
+-rw-r--r--   0        0        0    15116 1970-01-01 00:00:00.000000 py_linq_sql-1.8.3.1/setup.py
+-rw-r--r--   0        0        0    14834 1970-01-01 00:00:00.000000 py_linq_sql-1.8.3.1/PKG-INFO
```

### Comparing `py_linq_sql-1.8.2.1/LICENSE.md` & `py_linq_sql-1.8.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/README.md` & `py_linq_sql-1.8.3.1/README.md`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/__init__.py` & `py_linq_sql-1.8.3.1/py_linq_sql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Code of the project py-linq-sql."""
 
-__version__ = "1.8.2-pre-release"
+__version__ = "1.8.3-pre-release"
 
 # Local imports
 
 # Local imports
 from .build_request.consult_aggregate import (  # noqa: F401
     avg,
     concat,
```

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/build_request/alter.py` & `py_linq_sql-1.8.3.1/py_linq_sql/build_request/alter.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/build_request/build.py` & `py_linq_sql-1.8.3.1/py_linq_sql/build_request/build.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/build_request/consult.py` & `py_linq_sql-1.8.3.1/py_linq_sql/build_request/consult.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/build_request/consult_aggregate.py` & `py_linq_sql-1.8.3.1/py_linq_sql/build_request/consult_aggregate.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/build_request/consult_context.py` & `py_linq_sql-1.8.3.1/py_linq_sql/build_request/consult_context.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/build_request/consult_terminal.py` & `py_linq_sql-1.8.3.1/py_linq_sql/build_request/consult_terminal.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/build_request/one.py` & `py_linq_sql-1.8.3.1/py_linq_sql/build_request/one.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/config/config.py` & `py_linq_sql-1.8.3.1/py_linq_sql/config/config.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/exception/exception.py` & `py_linq_sql-1.8.3.1/py_linq_sql/exception/exception.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/sql_enumerable/sql_enumerable.py` & `py_linq_sql-1.8.3.1/py_linq_sql/sql_enumerable/sql_enumerable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1189,14 +1189,19 @@
         inner_key: LambdaMagicDotPath,
         result_function: LambdaMagicDotPathAggregate,
         join_type: JoinType = JoinType.INNER,
     ) -> SQLEnumerable:
         """
         Add a GROUP JOIN command to the command list.
 
+        /!\ For the moment you need to put inner before outer in the lambda
+
+        for example, if inner is satellite in the result function you need to make
+        lambda satellite, objects: stalellite.x.y, objects.a.b
+
         Args:
             inner: SQLEnumerable with which we want to make the join.
             outer_key: Lambda function to get the path(s) parameters
                 for comparison in the outer SQLEnumerable.
             inner_key: Lambda function to get the path(s) parameters
                 for comparison in the inner SQLEnumerable.
             result_function: Lambda function to get the path(s) for the selection.
@@ -1253,14 +1258,19 @@
         inner_key: LambdaMagicDotPath,
         result_function: LambdaMagicDotPath | None = None,
         join_type: JoinType = JoinType.INNER,
     ) -> SQLEnumerable:
         """
         Add a JOIN command to the command list.
 
+        /!\ For the moment you need to put inner before outer in the lambda
+
+        for example, if inner is satellite in the result function you need to make
+        lambda satellite, objects: stalellite.x.y, objects.a.b
+
         Args:
             inner: SQLEnumerable with which we want to make the join.
             outer_key: Lambda function to get the path(s) parameters
                 for comparison in the outer SQLEnumerable.
             inner_key: Lambda function to get the path(s) parameters
                 for comparison in the inner SQLEnumerable.
             result_function: Lambda function to get the path(s) for the selection.
```

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/classes/enum.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/classes/enum.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/classes/magicdotpath.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/classes/magicdotpath.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/classes/op_and_func_of_mdp.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/classes/op_and_func_of_mdp.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/classes/other_classes.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/classes/other_classes.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/db.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/db.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/execute.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/execute.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/aggregate_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/aggregate_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/join_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/join_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_hyperb_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_hyperb_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_maths_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_maths_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_other_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_other_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_str_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_str_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/magic_dp_trigo_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/magic_dp_trigo_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/other_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/other_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/path_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/path_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/py_linq_sql/utils/functions/predicate_functions.py` & `py_linq_sql-1.8.3.1/py_linq_sql/utils/functions/predicate_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.8.2.1/pyproject.toml` & `py_linq_sql-1.8.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-linq-sql"
-version = "1.8.2.1"
+version = "1.8.3.1"
 description = "A Python module used for interacting with sql database using LINQ syntax."
 license = "EUPL v1.2"
 authors = ["CHOSSON Ulysse <ulysse.chosson@obspm.fr>"]
 maintainers = ["CHOSSON Ulysse <ulysse.chosson@obspm.fr>", "MARTIN Pierre-Yves <pierre-yves.martin@obspm.fr>"]
 readme = "README.md"
 repository = "https://gitlab.obspm.fr/exoplanet/py-linq-sql"
 documentation = "https://py-linq-sql.readthedocs.io/en/latest/"
@@ -19,14 +19,15 @@
 dotmap = "^1.3.30"
 psycopg = "^3.1.4"
 toml = "^0.10.2"
 pyyaml = "^6.0"
 types-toml = "^0.10.8"
 types-pyyaml = "^6.0.12.1"
 six = "^1.16.0"
+strenum = "^0.4.8"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.2"
 pytest-sugar = "^0.9.6"
 pytest-pudb = "^0.7.0"
 assertpy = "^1.1"
@@ -48,15 +49,14 @@
 codespell = "^2.2.2"
 dlint = "^0.13.0"
 bandit = "^1.7.4"
 mypy = "^0.991"
 sqlfluff = "^1.4.1"
 pygments = "2.12.0"
 import-linter = "^1.4.0"
-strenum = "^0.4.8"
 ruff = "^0.0.227"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py_linq_sql-1.8.2.1/setup.py` & `py_linq_sql-1.8.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 install_requires = \
 ['dotmap>=1.3.30,<2.0.0',
  'psycopg>=3.1.4,<4.0.0',
  'py-linq>=1.3.0,<2.0.0',
  'pyyaml>=6.0,<7.0',
  'rich>=12.6.0,<13.0.0',
  'six>=1.16.0,<2.0.0',
+ 'strenum>=0.4.8,<0.5.0',
  'toml>=0.10.2,<0.11.0',
  'types-pyyaml>=6.0.12.1,<7.0.0.0',
  'types-toml>=0.10.8,<0.11.0']
 
 setup_kwargs = {
     'name': 'py-linq-sql',
-    'version': '1.8.2.1',
+    'version': '1.8.3.1',
     'description': 'A Python module used for interacting with sql database using LINQ syntax.',
     'long_description': '<!-- markdownlint-disable-file MD024 MD041 -->\n\n![maintenance](https://img.shields.io/maintenance/yes/2023)\n![open issue](https://img.shields.io/gitlab/issues/open-raw/exoplanet/py-linq-sql?gitlab_url=https%3A%2F%2Fgitlab.obspm.fr)\n\n[![pipeline status](https://gitlab.obspm.fr/exoplanet/py-linq-sql/badges/main/pipeline.svg)](https://gitlab.obspm.fr/exoplanet/py-linq-sql/-/commits/main)\n[![coverage report](https://gitlab.obspm.fr/exoplanet/py-linq-sql/badges/main/coverage.svg)](https://gitlab.obspm.fr/exoplanet/py-linq-sql/-/commits/main)\n\n![Banner](https://py-linq-sql.readthedocs.io/en/latest/banner.png)\n\n# Py-Linq-SQL\n\nA Python module used for interacting with sql database using [LINQ](https://docs.microsoft.com/fr-fr/dotnet/api/system.linq.enumerable?view=net-6.0)\nsyntax. The project is under [EUPL License v1.2](LICENSE.md).\n\nPy-linq-sql allows you to go from (SQLAlchemy using direct text query):\n\n```python\nconn.execute(\n  text(\n    """SELECT "data"->\'obj\'->\'name\' as name """\n    """FROM "objects" """\n    """WHERE "data"->\'obj\'->>\'name\' == "earth" """\n    """AND CAST("data"->\'obj\'->\'mass\' > 0.5 AS Decimal) """\n    """LIMIT 1 OFFSET 2"""\n  )\n)\n```\n\nto the safer and easier to read:\n\n```python\nsqle = (\n  SQLEnumerable(conn, "objects")  # objects is the name of the table\n  .select(lambda x: {"name": x.data.obj.name})  # data is a JSONB column\n  .where(lambda x: x.data.obj.mass > 0.5)  # data is a JSONB column\n  .skip(2)\n  .take(1)  # this is the last part of the query, till there nothing is executed\n  .execute()  # now we ask for the whole query to be executed on the DB server\n)\n```\n\nPro :\n\n- all the query expression are expressed in pure python expression\n- easy support of JSON database using a simple object notation\n- very difficult to have an SQL injection (only the names of the tables are strings)\n- standardized syntax/API of LINQ (used in java, C# and many .net languages)\n- very fast: even very long and complex queries are executed in one single query on the\n  server\n- no need to define a class for every table in the DB as you would do in an ORM here you\n  write query assuming the tables, columns and fields exist, if not then you get a clear\n  error about it\n- results are pylinq Enumerable that are themselves queryable in same way but locally\n- all kinds of join (inner, outer and full, with or without intersections) are easy to\n  use and combine with any kind of query\n\nCons :\n\n- currently only support PostgresQL\n\nAny feedback is welcome see [Contributing](CONTRIBUTING.md).\n\n## Contacts\n\n- Author: Ulysse CHOSSON (LESIA)\n- Maintainer: Ulysse CHOSSON (LESIA)\n- Email: <ulysse.chosson@obspm.fr>\n- Contributors:\n  - Pierre-Yves MARTIN (LESIA)\n\n## Table of Content\n\n- [Py-Linq-SQL](#py-linq-sql)\n  - [Contacts](#contacts)\n  - [Table of Content](#table-of-content)\n  - [Install](#install)\n  - [Implemented functions](#implemented-functions)\n    - [LINQ functions](#linq-functions)\n    - [Custom functions](#custom-functions)\n  - [Not implemented functions](#not-implemented-functions)\n    - [LINQ functions](#linq-functions-1)\n    - [Py-Linq functions](#py-linq-functions)\n  - [Contributing and info for developers](#contributing-and-info-for-developers)\n  - [Full documentation](#full-documentation)\n\n## Install\n\nFor all specific commands to this project, we use [just](https://github.com/casey/just).\n**You need to install it.**\n\nAfter you can install the dependencies:\n\n```bash\n$ just install\npwd\n/home/uchosson/Documents/py-linq-sql\npoetry install --no-dev --remove-untracked\nInstalling dependencies from lock file\nWarning: The lock file is not up to date with the latest changes in pyproject.toml.\nYou may be getting outdated dependencies. Run update to update them.\n\nNo dependencies to install or update\n\nInstalling the current project: py-linq-sql (0.109.0)\n```\n\nAnd if you need to develop the project, install development dependencies:\n\n```bash\n$ just install-all\npwd\n/home/uchosson/Documents/py-linq-sql\npoetry install --remove-untracked\nInstalling dependencies from lock file\nWarning: The lock file is not up to date with the latest changes in pyproject.toml.\nYou may be getting outdated dependencies. Run update to update them.\n\nNo dependencies to install or update\n\nInstalling the current project: py-linq-sql (0.109.0)\nnpm install\n\nup to date, audited 8 packages in 793ms\n\n1 package is looking for funding\n  run `npm fund` for details\n\nfound 0 vulnerabilities\nsudo npm install markdownlint-cli2 --global\n\nchanged 36 packages, and audited 37 packages in 2s\n\n8 packages are looking for funding\n  run `npm fund` for details\n\nfound 0 vulnerabilities\n```\n\nand the pre-commit dependencies:\n\n```bash\n$ just preinstall\npwd\n/home/uchosson/Documents/py-linq-sql\npre-commit clean\nCleaned /home/uchosson/.cache/pre-commit.\npre-commit autoupdate\nUpdating https://github.com/pre-commit/pre-commit-hooks ...\n[INFO] Initializing environment for https://github.com/pre-commit/pre-commit-hooks.\nalready up to date.\nUpdating https://github.com/pre-commit/pre-commit-hooks ... already up to date.\nUpdating https://github.com/pycqa/isort ...\n[INFO] Initializing environment for https://github.com/pycqa/isort.\nalready up to date.\nUpdating https://github.com/ambv/black ...\n[INFO] Initializing environment for https://github.com/ambv/black.\nalready up to date.\nUpdating https://github.com/codespell-project/codespell ...\n[INFO] Initializing environment for https://github.com/codespell-project/codespell.\nalready up to date.\nUpdating https://github.com/sqlfluff/sqlfluff ...\n[INFO] Initializing environment for https://github.com/sqlfluff/sqlfluff.\nupdating 1.1.0 -> 1.2.1.\nUpdating https://github.com/pycqa/flake8 ...\n[INFO] Initializing environment for https://github.com/pycqa/flake8.\nalready up to date.\nUpdating https://github.com/DavidAnson/markdownlint-cli2 ...\n[INFO] Initializing environment for https://github.com/DavidAnson/markdownlint-cli2.\nalready up to date.\npre-commit install --hook-type pre-merge-commit\npre-commit installed at .git/hooks/pre-merge-commit\npre-commit install --hook-type pre-push\npre-commit installed at .git/hooks/pre-push\npre-commit install --hook-type post-rewrite\npre-commit installed at .git/hooks/post-rewrite\npre-commit install-hooks\n[INFO] Installing environment for https://github.com/pre-commit/pre-commit-hooks.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/pycqa/isort.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/ambv/black.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/codespell-project/codespell.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/sqlfluff/sqlfluff.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/pycqa/flake8.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/DavidAnson/markdownlint-cli2.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\npre-commit install\npre-commit installed at .git/hooks/pre-commit\n```\n\n## Implemented functions\n\n### LINQ functions\n\n[LINQ documentation](https://docs.microsoft.com/fr-fr/dotnet/api/system.linq.enumerable?view=net-6.0)\n\nAll function make before an `.execute()` are executed by the database server.\n\nMDPA = MagicDotPathAggregate\n<!-- markdownlint-disable MD013 -->\n|Method Name           |Description                                                          |Output        |\n|:---------------------|:--------------------------------------------------------------------|:-------------|\n|all                   |Return True if all elements match the predicate.                     |SQLEnumerable |\n|any                   |Return True if any elements match the predicate.                     |SQLEnumerable |\n|avg                   |Aggregation function to get the average of the predicate.            |MDPA          |\n|contains              |Return True if at least one element match the predicate.             |SQLEnumerable |\n|concat                |Aggregation function to concat a predicate.                          |MDPA          |\n|count                 |Return the number of line in a table.                                |SQLEnumerable |\n|count                 |Aggregation function to count a predicate.                           |MDPA          |\n|distinct              |Return all elements that are not duplicate.                          |SQLEnumerable |\n|element_at            |Return the element at the specific index.                            |SQLEnumerable |\n|element_at_or_default |Return the element at the specific index or None if index > len.     |SQLEnumerable |\n|except                |Returns all elements except elements from another SQLEnumerable.     |SQLEnumerable |\n|first                 |Return the first element match the predicate.                        |SQLEnumerable |\n|first_or_default      |Return the first element match the predicate or None if none match.  |SQLEnumerable |\n|group_by              |Return the selection group by a predicate.                           |SQLEnumerable |\n|group_join            |Return the join between 2 selections group by a predicate.           |SQLEnumerable |\n|intersect             |Return the intersection between 2 selections.                        |SQLEnumerable |\n|join                  |Return the join between 2 selections.                                |SQLEnumerable |\n|last                  |Return the last element match the predicate.                         |SQLEnumerable |\n|last_or_default       |Return the last element match the predicate or None if none match.   |SQLEnumerable |\n|max                   |Return the max element.                                              |SQLEnumerable |\n|max                   |Aggregate function to get the max of predicate.                      |MDPA          |\n|min                   |Return the min element.                                              |SQLEnumerable |\n|min                   |Aggregate function to get the min of predicate.                      |MDPA          |\n|order_by              |Return the selection order by key(s).                                |SQLEnumerable |\n|order_by_descending   |Return the selection order by descending by key(s).                  |SQLEnumerable |\n|select                |Return a selection of elements.                                      |SQLEnumerable |\n|single                |Return the only element match the predicate.                         |SQLEnumerable |\n|single_or_default     |Return the only element match the predicate or None if many matches. |SQLEnumerable |\n|skip                  |Return the selection minus _X_ first elements.                       |SQLEnumerable |\n|skip_last             |Return the selection minus _X_ last elements.                        |SQLEnumerable |\n|sum                   |Aggregation function to get the sum of a predicate.                  |MDPA          |\n|take                  |Return _X_ first element of the selection.                           |SQLEnumerable |\n|take_last             |Return _X_ last element of the selection.                            |SQLEnumerable |\n|union                 |Return the union between 2 selections.                               |SQLEnumerable |\n|where                 |Return the selection with all elements match the predicate.          |SQLEnumerable |\n<!-- markdownlint-enable MD013 -->\n\nFor more information see the [detailed documentation](https://py-linq-sql.readthedocs.io/en/latest/api/sqle/sqlenumerable/).\n\n### Custom functions\n\n|Method Name |Description                              |Output                         |\n|:-----------|:----------------------------------------|:------------------------------|\n|delete      |Delete data in a SQL table.              |SQLEnumerable                  |\n|execute     |Execute a request from an SQLEnumerable. |Enumerable | int | bool | dict |\n|insert      |Insert data in a SQL table.              |SQLEnumerable                  |\n|update      |Update data in a table.                  |SQLEnumerable                  |\n\n## Not implemented functions\n\n### LINQ functions\n\n|Method Name      |Description     |\n|:----------------|:---------------|\n|append           |Not implemented |\n|default_if_empty |Not implemented |\n|empty            |Not implemented |\n|prepend          |Not implemented |\n|range            |Not implemented |\n|repeat           |Not implemented |\n|reverse          |Not implemented |\n|select_many      |Not implemented |\n|skip_while       |Not implemented |\n|take_while       |Not implemented |\n|to_dictionary    |Not implemented |\n|to_list          |Not implemented |\n|zip              |Not implemented |\n\n### Py-Linq functions\n\n|Method Name|Description     |\n|:----------|:---------------|\n|add        |Not implemented |\n|median     |Not implemented |\n\n[Py-Linq link](https://viralogic.github.io/py-enumerable)\n\n## Contributing and info for developers\n\n- [Changelog](CHANGELOG.md)\n- [Contributing](CONTRIBUTING.md)\n- [Our git workflow](https://py-linq-sql.readthedocs.io/en/latest/workflow/)\n\n## Full documentation\n\n- [Py-LINQ-SQL Documentation](https://py-linq-sql.readthedocs.io/en/latest/)\n',
     'author': 'CHOSSON Ulysse',
     'author_email': 'ulysse.chosson@obspm.fr',
     'maintainer': 'CHOSSON Ulysse',
     'maintainer_email': 'ulysse.chosson@obspm.fr',
     'url': 'https://gitlab.obspm.fr/exoplanet/py-linq-sql',
```

### Comparing `py_linq_sql-1.8.2.1/PKG-INFO` & `py_linq_sql-1.8.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-linq-sql
-Version: 1.8.2.1
+Version: 1.8.3.1
 Summary: A Python module used for interacting with sql database using LINQ syntax.
 Home-page: https://gitlab.obspm.fr/exoplanet/py-linq-sql
 License: EUPL v1.2
 Keywords: linq,py-linq,sql,database,requests
 Author: CHOSSON Ulysse
 Author-email: ulysse.chosson@obspm.fr
 Maintainer: CHOSSON Ulysse
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dotmap (>=1.3.30,<2.0.0)
 Requires-Dist: psycopg (>=3.1.4,<4.0.0)
 Requires-Dist: py-linq (>=1.3.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
+Requires-Dist: strenum (>=0.4.8,<0.5.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: types-pyyaml (>=6.0.12.1,<7.0.0.0)
 Requires-Dist: types-toml (>=0.10.8,<0.11.0)
 Project-URL: Documentation, https://py-linq-sql.readthedocs.io/en/latest/
 Project-URL: Repository, https://gitlab.obspm.fr/exoplanet/py-linq-sql
 Description-Content-Type: text/markdown
```

