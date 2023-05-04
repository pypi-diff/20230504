# Comparing `tmp/afloat-0.0.9.tar.gz` & `tmp/afloat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afloat-0.0.9.tar", last modified: Mon May  1 14:29:18 2023, max compression
+gzip compressed data, was "afloat-0.1.0.tar", last modified: Thu May  4 03:57:08 2023, max compression
```

## Comparing `afloat-0.0.9.tar` & `afloat-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.746236 afloat-0.0.9/
--rw-rw-rw-   0        0        0     1325 2022-08-09 17:09:53.000000 afloat-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      239 2023-05-01 14:29:18.744235 afloat-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1751 2022-08-09 15:09:43.000000 afloat-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.696240 afloat-0.0.9/afloat/
--rw-rw-rw-   0        0        0      240 2023-05-01 14:28:14.000000 afloat-0.0.9/afloat/__init__.py
--rw-rw-rw-   0        0        0    16757 2023-01-19 02:20:55.000000 afloat-0.0.9/afloat/bottom_lander.py
--rw-rw-rw-   0        0        0    13218 2022-12-07 02:43:21.000000 afloat-0.0.9/afloat/clean.py
--rw-rw-rw-   0        0        0     2370 2022-08-16 11:21:50.000000 afloat-0.0.9/afloat/currents.py
--rw-rw-rw-   0        0        0    12146 2022-01-22 05:49:30.000000 afloat-0.0.9/afloat/netcdf.py
--rw-rw-rw-   0        0        0     7419 2023-04-27 06:11:19.000000 afloat-0.0.9/afloat/operational.py
--rw-rw-rw-   0        0        0     3365 2022-04-19 11:48:03.000000 afloat-0.0.9/afloat/pca.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.719244 afloat-0.0.9/afloat/plot/
--rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.9/afloat/plot/__init__.py
--rw-rw-rw-   0        0        0     6711 2023-03-03 13:23:31.000000 afloat-0.0.9/afloat/plot/gif.py
--rw-rw-rw-   0        0        0    15402 2022-08-16 12:11:30.000000 afloat-0.0.9/afloat/plot/plotting.py
--rw-rw-rw-   0        0        0     1520 2023-04-27 13:53:14.000000 afloat-0.0.9/afloat/sentinel.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.725245 afloat-0.0.9/afloat/sfodautils/
--rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.9/afloat/sfodautils/__init__.py
--rw-rw-rw-   0        0        0     8537 2023-05-01 13:37:05.000000 afloat-0.0.9/afloat/sfodautils/harmonic_analysis.py
--rw-rw-rw-   0        0        0     1821 2022-01-21 01:42:50.000000 afloat-0.0.9/afloat/shape.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.732248 afloat-0.0.9/afloat/tides/
--rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.9/afloat/tides/__init__.py
--rw-rw-rw-   0        0        0    12795 2022-08-09 16:36:10.000000 afloat-0.0.9/afloat/tides/cons.py
--rw-rw-rw-   0        0        0    11409 2022-12-06 08:25:41.000000 afloat-0.0.9/afloat/time.py
--rw-rw-rw-   0        0        0    26775 2022-12-07 02:44:11.000000 afloat-0.0.9/afloat/timeseries.py
--rw-rw-rw-   0        0        0     2755 2021-09-22 07:39:10.000000 afloat-0.0.9/afloat/xr.py
--rw-rw-rw-   0        0        0    42626 2022-08-09 16:55:55.000000 afloat-0.0.9/afloat/xrwrap.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.739234 afloat-0.0.9/afloat/xutils/
--rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.0.9/afloat/xutils/__init__.py
--rw-rw-rw-   0        0        0    26195 2022-02-28 02:28:59.000000 afloat-0.0.9/afloat/xutils/windrose.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:29:18.712242 afloat-0.0.9/afloat.egg-info/
--rw-rw-rw-   0        0        0      239 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 14:29:18.000000 afloat-0.0.9/afloat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 14:29:18.747236 afloat-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-05-01 14:28:46.000000 afloat-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:57:08.742522 afloat-0.1.0/
+-rw-rw-rw-   0        0        0     1325 2022-08-09 17:09:53.000000 afloat-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      239 2023-05-04 03:57:08.742522 afloat-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1959 2023-05-02 11:13:21.000000 afloat-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 03:57:08.614503 afloat-0.1.0/afloat/
+-rw-rw-rw-   0        0        0      442 2023-05-04 03:33:33.000000 afloat-0.1.0/afloat/__init__.py
+-rw-rw-rw-   0        0        0    16757 2023-01-19 02:20:55.000000 afloat-0.1.0/afloat/bottom_lander.py
+-rw-rw-rw-   0        0        0    14012 2023-05-03 05:09:42.000000 afloat-0.1.0/afloat/clean.py
+-rw-rw-rw-   0        0        0     1050 2023-05-02 12:08:42.000000 afloat-0.1.0/afloat/config.py
+-rw-rw-rw-   0        0        0     2370 2022-08-16 11:21:50.000000 afloat-0.1.0/afloat/currents.py
+-rw-rw-rw-   0        0        0    12146 2022-01-22 05:49:30.000000 afloat-0.1.0/afloat/netcdf.py
+-rw-rw-rw-   0        0        0     7419 2023-04-27 06:11:19.000000 afloat-0.1.0/afloat/operational.py
+-rw-rw-rw-   0        0        0     3365 2022-04-19 11:48:03.000000 afloat-0.1.0/afloat/pca.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:57:08.670508 afloat-0.1.0/afloat/plot/
+-rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.1.0/afloat/plot/__init__.py
+-rw-rw-rw-   0        0        0     6711 2023-03-03 13:23:31.000000 afloat-0.1.0/afloat/plot/gif.py
+-rw-rw-rw-   0        0        0    17268 2023-05-02 12:17:29.000000 afloat-0.1.0/afloat/plot/plotting.py
+-rw-rw-rw-   0        0        0     1520 2023-04-27 13:53:14.000000 afloat-0.1.0/afloat/sentinel.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:57:08.694509 afloat-0.1.0/afloat/sfodautils/
+-rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.1.0/afloat/sfodautils/__init__.py
+-rw-rw-rw-   0        0        0     8537 2023-05-01 13:37:05.000000 afloat-0.1.0/afloat/sfodautils/harmonic_analysis.py
+-rw-rw-rw-   0        0        0     2133 2023-05-03 10:18:33.000000 afloat-0.1.0/afloat/shape.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:57:08.710511 afloat-0.1.0/afloat/tides/
+-rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.1.0/afloat/tides/__init__.py
+-rw-rw-rw-   0        0        0    12795 2022-08-09 16:36:10.000000 afloat-0.1.0/afloat/tides/cons.py
+-rw-rw-rw-   0        0        0    11847 2023-05-03 10:31:41.000000 afloat-0.1.0/afloat/time.py
+-rw-rw-rw-   0        0        0    30469 2023-05-03 04:46:54.000000 afloat-0.1.0/afloat/timeseries.py
+-rw-rw-rw-   0        0        0     2790 2023-05-01 14:45:31.000000 afloat-0.1.0/afloat/xr.py
+-rw-rw-rw-   0        0        0    42626 2022-08-09 16:55:55.000000 afloat-0.1.0/afloat/xrwrap.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:57:08.734514 afloat-0.1.0/afloat/xutils/
+-rw-rw-rw-   0        0        0        0 2023-05-01 14:07:32.000000 afloat-0.1.0/afloat/xutils/__init__.py
+-rw-rw-rw-   0        0        0    26288 2023-05-02 14:09:01.000000 afloat-0.1.0/afloat/xutils/windrose.py
+drwxrwxrwx   0        0        0        0 2023-05-04 03:57:08.638502 afloat-0.1.0/afloat.egg-info/
+-rw-rw-rw-   0        0        0      239 2023-05-04 03:57:07.000000 afloat-0.1.0/afloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-05-04 03:57:08.000000 afloat-0.1.0/afloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 03:57:07.000000 afloat-0.1.0/afloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-04 03:57:07.000000 afloat-0.1.0/afloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-04 03:57:07.000000 afloat-0.1.0/afloat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 03:57:08.742522 afloat-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-05-04 03:56:52.000000 afloat-0.1.0/setup.py
```

### Comparing `afloat-0.0.9/LICENSE` & `afloat-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/README.md` & `afloat-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 - Logical API rather than a dump of modules
 - Use of xarray accessors 
 - Pip installable through pipy
 
 ## Documentation
 The documentation can be found [here](https://iosonobert.github.io/afloat/).
 
+## Config file
+For full functionality you'll need a .afloatcongig file in your home directory [USERPROFILE directory in Windows]. The file should contain:
+
+afloat-extras: <path to afloat-extras folder>
+
 ## Other names:
 - **B**asic **O**cean **A**nalysis **T**ools [BOAT Taken on pypi]
 - **G**eneral **O**cean **A**nalysis **T**ools [GOAT Taken on pypi]
 - **B**asic **E**nvironmental **A**nalysis **T**ools [BEAT Taken on pypi]
 
 <!-- ![alt text](./doc/unlicensed_goat.jpg) -->
 <!-- ![alt text](./sphinx/goatafloat.jpg) -->
```

### Comparing `afloat-0.0.9/afloat/bottom_lander.py` & `afloat-0.1.0/afloat/bottom_lander.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/clean.py` & `afloat-0.1.0/afloat/clean.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 """
-Various tools for quality controling or otherwise preprocessing turbulenec timeseries data, including:
-
-Functions
-=========
-    - unwrap:               phase unwrapping pulse coherent velocity records
-    - goring_nikora_2002:   despike by the method of goring and nikora 2002
-
-For more conventional QAQC use the pIMOS library. 
+Various tools for quality controling or otherwise preprocessing turbulence timeseries data. For more conventional QAQC use the pIMOS library. 
 
 These functions work on continuous individual blocks of data. If they are to be done blockwise 
 this must be handled elsewhere.   
 
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import path as mplpath
 
 def unwrap(x, prev_block_median, ambiguity_velocity=0.23, verbose = False):
     """
     Unwrap a block of data, or don't if not needed:
 
-    Inputs
-    ======
-
-        - x: The block of data
-        - prev_block_median: the median of the previous block, to help determine whether its wrapped high or low. 
-
-    Outputs
-    =======
-
-        - thats_a_wrap: boolean, true if wrapped, false if not wrapped
-        - X: output data. equal to  x if the block was not deemed to be wrapped, or an unwrapped version otherwise. 
+    Parameters
+    ----------
+    x : np.array
+        The block of data that is potentially wrapped
+    prev_block_median : numeric
+        The median of the previous block. This is used in the event of a phase wrap to help determine whether its wrapped likely wrapped high or low. 
+    ambiguity_velocity(optional) : numeric
+        This is the +/- ambiguity point that maps to +/- pi. Default is 0.23, which is very specific and prob shouldn't be a default. 
+
+    Returns
+    -------
+    thats_a_wrap: boolean
+        Flag for wrap detection. True if wrapped, False if not wrapped.
+    X : np.array
+        Output data. Equal to  x if the block was not deemed to be wrapped, or an unwrapped version otherwise. 
 
     """
 
     def detect_wrap(x, prev_block_median, ambiguity_velocity, verbose = False):
         """
         Detect whether wrap is suspected. Method is to do a test unwrap (direction does not matter) 
         and compare the new variance with the old. If it goes down it's assumed to be wrapped. 
@@ -127,24 +124,46 @@
         else:
             print('I''m wrapped that it isn''t wrapped')
 
     return thats_a_wrap, X 
  
 def despike(u, fs, interp_opt='linear', intensity = 0.9, verbose=False):
     """
-    Despike a block of data. Binning to be done outside. Same as despikei but returns the first output only.  
+    Despike a single block of data. Binning to be done outside. Same as despikei but returns the first output only.  
+
+    See also
+    --------
+
+    afloat.clean.despikei
+
     """
 
     U, di = despikei(u, fs, interp_opt='linear', intensity = 0.9, verbose=False)
 
     return U
 
 def despikei(u, fs, interp_opt='linear', intensity = 0.9, verbose=False):
     """
-    Despike a block of data. Binning to be done outside.  
+    Despike a single block of data. Binning to be done outside.  
+
+    Parameters
+    ----------
+    u : np.array
+        Data to be despiked. Assumed to be well spaced in the dimension that it is sampled (time or space).
+    fs : numeric
+        The sample frequency of the data.
+    intensity : numeric
+        The intensity threshold used in the phase space method.
+
+    Returns
+    -------
+    U : np.array
+        Despiked u array
+    di : 
+        Indices of modified data
 
     """
 
     def phase_space_thres(u, fs, intensity = 0.9, verbose=False):
         """
         This function actually detects the spikes and nans them out. Single block, single component. 
         """
@@ -296,34 +315,42 @@
         plt.plot(u)
         plt.plot(U)
 
     return U, di
 
 def logical_clean(x, index):
     """
-    Interpolate over values indicated by some index. 
+    Remove data indicated by a logiocal index and interpolate over the gaps created.  
     """
 
     xo = x.copy()
     xo[index] = np.nan
 
     xo = fillgaps(xo)
 
     return xo
 
 def nan_helper(y):
     """Helper to handle indices and logical indices of NaNs.
 
-    Input:
-        - y, 1d numpy array with possible NaNs
-    Output:
-        - nans, logical indices of NaNs
-        - index, a function, with signature indices= index(logical_indices),
+    Parameters
+    ----------
+    y : 1d numpy array 
+        Data record with possible NaNs
+
+    Returns
+    -------
+    nans : np.array
+        Array of bools - logical indices of NaNs
+    index : function
+        A function, with signature indices=index(logical_indices),
           to convert logical indices of NaNs to 'equivalent' indices
-    Example:
+    
+    Example
+    -------
         >>> # linear interpolation of NaNs
         >>> nans, x= nan_helper(y)
         >>> y[nans]= np.interp(x(nans), x(~nans), y[~nans])
     """
 
     return np.isnan(y), lambda z: z.nonzero()[0]
 
@@ -371,15 +398,15 @@
       The dimension to operate along.
 
     extrapFlg : bool (optional: False)
       Whether to extrapolate if NaNs are found at the ends of the
       array.
 
     See Also
-    =====
+    --------
 
     interpgaps : Linearly interpolates in time.
 
     Notes
     =====
 
     This function interpolates assuming spacing/timestep between
```

### Comparing `afloat-0.0.9/afloat/currents.py` & `afloat-0.1.0/afloat/currents.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/netcdf.py` & `afloat-0.1.0/afloat/netcdf.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/operational.py` & `afloat-0.1.0/afloat/operational.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/pca.py` & `afloat-0.1.0/afloat/pca.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/plot/gif.py` & `afloat-0.1.0/afloat/plot/gif.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/plot/plotting.py` & `afloat-0.1.0/afloat/plot/plotting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.collections import LineCollection
+from matplotlib.collections import PolyCollection
+import os, warnings
+import afloat.config as config
 
-import os
+extras_folder = config.get('afloat-extras', home_dir=None)
 
 class axis_layer():
     """
     A class to assist in laying out axes for publication. 
 
     ...
 
@@ -393,46 +396,104 @@
     This just hides the y ticks of an axis. I'm surprised there isn't a simple matplotlib command for this.
         Inputs: 
                 ax - single axis object for which the ticks must be written.  
     """
     for tick in ax.axes.get_yticklabels():
         tick.set_visible(False)
 
-def auscoast_fill(ax=None, sandpit_folder=None, fill_kwargs={}):
+def global_coast_fill(ax=None, resolution='crude', collection_kwargs={'color': '0.5'}):
+    """
+    matplotlib fill global coast. 
+
+    Needs afloat-extras and a proper .afloatconfig file. See github. 
+
+    """
+
+    if not os.path.exists(extras_folder):
+        raise(Exception('sandpit required to run this function'))
+
+    ress = ['full', 'high', 'intermediate', 'low', 'crude']
+    ress = ress + [res[0] for res in ress]
+
+    if not resolution.lower() in ress:
+        raise(Exception('Resolution must be one of [{}]'.format(', '.join(ress))))
+    
+    resolution = resolution[0].lower()
+    print('Selected resolution: {}'.format(resolution))
+
+    sf = 'data/spatial/coastlines/global_coastline/gshhg-shp-2.3.7/GSHHS_shp/{res}/GSHHS_{res}_L1.shp'.format(res=resolution)
+    sf =  os.path.join(extras_folder, sf)
+
+    verts = quick_shape_fill(sf, ax=ax, collection_kwargs=collection_kwargs)
+
+def auscoast_fill(ax=None, sandpit_folder=None, collection_kwargs={'color': '0.5'}):
     """
     matplotlib fill australian coast. 
 
     Need to figure out why some of the polygons don't render properly with fill but look fine in QGIS. 
 
-    Won't work if you don't have the sandpit, i.e. if pulled from github. 
+    Needs afloat-extras and a proper .afloatconfig file. See github. 
 
     """
 
-    import shapefile
-
-    if sandpit_folder is None:
-        sandpit_folder = os.path.join(os.path.split(__file__)[0], '../sandpit')
+    if not sandpit_folder is None:
+        warnings.warn("No longer specify this, use .afloatconfig file instead.")
     
     # print(sandpit_folder)
     # print(os.listdir(sandpit_folder))
 
-    if not os.path.exists(sandpit_folder):
+    if not os.path.exists(extras_folder):
         raise(Exception('sandpit required to run this function'))
 
-    sf =  os.path.join(sandpit_folder, 'data/spatial/coastlines/ivica/Australia_NWS_polygons.shp')
+    sf =  os.path.join(extras_folder, 'data/spatial/coastlines/ivica/Australia_NWS_polygons.shp')
+
+    verts = quick_shape_fill(sf, ax=ax, collection_kwargs=collection_kwargs)
+    
+    return verts
+
+def quick_shape_fill(sf, ax=None, collection_kwargs={}):
+
+    import shapefile
 
     if ax is None:
         ax = plt.gca()
 
     sf = shapefile.Reader(sf)
 
+    verts = []
+    for shape in sf.shapeRecords():
+        x = [i[0] for i in shape.shape.points[:]]
+        y = [i[1] for i in shape.shape.points[:]]
+        # ax.fill(x, y, '0.5', **fill_kwargs)
+        verts += [list(zip(x, y))]
+
+    poly = PolyCollection(verts, **collection_kwargs)
+    # poly.set_alpha(alpha)
+
+    ax.add_collection(poly)
+
+    return verts
+
+def quick_shape_fill_slow(sf, ax=None, fill_kwargs={}):
+
+    import shapefile
+
+    if ax is None:
+        ax = plt.gca()
+
+    sf = shapefile.Reader(sf)
+
+    verts = []
     for shape in sf.shapeRecords():
         x = [i[0] for i in shape.shape.points[:]]
         y = [i[1] for i in shape.shape.points[:]]
         ax.fill(x, y, '0.5', **fill_kwargs)
+        verts += [list(zip(x, y))]
+
+    return verts
 
 def quick_shape_plot(sf, ax=None, plot_kwargs={'lw':0.5}, **kwargs):
     """
     Inputs:
 
     kwargs:
         label: a label that applies to only the first segment [prevents multi labels]
```

### Comparing `afloat-0.0.9/afloat/sentinel.py` & `afloat-0.1.0/afloat/sentinel.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/sfodautils/harmonic_analysis.py` & `afloat-0.1.0/afloat/sfodautils/harmonic_analysis.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/shape.py` & `afloat-0.1.0/afloat/shape.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+"""
+Some basic tools for interacting with shapefiles. afloat-extras and proper config file required for full functionality.
+"""
 import pandas as pd
 import matplotlib.pyplot as plt 
 import shapefile
 
 
 def xyzbathy_2_contourshp(infiles, outfile, levels, field_name='DEPTH', ):
     """
-    Function to convert xyz data into shapefiles of contours. Nominally it is for bathymetry, 
+    Function to convert xyz scatter data into shapefiles of contours. Nominally it is for bathymetry, 
     a different field_name can be used for other scalars. 
 
-    Inputs:
-        infiles - xyx csv [or iterable of] with headers X, Y, Z [in capitals]
-        outfile - name of the shapefile to be produced
-        levels - the levels the contours are to be specified at.
-        field_name - the field name that the scalar field (Z, column) will be written 
-                to in the shp file. 
+    Parameters
+    ----------
+        infiles: string or list 
+            Path of xyx formatted csv [or iterable of paths]. Use the headers X, Y, Z [in capitals]
+        outfile: string
+            Path of the shapefile to be produced
+        levels: iterable 
+            The levels the contours are to be specified at. Takes an iterable of numeric values.
+        field_name: string
+            The field name that the scalar field (Z, column) will be written to in the shp file. Default is "DEPTH" 
     """
 
     if type(infiles) == str:
         infiles = [infiles]
     
     CSs = []
```

### Comparing `afloat-0.0.9/afloat/tides/cons.py` & `afloat-0.1.0/afloat/tides/cons.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/time.py` & `afloat-0.1.0/afloat/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,32 @@
 my_datum = datetime.datetime(1990,1,1)
 
 def linspacetime(start, end, n=None, dt_s=None):
     """
     Create a linearly spaced np array of datetime objects. Currently uses pandas but could be done 
     with linspace and one of the ordinal time tools if I ever start to care about dependencies.
     
-    Inputs:
-     - start: datetime object for start of array. 
-     - end: datetime object for end of array. 
-     - n: number of points in array [use None if using dt_s]
-     - dt_s: number of seconds between points in the array [use None if using n]
+    Parameters
+    ----------
+     start: datetime object 
+        Start time of the desired of time vector. 
+     end: datetime object 
+        End time of the desired of time vector. 
+     n: int
+        Number of points in array [use None if using dt_s]
+     dt_s: numeric 
+        Spacing of the desired of time vector in seconds [use None if using n]
 
      If specifying dt_s, array will start from start, and be spaced perfectly by dt_s, ending at or before
      end.
+
+    Returns
+    -------
+    time: no.array
+        A spaced time vector
     """
 
     if n==None and dt_s==None:
         raise Exception('Must specify n or dt_s')
     elif (not n==None) and (not dt_s==None):
         raise Exception('Must specify only one of n or dt_s')
     elif not dt_s==None: # must calculate new end and n
@@ -53,20 +63,22 @@
 
 def is_well_spaced(date, fs, epsilon=0.01, verbose=False):
     """
     A function to determine whether a time array is well spaced at fs. This is necessary to determine 
     if we wish to block 'blindly' average over time T = n/fs where n is a constant set numbers of 
     samples and fs is the sample frequency.
     
-    Inputs:
-     - date: numpy row vector of datetime objects. 
-     - fs: sample frequncy in Hz
-     
-    Optional inputs:
-     - epsilon: maximum deviation from the specified fs
+    Parameters
+    ----------
+    date: np.array row vector of datetime objects
+        An input time vector to check for even spacing 
+    fs: numeric
+        The believed sample frequncy in Hz. Will check that this is the appropriate spacing (to some tolerance)
+    epsilon(optional): numeric 
+        Maximum deviation from the specified fs
     """
 
     # validation.is_np_date_rowvector(date)
 
     if type(date[0]) == datetime.datetime:
         max_dt = np.max(np.diff(date))
         min_dt = np.min(np.diff(date))
@@ -88,14 +100,18 @@
     elif min_dt < min_allow:
         raise Exception('Minimum time spacing of {} smaller than allowable [{}].'.format(min_dt, min_allow))
     else:
         if verbose:
             print('Time vector is well spaced')
 
 def datetime_2_timestamp(date_in):
+    """
+    Convert an array of datetime objects to pandas timestamps. 
+    """
+
 
     date_out = np.array([datetime.datetime.timestamp(date_in[i]) for i in np.arange(0, len(date_in))])
 
     return date_out
 
 def timestamp_2_datetime(date_in):
```

### Comparing `afloat-0.0.9/afloat/timeseries.py` & `afloat-0.1.0/afloat/timeseries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
-Rapid implementation timeseries analysis. 
+Rapid implementation timeseries analysis.
 
-Collection of utilities for timeseries analysis with a focus on rapid implementation, not rapid runtimes. Code interfaces with numpy, scipy, xarray, matplotlib  
+This module contains a collection of utilities for timeseries analysis with a focus on rapid implementation, not rapid runtimes. 
+Code interfaces with numpy, scipy, xarray, matplotlib. Much of this is becoming obsolete with the increasing power of xarray. 
 
 """
 
 import numpy as np, scipy.signal as signal, xarray as xr
 import matplotlib.pyplot as plt
 
 import afloat.time as ztime
@@ -33,25 +34,29 @@
 class DataSet():
     """
     Accessor for xarray DataSet.
 
     Accessor for xarray DataSet which provides functionality for rapid implementation of timeseries analysis.
 
     Parameters
-        ds : xarray.DataSet
-            The DataSet to be accessed
+    ----------
+    ds : xarray.DataSet
+        The DataSet to be accessed
 
     Returns
-        ds : timeseries.DataSet
-            The xarray accessor object
+    -------
+    ds : timeseries.DataSet
+        The xarray accessor object
 
     Examples
-        XXXXXXXX
+    --------
+        XXXXXXXXYYYYYYYYZZZZZZZZZZ
 
     See Also
+    --------
         xarray.DataSet
     """
 
     def __init__(self, ds): 
     
         self._obj = ds
 
@@ -71,25 +76,29 @@
 class DataArray():
     """
     Accessor for xarray DataArray.
 
     Accessor for xarray DataArray which provides functionality for rapid implementation of timeseries analysis.
 
     Parameters
-        da : xarray.DataArray
-            The DataArray to be accessed
+    ----------
+    da : xarray.DataArray
+        The DataArray to be accessed
 
     Returns
-        da : timeseries.DataArray
-            The xarray accessor object
+    -------
+    da : timeseries.DataArray
+        The xarray accessor object
 
     Examples
-        XXXXXXXX
+    --------
+        XXXXXXXXYYYYYYYYZZZZZZZZZZ
 
     See Also
+    --------
         xarray.DataArray
     """
 
     def __init__(self, da):
 
         if 'units' in da.attrs:
             self.units = da.attrs['units']
@@ -168,14 +177,30 @@
     def rolling_tidal_harmonic(self, Fin=None, **kwargs):
 
         return self._timeseries.rolling_tidal_harmonic(Fin=Fin, **kwargs)
 
 class TimeSeries():
     """
     An object to hold timeseries data and wrap the quick timeseries methods within this module. 
+
+    Parameters
+    ----------
+    time : np.array
+        Array containing the dime variable. Dtype can be datetime.daetime or np.datetime64.
+    data : np.array
+        Array containing the data variable
+    other_dims : list of strings
+        A list containing the names of other dimensions. Required if data is multidimensional.  
+    units(optional): string
+        Units of the data set. Used for some automated plot formatting or other operations. No dynamic conversions performed.
+
+    Returns
+    -------
+
+    XXXXXXXXYYYYYYYYZZZZZZZZZZ
     """
 
     def __init__(self, time, data, other_dims=[], **kwargs):
         """
 
         """
         ## Start with no validation. Build organically. 
@@ -192,69 +217,106 @@
 
         self.time = time
         self.data = data
 
         self.units = units
 
     def plot(self, ax=None, **kwargs):
+        """
+        Very quick plot of timeseries object.
 
+        Parameters
+        ----------
+        ax(optional) : matplotlib axis object
+            Axis to plot into.
+        set_xlim(optional) : bool
+            Use this to set the axis limits to the data extent. Default is False. 
+        """
         set_xlim = kwargs.pop("set_xlim", False)
 
         if ax is None:
             ax = plt.gca()
 
         ax.plot(self.time, self.data, **kwargs)
         ax.grid('on')
 
         if set_xlim:
             ax.set_xlim([min(self.time.values), max(self.time.values)])
 
     def interp(self, **kwargs):
+        """
+        Parser for afloat.timeseries.quick_interp
+        """
 
         return quick_interp(self.time, self.data, **kwargs)
 
     def despike_gn02(self, **kwargs):
+        """
+        Parser for afloat.timeseries.quick_despike_gn02
+        """
 
         return quick_despike_gn02(self.time, self.data, **kwargs)
 
     def butter(self, **kwargs):
-
+        """
+        Parser for afloat.timeseries.butter
+        """
+        
         return quick_butter(self.time, self.data, **kwargs)
 
     def psd(self, **kwargs):
-
+        """
+        Parser for afloat.timeseries.psd
+        """
+        
         return quick_psd(self.time, self.data, data_unit=self.units, **kwargs)
 
     def psd_welch(self, **kwargs):
-
+        """
+        Parser for afloat.timeseries.quick_psd_welch
+        """
+        
         return quick_psd_welch(self.time, self.data, data_unit=self.units, **kwargs)
 
     def rolling_tidal_harmonic(self, Fin=None, **kwargs):
+        """
+        Parser for afloat.timeseries.quick_rolling_tidal_harmonic
+        """
 
         return quick_rolling_tidal_harmonic(self.time, self.data, Fin=Fin, **kwargs)
 
     def tidal_harmonic(self, Fin=None, **kwargs):
+        """
+        Parser for afloat.timeseries.quick_tidal_harmonic
+        """
 
         return quick_tidal_harmonic(self.time, self.data, Fin=Fin, **kwargs)
 
 def quick_butter(time, data, T_cut_seconds, order=4, btype='lowpass', use_sos=False):
     """
     Very quick butterworth filter that works with python time objects. 
     
-    Usage:
-        filtered = quick_butter(time, data, T_cut_seconds, order=4, btype='lowpass')
-
-    args:
-        time: numpy array of time objects that can be converted by zutils.time.seconds_since and zutils.time.is_well_spaced
-        data: np.array to be filtered. Can be higher dimensional but goes into signal.butter as is.
-        T_cut_seconds: cutoff period in seconds
-        
-    kwargs: 
-        btype: 'lowpass' or 'highpass'
-        order: order of the butterworth
+    Parameters
+    ----------
+    time : np.array
+        Numpy array of time objects that can be converted by afloat.time.seconds_since and afloat.time.is_well_spaced
+    data : np.array
+        Data to be filtered. Can be higher dimensional but goes into signal.butter as is.
+    T_cut_seconds: numeric
+        Cutoff period in seconds
+    order: numeric
+        order of the butterworth
+    btype: string
+        Type of filter, must be 'lowpass' or 'highpass'
+    use_sos: bool
+        Whether to use sos filtering
+
+    Returns:
+    out : np.array
+        Filtered signal
 
     """
 
     quick_validate(time, data)
     
     # Convert to seconds
     t_sec = ztime.seconds_since(time)
@@ -295,32 +357,37 @@
         b, a = signal.butter(order, f_cut_norm, btype)
         out = signal.filtfilt(b, a, data, axis=0)
 
     return out
 
 def quick_interp(time, data, **kwargs):
     """
-    Very quick interp of timeseries data. 
+    Very quick interp of timeseries data. Obsolete with the xarray interp.
 
-    Usage:
-        time_out_secs, time_out_np64, var_interp = quick_interp(time, data, **kwargs)
+    Parameters
+    ----------
+    time : np.array
+        Numpy array of time objects of the original record. Can be converted by afloat.time.seconds_since and afloat.time.is_well_spaced
+    data : np.array
+        Data to be interpolated
+    dt_sec : numeric
+        Timestep of the interpolated record
+    start : datetime.datetime of np.datetime64
+        Start time of the interpolated record
+    end : datetime.datetime of np.datetime64
+        End time of the interpolated record
 
-    Arguments:
-        time
-        data
-    
-    Key word arguments:
-        dt_sec
-        start
-        end
-
-    Outputs:
-        time_out_secs
-        time_out_np64 
-        var_interp
+    Returns
+    -------
+    time_out_secs : np.array
+        The interpolated time array in seconds since a base time [numeric]
+    time_out_np64 :
+        The interpolated time array as np.datetime64
+    var_interp :
+        The interpolated data
     """
     dt_sec = kwargs.pop('dt_sec', 60)
     start = kwargs.pop('start', None)
     end = kwargs.pop('end', None)
     
     dt_file = time[1] - time[0]
     print('File dt initial: {}'.format(dt_file))
@@ -353,28 +420,31 @@
 
     return time_out_secs, time_out_np64, var_interp
 
 def quick_interp_tknown(time, data, interp_time):
     """
     Very quick interp of timeseries data. Here the time vector is known. 
 
-    Usage:
-        time_out_secs, time_out_np64, var_interp = quick_interp(time, data, interp_time)
-
-    Arguments:
-        time
-        data
-        interp_time
-    
-    Key word arguments:
-        
+    Parameters
+    ----------
+    time : np.array
+        Numpy array of time objects of the original record. Can be converted by afloat.time.seconds_since and afloat.time.is_well_spaced
+    data : np.array
+        Data to be interpolated
+    interp_time : np.array
+        Numpy array of time objects to interpolate onto. 
 
-    Outputs:
-        time_out_secs
-        var_interp
+    Returns
+    -------
+    time_out_secs : np.array
+        The interpolated time array in seconds since a base time [numeric]
+    time_out_np64 :
+        The interpolated time array as np.datetime64
+    var_interp :
+        The interpolated data
     """
     
     
     ref_time = time[0]
 
     time_in_secs = ztime.seconds_since(time, ref_time)
     time_out_secs = ztime.seconds_since(interp_time, ref_time)
@@ -386,42 +456,54 @@
         var_interp = np.array([np.interp(time_out_secs, time_in_secs, var_row) for var_row in data])
 
     return time_out_secs, time_out_np64, var_interp
 
 def tslice(time, start, end):
     """
     Get a quick time index for a slice between start and end dates. Does this by first converting to seconds_since. This is not fast, but it is easy for the operator as seconds_since handles the object conversion. 
-    
-    Usage:
-        tind = tslice(time, start, end)
+ 
+    Parameters
+    ----------
+    time : np.array
+        Numpy array of time objects of the original record. Can be converted by afloat.time.seconds_since and afloat.time.is_well_spaced
+    start : datetime.datetime of np.datetime64
+        Start time of the slice index
+    end : datetime.datetime of np.datetime64
+        End time of the slice index
+
+    Returns
+    -------
+    tind : nparray
+        Numpy array logical index for the slice. 
 
-    Inputs:
-        time: Time vector
-        start: datetime.datatime np.datetime64 for the start time
-        end: datetime.datatime np.datetime64 for the end time
     """
 
     time = ztime.seconds_since(time)
     start = ztime.seconds_since(start)
     end = ztime.seconds_since(end)
     
     tind = np.logical_and(time>=start, time<=end)
     
     return tind
 
 def tnearest(time, target):
     """
     Get a quick time index for nearest point to target time. Does this by first converting to seconds_since. This is not fast, but it is easy for the operator as seconds_since handles the object conversion. 
     
-    Usage:
-        tind = tnearest(time, start, end)
+    Parameters
+    ----------
+    time : np.array
+        Numpy array of time objects of the original record. Can be converted by afloat.time.seconds_since and afloat.time.is_well_spaced
+    target : datetime.datetime of np.datetime64
+        Time point to locate
 
-    Inputs:
-        time: Time vector
-        target: datetime.datatime np.datetime64 for the target time
+    Returns
+    -------
+    tind : int
+        Linear index corresponding to the target time
     """
 
     time = ztime.seconds_since(time)
     target = ztime.seconds_since(target)
     
     d = abs(time-target)
     tind = np.where(d==min(d))[0][0]
@@ -678,15 +760,18 @@
         data_c, di = zclean.despikei(data_c, fs=fs, intensity=int_val)
         any_clean = np.logical_or(any_clean, di)
         
 
     return data_c, any_clean
 
 def quick_decompose(time, data, T_cut_low, T_cut_high, plot=False, **kwargs):
-    
+    """
+    Decompose signal into lowpass, bandpass and highpass
+    """
+
     if 'btype' in kwargs:
         raise Exception("Can't pass btype to decompose")
 
     if T_cut_low >= T_cut_high:
         raise Exception("T_cut_low >= T_cut_high")
 
     
@@ -706,37 +791,44 @@
         plt.plot([24*3600/(T_cut_high)]*2, ylim, 'r--')
         plt.gca().set_ylim(ylim)
 
     return data_lp, data_bp, data_hp
 
 
 def quick_tidal_harmonic(time, data, Fin=None, **kwargs):
-
+    """
+    Fit tidal harmonics to a data record.
+    """
+    
     freq, fout = sha.getTideFreq(Fin=Fin)
     # amp, phs, c0, data_fit, data_residual = 
     output = quick_harmonic(time, data, freq, **kwargs)
     output['fout'] = fout
 
     return output
 
 def quick_rolling_tidal_harmonic(time, data, Fin=None, **kwargs):
-
+    """
+    Fit short term tidal harmonics to a data record using sliding window.
+    """
+    
     if Fin is None:
         Fin = ['M2', 'M4', 'M6']
 
     freq, fout = sha.getTideFreq(Fin=Fin)
     output = quick_rolling_harmonic(time, data, freq, **kwargs)
     output['fout'] = fout
     output['freq'] = freq
     # output['fout'] = fout
 
     return output
 
 def quick_rolling_harmonic(time, data, omega, windowlength=3*86400.0, overlap=12*3600.0, zero_pad_nans=True, **kwargs):
     """
+    Fit short term harmonics to a data record using sliding window.
 
     kwargs:
         remove_trans_in_recon - if true this sets the window swapover point in the reconstructed harmonic signal to np.nan to limit discontinuity.
 
     """
 
     if (spec := importlib.util.find_spec('sfoda')) is not None:
@@ -821,17 +913,15 @@
     output['data_residual']     = data_residual
     output['omega']             = omega
 
     return output
 
 def quick_harmonic(time, data, omega, zero_pad_nans=True, **kwargs):
     """
-
-    kwargs:
-
+    Harmonic fit to a data record.
     """
 
     if (spec := importlib.util.find_spec('sfoda')) is not None:
         module = importlib.util.module_from_spec(spec)
         sys.modules['sfoda'] = module
         spec.loader.exec_module(module)
     else:
@@ -880,37 +970,49 @@
     output['data_fit']          = data_fit
     output['data_residual']     = data_residual
     output['omega']             = omega
 
     return output
     
 def quick_validate(time, data, verbose=False):
+    """
+    Validate that time vector is an np array, that data vector is an np array with first dimension the same size as the time vector. 
+    """
 
     assert type(time) in [np.array, np.ndarray], "Time must be an np.array"
     assert type(data) in [np.array, np.ndarray], "Data must be an np.array"
     assert len(time)==data.shape[0], "Time must be the same length as the first dimension of Data"
 
     if verbose:
         print('Validation checks passed')
 
 def window_index_time(t, windowsize, overlap):
     """
-    Determines the indices for window start and end points of a time vector
-    
-    The window does not need to be evenly spaced
-    
-    Inputs:
+    Determines the indices for sliding windows over a time vector data. 
 
-        t: list or array of datetime objects
+    The time data does not need to be evenly spaced.
+    
+    Parameters
+    ----------
+    t: list of np.array 
+        Time vector input as list or array containing time objects. 
 
-        windowsize: length of the window [seconds]
+    windowsize: numeric 
+        Length of the window [seconds]
 
-        overlap: number of overlap points [seconds]
+    overlap: int
+        Number of seconds of overlap between successive windows [seconds]
+        
+    Returns
+    -------
+    pt1 : list
+        The start indices of each window
+    pt2 : list
+        The end indices of each window
         
-    Returns: pt1,pt2 the start and end indices of each window
     """
     
     tsec = ztime.seconds_since(t)
         
     t1=tsec[0]
     t2=t1 + windowsize
     pt1=[0]
```

### Comparing `afloat-0.0.9/afloat/xr.py` & `afloat-0.1.0/afloat/xr.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #     import validation
 
 import datetime
 import numpy as np
 import xarray as xr
 import pandas as pd
  
-# Alias for backward compat
-from zutils.xrwrap import *
+# Alias for backward compat. This is now moved out of here. 
+# from afloat.xrwrap import *
 
 #%% Some code for adding seasons to xarray datasets
 
 def add_season_custom(ds, month_season_dict, custom_season_name):
     """
     Add custom season to xarray dataset.
```

### Comparing `afloat-0.0.9/afloat/xrwrap.py` & `afloat-0.1.0/afloat/xrwrap.py`

 * *Files identical despite different names*

### Comparing `afloat-0.0.9/afloat/xutils/windrose.py` & `afloat-0.1.0/afloat/xutils/windrose.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # else:
 #     import validation
 
 import datetime
 import numpy as np
 import xarray as xr
 import pandas as pd
-from mpl_toolkits.axes_grid.inset_locator import inset_axes
+from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 
 # from windrose import WindroseAxes # duplicated below now
 # import windrose # duplicated below now
 
 import matplotlib as mpl
 import locale
 
@@ -700,15 +700,16 @@
     var_bins = bins.tolist()
     var_bins.append(np.inf)
 
     if blowto:
         direction = direction + 180.
         direction[direction >= 360.] = direction[direction >= 360.] - 360
 
-    table = histogram2d(x=var, y=direction, bins=[var_bins, dir_bins], normed=False)[0]
+    # table = histogram2d(x=var, y=direction, bins=[var_bins, dir_bins], normed=False)[0]
+    table = histogram2d(x=var, y=direction, bins=[var_bins, dir_bins], density=False)[0]
     # add the last value to the first to have the table of North winds
     table[:, 0] = table[:, 0] + table[:, -1]
     # and remove the last col
     table = table[:, :-1]
     if normed:
         table = table * 100 / table.sum()
```

### Comparing `afloat-0.0.9/afloat.egg-info/SOURCES.txt` & `afloat-0.1.0/afloat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 afloat/__init__.py
 afloat/bottom_lander.py
 afloat/clean.py
+afloat/config.py
 afloat/currents.py
 afloat/netcdf.py
 afloat/operational.py
 afloat/pca.py
 afloat/sentinel.py
 afloat/shape.py
 afloat/time.py
```

### Comparing `afloat-0.0.9/setup.py` & `afloat-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 
 class BinaryDistribution(Distribution):
     def is_pure(self):
         return False
 
 		
 setup(name='afloat',
-      version='0.0.9',
+      version='0.1.0',
       description='A Fairly useful Library of Ocean Analysis Tools',
       author='Andrew Zulberti',
       author_email='andrew.zulberti@gmail.com',
       packages=find_packages(),
       install_requires=['numpy',
                         'matplotlib', 
                         'netcdf4', 
                         'scipy',
-                        'xarray'],
+                        'xarray',
+                        'utm',
+                        'pyshp',],
       license='unlicensed to all but author',
       include_package_data=True,
       distclass=BinaryDistribution,
     )
```

