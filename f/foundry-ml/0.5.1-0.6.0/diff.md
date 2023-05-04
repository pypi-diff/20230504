# Comparing `tmp/foundry_ml-0.5.1.tar.gz` & `tmp/foundry_ml-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundry_ml-0.5.1.tar", last modified: Thu Feb 16 19:17:27 2023, max compression
+gzip compressed data, was "foundry_ml-0.6.0.tar", last modified: Thu May  4 20:00:42 2023, max compression
```

## Comparing `foundry_ml-0.5.1.tar` & `foundry_ml-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:17:27.204131 foundry_ml-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-02-16 19:17:27.204131 foundry_ml-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:17:27.204131 foundry_ml-0.5.1/foundry/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/foundry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29745 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/foundry/foundry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/foundry/https_download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:17:27.204131 foundry_ml-0.5.1/foundry/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/foundry/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/foundry/loaders/tf_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/foundry/loaders/torch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/foundry/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/foundry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:17:27.204131 foundry_ml-0.5.1/foundry_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-02-16 19:17:27.000000 foundry_ml-0.5.1/foundry_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-16 19:17:27.000000 foundry_ml-0.5.1/foundry_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 19:17:27.000000 foundry_ml-0.5.1/foundry_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-16 19:17:27.000000 foundry_ml-0.5.1/foundry_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-16 19:17:27.000000 foundry_ml-0.5.1/foundry_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-16 19:17:27.204131 foundry_ml-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:17:27.204131 foundry_ml-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-02-16 19:17:13.000000 foundry_ml-0.5.1/tests/test_foundry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:00:42.053247 foundry_ml-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-04 20:00:42.053247 foundry_ml-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:00:42.053247 foundry_ml-0.6.0/foundry/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33351 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/foundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/https_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/https_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:00:42.053247 foundry_ml-0.6.0/foundry/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/loaders/tf_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/loaders/torch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/foundry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:00:42.053247 foundry_ml-0.6.0/foundry_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-04 20:00:41.000000 foundry_ml-0.6.0/foundry_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-04 20:00:42.000000 foundry_ml-0.6.0/foundry_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:00:41.000000 foundry_ml-0.6.0/foundry_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-04 20:00:41.000000 foundry_ml-0.6.0/foundry_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 20:00:41.000000 foundry_ml-0.6.0/foundry_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 20:00:42.053247 foundry_ml-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:00:42.053247 foundry_ml-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-04 20:00:27.000000 foundry_ml-0.6.0/tests/test_foundry.py
```

### Comparing `foundry_ml-0.5.1/LICENSE` & `foundry_ml-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.5.1/PKG-INFO` & `foundry_ml-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry_ml
-Version: 0.5.1
+Version: 0.6.0
 Summary: Package to support simplified application of machine learning models to datasets in materials science
 Home-page: https://github.com/MLMI2-CSSI/foundry
 Author: Aristana Scourtas, KJ Schmidt, Isaac Darling, Aadit Ambadkar, Braeden Cullen,
             Imogen Foster, Ribhav Bose, Zoa Katok, Ethan Truelove, Ian Foster, Ben Blaiszik
 Author-email: blaiszik@uchicago.edu
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,15 @@
   <img src="https://raw.githubusercontent.com/MLMI2-CSSI/foundry/main/assets/foundry-black.png" height="175">
 </picture>
 
 [![PyPI](https://img.shields.io/pypi/v/foundry_ml.svg)](https://pypi.python.org/pypi/foundry_ml)
 [![Tests](https://github.com/MLMI2-CSSI/foundry/actions/workflows/tests.yml/badge.svg)](https://github.com/MLMI2-CSSI/foundry/actions/workflows/tests.yml)
 [![Tests](https://github.com/MLMI2-CSSI/foundry/actions/workflows/python-publish.yml/badge.svg)](https://github.com/MLMI2-CSSI/foundry/actions/workflows/python-publish.yml)
 [![NSF-1931306](https://img.shields.io/badge/NSF-1931306-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1931306&HistoricalAwards=false)
+[<img src="https://img.shields.io/badge/view-documentation-blue">](https://ai-materials-and-chemistry.gitbook.io/foundry/)
 
 
 Foundry-ML simplifies the discovery and usage of ML-ready datasets in materials science and chemistry providing a simple API to access even complex datasets. 
 * Load ML-ready data with just a few lines of code
 * Work with datasets in local or cloud environments. 
 * Publish your own datasets with Foundry to promote community usage
 * (in progress) Run published ML models without hassle
```

### Comparing `foundry_ml-0.5.1/README.md` & `foundry_ml-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   <img src="https://raw.githubusercontent.com/MLMI2-CSSI/foundry/main/assets/foundry-black.png" height="175">
 </picture>
 
 [![PyPI](https://img.shields.io/pypi/v/foundry_ml.svg)](https://pypi.python.org/pypi/foundry_ml)
 [![Tests](https://github.com/MLMI2-CSSI/foundry/actions/workflows/tests.yml/badge.svg)](https://github.com/MLMI2-CSSI/foundry/actions/workflows/tests.yml)
 [![Tests](https://github.com/MLMI2-CSSI/foundry/actions/workflows/python-publish.yml/badge.svg)](https://github.com/MLMI2-CSSI/foundry/actions/workflows/python-publish.yml)
 [![NSF-1931306](https://img.shields.io/badge/NSF-1931306-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1931306&HistoricalAwards=false)
+[<img src="https://img.shields.io/badge/view-documentation-blue">](https://ai-materials-and-chemistry.gitbook.io/foundry/)
 
 
 Foundry-ML simplifies the discovery and usage of ML-ready datasets in materials science and chemistry providing a simple API to access even complex datasets. 
 * Load ML-ready data with just a few lines of code
 * Work with datasets in local or cloud environments. 
 * Publish your own datasets with Foundry to promote community usage
 * (in progress) Run published ML models without hassle
```

### Comparing `foundry_ml-0.5.1/foundry/foundry.py` & `foundry_ml-0.6.0/foundry/foundry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import h5py
 import json
 import mdf_toolbox
 from json2table import convert
 import numpy as np
 import pandas as pd
-from typing import Any
+from typing import Any, Dict, List
 import logging
 import warnings
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from tqdm.auto import tqdm
 
 from mdf_connect_client import MDFConnectClient
 from mdf_forge import Forge
 from dlhub_sdk import DLHubClient
-from tqdm.auto import tqdm
+from globus_sdk import AuthClient
 
+from .auth import PubAuths
 from .utils import is_pandas_pytable, is_doi
 from .utils import _read_csv, _read_json, _read_excel
 
 from foundry.models import (
     FoundryMetadata,
     FoundryConfig,
     FoundryDataset
 )
 from foundry.https_download import download_file, recursive_ls
+from foundry.https_upload import upload_to_endpoint
 
 logger = logging.getLogger(__name__)
 
 
 class Foundry(FoundryMetadata):
     """Foundry Client Base Class
     TODO:
@@ -36,15 +39,17 @@
 
     """
 
     dlhub_client: Any
     forge_client: Any
     connect_client: Any
     transfer_client: Any
+    auth_client: Any
     index = ""
+    auths: Any
 
     xtract_tokens: Any
 
     def __init__(
             self, no_browser=False, no_local_server=False, index="mdf", authorizers=None, **data
     ):
         """Initialize a Foundry client
@@ -59,30 +64,33 @@
 
         Returns
         -------
             an initialized and authenticated Foundry client
         """
         super().__init__(**data)
         self.index = index
+        self.auths = None
 
         if authorizers:
-            auths = authorizers
+            self.auths = authorizers
         else:
             services = [
-                "data_mdf",
-                "mdf_connect",
-                "search",
-                "petrel",
-                "transfer",
-                "dlhub",
-                "funcx",
-                "openid",
-                "https://auth.globus.org/scopes/facd7ccc-c5f4-42aa-916b-a0e270e2c2a9/all",
-            ]
-            auths = mdf_toolbox.login(
+                    "data_mdf",
+                    "mdf_connect",
+                    "search",
+                    "petrel",
+                    "transfer",
+                    "dlhub",
+                    "openid",
+                    "https://auth.globus.org/scopes/facd7ccc-c5f4-42aa-916b-a0e270e2c2a9/all",  # funcx
+                    "https://auth.globus.org/scopes/f10a69a9-338c-4e5b-baa1-0dc92359ab47/https",  # Eagle HTTPS
+                    "https://auth.globus.org/scopes/82f1b5c6-6e9b-11e5-ba47-22000b92c6ec/https",  # NCSA HTTPS
+                    "https://auth.globus.org/scopes/d31d4f5d-be37-4adc-a761-2f716b7af105/action_all",  # Globus Search Lambda
+                ]
+            self.auths = mdf_toolbox.login(
                 services=services,
                 app_name="Foundry",
                 make_clients=True,
                 no_browser=no_browser,
                 no_local_server=no_local_server,
             )
             # request Search as an authorizer and not a client
@@ -90,51 +98,56 @@
                 services=['search'],
                 app_name="Foundry",
                 make_clients=False,
                 no_browser=no_browser,
                 no_local_server=no_local_server,
             )
             # add special SearchAuthorizer object
-            auths['search_authorizer'] = search_auth['search']
+            self.auths['search_authorizer'] = search_auth['search']
 
         self.forge_client = Forge(
             index=index,
             services=None,
-            search_client=auths["search"],
-            transfer_client=auths["transfer"],
-            data_mdf_authorizer=auths["data_mdf"],
-            petrel_authorizer=auths["petrel"],
+            search_client=self.auths["search"],
+            transfer_client=self.auths["transfer"],
+            data_mdf_authorizer=self.auths["data_mdf"],
+            petrel_authorizer=self.auths["petrel"],
         )
 
-        self.transfer_client = auths['transfer']
+        self.transfer_client = self.auths['transfer']
+
+        self.auth_client = AuthClient(authorizer=self.auths['openid'])
 
         if index == "mdf":
             test = False
         else:
             test = True
         # TODO: when release-ready, remove test=True
 
         self.connect_client = MDFConnectClient(
-            authorizer=auths["mdf_connect"], test=test
+            authorizer=self.auths["mdf_connect"], test=test
         )
 
         self.dlhub_client = DLHubClient(
-            dlh_authorizer=auths["dlhub"],
-            search_authorizer=auths["search_authorizer"],
-            fx_authorizer=auths[
+            dlh_authorizer=self.auths["dlhub"],
+            search_authorizer=self.auths["search_authorizer"],
+            fx_authorizer=self.auths[
                 "https://auth.globus.org/scopes/facd7ccc-c5f4-42aa-916b-a0e270e2c2a9/all"
             ],
-            openid_authorizer=auths['openid'],
+            openid_authorizer=self.auths['openid'],
+            sl_authorizer=self.auths[
+                "https://auth.globus.org/scopes/d31d4f5d-be37-4adc-a761-2f716b7af105/action_all"
+            ],
             force_login=False,
         )
 
         self.xtract_tokens = {
-            "auth_token": auths["petrel"].access_token,
-            "transfer_token": auths["transfer"].authorizer.access_token,
-            "funcx_token": auths[
+            "auth_token": self.auths["petrel"].access_token,
+            "transfer_token": self.auths["transfer"].authorizer.access_token,
+            "funcx_token": self.auths[
                 "https://auth.globus.org/scopes/facd7ccc-c5f4-42aa-916b-a0e270e2c2a9/all"
             ].access_token,
         }
 
     def load(self, name, download=True, globus=True, verbose=False, metadata=None, authorizers=None, **kwargs):
         """Load the metadata for a Foundry dataset into the client
         Args:
@@ -268,25 +281,25 @@
         Args:
            inputs (list): List of strings for input columns
            targets (list): List of strings for output columns
            source_id (string): Relative path to the source file
            as_hdf5 (bool): If True and dataset is in hdf5 format, keep data in hdf5 format
 
         Returns
-        -------s
+        -------
              (tuple): Tuple of X, y values
         """
         data = {}
 
         # Handle splits if they exist. Return as a labeled dictionary of tuples
         try:
             if self.dataset.splits:
                 for split in self.dataset.splits:
-                    data[split.label] = self._load_data(file=split.path,
-                                                        source_id=source_id, globus=globus, as_hdf5=as_hdf5)
+                    data[split.label] = self._load_data(file=split.path, source_id=source_id, globus=globus,
+                                                        as_hdf5=as_hdf5)
                 return data
             else:
                 return {"data": self._load_data(source_id=source_id, globus=globus, as_hdf5=as_hdf5)}
         except Exception as e:
             raise Exception(
                 "Metadata not loaded into Foundry object, make sure to call load()") from e
 
@@ -317,28 +330,41 @@
         bibtex = os.linesep.join([doi_str, url_str,
                                   author_str, title_str,
                                   keywords_str, publisher_str,
                                   year_str])
         bibtex = f"@misc{{https://doi.org/{self.dc['identifier']['identifier']}{os.linesep}{bibtex}}}"
         return bibtex
 
-    def publish(self, foundry_metadata, data_source, title, authors, update=False,
-                publication_year=None, **kwargs, ):
-        """Submit a dataset for publication
+    def publish_dataset(
+            self, foundry_metadata: Dict[str, Any], title: str, authors: List[str], https_data_path: str = None,
+            globus_data_source: str = None, update: bool = False, publication_year: int = None, test: bool = False,
+            **kwargs: Dict[str, Any],) -> Dict[str, Any]:
+        """Submit a dataset for publication; can choose to submit via HTTPS using `https_data_path` or via Globus
+            Transfer using the `globus_data_source` argument. Only one upload method may be specified.
         Args:
             foundry_metadata (dict): Dict of metadata describing data package
-            data_source (string): Url for Globus endpoint
             title (string): Title of data package
             authors (list): List of data package author names e.g., Jack Black
                 or Nunez, Victoria
+            https_data_path (str): Path to the local dataset to publish to Foundry via HTTPS. Creates an HTTPS PUT
+                request to upload the data specified to a Globus endpoint (default is NCSA endpoint) before it is
+                transferred to MDF. If None, the user must specify a 'globus_data_source' URL to the location of the
+                data on their own Globus endpoint. User must choose either `globus_data_source` or `https_data_path` to
+                publish their data.
+            globus_data_source (str): Url path for a data folder on a Globus endpoint; url can be obtained through
+                the Globus Web UI or SDK. If None, the user must specify an 'https_data_path' pointing to the location
+                of the data on their local machine. User must choose either `globus_data_source` or `https_data_path` to
+                publish their data.
             update (bool): True if this is an update to a prior data package
                 (default: self.config.metadata_file)
             publication_year (int): Year of dataset publication. If None, will
                 be set to the current calendar year by MDF Connect Client.
                 (default: $current_year)
+            test (bool): If True, do not submit the dataset for publication (ie transfer to the MDF endpoint).
+                Default is False.
 
         Keyword Args:
             affiliations (list): List of author affiliations
             tags (list): List of tags to apply to the data package
             short_name (string): Shortened/abbreviated name of the data package
             publisher (string): Data publishing entity (e.g. MDF, Zenodo, etc.)
             description (str): A description of the dataset.
@@ -348,32 +374,57 @@
 
         Returns
         -------
         (dict) MDF Connect Response: Response from MDF Connect to allow tracking
             of dataset. Contains `source_id`, which can be used to check the
             status of the submission
         """
+        # ensure that one of `https_data_path` or `globus_data_source` have been assigned values
+        if (https_data_path and globus_data_source) or \
+                (https_data_path is None and globus_data_source is None):
+            raise ValueError("Must assign either `https_data_path` or `globus_data_source`")
+
         self.connect_client.create_dc_block(
             title=title,
             authors=authors,
             affiliations=kwargs.get("affiliations", []),
             subjects=kwargs.get("tags", ["machine learning", "foundry"]),
             publisher=kwargs.get("publisher", ""),
             publication_year=publication_year,
             description=kwargs.get("description", ""),
             dataset_doi=kwargs.get("dataset_doi", ""),
             related_dois=kwargs.get("related_dois", [])
         )
         self.connect_client.add_organization(self.config.organization)
         self.connect_client.set_project_block(
             self.config.metadata_key, foundry_metadata)
-        self.connect_client.add_data_source(data_source)
+
+        # upload via HTTPS if specified
+        if https_data_path:
+            # gather auth'd clients necessary for publication to endpoint
+            endpoint_id = "82f1b5c6-6e9b-11e5-ba47-22000b92c6ec"  # NCSA endpoint
+            scope = f"https://auth.globus.org/scopes/{endpoint_id}/https"  # lets you HTTPS to specific endpoint
+            pub_auths = PubAuths(
+                transfer_client=self.auths["transfer"],
+                auth_client_openid=AuthClient(authorizer=self.auths['openid']),
+                endpoint_auth_clients={endpoint_id: AuthClient(authorizer=self.auths[scope])}
+            )
+            # upload (ie publish) data to endpoint
+            globus_data_source = upload_to_endpoint(pub_auths, https_data_path, endpoint_id)
+        # set Globus data source URL with MDF
+        self.connect_client.add_data_source(globus_data_source)
+        # set dataset name using the title if an abbreviated short_name isn't specified
         self.connect_client.set_source_name(kwargs.get("short_name", title))
 
-        res = self.connect_client.submit_dataset(update=update)
+        # do not submit to MDF if this is just a test
+        if not test:
+            # Globus Transfer the data from the data source to the MDF endpoint
+            res = self.connect_client.submit_dataset(update=update)
+        else:
+            res = None
         return res
 
     def publish_model(self, title, creators, short_name, servable_type, serv_options, affiliations=None, paper_doi=None):
         """Simplified publishing method for servables
 
         Args:
             title (string): title for the servable
```

### Comparing `foundry_ml-0.5.1/foundry/https_download.py` & `foundry_ml-0.6.0/foundry/https_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""Methods to download files from a Globus endpoint using Xtract (HTTPS). Now deprecated as of Aug 2022
+"""
+
+
 import os
 from collections import deque
 
 import requests
 from globus_sdk import TransferClient
```

### Comparing `foundry_ml-0.5.1/foundry/loaders/tf_wrapper.py` & `foundry_ml-0.6.0/foundry/loaders/tf_wrapper.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.5.1/foundry/loaders/torch_wrapper.py` & `foundry_ml-0.6.0/foundry/loaders/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.5.1/foundry/models.py` & `foundry_ml-0.6.0/foundry/models.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.5.1/foundry/utils.py` & `foundry_ml-0.6.0/foundry/utils.py`

 * *Files identical despite different names*

### Comparing `foundry_ml-0.5.1/foundry_ml.egg-info/PKG-INFO` & `foundry_ml-0.6.0/foundry_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-ml
-Version: 0.5.1
+Version: 0.6.0
 Summary: Package to support simplified application of machine learning models to datasets in materials science
 Home-page: https://github.com/MLMI2-CSSI/foundry
 Author: Aristana Scourtas, KJ Schmidt, Isaac Darling, Aadit Ambadkar, Braeden Cullen,
             Imogen Foster, Ribhav Bose, Zoa Katok, Ethan Truelove, Ian Foster, Ben Blaiszik
 Author-email: blaiszik@uchicago.edu
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,15 @@
   <img src="https://raw.githubusercontent.com/MLMI2-CSSI/foundry/main/assets/foundry-black.png" height="175">
 </picture>
 
 [![PyPI](https://img.shields.io/pypi/v/foundry_ml.svg)](https://pypi.python.org/pypi/foundry_ml)
 [![Tests](https://github.com/MLMI2-CSSI/foundry/actions/workflows/tests.yml/badge.svg)](https://github.com/MLMI2-CSSI/foundry/actions/workflows/tests.yml)
 [![Tests](https://github.com/MLMI2-CSSI/foundry/actions/workflows/python-publish.yml/badge.svg)](https://github.com/MLMI2-CSSI/foundry/actions/workflows/python-publish.yml)
 [![NSF-1931306](https://img.shields.io/badge/NSF-1931306-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1931306&HistoricalAwards=false)
+[<img src="https://img.shields.io/badge/view-documentation-blue">](https://ai-materials-and-chemistry.gitbook.io/foundry/)
 
 
 Foundry-ML simplifies the discovery and usage of ML-ready datasets in materials science and chemistry providing a simple API to access even complex datasets. 
 * Load ML-ready data with just a few lines of code
 * Work with datasets in local or cloud environments. 
 * Publish your own datasets with Foundry to promote community usage
 * (in progress) Run published ML models without hassle
```

### Comparing `foundry_ml-0.5.1/setup.py` & `foundry_ml-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 packages = (setuptools.find_packages(),)
 setuptools.setup(
     name="foundry_ml",
-    version="0.5.1",
+    version="0.6.0",
     author="""Aristana Scourtas, KJ Schmidt, Isaac Darling, Aadit Ambadkar, Braeden Cullen,
             Imogen Foster, Ribhav Bose, Zoa Katok, Ethan Truelove, Ian Foster, Ben Blaiszik""",
     author_email="blaiszik@uchicago.edu",
     packages=setuptools.find_packages(),
     description="Package to support simplified application of machine learning models to datasets in materials science",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `foundry_ml-0.5.1/tests/test_foundry.py` & `foundry_ml-0.6.0/tests/test_foundry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,44 @@
+import json
 import os
 import shutil
 import pytest
+from filecmp import cmp
 from datetime import datetime
+from math import floor
+import numpy as np
+import requests
 import mdf_toolbox
 import pandas as pd
 from mdf_forge import Forge
 from foundry import Foundry
+from foundry.auth import PubAuths
+from foundry.https_upload import upload_to_endpoint
 from dlhub_sdk import DLHubClient
+from globus_sdk import AuthClient
 from mdf_connect_client import MDFConnectClient
 
+
 client_id = os.getenv("CLIENT_ID")
 client_secret = os.getenv("CLIENT_SECRET")
 is_gha = os.getenv("GITHUB_ACTIONS")
 
 services = [
-            "data_mdf",
-            "mdf_connect",
-            "search",
-            "dlhub",
-            "petrel",
-            "transfer",
-            "openid",
-            "https://auth.globus.org/scopes/facd7ccc-c5f4-42aa-916b-a0e270e2c2a9/all"]
+    "data_mdf",
+    "mdf_connect",
+    "search",
+    "petrel",
+    "transfer",
+    "dlhub",
+    "openid",
+    "https://auth.globus.org/scopes/facd7ccc-c5f4-42aa-916b-a0e270e2c2a9/all",  # funcx
+    "https://auth.globus.org/scopes/f10a69a9-338c-4e5b-baa1-0dc92359ab47/https",  # Eagle HTTPS
+    "https://auth.globus.org/scopes/82f1b5c6-6e9b-11e5-ba47-22000b92c6ec/https",  # NCSA HTTPS
+    "https://auth.globus.org/scopes/d31d4f5d-be37-4adc-a761-2f716b7af105/action_all",  # Globus Search Lambda
+]
 
 if is_gha:
     auths = mdf_toolbox.confidential_login(client_id=client_id,
                                            client_secret=client_secret,
                                            services=services, make_clients=True)
 
     search_auth = mdf_toolbox.confidential_login(client_id=client_id,
@@ -239,47 +252,128 @@
     assert isinstance(X, pd.DataFrame)
     assert len(y) > 1
     assert isinstance(y, pd.DataFrame)
     _delete_test_data(f)
 
 
 @pytest.mark.skipif(bool(is_gha), reason="Not run as part of GHA CI")
-def test_publish():
+def test_publish_with_https():
+    """System test: Assess the end-to-end publication of a dataset via HTTPS
+    """
+
+    f = Foundry(index="mdf-test", authorizers=auths)
+    timestamp = datetime.now().timestamp()
+    title = "https_publish_test_{:.0f}".format(timestamp)
+    short_name = "https_pub_{:.0f}".format(timestamp)
+    authors = ["A Scourtas"]
+    local_path = "./data/https_test"
+
+    # create test JSON to upload (if it doesn't already exist)
+    _write_test_data(local_path)
+
+    res = f.publish_dataset(pub_test_metadata, title, authors, https_data_path=local_path, short_name=short_name)
+
+    assert res['success']
+    assert res['source_id'] == f"_test_{short_name}_v1.1"
+
+
+def test_upload_to_endpoint():
+    """Unit test: Test the _upload_to_endpoint() HTTPS functionality on its own, without publishing to MDF
+    """
+    endpoint_id = "82f1b5c6-6e9b-11e5-ba47-22000b92c6ec"  # NCSA endpoint
+    dest_parent = "/tmp"
+    dest_child = f"test_{floor(datetime.now().timestamp())}"
+    local_path = "./data/https_test"
+    filename = "test_data.json"
+
+    f = Foundry(index="mdf-test", authorizers=auths)
+    # create test JSON to upload (if it doesn't already exist)
+    _write_test_data(local_path, filename)
+
+    # gather auth'd clients necessary for publication to endpoint
+    endpoint_id = "82f1b5c6-6e9b-11e5-ba47-22000b92c6ec"  # NCSA endpoint
+    scope = f"https://auth.globus.org/scopes/{endpoint_id}/https"  # lets you HTTPS to specific endpoint
+    pub_auths = PubAuths(
+        transfer_client=f.auths["transfer"],
+        auth_client_openid=AuthClient(authorizer=f.auths['openid']),
+        endpoint_auth_clients={endpoint_id: AuthClient(authorizer=f.auths[scope])}
+    )
+    # upload via HTTPS to NCSA endpoint
+    globus_data_source = upload_to_endpoint(pub_auths, local_path, endpoint_id, dest_parent=dest_parent,
+                                            dest_child=dest_child)
+
+    expected_data_source = f"https://app.globus.org/file-manager?origin_id=82f1b5c6-6e9b-11e5-ba47-22000b92c6ec&" \
+                           f"origin_path=%2Ftmp%2F{dest_child}"
+    # confirm data source link was created properly, with correct folders
+    assert globus_data_source == expected_data_source
+
+    mdf_url = f"https://data.materialsdatafacility.org/tmp/{dest_child}/{filename}"
+    response = requests.get(mdf_url)
+    # check that we get a valid response back (note that a 200 could be a UI error, returned as HTML)
+    assert response.status_code == 200
+    # check that contents of response are as expected
+    tmp_file = "./data/tmp_data.json"
+    with open(tmp_file, "wb") as fl:
+        fl.write(response.content)
+    assert cmp(tmp_file, os.path.join(local_path, filename))
+
+
+def _write_test_data(dest_path="./data/https_test", filename="test_data.json"):
+    # Create random JSON data
+    data = pd.DataFrame(np.random.rand(100, 4), columns=list('ABCD'))
+    res = data.to_json(orient="records")
+
+    # Make data directory
+    os.makedirs(dest_path, exist_ok=True)
+    data_filepath = os.path.join(dest_path, filename)
+
+    # Write data to JSON file
+    with open(data_filepath, "w+") as f:
+        json.dump(res, f, indent=4)
+
+
+def test_ACL_creation_and_deletion():
+    pass
+
+
+@pytest.mark.skipif(bool(is_gha), reason="Not run as part of GHA CI")
+def test_publish_with_globus():
     # TODO: automate dealing with curation and cleaning after tests
 
     f = Foundry(authorizers=auths, index="mdf-test", no_browser=True, no_local_server=True)
 
     timestamp = datetime.now().timestamp()
     title = "scourtas_example_iris_test_publish_{:.0f}".format(timestamp)
     short_name = "example_AS_iris_test_{:.0f}".format(timestamp)
     authors = ["A Scourtas"]
 
-    res = f.publish(pub_test_metadata, pub_test_data_source, title, authors, short_name=short_name)
+    res = f.publish_dataset(pub_test_metadata, title, authors, globus_data_source=pub_test_data_source,
+                            short_name=short_name)
 
     # publish with short name
     assert res['success']
     assert res['source_id'] == "_test_example_iris_{:.0f}_v1.1".format(timestamp)
 
     # TODO: publish with long title -- for some reason even when I change the title, it still says it's already pub'd
     # title += "long"
     # res = f.publish(pub_test_metadata, pub_test_data_source, title, authors)
     # assert res['success']
     # assert res['source_id'] == "_test_scourtas_example_iris_publish_{:.0f}_v1.1".format(timestamp)
 
     # check that pushing same dataset without update flag fails
-    res = f.publish(pub_test_metadata, pub_test_data_source, title, authors, short_name=short_name)
+    res = f.publish_dataset(pub_test_metadata, title, authors, globus_data_source=pub_test_data_source, short_name=short_name)
     assert not res['success']
 
     # check that using update flag allows us to update dataset
-    res = f.publish(pub_test_metadata, pub_test_data_source, title, authors, short_name=short_name, update=True)
+    res = f.publish_dataset(pub_test_metadata, title, authors, globus_data_source=pub_test_data_source, short_name=short_name, update=True)
     assert res['success']
 
     # check that using update flag for new dataset fails
     new_short_name = short_name + "_update"
-    res = f.publish(pub_test_metadata, pub_test_data_source, title, authors, short_name=new_short_name, update=True)
+    res = f.publish_dataset(pub_test_metadata, title, authors, globus_data_source=pub_test_data_source, short_name=new_short_name,  update=True)
     assert not res['success']
 
 
 def test_check_status():
     # TODO: the 'active messages' in MDF CC's check_status() don't appear to do anything? need to determine how to test
     pass
```

