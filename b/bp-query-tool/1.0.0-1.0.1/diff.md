# Comparing `tmp/bp_query_tool-1.0.0.tar.gz` & `tmp/bp_query_tool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_query_tool-1.0.0.tar", last modified: Thu May  4 05:55:16 2023, max compression
+gzip compressed data, was "bp_query_tool-1.0.1.tar", last modified: Thu May  4 07:40:43 2023, max compression
```

## Comparing `bp_query_tool-1.0.0.tar` & `bp_query_tool-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 05:55:16.651220 bp_query_tool-1.0.0/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-1.0.0/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-1.0.0/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3668 2023-05-04 05:55:16.650358 bp_query_tool-1.0.0/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 05:55:16.634224 bp_query_tool-1.0.0/bp_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3668 2023-05-04 05:55:16.000000 bp_query_tool-1.0.0/bp_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-05-04 05:55:16.000000 bp_query_tool-1.0.0/bp_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-04 05:55:16.000000 bp_query_tool-1.0.0/bp_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-04 05:55:16.000000 bp_query_tool-1.0.0/bp_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-05-04 05:55:16.000000 bp_query_tool-1.0.0/bp_query_tool.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 05:55:16.634852 bp_query_tool-1.0.0/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 bp_query_tool-1.0.0/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 05:55:16.628616 bp_query_tool-1.0.0/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 05:55:16.636438 bp_query_tool-1.0.0/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 05:55:16.638176 bp_query_tool-1.0.0/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-26 07:58:40.000000 bp_query_tool-1.0.0/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1032251 2023-04-26 07:58:40.000000 bp_query_tool-1.0.0/query_tool/frontend/dist/assets/index-ec348719.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      568 2023-04-26 08:38:09.000000 bp_query_tool-1.0.0/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-26 07:58:39.000000 bp_query_tool-1.0.0/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 05:55:16.649435 bp_query_tool-1.0.0/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-1.0.0/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 bp_query_tool-1.0.0/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-1.0.0/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3839 2023-04-26 08:59:45.000000 bp_query_tool-1.0.0/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-1.0.0/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 bp_query_tool-1.0.0/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-1.0.0/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-04 05:55:16.651409 bp_query_tool-1.0.0/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      790 2023-05-04 05:54:56.000000 bp_query_tool-1.0.0/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:40:43.384341 bp_query_tool-1.0.1/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-1.0.1/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-1.0.1/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3668 2023-05-04 07:40:43.383849 bp_query_tool-1.0.1/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:40:43.365839 bp_query_tool-1.0.1/bp_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3668 2023-05-04 07:40:43.000000 bp_query_tool-1.0.1/bp_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-05-04 07:40:43.000000 bp_query_tool-1.0.1/bp_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-04 07:40:43.000000 bp_query_tool-1.0.1/bp_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-04 07:40:43.000000 bp_query_tool-1.0.1/bp_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-05-04 07:40:43.000000 bp_query_tool-1.0.1/bp_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:40:43.366519 bp_query_tool-1.0.1/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 bp_query_tool-1.0.1/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:40:43.361068 bp_query_tool-1.0.1/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:40:43.367730 bp_query_tool-1.0.1/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:40:43.369351 bp_query_tool-1.0.1/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-26 07:58:40.000000 bp_query_tool-1.0.1/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1032251 2023-04-26 07:58:40.000000 bp_query_tool-1.0.1/query_tool/frontend/dist/assets/index-ec348719.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      568 2023-04-26 08:38:09.000000 bp_query_tool-1.0.1/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-26 07:58:39.000000 bp_query_tool-1.0.1/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:40:43.382529 bp_query_tool-1.0.1/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-1.0.1/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1661 2023-05-04 07:12:03.000000 bp_query_tool-1.0.1/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-1.0.1/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3839 2023-04-26 08:59:45.000000 bp_query_tool-1.0.1/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-1.0.1/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2414 2023-05-04 07:36:07.000000 bp_query_tool-1.0.1/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-1.0.1/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-04 07:40:43.384492 bp_query_tool-1.0.1/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      790 2023-05-04 07:40:41.000000 bp_query_tool-1.0.1/setup.py
```

### Comparing `bp_query_tool-1.0.0/LICENSE` & `bp_query_tool-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.0/PKG-INFO` & `bp_query_tool-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp_query_tool
-Version: 1.0.0
+Version: 1.0.1
 Summary: Query tool to generate query from selection
 Home-page: UNKNOWN
 Author: Bluepinapple
 Author-email: vivek.sthul@bluepinapple.com
 License: UNKNOWN
 Description: # Query Tool
```

### Comparing `bp_query_tool-1.0.0/bp_query_tool.egg-info/PKG-INFO` & `bp_query_tool-1.0.1/bp_query_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp-query-tool
-Version: 1.0.0
+Version: 1.0.1
 Summary: Query tool to generate query from selection
 Home-page: UNKNOWN
 Author: Bluepinapple
 Author-email: vivek.sthul@bluepinapple.com
 License: UNKNOWN
 Description: # Query Tool
```

### Comparing `bp_query_tool-1.0.0/bp_query_tool.egg-info/SOURCES.txt` & `bp_query_tool-1.0.1/bp_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.0/query_tool/__init__.py` & `bp_query_tool-1.0.1/query_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.0/query_tool/frontend/dist/assets/index-ec348719.js` & `bp_query_tool-1.0.1/query_tool/frontend/dist/assets/index-ec348719.js`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.0/query_tool/frontend/dist/index.html` & `bp_query_tool-1.0.1/query_tool/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.0/query_tool/frontend/dist/vite.svg` & `bp_query_tool-1.0.1/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.0/query_tool/services/dimension_service.py` & `bp_query_tool-1.0.1/query_tool/services/dimension_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import List
 
 
 class DimensionService:
     def __init__(self):
         self.dimensions = []
         self.measures = []
+        self.measure_columns = []
 
     def get_dimension_query(self, dimensions: List = None, table_aliases: dict = {}):
         if dimensions is not None:
             for dimension in dimensions:
                 self.__get_dimension(dimension, table_aliases)
-        return self.dimensions, self.measures
+        return self.dimensions, self.measures, self.measure_columns
 
     def __get_dimension(self, dimension, table_aliases):
         if dimension.get("dimension", "") == "GROUP BY":
             self.dimensions.append(
                 "{0}.{1}".format(
                     table_aliases.get(
                         f"{dimension.get('database')}.{dimension.get('table')}",
@@ -34,7 +35,12 @@
         if measure is not None:
             table, column = measure.get("fqcn", "").rsplit(".", 1)
             self.measures.append(
                 "{0}({1}.{2})".format(
                     measure.get("measure"), table_aliases.get(table, table), column
                 )
             )
+            self.measure_columns.append(
+                "{0}.{1}".format(
+                    table_aliases.get(table, table), column
+                )
+            )
```

### Comparing `bp_query_tool-1.0.0/query_tool/services/entities_service.py` & `bp_query_tool-1.0.1/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.0/query_tool/services/filters_service.py` & `bp_query_tool-1.0.1/query_tool/services/filters_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.0/query_tool/services/query_tool_service.py` & `bp_query_tool-1.0.1/query_tool/services/query_tool_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,40 +10,47 @@
             entities_tables_with_aliases,
             relations,
             table_aliases,
         ) = self.__entities_cls.get_entities(query_json.get("entity_data"))
         filters = self.__filters_cls.get_filter_query(
             query_json.get("filter_data"), table_aliases
         )
-        dimensions, measures = self.__dimesion_cls.get_dimension_query(
+        dimensions, measures, measure_columns = self.__dimesion_cls.get_dimension_query(
             query_json.get("dimension_data"), table_aliases
         )
         return self.__get_query(
             entities_columns,
             relations,
             filters,
             dimensions,
             measures,
             entities_tables_with_aliases,
+            measure_columns
         )
 
     def __get_query(
         self,
         entities_columns,
         relations,
         filters,
         dimensions,
         measures,
         entities_tables_with_aliases,
+        measure_columns
     ) -> str:
         sql_array = ["SELECT"]
         select_query = ""
 
         if len(entities_columns) > 0:
-            select_query += ", ".join(entities_columns)
+            # Check select columns are in group by clause or in aggregate columns list
+            if len(dimensions) > 0:
+                select_columns = [select_column for select_column in entities_columns if select_column in dimensions or select_column in measure_columns]
+                select_query += ", ".join(select_columns)
+            else: 
+                select_query += ", ".join(entities_columns)
 
         if len(measures) > 0:
             select_query = f"{select_query}, " if select_query else select_query
             select_query += ", ".join(measures)
 
         sql_array.append(select_query)
```

### Comparing `bp_query_tool-1.0.0/query_tool/services/register.py` & `bp_query_tool-1.0.1/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-1.0.0/setup.py` & `bp_query_tool-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp_query_tool",
-    version="1.0.0",
+    version="1.0.1",
     author="Bluepinapple",
     author_email="vivek.sthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

