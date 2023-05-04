# Comparing `tmp/duckingit-0.0.3.tar.gz` & `tmp/duckingit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckingit-0.0.3.tar", last modified: Thu Apr 13 19:27:53 2023, max compression
+gzip compressed data, was "duckingit-0.0.4.tar", last modified: Thu May  4 20:01:57 2023, max compression
```

## Comparing `duckingit-0.0.3.tar` & `duckingit-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-04-13 19:27:53.604305 duckingit-0.0.3/
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3933 2023-04-13 19:27:53.603778 duckingit-0.0.3/PKG-INFO
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3328 2023-04-13 19:09:01.000000 duckingit-0.0.3/README.md
-drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-04-13 19:27:53.598373 duckingit-0.0.3/duckingit/
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       66 2023-04-10 18:13:42.000000 duckingit-0.0.3/duckingit/__init__.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     1350 2023-04-13 16:52:25.000000 duckingit-0.0.3/duckingit/_analyze.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     1773 2023-04-13 17:18:52.000000 duckingit-0.0.3/duckingit/_config.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     2104 2023-04-13 17:18:18.000000 duckingit-0.0.3/duckingit/_controller.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      760 2023-04-13 17:02:57.000000 duckingit-0.0.3/duckingit/_encode.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      186 2023-04-12 13:01:34.000000 duckingit-0.0.3/duckingit/_exceptions.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     2322 2023-04-13 17:14:20.000000 duckingit-0.0.3/duckingit/_parser.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     2294 2023-04-13 17:14:14.000000 duckingit-0.0.3/duckingit/_planner.py
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     5502 2023-04-13 17:18:29.000000 duckingit-0.0.3/duckingit/_session.py
-drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-04-13 19:27:53.602518 duckingit-0.0.3/duckingit.egg-info/
--rw-r--r--   0 tobiasegelund   (501) staff       (20)     3933 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/PKG-INFO
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      389 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/SOURCES.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)        1 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/dependency_links.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       29 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/requires.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       10 2023-04-13 19:27:53.000000 duckingit-0.0.3/duckingit.egg-info/top_level.txt
--rw-r--r--   0 tobiasegelund   (501) staff       (20)      824 2023-04-13 19:25:57.000000 duckingit-0.0.3/pyproject.toml
--rw-r--r--   0 tobiasegelund   (501) staff       (20)       38 2023-04-13 19:27:53.604469 duckingit-0.0.3/setup.cfg
+drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-05-04 20:01:57.600434 duckingit-0.0.4/
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     3989 2023-05-04 20:01:57.599905 duckingit-0.0.4/PKG-INFO
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     3384 2023-04-24 18:02:10.000000 duckingit-0.0.4/README.md
+drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-05-04 20:01:57.597292 duckingit-0.0.4/duckingit/
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)       84 2023-04-16 18:57:16.000000 duckingit-0.0.4/duckingit/__init__.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     9646 2023-05-01 17:56:53.000000 duckingit-0.0.4/duckingit/_config.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     6041 2023-05-04 19:55:25.000000 duckingit-0.0.4/duckingit/_controller.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     5304 2023-05-04 18:24:11.000000 duckingit-0.0.4/duckingit/_dataset.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)      281 2023-04-20 17:31:23.000000 duckingit-0.0.4/duckingit/_exceptions.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)      624 2023-04-16 10:14:45.000000 duckingit-0.0.4/duckingit/_extensions.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     2940 2023-05-01 18:26:48.000000 duckingit-0.0.4/duckingit/_parser.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     9323 2023-05-04 19:43:48.000000 duckingit-0.0.4/duckingit/_planner.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     3476 2023-05-01 17:56:53.000000 duckingit-0.0.4/duckingit/_session.py
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     4476 2023-05-01 18:02:27.000000 duckingit-0.0.4/duckingit/_utils.py
+drwxr-xr-x   0 tobiasegelund   (501) staff       (20)        0 2023-05-04 20:01:57.599268 duckingit-0.0.4/duckingit.egg-info/
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)     3989 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/PKG-INFO
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)      413 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)        1 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)       29 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/requires.txt
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)       10 2023-05-04 20:01:57.000000 duckingit-0.0.4/duckingit.egg-info/top_level.txt
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)      824 2023-05-04 20:01:15.000000 duckingit-0.0.4/pyproject.toml
+-rw-r--r--   0 tobiasegelund   (501) staff       (20)       38 2023-05-04 20:01:57.600594 duckingit-0.0.4/setup.cfg
```

### Comparing `duckingit-0.0.3/PKG-INFO` & `duckingit-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,37 +43,41 @@
 ```
 
 After waiting for a minute or two, the infrastructure should be set up, and you can check for the presence of a Lambda function called DuckExecutor and a lambda layer called duckdb under Lambda layers.
 
 Once you have verified the above components, the infrastructure should be set up and fully operational.
 
 ## Usage
-The framework's developer API draws inspiration from Spark's API, but it uses Python's naming conventions because the framework is implemented in Python.
+The developer API is inspired by the API of Spark, but it uses Python's naming conventions because the framework is implemented in Python.
 
 ```python
-from duckingit import DuckSession
+from duckingit import DuckSession, DuckConfig
 
 query = "SELECT * FROM READ_PARQUET(['s3://BUCKET_NAME/2023/*'])"
 
+# Following command will print possible configurations
+DuckConfig.show_configurations
+
+# Configuration
+conf = DuckConfig() \
+        .set("aws_lambda.FunctionName", "TestFunc") \
+        .set("aws_lambda.MemorySize", 256) \
+        .set("aws_lambda.WarmUp", True)
+
 # Creates an entrypoint to use serverless DuckDB instances
-session = DuckSession()
+session = DuckSession(conf=conf)
 
-# Updates the Lambda function with 128 MB memory size and 30 timeout
-# as well as initializing the Lambda function to avoid cold start
-session.conf.memory_size(128).timeout(30).warm_up().update()
+# Create a Dataset from the query
+ds = session.sql(query=query)
 
-# Execute the command
-session.execute(query=query)
+# Execute SQL query
+ds.show()
 ```
 
 ... To be continued
 
 ## Contribution
 Thank you for taking an interest in my project on GitHub. I am always looking for new contributors to help me improve and evolve my codebase. If you're interested in contributing, feel free to fork the repository and submit a pull request with your changes.
 
 I welcome all kinds of contributions, from bug fixes to feature additions and documentation improvements. If you're not sure where to start, take a look at the issues tab or reach out to us for guidance.
 
 Let's collaborate and make our project better together!
-
-
-___________________________________
-Ducking it ~ Killing it
```

### Comparing `duckingit-0.0.3/README.md` & `duckingit-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,37 +29,41 @@
 ```
 
 After waiting for a minute or two, the infrastructure should be set up, and you can check for the presence of a Lambda function called DuckExecutor and a lambda layer called duckdb under Lambda layers.
 
 Once you have verified the above components, the infrastructure should be set up and fully operational.
 
 ## Usage
-The framework's developer API draws inspiration from Spark's API, but it uses Python's naming conventions because the framework is implemented in Python.
+The developer API is inspired by the API of Spark, but it uses Python's naming conventions because the framework is implemented in Python.
 
 ```python
-from duckingit import DuckSession
+from duckingit import DuckSession, DuckConfig
 
 query = "SELECT * FROM READ_PARQUET(['s3://BUCKET_NAME/2023/*'])"
 
+# Following command will print possible configurations
+DuckConfig.show_configurations
+
+# Configuration
+conf = DuckConfig() \
+        .set("aws_lambda.FunctionName", "TestFunc") \
+        .set("aws_lambda.MemorySize", 256) \
+        .set("aws_lambda.WarmUp", True)
+
 # Creates an entrypoint to use serverless DuckDB instances
-session = DuckSession()
+session = DuckSession(conf=conf)
 
-# Updates the Lambda function with 128 MB memory size and 30 timeout
-# as well as initializing the Lambda function to avoid cold start
-session.conf.memory_size(128).timeout(30).warm_up().update()
+# Create a Dataset from the query
+ds = session.sql(query=query)
 
-# Execute the command
-session.execute(query=query)
+# Execute SQL query
+ds.show()
 ```
 
 ... To be continued
 
 ## Contribution
 Thank you for taking an interest in my project on GitHub. I am always looking for new contributors to help me improve and evolve my codebase. If you're interested in contributing, feel free to fork the repository and submit a pull request with your changes.
 
 I welcome all kinds of contributions, from bug fixes to feature additions and documentation improvements. If you're not sure where to start, take a look at the issues tab or reach out to us for guidance.
 
 Let's collaborate and make our project better together!
-
-
-___________________________________
-Ducking it ~ Killing it
```

### Comparing `duckingit-0.0.3/duckingit/_parser.py` & `duckingit-0.0.4/duckingit/_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,97 @@
 import re
+import typing as t
+import copy
 from dataclasses import dataclass
 
 import sqlglot
-import sqlglot.expressions as expr
-import sqlglot.planner as planner
+import sqlglot.expressions as exp
 
 from duckingit._exceptions import InvalidFilesystem, ParserError
-from duckingit._encode import create_md5_hash_string
+from duckingit._utils import create_hash_string, scan_source_for_prefixes
 
 
 @dataclass
 class Query:
     sql: str
     hashed: str
-    expression: expr.Expression
-    dag: planner.Plan
+    ast: exp.Expression
 
     _list_of_prefixes: list[str] | None = None
 
     @classmethod
     def parse(cls, query: str):
         query = cls._unify_query(query)
 
-        expression = sqlglot.parse_one(query)
-        dag = planner.Plan(expression)
+        expression = sqlglot.parse_one(query, read="duckdb")
+        # optimized_expression = optimizer.optimize(expression)
 
         return cls(
             sql=query,
-            hashed=create_md5_hash_string(query),
-            expression=expression,
-            dag=dag,
+            hashed=create_hash_string(query),
+            ast=expression,
         )
 
     @property
     def list_of_prefixes(self) -> list[str]:
         if self._list_of_prefixes is None:
-            return [self.source]
+            self._list_of_prefixes = scan_source_for_prefixes(source=self.source)
         return self._list_of_prefixes
 
-    @list_of_prefixes.setter
-    def list_of_prefixes(self, prefixes: list[str]) -> None:
-        if not isinstance(prefixes, list):
-            raise ValueError(f"{prefixes} must be a list of strings")
-        self._list_of_prefixes = prefixes
+    @property
+    def tables(self) -> t.Generator:
+        """Returns a generator that yields over table expressions, e.g. READ_PARQUET(VALUES(XX))"""
+        yield from self.ast.find_all(exp.Table)
+
+    @property
+    def from_(self) -> t.Generator:
+        """Returns a generator that yields over from expressions, e.g. FROM READ_PARQUET(VALUES(XX))"""
+        yield from self.ast.find_all(exp.From)
 
     @property
     def bucket(self) -> str:
-        pattern = r"s3:\/\/([A-Za-z0-9_-]+)"
-        match = re.search(pattern, self.sql)
+        """Returns the name of the bucket, e.g. s3://bucket-name-test
 
-        if not match:
-            raise ValueError("Couldn't find bucket name in query")
-        # TODO: Make regex more generic
-        return "s3://" + match.group(1)
+        Note that DuckDB uses S3 for GCP as well
+        https://duckdb.org/docs/guides/import/s3_import.html
+        """
+        for table in self.tables:
+            pattern = r"s3:\/\/([A-Za-z0-9_-]+)"
+            match = re.search(pattern, str(table))
 
-    @property
-    def _source(self) -> str:
-        return self.dag.root.source.sql()
+            if not match:
+                continue
+
+            return "s3://" + match.group(1)  # yield?
+
+        raise ValueError("Not able to locate any bucket name in query")
 
     @property
     def source(self) -> str:
+        """Returns the source of the table, e.g. s3://BUCKET_NAME/2023"""
         # TODO: Update exceptions to user-defined exceptions
-        if self._source[1:3] == "s3":
-            return self._source
+        for table in self.tables:
+            # TODO: Update pattern for other filesystems or extensions
+            # What about single file?
+            pattern = r"ARRAY\((.*?)\)"  # sqlglot bug, should be LIST_VALUE
+            match = re.search(pattern, str(table))
+
+            if not match:
+                continue
 
-        # TODO: Update pattern for other filesystems or extensions
-        # What about single file?
-        pattern = r"LIST_VALUE\((.*?)\)"
-        match = re.findall(pattern, self._source)
-
-        if len(match) == 0:
-            raise InvalidFilesystem(
-                "An acceptable filesystem, e.g. 's3://<BUCKET_NAME>/*', couldn't be \
-found."
-            )
+            # TODO: Update to generator
+            return match.group(1)
+
+        raise InvalidFilesystem(
+            "An acceptable filesystem, e.g. 's3://BUCKET_NAME/*', couldn't be found."
+        )
 
-        return match[0]
+    def copy(self):
+        """Returns a deep copy of the object itself"""
+        return copy.deepcopy(self)
 
     @classmethod
     def _unify_query(cls, query: str) -> str:
         try:
             return sqlglot.transpile(query, read="duckdb")[0]
         except Exception as e:
-            raise ParserError(e)
+            raise ParserError(e) from e
```

### Comparing `duckingit-0.0.3/duckingit.egg-info/PKG-INFO` & `duckingit-0.0.4/duckingit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckingit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB
 Author-email: Tobias Egelund <egelundtobias@gmail.com>
 Project-URL: Homepage, https://github.com/tobiasegelund/duckingit
 Project-URL: Bug Tracker, https://github.com/tobiasegelund/duckingit/issues
 Keywords: Serverless,DuckDB,Data Engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,37 +43,41 @@
 ```
 
 After waiting for a minute or two, the infrastructure should be set up, and you can check for the presence of a Lambda function called DuckExecutor and a lambda layer called duckdb under Lambda layers.
 
 Once you have verified the above components, the infrastructure should be set up and fully operational.
 
 ## Usage
-The framework's developer API draws inspiration from Spark's API, but it uses Python's naming conventions because the framework is implemented in Python.
+The developer API is inspired by the API of Spark, but it uses Python's naming conventions because the framework is implemented in Python.
 
 ```python
-from duckingit import DuckSession
+from duckingit import DuckSession, DuckConfig
 
 query = "SELECT * FROM READ_PARQUET(['s3://BUCKET_NAME/2023/*'])"
 
+# Following command will print possible configurations
+DuckConfig.show_configurations
+
+# Configuration
+conf = DuckConfig() \
+        .set("aws_lambda.FunctionName", "TestFunc") \
+        .set("aws_lambda.MemorySize", 256) \
+        .set("aws_lambda.WarmUp", True)
+
 # Creates an entrypoint to use serverless DuckDB instances
-session = DuckSession()
+session = DuckSession(conf=conf)
 
-# Updates the Lambda function with 128 MB memory size and 30 timeout
-# as well as initializing the Lambda function to avoid cold start
-session.conf.memory_size(128).timeout(30).warm_up().update()
+# Create a Dataset from the query
+ds = session.sql(query=query)
 
-# Execute the command
-session.execute(query=query)
+# Execute SQL query
+ds.show()
 ```
 
 ... To be continued
 
 ## Contribution
 Thank you for taking an interest in my project on GitHub. I am always looking for new contributors to help me improve and evolve my codebase. If you're interested in contributing, feel free to fork the repository and submit a pull request with your changes.
 
 I welcome all kinds of contributions, from bug fixes to feature additions and documentation improvements. If you're not sure where to start, take a look at the issues tab or reach out to us for guidance.
 
 Let's collaborate and make our project better together!
-
-
-___________________________________
-Ducking it ~ Killing it
```

### Comparing `duckingit-0.0.3/pyproject.toml` & `duckingit-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "duckingit"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   {name="Tobias Egelund", email="egelundtobias@gmail.com" },
 ]
 description = "A framework to leverage clusters of serverless functions for analytics. Powered by DuckDB"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["Serverless", "DuckDB", "Data Engineering"]
```

