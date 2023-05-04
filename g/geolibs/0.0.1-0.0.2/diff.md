# Comparing `tmp/geolibs-0.0.1.tar.gz` & `tmp/geolibs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolibs-0.0.1.tar", max compression
+gzip compressed data, was "geolibs-0.0.2.tar", max compression
```

## Comparing `geolibs-0.0.1.tar` & `geolibs-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      294 2023-05-03 12:27:37.610263 geolibs-0.0.1/README.rst
--rwxr-xr-x   0        0        0      430 2023-05-03 12:27:37.633972 geolibs-0.0.1/geolibs/__init__.py
--rwxr-xr-x   0        0        0     5129 2023-05-03 11:53:56.277548 geolibs-0.0.1/geolibs/engine_cocoext.py
--rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.1/geolibs/engine_cocometric.py
--rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.1/geolibs/enginelogger_hook.py
--rwxr-xr-x   0        0        0     8258 2023-05-03 11:53:56.311818 geolibs-0.0.1/geolibs/loading.py
--rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.1/geolibs/misc.py
--rwxr-xr-x   0        0        0     1198 2023-05-03 12:27:37.669954 geolibs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 geolibs-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      528 2023-05-04 20:41:51.294192 geolibs-0.0.2/README.rst
+-rwxr-xr-x   0        0        0      465 2023-05-04 20:42:02.507036 geolibs-0.0.2/geolibs/__init__.py
+-rwxr-xr-x   0        0        0     5514 2023-05-04 20:24:29.362348 geolibs-0.0.2/geolibs/engine_cocoext.py
+-rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.2/geolibs/engine_cocometric.py
+-rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.2/geolibs/enginelogger_hook.py
+-rwxr-xr-x   0        0        0    12295 2023-05-04 20:24:29.371193 geolibs-0.0.2/geolibs/loading.py
+-rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.2/geolibs/misc.py
+-rwxr-xr-x   0        0        0     1066 2023-05-04 20:42:02.499532 geolibs-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 geolibs-0.0.2/PKG-INFO
```

### Comparing `geolibs-0.0.1/geolibs/engine_cocoext.py` & `geolibs-0.0.2/geolibs/engine_cocoext.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,41 +18,50 @@
                  vector_dir_path: str,
                  split: str = "train",
                  class_title: str = None,
                  slice: bool = False,
                  window: tuple = None,
                  stride: tuple = None,
                  pipeline: List[Union[dict, Callable]] = [],
-                 max_refetch: int = 1000):
+                 max_refetch: int = 1000,
+                 ignore_index: int = 255,
+                 reduce_zero_label: bool = False):
         self.raster_data_path = f"{data_path}/{raster_dir_path}"
         self.vector_data_path = f"{data_path}/{vector_dir_path}"
 
         self.split = split
         self.slice = slice 
         self.window = window 
         self.stride = stride
         self.class_title = class_title
+        self.ignore_index = ignore_index
+        self.reduce_zero_label = reduce_zero_label
 
         self.pipeline = Compose(pipeline)
         self.max_refetch = max_refetch
 
         self.get_data_list()
+    
+    def full_init(self):
+        self.get_data_info
 
     def load_vector_file(self, vec_path):
         vec_map = json.load(open(vec_path))
 
         file_name = vec_map["images"][0]["file_name"].split("/")[-1]
         file_path = f"{self.raster_data_path}/{file_name}"
 
         img_map = {
             "img_path": file_path,
             "img_id": vec_map["info"]["id"],
             "height": vec_map["images"][0]["height"],
             "width": vec_map["images"][0]["width"],
-            "instances": []
+            "instances": [],
+            "seg_fields": [],
+            "reduce_zero_label": self.reduce_zero_label
         }
 
         for annotation in vec_map["annotations"]:
             try:
                 xmin, ymin, width, height = annotation["bbox"]
                 xmax,ymax = xmin+width, ymin+height
                 bbox = [xmin, ymin, xmax, ymax]
@@ -96,15 +105,16 @@
         self._metainfo = {
             "title": metadata["title"],
             "description": metadata["description"],
             "tags": metadata["tags"],
             "problemType": metadata["problemType"] if "problemType" in metadata else None,
             "question_title": metadata["label:metadata"][self.class_title_idx]["title"],
             "question_description": metadata["label:metadata"][self.class_title_idx]["description"],
-            "classes": metadata["label:metadata"][self.class_title_idx]["options"]
+            "classes": metadata["label:metadata"][self.class_title_idx]["options"],
+            "reduce_zero_label": self.reduce_zero_label
         }
 
         vec_path_list = [f"{self.vector_data_path}/{vec_file}" for vec_file in metadata["dataset"][self.split]]
 
         pool = Pool(16)
         self.data_list = list(tqdm(pool.imap(self.load_vector_file, vec_path_list), total=len(vec_path_list)))
         pool.close()
```

### Comparing `geolibs-0.0.1/geolibs/engine_cocometric.py` & `geolibs-0.0.2/geolibs/engine_cocometric.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.1/geolibs/enginelogger_hook.py` & `geolibs-0.0.2/geolibs/enginelogger_hook.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.1/geolibs/misc.py` & `geolibs-0.0.2/geolibs/misc.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.1/pyproject.toml` & `geolibs-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geolibs"
-version = "v0.0.1"
+version = "v0.0.2"
 description = "A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development."
 authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "geolibs"}]
 classifiers = [
     'Intended Audience :: Developers',
@@ -20,20 +20,14 @@
 numpy = "1.24.3"
 prettytable = "3.7.0"
 granular-engine = "^0.2.4"
 rasterio = "1.3.6"
 tqdm = "4.65.0"
 shapely = "2.0.1"
 albumentations = "1.3.0"
-torch = "2.0.0"
-torchvision = "0.15.1"
-mmengine = ">=0.6.0"
-mmcv = ">=2.0.0rc4,<2.1.0"
-mmdet = ">=3.0.0rc6,<3.1.0"
-mmyolo = "0.5.0"
 
 [tool.poetry.dev-dependencies]
 pip = "^21.1.3"
 beautifulsoup4 = "^4.10.0"
 bump2version = "^1.0.1"
 watchdog = "^2.1.3"
 flake8 = "^3.9.2"
```

### Comparing `geolibs-0.0.1/PKG-INFO` & `geolibs-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolibs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development.
 Home-page: https://github.com/granularai/geolibs
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Intended Audience :: Developers
@@ -15,38 +15,39 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: albumentations (==1.3.0)
 Requires-Dist: granular-engine (>=0.2.4,<0.3.0)
-Requires-Dist: mmcv (>=2.0.0rc4,<2.1.0)
-Requires-Dist: mmdet (>=3.0.0rc6,<3.1.0)
-Requires-Dist: mmengine (>=0.6.0)
-Requires-Dist: mmyolo (==0.5.0)
 Requires-Dist: numpy (==1.24.3)
 Requires-Dist: prettytable (==3.7.0)
 Requires-Dist: rasterio (==1.3.6)
 Requires-Dist: shapely (==2.0.1)
-Requires-Dist: torch (==2.0.0)
-Requires-Dist: torchvision (==0.15.1)
 Requires-Dist: tqdm (==4.65.0)
 Project-URL: Repository, https://github.com/granularai/geolibs
 Description-Content-Type: text/x-rst
 
 Engine
 ======
 
 A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development.
 
 Installation
 ------------
 
 .. code:: shell
 
+   pip install torch torchvision
+   pip install -U openmim
+   mim install "mmengine>=0.6.0"
+   mim install "mmcv>=2.0.0rc4,<2.1.0"
+   mim install "mmdet>=3.0.0rc6,<3.1.0"
+   mim install "mmyolo"
+   mim install "mmsegmentation>=1.0.0"
    pip install geolibs
 
 License
 -------
 
 GPLv3
```

