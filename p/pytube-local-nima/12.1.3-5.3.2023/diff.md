# Comparing `tmp/pytube_local_nima-12.1.3.tar.gz` & `tmp/pytube_local_nima-5.3.2023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytube_local_nima-12.1.3.tar", last modified: Wed May  3 23:37:36 2023, max compression
+gzip compressed data, was "dist/pytube_local_nima-5.3.2023.tar", last modified: Wed May  3 21:48:01 2023, max compression
```

## Comparing `pytube_local_nima-12.1.3.tar` & `pytube_local_nima-5.3.2023.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/
--rw-r--r--   0 nima       (501) staff       (20)     5993 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/PKG-INFO
--rw-r--r--   0 nima       (501) staff       (20)     1211 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/LICENSE
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/pytube/
--rw-r--r--   0 nima       (501) staff       (20)    11654 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/innertube.py
--rw-r--r--   0 nima       (501) staff       (20)    15288 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/streams.py
--rw-r--r--   0 nima       (501) staff       (20)     1482 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/metadata.py
--rw-r--r--   0 nima       (501) staff       (20)       74 2023-05-03 23:29:30.000000 pytube_local_nima-12.1.3/pytube/version.py
--rw-r--r--   0 nima       (501) staff       (20)      451 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/monostate.py
--rw-r--r--   0 nima       (501) staff       (20)    12844 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/query.py
--rw-r--r--   0 nima       (501) staff       (20)     8512 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/request.py
--rw-r--r--   0 nima       (501) staff       (20)      592 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/__init__.py
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/pytube/contrib/
--rw-r--r--   0 nima       (501) staff       (20)     6576 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/contrib/channel.py
--rw-r--r--   0 nima       (501) staff       (20)        0 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/contrib/__init__.py
--rw-r--r--   0 nima       (501) staff       (20)    14204 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/contrib/playlist.py
--rw-r--r--   0 nima       (501) staff       (20)     8886 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/contrib/search.py
--rw-r--r--   0 nima       (501) staff       (20)     5931 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/parser.py
--rw-r--r--   0 nima       (501) staff       (20)    22529 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/cipher.py
--rwxr-xr-x   0 nima       (501) staff       (20)    16635 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/cli.py
--rw-r--r--   0 nima       (501) staff       (20)     4311 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/itags.py
--rw-r--r--   0 nima       (501) staff       (20)     3907 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/exceptions.py
--rw-r--r--   0 nima       (501) staff       (20)     5648 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/captions.py
--rw-r--r--   0 nima       (501) staff       (20)     9794 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/helpers.py
--rw-r--r--   0 nima       (501) staff       (20)    17798 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/extract.py
--rw-r--r--   0 nima       (501) staff       (20)    15423 2023-05-03 20:32:44.000000 pytube_local_nima-12.1.3/pytube/__main__.py
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/tests/
--rw-r--r--   0 nima       (501) staff       (20)     1406 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_parser.py
--rw-r--r--   0 nima       (501) staff       (20)    13696 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_streams.py
--rw-r--r--   0 nima       (501) staff       (20)     2736 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_cipher.py
--rw-r--r--   0 nima       (501) staff       (20)     4921 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/conftest.py
--rw-r--r--   0 nima       (501) staff       (20)      276 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_itags.py
--rw-r--r--   0 nima       (501) staff       (20)     1820 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_request.py
--rw-r--r--   0 nima       (501) staff       (20)      498 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_metadata.py
--rw-r--r--   0 nima       (501) staff       (20)     3452 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_exceptions.py
--rw-r--r--   0 nima       (501) staff       (20)       57 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/__init__.py
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/tests/contrib/
--rw-r--r--   0 nima       (501) staff       (20)     3122 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/contrib/test_channel.py
--rw-r--r--   0 nima       (501) staff       (20)    11623 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/contrib/test_playlist.py
--rw-r--r--   0 nima       (501) staff       (20)     6148 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_query.py
--rw-r--r--   0 nima       (501) staff       (20)     5024 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_helpers.py
--rw-r--r--   0 nima       (501) staff       (20)     2957 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_extract.py
--rw-r--r--   0 nima       (501) staff       (20)    17295 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_cli.py
--rw-r--r--   0 nima       (501) staff       (20)     1915 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_main.py
--rw-r--r--   0 nima       (501) staff       (20)     5759 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/tests/test_captions.py
--rw-r--r--   0 nima       (501) staff       (20)       55 2023-05-03 20:08:10.000000 pytube_local_nima-12.1.3/MANIFEST.in
--rw-r--r--   0 nima       (501) staff       (20)     4054 2023-05-03 21:37:12.000000 pytube_local_nima-12.1.3/README.md
-drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/pytube_local_nima.egg-info/
--rw-r--r--   0 nima       (501) staff       (20)     5993 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/pytube_local_nima.egg-info/PKG-INFO
--rw-r--r--   0 nima       (501) staff       (20)        1 2023-05-03 21:48:01.000000 pytube_local_nima-12.1.3/pytube_local_nima.egg-info/zip-safe
--rw-r--r--   0 nima       (501) staff       (20)     1069 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/pytube_local_nima.egg-info/SOURCES.txt
--rw-r--r--   0 nima       (501) staff       (20)       55 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/pytube_local_nima.egg-info/entry_points.txt
--rw-r--r--   0 nima       (501) staff       (20)        7 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/pytube_local_nima.egg-info/top_level.txt
--rw-r--r--   0 nima       (501) staff       (20)        1 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/pytube_local_nima.egg-info/dependency_links.txt
--rwxr-xr-x   0 nima       (501) staff       (20)     1871 2023-05-03 21:38:46.000000 pytube_local_nima-12.1.3/setup.py
--rw-r--r--   0 nima       (501) staff       (20)       38 2023-05-03 23:37:36.000000 pytube_local_nima-12.1.3/setup.cfg
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/
+-rw-r--r--   0 nima       (501) staff       (20)     5995 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/PKG-INFO
+-rw-r--r--   0 nima       (501) staff       (20)     1211 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/LICENSE
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube/
+-rw-r--r--   0 nima       (501) staff       (20)    11654 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/innertube.py
+-rw-r--r--   0 nima       (501) staff       (20)    15288 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/streams.py
+-rw-r--r--   0 nima       (501) staff       (20)     1482 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/metadata.py
+-rw-r--r--   0 nima       (501) staff       (20)       76 2023-05-03 21:04:35.000000 pytube_local_nima-5.3.2023/pytube/version.py
+-rw-r--r--   0 nima       (501) staff       (20)      451 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/monostate.py
+-rw-r--r--   0 nima       (501) staff       (20)    12844 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/query.py
+-rw-r--r--   0 nima       (501) staff       (20)     8512 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/request.py
+-rw-r--r--   0 nima       (501) staff       (20)      592 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/__init__.py
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube/contrib/
+-rw-r--r--   0 nima       (501) staff       (20)     6576 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/contrib/channel.py
+-rw-r--r--   0 nima       (501) staff       (20)        0 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/contrib/__init__.py
+-rw-r--r--   0 nima       (501) staff       (20)    14204 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/contrib/playlist.py
+-rw-r--r--   0 nima       (501) staff       (20)     8886 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/contrib/search.py
+-rw-r--r--   0 nima       (501) staff       (20)     5931 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/parser.py
+-rw-r--r--   0 nima       (501) staff       (20)    22529 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/cipher.py
+-rwxr-xr-x   0 nima       (501) staff       (20)    16635 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/cli.py
+-rw-r--r--   0 nima       (501) staff       (20)     4311 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/itags.py
+-rw-r--r--   0 nima       (501) staff       (20)     3907 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/exceptions.py
+-rw-r--r--   0 nima       (501) staff       (20)     5648 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/captions.py
+-rw-r--r--   0 nima       (501) staff       (20)     9794 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/helpers.py
+-rw-r--r--   0 nima       (501) staff       (20)    17798 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/extract.py
+-rw-r--r--   0 nima       (501) staff       (20)    15423 2023-05-03 20:32:44.000000 pytube_local_nima-5.3.2023/pytube/__main__.py
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/tests/
+-rw-r--r--   0 nima       (501) staff       (20)     1406 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_parser.py
+-rw-r--r--   0 nima       (501) staff       (20)    13696 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_streams.py
+-rw-r--r--   0 nima       (501) staff       (20)     2736 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_cipher.py
+-rw-r--r--   0 nima       (501) staff       (20)     4921 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/conftest.py
+-rw-r--r--   0 nima       (501) staff       (20)      276 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_itags.py
+-rw-r--r--   0 nima       (501) staff       (20)     1820 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_request.py
+-rw-r--r--   0 nima       (501) staff       (20)      498 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_metadata.py
+-rw-r--r--   0 nima       (501) staff       (20)     3452 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_exceptions.py
+-rw-r--r--   0 nima       (501) staff       (20)       57 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/__init__.py
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/tests/contrib/
+-rw-r--r--   0 nima       (501) staff       (20)     3122 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/contrib/test_channel.py
+-rw-r--r--   0 nima       (501) staff       (20)    11623 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/contrib/test_playlist.py
+-rw-r--r--   0 nima       (501) staff       (20)     6148 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_query.py
+-rw-r--r--   0 nima       (501) staff       (20)     5024 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_helpers.py
+-rw-r--r--   0 nima       (501) staff       (20)     2957 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_extract.py
+-rw-r--r--   0 nima       (501) staff       (20)    17295 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_cli.py
+-rw-r--r--   0 nima       (501) staff       (20)     1915 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_main.py
+-rw-r--r--   0 nima       (501) staff       (20)     5759 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/tests/test_captions.py
+-rw-r--r--   0 nima       (501) staff       (20)       55 2023-05-03 20:08:10.000000 pytube_local_nima-5.3.2023/MANIFEST.in
+-rw-r--r--   0 nima       (501) staff       (20)     4054 2023-05-03 21:37:12.000000 pytube_local_nima-5.3.2023/README.md
+drwxr-xr-x   0 nima       (501) staff       (20)        0 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/
+-rw-r--r--   0 nima       (501) staff       (20)     5995 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/PKG-INFO
+-rw-r--r--   0 nima       (501) staff       (20)        1 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/zip-safe
+-rw-r--r--   0 nima       (501) staff       (20)     1069 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/SOURCES.txt
+-rw-r--r--   0 nima       (501) staff       (20)       55 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/entry_points.txt
+-rw-r--r--   0 nima       (501) staff       (20)        7 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/top_level.txt
+-rw-r--r--   0 nima       (501) staff       (20)        1 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/dependency_links.txt
+-rwxr-xr-x   0 nima       (501) staff       (20)     1871 2023-05-03 21:38:46.000000 pytube_local_nima-5.3.2023/setup.py
+-rw-r--r--   0 nima       (501) staff       (20)       38 2023-05-03 21:48:01.000000 pytube_local_nima-5.3.2023/setup.cfg
```

### Comparing `pytube_local_nima-12.1.3/PKG-INFO` & `pytube_local_nima-5.3.2023/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytube_local_nima
-Version: 12.1.3
+Version: 5.3.2023
 Summary: Python 3 library for downloading YouTube Videos.
 Home-page: https://github.com/nbehe/pytube_local_nima
 Author: Nima Beheshti
 License: The Unlicense (Unlicense)
 Description: 
         # This is a pytube fork created for specific purpose
         This fork was created for the specific purpose of fixing a pytube bug #1594. This fix will be used for my specific project. I have not done testing to ensure other functionality of the package still work with this change. If you decide to use please know their could be issues with the code not working properly going forward.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pytube_local_nima Version: 12.1.3 Summary: Python 3
-library for downloading YouTube Videos. Home-page: https://github.com/nbehe/
+Metadata-Version: 2.1 Name: pytube_local_nima Version: 5.3.2023 Summary: Python
+3 library for downloading YouTube Videos. Home-page: https://github.com/nbehe/
 pytube_local_nima Author: Nima Beheshti License: The Unlicense (Unlicense)
 Description: # This is a pytube fork created for specific purpose This fork was
 created for the specific purpose of fixing a pytube bug #1594. This fix will be
 used for my specific project. I have not done testing to ensure other
 functionality of the package still work with this change. If you decide to use
 please know their could be issues with the code not working properly going
 forward.
```

### Comparing `pytube_local_nima-12.1.3/LICENSE` & `pytube_local_nima-5.3.2023/LICENSE`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/innertube.py` & `pytube_local_nima-5.3.2023/pytube/innertube.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/streams.py` & `pytube_local_nima-5.3.2023/pytube/streams.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/metadata.py` & `pytube_local_nima-5.3.2023/pytube/metadata.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/query.py` & `pytube_local_nima-5.3.2023/pytube/query.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/request.py` & `pytube_local_nima-5.3.2023/pytube/request.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/__init__.py` & `pytube_local_nima-5.3.2023/pytube/__init__.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/contrib/channel.py` & `pytube_local_nima-5.3.2023/pytube/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/contrib/playlist.py` & `pytube_local_nima-5.3.2023/pytube/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/contrib/search.py` & `pytube_local_nima-5.3.2023/pytube/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/parser.py` & `pytube_local_nima-5.3.2023/pytube/parser.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/cipher.py` & `pytube_local_nima-5.3.2023/pytube/cipher.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/cli.py` & `pytube_local_nima-5.3.2023/pytube/cli.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/itags.py` & `pytube_local_nima-5.3.2023/pytube/itags.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/exceptions.py` & `pytube_local_nima-5.3.2023/pytube/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/captions.py` & `pytube_local_nima-5.3.2023/pytube/captions.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/helpers.py` & `pytube_local_nima-5.3.2023/pytube/helpers.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/extract.py` & `pytube_local_nima-5.3.2023/pytube/extract.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube/__main__.py` & `pytube_local_nima-5.3.2023/pytube/__main__.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_parser.py` & `pytube_local_nima-5.3.2023/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_streams.py` & `pytube_local_nima-5.3.2023/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_cipher.py` & `pytube_local_nima-5.3.2023/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/conftest.py` & `pytube_local_nima-5.3.2023/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_request.py` & `pytube_local_nima-5.3.2023/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_exceptions.py` & `pytube_local_nima-5.3.2023/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/contrib/test_channel.py` & `pytube_local_nima-5.3.2023/tests/contrib/test_channel.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/contrib/test_playlist.py` & `pytube_local_nima-5.3.2023/tests/contrib/test_playlist.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_query.py` & `pytube_local_nima-5.3.2023/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_helpers.py` & `pytube_local_nima-5.3.2023/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_extract.py` & `pytube_local_nima-5.3.2023/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_cli.py` & `pytube_local_nima-5.3.2023/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_main.py` & `pytube_local_nima-5.3.2023/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/tests/test_captions.py` & `pytube_local_nima-5.3.2023/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/README.md` & `pytube_local_nima-5.3.2023/README.md`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/pytube_local_nima.egg-info/PKG-INFO` & `pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytube-local-nima
-Version: 12.1.3
+Version: 5.3.2023
 Summary: Python 3 library for downloading YouTube Videos.
 Home-page: https://github.com/nbehe/pytube_local_nima
 Author: Nima Beheshti
 License: The Unlicense (Unlicense)
 Description: 
         # This is a pytube fork created for specific purpose
         This fork was created for the specific purpose of fixing a pytube bug #1594. This fix will be used for my specific project. I have not done testing to ensure other functionality of the package still work with this change. If you decide to use please know their could be issues with the code not working properly going forward.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: pytube-local-nima Version: 12.1.3 Summary: Python 3
-library for downloading YouTube Videos. Home-page: https://github.com/nbehe/
+Metadata-Version: 2.1 Name: pytube-local-nima Version: 5.3.2023 Summary: Python
+3 library for downloading YouTube Videos. Home-page: https://github.com/nbehe/
 pytube_local_nima Author: Nima Beheshti License: The Unlicense (Unlicense)
 Description: # This is a pytube fork created for specific purpose This fork was
 created for the specific purpose of fixing a pytube bug #1594. This fix will be
 used for my specific project. I have not done testing to ensure other
 functionality of the package still work with this change. If you decide to use
 please know their could be issues with the code not working properly going
 forward.
```

### Comparing `pytube_local_nima-12.1.3/pytube_local_nima.egg-info/SOURCES.txt` & `pytube_local_nima-5.3.2023/pytube_local_nima.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytube_local_nima-12.1.3/setup.py` & `pytube_local_nima-5.3.2023/setup.py`

 * *Files identical despite different names*

