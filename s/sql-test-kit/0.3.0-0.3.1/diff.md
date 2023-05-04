# Comparing `tmp/sql_test_kit-0.3.0.tar.gz` & `tmp/sql_test_kit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_test_kit-0.3.0.tar", max compression
+gzip compressed data, was "sql_test_kit-0.3.1.tar", max compression
```

## Comparing `sql_test_kit-0.3.0.tar` & `sql_test_kit-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    13595 2023-04-23 14:08:45.896932 sql_test_kit-0.3.0/LICENSE
--rw-r--r--   0        0        0      502 2023-04-23 14:57:57.897057 sql_test_kit-0.3.0/README.md
--rw-r--r--   0        0        0      680 2023-05-01 20:30:40.896634 sql_test_kit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      209 2023-05-01 19:40:26.357338 sql_test_kit-0.3.0/sql_test_kit/__init__.py
--rw-r--r--   0        0        0      695 2023-05-01 18:41:57.666535 sql_test_kit-0.3.0/sql_test_kit/bigquery.py
--rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.3.0/sql_test_kit/column.py
--rw-r--r--   0        0        0      893 2023-05-01 19:40:26.366078 sql_test_kit-0.3.0/sql_test_kit/data_literals.py
--rw-r--r--   0        0        0      187 2023-05-01 19:40:18.408718 sql_test_kit-0.3.0/sql_test_kit/interpolation_data.py
--rw-r--r--   0        0        0     1393 2023-05-01 19:44:04.943564 sql_test_kit-0.3.0/sql_test_kit/query_interpolation.py
--rw-r--r--   0        0        0      390 2023-04-23 16:54:17.064138 sql_test_kit-0.3.0/sql_test_kit/table.py
--rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 sql_test_kit-0.3.0/setup.py
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 sql_test_kit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    13595 2023-04-23 14:08:45.896932 sql_test_kit-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2075 2023-05-04 08:32:53.529008 sql_test_kit-0.3.1/README.md
+-rw-r--r--   0        0        0      680 2023-05-04 08:34:49.141515 sql_test_kit-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-05-01 19:40:26.357338 sql_test_kit-0.3.1/sql_test_kit/__init__.py
+-rw-r--r--   0        0        0      695 2023-05-01 18:41:57.666535 sql_test_kit-0.3.1/sql_test_kit/bigquery.py
+-rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.3.1/sql_test_kit/column.py
+-rw-r--r--   0        0        0      893 2023-05-01 19:40:26.366078 sql_test_kit-0.3.1/sql_test_kit/data_literals.py
+-rw-r--r--   0        0        0      187 2023-05-01 19:40:18.408718 sql_test_kit-0.3.1/sql_test_kit/interpolation_data.py
+-rw-r--r--   0        0        0     1393 2023-05-01 19:44:04.943564 sql_test_kit-0.3.1/sql_test_kit/query_interpolation.py
+-rw-r--r--   0        0        0      390 2023-04-23 16:54:17.064138 sql_test_kit-0.3.1/sql_test_kit/table.py
+-rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 sql_test_kit-0.3.1/setup.py
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 sql_test_kit-0.3.1/PKG-INFO
```

### Comparing `sql_test_kit-0.3.0/LICENSE` & `sql_test_kit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_test_kit-0.3.0/pyproject.toml` & `sql_test_kit-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-test-kit"
-version = "0.3.0"
+version = "0.3.1"
 description = "Framework for testing SQL queries"
 authors = ["victorlandeau <vlandeau@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "sql_test_kit" },
 ]
```

### Comparing `sql_test_kit-0.3.0/sql_test_kit/bigquery.py` & `sql_test_kit-0.3.1/sql_test_kit/bigquery.py`

 * *Files identical despite different names*

### Comparing `sql_test_kit-0.3.0/sql_test_kit/data_literals.py` & `sql_test_kit-0.3.1/sql_test_kit/data_literals.py`

 * *Files identical despite different names*

### Comparing `sql_test_kit-0.3.0/sql_test_kit/query_interpolation.py` & `sql_test_kit-0.3.1/sql_test_kit/query_interpolation.py`

 * *Files identical despite different names*

