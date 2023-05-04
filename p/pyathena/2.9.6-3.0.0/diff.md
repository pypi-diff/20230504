# Comparing `tmp/PyAthena-2.9.6.tar.gz` & `tmp/pyathena-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAthena-2.9.6.tar", max compression
+gzip compressed data, was "pyathena-3.0.0.tar", max compression
```

## Comparing `PyAthena-2.9.6.tar` & `pyathena-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,41 @@
--rw-r--r--   0        0        0     1055 2022-07-09 07:03:53.635669 PyAthena-2.9.6/LICENSE
--rw-r--r--   0        0        0    64666 2022-07-09 07:03:53.635669 PyAthena-2.9.6/README.rst
--rw-r--r--   0        0        0     1873 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/__init__.py
--rw-r--r--   0        0        0       24 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     4735 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2554 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     6952 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9526 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2443 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/arrow/util.py
--rw-r--r--   0        0        0     4957 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/async_cursor.py
--rw-r--r--   0        0        0    17700 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/common.py
--rw-r--r--   0        0        0     9074 2022-07-09 07:03:53.635669 PyAthena-2.9.6/pyathena/connection.py
--rw-r--r--   0        0        0     4227 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/converter.py
--rw-r--r--   0        0        0     5378 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/cursor.py
--rw-r--r--   0        0        0      660 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/error.py
--rw-r--r--   0        0        0     6781 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/formatter.py
--rw-r--r--   0        0        0    13165 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/model.py
--rw-r--r--   0        0        0       24 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5117 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1830 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     7264 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    10107 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0     9942 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/pandas/util.py
--rw-r--r--   0        0        0        0 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/py.typed
--rw-r--r--   0        0        0    18857 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/result_set.py
--rw-r--r--   0        0        0    29196 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/sqlalchemy_athena.py
--rw-r--r--   0        0        0     2270 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyathena/util.py
--rw-r--r--   0        0        0     2696 2022-07-09 07:03:53.639669 PyAthena-2.9.6/pyproject.toml
--rw-r--r--   0        0        0    68051 2022-07-09 07:08:46.980487 PyAthena-2.9.6/setup.py
--rw-r--r--   0        0        0    65879 2022-07-09 07:08:46.983854 PyAthena-2.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-05-04 18:42:17.601809 pyathena-3.0.0/LICENSE
+-rw-r--r--   0        0        0    70055 2023-05-04 18:42:17.601809 pyathena-3.0.0/README.rst
+-rw-r--r--   0        0        0     1923 2023-05-04 18:42:17.601809 pyathena-3.0.0/pyathena/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-04 18:42:17.601809 pyathena-3.0.0/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     5157 2023-05-04 18:42:17.601809 pyathena-3.0.0/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2554 2023-05-04 18:42:17.601809 pyathena-3.0.0/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     7250 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9529 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2421 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/arrow/util.py
+-rw-r--r--   0        0        0     5373 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    21136 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/common.py
+-rw-r--r--   0        0        0    10416 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/connection.py
+-rw-r--r--   0        0        0     4209 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/converter.py
+-rw-r--r--   0        0        0     5722 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/cursor.py
+-rw-r--r--   0        0        0      660 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/error.py
+-rw-r--r--   0        0        0       24 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2439 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    20474 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0     1216 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0     6571 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/formatter.py
+-rw-r--r--   0        0        0    16886 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/model.py
+-rw-r--r--   0        0        0      220 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5829 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1830 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     8327 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13377 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0     9822 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/util.py
+-rw-r--r--   0        0        0        0 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/py.typed
+-rw-r--r--   0        0        0    24126 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/result_set.py
+-rw-r--r--   0        0        0       24 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      661 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    36892 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      884 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2638 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1210 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0     1948 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/util.py
+-rw-r--r--   0        0        0     3482 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    71494 1970-01-01 00:00:00.000000 pyathena-3.0.0/PKG-INFO
```

### Comparing `PyAthena-2.9.6/LICENSE` & `pyathena-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAthena-2.9.6/README.rst` & `pyathena-3.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+.. image:: https://badge.fury.io/py/pyathena.svg
+    :target: https://badge.fury.io/py/pyathena
+
 .. image:: https://img.shields.io/pypi/pyversions/PyAthena.svg
     :target: https://pypi.org/project/PyAthena/
 
 .. image:: https://github.com/laughingman7743/PyAthena/actions/workflows/test.yaml/badge.svg
     :target: https://github.com/laughingman7743/PyAthena/actions/workflows/test.yaml
 
 .. image:: https://img.shields.io/pypi/l/PyAthena.svg
@@ -9,14 +12,17 @@
 
 .. image:: https://pepy.tech/badge/pyathena/month
     :target: https://pepy.tech/project/pyathena
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
+
 PyAthena
 ========
 
 PyAthena is a Python `DB API 2.0 (PEP 249)`_ client for `Amazon Athena`_.
 
 .. _`DB API 2.0 (PEP 249)`: https://www.python.org/dev/peps/pep-0249/
 .. _`Amazon Athena`: https://docs.aws.amazon.com/athena/latest/APIReference/Welcome.html
@@ -26,34 +32,36 @@
    :depth: 2
 
 Requirements
 ------------
 
 * Python
 
-  - CPython 3.7 3.8 3.9 3.10
+  - CPython 3.8 3.9 3.10, 3.11
 
 Installation
 ------------
 
 .. code:: bash
 
     $ pip install PyAthena
 
 Extra packages:
 
-+---------------+--------------------------------------+------------------+
-| Package       | Install command                      | Version          |
-+===============+======================================+==================+
-| SQLAlchemy    | ``pip install PyAthena[SQLAlchemy]`` | >=1.0.0, <2.0.0  |
-+---------------+--------------------------------------+------------------+
-| Pandas        | ``pip install PyAthena[Pandas]``     | >=1.3.0          |
-+---------------+--------------------------------------+------------------+
-| Arrow         | ``pip install PyAthena[Arrow]``      | >=7.0.0          |
-+---------------+--------------------------------------+------------------+
++---------------+---------------------------------------+------------------+
+| Package       | Install command                       | Version          |
++===============+=======================================+==================+
+| SQLAlchemy    | ``pip install PyAthena[SQLAlchemy]``  | >=1.0.0          |
++---------------+---------------------------------------+------------------+
+| Pandas        | ``pip install PyAthena[Pandas]``      | >=1.3.0          |
++---------------+---------------------------------------+------------------+
+| Arrow         | ``pip install PyAthena[Arrow]``       | >=7.0.0          |
++---------------+---------------------------------------+------------------+
+| fastparquet   | ``pip install PyAthena[fastparquet]`` | >=0.4.0          |
++---------------+---------------------------------------+------------------+
 
 Usage
 -----
 
 Basic usage
 ~~~~~~~~~~~
 
@@ -107,52 +115,48 @@
 
 .. _`DB API paramstyle`: https://www.python.org/dev/peps/pep-0249/#paramstyle
 .. _`named placeholders`: https://pyformat.info/#named_placeholders
 
 SQLAlchemy
 ~~~~~~~~~~
 
-Install SQLAlchemy with ``pip install "SQLAlchemy>=1.0.0, <2.0.0"`` or ``pip install PyAthena[SQLAlchemy]``.
-Supported SQLAlchemy is 1.0.0 or higher and less than 2.0.0.
+Install SQLAlchemy with ``pip install "SQLAlchemy>=1.0.0"`` or ``pip install PyAthena[SQLAlchemy]``.
+Supported SQLAlchemy is 1.0.0 or higher.
 
 .. code:: python
 
-    from urllib.parse import quote_plus
+    from sqlalchemy import func, select
     from sqlalchemy.engine import create_engine
-    from sqlalchemy.sql.expression import select
-    from sqlalchemy.sql.functions import func
     from sqlalchemy.sql.schema import Table, MetaData
 
     conn_str = "awsathena+rest://{aws_access_key_id}:{aws_secret_access_key}@athena.{region_name}.amazonaws.com:443/"\
                "{schema_name}?s3_staging_dir={s3_staging_dir}"
     engine = create_engine(conn_str.format(
-        aws_access_key_id=quote_plus("YOUR_ACCESS_KEY_ID"),
-        aws_secret_access_key=quote_plus("YOUR_SECRET_ACCESS_KEY"),
+        aws_access_key_id="YOUR_ACCESS_KEY_ID",
+        aws_secret_access_key="YOUR_SECRET_ACCESS_KEY",
         region_name="us-west-2",
         schema_name="default",
-        s3_staging_dir=quote_plus("s3://YOUR_S3_BUCKET/path/to/")))
+        s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/"))
     with engine.connect() as connection:
         many_rows = Table("many_rows", MetaData(), autoload_with=connection)
-        result = connection.execute(select([func.count("*")], from_obj=many_rows))
+        result = connection.execute(select(func.count()).select_from(many_rows))
         print(result.scalar())
 
 The connection string has the following format:
 
 .. code:: text
 
     awsathena+rest://{aws_access_key_id}:{aws_secret_access_key}@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&...
 
 If you do not specify ``aws_access_key_id`` and ``aws_secret_access_key`` using instance profile or boto3 configuration file:
 
 .. code:: text
 
     awsathena+rest://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&...
 
-NOTE: ``s3_staging_dir`` requires quote. If ``aws_access_key_id``, ``aws_secret_access_key`` and other parameter contain special characters, quote is also required.
-
 Dialect & driver
 ^^^^^^^^^^^^^^^^
 
 +-----------+--------+------------------+-----------------+
 | Dialect   | Driver | Schema           | Cursor          |
 +===========+========+==================+=================+
 | awsathena |        | awsathena        | DefaultCursor   |
@@ -370,36 +374,35 @@
     cursor.execute("SELECT * FROM many_rows")
     df = as_pandas(cursor)
     print(df.describe())
 
 If you want to use the query results output to S3 directly, you can use `PandasCursor`_.
 This cursor fetches query results faster than the default cursor. (See `benchmark results`_.)
 
-.. _`pandas.read_sql_query`: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_sql_query.html
+.. _`pandas.read_sql_query`: https://pandas.pydata.org/docs/reference/api/pandas.read_sql_query.html
 .. _`benchmark results`: benchmarks/
 
 To SQL
 ^^^^^^
 
 You can use `pandas.DataFrame.to_sql`_ to write records stored in DataFrame to Amazon Athena.
 `pandas.DataFrame.to_sql`_ uses `SQLAlchemy`_, so you need to install it.
 
 .. code:: python
 
     import pandas as pd
-    from urllib.parse import quote_plus
     from sqlalchemy import create_engine
 
     conn_str = "awsathena+rest://:@athena.{region_name}.amazonaws.com:443/"\
                "{schema_name}?s3_staging_dir={s3_staging_dir}&location={location}&compression=snappy"
     engine = create_engine(conn_str.format(
         region_name="us-west-2",
         schema_name="YOUR_SCHEMA",
-        s3_staging_dir=quote_plus("s3://YOUR_S3_BUCKET/path/to/"),
-        location=quote_plus("s3://YOUR_S3_BUCKET/path/to/")))
+        s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+        location="s3://YOUR_S3_BUCKET/path/to/"))
 
     df = pd.DataFrame({"a": [1, 2, 3, 4, 5]})
     df.to_sql("YOUR_TABLE", engine, schema="YOUR_SCHEMA", index=False, if_exists="replace", method="multi")
 
 The location of the Amazon S3 table is specified by the ``location`` parameter in the connection string.
 If ``location`` is not specified, ``s3_staging_dir`` parameter will be used. The following rules apply.
 
@@ -462,15 +465,15 @@
     conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
                    region_name="us-west-2")
     df = pd.DataFrame({"a": [1, 2, 3, 4, 5]})
     to_sql(df, "YOUR_TABLE", conn, "s3://YOUR_S3_BUCKET/path/to/",
            schema="YOUR_SCHEMA", index=False, if_exists="replace",
            chunksize=1, executor_class=ProcessPoolExecutor, max_workers=5)
 
-.. _`pandas.DataFrame.to_sql`: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_sql.html
+.. _`pandas.DataFrame.to_sql`: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_sql.html
 .. _`ThreadPoolExecutor`: https://docs.python.org/3/library/concurrent.futures.html#threadpoolexecutor
 .. _`ProcessPoolExecutor`: https://docs.python.org/3/library/concurrent.futures.html#processpoolexecutor
 
 DictCursor
 ~~~~~~~~~~
 
 DictCursor retrieve the query execution result as a dictionary type with column names and values.
@@ -927,26 +930,26 @@
 
     from pyathena import connect
     from pyathena.pandas.cursor import PandasCursor
 
     cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
                      region_name="us-west-2").cursor(PandasCursor, converter=CustomPandasTypeConverter())
 
-If the unload option is enabled, the Parquet file itself has a schema, so the conversion is done to the dtypes according to that schema,
-and the ``mappings`` and ``types`` settings of the Converter class are not used.
-
 .. code:: python
 
     from pyathena import connect
     from pyathena.pandas.cursor import PandasCursor
 
     cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
                      region_name="us-west-2",
                      converter=CustomPandasTypeConverter()).cursor(PandasCursor)
 
+If the unload option is enabled, the Parquet file itself has a schema, so the conversion is done to the dtypes according to that schema,
+and the ``mappings`` and ``types`` settings of the Converter class are not used.
+
 If you want to change the NaN behavior of pandas.Dataframe,
 you can do so by using the ``keep_default_na``, ``na_values`` and ``quoting`` arguments of the cursor object's execute method.
 
 .. code:: python
 
     from pyathena import connect
     from pyathena.pandas.cursor import PandasCursor
@@ -956,25 +959,120 @@
                      cursor_class=PandasCursor).cursor()
     df = cursor.execute("SELECT * FROM many_rows",
                         keep_default_na=False,
                         na_values=[""]).as_pandas()
 
 NOTE: PandasCursor handles the CSV file on memory. Pay attention to the memory capacity.
 
-.. _`pandas.DataFrame object`: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
-.. _`pandas.Timestamp`: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Timestamp.html
+.. _`pandas.DataFrame object`: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html
+.. _`pandas.Timestamp`: https://pandas.pydata.org/docs/reference/api/pandas.Timestamp.html
+
+[PandasCursor] Chunksize options
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+The Pandas cursor can read the CSV file for each specified number of rows by using the chunksize option.
+This option should reduce memory usage.
+
+The chunksize option can be enabled by specifying an integer value in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor,
+                     cursor_kwargs={
+                         "chunksize": 1_000_000
+                     }).cursor()
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor(chunksize=1_000_000)
+
+It can also be specified in the execution method when executing the query.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+    cursor.execute("SELECT * FROM many_rows", chunksize=1_000_000)
+
+SQLAlchemy allows this option to be specified in the connection string.
+
+.. code:: text
+
+    awsathena+pandas://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&chunksize=1000000...
+
+When this option is used, the object returned by the as_pandas method is a ``DataFrameIterator`` object.
+This object has exactly the same interface as the ``TextFileReader`` object and can be handled in the same way.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+    df_iter = cursor.execute("SELECT * FROM many_rows", chunksize=1_000_000).as_pandas()
+    for df in df_iter:
+        print(df.describe())
+        print(df.head())
+
+You can also concatenate them into a single `pandas.DataFrame object`_ using `pandas.concat`_.
+
+.. code:: python
+
+    import pandas
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+    df_iter = cursor.execute("SELECT * FROM many_rows", chunksize=1_000_000).as_pandas()
+    df = pandas.concat((df for df in df_iter), ignore_index=True)
+
+You can use the ``get_chunk`` method to retrieve a `pandas.DataFrame object`_ for each specified number of rows.
+When all rows have been read, calling the ``get_chunk`` method will raise ``StopIteration``.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+    df_iter = cursor.execute("SELECT * FROM many_rows LIMIT 15", chunksize=1_000_000).as_pandas()
+    df_iter.get_chunk(10)
+    df_iter.get_chunk(10)
+    df_iter.get_chunk(10)  # raise StopIteration
+
+.. _`pandas.concat`: https://pandas.pydata.org/docs/reference/api/pandas.concat.html
 
 [PandasCursor] Unload options
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-PandasCursor also supports the UNLOAD option, as does `ArrowCursor`_.
+PandasCursor also supports the unload option, as does `ArrowCursor`_.
 
 See `[ArrowCursor] Unload options`_ for more information.
 
-The UNLOAD option can be enabled by specifying it in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.
+The unload option can be enabled by specifying it in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.
 
 .. code:: python
 
     from pyathena import connect
     from pyathena.pandas.cursor import PandasCursor
 
     cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
@@ -1153,15 +1251,15 @@
     cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
                      region_name="us-west-2",
                      cursor_class=AsyncPandasCursor).cursor()
 
     query_id, future = cursor.execute("SELECT * FROM many_rows")
     cursor.cancel(query_id)
 
-As with PandasCursor, the UNLOAD option is also available.
+As with PandasCursor, the unload option is also available.
 
 .. code:: python
 
     from pyathena import connect
     from pyathena.pandas.cursor import AsyncPandasCursor
 
     cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
@@ -1366,29 +1464,29 @@
 
 If the unload option is enabled, the Parquet file itself has a schema, so the conversion is done to the Arrow type according to that schema,
 and the ``types`` setting of the Converter class is not used.
 
 [ArrowCursor] Unload options
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-ArrowCurosr supports the UNLOAD option. When this option is enabled,
-queries with SELECT statements are automatically converted to UNLOAD statements and executed to Athena,
+ArrowCursor supports the unload option. When this option is enabled,
+queries with SELECT statements are automatically converted to unload statements and executed to Athena,
 and the results are output in Parquet format (Snappy compressed) to ``s3_staging_dir``.
 The cursor reads the output Parquet file directly.
 
-The output of query results with the UNLOAD statement is faster than normal query execution.
+The output of query results with the unload statement is faster than normal query execution.
 In addition, the output Parquet file is split and can be read faster than a CSV file.
 We recommend trying this option if you are concerned about the time it takes to execute the query and retrieve the results.
 
-However, UNLOAD has some limitations. Please refer to the `official UNLOAD documentation`_ for more information on limitations.
-As per the limitations of the official documentation, the results of UNLOAD will be written to multiple files in parallel,
+However, unload has some limitations. Please refer to the `official unload documentation`_ for more information on limitations.
+As per the limitations of the official documentation, the results of unload will be written to multiple files in parallel,
 and the contents of each file will be in sort order, but the relative order of the files to each other will not be sorted.
 Note that specifying ORDER BY with this option enabled does not guarantee the sort order of the data.
 
-The UNLOAD option can be enabled by specifying it in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.
+The unload option can be enabled by specifying it in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.
 
 .. code:: python
 
     from pyathena import connect
     from pyathena.arrow.cursor import ArrowCursor
 
     cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
@@ -1409,30 +1507,30 @@
 
 SQLAlchemy allows this option to be specified in the connection string.
 
 .. code:: text
 
     awsathena+arrow://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&unload=true...
 
-If a ``NOT_SUPPORTED`` occurs, a type not supported by UNLOAD is included in the result of the SELECT.
+If a ``NOT_SUPPORTED`` occurs, a type not supported by unload is included in the result of the SELECT.
 Try converting to another type, such as ``SELECT CAST(1 AS VARCHAR) AS name``.
 
 .. code:: text
 
     pyathena.error.OperationalError: NOT_SUPPORTED: Unsupported Hive type: time
 
 In most cases of ``SYNTAX_ERROR``, you forgot to alias the column in the SELECT result.
 Try adding an alias to the SELECTed column, such as ``SELECT 1 AS name``.
 
 .. code:: text
 
     pyathena.error.OperationalError: SYNTAX_ERROR: line 1:1: Column name not specified at position 1
 
 .. _`pyarrow.Table object`: https://arrow.apache.org/docs/python/generated/pyarrow.Table.html
-.. _`official UNLOAD documentation`: https://docs.aws.amazon.com/athena/latest/ug/unload.html
+.. _`official unload documentation`: https://docs.aws.amazon.com/athena/latest/ug/unload.html
 
 AsyncArrowCursor
 ~~~~~~~~~~~~~~~~
 
 AsyncArrowCursor is an AsyncCursor that can handle `pyarrow.Table object`_.
 This cursor directly handles the CSV of query results output to S3 in the same way as ArrowCursor.
 
@@ -1601,14 +1699,59 @@
     cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
                      region_name="us-west-2",
                      cursor_class=AsyncArrowCursor).cursor(unload=True)
 
 Quickly re-run queries
 ~~~~~~~~~~~~~~~~~~~~~~
 
+Result reuse configuration
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Athena engine version 3 allows you to `reuse the results of previous queries`_.
+
+It is available by specifying the arguments ``result_reuse_enable`` and ``result_reuse_minutes`` in the connection object.
+
+.. code:: python
+
+    from pyathena import connect
+
+    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                   region_name="us-west-2",
+                   work_group="YOUR_WORK_GROUP",
+                   result_reuse_enable=True,
+                   result_reuse_minutes=60)
+
+You can also specify ``result_reuse_enable`` and ``result_reuse_minutes`` when executing a query.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+    cursor.execute("SELECT * FROM one_row",
+                   work_group="YOUR_WORK_GROUP",
+                   result_reuse_enable=True,
+                   result_reuse_minutes=60)
+
+If the following error occurs, please use a workgroup configured with Athena engine version 3.
+
+.. code:: text
+
+    pyathena.error.DatabaseError: An error occurred (InvalidRequestException) when calling the StartQueryExecution operation: This functionality is not enabled in the selected engine version. Please check the engine version settings or contact AWS support for further assistance.
+
+If for some reason you cannot use the reuse feature of Athena engine version 3, please use the `Cache configuration`_ implemented by PyAthena.
+
+.. _`reuse the results of previous queries`: https://docs.aws.amazon.com/athena/latest/ug/reusing-query-results.html
+
+Cache configuration
+^^^^^^^^^^^^^^^^^^^
+
+**Please use the Result reuse configuration.**
+
 You can attempt to re-use the results from a previously executed query to help save time and money in the cases where your underlying data isn't changing.
 Set the ``cache_size`` or ``cache_expiration_time`` parameter of ``cursor.execute()`` to a number larger than 0 to enable caching.
 
 .. code:: python
 
     from pyathena import connect
 
@@ -1795,15 +1938,15 @@
 Run test multiple Python versions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. code:: bash
 
     $ pip install poetry
     $ poetry install -v
-    $ pyenv local 3.10.1 3.9.1 3.8.2 3.7.2
+    $ pyenv local 3.11.1 3.10.1 3.9.1 3.8.2
     $ poetry run tox
 
 GitHub Actions
 ~~~~~~~~~~~~~~
 
 GitHub Actions uses OpenID Connect (OIDC) to access AWS resources. You will need to refer to the `GitHub Actions documentation`_ to configure it.
```

### Comparing `PyAthena-2.9.6/pyathena/__init__.py` & `pyathena-3.0.0/pyathena/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from typing import TYPE_CHECKING, FrozenSet, Type
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection
 
-__version__: str = "2.9.6"
+__version__: str = "3.0.0"
+user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
-threadsafety: int = 3
+threadsafety: int = 2
 paramstyle: str = "pyformat"
 
 
 class DBAPITypeObject(FrozenSet[str]):
     """Type Objects and Constructors
 
     https://www.python.org/dev/peps/pep-0249/#type-objects-and-constructors
```

### Comparing `PyAthena-2.9.6/pyathena/arrow/async_cursor.py` & `pyathena-3.0.0/pyathena/arrow/async_cursor.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         poll_interval: float = 1,
         encryption_option: Optional[str] = None,
         kms_key: Optional[str] = None,
         kill_on_interrupt: bool = True,
         max_workers: int = (cpu_count() or 1) * 5,
         arraysize: int = CursorIterator.DEFAULT_FETCH_SIZE,
         unload: bool = False,
+        result_reuse_enable: bool = False,
+        result_reuse_minutes: int = CursorIterator.DEFAULT_RESULT_REUSE_MINUTES,
     ) -> None:
         super(AsyncArrowCursor, self).__init__(
             connection=connection,
             converter=converter,
             formatter=formatter,
             retry_config=retry_config,
             s3_staging_dir=s3_staging_dir,
@@ -53,14 +55,16 @@
             work_group=work_group,
             poll_interval=poll_interval,
             encryption_option=encryption_option,
             kms_key=kms_key,
             kill_on_interrupt=kill_on_interrupt,
             max_workers=max_workers,
             arraysize=arraysize,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         self._unload = unload
 
     @staticmethod
     def get_default_converter(
         unload: bool = False,
     ) -> Union[DefaultArrowTypeConverter, DefaultArrowUnloadTypeConverter, Any]:
@@ -79,15 +83,15 @@
             raise ProgrammingError("arraysize must be a positive integer value.")
         self._arraysize = value
 
     def _collect_result_set(
         self,
         query_id: str,
         unload_location: Optional[str] = None,
-        kwargs: Dict[str, Any] = None,
+        kwargs: Optional[Dict[str, Any]] = None,
     ) -> AthenaArrowResultSet:
         if kwargs is None:
             kwargs = dict()
         query_execution = self._poll(query_id)
         return AthenaArrowResultSet(
             connection=self._connection,
             converter=self._converter,
@@ -103,21 +107,21 @@
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
+        result_reuse_enable: Optional[bool] = None,
+        result_reuse_minutes: Optional[int] = None,
         **kwargs,
     ) -> Tuple[str, "Future[Union[AthenaArrowResultSet, Any]]"]:
         if self._unload:
             s3_staging_dir = s3_staging_dir if s3_staging_dir else self._s3_staging_dir
-            assert (
-                s3_staging_dir
-            ), "If the unload option is used, s3_staging_dir is required."
+            assert s3_staging_dir, "If the unload option is used, s3_staging_dir is required."
             operation, unload_location = self._formatter.wrap_unload(
                 operation,
                 s3_staging_dir=s3_staging_dir,
                 format_=AthenaFileFormat.FILE_FORMAT_PARQUET,
                 compression=AthenaCompression.COMPRESSION_SNAPPY,
             )
         else:
@@ -125,14 +129,16 @@
         query_id = self._execute(
             operation,
             parameters=parameters,
             work_group=work_group,
             s3_staging_dir=s3_staging_dir,
             cache_size=cache_size,
             cache_expiration_time=cache_expiration_time,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         return (
             query_id,
             self._executor.submit(
                 self._collect_result_set,
                 query_id,
                 unload_location,
```

### Comparing `PyAthena-2.9.6/pyathena/arrow/converter.py` & `pyathena-3.0.0/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `PyAthena-2.9.6/pyathena/arrow/cursor.py` & `pyathena-3.0.0/pyathena/arrow/cursor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 
 from pyathena.arrow.converter import (
     DefaultArrowTypeConverter,
     DefaultArrowUnloadTypeConverter,
 )
 from pyathena.arrow.result_set import AthenaArrowResultSet
 from pyathena.common import BaseCursor, CursorIterator
 from pyathena.converter import Converter
 from pyathena.error import OperationalError, ProgrammingError
 from pyathena.formatter import Formatter
 from pyathena.model import AthenaCompression, AthenaFileFormat, AthenaQueryExecution
 from pyathena.result_set import WithResultSet
-from pyathena.util import RetryConfig, synchronized
+from pyathena.util import RetryConfig
 
 if TYPE_CHECKING:
     from pyarrow import Table
 
     from pyathena.connection import Connection
 
 _logger = logging.getLogger(__name__)  # type: ignore
-_T = TypeVar("_T", bound="ArrowCursor")
 
 
 class ArrowCursor(BaseCursor, CursorIterator, WithResultSet):
     def __init__(
         self,
         connection: "Connection",
         converter: Converter,
@@ -36,14 +37,16 @@
         catalog_name: Optional[str] = None,
         work_group: Optional[str] = None,
         poll_interval: float = 1,
         encryption_option: Optional[str] = None,
         kms_key: Optional[str] = None,
         kill_on_interrupt: bool = True,
         unload: bool = False,
+        result_reuse_enable: bool = False,
+        result_reuse_minutes: int = CursorIterator.DEFAULT_RESULT_REUSE_MINUTES,
         **kwargs,
     ) -> None:
         super(ArrowCursor, self).__init__(
             connection=connection,
             converter=converter,
             formatter=formatter,
             retry_config=retry_config,
@@ -51,14 +54,16 @@
             schema_name=schema_name,
             catalog_name=catalog_name,
             work_group=work_group,
             poll_interval=poll_interval,
             encryption_option=encryption_option,
             kms_key=kms_key,
             kill_on_interrupt=kill_on_interrupt,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
             **kwargs,
         )
         self._unload = unload
         self._query_id: Optional[str] = None
         self._result_set: Optional[AthenaArrowResultSet] = None
 
     @staticmethod
@@ -76,15 +81,15 @@
 
     @arraysize.setter
     def arraysize(self, value: int) -> None:
         if value <= 0:
             raise ProgrammingError("arraysize must be a positive integer value.")
         self._arraysize = value
 
-    @property
+    @property  # type: ignore
     def result_set(self) -> Optional[AthenaArrowResultSet]:
         return self._result_set
 
     @result_set.setter
     def result_set(self, val) -> None:
         self._result_set = val
 
@@ -100,31 +105,30 @@
     def rownumber(self) -> Optional[int]:
         return self.result_set.rownumber if self.result_set else None
 
     def close(self) -> None:
         if self.result_set and not self.result_set.is_closed:
             self.result_set.close()
 
-    @synchronized
     def execute(
-        self: _T,
+        self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
+        result_reuse_enable: Optional[bool] = None,
+        result_reuse_minutes: Optional[int] = None,
         **kwargs,
-    ) -> _T:
+    ) -> ArrowCursor:
         self._reset_state()
         if self._unload:
             s3_staging_dir = s3_staging_dir if s3_staging_dir else self._s3_staging_dir
-            assert (
-                s3_staging_dir
-            ), "If the unload option is used, s3_staging_dir is required."
+            assert s3_staging_dir, "If the unload option is used, s3_staging_dir is required."
             operation, unload_location = self._formatter.wrap_unload(
                 operation,
                 s3_staging_dir=s3_staging_dir,
                 format_=AthenaFileFormat.FILE_FORMAT_PARQUET,
                 compression=AthenaCompression.COMPRESSION_SNAPPY,
             )
         else:
@@ -132,14 +136,16 @@
         self.query_id = self._execute(
             operation,
             parameters=parameters,
             work_group=work_group,
             s3_staging_dir=s3_staging_dir,
             cache_size=cache_size,
             cache_expiration_time=cache_expiration_time,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         query_execution = self._poll(self.query_id)
         if query_execution.state == AthenaQueryExecution.STATE_SUCCEEDED:
             self.result_set = AthenaArrowResultSet(
                 connection=self._connection,
                 converter=self._converter,
                 query_execution=query_execution,
@@ -157,46 +163,41 @@
         self, operation: str, seq_of_parameters: List[Optional[Dict[str, Any]]]
     ) -> None:
         for parameters in seq_of_parameters:
             self.execute(operation, parameters)
         # Operations that have result sets are not allowed with executemany.
         self._reset_state()
 
-    @synchronized
     def cancel(self) -> None:
         if not self.query_id:
             raise ProgrammingError("QueryExecutionId is none or empty.")
         self._cancel(self.query_id)
 
-    @synchronized
     def fetchone(
         self,
     ) -> Optional[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaArrowResultSet, self.result_set)
         return result_set.fetchone()
 
-    @synchronized
     def fetchmany(
         self, size: Optional[int] = None
     ) -> List[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaArrowResultSet, self.result_set)
         return result_set.fetchmany(size)
 
-    @synchronized
     def fetchall(
         self,
     ) -> List[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaArrowResultSet, self.result_set)
         return result_set.fetchall()
 
-    @synchronized
     def as_arrow(self) -> "Table":
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaArrowResultSet, self.result_set)
         return result_set.as_arrow()
```

### Comparing `PyAthena-2.9.6/pyathena/arrow/result_set.py` & `pyathena-3.0.0/pyathena/arrow/result_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
     from pyathena.connection import Connection
 
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
 class AthenaArrowResultSet(AthenaResultSet):
-
     DEFAULT_BLOCK_SIZE = 1024 * 1024 * 128
 
     _timestamp_parsers: List[str] = [
         "%Y-%m-%d",
         "%Y-%m-%d %H:%M:%S",
         "%Y-%m-%d %H:%M:%S %Z",
         "%Y-%m-%d %H:%M:%S %z",
@@ -83,24 +82,24 @@
         self._batches = iter(self._table.to_batches(arraysize))
 
     def __s3_file_system(self):
         from pyarrow import fs
 
         connection = self.connection
         if "role_arn" in connection._kwargs and connection._kwargs["role_arn"]:
+            external_id = connection._kwargs.get("external_id", None)
             fs = fs.S3FileSystem(
-                role_arn=connection._kwargs.get("role_arn", None),
-                session_name=connection._kwargs.get("role_session_name", None),
-                load_frequency=connection._kwargs.get("duration_seconds", None),
+                role_arn=connection._kwargs["role_arn"],
+                session_name=connection._kwargs["role_session_name"],
+                external_id="" if external_id is None else external_id,
+                load_frequency=connection._kwargs["duration_seconds"],
                 region=connection.region_name,
             )
         elif connection.profile_name:
-            profile = connection.session._session.full_config["profiles"][
-                connection.profile_name
-            ]
+            profile = connection.session._session.full_config["profiles"][connection.profile_name]
             fs = fs.S3FileSystem(
                 access_key=profile.get("aws_access_key_id", None),
                 secret_key=profile.get("aws_secret_access_key", None),
                 session_token=profile.get("aws_session_token", None),
                 region=connection.region_name,
             )
         else:
@@ -110,19 +109,15 @@
                 session_token=connection._kwargs.get("aws_session_token", None),
                 region=connection.region_name,
             )
         return fs
 
     @property
     def is_unload(self):
-        return (
-            self._unload
-            and self.query
-            and self.query.strip().upper().startswith("UNLOAD")
-        )
+        return self._unload and self.query and self.query.strip().upper().startswith("UNLOAD")
 
     @property
     def timestamp_parsers(self) -> List[str]:
         from pyarrow.csv import ISO8601
 
         return [ISO8601] + self._timestamp_parsers
 
@@ -216,17 +211,15 @@
             parse_opts = csv.ParseOptions(
                 delimiter="\t",
                 quote_char=False,
                 double_quote=False,
                 escape_char=False,
             )
         elif length and self.output_location.endswith(".csv"):
-            read_opts = csv.ReadOptions(
-                skip_rows=0, block_size=self._block_size, use_threads=True
-            )
+            read_opts = csv.ReadOptions(skip_rows=0, block_size=self._block_size, use_threads=True)
             parse_opts = csv.ParseOptions(
                 delimiter=",",
                 quote_char='"',
                 double_quote=True,
                 escape_char=False,
             )
         else:
```

### Comparing `PyAthena-2.9.6/pyathena/arrow/util.py` & `pyathena-3.0.0/pyathena/arrow/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from typing import TYPE_CHECKING, Any, Dict, Tuple, cast
 
 if TYPE_CHECKING:
     from pyarrow import Schema
     from pyarrow.lib import DataType
```

### Comparing `PyAthena-2.9.6/pyathena/async_cursor.py` & `pyathena-3.0.0/pyathena/async_cursor.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,45 +33,48 @@
         work_group: Optional[str] = None,
         poll_interval: float = 1,
         encryption_option: Optional[str] = None,
         kms_key: Optional[str] = None,
         kill_on_interrupt: bool = True,
         max_workers: int = (cpu_count() or 1) * 5,
         arraysize: int = CursorIterator.DEFAULT_FETCH_SIZE,
+        result_reuse_enable: bool = False,
+        result_reuse_minutes: int = CursorIterator.DEFAULT_RESULT_REUSE_MINUTES,
     ) -> None:
         super(AsyncCursor, self).__init__(
             connection=connection,
             converter=converter,
             formatter=formatter,
             retry_config=retry_config,
             s3_staging_dir=s3_staging_dir,
             schema_name=schema_name,
             catalog_name=catalog_name,
             work_group=work_group,
             poll_interval=poll_interval,
             encryption_option=encryption_option,
             kms_key=kms_key,
             kill_on_interrupt=kill_on_interrupt,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         self._max_workers = max_workers
         self._executor = ThreadPoolExecutor(max_workers=max_workers)
         self._arraysize = arraysize
         self._result_set_class = AthenaResultSet
 
     @property
     def arraysize(self) -> int:
         return self._arraysize
 
     @arraysize.setter
     def arraysize(self, value: int) -> None:
         if value <= 0 or value > CursorIterator.DEFAULT_FETCH_SIZE:
             raise ProgrammingError(
-                "MaxResults is more than maximum allowed length {0}.".format(
-                    CursorIterator.DEFAULT_FETCH_SIZE
-                )
+                "MaxResults is more than maximum allowed length "
+                f"{CursorIterator.DEFAULT_FETCH_SIZE}."
             )
         self._arraysize = value
 
     def close(self, wait: bool = False) -> None:
         self._executor.shutdown(wait=wait)
 
     def _description(
@@ -105,22 +108,26 @@
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
+        result_reuse_enable: Optional[bool] = None,
+        result_reuse_minutes: Optional[int] = None,
     ) -> Tuple[str, "Future[Union[AthenaResultSet, Any]]"]:
         query_id = self._execute(
             operation,
             parameters=parameters,
             work_group=work_group,
             s3_staging_dir=s3_staging_dir,
             cache_size=cache_size,
             cache_expiration_time=cache_expiration_time,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         return query_id, self._executor.submit(self._collect_result_set, query_id)
 
     def executemany(
         self, operation: str, seq_of_parameters: List[Optional[Dict[str, Any]]]
     ) -> None:
         raise NotSupportedError
```

### Comparing `PyAthena-2.9.6/pyathena/common.py` & `pyathena-3.0.0/pyathena/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,45 +5,46 @@
 from abc import ABCMeta, abstractmethod
 from datetime import datetime, timedelta, timezone
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 from pyathena.converter import Converter, DefaultTypeConverter
 from pyathena.error import DatabaseError, OperationalError, ProgrammingError
 from pyathena.formatter import Formatter
-from pyathena.model import AthenaQueryExecution, AthenaTableMetadata
+from pyathena.model import AthenaDatabase, AthenaQueryExecution, AthenaTableMetadata
 from pyathena.util import RetryConfig, retry_api_call
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection
 
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
 class CursorIterator(metaclass=ABCMeta):
-
     # https://docs.aws.amazon.com/athena/latest/APIReference/API_GetQueryResults.html
     # Valid Range: Minimum value of 1. Maximum value of 1000.
     DEFAULT_FETCH_SIZE: int = 1000
+    # https://docs.aws.amazon.com/athena/latest/APIReference/API_ResultReuseByAgeConfiguration.html
+    # Specifies, in minutes, the maximum age of a previous query result
+    # that Athena should consider for reuse. The default is 60.
+    DEFAULT_RESULT_REUSE_MINUTES = 60
 
     def __init__(self, **kwargs) -> None:
         super(CursorIterator, self).__init__()
         self.arraysize: int = kwargs.get("arraysize", self.DEFAULT_FETCH_SIZE)
         self._rownumber: Optional[int] = None
 
     @property
     def arraysize(self) -> int:
         return self._arraysize
 
     @arraysize.setter
     def arraysize(self, value: int) -> None:
         if value <= 0 or value > self.DEFAULT_FETCH_SIZE:
             raise ProgrammingError(
-                "MaxResults is more than maximum allowed length {0}.".format(
-                    self.DEFAULT_FETCH_SIZE
-                )
+                f"MaxResults is more than maximum allowed length {self.DEFAULT_FETCH_SIZE}."
             )
         self._arraysize = value
 
     @property
     def rownumber(self) -> Optional[int]:
         return self._rownumber
 
@@ -72,21 +73,23 @@
             return row
 
     def __iter__(self):
         return self
 
 
 class BaseCursor(metaclass=ABCMeta):
-
     # https://docs.aws.amazon.com/athena/latest/APIReference/API_ListQueryExecutions.html
     # Valid Range: Minimum value of 0. Maximum value of 50.
     LIST_QUERY_EXECUTIONS_MAX_RESULTS = 50
     # https://docs.aws.amazon.com/athena/latest/APIReference/API_ListTableMetadata.html
     # Valid Range: Minimum value of 1. Maximum value of 50.
     LIST_TABLE_METADATA_MAX_RESULTS = 50
+    # https://docs.aws.amazon.com/athena/latest/APIReference/API_ListDatabases.html
+    # Valid Range: Minimum value of 1. Maximum value of 50.
+    LIST_DATABASES_MAX_RESULTS = 50
 
     def __init__(
         self,
         connection: "Connection",
         converter: Converter,
         formatter: Formatter,
         retry_config: RetryConfig,
@@ -94,187 +97,327 @@
         schema_name: Optional[str],
         catalog_name: Optional[str],
         work_group: Optional[str],
         poll_interval: float,
         encryption_option: Optional[str],
         kms_key: Optional[str],
         kill_on_interrupt: bool,
-        **kwargs
+        result_reuse_enable: bool,
+        result_reuse_minutes: int,
+        **kwargs,
     ) -> None:
         super(BaseCursor, self).__init__()
         self._connection = connection
         self._converter = converter
         self._formatter = formatter
         self._retry_config = retry_config
         self._s3_staging_dir = s3_staging_dir
         self._schema_name = schema_name
         self._catalog_name = catalog_name
         self._work_group = work_group
         self._poll_interval = poll_interval
         self._encryption_option = encryption_option
         self._kms_key = kms_key
         self._kill_on_interrupt = kill_on_interrupt
+        self._result_reuse_enable = result_reuse_enable
+        self._result_reuse_minutes = result_reuse_minutes
 
     @staticmethod
     def get_default_converter(unload: bool = False) -> Union[DefaultTypeConverter, Any]:
         return DefaultTypeConverter()
 
     @property
     def connection(self) -> "Connection":
         return self._connection
 
-    def _get_query_execution(self, query_id: str) -> AthenaQueryExecution:
-        request = {"QueryExecutionId": query_id}
+    def _build_start_query_execution_request(
+        self,
+        query: str,
+        work_group: Optional[str] = None,
+        s3_staging_dir: Optional[str] = None,
+        result_reuse_enable: Optional[bool] = None,
+        result_reuse_minutes: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        request: Dict[str, Any] = {
+            "QueryString": query,
+            "QueryExecutionContext": {},
+            "ResultConfiguration": {},
+        }
+        if self._schema_name:
+            request["QueryExecutionContext"].update({"Database": self._schema_name})
+        if self._catalog_name:
+            request["QueryExecutionContext"].update({"Catalog": self._catalog_name})
+        if self._s3_staging_dir or s3_staging_dir:
+            request["ResultConfiguration"].update(
+                {"OutputLocation": s3_staging_dir if s3_staging_dir else self._s3_staging_dir}
+            )
+        if self._work_group or work_group:
+            request.update({"WorkGroup": work_group if work_group else self._work_group})
+        if self._encryption_option:
+            enc_conf = {
+                "EncryptionOption": self._encryption_option,
+            }
+            if self._kms_key:
+                enc_conf.update({"KmsKey": self._kms_key})
+            request["ResultConfiguration"].update({"EncryptionConfiguration": enc_conf})
+        if self._result_reuse_enable or result_reuse_enable:
+            reuse_conf = {
+                "Enabled": result_reuse_enable
+                if result_reuse_enable is not None
+                else self._result_reuse_enable,
+                "MaxAgeInMinutes": result_reuse_minutes
+                if result_reuse_minutes is not None
+                else self._result_reuse_minutes,
+            }
+            request["ResultReuseConfiguration"] = {"ResultReuseByAgeConfiguration": reuse_conf}
+        return request
+
+    def _build_list_query_executions_request(
+        self,
+        work_group: Optional[str],
+        next_token: Optional[str] = None,
+        max_results: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        request: Dict[str, Any] = {
+            "MaxResults": max_results if max_results else self.LIST_QUERY_EXECUTIONS_MAX_RESULTS
+        }
+        if self._work_group or work_group:
+            request.update({"WorkGroup": work_group if work_group else self._work_group})
+        if next_token:
+            request.update({"NextToken": next_token})
+        return request
+
+    def _build_list_table_metadata_request(
+        self,
+        catalog_name: Optional[str],
+        schema_name: Optional[str],
+        expression: Optional[str] = None,
+        next_token: Optional[str] = None,
+        max_results: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        request: Dict[str, Any] = {
+            "CatalogName": catalog_name if catalog_name else self._catalog_name,
+            "DatabaseName": schema_name if schema_name else self._schema_name,
+            "MaxResults": max_results if max_results else self.LIST_TABLE_METADATA_MAX_RESULTS,
+        }
+        if expression:
+            request.update({"Expression": expression})
+        if next_token:
+            request.update({"NextToken": next_token})
+        return request
+
+    def _build_list_databases_request(
+        self,
+        catalog_name: Optional[str],
+        next_token: Optional[str] = None,
+        max_results: Optional[int] = None,
+    ):
+        request: Dict[str, Any] = {
+            "CatalogName": catalog_name if catalog_name else self._catalog_name,
+            "MaxResults": max_results if max_results else self.LIST_DATABASES_MAX_RESULTS,
+        }
+        if next_token:
+            request.update({"NextToken": next_token})
+        return request
+
+    def _list_databases(
+        self,
+        catalog_name: Optional[str],
+        next_token: Optional[str] = None,
+        max_results: Optional[int] = None,
+    ) -> Tuple[Optional[str], List[AthenaDatabase]]:
+        request = self._build_list_databases_request(
+            catalog_name=catalog_name,
+            next_token=next_token,
+            max_results=max_results,
+        )
         try:
             response = retry_api_call(
-                self._connection.client.get_query_execution,
+                self.connection._client.list_databases,
                 config=self._retry_config,
                 logger=_logger,
-                **request
+                **request,
             )
         except Exception as e:
-            _logger.exception("Failed to get query execution.")
+            _logger.exception("Failed to list databases.")
             raise OperationalError(*e.args) from e
         else:
-            return AthenaQueryExecution(response)
+            return response.get("NextToken", None), [
+                AthenaDatabase({"Database": r}) for r in response.get("DatabaseList", [])
+            ]
+
+    def list_databases(
+        self,
+        catalog_name: Optional[str],
+        max_results: Optional[int] = None,
+    ) -> List[AthenaDatabase]:
+        databases = []
+        next_token = None
+        while True:
+            next_token, response = self._list_databases(
+                catalog_name=catalog_name,
+                next_token=next_token,
+                max_results=max_results,
+            )
+            databases.extend(response)
+            if not next_token:
+                break
+        return databases
 
     def _get_table_metadata(
         self,
         table_name: str,
         catalog_name: Optional[str] = None,
         schema_name: Optional[str] = None,
+        logging_: bool = True,
     ) -> AthenaTableMetadata:
         request = {
             "CatalogName": catalog_name if catalog_name else self._catalog_name,
             "DatabaseName": schema_name if schema_name else self._schema_name,
             "TableName": table_name,
         }
         try:
             response = retry_api_call(
                 self._connection.client.get_table_metadata,
                 config=self._retry_config,
                 logger=_logger,
-                **request
+                **request,
             )
         except Exception as e:
-            _logger.exception("Failed to get table metadata.")
+            if logging_:
+                _logger.exception("Failed to get table metadata.")
             raise OperationalError(*e.args) from e
         else:
             return AthenaTableMetadata(response)
 
     def get_table_metadata(
         self,
         table_name: str,
         catalog_name: Optional[str] = None,
         schema_name: Optional[str] = None,
+        logging_: bool = True,
     ) -> AthenaTableMetadata:
         return self._get_table_metadata(
             table_name=table_name,
             catalog_name=catalog_name,
             schema_name=schema_name,
+            logging_=logging_,
         )
 
-    def _batch_get_query_execution(
-        self, query_ids: List[str]
-    ) -> List[AthenaQueryExecution]:
-        try:
-            response = retry_api_call(
-                self.connection._client.batch_get_query_execution,
-                config=self._retry_config,
-                logger=_logger,
-                QueryExecutionIds=query_ids,
-            )
-        except Exception as e:
-            _logger.exception("Failed to batch get query execution.")
-            raise OperationalError(*e.args) from e
-        else:
-            return [
-                AthenaQueryExecution({"QueryExecution": r})
-                for r in response.get("QueryExecutions", [])
-            ]
-
-    def _list_query_executions(
-        self,
-        max_results: Optional[int] = None,
-        work_group: Optional[str] = None,
-        next_token: Optional[str] = None,
-    ) -> Tuple[Optional[str], List[AthenaQueryExecution]]:
-        request = self._build_list_query_executions_request(
-            max_results=max_results, work_group=work_group, next_token=next_token
-        )
-        try:
-            response = retry_api_call(
-                self.connection._client.list_query_executions,
-                config=self._retry_config,
-                logger=_logger,
-                **request
-            )
-        except Exception as e:
-            _logger.exception("Failed to list query executions.")
-            raise OperationalError(*e.args) from e
-        else:
-            next_token = response.get("NextToken", None)
-            query_ids = response.get("QueryExecutionIds", None)
-            if not query_ids:
-                return next_token, []
-            return next_token, self._batch_get_query_execution(query_ids)
-
     def _list_table_metadata(
         self,
-        max_results: Optional[int] = None,
         catalog_name: Optional[str] = None,
         schema_name: Optional[str] = None,
         expression: Optional[str] = None,
         next_token: Optional[str] = None,
+        max_results: Optional[int] = None,
     ) -> Tuple[Optional[str], List[AthenaTableMetadata]]:
         request = self._build_list_table_metadata_request(
-            max_results=max_results,
             catalog_name=catalog_name,
             schema_name=schema_name,
             expression=expression,
             next_token=next_token,
+            max_results=max_results,
         )
         try:
             response = retry_api_call(
                 self.connection._client.list_table_metadata,
                 config=self._retry_config,
                 logger=_logger,
-                **request
+                **request,
             )
         except Exception as e:
             _logger.exception("Failed to list table metadata.")
             raise OperationalError(*e.args) from e
         else:
             return response.get("NextToken", None), [
                 AthenaTableMetadata({"TableMetadata": r})
                 for r in response.get("TableMetadataList", [])
             ]
 
     def list_table_metadata(
         self,
-        max_results: Optional[int] = None,
         catalog_name: Optional[str] = None,
         schema_name: Optional[str] = None,
         expression: Optional[str] = None,
+        max_results: Optional[int] = None,
     ) -> List[AthenaTableMetadata]:
         metadata = []
         next_token = None
         while True:
             next_token, response = self._list_table_metadata(
-                max_results=max_results,
                 catalog_name=catalog_name,
                 schema_name=schema_name,
                 expression=expression,
                 next_token=next_token,
+                max_results=max_results,
             )
             metadata.extend(response)
             if not next_token:
                 break
         return metadata
 
+    def _get_query_execution(self, query_id: str) -> AthenaQueryExecution:
+        request = {"QueryExecutionId": query_id}
+        try:
+            response = retry_api_call(
+                self._connection.client.get_query_execution,
+                config=self._retry_config,
+                logger=_logger,
+                **request,
+            )
+        except Exception as e:
+            _logger.exception("Failed to get query execution.")
+            raise OperationalError(*e.args) from e
+        else:
+            return AthenaQueryExecution(response)
+
+    def _batch_get_query_execution(self, query_ids: List[str]) -> List[AthenaQueryExecution]:
+        try:
+            response = retry_api_call(
+                self.connection._client.batch_get_query_execution,
+                config=self._retry_config,
+                logger=_logger,
+                QueryExecutionIds=query_ids,
+            )
+        except Exception as e:
+            _logger.exception("Failed to batch get query execution.")
+            raise OperationalError(*e.args) from e
+        else:
+            return [
+                AthenaQueryExecution({"QueryExecution": r})
+                for r in response.get("QueryExecutions", [])
+            ]
+
+    def _list_query_executions(
+        self,
+        work_group: Optional[str] = None,
+        next_token: Optional[str] = None,
+        max_results: Optional[int] = None,
+    ) -> Tuple[Optional[str], List[AthenaQueryExecution]]:
+        request = self._build_list_query_executions_request(
+            work_group=work_group, next_token=next_token, max_results=max_results
+        )
+        try:
+            response = retry_api_call(
+                self.connection._client.list_query_executions,
+                config=self._retry_config,
+                logger=_logger,
+                **request,
+            )
+        except Exception as e:
+            _logger.exception("Failed to list query executions.")
+            raise OperationalError(*e.args) from e
+        else:
+            next_token = response.get("NextToken", None)
+            query_ids = response.get("QueryExecutionIds", None)
+            if not query_ids:
+                return next_token, []
+            return next_token, self._batch_get_query_execution(query_ids)
+
     def __poll(self, query_id: str) -> AthenaQueryExecution:
         while True:
             query_execution = self._get_query_execution(query_id)
             if query_execution.state in [
                 AthenaQueryExecution.STATE_SUCCEEDED,
                 AthenaQueryExecution.STATE_FAILED,
                 AthenaQueryExecution.STATE_CANCELLED,
@@ -291,113 +434,35 @@
                 _logger.warning("Query canceled by user.")
                 self._cancel(query_id)
                 query_execution = self.__poll(query_id)
             else:
                 raise e
         return query_execution
 
-    def _build_start_query_execution_request(
-        self,
-        query: str,
-        work_group: Optional[str] = None,
-        s3_staging_dir: Optional[str] = None,
-    ) -> Dict[str, Any]:
-        request: Dict[str, Any] = {
-            "QueryString": query,
-            "QueryExecutionContext": {},
-            "ResultConfiguration": {},
-        }
-        if self._schema_name:
-            request["QueryExecutionContext"].update({"Database": self._schema_name})
-        if self._catalog_name:
-            request["QueryExecutionContext"].update({"Catalog": self._catalog_name})
-        if self._s3_staging_dir or s3_staging_dir:
-            request["ResultConfiguration"].update(
-                {
-                    "OutputLocation": s3_staging_dir
-                    if s3_staging_dir
-                    else self._s3_staging_dir
-                }
-            )
-        if self._work_group or work_group:
-            request.update(
-                {"WorkGroup": work_group if work_group else self._work_group}
-            )
-        if self._encryption_option:
-            enc_conf = {
-                "EncryptionOption": self._encryption_option,
-            }
-            if self._kms_key:
-                enc_conf.update({"KmsKey": self._kms_key})
-            request["ResultConfiguration"].update({"EncryptionConfiguration": enc_conf})
-        return request
-
-    def _build_list_query_executions_request(
-        self,
-        max_results: Optional[int],
-        work_group: Optional[str],
-        next_token: Optional[str] = None,
-    ) -> Dict[str, Any]:
-        request: Dict[str, Any] = {
-            "MaxResults": max_results
-            if max_results
-            else self.LIST_QUERY_EXECUTIONS_MAX_RESULTS
-        }
-        if self._work_group or work_group:
-            request.update(
-                {"WorkGroup": work_group if work_group else self._work_group}
-            )
-        if next_token:
-            request.update({"NextToken": next_token})
-        return request
-
-    def _build_list_table_metadata_request(
-        self,
-        max_results: Optional[int],
-        catalog_name: Optional[str],
-        schema_name: Optional[str],
-        expression: Optional[str] = None,
-        next_token: Optional[str] = None,
-    ) -> Dict[str, Any]:
-        request: Dict[str, Any] = {
-            "MaxResults": max_results
-            if max_results
-            else self.LIST_TABLE_METADATA_MAX_RESULTS,
-            "CatalogName": catalog_name if catalog_name else self._catalog_name,
-            "DatabaseName": schema_name if schema_name else self._schema_name,
-        }
-        if expression:
-            request.update({"Expression": expression})
-        if next_token:
-            request.update({"NextToken": next_token})
-        return request
-
     def _find_previous_query_id(
         self,
         query: str,
         work_group: Optional[str],
         cache_size: int = 0,
         cache_expiration_time: int = 0,
     ) -> Optional[str]:
         query_id = None
         if cache_size == 0 and cache_expiration_time > 0:
             cache_size = sys.maxsize
         if cache_expiration_time > 0:
-            expiration_time = datetime.now(timezone.utc) - timedelta(
-                seconds=cache_expiration_time
-            )
+            expiration_time = datetime.now(timezone.utc) - timedelta(seconds=cache_expiration_time)
         else:
             expiration_time = datetime.now(timezone.utc)
         try:
             next_token = None
             while cache_size > 0:
                 max_results = min(cache_size, self.LIST_QUERY_EXECUTIONS_MAX_RESULTS)
                 cache_size -= max_results
                 next_token, query_executions = self._list_query_executions(
-                    max_results, work_group, next_token=next_token
+                    work_group, next_token=next_token, max_results=max_results
                 )
                 for execution in sorted(
                     (
                         e
                         for e in query_executions
                         if e.state == AthenaQueryExecution.STATE_SUCCEEDED
                         and e.statement_type == AthenaQueryExecution.STATEMENT_TYPE_DML
@@ -416,47 +481,51 @@
                         break
                     if execution.query == query:
                         query_id = execution.query_id
                         break
                 if query_id or next_token is None:
                     break
         except Exception:
-            _logger.warning(
-                "Failed to check the cache. Moving on without cache.", exc_info=True
-            )
+            _logger.warning("Failed to check the cache. Moving on without cache.", exc_info=True)
         return query_id
 
     def _execute(
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
+        result_reuse_enable: Optional[bool] = None,
+        result_reuse_minutes: Optional[int] = None,
     ) -> str:
         query = self._formatter.format(operation, parameters)
         _logger.debug(query)
 
         request = self._build_start_query_execution_request(
-            query, work_group, s3_staging_dir
+            query=query,
+            work_group=work_group,
+            s3_staging_dir=s3_staging_dir,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         query_id = self._find_previous_query_id(
             query,
             work_group,
             cache_size=cache_size,
             cache_expiration_time=cache_expiration_time,
         )
         if query_id is None:
             try:
                 query_id = retry_api_call(
                     self._connection.client.start_query_execution,
                     config=self._retry_config,
                     logger=_logger,
-                    **request
+                    **request,
                 ).get("QueryExecutionId", None)
             except Exception as e:
                 _logger.exception("Failed to execute query.")
                 raise DatabaseError(*e.args) from e
         return query_id
 
     @abstractmethod
@@ -464,14 +533,16 @@
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
+        result_reuse_enable: Optional[bool] = None,
+        result_reuse_minutes: Optional[int] = None,
     ):
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     def executemany(
         self, operation: str, seq_of_parameters: List[Optional[Dict[str, Any]]]
     ) -> None:
@@ -484,15 +555,15 @@
     def _cancel(self, query_id: str) -> None:
         request = {"QueryExecutionId": query_id}
         try:
             retry_api_call(
                 self._connection.client.stop_query_execution,
                 config=self._retry_config,
                 logger=_logger,
-                **request
+                **request,
             )
         except Exception as e:
             _logger.exception("Failed to cancel query.")
             raise OperationalError(*e.args) from e
 
     def setinputsizes(self, sizes):
         """Does nothing by default"""
```

### Comparing `PyAthena-2.9.6/pyathena/connection.py` & `pyathena-3.0.0/pyathena/connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,86 @@
 # -*- coding: utf-8 -*-
 import logging
 import os
 import time
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type
 
 from boto3.session import Session
+from botocore.config import Config
 
-from pyathena.common import BaseCursor
+import pyathena
+from pyathena.common import BaseCursor, CursorIterator
 from pyathena.converter import Converter
 from pyathena.cursor import Cursor
 from pyathena.error import NotSupportedError
 from pyathena.formatter import DefaultParameterFormatter, Formatter
 from pyathena.util import RetryConfig
 
 if TYPE_CHECKING:
     from botocore.client import BaseClient
 
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
 class Connection:
-
     _ENV_S3_STAGING_DIR: str = "AWS_ATHENA_S3_STAGING_DIR"
     _ENV_WORK_GROUP: str = "AWS_ATHENA_WORK_GROUP"
     _SESSION_PASSING_ARGS: List[str] = [
         "aws_access_key_id",
         "aws_secret_access_key",
         "aws_session_token",
         "region_name",
         "botocore_session",
         "profile_name",
     ]
     _CLIENT_PASSING_ARGS: List[str] = [
         "aws_access_key_id",
         "aws_secret_access_key",
         "aws_session_token",
-        "config",
         "api_version",
         "use_ssl",
         "verify",
         "endpoint_url",
+        "region_name",
+        "config",
     ]
 
     def __init__(
         self,
         s3_staging_dir: Optional[str] = None,
         region_name: Optional[str] = None,
         schema_name: Optional[str] = "default",
         catalog_name: Optional[str] = "awsdatacatalog",
         work_group: Optional[str] = None,
         poll_interval: float = 1,
         encryption_option: Optional[str] = None,
         kms_key: Optional[str] = None,
         profile_name: Optional[str] = None,
         role_arn: Optional[str] = None,
-        role_session_name: str = "PyAthena-session-{0}".format(int(time.time())),
+        role_session_name: str = f"PyAthena-session-{int(time.time())}",
+        external_id: Optional[str] = None,
         serial_number: Optional[str] = None,
         duration_seconds: int = 3600,
         converter: Optional[Converter] = None,
         formatter: Optional[Formatter] = None,
         retry_config: Optional[RetryConfig] = None,
         cursor_class: Type[BaseCursor] = Cursor,
         cursor_kwargs: Optional[Dict[str, Any]] = None,
         kill_on_interrupt: bool = True,
         session: Optional[Session] = None,
-        **kwargs
+        config: Optional[Config] = None,
+        result_reuse_enable: bool = False,
+        result_reuse_minutes: int = CursorIterator.DEFAULT_RESULT_REUSE_MINUTES,
+        **kwargs,
     ) -> None:
         self._kwargs = {
             **kwargs,
             "role_arn": role_arn,
             "role_session_name": role_session_name,
+            "external_id": external_id,
             "serial_number": serial_number,
             "duration_seconds": duration_seconds,
         }
         if s3_staging_dir:
             self.s3_staging_dir: Optional[str] = s3_staging_dir
         else:
             self.s3_staging_dir = os.getenv(self._ENV_S3_STAGING_DIR, None)
@@ -84,28 +91,30 @@
             self.work_group: Optional[str] = work_group
         else:
             self.work_group = os.getenv(self._ENV_WORK_GROUP, None)
         self.poll_interval = poll_interval
         self.encryption_option = encryption_option
         self.kms_key = kms_key
         self.profile_name = profile_name
+        self.config: Optional[Config] = config if config else Config()
 
         assert (
             self.s3_staging_dir or self.work_group
         ), "Required argument `s3_staging_dir` or `work_group` not found."
 
         if session:
             self._session = session
         else:
             if role_arn:
                 creds = self._assume_role(
                     profile_name=self.profile_name,
                     region_name=self.region_name,
                     role_arn=role_arn,
                     role_session_name=role_session_name,
+                    external_id=external_id,
                     serial_number=serial_number,
                     duration_seconds=duration_seconds,
                 )
                 self.profile_name = None
                 self._kwargs.update(
                     {
                         "aws_access_key_id": creds["AccessKeyId"],
@@ -127,44 +136,63 @@
                         "aws_secret_access_key": creds["SecretAccessKey"],
                         "aws_session_token": creds["SessionToken"],
                     }
                 )
             self._session = Session(
                 region_name=self.region_name,
                 profile_name=self.profile_name,
-                **self._session_kwargs
+                **self._session_kwargs,
+            )
+
+        if not self.config.user_agent_extra or (
+            pyathena.user_agent_extra not in self.config.user_agent_extra
+        ):
+            self.config.user_agent_extra = (
+                f"{pyathena.user_agent_extra}"
+                f"{' ' + self.config.user_agent_extra if self.config.user_agent_extra else ''}"
             )
         self._client = self._session.client(
-            "athena", region_name=self.region_name, **self._client_kwargs
+            "athena", region_name=self.region_name, config=self.config, **self._client_kwargs
         )
         self._converter = converter
         self._formatter = formatter if formatter else DefaultParameterFormatter()
         self._retry_config = retry_config if retry_config else RetryConfig()
         self.cursor_class = cursor_class
         self.cursor_kwargs = cursor_kwargs if cursor_kwargs else dict()
         self.kill_on_interrupt = kill_on_interrupt
+        self.result_reuse_enable = result_reuse_enable
+        self.result_reuse_minutes = result_reuse_minutes
 
     def _assume_role(
         self,
         profile_name: Optional[str],
         region_name: Optional[str],
-        role_arn: Optional[str],
+        role_arn: str,
         role_session_name: str,
+        external_id: Optional[str],
         serial_number: Optional[str],
         duration_seconds: int,
     ) -> Dict[str, Any]:
         session = Session(
             region_name=region_name, profile_name=profile_name, **self._session_kwargs
         )
-        client = session.client("sts", region_name=region_name, **self._client_kwargs)
+        client = session.client(
+            "sts", region_name=region_name, config=self.config, **self._client_kwargs
+        )
         request = {
             "RoleArn": role_arn,
             "RoleSessionName": role_session_name,
             "DurationSeconds": duration_seconds,
         }
+        if external_id:
+            request.update(
+                {
+                    "ExternalId": external_id,
+                }
+            )
         if serial_number:
             token_code = input("Enter the MFA code: ")
             request.update(
                 {
                     "SerialNumber": serial_number,
                     "TokenCode": token_code,
                 }
@@ -177,30 +205,30 @@
         self,
         profile_name: Optional[str],
         region_name: Optional[str],
         serial_number: Optional[str],
         duration_seconds: int,
     ) -> Dict[str, Any]:
         session = Session(profile_name=profile_name, **self._session_kwargs)
-        client = session.client("sts", region_name=region_name, **self._client_kwargs)
+        client = session.client(
+            "sts", region_name=region_name, config=self.config, **self._client_kwargs
+        )
         token_code = input("Enter the MFA code: ")
         request = {
             "DurationSeconds": duration_seconds,
             "SerialNumber": serial_number,
             "TokenCode": token_code,
         }
         response = client.get_session_token(**request)
         creds: Dict[str, Any] = response["Credentials"]
         return creds
 
     @property
     def _session_kwargs(self) -> Dict[str, Any]:
-        return {
-            k: v for k, v in self._kwargs.items() if k in self._SESSION_PASSING_ARGS
-        }
+        return {k: v for k, v in self._kwargs.items() if k in self._SESSION_PASSING_ARGS}
 
     @property
     def _client_kwargs(self) -> Dict[str, Any]:
         return {k: v for k, v in self._kwargs.items() if k in self._CLIENT_PASSING_ARGS}
 
     @property
     def session(self) -> Session:
@@ -236,15 +264,17 @@
             schema_name=kwargs.pop("schema_name", self.schema_name),
             catalog_name=kwargs.pop("catalog_name", self.catalog_name),
             work_group=kwargs.pop("work_group", self.work_group),
             poll_interval=kwargs.pop("poll_interval", self.poll_interval),
             encryption_option=kwargs.pop("encryption_option", self.encryption_option),
             kms_key=kwargs.pop("kms_key", self.kms_key),
             kill_on_interrupt=kwargs.pop("kill_on_interrupt", self.kill_on_interrupt),
-            **kwargs
+            result_reuse_enable=kwargs.pop("result_reuse_enable", self.result_reuse_enable),
+            result_reuse_minutes=kwargs.pop("result_reuse_minutes", self.result_reuse_minutes),
+            **kwargs,
         )
 
     def close(self) -> None:
         pass
 
     def commit(self) -> None:
         pass
```

### Comparing `PyAthena-2.9.6/pyathena/converter.py` & `pyathena-3.0.0/pyathena/converter.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 
 class Converter(metaclass=ABCMeta):
     def __init__(
         self,
         mappings: Dict[str, Callable[[Optional[str]], Optional[Any]]],
         default: Callable[[Optional[str]], Optional[Any]] = _to_default,
-        types: Dict[str, Type[Any]] = None,
+        types: Optional[Dict[str, Type[Any]]] = None,
     ) -> None:
         if mappings:
             self._mappings = mappings
         else:
             self._mappings = dict()
         self._default = default
         if types:
@@ -118,25 +118,21 @@
     @property
     def types(self) -> Dict[str, Type[Any]]:
         return self._types
 
     def get(self, type_: str) -> Callable[[Optional[str]], Optional[Any]]:
         return self.mappings.get(type_, self._default)
 
-    def set(
-        self, type_: str, converter: Callable[[Optional[str]], Optional[Any]]
-    ) -> None:
+    def set(self, type_: str, converter: Callable[[Optional[str]], Optional[Any]]) -> None:
         self.mappings[type_] = converter
 
     def remove(self, type_: str) -> None:
         self.mappings.pop(type_, None)
 
-    def update(
-        self, mappings: Dict[str, Callable[[Optional[str]], Optional[Any]]]
-    ) -> None:
+    def update(self, mappings: Dict[str, Callable[[Optional[str]], Optional[Any]]]) -> None:
         self.mappings.update(mappings)
 
     @abstractmethod
     def convert(self, type_: str, value: Optional[str]) -> Optional[Any]:
         raise NotImplementedError  # pragma: no cover
```

### Comparing `PyAthena-2.9.6/pyathena/cursor.py` & `pyathena-3.0.0/pyathena/cursor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 
 from pyathena.common import BaseCursor, CursorIterator
 from pyathena.converter import Converter
 from pyathena.error import OperationalError, ProgrammingError
 from pyathena.formatter import Formatter
 from pyathena.model import AthenaQueryExecution
 from pyathena.result_set import AthenaDictResultSet, AthenaResultSet, WithResultSet
-from pyathena.util import RetryConfig, synchronized
+from pyathena.util import RetryConfig
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection
 
 _logger = logging.getLogger(__name__)  # type: ignore
-_T = TypeVar("_T", bound="Cursor")
 
 
 class Cursor(BaseCursor, CursorIterator, WithResultSet):
     def __init__(
         self,
         connection: "Connection",
         converter: Converter,
@@ -28,30 +29,34 @@
         schema_name: Optional[str] = None,
         catalog_name: Optional[str] = None,
         work_group: Optional[str] = None,
         poll_interval: float = 1,
         encryption_option: Optional[str] = None,
         kms_key: Optional[str] = None,
         kill_on_interrupt: bool = True,
-        **kwargs
+        result_reuse_enable: bool = False,
+        result_reuse_minutes: int = CursorIterator.DEFAULT_RESULT_REUSE_MINUTES,
+        **kwargs,
     ) -> None:
         super(Cursor, self).__init__(
             connection=connection,
             converter=converter,
             formatter=formatter,
             retry_config=retry_config,
             s3_staging_dir=s3_staging_dir,
             schema_name=schema_name,
             catalog_name=catalog_name,
             work_group=work_group,
             poll_interval=poll_interval,
             encryption_option=encryption_option,
             kms_key=kms_key,
             kill_on_interrupt=kill_on_interrupt,
-            **kwargs
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
+            **kwargs,
         )
         self._query_id: Optional[str] = None
         self._result_set: Optional[AthenaResultSet] = None
         self._result_set_class = AthenaResultSet
 
     @property
     def result_set(self) -> Optional[AthenaResultSet]:
@@ -73,32 +78,35 @@
     def rownumber(self) -> Optional[int]:
         return self.result_set.rownumber if self.result_set else None
 
     def close(self) -> None:
         if self.result_set and not self.result_set.is_closed:
             self.result_set.close()
 
-    @synchronized
     def execute(
-        self: _T,
+        self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
-    ) -> _T:
+        result_reuse_enable: Optional[bool] = None,
+        result_reuse_minutes: Optional[int] = None,
+    ) -> Cursor:
         self._reset_state()
         self.query_id = self._execute(
             operation,
             parameters=parameters,
             work_group=work_group,
             s3_staging_dir=s3_staging_dir,
             cache_size=cache_size,
             cache_expiration_time=cache_expiration_time,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         query_execution = self._poll(self.query_id)
         if query_execution.state == AthenaQueryExecution.STATE_SUCCEEDED:
             self.result_set = self._result_set_class(
                 self._connection,
                 self._converter,
                 query_execution,
@@ -113,39 +121,35 @@
         self, operation: str, seq_of_parameters: List[Optional[Dict[str, Any]]]
     ) -> None:
         for parameters in seq_of_parameters:
             self.execute(operation, parameters)
         # Operations that have result sets are not allowed with executemany.
         self._reset_state()
 
-    @synchronized
     def cancel(self) -> None:
         if not self.query_id:
             raise ProgrammingError("QueryExecutionId is none or empty.")
         self._cancel(self.query_id)
 
-    @synchronized
     def fetchone(
         self,
     ) -> Optional[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.fetchone()
 
-    @synchronized
     def fetchmany(
-        self, size: int = None
+        self, size: Optional[int] = None
     ) -> List[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.fetchmany(size)
 
-    @synchronized
     def fetchall(
         self,
     ) -> List[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.fetchall()
```

### Comparing `PyAthena-2.9.6/pyathena/error.py` & `pyathena-3.0.0/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `PyAthena-2.9.6/pyathena/formatter.py` & `pyathena-3.0.0/pyathena/formatter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
 import textwrap
 import uuid
 from abc import ABCMeta, abstractmethod
 from copy import deepcopy
 from datetime import date, datetime
 from decimal import Decimal
-from typing import Any, Callable, Dict, Optional, Type, TypeVar
+from typing import Any, Callable, Dict, Optional, Type
 
 from pyathena.error import ProgrammingError
 from pyathena.model import AthenaCompression, AthenaFileFormat
 
 _logger = logging.getLogger(__name__)  # type: ignore
-_T = TypeVar("_T", bound="Formatter")
 
 
 class Formatter(metaclass=ABCMeta):
     def __init__(
         self,
-        mappings: Dict[Type[Any], Callable[[_T, Callable[[str], str], Any], Any]],
-        default: Callable[[_T, Callable[[str], str], Any], Any] = None,
+        mappings: Dict[Type[Any], Callable[[Formatter, Callable[[str], str], Any], Any]],
+        default: Optional[Callable[[Formatter, Callable[[str], str], Any], Any]] = None,
     ) -> None:
         self._mappings = mappings
         self._default = default
 
     @property
     def mappings(
         self,
-    ) -> Dict[Type[Any], Callable[[_T, Callable[[str], str], Any], Any]]:
+    ) -> Dict[Type[Any], Callable[[Formatter, Callable[[str], str], Any], Any]]:
         return self._mappings
 
-    def get(self, type_) -> Optional[Callable[[_T, Callable[[str], str], Any], Any]]:
+    def get(self, type_) -> Optional[Callable[[Formatter, Callable[[str], str], Any], Any]]:
         return self.mappings.get(type(type_), self._default)
 
     def set(
         self,
         type_: Type[Any],
-        formatter: Callable[[_T, Callable[[str], str], Any], Any],
+        formatter: Callable[[Formatter, Callable[[str], str], Any], Any],
     ) -> None:
         self.mappings[type_] = formatter
 
     def remove(self, type_: Type[Any]) -> None:
         self.mappings.pop(type_, None)
 
     def update(
-        self, mappings: Dict[Type[Any], Callable[[_T, Callable[[str], str], Any], Any]]
+        self, mappings: Dict[Type[Any], Callable[[Formatter, Callable[[str], str], Any], Any]]
     ) -> None:
         self.mappings.update(mappings)
 
     @abstractmethod
-    def format(
-        self, operation: str, parameters: Optional[Dict[str, Any]] = None
-    ) -> str:
+    def format(self, operation: str, parameters: Optional[Dict[str, Any]] = None) -> str:
         raise NotImplementedError  # pragma: no cover
 
     @staticmethod
     def wrap_unload(
         operation: str,
         s3_staging_dir: str,
         format_: str = AthenaFileFormat.FILE_FORMAT_PARQUET,
@@ -82,51 +81,43 @@
             )
         else:
             location = None
         return operation, location
 
 
 def _escape_presto(val: str) -> str:
-    """ParamEscaper
-
-    https://github.com/dropbox/PyHive/blob/master/pyhive/common.py"""
-    return "'{0}'".format(val.replace("'", "''"))
+    escaped = val.replace("'", "''")
+    return f"'{escaped}'"
 
 
 def _escape_hive(val: str) -> str:
-    """HiveParamEscaper
-
-    https://github.com/dropbox/PyHive/blob/master/pyhive/hive.py"""
-    return "'{0}'".format(
+    escaped = (
         val.replace("\\", "\\\\")
         .replace("'", "\\'")
         .replace("\r", "\\r")
         .replace("\n", "\\n")
         .replace("\t", "\\t")
     )
+    return f"'{escaped}'"
 
 
 def _format_none(formatter: Formatter, escaper: Callable[[str], str], val: Any) -> Any:
     return "null"
 
 
-def _format_default(
-    formatter: Formatter, escaper: Callable[[str], str], val: Any
-) -> Any:
+def _format_default(formatter: Formatter, escaper: Callable[[str], str], val: Any) -> Any:
     return val
 
 
 def _format_date(formatter: Formatter, escaper: Callable[[str], str], val: Any) -> Any:
-    return "DATE '{0}'".format(val.strftime("%Y-%m-%d"))
+    return f"DATE '{val:%Y-%m-%d}'"
 
 
-def _format_datetime(
-    formatter: Formatter, escaper: Callable[[str], str], val: Any
-) -> Any:
-    return "TIMESTAMP '{0}'".format(val.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3])
+def _format_datetime(formatter: Formatter, escaper: Callable[[str], str], val: Any) -> Any:
+    return f"""TIMESTAMP '{val.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]}'"""
 
 
 def _format_bool(formatter: Formatter, escaper: Callable[[str], str], val: Any) -> Any:
     return str(val)
 
 
 def _format_str(formatter: Formatter, escaper: Callable[[str], str], val: Any) -> Any:
@@ -134,44 +125,41 @@
 
 
 def _format_seq(formatter: Formatter, escaper: Callable[[str], str], val: Any) -> Any:
     results = []
     for v in val:
         func = formatter.get(v)
         if not func:
-            raise TypeError("{0} is not defined formatter.".format(type(v)))
+            raise TypeError(f"{type(v)} is not defined formatter.")
         formatted = func(formatter, escaper, v)
         if not isinstance(
             formatted,
             (str,),
         ):
             # force string format
             if isinstance(
                 formatted,
                 (
                     float,
                     Decimal,
                 ),
             ):
-                formatted = "{0:f}".format(formatted)
+                formatted = f"{formatted:f}"
             else:
-                formatted = "{0}".format(formatted)
+                formatted = f"{formatted}"
         results.append(formatted)
-    return "({0})".format(", ".join(results))
+    return f"""({", ".join(results)})"""
 
 
-def _format_decimal(
-    formatter: Formatter, escaper: Callable[[str], str], val: Any
-) -> Any:
-    return "DECIMAL {0}".format(escaper("{0:f}".format(val)))
+def _format_decimal(formatter: Formatter, escaper: Callable[[str], str], val: Any) -> Any:
+    escaped = escaper(f"{val:f}")
+    return f"DECIMAL {escaped}"
 
 
-_DEFAULT_FORMATTERS: Dict[
-    Type[Any], Callable[[Formatter, Callable[[str], str], Any], Any]
-] = {
+_DEFAULT_FORMATTERS: Dict[Type[Any], Callable[[Formatter, Callable[[str], str], Any], Any]] = {
     type(None): _format_none,
     date: _format_date,
     datetime: _format_datetime,
     int: _format_default,
     float: _format_default,
     Decimal: _format_decimal,
     bool: _format_bool,
@@ -184,17 +172,15 @@
 
 class DefaultParameterFormatter(Formatter):
     def __init__(self) -> None:
         super(DefaultParameterFormatter, self).__init__(
             mappings=deepcopy(_DEFAULT_FORMATTERS), default=None
         )
 
-    def format(
-        self, operation: str, parameters: Optional[Dict[str, Any]] = None
-    ) -> str:
+    def format(self, operation: str, parameters: Optional[Dict[str, Any]] = None) -> str:
         if not operation or not operation.strip():
             raise ProgrammingError("Query is none or empty.")
         operation = operation.strip()
 
         operation_upper = operation.upper()
         if (
             operation_upper.startswith("SELECT")
@@ -204,20 +190,21 @@
             escaper = _escape_presto
         else:
             escaper = _escape_hive
 
         kwargs: Optional[Dict[str, Any]] = None
         if parameters is not None:
             kwargs = dict()
-            if isinstance(parameters, dict):
+            if not parameters:
+                pass
+            elif isinstance(parameters, dict):
                 for k, v in parameters.items():
                     func = self.get(v)
                     if not func:
-                        raise TypeError("{0} is not defined formatter.".format(type(v)))
+                        raise TypeError(f"{type(v)} is not defined formatter.")
                     kwargs.update({k: func(self, escaper, v)})
             else:
                 raise ProgrammingError(
-                    "Unsupported parameter "
-                    + "(Support for dict only): {0}".format(parameters)
+                    f"Unsupported parameter (Support for dict only): {parameters}"
                 )
 
         return (operation % kwargs).strip() if kwargs is not None else operation.strip()
```

### Comparing `PyAthena-2.9.6/pyathena/model.py` & `pyathena-3.0.0/pyathena/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,58 +6,68 @@
 
 from pyathena.error import DataError
 
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
 class AthenaQueryExecution:
-
     STATE_QUEUED: str = "QUEUED"
     STATE_RUNNING: str = "RUNNING"
     STATE_SUCCEEDED: str = "SUCCEEDED"
     STATE_FAILED: str = "FAILED"
     STATE_CANCELLED: str = "CANCELLED"
 
     STATEMENT_TYPE_DDL: str = "DDL"
     STATEMENT_TYPE_DML: str = "DML"
     STATEMENT_TYPE_UTILITY: str = "UTILITY"
 
+    ENCRYPTION_OPTION_SSE_S3: str = "SSE_S3"
+    ENCRYPTION_OPTION_SSE_KMS: str = "SSE_KMS"
+    ENCRYPTION_OPTION_CSE_KMS: str = "CSE_KMS"
+
+    ERROR_CATEGORY_SYSTEM: int = 1
+    ERROR_CATEGORY_USER: int = 2
+    ERROR_CATEGORY_OTHER: int = 3
+
+    S3_ACL_OPTION_BUCKET_OWNER_FULL_CONTROL = "BUCKET_OWNER_FULL_CONTROL"
+
     def __init__(self, response: Dict[str, Any]) -> None:
         query_execution = response.get("QueryExecution", None)
         if not query_execution:
             raise DataError("KeyError `QueryExecution`")
 
         query_execution_context = query_execution.get("QueryExecutionContext", {})
         self._database: Optional[str] = query_execution_context.get("Database", None)
+        self._catalog: Optional[str] = query_execution_context.get("Catalog", None)
 
         self._query_id: Optional[str] = query_execution.get("QueryExecutionId", None)
         if not self._query_id:
             raise DataError("KeyError `QueryExecutionId`")
-
         self._query: Optional[str] = query_execution.get("Query", None)
         if not self._query:
             raise DataError("KeyError `Query`")
         self._statement_type: Optional[str] = query_execution.get("StatementType", None)
+        self._work_group: Optional[str] = query_execution.get("WorkGroup", None)
+        self._execution_parameters: List[str] = query_execution.get("ExecutionParameters", [])
 
         status = query_execution.get("Status", None)
         if not status:
             raise DataError("KeyError `Status`")
         self._state: Optional[str] = status.get("State", None)
         self._state_change_reason: Optional[str] = status.get("StateChangeReason", None)
-        self._completion_date_time: Optional[datetime] = status.get(
-            "CompletionDateTime", None
-        )
-        self._submission_date_time: Optional[datetime] = status.get(
-            "SubmissionDateTime", None
-        )
+        self._submission_date_time: Optional[datetime] = status.get("SubmissionDateTime", None)
+        self._completion_date_time: Optional[datetime] = status.get("CompletionDateTime", None)
+        athena_error = status.get("AthenaError", {})
+        self._error_category: Optional[int] = athena_error.get("ErrorCategory", None)
+        self._error_type: Optional[int] = athena_error.get("ErrorType", None)
+        self._retryable: Optional[bool] = athena_error.get("Retryable", None)
+        self._error_message: Optional[str] = athena_error.get("ErrorMessage", None)
 
         statistics = query_execution.get("Statistics", {})
-        self._data_scanned_in_bytes: Optional[int] = statistics.get(
-            "DataScannedInBytes", None
-        )
+        self._data_scanned_in_bytes: Optional[int] = statistics.get("DataScannedInBytes", None)
         self._engine_execution_time_in_millis: Optional[int] = statistics.get(
             "EngineExecutionTimeInMillis", None
         )
         self._query_queue_time_in_millis: Optional[int] = statistics.get(
             "QueryQueueTimeInMillis", None
         )
         self._total_execution_time_in_millis: Optional[int] = statistics.get(
@@ -65,60 +75,99 @@
         )
         self._query_planning_time_in_millis: Optional[int] = statistics.get(
             "QueryPlanningTimeInMillis", None
         )
         self._service_processing_time_in_millis: Optional[int] = statistics.get(
             "ServiceProcessingTimeInMillis", None
         )
-        self._data_manifest_location: Optional[str] = statistics.get(
-            "DataManifestLocation", None
-        )
+        self._data_manifest_location: Optional[str] = statistics.get("DataManifestLocation", None)
+        reuse_info = statistics.get("ResultReuseInformation", {})
+        self._reused_previous_result: Optional[bool] = reuse_info.get("ReusedPreviousResult", None)
 
         result_conf = query_execution.get("ResultConfiguration", {})
         self._output_location: Optional[str] = result_conf.get("OutputLocation", None)
-
         encryption_conf = result_conf.get("EncryptionConfiguration", {})
-        self._encryption_option: Optional[str] = encryption_conf.get(
-            "EncryptionOption", None
-        )
+        self._encryption_option: Optional[str] = encryption_conf.get("EncryptionOption", None)
         self._kms_key: Optional[str] = encryption_conf.get("KmsKey", None)
-
-        self._work_group: Optional[str] = query_execution.get("WorkGroup", None)
+        self._expected_bucket_owner: Optional[str] = result_conf.get("ExpectedBucketOwner", None)
+        acl_conf = result_conf.get("AclConfiguration", {})
+        self._s3_acl_option: Optional[str] = acl_conf.get("S3AclOption", None)
+
+        engine_version = query_execution.get("EngineVersion", {})
+        self._selected_engine_version: Optional[str] = engine_version.get(
+            "SelectedEngineVersion", None
+        )
+        self._effective_engine_version: Optional[str] = engine_version.get(
+            "EffectiveEngineVersion", None
+        )
+
+        reuse_conf = query_execution.get("ResultReuseConfiguration", {})
+        reuse_age_conf = reuse_conf.get("ResultReuseByAgeConfiguration", {})
+        self._result_reuse_enabled: Optional[bool] = reuse_age_conf.get("Enabled", None)
+        self._result_reuse_minutes: Optional[int] = reuse_age_conf.get("MaxAgeInMinutes", None)
 
     @property
     def database(self) -> Optional[str]:
         return self._database
 
     @property
+    def catalog(self) -> Optional[str]:
+        return self._catalog
+
+    @property
     def query_id(self) -> Optional[str]:
         return self._query_id
 
     @property
     def query(self) -> Optional[str]:
         return self._query
 
     @property
     def statement_type(self) -> Optional[str]:
         return self._statement_type
 
     @property
+    def work_group(self) -> Optional[str]:
+        return self._work_group
+
+    @property
+    def execution_parameters(self) -> List[str]:
+        return self._execution_parameters
+
+    @property
     def state(self) -> Optional[str]:
         return self._state
 
     @property
     def state_change_reason(self) -> Optional[str]:
         return self._state_change_reason
 
     @property
+    def submission_date_time(self) -> Optional[datetime]:
+        return self._submission_date_time
+
+    @property
     def completion_date_time(self) -> Optional[datetime]:
         return self._completion_date_time
 
     @property
-    def submission_date_time(self) -> Optional[datetime]:
-        return self._submission_date_time
+    def error_category(self) -> Optional[int]:
+        return self._error_category
+
+    @property
+    def error_type(self) -> Optional[int]:
+        return self._error_type
+
+    @property
+    def retryable(self) -> Optional[bool]:
+        return self._retryable
+
+    @property
+    def error_message(self) -> Optional[str]:
+        return self._error_message
 
     @property
     def data_scanned_in_bytes(self) -> Optional[int]:
         return self._data_scanned_in_bytes
 
     @property
     def engine_execution_time_in_millis(self) -> Optional[int]:
@@ -145,24 +194,71 @@
         return self._output_location
 
     @property
     def data_manifest_location(self) -> Optional[str]:
         return self._data_manifest_location
 
     @property
+    def reused_previous_result(self) -> Optional[bool]:
+        return self._reused_previous_result
+
+    @property
     def encryption_option(self) -> Optional[str]:
         return self._encryption_option
 
     @property
     def kms_key(self) -> Optional[str]:
         return self._kms_key
 
     @property
-    def work_group(self) -> Optional[str]:
-        return self._work_group
+    def expected_bucket_owner(self) -> Optional[str]:
+        return self._expected_bucket_owner
+
+    @property
+    def s3_acl_option(self) -> Optional[str]:
+        return self._s3_acl_option
+
+    @property
+    def selected_engine_version(self) -> Optional[str]:
+        return self._selected_engine_version
+
+    @property
+    def effective_engine_version(self) -> Optional[str]:
+        return self._effective_engine_version
+
+    @property
+    def result_reuse_enabled(self) -> Optional[bool]:
+        return self._result_reuse_enabled
+
+    @property
+    def result_reuse_minutes(self) -> Optional[int]:
+        return self._result_reuse_minutes
+
+
+class AthenaDatabase:
+    def __init__(self, response):
+        database = response.get("Database", None)
+        if not database:
+            raise DataError("KeyError `Database`")
+
+        self._name: Optional[str] = database.get("Name", None)
+        self._description: Optional[str] = database.get("Description", None)
+        self._parameters: Dict[str, str] = database.get("Parameters", {})
+
+    @property
+    def name(self) -> Optional[str]:
+        return self._name
+
+    @property
+    def description(self) -> Optional[str]:
+        return self._description
+
+    @property
+    def parameters(self) -> Dict[str, str]:
+        return self._parameters
 
 
 class AthenaTableMetadataColumn:
     def __init__(self, response):
         self._name: Optional[str] = response.get("Name", None)
         self._type: Optional[str] = response.get("Type", None)
         self._comment: Optional[str] = response.get("Comment", None)
@@ -203,17 +299,15 @@
     def __init__(self, response):
         table_metadata = response.get("TableMetadata", None)
         if not table_metadata:
             raise DataError("KeyError `TableMetadata`")
 
         self._name: Optional[str] = table_metadata.get("Name", None)
         self._create_time: Optional[datetime] = table_metadata.get("CreateTime", None)
-        self._last_access_time: Optional[datetime] = table_metadata.get(
-            "LastAccessTime", None
-        )
+        self._last_access_time: Optional[datetime] = table_metadata.get("LastAccessTime", None)
         self._table_type: Optional[str] = table_metadata.get("TableType", None)
 
         columns = table_metadata.get("Columns", [])
         self._columns: List[AthenaTableMetadataColumn] = []
         for column in columns:
             self._columns.append(AthenaTableMetadataColumn(column))
 
@@ -306,23 +400,18 @@
             k.replace("serde.param.", ""): v
             for k, v in self._parameters.items()
             if k.startswith("serde.param.")
         }
 
     @property
     def table_properties(self) -> Dict[str, str]:
-        return {
-            k: v
-            for k, v in self._parameters.items()
-            if not k.startswith("serde.param.")
-        }
+        return {k: v for k, v in self._parameters.items() if not k.startswith("serde.param.")}
 
 
 class AthenaFileFormat:
-
     FILE_FORMAT_SEQUENCEFILE: str = "SEQUENCEFILE"
     FILE_FORMAT_TEXTFILE: str = "TEXTFILE"
     FILE_FORMAT_RCFILE: str = "RCFILE"
     FILE_FORMAT_ORC: str = "ORC"
     FILE_FORMAT_PARQUET: str = "PARQUET"
     FILE_FORMAT_AVRO: str = "AVRO"
     FILE_FORMAT_ION: str = "ION"
@@ -333,29 +422,24 @@
 
     @staticmethod
     def is_orc(value: str) -> bool:
         return value.upper() == AthenaFileFormat.FILE_FORMAT_ORC
 
 
 class AthenaRowFormatSerde:
-
     PATTERN_ROW_FORMAT_SERDE: Pattern[str] = re.compile(r"^(?i:serde) '(?P<serde>.+)'$")
 
     ROW_FORMAT_SERDE_CSV: str = "org.apache.hadoop.hive.serde2.OpenCSVSerde"
     ROW_FORMAT_SERDE_REGEX: str = "org.apache.hadoop.hive.serde2.RegexSerDe"
-    ROW_FORMAT_SERDE_LAZY_SIMPLE: str = (
-        "org.apache.hadoop.hive.serde2.lazy.LazySimpleSerDe"
-    )
+    ROW_FORMAT_SERDE_LAZY_SIMPLE: str = "org.apache.hadoop.hive.serde2.lazy.LazySimpleSerDe"
     ROW_FORMAT_SERDE_CLOUD_TRAIL: str = "com.amazon.emr.hive.serde.CloudTrailSerde"
     ROW_FORMAT_SERDE_GROK: str = "com.amazonaws.glue.serde.GrokSerDe"
     ROW_FORMAT_SERDE_JSON: str = "org.openx.data.jsonserde.JsonSerDe"
     ROW_FORMAT_SERDE_JSON_HCATALOG: str = "org.apache.hive.hcatalog.data.JsonSerDe"
-    ROW_FORMAT_SERDE_PARQUET: str = (
-        "org.apache.hadoop.hive.ql.io.parquet.serde.ParquetHiveSerDe"
-    )
+    ROW_FORMAT_SERDE_PARQUET: str = "org.apache.hadoop.hive.ql.io.parquet.serde.ParquetHiveSerDe"
     ROW_FORMAT_SERDE_ORC: str = "org.apache.hadoop.hive.ql.io.orc.OrcSerde"
     ROW_FORMAT_SERDE_AVRO: str = "org.apache.hadoop.hive.serde2.avro.AvroSerDe"
 
     @staticmethod
     def is_parquet(value: str) -> bool:
         match = AthenaRowFormatSerde.PATTERN_ROW_FORMAT_SERDE.search(value)
         if match:
@@ -371,15 +455,14 @@
             serde = match.group("serde")
             if serde == AthenaRowFormatSerde.ROW_FORMAT_SERDE_ORC:
                 return True
         return False
 
 
 class AthenaCompression:
-
     COMPRESSION_BZIP2: str = "BZIP2"
     COMPRESSION_DEFLATE: str = "DEFLATE"
     COMPRESSION_GZIP: str = "GZIP"
     COMPRESSION_LZ4: str = "LZ4"
     COMPRESSION_LZO: str = "LZO"
     COMPRESSION_SNAPPY: str = "SNAPPY"
     COMPRESSION_ZLIB: str = "ZLIB"
```

### Comparing `PyAthena-2.9.6/pyathena/pandas/async_cursor.py` & `pyathena-3.0.0/pyathena/pandas/async_cursor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import logging
 from concurrent.futures import Future
 from multiprocessing import cpu_count
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Tuple, Union
 
 from pyathena import ProgrammingError
 from pyathena.async_cursor import AsyncCursor
 from pyathena.common import CursorIterator
 from pyathena.converter import Converter
 from pyathena.formatter import Formatter
 from pyathena.model import AthenaCompression, AthenaFileFormat
@@ -37,14 +37,18 @@
         poll_interval: float = 1,
         encryption_option: Optional[str] = None,
         kms_key: Optional[str] = None,
         kill_on_interrupt: bool = True,
         max_workers: int = (cpu_count() or 1) * 5,
         arraysize: int = CursorIterator.DEFAULT_FETCH_SIZE,
         unload: bool = False,
+        engine: str = "auto",
+        chunksize: Optional[int] = None,
+        result_reuse_enable: bool = False,
+        result_reuse_minutes: int = CursorIterator.DEFAULT_RESULT_REUSE_MINUTES,
     ) -> None:
         super(AsyncPandasCursor, self).__init__(
             connection=connection,
             converter=converter,
             formatter=formatter,
             retry_config=retry_config,
             s3_staging_dir=s3_staging_dir,
@@ -53,16 +57,20 @@
             work_group=work_group,
             poll_interval=poll_interval,
             encryption_option=encryption_option,
             kms_key=kms_key,
             kill_on_interrupt=kill_on_interrupt,
             max_workers=max_workers,
             arraysize=arraysize,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         self._unload = unload
+        self._engine = engine
+        self._chunksize = chunksize
 
     @staticmethod
     def get_default_converter(
         unload: bool = False,
     ) -> Union[DefaultPandasTypeConverter, Any]:
         if unload:
             return DefaultPandasUnloadTypeConverter()
@@ -79,18 +87,18 @@
             raise ProgrammingError("arraysize must be a positive integer value.")
         self._arraysize = value
 
     def _collect_result_set(
         self,
         query_id: str,
         keep_default_na: bool = False,
-        na_values: List[str] = None,
+        na_values: Optional[Iterable[str]] = ("",),
         quoting: int = 1,
         unload_location: Optional[str] = None,
-        kwargs: Dict[str, Any] = None,
+        kwargs: Optional[Dict[str, Any]] = None,
     ) -> AthenaPandasResultSet:
         if kwargs is None:
             kwargs = dict()
         query_execution = self._poll(query_id)
         return AthenaPandasResultSet(
             connection=self._connection,
             converter=self._converter,
@@ -98,35 +106,37 @@
             arraysize=self._arraysize,
             retry_config=self._retry_config,
             keep_default_na=keep_default_na,
             na_values=na_values,
             quoting=quoting,
             unload=self._unload,
             unload_location=unload_location,
+            engine=kwargs.pop("engine", self._engine),
+            chunksize=kwargs.pop("chunksize", self._chunksize),
             **kwargs,
         )
 
     def execute(
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
+        result_reuse_enable: Optional[bool] = None,
+        result_reuse_minutes: Optional[int] = None,
         keep_default_na: bool = False,
-        na_values: List[str] = None,
+        na_values: Optional[Iterable[str]] = ("",),
         quoting: int = 1,
         **kwargs,
     ) -> Tuple[str, "Future[Union[AthenaPandasResultSet, Any]]"]:
         if self._unload:
             s3_staging_dir = s3_staging_dir if s3_staging_dir else self._s3_staging_dir
-            assert (
-                s3_staging_dir
-            ), "If the unload option is used, s3_staging_dir is required."
+            assert s3_staging_dir, "If the unload option is used, s3_staging_dir is required."
             operation, unload_location = self._formatter.wrap_unload(
                 operation,
                 s3_staging_dir=s3_staging_dir,
                 format_=AthenaFileFormat.FILE_FORMAT_PARQUET,
                 compression=AthenaCompression.COMPRESSION_SNAPPY,
             )
         else:
@@ -134,14 +144,16 @@
         query_id = self._execute(
             operation,
             parameters=parameters,
             work_group=work_group,
             s3_staging_dir=s3_staging_dir,
             cache_size=cache_size,
             cache_expiration_time=cache_expiration_time,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         return (
             query_id,
             self._executor.submit(
                 self._collect_result_set,
                 query_id,
                 keep_default_na,
```

### Comparing `PyAthena-2.9.6/pyathena/pandas/converter.py` & `pyathena-3.0.0/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `PyAthena-2.9.6/pyathena/pandas/cursor.py` & `pyathena-3.0.0/pyathena/pandas/cursor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import logging
+from multiprocessing import cpu_count
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Optional,
     Tuple,
-    TypeVar,
     Union,
     cast,
 )
 
 from pyathena.common import CursorIterator
 from pyathena.converter import Converter
 from pyathena.cursor import BaseCursor
@@ -21,23 +23,22 @@
 from pyathena.model import AthenaCompression, AthenaFileFormat, AthenaQueryExecution
 from pyathena.pandas.converter import (
     DefaultPandasTypeConverter,
     DefaultPandasUnloadTypeConverter,
 )
 from pyathena.pandas.result_set import AthenaPandasResultSet
 from pyathena.result_set import WithResultSet
-from pyathena.util import RetryConfig, synchronized
+from pyathena.util import RetryConfig
 
 if TYPE_CHECKING:
     from pandas import DataFrame
 
     from pyathena.connection import Connection
 
 _logger = logging.getLogger(__name__)  # type: ignore
-_T = TypeVar("_T", bound="PandasCursor")
 
 
 class PandasCursor(BaseCursor, CursorIterator, WithResultSet):
     def __init__(
         self,
         connection: "Connection",
         converter: Converter,
@@ -48,14 +49,21 @@
         catalog_name: Optional[str] = None,
         work_group: Optional[str] = None,
         poll_interval: float = 1,
         encryption_option: Optional[str] = None,
         kms_key: Optional[str] = None,
         kill_on_interrupt: bool = True,
         unload: bool = False,
+        engine: str = "auto",
+        chunksize: Optional[int] = None,
+        block_size: Optional[int] = None,
+        cache_type: Optional[str] = None,
+        max_workers: int = (cpu_count() or 1) * 5,
+        result_reuse_enable: bool = False,
+        result_reuse_minutes: int = CursorIterator.DEFAULT_RESULT_REUSE_MINUTES,
         **kwargs,
     ) -> None:
         super(PandasCursor, self).__init__(
             connection=connection,
             converter=converter,
             formatter=formatter,
             retry_config=retry_config,
@@ -63,17 +71,24 @@
             schema_name=schema_name,
             catalog_name=catalog_name,
             work_group=work_group,
             poll_interval=poll_interval,
             encryption_option=encryption_option,
             kms_key=kms_key,
             kill_on_interrupt=kill_on_interrupt,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
             **kwargs,
         )
         self._unload = unload
+        self._engine = engine
+        self._chunksize = chunksize
+        self._block_size = block_size
+        self._cache_type = cache_type
+        self._max_workers = max_workers
         self._query_id: Optional[str] = None
         self._result_set: Optional[AthenaPandasResultSet] = None
 
     @staticmethod
     def get_default_converter(
         unload: bool = False,
     ) -> Union[DefaultPandasTypeConverter, Any]:
@@ -88,15 +103,15 @@
 
     @arraysize.setter
     def arraysize(self, value: int) -> None:
         if value <= 0:
             raise ProgrammingError("arraysize must be a positive integer value.")
         self._arraysize = value
 
-    @property
+    @property  # type: ignore
     def result_set(self) -> Optional[AthenaPandasResultSet]:
         return self._result_set
 
     @result_set.setter
     def result_set(self, val) -> None:
         self._result_set = val
 
@@ -112,34 +127,33 @@
     def rownumber(self) -> Optional[int]:
         return self.result_set.rownumber if self.result_set else None
 
     def close(self) -> None:
         if self.result_set and not self.result_set.is_closed:
             self.result_set.close()
 
-    @synchronized
     def execute(
-        self: _T,
+        self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         work_group: Optional[str] = None,
         s3_staging_dir: Optional[str] = None,
         cache_size: int = 0,
         cache_expiration_time: int = 0,
+        result_reuse_enable: Optional[bool] = None,
+        result_reuse_minutes: Optional[int] = None,
         keep_default_na: bool = False,
         na_values: Optional[Iterable[str]] = ("",),
         quoting: int = 1,
         **kwargs,
-    ) -> _T:
+    ) -> PandasCursor:
         self._reset_state()
         if self._unload:
             s3_staging_dir = s3_staging_dir if s3_staging_dir else self._s3_staging_dir
-            assert (
-                s3_staging_dir
-            ), "If the unload option is used, s3_staging_dir is required."
+            assert s3_staging_dir, "If the unload option is used, s3_staging_dir is required."
             operation, unload_location = self._formatter.wrap_unload(
                 operation,
                 s3_staging_dir=s3_staging_dir,
                 format_=AthenaFileFormat.FILE_FORMAT_PARQUET,
                 compression=AthenaCompression.COMPRESSION_SNAPPY,
             )
         else:
@@ -147,74 +161,76 @@
         self.query_id = self._execute(
             operation,
             parameters=parameters,
             work_group=work_group,
             s3_staging_dir=s3_staging_dir,
             cache_size=cache_size,
             cache_expiration_time=cache_expiration_time,
+            result_reuse_enable=result_reuse_enable,
+            result_reuse_minutes=result_reuse_minutes,
         )
         query_execution = self._poll(self.query_id)
         if query_execution.state == AthenaQueryExecution.STATE_SUCCEEDED:
             self.result_set = AthenaPandasResultSet(
                 connection=self._connection,
                 converter=self._converter,
                 query_execution=query_execution,
                 arraysize=self.arraysize,
                 retry_config=self._retry_config,
                 keep_default_na=keep_default_na,
                 na_values=na_values,
                 quoting=quoting,
                 unload=self._unload,
                 unload_location=unload_location,
+                engine=kwargs.pop("engine", self._engine),
+                chunksize=kwargs.pop("chunksize", self._chunksize),
+                block_size=kwargs.pop("block_size", self._block_size),
+                cache_type=kwargs.pop("cache_type", self._cache_type),
+                max_workers=kwargs.pop("max_workers", self._max_workers),
                 **kwargs,
             )
         else:
             raise OperationalError(query_execution.state_change_reason)
         return self
 
     def executemany(
         self, operation: str, seq_of_parameters: List[Optional[Dict[str, Any]]]
     ) -> None:
         for parameters in seq_of_parameters:
             self.execute(operation, parameters)
         # Operations that have result sets are not allowed with executemany.
         self._reset_state()
 
-    @synchronized
     def cancel(self) -> None:
         if not self.query_id:
             raise ProgrammingError("QueryExecutionId is none or empty.")
         self._cancel(self.query_id)
 
-    @synchronized
     def fetchone(
         self,
     ) -> Optional[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaPandasResultSet, self.result_set)
         return result_set.fetchone()
 
-    @synchronized
     def fetchmany(
         self, size: Optional[int] = None
     ) -> List[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaPandasResultSet, self.result_set)
         return result_set.fetchmany(size)
 
-    @synchronized
     def fetchall(
         self,
     ) -> List[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaPandasResultSet, self.result_set)
         return result_set.fetchall()
 
-    @synchronized
     def as_pandas(self) -> "DataFrame":
         if not self.has_result_set:
             raise ProgrammingError("No result set.")
         result_set = cast(AthenaPandasResultSet, self.result_set)
         return result_set.as_pandas()
```

### Comparing `PyAthena-2.9.6/pyathena/pandas/util.py` & `pyathena-3.0.0/pyathena/pandas/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     from pyathena.connection import Connection
     from pyathena.cursor import Cursor
 
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
-def get_chunks(df: "DataFrame", chunksize: int = None) -> Iterator["DataFrame"]:
+def get_chunks(df: "DataFrame", chunksize: Optional[int] = None) -> Iterator["DataFrame"]:
     rows = len(df)
     if rows == 0:
         return
     if chunksize is None:
         chunksize = rows
     elif chunksize <= 0:
         raise ValueError("Chunk size argument must be greater than zero")
@@ -64,17 +64,15 @@
 def as_pandas(cursor: "Cursor", coerce_float: bool = False) -> "DataFrame":
     from pandas import DataFrame
 
     description = cursor.description
     if not description:
         return DataFrame()
     names = [metadata[0] for metadata in description]
-    return DataFrame.from_records(
-        cursor.fetchall(), columns=names, coerce_float=coerce_float
-    )
+    return DataFrame.from_records(cursor.fetchall(), columns=names, coerce_float=coerce_float)
 
 
 def to_sql_type_mappings(col: "Series") -> str:
     import pandas as pd
 
     col_type = pd.api.types.infer_dtype(col, skipna=True)
     if col_type == "datetime64" or col_type == "datetime":
@@ -107,15 +105,15 @@
 def to_parquet(
     df: "DataFrame",
     bucket_name: str,
     prefix: str,
     retry_config: RetryConfig,
     session_kwargs: Dict[str, Any],
     client_kwargs: Dict[str, Any],
-    compression: str = None,
+    compression: Optional[str] = None,
     flavor: str = "spark",
 ) -> str:
     import pyarrow as pa
     from pyarrow import parquet as pq
 
     session = Session(**session_kwargs)
     client = session.resource("s3", **client_kwargs)
@@ -136,23 +134,21 @@
     df: "DataFrame",
     name: str,
     conn: "Connection",
     location: str,
     schema: str = "default",
     index: bool = False,
     index_label: Optional[str] = None,
-    partitions: List[str] = None,
+    partitions: Optional[List[str]] = None,
     chunksize: Optional[int] = None,
     if_exists: str = "fail",
-    compression: str = None,
+    compression: Optional[str] = None,
     flavor: str = "spark",
     type_mappings: Callable[["Series"], str] = to_sql_type_mappings,
-    executor_class: Type[
-        Union[ThreadPoolExecutor, ProcessPoolExecutor]
-    ] = ThreadPoolExecutor,
+    executor_class: Type[Union[ThreadPoolExecutor, ProcessPoolExecutor]] = ThreadPoolExecutor,
     max_workers: int = (cpu_count() or 1) * 5,
     repair_table=True,
 ) -> None:
     # TODO Supports orc, avro, json, csv or tsv format
     if if_exists not in ("fail", "replace", "append"):
         raise ValueError(f"`{if_exists}` is not valid for if_exists")
     if compression is not None and not AthenaCompression.is_valid(compression):
@@ -203,22 +199,18 @@
         client_kwargs = deepcopy(conn._client_kwargs)
         client_kwargs.update({"region_name": conn.region_name})
         partition_prefixes = []
         if partitions:
             for keys, group in df.groupby(by=partitions, observed=True):
                 keys = keys if isinstance(keys, tuple) else (keys,)
                 group = group.drop(partitions, axis=1)
-                partition_prefix = "/".join(
-                    [f"{key}={val}" for key, val in zip(partitions, keys)]
-                )
+                partition_prefix = "/".join([f"{key}={val}" for key, val in zip(partitions, keys)])
                 partition_prefixes.append(
                     (
-                        ", ".join(
-                            [f"`{key}` = '{val}'" for key, val in zip(partitions, keys)]
-                        ),
+                        ", ".join([f"`{key}` = '{val}'" for key, val in zip(partitions, keys)]),
                         f"{location}{partition_prefix}/",
                     )
                 )
                 for chunk in get_chunks(group, chunksize):
                     futures.append(
                         e.submit(
                             to_parquet,
@@ -270,22 +262,17 @@
                 ADD IF NOT EXISTS PARTITION ({partition[0]}) LOCATION '{partition[1]}'
                 """
             )
             _logger.info(add_partition)
             cursor.execute(add_partition)
 
 
-def get_column_names_and_types(
-    df: "DataFrame", type_mappings
-) -> "OrderedDict[str, str]":
+def get_column_names_and_types(df: "DataFrame", type_mappings) -> "OrderedDict[str, str]":
     return OrderedDict(
-        (
-            (str(df.columns[i]), type_mappings(df.iloc[:, i]))
-            for i in range(len(df.columns))
-        )
+        ((str(df.columns[i]), type_mappings(df.iloc[:, i])) for i in range(len(df.columns)))
     )
 
 
 def generate_ddl(
     df: "DataFrame",
     name: str,
     location: str,
```

### Comparing `PyAthena-2.9.6/pyathena/result_set.py` & `pyathena-3.0.0/pyathena/result_set.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,15 +40,18 @@
         super(AthenaResultSet, self).__init__(arraysize=arraysize)
         self._connection: Optional["Connection"] = connection
         self._converter = converter
         self._query_execution: Optional[AthenaQueryExecution] = query_execution
         assert self._query_execution, "Required argument `query_execution` not found."
         self._retry_config = retry_config
         self._client = connection.session.client(
-            "s3", region_name=connection.region_name, **connection._client_kwargs
+            "s3",
+            region_name=connection.region_name,
+            config=connection.config,
+            **connection._client_kwargs,
         )
 
         self._metadata: Optional[Tuple[Dict[str, Any], ...]] = None
         self._rows: Deque[
             Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]
         ] = collections.deque()
         self._next_token: Optional[str] = None
@@ -60,14 +63,20 @@
     @property
     def database(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.database
 
     @property
+    def catalog(self) -> Optional[str]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.catalog
+
+    @property
     def query_id(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.query_id
 
     @property
     def query(self) -> Optional[str]:
@@ -78,36 +87,72 @@
     @property
     def statement_type(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.statement_type
 
     @property
+    def work_group(self) -> Optional[str]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.work_group
+
+    @property
+    def execution_parameters(self) -> List[str]:
+        if not self._query_execution:
+            return []
+        return self._query_execution.execution_parameters
+
+    @property
     def state(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.state
 
     @property
     def state_change_reason(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.state_change_reason
 
     @property
+    def submission_date_time(self) -> Optional[datetime]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.submission_date_time
+
+    @property
     def completion_date_time(self) -> Optional[datetime]:
         if not self._query_execution:
             return None
         return self._query_execution.completion_date_time
 
     @property
-    def submission_date_time(self) -> Optional[datetime]:
+    def error_category(self) -> Optional[int]:
         if not self._query_execution:
             return None
-        return self._query_execution.submission_date_time
+        return self._query_execution.error_category
+
+    @property
+    def error_type(self) -> Optional[int]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.error_type
+
+    @property
+    def retryable(self) -> Optional[bool]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.retryable
+
+    @property
+    def error_message(self) -> Optional[str]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.error_message
 
     @property
     def data_scanned_in_bytes(self) -> Optional[int]:
         if not self._query_execution:
             return None
         return self._query_execution.data_scanned_in_bytes
 
@@ -150,30 +195,66 @@
     @property
     def data_manifest_location(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.data_manifest_location
 
     @property
+    def reused_previous_result(self) -> Optional[bool]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.reused_previous_result
+
+    @property
     def encryption_option(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.encryption_option
 
     @property
     def kms_key(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.kms_key
 
     @property
-    def work_group(self) -> Optional[str]:
+    def expected_bucket_owner(self) -> Optional[str]:
         if not self._query_execution:
             return None
-        return self._query_execution.work_group
+        return self._query_execution.expected_bucket_owner
+
+    @property
+    def s3_acl_option(self) -> Optional[str]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.s3_acl_option
+
+    @property
+    def selected_engine_version(self) -> Optional[str]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.selected_engine_version
+
+    @property
+    def effective_engine_version(self) -> Optional[str]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.effective_engine_version
+
+    @property
+    def result_reuse_enabled(self) -> Optional[bool]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.result_reuse_enabled
+
+    @property
+    def result_reuse_minutes(self) -> Optional[int]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.result_reuse_minutes
 
     @property
     def description(
         self,
     ) -> Optional[List[Tuple[str, str, None, None, int, int, str]]]:
         if self._metadata is None:
             return None
@@ -286,17 +367,15 @@
 
     def _get_rows(
         self, offset: int, metadata: Tuple[Any, ...], rows: List[Dict[str, Any]]
     ) -> List[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         return [
             tuple(
                 [
-                    self._converter.convert(
-                        meta.get("Type", None), row.get("VarCharValue", None)
-                    )
+                    self._converter.convert(meta.get("Type", None), row.get("VarCharValue", None))
                     for meta, row in zip(metadata, rows[i].get("Data", []))
                 ]
             )
             for i in range(offset, len(rows))
         ]
 
     def _process_rows(self, response: Dict[str, Any]) -> None:
@@ -304,19 +383,15 @@
         if not result_set:
             raise DataError("KeyError `ResultSet`")
         rows = result_set.get("Rows", None)
         if rows is None:
             raise DataError("KeyError `Rows`")
         processed_rows = []
         if len(rows) > 0:
-            offset = (
-                1
-                if not self._next_token and self._is_first_row_column_labels(rows)
-                else 0
-            )
+            offset = 1 if not self._next_token and self._is_first_row_column_labels(rows) else 0
             metadata = cast(Tuple[Any, ...], self._metadata)
             processed_rows = self._get_rows(offset, metadata, rows)
         self._rows.extend(processed_rows)
         self._next_token = response.get("NextToken", None)
 
     def _is_first_row_column_labels(self, rows: List[Dict[str, Any]]) -> bool:
         first_row_data = rows[0].get("Data", [])
@@ -379,15 +454,14 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
 
 class AthenaDictResultSet(AthenaResultSet):
-
     # You can override this to use OrderedDict or other dict-like types.
     dict_type: Type[Any] = dict
 
     def _get_rows(
         self, offset: int, metadata: Tuple[Any, ...], rows: List[Dict[str, Any]]
     ) -> List[Union[Tuple[Optional[Any], ...], Dict[Any, Optional[Any]]]]:
         return [
@@ -442,14 +516,21 @@
     @property
     def database(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.database
 
+    @property
+    def catalog(self) -> Optional[str]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.catalog
+
     @property  # type: ignore
     @abstractmethod
     def query_id(self) -> Optional[str]:
         raise NotImplementedError  # pragma: no cover
 
     @query_id.setter  # type: ignore
     @abstractmethod
@@ -467,40 +548,82 @@
     def statement_type(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.statement_type
 
     @property
+    def work_group(self) -> Optional[str]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.work_group
+
+    @property
+    def execution_parameters(self) -> List[str]:
+        if not self.has_result_set:
+            return []
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.execution_parameters
+
+    @property
     def state(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.state
 
     @property
     def state_change_reason(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.state_change_reason
 
     @property
+    def submission_date_time(self) -> Optional[datetime]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.submission_date_time
+
+    @property
     def completion_date_time(self) -> Optional[datetime]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.completion_date_time
 
     @property
-    def submission_date_time(self) -> Optional[datetime]:
+    def error_category(self) -> Optional[int]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
-        return result_set.submission_date_time
+        return result_set.error_category
+
+    @property
+    def error_type(self) -> Optional[int]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.error_type
+
+    @property
+    def retryable(self) -> Optional[bool]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.retryable
+
+    @property
+    def error_message(self) -> Optional[str]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.error_message
 
     @property
     def data_scanned_in_bytes(self) -> Optional[int]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.data_scanned_in_bytes
@@ -551,26 +674,68 @@
     def data_manifest_location(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.data_manifest_location
 
     @property
+    def reused_previous_result(self) -> Optional[bool]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.reused_previous_result
+
+    @property
     def encryption_option(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.encryption_option
 
     @property
     def kms_key(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.kms_key
 
     @property
-    def work_group(self) -> Optional[str]:
+    def expected_bucket_owner(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
-        return result_set.work_group
+        return result_set.expected_bucket_owner
+
+    @property
+    def s3_acl_option(self) -> Optional[str]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.s3_acl_option
+
+    @property
+    def selected_engine_version(self) -> Optional[str]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.selected_engine_version
+
+    @property
+    def effective_engine_version(self) -> Optional[str]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.effective_engine_version
+
+    @property
+    def result_reuse_enabled(self) -> Optional[bool]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.result_reuse_enabled
+
+    @property
+    def result_reuse_minutes(self) -> Optional[int]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.result_reuse_minutes
```

### Comparing `PyAthena-2.9.6/pyathena/sqlalchemy_athena.py` & `pyathena-3.0.0/pyathena/sqlalchemy/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,369 +1,709 @@
 # -*- coding: utf-8 -*-
 import re
 from distutils.util import strtobool
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    List,
+    Mapping,
+    MutableMapping,
+    Optional,
+    Pattern,
+    Set,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 import botocore
 from sqlalchemy import exc, schema, types, util
 from sqlalchemy.engine import Engine, reflection
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.exc import NoSuchTableError
 from sqlalchemy.sql.compiler import (
+    ILLEGAL_INITIAL_CHARACTERS,
     DDLCompiler,
     GenericTypeCompiler,
     IdentifierPreparer,
     SQLCompiler,
 )
 
 import pyathena
 from pyathena.model import AthenaFileFormat, AthenaRowFormatSerde
+from pyathena.sqlalchemy.types import AthenaDate, AthenaTimestamp
+from pyathena.sqlalchemy.util import _HashableDict
 
+if TYPE_CHECKING:
+    from types import ModuleType
 
-class UniversalSet:
-    """UniversalSet
-
-    https://github.com/dropbox/PyHive/blob/master/pyhive/common.py"""
-
-    def __contains__(self, item):
-        return True
+    from sqlalchemy import (
+        URL,
+        Cast,
+        CheckConstraint,
+        ClauseElement,
+        Column,
+        Connection,
+        Dialect,
+        ExecutableDDLElement,
+        ForeignKeyConstraint,
+        FunctionElement,
+        GenerativeSelect,
+        PoolProxiedConnection,
+        PrimaryKeyConstraint,
+        Table,
+        UniqueConstraint,
+    )
+    from sqlalchemy.engine.interfaces import (
+        ReflectedForeignKeyConstraint,
+        ReflectedIndex,
+        ReflectedPrimaryKeyConstraint,
+        SchemaTranslateMapType,
+    )
+    from sqlalchemy.sql.base import _DialectArgDict
+    from sqlalchemy.sql.ddl import CreateColumn, CreateTable
+    from sqlalchemy.sql.schema import SchemaItem
+
+# https://docs.aws.amazon.com/athena/latest/ug/reserved-words.html#list-of-ddl-reserved-words
+DDL_RESERVED_WORDS: Set[str] = {
+    "ALL",
+    "ALTER",
+    "AND",
+    "ARRAY",
+    "AS",
+    "AUTHORIZATION",
+    "BETWEEN",
+    "BIGINT",
+    "BINARY",
+    "BOOLEAN",
+    "BOTH",
+    "BY",
+    "CASE",
+    "CASHE",
+    "CAST",
+    "CHAR",
+    "COLUMN",
+    "COMMIT",
+    "CONF",
+    "CONSTRAINT",
+    "CREATE",
+    "CROSS",
+    "CUBE",
+    "CURRENT",
+    "CURRENT_DATE",
+    "CURRENT_TIMESTAMP",
+    "CURSOR",
+    "DATABASE",
+    "DATE",
+    "DAYOFWEEK",
+    "DECIMAL",
+    "DELETE",
+    "DESCRIBE",
+    "DISTINCT",
+    "DOUBLE",
+    "DROP",
+    "ELSE",
+    "END",
+    "EXCHANGE",
+    "EXISTS",
+    "EXTENDED",
+    "EXTERNAL",
+    "EXTRACT",
+    "FALSE",
+    "FETCH",
+    "FLOAT",
+    "FLOOR",
+    "FOLLOWING",
+    "FOR",
+    "FOREIGN",
+    "FROM",
+    "FULL",
+    "FUNCTION",
+    "GRANT",
+    "GROUP",
+    "GROUPING",
+    "HAVING",
+    "IF",
+    "IMPORT",
+    "IN",
+    "INNER",
+    "INSERT",
+    "INT",
+    "INTEGER",
+    "INTERSECT",
+    "INTERVAL",
+    "INTO",
+    "IS",
+    "JOIN",
+    "LATERAL",
+    "LEFT",
+    "LESS",
+    "LIKE",
+    "LOCAL",
+    "MACRO",
+    "MAP",
+    "MORE",
+    "NONE",
+    "NOT",
+    "NULL",
+    "NUMERIC",
+    "OF",
+    "ON",
+    "ONLY",
+    "OR",
+    "ORDER",
+    "OUT",
+    "OUTER",
+    "OVER",
+    "PARTIALSCAN",
+    "PARTITION",
+    "PERCENT",
+    "PRECEDING",
+    "PRECISION",
+    "PRESERVE",
+    "PRIMARY",
+    "PROCEDURE",
+    "RANGE",
+    "READS",
+    "REDUCE",
+    "REFERENCES",
+    "REGEXP",
+    "REVOKE",
+    "RIGHT",
+    "RLIKE",
+    "ROLLBACK",
+    "ROLLUP",
+    "ROW",
+    "ROWS",
+    "SELECT",
+    "SET",
+    "SMALLINT",
+    "START",
+    "TABLE",
+    "TABLESAMPLE",
+    "THEN",
+    "TIME",
+    "TIMESTAMP",
+    "TO",
+    "TRANSFORM",
+    "TRIGGER",
+    "TRUE",
+    "TRUNCATE",
+    "UNBOUNDED",
+    "UNION",
+    "UNIQUEJOIN",
+    "UPDATE",
+    "USER",
+    "USING",
+    "UTC_TIMESTAMP",
+    "VALUES",
+    "VARCHAR",
+    "VIEWS",
+    "WHEN",
+    "WHERE",
+    "WINDOW",
+    "WITH",
+}
+# https://docs.aws.amazon.com/athena/latest/ug/reserved-words.html#list-of-reserved-words-sql-select
+SELECT_STATEMENT_RESERVED_WORDS: Set[str] = {
+    "ALL",
+    "ALTER",
+    "AND",
+    "ARRAY",
+    "AS",
+    "AUTHORIZATION",
+    "BETWEEN",
+    "BIGINT",
+    "BINARY",
+    "BOOLEAN",
+    "BOTH",
+    "BY",
+    "CASE",
+    "CASHE",
+    "CAST",
+    "CHAR",
+    "COLUMN",
+    "COMMIT",
+    "CONF",
+    "CONSTRAINT",
+    "CREATE",
+    "CROSS",
+    "CUBE",
+    "CURRENT",
+    "CURRENT_DATE",
+    "CURRENT_TIMESTAMP",
+    "CURSOR",
+    "DATABASE",
+    "DATE",
+    "DAYOFWEEK",
+    "DECIMAL",
+    "DELETE",
+    "DESCRIBE",
+    "DISTINCT",
+    "DOUBLE",
+    "DROP",
+    "ELSE",
+    "END",
+    "EXCHANGE",
+    "EXISTS",
+    "EXTENDED",
+    "EXTERNAL",
+    "EXTRACT",
+    "FALSE",
+    "FETCH",
+    "FLOAT",
+    "FLOOR",
+    "FOLLOWING",
+    "FOR",
+    "FOREIGN",
+    "FROM",
+    "FULL",
+    "FUNCTION",
+    "GRANT",
+    "GROUP",
+    "GROUPING",
+    "HAVING",
+    "IF",
+    "IMPORT",
+    "IN",
+    "INNER",
+    "INSERT",
+    "INT",
+    "INTEGER",
+    "INTERSECT",
+    "INTERVAL",
+    "INTO",
+    "IS",
+    "JOIN",
+    "LATERAL",
+    "LEFT",
+    "LESS",
+    "LIKE",
+    "LOCAL",
+    "MACRO",
+    "MAP",
+    "MORE",
+    "NONE",
+    "NOT",
+    "NULL",
+    "NUMERIC",
+    "OF",
+    "ON",
+    "ONLY",
+    "OR",
+    "ORDER",
+    "OUT",
+    "OUTER",
+    "OVER",
+    "PARTIALSCAN",
+    "PARTITION",
+    "PERCENT",
+    "PRECEDING",
+    "PRECISION",
+    "PRESERVE",
+    "PRIMARY",
+    "PROCEDURE",
+    "RANGE",
+    "READS",
+    "REDUCE",
+    "REFERENCES",
+    "REGEXP",
+    "REVOKE",
+    "RIGHT",
+    "RLIKE",
+    "ROLLBACK",
+    "ROLLUP",
+    "ROW",
+    "ROWS",
+    "SELECT",
+    "SET",
+    "SMALLINT",
+    "START",
+    "TABLE",
+    "TABLESAMPLE",
+    "THEN",
+    "TIME",
+    "TIMESTAMP",
+    "TO",
+    "TRANSFORM",
+    "TRIGGER",
+    "TRUE",
+    "TRUNCATE",
+    "UNBOUNDED",
+    "UNION",
+    "UNIQUEJOIN",
+    "UPDATE",
+    "USER",
+    "USING",
+    "UTC_TIMESTAMP",
+    "VALUES",
+    "VARCHAR",
+    "VIEWS",
+    "WHEN",
+    "WHERE",
+    "WINDOW",
+    "WITH",
+}
+RESERVED_WORDS: Set[str] = set(sorted(DDL_RESERVED_WORDS | SELECT_STATEMENT_RESERVED_WORDS))
+
+ischema_names: Dict[str, Type[Any]] = {
+    "boolean": types.BOOLEAN,
+    "float": types.FLOAT,
+    "double": types.FLOAT,
+    "real": types.FLOAT,
+    "tinyint": types.INTEGER,
+    "smallint": types.INTEGER,
+    "integer": types.INTEGER,
+    "int": types.INTEGER,
+    "bigint": types.BIGINT,
+    "decimal": types.DECIMAL,
+    "char": types.CHAR,
+    "varchar": types.VARCHAR,
+    "string": types.String,
+    "date": types.DATE,
+    "timestamp": types.TIMESTAMP,
+    "binary": types.BINARY,
+    "varbinary": types.BINARY,
+    "array": types.String,
+    "map": types.String,
+    "struct": types.String,
+    "row": types.String,
+    "json": types.String,
+}
 
 
 class AthenaDMLIdentifierPreparer(IdentifierPreparer):
-    """PrestoIdentifierPreparer
-
-    https://github.com/dropbox/PyHive/blob/master/pyhive/sqlalchemy_presto.py"""
-
-    reserved_words = UniversalSet()
-
-
-class HashableDict(dict):  # type: ignore
-    def __hash__(self):
-        return hash(tuple(sorted(self.items())))
+    reserved_words: Set[str] = SELECT_STATEMENT_RESERVED_WORDS
 
 
 class AthenaDDLIdentifierPreparer(IdentifierPreparer):
+    reserved_words = DDL_RESERVED_WORDS
+    illegal_initial_characters = ILLEGAL_INITIAL_CHARACTERS.union("_")
+
     def __init__(
         self,
-        dialect,
-        initial_quote="`",
-        final_quote=None,
-        escape_quote="`",
-        quote_case_sensitive_collations=True,
-        omit_schema=False,
+        dialect: "Dialect",
+        initial_quote: str = "`",
+        final_quote: Optional[str] = None,
+        escape_quote: str = "`",
+        quote_case_sensitive_collations: bool = True,
+        omit_schema: bool = False,
     ):
         super(AthenaDDLIdentifierPreparer, self).__init__(
             dialect=dialect,
             initial_quote=initial_quote,
             final_quote=final_quote,
             escape_quote=escape_quote,
             quote_case_sensitive_collations=quote_case_sensitive_collations,
             omit_schema=omit_schema,
         )
 
 
 class AthenaStatementCompiler(SQLCompiler):
-    """PrestoCompiler
-
-    https://github.com/dropbox/PyHive/blob/master/pyhive/sqlalchemy_presto.py"""
-
-    def visit_char_length_func(self, fn, **kw):
+    def visit_char_length_func(self, fn: "FunctionElement[Any]", **kw):
         return f"length{self.function_argspec(fn, **kw)}"
 
-    def visit_cast(self, cast, **kwargs):
-        if isinstance(cast.type, types.VARCHAR) and cast.type.length is None:
+    def visit_cast(self, cast: "Cast[Any]", **kwargs):
+        if (isinstance(cast.type, types.VARCHAR) and cast.type.length is None) or isinstance(
+            cast.type, types.String
+        ):
             type_clause = "VARCHAR"
         elif isinstance(cast.type, types.CHAR) and cast.type.length is None:
             type_clause = "CHAR"
+        elif isinstance(cast.type, (types.BINARY, types.VARBINARY)):
+            type_clause = "VARBINARY"
         else:
             type_clause = cast.typeclause._compiler_dispatch(self, **kwargs)
-        return (
-            f"CAST({cast.clause._compiler_dispatch(self, **kwargs)} AS {type_clause})"
-        )
+        return f"CAST({cast.clause._compiler_dispatch(self, **kwargs)} AS {type_clause})"
 
-    def limit_clause(self, select, **kw):
+    def limit_clause(self, select: "GenerativeSelect", **kw):
         text = []
-        # https://docs.sqlalchemy.org/en/14/core/connections.html#example-rendering-limit-offset-with-post-compile-parameters
-        if hasattr(select, "_simple_int_clause"):
-            offset_clause = select._offset_clause
-            if offset_clause is not None and select._simple_int_clause(offset_clause):
-                text.append(
-                    f" OFFSET {self.process(offset_clause.render_literal_execute(), **kw)}"
-                )
-            limit_clause = select._limit_clause
-            if limit_clause is not None and select._simple_int_clause(limit_clause):
-                text.append(
-                    f" LIMIT {self.process(limit_clause.render_literal_execute(), **kw)}"
-                )
-        else:
-            # SQLAlchemy < 1.4
-            if select._offset_clause is not None:
-                text.append(" OFFSET " + self.process(select._offset_clause, **kw))
-            if select._limit_clause is not None:
-                text.append(" LIMIT " + self.process(select._limit_clause, **kw))
+        if select._offset_clause is not None:
+            text.append(" OFFSET " + self.process(select._offset_clause, **kw))
+        if select._limit_clause is not None:
+            text.append(" LIMIT " + self.process(select._limit_clause, **kw))
         return "\n".join(text)
 
 
 class AthenaTypeCompiler(GenericTypeCompiler):
-    def visit_FLOAT(self, type_, **kw):
+    def visit_FLOAT(self, type_: Type[Any], **kw) -> str:
         return self.visit_REAL(type_, **kw)
 
-    def visit_REAL(self, type_, **kw):
+    def visit_REAL(self, type_: Type[Any], **kw) -> str:
         return "DOUBLE"
 
-    def visit_NUMERIC(self, type_, **kw):
+    def visit_NUMERIC(self, type_: Type[Any], **kw) -> str:
         return self.visit_DECIMAL(type_, **kw)
 
-    def visit_DECIMAL(self, type_, **kw):
+    def visit_DECIMAL(self, type_: Type[Any], **kw) -> str:
         if type_.precision is None:
             return "DECIMAL"
         elif type_.scale is None:
             return f"DECIMAL({type_.precision})"
         else:
             return f"DECIMAL({type_.precision}, {type_.scale})"
 
-    def visit_INTEGER(self, type_, **kw):
+    def visit_INTEGER(self, type_: Type[Any], **kw) -> str:
         return "INTEGER"
 
-    def visit_SMALLINT(self, type_, **kw):
+    def visit_SMALLINT(self, type_: Type[Any], **kw) -> str:
         return "SMALLINT"
 
-    def visit_BIGINT(self, type_, **kw):
+    def visit_BIGINT(self, type_: Type[Any], **kw) -> str:
         return "BIGINT"
 
-    def visit_TIMESTAMP(self, type_, **kw):
+    def visit_TIMESTAMP(self, type_: Type[Any], **kw) -> str:
         return "TIMESTAMP"
 
-    def visit_DATETIME(self, type_, **kw):
+    def visit_DATETIME(self, type_: Type[Any], **kw) -> str:
         return self.visit_TIMESTAMP(type_, **kw)
 
-    def visit_DATE(self, type_, **kw):
+    def visit_DATE(self, type_: Type[Any], **kw) -> str:
         return "DATE"
 
-    def visit_TIME(self, type_, **kw):
+    def visit_TIME(self, type_: Type[Any], **kw) -> str:
         raise exc.CompileError(f"Data type `{type_}` is not supported")
 
-    def visit_CLOB(self, type_, **kw):
+    def visit_CLOB(self, type_: Type[Any], **kw) -> str:
         return self.visit_BINARY(type_, **kw)
 
-    def visit_NCLOB(self, type_, **kw):
+    def visit_NCLOB(self, type_: Type[Any], **kw) -> str:
         return self.visit_BINARY(type_, **kw)
 
-    def visit_CHAR(self, type_, **kw):
+    def visit_CHAR(self, type_: Type[Any], **kw) -> str:
         if type_.length:
-            return self._render_string_type(type_, "CHAR")
+            return cast(str, self._render_string_type(type_, "CHAR"))
         return "STRING"
 
-    def visit_NCHAR(self, type_, **kw):
+    def visit_NCHAR(self, type_: Type[Any], **kw) -> str:
         return self.visit_CHAR(type_, **kw)
 
-    def visit_VARCHAR(self, type_, **kw):
+    def visit_VARCHAR(self, type_: Type[Any], **kw) -> str:
         if type_.length:
-            return self._render_string_type(type_, "VARCHAR")
+            return cast(str, self._render_string_type(type_, "VARCHAR"))
         return "STRING"
 
-    def visit_NVARCHAR(self, type_, **kw):
+    def visit_NVARCHAR(self, type_: Type[Any], **kw) -> str:
         return self.visit_VARCHAR(type_, **kw)
 
-    def visit_TEXT(self, type_, **kw):
+    def visit_TEXT(self, type_: Type[Any], **kw) -> str:
         return "STRING"
 
-    def visit_BLOB(self, type_, **kw):
+    def visit_BLOB(self, type_: Type[Any], **kw) -> str:
         return self.visit_BINARY(type_, **kw)
 
-    def visit_BINARY(self, type_, **kw):
+    def visit_BINARY(self, type_: Type[Any], **kw) -> str:
         return "BINARY"
 
-    def visit_VARBINARY(self, type_, **kw):
+    def visit_VARBINARY(self, type_: Type[Any], **kw) -> str:
         return self.visit_BINARY(type_, **kw)
 
-    def visit_BOOLEAN(self, type_, **kw):
+    def visit_BOOLEAN(self, type_: Type[Any], **kw) -> str:
         return "BOOLEAN"
 
+    def visit_string(self, type_, **kw):
+        return "STRING"
+
+    def visit_unicode(self, type_, **kw):
+        return "STRING"
+
+    def visit_unicode_text(self, type_, **kw):
+        return "STRING"
+
 
 class AthenaDDLCompiler(DDLCompiler):
     @property
-    def preparer(self):
+    def preparer(self) -> IdentifierPreparer:
         return self._preparer
 
     @preparer.setter
-    def preparer(self, value):
+    def preparer(self, value: IdentifierPreparer):
         pass
 
     def __init__(
         self,
-        dialect,
-        statement,
-        schema_translate_map=None,
-        compile_kwargs=util.immutabledict(),
+        dialect: "Dialect",
+        statement: "ExecutableDDLElement",
+        schema_translate_map: Optional["SchemaTranslateMapType"] = None,
+        render_schema_translate: bool = False,
+        compile_kwargs: Mapping[str, Any] = util.immutabledict(),
     ):
         self._preparer = AthenaDDLIdentifierPreparer(dialect)
         super(AthenaDDLCompiler, self).__init__(
             dialect=dialect,
             statement=statement,
+            render_schema_translate=render_schema_translate,
             schema_translate_map=schema_translate_map,
             compile_kwargs=compile_kwargs,
         )
 
-    def _raw_connection(self, table):
-        if hasattr(table, "bind") and table.bind:
-            bind = table.bind
-            if isinstance(bind, Engine):
-                conn = bind.raw_connection()
-            else:
-                conn = bind.connection
-        else:
-            conn = None
-        return conn
-
-    def _escape_comment(self, value):
+    def _escape_comment(self, value: str) -> str:
         value = value.replace("\\", "\\\\").replace("'", r"\'")
         # DDL statements raise a KeyError if the placeholders aren't escaped
         if self.dialect.identifier_preparer._double_percents:
             value = value.replace("%", "%%")
         return f"'{value}'"
 
-    def _get_comment_specification(self, comment):
+    def _get_comment_specification(self, comment: str) -> str:
         return f"COMMENT {self._escape_comment(comment)}"
 
-    def _get_bucket_count(self, dialect_opts, raw_connection):
+    def _get_bucket_count(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> Optional[str]:
         if dialect_opts["bucket_count"]:
             bucket_count = dialect_opts["bucket_count"]
-        elif raw_connection:
-            bucket_count = raw_connection._kwargs.get("bucket_count")
+        elif connect_opts:
+            bucket_count = connect_opts.get("bucket_count")
         else:
             bucket_count = None
-        return bucket_count
+        return cast(str, bucket_count) if bucket_count is not None else None
 
-    def _get_file_format(self, dialect_opts, raw_connection):
+    def _get_file_format(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> Optional[str]:
         if dialect_opts["file_format"]:
             file_format = dialect_opts["file_format"]
-        elif raw_connection:
-            file_format = raw_connection._kwargs.get("file_format")
+        elif connect_opts:
+            file_format = connect_opts.get("file_format")
         else:
             file_format = None
-        return file_format
+        return cast(Optional[str], file_format)
 
-    def _get_file_format_specification(self, dialect_opts, raw_connection):
-        file_format = self._get_file_format(dialect_opts, raw_connection)
+    def _get_file_format_specification(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> str:
+        file_format = self._get_file_format(dialect_opts, connect_opts)
         text = []
         if file_format:
             text.append(f"STORED AS {file_format}")
         return "\n".join(text)
 
-    def _get_row_format(self, dialect_opts, raw_connection):
+    def _get_row_format(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> Optional[str]:
         if dialect_opts["row_format"]:
             row_format = dialect_opts["row_format"]
-        elif raw_connection:
-            row_format = raw_connection._kwargs.get("row_format")
+        elif connect_opts:
+            row_format = connect_opts.get("row_format")
         else:
             row_format = None
-        return row_format
+        return cast(Optional[str], row_format)
 
-    def _get_row_format_specification(self, dialect_opts, raw_connection):
-        row_format = self._get_row_format(dialect_opts, raw_connection)
+    def _get_row_format_specification(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> str:
+        row_format = self._get_row_format(dialect_opts, connect_opts)
         text = []
         if row_format:
             text.append(f"ROW FORMAT {row_format}")
         return "\n".join(text)
 
-    def _get_serde_properties(self, dialect_opts, raw_connection):
+    def _get_serde_properties(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> Optional[str]:
         if dialect_opts["serdeproperties"]:
             serde_properties = dialect_opts["serdeproperties"]
-        elif raw_connection:
-            serde_properties = raw_connection._kwargs.get("serdeproperties")
+        elif connect_opts:
+            serde_properties = connect_opts.get("serdeproperties")
         else:
             serde_properties = None
-        return serde_properties
+        return cast(Optional[str], serde_properties)
 
-    def _get_serde_properties_specification(self, dialect_opts, raw_connection):
-        serde_properties = self._get_serde_properties(dialect_opts, raw_connection)
+    def _get_serde_properties_specification(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> str:
+        serde_properties = self._get_serde_properties(dialect_opts, connect_opts)
         text = []
         if serde_properties:
             text.append("WITH SERDEPROPERTIES (")
             if isinstance(serde_properties, dict):
-                text.append(
-                    ",\n".join(
-                        [f"\t'{k}' = '{v}'" for k, v in serde_properties.items()]
-                    )
-                )
+                text.append(",\n".join([f"\t'{k}' = '{v}'" for k, v in serde_properties.items()]))
             else:
                 text.append(serde_properties)
             text.append(")")
         return "\n".join(text)
 
-    def _get_table_location(self, table, dialect_opts, raw_connection):
+    def _get_table_location(
+        self, table, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> Optional[str]:
         if dialect_opts["location"]:
-            location = dialect_opts["location"]
+            location = cast(str, dialect_opts["location"])
             location += "/" if not location.endswith("/") else ""
-        elif raw_connection:
+        elif connect_opts:
             base_location = (
-                raw_connection._kwargs["location"]
-                if "location" in raw_connection._kwargs
-                else raw_connection.s3_staging_dir
+                cast(str, connect_opts["location"])
+                if "location" in connect_opts
+                else cast(str, connect_opts.get("s3_staging_dir"))
             )
-            schema = table.schema if table.schema else raw_connection.schema_name
+            schema = table.schema if table.schema else connect_opts["schema_name"]
             location = f"{base_location}{schema}/{table.name}/"
         else:
             location = None
         return location
 
-    def _get_table_location_specification(self, table, dialect_opts, raw_connection):
-        location = self._get_table_location(table, dialect_opts, raw_connection)
+    def _get_table_location_specification(
+        self, table, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> str:
+        location = self._get_table_location(table, dialect_opts, connect_opts)
         text = []
         if location:
             text.append(f"LOCATION '{location}'")
         else:
-            if raw_connection:
+            if connect_opts:
                 raise exc.CompileError(
                     "`location` or `s3_staging_dir` parameter is required "
                     "in the connection string"
                 )
             else:
                 raise exc.CompileError(
                     "The location of the table should be specified "
                     "by the dialect keyword argument `awsathena_location`"
                 )
         return "\n".join(text)
 
-    def _get_table_properties(self, dialect_opts, raw_connection):
+    def _get_table_properties(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> Optional[Union[Dict[str, str], str]]:
         if dialect_opts["tblproperties"]:
-            table_properties = dialect_opts["tblproperties"]
-        elif raw_connection:
-            table_properties = raw_connection._kwargs.get("tblproperties")
+            table_properties = cast(str, dialect_opts["tblproperties"])
+        elif connect_opts:
+            table_properties = cast(str, connect_opts.get("tblproperties"))
         else:
             table_properties = None
         return table_properties
 
-    def _get_compression(self, dialect_opts, raw_connection):
+    def _get_compression(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> Optional[str]:
         if dialect_opts["compression"]:
-            compression = dialect_opts["compression"]
-        elif raw_connection:
-            compression = raw_connection._kwargs.get("compression")
+            compression = cast(str, dialect_opts["compression"])
+        elif connect_opts:
+            compression = cast(str, connect_opts.get("compression"))
         else:
             compression = None
         return compression
 
-    def _get_table_properties_specification(self, dialect_opts, raw_connection):
-        table_properties = self._get_table_properties(dialect_opts, raw_connection)
-        if table_properties:
-            if isinstance(table_properties, dict):
-                table_properties = [
-                    ",\n".join(
-                        [f"\t'{k}' = '{v}'" for k, v in table_properties.items()]
-                    )
-                ]
+    def _get_table_properties_specification(
+        self, dialect_opts: "_DialectArgDict", connect_opts: Dict[str, Any]
+    ) -> str:
+        properties = self._get_table_properties(dialect_opts, connect_opts)
+        if properties:
+            if isinstance(properties, dict):
+                table_properties = [",\n".join([f"\t'{k}' = '{v}'" for k, v in properties.items()])]
             else:
-                table_properties = [table_properties]
+                table_properties = [properties]
         else:
             table_properties = []
 
-        compression = self._get_compression(dialect_opts, raw_connection)
+        compression = self._get_compression(dialect_opts, connect_opts)
         if compression:
-            file_format = self._get_file_format(dialect_opts, raw_connection)
-            row_format = self._get_row_format(dialect_opts, raw_connection)
+            file_format = self._get_file_format(dialect_opts, connect_opts)
+            row_format = self._get_row_format(dialect_opts, connect_opts)
             if file_format:
                 if file_format == AthenaFileFormat.FILE_FORMAT_PARQUET:
                     table_properties.append(f"\t'parquet.compress' = '{compression}'")
                 elif file_format == AthenaFileFormat.FILE_FORMAT_ORC:
                     table_properties.append(f"\t'orc.compress' = '{compression}'")
                 else:
                     table_properties.append(f"\t'write.compress' = '{compression}'")
@@ -371,174 +711,181 @@
                 if AthenaRowFormatSerde.is_parquet(row_format):
                     table_properties.append(f"\t'parquet.compress' = '{compression}'")
                 elif AthenaRowFormatSerde.is_orc(row_format):
                     table_properties.append(f"\t'orc.compress' = '{compression}'")
                 else:
                     table_properties.append(f"\t'write.compress' = '{compression}'")
 
-        table_properties = ",\n".join(table_properties)
         text = []
         if table_properties:
             text.append("TBLPROPERTIES (")
-            text.append(table_properties)
+            text.append(",\n".join(table_properties))
             text.append(")")
         return "\n".join(text)
 
-    def get_column_specification(self, column, **kwargs):
+    def get_column_specification(self, column: "Column[Any]", **kwargs) -> str:
         if isinstance(column.type, (types.Integer, types.INTEGER, types.INT)):
             # https://docs.aws.amazon.com/athena/latest/ug/create-table.html
             # In Data Definition Language (DDL) queries like CREATE TABLE,
             # use the int keyword to represent an integer
             type_ = "INT"
         else:
-            type_ = self.dialect.type_compiler.process(
-                column.type, type_expression=column
-            )
+            type_ = self.dialect.type_compiler.process(column.type, type_expression=column)
         text = [f"{self.preparer.format_column(column)} {type_}"]
         if column.comment:
             text.append(f"{self._get_comment_specification(column.comment)}")
         return " ".join(text)
 
-    def visit_check_constraint(self, constraint, **kw):
+    def visit_check_constraint(self, constraint: "CheckConstraint", **kw) -> Optional[str]:
         return None
 
-    def visit_column_check_constraint(self, constraint, **kw):
+    def visit_column_check_constraint(self, constraint: "CheckConstraint", **kw) -> Optional[str]:
         return None
 
-    def visit_foreign_key_constraint(self, constraint, **kw):
+    def visit_foreign_key_constraint(
+        self, constraint: "ForeignKeyConstraint", **kw
+    ) -> Optional[str]:
         return None
 
-    def visit_primary_key_constraint(self, constraint, **kw):
+    def visit_primary_key_constraint(
+        self, constraint: "PrimaryKeyConstraint", **kw
+    ) -> Optional[str]:
         return None
 
-    def visit_unique_constraint(self, constraint, **kw):
+    def visit_unique_constraint(self, constraint: "UniqueConstraint", **kw) -> Optional[str]:
         return None
 
-    def _get_raw_connection_partitions(self, raw_connection):
-        if raw_connection:
-            partition = raw_connection._kwargs.get("partition")
+    def _get_connect_option_partitions(self, connect_opts: Dict[str, Any]) -> List[str]:
+        if connect_opts:
+            partition = cast(str, connect_opts.get("partition"))
             partitions = partition.split(",") if partition else []
         else:
             partitions = []
         return partitions
 
-    def _get_raw_connection_buckets(self, raw_connection):
-        if raw_connection:
-            bucket = raw_connection._kwargs.get("cluster")
+    def _get_connect_option_buckets(self, connect_opts: Dict[str, Any]) -> List[str]:
+        if connect_opts:
+            bucket = cast(str, connect_opts.get("cluster"))
             buckets = bucket.split(",") if bucket else []
         else:
             buckets = []
         return buckets
 
-    def _prepared_columns(self, table, create_columns, raw_connection):
+    def _prepared_columns(
+        self, table, create_columns: List["CreateColumn"], connect_opts: Dict[str, Any]
+    ) -> Tuple[List[str], List[str], List[str]]:
         columns, partitions, buckets = [], [], []
-        raw_conn_partitions = self._get_raw_connection_partitions(raw_connection)
-        raw_conn_buckets = self._get_raw_connection_buckets(raw_connection)
+        conn_partitions = self._get_connect_option_partitions(connect_opts)
+        conn_buckets = self._get_connect_option_buckets(connect_opts)
         for create_column in create_columns:
             column = create_column.element
             column_dialect_opts = column.dialect_options["awsathena"]
             try:
                 processed = self.process(create_column)
                 if processed is not None:
                     if (
                         column_dialect_opts["partition"]
-                        or column.name in raw_conn_partitions
-                        or f"{table.name}.{column.name}" in raw_conn_partitions
+                        or column.name in conn_partitions
+                        or f"{table.name}.{column.name}" in conn_partitions
                     ):
                         partitions.append(f"\t{processed}")
                     else:
                         columns.append(f"\t{processed}")
                     if (
                         column_dialect_opts["cluster"]
-                        or column.name in raw_conn_buckets
-                        or f"{table.name}.{column.name}" in raw_conn_buckets
+                        or column.name in conn_buckets
+                        or f"{table.name}.{column.name}" in conn_buckets
                     ):
                         buckets.append(f"\t{self.preparer.format_column(column)}")
             except exc.CompileError as ce:
-                util.raise_(
-                    exc.CompileError(
-                        util.u(
-                            f"(in table '{table.description}', column '{column.name}'): "
-                            f"{ce.args[0]}"
-                        )
-                    ),
-                    from_=ce,
-                )
+                raise exc.CompileError(
+                    f"(in table '{table.description}', column '{column.name}'): {ce.args[0]}"
+                ) from ce
         return columns, partitions, buckets
 
-    def visit_create_table(self, create, **kwargs):
+    def visit_create_table(self, create: "CreateTable", **kwargs) -> str:
         table = create.element
-        table_dialect_opts = table.dialect_options["awsathena"]
-        raw_connection = self._raw_connection(table)
+        dialect_opts = table.dialect_options["awsathena"]
+        dialect = cast(AthenaDialect, self.dialect)
+        connect_opts = dialect._connect_options
+
+        table_properties = self._get_table_properties_specification(
+            dialect_opts, connect_opts
+        ).lower()
+        if ("table_type" in table_properties) and ("iceberg" in table_properties):
+            # https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-creating-tables.html
+            text = ["\nCREATE TABLE"]
+        else:
+            text = ["\nCREATE EXTERNAL TABLE"]
 
-        text = ["\nCREATE EXTERNAL TABLE"]
         if create.if_not_exists:
             text.append("IF NOT EXISTS")
         text.append(self.preparer.format_table(table))
         text.append("(")
         text = [" ".join(text)]
 
-        columns, partitions, buckets = self._prepared_columns(
-            table, create.columns, raw_connection
-        )
+        columns, partitions, buckets = self._prepared_columns(table, create.columns, connect_opts)
         text.append(",\n".join(columns))
         text.append(")")
 
         if table.comment:
             text.append(self._get_comment_specification(table.comment))
 
         if partitions:
             text.append("PARTITIONED BY (")
             text.append(",\n".join(partitions))
             text.append(")")
 
-        bucket_count = self._get_bucket_count(table_dialect_opts, raw_connection)
+        bucket_count = self._get_bucket_count(dialect_opts, connect_opts)
         if buckets and bucket_count:
             text.append("CLUSTERED BY (")
             text.append(",\n".join(buckets))
             text.append(f") INTO {bucket_count} BUCKETS")
 
         text.append(f"{self.post_create_table(table)}\n")
         return "\n".join(text)
 
-    def post_create_table(self, table):
-        dialect_opts = table.dialect_options["awsathena"]
-        raw_connection = self._raw_connection(table)
+    def post_create_table(self, table: "Table") -> str:
+        dialect_opts: "_DialectArgDict" = table.dialect_options["awsathena"]
+        dialect = cast(AthenaDialect, self.dialect)
+        connect_opts = dialect._connect_options
         text = [
-            self._get_row_format_specification(dialect_opts, raw_connection),
-            self._get_serde_properties_specification(dialect_opts, raw_connection),
-            self._get_file_format_specification(dialect_opts, raw_connection),
-            self._get_table_location_specification(table, dialect_opts, raw_connection),
-            self._get_table_properties_specification(dialect_opts, raw_connection),
+            self._get_row_format_specification(dialect_opts, connect_opts),
+            self._get_serde_properties_specification(dialect_opts, connect_opts),
+            self._get_file_format_specification(dialect_opts, connect_opts),
+            self._get_table_location_specification(table, dialect_opts, connect_opts),
+            self._get_table_properties_specification(dialect_opts, connect_opts),
         ]
         return "\n".join([t for t in text if t])
 
 
 class AthenaDialect(DefaultDialect):
-
-    name = "awsathena"
-    preparer = AthenaDMLIdentifierPreparer
-    statement_compiler = AthenaStatementCompiler
-    ddl_compiler = AthenaDDLCompiler
-    type_compiler = AthenaTypeCompiler
-    default_paramstyle = pyathena.paramstyle
-    supports_alter = False
-    supports_pk_autoincrement = False
-    supports_default_values = False
-    supports_empty_insert = False
-    supports_multivalues_insert = True
-    supports_native_decimal = True
-    supports_native_boolean = True
-    supports_unicode_statements = True
-    supports_unicode_binds = True
-    supports_statement_cache = True
-    returns_unicode_strings = True
-    description_encoding = None
-    postfetch_lastrowid = False
-    construct_arguments = [
+    name: str = "awsathena"
+    preparer: Type[IdentifierPreparer] = AthenaDMLIdentifierPreparer
+    statement_compiler: Type[SQLCompiler] = AthenaStatementCompiler
+    ddl_compiler: Type[DDLCompiler] = AthenaDDLCompiler
+    type_compiler: Type[GenericTypeCompiler] = AthenaTypeCompiler
+    default_paramstyle: str = pyathena.paramstyle
+    cte_follows_insert: bool = True
+    supports_alter: bool = False
+    supports_pk_autoincrement: Optional[bool] = False
+    supports_default_values: bool = False
+    supports_empty_insert: bool = False
+    supports_multivalues_insert: bool = True
+    supports_native_decimal: bool = True
+    supports_native_boolean: bool = True
+    supports_unicode_statements: Optional[bool] = True
+    supports_unicode_binds: Optional[bool] = True
+    supports_statement_cache: bool = True
+    returns_unicode_strings: Optional[bool] = True
+    description_encoding: Optional[bool] = None
+    postfetch_lastrowid: bool = False
+    construct_arguments: Optional[
+        List[Tuple[Type[Union["SchemaItem", "ClauseElement"]], Mapping[str, Any]]]
+    ] = [
         (
             schema.Table,
             {
                 "location": None,
                 "compression": None,
                 "row_format": None,
                 "file_format": None,
@@ -552,128 +899,164 @@
             {
                 "partition": False,
                 "cluster": False,
             },
         ),
     ]
 
-    _pattern_column_type = re.compile(r"^([a-zA-Z]+)(?:$|[\(|<](.+)[\)|>]$)")
+    colspecs = {
+        types.DATE: AthenaDate,
+        types.DATETIME: AthenaTimestamp,
+        types.TIMESTAMP: AthenaTimestamp,
+    }
+
+    ischema_names: Dict[str, Type[Any]] = ischema_names
+
+    _connect_options: Dict[str, Any] = dict()  # type: ignore
+    _pattern_column_type: Pattern[str] = re.compile(r"^([a-zA-Z]+)(?:$|[\(|<](.+)[\)|>]$)")
 
     @classmethod
-    def dbapi(cls):
+    def import_dbapi(cls) -> "ModuleType":
         return pyathena
 
-    def _raw_connection(self, connection):
+    def _raw_connection(self, connection: Union[Engine, "Connection"]) -> "PoolProxiedConnection":
         if isinstance(connection, Engine):
             return connection.raw_connection()
         return connection.connection
 
-    def create_connect_args(self, url):
+    def create_connect_args(self, url: "URL") -> Tuple[Tuple[str], MutableMapping[str, Any]]:
         # Connection string format:
         #   awsathena+rest://
         #   {aws_access_key_id}:{aws_secret_access_key}@athena.{region_name}.amazonaws.com:443/
         #   {schema_name}?s3_staging_dir={s3_staging_dir}&...
-        opts = self._create_connect_args(url)
-        return [[], opts]
+        self._connect_options = self._create_connect_args(url)
+        return cast(Tuple[str], tuple()), self._connect_options
 
-    def _create_connect_args(self, url):
-        opts = {
+    def _create_connect_args(self, url: "URL") -> Dict[str, Any]:
+        opts: Dict[str, Any] = {
             "aws_access_key_id": url.username if url.username else None,
             "aws_secret_access_key": url.password if url.password else None,
             "region_name": re.sub(
                 r"^athena\.([a-z0-9-]+)\.amazonaws\.(com|com.cn)$", r"\1", url.host
-            ),
+            )
+            if url.host
+            else None,
             "schema_name": url.database if url.database else "default",
         }
         opts.update(url.query)
         if "verify" in opts:
             verify = opts["verify"]
             try:
                 verify = bool(strtobool(verify))
             except ValueError:
                 # Probably a file name of the CA cert bundle to use
                 pass
             opts.update({"verify": verify})
         if "duration_seconds" in opts:
-            opts.update({"duration_seconds": int(url.query["duration_seconds"])})
+            opts.update({"duration_seconds": int(opts["duration_seconds"])})
         if "poll_interval" in opts:
-            opts.update({"poll_interval": float(url.query["poll_interval"])})
+            opts.update({"poll_interval": float(opts["poll_interval"])})
         if "kill_on_interrupt" in opts:
-            opts.update(
-                {"kill_on_interrupt": bool(strtobool(url.query["kill_on_interrupt"]))}
-            )
+            opts.update({"kill_on_interrupt": bool(strtobool(opts["kill_on_interrupt"]))})
         return opts
 
     @reflection.cache
-    def get_schema_names(self, connection, **kw):
-        query = """
-                SELECT schema_name
-                FROM information_schema.schemata
-                WHERE schema_name NOT IN ('information_schema')
-                """
-        return [row.schema_name for row in connection.execute(query).fetchall()]
+    def _get_schemas(self, connection, **kw):
+        raw_connection = self._raw_connection(connection)
+        catalog = raw_connection.catalog_name  # type: ignore
+        with raw_connection.driver_connection.cursor() as cursor:  # type: ignore
+            try:
+                return cursor.list_databases(catalog)
+            except pyathena.error.OperationalError as exc:
+                cause = exc.__cause__
+                if (
+                    isinstance(cause, botocore.exceptions.ClientError)
+                    and cause.response["Error"]["Code"] == "InvalidRequestException"
+                ):
+                    return []
+                raise
 
     @reflection.cache
-    def _get_table(self, connection, table_name, schema=None, **kw):
+    def _get_table(self, connection, table_name: str, schema: Optional[str] = None, **kw):
         raw_connection = self._raw_connection(connection)
-        schema = schema if schema else raw_connection.schema_name
-        with raw_connection.connection.cursor() as cursor:
+        schema = schema if schema else raw_connection.schema_name  # type: ignore
+        with raw_connection.driver_connection.cursor() as cursor:  # type: ignore
             try:
-                return cursor.get_table_metadata(table_name, schema_name=schema)
+                return cursor.get_table_metadata(table_name, schema_name=schema, logging_=False)
             except pyathena.error.OperationalError as exc:
                 cause = exc.__cause__
                 if (
                     isinstance(cause, botocore.exceptions.ClientError)
                     and cause.response["Error"]["Code"] == "MetadataException"
                 ):
                     raise NoSuchTableError(table_name) from exc
                 raise
 
     @reflection.cache
-    def _get_tables(self, connection, schema=None, **kw):
+    def _get_tables(self, connection, schema: Optional[str] = None, **kw):
         raw_connection = self._raw_connection(connection)
-        schema = schema if schema else raw_connection.schema_name
-        with raw_connection.connection.cursor() as cursor:
+        schema = schema if schema else raw_connection.schema_name  # type: ignore
+        with raw_connection.driver_connection.cursor() as cursor:  # type: ignore
             return cursor.list_table_metadata(schema_name=schema)
 
-    def get_table_names(self, connection, schema=None, **kw):
+    def get_schema_names(self, connection, **kw):
+        schemas = self._get_schemas(connection, **kw)
+        return [s.name for s in schemas]
+
+    def get_table_names(self, connection: "Connection", schema: Optional[str] = None, **kw):
+        # Tables created by Athena are always classified as `EXTERNAL_TABLE`,
+        # but Athena can also query tables classified as `MANAGED_TABLE`.
+        # Managed Tables are created by default when creating tables via Spark when
+        # Glue has been enabled as the Hive Metastore for Elastic Map Reduce (EMR) clusters.
+        # With Athena Federation, tables in the database that are connected to Athena via lambda
+        # function, is classified as `EXTERNAL` and fully queryable
         tables = self._get_tables(connection, schema, **kw)
-        # In Athena, only EXTERNAL_TABLE is supported.
-        # https://docs.aws.amazon.com/athena/latest/APIReference/API_TableMetadata.html
-        return [t.name for t in tables if t.table_type == "EXTERNAL_TABLE"]
+        return [
+            t.name
+            for t in tables
+            if t.table_type in ["EXTERNAL_TABLE", "MANAGED_TABLE", "EXTERNAL"]
+        ]
 
-    def get_view_names(self, connection, schema=None, **kw):
+    def get_view_names(self, connection: "Connection", schema: Optional[str] = None, **kw):
         tables = self._get_tables(connection, schema, **kw)
         return [t.name for t in tables if t.table_type == "VIRTUAL_VIEW"]
 
-    def get_table_comment(self, connection, table_name, schema=None, **kw):
+    def get_table_comment(
+        self, connection: "Connection", table_name: str, schema: Optional[str] = None, **kw
+    ):
         metadata = self._get_table(connection, table_name, schema=schema, **kw)
         return {"text": metadata.comment}
 
-    def get_table_options(self, connection, table_name, schema=None, **kw):
+    def get_table_options(
+        self, connection: "Connection", table_name: str, schema: Optional[str] = None, **kw
+    ):
         metadata = self._get_table(connection, table_name, schema=schema, **kw)
         # TODO The metadata retrieved from the API does not seem to include bucketing information.
         return {
             "awsathena_location": metadata.location,
             "awsathena_compression": metadata.compression,
             "awsathena_row_format": metadata.row_format,
             "awsathena_file_format": metadata.file_format,
-            "awsathena_serdeproperties": HashableDict(metadata.serde_properties),
-            "awsathena_tblproperties": HashableDict(metadata.table_properties),
+            "awsathena_serdeproperties": _HashableDict(metadata.serde_properties),
+            "awsathena_tblproperties": _HashableDict(metadata.table_properties),
         }
 
-    def has_table(self, connection, table_name, schema=None, **kw):
+    def has_table(
+        self, connection: "Connection", table_name: str, schema: Optional[str] = None, **kw
+    ):
         try:
             columns = self.get_columns(connection, table_name, schema)
             return True if columns else False
         except NoSuchTableError:
             return False
 
     @reflection.cache
-    def get_columns(self, connection, table_name, schema=None, **kw):
+    def get_columns(
+        self, connection: "Connection", table_name: str, schema: Optional[str] = None, **kw
+    ):
         metadata = self._get_table(connection, table_name, schema=schema, **kw)
         columns = [
             {
                 "name": c.name,
                 "type": self._get_column_type(c.type),
                 "nullable": True,
                 "default": None,
@@ -693,109 +1076,63 @@
                 "comment": c.comment,
                 "dialect_options": {"awsathena_partition": True},
             }
             for c in metadata.partition_keys
         ]
         return columns
 
-    def _get_column_type(self, type_):
+    def _get_column_type(self, type_: str):
         match = self._pattern_column_type.match(type_)
         if match:
             name = match.group(1).lower()
             length = match.group(2)
         else:
             name = type_.lower()
             length = None
 
+        if name in self.ischema_names:
+            col_type = self.ischema_names[name]
+        else:
+            util.warn(f"Did not recognize type '{type_}'")
+            col_type = types.NullType
+
         args = []
-        if name in ["boolean"]:
-            col_type = types.BOOLEAN
-        elif name in ["float", "double", "real"]:
-            col_type = types.FLOAT
-        elif name in ["tinyint", "smallint", "integer", "int"]:
-            col_type = types.INTEGER
-        elif name in ["bigint"]:
-            col_type = types.BIGINT
-        elif name in ["decimal"]:
-            col_type = types.DECIMAL
-            if length:
+        if length:
+            if col_type is types.DECIMAL:
                 precision, scale = length.split(",")
                 args = [int(precision), int(scale)]
-        elif name in ["char"]:
-            col_type = types.CHAR
-            if length:
-                args = [int(length)]
-        elif name in ["varchar"]:
-            col_type = types.VARCHAR
-            if length:
+            elif col_type is types.CHAR or col_type is types.VARCHAR:
                 args = [int(length)]
-        elif name in ["string"]:
-            col_type = types.String
-        elif name in ["date"]:
-            col_type = types.DATE
-        elif name in ["timestamp"]:
-            col_type = types.TIMESTAMP
-        elif name in ["binary", "varbinary"]:
-            col_type = types.BINARY
-        elif name in ["array", "map", "struct", "row", "json"]:
-            col_type = types.String
-        else:
-            util.warn(f"Did not recognize type '{type_}'")
-            col_type = types.NullType
+
         return col_type(*args)
 
-    def get_foreign_keys(self, connection, table_name, schema=None, **kw):
+    def get_foreign_keys(
+        self, connection: "Connection", table_name: str, schema: Optional[str] = None, **kw
+    ) -> List["ReflectedForeignKeyConstraint"]:
         # Athena has no support for foreign keys.
         return []  # pragma: no cover
 
-    def get_pk_constraint(self, connection, table_name, schema=None, **kw):
+    def get_pk_constraint(
+        self, connection: "Connection", table_name: str, schema: Optional[str] = None, **kw
+    ) -> "ReflectedPrimaryKeyConstraint":
         # Athena has no support for primary keys.
-        return []  # pragma: no cover
+        return {"name": None, "constrained_columns": []}  # pragma: no cover
 
-    def get_indexes(self, connection, table_name, schema=None, **kw):
+    def get_indexes(
+        self, connection: "Connection", table_name: str, schema: Optional[str] = None, **kw
+    ) -> List["ReflectedIndex"]:
         # Athena has no support for indexes.
         return []  # pragma: no cover
 
-    def do_rollback(self, dbapi_connection):
+    def do_rollback(self, dbapi_connection: "PoolProxiedConnection") -> None:
         # No transactions for Athena
         pass  # pragma: no cover
 
-    def _check_unicode_returns(self, connection, additional_tests=None):
+    def _check_unicode_returns(
+        self, connection: "Connection", additional_tests: Optional[List[Any]] = None
+    ) -> bool:
         # Requests gives back Unicode strings
         return True  # pragma: no cover
 
-    def _check_unicode_description(self, connection):
+    def _check_unicode_description(self, connection: "Connection") -> bool:
         # Requests gives back Unicode strings
         return True  # pragma: no cover
-
-
-class AthenaRestDialect(AthenaDialect):
-    driver = "rest"
-    supports_statement_cache = True
-
-
-class AthenaPandasDialect(AthenaDialect):
-    driver = "pandas"
-    supports_statement_cache = True
-
-    def create_connect_args(self, url):
-        from pyathena.pandas.cursor import PandasCursor
-
-        opts = super()._create_connect_args(url)
-        opts.update({"cursor_class": PandasCursor})
-        return [[], opts]
-
-
-class AthenaArrowDialect(AthenaDialect):
-    driver = "arrow"
-    supports_statement_cache = True
-
-    def create_connect_args(self, url):
-        from pyathena.arrow.cursor import ArrowCursor
-
-        opts = super()._create_connect_args(url)
-        opts.update({"cursor_class": ArrowCursor})
-        if "unload" in opts:
-            opts.update(
-                {"cursor_kwargs": {"unload": bool(strtobool(url.query["unload"]))}}
-            )
-        return [[], opts]
```

### Comparing `PyAthena-2.9.6/pyathena/util.py` & `pyathena-3.0.0/pyathena/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # -*- coding: utf-8 -*-
-import functools
 import logging
 import re
-import threading
-from typing import Any, Callable, Iterable, Pattern, Tuple
+from typing import Any, Callable, Iterable, Optional, Pattern, Tuple
 
 import tenacity
 from tenacity import after_log, retry_if_exception, stop_after_attempt, wait_exponential
 
 from pyathena import DataError
 
 _logger = logging.getLogger(__name__)  # type: ignore
@@ -21,28 +19,14 @@
     match = PATTERN_OUTPUT_LOCATION.search(output_location)
     if match:
         return match.group("bucket"), match.group("key")
     else:
         raise DataError("Unknown `output_location` format.")
 
 
-def synchronized(wrapped: Callable[..., Any]) -> Any:
-    """The missing @synchronized decorator
-
-    https://git.io/vydTA"""
-    _lock = threading.RLock()
-
-    @functools.wraps(wrapped)
-    def _wrapper(*args, **kwargs):
-        with _lock:
-            return wrapped(*args, **kwargs)
-
-    return _wrapper
-
-
 class RetryConfig:
     def __init__(
         self,
         exceptions: Iterable[str] = (
             "ThrottlingException",
             "TooManyRequestsException",
         ),
@@ -57,17 +41,17 @@
         self.max_delay = max_delay
         self.exponential_base = exponential_base
 
 
 def retry_api_call(
     func: Callable[..., Any],
     config: RetryConfig,
-    logger: logging.Logger = None,
+    logger: Optional[logging.Logger] = None,
     *args,
-    **kwargs
+    **kwargs,
 ) -> Any:
     retry = tenacity.Retrying(
         retry=retry_if_exception(
             lambda e: getattr(e, "response", {}).get("Error", {}).get("Code", None)
             in config.exceptions
             if e
             else False
```

### Comparing `PyAthena-2.9.6/pyproject.toml` & `pyathena-3.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,139 @@
 [tool.poetry]
 name = "PyAthena"
-version = "2.9.6"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L7
+version = "3.0.0"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
 description = "Python DB API 2.0 (PEP 249) client for Amazon Athena"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Database :: Front-Ends",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
 ]
 homepage = "https://github.com/laughingman7743/PyAthena/"
 authors = [
     "laughingman7743 <laughingman7743@gmail.com>"
 ]
 readme = "README.rst"
 packages = [
     { include = "pyathena" },
 ]
 include = [
     { path = "pyathena/py.typed" },
 ]
 
 [tool.poetry.dependencies]
-# https://github.com/pandas-dev/pandas/pull/35214
-python = "^3.7.1"
-boto3 = ">=1.13.20"
-botocore = ">=1.16.20"
+# https://bugs.python.org/issue38342
+python = ">=3.8.1"
+boto3 = ">=1.26.4"
+botocore = ">=1.29.4"
 tenacity = ">=4.1.0"
-sqlalchemy = {version = "<2.0.0,>=1.0.0", optional = true}
+fsspec = "*"
+sqlalchemy = {version = ">=1.0.0", optional = true}
 pandas = {version = ">=1.3.0", optional = true}
 pyarrow = {version = ">=7.0.0", optional = true}
-s3fs = {version = ">=2021.09.0", optional = true}
+fastparquet = {version = ">=0.4.0", optional = true}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 tox = "*"
 tox-gh-actions = "*"
 wheel = "*"
 twine = "*"
-sqlalchemy = ">=1.0.0, <2.0.0"
+sqlalchemy = ">=1.0.0"
 pandas = ">=1.3.0"
+numpy = ">=1.24.0"
 pyarrow = ">=7.0.0"
-s3fs = ">=2021.09.0"
+fastparquet = ">=0.4.0"
 Jinja2 = ">=3.1.0"
+isort = ">=5.10.1"
 black = ">=22.3.0"
 mypy = ">=0.900"
 flake8 = "*"
 pytest = ">=3.5"
 pytest-cov = "*"
-pytest-flake8 = ">=1.0.1"
-pytest-black = "*"
-pytest-isort = "*"
 pytest-xdist = "*"
-pytest-mypy = "*"
 
 [tool.poetry.extras]
-pandas = ["pandas", "pyarrow", "s3fs"]
+pandas = ["pandas"]
 sqlalchemy = ["sqlalchemy"]
 arrow = ["pyarrow"]
+fastparquet = ["fastparquet"]
 
 [tool.poetry.plugins."sqlalchemy.dialects"]
-"awsathena" = "pyathena.sqlalchemy_athena:AthenaDialect"
-"awsathena.rest" = "pyathena.sqlalchemy_athena:AthenaRestDialect"
-"awsathena.pandas" = "pyathena.sqlalchemy_athena:AthenaPandasDialect"
-"awsathena.arrow" = "pyathena.sqlalchemy_athena:AthenaArrowDialect"
+"awsathena" = "pyathena.sqlalchemy.base:AthenaDialect"
+"awsathena.rest" = "pyathena.sqlalchemy.rest:AthenaRestDialect"
+"awsathena.pandas" = "pyathena.sqlalchemy.pandas:AthenaPandasDialect"
+"awsathena.arrow" = "pyathena.sqlalchemy.arrow:AthenaArrowDialect"
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+isolated_build = true
+envlist = py{38,39,310,311},py{38,39,310,311}-sqla
+
+[gh-actions]
+python =
+    3.8: py38
+    3.9: py39
+    3.10: py310
+    3.11: py311
+
+[testenv]
+allowlist_externals =
+    poetry
+    make
+commands =
+    poetry install -v
+    make chk
+    poetry run pytest -n 8 --cov pyathena --cov-report html --cov-report term tests/pyathena/
+passenv =
+    AWS_*
+    TOXENV
+    GITHUB_*
+
+[testenv:py{38,39,310,311}-sqla]
+commands =
+    poetry install -v
+    poetry run pytest -n 8 --cov pyathena --cov-report html --cov-report term tests/sqlalchemy/
+"""
 
 [tool.pytest.ini_options]
-flake8-max-line-length = 100
-norecursedirs = "benchmarks"
+norecursedirs = ["benchmarks", ".poetry", ".tox"]
+
+[tool.black]
+line-length = 100
+target-version = ['py38']
+exclude = '(\.poetry|\.tox)'
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
+skip_glob = [".poetry/*", ".tox/*"]
 
 [tool.mypy]
-python_version = 3.7
+python_version = 3.8
 follow_imports = "silent"
 disallow_any_generics = true
 strict_optional = true
 check_untyped_defs = true
 allow_redefinition = true
 ignore_missing_imports = true
 warn_redundant_casts = true
 warn_no_return = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
+exclude = ["benchmarks.*", "tests.*", ".poetry.*", ".tox.*"]
 
-[[tool.mypy.overrides]]
-module = ["benchmarks.*", "tests.*"]
-ignore_errors = true
+[tool.sqla_testing]
+requirement_cls = "pyathena.sqlalchemy.requirements:Requirements"
+profile_file = "tests/sqlalchemy/profiles.txt"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `PyAthena-2.9.6/setup.py` & `pyathena-3.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,2046 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyathena
+Version: 3.0.0
+Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
+Home-page: https://github.com/laughingman7743/PyAthena/
+License: MIT
+Author: laughingman7743
+Author-email: laughingman7743@gmail.com
+Requires-Python: >=3.8.1
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Database :: Front-Ends
+Provides-Extra: arrow
+Provides-Extra: fastparquet
+Provides-Extra: pandas
+Provides-Extra: sqlalchemy
+Requires-Dist: boto3 (>=1.26.4)
+Requires-Dist: botocore (>=1.29.4)
+Requires-Dist: fastparquet (>=0.4.0) ; extra == "fastparquet"
+Requires-Dist: fsspec
+Requires-Dist: pandas (>=1.3.0) ; extra == "pandas"
+Requires-Dist: pyarrow (>=7.0.0) ; extra == "arrow"
+Requires-Dist: sqlalchemy (>=1.0.0) ; extra == "sqlalchemy"
+Requires-Dist: tenacity (>=4.1.0)
+Description-Content-Type: text/x-rst
 
-packages = \
-['pyathena', 'pyathena.arrow', 'pyathena.pandas']
+.. image:: https://badge.fury.io/py/pyathena.svg
+    :target: https://badge.fury.io/py/pyathena
 
-package_data = \
-{'': ['*']}
+.. image:: https://img.shields.io/pypi/pyversions/PyAthena.svg
+    :target: https://pypi.org/project/PyAthena/
 
-install_requires = \
-['boto3>=1.13.20', 'botocore>=1.16.20', 'tenacity>=4.1.0']
-
-extras_require = \
-{'arrow': ['pyarrow>=7.0.0'],
- 'pandas': ['pandas>=1.3.0', 'pyarrow>=7.0.0', 's3fs>=2021.09.0'],
- 'sqlalchemy': ['sqlalchemy>=1.0.0,<2.0.0']}
-
-entry_points = \
-{'sqlalchemy.dialects': ['awsathena = pyathena.sqlalchemy_athena:AthenaDialect',
-                         'awsathena.arrow = '
-                         'pyathena.sqlalchemy_athena:AthenaArrowDialect',
-                         'awsathena.pandas = '
-                         'pyathena.sqlalchemy_athena:AthenaPandasDialect',
-                         'awsathena.rest = '
-                         'pyathena.sqlalchemy_athena:AthenaRestDialect']}
-
-setup_kwargs = {
-    'name': 'pyathena',
-    'version': '2.9.6',
-    'description': 'Python DB API 2.0 (PEP 249) client for Amazon Athena',
-    'long_description': '.. image:: https://img.shields.io/pypi/pyversions/PyAthena.svg\n    :target: https://pypi.org/project/PyAthena/\n\n.. image:: https://github.com/laughingman7743/PyAthena/actions/workflows/test.yaml/badge.svg\n    :target: https://github.com/laughingman7743/PyAthena/actions/workflows/test.yaml\n\n.. image:: https://img.shields.io/pypi/l/PyAthena.svg\n    :target: https://github.com/laughingman7743/PyAthena/blob/master/LICENSE\n\n.. image:: https://pepy.tech/badge/pyathena/month\n    :target: https://pepy.tech/project/pyathena\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n\nPyAthena\n========\n\nPyAthena is a Python `DB API 2.0 (PEP 249)`_ client for `Amazon Athena`_.\n\n.. _`DB API 2.0 (PEP 249)`: https://www.python.org/dev/peps/pep-0249/\n.. _`Amazon Athena`: https://docs.aws.amazon.com/athena/latest/APIReference/Welcome.html\n\n.. contents:: Table of Contents:\n   :local:\n   :depth: 2\n\nRequirements\n------------\n\n* Python\n\n  - CPython 3.7 3.8 3.9 3.10\n\nInstallation\n------------\n\n.. code:: bash\n\n    $ pip install PyAthena\n\nExtra packages:\n\n+---------------+--------------------------------------+------------------+\n| Package       | Install command                      | Version          |\n+===============+======================================+==================+\n| SQLAlchemy    | ``pip install PyAthena[SQLAlchemy]`` | >=1.0.0, <2.0.0  |\n+---------------+--------------------------------------+------------------+\n| Pandas        | ``pip install PyAthena[Pandas]``     | >=1.3.0          |\n+---------------+--------------------------------------+------------------+\n| Arrow         | ``pip install PyAthena[Arrow]``      | >=7.0.0          |\n+---------------+--------------------------------------+------------------+\n\nUsage\n-----\n\nBasic usage\n~~~~~~~~~~~\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n    cursor.execute("SELECT * FROM one_row")\n    print(cursor.description)\n    print(cursor.fetchall())\n\nCursor iteration\n~~~~~~~~~~~~~~~~\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n    cursor.execute("SELECT * FROM many_rows LIMIT 10")\n    for row in cursor:\n        print(row)\n\nQuery with parameter\n~~~~~~~~~~~~~~~~~~~~\n\nSupported `DB API paramstyle`_ is only ``PyFormat``.\n``PyFormat`` only supports `named placeholders`_ with old ``%`` operator style and parameters specify dictionary format.\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n    cursor.execute("""\n                   SELECT col_string FROM one_row_complex\n                   WHERE col_string = %(param)s\n                   """, {"param": "a string"})\n    print(cursor.fetchall())\n\nif ``%`` character is contained in your query, it must be escaped with ``%%`` like the following:\n\n.. code:: sql\n\n    SELECT col_string FROM one_row_complex\n    WHERE col_string = %(param)s OR col_string LIKE \'a%%\'\n\n.. _`DB API paramstyle`: https://www.python.org/dev/peps/pep-0249/#paramstyle\n.. _`named placeholders`: https://pyformat.info/#named_placeholders\n\nSQLAlchemy\n~~~~~~~~~~\n\nInstall SQLAlchemy with ``pip install "SQLAlchemy>=1.0.0, <2.0.0"`` or ``pip install PyAthena[SQLAlchemy]``.\nSupported SQLAlchemy is 1.0.0 or higher and less than 2.0.0.\n\n.. code:: python\n\n    from urllib.parse import quote_plus\n    from sqlalchemy.engine import create_engine\n    from sqlalchemy.sql.expression import select\n    from sqlalchemy.sql.functions import func\n    from sqlalchemy.sql.schema import Table, MetaData\n\n    conn_str = "awsathena+rest://{aws_access_key_id}:{aws_secret_access_key}@athena.{region_name}.amazonaws.com:443/"\\\n               "{schema_name}?s3_staging_dir={s3_staging_dir}"\n    engine = create_engine(conn_str.format(\n        aws_access_key_id=quote_plus("YOUR_ACCESS_KEY_ID"),\n        aws_secret_access_key=quote_plus("YOUR_SECRET_ACCESS_KEY"),\n        region_name="us-west-2",\n        schema_name="default",\n        s3_staging_dir=quote_plus("s3://YOUR_S3_BUCKET/path/to/")))\n    with engine.connect() as connection:\n        many_rows = Table("many_rows", MetaData(), autoload_with=connection)\n        result = connection.execute(select([func.count("*")], from_obj=many_rows))\n        print(result.scalar())\n\nThe connection string has the following format:\n\n.. code:: text\n\n    awsathena+rest://{aws_access_key_id}:{aws_secret_access_key}@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&...\n\nIf you do not specify ``aws_access_key_id`` and ``aws_secret_access_key`` using instance profile or boto3 configuration file:\n\n.. code:: text\n\n    awsathena+rest://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&...\n\nNOTE: ``s3_staging_dir`` requires quote. If ``aws_access_key_id``, ``aws_secret_access_key`` and other parameter contain special characters, quote is also required.\n\nDialect & driver\n^^^^^^^^^^^^^^^^\n\n+-----------+--------+------------------+-----------------+\n| Dialect   | Driver | Schema           | Cursor          |\n+===========+========+==================+=================+\n| awsathena |        | awsathena        | DefaultCursor   |\n+-----------+--------+------------------+-----------------+\n| awsathena | rest   | awsathena+rest   | DefaultCursor   |\n+-----------+--------+------------------+-----------------+\n| awsathena | pandas | awsathena+pandas | `PandasCursor`_ |\n+-----------+--------+------------------+-----------------+\n| awsathena | arrow  | awsathena+arrow  | `ArrowCursor`_  |\n+-----------+--------+------------------+-----------------+\n| awsathena | jdbc   | awsathena+jdbc   | `PyAthenaJDBC`_ |\n+-----------+--------+------------------+-----------------+\n\n.. _`PyAthenaJDBC`: https://github.com/laughingman7743/PyAthenaJDBC\n\n\nDialect options\n^^^^^^^^^^^^^^^\n\nTable options\n#############\n\nlocation\n    Type:\n        str\n    Description:\n        Specifies the location of the underlying data in the Amazon S3 from which the table is created.\n    value:\n        s3://bucket/path/to/\n    Example:\n        .. code:: python\n\n            Table("some_table", metadata, ..., awsathena_location="s3://bucket/path/to/")\ncompression\n    Type:\n        str\n    Description:\n        Specifies the compression format.\n    Value:\n        * BZIP2\n        * DEFLATE\n        * GZIP\n        * LZ4\n        * LZO\n        * SNAPPY\n        * ZLIB\n        * ZSTD\n        * NONE|UNCOMPRESSED\n    Example:\n        .. code:: python\n\n            Table("some_table", metadata, ..., awsathena_compression="SNAPPY")\nrow_format\n    Type:\n        str\n    Description:\n        Specifies the row format of the table and its underlying source data if applicable.\n    Value:\n        * [DELIMITED FIELDS TERMINATED BY char [ESCAPED BY char]]\n        * [DELIMITED COLLECTION ITEMS TERMINATED BY char]\n        * [MAP KEYS TERMINATED BY char]\n        * [LINES TERMINATED BY char]\n        * [NULL DEFINED AS char]\n        * SERDE \'serde_name\'\n    Example:\n        .. code:: python\n\n            Table("some_table", metadata, ..., awsathena_row_format="SERDE \'org.openx.data.jsonserde.JsonSerDe\'")\nfile_format\n    Type:\n        str\n    Description:\n        Specifies the file format for table data.\n    Value:\n        * SEQUENCEFILE\n        * TEXTFILE\n        * RCFILE\n        * ORC\n        * PARQUET\n        * AVRO\n        * ION\n        * INPUTFORMAT input_format_classname OUTPUTFORMAT output_format_classname\n    Example:\n        .. code:: python\n\n            Table("some_table", metadata, ..., awsathena_file_format="PARQUET")\n            Table("some_table", metadata, ..., awsathena_file_format="INPUTFORMAT \'org.apache.hadoop.hive.ql.io.parquet.MapredParquetInputFormat\' OUTPUTFORMAT \'org.apache.hadoop.hive.ql.io.parquet.MapredParquetOutputFormat\'")\nserdeproperties\n    Type:\n        dict[str, str]\n    Description:\n        Specifies one or more custom properties allowed in SerDe.\n    Value:\n        .. code:: python\n\n            { "property_name": "property_value", "property_name": "property_value", ... }\n    Example:\n        .. code:: python\n\n            Table("some_table", metadata, ..., awsathena_serdeproperties={\n                "separatorChar": ",", "escapeChar": "\\\\\\\\"\n            })\ntblproperties\n    Type:\n        dict[str, str]\n    Description:\n        Specifies custom metadata key-value pairs for the table definition in addition to predefined table properties.\n    Value:\n        .. code:: python\n\n            { "property_name": "property_value", "property_name": "property_value", ... }\n    Example:\n        .. code:: python\n\n            Table("some_table", metadata, ..., awsathena_tblproperties={\n                "projection.enabled": "true",\n                "projection.dt.type": "date",\n                "projection.dt.range": "NOW-1YEARS,NOW",\n                "projection.dt.format": "yyyy-MM-dd",\n            })\nbucket_count\n    Type:\n        int\n    Description:\n        The number of buckets for bucketing your data.\n    Value:\n        Integer value greater than or equal to 0\n    Example:\n        .. code:: python\n\n            Table("some_table", metadata, ..., awsathena_bucket_count=5)\n\nAll table options can also be configured with the connection string as follows:\n\n.. code:: text\n\n    awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?s3_staging_dir=s3%3A%2F%2Fbucket%2Fpath%2Fto%2F&location=s3%3A%2F%2Fbucket%2Fpath%2Fto%2F&file_format=parquet&compression=snappy&...\n\n``serdeproperties`` and ``tblproperties`` must be converted to strings in the ``\'key\'=\'value\',\'key\'=\'value\'`` format and url encoded.\nIf single quotes are included, escape them with a backslash.\n\nFor example, if you configure a projection setting ``\'projection.enabled\'=\'true\',\'projection.dt.type\'=\'date\',\'projection.dt.range\'=\'NOW-1YEARS,NOW\',\'projection.dt.format\'= \'yyyy-MM-dd\'`` in tblproperties, it would look like this\n\n.. code:: text\n\n    awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?s3_staging_dir=s3%3A%2F%2Fbucket%2Fpath%2Fto%2F&tblproperties=%27projection.enabled%27%3D%27true%27%2C%27projection.dt.type%27%3D%27date%27%2C%27projection.dt.range%27%3D%27NOW-1YEARS%2CNOW%27%2C%27projection.dt.format%27%3D+%27yyyy-MM-dd%27\n\nColumn options\n##############\n\npartition\n    Type:\n        bool\n    Description:\n        Specifies a key for partitioning data.\n    Value:\n        True / False\n    Example:\n        .. code:: python\n\n            Column("some_column", types.String, ..., awsathena_partition=True)\ncluster\n    Type:\n        bool\n    Description:\n        Divides the data in the specified column into data subsets called buckets, with or without partitioning.\n    Value:\n        True / False\n    Example:\n        .. code:: python\n\n            Column("some_column", types.String, ..., awsathena_cluster=True)\n\nTo configure column options from the connection string, specify the column name as a comma-separated string.\n\n.. code:: text\n\n    awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?partition=column1%2Ccolumn2&cluster=column1%2Ccolumn2&...\n\nIf you want to limit the column options to specific table names only, specify the table and column names connected by dots as a comma-separated string.\n\n.. code:: text\n\n    awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?partition=table1.column1%2Ctable1.column2&cluster=table2.column1%2Ctable2.column2&...\n\nPandas\n~~~~~~\n\nAs DataFrame\n^^^^^^^^^^^^\n\nYou can use the `pandas.read_sql_query`_ to handle the query results as a `pandas.DataFrame object`_.\n\n.. code:: python\n\n    from pyathena import connect\n    import pandas as pd\n\n    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                   region_name="us-west-2")\n    df = pd.read_sql_query("SELECT * FROM many_rows", conn)\n    print(df.head())\n\nNOTE: `Poor performance when using pandas.read_sql #222 <https://github.com/laughingman7743/PyAthena/issues/222>`_\n\nThe ``pyathena.pandas.util`` package also has helper methods.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.util import as_pandas\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n    cursor.execute("SELECT * FROM many_rows")\n    df = as_pandas(cursor)\n    print(df.describe())\n\nIf you want to use the query results output to S3 directly, you can use `PandasCursor`_.\nThis cursor fetches query results faster than the default cursor. (See `benchmark results`_.)\n\n.. _`pandas.read_sql_query`: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_sql_query.html\n.. _`benchmark results`: benchmarks/\n\nTo SQL\n^^^^^^\n\nYou can use `pandas.DataFrame.to_sql`_ to write records stored in DataFrame to Amazon Athena.\n`pandas.DataFrame.to_sql`_ uses `SQLAlchemy`_, so you need to install it.\n\n.. code:: python\n\n    import pandas as pd\n    from urllib.parse import quote_plus\n    from sqlalchemy import create_engine\n\n    conn_str = "awsathena+rest://:@athena.{region_name}.amazonaws.com:443/"\\\n               "{schema_name}?s3_staging_dir={s3_staging_dir}&location={location}&compression=snappy"\n    engine = create_engine(conn_str.format(\n        region_name="us-west-2",\n        schema_name="YOUR_SCHEMA",\n        s3_staging_dir=quote_plus("s3://YOUR_S3_BUCKET/path/to/"),\n        location=quote_plus("s3://YOUR_S3_BUCKET/path/to/")))\n\n    df = pd.DataFrame({"a": [1, 2, 3, 4, 5]})\n    df.to_sql("YOUR_TABLE", engine, schema="YOUR_SCHEMA", index=False, if_exists="replace", method="multi")\n\nThe location of the Amazon S3 table is specified by the ``location`` parameter in the connection string.\nIf ``location`` is not specified, ``s3_staging_dir`` parameter will be used. The following rules apply.\n\n.. code:: text\n\n    s3://{location or s3_staging_dir}/{schema}/{table}/\n\nThe file format, row format, and compression settings are specified in the connection string, see `Table options`_.\n\nThe ``pyathena.pandas.util`` package also has helper methods.\n\n.. code:: python\n\n    import pandas as pd\n    from pyathena import connect\n    from pyathena.pandas.util import to_sql\n\n    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                   region_name="us-west-2")\n    df = pd.DataFrame({"a": [1, 2, 3, 4, 5]})\n    to_sql(df, "YOUR_TABLE", conn, "s3://YOUR_S3_BUCKET/path/to/",\n           schema="YOUR_SCHEMA", index=False, if_exists="replace")\n\nThis helper method supports partitioning.\n\n.. code:: python\n\n    import pandas as pd\n    from datetime import date\n    from pyathena import connect\n    from pyathena.pandas.util import to_sql\n\n    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                   region_name="us-west-2")\n    df = pd.DataFrame({\n        "a": [1, 2, 3, 4, 5],\n        "dt": [\n            date(2020, 1, 1), date(2020, 1, 1), date(2020, 1, 1),\n            date(2020, 1, 2),\n            date(2020, 1, 3)\n        ],\n    })\n    to_sql(df, "YOUR_TABLE", conn, "s3://YOUR_S3_BUCKET/path/to/",\n           schema="YOUR_SCHEMA", partitions=["dt"])\n\n    cursor = conn.cursor()\n    cursor.execute("SHOW PARTITIONS YOUR_TABLE")\n    print(cursor.fetchall())\n\nConversion to Parquet and upload to S3 use `ThreadPoolExecutor`_ by default.\nIt is also possible to use `ProcessPoolExecutor`_.\n\n.. code:: python\n\n    import pandas as pd\n    from concurrent.futures.process import ProcessPoolExecutor\n    from pyathena import connect\n    from pyathena.pandas.util import to_sql\n\n    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                   region_name="us-west-2")\n    df = pd.DataFrame({"a": [1, 2, 3, 4, 5]})\n    to_sql(df, "YOUR_TABLE", conn, "s3://YOUR_S3_BUCKET/path/to/",\n           schema="YOUR_SCHEMA", index=False, if_exists="replace",\n           chunksize=1, executor_class=ProcessPoolExecutor, max_workers=5)\n\n.. _`pandas.DataFrame.to_sql`: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_sql.html\n.. _`ThreadPoolExecutor`: https://docs.python.org/3/library/concurrent.futures.html#threadpoolexecutor\n.. _`ProcessPoolExecutor`: https://docs.python.org/3/library/concurrent.futures.html#processpoolexecutor\n\nDictCursor\n~~~~~~~~~~\n\nDictCursor retrieve the query execution result as a dictionary type with column names and values.\n\nYou can use the DictCursor by specifying the ``cursor_class``\nwith the connect method or connection object.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.cursor import DictCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=DictCursor).cursor()\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.cursor import DictCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2",\n                        cursor_class=DictCursor).cursor()\n\nIt can also be used by specifying the cursor class when calling the connection object\'s cursor method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.cursor import DictCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(DictCursor)\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.cursor import DictCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2").cursor(DictCursor)\n\nThe basic usage is the same as the Cursor.\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.cursor import DictCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2").cursor(DictCursor)\n    cursor.execute("SELECT * FROM many_rows LIMIT 10")\n    for row in cursor:\n        print(row["a"])\n\nIf you want to change the dictionary type (e.g., use OrderedDict), you can specify like the following.\n\n.. code:: python\n\n    from collections import OrderedDict\n    from pyathena import connect\n    from pyathena.cursor import DictCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=DictCursor).cursor(dict_type=OrderedDict)\n\n.. code:: python\n\n    from collections import OrderedDict\n    from pyathena import connect\n    from pyathena.cursor import DictCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(cursor=DictCursor, dict_type=OrderedDict)\n\nAsyncCursor\n~~~~~~~~~~~\n\nAsyncCursor is a simple implementation using the concurrent.futures package.\nThis cursor does not follow the `DB API 2.0 (PEP 249)`_.\n\nYou can use the AsyncCursor by specifying the ``cursor_class``\nwith the connect method or connection object.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncCursor).cursor()\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.async_cursor import AsyncCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2",\n                        cursor_class=AsyncCursor).cursor()\n\nIt can also be used by specifying the cursor class when calling the connection object\'s cursor method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(AsyncCursor)\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.async_cursor import AsyncCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2").cursor(AsyncCursor)\n\nThe default number of workers is 5 or cpu number * 5.\nIf you want to change the number of workers you can specify like the following.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncCursor).cursor(max_workers=10)\n\nThe execute method of the AsyncCursor returns the tuple of the query ID and the `future object`_.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n\nThe return value of the `future object`_ is an ``AthenaResultSet`` object.\nThis object has an interface that can fetch and iterate query results similar to synchronous cursors.\nIt also has information on the result of query execution.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncCursor).cursor()\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    result_set = future.result()\n    print(result_set.state)\n    print(result_set.state_change_reason)\n    print(result_set.completion_date_time)\n    print(result_set.submission_date_time)\n    print(result_set.data_scanned_in_bytes)\n    print(result_set.engine_execution_time_in_millis)\n    print(result_set.query_queue_time_in_millis)\n    print(result_set.total_execution_time_in_millis)\n    print(result_set.query_planning_time_in_millis)\n    print(result_set.service_processing_time_in_millis)\n    print(result_set.output_location)\n    print(result_set.description)\n    for row in result_set:\n        print(row)\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncCursor).cursor()\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    result_set = future.result()\n    print(result_set.fetchall())\n\nA query ID is required to cancel a query with the AsyncCursor.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncCursor).cursor()\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    cursor.cancel(query_id)\n\nNOTE: The cancel method of the `future object`_ does not cancel the query.\n\n.. _`future object`: https://docs.python.org/3/library/concurrent.futures.html#future-objects\n\nAsyncDictCursor\n~~~~~~~~~~~~~~~\n\nAsyncDIctCursor is an AsyncCursor that can retrieve the query execution result\nas a dictionary type with column names and values.\n\nYou can use the DictCursor by specifying the ``cursor_class``\nwith the connect method or connection object.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncDictCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncDictCursor).cursor()\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.async_cursor import AsyncDictCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2",\n                        cursor_class=AsyncDictCursor).cursor()\n\nIt can also be used by specifying the cursor class when calling the connection object\'s cursor method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncDictCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(AsyncDictCursor)\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.async_cursor import AsyncDictCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2").cursor(AsyncDictCursor)\n\nThe basic usage is the same as the AsyncCursor.\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.cursor import DictCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2").cursor(AsyncDictCursor)\n    query_id, future = cursor.execute("SELECT * FROM many_rows LIMIT 10")\n    result_set = future.result()\n    for row in result_set:\n        print(row["a"])\n\nIf you want to change the dictionary type (e.g., use OrderedDict), you can specify like the following.\n\n.. code:: python\n\n    from collections import OrderedDict\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncDictCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncDictCursor).cursor(dict_type=OrderedDict)\n\n.. code:: python\n\n    from collections import OrderedDict\n    from pyathena import connect\n    from pyathena.async_cursor import AsyncDictCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(cursor=AsyncDictCursor, dict_type=OrderedDict)\n\nPandasCursor\n~~~~~~~~~~~~\n\nPandasCursor directly handles the CSV file of the query execution result output to S3.\nThis cursor is to download the CSV file after executing the query, and then loaded into `pandas.DataFrame object`_.\nPerformance is better than fetching data with Cursor.\n\nYou can use the PandasCursor by specifying the ``cursor_class``\nwith the connect method or connection object.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=PandasCursor).cursor()\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2",\n                        cursor_class=PandasCursor).cursor()\n\nIt can also be used by specifying the cursor class when calling the connection object\'s cursor method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(PandasCursor)\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2").cursor(PandasCursor)\n\nThe as_pandas method returns a `pandas.DataFrame object`_.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=PandasCursor).cursor()\n\n    df = cursor.execute("SELECT * FROM many_rows").as_pandas()\n    print(df.describe())\n    print(df.head())\n\nSupport fetch and iterate query results.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=PandasCursor).cursor()\n\n    cursor.execute("SELECT * FROM many_rows")\n    print(cursor.fetchone())\n    print(cursor.fetchmany())\n    print(cursor.fetchall())\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=PandasCursor).cursor()\n\n    cursor.execute("SELECT * FROM many_rows")\n    for row in cursor:\n        print(row)\n\nThe DATE and TIMESTAMP of Athena\'s data type are returned as `pandas.Timestamp`_ type.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=PandasCursor).cursor()\n\n    cursor.execute("SELECT col_timestamp FROM one_row_complex")\n    print(type(cursor.fetchone()[0]))  # <class \'pandas._libs.tslibs.timestamps.Timestamp\'>\n\nExecution information of the query can also be retrieved.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=PandasCursor).cursor()\n\n    cursor.execute("SELECT * FROM many_rows")\n    print(cursor.state)\n    print(cursor.state_change_reason)\n    print(cursor.completion_date_time)\n    print(cursor.submission_date_time)\n    print(cursor.data_scanned_in_bytes)\n    print(cursor.engine_execution_time_in_millis)\n    print(cursor.query_queue_time_in_millis)\n    print(cursor.total_execution_time_in_millis)\n    print(cursor.query_planning_time_in_millis)\n    print(cursor.service_processing_time_in_millis)\n    print(cursor.output_location)\n\nIf you want to customize the pandas.Dataframe object dtypes and converters, create a converter class like this:\n\n.. code:: python\n\n    from pyathena.converter import Converter\n\n    class CustomPandasTypeConverter(Converter):\n\n        def __init__(self):\n            super(CustomPandasTypeConverter, self).__init__(\n                mappings=None,\n                types={\n                    "boolean": object,\n                    "tinyint": float,\n                    "smallint": float,\n                    "integer": float,\n                    "bigint": float,\n                    "float": float,\n                    "real": float,\n                    "double": float,\n                    "decimal": float,\n                    "char": str,\n                    "varchar": str,\n                    "array": str,\n                    "map": str,\n                    "row": str,\n                    "varbinary": str,\n                    "json": str,\n                }\n            )\n\n        def convert(self, type_, value):\n            # Not used in PandasCursor.\n            pass\n\nSpecify the combination of converter functions in the mappings argument and the dtypes combination in the types argument.\n\nThen you simply specify an instance of this class in the convertes argument when creating a connection or cursor.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(PandasCursor, converter=CustomPandasTypeConverter())\n\nIf the unload option is enabled, the Parquet file itself has a schema, so the conversion is done to the dtypes according to that schema,\nand the ``mappings`` and ``types`` settings of the Converter class are not used.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     converter=CustomPandasTypeConverter()).cursor(PandasCursor)\n\nIf you want to change the NaN behavior of pandas.Dataframe,\nyou can do so by using the ``keep_default_na``, ``na_values`` and ``quoting`` arguments of the cursor object\'s execute method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=PandasCursor).cursor()\n    df = cursor.execute("SELECT * FROM many_rows",\n                        keep_default_na=False,\n                        na_values=[""]).as_pandas()\n\nNOTE: PandasCursor handles the CSV file on memory. Pay attention to the memory capacity.\n\n.. _`pandas.DataFrame object`: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html\n.. _`pandas.Timestamp`: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Timestamp.html\n\n[PandasCursor] Unload options\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nPandasCursor also supports the UNLOAD option, as does `ArrowCursor`_.\n\nSee `[ArrowCursor] Unload options`_ for more information.\n\nThe UNLOAD option can be enabled by specifying it in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=PandasCursor,\n                     cursor_kwargs={\n                         "unload": True\n                     }).cursor()\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import PandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=PandasCursor).cursor(unload=True)\n\nSQLAlchemy allows this option to be specified in the connection string.\n\n.. code:: text\n\n    awsathena+pandas://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&unload=true...\n\nAsyncPandasCursor\n~~~~~~~~~~~~~~~~~\n\nAsyncPandasCursor is an AsyncCursor that can handle `pandas.DataFrame object`_.\nThis cursor directly handles the CSV of query results output to S3 in the same way as PandasCursor.\n\nYou can use the AsyncPandasCursor by specifying the ``cursor_class``\nwith the connect method or connection object.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor).cursor()\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2",\n                        cursor_class=AsyncPandasCursor).cursor()\n\nIt can also be used by specifying the cursor class when calling the connection object\'s cursor method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(AsyncPandasCursor)\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2").cursor(AsyncPandasCursor)\n\nThe default number of workers is 5 or cpu number * 5.\nIf you want to change the number of workers you can specify like the following.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor).cursor(max_workers=10)\n\nThe execute method of the AsyncPandasCursor returns the tuple of the query ID and the `future object`_.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n\nThe return value of the `future object`_ is an ``AthenaPandasResultSet`` object.\nThis object has an interface similar to ``AthenaResultSetObject``.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    result_set = future.result()\n    print(result_set.state)\n    print(result_set.state_change_reason)\n    print(result_set.completion_date_time)\n    print(result_set.submission_date_time)\n    print(result_set.data_scanned_in_bytes)\n    print(result_set.engine_execution_time_in_millis)\n    print(result_set.query_queue_time_in_millis)\n    print(result_set.total_execution_time_in_millis)\n    print(result_set.query_planning_time_in_millis)\n    print(result_set.service_processing_time_in_millis)\n    print(result_set.output_location)\n    print(result_set.description)\n    for row in result_set:\n        print(row)\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    result_set = future.result()\n    print(result_set.fetchall())\n\nThis object also has an as_pandas method that returns a `pandas.DataFrame object`_ similar to the PandasCursor.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    result_set = future.result()\n    df = result_set.as_pandas()\n    print(df.describe())\n    print(df.head())\n\nThe DATE and TIMESTAMP of Athena\'s data type are returned as `pandas.Timestamp`_ type.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT col_timestamp FROM one_row_complex")\n    result_set = future.result()\n    print(type(result_set.fetchone()[0]))  # <class \'pandas._libs.tslibs.timestamps.Timestamp\'>\n\nAs with AsyncCursor, you need a query ID to cancel a query.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.async_cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    cursor.cancel(query_id)\n\nAs with PandasCursor, the UNLOAD option is also available.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor,\n                     cursor_kwargs={\n                         "unload": True\n                     }).cursor()\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.pandas.cursor import AsyncPandasCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncPandasCursor).cursor(unload=True)\n\nArrowCursor\n~~~~~~~~~~~\n\nArrowCursor directly handles the CSV file of the query execution result output to S3.\nThis cursor is to download the CSV file after executing the query, and then loaded into `pyarrow.Table object`_.\nPerformance is better than fetching data with Cursor.\n\nYou can use the ArrowCursor by specifying the ``cursor_class``\nwith the connect method or connection object.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=ArrowCursor).cursor()\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2",\n                        cursor_class=ArrowCursor).cursor()\n\nIt can also be used by specifying the cursor class when calling the connection object\'s cursor method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(ArrowCursor)\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2").cursor(ArrowCursor)\n\nThe as_arrow method returns a `pyarrow.Table object`_.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=ArrowCursor).cursor()\n\n    table = cursor.execute("SELECT * FROM many_rows").as_arrow()\n    print(table)\n    print(table.column_names)\n    print(table.columns)\n    print(table.nbytes)\n    print(table.num_columns)\n    print(table.num_rows)\n    print(table.schema)\n    print(table.shape)\n\nSupport fetch and iterate query results.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=ArrowCursor).cursor()\n\n    cursor.execute("SELECT * FROM many_rows")\n    print(cursor.fetchone())\n    print(cursor.fetchmany())\n    print(cursor.fetchall())\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=ArrowCursor).cursor()\n\n    cursor.execute("SELECT * FROM many_rows")\n    for row in cursor:\n        print(row)\n\nExecution information of the query can also be retrieved.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=ArrowCursor).cursor()\n\n    cursor.execute("SELECT * FROM many_rows")\n    print(cursor.state)\n    print(cursor.state_change_reason)\n    print(cursor.completion_date_time)\n    print(cursor.submission_date_time)\n    print(cursor.data_scanned_in_bytes)\n    print(cursor.engine_execution_time_in_millis)\n    print(cursor.query_queue_time_in_millis)\n    print(cursor.total_execution_time_in_millis)\n    print(cursor.query_planning_time_in_millis)\n    print(cursor.service_processing_time_in_millis)\n    print(cursor.output_location)\n\nIf you want to customize the `pyarrow.Table object`_ types, create a converter class like this:\n\n.. code:: python\n\n    import pyarrow as pa\n    from pyathena.arrow.converter import _to_date\n    from pyathena.converter import Converter\n\n    class CustomArrowTypeConverter(Converter):\n        def __init__(self) -> None:\n            super(CustomArrowTypeConverter, self).__init__(\n                mappings={\n                    "date": _to_date,\n                },\n                types={\n                    "boolean": pa.bool_(),\n                    "tinyint": pa.int8(),\n                    "smallint": pa.int16(),\n                    "integer": pa.int32(),\n                    "bigint": pa.int64(),\n                    "float": pa.float32(),\n                    "real": pa.float64(),\n                    "double": pa.float64(),\n                    "char": pa.string(),\n                    "varchar": pa.string(),\n                    "string": pa.string(),\n                    "timestamp": pa.timestamp("ms"),\n                    "date": pa.timestamp("ms"),\n                    "time": pa.string(),\n                    "varbinary": pa.string(),\n                    "array": pa.string(),\n                    "map": pa.string(),\n                    "row": pa.string(),\n                    "decimal": pa.string(),\n                    "json": pa.string(),\n                },\n            )\n\n    def convert(self, type_, value):\n        converter = self.get(type_)\n        return converter(value)\n\n``types`` is used to explicitly specify the Arrow type when reading CSV files.\n``mappings`` is used as a conversion method when fetching data from a cursor object.\n\nThen you simply specify an instance of this class in the convertes argument when creating a connection or cursor.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(ArrowCursor, converter=CustomArrowTypeConverter())\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     converter=CustomArrowTypeConverter()).cursor(ArrowCursor)\n\nIf the unload option is enabled, the Parquet file itself has a schema, so the conversion is done to the Arrow type according to that schema,\nand the ``types`` setting of the Converter class is not used.\n\n[ArrowCursor] Unload options\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nArrowCurosr supports the UNLOAD option. When this option is enabled,\nqueries with SELECT statements are automatically converted to UNLOAD statements and executed to Athena,\nand the results are output in Parquet format (Snappy compressed) to ``s3_staging_dir``.\nThe cursor reads the output Parquet file directly.\n\nThe output of query results with the UNLOAD statement is faster than normal query execution.\nIn addition, the output Parquet file is split and can be read faster than a CSV file.\nWe recommend trying this option if you are concerned about the time it takes to execute the query and retrieve the results.\n\nHowever, UNLOAD has some limitations. Please refer to the `official UNLOAD documentation`_ for more information on limitations.\nAs per the limitations of the official documentation, the results of UNLOAD will be written to multiple files in parallel,\nand the contents of each file will be in sort order, but the relative order of the files to each other will not be sorted.\nNote that specifying ORDER BY with this option enabled does not guarantee the sort order of the data.\n\nThe UNLOAD option can be enabled by specifying it in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=ArrowCursor,\n                     cursor_kwargs={\n                         "unload": True\n                     }).cursor()\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import ArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=ArrowCursor).cursor(unload=True)\n\nSQLAlchemy allows this option to be specified in the connection string.\n\n.. code:: text\n\n    awsathena+arrow://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&unload=true...\n\nIf a ``NOT_SUPPORTED`` occurs, a type not supported by UNLOAD is included in the result of the SELECT.\nTry converting to another type, such as ``SELECT CAST(1 AS VARCHAR) AS name``.\n\n.. code:: text\n\n    pyathena.error.OperationalError: NOT_SUPPORTED: Unsupported Hive type: time\n\nIn most cases of ``SYNTAX_ERROR``, you forgot to alias the column in the SELECT result.\nTry adding an alias to the SELECTed column, such as ``SELECT 1 AS name``.\n\n.. code:: text\n\n    pyathena.error.OperationalError: SYNTAX_ERROR: line 1:1: Column name not specified at position 1\n\n.. _`pyarrow.Table object`: https://arrow.apache.org/docs/python/generated/pyarrow.Table.html\n.. _`official UNLOAD documentation`: https://docs.aws.amazon.com/athena/latest/ug/unload.html\n\nAsyncArrowCursor\n~~~~~~~~~~~~~~~~\n\nAsyncArrowCursor is an AsyncCursor that can handle `pyarrow.Table object`_.\nThis cursor directly handles the CSV of query results output to S3 in the same way as ArrowCursor.\n\nYou can use the AsyncArrowCursor by specifying the ``cursor_class``\nwith the connect method or connection object.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncArrowCursor).cursor()\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2",\n                        cursor_class=AsyncArrowCursor).cursor()\n\nIt can also be used by specifying the cursor class when calling the connection object\'s cursor method.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor(AsyncArrowCursor)\n\n.. code:: python\n\n    from pyathena.connection import Connection\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                        region_name="us-west-2").cursor(AsyncArrowCursor)\n\nThe default number of workers is 5 or cpu number * 5.\nIf you want to change the number of workers you can specify like the following.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncArrowCursor).cursor(max_workers=10)\n\nThe execute method of the AsyncArrowCursor returns the tuple of the query ID and the `future object`_.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncArrowCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n\nThe return value of the `future object`_ is an ``AthenaArrowResultSet`` object.\nThis object has an interface similar to ``AthenaResultSetObject``.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncArrowCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    result_set = future.result()\n    print(result_set.state)\n    print(result_set.state_change_reason)\n    print(result_set.completion_date_time)\n    print(result_set.submission_date_time)\n    print(result_set.data_scanned_in_bytes)\n    print(result_set.engine_execution_time_in_millis)\n    print(result_set.query_queue_time_in_millis)\n    print(result_set.total_execution_time_in_millis)\n    print(result_set.query_planning_time_in_millis)\n    print(result_set.service_processing_time_in_millis)\n    print(result_set.output_location)\n    print(result_set.description)\n    for row in result_set:\n        print(row)\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncArrowCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    result_set = future.result()\n    print(result_set.fetchall())\n\nThis object also has an as_arrow method that returns a `pyarrow.Table object`_ similar to the ArrowCursor.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncArrowCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    result_set = future.result()\n    table = result_set.as_arrow()\n    print(table)\n    print(table.column_names)\n    print(table.columns)\n    print(table.nbytes)\n    print(table.num_columns)\n    print(table.num_rows)\n    print(table.schema)\n    print(table.shape)\n\nAs with AsyncCursor, you need a query ID to cancel a query.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.async_cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncArrowCursor).cursor()\n\n    query_id, future = cursor.execute("SELECT * FROM many_rows")\n    cursor.cancel(query_id)\n\nAs with ArrowCursor, the UNLOAD option is also available.\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncArrowCursor,\n                     cursor_kwargs={\n                         "unload": True\n                     }).cursor()\n\n.. code:: python\n\n    from pyathena import connect\n    from pyathena.arrow.cursor import AsyncArrowCursor\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2",\n                     cursor_class=AsyncArrowCursor).cursor(unload=True)\n\nQuickly re-run queries\n~~~~~~~~~~~~~~~~~~~~~~\n\nYou can attempt to re-use the results from a previously executed query to help save time and money in the cases where your underlying data isn\'t changing.\nSet the ``cache_size`` or ``cache_expiration_time`` parameter of ``cursor.execute()`` to a number larger than 0 to enable caching.\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n    cursor.execute("SELECT * FROM one_row")  # run once\n    print(cursor.query_id)\n    cursor.execute("SELECT * FROM one_row", cache_size=10)  # re-use earlier results\n    print(cursor.query_id)  # You should expect to see the same Query ID\n\nThe unit of ``expiration_time`` is seconds. To use the results of queries executed up to one hour ago, specify like the following.\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n    cursor.execute("SELECT * FROM one_row", cache_expiration_time=3600)  # Use queries executed within 1 hour as cache.\n\nIf ``cache_size`` is not specified, the value of ``sys.maxsize`` will be automatically set and all query results executed up to one hour ago will be checked.\nTherefore, it is recommended to specify ``cache_expiration_time`` together with ``cache_size`` like the following.\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n    cursor.execute("SELECT * FROM one_row", cache_size=100, cache_expiration_time=3600)  # Use the last 100 queries within 1 hour as cache.\n\nResults will only be re-used if the query strings match *exactly*,\nand the query was a DML statement (the assumption being that you always want to re-run queries like ``CREATE TABLE`` and ``DROP TABLE``).\n\nThe S3 staging directory is not checked, so it\'s possible that the location of the results is not in your provided ``s3_staging_dir``.\n\nCredentials\n-----------\n\nSupport `Boto3 credentials`_.\n\n.. _`Boto3 credentials`: http://boto3.readthedocs.io/en/latest/guide/configuration.html\n\nAdditional environment variable:\n\n.. code:: bash\n\n    $ export AWS_ATHENA_S3_STAGING_DIR=s3://YOUR_S3_BUCKET/path/to/\n    $ export AWS_ATHENA_WORK_GROUP=YOUR_WORK_GROUP\n\nExamples\n~~~~~~~~\n\nPassing credentials as parameters\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(aws_access_key_id="YOUR_ACCESS_KEY_ID",\n                     aws_secret_access_key="YOUR_SECRET_ACCESS_KEY",\n                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(aws_access_key_id="YOUR_ACCESS_KEY_ID",\n                     aws_secret_access_key="YOUR_SECRET_ACCESS_KEY",\n                     aws_session_token="YOUR_SESSION_TOKEN",\n                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n\nMulti-factor authentication\n^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nYou will be prompted to enter the MFA code.\nThe program execution will be blocked until the MFA code is entered.\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(duration_seconds=3600,\n                     serial_number="arn:aws:iam::ACCOUNT_NUMBER_WITHOUT_HYPHENS:mfa/MFA_DEVICE_ID",\n                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n\nShared credentials file\n^^^^^^^^^^^^^^^^^^^^^^^\n\nThe shared credentials file has a default location of ~/.aws/credentials.\n\nIf you use the default profile, there is no need to specify credential information.\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n\nYou can also specify a profile other than the default.\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(profile_name="YOUR_PROFILE_NAME",\n                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n\nAssume role provider\n^^^^^^^^^^^^^^^^^^^^\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(role_arn="YOUR_ASSUME_ROLE_ARN",\n                     role_session_name="PyAthena-session",\n                     duration_seconds=3600,\n                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n\nAssume role provider with MFA\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nYou will be prompted to enter the MFA code.\nThe program execution will be blocked until the MFA code is entered.\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(role_arn="YOUR_ASSUME_ROLE_ARN",\n                     role_session_name="PyAthena-session",\n                     duration_seconds=3600,\n                     serial_number="arn:aws:iam::ACCOUNT_NUMBER_WITHOUT_HYPHENS:mfa/MFA_DEVICE_ID",\n                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n\nInstance profiles\n^^^^^^^^^^^^^^^^^\n\nNo need to specify credential information.\n\n.. code:: python\n\n    from pyathena import connect\n\n    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",\n                     region_name="us-west-2").cursor()\n\nTesting\n-------\n\nDepends on the following environment variables:\n\n.. code:: bash\n\n    $ export AWS_DEFAULT_REGION=us-west-2\n    $ export AWS_ATHENA_S3_STAGING_DIR=s3://YOUR_S3_BUCKET/path/to/\n    $ export AWS_ATHENA_WORKGROUP=pyathena-test\n\nIn addition, you need to create a workgroup with the `Query result location` set to the name specified in the `AWS_ATHENA_WORKGROUP` environment variable.\nIf primary is not available as the default workgroup, specify an alternative workgroup name for the default in the environment variable `AWS_ATHENA_DEFAULT_WORKGROUP`.\n\n.. code:: bash\n\n    $ export AWS_ATHENA_DEFAULT_WORKGROUP=DEFAULT_WORKGROUP\n\nRun test\n~~~~~~~~\n\n.. code:: bash\n\n    $ pip install poetry\n    $ poetry install -v\n    $ poetry run pytest\n\nRun test multiple Python versions\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n.. code:: bash\n\n    $ pip install poetry\n    $ poetry install -v\n    $ pyenv local 3.10.1 3.9.1 3.8.2 3.7.2\n    $ poetry run tox\n\nGitHub Actions\n~~~~~~~~~~~~~~\n\nGitHub Actions uses OpenID Connect (OIDC) to access AWS resources. You will need to refer to the `GitHub Actions documentation`_ to configure it.\n\n.. _`GitHub Actions documentation`: https://docs.github.com/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services\n\nThe CloudFormation templates for creating GitHub OIDC Provider and IAM Role can be found in the `aws-actions/configure-aws-credentials repository`_.\n\n.. _`aws-actions/configure-aws-credentials repository`: https://github.com/aws-actions/configure-aws-credentials#sample-iam-role-cloudformation-template\n\nUnder `scripts/cloudformation`_ you will also find a CloudFormation template with additional permissions and workgroup settings needed for testing.\n\n.. _`scripts/cloudformation`: scripts/cloudformation/\n\nThe example of the CloudFormation execution command is the following:\n\n.. code:: bash\n\n    $ aws --region us-west-2 \\\n        cloudformation create-stack \\\n        --stack-name github-actions-oidc-pyathena \\\n        --capabilities CAPABILITY_NAMED_IAM \\\n        --template-body file://./scripts/cloudformation/github_actions_oidc.yaml \\\n        --parameters ParameterKey=GitHubOrg,ParameterValue=laughingman7743 \\\n          ParameterKey=RepositoryName,ParameterValue=PyAthena \\\n          ParameterKey=BucketName,ParameterValue=laughingman7743-athena \\\n          ParameterKey=RoleName,ParameterValue=github-actions-oidc-pyathena-test \\\n          ParameterKey=WorkGroupName,ParameterValue=pyathena-test\n\nCode formatting\n---------------\n\nThe code formatting uses `black`_ and `isort`_.\n\nAppy format\n~~~~~~~~~~~\n\n.. code:: bash\n\n    $ make fmt\n\nCheck format\n~~~~~~~~~~~~\n\n.. code:: bash\n\n    $ make chk\n\n.. _`black`: https://github.com/psf/black\n.. _`isort`: https://github.com/timothycrosley/isort\n\nLicense\n-------\n\n`MIT license`_\n\nMany of the implementations in this library are based on `PyHive`_, thanks for `PyHive`_.\n\n.. _`MIT license`: LICENSE\n.. _`PyHive`: https://github.com/dropbox/PyHive\n',
-    'author': 'laughingman7743',
-    'author_email': 'laughingman7743@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/laughingman7743/PyAthena/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
+.. image:: https://github.com/laughingman7743/PyAthena/actions/workflows/test.yaml/badge.svg
+    :target: https://github.com/laughingman7743/PyAthena/actions/workflows/test.yaml
 
+.. image:: https://img.shields.io/pypi/l/PyAthena.svg
+    :target: https://github.com/laughingman7743/PyAthena/blob/master/LICENSE
+
+.. image:: https://pepy.tech/badge/pyathena/month
+    :target: https://pepy.tech/project/pyathena
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
+
+PyAthena
+========
+
+PyAthena is a Python `DB API 2.0 (PEP 249)`_ client for `Amazon Athena`_.
+
+.. _`DB API 2.0 (PEP 249)`: https://www.python.org/dev/peps/pep-0249/
+.. _`Amazon Athena`: https://docs.aws.amazon.com/athena/latest/APIReference/Welcome.html
+
+.. contents:: Table of Contents:
+   :local:
+   :depth: 2
+
+Requirements
+------------
+
+* Python
+
+  - CPython 3.8 3.9 3.10, 3.11
+
+Installation
+------------
+
+.. code:: bash
+
+    $ pip install PyAthena
+
+Extra packages:
+
++---------------+---------------------------------------+------------------+
+| Package       | Install command                       | Version          |
++===============+=======================================+==================+
+| SQLAlchemy    | ``pip install PyAthena[SQLAlchemy]``  | >=1.0.0          |
++---------------+---------------------------------------+------------------+
+| Pandas        | ``pip install PyAthena[Pandas]``      | >=1.3.0          |
++---------------+---------------------------------------+------------------+
+| Arrow         | ``pip install PyAthena[Arrow]``       | >=7.0.0          |
++---------------+---------------------------------------+------------------+
+| fastparquet   | ``pip install PyAthena[fastparquet]`` | >=0.4.0          |
++---------------+---------------------------------------+------------------+
+
+Usage
+-----
+
+Basic usage
+~~~~~~~~~~~
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+    cursor.execute("SELECT * FROM one_row")
+    print(cursor.description)
+    print(cursor.fetchall())
+
+Cursor iteration
+~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+    cursor.execute("SELECT * FROM many_rows LIMIT 10")
+    for row in cursor:
+        print(row)
+
+Query with parameter
+~~~~~~~~~~~~~~~~~~~~
+
+Supported `DB API paramstyle`_ is only ``PyFormat``.
+``PyFormat`` only supports `named placeholders`_ with old ``%`` operator style and parameters specify dictionary format.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+    cursor.execute("""
+                   SELECT col_string FROM one_row_complex
+                   WHERE col_string = %(param)s
+                   """, {"param": "a string"})
+    print(cursor.fetchall())
+
+if ``%`` character is contained in your query, it must be escaped with ``%%`` like the following:
+
+.. code:: sql
+
+    SELECT col_string FROM one_row_complex
+    WHERE col_string = %(param)s OR col_string LIKE 'a%%'
+
+.. _`DB API paramstyle`: https://www.python.org/dev/peps/pep-0249/#paramstyle
+.. _`named placeholders`: https://pyformat.info/#named_placeholders
+
+SQLAlchemy
+~~~~~~~~~~
+
+Install SQLAlchemy with ``pip install "SQLAlchemy>=1.0.0"`` or ``pip install PyAthena[SQLAlchemy]``.
+Supported SQLAlchemy is 1.0.0 or higher.
+
+.. code:: python
+
+    from sqlalchemy import func, select
+    from sqlalchemy.engine import create_engine
+    from sqlalchemy.sql.schema import Table, MetaData
+
+    conn_str = "awsathena+rest://{aws_access_key_id}:{aws_secret_access_key}@athena.{region_name}.amazonaws.com:443/"\
+               "{schema_name}?s3_staging_dir={s3_staging_dir}"
+    engine = create_engine(conn_str.format(
+        aws_access_key_id="YOUR_ACCESS_KEY_ID",
+        aws_secret_access_key="YOUR_SECRET_ACCESS_KEY",
+        region_name="us-west-2",
+        schema_name="default",
+        s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/"))
+    with engine.connect() as connection:
+        many_rows = Table("many_rows", MetaData(), autoload_with=connection)
+        result = connection.execute(select(func.count()).select_from(many_rows))
+        print(result.scalar())
+
+The connection string has the following format:
+
+.. code:: text
+
+    awsathena+rest://{aws_access_key_id}:{aws_secret_access_key}@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&...
+
+If you do not specify ``aws_access_key_id`` and ``aws_secret_access_key`` using instance profile or boto3 configuration file:
+
+.. code:: text
+
+    awsathena+rest://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&...
+
+Dialect & driver
+^^^^^^^^^^^^^^^^
+
++-----------+--------+------------------+-----------------+
+| Dialect   | Driver | Schema           | Cursor          |
++===========+========+==================+=================+
+| awsathena |        | awsathena        | DefaultCursor   |
++-----------+--------+------------------+-----------------+
+| awsathena | rest   | awsathena+rest   | DefaultCursor   |
++-----------+--------+------------------+-----------------+
+| awsathena | pandas | awsathena+pandas | `PandasCursor`_ |
++-----------+--------+------------------+-----------------+
+| awsathena | arrow  | awsathena+arrow  | `ArrowCursor`_  |
++-----------+--------+------------------+-----------------+
+| awsathena | jdbc   | awsathena+jdbc   | `PyAthenaJDBC`_ |
++-----------+--------+------------------+-----------------+
+
+.. _`PyAthenaJDBC`: https://github.com/laughingman7743/PyAthenaJDBC
+
+
+Dialect options
+^^^^^^^^^^^^^^^
+
+Table options
+#############
+
+location
+    Type:
+        str
+    Description:
+        Specifies the location of the underlying data in the Amazon S3 from which the table is created.
+    value:
+        s3://bucket/path/to/
+    Example:
+        .. code:: python
+
+            Table("some_table", metadata, ..., awsathena_location="s3://bucket/path/to/")
+compression
+    Type:
+        str
+    Description:
+        Specifies the compression format.
+    Value:
+        * BZIP2
+        * DEFLATE
+        * GZIP
+        * LZ4
+        * LZO
+        * SNAPPY
+        * ZLIB
+        * ZSTD
+        * NONE|UNCOMPRESSED
+    Example:
+        .. code:: python
+
+            Table("some_table", metadata, ..., awsathena_compression="SNAPPY")
+row_format
+    Type:
+        str
+    Description:
+        Specifies the row format of the table and its underlying source data if applicable.
+    Value:
+        * [DELIMITED FIELDS TERMINATED BY char [ESCAPED BY char]]
+        * [DELIMITED COLLECTION ITEMS TERMINATED BY char]
+        * [MAP KEYS TERMINATED BY char]
+        * [LINES TERMINATED BY char]
+        * [NULL DEFINED AS char]
+        * SERDE 'serde_name'
+    Example:
+        .. code:: python
+
+            Table("some_table", metadata, ..., awsathena_row_format="SERDE 'org.openx.data.jsonserde.JsonSerDe'")
+file_format
+    Type:
+        str
+    Description:
+        Specifies the file format for table data.
+    Value:
+        * SEQUENCEFILE
+        * TEXTFILE
+        * RCFILE
+        * ORC
+        * PARQUET
+        * AVRO
+        * ION
+        * INPUTFORMAT input_format_classname OUTPUTFORMAT output_format_classname
+    Example:
+        .. code:: python
+
+            Table("some_table", metadata, ..., awsathena_file_format="PARQUET")
+            Table("some_table", metadata, ..., awsathena_file_format="INPUTFORMAT 'org.apache.hadoop.hive.ql.io.parquet.MapredParquetInputFormat' OUTPUTFORMAT 'org.apache.hadoop.hive.ql.io.parquet.MapredParquetOutputFormat'")
+serdeproperties
+    Type:
+        dict[str, str]
+    Description:
+        Specifies one or more custom properties allowed in SerDe.
+    Value:
+        .. code:: python
+
+            { "property_name": "property_value", "property_name": "property_value", ... }
+    Example:
+        .. code:: python
+
+            Table("some_table", metadata, ..., awsathena_serdeproperties={
+                "separatorChar": ",", "escapeChar": "\\\\"
+            })
+tblproperties
+    Type:
+        dict[str, str]
+    Description:
+        Specifies custom metadata key-value pairs for the table definition in addition to predefined table properties.
+    Value:
+        .. code:: python
+
+            { "property_name": "property_value", "property_name": "property_value", ... }
+    Example:
+        .. code:: python
+
+            Table("some_table", metadata, ..., awsathena_tblproperties={
+                "projection.enabled": "true",
+                "projection.dt.type": "date",
+                "projection.dt.range": "NOW-1YEARS,NOW",
+                "projection.dt.format": "yyyy-MM-dd",
+            })
+bucket_count
+    Type:
+        int
+    Description:
+        The number of buckets for bucketing your data.
+    Value:
+        Integer value greater than or equal to 0
+    Example:
+        .. code:: python
+
+            Table("some_table", metadata, ..., awsathena_bucket_count=5)
+
+All table options can also be configured with the connection string as follows:
+
+.. code:: text
+
+    awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?s3_staging_dir=s3%3A%2F%2Fbucket%2Fpath%2Fto%2F&location=s3%3A%2F%2Fbucket%2Fpath%2Fto%2F&file_format=parquet&compression=snappy&...
+
+``serdeproperties`` and ``tblproperties`` must be converted to strings in the ``'key'='value','key'='value'`` format and url encoded.
+If single quotes are included, escape them with a backslash.
+
+For example, if you configure a projection setting ``'projection.enabled'='true','projection.dt.type'='date','projection.dt.range'='NOW-1YEARS,NOW','projection.dt.format'= 'yyyy-MM-dd'`` in tblproperties, it would look like this
+
+.. code:: text
+
+    awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?s3_staging_dir=s3%3A%2F%2Fbucket%2Fpath%2Fto%2F&tblproperties=%27projection.enabled%27%3D%27true%27%2C%27projection.dt.type%27%3D%27date%27%2C%27projection.dt.range%27%3D%27NOW-1YEARS%2CNOW%27%2C%27projection.dt.format%27%3D+%27yyyy-MM-dd%27
+
+Column options
+##############
+
+partition
+    Type:
+        bool
+    Description:
+        Specifies a key for partitioning data.
+    Value:
+        True / False
+    Example:
+        .. code:: python
+
+            Column("some_column", types.String, ..., awsathena_partition=True)
+cluster
+    Type:
+        bool
+    Description:
+        Divides the data in the specified column into data subsets called buckets, with or without partitioning.
+    Value:
+        True / False
+    Example:
+        .. code:: python
+
+            Column("some_column", types.String, ..., awsathena_cluster=True)
+
+To configure column options from the connection string, specify the column name as a comma-separated string.
+
+.. code:: text
+
+    awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?partition=column1%2Ccolumn2&cluster=column1%2Ccolumn2&...
+
+If you want to limit the column options to specific table names only, specify the table and column names connected by dots as a comma-separated string.
+
+.. code:: text
+
+    awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?partition=table1.column1%2Ctable1.column2&cluster=table2.column1%2Ctable2.column2&...
+
+Pandas
+~~~~~~
+
+As DataFrame
+^^^^^^^^^^^^
+
+You can use the `pandas.read_sql_query`_ to handle the query results as a `pandas.DataFrame object`_.
+
+.. code:: python
+
+    from pyathena import connect
+    import pandas as pd
+
+    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                   region_name="us-west-2")
+    df = pd.read_sql_query("SELECT * FROM many_rows", conn)
+    print(df.head())
+
+NOTE: `Poor performance when using pandas.read_sql #222 <https://github.com/laughingman7743/PyAthena/issues/222>`_
+
+The ``pyathena.pandas.util`` package also has helper methods.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.util import as_pandas
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+    cursor.execute("SELECT * FROM many_rows")
+    df = as_pandas(cursor)
+    print(df.describe())
+
+If you want to use the query results output to S3 directly, you can use `PandasCursor`_.
+This cursor fetches query results faster than the default cursor. (See `benchmark results`_.)
+
+.. _`pandas.read_sql_query`: https://pandas.pydata.org/docs/reference/api/pandas.read_sql_query.html
+.. _`benchmark results`: benchmarks/
+
+To SQL
+^^^^^^
+
+You can use `pandas.DataFrame.to_sql`_ to write records stored in DataFrame to Amazon Athena.
+`pandas.DataFrame.to_sql`_ uses `SQLAlchemy`_, so you need to install it.
+
+.. code:: python
+
+    import pandas as pd
+    from sqlalchemy import create_engine
+
+    conn_str = "awsathena+rest://:@athena.{region_name}.amazonaws.com:443/"\
+               "{schema_name}?s3_staging_dir={s3_staging_dir}&location={location}&compression=snappy"
+    engine = create_engine(conn_str.format(
+        region_name="us-west-2",
+        schema_name="YOUR_SCHEMA",
+        s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+        location="s3://YOUR_S3_BUCKET/path/to/"))
+
+    df = pd.DataFrame({"a": [1, 2, 3, 4, 5]})
+    df.to_sql("YOUR_TABLE", engine, schema="YOUR_SCHEMA", index=False, if_exists="replace", method="multi")
+
+The location of the Amazon S3 table is specified by the ``location`` parameter in the connection string.
+If ``location`` is not specified, ``s3_staging_dir`` parameter will be used. The following rules apply.
+
+.. code:: text
+
+    s3://{location or s3_staging_dir}/{schema}/{table}/
+
+The file format, row format, and compression settings are specified in the connection string, see `Table options`_.
+
+The ``pyathena.pandas.util`` package also has helper methods.
+
+.. code:: python
+
+    import pandas as pd
+    from pyathena import connect
+    from pyathena.pandas.util import to_sql
+
+    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                   region_name="us-west-2")
+    df = pd.DataFrame({"a": [1, 2, 3, 4, 5]})
+    to_sql(df, "YOUR_TABLE", conn, "s3://YOUR_S3_BUCKET/path/to/",
+           schema="YOUR_SCHEMA", index=False, if_exists="replace")
+
+This helper method supports partitioning.
+
+.. code:: python
+
+    import pandas as pd
+    from datetime import date
+    from pyathena import connect
+    from pyathena.pandas.util import to_sql
+
+    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                   region_name="us-west-2")
+    df = pd.DataFrame({
+        "a": [1, 2, 3, 4, 5],
+        "dt": [
+            date(2020, 1, 1), date(2020, 1, 1), date(2020, 1, 1),
+            date(2020, 1, 2),
+            date(2020, 1, 3)
+        ],
+    })
+    to_sql(df, "YOUR_TABLE", conn, "s3://YOUR_S3_BUCKET/path/to/",
+           schema="YOUR_SCHEMA", partitions=["dt"])
+
+    cursor = conn.cursor()
+    cursor.execute("SHOW PARTITIONS YOUR_TABLE")
+    print(cursor.fetchall())
+
+Conversion to Parquet and upload to S3 use `ThreadPoolExecutor`_ by default.
+It is also possible to use `ProcessPoolExecutor`_.
+
+.. code:: python
+
+    import pandas as pd
+    from concurrent.futures.process import ProcessPoolExecutor
+    from pyathena import connect
+    from pyathena.pandas.util import to_sql
+
+    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                   region_name="us-west-2")
+    df = pd.DataFrame({"a": [1, 2, 3, 4, 5]})
+    to_sql(df, "YOUR_TABLE", conn, "s3://YOUR_S3_BUCKET/path/to/",
+           schema="YOUR_SCHEMA", index=False, if_exists="replace",
+           chunksize=1, executor_class=ProcessPoolExecutor, max_workers=5)
+
+.. _`pandas.DataFrame.to_sql`: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_sql.html
+.. _`ThreadPoolExecutor`: https://docs.python.org/3/library/concurrent.futures.html#threadpoolexecutor
+.. _`ProcessPoolExecutor`: https://docs.python.org/3/library/concurrent.futures.html#processpoolexecutor
+
+DictCursor
+~~~~~~~~~~
+
+DictCursor retrieve the query execution result as a dictionary type with column names and values.
+
+You can use the DictCursor by specifying the ``cursor_class``
+with the connect method or connection object.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.cursor import DictCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=DictCursor).cursor()
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.cursor import DictCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2",
+                        cursor_class=DictCursor).cursor()
+
+It can also be used by specifying the cursor class when calling the connection object's cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.cursor import DictCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(DictCursor)
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.cursor import DictCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2").cursor(DictCursor)
+
+The basic usage is the same as the Cursor.
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.cursor import DictCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2").cursor(DictCursor)
+    cursor.execute("SELECT * FROM many_rows LIMIT 10")
+    for row in cursor:
+        print(row["a"])
+
+If you want to change the dictionary type (e.g., use OrderedDict), you can specify like the following.
+
+.. code:: python
+
+    from collections import OrderedDict
+    from pyathena import connect
+    from pyathena.cursor import DictCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=DictCursor).cursor(dict_type=OrderedDict)
+
+.. code:: python
+
+    from collections import OrderedDict
+    from pyathena import connect
+    from pyathena.cursor import DictCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(cursor=DictCursor, dict_type=OrderedDict)
+
+AsyncCursor
+~~~~~~~~~~~
+
+AsyncCursor is a simple implementation using the concurrent.futures package.
+This cursor does not follow the `DB API 2.0 (PEP 249)`_.
+
+You can use the AsyncCursor by specifying the ``cursor_class``
+with the connect method or connection object.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncCursor).cursor()
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.async_cursor import AsyncCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2",
+                        cursor_class=AsyncCursor).cursor()
+
+It can also be used by specifying the cursor class when calling the connection object's cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(AsyncCursor)
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.async_cursor import AsyncCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2").cursor(AsyncCursor)
+
+The default number of workers is 5 or cpu number * 5.
+If you want to change the number of workers you can specify like the following.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncCursor).cursor(max_workers=10)
+
+The execute method of the AsyncCursor returns the tuple of the query ID and the `future object`_.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+
+The return value of the `future object`_ is an ``AthenaResultSet`` object.
+This object has an interface that can fetch and iterate query results similar to synchronous cursors.
+It also has information on the result of query execution.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncCursor).cursor()
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    result_set = future.result()
+    print(result_set.state)
+    print(result_set.state_change_reason)
+    print(result_set.completion_date_time)
+    print(result_set.submission_date_time)
+    print(result_set.data_scanned_in_bytes)
+    print(result_set.engine_execution_time_in_millis)
+    print(result_set.query_queue_time_in_millis)
+    print(result_set.total_execution_time_in_millis)
+    print(result_set.query_planning_time_in_millis)
+    print(result_set.service_processing_time_in_millis)
+    print(result_set.output_location)
+    print(result_set.description)
+    for row in result_set:
+        print(row)
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncCursor).cursor()
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    result_set = future.result()
+    print(result_set.fetchall())
+
+A query ID is required to cancel a query with the AsyncCursor.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncCursor).cursor()
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    cursor.cancel(query_id)
+
+NOTE: The cancel method of the `future object`_ does not cancel the query.
+
+.. _`future object`: https://docs.python.org/3/library/concurrent.futures.html#future-objects
+
+AsyncDictCursor
+~~~~~~~~~~~~~~~
+
+AsyncDIctCursor is an AsyncCursor that can retrieve the query execution result
+as a dictionary type with column names and values.
+
+You can use the DictCursor by specifying the ``cursor_class``
+with the connect method or connection object.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncDictCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncDictCursor).cursor()
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.async_cursor import AsyncDictCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2",
+                        cursor_class=AsyncDictCursor).cursor()
+
+It can also be used by specifying the cursor class when calling the connection object's cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncDictCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(AsyncDictCursor)
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.async_cursor import AsyncDictCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2").cursor(AsyncDictCursor)
+
+The basic usage is the same as the AsyncCursor.
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.cursor import DictCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2").cursor(AsyncDictCursor)
+    query_id, future = cursor.execute("SELECT * FROM many_rows LIMIT 10")
+    result_set = future.result()
+    for row in result_set:
+        print(row["a"])
+
+If you want to change the dictionary type (e.g., use OrderedDict), you can specify like the following.
+
+.. code:: python
+
+    from collections import OrderedDict
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncDictCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncDictCursor).cursor(dict_type=OrderedDict)
+
+.. code:: python
+
+    from collections import OrderedDict
+    from pyathena import connect
+    from pyathena.async_cursor import AsyncDictCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(cursor=AsyncDictCursor, dict_type=OrderedDict)
+
+PandasCursor
+~~~~~~~~~~~~
+
+PandasCursor directly handles the CSV file of the query execution result output to S3.
+This cursor is to download the CSV file after executing the query, and then loaded into `pandas.DataFrame object`_.
+Performance is better than fetching data with Cursor.
+
+You can use the PandasCursor by specifying the ``cursor_class``
+with the connect method or connection object.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2",
+                        cursor_class=PandasCursor).cursor()
+
+It can also be used by specifying the cursor class when calling the connection object's cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(PandasCursor)
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2").cursor(PandasCursor)
+
+The as_pandas method returns a `pandas.DataFrame object`_.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+
+    df = cursor.execute("SELECT * FROM many_rows").as_pandas()
+    print(df.describe())
+    print(df.head())
+
+Support fetch and iterate query results.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+
+    cursor.execute("SELECT * FROM many_rows")
+    print(cursor.fetchone())
+    print(cursor.fetchmany())
+    print(cursor.fetchall())
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+
+    cursor.execute("SELECT * FROM many_rows")
+    for row in cursor:
+        print(row)
+
+The DATE and TIMESTAMP of Athena's data type are returned as `pandas.Timestamp`_ type.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+
+    cursor.execute("SELECT col_timestamp FROM one_row_complex")
+    print(type(cursor.fetchone()[0]))  # <class 'pandas._libs.tslibs.timestamps.Timestamp'>
+
+Execution information of the query can also be retrieved.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+
+    cursor.execute("SELECT * FROM many_rows")
+    print(cursor.state)
+    print(cursor.state_change_reason)
+    print(cursor.completion_date_time)
+    print(cursor.submission_date_time)
+    print(cursor.data_scanned_in_bytes)
+    print(cursor.engine_execution_time_in_millis)
+    print(cursor.query_queue_time_in_millis)
+    print(cursor.total_execution_time_in_millis)
+    print(cursor.query_planning_time_in_millis)
+    print(cursor.service_processing_time_in_millis)
+    print(cursor.output_location)
+
+If you want to customize the pandas.Dataframe object dtypes and converters, create a converter class like this:
+
+.. code:: python
+
+    from pyathena.converter import Converter
+
+    class CustomPandasTypeConverter(Converter):
+
+        def __init__(self):
+            super(CustomPandasTypeConverter, self).__init__(
+                mappings=None,
+                types={
+                    "boolean": object,
+                    "tinyint": float,
+                    "smallint": float,
+                    "integer": float,
+                    "bigint": float,
+                    "float": float,
+                    "real": float,
+                    "double": float,
+                    "decimal": float,
+                    "char": str,
+                    "varchar": str,
+                    "array": str,
+                    "map": str,
+                    "row": str,
+                    "varbinary": str,
+                    "json": str,
+                }
+            )
+
+        def convert(self, type_, value):
+            # Not used in PandasCursor.
+            pass
+
+Specify the combination of converter functions in the mappings argument and the dtypes combination in the types argument.
+
+Then you simply specify an instance of this class in the convertes argument when creating a connection or cursor.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(PandasCursor, converter=CustomPandasTypeConverter())
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     converter=CustomPandasTypeConverter()).cursor(PandasCursor)
+
+If the unload option is enabled, the Parquet file itself has a schema, so the conversion is done to the dtypes according to that schema,
+and the ``mappings`` and ``types`` settings of the Converter class are not used.
+
+If you want to change the NaN behavior of pandas.Dataframe,
+you can do so by using the ``keep_default_na``, ``na_values`` and ``quoting`` arguments of the cursor object's execute method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+    df = cursor.execute("SELECT * FROM many_rows",
+                        keep_default_na=False,
+                        na_values=[""]).as_pandas()
+
+NOTE: PandasCursor handles the CSV file on memory. Pay attention to the memory capacity.
+
+.. _`pandas.DataFrame object`: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html
+.. _`pandas.Timestamp`: https://pandas.pydata.org/docs/reference/api/pandas.Timestamp.html
+
+[PandasCursor] Chunksize options
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+The Pandas cursor can read the CSV file for each specified number of rows by using the chunksize option.
+This option should reduce memory usage.
+
+The chunksize option can be enabled by specifying an integer value in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor,
+                     cursor_kwargs={
+                         "chunksize": 1_000_000
+                     }).cursor()
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor(chunksize=1_000_000)
+
+It can also be specified in the execution method when executing the query.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+    cursor.execute("SELECT * FROM many_rows", chunksize=1_000_000)
+
+SQLAlchemy allows this option to be specified in the connection string.
+
+.. code:: text
+
+    awsathena+pandas://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&chunksize=1000000...
+
+When this option is used, the object returned by the as_pandas method is a ``DataFrameIterator`` object.
+This object has exactly the same interface as the ``TextFileReader`` object and can be handled in the same way.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+    df_iter = cursor.execute("SELECT * FROM many_rows", chunksize=1_000_000).as_pandas()
+    for df in df_iter:
+        print(df.describe())
+        print(df.head())
+
+You can also concatenate them into a single `pandas.DataFrame object`_ using `pandas.concat`_.
+
+.. code:: python
+
+    import pandas
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+    df_iter = cursor.execute("SELECT * FROM many_rows", chunksize=1_000_000).as_pandas()
+    df = pandas.concat((df for df in df_iter), ignore_index=True)
+
+You can use the ``get_chunk`` method to retrieve a `pandas.DataFrame object`_ for each specified number of rows.
+When all rows have been read, calling the ``get_chunk`` method will raise ``StopIteration``.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor()
+    df_iter = cursor.execute("SELECT * FROM many_rows LIMIT 15", chunksize=1_000_000).as_pandas()
+    df_iter.get_chunk(10)
+    df_iter.get_chunk(10)
+    df_iter.get_chunk(10)  # raise StopIteration
+
+.. _`pandas.concat`: https://pandas.pydata.org/docs/reference/api/pandas.concat.html
+
+[PandasCursor] Unload options
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+PandasCursor also supports the unload option, as does `ArrowCursor`_.
+
+See `[ArrowCursor] Unload options`_ for more information.
+
+The unload option can be enabled by specifying it in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor,
+                     cursor_kwargs={
+                         "unload": True
+                     }).cursor()
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import PandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=PandasCursor).cursor(unload=True)
+
+SQLAlchemy allows this option to be specified in the connection string.
+
+.. code:: text
+
+    awsathena+pandas://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&unload=true...
+
+AsyncPandasCursor
+~~~~~~~~~~~~~~~~~
+
+AsyncPandasCursor is an AsyncCursor that can handle `pandas.DataFrame object`_.
+This cursor directly handles the CSV of query results output to S3 in the same way as PandasCursor.
+
+You can use the AsyncPandasCursor by specifying the ``cursor_class``
+with the connect method or connection object.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor).cursor()
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2",
+                        cursor_class=AsyncPandasCursor).cursor()
+
+It can also be used by specifying the cursor class when calling the connection object's cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(AsyncPandasCursor)
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2").cursor(AsyncPandasCursor)
+
+The default number of workers is 5 or cpu number * 5.
+If you want to change the number of workers you can specify like the following.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor).cursor(max_workers=10)
+
+The execute method of the AsyncPandasCursor returns the tuple of the query ID and the `future object`_.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+
+The return value of the `future object`_ is an ``AthenaPandasResultSet`` object.
+This object has an interface similar to ``AthenaResultSetObject``.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    result_set = future.result()
+    print(result_set.state)
+    print(result_set.state_change_reason)
+    print(result_set.completion_date_time)
+    print(result_set.submission_date_time)
+    print(result_set.data_scanned_in_bytes)
+    print(result_set.engine_execution_time_in_millis)
+    print(result_set.query_queue_time_in_millis)
+    print(result_set.total_execution_time_in_millis)
+    print(result_set.query_planning_time_in_millis)
+    print(result_set.service_processing_time_in_millis)
+    print(result_set.output_location)
+    print(result_set.description)
+    for row in result_set:
+        print(row)
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    result_set = future.result()
+    print(result_set.fetchall())
+
+This object also has an as_pandas method that returns a `pandas.DataFrame object`_ similar to the PandasCursor.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    result_set = future.result()
+    df = result_set.as_pandas()
+    print(df.describe())
+    print(df.head())
+
+The DATE and TIMESTAMP of Athena's data type are returned as `pandas.Timestamp`_ type.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT col_timestamp FROM one_row_complex")
+    result_set = future.result()
+    print(type(result_set.fetchone()[0]))  # <class 'pandas._libs.tslibs.timestamps.Timestamp'>
+
+As with AsyncCursor, you need a query ID to cancel a query.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.async_cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    cursor.cancel(query_id)
+
+As with PandasCursor, the unload option is also available.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor,
+                     cursor_kwargs={
+                         "unload": True
+                     }).cursor()
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.pandas.cursor import AsyncPandasCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncPandasCursor).cursor(unload=True)
+
+ArrowCursor
+~~~~~~~~~~~
+
+ArrowCursor directly handles the CSV file of the query execution result output to S3.
+This cursor is to download the CSV file after executing the query, and then loaded into `pyarrow.Table object`_.
+Performance is better than fetching data with Cursor.
+
+You can use the ArrowCursor by specifying the ``cursor_class``
+with the connect method or connection object.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=ArrowCursor).cursor()
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2",
+                        cursor_class=ArrowCursor).cursor()
+
+It can also be used by specifying the cursor class when calling the connection object's cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(ArrowCursor)
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2").cursor(ArrowCursor)
+
+The as_arrow method returns a `pyarrow.Table object`_.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=ArrowCursor).cursor()
+
+    table = cursor.execute("SELECT * FROM many_rows").as_arrow()
+    print(table)
+    print(table.column_names)
+    print(table.columns)
+    print(table.nbytes)
+    print(table.num_columns)
+    print(table.num_rows)
+    print(table.schema)
+    print(table.shape)
+
+Support fetch and iterate query results.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=ArrowCursor).cursor()
+
+    cursor.execute("SELECT * FROM many_rows")
+    print(cursor.fetchone())
+    print(cursor.fetchmany())
+    print(cursor.fetchall())
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=ArrowCursor).cursor()
+
+    cursor.execute("SELECT * FROM many_rows")
+    for row in cursor:
+        print(row)
+
+Execution information of the query can also be retrieved.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=ArrowCursor).cursor()
+
+    cursor.execute("SELECT * FROM many_rows")
+    print(cursor.state)
+    print(cursor.state_change_reason)
+    print(cursor.completion_date_time)
+    print(cursor.submission_date_time)
+    print(cursor.data_scanned_in_bytes)
+    print(cursor.engine_execution_time_in_millis)
+    print(cursor.query_queue_time_in_millis)
+    print(cursor.total_execution_time_in_millis)
+    print(cursor.query_planning_time_in_millis)
+    print(cursor.service_processing_time_in_millis)
+    print(cursor.output_location)
+
+If you want to customize the `pyarrow.Table object`_ types, create a converter class like this:
+
+.. code:: python
+
+    import pyarrow as pa
+    from pyathena.arrow.converter import _to_date
+    from pyathena.converter import Converter
+
+    class CustomArrowTypeConverter(Converter):
+        def __init__(self) -> None:
+            super(CustomArrowTypeConverter, self).__init__(
+                mappings={
+                    "date": _to_date,
+                },
+                types={
+                    "boolean": pa.bool_(),
+                    "tinyint": pa.int8(),
+                    "smallint": pa.int16(),
+                    "integer": pa.int32(),
+                    "bigint": pa.int64(),
+                    "float": pa.float32(),
+                    "real": pa.float64(),
+                    "double": pa.float64(),
+                    "char": pa.string(),
+                    "varchar": pa.string(),
+                    "string": pa.string(),
+                    "timestamp": pa.timestamp("ms"),
+                    "date": pa.timestamp("ms"),
+                    "time": pa.string(),
+                    "varbinary": pa.string(),
+                    "array": pa.string(),
+                    "map": pa.string(),
+                    "row": pa.string(),
+                    "decimal": pa.string(),
+                    "json": pa.string(),
+                },
+            )
+
+    def convert(self, type_, value):
+        converter = self.get(type_)
+        return converter(value)
+
+``types`` is used to explicitly specify the Arrow type when reading CSV files.
+``mappings`` is used as a conversion method when fetching data from a cursor object.
+
+Then you simply specify an instance of this class in the convertes argument when creating a connection or cursor.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(ArrowCursor, converter=CustomArrowTypeConverter())
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     converter=CustomArrowTypeConverter()).cursor(ArrowCursor)
+
+If the unload option is enabled, the Parquet file itself has a schema, so the conversion is done to the Arrow type according to that schema,
+and the ``types`` setting of the Converter class is not used.
+
+[ArrowCursor] Unload options
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+ArrowCursor supports the unload option. When this option is enabled,
+queries with SELECT statements are automatically converted to unload statements and executed to Athena,
+and the results are output in Parquet format (Snappy compressed) to ``s3_staging_dir``.
+The cursor reads the output Parquet file directly.
+
+The output of query results with the unload statement is faster than normal query execution.
+In addition, the output Parquet file is split and can be read faster than a CSV file.
+We recommend trying this option if you are concerned about the time it takes to execute the query and retrieve the results.
+
+However, unload has some limitations. Please refer to the `official unload documentation`_ for more information on limitations.
+As per the limitations of the official documentation, the results of unload will be written to multiple files in parallel,
+and the contents of each file will be in sort order, but the relative order of the files to each other will not be sorted.
+Note that specifying ORDER BY with this option enabled does not guarantee the sort order of the data.
+
+The unload option can be enabled by specifying it in the ``cursor_kwargs`` argument of the connect method or as an argument to the cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=ArrowCursor,
+                     cursor_kwargs={
+                         "unload": True
+                     }).cursor()
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import ArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=ArrowCursor).cursor(unload=True)
+
+SQLAlchemy allows this option to be specified in the connection string.
+
+.. code:: text
+
+    awsathena+arrow://:@athena.{region_name}.amazonaws.com:443/{schema_name}?s3_staging_dir={s3_staging_dir}&unload=true...
+
+If a ``NOT_SUPPORTED`` occurs, a type not supported by unload is included in the result of the SELECT.
+Try converting to another type, such as ``SELECT CAST(1 AS VARCHAR) AS name``.
+
+.. code:: text
+
+    pyathena.error.OperationalError: NOT_SUPPORTED: Unsupported Hive type: time
+
+In most cases of ``SYNTAX_ERROR``, you forgot to alias the column in the SELECT result.
+Try adding an alias to the SELECTed column, such as ``SELECT 1 AS name``.
+
+.. code:: text
+
+    pyathena.error.OperationalError: SYNTAX_ERROR: line 1:1: Column name not specified at position 1
+
+.. _`pyarrow.Table object`: https://arrow.apache.org/docs/python/generated/pyarrow.Table.html
+.. _`official unload documentation`: https://docs.aws.amazon.com/athena/latest/ug/unload.html
+
+AsyncArrowCursor
+~~~~~~~~~~~~~~~~
+
+AsyncArrowCursor is an AsyncCursor that can handle `pyarrow.Table object`_.
+This cursor directly handles the CSV of query results output to S3 in the same way as ArrowCursor.
+
+You can use the AsyncArrowCursor by specifying the ``cursor_class``
+with the connect method or connection object.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncArrowCursor).cursor()
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2",
+                        cursor_class=AsyncArrowCursor).cursor()
+
+It can also be used by specifying the cursor class when calling the connection object's cursor method.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor(AsyncArrowCursor)
+
+.. code:: python
+
+    from pyathena.connection import Connection
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = Connection(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                        region_name="us-west-2").cursor(AsyncArrowCursor)
+
+The default number of workers is 5 or cpu number * 5.
+If you want to change the number of workers you can specify like the following.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncArrowCursor).cursor(max_workers=10)
+
+The execute method of the AsyncArrowCursor returns the tuple of the query ID and the `future object`_.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncArrowCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+
+The return value of the `future object`_ is an ``AthenaArrowResultSet`` object.
+This object has an interface similar to ``AthenaResultSetObject``.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncArrowCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    result_set = future.result()
+    print(result_set.state)
+    print(result_set.state_change_reason)
+    print(result_set.completion_date_time)
+    print(result_set.submission_date_time)
+    print(result_set.data_scanned_in_bytes)
+    print(result_set.engine_execution_time_in_millis)
+    print(result_set.query_queue_time_in_millis)
+    print(result_set.total_execution_time_in_millis)
+    print(result_set.query_planning_time_in_millis)
+    print(result_set.service_processing_time_in_millis)
+    print(result_set.output_location)
+    print(result_set.description)
+    for row in result_set:
+        print(row)
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncArrowCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    result_set = future.result()
+    print(result_set.fetchall())
+
+This object also has an as_arrow method that returns a `pyarrow.Table object`_ similar to the ArrowCursor.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncArrowCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    result_set = future.result()
+    table = result_set.as_arrow()
+    print(table)
+    print(table.column_names)
+    print(table.columns)
+    print(table.nbytes)
+    print(table.num_columns)
+    print(table.num_rows)
+    print(table.schema)
+    print(table.shape)
+
+As with AsyncCursor, you need a query ID to cancel a query.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.async_cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncArrowCursor).cursor()
+
+    query_id, future = cursor.execute("SELECT * FROM many_rows")
+    cursor.cancel(query_id)
+
+As with ArrowCursor, the UNLOAD option is also available.
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncArrowCursor,
+                     cursor_kwargs={
+                         "unload": True
+                     }).cursor()
+
+.. code:: python
+
+    from pyathena import connect
+    from pyathena.arrow.cursor import AsyncArrowCursor
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2",
+                     cursor_class=AsyncArrowCursor).cursor(unload=True)
+
+Quickly re-run queries
+~~~~~~~~~~~~~~~~~~~~~~
+
+Result reuse configuration
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Athena engine version 3 allows you to `reuse the results of previous queries`_.
+
+It is available by specifying the arguments ``result_reuse_enable`` and ``result_reuse_minutes`` in the connection object.
+
+.. code:: python
+
+    from pyathena import connect
+
+    conn = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                   region_name="us-west-2",
+                   work_group="YOUR_WORK_GROUP",
+                   result_reuse_enable=True,
+                   result_reuse_minutes=60)
+
+You can also specify ``result_reuse_enable`` and ``result_reuse_minutes`` when executing a query.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+    cursor.execute("SELECT * FROM one_row",
+                   work_group="YOUR_WORK_GROUP",
+                   result_reuse_enable=True,
+                   result_reuse_minutes=60)
+
+If the following error occurs, please use a workgroup configured with Athena engine version 3.
+
+.. code:: text
+
+    pyathena.error.DatabaseError: An error occurred (InvalidRequestException) when calling the StartQueryExecution operation: This functionality is not enabled in the selected engine version. Please check the engine version settings or contact AWS support for further assistance.
+
+If for some reason you cannot use the reuse feature of Athena engine version 3, please use the `Cache configuration`_ implemented by PyAthena.
+
+.. _`reuse the results of previous queries`: https://docs.aws.amazon.com/athena/latest/ug/reusing-query-results.html
+
+Cache configuration
+^^^^^^^^^^^^^^^^^^^
+
+**Please use the Result reuse configuration.**
+
+You can attempt to re-use the results from a previously executed query to help save time and money in the cases where your underlying data isn't changing.
+Set the ``cache_size`` or ``cache_expiration_time`` parameter of ``cursor.execute()`` to a number larger than 0 to enable caching.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+    cursor.execute("SELECT * FROM one_row")  # run once
+    print(cursor.query_id)
+    cursor.execute("SELECT * FROM one_row", cache_size=10)  # re-use earlier results
+    print(cursor.query_id)  # You should expect to see the same Query ID
+
+The unit of ``expiration_time`` is seconds. To use the results of queries executed up to one hour ago, specify like the following.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+    cursor.execute("SELECT * FROM one_row", cache_expiration_time=3600)  # Use queries executed within 1 hour as cache.
+
+If ``cache_size`` is not specified, the value of ``sys.maxsize`` will be automatically set and all query results executed up to one hour ago will be checked.
+Therefore, it is recommended to specify ``cache_expiration_time`` together with ``cache_size`` like the following.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+    cursor.execute("SELECT * FROM one_row", cache_size=100, cache_expiration_time=3600)  # Use the last 100 queries within 1 hour as cache.
+
+Results will only be re-used if the query strings match *exactly*,
+and the query was a DML statement (the assumption being that you always want to re-run queries like ``CREATE TABLE`` and ``DROP TABLE``).
+
+The S3 staging directory is not checked, so it's possible that the location of the results is not in your provided ``s3_staging_dir``.
+
+Credentials
+-----------
+
+Support `Boto3 credentials`_.
+
+.. _`Boto3 credentials`: http://boto3.readthedocs.io/en/latest/guide/configuration.html
+
+Additional environment variable:
+
+.. code:: bash
+
+    $ export AWS_ATHENA_S3_STAGING_DIR=s3://YOUR_S3_BUCKET/path/to/
+    $ export AWS_ATHENA_WORK_GROUP=YOUR_WORK_GROUP
+
+Examples
+~~~~~~~~
+
+Passing credentials as parameters
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(aws_access_key_id="YOUR_ACCESS_KEY_ID",
+                     aws_secret_access_key="YOUR_SECRET_ACCESS_KEY",
+                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(aws_access_key_id="YOUR_ACCESS_KEY_ID",
+                     aws_secret_access_key="YOUR_SECRET_ACCESS_KEY",
+                     aws_session_token="YOUR_SESSION_TOKEN",
+                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+
+Multi-factor authentication
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+You will be prompted to enter the MFA code.
+The program execution will be blocked until the MFA code is entered.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(duration_seconds=3600,
+                     serial_number="arn:aws:iam::ACCOUNT_NUMBER_WITHOUT_HYPHENS:mfa/MFA_DEVICE_ID",
+                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+
+Shared credentials file
+^^^^^^^^^^^^^^^^^^^^^^^
+
+The shared credentials file has a default location of ~/.aws/credentials.
+
+If you use the default profile, there is no need to specify credential information.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+
+You can also specify a profile other than the default.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(profile_name="YOUR_PROFILE_NAME",
+                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+
+Assume role provider
+^^^^^^^^^^^^^^^^^^^^
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(role_arn="YOUR_ASSUME_ROLE_ARN",
+                     role_session_name="PyAthena-session",
+                     duration_seconds=3600,
+                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+
+Assume role provider with MFA
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+You will be prompted to enter the MFA code.
+The program execution will be blocked until the MFA code is entered.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(role_arn="YOUR_ASSUME_ROLE_ARN",
+                     role_session_name="PyAthena-session",
+                     duration_seconds=3600,
+                     serial_number="arn:aws:iam::ACCOUNT_NUMBER_WITHOUT_HYPHENS:mfa/MFA_DEVICE_ID",
+                     s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+
+Instance profiles
+^^^^^^^^^^^^^^^^^
+
+No need to specify credential information.
+
+.. code:: python
+
+    from pyathena import connect
+
+    cursor = connect(s3_staging_dir="s3://YOUR_S3_BUCKET/path/to/",
+                     region_name="us-west-2").cursor()
+
+Testing
+-------
+
+Depends on the following environment variables:
+
+.. code:: bash
+
+    $ export AWS_DEFAULT_REGION=us-west-2
+    $ export AWS_ATHENA_S3_STAGING_DIR=s3://YOUR_S3_BUCKET/path/to/
+    $ export AWS_ATHENA_WORKGROUP=pyathena-test
+
+In addition, you need to create a workgroup with the `Query result location` set to the name specified in the `AWS_ATHENA_WORKGROUP` environment variable.
+If primary is not available as the default workgroup, specify an alternative workgroup name for the default in the environment variable `AWS_ATHENA_DEFAULT_WORKGROUP`.
+
+.. code:: bash
+
+    $ export AWS_ATHENA_DEFAULT_WORKGROUP=DEFAULT_WORKGROUP
+
+Run test
+~~~~~~~~
+
+.. code:: bash
+
+    $ pip install poetry
+    $ poetry install -v
+    $ poetry run pytest
+
+Run test multiple Python versions
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ pip install poetry
+    $ poetry install -v
+    $ pyenv local 3.11.1 3.10.1 3.9.1 3.8.2
+    $ poetry run tox
+
+GitHub Actions
+~~~~~~~~~~~~~~
+
+GitHub Actions uses OpenID Connect (OIDC) to access AWS resources. You will need to refer to the `GitHub Actions documentation`_ to configure it.
+
+.. _`GitHub Actions documentation`: https://docs.github.com/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services
+
+The CloudFormation templates for creating GitHub OIDC Provider and IAM Role can be found in the `aws-actions/configure-aws-credentials repository`_.
+
+.. _`aws-actions/configure-aws-credentials repository`: https://github.com/aws-actions/configure-aws-credentials#sample-iam-role-cloudformation-template
+
+Under `scripts/cloudformation`_ you will also find a CloudFormation template with additional permissions and workgroup settings needed for testing.
+
+.. _`scripts/cloudformation`: scripts/cloudformation/
+
+The example of the CloudFormation execution command is the following:
+
+.. code:: bash
+
+    $ aws --region us-west-2 \
+        cloudformation create-stack \
+        --stack-name github-actions-oidc-pyathena \
+        --capabilities CAPABILITY_NAMED_IAM \
+        --template-body file://./scripts/cloudformation/github_actions_oidc.yaml \
+        --parameters ParameterKey=GitHubOrg,ParameterValue=laughingman7743 \
+          ParameterKey=RepositoryName,ParameterValue=PyAthena \
+          ParameterKey=BucketName,ParameterValue=laughingman7743-athena \
+          ParameterKey=RoleName,ParameterValue=github-actions-oidc-pyathena-test \
+          ParameterKey=WorkGroupName,ParameterValue=pyathena-test
+
+Code formatting
+---------------
+
+The code formatting uses `black`_ and `isort`_.
+
+Appy format
+~~~~~~~~~~~
+
+.. code:: bash
+
+    $ make fmt
+
+Check format
+~~~~~~~~~~~~
+
+.. code:: bash
+
+    $ make chk
+
+.. _`black`: https://github.com/psf/black
+.. _`isort`: https://github.com/timothycrosley/isort
+
+License
+-------
+
+`MIT license`_
+
+Many of the implementations in this library are based on `PyHive`_, thanks for `PyHive`_.
+
+.. _`MIT license`: LICENSE
+.. _`PyHive`: https://github.com/dropbox/PyHive
 
-setup(**setup_kwargs)
```

