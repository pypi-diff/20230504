# Comparing `tmp/ome-zarr-0.6.1.tar.gz` & `tmp/ome-zarr-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ome-zarr-0.6.1.tar", last modified: Wed Oct 26 08:53:30 2022, max compression
+gzip compressed data, was "ome-zarr-0.7.0.tar", last modified: Thu May  4 09:13:49 2023, max compression
```

## Comparing `ome-zarr-0.6.1.tar` & `ome-zarr-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 08:53:30.971494 ome-zarr-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2022-10-26 08:53:30.971494 ome-zarr-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 08:53:30.971494 ome-zarr-0.6.1/ome_zarr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4221 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/axes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5608 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5360 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5912 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    11642 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     6261 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    24261 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     9104 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/scale.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4068 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    30626 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/ome_zarr/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 08:53:30.971494 ome-zarr-0.6.1/ome_zarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2022-10-26 08:53:30.000000 ome-zarr-0.6.1/ome_zarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-10-26 08:53:30.000000 ome-zarr-0.6.1/ome_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 08:53:30.000000 ome-zarr-0.6.1/ome_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-26 08:53:30.000000 ome-zarr-0.6.1/ome_zarr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-10-26 08:53:30.000000 ome-zarr-0.6.1/ome_zarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-26 08:53:30.000000 ome-zarr-0.6.1/ome_zarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 08:53:30.971494 ome-zarr-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-10-26 08:53:24.000000 ome-zarr-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/ome_zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/axes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5601 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24047 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/ome_zarr/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/ome_zarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 09:13:49.000000 ome-zarr-0.7.0/ome_zarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:13:49.217231 ome-zarr-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-04 09:13:47.000000 ome-zarr-0.7.0/setup.py
```

### Comparing `ome-zarr-0.6.1/LICENSE` & `ome-zarr-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.6.1/PKG-INFO` & `ome-zarr-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: ome-zarr
-Version: 0.6.1
+Version: 0.7.0
 Summary: Implementation of images in Zarr files.
 Home-page: https://github.com/ome/ome-zarr-py
 Author: The Open Microscopy Team
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -28,15 +30,15 @@
 Documentation
 -------------
 
 Documentation will be automatically built with `readthedocs`.
 
 It can be built locally with::
 
-    $ pip install spinx
+    $ pip install sphinx
     $ sphinx-build -b html docs/source/ docs/build/html
 
 Tests
 -----
 
 Tests can be run locally via `tox` with::
 
@@ -90,7 +92,9 @@
     :scale: 100%
     :target: https://ome-zarr.readthedocs.io/en/stable/?badge=stable
 
 .. |coverage| image:: https://codecov.io/gh/ome/ome-zarr-py/branch/master/graph/badge.svg
     :alt: Test coverage
     :scale: 100%
     :target: https://codecov.io/gh/ome/ome-zarr-py
+
+
```

### Comparing `ome-zarr-0.6.1/README.rst` & `ome-zarr-0.7.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Documentation
 -------------
 
 Documentation will be automatically built with `readthedocs`.
 
 It can be built locally with::
 
-    $ pip install spinx
+    $ pip install sphinx
     $ sphinx-build -b html docs/source/ docs/build/html
 
 Tests
 -----
 
 Tests can be run locally via `tox` with::
```

### Comparing `ome-zarr-0.6.1/ome_zarr/axes.py` & `ome-zarr-0.7.0/ome_zarr/axes.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         for axis in self.axes:
             if "name" not in axis:
                 raise ValueError("Axis Dict %s has no 'name'" % axis)
             axes_names.append(axis["name"])
         return axes_names
 
     def _validate_03(self) -> None:
-
         val_axes = tuple(self._get_names())
         if len(val_axes) == 2:
             if val_axes != ("y", "x"):
                 raise ValueError(f"2D data must have axes ('y', 'x') {val_axes}")
         elif len(val_axes) == 3:
             if val_axes not in [("z", "y", "x"), ("c", "y", "x"), ("t", "y", "x")]:
                 raise ValueError(
```

### Comparing `ome-zarr-0.6.1/ome_zarr/cli.py` & `ome-zarr-0.7.0/ome_zarr/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     """Adds csv data to labels properties"""
 
     print("csv_to_labels", args.csv_path, args.zarr_path)
 
     csv_to_zarr(args.csv_path, args.csv_id, args.csv_keys, args.zarr_path, args.zarr_id)
 
 
-def main(args: List[str] = None) -> None:
+def main(args: List[str]) -> None:
     """Run appropriate function with argparse arguments, handling errors."""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-v",
         "--verbose",
         action="count",
         default=0,
```

### Comparing `ome-zarr-0.6.1/ome_zarr/conversions.py` & `ome-zarr-0.7.0/ome_zarr/conversions.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.6.1/ome_zarr/csv.py` & `ome-zarr-0.7.0/ome_zarr/csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,14 @@
             labels_paths.append(
                 os.path.join(zarr_path, w["path"], field, "labels", "0")
             )
     else:
         labels_paths.append(os.path.join(zarr_path, "labels", "0"))
 
     for path_to_labels in labels_paths:
-
         label_group = zarr_open(path_to_labels)
         attrs = label_group.attrs.asdict()
         properties = attrs.get("image-label", {}).get("properties")
         if properties is None:
             continue
 
         for props_dict in properties:
```

### Comparing `ome-zarr-0.6.1/ome_zarr/dask_utils.py` & `ome-zarr-0.7.0/ome_zarr/dask_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,22 +29,34 @@
     # blocks size of full numbers.
     better_chunksize = tuple(
         np.maximum(1, np.round(np.array(image.chunksize) * factors) / factors).astype(
             int
         )
     )
     image_prepared = image.rechunk(better_chunksize)
+
+    # If E.g. we resize image from 6675 by 0.5 to 3337, factor is 0.49992509 so each
+    # chunk of size e.g. 1000 will resize to 499. When assumbled into a new array, the
+    # array will now be of size 3331 instead of 3337 because each of 6 chunks was
+    # smaller by 1. When we compute() this, dask will read 6 chunks of 1000 and expect
+    # last chunk to be 337 but instead it will only be 331.
+    # So we use ceil() here (and in resize_block) to round 499.925 up to chunk of 500
     block_output_shape = tuple(
-        np.floor(np.array(better_chunksize) * factors).astype(int)
+        np.ceil(np.array(better_chunksize) * factors).astype(int)
     )
 
     # Map overlap
     def resize_block(image_block: da.Array, block_info: dict) -> da.Array:
+        # if the input block is smaller than a 'regular' chunk (e.g. edge of image)
+        # we need to calculate target size for each chunk...
+        chunk_output_shape = tuple(
+            np.ceil(np.array(image_block.shape) * factors).astype(int)
+        )
         return skimage.transform.resize(
-            image_block, block_output_shape, *args, **kwargs
+            image_block, chunk_output_shape, *args, **kwargs
         ).astype(image_block.dtype)
 
     output_slices = tuple(slice(0, d) for d in output_shape)
     output = da.map_blocks(
         resize_block, image_prepared, dtype=image.dtype, chunks=block_output_shape
     )[output_slices]
     return output.rechunk(image.chunksize).astype(image.dtype)
```

### Comparing `ome-zarr-0.6.1/ome_zarr/data.py` & `ome-zarr-0.7.0/ome_zarr/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Functions for generating synthetic data."""
 from random import randrange
-from typing import Callable, List, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import zarr
 from scipy.ndimage import zoom
 from skimage import data
 from skimage.filters import threshold_otsu
 from skimage.measure import label
@@ -99,16 +99,16 @@
 
 
 def create_zarr(
     zarr_directory: str,
     method: Callable[..., Tuple[List, List]] = coins,
     label_name: str = "coins",
     fmt: Format = CurrentFormat(),
-    chunks: Union[Tuple, List] = None,
-) -> None:
+    chunks: Optional[Union[Tuple, List]] = None,
+) -> zarr.Group:
     """Generate a synthetic image pyramid with labels."""
     pyramid, labels = method()
 
     loc = parse_url(zarr_directory, mode="w")
     assert loc
     grp = zarr.group(loc.store)
     axes = None
@@ -166,15 +166,14 @@
                 },
             ],
             "rdefs": {"model": "color"},
         }
     grp.attrs["omero"] = image_data
 
     if labels:
-
         labels_grp = grp.create_group("labels")
         labels_grp.attrs["labels"] = [label_name]
 
         label_grp = labels_grp.create_group(label_name)
         if axes is not None:
             # remove channel axis for masks
             axes = axes.replace("c", "")
@@ -188,7 +187,9 @@
             properties.append({"label-value": x, "class": f"class {x}"})
         label_grp.attrs["image-label"] = {
             "version": fmt.version,
             "colors": colors,
             "properties": properties,
             "source": {"image": "../../"},
         }
+
+    return grp
```

### Comparing `ome-zarr-0.6.1/ome_zarr/format.py` & `ome-zarr-0.7.0/ome_zarr/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 from zarr.storage import FSStore
 
 LOGGER = logging.getLogger("ome_zarr.format")
 
 
 def format_from_version(version: str) -> "Format":
-
     for fmt in format_implementations():
-
         # Support floating-point versions like `0.2`
         if isinstance(version, float):
             version = str(version)
 
         if fmt.version == version:
             return fmt
     raise ValueError(f"Version {version} not recognized")
@@ -106,15 +104,15 @@
         raise NotImplementedError()
 
     @abstractmethod
     def validate_coordinate_transformations(
         self,
         ndim: int,
         nlevels: int,
-        coordinate_transformations: List[List[Dict[str, Any]]] = None,
+        coordinate_transformations: Optional[List[List[Dict[str, Any]]]] = None,
     ) -> Optional[List[List[Dict[str, Any]]]]:  # pragma: no cover
         raise NotImplementedError()
 
 
 class FormatV01(Format):
     """
     Initial format. (2020)
@@ -159,15 +157,15 @@
     ) -> Optional[List[List[Dict[str, Any]]]]:
         return None
 
     def validate_coordinate_transformations(
         self,
         ndim: int,
         nlevels: int,
-        coordinate_transformations: List[List[Dict[str, Any]]] = None,
+        coordinate_transformations: Optional[List[List[Dict[str, Any]]]] = None,
     ) -> None:
         return None
 
 
 class FormatV02(FormatV01):
     """
     Changelog: move to nested storage (April 2021)
@@ -254,30 +252,29 @@
             raise ValueError("%s is not defined in the plate columns", column)
         if well["columnIndex"] != columns.index(column):
             raise ValueError("Mismatching column index for %s", well)
 
     def generate_coordinate_transformations(
         self, shapes: List[tuple]
     ) -> Optional[List[List[Dict[str, Any]]]]:
-
         data_shape = shapes[0]
         coordinate_transformations: List[List[Dict[str, Any]]] = []
         # calculate minimal 'scale' transform based on pyramid dims
         for shape in shapes:
             assert len(shape) == len(data_shape)
             scale = [full / level for full, level in zip(data_shape, shape)]
             coordinate_transformations.append([{"type": "scale", "scale": scale}])
 
         return coordinate_transformations
 
     def validate_coordinate_transformations(
         self,
         ndim: int,
         nlevels: int,
-        coordinate_transformations: List[List[Dict[str, Any]]] = None,
+        coordinate_transformations: Optional[List[List[Dict[str, Any]]]] = None,
     ) -> None:
         """
         Validates that a list of dicts contains a 'scale' transformation
 
         Raises ValueError if no 'scale' found or doesn't match ndim
         :param ndim:       Number of image dimensions
         """
```

### Comparing `ome-zarr-0.6.1/ome_zarr/io.py` & `ome-zarr-0.7.0/ome_zarr/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     No assumptions about the existence of the given path string are made.
     Attempts are made to load various metadata files and cache them internally.
     """
 
     def __init__(
         self, path: Union[Path, str], mode: str = "r", fmt: Format = CurrentFormat()
     ) -> None:
-
         LOGGER.debug("ZarrLocation.__init__ path: %s, fmt: %s", path, fmt.version)
         self.__fmt = fmt
         self.__mode = mode
         if isinstance(path, Path):
             self.__path = str(path.resolve())
         elif isinstance(path, str):
             self.__path = path
```

### Comparing `ome-zarr-0.6.1/ome_zarr/reader.py` & `ome-zarr-0.7.0/ome_zarr/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,36 +273,32 @@
             if "multiscales" in zarr.root_attrs:
                 return True
         return False
 
     def __init__(self, node: Node) -> None:
         super().__init__(node)
 
-        try:
-            multiscales = self.lookup("multiscales", [])
-            version = multiscales[0].get(
-                "version", "0.1"
-            )  # should this be matched with Format.version?
-            datasets = multiscales[0]["datasets"]
-            axes = multiscales[0].get("axes")
-            fmt = format_from_version(version)
-            # Raises ValueError if not valid
-            axes_obj = Axes(axes, fmt)
-            node.metadata["axes"] = axes_obj.to_list()
-            # This will get overwritten by 'omero' metadata if present
-            node.metadata["name"] = multiscales[0].get("name")
-            paths = [d["path"] for d in datasets]
-            self.datasets: List[str] = paths
-            transformations = [d.get("coordinateTransformations") for d in datasets]
-            if any(trans is not None for trans in transformations):
-                node.metadata["coordinateTransformations"] = transformations
-            LOGGER.info("datasets %s", datasets)
-        except Exception:
-            LOGGER.exception("Failed to parse multiscale metadata")
-            return  # EARLY EXIT
+        multiscales = self.lookup("multiscales", [])
+        version = multiscales[0].get(
+            "version", "0.1"
+        )  # should this be matched with Format.version?
+        datasets = multiscales[0]["datasets"]
+        axes = multiscales[0].get("axes")
+        fmt = format_from_version(version)
+        # Raises ValueError if not valid
+        axes_obj = Axes(axes, fmt)
+        node.metadata["axes"] = axes_obj.to_list()
+        # This will get overwritten by 'omero' metadata if present
+        node.metadata["name"] = multiscales[0].get("name")
+        paths = [d["path"] for d in datasets]
+        self.datasets: List[str] = paths
+        transformations = [d.get("coordinateTransformations") for d in datasets]
+        if any(trans is not None for trans in transformations):
+            node.metadata["coordinateTransformations"] = transformations
+        LOGGER.info("datasets %s", datasets)
 
         for resolution in self.datasets:
             data: da.core.Array = self.array(resolution, version)
             chunk_sizes = [
                 str(c[0]) + (" (+ %s)" % c[-1] if c[-1] != c[0] else "")
                 for c in data.chunks
             ]
@@ -624,15 +620,14 @@
         assert zarr.exists()
         self.zarr = zarr
         self.seen: List[ZarrLocation] = [zarr]
 
     def __call__(self) -> Iterator[Node]:
         node = Node(self.zarr, self)
         if node.specs:  # Something has matched
-
             LOGGER.debug("treating %s as ome-zarr", self.zarr)
             yield from self.descend(node)
 
             # TODO: API thoughts for the Spec type
             # - ask for recursion or not
             # - ask for "provides data", "overrides data"
 
@@ -642,15 +637,14 @@
             yield node
 
         else:
             LOGGER.debug("ignoring %s", self.zarr)
             # yield nothing
 
     def descend(self, node: Node, depth: int = 0) -> Iterator[Node]:
-
         for pre_node in node.pre_nodes:
             yield from self.descend(pre_node, depth + 1)
 
         LOGGER.debug("returning %s", node)
         yield node
 
         for post_node in node.post_nodes:
```

### Comparing `ome-zarr-0.6.1/ome_zarr/scale.py` & `ome-zarr-0.7.0/ome_zarr/scale.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.6.1/ome_zarr/utils.py` & `ome-zarr-0.7.0/ome_zarr/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     All :class:`Nodes <ome_utils.reader.Node>` that are found from the given path will
     be visited recursively.
     """
     zarr = parse_url(path)
     assert zarr, f"not a zarr: {zarr}"
     reader = Reader(zarr)
     for node in reader():
-
         if not node.specs:
             print(f"not an ome-zarr node: {node}")
             continue
 
         print(node)
         print(" - metadata")
         for spec in node.specs:
@@ -69,15 +68,14 @@
     assert not root_path.exists(), f"{root_path} already exists!"
     print("downloading...")
     for path in paths:
         print("  ", Path(*path))
     print(f"to {output_dir}")
 
     for path, node in sorted(zip(paths, nodes)):
-
         target_path = output_path / Path(*path)
         target_path.mkdir(parents=True)
 
         with (target_path / ".zgroup").open("w") as f:
             f.write(json.dumps(node.zarr.zgroup))
         with (target_path / ".zattrs").open("w") as f:
             metadata: JSONDict = {}
```

### Comparing `ome-zarr-0.6.1/ome_zarr/writer.py` & `ome-zarr-0.7.0/ome_zarr/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 LOGGER = logging.getLogger("ome_zarr.writer")
 
 ListOfArrayLike = Union[List[da.Array], List[np.ndarray]]
 ArrayLike = Union[da.Array, np.ndarray]
 
 
 def _get_valid_axes(
-    ndim: int = None,
-    axes: Union[str, List[str], List[Dict[str, str]]] = None,
+    ndim: Optional[int] = None,
+    axes: Optional[Union[str, List[str], List[Dict[str, str]]]] = None,
     fmt: Format = CurrentFormat(),
 ) -> Union[None, List[str], List[Dict[str, str]]]:
     """Returns list of axes valid for fmt.version or raise exception if invalid"""
 
     if fmt.version in ("0.1", "0.2"):
         if axes is not None:
             LOGGER.info("axes ignored for version 0.1 or 0.2")
@@ -60,15 +60,14 @@
 
     return axes_obj.to_list(fmt)
 
 
 def _validate_well_images(
     images: List[Union[str, dict]], fmt: Format = CurrentFormat()
 ) -> List[dict]:
-
     VALID_KEYS = [
         "acquisition",
         "path",
     ]
     validated_images = []
     for image in images:
         if isinstance(image, str):
@@ -87,15 +86,14 @@
             raise ValueError(f"Unrecognized type for {image}")
     return validated_images
 
 
 def _validate_plate_acquisitions(
     acquisitions: List[Dict], fmt: Format = CurrentFormat()
 ) -> List[Dict]:
-
     VALID_KEYS = [
         "id",
         "name",
         "maximumfieldcount",
         "description",
         "starttime",
         "endtime",
@@ -113,29 +111,27 @@
     return acquisitions
 
 
 def _validate_plate_rows_columns(
     rows_or_columns: List[str],
     fmt: Format = CurrentFormat(),
 ) -> List[dict]:
-
     if len(set(rows_or_columns)) != len(rows_or_columns):
         raise ValueError(f"{rows_or_columns} must contain unique elements")
     validated_list = []
     for element in rows_or_columns:
         if not element.isalnum():
             raise ValueError(f"{element} must contain alphanumeric characters")
         validated_list.append({"name": str(element)})
     return validated_list
 
 
 def _validate_datasets(
     datasets: List[dict], dims: int, fmt: Format = CurrentFormat()
 ) -> List[Dict]:
-
     if datasets is None or len(datasets) == 0:
         raise ValueError("Empty datasets list")
     transformations = []
     for dataset in datasets:
         if isinstance(dataset, dict):
             if not dataset.get("path"):
                 raise ValueError("no 'path' in dataset")
@@ -152,15 +148,14 @@
 
 def _validate_plate_wells(
     wells: List[Union[str, dict]],
     rows: List[str],
     columns: List[str],
     fmt: Format = CurrentFormat(),
 ) -> List[dict]:
-
     validated_wells = []
     if wells is None or len(wells) == 0:
         raise ValueError("Empty wells list")
     for well in wells:
         if isinstance(well, str):
             well_dict = fmt.generate_well_dict(well, rows, columns)
             fmt.validate_well_dict(well_dict, rows, columns)
@@ -172,22 +167,23 @@
             raise ValueError(f"Unrecognized type for {well}")
     return validated_wells
 
 
 def write_multiscale(
     pyramid: ListOfArrayLike,
     group: zarr.Group,
-    chunks: Union[Tuple[Any, ...], int] = None,
+    chunks: Optional[Union[Tuple[Any, ...], int]] = None,
     fmt: Format = CurrentFormat(),
-    axes: Union[str, List[str], List[Dict[str, str]]] = None,
-    coordinate_transformations: List[List[Dict[str, Any]]] = None,
-    storage_options: Union[JSONDict, List[JSONDict]] = None,
-    name: str = None,
+    axes: Optional[Union[str, List[str], List[Dict[str, str]]]] = None,
+    coordinate_transformations: Optional[List[List[Dict[str, Any]]]] = None,
+    storage_options: Optional[Union[JSONDict, List[JSONDict]]] = None,
+    name: Optional[str] = None,
+    compute: Optional[bool] = True,
     **metadata: Union[str, JSONDict, List[JSONDict]],
-) -> None:
+) -> List:
     """
     Write a pyramid with multiscale metadata to disk.
 
     :type pyramid: list of :class:`numpy.ndarray` or :class:`dask.array.Array`
     :param pyramid:
         The image data to save. Largest level first. All image arrays MUST be up to
         5-dimensional with dimensions ordered (t, c, z, y, x)
@@ -215,17 +211,25 @@
         'scale' transform.
     :type storage_options: dict or list of dict, optional
     :param storage_options:
         Options to be passed on to the storage backend.
         A list would need to match the number of datasets in a multiresolution pyramid.
         One can provide different chunk size for each level of a pyramid using this
         option.
+    :param compute:
+        If true compute immediately otherwise a list of :class:`dask.delayed.Delayed`
+        is returned.
+    :return:
+        Empty list if the compute flag is True, otherwise it returns a list of
+        :class:`dask.delayed.Delayed` representing the value to be computed by
+        dask.
     """
     dims = len(pyramid[0].shape)
     axes = _get_valid_axes(dims, axes, fmt)
+    dask_delayed = []
 
     if chunks is not None:
         msg = """The 'chunks' argument is deprecated and will be removed in version 0.5.
 Please use the 'storage_options' argument instead."""
         warnings.warn(msg, DeprecationWarning)
 
     datasets: List[dict] = []
@@ -241,21 +245,27 @@
         if chunks_opt is not None:
             chunks_opt = _retuple(chunks_opt, data.shape)
 
         if isinstance(data, da.Array):
             if chunks_opt is not None:
                 data = da.array(data).rechunk(chunks=chunks_opt)
                 options["chunks"] = chunks_opt
-            da.to_zarr(
+            da_delayed = da.to_zarr(
                 arr=data,
                 url=group.store,
                 component=str(Path(group.path, str(path))),
                 storage_options=options,
-                compressor=options.get("compressor"),
+                compressor=options.get("compressor", zarr.storage.default_compressor),
+                dimension_separator=group._store._dimension_separator,
+                compute=compute,
             )
+
+            if not compute:
+                dask_delayed.append(da_delayed)
+
         else:
             group.create_dataset(str(path), data=data, chunks=chunks_opt, **options)
 
         datasets.append({"path": str(path)})
 
     if coordinate_transformations is None:
         shapes = [data.shape for data in pyramid]
@@ -267,21 +277,23 @@
     )
     if coordinate_transformations is not None:
         for dataset, transform in zip(datasets, coordinate_transformations):
             dataset["coordinateTransformations"] = transform
 
     write_multiscales_metadata(group, datasets, fmt, axes, name, **metadata)
 
+    return dask_delayed
+
 
 def write_multiscales_metadata(
     group: zarr.Group,
     datasets: List[dict],
     fmt: Format = CurrentFormat(),
-    axes: Union[str, List[str], List[Dict[str, str]]] = None,
-    name: str = None,
+    axes: Optional[Union[str, List[str], List[Dict[str, str]]]] = None,
+    name: Optional[str] = None,
     **metadata: Union[str, JSONDict, List[JSONDict]],
 ) -> None:
     """
     Write the multiscales metadata in the group.
 
     :type group: :class:`zarr.hierarchy.Group`
     :param group: The group within the zarr store to write the metadata in.
@@ -329,17 +341,17 @@
 
 def write_plate_metadata(
     group: zarr.Group,
     rows: List[str],
     columns: List[str],
     wells: List[Union[str, dict]],
     fmt: Format = CurrentFormat(),
-    acquisitions: List[dict] = None,
-    field_count: int = None,
-    name: str = None,
+    acquisitions: Optional[List[dict]] = None,
+    field_count: Optional[int] = None,
+    name: Optional[str] = None,
 ) -> None:
     """
     Write the plate metadata in the group.
 
     :type group: :class:`zarr.hierarchy.Group`
     :param group: The group within the zarr store to write the metadata in.
     :type rows: list of str
@@ -400,21 +412,22 @@
     group.attrs["well"] = well
 
 
 def write_image(
     image: ArrayLike,
     group: zarr.Group,
     scaler: Scaler = Scaler(),
-    chunks: Union[Tuple[Any, ...], int] = None,
+    chunks: Optional[Union[Tuple[Any, ...], int]] = None,
     fmt: Format = CurrentFormat(),
-    axes: Union[str, List[str], List[Dict[str, str]]] = None,
-    coordinate_transformations: List[List[Dict[str, Any]]] = None,
-    storage_options: Union[JSONDict, List[JSONDict]] = None,
+    axes: Optional[Union[str, List[str], List[Dict[str, str]]]] = None,
+    coordinate_transformations: Optional[List[List[Dict[str, Any]]]] = None,
+    storage_options: Optional[Union[JSONDict, List[JSONDict]]] = None,
+    compute: Optional[bool] = True,
     **metadata: Union[str, JSONDict, List[JSONDict]],
-) -> None:
+) -> List:
     """Writes an image to the zarr store according to ome-zarr specification
 
     :type image: :class:`numpy.ndarray` or `dask.array.Array`
     :param image:
       The image data to save. A downsampling of the data will be computed
       if the scaler argument is non-None.
       Image array MUST be up to 5-dimensional with dimensions
@@ -446,42 +459,55 @@
       Each list of dicts are added to each datasets in order.
     :type storage_options: dict or list of dict, optional
     :param storage_options:
         Options to be passed on to the storage backend.
         A list would need to match the number of datasets in a multiresolution pyramid.
         One can provide different chunk size for each level of a pyramid using this
         option.
+    :param compute:
+        If true compute immediately otherwise a list of :class:`dask.delayed.Delayed`
+        is returned.
+    :return:
+        Empty list if the compute flag is True, otherwise it returns a list of
+        :class:`dask.delayed.Delayed` representing the value to be computed by
+        dask.
     """
+    dask_delayed_jobs = []
+
     if isinstance(image, da.Array):
-        _write_dask_image(
+        dask_delayed_jobs = _write_dask_image(
             image,
             group,
             scaler,
             chunks=chunks,
             fmt=fmt,
             axes=axes,
             coordinate_transformations=coordinate_transformations,
             storage_options=storage_options,
             name=None,
+            compute=compute,
             **metadata,
         )
     else:
         mip, axes = _create_mip(image, fmt, scaler, axes)
-        write_multiscale(
+        dask_delayed_jobs = write_multiscale(
             mip,
             group,
             chunks=chunks,
             fmt=fmt,
             axes=axes,
             coordinate_transformations=coordinate_transformations,
             storage_options=storage_options,
             name=None,
+            compute=compute,
             **metadata,
         )
 
+    return dask_delayed_jobs
+
 
 def _resolve_storage_options(
     storage_options: Union[JSONDict, List[JSONDict], None], path: int
 ) -> JSONDict:
     options = {}
     if storage_options:
         options = (
@@ -492,23 +518,23 @@
     return options
 
 
 def _write_dask_image(
     image: da.Array,
     group: zarr.Group,
     scaler: Scaler = Scaler(),
-    chunks: Union[Tuple[Any, ...], int] = None,
+    chunks: Optional[Union[Tuple[Any, ...], int]] = None,
     fmt: Format = CurrentFormat(),
-    axes: Union[str, List[str], List[Dict[str, str]]] = None,
-    coordinate_transformations: List[List[Dict[str, Any]]] = None,
-    storage_options: Union[JSONDict, List[JSONDict]] = None,
-    name: str = None,
+    axes: Optional[Union[str, List[str], List[Dict[str, str]]]] = None,
+    coordinate_transformations: Optional[List[List[Dict[str, Any]]]] = None,
+    storage_options: Optional[Union[JSONDict, List[JSONDict]]] = None,
+    name: Optional[str] = None,
+    compute: Optional[bool] = True,
     **metadata: Union[str, JSONDict, List[JSONDict]],
-) -> None:
-
+) -> List:
     if fmt.version in ("0.1", "0.2"):
         # v0.1 and v0.2 are strictly 5D
         shape_5d: Tuple[Any, ...] = (*(1,) * (5 - image.ndim), *image.shape)
         image = image.reshape(shape_5d)
         # and we don't need axes
         axes = None
 
@@ -553,20 +579,24 @@
         delayed.append(
             da.to_zarr(
                 arr=image,
                 url=group.store,
                 component=str(Path(group.path, str(path))),
                 storage_options=options,
                 compute=False,
-                compressor=options.get("compressor"),
+                compressor=options.get("compressor", zarr.storage.default_compressor),
+                dimension_separator=group._store._dimension_separator,
             )
         )
         datasets.append({"path": str(path)})
 
-    da.compute(*delayed)
+    # Computing delayed jobs if necessary
+    if compute:
+        da.compute(*delayed)
+        delayed = []
 
     if coordinate_transformations is None:
         # shapes = [data.shape for data in delayed]
         coordinate_transformations = fmt.generate_coordinate_transformations(shapes)
 
     # we validate again later, but this catches length mismatch before zip(datasets...)
     fmt.validate_coordinate_transformations(
@@ -574,20 +604,22 @@
     )
     if coordinate_transformations is not None:
         for dataset, transform in zip(datasets, coordinate_transformations):
             dataset["coordinateTransformations"] = transform
 
     write_multiscales_metadata(group, datasets, fmt, axes, name, **metadata)
 
+    return delayed
+
 
 def write_label_metadata(
     group: zarr.Group,
     name: str,
-    colors: List[JSONDict] = None,
-    properties: List[JSONDict] = None,
+    colors: Optional[List[JSONDict]] = None,
+    properties: Optional[List[JSONDict]] = None,
     fmt: Format = CurrentFormat(),
     **metadata: Union[List[JSONDict], JSONDict, str],
 ) -> None:
     """
     Write image-label metadata to the group.
 
     The label data must have been written to a sub-group,
@@ -627,22 +659,23 @@
     group.attrs["labels"] = label_list
 
 
 def write_multiscale_labels(
     pyramid: List,
     group: zarr.Group,
     name: str,
-    chunks: Union[Tuple[Any, ...], int] = None,
+    chunks: Optional[Union[Tuple[Any, ...], int]] = None,
     fmt: Format = CurrentFormat(),
-    axes: Union[str, List[str], List[Dict[str, str]]] = None,
-    coordinate_transformations: List[List[Dict[str, Any]]] = None,
-    storage_options: Union[JSONDict, List[JSONDict]] = None,
-    label_metadata: JSONDict = None,
+    axes: Optional[Union[str, List[str], List[Dict[str, str]]]] = None,
+    coordinate_transformations: Optional[List[List[Dict[str, Any]]]] = None,
+    storage_options: Optional[Union[JSONDict, List[JSONDict]]] = None,
+    label_metadata: Optional[JSONDict] = None,
+    compute: Optional[bool] = True,
     **metadata: JSONDict,
-) -> None:
+) -> List:
     """
     Write pyramidal image labels to disk.
 
     Including the multiscales and image-label metadata.
     Creates the label data in the sub-group "labels/{name}"
 
     :type pyramid: list of :class:`numpy.ndarray`
@@ -678,48 +711,59 @@
         Options to be passed on to the storage backend.
         A list would need to match the number of datasets in a multiresolution pyramid.
         One can provide different chunk size for each level of a pyramid using this
         option.
     :type label_metadata: dict, optional
     :param label_metadata:
       Image label metadata. See :meth:`write_label_metadata` for details
+    :param compute:
+        If true compute immediately otherwise a list of :class:`dask.delayed.Delayed`
+        is returned.
+    :return:
+        Empty list if the compute flag is True, otherwise it returns a list of
+        :class:`dask.delayed.Delayed` representing the value to be computed by
+        dask.
     """
     sub_group = group.require_group(f"labels/{name}")
-    write_multiscale(
+    dask_delayed_jobs = write_multiscale(
         pyramid,
         sub_group,
         chunks=chunks,
         fmt=fmt,
         axes=axes,
         coordinate_transformations=coordinate_transformations,
         storage_options=storage_options,
         name=name,
+        compute=compute,
         **metadata,
     )
     write_label_metadata(
         group["labels"],
         name,
         fmt=fmt,
         **({} if label_metadata is None else label_metadata),
     )
 
+    return dask_delayed_jobs
+
 
 def write_labels(
     labels: Union[np.ndarray, da.Array],
     group: zarr.Group,
     name: str,
     scaler: Scaler = Scaler(),
-    chunks: Union[Tuple[Any, ...], int] = None,
+    chunks: Optional[Union[Tuple[Any, ...], int]] = None,
     fmt: Format = CurrentFormat(),
-    axes: Union[str, List[str], List[Dict[str, str]]] = None,
-    coordinate_transformations: List[List[Dict[str, Any]]] = None,
-    storage_options: Union[JSONDict, List[JSONDict]] = None,
-    label_metadata: JSONDict = None,
+    axes: Optional[Union[str, List[str], List[Dict[str, str]]]] = None,
+    coordinate_transformations: Optional[List[List[Dict[str, Any]]]] = None,
+    storage_options: Optional[Union[JSONDict, List[JSONDict]]] = None,
+    label_metadata: Optional[JSONDict] = None,
+    compute: Optional[bool] = True,
     **metadata: JSONDict,
-) -> None:
+) -> List:
     """
     Write image label data to disk.
 
     Including the multiscales and image-label metadata.
     Creates the label data in the sub-group "labels/{name}"
 
     :type labels: :class:`numpy.ndarray`
@@ -760,49 +804,62 @@
         Options to be passed on to the storage backend.
         A list would need to match the number of datasets in a multiresolution pyramid.
         One can provide different chunk size for each level of a pyramid using this
         option.
     :type label_metadata: dict, optional
     :param label_metadata:
       Image label metadata. See :meth:`write_label_metadata` for details
+    :param compute:
+        If true compute immediately otherwise a list of :class:`dask.delayed.Delayed`
+        is returned.
+    :return:
+        Empty list if the compute flag is True, otherwise it returns a list of
+        :class:`dask.delayed.Delayed` representing the value to be computed by
+        dask.
     """
     sub_group = group.require_group(f"labels/{name}")
+    dask_delayed_jobs = []
+
     if isinstance(labels, da.Array):
-        _write_dask_image(
+        dask_delayed_jobs = _write_dask_image(
             labels,
             sub_group,
             scaler,
             chunks=chunks,
             fmt=fmt,
             axes=axes,
             coordinate_transformations=coordinate_transformations,
             storage_options=storage_options,
             name=name,
+            compute=compute,
             **metadata,
         )
     else:
         mip, axes = _create_mip(labels, fmt, scaler, axes)
-        write_multiscale(
+        dask_delayed_jobs = write_multiscale(
             mip,
             sub_group,
             chunks=chunks,
             fmt=fmt,
             axes=axes,
             coordinate_transformations=coordinate_transformations,
             storage_options=storage_options,
             name=name,
+            compute=compute,
             **metadata,
         )
     write_label_metadata(
         group=group["labels"],
         name=name,
         fmt=fmt,
         **({} if label_metadata is None else label_metadata),
     )
 
+    return dask_delayed_jobs
+
 
 def _create_mip(
     image: np.ndarray,
     fmt: Format,
     scaler: Scaler,
     axes: Optional[Union[str, List[str], List[Dict[str, str]]]],
 ) -> Tuple[List[np.ndarray], Optional[Union[str, List[str], List[Dict[str, str]]]]]:
```

### Comparing `ome-zarr-0.6.1/ome_zarr.egg-info/PKG-INFO` & `ome-zarr-0.7.0/ome_zarr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: ome-zarr
-Version: 0.6.1
+Version: 0.7.0
 Summary: Implementation of images in Zarr files.
 Home-page: https://github.com/ome/ome-zarr-py
 Author: The Open Microscopy Team
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -28,15 +30,15 @@
 Documentation
 -------------
 
 Documentation will be automatically built with `readthedocs`.
 
 It can be built locally with::
 
-    $ pip install spinx
+    $ pip install sphinx
     $ sphinx-build -b html docs/source/ docs/build/html
 
 Tests
 -----
 
 Tests can be run locally via `tox` with::
 
@@ -90,7 +92,9 @@
     :scale: 100%
     :target: https://ome-zarr.readthedocs.io/en/stable/?badge=stable
 
 .. |coverage| image:: https://codecov.io/gh/ome/ome-zarr-py/branch/master/graph/badge.svg
     :alt: Test coverage
     :scale: 100%
     :target: https://codecov.io/gh/ome/ome-zarr-py
+
+
```

### Comparing `ome-zarr-0.6.1/setup.py` & `ome-zarr-0.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 
 
 install_requires: List[List[str]] = []
 install_requires += (["dataclasses;python_version<'3.7'"],)
 install_requires += (["tifffile<2020.09.22;python_version<'3.7'"],)
 install_requires += (["numpy"],)
 install_requires += (["dask"],)
+install_requires += (["distributed"],)
 install_requires += (["zarr>=2.8.1"],)
 install_requires += (["fsspec[s3]!=2021.07.0"],)
 # See https://github.com/fsspec/filesystem_spec/issues/819
 install_requires += (["aiohttp<4"],)
 install_requires += (["requests"],)
 install_requires += (["scikit-image"],)
 install_requires += (["toolz"],)
 
 
 setup(
     name="ome-zarr",
-    version="0.6.1",
+    version="0.7.0",
     author="The Open Microscopy Team",
     url="https://github.com/ome/ome-zarr-py",
     description="Implementation of images in Zarr files.",
     long_description=read("README.rst"),
     packages=["ome_zarr"],
     py_modules=["ome_zarr"],
     python_requires=">=3.6",
```

