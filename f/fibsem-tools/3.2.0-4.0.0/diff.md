# Comparing `tmp/fibsem_tools-3.2.0.tar.gz` & `tmp/fibsem_tools-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibsem_tools-3.2.0.tar", max compression
+gzip compressed data, was "fibsem_tools-4.0.0.tar", max compression
```

## Comparing `fibsem_tools-3.2.0.tar` & `fibsem_tools-4.0.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-02-21 23:22:56.299056 fibsem_tools-3.2.0/LICENSE
--rw-r--r--   0        0        0     1397 2023-04-24 15:38:16.499953 fibsem_tools-3.2.0/pyproject.toml
--rw-r--r--   0        0        0      183 2023-03-23 18:14:36.952245 fibsem_tools-3.2.0/src/fibsem_tools/__init__.py
--rw-r--r--   0        0        0      606 2023-04-02 16:17:29.203986 fibsem_tools-3.2.0/src/fibsem_tools/cli/tiff2zarr.css
--rw-r--r--   0        0        0    13481 2023-04-02 16:17:29.204298 fibsem_tools-3.2.0/src/fibsem_tools/cli/tiff2zarr.py
--rw-r--r--   0        0        0        0 2023-03-23 18:13:14.517927 fibsem_tools-3.2.0/src/fibsem_tools/io/__init__.py
--rw-r--r--   0        0        0     9151 2023-04-24 15:38:06.907899 fibsem_tools-3.2.0/src/fibsem_tools/io/core.py
--rw-r--r--   0        0        0    13817 2023-04-02 16:17:25.433740 fibsem_tools-3.2.0/src/fibsem_tools/io/dask.py
--rw-r--r--   0        0        0    29922 2023-03-23 19:37:34.954215 fibsem_tools-3.2.0/src/fibsem_tools/io/fibsem.py
--rw-r--r--   0        0        0     2258 2023-03-23 19:35:10.739676 fibsem_tools-3.2.0/src/fibsem_tools/io/h5.py
--rw-r--r--   0        0        0     3521 2023-03-23 19:35:10.739716 fibsem_tools-3.2.0/src/fibsem_tools/io/mrc.py
--rw-r--r--   0        0        0     6759 2023-04-05 15:51:53.357061 fibsem_tools-3.2.0/src/fibsem_tools/io/multiscale.py
--rw-r--r--   0        0        0       36 2023-03-23 19:35:10.687732 fibsem_tools-3.2.0/src/fibsem_tools/io/neuroglancer.py
--rw-r--r--   0        0        0     2341 2023-03-23 19:45:26.756642 fibsem_tools-3.2.0/src/fibsem_tools/io/server.py
--rw-r--r--   0        0        0     3551 2023-03-25 02:44:53.556172 fibsem_tools-3.2.0/src/fibsem_tools/io/util.py
--rw-r--r--   0        0        0     1454 2023-04-05 15:50:28.371811 fibsem_tools-3.2.0/src/fibsem_tools/io/xr.py
--rw-r--r--   0        0        0    13187 2023-04-15 17:19:41.433351 fibsem_tools-3.2.0/src/fibsem_tools/io/zarr.py
--rw-r--r--   0        0        0        0 2023-02-21 23:22:56.301100 fibsem_tools-3.2.0/src/fibsem_tools/metadata/__init__.py
--rw-r--r--   0        0        0     3195 2023-04-05 15:51:53.357628 fibsem_tools-3.2.0/src/fibsem_tools/metadata/cosem.py
--rw-r--r--   0        0        0     3479 2023-03-22 20:52:50.925475 fibsem_tools-3.2.0/src/fibsem_tools/metadata/groundtruth.py
--rw-r--r--   0        0        0     2123 2023-03-16 20:03:20.243743 fibsem_tools-3.2.0/src/fibsem_tools/metadata/neuroglancer.py
--rw-r--r--   0        0        0     3373 2023-03-16 20:01:35.764425 fibsem_tools-3.2.0/src/fibsem_tools/metadata/transform.py
--rw-r--r--   0        0        0        0 2023-03-23 17:36:07.629685 fibsem_tools-3.2.0/src/fibsem_tools/py.typed
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 fibsem_tools-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-21 23:22:56.299056 fibsem_tools-4.0.0/LICENSE
+-rw-r--r--   0        0        0     1425 2023-05-04 18:41:40.840291 fibsem_tools-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-04-25 22:22:07.080776 fibsem_tools-4.0.0/src/fibsem_tools/__init__.py
+-rw-r--r--   0        0        0      606 2023-04-02 16:17:29.203986 fibsem_tools-4.0.0/src/fibsem_tools/cli/tiff2zarr.css
+-rw-r--r--   0        0        0    13481 2023-04-02 16:17:29.204298 fibsem_tools-4.0.0/src/fibsem_tools/cli/tiff2zarr.py
+-rw-r--r--   0        0        0        0 2023-03-23 18:13:14.517927 fibsem_tools-4.0.0/src/fibsem_tools/io/__init__.py
+-rw-r--r--   0        0        0     7427 2023-05-04 18:29:01.062775 fibsem_tools-4.0.0/src/fibsem_tools/io/core.py
+-rw-r--r--   0        0        0    13817 2023-05-04 17:46:58.084105 fibsem_tools-4.0.0/src/fibsem_tools/io/dask.py
+-rw-r--r--   0        0        0    31797 2023-05-04 18:29:01.063113 fibsem_tools-4.0.0/src/fibsem_tools/io/dat.py
+-rw-r--r--   0        0        0     2258 2023-03-23 19:35:10.739676 fibsem_tools-4.0.0/src/fibsem_tools/io/h5.py
+-rw-r--r--   0        0        0     5081 2023-05-04 18:29:01.063414 fibsem_tools-4.0.0/src/fibsem_tools/io/mrc.py
+-rw-r--r--   0        0        0     6819 2023-05-04 18:29:01.063658 fibsem_tools-4.0.0/src/fibsem_tools/io/multiscale.py
+-rw-r--r--   0        0        0       36 2023-03-23 19:35:10.687732 fibsem_tools-4.0.0/src/fibsem_tools/io/neuroglancer.py
+-rw-r--r--   0        0        0     2341 2023-03-23 19:45:26.756642 fibsem_tools-4.0.0/src/fibsem_tools/io/server.py
+-rw-r--r--   0        0        0      431 2023-05-04 18:29:01.063967 fibsem_tools-4.0.0/src/fibsem_tools/io/tif.py
+-rw-r--r--   0        0        0     4340 2023-05-04 18:29:01.064387 fibsem_tools-4.0.0/src/fibsem_tools/io/util.py
+-rw-r--r--   0        0        0     1504 2023-05-04 18:29:01.064928 fibsem_tools-4.0.0/src/fibsem_tools/io/xr.py
+-rw-r--r--   0        0        0    15179 2023-05-04 18:29:01.065422 fibsem_tools-4.0.0/src/fibsem_tools/io/zarr.py
+-rw-r--r--   0        0        0        0 2023-02-21 23:22:56.301100 fibsem_tools-4.0.0/src/fibsem_tools/metadata/__init__.py
+-rw-r--r--   0        0        0     3195 2023-05-04 17:46:58.085649 fibsem_tools-4.0.0/src/fibsem_tools/metadata/cosem.py
+-rw-r--r--   0        0        0     3479 2023-05-04 17:46:58.086178 fibsem_tools-4.0.0/src/fibsem_tools/metadata/groundtruth.py
+-rw-r--r--   0        0        0     2123 2023-03-16 20:03:20.243743 fibsem_tools-4.0.0/src/fibsem_tools/metadata/neuroglancer.py
+-rw-r--r--   0        0        0     3371 2023-05-04 18:29:01.065840 fibsem_tools-4.0.0/src/fibsem_tools/metadata/transform.py
+-rw-r--r--   0        0        0        0 2023-03-23 17:36:07.629685 fibsem_tools-4.0.0/src/fibsem_tools/py.typed
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 fibsem_tools-4.0.0/PKG-INFO
```

### Comparing `fibsem_tools-3.2.0/LICENSE` & `fibsem_tools-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.2.0/pyproject.toml` & `fibsem_tools-4.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fibsem-tools"
-version = "3.2.0"
+version = "4.0.0"
 description = "Tools for processing FIBSEM datasets"
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 distributed = ">=2021.10.0"
@@ -23,14 +23,15 @@
 tifffile = "^2023.2.28"
 pydantic-ome-ngff = "^0.2.0"
 click = "^8.1.3"
 dask = "^2023.3.2"
 textual = "^0.16.0"
 aiohttp = "^3.8.4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
+xarray-datatree = "^0.0.12"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.1.2"
 pytest-cov = "^3.0.0"
 pre-commit = "2.21.0"
 mypy = "^1.1.1"
```

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/cli/tiff2zarr.css` & `fibsem_tools-4.0.0/src/fibsem_tools/cli/tiff2zarr.css`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/cli/tiff2zarr.py` & `fibsem_tools-4.0.0/src/fibsem_tools/cli/tiff2zarr.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/io/dask.py` & `fibsem_tools-4.0.0/src/fibsem_tools/io/dask.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/io/fibsem.py` & `fibsem_tools-4.0.0/src/fibsem_tools/io/dat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Functions for reading FIB-SEM data from Harald Hess' proprietary format
 Adapted from https://github.com/janelia-cosem/FIB-SEM-Aligner/blob/master/fibsem.py
 """
-
+from __future__ import annotations
 import os
-from pathlib import Path
-from typing import Any, Iterable, Sequence, Union
+from typing import Any, Dict, Literal, Sequence, Tuple
 
 import dask.array as da
 import numpy as np
 from xarray import DataArray
 
 import warnings
 
+from fibsem_tools.io.util import AccessMode, PathLike
+from fibsem_tools.io.xr import stt_coord
+
 # This value is used to ensure that the endianness of the data is correct
 MAGIC_NUMBER = 3_555_587_570
 # This is the size of the header, in bytes. Everything beyond this number of bytes is
 # data.
 OFFSET = 1024
 
 
@@ -79,15 +81,15 @@
     def __array_finalize__(self, obj):
         # see InfoArray.__array_finalize__ for comments
         if obj is None:
             return
         self.attrs = getattr(obj, "attrs", None)
 
 
-class _DTypeDict(object):
+class _DTypeDict:
     """
     Handle dtype dict manipulations. Note: this object is deprecated and will soon be
     removed.
     """
 
     def __init__(self, names=None, formats=None, offsets=None):
         # initialize internals to empty lists
@@ -118,15 +120,15 @@
 
     @property
     def dtype(self):
         """return the dtype"""
         return np.dtype(self.dict)
 
 
-def _read_header(path):
+def read_header(path: PathLike):
     # make emtpy header to fill
     header_dtype = _DTypeDict()
     header_dtype.update(
         [
             "FileMagicNum",  # Read in magic number, should be 3555587570
             "FileVersion",  # Read in file version number
             "FileType",  # Read in file type, 1 is Zeiss Neon detectors
@@ -607,30 +609,37 @@
         header = np.fromfile(fobj, dtype=header_dtype.dtype, count=1)
         fibsem_header = FIBSEMHeader(**dict(zip(header.dtype.names, header[0])))
         fibsem_header.to_native_types()
 
     return fibsem_header
 
 
-def _read(path: Union[str, Path]) -> FIBSEMData:
+def access(path: PathLike, mode: AccessMode) -> FIBSEMData:
     """
 
-    Read a single .dat file.
+    Access a .dat file created by FIB-SEM microscopes.
 
     Parameters
     ----------
     path : string denoting a path to a .dat file
 
     Returns : an instance of FIBSEMData
     -------
 
     """
+    if mode != "r":
+        raise ValueError(
+            f"""
+        .dat files can only be opened with read-only mode (r). Got {mode} instead.
+        """
+        )
+
     # Load raw_data data file 's' or 'ieee-be.l64' Big-ian ordering, 64-bit long data
     # type
-    fibsem_header = _read_header(path)
+    fibsem_header = read_header(path)
     # read data
     shape = (
         fibsem_header.YResolution,
         fibsem_header.XResolution,
         fibsem_header.ChanNum,
     )
 
@@ -661,39 +670,14 @@
 
     # Once read into the FIBSEMData structure it will be in memory, not memmap.
     result = FIBSEMData(raw_data, fibsem_header)
     del raw_data
     return result
 
 
-def read_fibsem(path: Union[str, Path, Iterable[str], Iterable[Path]]):
-    """
-
-    Parameters
-    ----------
-    path : string or iterable of strings representing paths to .dat files.
-
-    Returns a single FIBSEMDataset or an iterable of FIBSEMDatasets, depending on
-    whether a single path or multiple paths are supplied as arguments.
-    -------
-
-    """
-    if isinstance(path, (str, Path)):
-        return _read(path)
-    elif isinstance(path, Iterable):
-        return [_read(p) for p in path]
-    else:
-        raise ValueError(
-            f"""
-            Path '{path}' must be an instance of string or pathlib.Path, or iterable of 
-            strings / pathlib.Paths
-            """
-        )
-
-
 def _convert_data(fibsem):
     """
 
     Parameters
     ----------
     fibsem
 
@@ -757,24 +741,24 @@
                             + fibsem[1] * fibsem.header.Scaling[1, 1]
                         )
         else:
             pass
     return detector_a, detector_b, scaled
 
 
-def _chunked_fibsem_loader(
+def chunked_fibsem_loader(
     filenames, channel_axis, pad_values=None, concat_axis=0, block_info=None
 ):
     """
     Load fibsem data and pad if needed. Designed to work with da.map_blocks.
     """
     idx = block_info[None]["chunk-location"]
     output_shape = block_info[None]["chunk-shape"]
     filedata = np.expand_dims(
-        np.asanyarray(read_fibsem(filenames[idx[0]])), concat_axis
+        np.asanyarray(access(filenames[idx[0]], mode="r")), concat_axis
     )
     pad_width = np.subtract(output_shape, filedata.shape)
     if np.any(pad_width):
         if not pad_values:
             raise ValueError("Data must be padded but no pad values were supplied!")
         padded = []
         pw = np.take(pad_width, [x for x in range(len(pad_width)) if x != channel_axis])
@@ -792,100 +776,191 @@
     else:
         result = filedata
     return result
 
 
 def minmax(filenames, block_info):
     idx = block_info[None]["chunk-location"][0]
-    filedata = read_fibsem(filenames[idx])
+    filedata = access(filenames[idx], mode="r")
     return np.expand_dims(np.array([[f.min(), f.max()] for f in filedata]), 0)
 
 
 def aggregate_fibsem_metadata(fnames):
-    headers = [_read_header(f) for f in fnames]
+    headers = [read_header(f) for f in fnames]
     meta, shapes, dtypes = [], [], []
     # build lists of metadata for each image
     for d in headers:
         if d.EightBit == 1:
             dtype = ">u1"
         else:
             dtype = ">i2"
         meta.append(d.__dict__)
         shapes.append((d.ChanNum, d.YResolution, d.XResolution))
         dtypes.append(dtype)
     return meta, shapes, dtypes
 
 
+# todo: make this a dataarray
 class FibsemDataset:
     def __init__(self, filenames: Sequence[str]):
         """
         Create a representation of a collection of .dat files as a single dataset.
         """
         self.filenames = filenames
         self.metadata, self.shapes, self.dtypes = aggregate_fibsem_metadata(
             self.filenames
         )
-        self.axes = {"z": 0, "c": 1, "y": 2, "x": 3}
-        self.bounding_shape = {
+        self.dims = ("c", "z", "y", "x")
+        self.shape = {
             k: v
             for k, v in zip(
                 self.axes, (len(self.filenames), *np.array(self.shapes).max(0))
             )
         }
-        self.extrema = self._get_extrema()
+        self.extrema = self.get_extrema()
         self.needs_padding = len(set(self.shapes)) > 1
-        self.grid_spacing, self.coords = self._get_grid_spacing_and_coords()
+        self.grid_spacing, self.coords = self.infer_coords()
 
-    def _get_grid_spacing_and_coords(self):
+    def infer_coords(self):
         lateral = self.metadata[0]["PixelSize"]
         axial = (
             abs((self.metadata[0]["WD"] - self.metadata[-1]["WD"]) / len(self.metadata))
             / 1e-6
         )
         grid_spacing = {"z": axial, "c": 1, "y": lateral, "x": lateral}
         coords = {
             k: np.arange(0, grid_spacing[k] * self.bounding_shape[k], grid_spacing[k])
             for k in grid_spacing
         }
         return grid_spacing, coords
 
-    def _get_extrema(self):
+    def get_extrema(self):
         all_extrema = da.map_blocks(
             minmax,
             self.filenames,
             chunks=((1,) * len(self.filenames), self.bounding_shape["c"], 2),
             dtype=self.dtypes[0],
         )
         result_data = da.stack([all_extrema.min(0)[:, 0], all_extrema.max(0)[:, 1]])
         result = DataArray(
             result_data,
             dims=("statistic", "channel"),
             coords={"statistic": ["min", "max"], "channel": [0, 1]},
         )
         return result
 
-    def to_dask(self, pad_values=None):
-        num_channels = self.bounding_shape["c"]
-        if self.needs_padding:
+
+def to_dask(
+    data: FibsemDataset | FIBSEMData,
+    chunks: Literal["auto"] | Sequence[int],
+    pad_values=None,
+):
+    if isinstance(data, FIBSEMData):
+        return da.from_array(data, chunks=chunks)
+    elif isinstance(data, FibsemDataset):
+        num_channels = data.bounding_shape["c"]
+        if data.needs_padding:
             if pad_values is None:
                 raise ValueError("Data must be padded but no pad values were supplied!")
             elif len(pad_values) != num_channels:
                 raise ValueError(
                     f"""
                     Length of pad values {pad_values} does not match the length of the
                     channel axis ({num_channels})
                     """
                 )
 
         chunks = (
-            (1,) * self.bounding_shape["z"],
-            *[self.bounding_shape[k] for k in ("c", "y", "x")],
+            (1,) * data.bounding_shape["z"],
+            *[data.bounding_shape[k] for k in ("c", "y", "x")],
         )
         darr = da.map_blocks(
-            _chunked_fibsem_loader,
-            self.filenames,
-            self.axes["c"],
+            chunked_fibsem_loader,
+            data.filenames,
+            data.axes["c"],
             pad_values,
             chunks=chunks,
-            dtype=self.dtypes[0],
+            dtype=data.dtypes[0],
         )
         return darr
+
+
+def infer_coords(array: FIBSEMData):
+    grid_spacing_xy = array.attrs["PixelSize"]
+    dims = ("x", "y", "c")
+    scales = (grid_spacing_xy, grid_spacing_xy, 1)
+    translates = (0, 0, 0)
+    coords = [
+        stt_coord(
+            length=s,
+            dim=dims[idx],
+            scale=scales[idx],
+            translate=translates[idx],
+            unit="nm",
+        )
+        for idx, s in enumerate(array.shape)
+    ]
+    return coords
+
+
+def create_dataarray(
+    element: FIBSEMData,
+    chunks: Literal["auto"] | Tuple[int, ...] = "auto",
+    coords: Any = "auto",
+    use_dask: bool = True,
+    attrs: Dict[str, Any] | None = None,
+    name: str | None = None,
+):
+
+    if coords == "auto":
+        coords = infer_coords(element)
+    if use_dask:
+        element = to_dask(element, chunks)
+
+    return DataArray(element, coords, attrs, name=name)
+
+
+def create_datatree(
+    element: FibsemDataset,
+    chunks: Literal["auto"] | Tuple[int, ...] = "auto",
+    coords: Any = "auto",
+    use_dask: bool = True,
+    attrs: Dict[str, Any] | None = None,
+    name: str | None = None,
+):
+    raise NotImplementedError("This behavior has not been implemented yet.")
+
+
+def to_xarray(
+    element: FIBSEMData | FibsemDataset,
+    chunks: Literal["auto"] | Tuple[int, ...] = "auto",
+    coords: Any = "auto",
+    use_dask: bool = True,
+    attrs: Dict[str, Any] | None = None,
+    name: str | None = None,
+):
+    if isinstance(element, FibsemDataset):
+        return create_datatree(
+            element,
+            chunks=chunks,
+            coords=coords,
+            use_dask=use_dask,
+            attrs=attrs,
+            name=name,
+        )
+
+    elif isinstance(element, FIBSEMData):
+        return create_dataarray(
+            element,
+            chunks=chunks,
+            coords=coords,
+            use_dask=use_dask,
+            attrs=attrs,
+            name=name,
+        )
+    else:
+        raise ValueError(
+            f"""
+        This function only accepts instances of zarr.Group and zarr.Array. 
+        Got {type(element)} instead.
+        """
+        )
```

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/io/h5.py` & `fibsem_tools-4.0.0/src/fibsem_tools/io/h5.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/io/multiscale.py` & `fibsem_tools-4.0.0/src/fibsem_tools/io/multiscale.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import Any, Dict, Literal, Optional, Sequence, Tuple, Union, List
 
 from xarray import DataArray
 
 import zarr
 from fibsem_tools.io.core import AccessMode, create_group
 from fibsem_tools.metadata.cosem import COSEMGroupMetadataV1, COSEMGroupMetadataV2
@@ -72,21 +73,21 @@
     for flavor in metadata_types:
         flave, _, version = flavor.partition("@")
         if flave == "neuroglancer":
             g_meta = NeuroglancerN5GroupMetadata.fromDataArrays(arrays)
             group_attrs.update(g_meta.dict())
         elif flave == "cosem":
             if version == "2":
-                g_meta = COSEMGroupMetadataV2.fromDataArrays(arrays)
+                g_meta = COSEMGroupMetadataV2.fromDataArrays(arrays, array_paths)
             else:
-                g_meta = COSEMGroupMetadataV1.fromDataArrays(arrays)
+                g_meta = COSEMGroupMetadataV1.fromDataArrays(arrays, array_paths)
             group_attrs.update(g_meta.dict())
             for idx in range(len(array_attrs)):
                 array_attrs[idx] = {
-                    **STTransform.fromDataArray(arrays[idx]).dict(),
+                    "transform": STTransform.fromDataArray(arrays[idx]).dict(),
                     **array_attrs[idx],
                 }
         elif flave == "ome-ngff":
             if array_paths is None:
                 raise ValueError(
                     f"""
                 You requested {flave}-type metadata, but array_paths was set to None.
@@ -108,54 +109,55 @@
                 {multiscale_metadata_types}
                 """
             )
     return group_attrs, array_attrs
 
 
 def multiscale_group(
-    group_url: str,
+    url: str,
     arrays: List[DataArray],
     array_paths: List[str],
-    chunks: Union[Tuple[Tuple[int, ...], ...], Tuple[int, ...], None],
+    chunks: Tuple[Tuple[int, ...], ...] | Tuple[int, ...] | None,
     metadata_types: List[str],
     group_mode: AccessMode = "w-",
     array_mode: AccessMode = "w-",
-    group_attrs: Optional[Attrs] = None,
-    array_attrs: Optional[Sequence[Attrs]] = None,
+    group_attrs: Attrs | None = None,
+    array_attrs: Sequence[Attrs] | None = None,
     **kwargs: Any,
 ) -> zarr.Group:
+
     if array_attrs is None:
         array_attrs = [{}] * len(arrays)
     if group_attrs is None:
         group_attrs = {}
 
     mgroup_attrs, marray_attrs = multiscale_metadata(
         arrays, metadata_types, array_paths=array_paths
     )
-    group_attrs.update(mgroup_attrs)
-    [a.update(marray_attrs[idx]) for idx, a in enumerate(array_attrs)]
+    _group_attrs = {**group_attrs, **mgroup_attrs}
+    _arr_attrs = [{**a, **m} for a, m in zip(array_attrs, marray_attrs)]
 
     _chunks = _normalize_chunks(arrays, chunks)
     try:
         group = create_group(
-            group_url,
+            url,
             arrays,
             array_paths=array_paths,
             chunks=_chunks,
-            group_attrs=group_attrs,
-            array_attrs=array_attrs,
+            group_attrs=_group_attrs,
+            array_attrs=_arr_attrs,
             group_mode=group_mode,
             array_mode=array_mode,
             **kwargs,
         )
         return group
     except ContainsGroupError:
         raise FileExistsError(
             f"""
-            The resource at {group_url} resolves to an existing group. Use 'w' or 'a' 
+            The resource at {url} resolves to an existing group. Use 'w' or 'a' 
             access modes to enable writable / appendable access to this group.
             """
         )
 
 
 def prepare_multiscale(
     dest_url: str,
```

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/io/server.py` & `fibsem_tools-4.0.0/src/fibsem_tools/io/server.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/io/util.py` & `fibsem_tools-4.0.0/src/fibsem_tools/io/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,52 @@
+from __future__ import annotations
 import os
 from glob import glob
 from pathlib import Path
 from shutil import rmtree
-from typing import Any, Optional, Sequence, Tuple, Union, Dict, List
+from typing import Any, Iterable, Literal, Optional, Sequence, Tuple, Union, Dict, List
 
 import fsspec
 import toolz as tz
 from dask import bag, delayed
+from typing import Protocol, runtime_checkable
 
 JSON = Union[Dict[str, "JSON"], List["JSON"], str, int, float, bool, None]
 Attrs = Dict[str, JSON]
 PathLike = Union[Path, str]
+AccessMode = Literal["w", "w-", "r", "r+", "a"]
+
+
+@runtime_checkable
+class ArrayLike(Protocol):
+    shape: Tuple[int, ...]
+    dtype: Any
+
+    def __getitem__(self, *args) -> "ArrayLike" | float:
+        ...
+
+
+@runtime_checkable
+class GroupLike(Protocol):
+    def values(self) -> Iterable[Union["GroupLike", ArrayLike]]:
+        """
+        Iterable of the children of this group
+        """
+        ...
+
+    def create_group(self, name: str, **kwargs) -> "GroupLike":
+        ...
+
+    def create_array(
+        self, name: str, dtype: Any, chunks: Tuple[int, ...], compressor: Any
+    ) -> ArrayLike:
+        ...
+
+    def __getitem__(self, *args) -> ArrayLike | "GroupLike":
+        ...
 
 
 @delayed
 def _rmtree_after_delete_files(path: str, dependency: Any):
     rmtree(path)
```

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/io/xr.py` & `fibsem_tools-4.0.0/src/fibsem_tools/io/xr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import xarray as xr
+import xarray
 import numpy as np
 import numpy.typing as npt
-from typing import Tuple, Sequence
+from typing import Any, Tuple, Sequence
 
 
-def flip(data: xr.DataArray, dims: Sequence[str] = []) -> xr.DataArray:
+def flip(data: xarray.DataArray, dims: Sequence[str] = []) -> xarray.DataArray:
     """
     Reverse the data backing a DataArray along the specified dimension(s).
     """
     flip_selector = ()
     for dim in data.dims:
         if dim in dims:
             flip_selector += (slice(None, None, -1),)
@@ -18,30 +18,31 @@
 
 
 def stt_coord(length: int, dim: str, scale: float, translate: float, unit: str):
     """
     Create a coordinate variable parametrized by a shape, a scale, a translation, and
     a unit. The translation is applied after the scaling.
     """
-    return xr.DataArray(
+    return xarray.DataArray(
         (np.arange(length) * scale) + translate, dims=(dim,), attrs={"units": unit}
     )
 
 
 def stt_from_array(
     data: npt.ArrayLike,
     dims: Tuple[str, ...],
     scales: Tuple[float, ...],
     translates: Tuple[float, ...],
     units: Tuple[str, ...],
-) -> xr.DataArray:
+    **kwargs: Any,
+) -> xarray.DataArray:
 
     """
     Create a DataArray with coordinates parametrized by a shape, a sequence of dims,
-    a sequence of scales, a sequence of translates, and a sequence of units from an
+    a sequence of scales, a sequence of translations, and a sequence of units from an
     input array.
     """
     coords = []
     for idx, s in enumerate(data.shape):
         coords.append(stt_coord(s, dims[idx], scales[idx], translates[idx], units[idx]))
 
-    return xr.DataArray(data, dims=dims, coords=coords)
+    return xarray.DataArray(data, dims=dims, coords=coords, **kwargs)
```

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/io/zarr.py` & `fibsem_tools-4.0.0/src/fibsem_tools/io/zarr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,42 @@
+from __future__ import annotations
 import logging
 import os
 from os import PathLike
 import time
 from pathlib import Path
-from typing import Any, Dict, Generator, List, Sequence, Tuple, Union
+from typing import Any, Dict, Generator, List, Literal, Sequence, Tuple, Union
+from datatree import DataTree
 import pint
 
 import dask.array as da
 import numpy as np
+import xarray
 import zarr
 from zarr.storage import FSStore, contains_array, contains_group
 from dask import bag, delayed
 from distributed import Client, Lock
 from toolz import concat
 from xarray import DataArray
 from zarr.indexing import BasicIndexer
-from fibsem_tools.io.util import split_by_suffix
 from fibsem_tools.io.xr import stt_coord
 from fibsem_tools.metadata.transform import STTransform
-from fibsem_tools.io.util import JSON
 from xarray_ome_ngff.registry import get_adapters
 
 ureg = pint.UnitRegistry()
 
 # default axis order of zarr spatial metadata
 # is z,y,x
 ZARR_AXES_3D = ["z", "y", "x"]
 
 # default axis order of raw n5 spatial metadata
 # is x,y,z
 N5_AXES_3D = ZARR_AXES_3D[::-1]
 DEFAULT_ZARR_STORE = FSStore
+DEFAULT_N5_STORE = zarr.N5FSStore
 logger = logging.getLogger(__name__)
 
 
 def get_arrays(obj: Any) -> Tuple[zarr.Array]:
     result = ()
     if isinstance(obj, zarr.core.Array):
         result = (obj,)
@@ -163,19 +165,21 @@
         raise ValueError(
             f"""
         The store associated with this object has type {type(store)}, which 
         cannot be resolved to a url"""
         )
 
 
-def access_zarr(store: PathLike, path: PathLike, **kwargs) -> Any:
+def access_zarr(
+    store: PathLike, path: PathLike, **kwargs: Any
+) -> zarr.Array | zarr.Group:
     if isinstance(store, Path):
         store = str(store)
 
-    if isinstance(store, str) and kwargs.get("mode") == "w":
+    if isinstance(store, str):
         store = DEFAULT_ZARR_STORE(store)
 
     # set default dimension separator to /
     if "shape" in kwargs and "dimension_separator" not in kwargs:
         kwargs["dimension_separator"] = "/"
 
     if isinstance(path, Path):
@@ -213,178 +217,263 @@
     array_or_group = zarr.open(store, path=path, **kwargs, mode=access_mode)
 
     if access_mode != "r":
         array_or_group.attrs.update(attrs)
     return array_or_group
 
 
-def access_n5(store: PathLike, path: PathLike, **kwargs) -> Any:
-    store = zarr.N5FSStore(store, **kwargs.get("storage_options", {}))
+def access_n5(store: PathLike, path: PathLike, **kwargs: Any) -> Any:
+    store = DEFAULT_N5_STORE(store, **kwargs.get("storage_options", {}))
     return access_zarr(store, path, **kwargs)
 
 
-def zarr_to_dask(urlpath: str, chunks: Union[str, Sequence[int]], **kwargs):
-    store_path, key, _ = split_by_suffix(urlpath, (".zarr",))
-    arr = access_zarr(store_path, key, mode="r", **kwargs)
-    if not hasattr(arr, "shape"):
-        raise ValueError(f"{store_path}/{key} is not a zarr array")
-    if chunks == "original":
-        _chunks = arr.chunks
-    else:
-        _chunks = chunks
-    darr = da.from_array(arr, chunks=_chunks, inline_array=True)
-    return darr
-
-
-def n5_to_dask(urlpath: str, chunks: Union[str, Sequence[int]], **kwargs):
-    store_path, key, _ = split_by_suffix(urlpath, (".n5",))
-    arr = access_n5(store_path, key, mode="r", **kwargs)
-    if not hasattr(arr, "shape"):
-        raise ValueError(f"{store_path}/{key} is not an n5 array")
-    if chunks == "original":
-        _chunks = arr.chunks
-    else:
-        _chunks = chunks
-    darr = da.from_array(arr, chunks=_chunks, inline_array=True)
+def to_dask(
+    arr: zarr.Array, chunks: Literal["auto"] | Sequence[int], name: str | None = None
+):
+    darr = da.from_array(arr, chunks=chunks, inline_array=True, name=name)
     return darr
 
 
 def access_parent(node: Union[zarr.Array, zarr.Group], **kwargs):
     """
     Get the parent (zarr.Group) of a zarr array or group.
     """
     parent_path = "/".join(node.path.split("/")[:-1])
     return access_zarr(store=node.store, path=parent_path, **kwargs)
 
 
-def infer_coords(
-    shape: Tuple[int, ...],
-    array_attrs: Dict[str, JSON],
-    group_attrs: Dict[str, JSON] = {},
-    array_path: str = "",
-) -> List[DataArray]:
+def is_n5(array: zarr.core.Array) -> bool:
+    return isinstance(array.store, (zarr.N5Store, zarr.N5FSStore))
+
+
+def get_chunk_keys(
+    array: zarr.core.Array, region: slice = slice(None)
+) -> Generator[str, None, None]:
+    indexer = BasicIndexer(region, array)
+    chunk_coords = (idx.chunk_coords for idx in indexer)
+    keys = (array._chunk_key(cc) for cc in chunk_coords)
+    return keys
+
+
+def chunk_grid_shape(
+    array_shape: Tuple[int, ...], chunk_shape: Tuple[int, ...]
+) -> Tuple[int, ...]:
+    return tuple(np.ceil(np.divide(array_shape, chunk_shape)).astype("int").tolist())
+
+
+class ChunkLock:
+    def __init__(self, array: zarr.core.Array, client: Client):
+        self._locks = get_chunklock(array, client)
+        # from the perspective of a zarr array, metadata has this key regardless of the
+        # location on storage. unfortunately, the synchronizer does not get access to
+        # the indirection provided by the the store class.
+
+        array_attrs_key = f"{array.path}/.zarray"
+        if is_n5(array):
+            attrs_path = f"{array.path}/attributes.json"
+        else:
+            attrs_path = array_attrs_key
+        self._locks[array_attrs_key] = Lock(attrs_path, client=client)
+
+    def __getitem__(self, key):
+        return self._locks[key]
+
+
+def get_chunklock(array: zarr.core.Array, client: Client) -> Dict[str, Lock]:
+    result = {key: Lock(key, client=client) for key in get_chunk_keys(array)}
+    return result
+
+
+def lock_array(array: zarr.core.Array, client: Client) -> zarr.core.Array:
+    lock = ChunkLock(array, client)
+    locked_array = zarr.open(
+        store=array.store, path=array.path, synchronizer=lock, mode="a"
+    )
+    return locked_array
+
+
+def are_chunks_aligned(
+    source_chunks: Tuple[int, ...], dest_chunks: Tuple[int, ...]
+) -> bool:
+    assert len(source_chunks) == len(dest_chunks)
+    return all(
+        s_chunk % d_chunk == 0 for s_chunk, d_chunk in zip(source_chunks, dest_chunks)
+    )
+
 
-    if (transform := array_attrs.get("transform", None)) is not None:
-        coords = STTransform(**transform).to_coords(shape)
+def infer_coords(array: zarr.Array) -> List[DataArray]:
 
-    elif "pixelResolution" in array_attrs or "resolution" in array_attrs:
+    group = access_parent(array, mode="r")
+
+    if (transform := array.attrs.get("transform", None)) is not None:
+        coords = STTransform(**transform).to_coords(array.shape)
+
+    elif "pixelResolution" in array.attrs or "resolution" in array.attrs:
         input_axes = N5_AXES_3D
         output_axes = input_axes[::-1]
         translates = {ax: 0 for ax in output_axes}
         units = {ax: "nanometer" for ax in output_axes}
 
-        if "pixelResolution" in array_attrs:
-            pixelResolution = array_attrs["pixelResolution"]
+        if "pixelResolution" in array.attrs:
+            pixelResolution = array.attrs["pixelResolution"]
             scales = dict(zip(input_axes, pixelResolution["dimensions"]))
             units = {ax: pixelResolution["unit"] for ax in input_axes}
 
-        elif "resolution" in array_attrs:
-            _scales = array_attrs["resolution"]
+        elif "resolution" in array.attrs:
+            _scales = array.attrs["resolution"]
             scales = dict(zip(N5_AXES_3D, _scales))
 
         coords = [
-            stt_coord(shape[idx], ax, scales[ax], translates[ax], units[ax])
+            stt_coord(array.shape[idx], ax, scales[ax], translates[ax], units[ax])
             for idx, ax in enumerate(output_axes)
         ]
-    elif (multiscales := group_attrs.get("multiscales", None)) is not None:
+    elif (multiscales := group.attrs.get("multiscales", None)) is not None:
         if len(multiscales) > 0:
             multiscale = multiscales[0]
             if (ngff_version := multiscale.get("version", None)) == "0.4":
                 from pydantic_ome_ngff.v04 import Multiscale
             elif multiscale["version"] == "0.5-dev":
                 from pydantic_ome_ngff.latest import Multiscale
             else:
                 raise ValueError(
                     f"""
                     Could not resolve the version of the multiscales metadata 
-                    found in the group metadata {group_attrs}
+                    found in the group metadata {dict(group.attrs)}
                     """
                 )
         else:
             raise ValueError("Multiscales attribute was empty")
         xarray_adapters = get_adapters(ngff_version)
         multiscales_meta = [Multiscale(**entry) for entry in multiscales]
         transforms = []
         axes = []
         matched_multiscale = None
         matched_dataset = None
         # find the correct element in multiscales.datasets for this array
         for multi in multiscales_meta:
             for dataset in multi.datasets:
-                if dataset.path == array_path:
+                if dataset.path == array.basename:
                     matched_multiscale = multi
                     matched_dataset = dataset
         if matched_dataset is None or matched_multiscale is None:
             raise ValueError(
                 f"""
-            Could not find an entry referencing array {array_path} in the `multiscales`
-            metadata of the parent group.
+            Could not find an entry referencing array {array.basename} 
+            in the `multiscales` metadata of the parent group.
             """
             )
         else:
             transforms.extend(matched_multiscale.coordinateTransformations)
             transforms.extend(matched_dataset.coordinateTransformations)
             axes.extend(matched_multiscale.axes)
-            coords = xarray_adapters.transforms_to_coords(axes, transforms, shape)
+            coords = xarray_adapters.transforms_to_coords(axes, transforms, array.shape)
     else:
         raise ValueError("Could not infer coordinates from the supplied attributes.")
 
     return coords
 
 
-def is_n5(array: zarr.core.Array) -> bool:
-    return isinstance(array.store, (zarr.N5Store, zarr.N5FSStore))
-
-
-def get_chunk_keys(
-    array: zarr.core.Array, region: slice = slice(None)
-) -> Generator[str, None, None]:
-    indexer = BasicIndexer(region, array)
-    chunk_coords = (idx.chunk_coords for idx in indexer)
-    keys = (array._chunk_key(cc) for cc in chunk_coords)
-    return keys
-
-
-def chunk_grid_shape(
-    array_shape: Tuple[int, ...], chunk_shape: Tuple[int, ...]
-) -> Tuple[int, ...]:
-    return tuple(np.ceil(np.divide(array_shape, chunk_shape)).astype("int").tolist())
-
-
-class ChunkLock:
-    def __init__(self, array: zarr.core.Array, client: Client):
-        self._locks = get_chunklock(array, client)
-        # from the perspective of a zarr array, metadata has this key regardless of the
-        # location on storage. unfortunately, the synchronizer does not get access to
-        # the indirection provided by the the store class.
-
-        array_attrs_key = f"{array.path}/.zarray"
-        if is_n5(array):
-            attrs_path = f"{array.path}/attributes.json"
-        else:
-            attrs_path = array_attrs_key
-        self._locks[array_attrs_key] = Lock(attrs_path, client=client)
+def to_xarray(
+    element: zarr.Array | zarr.Group,
+    chunks: Literal["auto"] | Tuple[int, ...] = "auto",
+    use_dask: bool = True,
+    attrs: Dict[str, Any] | None = None,
+    coords: Any = "auto",
+    name: str | None = None,
+):
+    if isinstance(element, zarr.Group):
+        return create_datatree(
+            element,
+            chunks=chunks,
+            coords=coords,
+            attrs=attrs,
+            use_dask=use_dask,
+            name=name,
+        )
+    elif isinstance(element, zarr.Array):
+        return create_dataarray(
+            element,
+            chunks=chunks,
+            coords=coords,
+            attrs=attrs,
+            use_dask=use_dask,
+            name=name,
+        )
+    else:
+        raise ValueError(
+            f"""
+        This function only accepts instances of zarr.Group and zarr.Array. 
+        Got {type(element)} instead.
+        """
+        )
 
-    def __getitem__(self, key):
-        return self._locks[key]
 
+def create_dataarray(
+    element: zarr.Array,
+    chunks: Literal["auto"] | Tuple[int, ...] = "auto",
+    coords: Any = "auto",
+    use_dask: bool = True,
+    attrs: Dict[str, Any] | None = None,
+    name: str | None = None,
+) -> xarray.DataArray:
+    """
+    Create an xarray.DataArray from a zarr array.
+    """
+
+    if name is None:
+        name = element.basename
+
+    if coords == "auto":
+        coords = infer_coords(element)
+
+    # todo: fix this unfortunate structure
+    elif hasattr(coords, "to_coords"):
+        coords = coords.to_coords(element.shape)
+
+    if use_dask:
+        if attrs is None:
+            attrs = dict(element.attrs)
+        element = to_dask(element, chunks=chunks, name=name)
 
-def get_chunklock(array: zarr.core.Array, client: Client) -> Dict[str, Lock]:
-    result = {key: Lock(key, client=client) for key in get_chunk_keys(array)}
+    result = xarray.DataArray(element, coords=coords, attrs=attrs, name=name)
     return result
 
 
-def lock_array(array: zarr.core.Array, client: Client) -> zarr.core.Array:
-    lock = ChunkLock(array, client)
-    locked_array = zarr.open(
-        store=array.store, path=array.path, synchronizer=lock, mode="a"
-    )
-    return locked_array
+def create_datatree(
+    element: zarr.Group,
+    chunks: Union[str, Tuple[int, ...]] = "auto",
+    coords: Any = "auto",
+    use_dask: bool = True,
+    attrs: Dict[str, Any] | None = None,
+    name: str | None = None,
+) -> DataTree:
 
+    if coords != "auto":
+        raise NotImplementedError(
+            f"""
+        This function does not support values of `coords` other than `auto`. 
+        Got {coords}. This may change in the future.
+        """
+        )
 
-def are_chunks_aligned(
-    source_chunks: Tuple[int, ...], dest_chunks: Tuple[int, ...]
-) -> bool:
-    assert len(source_chunks) == len(dest_chunks)
-    return all(
-        s_chunk % d_chunk == 0 for s_chunk, d_chunk in zip(source_chunks, dest_chunks)
-    )
+    if name is None:
+        name = element.basename
+
+    nodes = {
+        name: create_dataarray(
+            array,
+            chunks=chunks,
+            coords=coords,
+            use_dask=use_dask,
+            attrs=None,
+            name="data",
+        )
+        for name, array in element.arrays()
+    }
+    if attrs is None:
+        root_attrs = dict(element.attrs)
+    else:
+        root_attrs = attrs
+    # insert root element
+    nodes["/"] = xarray.Dataset(attrs=root_attrs)
+    dtree = DataTree.from_dict(nodes, name=name)
+    return dtree
```

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/metadata/cosem.py` & `fibsem_tools-4.0.0/src/fibsem_tools/metadata/cosem.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/metadata/groundtruth.py` & `fibsem_tools-4.0.0/src/fibsem_tools/metadata/groundtruth.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/metadata/neuroglancer.py` & `fibsem_tools-4.0.0/src/fibsem_tools/metadata/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-3.2.0/src/fibsem_tools/metadata/transform.py` & `fibsem_tools-4.0.0/src/fibsem_tools/metadata/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Optional, Sequence, Tuple, Union, Literal
 
 from pydantic import BaseModel, root_validator
 from xarray import DataArray
-from fibsem_tools.io.xr import stt_coord
+import fibsem_tools.io.xr as fsxr
 
 ArrayOrder = Literal["C", "F"]
 
 
 class STTransform(BaseModel):
     """
     Representation of an N-dimensional scaling -> translation transform for labelled
@@ -43,15 +43,15 @@
         from this transform.
         """
         if self.order == "C":
             axes = self.axes
         else:
             axes = reversed(self.axes)
         return [
-            stt_coord(
+            fsxr.stt_coord(
                 shape[idx],
                 dim=k,
                 scale=self.scale[idx],
                 translate=self.translate[idx],
                 unit=self.units[idx],
             )
             for idx, k in enumerate(axes)
```

### Comparing `fibsem_tools-3.2.0/PKG-INFO` & `fibsem_tools-4.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibsem-tools
-Version: 3.2.0
+Version: 4.0.0
 Summary: Tools for processing FIBSEM datasets
 License: MIT
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,10 +24,11 @@
 Requires-Dist: pint (>=0.20.1,<0.21.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pydantic-ome-ngff (>=0.2.0,<0.3.0)
 Requires-Dist: s3fs (>=2022.2.0)
 Requires-Dist: textual (>=0.16.0,<0.17.0)
 Requires-Dist: tifffile (>=2023.2.28,<2024.0.0)
 Requires-Dist: xarray (>=2022.03.0)
+Requires-Dist: xarray-datatree (>=0.0.12,<0.0.13)
 Requires-Dist: xarray-multiscale (>=2.0.0,<3.0.0)
 Requires-Dist: xarray-ome-ngff (>=1.2.0,<2.0.0)
 Requires-Dist: zarr (>=2.10.3,<3.0.0)
```

