# Comparing `tmp/PyVecDB-0.1.1.tar.gz` & `tmp/PyVecDB-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyVecDB-0.1.1.tar", last modified: Mon May  1 11:19:41 2023, max compression
+gzip compressed data, was "PyVecDB-0.1.2.tar", last modified: Thu May  4 12:54:32 2023, max compression
```

## Comparing `PyVecDB-0.1.1.tar` & `PyVecDB-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/
--rw-rw-rw-   0        0        0     2666 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/PyVecDB.egg-info/
--rw-rw-rw-   0        0        0     2666 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 11:19:41.000000 PyVecDB-0.1.1/PyVecDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1928 2023-05-01 11:15:48.000000 PyVecDB-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-01 11:18:13.000000 PyVecDB-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/src/
--rw-rw-rw-   0        0        0       29 2023-05-01 07:38:16.000000 PyVecDB-0.1.1/src/__init__.py
--rw-rw-rw-   0        0        0     1583 2023-05-01 07:47:53.000000 PyVecDB-0.1.1/src/data_object.py
--rw-rw-rw-   0        0        0      459 2023-04-30 14:04:33.000000 PyVecDB-0.1.1/src/database.py
--rw-rw-rw-   0        0        0     1742 2023-05-01 07:37:56.000000 PyVecDB-0.1.1/src/stress_test.py
--rw-rw-rw-   0        0        0     3875 2023-04-30 16:05:40.000000 PyVecDB-0.1.1/src/vector_db.py
--rw-rw-rw-   0        0        0     5102 2023-05-01 08:46:52.000000 PyVecDB-0.1.1/src/word_generator.py
-drwxrwxrwx   0        0        0        0 2023-05-01 11:19:41.479534 PyVecDB-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-01 07:35:27.000000 PyVecDB-0.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:54:32.857917 PyVecDB-0.1.2/
+-rw-rw-rw-   0        0        0     2700 2023-05-04 12:54:32.856918 PyVecDB-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 12:54:32.805644 PyVecDB-0.1.2/PyVecDB.egg-info/
+-rw-rw-rw-   0        0        0     2700 2023-05-04 12:54:32.000000 PyVecDB-0.1.2/PyVecDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-04 12:54:32.000000 PyVecDB-0.1.2/PyVecDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 12:54:32.000000 PyVecDB-0.1.2/PyVecDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-04 12:54:32.000000 PyVecDB-0.1.2/PyVecDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 12:54:32.000000 PyVecDB-0.1.2/PyVecDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1962 2023-05-01 11:28:44.000000 PyVecDB-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 12:54:32.857917 PyVecDB-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      939 2023-05-04 12:54:18.000000 PyVecDB-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:54:32.853917 PyVecDB-0.1.2/src/
+-rw-rw-rw-   0        0        0       29 2023-05-01 07:38:16.000000 PyVecDB-0.1.2/src/__init__.py
+-rw-rw-rw-   0        0        0     1583 2023-05-01 07:47:53.000000 PyVecDB-0.1.2/src/data_object.py
+-rw-rw-rw-   0        0        0      691 2023-05-01 11:34:02.000000 PyVecDB-0.1.2/src/database.py
+-rw-rw-rw-   0        0        0     1746 2023-05-01 11:35:13.000000 PyVecDB-0.1.2/src/stress_test.py
+-rw-rw-rw-   0        0        0     3875 2023-04-30 16:05:40.000000 PyVecDB-0.1.2/src/vector_db.py
+-rw-rw-rw-   0        0        0     5102 2023-05-01 08:46:52.000000 PyVecDB-0.1.2/src/word_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-04 12:54:32.855917 PyVecDB-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:35:27.000000 PyVecDB-0.1.2/tests/__init__.py
```

### Comparing `PyVecDB-0.1.1/PKG-INFO` & `PyVecDB-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVecDB
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for efficient similarity search using high-dimensional vectors.
 Home-page: https://github.com/tyronenorth/PyVecDB
 Author: Your Name
 Author-email: north.tyronejr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -60,15 +60,15 @@
 
 # Search for similar entries
 entries = db.search_entries(vector=entry.vector, num_results=10)
 ```
 
 ## Documentation
 
-For detailed documentation and examples, please visit the [official documentation](https://example.com/docs).
+For detailed documentation and examples, please visit the [official documentation](https://github.com/TyroneNorth/pyvecdb/blob/master/Docs.md).
 
 ## Contributing
 
 Contributions are welcome! Please read our [contributing guidelines](CONTRIBUTING.md) to get started.
 
 ## License
```

### Comparing `PyVecDB-0.1.1/PyVecDB.egg-info/PKG-INFO` & `PyVecDB-0.1.2/PyVecDB.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVecDB
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for efficient similarity search using high-dimensional vectors.
 Home-page: https://github.com/tyronenorth/PyVecDB
 Author: Your Name
 Author-email: north.tyronejr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -60,15 +60,15 @@
 
 # Search for similar entries
 entries = db.search_entries(vector=entry.vector, num_results=10)
 ```
 
 ## Documentation
 
-For detailed documentation and examples, please visit the [official documentation](https://example.com/docs).
+For detailed documentation and examples, please visit the [official documentation](https://github.com/TyroneNorth/pyvecdb/blob/master/Docs.md).
 
 ## Contributing
 
 Contributions are welcome! Please read our [contributing guidelines](CONTRIBUTING.md) to get started.
 
 ## License
```

### Comparing `PyVecDB-0.1.1/README.md` & `PyVecDB-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 # Search for similar entries
 entries = db.search_entries(vector=entry.vector, num_results=10)
 ```
 
 ## Documentation
 
-For detailed documentation and examples, please visit the [official documentation](https://example.com/docs).
+For detailed documentation and examples, please visit the [official documentation](https://github.com/TyroneNorth/pyvecdb/blob/master/Docs.md).
 
 ## Contributing
 
 Contributions are welcome! Please read our [contributing guidelines](CONTRIBUTING.md) to get started.
 
 ## License
```

### Comparing `PyVecDB-0.1.1/setup.py` & `PyVecDB-0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="PyVecDB",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "annoy",
         "msgpack",
-        "sqlite3",
     ],
     author="Your Name",
     author_email="north.tyronejr@gmail.com",
     description="A Python library for efficient similarity search using high-dimensional vectors.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tyronenorth/PyVecDB",
```

### Comparing `PyVecDB-0.1.1/src/data_object.py` & `PyVecDB-0.1.2/src/data_object.py`

 * *Files identical despite different names*

### Comparing `PyVecDB-0.1.1/src/stress_test.py` & `PyVecDB-0.1.2/src/stress_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,7 +43,9 @@
     print(f"Performed {num_searches} similarity searches in {time.time() - search_start_time:.2f} seconds")
 
 if __name__ == "__main__":
     db_path = os.path.join(os.getcwd(), "stress_test.db")
     db = VectorDB(db_path=db_path)
     create_stress_test_table(db)
     stress_test(db, num_entries=100, num_searches=10)
+
+
```

### Comparing `PyVecDB-0.1.1/src/vector_db.py` & `PyVecDB-0.1.2/src/vector_db.py`

 * *Files identical despite different names*

### Comparing `PyVecDB-0.1.1/src/word_generator.py` & `PyVecDB-0.1.2/src/word_generator.py`

 * *Files identical despite different names*

