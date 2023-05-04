# Comparing `tmp/bp_data_fabric-1.0.2.tar.gz` & `tmp/bp_data_fabric-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-1.0.2.tar", last modified: Thu May  4 07:54:04 2023, max compression
+gzip compressed data, was "bp_data_fabric-1.0.3.tar", last modified: Thu May  4 09:48:08 2023, max compression
```

## Comparing `bp_data_fabric-1.0.2.tar` & `bp_data_fabric-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:54:04.618901 bp_data_fabric-1.0.2/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.2/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 07:54:04.618461 bp_data_fabric-1.0.2/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.2/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:54:04.615853 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-05-04 07:54:04.000000 bp_data_fabric-1.0.2/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 07:54:04.617280 bp_data_fabric-1.0.2/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1082 2023-04-26 08:43:55.000000 bp_data_fabric-1.0.2/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2515 2023-04-26 08:44:24.000000 bp_data_fabric-1.0.2/data_fabric/components.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-04 07:54:04.619098 bp_data_fabric-1.0.2/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      860 2023-05-04 07:48:59.000000 bp_data_fabric-1.0.2/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:48:08.718685 bp_data_fabric-1.0.3/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.3/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 09:48:08.718266 bp_data_fabric-1.0.3/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.3/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:48:08.716621 bp_data_fabric-1.0.3/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 09:48:08.000000 bp_data_fabric-1.0.3/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-05-04 09:48:08.000000 bp_data_fabric-1.0.3/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-04 09:48:08.000000 bp_data_fabric-1.0.3/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-05-04 09:48:08.000000 bp_data_fabric-1.0.3/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-05-04 09:48:08.000000 bp_data_fabric-1.0.3/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 09:48:08.717522 bp_data_fabric-1.0.3/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1082 2023-04-26 08:43:55.000000 bp_data_fabric-1.0.3/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2749 2023-05-04 09:47:19.000000 bp_data_fabric-1.0.3/data_fabric/components.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-04 09:48:08.718818 bp_data_fabric-1.0.3/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      860 2023-05-04 09:48:03.000000 bp_data_fabric-1.0.3/setup.py
```

### Comparing `bp_data_fabric-1.0.2/LICENSE` & `bp_data_fabric-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.2/data_fabric/__init__.py` & `bp_data_fabric-1.0.3/data_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.2/data_fabric/components.py` & `bp_data_fabric-1.0.3/data_fabric/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         columns: List[dict] = [],
         data={},
         error="",
         on_database_change=None,
         on_table_change=None,
         on_generate_query=None,
         on_copy_query=None,
-        on_execute=None,
+        on_execute_query=None,
         show_data_grid=True,
         show_charts=True,
     ):
     
 
     with open('style.css') as f:
         st.markdown(f'<style>{f.read()}</style>', unsafe_allow_html=True)
@@ -34,18 +34,19 @@
         tables=tables,
         columns=columns,
         error=error,
         on_database_change=on_database_change,
         on_table_change=on_table_change,
         on_generate_query=on_generate_query,
         on_copy_query=on_copy_query,
+        on_execute_query=on_execute_query,
     )
 
-    if query != "":
-      st.button("Execute", on_click=on_execute)
+    # if query != "":
+    #   st.button("Execute", on_click=on_execute_query)
     st.write("")
     st.write("")
     if show_data_grid == True:
         render_data_grid(
             title=data_grid_title,
             rows=data.get("rows", []),
             columns=data.get("columns", []),
@@ -59,29 +60,35 @@
 
 def render_query_tool(
         query: str = "",
         title: str = "",
         databases: List[str] = [],
         tables: List[dict] = [],
         columns: List[dict] = [],
+        show_execute=True,
+        error="",
         on_database_change=None,
         on_table_change=None,
         on_generate_query=None,
         on_copy_query=None,
+        on_execute_query=None,
 ):
     qt.query_tool(
         query=query,
         title=title,
         databases=databases,
         tables=tables,
         columns=columns,
+        error=error,
+        show_execute=show_execute,
         on_database_change=on_database_change,
         on_table_change=on_table_change,
         on_generate_query=on_generate_query,
         on_copy_query=on_copy_query,
+        on_execute_query=on_execute_query,
         key="query_builder",
     )  
 
 def render_data_grid(title: str="", rows: List = [], columns: List = []):
     dg.data_grid(
         title=title,
         rows=rows,
```

### Comparing `bp_data_fabric-1.0.2/setup.py` & `bp_data_fabric-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp_data_fabric",
-    version="1.0.2",
+    version="1.0.3",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="",    
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

