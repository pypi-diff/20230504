# Comparing `tmp/bp_data_fabric-1.0.5.tar.gz` & `tmp/bp_data_fabric-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-1.0.5.tar", last modified: Thu May  4 10:00:37 2023, max compression
+gzip compressed data, was "bp_data_fabric-1.0.6.tar", last modified: Thu May  4 10:06:45 2023, max compression
```

## Comparing `bp_data_fabric-1.0.5.tar` & `bp_data_fabric-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 10:00:37.354115 bp_data_fabric-1.0.5/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.5/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 10:00:37.353774 bp_data_fabric-1.0.5/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.5/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 10:00:37.351275 bp_data_fabric-1.0.5/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 10:00:37.000000 bp_data_fabric-1.0.5/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-05-04 10:00:37.000000 bp_data_fabric-1.0.5/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-04 10:00:37.000000 bp_data_fabric-1.0.5/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-05-04 10:00:37.000000 bp_data_fabric-1.0.5/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-05-04 10:00:37.000000 bp_data_fabric-1.0.5/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 10:00:37.352872 bp_data_fabric-1.0.5/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1140 2023-05-04 09:51:46.000000 bp_data_fabric-1.0.5/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2811 2023-05-04 09:57:35.000000 bp_data_fabric-1.0.5/data_fabric/components.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-04 10:00:37.354234 bp_data_fabric-1.0.5/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      860 2023-05-04 10:00:32.000000 bp_data_fabric-1.0.5/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 10:06:45.243146 bp_data_fabric-1.0.6/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-1.0.6/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 10:06:45.242789 bp_data_fabric-1.0.6/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-1.0.6/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 10:06:45.240739 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      265 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       88 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-05-04 10:06:45.000000 bp_data_fabric-1.0.6/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-04 10:06:45.241728 bp_data_fabric-1.0.6/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1158 2023-05-04 10:06:32.000000 bp_data_fabric-1.0.6/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2811 2023-05-04 09:57:35.000000 bp_data_fabric-1.0.6/data_fabric/components.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-04 10:06:45.243270 bp_data_fabric-1.0.6/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      860 2023-05-04 10:06:38.000000 bp_data_fabric-1.0.6/setup.py
```

### Comparing `bp_data_fabric-1.0.5/LICENSE` & `bp_data_fabric-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.5/data_fabric/__init__.py` & `bp_data_fabric-1.0.6/data_fabric/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     columns: List[dict] = [],
     error: str = "",
     show_execute=True,
     on_database_change=None,
     on_table_change=None,
     on_generate_query=None,
     on_copy_query=None,
-    on_execute=None,
+    on_execute_query=None,
     data={},
     show_data_grid=True,
     show_charts=True,
 ):
     
     main(
         query=query,
@@ -32,11 +32,11 @@
         data=data,
         error=error,
         show_execute=show_execute,
         on_database_change=on_database_change,
         on_table_change=on_table_change,
         on_generate_query=on_generate_query,
         on_copy_query=on_copy_query,
-        on_execute=on_execute,
+        on_execute_query=on_execute_query,
         show_data_grid=show_data_grid,
         show_charts=show_charts,
     )
```

### Comparing `bp_data_fabric-1.0.5/data_fabric/components.py` & `bp_data_fabric-1.0.6/data_fabric/components.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-1.0.5/setup.py` & `bp_data_fabric-1.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp_data_fabric",
-    version="1.0.5",
+    version="1.0.6",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="",    
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

