# Comparing `tmp/cygnsslib-1.3.1.tar.gz` & `tmp/cygnsslib-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cygnsslib-1.3.1.tar", last modified: Wed May  3 03:01:10 2023, max compression
+gzip compressed data, was "cygnsslib-1.3.2.tar", last modified: Thu May  4 00:07:45 2023, max compression
```

## Comparing `cygnsslib-1.3.1.tar` & `cygnsslib-1.3.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    15896 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13006 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/src/cygnsslib/
--rw-rw-rw-   0 root         (0) root         (0)    14486 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/CygDdmId.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    63464 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/cyg.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/src/cygnsslib/cygnss_download/
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/cygnss_download/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/src/cygnsslib/data_downloader/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/data_downloader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/data_downloader/cyg_ant_ptrn.py
--rw-rw-rw-   0 root         (0) root         (0)     5663 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/data_downloader/download_cyg_rawif.py
--rw-rw-rw-   0 root         (0) root         (0)    19211 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/data_downloader/download_cygnss.py
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/data_downloader/download_cygnss_sftp.py
--rw-rw-rw-   0 root         (0) root         (0)    13187 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/data_downloader/download_srtm.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/istarmap.py
--rw-rw-rw-   0 root         (0) root         (0)     4905 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/plotting.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/src/cygnsslib/srtm_download/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/srtm_download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9205 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/cygnsslib/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/src/cygnsslib.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    15896 2023-05-03 03:01:10.000000 cygnsslib-1.3.1/src/cygnsslib.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-03 03:01:10.000000 cygnsslib-1.3.1/src/cygnsslib.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-03 03:01:10.000000 cygnsslib-1.3.1/src/cygnsslib.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-03 03:01:10.000000 cygnsslib-1.3.1/src/cygnsslib.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-03 03:01:10.000000 cygnsslib-1.3.1/src/cygnsslib.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 03:01:10.964840 cygnsslib-1.3.1/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/tests/list_loc2kml.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/tests/test_download_cyg_data.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/tests/test_download_srtm.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/tests/test_find_land_prod_from_cvs.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/tests/test_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/tests/test_search_within_circle.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2023-05-03 03:00:53.000000 cygnsslib-1.3.1/src/tests/test_write_sp_within_radius.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)    15905 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13015 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib/
+-rw-rw-rw-   0 root         (0) root         (0)    14486 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/CygDdmId.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    63464 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/cyg.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib/cygnss_download/
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/cygnss_download/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib/data_downloader/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/cyg_ant_ptrn.py
+-rw-rw-rw-   0 root         (0) root         (0)     5663 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cyg_rawif.py
+-rw-rw-rw-   0 root         (0) root         (0)    19700 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cygnss.py
+-rw-rw-rw-   0 root         (0) root         (0)     6530 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cygnss_sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)    13187 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_srtm.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/istarmap.py
+-rw-rw-rw-   0 root         (0) root         (0)     4905 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/plotting.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib/srtm_download/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/srtm_download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9205 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/cygnsslib/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/cygnsslib.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    15905 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-04 00:07:45.000000 cygnsslib-1.3.2/src/cygnsslib.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 00:07:45.291879 cygnsslib-1.3.2/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/list_loc2kml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_download_cyg_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_download_srtm.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_find_land_prod_from_cvs.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_search_within_circle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2023-05-04 00:07:27.000000 cygnsslib-1.3.2/src/tests/test_write_sp_within_radius.py
```

### Comparing `cygnsslib-1.3.1/PKG-INFO` & `cygnsslib-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cygnsslib
-Version: 1.3.1
+Version: 1.3.2
 Summary: Toolset for working with CYGNSS data and downloading CYGNSS data from PODAAC
 Home-page: https://bitbucket.org/usc_mixil/cygnsslib
 Author: Amer Melebari and James D. Campbell
 Author-email: amelebar@usc.edu
 License: UNKNOWN
 Description: # CYGNSS Library
         
@@ -30,15 +30,15 @@
         You can then remove the local copy if you wish. Alternatively, if you wish to be able to make changes to your local copy without having to reinstall the package for the changes to take effect (e.g., for development purposes), you can use the following instead:
         ```console
         pip uninstall cygnsslib
         ```
         ### Required packages
         Here the required Python packages:
         ```console
-        gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pysftp requests tqdm
+        gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pysftp requests tqdm paramiko
         ```
         Note: `gdal` can be installed using conda   
         ```console
         conda install -c conda-forge gdal  
         ```
         or using [this method](https://mothergeo-py.readthedocs.io/en/latest/development/how-to/gdal-ubuntu-pkg.html) in Ubuntu  
         Also, you need the modified data-subscriber package from [https://github.com/MiXIL/data-subscriber](https://github.com/MiXIL/data-subscriber)
```

### Comparing `cygnsslib-1.3.1/README.md` & `cygnsslib-1.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 You can then remove the local copy if you wish. Alternatively, if you wish to be able to make changes to your local copy without having to reinstall the package for the changes to take effect (e.g., for development purposes), you can use the following instead:
 ```console
 pip uninstall cygnsslib
 ```
 ### Required packages
 Here the required Python packages:
 ```console
-gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pysftp requests tqdm
+gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pysftp requests tqdm paramiko
 ```
 Note: `gdal` can be installed using conda   
 ```console
 conda install -c conda-forge gdal  
 ```
 or using [this method](https://mothergeo-py.readthedocs.io/en/latest/development/how-to/gdal-ubuntu-pkg.html) in Ubuntu  
 Also, you need the modified data-subscriber package from [https://github.com/MiXIL/data-subscriber](https://github.com/MiXIL/data-subscriber)
```

### Comparing `cygnsslib-1.3.1/setup.py` & `cygnsslib-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as fh:
     req = fh.read()
 
 setup(
     name='cygnsslib',
-    version='1.3.1',
+    version='1.3.2',
     author='Amer Melebari and James D. Campbell',
     author_email='amelebar@usc.edu',
     description='Toolset for working with CYGNSS data and downloading CYGNSS data from PODAAC',
     long_description=long_description,
     install_requires=req.split(),
     long_description_content_type="text/markdown",
     url='https://bitbucket.org/usc_mixil/cygnsslib',
```

### Comparing `cygnsslib-1.3.1/src/cygnsslib/CygDdmId.py` & `cygnsslib-1.3.2/src/cygnsslib/CygDdmId.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/cygnsslib/__init__.py` & `cygnsslib-1.3.2/src/cygnsslib/__init__.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/cygnsslib/cyg.py` & `cygnsslib-1.3.2/src/cygnsslib/cyg.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/cygnsslib/data_downloader/cyg_ant_ptrn.py` & `cygnsslib-1.3.2/src/cygnsslib/data_downloader/cyg_ant_ptrn.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/cygnsslib/data_downloader/download_cyg_rawif.py` & `cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cyg_rawif.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/cygnsslib/data_downloader/download_cygnss.py` & `cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cygnss.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
  EMAIL    amelebar@usc.edu
  CREATED  2020‑07‑19
  Updated  2023-05-02
 
   Copyright 2023 University of Southern California
 """
 import logging
+from inspect import signature
 from typing import Optional, Union
 from cygnsslib.data_downloader.download_srtm import EarthdataSession
 import subscriber.podaac_access as pa
 from time import sleep
 from tqdm.auto import tqdm
 import datetime as dt
 import fnmatch
@@ -244,18 +245,19 @@
             output_path = prepare_time_output(file_start_times, cygnss_l1_path, f)
 
             # decide if we should actually download this file (e.g. we may already have the latest version)
             if os.path.exists(output_path) and not force_download and (not checksum_exist_file or pa.checksum_does_match(output_path, checksums)):
                 logging.info(str(dt.datetime.now()) + " SKIPPED: " + f)
                 skip_cnt += 1
                 continue
-
-            checksum_val = checksums.get(os.path.basename(output_path))
-            pa.download_file(f, output_path, checksum_val)
-
+            if len(list(signature(pa.download_file).parameters)) > 3:  # allow for the use of non MiXIL version
+                checksum_val = checksums.get(os.path.basename(output_path))
+                pa.download_file(f, output_path, checksum_val)
+            else:
+                pa.download_file(f, output_path)
             logging.info(str(dt.datetime.now()) + " SUCCESS: " + f)
             success_cnt += 1
 
         except Exception:
             logging.warning(str(dt.datetime.now()) + " FAILURE: " + f, exc_info=True)
             failure_cnt += 1
         else:
@@ -407,15 +409,19 @@
 
             # decide if we should actually download this file (e.g. we may already have the latest version)
             if os.path.exists(output_path) and not force_download and (not checksum_exist_file or pa.checksum_does_match(output_path, checksums)):
                 logging.info(str(dt.datetime.now()) + " SKIPPED: " + f)
                 skip_cnt += 1
                 continue
 
-            pa.download_file(f, output_path)
+            if len(list(signature(pa.download_file).parameters)) > 3:  # allow for the use of non MiXIL version
+                checksum_val = checksums.get(os.path.basename(output_path))
+                pa.download_file(f, output_path, checksum_val)
+            else:
+                pa.download_file(f, output_path)
 
             logging.info(str(dt.datetime.now()) + " SUCCESS: " + f)
             success_cnt += 1
 
         except Exception:
             logging.warning(str(dt.datetime.now()) + " FAILURE: " + f, exc_info=True)
             failure_cnt += 1
@@ -467,12 +473,13 @@
     else:
         warnings.warn(f"You are trying to download version {cyg_data_ver:s}, but the path doesn't contain the version name", RuntimeWarning)
         out = False
     return out
 
 
 if __name__ == "__main__":
+
     st_date = dt.date(year=2020, month=7, day=1)
     end_date = dt.date(year=2020, month=12, day=31)
     cyg_data_ver = 'v3.1'
     download_cyg_files(2019, [5, 30, 31, 40])
     download_cyg_files_between_date(st_date, end_date, cyg_data_ver=cyg_data_ver, checksum_exist_file=False)
```

### Comparing `cygnsslib-1.3.1/src/cygnsslib/data_downloader/download_cygnss_sftp.py` & `cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_cygnss_sftp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os.path
 import shutil
 from getpass import getpass
 from typing import Optional, Union
 import numpy as np
 import paramiko
 from cygnsslib.data_downloader.download_cygnss import checksum
-from cygnsslib.data_downloader.pass_core import MixilKeys
 import time
 import pysftp
 import tqdm
 MAX_CONNECTIONS_TRIES = 4
 
 
 def find_file_name_in_dir(dir_data: list, data_year: int, data_day: int, sc_num: int, ver_tag: str = '') -> Optional[str]:
@@ -69,15 +68,18 @@
     :param out_main_folder: path of the main folder, this should point to the folder of the version i.e. data/cygnss_data/v3.1a
     :param data_path_sftp: path of the data in the SFTP server, default is /data/cygnss/products/l1. Note there is no backslash at the end
     :param save_username_pass: save your username and pass?
     :param reset_pass: reset the saved data?
     :return: file(s) name or None if no files found
     """
 
-    sftp_host, sftp_username, sftp_pass = get_podaac_cred(pass_folder=None, save_data=save_username_pass, reset_data=reset_pass)
+    # sftp_host, sftp_username, sftp_pass = get_podaac_cred(pass_folder=None, save_data=save_username_pass, reset_data=reset_pass)
+    sftp_host = input('SFTP HOST')
+    sftp_username = input('SFTP USER NAME')
+    sftp_pass = getpass('SFTP PASS')
     saved_files_list = list()
     if data_path_sftp is None:
         data_path_sftp = '/data/cygnss/products/l1'
     for _ in range(MAX_CONNECTIONS_TRIES):
         try:
             with pysftp.Connection(sftp_host, username=sftp_username, password=sftp_pass) as sftp:
                 debug(f"{time.strftime('%d-%m-%Y %H:%M')} - Connected to SFTP")
@@ -140,35 +142,7 @@
 def debug(msg: str):
     print(msg)
 
 
 def bytes2mb(size_byte): return np.around(float(size_byte) / 1048576, decimals=2)
 
 
-def get_podaac_cred(pass_folder=None, save_data=True, reset_data=False) -> tuple[str, str, str]:
-    """
-    import podaac username and pass from the system, if not found it ask you to enter them
-
-    :return:
-    """
-    if reset_data:
-        mixil_keys = MixilKeys(pass_folder=pass_folder)
-        mixil_keys.remove('cygnss_sftp_host')
-        mixil_keys.remove('cygnss_sftp_username')
-        mixil_keys.remove('cygnss_sftp_pass')
-        del mixil_keys
-
-    if save_data:
-        mixil_keys = MixilKeys(pass_folder=pass_folder)
-        mixil_keys.require('cygnss_sftp_host', msg='CYGNSS Host IP/URL: ', is_password=False)
-        mixil_keys.require('cygnss_sftp_username', msg='username: ', is_password=False)
-        mixil_keys.require('cygnss_sftp_pass', msg='password: ', is_password=True)
-        sftp_host = mixil_keys.retrieve('cygnss_sftp_host')
-        sftp_username = mixil_keys.retrieve('cygnss_sftp_username')
-        sftp_pass = mixil_keys.retrieve('cygnss_sftp_pass')
-    else:
-        sftp_host = input('CYGNSS Host IP/URL: ')
-        sftp_username = input('username: ')
-        sftp_pass = getpass('password: ')
-
-    return sftp_host, sftp_username, sftp_pass
-
```

### Comparing `cygnsslib-1.3.1/src/cygnsslib/data_downloader/download_srtm.py` & `cygnsslib-1.3.2/src/cygnsslib/data_downloader/download_srtm.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/cygnsslib/istarmap.py` & `cygnsslib-1.3.2/src/cygnsslib/istarmap.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/cygnsslib/plotting.py` & `cygnsslib-1.3.2/src/cygnsslib/plotting.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/cygnsslib/util.py` & `cygnsslib-1.3.2/src/cygnsslib/util.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/cygnsslib.egg-info/PKG-INFO` & `cygnsslib-1.3.2/src/cygnsslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cygnsslib
-Version: 1.3.1
+Version: 1.3.2
 Summary: Toolset for working with CYGNSS data and downloading CYGNSS data from PODAAC
 Home-page: https://bitbucket.org/usc_mixil/cygnsslib
 Author: Amer Melebari and James D. Campbell
 Author-email: amelebar@usc.edu
 License: UNKNOWN
 Description: # CYGNSS Library
         
@@ -30,15 +30,15 @@
         You can then remove the local copy if you wish. Alternatively, if you wish to be able to make changes to your local copy without having to reinstall the package for the changes to take effect (e.g., for development purposes), you can use the following instead:
         ```console
         pip uninstall cygnsslib
         ```
         ### Required packages
         Here the required Python packages:
         ```console
-        gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pysftp requests tqdm
+        gdal geographiclib lxml matplotlib netcdf4 numpy openpyxl pandas pysftp requests tqdm paramiko
         ```
         Note: `gdal` can be installed using conda   
         ```console
         conda install -c conda-forge gdal  
         ```
         or using [this method](https://mothergeo-py.readthedocs.io/en/latest/development/how-to/gdal-ubuntu-pkg.html) in Ubuntu  
         Also, you need the modified data-subscriber package from [https://github.com/MiXIL/data-subscriber](https://github.com/MiXIL/data-subscriber)
```

### Comparing `cygnsslib-1.3.1/src/cygnsslib.egg-info/SOURCES.txt` & `cygnsslib-1.3.2/src/cygnsslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/tests/list_loc2kml.py` & `cygnsslib-1.3.2/src/tests/list_loc2kml.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/tests/test_download_cyg_data.py` & `cygnsslib-1.3.2/src/tests/test_download_cyg_data.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/tests/test_functions.py` & `cygnsslib-1.3.2/src/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/tests/test_search_within_circle.py` & `cygnsslib-1.3.2/src/tests/test_search_within_circle.py`

 * *Files identical despite different names*

### Comparing `cygnsslib-1.3.1/src/tests/test_write_sp_within_radius.py` & `cygnsslib-1.3.2/src/tests/test_write_sp_within_radius.py`

 * *Files identical despite different names*

