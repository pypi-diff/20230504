# Comparing `tmp/twb_project-0.9.2.tar.gz` & `tmp/twb_project-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.9.2.tar", max compression
+gzip compressed data, was "twb_project-0.9.3.tar", max compression
```

## Comparing `twb_project-0.9.2.tar` & `twb_project-0.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.2/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.2/README.md
--rw-r--r--   0        0        0      760 2023-05-03 16:56:00.321929 twb_project-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.2/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.2/twb/bip.py
--rw-r--r--   0        0        0    19310 2023-05-03 14:55:40.606683 twb_project-0.9.2/twb/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.2/twb/builder_helpers.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.2/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.2/twb/downloader.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.2/twb/logger.py
--rw-r--r--   0        0        0     1594 2023-05-02 23:19:18.752642 twb_project-0.9.2/twb/logger_init.py
--rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.2/twb/modifier.py
--rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.2/twb/parallelization.py
--rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.2/twb/reader.py
--rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.2/twb/utils.py
--rw-r--r--   0        0        0     5461 2023-05-03 17:57:27.349254 twb_project-0.9.2/twb/warehouse.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.2/setup.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.9.3/README.md
+-rw-r--r--   0        0        0      760 2023-05-04 16:31:40.383846 twb_project-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-0.9.3/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.9.3/twb/bip.py
+-rw-r--r--   0        0        0    19874 2023-05-04 17:29:52.015172 twb_project-0.9.3/twb/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-0.9.3/twb/builder_helpers.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.9.3/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.9.3/twb/downloader.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-0.9.3/twb/logger.py
+-rw-r--r--   0        0        0     1594 2023-05-02 23:19:18.752642 twb_project-0.9.3/twb/logger_init.py
+-rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-0.9.3/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-0.9.3/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-0.9.3/twb/reader.py
+-rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-0.9.3/twb/utils.py
+-rw-r--r--   0        0        0     6334 2023-05-04 17:39:06.788669 twb_project-0.9.3/twb/warehouse.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.9.3/setup.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.9.3/PKG-INFO
```

### Comparing `twb_project-0.9.2/LICENSE` & `twb_project-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/README.md` & `twb_project-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/pyproject.toml` & `twb_project-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.9.2"
+version = "0.9.3"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.9.2/twb/bip.py` & `twb_project-0.9.3/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/twb/builder.py` & `twb_project-0.9.3/twb/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import logging
 import os
-import shutil
 from functools import partial
 from multiprocessing import Pool
 from typing import List, Tuple, Optional
 import time
 import uuid
 
 import xmltodict
@@ -81,14 +80,16 @@
         os.makedirs(temp_dir, exist_ok=True)
 
         archive_filename = os.path.basename(file_path)
         decompressed_dir_name = '.'.join(archive_filename.split('.')[:-1])
         decompressed_dir_path = os.path.join(temp_dir, decompressed_dir_name)
         os.makedirs(decompressed_dir_path, exist_ok=True)
 
+        logging.debug(f'Decompressing [{archive_filename}]...')
+
         with py7zr.SevenZipFile(file_path, mode='r', mp=False) as z:
             start_time = time.time()
             z.extractall(path=decompressed_dir_path)
             end_time = time.time()
             execution_duration = end_time - start_time
             logging.debug(f'Decompression took {execution_duration:.2f} seconds. ({archive_filename})')
         decompressed_files = get_file_list(decompressed_dir_path)
@@ -101,14 +102,16 @@
         :param xml_path: the path of the file to be processed.
         :return: the number of URLs processed
         """
         # Initialize processed directory.
         processed_dir = os.path.join(self.output_dir, 'temp', 'processed')
         os.makedirs(processed_dir, exist_ok=True)
 
+        logging.debug(f'Processing {os.path.basename(xml_path)}...')
+
         article_id: Optional[str] = None
         article_title: Optional[str] = None
         article_info: Optional[dict] = None
 
         # A JSONL file.
         processed_filepath: Optional[str] = None
 
@@ -208,26 +211,33 @@
             # Finalize the last article.
             _finalizing_metadata()
 
         except Exception as e:
             logging.critical(f'Error occurred when processing the file [{xml_file}]: {e}')
             processed_files = []
 
-        finally:
+        try:
             # Remove XML file.
             os.remove(xml_path)
 
             # If the parent dir of this XML file is empty, remove it.
             parent_dir = os.path.dirname(xml_path)
             if len(os.listdir(parent_dir)) == 0:
-                shutil.rmtree(parent_dir)
+                cleanup_dir(parent_dir)
+
+        except:
+            logging.error(f'Failed to remove the XML file [{xml_path}].')
+
+        logging.debug(f'Processed (OK): {processed_files}')
 
         return processed_files
 
     def _warehouse_executor(self, assigned_warehouse: str, combo_files_list: List[Tuple[str, str]]):
+        logging.debug(f'Warehouse delivering: {assigned_warehouse}')
+
         try:
             warehouse_filename, warehouse_metadata_filename = get_warehouse_filenames(assigned_warehouse)
             warehouse_path = os.path.join(self.output_dir, warehouse_filename)
             warehouse_metadata_path = os.path.join(self.output_dir, warehouse_metadata_filename)
 
             warehouse_file = open(warehouse_path, 'a')
 
@@ -251,30 +261,36 @@
 
                 # Remove the modified file.
                 os.remove(processed_file)
                 os.remove(metadata_file)
 
             warehouse_file.close()
 
+            logging.debug(f'Warehouse delivered (OK): {assigned_warehouse}')
+
         except Exception as e:
             logging.critical(f'Error occurred when moving the file to the warehouse. {e}')
 
         return assigned_warehouse
 
     def _cleanup_executor(self, warehouse_filename: str):
+        logging.debug(f'Warehouse cleaning: {warehouse_filename}')
+
         try:
             original_file_path = os.path.join(self.output_dir, warehouse_filename)
             if not os.path.exists(original_file_path):
                 logging.critical(f'The file {warehouse_filename} [{original_file_path}] does not exist.')
                 return None
 
             compressed_path = original_file_path + COMPRESSION_EXTENSION
             compress_zstd(original_file_path, compressed_path)
             os.remove(original_file_path)
 
+            logging.debug(f'Warehouse cleaned (OK): {warehouse_filename}')
+
             return compressed_path
 
         except:
             logging.critical(f'Error occurred when compressing warehouse [{warehouse_filename}].')
             return None
 
     def build(self):
@@ -317,15 +333,15 @@
 
         processed_count = 0
         finished_count = 0
 
         def _decompress_callback(decompressed_files: List[str]):
             nonlocal available_process_count
 
-            logging.debug(f'Decompressed: {decompressed_files}')
+            logging.debug(f'Decompressed (OK): {decompressed_files}')
 
             for decompressed_file in decompressed_files:
                 next_task_type = 'process'
                 next_args = (decompressed_file,)
                 tasks.insert(0, (next_task_type, next_args))
 
             available_process_count += 1
```

### Comparing `twb_project-0.9.2/twb/decompressor.py` & `twb_project-0.9.3/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/twb/downloader.py` & `twb_project-0.9.3/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/twb/logger.py` & `twb_project-0.9.3/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/twb/logger_init.py` & `twb_project-0.9.3/twb/logger_init.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/twb/modifier.py` & `twb_project-0.9.3/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/twb/parallelization.py` & `twb_project-0.9.3/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/twb/reader.py` & `twb_project-0.9.3/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/twb/utils.py` & `twb_project-0.9.3/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.9.2/twb/warehouse.py` & `twb_project-0.9.3/twb/warehouse.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,26 +17,32 @@
         self.compress = compress
 
         self.warehouse_indexer = 0
         self.available_warehouses = []
         self.occupied_warehouses = []
 
     def create_warehouse(self):
-        # Fill 6 digits with 0s.
+        # Fill 5 digits with 0s.
         curr_index = str(self.warehouse_indexer).zfill(5)
         new_filename_basename = f'{self.prefix}{curr_index}{self.suffix}'
-        new_filename, new_metadata_filename = get_warehouse_filenames(new_filename_basename)
-        new_filepath = os.path.join(self.output_dir, new_filename)
-        new_metadata_filepath = os.path.join(self.output_dir, new_metadata_filename)
-        with open(new_filepath, 'w') as f:
-            f.truncate(0)
-        with open(new_metadata_filepath, 'w') as f:
-            f.truncate(0)
-        self.available_warehouses.append(new_filename_basename)
-        self.warehouse_indexer += 1
+
+        try:
+            new_filename, new_metadata_filename = get_warehouse_filenames(new_filename_basename)
+            new_filepath = os.path.join(self.output_dir, new_filename)
+            new_metadata_filepath = os.path.join(self.output_dir, new_metadata_filename)
+            with open(new_filepath, 'w') as f:
+                f.truncate(0)
+            with open(new_metadata_filepath, 'w') as f:
+                f.truncate(0)
+            logging.debug(f'New warehouse created: {new_filename_basename}.')
+            self.available_warehouses.append(new_filename_basename)
+            self.warehouse_indexer += 1
+
+        except:
+            logging.error(f'Failed to create new warehouse: {new_filename_basename}.')
 
     def assign_warehouse(self) -> str:
         """
         This function is intended to be called in main process (no parallelism).
         """
         free_warehouses = [w for w in self.available_warehouses if w not in self.occupied_warehouses]
         if len(free_warehouses) == 0:
@@ -60,48 +66,58 @@
 
         return min_size_warehouse
 
     def bulk_assign(self, files: List[str]) -> Dict[str, List[str]]:
         """
         This function is intended to be called in main process (no parallelism).
         """
-        free_warehouses = []
-        remaining_sizes = []
+        logging.debug(f'Bulk assigning {len(files)} files.')
+
+        free_warehouses = [w for w in self.available_warehouses if w not in self.occupied_warehouses]
+        remaining_sizes = {
+            w: self.max_size - get_file_size(os.path.join(self.output_dir, get_warehouse_filenames(w)[0]))
+            for w in free_warehouses
+        }
         warehouse_assignments = dict()
 
-        def _update_sizes():
+        def _sync_warehouses():
             nonlocal free_warehouses, remaining_sizes
             free_warehouses = [w for w in self.available_warehouses if w not in self.occupied_warehouses]
-            remaining_sizes = [
-                self.max_size - get_file_size(os.path.join(self.output_dir, get_warehouse_filenames(w)[0]))
-                for w in free_warehouses
-            ]
+            for w in free_warehouses:
+                if w not in remaining_sizes:
+                    remaining_sizes[w] = self.max_size
 
-        def _get_acceptable_warehouses():
+        def _get_acceptable_warehouses(needed_size):
             nonlocal free_warehouses, remaining_sizes
-            return [(w, s) for w, s in zip(free_warehouses, remaining_sizes) if s >= file_size]
-
-        _update_sizes()
+            acceptable_warehouses = []
+            for w in free_warehouses:
+                if w not in remaining_sizes:
+                    remaining_sizes[w] = self.max_size
+                if remaining_sizes[w] >= needed_size:
+                    acceptable_warehouses.append((w, remaining_sizes[w]))
+            return acceptable_warehouses
 
         for file in files:
             file_size = get_file_size(file)
-            _update_sizes()
-            acceptable_warehouses = _get_acceptable_warehouses()
-            if not acceptable_warehouses:
+            _sync_warehouses()
+            acceptable_warehouses = _get_acceptable_warehouses(needed_size=file_size)
+            while not acceptable_warehouses:
                 self.create_warehouse()
-                _update_sizes()
-                acceptable_warehouses = _get_acceptable_warehouses()
+                _sync_warehouses()
+                acceptable_warehouses = _get_acceptable_warehouses(needed_size=file_size)
+                if not acceptable_warehouses:
+                    logging.critical(f'Failed to create new warehouse for file: {file}.')
             min_size_warehouses = min(acceptable_warehouses, key=lambda x: x[1])
             min_size_warehouse = min_size_warehouses[0]
             if min_size_warehouse not in warehouse_assignments:
                 warehouse_assignments[min_size_warehouse] = []
             warehouse_assignments[min_size_warehouse].append(file)
-            remaining_sizes[free_warehouses.index(min_size_warehouse)] -= file_size
+            remaining_sizes[min_size_warehouse] -= file_size
 
-        for warehouse in warehouse_assignments:
+        for warehouse in warehouse_assignments.keys():
             logging.debug(f'Bulk assigning warehouse: {warehouse}.')
             self.occupied_warehouses.append(warehouse)
 
         return warehouse_assignments
 
     def release_warehouse(self, warehouse: str) -> Union[str, None]:
         try:
```

### Comparing `twb_project-0.9.2/setup.py` & `twb_project-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.9.2/PKG-INFO` & `twb_project-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.9.2
+Version: 0.9.3
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

