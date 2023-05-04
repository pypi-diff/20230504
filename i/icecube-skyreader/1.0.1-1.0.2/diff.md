# Comparing `tmp/icecube-skyreader-1.0.1.tar.gz` & `tmp/icecube-skyreader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-1.0.1.tar", last modified: Thu Apr 20 20:24:34 2023, max compression
+gzip compressed data, was "icecube-skyreader-1.0.2.tar", last modified: Thu May  4 17:43:34 2023, max compression
```

## Comparing `icecube-skyreader-1.0.1.tar` & `icecube-skyreader-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:24:34.076069 icecube-skyreader-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-20 20:24:31.000000 icecube-skyreader-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-20 20:24:34.076069 icecube-skyreader-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-04-20 20:24:31.000000 icecube-skyreader-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:24:34.076069 icecube-skyreader-1.0.1/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-20 20:24:34.000000 icecube-skyreader-1.0.1/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-04-20 20:24:34.000000 icecube-skyreader-1.0.1/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:24:34.000000 icecube-skyreader-1.0.1/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-20 20:24:34.000000 icecube-skyreader-1.0.1/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-20 20:24:34.000000 icecube-skyreader-1.0.1/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1762 2023-04-20 20:24:34.076069 icecube-skyreader-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-20 20:24:31.000000 icecube-skyreader-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:24:34.076069 icecube-skyreader-1.0.1/skyreader/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-20 20:24:31.000000 icecube-skyreader-1.0.1/skyreader/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-04-20 20:24:31.000000 icecube-skyreader-1.0.1/skyreader/event_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:24:34.076069 icecube-skyreader-1.0.1/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:24:31.000000 icecube-skyreader-1.0.1/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9057 2023-04-20 20:24:31.000000 icecube-skyreader-1.0.1/skyreader/plot/plotting_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 20:24:31.000000 icecube-skyreader-1.0.1/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)    47095 2023-04-20 20:24:31.000000 icecube-skyreader-1.0.1/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:43:34.785717 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-04 17:43:34.000000 icecube-skyreader-1.0.2/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-04 17:43:31.000000 icecube-skyreader-1.0.2/skyreader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/event_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 17:43:34.789717 icecube-skyreader-1.0.2/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9057 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/plot/plotting_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)    47027 2023-05-04 17:43:30.000000 icecube-skyreader-1.0.2/skyreader/result.py
```

### Comparing `icecube-skyreader-1.0.1/LICENSE` & `icecube-skyreader-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.1/PKG-INFO` & `icecube-skyreader-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.0.1
+Version: 1.0.2
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.0.1/README.md` & `icecube-skyreader-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.1/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-1.0.2/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.0.1
+Version: 1.0.2
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.0.1/setup.cfg` & `icecube-skyreader-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.1/skyreader/__init__.py` & `icecube-skyreader-1.0.2/skyreader/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skyreader-1.0.1/skyreader/event_metadata.py` & `icecube-skyreader-1.0.2/skyreader/event_metadata.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.1/skyreader/plot/plotting_tools.py` & `icecube-skyreader-1.0.2/skyreader/plot/plotting_tools.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.0.1/skyreader/result.py` & `icecube-skyreader-1.0.2/skyreader/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 import healpy
 import matplotlib
 import meander
 import numpy as np
 import pandas as pd
 from astropy.io import ascii
 from matplotlib import pyplot as plt
-from matplotlib import text
+from matplotlib import text, patheffects
 
 from .event_metadata import EventMetadata
 
+from .plot.plotting_tools import format_fits_header, hp_ticklabels, plot_catalog, DecFormatter, RaFormatter
+
 ###############################################################################
 # DATA TYPES
 
 
 class PyDictNSidePixels(TypedDict):
     columns: List[str]
     metadata: Dict[str, Any]
@@ -537,15 +539,14 @@
 
     def create_plot(self,
                     dosave=False,
                     dozoom=False,
                     log_func=None,
                     upload_func=None,
                     final_channels=None):
-        from .plotting_tools import DecFormatter, RaFormatter
 
         if log_func is None:
             def log_func(x):
                 print(x)
 
         if upload_func is None:
             def upload_func(file_buffer, name, title):
@@ -751,16 +752,14 @@
             ax.set_aspect('equal')
         ax.tick_params(axis='x', labelsize=10)
         ax.tick_params(axis='y', labelsize=10)
 
         # show the grid
         ax.grid(True, color='k', alpha=0.5)
 
-        from matplotlib import patheffects
-
         # Otherwise, add the path effects.
         effects = [patheffects.withStroke(linewidth=1.1, foreground='w')]
         for artist in ax.findobj(text.Text):
             artist.set_path_effects(effects)
 
         # remove white space around figure
         spacing = 0.01
@@ -794,15 +793,14 @@
                            extra_dec=np.nan,
                            extra_radius=np.nan,
                            systematics=False,
                            plot_bounding_box=False,
                            plot_4fgl=False,
                            final_channels=None):
         """Uses healpy to plot a map."""
-        from .plotting_tools import format_fits_header, hp_ticklabels, plot_catalog
 
         if log_func is None:
             def log_func(x):
                 print(x)
 
         if upload_func is None:
             def upload_func(file_buffer, name, title):
```

