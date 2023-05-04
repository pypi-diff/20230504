# Comparing `tmp/dcachefs-0.1.6.tar.gz` & `tmp/dcachefs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dcachefs-0.1.6.tar", last modified: Wed Sep 14 08:22:53 2022, max compression
+gzip compressed data, was "dist/dcachefs-0.1.7.tar", last modified: Thu May  4 21:12:37 2023, max compression
```

## Comparing `dcachefs-0.1.6.tar` & `dcachefs-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:22:53.000000 dcachefs-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-09-14 08:22:43.000000 dcachefs-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-14 08:22:43.000000 dcachefs-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5661 2022-09-14 08:22:53.000000 dcachefs-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3932 2022-09-14 08:22:43.000000 dcachefs-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:22:53.000000 dcachefs-0.1.6/dcachefs/
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-14 08:22:43.000000 dcachefs-0.1.6/dcachefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-14 08:22:43.000000 dcachefs-0.1.6/dcachefs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24821 2022-09-14 08:22:43.000000 dcachefs-0.1.6/dcachefs/dcachefs.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-14 08:22:43.000000 dcachefs-0.1.6/dcachefs/register_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 08:22:53.000000 dcachefs-0.1.6/dcachefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5661 2022-09-14 08:22:53.000000 dcachefs-0.1.6/dcachefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-14 08:22:53.000000 dcachefs-0.1.6/dcachefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 08:22:53.000000 dcachefs-0.1.6/dcachefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 08:22:53.000000 dcachefs-0.1.6/dcachefs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-14 08:22:53.000000 dcachefs-0.1.6/dcachefs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-14 08:22:53.000000 dcachefs-0.1.6/dcachefs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-14 08:22:53.000000 dcachefs-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-09-14 08:22:43.000000 dcachefs-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:37.000000 dcachefs-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-04 21:12:12.000000 dcachefs-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 21:12:12.000000 dcachefs-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-04 21:12:37.000000 dcachefs-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-04 21:12:12.000000 dcachefs-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:37.000000 dcachefs-0.1.7/dcachefs/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-04 21:12:12.000000 dcachefs-0.1.7/dcachefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 21:12:12.000000 dcachefs-0.1.7/dcachefs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25031 2023-05-04 21:12:12.000000 dcachefs-0.1.7/dcachefs/dcachefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:12:37.000000 dcachefs-0.1.7/dcachefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-04 21:12:37.000000 dcachefs-0.1.7/dcachefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-04 21:12:37.000000 dcachefs-0.1.7/dcachefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:12:37.000000 dcachefs-0.1.7/dcachefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:12:37.000000 dcachefs-0.1.7/dcachefs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 21:12:37.000000 dcachefs-0.1.7/dcachefs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 21:12:37.000000 dcachefs-0.1.7/dcachefs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-04 21:12:37.000000 dcachefs-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-04 21:12:12.000000 dcachefs-0.1.7/setup.py
```

### Comparing `dcachefs-0.1.6/LICENSE` & `dcachefs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dcachefs-0.1.6/PKG-INFO` & `dcachefs-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dcachefs
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python filesystem interface for dCache
 Home-page: https://github.com/NLeSC-GO-common-infrastructure/dcachefs
 Author: Francesco Nattino
 Author-email: f.nattino@esciencecenter.nl
 License: Apache Software License 2.0
 Description: .. list-table::
            :widths: 25 25
@@ -22,14 +22,16 @@
              - |Zenodo Badge|
            * - \5. Checklist
              - |CII Best Practices Badge|
            * - **Other best practices**
              -
            * - Continuous integration
              - |Python Build| |PyPI Publish|
+           * - Documentation
+             - |Read the Docs|
         
         
         .. |GitHub Badge| image:: https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue
            :target: https://github.com/NLeSC-GO-common-infrastructure/dcachefs
            :alt: GitHub Badge
         
         .. |License Badge| image:: https://img.shields.io/github/license/NLeSC-GO-common-infrastructure/dcachefs
@@ -52,14 +54,18 @@
            :target: https://github.com/NLeSC-GO-common-infrastructure/dcachefs/actions?query=workflow%3A%22Build%22
            :alt: Python Build
         
         .. |PyPI Publish| image:: https://github.com/NLeSC-GO-common-infrastructure/dcachefs/workflows/Publish/badge.svg
            :target: https://github.com/NLeSC-GO-common-infrastructure/dcachefs/actions?query=workflow%3A%22Publish%22
            :alt: PyPI Publish
         
+        .. |Read the Docs| image:: https://readthedocs.org/projects/dcachefs/badge/?version=latest
+           :target: https://dcachefs.readthedocs.io
+           :alt: Read the Docs
+        
         ################################################################################
         dCacheFS
         ################################################################################
         
         dCacheFS provides a file-system interface for a `dCache storage system`_, such as the `instance provided at SURF`_. 
         dCacheFS builds on the `Filesystem Spec`_ (`fsspec`) library and it can be used as an independent library or via the 
         more general `fsspec` functions.
```

### Comparing `dcachefs-0.1.6/README.rst` & `dcachefs-0.1.7/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
      - |Zenodo Badge|
    * - \5. Checklist
      - |CII Best Practices Badge|
    * - **Other best practices**
      -
    * - Continuous integration
      - |Python Build| |PyPI Publish|
+   * - Documentation
+     - |Read the Docs|
 
 
 .. |GitHub Badge| image:: https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue
    :target: https://github.com/NLeSC-GO-common-infrastructure/dcachefs
    :alt: GitHub Badge
 
 .. |License Badge| image:: https://img.shields.io/github/license/NLeSC-GO-common-infrastructure/dcachefs
@@ -44,14 +46,18 @@
    :target: https://github.com/NLeSC-GO-common-infrastructure/dcachefs/actions?query=workflow%3A%22Build%22
    :alt: Python Build
 
 .. |PyPI Publish| image:: https://github.com/NLeSC-GO-common-infrastructure/dcachefs/workflows/Publish/badge.svg
    :target: https://github.com/NLeSC-GO-common-infrastructure/dcachefs/actions?query=workflow%3A%22Publish%22
    :alt: PyPI Publish
 
+.. |Read the Docs| image:: https://readthedocs.org/projects/dcachefs/badge/?version=latest
+   :target: https://dcachefs.readthedocs.io
+   :alt: Read the Docs
+
 ################################################################################
 dCacheFS
 ################################################################################
 
 dCacheFS provides a file-system interface for a `dCache storage system`_, such as the `instance provided at SURF`_. 
 dCacheFS builds on the `Filesystem Spec`_ (`fsspec`) library and it can be used as an independent library or via the 
 more general `fsspec` functions.
```

### Comparing `dcachefs-0.1.6/dcachefs/dcachefs.py` & `dcachefs-0.1.7/dcachefs/dcachefs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import aiohttp
 import asyncio
 import logging
 import weakref
+import yarl
 
 from datetime import datetime
 from fsspec.asyn import sync_wrapper, sync, AsyncFileSystem
 from fsspec.implementations.http import get_client, HTTPFile, HTTPStreamFile
 from fsspec.utils import DEFAULT_BLOCK_SIZE
 from urllib.parse import quote
 from urlpath import URL
@@ -74,14 +75,15 @@
         is the buffer size (in bytes) for reading and writing. when reading,
         this is also the size downloaded in one request. if 0, will default to
         raw requests file-like objects
     :param asynchronous: (bool, optional) use in asynchronous mode
     :param loop: (optional) if asynchronous, event loop where to run coroutines
     :param batch_size: (int, optional) if asynchronous, number of coroutines to
         submit/wait on simultaneously
+    :param encoded: use encoded strings when formatting URLs
     :param storage_options: (dict, optional) keyword arguments passed on to the
         super-class
     """
 
     def __init__(
         self,
         api_url=None,
@@ -91,27 +93,29 @@
         token=None,
         client_kwargs=None,
         request_kwargs=None,
         block_size=None,
         asynchronous=False,
         loop=None,
         batch_size=None,
+        encoded=True,
         **storage_options
     ):
         super().__init__(
             self,
             asynchronous=asynchronous,
             loop=loop,
             batch_size=batch_size,
             **storage_options
         )
         self.api_url = api_url
         self.webdav_url = webdav_url
         self.client_kwargs = {} if client_kwargs is None else client_kwargs
         self.request_kwargs = {} if request_kwargs is None else request_kwargs
+        self.encoded = encoded
         if (username is None) ^ (password is None):
             raise ValueError('Username or password not provided')
         if (username is not None) and (password is not None):
             self.client_kwargs.update(
                 auth=aiohttp.BasicAuth(username, password)
             )
         if token is not None:
@@ -135,14 +139,17 @@
             except (TimeoutError, FSTimeoutError):
                 pass
         connector = getattr(session, "_connector", None)
         if connector is not None:
             # close after loop is dead
             connector._close()
 
+    def encode_url(self, url):
+        return yarl.URL(url, encoded=self.encoded)
+
     async def set_session(self):
         if self._session is None:
             self._session = await get_client(
                 loop=self.loop,
                 **self.client_kwargs
             )
             if not self.asynchronous:
@@ -182,15 +189,15 @@
         :param path: (str or list) target path(s)
         :return: (str or list) target path(s) stripped from protocol and WebDAV
             door
         """
         if isinstance(path, list):
             return [cls._strip_protocol(p) for p in path]
         url = URL(path)
-        return url.path if "http" in url.scheme else path.split(":/")[-1]
+        return url.path if "http" in url.scheme else path.split("://")[-1]
 
     @classmethod
     def _get_kwargs_from_urls(cls, path):
         """
         Extract keyword arguments encoded in the urlpath.
 
         :param path: (str) target path
```

### Comparing `dcachefs-0.1.6/dcachefs.egg-info/PKG-INFO` & `dcachefs-0.1.7/dcachefs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dcachefs
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python filesystem interface for dCache
 Home-page: https://github.com/NLeSC-GO-common-infrastructure/dcachefs
 Author: Francesco Nattino
 Author-email: f.nattino@esciencecenter.nl
 License: Apache Software License 2.0
 Description: .. list-table::
            :widths: 25 25
@@ -22,14 +22,16 @@
              - |Zenodo Badge|
            * - \5. Checklist
              - |CII Best Practices Badge|
            * - **Other best practices**
              -
            * - Continuous integration
              - |Python Build| |PyPI Publish|
+           * - Documentation
+             - |Read the Docs|
         
         
         .. |GitHub Badge| image:: https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue
            :target: https://github.com/NLeSC-GO-common-infrastructure/dcachefs
            :alt: GitHub Badge
         
         .. |License Badge| image:: https://img.shields.io/github/license/NLeSC-GO-common-infrastructure/dcachefs
@@ -52,14 +54,18 @@
            :target: https://github.com/NLeSC-GO-common-infrastructure/dcachefs/actions?query=workflow%3A%22Build%22
            :alt: Python Build
         
         .. |PyPI Publish| image:: https://github.com/NLeSC-GO-common-infrastructure/dcachefs/workflows/Publish/badge.svg
            :target: https://github.com/NLeSC-GO-common-infrastructure/dcachefs/actions?query=workflow%3A%22Publish%22
            :alt: PyPI Publish
         
+        .. |Read the Docs| image:: https://readthedocs.org/projects/dcachefs/badge/?version=latest
+           :target: https://dcachefs.readthedocs.io
+           :alt: Read the Docs
+        
         ################################################################################
         dCacheFS
         ################################################################################
         
         dCacheFS provides a file-system interface for a `dCache storage system`_, such as the `instance provided at SURF`_. 
         dCacheFS builds on the `Filesystem Spec`_ (`fsspec`) library and it can be used as an independent library or via the 
         more general `fsspec` functions.
```

### Comparing `dcachefs-0.1.6/setup.py` & `dcachefs-0.1.7/setup.py`

 * *Files identical despite different names*

