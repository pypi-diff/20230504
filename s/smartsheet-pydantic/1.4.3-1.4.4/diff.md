# Comparing `tmp/smartsheet-pydantic-1.4.3.tar.gz` & `tmp/smartsheet-pydantic-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsheet-pydantic-1.4.3.tar", last modified: Wed May  3 23:07:24 2023, max compression
+gzip compressed data, was "smartsheet-pydantic-1.4.4.tar", last modified: Thu May  4 18:43:30 2023, max compression
```

## Comparing `smartsheet-pydantic-1.4.3.tar` & `smartsheet-pydantic-1.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/
--rw-rw-r--   0 agile     (1000) agile     (1000)     1091 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/LICENSE
--rw-rw-r--   0 agile     (1000) agile     (1000)     8773 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/PKG-INFO
--rw-rw-r--   0 agile     (1000) agile     (1000)     7123 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/README.md
--rw-rw-r--   0 agile     (1000) agile     (1000)      811 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/pyproject.toml
--rw-rw-r--   0 agile     (1000) agile     (1000)       38 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/setup.cfg
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.507820 smartsheet-pydantic-1.4.3/src/
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.511820 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/
--rw-rw-r--   0 agile     (1000) agile     (1000)        0 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/__init__.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     7623 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/controller.py
--rw-rw-r--   0 agile     (1000) agile     (1000)      493 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/debug_logger.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     2816 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/filters.py
--rw-rw-r--   0 agile     (1000) agile     (1000)    12506 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/smartmodels.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     3087 2023-05-01 22:53:34.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/sources.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     2329 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/transformer.py
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/
--rw-rw-r--   0 agile     (1000) agile     (1000)     8773 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 agile     (1000) agile     (1000)      622 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 agile     (1000) agile     (1000)        1 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 agile     (1000) agile     (1000)      102 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/requires.txt
--rw-rw-r--   0 agile     (1000) agile     (1000)       20 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/top_level.txt
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/tests/
--rw-rw-r--   0 agile     (1000) agile     (1000)     6597 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/tests/test_controller.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     3527 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/tests/test_filters.py
--rw-rw-r--   0 agile     (1000) agile     (1000)    14465 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/tests/test_smartmodel.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     1714 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/tests/test_sources.py
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-04 18:43:30.185801 smartsheet-pydantic-1.4.4/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     1091 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.4/LICENSE
+-rw-rw-r--   0 agile     (1000) agile     (1000)     8773 2023-05-04 18:43:30.185801 smartsheet-pydantic-1.4.4/PKG-INFO
+-rw-rw-r--   0 agile     (1000) agile     (1000)     7123 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.4/README.md
+-rw-rw-r--   0 agile     (1000) agile     (1000)      811 2023-05-04 18:43:16.000000 smartsheet-pydantic-1.4.4/pyproject.toml
+-rw-rw-r--   0 agile     (1000) agile     (1000)       38 2023-05-04 18:43:30.185801 smartsheet-pydantic-1.4.4/setup.cfg
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-04 18:43:30.181801 smartsheet-pydantic-1.4.4/src/
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-04 18:43:30.185801 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/
+-rw-rw-r--   0 agile     (1000) agile     (1000)        0 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/__init__.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     7624 2023-05-04 18:43:16.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/controller.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)      493 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/debug_logger.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     2816 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/filters.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)    12506 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/smartmodels.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     3087 2023-05-01 22:53:34.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/sources.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     2329 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/transformer.py
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-04 18:43:30.185801 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic.egg-info/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     8773 2023-05-04 18:43:30.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 agile     (1000) agile     (1000)      622 2023-05-04 18:43:30.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)        1 2023-05-04 18:43:30.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)      102 2023-05-04 18:43:30.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)       20 2023-05-04 18:43:30.000000 smartsheet-pydantic-1.4.4/src/smartsheet_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-04 18:43:30.185801 smartsheet-pydantic-1.4.4/tests/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     6597 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.4/tests/test_controller.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     3527 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.4/tests/test_filters.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)    14465 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.4/tests/test_smartmodel.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     1714 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.4/tests/test_sources.py
```

### Comparing `smartsheet-pydantic-1.4.3/LICENSE` & `smartsheet-pydantic-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/PKG-INFO` & `smartsheet-pydantic-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.4.3
+Version: 1.4.4
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `smartsheet-pydantic-1.4.3/README.md` & `smartsheet-pydantic-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/pyproject.toml` & `smartsheet-pydantic-1.4.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=67.7.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smartsheet-pydantic"
-version = "1.4.3"
+version = "1.4.4"
 description = "Smartsheet Python SDK and Pydantic Wrapper"
 readme = "README.md"
 authors = [{ name = "Takahiro Watanabe" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/controller.py` & `smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                     subset = dataset[:partition_size]
                     dataset = dataset[partition_size:]
                     add_rows(subset)
                     partition_count += 1
                 else:
                     add_rows(dataset)
                     partition_count += 1
-                    dataset = 0
+                    dataset = []
             logging.info(f"Addition complete in {partition_count} partitions, with each partition size of {partition_size}")
             return {"status_code": 201}
         except Exception as e:
             raise Exception(f"Row addition failed {e}")
 
     @debug_logger
     def update_rows(self, dataset: set[SmartModel]) -> dict[str: int]:
```

### Comparing `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/filters.py` & `smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/smartmodels.py` & `smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/smartmodels.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/sources.py` & `smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/sources.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/transformer.py` & `smartsheet-pydantic-1.4.4/src/smartsheet_pydantic/transformer.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/PKG-INFO` & `smartsheet-pydantic-1.4.4/src/smartsheet_pydantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.4.3
+Version: 1.4.4
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/SOURCES.txt` & `smartsheet-pydantic-1.4.4/src/smartsheet_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/tests/test_controller.py` & `smartsheet-pydantic-1.4.4/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/tests/test_filters.py` & `smartsheet-pydantic-1.4.4/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/tests/test_smartmodel.py` & `smartsheet-pydantic-1.4.4/tests/test_smartmodel.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.3/tests/test_sources.py` & `smartsheet-pydantic-1.4.4/tests/test_sources.py`

 * *Files identical despite different names*

