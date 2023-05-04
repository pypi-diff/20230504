# Comparing `tmp/cads_sdk-0.0.15-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.16rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 55297 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-Apr-28 02:33 cads_sdk/__init__.py
+Zip file size: 55291 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     1268 b- defN 23-May-04 08:32 cads_sdk/__init__.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
 -rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
 -rw-rw-r--  2.0 unx    84386 b- defN 23-Apr-28 02:32 cads_sdk/nosql/converter.py
--rw-rw-r--  2.0 unx    19499 b- defN 23-Apr-20 10:32 cads_sdk/nosql/display.py
+-rw-rw-r--  2.0 unx    18788 b- defN 23-May-04 08:32 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
 -rw-rw-r--  2.0 unx      591 b- defN 23-Apr-09 13:11 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7126 b- defN 23-Apr-28 02:36 cads_sdk-0.0.15.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-28 02:36 cads_sdk-0.0.15.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-28 02:36 cads_sdk-0.0.15.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1479 b- defN 23-Apr-28 02:36 cads_sdk-0.0.15.dist-info/RECORD
-18 files, 275607 bytes uncompressed, 52891 bytes compressed:  80.8%
+-rw-rw-r--  2.0 unx     7129 b- defN 23-May-04 08:33 cads_sdk-0.0.16rc0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-04 08:33 cads_sdk-0.0.16rc0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-04 08:33 cads_sdk-0.0.16rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1491 b- defN 23-May-04 08:33 cads_sdk-0.0.16rc0.dist-info/RECORD
+18 files, 274914 bytes uncompressed, 52861 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.15.dist-info/METADATA
+Filename: cads_sdk-0.0.16rc0.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.15.dist-info/WHEEL
+Filename: cads_sdk-0.0.16rc0.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.15.dist-info/top_level.txt
+Filename: cads_sdk-0.0.16rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.15.dist-info/RECORD
+Filename: cads_sdk-0.0.16rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.15'
+__version__ = '0.0.16rc0'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## cads_sdk/nosql/display.py

```diff
@@ -110,15 +110,15 @@
     if isinstance(self.from_idx, int):
         self.from_idx = self.from_idx
         if isinstance(self.to_idx, int):
             self.to_idx = self.to_idx
         else:
             self.to_idx = self.from_idx + self.limit_idx
     else:
-        self.from_idx = 0
+        self.from_idx = 1
         if isinstance(self.to_idx, int):
             self.to_idx = self.to_idx
         else:
             self.to_idx = self.limit_idx
     from pyspark.sql import DataFrame as SparkDataFrame
     SparkDataFrame.from_idx = self.from_idx
     SparkDataFrame.to_idx = self.to_idx
@@ -315,28 +315,15 @@
         self.height = height
         self.html_attributes = html_attributes
         self.thumbnail_width = thumbnail_width
         self.thumbnail_height = thumbnail_height
         self.from_idx = from_idx
         self.to_idx = to_idx
         self.limit = limit
-        
-    def convert_to_index_sliceable(self):
-        if isinstance(self.from_idx, int):
-            self.from_idx = self.from_idx
-            if isinstance(self.to_idx, int):
-                self.to_idx = self.to_idx
-            else:
-                self.to_idx = self.from_idx + self.limit
-        else:
-            self.from_idx = 0
-            if isinstance(self.to_idx, int):
-                self.to_idx = self.to_idx
-            else:
-                self.to_idx = self.limit
+    
         
         
     def get_spark(self):
         return ss.PySpark(driver_memory='32G', num_executors='4', executor_memory='4G', port='', yarn=False).spark
     
     def check_delta(self, input_path):
         list_file = ss.ls(input_path)
@@ -400,17 +387,18 @@
             width = ' width="%d"' % self.width
         if self.height:
             height = ' height="%d"' % self.height
             
         if isinstance(self.input_path, str):
             df_path = self.generate_sql("path, thumbnail")
         
-            if self.from_idx:
-                self.convert_to_index_sliceable()
+            if isinstance(self.from_idx, int):
                 df_path = df_path[self.from_idx:self.to_idx]
+        elif isinstance(self.input_path, SparkDataFrame):
+            df_path = self.input_path
         else:
             raise ValueError("Check your input_path, it not string or can not be found")
         
         selection_box = widgets.VBox()
         selection_toggles = []
         selected_labels = {}
         labels = {}
@@ -484,27 +472,14 @@
         self.html_attributes = html_attributes
         self.thumbnail_width = thumbnail_width
         self.thumbnail_height = thumbnail_height
         self.from_idx = from_idx
         self.to_idx = to_idx
         self.limit = limit
         
-    def convert_to_index_sliceable(self):
-        if isinstance(self.from_idx, int):
-            self.from_idx = self.from_idx
-            if isinstance(self.to_idx, int):
-                self.to_idx = self.to_idx
-            else:
-                self.to_idx = self.from_idx + self.limit
-        else:
-            self.from_idx = 0
-            if isinstance(self.to_idx, int):
-                self.to_idx = self.to_idx
-            else:
-                self.to_idx = self.limit
         
     def get_spark(self):
         return ss.PySpark(driver_memory='32G', num_executors='4', executor_memory='4G', port='', yarn=False).spark
     
     def check_delta(self, input_path):
         list_file = ss.ls(input_path)
         for f in list_file:
@@ -554,17 +529,22 @@
             width = ' width="%d"' % self.width
         if self.height:
             height = ' height="%d"' % self.height
             
         if isinstance(self.input_path, str):
             df_path = self.generate_sql("path")
         
-            if self.from_idx:
-                self.convert_to_index_sliceable()
+            if isinstance(self.from_idx, int):
                 df_path = df_path[self.from_idx:self.to_idx]
+        elif isinstance(self.input_path, SparkDataFrame):
+            df_path = self.input_path
+        
+        else:
+            raise ValueError("Check your input_path, it not string or can not be found")
+            
         
         selection_box = widgets.VBox()
         selection_toggles = []
         selected_labels = {}
         
         layout = widgets.Layout(width=str(pd.options.display.width*5)+'px', height='40px')
```

## Comparing `cads_sdk-0.0.15.dist-info/METADATA` & `cads_sdk-0.0.16rc0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.15
+Version: 0.0.16rc0
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -16,15 +16,15 @@
 Requires-Dist: pydub
 Requires-Dist: ipywidgets
 Requires-Dist: petastorm
 
 -----------------
 
 # cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
-[![PyPI Latest Release](https://img.shields.io/badge/pypi-0.0.15-blue)](https://pypi.org/project/cads-sdk/)
+[![PyPI Latest Release](https://img.shields.io/badge/pypi-0.0.16-blue)](https://pypi.org/project/cads-sdk/)
 [![Package Status](https://img.shields.io/badge/status-stable-green)](https://pypi.org/project/cads-sdk/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cads-sdk?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cads-sdk)
 [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-CADS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://blog.cads.live/)
 
 
 
 ## What is it?
```

