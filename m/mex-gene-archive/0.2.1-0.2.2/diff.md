# Comparing `tmp/mex_gene_archive-0.2.1.tar.gz` & `tmp/mex_gene_archive-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mex_gene_archive-0.2.1.tar", last modified: Wed Jan 19 19:21:06 2022, max compression
+gzip compressed data, was "mex_gene_archive-0.2.2.tar", last modified: Thu May  4 20:46:26 2023, max compression
```

## Comparing `mex_gene_archive-0.2.1.tar` & `mex_gene_archive-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-01-19 19:21:06.014898 mex_gene_archive-0.2.1/
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-01-19 19:21:06.006898 mex_gene_archive-0.2.1/.github/
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-01-19 19:21:06.010898 mex_gene_archive-0.2.1/.github/workflows/
--rw-r--r--   0 diane     (1000) diane     (1000)      654 2021-10-26 21:45:01.000000 mex_gene_archive-0.2.1/.github/workflows/ci-test.yml
--rw-r--r--   0 diane     (1000) diane     (1000)      108 2021-10-26 23:05:13.000000 mex_gene_archive-0.2.1/.gitignore
--rw-r--r--   0 diane     (1000) diane     (1000)     1007 2022-01-19 19:18:58.000000 mex_gene_archive-0.2.1/Changelog.rst
--rw-r--r--   0 diane     (1000) diane     (1000)     1547 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.1/LICENSE.txt
--rw-r--r--   0 diane     (1000) diane     (1000)     2805 2022-01-19 19:21:06.014898 mex_gene_archive-0.2.1/PKG-INFO
--rw-r--r--   0 diane     (1000) diane     (1000)     2313 2021-10-26 21:55:37.000000 mex_gene_archive-0.2.1/README.rst
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-01-19 19:21:06.010898 mex_gene_archive-0.2.1/mex_gene_archive/
--rw-r--r--   0 diane     (1000) diane     (1000)        0 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.1/mex_gene_archive/__init__.py
--rw-r--r--   0 diane     (1000) diane     (1000)      142 2022-01-19 19:21:05.000000 mex_gene_archive-0.2.1/mex_gene_archive/_version.py
--rw-r--r--   0 diane     (1000) diane     (1000)     5312 2022-01-13 20:01:28.000000 mex_gene_archive-0.2.1/mex_gene_archive/filter.py
--rw-r--r--   0 diane     (1000) diane     (1000)     4127 2022-01-13 20:01:28.000000 mex_gene_archive-0.2.1/mex_gene_archive/manifest.py
--rw-r--r--   0 diane     (1000) diane     (1000)     4941 2022-01-13 22:29:25.000000 mex_gene_archive-0.2.1/mex_gene_archive/reader.py
--rw-r--r--   0 diane     (1000) diane     (1000)     7306 2022-01-13 20:03:30.000000 mex_gene_archive-0.2.1/mex_gene_archive/starsolo.py
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-01-19 19:21:06.010898 mex_gene_archive-0.2.1/mex_gene_archive.egg-info/
--rw-r--r--   0 diane     (1000) diane     (1000)     2805 2022-01-19 19:21:05.000000 mex_gene_archive-0.2.1/mex_gene_archive.egg-info/PKG-INFO
--rw-r--r--   0 diane     (1000) diane     (1000)      585 2022-01-19 19:21:06.000000 mex_gene_archive-0.2.1/mex_gene_archive.egg-info/SOURCES.txt
--rw-r--r--   0 diane     (1000) diane     (1000)        1 2022-01-19 19:21:05.000000 mex_gene_archive-0.2.1/mex_gene_archive.egg-info/dependency_links.txt
--rw-r--r--   0 diane     (1000) diane     (1000)       29 2022-01-19 19:21:05.000000 mex_gene_archive-0.2.1/mex_gene_archive.egg-info/requires.txt
--rw-r--r--   0 diane     (1000) diane     (1000)       23 2022-01-19 19:21:05.000000 mex_gene_archive-0.2.1/mex_gene_archive.egg-info/top_level.txt
--rw-r--r--   0 diane     (1000) diane     (1000)      367 2021-10-26 22:20:36.000000 mex_gene_archive-0.2.1/pyproject.toml
--rw-r--r--   0 diane     (1000) diane     (1000)      624 2022-01-19 19:21:06.014898 mex_gene_archive-0.2.1/setup.cfg
--rw-r--r--   0 diane     (1000) diane     (1000)       69 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.1/setup.py
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-01-19 19:21:06.014898 mex_gene_archive-0.2.1/tests/
--rw-r--r--   0 diane     (1000) diane     (1000)        0 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.1/tests/__init__.py
--rw-r--r--   0 diane     (1000) diane     (1000)    31823 2021-12-16 21:43:01.000000 mex_gene_archive-0.2.1/tests/stage_data.py
--rw-r--r--   0 diane     (1000) diane     (1000)     2431 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.1/tests/test_filter.py
--rw-r--r--   0 diane     (1000) diane     (1000)     3074 2022-01-13 20:01:28.000000 mex_gene_archive-0.2.1/tests/test_manifest.py
--rw-r--r--   0 diane     (1000) diane     (1000)    11393 2022-01-13 22:29:25.000000 mex_gene_archive-0.2.1/tests/test_starsolo.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.622010 mex_gene_archive-0.2.2/
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.606010 mex_gene_archive-0.2.2/.github/
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.614010 mex_gene_archive-0.2.2/.github/workflows/
+-rw-r--r--   0 diane     (1000) diane     (1000)      654 2021-10-26 21:45:01.000000 mex_gene_archive-0.2.2/.github/workflows/ci-test.yml
+-rw-r--r--   0 diane     (1000) diane     (1000)      129 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/.gitignore
+-rw-r--r--   0 diane     (1000) diane     (1000)     1255 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/Changelog.rst
+-rw-r--r--   0 diane     (1000) diane     (1000)     1547 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/LICENSE.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)     2809 2023-05-04 20:46:26.622010 mex_gene_archive-0.2.2/PKG-INFO
+-rw-r--r--   0 diane     (1000) diane     (1000)     2337 2023-04-28 17:46:50.000000 mex_gene_archive-0.2.2/README.rst
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.618010 mex_gene_archive-0.2.2/mex_gene_archive/
+-rw-r--r--   0 diane     (1000) diane     (1000)        0 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/mex_gene_archive/__init__.py
+-rw-r--r--   0 diane     (1000) diane     (1000)      160 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive/_version.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     5199 2023-04-29 06:07:52.000000 mex_gene_archive-0.2.2/mex_gene_archive/anndata.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     5312 2022-01-13 20:01:28.000000 mex_gene_archive-0.2.2/mex_gene_archive/filter.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     4291 2023-05-01 19:12:18.000000 mex_gene_archive-0.2.2/mex_gene_archive/manifest.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     5051 2023-04-29 00:36:47.000000 mex_gene_archive-0.2.2/mex_gene_archive/reader.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     7338 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/mex_gene_archive/starsolo.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.618010 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/
+-rw-r--r--   0 diane     (1000) diane     (1000)     2809 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/PKG-INFO
+-rw-r--r--   0 diane     (1000) diane     (1000)      635 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)        1 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)       29 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/requires.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)       23 2023-05-04 20:46:26.000000 mex_gene_archive-0.2.2/mex_gene_archive.egg-info/top_level.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)      396 2023-04-28 21:37:26.000000 mex_gene_archive-0.2.2/pyproject.toml
+-rw-r--r--   0 diane     (1000) diane     (1000)      624 2023-05-04 20:46:26.622010 mex_gene_archive-0.2.2/setup.cfg
+-rw-r--r--   0 diane     (1000) diane     (1000)       69 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/setup.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-04 20:46:26.622010 mex_gene_archive-0.2.2/tests/
+-rw-r--r--   0 diane     (1000) diane     (1000)        0 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/tests/__init__.py
+-rw-r--r--   0 diane     (1000) diane     (1000)    31823 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/tests/stage_data.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     3327 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/tests/test_anndata.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     2431 2021-10-26 17:27:08.000000 mex_gene_archive-0.2.2/tests/test_filter.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     3754 2023-05-01 19:15:57.000000 mex_gene_archive-0.2.2/tests/test_manifest.py
+-rw-r--r--   0 diane     (1000) diane     (1000)    12358 2023-05-04 18:43:03.000000 mex_gene_archive-0.2.2/tests/test_starsolo.py
```

### Comparing `mex_gene_archive-0.2.1/.github/workflows/ci-test.yml` & `mex_gene_archive-0.2.2/.github/workflows/ci-test.yml`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.1/Changelog.rst` & `mex_gene_archive-0.2.2/Changelog.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,24 @@
+
 Changelog
 =========
 
+Release 0.2.2
+-------------
+
+Add function to write an AnnData archive to a mex_gene_archive file.
+
+def write_anndata_as_mex_archive(
+    adata,
+    quantification="GeneFull",
+    multiread="Unique",
+    matrix="raw",
+    *,
+    destination=None)
+
 Release 0.2.1
 -------------
 
 The manifest.tsv file is now being written into the same logical
 directory as the matrix being archived, to make it easier to extract
 multiple matrices.
```

### Comparing `mex_gene_archive-0.2.1/LICENSE.txt` & `mex_gene_archive-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.1/PKG-INFO` & `mex_gene_archive-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: mex_gene_archive
-Version: 0.2.1
+Version: 0.2.2
 Summary: matrix market tar archive access utilities
 Home-page: https://github.com/detrout/mex_gene_archive
 Author: Diane Trout
 Author-email: diane@caltech.edu
 License: BSD-3
 Project-URL: Source, https://github.com/detrout/mex_gene_archive
 Project-URL: Tracker, https://github.com/detrout/mex_gene_archive/issues
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: test
 License-File: LICENSE.txt
 
 |ci-test|
 
 Introduction
@@ -42,22 +41,22 @@
 
 Probably the more useful function is the one that will read an archive
 into an anndata structure with the gene features going across the
 columns and the cell barcode observations going down across the rows.
 
 .. code-block:: python
 
-   from mex_gene_archive.reader import read_mex_as_anndata
+   from mex_gene_archive.reader import read_mex_archive_as_anndata
 
-   adata = read_mex_as_anndata("archive.tar.gz")
+   adata = read_mex_archive_as_anndata("archive.tar.gz")
 
    req = requests.get(
        "https://www.encodeproject.org/files/ENCFFexample/@@download/ENCFFexample.fastq.gz",
        stream=True)
-   adata = read_mex_as_anndata(fileobj=req.raw)
+   adata = read_mex_archive_as_anndata(fileobj=req.raw)
 
 
 The reader module can also convert archives to anndata directly from
 the command line
 
 .. code-block:: bash
 
@@ -83,9 +82,7 @@
       "description": "snRNA on human adrenal gland.",
       "library_accession": "ENCLB002DZK",
    }
    archive_star_solo("experiment", config)
 
 .. _`matrix market exchange`: https://math.nist.gov/MatrixMarket/
 .. |ci-test| image:: https://github.com/detrout/mex_gene_archive/actions/workflows/ci-test.yml/badge.svg
-
-
```

### Comparing `mex_gene_archive-0.2.1/README.rst` & `mex_gene_archive-0.2.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 
 Probably the more useful function is the one that will read an archive
 into an anndata structure with the gene features going across the
 columns and the cell barcode observations going down across the rows.
 
 .. code-block:: python
 
-   from mex_gene_archive.reader import read_mex_as_anndata
+   from mex_gene_archive.reader import read_mex_archive_as_anndata
 
-   adata = read_mex_as_anndata("archive.tar.gz")
+   adata = read_mex_archive_as_anndata("archive.tar.gz")
 
    req = requests.get(
        "https://www.encodeproject.org/files/ENCFFexample/@@download/ENCFFexample.fastq.gz",
        stream=True)
-   adata = read_mex_as_anndata(fileobj=req.raw)
+   adata = read_mex_archive_as_anndata(fileobj=req.raw)
 
 
 The reader module can also convert archives to anndata directly from
 the command line
 
 .. code-block:: bash
```

### Comparing `mex_gene_archive-0.2.1/mex_gene_archive/filter.py` & `mex_gene_archive-0.2.2/mex_gene_archive/filter.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.1/mex_gene_archive/manifest.py` & `mex_gene_archive-0.2.2/mex_gene_archive/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from pathlib import Path
 import hashlib
 
 #######
 # Functions for making manifest
 #
 logger = logging.getLogger(__name__)
-IO_BUFFER = 2 ** 10
+IO_BUFFER = 2**10
 
 
 class ConfigError(ValueError):
     """Indicate the config dictionary isn't correct"""
+
     pass
 
 
 def compute_md5sums(files):
     """Compute md5sums of a list of files
 
     Parameters
@@ -75,21 +76,25 @@
         description, and library_accession.
     md5s : list((filename, md5 hexdigest))
         List of filename and hexdigest tuples that will be added to the manifest
         dictionary.
     """
     metadata = {
         "type": "MexGeneArchive_v1",
-        "output_type": config['output_type'],
+        "output_type": config["output_type"],
         "software_version": config["software_version"],
         "arguments": config["arguments"],
     }
     for key in ["experiment_accession", "description", "library_accession"]:
         if key in config:
             metadata[key] = config[key]
+        else:
+            raise ConfigError(
+                "Expected attribute {} is missing from configuration".format(key)
+            )
 
     for filename, md5 in md5s:
         metadata[filename] = "md5sum:{}".format(md5)
 
     return metadata
 
 
@@ -109,20 +114,20 @@
     """
     not_user = ["type", "output_type", "software_version", "arguments"]
     user = ["experiment_accession", "description", "library_accession"]
     has_errors = False
 
     for key in not_user:
         if key in config:
-            logger.error("{} will be generated by the pipeline")
+            logger.error("{} will be generated by the pipeline".format(key))
             has_errors = True
 
     for key in user:
         if key not in config:
-            logger.error("{} needs to be provided in the config file")
+            logger.error("{} needs to be provided in the config file".format(key))
             has_errors = True
 
     if has_errors:
         raise ConfigError("Invalid attributes in config file")
 
 
 def write_manifest(outstream, config):
```

### Comparing `mex_gene_archive-0.2.1/mex_gene_archive/reader.py` & `mex_gene_archive-0.2.2/mex_gene_archive/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
-import csv
 from io import TextIOWrapper
 import logging
+import numpy
 from pathlib import Path
 import pandas
 from scipy.io import mmread
 import tarfile
 
 from .manifest import read_manifest
 
@@ -103,14 +103,15 @@
                     result["features"] = read_sj_features(text_stream)
                 else:
                     result["features"] = read_gene_features(text_stream)
             elif member_path.suffix == ".mtx":
                 result["matrix"] = mmread(archive.extractfile(member))
             else:
                 logger.warning("Unrecognized archive member {}".format(member.name))
+
     return result
 
 
 def read_mex_archive_as_anndata(filename=None, fileobj=None):
     """Reads a mex archive into an AnnData structure
 
     Parameters
@@ -125,15 +126,19 @@
 
     AnnData object
     """
     from anndata import AnnData
 
     result = read_mex_archive(filename=filename, fileobj=fileobj)
     result["metadata"] = remove_manifest_md5s(result["metadata"])
-    adata = AnnData(X=result["matrix"].T.tocsc(), uns=result["metadata"])
+    if isinstance(result["matrix"], numpy.ndarray):
+        X = result["matrix"].T
+    else:
+        X = result["matrix"].T.tocsc()
+    adata = AnnData(X=X, uns=result["metadata"])
     adata.obs_names = result["barcodes"]
 
     for column in result["features"]:
         if column == "gene_id":
             adata.var_names = result["features"][column].to_numpy()
         else:
             adata.var[column] = result["features"][column].to_numpy()
```

### Comparing `mex_gene_archive-0.2.1/mex_gene_archive/starsolo.py` & `mex_gene_archive-0.2.2/mex_gene_archive/starsolo.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     return solo_root / quantification / matrix
 
 
 def make_tar_archive_name(
         solo_root, quantification, multiread, matrix, destination):
     """Compute name of mex gene tar archives for different matrices
     """
+    solo_root = Path(solo_root)
     tar_name = "{}_{}_{}.tar.gz".format(quantification, multiread, matrix)
     if destination is not None:
         destination = Path(destination)
         if destination.is_dir():
             tar_name = destination / tar_name
         else:
             tar_name = destination
```

### Comparing `mex_gene_archive-0.2.1/mex_gene_archive.egg-info/PKG-INFO` & `mex_gene_archive-0.2.2/mex_gene_archive.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: mex-gene-archive
-Version: 0.2.1
+Version: 0.2.2
 Summary: matrix market tar archive access utilities
 Home-page: https://github.com/detrout/mex_gene_archive
 Author: Diane Trout
 Author-email: diane@caltech.edu
 License: BSD-3
 Project-URL: Source, https://github.com/detrout/mex_gene_archive
 Project-URL: Tracker, https://github.com/detrout/mex_gene_archive/issues
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: test
 License-File: LICENSE.txt
 
 |ci-test|
 
 Introduction
@@ -42,22 +41,22 @@
 
 Probably the more useful function is the one that will read an archive
 into an anndata structure with the gene features going across the
 columns and the cell barcode observations going down across the rows.
 
 .. code-block:: python
 
-   from mex_gene_archive.reader import read_mex_as_anndata
+   from mex_gene_archive.reader import read_mex_archive_as_anndata
 
-   adata = read_mex_as_anndata("archive.tar.gz")
+   adata = read_mex_archive_as_anndata("archive.tar.gz")
 
    req = requests.get(
        "https://www.encodeproject.org/files/ENCFFexample/@@download/ENCFFexample.fastq.gz",
        stream=True)
-   adata = read_mex_as_anndata(fileobj=req.raw)
+   adata = read_mex_archive_as_anndata(fileobj=req.raw)
 
 
 The reader module can also convert archives to anndata directly from
 the command line
 
 .. code-block:: bash
 
@@ -83,9 +82,7 @@
       "description": "snRNA on human adrenal gland.",
       "library_accession": "ENCLB002DZK",
    }
    archive_star_solo("experiment", config)
 
 .. _`matrix market exchange`: https://math.nist.gov/MatrixMarket/
 .. |ci-test| image:: https://github.com/detrout/mex_gene_archive/actions/workflows/ci-test.yml/badge.svg
-
-
```

### Comparing `mex_gene_archive-0.2.1/mex_gene_archive.egg-info/SOURCES.txt` & `mex_gene_archive-0.2.2/mex_gene_archive.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/ci-test.yml
 mex_gene_archive/__init__.py
 mex_gene_archive/_version.py
+mex_gene_archive/anndata.py
 mex_gene_archive/filter.py
 mex_gene_archive/manifest.py
 mex_gene_archive/reader.py
 mex_gene_archive/starsolo.py
 mex_gene_archive.egg-info/PKG-INFO
 mex_gene_archive.egg-info/SOURCES.txt
 mex_gene_archive.egg-info/dependency_links.txt
 mex_gene_archive.egg-info/requires.txt
 mex_gene_archive.egg-info/top_level.txt
 tests/__init__.py
 tests/stage_data.py
+tests/test_anndata.py
 tests/test_filter.py
 tests/test_manifest.py
 tests/test_starsolo.py
```

### Comparing `mex_gene_archive-0.2.1/setup.cfg` & `mex_gene_archive-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.1/tests/stage_data.py` & `mex_gene_archive-0.2.2/tests/stage_data.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.1/tests/test_filter.py` & `mex_gene_archive-0.2.2/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mex_gene_archive-0.2.1/tests/test_manifest.py` & `mex_gene_archive-0.2.2/tests/test_manifest.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,7 +79,25 @@
             "genome_dir": "genome_dir",
             "allow_list": "allow_list",
             "mem_mb": 65535,
             "disk_mb": 51200,
         }
         with self.assertLogs(manifest_logger) as log:
             self.assertRaises(ConfigError, validate_config_metadata, config)
+
+    def test_validate_config_metadata_missing_library_accession(self):
+        config = {
+            "read1": ["ENCFF150FBF", "ENCFF385IAW"],
+            "read2": ["ENCFF351VBS", "ENCFF503CCI"],
+            "include_introns": True,
+            "stranded": "Forward",
+            "experiment_accession": "ENCSR724KET",
+            "library_accession": "ENCLB002DZK",
+            "umi_version": 12,
+            "genome_dir": "genome_dir",
+            "allow_list": "allow_list",
+            "mem_mb": 65535,
+            "disk_mb": 51200,
+        }
+        with self.assertLogs(manifest_logger) as log:
+            self.assertRaises(ConfigError, validate_config_metadata, config)
+
```

### Comparing `mex_gene_archive-0.2.1/tests/test_starsolo.py` & `mex_gene_archive-0.2.2/tests/test_starsolo.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     read_sj_features,
     main as reader_main,
 )
 from mex_gene_archive.starsolo import (
     MULTIREAD_NAME,
     make_list_of_archive_files,
     make_output_type_term,
+    make_tar_archive_name,
     validate_star_solo_out_arguments,
     parse_star_log_out_stream,
     archive_star_solo,
 )
 from .stage_data import (
     generate_count_matrix,
     make_sample_data,
@@ -279,7 +280,29 @@
             raw_files[BARCODE_TSV_INDEX],
             raw_files[MTX_INDEX],
             filtered_files[BARCODE_TSV_INDEX],
         ):
             md5.update(line.encode("utf-8"))
 
         self.assertEqual(files_md5[0][1], md5.hexdigest())
+
+    def test_make_tar_archive_name(self):
+        dest = "/tmp"
+        tar_name = make_tar_archive_name(self.solo_dir, "Gene", "Unique", "raw", dest)
+        self.assertEqual(tar_name,  Path("/tmp/Gene_Unique_raw.tar.gz"))
+
+        filename = "/tmp/archive.tar.gz"
+        tar_name = make_tar_archive_name(
+            self.solo_dir, "Gene", "Unique", "raw", filename)
+        self.assertEqual(tar_name, Path(filename))
+
+        filename = Path("/tmp/archive.tar.gz")
+        tar_name = make_tar_archive_name(
+            self.solo_dir, "Gene", "Unique", "raw", filename)
+        self.assertEqual(tar_name, filename)
+
+        tar_name = make_tar_archive_name(self.solo_dir, "Gene", "Unique", "raw", None)
+        filename = self.solo_dir.parent / "Gene_Unique_raw.tar.gz"
+        self.assertEqual(tar_name,  filename)
+
+        self.assertRaises(
+            RuntimeError, make_tar_archive_name, __file__, "Gene", "Unique", "raw", None)
```

