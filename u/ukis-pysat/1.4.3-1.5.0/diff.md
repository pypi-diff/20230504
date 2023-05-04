# Comparing `tmp/ukis-pysat-1.4.3.tar.gz` & `tmp/ukis-pysat-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukis-pysat-1.4.3.tar", last modified: Mon Sep 19 15:46:40 2022, max compression
+gzip compressed data, was "ukis-pysat-1.5.0.tar", last modified: Thu May  4 08:19:39 2023, max compression
```

## Comparing `ukis-pysat-1.4.3.tar` & `ukis-pysat-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 15:46:40.711266 ukis-pysat-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11438 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7012 2022-09-19 15:46:40.711266 ukis-pysat-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6277 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-19 15:46:40.711266 ukis-pysat-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 15:46:40.707266 ukis-pysat-1.4.3/ukis_pysat/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/ukis_pysat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4530 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/ukis_pysat/_landsat.py
--rw-r--r--   0 runner    (1001) docker     (121)    19035 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/ukis_pysat/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    10909 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/ukis_pysat/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/ukis_pysat/members.py
--rw-r--r--   0 runner    (1001) docker     (121)    22371 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/ukis_pysat/raster.py
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-09-19 15:46:27.000000 ukis-pysat-1.4.3/ukis_pysat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 15:46:40.711266 ukis-pysat-1.4.3/ukis_pysat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7012 2022-09-19 15:46:40.000000 ukis-pysat-1.4.3/ukis_pysat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-19 15:46:40.000000 ukis-pysat-1.4.3/ukis_pysat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 15:46:40.000000 ukis-pysat-1.4.3/ukis_pysat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 15:46:40.000000 ukis-pysat-1.4.3/ukis_pysat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-09-19 15:46:40.000000 ukis-pysat-1.4.3/ukis_pysat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-19 15:46:40.000000 ukis-pysat-1.4.3/ukis_pysat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/ukis_pysat/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/ukis_pysat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/ukis_pysat/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/ukis_pysat/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22369 2023-05-04 08:19:24.000000 ukis-pysat-1.5.0/ukis_pysat/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:39.905615 ukis-pysat-1.5.0/ukis_pysat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 08:19:39.000000 ukis-pysat-1.5.0/ukis_pysat.egg-info/top_level.txt
```

### Comparing `ukis-pysat-1.4.3/LICENSE.txt` & `ukis-pysat-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ukis-pysat-1.4.3/PKG-INFO` & `ukis-pysat-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ukis-pysat
-Version: 1.4.3
+Version: 1.5.0
 Summary: generic classes and functions to query, access and process multi-spectral and SAR satellite images
 Home-page: https://github.com/dlr-eoc/ukis-pysat
 Author: German Aerospace Center (DLR)
 Author-email: ukis-helpdesk@dlr.de
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: data
 Provides-Extra: raster
 Provides-Extra: complete
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 [![UKIS](https://raw.githubusercontent.com/dlr-eoc/ukis-pysat/master/docs/ukis-logo.png)](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) UKIS-pysat
 ==============
@@ -28,18 +27,15 @@
 [![PyPI version](https://img.shields.io/pypi/v/ukis-pysat)](https://pypi.python.org/pypi/ukis-pysat/)
 [![Documentation Status](https://readthedocs.org/projects/ukis-pysat/badge/?version=latest)](https://ukis-pysat.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE.txt)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/259635994.svg)](https://zenodo.org/badge/latestdoi/259635994)
 
 
-The UKIS-pysat package provides generic classes and functions to query, access and process multi-spectral and SAR satellite images.
-
-### data
-Download satellites data from different sources (currently Earth Explorer, SciHub, STAC), deal with and structure metadata.
+The UKIS-pysat package provides generic classes and functions to access and process multi-spectral and SAR satellite images.
 
 
 ### file
 Work with you local satellite data files and read information out of file names and metadata files. Currently, focusing on Sentinel-1.
 
 
 ### raster
@@ -50,59 +46,30 @@
 
 ## Example
 Here's an example about some basic features, it might also help to read through the [tests](https://github.com/dlr-eoc/ukis-pysat/blob/master/tests).
 ###Sentinel Dataset
 
 ```python
 # import all the required libraries
-from ukis_pysat.data import Source
 from ukis_pysat.file import get_sentinel_scene_from_dir
-from ukis_pysat.members import Datahub, Platform
 from ukis_pysat.raster import Image
 
-# connect to Copernicus Open Access Hub  and query metadata
-src = Source(Datahub.Scihub)
-meta = src.query_metadata(
-    platform=Platform.Sentinel2,
-    date=("20200101", "NOW"),
-    aoi=(11.90, 51.46, 11.94, 51.50),
-    cloud_cover=(0, 50),
-)
-for item in meta:  # item is now a PySTAC item
-    print(item.id)
-    uuid = item.properties["srcuuid"]
-
-    # download geocoded quicklook and image
-    src.download_quicklook(product_uuid=uuid, target_dir="/users/username/tmp")
-    src.download_image(product_uuid=uuid, target_dir="/users/username/tmp")
-    
-    break
 
 # get sentinel scene from directory
 with get_sentinel_scene_from_dir("/users/username/tmp") as (full_path, ident):
     with Image(full_path.join("pre_nrcs.tif")) as img:
         # scale the image array, having one band
         img.arr = img.arr * 0.3
 ```
 For working with the Landsat we need an item id for downloading the product
 Check [Pystac](https://pystac.readthedocs.io/en/1.0/) documentation for more functionality on [STAC](https://stacspec.org/).
 
-### Environment variables to configure Datahub credentials
-To use ``ukis_pysat.data`` and to download from the respective Datahub you need to set the credentials as environment variables.
-
-For EarthExplorer that's: \
-``EARTHEXPLORER_USER=your_username`` \
-``EARTHEXPLORER_PW=your_password``
-
-For SciHub that's: \
-``SCIHUB_USER=your_username`` \
-``SCIHUB_PW=your_password``
 
 ## Installation
-The easiest way to install `pysat` is through pip. Be aware, that Rasterio requires GDAL >= 1.11, < 3.1.
+The easiest way to install `ukis-pysat` is through pip. Be aware, that Rasterio requires GDAL >= 1.11, < 3.1.
 
 Most users will want to do this:
 ```shell
 pip install ukis-pysat[complete]  # install everything
 ```
 
 There's also some lighter versions with less dependencies:
```

### Comparing `ukis-pysat-1.4.3/README.md` & `ukis-pysat-1.5.0/ukis_pysat.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,41 @@
+Metadata-Version: 2.1
+Name: ukis-pysat
+Version: 1.5.0
+Summary: generic classes and functions to query, access and process multi-spectral and SAR satellite images
+Home-page: https://github.com/dlr-eoc/ukis-pysat
+Author: German Aerospace Center (DLR)
+Author-email: ukis-helpdesk@dlr.de
+License: Apache 2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: raster
+Provides-Extra: complete
+Provides-Extra: dev
+License-File: LICENSE.txt
+
 [![UKIS](https://raw.githubusercontent.com/dlr-eoc/ukis-pysat/master/docs/ukis-logo.png)](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) UKIS-pysat
 ==============
 
 ![ukis-pysat](https://github.com/dlr-eoc/ukis-pysat/workflows/ukis-pysat/badge.svg)
 [![codecov](https://codecov.io/gh/dlr-eoc/ukis-pysat/branch/master/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-pysat)
 ![Upload Python Package](https://github.com/dlr-eoc/ukis-pysat/workflows/Upload%20Python%20Package/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ukis-pysat)](https://pypi.python.org/pypi/ukis-pysat/)
 [![Documentation Status](https://readthedocs.org/projects/ukis-pysat/badge/?version=latest)](https://ukis-pysat.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE.txt)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/259635994.svg)](https://zenodo.org/badge/latestdoi/259635994)
 
 
-The UKIS-pysat package provides generic classes and functions to query, access and process multi-spectral and SAR satellite images.
-
-### data
-Download satellites data from different sources (currently Earth Explorer, SciHub, STAC), deal with and structure metadata.
+The UKIS-pysat package provides generic classes and functions to access and process multi-spectral and SAR satellite images.
 
 
 ### file
 Work with you local satellite data files and read information out of file names and metadata files. Currently, focusing on Sentinel-1.
 
 
 ### raster
@@ -29,59 +46,30 @@
 
 ## Example
 Here's an example about some basic features, it might also help to read through the [tests](https://github.com/dlr-eoc/ukis-pysat/blob/master/tests).
 ###Sentinel Dataset
 
 ```python
 # import all the required libraries
-from ukis_pysat.data import Source
 from ukis_pysat.file import get_sentinel_scene_from_dir
-from ukis_pysat.members import Datahub, Platform
 from ukis_pysat.raster import Image
 
-# connect to Copernicus Open Access Hub  and query metadata
-src = Source(Datahub.Scihub)
-meta = src.query_metadata(
-    platform=Platform.Sentinel2,
-    date=("20200101", "NOW"),
-    aoi=(11.90, 51.46, 11.94, 51.50),
-    cloud_cover=(0, 50),
-)
-for item in meta:  # item is now a PySTAC item
-    print(item.id)
-    uuid = item.properties["srcuuid"]
-
-    # download geocoded quicklook and image
-    src.download_quicklook(product_uuid=uuid, target_dir="/users/username/tmp")
-    src.download_image(product_uuid=uuid, target_dir="/users/username/tmp")
-    
-    break
 
 # get sentinel scene from directory
 with get_sentinel_scene_from_dir("/users/username/tmp") as (full_path, ident):
     with Image(full_path.join("pre_nrcs.tif")) as img:
         # scale the image array, having one band
         img.arr = img.arr * 0.3
 ```
 For working with the Landsat we need an item id for downloading the product
 Check [Pystac](https://pystac.readthedocs.io/en/1.0/) documentation for more functionality on [STAC](https://stacspec.org/).
 
-### Environment variables to configure Datahub credentials
-To use ``ukis_pysat.data`` and to download from the respective Datahub you need to set the credentials as environment variables.
-
-For EarthExplorer that's: \
-``EARTHEXPLORER_USER=your_username`` \
-``EARTHEXPLORER_PW=your_password``
-
-For SciHub that's: \
-``SCIHUB_USER=your_username`` \
-``SCIHUB_PW=your_password``
 
 ## Installation
-The easiest way to install `pysat` is through pip. Be aware, that Rasterio requires GDAL >= 1.11, < 3.1.
+The easiest way to install `ukis-pysat` is through pip. Be aware, that Rasterio requires GDAL >= 1.11, < 3.1.
 
 Most users will want to do this:
 ```shell
 pip install ukis-pysat[complete]  # install everything
 ```
 
 There's also some lighter versions with less dependencies:
```

### Comparing `ukis-pysat-1.4.3/setup.py` & `ukis-pysat-1.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,24 +21,14 @@
             return line.split(delim)[1]
 
         raise RuntimeError("Unable to find version string.")
 
 
 # please also update requirements.txt for testing. Make sure package versions are the same in each subset.
 extras_require = {
-    "data": [
-        "numpy",
-        "pillow",
-        "pystac>=1.0.0",
-        "python-dateutil",
-        "requests",
-        "sentinelsat>=1.0.1",
-        "shapely",
-        "pydantic",
-    ],
     "raster": [
         "numpy",
         "rasterio>=1.1.8",
         "rio_toa>=0.3.0",
         "shapely",
         "xmltodict",
     ],
@@ -46,18 +36,16 @@
 extras_require["complete"] = list(set([v for req in extras_require.values() for v in req]))
 
 extras_require["dev"] = sorted(
     extras_require["complete"]
     + [
         "dask[array]",
         "fiona",
-        "landsatxplore>=0.13.0",
         "pandas",
         "pyproj>=3.0.0",
-        "requests_mock",
         "utm>=0.7.0",
         "sphinx>=1.3",
         "sphinx_rtd_theme",
     ]
 )
 
 setup(
```

### Comparing `ukis-pysat-1.4.3/ukis_pysat/file.py` & `ukis-pysat-1.5.0/ukis_pysat/file.py`

 * *Files identical despite different names*

### Comparing `ukis-pysat-1.4.3/ukis_pysat/raster.py` & `ukis-pysat-1.5.0/ukis_pysat/raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         "Please pip install as follows:\n\n"
         "  python -m pip install ukis-pysat[raster] --upgrade"
     )
     raise ImportError(str(e) + "\n\n" + msg)
 
 
 class Image:
-
     da_arr = None
 
     def __init__(self, data, dimorder="first", crs=None, transform=None, nodata=None):
         """
         :param data: rasterio.io.DatasetReader or path to raster or np.ndarray of shape (bands, rows, columns)
         :param dimorder: Order of channels or bands 'first' or 'last' (default: 'first')
         :param crs: Coordinate reference system used when creating form array. If 'data' is np.ndarray this is required (default: None)
```

### Comparing `ukis-pysat-1.4.3/ukis_pysat.egg-info/PKG-INFO` & `ukis-pysat-1.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,21 @@
-Metadata-Version: 2.1
-Name: ukis-pysat
-Version: 1.4.3
-Summary: generic classes and functions to query, access and process multi-spectral and SAR satellite images
-Home-page: https://github.com/dlr-eoc/ukis-pysat
-Author: German Aerospace Center (DLR)
-Author-email: ukis-helpdesk@dlr.de
-License: Apache 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: data
-Provides-Extra: raster
-Provides-Extra: complete
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 [![UKIS](https://raw.githubusercontent.com/dlr-eoc/ukis-pysat/master/docs/ukis-logo.png)](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) UKIS-pysat
 ==============
 
 ![ukis-pysat](https://github.com/dlr-eoc/ukis-pysat/workflows/ukis-pysat/badge.svg)
 [![codecov](https://codecov.io/gh/dlr-eoc/ukis-pysat/branch/master/graph/badge.svg)](https://codecov.io/gh/dlr-eoc/ukis-pysat)
 ![Upload Python Package](https://github.com/dlr-eoc/ukis-pysat/workflows/Upload%20Python%20Package/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/ukis-pysat)](https://pypi.python.org/pypi/ukis-pysat/)
 [![Documentation Status](https://readthedocs.org/projects/ukis-pysat/badge/?version=latest)](https://ukis-pysat.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE.txt)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/259635994.svg)](https://zenodo.org/badge/latestdoi/259635994)
 
 
-The UKIS-pysat package provides generic classes and functions to query, access and process multi-spectral and SAR satellite images.
-
-### data
-Download satellites data from different sources (currently Earth Explorer, SciHub, STAC), deal with and structure metadata.
+The UKIS-pysat package provides generic classes and functions to access and process multi-spectral and SAR satellite images.
 
 
 ### file
 Work with you local satellite data files and read information out of file names and metadata files. Currently, focusing on Sentinel-1.
 
 
 ### raster
@@ -50,59 +26,30 @@
 
 ## Example
 Here's an example about some basic features, it might also help to read through the [tests](https://github.com/dlr-eoc/ukis-pysat/blob/master/tests).
 ###Sentinel Dataset
 
 ```python
 # import all the required libraries
-from ukis_pysat.data import Source
 from ukis_pysat.file import get_sentinel_scene_from_dir
-from ukis_pysat.members import Datahub, Platform
 from ukis_pysat.raster import Image
 
-# connect to Copernicus Open Access Hub  and query metadata
-src = Source(Datahub.Scihub)
-meta = src.query_metadata(
-    platform=Platform.Sentinel2,
-    date=("20200101", "NOW"),
-    aoi=(11.90, 51.46, 11.94, 51.50),
-    cloud_cover=(0, 50),
-)
-for item in meta:  # item is now a PySTAC item
-    print(item.id)
-    uuid = item.properties["srcuuid"]
-
-    # download geocoded quicklook and image
-    src.download_quicklook(product_uuid=uuid, target_dir="/users/username/tmp")
-    src.download_image(product_uuid=uuid, target_dir="/users/username/tmp")
-    
-    break
 
 # get sentinel scene from directory
 with get_sentinel_scene_from_dir("/users/username/tmp") as (full_path, ident):
     with Image(full_path.join("pre_nrcs.tif")) as img:
         # scale the image array, having one band
         img.arr = img.arr * 0.3
 ```
 For working with the Landsat we need an item id for downloading the product
 Check [Pystac](https://pystac.readthedocs.io/en/1.0/) documentation for more functionality on [STAC](https://stacspec.org/).
 
-### Environment variables to configure Datahub credentials
-To use ``ukis_pysat.data`` and to download from the respective Datahub you need to set the credentials as environment variables.
-
-For EarthExplorer that's: \
-``EARTHEXPLORER_USER=your_username`` \
-``EARTHEXPLORER_PW=your_password``
-
-For SciHub that's: \
-``SCIHUB_USER=your_username`` \
-``SCIHUB_PW=your_password``
 
 ## Installation
-The easiest way to install `pysat` is through pip. Be aware, that Rasterio requires GDAL >= 1.11, < 3.1.
+The easiest way to install `ukis-pysat` is through pip. Be aware, that Rasterio requires GDAL >= 1.11, < 3.1.
 
 Most users will want to do this:
 ```shell
 pip install ukis-pysat[complete]  # install everything
 ```
 
 There's also some lighter versions with less dependencies:
```

