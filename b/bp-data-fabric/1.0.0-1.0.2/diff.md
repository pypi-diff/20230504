# Comparing `tmp/bp_data_fabric-1.0.0.tar.gz` & `tmp/bp_data_fabric-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-1.0.0.tar", last modified: Wed Apr 26 08:41:51 2023, max compression
+gzip compressed data, was "bp_data_fabric-1.0.2.tar", last modified: Thu May  4 07:54:04 2023, max compression
```

## Comparing `bp_data_fabric-1.0.0.tar` & `bp_data_fabric-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:41:51.472012 bp_data_fabric-1.0.0/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.0/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-26 08:41:51.471571 bp_data_fabric-1.0.0/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.0/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:41:51.470043 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      276 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-26 08:41:51.000000 bp_data_fabric-1.0.0/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-26 08:41:51.470967 bp_data_fabric-1.0.0/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1040 2023-04-24 07:05:06.000000 bp_data_fabric-1.0.0/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2476 2023-04-24 09:14:37.000000 bp_data_fabric-1.0.0/data_fabric/components.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-26 08:41:51.472157 bp_data_fabric-1.0.0/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      712 2023-04-26 08:41:39.000000 bp_data_fabric-1.0.0/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:54:04.618901 bp_data_fabric-1.0.2/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.2/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 07:54:04.618461 bp_data_fabric-1.0.2/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.2/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:54:04.615853 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:54:04.617280 bp_data_fabric-1.0.2/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1082 2023-04-26 08:43:55.000000 bp_data_fabric-1.0.2/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2515 2023-04-26 08:44:24.000000 bp_data_fabric-1.0.2/data_fabric/components.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-04 07:54:04.619098 bp_data_fabric-1.0.2/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      860 2023-05-04 07:48:59.000000 bp_data_fabric-1.0.2/setup.py
```

### Comparing `bp_data_fabric-1.0.0/LICENSE` & `bp_data_fabric-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.0/data_fabric/__init__.py` & `bp_data_fabric-1.0.2/data_fabric/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     query: str = "",
     query_tool_title: str = "",
     data_grid_title: str = "",
     data_visualization_title: str = "",
     databases: List[str] = [],
     tables: List[dict] = [],
     columns: List[dict] = [],
+    error: str = "",
     on_database_change=None,
     on_table_change=None,
     on_generate_query=None,
     on_copy_query=None,
     on_execute=None,
     data={},
     show_data_grid=True,
@@ -24,14 +25,15 @@
         query_tool_title=query_tool_title,
         data_grid_title=data_grid_title,
         data_visualization_title=data_visualization_title,
         databases=databases,
         tables=tables,
         columns=columns,
         data=data,
+        error=error,
         on_database_change=on_database_change,
         on_table_change=on_table_change,
         on_generate_query=on_generate_query,
         on_copy_query=on_copy_query,
         on_execute=on_execute,
         show_data_grid=show_data_grid,
         show_charts=show_charts,
```

### Comparing `bp_data_fabric-1.0.0/data_fabric/components.py` & `bp_data_fabric-1.0.2/data_fabric/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         query_tool_title: str = "",
         data_grid_title: str = "",
         data_visualization_title: str = "",
         databases: List[str] = [],
         tables: List[dict] = [],
         columns: List[dict] = [],
         data={},
+        error="",
         on_database_change=None,
         on_table_change=None,
         on_generate_query=None,
         on_copy_query=None,
         on_execute=None,
         show_data_grid=True,
         show_charts=True,
@@ -28,14 +29,15 @@
 
     render_query_tool(
         query=query,
         title=query_tool_title,
         databases=databases,
         tables=tables,
         columns=columns,
+        error=error,
         on_database_change=on_database_change,
         on_table_change=on_table_change,
         on_generate_query=on_generate_query,
         on_copy_query=on_copy_query,
     )
 
     if query != "":
```

### Comparing `bp_data_fabric-1.0.0/setup.py` & `bp_data_fabric-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import setuptools
 
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setuptools.setup(
     name="bp_data_fabric",
-    version="1.0.0",
+    version="1.0.2",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
-    description="",
-    long_description="",
-    long_description_content_type="text/plain",
+    description="",    
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.8.10",
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
```

