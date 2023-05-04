# Comparing `tmp/bipl-0.1.0.post2.tar.gz` & `tmp/bipl-0.1.1.tar.gz`

## Comparing `bipl-0.1.0.post2.tar` & `bipl-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    13933 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/hatch_build.py
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/pyproject.toml
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 bipl-0.1.0.post2/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    14278 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bipl-0.1.1/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.1.1/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.1.1/hatch_build.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 bipl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 bipl-0.1.1/PKG-INFO
```

### Comparing `bipl-0.1.0.post2/src/bipl/io/__init__.py` & `bipl-0.1.1/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/src/bipl/io/_dzi.py` & `bipl-0.1.1/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/src/bipl/io/_libs.py` & `bipl-0.1.1/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/src/bipl/io/_openslide.py` & `bipl-0.1.1/src/bipl/io/_openslide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/src/bipl/io/_slide.py` & `bipl-0.1.1/src/bipl/io/_slide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/src/bipl/io/_slide_bases.py` & `bipl-0.1.1/src/bipl/io/_slide_bases.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/src/bipl/io/_tiff.py` & `bipl-0.1.1/src/bipl/io/_tiff.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/src/bipl/ops/_mosaic.py` & `bipl-0.1.1/src/bipl/ops/_mosaic.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import dataclasses
 from collections import defaultdict
 from collections.abc import Callable, Iterable, Iterator
 from dataclasses import dataclass, field
 from functools import partial
 from itertools import chain
-from typing import NamedTuple, Protocol, TypeVar, cast
+from typing import ContextManager, NamedTuple, Protocol, TypeVar, cast
 
 import cv2
 import numpy as np
 from glow import chunked, map_n
 
 from ._util import get_trapz
 
@@ -203,14 +203,17 @@
         assert v_scale >= 1
         for tile in self:
             tw, th = tile.data.shape[:2]
             v = view[tile.vec[0] // v_scale:,
                      tile.vec[1] // v_scale:][:tw // v_scale, :th // v_scale]
             yield tile.idx, tile.vec, tile.data, v
 
+    def with_cm(self: _Self, cm: ContextManager) -> _Self:
+        return cast(_Self, _CmView(self.m, self.shape, self.cells, self, cm))
+
 
 @dataclass
 class _View(_BaseView):
     def map_batched(self,
                     fn: Callable[[list[np.ndarray]], Iterable[np.ndarray]],
                     /,
                     batch_size: int = 1,
@@ -265,14 +268,24 @@
     source: Iterable[Tile]
 
     def __iter__(self) -> Iterator[Tile]:
         return iter(self.source)
 
 
 @dataclass
+class _CmView(_BaseView):
+    source: Iterable[Tile]
+    _cm: ContextManager
+
+    def __iter__(self) -> Iterator[Tile]:
+        with self._cm:
+            yield from self.source
+
+
+@dataclass
 class _DecimatedView(_View):
     """
     Decimates tiles.
     Doesn't change size uniformity.
     Yields decimated views of original tiles.
     """
     stride: int
```

### Comparing `bipl-0.1.0.post2/src/bipl/ops/_util.py` & `bipl-0.1.1/src/bipl/ops/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/LICENSE` & `bipl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/README.md` & `bipl-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/hatch_build.py` & `bipl-0.1.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.0.post2/pyproject.toml` & `bipl-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.1.0.post2"
+version = "0.1.1"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
```

### Comparing `bipl-0.1.0.post2/PKG-INFO` & `bipl-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.1.0.post2
+Version: 0.1.1
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
```

