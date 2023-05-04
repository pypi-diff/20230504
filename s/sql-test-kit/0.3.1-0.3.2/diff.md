# Comparing `tmp/sql_test_kit-0.3.1.tar.gz` & `tmp/sql_test_kit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_test_kit-0.3.1.tar", max compression
+gzip compressed data, was "sql_test_kit-0.3.2.tar", max compression
```

## Comparing `sql_test_kit-0.3.1.tar` & `sql_test_kit-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    13595 2023-04-23 14:08:45.896932 sql_test_kit-0.3.1/LICENSE
--rw-r--r--   0        0        0     2075 2023-05-04 08:32:53.529008 sql_test_kit-0.3.1/README.md
--rw-r--r--   0        0        0      680 2023-05-04 08:34:49.141515 sql_test_kit-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      209 2023-05-01 19:40:26.357338 sql_test_kit-0.3.1/sql_test_kit/__init__.py
--rw-r--r--   0        0        0      695 2023-05-01 18:41:57.666535 sql_test_kit-0.3.1/sql_test_kit/bigquery.py
--rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.3.1/sql_test_kit/column.py
--rw-r--r--   0        0        0      893 2023-05-01 19:40:26.366078 sql_test_kit-0.3.1/sql_test_kit/data_literals.py
--rw-r--r--   0        0        0      187 2023-05-01 19:40:18.408718 sql_test_kit-0.3.1/sql_test_kit/interpolation_data.py
--rw-r--r--   0        0        0     1393 2023-05-01 19:44:04.943564 sql_test_kit-0.3.1/sql_test_kit/query_interpolation.py
--rw-r--r--   0        0        0      390 2023-04-23 16:54:17.064138 sql_test_kit-0.3.1/sql_test_kit/table.py
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 sql_test_kit-0.3.1/setup.py
--rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 sql_test_kit-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    13595 2023-04-23 14:08:45.896932 sql_test_kit-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2071 2023-05-04 08:39:46.202781 sql_test_kit-0.3.2/README.md
+-rw-r--r--   0        0        0      680 2023-05-04 08:39:46.200186 sql_test_kit-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-05-01 19:40:26.357338 sql_test_kit-0.3.2/sql_test_kit/__init__.py
+-rw-r--r--   0        0        0      695 2023-05-01 18:41:57.666535 sql_test_kit-0.3.2/sql_test_kit/bigquery.py
+-rw-r--r--   0        0        0      115 2023-04-22 22:03:27.645182 sql_test_kit-0.3.2/sql_test_kit/column.py
+-rw-r--r--   0        0        0      893 2023-05-01 19:40:26.366078 sql_test_kit-0.3.2/sql_test_kit/data_literals.py
+-rw-r--r--   0        0        0      187 2023-05-01 19:40:18.408718 sql_test_kit-0.3.2/sql_test_kit/interpolation_data.py
+-rw-r--r--   0        0        0     1393 2023-05-01 19:44:04.943564 sql_test_kit-0.3.2/sql_test_kit/query_interpolation.py
+-rw-r--r--   0        0        0      390 2023-04-23 16:54:17.064138 sql_test_kit-0.3.2/sql_test_kit/table.py
+-rw-r--r--   0        0        0     2758 1970-01-01 00:00:00.000000 sql_test_kit-0.3.2/setup.py
+-rw-r--r--   0        0        0     2705 1970-01-01 00:00:00.000000 sql_test_kit-0.3.2/PKG-INFO
```

### Comparing `sql_test_kit-0.3.1/LICENSE` & `sql_test_kit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_test_kit-0.3.1/README.md` & `sql_test_kit-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # sql-test-kit
 
 This is a framework for testing SQL queries.
 It works by directly running the queries against the targeted engine, thus being robust to any change in the
 corresponding SQL dialect.
 Moreover, it is currently focused on interpolating test data directly inside the SQL queries, making the test much
-quicker than if it were creating temporary tables.
+quicker than if it was creating actual tables.
 
 # Application example
 
 Using the Table and Column class, you can generate variablized SQL queries such as this :
 
     sales_amount_col = "SALES_AMOUNT"
     sales_date_col = "SALES_DATE"
```

### Comparing `sql_test_kit-0.3.1/pyproject.toml` & `sql_test_kit-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-test-kit"
-version = "0.3.1"
+version = "0.3.2"
 description = "Framework for testing SQL queries"
 authors = ["victorlandeau <vlandeau@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "sql_test_kit" },
 ]
```

### Comparing `sql_test_kit-0.3.1/sql_test_kit/bigquery.py` & `sql_test_kit-0.3.2/sql_test_kit/bigquery.py`

 * *Files identical despite different names*

### Comparing `sql_test_kit-0.3.1/sql_test_kit/data_literals.py` & `sql_test_kit-0.3.2/sql_test_kit/data_literals.py`

 * *Files identical despite different names*

### Comparing `sql_test_kit-0.3.1/sql_test_kit/query_interpolation.py` & `sql_test_kit-0.3.2/sql_test_kit/query_interpolation.py`

 * *Files identical despite different names*

### Comparing `sql_test_kit-0.3.1/setup.py` & `sql_test_kit-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.0.0']
 
 setup_kwargs = {
     'name': 'sql-test-kit',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Framework for testing SQL queries',
-    'long_description': '# sql-test-kit\n\nThis is a framework for testing SQL queries.\nIt works by directly running the queries against the targeted engine, thus being robust to any change in the\ncorresponding SQL dialect.\nMoreover, it is currently focused on interpolating test data directly inside the SQL queries, making the test much\nquicker than if it were creating temporary tables.\n\n# Application example\n\nUsing the Table and Column class, you can generate variablized SQL queries such as this :\n\n    sales_amount_col = "SALES_AMOUNT"\n    sales_date_col = "SALES_DATE"\n    sales_table = BigqueryTable(\n        project="project",\n        dataset="dataset",\n        table="table",\n        columns=[\n            Column(sales_amount_col, "FLOAT64"),\n            Column(sales_date_col, "STRING"),\n        ],\n    )\n    current_year_sales_by_day_query = f"""\n        SELECT {sales_date_col}, SUM({sales_amount_col}) as {sales_amount_col}\n        FROM {sales_table}\n        WHERE {sales_date_col} >= "2023-01-01"\n        GROUP BY {sales_date_col}\n    """\n\nYou can then test it this way :\n\n    def test_current_year_sales_by_day_query():\n        # Given\n        sales_data = pd.DataFrame(\n            {\n                "SALES_ID": [1, 2, 3, 4],\n                sales_date_col: ["2022-12-31", "2023-01-01", "2023-01-01", "2023-01-02"],\n                sales_amount_col: [10, 20, 30, 40],\n            }\n        )\n    \n        # When\n        interpolated_query = QueryInterpolator() \\\n            .add_input_table(sales_table, sales_data) \\\n            .interpolate_query(current_year_sales_by_day_query)\n        current_year_sales_by_day_data = Client().query(interpolated_query).to_dataframe()\n    \n        # Then\n        expected_current_year_sales_by_day_data = pd.DataFrame(\n            {\n                sales_date_col: ["2023-01-01", "2023-01-02"],\n                sales_amount_col: [50, 40],\n            }\n        )\n    \n        pd.testing.assert_frame_equal(\n            current_year_sales_by_day_data,\n            expected_current_year_sales_by_day_data,\n            check_dtype=False,\n        )\n',
+    'long_description': '# sql-test-kit\n\nThis is a framework for testing SQL queries.\nIt works by directly running the queries against the targeted engine, thus being robust to any change in the\ncorresponding SQL dialect.\nMoreover, it is currently focused on interpolating test data directly inside the SQL queries, making the test much\nquicker than if it was creating actual tables.\n\n# Application example\n\nUsing the Table and Column class, you can generate variablized SQL queries such as this :\n\n    sales_amount_col = "SALES_AMOUNT"\n    sales_date_col = "SALES_DATE"\n    sales_table = BigqueryTable(\n        project="project",\n        dataset="dataset",\n        table="table",\n        columns=[\n            Column(sales_amount_col, "FLOAT64"),\n            Column(sales_date_col, "STRING"),\n        ],\n    )\n    current_year_sales_by_day_query = f"""\n        SELECT {sales_date_col}, SUM({sales_amount_col}) as {sales_amount_col}\n        FROM {sales_table}\n        WHERE {sales_date_col} >= "2023-01-01"\n        GROUP BY {sales_date_col}\n    """\n\nYou can then test it this way :\n\n    def test_current_year_sales_by_day_query():\n        # Given\n        sales_data = pd.DataFrame(\n            {\n                "SALES_ID": [1, 2, 3, 4],\n                sales_date_col: ["2022-12-31", "2023-01-01", "2023-01-01", "2023-01-02"],\n                sales_amount_col: [10, 20, 30, 40],\n            }\n        )\n    \n        # When\n        interpolated_query = QueryInterpolator() \\\n            .add_input_table(sales_table, sales_data) \\\n            .interpolate_query(current_year_sales_by_day_query)\n        current_year_sales_by_day_data = Client().query(interpolated_query).to_dataframe()\n    \n        # Then\n        expected_current_year_sales_by_day_data = pd.DataFrame(\n            {\n                sales_date_col: ["2023-01-01", "2023-01-02"],\n                sales_amount_col: [50, 40],\n            }\n        )\n    \n        pd.testing.assert_frame_equal(\n            current_year_sales_by_day_data,\n            expected_current_year_sales_by_day_data,\n            check_dtype=False,\n        )\n',
     'author': 'victorlandeau',
     'author_email': 'vlandeau@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sql_test_kit-0.3.1/PKG-INFO` & `sql_test_kit-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-test-kit
-Version: 0.3.1
+Version: 0.3.2
 Summary: Framework for testing SQL queries
 Author: victorlandeau
 Author-email: vlandeau@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 
 # sql-test-kit
 
 This is a framework for testing SQL queries.
 It works by directly running the queries against the targeted engine, thus being robust to any change in the
 corresponding SQL dialect.
 Moreover, it is currently focused on interpolating test data directly inside the SQL queries, making the test much
-quicker than if it were creating temporary tables.
+quicker than if it was creating actual tables.
 
 # Application example
 
 Using the Table and Column class, you can generate variablized SQL queries such as this :
 
     sales_amount_col = "SALES_AMOUNT"
     sales_date_col = "SALES_DATE"
```

