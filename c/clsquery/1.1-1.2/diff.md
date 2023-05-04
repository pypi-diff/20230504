# Comparing `tmp/clsquery-1.1.tar.gz` & `tmp/clsquery-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\mzfg28\OneDrive - General Motors\Work\2nd Rotation\clsquery\dist\.tmp-1z127epu\clsquery-1.1.tar", last modified: Wed May  3 20:33:06 2023, max compression
+gzip compressed data, was "C:\Users\mzfg28\OneDrive - General Motors\Work\2nd Rotation\clsquery\dist\.tmp-l7xph2gc\clsquery-1.2.tar", last modified: Thu May  4 20:29:58 2023, max compression
```

## Comparing `clsquery-1.1.tar` & `clsquery-1.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 20:33:06.000000 clsquery-1.1/
--rw-rw-rw-   0        0        0     1068 2023-05-03 13:25:17.000000 clsquery-1.1/LICENSE
--rw-rw-rw-   0        0        0     5462 2023-05-03 20:33:06.000000 clsquery-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4828 2023-05-03 20:21:43.000000 clsquery-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 20:33:06.000000 clsquery-1.1/clsquery/
--rw-rw-rw-   0        0        0      871 2023-05-03 20:27:23.000000 clsquery-1.1/clsquery/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:33:06.000000 clsquery-1.1/clsquery/classes/
--rw-rw-rw-   0        0        0     1723 2023-05-03 16:16:09.000000 clsquery-1.1/clsquery/classes/class_query.py
--rw-rw-rw-   0        0        0      261 2023-05-03 19:56:36.000000 clsquery-1.1/clsquery/classes/class_query_formatter.py
--rw-rw-rw-   0        0        0      366 2023-05-03 20:18:53.000000 clsquery-1.1/clsquery/classes/class_query_item.py
--rw-rw-rw-   0        0        0      517 2023-05-03 20:06:24.000000 clsquery-1.1/clsquery/classes/class_query_results.py
--rw-rw-rw-   0        0        0     1810 2023-05-03 13:55:45.000000 clsquery-1.1/clsquery/cli.py
--rw-rw-rw-   0        0        0      233 2023-05-03 15:57:27.000000 clsquery-1.1/clsquery/constants.py
--rw-rw-rw-   0        0        0      662 2023-05-02 18:23:09.000000 clsquery-1.1/clsquery/convert_classes_to_table.py
--rw-rw-rw-   0        0        0     1596 2023-05-02 17:44:29.000000 clsquery-1.1/clsquery/custom_logger.py
--rw-rw-rw-   0        0        0     2176 2023-05-03 20:11:19.000000 clsquery-1.1/clsquery/default_formatter.py
--rw-rw-rw-   0        0        0      356 2023-05-02 21:34:29.000000 clsquery-1.1/clsquery/filter_by_types.py
--rw-rw-rw-   0        0        0      467 2023-05-02 17:50:57.000000 clsquery-1.1/clsquery/format_list.py
--rw-rw-rw-   0        0        0     1023 2023-05-02 17:47:40.000000 clsquery-1.1/clsquery/format_table.py
--rw-rw-rw-   0        0        0     4433 2023-05-03 20:27:52.000000 clsquery-1.1/clsquery/get_classes_from_paths.py
--rw-rw-rw-   0        0        0      184 2023-05-03 15:01:57.000000 clsquery-1.1/clsquery/get_time.py
--rw-rw-rw-   0        0        0      625 2023-05-02 17:27:34.000000 clsquery-1.1/clsquery/has_supertype.py
--rw-rw-rw-   0        0        0     4456 2023-05-03 20:15:45.000000 clsquery-1.1/clsquery/query.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:33:06.000000 clsquery-1.1/clsquery.egg-info/
--rw-rw-rw-   0        0        0     5462 2023-05-03 20:33:06.000000 clsquery-1.1/clsquery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      691 2023-05-03 20:33:06.000000 clsquery-1.1/clsquery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 20:33:06.000000 clsquery-1.1/clsquery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 20:33:06.000000 clsquery-1.1/clsquery.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 20:33:06.000000 clsquery-1.1/clsquery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      735 2023-05-03 20:32:31.000000 clsquery-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 20:33:06.000000 clsquery-1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 20:33:06.000000 clsquery-1.1/tests/
--rw-rw-rw-   0        0        0     1635 2023-05-03 20:29:17.000000 clsquery-1.1/tests/test_query.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:58.000000 clsquery-1.2/
+-rw-rw-rw-   0        0        0     1068 2023-05-03 13:25:17.000000 clsquery-1.2/LICENSE
+-rw-rw-rw-   0        0        0     7466 2023-05-04 20:29:58.000000 clsquery-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6832 2023-05-04 20:29:10.000000 clsquery-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:58.000000 clsquery-1.2/clsquery/
+-rw-rw-rw-   0        0        0      871 2023-05-03 20:27:23.000000 clsquery-1.2/clsquery/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:58.000000 clsquery-1.2/clsquery/classes/
+-rw-rw-rw-   0        0        0     3011 2023-05-04 20:15:23.000000 clsquery-1.2/clsquery/classes/class_query.py
+-rw-rw-rw-   0        0        0      261 2023-05-03 19:56:36.000000 clsquery-1.2/clsquery/classes/class_query_formatter.py
+-rw-rw-rw-   0        0        0      366 2023-05-03 20:18:53.000000 clsquery-1.2/clsquery/classes/class_query_item.py
+-rw-rw-rw-   0        0        0      517 2023-05-03 20:06:24.000000 clsquery-1.2/clsquery/classes/class_query_results.py
+-rw-rw-rw-   0        0        0     1872 2023-05-04 20:24:53.000000 clsquery-1.2/clsquery/cli.py
+-rw-rw-rw-   0        0        0      233 2023-05-03 15:57:27.000000 clsquery-1.2/clsquery/constants.py
+-rw-rw-rw-   0        0        0      715 2023-05-04 19:30:43.000000 clsquery-1.2/clsquery/convert_classes_to_table.py
+-rw-rw-rw-   0        0        0     1715 2023-05-04 18:31:13.000000 clsquery-1.2/clsquery/custom_logger.py
+-rw-rw-rw-   0        0        0     2353 2023-05-04 20:18:43.000000 clsquery-1.2/clsquery/default_formatter.py
+-rw-rw-rw-   0        0        0      356 2023-05-02 21:34:29.000000 clsquery-1.2/clsquery/filter_by_types.py
+-rw-rw-rw-   0        0        0      467 2023-05-02 17:50:57.000000 clsquery-1.2/clsquery/format_list.py
+-rw-rw-rw-   0        0        0     1029 2023-05-04 19:30:50.000000 clsquery-1.2/clsquery/format_table.py
+-rw-rw-rw-   0        0        0     2231 2023-05-04 16:16:03.000000 clsquery-1.2/clsquery/get_classes_at_path.py
+-rw-rw-rw-   0        0        0     3644 2023-05-04 18:54:02.000000 clsquery-1.2/clsquery/get_classes_from_paths.py
+-rw-rw-rw-   0        0        0      184 2023-05-03 15:01:57.000000 clsquery-1.2/clsquery/get_time.py
+-rw-rw-rw-   0        0        0      625 2023-05-02 17:27:34.000000 clsquery-1.2/clsquery/has_supertype.py
+-rw-rw-rw-   0        0        0     5795 2023-05-04 19:58:13.000000 clsquery-1.2/clsquery/query.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:58.000000 clsquery-1.2/clsquery.egg-info/
+-rw-rw-rw-   0        0        0     7466 2023-05-04 20:29:58.000000 clsquery-1.2/clsquery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-05-04 20:29:58.000000 clsquery-1.2/clsquery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 20:29:58.000000 clsquery-1.2/clsquery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-04 20:29:58.000000 clsquery-1.2/clsquery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-04 20:29:58.000000 clsquery-1.2/clsquery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      735 2023-05-04 19:34:52.000000 clsquery-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 20:29:58.000000 clsquery-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 20:29:58.000000 clsquery-1.2/tests/
+-rw-rw-rw-   0        0        0     2842 2023-05-04 19:43:48.000000 clsquery-1.2/tests/test_query.py
```

### Comparing `clsquery-1.1/LICENSE` & `clsquery-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clsquery-1.1/PKG-INFO` & `clsquery-1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,130 @@
-Metadata-Version: 2.1
-Name: clsquery
-Version: 1.1
-Summary: A package for querying Python classes
-Author-email: Kenneth Mead <kennethmead784@gmail.com>
-Project-URL: Homepage, https://github.com/Xerner/python-class-query
-Classifier: Programming Language :: Python :: 3
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python Class Query <!-- omit from toc -->
 
-A package for querying Python classes
+`clsquery` is a searching tool implemented to help developers query classes available in files and folders for viewing or for use during runtime. Only classes defined in the files being searched are included. Imported classes are ignored.
 
-- [Todo](#todo)
+- [Installation](#installation)
 - [Usage](#usage)
   - [Python](#python)
   - [Command Line](#command-line)
 - [Examples](#examples)
   - [Basic Search](#basic-search)
   - [With a tag filter and additional attributes](#with-a-tag-filter-and-additional-attributes)
   - [With grouping](#with-grouping)
-  - [With presets](#with-presets)
 
-## Todo
+**Todo**
 
-- Add a way to distinguish classes with the same name that come from difference sources
 - Make use of different log levels
 
+## Installation
+
+```bash
+python -m pip install clsquery
+```
+
 ## Usage
 
 ### Python
 
-TODO
+Simple query that finds any Python Class and prints results to console
+
+```python
+import clsquery
+
+results = clsquery.query("/path/to/classes", log_results=True)
+```
+
+Simple query that finds any Python Class that inherits from `MyParentClass` and prints results to console
+
+```python
+import clsquery
+
+results = clsquery.query("/path/to/classes", "MyParentClass", log_results=True)
+```
+
+Reusing a saved query
+
+```python
+import clsquery
+
+saved_query = clsquery.ClassQuery("/path/to/classes", "MyParentClass")
+results = saved_query.query(log_results=True)
+# or
+results = clsquery.query(query=saved_query, log_results=True)
+```
+
+Overriding an attribute of a saved query
+
+```python
+import clsquery
+
+saved_query = clsquery.ClassQuery("/path/to/classes", "MyParentClass")
+results = saved_query.query(paths="/different/path/to/classes", log_results=True)
+```
+
+A query that will find all Python Classes in each module found at the path provided that
+- Inherits from `MyParentClass`
+- has an attribute `tags` that is a list containing the value `"snake"`
+- has an attribute `tags` that is a list that **does not** contain the value `"wolverine"`
+
+And, using the default formatter, will print each class grouped by the module it came from and display its name and docstring in a table-like format
+
+```python
+import clsquery
+
+results = clsquery.query(paths="/path/to/classes", 
+                         supertypes="MyParentClass",
+                         tags=["snake", "_wolverine"],
+                         attributes=["__name__", "__doc__"],
+                         group_by="__module__")
+```
+
+> Prefix tags with a _ (underscore) to specify they should NOT be included
+
+A recursive search that will look in all folders and modules under the paths provided
+
+```python
+import clsquery
+
+results = clsquery.query("/path/to/parent/folder", recursive=True, log_results=True)
+```
 
 ### Command Line
 
+Help dialog
+
 ```
-usage: python list.py --path STRING
- 
-A search command for Python classes
- 
+usage: python -m clsquery.cli.py --path STRING
+
+A query command for Python classes
+
 optional arguments:
   -h, --help            show this help message and exit
   -p [STRING [STRING ...]], --paths [STRING [STRING ...]]
-                        directory path or filepath to the classes to generate docs for
+                        directory path or filepath to the classes to generate
+                        docs for
   -t [STRING [STRING ...]], --tags [STRING [STRING ...]]
-                        the tags to look for when including classes. A class must have a 'tags' attribute for this to work. Prefix tags with '_' to specify they should NOT be included
+                        the tags to look for when including classes. A class
+                        must have a 'tags' attribute for this to work. Prefix
+                        tags with '_' to specify they should NOT be included
   -s [STRING [STRING ...]], --supertypes [STRING [STRING ...]]
                         The supertypes to look for when including classes
   -a [STRING [STRING ...]], --attributes [STRING [STRING ...]]
                         What attributes of the class to return
   -g [STRING [STRING ...]], --group-by [STRING [STRING ...]]
                         What attribute to group the classes by
-  -l PRESET, --load-preset PRESET
-                        load a preset list of args
- 
-Options provided on the command line will override options loaded by a preset
+  -r, --recursive       Whether or not a recursive search should be done on
+                        each path in 'paths'
 ```
 
-The list command is a generic python class searching tool implemented to help users discover topic, metric, and requirement classes available. Only classes defined in the files being searched are included. Imported classes are ignored.
-
-It returns a format similar to below
+Queries are, by default, formatted by an internal formatter function with results similar to the below
 
 ```
 # Input
-list.py -p "path/to/classes1" "path/to/classes2" -t Tag1 Tag2 _Tag3 -s ParentClass1 ParentClass2 -a __name__ tags <other attributes>
+python -m clsquery.cli -p "path/to/classes1" "path/to/classes2" -t Tag1 Tag2 _Tag3 -s ParentClass1 ParentClass2 -a __name__ tags <other attributes>
  
 # Output
 Search Results
 ---------------
  
 Date:              2022-12-07 10:10:26
 Paths:            
@@ -96,15 +145,15 @@
 
 ## Examples
 
 ### Basic Search
 
 ```
 # Input
-list -p /path/to/classes
+python -m clsquery.cli -p /path/to/classes
  
 # Output
 Search Results
 ---------------
  
 Date:              2022-12-07 14:06:31
 Paths:            
@@ -125,15 +174,15 @@
 
 Notice
 - `_special` was supplied as a parameter to exclude `ASpecialClass` which contained `special` in its tags attribute
 - `__doc__` is allowed. References to any class attribute is allowed, as long as it can be turned into a string
 
 ```
 # Input
-list -p /path/to/classes --tags _avoid_me -a __name__ __doc__
+python -m clsquery.cli -p /path/to/classes --tags _avoid_me -a __name__ __doc__
  
 # Output
 Search Results
 ---------------
  
 Date:              2022-12-07 14:54:52
 Paths:            
@@ -152,15 +201,15 @@
 Below is assuming the `ASpecialClass` class has an attribute `is_special` with the value `True`, and `SomeClass` has the same attribute with the value `False`
 
 Notice
 - It is possible to have multiple levels of grouping
 
 ```
 # Input
-list -p /path/to/classes -g __base__.__name__ is_special  
+python -m clsquery.cli -p /path/to/classes -g __base__.__name__ is_special  
  
 # Output
 Search Results
 ---------------
  
 Date:              2022-12-07 17:21:36
 Paths:            
@@ -180,11 +229,7 @@
  
     False
  
         __name__         
         ------------------
         ASpecialClass
 ```
-
-### With presets
-
-TODO
```

### Comparing `clsquery-1.1/clsquery/__init__.py` & `clsquery-1.2/clsquery/__init__.py`

 * *Files identical despite different names*

### Comparing `clsquery-1.1/clsquery/classes/class_query.py` & `clsquery-1.2/clsquery/classes/class_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,65 @@
-from typing import List, TYPE_CHECKING
+from typing import List, TYPE_CHECKING, Union
 if TYPE_CHECKING:
-    from clsquery import ClassQueryFormatter    
+    from clsquery import ClassQueryFormatter
 from clsquery import default_formatter, AVOID_TAG_STR
 
 
 class ClassQuery:
     def __init__(self, 
                  paths: List[str], 
                  supertypes: List[str] = None, 
                  tags: List[str] = None, 
                  attributes: List[str] = ["__name__"], 
                  group_by: List[str] = None, 
+                 recursive = False,
                  formatter: 'ClassQueryFormatter' = default_formatter,
                  avoid_tag_str = AVOID_TAG_STR):
         """
         - `paths` A list of file and/or directory paths
         - `supertypes` A list of parent types to limit the search to
         - `tags` A list of tags to limit the search to. This is assuming classes found have a global attribute `tags`
         - `attributes` A list of attributes to be printed for each class found
         - `group_by` A list of attributes to group the found classes by
         - `formatter` A function that takes in query results, and a few other args, and returns a str to be printed and returned by this function
-        
-            Default: default_formatter
+
+            Default: clsquery.default_formatter
         - `avoid_tag_str` A string that if found prefixing a tag, the search will avoid the tag rather than include it
 
             Default: '_'
+        - `query` A ClassQuery instance. Other provided args will override the args in the query instance
+        - `recursive` Whether or not a recursive search should be done on each path in `paths`
+            
+            Default: False
+        - `log_results` Whether or not the query results should be logged to the console using the str returned from `formatter`
+
+            Default: False
         """
         self.paths = paths
         self.supertypes = supertypes
         self.tags = tags
         self.attributes = attributes
         self.group_by = group_by
+        self.recursive = recursive
         self.formatter = formatter
         self.avoid_tag_str = avoid_tag_str
 
-    def query(self, log_results=False):
+    def query(self, 
+              paths: Union['ClassQuery', str, List[str]] = None, 
+              supertypes: Union[str, List[str]] = None, 
+              tags: Union[str, List[str]] = None, 
+              attributes: Union[str, List[str]] = ["__name__"], 
+              group_by: Union[str, List[str]] = None, 
+              formatter: 'ClassQueryFormatter' = None,
+              avoid_tag_str = None,
+              recursive: bool = None,log_results=False):
         from clsquery import query as query_
-        query_(query=self, log_results=log_results)
+        return query_(paths=paths,
+                      supertypes=supertypes,
+                      tags=tags,
+                      attributes=attributes,
+                      group_by=group_by,
+                      formatter=formatter,
+                      avoid_tag_str=avoid_tag_str,
+                      query=self, 
+                      recursive=recursive,
+                      log_results=log_results)
```

### Comparing `clsquery-1.1/clsquery/classes/class_query_results.py` & `clsquery-1.2/clsquery/classes/class_query_results.py`

 * *Files identical despite different names*

### Comparing `clsquery-1.1/clsquery/cli.py` & `clsquery-1.2/clsquery/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import argparse
 import json
 from pathlib import Path
 from clsquery import query, AVOID_TAG_STR
 
 def cli():
     """
-    run `cli.py -h` for help
+    run `python -m clsquery.cli -h` for help
 
     Note: Custom formatting is only supported when calling the query function directly from a script
     """
-    usage = f"""python {Path(__file__).name} --path STRING
+    usage = f"""python -m clsquery.{Path(__file__).name} --path STRING
 
 A query command for Python classes
 
 """
-    epilog = "Options provided on the command line will override options loaded by a saved query"
-    parser = argparse.ArgumentParser(usage=usage, epilog=epilog, formatter_class=argparse.RawDescriptionHelpFormatter)
+    parser = argparse.ArgumentParser(usage=usage, formatter_class=argparse.RawDescriptionHelpFormatter)
     mutex = parser.add_mutually_exclusive_group(required=True)
     mutex.add_argument('-p', '--paths', metavar="STRING", type=str, nargs="*", help='directory path or filepath to the classes to generate docs for')
     parser.add_argument('-t', '--tags', metavar="STRING", type=str, nargs="*", help=f"the tags to look for when including classes. A class must have a 'tags' attribute for this to work. Prefix tags with '{AVOID_TAG_STR}' to specify they should NOT be included")
     parser.add_argument('-s', '--supertypes', metavar="STRING", type=str, nargs="*", help="The supertypes to look for when including classes")
     parser.add_argument('-a', '--attributes', metavar="STRING", type=str, nargs="*", default=["__name__"], help="What attributes of the class to return")
-    # parser.add_argument('-g', '--group-by', metavar="STRING", type=str, nargs="?", default="", const="", help="What attribute to group the classes by")
     parser.add_argument('-g', '--group-by', metavar="STRING", type=str, nargs="*", help="What attribute to group the classes by")
+    parser.add_argument('-r', '--recursive', action="store_true", help="Whether or not a recursive search should be done on each path in 'paths'")
     args = parser.parse_args()
-
-    query(args.paths, args.supertypes, args.tags, args.attributes, args.group_by)
+    query(paths=args.paths, 
+          supertypes=args.supertypes, 
+          tags=args.tags, 
+          attributes=args.attributes, 
+          group_by=args.group_by, 
+          recursive=args.recursive,
+          log_results=True)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `clsquery-1.1/clsquery/custom_logger.py` & `clsquery-1.2/clsquery/custom_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,19 +29,21 @@
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt)
         return formatter.format(record)
 
 # Create custom logger logging all five levels
 logger = logging.getLogger(LOGGER_NAME)
-logger.setLevel(logging.DEBUG)
 
-# Define format for logs
-fmt = '%(levelname)8s | %(message)s'
+if logging.StreamHandler not in [type(handler) for handler in logger.handlers]:
+    logger.setLevel(logging.DEBUG)
 
-# Create stdout handler for logging to the console (logs all five levels)
-stdout_handler = logging.StreamHandler()
-stdout_handler.setLevel(logging.DEBUG)
-stdout_handler.setFormatter(CustomFormatter(fmt))
+    # Define format for logs
+    fmt = '%(levelname)8s | %(message)s'
 
-# Add both handlers to the logger
-logger.addHandler(stdout_handler)
+    # Create stdout handler for logging to the console (logs all five levels)
+    stdout_handler = logging.StreamHandler()
+    stdout_handler.setLevel(logging.DEBUG)
+    stdout_handler.setFormatter(CustomFormatter(fmt))
+
+    # Add both handlers to the logger
+    logger.addHandler(stdout_handler)
```

### Comparing `clsquery-1.1/clsquery/default_formatter.py` & `clsquery-1.2/clsquery/default_formatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,22 +17,24 @@
         str_ = ""
         for group in classes_or_groups:
             str_ += ("\t"*indent) + group + "\n\n" + grouped_formatting(classes_or_groups[group], attributes, indent=indent+1)
         return str_
 
     is_grouped = results.groups is not None and type(results.groups) != list and results.query.group_by is not None and len(results.query.group_by) != 0
     lines = []
+    lines.append("Logging results with default formatter")
     lines.append("")
     lines.append("Search Results")
     lines.append("---------------")
     lines.append("")
-    lines.append(f"Date:              {get_time()}")
-    lines.append("Paths:             " + format_list(results.query.paths, is_long_format=True))
-    lines.append("Supertypes filter: " + format_list(results.query.supertypes))
-    lines.append("Tag filter:        " + format_list(results.query.tags))
+    lines.append("{: <20}{}".format("Date", get_time()))
+    lines.append("{: <20}{}".format("Paths", format_list(results.query.paths, is_long_format=True)))
+    lines.append("{: <20}{}".format("Recursive", str(results.query.recursive)))
+    lines.append("{: <20}{}".format("Supertypes filter", format_list(results.query.supertypes)))
+    lines.append("{: <20}{}".format("Tag filter", format_list(results.query.tags)))
     if results.query.group_by is not None:
         lines.append(f"Grouped by:        {format_list(results.query.group_by)}")
     lines.append("")
 
     # grouped formatting
     if is_grouped:
         lines.append(grouped_formatting(results.groups, results.query.attributes, indent))
```

### Comparing `clsquery-1.1/clsquery/format_table.py` & `clsquery-1.2/clsquery/format_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 def format_table(values: list, indent = 0, margin = 4, has_headers = True) -> str:
     table = []
     if len(values) == 0:
         return "No values"
+    
     format_str = []
     for row in values:
         if type(row) == tuple:
             row = list(row)
         if type(row) == list and len(row) > len(format_str):
             format_str = [0] * len(row)
         row_str = []
```

### Comparing `clsquery-1.1/clsquery/get_classes_from_paths.py` & `clsquery-1.2/clsquery/get_classes_from_paths.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,73 @@
 import os
-import inspect
-import importlib
-import sys
 from glob import glob
+from pathlib import Path
 from typing import List
 from clsquery.classes.class_query_item import ClassQueryItem
-from clsquery.has_supertype import has_supertype
 from clsquery.constants import AVOID_TAG_STR
+from clsquery.get_classes_at_path import get_classes_in_module
+from clsquery.format_list import format_list
+from clsquery.custom_logger import logger
 
 
-def get_classes_from_paths(file_or_dir_paths: List[str], supertype_filter: List[str] = [], tag_filter: List[str] = [], avoid_tag_str = AVOID_TAG_STR):
+def get_classes_from_paths(file_or_dir_paths: List[str], 
+                           supertype_filter: List[str] = [], 
+                           tag_filter: List[str] = [],
+                           avoid_tag_str = AVOID_TAG_STR,
+                           recursive=False):
     # https://docs.python.org/3/library/importlib.html#importing-a-source-file-directly
     # https://stackoverflow.com/questions/3178285/list-classes-in-directory-python
-    
-    classes: List[ClassQueryItem] = []
-
-    def remove_avoid_tag_str(tag: str):
-        if should_avoid_tag(tag):
-            return tag[1:]
-
-    def should_avoid_tag(tag: str) -> bool:
-        return tag[0] == avoid_tag_str
-
-    def find_classes(path: str, supertypes: List[str] = [], tag_filter: List[str] = []) -> List[ClassQueryItem]:
-        def filter_classes(cls: object, supertypes: List[str] = [], tag_filter: List[str] = []):
-            if not inspect.isclass(cls) or cls.__module__ != name:
-                return False
-
-            has_tag = True
-            if tag_filter is not None and len(tag_filter) > 0:
-                has_tag = False
-                if hasattr(cls, "tags"):
-                    for tag in tag_filter:
-                        if should_avoid_tag(tag):
-                            if remove_avoid_tag_str(tag) in cls.tags:
-                                return False
-                            else:
-                                has_tag = True
-                        else:
-                            if tag in cls.tags:
-                                has_tag = True
-                                break
-                            else:
-                                has_tag = False
-
-            if supertypes is None or len(supertypes) == 0:
-                valid_supertype = True
-            else:
-                valid_supertype = any([has_supertype(cls, supertype) for supertype in supertypes])
-
-            return has_tag and valid_supertype
-        
-        name = os.path.splitext(os.path.basename(path))[0]
-        spec = importlib.util.spec_from_file_location(name,path)
-        module = importlib.util.module_from_spec(spec)
-        sys.modules[name] = module
-        spec.loader.exec_module(module)
-        classes: List[ClassQueryItem] = []
-        for _, cls in inspect.getmembers(module, lambda cls: filter_classes(cls, supertypes, tag_filter)):
-            classes.append(ClassQueryItem(cls, path))
-        return classes
-
-    def find_and_extend_classes(classes: List[ClassQueryItem], file_or_dir_path: str, type_filter: List[str], tag_filter: List[str] = []):
-        query_result = find_classes(file_or_dir_path, type_filter, tag_filter)
+    def find_and_extend_classes(classes: List[ClassQueryItem], file_or_dir_path: str, type_filter: List[str], tag_filter: List[str] = [], avoid_tag_str = AVOID_TAG_STR):
+        query_result = get_classes_in_module(file_or_dir_path, type_filter, tag_filter, avoid_tag_str)
         for query_item in query_result:
             if query_item in classes:
                 continue
             classes.append(query_item)
 
-        if len(classes) == 0:
-            log_func = print # used to be a warning
+        if len(query_result) == 0:
+            log_func = logger.warning # used to be a warning
         else:
-            log_func = print # used to be a success
+            log_func = logger.info # used to be a success
         
         if len(query_result) == 1:
             log_func(f"Fetched {len(query_result)} class from {file_or_dir_path}")
         else:
             log_func(f"Fetched {len(query_result)} classes from {file_or_dir_path}")
+        if len(query_result) > 0:
+            long_format = len(query_result) > 1
+            logger.info(f"Classes fetched: " + format_list([item.cls.__name__ for item in query_result], is_long_format=long_format))
     
-    print("Fetching classes...")
-    print("Paths to search:  " + str(file_or_dir_paths))
-    print("Supertype filter: " + str(supertype_filter))
-    print("Tag filter:       " + str(tag_filter))
+    classes: List[ClassQueryItem] = []
+
+    logger.info("Fetching classes...")
+    logger.info("Paths to search:  " + format_list(file_or_dir_paths, is_long_format=True))
+    logger.info("Recursive:        " + str(recursive))
+    logger.info("Supertype filter: " + format_list(supertype_filter))
+    logger.info("Tag filter:       " + format_list(tag_filter))
 
     for file_or_dir_path in file_or_dir_paths:
+        path = Path(os.path.expandvars(file_or_dir_path))
+        
         file_or_dir_path = os.path.expandvars(file_or_dir_path)
-        if os.path.isdir(file_or_dir_path):
-            for file_path in glob(os.path.join(file_or_dir_path, "*.py")):
-                find_and_extend_classes(classes, file_path, supertype_filter, tag_filter)
+        if path.is_dir():
+            # recursive search
+            # https://stackoverflow.com/questions/50714469/recursively-iterate-through-all-subdirectories-using-pathlib
+            for file_path in path.glob("*.py"):
+                find_and_extend_classes(classes, file_path, supertype_filter, tag_filter, avoid_tag_str)
+            
+            if recursive:
+                for recursive_path in path.glob('**/*'):
+                    if recursive_path.is_dir():
+                        for file_path in recursive_path.glob("*.py"):
+                            find_and_extend_classes(classes, file_path, supertype_filter, tag_filter, avoid_tag_str)
         elif os.path.isfile(file_or_dir_path):
-            find_and_extend_classes(classes, file_or_dir_path, supertype_filter, tag_filter)
+            find_and_extend_classes(classes, file_or_dir_path, supertype_filter, tag_filter, avoid_tag_str)
         else:
             raise FileNotFoundError(file_or_dir_path)
 
     classes.sort(key=lambda item: item.cls.__name__)
     class_names = [item.cls.__name__ for item in classes]
     if len(classes) == 0:
-        print("No classes fetched: " + str(class_names)) # was a warning
+        logger.warning("No classes fetched: " + format_list(class_names)) # was a warning
     else:
-        print("All classes fetched: " + str(class_names))
+        logger.info("All classes fetched: " + format_list(class_names))
     return classes
```

### Comparing `clsquery-1.1/clsquery/has_supertype.py` & `clsquery-1.2/clsquery/has_supertype.py`

 * *Files identical despite different names*

### Comparing `clsquery-1.1/clsquery.egg-info/SOURCES.txt` & `clsquery-1.2/clsquery.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 clsquery/constants.py
 clsquery/convert_classes_to_table.py
 clsquery/custom_logger.py
 clsquery/default_formatter.py
 clsquery/filter_by_types.py
 clsquery/format_list.py
 clsquery/format_table.py
+clsquery/get_classes_at_path.py
 clsquery/get_classes_from_paths.py
 clsquery/get_time.py
 clsquery/has_supertype.py
 clsquery/query.py
 clsquery.egg-info/PKG-INFO
 clsquery.egg-info/SOURCES.txt
 clsquery.egg-info/dependency_links.txt
```

### Comparing `clsquery-1.1/pyproject.toml` & `clsquery-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clsquery"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="Kenneth Mead", email="kennethmead784@gmail.com" },
 ]
 description = "A package for querying Python classes"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers=[
```

### Comparing `clsquery-1.1/tests/test_query.py` & `clsquery-1.2/tests/test_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,31 +11,57 @@
             # module
             os.path.join(self.base_folder, "clsquery", "classes", "class_query.py")
         ]
 
     def test_basic_query(self):
         result = clsquery.query(self.paths, log_results=True)
 
+    def test_basic_query_literal_type_args(self):
+        result = clsquery.query(paths=self.paths[0], 
+                                supertypes="object", 
+                                tags="", 
+                                log_results=True)
+
+    def test_basic_query_mixed_type_args(self):
+        result = clsquery.query(paths=self.paths, 
+                                supertypes="object", 
+                                tags=None, 
+                                log_results=True)
+
     def test_saved_query(self):
         saved_query = clsquery.ClassQuery(self.paths)
         results = saved_query.query(log_results=True)
 
+    def test_saved_query_with_overrides(self):
+        saved_query = clsquery.ClassQuery(self.paths, group_by=None)
+        results = saved_query.query(paths=self.paths[0], group_by="__base__.__name__", log_results=True)
+
+    def test_saved_query_with_overrides2(self):
+        saved_query = clsquery.ClassQuery(self.paths, group_by=None)
+        results = clsquery.query(paths=self.paths[0], group_by="__base__.__name__", query=saved_query, log_results=True)
+
     def test_grouped_query(self):
         result = clsquery.query(self.paths, group_by=["__base__.__name__", "__name__"], log_results=True)
 
     def test_no_duplicate_class(self):
         # This query runs into the DuplicateClassError class twice
         result = clsquery.query(paths=self.paths, log_results=True)
         query_item_set = set()
         for query_item in result.classes:
             if (query_item.cls.__name__, query_item.path) not in query_item_set:
                 query_item_set.add(query_item.cls.__name__)
             else:
                 raise DuplicateClassError(query_item.cls.__name__, query_item.path)
 
+    def test_recursive_query(self):
+        result = clsquery.query(paths=[os.path.join(self.base_folder, "clsquery")], 
+                                recursive=True,
+                                log_results=True)
+
+
 class DuplicateClassError(Exception):
     def __init__(self, class_name: str, filepath:str) -> None:
         message = f"""While fetching classes, two classes with the same name and path were added to the query. This should not be possible
 
 Class Name:  {class_name}
 Path:  {filepath}
 """
```

