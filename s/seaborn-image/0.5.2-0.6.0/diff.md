# Comparing `tmp/seaborn_image-0.5.2.tar.gz` & `tmp/seaborn_image-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn_image-0.5.2.tar", max compression
+gzip compressed data, was "seaborn_image-0.6.0.tar", max compression
```

## Comparing `seaborn_image-0.5.2.tar` & `seaborn_image-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-03-17 17:34:24.427780 seaborn_image-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0     2755 2023-03-17 17:34:24.427780 seaborn_image-0.5.2/README.md
--rw-r--r--   0        0        0     1373 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      535 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/src/seaborn_image/__init__.py
--rw-r--r--   0        0        0     1442 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/src/seaborn_image/_colormap.py
--rw-r--r--   0        0        0     6997 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/src/seaborn_image/_context.py
--rw-r--r--   0        0        0     7895 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/src/seaborn_image/_core.py
--rw-r--r--   0        0        0     2132 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/src/seaborn_image/_datasets.py
--rw-r--r--   0        0        0    11282 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/src/seaborn_image/_filters.py
--rw-r--r--   0        0        0    19496 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/src/seaborn_image/_general.py
--rw-r--r--   0        0        0    43923 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/src/seaborn_image/_grid.py
--rw-r--r--   0        0        0     4523 2023-03-17 17:34:24.623786 seaborn_image-0.5.2/src/seaborn_image/utils.py
--rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 seaborn_image-0.5.2/setup.py
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 seaborn_image-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-04 01:15:10.718739 seaborn_image-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     2755 2023-05-04 01:15:10.718739 seaborn_image-0.6.0/README.md
+-rw-r--r--   0        0        0     1373 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      535 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/__init__.py
+-rw-r--r--   0        0        0     2070 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_colormap.py
+-rw-r--r--   0        0        0     7170 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_context.py
+-rw-r--r--   0        0        0     8043 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_core.py
+-rw-r--r--   0        0        0     2507 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_datasets.py
+-rw-r--r--   0        0        0    11282 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_filters.py
+-rw-r--r--   0        0        0    19589 2023-05-04 01:15:10.922742 seaborn_image-0.6.0/src/seaborn_image/_general.py
+-rw-r--r--   0        0        0    45585 2023-05-04 01:15:10.922742 seaborn_image-0.6.0/src/seaborn_image/_grid.py
+-rw-r--r--   0        0        0     4523 2023-05-04 01:15:10.922742 seaborn_image-0.6.0/src/seaborn_image/utils.py
+-rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 seaborn_image-0.6.0/setup.py
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 seaborn_image-0.6.0/PKG-INFO
```

### Comparing `seaborn_image-0.5.2/LICENSE.txt` & `seaborn_image-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.5.2/README.md` & `seaborn_image-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.5.2/pyproject.toml` & `seaborn_image-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seaborn-image"
-version = "0.5.2"
+version = "0.6.0"
 description = "Attractive, descriptive and effective image visualization with seaborn-like API built on top of matplotlib"
 authors = ["Sarthak Jariwala <contact@sarthakjariwala.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/SarthakJariwala/seaborn-image"
 repository = "https://github.com/SarthakJariwala/seaborn-image"
 documentation = "https://seaborn-image.readthedocs.io/"
```

### Comparing `seaborn_image-0.5.2/src/seaborn_image/__init__.py` & `seaborn_image-0.6.0/src/seaborn_image/__init__.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.5.2/src/seaborn_image/_context.py` & `seaborn_image-0.6.0/src/seaborn_image/_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import warnings
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-from matplotlib.cm import register_cmap
 
-from ._colormap import _CMAP_QUAL
+from ._colormap import _CMAP_QUAL, _CMAP_EXTRA
 
 __all__ = [
     "set_context",
     "set_save_context",
     "reset_defaults",
     "set_image",
     "set_scalebar",
@@ -119,21 +118,26 @@
     --------
         >>> import seaborn_image as isns
         >>> isns.set_image(cmap="inferno", interpolation="bicubic")
         >>> isns.set_image(despine=False)
 
     """
 
+    # Load colormap from palletable 
     if isinstance(cmap, str) and cmap in _CMAP_QUAL.keys():
-        cmap_mpl = _CMAP_QUAL.get(cmap).mpl_colormap
-        try:
-            register_cmap(name=cmap, cmap=cmap_mpl)
-        # above line will raise ValueError in matplotlib>3.6 if cmap already registered
-        except ValueError:  # pragma: no cover
-            pass
+        cmap_qual_mpl = _CMAP_QUAL.get(cmap).mpl_colormap
+        if cmap not in mpl.colormaps.keys():
+            mpl.colormaps.register(name=cmap, cmap=cmap_qual_mpl)
+    
+    # Load extra colormap
+    if isinstance(cmap, str) and cmap in _CMAP_EXTRA.keys():
+        cmap_channel_mpl = _CMAP_EXTRA.get(cmap)
+        if cmap not in mpl.colormaps.keys():
+            mpl.colormaps.register(name=cmap, cmap=cmap_channel_mpl)
+        
 
     # change the axes spines
     # "not" is required because of the despine parameter name
     # if depine is True ---> you don't want the axes spines
     # and therfore, axes.spines.bottom == False (or not True)
     mpl.rcParams.update(
         {
```

### Comparing `seaborn_image-0.5.2/src/seaborn_image/_core.py` & `seaborn_image-0.6.0/src/seaborn_image/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import matplotlib as mpl
 import matplotlib.colors as colors
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib_scalebar.scalebar import ScaleBar
 from mpl_toolkits.axes_grid1 import axes_size, make_axes_locatable
 
-from ._colormap import _CMAP_QUAL
+from ._colormap import _CMAP_QUAL, _CMAP_EXTRA
 from .utils import despine, scientific_ticks
 
 # dimensions for scalebar
 _DIMENSIONS = {
     "si": "si-length",
     "si-reciprocal": "si-length-reciprocal",
     "imperial": "imperial-length",
@@ -100,14 +100,17 @@
         ax.add_artist(scalebar)
 
     def plot(self):
         f, ax = self._setup_figure()
 
         if isinstance(self.cmap, str) and self.cmap in _CMAP_QUAL.keys():
             self.cmap = _CMAP_QUAL.get(self.cmap).mpl_colormap
+        
+        if isinstance(self.cmap, str) and self.cmap in _CMAP_EXTRA.keys():
+            self.cmap = _CMAP_EXTRA.get(self.cmap)
 
         if self.robust:
             min_robust = False
             max_robust = False
             if self.vmin is None:
                 min_robust = (
                     True  # remember that vmin was None and now set to new value
```

### Comparing `seaborn_image-0.5.2/src/seaborn_image/_datasets.py` & `seaborn_image-0.6.0/src/seaborn_image/_datasets.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     base_url="https://github.com/SarthakJariwala/seaborn-image/raw/master/data/",
     # The registry specifies the files that can be fetched
     registry={
         # The registry is a dict with file names and their SHA256 hashes
         "PolymerImage.txt": "7b6798865080adf3ecf11e342f3d86d7b52ea0700020a1f062544ee825fb8a0e",
         "Perovskite.txt": "3228eeade5afec3c2b1ed116b2d4fe35877224d2d9bf7b4a17e04a432e6135c5",
         "cells.tif": "2120cfe08e0396324793a10a905c9bbcb64b117215eb63b2c24b643e1600c8c9",
+        "cifar10.npy": "c0a12085b3b82f4a6d1f95e609a40701648a137eb9ff1fb5751071f54cc8e05c",
     },
 )
 
 
 def load_image(name):
     """Load image data shippped with seaborn-image.
 
@@ -62,13 +63,22 @@
     elif name == "cells":
         path = POOCH.fetch("cells.tif")
         img = io.imread(path).T
 
     elif name == "retina-gray":
         img = color.rgb2gray(data.retina())[300:700, 700:900]
 
+    elif name == "cifar10":
+        path = POOCH.fetch("cifar10.npy")
+        img = np.load(path)
+
+    elif name == "cifar10 list":
+        path = POOCH.fetch("cifar10.npy")
+        img_array = np.load(path)
+        img = [arr for arr in img_array]
+
     else:
         raise ValueError(
-            f"No '{name}' image dataset. Available image datasets include: polymer, polymer outliers, fluorescence, cells"
+            f"No '{name}' image dataset. Available image datasets include: polymer, polymer outliers, fluorescence, cells, retina-gray, cifar10, cifar list"
         )
 
     return img
```

### Comparing `seaborn_image-0.5.2/src/seaborn_image/_filters.py` & `seaborn_image-0.6.0/src/seaborn_image/_filters.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.5.2/src/seaborn_image/_general.py` & `seaborn_image-0.6.0/src/seaborn_image/_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import scipy.stats as ss
 from matplotlib import gridspec
 from matplotlib.axes import Axes
 from matplotlib.cm import get_cmap
 from matplotlib.colors import Colormap
 from skimage.color import rgb2gray
 
-from ._colormap import _CMAP_QUAL
+from ._colormap import _CMAP_QUAL, _CMAP_EXTRA
 from ._core import _SetupImage
 from .utils import is_documented_by
 
 __all__ = ["imgplot", "imghist", "imshow"]
 
 
 def imgplot(
@@ -648,14 +648,16 @@
     ax2.set_frame_on(False)
 
     if cmap is None:
         cm = get_cmap()
     else:
         if cmap in _CMAP_QUAL.keys():
             cm = _CMAP_QUAL.get(cmap).mpl_colormap
+        elif cmap in _CMAP_EXTRA.keys():
+            cm = _CMAP_EXTRA.get(cmap)
         else:
             cm = plt.cm.get_cmap(cmap)
 
     bin_centers = bins[:-1] + bins[1:]
 
     # convert to logscale
     if cbar_log is True:
```

### Comparing `seaborn_image-0.5.2/src/seaborn_image/_grid.py` & `seaborn_image-0.6.0/src/seaborn_image/_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import itertools
 import warnings
 from typing import Iterable
 
 import matplotlib.pyplot as plt
 import numpy as np
+from copy import copy
 
 from ._filters import filterplot
 from ._general import imgplot
 from .utils import despine
 
 __all__ = ["ParamGrid", "ImageGrid", "rgbplot", "FilterGrid"]
 
 
 class ImageGrid:
     """
-    Figure level : plot a collection of 2-D images or 3-D image data
-    along a grid. This class also supports slicing of the 3-D image
+    Figure level : plot a collection of 2-D or 3-D images or 3-D or 4-D image data
+    along a grid. This class also supports slicing of the 3-D and 4-D image data
     along different axis with variable step sizes and start/end indexes.
 
     Parameters
     ----------
     data :
-        3-D Image data (array-like) or list of 2-D image data. Supported array shapes are all
+        3-D or 4-D Image data (array-like), or list of 2-D or 3-D image data. Supported array shapes are all
         `matplotlib.pyplot.imshow` array shapes
     slices : int or list, optional
-        If `data` is 3-D, `slices` will index the specific slice from the last axis and only plot
+        If `data` is 3-D or 4-D, `slices` will index the specific slice from the last axis and only plot
         the resulting images. If None, it will plot all the slices from the last axis, by default None
     axis : int, optional
-        Axis along which the data will be sliced, by default -1
+        Axis along which the data will be sliced, by default -1 for 3-D arrays and 0 for 4-D arrays
     step : int, optional
         Step along the given axis, by default 1
     start : int, optional
         Starting index to select from the the data, by default None
     stop : int, optional
         Stopping index to select from the data, by default None
     map_func : callable or list/tuple or callables, optional
@@ -63,14 +64,17 @@
         Image origin, by default None
     vmin : float or list of floats, optional
         Minimum data value that colormap covers, by default None
     vmax : float or list of floats, optional
         Maximum data value that colormap covers, by default None
     interpolation : str, optional
         `matplotlib.pyplot.imshow` interpolation method used, by default None
+    norm : `matplotlib.colors.Normalize` or list of `matplotlib.colors.Normalize`, optional
+        `matplotlib` Normalize instance used to scale scalar data before
+        mapping to colors using cmap.
     dx : float or list, optional
         Size per pixel of the image data. If scalebar
         is required, `dx` and `units` must be sepcified.
         Can be a list of floats, if input data is a list of images.
         Defaults to None.
     units : str or list, optional
         Units of `dx`.
@@ -115,23 +119,25 @@
         A `seaborn_image.ImageGrid` object
 
     Raises
     ------
     ValueError
         If `data` is None
     ValueError
-        If `data` has more than 3 dimensions
+        If `data` has 1 dimension
     ValueError
-        If `data` contains a 3D image within a list of images
+        If `data` has more than 4 dimensions
+    ValueError
+        If `data` contains a 4D image within a list of images
     ValueError
         If `axis` is not 0, 1, 2 or -1
     TypeError
         If `map_func` is not a callable object or a list/tuple of callable objects
     ValueError
-        If `map_func` is a list/tuple of callable objects when `data` is 3D
+        If `map_func` is a list/tuple of callable objects when `data` is 3D or 4D
 
     Examples
     --------
 
     Plot a collection of images
 
     .. plot::
@@ -210,14 +216,30 @@
     Visulaize image intensities relative to other images on the grid
 
     .. plot::
         :context: close-figs
 
         >>> g = isns.ImageGrid(cells, vmin=0, vmax=1, height=1, col_wrap=5)
 
+    Plot a list of 3-D images
+
+    .. plot::
+        :context: close-figs
+
+        >>> from skimage.data import astronaut, chelsea
+        >>> g = isns.ImageGrid([astronaut(), chelsea()], origin="upper")
+
+    Plot 4-D image data cube
+
+    .. plot::
+        :context: close-figs
+
+        >>> cifar = isns.load_image("cifar10")
+        >>> g = isns.ImageGrid(cifar, height=1, col_wrap=6)
+
     Map a function to the image data
 
     .. plot::
         :context: close-figs
 
         >>> from skimage.exposure import adjust_gamma
         >>> g = isns.ImageGrid(
@@ -281,15 +303,15 @@
     """
 
     def __init__(
         self,
         data,
         *,
         slices=None,
-        axis=-1,
+        axis=None,
         step=1,
         start=None,
         stop=None,
         map_func=None,
         map_func_kw=None,
         col_wrap=None,
         height=3,
@@ -298,14 +320,15 @@
         robust=False,
         perc=(2, 98),
         alpha=None,
         origin=None,
         vmin=None,
         vmax=None,
         interpolation=None,
+        norm=None,
         dx=None,
         units=None,
         dimension=None,
         cbar=True,
         orientation="v",
         cbar_log=False,
         cbar_label=None,
@@ -318,75 +341,97 @@
 
         if isinstance(
             data, (list, tuple)
         ):  # using 'Iterable' numpy was being picked up
             # check the number of images to be plotted
             _nimages = len(data)
 
-            # --- List/Tuple of 2D images with a List/Tuple of map_func ---
+            # --- List/Tuple of 2D or 3D images with a List/Tuple of map_func ---
             # change the number of images on the grid accordingly
             map_func_type = self._check_map_func(map_func, map_func_kw)
             if map_func_type == "list/tuple":
                 _nimages = len(data) * len(map_func)
                 # no of columns should either be len of data list or len of map_func list
                 # whichever is higher
                 if col_wrap is None:
                     col_wrap = (
                         len(map_func) if len(map_func) >= len(data) else len(data)
                     )
 
-        elif data.ndim > 3:
-            raise ValueError("image data can not have more than 3 dimensions")
+        elif not isinstance(data, np.ndarray):
+            raise ValueError("image data must be a list of images or a 3d or 4d array.")
+
+        elif data.ndim == 2:
+            warnings.warn(
+                "The data inputed is a 2d array which contains a single image. "
+                "It is recomended that you use `imgplot` instead of `ImageGrid`.",
+                RuntimeWarning,
+            )
+            _nimages = 1
+
+            # ---- 2D image with a list/tuple of map_func or individual map_func ------
+            # check if map_func is a list/tuple of callables
+            # and assign the new number of images
+            map_func_type = self._check_map_func(map_func, map_func_kw)
+            if map_func_type == "list/tuple":
+                _nimages = len(map_func)
+                # no of columns should now be len of map_func list
+                col_wrap = len(map_func) if col_wrap is None else col_wrap
+
+        elif data.ndim in [3, 4]:
+            if data.ndim == 4 and data.shape[-1] not in [1, 3, 4]:
+                raise ValueError(
+                    "The number of channels in the images must be 1, 3 or 4"
+                )
+
+            if axis is None:
+                if data.ndim == 3:
+                    axis = -1
+                else:
+                    axis = 0
+
+            if data.ndim == 3 and axis not in [0, 1, 2, -1]:
+                raise ValueError("Incorrect 'axis'; must be either 0, 1, 2, or -1")
+
+            if data.ndim == 4 and axis not in [0, 1, 2, 3, -1]:
+                raise ValueError("Incorrect 'axis'; must be either 0, 1, 2, 3, or -1")
 
-        elif data.ndim == 3:
             if slices is None:
-                if axis not in [0, 1, 2, -1]:
-                    raise ValueError("Incorrect 'axis'; must be either 0, 1, 2, or -1")
                 # slice the image array along specified axis;
                 # if start, stop and step are not provided, default is step=1
                 data = data[
                     (slice(None),) * (axis % data.ndim) + (slice(start, stop, step),)
                 ]
                 slices = np.arange(data.shape[axis])
 
             # if a single slice is provided and
             # it is not an interable
             elif not isinstance(slices, Iterable):
                 slices = [slices]
 
             _nimages = len(slices)
 
-            # ---- 3D image with an individual map_func ----
+            # ---- 3D or 4D image with an individual map_func ----
             map_func_type = self._check_map_func(map_func, map_func_kw)
             # raise a ValueError if a list of map_func is provided for 3d image
             # TODO - support multiple map_func if "chaining"?
             if map_func_type == "list/tuple":
                 raise ValueError(
-                    "Can not map multiple functions to a 3D image. Please provide a single `map_func`"
+                    "Can not map multiple functions to 3D or 4D image. Please provide a single `map_func`"
                 )
 
         else:
-            # if data dim is not >2,
-            _nimages = 1
-
-            # ---- 2D image with a list/tuple of map_func or individual map_func ------
-            # check if map_func is a list/tuple of callables
-            # and assign the new number of images
-            map_func_type = self._check_map_func(map_func, map_func_kw)
-            if map_func_type == "list/tuple":
-                _nimages = len(map_func)
-                # no of columns should now be len of map_func list
-                col_wrap = len(map_func) if col_wrap is None else col_wrap
+            raise ValueError("Image data can not have more than 4 dimensions")
 
         # if no column wrap specified
         # set it to default 3
         if col_wrap is None:
             col_wrap = 3
 
-            # don't create extra columns when there aren't enough images
+        # don't create extra columns when there aren't enough images
         if col_wrap > _nimages:
             col_wrap = _nimages
 
         # Compute the grid shape if col_wrap is specified
         ncol = col_wrap
         nrow = int(np.ceil(_nimages / col_wrap))
 
@@ -413,14 +458,15 @@
         self.robust = robust
         self.perc = perc
         self.alpha = alpha
         self.origin = origin
         self.vmin = vmin
         self.vmax = vmax
         self.interpolation = interpolation
+        self.norm = norm
         self.dx = dx
         self.units = units
         self.dimension = dimension
         self.cbar = cbar
         self.orientation = orientation
         self.cbar_log = cbar_log
         self.cbar_label = cbar_label
@@ -475,46 +521,43 @@
         """Map image data cube to the image grid."""
 
         _cmap = self.cmap
         _robust = self.robust
         _perc = self.perc
         _vmin = self.vmin
         _vmax = self.vmax
+        _norm = self.norm
         _dx = self.dx
         _units = self.units
         _dimension = self.dimension
         _cbar = self.cbar
         _cbar_log = self.cbar_log
         _cbar_label = self.cbar_label
 
         for i in range(self._nimages):
             ax = self.axes.flat[i]
 
             if isinstance(self.data, (list, tuple)):
                 _d = self.data[i]
 
                 # check if the image has more than 2 dimensions
-                if _d.ndim > 2:
+                if _d.ndim > 3:
                     raise ValueError(
-                        "can not plot multiple 3D images. Supply an individual 3D image"
+                        f"Image {i} in the list has more than 3 dimensions"
                     )
 
-            elif self.data.ndim == 3:
-                if self.axis == 0:
-                    _d = self.data[self.slices[i], :, :]
-                elif self.axis == 1:
-                    _d = self.data[:, self.slices[i], :]
-                elif self.axis == 2 or self.axis == -1:
-                    _d = self.data[:, :, self.slices[i]]
+                if _d.ndim == 3 and _d.shape[-1] not in [1, 3, 4]:
+                    raise ValueError(f"Image {i} in the list has more than 4 channels")
 
-            else:
-                # if a single 2D image is supplied
-                # TODO issue a warning and direct the user to imgplot()
+            elif self.data.ndim == 2:
                 _d = self.data
 
+            else:
+                _d = self.data.take(indices=self.slices[i], axis=self.axis)
+
             if isinstance(self.cmap, (list, tuple)):
                 self._check_len_wrt_n_images(self.cmap)
                 _cmap = self.cmap[i]
 
             if isinstance(self.robust, (list, tuple)):
                 self._check_len_wrt_n_images(self.robust)
                 _robust = self.robust[i]
@@ -527,14 +570,18 @@
                 self._check_len_wrt_n_images(self.vmax)
                 _vmax = self.vmax[i]
 
             if isinstance(self.perc, (list)):
                 self._check_len_wrt_n_images(self.perc)
                 _perc = self.perc[i]
 
+            if isinstance(self.norm, (list)):
+                self._check_len_wrt_n_images(self.norm)
+                _norm = self.norm[i]
+
             if isinstance(self.dx, (list, tuple)):
                 self._check_len_wrt_n_images(self.dx)
                 _dx = self.dx[i]
 
             if isinstance(self.units, (list, tuple)):
                 self._check_len_wrt_n_images(self.units)
                 _units = self.units[i]
@@ -562,14 +609,15 @@
                 robust=_robust,
                 perc=_perc,
                 vmin=_vmin,
                 vmax=_vmax,
                 alpha=self.alpha,
                 origin=self.origin,
                 interpolation=self.interpolation,
+                norm=_norm,
                 dx=_dx,
                 units=_units,
                 dimension=_dimension,
                 cbar=_cbar,
                 orientation=self.orientation,
                 cbar_log=_cbar_log,
                 cbar_label=_cbar_label,
@@ -622,15 +670,16 @@
             self.cbar_label = self.cbar_label * len(map_func)
 
         if isinstance(self.cbar_log, (list, tuple)):
             self.cbar_log = self.cbar_log * len(map_func)
 
     def _map_func_to_data(self, map_func, map_func_kw):
         """Transform image data using the map_func callable object."""
-        # if data is a list or tuple of 2D images
+        self.data = copy(self.data)
+        # if data is a list or tuple of 2D or 3D images
         if isinstance(self.data, (list, tuple)):
             if self._check_map_func(map_func, map_func_kw) == "list/tuple":
                 self._adjust_param_list_len(map_func)
                 _d = self.data
                 # only pass on kwargs if not None
                 if map_func_kw is not None:
                     # check if one of the supplied kwargs in the list is None
@@ -647,23 +696,23 @@
                 for i in range(len(self.data)):
                     # only pass on kwargs if not None
                     if map_func_kw is not None:
                         self.data[i] = map_func(self.data[i], **map_func_kw)
                     else:
                         self.data[i] = map_func(self.data[i])
 
-        # if data is 3D or 2D and map_func is single callable
         else:
+            # if data is 4D, 3D or 2D and map_func is single callable
             if self._check_map_func(map_func, map_func_kw) == "callable":
-                # only pass on kwargs if not None
                 if map_func_kw is not None:
                     self.data = map_func(self.data, **map_func_kw)
                 else:
                     self.data = map_func(self.data)
-            # list of callables -- only for 2D image
+
+            # list of callables -- only for list of 2D or list of 3D images
             else:
                 _d = self.data
                 # only pass on kwargs if not None
                 if map_func_kw is not None:
                     # check if one of the supplied kwargs in the list is None
                     # if None - change it to empty {}
                     map_func_kw = [{} if kw is None else kw for kw in map_func_kw]
@@ -830,22 +879,22 @@
     .. plot::
         :context: close-figs
 
         >>> g = isns.rgbplot(astronaut(), orientation="h")
     """
 
     if not data.ndim == 3:
-        raise ValueError("imput image must be a RGB image")
+        raise ValueError("input image must be a RGB image")
 
     if data.shape[-1] != 3:
         raise ValueError("input image must be a RGB image")
 
     # if no cmap, assign reds, greens and blues cmap
     if cmap is None:
-        cmap = ["Reds", "Greens", "Blues"]
+        cmap = ["R", "G", "B"]
 
     # split RGB channels
     _d = [data[:, :, 0], data[:, :, 1], data[:, :, 2]]
 
     g = ImageGrid(
         _d,
         height=height,
@@ -1055,15 +1104,14 @@
         cbar_log=False,
         cbar_label=None,
         cbar_ticks=None,
         showticks=False,
         despine=None,
         **kwargs,
     ):
-
         if data is None:
             raise ValueError("image data can not be None")
 
         if map_func is None:
             raise ValueError("'map_func' can not be None; must be a string or callable")
 
         row_params = []
```

### Comparing `seaborn_image-0.5.2/src/seaborn_image/utils.py` & `seaborn_image-0.6.0/src/seaborn_image/utils.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.5.2/setup.py` & `seaborn_image-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'scipy>=1.5.1']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib_metadata>=1.7.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'seaborn-image',
-    'version': '0.5.2',
+    'version': '0.6.0',
     'description': 'Attractive, descriptive and effective image visualization with seaborn-like API built on top of matplotlib',
     'long_description': '# seaborn-image: image data visualization\n\n[![Tests](https://github.com/SarthakJariwala/seaborn-image/workflows/Tests/badge.svg)](https://github.com/SarthakJariwala/seaborn-image/actions?workflow=Tests)\n[![Codecov](https://codecov.io/gh/SarthakJariwala/seaborn-image/branch/master/graph/badge.svg)](https://codecov.io/gh/SarthakJariwala/seaborn-image)\n[![PyPI](https://img.shields.io/pypi/v/seaborn-image.svg)](https://pypi.org/project/seaborn-image/)\n[![Documentation Status](https://readthedocs.org/projects/seaborn-image/badge/?version=latest)](https://seaborn-image.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\n<div class="row">\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_image_hist.html">\n  <img src="./images/sphx_glr_plot_image_hist_001.png" height="120" width="170">\n  </a>\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_filter.html">\n  <img src="./images/sphx_glr_plot_filter_001.png" height="120" width="130">\n  </a>\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_fft.html">\n  <img src="./images/sphx_glr_plot_fft_001.png" height="120" width="120">\n  </a>\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_filtergrid.html">\n  <img src="./images/sphx_glr_plot_filtergrid_001.png" height="120" width="120">\n  </a>\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_image_robust.html">\n  <img src="./images/sphx_glr_plot_image_robust_001.png" height="120" width="260">\n  </a>\n\n</div>\n\n\n## Description\n\nSeaborn-image is a Python **image** visualization library based on matplotlib\nand provides a high-level API to **draw attractive and informative images quickly and effectively**.\n\nIt is heavily inspired by [seaborn](https://seaborn.pydata.org/), a high-level visualization library\nfor drawing attractive statistical graphics in Python.\n\n## Documentation\n\nDetailed documentation can be found [here](https://seaborn-image.readthedocs.io/).\n\n- [Tutorial](https://seaborn-image.readthedocs.io/en/latest/tutorial.html)\n- [Examples](https://seaborn-image.sarthakjariwala.com/en/latest/auto_examples/index.html)\n- [API Reference](https://seaborn-image.readthedocs.io/en/latest/reference.html)\n\n## Installation\n\nFor latest release:\n\nUsing `pip`\n\n```bash\npip install -U seaborn-image\n```\n\nUsing `conda`\n\n```bash\nconda install seaborn-image -c conda-forge\n```\n\nFor latest commit\n```bash\npip install git+https://github.com/SarthakJariwala/seaborn-image\n```\n\n## Contributing\n\nPlease see the [contributing guidelines](https://github.com/SarthakJariwala/seaborn-image/blob/master/CONTRIBUTING.rst)\n',
     'author': 'Sarthak Jariwala',
     'author_email': 'contact@sarthakjariwala.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SarthakJariwala/seaborn-image',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['seaborn_image'] package_data = \ {'': ['*']}
 install_requires = \ ['matplotlib-scalebar>=0.7.0,<0.9.0', 'matplotlib>=3.2.2',
 'palettable>=3.3.0', 'pooch>=1.2.0', 'scikit-image>=0.17.2', 'scipy>=1.5.1']
 extras_require = \ {':python_version < "3.8"':
 ['importlib_metadata>=1.7.0,<2.0.0']} setup_kwargs = { 'name': 'seaborn-image',
-'version': '0.5.2', 'description': 'Attractive, descriptive and effective image
+'version': '0.6.0', 'description': 'Attractive, descriptive and effective image
 visualization with seaborn-like API built on top of matplotlib',
 'long_description': '# seaborn-image: image data visualization\n\n[![Tests]
 (https://github.com/SarthakJariwala/seaborn-image/workflows/Tests/badge.svg)]
 (https://github.com/SarthakJariwala/seaborn-image/actions?workflow=Tests)\n[!
 [Codecov](https://codecov.io/gh/SarthakJariwala/seaborn-image/branch/master/
 graph/badge.svg)](https://codecov.io/gh/SarthakJariwala/seaborn-image)\n[!
 [PyPI](https://img.shields.io/pypi/v/seaborn-image.svg)](https://pypi.org/
```

### Comparing `seaborn_image-0.5.2/PKG-INFO` & `seaborn_image-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-image
-Version: 0.5.2
+Version: 0.6.0
 Summary: Attractive, descriptive and effective image visualization with seaborn-like API built on top of matplotlib
 Home-page: https://github.com/SarthakJariwala/seaborn-image
 License: MIT
 Author: Sarthak Jariwala
 Author-email: contact@sarthakjariwala.com
 Requires-Python: >=3.8,<3.11
 Classifier: Framework :: Matplotlib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seaborn-image Version: 0.5.2 Summary: Attractive,
+Metadata-Version: 2.1 Name: seaborn-image Version: 0.6.0 Summary: Attractive,
 descriptive and effective image visualization with seaborn-like API built on
 top of matplotlib Home-page: https://github.com/SarthakJariwala/seaborn-image
 License: MIT Author: Sarthak Jariwala Author-email: contact@sarthakjariwala.com
 Requires-Python: >=3.8,<3.11 Classifier: Framework :: Matplotlib Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

